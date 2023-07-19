# Comparing `tmp/strangeworks_qiskit_runtime-0.1.2.tar.gz` & `tmp/strangeworks_qiskit_runtime-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strangeworks_qiskit_runtime-0.1.2.tar", max compression
+gzip compressed data, was "strangeworks_qiskit_runtime-0.1.3.tar", max compression
```

## Comparing `strangeworks_qiskit_runtime-0.1.2.tar` & `strangeworks_qiskit_runtime-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      204 2023-05-30 10:29:40.207283 strangeworks_qiskit_runtime-0.1.2/README.md
--rw-r--r--   0        0        0      887 2023-05-30 10:29:54.584081 strangeworks_qiskit_runtime-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      389 2023-05-30 10:29:40.211283 strangeworks_qiskit_runtime-0.1.2/strangeworks_qiskit_runtime/__init__.py
--rw-r--r--   0        0        0     4753 2023-05-30 10:29:40.211283 strangeworks_qiskit_runtime-0.1.2/strangeworks_qiskit_runtime/runtime_client.py
--rw-r--r--   0        0        0    10901 2023-05-30 10:29:40.211283 strangeworks_qiskit_runtime-0.1.2/strangeworks_qiskit_runtime/service.py
--rw-r--r--   0        0        0     6805 2023-05-30 10:29:40.211283 strangeworks_qiskit_runtime-0.1.2/strangeworks_qiskit_runtime/sw_runtime_job.py
--rw-r--r--   0        0        0     5515 2023-05-30 10:29:40.211283 strangeworks_qiskit_runtime-0.1.2/strangeworks_qiskit_runtime/swestimator.py
--rw-r--r--   0        0        0     4549 2023-05-30 10:29:40.211283 strangeworks_qiskit_runtime-0.1.2/strangeworks_qiskit_runtime/swsampler.py
--rw-r--r--   0        0        0      708 1970-01-01 00:00:00.000000 strangeworks_qiskit_runtime-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      204 2023-07-19 12:50:43.016410 strangeworks_qiskit_runtime-0.1.3/README.md
+-rw-r--r--   0        0        0      880 2023-07-19 12:50:56.592562 strangeworks_qiskit_runtime-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      389 2023-07-19 12:50:43.020410 strangeworks_qiskit_runtime-0.1.3/strangeworks_qiskit_runtime/__init__.py
+-rw-r--r--   0        0        0     4965 2023-07-19 12:50:43.020410 strangeworks_qiskit_runtime-0.1.3/strangeworks_qiskit_runtime/runtime_client.py
+-rw-r--r--   0        0        0    11935 2023-07-19 12:50:43.020410 strangeworks_qiskit_runtime-0.1.3/strangeworks_qiskit_runtime/service.py
+-rw-r--r--   0        0        0     6805 2023-07-19 12:50:43.020410 strangeworks_qiskit_runtime-0.1.3/strangeworks_qiskit_runtime/sw_runtime_job.py
+-rw-r--r--   0        0        0     5515 2023-07-19 12:50:43.020410 strangeworks_qiskit_runtime-0.1.3/strangeworks_qiskit_runtime/swestimator.py
+-rw-r--r--   0        0        0     4549 2023-07-19 12:50:43.020410 strangeworks_qiskit_runtime-0.1.3/strangeworks_qiskit_runtime/swsampler.py
+-rw-r--r--   0        0        0      694 1970-01-01 00:00:00.000000 strangeworks_qiskit_runtime-0.1.3/PKG-INFO
```

### Comparing `strangeworks_qiskit_runtime-0.1.2/pyproject.toml` & `strangeworks_qiskit_runtime-0.1.3/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "strangeworks-qiskit-runtime"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["Your Name <you@example.com>"]
 readme = "README.md"
 packages = [{include = "strangeworks_qiskit_runtime"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-qiskit-ibm-runtime = "^0.9.2"
-strangeworks = "^0.4.2"
-strangeworks-python-core = "^0.1.7"
+qiskit-ibm-runtime = "0.11.2"
+strangeworks = "^0.4.4"
+strangeworks-core = "^0.2.3"
 
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.2.2"
 black = "^22.10.0"
 pytest = "^7.2.2"
 flake8-pyproject = "^1.2.3"
```

### Comparing `strangeworks_qiskit_runtime-0.1.2/strangeworks_qiskit_runtime/runtime_client.py` & `strangeworks_qiskit_runtime-0.1.3/strangeworks_qiskit_runtime/runtime_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,31 +95,38 @@
         if start_session:
             payload["start_session"] = start_session
             payload["session_time"] = session_time
         data = json.dumps(payload, cls=RuntimeEncoder)
 
         circ_params = params.get("parameter_values")
         if circ_params is None or len(circ_params[0]) == 0:
-            qobj_dict = assemble(params["circuits"][0]).to_dict()
+            qobj_dict = [
+                assemble(params["circuits"][circ]).to_dict()
+                for circ in range(len(params["circuits"]))
+            ]
         else:
-            qobj_dict = assemble(
-                params["circuits"][0]
-                .bind_parameters(circ_params[0])
-                .decompose()
-                .decompose()
-            ).to_dict()
+            qobj_dict = [
+                assemble(
+                    params["circuits"][circ]
+                    .bind_parameters(circ_params[circ])
+                    .decompose()
+                    .decompose()
+                ).to_dict()
+                for circ in range(len(params["circuits"]))
+            ]
 
         payload = {
             "data": data,
             "circuit": qobj_dict,
             "program_id": program_id,
             "backend": backend_name,
             "channel": self._channel,
             "runtime": True,
         }
+
         response = strangeworks.execute(self.rsc, payload, "create_runtime_job")
 
         return response
 
     def job_get(self, job_slug, **kwargs):
         return strangeworks.jobs(slug=job_slug)[0]
```

### Comparing `strangeworks_qiskit_runtime-0.1.2/strangeworks_qiskit_runtime/service.py` & `strangeworks_qiskit_runtime-0.1.3/strangeworks_qiskit_runtime/service.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """Strangeworks Qiskit Runtime Service."""
 import json
 import logging
 from typing import Any, Callable, Dict, List, Optional, Sequence, Type, Union
 
 import strangeworks
 from qiskit.providers.backend import BackendV1 as Backend
+from qiskit_ibm_provider.utils.backend_decoder import configuration_from_server_data
 from qiskit_ibm_runtime import ibm_backend
 from qiskit_ibm_runtime.accounts import ChannelType
 from qiskit_ibm_runtime.api.exceptions import RequestsApiError
 from qiskit_ibm_runtime.exceptions import IBMRuntimeError, RuntimeProgramNotFound
+from qiskit_ibm_runtime.ibm_backend import IBMBackend
 from qiskit_ibm_runtime.program.result_decoder import ResultDecoder
 from qiskit_ibm_runtime.runtime_options import RuntimeOptions
 from qiskit_ibm_runtime.runtime_program import ParameterNamespace
 from strangeworks.core.errors.error import StrangeworksError
 
 from .runtime_client import StrangeworksRuntimeClient
 from .sw_runtime_job import StrangeworksRuntimeJob
@@ -167,14 +169,43 @@
         """Return a list of available backends."""
         if self._channel == "ibm_quantum":
             slug = "ibm-quantum"
         elif self._channel == "ibm_cloud":
             slug = "ibm-cloud"
         return strangeworks.backends(backend_type_slugs=[slug])
 
+    def backend(
+        self,
+        name: str = None,
+        instance: Optional[str] = None,
+    ) -> Backend:
+        """Return a single backend matching the specified filtering."""
+        backends = self.backends()
+        for b in backends:
+            if b.name == name:
+                backend = b
+
+        # To-Do: Need to get backend configuration from service side
+        payload = {
+            "runtime": True,
+            "channel": self.channel,
+            "name": name,
+        }
+        raw_config = strangeworks.execute(self.rsc, payload, "runtime_backend_config")
+        config = configuration_from_server_data(
+            raw_config=raw_config, instance=instance
+        )
+        backend = IBMBackend(
+            configuration=config,
+            service=self,
+            api_client=self._api_client,
+            instance=instance,
+        )
+        return backend
+
     def run(
         self,
         program_id: str,
         inputs: Union[Dict, ParameterNamespace],
         options: Optional[Union[RuntimeOptions, Dict]] = None,
         callback: Optional[Callable] = None,
         result_decoder: Optional[
```

### Comparing `strangeworks_qiskit_runtime-0.1.2/strangeworks_qiskit_runtime/sw_runtime_job.py` & `strangeworks_qiskit_runtime-0.1.3/strangeworks_qiskit_runtime/sw_runtime_job.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qiskit_runtime-0.1.2/strangeworks_qiskit_runtime/swestimator.py` & `strangeworks_qiskit_runtime-0.1.3/strangeworks_qiskit_runtime/swestimator.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qiskit_runtime-0.1.2/strangeworks_qiskit_runtime/swsampler.py` & `strangeworks_qiskit_runtime-0.1.3/strangeworks_qiskit_runtime/swsampler.py`

 * *Files identical despite different names*

