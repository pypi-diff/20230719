# Comparing `tmp/PyWinBox-0.0.6-py3-none-any.whl.zip` & `tmp/PyWinBox-0.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 49242 bytes, number of entries: 12
--rw-rw-rw-  2.0 fat    14292 b- defN 23-Jul-19 13:10 pywinbox/__init__.py
--rw-rw-rw-  2.0 fat     1963 b- defN 23-Jul-19 12:32 pywinbox/_pywinbox_linux.py
+Zip file size: 49247 bytes, number of entries: 12
+-rw-rw-rw-  2.0 fat    14292 b- defN 23-Jul-19 13:18 pywinbox/__init__.py
+-rw-rw-rw-  2.0 fat     1990 b- defN 23-Jul-19 13:18 pywinbox/_pywinbox_linux.py
 -rw-rw-rw-  2.0 fat     6757 b- defN 23-May-23 07:48 pywinbox/_pywinbox_macos.py
 -rw-rw-rw-  2.0 fat     1009 b- defN 23-May-23 07:48 pywinbox/_pywinbox_win.py
 -rw-rw-rw-  2.0 fat   165002 b- defN 23-Apr-19 07:41 pywinbox/_xlibcontainer.py
 -rw-rw-rw-  2.0 fat       67 b- defN 23-May-23 09:29 pywinbox/py.typed
--rw-rw-rw-  2.0 fat      127 b- defN 23-Jul-19 13:11 PyWinBox-0.0.6.dist-info/AUTHORS.txt
--rw-rw-rw-  2.0 fat     1537 b- defN 23-Jul-19 13:11 PyWinBox-0.0.6.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     6646 b- defN 23-Jul-19 13:11 PyWinBox-0.0.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-19 13:11 PyWinBox-0.0.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Jul-19 13:11 PyWinBox-0.0.6.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      971 b- defN 23-Jul-19 13:11 PyWinBox-0.0.6.dist-info/RECORD
-12 files, 198472 bytes uncompressed, 47616 bytes compressed:  76.0%
+-rw-rw-rw-  2.0 fat      127 b- defN 23-Jul-19 13:19 PyWinBox-0.0.7.dist-info/AUTHORS.txt
+-rw-rw-rw-  2.0 fat     1537 b- defN 23-Jul-19 13:19 PyWinBox-0.0.7.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     6646 b- defN 23-Jul-19 13:19 PyWinBox-0.0.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-19 13:19 PyWinBox-0.0.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Jul-19 13:19 PyWinBox-0.0.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      971 b- defN 23-Jul-19 13:19 PyWinBox-0.0.7.dist-info/RECORD
+12 files, 198499 bytes uncompressed, 47621 bytes compressed:  76.0%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: pywinbox/_xlibcontainer.py
 Comment: 
 
 Filename: pywinbox/py.typed
 Comment: 
 
-Filename: PyWinBox-0.0.6.dist-info/AUTHORS.txt
+Filename: PyWinBox-0.0.7.dist-info/AUTHORS.txt
 Comment: 
 
-Filename: PyWinBox-0.0.6.dist-info/LICENSE.txt
+Filename: PyWinBox-0.0.7.dist-info/LICENSE.txt
 Comment: 
 
-Filename: PyWinBox-0.0.6.dist-info/METADATA
+Filename: PyWinBox-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: PyWinBox-0.0.6.dist-info/WHEEL
+Filename: PyWinBox-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: PyWinBox-0.0.6.dist-info/top_level.txt
+Filename: PyWinBox-0.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: PyWinBox-0.0.6.dist-info/RECORD
+Filename: PyWinBox-0.0.7.dist-info/RECORD
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
 
-__version__ = "0.0.6"
+__version__ = "0.0.7"
 
 
 def version(numberOnly: bool = True):
     """Returns the current version of PyWinCtl module, in the form ''x.x.xx'' as string"""
     return ("" if numberOnly else "PyWinBox-")+__version__
```

## pywinbox/_pywinbox_linux.py

```diff
@@ -8,15 +8,15 @@
 
 from typing import Union, Optional
 
 from pywinbox._xlibcontainer import defaultDisplay, defaultRootWindow, XWindow, EwmhWindow
 from pywinbox import Box
 
 _ewmhWin: Optional[EwmhWindow] = None
-_net_extents: list[int] = []
+_net_extents: Optional[list[int]] = []
 
 
 def _getHandle(handle: Union[int, XWindow]) -> Optional[XWindow]:
     newHandle = None
     if isinstance(handle, int):
         newHandle = defaultDisplay.create_resource_object('window', handle)
     elif isinstance(handle, XWindow):
@@ -43,15 +43,15 @@
         win = parent
     # Thanks to roym899 (https://github.com/roym899) for his HELP!!!!
     global _ewmhWin
     global _net_extents
     if _ewmhWin is None:
         _ewmhWin = EwmhWindow(handle.id)
         _net_extents = _ewmhWin._getNetFrameExtents()
-    if len(_net_extents) >= 4:
+    if _net_extents and len(_net_extents) >= 4:
         x = x - _net_extents[0]
         y = y - _net_extents[2]
         w = w + _net_extents[0] + _net_extents[1]
         h = h + _net_extents[2] + _net_extents[3]
     return Box(x, y, w, h)
```

## Comparing `PyWinBox-0.0.6.dist-info/LICENSE.txt` & `PyWinBox-0.0.7.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `PyWinBox-0.0.6.dist-info/METADATA` & `PyWinBox-0.0.7.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyWinBox
-Version: 0.0.6
+Version: 0.0.7
 Summary: Cross-Platform and multi-monitor toolkit to handle rectangular areas and windows box
 Home-page: https://github.com/Kalmat/PyWinBox
 Author: Kalmat
 Author-email: palookjones@gmail.com
 License: BSD 3
 Keywords: left top right bottom size width height topleft bottomleft topright bottomright midtop midleft midbottom midright center centerx centery box rect boundingbox area
 Classifier: Development Status :: 4 - Beta
```

## Comparing `PyWinBox-0.0.6.dist-info/RECORD` & `PyWinBox-0.0.7.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-pywinbox/__init__.py,sha256=C0plN2bzBeJ9chCoFWv44BwmEVQCpCZfqvndQ6QYejQ,14292
-pywinbox/_pywinbox_linux.py,sha256=dqAwKVlCzbMjhBLIVQJtsYiE2BIvMASYVPCVOIhi_Uk,1963
+pywinbox/__init__.py,sha256=Vb9EFU97ZET39zXAjXrGzBTXxe9krtLYIfRrKlg5QwA,14292
+pywinbox/_pywinbox_linux.py,sha256=tc85w4CzeU80VaQaHJcRrhtQcpgQcGLdyLlqhGDSUAs,1990
 pywinbox/_pywinbox_macos.py,sha256=JeJx1Cvv2_X4mz7GYgueWjMAyYJ_YBoGVSBoK_1SDzU,6757
 pywinbox/_pywinbox_win.py,sha256=SB_l866-j_vgre4EbVe5x24DUmZ79Mqqmjmbi8pdWjg,1009
 pywinbox/_xlibcontainer.py,sha256=dJ2xEkVYtcHfXEd-PUZqd6GSFhRpz7RF4Yuq5ZHCHMk,165002
 pywinbox/py.typed,sha256=mAeBY6TvO_5r6EkS1X7q7RIxVMAb__SungbyrvIC98U,67
-PyWinBox-0.0.6.dist-info/AUTHORS.txt,sha256=0TxZiNgtcIKwZtd11TP4-zsDIeDxmV7wCKHu_WefSSk,127
-PyWinBox-0.0.6.dist-info/LICENSE.txt,sha256=CDxlTE1hRDjEq4SrS2ZwFEexw7hLgN3kgoWVYeBNI7Y,1537
-PyWinBox-0.0.6.dist-info/METADATA,sha256=rvZ74s_p8LOhOwPzZ7CJ8T28Fxi3RmLg20DSYPbLB6U,6646
-PyWinBox-0.0.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-PyWinBox-0.0.6.dist-info/top_level.txt,sha256=_QapqXVUQP5IYu2yZiHsxw3G5CK_KzzyOBJ0SBEWOHA,9
-PyWinBox-0.0.6.dist-info/RECORD,,
+PyWinBox-0.0.7.dist-info/AUTHORS.txt,sha256=0TxZiNgtcIKwZtd11TP4-zsDIeDxmV7wCKHu_WefSSk,127
+PyWinBox-0.0.7.dist-info/LICENSE.txt,sha256=CDxlTE1hRDjEq4SrS2ZwFEexw7hLgN3kgoWVYeBNI7Y,1537
+PyWinBox-0.0.7.dist-info/METADATA,sha256=mYd1qMA7mUvvobvyLyKoFsJzSH0BYTNuRhk57TVHkvY,6646
+PyWinBox-0.0.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+PyWinBox-0.0.7.dist-info/top_level.txt,sha256=_QapqXVUQP5IYu2yZiHsxw3G5CK_KzzyOBJ0SBEWOHA,9
+PyWinBox-0.0.7.dist-info/RECORD,,
```

