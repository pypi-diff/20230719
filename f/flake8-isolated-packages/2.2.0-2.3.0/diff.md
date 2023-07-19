# Comparing `tmp/flake8_isolated_packages-2.2.0.tar.gz` & `tmp/flake8_isolated_packages-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8_isolated_packages-2.2.0.tar", max compression
+gzip compressed data, was "flake8_isolated_packages-2.3.0.tar", max compression
```

## Comparing `flake8_isolated_packages-2.2.0.tar` & `flake8_isolated_packages-2.3.0.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1070 2021-02-27 13:16:03.301056 flake8_isolated_packages-2.2.0/LICENSE
--rw-r--r--   0        0        0      892 2021-03-02 11:27:51.305414 flake8_isolated_packages-2.2.0/README.md
--rw-r--r--   0        0        0     3421 2022-06-08 11:07:54.945300 flake8_isolated_packages-2.2.0/flake8_isolated_packages.py
--rw-r--r--   0        0        0      666 2023-06-26 13:36:13.553271 flake8_isolated_packages-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     1715 2023-06-26 13:38:51.170786 flake8_isolated_packages-2.2.0/setup.py
--rw-r--r--   0        0        0     1689 2023-06-26 13:38:51.171043 flake8_isolated_packages-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2021-02-27 13:16:03.301056 flake8_isolated_packages-2.3.0/LICENSE
+-rw-r--r--   0        0        0      892 2021-03-02 11:27:51.305414 flake8_isolated_packages-2.3.0/README.md
+-rw-r--r--   0        0        0     3455 2023-07-19 15:03:47.200580 flake8_isolated_packages-2.3.0/flake8_isolated_packages.py
+-rw-r--r--   0        0        0     2092 2023-07-19 15:03:47.204530 flake8_isolated_packages-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1860 1970-01-01 00:00:00.000000 flake8_isolated_packages-2.3.0/PKG-INFO
```

### Comparing `flake8_isolated_packages-2.2.0/LICENSE` & `flake8_isolated_packages-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8_isolated_packages-2.2.0/README.md` & `flake8_isolated_packages-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `flake8_isolated_packages-2.2.0/flake8_isolated_packages.py` & `flake8_isolated_packages-2.3.0/flake8_isolated_packages.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,75 +8,74 @@
     import importlib.metadata as importlib_metadata
 
 
 MESSAGE = 'FIP100: You try to import from isolated package'
 
 
 class Visitor(ast.NodeVisitor):
-    def __init__(self, filename: str, isolated_packages: List[str], test_folders: List['str']) -> None:
+    def __init__(self, filename: str, isolated_packages: List[str], test_folders: List[str]) -> None:
         self.package_name = self._get_package_name(filename)
         self.errors: List[Tuple[int, int]] = []
         self.isolated_packages = isolated_packages
         self.test_folders = test_folders
 
     def visit_ImportFrom(self, node: ast.ImportFrom) -> None:
         if self.package_name in self.test_folders or node.level > 0:
             self.generic_visit(node)
             return
 
-        root_import_package_name = node.module.split('.')[0]
-        if (root_import_package_name in self.isolated_packages
-                and root_import_package_name != self.package_name):
-            self.errors.append((node.lineno, node.col_offset))
+        if node.module is not None:
+            root_import_package_name = node.module.split('.')[0]
+            if root_import_package_name in self.isolated_packages and root_import_package_name != self.package_name:
+                self.errors.append((node.lineno, node.col_offset))
 
         self.generic_visit(node)
 
     @staticmethod
     def _get_package_name(filename) -> Optional[str]:
         if filename.startswith('./'):
             filename = filename[2:]
         split_filepath = filename.split('/')
-        if not len(split_filepath):
+        if not split_filepath:
             return None
         package_name = split_filepath[0]
         if package_name.endswith('.py'):
             return None
         return package_name
 
 
 class Plugin:
     name = __name__
     version = importlib_metadata.version(__name__)
 
     isolated_packages_option_name = 'isolated_packages'
     test_folders_option_name = 'test_folders'
 
-    default_isolated_packages = []
+    default_isolated_packages: List[str] = []
     default_test_folders = ['tests']
 
     @classmethod
     def add_options(cls, parser):
         """Required by flake8
         add the possible options, called first
         Args:
             parser (OptionsManager):
         """
-        kwargs = {'action': 'store', 'parse_from_config': True,
-                  'comma_separated_list': True}
+        kwargs = {'action': 'store', 'parse_from_config': True, 'comma_separated_list': True}
         parser.add_option(
             f'-{cls.isolated_packages_option_name}',
             f'--{cls.isolated_packages_option_name}',
             default=', '.join(cls.default_isolated_packages),
-            **kwargs
+            **kwargs,
         )
         parser.add_option(
             f'-{cls.test_folders_option_name}',
             f'--{cls.test_folders_option_name}',
             default=', '.join(cls.default_test_folders),
-            **kwargs
+            **kwargs,
         )
 
     @classmethod
     def parse_options(cls, options):
         """Required by flake8
         parse the options, called after add_options
         Args:
@@ -89,11 +88,11 @@
         self._filename = filename
         self._tree = tree
 
     def run(self) -> Generator[Tuple[int, int, str, Type[Any]], None, None]:
         """
         Any module from specified package could not be import in another package
         """
-        visitor = Visitor(self._filename, self._isolated_packages, self._test_folders)
+        visitor = Visitor(self._filename, self._isolated_packages, self._test_folders)  # type: ignore
         visitor.visit(self._tree)
         for line, col in visitor.errors:
             yield line, col, MESSAGE, type(self)
```

### Comparing `flake8_isolated_packages-2.2.0/PKG-INFO` & `flake8_isolated_packages-2.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: flake8-isolated-packages
-Version: 2.2.0
+Version: 2.3.0
 Summary: This Flake8 plugin is for checking imports isolations.
 Home-page: https://github.com/DDmitiy/flake8_isolated_packages
 License: MIT
 Keywords: flake8_isolated_packages,flake8,plugin,isolated_packages
 Author: Dudov Dmitry
 Author-email: dudov.dm@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.9,<4.0
+Classifier: Framework :: Flake8
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: astpretty (>=2.1.0,<3.0.0)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: Quality Assurance
 Requires-Dist: flake8 (>=3.0)
 Project-URL: Repository, https://github.com/DDmitiy/flake8_isolated_packages
 Description-Content-Type: text/markdown
 
 # flake8_isolated_packages
 
 This *Flake8* plugin is for checking imports isolations.
```

