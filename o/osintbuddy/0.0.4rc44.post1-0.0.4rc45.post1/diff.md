# Comparing `tmp/osintbuddy-0.0.4rc44.post1.tar.gz` & `tmp/osintbuddy-0.0.4rc45.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osintbuddy-0.0.4rc44.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "osintbuddy-0.0.4rc45.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `osintbuddy-0.0.4rc44.post1.tar` & `osintbuddy-0.0.4rc45.post1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      359 2023-07-15 03:47:07.930484 osintbuddy-0.0.4rc44.post1/.github/workflows/CI.yml
--rw-r--r--   0        0        0      284 2023-07-15 03:47:07.930484 osintbuddy-0.0.4rc44.post1/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1807 2023-07-15 03:47:07.930484 osintbuddy-0.0.4rc44.post1/.gitignore
--rw-r--r--   0        0        0     1540 2023-07-15 03:47:07.930484 osintbuddy-0.0.4rc44.post1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      158 2023-07-15 03:47:07.930484 osintbuddy-0.0.4rc44.post1/.pypirc
--rw-r--r--   0        0        0        5 2023-07-15 03:47:07.930484 osintbuddy-0.0.4rc44.post1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      316 2023-07-15 03:47:07.930484 osintbuddy-0.0.4rc44.post1/Dockerfile
--rw-r--r--   0        0        0     1059 2023-07-15 03:47:07.930484 osintbuddy-0.0.4rc44.post1/LICENSE
--rw-r--r--   0        0        0     4493 2023-07-15 03:47:07.930484 osintbuddy-0.0.4rc44.post1/README.md
--rw-r--r--   0        0        0       47 2023-07-15 03:47:07.930484 osintbuddy-0.0.4rc44.post1/docs/developer.md
--rw-r--r--   0        0        0      471 2023-07-15 03:47:07.930484 osintbuddy-0.0.4rc44.post1/docs/pre-commit-config.md
--rw-r--r--   0        0        0    16088 2023-07-15 03:47:07.930484 osintbuddy-0.0.4rc44.post1/docs/pylint.md
--rw-r--r--   0        0        0      497 2023-07-15 03:47:07.930484 osintbuddy-0.0.4rc44.post1/docs/pyproject.md
--rw-r--r--   0        0        0      208 2023-07-15 03:47:07.930484 osintbuddy-0.0.4rc44.post1/docs/workflows.md
--rw-r--r--   0        0        0     6639 2023-07-15 03:47:07.930484 osintbuddy-0.0.4rc44.post1/pyproject.toml
--rw-r--r--   0        0        0      166 2023-07-15 03:47:07.930484 osintbuddy-0.0.4rc44.post1/requirements.txt
--rw-r--r--   0        0        0     4413 2023-07-15 03:47:07.930484 osintbuddy-0.0.4rc44.post1/src/README.md
--rw-r--r--   0        0        0      465 2023-07-15 03:47:10.910524 osintbuddy-0.0.4rc44.post1/src/osintbuddy/__init__.py
--rw-r--r--   0        0        0      396 2023-07-15 03:47:07.930484 osintbuddy-0.0.4rc44.post1/src/osintbuddy/elements/__init__.py
--rw-r--r--   0        0        0     1314 2023-07-15 03:47:07.930484 osintbuddy-0.0.4rc44.post1/src/osintbuddy/elements/base.py
--rw-r--r--   0        0        0     2993 2023-07-15 03:47:07.930484 osintbuddy-0.0.4rc44.post1/src/osintbuddy/elements/displays.py
--rw-r--r--   0        0        0     4116 2023-07-15 03:47:07.930484 osintbuddy-0.0.4rc44.post1/src/osintbuddy/elements/inputs.py
--rw-r--r--   0        0        0       62 2023-07-15 03:47:07.930484 osintbuddy-0.0.4rc44.post1/src/osintbuddy/entities/INDEX.md
--rw-r--r--   0        0        0      151 2023-07-15 03:47:07.930484 osintbuddy-0.0.4rc44.post1/src/osintbuddy/errors.py
--rw-r--r--   0        0        0     8551 2023-07-15 03:47:07.930484 osintbuddy-0.0.4rc44.post1/src/osintbuddy/plugins.py
--rw-r--r--   0        0        0     1301 2023-07-15 03:47:07.930484 osintbuddy-0.0.4rc44.post1/src/osintbuddy/utils.py
--rw-r--r--   0        0        0      964 2023-07-15 03:47:07.930484 osintbuddy-0.0.4rc44.post1/tests/conftest.py
--rw-r--r--   0        0        0      590 2023-07-15 03:47:07.930484 osintbuddy-0.0.4rc44.post1/tests/plugins.py
--rw-r--r--   0        0        0      530 2023-07-15 03:47:07.930484 osintbuddy-0.0.4rc44.post1/tests/test_methods.py
--rw-r--r--   0        0        0     6790 1970-01-01 00:00:00.000000 osintbuddy-0.0.4rc44.post1/PKG-INFO
+-rw-r--r--   0        0        0      359 2023-07-19 01:42:32.851998 osintbuddy-0.0.4rc45.post1/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      284 2023-07-19 01:42:32.851998 osintbuddy-0.0.4rc45.post1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1807 2023-07-19 01:42:32.851998 osintbuddy-0.0.4rc45.post1/.gitignore
+-rw-r--r--   0        0        0     1540 2023-07-19 01:42:32.851998 osintbuddy-0.0.4rc45.post1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      158 2023-07-19 01:42:32.851998 osintbuddy-0.0.4rc45.post1/.pypirc
+-rw-r--r--   0        0        0        5 2023-07-19 01:42:32.851998 osintbuddy-0.0.4rc45.post1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      316 2023-07-19 01:42:32.851998 osintbuddy-0.0.4rc45.post1/Dockerfile
+-rw-r--r--   0        0        0     1059 2023-07-19 01:42:32.851998 osintbuddy-0.0.4rc45.post1/LICENSE
+-rw-r--r--   0        0        0     4493 2023-07-19 01:42:32.851998 osintbuddy-0.0.4rc45.post1/README.md
+-rw-r--r--   0        0        0       47 2023-07-19 01:42:32.851998 osintbuddy-0.0.4rc45.post1/docs/developer.md
+-rw-r--r--   0        0        0      471 2023-07-19 01:42:32.851998 osintbuddy-0.0.4rc45.post1/docs/pre-commit-config.md
+-rw-r--r--   0        0        0    16088 2023-07-19 01:42:32.851998 osintbuddy-0.0.4rc45.post1/docs/pylint.md
+-rw-r--r--   0        0        0      497 2023-07-19 01:42:32.851998 osintbuddy-0.0.4rc45.post1/docs/pyproject.md
+-rw-r--r--   0        0        0      208 2023-07-19 01:42:32.851998 osintbuddy-0.0.4rc45.post1/docs/workflows.md
+-rw-r--r--   0        0        0     6639 2023-07-19 01:42:32.851998 osintbuddy-0.0.4rc45.post1/pyproject.toml
+-rw-r--r--   0        0        0      166 2023-07-19 01:42:32.851998 osintbuddy-0.0.4rc45.post1/requirements.txt
+-rw-r--r--   0        0        0     4413 2023-07-19 01:42:32.851998 osintbuddy-0.0.4rc45.post1/src/README.md
+-rw-r--r--   0        0        0      465 2023-07-19 01:42:35.655998 osintbuddy-0.0.4rc45.post1/src/osintbuddy/__init__.py
+-rw-r--r--   0        0        0      396 2023-07-19 01:42:32.851998 osintbuddy-0.0.4rc45.post1/src/osintbuddy/elements/__init__.py
+-rw-r--r--   0        0        0     1314 2023-07-19 01:42:32.855998 osintbuddy-0.0.4rc45.post1/src/osintbuddy/elements/base.py
+-rw-r--r--   0        0        0     2993 2023-07-19 01:42:32.855998 osintbuddy-0.0.4rc45.post1/src/osintbuddy/elements/displays.py
+-rw-r--r--   0        0        0     4116 2023-07-19 01:42:32.855998 osintbuddy-0.0.4rc45.post1/src/osintbuddy/elements/inputs.py
+-rw-r--r--   0        0        0       62 2023-07-19 01:42:32.855998 osintbuddy-0.0.4rc45.post1/src/osintbuddy/entities/INDEX.md
+-rw-r--r--   0        0        0      151 2023-07-19 01:42:32.855998 osintbuddy-0.0.4rc45.post1/src/osintbuddy/errors.py
+-rw-r--r--   0        0        0     8847 2023-07-19 01:42:32.855998 osintbuddy-0.0.4rc45.post1/src/osintbuddy/plugins.py
+-rw-r--r--   0        0        0     1319 2023-07-19 01:42:32.855998 osintbuddy-0.0.4rc45.post1/src/osintbuddy/utils.py
+-rw-r--r--   0        0        0      964 2023-07-19 01:42:32.855998 osintbuddy-0.0.4rc45.post1/tests/conftest.py
+-rw-r--r--   0        0        0      590 2023-07-19 01:42:32.855998 osintbuddy-0.0.4rc45.post1/tests/plugins.py
+-rw-r--r--   0        0        0      530 2023-07-19 01:42:32.855998 osintbuddy-0.0.4rc45.post1/tests/test_methods.py
+-rw-r--r--   0        0        0     6790 1970-01-01 00:00:00.000000 osintbuddy-0.0.4rc45.post1/PKG-INFO
```

### Comparing `osintbuddy-0.0.4rc44.post1/.gitignore` & `osintbuddy-0.0.4rc45.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.4rc44.post1/.pre-commit-config.yaml` & `osintbuddy-0.0.4rc45.post1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.4rc44.post1/LICENSE` & `osintbuddy-0.0.4rc45.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.4rc44.post1/README.md` & `osintbuddy-0.0.4rc45.post1/README.md`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.4rc44.post1/docs/pylint.md` & `osintbuddy-0.0.4rc45.post1/docs/pylint.md`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.4rc44.post1/pyproject.toml` & `osintbuddy-0.0.4rc45.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.4rc44.post1/src/README.md` & `osintbuddy-0.0.4rc45.post1/src/README.md`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.4rc44.post1/src/osintbuddy/elements/base.py` & `osintbuddy-0.0.4rc45.post1/src/osintbuddy/elements/base.py`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.4rc44.post1/src/osintbuddy/elements/displays.py` & `osintbuddy-0.0.4rc45.post1/src/osintbuddy/elements/displays.py`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.4rc44.post1/src/osintbuddy/elements/inputs.py` & `osintbuddy-0.0.4rc45.post1/src/osintbuddy/elements/inputs.py`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.4rc44.post1/src/osintbuddy/plugins.py` & `osintbuddy-0.0.4rc45.post1/src/osintbuddy/plugins.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,21 @@
         """
         Initializes the OBRegistry metaclass by adding the plugin class
         and its label if it is a valid plugin.
         """
         if name != 'OBPlugin' and name != 'Plugin' and issubclass(cls, OBPlugin):
             label = cls.label.strip()
             if cls.show_label is True:
-                OBRegistry.ui_labels.append(label)
+                if isinstance(cls.author, list):
+                    cls.author = ', '.join(cls.author)
+                OBRegistry.ui_labels.append({
+                    'label': label,
+                    'description': cls.description,
+                    'author': cls.author
+                })
             else:
                 OBRegistry.ui_labels.append(None)
             OBRegistry.labels.append(label)
             OBRegistry.plugins.append(cls)
 
     @classmethod
     async def get_plugin(cls, plugin_label: str):
@@ -77,38 +83,35 @@
                     importlib.import_module(f'{modpath}{modname}')
                 except ImportError as e:
                     print(f"Error importing plugin '{modpath}{modname}': {e}")
 
     return OBRegistry.plugins
 
 
-def transform(label, icon='list', prompt=None, edge_label='transformed_to'):
+def transform(label, icon='list', edge_label='transformed_to'):
     """
     A decorator add transforms to an osintbuddy plugin.
 
     Usage:
     @transform(label=<label_text>, icon=<tabler_react_icon_name>)
     def transform_to_ip(self, node, **kwargs):
         # Method implementation
 
     :param label: str, A string representing the label for the transform
         method, which can be utilized for displaying in the context menu.
     :param icon: str, Optional icon name, representing the icon associated
         displayed by the transform label. Default is "list".
     :return: A decorator for the plugin transform method.
     """
-    def decorator_transform(func):
+    def decorator_transform(func, edge_label=edge_label):
         async def wrapper(self, node, **kwargs):
             return await func(self=self, node=node, **kwargs)
         wrapper.label = label
         wrapper.icon = icon
         wrapper.edge_label = edge_label
-        if prompt is not None:
-            wrapper.prompt = prompt
-
         return wrapper
     return decorator_transform
 
 
 class OBPlugin(object, metaclass=OBRegistry):
     """
     OBPlugin is the base class for all plugin classes in this application.
@@ -117,21 +120,27 @@
     node: List[BaseElement]
     color: str = '#145070'
     label: str = ''
     icon: str = 'atom-2'
     show_label = True
     style: dict = {}
 
+    author = 'Unknown'
+    description = 'No description.'
+
     def __init__(self):
         transforms = self.__class__.__dict__.values()
         self.transforms = {
             to_snake_case(func.label): func for func in transforms if hasattr(func, 'label')
         }
         self.transform_labels = [
-            {'label': func.label, 'icon': func.icon} for func in transforms
+            {
+                'label': func.label,
+                'icon': func.icon,
+            } for func in transforms
             if hasattr(func, 'icon') and hasattr(func, 'label')
         ]
 
     def __call__(self):
         return self.blueprint()
 
     @staticmethod
```

### Comparing `osintbuddy-0.0.4rc44.post1/src/osintbuddy/utils.py` & `osintbuddy-0.0.4rc45.post1/src/osintbuddy/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,12 +27,12 @@
 
 def to_camel_case(value: str):
     value_list = value.replace(' ', '_').lower().split('_')
     return value_list[0] + ''.join(e.title() for e in value_list[1:])
 
 
 def to_snake_case(name):
-    name = to_camel_case(name)
+    name = to_camel_case(name.replace('-', '_'))
     name = re.sub('(.)([A-Z][a-z]+)', r'\1_\2', name)
     name = re.sub('__([A-Z])', r'_\1', name)
     name = re.sub('([a-z0-9])([A-Z])', r'\1_\2', name)
     return name.lower()
```

### Comparing `osintbuddy-0.0.4rc44.post1/tests/conftest.py` & `osintbuddy-0.0.4rc45.post1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.4rc44.post1/tests/plugins.py` & `osintbuddy-0.0.4rc45.post1/tests/plugins.py`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.4rc44.post1/tests/test_methods.py` & `osintbuddy-0.0.4rc45.post1/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.4rc44.post1/PKG-INFO` & `osintbuddy-0.0.4rc45.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osintbuddy
-Version: 0.0.4rc44.post1
+Version: 0.0.4rc45.post1
 Summary: OSINTBuddy - mine, merge, and map data for novel insights
 Author-email: jerlendds <theosintbuddyproject@openinfolabs.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

