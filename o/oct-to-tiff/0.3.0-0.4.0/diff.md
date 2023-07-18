# Comparing `tmp/oct_to_tiff-0.3.0.tar.gz` & `tmp/oct_to_tiff-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/oct-to-tiff/oct-to-tiff/dist/tmpq5xp21ud/oct_to_tiff-0.3.0.tar", last modified: Sun Nov 13 19:29:12 2022, max compression
+gzip compressed data, was "oct_to_tiff-0.4.0.tar", last modified: Tue Jul 18 22:21:20 2023, max compression
```

## Comparing `oct_to_tiff-0.3.0.tar` & `oct_to_tiff-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 19:29:12.000000 oct_to_tiff-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1521 2022-11-13 19:29:01.000000 oct_to_tiff-0.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3734 2022-11-13 19:29:12.000000 oct_to_tiff-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2829 2022-11-13 19:29:01.000000 oct_to_tiff-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-11-13 19:29:01.000000 oct_to_tiff-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1063 2022-11-13 19:29:12.000000 oct_to_tiff-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-13 19:29:01.000000 oct_to_tiff-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 19:29:12.000000 oct_to_tiff-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 19:29:12.000000 oct_to_tiff-0.3.0/src/oct_to_tiff/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-13 19:29:01.000000 oct_to_tiff-0.3.0/src/oct_to_tiff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14174 2022-11-13 19:29:01.000000 oct_to_tiff-0.3.0/src/oct_to_tiff/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 19:29:12.000000 oct_to_tiff-0.3.0/src/oct_to_tiff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3734 2022-11-13 19:29:12.000000 oct_to_tiff-0.3.0/src/oct_to_tiff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      342 2022-11-13 19:29:12.000000 oct_to_tiff-0.3.0/src/oct_to_tiff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-13 19:29:12.000000 oct_to_tiff-0.3.0/src/oct_to_tiff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-11-13 19:29:12.000000 oct_to_tiff-0.3.0/src/oct_to_tiff.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-11-13 19:29:12.000000 oct_to_tiff-0.3.0/src/oct_to_tiff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-11-13 19:29:12.000000 oct_to_tiff-0.3.0/src/oct_to_tiff.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:21:20.127637 oct_to_tiff-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-18 22:21:09.000000 oct_to_tiff-0.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-07-18 22:21:20.127637 oct_to_tiff-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-07-18 22:21:09.000000 oct_to_tiff-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-18 22:21:09.000000 oct_to_tiff-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-18 22:21:20.127637 oct_to_tiff-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 22:21:09.000000 oct_to_tiff-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:21:20.127637 oct_to_tiff-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:21:20.127637 oct_to_tiff-0.4.0/src/oct_to_tiff/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 22:21:09.000000 oct_to_tiff-0.4.0/src/oct_to_tiff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15115 2023-07-18 22:21:09.000000 oct_to_tiff-0.4.0/src/oct_to_tiff/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:21:20.127637 oct_to_tiff-0.4.0/src/oct_to_tiff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-07-18 22:21:20.000000 oct_to_tiff-0.4.0/src/oct_to_tiff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-18 22:21:20.000000 oct_to_tiff-0.4.0/src/oct_to_tiff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 22:21:20.000000 oct_to_tiff-0.4.0/src/oct_to_tiff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-18 22:21:20.000000 oct_to_tiff-0.4.0/src/oct_to_tiff.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-18 22:21:20.000000 oct_to_tiff-0.4.0/src/oct_to_tiff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-18 22:21:20.000000 oct_to_tiff-0.4.0/src/oct_to_tiff.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `oct_to_tiff-0.3.0/LICENSE.txt` & `oct_to_tiff-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `oct_to_tiff-0.3.0/PKG-INFO` & `oct_to_tiff-0.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: oct_to_tiff
-Version: 0.3.0
+Version: 0.4.0
 Summary: A command line tool for converting optical coherence tomography angiography (OCTA) data.
 Home-page: https://github.com/camlloyd/oct-to-tiff
 Author: Cameron Lloyd
 Author-email: lloyd@med.unideb.hu
 Project-URL: Bug Tracker, https://github.com/camlloyd/oct-to-tiff/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # oct-to-tiff
 
 [![DOI](https://zenodo.org/badge/382486199.svg)](https://zenodo.org/badge/latestdoi/382486199)
 
@@ -114,15 +114,15 @@
 #### `--version`
 **Description**: show program's version number and exit.
 
 **Usage**:
 
     oct-to-tiff --version
 
-#### The following options are currently experimental:
+#### The following options are mutually exclusive:
     
 #### `--angio`
 **Description**: convert extracted OCTA data. 
 
 Requires `--size SIZE`.
 
 **Usage**:
@@ -141,14 +141,21 @@
 #### `--seg-curve`
 **Description**: convert extracted segmentation data.
 
 **Usage**:
 
     oct-to-tiff /path/to/data --seg-curve
 
+#### `--boundaries`
+**Description**: extract segmentation lines.
+
+**Usage**:
+
+    oct-to-tiff /path/to/curve.xml --boundaries
+
 ## Contributing
 
 This project uses [black](https://github.com/psf/black) for formatting and [isort](https://github.com/PyCQA/isort) for sorting imports.
 
 ## Requirements
 
-Requires Python 3.7 or higher.
+Requires Python 3.8 or higher.
```

### Comparing `oct_to_tiff-0.3.0/README.md` & `oct_to_tiff-0.4.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 #### `--version`
 **Description**: show program's version number and exit.
 
 **Usage**:
 
     oct-to-tiff --version
 
-#### The following options are currently experimental:
+#### The following options are mutually exclusive:
     
 #### `--angio`
 **Description**: convert extracted OCTA data. 
 
 Requires `--size SIZE`.
 
 **Usage**:
@@ -119,14 +119,21 @@
 #### `--seg-curve`
 **Description**: convert extracted segmentation data.
 
 **Usage**:
 
     oct-to-tiff /path/to/data --seg-curve
 
+#### `--boundaries`
+**Description**: extract segmentation lines.
+
+**Usage**:
+
+    oct-to-tiff /path/to/curve.xml --boundaries
+
 ## Contributing
 
 This project uses [black](https://github.com/psf/black) for formatting and [isort](https://github.com/PyCQA/isort) for sorting imports.
 
 ## Requirements
 
-Requires Python 3.7 or higher.
+Requires Python 3.8 or higher.
```

### Comparing `oct_to_tiff-0.3.0/setup.cfg` & `oct_to_tiff-0.4.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oct_to_tiff
-version = 0.3.0
+version = 0.4.0
 author = Cameron Lloyd
 author_email = lloyd@med.unideb.hu
 description = A command line tool for converting optical coherence tomography angiography (OCTA) data.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/camlloyd/oct-to-tiff
 project_urls = 
@@ -12,24 +12,24 @@
 classifiers = 
 	Development Status :: 3 - Alpha
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: BSD License
 	Natural Language :: English
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 
 [options]
 packages = find:
 package_dir = 
 	=src
-python_requires = >=3.7
+python_requires = >=3.8
 install_requires = 
 	numpy
 	tifffile
 
 [options.entry_points]
 console_scripts = 
 	oct-to-tiff = oct_to_tiff.cli:main
```

### Comparing `oct_to_tiff-0.3.0/src/oct_to_tiff/cli.py` & `oct_to_tiff-0.4.0/src/oct_to_tiff/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,195 @@
 import argparse
 import logging
+import xml.etree.ElementTree as ET
 from pathlib import Path
 
 import numpy as np
 import tifffile
 
 logging.basicConfig(
     format="%(asctime)s %(name)s:%(funcName)s %(levelname)s - %(message)s"
 )
 logger = logging.getLogger(__name__)
 
 
-def convert_oct_file(args, file_name, input_path, output_path):
+def reshape_volume(
+    volume, frames_per_data_group, total_data_groups, oct_window_height, xy_scan_length
+):
+    """Reshape a 1-dimensional array to a 3-dimensional array.
+
+    Parameters
+    ----------
+    volume : ndarray
+        A 1-dimensional array.
+    frames_per_data_group : int
+        The number of frames per data group.
+    total_data_groups : int
+        The total number of data groups.
+    oct_window_height : int
+        The OCT window height.
+    xy_scan_length : int
+        The XY scan length.
+
+    Returns
+    -------
+    volume : ndarray
+        A 3-dimensional array.
+
+    """
+    volume = np.reshape(
+        volume,
+        (
+            frames_per_data_group * total_data_groups,
+            xy_scan_length,
+            oct_window_height,
+        ),
+    )
+    return volume
+
+
+def rotate_volume(volume):
+    """Rotate a 3-dimensional array 90 degrees left (anti-clockwise) about the z-axis.
+
+    Parameters
+    ----------
+    volume : ndarray
+        A 3-dimensional array.
+
+    Returns
+    -------
+    volume : ndarray
+        A rotated version of the input volume.
+
+    """
+    volume = np.rot90(volume, k=1, axes=(1, 2))
+    return volume
+
+
+def write_volume(output_path, volume, pixel_size_x, pixel_size_y, pixel_size_z):
+    """Write a 3-dimensional array to the output path as an OME-TIFF file, including voxel size in the metadata.
+
+    Parameters
+    ----------
+    output_path : Path
+        The specified output path.
+    volume : ndarray
+        A 3-dimensional array.
+    pixel_size_x : float
+        The pixel (voxel) width in mm.
+    pixel_size_y : float
+        The pixel (voxel) height in mm.
+    pixel_size_z : float
+        The pixel (voxel) depth in mm.
+
+    """
+    tifffile.imwrite(
+        output_path,
+        volume,
+        photometric="minisblack",
+        metadata={
+            "axes": "ZYX",
+            "PhysicalSizeX": pixel_size_x,
+            "PhysicalSizeXUnit": "mm",
+            "PhysicalSizeY": pixel_size_y,
+            "PhysicalSizeYUnit": "mm",
+            "PhysicalSizeZ": pixel_size_z,
+            "PhysicalSizeZUnit": "mm",
+        },
+    )
+
+
+def extract_boundaries(input_path):
+    """Extract segmentation lines.
+
+    Parameters
+    ----------
+    input_path : Path
+        The specified input path.
+
+    """
+    tree = ET.parse(input_path)
+    root = tree.getroot()
+
+    array_size = int(root.findtext("./Curve_Set/Image/Curve/ARRAY"))
+    data_points = [
+        int(point.text) for point in root.findall("./Curve_Set/Image/Curve/D")
+    ]
+    scan_length = np.arange(len(data_points))
+    num_files = len(data_points) // array_size
+    for i in range(num_files):
+        start = i * array_size
+        end = start + array_size
+        table = np.column_stack([scan_length[start:end], data_points[start:end]])
+        table_path = f"{input_path.parent}/{input_path.stem}_{i+1}.txt"
+        np.savetxt(table_path, table, delimiter="\t", fmt="%d")
+
+
+def main():
+    parser = argparse.ArgumentParser(
+        description="Convert optical coherence tomography angiography (OCTA) data."
+    )
+    parser.add_argument("input", type=Path, help="OCT file to convert")
+    parser.add_argument("--output", type=Path, help="specify a custom output directory")
+    parser.add_argument(
+        "--overwrite",
+        default=False,
+        action="store_true",
+        help="overwrite output file if it exists",
+    )
+    parser.add_argument("--size", type=float, help="scan size in mm")
+    group = parser.add_mutually_exclusive_group()
+    group.add_argument(
+        "--angio",
+        default=False,
+        action="store_true",
+        help="convert extracted OCTA data",
+    )
+    group.add_argument(
+        "--en-face",
+        default=False,
+        action="store_true",
+        help="convert extracted en face image",
+    )
+    group.add_argument(
+        "--seg-curve",
+        default=False,
+        action="store_true",
+        help="convert extracted segmentation data",
+    )
+    group.add_argument(
+        "--boundaries",
+        default=False,
+        action="store_true",
+        help="extract segmentation lines",
+    )
+    parser.add_argument("--version", action="version", version="%(prog)s 0.4.0")
+    args = parser.parse_args()
+
+    input_path = args.input
+    if args.output:
+        dir_name = args.output
+        dir_name.mkdir(parents=True, exist_ok=True)
+    else:
+        dir_name = input_path.parent
+    file_name = input_path.stem
+    file_extension = ".ome.tif"
+    output_path = dir_name / (file_name + file_extension)
+
+    if Path.is_file(output_path):
+        if args.overwrite:
+            pass
+        else:
+            logger.error(f"{output_path} already exists.")
+            return
+
+    if args.boundaries:
+        extract_boundaries(input_path)
+        return
+
     with open(input_path, "rb") as f:
         if args.angio and args.size:
             volume = np.frombuffer(f.read(), dtype=np.uint16)
             oct_window_height = 160
             frames_per_data_group = int((len(volume) // oct_window_height) ** 0.5)
             total_data_groups = 1
             xy_scan_length = int((len(volume) // oct_window_height) ** 0.5)
@@ -262,148 +436,9 @@
 
         if not args.en_face and not args.seg_curve:
             volume = rotate_volume(volume)
 
         write_volume(output_path, volume, pixel_size_x, pixel_size_y, pixel_size_z)
 
 
-def reshape_volume(
-    volume, frames_per_data_group, total_data_groups, oct_window_height, xy_scan_length
-):
-    """Reshape a 1-dimensional array to a 3-dimensional array.
-
-    Parameters
-    ----------
-    volume : ndarray
-        A 1-dimensional array.
-    frames_per_data_group : int
-        The number of frames per data group.
-    total_data_groups : int
-        The total number of data groups.
-    oct_window_height : int
-        The OCT window height.
-    xy_scan_length : int
-        The XY scan length.
-
-    Returns
-    -------
-    volume : ndarray
-        A 3-dimensional array.
-
-    """
-    volume = np.reshape(
-        volume,
-        (
-            frames_per_data_group * total_data_groups,
-            xy_scan_length,
-            oct_window_height,
-        ),
-    )
-    return volume
-
-
-def rotate_volume(volume):
-    """Rotate a 3-dimensional array 90 degrees left (anti-clockwise) about the z-axis.
-
-    Parameters
-    ----------
-    volume : ndarray
-        A 3-dimensional array.
-
-    Returns
-    -------
-    volume : ndarray
-        A rotated version of the input volume.
-
-    """
-    volume = np.rot90(volume, k=1, axes=(1, 2))
-    return volume
-
-
-def write_volume(output_path, volume, pixel_size_x, pixel_size_y, pixel_size_z):
-    """Write a 3-dimensional array to the output path as an OME-TIFF file, including voxel size in the metadata.
-
-    Parameters
-    ----------
-    output_path : Path
-        The specified output path.
-    volume : ndarray
-        A 3-dimensional array.
-    pixel_size_x : float
-        The pixel (voxel) width in mm.
-    pixel_size_y : float
-        The pixel (voxel) height in mm.
-    pixel_size_z : float
-        The pixel (voxel) depth in mm.
-
-    """
-    tifffile.imwrite(
-        output_path,
-        volume,
-        photometric="minisblack",
-        metadata={
-            "axes": "ZYX",
-            "PhysicalSizeX": pixel_size_x,
-            "PhysicalSizeXUnit": "mm",
-            "PhysicalSizeY": pixel_size_y,
-            "PhysicalSizeYUnit": "mm",
-            "PhysicalSizeZ": pixel_size_z,
-            "PhysicalSizeZUnit": "mm",
-        },
-    )
-
-
-def main():
-    parser = argparse.ArgumentParser(
-        description="Convert optical coherence tomography angiography (OCTA) data."
-    )
-    parser.add_argument("input", type=Path, help="OCT file to convert")
-    parser.add_argument("--output", type=Path, help="specify a custom output directory")
-    parser.add_argument(
-        "--overwrite",
-        default=False,
-        action="store_true",
-        help="overwrite output file if it exists",
-    )
-    parser.add_argument("--size", type=float, help="scan size in mm")
-    parser.add_argument(
-        "--angio",
-        default=False,
-        action="store_true",
-        help="convert extracted OCTA data",
-    )
-    parser.add_argument(
-        "--en-face",
-        default=False,
-        action="store_true",
-        help="convert extracted en face image",
-    )
-    parser.add_argument(
-        "--seg-curve",
-        default=False,
-        action="store_true",
-        help="convert extracted segmentation data",
-    )
-    parser.add_argument("--version", action="version", version="%(prog)s 0.3.0")
-    args = parser.parse_args()
-
-    input_path = args.input
-    if args.output:
-        dir_name = args.output
-        dir_name.mkdir(parents=True, exist_ok=True)
-    else:
-        dir_name = input_path.parent
-    file_name = input_path.stem
-    file_extension = ".ome.tif"
-    output_path = dir_name / (file_name + file_extension)
-
-    if Path.is_file(output_path):
-        if args.overwrite:
-            convert_oct_file(args, file_name, input_path, output_path)
-        else:
-            logger.error(f"{output_path} already exists.")
-    else:
-        convert_oct_file(args, file_name, input_path, output_path)
-
-
 if __name__ == "__main__":
     main()
```

### Comparing `oct_to_tiff-0.3.0/src/oct_to_tiff.egg-info/PKG-INFO` & `oct_to_tiff-0.4.0/src/oct_to_tiff.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: oct-to-tiff
-Version: 0.3.0
+Version: 0.4.0
 Summary: A command line tool for converting optical coherence tomography angiography (OCTA) data.
 Home-page: https://github.com/camlloyd/oct-to-tiff
 Author: Cameron Lloyd
 Author-email: lloyd@med.unideb.hu
 Project-URL: Bug Tracker, https://github.com/camlloyd/oct-to-tiff/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # oct-to-tiff
 
 [![DOI](https://zenodo.org/badge/382486199.svg)](https://zenodo.org/badge/latestdoi/382486199)
 
@@ -114,15 +114,15 @@
 #### `--version`
 **Description**: show program's version number and exit.
 
 **Usage**:
 
     oct-to-tiff --version
 
-#### The following options are currently experimental:
+#### The following options are mutually exclusive:
     
 #### `--angio`
 **Description**: convert extracted OCTA data. 
 
 Requires `--size SIZE`.
 
 **Usage**:
@@ -141,14 +141,21 @@
 #### `--seg-curve`
 **Description**: convert extracted segmentation data.
 
 **Usage**:
 
     oct-to-tiff /path/to/data --seg-curve
 
+#### `--boundaries`
+**Description**: extract segmentation lines.
+
+**Usage**:
+
+    oct-to-tiff /path/to/curve.xml --boundaries
+
 ## Contributing
 
 This project uses [black](https://github.com/psf/black) for formatting and [isort](https://github.com/PyCQA/isort) for sorting imports.
 
 ## Requirements
 
-Requires Python 3.7 or higher.
+Requires Python 3.8 or higher.
```

