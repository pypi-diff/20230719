# Comparing `tmp/rubpy-6.2.6.tar.gz` & `tmp/rubpy-6.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubpy-6.2.6.tar", last modified: Tue Jul 18 01:20:09 2023, max compression
+gzip compressed data, was "rubpy-6.2.7.tar", last modified: Wed Jul 19 15:54:44 2023, max compression
```

## Comparing `rubpy-6.2.6.tar` & `rubpy-6.2.7.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 01:20:09.777094 rubpy-6.2.6/
--rw-rw-rw-   0        0        0     3378 2023-07-18 01:20:09.777094 rubpy-6.2.6/PKG-INFO
--rw-rw-rw-   0        0        0     2238 2023-04-26 17:35:11.000000 rubpy-6.2.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-18 01:20:09.730214 rubpy-6.2.6/rubpy/
--rw-rw-rw-   0        0        0      240 2023-06-29 13:16:44.000000 rubpy-6.2.6/rubpy/__init__.py
--rw-rw-rw-   0        0        0    44856 2023-07-18 01:17:24.000000 rubpy-6.2.6/rubpy/client.py
-drwxrwxrwx   0        0        0        0 2023-07-18 01:20:09.761471 rubpy-6.2.6/rubpy/crypto/
--rw-rw-rw-   0        0        0       26 2022-09-12 11:03:20.000000 rubpy-6.2.6/rubpy/crypto/__init__.py
--rw-rw-rw-   0        0        0     2891 2023-06-14 11:35:15.000000 rubpy-6.2.6/rubpy/crypto/crypto.py
-drwxrwxrwx   0        0        0        0 2023-07-18 01:20:09.761471 rubpy-6.2.6/rubpy/gadgets/
--rw-rw-rw-   0        0        0      106 2022-09-12 11:03:20.000000 rubpy-6.2.6/rubpy/gadgets/__init__.py
--rw-rw-rw-   0        0        0      892 2023-06-14 19:16:37.000000 rubpy-6.2.6/rubpy/gadgets/classino.py
--rw-rw-rw-   0        0        0     2118 2023-04-26 18:12:01.000000 rubpy-6.2.6/rubpy/gadgets/exceptions.py
--rw-rw-rw-   0        0        0    27137 2023-06-15 19:36:00.000000 rubpy-6.2.6/rubpy/gadgets/grouping.py
--rw-rw-rw-   0        0        0    14188 2023-04-26 17:30:17.000000 rubpy-6.2.6/rubpy/gadgets/methods.py
--rw-rw-rw-   0        0        0     6772 2023-06-29 12:36:38.000000 rubpy-6.2.6/rubpy/gadgets/thumbnail.py
-drwxrwxrwx   0        0        0        0 2023-07-18 01:20:09.761471 rubpy-6.2.6/rubpy/network/
--rw-rw-rw-   0        0        0       64 2022-09-12 11:03:20.000000 rubpy-6.2.6/rubpy/network/__init__.py
--rw-rw-rw-   0        0        0    11464 2023-07-18 01:15:37.000000 rubpy-6.2.6/rubpy/network/connection.py
--rw-rw-rw-   0        0        0    14807 2022-09-12 11:03:20.000000 rubpy-6.2.6/rubpy/network/proxies.py
-drwxrwxrwx   0        0        0        0 2023-07-18 01:20:09.777094 rubpy-6.2.6/rubpy/sessions/
--rw-rw-rw-   0        0        0       82 2022-09-12 11:03:20.000000 rubpy-6.2.6/rubpy/sessions/__init__.py
--rw-rw-rw-   0        0        0     2295 2023-06-14 11:13:33.000000 rubpy-6.2.6/rubpy/sessions/sqliteSession.py
--rw-rw-rw-   0        0        0     1223 2022-09-12 11:03:20.000000 rubpy-6.2.6/rubpy/sessions/stringSession.py
-drwxrwxrwx   0        0        0        0 2023-07-18 01:20:09.777094 rubpy-6.2.6/rubpy/structs/
--rw-rw-rw-   0        0        0       99 2022-09-12 11:03:20.000000 rubpy-6.2.6/rubpy/structs/__init__.py
--rw-rw-rw-   0        0        0     1985 2022-09-12 11:03:20.000000 rubpy-6.2.6/rubpy/structs/handlers.py
--rw-rw-rw-   0        0        0     4585 2022-09-12 11:03:20.000000 rubpy-6.2.6/rubpy/structs/models.py
--rw-rw-rw-   0        0        0      702 2022-09-12 11:03:20.000000 rubpy-6.2.6/rubpy/structs/results.py
--rw-rw-rw-   0        0        0    15140 2023-04-23 17:55:22.000000 rubpy-6.2.6/rubpy/structs/struct.py
-drwxrwxrwx   0        0        0        0 2023-07-18 01:20:09.761471 rubpy-6.2.6/rubpy.egg-info/
--rw-rw-rw-   0        0        0     3378 2023-07-18 01:20:09.000000 rubpy-6.2.6/rubpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      697 2023-07-18 01:20:09.000000 rubpy-6.2.6/rubpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 01:20:09.000000 rubpy-6.2.6/rubpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-07-18 01:20:09.000000 rubpy-6.2.6/rubpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-18 01:20:09.000000 rubpy-6.2.6/rubpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-18 01:20:09.777094 rubpy-6.2.6/setup.cfg
--rw-rw-rw-   0        0        0     1547 2023-07-18 01:17:55.000000 rubpy-6.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 15:54:44.720332 rubpy-6.2.7/
+-rw-rw-rw-   0        0        0     3378 2023-07-19 15:54:44.720332 rubpy-6.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2238 2023-04-26 17:35:11.000000 rubpy-6.2.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-19 15:54:44.689082 rubpy-6.2.7/rubpy/
+-rw-rw-rw-   0        0        0      240 2023-07-19 15:44:17.000000 rubpy-6.2.7/rubpy/__init__.py
+-rw-rw-rw-   0        0        0    44693 2023-07-19 15:51:55.000000 rubpy-6.2.7/rubpy/client.py
+drwxrwxrwx   0        0        0        0 2023-07-19 15:54:44.704707 rubpy-6.2.7/rubpy/crypto/
+-rw-rw-rw-   0        0        0       26 2022-09-12 11:03:20.000000 rubpy-6.2.7/rubpy/crypto/__init__.py
+-rw-rw-rw-   0        0        0     3288 2023-07-19 15:43:06.000000 rubpy-6.2.7/rubpy/crypto/crypto.py
+drwxrwxrwx   0        0        0        0 2023-07-19 15:54:44.704707 rubpy-6.2.7/rubpy/gadgets/
+-rw-rw-rw-   0        0        0      106 2022-09-12 11:03:20.000000 rubpy-6.2.7/rubpy/gadgets/__init__.py
+-rw-rw-rw-   0        0        0      892 2023-06-14 19:16:37.000000 rubpy-6.2.7/rubpy/gadgets/classino.py
+-rw-rw-rw-   0        0        0     2118 2023-04-26 18:12:01.000000 rubpy-6.2.7/rubpy/gadgets/exceptions.py
+-rw-rw-rw-   0        0        0    27137 2023-06-15 19:36:00.000000 rubpy-6.2.7/rubpy/gadgets/grouping.py
+-rw-rw-rw-   0        0        0    14188 2023-04-26 17:30:17.000000 rubpy-6.2.7/rubpy/gadgets/methods.py
+-rw-rw-rw-   0        0        0     6772 2023-06-29 12:36:38.000000 rubpy-6.2.7/rubpy/gadgets/thumbnail.py
+drwxrwxrwx   0        0        0        0 2023-07-19 15:54:44.720332 rubpy-6.2.7/rubpy/network/
+-rw-rw-rw-   0        0        0       64 2022-09-12 11:03:20.000000 rubpy-6.2.7/rubpy/network/__init__.py
+-rw-rw-rw-   0        0        0    12211 2023-07-19 15:35:24.000000 rubpy-6.2.7/rubpy/network/connection.py
+-rw-rw-rw-   0        0        0    14807 2022-09-12 11:03:20.000000 rubpy-6.2.7/rubpy/network/proxies.py
+drwxrwxrwx   0        0        0        0 2023-07-19 15:54:44.720332 rubpy-6.2.7/rubpy/sessions/
+-rw-rw-rw-   0        0        0       82 2022-09-12 11:03:20.000000 rubpy-6.2.7/rubpy/sessions/__init__.py
+-rw-rw-rw-   0        0        0     2295 2023-06-14 11:13:33.000000 rubpy-6.2.7/rubpy/sessions/sqliteSession.py
+-rw-rw-rw-   0        0        0     1223 2022-09-12 11:03:20.000000 rubpy-6.2.7/rubpy/sessions/stringSession.py
+drwxrwxrwx   0        0        0        0 2023-07-19 15:54:44.720332 rubpy-6.2.7/rubpy/structs/
+-rw-rw-rw-   0        0        0       99 2022-09-12 11:03:20.000000 rubpy-6.2.7/rubpy/structs/__init__.py
+-rw-rw-rw-   0        0        0     1985 2022-09-12 11:03:20.000000 rubpy-6.2.7/rubpy/structs/handlers.py
+-rw-rw-rw-   0        0        0     4585 2022-09-12 11:03:20.000000 rubpy-6.2.7/rubpy/structs/models.py
+-rw-rw-rw-   0        0        0      702 2022-09-12 11:03:20.000000 rubpy-6.2.7/rubpy/structs/results.py
+-rw-rw-rw-   0        0        0    15140 2023-04-23 17:55:22.000000 rubpy-6.2.7/rubpy/structs/struct.py
+drwxrwxrwx   0        0        0        0 2023-07-19 15:54:44.704707 rubpy-6.2.7/rubpy.egg-info/
+-rw-rw-rw-   0        0        0     3378 2023-07-19 15:54:44.000000 rubpy-6.2.7/rubpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      697 2023-07-19 15:54:44.000000 rubpy-6.2.7/rubpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 15:54:44.000000 rubpy-6.2.7/rubpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-07-19 15:54:44.000000 rubpy-6.2.7/rubpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-19 15:54:44.000000 rubpy-6.2.7/rubpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-19 15:54:44.720332 rubpy-6.2.7/setup.cfg
+-rw-rw-rw-   0        0        0     1547 2023-07-19 15:44:09.000000 rubpy-6.2.7/setup.py
```

### Comparing `rubpy-6.2.6/PKG-INFO` & `rubpy-6.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubpy
-Version: 6.2.6
+Version: 6.2.7
 Summary: This is an unofficial library and fastest library for deploying robots on Rubika accounts.
 Home-page: https://github.com/shayanheidari01/rubika
 Author: Shayan Heidari
 Author-email: contact@shayanheidari.info
 Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rubpy Version: 6.2.6 Summary: This is an unofficial
+Metadata-Version: 2.1 Name: rubpy Version: 6.2.7 Summary: This is an unofficial
 library and fastest library for deploying robots on Rubika accounts. Home-page:
 https://github.com/shayanheidari01/rubika Author: Shayan Heidari Author-email:
 contact@shayanheidari.info Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `rubpy-6.2.6/README.md` & `rubpy-6.2.7/README.md`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.6/rubpy/client.py` & `rubpy-6.2.7/rubpy/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -728,40 +728,34 @@
 
     async def send_music(self,
         object_guid: str,
         music: bytes,
         caption: str = None,
         file_name: str = None,
         time: str = None,
-        music_performer: str = None,
+        performer: str = None,
         reply_to_message_id: str = None,
         *args,
         **kwargs,
     ):
         if object_guid.lower() in ('me', 'self', 'cloud'):
             object_guid = self._guid
 
-        if type(music) != bytes:
-            async with aiofiles.open(music, 'rb') as file:
-                file_name = os.path.basename(music)
-                kwargs['file_name'] = kwargs.get('file_name', file_name)
-                file = await file.read()
-                await file.close()
-        else:
+        if isinstance(music, bytes):
             kwargs['file_name'] = kwargs.get('file_name', file_name)
+        else:
+            async with aiofiles.open(music, 'rb') as file:
+                kwargs['file_name'] = kwargs.get('file_name', os.path.basename(music))
+                music = await file.read()
 
         file_inline = await self.upload(music, *args, **kwargs)
         file_inline['type'] = 'Music'
         file_inline['auto_play'] = False
-        file_inline['music_performer'] = kwargs.get('performer', music_performer or '')
-
-        if time != None:
-            file_inline['time'] = time
-        else:
-            file_inline['time'] = '60'
+        file_inline['music_performer'] = kwargs.get('performer', performer or '')
+        file_inline['time'] = time or 60
 
         return await self(
             methods.messages.SendMessage(
                 object_guid,
                 message=caption,
                 file_inline=file_inline,
                 reply_to_message_id=reply_to_message_id))
```

### Comparing `rubpy-6.2.6/rubpy/gadgets/classino.py` & `rubpy-6.2.7/rubpy/gadgets/classino.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.6/rubpy/gadgets/exceptions.py` & `rubpy-6.2.7/rubpy/gadgets/exceptions.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.6/rubpy/gadgets/grouping.py` & `rubpy-6.2.7/rubpy/gadgets/grouping.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.6/rubpy/gadgets/methods.py` & `rubpy-6.2.7/rubpy/gadgets/methods.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.6/rubpy/gadgets/thumbnail.py` & `rubpy-6.2.7/rubpy/gadgets/thumbnail.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.6/rubpy/network/connection.py` & `rubpy-6.2.7/rubpy/network/connection.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,94 +32,94 @@
                 methods.authorisations.GetDCs())
 
         return self._client._dcs
 
     async def close(self):
         await self._connection.close()
 
-    async def upload_file(self, file,
-                          mime: str = None, file_name: str = None,
-                          chunk: int = 131072, callback=None, *args, **kwargs):
+    async def upload_file(self, file, mime: str = None, file_name: str = None,
+                     chunk: int = 131072, callback=None, *args, **kwargs):
         if isinstance(file, str):
             if not os.path.exists(file):
                 raise ValueError('file not found in the given path')
             if file_name is None:
                 file_name = os.path.basename(file)
 
             async with aiofiles.open(file, 'rb') as f:
-                file = await file.read()
-                await f.close()
+                file_data = await f.read()
 
-        elif not isinstance(file, bytes):
+        elif isinstance(file, bytes):
+            file_data = file
+        else:
             raise TypeError('file arg value must be file path or bytes')
 
         if file_name is None:
             raise ValueError('the file_name is not set')
 
         if mime is None:
             mime = file_name.split('.')[-1]
 
         result = await self.execute(
             methods.messages.RequestSendFile(
-                mime=mime, size=len(file), file_name=file_name))
+                mime=mime, size=len(file_data), file_name=file_name))
 
-        id = result.id
+        file_id = result.id
         index = 0
         dc_id = result.dc_id
-        total = int(len(file) / chunk + 1)
+        total = int(len(file_data) / chunk + 1)
         upload_url = result.upload_url
         access_hash_send = result.access_hash_send
 
         while index < total:
-            data = file[index * chunk: index * chunk + chunk]
+            data = file_data[index * chunk: index * chunk + chunk]
             try:
-                result = await self._connection.post(
+                upload_result = await self._connection.post(
                     upload_url,
                     headers={
                         'auth': self._client._auth,
-                        'file-id': id,
+                        'file-id': file_id,
                         'total-part': str(total),
                         'part-number': str(index + 1),
                         'chunk-size': str(len(data)),
                         'access-hash-send': access_hash_send,
                         'User-Agent': self._client._user_agent
                     },
                     data=data
                 )
-                result = await result.json()
+                upload_result = await upload_result.json()
                 if callable(callback):
                     try:
-                        await callback(len(file), index * chunk)
+                        await callback(len(file_data), index * chunk)
 
                     except exceptions.CancelledError:
                         return None
 
                     except Exception:
                         pass
 
                 index += 1
             except Exception:
-                pass
+                break
 
-        status = result['status']
-        status_det = result['status_det']
+        status = upload_result.get('status')
+        status_det = upload_result.get('status_det')
         if status == 'OK' and status_det == 'OK':
             result = {
                 'mime': mime,
-                'size': len(file),
+                'size': len(file_data),
                 'dc_id': dc_id,
-                'file_id': id,
+                'file_id': file_id,
                 'file_name': file_name,
-                'access_hash_rec': result['data']['access_hash_rec']
+                'access_hash_rec': upload_result['data']['access_hash_rec']
             }
 
             return results('UploadFile', result)
 
-        self._client._logger.debug('upload failed', extra={'data': result})
-        raise exceptions(status_det)(result, request=result)
+        self._client._logger.debug('upload failed', extra={'data': upload_result})
+        raise exceptions(status_det)(upload_result, request=upload_result)
 
     async def execute(self, request: dict):
         if not isinstance(request, dict):
             request = request()
 
         self._client._logger.info('execute method', extra={'data': request})
         method_urls = request.pop('urls')
@@ -190,25 +190,43 @@
 
                 except aiohttp.ServerTimeoutError:
                     pass
 
         raise exceptions.InternalProblem(
             'rubika server has an internal problem', request=request)
 
-    async def download(self, dc_id, file_id,
-                       access_hash, chunk=131072, callback=None):
-        url = (await self._dcs()).storages[str(dc_id)]
+    async def download(self, dc_id: int, file_id: int, access_hash: str, size: int, chunk=131072, callback=None) -> bytes:
+        result = bytearray()
+        url = f'https://messenger{dc_id}.iranlms.ir/GetFile.ashx'
+
         headers = {
-            'file-id': str(file_id),
             'auth': self._client._auth,
-            'access-hash-rec': access_hash,
-            'User-Agent': self._client._user_agent}
-        async with aiohttp.ClientSession() as connection:
-            async with connection.post(url, headers=headers) as result:
-                return await result.read()
+            'file-id': str(file_id),
+            'start-index': '0',
+            'last-index': str(size),
+            'access-hash-rec': access_hash
+        }
+
+        async with aiohttp.ClientSession() as session:
+            if size <= chunk:
+                response = await session.post(url=url, headers=headers)
+                result.extend(await response.read())
+                if callback:
+                    await callback(size, len(result))
+            else:
+                for i in range(0, size, chunk):
+                    headers['start-index'] = str(i)
+                    headers['last-index'] = str(min(i + chunk, size))
+
+                    response = await session.post(url, headers=headers)
+                    result.extend(await response.read())
+                    if callback:
+                        await callback(size, len(result))
+
+        return bytes(result)
 
     async def handel_update(self, name, update):
         handlers = self._client._handlers.copy()
         for func, handler in handlers.items():
             try:
                 # if handler is empty filters
                 if isinstance(handler, type):
```

### Comparing `rubpy-6.2.6/rubpy/network/proxies.py` & `rubpy-6.2.7/rubpy/network/proxies.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.6/rubpy/sessions/sqliteSession.py` & `rubpy-6.2.7/rubpy/sessions/sqliteSession.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.6/rubpy/sessions/stringSession.py` & `rubpy-6.2.7/rubpy/sessions/stringSession.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.6/rubpy/structs/handlers.py` & `rubpy-6.2.7/rubpy/structs/handlers.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.6/rubpy/structs/models.py` & `rubpy-6.2.7/rubpy/structs/models.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.6/rubpy/structs/results.py` & `rubpy-6.2.7/rubpy/structs/results.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.6/rubpy/structs/struct.py` & `rubpy-6.2.7/rubpy/structs/struct.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.6/rubpy.egg-info/PKG-INFO` & `rubpy-6.2.7/rubpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubpy
-Version: 6.2.6
+Version: 6.2.7
 Summary: This is an unofficial library and fastest library for deploying robots on Rubika accounts.
 Home-page: https://github.com/shayanheidari01/rubika
 Author: Shayan Heidari
 Author-email: contact@shayanheidari.info
 Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rubpy Version: 6.2.6 Summary: This is an unofficial
+Metadata-Version: 2.1 Name: rubpy Version: 6.2.7 Summary: This is an unofficial
 library and fastest library for deploying robots on Rubika accounts. Home-page:
 https://github.com/shayanheidari01/rubika Author: Shayan Heidari Author-email:
 contact@shayanheidari.info Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `rubpy-6.2.6/rubpy.egg-info/SOURCES.txt` & `rubpy-6.2.7/rubpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.6/setup.py` & `rubpy-6.2.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requirements = ['aiohttp', 'pycryptodome', 'aiofiles']
 
 with open("README.md", encoding="UTF-8") as f:
     readme = f.read()
 
 setup(
     name = 'rubpy',
-    version = '6.2.6',
+    version = '6.2.7',
     author='Shayan Heidari',
     author_email = 'contact@shayanheidari.info',
     description = 'This is an unofficial library and fastest library for deploying robots on Rubika accounts.',
     keywords = ['rubika', 'rubpy', 'chat', 'bot', 'robot', 'asyncio'],
     long_description = readme,
     python_requires="~=3.7",
     long_description_content_type = 'text/markdown',
```

