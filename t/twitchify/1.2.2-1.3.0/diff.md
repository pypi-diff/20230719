# Comparing `tmp/twitchify-1.2.2.tar.gz` & `tmp/twitchify-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitchify-1.2.2.tar", last modified: Fri Jul 14 02:40:39 2023, max compression
+gzip compressed data, was "twitchify-1.3.0.tar", last modified: Wed Jul 19 02:39:04 2023, max compression
```

## Comparing `twitchify-1.2.2.tar` & `twitchify-1.3.0.tar`

### file list

```diff
@@ -1,54 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:39.647008 twitchify-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-14 02:40:28.000000 twitchify-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-14 02:40:39.647008 twitchify-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-07-14 02:40:28.000000 twitchify-1.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 02:40:39.647008 twitchify-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-14 02:40:28.000000 twitchify-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:39.643008 twitchify-1.2.2/twitch/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/broadcaster.py
--rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     9565 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10890 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     8497 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/goals.py
--rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/guest.py
--rw-r--r--   0 runner    (1001) docker     (123)    17683 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/moderation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/reward.py
--rw-r--r--   0 runner    (1001) docker     (123)    15857 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     5386 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/survey.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:39.647008 twitchify-1.2.2/twitch/types/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/types/channel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:39.647008 twitchify-1.2.2/twitch/types/eventsub/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/types/eventsub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/types/eventsub/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/types/eventsub/charity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/types/eventsub/goal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/types/eventsub/guest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/types/eventsub/hypertrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/types/eventsub/moderation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/types/eventsub/poll.py
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/types/eventsub/prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/types/eventsub/reward.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/types/eventsub/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/types/eventsub/subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/types/eventsub/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/types/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/types/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/types/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/types/scoopes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/types/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/types/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    13267 2023-07-14 02:40:28.000000 twitchify-1.2.2/twitch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:39.647008 twitchify-1.2.2/twitchify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-14 02:40:39.000000 twitchify-1.2.2/twitchify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-14 02:40:39.000000 twitchify-1.2.2/twitchify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 02:40:39.000000 twitchify-1.2.2/twitchify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-14 02:40:39.000000 twitchify-1.2.2/twitchify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-14 02:40:39.000000 twitchify-1.2.2/twitchify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:39:04.154350 twitchify-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-19 02:38:47.000000 twitchify-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-07-19 02:39:04.154350 twitchify-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-07-19 02:38:47.000000 twitchify-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 02:39:04.154350 twitchify-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-19 02:38:47.000000 twitchify-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:39:04.146350 twitchify-1.3.0/twitch/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-19 02:38:47.000000 twitchify-1.3.0/twitch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-07-19 02:38:47.000000 twitchify-1.3.0/twitch/broadcaster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-07-19 02:38:47.000000 twitchify-1.3.0/twitch/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16766 2023-07-19 02:38:47.000000 twitchify-1.3.0/twitch/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-07-19 02:38:47.000000 twitchify-1.3.0/twitch/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10957 2023-07-19 02:38:47.000000 twitchify-1.3.0/twitch/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8497 2023-07-19 02:38:47.000000 twitchify-1.3.0/twitch/goals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-07-19 02:38:47.000000 twitchify-1.3.0/twitch/guest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20690 2023-07-19 02:38:47.000000 twitchify-1.3.0/twitch/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-07-19 02:38:47.000000 twitchify-1.3.0/twitch/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-07-19 02:38:47.000000 twitchify-1.3.0/twitch/moderation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-07-19 02:38:47.000000 twitchify-1.3.0/twitch/reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15857 2023-07-19 02:38:47.000000 twitchify-1.3.0/twitch/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5386 2023-07-19 02:38:47.000000 twitchify-1.3.0/twitch/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-07-19 02:38:47.000000 twitchify-1.3.0/twitch/survey.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:39:04.150350 twitchify-1.3.0/twitch/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-19 02:38:47.000000 twitchify-1.3.0/twitch/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-19 02:38:47.000000 twitchify-1.3.0/twitch/types/channel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:39:04.150350 twitchify-1.3.0/twitch/types/eventsub/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-19 02:38:47.000000 twitchify-1.3.0/twitch/types/eventsub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-07-19 02:38:47.000000 twitchify-1.3.0/twitch/types/eventsub/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-19 02:38:47.000000 twitchify-1.3.0/twitch/types/eventsub/charity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-07-19 02:38:47.000000 twitchify-1.3.0/twitch/types/eventsub/goal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-07-19 02:38:47.000000 twitchify-1.3.0/twitch/types/eventsub/guest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-19 02:38:47.000000 twitchify-1.3.0/twitch/types/eventsub/hypertrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-19 02:38:47.000000 twitchify-1.3.0/twitch/types/eventsub/moderation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-07-19 02:38:47.000000 twitchify-1.3.0/twitch/types/eventsub/poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-07-19 02:38:47.000000 twitchify-1.3.0/twitch/types/eventsub/prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-07-19 02:38:47.000000 twitchify-1.3.0/twitch/types/eventsub/reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-19 02:38:47.000000 twitchify-1.3.0/twitch/types/eventsub/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-19 02:38:47.000000 twitchify-1.3.0/twitch/types/eventsub/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-19 02:38:47.000000 twitchify-1.3.0/twitch/types/eventsub/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-07-19 02:38:47.000000 twitchify-1.3.0/twitch/types/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-07-19 02:38:47.000000 twitchify-1.3.0/twitch/types/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-19 02:38:47.000000 twitchify-1.3.0/twitch/types/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-07-19 02:38:47.000000 twitchify-1.3.0/twitch/types/scoopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-19 02:38:47.000000 twitchify-1.3.0/twitch/types/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-07-19 02:38:47.000000 twitchify-1.3.0/twitch/types/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-07-19 02:38:47.000000 twitchify-1.3.0/twitch/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14852 2023-07-19 02:38:47.000000 twitchify-1.3.0/twitch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:39:04.154350 twitchify-1.3.0/twitchify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-07-19 02:39:04.000000 twitchify-1.3.0/twitchify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-19 02:39:04.000000 twitchify-1.3.0/twitchify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 02:39:04.000000 twitchify-1.3.0/twitchify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-19 02:39:04.000000 twitchify-1.3.0/twitchify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-19 02:39:04.000000 twitchify-1.3.0/twitchify.egg-info/top_level.txt
```

### Comparing `twitchify-1.2.2/LICENSE` & `twitchify-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `twitchify-1.2.2/PKG-INFO` & `twitchify-1.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitchify
-Version: 1.2.2
+Version: 1.3.0
 Summary: A Python library for Twitch's WebSocket EventSub integration.
 Home-page: https://github.com/mrsnifo/twitchify
 Author: Snifo
 Author-email: Snifo@mail.com
 License: MIT
 Project-URL: Issue tracker, https://github.com/mrsnifo/twitchify/issues
 Classifier: Development Status :: 5 - Production/Stable
@@ -75,34 +75,38 @@
 
 ### With built-in Authorization
 
 ```python
 from twitch import Client
 from twitch.user import Follower
 
-# Initialize the Twitch client with your client ID and client secret.
 client = Client(client_id="YOUR_CLIENT_ID", client_secret="YOUR_CLIENT_SECRET")
 
-# Generate the authorization URL for the Twitch client.
-# The user should visit the provided URL to authorize the app.
-auth = client.auth()
-
 @client.event
 async def on_ready():
     """
     Event handler triggered when the client is ready to start processing events.
     """
     print("Ready as %s" % client.user.display_name)
-
-
+    
 @client.event
 async def on_follow(user: Follower):
     """
     Event handler triggered when a user follows the channel.
     """
     print("%s just followed you!" % user.display_name)
 
-# You can store the access token and refresh token for future use, so you don't have to authorize again.
-client.run(access_token=auth.access_token, refresh_token=auth.refresh_token)
+@client.event
+async def on_auth(access_token: str, refresh_token: str):
+    """
+    Event handler triggered when the user authorized to the app.
+    """
+    # Store those for future use.
+    print('Received access token:', access_token)
+    print('Received refresh token:', refresh_token)
+    
+# Generate the authorization URL for the Twitch client.
+# The user should visit the provided URL to authorize the app.
+client.run()
 ```
 
 Please refer to the [Documentation](https://github.com/MrSniFo/Twitchify/blob/main/docs) or [Examples](https://github.com/MrSniFo/Twitchify/tree/main/examples) for more details.
```

### Comparing `twitchify-1.2.2/README.md` & `twitchify-1.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -50,34 +50,38 @@
 
 ### With built-in Authorization
 
 ```python
 from twitch import Client
 from twitch.user import Follower
 
-# Initialize the Twitch client with your client ID and client secret.
 client = Client(client_id="YOUR_CLIENT_ID", client_secret="YOUR_CLIENT_SECRET")
 
-# Generate the authorization URL for the Twitch client.
-# The user should visit the provided URL to authorize the app.
-auth = client.auth()
-
 @client.event
 async def on_ready():
     """
     Event handler triggered when the client is ready to start processing events.
     """
     print("Ready as %s" % client.user.display_name)
-
-
+    
 @client.event
 async def on_follow(user: Follower):
     """
     Event handler triggered when a user follows the channel.
     """
     print("%s just followed you!" % user.display_name)
 
-# You can store the access token and refresh token for future use, so you don't have to authorize again.
-client.run(access_token=auth.access_token, refresh_token=auth.refresh_token)
+@client.event
+async def on_auth(access_token: str, refresh_token: str):
+    """
+    Event handler triggered when the user authorized to the app.
+    """
+    # Store those for future use.
+    print('Received access token:', access_token)
+    print('Received refresh token:', refresh_token)
+    
+# Generate the authorization URL for the Twitch client.
+# The user should visit the provided URL to authorize the app.
+client.run()
 ```
 
-Please refer to the [Documentation](https://github.com/MrSniFo/Twitchify/blob/main/docs) or [Examples](https://github.com/MrSniFo/Twitchify/tree/main/examples) for more details.
+Please refer to the [Documentation](https://github.com/MrSniFo/Twitchify/blob/main/docs) or [Examples](https://github.com/MrSniFo/Twitchify/tree/main/examples) for more details.
```

### Comparing `twitchify-1.2.2/setup.py` & `twitchify-1.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.2.2/twitch/__init__.py` & `twitchify-1.3.0/twitch/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,22 +4,21 @@
 A Python library for Twitch's WebSocket EventSub integration.
 
 :copyright: (c) 2023-present Snifo
 :license: MIT, see LICENSE for more details.
 """
 
 __title__ = 'Twitchify'
-__version__ = '1.2.2'
+__version__ = '1.3.0'
 __license__ = 'MIT License'
 __author__ = 'Snifo'
 __email__ = 'Snifo@mail.com'
 __github__ = 'https://github.com/mrsnifo/twitchify'
 
 from .client import *
-from .auth import *
 from .user import *
 from .broadcaster import *
 from .channel import *
 from .stream import *
 from .moderation import *
 from .reward import *
 from .goals import *
```

### Comparing `twitchify-1.2.2/twitch/auth.py` & `twitchify-1.3.0/twitch/survey.py`

 * *Files 27% similar despite different names*

```diff
@@ -20,165 +20,231 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
 from __future__ import annotations
 
-from .utils import Scopes, generate_random_state
-from .errors import AuthorizationError
-from . import __version__, __github__
-
-from aiohttp import web
-import urllib.parse
-import asyncio
+from .utils import parse_rfc3339_timestamp
+from .user import Predictor
 
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
-    from .types.scoopes import ScopesType
-    from .http import HTTPClient
-    from .types.http import Token
-    from typing import Optional
-
-import logging
-access_logger = logging.getLogger('aiohttp.access')
-access_logger.setLevel(logging.WARNING)
-_logger = logging.getLogger(__name__)
-
-__all__ = ('Auth',)
-
-
-class Auth:
-    """
-    Authorization code grant flow
-
-    :param http: The HTTP client for making API requests.
-    :param client_id: The client application ID.
-    """
-    __slots__ = ('_http', '_client_id', 'access_token', 'refresh_token', 'scopes', '_host', '_port',
-                 '_force_verify', '_code', '_query', '_state', '_app', '_shutdown_event')
-
-    def __init__(self, http: HTTPClient, client_id: str) -> None:
-        self._http: HTTPClient = http
-        self._client_id: str = client_id
-        # Default values
-        self.access_token: Optional[str] = None
-        self.refresh_token: Optional[str] = None
-        self.scopes: ScopesType = Scopes
-        self._host: str = 'localhost'
-        self._port: int = 3000
-        self._force_verify: bool = False
-        self._code: Optional[str] = None
-        self._query: Optional[web.Request.query] = None
-        # Help prevent Cross-Site Request Forgery (CSRF) attacks.
-        self._state: str = generate_random_state()
-        # Application.
-        self._app = web.Application()
-        self._app.router.add_get('/{tail:.*}', self.handle_redirect)
-        # Shutdown the server after receiving one response
-        self._shutdown_event = asyncio.Event()
+    from typing import Optional, List, Union, Literal
+    from .types.eventsub import prediction as pd
+    from .types.eventsub import poll as pl
+    from datetime import datetime
+
+__all__ = ('Poll', 'Prediction')
+
+
+class Voting:
+    """
+    Represents voting settings for a poll.
+
+    :param vote: The voting settings for the poll.
+    """
+    __slots__ = ('enabled', 'amount_per_vote')
+
+    def __init__(self, vote: pl.Voting) -> None:
+        self.enabled: bool = vote['is_enabled']
+        self.amount_per_vote: int = vote['amount_per_vote']
+
+    def __repr__(self):
+        return f'<Voting enabled={self.enabled} amount_per_vote={self.amount_per_vote}>'
+
+
+class Choice:
+    """
+    Represents a choice in a poll.
+
+    :param choice: The choice data for the poll.
+    """
+    __slots__ = ('id', 'title', 'bits_votes', 'points_votes')
+
+    def __init__(self, choice: Union[pl.Choice, pl.ChoicesCount]) -> None:
+        self.id: str = choice['id']
+        self.title: str = choice['title']
+        self.bits_votes: int = choice.get('bits_votes') or 0
+        self.points_votes: int = choice.get('channel_points_votes') or 0
 
     def __repr__(self) -> str:
-        return f'<Auth access_token={self.access_token} refresh_token={self.refresh_token}>'
+        return f'<Choice id={self.id} title={self.title}>'
+
+
+class Poll:
+    """
+    Represents a channel poll.
+
+    :param poll: The poll data.
+    """
+    __slots__ = ('id', 'title', '_choices', 'bits_voting', 'points_voting', 'started_at',
+                 '_ends_at', '_ended_at', '_status')
+
+    def __init__(self, poll: Union[pl.Begin, pl.Progress, pl.End]) -> None:
+        self.id: str = poll['id']
+        self.title: str = poll['title']
+        self._choices: List[Union[pl.Choice, pl.ChoicesCount]] = poll['choices']
+        self.bits_voting: Voting = Voting(vote=poll['bits_voting'])
+        self.points_voting: Voting = Voting(vote=poll['channel_points_voting'])
+        self.started_at: datetime = parse_rfc3339_timestamp(timestamp=poll['started_at'])
+        self._ends_at: Optional[str] = poll.get('ends_at')
+        self._ended_at: Optional[str] = poll.get('ended_at')
+        self._status: Literal['completed', 'archived', 'terminated'] = poll.get('status')
+
+    def __repr__(self) -> str:
+        return f'<Poll id={self.id} title={self.title}>'
+
+    @property
+    def choices(self) -> List[Choice]:
+        """
+        Get the list of choices for the poll.
+
+        :return: The list of poll choices.
+        """
+        return [Choice(choice=c) for c in self._choices]
+
+    @property
+    def is_ended(self) -> bool:
+        """
+        Check if the poll has ended.
+
+        :return: True if the poll has ended, False otherwise.
+        """
+        return self._ended_at is not None
 
     @property
-    def uri(self) -> str:
-        """Get the URI of the server."""
-        return f'http://{self._host}:{self._port}'
-
-    @property
-    def url(self) -> str:
-        """Get the authorization URL."""
-        if 'user:read:email' not in self.scopes:
-            self.scopes.append('user:read:email')
-        # Removing duplicates.
-        self.scopes = list(dict.fromkeys(self.scopes))
-        encoded_scope = '+'.join(urllib.parse.quote(s) for s in self.scopes)
-        url = f'https://id.twitch.tv/oauth2/authorize?response_type=code&client_id={self._client_id}' \
-              f'&force_verify={self._force_verify}&redirect_uri={self.uri}&scope={encoded_scope}' \
-              f'&state={self._state}'
-        return url
-
-    async def handle_redirect(self, request: web.Request) -> web.Response:
-        """
-        Handle the redirect from Twitch authorization.
-
-        :param request: The web request.
-        """
-        _logger.debug('Received request to URL: %s', request.rel_url)
-        query_params = request.query
-        if (query_params.get('code') or query_params.get('error')) \
-                and self._state == query_params.get('state'):
-            await self.shutdown(query=query_params)
-            if query_params.get('code'):
-                self._code = query_params.get('code')
-                html = f'''
-                    <html>
-                        <body>
-                            <h1>Redirect Completed</h1>
-                            <p><a href="{__github__}">Twitchify</a> Version: {__version__}</p>
-                            <p>You can now close this page.</p>
-                        </body>
-                    </html>
-                    '''
-                return web.Response(
-                    text=html,
-                    content_type='text/html'
-                )
-            if query_params.get('error'):
-                error_description = query_params.get('error_description')
-                return web.Response(status=403, text=error_description.replace('+', ' '))
-        return web.Response(status=403, text='')
-
-    async def run_server(self) -> None:
-        """Run the server."""
-        runner = web.AppRunner(self._app)
-        await runner.setup()
-        uri = urllib.parse.urlparse(self.uri)
-        site = web.TCPSite(runner, uri.hostname, uri.port)
-        _logger.debug('Starting the authorization server.')
-        await site.start()
-        _logger.debug('Server is now running on %s', self.uri)
-        await self._shutdown_event.wait()
-        if self._code is not None:
-            response: Token = await self._http.auth_code(code=self._code, redirect_uri=self.uri)
-            if response is not None:
-                self.access_token: str = response['access_token']
-                self.refresh_token: str = response['refresh_token']
-        _logger.debug('Shutting down the authorization server.')
-        await runner.cleanup()
-        await runner.shutdown()
-
-    async def shutdown(self, query: web.Request.query) -> None:
-        """
-        Shutdown the server.
-
-        :param query: The web request query.
-        """
-        _logger.debug('Shutting down the server app.')
-        await self._app.shutdown()
-        await self._app.cleanup()
-        self._query = query
-        self._shutdown_event.set()
-
-    def get_code(self, verify: bool = False, port: int = 3000) -> str:
-        """
-        Get the authorization code.
-
-        :param verify: Whether to force verification.
-        :param port: The server port to use.
-        """
-        try:
-            loop = asyncio.get_running_loop()
-        except RuntimeError:
-            loop = asyncio.get_event_loop()
-        if verify:
-            self._force_verify = verify
-        if port:
-            self._port = port
-        loop.run_until_complete(self.run_server())
-        if self._query.get('error'):
-            error_description = self._query.get('error_description')
-            raise AuthorizationError(message=error_description.replace('+', ' ') + '.')
-        if self._query.get('code') is None:
-            raise AuthorizationError(message='Failed to authorize.')
-        return self._query.get('code')
+    def status(self) -> Literal['active', 'completed', 'archived', 'terminated']:
+        """
+        Get the status of the poll.
+
+        :return: The status of the poll.
+        """
+        if self._ended_at:
+            return self._status
+        return 'active'
+
+    @property
+    def end_at(self) -> datetime:
+        """
+        Get the end timestamp of the poll.
+
+        :return: The end timestamp of the poll.
+        """
+        if self._ended_at is not None:
+            return parse_rfc3339_timestamp(timestamp=self._ended_at)
+        return parse_rfc3339_timestamp(timestamp=self._ends_at)
+
+
+class Outcome:
+    """
+    Represents an outcome in a prediction.
+
+    :param outcome: The outcome data.
+    """
+    __slots__ = ('id', 'title', 'color', '_users', '_top_predictors')
+
+    def __init__(self, outcome: Union[pd.BaseOutcome, pd.Outcome]) -> None:
+        self.id: str = outcome['id']
+        self.title: str = outcome['title']
+        self.color: str = outcome['color']
+        self._users: int = outcome.get('users') or 0
+        self._top_predictors: Optional[List[pd.Predictor]] = outcome.get('top_predictors')
+
+    def __repr__(self) -> str:
+        return f'<Outcome user={self.id} title={self.title} color={self.color}>'
+
+    @property
+    def users(self) -> int:
+        """
+        Get the number of users associated with the outcome.
+
+        :return: The number of users associated with the outcome.
+        """
+        if self._top_predictors is None:
+            return self._users
+        return len(self._top_predictors)
+
+    @property
+    def top_predictors(self) -> List[Predictor]:
+        """
+        Get the list of top predictors for the outcome.
+
+        :return: The list of top predictors.
+        """
+        if self._top_predictors:
+            return [Predictor(predictor=p) for p in self._top_predictors]
+        return []
+
+
+class Prediction:
+    """
+    Represents a channel prediction.
+
+    :param prediction: The prediction data.
+    """
+    __slots__ = ('id', 'title', '_outcomes', 'started_at', '_locks_at', '_locked_at', '_ended_at',
+                 '_status')
+
+    def __init__(self, prediction: Union[pd.Begin, pd.Progress, pd.Lock, pd.End]) -> None:
+        self.id: str = prediction['id']
+        self.title: str = prediction['title']
+        self._outcomes: List[Union[pd.BaseOutcome, pd.Outcome]] = prediction['outcomes']
+        self.started_at: datetime = parse_rfc3339_timestamp(timestamp=prediction['started_at'])
+        self._locks_at: Optional[str] = prediction.get('locks_at')
+        self._locked_at: Optional[str] = prediction.get('locked_at')
+        self._ended_at: Optional[str] = prediction.get('ended_at')
+        self._status: Literal['active', 'completed', 'archived', 'resolved'] = prediction.get('status')
+
+    def __repr__(self) -> str:
+        return f'<Prediction id={self.id} title={self.title}>'
+
+    @property
+    def outcomes(self) -> List[Outcome]:
+        """
+        Get the list of outcomes for the prediction.
+
+        :return: The list of prediction outcomes.
+        """
+        return [Outcome(outcome=o) for o in self._outcomes]
+
+    @property
+    def is_ended(self) -> bool:
+        """
+        Check if the prediction has ended.
+
+        :return: True if the prediction has ended, False otherwise.
+        """
+        return self._ended_at is not None
+
+    @property
+    def status(self) -> Literal['active', 'completed', 'archived', 'resolved']:
+        """
+        Get the status of the prediction.
+
+        :return: The status of the prediction.
+        """
+        if self._ended_at:
+            return self._status
+        return 'active'
+
+    @property
+    def locks_at(self) -> datetime:
+        """
+        Get the locks timestamp of the prediction.
+
+        :return: The locks timestamp of the prediction.
+        """
+        if self._locked_at is not None:
+            return parse_rfc3339_timestamp(timestamp=self._locked_at)
+        return parse_rfc3339_timestamp(timestamp=self._locks_at)
+
+    @property
+    def ended_at(self) -> Optional[datetime]:
+        """
+        Get the end time of Prediction.
+
+        :return: The end time as a datetime object.
+        """
+        if self._ended_at:
+            return parse_rfc3339_timestamp(timestamp=self._ended_at)
+        return None
```

### Comparing `twitchify-1.2.2/twitch/broadcaster.py` & `twitchify-1.3.0/twitch/broadcaster.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.2.2/twitch/channel.py` & `twitchify-1.3.0/twitch/channel.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.2.2/twitch/errors.py` & `twitchify-1.3.0/twitch/errors.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.2.2/twitch/gateway.py` & `twitchify-1.3.0/twitch/gateway.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,14 @@
                      WsReconnect)
 from .utils import to_json, get_subscriptions
 
 from json import JSONDecodeError
 import asyncio
 import aiohttp
 
-
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     from .types.eventsub.subscriptions import SubscriptionInfo
     from asyncio import AbstractEventLoop
     from typing import Optional, List, Dict, Any
     from aiohttp import ClientWebSocketResponse
     from .state import ConnectionState
@@ -54,37 +53,38 @@
     :param http: The HTTP client for making API requests.
     :param connection: The ConnectionState object.
     :param loop: The event loop.
     :param events: A list of events.
     """
 
     __slots__ = ('__http', '__connection', '__loop', 'subscriptions', '_ready', '_keep_alive',
-                 '_ws', '_ws_switch', 'session_id', '__reconnect')
+                 '_ws', '_ws_switch', 'session_id', '__reconnect', 'cli')
 
     def __init__(self, *, http: HTTPClient, connection: ConnectionState, loop: AbstractEventLoop,
                  events: List[str]) -> None:
         self.__http: HTTPClient = http
         self.__connection: ConnectionState = connection
         self.__loop: AbstractEventLoop = loop
         self.subscriptions: List[SubscriptionInfo] = get_subscriptions(events=events)
         # Default subscription
-        self.subscriptions.append({'name': 'user.update', 'version': '1'})
+        self.subscriptions.append(get_subscriptions(events=['channel_update'])[0])
         # Default Session KeepAlive.
         self._keep_alive: int = 10
         self._ws: Optional[ClientWebSocketResponse] = None
         self._ws_switch: Optional[ClientWebSocketResponse] = None
         self.session_id: Optional[str] = None
+        # Twitch CLI.
+        self.cli: Optional[str] = None
 
     async def connect(self, reconnect: bool, url: str = 'wss://eventsub.wss.twitch.tv/ws') -> None:
         """
         Connect to the WebSocket.
-
-        :param reconnect: reconnect to the websocket if an error occurred
-        :param url: The URL to connect to. Default is the DEFAULT_URL.
         """
+        if self.cli:
+            url = self.cli
         _retry: int = 0
         while True:
             # Reset retry timer
             if _retry == 12:
                 _retry = 1
             else:
                 _retry += 1
@@ -106,15 +106,15 @@
                 if isinstance(error, SessionClosed):
                     _logger.error('Failed to establish a WebSocket connection due to a closed session. '
                                   'Retrying in %s seconds...', _retry * 5)
                 else:
                     _logger.error('WebSocket connection failed: %s Retrying in %s seconds...',
                                   str(error), _retry * 5)
                 await asyncio.sleep(5 * _retry)
-            except (WebSocketError, aiohttp.ClientConnectorError, TimeoutError) as error:
+            except (WebSocketError, aiohttp.ClientConnectorError) as error:
                 if reconnect:
                     _logger.error('WebSocket connection error: %s Retrying in %s seconds...',
                                   str(error), _retry * 5)
                     await asyncio.sleep(5 * _retry)
                 else:
                     raise
 
@@ -139,14 +139,15 @@
                     raise WebsocketClosed(message='Reconnect grace time expired.')
                 elif close_code == 4005:
                     raise WebsocketClosed(message='Network timeout.')
                 elif close_code == 4006:
                     raise WebsocketClosed(message='Network error.')
                 elif close_code == 4007:
                     raise WebsocketClosed(message='Invalid reconnect.')
+                raise WebSocketError(message=f'Connection has been closed, Close code: {close_code}.')
             elif msg.type == aiohttp.WSMsgType.ERROR:
                 exception = self._ws.exception()
                 error_message = str(exception) if exception else 'Unknown error occurred.'
                 raise WebSocketError(message=error_message)
 
     async def received_response(self, response: str) -> None:
         """
```

### Comparing `twitchify-1.2.2/twitch/goals.py` & `twitchify-1.3.0/twitch/goals.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.2.2/twitch/guest.py` & `twitchify-1.3.0/twitch/guest.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.2.2/twitch/http.py` & `twitchify-1.3.0/twitch/http.py`

 * *Files 17% similar despite different names*

```diff
@@ -20,44 +20,47 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
 from __future__ import annotations
 
-from .errors import (TwitchServerError, BadRequest, Unauthorized, Forbidden, HTTPException, NotFound,
-                     SessionClosed)
-from aiohttp import ClientSession, helpers
+from .errors import (TwitchServerError, BadRequest, Unauthorized, Forbidden,
+                     HTTPException, NotFound, SessionClosed)
 from . import __version__, __github__
+from .utils import format_seconds, generate_random_state
+
+from aiohttp import ClientSession, helpers, web
 from asyncio import Lock, sleep, Task
-from .utils import format_seconds
-from time import time
 from json import JSONDecodeError
+from time import time
+import urllib.parse
+import asyncio
 
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
+    from typing import Optional, List, Callable, Any, Type, Tuple
     from .types.eventsub.subscriptions import SubscriptionInfo
-    from typing import Optional, List, Callable, Any
     from aiohttp import ClientWebSocketResponse
-    from .types.http import Validate, Token
+    from .types.http import Validate, Token, ScopesType
+    from .types.channel import Channel
     from .types.stream import Stream
     from .types.user import UserType
-    from .types.channel import Channel
+    from types import TracebackType
+    from typing import Type
 
 import logging
 _logger = logging.getLogger(__name__)
 
+__all__ = ('HTTPClient', 'Server')
+
 
 class Route:
     """
     Initialize a Route object.
-
-    :param method: The HTTP method of the route.
-    :param path: The path of the route.
-    :param url: The complete URL of the route (overrides BASE_ROUTE + path). Defaults to None.
     """
     BASE_ROUTE: str = 'https://api.twitch.tv/helix/'
 
     __slots__ = ('method', 'url')
 
     def __init__(self, method: str, path: Optional[str] = None, url: Optional[str] = None) -> None:
         self.method: str = method
@@ -72,42 +75,37 @@
     def __repr__(self) -> str:
         return f'<Route method={self.method} url={self.url}>'
 
 
 class HTTPClient:
     """Serves as an HTTP client responsible for sending HTTP requests to the Twitch API."""
     __slots__ = ('_dispatch', '_client_id', '_client_secret', '__session', '_session_lock',
-                 '_user_agent', '_refresh_token')
+                 '_user_agent', '_refresh_token', 'cli')
 
     def __init__(self, dispatcher: Callable[..., Any], client_id: str, secret_secret: Optional[str]) -> None:
-        """
-        Initialize the HTTPClient object.
-        """
         self._dispatch: Callable[[str, Any, Any], Task] = dispatcher
         self._client_id: str = client_id
         self._client_secret: str = secret_secret
         self.__session: Optional[ClientSession] = None
         self._session_lock: Lock = Lock()
         self._user_agent: str = f'Twitchify/{__version__} (GitHub: {__github__})'
         self._refresh_token: Optional[str] = None
+        # Twitch CLI.
+        self.cli: Optional[str] = None
 
     @property
     def is_open(self) -> bool:
         """
         Checks if the HTTP session is open.
-
-        :return: True if the session is open, False otherwise.
         """
         return self.__session is not None and not self.__session.closed
 
     async def _open(self, *, access_token: Optional[str] = None) -> None:
         """
         Opens an HTTP session.
-
-        :param access_token: The access token to use for authentication.
         """
         async with self._session_lock:
             if not self.is_open:
                 headers = {
                     'Client-ID': self._client_id,
                     'Content-Type': 'application/json'
                 }
@@ -115,36 +113,25 @@
                     headers.update({'Authorization': f'Bearer {access_token}'})
                 self.__session = ClientSession(headers=headers)
                 _logger.debug('New HTTP session has been created.')
 
     async def close(self) -> bool:
         """
         Closes the HTTP session.
-
-        :return:
-         True if the session is closed, False otherwise.
         """
         async with self._session_lock:
             if self.is_open:
                 await self.__session.close()
                 self.__session = None
                 _logger.debug('HTTP session has been closed.')
         return not self.is_open
 
     async def open_session(self, token: str, refresh_token: Optional[str] = None) -> Validate:
         """
         Verifies the access token and opens a new session with it.
-
-        :param token:
-         The access token for authentication.
-
-        :param refresh_token:
-         (Optional) The refresh token for refreshing the access token.
-
-        :return: A validation response.
         """
         # Opening a session.
         if self.is_open:
             self.__session.headers.update({'Authorization': f'Bearer {token}'})
         else:
             await self._open(access_token=token)
         self._refresh_token = refresh_token
@@ -158,17 +145,14 @@
                     ' expire time of 0.')
                 self._refresh_token = None
         return validation
 
     async def ws_connect(self, *, url: str) -> ClientWebSocketResponse:
         """
         Creates a websocket using the existing session.
-
-        :return:
-         The created websocket.
         """
 
         if self.is_open:
             websocket: ClientWebSocketResponse = await self.__session.ws_connect(
                 url=url,
                 headers={'User-Agent': self._user_agent},
                 timeout=30,
@@ -176,23 +160,14 @@
             )
             return websocket
         raise SessionClosed
 
     async def _request(self, *, route: Route, **kwargs) -> dict:
         """
         HTTP request base.
-
-        :param route:
-         The route to send the request to.
-
-        :param kwargs:
-         Additional parameters to pass to the request.
-
-        :return:
-         The response from the API.
         """
         method = route.method
         url = route.url
         for retry_count in range(1, 4):
             try:
                 async with self.__session.request(method, url, **kwargs) as response:
                     if response.status in [200, 202]:
@@ -243,43 +218,31 @@
                     self.__session.headers.update({'Authorization': f'Bearer {refresh["access_token"]}'})
                     _logger.debug('Session headers have been successfully updated with'
                                   ' the new access token.')
                     self._dispatch('refresh_token', refresh['access_token'])
                     return refresh
         return None
 
-    async def auth_code(self, code: str, redirect_uri: str) -> Token:
+    async def auth_code(self, code: str, redirect_uri: str) -> Tuple[str, str]:
         """
         Authorization using the code to get the access token and refresh token.
-
-        :param code: The authorization code.
-        :param redirect_uri: The redirect URI.
-
-        :return:
-         User Token.
         """
         await self._open()
         params = {'client_id': self._client_id,
                   'client_secret': self._client_secret,
                   'code': code,
                   'grant_type': 'authorization_code',
                   'redirect_uri': redirect_uri}
         route = Route(method='POST', url='https://id.twitch.tv/oauth2/token')
-        generate: Token = await self.request(route=route, params=params)
-        return generate
+        token: Token = await self.request(route=route, params=params)
+        return token['access_token'], token['refresh_token']
 
     async def _validate_token(self, *, generate: bool = False) -> Validate:
         """
         Validate access token.
-
-        :param generate:
-         Generate a new token if it's unauthorized. Defaults to False.
-
-        :return:
-         The validation response.
         """
         while True:
             try:
                 route = Route(method='GET', url='https://id.twitch.tv/oauth2/validate')
                 validation: Validate = await self._request(route=route)
                 _logger.debug('Access token successfully validated.')
                 return validation
@@ -293,27 +256,25 @@
                         raise Unauthorized(message='Invalid refresh token or client secret.') from exc
                 else:
                     raise
 
     async def refresher(self, *, expires_in: int) -> None:
         """
         Refresher task to refresh the current access token.
-
-        :param expires_in:
-         The expiration time of the current access token.
         """
         start_time = time()
         # If the refresh_token or client_secret is missing,
         if self._refresh_token and self._client_secret:
             _logger.debug('A new token will be generated in %s.', format_seconds(expires_in - 300))
         else:
             # Set expires_in to a default value of 3540 seconds (59 minutes).
             expires_in = 3540 + 300
-            _logger.debug('Access token generation disabled due to'
-                          ' missing refresh token or client secret.')
+            _logger.warning('Access token will expire in %s,'
+                            ' and won\'t be generated without the refresh token or client secret.',
+                            format_seconds(expires_in - 300))
         while True:
             # Create a new access token approximately 5 minutes before the
             # current token's expiration.
             await sleep(min((expires_in - 300), 3540))
             current_time = time()
             elapsed_time = current_time - start_time
             try:
@@ -331,23 +292,14 @@
                 _logger.warning('Invalid Refresh Token.'
                                 ' The automatic generation feature has been disabled.')
                 self._refresh_token = None
 
     async def request(self, *, route: Route, **kwargs) -> _request:
         """
         Sends an HTTP request to the specified route.
-
-        :param route:
-         The route to send the request to.
-
-        :param kwargs:
-         Additional parameters to pass to the request.
-
-        :return:
-         The response from the API.
         """
         while True:
             try:
                 _logger.debug('Sending request: %s kwargs: %s.', route, kwargs)
                 data: dict = await self._request(route=route, **kwargs)
                 _logger.debug('Received response: %s', data)
                 return data
@@ -360,23 +312,14 @@
                 except (Unauthorized, BadRequest):
                     raise
 
     async def subscribe(self, *, user_id: str, session_id: str,
                         subscriptions: List[SubscriptionInfo]) -> None:
         """
         Subscribes to multiple events with the specified subscriptions.
-
-        :param user_id:
-         The user ID.
-
-        :param session_id:
-         The session ID for the subscriptions.
-
-        :param subscriptions:
-         A list of subscription events.
         """
         for subscription in subscriptions:
             try:
                 data = {
                     'type': subscription['name'],
                     'version': subscription['version'],
                     'condition': {
@@ -388,20 +331,23 @@
                     'transport': {
                         'method': 'websocket',
                         'session_id': session_id
                     }
                 }
                 _logger.debug('Subscribing to `%s` event version %s.',
                               subscription['name'], subscription['version'])
-                route = Route(method='POST', path='eventsub/subscriptions')
+                if self.cli:
+                    route = Route(method='POST', url=self.cli)
+                else:
+                    route = Route(method='POST', path='eventsub/subscriptions')
                 await self.request(route=route, json=data)
             except (Forbidden, BadRequest) as error:
                 if isinstance(error, Forbidden):
-                    _logger.error('Subscription type `%s` version `%s` is missing proper authorization.',
-                                  subscription['name'], subscription['version'])
+                    _logger.error('Subscription type `%s` version `%s` is missing scope `%s`.',
+                                  subscription['name'], subscription['version'], subscription['scope'])
                 if isinstance(error, BadRequest):
                     _logger.warning('Subscription type `%s` version `%s` unsupported.',
                                     subscription['name'], subscription['version'])
         self._dispatch('ready')
 
     async def get_client(self) -> UserType:
         """
@@ -426,7 +372,109 @@
             _route = Route(method='GET', path=f'streams?user_id={user_id}')
             data = await self.request(route=_route)
             if len(data['data']) == 1:
                 return data['data'][0]
         except NotFound:
             pass
         return None
+
+
+class Server:
+    """Serves as an HTTP server responsible for user authorization."""
+    __slots__ = ('host', 'port', 'app', 'event', '__state', '__code')
+
+    def __init__(self, port: int):
+        self.host: str = 'localhost'
+        self.port: int = port
+        self.app: web.Application = web.Application()
+        self.event: asyncio.Event = asyncio.Event()
+        self.app['runner']: Optional[web.AppRunner] = None
+        self.app.router.add_get('/', self.handle_request)
+        self.__state: Optional[str] = None
+        self.__code: Optional[str] = None
+
+    async def __aenter__(self) -> 'Server':
+        """
+        Method to be called when entering the async with block.
+        """
+        self.__state = generate_random_state()
+        await self.start_server()
+        return self
+
+    async def start_server(self):
+        """
+        This method sets up the server.
+        """
+        runner = web.AppRunner(self.app)
+        self.app['runner'] = runner
+        await runner.setup()
+        site = web.TCPSite(runner, self.host, self.port)
+        _logger.debug('Starting the authorization server.')
+        await site.start()
+        _logger.debug('Server is now running on %s', self.uri)
+
+    def url(self, client_id: str, scopes: ScopesType, force_verify: bool = True) -> str:
+        """Get the authorization URL."""
+        if 'user:read:email' not in scopes:
+            scopes.append('user:read:email')
+        # Removing duplicates.
+        scopes = list(dict.fromkeys(scopes))
+        encoded_scope = '+'.join(urllib.parse.quote(s) for s in scopes)
+        url = f'https://id.twitch.tv/oauth2/authorize?response_type=code&client_id={client_id}' \
+              f'&force_verify={force_verify}&redirect_uri={self.uri}&scope={encoded_scope}' \
+              f'&state={self.__state}'
+        return url
+
+    @property
+    def uri(self) -> str:
+        """Get the URI of the server."""
+        return f'http://{self.host}:{self.port}'
+
+    async def wait_for_code(self) -> str:
+        """
+        This method waits for the 'event' to be set
+        indicating that the authorization code has been received.
+        """
+        await self.event.wait()
+        return self.__code
+
+    async def handle_request(self, request: web.Request) -> web.Response:
+        """
+        This method handles the incoming request from Twitch during the authorization process.
+        """
+        _logger.debug('Received request to URL: %s', request.rel_url)
+        query_params = request.query
+        if (query_params.get('code') or query_params.get('error')) \
+                and self.__state == query_params.get('state'):
+            if query_params.get('code'):
+                self.__code = query_params.get('code')
+                self.event.set()
+                html = f'''
+                    <html>
+                        <body>
+                            <h1>Redirect Completed</h1>
+                            <p><a href="{__github__}">Twitchify</a> Version: {__version__}</p>
+                            <p>You can now close this page.</p>
+                        </body>
+                    </html>
+                    '''
+                return web.Response(
+                    text=html,
+                    content_type='text/html'
+                )
+            if query_params.get('error'):
+                error_description = query_params.get('error_description')
+                return web.Response(status=403, text=error_description.replace('+', ' '))
+        return web.Response(status=403, text='')
+
+    async def __aexit__(self, exc_type: Optional[Type[BaseException]],
+                        exc_value: Optional[BaseException],
+                        traceback: Optional[TracebackType]) -> None:
+        """
+        Method to be called when exiting the async with block.
+
+        This method performs the cleanup tasks when exiting the async with block,
+        ensuring that the server is closed gracefully.
+        """
+        if self.app['runner'] is not None:
+            _logger.debug('Shutting down the authorization server.')
+            await self.app['runner'].cleanup()
```

### Comparing `twitchify-1.2.2/twitch/message.py` & `twitchify-1.3.0/twitch/message.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.2.2/twitch/moderation.py` & `twitchify-1.3.0/twitch/moderation.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.2.2/twitch/reward.py` & `twitchify-1.3.0/twitch/reward.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.2.2/twitch/state.py` & `twitchify-1.3.0/twitch/state.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.2.2/twitch/stream.py` & `twitchify-1.3.0/twitch/stream.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.2.2/twitch/types/channel.py` & `twitchify-1.3.0/twitch/types/channel.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.2.2/twitch/types/eventsub/channel.py` & `twitchify-1.3.0/twitch/types/eventsub/channel.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.2.2/twitch/types/eventsub/charity.py` & `twitchify-1.3.0/twitch/types/eventsub/charity.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.2.2/twitch/types/eventsub/goal.py` & `twitchify-1.3.0/twitch/types/eventsub/goal.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.2.2/twitch/types/eventsub/guest.py` & `twitchify-1.3.0/twitch/types/eventsub/guest.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.2.2/twitch/types/eventsub/hypertrain.py` & `twitchify-1.3.0/twitch/types/eventsub/hypertrain.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.2.2/twitch/types/eventsub/moderation.py` & `twitchify-1.3.0/twitch/types/eventsub/moderation.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.2.2/twitch/types/eventsub/poll.py` & `twitchify-1.3.0/twitch/types/eventsub/poll.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.2.2/twitch/types/eventsub/prediction.py` & `twitchify-1.3.0/twitch/types/eventsub/prediction.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.2.2/twitch/types/eventsub/reward.py` & `twitchify-1.3.0/twitch/types/eventsub/reward.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.2.2/twitch/types/eventsub/stream.py` & `twitchify-1.3.0/twitch/types/eventsub/stream.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.2.2/twitch/types/eventsub/subscriptions.py` & `twitchify-1.3.0/twitch/types/eventsub/subscriptions.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,16 +18,17 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NON-INFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
-from typing import TypedDict
+from typing import TypedDict, Optional
 
 
 class SubscriptionInfo(TypedDict):
     """
     Represents a subscription with a name and a version.
     """
     name: str
     version: str
+    scope: Optional[str]
```

### Comparing `twitchify-1.2.2/twitch/types/eventsub/user.py` & `twitchify-1.3.0/twitch/types/eventsub/user.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.2.2/twitch/types/gateway.py` & `twitchify-1.3.0/twitch/types/gateway.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.2.2/twitch/types/http.py` & `twitchify-1.3.0/twitch/types/message.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,20 +21,16 @@
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
 from typing import TypedDict, List
 
 
-class Validate(TypedDict):
-    client_id: str
-    login: str
-    scopes: List[str]
-    user_id: str
-    expires_in: int
+class Emote(TypedDict):
+    begin: int
+    end: int
+    id: str
 
 
-class Token(TypedDict):
-    access_token: str
-    refresh_token: str
-    scope: List[str]
-    token_type: str
+class Message(TypedDict):
+    text: str
+    emotes: List[Emote]
```

### Comparing `twitchify-1.2.2/twitch/types/message.py` & `twitchify-1.3.0/twitch/types/stream.py`

 * *Files 27% similar despite different names*

```diff
@@ -18,19 +18,26 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NON-INFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
-from typing import TypedDict, List
+from .user import SpecificUser
+from typing import TypedDict, Literal, List
 
 
-class Emote(TypedDict):
-    begin: int
-    end: int
-    id: str
+class Category(TypedDict):
+    game_id: str
+    game_name: str
 
 
-class Message(TypedDict):
-    text: str
-    emotes: List[Emote]
+class Stream(SpecificUser, Category):
+    id: str
+    title: str
+    language: str
+    tags: List[str]
+    type: Literal['live', '']
+    is_mature: bool
+    viewer_count: int
+    thumbnail_url: str
+    started_at: str
```

### Comparing `twitchify-1.2.2/twitch/types/scoopes.py` & `twitchify-1.3.0/twitch/types/scoopes.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.2.2/twitch/types/user.py` & `twitchify-1.3.0/twitch/types/user.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.2.2/twitch/user.py` & `twitchify-1.3.0/twitch/user.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.2.2/twitchify.egg-info/PKG-INFO` & `twitchify-1.3.0/twitchify.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitchify
-Version: 1.2.2
+Version: 1.3.0
 Summary: A Python library for Twitch's WebSocket EventSub integration.
 Home-page: https://github.com/mrsnifo/twitchify
 Author: Snifo
 Author-email: Snifo@mail.com
 License: MIT
 Project-URL: Issue tracker, https://github.com/mrsnifo/twitchify/issues
 Classifier: Development Status :: 5 - Production/Stable
@@ -75,34 +75,38 @@
 
 ### With built-in Authorization
 
 ```python
 from twitch import Client
 from twitch.user import Follower
 
-# Initialize the Twitch client with your client ID and client secret.
 client = Client(client_id="YOUR_CLIENT_ID", client_secret="YOUR_CLIENT_SECRET")
 
-# Generate the authorization URL for the Twitch client.
-# The user should visit the provided URL to authorize the app.
-auth = client.auth()
-
 @client.event
 async def on_ready():
     """
     Event handler triggered when the client is ready to start processing events.
     """
     print("Ready as %s" % client.user.display_name)
-
-
+    
 @client.event
 async def on_follow(user: Follower):
     """
     Event handler triggered when a user follows the channel.
     """
     print("%s just followed you!" % user.display_name)
 
-# You can store the access token and refresh token for future use, so you don't have to authorize again.
-client.run(access_token=auth.access_token, refresh_token=auth.refresh_token)
+@client.event
+async def on_auth(access_token: str, refresh_token: str):
+    """
+    Event handler triggered when the user authorized to the app.
+    """
+    # Store those for future use.
+    print('Received access token:', access_token)
+    print('Received refresh token:', refresh_token)
+    
+# Generate the authorization URL for the Twitch client.
+# The user should visit the provided URL to authorize the app.
+client.run()
 ```
 
 Please refer to the [Documentation](https://github.com/MrSniFo/Twitchify/blob/main/docs) or [Examples](https://github.com/MrSniFo/Twitchify/tree/main/examples) for more details.
```

### Comparing `twitchify-1.2.2/twitchify.egg-info/SOURCES.txt` & `twitchify-1.3.0/twitchify.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 LICENSE
 README.md
 setup.py
 twitch/__init__.py
-twitch/auth.py
 twitch/broadcaster.py
 twitch/channel.py
 twitch/client.py
 twitch/errors.py
 twitch/gateway.py
 twitch/goals.py
 twitch/guest.py
```

