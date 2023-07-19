# Comparing `tmp/langchain_plantuml-0.0.3.tar.gz` & `tmp/langchain_plantuml-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_plantuml-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "langchain_plantuml-0.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `langchain_plantuml-0.0.3.tar` & `langchain_plantuml-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11356 2023-07-17 04:15:28.988093 langchain_plantuml-0.0.3/LICENSE
--rw-r--r--   0        0        0     2870 2023-07-17 04:15:28.988093 langchain_plantuml-0.0.3/README.md
--rw-r--r--   0        0        0      573 2023-07-17 04:15:28.988093 langchain_plantuml-0.0.3/langchain_plantuml/__init__.py
--rw-r--r--   0        0        0      573 2023-07-17 04:15:28.988093 langchain_plantuml-0.0.3/langchain_plantuml/activity_diagram_beta/__init__.py
--rw-r--r--   0        0        0     9386 2023-07-17 04:15:28.988093 langchain_plantuml-0.0.3/langchain_plantuml/activity_diagram_beta/plantuml_activity_diagram_beta_callback_handler.py
--rw-r--r--   0        0        0    13242 2023-07-17 04:15:28.992093 langchain_plantuml-0.0.3/langchain_plantuml/activity_diagram_beta/plantuml_sequence_diagram_callback_handler.py
--rw-r--r--   0        0        0      573 2023-07-17 04:15:28.992093 langchain_plantuml-0.0.3/langchain_plantuml/core/__init__.py
--rw-r--r--   0        0        0     2819 2023-07-17 04:15:28.992093 langchain_plantuml-0.0.3/langchain_plantuml/core/plantuml_callback_handler.py
--rw-r--r--   0        0        0     1139 2023-07-17 04:15:28.992093 langchain_plantuml-0.0.3/langchain_plantuml/diagram.py
--rw-r--r--   0        0        0     1749 2023-07-17 04:15:28.992093 langchain_plantuml-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3982 1970-01-01 00:00:00.000000 langchain_plantuml-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-07-19 11:28:01.365304 langchain_plantuml-0.0.4/LICENSE
+-rw-r--r--   0        0        0     3006 2023-07-19 11:28:01.365304 langchain_plantuml-0.0.4/README.md
+-rw-r--r--   0        0        0      573 2023-07-19 11:28:01.365304 langchain_plantuml-0.0.4/langchain_plantuml/__init__.py
+-rw-r--r--   0        0        0      573 2023-07-19 11:28:01.365304 langchain_plantuml-0.0.4/langchain_plantuml/activity_diagram_beta/__init__.py
+-rw-r--r--   0        0        0     9487 2023-07-19 11:28:01.365304 langchain_plantuml-0.0.4/langchain_plantuml/activity_diagram_beta/plantuml_activity_diagram_beta_callback_handler.py
+-rw-r--r--   0        0        0    13343 2023-07-19 11:28:01.365304 langchain_plantuml-0.0.4/langchain_plantuml/activity_diagram_beta/plantuml_sequence_diagram_callback_handler.py
+-rw-r--r--   0        0        0      573 2023-07-19 11:28:01.365304 langchain_plantuml-0.0.4/langchain_plantuml/core/__init__.py
+-rw-r--r--   0        0        0     2819 2023-07-19 11:28:01.365304 langchain_plantuml-0.0.4/langchain_plantuml/core/plantuml_callback_handler.py
+-rw-r--r--   0        0        0     1255 2023-07-19 11:28:01.365304 langchain_plantuml-0.0.4/langchain_plantuml/diagram.py
+-rw-r--r--   0        0        0     1749 2023-07-19 11:28:01.365304 langchain_plantuml-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4118 1970-01-01 00:00:00.000000 langchain_plantuml-0.0.4/PKG-INFO
```

### Comparing `langchain_plantuml-0.0.3/LICENSE` & `langchain_plantuml-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_plantuml-0.0.3/README.md` & `langchain_plantuml-0.0.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -75,14 +75,20 @@
 
 Sequence Diagram
 
 ```python
 callback_handler = diagram.sequence_diagram_callback()
 ```
 
+Support Custom Note Max Length(default 1000)
+
+```python
+callback_handler = diagram.activity_diagram_callback(note_max_length=2000)
+```
+
 ## Exporting PlantUML to PNG
 
 You can download [plantuml.1.2023.10.jar](https://github.com/plantuml/plantuml/releases/download/v1.2023.10/plantuml-1.2023.10.jar)
 
 ```shell
 java -DPLANTUML_LIMIT_SIZE=81920 -jar plantuml-1.2023.10.jar example-activity.puml
 ```
```

### Comparing `langchain_plantuml-0.0.3/langchain_plantuml/__init__.py` & `langchain_plantuml-0.0.4/langchain_plantuml/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_plantuml-0.0.3/langchain_plantuml/activity_diagram_beta/__init__.py` & `langchain_plantuml-0.0.4/langchain_plantuml/activity_diagram_beta/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_plantuml-0.0.3/langchain_plantuml/activity_diagram_beta/plantuml_activity_diagram_beta_callback_handler.py` & `langchain_plantuml-0.0.4/langchain_plantuml/activity_diagram_beta/plantuml_activity_diagram_beta_callback_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,21 +29,25 @@
 ]
 
 
 class PlantUMLActivityDiagramCallbackHandler(BasePlantUMLCallbackHandler):
     _runs_metrics: dict = {}
 
     def __init__(
-        self, color: Optional[str] = None, skin_param: List[str] = DEFAULT_SKIN_PARAM
+        self,
+        color: Optional[str] = None,
+        skin_param: List[str] = DEFAULT_SKIN_PARAM,
+        note_max_length: int = 1000,
     ) -> None:
         super().__init__()
         for param in skin_param:
             self.uml_content.append(param)
         self.uml_content.append("start")
         self.color = color
+        self.note_max_length = note_max_length
 
     def on_llm_start(
         self, serialized: Dict[str, Any], prompts: List[str], **kwargs: Any
     ) -> None:
         run_metric = self._get_run_object(serialized=serialized, **kwargs)
         activity_name = self._wrapper_activity_name(
             self.on_llm_start.__name__,
```

### Comparing `langchain_plantuml-0.0.3/langchain_plantuml/activity_diagram_beta/plantuml_sequence_diagram_callback_handler.py` & `langchain_plantuml-0.0.4/langchain_plantuml/activity_diagram_beta/plantuml_sequence_diagram_callback_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,23 +30,27 @@
 UML_PARTICIPANTS_FLAG = "-participants-"
 
 
 class PlantUMLSequenceDiagramCallbackHandler(BasePlantUMLCallbackHandler):
     _runs_metrics: dict = {}
 
     def __init__(
-        self, color: Optional[str] = None, skin_param: List[str] = DEFAULT_SKIN_PARAM
+        self,
+        color: Optional[str] = None,
+        skin_param: List[str] = DEFAULT_SKIN_PARAM,
+        note_max_length: int = 1000,
     ) -> None:
         super().__init__()
         for param in skin_param:
             self.uml_content.append(param)
         self.uml_content.append(UML_PARTICIPANTS_FLAG)
         self.participants = {}
         self.participant_name_indexes = []
         self.color = color
+        self.note_max_length = note_max_length
 
     def on_llm_start(
         self, serialized: Dict[str, Any], prompts: List[str], **kwargs: Any
     ) -> None:
         run_metric = self._get_run_object(serialized=serialized, **kwargs)
         activity_name = self._wrapper_sequence_name(
             self.on_llm_start.__name__,
```

### Comparing `langchain_plantuml-0.0.3/langchain_plantuml/core/__init__.py` & `langchain_plantuml-0.0.4/langchain_plantuml/core/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_plantuml-0.0.3/langchain_plantuml/core/plantuml_callback_handler.py` & `langchain_plantuml-0.0.4/langchain_plantuml/core/plantuml_callback_handler.py`

 * *Files identical despite different names*

### Comparing `langchain_plantuml-0.0.3/langchain_plantuml/diagram.py` & `langchain_plantuml-0.0.4/langchain_plantuml/diagram.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,13 +16,13 @@
 
 from langchain_plantuml.activity_diagram_beta.plantuml_activity_diagram_beta_callback_handler import \
     PlantUMLActivityDiagramCallbackHandler
 from langchain_plantuml.activity_diagram_beta.plantuml_sequence_diagram_callback_handler import \
     PlantUMLSequenceDiagramCallbackHandler
 
 
-def activity_diagram_callback() -> BaseCallbackHandler:
-    return PlantUMLActivityDiagramCallbackHandler()
+def activity_diagram_callback(note_max_length: int = 1000) -> BaseCallbackHandler:
+    return PlantUMLActivityDiagramCallbackHandler(note_max_length=note_max_length)
 
 
-def sequence_diagram_callback() -> BaseCallbackHandler:
-    return PlantUMLSequenceDiagramCallbackHandler()
+def sequence_diagram_callback(note_max_length: int = 1000) -> BaseCallbackHandler:
+    return PlantUMLSequenceDiagramCallbackHandler(note_max_length=note_max_length)
```

### Comparing `langchain_plantuml-0.0.3/pyproject.toml` & `langchain_plantuml-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 [build-system]
 requires = ["flit_core==3.9.0"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "langchain-plantuml"
-version = "0.0.3"
+version = "0.0.4"
 description = "Subscribe to events using a callback and store them in PlantUML format. You can easily subscribe to events and keep them in a form that is easy to visualize and analyze."
 authors = [{ name = "Lei Zhang", email = "zhanglei@apache.org" }]
 license = {file = "LICENSE"}
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
     "langchain==0.0.228"
```

### Comparing `langchain_plantuml-0.0.3/PKG-INFO` & `langchain_plantuml-0.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-plantuml
-Version: 0.0.3
+Version: 0.0.4
 Summary: Subscribe to events using a callback and store them in PlantUML format. You can easily subscribe to events and keep them in a form that is easy to visualize and analyze.
 Author-email: Lei Zhang <zhanglei@apache.org>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: langchain==0.0.228
 Requires-Dist: flake8==5.0.4 ; extra == "lint"
 Requires-Dist: pyproject-flake8==5.0.4 ; extra == "lint"
@@ -99,14 +99,20 @@
 
 Sequence Diagram
 
 ```python
 callback_handler = diagram.sequence_diagram_callback()
 ```
 
+Support Custom Note Max Length(default 1000)
+
+```python
+callback_handler = diagram.activity_diagram_callback(note_max_length=2000)
+```
+
 ## Exporting PlantUML to PNG
 
 You can download [plantuml.1.2023.10.jar](https://github.com/plantuml/plantuml/releases/download/v1.2023.10/plantuml-1.2023.10.jar)
 
 ```shell
 java -DPLANTUML_LIMIT_SIZE=81920 -jar plantuml-1.2023.10.jar example-activity.puml
 ```
```

