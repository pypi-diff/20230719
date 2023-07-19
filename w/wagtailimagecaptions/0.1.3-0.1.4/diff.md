# Comparing `tmp/wagtailimagecaptions-0.1.3.tar.gz` & `tmp/wagtailimagecaptions-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtailimagecaptions-0.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "wagtailimagecaptions-0.1.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `wagtailimagecaptions-0.1.3.tar` & `wagtailimagecaptions-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0     1535 2023-07-12 15:23:46.552175 wagtailimagecaptions-0.1.3/LICENSE
--rw-r--r--   0        0        0     1475 2023-07-14 13:50:22.365434 wagtailimagecaptions-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-07-13 14:44:01.512371 wagtailimagecaptions-0.1.3/media/.gitkeep
--rw-r--r--   0        0        0     1203 2023-07-14 11:29:58.621176 wagtailimagecaptions-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      745 2023-07-12 20:59:42.949204 wagtailimagecaptions-0.1.3/setup.cfg
--rw-r--r--   0        0        0      164 2023-07-15 12:16:33.025900 wagtailimagecaptions-0.1.3/src/wagtailimagecaptions/__init__.py
--rw-r--r--   0        0        0      303 2023-07-13 14:41:40.271684 wagtailimagecaptions-0.1.3/src/wagtailimagecaptions/apps.py
--rw-r--r--   0        0        0     5372 2023-07-13 18:39:44.969787 wagtailimagecaptions-0.1.3/src/wagtailimagecaptions/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-07-13 18:39:44.859852 wagtailimagecaptions-0.1.3/src/wagtailimagecaptions/migrations/__init__.py
--rw-r--r--   0        0        0     1309 2023-07-13 20:26:51.640869 wagtailimagecaptions-0.1.3/src/wagtailimagecaptions/models.py
--rw-r--r--   0        0        0     2957 2023-07-13 20:46:08.375450 wagtailimagecaptions-0.1.3/src/wagtailimagecaptions/services.py
--rw-r--r--   0        0        0     1123 2023-07-15 12:07:14.107381 wagtailimagecaptions-0.1.3/src/wagtailimagecaptions/signals.py
--rw-r--r--   0        0        0        0 2023-07-12 16:59:49.767369 wagtailimagecaptions-0.1.3/test_project/__init__.py
--rw-r--r--   0        0        0      401 2023-07-12 16:59:49.936484 wagtailimagecaptions-0.1.3/test_project/asgi.py
--rw-r--r--   0        0        0     3859 2023-07-13 18:39:25.980594 wagtailimagecaptions-0.1.3/test_project/settings.py
--rw-r--r--   0        0        0      571 2023-07-13 18:51:17.131227 wagtailimagecaptions-0.1.3/test_project/urls.py
--rw-r--r--   0        0        0      401 2023-07-12 16:59:49.939984 wagtailimagecaptions-0.1.3/test_project/wsgi.py
--rw-r--r--   0        0        0     2291 1970-01-01 00:00:00.000000 wagtailimagecaptions-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1535 2023-07-12 15:23:46.552175 wagtailimagecaptions-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1475 2023-07-14 13:50:22.365434 wagtailimagecaptions-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-07-13 14:44:01.512371 wagtailimagecaptions-0.1.4/media/.gitkeep
+-rw-r--r--   0        0        0     1203 2023-07-14 11:29:58.621176 wagtailimagecaptions-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      745 2023-07-12 20:59:42.949204 wagtailimagecaptions-0.1.4/setup.cfg
+-rw-r--r--   0        0        0      164 2023-07-19 11:13:29.102476 wagtailimagecaptions-0.1.4/src/wagtailimagecaptions/__init__.py
+-rw-r--r--   0        0        0      303 2023-07-13 14:41:40.271684 wagtailimagecaptions-0.1.4/src/wagtailimagecaptions/apps.py
+-rw-r--r--   0        0        0     5372 2023-07-13 18:39:44.969787 wagtailimagecaptions-0.1.4/src/wagtailimagecaptions/migrations/0001_initial.py
+-rw-r--r--   0        0        0      352 2023-07-19 11:10:26.633109 wagtailimagecaptions-0.1.4/src/wagtailimagecaptions/migrations/0002_rename_extendedrendition_captionedrendition.py
+-rw-r--r--   0        0        0        0 2023-07-13 18:39:44.859852 wagtailimagecaptions-0.1.4/src/wagtailimagecaptions/migrations/__init__.py
+-rw-r--r--   0        0        0     1310 2023-07-19 11:06:54.268437 wagtailimagecaptions-0.1.4/src/wagtailimagecaptions/models.py
+-rw-r--r--   0        0        0     2957 2023-07-13 20:46:08.375450 wagtailimagecaptions-0.1.4/src/wagtailimagecaptions/services.py
+-rw-r--r--   0        0        0     1123 2023-07-15 12:07:14.107381 wagtailimagecaptions-0.1.4/src/wagtailimagecaptions/signals.py
+-rw-r--r--   0        0        0        0 2023-07-12 16:59:49.767369 wagtailimagecaptions-0.1.4/test_project/__init__.py
+-rw-r--r--   0        0        0      401 2023-07-12 16:59:49.936484 wagtailimagecaptions-0.1.4/test_project/asgi.py
+-rw-r--r--   0        0        0     3859 2023-07-13 18:39:25.980594 wagtailimagecaptions-0.1.4/test_project/settings.py
+-rw-r--r--   0        0        0      571 2023-07-13 18:51:17.131227 wagtailimagecaptions-0.1.4/test_project/urls.py
+-rw-r--r--   0        0        0      401 2023-07-12 16:59:49.939984 wagtailimagecaptions-0.1.4/test_project/wsgi.py
+-rw-r--r--   0        0        0     2291 1970-01-01 00:00:00.000000 wagtailimagecaptions-0.1.4/PKG-INFO
```

### Comparing `wagtailimagecaptions-0.1.3/LICENSE` & `wagtailimagecaptions-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtailimagecaptions-0.1.3/README.md` & `wagtailimagecaptions-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `wagtailimagecaptions-0.1.3/pyproject.toml` & `wagtailimagecaptions-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wagtailimagecaptions-0.1.3/setup.cfg` & `wagtailimagecaptions-0.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `wagtailimagecaptions-0.1.3/src/wagtailimagecaptions/migrations/0001_initial.py` & `wagtailimagecaptions-0.1.4/src/wagtailimagecaptions/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtailimagecaptions-0.1.3/src/wagtailimagecaptions/models.py` & `wagtailimagecaptions-0.1.4/src/wagtailimagecaptions/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,12 +28,12 @@
     def default_alt_text(self):
         """ Return our stored alt value, otherwise Wagtail defaults to the title. """
         if self.alt:
             return self.alt
         return super().default_alt_text
 
 
-class ExtendedRendition(AbstractRendition):
+class CaptionedRendition(AbstractRendition):
     image = models.ForeignKey(CaptionedImage, on_delete=models.CASCADE, related_name="renditions")
 
     class Meta:
         unique_together = (("image", "filter_spec", "focal_point_key"),)
```

### Comparing `wagtailimagecaptions-0.1.3/src/wagtailimagecaptions/services.py` & `wagtailimagecaptions-0.1.4/src/wagtailimagecaptions/services.py`

 * *Files identical despite different names*

### Comparing `wagtailimagecaptions-0.1.3/src/wagtailimagecaptions/signals.py` & `wagtailimagecaptions-0.1.4/src/wagtailimagecaptions/signals.py`

 * *Files identical despite different names*

### Comparing `wagtailimagecaptions-0.1.3/test_project/settings.py` & `wagtailimagecaptions-0.1.4/test_project/settings.py`

 * *Files identical despite different names*

### Comparing `wagtailimagecaptions-0.1.3/test_project/urls.py` & `wagtailimagecaptions-0.1.4/test_project/urls.py`

 * *Files identical despite different names*

### Comparing `wagtailimagecaptions-0.1.3/PKG-INFO` & `wagtailimagecaptions-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtailimagecaptions
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Django app for extending the Wagtail Image model to add captions and alt fields as
 Author-email: Stephan Rohde <appsupport@newshour.org>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

