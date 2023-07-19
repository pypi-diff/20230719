# Comparing `tmp/ezgpx-0.1.1.tar.gz` & `tmp/ezgpx-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezgpx-0.1.1.tar", last modified: Tue Jul 18 12:29:51 2023, max compression
+gzip compressed data, was "ezgpx-0.1.2.tar", last modified: Wed Jul 19 14:55:09 2023, max compression
```

## Comparing `ezgpx-0.1.1.tar` & `ezgpx-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2023-07-18 12:29:51.776976 ezgpx-0.1.1/
--rw-rw-r--   0 fabien    (1000) fabien    (1000)    35149 2023-06-06 11:52:29.000000 ezgpx-0.1.1/LICENSE
--rw-rw-r--   0 fabien    (1000) fabien    (1000)     2111 2023-07-18 12:29:51.776976 ezgpx-0.1.1/PKG-INFO
--rw-rw-r--   0 fabien    (1000) fabien    (1000)     1243 2023-07-16 16:02:43.000000 ezgpx-0.1.1/README.md
-drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2023-07-18 12:29:51.776976 ezgpx-0.1.1/ezgpx/
--rw-rw-r--   0 fabien    (1000) fabien    (1000)       98 2023-06-08 09:27:44.000000 ezgpx-0.1.1/ezgpx/__init__.py
-drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2023-07-18 12:29:51.776976 ezgpx-0.1.1/ezgpx.egg-info/
--rw-rw-r--   0 fabien    (1000) fabien    (1000)     2111 2023-07-18 12:29:51.000000 ezgpx-0.1.1/ezgpx.egg-info/PKG-INFO
--rw-rw-r--   0 fabien    (1000) fabien    (1000)      226 2023-07-18 12:29:51.000000 ezgpx-0.1.1/ezgpx.egg-info/SOURCES.txt
--rw-rw-r--   0 fabien    (1000) fabien    (1000)        1 2023-07-18 12:29:51.000000 ezgpx-0.1.1/ezgpx.egg-info/dependency_links.txt
--rw-rw-r--   0 fabien    (1000) fabien    (1000)       12 2023-07-18 12:29:51.000000 ezgpx-0.1.1/ezgpx.egg-info/requires.txt
--rw-rw-r--   0 fabien    (1000) fabien    (1000)        6 2023-07-18 12:29:51.000000 ezgpx-0.1.1/ezgpx.egg-info/top_level.txt
--rw-rw-r--   0 fabien    (1000) fabien    (1000)       38 2023-07-18 12:29:51.776976 ezgpx-0.1.1/setup.cfg
--rw-rw-r--   0 fabien    (1000) fabien    (1000)     1642 2023-07-18 09:45:47.000000 ezgpx-0.1.1/setup.py
-drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2023-07-18 12:29:51.776976 ezgpx-0.1.1/tests/
--rw-rw-r--   0 fabien    (1000) fabien    (1000)     3193 2023-07-18 12:25:14.000000 ezgpx-0.1.1/tests/test_GPX.py
--rw-rw-r--   0 fabien    (1000) fabien    (1000)     1747 2023-07-18 12:27:24.000000 ezgpx-0.1.1/tests/test_utils.py
+drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2023-07-19 14:55:09.013672 ezgpx-0.1.2/
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)    35149 2023-06-06 11:52:29.000000 ezgpx-0.1.2/LICENSE
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)     2158 2023-07-19 14:55:09.009672 ezgpx-0.1.2/PKG-INFO
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)     1179 2023-07-19 12:57:20.000000 ezgpx-0.1.2/README.md
+drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2023-07-19 14:55:09.009672 ezgpx-0.1.2/ezgpx/
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)       98 2023-06-08 09:27:44.000000 ezgpx-0.1.2/ezgpx/__init__.py
+drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2023-07-19 14:55:09.009672 ezgpx-0.1.2/ezgpx.egg-info/
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)     2158 2023-07-19 14:55:08.000000 ezgpx-0.1.2/ezgpx.egg-info/PKG-INFO
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)      226 2023-07-19 14:55:08.000000 ezgpx-0.1.2/ezgpx.egg-info/SOURCES.txt
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)        1 2023-07-19 14:55:08.000000 ezgpx-0.1.2/ezgpx.egg-info/dependency_links.txt
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)       12 2023-07-19 14:55:08.000000 ezgpx-0.1.2/ezgpx.egg-info/requires.txt
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)        6 2023-07-19 14:55:08.000000 ezgpx-0.1.2/ezgpx.egg-info/top_level.txt
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)       38 2023-07-19 14:55:09.013672 ezgpx-0.1.2/setup.cfg
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)     1643 2023-07-19 14:54:51.000000 ezgpx-0.1.2/setup.py
+drwxrwxr-x   0 fabien    (1000) fabien    (1000)        0 2023-07-19 14:55:09.009672 ezgpx-0.1.2/tests/
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)     3193 2023-07-18 12:25:14.000000 ezgpx-0.1.2/tests/test_GPX.py
+-rw-rw-r--   0 fabien    (1000) fabien    (1000)     1747 2023-07-18 12:27:24.000000 ezgpx-0.1.2/tests/test_utils.py
```

### Comparing `ezgpx-0.1.1/LICENSE` & `ezgpx-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ezgpx-0.1.1/PKG-INFO` & `ezgpx-0.1.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: ezgpx
-Version: 0.1.1
+Version: 0.1.2
 Summary: Easy to use Python GPX library
+Home-page: https://pypi.org/project/ezgpx/
 Download-URL: https://github.com/FABallemand/ezGPX
 Author: Fabien ALLEMAND
 Author-email: allemand.fabien@orange.fr
 License: GNU GPLv3
 Project-URL: Bug Tracker, https://github.com/FABallemand/ezGPX/issues
+Project-URL: Documentation, https://ezgpx.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/FABallemand/ezGPX
 Keywords: gpx,gpx-files,gpx-parser,gpx-reader,gpx-writer,gpx-data
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -21,14 +23,19 @@
 License-File: LICENSE
 
 # 🗺️ ezGPX
 
 ## 🔎 Description
 Easy to use Python GPX library.
 
+- PyPi: https://pypi.org/project/ezgpx/
+- Documentation: https://ezgpx.readthedocs.io/en/latest/
+- Source code: https://github.com/FABallemand/ezGPX
+- Bug reports: https://github.com/FABallemand/ezGPX/issues
+
 ## 🛠️ Installation
 
 ```bash
 pip install ezgpx
 ```
 
 ## 🏁 Get started
@@ -39,35 +46,32 @@
 # Parse GPX file
 gpx = ezgpx.GPX("file.gpx")
 
 # Simplify (using Ramer-Dougle-Peucker algorithm)
 gpx.simplify()
 
 # Plot with Matplotlib
-gpx.matplotlib_plot(title="Track", base_color="#FF0000",
-                    start_stop=True, way_points=False, file_path="img_1")
-
-# Plot with Matplotlib Basemap Toolkit
-gpx.matplotlib_basemap_plot(title="Track", base_color="#00FF00",
-                            start_stop=False, way_points=False, file_path="img_2")
-
-# Plot with gmap (Google Maps)
-gpx.gmap_plot(title="Track", base_color="#0000FF", start_stop=True,
-              way_points=True, file_path="map_1.html", open=True)
-
-# Plot with Folium
-gpx.folium_plot(title="Track", tiles="OpenStreetMap", base_color="#000000", start_stop=True,
-                way_points=True, minimap=True, coord_popup=True, file_path="map_2.html", open=True)
+gpx.matplotlib_plot(elevation_color=True,
+                    start_stop_colors=("green", "red"),
+                    way_points_color="blue",
+                    title=gpx.name(),
+                    duration=(0, 0),
+                    distance=(0.5, 0),
+                    ascent=None,
+                    pace=(1, 0),
+                    speed=None,
+                    file_path="img_1")
 
 # Remove metadata
 gpx.remove_metadata()
 
 # Write new simplified GPX file
 gpx.to_gpx("new_file.gpx")
 ```
+![](img/matplotlib_plot_1.png)
 
 ## 📚 References:
 
 ### 🧭 Other Python GPX Library
 - [gpxpy](https://github.com/tkrajina/gpxpy)
 
 ## 👤 Author
```

### Comparing `ezgpx-0.1.1/ezgpx.egg-info/PKG-INFO` & `ezgpx-0.1.2/ezgpx.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: ezgpx
-Version: 0.1.1
+Version: 0.1.2
 Summary: Easy to use Python GPX library
+Home-page: https://pypi.org/project/ezgpx/
 Download-URL: https://github.com/FABallemand/ezGPX
 Author: Fabien ALLEMAND
 Author-email: allemand.fabien@orange.fr
 License: GNU GPLv3
 Project-URL: Bug Tracker, https://github.com/FABallemand/ezGPX/issues
+Project-URL: Documentation, https://ezgpx.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/FABallemand/ezGPX
 Keywords: gpx,gpx-files,gpx-parser,gpx-reader,gpx-writer,gpx-data
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -21,14 +23,19 @@
 License-File: LICENSE
 
 # 🗺️ ezGPX
 
 ## 🔎 Description
 Easy to use Python GPX library.
 
+- PyPi: https://pypi.org/project/ezgpx/
+- Documentation: https://ezgpx.readthedocs.io/en/latest/
+- Source code: https://github.com/FABallemand/ezGPX
+- Bug reports: https://github.com/FABallemand/ezGPX/issues
+
 ## 🛠️ Installation
 
 ```bash
 pip install ezgpx
 ```
 
 ## 🏁 Get started
@@ -39,35 +46,32 @@
 # Parse GPX file
 gpx = ezgpx.GPX("file.gpx")
 
 # Simplify (using Ramer-Dougle-Peucker algorithm)
 gpx.simplify()
 
 # Plot with Matplotlib
-gpx.matplotlib_plot(title="Track", base_color="#FF0000",
-                    start_stop=True, way_points=False, file_path="img_1")
-
-# Plot with Matplotlib Basemap Toolkit
-gpx.matplotlib_basemap_plot(title="Track", base_color="#00FF00",
-                            start_stop=False, way_points=False, file_path="img_2")
-
-# Plot with gmap (Google Maps)
-gpx.gmap_plot(title="Track", base_color="#0000FF", start_stop=True,
-              way_points=True, file_path="map_1.html", open=True)
-
-# Plot with Folium
-gpx.folium_plot(title="Track", tiles="OpenStreetMap", base_color="#000000", start_stop=True,
-                way_points=True, minimap=True, coord_popup=True, file_path="map_2.html", open=True)
+gpx.matplotlib_plot(elevation_color=True,
+                    start_stop_colors=("green", "red"),
+                    way_points_color="blue",
+                    title=gpx.name(),
+                    duration=(0, 0),
+                    distance=(0.5, 0),
+                    ascent=None,
+                    pace=(1, 0),
+                    speed=None,
+                    file_path="img_1")
 
 # Remove metadata
 gpx.remove_metadata()
 
 # Write new simplified GPX file
 gpx.to_gpx("new_file.gpx")
 ```
+![](img/matplotlib_plot_1.png)
 
 ## 📚 References:
 
 ### 🧭 Other Python GPX Library
 - [gpxpy](https://github.com/tkrajina/gpxpy)
 
 ## 👤 Author
```

### Comparing `ezgpx-0.1.1/setup.py` & `ezgpx-0.1.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 
 # Get the long description from the README file
 with open(os.path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='ezgpx',
-    version='0.1.1',
+    version='0.1.2',
     description='Easy to use Python GPX library',
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords=['gpx', 'gpx-files', 'gpx-parser', 'gpx-reader', 'gpx-writer', 'gpx-data'],
-    # url='https://medium-multiply.readthedocs.io/',
+    url='https://pypi.org/project/ezgpx/',
     download_url='https://github.com/FABallemand/ezGPX',
     project_urls={
             "Bug Tracker": "https://github.com/FABallemand/ezGPX/issues",
-            # "Documentation": "",
+            "Documentation": "https://ezgpx.readthedocs.io/en/latest/",
             "Source Code": "https://github.com/FABallemand/ezGPX",
         },
     author='Fabien ALLEMAND',
     author_email='allemand.fabien@orange.fr',
     license='GNU GPLv3',
     classifiers=[
         'Intended Audience :: Developers',
@@ -32,15 +32,14 @@
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Operating System :: OS Independent'
     ],
-    # packages=find_packages(include=['ezgpx']),
-    packages=['ezgpx'],
+    packages=find_packages(include=['ezgpx']),
     include_package_data=True,
     install_requires=['gmap', 'folium'],
     setup_requires=['pytest-runner'],
     tests_require=['pytest'],
     test_suite='tests'
 )
```

### Comparing `ezgpx-0.1.1/tests/test_GPX.py` & `ezgpx-0.1.2/tests/test_GPX.py`

 * *Files identical despite different names*

### Comparing `ezgpx-0.1.1/tests/test_utils.py` & `ezgpx-0.1.2/tests/test_utils.py`

 * *Files identical despite different names*

