# Comparing `tmp/streamlink-repo-1.0.4.tar.gz` & `tmp/streamlink-repo-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\streamlink-repo-1.0.4.tar", last modified: Mon Jul 17 15:49:17 2023, max compression
+gzip compressed data, was "dist\streamlink-repo-1.0.5.tar", last modified: Wed Jul 19 13:45:01 2023, max compression
```

## Comparing `streamlink-repo-1.0.4.tar` & `streamlink-repo-1.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 15:49:17.201935 streamlink-repo-1.0.4/
--rw-rw-rw-   0        0        0    17096 2023-07-17 12:16:21.000000 streamlink-repo-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     1416 2023-07-17 15:49:17.200410 streamlink-repo-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1187 2023-07-17 15:14:48.000000 streamlink-repo-1.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-07-17 15:49:17.201935 streamlink-repo-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      681 2023-07-17 15:46:30.000000 streamlink-repo-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 15:49:17.167621 streamlink-repo-1.0.4/streamlink_repo/
--rw-rw-rw-   0        0        0    13925 2023-07-17 12:57:44.000000 streamlink-repo-1.0.4/streamlink_repo/__init__.py
--rw-rw-rw-   0        0        0     4635 2023-07-17 12:35:55.000000 streamlink-repo-1.0.4/streamlink_repo/common.py
--rw-rw-rw-   0        0        0      632 2023-07-17 08:49:48.000000 streamlink-repo-1.0.4/streamlink_repo/paths.py
-drwxrwxrwx   0        0        0        0 2023-07-17 15:49:17.199293 streamlink-repo-1.0.4/streamlink_repo.egg-info/
--rw-rw-rw-   0        0        0     1416 2023-07-17 15:49:16.000000 streamlink-repo-1.0.4/streamlink_repo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      341 2023-07-17 15:49:17.000000 streamlink-repo-1.0.4/streamlink_repo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 15:49:16.000000 streamlink-repo-1.0.4/streamlink_repo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-07-17 15:49:16.000000 streamlink-repo-1.0.4/streamlink_repo.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       31 2023-07-17 15:49:16.000000 streamlink-repo-1.0.4/streamlink_repo.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-17 15:49:16.000000 streamlink-repo-1.0.4/streamlink_repo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-19 13:45:01.197776 streamlink-repo-1.0.5/
+-rw-rw-rw-   0        0        0    17096 2023-07-17 12:16:21.000000 streamlink-repo-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1416 2023-07-19 13:45:01.195766 streamlink-repo-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1187 2023-07-17 15:14:48.000000 streamlink-repo-1.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-19 13:45:01.197776 streamlink-repo-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      681 2023-07-19 13:44:52.000000 streamlink-repo-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 13:45:01.162785 streamlink-repo-1.0.5/streamlink_repo/
+-rw-rw-rw-   0        0        0    18076 2023-07-19 13:43:33.000000 streamlink-repo-1.0.5/streamlink_repo/__init__.py
+-rw-rw-rw-   0        0        0     4635 2023-07-17 12:35:55.000000 streamlink-repo-1.0.5/streamlink_repo/common.py
+-rw-rw-rw-   0        0        0      632 2023-07-17 08:49:48.000000 streamlink-repo-1.0.5/streamlink_repo/paths.py
+drwxrwxrwx   0        0        0        0 2023-07-19 13:45:01.193853 streamlink-repo-1.0.5/streamlink_repo.egg-info/
+-rw-rw-rw-   0        0        0     1416 2023-07-19 13:45:00.000000 streamlink-repo-1.0.5/streamlink_repo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      341 2023-07-19 13:45:01.000000 streamlink-repo-1.0.5/streamlink_repo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 13:45:00.000000 streamlink-repo-1.0.5/streamlink_repo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-07-19 13:45:00.000000 streamlink-repo-1.0.5/streamlink_repo.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       31 2023-07-19 13:45:00.000000 streamlink-repo-1.0.5/streamlink_repo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-19 13:45:00.000000 streamlink-repo-1.0.5/streamlink_repo.egg-info/top_level.txt
```

### Comparing `streamlink-repo-1.0.4/LICENSE` & `streamlink-repo-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlink-repo-1.0.4/PKG-INFO` & `streamlink-repo-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlink-repo
-Version: 1.0.4
+Version: 1.0.5
 Summary: Unofficial Plugin repository implementation for streamlink-cli.
 Author: Parrot Developers
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Streamlink-Repo
```

### Comparing `streamlink-repo-1.0.4/README.md` & `streamlink-repo-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `streamlink-repo-1.0.4/setup.py` & `streamlink-repo-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='streamlink-repo',
-    version='1.0.4',
+    version='1.0.5',
     author='Parrot Developers',
     description='Unofficial Plugin repository implementation for streamlink-cli.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=['streamlink_repo'],
     install_requires=[
         'pyinquirer',
```

### Comparing `streamlink-repo-1.0.4/streamlink_repo/__init__.py` & `streamlink-repo-1.0.5/streamlink_repo/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 import os
 import sys
 import json
 import typer
 import requests
+import subprocess
 from colorama import init, Fore
 from urllib.parse import urljoin, urlparse
 from PyInquirer import style_from_dict, Token, prompt, Separator
 from .paths import USERDATA, DB_FOLDER
 from .common import get_plugins_folder, download_file, clear_console, banner
 init()
 
 repos_file = os.path.join(DB_FOLDER, "repos.json")
 repos_plugins_file = os.path.join(DB_FOLDER, "repos_plugins.json")
 installed_file = os.path.join(DB_FOLDER, "installed.json")
+settings_file = os.path.join(DB_FOLDER, "settings.json")
+
 
 if not os.path.exists(repos_file):
     open(repos_file, "w", encoding="utf-8").write("[]")
 
 if not os.path.exists(repos_plugins_file):
     open(repos_plugins_file, "w", encoding="utf-8").write("[]")
 
 if not os.path.exists(installed_file):
     open(installed_file, "w", encoding="utf-8").write("[]")
 
+
+if not os.path.exists(settings_file):
+    open(settings_file, "w", encoding="utf-8").write("{}")
+
 app = typer.Typer()
 style = style_from_dict({
     Token.Separator: '#cc5454',
     Token.QuestionMark: '#673ab7 bold',
     Token.Selected: '#cc5454',  # default
     Token.Pointer: '#673ab7 bold',
     Token.Instruction: '',  # default
@@ -187,38 +194,65 @@
         home()
         return
 
 
 
 
     def install_deps(deps):
-        pass
-
+        settings_ = json.load(open(settings_file, encoding="utf-8"))
+        streamlink_packages_path = settings_.get("streamlink_packages_path", "")
+        if not streamlink_packages_path:
+            print("Automatic installation requires you to set pkgs path")
+            print("Do you want to set it now?")
+            options = [
+                {
+                    'type': 'list',
+                    'message': 'Select option',
+                    'name': 'options',
+                    'choices': [
+                        {
+                            'name': 'Yes',
+                            'func': extra_settings,
+                        },
+                        {
+                            'name': 'No',
+                            'func': None,
+                        }
+                    ]
+                }
+            ]
+            answer = prompt(options, style=style)
+            picked = [item for item in options[0]["choices"] if item['name'] == answer['options']][0]
+            if picked['func']:
+                picked['func']()
+            return
+        
+        for dep in deps:
+            subprocess.check_call(["pip", "install", "--target", streamlink_packages_path, dep])
+        print("Installed all dependencies")
 
 
 
-    #if plugin['deps']:
-    if False: #TODO: finish this ...
+    if plugin['deps']:
         print(f'This plugin contains dependencies: {Fore.CYAN} {", ".join(plugin["deps"])} {Fore.WHITE}\n',
-              f'Do you want to install them automatically? (WARNING: This option is in testing and may cause issues. ',
-              f'It is recommended to install them manually.)')
+              f'Do you want to install them automatically? (WARNING: This option is in testing and may cause issues)')
         options = [
             {
                 'type': 'list',
                 'message': 'Select option',
                 'name': 'options',
                 'choices': [
                     {
-                        'name': 'No (Recommended)',
-                        'func': None,
-                    },
-                    {
-                        'name': 'Yes (Not Recommended)',
+                        'name': 'Yes, Install automatically',
                         'func': install_deps,
                     },
+                    {
+                        'name': 'No, Install manually',
+                        'func': None,
+                    }
                 ]
             }
         ]
         answer = prompt(options, style=style)
         picked = [item for item in options[0]["choices"] if item['name'] == answer['options']][0]
         if picked['func']:
             picked['func'](plugin['deps'])
@@ -329,22 +363,121 @@
                     'name': 'Scan repos',
                     'func': scan_repos
                 },
                 {
                     'name': 'Remove Repo',
                     'func': remove_repo
                 },
+                {
+                    'name': 'Extra Settings',
+                    'func': extra_settings
+                },
             ]
         }
     ]
 
     answer = prompt(options, style=style)
     [item for item in options[0]["choices"] if item['name'] == answer['options']][0]['func']()
 
 
+
+def extra_settings():
+    clear_console()
+    options = [
+        {
+            'type': 'list',
+            'message': 'Select option',
+            'name': 'options',
+            'choices': [  
+                {
+                    'name': 'Go Back',
+                    'func': settings,
+                    'args': None
+                },       
+                {
+                    'name': 'Streamlink Path (streamlink.exe)',
+                    'func': options_extra,
+                    'args': ("streamlink_path",)
+                },
+                {
+                    'name': 'Streamlink Python Packages Folder (pkgs/)',
+                    'func': options_extra,
+                    'args': ("streamlink_packages_path",)
+                },
+
+            ]
+        }
+    ]
+
+    answer = prompt(options, style=style)
+    picked = [item for item in options[0]["choices"] if item['name'] == answer['options']][0]
+    if picked['args']:
+        args = (picked['name'],) + picked['args']
+        picked['func'](*args)
+    else:
+        picked['func']()
+
+def options_extra(name, key):
+    clear_console()
+
+    options = [
+        {
+            'type': 'list',
+            'message': 'Select option',
+            'name': 'options',
+            'choices': [  
+                {
+                    'name': 'Go Back',
+                    'func': extra_settings,
+                    'args': None
+                },     
+                {
+                    'name': f'Set {name}',
+                    'func': input_extra,
+                    'args': (key,)
+                }, 
+                {
+                    'name': f'Get {name}',
+                    'func': info_extra,
+                    'args': (key,)
+                },
+            ]
+        }
+    ]
+
+    answer = prompt(options, style=style)
+    picked = [item for item in options[0]["choices"] if item['name'] == answer['options']][0]
+    if picked['args']:
+        args = (picked['name'],) + picked['args']
+        picked['func'](*args)
+    else:
+        picked['func']()
+
+
+def info_extra(name, key):
+    clear_console()
+    settings_ = json.load(open(settings_file, encoding="utf-8"))
+    print(Fore.RED+settings_.get(key, "")+Fore.WHITE)
+    input("Press enter to continue ...")
+    extra_settings()
+
+
+def input_extra(name, key):
+    clear_console()
+    settings_ = json.load(open(settings_file, encoding="utf-8"))
+    inp = input(f"{name}: ")
+    print(inp)
+
+    if inp:
+        settings_[key] = inp
+        json.dump(settings_, open(settings_file, "w", encoding="utf-8"))
+    extra_settings()
+
+
+
 def list_repos():
     clear_console()
     repos = json.load(open(repos_file))
     print(Fore.RED+"\n".join(repos)+Fore.WHITE)
     input("Press enter to continue ...")
     settings()
```

### Comparing `streamlink-repo-1.0.4/streamlink_repo/common.py` & `streamlink-repo-1.0.5/streamlink_repo/common.py`

 * *Files identical despite different names*

### Comparing `streamlink-repo-1.0.4/streamlink_repo/paths.py` & `streamlink-repo-1.0.5/streamlink_repo/paths.py`

 * *Files identical despite different names*

### Comparing `streamlink-repo-1.0.4/streamlink_repo.egg-info/PKG-INFO` & `streamlink-repo-1.0.5/streamlink_repo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlink-repo
-Version: 1.0.4
+Version: 1.0.5
 Summary: Unofficial Plugin repository implementation for streamlink-cli.
 Author: Parrot Developers
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Streamlink-Repo
```

