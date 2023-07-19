# Comparing `tmp/stac_geoparquet-0.2.1.tar.gz` & `tmp/stac_geoparquet-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac_geoparquet-0.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "stac_geoparquet-0.3.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `stac_geoparquet-0.2.1.tar` & `stac_geoparquet-0.3.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1081 2023-05-26 14:30:16.179537 stac_geoparquet-0.2.1/LICENSE
--rw-r--r--   0        0        0     1810 2023-05-26 14:30:16.179537 stac_geoparquet-0.2.1/README.md
--rw-r--r--   0        0        0     1275 2023-05-26 14:30:16.179537 stac_geoparquet-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      199 2023-05-26 14:30:16.179537 stac_geoparquet-0.2.1/stac_geoparquet/__init__.py
--rw-r--r--   0        0        0      143 2023-05-26 14:30:16.179537 stac_geoparquet-0.2.1/stac_geoparquet/_compat.py
--rw-r--r--   0        0        0     3823 2023-05-26 14:30:16.179537 stac_geoparquet-0.2.1/stac_geoparquet/cli.py
--rw-r--r--   0        0        0     4455 2023-05-26 14:30:16.179537 stac_geoparquet-0.2.1/stac_geoparquet/pc_runner.py
--rw-r--r--   0        0        0    12037 2023-05-26 14:30:16.179537 stac_geoparquet-0.2.1/stac_geoparquet/pgstac_reader.py
--rw-r--r--   0        0        0     3817 2023-05-26 14:30:16.179537 stac_geoparquet-0.2.1/stac_geoparquet/stac_geoparquet.py
--rw-r--r--   0        0        0     2480 2023-05-26 14:30:16.179537 stac_geoparquet-0.2.1/stac_geoparquet/utils.py
--rw-r--r--   0        0        0     2911 1970-01-01 00:00:00.000000 stac_geoparquet-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-07-19 14:16:30.017598 stac_geoparquet-0.3.2/LICENSE
+-rw-r--r--   0        0        0     1810 2023-07-19 14:16:30.017598 stac_geoparquet-0.3.2/README.md
+-rw-r--r--   0        0        0     1331 2023-07-19 14:16:30.017598 stac_geoparquet-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      199 2023-07-19 14:16:30.017598 stac_geoparquet-0.3.2/stac_geoparquet/__init__.py
+-rw-r--r--   0        0        0      143 2023-07-19 14:16:30.017598 stac_geoparquet-0.3.2/stac_geoparquet/_compat.py
+-rw-r--r--   0        0        0     3823 2023-07-19 14:16:30.017598 stac_geoparquet-0.3.2/stac_geoparquet/cli.py
+-rw-r--r--   0        0        0     4455 2023-07-19 14:16:30.017598 stac_geoparquet-0.3.2/stac_geoparquet/pc_runner.py
+-rw-r--r--   0        0        0    12086 2023-07-19 14:16:30.017598 stac_geoparquet-0.3.2/stac_geoparquet/pgstac_reader.py
+-rw-r--r--   0        0        0        0 2023-07-19 14:16:30.017598 stac_geoparquet-0.3.2/stac_geoparquet/py.typed
+-rw-r--r--   0        0        0     4952 2023-07-19 14:16:30.017598 stac_geoparquet-0.3.2/stac_geoparquet/stac_geoparquet.py
+-rw-r--r--   0        0        0     2480 2023-07-19 14:16:30.017598 stac_geoparquet-0.3.2/stac_geoparquet/utils.py
+-rw-r--r--   0        0        0     3018 1970-01-01 00:00:00.000000 stac_geoparquet-0.3.2/PKG-INFO
```

### Comparing `stac_geoparquet-0.2.1/LICENSE` & `stac_geoparquet-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `stac_geoparquet-0.2.1/README.md` & `stac_geoparquet-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `stac_geoparquet-0.2.1/pyproject.toml` & `stac_geoparquet-0.3.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -33,20 +33,22 @@
     "psycopg[binary,pool]",
     "tqdm",
     "azure-data-tables",
 ]
 test = [
     "pytest",
     "requests",
-    "pre-commit"
+    "pre-commit",
+    "stac-geoparquet[pgstac]",
+    "stac-geoparquet[pc]",
 ]
 
 
 [project.urls]
-Home = "https://github.com/TomAugspurger/stac_geoparquet"
+Home = "https://github.com/stac-utils/stac-geoparquet"
 
 [project.scripts]
 pc-geoparquet = "stac_geoparquet.cli:main"
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 filterwarnings = [
```

### Comparing `stac_geoparquet-0.2.1/stac_geoparquet/cli.py` & `stac_geoparquet-0.3.2/stac_geoparquet/cli.py`

 * *Files identical despite different names*

### Comparing `stac_geoparquet-0.2.1/stac_geoparquet/pc_runner.py` & `stac_geoparquet-0.3.2/stac_geoparquet/pc_runner.py`

 * *Files identical despite different names*

### Comparing `stac_geoparquet-0.2.1/stac_geoparquet/pgstac_reader.py` & `stac_geoparquet-0.3.2/stac_geoparquet/pgstac_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -317,15 +317,16 @@
             assert isinstance(content, dict)
             if "bbox" in content:
                 item["bbox"] = content["bbox"]
             else:
                 item["bbox"] = list(geom.bounds)
 
             item["assets"] = content["assets"]
-            item["stac_extensions"] = content["stac_extensions"]
+            if "stac_extensions" in content:
+                item["stac_extensions"] = content["stac_extensions"]
             item["properties"] = content["properties"]
 
             pypgstac.hydration.hydrate(base_item, item)
 
             if self.should_inject_dynamic_properties:
                 self.inject_links(item)
                 self.inject_assets(item)
```

### Comparing `stac_geoparquet-0.2.1/stac_geoparquet/stac_geoparquet.py` & `stac_geoparquet-0.3.2/stac_geoparquet/stac_geoparquet.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,49 +7,69 @@
 
 import pystac
 import geopandas
 import pandas as pd
 import numpy as np
 import shapely.geometry
 
+from urllib.parse import urlparse
+
 from stac_geoparquet.utils import fix_empty_multipolygon
 
+STAC_ITEM_TYPES = ["application/json", "application/geo+json"]
+
+SELF_LINK_COLUMN = "self_link"
+
 
 def _fix_array(v):
     if isinstance(v, np.ndarray):
         v = v.tolist()
 
     elif isinstance(v, dict):
         v = {k: _fix_array(v2) for k, v2 in v.items()}
 
     return v
 
 
-def to_geodataframe(items: Sequence[dict[str, Any]]) -> geopandas.GeoDataFrame:
+def to_geodataframe(
+    items: Sequence[dict[str, Any]], add_self_link: bool = False
+) -> geopandas.GeoDataFrame:
     """
     Convert a sequence of STAC items to a :class:`geopandas.GeoDataFrame`.
 
     The objects under `properties` are moved up to the top-level of the
     DataFrame, similar to :meth:`geopandas.GeoDataFrame.from_features`.
 
     Parameters
     ----------
     items: A sequence of STAC items.
+    add_self_link: Add the absolute link (if available) to the source STAC Item as a separate column named "self_link"
 
     Returns
     -------
     The converted GeoDataFrame.
     """
     items2 = []
     for item in items:
         item2 = {k: v for k, v in item.items() if k != "properties"}
         for k, v in item["properties"].items():
             if k in item2:
                 raise ValueError("k", k)
             item2[k] = v
+        if add_self_link:
+            self_href = None
+            for link in item["links"]:
+                if (
+                    link["rel"] == "self"
+                    and (not link["type"] or link["type"] in STAC_ITEM_TYPES)
+                    and urlparse(link["href"]).netloc
+                ):
+                    self_href = link["href"]
+                    break
+            item2[SELF_LINK_COLUMN] = self_href
         items2.append(item2)
 
     # Filter out missing geoms in MultiPolygons
     # https://github.com/shapely/shapely/issues/1407
     # geometry = [shapely.geometry.shape(x["geometry"]) for x in items2]
 
     geometry = []
@@ -57,32 +77,47 @@
         item_geometry = item2["geometry"]
         if item_geometry:
             item_geometry = fix_empty_multipolygon(item_geometry)  # type: ignore
         geometry.append(item_geometry)
 
     gdf = geopandas.GeoDataFrame(items2, geometry=geometry, crs="WGS84")
 
-    for column in ["datetime", "start_datetime", "end_datetime"]:
+    for column in [
+        "datetime",  # common metadata
+        "start_datetime",
+        "end_datetime",
+        "created",
+        "updated",
+        "expires",  # timestamps extension
+        "published",
+        "unpublished",
+    ]:
         if column in gdf.columns:
             gdf[column] = pd.to_datetime(gdf[column], format="ISO8601")
 
     columns = [
         "type",
         "stac_version",
         "stac_extensions",
         "id",
         "geometry",
         "bbox",
         "links",
         "assets",
         "collection",
     ]
+    opt_columns = ["stac_extensions", "collection"]
+    for col in opt_columns:
+        if col not in gdf.columns:
+            columns.remove(col)
+
     gdf = pd.concat([gdf[columns], gdf.drop(columns=columns)], axis="columns")
-    for k in ["type", "stac_version", "id", "collection"]:
-        gdf[k] = gdf[k].astype("string")
+    for k in ["type", "stac_version", "id", "collection", SELF_LINK_COLUMN]:
+        if k in gdf:
+            gdf[k] = gdf[k].astype("string")
 
     return gdf
 
 
 def to_dict(record: dict) -> dict:
     """
     Create a dictionary representing a STAC item from a row of the GeoDataFrame.
@@ -103,15 +138,17 @@
         "collection",
         "stac_extensions",
     }
     item = {}
     for k, v in record.items():
         v = _fix_array(v)
 
-        if k in top_level_keys:
+        if k == SELF_LINK_COLUMN:
+            continue
+        elif k in top_level_keys:
             item[k] = v
         else:
             properties[k] = v
 
     item["geometry"] = shapely.geometry.mapping(item["geometry"])
     item["properties"] = properties
```

### Comparing `stac_geoparquet-0.2.1/stac_geoparquet/utils.py` & `stac_geoparquet-0.3.2/stac_geoparquet/utils.py`

 * *Files identical despite different names*

### Comparing `stac_geoparquet-0.2.1/PKG-INFO` & `stac_geoparquet-0.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac_geoparquet
-Version: 0.2.1
+Version: 0.3.2
 Summary: stac-geoparquet
 Author-email: Tom Augspurger <taugspurger@microsoft.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: pystac
 Requires-Dist: geopandas
@@ -21,15 +21,17 @@
 Requires-Dist: pypgstac ; extra == "pgstac"
 Requires-Dist: psycopg[binary,pool] ; extra == "pgstac"
 Requires-Dist: tqdm ; extra == "pgstac"
 Requires-Dist: python-dateutil ; extra == "pgstac"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: requests ; extra == "test"
 Requires-Dist: pre-commit ; extra == "test"
-Project-URL: Home, https://github.com/TomAugspurger/stac_geoparquet
+Requires-Dist: stac-geoparquet[pgstac] ; extra == "test"
+Requires-Dist: stac-geoparquet[pc] ; extra == "test"
+Project-URL: Home, https://github.com/stac-utils/stac-geoparquet
 Provides-Extra: pc
 Provides-Extra: pgstac
 Provides-Extra: test
 
 # STAC-geoparquet
 
 Convert STAC items to geoparquet.
```

