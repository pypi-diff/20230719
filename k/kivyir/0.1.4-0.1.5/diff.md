# Comparing `tmp/kivyir-0.1.4.tar.gz` & `tmp/kivyir-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\kivyir-0.1.4.tar", last modified: Sun Jul 16 07:53:33 2023, max compression
+gzip compressed data, was "dist\kivyir-0.1.5.tar", last modified: Wed Jul 19 13:21:23 2023, max compression
```

## Comparing `kivyir-0.1.4.tar` & `kivyir-0.1.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 07:53:33.000000 kivyir-0.1.4/
--rw-rw-rw-   0        0        0     1069 2023-07-14 09:57:59.000000 kivyir-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     2755 2023-07-16 07:53:33.000000 kivyir-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1487 2023-07-14 09:57:59.000000 kivyir-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-16 07:53:33.000000 kivyir-0.1.4/kivyir/
--rw-rw-rw-   0        0        0    26727 2023-07-16 07:52:04.000000 kivyir-0.1.4/kivyir/ConfigBase.py
--rw-rw-rw-   0        0        0      422 2023-07-14 09:57:59.000000 kivyir-0.1.4/kivyir/IrLabel.py
--rw-rw-rw-   0        0        0     4010 2023-07-14 09:57:59.000000 kivyir-0.1.4/kivyir/IrTextInput.py
--rw-rw-rw-   0        0        0      258 2023-07-14 09:57:59.000000 kivyir-0.1.4/kivyir/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-16 07:53:33.000000 kivyir-0.1.4/kivyir/font/
--rw-rw-rw-   0        0        0    76372 2023-07-14 09:57:59.000000 kivyir-0.1.4/kivyir/font/Sahel-Bold.ttf
--rw-rw-rw-   0        0        0    75308 2023-07-14 09:57:59.000000 kivyir-0.1.4/kivyir/font/Sahel.ttf
-drwxrwxrwx   0        0        0        0 2023-07-16 07:53:33.000000 kivyir-0.1.4/kivyir.egg-info/
--rw-rw-rw-   0        0        0     2755 2023-07-16 07:53:33.000000 kivyir-0.1.4/kivyir.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      317 2023-07-16 07:53:33.000000 kivyir-0.1.4/kivyir.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 07:53:33.000000 kivyir-0.1.4/kivyir.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-07-16 07:53:33.000000 kivyir-0.1.4/kivyir.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-16 07:53:33.000000 kivyir-0.1.4/kivyir.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-16 07:53:33.000000 kivyir-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1714 2023-07-16 07:25:57.000000 kivyir-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-16 07:53:33.000000 kivyir-0.1.4/test/
--rw-rw-rw-   0        0        0     1216 2023-07-16 07:32:53.000000 kivyir-0.1.4/test/main.py
+drwxrwxrwx   0        0        0        0 2023-07-19 13:21:23.000000 kivyir-0.1.5/
+-rw-rw-rw-   0        0        0     1069 2023-07-14 09:57:59.000000 kivyir-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     2755 2023-07-19 13:21:23.000000 kivyir-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1487 2023-07-14 09:57:59.000000 kivyir-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-19 13:21:23.000000 kivyir-0.1.5/kivyir/
+-rw-rw-rw-   0        0        0    26602 2023-07-19 13:18:47.000000 kivyir-0.1.5/kivyir/ConfigBase.py
+-rw-rw-rw-   0        0        0      422 2023-07-14 09:57:59.000000 kivyir-0.1.5/kivyir/IrLabel.py
+-rw-rw-rw-   0        0        0     4010 2023-07-14 09:57:59.000000 kivyir-0.1.5/kivyir/IrTextInput.py
+-rw-rw-rw-   0        0        0      258 2023-07-14 09:57:59.000000 kivyir-0.1.5/kivyir/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 13:21:23.000000 kivyir-0.1.5/kivyir/font/
+-rw-rw-rw-   0        0        0    76372 2023-07-14 09:57:59.000000 kivyir-0.1.5/kivyir/font/Sahel-Bold.ttf
+-rw-rw-rw-   0        0        0    75308 2023-07-14 09:57:59.000000 kivyir-0.1.5/kivyir/font/Sahel.ttf
+drwxrwxrwx   0        0        0        0 2023-07-19 13:21:23.000000 kivyir-0.1.5/kivyir.egg-info/
+-rw-rw-rw-   0        0        0     2755 2023-07-19 13:21:23.000000 kivyir-0.1.5/kivyir.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2023-07-19 13:21:23.000000 kivyir-0.1.5/kivyir.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 13:21:23.000000 kivyir-0.1.5/kivyir.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-07-19 13:21:23.000000 kivyir-0.1.5/kivyir.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-19 13:21:23.000000 kivyir-0.1.5/kivyir.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-19 13:21:23.000000 kivyir-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1715 2023-07-19 13:20:33.000000 kivyir-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 13:21:23.000000 kivyir-0.1.5/test/
+-rw-rw-rw-   0        0        0     1216 2023-07-16 07:32:53.000000 kivyir-0.1.5/test/main.py
```

### Comparing `kivyir-0.1.4/LICENSE` & `kivyir-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kivyir-0.1.4/PKG-INFO` & `kivyir-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kivyir
-Version: 0.1.4
+Version: 0.1.5
 Summary: Improving the display of Persian text for Persian speakers
 Home-page: https://github.com/goldaaa/kivyir
 Download-URL: https://github.com/goldaaa/kivyir/tarball/master
 Author: navid nasiri
 Author-email: goldaaa.program@gmail.com
 Maintainer: navid nasiri
 Maintainer-email: goldaaa.program@gmail.com
```

### Comparing `kivyir-0.1.4/README.md` & `kivyir-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `kivyir-0.1.4/kivyir/ConfigBase.py` & `kivyir-0.1.5/kivyir/ConfigBase.py`

 * *Files 1% similar despite different names*

```diff
@@ -370,17 +370,15 @@
             elif not clipped and item[:8] == '[anchor=':
                 options['_anchor'] = item[8:-1]
             elif not clipped:
                 item = item.replace('&bl;', '[').replace(
                     '&br;', ']').replace('&amp;', '&')
                 if len(item) > 1:
                     item = cleaning(item)
-                    if self.options['font_name'] == 'Roboto':
-                        options['font_name'] = font_name
-                        self.resolve_font_name()
+                    self.resolve_font_name()
                 if not base_dir:
                     base_dir = self._resolved_base_dir = find_base_dir(item)
                 opts = copy(options)
                 extents = self.get_cached_extents()
                 opts['space_width'] = extents(' ')[0]
                 w, h, clipped = layout_text(
                     item, lines, (w, h), (uw_temp, uhh),
```

### Comparing `kivyir-0.1.4/kivyir/IrTextInput.py` & `kivyir-0.1.5/kivyir/IrTextInput.py`

 * *Files identical despite different names*

### Comparing `kivyir-0.1.4/kivyir/font/Sahel-Bold.ttf` & `kivyir-0.1.5/kivyir/font/Sahel-Bold.ttf`

 * *Files identical despite different names*

### Comparing `kivyir-0.1.4/kivyir/font/Sahel.ttf` & `kivyir-0.1.5/kivyir/font/Sahel.ttf`

 * *Files identical despite different names*

### Comparing `kivyir-0.1.4/kivyir.egg-info/PKG-INFO` & `kivyir-0.1.5/kivyir.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kivyir
-Version: 0.1.4
+Version: 0.1.5
 Summary: Improving the display of Persian text for Persian speakers
 Home-page: https://github.com/goldaaa/kivyir
 Download-URL: https://github.com/goldaaa/kivyir/tarball/master
 Author: navid nasiri
 Author-email: goldaaa.program@gmail.com
 Maintainer: navid nasiri
 Maintainer-email: goldaaa.program@gmail.com
```

### Comparing `kivyir-0.1.4/setup.py` & `kivyir-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     long_description = fh.read()
 
 setup(
     name="kivyir",
     description="Improving the display of Persian text for Persian speakers",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version='0.1.4',
+    version='0.1.5',
     platforms="ALL",
     license="MIT",
     packages=['kivyir', 'test'],
     install_requires=["kivy>=2.0.0", "pillow", "facleaning"],
     author="navid nasiri",
     author_email="goldaaa.program@gmail.com",
     maintainer="navid nasiri",
@@ -24,15 +24,15 @@
     package_dir={'kivyir': 'kivyir'},
     test_suite='kivyir.test',
     include_package_data=True,
     keywords="kivy persian farsi iran",
     url="https://github.com/goldaaa/kivyir",
     download_url="https://github.com/goldaaa/kivyir/tarball/master",
     package_data={
-        "kivyir": ["font/*.ttf",]
+        "kivyir": ["font/*.ttf", ]
     },
     setup_requires=[],
     python_requires=">=3.5",
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Intended Audience :: Developers',
         'Natural Language :: Persian',
```

### Comparing `kivyir-0.1.4/test/main.py` & `kivyir-0.1.5/test/main.py`

 * *Files identical despite different names*

