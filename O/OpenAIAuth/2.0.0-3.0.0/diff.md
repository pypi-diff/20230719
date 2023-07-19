# Comparing `tmp/OpenAIAuth-2.0.0.tar.gz` & `tmp/OpenAIAuth-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpenAIAuth-2.0.0.tar", last modified: Sat Jun 24 14:02:20 2023, max compression
+gzip compressed data, was "OpenAIAuth-3.0.0.tar", last modified: Wed Jul 19 09:25:33 2023, max compression
```

## Comparing `OpenAIAuth-2.0.0.tar` & `OpenAIAuth-3.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:02:20.794830 OpenAIAuth-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-24 14:01:51.000000 OpenAIAuth-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-24 14:02:20.794830 OpenAIAuth-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-24 14:01:51.000000 OpenAIAuth-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 14:02:20.794830 OpenAIAuth-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-24 14:01:51.000000 OpenAIAuth-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:02:20.794830 OpenAIAuth-2.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:02:20.794830 OpenAIAuth-2.0.0/src/OpenAIAuth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-24 14:02:20.000000 OpenAIAuth-2.0.0/src/OpenAIAuth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-24 14:02:20.000000 OpenAIAuth-2.0.0/src/OpenAIAuth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 14:02:20.000000 OpenAIAuth-2.0.0/src/OpenAIAuth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-24 14:02:20.000000 OpenAIAuth-2.0.0/src/OpenAIAuth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-24 14:02:20.000000 OpenAIAuth-2.0.0/src/OpenAIAuth.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9638 2023-06-24 14:01:51.000000 OpenAIAuth-2.0.0/src/OpenAIAuth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:25:33.394474 OpenAIAuth-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-19 09:25:10.000000 OpenAIAuth-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-19 09:25:33.394474 OpenAIAuth-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-19 09:25:10.000000 OpenAIAuth-3.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 09:25:33.394474 OpenAIAuth-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-19 09:25:10.000000 OpenAIAuth-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:25:33.394474 OpenAIAuth-3.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:25:33.394474 OpenAIAuth-3.0.0/src/OpenAIAuth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-19 09:25:33.000000 OpenAIAuth-3.0.0/src/OpenAIAuth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-19 09:25:33.000000 OpenAIAuth-3.0.0/src/OpenAIAuth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 09:25:33.000000 OpenAIAuth-3.0.0/src/OpenAIAuth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-19 09:25:33.000000 OpenAIAuth-3.0.0/src/OpenAIAuth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-19 09:25:33.000000 OpenAIAuth-3.0.0/src/OpenAIAuth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12444 2023-07-19 09:25:10.000000 OpenAIAuth-3.0.0/src/OpenAIAuth.py
```

### Comparing `OpenAIAuth-2.0.0/LICENSE` & `OpenAIAuth-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `OpenAIAuth-2.0.0/PKG-INFO` & `OpenAIAuth-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenAIAuth
-Version: 2.0.0
+Version: 3.0.0
 Summary: OpenAI Authentication Reverse Engineered
 Home-page: https://github.com/acheong08/OpenAIAuth
 Author: pengzhile
 Author-email: acheong@student.dalat.org
 License: MIT
 Project-URL: Bug Report, https://github.com/acheong08/OpenAIAuth/issues/new
 Classifier: License :: OSI Approved :: MIT License
@@ -23,15 +23,15 @@
 # OpenAIAuth
 Fetch access tokens for chat.openai.com
 
 ## Python version
 ```py
 from OpenAIAuth import Auth0
 auth = Auth0(email="example@example.com", password="example_password")
-access_token = auth.auth()
+access_token = auth.get_access_token()
 ```
 
 ## Go version
 ```go
 package main
 
 import (
```

### Comparing `OpenAIAuth-2.0.0/README.md` & `OpenAIAuth-3.0.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # OpenAIAuth
 Fetch access tokens for chat.openai.com
 
 ## Python version
 ```py
 from OpenAIAuth import Auth0
 auth = Auth0(email="example@example.com", password="example_password")
-access_token = auth.auth()
+access_token = auth.get_access_token()
 ```
 
 ## Go version
 ```go
 package main
 
 import (
```

### Comparing `OpenAIAuth-2.0.0/setup.py` & `OpenAIAuth-3.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name="OpenAIAuth",
-    version="2.0.0",
+    version="3.0.0",
     license="MIT",
     author="pengzhile",
     author_email="acheong@student.dalat.org",
     description="OpenAI Authentication Reverse Engineered",
     packages=find_packages("src"),
     package_dir={"": "src"},
     py_modules=["OpenAIAuth"],
     url="https://github.com/acheong08/OpenAIAuth",
     project_urls={"Bug Report": "https://github.com/acheong08/OpenAIAuth/issues/new"},
     install_requires=[
-        "requests",
+        "tls_client",
     ],
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Intended Audience :: Developers",
         "Natural Language :: English",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Programming Language :: Python :: 3 :: Only",
```

### Comparing `OpenAIAuth-2.0.0/src/OpenAIAuth.egg-info/PKG-INFO` & `OpenAIAuth-3.0.0/src/OpenAIAuth.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenAIAuth
-Version: 2.0.0
+Version: 3.0.0
 Summary: OpenAI Authentication Reverse Engineered
 Home-page: https://github.com/acheong08/OpenAIAuth
 Author: pengzhile
 Author-email: acheong@student.dalat.org
 License: MIT
 Project-URL: Bug Report, https://github.com/acheong08/OpenAIAuth/issues/new
 Classifier: License :: OSI Approved :: MIT License
@@ -23,15 +23,15 @@
 # OpenAIAuth
 Fetch access tokens for chat.openai.com
 
 ## Python version
 ```py
 from OpenAIAuth import Auth0
 auth = Auth0(email="example@example.com", password="example_password")
-access_token = auth.auth()
+access_token = auth.get_access_token()
 ```
 
 ## Go version
 ```go
 package main
 
 import (
```

### Comparing `OpenAIAuth-2.0.0/src/OpenAIAuth.py` & `OpenAIAuth-3.0.0/src/OpenAIAuth.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,271 +1,347 @@
-# -*- coding: utf-8 -*-
-# By @pengzhile on GitHub
-
-import datetime
+# Credits to github.com/rawandahmad698/PyChatGPT
 import re
-from datetime import datetime as dt
-from os import getenv
-from urllib.parse import urlparse, parse_qs
+import os
+import urllib
+
+import tls_client as requests
+
 
-import requests
-from certifi import where
+class Error(Exception):
+    """
+    Base error class
+    """
+
+    location: str
+    status_code: int
+    details: str
+
+    def __init__(self, location: str, status_code: int, details: str):
+        self.location = location
+        self.status_code = status_code
+        self.details = details
 
 
 class Auth0:
+    """
+    OpenAI Authentication Reverse Engineered
+    """
+
     def __init__(
         self,
-        email: str,
+        email_address: str,
         password: str,
+        puid: str = None,
         proxy: str = None,
-        mfa: str = None,
     ):
-        """
-        Initializes an instance of the Auth0 class.
-
-        Args:
-        - email (str): The email address of the user.
-        - password (str): The password of the user.
-        - proxy (str, optional): The proxy server to use for requests. Defaults to None.
-        - mfa (str, optional): The multi-factor authentication method. Defaults to None.
-        """
-        self.session_token = None
-        self.email = email
+        puid = puid or os.environ.get("PUID")
+        # if not puid:
+        #     raise ValueError("PUID is required")
+        self.email_address = email_address
         self.password = password
-        self.mfa = mfa
-        self.session = requests.Session()
-        self.req_kwargs = {
-            "proxies": {
-                "http": proxy,
-                "https": proxy,
-            }
-            if proxy
-            else None,
-            "verify": where(),
-            "timeout": 100,
-        }
-        self.access_token = None
-        self.expires = None
-        self.user_agent = (
-            "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) "
-            "Chrome/109.0.0.0 Safari/537.36"
+        self.proxy = proxy
+        self.session = requests.Session(
+            client_identifier="chrome112",
+            random_tls_extension_order=True,
         )
+        proxies = {
+            "http": self.proxy,
+            "https": self.proxy,
+        }
+        self.session.proxies.update(proxies)
+        self.access_token: str = None
+        self.user_agent = "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/109.0.0.0 Safari/537.36"
+        self.session.cookies.set("_puid", puid)
 
     @staticmethod
-    def __check_email(email: str):
-        regex = r"\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,7}\b"
-        return re.fullmatch(regex, email)
-
-    def get_access_token(self) -> str:
+    def url_encode(string: str) -> str:
         """
-        Authenticates the user and returns the access token.
-
-        Returns:
-        - str: The access token.
+        URL encode a string
+        :param string:
+        :return:
         """
+        return urllib.parse.quote(string)
 
-        if not self.__check_email(self.email) or not self.password:
-            raise Exception("invalid email or password.")
-
-        return self.__part_two()
-
-    def __part_two(self) -> str:
-        code_challenge = "w6n3Ix420Xhhu-Q5-mOOEyuPZmAsJHUbBpO8Ub7xBCY"
-        code_verifier = "yGrXROHx_VazA0uovsxKfE263LMFcrSrdm4SlC-rob8"
-
-        url = (
-            "https://auth0.openai.com/authorize?client_id=pdlLIX2Y72MIl2rhLhTE9VV9bN905kBh&audience=https%3A%2F"
-            "%2Fapi.openai.com%2Fv1&redirect_uri=com.openai.chat%3A%2F%2Fauth0.openai.com%2Fios%2Fcom.openai.chat"
-            "%2Fcallback&scope=openid%20email%20profile%20offline_access%20model.request%20model.read"
-            "%20organization.read%20offline&response_type=code&code_challenge={}"
-            "&code_challenge_method=S256&prompt=login".format(code_challenge)
-        )
-        return self.__part_three(code_verifier, url)
-
-    def __part_three(self, code_verifier, url: str) -> str:
+    def begin(self) -> None:
+        """
+        In part two, We make a request to https://chat.openai.com/api/auth/csrf and grab a fresh csrf token
+        """
+        url = "https://chat.openai.com/api/auth/csrf"
         headers = {
+            "Host": "chat.openai.com",
+            "Accept": "*/*",
+            "Connection": "keep-alive",
             "User-Agent": self.user_agent,
-            "Referer": "https://ios.chat.openai.com/",
-        }
-        resp = self.session.get(
-            url, headers=headers, allow_redirects=True, **self.req_kwargs
+            "Accept-Language": "en-GB,en-US;q=0.9,en;q=0.8",
+            "Referer": "https://chat.openai.com/auth/login",
+            "Accept-Encoding": "gzip, deflate, br",
+        }
+        response = self.session.get(
+            url=url,
+            headers=headers,
         )
-
-        if resp.status_code == 200:
-            try:
-                url_params = parse_qs(urlparse(resp.url).query)
-                state = url_params["state"][0]
-                return self.__part_four(code_verifier, state)
-            except IndexError as exc:
-                raise Exception("Rate limit hit.") from exc
+        if response.status_code == 200 and "json" in response.headers["Content-Type"]:
+            csrf_token = response.json()["csrfToken"]
+            # self.session.cookies.set("__Host-next-auth.csrf-token", csrf_token)
+            self.__part_one(token=csrf_token)
         else:
-            raise Exception("Error request login url.")
+            error = Error(
+                location="begin",
+                status_code=response.status_code,
+                details=response.text,
+            )
+            print(error.details)
+            raise error
 
-    def __part_four(self, code_verifier: str, state: str) -> str:
-        url = "https://auth0.openai.com/u/login/identifier?state=" + state
+    def __part_one(self, token: str) -> None:
+        """
+        We reuse the token from part to make a request to /api/auth/signin/auth0?prompt=login
+        """
+        url = "https://chat.openai.com/api/auth/signin/auth0?prompt=login"
+        payload = f"callbackUrl=%2F&csrfToken={token}&json=true"
         headers = {
+            "Host": "chat.openai.com",
             "User-Agent": self.user_agent,
-            "Referer": url,
-            "Origin": "https://auth0.openai.com",
-        }
-        data = {
-            "state": state,
-            "username": self.email,
-            "js-available": "true",
-            "webauthn-available": "true",
-            "is-brave": "false",
-            "webauthn-platform-available": "false",
-            "action": "default",
-        }
-        resp = self.session.post(
-            url, headers=headers, data=data, allow_redirects=False, **self.req_kwargs
-        )
-
-        if resp.status_code == 302:
-            return self.__part_five(code_verifier, state)
+            "Content-Type": "application/x-www-form-urlencoded",
+            "Accept": "*/*",
+            "Sec-Gpc": "1",
+            "Accept-Language": "en-US,en;q=0.8",
+            "Origin": "https://chat.openai.com",
+            "Sec-Fetch-Site": "same-origin",
+            "Sec-Fetch-Mode": "cors",
+            "Sec-Fetch-Dest": "empty",
+            "Referer": "https://chat.openai.com/auth/login",
+            "Accept-Encoding": "gzip, deflate",
+            #
+        }
+        response = self.session.post(url=url, headers=headers, data=payload)
+        if response.status_code == 200 and "json" in response.headers["Content-Type"]:
+            url = response.json()["url"]
+            if (
+                url == "https://chat.openai.com/api/auth/error?error=OAuthSignin"
+                or "error" in url
+            ):
+                error = Error(
+                    location="__part_one",
+                    status_code=response.status_code,
+                    details="You have been rate limited. Please try again later.",
+                )
+                raise error
+            self.__part_two(url=url)
         else:
-            raise Exception("Error check email.")
+            error = Error(
+                location="__part_one",
+                status_code=response.status_code,
+                details=response.text,
+            )
+            raise error
 
-    def __part_five(self, code_verifier: str, state: str) -> str:
-        url = "https://auth0.openai.com/u/login/password?state=" + state
+    def __part_two(self, url: str) -> None:
+        """
+        We make a GET request to url
+        :param url:
+        :return:
+        """
         headers = {
+            "Host": "auth0.openai.com",
+            "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8",
+            "Connection": "keep-alive",
             "User-Agent": self.user_agent,
-            "Referer": url,
-            "Origin": "https://auth0.openai.com",
+            "Accept-Language": "en-US,en;q=0.9",
+            "Referer": "https://chat.openai.com/",
         }
-        data = {
-            "state": state,
-            "username": self.email,
-            "password": self.password,
-            "action": "default",
-        }
-
-        resp = self.session.post(
-            url, headers=headers, data=data, allow_redirects=False, **self.req_kwargs
+        response = self.session.get(
+            url=url,
+            headers=headers,
         )
-        if resp.status_code == 302:
-            location = resp.headers["Location"]
-            if not location.startswith("/authorize/resume?"):
-                raise Exception("Login failed.")
-
-            return self.__part_six(code_verifier, location, url)
-
-        if resp.status_code == 400:
-            raise Exception("Wrong email or password.")
+        if response.status_code == 302 or response.status_code == 200:
+            state = re.findall(r"state=(.*)", response.text)[0]
+            state = state.split('"')[0]
+            self.__part_three(state=state)
         else:
-            raise Exception("Error login.")
+            error = Error(
+                location="__part_two",
+                status_code=response.status_code,
+                details=response.text,
+            )
+            raise error
+
+    def __part_three(self, state: str) -> None:
+        """
+        We use the state to get the login page
+        """
+        url = f"https://auth0.openai.com/u/login/identifier?state={state}"
 
-    def __part_six(self, code_verifier: str, location: str, ref: str) -> str:
-        url = "https://auth0.openai.com" + location
         headers = {
+            "Host": "auth0.openai.com",
+            "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8",
+            "Connection": "keep-alive",
             "User-Agent": self.user_agent,
-            "Referer": ref,
+            "Accept-Language": "en-US,en;q=0.9",
+            "Referer": "https://chat.openai.com/",
         }
+        response = self.session.get(url, headers=headers)
+        if response.status_code == 200:
+            self.__part_four(state=state)
+        else:
+            error = Error(
+                location="__part_three",
+                status_code=response.status_code,
+                details=response.text,
+            )
+            raise error
 
-        resp = self.session.get(
-            url, headers=headers, allow_redirects=False, **self.req_kwargs
-        )
-        if resp.status_code == 302:
-            location = resp.headers["Location"]
-            if location.startswith("/u/mfa-otp-challenge?"):
-                if not self.mfa:
-                    raise Exception("MFA required.")
-                return self.__part_seven(code_verifier, location)
-
-            if not location.startswith(
-                "com.openai.chat://auth0.openai.com/ios/com.openai.chat/callback?"
-            ):
-                raise Exception("Login callback failed.")
-
-            return self.__get_access_token(code_verifier, resp.headers["Location"])
+    def __part_four(self, state: str) -> None:
+        """
+        We make a POST request to the login page with the captcha, email
+        :param state:
+        :return:
+        """
+        url = f"https://auth0.openai.com/u/login/identifier?state={state}"
+        email_url_encoded = self.url_encode(self.email_address)
 
-        raise Exception("Error login.")
+        payload = (
+            f"state={state}&username={email_url_encoded}&js-available=false&webauthn-available=true&is"
+            f"-brave=false&webauthn-platform-available=true&action=default "
+        )
 
-    def __part_seven(self, code_verifier: str, location: str) -> str:
-        url = "https://auth0.openai.com" + location
-        data = {
-            "state": parse_qs(urlparse(url).query)["state"][0],
-            "code": self.mfa,
-            "action": "default",
-        }
         headers = {
-            "User-Agent": self.user_agent,
-            "Referer": url,
+            "Host": "auth0.openai.com",
             "Origin": "https://auth0.openai.com",
-        }
-
-        resp = self.session.post(
-            url, headers=headers, data=data, allow_redirects=False, **self.req_kwargs
+            "Connection": "keep-alive",
+            "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8",
+            "User-Agent": self.user_agent,
+            "Referer": f"https://auth0.openai.com/u/login/identifier?state={state}",
+            "Accept-Language": "en-US,en;q=0.9",
+            "Content-Type": "application/x-www-form-urlencoded",
+        }
+        response = self.session.post(
+            url,
+            headers=headers,
+            data=payload,
         )
-        if resp.status_code == 302:
-            location = resp.headers["Location"]
-            if not location.startswith("/authorize/resume?"):
-                raise Exception("MFA failed.")
-
-            return self.__part_six(code_verifier, location, url)
-
-        if resp.status_code == 400:
-            raise Exception("Wrong MFA code.")
+        if response.status_code == 302 or response.status_code == 200:
+            self.__part_five(state=state)
         else:
-            raise Exception("Error login.")
+            error = Error(
+                location="__part_four",
+                status_code=response.status_code,
+                details="Your email address is invalid.",
+            )
+            raise error
 
-    def __get_access_token(self, code_verifier: str, callback_url: str) -> str:
-        url_params = parse_qs(urlparse(callback_url).query)
+    def __part_five(self, state: str) -> None:
+        """
+        We enter the password
+        :param state:
+        :return:
+        """
 
-        if "error" in url_params:
-            error = url_params["error"][0]
-            error_description = (
-                url_params["error_description"][0]
-                if "error_description" in url_params
-                else ""
+        email_url_encoded = self.url_encode(self.email_address)
+        password_url_encoded = self.url_encode(self.password)
+        payload = f"state={state}&username={email_url_encoded}&password={password_url_encoded}&action=default"
+        url = f"https://auth0.openai.com/u/login/password?state={state}"
+        headers = {
+            "Host": "auth0.openai.com",
+            "Origin": "https://auth0.openai.com",
+            "Connection": "keep-alive",
+            "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8",
+            "User-Agent": self.user_agent,
+            "Referer": f"https://auth0.openai.com/u/login/password?state={state}",
+            "Accept-Language": "en-US,en;q=0.9",
+            "Content-Type": "application/x-www-form-urlencoded",
+        }
+        response = self.session.post(
+            url,
+            headers=headers,
+            allow_redirects=False,
+            data=payload,
+        )
+        if response.status_code == 302:
+            redirect_url = response.headers.get("Location")
+            self.__part_six(old_state=state, redirect_url=redirect_url)
+        else:
+            error = Error(
+                location="__part_five",
+                status_code=response.status_code,
+                details="Your credentials are invalid.",
             )
-            raise Exception("{}: {}".format(error, error_description))
-
-        if "code" not in url_params:
-            raise Exception("Error get code from callback url.")
+            raise error
 
-        url = "https://auth0.openai.com/oauth/token"
+    def __part_six(self, old_state: str, redirect_url) -> None:
+        url = "https://auth0.openai.com" + redirect_url
         headers = {
+            "Host": "auth0.openai.com",
+            "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8",
+            "Connection": "keep-alive",
             "User-Agent": self.user_agent,
+            "Accept-Language": "en-GB,en-US;q=0.9,en;q=0.8",
+            "Referer": f"https://auth0.openai.com/u/login/password?state={old_state}",
         }
-        data = {
-            "redirect_uri": "com.openai.chat://auth0.openai.com/ios/com.openai.chat/callback",
-            "grant_type": "authorization_code",
-            "client_id": "pdlLIX2Y72MIl2rhLhTE9VV9bN905kBh",
-            "code": url_params["code"][0],
-            "code_verifier": code_verifier,
-        }
-        resp = self.session.post(
-            url, headers=headers, json=data, allow_redirects=False, **self.req_kwargs
-        )
+        response = self.session.get(url, headers=headers, allow_redirects=False)
+        if response.status_code == 302:
+            redirect_url = response.headers.get("Location")
+            self.__part_seven(redirect_url=redirect_url, previous_url=url)
+        else:
+            error = Error(
+                location="__part_six",
+                status_code=response.status_code,
+                details=response.text,
+            )
+            raise error
 
-        if resp.status_code == 200:
-            json = resp.json()
-            if "access_token" not in json:
-                raise Exception("Get access token failed, maybe you need a proxy.")
-
-            self.access_token = json["access_token"]
-            self.expires = (
-                dt.utcnow()
-                + datetime.timedelta(seconds=json["expires_in"])
-                - datetime.timedelta(minutes=5)
+    def __part_seven(self, redirect_url: str, previous_url: str) -> None:
+        url = redirect_url
+        headers = {
+            "Host": "chat.openai.com",
+            "Accept": "application/json",
+            "Connection": "keep-alive",
+            "User-Agent": self.user_agent,
+            "Accept-Language": "en-GB,en-US;q=0.9,en;q=0.8",
+            "Referer": previous_url,
+        }
+        response = self.session.get(url, headers=headers, allow_redirects=True)
+        if response.status_code == 200:
+            return
+        else:
+            error = Error(
+                location="__part_seven",
+                status_code=response.status_code,
+                details=response.text,
             )
+            raise error
+
+    def get_access_token(self):
+        """
+        Gets access token
+        """
+        self.begin()
+        response = self.session.get(
+            "https://chat.openai.com/api/auth/session",
+        )
+        if response.status_code == 200:
+            self.access_token = response.json().get("accessToken")
             return self.access_token
         else:
-            raise Exception(resp.text)
+            error = Error(
+                location="get_access_token",
+                status_code=response.status_code,
+                details=response.text,
+            )
+            raise error
 
     def get_puid(self) -> str:
-        url = "https://bypass.churchless.tech/models"
+        url = os.getenv("OPENAI_MODELS_URL", "https://bypass.churchless.tech/models")
         headers = {
             "Authorization": "Bearer " + self.access_token,
         }
-        resp = self.session.get(url, headers=headers, **self.req_kwargs)
+        resp = self.session.get(url, headers=headers)
         if resp.status_code == 200:
             # Get _puid cookie
-            puid = resp.headers.get("set-cookie", "")
+            puid = resp.headers.get("Set-Cookie", "")
             if not puid:
                 raise Exception("Get _puid cookie failed.")
             self.puid = puid.split("_puid=")[1].split(";")[0]
             return self.puid
         else:
             raise Exception(resp.text)
```

