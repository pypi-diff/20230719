# Comparing `tmp/claude-api-1.0.5.tar.gz` & `tmp/claude-api-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "claude-api-1.0.5.tar", last modified: Mon Jul 17 07:06:06 2023, max compression
+gzip compressed data, was "claude-api-1.0.6.tar", last modified: Wed Jul 19 02:23:40 2023, max compression
```

## Comparing `claude-api-1.0.5.tar` & `claude-api-1.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 07:06:06.217369 claude-api-1.0.5/
--rw-rw-rw-   0        0        0     1094 2023-07-17 06:55:41.000000 claude-api-1.0.5/LICENSE
--rw-rw-rw-   0        0        0     4642 2023-07-17 07:06:06.217369 claude-api-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     3824 2023-07-17 06:55:41.000000 claude-api-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 07:06:06.195729 claude-api-1.0.5/claude-api/
-drwxrwxrwx   0        0        0        0 2023-07-17 07:06:06.211415 claude-api-1.0.5/claude-api/claude_api.egg-info/
--rw-rw-rw-   0        0        0     4642 2023-07-17 07:06:06.000000 claude-api-1.0.5/claude-api/claude_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-07-17 07:06:06.000000 claude-api-1.0.5/claude-api/claude_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 07:06:06.000000 claude-api-1.0.5/claude-api/claude_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-17 07:06:06.000000 claude-api-1.0.5/claude-api/claude_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-17 07:06:06.000000 claude-api-1.0.5/claude-api/claude_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7623 2023-07-17 07:04:57.000000 claude-api-1.0.5/claude-api/claude_api.py
--rw-rw-rw-   0        0        0       42 2023-07-17 07:06:06.217369 claude-api-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1258 2023-07-17 07:05:56.000000 claude-api-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 02:23:40.692667 claude-api-1.0.6/
+-rw-rw-rw-   0        0        0     1094 2023-07-19 02:20:29.000000 claude-api-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0     4698 2023-07-19 02:23:40.689982 claude-api-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3880 2023-07-19 02:20:29.000000 claude-api-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-19 02:23:40.667912 claude-api-1.0.6/claude-api/
+drwxrwxrwx   0        0        0        0 2023-07-19 02:23:40.688335 claude-api-1.0.6/claude-api/claude_api.egg-info/
+-rw-rw-rw-   0        0        0     4698 2023-07-19 02:23:40.000000 claude-api-1.0.6/claude-api/claude_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-07-19 02:23:40.000000 claude-api-1.0.6/claude-api/claude_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 02:23:40.000000 claude-api-1.0.6/claude-api/claude_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-19 02:23:40.000000 claude-api-1.0.6/claude-api/claude_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-19 02:23:40.000000 claude-api-1.0.6/claude-api/claude_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7647 2023-07-19 02:20:29.000000 claude-api-1.0.6/claude-api/claude_api.py
+-rw-rw-rw-   0        0        0       42 2023-07-19 02:23:40.692667 claude-api-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1258 2023-07-19 02:23:12.000000 claude-api-1.0.6/setup.py
```

### Comparing `claude-api-1.0.5/LICENSE` & `claude-api-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `claude-api-1.0.5/PKG-INFO` & `claude-api-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: claude-api
-Version: 1.0.5
+Version: 1.0.6
 Summary: An unofficial API for Claude AI, allowing users to access and interact with Claude AII
 Home-page: https://github.com/KoushikNavuluri/Claude-API/
 Author: Koushik
 Author-email: koushikk@outlook.com
 License: MIT
 Keywords: claude,ai,claude-ai,API,requests,chatbot
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,15 +20,15 @@
 License-File: LICENSE
 
 # Claude AI-API ( Unofficial )
 This project provides an unofficial API for Claude AI, allowing users to access and interact with Claude AI .
 
 ## Use Cases 
 
-    1. Python Console ChatBot
+    1. Python Console ChatBot ( Check in usecases folder for sample console chatbot )
 
     2. Discord Chatbot   
     
     3. Many more can be done....
     
 
 ## Prerequisites
```

### Comparing `claude-api-1.0.5/README.md` & `claude-api-1.0.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Claude AI-API ( Unofficial )
 This project provides an unofficial API for Claude AI, allowing users to access and interact with Claude AI .
 
 ## Use Cases 
 
-    1. Python Console ChatBot
+    1. Python Console ChatBot ( Check in usecases folder for sample console chatbot )
 
     2. Discord Chatbot   
     
     3. Many more can be done....
     
 
 ## Prerequisites
```

### Comparing `claude-api-1.0.5/claude-api/claude_api.egg-info/PKG-INFO` & `claude-api-1.0.6/claude-api/claude_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: claude-api
-Version: 1.0.5
+Version: 1.0.6
 Summary: An unofficial API for Claude AI, allowing users to access and interact with Claude AII
 Home-page: https://github.com/KoushikNavuluri/Claude-API/
 Author: Koushik
 Author-email: koushikk@outlook.com
 License: MIT
 Keywords: claude,ai,claude-ai,API,requests,chatbot
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,15 +20,15 @@
 License-File: LICENSE
 
 # Claude AI-API ( Unofficial )
 This project provides an unofficial API for Claude AI, allowing users to access and interact with Claude AI .
 
 ## Use Cases 
 
-    1. Python Console ChatBot
+    1. Python Console ChatBot ( Check in usecases folder for sample console chatbot )
 
     2. Discord Chatbot   
     
     3. Many more can be done....
     
 
 ## Prerequisites
```

### Comparing `claude-api-1.0.5/claude-api/claude_api.py` & `claude-api-1.0.6/claude-api/claude_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,17 @@
     self.organization_id = self.get_organization_id()
 
   def get_organization_id(self):
     url = "https://claude.ai/api/organizations"
   
     headers = {
       'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/115.0',
+      'Accept': '*/*',
       'Accept-Language': 'en-US,en;q=0.5',
+      'Accept-Encoding': 'gzip, deflate, br',
       'Referer': 'https://claude.ai/chats',
       'Content-Type': 'application/json',
       'Sec-Fetch-Dest': 'empty',
       'Sec-Fetch-Mode': 'cors',
       'Sec-Fetch-Site': 'same-origin',
       'Connection': 'keep-alive',
       'Cookie': f'{self.cookie}'
@@ -73,15 +75,14 @@
       "attachments": []
     })
     headers = {
       'User-Agent':
       'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/115.0',
       'Accept': 'text/event-stream, text/event-stream',
       'Accept-Language': 'en-US,en;q=0.5',
-      'Accept-Encoding': 'gzip, deflate, br',
       'Referer': 'https://claude.ai/chats',
       'Content-Type': 'application/json',
       'Origin': 'https://claude.ai',
       'DNT': '1',
       'Connection': 'keep-alive',
       'Cookie': f'{self.cookie}',
       'Sec-Fetch-Dest': 'empty',
```

### Comparing `claude-api-1.0.5/setup.py` & `claude-api-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 base_path = Path(__file__).parent
 long_description = (base_path / "README.md").read_text()
 
 
 setup(
     name='claude-api', 
-    version='1.0.5',  
+    version='1.0.6',  
     author='Koushik',
     license="MIT",
     author_email='koushikk@outlook.com',
     description='An unofficial API for Claude AI, allowing users to access and interact with Claude AII',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/KoushikNavuluri/Claude-API/',
```

