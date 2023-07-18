# Comparing `tmp/together-0.0.7.tar.gz` & `tmp/together-0.0.8.tar.gz`

## Comparing `together-0.0.7.tar` & `together-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,25 @@
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 together-0.0.7/.github/workflows/check_code_quality.yml
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 together-0.0.7/src/together/__init__.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 together-0.0.7/src/together/api.py
--rw-r--r--   0        0        0     8689 2020-02-02 00:00:00.000000 together-0.0.7/src/together/files.py
--rw-r--r--   0        0        0    10069 2020-02-02 00:00:00.000000 together-0.0.7/src/together/finetune.py
--rw-r--r--   0        0        0     3897 2020-02-02 00:00:00.000000 together-0.0.7/src/together/inference.py
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 together-0.0.7/src/together/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 together-0.0.7/src/together/cli/__init__.py
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 together-0.0.7/src/together/cli/cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 together-0.0.7/src/together/commands/__init__.py
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 together-0.0.7/src/together/commands/api.py
--rw-r--r--   0        0        0     3833 2020-02-02 00:00:00.000000 together-0.0.7/src/together/commands/files.py
--rw-r--r--   0        0        0    10688 2020-02-02 00:00:00.000000 together-0.0.7/src/together/commands/finetune.py
--rw-r--r--   0        0        0     6609 2020-02-02 00:00:00.000000 together-0.0.7/src/together/commands/inference.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 together-0.0.7/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 together-0.0.7/LICENSE
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 together-0.0.7/README.md
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 together-0.0.7/pyproject.toml
--rw-r--r--   0        0        0    14342 2020-02-02 00:00:00.000000 together-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 together-0.0.8/.DS_Store
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 together-0.0.8/.github/workflows/check_code_quality.yml
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 together-0.0.8/src/.DS_Store
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 together-0.0.8/src/together/.DS_Store
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 together-0.0.8/src/together/__init__.py
+-rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 together-0.0.8/src/together/api.py
+-rw-r--r--   0        0        0     8695 2020-02-02 00:00:00.000000 together-0.0.8/src/together/files.py
+-rw-r--r--   0        0        0    10075 2020-02-02 00:00:00.000000 together-0.0.8/src/together/finetune.py
+-rw-r--r--   0        0        0     5876 2020-02-02 00:00:00.000000 together-0.0.8/src/together/inference.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 together-0.0.8/src/together/cli/__init__.py
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 together-0.0.8/src/together/cli/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 together-0.0.8/src/together/commands/__init__.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 together-0.0.8/src/together/commands/api.py
+-rw-r--r--   0        0        0     4628 2020-02-02 00:00:00.000000 together-0.0.8/src/together/commands/chat.py
+-rw-r--r--   0        0        0     3833 2020-02-02 00:00:00.000000 together-0.0.8/src/together/commands/files.py
+-rw-r--r--   0        0        0    10688 2020-02-02 00:00:00.000000 together-0.0.8/src/together/commands/finetune.py
+-rw-r--r--   0        0        0     7057 2020-02-02 00:00:00.000000 together-0.0.8/src/together/commands/inference.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 together-0.0.8/src/together/utils/__init__.py
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 together-0.0.8/src/together/utils/conversation.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 together-0.0.8/src/together/utils/utils.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 together-0.0.8/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 together-0.0.8/LICENSE
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 together-0.0.8/README.md
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 together-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0    14397 2020-02-02 00:00:00.000000 together-0.0.8/PKG-INFO
```

### Comparing `together-0.0.7/.github/workflows/check_code_quality.yml` & `together-0.0.8/.github/workflows/check_code_quality.yml`

 * *Files identical despite different names*

### Comparing `together-0.0.7/src/together/api.py` & `together-0.0.8/src/together/api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import os
-from typing import Any, Dict, List, Optional, cast
+import urllib.parse
+from typing import Any, List, Optional
 
 import requests
 
 from together.files import Files
 from together.finetune import Finetune
 from together.inference import Inference
-from together.utils import exit_1, get_logger
+from together.utils.utils import exit_1, get_logger
 
 
 DEFAULT_ENDPOINT = "https://api.together.xyz/"
 DEFAULT_SUPPLY_ENDPOINT = "https://computer.together.xyz"
 
 
 class API:
@@ -35,52 +36,37 @@
 
         if supply_endpoint_url is None:
             supply_endpoint_url = DEFAULT_SUPPLY_ENDPOINT
 
         self.endpoint_url = endpoint_url
         self.supply_endpoint_url = supply_endpoint_url
 
-    def get_supply(self) -> Dict[str, Any]:
+    def get_models(self) -> List[Any]:
+        model_url = urllib.parse.urljoin(self.endpoint_url, "models/info?=")
+        headers = {
+            "Authorization": f"Bearer {self.together_api_key}",
+        }
         try:
             response = requests.get(
-                self.supply_endpoint_url,
-                json={
-                    "method": "together_getDepth",
-                    "id": 1,
-                },
+                model_url,
+                headers=headers,
             )
         except requests.exceptions.RequestException as e:
             self.logger.critical(f"Response error raised: {e}")
             exit_1(self.logger)
 
         try:
-            response_json = dict(response.json())
+            response_list = list(response.json())
         except Exception as e:
             self.logger.critical(
                 f"JSON Error raised: {e}\nResponse status code = {response.status_code}"
             )
             exit_1(self.logger)
 
-        return response_json
-
-    def get_all_models(self) -> List[str]:
-        models = cast(List[str], self.get_supply()["result"].keys())
-
-        models = [str(sub[:-1]) for sub in models]  # remove the ? after the model names
-
-        return models
-
-    def get_available_models(self) -> List[str]:
-        res = self.get_supply()
-        names = res["result"].keys()
-        available_models = [
-            name[:-1] for name in names if res["result"][name]["num_asks"] > 0
-        ]
-
-        return available_models
+        return response_list
 
     def finetune(self) -> Finetune:
         return Finetune(
             endpoint_url=self.endpoint_url,
         )
 
     def complete(self, **model_kwargs: Any) -> Inference:
```

### Comparing `together-0.0.7/src/together/files.py` & `together-0.0.8/src/together/files.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from logging import Logger
 from typing import Dict, List, Optional, Union
 
 import requests
 from tqdm import tqdm
 from tqdm.utils import CallbackIOWrapper
 
-from together.utils import exit_1, get_logger
+from together.utils.utils import exit_1, get_logger
 
 
 DEFAULT_ENDPOINT = "https://api.together.xyz/"
 
 
 class JSONException(Exception):
     pass
```

### Comparing `together-0.0.7/src/together/finetune.py` & `together-0.0.8/src/together/finetune.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import posixpath
 import urllib.parse
 from typing import Any, Dict, List, Optional, Union
 
 import requests
 from tqdm import tqdm
 
-from together.utils import exit_1, get_logger
+from together.utils.utils import exit_1, get_logger
 
 
 DEFAULT_ENDPOINT = "https://api.together.xyz/"
 
 
 class Finetune:
     def __init__(
```

### Comparing `together-0.0.7/src/together/utils.py` & `together-0.0.8/src/together/utils/utils.py`

 * *Files identical despite different names*

### Comparing `together-0.0.7/src/together/cli/cli.py` & `together-0.0.8/src/together/cli/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #! python
 import argparse
 
-from together.commands import api, files, finetune, inference
-from together.utils import exit_1, get_logger
+from together.commands import api, chat, files, finetune, inference
+from together.utils.utils import get_logger
 
 
 def main() -> None:
     parser = argparse.ArgumentParser(
         description="CLI client for Together API",
         prog="together",
     )
@@ -32,28 +32,29 @@
 
     subparser = parser.add_subparsers(dest="base")
 
     api.add_parser(subparser, parents=[base_subparser])
     inference.add_parser(subparser, parents=[base_subparser])
     finetune.add_parser(subparser, parents=[base_subparser])
     files.add_parser(subparser, parents=[base_subparser])
+    chat.add_parser(subparser, parents=[base_subparser])
 
     args = parser.parse_args()
 
     # Setup logging
     try:
-        logger = get_logger(__name__, log_level=args.log)
+        get_logger(__name__, log_level=args.log)
     except Exception:
-        logger = get_logger(__name__, log_level="WARNING")
+        get_logger(__name__, log_level="WARNING")
 
-    try:
-        args.func(args)
-    except AttributeError as e:
-        # print error, but ignore if `together` is run.
-        if str(e) != "'Namespace' object has no attribute 'func'":
-            logger.critical(f"Error raised: {e}")
-            exit_1(logger)
-        parser.print_help()
+    # try:
+    args.func(args)
+    # except AttributeError as e:
+    #    # print error, but ignore if `together` is run.
+    ##    if str(e) != "'Namespace' object has no attribute 'func'":
+    #        logger.critical(f"Error raised: {e}")
+    #        exit_1(logger)
+    #    parser.print_help()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `together-0.0.7/src/together/commands/api.py` & `together-0.0.8/src/together/commands/api.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,48 +13,33 @@
 ) -> None:
     COMMAND_NAME = "api"
     parser = subparsers.add_parser(COMMAND_NAME)
 
     child_parsers = parser.add_subparsers(required=True)
 
     _add_list(child_parsers, parents=parents)
-    _add_raw(child_parsers, parents=parents)
 
 
 def _add_list(
     parser: argparse._SubParsersAction[argparse.ArgumentParser],
     parents: List[argparse.ArgumentParser],
 ) -> None:
     list_model_subparser = parser.add_parser("list", parents=parents)
     list_model_subparser.add_argument(
-        "--all",
-        "-a",
-        help="List all models (available and unavailable)",
+        "--raw",
+        help="Raw details of all models",
         default=False,
         action="store_true",
     )
     list_model_subparser.set_defaults(func=_run_list)
 
 
-def _add_raw(
-    parser: argparse._SubParsersAction[argparse.ArgumentParser],
-    parents: List[argparse.ArgumentParser],
-) -> None:
-    list_parser = parser.add_parser("raw-supply", parents=parents)
-    list_parser.set_defaults(func=_run_raw)
-
-
 def _run_list(args: argparse.Namespace) -> None:
     api = API(endpoint_url=args.endpoint, log_level=args.log)
-
-    if args.all:
-        response = api.get_all_models()
+    response = api.get_models()
+    if args.raw:
+        print(json.dumps(response, indent=4))
     else:
-        response = api.get_available_models()
-
-    print(json.dumps(response, indent=4))
-
-
-def _run_raw(args: argparse.Namespace) -> None:
-    api = API(endpoint_url=args.endpoint, log_level=args.log)
-    response = api.get_supply()
-    print(json.dumps(response, indent=4))
+        models = []
+        for i in response:
+            models.append(i["name"])
+        print(json.dumps(models, indent=4))
```

### Comparing `together-0.0.7/src/together/commands/files.py` & `together-0.0.8/src/together/commands/files.py`

 * *Files identical despite different names*

### Comparing `together-0.0.7/src/together/commands/finetune.py` & `together-0.0.8/src/together/commands/finetune.py`

 * *Files identical despite different names*

### Comparing `together-0.0.7/src/together/commands/inference.py` & `together-0.0.8/src/together/commands/inference.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from __future__ import annotations
 
 import argparse
 import base64
 import json
+import logging
 import re
 import sys
-from typing import List
+from typing import Any, Dict, List
 
 from together.inference import Inference
-from together.utils import exit_1, get_logger
+from together.utils.utils import exit_1, get_logger
 
 
 def add_parser(
     subparsers: argparse._SubParsersAction[argparse.ArgumentParser],
     parents: List[argparse.ArgumentParser],
 ) -> None:
     COMMAND_NAME = "complete"
@@ -38,14 +39,21 @@
         "--task",
         default="text2text",
         type=str,
         help="Task type: text2text, text2img. Default=text2text",
         choices=["text2text", "text2img"],
     )
 
+    inf_parser.add_argument(
+        "--no-stream",
+        default=False,
+        action="store_true",
+        help="Indicates wether to disable streaming",
+    )
+
     text2textargs = inf_parser.add_argument_group("Text2Text Arguments")
 
     text2textargs.add_argument(
         "--max-tokens",
         default=128,
         type=int,
         help="Maximum number of tokens to generate. Default=128",
@@ -140,37 +148,17 @@
 
 
 def _enforce_stop_tokens(text: str, stop: List[str]) -> str:
     """Cut off the text as soon as any stop words occur."""
     return re.split("|".join(stop), text)[0]
 
 
-def _run_complete(args: argparse.Namespace) -> None:
-    logger = get_logger(__name__, log_level=args.log)
-
-    inference = Inference(
-        endpoint_url=args.endpoint,
-        task=args.task,
-        model=args.model,
-        max_tokens=args.max_tokens,
-        stop=args.stop,
-        temperature=args.temperature,
-        top_p=args.top_p,
-        top_k=args.top_k,
-        repetition_penalty=args.repetition_penalty,
-        logprobs=args.logprobs,
-        steps=args.steps,
-        seed=args.seed,
-        results=args.results,
-        height=args.height,
-        width=args.width,
-    )
-
-    response = inference.inference(prompt=args.prompt)
-
+def no_streamer(
+    args: argparse.Namespace, response: Dict[str, Any], logger: logging.Logger
+) -> None:
     if args.raw:
         print(json.dumps(response, indent=4))
         sys.exit()
 
     if "output" in response.keys():
         if args.task == "text2text":
             try:
@@ -214,7 +202,35 @@
             logger.critical(f"Error raised: {response['error']}")
 
     else:
         logger.critical("Unknown response received")
         exit_1(logger)
 
     print(text.strip())
+
+
+def _run_complete(args: argparse.Namespace) -> None:
+    logger = get_logger(__name__, log_level=args.log)
+
+    inference = Inference(
+        endpoint_url=args.endpoint,
+        task=args.task,
+        model=args.model,
+        max_tokens=args.max_tokens,
+        stop=args.stop,
+        temperature=args.temperature,
+        top_p=args.top_p,
+        top_k=args.top_k,
+        repetition_penalty=args.repetition_penalty,
+        logprobs=args.logprobs,
+        steps=args.steps,
+        seed=args.seed,
+        results=args.results,
+        height=args.height,
+        width=args.width,
+    )
+
+    if args.no_stream:
+        response = inference.inference(prompt=args.prompt)
+        no_streamer(args, response, logger)
+    else:
+        _ = inference.streaming_inference(prompt=args.prompt)
```

### Comparing `together-0.0.7/.gitignore` & `together-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `together-0.0.7/LICENSE` & `together-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `together-0.0.7/pyproject.toml` & `together-0.0.8/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "together"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Together Computer", email="community@together.xyz" },
 ]
 description = "Python client for Together's Cloud Platform!"
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.6"
@@ -21,15 +21,15 @@
 dependencies = [
     "typer",
     "requests",
     "tqdm"
 ]
 
 [project.optional-dependencies]
-quality = ["black~=23.1", "ruff>=0.0.241,<=0.0.259", "mypy>=1.3.0", "types-requests>=2.31.0.1", "types-tqdm>=4.65.0.0"]
+quality = ["black~=23.1", "ruff>=0.0.241,<=0.0.259", "mypy>=1.3.0", "types-requests>=2.31.0.1", "types-tqdm>=4.65.0.0", "sseclient-py>=1.7.0"]
 
 [project.urls]
 "Homepage" = "https://github.com/togethercomputer/together"
 "Bug Tracker" = "https://github.com/togethercomputer/together/issues"
 
 [project.scripts]
 together = "together.cli.cli:main"
```

### Comparing `together-0.0.7/PKG-INFO` & `together-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: together
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python client for Together's Cloud Platform!
 Project-URL: Homepage, https://github.com/togethercomputer/together
 Project-URL: Bug Tracker, https://github.com/togethercomputer/together/issues
 Author-email: Together Computer <community@together.xyz>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -214,14 +214,15 @@
 Requires-Dist: requests
 Requires-Dist: tqdm
 Requires-Dist: typer
 Provides-Extra: quality
 Requires-Dist: black~=23.1; extra == 'quality'
 Requires-Dist: mypy>=1.3.0; extra == 'quality'
 Requires-Dist: ruff<=0.0.259,>=0.0.241; extra == 'quality'
+Requires-Dist: sseclient-py>=1.7.0; extra == 'quality'
 Requires-Dist: types-requests>=2.31.0.1; extra == 'quality'
 Requires-Dist: types-tqdm>=4.65.0.0; extra == 'quality'
 Description-Content-Type: text/markdown
 
 Python client for Together's Cloud Platform
 
 ## Installation
```

