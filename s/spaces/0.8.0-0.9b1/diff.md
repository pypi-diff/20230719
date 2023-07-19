# Comparing `tmp/spaces-0.8.0.tar.gz` & `tmp/spaces-0.9b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spaces-0.8.0.tar", max compression
+gzip compressed data, was "spaces-0.9b1.tar", max compression
```

## Comparing `spaces-0.8.0.tar` & `spaces-0.9b1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       61 2023-02-23 09:04:36.869652 spaces-0.8.0/README.md
--rw-r--r--   0        0        0     1524 2023-07-12 10:17:10.011073 spaces-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      212 2023-06-30 09:31:31.779698 spaces-0.8.0/spaces/__init__.py
--rw-r--r--   0        0        0      489 2023-06-30 09:32:40.450793 spaces-0.8.0/spaces/config.py
--rw-r--r--   0        0        0      262 2023-06-30 15:54:25.725430 spaces-0.8.0/spaces/gpu/__init__.py
--rw-r--r--   0        0        0     2330 2023-07-12 09:59:29.756084 spaces-0.8.0/spaces/gpu/client.py
--rw-r--r--   0        0        0      883 2023-06-30 15:54:55.853086 spaces-0.8.0/spaces/gpu/decorator.py
--rw-r--r--   0        0        0     3573 2023-07-07 16:29:17.706242 spaces-0.8.0/spaces/gpu/torch.py
--rw-r--r--   0        0        0     7058 2023-07-12 10:03:26.126469 spaces-0.8.0/spaces/gpu/wrappers.py
--rw-r--r--   0        0        0      772 2023-06-30 15:52:15.754907 spaces-0.8.0/spaces/gradio.py
--rw-r--r--   0        0        0     1248 2023-06-30 15:55:09.648928 spaces-0.8.0/spaces/utils.py
--rw-r--r--   0        0        0      836 1970-01-01 00:00:00.000000 spaces-0.8.0/setup.py
--rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 spaces-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0       61 2023-02-23 09:04:36.869652 spaces-0.9b1/README.md
+-rw-r--r--   0        0        0     1524 2023-07-19 11:04:41.709260 spaces-0.9b1/pyproject.toml
+-rw-r--r--   0        0        0      212 2023-06-30 09:31:31.779698 spaces-0.9b1/spaces/__init__.py
+-rw-r--r--   0        0        0      489 2023-06-30 09:32:40.450793 spaces-0.9b1/spaces/config.py
+-rw-r--r--   0        0        0      262 2023-06-30 15:54:25.725430 spaces-0.9b1/spaces/gpu/__init__.py
+-rw-r--r--   0        0        0     2662 2023-07-19 11:04:13.597888 spaces-0.9b1/spaces/gpu/client.py
+-rw-r--r--   0        0        0     1650 2023-07-19 11:04:13.597888 spaces-0.9b1/spaces/gpu/decorator.py
+-rw-r--r--   0        0        0     3573 2023-07-07 16:29:17.706242 spaces-0.9b1/spaces/gpu/torch.py
+-rw-r--r--   0        0        0     7768 2023-07-19 11:04:13.597888 spaces-0.9b1/spaces/gpu/wrappers.py
+-rw-r--r--   0        0        0     1264 2023-07-19 11:04:13.597888 spaces-0.9b1/spaces/gradio.py
+-rw-r--r--   0        0        0     1198 2023-07-19 11:04:13.597888 spaces-0.9b1/spaces/utils.py
+-rw-r--r--   0        0        0      836 1970-01-01 00:00:00.000000 spaces-0.9b1/setup.py
+-rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 spaces-0.9b1/PKG-INFO
```

### Comparing `spaces-0.8.0/pyproject.toml` & `spaces-0.9b1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spaces"
-version = "0.8.0"
+version = "0.9b1"
 description = "Utilities for Hugging Face Spaces"
 authors = ["Charles Bensimon <charles@huggingface.co>"]
 readme = "README.md"
 homepage = "https://huggingface.co"
 repository = "https://github.com/huggingface/huggingface_hub"
 license = "Apache-2.0"
```

### Comparing `spaces-0.8.0/spaces/gpu/client.py` & `spaces-0.9b1/spaces/gpu/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,19 +10,21 @@
 from pydantic import BaseModel
 
 from .. import utils
 from ..config import Config
 
 
 CGROUP_PATH = utils.self_cgroup_device_path()
+TOKEN_HEADER = 'X-IP-Token'
 
 
 class ScheduleParams(BaseModel):
     cgroupPath: str
     taskId: int
+    token: str
 
 class ScheduleResponse(BaseModel):
     idle: bool
     nvidiaIndex: int
     nvidiaUUID: str
 
 class ReleaseParams(BaseModel):
@@ -47,19 +49,26 @@
         time.sleep(1)
         if (retries := retries + 1) > max_retries:
             raise RuntimeError("Error while initializing ZeroGPU: NotFound")
     if status != HTTPStatus.OK: # pragma: no cover
         raise RuntimeError("Error while initializing ZeroGPU: Unknown")
 
 
-def schedule(task_id: int) -> ScheduleResponse:
+def schedule(task_id: int, request: gr.Request) -> ScheduleResponse:
+
+    if not hasattr(request, 'headers') or not hasattr(request.headers, '__dict__'):
+        raise gr.Error("Internal Gradio error")
+
+    if not (token := request.headers.__dict__.get(TOKEN_HEADER)):
+        raise gr.Error("Internal infra error")
 
     res = post('/schedule', params=ScheduleParams(
         cgroupPath=CGROUP_PATH,
         taskId=task_id,
+        token=token,
     ))
 
     if res.status_code == HTTPStatus.TOO_MANY_REQUESTS:
         raise gr.Error("No GPU is currently available")
 
     try:
         data = res.json()
```

### Comparing `spaces-0.8.0/spaces/gpu/torch.py` & `spaces-0.9b1/spaces/gpu/torch.py`

 * *Files identical despite different names*

### Comparing `spaces-0.8.0/spaces/gpu/wrappers.py` & `spaces-0.9b1/spaces/gpu/wrappers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 """
 """
 from __future__ import annotations
 
 import gradio as gr
 import multiprocessing
+import inspect
 import os
 import signal
 import traceback
+import uuid
 from concurrent.futures import ThreadPoolExecutor
 from functools import partial
+from inspect import Parameter
 from pickle import PicklingError
 from threading import Thread
 from typing import TYPE_CHECKING
 from typing import Any
 from typing import Callable
 from typing import Generator
 from typing import Generic
 from typing import TypeVar
+from typing_extensions import Concatenate
 from typing_extensions import ParamSpec
 
 import psutil
 
 from ..utils import drop_params
 from ..utils import SimpleQueue as Queue
 from . import client
@@ -58,30 +62,30 @@
             target=target,
             args=args,
             daemon=True,
         )
         self.process.start()
         self._sentinel.start()
 
-    def _close_on_exit(self): # TODO: differentiate 137 (killed) vs. other return codes (internal errors)
+    def _close_on_exit(self):
         self.process.join()
         self.res_queue.close()
 
 
 def regular_function_wrapper(
     task:
      Callable[Param, Res],
-) -> Callable[Param, Res]:
+) -> Callable[Concatenate[gr.Request, Param], Res]:
 
     workers: dict[NvidiaIndex, Worker[list[Res] | Exception]] = {}
     task_id = id(task)
 
-    def process_wrapper(*args: Param.args, **kwargs: Param.kwargs) -> Res:
+    def gradio_handler(request: gr.Request, /, *args: Param.args, **kwargs: Param.kwargs) -> Res:
 
-        schedule_response = client.schedule(task_id)
+        schedule_response = client.schedule(task_id, request)
         nvidia_index = schedule_response.nvidiaIndex
         nvidia_uuid = schedule_response.nvidiaUUID
         release = partial(client.release, task_id=task_id, nvidia_index=nvidia_index)
 
         worker = workers.get(nvidia_index)
         if worker is None or not worker.process.is_alive():
             worker = Worker(thread_wrapper, nvidia_uuid)
@@ -129,28 +133,30 @@
                 traceback.print_exc()
                 res = e
             try:
                 res_queue.put(res)
             except PicklingError as e:
                 res_queue.put(e)
     
-    return process_wrapper
+    update_handler_meta(gradio_handler, inspect.signature(task))
+
+    return gradio_handler
 
 
 def generator_function_wrapper(
     task:
      Callable[Param, Generator[Res, None, None]],
-) -> Callable[Param, Generator[Res, None, None]]:
+) -> Callable[Concatenate[gr.Request, Param], Generator[Res, None, None]]:
 
     workers: dict[NvidiaIndex, Worker[list[Res] | Exception | None]] = {}
     task_id = id(task)
 
-    def process_wrapper(*args: Param.args, **kwargs: Param.kwargs) -> Generator[Res, None, None]:
+    def gradio_handler(request: gr.Request, /, *args: Param.args, **kwargs: Param.kwargs) -> Generator[Res, None, None]:
 
-        schedule_response = client.schedule(task_id)
+        schedule_response = client.schedule(task_id, request)
         nvidia_index = schedule_response.nvidiaIndex
         nvidia_uuid = schedule_response.nvidiaUUID
         release = partial(client.release, task_id=task_id, nvidia_index=nvidia_index)
 
         worker = workers.get(nvidia_index)
         if worker is None or not worker.process.is_alive():
             worker = Worker(thread_wrapper, nvidia_uuid)
@@ -228,8 +234,18 @@
                         break
                     else:
                         continue
             with ThreadPoolExecutor() as executor:
                 executor.submit(iterate)
             res_queue.put(None)
 
-    return process_wrapper
+    update_handler_meta(gradio_handler, inspect.signature(task))
+
+    return gradio_handler
+
+
+def update_handler_meta(handler: Callable, task_signature: inspect.Signature):
+    param_name = f'request_{uuid.uuid4().hex}'
+    new_param = Parameter(param_name, Parameter.POSITIONAL_ONLY, annotation=gr.Request)
+    new_params = [new_param] + list(task_signature.parameters.values())
+    handler.__signature__ = task_signature.replace(parameters=new_params)
+    handler.__annotations__ = handler.__annotations__ | {param_name: gr.Request}
```

### Comparing `spaces-0.8.0/spaces/utils.py` & `spaces-0.9b1/spaces/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 from pickle import PicklingError
 from typing import Callable
 from typing import TypeVar
 
 
 T = TypeVar('T')
 
-CallableT = TypeVar("CallableT", bound=Callable)
-
 
 def self_cgroup_device_path() -> str:
     cgroup_content = Path('/proc/self/cgroup').read_text()
     for line in cgroup_content.strip().split('\n'):
         contents = line.split(':devices:')
         if len(contents) != 2:
             continue # pragma: no cover
```

### Comparing `spaces-0.8.0/setup.py` & `spaces-0.9b1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
  'psutil>=5.9.5,<6.0.0',
  'pydantic>=1.10.8,<2.0.0',
  'requests>=2.29.0,<3.0.0',
  'typing-extensions>=4.5.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'spaces',
-    'version': '0.8.0',
+    'version': '0.9b1',
     'description': 'Utilities for Hugging Face Spaces',
     'long_description': '# Hugging Face Spaces\n\n## Installation\n\n`pip install spaces`\n',
     'author': 'Charles Bensimon',
     'author_email': 'charles@huggingface.co',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://huggingface.co',
```

### Comparing `spaces-0.8.0/PKG-INFO` & `spaces-0.9b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spaces
-Version: 0.8.0
+Version: 0.9b1
 Summary: Utilities for Hugging Face Spaces
 Home-page: https://huggingface.co
 License: Apache-2.0
 Author: Charles Bensimon
 Author-email: charles@huggingface.co
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

