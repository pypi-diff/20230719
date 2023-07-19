# Comparing `tmp/understar-2.32.tar.gz` & `tmp/understar-2.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "understar-2.32.tar", last modified: Wed Jul 19 04:53:08 2023, max compression
+gzip compressed data, was "understar-2.33.tar", last modified: Wed Jul 19 05:20:21 2023, max compression
```

## Comparing `understar-2.32.tar` & `understar-2.33.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-19 04:53:08.392839 understar-2.32/
--rw-r--r--   0 maxence    (501) staff       (20)     1188 2023-05-26 01:06:57.000000 understar-2.32/LICENSE.md
--rw-r--r--   0 maxence    (501) staff       (20)      590 2023-07-19 04:53:08.392709 understar-2.32/PKG-INFO
--rw-r--r--   0 maxence    (501) staff       (20)       45 2023-05-26 01:06:57.000000 understar-2.32/README.md
--rw-r--r--   0 maxence    (501) staff       (20)       38 2023-07-19 04:53:08.392922 understar-2.32/setup.cfg
--rw-r--r--   0 maxence    (501) staff       (20)     1293 2023-07-19 02:00:27.000000 understar-2.32/setup.py
-drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-19 04:53:08.386520 understar-2.32/understar/
--rw-r--r--   0 maxence    (501) staff       (20)       25 2023-07-19 04:14:38.000000 understar-2.32/understar/__init__.py
-drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-19 04:53:08.388134 understar-2.32/understar/system/
--rw-r--r--   0 maxence    (501) staff       (20)       22 2023-07-16 04:49:43.000000 understar-2.32/understar/system/__init__.py
-drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-19 04:53:08.388445 understar-2.32/understar/system/app/
--rw-r--r--   0 maxence    (501) staff       (20)       89 2023-07-16 04:47:12.000000 understar-2.32/understar/system/app/__init__.py
-drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-19 04:53:08.388716 understar-2.32/understar/system/app/config/
--rw-r--r--   0 maxence    (501) staff       (20)    20066 2023-07-19 04:34:41.000000 understar-2.32/understar/system/app/config/__init__.py
-drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-19 04:53:08.389673 understar-2.32/understar/system/app/config/apt/
--rw-r--r--   0 maxence    (501) staff       (20)       32 2023-07-12 03:26:34.000000 understar-2.32/understar/system/app/config/apt/__init__.py
--rw-r--r--   0 maxence    (501) staff       (20)     3351 2023-07-19 04:34:43.000000 understar-2.32/understar/system/app/config/apt/install.py
--rw-r--r--   0 maxence    (501) staff       (20)     1329 2023-07-19 04:34:44.000000 understar-2.32/understar/system/app/config/apt/uninstall.py
-drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-19 04:53:08.389960 understar-2.32/understar/system/app/maintenance/
--rw-r--r--   0 maxence    (501) staff       (20)      902 2023-07-19 04:34:46.000000 understar-2.32/understar/system/app/maintenance/__init__.py
-drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-19 04:53:08.392285 understar-2.32/understar/system/lib/
--rw-r--r--   0 maxence    (501) staff       (20)      149 2023-07-12 03:30:52.000000 understar-2.32/understar/system/lib/__init__.py
--rw-r--r--   0 maxence    (501) staff       (20)     5517 2023-07-19 02:04:00.000000 understar-2.32/understar/system/lib/app.py
--rw-r--r--   0 maxence    (501) staff       (20)     1015 2023-06-23 09:10:23.000000 understar-2.32/understar/system/lib/com.py
--rw-r--r--   0 maxence    (501) staff       (20)    11757 2023-06-19 00:59:20.000000 understar-2.32/understar/system/lib/event.py
--rw-r--r--   0 maxence    (501) staff       (20)     3784 2023-06-19 05:27:26.000000 understar-2.32/understar/system/lib/save.py
--rw-r--r--   0 maxence    (501) staff       (20)     2716 2023-07-19 04:01:29.000000 understar-2.32/understar/system/lib/store.py
--rw-r--r--   0 maxence    (501) staff       (20)      174 2023-06-23 09:10:04.000000 understar-2.32/understar/system/lib/types.py
--rw-r--r--   0 maxence    (501) staff       (20)     5138 2023-07-19 00:40:50.000000 understar-2.32/understar/system/lib/utils.py
--rw-r--r--   0 maxence    (501) staff       (20)    31108 2023-07-19 04:20:00.000000 understar-2.32/understar/understar.py
-drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-19 04:53:08.387913 understar-2.32/understar.egg-info/
--rw-r--r--   0 maxence    (501) staff       (20)      590 2023-07-19 04:53:08.000000 understar-2.32/understar.egg-info/PKG-INFO
--rw-r--r--   0 maxence    (501) staff       (20)      755 2023-07-19 04:53:08.000000 understar-2.32/understar.egg-info/SOURCES.txt
--rw-r--r--   0 maxence    (501) staff       (20)        1 2023-07-19 04:53:08.000000 understar-2.32/understar.egg-info/dependency_links.txt
--rw-r--r--   0 maxence    (501) staff       (20)       49 2023-07-19 04:53:08.000000 understar-2.32/understar.egg-info/requires.txt
--rw-r--r--   0 maxence    (501) staff       (20)       10 2023-07-19 04:53:08.000000 understar-2.32/understar.egg-info/top_level.txt
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-19 05:20:21.871348 understar-2.33/
+-rw-r--r--   0 maxence    (501) staff       (20)     1188 2023-05-26 01:06:57.000000 understar-2.33/LICENSE.md
+-rw-r--r--   0 maxence    (501) staff       (20)      590 2023-07-19 05:20:21.871229 understar-2.33/PKG-INFO
+-rw-r--r--   0 maxence    (501) staff       (20)       45 2023-05-26 01:06:57.000000 understar-2.33/README.md
+-rw-r--r--   0 maxence    (501) staff       (20)       38 2023-07-19 05:20:21.871395 understar-2.33/setup.cfg
+-rw-r--r--   0 maxence    (501) staff       (20)     1747 2023-07-19 05:14:51.000000 understar-2.33/setup.py
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-19 05:20:21.862328 understar-2.33/understar/
+-rw-r--r--   0 maxence    (501) staff       (20)       25 2023-07-19 04:14:38.000000 understar-2.33/understar/__init__.py
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-19 05:20:21.863545 understar-2.33/understar/system/
+-rw-r--r--   0 maxence    (501) staff       (20)       22 2023-07-16 04:49:43.000000 understar-2.33/understar/system/__init__.py
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-19 05:20:21.863921 understar-2.33/understar/system/app/
+-rw-r--r--   0 maxence    (501) staff       (20)       89 2023-07-16 04:47:12.000000 understar-2.33/understar/system/app/__init__.py
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-19 05:20:21.864156 understar-2.33/understar/system/app/config/
+-rw-r--r--   0 maxence    (501) staff       (20)    20066 2023-07-19 04:34:41.000000 understar-2.33/understar/system/app/config/__init__.py
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-19 05:20:21.865099 understar-2.33/understar/system/app/config/apt/
+-rw-r--r--   0 maxence    (501) staff       (20)       32 2023-07-12 03:26:34.000000 understar-2.33/understar/system/app/config/apt/__init__.py
+-rw-r--r--   0 maxence    (501) staff       (20)     3351 2023-07-19 04:34:43.000000 understar-2.33/understar/system/app/config/apt/install.py
+-rw-r--r--   0 maxence    (501) staff       (20)     1329 2023-07-19 04:34:44.000000 understar-2.33/understar/system/app/config/apt/uninstall.py
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-19 05:20:21.865352 understar-2.33/understar/system/app/maintenance/
+-rw-r--r--   0 maxence    (501) staff       (20)      902 2023-07-19 04:34:46.000000 understar-2.33/understar/system/app/maintenance/__init__.py
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-19 05:20:21.870847 understar-2.33/understar/system/lib/
+-rw-r--r--   0 maxence    (501) staff       (20)      149 2023-07-12 03:30:52.000000 understar-2.33/understar/system/lib/__init__.py
+-rw-r--r--   0 maxence    (501) staff       (20)     5517 2023-07-19 02:04:00.000000 understar-2.33/understar/system/lib/app.py
+-rw-r--r--   0 maxence    (501) staff       (20)     1015 2023-06-23 09:10:23.000000 understar-2.33/understar/system/lib/com.py
+-rw-r--r--   0 maxence    (501) staff       (20)    11757 2023-06-19 00:59:20.000000 understar-2.33/understar/system/lib/event.py
+-rw-r--r--   0 maxence    (501) staff       (20)     3784 2023-06-19 05:27:26.000000 understar-2.33/understar/system/lib/save.py
+-rw-r--r--   0 maxence    (501) staff       (20)     2716 2023-07-19 04:01:29.000000 understar-2.33/understar/system/lib/store.py
+-rw-r--r--   0 maxence    (501) staff       (20)      174 2023-06-23 09:10:04.000000 understar-2.33/understar/system/lib/types.py
+-rw-r--r--   0 maxence    (501) staff       (20)     5127 2023-07-19 05:03:32.000000 understar-2.33/understar/system/lib/utils.py
+-rw-r--r--   0 maxence    (501) staff       (20)    31108 2023-07-19 04:20:00.000000 understar-2.33/understar/understar.py
+drwxr-xr-x   0 maxence    (501) staff       (20)        0 2023-07-19 05:20:21.863255 understar-2.33/understar.egg-info/
+-rw-r--r--   0 maxence    (501) staff       (20)      590 2023-07-19 05:20:21.000000 understar-2.33/understar.egg-info/PKG-INFO
+-rw-r--r--   0 maxence    (501) staff       (20)      755 2023-07-19 05:20:21.000000 understar-2.33/understar.egg-info/SOURCES.txt
+-rw-r--r--   0 maxence    (501) staff       (20)        1 2023-07-19 05:20:21.000000 understar-2.33/understar.egg-info/dependency_links.txt
+-rw-r--r--   0 maxence    (501) staff       (20)       49 2023-07-19 05:20:21.000000 understar-2.33/understar.egg-info/requires.txt
+-rw-r--r--   0 maxence    (501) staff       (20)       10 2023-07-19 05:20:21.000000 understar-2.33/understar.egg-info/top_level.txt
```

### Comparing `understar-2.32/LICENSE.md` & `understar-2.33/LICENSE.md`

 * *Files identical despite different names*

### Comparing `understar-2.32/PKG-INFO` & `understar-2.33/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: understar
-Version: 2.32
+Version: 2.33
 Summary: A discord bot framewrok
 Home-page: https://github.com/GalTechDev/UnderStar-OS
 Download-URL: https://github.com/GalTechDev/UnderStar-OS/tarball/master
 Author: GalTech
 Author-email: poussigalitv@gmail.com
 License: MIT
 Keywords: discord,bot,discord.py,understar,os,framework
```

### Comparing `understar-2.32/setup.py` & `understar-2.33/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,62 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as stream:
     long_description = stream.read()
     
-with open(".version", "r") as stream:
+with open("understar/.version", "r") as stream:
     ver = stream.read()
 
 # long_description = "An universal wrapper (and useful tool) to make event / commands in python"
 
-setup(
-    name='understar',
-    version=f"{ver}",
-    url='https://github.com/GalTechDev/UnderStar-OS',
-    download_url='https://github.com/GalTechDev/UnderStar-OS/tarball/master',
-    license='MIT',
-    author='GalTech',
-    author_email='poussigalitv@gmail.com',
-    description='A discord bot framewrok',
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-    keywords=[
+name='understar'
+version=f"{ver}"
+url='https://github.com/GalTechDev/UnderStar-OS'
+download_url='https://github.com/GalTechDev/UnderStar-OS/tarball/master'
+license='MIT'
+author='GalTech'
+author_email='poussigalitv@gmail.com'
+description='A discord bot framewrok'
+long_description=long_description
+long_description_content_type='text/markdown'
+keywords=[
         "discord",
         "bot",
         "discord.py",
         "understar",
         "os",
         "framework"
-    ],
-    install_requires=[
+]
+install_requires=[
         "easy-events>=2.9.0",
         "discord.py>=2.1",
         "requests_html",
-    ],
-    setup_requires=[
+]
+setup_requires=[
         'wheel'
-    ],
-    classifiers=[
+]
+classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
-    ],
-    packages=find_packages()
-    # packages=["sdist", "bdist_wheel"]
-    # python_requires='>=3.10',
-)
+]
+
+if __name__ == "__main__":
+    setup(
+        name=name,
+        version=version,
+        url=url,
+        download_url=download_url,
+        license=license,
+        author=author,
+        author_email=author_email,
+        description=description,
+        long_description=long_description,
+        long_description_content_type=long_description_content_type,
+        keywords=keywords,
+        install_requires=install_requires,
+        setup_requires=setup_requires,
+        classifiers=classifiers,
+        packages=find_packages()
+        # packages=["sdist", "bdist_wheel"]
+        # python_requires='>=3.10',
+    )
```

### Comparing `understar-2.32/understar/system/app/config/__init__.py` & `understar-2.33/understar/system/app/config/__init__.py`

 * *Files identical despite different names*

### Comparing `understar-2.32/understar/system/app/config/apt/install.py` & `understar-2.33/understar/system/app/config/apt/install.py`

 * *Files identical despite different names*

### Comparing `understar-2.32/understar/system/app/config/apt/uninstall.py` & `understar-2.33/understar/system/app/config/apt/uninstall.py`

 * *Files identical despite different names*

### Comparing `understar-2.32/understar/system/app/maintenance/__init__.py` & `understar-2.33/understar/system/app/maintenance/__init__.py`

 * *Files identical despite different names*

### Comparing `understar-2.32/understar/system/lib/app.py` & `understar-2.33/understar/system/lib/app.py`

 * *Files identical despite different names*

### Comparing `understar-2.32/understar/system/lib/com.py` & `understar-2.33/understar/system/lib/com.py`

 * *Files identical despite different names*

### Comparing `understar-2.32/understar/system/lib/event.py` & `understar-2.33/understar/system/lib/event.py`

 * *Files identical despite different names*

### Comparing `understar-2.32/understar/system/lib/save.py` & `understar-2.33/understar/system/lib/save.py`

 * *Files identical despite different names*

### Comparing `understar-2.32/understar/system/lib/store.py` & `understar-2.33/understar/system/lib/store.py`

 * *Files identical despite different names*

### Comparing `understar-2.32/understar/system/lib/utils.py` & `understar-2.33/understar/system/lib/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     try:
         await interaction.response.send_message()
     except Exception as error:
         pass
 
 chemin_fichier = pkg_resources.resource_filename(__name__, '.version')
 
-with open(chemin_fichier.removesuffix("understar2/system/lib/.version")+".version", 'r') as f:
+with open(chemin_fichier.removesuffix("system/lib/.version")+".version", 'r') as f:
     BOT_VERSION = f.read()
 
 def import_module(folder: str, log=False, catch_error=True):
     # Parcours des apps dans le répertoire du package
     if log:
         print(f" * Import Module Start :")
     modules = {}
```

### Comparing `understar-2.32/understar/understar.py` & `understar-2.33/understar/understar.py`

 * *Files identical despite different names*

### Comparing `understar-2.32/understar.egg-info/PKG-INFO` & `understar-2.33/understar.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: understar
-Version: 2.32
+Version: 2.33
 Summary: A discord bot framewrok
 Home-page: https://github.com/GalTechDev/UnderStar-OS
 Download-URL: https://github.com/GalTechDev/UnderStar-OS/tarball/master
 Author: GalTech
 Author-email: poussigalitv@gmail.com
 License: MIT
 Keywords: discord,bot,discord.py,understar,os,framework
```

### Comparing `understar-2.32/understar.egg-info/SOURCES.txt` & `understar-2.33/understar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

