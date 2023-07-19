# Comparing `tmp/unigui-1.8.4.tar.gz` & `tmp/unigui-1.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/unigui-1.8.4.tar", last modified: Mon Jul 17 00:03:32 2023, max compression
+gzip compressed data, was "dist/unigui-1.8.5.tar", last modified: Wed Jul 19 03:26:32 2023, max compression
```

## Comparing `unigui-1.8.4.tar` & `unigui-1.8.5.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-17 00:03:32.000000 unigui-1.8.4/
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-17 00:03:31.000000 unigui-1.8.4/unigui/
--rw-rw-r--   0 george    (1000) george    (1000)     8633 2023-07-16 20:25:20.000000 unigui-1.8.4/unigui/guielements.py
--rw-rw-r--   0 george    (1000) george    (1000)     3145 2023-07-16 20:04:28.000000 unigui-1.8.4/unigui/server.py
--rw-rw-r--   0 george    (1000) george    (1000)      100 2023-07-14 22:20:13.000000 unigui-1.8.4/unigui/__init__.py
--rw-rw-r--   0 george    (1000) george    (1000)     2525 2023-07-16 23:57:38.000000 unigui-1.8.4/unigui/autotest.py
--rw-r--r--   0 george    (1000) george    (1000)     2916 2023-07-16 11:20:18.000000 unigui-1.8.4/unigui/utils.py
--rw-rw-r--   0 george    (1000) george    (1000)     4564 2023-07-14 22:55:02.000000 unigui-1.8.4/unigui/reloader.py
--rw-rw-r--   0 george    (1000) george    (1000)     9852 2023-07-16 20:04:15.000000 unigui-1.8.4/unigui/users.py
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-17 00:03:31.000000 unigui-1.8.4/unigui/web/
--rw-rw-r--   0 george    (1000) george    (1000)    64483 2023-07-17 00:00:44.000000 unigui-1.8.4/unigui/web/favicon.ico
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-17 00:03:31.000000 unigui-1.8.4/unigui/web/css/
--rw-rw-r--   0 george    (1000) george    (1000)   220628 2023-07-17 00:00:44.000000 unigui-1.8.4/unigui/web/css/vendor.191faa77.css
--rw-rw-r--   0 george    (1000) george    (1000)        0 2023-07-17 00:00:44.000000 unigui-1.8.4/unigui/web/css/app.31d6cfe0.css
--rw-rw-r--   0 george    (1000) george    (1000)     3267 2023-07-17 00:00:44.000000 unigui-1.8.4/unigui/web/css/786.d75b8133.css
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-17 00:03:32.000000 unigui-1.8.4/unigui/web/icons/
--rw-rw-r--   0 george    (1000) george    (1000)     9643 2023-07-17 00:00:44.000000 unigui-1.8.4/unigui/web/icons/favicon-96x96.png
--rw-rw-r--   0 george    (1000) george    (1000)      859 2023-07-17 00:00:44.000000 unigui-1.8.4/unigui/web/icons/favicon-16x16.png
--rw-rw-r--   0 george    (1000) george    (1000)     2039 2023-07-17 00:00:44.000000 unigui-1.8.4/unigui/web/icons/favicon-32x32.png
--rw-rw-r--   0 george    (1000) george    (1000)    12324 2023-07-17 00:00:44.000000 unigui-1.8.4/unigui/web/icons/favicon-128x128.png
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-17 00:03:32.000000 unigui-1.8.4/unigui/web/fonts/
--rw-rw-r--   0 george    (1000) george    (1000)   128616 2023-07-17 00:00:44.000000 unigui-1.8.4/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2
--rw-rw-r--   0 george    (1000) george    (1000)   164912 2023-07-17 00:00:44.000000 unigui-1.8.4/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20344 2023-07-17 00:00:44.000000 unigui-1.8.4/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20416 2023-07-17 00:00:44.000000 unigui-1.8.4/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20408 2023-07-17 00:00:44.000000 unigui-1.8.4/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20424 2023-07-17 00:00:44.000000 unigui-1.8.4/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20544 2023-07-17 00:00:44.000000 unigui-1.8.4/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20436 2023-07-17 00:00:44.000000 unigui-1.8.4/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-17 00:03:32.000000 unigui-1.8.4/unigui/web/js/
--rw-rw-r--   0 george    (1000) george    (1000)    44918 2023-07-17 00:00:44.000000 unigui-1.8.4/unigui/web/js/786.93a21e48.js
--rw-rw-r--   0 george    (1000) george    (1000)     6560 2023-07-17 00:00:44.000000 unigui-1.8.4/unigui/web/js/430.591e9a73.js
--rw-rw-r--   0 george    (1000) george    (1000)  1434072 2023-07-17 00:00:44.000000 unigui-1.8.4/unigui/web/js/vendor.3076c5e7.js
--rw-rw-r--   0 george    (1000) george    (1000)     5868 2023-07-17 00:00:44.000000 unigui-1.8.4/unigui/web/js/app.4491f085.js
--rw-rw-r--   0 george    (1000) george    (1000)      763 2023-07-17 00:00:44.000000 unigui-1.8.4/unigui/web/js/193.283445be.js
--rw-rw-r--   0 george    (1000) george    (1000)      907 2023-07-17 00:00:44.000000 unigui-1.8.4/unigui/web/index.html
--rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.8.4/LICENSE
--rw-rw-r--   0 george    (1000) george    (1000)      612 2023-07-17 00:02:37.000000 unigui-1.8.4/setup.py
--rw-rw-r--   0 george    (1000) george    (1000)    19002 2023-07-17 00:03:32.000000 unigui-1.8.4/PKG-INFO
--rw-rw-r--   0 george    (1000) george    (1000)       38 2023-07-17 00:03:32.000000 unigui-1.8.4/setup.cfg
--rw-rw-r--   0 george    (1000) george    (1000)    18697 2023-07-16 06:09:11.000000 unigui-1.8.4/README.md
--rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.8.4/MANIFEST.in
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-17 00:03:31.000000 unigui-1.8.4/unigui.egg-info/
--rw-rw-r--   0 george    (1000) george    (1000)       39 2023-07-17 00:03:31.000000 unigui-1.8.4/unigui.egg-info/requires.txt
--rw-r--r--   0 george    (1000) george    (1000)        1 2023-07-17 00:03:31.000000 unigui-1.8.4/unigui.egg-info/dependency_links.txt
--rw-r--r--   0 george    (1000) george    (1000)    19002 2023-07-17 00:03:31.000000 unigui-1.8.4/unigui.egg-info/PKG-INFO
--rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.8.4/unigui.egg-info/not-zip-safe
--rw-r--r--   0 george    (1000) george    (1000)     1241 2023-07-17 00:03:31.000000 unigui-1.8.4/unigui.egg-info/SOURCES.txt
--rw-r--r--   0 george    (1000) george    (1000)        7 2023-07-17 00:03:31.000000 unigui-1.8.4/unigui.egg-info/top_level.txt
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-19 03:26:32.000000 unigui-1.8.5/
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-19 03:26:32.000000 unigui-1.8.5/unigui/
+-rw-rw-r--   0 george    (1000) george    (1000)     8519 2023-07-19 00:31:05.000000 unigui-1.8.5/unigui/guielements.py
+-rw-rw-r--   0 george    (1000) george    (1000)     2744 2023-07-18 23:50:34.000000 unigui-1.8.5/unigui/server.py
+-rw-rw-r--   0 george    (1000) george    (1000)      100 2023-07-14 22:20:13.000000 unigui-1.8.5/unigui/__init__.py
+-rw-rw-r--   0 george    (1000) george    (1000)     3321 2023-07-18 19:22:00.000000 unigui-1.8.5/unigui/autotest.py
+-rw-r--r--   0 george    (1000) george    (1000)     2199 2023-07-18 23:05:47.000000 unigui-1.8.5/unigui/utils.py
+-rw-rw-r--   0 george    (1000) george    (1000)     4544 2023-07-18 18:55:27.000000 unigui-1.8.5/unigui/reloader.py
+-rw-rw-r--   0 george    (1000) george    (1000)     8612 2023-07-18 22:22:05.000000 unigui-1.8.5/unigui/users.py
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-19 03:26:32.000000 unigui-1.8.5/unigui/web/
+-rw-rw-r--   0 george    (1000) george    (1000)    64483 2023-07-19 03:24:30.000000 unigui-1.8.5/unigui/web/favicon.ico
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-19 03:26:32.000000 unigui-1.8.5/unigui/web/css/
+-rw-rw-r--   0 george    (1000) george    (1000)   220628 2023-07-19 03:24:30.000000 unigui-1.8.5/unigui/web/css/vendor.191faa77.css
+-rw-rw-r--   0 george    (1000) george    (1000)        0 2023-07-19 03:24:30.000000 unigui-1.8.5/unigui/web/css/app.31d6cfe0.css
+-rw-rw-r--   0 george    (1000) george    (1000)     3267 2023-07-19 03:24:30.000000 unigui-1.8.5/unigui/web/css/164.06cedad1.css
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-19 03:26:32.000000 unigui-1.8.5/unigui/web/icons/
+-rw-rw-r--   0 george    (1000) george    (1000)     9643 2023-07-19 03:24:30.000000 unigui-1.8.5/unigui/web/icons/favicon-96x96.png
+-rw-rw-r--   0 george    (1000) george    (1000)      859 2023-07-19 03:24:30.000000 unigui-1.8.5/unigui/web/icons/favicon-16x16.png
+-rw-rw-r--   0 george    (1000) george    (1000)     2039 2023-07-19 03:24:30.000000 unigui-1.8.5/unigui/web/icons/favicon-32x32.png
+-rw-rw-r--   0 george    (1000) george    (1000)    12324 2023-07-19 03:24:30.000000 unigui-1.8.5/unigui/web/icons/favicon-128x128.png
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-19 03:26:32.000000 unigui-1.8.5/unigui/web/fonts/
+-rw-rw-r--   0 george    (1000) george    (1000)   128616 2023-07-19 03:24:30.000000 unigui-1.8.5/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2
+-rw-rw-r--   0 george    (1000) george    (1000)   164912 2023-07-19 03:24:30.000000 unigui-1.8.5/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20344 2023-07-19 03:24:30.000000 unigui-1.8.5/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20416 2023-07-19 03:24:30.000000 unigui-1.8.5/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20408 2023-07-19 03:24:30.000000 unigui-1.8.5/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20424 2023-07-19 03:24:30.000000 unigui-1.8.5/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20544 2023-07-19 03:24:30.000000 unigui-1.8.5/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20436 2023-07-19 03:24:30.000000 unigui-1.8.5/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-19 03:26:32.000000 unigui-1.8.5/unigui/web/js/
+-rw-rw-r--   0 george    (1000) george    (1000)    45370 2023-07-19 03:24:30.000000 unigui-1.8.5/unigui/web/js/164.2b869daf.js
+-rw-rw-r--   0 george    (1000) george    (1000)     6560 2023-07-19 03:24:30.000000 unigui-1.8.5/unigui/web/js/430.591e9a73.js
+-rw-rw-r--   0 george    (1000) george    (1000)  1434072 2023-07-19 03:24:30.000000 unigui-1.8.5/unigui/web/js/vendor.3076c5e7.js
+-rw-rw-r--   0 george    (1000) george    (1000)     5868 2023-07-19 03:24:30.000000 unigui-1.8.5/unigui/web/js/app.e17901f8.js
+-rw-rw-r--   0 george    (1000) george    (1000)      763 2023-07-19 03:24:30.000000 unigui-1.8.5/unigui/web/js/193.283445be.js
+-rw-rw-r--   0 george    (1000) george    (1000)      907 2023-07-19 03:24:30.000000 unigui-1.8.5/unigui/web/index.html
+-rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.8.5/LICENSE
+-rw-rw-r--   0 george    (1000) george    (1000)      612 2023-07-19 03:25:49.000000 unigui-1.8.5/setup.py
+-rw-rw-r--   0 george    (1000) george    (1000)    19239 2023-07-19 03:26:32.000000 unigui-1.8.5/PKG-INFO
+-rw-rw-r--   0 george    (1000) george    (1000)       38 2023-07-19 03:26:32.000000 unigui-1.8.5/setup.cfg
+-rw-rw-r--   0 george    (1000) george    (1000)    18934 2023-07-17 14:52:22.000000 unigui-1.8.5/README.md
+-rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.8.5/MANIFEST.in
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-07-19 03:26:32.000000 unigui-1.8.5/unigui.egg-info/
+-rw-rw-r--   0 george    (1000) george    (1000)       39 2023-07-19 03:26:32.000000 unigui-1.8.5/unigui.egg-info/requires.txt
+-rw-r--r--   0 george    (1000) george    (1000)        1 2023-07-19 03:26:32.000000 unigui-1.8.5/unigui.egg-info/dependency_links.txt
+-rw-r--r--   0 george    (1000) george    (1000)    19239 2023-07-19 03:26:32.000000 unigui-1.8.5/unigui.egg-info/PKG-INFO
+-rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.8.5/unigui.egg-info/not-zip-safe
+-rw-r--r--   0 george    (1000) george    (1000)     1241 2023-07-19 03:26:32.000000 unigui-1.8.5/unigui.egg-info/SOURCES.txt
+-rw-r--r--   0 george    (1000) george    (1000)        7 2023-07-19 03:26:32.000000 unigui-1.8.5/unigui.egg-info/top_level.txt
```

### Comparing `unigui-1.8.4/unigui/guielements.py` & `unigui-1.8.5/unigui/guielements.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,16 @@
     return complete
 
 class Edit(Gui):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)        
         if 'type' not in kwargs:
             self.type =  'autoedit' if 'complete' in kwargs else 'edit'
-        self.check('value')
+        if not hasattr(self,'value'):
+            self.value = '' if self.type != 'number' else 0
 
 class Text(Gui):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.value = ''
         self.edit = False
 
@@ -60,31 +61,27 @@
     def __init__(self, *args, **kwargs):
         self.name = args[0]
         if len(args) > 1:
             self.changed = args[1]        
         for key in kwargs.keys():            
             self.add(key, kwargs[key])
 
-def CameraButton(name, *args,**kwargs):
-    kwargs['type'] = 'camera'
-    return Button(name, *args, **kwargs)
-
-def UploadButton(name, handler,**kwargs):
-    if 'type' not in kwargs:
-        kwargs['type'] = 'gallery'
+def CameraButton(name, *args):    
+    return Button(name, *args, type = 'camera')
+        
+def UploadImageButton(name, handler,**kwargs):    
+    kwargs['type'] = 'image_uploader'
     if 'width' not in kwargs:
         kwargs['width'] = 250.0              
     if 'height' not in kwargs:
-        kwargs['height'] = 300.0                  
+        kwargs['height'] = 300.0         
     return Button(name, handler, **kwargs)
 
-def UploadImageButton(name, handler,**kwargs):
-    kwargs['type'] = 'gimages'
-    return UploadButton(name, handler, **kwargs)    
-        
+UploadButton = UploadImageButton
+
 class Image(Gui):
     '''has to contain file parameter as name'''
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.type='image'
         if not hasattr(self,'width'):
             self.width = 500.0              
@@ -192,16 +189,15 @@
         if not hasattr(self,'value'):
             self.value = None
 
         if getattr(self,'edit', True):
             edit_setting = hasattr(self,'modify') or hasattr(self,'delete') or hasattr(self,'append')
             if not edit_setting:                             
                 self.delete = delete_table_row             
-                self.append = append_table_row 
-            if not hasattr(self,'modify'): 
+                self.append = append_table_row             
                 self.modify = accept_cell_value             
         
     def selected_list(self):                            
         return [self.value] if self.value != None else [] if type(self.value) == int else self.value   
 
     def clean(self):
         self.rows = []
```

### Comparing `unigui-1.8.4/unigui/server.py` & `unigui-1.8.5/unigui/server.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,45 +1,41 @@
 from aiohttp import web, WSMsgType
 from .users import *
-from config import port, pretty_print, socket_ip, upload_dir
 from pathlib import Path
 from .reloader import empty_app 
 from .autotest import recorder
+from config import port, pretty_print, upload_dir
+from .utils import app_dir
+import traceback
 
 async def post_handler(request):
     reader = await request.multipart()
     field = await reader.next()   
-    filename = upload_path(field.filename)  
-    # You cannot rely on Content-Length if transfer is chunked.
+    filename = upload_path(field.filename)      
     size = 0
     with open(filename, 'wb') as f:
         while True:
-            chunk = await field.read_chunk()  # 8192 bytes by default.
+            chunk = await field.read_chunk()  
             if not chunk:
                 break
             size += len(chunk)
             f.write(chunk)
 
-    return web.Response(text=f'{filename} sized of {size} successfully stored')
+    return web.Response(text=filename)
 
 def jsonString(obj):
     return toJson(obj, 2 if pretty_print else 0, pretty_print)
 
 async def static_serve(request):    
-    file_path = request.path
-    if upload_dir not in  request.path:
-        file_path = f"{webpath}{file_path}"  # rebase into static dir
-    file_path  = Path(file_path)
-    
+    file_path = request.path    
+    file_path  = Path(f"{webpath}{file_path}" )
     if request.path == '/':
-        file_path /= 'index.html'
-        
-    answer = web.HTTPNotFound() if not file_path.exists() else (web.FileResponse(file_path)     
-         if request.path != User.fix_file else web.Response(text = User.configured_main)) 
-
+        file_path /= 'index.html' 
+    
+    answer = web.HTTPNotFound() if not file_path.exists() else web.FileResponse(file_path)          
     return answer
 
 async def websocket_handler(request):
     ws = web.WebSocketResponse()
     await ws.prepare(request)
     user = User.UserType()
 
@@ -63,32 +59,28 @@
                     if result:            
                         result = jsonString(user.prepare_result(result))    
                         await ws.send_str(result)
                     recorder(msg.data, result)
 
             elif msg.type == WSMsgType.ERROR:
                 print('ws connection closed with exception %s' % ws.exception())
-    except:
-        type, value, traceback = sys.exc_info()
-        user.log(f'{type}: {value} \n{traceback.format_exc()}\n')
+    except:        
+        user.log(traceback.format_exc())
     
     return ws       
 
-def start(appname, user_type = User, http_handlers = []):
-    
-    set_utils(appname, port, upload_dir, socket_ip)    
-    
-    if upload_dir and not os.path.exists(upload_dir):
-        os.makedirs(upload_dir)
+def start(appname = '', user_type = User, http_handlers = []):
+    if appname:
+        config.appname = appname
 
     User.UserType = user_type    
-    User.create_fixed_js()      
     http_handlers.insert(0, web.get('/ws', websocket_handler))
         
-    for h in [web.get('/{tail:.*}', static_serve), web.post('/', post_handler)]:
+    for h in [web.static(f'/{config.upload_dir}', f"/{app_dir}/{upload_dir}"), 
+        web.get('/{tail:.*}', static_serve), web.post('/', post_handler)]:
         http_handlers.append(h)
 
     print(f'Start {appname} server on {port} port..')    
     app = web.Application()
     app.add_routes(http_handlers)    
     web.run_app(app,  port=port)
```

### Comparing `unigui-1.8.4/unigui/autotest.py` & `unigui-1.8.5/unigui/autotest.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,58 @@
-import config, os
+import config, os, logging
+from .utils import *
 from .guielements import * 
 from .users import User
-from .utils import *
 
+#setting default config variables
 testdir = 'autotest'
-autotest = hasattr(config, testdir)
+if not hasattr(config, testdir):
+    config.autotest = False
+if not hasattr(config, 'port'):
+    config.port = 8000
+if not hasattr(config, 'pretty_print'):
+    config.pretty_print = False
+if not hasattr(config, 'upload_dir'):
+    config.upload_dir = 'web'
+if not hasattr(config, 'logfile'):
+    config.logfile = None
+if not hasattr(config, 'hot_reload'):
+    config.hot_reload = False
+if not hasattr(config, 'appname'):
+    config.appname = 'Unigui'
+
+if not os.path.exists(config.upload_dir):
+    os.makedirs(config.upload_dir)
+
+#start logging 
+format = "%(asctime)s - %(levelname)s - %(message)s"
+handlers = [logging.FileHandler(config.logfile), logging.StreamHandler()] if config.logfile else []
+logging.basicConfig(level = logging.WARNING, format = format, handlers = handlers)
+
 record_file = None
 ignored_1message = False
 record_buffer = []
 
 def recorder(msg, response):
     if record_file:
         global ignored_1message, record_buffer
         if ignored_1message:            
             record_buffer.append(f'{msg},\n{"null" if response is None else response}\n')
         else:
             ignored_1message = True
 
-if autotest:
+if config.autotest:
     if not os.path.exists(testdir):
         os.makedirs(testdir)
 
     def test(file):
         pass
 
     def alltest():    
-        files = config[testdir]
+        files = config.autotest
         for file in os.listdir(testdir):
             if  files == '*' or file in files:
                 test(file)
 
     test_name = Edit('Name test file', '')
     rewrite = Switch('Overwrite existing', False, type = 'check')
```

### Comparing `unigui-1.8.4/unigui/utils.py` & `unigui-1.8.5/unigui/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,71 +1,47 @@
 import os 
 import jsonpickle
 import json
 
-resource_port = None
-appname = 'Unigui'
-app_user_dir = os.getcwd()
-upload_dir = 'upload'
-socket_ip = ''
-socket_port = 1234
 blocks_dir = 'blocks'        
 screens_dir =  'screens'        
 UpdateScreen = True
 
 libpath = os.path.dirname(os.path.realpath(__file__))
 webpath = libpath + '/web' 
+app_dir = os.getcwd()
 
 try:
     import config
 except:
     with open('config.py', 'w') as f:        
         f.write("""port = 8000 
-#for remote server socket_ip is its ip 
-socket_ip  = 'localhost' 
 upload_dir = 'web'
 pretty_print = True
 hot_reload   = True
 logfile  = 'log'
 autotest = '*'
 """)
+        import config
         print("Config with default parameters is created!")
 
 def toJson(obj, indent, pretty_print):
     return json.dumps(json.loads(jsonpickle.encode(obj,unpicklable=False)), 
         indent = indent, sort_keys = pretty_print)
 
-def fn2url(fn):   
+def filename2url(fn):   
     if fn[0] == '/':
-        fn = fn[len(app_user_dir):]   
+        fn = fn[len(app_dir):]   
     return fn.replace(' ','%20')
 
-def url2fn(url):
-    return url[url.find('/') + 1:].replace('%20',' ')
-
-def upload_fn(fn):
-    return f'{upload_dir}/{fn}'     
+def url2filename(url):
+    return url[url.find('/') + 1:].replace('%20',' ')   
 
 def upload_path(fpath):
-    return f'{os.getcwd()}/{upload_dir}/{fpath}'
-    
-def translate_http_path(path):
-    if '?' in path:
-        path = path.split('?')[0]
-    if path.startswith(f'/{upload_dir}/'):             
-        return f'{app_user_dir}{path}'.replace('%20',' ')     
-    return f'{webpath}{path}'.replace('%20',' ') 
-
-def set_utils(appname_,port_,upload_dir_, socket_ip_):
-    global appname, resource_port, upload_dir, socket_ip, socket_port
-    appname = appname_
-    resource_port = port_
-    upload_dir = upload_dir_
-    socket_ip = socket_ip_
-    socket_port = port_    
+    return f'{config.upload_dir}/{fpath}'
 
 def flatten(*arr):
     for a in arr:
         if isinstance(a, list):
             yield from flatten(*a)
         else:
             yield a
```

### Comparing `unigui-1.8.4/unigui/reloader.py` & `unigui-1.8.5/unigui/reloader.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,40 @@
-import config
+from .autotest import config
 
 empty_app = {
     "blocks": [],
     "header": "No screens",
     "icon": None,
     "menu": [["You need to put at least 1 file in the 'screens' folder.",'exclamation']],
     "name": "",
     "order": 0,
     "toolbar": [],
     "type": "screen"
 }
 
-if hasattr(config, 'hot_reload') and config.hot_reload:
+if config.hot_reload:
     import logging, os, traceback
     from watchdog.observers import Observer
     from watchdog.events import PatternMatchingEventHandler
-    from unigui import User
+    from .users import User
     busy = False        
 
     def free():
         global busy
         if request_file:
             reload(request_file)
         else:
             busy = False
 
     def reload(sname):
         user = User.last_user
         if user:
             global busy, request_file
             busy = True
-            request_file = None
-            
+            request_file = None            
             try:
                 module = user.load_module(sname)
             except:
                 busy = False
                 traceback.print_exc()        
                 return
```

### Comparing `unigui-1.8.4/unigui/users.py` & `unigui-1.8.5/unigui/users.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,47 +37,27 @@
             if response.status_code != 200:
                 return None
             file = open(cname, "wb")
             file.write(response.content)
             file.close() 
         return cname
 
-    @staticmethod
-    def create_fixed_js():
-        dir = f"{utils.webpath}/js"
-        b = None        
-        def replace(what, tothat):
-            return b.replace(bytes(what,encoding='utf8'), bytes(str(tothat),encoding='utf8'))  
-        for file in os.listdir(dir):
-            fn = f'{dir}/{file}'
-            if file[0].isdigit() and file.endswith(".js") and os.path.getsize(fn) > 25000:
-                User.fix_file = f'/js/{file}'
-                with open(fn, 'rb') as main:
-                    b = main.read()
-                    if utils.socket_ip != 'localhost':
-                        b = replace('localhost', utils.socket_ip)
-                    if utils.resource_port != 8000:
-                        b = replace('8000',utils.resource_port)                    
-                    User.configured_main = b.decode("utf-8") 
-                    print(f"Configuring for http port {utils.resource_port}, socket ip is {utils.socket_ip}.")
-                    break
-
     def sync_send(self, obj):
         asyncio.run_coroutine_threadsafe(self.send(obj), self.extra_loop)            
 
     def progress(self, str, *updates):
         """open or update progress window if str != null else close it  """             
         return self.sync_send(TextMessage('progress', str, *updates, user = self))
                        
     def load_module(self, file):
         screen_vars = {
             'icon' : None,
             'prepare' : None,            
             'blocks' : [],
-            'header' : utils.appname,                        
+            'header' : config.appname,                        
             'toolbar' : User.toolbar, 
             'order' : 0
         }             
         name = file[0:-3]        
         path = f'{screens_dir}/{file}'                
         spec = importlib.util.spec_from_file_location(name,path)
         module = importlib.util.module_from_spec(spec)        
@@ -252,14 +232,8 @@
     loop.run_forever() 
     
 async_thread = Thread(target=f, args=(loop,))
 async_thread.start()  
 
 User.toolbar = []
 
-#Logging 
-format = "%(asctime)s - %(levelname)s - %(message)s"
-handlers = [logging.FileHandler(config.logfile), logging.StreamHandler()] if hasattr(config,'logfile') else []
-logging.basicConfig(level = logging.WARNING, format = format, handlers = handlers)
-
-
```

### Comparing `unigui-1.8.4/unigui/web/favicon.ico` & `unigui-1.8.5/unigui/web/favicon.ico`

 * *Files identical despite different names*

### Comparing `unigui-1.8.4/unigui/web/css/vendor.191faa77.css` & `unigui-1.8.5/unigui/web/css/vendor.191faa77.css`

 * *Files identical despite different names*

### Comparing `unigui-1.8.4/unigui/web/css/786.d75b8133.css` & `unigui-1.8.5/unigui/web/css/164.06cedad1.css`

 * *Files 9% similar despite different names*

```diff
@@ -1 +1 @@
-thead tr:first-child th{-webkit-backdrop-filter:blur(10px);backdrop-filter:blur(10px);position:sticky;top:0;z-index:1000}:root{--scrollbar-width-height:10px;--scrollbar-track:#eee;--scrollbar-thumb:#cce7ff;--scrollbar-thumb-hover:#2176d2;--scrollbar-track-dark:#eee;--scrollbar-thumb-dark:#cce7ff;--scrollbar-thumb-hover-dark:#2176d2}::-webkit-scrollbar{height:var(--scrollbar-width-height);width:var(--scrollbar-width-height)}::-webkit-scrollbar-track{box-shadow:inset 0 0 4px var(--scrollbar-track-dark)}::-webkit-scrollbar-corner,::-webkit-scrollbar-track{background:var(--scrollbar-track-dark)}::-webkit-scrollbar-thumb{background:var(--scrollbar-thumb-dark);border-radius:5px}::-webkit-scrollbar-thumb:hover{background:var(--scrollbar-thumb-hover-dark)}.my-sticky-header-table{height:310px}.my-sticky-header-table .q-table__bottom,.my-sticky-header-table .q-table__top,.my-sticky-header-table thead tr:first-child th{background-color:#c1f4cd}.my-sticky-header-table thead tr th{position:sticky;z-index:1}.my-sticky-header-table thead tr:first-child th{top:0}.my-sticky-header-table.q-table--loading thead tr:last-child th{top:48px}body[data-v-84c697a8]{display:flex;justify-content:center}.custom-caption[data-v-84c697a8]{padding:5px!important}.web-camera-container[data-v-84c697a8]{align-items:center;border:1px solid #ccc;border-radius:4px;display:flex;flex-direction:column;justify-content:center;margin-bottom:2rem;margin-top:2rem;padding:2rem;width:500px}.web-camera-container .camera-button[data-v-84c697a8]{margin-bottom:2rem}.web-camera-container .camera-box .camera-shutter[data-v-84c697a8]{background-color:#fff;height:337.5px;opacity:0;position:absolute;width:450px}.web-camera-container .camera-box .camera-shutter.flash[data-v-84c697a8]{opacity:1}.web-camera-container .camera-shoot[data-v-84c697a8]{margin:1rem 0}.web-camera-container .camera-shoot button[data-v-84c697a8]{align-items:center;border-radius:100%;display:flex;height:60px;justify-content:center;width:60px}.web-camera-container .camera-shoot button img[data-v-84c697a8]{height:35px;object-fit:cover}.web-camera-container .camera-loading[data-v-84c697a8]{height:100%;margin:3rem 0 0 -1.2rem;min-height:150px;overflow:hidden;position:absolute;width:100%}.web-camera-container .camera-loading ul[data-v-84c697a8]{height:100%;margin:0;position:absolute;width:100%;z-index:999999}.web-camera-container .camera-loading .loader-circle[data-v-84c697a8]{display:block;height:14px;left:100%;margin:0 auto;padding:0;position:absolute;top:50%;transform:translateY(-50%);transform:translateX(-50%);width:100%}.web-camera-container .camera-loading .loader-circle li[data-v-84c697a8]{animation:preload-84c697a8 1s infinite;background:#999;border-radius:100%;display:block;float:left;height:10px;line-height:10px;margin:0 0 0 4px;padding:0;position:relative;top:-50%;width:10px}.web-camera-container .camera-loading .loader-circle li[data-v-84c697a8]:nth-child(2){animation-delay:.2s}.web-camera-container .camera-loading .loader-circle li[data-v-84c697a8]:nth-child(3){animation-delay:.4s}@keyframes preload-84c697a8{0%{opacity:1}50%{opacity:.4}to{opacity:1}}.textarea[data-v-84c697a8]{border:2px solid #ddd;border-radius:10px;font-size:inherit;min-height:100px;outline:none;padding:20px;width:100%}
+thead tr:first-child th{-webkit-backdrop-filter:blur(10px);backdrop-filter:blur(10px);position:sticky;top:0;z-index:1000}:root{--scrollbar-width-height:10px;--scrollbar-track:#eee;--scrollbar-thumb:#cce7ff;--scrollbar-thumb-hover:#2176d2;--scrollbar-track-dark:#eee;--scrollbar-thumb-dark:#cce7ff;--scrollbar-thumb-hover-dark:#2176d2}::-webkit-scrollbar{height:var(--scrollbar-width-height);width:var(--scrollbar-width-height)}::-webkit-scrollbar-track{box-shadow:inset 0 0 4px var(--scrollbar-track-dark)}::-webkit-scrollbar-corner,::-webkit-scrollbar-track{background:var(--scrollbar-track-dark)}::-webkit-scrollbar-thumb{background:var(--scrollbar-thumb-dark);border-radius:5px}::-webkit-scrollbar-thumb:hover{background:var(--scrollbar-thumb-hover-dark)}.my-sticky-header-table{height:310px}.my-sticky-header-table .q-table__bottom,.my-sticky-header-table .q-table__top,.my-sticky-header-table thead tr:first-child th{background-color:#c1f4cd}.my-sticky-header-table thead tr th{position:sticky;z-index:1}.my-sticky-header-table thead tr:first-child th{top:0}.my-sticky-header-table.q-table--loading thead tr:last-child th{top:48px}body[data-v-7eaff898]{display:flex;justify-content:center}.custom-caption[data-v-7eaff898]{padding:5px!important}.web-camera-container[data-v-7eaff898]{align-items:center;border:1px solid #ccc;border-radius:4px;display:flex;flex-direction:column;justify-content:center;margin-bottom:2rem;margin-top:2rem;padding:2rem;width:500px}.web-camera-container .camera-button[data-v-7eaff898]{margin-bottom:2rem}.web-camera-container .camera-box .camera-shutter[data-v-7eaff898]{background-color:#fff;height:337.5px;opacity:0;position:absolute;width:450px}.web-camera-container .camera-box .camera-shutter.flash[data-v-7eaff898]{opacity:1}.web-camera-container .camera-shoot[data-v-7eaff898]{margin:1rem 0}.web-camera-container .camera-shoot button[data-v-7eaff898]{align-items:center;border-radius:100%;display:flex;height:60px;justify-content:center;width:60px}.web-camera-container .camera-shoot button img[data-v-7eaff898]{height:35px;object-fit:cover}.web-camera-container .camera-loading[data-v-7eaff898]{height:100%;margin:3rem 0 0 -1.2rem;min-height:150px;overflow:hidden;position:absolute;width:100%}.web-camera-container .camera-loading ul[data-v-7eaff898]{height:100%;margin:0;position:absolute;width:100%;z-index:999999}.web-camera-container .camera-loading .loader-circle[data-v-7eaff898]{display:block;height:14px;left:100%;margin:0 auto;padding:0;position:absolute;top:50%;transform:translateY(-50%);transform:translateX(-50%);width:100%}.web-camera-container .camera-loading .loader-circle li[data-v-7eaff898]{animation:preload-7eaff898 1s infinite;background:#999;border-radius:100%;display:block;float:left;height:10px;line-height:10px;margin:0 0 0 4px;padding:0;position:relative;top:-50%;width:10px}.web-camera-container .camera-loading .loader-circle li[data-v-7eaff898]:nth-child(2){animation-delay:.2s}.web-camera-container .camera-loading .loader-circle li[data-v-7eaff898]:nth-child(3){animation-delay:.4s}@keyframes preload-7eaff898{0%{opacity:1}50%{opacity:.4}to{opacity:1}}.textarea[data-v-7eaff898]{border:2px solid #ddd;border-radius:10px;font-size:inherit;min-height:100px;outline:none;padding:20px;width:100%}
```

### Comparing `unigui-1.8.4/unigui/web/icons/favicon-96x96.png` & `unigui-1.8.5/unigui/web/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `unigui-1.8.4/unigui/web/icons/favicon-16x16.png` & `unigui-1.8.5/unigui/web/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `unigui-1.8.4/unigui/web/icons/favicon-32x32.png` & `unigui-1.8.5/unigui/web/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `unigui-1.8.4/unigui/web/icons/favicon-128x128.png` & `unigui-1.8.5/unigui/web/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `unigui-1.8.4/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2` & `unigui-1.8.5/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2`

 * *Files identical despite different names*

### Comparing `unigui-1.8.4/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff` & `unigui-1.8.5/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.8.4/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff` & `unigui-1.8.5/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.8.4/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff` & `unigui-1.8.5/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.8.4/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff` & `unigui-1.8.5/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.8.4/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff` & `unigui-1.8.5/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.8.4/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff` & `unigui-1.8.5/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.8.4/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff` & `unigui-1.8.5/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.8.4/unigui/web/js/786.93a21e48.js` & `unigui-1.8.5/unigui/web/js/164.2b869daf.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,24 +1,24 @@
 "use strict";
 (globalThis["webpackChunkuniqua"] = globalThis["webpackChunkuniqua"] || []).push([
-    [786], {
-        9031: (e, t, a) => {
+    [164], {
+        4164: (e, t, a) => {
             a.r(t), a.d(t, {
-                default: () => Xt
+                default: () => ea
             });
             var l = a(3673),
                 s = a(2323);
             const i = (0, l._)("div", {
                     class: "q-pa-lg"
                 }, null, -1),
-                o = (0, l._)("div", {
+                n = (0, l._)("div", {
                     class: "q-pa-lg"
                 }, null, -1);
 
-            function n(e, t, a, n, d, r) {
+            function o(e, t, a, o, d, r) {
                 const c = (0, l.up)("q-item-label"),
                     h = (0, l.up)("element"),
                     u = (0, l.up)("q-tab"),
                     p = (0, l.up)("q-tabs"),
                     g = (0, l.up)("q-toolbar"),
                     m = (0, l.up)("q-header"),
                     f = (0, l.up)("zone"),
@@ -37,15 +37,15 @@
                             }, {
                                 default: (0, l.w5)((() => [(0, l.Uk)((0, s.zw)(e.screen.header ? e.screen.header : ""), 1)])),
                                 _: 1
                             }), i, ((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e.screen.toolbar, (t => ((0, l.wg)(), (0, l.j4)(h, {
                                 class: "q-ma-xs bg-blue-5",
                                 data: t,
                                 pdata: e.tooldata
-                            }, null, 8, ["data", "pdata"])))), 256)), o, (0, l.Wm)(p, {
+                            }, null, 8, ["data", "pdata"])))), 256)), n, (0, l.Wm)(p, {
                                 class: "text-teal",
                                 align: "center",
                                 "inline-label": "",
                                 dense: "",
                                 modelValue: e.tab,
                                 "onUpdate:modelValue": t[0] || (t[0] = t => e.tab = t),
                                 style: {
@@ -84,15 +84,15 @@
                         })])),
                         _: 1
                     })])),
                     _: 1
                 })
             }
 
-            function d(e, t, a, i, o, n) {
+            function d(e, t, a, i, n, o) {
                 const d = (0, l.up)("q-icon"),
                     r = (0, l.up)("q-item-section"),
                     c = (0, l.up)("q-item-label"),
                     h = (0, l.up)("q-item");
                 return (0, l.wg)(), (0, l.j4)(h, {
                     clickable: "",
                     tag: "a",
@@ -128,432 +128,449 @@
                 y = `height: ${m}px; width: ${f}px`;
 
             function w(e) {
                 let t = e.minheight ? e.minheight : m,
                     a = e.minwidth ? e.minwidth : f;
                 return `height: ${t}px; width: ${a}px`
             }
-            let b = {},
-                k = {};
+            const b = window.location.host,
+                k = `${window.location.protocol}//${b}`;
+            console.log(k);
+            const v = !1;
+            let C = {},
+                q = {};
 
-            function v(e) {
-                p = new WebSocket("ws://localhost:8000/ws"), p.onopen = () => e.statusConnect = !0, p.onmessage = t => {
+            function _(e) {
+                p = new WebSocket(v ? "ws://localhost:8000/ws" : `ws://${b}/ws`), p.onopen = () => e.statusConnect = !0, p.onmessage = t => {
                     g && console.log("incoming message", t.data), e.processMessage(JSON.parse(t.data))
                 }, p.onerror = t => e.error(t), p.onclose = t => {
                     t.wasClean ? e.info("Connection was finished by the server.") : e.error("Connection suddenly closed!"), e.statusConnect = !1, g && console.info("close code : " + t.code + " reason: " + t.reason)
                 }, h = e
             }
 
-            function C(e) {
+            function j(e) {
                 console.log("sended", e), p.send(JSON.stringify(e))
             }
-            let q, _ = 0;
+            let S, z = 0;
 
-            function j() {
-                for (let [e, t] of Object.entries(k)) t.styleSize = null
+            function A() {
+                for (let [e, t] of Object.entries(q)) t.styleSize = null
             }
 
-            function S(e, t, a, l = "complete") {
-                let s = ++_,
+            function Z(e, t, a, l = "complete") {
+                let s = ++z,
                     i = [e.pdata.name, e.data.name, l, t, s];
-                C(i), u[s] = a
+                j(i), u[s] = a
             }
 
-            function z() {
-                b = {}, k = {}
+            function D() {
+                C = {}, q = {}
             }
 
-            function A(e, t) {
+            function M(e, t) {
                 Object.assign(e.data, t), e.updated = t.value, e.value = t.value
             }
 
-            function Z(e) {
+            function $(e) {
                 for (let t of e) {
                     let e = t.path;
                     if (e.length > 1) {
                         e.reverse();
                         let a = e.join("@"),
-                            l = k[a];
-                        A(l, t.data)
+                            l = q[a];
+                        M(l, t.data)
                     } else {
-                        let a = b[e[0]];
+                        let a = C[e[0]];
                         Object.assign(a.data, t.data)
                     }
                 }
             }
 
-            function D(e) {
+            function V(e) {
                 "string" == typeof e.value ? h.error(e.value) : u[e.id](e.value), delete u[e.id]
             }
 
-            function M(e) {
+            function E(e) {
                 let t = [];
                 for (let l of e) l instanceof Array ? t.push(l) : t.push([l]);
                 let a = t.shift();
                 return t.reduce(((e, t) => e.flatMap((e => t.map((t => e instanceof Array ? [...e, t] : [e, t]))))), a)
             }
 
-            function V() {
-                for (let [e, t] of Object.entries(k)) t.expanding && (t.styleSize = w(t.data));
+            function K() {
+                for (let [e, t] of Object.entries(q)) t.expanding && (t.styleSize = w(t.data));
                 (0, l.Y3)((() => {
                     requestAnimationFrame((() => {
                         requestAnimationFrame((() => {
-                            K()
+                            O()
                         }))
                     }))
                 }))
             }
-            let $ = (0, c.debounce)(V, 200);
+            let W = (0, c.debounce)(K, 200);
 
-            function K(e) {
-                Array.isArray(e) && (e = null), q && (q.disconnect(), q = null), g && console.log("------------------recalc design");
-                const t = W(e),
-                    a = E(e);
+            function O(e) {
+                Array.isArray(e) && (e = null), S && (S.disconnect(), S = null), g && console.log("------------------recalc design");
+                const t = Q(e),
+                    a = H(e);
                 for (let [l, s] of Object.entries(t)) {
-                    let e = k[l];
+                    let e = q[l];
                     const [t, i] = a[l];
-                    let o, n = e.geom().el,
+                    let n, o = e.geom().el,
                         d = e.pdata ? e.pdata.name : e.name,
-                        r = b[d];
+                        r = C[d];
                     for (let a of r.data.value.slice(1))
                         if (Array.isArray(a)) {
                             if (a.find((t => t.name == e.data.name))) {
                                 let e = a[a.length - 1],
                                     t = `${e.name}@${d}`;
-                                o = k[t];
+                                n = q[t];
                                 break
                             }
                         } else if (a.name == e.data.name) {
-                        o = e;
+                        n = e;
                         break
                     }
-                    let c = r.data.width ? r.data.width - n.clientWidth - t : r.$el.getBoundingClientRect().right - (o ? o.geom().right : e.geom().right);
+                    let c = r.data.width ? r.data.width - o.clientWidth - t : r.$el.getBoundingClientRect().right - (n ? n.geom().right : e.geom().right);
                     c /= i;
-                    let h = l.startsWith("_scroll@") ? e.geom().inner.clientHeight : n.clientHeight;
-                    e.styleSize = `height: ${h+s}px; width: ${n.clientWidth+c+t}px;`
+                    let h = l.startsWith("_scroll@") ? e.geom().inner.clientHeight : o.clientHeight;
+                    e.styleSize = `height: ${h+s}px; width: ${o.clientWidth+c+t}px;`
                 }
             }
 
-            function W(e) {
+            function Q(e) {
                 const t = h.screen.blocks;
                 let a = window.innerHeight;
                 a -= 2;
                 let l = {},
                     s = new Map,
                     i = {};
-                for (let [d, r] of Object.entries(b)) i[r.name] = r.$el.getBoundingClientRect().height;
-                let o = [];
+                for (let [d, r] of Object.entries(C)) i[r.name] = r.$el.getBoundingClientRect().height;
+                let n = [];
                 for (let d of t) {
                     const e = [];
                     let t = d instanceof Array,
-                        n = t ? M(d) : [
+                        o = t ? E(d) : [
                             [d]
                         ];
-                    for (let a of n) {
+                    for (let a of o) {
                         let e = 0;
                         for (let t of a) e += i[t.name] + 8;
-                        o.push([e, a])
+                        n.push([e, a])
                     }
-                    o.sort(((e, t) => e[0] > t[0] ? -1 : e[0] == t[0] ? 0 : 1));
-                    for (let l of o) {
+                    n.sort(((e, t) => e[0] > t[0] ? -1 : e[0] == t[0] ? 0 : 1));
+                    for (let l of n) {
                         let t = l[1];
                         (0, r.hu)(Array.isArray(t));
                         const i = [];
-                        for (let [e, a] of Object.entries(k))
+                        for (let [e, a] of Object.entries(q))
                             if (a.expanding_height) {
-                                let [l, o] = e.split("@");
-                                if (t.find((e => e.name == o))) {
+                                let [l, n] = e.split("@");
+                                if (t.find((e => e.name == n))) {
                                     let e = !0;
                                     const t = a.geom();
-                                    for (let [l, o] of i.entries()) {
-                                        let n = o.geom();
-                                        if (o !== a && n.top == t.top) {
-                                            n.scrollHeight < t.scrollHeight && (i[l] = a), e = !1, s.set(a.fullname, o.fullname);
+                                    for (let [l, n] of i.entries()) {
+                                        let o = n.geom();
+                                        if (n !== a && o.top == t.top) {
+                                            o.scrollHeight < t.scrollHeight && (i[l] = a), e = !1, s.set(a.fullname, n.fullname);
                                             break
                                         }
                                     }
                                     e && i.push(a)
                                 }
                             } i.length && e.push([a - l[0] - 64, i])
                     }
                     for (let [a, s] of e) {
                         s.sort(((e, t) => e.geom().scrollHeight < t.geom().scrollHeight));
                         let e = s.length;
                         for (let i of s) i.fullname in l && (e--, a -= l[i.fullname]);
                         let t = 0;
                         for (let i of s)
                             if (!(i.fullname in l)) {
-                                let s, o = a / e;
-                                if (1 == e) s = o;
-                                else if (s = Math.floor(o), o - s) {
-                                    t += o - s;
+                                let s, n = a / e;
+                                if (1 == e) s = n;
+                                else if (s = Math.floor(n), n - s) {
+                                    t += n - s;
                                     let e = Math.round(t) - t;
                                     e < .001 && e > -.001 && (s += Math.round(t), t = 0)
                                 }
                                 "docviewer" == i.type ? l[i.fullname] = s + 4 : l[i.fullname] = s
                             }
                     }
                 }
-                let n = Array.from(s.entries());
-                n.sort(((e, t) => e[0] in l || e[1] in l ? -1 : 1));
-                for (let [d, r] of n) r in l ? l[d] = l[r] : l[r] = l[d];
+                let o = Array.from(s.entries());
+                o.sort(((e, t) => e[0] in l || e[1] in l ? -1 : 1));
+                for (let [d, r] of o) r in l ? l[d] = l[r] : l[r] = l[d];
                 return l
             }
 
-            function E(e) {
+            function H(e) {
                 e = null;
                 const t = e ? [e] : h.screen.blocks;
                 let a = window.innerWidth - 30,
                     l = [],
                     s = {};
-                for (let n of t)
+                for (let o of t)
                     if (0 == l.length)
-                        if (Array.isArray(n))
-                            for (let e of n) l.push(Array.isArray(e) ? e : [e]);
+                        if (Array.isArray(o))
+                            for (let e of o) l.push(Array.isArray(e) ? e : [e]);
                         else l = [
-                            [n]
+                            [o]
                         ];
                 else {
                     let e = [];
-                    if (Array.isArray(n))
-                        for (let t of n)
+                    if (Array.isArray(o))
+                        for (let t of o)
                             for (let a of l) e.push(Array.isArray(t) ? a.concat(t) : [...a, t]);
                     else
-                        for (let t of l) e.push([...t, n]);
+                        for (let t of l) e.push([...t, o]);
                     l = e
                 }
                 l.sort(((e, t) => e.length > t.length ? -1 : e.length == t.length ? 0 : 1));
                 const i = [];
-                let o = new Map;
-                for (let n of l) {
-                    let e = Array.isArray(n) ? n[n.length - 1] : n,
-                        t = b[e.name].$el.getBoundingClientRect().right;
-                    e = Array.isArray(n) ? n[0] : n;
-                    let l = b[e.name].$el.getBoundingClientRect().left,
+                let n = new Map;
+                for (let o of l) {
+                    let e = Array.isArray(o) ? o[o.length - 1] : o,
+                        t = C[e.name].$el.getBoundingClientRect().right;
+                    e = Array.isArray(o) ? o[0] : o;
+                    let l = C[e.name].$el.getBoundingClientRect().left,
                         s = a - t + l - 10;
                     const d = [];
-                    for (let [a, i] of Object.entries(k))
+                    for (let [a, i] of Object.entries(q))
                         if (i.expanding_width) {
                             let e = a.split("@")[1];
-                            if (n.find((t => t.name == e))) {
+                            if (o.find((t => t.name == e))) {
                                 let e = !0,
                                     t = i.geom().left;
                                 for (let [a, l] of d.entries())
                                     if (l !== i && l.geom().left == t) {
-                                        l.geom().scrollWidth < i.geom().scrollWidth ? (d[a] = i, o.set(l.fullname, i.fullname)) : o.set(i.fullname, l.fullname), e = !1;
+                                        l.geom().scrollWidth < i.geom().scrollWidth ? (d[a] = i, n.set(l.fullname, i.fullname)) : n.set(i.fullname, l.fullname), e = !1;
                                         break
                                     } e && d.push(i)
                             }
                         } d.length && i.push([s, d])
                 }
-                for (let [n, d] of i) {
+                for (let [o, d] of i) {
                     d.sort(((e, t) => e.geom().scrollWidth - t.geom().scrollWidth));
                     let e = d.length,
                         t = {};
-                    for (let a of d) {
-                        let l = s[a.fullname];
-                        l && (e--, n -= l[0] / l[1]);
-                        let i = a.pdata ? a.pdata.name : a.name;
-                        t[i] ? t[i]++ : t[i] = 1
+                    for (let a = 0; a < d.length; a++) {
+                        let l = d[a],
+                            i = l.parent_name,
+                            n = i || l.name;
+                        if (t[n] ? t[n]++ : t[n] = 1, n = l.parent_name, n) {
+                            let e = C[n];
+                            if (e.data.width) {
+                                let t = a + 1,
+                                    i = d[t];
+                                if (i && i.parent_name != n) {
+                                    let t = l.geom().right - l.geom().left,
+                                        a = e.data.width - t;
+                                    s[l.fullname] = [a, 1]
+                                }
+                            }
+                        }
+                        let r = s[l.fullname];
+                        r && (e--, o -= r[0] / r[1])
                     }
                     for (let a of d) {
                         let l = s[a.fullname];
                         if (void 0 === l) {
                             let l = a.pdata ? a.pdata.name : a.name;
-                            s[a.fullname] = [Math.floor(n / e), t[l]]
+                            s[a.fullname] = [Math.floor(o / e), t[l]]
                         }
                     }
                 }
-                for (let [n, d] of o.entries()) d in s ? s[n] = s[d] : s[d] = s[n];
+                for (let [o, d] of n.entries()) d in s ? s[o] = s[d] : s[d] = s[o];
                 return s
             }
-            const O = (0, l.aZ)({
+            const U = (0, l.aZ)({
                 name: "menubar",
                 methods: {
                     send() {
-                        C(["root", this.name])
+                        j(["root", this.name])
                     }
                 },
                 props: {
                     name: {
                         type: String,
                         required: !0
                     },
                     icon: {
                         type: String,
                         default: ""
                     }
                 }
             });
-            var Q = a(4260),
-                H = a(3414),
-                U = a(2035),
-                N = a(4554),
-                F = a(2350),
-                P = a(7518),
-                T = a.n(P);
-            const I = (0, Q.Z)(O, [
+            var N = a(4260),
+                F = a(3414),
+                T = a(2035),
+                P = a(4554),
+                I = a(2350),
+                R = a(7518),
+                L = a.n(R);
+            const B = (0, N.Z)(U, [
                     ["render", d]
                 ]),
-                R = I;
-            T()(O, "components", {
-                QItem: H.Z,
-                QItemSection: U.Z,
-                QIcon: N.Z,
-                QItemLabel: F.Z
+                Y = B;
+            L()(U, "components", {
+                QItem: F.Z,
+                QItemSection: T.Z,
+                QIcon: P.Z,
+                QItemLabel: I.Z
             });
-            const L = {
+            const X = {
                     key: 0,
                     class: "row q-col-gutter-sm q-py-sm"
                 },
-                B = {
+                G = {
                     class: "q-col-gutter-sm"
                 },
-                Y = {
+                J = {
                     key: 0,
                     class: "column q-col-gutter-sm"
                 };
 
-            function X(e, t, a, s, i, o) {
-                const n = (0, l.up)("zone", !0),
+            function ee(e, t, a, s, i, n) {
+                const o = (0, l.up)("zone", !0),
                     d = (0, l.up)("block");
-                return e.data instanceof Array ? ((0, l.wg)(), (0, l.iD)("div", L, [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e.data, (e => ((0, l.wg)(), (0, l.iD)("div", B, [e instanceof Array ? ((0, l.wg)(), (0, l.iD)("div", Y, [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e, (e => ((0, l.wg)(), (0, l.j4)(n, {
+                return e.data instanceof Array ? ((0, l.wg)(), (0, l.iD)("div", X, [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e.data, (e => ((0, l.wg)(), (0, l.iD)("div", G, [e instanceof Array ? ((0, l.wg)(), (0, l.iD)("div", J, [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e, (e => ((0, l.wg)(), (0, l.j4)(o, {
                     data: e
                 }, null, 8, ["data"])))), 256))])) : ((0, l.wg)(), (0, l.j4)(d, {
                     key: 1,
                     data: e
                 }, null, 8, ["data"]))])))), 256))])) : ((0, l.wg)(), (0, l.j4)(d, {
                     key: 1,
                     data: e.data
                 }, null, 8, ["data"]))
             }
-            const G = {
+            const te = {
                     class: "row"
                 },
-                J = {
+                ae = {
                     key: 2,
                     class: "q-ma-sm",
                     style: {
                         "font-size": "18px"
                     }
                 },
-                ee = ["data", "pdata"],
-                te = {
+                le = ["data", "pdata"],
+                se = {
                     key: 0,
                     class: "row"
                 },
-                ae = ["data", "pdata"],
-                le = {
+                ie = ["data", "pdata"],
+                ne = {
                     key: 0,
                     class: "row"
                 };
 
-            function se(e, t, a, i, o, n) {
+            function oe(e, t, a, i, n, o) {
                 const d = (0, l.up)("element"),
                     r = (0, l.up)("q-icon"),
                     c = (0, l.up)("q-scroll-area"),
                     h = (0, l.up)("q-card");
                 return (0, l.wg)(), (0, l.j4)(h, {
                     class: "my-card q-ma-xs"
                 }, {
-                    default: (0, l.w5)((() => [(0, l._)("div", G, [e.data.logo ? ((0, l.wg)(), (0, l.j4)(d, {
+                    default: (0, l.w5)((() => [(0, l._)("div", te, [e.data.logo ? ((0, l.wg)(), (0, l.j4)(d, {
                         key: 0,
                         data: e.data.logo,
                         pdata: e.data
                     }, null, 8, ["data", "pdata"])) : e.data.icon ? ((0, l.wg)(), (0, l.j4)(r, {
                         key: 1,
                         size: "sm",
                         name: e.data.icon
-                    }, null, 8, ["name"])) : (0, l.kq)("", !0), "_" != e.name[0] ? ((0, l.wg)(), (0, l.iD)("p", J, (0, s.zw)(e.name), 1)) : (0, l.kq)("", !0), ((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e.tops, (t => ((0, l.wg)(), (0, l.j4)(d, {
+                    }, null, 8, ["name"])) : (0, l.kq)("", !0), "_" != e.name[0] ? ((0, l.wg)(), (0, l.iD)("p", ae, (0, s.zw)(e.name), 1)) : (0, l.kq)("", !0), ((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e.tops, (t => ((0, l.wg)(), (0, l.j4)(d, {
                         class: "q-ma-xs",
                         data: t,
                         pdata: e.data
                     }, null, 8, ["data", "pdata"])))), 256))]), e.data.scroll ? ((0, l.wg)(), (0, l.j4)(c, {
                         key: 0,
                         style: (0, s.j5)(e.styleSize),
                         "thumb-style": e.thumbStyle,
                         "bar-style": e.barStyle
                     }, {
                         default: (0, l.w5)((() => [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(e.data.value.slice(1), (t => ((0, l.wg)(), (0, l.iD)("div", {
                             class: "column",
                             data: t,
                             pdata: e.data
-                        }, [t instanceof Array ? ((0, l.wg)(), (0, l.iD)("div", te, [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(t, (t => ((0, l.wg)(), (0, l.j4)(d, {
+                        }, [t instanceof Array ? ((0, l.wg)(), (0, l.iD)("div", se, [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(t, (t => ((0, l.wg)(), (0, l.j4)(d, {
                             class: "q-ma-xs",
                             data: t,
                             pdata: e.data
                         }, null, 8, ["data", "pdata"])))), 256))])) : ((0, l.wg)(), (0, l.j4)(d, {
                             key: 1,
                             class: "q-ma-xs",
                             data: t,
                             pdata: e.data
-                        }, null, 8, ["data", "pdata"]))], 8, ee)))), 256))])),
+                        }, null, 8, ["data", "pdata"]))], 8, le)))), 256))])),
                         _: 1
                     }, 8, ["style", "thumb-style", "bar-style"])) : ((0, l.wg)(!0), (0, l.iD)(l.HY, {
                         key: 1
                     }, (0, l.Ko)(e.data.value.slice(1), (t => ((0, l.wg)(), (0, l.iD)("div", {
                         class: "column",
                         data: t,
                         pdata: e.data
-                    }, [t instanceof Array ? ((0, l.wg)(), (0, l.iD)("div", le, [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(t, (t => ((0, l.wg)(), (0, l.j4)(d, {
+                    }, [t instanceof Array ? ((0, l.wg)(), (0, l.iD)("div", ne, [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(t, (t => ((0, l.wg)(), (0, l.j4)(d, {
                         class: "q-ma-xs",
                         data: t,
                         pdata: e.data
                     }, null, 8, ["data", "pdata"])))), 256))])) : ((0, l.wg)(), (0, l.j4)(d, {
                         key: 1,
                         class: "q-ma-xs",
                         data: t,
                         pdata: e.data
-                    }, null, 8, ["data", "pdata"]))], 8, ae)))), 256))])),
+                    }, null, 8, ["data", "pdata"]))], 8, ie)))), 256))])),
                     _: 1
                 })
             }
-            var ie = a(8880);
-            const oe = e => ((0, l.dD)("data-v-84c697a8"), e = e(), (0, l.Cn)(), e),
-                ne = {
+            var de = a(8880);
+            const re = e => ((0, l.dD)("data-v-7eaff898"), e = e(), (0, l.Cn)(), e),
+                ce = {
                     key: 4
                 },
-                de = ["width", "height"],
-                re = ["src"],
-                ce = {
+                he = ["width", "height"],
+                ue = ["src"],
+                pe = {
                     key: 17,
                     class: "web-camera-container"
                 },
-                he = {
+                ge = {
                     class: "camera-button"
                 },
-                ue = {
+                me = {
                     key: 0
                 },
-                pe = {
+                fe = {
                     key: 1
                 },
-                ge = {
+                ye = {
                     class: "camera-loading"
                 },
-                me = oe((() => (0, l._)("ul", {
+                we = re((() => (0, l._)("ul", {
                     class: "loader-circle"
                 }, [(0, l._)("li"), (0, l._)("li"), (0, l._)("li")], -1))),
-                fe = [me],
-                ye = ["height"],
-                we = ["height"],
-                be = {
+                be = [we],
+                ke = ["height"],
+                ve = ["height"],
+                xe = {
                     key: 1,
                     class: "camera-shoot"
                 },
-                ke = oe((() => (0, l._)("img", {
+                Ce = re((() => (0, l._)("img", {
                     src: "https://img.icons8.com/material-outlined/50/000000/camera--v2.png"
                 }, null, -1))),
-                ve = [ke],
-                xe = {
+                qe = [Ce],
+                _e = {
                     key: 2,
                     class: "camera-download"
                 };
 
-            function Ce(e, t, a, i, o, n) {
+            function je(e, t, a, i, n, o) {
                 const d = (0, l.up)("q-icon"),
                     r = (0, l.up)("q-img"),
                     c = (0, l.up)("q-badge"),
                     h = (0, l.up)("q-select"),
                     u = (0, l.up)("q-checkbox"),
                     p = (0, l.up)("q-toggle"),
                     g = (0, l.up)("q-btn"),
@@ -568,28 +585,28 @@
                     C = (0, l.up)("cgraph"),
                     q = (0, l.up)("q-tooltip"),
                     _ = (0, l.up)("q-spinner-puff");
                 return "image" == e.type ? ((0, l.wg)(), (0, l.j4)(r, {
                     key: 0,
                     src: e.data.name,
                     "spinner-color": "blue",
-                    onClick: (0, ie.iM)(e.switchValue, ["stop"]),
+                    onClick: (0, de.iM)(e.switchValue, ["stop"]),
                     fit: "cover",
                     style: (0, s.j5)(e.elemSize)
                 }, {
                     default: (0, l.w5)((() => [e.data.header ? ((0, l.wg)(), (0, l.iD)("div", {
                         key: 0,
                         class: "absolute-bottom-right text-subtitle2 custom-caption",
-                        onClick: t[0] || (t[0] = (0, ie.iM)(((...t) => e.lens && e.lens(...t)), ["stop"]))
+                        onClick: t[0] || (t[0] = (0, de.iM)(((...t) => e.lens && e.lens(...t)), ["stop"]))
                     }, (0, s.zw)(e.data.header), 1)) : (0, l.kq)("", !0), e.value ? ((0, l.wg)(), (0, l.j4)(d, {
                         key: 1,
                         class: "absolute all-pointer-events",
                         size: "32px",
                         name: "check_circle",
-                        color: "gray",
+                        color: "light-blue-2",
                         style: {
                             "font-size": "2em",
                             top: "8px",
                             left: "8px"
                         }
                     })) : (0, l.kq)("", !0)])),
                     _: 1
@@ -623,15 +640,15 @@
                 }, null, 8, ["modelValue", "label"])) : "switch" == e.type ? ((0, l.wg)(), (0, l.j4)(p, {
                     key: 3,
                     modelValue: e.value,
                     "onUpdate:modelValue": t[3] || (t[3] = t => e.value = t),
                     color: "primary",
                     label: e.nameLabel,
                     "left-label": ""
-                }, null, 8, ["modelValue", "label"])) : "radio" == e.type ? ((0, l.wg)(), (0, l.iD)("div", ne, [e.showname ? ((0, l.wg)(), (0, l.j4)(g, {
+                }, null, 8, ["modelValue", "label"])) : "radio" == e.type ? ((0, l.wg)(), (0, l.iD)("div", ce, [e.showname ? ((0, l.wg)(), (0, l.j4)(g, {
                     key: 0,
                     ripple: !1,
                     color: "secondary",
                     disable: "",
                     label: e.name,
                     "no-caps": ""
                 }, null, 8, ["label"])) : (0, l.kq)("", !0), (0, l.Wm)(m, {
@@ -656,27 +673,27 @@
                     key: 7,
                     modelValue: e.value,
                     "onUpdate:modelValue": t[5] || (t[5] = t => e.value = t),
                     label: e.name,
                     ref: "inputRef",
                     autogrow: e.data.autogrow,
                     dense: "",
-                    onKeyup: (0, ie.D2)(e.pressedEnter, ["enter"]),
+                    onKeyup: (0, de.D2)(e.pressedEnter, ["enter"]),
                     readonly: !1 === e.data.edit
                 }, null, 8, ["modelValue", "label", "autogrow", "onKeyup", "readonly"])) : "number" == e.type ? ((0, l.wg)(), (0, l.j4)(w, {
                     key: 8,
                     modelValue: e.value,
                     "onUpdate:modelValue": t[6] || (t[6] = t => e.value = t),
                     modelModifiers: {
                         number: !0
                     },
                     label: e.name,
                     ref: "inputRef",
                     dense: "",
-                    onKeyup: (0, ie.D2)(e.pressedEnter, ["enter"]),
+                    onKeyup: (0, de.D2)(e.pressedEnter, ["enter"]),
                     type: "number",
                     readonly: !1 === e.data.edit
                 }, null, 8, ["modelValue", "label", "onKeyup", "readonly"])) : "autoedit" == e.type ? ((0, l.wg)(), (0, l.j4)(h, {
                     key: 9,
                     dense: "",
                     modelValue: e.value,
                     "onUpdate:modelValue": t[7] || (t[7] = t => e.value = t),
@@ -686,15 +703,15 @@
                     outlined: "",
                     "hide-bottom-space": "",
                     "fill-input": "",
                     "input-debounce": "0",
                     options: e.options,
                     onFilter: e.complete,
                     label: e.name,
-                    onKeyup: (0, ie.D2)(e.pressedEnter, ["enter"])
+                    onKeyup: (0, de.D2)(e.pressedEnter, ["enter"])
                 }, null, 8, ["modelValue", "options", "onFilter", "label", "onKeyup"])) : "tree" == e.type || "list" == e.type ? ((0, l.wg)(), (0, l.j4)(k, {
                     key: 10,
                     style: (0, s.j5)(e.styleSize),
                     "thumb-style": e.thumbStyle,
                     "bar-style": e.barStyle
                 }, {
                     default: (0, l.w5)((() => [(0, l.Wm)(b, {
@@ -712,91 +729,91 @@
                     key: 11,
                     class: "textarea",
                     "onUpdate:modelValue": t[10] || (t[10] = t => e.value = t),
                     filled: "",
                     type: "textarea",
                     style: (0, s.j5)(e.elemSize)
                 }, null, 4)), [
-                    [ie.nr, e.value]
+                    [de.nr, e.value]
                 ]) : "line" == e.type ? ((0, l.wg)(), (0, l.j4)(v, {
                     key: 12,
                     color: "green"
                 })) : "video" == e.type ? ((0, l.wg)(), (0, l.iD)("video", {
                     width: e.data.width,
                     height: e.data.height,
                     key: e.data.src,
                     controls: ""
                 }, [(0, l._)("source", {
                     src: e.data.src,
                     type: "video/mp4"
-                }, null, 8, re)], 8, de)) : "gallery" == e.type ? ((0, l.wg)(), (0, l.j4)(x, {
+                }, null, 8, ue)], 8, he)) : "uploader" == e.type ? ((0, l.wg)(), (0, l.j4)(x, {
                     key: 14,
                     label: e.name,
                     "auto-upload": "",
                     thumbnails: "",
-                    url: "http://localhost:8000",
+                    url: e.host_path,
                     onUploaded: e.updateDom,
                     onAdded: e.onAdded,
                     style: (0, s.j5)(e.elemSize),
                     ref: "uploaderRef",
                     flat: ""
-                }, null, 8, ["label", "onUploaded", "onAdded", "style"])) : "gimages" == e.type ? ((0, l.wg)(), (0, l.j4)(x, {
+                }, null, 8, ["label", "url", "onUploaded", "onAdded", "style"])) : "image_uploader" == e.type ? ((0, l.wg)(), (0, l.j4)(x, {
                     key: 15,
                     label: e.name,
                     "auto-upload": "",
                     thumbnails: "",
-                    url: "http://localhost:8000",
+                    url: e.host_path,
                     onUploaded: e.updateDom,
                     onAdded: e.onAdded,
                     ref: "uploaderRef",
                     flat: ""
-                }, null, 8, ["label", "onUploaded", "onAdded"])) : "graph" == e.type ? ((0, l.wg)(), (0, l.j4)(C, {
+                }, null, 8, ["label", "url", "onUploaded", "onAdded"])) : "graph" == e.type ? ((0, l.wg)(), (0, l.j4)(C, {
                     key: 16,
                     data: e.data,
                     pdata: e.pdata,
                     styleSize: e.elemSize
-                }, null, 8, ["data", "pdata", "styleSize"])) : "camera" == e.type ? ((0, l.wg)(), (0, l.iD)("div", ce, [(0, l._)("div", he, [(0, l._)("button", {
+                }, null, 8, ["data", "pdata", "styleSize"])) : "camera" == e.type ? ((0, l.wg)(), (0, l.iD)("div", pe, [(0, l._)("div", ge, [(0, l._)("button", {
                     class: (0, s.C_)(["button is-rounded", {
                         "is-primary": !e.isCameraOpen,
                         "is-danger": e.isCameraOpen
                     }]),
                     type: "button",
                     onClick: t[11] || (t[11] = (...t) => e.toggleCamera && e.toggleCamera(...t))
-                }, [e.isCameraOpen ? ((0, l.wg)(), (0, l.iD)("span", pe, "Close Camera")) : ((0, l.wg)(), (0, l.iD)("span", ue, "Open Camera"))], 2)]), (0, l.wy)((0, l._)("div", ge, fe, 512), [
-                    [ie.F8, e.isCameraOpen && e.isLoading]
+                }, [e.isCameraOpen ? ((0, l.wg)(), (0, l.iD)("span", fe, "Close Camera")) : ((0, l.wg)(), (0, l.iD)("span", me, "Open Camera"))], 2)]), (0, l.wy)((0, l._)("div", ye, be, 512), [
+                    [de.F8, e.isCameraOpen && e.isLoading]
                 ]), e.isCameraOpen ? (0, l.wy)(((0, l.wg)(), (0, l.iD)("div", {
                     key: 0,
                     class: (0, s.C_)(["camera-box", {
                         flash: e.isShotPhoto
                     }])
                 }, [(0, l._)("div", {
                     class: (0, s.C_)(["camera-shutter", {
                         flash: e.isShotPhoto
                     }])
                 }, null, 2), (0, l.wy)((0, l._)("video", {
                     ref: "camera",
                     width: 450,
                     height: 337.5,
                     autoplay: ""
-                }, null, 8, ye), [
-                    [ie.F8, !e.isPhotoTaken]
+                }, null, 8, ke), [
+                    [de.F8, !e.isPhotoTaken]
                 ]), (0, l.wy)((0, l._)("canvas", {
                     id: "photoTaken",
                     ref: "canvas",
                     width: 450,
                     height: 337.5
-                }, null, 8, we), [
-                    [ie.F8, e.isPhotoTaken]
+                }, null, 8, ve), [
+                    [de.F8, e.isPhotoTaken]
                 ])], 2)), [
-                    [ie.F8, !e.isLoading]
-                ]) : (0, l.kq)("", !0), e.isCameraOpen && !e.isLoading ? ((0, l.wg)(), (0, l.iD)("div", be, [(0, l._)("button", {
+                    [de.F8, !e.isLoading]
+                ]) : (0, l.kq)("", !0), e.isCameraOpen && !e.isLoading ? ((0, l.wg)(), (0, l.iD)("div", xe, [(0, l._)("button", {
                     class: "button",
                     type: "button",
                     onClick: t[12] || (t[12] = (...t) => e.takePhoto && e.takePhoto(...t))
-                }, ve)])) : (0, l.kq)("", !0), e.isPhotoTaken && e.isCameraOpen ? ((0, l.wg)(), (0, l.iD)("div", xe, [(0, l.Wm)(g, {
+                }, qe)])) : (0, l.kq)("", !0), e.isPhotoTaken && e.isCameraOpen ? ((0, l.wg)(), (0, l.iD)("div", _e, [(0, l.Wm)(g, {
                     onClick: e.downloadImage,
                     label: "Send"
                 }, null, 8, ["onClick"])])) : (0, l.kq)("", !0)])) : "" != e.showname ? ((0, l.wg)(), (0, l.j4)(g, {
                     key: 18,
                     "no-caps": "",
                     label: e.name,
                     icon: e.data.icon,
@@ -839,23 +856,23 @@
                     }, {
                         default: (0, l.w5)((() => [(0, l.Uk)((0, s.zw)(e.data.tooltip), 1)])),
                         _: 1
                     })) : (0, l.kq)("", !0)])),
                     _: 1
                 }, 8, ["icon", "onClick"]))
             }
-            const qe = {
+            const Se = {
                     key: 0
                 },
-                _e = {
+                ze = {
                     class: "row"
                 },
-                je = ["onClick"];
+                Ae = ["onClick"];
 
-            function Se(e, t, a, i, o, n) {
+            function Ze(e, t, a, i, n, o) {
                 const d = (0, l.up)("q-icon"),
                     r = (0, l.up)("q-tooltip"),
                     c = (0, l.up)("q-input"),
                     h = (0, l.up)("q-btn"),
                     u = (0, l.up)("q-th"),
                     p = (0, l.up)("q-tr"),
                     g = (0, l.up)("q-checkbox"),
@@ -877,15 +894,15 @@
                     title: e.name,
                     rows: e.rows,
                     columns: e.columns,
                     selection: e.singleMode ? "single" : "multiple",
                     selected: e.selected,
                     "onUpdate:selected": t[2] || (t[2] = t => e.selected = t)
                 }, {
-                    "top-right": (0, l.w5)((() => [!1 !== e.data.tools ? ((0, l.wg)(), (0, l.iD)("div", qe, [(0, l._)("div", _e, [(0, l.Wm)(c, {
+                    "top-right": (0, l.w5)((() => [!1 !== e.data.tools ? ((0, l.wg)(), (0, l.iD)("div", Se, [(0, l._)("div", ze, [(0, l.Wm)(c, {
                         modelValue: e.search,
                         "onUpdate:modelValue": t[1] || (t[1] = t => e.search = t),
                         label: "Search",
                         dense: "",
                         ref: "searchField"
                     }, (0, l.Nv)({
                         append: (0, l.w5)((() => ["" != e.search ? ((0, l.wg)(), (0, l.j4)(d, {
@@ -1066,75 +1083,75 @@
                                 "onUpdate:modelValue": [e => t.row[a.name] = e, e.change],
                                 dense: "",
                                 onKeydown: e.keyInput,
                                 autofocus: ""
                             }, null, 8, ["modelValue", "onUpdate:modelValue", "onKeydown"])) : ((0, l.wg)(), (0, l.iD)("div", {
                                 key: 3,
                                 onClick: a => e.select(t.row.iiid, i)
-                            }, (0, s.zw)(t.row[a.name]), 9, je))])),
+                            }, (0, s.zw)(t.row[a.name]), 9, Ae))])),
                             _: 2
                         }, 1032, ["props"])))), 128))])),
                         _: 2
                     }, 1032, ["props", "onClick"])])),
                     _: 1
                 }, 8, ["style", "filter", "title", "rows", "columns", "selection", "selected"])
             }
-            var ze = a(1959);
+            var De = a(1959);
 
-            function Ae(e, t) {
+            function Me(e, t) {
                 return e.length === t.length && e.every(((e, a) => e.iiid == t[a].iiid))
             }
-            const Ze = (0, l.aZ)({
+            const $e = (0, l.aZ)({
                 name: "utable",
                 setup(e) {
                     const {
                         data: t,
                         pdata: a
-                    } = (0, ze.BK)(e);
+                    } = (0, De.BK)(e);
                     let s = (0, l.Fl)((() => {
                             let e = [],
                                 a = t.value;
                             const l = a.headers,
                                 s = l.length,
                                 i = a.rows,
-                                o = i.length;
-                            for (var n = 0; n < o; n++) {
+                                n = i.length;
+                            for (var o = 0; o < n; o++) {
                                 const t = {},
-                                    a = i[n];
+                                    a = i[o];
                                 for (var d = 0; d < s; d++) t[l[d]] = a[d];
-                                t.iiid = n, e.push(t)
+                                t.iiid = o, e.push(t)
                             }
                             return e
                         })),
                         i = () => {
                             let e = t.value,
                                 a = null === e.value || 0 == s.value.length ? [] : Array.isArray(e.value) ? e.value.map((e => s.value[e])) : [s.value[e.value]];
                             return a
                         },
-                        o = i(),
-                        n = (0, ze.iH)(o),
-                        d = (0, ze.iH)(o),
-                        r = (0, ze.iH)(!Array.isArray(t.value.value)),
+                        n = i(),
+                        o = (0, De.iH)(n),
+                        d = (0, De.iH)(n),
+                        r = (0, De.iH)(!Array.isArray(t.value.value)),
                         c = (e, l) => {
-                            C([a.value.name, t.value.name, e, l])
+                            j([a.value.name, t.value.name, e, l])
                         },
                         h = (0, l.Fl)((() => r.value ? d.value.length > 0 ? d.value[0].iiid : null : d.value.map((e => e.iiid)))),
                         u = (0, l.Fl)((() => t.value.value));
                     return (0, l.YP)(s, ((e, t) => {
-                        d.value = i(), n.value = d.value
+                        d.value = i(), o.value = d.value
                     })), (0, l.YP)(t, ((e, a) => {
-                        g && console.log("data update", a.name), d.value = i(), n.value = d.value, r.value = !Array.isArray(t.value.value)
+                        g && console.log("data update", a.name), d.value = i(), o.value = d.value, r.value = !Array.isArray(t.value.value)
                     })), {
                         rows: s,
                         value: h,
                         selected: d,
                         singleMode: r,
                         sendMessage: c,
                         datavalue: u,
-                        updated: n
+                        updated: o
                     }
                 },
                 data() {
                     return {
                         search: "",
                         editMode: !1,
                         options: [],
@@ -1208,23 +1225,23 @@
                                         a = typeof t.rows[e][this.cedit];
                                     "string" != a && "number" != a || (t.value = e), this.selected = [this.rows[e]]
                                 }
                                 break
                         }
                     },
                     complete(e, t, a) {
-                        S(this, [e, [this.redit, this.cedit]], (e => t((() => {
+                        Z(this, [e, [this.redit, this.cedit]], (e => t((() => {
                             this.options = e
                         }))))
                     },
                     append() {
                         let e = this.data.rows,
                             t = e.length,
                             a = this;
-                        S(this, [t, this.search], (function(l) {
+                        Z(this, [t, this.search], (function(l) {
                             if (!Array.isArray(l)) return h.error(l);
                             g && console.log("added row", l), a.search = "", e.push(l), setTimeout((() => {
                                 let e = a.rows;
                                 a.selected = [e[t]], a.showSelected(), a.editMode || a.switchEdit(), a.select(e[t], 0)
                             }), 100)
                         }), "append")
                     },
@@ -1259,15 +1276,15 @@
                         }
                         this.selected = []
                     }
                 },
                 watch: {
                     selected(e) {
                         const t = this.data;
-                        if (!Ae(this.updated, this.selected)) {
+                        if (!Me(this.updated, this.selected)) {
                             let e = this.selected.length;
                             this.sendMessage("changed", this.singleMode ? 1 == e ? this.selected[0].iiid : null : this.selected.map((e => e.iiid))), this.updated = this.selected
                         }
                         t.show && (this.showSelected(), t.show = !1), this.editMode && this.selected.length && (t.value = this.selected[0].iiid)
                     }
                 },
                 computed: {
@@ -1292,52 +1309,52 @@
                 },
                 props: {
                     data: Object,
                     pdata: Object,
                     styleSize: String
                 }
             });
-            var De = a(9267),
-                Me = a(4842),
-                Ve = a(8870),
-                $e = a(2165),
-                Ke = a(8186),
-                We = a(2414),
-                Ee = a(3884),
-                Oe = a(5735),
-                Qe = a(7208);
-            const He = (0, Q.Z)(Ze, [
-                    ["render", Se]
+            var Ve = a(9267),
+                Ee = a(4842),
+                Ke = a(8870),
+                We = a(2165),
+                Oe = a(8186),
+                Qe = a(2414),
+                He = a(3884),
+                Ue = a(5735),
+                Ne = a(7208);
+            const Fe = (0, N.Z)($e, [
+                    ["render", Ze]
                 ]),
-                Ue = He;
-            T()(Ze, "components", {
-                QTable: De.Z,
-                QInput: Me.Z,
-                QIcon: N.Z,
-                QTooltip: Ve.Z,
-                QBtn: $e.Z,
-                QTr: Ke.Z,
-                QTh: We.Z,
-                QTd: Ee.Z,
-                QCheckbox: Oe.Z,
-                QSelect: Qe.Z
+                Te = Fe;
+            L()($e, "components", {
+                QTable: Ve.Z,
+                QInput: Ee.Z,
+                QIcon: P.Z,
+                QTooltip: Ke.Z,
+                QBtn: We.Z,
+                QTr: Oe.Z,
+                QTh: Qe.Z,
+                QTd: He.Z,
+                QCheckbox: Ue.Z,
+                QSelect: Ne.Z
             });
-            const Ne = ["nodes", "edges"];
+            const Pe = ["nodes", "edges"];
 
-            function Fe(e, t, a, i, o, n) {
+            function Ie(e, t, a, i, n, o) {
                 return (0, l.wg)(), (0, l.iD)("div", {
                     nodes: e.nodes,
                     edges: e.edges,
                     style: (0, s.j5)(e.styleSize),
                     ref: "cy"
-                }, null, 12, Ne)
+                }, null, 12, Pe)
             }
-            var Pe = a(2393),
-                Te = a.n(Pe);
-            const Ie = Te().stylesheet().selector("node").css({
+            var Re = a(2393),
+                Le = a.n(Re);
+            const Be = Le().stylesheet().selector("node").css({
                     content: "data(id)",
                     "background-color": "#4286f4",
                     "font-size": "14px"
                 }).selector(".selected").css({
                     "background-color": "#ff5555",
                     "border-color": "#ff5555",
                     "font-size": "14px"
@@ -1362,50 +1379,50 @@
                     label: "data(label)",
                     "text-rotation": "autorotate",
                     "text-margin-x": "-8px",
                     "text-margin-y": "-8px",
                     color: "gray",
                     "font-size": "12px"
                 }),
-                Re = {
+                Ye = {
                     animate: !0,
                     randomize: !0
                 };
 
-            function Le(e, t) {
+            function Xe(e, t) {
                 if (e.length != t.length) return !0;
                 for (let a = 0; a < e.length; a++)
                     if (e[a].id != t[a].id || e[a].label != t[a].label) return !0;
                 return !1
             }
-            const Be = (0, l.aZ)({
+            const Ge = (0, l.aZ)({
                     name: "cgraph",
                     props: {
                         data: Object,
                         pdata: Object,
                         styleSize: String
                     },
                     data() {
                         return {
                             cy: null,
-                            style: Ie,
-                            layoutOptions: Re,
+                            style: Be,
+                            layoutOptions: Ye,
                             selectedNodes: [],
                             selectedEdges: [],
                             oldNodes: [],
                             oldEdges: [],
                             shiftKey: !1
                         }
                     },
                     beforeUnmount() {
                         window.removeEventListener("keydown", this.handleKeyDown), window.removeEventListener("keyup", this.handleKeyUp)
                     },
                     mounted() {
                         window.addEventListener("keydown", this.handleKeyDown), window.addEventListener("keyup", this.handleKeyUp);
-                        let e = Te()({
+                        let e = Le()({
                                 container: this.$refs.cy,
                                 elements: {
                                     nodes: this.nodes,
                                     edges: this.edges
                                 },
                                 style: this.style
                             }),
@@ -1455,15 +1472,15 @@
                         },
                         value() {
                             return this.data.value
                         }
                     },
                     methods: {
                         sendMessage(e, t) {
-                            C([this.pdata["name"], this.data["name"], e, t])
+                            j([this.pdata["name"], this.data["name"], e, t])
                         },
                         handleKeyDown(e) {
                             "Shift" == e.key && (this.shiftKey = !0)
                         },
                         handleKeyUp(e) {
                             "Shift" == e.key && (this.shiftKey = !1)
                         },
@@ -1527,15 +1544,15 @@
                                 for (let t of e) a.edges("[id='" + t + "']").addClass("highlighted")
                             }
                         },
                         data: {
                             handler(e, t) {
                                 let a = e.value,
                                     l = !1;
-                                if (void 0 !== a.nodes && this.selectedNodes != a.nodes && (this.selectedNodes = a.nodes), Le(e.nodes, this.oldNodes) && (l = !0, this.oldNodes = e.nodes), void 0 !== a.edges && this.selectedEdges !== a.edges && (this.selectedEdges = a.edges), Le(e.edges, this.oldEdges) && (l = !0, this.oldEdges = e.edges), l && null != this.cy) {
+                                if (void 0 !== a.nodes && this.selectedNodes != a.nodes && (this.selectedNodes = a.nodes), Xe(e.nodes, this.oldNodes) && (l = !0, this.oldNodes = e.nodes), void 0 !== a.edges && this.selectedEdges !== a.edges && (this.selectedEdges = a.edges), Xe(e.edges, this.oldEdges) && (l = !0, this.oldEdges = e.edges), l && null != this.cy) {
                                     this.cy.json({
                                         elements: {
                                             nodes: this.nodes,
                                             edges: this.edges
                                         }
                                     });
                                     let e = this.data.method;
@@ -1552,53 +1569,53 @@
                             this.cy.style(e)
                         },
                         layoutOptions(e) {
                             this.cy.layout(e).run()
                         }
                     }
                 }),
-                Ye = (0, Q.Z)(Be, [
-                    ["render", Fe]
+                Je = (0, N.Z)(Ge, [
+                    ["render", Ie]
                 ]),
-                Xe = Ye;
+                et = Je;
 
-            function Ge(e, t, a, i, o, n) {
+            function tt(e, t, a, i, n, o) {
                 const d = (0, l.up)("v-chart");
                 return (0, l.wg)(), (0, l.j4)(d, {
                     ref: "chart",
-                    option: o.options,
+                    option: n.options,
                     style: (0, s.j5)(a.styleSize),
                     autoresize: !0
                 }, null, 8, ["option", "style"])
             }
-            var Je = a(7559),
-                et = a(4447),
-                tt = a(1006),
-                at = a(3526),
-                lt = a(763),
-                st = a(546),
-                it = a(6902),
-                ot = a(2826),
-                nt = a(5256),
-                dt = a(3825),
-                rt = a(8825);
-            (0, lt.D)([et.N, tt.N, at.N]), (0, lt.D)([st.N, it.N, ot.N, nt.N, dt.N]);
-            let ct = ["", "#80FFA5", "#00DDFF", "#37A2FF", "#FF0087", "#FFBF00", "rgba(128, 255, 165)", "rgba(77, 119, 255)"];
-            const ht = {
+            var at = a(7559),
+                lt = a(4447),
+                st = a(1006),
+                it = a(3526),
+                nt = a(763),
+                ot = a(546),
+                dt = a(6902),
+                rt = a(2826),
+                ct = a(5256),
+                ht = a(3825),
+                ut = a(8825);
+            (0, nt.D)([lt.N, st.N, it.N]), (0, nt.D)([ot.N, dt.N, rt.N, ct.N, ht.N]);
+            let pt = ["", "#80FFA5", "#00DDFF", "#37A2FF", "#FF0087", "#FFBF00", "rgba(128, 255, 165)", "rgba(77, 119, 255)"];
+            const gt = {
                     name: "linechart",
                     components: {
-                        VChart: Je.ZP
+                        VChart: at.ZP
                     },
                     props: {
                         data: Object,
                         pdata: Object,
                         styleSize: String
                     },
                     data() {
-                        const e = (0, rt.Z)();
+                        const e = (0, ut.Z)();
                         return {
                             $q: e,
                             model: !1,
                             options: {
                                 responsive: !0,
                                 maintainAspectRatio: !1,
                                 legend: {
@@ -1664,83 +1681,83 @@
                             let e = this.data.view,
                                 t = this.data.headers;
                             "_" != this.data.name[0] && (this.options.title.text = this.data.name);
                             let a = e.split("-"),
                                 l = a[1].split(",");
                             l.unshift(a[0]);
                             let s = [];
-                            for (let o = 0; o < l.length; o++) l[o] = "i" == l[o] ? -1 : parseInt(l[o]), s.push([]), o && (this.options.series.push({
-                                name: t[l[o]],
+                            for (let n = 0; n < l.length; n++) l[n] = "i" == l[n] ? -1 : parseInt(l[n]), s.push([]), n && (this.options.series.push({
+                                name: t[l[n]],
                                 type: "line",
                                 symbol: "none",
                                 sampling: "lttb",
                                 itemStyle: {
-                                    color: ct[o]
+                                    color: pt[n]
                                 },
-                                data: s[o]
-                            }), this.options.legend.data.push(t[l[o]]));
+                                data: s[n]
+                            }), this.options.legend.data.push(t[l[n]]));
                             this.options.xAxis.data = s[0];
                             let i = this.data.rows;
-                            for (let o = 0; o < i.length; o++)
-                                for (let e = 0; e < l.length; e++) s[e].push(-1 == l[e] ? o : i[o][l[e]]);
+                            for (let n = 0; n < i.length; n++)
+                                for (let e = 0; e < l.length; e++) s[e].push(-1 == l[e] ? n : i[n][l[e]]);
                             this.$refs.chart.setOption(this.options), this.$refs.chart.chart.on("click", (e => alert("!")))
                         }
                     },
                     mounted() {
                         this.calcSeries()
                     }
                 },
-                ut = (0, Q.Z)(ht, [
-                    ["render", Ge]
+                mt = (0, N.Z)(gt, [
+                    ["render", tt]
                 ]),
-                pt = ut;
+                ft = mt;
 
-            function gt(e) {
+            function yt(e) {
                 let t = new FormData;
                 t.append("image", e);
                 let a = new XMLHttpRequest;
-                a.open("POST", "http://localhost:8000", !0), a.onload = function() {
+                a.open("POST", k, !0), a.onload = function() {
                     200 === this.status ? console.log(this.response) : console.error(a)
                 }, a.send(t)
             }
-            const mt = (0, l.aZ)({
+            const wt = (0, l.aZ)({
                 name: "element",
                 components: {
-                    utable: Ue,
-                    cgraph: Xe,
-                    linechart: pt
+                    utable: Te,
+                    cgraph: et,
+                    linechart: ft
                 },
                 methods: {
                     log(e) {
                         console.log(e)
                     },
                     onAdded(e) {
                         0 !== e.length && (0 !== this.fileArr.length ? (this.$refs.uploaderRef.removeFile(this.fileArr[0]), this.fileArr.splice(0, 1, e[0])) : this.fileArr.push(e[0]))
                     },
                     sendMessage(e, t) {
-                        C([this.pdata["name"], this.data["name"], e, t])
+                        j([this.pdata["name"], this.data["name"], e, t])
                     },
                     pressedEnter() {
                         "update" in this.data && this.sendMessage("update", this.value)
                     },
                     updateDom(e) {
                         let t = e.files.length;
-                        t && (this.sendMessage("changed", e.files[t - 1].name), $())
+                        t && this.sendMessage("changed", e.xhr.responseText)
                     },
                     sendValue() {
                         this.sendMessage("changed", this.value)
                     },
                     switchValue() {
                         this.value = !this.value
                     },
                     setValue(e) {
                         this.value = e
                     },
                     complete(e, t, a) {
-                        "" != e && S(this, e, (e => t((() => {
+                        "" != e && Z(this, e, (e => t((() => {
                             this.options = e
                         }))))
                     },
                     lens() {
                         h.lens(this.data)
                     },
                     toggleCamera() {
@@ -1751,15 +1768,15 @@
                         const e = window.constraints = {
                             audio: !1,
                             video: !0
                         };
                         navigator.mediaDevices.getUserMedia(e).then((e => {
                             this.isLoading = !1, this.$refs.camera.srcObject = e
                         })).catch((e => {
-                            this.isLoading = !1, alert("May the browser didn't support or there is some errors.")
+                            this.isLoading = !1, alert("May the browser didn't support or there are some errors.")
                         }))
                     },
                     stopCameraStream() {
                         let e = this.$refs.camera.srcObject.getTracks();
                         e.forEach((e => {
                             e.stop()
                         }))
@@ -1773,15 +1790,19 @@
                             }), e)
                         }
                         this.isPhotoTaken = !this.isPhotoTaken;
                         const e = this.$refs.canvas.getContext("2d");
                         e.drawImage(this.$refs.camera, 0, 0, 450, 337.5)
                     },
                     downloadImage() {
-                        document.getElementById("downloadPhoto"), document.getElementById("photoTaken").toBlob(gt, "image/jpeg")
+                        document.getElementById("downloadPhoto"), document.getElementById("photoTaken").toBlob(yt, "image/jpeg")
+                    },
+                    rect() {
+                        let e = "clientHeight" in this.$el ? this.$el : this.$el.nextElementSibling;
+                        return e.getBoundingClientRect()
                     },
                     geom() {
                         let e = "clientHeight" in this.$el ? this.$el : this.$el.nextElementSibling;
                         e || (e = this.$el.previousElementSibling, e = "clientHeight" in e ? e : e.nextElementSibling);
                         let t = this.type;
                         const a = "docviewer" == t || "graph" == t || "linechart" == t ? e : e.querySelector("table" == t ? ".scroll" : ".q-tree"),
                             l = e.getBoundingClientRect();
@@ -1793,20 +1814,21 @@
                             top: l.top,
                             scrollHeight: a.scrollHeight,
                             scrollWidth: a.scrollWidth
                         }
                     }
                 },
                 mounted() {
-                    k[this.fullname] = this
+                    q[this.fullname] = this
                 },
                 data() {
                     return {
                         value: this.data.value,
                         styleSize: w(this.data),
+                        host_path: k,
                         options: [],
                         expandedKeys: [],
                         thumbStyle: {
                             right: "4px",
                             borderRadius: "7px",
                             backgroundColor: "#027be3",
                             width: "4px",
@@ -1829,14 +1851,17 @@
                     }
                 },
                 computed: {
                     elemSize() {
                         let e = "";
                         return this.data.width && (e = `width:${this.data.width}px`), this.data.height && ("" != e && (e += "; "), e += `height:${this.data.height}px`), "" == e ? this.styleSize : e
                     },
+                    parent_name() {
+                        return this.pdata ? this.pdata.name : null
+                    },
                     name() {
                         return this.data.name
                     },
                     fullname() {
                         return `${this.data.name}@${this.pdata.name}`
                     },
                     showname() {
@@ -1912,53 +1937,53 @@
                         Array.isArray(e) || (e = [0, 0]);
                         let t = this.$refs.inputRef.$el;
                         t.focus();
                         let a = t.getElementsByTagName("textarea");
                         0 == a.length && (a = t.getElementsByTagName("input")), a[0].setSelectionRange(e[0], e[1])
                     },
                     data(e, t) {
-                        this.styleSize || (this.styleSize = w(this.data)), this.value = this.data.value, this.updated = this.value, k[this.fullname] = this
+                        this.styleSize || (this.styleSize = w(this.data)), this.value = this.data.value, this.updated = this.value, q[this.fullname] = this
                     }
                 }
             });
-            var ft = a(4027),
-                yt = a(9721),
-                wt = a(8886),
-                bt = a(8761),
-                kt = a(1232),
-                vt = a(5551),
-                xt = a(5869),
-                Ct = a(1745),
-                qt = a(8430);
-            const _t = (0, Q.Z)(mt, [
-                    ["render", Ce],
-                    ["__scopeId", "data-v-84c697a8"]
+            var bt = a(4027),
+                kt = a(9721),
+                vt = a(8886),
+                xt = a(8761),
+                Ct = a(1232),
+                qt = a(5551),
+                _t = a(5869),
+                jt = a(1745),
+                St = a(8430);
+            const zt = (0, N.Z)(wt, [
+                    ["render", je],
+                    ["__scopeId", "data-v-7eaff898"]
                 ]),
-                jt = _t;
-            T()(mt, "components", {
-                QImg: ft.Z,
-                QIcon: N.Z,
-                QSelect: Qe.Z,
-                QBadge: yt.Z,
-                QCheckbox: Oe.Z,
-                QToggle: wt.Z,
-                QBtn: $e.Z,
-                QBtnToggle: bt.Z,
-                QInput: Me.Z,
-                QScrollArea: kt.Z,
-                QTree: vt.Z,
-                QSeparator: xt.Z,
-                QUploader: Ct.Z,
-                QTooltip: Ve.Z,
-                QSpinnerPuff: qt.Z
+                At = zt;
+            L()(wt, "components", {
+                QImg: bt.Z,
+                QIcon: P.Z,
+                QSelect: Ne.Z,
+                QBadge: kt.Z,
+                QCheckbox: Ue.Z,
+                QToggle: vt.Z,
+                QBtn: We.Z,
+                QBtnToggle: xt.Z,
+                QInput: Ee.Z,
+                QScrollArea: Ct.Z,
+                QTree: qt.Z,
+                QSeparator: _t.Z,
+                QUploader: jt.Z,
+                QTooltip: Ke.Z,
+                QSpinnerPuff: St.Z
             });
-            const St = (0, l.aZ)({
+            const Zt = (0, l.aZ)({
                 name: "block",
                 components: {
-                    element: jt
+                    element: At
                 },
                 data() {
                     return {
                         styleSize: y,
                         thumbStyle: {
                             right: "4px",
                             borderRadius: "7px",
@@ -1973,15 +1998,15 @@
                             width: "8px",
                             opacity: .2
                         }
                     }
                 },
                 methods: {
                     log() {
-                        console.log(Object.keys(b).length, this.name, this.$el.getBoundingClientRect())
+                        console.log(Object.keys(C).length, this.name, this.$el.getBoundingClientRect())
                     },
                     geom() {
                         let e = "clientHeight" in this.$el ? this.$el : this.$el.nextElementSibling;
                         const t = e.querySelector(".q-scrollarea"),
                             a = e.getBoundingClientRect();
                         return {
                             el: e,
@@ -1991,15 +2016,15 @@
                             top: a.top,
                             scrollHeight: window.innerHeight,
                             scrollWidth: window.innerWidth
                         }
                     }
                 },
                 mounted() {
-                    b[this.name] = this, this.expanding && (k[this.fullname] = this)
+                    C[this.name] = this, this.expanding && (q[this.fullname] = this)
                 },
                 computed: {
                     name() {
                         return this.data.name
                     },
                     fullname() {
                         return `_scroll@${this.name}`
@@ -2025,104 +2050,104 @@
                     data: {
                         type: Object,
                         required: !0
                     }
                 },
                 watch: {
                     data(e) {
-                        g && console.log("data update", this.name), this.styleSize = y, b[this.name] = this, this.expanding && (k[this.fullname] = this)
+                        g && console.log("data update", this.name), this.styleSize = y, C[this.name] = this, this.expanding && (q[this.fullname] = this)
                     }
                 }
             });
-            var zt = a(151);
-            const At = (0, Q.Z)(St, [
-                    ["render", se]
+            var Dt = a(151);
+            const Mt = (0, N.Z)(Zt, [
+                    ["render", oe]
                 ]),
-                Zt = At;
-            T()(St, "components", {
-                QCard: zt.Z,
-                QIcon: N.Z,
-                QScrollArea: kt.Z
+                $t = Mt;
+            L()(Zt, "components", {
+                QCard: Dt.Z,
+                QIcon: P.Z,
+                QScrollArea: Ct.Z
             });
-            const Dt = (0, l.aZ)({
+            const Vt = (0, l.aZ)({
                     name: "zone",
                     components: {
-                        block: Zt
+                        block: $t
                     },
                     props: {
                         data: Object
                     },
                     updated(e) {
                         (0, l.Y3)((() => {
                             requestAnimationFrame((() => {
                                 requestAnimationFrame((() => {
-                                    K()
+                                    O()
                                 }))
                             }))
                         }))
                     }
                 }),
-                Mt = (0, Q.Z)(Dt, [
-                    ["render", X]
+                Et = (0, N.Z)(Vt, [
+                    ["render", ee]
                 ]),
-                Vt = Mt,
-                $t = {
+                Kt = Et,
+                Wt = {
                     class: "row q-gutter-sm row-md"
                 };
 
-            function Kt(e, t, a, i, o, n) {
+            function Ot(e, t, a, i, n, o) {
                 const d = (0, l.up)("block"),
                     r = (0, l.up)("q-item-label"),
                     c = (0, l.up)("q-space"),
                     h = (0, l.up)("q-btn"),
                     u = (0, l.up)("q-card"),
                     p = (0, l.up)("q-dialog");
                 return (0, l.wg)(), (0, l.j4)(p, {
                     ref: "dialog",
-                    onHide: n.onDialogHide
+                    onHide: o.onDialogHide
                 }, {
                     default: (0, l.w5)((() => [(0, l.Wm)(u, {
                         class: "q-dialog-plugin q-pa-md items-start q-gutter-md",
                         bordered: "",
                         style: (0, s.j5)(a.data.internal ? "width: 800px; max-width: 80vw;" : "")
                     }, {
                         default: (0, l.w5)((() => [a.data ? ((0, l.wg)(), (0, l.j4)(d, {
                             key: 0,
                             data: a.data
                         }, null, 8, ["data"])) : (0, l.kq)("", !0), (0, l.Wm)(r, {
                             class: "text-h6"
                         }, {
                             default: (0, l.w5)((() => [(0, l.Uk)((0, s.zw)(a.data.text ? a.data.text : ""), 1)])),
                             _: 1
-                        }), (0, l._)("div", $t, [(0, l.Wm)(c), ((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(a.buttons, (e => ((0, l.wg)(), (0, l.j4)(h, {
+                        }), (0, l._)("div", Wt, [(0, l.Wm)(c), ((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(a.buttons, (e => ((0, l.wg)(), (0, l.j4)(h, {
                             class: "col-md-3",
                             label: e,
                             color: a.buttons[0] == e ? "primary" : "secondary",
-                            onClick: t => n.sendMessage(e)
+                            onClick: t => o.sendMessage(e)
                         }, null, 8, ["label", "color", "onClick"])))), 256))])])),
                         _: 1
                     }, 8, ["style"])])),
                     _: 1
                 }, 8, ["onHide"])
             }
-            const Wt = {
+            const Qt = {
                 props: {
                     data: Object,
                     buttons: Array
                 },
                 components: {
-                    block: Zt
+                    block: $t
                 },
                 emits: ["ok", "hide"],
                 methods: {
                     show() {
                         this.$refs.dialog.show()
                     },
                     sendMessage(e) {
-                        this.data.internal || C([this.data["name"], e]), this.hide()
+                        this.data.internal || j([this.data["name"], e]), this.hide()
                     },
                     hide() {
                         this.$refs.dialog.hide()
                     },
                     onDialogHide() {
                         this.$emit("hide")
                     },
@@ -2130,29 +2155,29 @@
                         this.$emit("ok"), this.hide()
                     },
                     onCancelClick() {
                         this.hide()
                     }
                 }
             };
-            var Et = a(5926),
-                Ot = a(2025);
-            const Qt = (0, Q.Z)(Wt, [
-                    ["render", Kt]
+            var Ht = a(5926),
+                Ut = a(2025);
+            const Nt = (0, N.Z)(Qt, [
+                    ["render", Ot]
                 ]),
-                Ht = Qt;
-            T()(Wt, "components", {
-                QDialog: Et.Z,
-                QCard: zt.Z,
-                QItemLabel: F.Z,
-                QSpace: Ot.Z,
-                QBtn: $e.Z
+                Ft = Nt;
+            L()(Qt, "components", {
+                QDialog: Ht.Z,
+                QCard: Dt.Z,
+                QItemLabel: I.Z,
+                QSpace: Ut.Z,
+                QBtn: We.Z
             });
-            let Ut = null;
-            const Nt = (0, l.aZ)({
+            let Tt = null;
+            const Pt = (0, l.aZ)({
                 name: "MainLayout",
                 data() {
                     return {
                         leftDrawerOpen: !1,
                         menu: [],
                         tab: "",
                         tooldata: {
@@ -2162,41 +2187,41 @@
                         statusConnect: !1,
                         screen: {
                             blocks: []
                         }
                     }
                 },
                 components: {
-                    menubar: R,
-                    zone: Vt,
-                    element: jt
+                    menubar: Y,
+                    zone: Kt,
+                    element: At
                 },
                 created() {
-                    v(this)
+                    _(this)
                 },
                 unmounted() {
                     window.removeEventListener("resize", this.onResize)
                 },
                 methods: {
                     toggleLeftDrawer() {
                         this.leftDrawerOpen = !this.leftDrawerOpen
                     },
                     tabclick(e) {
-                        C(["root", e])
+                        j(["root", e])
                     },
                     onResize(e) {
-                        g && console.log("window has been resized", window.innerHeight, window.innerWidth), $()
+                        g && console.log("window has been resized", window.innerHeight, window.innerWidth), W()
                     },
                     lens(e) {
                         let t = {
                                 title: "Photo lens",
                                 message: e.text,
                                 cancel: !0,
                                 persistent: !0,
-                                component: Ht
+                                component: Ft
                             },
                             {
                                 height: a,
                                 ...l
                             } = e;
                         l.width = 750;
                         let s = {
@@ -2215,80 +2240,80 @@
                         let a = t,
                             l = {
                                 message: e,
                                 type: t,
                                 position: "top",
                                 icon: a
                             };
-                        "progress" == t ? null == Ut ? (l = {
+                        "progress" == t ? null == Tt ? (l = {
                             group: !1,
                             timeout: 0,
                             spinner: !0,
                             type: "info",
                             message: e || "Progress..",
                             position: "top",
                             color: "secondary"
-                        }, Ut = this.$q.notify(l)) : null == e ? (Ut(), Ut = null) : (l = {
+                        }, Tt = this.$q.notify(l)) : null == e ? (Tt(), Tt = null) : (l = {
                             caption: e
-                        }, Ut(l)) : ("error" == t && l.type, this.$q.notify(l))
+                        }, Tt(l)) : ("error" == t && l.type, this.$q.notify(l))
                     },
                     error(e) {
                         this.notify(e, "error")
                     },
                     info(e) {
                         this.notify(e, "info")
                     },
                     processMessage(e) {
-                        if ("screen" == e.type) this.screen.name != e.name && j(), z(), this.screen = e, this.menu = e.menu.map((e => ({
+                        if ("screen" == e.type) this.screen.name != e.name && A(), D(), this.screen = e, this.menu = e.menu.map((e => ({
                             name: e[0],
                             icon: e[1],
                             order: e[2]
                         }))), this.tab = this.screen.name;
                         else if ("dialog" == e.type) {
                             let t = {
                                 title: e.name,
                                 message: e.text,
                                 cancel: !0,
                                 persistent: !0
                             };
-                            t.component = Ht, t.componentProps = {
+                            t.component = Ft, t.componentProps = {
                                 data: e.content ? e.content : e,
                                 buttons: e.buttons
                             }, this.$q.dialog(t)
-                        } else if ("answer" == e.type) D(e);
+                        } else if ("answer" == e.type) V(e);
                         else {
-                            e.updates && Z(e.updates);
+                            e.updates && $(e.updates);
                             let t = !1;
                             ["error", "progress", "warning", "info"].includes(e.type) && (this.notify(e.value, e.type), t = !0), t || e.updates || (this.error("Invalid data came from the server! Look the console."), console.log(`Invalid data came from the server! ${e}`))
                         }
-                        Ut && "progress" != e.type && this.notify(null, "progress")
+                        Tt && "progress" != e.type && this.notify(null, "progress")
                     }
                 },
                 mounted() {
                     window.addEventListener("resize", this.onResize)
                 }
             });
-            var Ft = a(9214),
-                Pt = a(3812),
-                Tt = a(9570),
-                It = a(7547),
-                Rt = a(3269),
-                Lt = a(2652),
-                Bt = a(4379);
-            const Yt = (0, Q.Z)(Nt, [
-                    ["render", n]
+            var It = a(9214),
+                Rt = a(3812),
+                Lt = a(9570),
+                Bt = a(7547),
+                Yt = a(3269),
+                Xt = a(2652),
+                Gt = a(4379);
+            const Jt = (0, N.Z)(Pt, [
+                    ["render", o]
                 ]),
-                Xt = Yt;
-            T()(Nt, "components", {
-                QLayout: Ft.Z,
-                QHeader: Pt.Z,
-                QToolbar: Tt.Z,
-                QBtn: $e.Z,
-                QItemLabel: F.Z,
-                QTabs: It.Z,
-                QTab: Rt.Z,
-                QPageContainer: Lt.Z,
-                QPage: Bt.Z
+                ea = Jt;
+            L()(Pt, "components", {
+                QLayout: It.Z,
+                QHeader: Rt.Z,
+                QToolbar: Lt.Z,
+                QBtn: We.Z,
+                QItemLabel: I.Z,
+                QTabs: Bt.Z,
+                QTab: Yt.Z,
+                QPageContainer: Xt.Z,
+                QPage: Gt.Z
             })
         }
     }
 ]);
```

### Comparing `unigui-1.8.4/unigui/web/js/430.591e9a73.js` & `unigui-1.8.5/unigui/web/js/430.591e9a73.js`

 * *Files identical despite different names*

### Comparing `unigui-1.8.4/unigui/web/js/vendor.3076c5e7.js` & `unigui-1.8.5/unigui/web/js/vendor.3076c5e7.js`

 * *Files identical despite different names*

### Comparing `unigui-1.8.4/unigui/web/js/app.4491f085.js` & `unigui-1.8.5/unigui/web/js/app.e17901f8.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -22,15 +22,15 @@
                         ["render", l]
                     ]),
                     d = c;
                 var p = r(3340),
                     f = r(8339);
                 const h = [{
                         path: "/",
-                        component: () => Promise.all([r.e(736), r.e(786)]).then(r.bind(r, 9031)),
+                        component: () => Promise.all([r.e(736), r.e(164)]).then(r.bind(r, 4164)),
                         children: [{
                             path: "",
                             component: () => Promise.all([r.e(736), r.e(430)]).then(r.bind(r, 6430))
                         }]
                     }, {
                         path: "/:catchAll(.*)*",
                         component: () => Promise.all([r.e(736), r.e(193)]).then(r.bind(r, 2193))
@@ -158,26 +158,26 @@
                 get: t[n]
             })
         }
     })(), (() => {
         r.f = {}, r.e = e => Promise.all(Object.keys(r.f).reduce(((t, n) => (r.f[n](e, t), t)), []))
     })(), (() => {
         r.u = e => "js/" + e + "." + {
+            164: "2b869daf",
             193: "283445be",
-            430: "591e9a73",
-            786: "93a21e48"
+            430: "591e9a73"
         } [e] + ".js"
     })(), (() => {
         r.miniCssF = e => "css/" + ({
             143: "app",
             736: "vendor"
         } [e] || e) + "." + {
             143: "31d6cfe0",
-            736: "191faa77",
-            786: "d75b8133"
+            164: "06cedad1",
+            736: "191faa77"
         } [e] + ".css"
     })(), (() => {
         r.g = function() {
             if ("object" === typeof globalThis) return globalThis;
             try {
                 return this || new Function("return this")()
             } catch (e) {
@@ -260,15 +260,15 @@
                 e(n, l, o, a)
             })),
             o = {
                 143: 0
             };
         r.f.miniCss = (e, t) => {
             var r = {
-                786: 1
+                164: 1
             };
             o[e] ? t.push(o[e]) : 0 !== o[e] && r[e] && t.push(o[e] = n(e).then((() => {
                 o[e] = 0
             }), (t => {
                 throw delete o[e], t
             })))
         }
```

### Comparing `unigui-1.8.4/unigui/web/js/193.283445be.js` & `unigui-1.8.5/unigui/web/js/193.283445be.js`

 * *Files identical despite different names*

### Comparing `unigui-1.8.4/unigui/web/index.html` & `unigui-1.8.5/unigui/web/index.html`

 * *Files 8% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html><head><title>Unigui</title><meta charset=utf-8><meta name=description content="Unigui on Quasar"><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><link rel=icon type=image/png sizes=96x96 href=icons/favicon-96x96.png><link rel=icon type=image/png sizes=32x32 href=icons/favicon-32x32.png><link rel=icon type=image/png sizes=16x16 href=icons/favicon-16x16.png><link rel=icon type=image/ico href=favicon.ico><script defer src=js/vendor.3076c5e7.js></script><script defer src=js/app.4491f085.js></script><link href=css/vendor.191faa77.css rel=stylesheet><link href=css/app.31d6cfe0.css rel=stylesheet></head><body><div id=q-app></div></body></html>
+<!DOCTYPE html><html><head><title>Unigui</title><meta charset=utf-8><meta name=description content="Unigui on Quasar"><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><link rel=icon type=image/png sizes=96x96 href=icons/favicon-96x96.png><link rel=icon type=image/png sizes=32x32 href=icons/favicon-32x32.png><link rel=icon type=image/png sizes=16x16 href=icons/favicon-16x16.png><link rel=icon type=image/ico href=favicon.ico><script defer src=js/vendor.3076c5e7.js></script><script defer src=js/app.e17901f8.js></script><link href=css/vendor.191faa77.css rel=stylesheet><link href=css/app.31d6cfe0.css rel=stylesheet></head><body><div id=q-app></div></body></html>
```

### Comparing `unigui-1.8.4/LICENSE` & `unigui-1.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `unigui-1.8.4/setup.py` & `unigui-1.8.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
  
 setup(name='unigui',
-      version='1.8.4',      
+      version='1.8.5',      
       license='MIT',
       author='Georgii Dernovyi',
       author_email='g.dernovoy@gmail.com',
       description='Unigui - Universal GUI Framework and protocol',
       packages=find_packages(exclude=['tests']),
       long_description=open('README.md').read(),
       long_description_content_type="text/markdown",
```

### Comparing `unigui-1.8.4/PKG-INFO` & `unigui-1.8.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.8.4
+Version: 1.8.5
 Summary: Unigui - Universal GUI Framework and protocol
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -293,14 +293,16 @@
 Unigui counts rows id as an index in a rows array. If table does not contain append, delete arguments, then it will be drawn without add and remove icons.  
 value = [0] means 0 row is selected in multiselect mode (in array). multimode is False so switch icon for single select mode will be not drawn and switching to single select mode is not allowed.
 
 | Table option parameter |	Description |
 | :---: | :---: | 
 | changed  | table handler accept the selected row number |
 | complete |  Autocomplete handler as with value type (string value, (row index, column index)) that returns a string list of possible complitions |
+| append |  A handler gets new row index and return filled row with proposed values, has system append_table_row by default |
+| delete | A handler gets list or index of selected rows and remove them. system delete_table_row by default |
 | update | called when the user presses the Enter in a table cell |
 | modify | default = accept_rowvalue(table, value). called when the cell value is changed by the user |
 | edit   | default True. if true user can edit table, using standart or overloaded table methods |
 | tools  | default True, then  Table has toolbar with search field and icon action buttons. |
 | show   | default False, the table scrolls to (the first) selected row, if True and it is not visible |
 | multimode | default True, allows to select single or multi selection mode |
```

### Comparing `unigui-1.8.4/README.md` & `unigui-1.8.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -281,14 +281,16 @@
 Unigui counts rows id as an index in a rows array. If table does not contain append, delete arguments, then it will be drawn without add and remove icons.  
 value = [0] means 0 row is selected in multiselect mode (in array). multimode is False so switch icon for single select mode will be not drawn and switching to single select mode is not allowed.
 
 | Table option parameter |	Description |
 | :---: | :---: | 
 | changed  | table handler accept the selected row number |
 | complete |  Autocomplete handler as with value type (string value, (row index, column index)) that returns a string list of possible complitions |
+| append |  A handler gets new row index and return filled row with proposed values, has system append_table_row by default |
+| delete | A handler gets list or index of selected rows and remove them. system delete_table_row by default |
 | update | called when the user presses the Enter in a table cell |
 | modify | default = accept_rowvalue(table, value). called when the cell value is changed by the user |
 | edit   | default True. if true user can edit table, using standart or overloaded table methods |
 | tools  | default True, then  Table has toolbar with search field and icon action buttons. |
 | show   | default False, the table scrolls to (the first) selected row, if True and it is not visible |
 | multimode | default True, allows to select single or multi selection mode |
```

### Comparing `unigui-1.8.4/unigui.egg-info/PKG-INFO` & `unigui-1.8.5/unigui.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.8.4
+Version: 1.8.5
 Summary: Unigui - Universal GUI Framework and protocol
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -293,14 +293,16 @@
 Unigui counts rows id as an index in a rows array. If table does not contain append, delete arguments, then it will be drawn without add and remove icons.  
 value = [0] means 0 row is selected in multiselect mode (in array). multimode is False so switch icon for single select mode will be not drawn and switching to single select mode is not allowed.
 
 | Table option parameter |	Description |
 | :---: | :---: | 
 | changed  | table handler accept the selected row number |
 | complete |  Autocomplete handler as with value type (string value, (row index, column index)) that returns a string list of possible complitions |
+| append |  A handler gets new row index and return filled row with proposed values, has system append_table_row by default |
+| delete | A handler gets list or index of selected rows and remove them. system delete_table_row by default |
 | update | called when the user presses the Enter in a table cell |
 | modify | default = accept_rowvalue(table, value). called when the cell value is changed by the user |
 | edit   | default True. if true user can edit table, using standart or overloaded table methods |
 | tools  | default True, then  Table has toolbar with search field and icon action buttons. |
 | show   | default False, the table scrolls to (the first) selected row, if True and it is not visible |
 | multimode | default True, allows to select single or multi selection mode |
```

### Comparing `unigui-1.8.4/unigui.egg-info/SOURCES.txt` & `unigui-1.8.5/unigui.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -13,27 +13,27 @@
 unigui.egg-info/SOURCES.txt
 unigui.egg-info/dependency_links.txt
 unigui.egg-info/not-zip-safe
 unigui.egg-info/requires.txt
 unigui.egg-info/top_level.txt
 unigui/web/favicon.ico
 unigui/web/index.html
-unigui/web/css/786.d75b8133.css
+unigui/web/css/164.06cedad1.css
 unigui/web/css/app.31d6cfe0.css
 unigui/web/css/vendor.191faa77.css
 unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
 unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
 unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
 unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2
 unigui/web/icons/favicon-128x128.png
 unigui/web/icons/favicon-16x16.png
 unigui/web/icons/favicon-32x32.png
 unigui/web/icons/favicon-96x96.png
+unigui/web/js/164.2b869daf.js
 unigui/web/js/193.283445be.js
 unigui/web/js/430.591e9a73.js
-unigui/web/js/786.93a21e48.js
-unigui/web/js/app.4491f085.js
+unigui/web/js/app.e17901f8.js
 unigui/web/js/vendor.3076c5e7.js
```

