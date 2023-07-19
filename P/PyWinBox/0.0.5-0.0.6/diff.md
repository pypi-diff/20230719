# Comparing `tmp/PyWinBox-0.0.5-py3-none-any.whl.zip` & `tmp/PyWinBox-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 48318 bytes, number of entries: 12
--rw-rw-rw-  2.0 fat    15635 b- defN 23-May-23 15:06 pywinbox/__init__.py
--rw-rw-rw-  2.0 fat     1426 b- defN 23-May-23 07:48 pywinbox/_pywinbox_linux.py
+Zip file size: 49242 bytes, number of entries: 12
+-rw-rw-rw-  2.0 fat    14292 b- defN 23-Jul-19 13:10 pywinbox/__init__.py
+-rw-rw-rw-  2.0 fat     1963 b- defN 23-Jul-19 12:32 pywinbox/_pywinbox_linux.py
 -rw-rw-rw-  2.0 fat     6757 b- defN 23-May-23 07:48 pywinbox/_pywinbox_macos.py
 -rw-rw-rw-  2.0 fat     1009 b- defN 23-May-23 07:48 pywinbox/_pywinbox_win.py
 -rw-rw-rw-  2.0 fat   165002 b- defN 23-Apr-19 07:41 pywinbox/_xlibcontainer.py
 -rw-rw-rw-  2.0 fat       67 b- defN 23-May-23 09:29 pywinbox/py.typed
--rw-rw-rw-  2.0 fat       85 b- defN 23-May-23 15:06 PyWinBox-0.0.5.dist-info/AUTHORS.txt
--rw-rw-rw-  2.0 fat     1537 b- defN 23-May-23 15:06 PyWinBox-0.0.5.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     6178 b- defN 23-May-23 15:06 PyWinBox-0.0.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-23 15:06 PyWinBox-0.0.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-May-23 15:06 PyWinBox-0.0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      970 b- defN 23-May-23 15:06 PyWinBox-0.0.5.dist-info/RECORD
-12 files, 198767 bytes uncompressed, 46692 bytes compressed:  76.5%
+-rw-rw-rw-  2.0 fat      127 b- defN 23-Jul-19 13:11 PyWinBox-0.0.6.dist-info/AUTHORS.txt
+-rw-rw-rw-  2.0 fat     1537 b- defN 23-Jul-19 13:11 PyWinBox-0.0.6.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     6646 b- defN 23-Jul-19 13:11 PyWinBox-0.0.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-19 13:11 PyWinBox-0.0.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Jul-19 13:11 PyWinBox-0.0.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      971 b- defN 23-Jul-19 13:11 PyWinBox-0.0.6.dist-info/RECORD
+12 files, 198472 bytes uncompressed, 47616 bytes compressed:  76.0%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: pywinbox/_xlibcontainer.py
 Comment: 
 
 Filename: pywinbox/py.typed
 Comment: 
 
-Filename: PyWinBox-0.0.5.dist-info/AUTHORS.txt
+Filename: PyWinBox-0.0.6.dist-info/AUTHORS.txt
 Comment: 
 
-Filename: PyWinBox-0.0.5.dist-info/LICENSE.txt
+Filename: PyWinBox-0.0.6.dist-info/LICENSE.txt
 Comment: 
 
-Filename: PyWinBox-0.0.5.dist-info/METADATA
+Filename: PyWinBox-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: PyWinBox-0.0.5.dist-info/WHEEL
+Filename: PyWinBox-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: PyWinBox-0.0.5.dist-info/top_level.txt
+Filename: PyWinBox-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: PyWinBox-0.0.5.dist-info/RECORD
+Filename: PyWinBox-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pywinbox/__init__.py

```diff
@@ -6,15 +6,15 @@
 from collections.abc import Callable
 from typing import Union, Tuple, overload, Optional, NamedTuple
 
 __all__ = [
     "version", "PyWinBox", "defaultOnQuery", "defaultOnSet", "Box", "Rect", "Point", "Size", "pointInBox"
 ]
 
-__version__ = "0.0.5"
+__version__ = "0.0.6"
 
 
 def version(numberOnly: bool = True):
     """Returns the current version of PyWinCtl module, in the form ''x.x.xx'' as string"""
     return ("" if numberOnly else "PyWinBox-")+__version__
 
 
@@ -45,128 +45,97 @@
 def pointInBox(x: int, y: int, box: Box):
     """Returns ``True`` if the ``(x, y)`` point is within the box described
     by ``(left, top, width, height)``."""
     return box.left <= x <= box.left + box.width and box.top <= y <= box.top + box.height
 
 
 def defaultOnQuery() -> Box:
+    """
+    Default function to invoke when any property is queried.
+
+    :return: current window position and size, as a Box Struct (x, y, width, height)
+    """
     raise NotImplementedError
 
 
-def defaultOnSet(box: Box):
-   raise NotImplementedError
+def defaultOnSet(box: Box) -> None:
+    """
+    Default function to invoke when any property is set.
+
+    :param: target window position and/or size as a Box Struct (x, y, width, height)
+    """
+    raise NotImplementedError
 
 
 class PyWinBox:
 
-    if sys.platform == "win32":
-        @overload
-        def __init__(self, onQuery: Callable[[], Box], onSet: Callable[[Box], None], handle: int): ...
-        @overload
-        def __init__(self, onQuery: Callable[[], Box], onSet: Callable[[Box], None], handle: str): ...
-        @overload
-        def __init__(self, onQuery: Callable[[], Box], onSet: Callable[[Box], None], handle: None = ...): ...
-
-        def __init__(self, onQuery: Callable[[], Box], onSet: Callable[[Box], None], handle: Optional[Union[int, str]] = None):
-            self._box: Box = Box(0, 0, 0, 0)
-            self._onQuery: Callable[[], Box] = onQuery
-            self._onSet: Callable[[Box], None] = onSet
-            if handle is not None:
-                self._handle: Optional[int] = _getHandle(handle)
-                try:
-                    self._onQuery()
-                except NotImplementedError:
-                    self._onQuery = self.__onQuery
-                try:
-                    self._onSet(self._box)
-                except NotImplementedError:
-                    self._onSet = self.__onSet
-            else:
-                self._handle = None
-
-        def __onQuery(self):
-            if self._handle is not None:
-                self._box = _getWindowBox(self._handle)
-            return self._box
-
-        def __onSet(self, newBox: Box):
-            if self._handle is not None:
-                _moveResizeWindow(self._handle, newBox)
-
-    elif sys.platform == "linux":
-        from pywinbox._xlibcontainer import XWindow
-        @overload
-        def __init__(self, onQuery: Callable[[], Box], onSet: Callable[[Box], None], handle: int): ...
-        @overload
-        def __init__(self, onQuery: Callable[[], Box], onSet: Callable[[Box], None], handle: XWindow): ...
-        @overload
-        def __init__(self, onQuery: Callable[[], Box], onSet: Callable[[Box], None], handle: None = ...): ...
-
-        def __init__(self, onQuery: Callable[[], Box], onSet: Callable[[Box], None], handle: Optional[Union[int, XWindow]] = None):
-            from pywinbox._xlibcontainer import XWindow
-            self._box: Box = Box(0, 0, 0, 0)
-            self._onQuery: Callable[[], Box] = onQuery
-            self._onSet: Callable[[Box], None] = onSet
-            if handle is not None:
-                self._handle: Optional[XWindow] = _getHandle(handle)
-                try:
-                    self._onQuery()
-                except NotImplementedError:
-                    self._onQuery = self.__onQuery
-                try:
-                    self._onSet(self._box)
-                except NotImplementedError:
-                    self._onSet = self.__onSet
-            else:
-                self._handle = None
-
-        def __onQuery(self):
-            if self._handle is not None:
-                self._box = _getWindowBox(self._handle)
-            return self._box
-
-        def __onSet(self, newBox: Box):
-            if self._handle is not None:
-                _moveResizeWindow(self._handle, newBox)
-
-    elif sys.platform == "darwin":
-        import AppKit
-        @overload
-        def __init__(self, onQuery: Callable[[], Box], onSet: Callable[[Box], None], handle: Tuple[str, str]): ...
-        @overload
-        def __init__(self, onQuery: Callable[[], Box], onSet: Callable[[Box], None], handle: AppKit.NSWindow): ...
-        @overload
-        def __init__(self, onQuery: Callable[[], Box], onSet: Callable[[Box], None], handle: None = ...): ...
-
-        def __init__(self, onQuery: Callable[[], Box], onSet: Callable[[Box], None], handle: Optional[Union[Tuple[str, str], AppKit.NSWindow]] = None):
-            self._flipValues = False
-            self._box: Box = Box(0, 0, 0, 0)
-            self._onQuery: Callable[[], Box] = onQuery
-            self._onSet: Callable[[Box], None] = onSet
-            if handle is not None:
-                self._handle: Optional[Union[macOSNSHandle, macOSCGHandle]] = _getHandle(handle)
-                try:
-                    self._onQuery()
-                except NotImplementedError:
-                    self._onQuery = self.__onQuery
-                try:
-                    self._onSet(self._box)
-                except NotImplementedError:
-                    self._onSet = self.__onSet
-            else:
-                self._handle = None
-
-        def __onQuery(self):
-            if self._handle is not None:
-                self._box = _getWindowBox(self._handle, self._flipValues)
-            return self._box
-
-        def __onSet(self, newBox: Box):
-            if self._handle is not None:
-                _moveResizeWindow(self._handle, newBox, self._flipValues)
+    def __init__(self, onQuery: Callable[[], Box], onSet: Callable[[Box], None], handle=None):
+        """
+        Class to access all area/window box properties.
+
+
+        ## Rectangular areas
+
+        You just need to instantiate the PyWinBox class, passing custom callbacks to be called when any property is
+        queried (onQuery) or set (onSet).
+
+            myPyWinBox = pywinbox.PyWinBox(onQuery=customOnQuery, onSet=customOnSet)
+
+
+        ## Window areas
+
+        To manage window areas, you need to also pass the window handle when instantiating the class, in the following formats:
+
+        - MS-Windows: integer (window id) or str (as returned by, e.g., PyQt's winId() method)
+        - Linux: integer (window id) or X-Window object
+        - macOS / foreign window: in case you want to manage a window from another application, you must pass target app and window names, as a tuple of strings (appName, windowTitle)
+        - macOS / own window: if you want to manage your own application window, you must pass NSWindow() object
+
+        (Search for cross-platform modules if you need a cross-platform handle. For instance, you can get this kind of handles
+        using PyWinCtl's getHandle(), getAppName() or title methods)
+
+        In this case, you can use the default, built-in methods to manage the window when its properties are queried or set:
+
+        - defaultOnQuery: Will update the window position and size values when any property is queried
+        - defaultOnSet: Will move and/or resize the window when any property is set
+
+            myPyWinBox = pywinbox.PyWinBox(onQuery=pywinbox.deafultOnQuery, onSet=pywinbox.defaultOnSet, handle=windowHandle)
+
+        Of course, you can also define (and pass) your own custom functions if you need to perform other actions on these events.
+
+            myPyWinBox = pywinbox.PyWinBox(onQuery=customOnQuery, onSet=customOnSet, handle=windowHandle))
+
+        In this case, if your custom functions do not properly retrieve or set the actual window position and size, the
+        information contained in the PyWinBox class, and returned by all properties, will likely become obsolete.
+        """
+
+        self._box: Box = Box(0, 0, 0, 0)
+        self._onQuery: Callable[[], Box] = onQuery
+        self._onSet: Callable[[Box], None] = onSet
+        if handle is not None:
+            self._handle = _getHandle(handle)
+            try:
+                self._onQuery()
+            except NotImplementedError:
+                self._onQuery = self.__onQuery
+            try:
+                self._onSet(self._box)
+            except NotImplementedError:
+                self._onSet = self.__onSet
+        else:
+            self._handle = None
+
+    def __onQuery(self) -> Box:
+        if self._handle is not None:
+            self._box = _getWindowBox(self._handle)
+        return self._box
+
+    def __onSet(self, newBox: Box):
+        if self._handle is not None:
+            _moveResizeWindow(self._handle, newBox)
 
     def __repr__(self):
         """Return a string of the constructor function call to create this Box object."""
         return "%s(left=%s, top=%s, width=%s, height=%s)" % (
             self.__class__.__name__,
             self._box.left,
             self._box.top,
```

## pywinbox/_pywinbox_linux.py

```diff
@@ -4,17 +4,20 @@
 
 import sys
 
 assert sys.platform == "linux"
 
 from typing import Union, Optional
 
-from pywinbox._xlibcontainer import defaultDisplay, defaultRootWindow, XWindow
+from pywinbox._xlibcontainer import defaultDisplay, defaultRootWindow, XWindow, EwmhWindow
 from pywinbox import Box
 
+_ewmhWin: Optional[EwmhWindow] = None
+_net_extents: list[int] = []
+
 
 def _getHandle(handle: Union[int, XWindow]) -> Optional[XWindow]:
     newHandle = None
     if isinstance(handle, int):
         newHandle = defaultDisplay.create_resource_object('window', handle)
     elif isinstance(handle, XWindow):
         newHandle = handle
@@ -26,22 +29,33 @@
     geom = win.get_geometry()
     x = geom.x
     y = geom.y
     w = geom.width
     h = geom.height
     while True:
         parent = win.query_tree().parent
-        if not isinstance(parent, XWindow):
+        if not parent or not isinstance(parent, XWindow):
             break
         pgeom = parent.get_geometry()
         x += pgeom.x
         y += pgeom.y
         if parent.id == 0:
             break
         win = parent
+    # Thanks to roym899 (https://github.com/roym899) for his HELP!!!!
+    global _ewmhWin
+    global _net_extents
+    if _ewmhWin is None:
+        _ewmhWin = EwmhWindow(handle.id)
+        _net_extents = _ewmhWin._getNetFrameExtents()
+    if len(_net_extents) >= 4:
+        x = x - _net_extents[0]
+        y = y - _net_extents[2]
+        w = w + _net_extents[0] + _net_extents[1]
+        h = h + _net_extents[2] + _net_extents[3]
     return Box(x, y, w, h)
 
 
 def _moveResizeWindow(handle: XWindow, newBox: Box):
     newLeft = max(0, newBox.left)  # Xlib won't accept negative positions
     newTop = max(0, newBox.top)
     defaultRootWindow.setMoveResize(winId=handle.id, x=newLeft, y=newTop, width=newBox.width, height=newBox.height, userAction=True)
```

## Comparing `PyWinBox-0.0.5.dist-info/LICENSE.txt` & `PyWinBox-0.0.6.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `PyWinBox-0.0.5.dist-info/METADATA` & `PyWinBox-0.0.6.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyWinBox
-Version: 0.0.5
+Version: 0.0.6
 Summary: Cross-Platform and multi-monitor toolkit to handle rectangular areas and windows box
 Home-page: https://github.com/Kalmat/PyWinBox
 Author: Kalmat
 Author-email: palookjones@gmail.com
 License: BSD 3
 Keywords: left top right bottom size width height topleft bottomleft topright bottomright midtop midleft midbottom midright center centerx centery box rect boundingbox area
 Classifier: Development Status :: 4 - Beta
@@ -34,14 +34,16 @@
 Requires-Dist: types-pywin32 (>=305.0.0.3) ; extra == 'dev'
 Requires-Dist: types-python-xlib (>=0.32) ; extra == 'dev'
 Requires-Dist: pywinctl (>=0.0.43) ; extra == 'dev'
 
 # PyWinBox
 
 [![Type Checking](https://github.com/Kalmat/PyWinBox/actions/workflows/type-checking.yml/badge.svg)](https://github.com/Kalmat/PyWinBox/actions/workflows/type-checking.yml)
+[![PyPI version](https://badge.fury.io/py/PyWinBox.svg)](https://badge.fury.io/py/PyWinBox)
+
 
 Cross-Platform and multi-monitor module which allows to manage window areas (position and
 size) and all their properties, as well as any rectangular area.
 
 **WARNING: Multi-monitor support is still experimental and not fully tested in macOS.**
 
 ## Rectangular areas
@@ -65,24 +67,36 @@
 using PyWinCtl's getHandle(), getAppName() or title methods)
 
 In this case, you can use the default, built-in methods to manage the window when its properties are queried or set:
 
 - defaultOnQuery: Will update the window position and size values when any property is queried
 - defaultOnSet: Will move and/or resize the window when any property is set
 
+.
 
-
-    myPyWinBox = pywinbox.PyWinBox(onQuery=pywinbox.deafultOnQuery, onSet=pywinbox.defaultOnSet, handle=windowHandle)
+    myPyWinBox = pywinbox.PyWinBox(onQuery=pywinbox.defaultOnQuery, onSet=pywinbox.defaultOnSet, handle=windowHandle)
 
 Of course, you can also define (and pass) your own custom functions if you need to perform other actions on these events.
 
     myPyWinBox = pywinbox.PyWinBox(onQuery=customOnQuery, onSet=customOnSet, handle=windowHandle))
 
 In this case, if your custom functions do not properly retrieve or set the actual window position and size, the 
-information contained in the PyWinBox class, and returned by all properties, will likely become obsolete.
+information contained in the PyWinBox class, and returned by all properties, will likely become obsolete. So, you can
+use both in your custom callback:
+
+    def customOnQuery():
+        # ... do your stuff ...
+        currBox = pywinbox.defaultOnQuery()
+        # ... do more stuff if needed ...
+        return currBox
+
+    def customOnSet(newBox: Box):
+        # ... do your stuff ...
+        pywinbox.defaultOnSet(newBox)
+        # ... do more stuff if needed ...
 
 
 ## Class Properties
 
     left, top, right, bottom
 
     size, width, height
```

