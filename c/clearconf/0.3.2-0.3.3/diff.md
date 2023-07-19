# Comparing `tmp/clearconf-0.3.2.tar.gz` & `tmp/clearconf-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clearconf-0.3.2.tar", max compression
+gzip compressed data, was "clearconf-0.3.3.tar", max compression
```

## Comparing `clearconf-0.3.2.tar` & `clearconf-0.3.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     2786 2023-06-22 21:13:09.616037 clearconf-0.3.2/README.md
--rw-r--r--   0        0        0       37 2023-06-22 21:13:09.616037 clearconf-0.3.2/clearconf/__init__.py
--rw-r--r--   0        0        0     1745 2023-06-22 21:13:09.626037 clearconf-0.3.2/clearconf/assets/example_conf.py
--rw-r--r--   0        0        0      968 2023-06-22 21:13:09.626037 clearconf-0.3.2/clearconf/assets/init.py
--rw-r--r--   0        0        0      213 2023-06-22 21:13:09.626037 clearconf-0.3.2/clearconf/assets/stub_conf.py
--rw-r--r--   0        0        0     6347 2023-06-26 12:08:00.831325 clearconf-0.3.2/clearconf/base_config.py
--rw-r--r--   0        0        0        0 2023-06-22 21:13:09.626037 clearconf-0.3.2/clearconf/cli/__init__.py
--rw-r--r--   0        0        0      930 2023-06-22 21:13:09.626037 clearconf-0.3.2/clearconf/cli/defaults.py
--rw-r--r--   0        0        0     1729 2023-06-22 21:13:09.626037 clearconf-0.3.2/clearconf/cli/main.py
--rw-r--r--   0        0        0        0 2023-06-22 21:13:09.626037 clearconf-0.3.2/clearconf/utils/__init__.py
--rw-r--r--   0        0        0      746 2023-06-22 21:13:09.626037 clearconf-0.3.2/clearconf/utils/conf.py
--rw-r--r--   0        0        0      917 2023-06-22 21:13:09.626037 clearconf-0.3.2/clearconf/utils/file.py
--rw-r--r--   0        0        0      509 2023-06-22 21:13:09.626037 clearconf-0.3.2/clearconf/utils/stdout.py
--rw-r--r--   0        0        0      723 2023-06-26 12:08:40.671325 clearconf-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     3524 1970-01-01 00:00:00.000000 clearconf-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     2786 2023-07-19 06:41:06.394975 clearconf-0.3.3/README.md
+-rw-r--r--   0        0        0       37 2023-07-19 06:41:06.394975 clearconf-0.3.3/clearconf/__init__.py
+-rw-r--r--   0        0        0     1745 2023-07-19 06:41:06.394975 clearconf-0.3.3/clearconf/assets/example_conf.py
+-rw-r--r--   0        0        0      968 2023-07-19 06:41:06.394975 clearconf-0.3.3/clearconf/assets/init.py
+-rw-r--r--   0        0        0      213 2023-07-19 06:41:06.394975 clearconf-0.3.3/clearconf/assets/stub_conf.py
+-rw-r--r--   0        0        0     7278 2023-07-19 14:33:19.976638 clearconf-0.3.3/clearconf/base_config.py
+-rw-r--r--   0        0        0        0 2023-07-19 06:41:06.394975 clearconf-0.3.3/clearconf/cli/__init__.py
+-rw-r--r--   0        0        0      930 2023-07-19 06:41:06.394975 clearconf-0.3.3/clearconf/cli/defaults.py
+-rw-r--r--   0        0        0     1729 2023-07-19 06:41:06.394975 clearconf-0.3.3/clearconf/cli/main.py
+-rw-r--r--   0        0        0        0 2023-07-19 06:41:06.394975 clearconf-0.3.3/clearconf/utils/__init__.py
+-rw-r--r--   0        0        0      746 2023-07-19 06:41:06.394975 clearconf-0.3.3/clearconf/utils/conf.py
+-rw-r--r--   0        0        0      917 2023-07-19 06:41:06.394975 clearconf-0.3.3/clearconf/utils/file.py
+-rw-r--r--   0        0        0      509 2023-07-19 06:41:06.394975 clearconf-0.3.3/clearconf/utils/stdout.py
+-rw-r--r--   0        0        0      723 2023-07-19 14:36:56.627521 clearconf-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     3524 1970-01-01 00:00:00.000000 clearconf-0.3.3/PKG-INFO
```

### Comparing `clearconf-0.3.2/README.md` & `clearconf-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `clearconf-0.3.2/clearconf/assets/example_conf.py` & `clearconf-0.3.3/clearconf/assets/example_conf.py`

 * *Files identical despite different names*

### Comparing `clearconf-0.3.2/clearconf/assets/init.py` & `clearconf-0.3.3/clearconf/assets/init.py`

 * *Files identical despite different names*

### Comparing `clearconf-0.3.2/clearconf/base_config.py` & `clearconf-0.3.3/clearconf/base_config.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 import inspect
 import json
 from pathlib import Path
 
 
 class Watcher(type):
     def __init__(cls, name, bases, clsdict):
+        # This is first called for BaseConfig, then for Config
+        # After subclass is called, or the classes defined insided Config inherit
+        # from BaseConfig and this is called for those too.
+        
+        # This allows us to propagate BaseConfig deeper.
         if len(cls.mro()) > 2:
             cls._subclass()
         super(Watcher, cls).__init__(name, bases, clsdict)
 
 class BaseConfig(metaclass=Watcher):
 
     @classmethod
@@ -31,15 +36,15 @@
             if len(target.mro()) >= 5:
                 key = f'{key}({target.mro()[3].__name__})'
             output = {key: res}
 
         target_attr = set(dir(target))
         # This removes variables from superclasses
         for i in range(3, len(target.__mro__) - 1):
-            # The if allows inheritance between configs but I guess there are better solutions
+            # The allows inheritance between configs but I guess there are better solutions
             if 'configs' not in target.__mro__[i].__module__:
                 target_attr = target_attr - set(dir(target.__mro__[i]))
 
         for k in target_attr:
             if not k.startswith('_') and k not in ['to_dict', 'to_json', 'to_list', 'init', 'to_flat_dict', 'get_cfg']:
                 attr = getattr(target, k)
 
@@ -59,20 +64,21 @@
                     elif attr.__module__.split('.')[0] == '__main__' or 'config' in attr.__module__:
                         if len(attr.mro()) >= 5: # when a config class is subclassed to use it directly
                             k = f'{k}({attr.mro()[3].__name__})'
                         res[k] = attr.to_dict()
                     else:
                         # End up here if attr is not a class defined inside module.
                         if type(attr).__name__ == 'type':  # it is a class
-                            name = attr.__name__
+                            name = f'{attr.__module__}.{attr.__name__}'
                         else: # it is an object
-                            name = type(attr).__name__
                             if attr.__str__ is not object.__str__:
-                                name = attr.__str__()   
-                        res[k] = f'{attr.__module__}.{name}'
+                                name = attr.__str__()  # sometimes repr() might be preferable
+                            else:
+                                name = f'{type(attr).__name__}.{attr.__name__}'
+                            res[k] = name
                 # If it's not a class save it. This is done for basic types.
                 # Could cause problems with complex objects
                 else:
                     res[k] = attr
 
         return output
 
@@ -93,23 +99,21 @@
                     # Not ideal but config could be anywhere in the name
                     # Need to find a better way to do this
                     if attr.__module__.split('.')[0] == '__main__' or 'config' in attr.__module__:
                         # This way the module keeps its subclasses but it is also subclassed by
                         # BaseConfig inheriting its method. A security check could be used to assure
                         # that the new methods are not overriding any old one.
                         setattr(target, k, type(f'{k}_mod', (BaseConfig, ) + tuple(attr.__mro__), dict(list(dict(vars(BaseConfig)).items()) + list(dict(vars(attr)).items()))))
-                        getattr(target, k)._subclass()
         return res
 
     @classmethod
     def to_flat_dict(cls) -> dict:
         import torch
         res = cls.to_dict()
         res = flatten(res)
-        # res = {k.split('.')[-1]: torch.tensor(v) if isinstance(v, list) else v for k, v in res.items()}
         return res
 
     @classmethod
     def to_list(cls):
         target = cls
 
         res = []
@@ -125,17 +129,32 @@
                         res.append(f'{attr.__module__}.{attr.__name__}')
                 # If it's not a class save it. This is done for basic types.
                 # Could cause problems with complex objects
                 else:
                     res.append(attr)
         return res
     
-    def get_cfg(self):
-        return self.__class__
-
+    def get_cfg(self, to_self=False):
+        if not to_self:
+            return self.__class__
+        
+        target = self.__class__
+        
+        target_attr = set(dir(target))
+        # This removes variables from superclasses
+        for i in range(3, len(target.__mro__) - 1):
+            # The allows inheritance between configs but I guess there are better solutions
+            if 'configs' not in target.__mro__[i].__module__:
+                target_attr = target_attr - set(dir(target.__mro__[i]))
+        
+        for k in target_attr:
+            if not k.startswith('_') and k not in ['to_dict', 'to_json', 'to_list', 'init', 'to_flat_dict', 'get_cfg']:
+                attr = getattr(target, k)
+                setattr(self, k, attr)
+    
     def __getattribute__(self, item):
         return object.__getattribute__(self, item)
 
 
 def flatten(d, parent_key='', sep='.'):
     items = []
     for k, v in d.items():
```

### Comparing `clearconf-0.3.2/clearconf/cli/defaults.py` & `clearconf-0.3.3/clearconf/cli/defaults.py`

 * *Files identical despite different names*

### Comparing `clearconf-0.3.2/clearconf/cli/main.py` & `clearconf-0.3.3/clearconf/cli/main.py`

 * *Files identical despite different names*

### Comparing `clearconf-0.3.2/clearconf/utils/conf.py` & `clearconf-0.3.3/clearconf/utils/conf.py`

 * *Files identical despite different names*

### Comparing `clearconf-0.3.2/clearconf/utils/file.py` & `clearconf-0.3.3/clearconf/utils/file.py`

 * *Files identical despite different names*

### Comparing `clearconf-0.3.2/pyproject.toml` & `clearconf-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clearconf"
-version = "0.3.2"
+version = "0.3.3"
 description = "ClearConf is a library created to support easy and manageble python configuration. It consists in a CLI tool to manage the configuration directory, and in a python class (BaseConfig) which adds additional functionalities to a configuration class."
 authors = ["andrearosasco <andrea.rosasco@iit.it>"]
 homepage = "https://github.com/andrearosasco/clearconf"
 repository = "https://github.com/andrearosasco/clearconf"
 readme = "README.md"
```

### Comparing `clearconf-0.3.2/PKG-INFO` & `clearconf-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clearconf
-Version: 0.3.2
+Version: 0.3.3
 Summary: ClearConf is a library created to support easy and manageble python configuration. It consists in a CLI tool to manage the configuration directory, and in a python class (BaseConfig) which adds additional functionalities to a configuration class.
 Home-page: https://github.com/andrearosasco/clearconf
 Author: andrearosasco
 Author-email: andrea.rosasco@iit.it
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

