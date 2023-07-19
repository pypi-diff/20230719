# Comparing `tmp/timedctl-2.0.1.tar.gz` & `tmp/timedctl-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timedctl-2.0.1.tar", max compression
+gzip compressed data, was "timedctl-3.0.0.tar", max compression
```

## Comparing `timedctl-2.0.1.tar` & `timedctl-3.0.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    34454 2023-07-19 07:57:19.602778 timedctl-2.0.1/LICENSE
--rw-r--r--   0        0        0      810 2023-07-19 07:57:19.602778 timedctl-2.0.1/README.md
--rw-r--r--   0        0        0      824 2023-07-19 07:57:20.322775 timedctl-2.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-19 07:57:19.602778 timedctl-2.0.1/timedctl/__init__.py
--rwxr-xr-x   0        0        0    11609 2023-07-19 07:57:19.606778 timedctl-2.0.1/timedctl/timedctl.py
--rw-r--r--   0        0        0     1519 1970-01-01 00:00:00.000000 timedctl-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0    34454 2023-07-19 10:03:17.733500 timedctl-3.0.0/LICENSE
+-rw-r--r--   0        0        0      810 2023-07-19 10:03:17.733500 timedctl-3.0.0/README.md
+-rw-r--r--   0        0        0      823 2023-07-19 10:03:18.757514 timedctl-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-19 10:03:17.733500 timedctl-3.0.0/timedctl/__init__.py
+-rwxr-xr-x   0        0        0    11501 2023-07-19 10:03:17.733500 timedctl-3.0.0/timedctl/timedctl.py
+-rw-r--r--   0        0        0     1512 1970-01-01 00:00:00.000000 timedctl-3.0.0/PKG-INFO
```

### Comparing `timedctl-2.0.1/LICENSE` & `timedctl-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `timedctl-2.0.1/README.md` & `timedctl-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `timedctl-2.0.1/pyproject.toml` & `timedctl-3.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "timedctl"
-version = "2.0.1"
+version = "3.0.0"
 description = "CLI for timed"
 authors = ["Arthur Deierlein <arthur.deierlein@adfinis.com>", "Gian Klug <gian.klug@adfinis.com>"]
 readme = "README.md"
 license = "AGPL-3.0-only"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 click = "^8.1.3"
 pyfzf = "^0.3.1"
 rich = "^13.4.2"
-libtimed = "^0.1.0"
+libtimed = "0.2.0"
 terminaltables = "^3.1.10"
 tomlkit = "^0.11.8"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pytest = "^7.3.2"
```

### Comparing `timedctl-2.0.1/timedctl/timedctl.py` & `timedctl-3.0.0/timedctl/timedctl.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 from libtimed import TimedAPIClient
 from libtimed.oidc import OIDCClient
 
 
 def load_config():
     """Load the timedctl config."""
     cfg = {
-        "username": "",
+        "username": "test",
         "timed_url": "https://timed.example.com",
-        "oidc_client_id": "timed",
-        "oidc_auth_endpoint": "http://sso.local/auth/realms/test/protocol/openid-connect/auth",
-        "oidc_token_endpoint": "http://sso.local/auth/realms/test/protocol/openid-connect/token",
+        "sso_url": "https://sso.example.com",
+        "sso_realm": "example",
+        "sso_client_id": "timedctl",
     }
 
     # Get the path to the config file based on the $XDG_config_HOME environment variable
     if not os.getenv("HOME"):
         raise EnvironmentError("$HOME is not set")
 
     xdg_config_home = os.getenv(
@@ -36,15 +36,15 @@
     config_dir = os.path.join(xdg_config_home, "timedctl")
     config_file = os.path.join(config_dir, "config.toml")
 
     if not os.path.isfile(config_file):
         os.makedirs(config_dir, exist_ok=True)
         print("No config file found. Please enter the following infos.")
         for key in cfg:
-            cfg[key] = input(f"{key}: ")
+            cfg[key] = input(f"{key} ({cfg[key]}): ")
         with open(config_file, "w", encoding="utf-8") as file:
             dump(cfg, file)
     else:
         with open(config_file, "rb") as file:
             user_config = tomllib.load(file)
         for key in user_config:
             cfg[key] = user_config[key]
@@ -57,19 +57,19 @@
 def client_setup():
     """Set up the timed client."""
     # initialize libtimed
     url = config.get("timed_url")
     api_namespace = "api/v1"
 
     # Auth stuff
-    client_id = config.get("oidc_client_id")
-    auth_endpoint = config.get("oidc_auth_endpoint")
-    token_endpoint = config.get("oidc_token_endpoint")
+    client_id = config.get("sso_client_id")
+    sso_url = config.get("sso_url")
+    sso_realm = config.get("sso_realm")
     auth_path = "timedctl/auth"
-    oidc_client = OIDCClient(client_id, auth_endpoint, token_endpoint, auth_path)
+    oidc_client = OIDCClient(client_id, sso_url, sso_realm, auth_path)
     token = oidc_client.authorize()
     return TimedAPIClient(token, url, api_namespace)
 
 
 def msg(message, nonl=False):
     """Print a message in bold green."""
     rich.print(f"[bold green]{message}[/bold green]", end="" if nonl else "\n")
@@ -217,15 +217,15 @@
                 project,
                 task,
                 report["attributes"]["comment"],
                 report["attributes"]["duration"],
             ]
         )
     output = terminaltables.SingleTable(table)
-    msg(f"Reports for {date}:")
+    msg(f"Reports for {date if date is not None else 'today'}:")
     click.echo(output.table)
     msg(f"Total: {time_sum(table)}")
 
 
 @get.command("absences")
 def get_absences():
     """Get absences."""
```

### Comparing `timedctl-2.0.1/PKG-INFO` & `timedctl-3.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: timedctl
-Version: 2.0.1
+Version: 3.0.0
 Summary: CLI for timed
 License: AGPL-3.0-only
 Author: Arthur Deierlein
 Author-email: arthur.deierlein@adfinis.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: libtimed (>=0.1.0,<0.2.0)
+Requires-Dist: libtimed (==0.2.0)
 Requires-Dist: pyfzf (>=0.3.1,<0.4.0)
 Requires-Dist: rich (>=13.4.2,<14.0.0)
 Requires-Dist: terminaltables (>=3.1.10,<4.0.0)
 Requires-Dist: tomlkit (>=0.11.8,<0.12.0)
 Description-Content-Type: text/markdown
 
 # timedctl
```

