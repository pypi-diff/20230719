# Comparing `tmp/minetcookies-0.3.6.tar.gz` & `tmp/minetcookies-0.3.7.tar.gz`

## Comparing `minetcookies-0.3.6.tar` & `minetcookies-0.3.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 minetcookies-0.3.6/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 minetcookies-0.3.6/src/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 minetcookies-0.3.6/src/minetcookies/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 minetcookies-0.3.6/src/minetcookies/__init__.py
--rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 minetcookies-0.3.6/src/minetcookies/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 minetcookies-0.3.6/tests/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 minetcookies-0.3.6/.gitignore
--rw-r--r--   0        0        0    34503 2020-02-02 00:00:00.000000 minetcookies-0.3.6/LICENSE.txt
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 minetcookies-0.3.6/README.md
--rw-r--r--   0        0        0     3786 2020-02-02 00:00:00.000000 minetcookies-0.3.6/pyproject.toml
--rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 minetcookies-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 minetcookies-0.3.7/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 minetcookies-0.3.7/src/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 minetcookies-0.3.7/src/minetcookies/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 minetcookies-0.3.7/src/minetcookies/__init__.py
+-rw-r--r--   0        0        0     3856 2020-02-02 00:00:00.000000 minetcookies-0.3.7/src/minetcookies/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 minetcookies-0.3.7/tests/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 minetcookies-0.3.7/.gitignore
+-rw-r--r--   0        0        0    34503 2020-02-02 00:00:00.000000 minetcookies-0.3.7/LICENSE.txt
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 minetcookies-0.3.7/README.md
+-rw-r--r--   0        0        0     3767 2020-02-02 00:00:00.000000 minetcookies-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 minetcookies-0.3.7/PKG-INFO
```

### Comparing `minetcookies-0.3.6/src/minetcookies/main.py` & `minetcookies-0.3.7/src/minetcookies/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import subprocess
 import sys
 from pathlib import Path
 
 import yaml
 
-
 default_yaml = """
 ---
 buzzsumo:
   token: "MY_BZ_TOKEN"
 crowdtangle:
   token: "MY_CT_TOKEN"
   rate_limit: 10
@@ -43,15 +42,15 @@
     pass
 
 
 class NotLoggedIn(Exception):
     pass
 
 
-def CookieChecker(cookie:str, media:str):
+def CookieChecker(cookie: str, media: str):
     media_spec = {
         "twitter": "_twitter_sess=",
         "instagram": "sessionid=",  # "ds_user_id="
         "facebook": "c_user=",
         "tiktok": "sessionid=",
     }
     if cookie is None or cookie == "" or cookie.startswith("MY"):
@@ -62,17 +61,16 @@
 
 
 def minettest():
     try:
         subprocess.run(["minet", "--version"], capture_output=True)
     except FileNotFoundError:
         raise RuntimeError("Minet n'est pas installé ou n'est pas dans le PATH, veuillez exécuter:\n"
-                           "pip install minet\n"
-                           "ou\n"
-                           "pipx install minet")
+                           "pip install minet")
+
 
 def get(media: str, key: str):
     return config[media][key]
 
 
 def set(media: str, key: str, value: str):
     config[media][key] = value
@@ -82,32 +80,36 @@
     configfile.write_text(yaml.dump(config))
 
 
 def recover_cookies(media: str):
     bros = ['chrome', 'firefox', 'chromium', 'edge']
     loggedout = False
     for navigator in bros:
-        cookie = subprocess.run(["minet", "cookies", navigator, "--url", f"https://www.{media}.com"],
-                                capture_output=True)
+        cookie = subprocess.run(
+            ["minet", "cookies", navigator, "--url", f"https://www.{media}.com"],
+            capture_output=True
+        )
         cookie = cookie.stdout.decode("utf-8").strip()
 
         try:
             CookieChecker(cookie, media)
             break
         except UndefinedCookie:
             continue
         except NotLoggedIn:
             loggedout = True
             continue
     else:
         if loggedout:
             raise RuntimeError(
-                f"Vous êtes déconnecté de {media}.com veillez à vous connecter puis réessayez.\n(Navigateurs supportés : {bros})")
+                f"Vous êtes déconnecté de {media}.com veillez à vous connecter puis réessayez."
+                f"\n(Navigateurs supportés : {bros})")
         raise RuntimeError(
-            f"Aucun cookie trouvé pour {media} veillez à vous connecter sur https://www.{media}.com puis réessayez.\n(Navigateurs supportés : {bros})")
+            f"Aucun cookie trouvé pour {media} veillez à vous connecter sur "
+            f"https://www.{media}.com puis réessayez.\n(Navigateurs supportés : {bros})")
 
     cookie = cookie.replace("\n", " ")
 
     set(media, "cookie", cookie)
     save()
 
     print(f"Cookie for {media} saved")
```

### Comparing `minetcookies-0.3.6/LICENSE.txt` & `minetcookies-0.3.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `minetcookies-0.3.6/README.md` & `minetcookies-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `minetcookies-0.3.6/pyproject.toml` & `minetcookies-0.3.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "minetcookies"
 dynamic = ["version"]
-#version = "0.0.4"
 description = 'A simple cookie manager for Minet by Medialab'
 readme = "README.md"
 requires-python = ">=3.7"
 license = "AGPL-3.0-or-later"
 keywords = ["minet", "cookie", "cookies", "manager", "minetcookies", "minet-cookies"]
 authors = [
     { name = "Marceau-h", email = "106751184+Marceau-h@users.noreply.github.com" },
```

### Comparing `minetcookies-0.3.6/PKG-INFO` & `minetcookies-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minetcookies
-Version: 0.3.6
+Version: 0.3.7
 Summary: A simple cookie manager for Minet by Medialab
 Project-URL: Documentation, https://github.com/Marceau-h/minetcookies#readme
 Project-URL: Issues, https://github.com/Marceau-h/minetcookies/issues
 Project-URL: Source, https://github.com/Marceau-h/minetcookies
 Author-email: Marceau-h <106751184+Marceau-h@users.noreply.github.com>
 Maintainer-email: Marceau-h <106751184+Marceau-h@users.noreply.github.com>
 License-Expression: AGPL-3.0-or-later
```

