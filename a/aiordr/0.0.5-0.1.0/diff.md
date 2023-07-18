# Comparing `tmp/aiordr-0.0.5.tar.gz` & `tmp/aiordr-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiordr-0.0.5.tar", max compression
+gzip compressed data, was "aiordr-0.1.0.tar", max compression
```

## Comparing `aiordr-0.0.5.tar` & `aiordr-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    35149 2023-03-05 15:00:19.703209 aiordr-0.0.5/LICENSE
--rw-r--r--   0        0        0     3313 2023-03-05 15:00:19.703209 aiordr-0.0.5/README.rst
--rw-r--r--   0        0        0      594 2023-03-05 15:00:19.703209 aiordr-0.0.5/aiordr/__init__.py
--rw-r--r--   0        0        0    14239 2023-03-05 15:00:19.703209 aiordr-0.0.5/aiordr/client.py
--rw-r--r--   0        0        0      813 2023-03-05 15:00:19.703209 aiordr-0.0.5/aiordr/exceptions.py
--rw-r--r--   0        0        0     1790 2023-03-05 15:00:19.703209 aiordr-0.0.5/aiordr/helpers.py
--rw-r--r--   0        0        0      226 2023-03-05 15:00:19.703209 aiordr-0.0.5/aiordr/models/__init__.py
--rw-r--r--   0        0        0      760 2023-03-05 15:00:19.703209 aiordr-0.0.5/aiordr/models/base.py
--rw-r--r--   0        0        0     1135 2023-03-05 15:00:19.703209 aiordr-0.0.5/aiordr/models/errorcode.py
--rw-r--r--   0        0        0      975 2023-03-05 15:00:19.703209 aiordr-0.0.5/aiordr/models/events.py
--rw-r--r--   0        0        0     5303 2023-03-05 15:00:19.703209 aiordr-0.0.5/aiordr/models/render.py
--rw-r--r--   0        0        0     1338 2023-03-05 15:00:19.703209 aiordr-0.0.5/aiordr/models/renderserver.py
--rw-r--r--   0        0        0     1038 2023-03-05 15:00:19.703209 aiordr-0.0.5/aiordr/models/skin.py
--rw-r--r--   0        0        0        0 2023-03-05 15:00:19.707209 aiordr-0.0.5/py.typed
--rw-r--r--   0        0        0     1875 2023-03-05 15:00:19.707209 aiordr-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     4890 1970-01-01 00:00:00.000000 aiordr-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-18 23:35:17.828672 aiordr-0.1.0/LICENSE
+-rw-r--r--   0        0        0     3313 2023-07-18 23:35:17.828672 aiordr-0.1.0/README.rst
+-rw-r--r--   0        0        0      594 2023-07-18 23:35:17.828672 aiordr-0.1.0/aiordr/__init__.py
+-rw-r--r--   0        0        0    14400 2023-07-18 23:35:17.828672 aiordr-0.1.0/aiordr/client.py
+-rw-r--r--   0        0        0      813 2023-07-18 23:35:17.828672 aiordr-0.1.0/aiordr/exceptions.py
+-rw-r--r--   0        0        0     1790 2023-07-18 23:35:17.828672 aiordr-0.1.0/aiordr/helpers.py
+-rw-r--r--   0        0        0      226 2023-07-18 23:35:17.828672 aiordr-0.1.0/aiordr/models/__init__.py
+-rw-r--r--   0        0        0      784 2023-07-18 23:35:17.828672 aiordr-0.1.0/aiordr/models/base.py
+-rw-r--r--   0        0        0     1135 2023-07-18 23:35:17.828672 aiordr-0.1.0/aiordr/models/errorcode.py
+-rw-r--r--   0        0        0      975 2023-07-18 23:35:17.828672 aiordr-0.1.0/aiordr/models/events.py
+-rw-r--r--   0        0        0     5303 2023-07-18 23:35:17.828672 aiordr-0.1.0/aiordr/models/render.py
+-rw-r--r--   0        0        0     1338 2023-07-18 23:35:17.828672 aiordr-0.1.0/aiordr/models/renderserver.py
+-rw-r--r--   0        0        0     1038 2023-07-18 23:35:17.832672 aiordr-0.1.0/aiordr/models/skin.py
+-rw-r--r--   0        0        0        0 2023-07-18 23:35:17.832672 aiordr-0.1.0/py.typed
+-rw-r--r--   0        0        0     1868 2023-07-18 23:35:17.832672 aiordr-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4884 1970-01-01 00:00:00.000000 aiordr-0.1.0/PKG-INFO
```

### Comparing `aiordr-0.0.5/LICENSE` & `aiordr-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiordr-0.0.5/README.rst` & `aiordr-0.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `aiordr-0.0.5/aiordr/__init__.py` & `aiordr-0.1.0/aiordr/__init__.py`

 * *Files identical despite different names*

### Comparing `aiordr-0.0.5/aiordr/client.py` & `aiordr-0.1.0/aiordr/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -107,54 +107,54 @@
         r"""Returns a callable that is called when a render is added, to be used as:
         @client.on_render_added()
         async def render_added(event: RenderAddEvent):
         """
 
         @functools.wraps(func)
         async def wrapper(data: dict) -> Any:
-            return await func(RenderAddEvent.parse_obj(data))
+            return await func(RenderAddEvent.model_validate(data))
 
         self.socket.on("render_added_json", wrapper)
         return wrapper
 
     def on_render_progress(self, func: Callable) -> Callable:
         r"""Returns a callable that is called when a render is updated, to be used as:
         @client.on_render_progress()
         async def render_progress(event: RenderProgressEvent):
         """
 
         @functools.wraps(func)
         async def wrapper(data: dict) -> Any:
-            return await func(RenderProgressEvent.parse_obj(data))
+            return await func(RenderProgressEvent.model_validate(data))
 
         self.socket.on("render_progress_json", wrapper)
         return wrapper
 
     def on_render_fail(self, func: Callable) -> Callable:
         r"""Returns a callable that is called when a render fails, to be used as:
         @client.on_render_fail()
         async def render_fail(event: RenderFailEvent):
         """
 
         @functools.wraps(func)
         async def wrapper(data: dict) -> Any:
-            return await func(RenderFailEvent.parse_obj(data))
+            return await func(RenderFailEvent.model_validate(data))
 
         self.socket.on("render_fail_json", wrapper)
         return wrapper
 
     def on_render_finish(self, func: Callable) -> Callable:
         r"""Returns a callable that is called when a render finishes, to be used as:
         @client.on_render_finish()
         async def render_finish(event: RenderFinishEvent):
         """
 
         @functools.wraps(func)
         async def wrapper(data: dict) -> Any:
-            return await func(RenderFinishEvent.parse_obj(data))
+            return await func(RenderFinishEvent.model_validate(data))
 
         self.socket.on("render_done_json", wrapper)
         return wrapper
 
     async def __aenter__(self) -> ordrClient:
         self._session = aiohttp.ClientSession()
         await self.connect()
@@ -165,15 +165,18 @@
         exc_type: Optional[Type[BaseException]],
         exc: Optional[BaseException],
         traceback: Optional[TracebackType],
     ) -> None:
         await self.close()
 
     async def _request(
-        self, request_type: ClientRequestType, *args: Any, **kwargs: Any
+        self,
+        request_type: ClientRequestType,
+        *args: Any,
+        **kwargs: Any,
     ) -> Any:
         if not self.socket.connected:
             await self.connect()
         if self._session is None:
             self._session = aiohttp.ClientSession()
 
         req: dict[str, Callable] = {
@@ -213,18 +216,21 @@
         """
         params = {"id": skin_id}
         json = await self._request(
             "GET",
             f"{self._base_url}/ordr/skins/custom",
             params=params,
         )
-        return SkinCompact.parse_obj(json)
+        return SkinCompact.model_validate(json)
 
     async def get_skins(
-        self, page: int = 1, page_size: int = 5, **kwargs: Any
+        self,
+        page: int = 1,
+        page_size: int = 5,
+        **kwargs: Any,
     ) -> SkinsResponse:
         r"""Get custom skins.
 
         :param page: Page number
         :type page: ``int``
         :param page_size: Page size
         :type page_size: ``int``
@@ -245,18 +251,21 @@
         }
         add_param(params, kwargs, "search")
         json = await self._request(
             "GET",
             f"{self._base_url}/ordr/skins",
             params=params,
         )
-        return SkinsResponse.parse_obj(json)
+        return SkinsResponse.model_validate(json)
 
     async def get_render_list(
-        self, page: int = 1, page_size: int = 5, **kwargs: Any
+        self,
+        page: int = 1,
+        page_size: int = 5,
+        **kwargs: Any,
     ) -> RendersResponse:
         r"""Get render list.
 
         :param page: Page number
         :type page: ``int``
         :param page_size: Page size
         :type page_size: ``int``
@@ -291,49 +300,52 @@
         add_param(params, kwargs, "no_bots", "nobots")
         add_param(params, kwargs, "link")
         add_param(params, kwargs, "beatmapset_id", "beatmapsetid")
         json = await self._request(
             "GET",
             f"{self._base_url}/ordr/renders",
         )
-        return RendersResponse.parse_obj(json)
+        return RendersResponse.model_validate(json)
 
     async def get_server_list(self) -> list[RenderServer]:
         r"""Get the list of available servers.
 
 
         :raises: ``aiordr.exceptions.APIException``: Contains status code, error message, and error code
         :return: List of servers
         :rtype: ``list[aiordr.models.server.RenderServer]``
         """
         json = await self._request(
             "GET",
-            f"{self._base_url}/servers",
+            f"{self._base_url}/ordr/servers",
         )
-        return from_list(RenderServer.parse_obj, json.get("servers", []))
+        return from_list(RenderServer.model_validate, json.get("servers", []))
 
     async def get_server_online_count(self) -> int:
         r"""Get the number of online servers.
 
 
         :raises: ``aiordr.exceptions.APIException``: Contains status code, error message, and error code
         :return: Number of online servers
         :rtype: ``int``
         """
         data = await self._request(
             "GET",
-            f"{self._base_url}/servers/onlinecount",
+            f"{self._base_url}/ordr/servers/onlinecount",
         )
         try:
             return int(data)
         except ValueError:
             return 0
 
     async def create_render(
-        self, username: str, skin: Union[str, int], **kwargs: Any
+        self,
+        username: str,
+        skin: Union[str, int],
+        **kwargs: Any,
     ) -> RenderCreateResponse:
         r"""Create a render.
 
         :param username: Username of the user who ordered the render
         :type username: ``str``
         :param skin: Skin ID or name
         :type skin: ``Union[str, int]``
@@ -368,15 +380,15 @@
 
         if "render_options" not in kwargs:
             kwargs["render_options"] = RenderOptions()
         options: RenderOptions = kwargs["render_options"]
         if not isinstance(options, RenderOptions):
             raise TypeError("render_options must be a RenderOptions object")
 
-        data.update(options.dict(exclude_defaults=True, by_alias=True))
+        data.update(options.model_dump(exclude_defaults=True, by_alias=True))
         data["resolution"] = options.resolution.value
 
         add_param(data, kwargs, "replay_url", "replayURL")
         add_param(data, kwargs, "custom_skin", "customSkin")
 
         form_data = aiohttp.FormData()
         for key, value in data.items():
@@ -392,15 +404,15 @@
             )
 
         json = await self._request(
             "POST",
             f"{self._base_url}/ordr/renders",
             data=form_data,
         )
-        return RenderCreateResponse.parse_obj(json)
+        return RenderCreateResponse.model_validate(json)
 
     async def connect(self) -> None:
         r"""Connects to the websocket server.
 
         :return: None
         """
         await self.socket.connect(url=self._websocket_url)
```

### Comparing `aiordr-0.0.5/aiordr/exceptions.py` & `aiordr-0.1.0/aiordr/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiordr-0.0.5/aiordr/helpers.py` & `aiordr-0.1.0/aiordr/helpers.py`

 * *Files identical despite different names*

### Comparing `aiordr-0.0.5/aiordr/models/errorcode.py` & `aiordr-0.1.0/aiordr/models/errorcode.py`

 * *Files identical despite different names*

### Comparing `aiordr-0.0.5/aiordr/models/events.py` & `aiordr-0.1.0/aiordr/models/events.py`

 * *Files identical despite different names*

### Comparing `aiordr-0.0.5/aiordr/models/render.py` & `aiordr-0.1.0/aiordr/models/render.py`

 * *Files identical despite different names*

### Comparing `aiordr-0.0.5/aiordr/models/renderserver.py` & `aiordr-0.1.0/aiordr/models/renderserver.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     "RenderServerOptions",
     "RenderServer",
 )
 
 
 class RenderServerOptions(BaseModel):
     text_color: str = Field(alias="textColor")
-    background_type: str = Field(alias="backgroundType")
+    background_type: int = Field(alias="backgroundType")
 
 
 class RenderServer(BaseModel):
     enabled: bool
     last_seen: datetime = Field(alias="lastSeen")
     name: str
     priority: float
```

### Comparing `aiordr-0.0.5/aiordr/models/skin.py` & `aiordr-0.1.0/aiordr/models/skin.py`

 * *Files identical despite different names*

### Comparing `aiordr-0.0.5/pyproject.toml` & `aiordr-0.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 show_error_codes = true
 
 [tools.pytest.ini_options]
 testpaths = ["tests"]
 
 [tool.poetry]
 name = "aiordr"
-version = "0.0.5"
+version = "0.1.0"
 description = "Simple and fast library for interacting with the o!rdr API."
 authors = ["Nice Aesthetics <nice@aesth.dev>"]
 license = "GPLv3+"
 readme = "README.rst"
 repository = "https://github.com/NiceAesth/aiordr"
 documentation = "https://aiordr.readthedocs.io/"
 keywords = ["osu!", "osu", "api"]
@@ -30,36 +30,37 @@
 include = ["py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 aiohttp = "^3.8.3"
 aiolimiter = "^1.0.0"
 orjson = "^3.8.3"
-pydantic = "^1.10.2"
+pydantic = "^2.0.3"
 pytest = {version="^7.2.0", optional = true}
-pytest-asyncio = {version="^0.20.2", optional = true}
+pytest-asyncio = {version="^0.21.0", optional = true}
 pytest-mock = {version="^3.10.0", optional = true}
 toml = {version="^0.10.2", optional = true}
-sphinx = {version="^6.0.0", optional = true}
-sphinx-rtd-theme = {version="^1.1.1", optional = true}
+sphinx = {version="^7.0.0", optional = true}
+furo = {version="^2023.5.20", optional = true}
 types-toml = {version = "^0.10.8.1", optional = true}
 python-socketio = {extras = ["asyncio-client"], version = "^5.7.2"}
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
-pytest-asyncio = "^0.20.2"
+pytest-asyncio = "^0.21.0"
 pytest-mock = "^3.10.0"
 mypy = "^1.0"
 toml = "^0.10.2"
 types-toml = "^0.10.8.1"
-sphinx = "^6.0.0"
-sphinx-rtd-theme = "^1.2.0"
+sphinx = "^7.0.0"
+furo = "^2023.5.20"
 pytest-cov = "^4.0.0"
 black = {version = "^23.0.0", allow-prereleases = true}
+pre-commit = "^3.2.2"
 
 [tool.poetry.extras]
 test = ["pytest", "pytest-asyncio", "pytest-mock", "toml", "types-toml"]
-docs = ["Sphinx", "sphinx-rtd-theme", "toml"]
+docs = ["Sphinx", "furo", "toml"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `aiordr-0.0.5/PKG-INFO` & `aiordr-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiordr
-Version: 0.0.5
+Version: 0.1.0
 Summary: Simple and fast library for interacting with the o!rdr API.
 Home-page: https://github.com/NiceAesth/aiordr
 License: GPLv3+
 Keywords: osu!,osu,api
 Author: Nice Aesthetics
 Author-email: nice@aesth.dev
 Requires-Python: >=3.9,<4.0
@@ -16,22 +16,22 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Provides-Extra: docs
 Provides-Extra: test
 Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
 Requires-Dist: aiolimiter (>=1.0.0,<2.0.0)
+Requires-Dist: furo (>=2023.5.20,<2024.0.0) ; extra == "docs"
 Requires-Dist: orjson (>=3.8.3,<4.0.0)
-Requires-Dist: pydantic (>=1.10.2,<2.0.0)
+Requires-Dist: pydantic (>=2.0.3,<3.0.0)
 Requires-Dist: pytest (>=7.2.0,<8.0.0) ; extra == "test"
-Requires-Dist: pytest-asyncio (>=0.20.2,<0.21.0) ; extra == "test"
+Requires-Dist: pytest-asyncio (>=0.21.0,<0.22.0) ; extra == "test"
 Requires-Dist: pytest-mock (>=3.10.0,<4.0.0) ; extra == "test"
 Requires-Dist: python-socketio[asyncio-client] (>=5.7.2,<6.0.0)
-Requires-Dist: sphinx (>=6.0.0,<7.0.0) ; extra == "docs"
-Requires-Dist: sphinx-rtd-theme (>=1.1.1,<2.0.0) ; extra == "docs"
+Requires-Dist: sphinx (>=7.0.0,<8.0.0) ; extra == "docs"
 Requires-Dist: toml (>=0.10.2,<0.11.0) ; extra == "test" or extra == "docs"
 Requires-Dist: types-toml (>=0.10.8.1,<0.11.0.0) ; extra == "test"
 Project-URL: Documentation, https://aiordr.readthedocs.io/
 Project-URL: Repository, https://github.com/NiceAesth/aiordr
 Description-Content-Type: text/x-rst
 
 aiordr
```

