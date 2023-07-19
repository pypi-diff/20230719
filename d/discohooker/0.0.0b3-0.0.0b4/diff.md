# Comparing `tmp/discohooker-0.0.0b3.tar.gz` & `tmp/discohooker-0.0.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discohooker-0.0.0b3.tar", last modified: Wed Jul 19 15:47:40 2023, max compression
+gzip compressed data, was "discohooker-0.0.0b4.tar", last modified: Wed Jul 19 16:01:51 2023, max compression
```

## Comparing `discohooker-0.0.0b3.tar` & `discohooker-0.0.0b4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-19 15:47:40.454357 discohooker-0.0.0b3/
--rw-r--r--   0 runner    (1000) runner    (1000)     1066 2023-07-17 08:42:29.000000 discohooker-0.0.0b3/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)     1113 2023-07-19 15:47:40.450357 discohooker-0.0.0b3/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      647 2023-07-19 15:15:07.000000 discohooker-0.0.0b3/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-19 15:47:40.450357 discohooker-0.0.0b3/discohooker/
--rw-r--r--   0 runner    (1000) runner    (1000)       92 2023-07-19 13:55:35.000000 discohooker-0.0.0b3/discohooker/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     3670 2023-07-19 15:47:07.000000 discohooker-0.0.0b3/discohooker/embed.py
--rw-r--r--   0 runner    (1000) runner    (1000)      278 2023-07-19 15:15:06.000000 discohooker-0.0.0b3/discohooker/errors.py
--rw-r--r--   0 runner    (1000) runner    (1000)     4844 2023-07-19 15:15:06.000000 discohooker-0.0.0b3/discohooker/webhook.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-19 15:47:40.450357 discohooker-0.0.0b3/discohooker.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1113 2023-07-19 15:47:39.000000 discohooker-0.0.0b3/discohooker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      305 2023-07-19 15:47:39.000000 discohooker-0.0.0b3/discohooker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-19 15:47:39.000000 discohooker-0.0.0b3/discohooker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       23 2023-07-19 15:47:39.000000 discohooker-0.0.0b3/discohooker.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       12 2023-07-19 15:47:39.000000 discohooker-0.0.0b3/discohooker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)      472 2023-07-15 08:52:33.000000 discohooker-0.0.0b3/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-19 15:47:40.454357 discohooker-0.0.0b3/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      714 2023-07-19 15:47:29.000000 discohooker-0.0.0b3/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-19 16:01:51.936642 discohooker-0.0.0b4/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1066 2023-07-17 08:42:29.000000 discohooker-0.0.0b4/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     1113 2023-07-19 16:01:51.936642 discohooker-0.0.0b4/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      647 2023-07-19 15:15:07.000000 discohooker-0.0.0b4/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-19 16:01:51.936642 discohooker-0.0.0b4/discohooker/
+-rw-r--r--   0 runner    (1000) runner    (1000)       92 2023-07-19 13:55:35.000000 discohooker-0.0.0b4/discohooker/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3723 2023-07-19 16:01:13.000000 discohooker-0.0.0b4/discohooker/embed.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      278 2023-07-19 15:15:06.000000 discohooker-0.0.0b4/discohooker/errors.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     4925 2023-07-19 15:59:32.000000 discohooker-0.0.0b4/discohooker/webhook.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-19 16:01:51.936642 discohooker-0.0.0b4/discohooker.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1113 2023-07-19 16:01:51.000000 discohooker-0.0.0b4/discohooker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      305 2023-07-19 16:01:51.000000 discohooker-0.0.0b4/discohooker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-19 16:01:51.000000 discohooker-0.0.0b4/discohooker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       23 2023-07-19 16:01:51.000000 discohooker-0.0.0b4/discohooker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       12 2023-07-19 16:01:51.000000 discohooker-0.0.0b4/discohooker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)      472 2023-07-15 08:52:33.000000 discohooker-0.0.0b4/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-19 16:01:51.936642 discohooker-0.0.0b4/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      714 2023-07-19 16:01:41.000000 discohooker-0.0.0b4/setup.py
```

### Comparing `discohooker-0.0.0b3/LICENSE` & `discohooker-0.0.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `discohooker-0.0.0b3/PKG-INFO` & `discohooker-0.0.0b4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discohooker
-Version: 0.0.0b3
+Version: 0.0.0b4
 Summary: A easy PyPI to send Discord Webhook!
 Home-page: https://replit.com/@MAX110331/discohooker
 Author: MaxPython110331
 Author-email: max.gamil110331@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `discohooker-0.0.0b3/README.md` & `discohooker-0.0.0b4/README.md`

 * *Files identical despite different names*

### Comparing `discohooker-0.0.0b3/discohooker/embed.py` & `discohooker-0.0.0b4/discohooker/embed.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,17 +31,20 @@
 
 
 class Embed:
     def __init__(self, title: str=None, description: str=None, colour: str=0xffffff, url: str=None, fields: list[EmbedField]=[], timestamp: datetime=None):
         self.title=title
         self.description=description
         self.colour=colour
-        if not url.startswith("https://") and url != None:
+        if url == None:
+            self.url=url
+        elif not url.startswith("https://"):
             raise Errors.URLError("This is not URL! Please check and change your URL!")
-        self.url=url
+        else:
+            self.url=url
         self.fields=fields
         self.timestamp=timestamp
         self._image={}
         self._thumbnail={}
         self._author={}
         self._footer={}
```

### Comparing `discohooker-0.0.0b3/discohooker/webhook.py` & `discohooker-0.0.0b4/discohooker/webhook.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,32 +5,35 @@
 import requests
 
 
 class Webhook:
     def __init__(self, weburl: str, name: str=None, avatar_url: str=None):
         if not weburl.startswith("https://discord.com/api/webhooks/"):
             raise Errors.WebhookURLError("This is not Discord Webhook URL! Please check your URL and change the URL to the correct URL!")
-        if not avatar_url.startswith("https:") and avatar_url != None:
+        response=requests.get(weburl).json()
+        if avatar_url == None:
+            self.avatar_url=response["avatar_url"]
+        elif not avatar_url.startswith("https://"):
             raise Errors.URLError("This is not URL! Please check and change your URL!")
+        else:
+            self.avatar_url=avatar_url
         self.weburl=weburl
-        response=requests.get(weburl).json()
         if  self.name == None:
             self.name=response["name"]
         else:
             self.name=name
         self.id=response["id"]
         self.mention=f"<@{self.id}>"
         self.token=response["token"]
         if response["application_id"] == None:
             self.application_id=0
         else:
             self.application_id=response["application_id"]
         self.channel_id=response["channel_id"]
         self.guild_id=response["guild_id"]
-        self.avatar_url=avatar_url
         self.json=response
 
 
     @property
     def url(self):
         return self.weburl
```

### Comparing `discohooker-0.0.0b3/discohooker.egg-info/PKG-INFO` & `discohooker-0.0.0b4/discohooker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discohooker
-Version: 0.0.0b3
+Version: 0.0.0b4
 Summary: A easy PyPI to send Discord Webhook!
 Home-page: https://replit.com/@MAX110331/discohooker
 Author: MaxPython110331
 Author-email: max.gamil110331@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `discohooker-0.0.0b3/setup.py` & `discohooker-0.0.0b4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="discohooker",
-    version="0.0.0b3",
+    version="0.0.0b4",
     author="MaxPython110331",
     author_email="max.gamil110331@gmail.com",
     description="A easy PyPI to send Discord Webhook!",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://replit.com/@MAX110331/discohooker",
```

