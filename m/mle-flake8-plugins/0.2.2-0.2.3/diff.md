# Comparing `tmp/mle_flake8_plugins-0.2.2.tar.gz` & `tmp/mle_flake8_plugins-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mle_flake8_plugins-0.2.2.tar", max compression
+gzip compressed data, was "mle_flake8_plugins-0.2.3.tar", max compression
```

## Comparing `mle_flake8_plugins-0.2.2.tar` & `mle_flake8_plugins-0.2.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2023-06-30 12:06:40.596240 mle_flake8_plugins-0.2.2/mle_flake8_plugins/__init__.py
--rw-r--r--   0        0        0      811 2023-06-30 12:06:40.596240 mle_flake8_plugins-0.2.2/mle_flake8_plugins/flake8_mle_convention/__init__.py
--rw-r--r--   0        0        0     1197 2023-06-30 12:06:40.596240 mle_flake8_plugins-0.2.2/mle_flake8_plugins/flake8_mle_convention/disallow_final_w_pydantic.py
--rw-r--r--   0        0        0      226 2023-06-30 12:06:40.596240 mle_flake8_plugins-0.2.2/mle_flake8_plugins/flake8_mle_convention/errors.py
--rw-r--r--   0        0        0     1327 2023-06-30 12:06:40.596240 mle_flake8_plugins-0.2.2/mle_flake8_plugins/flake8_mle_convention/legacy_type_hint_checker.py
--rw-r--r--   0        0        0     1764 2023-06-30 12:06:40.596240 mle_flake8_plugins-0.2.2/mle_flake8_plugins/flake8_mle_convention/no_operation_checker.py
--rw-r--r--   0        0        0     2178 2023-06-30 12:06:40.596240 mle_flake8_plugins-0.2.2/mle_flake8_plugins/flake8_mle_docstring/__init__.py
--rw-r--r--   0        0        0     2170 2023-06-30 12:06:40.596240 mle_flake8_plugins-0.2.2/mle_flake8_plugins/flake8_mle_docstring/attribute_checker.py
--rw-r--r--   0        0        0      111 2023-06-30 12:06:40.596240 mle_flake8_plugins-0.2.2/mle_flake8_plugins/flake8_mle_docstring/errors.py
--rw-r--r--   0        0        0      596 2023-06-30 12:06:40.600240 mle_flake8_plugins-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      484 1970-01-01 00:00:00.000000 mle_flake8_plugins-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-19 13:13:11.183076 mle_flake8_plugins-0.2.3/mle_flake8_plugins/__init__.py
+-rw-r--r--   0        0        0      811 2023-07-19 13:13:11.183076 mle_flake8_plugins-0.2.3/mle_flake8_plugins/flake8_mle_convention/__init__.py
+-rw-r--r--   0        0        0     1197 2023-07-19 13:13:11.183076 mle_flake8_plugins-0.2.3/mle_flake8_plugins/flake8_mle_convention/disallow_final_w_pydantic.py
+-rw-r--r--   0        0        0      226 2023-07-19 13:13:11.183076 mle_flake8_plugins-0.2.3/mle_flake8_plugins/flake8_mle_convention/errors.py
+-rw-r--r--   0        0        0     1327 2023-07-19 13:13:11.183076 mle_flake8_plugins-0.2.3/mle_flake8_plugins/flake8_mle_convention/legacy_type_hint_checker.py
+-rw-r--r--   0        0        0     1818 2023-07-19 13:13:11.183076 mle_flake8_plugins-0.2.3/mle_flake8_plugins/flake8_mle_convention/no_operation_checker.py
+-rw-r--r--   0        0        0     2178 2023-07-19 13:13:11.183076 mle_flake8_plugins-0.2.3/mle_flake8_plugins/flake8_mle_docstring/__init__.py
+-rw-r--r--   0        0        0     2777 2023-07-19 13:13:11.183076 mle_flake8_plugins-0.2.3/mle_flake8_plugins/flake8_mle_docstring/attribute_checker.py
+-rw-r--r--   0        0        0      111 2023-07-19 13:13:11.183076 mle_flake8_plugins-0.2.3/mle_flake8_plugins/flake8_mle_docstring/errors.py
+-rw-r--r--   0        0        0      596 2023-07-19 13:13:11.187076 mle_flake8_plugins-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      484 1970-01-01 00:00:00.000000 mle_flake8_plugins-0.2.3/PKG-INFO
```

### Comparing `mle_flake8_plugins-0.2.2/mle_flake8_plugins/flake8_mle_convention/__init__.py` & `mle_flake8_plugins-0.2.3/mle_flake8_plugins/flake8_mle_convention/__init__.py`

 * *Files identical despite different names*

### Comparing `mle_flake8_plugins-0.2.2/mle_flake8_plugins/flake8_mle_convention/disallow_final_w_pydantic.py` & `mle_flake8_plugins-0.2.3/mle_flake8_plugins/flake8_mle_convention/disallow_final_w_pydantic.py`

 * *Files identical despite different names*

### Comparing `mle_flake8_plugins-0.2.2/mle_flake8_plugins/flake8_mle_convention/legacy_type_hint_checker.py` & `mle_flake8_plugins-0.2.3/mle_flake8_plugins/flake8_mle_convention/legacy_type_hint_checker.py`

 * *Files identical despite different names*

### Comparing `mle_flake8_plugins-0.2.2/mle_flake8_plugins/flake8_mle_convention/no_operation_checker.py` & `mle_flake8_plugins-0.2.3/mle_flake8_plugins/flake8_mle_convention/no_operation_checker.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,18 @@
     ast.Or,
     ast.Eq,
     ast.NotEq,
     ast.Lt,
     ast.LtE,
     ast.Gt,
     ast.GtE,
+    ast.If,
+    ast.For,
+    ast.While,
+    ast.With,
 )
 
 
 class NoOperationsChecker(ast.NodeVisitor):
     def __init__(self):
         self.errors = []
         self._class_stack = []
```

### Comparing `mle_flake8_plugins-0.2.2/mle_flake8_plugins/flake8_mle_docstring/__init__.py` & `mle_flake8_plugins-0.2.3/mle_flake8_plugins/flake8_mle_docstring/__init__.py`

 * *Files identical despite different names*

### Comparing `mle_flake8_plugins-0.2.2/mle_flake8_plugins/flake8_mle_docstring/attribute_checker.py` & `mle_flake8_plugins-0.2.3/mle_flake8_plugins/flake8_mle_docstring/attribute_checker.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,17 +19,31 @@
             if param.args[0] == "attribute":
                 attrs.append(param.args[1].strip())
         return attrs
 
     def is_public(self, attr_name):
         return attr_name[0] != "_"
 
+    def is_enum(self, node):
+        for base in node.bases:
+            if isinstance(base, ast.Attribute):
+                if base.attr == "Enum":
+                    return True
+            elif isinstance(base, ast.Name):
+                if base.id == "Enum":
+                    return True
+        return False
+
     def visit_ClassDef(self, node):
+        # モジュール内でprivateなクラスは無視
         if not self.is_public(node.name):
             return
+        # Enumを継承したクラスは無視
+        if self.is_enum(node):
+            return
         doc_attrs = self.docstring_attribute(node)
 
         for child in node.body:
             # dataclass, class member
             if (
                 isinstance(child, ast.AnnAssign)
                 and isinstance(child.target, ast.Name)
@@ -47,14 +61,16 @@
             # assign value in functions
             if isinstance(child, ast.FunctionDef):
                 for gc in child.body:
                     if (
                         isinstance(gc, ast.Assign)
                         and gc.targets
                         and isinstance(gc.targets[0], ast.Attribute)
+                        and isinstance(gc.targets[0].value, ast.Name)
+                        and gc.targets[0].value.id == 'self'
                         and self.is_public(gc.targets[0].attr)
                         and gc.targets[0].attr not in doc_attrs
                     ):
                         self.errors.append(
                             (
                                 node.lineno,
                                 node.col_offset,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mle_flake8_plugins-0.2.2/pyproject.toml` & `mle_flake8_plugins-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mle-flake8-plugins"
-version = "0.2.2"
+version = "0.2.3"
 description = ""
 authors = ["Your Name <you@example.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 docstring-parser = "^0.15"
 flake8 = "^5.0.4"
```

