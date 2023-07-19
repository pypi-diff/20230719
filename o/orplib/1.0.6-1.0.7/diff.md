# Comparing `tmp/orplib-1.0.6.tar.gz` & `tmp/orplib-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orplib-1.0.6.tar", last modified: Tue Jun  6 16:13:54 2023, max compression
+gzip compressed data, was "orplib-1.0.7.tar", last modified: Wed Jul 19 15:24:48 2023, max compression
```

## Comparing `orplib-1.0.6.tar` & `orplib-1.0.7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 gsheehy   (1000) gsheehy   (1000)        0 2023-06-06 16:13:54.625627 orplib-1.0.6/
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)       23 2023-05-11 21:09:19.000000 orplib-1.0.6/MANIFEST.in
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     7207 2023-06-06 16:13:54.625627 orplib-1.0.6/PKG-INFO
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     6777 2023-05-11 21:32:45.000000 orplib-1.0.6/README.md
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)      101 2023-04-14 19:45:52.000000 orplib-1.0.6/pyproject.toml
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)      821 2023-06-06 16:13:54.625627 orplib-1.0.6/setup.cfg
-drwxr-xr-x   0 gsheehy   (1000) gsheehy   (1000)        0 2023-06-06 16:13:54.622627 orplib-1.0.6/src/
-drwxr-xr-x   0 gsheehy   (1000) gsheehy   (1000)        0 2023-06-06 16:13:54.624627 orplib-1.0.6/src/orpl/
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)      317 2023-05-12 18:34:44.000000 orplib-1.0.6/src/orpl/__init__.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)       89 2023-06-06 16:02:21.000000 orplib-1.0.6/src/orpl/__main__.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)    15209 2023-04-14 19:45:52.000000 orplib-1.0.6/src/orpl/baseline_removal.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)    16694 2023-04-14 19:45:52.000000 orplib-1.0.6/src/orpl/bubblegif.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     8250 2023-04-14 19:45:52.000000 orplib-1.0.6/src/orpl/calibration.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     3772 2023-04-14 19:45:52.000000 orplib-1.0.6/src/orpl/cosmic_ray.py
-drwxr-xr-x   0 gsheehy   (1000) gsheehy   (1000)        0 2023-06-06 16:13:54.624627 orplib-1.0.6/src/orpl/data/
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)        0 2023-04-14 19:45:52.000000 orplib-1.0.6/src/orpl/data/__init__.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)    63150 2023-04-14 19:45:52.000000 orplib-1.0.6/src/orpl/data/synthetic_presets.json
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     1163 2023-06-06 16:05:52.000000 orplib-1.0.6/src/orpl/datatypes.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)    10430 2023-06-06 16:05:49.000000 orplib-1.0.6/src/orpl/file_io.py
-drwxr-xr-x   0 gsheehy   (1000) gsheehy   (1000)        0 2023-06-06 16:13:54.624627 orplib-1.0.6/src/orpl/gui/
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)        0 2023-04-14 19:45:52.000000 orplib-1.0.6/src/orpl/gui/__init__.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     1100 2023-04-14 19:45:52.000000 orplib-1.0.6/src/orpl/gui/mplcanvas.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)    28411 2023-06-06 16:05:46.000000 orplib-1.0.6/src/orpl/gui/orplGUI.py
-drwxr-xr-x   0 gsheehy   (1000) gsheehy   (1000)        0 2023-06-06 16:13:54.624627 orplib-1.0.6/src/orpl/gui/uis/
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)        0 2023-04-14 19:45:52.000000 orplib-1.0.6/src/orpl/gui/uis/__init__.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)    30648 2023-06-06 15:27:30.000000 orplib-1.0.6/src/orpl/gui/uis/ui_mainWindow.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     1846 2023-04-14 19:45:52.000000 orplib-1.0.6/src/orpl/metrics.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     2135 2023-04-14 19:45:52.000000 orplib-1.0.6/src/orpl/normalization.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)       92 2023-04-14 19:45:52.000000 orplib-1.0.6/src/orpl/pipelines.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     4566 2023-04-14 19:45:52.000000 orplib-1.0.6/src/orpl/plot.py
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     7014 2023-04-14 19:45:52.000000 orplib-1.0.6/src/orpl/synthetic.py
-drwxr-xr-x   0 gsheehy   (1000) gsheehy   (1000)        0 2023-06-06 16:13:54.625627 orplib-1.0.6/src/orplib.egg-info/
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     7207 2023-06-06 16:13:54.000000 orplib-1.0.6/src/orplib.egg-info/PKG-INFO
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)      705 2023-06-06 16:13:54.000000 orplib-1.0.6/src/orplib.egg-info/SOURCES.txt
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)        1 2023-06-06 16:13:54.000000 orplib-1.0.6/src/orplib.egg-info/dependency_links.txt
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)      161 2023-06-06 16:13:54.000000 orplib-1.0.6/src/orplib.egg-info/requires.txt
--rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)        5 2023-06-06 16:13:54.000000 orplib-1.0.6/src/orplib.egg-info/top_level.txt
+drwxr-xr-x   0 gsheehy   (1000) gsheehy   (1000)        0 2023-07-19 15:24:48.798419 orplib-1.0.7/
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)       23 2023-05-11 21:09:19.000000 orplib-1.0.7/MANIFEST.in
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     7207 2023-07-19 15:24:48.798419 orplib-1.0.7/PKG-INFO
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     6777 2023-05-11 21:32:45.000000 orplib-1.0.7/README.md
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)      101 2023-04-14 19:45:52.000000 orplib-1.0.7/pyproject.toml
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)      821 2023-07-19 15:24:48.799419 orplib-1.0.7/setup.cfg
+drwxr-xr-x   0 gsheehy   (1000) gsheehy   (1000)        0 2023-07-19 15:24:48.748419 orplib-1.0.7/src/
+drwxr-xr-x   0 gsheehy   (1000) gsheehy   (1000)        0 2023-07-19 15:24:48.778419 orplib-1.0.7/src/orpl/
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)      317 2023-05-12 18:34:44.000000 orplib-1.0.7/src/orpl/__init__.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)       89 2023-06-06 16:02:21.000000 orplib-1.0.7/src/orpl/__main__.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)    15209 2023-04-14 19:45:52.000000 orplib-1.0.7/src/orpl/baseline_removal.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)    16694 2023-04-14 19:45:52.000000 orplib-1.0.7/src/orpl/bubblegif.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     8250 2023-04-14 19:45:52.000000 orplib-1.0.7/src/orpl/calibration.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     3772 2023-04-14 19:45:52.000000 orplib-1.0.7/src/orpl/cosmic_ray.py
+drwxr-xr-x   0 gsheehy   (1000) gsheehy   (1000)        0 2023-07-19 15:24:48.779419 orplib-1.0.7/src/orpl/data/
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)        0 2023-04-14 19:45:52.000000 orplib-1.0.7/src/orpl/data/__init__.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)    63150 2023-04-14 19:45:52.000000 orplib-1.0.7/src/orpl/data/synthetic_presets.json
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     1163 2023-06-06 16:05:52.000000 orplib-1.0.7/src/orpl/datatypes.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)    10916 2023-06-29 13:55:16.000000 orplib-1.0.7/src/orpl/file_io.py
+drwxr-xr-x   0 gsheehy   (1000) gsheehy   (1000)        0 2023-07-19 15:24:48.779419 orplib-1.0.7/src/orpl/gui/
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)        0 2023-04-14 19:45:52.000000 orplib-1.0.7/src/orpl/gui/__init__.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     1100 2023-04-14 19:45:52.000000 orplib-1.0.7/src/orpl/gui/mplcanvas.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)    28572 2023-06-20 20:29:22.000000 orplib-1.0.7/src/orpl/gui/orplGUI.py
+drwxr-xr-x   0 gsheehy   (1000) gsheehy   (1000)        0 2023-07-19 15:24:48.779419 orplib-1.0.7/src/orpl/gui/uis/
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)        0 2023-04-14 19:45:52.000000 orplib-1.0.7/src/orpl/gui/uis/__init__.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)    30648 2023-06-06 15:27:30.000000 orplib-1.0.7/src/orpl/gui/uis/ui_mainWindow.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     1846 2023-04-14 19:45:52.000000 orplib-1.0.7/src/orpl/metrics.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     2135 2023-04-14 19:45:52.000000 orplib-1.0.7/src/orpl/normalization.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)       92 2023-04-14 19:45:52.000000 orplib-1.0.7/src/orpl/pipelines.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     4566 2023-04-14 19:45:52.000000 orplib-1.0.7/src/orpl/plot.py
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     7014 2023-04-14 19:45:52.000000 orplib-1.0.7/src/orpl/synthetic.py
+drwxr-xr-x   0 gsheehy   (1000) gsheehy   (1000)        0 2023-07-19 15:24:48.798419 orplib-1.0.7/src/orplib.egg-info/
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)     7207 2023-07-19 15:24:48.000000 orplib-1.0.7/src/orplib.egg-info/PKG-INFO
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)      705 2023-07-19 15:24:48.000000 orplib-1.0.7/src/orplib.egg-info/SOURCES.txt
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)        1 2023-07-19 15:24:48.000000 orplib-1.0.7/src/orplib.egg-info/dependency_links.txt
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)      161 2023-07-19 15:24:48.000000 orplib-1.0.7/src/orplib.egg-info/requires.txt
+-rw-r--r--   0 gsheehy   (1000) gsheehy   (1000)        5 2023-07-19 15:24:48.000000 orplib-1.0.7/src/orplib.egg-info/top_level.txt
```

### Comparing `orplib-1.0.6/PKG-INFO` & `orplib-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orplib
-Version: 1.0.6
+Version: 1.0.7
 Summary: Open Raman Processing Library
 Home-page: https://github.com/mr-sheg/orpl
 Author: Guillaume Sheehy
 Author-email: guillaume.sheehy@polymtl.ca
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `orplib-1.0.6/README.md` & `orplib-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `orplib-1.0.6/setup.cfg` & `orplib-1.0.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = orplib
-version = 1.0.6
+version = 1.0.7
 author = Guillaume Sheehy
 author_email = guillaume.sheehy@polymtl.ca
 description = Open Raman Processing Library
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT License
 url = https://github.com/mr-sheg/orpl
```

### Comparing `orplib-1.0.6/src/orpl/baseline_removal.py` & `orplib-1.0.7/src/orpl/baseline_removal.py`

 * *Files identical despite different names*

### Comparing `orplib-1.0.6/src/orpl/bubblegif.py` & `orplib-1.0.7/src/orpl/bubblegif.py`

 * *Files identical despite different names*

### Comparing `orplib-1.0.6/src/orpl/calibration.py` & `orplib-1.0.7/src/orpl/calibration.py`

 * *Files identical despite different names*

### Comparing `orplib-1.0.6/src/orpl/cosmic_ray.py` & `orplib-1.0.7/src/orpl/cosmic_ray.py`

 * *Files identical despite different names*

### Comparing `orplib-1.0.6/src/orpl/data/synthetic_presets.json` & `orplib-1.0.7/src/orpl/data/synthetic_presets.json`

 * *Files identical despite different names*

### Comparing `orplib-1.0.6/src/orpl/datatypes.py` & `orplib-1.0.7/src/orpl/datatypes.py`

 * *Files identical despite different names*

### Comparing `orplib-1.0.6/src/orpl/file_io.py` & `orplib-1.0.7/src/orpl/file_io.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,35 +11,15 @@
 import pandas as pd
 import sif_parser
 from renishawWiRE import WDFReader
 from ruamel import yaml
 
 from orpl.datatypes import Acquisition_info, Rdf_metadata, Spectrum
 
-SUPPORTED_EXTENSIONS = [".sif", ".json", ".wdf", ".sdf"]
-
-
-def is_file_supported(file_path: Path) -> bool:
-    return file_path.suffix in SUPPORTED_EXTENSIONS
-
-
-def load_file(file_name: str) -> Spectrum:
-    file_path = Path(file_name)
-    if not is_file_supported(file_path):
-        raise TypeError(f"{file_path} is not supported as a spectrum file.")
-
-    load_function = {
-        ".sif": load_sif,
-        ".json": load_json,
-        ".wdf": load_wdf,
-        ".sdf": load_sdf,
-    }
-    spectrum = load_function[file_path.suffix](file_path)
-
-    return spectrum
+## File specific load functions
 
 
 def load_sif(sif_file: Path) -> Spectrum:
     data_array, meta_dict = sif_parser.np_open(sif_file)
     data_array = np.squeeze(data_array).T
     if data_array.ndim > 1:
         data_array = np.flip(data_array, axis=0)
@@ -54,15 +34,15 @@
     metadata = Rdf_metadata(
         filepath=sif_file,
         source_power=None,
         exposure_time=meta_dict["CycleTime"],
         details=dict(meta_dict),
         comment="",
     )
-    spectrum = Spectrum(accumulations=data_array, metadata=metadata, background=None)
+    spectrum = Spectrum(accumulations=data_array, background=None, metadata=metadata)
 
     return spectrum
 
 
 def load_json(json_file: Path) -> Spectrum:
     with open(json_file, encoding="utf8") as f:
         json_data = json.load(f)
@@ -192,14 +172,57 @@
 
     spectrum = Spectrum(
         accumulations=accumulations, background=background, metadata=metadata
     )
     return spectrum
 
 
+def load_txt(txt_file: Path) -> Spectrum:
+    data = np.genfromtxt(txt_file, delimiter=",", skip_header=1)
+    xaxis = data[:, 0]
+    background = data[:, 1]
+    accumulations = data[:, 2:]
+    metadata = Rdf_metadata(
+        filepath=txt_file,
+        exposure_time=np.nan,
+        source_power=np.nan,
+        details={},
+        comment="",
+    )
+    spectrum = Spectrum(
+        accumulations=accumulations, background=background, metadata=metadata
+    )
+
+    return spectrum
+
+
+LOAD_FUNCTIONS = {
+    ".sif": load_sif,
+    ".json": load_json,
+    ".wdf": load_wdf,
+    ".sdf": load_sdf,
+    ".csv": load_txt,
+    ".txt": load_txt,
+}
+
+
+def is_file_supported(file_path: Path) -> bool:
+    return file_path.suffix in LOAD_FUNCTIONS.keys()
+
+
+def load_file(file_name: str) -> Spectrum:
+    file_path = Path(file_name)
+    if not is_file_supported(file_path):
+        raise TypeError(f"{file_path} is not supported as a spectrum file.")
+
+    spectrum = LOAD_FUNCTIONS[file_path.suffix](file_path)
+
+    return spectrum
+
+
 class RDF:
     metadata: Type[Rdf_metadata]
     xaxis: Type[np.ndarray]
     raman: Type[np.ndarray]
     baseline: Type[np.ndarray]
 
     def get_metadata_string(self) -> str:
@@ -337,11 +360,12 @@
             k: self.__dict__[k] for k in self.__meta_attrs__() + self.__data_attrs__()
         }
 
         return pd.Series(data)
 
 
 if __name__ == "__main__":
-    sdf_file = Path().home() / "oras/2023_05_26_10_28/acquisition/acquisition_0.sdf"
-    s = load_file(sdf_file)
+    file2load = Path().cwd() / "sample data/Generic/collagen.csv"
+    print(file2load)
 
+    s = load_file(file2load)
     print(s)
```

### Comparing `orplib-1.0.6/src/orpl/gui/mplcanvas.py` & `orplib-1.0.7/src/orpl/gui/mplcanvas.py`

 * *Files identical despite different names*

### Comparing `orplib-1.0.6/src/orpl/gui/orplGUI.py` & `orplib-1.0.7/src/orpl/gui/orplGUI.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,14 +96,15 @@
 
 
 class main_window(Ui_mainWindow, QMainWindow):
     def __init__(self):
         super().__init__()
 
         # Internal references
+        self.working_directory = Path().cwd()
         self.raw_spectra: List[np.ndarray] = []
         self.baseline_spectra: List[np.ndarray] = []
         self.irf_corrections: List[np.ndarray] = []
         self.raman_spectra = None
         self.xaxis: Spectrum = None
         self.irf: Spectrum = None
         self.auto_update_processing: bool = False
@@ -135,16 +136,18 @@
     def defaultSetup(self):
         # window setup
         self.setWindowTitle(f"ORPL GUI - {ORPL_VERSION}")
 
         # File IO tab
         self.file_system_model.setRootPath("/")
         self.treeViewFiles.setModel(self.file_system_model)
-        self.treeViewFiles.setRootIndex(self.file_system_model.index(str(HOME_DIR)))
-        self.textEditDataDir.setText(str(HOME_DIR))
+        self.treeViewFiles.setRootIndex(
+            self.file_system_model.index(str(self.working_directory))
+        )
+        self.textEditDataDir.setText(str(self.working_directory))
 
         pixmapi = getattr(QStyle, "SP_TrashIcon")
         trash_icon = self.style().standardIcon(pixmapi)
         self.buttonDropSpectra.setIcon(trash_icon)
         self.buttonDropXref.setIcon(trash_icon)
         self.buttonDropYref.setIcon(trash_icon)
 
@@ -154,15 +157,15 @@
         self.spinBoxSCRRWidth.setValue(3)
         self.spinBoxSCRRstd.setValue(5)
         self.spinBoxPolyOrder.setValue(6)
         self.spinBoxHWS.setMaximum(1024)
         self.spinBoxHWS.setValue(100)
         self.spinBoxBubbleWidth.setMaximum(1024)
         self.spinBoxBubbleWidth.setValue(200)
-        self.textEditExportDir.setText(str(HOME_DIR))
+        self.textEditExportDir.setText(str(self.working_directory))
 
         # Log
         self.labelLogPath.setText(str(LOG_PATH))
         logger.info("setted default logTab setup")
 
     def setupPlots(self):
         self.boxDataSelection.setLayout(self.currentSpectrumPlot.createLayout())
@@ -254,14 +257,15 @@
     def select_working_directory(self):
         options = QFileDialog.Options()
         new_dir = QFileDialog.getExistingDirectory(
             self, options=options, directory=self.textEditDataDir.text()
         )
 
         if new_dir:
+            self.working_directory = Path(new_dir)
             self.treeViewFiles.setRootIndex(self.file_system_model.index(new_dir))
             self.textEditDataDir.setText(new_dir)
             self.textEditExportDir.setText(new_dir)
 
         logger.info("Changed data directory - %s", new_dir)
 
     def load_spectra(self):
```

### Comparing `orplib-1.0.6/src/orpl/gui/uis/ui_mainWindow.py` & `orplib-1.0.7/src/orpl/gui/uis/ui_mainWindow.py`

 * *Files identical despite different names*

### Comparing `orplib-1.0.6/src/orpl/metrics.py` & `orplib-1.0.7/src/orpl/metrics.py`

 * *Files identical despite different names*

### Comparing `orplib-1.0.6/src/orpl/normalization.py` & `orplib-1.0.7/src/orpl/normalization.py`

 * *Files identical despite different names*

### Comparing `orplib-1.0.6/src/orpl/plot.py` & `orplib-1.0.7/src/orpl/plot.py`

 * *Files identical despite different names*

### Comparing `orplib-1.0.6/src/orpl/synthetic.py` & `orplib-1.0.7/src/orpl/synthetic.py`

 * *Files identical despite different names*

### Comparing `orplib-1.0.6/src/orplib.egg-info/PKG-INFO` & `orplib-1.0.7/src/orplib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orplib
-Version: 1.0.6
+Version: 1.0.7
 Summary: Open Raman Processing Library
 Home-page: https://github.com/mr-sheg/orpl
 Author: Guillaume Sheehy
 Author-email: guillaume.sheehy@polymtl.ca
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `orplib-1.0.6/src/orplib.egg-info/SOURCES.txt` & `orplib-1.0.7/src/orplib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

