# Comparing `tmp/mutual-0.1.1.tar.gz` & `tmp/mutual-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mutual-0.1.1.tar", last modified: Fri Jul 14 09:10:31 2023, max compression
+gzip compressed data, was "mutual-0.1.2.tar", last modified: Wed Jul 19 07:30:22 2023, max compression
```

## Comparing `mutual-0.1.1.tar` & `mutual-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-14 09:10:31.046095 mutual-0.1.1/
--rw-r--r--   0 alexbetita   (501) staff       (20)     1068 2023-07-14 00:38:03.000000 mutual-0.1.1/LICENSE.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)     3776 2023-07-14 09:10:31.045928 mutual-0.1.1/PKG-INFO
--rw-r--r--   0 alexbetita   (501) staff       (20)     3349 2023-07-14 08:50:36.000000 mutual-0.1.1/README.md
-drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-14 09:10:31.044672 mutual-0.1.1/mutual/
--rw-r--r--   0 alexbetita   (501) staff       (20)     1560 2023-07-14 07:16:33.000000 mutual-0.1.1/mutual/Auth.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     6185 2023-07-14 08:22:10.000000 mutual-0.1.1/mutual/Bot.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     3694 2023-07-14 08:06:23.000000 mutual-0.1.1/mutual/Chat.py
--rw-r--r--   0 alexbetita   (501) staff       (20)      546 2023-07-14 08:11:54.000000 mutual-0.1.1/mutual/Dev.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     4229 2023-07-14 08:30:49.000000 mutual-0.1.1/mutual/Prompt.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     1403 2023-07-14 08:23:22.000000 mutual-0.1.1/mutual/__init__.py
-drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-14 09:10:31.045704 mutual-0.1.1/mutual.egg-info/
--rw-r--r--   0 alexbetita   (501) staff       (20)     3776 2023-07-14 09:10:31.000000 mutual-0.1.1/mutual.egg-info/PKG-INFO
--rw-r--r--   0 alexbetita   (501) staff       (20)      273 2023-07-14 09:10:31.000000 mutual-0.1.1/mutual.egg-info/SOURCES.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)        1 2023-07-14 09:10:31.000000 mutual-0.1.1/mutual.egg-info/dependency_links.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)        9 2023-07-14 09:10:31.000000 mutual-0.1.1/mutual.egg-info/requires.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)        7 2023-07-14 09:10:31.000000 mutual-0.1.1/mutual.egg-info/top_level.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)       38 2023-07-14 09:10:31.046140 mutual-0.1.1/setup.cfg
--rw-r--r--   0 alexbetita   (501) staff       (20)      727 2023-07-14 09:10:22.000000 mutual-0.1.1/setup.py
+drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-19 07:30:22.856367 mutual-0.1.2/
+-rw-r--r--   0 alexbetita   (501) staff       (20)     1068 2023-07-14 00:38:03.000000 mutual-0.1.2/LICENSE.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)     6408 2023-07-19 07:30:22.856216 mutual-0.1.2/PKG-INFO
+-rw-r--r--   0 alexbetita   (501) staff       (20)     5982 2023-07-19 07:20:58.000000 mutual-0.1.2/README.md
+drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-19 07:30:22.854949 mutual-0.1.2/mutual/
+-rw-r--r--   0 alexbetita   (501) staff       (20)      993 2023-07-19 07:15:27.000000 mutual-0.1.2/mutual/APIKey.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     1629 2023-07-19 07:15:42.000000 mutual-0.1.2/mutual/Auth.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     8915 2023-07-19 07:16:09.000000 mutual-0.1.2/mutual/Bot.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     4858 2023-07-19 07:16:20.000000 mutual-0.1.2/mutual/Chat.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)      602 2023-07-19 07:16:27.000000 mutual-0.1.2/mutual/Dev.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     3619 2023-07-19 07:16:46.000000 mutual-0.1.2/mutual/Judge.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     3649 2023-07-19 07:17:05.000000 mutual-0.1.2/mutual/JudgeMessage.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     3948 2023-07-19 07:17:24.000000 mutual-0.1.2/mutual/Prompt.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     4096 2023-07-19 06:46:45.000000 mutual-0.1.2/mutual/__init__.py
+drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-19 07:30:22.855983 mutual-0.1.2/mutual.egg-info/
+-rw-r--r--   0 alexbetita   (501) staff       (20)     6408 2023-07-19 07:30:22.000000 mutual-0.1.2/mutual.egg-info/PKG-INFO
+-rw-r--r--   0 alexbetita   (501) staff       (20)      329 2023-07-19 07:30:22.000000 mutual-0.1.2/mutual.egg-info/SOURCES.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)        1 2023-07-19 07:30:22.000000 mutual-0.1.2/mutual.egg-info/dependency_links.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)        9 2023-07-19 07:30:22.000000 mutual-0.1.2/mutual.egg-info/requires.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)        7 2023-07-19 07:30:22.000000 mutual-0.1.2/mutual.egg-info/top_level.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)       38 2023-07-19 07:30:22.856414 mutual-0.1.2/setup.cfg
+-rw-r--r--   0 alexbetita   (501) staff       (20)      727 2023-07-19 07:30:05.000000 mutual-0.1.2/setup.py
```

### Comparing `mutual-0.1.1/LICENSE.txt` & `mutual-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mutual-0.1.1/mutual/Auth.py` & `mutual-0.1.2/mutual/Auth.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import requests
 import json
 import mutual
 
-def signup(user_id, email):
+def signup(password = None, email = None):
     url = "https://api-agent.mutuai.io/api/signup"
+    # url = "http://127.0.0.1:8000/api/signup"
     data = {
-        "user_id": user_id,
+        "password": password,
         "email": email
     }
 
     headers = {
         'Content-Type': 'application/json'
     }
 
@@ -17,25 +18,25 @@
 
     if response.status_code < 300:
         response_json = response.json()
         mutual.api_key = response_json.get('api_key') # save the api_key to config
         return response_json
     else:
         return {
-            "user_id": None,
             "email": None,
             "api_key": None,
             "details":f"Request failed with status code {response.status_code}, with an Error Message: {json.loads(response.text)['detail'] or response.text}"
         }
 
 
-def login(user_id, email):
+def login(password = None, email = None):
     url = "https://api-agent.mutuai.io/api/login"
+    # url = "http://127.0.0.1:8000/api/login"
     data = {
-        "user_id": user_id,
+        "password": password,
         "email": email
     }
 
     headers = {
         'Content-Type': 'application/json'
     }
 
@@ -43,12 +44,11 @@
 
     if response.status_code < 300:
         response_json = response.json()
         mutual.api_key = response_json.get('api_key') # save the api_key to config
         return response_json
     else:
         return {
-            "user_id": None,
             "email": None,
             "api_key": None,
             "details":f"Request failed with status code {response.status_code}, with an Error Message: {json.loads(response.text)['detail'] or response.text}"
         }
```

### Comparing `mutual-0.1.1/mutual/Bot.py` & `mutual-0.1.2/mutual/Bot.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,151 +1,201 @@
 import requests
 import json
 import mutual
 
 bot_default_response = {
             "bot_id": None,
             "bot_name": None,
-            "bot_org": None,
+            # "bot_org": None,
             "bot_chat_index": None,
             "prompt_id": None,
+            "judge_id": None,
+            "judge_message_id": None,
             "details": None
         }
 
 def get_bots(limit=20, offset=0):
     url = f"https://api-agent.mutuai.io/api/bots?limit={limit}&offset={offset}"
+    # url = f"http://127.0.0.1:8000/api/bots?limit={limit}&offset={offset}"
     headers = {
         "Authorization": f"Bearer {mutual.api_key}"
     }
     response = requests.get(url, headers=headers)
     if response.status_code < 300:
         return response.json()
     else:
         bot_default_response["details"] = f"Request failed with status code {response.status_code}, with an Error Message: {json.loads(response.text)['detail'] or response.text}"
         return bot_default_response
 
-def get_bot(bot_id):
-    url = f"https://api-agent.mutuai.io/api/bots/{str(bot_id)}"
+def get_bot(bot_arg):
+    url = f"https://api-agent.mutuai.io/api/bots/{str(bot_arg)}"
+    # url = f"http://127.0.0.1:8000/api/bots/{str(bot_arg)}"
     headers = {
         "Authorization": f"Bearer {mutual.api_key}"
     }
     response = requests.get(url, headers=headers)
     # response.raise_for_status()  # Raise an exception if the response contains an HTTP error status code
     if response.status_code < 300:
         return response.json()
     else:
         bot_default_response["details"] = f"Request failed with status code {response.status_code}, with an Error Message: {json.loads(response.text)['detail'] or response.text}"
         return bot_default_response
 
-def create_bot(bot_name, bot_org = "Mutual", prompt_id = "default"):
+def create_bot(bot_name=None, prompt=None, prompt_id = "default", judge_id="default", judge_message_id="default"):
     url = "https://api-agent.mutuai.io/api/bots"
+    # url = "http://127.0.0.1:8000/api/bots"
     headers = {
         "Content-Type": "application/json",
         "Authorization": f"Bearer {mutual.api_key}"
     }
     data = {
-        # "bot_id": str(bot_id),
         "bot_name": bot_name,
-        "bot_org": bot_org,
-        "prompt_id": prompt_id
+        "prompt": prompt,
+        "prompt_id": prompt_id,
+        "judge_id": judge_id,
+        "judge_message_id": judge_message_id
     }
     response = requests.post(url, data=json.dumps(data), headers=headers)
     if response.status_code < 300:
         return response.json()
     else:
         bot_default_response["details"] = f"Request failed with status code {response.status_code}, with an Error Message: {json.loads(response.text)['detail'] or response.text}"
         return bot_default_response
 
-def update_bot(bot_id, bot_name=None, bot_org=None, prompt_id=None):
+def update_bot(bot_id=None, bot_name=None, prompt_id=None, judge_id=None, judge_message_id=None):
     url = f"https://api-agent.mutuai.io/api/bots/{str(bot_id)}"
+    # url = f"http://127.0.0.1:8000/api/bots/{str(bot_id)}"
     headers = {
         "Content-Type": "application/json",
         "Authorization": f"Bearer {mutual.api_key}"
     }
     data = {
         "bot_name": bot_name,
-        "bot_org": bot_org,
-        "prompt_id": prompt_id
+        "prompt_id": prompt_id,
+        "judge_id": judge_id,
+        "judge_message_id": judge_message_id
     }
     # remove keys with None value
     data = {k: v for k, v in data.items() if v is not None}
     response = requests.patch(url, data=json.dumps(data), headers=headers)
     if response.status_code < 300:
         return response.json()
     else:
         bot_default_response["details"] = f"Request failed with status code {response.status_code}, with an Error Message: {json.loads(response.text)['detail'] or response.text}"
         return bot_default_response
 
 
 class Bot:
-    def __init__(self, api_key, bot_id=None, bot_name=None, prompt_id = "default"):
+    def __init__(self, api_key, bot_id=None, bot_name=None, prompt_id = "default", judge_id="default", judge_message_id="default"):
         self.api_key = api_key
         self.bot_id = bot_id
         self.bot_name = bot_name
         self.prompt_id = prompt_id
+        self.judge_id = judge_id
+        self.judge_message_id = judge_message_id
+
+        #
+        self.flow = False
 
         self.default_stream_response = {
                         "error": None,
-                        "status": None,
+                        "status": "processing",
                         "content": None,
-                        "bot_id": None,
-                        "user_id": None,
-                        "new_bot": None,
-                        "new_bot_user": None,
-                        "prompt_id": None
-        }
+                        "data" : {
+                            "bot_data": {
+                                "bot_id": None,
+                                "new_bot": False,
+                                "new_bot_message": "Not a new bot.", 
+                                "new_bot_user": False,
+                                "new_bot_user_message": "Not a new bot_user.",
+                            },
+                            "prompt_data": {
+                                "prompt_id": None,
+                                "judge_id": None,
+                                "judge_message_id": None,
+                            },
+                            "user_data": {
+                                "username": None,
+                                "tokens_used" : None
+                            }
+                        },
+                    }
 
-    def updateBot(self, bot_name=None, bot_org=None, prompt_id=None):
+    def update_bot(self, bot_name=None, prompt_id=None, judge_id=None, judge_message_id=None):
         url = f"https://api-agent.mutuai.io/api/bots/{str(self.bot_id)}"
+        # url = f"http://127.0.0.1:8000/api/bots/{str(self.bot_id)}"
         headers = {
             "Content-Type": "application/json",
             "Authorization": f"Bearer {self.api_key}"
         }
         data = {
             "bot_name": bot_name,
-            "bot_org": bot_org,
-            "prompt_id": prompt_id
+            "prompt_id": prompt_id,
+            "judge_id" : judge_id,
+            "judge_message_id" : judge_message_id
         }
         # remove keys with None value
         data = {k: v for k, v in data.items() if v is not None}
         response = requests.patch(url, data=json.dumps(data), headers=headers)
         if response.status_code < 300:
             return response.json()
         else:
             self.default_stream_response["content"] = f"Request failed with status code {response.status_code}, with an Error Message: {json.loads(response.text)['detail'] or response.text}"
             return self.default_stream_response
 
-    def chat(self, content, username=None, multiplayer_memory = True, context_window = 2):
+    def chat(self, content=None, username=None, prompt=None, multiplayer_memory = True, context_window = 2, flow=False, error_logs=False):
         url = "https://api-agent.mutuai.io/api/chat"
+        # url = "http://127.0.0.1:8000/api/chat"
         headers = {
             "Content-Type": "application/json",
             "Authorization": f"Bearer {self.api_key}"
         }
         data = {
             "content": content,
             "bot_id": str(self.bot_id),
+            "bot_name": self.bot_name,
+            "prompt": prompt,
             "username": username,
             "prompt_id": self.prompt_id,
+            "judge_id": self.judge_id,
+            "judge_message_id": self.judge_message_id,
             "multiplayer": multiplayer_memory,
             "context_window": context_window
         }
 
         response = requests.post(url, data=json.dumps(data), headers=headers, stream=True)
 
         if response.status_code < 300:
             is_new_bot = False
             is_new_user = False
+
+            # add the newly created bot to the bot class
+            
+
             for line in response.iter_lines():
                 if line:  # filter out keep-alive new lines
                     json_data = json.loads(line)
-                    if json_data['new_bot'] and not is_new_bot:
+                    if not self.bot_id:
+                        self.bot_id = json_data['data']['bot_data']['bot_id']
+                    if json_data['error'] is not None and not error_logs:
+                        continue
+                    if json_data['data']['bot_data']['new_bot'] and not is_new_bot:
                         is_new_bot = True
-                        print(f"Newly created bot! Here is your id: {json_data['bot_id']}")
-                    if json_data['new_bot_user'] and not is_new_user:
+                        print(f"Newly created bot! Here is your id: {json_data['data']['bot_data']['bot_id']}")
+                    if json_data['data']['bot_data']['new_bot_user'] and not is_new_user:
                         is_new_user = True
-                        print(f"New user {json_data['user_id']} created interacting with bot id: {json_data['bot_id']}")
+                        print(f"New user {json_data['data']['user_data']['username']} created interacting with bot id: {json_data['data']['bot_data']['bot_id']}")
                     if json_data['content'] =='[close]':
                         continue
                     yield json_data
+
+            if flow or self.flow:
+                print("\n\n", end="", flush=True)
+                new_content = input("Please enter a new response or type exit to exit: ")
+                if new_content.strip().lower() == "exit":
+                    return
+                for msg in self.chat(content=new_content, username=username, prompt=prompt, multiplayer_memory=multiplayer_memory, context_window=context_window, flow=flow):
+                    yield msg
         else:
             self.default_stream_response['content'] = f"Request failed with status code {response.status_code}, with an Error Message: {json.loads(response.text)['detail'] or response.text}"
+            print(f"Request failed with status code {response.status_code}, with an Error Message: {json.loads(response.text)['detail'] or response.text}")
             return self.default_stream_response
```

### Comparing `mutual-0.1.1/mutual/Chat.py` & `mutual-0.1.2/mutual/Chat.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,77 +1,101 @@
 import requests
 import json
 import mutual
 
 default_stream_response = {
                         "error": None,
-                        "status": None,
+                        "status": "processing",
                         "content": None,
-                        "bot_id": None,
-                        "user_id": None,
-                        "new_bot": None,
-                        "new_bot_user": None,
-                        "prompt_id": None
-                        }
-
-def create(content, bot_id=None, username=None, prompt_id=None, error_logs=False, multiplayer_memory = True, context_window = 2):
+                        "data" : {
+                            "bot_data": {
+                                "bot_id": None,
+                                "new_bot": False,
+                                "new_bot_message": "Not a new bot.", 
+                                "new_bot_user": False,
+                                "new_bot_user_message": "Not a new bot_user.",
+                            },
+                            "prompt_data": {
+                                "prompt_id": None,
+                                "judge_id": None,
+                                "judge_message_id": None,
+                            },
+                            "user_data": {
+                                "username": None,
+                                "tokens_used" : None
+                            }
+                        },
+                    }
+
+def create(content, bot_name=None, username=None, prompt=None, bot_id=None, prompt_id=None,
+            judge_id=None, judge_message_id=None, error_logs=False, multiplayer_memory = True, 
+            context_window = 2):
+    
     if bot_id is None:
         bot_id = mutual.bot_id
-    if bot_id is None:
-        raise ValueError("bot_id must be provided either as argument or set in config")
+    if bot_id is None and bot_name is None:
+        raise ValueError("bot_id or bot_name must be provided either as argument or set in config")
 
     url = "https://api-agent.mutuai.io/api/chat"
+    # url = "http://127.0.0.1:8000/api/chat"
 
     headers = {
         "Content-Type": "application/json",
         "Authorization": f"Bearer {mutual.api_key}"
     }
     data = {
         "content": content,
         "bot_id": str(bot_id),
+        "bot_name": bot_name,
+        "prompt": prompt,
         "username": username,
         "prompt_id": prompt_id,
+        "judge_id": judge_id,
+        "judge_message_id": judge_message_id,
         "multiplayer": multiplayer_memory,
         "context_window": context_window
     }
 
     response = requests.post(url, data=json.dumps(data), headers=headers, stream=True)
 
     if response.status_code < 300:
         is_new_bot = False
         is_new_user = False
         for line in response.iter_lines():
             if line:  # filter out keep-alive new lines
                 json_data = json.loads(line)
                 if json_data['error'] is not None and not error_logs:
                     continue
-                if json_data['new_bot'] and not is_new_bot:
-                    is_new_bot = True
-                    print(f"Newly created bot! Here is your id: {json_data['bot_id']}")
-                if json_data['new_bot_user'] and not is_new_user:
+                if json_data['data']['bot_data']['new_bot'] and not is_new_bot:
+                        is_new_bot = True
+                        print(f"Newly created bot! Here is your id: {json_data['data']['bot_data']['bot_id']}")
+                if json_data['data']['bot_data']['new_bot_user'] and not is_new_user:
                     is_new_user = True
-                    print(f"New user {json_data['user_id']} created interacting with bot id: {json_data['bot_id']}")
+                    print(f"New user {json_data['data']['user_data']['username']} created interacting with bot id: {json_data['data']['bot_data']['bot_id']}")
                 if json_data['content'] =='[close]':
                     continue
+                
                 yield json_data
     else:
         # raise Exception(f"Request failed with status code {response.status_code}, with an Error Message: {json.loads(response.text)['detail']}")
         default_stream_response['content'] = f"Request failed with status code {response.status_code}, with an Error Message: {json.loads(response.text)['detail'] or response.text}"
         return default_stream_response
 
 
-def create_demo(content, error_logs=False, multiplayer_memory = True, context_window = 2):
+def create_demo(content, prompt=None, error_logs=False, multiplayer_memory = True, context_window = 2):
 
     url = "https://api-agent.mutuai.io/api/test_chat"
+    # url = "http://127.0.0.1:8000/api/test_chat"
     headers = {
         "Content-Type": "application/json",
         "Authorization": f"Bearer {mutual.api_key}"
     }
     data = {
         "content": content,
+        "prompt": prompt,
         "multiplayer": multiplayer_memory,
         "context_window": context_window
     }
 
     response = requests.post(url, data=json.dumps(data), headers=headers, stream=True)
 
     if response.status_code < 300:
```

### Comparing `mutual-0.1.1/mutual/Prompt.py` & `mutual-0.1.2/mutual/Prompt.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,107 +1,97 @@
 import requests
 import json
 import mutual
 
 default_prompt_response = {
     "prompt_id": None,
-    "identity_prompt": None,
-    "backstory_prompt": None,
-    "world_prompt": None,
-    "action_prompt": None,
+    "prompt": None,
     "internal_thought": None,
     "external_thought": None,
     "internal_thought_memory": None,
     "external_thought_memory": None,
     "summarization_prompt": None,
     "details": "Successful"
 }
 
 def get_prompts(limit=20, offset=0):
     url = f"https://api-agent.mutuai.io/api/prompts?limit={limit}&offset={offset}"
+    # url = f"http://127.0.0.1:8000/api/prompts?limit={limit}&offset={offset}"
     headers = {
         "Authorization": f"Bearer {mutual.api_key}"
     }
     response = requests.get(url, headers=headers)
     if response.status_code < 300:
         return response.json()
     else:
         default_prompt_response["details"] = f"Request failed with status code {response.status_code}, with an Error Message: {json.loads(response.text)['detail'] or response.text}"
         return default_prompt_response
 
 def get_prompt(prompt_id):
     url = f"https://api-agent.mutuai.io/api/prompts/{str(prompt_id)}"
+    # url = f"http://127.0.0.1:8000/api/prompts/{str(prompt_id)}"
     headers = {
         "Authorization": f"Bearer {mutual.api_key}"
     }
     response = requests.get(url, headers=headers)
     # response.raise_for_status()  # Raise an exception if the response contains an HTTP error status code
     if response.status_code < 300:
         return response.json()
     else:
         default_prompt_response["details"] = f"Request failed with status code {response.status_code}, with an Error Message: {json.loads(response.text)['detail'] or response.text}"
         return default_prompt_response
 
 def create_prompt(
     prompt_id,
-    identity_prompt=None,
-    backstory_prompt=None,
-    world_prompt=None,
-    action_prompt=None,
+    prompt=None,
     internal_thought=None,
     external_thought=None,
     internal_thought_memory=None,
     external_thought_memory=None,
     summarization_prompt=None
 ):
     url = f"https://api-agent.mutuai.io/api/prompts"
+    # url = f"http://127.0.0.1:8000/api/prompts"
+
     headers = {
         "Content-Type": "application/json",
         "Authorization": f"Bearer {mutual.api_key}"
     }
     data = {
         "prompt_id": prompt_id,
-        "identity_prompt": identity_prompt,
-        "backstory_prompt": backstory_prompt,
-        "world_prompt": world_prompt,
-        "action_prompt": action_prompt,
+        "prompt": prompt,
         "internal_thought": internal_thought,
         "external_thought": external_thought,
         "internal_thought_memory": internal_thought_memory,
         "external_thought_memory": external_thought_memory,
         "summarization_prompt": summarization_prompt
     }
     response = requests.post(url, json=data, headers=headers)
     if response.status_code < 300:
         return response.json()
     else:
         default_prompt_response["details"] = f"Request failed with status code {response.status_code}, with an Error Message: {response.text}"
         return default_prompt_response
 
 def update_prompt(prompt_id,
-    identity_prompt=None,
-    backstory_prompt=None,
-    world_prompt=None,
-    action_prompt=None,
+    prompt=None,
     internal_thought=None,
     external_thought=None,
     internal_thought_memory=None,
     external_thought_memory=None,
     summarization_prompt=None):
 
     url = f"https://api-agent.mutuai.io/api/prompts/{str(prompt_id)}"
+    # url = f"http://127.0.0.1:8000/api/prompts/{str(prompt_id)}"
     headers = {
         "Content-Type": "application/json",
         "Authorization": f"Bearer {mutual.api_key}"
     }
     data = {
-        "identity_prompt": identity_prompt,
-        "backstory_prompt": backstory_prompt,
-        "world_prompt": world_prompt,
-        "action_prompt": action_prompt,
+        "prompt": prompt,
         "internal_thought": internal_thought,
         "external_thought": external_thought,
         "internal_thought_memory": internal_thought_memory,
         "external_thought_memory": external_thought_memory,
         "summarization_prompt": summarization_prompt
     }
```

### Comparing `mutual-0.1.1/setup.py` & `mutual-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mutual',
-    version='0.1.1',  # beta
+    version='0.1.2',  # beta
     description='A Python client for the Mutual API.',
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     author='Alex Betita', # placeholder for now
     author_email='alexbetita25@gmail.com', # placeholder for now
     url='https://github.com/Mutu-AI',  # if you have a github repo for the package
     packages=find_packages(),
```

