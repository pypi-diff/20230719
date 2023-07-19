# Comparing `tmp/onyx_client-7.0.0.tar.gz` & `tmp/onyx_client-7.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onyx_client-7.0.0.tar", max compression
+gzip compressed data, was "onyx_client-7.1.0.tar", max compression
```

## Comparing `onyx_client-7.0.0.tar` & `onyx_client-7.1.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1090 2023-06-08 07:18:16.339206 onyx_client-7.0.0/LICENSE
--rw-r--r--   0        0        0     5830 2023-06-08 07:18:16.339206 onyx_client-7.0.0/README.md
--rw-r--r--   0        0        0       47 2023-06-08 07:18:16.339206 onyx_client-7.0.0/onyx_client/__init__.py
--rw-r--r--   0        0        0     1289 2023-06-08 07:18:16.339206 onyx_client-7.0.0/onyx_client/authorizer/__init__.py
--rw-r--r--   0        0        0     9359 2023-06-08 07:18:16.339206 onyx_client-7.0.0/onyx_client/client.py
--rw-r--r--   0        0        0       33 2023-06-08 07:18:16.339206 onyx_client-7.0.0/onyx_client/configuration/__init__.py
--rw-r--r--   0        0        0      290 2023-06-08 07:18:16.339206 onyx_client-7.0.0/onyx_client/configuration/configuration.py
--rw-r--r--   0        0        0       32 2023-06-08 07:18:16.339206 onyx_client-7.0.0/onyx_client/data/__init__.py
--rw-r--r--   0        0        0     1119 2023-06-08 07:18:16.339206 onyx_client-7.0.0/onyx_client/data/animation_keyframe.py
--rw-r--r--   0        0        0     1072 2023-06-08 07:18:16.339206 onyx_client-7.0.0/onyx_client/data/animation_value.py
--rw-r--r--   0        0        0      768 2023-06-08 07:18:16.339206 onyx_client-7.0.0/onyx_client/data/boolean_value.py
--rw-r--r--   0        0        0      383 2023-06-08 07:18:16.339206 onyx_client-7.0.0/onyx_client/data/date_information.py
--rw-r--r--   0        0        0     1297 2023-06-08 07:18:16.339206 onyx_client-7.0.0/onyx_client/data/device_command.py
--rw-r--r--   0        0        0      312 2023-06-08 07:18:16.339206 onyx_client-7.0.0/onyx_client/data/device_mode.py
--rw-r--r--   0        0        0     2030 2023-06-08 07:18:16.339206 onyx_client-7.0.0/onyx_client/data/numeric_value.py
--rw-r--r--   0        0        0      384 2023-06-08 07:18:16.339206 onyx_client-7.0.0/onyx_client/data/supported_versions.py
--rw-r--r--   0        0        0       24 2023-06-08 07:18:16.339206 onyx_client-7.0.0/onyx_client/device/__init__.py
--rw-r--r--   0        0        0      833 2023-06-08 07:18:16.339206 onyx_client-7.0.0/onyx_client/device/click.py
--rw-r--r--   0        0        0     1365 2023-06-08 07:18:16.339206 onyx_client-7.0.0/onyx_client/device/device.py
--rw-r--r--   0        0        0     1572 2023-06-08 07:18:16.339206 onyx_client-7.0.0/onyx_client/device/light.py
--rw-r--r--   0        0        0     2010 2023-06-08 07:18:16.339206 onyx_client-7.0.0/onyx_client/device/shutter.py
--rw-r--r--   0        0        0      663 2023-06-08 07:18:16.339206 onyx_client-7.0.0/onyx_client/device/switch.py
--rw-r--r--   0        0        0     2270 2023-06-08 07:18:16.339206 onyx_client-7.0.0/onyx_client/device/weather.py
--rw-r--r--   0        0        0       29 2023-06-08 07:18:16.339206 onyx_client-7.0.0/onyx_client/enum/__init__.py
--rw-r--r--   0        0        0      635 2023-06-08 07:18:16.339206 onyx_client-7.0.0/onyx_client/enum/action.py
--rw-r--r--   0        0        0      989 2023-06-08 07:18:16.339206 onyx_client-7.0.0/onyx_client/enum/device_type.py
--rw-r--r--   0        0        0       27 2023-06-08 07:18:16.339206 onyx_client-7.0.0/onyx_client/exception/__init__.py
--rw-r--r--   0        0        0      136 2023-06-08 07:18:16.339206 onyx_client-7.0.0/onyx_client/exception/invalid_command.py
--rw-r--r--   0        0        0      122 2023-06-08 07:18:16.339206 onyx_client-7.0.0/onyx_client/exception/update_exception.py
--rw-r--r--   0        0        0       23 2023-06-08 07:18:16.339206 onyx_client-7.0.0/onyx_client/group/__init__.py
--rw-r--r--   0        0        0      457 2023-06-08 07:18:16.339206 onyx_client-7.0.0/onyx_client/group/group.py
--rw-r--r--   0        0        0       27 2023-06-08 07:18:16.339206 onyx_client-7.0.0/onyx_client/helpers/__init__.py
--rw-r--r--   0        0        0     2751 2023-06-08 07:18:16.339206 onyx_client-7.0.0/onyx_client/helpers/url.py
--rw-r--r--   0        0        0       25 2023-06-08 07:18:16.339206 onyx_client-7.0.0/onyx_client/utils/__init__.py
--rw-r--r--   0        0        0      150 2023-06-08 07:18:16.339206 onyx_client-7.0.0/onyx_client/utils/const.py
--rw-r--r--   0        0        0     1823 2023-06-08 07:18:16.339206 onyx_client-7.0.0/onyx_client/utils/device_type.py
--rw-r--r--   0        0        0      125 2023-06-08 07:18:16.339206 onyx_client-7.0.0/onyx_client/utils/filter.py
--rw-r--r--   0        0        0     3373 2023-06-08 07:18:16.339206 onyx_client-7.0.0/onyx_client/utils/mapper.py
--rw-r--r--   0        0        0      536 2023-06-08 07:18:16.339206 onyx_client-7.0.0/onyx_client/utils/response.py
--rw-r--r--   0        0        0     2927 2023-06-08 07:18:55.887450 onyx_client-7.0.0/pyproject.toml
--rw-r--r--   0        0        0     6636 1970-01-01 00:00:00.000000 onyx_client-7.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-07-19 07:47:12.708170 onyx_client-7.1.0/LICENSE
+-rw-r--r--   0        0        0     5579 2023-07-19 07:47:12.708170 onyx_client-7.1.0/README.md
+-rw-r--r--   0        0        0       47 2023-07-19 07:47:12.708170 onyx_client-7.1.0/onyx_client/__init__.py
+-rw-r--r--   0        0        0     1289 2023-07-19 07:47:12.712170 onyx_client-7.1.0/onyx_client/authorizer/__init__.py
+-rw-r--r--   0        0        0     9359 2023-07-19 07:47:12.712170 onyx_client-7.1.0/onyx_client/client.py
+-rw-r--r--   0        0        0       33 2023-07-19 07:47:12.712170 onyx_client-7.1.0/onyx_client/configuration/__init__.py
+-rw-r--r--   0        0        0      290 2023-07-19 07:47:12.712170 onyx_client-7.1.0/onyx_client/configuration/configuration.py
+-rw-r--r--   0        0        0       32 2023-07-19 07:47:12.712170 onyx_client-7.1.0/onyx_client/data/__init__.py
+-rw-r--r--   0        0        0     1119 2023-07-19 07:47:12.712170 onyx_client-7.1.0/onyx_client/data/animation_keyframe.py
+-rw-r--r--   0        0        0     1072 2023-07-19 07:47:12.712170 onyx_client-7.1.0/onyx_client/data/animation_value.py
+-rw-r--r--   0        0        0      768 2023-07-19 07:47:12.712170 onyx_client-7.1.0/onyx_client/data/boolean_value.py
+-rw-r--r--   0        0        0      383 2023-07-19 07:47:12.712170 onyx_client-7.1.0/onyx_client/data/date_information.py
+-rw-r--r--   0        0        0     1297 2023-07-19 07:47:12.712170 onyx_client-7.1.0/onyx_client/data/device_command.py
+-rw-r--r--   0        0        0      312 2023-07-19 07:47:12.712170 onyx_client-7.1.0/onyx_client/data/device_mode.py
+-rw-r--r--   0        0        0     2030 2023-07-19 07:47:12.712170 onyx_client-7.1.0/onyx_client/data/numeric_value.py
+-rw-r--r--   0        0        0      384 2023-07-19 07:47:12.712170 onyx_client-7.1.0/onyx_client/data/supported_versions.py
+-rw-r--r--   0        0        0       24 2023-07-19 07:47:12.712170 onyx_client-7.1.0/onyx_client/device/__init__.py
+-rw-r--r--   0        0        0      833 2023-07-19 07:47:12.712170 onyx_client-7.1.0/onyx_client/device/click.py
+-rw-r--r--   0        0        0     1365 2023-07-19 07:47:12.712170 onyx_client-7.1.0/onyx_client/device/device.py
+-rw-r--r--   0        0        0     1572 2023-07-19 07:47:12.712170 onyx_client-7.1.0/onyx_client/device/light.py
+-rw-r--r--   0        0        0     2010 2023-07-19 07:47:12.712170 onyx_client-7.1.0/onyx_client/device/shutter.py
+-rw-r--r--   0        0        0      663 2023-07-19 07:47:12.712170 onyx_client-7.1.0/onyx_client/device/switch.py
+-rw-r--r--   0        0        0     2270 2023-07-19 07:47:12.712170 onyx_client-7.1.0/onyx_client/device/weather.py
+-rw-r--r--   0        0        0       29 2023-07-19 07:47:12.712170 onyx_client-7.1.0/onyx_client/enum/__init__.py
+-rw-r--r--   0        0        0      635 2023-07-19 07:47:12.712170 onyx_client-7.1.0/onyx_client/enum/action.py
+-rw-r--r--   0        0        0     1216 2023-07-19 07:47:12.712170 onyx_client-7.1.0/onyx_client/enum/device_type.py
+-rw-r--r--   0        0        0       27 2023-07-19 07:47:12.712170 onyx_client-7.1.0/onyx_client/exception/__init__.py
+-rw-r--r--   0        0        0      136 2023-07-19 07:47:12.712170 onyx_client-7.1.0/onyx_client/exception/invalid_command.py
+-rw-r--r--   0        0        0      122 2023-07-19 07:47:12.712170 onyx_client-7.1.0/onyx_client/exception/update_exception.py
+-rw-r--r--   0        0        0       23 2023-07-19 07:47:12.712170 onyx_client-7.1.0/onyx_client/group/__init__.py
+-rw-r--r--   0        0        0      457 2023-07-19 07:47:12.712170 onyx_client-7.1.0/onyx_client/group/group.py
+-rw-r--r--   0        0        0       27 2023-07-19 07:47:12.712170 onyx_client-7.1.0/onyx_client/helpers/__init__.py
+-rw-r--r--   0        0        0     2751 2023-07-19 07:47:12.712170 onyx_client-7.1.0/onyx_client/helpers/url.py
+-rw-r--r--   0        0        0       25 2023-07-19 07:47:12.712170 onyx_client-7.1.0/onyx_client/utils/__init__.py
+-rw-r--r--   0        0        0      150 2023-07-19 07:47:12.712170 onyx_client-7.1.0/onyx_client/utils/const.py
+-rw-r--r--   0        0        0     1823 2023-07-19 07:47:12.712170 onyx_client-7.1.0/onyx_client/utils/device_type.py
+-rw-r--r--   0        0        0      125 2023-07-19 07:47:12.712170 onyx_client-7.1.0/onyx_client/utils/filter.py
+-rw-r--r--   0        0        0     3373 2023-07-19 07:47:12.712170 onyx_client-7.1.0/onyx_client/utils/mapper.py
+-rw-r--r--   0        0        0      536 2023-07-19 07:47:12.712170 onyx_client-7.1.0/onyx_client/utils/response.py
+-rw-r--r--   0        0        0     2684 2023-07-19 07:47:12.712170 onyx_client-7.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6385 1970-01-01 00:00:00.000000 onyx_client-7.1.0/PKG-INFO
```

### Comparing `onyx_client-7.0.0/LICENSE` & `onyx_client-7.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `onyx_client-7.0.0/README.md` & `onyx_client-7.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -139,32 +139,14 @@
 ### Commit Message
 
 This project follows [Conventional Commits](https://www.conventionalcommits.org/), and your commit message must also
 adhere to the additional rules outlined in `.conform.yaml`.
 
 ---
 
-## Release
-
-To draft a release, use [standard-version](https://github.com/conventional-changelog/standard-version):
-
-```bash
-standard-version
-# alternatively
-npx standard-version
-```
-
-Finally, push with tags:
-
-```bash
-git push --follow-tags
-```
-
----
-
 ## Contributions
 
 Please feel free to contribute, be it with Issues or Pull Requests! Please read
 the [Contribution guidelines](CONTRIBUTING.md)
 
 ## Supporting
```

#### html2text {}

```diff
@@ -56,15 +56,12 @@
 run flakehell lint ``` ### Building This package uses [poetry-dynamic-
 versioning](https://github.com/mtkennerly/poetry-dynamic-versioning) which
 infers the version number based on the Git tags. Hence, to have a proper
 versioning for the distribution, use Python's build system like: ```bash pip
 install build python -m build ``` Your distribution will be in the `dist`
 directory. ### Commit Message This project follows [Conventional Commits]
 (https://www.conventionalcommits.org/), and your commit message must also
-adhere to the additional rules outlined in `.conform.yaml`. --- ## Release To
-draft a release, use [standard-version](https://github.com/conventional-
-changelog/standard-version): ```bash standard-version # alternatively npx
-standard-version ``` Finally, push with tags: ```bash git push --follow-tags
-``` --- ## Contributions Please feel free to contribute, be it with Issues or
-Pull Requests! Please read the [Contribution guidelines](CONTRIBUTING.md) ##
+adhere to the additional rules outlined in `.conform.yaml`. --- ##
+Contributions Please feel free to contribute, be it with Issues or Pull
+Requests! Please read the [Contribution guidelines](CONTRIBUTING.md) ##
 Supporting If you enjoy the application and want to support my efforts, please
 feel free to buy me a coffe. :) [Buy_Me_A_Coffee]
```

### Comparing `onyx_client-7.0.0/onyx_client/authorizer/__init__.py` & `onyx_client-7.1.0/onyx_client/authorizer/__init__.py`

 * *Files identical despite different names*

### Comparing `onyx_client-7.0.0/onyx_client/client.py` & `onyx_client-7.1.0/onyx_client/client.py`

 * *Files identical despite different names*

### Comparing `onyx_client-7.0.0/onyx_client/data/animation_keyframe.py` & `onyx_client-7.1.0/onyx_client/data/animation_keyframe.py`

 * *Files identical despite different names*

### Comparing `onyx_client-7.0.0/onyx_client/data/animation_value.py` & `onyx_client-7.1.0/onyx_client/data/animation_value.py`

 * *Files identical despite different names*

### Comparing `onyx_client-7.0.0/onyx_client/data/boolean_value.py` & `onyx_client-7.1.0/onyx_client/data/boolean_value.py`

 * *Files identical despite different names*

### Comparing `onyx_client-7.0.0/onyx_client/data/device_command.py` & `onyx_client-7.1.0/onyx_client/data/device_command.py`

 * *Files identical despite different names*

### Comparing `onyx_client-7.0.0/onyx_client/data/numeric_value.py` & `onyx_client-7.1.0/onyx_client/data/numeric_value.py`

 * *Files identical despite different names*

### Comparing `onyx_client-7.0.0/onyx_client/device/click.py` & `onyx_client-7.1.0/onyx_client/device/click.py`

 * *Files identical despite different names*

### Comparing `onyx_client-7.0.0/onyx_client/device/device.py` & `onyx_client-7.1.0/onyx_client/device/device.py`

 * *Files identical despite different names*

### Comparing `onyx_client-7.0.0/onyx_client/device/light.py` & `onyx_client-7.1.0/onyx_client/device/light.py`

 * *Files identical despite different names*

### Comparing `onyx_client-7.0.0/onyx_client/device/shutter.py` & `onyx_client-7.1.0/onyx_client/device/shutter.py`

 * *Files identical despite different names*

### Comparing `onyx_client-7.0.0/onyx_client/device/switch.py` & `onyx_client-7.1.0/onyx_client/device/switch.py`

 * *Files identical despite different names*

### Comparing `onyx_client-7.0.0/onyx_client/device/weather.py` & `onyx_client-7.1.0/onyx_client/device/weather.py`

 * *Files identical despite different names*

### Comparing `onyx_client-7.0.0/onyx_client/enum/action.py` & `onyx_client-7.1.0/onyx_client/enum/action.py`

 * *Files identical despite different names*

### Comparing `onyx_client-7.0.0/onyx_client/enum/device_type.py` & `onyx_client-7.1.0/onyx_client/enum/device_type.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,27 +10,34 @@
     RAFFSTORE_90 = auto()
     RAFFSTORE_180 = auto()
     WEATHER = auto()
     VENEER = auto()
     BASIC_LIGHT = auto()
     CLICK = auto()
     SWITCH = auto()
+    PERGOLA_AWNING_ROOF = (auto(),)
+    PERGOLA_SIDE = (auto,)
+    PERGOLA_SLAT_ROOF = (auto(),)
     UNKNOWN = 9999
 
     def string(self) -> str:
         """Get the string representation for the Onyx API."""
         return self.name.lower()
 
     def is_shutter(self) -> bool:
         """Check if the type corresponds to any kind of shutter."""
         return self in [
             self.ROLLERSHUTTER,
             self.AWNING,
             self.RAFFSTORE_90,
             self.RAFFSTORE_180,
+            self.VENEER,
+            self.PERGOLA_AWNING_ROOF,
+            self.PERGOLA_SIDE,
+            self.PERGOLA_SLAT_ROOF,
         ]
 
     @staticmethod
     def convert(lower: str):
         """Get the device type from the Onyx API's type information."""
         try:
             return DeviceType[lower.upper()]
```

### Comparing `onyx_client-7.0.0/onyx_client/helpers/url.py` & `onyx_client-7.1.0/onyx_client/helpers/url.py`

 * *Files identical despite different names*

### Comparing `onyx_client-7.0.0/onyx_client/utils/device_type.py` & `onyx_client-7.1.0/onyx_client/utils/device_type.py`

 * *Files identical despite different names*

### Comparing `onyx_client-7.0.0/onyx_client/utils/mapper.py` & `onyx_client-7.1.0/onyx_client/utils/mapper.py`

 * *Files identical despite different names*

### Comparing `onyx_client-7.0.0/onyx_client/utils/response.py` & `onyx_client-7.1.0/onyx_client/utils/response.py`

 * *Files identical despite different names*

### Comparing `onyx_client-7.0.0/pyproject.toml` & `onyx_client-7.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 [build-system]
 requires = [
-    "poetry>=1.5.1",
-    "poetry-dynamic-versioning>=0.21.4"
+    "poetry-core"
 ]
-build-backend = "poetry_dynamic_versioning.backend"
+build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "onyx-client"
-version = "7.0.0"
+version = "7.1.0"
 description = "HTTP Client for Hella's ONYX.CENTER API."
 license = "MIT"
 authors = [
     "Daniel Muehlbachler-Pietrzykowski <daniel.muehlbachler@niftyside.io>"
 ]
 readme = "README.md"
 repository = "https://github.com/muhlba91/onyx-client"
@@ -39,21 +38,14 @@
 flakeheaven = "^3.2.1"
 coverage = { extras = ["toml"], version = "^7.0.0" }
 black = "^23.1.0"
 pre-commit = "^3.1.1"
 pytest-asyncio = "^0.21.0"
 aioresponses = "^0.7.4"
 
-[tool.poetry-dynamic-versioning]
-enable = false
-vcs = "git"
-style = "pep440"
-format-jinja = "{% if distance == 0 %}{{ base }}{% else %}{{ base }}.dev{{ distance }}{% endif %}"
-dirty = true
-
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "--strict-markers --cov=onyx_client"
 testpaths = [
     "tests",
 ]
 norecursedirs = [
```

### Comparing `onyx_client-7.0.0/PKG-INFO` & `onyx_client-7.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onyx-client
-Version: 7.0.0
+Version: 7.1.0
 Summary: HTTP Client for Hella's ONYX.CENTER API.
 Home-page: https://github.com/muhlba91/onyx-client
 License: MIT
 Keywords: hella-info,onyx,onyx-center
 Author: Daniel Muehlbachler-Pietrzykowski
 Author-email: daniel.muehlbachler@niftyside.io
 Requires-Python: >=3.11,<4.0
@@ -160,32 +160,14 @@
 ### Commit Message
 
 This project follows [Conventional Commits](https://www.conventionalcommits.org/), and your commit message must also
 adhere to the additional rules outlined in `.conform.yaml`.
 
 ---
 
-## Release
-
-To draft a release, use [standard-version](https://github.com/conventional-changelog/standard-version):
-
-```bash
-standard-version
-# alternatively
-npx standard-version
-```
-
-Finally, push with tags:
-
-```bash
-git push --follow-tags
-```
-
----
-
 ## Contributions
 
 Please feel free to contribute, be it with Issues or Pull Requests! Please read
 the [Contribution guidelines](CONTRIBUTING.md)
 
 ## Supporting
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: onyx-client Version: 7.0.0 Summary: HTTP Client for
+Metadata-Version: 2.1 Name: onyx-client Version: 7.1.0 Summary: HTTP Client for
 Hella's ONYX.CENTER API. Home-page: https://github.com/muhlba91/onyx-client
 License: MIT Keywords: hella-info,onyx,onyx-center Author: Daniel Muehlbachler-
 Pietrzykowski Author-email: daniel.muehlbachler@niftyside.io Requires-Python:
 >=3.11,<4.0 Classifier: Development Status :: 5 - Production/Stable Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.11
@@ -66,15 +66,12 @@
 run flakehell lint ``` ### Building This package uses [poetry-dynamic-
 versioning](https://github.com/mtkennerly/poetry-dynamic-versioning) which
 infers the version number based on the Git tags. Hence, to have a proper
 versioning for the distribution, use Python's build system like: ```bash pip
 install build python -m build ``` Your distribution will be in the `dist`
 directory. ### Commit Message This project follows [Conventional Commits]
 (https://www.conventionalcommits.org/), and your commit message must also
-adhere to the additional rules outlined in `.conform.yaml`. --- ## Release To
-draft a release, use [standard-version](https://github.com/conventional-
-changelog/standard-version): ```bash standard-version # alternatively npx
-standard-version ``` Finally, push with tags: ```bash git push --follow-tags
-``` --- ## Contributions Please feel free to contribute, be it with Issues or
-Pull Requests! Please read the [Contribution guidelines](CONTRIBUTING.md) ##
+adhere to the additional rules outlined in `.conform.yaml`. --- ##
+Contributions Please feel free to contribute, be it with Issues or Pull
+Requests! Please read the [Contribution guidelines](CONTRIBUTING.md) ##
 Supporting If you enjoy the application and want to support my efforts, please
 feel free to buy me a coffe. :) [Buy_Me_A_Coffee]
```

