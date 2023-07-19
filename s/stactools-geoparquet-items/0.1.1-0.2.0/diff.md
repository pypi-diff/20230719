# Comparing `tmp/stactools-geoparquet-items-0.1.1.tar.gz` & `tmp/stactools-geoparquet-items-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stactools-geoparquet-items-0.1.1.tar", last modified: Mon Jul  3 21:34:49 2023, max compression
+gzip compressed data, was "stactools-geoparquet-items-0.2.0.tar", last modified: Wed Jul 19 10:49:39 2023, max compression
```

## Comparing `stactools-geoparquet-items-0.1.1.tar` & `stactools-geoparquet-items-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 21:34:49.623260 stactools-geoparquet-items-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-03 21:34:33.000000 stactools-geoparquet-items-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-03 21:34:49.623260 stactools-geoparquet-items-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-03 21:34:33.000000 stactools-geoparquet-items-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-03 21:34:33.000000 stactools-geoparquet-items-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-03 21:34:49.623260 stactools-geoparquet-items-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 21:34:49.623260 stactools-geoparquet-items-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 21:34:49.619260 stactools-geoparquet-items-0.1.1/src/stactools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 21:34:49.623260 stactools-geoparquet-items-0.1.1/src/stactools/geoparquet_items/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-03 21:34:33.000000 stactools-geoparquet-items-0.1.1/src/stactools/geoparquet_items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-07-03 21:34:33.000000 stactools-geoparquet-items-0.1.1/src/stactools/geoparquet_items/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 21:34:49.623260 stactools-geoparquet-items-0.1.1/src/stactools_geoparquet_items.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-03 21:34:49.000000 stactools-geoparquet-items-0.1.1/src/stactools_geoparquet_items.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-03 21:34:49.000000 stactools-geoparquet-items-0.1.1/src/stactools_geoparquet_items.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 21:34:49.000000 stactools-geoparquet-items-0.1.1/src/stactools_geoparquet_items.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-03 21:34:49.000000 stactools-geoparquet-items-0.1.1/src/stactools_geoparquet_items.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-03 21:34:49.000000 stactools-geoparquet-items-0.1.1/src/stactools_geoparquet_items.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:49:39.373247 stactools-geoparquet-items-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-19 10:49:21.000000 stactools-geoparquet-items-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-19 10:49:39.373247 stactools-geoparquet-items-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-07-19 10:49:21.000000 stactools-geoparquet-items-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-19 10:49:21.000000 stactools-geoparquet-items-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-19 10:49:39.373247 stactools-geoparquet-items-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:49:39.369248 stactools-geoparquet-items-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:49:39.369248 stactools-geoparquet-items-0.2.0/src/stactools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:49:39.369248 stactools-geoparquet-items-0.2.0/src/stactools/geoparquet_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-19 10:49:21.000000 stactools-geoparquet-items-0.2.0/src/stactools/geoparquet_items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-07-19 10:49:21.000000 stactools-geoparquet-items-0.2.0/src/stactools/geoparquet_items/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:49:39.373247 stactools-geoparquet-items-0.2.0/src/stactools_geoparquet_items.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-19 10:49:39.000000 stactools-geoparquet-items-0.2.0/src/stactools_geoparquet_items.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-19 10:49:39.000000 stactools-geoparquet-items-0.2.0/src/stactools_geoparquet_items.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 10:49:39.000000 stactools-geoparquet-items-0.2.0/src/stactools_geoparquet_items.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-19 10:49:39.000000 stactools-geoparquet-items-0.2.0/src/stactools_geoparquet_items.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-19 10:49:39.000000 stactools-geoparquet-items-0.2.0/src/stactools_geoparquet_items.egg-info/top_level.txt
```

### Comparing `stactools-geoparquet-items-0.1.1/LICENSE` & `stactools-geoparquet-items-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stactools-geoparquet-items-0.1.1/PKG-INFO` & `stactools-geoparquet-items-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stactools-geoparquet-items
-Version: 0.1.1
+Version: 0.2.0
 Summary: Uses stac-geoparquet to generate a geoparquet for a list of STAC items
 Home-page: https://github.com/stactools-packages/geoparquet-items
 Author: Matthias Mohr
 Author-email: matthias@mohr.ws
 Project-URL: Issues, https://github.com/stactools-packages/geoparquet-items/issues
 Keywords: stactools,pystac,catalog,STAC
 Classifier: Development Status :: 4 - Beta
@@ -31,27 +31,45 @@
 
 ```shell
 pip install stactools-geoparquet-items
 ```
 
 ## Command-line Usage
 
+Use `stac geoparquet-items --help` to see all subcommands and options.
+
+### Create GeoParquet from STAC Items
+
 You need to provide a folder to read the items (deeply) from.
 Then you provide a file to write the geoparquet to.
 Optionally, you can add the geoparquet as an asset to a STAC Collection.
 
 ```shell
 stac geoparquet-items create https://example.com/collections/id/items result.geoparquet
 ```
 
 ```shell
 stac geoparquet-items create /path/to/folder result.geoparquet --collection /path/to/collection.json
 ```
 
-Use `stac geoparquet-items --help` to see all subcommands and options.
+### Convert from GeoParquet to other file formats
+
+Convert from geoparquet to GeoPackage (without stac_version, type and assets):
+
+```shell
+stac geoparquet-items convert source.geoparquet result.gpkg
+```
+
+Convert to FlatGeoBuf and exclude even more fields:
+
+```shell
+stac geoparquet-items convert source.geoparquet result.fgb --format flatgeobuf --exclude stac_version,type,assets,links,collection
+```
+
+Supported formats: flatgeobuf, geojson, geojsonseq, gpkg (default), shapefile
 
 ## Contributing
 
 We use [pre-commit](https://pre-commit.com/) to check any changes.
 To set up your development environment:
 
 ```shell
```

### Comparing `stactools-geoparquet-items-0.1.1/README.md` & `stactools-geoparquet-items-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -13,27 +13,45 @@
 
 ```shell
 pip install stactools-geoparquet-items
 ```
 
 ## Command-line Usage
 
+Use `stac geoparquet-items --help` to see all subcommands and options.
+
+### Create GeoParquet from STAC Items
+
 You need to provide a folder to read the items (deeply) from.
 Then you provide a file to write the geoparquet to.
 Optionally, you can add the geoparquet as an asset to a STAC Collection.
 
 ```shell
 stac geoparquet-items create https://example.com/collections/id/items result.geoparquet
 ```
 
 ```shell
 stac geoparquet-items create /path/to/folder result.geoparquet --collection /path/to/collection.json
 ```
 
-Use `stac geoparquet-items --help` to see all subcommands and options.
+### Convert from GeoParquet to other file formats
+
+Convert from geoparquet to GeoPackage (without stac_version, type and assets):
+
+```shell
+stac geoparquet-items convert source.geoparquet result.gpkg
+```
+
+Convert to FlatGeoBuf and exclude even more fields:
+
+```shell
+stac geoparquet-items convert source.geoparquet result.fgb --format flatgeobuf --exclude stac_version,type,assets,links,collection
+```
+
+Supported formats: flatgeobuf, geojson, geojsonseq, gpkg (default), shapefile
 
 ## Contributing
 
 We use [pre-commit](https://pre-commit.com/) to check any changes.
 To set up your development environment:
 
 ```shell
```

### Comparing `stactools-geoparquet-items-0.1.1/setup.cfg` & `stactools-geoparquet-items-0.2.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -26,14 +26,17 @@
 package_dir = 
 	= src
 packages = find_namespace:
 install_requires = 
 	stactools >= 0.4.0
 	stac-geoparquet >= 0.2.1
 	requests >= 2.0.0
+	pyogrio >= 0.6.0
+	geopandas >= 0.13.2
+	pyarrow >= 12.0.0
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `stactools-geoparquet-items-0.1.1/src/stactools_geoparquet_items.egg-info/PKG-INFO` & `stactools-geoparquet-items-0.2.0/src/stactools_geoparquet_items.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stactools-geoparquet-items
-Version: 0.1.1
+Version: 0.2.0
 Summary: Uses stac-geoparquet to generate a geoparquet for a list of STAC items
 Home-page: https://github.com/stactools-packages/geoparquet-items
 Author: Matthias Mohr
 Author-email: matthias@mohr.ws
 Project-URL: Issues, https://github.com/stactools-packages/geoparquet-items/issues
 Keywords: stactools,pystac,catalog,STAC
 Classifier: Development Status :: 4 - Beta
@@ -31,27 +31,45 @@
 
 ```shell
 pip install stactools-geoparquet-items
 ```
 
 ## Command-line Usage
 
+Use `stac geoparquet-items --help` to see all subcommands and options.
+
+### Create GeoParquet from STAC Items
+
 You need to provide a folder to read the items (deeply) from.
 Then you provide a file to write the geoparquet to.
 Optionally, you can add the geoparquet as an asset to a STAC Collection.
 
 ```shell
 stac geoparquet-items create https://example.com/collections/id/items result.geoparquet
 ```
 
 ```shell
 stac geoparquet-items create /path/to/folder result.geoparquet --collection /path/to/collection.json
 ```
 
-Use `stac geoparquet-items --help` to see all subcommands and options.
+### Convert from GeoParquet to other file formats
+
+Convert from geoparquet to GeoPackage (without stac_version, type and assets):
+
+```shell
+stac geoparquet-items convert source.geoparquet result.gpkg
+```
+
+Convert to FlatGeoBuf and exclude even more fields:
+
+```shell
+stac geoparquet-items convert source.geoparquet result.fgb --format flatgeobuf --exclude stac_version,type,assets,links,collection
+```
+
+Supported formats: flatgeobuf, geojson, geojsonseq, gpkg (default), shapefile
 
 ## Contributing
 
 We use [pre-commit](https://pre-commit.com/) to check any changes.
 To set up your development environment:
 
 ```shell
```

