# Comparing `tmp/SOMcreator-1.1.7.tar.gz` & `tmp/SOMcreator-1.1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SOMcreator-1.1.7.tar", last modified: Thu Apr  6 10:28:15 2023, max compression
+gzip compressed data, was "SOMcreator-1.1.7.2.tar", last modified: Wed Jul 19 10:56:20 2023, max compression
```

## Comparing `SOMcreator-1.1.7.tar` & `SOMcreator-1.1.7.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 10:28:15.989741 SOMcreator-1.1.7/
--rw-rw-rw-   0        0        0     1095 2022-10-28 12:14:14.000000 SOMcreator-1.1.7/LICENSE
--rw-rw-rw-   0        0        0       81 2022-11-01 07:22:32.000000 SOMcreator-1.1.7/MANIFEST.in
--rw-rw-rw-   0        0        0     1554 2023-04-06 10:28:15.989741 SOMcreator-1.1.7/PKG-INFO
--rw-rw-rw-   0        0        0        9 2022-10-28 11:24:11.000000 SOMcreator-1.1.7/README.md
--rw-rw-rw-   0        0        0      876 2023-03-20 13:30:05.000000 SOMcreator-1.1.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-06 10:28:15.989741 SOMcreator-1.1.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-06 10:28:15.782329 SOMcreator-1.1.7/src/
-drwxrwxrwx   0        0        0        0 2023-04-06 10:28:15.813508 SOMcreator-1.1.7/src/SOMcreator/
-drwxrwxrwx   0        0        0        0 2023-04-06 10:28:15.879756 SOMcreator-1.1.7/src/SOMcreator/Template/
--rw-rw-rw-   0        0        0      375 2023-03-14 10:38:41.000000 SOMcreator-1.1.7/src/SOMcreator/Template/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-06 10:28:15.890492 SOMcreator-1.1.7/src/SOMcreator/Template/__pyinstaller/
--rw-rw-rw-   0        0        0       71 2022-11-02 03:35:28.000000 SOMcreator-1.1.7/src/SOMcreator/Template/__pyinstaller/__init__.py
--rw-rw-rw-   0        0        0      202 2022-11-02 03:56:29.000000 SOMcreator-1.1.7/src/SOMcreator/Template/__pyinstaller/hook-SOMcreator.py
--rw-rw-rw-   0        0        0      331 2023-03-14 10:42:57.000000 SOMcreator-1.1.7/src/SOMcreator/Template/bookmark_template.txt
--rw-rw-rw-   0        0        0    25168 2022-11-01 13:55:19.000000 SOMcreator-1.1.7/src/SOMcreator/Template/ifc.json
-drwxrwxrwx   0        0        0        0 2023-04-06 10:28:15.932307 SOMcreator-1.1.7/src/SOMcreator/Template/js_templates/
--rw-rw-rw-   0        0        0     1001 2023-01-17 17:04:49.000000 SOMcreator-1.1.7/src/SOMcreator/Template/js_templates/end_ungetestet.js
--rw-rw-rw-   0        0        0     7071 2023-03-13 14:55:58.000000 SOMcreator-1.1.7/src/SOMcreator/Template/js_templates/start_check_start.js
--rw-rw-rw-   0        0        0      598 2022-05-18 15:06:32.000000 SOMcreator-1.1.7/src/SOMcreator/Template/js_templates/start_koordinaten.js
--rw-rw-rw-   0        0        0     2938 2023-01-17 17:04:49.000000 SOMcreator-1.1.7/src/SOMcreator/Template/mapping_template.txt
--rw-rw-rw-   0        0        0     3121 2023-03-09 10:50:23.000000 SOMcreator-1.1.7/src/SOMcreator/Template/template.txt
--rw-rw-rw-   0        0        0      154 2023-04-06 10:26:32.000000 SOMcreator-1.1.7/src/SOMcreator/__init__.py
--rw-rw-rw-   0        0        0    24647 2023-04-06 10:27:32.000000 SOMcreator-1.1.7/src/SOMcreator/classes.py
--rw-rw-rw-   0        0        0     1898 2023-03-31 12:00:15.000000 SOMcreator-1.1.7/src/SOMcreator/constants.py
-drwxrwxrwx   0        0        0        0 2023-04-06 10:28:15.988742 SOMcreator-1.1.7/src/SOMcreator/external_software/
--rw-rw-rw-   0        0        0        0 2023-01-17 17:04:49.000000 SOMcreator-1.1.7/src/SOMcreator/external_software/__init__.py
--rw-rw-rw-   0        0        0     4311 2023-01-17 17:04:49.000000 SOMcreator-1.1.7/src/SOMcreator/external_software/allplan.py
--rw-rw-rw-   0        0        0     1365 2023-02-01 08:26:32.000000 SOMcreator-1.1.7/src/SOMcreator/external_software/card1.py
--rw-rw-rw-   0        0        0    22331 2023-03-31 12:44:34.000000 SOMcreator-1.1.7/src/SOMcreator/external_software/desite.py
--rw-rw-rw-   0        0        0    21983 2023-04-05 09:10:58.000000 SOMcreator-1.1.7/src/SOMcreator/external_software/excel.py
--rw-rw-rw-   0        0        0     3326 2023-03-31 12:44:34.000000 SOMcreator-1.1.7/src/SOMcreator/external_software/revit.py
--rw-rw-rw-   0        0        0     3227 2023-02-01 08:26:32.000000 SOMcreator-1.1.7/src/SOMcreator/external_software/vestra.py
--rw-rw-rw-   0        0        0     9363 2023-04-06 08:47:51.000000 SOMcreator-1.1.7/src/SOMcreator/filehandling.py
--rw-rw-rw-   0        0        0      970 2023-02-21 12:05:09.000000 SOMcreator-1.1.7/src/SOMcreator/quality_check.py
-drwxrwxrwx   0        0        0        0 2023-04-06 10:28:15.835077 SOMcreator-1.1.7/src/SOMcreator.egg-info/
--rw-rw-rw-   0        0        0     1554 2023-04-06 10:28:15.000000 SOMcreator-1.1.7/src/SOMcreator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1194 2023-04-06 10:28:15.000000 SOMcreator-1.1.7/src/SOMcreator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 10:28:15.000000 SOMcreator-1.1.7/src/SOMcreator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2023-04-06 10:28:15.000000 SOMcreator-1.1.7/src/SOMcreator.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2023-04-06 10:28:15.000000 SOMcreator-1.1.7/src/SOMcreator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-04-06 10:28:15.000000 SOMcreator-1.1.7/src/SOMcreator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-19 10:56:20.322981 SOMcreator-1.1.7.2/
+-rw-rw-rw-   0        0        0     1095 2022-10-28 12:14:14.000000 SOMcreator-1.1.7.2/LICENSE
+-rw-rw-rw-   0        0        0       81 2022-11-01 07:22:32.000000 SOMcreator-1.1.7.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1556 2023-07-19 10:56:20.322981 SOMcreator-1.1.7.2/PKG-INFO
+-rw-rw-rw-   0        0        0        9 2022-10-28 11:24:11.000000 SOMcreator-1.1.7.2/README.md
+-rw-rw-rw-   0        0        0      876 2023-03-20 13:30:05.000000 SOMcreator-1.1.7.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-19 10:56:20.322981 SOMcreator-1.1.7.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-19 10:56:20.268473 SOMcreator-1.1.7.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-19 10:56:20.274693 SOMcreator-1.1.7.2/src/SOMcreator/
+drwxrwxrwx   0        0        0        0 2023-07-19 10:56:20.314981 SOMcreator-1.1.7.2/src/SOMcreator/Template/
+-rw-rw-rw-   0        0        0      375 2023-05-16 05:28:24.000000 SOMcreator-1.1.7.2/src/SOMcreator/Template/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 10:56:20.315981 SOMcreator-1.1.7.2/src/SOMcreator/Template/__pyinstaller/
+-rw-rw-rw-   0        0        0       71 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.2/src/SOMcreator/Template/__pyinstaller/__init__.py
+-rw-rw-rw-   0        0        0      202 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.2/src/SOMcreator/Template/__pyinstaller/hook-SOMcreator.py
+-rw-rw-rw-   0        0        0      331 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.2/src/SOMcreator/Template/bookmark_template.txt
+-rw-rw-rw-   0        0        0    25168 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.2/src/SOMcreator/Template/ifc.json
+drwxrwxrwx   0        0        0        0 2023-07-19 10:56:20.317981 SOMcreator-1.1.7.2/src/SOMcreator/Template/js_templates/
+-rw-rw-rw-   0        0        0     1001 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.2/src/SOMcreator/Template/js_templates/end_ungetestet.js
+-rw-rw-rw-   0        0        0     7071 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.2/src/SOMcreator/Template/js_templates/start_check_start.js
+-rw-rw-rw-   0        0        0      598 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.2/src/SOMcreator/Template/js_templates/start_koordinaten.js
+-rw-rw-rw-   0        0        0     2938 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.2/src/SOMcreator/Template/mapping_template.txt
+-rw-rw-rw-   0        0        0     3121 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.2/src/SOMcreator/Template/template.txt
+-rw-rw-rw-   0        0        0      156 2023-07-19 10:55:35.000000 SOMcreator-1.1.7.2/src/SOMcreator/__init__.py
+-rw-rw-rw-   0        0        0    24607 2023-07-19 10:49:58.000000 SOMcreator-1.1.7.2/src/SOMcreator/classes.py
+-rw-rw-rw-   0        0        0     1898 2023-05-04 10:57:17.000000 SOMcreator-1.1.7.2/src/SOMcreator/constants.py
+drwxrwxrwx   0        0        0        0 2023-07-19 10:56:20.321981 SOMcreator-1.1.7.2/src/SOMcreator/external_software/
+-rw-rw-rw-   0        0        0        0 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.2/src/SOMcreator/external_software/__init__.py
+-rw-rw-rw-   0        0        0     4311 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.2/src/SOMcreator/external_software/allplan.py
+-rw-rw-rw-   0        0        0     1365 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.2/src/SOMcreator/external_software/card1.py
+-rw-rw-rw-   0        0        0    22331 2023-05-04 10:57:17.000000 SOMcreator-1.1.7.2/src/SOMcreator/external_software/desite.py
+-rw-rw-rw-   0        0        0    21951 2023-06-28 13:16:14.000000 SOMcreator-1.1.7.2/src/SOMcreator/external_software/excel.py
+-rw-rw-rw-   0        0        0     3326 2023-05-04 10:57:17.000000 SOMcreator-1.1.7.2/src/SOMcreator/external_software/revit.py
+-rw-rw-rw-   0        0        0     3227 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.2/src/SOMcreator/external_software/vestra.py
+-rw-rw-rw-   0        0        0     9363 2023-05-04 10:57:17.000000 SOMcreator-1.1.7.2/src/SOMcreator/filehandling.py
+-rw-rw-rw-   0        0        0      970 2023-04-06 10:29:25.000000 SOMcreator-1.1.7.2/src/SOMcreator/quality_check.py
+drwxrwxrwx   0        0        0        0 2023-07-19 10:56:20.311613 SOMcreator-1.1.7.2/src/SOMcreator.egg-info/
+-rw-rw-rw-   0        0        0     1556 2023-07-19 10:56:20.000000 SOMcreator-1.1.7.2/src/SOMcreator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1194 2023-07-19 10:56:20.000000 SOMcreator-1.1.7.2/src/SOMcreator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 10:56:20.000000 SOMcreator-1.1.7.2/src/SOMcreator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2023-07-19 10:56:20.000000 SOMcreator-1.1.7.2/src/SOMcreator.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2023-07-19 10:56:20.000000 SOMcreator-1.1.7.2/src/SOMcreator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-19 10:56:20.000000 SOMcreator-1.1.7.2/src/SOMcreator.egg-info/top_level.txt
```

### Comparing `SOMcreator-1.1.7/LICENSE` & `SOMcreator-1.1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7/PKG-INFO` & `SOMcreator-1.1.7.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SOMcreator
-Version: 1.1.7
+Version: 1.1.7.2
 Summary: create simple Datastructures for BIM Models
 License: MIT License
         
         Copyright (c) 2022 Christoph Mellüh
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `SOMcreator-1.1.7/pyproject.toml` & `SOMcreator-1.1.7.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7/src/SOMcreator/Template/ifc.json` & `SOMcreator-1.1.7.2/src/SOMcreator/Template/ifc.json`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7/src/SOMcreator/Template/js_templates/end_ungetestet.js` & `SOMcreator-1.1.7.2/src/SOMcreator/Template/js_templates/end_ungetestet.js`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7/src/SOMcreator/Template/js_templates/start_check_start.js` & `SOMcreator-1.1.7.2/src/SOMcreator/Template/js_templates/start_check_start.js`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7/src/SOMcreator/Template/js_templates/start_koordinaten.js` & `SOMcreator-1.1.7.2/src/SOMcreator/Template/js_templates/start_koordinaten.js`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7/src/SOMcreator/Template/mapping_template.txt` & `SOMcreator-1.1.7.2/src/SOMcreator/Template/mapping_template.txt`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7/src/SOMcreator/Template/template.txt` & `SOMcreator-1.1.7.2/src/SOMcreator/Template/template.txt`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7/src/SOMcreator/classes.py` & `SOMcreator-1.1.7.2/src/SOMcreator/classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,22 +20,20 @@
         return iter(sorted(list(self._registry), key=lambda x: x.name))
 
     def __len__(self) -> int:
         return len(self._registry)
 
 
 class Project(object):
-    def __init__(self, name: str, author: str|None = None) -> None:
+    def __init__(self, name: str = "", author: str|None = None) -> None:
         self._name = ""
         self._author = author
         self._version = "1.0.0"
-        self._changed = True
+        self._changed = True        # indecates if project was modified -> used for close dialog
         self.name = name
-        self.seperator_status = True
-        self.seperator = ","
 
     def get_uuid_dict(self) -> dict[str,Object|PropertySet|Attribute|Aggregation]:
         pset_dict = {pset.uuid: pset for pset in PropertySet}
         object_dict = {obj.uuid: obj for obj in Object}
         attribute_dict = {attribute.uuid: attribute for attribute in Attribute}
         aggregation_dict = {aggreg.uuid: aggreg for aggreg in Aggregation}
         full_dict = pset_dict | object_dict | attribute_dict | aggregation_dict
@@ -116,16 +114,14 @@
         for attribute in Attribute:
             attribute.delete()
         self.name = ""
         self.author = ""
         self.version = "1.0.0"
         self.changed = True
         self.name = ""
-        self.seperator_status = True
-        self.seperator = ","
 
     def import_excel(self, path: str, ws_name: str) -> None:
         excel.open_file(path, ws_name)
 
     @property
     def objects(self) -> Iterator[Object]:
         return iter(Object)
@@ -630,14 +626,15 @@
         return self._aggregations
 
     def add_aggregation_representation(self, node: Aggregation) -> None:
         self._aggregations.add(node)
 
     def remove_node(self, node: Aggregation) -> None:
         self.aggregation_representations.remove(node)
+        node.delete()
 
     @property
     def inherited_property_sets(self) -> dict[Object, list[PropertySet]]:
         def recursion(recursion_property_sets, recursion_obj: Object):
             psets = recursion_obj.property_sets
 
             if psets:
```

### Comparing `SOMcreator-1.1.7/src/SOMcreator/constants.py` & `SOMcreator-1.1.7.2/src/SOMcreator/constants.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7/src/SOMcreator/external_software/allplan.py` & `SOMcreator-1.1.7.2/src/SOMcreator/external_software/allplan.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7/src/SOMcreator/external_software/card1.py` & `SOMcreator-1.1.7.2/src/SOMcreator/external_software/card1.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7/src/SOMcreator/external_software/desite.py` & `SOMcreator-1.1.7.2/src/SOMcreator/external_software/desite.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7/src/SOMcreator/external_software/excel.py` & `SOMcreator-1.1.7.2/src/SOMcreator/external_software/excel.py`

 * *Files 0% similar despite different names*

```diff
@@ -467,15 +467,15 @@
         sheet.cell(start_row,start_column).value = "bauteilName"
         sheet.cell(start_row,start_column+1).value = obj.name
 
         sheet.cell(start_row+1, start_column).value = "bauteilKlassifikation"
         sheet.cell(start_row+1,start_column+1).value = obj.ident_value
 
         sheet.cell(start_row + 2, start_column).value = "Kürzel"
-        sheet.cell(start_row+2,start_column+1).value = str(obj.custom_attribues.get(constants.ABBREVIATION))
+        sheet.cell(start_row+2,start_column+1).value = str(obj.abbreviation)
 
         sheet.cell(start_row+3,start_column).value = "Property"
         sheet.cell(start_row+3,start_column+1).value = "Propertyset"
         sheet.cell(start_row+3,start_column+2).value = "Beispiele / Beschreibung"
 
         for i in range(0,4):
             for k in range(0,3):
```

### Comparing `SOMcreator-1.1.7/src/SOMcreator/external_software/revit.py` & `SOMcreator-1.1.7.2/src/SOMcreator/external_software/revit.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7/src/SOMcreator/external_software/vestra.py` & `SOMcreator-1.1.7.2/src/SOMcreator/external_software/vestra.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7/src/SOMcreator/filehandling.py` & `SOMcreator-1.1.7.2/src/SOMcreator/filehandling.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7/src/SOMcreator/quality_check.py` & `SOMcreator-1.1.7.2/src/SOMcreator/quality_check.py`

 * *Files identical despite different names*

### Comparing `SOMcreator-1.1.7/src/SOMcreator.egg-info/PKG-INFO` & `SOMcreator-1.1.7.2/src/SOMcreator.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SOMcreator
-Version: 1.1.7
+Version: 1.1.7.2
 Summary: create simple Datastructures for BIM Models
 License: MIT License
         
         Copyright (c) 2022 Christoph Mellüh
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `SOMcreator-1.1.7/src/SOMcreator.egg-info/SOURCES.txt` & `SOMcreator-1.1.7.2/src/SOMcreator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

