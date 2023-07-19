# Comparing `tmp/TravSHACL-1.4.1.tar.gz` & `tmp/TravSHACL-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TravSHACL-1.4.1.tar", last modified: Tue Jul 18 12:29:38 2023, max compression
+gzip compressed data, was "TravSHACL-1.4.2.tar", last modified: Wed Jul 19 09:55:25 2023, max compression
```

## Comparing `TravSHACL-1.4.1.tar` & `TravSHACL-1.4.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:29:38.109178 TravSHACL-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35150 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9124 2023-07-18 12:29:38.109178 TravSHACL-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:29:38.093178 TravSHACL-1.4.1/TravSHACL/
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/TravSHACL/TravSHACL.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/TravSHACL/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:29:38.101178 TravSHACL-1.4.1/TravSHACL/constraints/
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/TravSHACL/constraints/Constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/TravSHACL/constraints/MaxOnlyConstraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/TravSHACL/constraints/MinMaxConstraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/TravSHACL/constraints/MinOnlyConstraint.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/TravSHACL/constraints/SPARQLConstraint.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/TravSHACL/constraints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:29:38.105178 TravSHACL-1.4.1/TravSHACL/core/
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/TravSHACL/core/GraphTraversal.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/TravSHACL/core/RulePattern.py
--rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/TravSHACL/core/Shape.py
--rw-r--r--   0 runner    (1001) docker     (123)    24062 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/TravSHACL/core/ShapeParser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/TravSHACL/core/ShapeSchema.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/TravSHACL/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:29:38.105178 TravSHACL-1.4.1/TravSHACL/rule_based_validation/
--rw-r--r--   0 runner    (1001) docker     (123)    13580 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/TravSHACL/rule_based_validation/InstancesRetrieval.py
--rw-r--r--   0 runner    (1001) docker     (123)    34527 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/TravSHACL/rule_based_validation/Validation.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/TravSHACL/rule_based_validation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:29:38.109178 TravSHACL-1.4.1/TravSHACL/sparql/
--rw-r--r--   0 runner    (1001) docker     (123)    27726 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/TravSHACL/sparql/QueryGenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/TravSHACL/sparql/SPARQLEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/TravSHACL/sparql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:29:38.109178 TravSHACL-1.4.1/TravSHACL/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/TravSHACL/utils/ValidationStats.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/TravSHACL/utils/VariableGenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/TravSHACL/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/TravSHACL/utils/fileManagement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:29:38.097178 TravSHACL-1.4.1/TravSHACL.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9124 2023-07-18 12:29:38.000000 TravSHACL-1.4.1/TravSHACL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-18 12:29:38.000000 TravSHACL-1.4.1/TravSHACL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 12:29:38.000000 TravSHACL-1.4.1/TravSHACL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-18 12:29:38.000000 TravSHACL-1.4.1/TravSHACL.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-18 12:29:38.000000 TravSHACL-1.4.1/TravSHACL.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-18 12:29:38.113178 TravSHACL-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:29:38.109178 TravSHACL-1.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-07-18 12:29:20.000000 TravSHACL-1.4.1/tests/test_cases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:55:25.774923 TravSHACL-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35150 2023-07-19 09:55:12.000000 TravSHACL-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-19 09:55:12.000000 TravSHACL-1.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9124 2023-07-19 09:55:25.774923 TravSHACL-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-07-19 09:55:12.000000 TravSHACL-1.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:55:25.770923 TravSHACL-1.4.2/TravSHACL/
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-19 09:55:12.000000 TravSHACL-1.4.2/TravSHACL/TravSHACL.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-19 09:55:12.000000 TravSHACL-1.4.2/TravSHACL/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:55:25.770923 TravSHACL-1.4.2/TravSHACL/constraints/
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-07-19 09:55:12.000000 TravSHACL-1.4.2/TravSHACL/constraints/Constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-19 09:55:12.000000 TravSHACL-1.4.2/TravSHACL/constraints/MaxOnlyConstraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-19 09:55:12.000000 TravSHACL-1.4.2/TravSHACL/constraints/MinMaxConstraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-19 09:55:12.000000 TravSHACL-1.4.2/TravSHACL/constraints/MinOnlyConstraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-19 09:55:12.000000 TravSHACL-1.4.2/TravSHACL/constraints/SPARQLConstraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 09:55:12.000000 TravSHACL-1.4.2/TravSHACL/constraints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:55:25.770923 TravSHACL-1.4.2/TravSHACL/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-07-19 09:55:12.000000 TravSHACL-1.4.2/TravSHACL/core/GraphTraversal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-19 09:55:12.000000 TravSHACL-1.4.2/TravSHACL/core/RulePattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-07-19 09:55:12.000000 TravSHACL-1.4.2/TravSHACL/core/Shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23827 2023-07-19 09:55:12.000000 TravSHACL-1.4.2/TravSHACL/core/ShapeParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-07-19 09:55:12.000000 TravSHACL-1.4.2/TravSHACL/core/ShapeSchema.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 09:55:12.000000 TravSHACL-1.4.2/TravSHACL/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:55:25.770923 TravSHACL-1.4.2/TravSHACL/rule_based_validation/
+-rw-r--r--   0 runner    (1001) docker     (123)    13580 2023-07-19 09:55:12.000000 TravSHACL-1.4.2/TravSHACL/rule_based_validation/InstancesRetrieval.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34527 2023-07-19 09:55:12.000000 TravSHACL-1.4.2/TravSHACL/rule_based_validation/Validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 09:55:12.000000 TravSHACL-1.4.2/TravSHACL/rule_based_validation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:55:25.774923 TravSHACL-1.4.2/TravSHACL/sparql/
+-rw-r--r--   0 runner    (1001) docker     (123)    27370 2023-07-19 09:55:12.000000 TravSHACL-1.4.2/TravSHACL/sparql/QueryGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-07-19 09:55:12.000000 TravSHACL-1.4.2/TravSHACL/sparql/SPARQLEndpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 09:55:12.000000 TravSHACL-1.4.2/TravSHACL/sparql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:55:25.774923 TravSHACL-1.4.2/TravSHACL/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-07-19 09:55:12.000000 TravSHACL-1.4.2/TravSHACL/utils/ValidationStats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-19 09:55:12.000000 TravSHACL-1.4.2/TravSHACL/utils/VariableGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 09:55:12.000000 TravSHACL-1.4.2/TravSHACL/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-19 09:55:12.000000 TravSHACL-1.4.2/TravSHACL/utils/fileManagement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:55:25.770923 TravSHACL-1.4.2/TravSHACL.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9124 2023-07-19 09:55:25.000000 TravSHACL-1.4.2/TravSHACL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-19 09:55:25.000000 TravSHACL-1.4.2/TravSHACL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 09:55:25.000000 TravSHACL-1.4.2/TravSHACL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-19 09:55:25.000000 TravSHACL-1.4.2/TravSHACL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-19 09:55:25.000000 TravSHACL-1.4.2/TravSHACL.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-19 09:55:12.000000 TravSHACL-1.4.2/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-19 09:55:25.774923 TravSHACL-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-07-19 09:55:12.000000 TravSHACL-1.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:55:25.774923 TravSHACL-1.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-07-19 09:55:12.000000 TravSHACL-1.4.2/tests/test_cases.py
```

### Comparing `TravSHACL-1.4.1/LICENSE` & `TravSHACL-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.4.1/PKG-INFO` & `TravSHACL-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: TravSHACL
-Version: 1.4.1
+Version: 1.4.2
 Summary: A SHACL validator capable of planning the traversal and execution of the validation of a shape schema to detect violations early.
 Home-page: https://github.com/SDM-TIB/Trav-SHACL
-Download-URL: https://github.com/SDM-TIB/Trav-SHACL/archive/refs/tags/v1.4.1.tar.gz
+Download-URL: https://github.com/SDM-TIB/Trav-SHACL/archive/refs/tags/v1.4.2.tar.gz
 Author: Mónica Figuera, Philipp D. Rohde
 Author-email: philipp.rohde@tib.eu
 License: GNU/GPLv3
 Classifier: Development Status :: 5 - Production/Stable 
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `TravSHACL-1.4.1/README.md` & `TravSHACL-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.4.1/TravSHACL/TravSHACL.py` & `TravSHACL-1.4.2/TravSHACL/TravSHACL.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.4.1/TravSHACL/constraints/Constraint.py` & `TravSHACL-1.4.2/TravSHACL/constraints/Constraint.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,34 +2,32 @@
 __author__ = 'Monica Figuera and Philipp D. Rohde'
 
 
 class Constraint:
     """Base class for all constraints."""
 
     def __init__(self, id_=None, is_pos=None, satisfied=None, datatype=None, value=None,
-                 shape_ref=None, target_def=None, path=None, options=None, raw_or=None):
+                 shape_ref=None, target_def=None, path=None, options=None):
         """
         Base constructor for all constraints.
 
         :param id_: name of the constraint
         :param is_pos: true if it is a positive constraint, false otherwise
         :param satisfied: indicates whether the constraint is satisfied, should be unknown at creation
         :param datatype: contains the datatype the object must fulfill
         :param value: contains the value the constraint checks again, i.e., an object
         :param shape_ref: contains the name of the shape referenced by the constraint, none otherwise
         :param target_def: contains the target definition of the shape the constraint belongs to if it has one
         :param path: the path associated with this constraint, e.g., a predicate
         :param options: gets the options to be used in or_operation
-        :param raw_or: contains the specific constraints for or in the shapes graph
         """
         self.id = id_
         self.isPos = is_pos
         self.satisfied = satisfied
         self.options = options
-        self.raw_or = raw_or
         self.datatype = datatype
         self.value = value
         self.shapeRef = shape_ref
         self.target = target_def
 
         self.variables = []
         self.path = path
```

### Comparing `TravSHACL-1.4.1/TravSHACL/constraints/MaxOnlyConstraint.py` & `TravSHACL-1.4.2/TravSHACL/constraints/MaxOnlyConstraint.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,29 +4,29 @@
 from TravSHACL.utils.VariableGenerator import VariableType
 from TravSHACL.constraints.Constraint import Constraint
 
 
 class MaxOnlyConstraint(Constraint):
     """This class represents max constraints, i.e., a constraint for the maximal occurrence of a path."""
 
-    def __init__(self, var_generator, id_, path, max_, is_pos, options, raw_or, datatype=None, value=None, shape_ref=None, target_def=None):
+    def __init__(self, var_generator, id_, path, max_, is_pos, options, datatype=None, value=None, shape_ref=None, target_def=None):
         """
         Creates a new max constraint.
 
         :param var_generator: variable generator instance
         :param id_: name of the constraint
         :param path: the path associated with this constraint, e.g., a predicate
         :param max_: the maximal occurrence allowed
         :param is_pos: true if it is a positive constraint, false otherwise
         :param datatype: contains the datatype the object must fulfill
         :param value: contains the value the constraint checks again, i.e., an object
         :param shape_ref: contains the name of the shape referenced by the constraint, none otherwise
         :param target_def: contains the target definition of the shape the constraint belongs to if it has one
         """
-        super().__init__(id_, is_pos, None, datatype, value, shape_ref, target_def, path, options, raw_or)
+        super().__init__(id_, is_pos, None, datatype, value, shape_ref, target_def, path, options)
         self.varGenerator = var_generator
         self.min = -1
         self.max = max_
         self.variables = self.compute_variables()
 
     def compute_variables(self):
         """Computes variable names for the SPARQL queries of the constraint."""
```

### Comparing `TravSHACL-1.4.1/TravSHACL/constraints/MinMaxConstraint.py` & `TravSHACL-1.4.2/TravSHACL/constraints/MinOnlyConstraint.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 # -*- coding: utf-8 -*-
-__author__ = 'Philipp D. Rohde'
+__author__ = 'Monica Figuera and Philipp D. Rohde'
 
 from TravSHACL.utils.VariableGenerator import VariableType
 from TravSHACL.constraints.Constraint import Constraint
 
 
-class MinMaxConstraint(Constraint):
-    """
-    This class represents min-max constraints, i.e., a constraint for the minimal and maximal occurrence of a path.
-    """
+class MinOnlyConstraint(Constraint):
+    """This class represents min constraints, i.e., a constraint for the minimal occurrence of a path."""
 
-    def __init__(self, var_generator, id_, path, min_, max_, is_pos, datatype=None, value=None, shape_ref=None, target_def=None):
+    def __init__(self, var_generator, id_, path, min_, is_pos, options, datatype=None, value=None, shape_ref=None, target_def=None):
         """
-        Creates a new min-max constraint.
+        Creates a new min constraint.
 
         :param var_generator: variable generator instance
         :param id_: name of the constraint
         :param path: the path associated with this constraint, e.g., a predicate
         :param min_: the minimal occurrence allowed
-        :param max_: the maximal occurrence allowed
         :param is_pos: true if it is a positive constraint, false otherwise
         :param datatype: contains the datatype the object must fulfill
         :param value: contains the value the constraint checks again, i.e., an object
         :param shape_ref: contains the name of the shape referenced by the constraint, none otherwise
         :param target_def: contains the target definition of the shape the constraint belongs to if it has one
         """
-        super().__init__(id_, is_pos, None, datatype, value, shape_ref, target_def, path)
+        super().__init__(id_, is_pos, None, datatype, value, shape_ref, target_def, path, options)
         self.varGenerator = var_generator
         self.min = min_
-        self.max = max_
+        self.max = -1
         self.variables = self.compute_variables()
 
     def compute_variables(self):
         """Computes variable names for the SPARQL queries of the constraint."""
         atomic_constraint = Constraint()
         return atomic_constraint.generate_variables(self.varGenerator, VariableType.VALIDATION, self.min)
```

### Comparing `TravSHACL-1.4.1/TravSHACL/constraints/MinOnlyConstraint.py` & `TravSHACL-1.4.2/TravSHACL/constraints/MinMaxConstraint.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 # -*- coding: utf-8 -*-
-__author__ = 'Monica Figuera and Philipp D. Rohde'
+__author__ = 'Philipp D. Rohde'
 
 from TravSHACL.utils.VariableGenerator import VariableType
 from TravSHACL.constraints.Constraint import Constraint
 
 
-class MinOnlyConstraint(Constraint):
-    """This class represents min constraints, i.e., a constraint for the minimal occurrence of a path."""
+class MinMaxConstraint(Constraint):
+    """
+    This class represents min-max constraints, i.e., a constraint for the minimal and maximal occurrence of a path.
+    """
 
-    def __init__(self, var_generator, id_, path, min_, is_pos, options, raw_or, datatype=None, value=None, shape_ref=None, target_def=None):
+    def __init__(self, var_generator, id_, path, min_, max_, is_pos, datatype=None, value=None, shape_ref=None, target_def=None):
         """
-        Creates a new min constraint.
+        Creates a new min-max constraint.
 
         :param var_generator: variable generator instance
         :param id_: name of the constraint
         :param path: the path associated with this constraint, e.g., a predicate
         :param min_: the minimal occurrence allowed
+        :param max_: the maximal occurrence allowed
         :param is_pos: true if it is a positive constraint, false otherwise
         :param datatype: contains the datatype the object must fulfill
         :param value: contains the value the constraint checks again, i.e., an object
         :param shape_ref: contains the name of the shape referenced by the constraint, none otherwise
         :param target_def: contains the target definition of the shape the constraint belongs to if it has one
         """
-        super().__init__(id_, is_pos, None, datatype, value, shape_ref, target_def, path, options, raw_or)
+        super().__init__(id_, is_pos, None, datatype, value, shape_ref, target_def, path, None)
         self.varGenerator = var_generator
         self.min = min_
-        self.max = -1
+        self.max = max_
         self.variables = self.compute_variables()
 
     def compute_variables(self):
         """Computes variable names for the SPARQL queries of the constraint."""
         atomic_constraint = Constraint()
         return atomic_constraint.generate_variables(self.varGenerator, VariableType.VALIDATION, self.min)
```

### Comparing `TravSHACL-1.4.1/TravSHACL/constraints/SPARQLConstraint.py` & `TravSHACL-1.4.2/TravSHACL/constraints/SPARQLConstraint.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,11 +10,11 @@
     def __init__(self, id_, is_pos, query: str = None):
         """
         Creates a new SPARQL constraint.
 
         :param id_: name of the constraint
         :param query: a string representing the SPARQL query to be executed for the constraint evaluation
         """
-        super().__init__(id_, is_pos, None, None, None, None, None, None)
+        super().__init__(id_, is_pos, None, None, None, None, None, None, None)
         self.min = -1
         self.max = -1
         self.query = query
```

### Comparing `TravSHACL-1.4.1/TravSHACL/core/GraphTraversal.py` & `TravSHACL-1.4.2/TravSHACL/core/GraphTraversal.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.4.1/TravSHACL/core/RulePattern.py` & `TravSHACL-1.4.2/TravSHACL/core/RulePattern.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.4.1/TravSHACL/core/Shape.py` & `TravSHACL-1.4.2/TravSHACL/core/Shape.py`

 * *Files 2% similar despite different names*

```diff
@@ -225,10 +225,13 @@
         return self.maxValidRefs
 
     def get_prefix_string(self):
         return '\n'.join([''.join('PREFIX ' + key + ': ' + value) for (key, value) in self.prefixes.items()]) + '\n'
 
     def get_or_query(self):
         if True in self.flag:
-            return self.QueryGenerator.options_query(self.constraints, self.targetQuery, self.includePrefixes,
-                                                     self.ORDERBYinQueries)
+            or_constraints = [c for c in self.constraints if c.options]
+            if len(or_constraints) == 0:
+                return
+            else:
+                return self.QueryGenerator.options_query(or_constraints, self.targetQuery, self.includePrefixes, self.ORDERBYinQueries)
         return
```

### Comparing `TravSHACL-1.4.1/TravSHACL/core/ShapeParser.py` & `TravSHACL-1.4.2/TravSHACL/core/ShapeParser.py`

 * *Files 2% similar despite different names*

```diff
@@ -446,36 +446,33 @@
         """
         var_generator = VariableGenerator()
         constraints = []
 
         for i, constraint in enumerate(array):
             if constraint.get('flag'):
                 or_constraints = []
-                raw_or = []
                 for key in constraint['or'].keys():
                     sub_constraint = constraint['or'][key]
-                    raw_or.append(sub_constraint)
-                    or_constraints.extend(self.parse_constraint(var_generator, sub_constraint, constraints_id + '_c' + str(i + 1), target_def, None, []))
-                constraints.extend(self.parse_constraint(var_generator, constraint, constraints_id + '_c' + str(i + 1), target_def, or_constraints, raw_or))
+                    or_constraints.extend(self.parse_constraint(var_generator, sub_constraint, constraints_id + '_c' + str(i + 1), target_def, None))
+                constraints.extend(self.parse_constraint(var_generator, constraint, constraints_id + '_c' + str(i + 1), target_def, or_constraints))
             else:
-                constraints.extend(self.parse_constraint(var_generator, constraint, constraints_id + '_c' + str(i + 1), target_def, None, []))
+                constraints.extend(self.parse_constraint(var_generator, constraint, constraints_id + '_c' + str(i + 1), target_def, None))
 
         return constraints
 
     @staticmethod
-    def parse_constraint(var_generator, obj, id_, target_def, options=None, raw_or=None):
+    def parse_constraint(var_generator, obj, id_, target_def, options=None):
         """
         Parses one constraint to the internal representation.
 
         :param var_generator: reference to the VariableGenerator instance for variable generation for SPARQL queries
         :param obj: the constraint in its original representation
         :param id_: suffix for the constraint ID
         :param target_def: the target definition of the associated shape
         :param options: contains Constraints for or_operation
-        :param raw_or: contains only the raw form of the options for the 'or' operation
         :return: constraint in internal representation
         """
         min_ = obj.get('min')
         max_ = obj.get('max')
         shape_ref = obj.get('shape')
         datatype = obj.get('datatype')
         value = obj.get('value')
@@ -512,16 +509,16 @@
 
         if urlparse(datatype).netloc != '' and datatype is not None:  # if the data type is a url, add '<>' to it
             o_datatype = '<' + datatype + '>'
 
         if o_path is not None:
             if o_min is not None:
                 if o_max is not None:
-                    return [MinOnlyConstraint(var_generator, id_, o_path, o_min, o_neg, options, raw_or, o_datatype, o_value, o_shape_ref, target_def),
-                            MaxOnlyConstraint(var_generator, id_, o_path, o_max, o_neg, options, raw_or, o_datatype, o_value, o_shape_ref, target_def)]
-                return [MinOnlyConstraint(var_generator, id_, o_path, o_min, o_neg, options, raw_or, o_datatype, o_value, o_shape_ref, target_def)]
+                    return [MinOnlyConstraint(var_generator, id_, o_path, o_min, o_neg, options, o_datatype, o_value, o_shape_ref, target_def),
+                            MaxOnlyConstraint(var_generator, id_, o_path, o_max, o_neg, options, o_datatype, o_value, o_shape_ref, target_def)]
+                return [MinOnlyConstraint(var_generator, id_, o_path, o_min, o_neg, options, o_datatype, o_value, o_shape_ref, target_def)]
             if o_max is not None:
-                return [MaxOnlyConstraint(var_generator, id_, o_path, o_max, o_neg, options, raw_or, o_datatype, o_value, o_shape_ref, target_def)]
+                return [MaxOnlyConstraint(var_generator, id_, o_path, o_max, o_neg, options, o_datatype, o_value, o_shape_ref, target_def)]
         elif o_query is not None:
             return [SPARQLConstraint(id_, o_neg, o_query)]
         elif o_path is None:
-            return [MinOnlyConstraint(var_generator, id_, o_path, o_min, o_neg, options, raw_or, o_datatype, o_value, o_shape_ref, target_def)]
+            return [MinOnlyConstraint(var_generator, id_, o_path, o_min, o_neg, options, o_datatype, o_value, o_shape_ref, target_def)]
```

### Comparing `TravSHACL-1.4.1/TravSHACL/core/ShapeSchema.py` & `TravSHACL-1.4.2/TravSHACL/core/ShapeSchema.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.4.1/TravSHACL/rule_based_validation/InstancesRetrieval.py` & `TravSHACL-1.4.2/TravSHACL/rule_based_validation/InstancesRetrieval.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.4.1/TravSHACL/rule_based_validation/Validation.py` & `TravSHACL-1.4.2/TravSHACL/rule_based_validation/Validation.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.4.1/TravSHACL/sparql/QueryGenerator.py` & `TravSHACL-1.4.2/TravSHACL/sparql/QueryGenerator.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,15 +254,14 @@
         self.id = id_
         self.subquery = subquery
         self.projected_variables = projected_variables
         self.filters = []
         self.triples = []
         self.union_triples = []
         self.max_dict = {}
-        self.or_triples = []
 
         self.include_selectivity = is_selective
         self.target_query = target_query
         self.constraints = constraints
         self.include_ORDERBY = include_order_by
         self.inter_shape_refs = {}
         self.prefix_string = prefix_string
@@ -541,36 +540,33 @@
 
         :param c: the constraint to be included in the query
         :param or_value: used in the case of multiple 'or' for triple grouping
         :param or_affix: used in the case of more than one or triple within an option in an 'or' operation
         :param maxonly: tells if the constraint is maxonly
         """
         variables = c.get_variables()
-        if c.raw_or:            # the use of raw_or is highly debatable. Only important with or_constraint within property in shapes_graph
-            self.or_triples = ['<' + entry['path'] + '>' for entry in c.raw_or]
         if not maxonly:
             if isinstance(c, Constraint):
                 path = c.path
-                if path not in self.or_triples:
-                    if c.get_value() is not None:  # if there is fixed value for the object
-                        if or_value > 0:
-                            self.add_union_triples(path, c.get_value(), or_value, or_affix)
-                        else:
-                            self.add_triple(path, c.get_value())
-                        return
-
+                if c.get_value() is not None:  # if there is fixed value for the object
                     if or_value > 0:
-                        v = variables[0]
-                        self.add_union_triples(path, '?' + v, or_value, or_affix, card=c.min)
+                        self.add_union_triples(path, c.get_value(), or_value, or_affix)
                     else:
-                        for v in variables:
-                            if c.get_shape_ref() is not None:  # if there is an existing reference to another shape
-                                self.inter_shape_refs[v] = c.get_shape_ref()
-                                self.triples.append('\n$inter_shape_type_to_add$')
-                            self.add_triple(path, '?' + v)
+                        self.add_triple(path, c.get_value())
+                    return
+
+                if or_value > 0:
+                    v = variables[0]
+                    self.add_union_triples(path, '?' + v, or_value, or_affix, card=c.min)
+                else:
+                    for v in variables:
+                        if c.get_shape_ref() is not None:  # if there is an existing reference to another shape
+                            self.inter_shape_refs[v] = c.get_shape_ref()
+                            self.triples.append('\n$inter_shape_type_to_add$')
+                        self.add_triple(path, '?' + v)
 
             if c.get_value() is not None:
                 self.add_constant_filter(
                     variables.iterator().next(),
                     c.get_value().get(),
                     c.get_is_pos()
                 )
```

### Comparing `TravSHACL-1.4.1/TravSHACL/sparql/SPARQLEndpoint.py` & `TravSHACL-1.4.2/TravSHACL/sparql/SPARQLEndpoint.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.4.1/TravSHACL/utils/ValidationStats.py` & `TravSHACL-1.4.2/TravSHACL/utils/ValidationStats.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.4.1/TravSHACL/utils/VariableGenerator.py` & `TravSHACL-1.4.2/TravSHACL/utils/VariableGenerator.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.4.1/TravSHACL/utils/fileManagement.py` & `TravSHACL-1.4.2/TravSHACL/utils/fileManagement.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.4.1/TravSHACL.egg-info/PKG-INFO` & `TravSHACL-1.4.2/TravSHACL.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: TravSHACL
-Version: 1.4.1
+Version: 1.4.2
 Summary: A SHACL validator capable of planning the traversal and execution of the validation of a shape schema to detect violations early.
 Home-page: https://github.com/SDM-TIB/Trav-SHACL
-Download-URL: https://github.com/SDM-TIB/Trav-SHACL/archive/refs/tags/v1.4.1.tar.gz
+Download-URL: https://github.com/SDM-TIB/Trav-SHACL/archive/refs/tags/v1.4.2.tar.gz
 Author: Mónica Figuera, Philipp D. Rohde
 Author-email: philipp.rohde@tib.eu
 License: GNU/GPLv3
 Classifier: Development Status :: 5 - Production/Stable 
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `TravSHACL-1.4.1/TravSHACL.egg-info/SOURCES.txt` & `TravSHACL-1.4.2/TravSHACL.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.4.1/setup.py` & `TravSHACL-1.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.4.1/tests/test_cases.py` & `TravSHACL-1.4.2/tests/test_cases.py`

 * *Files identical despite different names*

