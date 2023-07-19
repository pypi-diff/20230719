# Comparing `tmp/gmcapsule-0.5.2.tar.gz` & `tmp/gmcapsule-0.5.3.tar.gz`

## Comparing `gmcapsule-0.5.2.tar` & `gmcapsule-0.5.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 gmcapsule-0.5.2/example.ini
--rw-r--r--   0        0        0    21706 2020-02-02 00:00:00.000000 gmcapsule-0.5.2/gmcapsule/__init__.py
--rw-r--r--   0        0        0    33471 2020-02-02 00:00:00.000000 gmcapsule-0.5.2/gmcapsule/gemini.py
--rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 gmcapsule-0.5.2/gmcapsule/markdown.py
--rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 gmcapsule-0.5.2/gmcapsule/modules/10_rewrite.py
--rwxr-xr-x   0        0        0    18619 2020-02-02 00:00:00.000000 gmcapsule-0.5.2/gmcapsule/modules/80_gitview.py
--rw-r--r--   0        0        0     6379 2020-02-02 00:00:00.000000 gmcapsule-0.5.2/gmcapsule/modules/90_cgi.py
--rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 gmcapsule-0.5.2/gmcapsule/modules/99_static.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 gmcapsule-0.5.2/.gitignore
--rw-r--r--   0        0        0     4080 2020-02-02 00:00:00.000000 gmcapsule-0.5.2/README.md
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 gmcapsule-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     4993 2020-02-02 00:00:00.000000 gmcapsule-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 gmcapsule-0.5.3/example.ini
+-rw-r--r--   0        0        0    21706 2020-02-02 00:00:00.000000 gmcapsule-0.5.3/gmcapsule/__init__.py
+-rw-r--r--   0        0        0    33551 2020-02-02 00:00:00.000000 gmcapsule-0.5.3/gmcapsule/gemini.py
+-rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 gmcapsule-0.5.3/gmcapsule/markdown.py
+-rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 gmcapsule-0.5.3/gmcapsule/modules/10_rewrite.py
+-rwxr-xr-x   0        0        0    18619 2020-02-02 00:00:00.000000 gmcapsule-0.5.3/gmcapsule/modules/80_gitview.py
+-rw-r--r--   0        0        0     6379 2020-02-02 00:00:00.000000 gmcapsule-0.5.3/gmcapsule/modules/90_cgi.py
+-rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 gmcapsule-0.5.3/gmcapsule/modules/99_static.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 gmcapsule-0.5.3/.gitignore
+-rw-r--r--   0        0        0     4177 2020-02-02 00:00:00.000000 gmcapsule-0.5.3/README.md
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 gmcapsule-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     5090 2020-02-02 00:00:00.000000 gmcapsule-0.5.3/PKG-INFO
```

### Comparing `gmcapsule-0.5.2/example.ini` & `gmcapsule-0.5.3/example.ini`

 * *Files identical despite different names*

### Comparing `gmcapsule-0.5.2/gmcapsule/__init__.py` & `gmcapsule-0.5.3/gmcapsule/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -491,15 +491,15 @@
 import subprocess
 from pathlib import Path
 
 from .gemini import Server, Cache, Context, Identity
 from .markdown import to_gemtext as markdown_to_gemtext
 
 
-__version__ = '0.5.2'
+__version__ = '0.5.3'
 __all__ = [
     'Config', 'Cache', 'Context', 'Identity',
     'get_mime_type', 'markdown_to_gemtext'
 ]
 
 
 class Config:
```

### Comparing `gmcapsule-0.5.2/gmcapsule/gemini.py` & `gmcapsule-0.5.3/gmcapsule/gemini.py`

 * *Files 1% similar despite different names*

```diff
@@ -849,14 +849,15 @@
 
     def run(self):
         attempts = 60
         print(f'Opening port {self.port}...')
         while True:
             try:
                 self.sock = socket.socket()
+                self.sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
                 self.sock.bind((self.address, self.port))
                 self.sock.listen(5)
                 self.sv_conn = SSL.Connection(self.context, self.sock)
                 self.sv_conn.set_accept_state()
                 break
             except:
                 attempts -= 1
```

### Comparing `gmcapsule-0.5.2/gmcapsule/markdown.py` & `gmcapsule-0.5.3/gmcapsule/markdown.py`

 * *Files identical despite different names*

### Comparing `gmcapsule-0.5.2/gmcapsule/modules/10_rewrite.py` & `gmcapsule-0.5.3/gmcapsule/modules/10_rewrite.py`

 * *Files identical despite different names*

### Comparing `gmcapsule-0.5.2/gmcapsule/modules/80_gitview.py` & `gmcapsule-0.5.3/gmcapsule/modules/80_gitview.py`

 * *Files identical despite different names*

### Comparing `gmcapsule-0.5.2/gmcapsule/modules/90_cgi.py` & `gmcapsule-0.5.3/gmcapsule/modules/90_cgi.py`

 * *Files identical despite different names*

### Comparing `gmcapsule-0.5.2/gmcapsule/modules/99_static.py` & `gmcapsule-0.5.3/gmcapsule/modules/99_static.py`

 * *Files identical despite different names*

### Comparing `gmcapsule-0.5.2/README.md` & `gmcapsule-0.5.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,18 @@
 
 * `Identity` class is available when importing the `gmcapsule` module.
 
 v0.5.2:
 
 * Fixed error in the "rewrite" module (Codeberg PR #1).
 
+v0.5.3:
+
+* Enable address reuse on the server socket for unimpeded restarting (Codeberg PR #3).
+
 ### v0.4
 
 * Added built-in module "rewrite" that matches regular expressions against the request path and can rewrite the path or return a custom status for redirection, "Gone" messages, or other exceptional situations.
 * Extension module load order is determined after locating all modules from all directories. Previously, the order was local to each directory.
 * Added a new configuration section `[priority]` for overriding default module priorities determined from file names. This is useful for changing the priority of the built-in modules.
 
 v0.4.1:
```

### Comparing `gmcapsule-0.5.2/pyproject.toml` & `gmcapsule-0.5.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gmcapsule-0.5.2/PKG-INFO` & `gmcapsule-0.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmcapsule
-Version: 0.5.2
+Version: 0.5.3
 Summary: Extensible Gemini/Titan server
 Project-URL: Home-page, https://geminispace.org/gmcapsule/
 Project-URL: Documentation, https://geminispace.org/gmcapsule/gmcapsule.html
 Project-URL: Source, https://codeberg.org/skyjake/gmcapsule
 Project-URL: Issues, https://codeberg.org/skyjake/gmcapsule/issues
 Author-email: Jaakko Keränen <jaakko.keranen@iki.fi>
 Keywords: gemini,internet,server,titan
@@ -81,14 +81,18 @@
 
 * `Identity` class is available when importing the `gmcapsule` module.
 
 v0.5.2:
 
 * Fixed error in the "rewrite" module (Codeberg PR #1).
 
+v0.5.3:
+
+* Enable address reuse on the server socket for unimpeded restarting (Codeberg PR #3).
+
 ### v0.4
 
 * Added built-in module "rewrite" that matches regular expressions against the request path and can rewrite the path or return a custom status for redirection, "Gone" messages, or other exceptional situations.
 * Extension module load order is determined after locating all modules from all directories. Previously, the order was local to each directory.
 * Added a new configuration section `[priority]` for overriding default module priorities determined from file names. This is useful for changing the priority of the built-in modules.
 
 v0.4.1:
```

