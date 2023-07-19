# Comparing `tmp/openssm_dev-0.1.5.tar.gz` & `tmp/openssm_dev-0.1.6.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openssm_dev-0.1.5.tar", max compression
+gzip compressed data, was "openssm_dev-0.1.6.dev0.tar", max compression
```

## Comparing `openssm_dev-0.1.5.tar` & `openssm_dev-0.1.6.dev0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     7181 2023-07-18 23:30:27.448992 openssm_dev-0.1.5/README.md
--rw-r--r--   0        0        0       79 2023-07-11 05:54:22.327687 openssm_dev-0.1.5/openssm/Makefile
--rw-r--r--   0        0        0     2553 2023-07-11 05:54:22.327950 openssm_dev-0.1.5/openssm/README.md
--rw-r--r--   0        0        0        0 2023-07-05 16:04:01.482785 openssm_dev-0.1.5/openssm/__init__.py
--rw-r--r--   0        0        0      899 2023-07-18 02:22:03.792028 openssm_dev-0.1.5/openssm/config.py
--rw-r--r--   0        0        0      754 2023-07-18 02:22:03.792311 openssm_dev-0.1.5/openssm/contrib/ssms/industrial_boilers_ssm/__init__.py
--rw-r--r--   0        0        0      789 2023-07-18 02:22:03.792644 openssm_dev-0.1.5/openssm/contrib/ssms/japan_fish_kcp_ssm/__init__.py
--rw-r--r--   0        0        0     1010 2023-07-18 02:22:03.792852 openssm_dev-0.1.5/openssm/contrib/ssms/mri_operator_ssm/__init__.py
--rw-r--r--   0        0        0     1610 2023-07-18 02:22:03.793056 openssm_dev-0.1.5/openssm/contrib/ssms/semiconductor_ssm/__init__.py
--rw-r--r--   0        0        0       19 2023-07-05 16:04:01.482973 openssm_dev-0.1.5/openssm/core/__init__.py
--rw-r--r--   0        0        0        0 2023-07-18 06:13:04.768495 openssm_dev-0.1.5/openssm/core/adapter/__init__.py
--rw-r--r--   0        0        0     2203 2023-07-18 23:30:27.459226 openssm_dev-0.1.5/openssm/core/adapter/abstract_adapter.py
--rw-r--r--   0        0        0     3399 2023-07-18 23:30:27.459767 openssm_dev-0.1.5/openssm/core/adapter/base_adapter.py
--rw-r--r--   0        0        0     4042 2023-07-18 23:30:27.460035 openssm_dev-0.1.5/openssm/core/adapter/llama_index_adapter.py
--rw-r--r--   0        0        0        0 2023-07-18 06:13:04.769364 openssm_dev-0.1.5/openssm/core/backend/__init__.py
--rw-r--r--   0        0        0     1192 2023-07-18 23:30:27.460229 openssm_dev-0.1.5/openssm/core/backend/abstract_backend.py
--rw-r--r--   0        0        0     1633 2023-07-18 23:30:27.460388 openssm_dev-0.1.5/openssm/core/backend/base_backend.py
--rw-r--r--   0        0        0      896 2023-07-18 23:30:27.460553 openssm_dev-0.1.5/openssm/core/backend/text_backend.py
--rw-r--r--   0        0        0        0 2023-07-18 06:13:04.770313 openssm_dev-0.1.5/openssm/core/inferencer/__init__.py
--rw-r--r--   0        0        0      720 2023-07-11 05:54:22.329332 openssm_dev-0.1.5/openssm/core/inferencer/abstract_inferencer.py
--rw-r--r--   0        0        0      458 2023-07-18 02:22:03.796108 openssm_dev-0.1.5/openssm/core/inferencer/base_inferencer.py
--rw-r--r--   0        0        0      442 2023-07-11 20:37:04.252092 openssm_dev-0.1.5/openssm/core/inferencer/text_formula_inferencer.py
--rw-r--r--   0        0        0        0 2023-07-18 06:13:04.770377 openssm_dev-0.1.5/openssm/core/slm/__init__.py
--rw-r--r--   0        0        0      885 2023-07-18 02:22:03.796723 openssm_dev-0.1.5/openssm/core/slm/abstract_slm.py
--rw-r--r--   0        0        0     5007 2023-07-18 23:30:27.460799 openssm_dev-0.1.5/openssm/core/slm/base_slm.py
--rw-r--r--   0        0        0     6355 2023-07-18 23:30:27.461046 openssm_dev-0.1.5/openssm/core/slm/huggingface_slm.py
--rw-r--r--   0        0        0        0 2023-07-18 06:13:04.770841 openssm_dev-0.1.5/openssm/core/slm/memory/__init__.py
--rw-r--r--   0        0        0      452 2023-07-18 23:30:27.461233 openssm_dev-0.1.5/openssm/core/slm/memory/conversation_db.py
--rw-r--r--   0        0        0     1620 2023-07-18 02:22:03.797836 openssm_dev-0.1.5/openssm/core/slm/memory/sqlite_conversation_db.py
--rw-r--r--   0        0        0     1683 2023-07-18 23:30:27.461419 openssm_dev-0.1.5/openssm/core/slm/openai_slm.py
--rw-r--r--   0        0        0        0 2023-07-18 06:13:04.771113 openssm_dev-0.1.5/openssm/core/ssm/__init__.py
--rw-r--r--   0        0        0     2307 2023-07-18 02:22:03.798567 openssm_dev-0.1.5/openssm/core/ssm/abstract_ssm.py
--rw-r--r--   0        0        0     3037 2023-07-18 02:22:03.798847 openssm_dev-0.1.5/openssm/core/ssm/base_ssm.py
--rw-r--r--   0        0        0      454 2023-07-18 23:27:32.506046 openssm_dev-0.1.5/openssm/core/ssm/gpt3_llama_index_ssm.py
--rw-r--r--   0        0        0      747 2023-07-18 02:22:03.799477 openssm_dev-0.1.5/openssm/core/ssm/huggingface_ssm.py
--rw-r--r--   0        0        0      770 2023-07-18 06:13:04.771412 openssm_dev-0.1.5/openssm/core/ssm/openai_ssm.py
--rw-r--r--   0        0        0       58 2023-07-05 16:04:01.488477 openssm_dev-0.1.5/openssm/industrial/interpretability/README.md
--rw-r--r--   0        0        0       60 2023-07-05 16:04:01.488662 openssm_dev-0.1.5/openssm/industrial/monitoring/README.md
--rw-r--r--   0        0        0        0 2023-07-05 16:04:01.488770 openssm_dev-0.1.5/openssm/industrial/security/README.md
--rw-r--r--   0        0        0        0 2023-07-05 16:04:01.488908 openssm_dev-0.1.5/openssm/industrial/security/audit/README.md
--rw-r--r--   0        0        0        0 2023-07-05 16:04:01.489033 openssm_dev-0.1.5/openssm/industrial/security/best_practices/README.md
--rw-r--r--   0        0        0       63 2023-07-05 16:04:01.489309 openssm_dev-0.1.5/openssm/integration/README.md
--rw-r--r--   0        0        0     3574 2023-07-05 16:04:01.489472 openssm_dev-0.1.5/openssm/integration/llamaindex/README.md
--rw-r--r--   0        0        0       34 2023-07-05 16:04:01.489708 openssm_dev-0.1.5/openssm/integration/testing_tools/README.md
--rw-r--r--   0        0        0      831 2023-07-18 23:36:39.596675 openssm_dev-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     7940 1970-01-01 00:00:00.000000 openssm_dev-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     7181 2023-07-19 02:34:22.673459 openssm_dev-0.1.6.dev0/README.md
+-rw-r--r--   0        0        0       79 2023-07-11 05:54:22.327687 openssm_dev-0.1.6.dev0/openssm/Makefile
+-rw-r--r--   0        0        0     2553 2023-07-11 05:54:22.327950 openssm_dev-0.1.6.dev0/openssm/README.md
+-rw-r--r--   0        0        0        0 2023-07-05 16:04:01.482785 openssm_dev-0.1.6.dev0/openssm/__init__.py
+-rw-r--r--   0        0        0      899 2023-07-18 02:22:03.792028 openssm_dev-0.1.6.dev0/openssm/config.py
+-rw-r--r--   0        0        0      754 2023-07-18 02:22:03.792311 openssm_dev-0.1.6.dev0/openssm/contrib/ssms/industrial_boilers_ssm/__init__.py
+-rw-r--r--   0        0        0      789 2023-07-18 02:22:03.792644 openssm_dev-0.1.6.dev0/openssm/contrib/ssms/japan_fish_kcp_ssm/__init__.py
+-rw-r--r--   0        0        0     1010 2023-07-18 02:22:03.792852 openssm_dev-0.1.6.dev0/openssm/contrib/ssms/mri_operator_ssm/__init__.py
+-rw-r--r--   0        0        0     1610 2023-07-18 02:22:03.793056 openssm_dev-0.1.6.dev0/openssm/contrib/ssms/semiconductor_ssm/__init__.py
+-rw-r--r--   0        0        0       19 2023-07-05 16:04:01.482973 openssm_dev-0.1.6.dev0/openssm/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-18 06:13:04.768495 openssm_dev-0.1.6.dev0/openssm/core/adapter/__init__.py
+-rw-r--r--   0        0        0     2199 2023-07-19 02:43:24.231241 openssm_dev-0.1.6.dev0/openssm/core/adapter/abstract_adapter.py
+-rw-r--r--   0        0        0     3401 2023-07-19 02:43:24.231585 openssm_dev-0.1.6.dev0/openssm/core/adapter/base_adapter.py
+-rw-r--r--   0        0        0     4001 2023-07-19 03:54:14.438862 openssm_dev-0.1.6.dev0/openssm/core/adapter/llama_index_adapter.py
+-rw-r--r--   0        0        0        0 2023-07-18 06:13:04.769364 openssm_dev-0.1.6.dev0/openssm/core/backend/__init__.py
+-rw-r--r--   0        0        0     1194 2023-07-19 02:43:24.231970 openssm_dev-0.1.6.dev0/openssm/core/backend/abstract_backend.py
+-rw-r--r--   0        0        0     1635 2023-07-19 02:43:24.232293 openssm_dev-0.1.6.dev0/openssm/core/backend/base_backend.py
+-rw-r--r--   0        0        0      897 2023-07-19 02:43:24.232711 openssm_dev-0.1.6.dev0/openssm/core/backend/text_backend.py
+-rw-r--r--   0        0        0        0 2023-07-18 06:13:04.770313 openssm_dev-0.1.6.dev0/openssm/core/inferencer/__init__.py
+-rw-r--r--   0        0        0      720 2023-07-11 05:54:22.329332 openssm_dev-0.1.6.dev0/openssm/core/inferencer/abstract_inferencer.py
+-rw-r--r--   0        0        0      458 2023-07-18 02:22:03.796108 openssm_dev-0.1.6.dev0/openssm/core/inferencer/base_inferencer.py
+-rw-r--r--   0        0        0      442 2023-07-11 20:37:04.252092 openssm_dev-0.1.6.dev0/openssm/core/inferencer/text_formula_inferencer.py
+-rw-r--r--   0        0        0        0 2023-07-18 06:13:04.770377 openssm_dev-0.1.6.dev0/openssm/core/slm/__init__.py
+-rw-r--r--   0        0        0      885 2023-07-18 02:22:03.796723 openssm_dev-0.1.6.dev0/openssm/core/slm/abstract_slm.py
+-rw-r--r--   0        0        0     5007 2023-07-19 02:34:22.688509 openssm_dev-0.1.6.dev0/openssm/core/slm/base_slm.py
+-rw-r--r--   0        0        0     6355 2023-07-19 02:34:22.689111 openssm_dev-0.1.6.dev0/openssm/core/slm/huggingface_slm.py
+-rw-r--r--   0        0        0        0 2023-07-18 06:13:04.770841 openssm_dev-0.1.6.dev0/openssm/core/slm/memory/__init__.py
+-rw-r--r--   0        0        0      452 2023-07-19 02:34:22.689574 openssm_dev-0.1.6.dev0/openssm/core/slm/memory/conversation_db.py
+-rw-r--r--   0        0        0     1620 2023-07-18 02:22:03.797836 openssm_dev-0.1.6.dev0/openssm/core/slm/memory/sqlite_conversation_db.py
+-rw-r--r--   0        0        0     1685 2023-07-19 02:34:22.689924 openssm_dev-0.1.6.dev0/openssm/core/slm/openai_slm.py
+-rw-r--r--   0        0        0        0 2023-07-18 06:13:04.771113 openssm_dev-0.1.6.dev0/openssm/core/ssm/__init__.py
+-rw-r--r--   0        0        0     2307 2023-07-18 02:22:03.798567 openssm_dev-0.1.6.dev0/openssm/core/ssm/abstract_ssm.py
+-rw-r--r--   0        0        0     3037 2023-07-18 02:22:03.798847 openssm_dev-0.1.6.dev0/openssm/core/ssm/base_ssm.py
+-rw-r--r--   0        0        0      471 2023-07-19 03:54:14.439712 openssm_dev-0.1.6.dev0/openssm/core/ssm/gpt3_llama_index_ssm.py
+-rw-r--r--   0        0        0      747 2023-07-18 02:22:03.799477 openssm_dev-0.1.6.dev0/openssm/core/ssm/huggingface_ssm.py
+-rw-r--r--   0        0        0      770 2023-07-18 06:13:04.771412 openssm_dev-0.1.6.dev0/openssm/core/ssm/openai_ssm.py
+-rw-r--r--   0        0        0       58 2023-07-05 16:04:01.488477 openssm_dev-0.1.6.dev0/openssm/industrial/interpretability/README.md
+-rw-r--r--   0        0        0       60 2023-07-05 16:04:01.488662 openssm_dev-0.1.6.dev0/openssm/industrial/monitoring/README.md
+-rw-r--r--   0        0        0        0 2023-07-05 16:04:01.488770 openssm_dev-0.1.6.dev0/openssm/industrial/security/README.md
+-rw-r--r--   0        0        0        0 2023-07-05 16:04:01.488908 openssm_dev-0.1.6.dev0/openssm/industrial/security/audit/README.md
+-rw-r--r--   0        0        0        0 2023-07-05 16:04:01.489033 openssm_dev-0.1.6.dev0/openssm/industrial/security/best_practices/README.md
+-rw-r--r--   0        0        0       63 2023-07-05 16:04:01.489309 openssm_dev-0.1.6.dev0/openssm/integration/README.md
+-rw-r--r--   0        0        0     3574 2023-07-05 16:04:01.489472 openssm_dev-0.1.6.dev0/openssm/integration/llamaindex/README.md
+-rw-r--r--   0        0        0       34 2023-07-05 16:04:01.489708 openssm_dev-0.1.6.dev0/openssm/integration/testing_tools/README.md
+-rw-r--r--   0        0        0      837 2023-07-19 06:30:05.159596 openssm_dev-0.1.6.dev0/pyproject.toml
+-rw-r--r--   0        0        0     7873 1970-01-01 00:00:00.000000 openssm_dev-0.1.6.dev0/PKG-INFO
```

### Comparing `openssm_dev-0.1.5/README.md` & `openssm_dev-0.1.6.dev0/README.md`

 * *Files identical despite different names*

### Comparing `openssm_dev-0.1.5/openssm/README.md` & `openssm_dev-0.1.6.dev0/openssm/README.md`

 * *Files identical despite different names*

### Comparing `openssm_dev-0.1.5/openssm/config.py` & `openssm_dev-0.1.6.dev0/openssm/config.py`

 * *Files identical despite different names*

### Comparing `openssm_dev-0.1.5/openssm/contrib/ssms/industrial_boilers_ssm/__init__.py` & `openssm_dev-0.1.6.dev0/openssm/contrib/ssms/industrial_boilers_ssm/__init__.py`

 * *Files identical despite different names*

### Comparing `openssm_dev-0.1.5/openssm/contrib/ssms/japan_fish_kcp_ssm/__init__.py` & `openssm_dev-0.1.6.dev0/openssm/contrib/ssms/japan_fish_kcp_ssm/__init__.py`

 * *Files identical despite different names*

### Comparing `openssm_dev-0.1.5/openssm/contrib/ssms/mri_operator_ssm/__init__.py` & `openssm_dev-0.1.6.dev0/openssm/contrib/ssms/mri_operator_ssm/__init__.py`

 * *Files identical despite different names*

### Comparing `openssm_dev-0.1.5/openssm/contrib/ssms/semiconductor_ssm/__init__.py` & `openssm_dev-0.1.6.dev0/openssm/contrib/ssms/semiconductor_ssm/__init__.py`

 * *Files identical despite different names*

### Comparing `openssm_dev-0.1.5/openssm/core/adapter/abstract_adapter.py` & `openssm_dev-0.1.6.dev0/openssm/core/adapter/abstract_adapter.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     """
     The AbstractAdapter serves as the base for all concrete Adapter classes.
     It provides an interface for interaction between the Small Language Model
     (SLM) and the Backend.
     """
 
     @abstractmethod
-    def query(self, conversation_id: str, user_input: str) -> list({}):
+    def query(self, conversation_id: str, user_input: str) -> list[dict]:
         """
         Queries the backends for a response to the user's input.
         :param user_query: The user's input.
         :return: The backend's response.
         """
 
     @abstractmethod
@@ -31,33 +31,33 @@
 
     @abstractmethod
     def list_facts(self) -> list[str]:
         """Lists all known facts."""
         facts = set()
         for backend in self.get_backends():
             if backend is AbstractBackend:
-                facts.add(backend.list_facts())
+                facts |= backend.list_facts()
         return facts
 
     @abstractmethod
     def list_inferencers(self):
         """Lists all known inferencers."""
         inferencers = set()
         for backend in self.get_backends():
             if backend is AbstractBackend:
-                inferencers.add(backend.list_inferencers())
+                inferencers |= backend.list_inferencers()
         return inferencers
 
     @abstractmethod
     def list_heuristics(self):
         """Lists all known heuristics."""
         heuristics = set()
         for backend in self.get_backends():
             if backend is AbstractBackend:
-                heuristics.add(backend.list_inferencers())
+                heuristics |= backend.list_inferencers()
         return heuristics
 
     @abstractmethod
     def select_facts(self, criteria):
         """Selects or searches for facts based on provided criteria."""
 
     @abstractmethod
```

### Comparing `openssm_dev-0.1.5/openssm/core/adapter/base_adapter.py` & `openssm_dev-0.1.6.dev0/openssm/core/adapter/base_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 class BaseAdapter(AbstractAdapter):
     """Base adapter class for SSMs."""
 
     def __init__(self, backends: list[AbstractBackend] = None):
         self.backends = backends or []
 
-    def query(self, conversation_id: str, user_input: str) -> list({}):
+    def query(self, conversation_id: str, user_input: str) -> list[dict]:
         """
         Queries the backends for a response to the user's input.
         :param user_query: The user's input.
         :return: The backend's response.
         """
         responses = [
             r for b in self.backends for r in b.query(
```

### Comparing `openssm_dev-0.1.5/openssm/core/adapter/llama_index_adapter.py` & `openssm_dev-0.1.6.dev0/openssm/core/adapter/llama_index_adapter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-from ast import List
 from typing import Any
-# import llama_index
 from llama_index.indices.base import BaseIndex
 from llama_index.indices.query.base import BaseQueryEngine
 from openssm.core.adapter.base_adapter import BaseAdapter
 from openssm.core.backend.abstract_backend import AbstractBackend
 
 
 class LlamaIndexAdapter(BaseAdapter):
@@ -18,28 +16,28 @@
         super().__init__(backends)
         self.llama_tuples = []
 
     class _LlamaTuple:
         index: BaseIndex = None
         query_engine: BaseQueryEngine = None
 
-    def _get_llama_tuples(self) -> List[_LlamaTuple]:
+    def _get_llama_tuples(self) -> list[_LlamaTuple]:
         if self.llama_tuples is None:
             self.llama_tuples = []
         return self.llama_tuples
 
-    def _get_indexes(self) -> List[BaseIndex]:
+    def _get_indexes(self) -> list[BaseIndex]:
         indexes = [lt.index for lt in self._get_llama_tuples()]
         return indexes
 
-    def _get_query_engines(self) -> List[BaseQueryEngine]:
+    def _get_query_engines(self) -> list[BaseQueryEngine]:
         query_engines = [lt.query_engine for lt in self._get_llama_tuples()]
         return query_engines
 
-    def _query_llama(self, query: str) -> List[Any]:
+    def _query_llama(self, query: str) -> list[Any]:
         responses = []
         # pylint: disable=invalid-name
         for qe in self._get_query_engines():
             response = qe.query(query)
             responses.append(response)
         return responses
 
@@ -95,11 +93,11 @@
         return results
 
     def solve_problem(self, problem_description):
         """Solves a problem based on the provided description."""
         # Use the problem description to query index
         # and retrieve relevant heuristics
         results = self._query_llama(
-            f"problem:{problem_description}")
+            f"problem: {problem_description}")
         # This is a simple example and may need to be enhanced
         # based on how the problem-solving process should work
         return results
```

### Comparing `openssm_dev-0.1.5/openssm/core/backend/abstract_backend.py` & `openssm_dev-0.1.6.dev0/openssm/core/backend/abstract_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from abc import ABC, abstractmethod
 from openssm.core.inferencer.abstract_inferencer import AbstractInferencer
 
 
 # pylint: disable=duplicate-code
 class AbstractBackend(ABC):
     @abstractmethod
-    def query(self, conversation_id: str, user_input: str) -> list({}):
+    def query(self, conversation_id: str, user_input: str) -> list[dict]:
         pass
 
     @abstractmethod
     def load_all(self):
         """
         Loads all facts, inferencers, and heuristics,
         if appropriate. Some backends may not need to,
```

### Comparing `openssm_dev-0.1.5/openssm/core/backend/base_backend.py` & `openssm_dev-0.1.6.dev0/openssm/core/backend/base_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 class BaseBackend(AbstractBackend):
     def __init__(self):
         self.facts = set()
         self.inferencers = set()
         self.heuristics = set()
 
     # pylint: disable=unused-argument
-    def query(self, conversation_id: str, user_input: str) -> list({}):
+    def query(self, conversation_id: str, user_input: str) -> list[dict]:
         return []
 
     def load_all(self):
         """
         The base backend does not load anything.
         It gets all its facts, inferencers, and heuristics
         through the add_* methods.
```

### Comparing `openssm_dev-0.1.5/openssm/core/backend/text_backend.py` & `openssm_dev-0.1.6.dev0/openssm/core/backend/text_backend.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 class TextBackend(BaseBackend):
     def __init__(self):
         super().__init__()
         self.texts = set()
 
     # pylint: disable=unused-argument
-    def query(self, conversation_id: str, user_input: str) -> list({}):
+    def query(self, conversation_id: str, user_input: str) -> list[dict]:
         responses = [{"item": text} for text in self.texts]
         return responses
 
     def all_texts(self):
         return self.texts
 
     def add_fact(self, fact: str):
@@ -22,8 +22,7 @@
     def add_inferencer(self, inferencer: AbstractInferencer):
         super().add_inferencer(inferencer)
         self.texts.add(f"inferencer: {inferencer}")
 
     def add_heuristic(self, heuristic: str):
         super().add_heuristic(heuristic)
         self.texts.add(f"heuristic: {heuristic}")
-
```

### Comparing `openssm_dev-0.1.5/openssm/core/inferencer/abstract_inferencer.py` & `openssm_dev-0.1.6.dev0/openssm/core/inferencer/abstract_inferencer.py`

 * *Files identical despite different names*

### Comparing `openssm_dev-0.1.5/openssm/core/slm/abstract_slm.py` & `openssm_dev-0.1.6.dev0/openssm/core/slm/abstract_slm.py`

 * *Files identical despite different names*

### Comparing `openssm_dev-0.1.5/openssm/core/slm/base_slm.py` & `openssm_dev-0.1.6.dev0/openssm/core/slm/base_slm.py`

 * *Files identical despite different names*

### Comparing `openssm_dev-0.1.5/openssm/core/slm/huggingface_slm.py` & `openssm_dev-0.1.6.dev0/openssm/core/slm/huggingface_slm.py`

 * *Files identical despite different names*

### Comparing `openssm_dev-0.1.5/openssm/core/slm/memory/sqlite_conversation_db.py` & `openssm_dev-0.1.6.dev0/openssm/core/slm/memory/sqlite_conversation_db.py`

 * *Files identical despite different names*

### Comparing `openssm_dev-0.1.5/openssm/core/slm/openai_slm.py` & `openssm_dev-0.1.6.dev0/openssm/core/slm/openai_slm.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,23 +28,25 @@
 
 class GPT3CompletionSLM(GPT3BaseSLM):
     def __init__(self, adapter: AbstractAdapter = None):
         super().__init__(adapter)
 
     def call_lm_api(self, conversation: list[dict]) -> list[dict]:
         prompt = self._make_completion_prompt(conversation)
+
         response = openai.Completion.create(
             engine="text-davinci-002",
             prompt=prompt,
             temperature=0.7,
             max_tokens=500
         )
         # print(f"prompt: {prompt}")
         # print(f"response: {response}")
         response = response.choices[0].text.strip()
+
         replies = self._parse_llm_response(response)
 
         if len(replies) == 0 or len(replies[0]) == 0:
             replies = [{'role': 'assistant', 'content': 'I got nothing.'}]
 
         # print(f"replies: {replies}")
```

### Comparing `openssm_dev-0.1.5/openssm/core/ssm/abstract_ssm.py` & `openssm_dev-0.1.6.dev0/openssm/core/ssm/abstract_ssm.py`

 * *Files identical despite different names*

### Comparing `openssm_dev-0.1.5/openssm/core/ssm/base_ssm.py` & `openssm_dev-0.1.6.dev0/openssm/core/ssm/base_ssm.py`

 * *Files identical despite different names*

### Comparing `openssm_dev-0.1.5/openssm/core/ssm/huggingface_ssm.py` & `openssm_dev-0.1.6.dev0/openssm/core/ssm/huggingface_ssm.py`

 * *Files identical despite different names*

### Comparing `openssm_dev-0.1.5/openssm/core/ssm/openai_ssm.py` & `openssm_dev-0.1.6.dev0/openssm/core/ssm/openai_ssm.py`

 * *Files identical despite different names*

### Comparing `openssm_dev-0.1.5/openssm/integration/llamaindex/README.md` & `openssm_dev-0.1.6.dev0/openssm/integration/llamaindex/README.md`

 * *Files identical despite different names*

### Comparing `openssm_dev-0.1.5/pyproject.toml` & `openssm_dev-0.1.6.dev0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 [tool.poetry]
 authors = ["Aitomatic Engineering <engineering@aitomatic.com>"]
 description = "OpenSSM - 'Small Specialist Models' for Industrial AI"
 name = "openssm-dev"
 packages = [
-  { include = "openssm" },
+  {include = "openssm"},
 ]
 readme = "README.md"
-version = "0.1.5"
+version = "0.1.6.dev0"
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
 
 [tool.poetry.dependencies]
-python = ">=3.8.1,<4.0"
+python = ">=3.10,<4.0"
 # LlamaIndex & related
-llama-hub = ">=0.0.4"
-llama-index = ">=0.6.33"
+llama-hub = ">=0.0.12"
+llama-index = ">=0.7.10"
 # misc / other
-accelerate = "^0.20.3"
-einops = "^0.6.1"
-pypdf = ">=3.11.0"
-pytest = ">=7.0.0"
-transformers = "^4.30.2"
+accelerate = ">=0.21.0"
+einops = ">=0.6.1"
+pypdf = ">=3.12.2"
+pytest = ">=7.4.0"
+transformers = ">=4.31.0"
 torch = ">=1.13.1"
 #xformers = ">=0.0.16"	# don’t include this. It fails on GitHub actions. Support in Makefile.
 #xformers = ">=0.0.20"
 
 [tool.pytest.ini_options]
 filterwarnings = [
   "ignore:pkg_resources is deprecated as an API:DeprecationWarning",
```

### Comparing `openssm_dev-0.1.5/PKG-INFO` & `openssm_dev-0.1.6.dev0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
 Name: openssm-dev
-Version: 0.1.5
+Version: 0.1.6.dev0
 Summary: OpenSSM - 'Small Specialist Models' for Industrial AI
 Author: Aitomatic Engineering
 Author-email: engineering@aitomatic.com
-Requires-Python: >=3.8.1,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: accelerate (>=0.20.3,<0.21.0)
-Requires-Dist: einops (>=0.6.1,<0.7.0)
-Requires-Dist: llama-hub (>=0.0.4)
-Requires-Dist: llama-index (>=0.6.33)
-Requires-Dist: pypdf (>=3.11.0)
-Requires-Dist: pytest (>=7.0.0)
+Requires-Dist: accelerate (>=0.21.0)
+Requires-Dist: einops (>=0.6.1)
+Requires-Dist: llama-hub (>=0.0.12)
+Requires-Dist: llama-index (>=0.7.10)
+Requires-Dist: pypdf (>=3.12.2)
+Requires-Dist: pytest (>=7.4.0)
 Requires-Dist: torch (>=1.13.1)
-Requires-Dist: transformers (>=4.30.2,<5.0.0)
+Requires-Dist: transformers (>=4.31.0)
 Description-Content-Type: text/markdown
 
 # OpenSSM – “Small Specialist Models” for Industrial AI
 
 > &nbsp;
 > See full documentation at [aitomatic.github.io/openssm/](https://aitomatic.github.io/openssm/).
 > &nbsp;
```

