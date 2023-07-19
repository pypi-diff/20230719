# Comparing `tmp/pixel-font-builder-0.0.3.tar.gz` & `tmp/pixel-font-builder-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixel-font-builder-0.0.3.tar", last modified: Tue Jul 11 15:48:43 2023, max compression
+gzip compressed data, was "pixel-font-builder-0.0.4.tar", last modified: Wed Jul 19 15:18:55 2023, max compression
```

## Comparing `pixel-font-builder-0.0.3.tar` & `pixel-font-builder-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:48:43.380712 pixel-font-builder-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-11 15:48:33.000000 pixel-font-builder-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-07-11 15:48:43.380712 pixel-font-builder-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-07-11 15:48:33.000000 pixel-font-builder-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-11 15:48:33.000000 pixel-font-builder-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 15:48:43.380712 pixel-font-builder-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:48:43.376712 pixel-font-builder-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:48:43.376712 pixel-font-builder-0.0.3/src/pixel_font_builder/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-11 15:48:33.000000 pixel-font-builder-0.0.3/src/pixel_font_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-07-11 15:48:33.000000 pixel-font-builder-0.0.3/src/pixel_font_builder/bdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-07-11 15:48:33.000000 pixel-font-builder-0.0.3/src/pixel_font_builder/font.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-11 15:48:33.000000 pixel-font-builder-0.0.3/src/pixel_font_builder/glyph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-11 15:48:33.000000 pixel-font-builder-0.0.3/src/pixel_font_builder/info.py
--rw-r--r--   0 runner    (1001) docker     (123)    10939 2023-07-11 15:48:33.000000 pixel-font-builder-0.0.3/src/pixel_font_builder/opentype.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:48:43.380712 pixel-font-builder-0.0.3/src/pixel_font_builder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-07-11 15:48:43.000000 pixel-font-builder-0.0.3/src/pixel_font_builder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-11 15:48:43.000000 pixel-font-builder-0.0.3/src/pixel_font_builder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 15:48:43.000000 pixel-font-builder-0.0.3/src/pixel_font_builder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-11 15:48:43.000000 pixel-font-builder-0.0.3/src/pixel_font_builder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-11 15:48:43.000000 pixel-font-builder-0.0.3/src/pixel_font_builder.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:48:43.380712 pixel-font-builder-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-11 15:48:33.000000 pixel-font-builder-0.0.3/tests/test_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:18:55.276489 pixel-font-builder-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-19 15:18:43.000000 pixel-font-builder-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-07-19 15:18:55.276489 pixel-font-builder-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-07-19 15:18:43.000000 pixel-font-builder-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-19 15:18:43.000000 pixel-font-builder-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 15:18:55.276489 pixel-font-builder-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:18:55.272489 pixel-font-builder-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:18:55.276489 pixel-font-builder-0.0.4/src/pixel_font_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-19 15:18:43.000000 pixel-font-builder-0.0.4/src/pixel_font_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-07-19 15:18:43.000000 pixel-font-builder-0.0.4/src/pixel_font_builder/bdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-07-19 15:18:43.000000 pixel-font-builder-0.0.4/src/pixel_font_builder/font.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-19 15:18:43.000000 pixel-font-builder-0.0.4/src/pixel_font_builder/glyph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-19 15:18:43.000000 pixel-font-builder-0.0.4/src/pixel_font_builder/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13161 2023-07-19 15:18:43.000000 pixel-font-builder-0.0.4/src/pixel_font_builder/opentype.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:18:55.276489 pixel-font-builder-0.0.4/src/pixel_font_builder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-07-19 15:18:55.000000 pixel-font-builder-0.0.4/src/pixel_font_builder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-19 15:18:55.000000 pixel-font-builder-0.0.4/src/pixel_font_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 15:18:55.000000 pixel-font-builder-0.0.4/src/pixel_font_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-19 15:18:55.000000 pixel-font-builder-0.0.4/src/pixel_font_builder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-19 15:18:55.000000 pixel-font-builder-0.0.4/src/pixel_font_builder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:18:55.276489 pixel-font-builder-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-19 15:18:43.000000 pixel-font-builder-0.0.4/tests/test_.py
```

### Comparing `pixel-font-builder-0.0.3/LICENSE` & `pixel-font-builder-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pixel-font-builder-0.0.3/PKG-INFO` & `pixel-font-builder-0.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixel-font-builder
-Version: 0.0.3
+Version: 0.0.4
 Summary: A library that helps create pixel style fonts.
 Author: TakWolf
 Maintainer: TakWolf
 License: MIT License
 Project-URL: homepage, https://github.com/TakWolf/pixel-font-builder
 Project-URL: source, https://github.com/TakWolf/pixel-font-builder
 Project-URL: issues, https://github.com/TakWolf/pixel-font-builder/issues
@@ -21,15 +21,15 @@
 [![Python](https://img.shields.io/badge/python-3.11-brightgreen)](https://www.python.org)
 [![PyPI](https://img.shields.io/pypi/v/pixel-font-builder)](https://pypi.org/project/pixel-font-builder/)
 
 A library that helps create pixel style fonts.
 
 ## Installation
 
-```commandline
+```shell
 pip install pixel-font-builder
 ```
 
 ## Usage
 
 ```python
 import logging
@@ -102,14 +102,15 @@
     builder.meta_infos.designer = 'TakWolf'
     builder.meta_infos.description = 'A demo pixel font.'
     builder.meta_infos.copyright_info = 'Copyright (c) TakWolf'
     builder.meta_infos.license_info = 'This Font Software is licensed under the SIL Open Font License, Version 1.1.'
     builder.meta_infos.vendor_url = 'https://github.com/TakWolf/pixel-font-builder'
     builder.meta_infos.designer_url = 'https://takwolf.com'
     builder.meta_infos.license_url = 'https://scripts.sil.org/OFL'
+    builder.meta_infos.sample_text = 'Hello World!'
 
     builder.save_otf(os.path.join(outputs_dir, 'demo.otf'))
     builder.save_otf(os.path.join(outputs_dir, 'demo.woff2'), flavor=opentype.Flavor.WOFF2)
     builder.save_ttf(os.path.join(outputs_dir, 'demo.ttf'))
     builder.save_bdf(os.path.join(outputs_dir, 'demo.bdf'))
```

### Comparing `pixel-font-builder-0.0.3/README.md` & `pixel-font-builder-0.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [![Python](https://img.shields.io/badge/python-3.11-brightgreen)](https://www.python.org)
 [![PyPI](https://img.shields.io/pypi/v/pixel-font-builder)](https://pypi.org/project/pixel-font-builder/)
 
 A library that helps create pixel style fonts.
 
 ## Installation
 
-```commandline
+```shell
 pip install pixel-font-builder
 ```
 
 ## Usage
 
 ```python
 import logging
@@ -84,14 +84,15 @@
     builder.meta_infos.designer = 'TakWolf'
     builder.meta_infos.description = 'A demo pixel font.'
     builder.meta_infos.copyright_info = 'Copyright (c) TakWolf'
     builder.meta_infos.license_info = 'This Font Software is licensed under the SIL Open Font License, Version 1.1.'
     builder.meta_infos.vendor_url = 'https://github.com/TakWolf/pixel-font-builder'
     builder.meta_infos.designer_url = 'https://takwolf.com'
     builder.meta_infos.license_url = 'https://scripts.sil.org/OFL'
+    builder.meta_infos.sample_text = 'Hello World!'
 
     builder.save_otf(os.path.join(outputs_dir, 'demo.otf'))
     builder.save_otf(os.path.join(outputs_dir, 'demo.woff2'), flavor=opentype.Flavor.WOFF2)
     builder.save_ttf(os.path.join(outputs_dir, 'demo.ttf'))
     builder.save_bdf(os.path.join(outputs_dir, 'demo.bdf'))
```

### Comparing `pixel-font-builder-0.0.3/pyproject.toml` & `pixel-font-builder-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pixel-font-builder"
-version = "0.0.3"
+version = "0.0.4"
 description = "A library that helps create pixel style fonts."
 readme = "README.md"
 license = { text = "MIT License" }
 requires-python = ">=3.11"
 authors = [
     { name = "TakWolf" },
 ]
@@ -15,15 +15,15 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
-    "fonttools>=4.40.0",
+    "fonttools>=4.41.0",
     "Brotli>=1.0.9",
     "bdffont>=0.0.13",
 ]
 
 [project.urls]
 homepage = "https://github.com/TakWolf/pixel-font-builder"
 source = "https://github.com/TakWolf/pixel-font-builder"
```

### Comparing `pixel-font-builder-0.0.3/src/pixel_font_builder/bdf.py` & `pixel-font-builder-0.0.4/src/pixel_font_builder/bdf.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+import logging
 import math
 
 from bdffont import BdfFont, BdfGlyph, xlfd
 
 from pixel_font_builder import font
 from pixel_font_builder.info import SerifMode, WidthMode
 
+logger = logging.getLogger('pixel_font_builder.bdf')
+
 
 class Configs:
     def __init__(
             self,
             resolution_x: int = 75,
             resolution_y: int = 75,
     ):
@@ -27,27 +30,31 @@
         bounding_box_size=glyph.size,
         bounding_box_offset=glyph.offset,
         bitmap=glyph.data,
     )
 
 
 def create_builder(context: 'font.FontBuilder') -> BdfFont:
+    logger.debug("Create 'BDFBuilder': %s", context.meta_infos.family_name)
     context.check_ready()
 
     builder = BdfFont(
         point_size=context.size,
         resolution_xy=(context.bdf_configs.resolution_x, context.bdf_configs.resolution_y),
         bounding_box_size=(context.size, context.line_height),
         bounding_box_offset=(0, context.descent),
     )
 
+    logger.debug("Add 'Glyph': %s", '.notdef')
     builder.add_glyph(_create_glyph(context, -1, '.notdef'))
     for code_point, glyph_name in context.character_mapping.items():
+        logger.debug("Add 'Glyph': %s", glyph_name)
         builder.add_glyph(_create_glyph(context, code_point, glyph_name))
 
+    logger.debug("Setup 'Properties'")
     builder.properties.foundry = context.meta_infos.manufacturer
     builder.properties.family_name = context.meta_infos.family_name
     builder.properties.weight_name = context.meta_infos.style_name
     builder.properties.slant = xlfd.Slant.ROMAN
     builder.properties.setwidth_name = xlfd.SetwidthName.NORMAL
     if context.meta_infos.serif_mode == SerifMode.SERIF:
         builder.properties.add_style_name = xlfd.AddStyleName.SERIF
@@ -77,8 +84,9 @@
 
     builder.properties.font_version = context.meta_infos.version
     builder.properties.copyright = context.meta_infos.copyright_info
     builder.properties['LICENSE'] = context.meta_infos.license_info
 
     builder.generate_xlfd_font_name()
 
+    logger.debug("Create 'BDFBuilder' finished")
     return builder
```

### Comparing `pixel-font-builder-0.0.3/src/pixel_font_builder/font.py` & `pixel-font-builder-0.0.4/src/pixel_font_builder/font.py`

 * *Files identical despite different names*

### Comparing `pixel-font-builder-0.0.3/src/pixel_font_builder/glyph.py` & `pixel-font-builder-0.0.4/src/pixel_font_builder/glyph.py`

 * *Files identical despite different names*

### Comparing `pixel-font-builder-0.0.3/src/pixel_font_builder/info.py` & `pixel-font-builder-0.0.4/src/pixel_font_builder/info.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,21 +32,23 @@
             designer: str = None,
             description: str = None,
             copyright_info: str = None,
             license_info: str = None,
             vendor_url: str = None,
             designer_url: str = None,
             license_url: str = None,
+            sample_text: str = None,
     ):
         self.version = version
         self.family_name = family_name
         self.style_name = style_name
         self.serif_mode = serif_mode
         self.width_mode = width_mode
         self.manufacturer = manufacturer
         self.designer = designer
         self.description = description
         self.copyright_info = copyright_info
         self.license_info = license_info
         self.vendor_url = vendor_url
         self.designer_url = designer_url
         self.license_url = license_url
+        self.sample_text = sample_text
```

### Comparing `pixel-font-builder-0.0.3/src/pixel_font_builder/opentype.py` & `pixel-font-builder-0.0.4/src/pixel_font_builder/opentype.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,26 @@
+import logging
 from enum import StrEnum
 
 from fontTools.fontBuilder import FontBuilder
-from fontTools.misc.psCharStrings import T2CharString
-from fontTools.pens.t2CharStringPen import T2CharStringPen
-from fontTools.pens.ttGlyphPen import TTGlyphPen
-from fontTools.ttLib.tables._g_l_y_f import Glyph
+from fontTools.misc.psCharStrings import T2CharString as OTFGlyph
+from fontTools.pens.t2CharStringPen import T2CharStringPen as OTFGlyphPen
+from fontTools.pens.ttGlyphPen import TTGlyphPen as TTFGlyphPen
+from fontTools.ttLib.tables._g_l_y_f import Glyph as TTFGlyph
 
 from pixel_font_builder import font
+from pixel_font_builder.glyph import Glyph
+from pixel_font_builder.info import MetaInfos
+
+logger = logging.getLogger('pixel_font_builder.opentype')
+
+_CACHE_NAME_TAG = '_opentype_cache_tag'
+_CACHE_NAME_OUTLINES = '_opentype_cache_outlines'
+_CACHE_NAME_OTF_GLYPH = '_opentype_cache_otf_glyph'
+_CACHE_NAME_TTF_GLYPH = '_opentype_cache_ttf_glyph'
 
 
 class Configs:
     def __init__(
             self,
             px_to_units: int = 100,
     ):
@@ -18,16 +28,17 @@
 
 
 class Flavor(StrEnum):
     WOFF = 'woff'
     WOFF2 = 'woff2'
 
 
-def _create_name_strings(context: 'font.FontBuilder') -> dict[str, str]:
+def _create_name_strings(meta_infos: MetaInfos) -> dict[str, str]:
     """
+    https://learn.microsoft.com/en-us/typography/opentype/spec/name#name-ids
     copyright (nameID 0)
     familyName (nameID 1)
     styleName (nameID 2)
     uniqueFontIdentifier (nameID 3)
     fullName (nameID 4)
     version (nameID 5)
     psName (nameID 6)
@@ -46,43 +57,45 @@
     postScriptCIDFindfontName (nameID 20)
     wwsFamilyName (nameID 21)
     wwsSubfamilyName (nameID 22)
     lightBackgroundPalette (nameID 23)
     darkBackgroundPalette (nameID 24)
     variationsPostScriptNamePrefix (nameID 25)
     """
-    unique_name = context.meta_infos.family_name.replace(' ', '-')
+    unique_name = meta_infos.family_name.replace(' ', '-')
     name_strings = {
-        'familyName': context.meta_infos.family_name,
-        'styleName': context.meta_infos.style_name,
-        'uniqueFontIdentifier': f'{unique_name}-{context.meta_infos.style_name};{context.meta_infos.version}',
-        'fullName': context.meta_infos.family_name,
-        'version': context.meta_infos.version,
-        'psName': f'{unique_name}-{context.meta_infos.style_name}',
+        'familyName': meta_infos.family_name,
+        'styleName': meta_infos.style_name,
+        'uniqueFontIdentifier': f'{unique_name}-{meta_infos.style_name};{meta_infos.version}',
+        'fullName': meta_infos.family_name,
+        'version': meta_infos.version,
+        'psName': f'{unique_name}-{meta_infos.style_name}',
     }
-    if context.meta_infos.copyright_info is not None:
-        name_strings['copyright'] = context.meta_infos.copyright_info
-    if context.meta_infos.manufacturer is not None:
-        name_strings['manufacturer'] = context.meta_infos.manufacturer
-    if context.meta_infos.designer is not None:
-        name_strings['designer'] = context.meta_infos.designer
-    if context.meta_infos.description is not None:
-        name_strings['description'] = context.meta_infos.description
-    if context.meta_infos.vendor_url is not None:
-        name_strings['vendorURL'] = context.meta_infos.vendor_url
-    if context.meta_infos.designer_url is not None:
-        name_strings['designerURL'] = context.meta_infos.designer_url
-    if context.meta_infos.license_info is not None:
-        name_strings['licenseDescription'] = context.meta_infos.license_info
-    if context.meta_infos.license_url is not None:
-        name_strings['licenseInfoURL'] = context.meta_infos.license_url
+    if meta_infos.copyright_info is not None:
+        name_strings['copyright'] = meta_infos.copyright_info
+    if meta_infos.manufacturer is not None:
+        name_strings['manufacturer'] = meta_infos.manufacturer
+    if meta_infos.designer is not None:
+        name_strings['designer'] = meta_infos.designer
+    if meta_infos.description is not None:
+        name_strings['description'] = meta_infos.description
+    if meta_infos.vendor_url is not None:
+        name_strings['vendorURL'] = meta_infos.vendor_url
+    if meta_infos.designer_url is not None:
+        name_strings['designerURL'] = meta_infos.designer_url
+    if meta_infos.license_info is not None:
+        name_strings['licenseDescription'] = meta_infos.license_info
+    if meta_infos.license_url is not None:
+        name_strings['licenseInfoURL'] = meta_infos.license_url
+    if meta_infos.sample_text is not None:
+        name_strings['sampleText'] = meta_infos.sample_text
     return name_strings
 
 
-def _get_outlines(glyph_data: list[list[int]], px_to_units: int) -> list[list[tuple[int, int]]]:
+def _create_outlines(glyph_data: list[list[int]], px_to_units: int) -> list[list[tuple[int, int]]]:
     """
     将字形数据转换为轮廓数据，左上角原点坐标系
     """
     # 相邻像素分组
     point_group_list = []
     for y, glyph_data_row in enumerate(glyph_data):
         for x, alpha in enumerate(glyph_data_row):
@@ -162,29 +175,27 @@
             if (x == xl and x == xr) or (y == yl and y == yr):
                 solved_line_segment.pop()
             # 添加到轮廓
             outlines.append(solved_line_segment)
     return outlines
 
 
-def _create_glyph(context: 'font.FontBuilder', glyph_name: str, is_ttf: bool) -> T2CharString | Glyph:
-    glyph = context.get_glyph(glyph_name)
-    outlines = _get_outlines(glyph.data, context.opentype_configs.px_to_units)
+def _create_glyph(outlines: list[list[tuple[int, int]]], glyph: Glyph, px_to_units: int, is_ttf: bool) -> OTFGlyph | TTFGlyph:
     if is_ttf:
-        pen = TTGlyphPen()
+        pen = TTFGlyphPen()
     else:
-        pen = T2CharStringPen(glyph.advance_width * context.opentype_configs.px_to_units, None)
+        pen = OTFGlyphPen(glyph.advance_width * px_to_units, None)
     if len(outlines) > 0:
         for outline_index, outline in enumerate(outlines):
             for point_index, point in enumerate(outline):
 
                 # 转换左上角原点坐标系为左下角原点坐标系
                 x, y = point
-                x += glyph.offset_x * context.opentype_configs.px_to_units
-                y = (glyph.height + glyph.offset_y) * context.opentype_configs.px_to_units - y
+                x += glyph.offset_x * px_to_units
+                y = (glyph.height + glyph.offset_y) * px_to_units - y
                 point = x, y
 
                 if point_index == 0:
                     pen.moveTo(point)
                 else:
                     pen.lineTo(point)
             if outline_index < len(outlines) - 1:
@@ -197,61 +208,101 @@
     if is_ttf:
         return pen.glyph()
     else:
         return pen.getCharString()
 
 
 def create_builder(context: 'font.FontBuilder', is_ttf: bool, flavor: Flavor) -> FontBuilder:
+    xtf_name = 'TTF' if is_ttf else 'OTF'
+
+    logger.debug("Create '%sBuilder': %s", xtf_name, context.meta_infos.family_name)
     context.check_ready()
 
     units_per_em = context.size * context.opentype_configs.px_to_units
     builder = FontBuilder(units_per_em, isTTF=is_ttf)
 
-    name_strings = _create_name_strings(context)
+    logger.debug("Setup 'Name Strings'")
+    name_strings = _create_name_strings(context.meta_infos)
     builder.setupNameTable(name_strings)
 
+    logger.debug("Setup 'Glyph Order'")
     glyph_order = ['.notdef']
     for _, glyph_name in context.get_character_mapping_sequence():
         if glyph_name not in glyph_order:
             glyph_order.append(glyph_name)
     builder.setupGlyphOrder(glyph_order)
+    logger.debug("Setup 'Character Mapping'")
     builder.setupCharacterMap(context.character_mapping)
 
-    glyphs = {glyph_name: _create_glyph(context, glyph_name, is_ttf) for glyph_name in glyph_order}
+    logger.debug("Setup 'Glyphs'")
+    glyphs = {}
+    for glyph_name in glyph_order:
+        glyph_context = context.get_glyph(glyph_name)
+
+        cache_tag = f'{glyph_context.advance_width}#{glyph_context.offset}#{glyph_context.data}'.replace(' ', '')
+        if getattr(glyph_context, _CACHE_NAME_TAG, None) != cache_tag:
+            setattr(glyph_context, _CACHE_NAME_OUTLINES, None)
+            setattr(glyph_context, _CACHE_NAME_OTF_GLYPH, None)
+            setattr(glyph_context, _CACHE_NAME_TTF_GLYPH, None)
+            setattr(glyph_context, _CACHE_NAME_TAG, cache_tag)
+
+        outlines = getattr(glyph_context, _CACHE_NAME_OUTLINES, None)
+        if outlines is None:
+            logger.debug("Create 'Outlines': %s", glyph_context.name)
+            outlines = _create_outlines(glyph_context.data, context.opentype_configs.px_to_units)
+            setattr(glyph_context, _CACHE_NAME_OUTLINES, outlines)
+        else:
+            logger.debug("Use cached 'Outlines': %s", glyph_context.name)
+
+        cache_name_xtf_glyph = _CACHE_NAME_TTF_GLYPH if is_ttf else _CACHE_NAME_OTF_GLYPH
+        glyph = getattr(glyph_context, cache_name_xtf_glyph, None)
+        if glyph is None:
+            logger.debug("Create '%sGlyph': %s", xtf_name, glyph_context.name)
+            glyph = _create_glyph(outlines, glyph_context, context.opentype_configs.px_to_units, is_ttf)
+            setattr(glyph_context, cache_name_xtf_glyph, glyph)
+        else:
+            logger.debug("Use cached '%sGlyph': %s", xtf_name, glyph_context.name)
+        glyphs[glyph_name] = glyph
     if is_ttf:
         builder.setupGlyf(glyphs)
     else:
         builder.setupCFF(name_strings['psName'], {'FullName': name_strings['fullName']}, glyphs, {})
 
+    logger.debug("Setup 'Horizontal Metrics'")
     horizontal_metrics = {}
     for glyph_name in glyph_order:
         advance_width = context.get_glyph(glyph_name).advance_width * context.opentype_configs.px_to_units
         if is_ttf:
             lsb = glyphs[glyph_name].xMin
         else:
             lsb = glyphs[glyph_name].calcBounds(None)[0]
         horizontal_metrics[glyph_name] = advance_width, lsb
     builder.setupHorizontalMetrics(horizontal_metrics)
 
     ascent = context.ascent * context.opentype_configs.px_to_units
     descent = context.descent * context.opentype_configs.px_to_units
     x_height = context.x_height * context.opentype_configs.px_to_units if context.x_height is not None else None
     cap_height = context.cap_height * context.opentype_configs.px_to_units if context.cap_height is not None else None
+    logger.debug("Setup 'Horizontal Header'")
     builder.setupHorizontalHeader(
         ascent=ascent,
         descent=descent,
     )
+    logger.debug("Setup 'OS2'")
     builder.setupOS2(
         sTypoAscender=ascent,
         sTypoDescender=descent,
         usWinAscent=ascent,
         usWinDescent=-descent,
         sxHeight=x_height,
         sCapHeight=cap_height,
     )
 
+    logger.debug("Setup 'Post'")
     builder.setupPost()
 
     if flavor is not None:
+        logger.debug("Setup 'Flavor': %s", flavor)
         builder.font.flavor = flavor
 
+    logger.debug("Create '%sBuilder' finished", xtf_name)
     return builder
```

### Comparing `pixel-font-builder-0.0.3/src/pixel_font_builder.egg-info/PKG-INFO` & `pixel-font-builder-0.0.4/src/pixel_font_builder.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixel-font-builder
-Version: 0.0.3
+Version: 0.0.4
 Summary: A library that helps create pixel style fonts.
 Author: TakWolf
 Maintainer: TakWolf
 License: MIT License
 Project-URL: homepage, https://github.com/TakWolf/pixel-font-builder
 Project-URL: source, https://github.com/TakWolf/pixel-font-builder
 Project-URL: issues, https://github.com/TakWolf/pixel-font-builder/issues
@@ -21,15 +21,15 @@
 [![Python](https://img.shields.io/badge/python-3.11-brightgreen)](https://www.python.org)
 [![PyPI](https://img.shields.io/pypi/v/pixel-font-builder)](https://pypi.org/project/pixel-font-builder/)
 
 A library that helps create pixel style fonts.
 
 ## Installation
 
-```commandline
+```shell
 pip install pixel-font-builder
 ```
 
 ## Usage
 
 ```python
 import logging
@@ -102,14 +102,15 @@
     builder.meta_infos.designer = 'TakWolf'
     builder.meta_infos.description = 'A demo pixel font.'
     builder.meta_infos.copyright_info = 'Copyright (c) TakWolf'
     builder.meta_infos.license_info = 'This Font Software is licensed under the SIL Open Font License, Version 1.1.'
     builder.meta_infos.vendor_url = 'https://github.com/TakWolf/pixel-font-builder'
     builder.meta_infos.designer_url = 'https://takwolf.com'
     builder.meta_infos.license_url = 'https://scripts.sil.org/OFL'
+    builder.meta_infos.sample_text = 'Hello World!'
 
     builder.save_otf(os.path.join(outputs_dir, 'demo.otf'))
     builder.save_otf(os.path.join(outputs_dir, 'demo.woff2'), flavor=opentype.Flavor.WOFF2)
     builder.save_ttf(os.path.join(outputs_dir, 'demo.ttf'))
     builder.save_bdf(os.path.join(outputs_dir, 'demo.bdf'))
```

