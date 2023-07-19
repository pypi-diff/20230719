# Comparing `tmp/understar-2.4.tar.gz` & `tmp/understar-2.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "understar-2.4.tar", last modified: Wed Jul 19 05:48:05 2023, max compression
+gzip compressed data, was "understar-2.41.tar", last modified: Wed Jul 19 06:28:26 2023, max compression
```

## Comparing `understar-2.4.tar` & `understar-2.41.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-19 05:48:05.418703 understar-2.4/
--rw-r--r--   0 maxence    (501) staff       (20)     1188 2023-05-26 01:06:57.000000 understar-2.4/LICENSE.md
--rw-r--r--   0 maxence    (501) staff       (20)      589 2023-07-19 05:48:05.418583 understar-2.4/PKG-INFO
--rw-r--r--   0 maxence    (501) staff       (20)       45 2023-05-26 01:06:57.000000 understar-2.4/README.md
--rw-r--r--   0 maxence    (501) staff       (20)       38 2023-07-19 05:48:05.418753 understar-2.4/setup.cfg
--rw-r--r--   0 maxence    (501) staff       (20)     1885 2023-07-19 05:42:26.000000 understar-2.4/setup.py
-drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-19 05:48:05.414945 understar-2.4/understar/
--rw-r--r--   0 maxence    (501) staff       (20)        4 2023-07-19 05:47:53.000000 understar-2.4/understar/.version
--rw-r--r--   0 maxence    (501) staff       (20)       25 2023-07-19 04:14:38.000000 understar-2.4/understar/__init__.py
-drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-19 05:48:05.415856 understar-2.4/understar/system/
--rw-r--r--   0 maxence    (501) staff       (20)       22 2023-07-16 04:49:43.000000 understar-2.4/understar/system/__init__.py
-drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-19 05:48:05.415997 understar-2.4/understar/system/app/
--rw-r--r--   0 maxence    (501) staff       (20)       89 2023-07-16 04:47:12.000000 understar-2.4/understar/system/app/__init__.py
-drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-19 05:48:05.416137 understar-2.4/understar/system/app/config/
--rw-r--r--   0 maxence    (501) staff       (20)    20066 2023-07-19 04:34:41.000000 understar-2.4/understar/system/app/config/__init__.py
-drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-19 05:48:05.416599 understar-2.4/understar/system/app/config/apt/
--rw-r--r--   0 maxence    (501) staff       (20)       32 2023-07-12 03:26:34.000000 understar-2.4/understar/system/app/config/apt/__init__.py
--rw-r--r--   0 maxence    (501) staff       (20)     3351 2023-07-19 04:34:43.000000 understar-2.4/understar/system/app/config/apt/install.py
--rw-r--r--   0 maxence    (501) staff       (20)     1329 2023-07-19 04:34:44.000000 understar-2.4/understar/system/app/config/apt/uninstall.py
-drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-19 05:48:05.416726 understar-2.4/understar/system/app/maintenance/
--rw-r--r--   0 maxence    (501) staff       (20)      902 2023-07-19 04:34:46.000000 understar-2.4/understar/system/app/maintenance/__init__.py
-drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-19 05:48:05.418154 understar-2.4/understar/system/lib/
--rw-r--r--   0 maxence    (501) staff       (20)      149 2023-07-12 03:30:52.000000 understar-2.4/understar/system/lib/__init__.py
--rw-r--r--   0 maxence    (501) staff       (20)     5517 2023-07-19 02:04:00.000000 understar-2.4/understar/system/lib/app.py
--rw-r--r--   0 maxence    (501) staff       (20)     1015 2023-06-23 09:10:23.000000 understar-2.4/understar/system/lib/com.py
--rw-r--r--   0 maxence    (501) staff       (20)    11757 2023-06-19 00:59:20.000000 understar-2.4/understar/system/lib/event.py
--rw-r--r--   0 maxence    (501) staff       (20)     3784 2023-06-19 05:27:26.000000 understar-2.4/understar/system/lib/save.py
--rw-r--r--   0 maxence    (501) staff       (20)     2716 2023-07-19 04:01:29.000000 understar-2.4/understar/system/lib/store.py
--rw-r--r--   0 maxence    (501) staff       (20)      174 2023-06-23 09:10:04.000000 understar-2.4/understar/system/lib/types.py
--rw-r--r--   0 maxence    (501) staff       (20)     5127 2023-07-19 05:03:32.000000 understar-2.4/understar/system/lib/utils.py
--rw-r--r--   0 maxence    (501) staff       (20)    31108 2023-07-19 04:20:00.000000 understar-2.4/understar/understar.py
-drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-19 05:48:05.415702 understar-2.4/understar.egg-info/
--rw-r--r--   0 maxence    (501) staff       (20)      589 2023-07-19 05:48:05.000000 understar-2.4/understar.egg-info/PKG-INFO
--rw-r--r--   0 maxence    (501) staff       (20)      774 2023-07-19 05:48:05.000000 understar-2.4/understar.egg-info/SOURCES.txt
--rw-r--r--   0 maxence    (501) staff       (20)        1 2023-07-19 05:48:05.000000 understar-2.4/understar.egg-info/dependency_links.txt
--rw-r--r--   0 maxence    (501) staff       (20)       49 2023-07-19 05:48:05.000000 understar-2.4/understar.egg-info/requires.txt
--rw-r--r--   0 maxence    (501) staff       (20)       10 2023-07-19 05:48:05.000000 understar-2.4/understar.egg-info/top_level.txt
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-19 06:28:26.136985 understar-2.41/
+-rw-r--r--   0 maxence    (501) staff       (20)     1188 2023-05-26 01:06:57.000000 understar-2.41/LICENSE.md
+-rw-r--r--   0 maxence    (501) staff       (20)      590 2023-07-19 06:28:26.136835 understar-2.41/PKG-INFO
+-rw-r--r--   0 maxence    (501) staff       (20)       45 2023-05-26 01:06:57.000000 understar-2.41/README.md
+-rw-r--r--   0 maxence    (501) staff       (20)       38 2023-07-19 06:28:26.137030 understar-2.41/setup.cfg
+-rw-r--r--   0 maxence    (501) staff       (20)     1885 2023-07-19 05:42:26.000000 understar-2.41/setup.py
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-19 06:28:26.128643 understar-2.41/understar/
+-rw-r--r--   0 maxence    (501) staff       (20)        5 2023-07-19 06:28:06.000000 understar-2.41/understar/.version
+-rw-r--r--   0 maxence    (501) staff       (20)       25 2023-07-19 04:14:38.000000 understar-2.41/understar/__init__.py
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-19 06:28:26.129693 understar-2.41/understar/system/
+-rw-r--r--   0 maxence    (501) staff       (20)       22 2023-07-16 04:49:43.000000 understar-2.41/understar/system/__init__.py
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-19 06:28:26.130056 understar-2.41/understar/system/app/
+-rw-r--r--   0 maxence    (501) staff       (20)       89 2023-07-16 04:47:12.000000 understar-2.41/understar/system/app/__init__.py
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-19 06:28:26.130382 understar-2.41/understar/system/app/config/
+-rw-r--r--   0 maxence    (501) staff       (20)    20066 2023-07-19 04:34:41.000000 understar-2.41/understar/system/app/config/__init__.py
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-19 06:28:26.131228 understar-2.41/understar/system/app/config/apt/
+-rw-r--r--   0 maxence    (501) staff       (20)       32 2023-07-12 03:26:34.000000 understar-2.41/understar/system/app/config/apt/__init__.py
+-rw-r--r--   0 maxence    (501) staff       (20)     3351 2023-07-19 04:34:43.000000 understar-2.41/understar/system/app/config/apt/install.py
+-rw-r--r--   0 maxence    (501) staff       (20)     1329 2023-07-19 04:34:44.000000 understar-2.41/understar/system/app/config/apt/uninstall.py
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-19 06:28:26.131468 understar-2.41/understar/system/app/maintenance/
+-rw-r--r--   0 maxence    (501) staff       (20)      902 2023-07-19 04:34:46.000000 understar-2.41/understar/system/app/maintenance/__init__.py
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-19 06:28:26.136283 understar-2.41/understar/system/lib/
+-rw-r--r--   0 maxence    (501) staff       (20)      149 2023-07-12 03:30:52.000000 understar-2.41/understar/system/lib/__init__.py
+-rw-r--r--   0 maxence    (501) staff       (20)     5517 2023-07-19 02:04:00.000000 understar-2.41/understar/system/lib/app.py
+-rw-r--r--   0 maxence    (501) staff       (20)     1015 2023-06-23 09:10:23.000000 understar-2.41/understar/system/lib/com.py
+-rw-r--r--   0 maxence    (501) staff       (20)    11757 2023-06-19 00:59:20.000000 understar-2.41/understar/system/lib/event.py
+-rw-r--r--   0 maxence    (501) staff       (20)     3784 2023-06-19 05:27:26.000000 understar-2.41/understar/system/lib/save.py
+-rw-r--r--   0 maxence    (501) staff       (20)     2716 2023-07-19 04:01:29.000000 understar-2.41/understar/system/lib/store.py
+-rw-r--r--   0 maxence    (501) staff       (20)      174 2023-06-23 09:10:04.000000 understar-2.41/understar/system/lib/types.py
+-rw-r--r--   0 maxence    (501) staff       (20)     5155 2023-07-19 06:27:08.000000 understar-2.41/understar/system/lib/utils.py
+-rw-r--r--   0 maxence    (501) staff       (20)    31108 2023-07-19 04:20:00.000000 understar-2.41/understar/understar.py
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-19 06:28:26.129530 understar-2.41/understar.egg-info/
+-rw-r--r--   0 maxence    (501) staff       (20)      590 2023-07-19 06:28:26.000000 understar-2.41/understar.egg-info/PKG-INFO
+-rw-r--r--   0 maxence    (501) staff       (20)      774 2023-07-19 06:28:26.000000 understar-2.41/understar.egg-info/SOURCES.txt
+-rw-r--r--   0 maxence    (501) staff       (20)        1 2023-07-19 06:28:26.000000 understar-2.41/understar.egg-info/dependency_links.txt
+-rw-r--r--   0 maxence    (501) staff       (20)       49 2023-07-19 06:28:26.000000 understar-2.41/understar.egg-info/requires.txt
+-rw-r--r--   0 maxence    (501) staff       (20)       10 2023-07-19 06:28:26.000000 understar-2.41/understar.egg-info/top_level.txt
```

### Comparing `understar-2.4/LICENSE.md` & `understar-2.41/LICENSE.md`

 * *Files identical despite different names*

### Comparing `understar-2.4/PKG-INFO` & `understar-2.41/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: understar
-Version: 2.4
+Version: 2.41
 Summary: A discord bot framewrok
 Home-page: https://github.com/GalTechDev/UnderStar-OS
 Download-URL: https://github.com/GalTechDev/UnderStar-OS/tarball/master
 Author: GalTech
 Author-email: poussigalitv@gmail.com
 License: MIT
 Keywords: discord,bot,discord.py,understar,os,framework
```

### Comparing `understar-2.4/setup.py` & `understar-2.41/setup.py`

 * *Files identical despite different names*

### Comparing `understar-2.4/understar/system/app/config/__init__.py` & `understar-2.41/understar/system/app/config/__init__.py`

 * *Files identical despite different names*

### Comparing `understar-2.4/understar/system/app/config/apt/install.py` & `understar-2.41/understar/system/app/config/apt/install.py`

 * *Files identical despite different names*

### Comparing `understar-2.4/understar/system/app/config/apt/uninstall.py` & `understar-2.41/understar/system/app/config/apt/uninstall.py`

 * *Files identical despite different names*

### Comparing `understar-2.4/understar/system/app/maintenance/__init__.py` & `understar-2.41/understar/system/app/maintenance/__init__.py`

 * *Files identical despite different names*

### Comparing `understar-2.4/understar/system/lib/app.py` & `understar-2.41/understar/system/lib/app.py`

 * *Files identical despite different names*

### Comparing `understar-2.4/understar/system/lib/com.py` & `understar-2.41/understar/system/lib/com.py`

 * *Files identical despite different names*

### Comparing `understar-2.4/understar/system/lib/event.py` & `understar-2.41/understar/system/lib/event.py`

 * *Files identical despite different names*

### Comparing `understar-2.4/understar/system/lib/save.py` & `understar-2.41/understar/system/lib/save.py`

 * *Files identical despite different names*

### Comparing `understar-2.4/understar/system/lib/store.py` & `understar-2.41/understar/system/lib/store.py`

 * *Files identical despite different names*

### Comparing `understar-2.4/understar/system/lib/utils.py` & `understar-2.41/understar/system/lib/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     try:
         await interaction.response.send_message()
     except Exception as error:
         pass
 
 chemin_fichier = pkg_resources.resource_filename(__name__, '.version')
 
-with open(chemin_fichier.removesuffix("system/lib/.version")+".version", 'r') as f:
+with open(os.path.join(chemin_fichier.removesuffix(os.path.join("system/lib/.version")),".version"), 'r') as f:
     BOT_VERSION = f.read()
 
 def import_module(folder: str, log=False, catch_error=True):
     # Parcours des apps dans le répertoire du package
     if log:
         print(f" * Import Module Start :")
     modules = {}
```

### Comparing `understar-2.4/understar/understar.py` & `understar-2.41/understar/understar.py`

 * *Files identical despite different names*

### Comparing `understar-2.4/understar.egg-info/PKG-INFO` & `understar-2.41/understar.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: understar
-Version: 2.4
+Version: 2.41
 Summary: A discord bot framewrok
 Home-page: https://github.com/GalTechDev/UnderStar-OS
 Download-URL: https://github.com/GalTechDev/UnderStar-OS/tarball/master
 Author: GalTech
 Author-email: poussigalitv@gmail.com
 License: MIT
 Keywords: discord,bot,discord.py,understar,os,framework
```

### Comparing `understar-2.4/understar.egg-info/SOURCES.txt` & `understar-2.41/understar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

