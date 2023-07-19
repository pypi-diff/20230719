# Comparing `tmp/understar-0.2.4.tar.gz` & `tmp/understar-2.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "understar-0.2.4.tar", last modified: Sun Jul 16 05:00:25 2023, max compression
+gzip compressed data, was "understar-2.32.tar", last modified: Wed Jul 19 04:53:08 2023, max compression
```

## Comparing `understar-0.2.4.tar` & `understar-2.32.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-16 05:00:25.122559 understar-0.2.4/
--rw-r--r--   0 maxence    (501) staff       (20)     1188 2023-05-26 01:06:57.000000 understar-0.2.4/LICENSE.md
--rw-r--r--   0 maxence    (501) staff       (20)      591 2023-07-16 05:00:25.122293 understar-0.2.4/PKG-INFO
--rw-r--r--   0 maxence    (501) staff       (20)       45 2023-05-26 01:06:57.000000 understar-0.2.4/README.md
--rw-r--r--   0 maxence    (501) staff       (20)       38 2023-07-16 05:00:25.122615 understar-0.2.4/setup.cfg
--rw-r--r--   0 maxence    (501) staff       (20)     1222 2023-07-16 04:54:52.000000 understar-0.2.4/setup.py
-drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-16 05:00:25.114992 understar-0.2.4/understar/
--rw-r--r--   0 maxence    (501) staff       (20)       49 2023-07-12 03:28:50.000000 understar-0.2.4/understar/__init__.py
-drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-16 05:00:25.116239 understar-0.2.4/understar/system/
--rw-r--r--   0 maxence    (501) staff       (20)       22 2023-07-16 04:49:43.000000 understar-0.2.4/understar/system/__init__.py
-drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-16 05:00:25.116561 understar-0.2.4/understar/system/app/
--rw-r--r--   0 maxence    (501) staff       (20)       89 2023-07-16 04:47:12.000000 understar-0.2.4/understar/system/app/__init__.py
-drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-16 05:00:25.116900 understar-0.2.4/understar/system/app/config/
--rw-r--r--   0 maxence    (501) staff       (20)    19996 2023-07-16 04:54:09.000000 understar-0.2.4/understar/system/app/config/__init__.py
-drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-16 05:00:25.117883 understar-0.2.4/understar/system/app/config/apt/
--rw-r--r--   0 maxence    (501) staff       (20)       32 2023-07-12 03:26:34.000000 understar-0.2.4/understar/system/app/config/apt/__init__.py
--rw-r--r--   0 maxence    (501) staff       (20)     3351 2023-07-16 04:54:11.000000 understar-0.2.4/understar/system/app/config/apt/install.py
--rw-r--r--   0 maxence    (501) staff       (20)     1329 2023-07-16 04:54:12.000000 understar-0.2.4/understar/system/app/config/apt/uninstall.py
-drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-16 05:00:25.118108 understar-0.2.4/understar/system/app/maintenance/
--rw-r--r--   0 maxence    (501) staff       (20)      902 2023-07-16 04:54:14.000000 understar-0.2.4/understar/system/app/maintenance/__init__.py
-drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-16 05:00:25.121731 understar-0.2.4/understar/system/lib/
--rw-r--r--   0 maxence    (501) staff       (20)      149 2023-07-12 03:30:52.000000 understar-0.2.4/understar/system/lib/__init__.py
--rw-r--r--   0 maxence    (501) staff       (20)     5512 2023-07-13 02:32:11.000000 understar-0.2.4/understar/system/lib/app.py
--rw-r--r--   0 maxence    (501) staff       (20)     1015 2023-06-23 09:10:23.000000 understar-0.2.4/understar/system/lib/com.py
--rw-r--r--   0 maxence    (501) staff       (20)    11757 2023-06-19 00:59:20.000000 understar-0.2.4/understar/system/lib/event.py
--rw-r--r--   0 maxence    (501) staff       (20)     3784 2023-06-19 05:27:26.000000 understar-0.2.4/understar/system/lib/save.py
--rw-r--r--   0 maxence    (501) staff       (20)     2402 2023-06-25 03:39:17.000000 understar-0.2.4/understar/system/lib/store.py
--rw-r--r--   0 maxence    (501) staff       (20)      174 2023-06-23 09:10:04.000000 understar-0.2.4/understar/system/lib/types.py
--rw-r--r--   0 maxence    (501) staff       (20)     4978 2023-07-12 03:07:24.000000 understar-0.2.4/understar/system/lib/utils.py
--rw-r--r--   0 maxence    (501) staff       (20)    31301 2023-07-16 04:52:59.000000 understar-0.2.4/understar/understar.py
-drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-16 05:00:25.116111 understar-0.2.4/understar.egg-info/
--rw-r--r--   0 maxence    (501) staff       (20)      591 2023-07-16 05:00:25.000000 understar-0.2.4/understar.egg-info/PKG-INFO
--rw-r--r--   0 maxence    (501) staff       (20)      755 2023-07-16 05:00:25.000000 understar-0.2.4/understar.egg-info/SOURCES.txt
--rw-r--r--   0 maxence    (501) staff       (20)        1 2023-07-16 05:00:25.000000 understar-0.2.4/understar.egg-info/dependency_links.txt
--rw-r--r--   0 maxence    (501) staff       (20)       49 2023-07-16 05:00:25.000000 understar-0.2.4/understar.egg-info/requires.txt
--rw-r--r--   0 maxence    (501) staff       (20)       10 2023-07-16 05:00:25.000000 understar-0.2.4/understar.egg-info/top_level.txt
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-19 04:53:08.392839 understar-2.32/
+-rw-r--r--   0 maxence    (501) staff       (20)     1188 2023-05-26 01:06:57.000000 understar-2.32/LICENSE.md
+-rw-r--r--   0 maxence    (501) staff       (20)      590 2023-07-19 04:53:08.392709 understar-2.32/PKG-INFO
+-rw-r--r--   0 maxence    (501) staff       (20)       45 2023-05-26 01:06:57.000000 understar-2.32/README.md
+-rw-r--r--   0 maxence    (501) staff       (20)       38 2023-07-19 04:53:08.392922 understar-2.32/setup.cfg
+-rw-r--r--   0 maxence    (501) staff       (20)     1293 2023-07-19 02:00:27.000000 understar-2.32/setup.py
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-19 04:53:08.386520 understar-2.32/understar/
+-rw-r--r--   0 maxence    (501) staff       (20)       25 2023-07-19 04:14:38.000000 understar-2.32/understar/__init__.py
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-19 04:53:08.388134 understar-2.32/understar/system/
+-rw-r--r--   0 maxence    (501) staff       (20)       22 2023-07-16 04:49:43.000000 understar-2.32/understar/system/__init__.py
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-19 04:53:08.388445 understar-2.32/understar/system/app/
+-rw-r--r--   0 maxence    (501) staff       (20)       89 2023-07-16 04:47:12.000000 understar-2.32/understar/system/app/__init__.py
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-19 04:53:08.388716 understar-2.32/understar/system/app/config/
+-rw-r--r--   0 maxence    (501) staff       (20)    20066 2023-07-19 04:34:41.000000 understar-2.32/understar/system/app/config/__init__.py
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-19 04:53:08.389673 understar-2.32/understar/system/app/config/apt/
+-rw-r--r--   0 maxence    (501) staff       (20)       32 2023-07-12 03:26:34.000000 understar-2.32/understar/system/app/config/apt/__init__.py
+-rw-r--r--   0 maxence    (501) staff       (20)     3351 2023-07-19 04:34:43.000000 understar-2.32/understar/system/app/config/apt/install.py
+-rw-r--r--   0 maxence    (501) staff       (20)     1329 2023-07-19 04:34:44.000000 understar-2.32/understar/system/app/config/apt/uninstall.py
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-19 04:53:08.389960 understar-2.32/understar/system/app/maintenance/
+-rw-r--r--   0 maxence    (501) staff       (20)      902 2023-07-19 04:34:46.000000 understar-2.32/understar/system/app/maintenance/__init__.py
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-19 04:53:08.392285 understar-2.32/understar/system/lib/
+-rw-r--r--   0 maxence    (501) staff       (20)      149 2023-07-12 03:30:52.000000 understar-2.32/understar/system/lib/__init__.py
+-rw-r--r--   0 maxence    (501) staff       (20)     5517 2023-07-19 02:04:00.000000 understar-2.32/understar/system/lib/app.py
+-rw-r--r--   0 maxence    (501) staff       (20)     1015 2023-06-23 09:10:23.000000 understar-2.32/understar/system/lib/com.py
+-rw-r--r--   0 maxence    (501) staff       (20)    11757 2023-06-19 00:59:20.000000 understar-2.32/understar/system/lib/event.py
+-rw-r--r--   0 maxence    (501) staff       (20)     3784 2023-06-19 05:27:26.000000 understar-2.32/understar/system/lib/save.py
+-rw-r--r--   0 maxence    (501) staff       (20)     2716 2023-07-19 04:01:29.000000 understar-2.32/understar/system/lib/store.py
+-rw-r--r--   0 maxence    (501) staff       (20)      174 2023-06-23 09:10:04.000000 understar-2.32/understar/system/lib/types.py
+-rw-r--r--   0 maxence    (501) staff       (20)     5138 2023-07-19 00:40:50.000000 understar-2.32/understar/system/lib/utils.py
+-rw-r--r--   0 maxence    (501) staff       (20)    31108 2023-07-19 04:20:00.000000 understar-2.32/understar/understar.py
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-19 04:53:08.387913 understar-2.32/understar.egg-info/
+-rw-r--r--   0 maxence    (501) staff       (20)      590 2023-07-19 04:53:08.000000 understar-2.32/understar.egg-info/PKG-INFO
+-rw-r--r--   0 maxence    (501) staff       (20)      755 2023-07-19 04:53:08.000000 understar-2.32/understar.egg-info/SOURCES.txt
+-rw-r--r--   0 maxence    (501) staff       (20)        1 2023-07-19 04:53:08.000000 understar-2.32/understar.egg-info/dependency_links.txt
+-rw-r--r--   0 maxence    (501) staff       (20)       49 2023-07-19 04:53:08.000000 understar-2.32/understar.egg-info/requires.txt
+-rw-r--r--   0 maxence    (501) staff       (20)       10 2023-07-19 04:53:08.000000 understar-2.32/understar.egg-info/top_level.txt
```

### Comparing `understar-0.2.4/LICENSE.md` & `understar-2.32/LICENSE.md`

 * *Files identical despite different names*

### Comparing `understar-0.2.4/PKG-INFO` & `understar-2.32/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: understar
-Version: 0.2.4
+Version: 2.32
 Summary: A discord bot framewrok
 Home-page: https://github.com/GalTechDev/UnderStar-OS
 Download-URL: https://github.com/GalTechDev/UnderStar-OS/tarball/master
 Author: GalTech
 Author-email: poussigalitv@gmail.com
 License: MIT
 Keywords: discord,bot,discord.py,understar,os,framework
```

### Comparing `understar-0.2.4/setup.py` & `understar-2.32/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as stream:
     long_description = stream.read()
+    
+with open(".version", "r") as stream:
+    ver = stream.read()
 
 # long_description = "An universal wrapper (and useful tool) to make event / commands in python"
 
 setup(
     name='understar',
-    version="0.2.4",
+    version=f"{ver}",
     url='https://github.com/GalTechDev/UnderStar-OS',
     download_url='https://github.com/GalTechDev/UnderStar-OS/tarball/master',
     license='MIT',
     author='GalTech',
     author_email='poussigalitv@gmail.com',
     description='A discord bot framewrok',
     long_description=long_description,
```

### Comparing `understar-0.2.4/understar/system/app/config/__init__.py` & `understar-2.32/understar/system/app/config/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from os import execv, path
 from sys import executable, argv
 import discord 
 from .apt import install, uninstall
 
 
 Lib = lib.App()
-
+Lib.app.fusion([install, uninstall])
 """class lang_select(discord.ui.Select):
     def __init__(self) -> None:
         super().__init__(placeholder=f"{Lib.get_lang_ref(10, langage)}",max_values=1,min_values=1,options=[discord.SelectOption(label=lang,description="100%") for lang in Lib.get_lang_ref(all_lang_ref, langage)])
 
     async def callback(self, interaction: discord.Interaction):
         langage = self.values[0]
         embed = discord.Embed(title=f"{Lib.get_lang_ref(11, langage)}", description=f"{Lib.get_lang_ref(10, langage)}", color=discord.Color.blue())
@@ -201,15 +201,15 @@
         else:
             self.add_item(self.Add_to_serv(app=app, label="Ajouter au server", style=discord.ButtonStyle.primary, disabled=self.instaled))
 
         if owner.id == ctx.user.id:
             if self.downloaded:
                 self.add_item(self.Delete(app=app, label="Supprimer", style=discord.ButtonStyle.danger, disabled=(not self.downloaded)))
             else:
-                self.add_item(self.Download(app=app, label="Télécharger", style=discord.ButtonStyle.primary, disabled=self.downloaded))
+                self.add_item(self.Download(app=app, label="Télécharger", style=discord.ButtonStyle.primary, disabled= (self.downloaded or not Lib.store.get_link(app))))
             self.add_item(self.Set_app_link(app=app, label="Changer le lien", style=discord.ButtonStyle.gray))
             self.add_item(self.Del_app_link(app=app, label="Supprimer le lien", style=discord.ButtonStyle.danger))
 
         if self.downloaded and self.instaled:
             self.add_item(self.Config_app(app=app, label="Config", style=discord.ButtonStyle.primary, disabled=(Lib.store.get_installed()[self.app]==None or Lib.store.get_installed()[self.app].Lib.app.conf_com==None)))
 
     async def reload(self):
```

### Comparing `understar-0.2.4/understar/system/app/config/apt/install.py` & `understar-2.32/understar/system/app/config/apt/install.py`

 * *Files identical despite different names*

### Comparing `understar-0.2.4/understar/system/app/config/apt/uninstall.py` & `understar-2.32/understar/system/app/config/apt/uninstall.py`

 * *Files identical despite different names*

### Comparing `understar-0.2.4/understar/system/app/maintenance/__init__.py` & `understar-2.32/understar/system/app/maintenance/__init__.py`

 * *Files identical despite different names*

### Comparing `understar-0.2.4/understar/system/lib/app.py` & `understar-2.32/understar/system/lib/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,34 +17,34 @@
     def __init__(self) -> None:
         self.app = App()
         self.app_name = ""
         self.client: discord_commands.bot = None
         self.store = App_store(None)
         self.save = Save(self.app_name)
         self.guilds = Guilds()
-        self.store.installed_app = self.get_apps()
         self.event = Event()
 
 
     def set_app_name(self, app_name: str) -> None:
         """"""
         self.app_name = app_name
         self.save.app_name = app_name
         self.app_path = f"app/{app_name}/"
         if self.app.fusioned:
             for mod in self.app.fusioned_module:
                 mod.Lib.set_app_name(app_name)
 
-    def init(self, bot_client: discord_commands.Bot, tasks):
+    def init(self, bot_client: discord_commands.Bot, tasks, installed_app):
         """"""
         self.client = bot_client
         self.tasks = tasks
+        self.store = App_store(installed_app)
         if self.app.fusioned:
             for app in self.app.fusioned_module:
-                app.Lib.init(bot_client, tasks)
+                app.Lib.init(bot_client, tasks, installed_app)
 
     def is_in_guild(self, ctx:discord_commands.Context):
         guild_id = ctx.guild.id
         
 
     def is_in_staff(self, ctx:Interaction | discord_commands.Context, direct_author=False):
         """"""
@@ -97,16 +97,15 @@
 
     async def change_presence(self, activity, status):
         """"""
         await self.client.change_presence(activity=activity, status=status)
         
     def get_apps(self) -> dict:
         """"""
-        all_app=import_module("app")
-        return all_app
+        return self.store.installed_app
 
 class App:
     """"""
     def __init__(self) -> None:
         self.commands = []
         self.slashs = []
         self.all_tasks = []
```

### Comparing `understar-0.2.4/understar/system/lib/com.py` & `understar-2.32/understar/system/lib/com.py`

 * *Files identical despite different names*

### Comparing `understar-0.2.4/understar/system/lib/event.py` & `understar-2.32/understar/system/lib/event.py`

 * *Files identical despite different names*

### Comparing `understar-0.2.4/understar/system/lib/save.py` & `understar-2.32/understar/system/lib/save.py`

 * *Files identical despite different names*

### Comparing `understar-0.2.4/understar/system/lib/store.py` & `understar-2.32/understar/system/lib/store.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         """Give a dict object {"app_name":"app_link",}"""
         with open("save/system/app_store.json") as file:
             data = json.load(file)
         return data
 
     def get_installed(self):
         """"""
-        return self.installed_app.all_app
+        return self.installed_app
 
     def is_in_store(self, app_name: str) -> bool:
         """"""
         apps = self.get_apps()
         return app_name in list(apps.keys())
 
     def is_downloaded(self, app_name: str) -> bool:
@@ -34,14 +34,25 @@
             data = json.load(file)
             
         guilds = []
         for guild_id in data.keys():
             if app_name in data[str(guild_id)]["apps"]:
                 guilds.append(int(guild_id))
         return guilds
+    
+    def get_link(self, app_name: str) -> str:
+        file_path="save/system/app_store.json"
+        with open(file_path) as file:
+            store = json.load(file)
+
+        if not (app_name in store.keys()):
+            return None
+        else: 
+            app_link = store[app_name]
+            return app_link
 
     def add_link(self, app_name: str, app_link: str) -> None:
         file_path="save/system/app_store.json"
         with open(file_path) as file:
             store = json.load(file)
 
         if app_name in store.keys():
```

### Comparing `understar-0.2.4/understar/system/lib/utils.py` & `understar-2.32/understar/system/lib/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 import discord
 from .types import *
 import json
 import importlib
 import glob
 import os
+import pkg_resources
 
 LANGAGE = "fr"
 
 THEME = {"gris": discord.Color.dark_grey, "bleu": discord.Color.blue, "rouge": discord.Color.red, "vert": discord.Color.green, "jaune":discord.Color.yellow}
 
 async def valide_intaraction(interaction: discord.Interaction):
     try:
         await interaction.response.send_message()
     except Exception as error:
         pass
 
-with open(".version") as f:
+chemin_fichier = pkg_resources.resource_filename(__name__, '.version')
+
+with open(chemin_fichier.removesuffix("understar2/system/lib/.version")+".version", 'r') as f:
     BOT_VERSION = f.read()
 
 def import_module(folder: str, log=False, catch_error=True):
     # Parcours des apps dans le répertoire du package
     if log:
         print(f" * Import Module Start :")
     modules = {}
```

### Comparing `understar-0.2.4/understar/understar.py` & `understar-2.32/understar/understar.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,19 +20,19 @@
 APP_FOLDER = "app"
 BOT_TOKEN_PATH = f"{TOKEN_FOLDER}/bot_token"
 PREFIX = "?"
 CODING = "utf-8"
 
 programmer = os.path.basename(sys.argv[0])
 
-
-
 class OS:
     
     Lib = App()
+    all_app = import_module("app")
+    
     vals = [DOWNLOAD_FOLDER, TOKEN_FOLDER, SAVE_FOLDER, SAVE_APP_FOLDER, APP_FOLDER]
     for name in vals:
         Path(name).mkdir(exist_ok=True)
         
     BOT_TOKEN = ""
     
     intents = discord.Intents.all()
@@ -45,18 +45,19 @@
     timer = time.time()
        
     def start(self):
         self.client.run(self.BOT_TOKEN)
          
     async def import_apps(self, sys :bool=False) -> None:
         """"""
-        for app_name,app in (self.Lib.get_apps().items() if not sys else sys_app.all_app.items()):
+        #print((self.all_app.items() if not sys else sys_app.all_app.items()))
+        for app_name,app in (self.all_app.items() if not sys else sys_app.all_app.items()):
             print(f"\n * IMPORT {app_name}: ")
 
-            app.Lib.init(self.client, discord_tasks)
+            app.Lib.init(self.client, discord_tasks, self.all_app)
             app.Lib.set_app_name(app_name)
             if not os.path.exists(os.path.join(app.Lib.save.save_path, app_name)):
                 os.mkdir(os.path.join(app.Lib.save.save_path, app_name))
 
             # Task
 
             loaded = 0
@@ -214,28 +215,28 @@
             await ctx.send(":pizza:")
 
 
         @client.command(name="os-ping", aliases=["os-ver", "ver", "ping"], help="Donne des infos sur le bot")
         @discord_commands.check(Lib.is_in_staff)
         async def version(ctx:discord_commands.context.Context):
             embed = discord.Embed(title="INFO")
-            embed.add_field(name=f"Version :", value=f"` {BOT_VERSION}   `")
-            embed.add_field(name=f"Ping :", value=f"` {round(client.latency * 1000)} `")
-            embed.add_field(name=f"Time up :", value=f"`{convert_time(int(time.time()-self.timer))}`")
+            embed.add_field(name=f"Version :", value=f"`{BOT_VERSION}`")
+            embed.add_field(name=f"Ping :", value=f"` {round(self.client.latency * 1000)} `")
+            embed.add_field(name=f"Time up :", value=f"<t:{int(self.timer)}:R>")
             await ctx.send(embed=embed)
 
 
         @client.command(name="os-help", aliases=["help"], help="Pour avoir ce message")
         async def help(ctx:discord_commands.context.Context,*args):
             if args==():
                 await ctx.send(embeds=self.get_help(ctx))
             else :
-                if args[0] in Lib.get_apps().keys():
+                if args[0] in self.all_app.keys():
                     sys_com = False
-                    com = Lib.get_apps()
+                    com = self.all_app
                 elif args[0] in sys_app.all_app:
                     sys_com = True
                     com = sys_app.all_app
                 else:
                     return
                 if len(args)==1:
                     try:
@@ -264,15 +265,15 @@
                     except Exception as error:
                         print(error)
 
         # ---------------------------------- EVENTS ------------------------------------
 
         #@terminal()
         async def manage_event(command, *args, **kwargs):
-            for app in list(Lib.get_apps().values()) + list(sys_app.all_app.values()):
+            for app in list(self.all_app.values()) + list(sys_app.all_app.values()):
                 if app:
                     data = getattr(app.Lib.event, command)
                     await data(*args, **kwargs)
                     if app.Lib.app.fusioned:
                         for sub_app in app.Lib.app.fusioned_module:
                             data = getattr(sub_app.Lib.event, command)
                             await data(*args, **kwargs)
@@ -413,26 +414,19 @@
 
             change_status.start()
 
             #maintenance.start()
             await self.import_apps(True)
             await self.import_apps()
 
-            with open(f'{SYS_FOLDER}/icon.png', 'rb') as image:
-                pass
-                #await client.user.edit(avatar=image.read())
             print("\n * Bot Starting...")
             print(" * version : ", programmer, BOT_VERSION)
             print(" * Logged in as : ", client.user.name)
             print(" * ID : ", client.user.id)
-            #await import_apps(True)
-            #await import_apps()
-
-            #await sync(client, "sync" in sys.argv)
-            #print(client.guilds)
+            
             await client.tree.sync()
 
             with open(f"{SAVE_FOLDER}/{SYS_FOLDER}/guilds.json") as f:
                 data = json.load(f)
 
             for guild in client.guilds:
                 if "sync" in sys.argv:
```

### Comparing `understar-0.2.4/understar.egg-info/PKG-INFO` & `understar-2.32/understar.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: understar
-Version: 0.2.4
+Version: 2.32
 Summary: A discord bot framewrok
 Home-page: https://github.com/GalTechDev/UnderStar-OS
 Download-URL: https://github.com/GalTechDev/UnderStar-OS/tarball/master
 Author: GalTech
 Author-email: poussigalitv@gmail.com
 License: MIT
 Keywords: discord,bot,discord.py,understar,os,framework
```

### Comparing `understar-0.2.4/understar.egg-info/SOURCES.txt` & `understar-2.32/understar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

