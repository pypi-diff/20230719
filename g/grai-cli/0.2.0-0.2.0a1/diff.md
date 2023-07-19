# Comparing `tmp/grai_cli-0.2.0.tar.gz` & `tmp/grai_cli-0.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_cli-0.2.0.tar", max compression
+gzip compressed data, was "grai_cli-0.2.0a1.tar", max compression
```

## Comparing `grai_cli-0.2.0.tar` & `grai_cli-0.2.0a1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      237 2023-05-02 08:01:59.659416 grai_cli-0.2.0/README.md
--rw-r--r--   0        0        0      316 2023-07-19 14:10:28.949685 grai_cli-0.2.0/grai_cli/__init__.py
--rw-r--r--   0        0        0       63 2023-02-14 12:06:39.054801 grai_cli-0.2.0/grai_cli/api/__init__.py
--rw-r--r--   0        0        0       51 2023-02-14 12:06:39.054868 grai_cli-0.2.0/grai_cli/api/config/__init__.py
--rw-r--r--   0        0        0     2024 2023-07-19 14:07:41.925075 grai_cli-0.2.0/grai_cli/api/config/config.py
--rw-r--r--   0        0        0     3632 2023-06-06 17:35:16.710877 grai_cli-0.2.0/grai_cli/api/config/set.py
--rw-r--r--   0        0        0      463 2023-02-14 12:06:39.055086 grai_cli-0.2.0/grai_cli/api/config/setup.py
--rw-r--r--   0        0        0     1317 2023-06-06 17:35:16.711010 grai_cli-0.2.0/grai_cli/api/entrypoint.py
--rw-r--r--   0        0        0       49 2023-02-14 12:06:39.055218 grai_cli-0.2.0/grai_cli/api/server/__init__.py
--rw-r--r--   0        0        0     6016 2023-07-19 14:07:41.925515 grai_cli-0.2.0/grai_cli/api/server/endpoints.py
--rw-r--r--   0        0        0     1094 2023-07-19 14:07:41.925819 grai_cli-0.2.0/grai_cli/api/server/setup.py
--rw-r--r--   0        0        0       44 2023-02-14 12:06:39.055429 grai_cli-0.2.0/grai_cli/api/telemetry/__init__.py
--rw-r--r--   0        0        0      376 2023-06-06 17:35:16.711336 grai_cli-0.2.0/grai_cli/api/telemetry/commands.py
--rw-r--r--   0        0        0       89 2023-03-14 10:37:42.059892 grai_cli-0.2.0/grai_cli/config_default.yaml
--rw-r--r--   0        0        0        0 2023-02-14 12:06:39.055556 grai_cli-0.2.0/grai_cli/py.typed
--rw-r--r--   0        0        0       44 2023-02-14 12:06:39.055645 grai_cli-0.2.0/grai_cli/settings/__init__.py
--rw-r--r--   0        0        0     3000 2023-07-19 14:07:41.925979 grai_cli-0.2.0/grai_cli/settings/cache.py
--rw-r--r--   0        0        0     6344 2023-07-19 14:07:41.926140 grai_cli-0.2.0/grai_cli/settings/config.py
--rw-r--r--   0        0        0       88 2023-02-14 12:06:39.055861 grai_cli-0.2.0/grai_cli/utilities/__init__.py
--rw-r--r--   0        0        0     1588 2023-06-06 17:35:16.711673 grai_cli-0.2.0/grai_cli/utilities/headers.py
--rw-r--r--   0        0        0     1180 2023-06-06 17:35:16.711784 grai_cli-0.2.0/grai_cli/utilities/styling.py
--rw-r--r--   0        0        0      796 2023-06-06 17:35:16.711900 grai_cli-0.2.0/grai_cli/utilities/telemetry.py
--rw-r--r--   0        0        0      515 2023-07-19 14:07:41.926264 grai_cli-0.2.0/grai_cli/utilities/test.py
--rw-r--r--   0        0        0     5013 2023-06-06 17:35:16.712102 grai_cli-0.2.0/grai_cli/utilities/utilities.py
--rw-r--r--   0        0        0     2305 2023-06-06 17:35:16.712204 grai_cli-0.2.0/grai_cli/utilities/validators.py
--rw-r--r--   0        0        0     1041 2023-07-19 14:08:00.988556 grai_cli-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1272 1970-01-01 00:00:00.000000 grai_cli-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      237 2023-05-19 11:07:12.863498 grai_cli-0.2.0a1/README.md
+-rw-r--r--   0        0        0      323 2023-07-18 02:25:32.298110 grai_cli-0.2.0a1/grai_cli/__init__.py
+-rw-r--r--   0        0        0       63 2022-11-09 15:55:13.272679 grai_cli-0.2.0a1/grai_cli/api/__init__.py
+-rw-r--r--   0        0        0       51 2022-07-24 08:00:09.094234 grai_cli-0.2.0a1/grai_cli/api/config/__init__.py
+-rw-r--r--   0        0        0     2024 2023-07-17 16:42:30.681148 grai_cli-0.2.0a1/grai_cli/api/config/config.py
+-rw-r--r--   0        0        0     3632 2023-06-14 21:02:53.335424 grai_cli-0.2.0a1/grai_cli/api/config/set.py
+-rw-r--r--   0        0        0      463 2023-06-14 21:02:53.375897 grai_cli-0.2.0a1/grai_cli/api/config/setup.py
+-rw-r--r--   0        0        0     1317 2023-06-14 21:02:53.291370 grai_cli-0.2.0a1/grai_cli/api/entrypoint.py
+-rw-r--r--   0        0        0       49 2022-07-24 08:00:09.100216 grai_cli-0.2.0a1/grai_cli/api/server/__init__.py
+-rw-r--r--   0        0        0     6030 2023-07-17 20:13:45.162367 grai_cli-0.2.0a1/grai_cli/api/server/endpoints.py
+-rw-r--r--   0        0        0     1094 2023-07-17 16:43:38.992726 grai_cli-0.2.0a1/grai_cli/api/server/setup.py
+-rw-r--r--   0        0        0       44 2022-11-09 15:55:13.273574 grai_cli-0.2.0a1/grai_cli/api/telemetry/__init__.py
+-rw-r--r--   0        0        0      376 2023-06-14 21:02:53.379310 grai_cli-0.2.0a1/grai_cli/api/telemetry/commands.py
+-rw-r--r--   0        0        0       89 2023-03-16 04:12:39.225317 grai_cli-0.2.0a1/grai_cli/config_default.yaml
+-rw-r--r--   0        0        0        0 2022-07-24 06:33:14.647347 grai_cli-0.2.0a1/grai_cli/py.typed
+-rw-r--r--   0        0        0       44 2022-11-09 15:55:13.273862 grai_cli-0.2.0a1/grai_cli/settings/__init__.py
+-rw-r--r--   0        0        0     2999 2023-07-18 01:57:07.330038 grai_cli-0.2.0a1/grai_cli/settings/cache.py
+-rw-r--r--   0        0        0     6413 2023-07-18 02:21:27.966349 grai_cli-0.2.0a1/grai_cli/settings/config.py
+-rw-r--r--   0        0        0       88 2023-01-10 17:15:31.923336 grai_cli-0.2.0a1/grai_cli/utilities/__init__.py
+-rw-r--r--   0        0        0     1588 2023-06-01 16:01:43.233062 grai_cli-0.2.0a1/grai_cli/utilities/headers.py
+-rw-r--r--   0        0        0     1180 2023-06-01 16:01:43.233302 grai_cli-0.2.0a1/grai_cli/utilities/styling.py
+-rw-r--r--   0        0        0      796 2023-06-01 16:01:43.233445 grai_cli-0.2.0a1/grai_cli/utilities/telemetry.py
+-rw-r--r--   0        0        0      507 2023-07-17 16:42:57.404252 grai_cli-0.2.0a1/grai_cli/utilities/test.py
+-rw-r--r--   0        0        0     5013 2023-06-14 21:02:53.399455 grai_cli-0.2.0a1/grai_cli/utilities/utilities.py
+-rw-r--r--   0        0        0     2305 2023-06-14 21:02:53.362258 grai_cli-0.2.0a1/grai_cli/utilities/validators.py
+-rw-r--r--   0        0        0     1056 2023-07-18 02:25:32.292022 grai_cli-0.2.0a1/pyproject.toml
+-rw-r--r--   0        0        0     1282 1970-01-01 00:00:00.000000 grai_cli-0.2.0a1/PKG-INFO
```

### Comparing `grai_cli-0.2.0/grai_cli/api/config/config.py` & `grai_cli-0.2.0a1/grai_cli/api/config/config.py`

 * *Files identical despite different names*

### Comparing `grai_cli-0.2.0/grai_cli/api/config/set.py` & `grai_cli-0.2.0a1/grai_cli/api/config/set.py`

 * *Files identical despite different names*

### Comparing `grai_cli-0.2.0/grai_cli/api/entrypoint.py` & `grai_cli-0.2.0a1/grai_cli/api/entrypoint.py`

 * *Files identical despite different names*

### Comparing `grai_cli-0.2.0/grai_cli/api/server/endpoints.py` & `grai_cli-0.2.0a1/grai_cli/api/server/endpoints.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from pathlib import Path
 from typing import Optional
 
 import typer
-from grai_client.schemas.schema import validate_file
 
 from grai_cli.api.entrypoint import app
 from grai_cli.api.server.setup import client_app, client_get_app, get_default_client
 from grai_cli.utilities import utilities
 from grai_cli.utilities.styling import default_styler
 from grai_cli.utilities.utilities import merge_dicts, write_yaml
+from grai_client.schemas.schema import validate_file
 
 
 @client_app.command("is_authenticated", help="Verify auth credentials are valid")
 def is_authenticated():
     """ """
     client = get_default_client()
     authentication_status = client.check_authentication()
@@ -20,15 +20,19 @@
         utilities.print("Authenticated")
     else:
         utilities.print(
             f"Failed to Authenticate: Code {authentication_status.status_code}, {authentication_status.content}"
         )
 
 
-def get_nodes(print: bool = True, to_file: Optional[Path] = None, **kwargs):
+def get_nodes(
+    print: bool = True,
+    to_file: Optional[Path] = None,
+    **kwargs
+):
     """
 
     Args:
         name (Optional[str], optional):  (Default value = None)
         namespace (Optional[str], optional):  (Default value = None)
         print (bool, optional):  (Default value = True)
         to_file (Optional[Path], optional):  (Default value = None)
```

### Comparing `grai_cli-0.2.0/grai_cli/api/server/setup.py` & `grai_cli-0.2.0a1/grai_cli/api/server/setup.py`

 * *Files identical despite different names*

### Comparing `grai_cli-0.2.0/grai_cli/settings/cache.py` & `grai_cli-0.2.0a1/grai_cli/settings/cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import os
 import shelve
 import tempfile
 import uuid
 import warnings
-from tempfile import NamedTemporaryFile
 
 import typer
 
 from grai_cli.settings.config import config
-
+from tempfile import NamedTemporaryFile
 
 class GraiCache:
     """ """
 
     def __init__(self):
         self.cache_filename = "cache"
```

### Comparing `grai_cli-0.2.0/grai_cli/settings/config.py` & `grai_cli-0.2.0a1/grai_cli/settings/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import platform
 import warnings
 from typing import Any, Dict, Literal, Optional, Union
 
 import yaml
 from pydantic import BaseModel, BaseSettings, SecretStr
+import warnings
 
 OS = platform.system()
 if OS == "Darwin":
     _HOME_PATH = os.path.expanduser("~")
     DEFAULT_CONFIG_PATHS = [f"{_HOME_PATH}/.config/grai"]
 elif OS == "Linux":
     _HOME_PATH = os.path.expanduser("~")
@@ -21,33 +22,30 @@
 else:
     warnings.warn(f"Operating system {OS} not recognized. Expected either 'Darwin', 'Windows', or 'Linux'")
     _HOME_PATH = os.path.expanduser("~")
     DEFAULT_CONFIG_PATHS = [f"{_HOME_PATH}/.config/grai"]
 
 DEFAULT_CONFIG_PATH = DEFAULT_CONFIG_PATHS[0]
 
-
 class ConfigDirHandler:
     """ """
-
     DEFAULT_CONFIG_PATHS = DEFAULT_CONFIG_PATHS
     DEFAULT_CONFIG_PATH = DEFAULT_CONFIG_PATHS[0]
     DEFAULT_CONFIG_FILE_NAMES = ["config.yaml", "config.yml"]
 
     def __init__(self):
         path = os.environ.get("GRAI_CLI_CONFIG_DIR", None)
         self.config_paths = [path, *self.DEFAULT_CONFIG_PATHS] if path is not None else [*self.DEFAULT_CONFIG_PATHS]
         self.default_config_file = os.path.join(self.DEFAULT_CONFIG_PATH, self.DEFAULT_CONFIG_FILE_NAMES[0])
 
         self.config_file: str = self.get_config_file()
         self.has_config_file: bool = self.config_file is not None
         self.config_dir: Optional[str] = os.path.dirname(self.config_file) if self.has_config_file else None
 
         self._config_content: Dict = None
-
     def get_config_file(self) -> Optional[str]:
         for path in self.config_paths:
             for filename in self.DEFAULT_CONFIG_FILE_NAMES:
                 config_file = os.path.join(path, filename)
                 if os.path.exists(config_file):
                     return config_file
 
@@ -58,15 +56,15 @@
         """ """
         if isinstance(self._config_content, dict):
             return self._config_content
         elif not self.has_config_file:
             return {}
 
         with open(self.config_file, "r") as file:
-            self._config_content = yaml.safe_load(file)
+            self._config_content= yaml.safe_load(file)
         return self._config_content
 
     @config_content.setter
     def config_content(self, value: Dict):
         """
 
         Args:
@@ -82,15 +80,14 @@
         self._config_content = value
 
     def save_content(self):
         """ """
         with open(self.config_file, "w") as file:
             yaml.safe_dump(self._config_content, file)
 
-
 def unredact(obj: Any) -> Any:
     """
 
     Args:
         obj (Any):
 
     Returns:
@@ -116,17 +113,19 @@
         settings:
 
     Returns:
 
     Raises:
 
     """
+    print('yaml loader', config_handler.config_content)
     return config_handler.config_content
 
 
+
 class ServerSettingsV1(BaseModel):
     """ """
 
     api_version: Literal["v1"] = "v1"
     url: str
     workspace: str
 
@@ -231,7 +230,8 @@
         f"2) The config directory is incorrect. We've attempted looking in the following directories: "
         f"{config_handler.DEFAULT_CONFIG_PATHS} based on our operating system and the `GRAI_CLI_CONFIG_DIR` env var. \n"
         f"3) You may have made a mistake configuring your environment based purely on environment variables. \n"
         f"{os.environ.get('GRAI_CLI_CONFIG_DIR')}"
     )
     warnings.warn(message)
     config = GraiConfig.default_config()
+
```

### Comparing `grai_cli-0.2.0/grai_cli/utilities/headers.py` & `grai_cli-0.2.0a1/grai_cli/utilities/headers.py`

 * *Files identical despite different names*

### Comparing `grai_cli-0.2.0/grai_cli/utilities/styling.py` & `grai_cli-0.2.0a1/grai_cli/utilities/styling.py`

 * *Files identical despite different names*

### Comparing `grai_cli-0.2.0/grai_cli/utilities/telemetry.py` & `grai_cli-0.2.0a1/grai_cli/utilities/telemetry.py`

 * *Files identical despite different names*

### Comparing `grai_cli-0.2.0/grai_cli/utilities/utilities.py` & `grai_cli-0.2.0a1/grai_cli/utilities/utilities.py`

 * *Files identical despite different names*

### Comparing `grai_cli-0.2.0/grai_cli/utilities/validators.py` & `grai_cli-0.2.0a1/grai_cli/utilities/validators.py`

 * *Files identical despite different names*

### Comparing `grai_cli-0.2.0/pyproject.toml` & `grai_cli-0.2.0a1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grai-cli"
-version = "0.2.0"
+version = "0.2.0-alpha1"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>"]
 license = "Elastic-2.0"
 readme = "README.md"
 packages = [{include = "grai_cli"}]
 homepage = "https://www.grai.io/"
 repository = "https://github.com/grai-io/grai-core/tree/master/grai-cli"
@@ -16,15 +16,15 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 multimethod = "^1.9"
 typer = "^0.7.0"
 confuse = "^2.0.0"
 requests = "^2.28.1"
 pydantic = "^1.10.11"
-grai-client = "^0.3.0"
+grai-client = "^0.3.0-alpha25"
 posthog = "^2.2.0"
 rich = "^12.6.0"
 grai-schemas = "^0.2.0a10"
 
 [tool.isort]
 profile = "black"
 known_first_party = "grai_cli"
```

### Comparing `grai_cli-0.2.0/PKG-INFO` & `grai_cli-0.2.0a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: grai-cli
-Version: 0.2.0
+Version: 0.2.0a1
 Summary: 
 Home-page: https://www.grai.io/
 License: Elastic-2.0
 Author: Ian Eaves
 Author-email: ian@grai.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: confuse (>=2.0.0,<3.0.0)
-Requires-Dist: grai-client (>=0.3.0,<0.4.0)
+Requires-Dist: grai-client (>=0.3.0-alpha25,<0.4.0)
 Requires-Dist: grai-schemas (>=0.2.0a10,<0.3.0)
 Requires-Dist: multimethod (>=1.9,<2.0)
 Requires-Dist: posthog (>=2.2.0,<3.0.0)
 Requires-Dist: pydantic (>=1.10.11,<2.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: rich (>=12.6.0,<13.0.0)
 Requires-Dist: typer (>=0.7.0,<0.8.0)
```

