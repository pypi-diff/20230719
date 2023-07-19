# Comparing `tmp/aaa1111-0.1.0.dev6.tar.gz` & `tmp/aaa1111-0.1.0.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aaa1111-0.1.0.dev6.tar", last modified: Mon Jul 17 14:54:34 2023, max compression
+gzip compressed data, was "aaa1111-0.1.0.dev7.tar", last modified: Wed Jul 19 12:08:39 2023, max compression
```

## Comparing `aaa1111-0.1.0.dev6.tar` & `aaa1111-0.1.0.dev7.tar`

### file list

```diff
@@ -1,31 +1,36 @@
--rw-r--r--   0        0        0     1083 2023-07-13 05:37:34.132225 aaa1111-0.1.0.dev6/LICENSE
--rw-r--r--   0        0        0       88 2023-07-13 15:33:45.322313 aaa1111-0.1.0.dev6/README.md
--rw-r--r--   0        0        0       61 2023-07-16 11:12:17.652504 aaa1111-0.1.0.dev6/aaa1111/__init__.py
--rw-r--r--   0        0        0     6232 2023-07-16 05:29:53.454992 aaa1111-0.1.0.dev6/aaa1111/__main__.py
--rw-r--r--   0        0        0       28 2023-07-17 12:55:33.157432 aaa1111-0.1.0.dev6/aaa1111/__version__.py
--rw-r--r--   0        0        0       52 2023-07-14 05:41:34.045117 aaa1111-0.1.0.dev6/aaa1111/client/__init__.py
--rw-r--r--   0        0        0     2073 2023-07-17 02:54:36.587173 aaa1111-0.1.0.dev6/aaa1111/client/action.py
--rw-r--r--   0        0        0     3442 2023-07-16 09:11:37.426730 aaa1111-0.1.0.dev6/aaa1111/client/extras.py
--rw-r--r--   0        0        0     9458 2023-07-16 10:50:01.709231 aaa1111-0.1.0.dev6/aaa1111/client/info.py
--rw-r--r--   0        0        0     2678 2023-07-17 14:42:44.488541 aaa1111-0.1.0.dev6/aaa1111/client/main.py
--rw-r--r--   0        0        0      853 2023-07-17 12:19:06.015859 aaa1111-0.1.0.dev6/aaa1111/client/options.py
--rw-r--r--   0        0        0     5946 2023-07-17 03:32:55.702077 aaa1111-0.1.0.dev6/aaa1111/client/toimg.py
--rw-r--r--   0        0        0      368 2023-07-16 11:44:07.758916 aaa1111-0.1.0.dev6/aaa1111/types/__init__.py
--rw-r--r--   0        0        0      587 2023-07-16 09:12:58.603870 aaa1111-0.1.0.dev6/aaa1111/types/base.py
--rw-r--r--   0        0        0        0 2023-07-16 12:42:28.785881 aaa1111-0.1.0.dev6/aaa1111/types/extension/__init__.py
--rw-r--r--   0        0        0     1782 2023-07-16 13:38:52.293106 aaa1111-0.1.0.dev6/aaa1111/types/extension/controlnet.py
--rw-r--r--   0        0        0     2384 2023-07-16 13:38:24.656274 aaa1111-0.1.0.dev6/aaa1111/types/extension/lora_block_weight.py
--rw-r--r--   0        0        0      306 2023-07-16 13:14:51.579466 aaa1111-0.1.0.dev6/aaa1111/types/extension/misc.py
--rw-r--r--   0        0        0     1950 2023-07-16 09:12:58.605870 aaa1111-0.1.0.dev6/aaa1111/types/extras.py
--rw-r--r--   0        0        0     2811 2023-07-16 11:02:56.779986 aaa1111-0.1.0.dev6/aaa1111/types/info.py
--rw-r--r--   0        0        0     5493 2023-07-17 03:04:40.400483 aaa1111-0.1.0.dev6/aaa1111/types/toimg.py
--rw-r--r--   0        0        0     5579 2023-07-17 14:00:36.489658 aaa1111-0.1.0.dev6/aaa1111/utils.py
--rw-r--r--   0        0        0     1230 2023-07-17 14:54:34.930184 aaa1111-0.1.0.dev6/pyproject.toml
--rw-r--r--   0        0        0      731 2023-07-17 14:27:53.688121 aaa1111-0.1.0.dev6/tests/conftest.py
--rw-r--r--   0        0        0   573492 2023-07-14 12:24:42.631826 aaa1111-0.1.0.dev6/tests/image/test1.png
--rw-r--r--   0        0        0   466758 2023-07-17 13:52:38.641903 aaa1111-0.1.0.dev6/tests/image/test2.webp
--rw-r--r--   0        0        0   132490 2023-07-17 13:53:50.814172 aaa1111-0.1.0.dev6/tests/image/test3.jpg
--rw-r--r--   0        0        0      349 2023-07-17 14:30:35.485475 aaa1111-0.1.0.dev6/tests/test_action.py
--rw-r--r--   0        0        0     3833 2023-07-17 14:53:06.259898 aaa1111-0.1.0.dev6/tests/test_info.py
--rw-r--r--   0        0        0     1165 2023-07-17 14:50:26.087051 aaa1111-0.1.0.dev6/tests/test_misc.py
--rw-r--r--   0        0        0      648 1970-01-01 00:00:00.000000 aaa1111-0.1.0.dev6/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-07-13 05:37:34.132225 aaa1111-0.1.0.dev7/LICENSE
+-rw-r--r--   0        0        0     8095 2023-07-19 12:06:51.127933 aaa1111-0.1.0.dev7/README.md
+-rw-r--r--   0        0        0       61 2023-07-16 11:12:17.652504 aaa1111-0.1.0.dev7/aaa1111/__init__.py
+-rw-r--r--   0        0        0     6232 2023-07-16 05:29:53.454992 aaa1111-0.1.0.dev7/aaa1111/__main__.py
+-rw-r--r--   0        0        0       28 2023-07-19 12:07:54.447582 aaa1111-0.1.0.dev7/aaa1111/__version__.py
+-rw-r--r--   0        0        0       52 2023-07-14 05:41:34.045117 aaa1111-0.1.0.dev7/aaa1111/client/__init__.py
+-rw-r--r--   0        0        0     2073 2023-07-17 02:54:36.587173 aaa1111-0.1.0.dev7/aaa1111/client/action.py
+-rw-r--r--   0        0        0     3442 2023-07-16 09:11:37.426730 aaa1111-0.1.0.dev7/aaa1111/client/extras.py
+-rw-r--r--   0        0        0     9458 2023-07-16 10:50:01.709231 aaa1111-0.1.0.dev7/aaa1111/client/info.py
+-rw-r--r--   0        0        0     2546 2023-07-19 07:54:31.219790 aaa1111-0.1.0.dev7/aaa1111/client/main.py
+-rw-r--r--   0        0        0      853 2023-07-17 12:19:06.015859 aaa1111-0.1.0.dev7/aaa1111/client/options.py
+-rw-r--r--   0        0        0     5946 2023-07-17 03:32:55.702077 aaa1111-0.1.0.dev7/aaa1111/client/toimg.py
+-rw-r--r--   0        0        0      368 2023-07-16 11:44:07.758916 aaa1111-0.1.0.dev7/aaa1111/types/__init__.py
+-rw-r--r--   0        0        0      664 2023-07-18 02:38:46.890339 aaa1111-0.1.0.dev7/aaa1111/types/base.py
+-rw-r--r--   0        0        0      326 2023-07-18 03:10:40.329532 aaa1111-0.1.0.dev7/aaa1111/types/extension/__init__.py
+-rw-r--r--   0        0        0     1782 2023-07-16 13:38:52.293106 aaa1111-0.1.0.dev7/aaa1111/types/extension/controlnet.py
+-rw-r--r--   0        0        0     1579 2023-07-18 03:10:40.334047 aaa1111-0.1.0.dev7/aaa1111/types/extension/dynamic_thresholding.py
+-rw-r--r--   0        0        0     2384 2023-07-16 13:38:24.656274 aaa1111-0.1.0.dev7/aaa1111/types/extension/lora_block_weight.py
+-rw-r--r--   0        0        0      306 2023-07-16 13:14:51.579466 aaa1111-0.1.0.dev7/aaa1111/types/extension/misc.py
+-rw-r--r--   0        0        0     1950 2023-07-16 09:12:58.605870 aaa1111-0.1.0.dev7/aaa1111/types/extras.py
+-rw-r--r--   0        0        0     2811 2023-07-16 11:02:56.779986 aaa1111-0.1.0.dev7/aaa1111/types/info.py
+-rw-r--r--   0        0        0     5493 2023-07-17 03:04:40.400483 aaa1111-0.1.0.dev7/aaa1111/types/toimg.py
+-rw-r--r--   0        0        0     5359 2023-07-19 11:31:02.433094 aaa1111-0.1.0.dev7/aaa1111/utils.py
+-rw-r--r--   0        0        0     1301 2023-07-19 12:08:39.849192 aaa1111-0.1.0.dev7/pyproject.toml
+-rw-r--r--   0        0        0     1082 2023-07-19 08:06:06.424527 aaa1111-0.1.0.dev7/tests/async.py
+-rw-r--r--   0        0        0      847 2023-07-19 07:58:54.380958 aaa1111-0.1.0.dev7/tests/conftest.py
+-rw-r--r--   0        0        0   573492 2023-07-14 12:24:42.631826 aaa1111-0.1.0.dev7/tests/image/test1.png
+-rw-r--r--   0        0        0   466758 2023-07-17 13:52:38.641903 aaa1111-0.1.0.dev7/tests/image/test2.webp
+-rw-r--r--   0        0        0   132490 2023-07-17 13:53:50.814172 aaa1111-0.1.0.dev7/tests/image/test3.jpg
+-rw-r--r--   0        0        0      349 2023-07-17 14:30:35.485475 aaa1111-0.1.0.dev7/tests/test_action.py
+-rw-r--r--   0        0        0      452 2023-07-19 11:36:13.551221 aaa1111-0.1.0.dev7/tests/test_async_action.py
+-rw-r--r--   0        0        0     4170 2023-07-19 11:36:13.551221 aaa1111-0.1.0.dev7/tests/test_async_info.py
+-rw-r--r--   0        0        0     1247 2023-07-19 11:36:13.552221 aaa1111-0.1.0.dev7/tests/test_async_misc.py
+-rw-r--r--   0        0        0     3833 2023-07-17 14:53:06.259898 aaa1111-0.1.0.dev7/tests/test_info.py
+-rw-r--r--   0        0        0     1165 2023-07-17 14:50:26.087051 aaa1111-0.1.0.dev7/tests/test_misc.py
+-rw-r--r--   0        0        0     8460 1970-01-01 00:00:00.000000 aaa1111-0.1.0.dev7/PKG-INFO
```

### Comparing `aaa1111-0.1.0.dev6/LICENSE` & `aaa1111-0.1.0.dev7/LICENSE`

 * *Files identical despite different names*

### Comparing `aaa1111-0.1.0.dev6/aaa1111/__main__.py` & `aaa1111-0.1.0.dev7/aaa1111/__main__.py`

 * *Files identical despite different names*

### Comparing `aaa1111-0.1.0.dev6/aaa1111/client/action.py` & `aaa1111-0.1.0.dev7/aaa1111/client/action.py`

 * *Files identical despite different names*

### Comparing `aaa1111-0.1.0.dev6/aaa1111/client/extras.py` & `aaa1111-0.1.0.dev7/aaa1111/client/extras.py`

 * *Files identical despite different names*

### Comparing `aaa1111-0.1.0.dev6/aaa1111/client/info.py` & `aaa1111-0.1.0.dev7/aaa1111/client/info.py`

 * *Files identical despite different names*

### Comparing `aaa1111-0.1.0.dev6/aaa1111/client/main.py` & `aaa1111-0.1.0.dev7/aaa1111/client/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 import asyncio
-import platform
 from pathlib import Path
 from typing import Any, Mapping, Optional, Union
 
 from beartype import beartype
 from httpx import URL, AsyncClient, BasicAuth, Client, Timeout
 
 from aaa1111.utils import load_from_file
 
 from .action import ActionMixin
 from .extras import ExtrasMixin
 from .info import InfoMixin
 from .options import OptionsMixin
 from .toimg import ToImageMixin
 
-if platform.system() == "Windows":
-    asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
-
 
 @beartype
 class AAA1111(OptionsMixin, InfoMixin, ActionMixin, ExtrasMixin, ToImageMixin):
     def __init__(
         self,
         host: str = "127.0.0.1",
         port: int = 7860,
```

### Comparing `aaa1111-0.1.0.dev6/aaa1111/client/options.py` & `aaa1111-0.1.0.dev7/aaa1111/client/options.py`

 * *Files identical despite different names*

### Comparing `aaa1111-0.1.0.dev6/aaa1111/client/toimg.py` & `aaa1111-0.1.0.dev7/aaa1111/client/toimg.py`

 * *Files identical despite different names*

### Comparing `aaa1111-0.1.0.dev6/aaa1111/types/base.py` & `aaa1111-0.1.0.dev7/aaa1111/types/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-from dataclasses import asdict, fields
+from dataclasses import MISSING, fields
 from pathlib import Path
 from typing import Any, Dict, Sized, Union
 
 from PIL import Image
 
 ImageType = Union[str, Path, Image.Image]
 PathType = Union[str, Path]
 Number = Union[int, float]
 
 
 class AsdictMixin:
     def asdict(self) -> Dict[str, Any]:
-        d = asdict(self)
+        d = {}
         for field in fields(self):
             value = getattr(self, field.name)
             default = field.default
 
-            if value == default or (isinstance(value, Sized) and not value):
-                d.pop(field.name, None)
+            if (default is not MISSING and value != default) or (
+                not isinstance(value, str) and isinstance(value, Sized) and value
+            ):
+                d[field.name] = value
         return d
```

### Comparing `aaa1111-0.1.0.dev6/aaa1111/types/extension/controlnet.py` & `aaa1111-0.1.0.dev7/aaa1111/types/extension/controlnet.py`

 * *Files identical despite different names*

### Comparing `aaa1111-0.1.0.dev6/aaa1111/types/extension/lora_block_weight.py` & `aaa1111-0.1.0.dev7/aaa1111/types/extension/lora_block_weight.py`

 * *Files identical despite different names*

### Comparing `aaa1111-0.1.0.dev6/aaa1111/types/extras.py` & `aaa1111-0.1.0.dev7/aaa1111/types/extras.py`

 * *Files identical despite different names*

### Comparing `aaa1111-0.1.0.dev6/aaa1111/types/info.py` & `aaa1111-0.1.0.dev7/aaa1111/types/info.py`

 * *Files identical despite different names*

### Comparing `aaa1111-0.1.0.dev6/aaa1111/types/toimg.py` & `aaa1111-0.1.0.dev7/aaa1111/types/toimg.py`

 * *Files identical despite different names*

### Comparing `aaa1111-0.1.0.dev6/aaa1111/utils.py` & `aaa1111-0.1.0.dev7/aaa1111/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,67 +3,68 @@
 from pathlib import Path
 from typing import Any, Dict, Mapping, Optional, Sequence, Union
 
 import orjson
 import pyjson5
 import rtoml
 from aiofile import async_open
+from beartype import beartype
 from PIL import Image, PngImagePlugin
 from ruamel.yaml import YAML
 from ulid import ULID
 
 ImageType = Union[str, Path, Image.Image]  # prevent circular import
 PathType = Union[str, Path]
 
 FILE_EXT = (".toml", ".yaml", ".yml", ".json", ".json5")
 available_extensions = Image.registered_extensions()
 
 
+@beartype
+def pil_to_base64(img: Image.Image) -> str:
+    buf = io.BytesIO()
+    # 1. png
+    if "parameters" in img.info:
+        pnginfo = PngImagePlugin.PngInfo()
+        pnginfo.add_text("parameters", img.info["parameters"])
+        img.save(buf, format="png", pnginfo=pnginfo)
+    # 2. else
+    else:
+        img.save(buf, format="webp", lossless=True, exif=img.getexif())
+    value = buf.getvalue()
+    return base64.b64encode(value).decode("utf-8")
+
+
+@beartype
 def image_to_base64(img: ImageType) -> str:
     if isinstance(img, Image.Image):
-        buf = io.BytesIO()
-        # 1. png
-        if "parameters" in img.info:
-            pnginfo = PngImagePlugin.PngInfo()
-            pnginfo.add_text("parameters", img.info["parameters"])
-            img.save(buf, format="png", pnginfo=pnginfo)
-        # 2. else
-        else:
-            img.save(buf, format="webp", lossless=True, exif=img.getexif())
-        value = buf.getvalue()
-    else:
-        if isinstance(img, str) and not Path(img).is_file():
-            # expect img is base64 string
-            return img
-        with open(img, "rb") as f:
-            value = f.read()
+        return pil_to_base64(img)
+
+    if isinstance(img, str) and not Path(img).is_file():
+        # expect img is base64 string
+        return img
+    with open(img, "rb") as f:
+        value = f.read()
     return base64.b64encode(value).decode("utf-8")
 
 
+@beartype
 async def aimage_to_base64(img: ImageType) -> str:
     if isinstance(img, Image.Image):
-        buf = io.BytesIO()
-        # 1. png
-        if "parameters" in img.info:
-            pnginfo = PngImagePlugin.PngInfo()
-            pnginfo.add_text("parameters", img.info["parameters"])
-            img.save(buf, format="png", pnginfo=pnginfo)
-        # 2. else
-        else:
-            img.save(buf, format="webp", lossless=True, exif=img.getexif())
-        value = buf.getvalue()
-    else:
-        if isinstance(img, str) and not Path(img).is_file():
-            # expect img is base64 string
-            return img
-        async with async_open(img, "rb") as f:
-            value = await f.read()
+        return pil_to_base64(img)
+
+    if isinstance(img, str) and not Path(img).is_file():
+        # expect img is base64 string
+        return img
+    async with async_open(img, "rb") as f:
+        value = await f.read()
     return base64.b64encode(value).decode("utf-8")
 
 
+@beartype
 def base64_to_image(s: str) -> Image.Image:
     return Image.open(io.BytesIO(base64.b64decode(s)))
 
 
 def is_image(obj: Any) -> bool:
     if isinstance(obj, (str, Path)) and (p := Path(obj)).is_file():
         return p.suffix.lower() in available_extensions
@@ -106,19 +107,21 @@
     return item
 
 
 async def arecursive_read_image(item: Mapping[str, Any]) -> Dict[str, Any]:
     return await _arecursive_read_image(item)
 
 
+@beartype
 def is_valid_file(file: PathType) -> bool:
     ext = Path(file).suffix.lower()
     return ext in FILE_EXT
 
 
+@beartype
 def load_from_file(file: PathType) -> Dict[str, Any]:
     if not is_valid_file(file):
         msg = f"Unsupported file extension: {file!r}"
         raise ValueError(msg)
     ext = Path(file).suffix.lower()
 
     with open(file, encoding="utf-8") as raw:
@@ -127,14 +130,15 @@
         if ext == ".json":
             return orjson.loads(raw.read())
         if ext == ".json5":
             return pyjson5.decode_io(raw)
         return dict(YAML().load(raw))
 
 
+@beartype
 async def aload_from_file(file: PathType) -> Dict[str, Any]:
     if not is_valid_file(file):
         msg = f"Unsupported file extension: {file!r}"
         raise ValueError(msg)
     ext = Path(file).suffix.lower()
 
     async with async_open(file, encoding="utf-8") as raw:
```

### Comparing `aaa1111-0.1.0.dev6/pyproject.toml` & `aaa1111-0.1.0.dev7/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "python-ulid",
     "rich",
     "typer>=0.9.0",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 dynamic = []
-version = "0.1.0.dev6"
+version = "0.1.0.dev7"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 repository = "https://github.com/Bing-su/AAA1111"
 
@@ -44,14 +44,15 @@
     "black",
     "ruff",
     "pre-commit",
     "ipywidgets",
 ]
 test = [
     "pytest",
+    "pytest-asyncio",
     "python-dotenv",
 ]
 
 [tool.pdm.version]
 source = "file"
 path = "aaa1111/__version__.py"
 
@@ -81,7 +82,10 @@
     "B905",
     "E501",
     "FA100",
 ]
 unfixable = [
     "F401",
 ]
+
+[tool.pytest.ini_options]
+asyncio_mode = "auto"
```

### Comparing `aaa1111-0.1.0.dev6/tests/image/test1.png` & `aaa1111-0.1.0.dev7/tests/image/test1.png`

 * *Files identical despite different names*

### Comparing `aaa1111-0.1.0.dev6/tests/image/test2.webp` & `aaa1111-0.1.0.dev7/tests/image/test2.webp`

 * *Files identical despite different names*

### Comparing `aaa1111-0.1.0.dev6/tests/image/test3.jpg` & `aaa1111-0.1.0.dev7/tests/image/test3.jpg`

 * *Files identical despite different names*

### Comparing `aaa1111-0.1.0.dev6/tests/test_info.py` & `aaa1111-0.1.0.dev7/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `aaa1111-0.1.0.dev6/tests/test_misc.py` & `aaa1111-0.1.0.dev7/tests/test_misc.py`

 * *Files identical despite different names*

