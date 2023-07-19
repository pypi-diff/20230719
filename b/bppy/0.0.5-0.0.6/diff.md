# Comparing `tmp/bppy-0.0.5.tar.gz` & `tmp/bppy-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bppy-0.0.5.tar", last modified: Wed May 31 14:48:36 2023, max compression
+gzip compressed data, was "bppy-0.0.6.tar", last modified: Wed Jul 19 14:03:11 2023, max compression
```

## Comparing `bppy-0.0.5.tar` & `bppy-0.0.6.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:48:36.863540 bppy-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-31 14:48:25.000000 bppy-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-31 14:48:25.000000 bppy-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-31 14:48:36.863540 bppy-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-31 14:48:25.000000 bppy-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:48:36.859540 bppy-0.0.5/bppy/
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:48:36.859540 bppy-0.0.5/bppy/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/examples/exponential_growth.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/examples/external_events.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/examples/hello_world.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/examples/hot_cold_all.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/examples/hot_cold_bath.py
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/examples/hot_cold_dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/examples/hot_cold_smt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/examples/robots_smt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/examples/tic_tac_toe_priorities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:48:36.859540 bppy-0.0.5/bppy/execution/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/execution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:48:36.859540 bppy-0.0.5/bppy/execution/listeners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/execution/listeners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/execution/listeners/b_program_runner_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/execution/listeners/print_b_program_runner_listener.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:48:36.859540 bppy-0.0.5/bppy/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/model/b_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/model/b_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/model/bprogram.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:48:36.859540 bppy-0.0.5/bppy/model/event_selection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/model/event_selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/model/event_selection/event_selection_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/model/event_selection/experimental_smt_event_selection_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/model/event_selection/priority_based_event_selection_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/model/event_selection/simple_event_selection_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/model/event_selection/smt_event_selection_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/model/event_selection/solver_based_event_selection_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/model/event_set.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/model/sync_statement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:48:36.863540 bppy-0.0.5/bppy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-31 14:48:25.000000 bppy-0.0.5/bppy/utils/z3helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:48:36.859540 bppy-0.0.5/bppy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-31 14:48:36.000000 bppy-0.0.5/bppy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-31 14:48:36.000000 bppy-0.0.5/bppy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 14:48:36.000000 bppy-0.0.5/bppy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-31 14:48:36.000000 bppy-0.0.5/bppy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-31 14:48:36.000000 bppy-0.0.5/bppy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 14:48:36.863540 bppy-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-31 14:48:25.000000 bppy-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:48:36.863540 bppy-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-31 14:48:25.000000 bppy-0.0.5/tests/test_bprogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     9608 2023-05-31 14:48:25.000000 bppy-0.0.5/tests/test_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:03:11.483063 bppy-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-19 14:02:59.000000 bppy-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-19 14:02:59.000000 bppy-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-19 14:03:11.483063 bppy-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-19 14:02:59.000000 bppy-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:03:11.479063 bppy-0.0.6/bppy/
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-19 14:02:59.000000 bppy-0.0.6/bppy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:03:11.483063 bppy-0.0.6/bppy/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-19 14:02:59.000000 bppy-0.0.6/bppy/examples/exponential_growth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-19 14:02:59.000000 bppy-0.0.6/bppy/examples/external_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-19 14:02:59.000000 bppy-0.0.6/bppy/examples/hello_world.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-19 14:02:59.000000 bppy-0.0.6/bppy/examples/hot_cold_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-19 14:02:59.000000 bppy-0.0.6/bppy/examples/hot_cold_bath.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-19 14:02:59.000000 bppy-0.0.6/bppy/examples/hot_cold_dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-19 14:02:59.000000 bppy-0.0.6/bppy/examples/hot_cold_smt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-07-19 14:02:59.000000 bppy-0.0.6/bppy/examples/robots_smt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-07-19 14:02:59.000000 bppy-0.0.6/bppy/examples/tic_tac_toe_priorities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:03:11.483063 bppy-0.0.6/bppy/execution/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 14:02:59.000000 bppy-0.0.6/bppy/execution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:03:11.483063 bppy-0.0.6/bppy/execution/listeners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 14:02:59.000000 bppy-0.0.6/bppy/execution/listeners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-19 14:02:59.000000 bppy-0.0.6/bppy/execution/listeners/b_program_runner_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-19 14:02:59.000000 bppy-0.0.6/bppy/execution/listeners/print_b_program_runner_listener.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:03:11.483063 bppy-0.0.6/bppy/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 14:02:59.000000 bppy-0.0.6/bppy/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-19 14:02:59.000000 bppy-0.0.6/bppy/model/b_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-19 14:02:59.000000 bppy-0.0.6/bppy/model/b_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-07-19 14:02:59.000000 bppy-0.0.6/bppy/model/bprogram.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:03:11.483063 bppy-0.0.6/bppy/model/event_selection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 14:02:59.000000 bppy-0.0.6/bppy/model/event_selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-19 14:02:59.000000 bppy-0.0.6/bppy/model/event_selection/event_selection_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-19 14:02:59.000000 bppy-0.0.6/bppy/model/event_selection/experimental_smt_event_selection_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-07-19 14:02:59.000000 bppy-0.0.6/bppy/model/event_selection/priority_based_event_selection_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-07-19 14:02:59.000000 bppy-0.0.6/bppy/model/event_selection/simple_event_selection_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-07-19 14:02:59.000000 bppy-0.0.6/bppy/model/event_selection/smt_event_selection_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-19 14:02:59.000000 bppy-0.0.6/bppy/model/event_selection/solver_based_event_selection_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-07-19 14:02:59.000000 bppy-0.0.6/bppy/model/event_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-19 14:02:59.000000 bppy-0.0.6/bppy/model/sync_statement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:03:11.483063 bppy-0.0.6/bppy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 14:02:59.000000 bppy-0.0.6/bppy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-19 14:02:59.000000 bppy-0.0.6/bppy/utils/z3helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:03:11.479063 bppy-0.0.6/bppy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-19 14:03:11.000000 bppy-0.0.6/bppy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-19 14:03:11.000000 bppy-0.0.6/bppy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 14:03:11.000000 bppy-0.0.6/bppy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-19 14:03:11.000000 bppy-0.0.6/bppy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-19 14:03:11.000000 bppy-0.0.6/bppy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 14:03:11.483063 bppy-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-19 14:02:59.000000 bppy-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:03:11.483063 bppy-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-19 14:02:59.000000 bppy-0.0.6/tests/test_bprogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9608 2023-07-19 14:02:59.000000 bppy-0.0.6/tests/test_examples.py
```

### Comparing `bppy-0.0.5/LICENSE` & `bppy-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bppy-0.0.5/PKG-INFO` & `bppy-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bppy
-Version: 0.0.5
+Version: 0.0.6
 Summary: BPpy: Behavioral Programming In Python
 Home-page: https://github.com/bThink-BGU/BPpy
 Author: Tom Yaacov
 Author-email: tomyaacov1210@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `bppy-0.0.5/README.md` & `bppy-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `bppy-0.0.5/bppy/__init__.py` & `bppy-0.0.6/bppy/__init__.py`

 * *Files identical despite different names*

### Comparing `bppy-0.0.5/bppy/examples/external_events.py` & `bppy-0.0.6/bppy/examples/external_events.py`

 * *Files identical despite different names*

### Comparing `bppy-0.0.5/bppy/examples/hot_cold_all.py` & `bppy-0.0.6/bppy/examples/hot_cold_all.py`

 * *Files identical despite different names*

### Comparing `bppy-0.0.5/bppy/examples/hot_cold_bath.py` & `bppy-0.0.6/bppy/examples/hot_cold_bath.py`

 * *Files identical despite different names*

### Comparing `bppy-0.0.5/bppy/examples/hot_cold_dynamic.py` & `bppy-0.0.6/bppy/examples/hot_cold_dynamic.py`

 * *Files identical despite different names*

### Comparing `bppy-0.0.5/bppy/examples/hot_cold_smt.py` & `bppy-0.0.6/bppy/examples/hot_cold_smt.py`

 * *Files identical despite different names*

### Comparing `bppy-0.0.5/bppy/examples/robots_smt.py` & `bppy-0.0.6/bppy/examples/robots_smt.py`

 * *Files identical despite different names*

### Comparing `bppy-0.0.5/bppy/examples/tic_tac_toe_priorities.py` & `bppy-0.0.6/bppy/examples/tic_tac_toe_priorities.py`

 * *Files identical despite different names*

### Comparing `bppy-0.0.5/bppy/model/event_selection/smt_event_selection_strategy.py` & `bppy-0.0.6/bppy/model/event_selection/smt_event_selection_strategy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 from bppy.model.event_selection.solver_based_event_selection_strategy import SolverBasedEventSelectionStrategy
 from bppy.utils.z3helper import *
 
 
 class SMTEventSelectionStrategy(SolverBasedEventSelectionStrategy):
+    """
+    A solver-based implementation of EventSelectionStrategy using z3 SMT solver. The strategy used is the one
+    presented in the paper `Executing Scenario-Based Specification with Dynamic Generation of Rich Events
+    <https://www.wisdom.weizmann.ac.il/~dharel/papers/CCIS2019RichEvents.pdf>`_.
+    """
 
     def is_satisfied(self, event, statement):
         return is_true(event.eval(statement.get('waitFor', true)))  
 
     # TODO: implement a way to set additional_statement
     def select(self, statements, additional_statement=None):
         if isinstance(additional_statement, list) and len(additional_statement) > 0:
```

### Comparing `bppy-0.0.5/bppy/utils/z3helper.py` & `bppy-0.0.6/bppy/utils/z3helper.py`

 * *Files identical despite different names*

### Comparing `bppy-0.0.5/bppy.egg-info/PKG-INFO` & `bppy-0.0.6/bppy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bppy
-Version: 0.0.5
+Version: 0.0.6
 Summary: BPpy: Behavioral Programming In Python
 Home-page: https://github.com/bThink-BGU/BPpy
 Author: Tom Yaacov
 Author-email: tomyaacov1210@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `bppy-0.0.5/bppy.egg-info/SOURCES.txt` & `bppy-0.0.6/bppy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bppy-0.0.5/setup.py` & `bppy-0.0.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import setuptools
-
-with open("README.md", "r") as fh:
+import os
+__location__ = os.path.realpath(os.path.join(os.getcwd(), os.path.dirname(__file__)))
+with open(os.path.join(__location__, "README.md"), "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="bppy",
-    version="0.0.5",
+    version="0.0.6",
     author="Tom Yaacov",
     author_email="tomyaacov1210@gmail.com",
     description="BPpy: Behavioral Programming In Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/bThink-BGU/BPpy",
     packages=setuptools.find_packages(),
```

### Comparing `bppy-0.0.5/tests/test_bprogram.py` & `bppy-0.0.6/tests/test_bprogram.py`

 * *Files identical despite different names*

### Comparing `bppy-0.0.5/tests/test_examples.py` & `bppy-0.0.6/tests/test_examples.py`

 * *Files identical despite different names*

