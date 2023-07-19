# Comparing `tmp/LolzteamApi-1.0.20.tar.gz` & `tmp/LolzteamApi-1.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LolzteamApi-1.0.20.tar", last modified: Tue Jul 18 11:40:17 2023, max compression
+gzip compressed data, was "LolzteamApi-1.0.21.tar", last modified: Wed Jul 19 12:30:30 2023, max compression
```

## Comparing `LolzteamApi-1.0.20.tar` & `LolzteamApi-1.0.21.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 11:40:17.042615 LolzteamApi-1.0.20/
--rw-rw-rw-   0        0        0     1089 2023-07-08 18:11:39.000000 LolzteamApi-1.0.20/LICENSE
-drwxrwxrwx   0        0        0        0 2023-07-18 11:40:17.034616 LolzteamApi-1.0.20/LolzteamApi/
--rw-rw-rw-   0        0        0   179761 2023-07-18 11:32:30.000000 LolzteamApi-1.0.20/LolzteamApi/LolzteamApi.py
--rw-rw-rw-   0        0        0       43 2023-07-15 08:07:56.000000 LolzteamApi-1.0.20/LolzteamApi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 11:40:17.040615 LolzteamApi-1.0.20/LolzteamApi.egg-info/
--rw-rw-rw-   0        0        0     2262 2023-07-18 11:40:16.000000 LolzteamApi-1.0.20/LolzteamApi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-07-18 11:40:16.000000 LolzteamApi-1.0.20/LolzteamApi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 11:40:16.000000 LolzteamApi-1.0.20/LolzteamApi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-07-18 11:40:16.000000 LolzteamApi-1.0.20/LolzteamApi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-18 11:40:16.000000 LolzteamApi-1.0.20/LolzteamApi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2262 2023-07-18 11:40:17.041616 LolzteamApi-1.0.20/PKG-INFO
--rw-rw-rw-   0        0        0     1860 2023-07-10 01:19:44.000000 LolzteamApi-1.0.20/README.md
--rw-rw-rw-   0        0        0       42 2023-07-18 11:40:17.042615 LolzteamApi-1.0.20/setup.cfg
--rw-rw-rw-   0        0        0      695 2023-07-18 11:32:42.000000 LolzteamApi-1.0.20/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 12:30:30.255895 LolzteamApi-1.0.21/
+-rw-rw-rw-   0        0        0     1089 2023-07-08 18:11:39.000000 LolzteamApi-1.0.21/LICENSE
+drwxrwxrwx   0        0        0        0 2023-07-19 12:30:30.248902 LolzteamApi-1.0.21/LolzteamApi/
+-rw-rw-rw-   0        0        0   179777 2023-07-19 12:29:06.000000 LolzteamApi-1.0.21/LolzteamApi/LolzteamApi.py
+-rw-rw-rw-   0        0        0       43 2023-07-15 08:07:56.000000 LolzteamApi-1.0.21/LolzteamApi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 12:30:30.253898 LolzteamApi-1.0.21/LolzteamApi.egg-info/
+-rw-rw-rw-   0        0        0     2262 2023-07-19 12:30:29.000000 LolzteamApi-1.0.21/LolzteamApi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-07-19 12:30:29.000000 LolzteamApi-1.0.21/LolzteamApi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 12:30:29.000000 LolzteamApi-1.0.21/LolzteamApi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-07-19 12:30:29.000000 LolzteamApi-1.0.21/LolzteamApi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-19 12:30:29.000000 LolzteamApi-1.0.21/LolzteamApi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2262 2023-07-19 12:30:30.254894 LolzteamApi-1.0.21/PKG-INFO
+-rw-rw-rw-   0        0        0     1860 2023-07-10 01:19:44.000000 LolzteamApi-1.0.21/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-19 12:30:30.256897 LolzteamApi-1.0.21/setup.cfg
+-rw-rw-rw-   0        0        0      695 2023-07-19 12:30:02.000000 LolzteamApi-1.0.21/setup.py
```

### Comparing `LolzteamApi-1.0.20/LICENSE` & `LolzteamApi-1.0.21/LICENSE`

 * *Files identical despite different names*

### Comparing `LolzteamApi-1.0.20/LolzteamApi/LolzteamApi.py` & `LolzteamApi-1.0.21/LolzteamApi/LolzteamApi.py`

 * *Files 0% similar despite different names*

```diff
@@ -3978,15 +3978,15 @@
                     "password": password,
                     "login_password": login_password,
                     "close_item": close_item,
                     "extra": extra,
                     "resell_item_id": resell_item_id,
                     "random_proxy": random_proxy
                 }
-                for key, value in extra:
+                for key, value in extra.items():
                     es = f"extra[{key}]"
                     params[es] = value
                 return LolzteamApi.send_request(self=self.__api, method="POST", url=url, params=params)
 
             def add(self, category_id: int, price: int, currency: str, item_origin: str, extended_guarantee: int,
                     title: str = None, title_en: str = None, description: str = None, information: str = None,
                     has_email_login_data: bool = None, email_login_data: str = None, email_type: str = None,
@@ -4144,15 +4144,15 @@
                     "allow_ask_discount": allow_ask_discount,
                     "proxy_id": proxy_id,
                     "random_proxy": random_proxy,
                     "login": login,
                     "password": password,
                     "login_password": login_password
                 }
-                for key, value in extra:
+                for key, value in extra.items():
                     es = f"extra[{key}]"
                     params[es] = value
                 return LolzteamApi.send_request(self=self.__api, method="POST", url=url, params=params)
 
             # Copy of __Managing.edit
             def edit(self, item_id: int, price: int = None, currency: str = None, item_origin: str = None,
                      title: str = None, title_en: str = None, description: str = None, information: str = None,
```

### Comparing `LolzteamApi-1.0.20/LolzteamApi.egg-info/PKG-INFO` & `LolzteamApi-1.0.21/LolzteamApi.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LolzteamApi
-Version: 1.0.20
+Version: 1.0.21
 Summary: A library that contains all the methods of the Lolzteam API (Market/Forum)
 Home-page: https://github.com/AS7RIDENIED/Lolzteam_Python_Api
 Author: AS7RID
 Author-email: as7ridwork@gmail.com
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: LolzteamApi Version: 1.0.20 Summary: A library that
+Metadata-Version: 2.1 Name: LolzteamApi Version: 1.0.21 Summary: A library that
 contains all the methods of the Lolzteam API (Market/Forum) Home-page: https://
 github.com/AS7RIDENIED/Lolzteam_Python_Api Author: AS7RID Author-email:
 as7ridwork@gmail.com Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
 LICENSE # Lolzteam Python API
                              [Material_Bread_logo]
 [![Static Badge](https://img.shields.io/badge/DONATE-LOLZTEAM-
```

### Comparing `LolzteamApi-1.0.20/PKG-INFO` & `LolzteamApi-1.0.21/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LolzteamApi
-Version: 1.0.20
+Version: 1.0.21
 Summary: A library that contains all the methods of the Lolzteam API (Market/Forum)
 Home-page: https://github.com/AS7RIDENIED/Lolzteam_Python_Api
 Author: AS7RID
 Author-email: as7ridwork@gmail.com
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: LolzteamApi Version: 1.0.20 Summary: A library that
+Metadata-Version: 2.1 Name: LolzteamApi Version: 1.0.21 Summary: A library that
 contains all the methods of the Lolzteam API (Market/Forum) Home-page: https://
 github.com/AS7RIDENIED/Lolzteam_Python_Api Author: AS7RID Author-email:
 as7ridwork@gmail.com Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
 LICENSE # Lolzteam Python API
                              [Material_Bread_logo]
 [![Static Badge](https://img.shields.io/badge/DONATE-LOLZTEAM-
```

### Comparing `LolzteamApi-1.0.20/README.md` & `LolzteamApi-1.0.21/README.md`

 * *Files identical despite different names*

### Comparing `LolzteamApi-1.0.20/setup.py` & `LolzteamApi-1.0.21/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 requirements = ["requests", "beautifulsoup4"]
 
 setuptools.setup(
     name="LolzteamApi",
-    version="1.0.20",
+    version="1.0.21",
     author="AS7RID",
     author_email="as7ridwork@gmail.com",
     description="A library that contains all the methods of the Lolzteam API (Market/Forum)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AS7RIDENIED/Lolzteam_Python_Api",
     packages=setuptools.find_packages(),
```

