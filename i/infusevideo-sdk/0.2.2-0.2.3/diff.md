# Comparing `tmp/infusevideo-sdk-0.2.2.tar.gz` & `tmp/infusevideo-sdk-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infusevideo-sdk-0.2.2.tar", last modified: Tue May 24 22:48:39 2022, max compression
+gzip compressed data, was "infusevideo-sdk-0.2.3.tar", last modified: Wed Jul 19 14:14:10 2023, max compression
```

## Comparing `infusevideo-sdk-0.2.2.tar` & `infusevideo-sdk-0.2.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 dataghost  (1000) dataghost  (1000)        0 2022-05-24 22:48:39.863213 infusevideo-sdk-0.2.2/
--rw-rw-r--   0 dataghost  (1000) dataghost  (1000)     1096 2022-03-03 13:50:03.000000 infusevideo-sdk-0.2.2/LICENSE
--rw-rw-r--   0 dataghost  (1000) dataghost  (1000)     3547 2022-05-24 22:48:39.863213 infusevideo-sdk-0.2.2/PKG-INFO
--rw-rw-r--   0 dataghost  (1000) dataghost  (1000)     2869 2022-05-10 11:40:23.000000 infusevideo-sdk-0.2.2/README.md
-drwxrwxr-x   0 dataghost  (1000) dataghost  (1000)        0 2022-05-24 22:48:39.863213 infusevideo-sdk-0.2.2/infusevideo/
--rw-rw-r--   0 dataghost  (1000) dataghost  (1000)     1641 2022-05-19 23:17:14.000000 infusevideo-sdk-0.2.2/infusevideo/__init__.py
--rw-rw-r--   0 dataghost  (1000) dataghost  (1000)     5462 2022-05-10 12:05:50.000000 infusevideo-sdk-0.2.2/infusevideo/auth.py
--rw-rw-r--   0 dataghost  (1000) dataghost  (1000)     1836 2022-03-09 23:16:52.000000 infusevideo-sdk-0.2.2/infusevideo/authserver.py
--rw-rw-r--   0 dataghost  (1000) dataghost  (1000)     3857 2022-05-24 21:54:41.000000 infusevideo-sdk-0.2.2/infusevideo/client.py
--rw-rw-r--   0 dataghost  (1000) dataghost  (1000)     5643 2022-04-20 15:32:28.000000 infusevideo-sdk-0.2.2/infusevideo/config.py
--rw-rw-r--   0 dataghost  (1000) dataghost  (1000)     2263 2022-05-19 23:23:07.000000 infusevideo-sdk-0.2.2/infusevideo/errors.py
--rw-rw-r--   0 dataghost  (1000) dataghost  (1000)      165 2022-04-06 11:32:16.000000 infusevideo-sdk-0.2.2/infusevideo/filterwarnings.py
--rw-rw-r--   0 dataghost  (1000) dataghost  (1000)     1045 2022-02-23 01:26:03.000000 infusevideo-sdk-0.2.2/infusevideo/scope.py
-drwxrwxr-x   0 dataghost  (1000) dataghost  (1000)        0 2022-05-24 22:48:39.863213 infusevideo-sdk-0.2.2/infusevideo_sdk.egg-info/
--rw-rw-r--   0 dataghost  (1000) dataghost  (1000)     3547 2022-05-24 22:48:39.000000 infusevideo-sdk-0.2.2/infusevideo_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 dataghost  (1000) dataghost  (1000)      423 2022-05-24 22:48:39.000000 infusevideo-sdk-0.2.2/infusevideo_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 dataghost  (1000) dataghost  (1000)        1 2022-05-24 22:48:39.000000 infusevideo-sdk-0.2.2/infusevideo_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 dataghost  (1000) dataghost  (1000)       33 2022-05-24 22:48:39.000000 infusevideo-sdk-0.2.2/infusevideo_sdk.egg-info/requires.txt
--rw-rw-r--   0 dataghost  (1000) dataghost  (1000)       12 2022-05-24 22:48:39.000000 infusevideo-sdk-0.2.2/infusevideo_sdk.egg-info/top_level.txt
--rw-rw-r--   0 dataghost  (1000) dataghost  (1000)       98 2022-03-03 23:16:34.000000 infusevideo-sdk-0.2.2/pyproject.toml
--rw-rw-r--   0 dataghost  (1000) dataghost  (1000)      788 2022-05-24 22:48:39.863213 infusevideo-sdk-0.2.2/setup.cfg
+drwxrwxr-x   0 dataghost  (1000) dataghost  (1000)        0 2023-07-19 14:14:10.307709 infusevideo-sdk-0.2.3/
+-rw-rw-r--   0 dataghost  (1000) dataghost  (1000)     1096 2022-03-03 13:50:03.000000 infusevideo-sdk-0.2.3/LICENSE
+-rw-rw-r--   0 dataghost  (1000) dataghost  (1000)     3852 2023-07-19 14:14:10.307709 infusevideo-sdk-0.2.3/PKG-INFO
+-rw-rw-r--   0 dataghost  (1000) dataghost  (1000)     3174 2023-07-19 14:10:42.000000 infusevideo-sdk-0.2.3/README.md
+drwxrwxr-x   0 dataghost  (1000) dataghost  (1000)        0 2023-07-19 14:14:10.307709 infusevideo-sdk-0.2.3/infusevideo/
+-rw-rw-r--   0 dataghost  (1000) dataghost  (1000)     1641 2022-06-30 16:01:38.000000 infusevideo-sdk-0.2.3/infusevideo/__init__.py
+-rw-rw-r--   0 dataghost  (1000) dataghost  (1000)     5550 2022-07-03 21:41:04.000000 infusevideo-sdk-0.2.3/infusevideo/auth.py
+-rw-rw-r--   0 dataghost  (1000) dataghost  (1000)     1836 2022-03-09 23:16:52.000000 infusevideo-sdk-0.2.3/infusevideo/authserver.py
+-rw-rw-r--   0 dataghost  (1000) dataghost  (1000)     4027 2023-07-19 14:10:42.000000 infusevideo-sdk-0.2.3/infusevideo/client.py
+-rw-rw-r--   0 dataghost  (1000) dataghost  (1000)     5651 2022-07-03 21:34:18.000000 infusevideo-sdk-0.2.3/infusevideo/config.py
+-rw-rw-r--   0 dataghost  (1000) dataghost  (1000)     2263 2022-05-19 23:23:07.000000 infusevideo-sdk-0.2.3/infusevideo/errors.py
+-rw-rw-r--   0 dataghost  (1000) dataghost  (1000)      165 2022-04-06 11:32:16.000000 infusevideo-sdk-0.2.3/infusevideo/filterwarnings.py
+-rw-rw-r--   0 dataghost  (1000) dataghost  (1000)     1309 2023-07-19 14:10:42.000000 infusevideo-sdk-0.2.3/infusevideo/scope.py
+drwxrwxr-x   0 dataghost  (1000) dataghost  (1000)        0 2023-07-19 14:14:10.307709 infusevideo-sdk-0.2.3/infusevideo_sdk.egg-info/
+-rw-rw-r--   0 dataghost  (1000) dataghost  (1000)     3852 2023-07-19 14:14:10.000000 infusevideo-sdk-0.2.3/infusevideo_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 dataghost  (1000) dataghost  (1000)      423 2023-07-19 14:14:10.000000 infusevideo-sdk-0.2.3/infusevideo_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 dataghost  (1000) dataghost  (1000)        1 2023-07-19 14:14:10.000000 infusevideo-sdk-0.2.3/infusevideo_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 dataghost  (1000) dataghost  (1000)       36 2023-07-19 14:14:10.000000 infusevideo-sdk-0.2.3/infusevideo_sdk.egg-info/requires.txt
+-rw-rw-r--   0 dataghost  (1000) dataghost  (1000)       12 2023-07-19 14:14:10.000000 infusevideo-sdk-0.2.3/infusevideo_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 dataghost  (1000) dataghost  (1000)       98 2022-03-03 23:16:34.000000 infusevideo-sdk-0.2.3/pyproject.toml
+-rw-rw-r--   0 dataghost  (1000) dataghost  (1000)      791 2023-07-19 14:14:10.307709 infusevideo-sdk-0.2.3/setup.cfg
```

### Comparing `infusevideo-sdk-0.2.2/LICENSE` & `infusevideo-sdk-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `infusevideo-sdk-0.2.2/PKG-INFO` & `infusevideo-sdk-0.2.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infusevideo-sdk
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python SDK for the Infuse Video API
 Home-page: https://www.infuse.video
 Author: Infuse Video
 Author-email: support@infuse.video
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -62,14 +62,26 @@
 
 	import infusevideo
 
 	api = infusevideo.InfuseVideo()
 	result = api.get("/media")
 	print(result)
 
+
+Create a new Media and upload a video file:
+
+	import infusevideo
+
+	api = infusevideo.InfuseVideo()
+	result = api.post("/media", data={"name": "A name", "metadata": "Example metadata"})
+	mediaId = result["mediaId"]
+	
+	result = api.put(f"/media/{mediaId}", fileName="/path/to/my/file.mp4")
+	print(result)
+
 #### Creating a sample configuration file
 By default, the SDK will connect to the API, ask for your credentials interactively, and
 attempt to obtain an authorization token with all permissions that were granted to you. If you have
 access to multiple accounts, the token will be valid only for your default account. In order to
 easily use multiple accounts, choose a different, limited, set of permissions or use non-interactive
 M2M authentication, you will need to customise a profile in the configuration file. This
 configuration file is normally located in the `.infusevideo/` directory in your home directory. If
```

### Comparing `infusevideo-sdk-0.2.2/README.md` & `infusevideo-sdk-0.2.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -42,14 +42,26 @@
 
 	import infusevideo
 
 	api = infusevideo.InfuseVideo()
 	result = api.get("/media")
 	print(result)
 
+
+Create a new Media and upload a video file:
+
+	import infusevideo
+
+	api = infusevideo.InfuseVideo()
+	result = api.post("/media", data={"name": "A name", "metadata": "Example metadata"})
+	mediaId = result["mediaId"]
+	
+	result = api.put(f"/media/{mediaId}", fileName="/path/to/my/file.mp4")
+	print(result)
+
 #### Creating a sample configuration file
 By default, the SDK will connect to the API, ask for your credentials interactively, and
 attempt to obtain an authorization token with all permissions that were granted to you. If you have
 access to multiple accounts, the token will be valid only for your default account. In order to
 easily use multiple accounts, choose a different, limited, set of permissions or use non-interactive
 M2M authentication, you will need to customise a profile in the configuration file. This
 configuration file is normally located in the `.infusevideo/` directory in your home directory. If
```

### Comparing `infusevideo-sdk-0.2.2/infusevideo/__init__.py` & `infusevideo-sdk-0.2.3/infusevideo/__init__.py`

 * *Files identical despite different names*

### Comparing `infusevideo-sdk-0.2.2/infusevideo/auth.py` & `infusevideo-sdk-0.2.3/infusevideo/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,17 @@
 	def refresh(self) -> None:
 		if self._profile.auth == "human":
 			self._refresh_human()
 		elif self._profile.auth == "m2m":
 			self._refresh_m2m()
 		elif self._profile.auth == "human-oauth2-implicit":
 			self._refresh_oauth2_implicit()
+		elif self._profile.auth == "skip":
+			self._cache["oauth2"] = {"token": ""}
+			return
 		else:
 			raise NotImplementedError(f"Unknown auth type {self._profile.auth!r}")
 		with open(self._cacheFile, "w") as f:
 			self._cache.write(f)
 
 	def _refresh_oauth2_implicit(self) -> None:
 		"""Refresh the access token using the OAuth2 Implicit flow. Credentials are entered using
```

### Comparing `infusevideo-sdk-0.2.2/infusevideo/authserver.py` & `infusevideo-sdk-0.2.3/infusevideo/authserver.py`

 * *Files identical despite different names*

### Comparing `infusevideo-sdk-0.2.2/infusevideo/client.py` & `infusevideo-sdk-0.2.3/infusevideo/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,18 +12,22 @@
 class Client:
 	class Response:
 		def __init__(self, response: requests.Response) -> None:
 			self._response = response
 			self._code: int = response.status_code
 			self._ok: bool = response.ok
 			self._data: Union[list[Any], dict[str, Any]] = {}
-			try:
-				self._data = response.json()
-			except requests.JSONDecodeError:
-				raise errors.ApiResponseDecodeError(response.text)
+			if self._code == 204:
+				if response.text:
+					raise errors.ApiError(f"Received non-empty 204: {response.text}")
+			else:
+				try:
+					self._data = response.json()
+				except requests.JSONDecodeError:
+					raise errors.ApiResponseDecodeError(response.text)
 			if not self.ok:
 				raise errors.ApiError(self)
 
 		@property
 		def data(self) -> Union[list[Any], dict[str, Any]]:
 			return self._data
 
@@ -32,14 +36,16 @@
 			return self._code
 
 		@property
 		def ok(self) -> bool:
 			return self._ok
 
 		def __str__(self) -> str:
+			if self._code == 204:
+				return ""
 			return json.dumps(self.data, indent=4)
 
 		def __getitem__(self, key) -> Any:
 			return self.data[key]
 
 		def __len__(self, key) -> int:
 			return len(self.data)
```

### Comparing `infusevideo-sdk-0.2.2/infusevideo/config.py` & `infusevideo-sdk-0.2.3/infusevideo/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from .errors import ConfigurationError, ConfigAlreadyExists, ConfigNotFound, InvalidScopeError
 from .scope import resolve_scope
 
 
 class Profile(BaseSettings):
 	name: str
 	server: str = "api.infuse.video"
-	auth: Literal["m2m", "human", "human-oauth2-implicit"] = "human"
+	auth: Literal["m2m", "human", "human-oauth2-implicit", "skip"] = "human"
 	scope_type: Literal["account", "global"] = "account"
 	account: Optional[str] = Field(
 		default=None,
 		alias="organization",
 	)
 	m2m_id: Optional[str] = None
 	m2m_secret: Optional[str] = None
```

### Comparing `infusevideo-sdk-0.2.2/infusevideo/errors.py` & `infusevideo-sdk-0.2.3/infusevideo/errors.py`

 * *Files identical despite different names*

### Comparing `infusevideo-sdk-0.2.2/infusevideo_sdk.egg-info/PKG-INFO` & `infusevideo-sdk-0.2.3/infusevideo_sdk.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infusevideo-sdk
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python SDK for the Infuse Video API
 Home-page: https://www.infuse.video
 Author: Infuse Video
 Author-email: support@infuse.video
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -62,14 +62,26 @@
 
 	import infusevideo
 
 	api = infusevideo.InfuseVideo()
 	result = api.get("/media")
 	print(result)
 
+
+Create a new Media and upload a video file:
+
+	import infusevideo
+
+	api = infusevideo.InfuseVideo()
+	result = api.post("/media", data={"name": "A name", "metadata": "Example metadata"})
+	mediaId = result["mediaId"]
+	
+	result = api.put(f"/media/{mediaId}", fileName="/path/to/my/file.mp4")
+	print(result)
+
 #### Creating a sample configuration file
 By default, the SDK will connect to the API, ask for your credentials interactively, and
 attempt to obtain an authorization token with all permissions that were granted to you. If you have
 access to multiple accounts, the token will be valid only for your default account. In order to
 easily use multiple accounts, choose a different, limited, set of permissions or use non-interactive
 M2M authentication, you will need to customise a profile in the configuration file. This
 configuration file is normally located in the `.infusevideo/` directory in your home directory. If
```

### Comparing `infusevideo-sdk-0.2.2/setup.cfg` & `infusevideo-sdk-0.2.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = infusevideo-sdk
-version = 0.2.2
+version = 0.2.3
 author = Infuse Video
 author_email = support@infuse.video
 license = MIT
 description = Python SDK for the Infuse Video API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://www.infuse.video
@@ -21,13 +21,13 @@
 [options]
 python_requires = >=3.9
 package_dir = 
 	infusevideo = infusevideo
 packages = infusevideo
 install_requires = 
 	requests>=2.27.1
-	pydantic>=1.9.0
+	pydantic>=1.9.0,<2
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

