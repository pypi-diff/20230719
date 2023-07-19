# Comparing `tmp/pytermgame-1.0.0.tar.gz` & `tmp/pytermgame-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytermgame-1.0.0.tar", last modified: Sun Jul 16 07:59:39 2023, max compression
+gzip compressed data, was "pytermgame-1.0.1.tar", last modified: Wed Jul 19 14:57:06 2023, max compression
```

## Comparing `pytermgame-1.0.0.tar` & `pytermgame-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 07:59:39.794488 pytermgame-1.0.0/
--rw-rw-rw-   0        0        0    35823 2023-07-16 07:58:21.000000 pytermgame-1.0.0/LICENSE
--rw-rw-rw-   0        0        0    42026 2023-07-16 07:59:39.793488 pytermgame-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      424 2023-07-16 07:56:06.000000 pytermgame-1.0.0/README.md
--rw-rw-rw-   0        0        0      470 2023-07-16 07:58:58.000000 pytermgame-1.0.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-07-16 07:59:39.747495 pytermgame-1.0.0/pytermgame/
--rw-rw-rw-   0        0        0      386 2023-07-16 07:36:33.000000 pytermgame-1.0.0/pytermgame/__init__.py
--rw-rw-rw-   0        0        0     1797 2023-07-16 07:37:02.000000 pytermgame-1.0.0/pytermgame/_get_key.py
--rw-rw-rw-   0        0        0      829 2023-07-16 07:37:36.000000 pytermgame-1.0.0/pytermgame/event.py
--rw-rw-rw-   0        0        0     3088 2023-07-16 07:39:44.000000 pytermgame-1.0.0/pytermgame/game.py
--rw-rw-rw-   0        0        0      215 2023-07-16 07:28:20.000000 pytermgame-1.0.0/pytermgame/key.py
--rw-rw-rw-   0        0        0     1285 2023-07-16 06:20:18.000000 pytermgame-1.0.0/pytermgame/matrixstring.py
--rw-rw-rw-   0        0        0     3685 2023-07-16 07:36:28.000000 pytermgame-1.0.0/pytermgame/sprite.py
--rw-rw-rw-   0        0        0      853 2023-07-16 07:26:35.000000 pytermgame-1.0.0/pytermgame/terminal.py
-drwxrwxrwx   0        0        0        0 2023-07-16 07:59:39.790491 pytermgame-1.0.0/pytermgame.egg-info/
--rw-rw-rw-   0        0        0    42026 2023-07-16 07:59:39.000000 pytermgame-1.0.0/pytermgame.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2023-07-16 07:59:39.000000 pytermgame-1.0.0/pytermgame.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 07:59:39.000000 pytermgame-1.0.0/pytermgame.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-07-16 07:59:39.000000 pytermgame-1.0.0/pytermgame.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-16 07:59:39.794488 pytermgame-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-19 14:57:06.487216 pytermgame-1.0.1/
+-rw-rw-rw-   0        0        0    35823 2023-07-16 07:58:21.000000 pytermgame-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0    42543 2023-07-19 14:57:06.484167 pytermgame-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      941 2023-07-19 14:53:13.000000 pytermgame-1.0.1/README.md
+-rw-rw-rw-   0        0        0      470 2023-07-19 14:56:21.000000 pytermgame-1.0.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-07-19 14:57:06.295884 pytermgame-1.0.1/pytermgame/
+-rw-rw-rw-   0        0        0      235 2023-07-19 14:39:15.000000 pytermgame-1.0.1/pytermgame/__init__.py
+-rw-rw-rw-   0        0        0     1797 2023-07-16 07:37:02.000000 pytermgame-1.0.1/pytermgame/_get_key.py
+-rw-rw-rw-   0        0        0      697 2023-07-19 14:38:03.000000 pytermgame-1.0.1/pytermgame/clock.py
+-rw-rw-rw-   0        0        0      485 2023-07-19 14:30:59.000000 pytermgame-1.0.1/pytermgame/event.py
+-rw-rw-rw-   0        0        0     4478 2023-07-19 14:40:45.000000 pytermgame-1.0.1/pytermgame/game.py
+-rw-rw-rw-   0        0        0      215 2023-07-16 07:28:20.000000 pytermgame-1.0.1/pytermgame/key.py
+-rw-rw-rw-   0        0        0     5195 2023-07-19 14:43:09.000000 pytermgame-1.0.1/pytermgame/sprite.py
+-rw-rw-rw-   0        0        0     1268 2023-07-19 14:34:14.000000 pytermgame-1.0.1/pytermgame/sprites.py
+-rw-rw-rw-   0        0        0     1064 2023-07-19 14:34:28.000000 pytermgame-1.0.1/pytermgame/surface.py
+-rw-rw-rw-   0        0        0     1179 2023-07-19 14:38:41.000000 pytermgame-1.0.1/pytermgame/terminal.py
+drwxrwxrwx   0        0        0        0 2023-07-19 14:57:06.469102 pytermgame-1.0.1/pytermgame.egg-info/
+-rw-rw-rw-   0        0        0    42543 2023-07-19 14:57:06.000000 pytermgame-1.0.1/pytermgame.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      379 2023-07-19 14:57:06.000000 pytermgame-1.0.1/pytermgame.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 14:57:06.000000 pytermgame-1.0.1/pytermgame.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-07-19 14:57:06.000000 pytermgame-1.0.1/pytermgame.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-19 14:57:06.488220 pytermgame-1.0.1/setup.cfg
```

### Comparing `pytermgame-1.0.0/LICENSE` & `pytermgame-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytermgame-1.0.0/PKG-INFO` & `pytermgame-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytermgame
-Version: 1.0.0
+Version: 1.0.1
 Summary: Like pygame, but in the terminal
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -681,24 +681,33 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pytermgame
-Like pygame, but in the terminal
 
-Working example: `jet_and_ball.py`
+You've seen frameworks for making terminal apps (`textual`, `pytermgraphics`, `asciimatics`) ... but how about a framework for games ... like `pygame`?
 
-`pip install pytermgame`
+Installation: `pip install pytermgame`
 
-note: key input is a bit laggy on linux
+## Features
+- pygame-inspired structure
+- customizable terminal behaviour (alternate screen, cursor visibility)
+- optimized rendering, game figures out which sprites requires erase and re-render **(it takes care of overlapping sprites too!)**
+- cross-platform support for reading and identifying keys
 
-TODO:
+## Examples
+Currently there is one only: `jet_and_ball.py`
+
+Use up and down arrows to control, just dodge the balls
+
+The grey line is for alignment
+
+### TODO:
 - support for more keys
 - simulated scrolling (extended axis)
+- use integer IDs to reference sprites (for performance?)
 - support color using ANSI (Char class?)
     - option to remain black and white (less memory)
 - mouse support
 - more examples
-- special sprites (background, text)
-- more options at Game()
```

### Comparing `pytermgame-1.0.0/pytermgame/_get_key.py` & `pytermgame-1.0.1/pytermgame/_get_key.py`

 * *Files identical despite different names*

### Comparing `pytermgame-1.0.0/pytermgame/matrixstring.py` & `pytermgame-1.0.1/pytermgame/surface.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-class MatrixString:
+class Surface:
     data: list[str]
 
     def __init__(self, string: str):
         self.data = string.splitlines()
 
     @classmethod
     def blank(cls, width: int, height: int):
@@ -35,19 +35,7 @@
             yield line
 
     def to_blank(self):
         string = ""
         for line in self.lines():
             string += " " * len(line) + "\n"
         return type(self).strip(string)
-    
-if __name__ == "__main__":
-    mstr = MatrixString(
-"""
-abc
-defg
-weeeeee
-""".strip("\n")
-    )
-    assert mstr[2] == "weeeeee"
-    assert mstr[1][1] == "e"
-    assert mstr[1, 1] == mstr[1][1] == "e"
```

### Comparing `pytermgame-1.0.0/pytermgame/terminal.py` & `pytermgame-1.0.1/pytermgame/terminal.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import sys
 import os
 import platform
+from random import randint
 
 WINDOWS = platform.system() == "Windows"
 
 width, height = os.get_terminal_size()
 
 def write(string: str):
     sys.stdout.write(string)
@@ -16,15 +17,16 @@
     write(string)
     flush()
 
 def goto(x: int, y: int):
     write(f"\033[{y};{x}H")
 
 def transform_coords(x: int, y: int):
-    # screen coords -> terminal coords
+    # screen coords (0, 0) based -> terminal coords (1, 1) based
+    # may support extended axis scrolling in the future
     return x + 1, y + 1
 
 def enable_alternate_buffer():
     fwrite("\033[?1049h")
 
 def disable_alternate_buffer():
     fwrite("\033[?1049l")
@@ -37,9 +39,21 @@
 
 def clear():
     write("\033[2J")
 
 def home():
     write("\033[H")
 
-def fullclear(): # currently unused, may cause flickering
+def full_clear(): # currently unused, may cause flickering
     os.system("cls" if os.name == "nt" else "clear")
+
+def enable_autowrap():
+    write("\033[?7h")
+
+def disable_autowrap():
+    write("\033[?7l")
+
+# code helpers
+def randy():
+    return randint(0, height - 1)
+def randx():
+    return randint(0, width - 1)
```

### Comparing `pytermgame-1.0.0/pytermgame.egg-info/PKG-INFO` & `pytermgame-1.0.1/pytermgame.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytermgame
-Version: 1.0.0
+Version: 1.0.1
 Summary: Like pygame, but in the terminal
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -681,24 +681,33 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pytermgame
-Like pygame, but in the terminal
 
-Working example: `jet_and_ball.py`
+You've seen frameworks for making terminal apps (`textual`, `pytermgraphics`, `asciimatics`) ... but how about a framework for games ... like `pygame`?
 
-`pip install pytermgame`
+Installation: `pip install pytermgame`
 
-note: key input is a bit laggy on linux
+## Features
+- pygame-inspired structure
+- customizable terminal behaviour (alternate screen, cursor visibility)
+- optimized rendering, game figures out which sprites requires erase and re-render **(it takes care of overlapping sprites too!)**
+- cross-platform support for reading and identifying keys
 
-TODO:
+## Examples
+Currently there is one only: `jet_and_ball.py`
+
+Use up and down arrows to control, just dodge the balls
+
+The grey line is for alignment
+
+### TODO:
 - support for more keys
 - simulated scrolling (extended axis)
+- use integer IDs to reference sprites (for performance?)
 - support color using ANSI (Char class?)
     - option to remain black and white (less memory)
 - mouse support
 - more examples
-- special sprites (background, text)
-- more options at Game()
```

