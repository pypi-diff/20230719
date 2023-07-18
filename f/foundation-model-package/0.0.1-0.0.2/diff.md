# Comparing `tmp/foundation-model-package-0.0.1.tar.gz` & `tmp/foundation-model-package-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foundation-model-package-0.0.1.tar", last modified: Tue Jul 18 23:01:31 2023, max compression
+gzip compressed data, was "foundation-model-package-0.0.2.tar", last modified: Tue Jul 18 23:20:06 2023, max compression
```

## Comparing `foundation-model-package-0.0.1.tar` & `foundation-model-package-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 23:01:31.813368 foundation-model-package-0.0.1/
--rw-rw-rw-   0        0        0       36 2023-07-18 17:27:15.000000 foundation-model-package-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      135 2023-07-18 23:01:31.802400 foundation-model-package-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     4117 2023-07-18 17:27:15.000000 foundation-model-package-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-18 23:01:31.660048 foundation-model-package-0.0.1/foundation_model_package.egg-info/
--rw-rw-rw-   0        0        0      135 2023-07-18 23:01:31.000000 foundation-model-package-0.0.1/foundation_model_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      470 2023-07-18 23:01:31.000000 foundation-model-package-0.0.1/foundation_model_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 23:01:31.000000 foundation-model-package-0.0.1/foundation_model_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2023-07-18 23:01:31.000000 foundation-model-package-0.0.1/foundation_model_package.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       27 2023-07-18 23:01:31.000000 foundation-model-package-0.0.1/foundation_model_package.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-18 23:01:31.709596 foundation-model-package-0.0.1/foundation_model_pkg/
--rw-rw-rw-   0        0        0       82 2023-07-18 17:27:15.000000 foundation-model-package-0.0.1/foundation_model_pkg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 23:01:31.767370 foundation-model-package-0.0.1/foundation_model_pkg/tools/
--rw-rw-rw-   0        0        0       82 2023-07-18 17:27:15.000000 foundation-model-package-0.0.1/foundation_model_pkg/tools/__init__.py
--rw-rw-rw-   0        0        0     6394 2023-07-18 17:42:33.000000 foundation-model-package-0.0.1/foundation_model_pkg/tools/foundation_model.py
--rw-rw-rw-   0        0        0      524 2023-07-18 17:27:15.000000 foundation-model-package-0.0.1/foundation_model_pkg/tools/utils.py
--rw-rw-rw-   0        0        0       42 2023-07-18 23:01:31.813368 foundation-model-package-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      450 2023-07-18 19:47:45.000000 foundation-model-package-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-18 23:01:31.799372 foundation-model-package-0.0.1/tests/
--rw-rw-rw-   0        0        0        0 2023-07-18 17:27:15.000000 foundation-model-package-0.0.1/tests/__init__.py
--rw-rw-rw-   0        0        0      713 2023-07-18 17:46:56.000000 foundation-model-package-0.0.1/tests/test_my_tool_1.py
+drwxrwxrwx   0        0        0        0 2023-07-18 23:20:06.597123 foundation-model-package-0.0.2/
+-rw-rw-rw-   0        0        0       36 2023-07-18 17:27:15.000000 foundation-model-package-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      135 2023-07-18 23:20:06.596076 foundation-model-package-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4117 2023-07-18 17:27:15.000000 foundation-model-package-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 23:20:06.576844 foundation-model-package-0.0.2/foundation_model_package.egg-info/
+-rw-rw-rw-   0        0        0      135 2023-07-18 23:20:06.000000 foundation-model-package-0.0.2/foundation_model_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      470 2023-07-18 23:20:06.000000 foundation-model-package-0.0.2/foundation_model_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 23:20:06.000000 foundation-model-package-0.0.2/foundation_model_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2023-07-18 23:20:06.000000 foundation-model-package-0.0.2/foundation_model_package.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       27 2023-07-18 23:20:06.000000 foundation-model-package-0.0.2/foundation_model_package.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 23:20:06.579837 foundation-model-package-0.0.2/foundation_model_pkg/
+-rw-rw-rw-   0        0        0       82 2023-07-18 17:27:15.000000 foundation-model-package-0.0.2/foundation_model_pkg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 23:20:06.585657 foundation-model-package-0.0.2/foundation_model_pkg/tools/
+-rw-rw-rw-   0        0        0       82 2023-07-18 17:27:15.000000 foundation-model-package-0.0.2/foundation_model_pkg/tools/__init__.py
+-rw-rw-rw-   0        0        0     6395 2023-07-18 22:29:03.000000 foundation-model-package-0.0.2/foundation_model_pkg/tools/foundation_model.py
+-rw-rw-rw-   0        0        0      524 2023-07-18 17:27:15.000000 foundation-model-package-0.0.2/foundation_model_pkg/tools/utils.py
+-rw-rw-rw-   0        0        0       42 2023-07-18 23:20:06.597123 foundation-model-package-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      450 2023-07-18 23:17:56.000000 foundation-model-package-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 23:20:06.593672 foundation-model-package-0.0.2/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-18 17:27:15.000000 foundation-model-package-0.0.2/tests/__init__.py
+-rw-rw-rw-   0        0        0      713 2023-07-18 17:46:56.000000 foundation-model-package-0.0.2/tests/test_my_tool_1.py
```

### Comparing `foundation-model-package-0.0.1/README.md` & `foundation-model-package-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `foundation-model-package-0.0.1/foundation_model_pkg/tools/foundation_model.py` & `foundation-model-package-0.0.2/foundation_model_pkg/tools/foundation_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 class ModelFamily(str, Enum):
     LLAMA = "llama"
     DOLLY = "dolly"
     GPT2 = "gpt2"
 
 class API(str, Enum):
     CHAT = "chat"
-    COMPLETION = "completon"
+    COMPLETION = "completion"
 
 class LlamaContentFormatter(ContentFormatterBase):
 
     def __init__(self, api: API, chat_history: Optional[List[Dict]] = []):
         super().__init__()
         self.api = api
         self.chat_history = chat_history
```

### Comparing `foundation-model-package-0.0.1/foundation_model_pkg/tools/utils.py` & `foundation-model-package-0.0.2/foundation_model_pkg/tools/utils.py`

 * *Files identical despite different names*

### Comparing `foundation-model-package-0.0.1/tests/test_my_tool_1.py` & `foundation-model-package-0.0.2/tests/test_my_tool_1.py`

 * *Files identical despite different names*

