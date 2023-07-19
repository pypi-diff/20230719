# Comparing `tmp/aify-0.1.2-py3-none-any.whl.zip` & `tmp/aify-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,28 +1,31 @@
-Zip file size: 1368391 bytes, number of entries: 26
--rw-r--r--  2.0 unx       49 b- defN 23-Jul-19 02:27 aify/__init__.py
+Zip file size: 1370569 bytes, number of entries: 29
+-rw-r--r--  2.0 unx       49 b- defN 23-Jul-19 08:31 aify/__init__.py
 -rw-r--r--  2.0 unx     3129 b- defN 23-Jul-19 02:14 aify/__main__.py
--rw-r--r--  2.0 unx     5630 b- defN 23-Jul-19 02:10 aify/_entry.py
+-rw-r--r--  2.0 unx     2411 b- defN 23-Jul-19 06:58 aify/_auth.py
+-rw-r--r--  2.0 unx     6680 b- defN 23-Jul-19 07:10 aify/_entry.py
 -rw-r--r--  2.0 unx      415 b- defN 23-Jul-19 02:13 aify/_env.py
 -rw-r--r--  2.0 unx       37 b- defN 23-Jul-19 02:15 aify/_error.py
 -rw-r--r--  2.0 unx       51 b- defN 23-Jul-19 02:15 aify/_logging.py
 -rw-r--r--  2.0 unx     4905 b- defN 23-Jul-19 02:18 aify/_program.py
 -rw-r--r--  2.0 unx      439 b- defN 23-Jul-19 02:19 aify/_web_template.py
 -rw-r--r--  2.0 unx     1422 b- defN 23-Jul-19 02:25 aify/embeddings.py
 -rw-r--r--  2.0 unx      322 b- defN 23-Jul-19 02:21 aify/embeddings_openai.py
 -rw-r--r--  2.0 unx     2036 b- defN 23-Jul-19 02:11 aify/memory.py
--rwxr-xr-x  2.0 unx       36 b- defN 23-Jul-18 04:20 aify-0.1.2.data/scripts/aify
--rwxr-xr-x  2.0 unx       95 b- defN 23-Jul-18 06:08 aify-0.1.2.data/scripts/requirements.txt
--rwxr-xr-x  2.0 unx     1351 b- defN 23-Jul-18 07:03 aify-0.1.2.data/scripts/setup.py
+-rwxr-xr-x  2.0 unx       36 b- defN 23-Jul-18 04:20 aify-0.1.3.data/scripts/aify
+-rwxr-xr-x  2.0 unx      112 b- defN 23-Jul-19 06:50 aify-0.1.3.data/scripts/requirements.txt
+-rwxr-xr-x  2.0 unx     1351 b- defN 23-Jul-18 07:03 aify-0.1.3.data/scripts/setup.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-18 03:44 webui/__init__.py
--rw-r--r--  2.0 unx   241104 b- defN 23-Jul-19 02:27 webui/static/aify/aify.css
--rw-r--r--  2.0 unx   656493 b- defN 23-Jul-19 02:27 webui/static/aify/aify.css.map
--rw-r--r--  2.0 unx   866549 b- defN 23-Jul-19 02:27 webui/static/aify/aify.js
--rw-r--r--  2.0 unx     1852 b- defN 23-Jul-19 02:27 webui/static/aify/aify.js.LICENSE.txt
--rw-r--r--  2.0 unx  3610429 b- defN 23-Jul-19 02:27 webui/static/aify/aify.js.map
--rw-r--r--  2.0 unx      692 b- defN 23-Jul-19 02:09 webui/templates/index.html
--rw-r--r--  2.0 unx     1071 b- defN 23-Jul-19 02:27 aify-0.1.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     5789 b- defN 23-Jul-19 02:27 aify-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-19 02:27 aify-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jul-19 02:27 aify-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2032 b- defN 23-Jul-19 02:27 aify-0.1.2.dist-info/RECORD
-26 files, 5406031 bytes uncompressed, 1365161 bytes compressed:  74.7%
+-rw-r--r--  2.0 unx   241104 b- defN 23-Jul-19 08:31 webui/static/aify/aify.css
+-rw-r--r--  2.0 unx   656493 b- defN 23-Jul-19 08:31 webui/static/aify/aify.css.map
+-rw-r--r--  2.0 unx   866549 b- defN 23-Jul-19 08:31 webui/static/aify/aify.js
+-rw-r--r--  2.0 unx     1852 b- defN 23-Jul-19 08:31 webui/static/aify/aify.js.LICENSE.txt
+-rw-r--r--  2.0 unx  3610429 b- defN 23-Jul-19 08:31 webui/static/aify/aify.js.map
+-rw-r--r--  2.0 unx      559 b- defN 23-Jul-19 06:52 webui/templates/auth.html
+-rw-r--r--  2.0 unx      543 b- defN 23-Jul-19 06:23 webui/templates/basic.html
+-rw-r--r--  2.0 unx      665 b- defN 23-Jul-19 06:09 webui/templates/index.html
+-rw-r--r--  2.0 unx     1071 b- defN 23-Jul-19 08:31 aify-0.1.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5821 b- defN 23-Jul-19 08:31 aify-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-19 08:31 aify-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jul-19 08:31 aify-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2266 b- defN 23-Jul-19 08:31 aify-0.1.3.dist-info/RECORD
+29 files, 5410850 bytes uncompressed, 1366983 bytes compressed:  74.7%
```

## zipnote {}

```diff
@@ -1,13 +1,16 @@
 Filename: aify/__init__.py
 Comment: 
 
 Filename: aify/__main__.py
 Comment: 
 
+Filename: aify/_auth.py
+Comment: 
+
 Filename: aify/_entry.py
 Comment: 
 
 Filename: aify/_env.py
 Comment: 
 
 Filename: aify/_error.py
@@ -27,21 +30,21 @@
 
 Filename: aify/embeddings_openai.py
 Comment: 
 
 Filename: aify/memory.py
 Comment: 
 
-Filename: aify-0.1.2.data/scripts/aify
+Filename: aify-0.1.3.data/scripts/aify
 Comment: 
 
-Filename: aify-0.1.2.data/scripts/requirements.txt
+Filename: aify-0.1.3.data/scripts/requirements.txt
 Comment: 
 
-Filename: aify-0.1.2.data/scripts/setup.py
+Filename: aify-0.1.3.data/scripts/setup.py
 Comment: 
 
 Filename: webui/__init__.py
 Comment: 
 
 Filename: webui/static/aify/aify.css
 Comment: 
@@ -54,26 +57,32 @@
 
 Filename: webui/static/aify/aify.js.LICENSE.txt
 Comment: 
 
 Filename: webui/static/aify/aify.js.map
 Comment: 
 
+Filename: webui/templates/auth.html
+Comment: 
+
+Filename: webui/templates/basic.html
+Comment: 
+
 Filename: webui/templates/index.html
 Comment: 
 
-Filename: aify-0.1.2.dist-info/LICENSE
+Filename: aify-0.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: aify-0.1.2.dist-info/METADATA
+Filename: aify-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: aify-0.1.2.dist-info/WHEEL
+Filename: aify-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: aify-0.1.2.dist-info/top_level.txt
+Filename: aify-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: aify-0.1.2.dist-info/RECORD
+Filename: aify-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aify/__init__.py

```diff
@@ -1,3 +1,3 @@
-__version__ = '0.1.2'
+__version__ = '0.1.3'
 
 from ._entry import entry
```

## aify/_entry.py

```diff
@@ -1,19 +1,22 @@
 import os
 import json
 import contextlib
 from starlette.applications import Starlette
 from starlette.routing import Mount, Route
 from starlette.staticfiles import StaticFiles
-from starlette.responses import JSONResponse, StreamingResponse
+from starlette.responses import JSONResponse, StreamingResponse, RedirectResponse
+from starlette.middleware import Middleware
+from starlette.middleware.authentication import AuthenticationMiddleware
+from starlette.authentication import requires
 from starlette.exceptions import HTTPException
 from fastapi import FastAPI, Request
 from . import _env
 from . import _program
-from . import memory
+from . import _auth
 from ._logging import logger
 from ._web_template import render
 
 # FastAPI
 api = FastAPI()
 
 def get_program(name: str) -> _program.Program:
@@ -30,14 +33,15 @@
     except Exception as e:
         logger.error(e, exc_info=e)
         raise HTTPException(
             status_code=404, detail=f"Not a valid app: {e}")
     return program
 
 @api.put('/apps/{name}/{session_id}')
+@requires(['authenticated', 'write'])
 async def execute_program(request: Request, name: str, session_id: str):
     """Execute the program identified by the name."""
     program = get_program(name)
     
     kwargs = {}
     try:
         kwargs = await request.json()
@@ -103,26 +107,28 @@
         it = _aiter()
     except Exception as e:
         raise HTTPException(status_code=400, detail=f"Something wrong: {e}")
 
     return StreamingResponse(it, headers={'Content-Type': content_type})
 
 @api.get('/apps/{name}/{session_id}/memories')
+@requires(['authenticated'])
 async def get_memories(request: Request, name: str, session_id: str, limit=1000):
     """Get the memory content of the specified application's current session."""
     memories = []
     program = get_program(name)
     memory = program.modules.get('memory')
     if memory:
         m = memory.read(name, session_id, max_len=2040*1024, n=limit)
         if m:
             memories = m
     return JSONResponse(memories)
 
 @api.get('/apps')
+@requires(['authenticated'])
 async def list_apps(request: Request):
     """List applications"""
     progs = []
     if len(_program.programs) == 0:
         _program.reload()
 
     for name, prog in _program.programs.items():
@@ -132,14 +138,15 @@
             'description': prog.template.get('description'),
             'icon_emoji': prog.template.get('icon_emoji'),
         })
     
     return JSONResponse(progs)
 
 @api.get('/sessions')
+@requires(['authenticated'])
 async def list_sessions(request: Request):
     """List sessions"""
     
     sessions = []
 
     progs = []
     if len(_program.programs) == 0:
@@ -149,14 +156,27 @@
         memory = prog.modules.get('memory')
         sessions.extend(memory.sessions(name))
 
     sessions = sorted(sessions, key=lambda x: x.get('last_modified'), reverse=True)
 
     return JSONResponse(sessions)
 
+async def auth(request: Request):
+    response = await render('auth.html')(request=request)
+    if request.method == 'POST':
+        next = request.query_params.get('next')
+        print(next)
+        if next:
+            response = RedirectResponse(next, status_code=302)
+        
+        async with request.form() as form:
+            token = form.get('token')
+            response.set_cookie('token', token, max_age=7*24*3600)
+    return response
+
 # Routes
 routes = [
     Mount(
         '/api',
         name='api',
         app=api
     ),
@@ -164,24 +184,35 @@
         '/static',
         name='static',
         app=StaticFiles(directory=os.path.join(_env.webui_dir(), 'static'), check_dir=False),
     ),
     Route(
         '/',
         name='home',
-        endpoint=render('index.html')
+        endpoint=requires(scopes=['authenticated'], redirect='auth')(render('index.html'))
+    ),
+    Route(
+        '/auth',
+        name='auth',
+        methods=['POST', 'GET'],
+        endpoint=auth
     )
 ]
 
 apps_static_dir = os.path.join(_env.apps_dir(), 'static')
 if os.path.exists(apps_static_dir):
     routes.append(Mount(
         '/apps/static',
         name='apps_static',
         app=StaticFiles(directory=apps_static_dir, check_dir=False),
     ))
 
+# Middlewares
+middleware = [
+    Middleware(AuthenticationMiddleware, backend=_auth.BasicAuthBackend())
+]
+
 @contextlib.asynccontextmanager
 async def lifespan(app):
     yield
 
-entry = Starlette(debug=True, routes=routes, lifespan=lifespan)
+entry = Starlette(debug=True, routes=routes, middleware=middleware, lifespan=lifespan)
```

## webui/templates/index.html

```diff
@@ -13,12 +13,11 @@
 
 <body>
     <noscript>You need to enable JavaScript to run this app.</noscript>
     <div id="root"></div>
 </body>
 <script defer>
     window.onload = function () {
-        console.log(aify);
         aify.create('root');
     }
 </script>
 </html>
```

## Comparing `aify-0.1.2.data/scripts/setup.py` & `aify-0.1.3.data/scripts/setup.py`

 * *Files identical despite different names*

## Comparing `aify-0.1.2.dist-info/LICENSE` & `aify-0.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `aify-0.1.2.dist-info/METADATA` & `aify-0.1.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aify
-Version: 0.1.2
+Version: 0.1.3
 Summary: aify is an AI-native application framework and runtime
 Home-page: https://github.com/shellc/aify
 Author-email: shenggong.wang@gmail.com
 Keywords: AI-Native,LLM,aify,chatbot
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: guidance
@@ -12,14 +12,15 @@
 Requires-Dist: openai
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: uvicorn
 Requires-Dist: starlette
 Requires-Dist: fastapi
 Requires-Dist: jinja2
+Requires-Dist: python-multipart
 Requires-Dist: python-dotenv
 Requires-Dist: watchfiles
 
 # 🚀 aify
 
 ### Build your AI-native application in seconds.
```

## Comparing `aify-0.1.2.dist-info/RECORD` & `aify-0.1.3.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,29 @@
-aify/__init__.py,sha256=AndgzZkhBAJh-t8vpNUPySURL_th41wDDNX6SsJTOUQ,49
+aify/__init__.py,sha256=WGsxxZY6QXHQ71F71yUZ5Kx0SauW_bmbGg33UmLwcaI,49
 aify/__main__.py,sha256=sp9Te15kUdkjA_z3jD5UFBz8n_LOvvVaRgVBWIJ9ZYE,3129
-aify/_entry.py,sha256=7rgTTyQt56vYrXFSoJMBC7sMXttL5KxWZUyn-bEQaHg,5630
+aify/_auth.py,sha256=56N-Fa3CnSI0k1chYKp3JcIbUqSQveLkE8pSUwSS8IA,2411
+aify/_entry.py,sha256=P70M_BKabSSM6AFRWBIP7pbACsItvX7mo8PlFHIaeYA,6680
 aify/_env.py,sha256=MsNbVndyOBQODho36aUkVr8FyBhvzdQGSl_w_NcJG3c,415
 aify/_error.py,sha256=VCA0ZV7ivQ0pGHxdFHLc5-KBxQtccnbML_b_nV01-9I,37
 aify/_logging.py,sha256=CtB4dWhVt76j0ype0ii7YmoBN9FcDZ4m0-DCqCSnVws,51
 aify/_program.py,sha256=gbWReyausB6X52eO54xQ4hzwYtv2uMQt9Qqkr-_k7j4,4905
 aify/_web_template.py,sha256=YHRgKN8bOM-b0qktG6OV2gLzxIUPZIPp_bj6nQWybrc,439
 aify/embeddings.py,sha256=vr-LkxblVKsqwwBbnOSpY7k_3y2fQ8OMWmVXPR4LoZo,1422
 aify/embeddings_openai.py,sha256=aGDGoYfv-F7DkI9pOJfCQOyTMdurxVCwJm6_AduSU0I,322
 aify/memory.py,sha256=aWApvK44UrP753iz_h8AuCbGdAJv7RUUvKcMQcydFIs,2036
-aify-0.1.2.data/scripts/aify,sha256=ocvEBE3luWtvoqhheCj039mK_5OnuJ5UgPDUX2boMck,36
-aify-0.1.2.data/scripts/requirements.txt,sha256=Nji-RAcec7gXlkH4uoxRQzwGkzoMw__sTEVQzTtl2R4,95
-aify-0.1.2.data/scripts/setup.py,sha256=lmsPrm7hdZNu25-NpZjzJSGe2QSg0NgMfrlaZQRGrNs,1351
+aify-0.1.3.data/scripts/aify,sha256=ocvEBE3luWtvoqhheCj039mK_5OnuJ5UgPDUX2boMck,36
+aify-0.1.3.data/scripts/requirements.txt,sha256=trxB65baEVvkOHViMA3TxYeyZPywANzlCq2Fgq2PL3o,112
+aify-0.1.3.data/scripts/setup.py,sha256=lmsPrm7hdZNu25-NpZjzJSGe2QSg0NgMfrlaZQRGrNs,1351
 webui/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 webui/static/aify/aify.css,sha256=RA0SEF4RG6GT4ethKNKxTg8OzIQD5bj7dyIA4yVyDMA,241104
 webui/static/aify/aify.css.map,sha256=o7IC2Lpkr4o9TxNhuXmDNKhs2MTCDu_CHpMI8baedhI,656493
 webui/static/aify/aify.js,sha256=EQwp80Cmk9ugeY-WqZKM-KDqrTABBxQ2JryhV4QEoqs,866549
 webui/static/aify/aify.js.LICENSE.txt,sha256=zNsFYopKdSoihu-yaqZFz6FfKE43eGeoLnRHd2IL41c,1852
 webui/static/aify/aify.js.map,sha256=jyC5dZlXJofwjObvFS8h3jLPGM_MgPPGB-IAtTMZ_zU,3610429
-webui/templates/index.html,sha256=5BhRxsPKJDqHU_PC7gXAATRxhcH1YO0tjfGu4CmauMg,692
-aify-0.1.2.dist-info/LICENSE,sha256=r-u8iAmSxCFjnZKeQcZnZF8KMi2Cs4cgGQMBxA2Hbwg,1071
-aify-0.1.2.dist-info/METADATA,sha256=xWO7X5PXj2cOQ4znyHvmyOwAP78X6wm38JEQw8IwWlg,5789
-aify-0.1.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-aify-0.1.2.dist-info/top_level.txt,sha256=P7ZAYFs-muF2wH0-BCCEU-jNq9bSQiaMUj9yqOX2hcQ,11
-aify-0.1.2.dist-info/RECORD,,
+webui/templates/auth.html,sha256=cndbRF4xry5Ng5MSWxjqGi8SQADlW_DrWDMh4BizUrc,559
+webui/templates/basic.html,sha256=G4Gzn1lvfG8pC4PSRTW38KgbgXQ3lbtqSaYc9MHctO8,543
+webui/templates/index.html,sha256=ARa99ojduQ5RoSZqoupv1wpvw1n-ZnzYqfikl6wW9Sc,665
+aify-0.1.3.dist-info/LICENSE,sha256=r-u8iAmSxCFjnZKeQcZnZF8KMi2Cs4cgGQMBxA2Hbwg,1071
+aify-0.1.3.dist-info/METADATA,sha256=V2o9UxwmSiF2cWDfhxvRrbYQMo0uT_65RSbixKl1ULs,5821
+aify-0.1.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+aify-0.1.3.dist-info/top_level.txt,sha256=P7ZAYFs-muF2wH0-BCCEU-jNq9bSQiaMUj9yqOX2hcQ,11
+aify-0.1.3.dist-info/RECORD,,
```

