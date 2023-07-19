# Comparing `tmp/sophia_doc-0.1.4.tar.gz` & `tmp/sophia_doc-0.1.5.tar.gz`

## Comparing `sophia_doc-0.1.4.tar` & `sophia_doc-0.1.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 sophia_doc-0.1.4/sophia_doc/.DS_Store
--rw-r--r--   0        0        0    15629 2020-02-02 00:00:00.000000 sophia_doc-0.1.4/sophia_doc/__init__.py
--rw-r--r--   0        0        0     3621 2020-02-02 00:00:00.000000 sophia_doc-0.1.4/sophia_doc/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sophia_doc-0.1.4/sophia_doc/py.typed
--rw-r--r--   0        0        0     4891 2020-02-02 00:00:00.000000 sophia_doc-0.1.4/sophia_doc/utils.py
--rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 sophia_doc-0.1.4/sophia_doc/builders/__init__.py
--rw-r--r--   0        0        0    16468 2020-02-02 00:00:00.000000 sophia_doc-0.1.4/sophia_doc/builders/markdown.py
--rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 sophia_doc-0.1.4/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 sophia_doc-0.1.4/LICENSE
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 sophia_doc-0.1.4/README.md
--rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 sophia_doc-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 sophia_doc-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 sophia_doc-0.1.5/sophia_doc/.DS_Store
+-rw-r--r--   0        0        0    15605 2020-02-02 00:00:00.000000 sophia_doc-0.1.5/sophia_doc/__init__.py
+-rw-r--r--   0        0        0     3621 2020-02-02 00:00:00.000000 sophia_doc-0.1.5/sophia_doc/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sophia_doc-0.1.5/sophia_doc/py.typed
+-rw-r--r--   0        0        0     4915 2020-02-02 00:00:00.000000 sophia_doc-0.1.5/sophia_doc/utils.py
+-rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 sophia_doc-0.1.5/sophia_doc/builders/__init__.py
+-rw-r--r--   0        0        0    16335 2020-02-02 00:00:00.000000 sophia_doc-0.1.5/sophia_doc/builders/markdown.py
+-rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 sophia_doc-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 sophia_doc-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 sophia_doc-0.1.5/README.md
+-rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 sophia_doc-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 sophia_doc-0.1.5/PKG-INFO
```

### Comparing `sophia_doc-0.1.4/sophia_doc/.DS_Store` & `sophia_doc-0.1.5/sophia_doc/.DS_Store`

 * *Files identical despite different names*

### Comparing `sophia_doc-0.1.4/sophia_doc/__init__.py` & `sophia_doc-0.1.5/sophia_doc/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,42 +7,44 @@
 import sophia_doc.builders.markdown
 
 module = sophia_doc.ModuleNode(sophia_doc)
 builder = sophia_doc.builders.markdown.MarkdownBuilder(module)
 builder.write('doc_dir')
 ```
 """
+from __future__ import annotations
+
 import inspect
 import pkgutil
 import sys
 import traceback
 import types
 import warnings
 from enum import Enum
 from functools import cached_property
-from typing import Any, Dict, Generic, List, NamedTuple, Optional, Tuple, TypeVar, Union
+from typing import Any, Generic, NamedTuple, TypeVar, Union
 
 from sophia_doc.utils import import_module
 
 _T = TypeVar("_T")
 
 
-def _find_class(func: Any) -> Optional[type]:
+def _find_class(func: Any) -> type | None:
     # cut from pydoc
     cls = sys.modules.get(func.__module__)
     if cls is None:
         return None
     for name in func.__qualname__.split(".")[:-1]:
         cls = getattr(cls, name)
     if not inspect.isclass(cls):
         return None
     return cls
 
 
-def _find_doc(obj: Any) -> Optional[str]:
+def _find_doc(obj: Any) -> str | None:
     # cut from pydoc
     if inspect.ismethod(obj):
         name = obj.__func__.__name__  # type: ignore
         self = obj.__self__
         if (
             inspect.isclass(self)
             and getattr(self, name, None).__func__ is obj.__func__  # type: ignore
@@ -88,28 +90,29 @@
         except AttributeError:
             continue
         if doc is not None:
             return doc
     return None
 
 
-def _get_own_doc(obj: Any) -> Optional[str]:
+def _get_own_doc(obj: Any) -> str | None:
     """Get the documentation string for an object if it is not inherited from its class."""
     # cut from pydoc
     try:
         doc = object.__getattribute__(obj, "__doc__")
         if doc is None:
             return None
         if obj is not type:
             typedoc = type(obj).__doc__
             if isinstance(typedoc, str) and typedoc == doc:
                 return None
-        return doc
     except AttributeError:
         return None
+    else:
+        return doc
 
 
 def _getdoc(obj: Any):
     """Get the documentation string for an object.
 
     All tabs are expanded to space. To clean up docstrings that are
     indented to line up with blocks of code, any whitespace than can be
@@ -143,15 +146,15 @@
         or inspect.isroutine(obj)
         or inspect.isframe(obj)
         or inspect.istraceback(obj)
         or inspect.iscode(obj)
     )
 
 
-def is_visible_name(name: str, _all: Optional[list] = None) -> bool:
+def is_visible_name(name: str, _all: list | None = None) -> bool:
     """Decide whether to show documentation on a variable.
 
     Args:
         name: The variable name.
         _all: __all__ list of a module.
 
     Returns:
@@ -161,15 +164,15 @@
         return True
     # only document that which the programmer exported in __all__
     if _all is not None:
         return name in _all
     return not name.startswith("_")
 
 
-def get_annotations(obj: Any) -> Dict[str, Any]:
+def get_annotations(obj: Any) -> dict[str, Any]:
     """Get the annotations dict for an object."""
     # refs: https://docs.python.org/3/howto/annotations.html
     if sys.version_info >= (3, 10):
         return inspect.get_annotations(obj)
     if isinstance(obj, type):
         return obj.__dict__.get("__annotations__", {})
     return getattr(obj, "__annotations__", {})
@@ -183,18 +186,18 @@
         name: The name of this object.
         module: The module of this object.
     """
 
     __slots__ = ("obj", "name", "module", "_qualname")
     obj: _T
     name: str
-    module: "ModuleNode"
+    module: ModuleNode
     _qualname: str
 
-    def __init__(self, obj: _T, name: str, qualname: str, module: "ModuleNode"):
+    def __init__(self, obj: _T, name: str, qualname: str, module: ModuleNode):
         """Init DocNode."""
         self.obj = obj
         self.name = name
         self._qualname = qualname
         self.module = module
 
     @cached_property
@@ -204,25 +207,25 @@
 
     @cached_property
     def realname(self) -> str:
         """Real name of this object."""
         return getattr(self.obj, "__name__", self.name)
 
     @cached_property
-    def annotations(self) -> Dict[str, Any]:
+    def annotations(self) -> dict[str, Any]:
         """Annotations of this object."""
         return get_annotations(self.obj)
 
     @cached_property
     def docstring(self) -> str:
         """Docstring of this object."""
         return getdoc(self.obj)
 
     @staticmethod
-    def from_obj(obj: Any, name: str, qualname: str, module: "ModuleNode") -> "DocNode":
+    def from_obj(obj: Any, name: str, qualname: str, module: ModuleNode) -> DocNode:
         """Returns an object of DocNode's subclass.
 
         Args:
             obj: An object.
             name: The name of the object.
             qualname: The qualname of the object.
             module: The module of the object.
@@ -255,27 +258,27 @@
     """The class of module node."""
 
     def __init__(self, obj: types.ModuleType):
         """Init ModuleNode."""
         super().__init__(obj, obj.__name__, "", self)
 
     @cached_property
-    def attributes(self) -> List[DocNode]:
+    def attributes(self) -> list[DocNode]:
         """A list of attributes of this module."""
         _all = getattr(self.obj, "__all__", None)
         attributes = []
         for key, value in list(getattr(self.obj, "__dict__", {}).items()):
             if (inspect.getmodule(value) or self.obj) is self.obj and is_visible_name(
                 key, _all
             ):
                 attributes.append(self.from_obj(value, key, key, self))
         return attributes
 
     @cached_property
-    def submodules(self) -> List["ModuleNode"]:
+    def submodules(self) -> list[ModuleNode]:
         """A list of submodules of this module."""
         submodules = []
         submodule_names = set()
         if self.is_package:
             for _importer, modname, _ispkg in pkgutil.iter_modules(self.obj.__path__):
                 if not is_visible_name(modname):
                     continue
@@ -294,23 +297,23 @@
                 value.__name__.startswith(self.name + ".")
                 and key not in submodule_names
             ):
                 submodules.append(ModuleNode(value))
         return submodules
 
     @cached_property
-    def file(self) -> Optional[str]:
+    def file(self) -> str | None:
         """The source file name of this module."""
         try:
             return inspect.getabsfile(self.obj)
         except TypeError:
             return None
 
     @cached_property
-    def source(self) -> Optional[str]:
+    def source(self) -> str | None:
         """The source of this module."""
         loader = getattr(self.obj, "__loader__", None)
         if loader and getattr(loader, "get_source", None):
             try:
                 source = loader.get_source(self.name)
                 if source:
                     return source
@@ -328,25 +331,25 @@
 
     @cached_property
     def is_namespace(self) -> bool:
         """Returns True if this module is a namespace package."""
         return hasattr(self.obj, "__path__") and not hasattr(self.obj, "__file__")
 
     @cached_property
-    def classes(self) -> List["ClassNode"]:
+    def classes(self) -> list[ClassNode]:
         """A list of class objects in this module's attributes."""
         return [i for i in self.attributes if isinstance(i, ClassNode)]
 
     @cached_property
-    def functions(self) -> List["FunctionNode"]:
+    def functions(self) -> list[FunctionNode]:
         """A list of function objects in this module's attributes."""
         return [i for i in self.attributes if isinstance(i, FunctionNode)]
 
     @cached_property
-    def data(self) -> List["DataNode"]:
+    def data(self) -> list[DataNode]:
         """A list of data objects in module's this attributes."""
         return [i for i in self.attributes if isinstance(i, DataNode)]
 
 
 class ClassNode(DocNode[type]):
     """The class of class node."""
 
@@ -354,15 +357,15 @@
         """The attribute of a class."""
 
         name: str
         kind: str
         node: DocNode
 
     @cached_property
-    def attributes(self) -> List["ClassNode.Attribute"]:
+    def attributes(self) -> list[ClassNode.Attribute]:
         """A list of attributes of this class."""
         attributes = []
         for name in filter(is_visible_name, dir(self.obj)):
             if isinstance(self.obj, Enum) and name == "__init__":
                 continue
 
             if (
@@ -404,32 +407,32 @@
                 )
 
             attributes.append(self.Attribute(name, kind, node))
 
         return attributes
 
     @cached_property
-    def subclasses(self) -> List["ClassNode"]:
+    def subclasses(self) -> list[ClassNode]:
         """A list of subclasses of this class."""
         return [
             ClassNode(cls, cls.__name__, cls.__qualname__, self.module)
             for cls in type.__subclasses__(self.obj)
             if not (cls.__name__.startswith("_") and cls.__module__ == "builtins")
         ]
 
     @cached_property
-    def bases(self) -> Tuple[str, ...]:
+    def bases(self) -> tuple[str, ...]:
         """Base class names of this class."""
         return tuple(
             (x.__module__ + "." if x.__module__ != "builtins" else "") + x.__qualname__
             for x in self.obj.__bases__
         )
 
     @cached_property
-    def mro(self) -> Tuple[type, ...]:
+    def mro(self) -> tuple[type, ...]:
         """The mro of this class."""
         return inspect.getmro(self.obj)
 
     @cached_property
     def is_abstract(self) -> bool:
         """Returns True if this class is an abstract class."""
         return inspect.isabstract(self.obj)
@@ -437,15 +440,15 @@
 
 class FunctionNode(
     DocNode[Union[types.FunctionType, types.MethodType, types.MethodDescriptorType]]
 ):
     """The class of function node."""
 
     @cached_property
-    def signature(self) -> Optional[inspect.Signature]:
+    def signature(self) -> inspect.Signature | None:
         """Signature of this function."""
         try:
             return inspect.signature(self.obj)
         except (ValueError, TypeError):
             return None
 
     @cached_property
@@ -471,15 +474,15 @@
         return self.realname == "<lambda>"
 
 
 class DataNode(DocNode[_T]):
     """The class of data node."""
 
     @cached_property
-    def annotations(self) -> Dict[str, Any]:
+    def annotations(self) -> dict[str, Any]:
         """Annotations of this object."""
         if isinstance(self.obj, property):
             return get_annotations(self.obj.fget)
         if isinstance(self.obj, cached_property):
             return get_annotations(self.obj.func)
         return get_annotations(self.obj)
```

### Comparing `sophia_doc-0.1.4/sophia_doc/__main__.py` & `sophia_doc-0.1.5/sophia_doc/__main__.py`

 * *Files identical despite different names*

### Comparing `sophia_doc-0.1.4/sophia_doc/utils.py` & `sophia_doc-0.1.5/sophia_doc/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 """Utils of sophia_doc."""
+from __future__ import annotations
+
 import importlib
 import inspect
 import re
 import traceback
 import warnings
-from types import ModuleType
-from typing import Any, Optional
+from typing import TYPE_CHECKING, Any
+
+if TYPE_CHECKING:
+    from types import ModuleType
 
 
 def import_module(modname: str) -> ModuleType:
     """A wrapper of importlib.import_module, convert exceptions to ImportError.
 
     Args:
         modname: The name of the module to be imported.
@@ -17,24 +21,24 @@
     Returns:
         The imported module.
     """
     try:
         with warnings.catch_warnings():
             warnings.filterwarnings("ignore", category=ImportWarning)
             return importlib.import_module(modname)
+    except KeyboardInterrupt:
+        # Dot not catch KeyboardInterrupt.
+        # Catch KeyboardInterrupt may prevent user kill python
+        # when the module took a too long time to import.
+        raise
     except BaseException as exc:
-        if isinstance(exc, KeyboardInterrupt):
-            # Dot not catch KeyboardInterrupt.
-            # Catch KeyboardInterrupt may prevent user kill python
-            # when the module took a too long time to import.
-            raise exc
         raise ImportError(exc, traceback.format_exc()) from exc
 
 
-def format_annotation(annotation: Any, base_module: Optional[ModuleType] = None) -> str:
+def format_annotation(annotation: Any, base_module: ModuleType | None = None) -> str:
     """Format the annotation.
 
     Args:
         annotation: The annotation object to be formatted.
         base_module: A module which the object from.
 
     Returns:
```

### Comparing `sophia_doc-0.1.4/sophia_doc/builders/__init__.py` & `sophia_doc-0.1.5/sophia_doc/builders/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """Builder is class to build ModuleNode to target formats."""
+from __future__ import annotations
+
 from abc import ABC, abstractmethod
 from pathlib import Path
 from typing import TYPE_CHECKING
 
 from docstring_parser import Docstring, DocstringStyle, parse
 
 if TYPE_CHECKING:
@@ -15,37 +17,37 @@
     Builds target formats from ModuleNode.
 
     Attributes:
         module: A ModuleNode object.
         docstring_style: The docstring style the module used, auto check by default.
     """
 
-    module: "ModuleNode"
+    module: ModuleNode
     docstring_style: DocstringStyle
 
     def __init__(
         self,
-        module: "ModuleNode",
+        module: ModuleNode,
         *,
         docstring_style: DocstringStyle = DocstringStyle.AUTO,
     ):
         """Init Builder.
 
         Args:
             module: The Module Node to build.
             docstring_style: The docstring style. Defaults to DocstringStyle.AUTO.
         """
         self.module = module
         self.docstring_style = docstring_style
 
-    def _new_builder(self, module: "ModuleNode") -> "Builder":
+    def _new_builder(self, module: ModuleNode) -> Builder:
         """Get a new instance of Builder class, is used in write method."""
         return self.__class__(module, docstring_style=self.docstring_style)
 
-    def get_docstring(self, obj: "DocNode") -> "Docstring":
+    def get_docstring(self, obj: DocNode) -> Docstring:
         """Get the Docstring object of a DocNode object.
 
         Args:
             obj: A DocNode object.
 
         Returns:
             A Docstring object.
```

### Comparing `sophia_doc-0.1.4/sophia_doc/builders/markdown.py` & `sophia_doc-0.1.5/sophia_doc/builders/markdown.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 """The Markdown Builder."""
+from __future__ import annotations
+
 import inspect
 import warnings
 from pathlib import Path
 from textwrap import indent
-from typing import Dict, List, Optional, Tuple
 
 from docstring_parser import Docstring, DocstringParam, DocstringStyle
 
 from sophia_doc import ClassNode, DataNode, DocNode, FunctionNode, ModuleNode
 from sophia_doc.builders import Builder
 from sophia_doc.utils import format_annotation, format_signature
 
 
-def get_description(docstring: Docstring) -> List[str]:
+def get_description(docstring: Docstring) -> list[str]:
     """Get description form a Docstring object.
 
     Args:
         docstring: A Docstring object.
 
     Returns:
         A list of description string.
     """
-    result: List[str] = []
+    result: list[str] = []
     if docstring.short_description:
         result.append(docstring.short_description)
     if docstring.long_description:
         result.append(docstring.long_description)
     return result
 
 
-def parser_param(
-    name: str, annotation: Optional[str], description: Optional[str]
-) -> str:
+def parser_param(name: str, annotation: str | None, description: str | None) -> str:
     """Get formatted string of parameter.
 
     Args:
         name: Parameter name.
         annotation: Parameter annotation.
         description: Parameter description.
 
@@ -112,15 +111,15 @@
         ignore_data: bool = False,
     ):
         """Init Markdown Builder."""
         super().__init__(module, docstring_style=docstring_style)
         self.anchor_extend = anchor_extend
         self.ignore_data = ignore_data
 
-    def _new_builder(self, module: ModuleNode) -> "Builder":
+    def _new_builder(self, module: ModuleNode) -> Builder:
         return self.__class__(
             module,
             docstring_style=self.docstring_style,
             anchor_extend=self.anchor_extend,
             ignore_data=self.ignore_data,
         )
 
@@ -146,27 +145,26 @@
             path = Path(*self.module.name.split(".")[0:])
         return (
             path / init_file_name if self.module.is_package else path.with_suffix(".md")
         )
 
     def text(self) -> str:
         """Get string of current module documentation."""
-        result: List[str] = []
+        result: list[str] = []
         result.append(Markdown.title(self.module.name, 1))
 
         docstring = self.get_docstring(self.module)
         result.extend(get_description(docstring))
 
-        for node in self.module.attributes:
-            result.append(self.build_doc(node))
+        result.extend(self.build_doc(node) for node in self.module.attributes)
 
         return self._build_str(result).replace("<", r"\<").replace(">", r"\>")
 
     @staticmethod
-    def _build_str(str_list: List[str]) -> str:
+    def _build_str(str_list: list[str]) -> str:
         return "\n\n".join(filter(lambda x: x, str_list))
 
     def build_doc(self, node: DocNode, *, level: int = 1, **kwargs) -> str:
         """Build markdown string from a DocNode.
 
         Args:
             node: A DocNode.
@@ -208,15 +206,15 @@
 
         init = None
         for attr in node.attributes:
             if attr.name == "__init__":
                 assert isinstance(attr.node, FunctionNode)
                 init = attr.node
 
-        result: List[str] = []
+        result: list[str] = []
         title = Markdown.title(
             Markdown.italic(_kind) + " " + Markdown.inline_code(node.name), level + 1
         )
         if init and init.signature:
             title += format_signature(init.signature)
         else:
             warnings.warn(
@@ -236,17 +234,15 @@
                     init, self.get_docstring(init), ignore_first_arg=True
                 )
             )
 
         if docstring.params or node.annotations:
             result.append("- **Attributes**")
 
-            parma_dict: Dict[
-                str, Tuple[inspect.Parameter, Optional[DocstringParam]]
-            ] = {}
+            parma_dict: dict[str, tuple[inspect.Parameter, DocstringParam | None]] = {}
             if node.annotations:
                 parma_dict = {
                     key: (annotation, None)
                     for key, annotation in node.annotations.items()
                     if not key.startswith("_")
                 }
 
@@ -295,20 +291,18 @@
             )
 
         return self._build_str(result)
 
     @staticmethod
     def _build_argument(
         node: FunctionNode, docstring: Docstring, *, ignore_first_arg: bool = False
-    ) -> List[str]:
+    ) -> list[str]:
         result = []
         if docstring.params or (node.signature and node.signature.parameters):
-            parma_dict: Dict[
-                str, Tuple[inspect.Parameter, Optional[DocstringParam]]
-            ] = {}
+            parma_dict: dict[str, tuple[inspect.Parameter, DocstringParam | None]] = {}
             if node.signature and node.signature.parameters:
                 for key, param in node.signature.parameters.items():
                     if param.kind == param.VAR_POSITIONAL:
                         key = "*" + key  # noqa: PLW2901
                     elif param.kind == param.VAR_KEYWORD:
                         key = "**" + key  # noqa: PLW2901
                     parma_dict[key] = (param, None)
@@ -387,15 +381,15 @@
         if node.is_async:
             _kind.append("async")
         if node.is_lambda_func:
             _kind.append("lambda")
         _kind.append(kind)
         _kind = " ".join(_kind)
 
-        result: List[str] = []
+        result: list[str] = []
         result.append(
             self._extend_title(
                 Markdown.title(
                     Markdown.italic(_kind)
                     + " "
                     + Markdown.inline_code(
                         f"{node.name}{format_signature(node.signature)}"
@@ -434,23 +428,23 @@
                 result.append(Markdown.indent(f"Type: {Markdown.italic(type_name)}"))
 
             if docstring.returns and docstring.returns.description:
                 result.append(Markdown.indent(docstring.returns.description))
 
         if docstring.raises:
             result.append("- **Raises**")
-            for raise_doc in docstring.raises:
-                result.append(
-                    Markdown.indent(
-                        "- {type_name} - {description}".format(
-                            type_name=Markdown.bold(raise_doc.type_name or ""),
-                            description=raise_doc.description,
-                        )
+            result.extend(
+                Markdown.indent(
+                    "- {type_name} - {description}".format(
+                        type_name=Markdown.bold(raise_doc.type_name or ""),
+                        description=raise_doc.description,
                     )
                 )
+                for raise_doc in docstring.raises
+            )
 
         if docstring.examples:
             result.append("- **Examples**")
             result.append(Markdown.indent(docstring.examples[0].description or ""))
 
         return self._build_str(result)
 
@@ -472,15 +466,15 @@
 
         Returns:
             A markdown string.
         """
         if self.ignore_data and kind == "data":
             return ""
 
-        result: List[str] = []
+        result: list[str] = []
         result.append(
             self._extend_title(
                 Markdown.title(
                     Markdown.italic(kind) + " " + Markdown.inline_code(node.name),
                     level + 1,
                 ),
                 node,
```

### Comparing `sophia_doc-0.1.4/.gitignore` & `sophia_doc-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `sophia_doc-0.1.4/LICENSE` & `sophia_doc-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sophia_doc-0.1.4/README.md` & `sophia_doc-0.1.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -8,29 +8,29 @@
 
 It's a lot like sphinx, but it only focuses on generating markdown documentation.
 
 It does not support PEP 224 attribute docstring, because the PEP was rejected, and have to use ast module to support it, which brings additional complexity to this project.
 
 ## Install
 
-```shell
+```sh
 pip install sophia-doc
 ```
 
 ## Quickstart
 
-```shell
+```sh
 sophia_doc "sophia_doc" -o ./doc
 ```
 
 ## Usage
 
 Command line:
 
-```shell
+```txt
 usage: sophia_doc [-h] [-o OUTPUT_DIR] [--docstring-style DOCSTRING_STYLE] [--anchor-extend | --no-anchor-extend] [--overwrite | --no-overwrite]
                    [--exclude-module-name | --no-exclude-module-name]
                    module
 
 Sophia_doc is a python package to automatically generate API documents for Python modules
 
 positional arguments:
```

### Comparing `sophia_doc-0.1.4/pyproject.toml` & `sophia_doc-0.1.5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sophia-doc"
-version = "0.1.4"
+version = "0.1.5"
 description = "A python package to automatically generate API documents for Python modules."
 authors = [{ name = "st1020", email = "stone_1020@qq.com" }]
 license = { text = "MIT" }
 readme = "README.md"
 keywords = ["sophia-doc", "documentation", "doc", "pydoc", "markdown"]
 classifiers = [
   "Development Status :: 3 - Alpha",
@@ -33,49 +33,60 @@
 
 [tool.black]
 target-version = ["py38", "py39", "py310", "py311"]
 
 [tool.ruff]
 line-length = 88
 select = [
-  "F",   # Pyflakes
-  "E",   # pycodestyle errors
-  "W",   # pycodestyle warnings
-  "I",   # isort
-  "N",   # pep8-naming
-  "D",   # pydocstyle
-  "UP",  # pyupgrade
-  "S",   # flake8-bandit
-  "B",   # flake8-bugbear
-  "C4",  # flake8-comprehensions
-  "T10", # flake8-debugger
-  "ISC", # flake8-implicit-str-concat
-  "PIE", # flake8-pie
-  "T20", # flake8-print
-  "Q",   # flake8-quotes
-  "RSE", # flake8-raise
-  "RET", # flake8-return
-  "SLF", # flake8-self
-  "SIM", # flake8-simplify
-  "TCH", # flake8-type-checking
-  "INT", # flake8-gettext
-  "ARG", # flake8-unused-arguments
-  "TD",  # flake8-todos
-  "PGH", # pygrep-hooks
-  "PL",  # Pylint
-  "FLY", # flynt
-  "RUF", # Ruff-specific rules
+  "F",     # Pyflakes
+  "E",     # pycodestyle errors
+  "W",     # pycodestyle warnings
+  "I",     # isort
+  "N",     # pep8-naming
+  "D",     # pydocstyle
+  "UP",    # pyupgrade
+  "YTT",   # flake8-2020
+  "ASYNC", # flake8-async
+  "S",     # flake8-bandit
+  "B",     # flake8-bugbear
+  "C4",    # flake8-comprehensions
+  "DTZ",   # flake8-datetimez
+  "T10",   # flake8-debugger
+  "FA",    # flake8-future-annotations
+  "ISC",   # flake8-implicit-str-concat
+  "G",     # flake8-logging-format
+  "PIE",   # flake8-pie
+  "T20",   # flake8-print
+  "Q",     # flake8-quotes
+  "RSE",   # flake8-raise
+  "RET",   # flake8-return
+  "SLF",   # flake8-self
+  "SLOT",  # flake8-slots
+  "SIM",   # flake8-simplify
+  "TCH",   # flake8-type-checking
+  "INT",   # flake8-gettext
+  "ARG",   # flake8-unused-arguments
+  "TD",    # flake8-todos
+  "FIX",   # flake8-fixme
+  "ERA",   # eradicate
+  "PGH",   # pygrep-hooks
+  "PL",    # Pylint
+  "TRY",   # tryceratops
+  "FLY",   # flynt
+  "PERF",  # Perflint
+  "RUF",   # Ruff-specific rules
 ]
 ignore = [
   "E501",    # Line too long, handled by black
   "S101",    # Use of assert detected
   "PGH003",  # Use specific rule codes when ignoring type issues
   "PLR0911", # Too many return statements
   "PLR0912", # Too many branches
   "PLR0913", # Too many arguments to function call
+  "PERF203", # try-except within a loop incurs performance overhead
 ]
 target-version = "py38"
 
 [tool.ruff.pydocstyle]
 convention = "google"
 
 [tool.ruff.per-file-ignores]
```

### Comparing `sophia_doc-0.1.4/PKG-INFO` & `sophia_doc-0.1.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sophia-doc
-Version: 0.1.4
+Version: 0.1.5
 Summary: A python package to automatically generate API documents for Python modules.
 Project-URL: Homepage, https://github.com/st1020/sophia-doc
 Project-URL: Source, https://github.com/st1020/sophia-doc
 Author-email: st1020 <stone_1020@qq.com>
 License: MIT
 License-File: LICENSE
 Keywords: doc,documentation,markdown,pydoc,sophia-doc
@@ -32,29 +32,29 @@
 
 It's a lot like sphinx, but it only focuses on generating markdown documentation.
 
 It does not support PEP 224 attribute docstring, because the PEP was rejected, and have to use ast module to support it, which brings additional complexity to this project.
 
 ## Install
 
-```shell
+```sh
 pip install sophia-doc
 ```
 
 ## Quickstart
 
-```shell
+```sh
 sophia_doc "sophia_doc" -o ./doc
 ```
 
 ## Usage
 
 Command line:
 
-```shell
+```txt
 usage: sophia_doc [-h] [-o OUTPUT_DIR] [--docstring-style DOCSTRING_STYLE] [--anchor-extend | --no-anchor-extend] [--overwrite | --no-overwrite]
                    [--exclude-module-name | --no-exclude-module-name]
                    module
 
 Sophia_doc is a python package to automatically generate API documents for Python modules
 
 positional arguments:
```

