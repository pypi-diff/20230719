# Comparing `tmp/metabolights_utils-0.9.2.tar.gz` & `tmp/metabolights_utils-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metabolights_utils-0.9.2.tar", max compression
+gzip compressed data, was "metabolights_utils-0.9.3.tar", max compression
```

## Comparing `metabolights_utils-0.9.2.tar` & `metabolights_utils-0.9.3.tar`

### file list

```diff
@@ -1,56 +1,55 @@
--rw-r--r--   0        0        0    11357 2023-07-11 10:00:28.160792 metabolights_utils-0.9.2/LICENSE
--rw-r--r--   0        0        0     3259 2023-07-17 20:48:23.394069 metabolights_utils-0.9.2/README.md
--rw-r--r--   0        0        0        0 2023-07-10 10:49:29.981642 metabolights_utils-0.9.2/metabolights_utils/__init__.py
--rw-r--r--   0        0        0      244 2023-07-18 12:41:51.755776 metabolights_utils-0.9.2/metabolights_utils/common.py
--rw-r--r--   0        0        0        0 2023-07-14 06:51:23.231059 metabolights_utils-0.9.2/metabolights_utils/isatab/__init__.py
--rw-r--r--   0        0        0        0 2023-07-17 13:19:51.764169 metabolights_utils-0.9.2/metabolights_utils/isatab/helper/__init__.py
--rw-r--r--   0        0        0      708 2023-07-15 14:29:29.004862 metabolights_utils-0.9.2/metabolights_utils/isatab/helper/assay_file_helper.py
--rw-r--r--   0        0        0     1260 2023-07-15 14:29:28.898072 metabolights_utils-0.9.2/metabolights_utils/isatab/helper/assignment_file_helper.py
--rw-r--r--   0        0        0     1512 2023-07-14 08:36:13.926789 metabolights_utils-0.9.2/metabolights_utils/isatab/helper/base_isa_file_helper.py
--rw-r--r--   0        0        0     5829 2023-07-17 20:54:44.959168 metabolights_utils-0.9.2/metabolights_utils/isatab/helper/base_isa_table_file_helper.py
--rw-r--r--   0        0        0    10677 2023-07-17 21:37:37.333171 metabolights_utils-0.9.2/metabolights_utils/isatab/helper/investigation_file_helper.py
--rw-r--r--   0        0        0      698 2023-07-15 14:29:29.056606 metabolights_utils-0.9.2/metabolights_utils/isatab/helper/sample_file_helper.py
--rw-r--r--   0        0        0     1682 2023-07-17 20:52:46.971222 metabolights_utils-0.9.2/metabolights_utils/isatab/investigation_file_reader.py
--rw-r--r--   0        0        0     2050 2023-07-14 08:12:36.253515 metabolights_utils-0.9.2/metabolights_utils/isatab/investigation_file_writer.py
--rw-r--r--   0        0        0     8102 2023-07-15 15:46:43.496883 metabolights_utils-0.9.2/metabolights_utils/isatab/isa_table_file_reader.py
--rw-r--r--   0        0        0     2909 2023-07-18 17:00:04.330628 metabolights_utils-0.9.2/metabolights_utils/isatab/isa_table_file_writer.py
--rw-r--r--   0        0        0     1844 2023-07-18 16:48:05.150888 metabolights_utils-0.9.2/metabolights_utils/isatab/isatab_file_helper.py
--rw-r--r--   0        0        0        0 2023-07-10 10:51:24.233594 metabolights_utils-0.9.2/metabolights_utils/models/__init__.py
--rw-r--r--   0        0        0      442 2023-07-18 12:41:42.144955 metabolights_utils-0.9.2/metabolights_utils/models/common.py
--rw-r--r--   0        0        0      149 2023-07-12 17:00:03.147342 metabolights_utils-0.9.2/metabolights_utils/models/enums.py
--rw-r--r--   0        0        0        0 2023-07-10 12:23:13.111498 metabolights_utils-0.9.2/metabolights_utils/models/isa/__init__.py
--rw-r--r--   0        0        0      531 2023-07-17 20:42:23.361722 metabolights_utils-0.9.2/metabolights_utils/models/isa/assay_file.py
--rw-r--r--   0        0        0      402 2023-07-17 20:41:02.431487 metabolights_utils-0.9.2/metabolights_utils/models/isa/assignment_file.py
--rw-r--r--   0        0        0    10881 2023-07-17 21:24:19.800755 metabolights_utils-0.9.2/metabolights_utils/models/isa/common.py
--rw-r--r--   0        0        0      478 2023-07-12 16:53:15.362181 metabolights_utils-0.9.2/metabolights_utils/models/isa/enums.py
--rw-r--r--   0        0        0    10817 2023-07-17 21:27:02.610563 metabolights_utils-0.9.2/metabolights_utils/models/isa/investigation_file.py
--rw-r--r--   0        0        0    17617 2023-07-17 20:53:30.375766 metabolights_utils-0.9.2/metabolights_utils/models/isa/parser/common.py
--rw-r--r--   0        0        0     9125 2023-07-16 16:31:04.548645 metabolights_utils-0.9.2/metabolights_utils/models/isa/parser/filter.py
--rw-r--r--   0        0        0    21626 2023-07-17 21:25:57.104435 metabolights_utils-0.9.2/metabolights_utils/models/isa/parser/investigation_parser.py
--rw-r--r--   0        0        0    17992 2023-07-17 20:54:45.872793 metabolights_utils-0.9.2/metabolights_utils/models/isa/parser/isa_table_parser.py
--rw-r--r--   0        0        0     5159 2023-07-16 16:31:08.768258 metabolights_utils-0.9.2/metabolights_utils/models/isa/parser/sort.py
--rw-r--r--   0        0        0      457 2023-07-17 20:43:34.998092 metabolights_utils-0.9.2/metabolights_utils/models/isa/samples_file.py
--rw-r--r--   0        0        0        0 2023-07-12 15:31:33.134362 metabolights_utils-0.9.2/metabolights_utils/models/metabolights/__init__.py
--rw-r--r--   0        0        0     1077 2023-07-17 20:39:40.816755 metabolights_utils-0.9.2/metabolights_utils/models/metabolights/metabolights_study.py
--rw-r--r--   0        0        0        0 2023-07-12 15:36:01.541604 metabolights_utils-0.9.2/metabolights_utils/models/parser/__init__.py
--rw-r--r--   0        0        0      766 2023-07-15 08:09:31.938967 metabolights_utils-0.9.2/metabolights_utils/models/parser/common.py
--rw-r--r--   0        0        0      148 2023-07-15 08:10:44.291129 metabolights_utils-0.9.2/metabolights_utils/models/parser/enums.py
--rw-r--r--   0        0        0        0 2023-07-18 12:31:01.631181 metabolights_utils-0.9.2/metabolights_utils/tsv/__init__.py
--rw-r--r--   0        0        0        0 2023-07-17 13:19:49.880266 metabolights_utils-0.9.2/metabolights_utils/tsv/actions/__init__.py
--rw-r--r--   0        0        0     3413 2023-07-18 12:46:07.521346 metabolights_utils-0.9.2/metabolights_utils/tsv/actions/add_column.py
--rw-r--r--   0        0        0     3201 2023-07-18 12:49:27.614018 metabolights_utils-0.9.2/metabolights_utils/tsv/actions/add_row.py
--rw-r--r--   0        0        0     1342 2023-07-18 15:49:15.831466 metabolights_utils-0.9.2/metabolights_utils/tsv/actions/base.py
--rw-r--r--   0        0        0     3351 2023-07-18 13:49:23.813831 metabolights_utils-0.9.2/metabolights_utils/tsv/actions/copy_column.py
--rw-r--r--   0        0        0     3097 2023-07-18 15:16:49.116854 metabolights_utils-0.9.2/metabolights_utils/tsv/actions/copy_row.py
--rw-r--r--   0        0        0     2423 2023-07-18 14:00:02.070569 metabolights_utils-0.9.2/metabolights_utils/tsv/actions/delete_column.py
--rw-r--r--   0        0        0     2012 2023-07-18 12:45:05.682152 metabolights_utils-0.9.2/metabolights_utils/tsv/actions/delete_row.py
--rw-r--r--   0        0        0     2780 2023-07-18 13:38:55.025530 metabolights_utils-0.9.2/metabolights_utils/tsv/actions/move_column.py
--rw-r--r--   0        0        0     3372 2023-07-18 12:45:05.343441 metabolights_utils-0.9.2/metabolights_utils/tsv/actions/move_row.py
--rw-r--r--   0        0        0     3062 2023-07-18 16:25:10.033932 metabolights_utils-0.9.2/metabolights_utils/tsv/actions/update_cell.py
--rw-r--r--   0        0        0     3384 2023-07-18 14:51:21.210651 metabolights_utils-0.9.2/metabolights_utils/tsv/actions/update_column.py
--rw-r--r--   0        0        0     2047 2023-07-18 14:15:45.293287 metabolights_utils-0.9.2/metabolights_utils/tsv/actions/update_column_header.py
--rw-r--r--   0        0        0     2294 2023-07-18 15:46:46.103848 metabolights_utils-0.9.2/metabolights_utils/tsv/actions/update_row.py
--rw-r--r--   0        0        0     3549 2023-07-18 15:46:02.737733 metabolights_utils-0.9.2/metabolights_utils/tsv/model.py
--rw-r--r--   0        0        0     5701 2023-07-18 16:14:32.052914 metabolights_utils-0.9.2/metabolights_utils/tsv/tsv_file_updater.py
--rw-r--r--   0        0        0     1310 2023-07-18 17:31:44.686363 metabolights_utils-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     4243 1970-01-01 00:00:00.000000 metabolights_utils-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-11 10:00:28.160792 metabolights_utils-0.9.3/LICENSE
+-rw-r--r--   0        0        0    14216 2023-07-19 00:08:10.995500 metabolights_utils-0.9.3/README.md
+-rw-r--r--   0        0        0        0 2023-07-10 10:49:29.981642 metabolights_utils-0.9.3/metabolights_utils/__init__.py
+-rw-r--r--   0        0        0      244 2023-07-18 12:41:51.755776 metabolights_utils-0.9.3/metabolights_utils/common.py
+-rw-r--r--   0        0        0     2214 2023-07-18 21:47:52.784928 metabolights_utils-0.9.3/metabolights_utils/isatab/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-17 13:19:51.764169 metabolights_utils-0.9.3/metabolights_utils/isatab/default/__init__.py
+-rw-r--r--   0        0        0      716 2023-07-18 21:00:22.599458 metabolights_utils-0.9.3/metabolights_utils/isatab/default/assay_file.py
+-rw-r--r--   0        0        0     1268 2023-07-18 21:00:23.409605 metabolights_utils-0.9.3/metabolights_utils/isatab/default/assignment_file.py
+-rw-r--r--   0        0        0     1536 2023-07-18 20:55:33.062347 metabolights_utils-0.9.3/metabolights_utils/isatab/default/base_isa_file.py
+-rw-r--r--   0        0        0     5906 2023-07-18 21:10:17.881501 metabolights_utils-0.9.3/metabolights_utils/isatab/default/base_isa_table_file.py
+-rw-r--r--   0        0        0     1847 2023-07-18 21:29:16.380647 metabolights_utils-0.9.3/metabolights_utils/isatab/default/factory.py
+-rw-r--r--   0        0        0    11163 2023-07-18 21:11:46.711336 metabolights_utils-0.9.3/metabolights_utils/isatab/default/investigation_file.py
+-rw-r--r--   0        0        0      706 2023-07-18 21:00:23.587697 metabolights_utils-0.9.3/metabolights_utils/isatab/default/sample_file.py
+-rw-r--r--   0        0        0     1488 2023-07-18 21:10:17.496617 metabolights_utils-0.9.3/metabolights_utils/isatab/default/writer.py
+-rw-r--r--   0        0        0     9873 2023-07-18 21:25:37.213260 metabolights_utils-0.9.3/metabolights_utils/isatab/reader.py
+-rw-r--r--   0        0        0     3692 2023-07-18 21:22:20.774314 metabolights_utils-0.9.3/metabolights_utils/isatab/writer.py
+-rw-r--r--   0        0        0        0 2023-07-10 10:51:24.233594 metabolights_utils-0.9.3/metabolights_utils/models/__init__.py
+-rw-r--r--   0        0        0      442 2023-07-18 12:41:42.144955 metabolights_utils-0.9.3/metabolights_utils/models/common.py
+-rw-r--r--   0        0        0      149 2023-07-12 17:00:03.147342 metabolights_utils-0.9.3/metabolights_utils/models/enums.py
+-rw-r--r--   0        0        0        0 2023-07-10 12:23:13.111498 metabolights_utils-0.9.3/metabolights_utils/models/isa/__init__.py
+-rw-r--r--   0        0        0      531 2023-07-17 20:42:23.361722 metabolights_utils-0.9.3/metabolights_utils/models/isa/assay_file.py
+-rw-r--r--   0        0        0      402 2023-07-17 20:41:02.431487 metabolights_utils-0.9.3/metabolights_utils/models/isa/assignment_file.py
+-rw-r--r--   0        0        0    10914 2023-07-18 20:43:53.821951 metabolights_utils-0.9.3/metabolights_utils/models/isa/common.py
+-rw-r--r--   0        0        0      478 2023-07-12 16:53:15.362181 metabolights_utils-0.9.3/metabolights_utils/models/isa/enums.py
+-rw-r--r--   0        0        0    11080 2023-07-18 20:43:53.902912 metabolights_utils-0.9.3/metabolights_utils/models/isa/investigation_file.py
+-rw-r--r--   0        0        0    18241 2023-07-18 20:43:54.081050 metabolights_utils-0.9.3/metabolights_utils/models/isa/parser/common.py
+-rw-r--r--   0        0        0     9969 2023-07-18 20:43:54.037206 metabolights_utils-0.9.3/metabolights_utils/models/isa/parser/filter.py
+-rw-r--r--   0        0        0    22198 2023-07-18 20:43:54.398222 metabolights_utils-0.9.3/metabolights_utils/models/isa/parser/investigation_parser.py
+-rw-r--r--   0        0        0    18279 2023-07-18 20:43:54.437998 metabolights_utils-0.9.3/metabolights_utils/models/isa/parser/isa_table_parser.py
+-rw-r--r--   0        0        0     5421 2023-07-18 20:43:54.520986 metabolights_utils-0.9.3/metabolights_utils/models/isa/parser/sort.py
+-rw-r--r--   0        0        0      457 2023-07-17 20:43:34.998092 metabolights_utils-0.9.3/metabolights_utils/models/isa/samples_file.py
+-rw-r--r--   0        0        0        0 2023-07-12 15:31:33.134362 metabolights_utils-0.9.3/metabolights_utils/models/metabolights/__init__.py
+-rw-r--r--   0        0        0     1077 2023-07-17 20:39:40.816755 metabolights_utils-0.9.3/metabolights_utils/models/metabolights/metabolights_study.py
+-rw-r--r--   0        0        0        0 2023-07-12 15:36:01.541604 metabolights_utils-0.9.3/metabolights_utils/models/parser/__init__.py
+-rw-r--r--   0        0        0      766 2023-07-15 08:09:31.938967 metabolights_utils-0.9.3/metabolights_utils/models/parser/common.py
+-rw-r--r--   0        0        0      148 2023-07-15 08:10:44.291129 metabolights_utils-0.9.3/metabolights_utils/models/parser/enums.py
+-rw-r--r--   0        0        0        0 2023-07-18 12:31:01.631181 metabolights_utils-0.9.3/metabolights_utils/tsv/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-17 13:19:49.880266 metabolights_utils-0.9.3/metabolights_utils/tsv/actions/__init__.py
+-rw-r--r--   0        0        0     3579 2023-07-18 20:43:54.645743 metabolights_utils-0.9.3/metabolights_utils/tsv/actions/add_column.py
+-rw-r--r--   0        0        0     3497 2023-07-18 20:43:54.654143 metabolights_utils-0.9.3/metabolights_utils/tsv/actions/add_row.py
+-rw-r--r--   0        0        0     1342 2023-07-18 15:49:15.831466 metabolights_utils-0.9.3/metabolights_utils/tsv/actions/base.py
+-rw-r--r--   0        0        0     3399 2023-07-18 20:43:54.957085 metabolights_utils-0.9.3/metabolights_utils/tsv/actions/copy_column.py
+-rw-r--r--   0        0        0     3153 2023-07-18 20:43:54.916074 metabolights_utils-0.9.3/metabolights_utils/tsv/actions/copy_row.py
+-rw-r--r--   0        0        0     2501 2023-07-18 20:43:54.957976 metabolights_utils-0.9.3/metabolights_utils/tsv/actions/delete_column.py
+-rw-r--r--   0        0        0     2012 2023-07-18 12:45:05.682152 metabolights_utils-0.9.3/metabolights_utils/tsv/actions/delete_row.py
+-rw-r--r--   0        0        0     2876 2023-07-18 20:43:55.038645 metabolights_utils-0.9.3/metabolights_utils/tsv/actions/move_column.py
+-rw-r--r--   0        0        0     3372 2023-07-18 12:45:05.343441 metabolights_utils-0.9.3/metabolights_utils/tsv/actions/move_row.py
+-rw-r--r--   0        0        0     3166 2023-07-18 20:43:55.131109 metabolights_utils-0.9.3/metabolights_utils/tsv/actions/update_cell.py
+-rw-r--r--   0        0        0     3564 2023-07-18 20:43:55.148168 metabolights_utils-0.9.3/metabolights_utils/tsv/actions/update_column.py
+-rw-r--r--   0        0        0     2103 2023-07-18 20:43:55.218071 metabolights_utils-0.9.3/metabolights_utils/tsv/actions/update_column_header.py
+-rw-r--r--   0        0        0     2238 2023-07-18 20:43:55.218128 metabolights_utils-0.9.3/metabolights_utils/tsv/actions/update_row.py
+-rw-r--r--   0        0        0     3591 2023-07-18 20:43:55.383088 metabolights_utils-0.9.3/metabolights_utils/tsv/model.py
+-rw-r--r--   0        0        0     5851 2023-07-18 20:43:55.381399 metabolights_utils-0.9.3/metabolights_utils/tsv/tsv_file_updater.py
+-rw-r--r--   0        0        0     1310 2023-07-19 00:15:00.063652 metabolights_utils-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0    15200 1970-01-01 00:00:00.000000 metabolights_utils-0.9.3/PKG-INFO
```

### Comparing `metabolights_utils-0.9.2/LICENSE` & `metabolights_utils-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.2/metabolights_utils/isatab/helper/assay_file_helper.py` & `metabolights_utils-0.9.3/metabolights_utils/isatab/default/assay_file.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from typing import List
 
-from metabolights_utils.isatab.helper.base_isa_table_file_helper import BaseIsaTableFileHelper
+from metabolights_utils.isatab.default.base_isa_table_file import BaseIsaTableFileReader
 
 
-class AssayFileHelper(BaseIsaTableFileHelper):
+class DefaultAssayFileReader(BaseIsaTableFileReader):
     patterns = [
         ["^(Extract Name)$", ""],
         ["^(Protocol REF)(\.\d+)?$", "Protocol"],
         ["^(Sample Name)$", ""],
         ["^Parameter Value\[(\w[ -~]*)\]$", "Parameter Value"],
         ["^Comment\b\[(\w{1}[ -~]*)\]$", "Comment"],
         ["^(Labeled Extract Name)$", ""],
         ["^(Label)$", ""],
     ]
 
     def __init__(self, results_per_page=100) -> None:
         super().__init__(results_per_page=results_per_page)
 
     def _get_expected_patterns(self) -> List[List[str]]:
-        return AssayFileHelper.patterns
+        return DefaultAssayFileReader.patterns
```

### Comparing `metabolights_utils-0.9.2/metabolights_utils/isatab/helper/assignment_file_helper.py` & `metabolights_utils-0.9.3/metabolights_utils/isatab/default/assignment_file.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List
 
-from metabolights_utils.isatab.helper.base_isa_table_file_helper import BaseIsaTableFileHelper
+from metabolights_utils.isatab.default.base_isa_table_file import BaseIsaTableFileReader
 
 
-class AssignmentFileHelper(BaseIsaTableFileHelper):
+class DefaultAssignmentFileReader(BaseIsaTableFileReader):
     patterns = [
         ["^(datdatabase_identifier)$", ""],
         ["^(chemical_formula)$", ""],
         ["^(smiles)$", ""],
         ["^(inchi)$", ""],
         ["^(metabolite_identification)$", ""],
         ["^(mass_to_charge)$", ""],
@@ -30,8 +30,8 @@
         ["^(smallmolecule_abundance_std_error_sub)$", ""],
     ]
 
     def __init__(self, results_per_page=100) -> None:
         super().__init__(results_per_page=results_per_page)
 
     def _get_expected_patterns(self) -> List[List[str]]:
-        return AssignmentFileHelper.patterns
+        return DefaultAssignmentFileReader.patterns
```

### Comparing `metabolights_utils-0.9.2/metabolights_utils/isatab/helper/base_isa_file_helper.py` & `metabolights_utils-0.9.3/metabolights_utils/isatab/default/base_isa_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,17 @@
         self,
         file_buffer: IOBase = None,
         file_path: Union[str, pathlib.Path] = None,
     ) -> int:
         if not file_buffer and not file_path:
             ValueError("At least file buffer or file path should be defined")
 
-        selected_file_buffer = file_path if file_path and not file_buffer else file_buffer
+        selected_file_buffer = (
+            file_path if file_path and not file_buffer else file_buffer
+        )
         selected_file_path = file_path if file_path else "<processed content>"
         return selected_file_buffer, selected_file_path
 
     def _get_file_buffer(self, file: Union[str, pathlib.Path, IOBase]) -> IOBase:
         if isinstance(file, IOBase):
             file_buffer = file
         elif isinstance(file, pathlib.Path):
```

### Comparing `metabolights_utils-0.9.2/metabolights_utils/isatab/helper/base_isa_table_file_helper.py` & `metabolights_utils-0.9.3/metabolights_utils/isatab/default/base_isa_table_file.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import os
 import pathlib
 from abc import ABC, abstractmethod
 from io import IOBase
 from typing import List, Union
 
-from metabolights_utils.isatab.helper.base_isa_file_helper import BaseIsaFile
-from metabolights_utils.isatab.isa_table_file_reader import (
+from metabolights_utils.isatab.default.base_isa_file import BaseIsaFile
+from metabolights_utils.isatab.reader import (
     IsaTableFileReader,
     IsaTableFileReaderResult,
 )
 from metabolights_utils.models.isa.parser.filter import TsvFileFilterOption
 from metabolights_utils.models.isa.parser.isa_table_parser import get_isa_table
 from metabolights_utils.models.isa.parser.sort import TsvFileSortOption
 from metabolights_utils.models.parser.common import ParserMessage, ParserReport
 from metabolights_utils.models.parser.enums import ParserMessageType
 
 
-class BaseIsaTableFileHelper(BaseIsaFile, IsaTableFileReader, ABC):
+class BaseIsaTableFileReader(BaseIsaFile, IsaTableFileReader, ABC):
     def __init__(self, results_per_page=100) -> None:
         self.results_per_page = results_per_page if results_per_page > 0 else 100
 
     @abstractmethod
     def _get_expected_patterns(self) -> List[List[str]]:
         pass
 
@@ -29,15 +29,17 @@
         file_buffer: IOBase = None,
         results_per_page: int = 100,
         file_path: Union[str, pathlib.Path] = None,
     ) -> int:
         buffer_or_path, path = self._get_file_buffer_and_path(file_buffer, file_path)
 
         total = self.get_total_row_count(buffer_or_path, path)
-        return int(total / results_per_page) + (1 if total % results_per_page > 0 else 0)
+        return int(total / results_per_page) + (
+            1 if total % results_per_page > 0 else 0
+        )
 
     def get_total_row_count(
         self,
         file_buffer: IOBase = None,
         file_path: Union[str, pathlib.Path] = None,
     ) -> int:
         buffer_or_path, path = self._get_file_buffer_and_path(file_buffer, file_path)
@@ -52,15 +54,17 @@
         results_per_page: int = 100,
         selected_columns: Union[List[str], None] = None,
         file_path: Union[str, pathlib.Path] = None,
         filter_options: List[TsvFileFilterOption] = None,
         sort_options: List[TsvFileSortOption] = None,
     ) -> IsaTableFileReaderResult:
         page = page if page and page > 1 else 1
-        results_per_page = results_per_page if results_per_page > 0 else self.results_per_page
+        results_per_page = (
+            results_per_page if results_per_page > 0 else self.results_per_page
+        )
         offset = (page - 1) * results_per_page
         buffer_or_path, path = self._get_file_buffer_and_path(file_buffer, file_path)
         return self.get_rows(
             file_buffer=buffer_or_path,
             offset=offset,
             limit=results_per_page,
             selected_columns=selected_columns,
@@ -123,15 +127,17 @@
         skip_parser_info_messages: bool = True,
         filter_options: List[TsvFileFilterOption] = None,
         sort_options: List[TsvFileSortOption] = None,
     ) -> IsaTableFileReaderResult:
         buffer: IOBase = None
         read_messages: List[ParserMessage] = []
         try:
-            buffer_or_path, path = self._get_file_buffer_and_path(file_path_or_buffer, file_path)
+            buffer_or_path, path = self._get_file_buffer_and_path(
+                file_path_or_buffer, file_path
+            )
             basename = os.path.basename(str(path))
             file_buffer = self._get_file_buffer(buffer_or_path)
             isa_table = get_isa_table(
                 file_buffer,
                 basename,
                 messages=read_messages,
                 expected_patterns=self._get_expected_patterns(),
@@ -144,8 +150,10 @@
         finally:
             self._close_file(buffer, file_path_or_buffer)
 
         messages = read_messages
         if skip_parser_info_messages:
             messages = [x for x in read_messages if x.type != ParserMessageType.INFO]
         parser_report = ParserReport(messages=messages)
-        return IsaTableFileReaderResult(isa_table_file=isa_table, parser_report=parser_report)
+        return IsaTableFileReaderResult(
+            isa_table_file=isa_table, parser_report=parser_report
+        )
```

### Comparing `metabolights_utils-0.9.2/metabolights_utils/isatab/helper/investigation_file_helper.py` & `metabolights_utils-0.9.3/metabolights_utils/isatab/default/investigation_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,79 +1,90 @@
 import pathlib
 import sys
-from abc import ABC
 from io import IOBase
-from typing import List, Tuple, Union
+from typing import List, Union
 
 import humps
-from pydantic import BaseModel, Field
+from pydantic import BaseModel
 
-from metabolights_utils.isatab.helper.base_isa_file_helper import BaseIsaFile
-from metabolights_utils.isatab.investigation_file_reader import (
+from metabolights_utils.isatab.default.base_isa_file import BaseIsaFile
+from metabolights_utils.isatab.reader import (
     InvestigationFileReader,
     InvestigationFileReaderResult,
 )
-from metabolights_utils.isatab.investigation_file_writer import InvestigationFileWriter
-from metabolights_utils.models.common import MetabolightsBaseModel
+from metabolights_utils.isatab.writer import InvestigationFileWriter
 from metabolights_utils.models.isa.common import IsaAbstractModel
 from metabolights_utils.models.isa.investigation_file import BaseSection, Investigation
-from metabolights_utils.models.isa.investigation_file import module_name as inv_module_name
+from metabolights_utils.models.isa.investigation_file import (
+    module_name as inv_module_name,
+)
 from metabolights_utils.models.isa.parser.investigation_parser import get_investigation
 from metabolights_utils.models.parser.common import ParserMessage, ParserReport
 from metabolights_utils.models.parser.enums import ParserMessageType
 
 
-class InvestigationFileHelper(InvestigationFileWriter, InvestigationFileReader, BaseIsaFile):
+class DefaultInvestigationFileReader(InvestigationFileReader, BaseIsaFile):
     def read(
         self,
         file_buffer: IOBase = None,
         file_path: Union[str, pathlib.Path] = None,
         skip_parser_info_messages: bool = True,
     ) -> InvestigationFileReaderResult:
         buffer_or_path, path = self._get_file_buffer_and_path(file_buffer, file_path)
         file_buffer = self._get_file_buffer(buffer_or_path)
         try:
             read_messages: List[ParserMessage] = []
             investigation = get_investigation(file_buffer, path, messages=read_messages)
             messages = read_messages
             if skip_parser_info_messages:
-                messages = [x for x in read_messages if x.type != ParserMessageType.INFO]
+                messages = [
+                    x for x in read_messages if x.type != ParserMessageType.INFO
+                ]
             report = ParserReport(messages=messages)
-            return InvestigationFileReaderResult(investigation=investigation, parser_report=report)
+            return InvestigationFileReaderResult(
+                investigation=investigation, parser_report=report
+            )
         except Exception as exc:
             raise exc
         finally:
             self._close_file(file_buffer, file_path)
 
+
+class DefaultInvestigationFileWriter(InvestigationFileWriter, BaseIsaFile):
     def write(
         self,
         investigation: Investigation,
         file_buffer: IOBase = None,
         file_path: Union[str, pathlib.Path] = None,
         values_in_quatation_mark: bool = True,
         verify_file_after_update: bool = True,
         skip_parser_info_messages: bool = True,
     ) -> InvestigationFileReaderResult:
         content = InvestigationFileSerializer.to_isa_file_string(
-            investigation=investigation, values_in_quatation_mark=values_in_quatation_mark
+            investigation=investigation,
+            values_in_quatation_mark=values_in_quatation_mark,
         )
         buffer_or_path, path = self._get_file_buffer_and_path(file_buffer, file_path)
         try:
             if file_buffer:
                 file_buffer.write(content)
             else:
                 with open(buffer_or_path, "w") as f:
                     f.write(content)
 
             if verify_file_after_update:
                 read_messages: List[ParserMessage] = []
-                new_investigation = get_investigation(buffer_or_path, path, messages=read_messages)
+                new_investigation = get_investigation(
+                    buffer_or_path, path, messages=read_messages
+                )
                 messages = read_messages
                 if skip_parser_info_messages:
-                    messages = [x for x in read_messages if x.type != ParserMessageType.INFO]
+                    messages = [
+                        x for x in read_messages if x.type != ParserMessageType.INFO
+                    ]
                 report = ParserReport(messages=messages)
                 return InvestigationFileReaderResult(
                     investigation=new_investigation, parser_report=report
                 )
             return InvestigationFileReaderResult(
                 investigation=investigation, parser_report=ParserReport()
             )
@@ -110,23 +121,33 @@
         rows.extend(cls.add_sub_section("", investigation))
         rows.extend(
             cls.add_sub_section(
                 investigation.section_prefix, investigation.investigation_publications
             )
         )
         rows.extend(
-            cls.add_sub_section(investigation.section_prefix, investigation.investigation_contacts)
+            cls.add_sub_section(
+                investigation.section_prefix, investigation.investigation_contacts
+            )
         )
         for study in investigation.studies:
             rows.extend(cls.add_sub_section("", study))
-            rows.extend(cls.add_sub_section(study.section_prefix, study.study_design_descriptors))
-            rows.extend(cls.add_sub_section(study.section_prefix, study.study_publications))
+            rows.extend(
+                cls.add_sub_section(
+                    study.section_prefix, study.study_design_descriptors
+                )
+            )
+            rows.extend(
+                cls.add_sub_section(study.section_prefix, study.study_publications)
+            )
             rows.extend(cls.add_sub_section(study.section_prefix, study.study_factors))
             rows.extend(cls.add_sub_section(study.section_prefix, study.study_assays))
-            rows.extend(cls.add_sub_section(study.section_prefix, study.study_protocols))
+            rows.extend(
+                cls.add_sub_section(study.section_prefix, study.study_protocols)
+            )
             rows.extend(cls.add_sub_section(study.section_prefix, study.study_contacts))
         return rows
 
     @staticmethod
     def get_attribute(model, field_name):
         model_field_name = humps.decamelize(field_name)
         return getattr(model, model_field_name)
@@ -151,28 +172,34 @@
             if isinstance(value, list):
                 properties = data_schema["properties"]
                 if "allOf" in properties[field_key] or "items" in properties[field_key]:
                     if "allOf" in "allOf" in properties[field_key]:
                         item_ref = properties[field_key]["allOf"][0]["$ref"]
                     else:
                         item_ref = properties[field_key]["items"]["$ref"]
-                    default_object_name = item_ref.replace("#/definitions/", "").replace(
-                        "#/$defs/", ""
-                    )
+                    default_object_name = item_ref.replace(
+                        "#/definitions/", ""
+                    ).replace("#/$defs/", "")
                     obj = getattr(sys.modules[inv_module_name], default_object_name)
                     props = obj.schema()["properties"]
                     header.append(data_schema["properties"][field_key]["header_name"])
-                    sub_model_rows = cls.add_model_content(" ".join(header).strip(), value, props)
+                    sub_model_rows = cls.add_model_content(
+                        " ".join(header).strip(), value, props
+                    )
                     if sub_model_rows:
                         rows.extend(sub_model_rows)
             elif isinstance(value, str):
                 field_attribute = humps.decamelize(field_name)
-                header_name = model.__fields__[field_attribute].field_info.extra["header_name"]
+                header_name = model.__fields__[field_attribute].field_info.extra[
+                    "header_name"
+                ]
                 header_name = (
-                    f"{model.section_prefix} {header_name}" if model.section_prefix else header_name
+                    f"{model.section_prefix} {header_name}"
+                    if model.section_prefix
+                    else header_name
                 )
                 rows.append([header_name, value])
             else:
                 raise Exception()
 
         cls.add_comments(model, rows)
         return rows
@@ -196,25 +223,31 @@
             header_name = properties[field_key]["header_name"]
             header_name = f"{prefix} {header_name}".strip() if prefix else header_name
             if "allOf" in properties[field_key] or "items" in properties[field_key]:
                 if "allOf" in "allOf" in properties[field_key]:
                     item_ref: str = properties[field_key]["allOf"][0]["$ref"]
                 else:
                     item_ref: str = properties[field_key]["items"]["$ref"]
-                class_name = item_ref.replace("#/definitions/", "").replace("#/$defs/", "")
+                class_name = item_ref.replace("#/definitions/", "").replace(
+                    "#/$defs/", ""
+                )
                 obj: BaseModel = getattr(sys.modules[inv_module_name], class_name)
                 props = obj.schema()["properties"]
                 input_items = (
-                    [cls.get_attribute(item, field_key) for item in items] if items else [obj()]
+                    [cls.get_attribute(item, field_key) for item in items]
+                    if items
+                    else [obj()]
                 )
 
                 item_values = cls.add_model_content(header_name, input_items, props)
                 rows.extend(item_values)
             elif "type" in properties[field_key]:
-                cls.assign_type(items, properties, rows, row_map, fields, i, header_name)
+                cls.assign_type(
+                    items, properties, rows, row_map, fields, i, header_name
+                )
 
         return rows
 
     @classmethod
     def assign_type(cls, items, properties, rows, row_map, fields, i, header_name):
         field_key = humps.camelize(fields[i])
         object_type = properties[field_key]["type"]
```

### Comparing `metabolights_utils-0.9.2/metabolights_utils/isatab/helper/sample_file_helper.py` & `metabolights_utils-0.9.3/metabolights_utils/isatab/default/sample_file.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from typing import List
 
-from metabolights_utils.isatab.helper.base_isa_table_file_helper import BaseIsaTableFileHelper
+from metabolights_utils.isatab.default.base_isa_table_file import BaseIsaTableFileReader
 
 
-class SampleFileHelper(BaseIsaTableFileHelper):
+class DefaultSampleFileReader(BaseIsaTableFileReader):
     patterns = [
         ["^(Source Name)$", ""],
         ["^Characteristics\[(\w[ -~]*)\]$", "Characteristics"],
         ["^(Protocol REF)(\.\d+)?$", "Protocol"],
         ["^(Sample Name)$", ""],
         ["^Factor Value\[(\w[ -~]*)\]$", "Factor Value"],
         ["^Comment\b\[(\w{1}[ -~]*)\]$", "Comment"],
     ]
 
     def __init__(self, results_per_page=100) -> None:
         super().__init__(results_per_page=results_per_page)
 
     def _get_expected_patterns(self) -> List[List[str]]:
-        return SampleFileHelper.patterns
+        return DefaultSampleFileReader.patterns
```

### Comparing `metabolights_utils-0.9.2/metabolights_utils/isatab/isa_table_file_reader.py` & `metabolights_utils-0.9.3/metabolights_utils/isatab/reader.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,24 +3,56 @@
 from io import IOBase
 from typing import List, Union
 
 from pydantic import Field
 
 from metabolights_utils.models.common import MetabolightsBaseModel
 from metabolights_utils.models.isa.common import IsaTableFile
+from metabolights_utils.models.isa.investigation_file import Investigation
 from metabolights_utils.models.isa.parser.filter import TsvFileFilterOption
 from metabolights_utils.models.isa.parser.sort import TsvFileSortOption
 from metabolights_utils.models.parser.common import ParserReport
 
 
 class IsaTableFileReaderResult(MetabolightsBaseModel):
     isa_table_file: IsaTableFile = Field(IsaTableFile())
     parser_report: ParserReport = Field(ParserReport())
 
 
+class InvestigationFileReaderResult(MetabolightsBaseModel):
+    investigation: Investigation = Field(Investigation())
+    parser_report: ParserReport = Field(ParserReport())
+
+
+class InvestigationFileReader(ABC):
+    @abstractmethod
+    def read(
+        self,
+        file_buffer: IOBase = None,
+        file_path: Union[str, pathlib.Path] = None,
+        skip_parser_info_messages: bool = True,
+    ) -> InvestigationFileReaderResult:
+        """Reads investigation an file and return Investigation model and parser messages.
+            If file buffer is not defined, it reads file_path.
+           At least one of the file_buffer and file_path parameters should be defined.
+
+        Args:
+            file_buffer (IOBase): File buffer to read file content.
+            io.StringIO, io.TextIOWrapper with open(), etc. Defaults to None.
+            file_path (Union[str, pathlib.Path], optional): File path or pathlib.Path object. Defaults to None.
+            skip_parser_info_messages (bool, optional): clear INFO messages from parser messages. Defaults to True.
+
+        Raises:
+            exc: any unexpected exception while reading file
+
+        Returns:
+            InvestigationFileReaderResult: Investigation model and parser messages
+        """
+
+
 class IsaTableFileReader(ABC):
     @abstractmethod
     def get_headers(
         self,
         file_buffer: IOBase,
         file_path: Union[str, pathlib.Path] = None,
     ) -> IsaTableFileReaderResult:
@@ -30,15 +62,14 @@
             file_buffer (IOBase): File buffer to read file content. io.StringIO, io.TextIOWrapper with open(), etc.
             results_per_page (int): Items per page. Defaults: 100.
             file_path (Union[str, pathlib.Path], optional): File path or pathlib.Path object.
 
         Returns:
             IsaTableFileWrapperResult: Returns IsaTableFile without rows and parser messages.
         """
-        pass
 
     @abstractmethod
     def get_total_pages(
         self,
         file_buffer: IOBase = None,
         results_per_page: int = 100,
         file_path: Union[str, pathlib.Path] = None,
@@ -69,15 +100,14 @@
         Args:
             file_buffer (IOBase): File buffer to read file content. io.StringIO, io.TextIOWrapper with open(), etc.
             file_path (Union[str, pathlib.Path], optional): File path or pathlib.Path object.
 
         Returns:
             int: total number of rows in file. First column is assigned as header row.
         """
-        pass
 
     @abstractmethod
     def get_page(
         self,
         file_buffer: IOBase = None,
         page: int = 1,
         results_per_page: int = 100,
@@ -126,16 +156,14 @@
             filter_options (List[TsvFileFilterOption]): filter column names and filter methods. Defaults to None.
             sort_options (List[TsvFileSortOption]): Sort column names. Defaults to None.
 
         Returns:
             IsaTableFileReaderResult: IsaTableFile model and parser messages.
         """
 
-        pass
-
     @abstractmethod
     def read(
         self,
         file_path_or_buffer: Union[str, pathlib.Path, IOBase],
         file_path: Union[str, pathlib.Path] = None,
         offset: Union[None, int] = 0,
         limit: Union[None, int] = 1000,
@@ -155,8 +183,25 @@
             column_names (Union[List[str], None], optional): Column names will be returned. Returns all columns if it is None. Defaults to None.
             skip_parser_info_messages (bool, optional): clear INFO messages from parser messages. Defaults to True.
             filter_options (List[TsvFileFilterOption]): filter column names and filter methods. Defaults to None.
             sort_options (List[TsvFileSortOption]): Sort column names. Defaults to None.
         Returns:
             IsaTableFileReaderResult: IsaTableFile model and parser messages.
         """
+
+
+class IsaTabReaderFactory(ABC):
+    @abstractmethod
+    def get_investigation_file_reader(self) -> InvestigationFileReader:
+        pass
+
+    @abstractmethod
+    def get_assay_file_reader(self, results_per_page=100) -> IsaTableFileReader:
+        pass
+
+    @abstractmethod
+    def get_sample_file_reader(self, results_per_page=100) -> IsaTableFileReader:
+        pass
+
+    @abstractmethod
+    def get_assignment_file_reader(self, results_per_page=100) -> IsaTableFileReader:
         pass
```

### Comparing `metabolights_utils-0.9.2/metabolights_utils/isatab/isatab_file_helper.py` & `metabolights_utils-0.9.3/metabolights_utils/isatab/default/factory.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,40 @@
-from metabolights_utils.isatab.helper.assay_file_helper import AssayFileHelper
-from metabolights_utils.isatab.helper.assignment_file_helper import AssignmentFileHelper
-from metabolights_utils.isatab.helper.investigation_file_helper import InvestigationFileHelper
-from metabolights_utils.isatab.helper.sample_file_helper import SampleFileHelper
-from metabolights_utils.isatab.investigation_file_reader import InvestigationFileReader
-from metabolights_utils.isatab.investigation_file_writer import InvestigationFileWriter
-from metabolights_utils.isatab.isa_table_file_reader import IsaTableFileReader
-from metabolights_utils.isatab.isa_table_file_writer import (
-    IsaTableFileWriter,
-    IsaTableFileWriterImpl,
+from metabolights_utils.isatab.default.assay_file import DefaultAssayFileReader
+from metabolights_utils.isatab.default.assignment_file import (
+    DefaultAssignmentFileReader,
 )
+from metabolights_utils.isatab.default.investigation_file import (
+    DefaultInvestigationFileReader,
+    DefaultInvestigationFileWriter,
+)
+from metabolights_utils.isatab.default.sample_file import DefaultSampleFileReader
+from metabolights_utils.isatab.default.writer import DefaultIsaTableFileWriter
+from metabolights_utils.isatab.reader import InvestigationFileReader, IsaTabReaderFactory, IsaTableFileReader
+from metabolights_utils.isatab.writer import InvestigationFileWriter, IsaTabWriterFactory, IsaTableFileWriter
+
+
+class DefaultIsaTabReaderFactory(IsaTabReaderFactory):
+    def get_investigation_file_reader(self) -> InvestigationFileReader:
+        return DefaultInvestigationFileReader()
+
+    def get_assay_file_reader(self, results_per_page=100) -> IsaTableFileReader:
+        return DefaultAssayFileReader(results_per_page=results_per_page)
+
+    def get_sample_file_reader(self, results_per_page=100) -> IsaTableFileReader:
+        return DefaultSampleFileReader(results_per_page=results_per_page)
+
+    def get_assignment_file_reader(self, results_per_page=100) -> IsaTableFileReader:
+        return DefaultAssignmentFileReader(results_per_page=results_per_page)
+
+
+class DefaultIsaTabWriterFactory(IsaTabWriterFactory):
+    def get_investigation_file_writer(self) -> InvestigationFileWriter:
+        return DefaultInvestigationFileWriter()
+
+    def get_assay_file_writer(self) -> IsaTableFileWriter:
+        return DefaultIsaTableFileWriter()
 
+    def get_sample_file_writer(self) -> IsaTableFileWriter:
+        return DefaultIsaTableFileWriter()
 
-class IsaTabFileHelper(object):
-    @staticmethod
-    def get_investigation_file_reader() -> InvestigationFileReader:
-        return InvestigationFileHelper()
-
-    @staticmethod
-    def get_investigation_file_writer() -> InvestigationFileWriter:
-        return InvestigationFileHelper()
-
-    @staticmethod
-    def get_assay_file_reader(results_per_page=100) -> IsaTableFileReader:
-        return AssayFileHelper(results_per_page=results_per_page)
-
-    @staticmethod
-    def get_assay_file_writer() -> IsaTableFileWriter:
-        return IsaTableFileWriterImpl()
-
-    @staticmethod
-    def get_sample_file_reader(results_per_page=100) -> IsaTableFileReader:
-        return SampleFileHelper(results_per_page=results_per_page)
-
-    @staticmethod
-    def get_sample_file_writer() -> IsaTableFileWriter:
-        return IsaTableFileWriterImpl()
-
-    @staticmethod
-    def get_assignment_file_reader(results_per_page=100) -> IsaTableFileReader:
-        return AssignmentFileHelper(results_per_page=results_per_page)
-
-    @staticmethod
-    def get_assignment_file_writer() -> IsaTableFileWriter:
-        return IsaTableFileWriterImpl()
+    def get_assignment_file_writer(self) -> IsaTableFileWriter:
+        return DefaultIsaTableFileWriter()
```

### Comparing `metabolights_utils-0.9.2/metabolights_utils/models/isa/assay_file.py` & `metabolights_utils-0.9.3/metabolights_utils/models/isa/assay_file.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.2/metabolights_utils/models/isa/common.py` & `metabolights_utils-0.9.3/metabolights_utils/models/isa/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,19 +109,20 @@
 
 
 class IsaAbstractModel(MetabolightsBaseModel):
     field_order: Union[None, List[str]] = Field(None, auto_fill=False)
 
     class Config:
         extra = Extra.forbid
+
     @classmethod
     def get_attribute(cls, model: BaseModel, attribute_name):
         model_attribute_key = humps.decamelize(attribute_name)
         return getattr(model, model_attribute_key)
-        
+
     @classmethod
     def is_empty_model(cls, model: BaseModel):
         schema = model.schema()
         for item_key in schema["properties"]:
             item_field_definition = schema["properties"][item_key]
             if (
                 not item_field_definition
@@ -163,15 +164,17 @@
     term: str = ""
     term_source_ref: str = ""
     term_accession_number: str = ""
 
     def __str__(self) -> str:
         if self.term:
             if self.term_source_ref or self.term_accession_number:
-                return f"{self.term} [{self.term_source_ref}:{self.term_accession_number}]"
+                return (
+                    f"{self.term} [{self.term_source_ref}:{self.term_accession_number}]"
+                )
             else:
                 return self.term
         return ""
 
     def __eq__(self, other):
         return self.__str__() == other.__str__()
```

### Comparing `metabolights_utils-0.9.2/metabolights_utils/models/isa/investigation_file.py` & `metabolights_utils-0.9.3/metabolights_utils/models/isa/investigation_file.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,33 +20,46 @@
 class OntologySourceReference(IsaAbstractModel):
     field_order: List[str] = [
         "source_name",
         "source_file",
         "source_version",
         "source_description",
     ]
-    source_name: str = Field("", source_description=True, auto_fill=True, header_name="Source Name")
+    source_name: str = Field(
+        "", source_description=True, auto_fill=True, header_name="Source Name"
+    )
     source_file: str = Field("", auto_fill=True, header_name="Source File")
     source_version: str = Field("", auto_fill=True, header_name="Source Version")
-    source_description: str = Field("", auto_fill=True, header_name="Source Description")
+    source_description: str = Field(
+        "", auto_fill=True, header_name="Source Description"
+    )
 
 
 class OntologyAnnotation(IsaAbstractModel):
     field_order: List[str] = ["term", "term_accession_number", "term_source_ref"]
 
     term: str = Field("", auto_fill=True, header_name="")
-    term_accession_number: str = Field("", auto_fill=True, header_name="Term Accession Number")
+    term_accession_number: str = Field(
+        "", auto_fill=True, header_name="Term Accession Number"
+    )
     term_source_ref: str = Field("", auto_fill=True, header_name="Term Source REF")
 
 
 class ValueTypeAnnotation(IsaAbstractModel):
-    field_order: List[str] = ["name", "type", "term_accession_number", "term_source_ref"]
+    field_order: List[str] = [
+        "name",
+        "type",
+        "term_accession_number",
+        "term_source_ref",
+    ]
     name: str = Field("", auto_fill=True, header_name="Name")
     type: str = Field("", auto_fill=True, header_name="Type")
-    term_accession_number: str = Field("", auto_fill=True, header_name="Type Term Accession Number")
+    term_accession_number: str = Field(
+        "", auto_fill=True, header_name="Type Term Accession Number"
+    )
     term_source_ref: str = Field("", auto_fill=True, header_name="Type Term Source REF")
 
 
 class Publication(IsaAbstractModel):
     field_order: List[str] = ["pub_med_id", "doi", "author_list", "title", "status"]
 
     pub_med_id: str = Field("", auto_fill=True, header_name="PubMed ID")
@@ -86,15 +99,17 @@
         seperator=";",
     )
 
 
 class Factor(IsaAbstractModel):
     field_order: List[str] = ["name", "type"]
     name: str = Field("", auto_fill=True, header_name="Name")
-    type: OntologyAnnotation = Field(OntologyAnnotation(), auto_fill=True, header_name="Type")
+    type: OntologyAnnotation = Field(
+        OntologyAnnotation(), auto_fill=True, header_name="Type"
+    )
 
 
 class Assay(IsaAbstractModel):
     field_order: List[str] = [
         "file_name",
         "measurement_type",
         "technology_type",
@@ -103,15 +118,17 @@
     file_name: str = Field("", auto_fill=True, header_name="File Name")
     measurement_type: OntologyAnnotation = Field(
         OntologyAnnotation(), auto_fill=True, header_name="Measurement Type"
     )
     technology_type: OntologyAnnotation = Field(
         OntologyAnnotation(), auto_fill=True, header_name="Technology Type"
     )
-    technology_platform: str = Field("", auto_fill=True, header_name="Technology Platform")
+    technology_platform: str = Field(
+        "", auto_fill=True, header_name="Technology Platform"
+    )
 
 
 class Protocol(IsaAbstractModel):
     field_order: List[str] = [
         "name",
         "protocol_type",
         "description",
@@ -168,22 +185,26 @@
 
 
 class InvestigationContacts(BaseSection):
     section_header: str = Field("INVESTIGATION CONTACTS", exclude=True)
     section_prefix: str = Field("Person", exclude=True)
 
     field_order: List[str] = ["people"]
-    people: List[Person] = Field([], auto_fill=True, header_name="", search_header="Last Name")
+    people: List[Person] = Field(
+        [], auto_fill=True, header_name="", search_header="Last Name"
+    )
 
 
 class StudyDesignDescriptors(BaseSection):
     field_order: List[str] = ["design_types"]
     section_header: str = Field("STUDY DESIGN DESCRIPTORS", exclude=True)
     section_prefix: str = Field("Design", exclude=True)
-    design_types: List[OntologyAnnotation] = Field([], auto_fill=True, header_name="Type")
+    design_types: List[OntologyAnnotation] = Field(
+        [], auto_fill=True, header_name="Type"
+    )
 
 
 class StudyPublications(BaseSection):
     field_order: List[str] = ["publications"]
     section_header: str = Field("STUDY PUBLICATIONS", exclude=True)
     section_prefix: str = Field("", exclude=True)
     publications: List[Publication] = Field(
@@ -191,36 +212,44 @@
     )
 
 
 class StudyFactors(BaseSection):
     field_order: List[str] = ["factors"]
     section_header: str = Field("STUDY FACTORS", exclude=True)
     section_prefix: str = Field("Factor", exclude=True)
-    factors: List[Factor] = Field([], auto_fill=True, header_name="", search_header="Name")
+    factors: List[Factor] = Field(
+        [], auto_fill=True, header_name="", search_header="Name"
+    )
 
 
 class StudyAssays(BaseSection):
     field_order: List[str] = ["assays"]
     section_header: str = Field("STUDY ASSAYS", exclude=True)
     section_prefix: str = Field("Assay", exclude=True)
-    assays: List[Assay] = Field([], auto_fill=True, header_name="", search_header="File Name")
+    assays: List[Assay] = Field(
+        [], auto_fill=True, header_name="", search_header="File Name"
+    )
 
 
 class StudyProtocols(BaseSection):
     field_order: List[str] = ["protocols"]
     section_header: str = Field("STUDY PROTOCOLS", exclude=True)
     section_prefix: str = Field("Protocol", exclude=True)
-    protocols: List[Protocol] = Field([], auto_fill=True, header_name="", search_header="Name")
+    protocols: List[Protocol] = Field(
+        [], auto_fill=True, header_name="", search_header="Name"
+    )
 
 
 class StudyContacts(BaseSection):
     field_order: List[str] = ["people"]
     section_header: str = Field("STUDY CONTACTS", exclude=True)
     section_prefix: str = Field("Person", exclude=True)
-    people: List[Person] = Field([], auto_fill=True, header_name="", search_header="Last Name")
+    people: List[Person] = Field(
+        [], auto_fill=True, header_name="", search_header="Last Name"
+    )
 
 
 class Study(BaseSection):
     field_order: List[str] = [
         "identifier",
         "title",
         "description",
@@ -230,27 +259,33 @@
     ]
     section_header: str = Field("STUDY", exclude=True)
     section_prefix: str = Field("Study", exclude=True)
     identifier: str = Field("", auto_fill=True, header_name="Identifier")
     title: str = Field("", auto_fill=True, header_name="Title")
     description: str = Field("", auto_fill=True, header_name="Description")
     submission_date: str = Field("", auto_fill=True, header_name="Submission Date")
-    public_release_date: str = Field("", auto_fill=True, header_name="Public Release Date")
+    public_release_date: str = Field(
+        "", auto_fill=True, header_name="Public Release Date"
+    )
     file_name: str = Field("", auto_fill=True, header_name="File Name")
 
     study_design_descriptors: StudyDesignDescriptors = Field(
         StudyDesignDescriptors(), auto_fill=True, header_name=""
     )
     study_publications: StudyPublications = Field(
         StudyPublications(), auto_fill=True, header_name=""
     )
     study_factors: StudyFactors = Field(StudyFactors(), auto_fill=True, header_name="")
     study_assays: StudyAssays = Field(StudyAssays(), auto_fill=True, header_name="")
-    study_protocols: StudyProtocols = Field(StudyProtocols(), auto_fill=True, header_name="")
-    study_contacts: StudyContacts = Field(StudyContacts(), auto_fill=True, header_name="")
+    study_protocols: StudyProtocols = Field(
+        StudyProtocols(), auto_fill=True, header_name=""
+    )
+    study_contacts: StudyContacts = Field(
+        StudyContacts(), auto_fill=True, header_name=""
+    )
 
 
 class Investigation(BaseSection):
     section_header: str = Field("INVESTIGATION", exclude=True)
     section_prefix: str = Field("Investigation", exclude=True)
     field_order: List[str] = [
         "identifier",
@@ -262,15 +297,17 @@
     specification_version: str = Field("1.0")
     specification_date: str = Field("2016-10-28")
 
     identifier: str = Field("", auto_fill=True, header_name="Identifier")
     title: str = Field("", auto_fill=True, header_name="Title")
     description: str = Field("", auto_fill=True, header_name="Description")
     submission_date: str = Field("", auto_fill=True, header_name="Submission Date")
-    public_release_date: str = Field("", auto_fill=True, header_name="Public Release Date")
+    public_release_date: str = Field(
+        "", auto_fill=True, header_name="Public Release Date"
+    )
 
     ontology_source_references: OntologySourceReferences = Field(
         OntologySourceReferences(), auto_fill=True, header_name="", inherit_prefix=False
     )
     investigation_publications: InvestigationPublications = Field(
         InvestigationPublications(), auto_fill=True, header_name=""
     )
```

### Comparing `metabolights_utils-0.9.2/metabolights_utils/models/isa/parser/common.py` & `metabolights_utils-0.9.3/metabolights_utils/models/isa/parser/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,18 @@
 from pydantic import BaseModel
 from metabolights_utils.models.common import MetabolightsBaseModel
 
 from metabolights_utils.models.isa.common import (
     INVESTIGATION_FILE_INITIAL_ROWS_SET,
     INVESTIGATION_FILE_STUDY_ROWS_SET,
 )
-from metabolights_utils.models.isa.parser.filter import TsvFileFilterOption, get_filter_operation
+from metabolights_utils.models.isa.parser.filter import (
+    TsvFileFilterOption,
+    get_filter_operation,
+)
 from metabolights_utils.models.isa.parser.sort import (
     TsvFileSortOption,
     get_sorter,
     sort_by_multiple_column,
 )
 from metabolights_utils.models.parser.common import ParserMessage
 from metabolights_utils.models.parser.enums import ParserMessageType
@@ -52,15 +55,17 @@
                 cleared_item in INVESTIGATION_FILE_STUDY_ROWS_SET
                 or cleared_item in INVESTIGATION_FILE_INITIAL_ROWS_SET
                 or cleared_item.startswith("Comment")
             ):
                 if richtext_lines:
                     if not tracked_lines:
                         tracked_lines.append("")
-                    tracked_lines[-1] = tracked_lines[-1] + "\n" + "\n".join(richtext_lines)
+                    tracked_lines[-1] = (
+                        tracked_lines[-1] + "\n" + "\n".join(richtext_lines)
+                    )
                     richtext_lines = []
 
                 tracked_lines.append(token.replace("Comment ", "Comment", 1))
             else:
                 if not richtext_lines:
                     richtext_lines = []
                 richtext_lines.append(token)
@@ -77,15 +82,17 @@
 
             first_item = result[0]
             for item in result:
                 complete_line = False
                 if cleared_lines:
                     previous: str = cleared_lines[-1]
                     if (
-                        previous.startswith('"') and len(previous) > 1 and previous.endswith('"')
+                        previous.startswith('"')
+                        and len(previous) > 1
+                        and previous.endswith('"')
                     ) or (not previous.startswith('"')):
                         complete_line = True
                 else:
                     complete_line = True
                 if complete_line:
                     cleared_lines.append(item)
                 else:
@@ -178,15 +185,17 @@
             filter_options,
             sort_options,
         )
 
     content.total_filtered_rows = total_data_rows
     offset = 0 if not offset else offset
 
-    content.offset = offset if offset < content.total_filtered_rows else content.total_filtered_rows
+    content.offset = (
+        offset if offset < content.total_filtered_rows else content.total_filtered_rows
+    )
 
     if content.offset < 0:
         content.offset = 0
     remaining_row_count = content.total_filtered_rows - content.offset
 
     if limit is None:
         content.limit = (
@@ -225,15 +234,18 @@
             else:
                 if offset and skipped_rows < offset:
                     skipped_rows += 1
                     continue
                 if not limit or (limit and read_rows < limit):
                     read_rows += 1
                     add_tsv_file_data_row(
-                        row, row_index - 1, columns, selected_column_indices=selected_column_indices
+                        row,
+                        row_index - 1,
+                        columns,
+                        selected_column_indices=selected_column_indices,
                     )
     except Exception as exc:
         message = ParserMessage(type=ParserMessageType.CRITICAL)
         message.short = f"ISA table file can not be read successfully."
         message.detail = f"Returned result is not complete. {str(exc)}"
         messages.append(message)
         return SelectedTsvFileContent()
@@ -272,25 +284,29 @@
                     selected_column_indices,
                 )
                 if filter_options:
                     for filter_option in filter_options:
                         filter_operation = get_filter_operation(filter_option)
                         if filter_option.column_name not in filter_operations:
                             filter_operations[filter_option.column_name] = []
-                        filter_operations[filter_option.column_name].append(filter_operation)
+                        filter_operations[filter_option.column_name].append(
+                            filter_operation
+                        )
             else:
                 if not filter_options:
                     filtered_rows.append((row_index - 1, row))
                 else:
                     selected = True
 
                     for filter_option in filter_options:
                         col_index = column_name_indices[filter_option.column_name]
                         val = row[col_index]
-                        for filter_operation in filter_operations[filter_option.column_name]:
+                        for filter_operation in filter_operations[
+                            filter_option.column_name
+                        ]:
                             if not filter_operation(val):
                                 selected = False
                                 break
                         if not selected:
                             break
                     if selected:
                         filtered_rows.append((row_index - 1, row))
@@ -304,47 +320,57 @@
                 sort_list.append((row_sorter, sort_option.reverse))
         filtered_rows = sort_by_multiple_column(filtered_rows, sort_list)
 
         content.total_filtered_rows = len(filtered_rows)
         offset = 0 if not offset else offset
 
         content.offset = (
-            offset if offset < content.total_filtered_rows else content.total_filtered_rows
+            offset
+            if offset < content.total_filtered_rows
+            else content.total_filtered_rows
         )
         remaining_row_count = content.total_filtered_rows - content.offset
         if limit is None:
             content.limit = (
                 remaining_row_count
                 if remaining_row_count <= content.total_filtered_rows
                 else content.total_filtered_rows
             )
         else:
-            content.limit = remaining_row_count if remaining_row_count < limit else limit
+            content.limit = (
+                remaining_row_count if remaining_row_count < limit else limit
+            )
 
         skipped_rows = 0
         read_rows = 0
         for data_row_index, row in filtered_rows:
             if offset and skipped_rows < offset:
                 skipped_rows += 1
                 continue
             if not limit or (limit and read_rows < limit):
                 read_rows += 1
                 add_tsv_file_data_row(
-                    row, data_row_index, columns, selected_column_indices=selected_column_indices
+                    row,
+                    data_row_index,
+                    columns,
+                    selected_column_indices=selected_column_indices,
                 )
     except Exception as exc:
         message = ParserMessage(type=ParserMessageType.CRITICAL)
         message.short = f"ISA table file can not be read successfully."
         message.detail = f"Returned result is not complete. {str(exc)}"
         messages.append(message)
     return content
 
 
 def add_tsv_file_data_row(
-    data_row, row_index: int, columns: Dict[str, TsvColumn], selected_column_indices: Dict[int, str]
+    data_row,
+    row_index: int,
+    columns: Dict[str, TsvColumn],
+    selected_column_indices: Dict[int, str],
 ):
     for column_index in selected_column_indices:
         column = columns[selected_column_indices[column_index]]
         column.rows[row_index] = data_row[column_index]
 
 
 def prepare_column_names(
@@ -375,15 +401,17 @@
         for name in selected_column_names:
             if name in new_ordered_columns:
                 continue
             if name == "Unit" or name.startswith("Unit."):
                 continue
             elif name == "Term Source REF" or name.startswith("Term Source REF."):
                 continue
-            elif name == "Term Accession Number" or name.startswith("Term Accession Number."):
+            elif name == "Term Accession Number" or name.startswith(
+                "Term Accession Number."
+            ):
                 continue
             elif name not in column_name_indices:
                 invalid_column_names.append(name)
                 continue
             else:
                 new_ordered_columns.append(name)
                 col_index = column_name_indices[name]
@@ -394,23 +422,27 @@
                         new_ordered_columns.append(next)
                         term_source_relative_index = 2
 
                 if col_index + term_source_relative_index + 1 < len(header_row):
                     next: str = column_indices[col_index + term_source_relative_index]
                     if next == "Term Source REF" or next.startswith("Term Source REF."):
                         new_ordered_columns.append(next)
-                        next: str = column_indices[col_index + term_source_relative_index + 1]
+                        next: str = column_indices[
+                            col_index + term_source_relative_index + 1
+                        ]
                         if next == "Term Accession Number" or next.startswith(
                             "Term Accession Number."
                         ):
                             new_ordered_columns.append(next)
         selected_column_names.clear()
         selected_column_names.extend(new_ordered_columns)
     if invalid_column_names:
-        raise TypeError(f"Column(s) do(es) not exist: " + ", ".join(invalid_column_names))
+        raise TypeError(
+            f"Column(s) do(es) not exist: " + ", ".join(invalid_column_names)
+        )
 
 
 def read_tsv_file_header(
     content: SelectedTsvFileContent,
     header_row,
     column_names: Union[None, List[str]],
     columns: Dict[str, TsvColumn],
@@ -424,25 +456,29 @@
 
     try:
         if column_names:
             for column_name in column_names:
                 col_index = column_name_indices[column_name]
                 column_header = header_row[col_index]
                 column = TsvColumn(
-                    column_index=col_index, column_header=column_header, column_name=column_name
+                    column_index=col_index,
+                    column_header=column_header,
+                    column_name=column_name,
                 )
                 columns[column_name] = column
                 selected_column_indices[col_index] = column_name
                 content.columns.append(column)
         else:
             for col_index in range(len(header_row)):
                 column_name = column_indices[col_index]
                 column_header = header_row[col_index]
                 column = TsvColumn(
-                    column_index=col_index, column_header=column_header, column_name=column_name
+                    column_index=col_index,
+                    column_header=column_header,
+                    column_name=column_name,
                 )
                 columns[column_name] = column
                 selected_column_indices[col_index] = column_name
                 content.columns.append(column)
 
         # if column_names:
         #     invalid_column_names = []
```

### Comparing `metabolights_utils-0.9.2/metabolights_utils/models/isa/parser/filter.py` & `metabolights_utils-0.9.3/metabolights_utils/models/isa/parser/filter.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,16 +2,19 @@
 from datetime import datetime
 from enum import Enum
 from functools import partial
 from typing import Any, Dict, Union
 
 from pydantic import BaseModel
 
-from metabolights_utils.models.isa.common import FilterOperation, FilterParameterType, TsvFileFilterOption
-
+from metabolights_utils.models.isa.common import (
+    FilterOperation,
+    FilterParameterType,
+    TsvFileFilterOption,
+)
 
 
 def get_filter_operation(filter_option: TsvFileFilterOption):
     def filter(filter_option: TsvFileFilterOption, row_value: str):
         filter_method = FILTER_METHODS[filter_option.operation]
         if filter_option.negate_result:
             return not filter_method(filter_option, row_value)
@@ -33,25 +36,29 @@
 
 
 def filter_startswith(filter_option: TsvFileFilterOption, row_value: str) -> bool:
     if filter_option.case_sensitive:
         if row_value and str(row_value).startswith(str(filter_option.parameter)):
             return True
     else:
-        if row_value and str(row_value).lower().startswith(str(filter_option.parameter).lower()):
+        if row_value and str(row_value).lower().startswith(
+            str(filter_option.parameter).lower()
+        ):
             return True
     return False
 
 
 def filter_endswith(filter_option: TsvFileFilterOption, row_value: str) -> bool:
     if filter_option.case_sensitive:
         if row_value and str(row_value).endswith(str(filter_option.parameter)):
             return True
     else:
-        if row_value and str(row_value).lower().endswith(str(filter_option.parameter).lower()):
+        if row_value and str(row_value).lower().endswith(
+            str(filter_option.parameter).lower()
+        ):
             return True
     return False
 
 
 def filter_equal(filter_option: TsvFileFilterOption, row_value: str) -> bool:
     if filter_option.case_sensitive:
         if row_value and str(row_value) == str(filter_option.parameter):
@@ -63,27 +70,39 @@
 
 
 def filter_greater(filter_option: TsvFileFilterOption, row_value: str) -> bool:
     if row_value:
         try:
             if filter_option.parameter_type == FilterParameterType.AUTO:
                 if isinstance(filter_option.parameter, int):
-                    return True if int(row_value) > int(filter_option.parameter) else False
+                    return (
+                        True if int(row_value) > int(filter_option.parameter) else False
+                    )
                 elif isinstance(filter_option.parameter, float):
-                    return True if float(row_value) > float(filter_option.parameter) else False
+                    return (
+                        True
+                        if float(row_value) > float(filter_option.parameter)
+                        else False
+                    )
                 else:
-                    return True if str(row_value) > str(filter_option.parameter) else False
+                    return (
+                        True if str(row_value) > str(filter_option.parameter) else False
+                    )
             elif filter_option.parameter_type == FilterParameterType.INTEGER:
                 return True if int(row_value) > int(filter_option.parameter) else False
             elif filter_option.parameter_type == FilterParameterType.FLOAT:
-                return True if float(row_value) > float(filter_option.parameter) else False
+                return (
+                    True if float(row_value) > float(filter_option.parameter) else False
+                )
             elif filter_option.parameter_type == FilterParameterType.DATETIME:
                 return (
                     True
-                    if datetime.strptime(row_value, filter_option.default_datetime_pattern)
+                    if datetime.strptime(
+                        row_value, filter_option.default_datetime_pattern
+                    )
                     > datetime.strptime(
                         filter_option.parameter, filter_option.default_datetime_pattern
                     )
                     else False
                 )
             else:
                 return True if str(row_value) > str(filter_option.parameter) else False
@@ -93,27 +112,45 @@
 
 
 def filter_greater_equal(filter_option: TsvFileFilterOption, row_value: str) -> bool:
     if row_value:
         try:
             if filter_option.parameter_type == FilterParameterType.AUTO:
                 if isinstance(filter_option.parameter, int):
-                    return True if int(row_value) >= int(filter_option.parameter) else False
+                    return (
+                        True
+                        if int(row_value) >= int(filter_option.parameter)
+                        else False
+                    )
                 elif isinstance(filter_option.parameter, float):
-                    return True if float(row_value) >= float(filter_option.parameter) else False
+                    return (
+                        True
+                        if float(row_value) >= float(filter_option.parameter)
+                        else False
+                    )
                 else:
-                    return True if str(row_value) >= str(filter_option.parameter) else False
+                    return (
+                        True
+                        if str(row_value) >= str(filter_option.parameter)
+                        else False
+                    )
             elif filter_option.parameter_type == FilterParameterType.INTEGER:
                 return True if int(row_value) >= int(filter_option.parameter) else False
             elif filter_option.parameter_type == FilterParameterType.FLOAT:
-                return True if float(row_value) >= float(filter_option.parameter) else False
+                return (
+                    True
+                    if float(row_value) >= float(filter_option.parameter)
+                    else False
+                )
             elif filter_option.parameter_type == FilterParameterType.DATETIME:
                 return (
                     True
-                    if datetime.strptime(row_value, filter_option.default_datetime_pattern)
+                    if datetime.strptime(
+                        row_value, filter_option.default_datetime_pattern
+                    )
                     >= datetime.strptime(
                         filter_option.parameter, filter_option.default_datetime_pattern
                     )
                     else False
                 )
             else:
                 return True if str(row_value) >= str(filter_option.parameter) else False
@@ -136,15 +173,17 @@
             elif param_type == FilterParameterType.INTEGER:
                 return True if int(row_value) < int(param) else False
             elif param_type == FilterParameterType.FLOAT:
                 return True if float(row_value) < float(param) else False
             elif param_type == FilterParameterType.DATETIME:
                 return (
                     True
-                    if datetime.strptime(row_value, filter_option.default_datetime_pattern)
+                    if datetime.strptime(
+                        row_value, filter_option.default_datetime_pattern
+                    )
                     < datetime.strptime(param, filter_option.default_datetime_pattern)
                     else False
                 )
             else:
                 return True if str(row_value) < str(param) else False
         except:
             return False
@@ -165,15 +204,17 @@
             elif param_type == FilterParameterType.INTEGER:
                 return True if int(row_value) <= int(param) else False
             elif param_type == FilterParameterType.FLOAT:
                 return True if float(row_value) <= float(param) else False
             elif param_type == FilterParameterType.DATETIME:
                 return (
                     True
-                    if datetime.strptime(row_value, filter_option.default_datetime_pattern)
+                    if datetime.strptime(
+                        row_value, filter_option.default_datetime_pattern
+                    )
                     <= datetime.strptime(param, filter_option.default_datetime_pattern)
                     else False
                 )
             else:
                 return True if str(row_value) <= str(param) else False
         except:
             return False
```

### Comparing `metabolights_utils-0.9.2/metabolights_utils/models/isa/parser/investigation_parser.py` & `metabolights_utils-0.9.3/metabolights_utils/models/isa/parser/investigation_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,17 @@
 def parse_investigation_from_fs(
     file_path: str,
 ) -> Tuple[Union[model.Investigation, None], List[ParserMessage]]:
     messages: List[ParserMessage] = []
     basename = os.path.basename(file_path)
     if not os.path.exists(file_path):
         print(f"File does not exist: {basename}")
-        message = ParserMessage(short="File does not exist", type=ParserMessageType.CRITICAL)
+        message = ParserMessage(
+            short="File does not exist", type=ParserMessageType.CRITICAL
+        )
         message.detail = f"File does not exist: {basename}"
         messages.append(message)
         return None, messages
     file_size = os.stat(file_path).st_size
     if file_size == 0:
         print(f"File is empty: {basename}")
         message = ParserMessage(short="File is empty", type=ParserMessageType.CRITICAL)
@@ -41,15 +43,17 @@
         return None, messages
 
     with open(file_path, "r") as f:
         investigation = get_investigation(f, file_path, messages=messages)
         return investigation, messages
 
 
-def get_investigation(file_buffer: IOBase, file_path: str, messages: List[ParserMessage]):
+def get_investigation(
+    file_buffer: IOBase, file_path: str, messages: List[ParserMessage]
+):
     if messages is None:
         messages = []
     index_map = {}
     initial_part = []
     study_parts = []
     initial_part_index_map = {}
     study_parts_index_map = []
@@ -105,28 +109,34 @@
                         short="Invalid ISA comment line", type=ParserMessageType.WARNING
                     )
                     message.detail = f"{message_detail}"
                     message.line = str(line)
                     messages.append(message)
                 continue
             else:
-                message = ParserMessage(short="Invalid line", type=ParserMessageType.ERROR)
+                message = ParserMessage(
+                    short="Invalid line", type=ParserMessageType.ERROR
+                )
                 message.detail = f" {index_string}"
                 messages.append(message)
                 message.line = str(line)
                 continue
 
         if re.match(r"^[A-Z][A-Z0-9 ]+[A-Z0-9]$", index_string):
             current_section = index_string
             if index_string != "STUDY":
                 continue
 
         if not current_section:
-            message = ParserMessage(short="Invalid start section", type=ParserMessageType.ERROR)
-            message.detail = f"Line {str(line + 1)}: {index_string} is not valid section start"
+            message = ParserMessage(
+                short="Invalid start section", type=ParserMessageType.ERROR
+            )
+            message.detail = (
+                f"Line {str(line + 1)}: {index_string} is not valid section start"
+            )
             messages.append(message)
             message.line = str(line)
 
         if not is_study_part:
             if index_string == "STUDY":
                 is_study_part = True
             elif index_string not in INVESTIGATION_FILE_INITIAL_ROWS_SET:
@@ -316,22 +326,28 @@
         field_definition = data_schema["properties"][key]
         if (
             not field_definition
             or "auto_fill" not in field_definition
             or not field_definition["auto_fill"]
         ):
             continue
-        if "inherit_prefix" in field_definition and not field_definition["inherit_prefix"]:
+        if (
+            "inherit_prefix" in field_definition
+            and not field_definition["inherit_prefix"]
+        ):
             name_prefix = prefix.strip() if prefix else ""
 
         if "$ref" in field_definition and field_definition["$ref"]:
             data_type = "ref"
             ref_object_definition = field_definition["$ref"]
         elif "allOf" in field_definition and field_definition["allOf"]:
-            if "$ref" in field_definition["allOf"][0] and field_definition["allOf"][0]["$ref"]:
+            if (
+                "$ref" in field_definition["allOf"][0]
+                and field_definition["allOf"][0]["$ref"]
+            ):
                 data_type = "ref"
                 ref_object_definition = field_definition["allOf"][0]["$ref"]
         elif "anyOf" in field_definition and field_definition["anyOf"]:
             primitives = {"string", "int", "float"}
             for field_item in field_definition["anyOf"]:
                 if "type" in field_item and field_item["type"] in primitives:
                     data_type = "string"
@@ -342,15 +358,18 @@
         if (
             field_definition
             and "text_multiple_value" in field_definition
             and field_definition["text_multiple_value"]
         ):
             text_multiple_value = True
         if field_definition and "header_name" in field_definition:
-            if "section_prefix" in field_definition and field_definition["section_prefix"]:
+            if (
+                "section_prefix" in field_definition
+                and field_definition["section_prefix"]
+            ):
                 field_name = " ".join(
                     [
                         f"{name_prefix}",
                         f"{field_definition['section_prefix']}",
                         f"{field_definition['header_name']}",
                     ]
                 ).strip()
@@ -370,29 +389,33 @@
                                     [
                                         name_prefix,
                                         field_definition["section_prefix"],
                                         field_definition["search_header"],
                                     ]
                                 )
                             else:
-                                search_field = f"{name_prefix} {field_definition['search_header']}"
+                                search_field = (
+                                    f"{name_prefix} {field_definition['search_header']}"
+                                )
 
                         item_list = []
                         set_value(data, key, item_list)
 
                         if search_field not in index_map:
                             print(
                                 f"{search_field} is not in file. Skipping {field_name} in {file_path}"
                             )
                             continue
                         index = index_map[search_field]
 
                         max = len(tab[index])
                         ref_class_name = (
-                            items["$ref"].replace("#/definitions/", "").replace("#/$defs/", "")
+                            items["$ref"]
+                            .replace("#/definitions/", "")
+                            .replace("#/$defs/", "")
                         )
                         ref_class = getattr(
                             sys.modules[model_module_name],
                             ref_class_name,
                         )
                         for i in range(1, max):
                             instance = ref_class()
@@ -416,15 +439,17 @@
                             else:
                                 break
             elif data_type == "array" and text_multiple_value:
                 if "items" in field_definition and field_definition["items"]:
                     items = field_definition["items"]
                     if "$ref" in items and items["$ref"]:
                         ref_class_name = (
-                            items["$ref"].replace("#/definitions/", "").replace("#/$defs/", "")
+                            items["$ref"]
+                            .replace("#/definitions/", "")
+                            .replace("#/$defs/", "")
                         )
                         ref_class = getattr(
                             sys.modules[model_module_name],
                             ref_class_name,
                         )
                         instance = ref_class()
                         set_value(data, key, [instance])
@@ -461,15 +486,17 @@
                             for _ in range(len(seperated_values)):
                                 instance_count = len(new_instances)
                                 values_count = len(seperated_values)
                                 if instance_count < values_count:
                                     for _ in range(instance_count, values_count):
                                         new_instances.append(ref_class())
                                 for j in range(values_count):
-                                    set_value(new_instances[j], item_key, seperated_values[j])
+                                    set_value(
+                                        new_instances[j], item_key, seperated_values[j]
+                                    )
                         count = len(new_instances)
                         for i in range(len(new_instances)):
                             instance_item = new_instances[count - i - 1]
                             if IsaAbstractModel.is_empty_model(model=instance_item):
                                 new_instances.pop()
                             else:
                                 break
@@ -503,17 +530,17 @@
                 value = ""
                 if len(tab[index]) > value_index:
                     value = tab[index][value_index]
                 else:
                     value = ""
                 set_value(data, key, str(value) or "")
             elif data_type == "ref":
-                ref_class_name = ref_object_definition.replace("#/definitions/", "").replace(
-                    "#/$defs/", ""
-                )
+                ref_class_name = ref_object_definition.replace(
+                    "#/definitions/", ""
+                ).replace("#/$defs/", "")
                 ref_class = getattr(sys.modules[model_module_name], ref_class_name)
                 instance = ref_class()
                 set_value(data, key, instance)
                 assign_by_field_name(
                     file_path,
                     instance,
                     index_map,
@@ -521,15 +548,17 @@
                     prefix=field_name,
                     value_index=value_index,
                     messages=messages,
                     comments_map=comments_map,
                 )
             else:
                 if data_type:
-                    message = ParserMessage(short="Invalid data type", type=ParserMessageType.ERROR)
+                    message = ParserMessage(
+                        short="Invalid data type", type=ParserMessageType.ERROR
+                    )
                     message.detail = f"Invalid data type {data_type} in {file_path}"
                     messages.append(message)
                 else:
                     message = ParserMessage(
                         short=f"Invalid data type in {file_path}",
                         type=ParserMessageType.ERROR,
                     )
```

### Comparing `metabolights_utils-0.9.2/metabolights_utils/models/isa/parser/isa_table_parser.py` & `metabolights_utils-0.9.3/metabolights_utils/models/isa/parser/isa_table_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import os
 import re
 from io import IOBase
 from typing import List, Tuple, Union
 
 from metabolights_utils.models.isa.common import IsaTableColumn, IsaTableFile
-from metabolights_utils.models.isa.enums import ColumnsStructure, IsaTableAdditionalColumn
+from metabolights_utils.models.isa.enums import (
+    ColumnsStructure,
+    IsaTableAdditionalColumn,
+)
 from metabolights_utils.models.isa.parser.common import (
     SelectedTsvFileContent,
     TsvFileFilterOption,
     read_table_file,
 )
 from metabolights_utils.models.isa.parser.sort import TsvFileSortOption
 from metabolights_utils.models.parser.common import ParserMessage
@@ -24,25 +27,29 @@
     filter_options: List[TsvFileFilterOption] = None,
     sort_options: List[TsvFileSortOption] = None,
 ) -> Tuple[IsaTableFile, List[ParserMessage]]:
     basename = os.path.basename(file_path)
     dirname = os.path.basename(os.path.dirname(file_path))
     messages: List[ParserMessage] = []
     if not file_path:
-        message = ParserMessage(short="File path is not valid", type=ParserMessageType.CRITICAL)
+        message = ParserMessage(
+            short="File path is not valid", type=ParserMessageType.CRITICAL
+        )
         message.detail = "File path is not valid"
         messages.append(message)
         return IsaTableFile(), messages
 
     if not os.path.exists(file_path) or not os.path.isfile(file_path):
         message = ParserMessage(
             short="File does not exist or it is not a file",
             type=ParserMessageType.CRITICAL,
         )
-        message.detail = f"File does not exist or is not a file: {basename} in {dirname}"
+        message.detail = (
+            f"File does not exist or is not a file: {basename} in {dirname}"
+        )
         messages.append(message)
         return IsaTableFile(), messages
 
     file_size = os.stat(file_path).st_size
     if file_size == 0:
         message = ParserMessage(short="File is empty", type=ParserMessageType.CRITICAL)
         message.detail = f"File is empty: {basename} in {dirname}"
@@ -163,18 +170,22 @@
                 message.short = "Column header starts or ends with space"
                 message.detail = (
                     f"'{column_name}' header at column {column_index + 1} "
                     + "ends or starts with space."
                 )
             else:
                 message.short = "Column header is empty"
-                message.detail = f"'{column_name}' header at column {column_index + 1}  is empty."
+                message.detail = (
+                    f"'{column_name}' header at column {column_index + 1}  is empty."
+                )
             messages.append(message)
 
-    headers = get_headers(columns, expected_patterns=expected_patterns, messages=messages)
+    headers = get_headers(
+        columns, expected_patterns=expected_patterns, messages=messages
+    )
     study_table.table.headers = headers
     study_table.table.total_row_count = content.total_rows
     study_table.table.row_offset = content.offset
     study_table.table.row_count = content.limit
     study_table.table.filtered_total_row_count = content.total_filtered_rows
     study_table.table.selected_column_count = content.selected_column_count
     study_table.table.total_column_count = content.total_columns
@@ -183,15 +194,17 @@
 
     filtered_data = {}
 
     for column in content.columns:
         if not study_table.table.row_indices:
             study_table.table.row_indices = [x for x in column.rows]
         filtered_data[column.column_name] = [column.rows[x] for x in column.rows]
-    study_table.table.column_indices = [column.column_index for column in content.columns]
+    study_table.table.column_indices = [
+        column.column_index for column in content.columns
+    ]
     # data = df.to_dict(orient="list")
     study_table.table.data = filtered_data
     study_table.table.columns = columns
     # study_table.table.row_count = len(content.columns[0].rows)
     study_table.file_path = file_name
 
     return study_table
@@ -219,20 +232,24 @@
             "(Term Source REF)(\.\d+)?",
             "(Term Accession Number)(\.\d+)?",
         ],
     },
 }
 
 additional_column_templates = [
-    MULTI_COLUMN_TEMPLATES[ColumnsStructure.SINGLE_COLUMN_AND_UNIT_ONTOLOGY]["searchPatterns"],
+    MULTI_COLUMN_TEMPLATES[ColumnsStructure.SINGLE_COLUMN_AND_UNIT_ONTOLOGY][
+        "searchPatterns"
+    ],
     MULTI_COLUMN_TEMPLATES[ColumnsStructure.ONTOLOGY_COLUMN]["searchPatterns"],
 ]
 
 additional_column_headers = [
-    MULTI_COLUMN_TEMPLATES[ColumnsStructure.SINGLE_COLUMN_AND_UNIT_ONTOLOGY]["column_names"],
+    MULTI_COLUMN_TEMPLATES[ColumnsStructure.SINGLE_COLUMN_AND_UNIT_ONTOLOGY][
+        "column_names"
+    ],
     MULTI_COLUMN_TEMPLATES[ColumnsStructure.ONTOLOGY_COLUMN]["column_names"],
 ]
 
 multiple_columns_additional_header_patterns = MULTI_COLUMN_TEMPLATES[
     ColumnsStructure.SINGLE_COLUMN_AND_UNIT_ONTOLOGY
 ]["searchPatterns"]
 
@@ -271,28 +288,32 @@
 def get_headers(columns: List[str], expected_patterns, messages: List[ParserMessage]):
     headers = []
     column_index = 0
     columns_count = len(columns)
     while column_index < columns_count:
         column_name = columns[column_index]
         cleaned_column_name = get_cleaned_header(column_name)
-        column_structure, additional_column_headers = define_column_structure(column_index, columns)
+        column_structure, additional_column_headers = define_column_structure(
+            column_index, columns
+        )
 
         result = None
         pattern_index = -1
         expected_header: bool = False
         message = ParserMessage(type=ParserMessageType.INFO)
         for i in range(len(expected_patterns)):
             result = re.search(expected_patterns[i][0], column_name)
             if result and result.groups():
                 pattern_index = i
                 expected_header = result and result.groups()
                 break
 
-        column = IsaTableColumn(column_index=str(column_index), colummn_structure=column_structure)
+        column = IsaTableColumn(
+            column_index=str(column_index), colummn_structure=column_structure
+        )
         column.column_name = column_name
         column.column_header = cleaned_column_name
         linked_columns = []
 
         if column_structure == ColumnsStructure.ADDITIONAL_COLUMN:
             column.column_category = "Additional"
             message.type = ParserMessageType.CRITICAL
@@ -380,15 +401,17 @@
     if expected_header:
         column.column_search_pattern = expected_patterns[pattern_index][0]
         column.column_category = expected_patterns[pattern_index][1]
         column.column_prefix = expected_patterns[pattern_index][1]
     else:
         column.column_category = "Undefined"
         message.type = ParserMessageType.INFO
-        message.short = f"Multi column '{cleaned_column_name}' is not in expected column list."
+        message.short = (
+            f"Multi column '{cleaned_column_name}' is not in expected column list."
+        )
 
 
 def update_as_invalid_column(
     expected_patterns,
     cleaned_column_name,
     pattern_index,
     expected_header,
@@ -419,15 +442,17 @@
     if expected_header:
         column.column_search_pattern = expected_patterns[pattern_index][0]
         column.column_category = expected_patterns[pattern_index][1]
         column.column_prefix = expected_patterns[pattern_index][1]
     else:
         column.column_category = "Undefined"
         message.type = ParserMessageType.INFO
-        message.short = f"Single column '{cleaned_column_name}' is not in expected column list."
+        message.short = (
+            f"Single column '{cleaned_column_name}' is not in expected column list."
+        )
 
 
 def define_column_structure(column_index, columns):
     column_is_additional = False
     for additional_column_pattern in multiple_columns_additional_header_patterns:
         if re.match(additional_column_pattern, columns[column_index]):
             column_is_additional = True
@@ -456,15 +481,17 @@
             )
     else:
         if additional_columns_count > 0:
             return ColumnsStructure.INVALID_MULTI_COLUMN, []
         else:
             next_column_is_additional = False
             if column_index + 1 < columns_count:
-                for additional_column_pattern in multiple_columns_additional_header_patterns:
+                for (
+                    additional_column_pattern
+                ) in multiple_columns_additional_header_patterns:
                     if re.match(additional_column_pattern, columns[column_index + 1]):
                         next_column_is_additional = True
                         break
             if next_column_is_additional:
                 return ColumnsStructure.INVALID_MULTI_COLUMN, []
 
     return ColumnsStructure.SINGLE_COLUMN, []
```

### Comparing `metabolights_utils-0.9.2/metabolights_utils/models/isa/parser/sort.py` & `metabolights_utils-0.9.3/metabolights_utils/models/isa/parser/sort.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,28 +3,36 @@
 from datetime import datetime
 from enum import Enum
 from functools import reduce
 from typing import Any, Dict, List, Tuple, Union
 
 from pydantic import BaseModel
 
-from metabolights_utils.models.isa.common import SortType, SortValueClassification, TsvFileSortOption
+from metabolights_utils.models.isa.common import (
+    SortType,
+    SortValueClassification,
+    TsvFileSortOption,
+)
 
 
-def get_sort_value_order(sort_option: TsvFileSortOption, classification: SortValueClassification):
+def get_sort_value_order(
+    sort_option: TsvFileSortOption, classification: SortValueClassification
+):
     if sort_option.value_order & 0o007 == classification:
         return 3
     elif (sort_option.value_order & 0o070) >> 3 == classification:
         return 2
     return 1
 
 
 def sort_by_multiple_column(sequence, sort_order):
     return reduce(
-        lambda s, order: sorted(s, key=order[0], reverse=order[1]), reversed(sort_order), sequence
+        lambda s, order: sorted(s, key=order[0], reverse=order[1]),
+        reversed(sort_order),
+        sequence,
     )
 
 
 def get_sorter(sort_option: TsvFileSortOption, col_index: int):
     def row_sorter(filtered_row: Tuple[int, List[str]]):
         val = filtered_row[1][col_index]
         sorter = SORTERS[sort_option.column_sort_type]
@@ -34,15 +42,17 @@
 
 
 # SORTERS
 
 
 class AbstractSorter(ABC):
     @abstractmethod
-    def sort(self, sort_option: TsvFileSortOption, value: str) -> Union[int, float, str, datetime]:
+    def sort(
+        self, sort_option: TsvFileSortOption, value: str
+    ) -> Union[int, float, str, datetime]:
         pass
 
 
 class IntegerSorter(AbstractSorter):
     def get_int_value_by_order(self, order: int, valid_value_order: int):
         if order == 1:
             return -sys.maxsize - 1
@@ -52,22 +62,26 @@
             else:
                 return sys.maxsize - 1
         return sys.maxsize
 
     def sort(self, sort_option: TsvFileSortOption, value: str) -> int:
         if not value:
             order = get_sort_value_order(sort_option, SortValueClassification.EMPTY)
-            valid_value_order = get_sort_value_order(sort_option, SortValueClassification.VALID)
+            valid_value_order = get_sort_value_order(
+                sort_option, SortValueClassification.VALID
+            )
             return self.get_int_value_by_order(order, valid_value_order)
 
         try:
             return int(value)
         except Exception as exc:
             order = get_sort_value_order(sort_option, SortValueClassification.INVALID)
-            valid_value_order = get_sort_value_order(sort_option, SortValueClassification.VALID)
+            valid_value_order = get_sort_value_order(
+                sort_option, SortValueClassification.VALID
+            )
             return self.get_int_value_by_order(order, valid_value_order)
 
 
 class FloatSorter(AbstractSorter):
     def get_float_value_by_order(self, order: int, valid_value_order: int):
         if order == 1:
             return sys.float_info.min
@@ -77,50 +91,62 @@
             else:
                 return sys.float_info.max - 1
         return sys.float_info.max
 
     def sort(self, sort_option: TsvFileSortOption, value: str) -> float:
         if not value:
             order = get_sort_value_order(sort_option, SortValueClassification.EMPTY)
-            valid_value_order = get_sort_value_order(sort_option, SortValueClassification.VALID)
+            valid_value_order = get_sort_value_order(
+                sort_option, SortValueClassification.VALID
+            )
             return self.get_float_value_by_order(order, valid_value_order)
 
         try:
             return float(value)
         except Exception as exc:
             order = get_sort_value_order(sort_option, SortValueClassification.INVALID)
-            valid_value_order = get_sort_value_order(sort_option, SortValueClassification.VALID)
+            valid_value_order = get_sort_value_order(
+                sort_option, SortValueClassification.VALID
+            )
             return self.get_float_value_by_order(order, valid_value_order)
 
 
 class DateTimeSorter(AbstractSorter):
-    DATETIME_MIN_MINUS_1 = datetime.min.replace(microsecond=(datetime.min.microsecond + 1))
-    DATETIME_MAX_MINUS_1 = datetime.max.replace(microsecond=(datetime.max.microsecond - 1))
+    DATETIME_MIN_MINUS_1 = datetime.min.replace(
+        microsecond=(datetime.min.microsecond + 1)
+    )
+    DATETIME_MAX_MINUS_1 = datetime.max.replace(
+        microsecond=(datetime.max.microsecond - 1)
+    )
 
     def get_datetime_value_by_order(self, order: int, valid_value_order: int):
         if order == 1:
             return datetime.min
         elif order == 2:
             if valid_value_order > order:
                 return DateTimeSorter.DATETIME_MIN_MINUS_1
             else:
                 return DateTimeSorter.DATETIME_MAX_MINUS_1
         return datetime.max
 
     def sort(self, sort_option: TsvFileSortOption, value: str) -> datetime:
         if not value:
             order = get_sort_value_order(sort_option, SortValueClassification.EMPTY)
-            valid_value_order = get_sort_value_order(sort_option, SortValueClassification.VALID)
+            valid_value_order = get_sort_value_order(
+                sort_option, SortValueClassification.VALID
+            )
             return self.get_datetime_value_by_order(order, valid_value_order)
 
         try:
             return datetime.strptime(value, sort_option.default_datetime_pattern)
         except Exception as exc:
             order = get_sort_value_order(sort_option, SortValueClassification.INVALID)
-            valid_value_order = get_sort_value_order(sort_option, SortValueClassification.VALID)
+            valid_value_order = get_sort_value_order(
+                sort_option, SortValueClassification.VALID
+            )
             return self.get_datetime_value_by_order(order, valid_value_order)
 
 
 class StringSorter(AbstractSorter):
     def sort(self, sort_option: TsvFileSortOption, value: str) -> str:
         if not value:
             return "~"
```

### Comparing `metabolights_utils-0.9.2/metabolights_utils/models/metabolights/metabolights_study.py` & `metabolights_utils-0.9.3/metabolights_utils/models/metabolights/metabolights_study.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.2/metabolights_utils/models/parser/common.py` & `metabolights_utils-0.9.3/metabolights_utils/models/parser/common.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.2/metabolights_utils/tsv/actions/add_column.py` & `metabolights_utils-0.9.3/metabolights_utils/tsv/actions/add_column.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,17 @@
         result: actions.TsvActionResult = actions.TsvActionResult(action=action)
         if action.name != actions.TsvActionName.ADD_COLUMN:
             result.message = "Action name is not valid"
             return result
 
         action: actions.TsvAddColumnsAction = action
 
-        column_data: Dict[int, actions.TsvColumnData] = action.columns if action.columns else {}
+        column_data: Dict[int, actions.TsvColumnData] = (
+            action.columns if action.columns else {}
+        )
         if not column_data:
             result.message = "There is not column index"
             return result
 
         cell_default_values: Dict[int, str] = (
             action.cell_default_values if action.cell_default_values else {}
         )
@@ -42,20 +44,23 @@
                 header_line = source.readline()
                 header_names = header_line.strip().split("\t")
                 for column_idx in column_indices:
                     if column_idx < 0:
                         column_idx = len(header_names)
                     default_value = (
                         cell_default_values[column_idx]
-                        if column_idx in cell_default_values and cell_default_values[column_idx]
+                        if column_idx in cell_default_values
+                        and cell_default_values[column_idx]
                         else ""
                     )
                     value: actions.TsvColumnData = column_data[column_idx]
                     if not value or not value.header_name:
-                        result.message = f"There is not header name for column index {column_idx}"
+                        result.message = (
+                            f"There is not header name for column index {column_idx}"
+                        )
                         return result
                     header_names.insert(column_idx, value.header_name)
 
                 with open(target_file_path, "w") as target:
                     self.write_row(target, header_names)
                     row_index = 0
                     for line in source:
@@ -63,15 +68,17 @@
                         for column_idx in column_indices:
                             default_value = (
                                 cell_default_values[column_idx]
                                 if column_idx in cell_default_values
                                 and cell_default_values[column_idx]
                                 else ""
                             )
-                            coloumn_data: actions.TsvColumnData = column_data[column_idx]
+                            coloumn_data: actions.TsvColumnData = column_data[
+                                column_idx
+                            ]
                             value = (
                                 coloumn_data.values[row_index]
                                 if row_index in coloumn_data.values
                                 else default_value
                             )
                             row.insert(column_idx, value)
                         self.write_row(target, row)
```

### Comparing `metabolights_utils-0.9.2/metabolights_utils/tsv/actions/add_row.py` & `metabolights_utils-0.9.3/metabolights_utils/tsv/actions/add_row.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,15 +21,17 @@
         action: model.TsvAddRowsAction = action
         target_row_indices: List[int] = action.new_row_indices
 
         if not target_row_indices:
             result.message = "There is not row index"
             return result
 
-        row_data: Dict[int, model.TsvRowData] = action.row_data if action.row_data else {}
+        row_data: Dict[int, model.TsvRowData] = (
+            action.row_data if action.row_data else {}
+        )
 
         row_indices = target_row_indices.copy()
         row_indices.sort()
 
         if action.id:
             uuid_value = str(uuid.uuid4().hex)
             action.id = uuid_value
@@ -43,37 +45,45 @@
                 with open(target_file_path, "w") as target:
                     self.write_row(target, header_names)
                     row_index = -1
                     for line in source:
                         row_index += 1
                         if row_index in row_indices:
                             while row_index in row_indices:
-                                input_row = row_data[row_index] if row_index in row_data else None
+                                input_row = (
+                                    row_data[row_index]
+                                    if row_index in row_data
+                                    else None
+                                )
                                 if not input_row:
                                     self.write_row(target, empty_row)
                                 else:
                                     new_row = self.get_updated_row(empty_row, input_row)
                                     self.write_row(target, new_row)
                                 row_indices.remove(row_index)
                                 row_index += 1
                         target.write(line)
 
                     if len(row_indices):
                         row_index += 1
                         while row_index in row_indices:
-                            input_row = row_data[row_index] if row_index in row_data else None
+                            input_row = (
+                                row_data[row_index] if row_index in row_data else None
+                            )
                             if not input_row:
                                 self.write_row(target, empty_row)
                             else:
                                 new_row = self.get_updated_row(empty_row, input_row)
                                 self.write_row(target, new_row)
                             row_indices.remove(row_index)
                             row_index += 1
 
                         if len(row_indices):
-                            result.message = f"Invalid row indices {', '.join(row_indices)}"
+                            result.message = (
+                                f"Invalid row indices {', '.join(row_indices)}"
+                            )
                             return result
             result.success = True
         except Exception as exc:
             result.message = f"{str(exc)}"
 
         return result
```

### Comparing `metabolights_utils-0.9.2/metabolights_utils/tsv/actions/base.py` & `metabolights_utils-0.9.3/metabolights_utils/tsv/actions/base.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.2/metabolights_utils/tsv/actions/copy_column.py` & `metabolights_utils-0.9.3/metabolights_utils/tsv/actions/copy_column.py`

 * *Files 7% similar despite different names*

```diff
@@ -55,26 +55,27 @@
                     return result
                 invalid_targets = []
                 for column_idx in columns:
                     if column_idx >= len(header_names) and column_idx < 0:
                         invalid_targets.append(column_idx)
 
                 if invalid_targets:
-                    result.message = (
-                        f"Target column indices are not valid: {', '.join(invalid_targets)}."
-                    )
+                    result.message = f"Target column indices are not valid: {', '.join(invalid_targets)}."
                     return result
 
                 with open(target_file_path, "w") as target:
                     self.write_row(target, header_names)
                     row_index = 0
                     for line in source:
                         row = line.strip().split("\t")
                         for column_idx in columns:
-                            if not selected_row_indices or row_index in selected_row_indices:
+                            if (
+                                not selected_row_indices
+                                or row_index in selected_row_indices
+                            ):
                                 row[column_idx] = row[source_column_index]
 
                         self.write_row(target, row)
                         row_index += 1
 
             result.success = True
         except Exception as exc:
```

### Comparing `metabolights_utils-0.9.2/metabolights_utils/tsv/actions/copy_row.py` & `metabolights_utils-0.9.3/metabolights_utils/tsv/actions/copy_row.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,14 +70,16 @@
                                     self.write_row(target, new_row)
                             row_indices.remove(row_index)
                         else:
                             target.write(line)
                         row_index += 1
 
                     if len(row_indices):
-                        result.message = f"Invalid target row indices {', '.join(row_indices)}"
+                        result.message = (
+                            f"Invalid target row indices {', '.join(row_indices)}"
+                        )
                         return result
             result.success = True
         except Exception as exc:
             result.message = f"{str(exc)}"
 
         return result
```

### Comparing `metabolights_utils-0.9.2/metabolights_utils/tsv/actions/delete_column.py` & `metabolights_utils-0.9.3/metabolights_utils/tsv/actions/delete_column.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,17 @@
         result: actions.TsvActionResult = actions.TsvActionResult(action=action)
         if action.name != actions.TsvActionName.DELETE_COLUMN:
             result.message = "Action name is not valid"
             return result
 
         action: actions.TsvDeleteColumnsAction = action
 
-        columns: Dict[int, str] = action.current_columns if action.current_columns else {}
+        columns: Dict[int, str] = (
+            action.current_columns if action.current_columns else {}
+        )
         if not columns:
             result.message = "There is not column index"
             return result
 
         column_indices: List[int] = list(columns.keys()).copy()
         column_indices.sort()
 
@@ -48,15 +50,17 @@
                     new_header_names.append(value)
 
                 with open(target_file_path, "w") as target:
                     self.write_row(target, new_header_names)
                     for line in source:
                         new_row = []
                         row = line.strip().split("\t")
-                        new_row = [x[1] for x in enumerate(row) if x[0] not in column_indices]
+                        new_row = [
+                            x[1] for x in enumerate(row) if x[0] not in column_indices
+                        ]
                         new_row.append(value)
                         self.write_row(target, new_row)
             result.success = True
         except Exception as exc:
             result.message = f"{str(exc)}"
 
         return result
```

### Comparing `metabolights_utils-0.9.2/metabolights_utils/tsv/actions/delete_row.py` & `metabolights_utils-0.9.3/metabolights_utils/tsv/actions/delete_row.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.2/metabolights_utils/tsv/actions/move_column.py` & `metabolights_utils-0.9.3/metabolights_utils/tsv/actions/move_column.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,18 +28,22 @@
 
         try:
             with open(source_file_path, "r") as source:
                 header_line = source.readline()
                 header_names = header_line.strip().split("\t")
                 new_header_names = []
                 if source_column_index < 0 or source_column_index >= len(header_names):
-                    result.message = f"Source column index is not in range. {source_column_index}"
+                    result.message = (
+                        f"Source column index is not in range. {source_column_index}"
+                    )
                     return result
                 if new_column_index < 0 or new_column_index >= len(header_names):
-                    result.message = f"New column index is not in range. {new_column_index}"
+                    result.message = (
+                        f"New column index is not in range. {new_column_index}"
+                    )
                     return result
 
                 moved_header = header_names[source_column_index]
                 if moved_header != source_column_header:
                     result.message = (
                         f"Input header name does not math the actual one for the index {source_column_index}."
                         + f"Expected: {source_column_header}, found: {moved_header}"
```

### Comparing `metabolights_utils-0.9.2/metabolights_utils/tsv/actions/move_row.py` & `metabolights_utils-0.9.3/metabolights_utils/tsv/actions/move_row.py`

 * *Files identical despite different names*

### Comparing `metabolights_utils-0.9.2/metabolights_utils/tsv/actions/update_cell.py` & `metabolights_utils-0.9.3/metabolights_utils/tsv/actions/update_cell.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,17 @@
             with open(source_file_path, "r") as source:
                 header_line = source.readline()
                 header_names = header_line.strip().split("\t")
                 invalid_column_indices = [
                     x for x in column_indices if x < 0 or x > len(header_names)
                 ]
                 if invalid_column_indices:
-                    result.message = f"Invalid column indices: {', '.join(invalid_column_indices)}"
+                    result.message = (
+                        f"Invalid column indices: {', '.join(invalid_column_indices)}"
+                    )
                     return result
 
                 with open(target_file_path, "w") as target:
                     self.write_row(target, header_names)
                     row_index = 0
                     for line in source:
                         row = line.strip().split("\t")
@@ -66,14 +68,16 @@
                                 row[column_idx] = row_data_item.values[column_idx]
                             if row_index in row_indices:
                                 row_indices.remove(row_index)
 
                         self.write_row(target, row)
                         row_index += 1
                     if row_indices:
-                        result.message = f"Invalid row indices: {', '.join(row_indices)}"
+                        result.message = (
+                            f"Invalid row indices: {', '.join(row_indices)}"
+                        )
                         return result
             result.success = True
         except Exception as exc:
             result.message = f"{str(exc)}"
 
         return result
```

### Comparing `metabolights_utils-0.9.2/metabolights_utils/tsv/actions/update_column.py` & `metabolights_utils-0.9.3/metabolights_utils/tsv/actions/update_column.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,17 @@
         result: actions.TsvActionResult = actions.TsvActionResult(action=action)
         if action.name != actions.TsvActionName.UPDATE_COLUMN_DATA:
             result.message = "Action name is not valid"
             return result
 
         action: actions.TsvUpdateColumnsAction = action
 
-        columns: Dict[int, actions.TsvColumnData] = action.columns if action.columns else {}
+        columns: Dict[int, actions.TsvColumnData] = (
+            action.columns if action.columns else {}
+        )
 
         if not columns:
             result.message = "There is not target column index"
             return result
 
         column_indices: List[int] = list(columns.keys()).copy()
         column_indices.sort()
@@ -46,35 +48,41 @@
                                 f"Input header name does not math the actual one for index {column_idx}."
                                 + f"Expected: {columns[column_idx].header_name}, found: {value}"
                             )
                             return result
                         selected_columns.append(column_idx)
 
                 if len(selected_columns) != len(column_indices):
-                    invalid_indices = [x for x in column_indices if x not in selected_columns]
+                    invalid_indices = [
+                        x for x in column_indices if x not in selected_columns
+                    ]
                     result.message = (
-                        f"Some column indices are not found :" + f"{', '.join(invalid_indices)}"
+                        f"Some column indices are not found :"
+                        + f"{', '.join(invalid_indices)}"
                     )
                     return result
 
-                invalid_targets = [x for x in columns if x >= len(header_names) and x < 0]
+                invalid_targets = [
+                    x for x in columns if x >= len(header_names) and x < 0
+                ]
                 if invalid_targets:
-                    result.message = (
-                        f"Target column indices are not valid: {', '.join(invalid_targets)}."
-                    )
+                    result.message = f"Target column indices are not valid: {', '.join(invalid_targets)}."
                     return result
 
                 with open(target_file_path, "w") as target:
                     self.write_row(target, header_names)
                     row_index = 0
                     for line in source:
                         row = line.strip().split("\t")
                         for column_idx, value in columns.items():
                             column_data: actions.TsvColumnData = value
-                            if not column_data.values or row_index in column_data.values:
+                            if (
+                                not column_data.values
+                                or row_index in column_data.values
+                            ):
                                 row[column_idx] = column_data.values[row_index]
 
                         self.write_row(target, row)
                         row_index += 1
 
             result.success = True
         except Exception as exc:
```

### Comparing `metabolights_utils-0.9.2/metabolights_utils/tsv/actions/update_column_header.py` & `metabolights_utils-0.9.3/metabolights_utils/tsv/actions/update_column_header.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,17 @@
                 header_line = source.readline()
                 header_names = header_line.strip().split("\t")
                 column_count = len(header_names)
                 for column_idx in column_indices:
                     if column_idx < column_count and headers[column_idx]:
                         header_names[column_idx] = headers[column_idx]
                     else:
-                        headers[column_idx] = headers[column_idx] if headers[column_idx] else ""
+                        headers[column_idx] = (
+                            headers[column_idx] if headers[column_idx] else ""
+                        )
                         result.message = f"Invalid column index {column_idx} with column name '{headers[column_idx]}'"
                         return result
                 with open(target_file_path, "w") as target:
                     self.write_row(target, header_names)
                     for line in source:
                         target.write(line)
             result.success = True
```

### Comparing `metabolights_utils-0.9.2/metabolights_utils/tsv/actions/update_row.py` & `metabolights_utils-0.9.3/metabolights_utils/tsv/actions/update_row.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,16 +48,14 @@
                             new_row = self.get_updated_row(empty_row, input_row)
                             self.write_row(target, new_row)
                             row_indices.remove(row_index)
                         else:
                             target.write(line)
 
                     if len(row_indices):
-                        result.message = (
-                            f"Invalid row indices {', '.join([str(x) for x in row_indices])}"
-                        )
+                        result.message = f"Invalid row indices {', '.join([str(x) for x in row_indices])}"
                         return result
             result.success = True
         except Exception as exc:
             result.message = f"{str(exc)}"
 
         return result
```

### Comparing `metabolights_utils-0.9.2/metabolights_utils/tsv/model.py` & `metabolights_utils-0.9.3/metabolights_utils/tsv/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,15 +57,17 @@
 class TsvDeleteRowsAction(TsvAction):
     name: str = TsvActionName.DELETE_ROW
     current_row_indices: List[int] = []
 
 
 class TsvDeleteColumnsAction(TsvAction):
     name: str = TsvActionName.DELETE_COLUMN
-    current_columns: Dict[int, str] = Field({}, description="Current column indices and headers.")
+    current_columns: Dict[int, str] = Field(
+        {}, description="Current column indices and headers."
+    )
 
 
 class TsvMoveRowAction(TsvAction):
     name: str = TsvActionName.MOVE_ROW
     source_row_index: int = -1
     new_row_index: int = -1
 
@@ -85,16 +87,20 @@
         [], description="Column indices. If it is None or empty, Copy all columns"
     )
 
 
 class TsvCopyColumnAction(TsvAction):
     name: str = TsvActionName.COPY_COLUMN
     source_column_index: int = Field(-1, description="Source colum index")
-    source_column_header: Union[None, str] = Field("", description="Source colum header to verify.")
-    target_columns: Dict[int, str] = Field({}, description="target colum indices and headers.")
+    source_column_header: Union[None, str] = Field(
+        "", description="Source colum header to verify."
+    )
+    target_columns: Dict[int, str] = Field(
+        {}, description="target colum indices and headers."
+    )
     selected_row_indices: List[int] = Field(
         [], description="Row indices. If it is None or empty, Copy all rows"
     )
 
 
 class TsvUpdateRowsAction(TsvAction):
     name: str = TsvActionName.UPDATE_ROW_DATA
```

### Comparing `metabolights_utils-0.9.2/metabolights_utils/tsv/tsv_file_updater.py` & `metabolights_utils-0.9.3/metabolights_utils/tsv/tsv_file_updater.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,30 +13,39 @@
 from metabolights_utils.tsv.actions.copy_row import CopyRowActionHelper
 from metabolights_utils.tsv.actions.delete_column import DeleteColumnsActionHelper
 from metabolights_utils.tsv.actions.delete_row import DeleteRowsActionHelper
 from metabolights_utils.tsv.actions.move_column import MoveColumnActionHelper
 from metabolights_utils.tsv.actions.move_row import MoveRowActionHelper
 from metabolights_utils.tsv.actions.update_cell import UpdateCellsActionHelper
 from metabolights_utils.tsv.actions.update_column import UpdateColumnsActionHelper
-from metabolights_utils.tsv.actions.update_column_header import UpdateColumnHeadersActionHelper
+from metabolights_utils.tsv.actions.update_column_header import (
+    UpdateColumnHeadersActionHelper,
+)
 from metabolights_utils.tsv.actions.update_row import UpdateRowsActionHelper
-from metabolights_utils.tsv.model import TsvAction, TsvActionName, TsvActionReport, TsvActionResult
+from metabolights_utils.tsv.model import (
+    TsvAction,
+    TsvActionName,
+    TsvActionReport,
+    TsvActionResult,
+)
 
 ISA_TABLE_ACTION_HELPERS: Dict[TsvActionName, BaseActionHelper] = {}
 ISA_TABLE_ACTION_HELPERS[TsvActionName.ADD_ROW] = AddRowsActionHelper()
 ISA_TABLE_ACTION_HELPERS[TsvActionName.DELETE_ROW] = DeleteRowsActionHelper()
 ISA_TABLE_ACTION_HELPERS[TsvActionName.UPDATE_ROW_DATA] = UpdateRowsActionHelper()
 ISA_TABLE_ACTION_HELPERS[TsvActionName.COPY_ROW] = CopyRowActionHelper()
 ISA_TABLE_ACTION_HELPERS[TsvActionName.MOVE_ROW] = MoveRowActionHelper()
 ISA_TABLE_ACTION_HELPERS[TsvActionName.ADD_COLUMN] = AddColumnsActionHelper()
 ISA_TABLE_ACTION_HELPERS[TsvActionName.DELETE_COLUMN] = DeleteColumnsActionHelper()
 ISA_TABLE_ACTION_HELPERS[TsvActionName.COPY_COLUMN] = CopyColumnActionHelper()
 ISA_TABLE_ACTION_HELPERS[TsvActionName.UPDATE_COLUMN_DATA] = UpdateColumnsActionHelper()
 ISA_TABLE_ACTION_HELPERS[TsvActionName.MOVE_COLUMN] = MoveColumnActionHelper()
-ISA_TABLE_ACTION_HELPERS[TsvActionName.UPDATE_COLUMN_HEADER] = UpdateColumnHeadersActionHelper()
+ISA_TABLE_ACTION_HELPERS[
+    TsvActionName.UPDATE_COLUMN_HEADER
+] = UpdateColumnHeadersActionHelper()
 ISA_TABLE_ACTION_HELPERS[TsvActionName.UPDATE_CELL_DATA] = UpdateCellsActionHelper()
 
 
 class TsvFileUpdater:
     def apply_actions(
         self,
         file_path: Union[str, pathlib.Path],
@@ -60,43 +69,51 @@
 
         if isinstance(file_path, pathlib.Path):
             file = file_path
         else:
             file = pathlib.Path(file_path)
 
         if not file.exists() or not file.is_file():
-            report.message = f"File '{str(file)}' does not exist or it is not a regular file."
+            report.message = (
+                f"File '{str(file)}' does not exist or it is not a regular file."
+            )
             return report
         sha256 = self.calculate_sha256(file)
 
         if sha256 != file_sha256_hash:
             report.message = f"SH256 of '{str(file)}' does not match the input value."
             return report
 
         task_id = str(uuid.uuid4().hex)
         timestamp = str(int(datetime.datetime.now().timestamp()))
         temp_folder = pathlib.Path(f"/tmp/isa_table_actions/{timestamp}/{task_id}")
         os.makedirs(str(temp_folder))
 
         file_copy_path = temp_folder / pathlib.Path(f"{file.name}_{task_id}")
-        temp_source_file_path = temp_folder / pathlib.Path(f".{file.name}_{task_id}_temp_1")
-        temp_target_file_path = temp_folder / pathlib.Path(f".{file.name}_{task_id}_temp_2")
+        temp_source_file_path = temp_folder / pathlib.Path(
+            f".{file.name}_{task_id}_temp_1"
+        )
+        temp_target_file_path = temp_folder / pathlib.Path(
+            f".{file.name}_{task_id}_temp_2"
+        )
 
         source_path = file_copy_path
         target_path = temp_target_file_path
         last_file = None
         try:
             for action in actions:
                 if action.name not in ISA_TABLE_ACTION_HELPERS:
                     report.message = f"Upsupported action: action.name."
                     return report
             shutil.move(file, file_copy_path)
             for action in actions:
                 helper = ISA_TABLE_ACTION_HELPERS[action.name]
-                result: TsvActionResult = helper.apply_action(source_path, target_path, action)
+                result: TsvActionResult = helper.apply_action(
+                    source_path, target_path, action
+                )
                 last_file = target_path
                 source_path = last_file
                 target_path = (
                     temp_target_file_path
                     if source_path == temp_source_file_path
                     else temp_source_file_path
                 )
```

### Comparing `metabolights_utils-0.9.2/pyproject.toml` & `metabolights_utils-0.9.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "metabolights-utils"
-version = "0.9.2"
+version = "0.9.3"
 description = "Metabolights common models, utility methods and classes for python-based Metabolights projects."
 authors = ["Ozgur Yurekten <ozgur@ebi.ac.uk>"]
 readme = "README.md"
 packages = [{include = "metabolights_utils"}]
 license = "Apache-2.0"
 homepage = "https://github.com/EBI-Metabolights"
 repository = "https://github.com/EBI-Metabolights/metabolights-utils"
```

