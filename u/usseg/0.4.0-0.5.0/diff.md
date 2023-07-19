# Comparing `tmp/usseg-0.4.0.tar.gz` & `tmp/usseg-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usseg-0.4.0.tar", max compression
+gzip compressed data, was "usseg-0.5.0.tar", max compression
```

## Comparing `usseg-0.4.0.tar` & `usseg-0.5.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     3203 2023-05-18 17:29:24.569730 usseg-0.4.0/README.md
--rw-r--r--   0        0        0      710 2023-06-29 13:02:56.462211 usseg-0.4.0/pyproject.toml
--rw-r--r--   0        0        0    54798 2023-06-29 13:02:03.831335 usseg-0.4.0/usseg/General_functions.py
--rw-r--r--   0        0        0     4117 2023-06-29 13:02:03.831335 usseg-0.4.0/usseg/Organise_files.py
--rw-r--r--   0        0        0    11591 2023-06-29 13:02:03.831335 usseg-0.4.0/usseg/Refined_anon_2_html.py
--rw-r--r--   0        0        0     5240 2023-06-29 13:02:03.831335 usseg-0.4.0/usseg/Single_image_processing.py
--rw-r--r--   0        0        0      361 2023-06-29 13:02:03.831335 usseg-0.4.0/usseg/__init__.py
--rw-r--r--   0        0        0      771 2023-06-29 13:02:03.831335 usseg-0.4.0/usseg/example.py
--rw-r--r--   0        0        0      878 2023-06-29 13:02:03.831335 usseg-0.4.0/usseg/main.py
--rw-r--r--   0        0        0     4993 2023-06-29 13:02:03.831335 usseg-0.4.0/usseg/visualisation_html.py
--rw-r--r--   0        0        0     4190 1970-01-01 00:00:00.000000 usseg-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     3203 2023-05-18 17:29:24.569730 usseg-0.5.0/README.md
+-rw-r--r--   0        0        0      710 2023-07-19 08:41:01.228873 usseg-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0    54791 2023-06-29 15:10:01.142427 usseg-0.5.0/usseg/#General_functions.py#
+-rw-r--r--   0        0        0    54835 2023-07-19 08:37:32.321865 usseg-0.5.0/usseg/General_functions.py
+-rw-r--r--   0        0        0     4117 2023-06-29 13:02:03.831335 usseg-0.5.0/usseg/Organise_files.py
+-rw-r--r--   0        0        0    11644 2023-07-19 08:37:32.321865 usseg-0.5.0/usseg/Refined_anon_2_html.py
+-rw-r--r--   0        0        0     5204 2023-07-19 08:37:32.321865 usseg-0.5.0/usseg/Single_image_processing.py
+-rw-r--r--   0        0        0      361 2023-06-29 13:02:03.831335 usseg-0.5.0/usseg/__init__.py
+-rw-r--r--   0        0        0      771 2023-06-29 13:02:03.831335 usseg-0.5.0/usseg/example.py
+-rw-r--r--   0        0        0      878 2023-06-29 13:02:03.831335 usseg-0.5.0/usseg/main.py
+-rw-r--r--   0        0        0     4993 2023-06-29 13:02:03.831335 usseg-0.5.0/usseg/visualisation_html.py
+-rw-r--r--   0        0        0     4190 1970-01-01 00:00:00.000000 usseg-0.5.0/PKG-INFO
```

### Comparing `usseg-0.4.0/README.md` & `usseg-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `usseg-0.4.0/pyproject.toml` & `usseg-0.5.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "usseg"
-version = "0.4.0"
+version = "0.5.0"
 description = "Tools to segment doppler ultrasound signals from scan images."
 authors = ["Dale Kernot <874043@swansea.ac.uk>"]
 license = "GPL-v3-or-later"
 readme = "README.md"
 packages = [{include = "usseg"}]
 
 [tool.poetry.dependencies]
```

### Comparing `usseg-0.4.0/usseg/General_functions.py` & `usseg-0.5.0/usseg/#General_functions.py#`

 * *Files 1% similar despite different names*

```diff
@@ -258,18 +258,17 @@
 
     # Checks if waveforms are inverted, if so gets the bottom of the curve
     if check_inverted_curve(top_curve_mask, Ymax, Ymin):
         top_curve_mask = refined_segmentation_mask - ws
         for x in range(0, int(rp[0].centroid[0])):
             top_curve_mask[x, :] = 0
 
-    o = list(zip(*np.nonzero(top_curve_mask)))
-    np.savetxt("test1.txt", o, fmt="%d")
+    top_curve_coords  = list(zip(*np.nonzero(top_curve_mask)))
 
-    return refined_segmentation_mask, top_curve_mask
+    return refined_segmentation_mask, top_curve_mask, top_curve_coords
 
 def Search_for_ticks(input_image_obj, Side, Left_dimensions, Right_dimensions):
     """
     Function to search for the ticks in either of the axes ROIs
 
     Args:
         input_image_filename (str) : Name of file within current directory, or path to a file.
```

### Comparing `usseg-0.4.0/usseg/Organise_files.py` & `usseg-0.5.0/usseg/Organise_files.py`

 * *Files identical despite different names*

### Comparing `usseg-0.4.0/usseg/Refined_anon_2_html.py` & `usseg-0.5.0/usseg/Refined_anon_2_html.py`

 * *Files 2% similar despite different names*

```diff
@@ -236,28 +236,31 @@
             traceback.print_exc()  # prints the error message and traceback
             print("Failed Axes search")
             
             Fail = Fail + 1
             pass
 
         try:
-            Xplot, Yplot, Ynought = General_functions.Plot_Digitized_data(
-                Rticks=Rnumber, Rlocs=Rpositions, Lticks=Lnumber, Llocs=Lpositions
-            )
-            
             try:  # Refine segmentation
-                refined_segmentation_mask, top_curve_mask = General_functions.Segment_refinement(
+                (
+                    refined_segmentation_mask, top_curve_mask, top_curve_coords
+                ) = General_functions.Segment_refinement(
                     cv2_img, Xmin, Xmax, Ymin, Ymax
                 )
             except Exception:
                 traceback.print_exc()  # prints the error message and traceback
                 print("Failed Segment refinement")
                 Fail = Fail + 1
                 pass
 
+            Xplot, Yplot, Ynought = General_functions.Plot_Digitized_data(
+                Rnumber, Rpositions, Lnumber, Lpositions, top_curve_coords,
+            )
+            
+
             col = General_functions.Annotate(
                 input_image_obj=colRGBA,
                 refined_segmentation_mask=refined_segmentation_mask,
                 Left_dimensions=Left_dimensions,
                 Right_dimensions=Right_dimensions,
                 Waveform_dimensions=Waveform_dimensions,
                 Left_axis=ROIL,
@@ -279,14 +282,15 @@
                 traceback.print_exc()
                 print("Failed correction")
                 continue
             Digitized_path = output_dir + image_name.partition(".")[0] + "_Digitized.png"
             plt.figure(2)
             plt.savefig(Digitized_path, dpi=900, bbox_inches="tight", pad_inches=0)
             Digitized_scans.append(Digitized_path)
+
         except Exception:
             print("Failed Digitization")
             Annotated_scans.append(None)
             traceback.print_exc()
             try:
                 Text_data.append(df)
             except Exception:
```

### Comparing `usseg-0.4.0/usseg/Single_image_processing.py` & `usseg-0.5.0/usseg/Single_image_processing.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,47 +136,49 @@
     except Exception:
         traceback.print_exc()  # prints the error message and traceback
         print("Failed Axes search")
         
         Fail = Fail + 1
         pass
 
-    try:
+    try:  # Refine segmentation
+        (
+            refined_segmentation_mask, top_curve_mask, top_curve_coords
+        ) = General_functions.Segment_refinement(
+            cv2_img, Xmin, Xmax, Ymin, Ymax
+        )
+    except Exception:
+        traceback.print_exc()  # prints the error message and traceback
+        print("Failed Segment refinement")
+        Fail = Fail + 1
+        pass
+
+    try: 
         Xplot, Yplot, Ynought = General_functions.Plot_Digitized_data(
-            Rticks=Rnumber, Rlocs=Rpositions, Lticks=Lnumber, Llocs=Lpositions
+            Rnumber, Rpositions, Lnumber, Lpositions, top_curve_coords,
         )
-        
-        try:  # Refine segmentation
-            refined_segmentation_mask, top_curve_mask = General_functions.Segment_refinement(
-                cv2_img, Xmin, Xmax, Ymin, Ymax
-            )
-        except Exception:
-            traceback.print_exc()  # prints the error message and traceback
-            print("Failed Segment refinement")
-            Fail = Fail + 1
-            pass
 
-        try:
-            df = General_functions.Plot_correction(Xplot, Yplot, df)
-            Text_data.append(df)
-        except Exception:
-            traceback.print_exc()
-            print("Failed correction")
-            pass
     except Exception:
         print("Failed Digitization")
         traceback.print_exc()
         try:
             Text_data.append(df)
         except Exception:
             traceback.print_exc()
             Text_data.append(None)
         Fail = Fail + 1
         pass
 
+    try:
+        df = General_functions.Plot_correction(Xplot, Yplot, df)
+        Text_data.append(df)
+    except Exception:
+        traceback.print_exc()
+        print("Failed correction")
+        pass
     to_del = [
         "df",
         "image_name",
         "Xmax",
         "Xmin",
         "Ymax",
         "Ymin",
```

### Comparing `usseg-0.4.0/usseg/example.py` & `usseg-0.5.0/usseg/example.py`

 * *Files identical despite different names*

### Comparing `usseg-0.4.0/usseg/main.py` & `usseg-0.5.0/usseg/main.py`

 * *Files identical despite different names*

### Comparing `usseg-0.4.0/usseg/visualisation_html.py` & `usseg-0.5.0/usseg/visualisation_html.py`

 * *Files identical despite different names*

### Comparing `usseg-0.4.0/PKG-INFO` & `usseg-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usseg
-Version: 0.4.0
+Version: 0.5.0
 Summary: Tools to segment doppler ultrasound signals from scan images.
 License: GPL-v3-or-later
 Author: Dale Kernot
 Author-email: 874043@swansea.ac.uk
 Requires-Python: >=3.10,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

