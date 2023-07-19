# Comparing `tmp/aiworkflows-0.0.1.tar.gz` & `tmp/aiworkflows-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiworkflows-0.0.1.tar", last modified: Wed Jul 12 06:20:40 2023, max compression
+gzip compressed data, was "aiworkflows-0.0.2.tar", last modified: Wed Jul 19 06:51:41 2023, max compression
```

## Comparing `aiworkflows-0.0.1.tar` & `aiworkflows-0.0.2.tar`

### file list

```diff
@@ -1,40 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 06:20:40.141084 aiworkflows-0.0.1/
--rw-rw-rw-   0        0        0      303 2023-07-12 06:20:40.141084 aiworkflows-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1073 2023-07-12 05:56:43.000000 aiworkflows-0.0.1/license.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 06:20:40.141084 aiworkflows-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      564 2023-07-12 06:20:38.000000 aiworkflows-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-12 06:20:40.125460 aiworkflows-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-12 06:20:40.125460 aiworkflows-0.0.1/src/aiworkflows/
--rw-rw-rw-   0        0        0        0 2023-07-11 06:32:43.000000 aiworkflows-0.0.1/src/aiworkflows/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 06:20:40.141084 aiworkflows-0.0.1/src/aiworkflows/api/
--rw-rw-rw-   0        0        0        0 2023-07-11 07:23:33.000000 aiworkflows-0.0.1/src/aiworkflows/api/__init__.py
--rw-rw-rw-   0        0        0     1682 2023-07-12 06:05:11.000000 aiworkflows-0.0.1/src/aiworkflows/api/aiworkflows_api.py
--rw-rw-rw-   0        0        0     4849 2023-07-11 09:34:21.000000 aiworkflows-0.0.1/src/aiworkflows/api/tasks.py
-drwxrwxrwx   0        0        0        0 2023-07-12 06:20:40.141084 aiworkflows-0.0.1/src/aiworkflows/api/utils/
--rw-rw-rw-   0        0        0        0 2023-07-11 07:56:04.000000 aiworkflows-0.0.1/src/aiworkflows/api/utils/__init__.py
--rw-rw-rw-   0        0        0     1157 2023-07-12 06:02:07.000000 aiworkflows-0.0.1/src/aiworkflows/api/utils/request_handler.py
-drwxrwxrwx   0        0        0        0 2023-07-12 06:20:40.141084 aiworkflows-0.0.1/src/aiworkflows/compiler/
--rw-rw-rw-   0        0        0        0 2023-07-11 07:23:56.000000 aiworkflows-0.0.1/src/aiworkflows/compiler/__init__.py
--rw-rw-rw-   0        0        0     2597 2023-07-11 09:30:22.000000 aiworkflows-0.0.1/src/aiworkflows/compiler/compiler.py
-drwxrwxrwx   0        0        0        0 2023-07-12 06:20:40.141084 aiworkflows-0.0.1/src/aiworkflows/compiler/utils/
--rw-rw-rw-   0        0        0        0 2023-07-11 07:38:26.000000 aiworkflows-0.0.1/src/aiworkflows/compiler/utils/__init__.py
--rw-rw-rw-   0        0        0     2054 2023-07-11 10:15:29.000000 aiworkflows-0.0.1/src/aiworkflows/compiler/utils/json_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-12 06:20:40.141084 aiworkflows-0.0.1/src/aiworkflows/models/
--rw-rw-rw-   0        0        0        0 2023-07-11 06:38:09.000000 aiworkflows-0.0.1/src/aiworkflows/models/__init__.py
--rw-rw-rw-   0        0        0      137 2023-07-11 06:40:29.000000 aiworkflows-0.0.1/src/aiworkflows/models/ai_model_source.py
--rw-rw-rw-   0        0        0     5348 2023-07-11 10:01:23.000000 aiworkflows-0.0.1/src/aiworkflows/models/ai_task.py
--rw-rw-rw-   0        0        0     3246 2023-07-11 10:01:23.000000 aiworkflows-0.0.1/src/aiworkflows/models/ai_task_call.py
--rw-rw-rw-   0        0        0     1483 2023-07-11 10:01:23.000000 aiworkflows-0.0.1/src/aiworkflows/models/ai_task_call_usage.py
--rw-rw-rw-   0        0        0     1968 2023-07-11 10:01:23.000000 aiworkflows-0.0.1/src/aiworkflows/models/ai_task_configuration.py
--rw-rw-rw-   0        0        0     1279 2023-07-11 10:16:05.000000 aiworkflows-0.0.1/src/aiworkflows/models/ai_task_data_object.py
--rw-rw-rw-   0        0        0      196 2023-07-11 06:43:16.000000 aiworkflows-0.0.1/src/aiworkflows/models/ai_task_error_options.py
--rw-rw-rw-   0        0        0     1856 2023-07-11 10:01:42.000000 aiworkflows-0.0.1/src/aiworkflows/models/ai_task_execution.py
--rw-rw-rw-   0        0        0     1939 2023-07-11 10:01:59.000000 aiworkflows-0.0.1/src/aiworkflows/models/ai_task_input.py
--rw-rw-rw-   0        0        0     1566 2023-07-11 10:02:08.000000 aiworkflows-0.0.1/src/aiworkflows/models/ai_task_output.py
--rw-rw-rw-   0        0        0      695 2023-07-11 07:33:40.000000 aiworkflows-0.0.1/src/aiworkflows/models/ai_task_primitive_type.py
-drwxrwxrwx   0        0        0        0 2023-07-12 06:20:40.141084 aiworkflows-0.0.1/src/aiworkflows.egg-info/
--rw-rw-rw-   0        0        0      303 2023-07-12 06:20:40.000000 aiworkflows-0.0.1/src/aiworkflows.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1098 2023-07-12 06:20:40.000000 aiworkflows-0.0.1/src/aiworkflows.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 06:20:40.000000 aiworkflows-0.0.1/src/aiworkflows.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-12 06:20:40.000000 aiworkflows-0.0.1/src/aiworkflows.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-12 06:20:40.000000 aiworkflows-0.0.1/src/aiworkflows.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-19 06:51:41.823478 aiworkflows-0.0.2/
+-rw-rw-rw-   0        0        0      351 2023-07-19 06:51:41.823478 aiworkflows-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1073 2023-07-12 07:13:34.000000 aiworkflows-0.0.2/license.txt
+-rw-rw-rw-   0        0        0       42 2023-07-19 06:51:41.823478 aiworkflows-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      758 2023-07-19 06:51:36.000000 aiworkflows-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 06:51:41.792089 aiworkflows-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-19 06:51:41.792089 aiworkflows-0.0.2/src/aiworkflows/
+-rw-rw-rw-   0        0        0      109 2023-07-19 06:51:36.000000 aiworkflows-0.0.2/src/aiworkflows/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 06:51:41.814802 aiworkflows-0.0.2/src/aiworkflows/api/
+-rw-rw-rw-   0        0        0       87 2023-07-19 06:51:36.000000 aiworkflows-0.0.2/src/aiworkflows/api/__init__.py
+-rw-rw-rw-   0        0        0     3976 2023-07-19 06:51:36.000000 aiworkflows-0.0.2/src/aiworkflows/api/api.py
+-rw-rw-rw-   0        0        0     4849 2023-07-19 06:35:38.000000 aiworkflows-0.0.2/src/aiworkflows/api/tasks.py
+drwxrwxrwx   0        0        0        0 2023-07-19 06:51:41.815849 aiworkflows-0.0.2/src/aiworkflows/api/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-12 07:13:34.000000 aiworkflows-0.0.2/src/aiworkflows/api/utils/__init__.py
+-rw-rw-rw-   0        0        0     1157 2023-07-12 07:13:34.000000 aiworkflows-0.0.2/src/aiworkflows/api/utils/request_handler.py
+-rw-rw-rw-   0        0        0     3040 2023-07-19 06:51:36.000000 aiworkflows-0.0.2/src/aiworkflows/cli.py
+drwxrwxrwx   0        0        0        0 2023-07-19 06:51:41.816888 aiworkflows-0.0.2/src/aiworkflows/compiler/
+-rw-rw-rw-   0        0        0        0 2023-07-12 07:13:34.000000 aiworkflows-0.0.2/src/aiworkflows/compiler/__init__.py
+-rw-rw-rw-   0        0        0     2589 2023-07-19 06:51:36.000000 aiworkflows-0.0.2/src/aiworkflows/compiler/task_compiler.py
+drwxrwxrwx   0        0        0        0 2023-07-19 06:51:41.817920 aiworkflows-0.0.2/src/aiworkflows/compiler/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-12 07:13:34.000000 aiworkflows-0.0.2/src/aiworkflows/compiler/utils/__init__.py
+-rw-rw-rw-   0        0        0     2054 2023-07-12 07:13:34.000000 aiworkflows-0.0.2/src/aiworkflows/compiler/utils/json_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-19 06:51:41.823478 aiworkflows-0.0.2/src/aiworkflows/models/
+-rw-rw-rw-   0        0        0      707 2023-07-19 06:51:36.000000 aiworkflows-0.0.2/src/aiworkflows/models/__init__.py
+-rw-rw-rw-   0        0        0      137 2023-07-12 07:13:34.000000 aiworkflows-0.0.2/src/aiworkflows/models/ai_model_source.py
+-rw-rw-rw-   0        0        0     6554 2023-07-19 06:51:36.000000 aiworkflows-0.0.2/src/aiworkflows/models/ai_task.py
+-rw-rw-rw-   0        0        0     4136 2023-07-19 06:51:36.000000 aiworkflows-0.0.2/src/aiworkflows/models/ai_task_call.py
+-rw-rw-rw-   0        0        0     2127 2023-07-19 06:51:36.000000 aiworkflows-0.0.2/src/aiworkflows/models/ai_task_call_usage.py
+-rw-rw-rw-   0        0        0     2639 2023-07-19 06:51:36.000000 aiworkflows-0.0.2/src/aiworkflows/models/ai_task_configuration.py
+-rw-rw-rw-   0        0        0     1887 2023-07-19 06:51:36.000000 aiworkflows-0.0.2/src/aiworkflows/models/ai_task_data_object.py
+-rw-rw-rw-   0        0        0      196 2023-07-12 07:13:34.000000 aiworkflows-0.0.2/src/aiworkflows/models/ai_task_error_options.py
+-rw-rw-rw-   0        0        0     2543 2023-07-19 06:51:36.000000 aiworkflows-0.0.2/src/aiworkflows/models/ai_task_execution.py
+-rw-rw-rw-   0        0        0     2662 2023-07-19 06:51:36.000000 aiworkflows-0.0.2/src/aiworkflows/models/ai_task_input.py
+-rw-rw-rw-   0        0        0     2214 2023-07-19 06:51:36.000000 aiworkflows-0.0.2/src/aiworkflows/models/ai_task_output.py
+-rw-rw-rw-   0        0        0      945 2023-07-19 06:51:36.000000 aiworkflows-0.0.2/src/aiworkflows/models/ai_task_primitive_type.py
+drwxrwxrwx   0        0        0        0 2023-07-19 06:51:41.813142 aiworkflows-0.0.2/src/aiworkflows.egg-info/
+-rw-rw-rw-   0        0        0      351 2023-07-19 06:51:41.000000 aiworkflows-0.0.2/src/aiworkflows.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1156 2023-07-19 06:51:41.000000 aiworkflows-0.0.2/src/aiworkflows.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 06:51:41.000000 aiworkflows-0.0.2/src/aiworkflows.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-07-19 06:51:41.000000 aiworkflows-0.0.2/src/aiworkflows.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       23 2023-07-19 06:51:41.000000 aiworkflows-0.0.2/src/aiworkflows.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-19 06:51:41.000000 aiworkflows-0.0.2/src/aiworkflows.egg-info/top_level.txt
```

### Comparing `aiworkflows-0.0.1/license.txt` & `aiworkflows-0.0.2/license.txt`

 * *Files identical despite different names*

### Comparing `aiworkflows-0.0.1/setup.py` & `aiworkflows-0.0.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 from setuptools import setup, find_packages
 
 setup(
     name='aiworkflows',
-    version='0.0.1',
+    version='0.0.2',
+    url='https://github.com/ai-workflows/sdk',
     description='AI Workflows Python SDK',
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Joseph Vitko',
     author_email='me@josephvitko.com',
     license='MIT',
     install_requires=[
         'requests',
+        'python-dotenv',
     ],
     python_requires='>=3.10',
     classifiers=[
         'Development Status :: 1 - Planning',
-    ]
+    ],
+    entry_points={
+        "console_scripts": [
+            "aiworkflows=aiworkflows.cli:main",
+        ],
+    },
 )
```

### Comparing `aiworkflows-0.0.1/src/aiworkflows/api/tasks.py` & `aiworkflows-0.0.2/src/aiworkflows/api/tasks.py`

 * *Files identical despite different names*

### Comparing `aiworkflows-0.0.1/src/aiworkflows/api/utils/request_handler.py` & `aiworkflows-0.0.2/src/aiworkflows/api/utils/request_handler.py`

 * *Files identical despite different names*

### Comparing `aiworkflows-0.0.1/src/aiworkflows/compiler/compiler.py` & `aiworkflows-0.0.2/src/aiworkflows/compiler/task_compiler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import os
 
-from aiworkflows.api.aiworkflows_api import AiWorkflowsApi
+from aiworkflows.api.api import AiWorkflowsApi
 from aiworkflows.models.ai_task import AiTask
 
 
-class Compiler:
+class TaskCompiler:
     def __init__(self, api: AiWorkflowsApi):
         self.api: AiWorkflowsApi = api
 
     def deploy_json_tasks_from_directory(self, directory_path: str, recursive: bool = False) -> list[AiTask]:
         """
         Deploys all json tasks from a directory.
         :param directory_path:
```

### Comparing `aiworkflows-0.0.1/src/aiworkflows/compiler/utils/json_utils.py` & `aiworkflows-0.0.2/src/aiworkflows/compiler/utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `aiworkflows-0.0.1/src/aiworkflows/models/ai_task.py` & `aiworkflows-0.0.2/src/aiworkflows/models/ai_task.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,47 +1,76 @@
 from aiworkflows.compiler.utils.json_utils import parse_required_field, parse_optional_field
 from aiworkflows.models.ai_task_configuration import AiTaskConfiguration
+from aiworkflows.models.ai_task_execution import AiTaskExecution
 from aiworkflows.models.ai_task_input import AiTaskInput
 from aiworkflows.models.ai_task_output import AiTaskOutput
 from aiworkflows.models.ai_task_primitive_type import get_mapped_type
 
 
 class AiTask:
+    """
+    Represents a task in the AI Workflows system.
+    """
+
     def __init__(self,
                  task_ref: str,
                  configuration: AiTaskConfiguration,
                  prompt: str,
                  output: AiTaskOutput,
                  inputs: list[AiTaskInput] = None,
                  name: str = None,
                  description: str = None,
                  task_id: str = None,
                  tenant_id: str = None,
                  ):
+        """
+        Initializes a new instance of the AiTask class.
+
+        :param task_ref: The reference to the task.
+        :param configuration: The configuration of the task.
+        :param prompt: The prompt for the task.
+        :param output: The output of the task.
+        :param inputs: The inputs of the task.
+        :param name: The name of the task.
+        :param description: The description of the task.
+        :param task_id: The ID of the task.
+        :param tenant_id: The ID of the tenant.
+        """
         self.task_ref: str = task_ref
         self.configuration: AiTaskConfiguration = configuration
         self.prompt: str = prompt
         self.output: AiTaskOutput = output
         self.inputs: list[AiTaskInput] = inputs
         self.name: str = name
         self.description: str = description
         self.task_id: str = task_id
         self.tenant_id: str = tenant_id
 
         self._api: "AiWorkflowsApi" = None
 
     def bind_api(self, api: "AiWorkflowsApi"):
+        """
+        Binds the API to the task so that it can be used to execute the task.
+        """
         self._api = api
 
     @property
     def api(self) -> "AiWorkflowsApi":
+        """
+        The API that is bound to the task.
+        """
         return self._api
 
     @staticmethod
-    def from_json(json: dict):
+    def from_json(json: dict) -> "AiTask":
+        """
+        Creates an AiTask from a JSON object.
+
+        :param json: The JSON object.
+        """
         task_ref = parse_required_field(json, 'taskRef', str)
         configuration = parse_required_field(json, 'configuration', AiTaskConfiguration)
         prompt = parse_required_field(json, 'prompt', str)
         output = parse_required_field(json, 'output', AiTaskOutput)
         name = parse_optional_field(json, 'name', str)
         description = parse_optional_field(json, 'description', str)
         task_id = parse_optional_field(json, 'id', str)
@@ -57,28 +86,34 @@
                       output=output,
                       inputs=inputs,
                       name=name,
                       description=description,
                       task_id=task_id,
                       tenant_id=tenant_id)
 
-    def to_json(self):
+    def to_json(self) -> dict:
+        """
+        Converts the AiTask to a JSON object.
+        """
         return {
             'taskRef': self.task_ref,
             'configuration': self.configuration.to_json(),
             'prompt': self.prompt,
             'output': self.output.to_json(),
             'inputs': [i.to_json() for i in self.inputs] if self.inputs else None,
             'name': self.name,
             'description': self.description,
             'id': self.task_id,
             'tenantId': self.tenant_id,
         }
 
-    def __call__(self, *args, **kwargs):
+    def __call__(self, *args, **kwargs) -> AiTaskExecution:
+        """
+        Executes the task.
+        """
         if self.api is None:
             raise RuntimeError('Error running task: API not bound')
 
         inputs: dict = {}
         if self.inputs is not None:
             # bind all args in sequential order to inputs and kwargs to specific inputs
             if (len(args) + len(kwargs)) > len(self.inputs):
@@ -110,15 +145,18 @@
             # make sure all required inputs are present
             for input_schema in self.inputs:
                 if input_schema.is_required and input_schema.input_ref not in inputs:
                     raise RuntimeError(f'Error running task: missing required input {input_schema.input_ref}')
 
         return self.api.run_task(task_ref=self.task_ref, inputs=inputs)
 
-    def run(self, *args, **kwargs):
+    def run(self, *args, **kwargs) -> AiTaskExecution:
+        """
+        Executes the task.
+        """
         return self.__call__(*args, **kwargs)
 
     def __repr__(self):
         return f'AiTask(tenant_id={self.tenant_id}, id={self.task_id}, task_ref={self.task_ref}, ' \
                f'name={self.name}, description={self.description})'
 
     def __str__(self):
```

### Comparing `aiworkflows-0.0.1/src/aiworkflows/models/ai_task_call.py` & `aiworkflows-0.0.2/src/aiworkflows/models/ai_task_call.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,59 @@
 from aiworkflows.compiler.utils.json_utils import parse_optional_field
 from aiworkflows.models.ai_model_source import AiModelSource
 from aiworkflows.models.ai_task_call_usage import AiTaskCallUsage
 from aiworkflows.models.ai_task_data_object import AiTaskDataObject
 
 
 class AiTaskCall:
+    """
+    Represents a call to an AI task.
+    """
+
     def __init__(self,
                  inputs: dict = None,
                  output: AiTaskDataObject = None,
                  model_id: str = None,
                  response_model_id: str = None,
                  model_source: AiModelSource = None,
                  success: bool = None,
                  timestamp: int = None,
                  task_id: str = None,
                  usage: AiTaskCallUsage = None,
                  ):
+        """
+        Initializes a new instance of the AiTaskCall class.
+
+        :param inputs: The inputs of the task call.
+        :param output: The output of the task call.
+        :param model_id: The ID of the model.
+        :param response_model_id: The ID of the response model.
+        :param model_source: The source of the model.
+        :param success: Whether the task call was successful.
+        :param timestamp: The timestamp of the task call.
+        :param task_id: The ID of the task.
+        :param usage: The usage of the task call.
+        """
         self.inputs: dict = inputs
         self.output: AiTaskDataObject = output
         self.model_id: str = model_id
         self.response_model_id: str = response_model_id
         self.model_source: AiModelSource = model_source
         self.success: bool = success
         self.timestamp: int = timestamp
         self.task_id: str = task_id
         self.usage: AiTaskCallUsage = usage
 
     @staticmethod
-    def from_json(json: dict):
+    def from_json(json: dict) -> 'AiTaskCall':
+        """
+        Creates a new instance of the AiTaskCall class from a JSON object.
+
+        :param json: The JSON object.
+        """
         inputs = parse_optional_field(json, 'inputs', dict)
         output = parse_optional_field(json, 'output', AiTaskDataObject)
         model_id = parse_optional_field(json, 'model', str)
         response_model_id = parse_optional_field(json, 'responseModel', str)
         model_source = parse_optional_field(json, 'modelSource', AiModelSource)
         success = parse_optional_field(json, 'success', bool)
         timestamp = parse_optional_field(json, 'timestamp', int)
@@ -44,15 +66,18 @@
                           response_model_id=response_model_id,
                           model_source=model_source,
                           success=success,
                           timestamp=timestamp,
                           task_id=task_id,
                           usage=usage)
 
-    def to_json(self):
+    def to_json(self) -> dict:
+        """
+        Creates a JSON object from the AiTaskCall object.
+        """
         return {
             'inputs': self.inputs,
             'output': self.output,
             'model': self.model_id,
             'responseModel': self.response_model_id,
             'modelSource': self.model_source,
             'success': self.success,
```

### Comparing `aiworkflows-0.0.1/src/aiworkflows/models/ai_task_primitive_type.py` & `aiworkflows-0.0.2/src/aiworkflows/models/ai_task_primitive_type.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 from enum import Enum
 
 
 class AiTaskPrimitiveType(Enum):
+    """
+    Enum for the primitive types of AI task data objects.
+    """
     String = "String"
     Integer = "Integer"
     Float = "Float"
     Boolean = "Boolean"
     Dictionary = "Dictionary"
     List = "List"
 
 
+# map from AiTaskPrimitiveType to Python type
 _type_map: dict[AiTaskPrimitiveType, type] = {
     AiTaskPrimitiveType.String: str,
     AiTaskPrimitiveType.Integer: int,
     AiTaskPrimitiveType.Float: float,
+    AiTaskPrimitiveType.Boolean: bool,
     AiTaskPrimitiveType.Dictionary: dict,
     AiTaskPrimitiveType.List: list
 }
 
 
 def get_mapped_type(obj_type: AiTaskPrimitiveType):
+    """
+    Gets the mapped Python type for the given AiTaskPrimitiveType.
+    """
     if obj_type not in _type_map:
         raise ValueError(f"Error getting mapped type: AiTaskPrimitiveType {obj_type.value} has no type mapping")
 
     return _type_map[obj_type]
```

### Comparing `aiworkflows-0.0.1/src/aiworkflows.egg-info/SOURCES.txt` & `aiworkflows-0.0.2/src/aiworkflows.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 license.txt
 setup.py
 src/aiworkflows/__init__.py
+src/aiworkflows/cli.py
 src/aiworkflows.egg-info/PKG-INFO
 src/aiworkflows.egg-info/SOURCES.txt
 src/aiworkflows.egg-info/dependency_links.txt
+src/aiworkflows.egg-info/entry_points.txt
 src/aiworkflows.egg-info/requires.txt
 src/aiworkflows.egg-info/top_level.txt
 src/aiworkflows/api/__init__.py
-src/aiworkflows/api/aiworkflows_api.py
+src/aiworkflows/api/api.py
 src/aiworkflows/api/tasks.py
 src/aiworkflows/api/utils/__init__.py
 src/aiworkflows/api/utils/request_handler.py
 src/aiworkflows/compiler/__init__.py
-src/aiworkflows/compiler/compiler.py
+src/aiworkflows/compiler/task_compiler.py
 src/aiworkflows/compiler/utils/__init__.py
 src/aiworkflows/compiler/utils/json_utils.py
 src/aiworkflows/models/__init__.py
 src/aiworkflows/models/ai_model_source.py
 src/aiworkflows/models/ai_task.py
 src/aiworkflows/models/ai_task_call.py
 src/aiworkflows/models/ai_task_call_usage.py
```

