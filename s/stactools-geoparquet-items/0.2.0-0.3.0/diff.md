# Comparing `tmp/stactools-geoparquet-items-0.2.0.tar.gz` & `tmp/stactools-geoparquet-items-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stactools-geoparquet-items-0.2.0.tar", last modified: Wed Jul 19 10:49:39 2023, max compression
+gzip compressed data, was "stactools-geoparquet-items-0.3.0.tar", last modified: Wed Jul 19 15:22:26 2023, max compression
```

## Comparing `stactools-geoparquet-items-0.2.0.tar` & `stactools-geoparquet-items-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:49:39.373247 stactools-geoparquet-items-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-19 10:49:21.000000 stactools-geoparquet-items-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-19 10:49:39.373247 stactools-geoparquet-items-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-07-19 10:49:21.000000 stactools-geoparquet-items-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-19 10:49:21.000000 stactools-geoparquet-items-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-19 10:49:39.373247 stactools-geoparquet-items-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:49:39.369248 stactools-geoparquet-items-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:49:39.369248 stactools-geoparquet-items-0.2.0/src/stactools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:49:39.369248 stactools-geoparquet-items-0.2.0/src/stactools/geoparquet_items/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-19 10:49:21.000000 stactools-geoparquet-items-0.2.0/src/stactools/geoparquet_items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-07-19 10:49:21.000000 stactools-geoparquet-items-0.2.0/src/stactools/geoparquet_items/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:49:39.373247 stactools-geoparquet-items-0.2.0/src/stactools_geoparquet_items.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-19 10:49:39.000000 stactools-geoparquet-items-0.2.0/src/stactools_geoparquet_items.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-19 10:49:39.000000 stactools-geoparquet-items-0.2.0/src/stactools_geoparquet_items.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 10:49:39.000000 stactools-geoparquet-items-0.2.0/src/stactools_geoparquet_items.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-19 10:49:39.000000 stactools-geoparquet-items-0.2.0/src/stactools_geoparquet_items.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-19 10:49:39.000000 stactools-geoparquet-items-0.2.0/src/stactools_geoparquet_items.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:22:26.176372 stactools-geoparquet-items-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-19 15:22:06.000000 stactools-geoparquet-items-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-07-19 15:22:26.176372 stactools-geoparquet-items-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-19 15:22:06.000000 stactools-geoparquet-items-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-19 15:22:06.000000 stactools-geoparquet-items-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-19 15:22:26.176372 stactools-geoparquet-items-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:22:26.176372 stactools-geoparquet-items-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:22:26.176372 stactools-geoparquet-items-0.3.0/src/stactools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:22:26.176372 stactools-geoparquet-items-0.3.0/src/stactools/geoparquet_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-19 15:22:06.000000 stactools-geoparquet-items-0.3.0/src/stactools/geoparquet_items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8839 2023-07-19 15:22:06.000000 stactools-geoparquet-items-0.3.0/src/stactools/geoparquet_items/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:22:26.176372 stactools-geoparquet-items-0.3.0/src/stactools_geoparquet_items.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-07-19 15:22:26.000000 stactools-geoparquet-items-0.3.0/src/stactools_geoparquet_items.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-19 15:22:26.000000 stactools-geoparquet-items-0.3.0/src/stactools_geoparquet_items.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 15:22:26.000000 stactools-geoparquet-items-0.3.0/src/stactools_geoparquet_items.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-19 15:22:26.000000 stactools-geoparquet-items-0.3.0/src/stactools_geoparquet_items.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-19 15:22:26.000000 stactools-geoparquet-items-0.3.0/src/stactools_geoparquet_items.egg-info/top_level.txt
```

### Comparing `stactools-geoparquet-items-0.2.0/LICENSE` & `stactools-geoparquet-items-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stactools-geoparquet-items-0.2.0/PKG-INFO` & `stactools-geoparquet-items-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stactools-geoparquet-items
-Version: 0.2.0
+Version: 0.3.0
 Summary: Uses stac-geoparquet to generate a geoparquet for a list of STAC items
 Home-page: https://github.com/stactools-packages/geoparquet-items
 Author: Matthias Mohr
 Author-email: matthias@mohr.ws
 Project-URL: Issues, https://github.com/stactools-packages/geoparquet-items/issues
 Keywords: stactools,pystac,catalog,STAC
 Classifier: Development Status :: 4 - Beta
@@ -63,14 +63,22 @@
 
 ```shell
 stac geoparquet-items convert source.geoparquet result.fgb --format flatgeobuf --exclude stac_version,type,assets,links,collection
 ```
 
 Supported formats: flatgeobuf, geojson, geojsonseq, gpkg (default), shapefile
 
+### Show information about geoparquet file
+
+You can easily retrieve metadata and a data excerpt:
+
+```shell
+stac geoparquet-items info source.geoparquet
+```
+
 ## Contributing
 
 We use [pre-commit](https://pre-commit.com/) to check any changes.
 To set up your development environment:
 
 ```shell
 pip install -e .
```

### Comparing `stactools-geoparquet-items-0.2.0/README.md` & `stactools-geoparquet-items-0.3.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -45,14 +45,22 @@
 
 ```shell
 stac geoparquet-items convert source.geoparquet result.fgb --format flatgeobuf --exclude stac_version,type,assets,links,collection
 ```
 
 Supported formats: flatgeobuf, geojson, geojsonseq, gpkg (default), shapefile
 
+### Show information about geoparquet file
+
+You can easily retrieve metadata and a data excerpt:
+
+```shell
+stac geoparquet-items info source.geoparquet
+```
+
 ## Contributing
 
 We use [pre-commit](https://pre-commit.com/) to check any changes.
 To set up your development environment:
 
 ```shell
 pip install -e .
```

### Comparing `stactools-geoparquet-items-0.2.0/setup.cfg` & `stactools-geoparquet-items-0.3.0/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -24,19 +24,22 @@
 
 [options]
 package_dir = 
 	= src
 packages = find_namespace:
 install_requires = 
 	stactools >= 0.4.0
-	stac-geoparquet >= 0.2.1
+	stac-geoparquet >= 0.3.2
 	requests >= 2.0.0
+	pathlib2 >= 2.3.6
 	pyogrio >= 0.6.0
-	geopandas >= 0.13.2
 	pyarrow >= 12.0.0
+	dask >= 2023.5.0
+	geopandas >= 0.13.2
+	dask-geopandas >= 0.3.1
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `stactools-geoparquet-items-0.2.0/src/stactools/geoparquet_items/commands.py` & `stactools-geoparquet-items-0.3.0/src/stactools/geoparquet_items/commands.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,22 @@
+import io
 import json
 import logging
 import os
-from typing import Optional
+
+# Used only for partitioning / dask variant
+import pathlib
+import shutil
+from typing import Any, Optional, Sequence
 
 import click
+import dask.bag as db
+import dask_geopandas
 import geopandas
+import pyarrow
 import pyarrow.parquet as pq
 import pyogrio
 import requests
 import stac_geoparquet
 from click import Command, Group
 
 logger = logging.getLogger(__name__)
@@ -30,61 +38,126 @@
     @click.argument("source")
     @click.argument("destination")
     @click.option(
         "--collection",
         default="",
         help="Adds a geoparquet asset to the Collection JSON at the given path.",
     )
-    def create_command(source: str, destination: str, collection: str = "") -> None:
+    @click.option(
+        "--partition",
+        default=1,
+        show_default=True,
+        help="Runs via dask and creates the number of partitions given (if >= 2)",
+    )
+    @click.option(
+        "--selflink",
+        default=False,
+        show_default=True,
+        help="Tries to add the absolute link to the source STAC Item to a column named 'self_link'",
+        is_flag=True,
+    )
+    def create_command(
+        source: str,
+        destination: str,
+        collection: str = "",
+        partition: int = 1,
+        selflink: bool = False,
+    ) -> None:
         """Create geoparquet from STAC Items
 
         Args:
             source (str): Link to a list of STAC Items (ItemCollection) or a folder with STAC files.
             destination (str): Path where the geoparquet file will be stored.
         """
+        p = pathlib.Path(destination)
+        if p.is_dir():
+            shutil.rmtree(p, ignore_errors=True)
+        else:
+            p.unlink(missing_ok=True)
+
+        if partition > 1:
+            p.mkdir()
+            print("Created destination folder")
 
         items = []
+        bag = None
         if source.startswith("https://") or source.startswith("http://"):
             print("Requesting remote source")
             response = requests.get(source)
             features = response.json().get("features")
             if features is not None:
                 items = features
+
+            if partition > 1:
+                bag = db.from_sequence(items, npartitions=partition)
+
         elif os.path.exists(source):
             print("Reading from file system")
             paths = []
             for root, _, files in os.walk(source):
                 for name in files:
                     if not name.endswith(".json"):
                         continue
                     elif name == "catalog.json" or name == "collection.json":
                         continue
                     else:
                         path = os.path.join(root, name)
-                        paths.append(path)
+                        paths.append(pathlib.Path(path))
 
             print("Found {} potential STAC Items".format(len(paths)))
 
-            for path in paths:
-                with open(path) as f:
+            if partition > 1:
+                bag = (
+                    db.from_sequence(paths, npartitions=partition)
+                    .map(lambda file: file.read_text())
+                    .map(json.loads)
+                    .filter(lambda item: item["type"] == "Feature")
+                )
+
+        def create_fn(items: Sequence[dict[str, Any]]) -> geopandas.GeoDataFrame:
+            return stac_geoparquet.to_geodataframe(items, add_self_link=selflink)
+
+        if bag is not None:
+            print("Initialized for parallel processing")
+            # Taken from Tom Augpurger's notbook at
+            # https://notebooksharing.space/view/1c2922b90622013d91dc22182e7f60d64e119c0f7cf1f977ccaa4dd0994bd1b6
+            sample = create_fn(bag.take(1))
+            meta = sample.iloc[:0, :]
+
+            dfs = bag.map_partitions(create_fn)
+            df = dask_geopandas.GeoDataFrame(
+                dfs.dask, dfs.name, meta, [None] * (dfs.npartitions + 1)
+            )
+
+            buf = io.BytesIO()
+            sample.to_parquet(buf, engine="pyarrow")
+            buf.seek(0)
+            schema = pq.read_schema(buf)
+
+            df.to_parquet(destination, schema=schema, write_index=False)
+            print("Wrote geoparquet file(s)")
+        else:
+            for p in paths:
+                with p.open() as f:
                     item = json.load(f)
                     if item["type"] == "Feature":
                         items.append(item)
+            del paths
 
-        num = len(items)
-        if num > 0:
-            print("Loaded {} actual STAC Items".format(num))
-            df = stac_geoparquet.to_geodataframe(items)
-            del items
-            print("Created dataframe")
-            df.to_parquet(destination)
-            del df
-            print("Wrote geoparquet file")
-        else:
-            raise Exception("No items found")
+            num = len(items)
+            if num > 0:
+                print(f"Loaded {num} actual STAC Items")
+                df = create_fn(items)
+                del items
+                print("Created dataframe")
+                df.to_parquet(destination)
+                del df
+                print("Wrote geoparquet file")
+            else:
+                raise Exception("Aborting, no items available")
 
         if len(collection) > 0:
             with open(collection, "r+") as f:
                 collection_json = json.load(f)
                 if "assets" not in collection_json:
                     collection_json["assets"] = {}
 
@@ -108,27 +181,28 @@
     )
     @click.argument("source")
     @click.argument("destination")
     @click.option(
         "--exclude",
         "-e",
         default=",".join(IGNORE_FIELDS),
+        show_default=True,
         help="A list of comma-separated fields that should be excluded from the target file. "
-        + " Use 'none' to include all fields. Default: "
-        + ",".join(IGNORE_FIELDS),
+        + " Use 'none' to include all fields."
     )
     @click.option(
         "--format",
         "-f",
         type=click.Choice(
             ["shapefile", "gpkg", "geojson", "geojsonseq", "flatgeobuf"],
             case_sensitive=False,
         ),
         default="gpkg",
-        help="File format to convert to. Default: gpkg",
+        show_default=True,
+        help="File format to convert to.",
     )
     def convert_command(
         source: str,
         destination: str,
         format: str = "gpkg",
         exclude: Optional[str] = None,
     ) -> None:
@@ -156,8 +230,41 @@
                 columns.remove(col.strip())
 
         df = geopandas.read_parquet(source, columns=columns)
         pyogrio.write_dataframe(df, destination, driver=format)
 
         return None
 
+    @geoparquetitems.command(
+        "info", short_help="Show some information about a geoparquet file"
+    )
+    @click.argument("source")
+    def info_command(source: str) -> None:
+        """Print some information about a geoparquet file
+
+        Args:
+            source (str): Path where the geoparquet file is located.
+        """
+        if not os.path.exists(source):
+            raise Exception("Source file does not exist")
+        
+        metadata = pq.read_metadata(source)
+        
+        print("Parquet Format Version:", metadata.format_version)
+        print("Created by:", metadata.created_by)
+        print("Columns:", metadata.num_columns, "(", ", ".join(metadata.schema.names), ")")
+        print("Rows/Items:", metadata.num_rows, "in", metadata.num_row_groups, "groups")
+        print("")
+
+        geo = json.loads(metadata.metadata[b"geo"])
+        print("GeoParquet metadata:", geo)
+        print("")
+
+        print("Excerpt:")
+        pf = pq.ParquetFile(source) 
+        rows = next(pf.iter_batches(batch_size = 10)) 
+        df = pyarrow.Table.from_batches([rows]).to_pandas()
+        print(df)
+
+        return None
+
     return geoparquetitems
```

### Comparing `stactools-geoparquet-items-0.2.0/src/stactools_geoparquet_items.egg-info/PKG-INFO` & `stactools-geoparquet-items-0.3.0/src/stactools_geoparquet_items.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stactools-geoparquet-items
-Version: 0.2.0
+Version: 0.3.0
 Summary: Uses stac-geoparquet to generate a geoparquet for a list of STAC items
 Home-page: https://github.com/stactools-packages/geoparquet-items
 Author: Matthias Mohr
 Author-email: matthias@mohr.ws
 Project-URL: Issues, https://github.com/stactools-packages/geoparquet-items/issues
 Keywords: stactools,pystac,catalog,STAC
 Classifier: Development Status :: 4 - Beta
@@ -63,14 +63,22 @@
 
 ```shell
 stac geoparquet-items convert source.geoparquet result.fgb --format flatgeobuf --exclude stac_version,type,assets,links,collection
 ```
 
 Supported formats: flatgeobuf, geojson, geojsonseq, gpkg (default), shapefile
 
+### Show information about geoparquet file
+
+You can easily retrieve metadata and a data excerpt:
+
+```shell
+stac geoparquet-items info source.geoparquet
+```
+
 ## Contributing
 
 We use [pre-commit](https://pre-commit.com/) to check any changes.
 To set up your development environment:
 
 ```shell
 pip install -e .
```

