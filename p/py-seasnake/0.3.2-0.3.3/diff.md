# Comparing `tmp/py_seasnake-0.3.2.tar.gz` & `tmp/py_seasnake-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_seasnake-0.3.2.tar", max compression
+gzip compressed data, was "py_seasnake-0.3.3.tar", max compression
```

## Comparing `py_seasnake-0.3.2.tar` & `py_seasnake-0.3.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1070 2023-05-14 17:40:09.264295 py_seasnake-0.3.2/LICENSE
--rw-r--r--   0        0        0      745 2023-05-14 17:40:09.264295 py_seasnake-0.3.2/README.md
--rw-r--r--   0        0        0     1332 2023-05-14 17:40:09.264295 py_seasnake-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      129 2023-05-14 17:40:09.264295 py_seasnake-0.3.2/seasnake/__init__.py
--rw-r--r--   0        0        0     4394 2023-05-14 17:40:09.264295 py_seasnake-0.3.2/seasnake/auth.py
--rw-r--r--   0        0        0     9230 2023-05-14 17:40:09.264295 py_seasnake-0.3.2/seasnake/base.py
--rw-r--r--   0        0        0     1445 2023-05-14 17:40:09.264295 py_seasnake-0.3.2/seasnake/io.py
--rw-r--r--   0        0        0     2775 2023-05-14 17:40:09.264295 py_seasnake-0.3.2/seasnake/projects.py
--rw-r--r--   0        0        0      386 2023-05-14 17:40:09.264295 py_seasnake-0.3.2/seasnake/summaries/__init__.py
--rw-r--r--   0        0        0     3114 2023-05-14 17:40:09.264295 py_seasnake-0.3.2/seasnake/summaries/base.py
--rw-r--r--   0        0        0     2853 2023-05-14 17:40:09.264295 py_seasnake-0.3.2/seasnake/summaries/benthic_lit.py
--rw-r--r--   0        0        0     2979 2023-05-14 17:40:09.268295 py_seasnake-0.3.2/seasnake/summaries/benthic_photo_quadrat.py
--rw-r--r--   0        0        0     2854 2023-05-14 17:40:09.268295 py_seasnake-0.3.2/seasnake/summaries/benthic_pit.py
--rw-r--r--   0        0        0     3741 2023-05-14 17:40:09.268295 py_seasnake-0.3.2/seasnake/summaries/bleaching.py
--rw-r--r--   0        0        0     2654 2023-05-14 17:40:09.268295 py_seasnake-0.3.2/seasnake/summaries/fish_belt.py
--rw-r--r--   0        0        0     2957 2023-05-14 17:40:09.268295 py_seasnake-0.3.2/seasnake/summaries/habitat_complexity.py
--rw-r--r--   0        0        0     2356 2023-05-14 17:40:09.268295 py_seasnake-0.3.2/seasnake/summaries/sample_event.py
--rw-r--r--   0        0        0      606 2023-05-14 17:40:09.268295 py_seasnake-0.3.2/seasnake/timer.py
--rw-r--r--   0        0        0     1850 1970-01-01 00:00:00.000000 py_seasnake-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-19 04:23:02.121797 py_seasnake-0.3.3/LICENSE
+-rw-r--r--   0        0        0      741 2023-07-19 04:23:02.121797 py_seasnake-0.3.3/README.md
+-rw-r--r--   0        0        0     1332 2023-07-19 04:23:02.125798 py_seasnake-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      129 2023-07-19 04:23:02.125798 py_seasnake-0.3.3/seasnake/__init__.py
+-rw-r--r--   0        0        0     4551 2023-07-19 04:23:02.125798 py_seasnake-0.3.3/seasnake/auth.py
+-rw-r--r--   0        0        0     9230 2023-07-19 04:23:02.125798 py_seasnake-0.3.3/seasnake/base.py
+-rw-r--r--   0        0        0     1445 2023-07-19 04:23:02.125798 py_seasnake-0.3.3/seasnake/io.py
+-rw-r--r--   0        0        0     2775 2023-07-19 04:23:02.125798 py_seasnake-0.3.3/seasnake/projects.py
+-rw-r--r--   0        0        0      386 2023-07-19 04:23:02.125798 py_seasnake-0.3.3/seasnake/summaries/__init__.py
+-rw-r--r--   0        0        0     3114 2023-07-19 04:23:02.125798 py_seasnake-0.3.3/seasnake/summaries/base.py
+-rw-r--r--   0        0        0     2853 2023-07-19 04:23:02.125798 py_seasnake-0.3.3/seasnake/summaries/benthic_lit.py
+-rw-r--r--   0        0        0     2979 2023-07-19 04:23:02.125798 py_seasnake-0.3.3/seasnake/summaries/benthic_photo_quadrat.py
+-rw-r--r--   0        0        0     2854 2023-07-19 04:23:02.125798 py_seasnake-0.3.3/seasnake/summaries/benthic_pit.py
+-rw-r--r--   0        0        0     3741 2023-07-19 04:23:02.125798 py_seasnake-0.3.3/seasnake/summaries/bleaching.py
+-rw-r--r--   0        0        0     2654 2023-07-19 04:23:02.125798 py_seasnake-0.3.3/seasnake/summaries/fish_belt.py
+-rw-r--r--   0        0        0     2957 2023-07-19 04:23:02.125798 py_seasnake-0.3.3/seasnake/summaries/habitat_complexity.py
+-rw-r--r--   0        0        0     2356 2023-07-19 04:23:02.125798 py_seasnake-0.3.3/seasnake/summaries/sample_event.py
+-rw-r--r--   0        0        0      606 2023-07-19 04:23:02.125798 py_seasnake-0.3.3/seasnake/timer.py
+-rw-r--r--   0        0        0     1846 1970-01-01 00:00:00.000000 py_seasnake-0.3.3/PKG-INFO
```

### Comparing `py_seasnake-0.3.2/LICENSE` & `py_seasnake-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `py_seasnake-0.3.2/README.md` & `py_seasnake-0.3.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 ```
 from seasnake import auth
 from seasnake.auth import MermaidAuth
 from seasnake.summaries import FishBeltTransect
 
 auth = MermaidAuth()
-token = auth.request_token()
+token = auth.get_token()
 
 project_id = "<YOUR PROJECT ID>"
 fb = FishBeltTransect(token=token)
 df_obs = fb.observations(project_id)
 
 print(df_obs)
```

### Comparing `py_seasnake-0.3.2/pyproject.toml` & `py_seasnake-0.3.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "py-seasnake"
 packages = [
     { include = "seasnake" },
 ]
-version = "0.3.2"
+version = "0.3.3"
 description = "A Python wrapper for accessing and managing MERMAID (Marine Ecological Research Management Aid) data with ease."
 authors = ["Dustin Sampson <gridcell@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://gridcell.github.io/py-seasnake/"
 repository = "https://github.com/gridcell/py-seasnake"
 documentation = "https://gridcell.github.io/py-seasnake/"
```

### Comparing `py_seasnake-0.3.2/seasnake/auth.py` & `py_seasnake-0.3.3/seasnake/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,17 @@
     """
     A class for handling authentication and access token management for the Mermaid API.
 
     The MermaidAuth class is responsible for managing the process of obtaining and storing
     access tokens for use with the Mermaid API. It checks if the stored token is expired,
     and if so, initiates an authentication process to obtain a new token.
 
+    Authenication is performed using [Device Authorization Grant](https://oauth.net/2/grant-types/device-code/)
+    type, and requires input from the user.
+
     Example usage:
 
         mermaid_auth = MermaidAuth()
         token = mermaid_auth.get_token()
     """
 
     AUTH_CODE_URL = f"https://{AUTH0_DOMAIN}/oauth/device/code"
```

### Comparing `py_seasnake-0.3.2/seasnake/base.py` & `py_seasnake-0.3.3/seasnake/base.py`

 * *Files identical despite different names*

### Comparing `py_seasnake-0.3.2/seasnake/io.py` & `py_seasnake-0.3.3/seasnake/io.py`

 * *Files identical despite different names*

### Comparing `py_seasnake-0.3.2/seasnake/projects.py` & `py_seasnake-0.3.3/seasnake/projects.py`

 * *Files identical despite different names*

### Comparing `py_seasnake-0.3.2/seasnake/summaries/base.py` & `py_seasnake-0.3.3/seasnake/summaries/base.py`

 * *Files identical despite different names*

### Comparing `py_seasnake-0.3.2/seasnake/summaries/benthic_lit.py` & `py_seasnake-0.3.3/seasnake/summaries/benthic_lit.py`

 * *Files identical despite different names*

### Comparing `py_seasnake-0.3.2/seasnake/summaries/benthic_photo_quadrat.py` & `py_seasnake-0.3.3/seasnake/summaries/benthic_photo_quadrat.py`

 * *Files identical despite different names*

### Comparing `py_seasnake-0.3.2/seasnake/summaries/benthic_pit.py` & `py_seasnake-0.3.3/seasnake/summaries/benthic_pit.py`

 * *Files identical despite different names*

### Comparing `py_seasnake-0.3.2/seasnake/summaries/bleaching.py` & `py_seasnake-0.3.3/seasnake/summaries/bleaching.py`

 * *Files identical despite different names*

### Comparing `py_seasnake-0.3.2/seasnake/summaries/fish_belt.py` & `py_seasnake-0.3.3/seasnake/summaries/fish_belt.py`

 * *Files identical despite different names*

### Comparing `py_seasnake-0.3.2/seasnake/summaries/habitat_complexity.py` & `py_seasnake-0.3.3/seasnake/summaries/habitat_complexity.py`

 * *Files identical despite different names*

### Comparing `py_seasnake-0.3.2/seasnake/summaries/sample_event.py` & `py_seasnake-0.3.3/seasnake/summaries/sample_event.py`

 * *Files identical despite different names*

### Comparing `py_seasnake-0.3.2/seasnake/timer.py` & `py_seasnake-0.3.3/seasnake/timer.py`

 * *Files identical despite different names*

### Comparing `py_seasnake-0.3.2/PKG-INFO` & `py_seasnake-0.3.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-seasnake
-Version: 0.3.2
+Version: 0.3.3
 Summary: A Python wrapper for accessing and managing MERMAID (Marine Ecological Research Management Aid) data with ease.
 Home-page: https://gridcell.github.io/py-seasnake/
 License: MIT
 Keywords: MERMAID,coral,fish,API
 Author: Dustin Sampson
 Author-email: gridcell@gmail.com
 Requires-Python: >=3.8,<3.12
@@ -39,15 +39,15 @@
 
 ```
 from seasnake import auth
 from seasnake.auth import MermaidAuth
 from seasnake.summaries import FishBeltTransect
 
 auth = MermaidAuth()
-token = auth.request_token()
+token = auth.get_token()
 
 project_id = "<YOUR PROJECT ID>"
 fb = FishBeltTransect(token=token)
 df_obs = fb.observations(project_id)
 
 print(df_obs)
```

