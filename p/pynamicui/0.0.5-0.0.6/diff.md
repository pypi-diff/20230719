# Comparing `tmp/pynamicui-0.0.5.tar.gz` & `tmp/pynamicui-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynamicui-0.0.5.tar", last modified: Tue Jul 18 21:16:26 2023, max compression
+gzip compressed data, was "pynamicui-0.0.6.tar", last modified: Wed Jul 19 00:46:39 2023, max compression
```

## Comparing `pynamicui-0.0.5.tar` & `pynamicui-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 21:16:25.998607 pynamicui-0.0.5/
--rw-rw-rw-   0        0        0    11542 2023-07-18 06:19:12.000000 pynamicui-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     4825 2023-07-18 21:16:25.996610 pynamicui-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     4342 2023-07-18 08:45:35.000000 pynamicui-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-18 21:16:25.940065 pynamicui-0.0.5/pynamicui/
--rw-rw-rw-   0        0        0      386 2023-07-18 21:13:29.000000 pynamicui-0.0.5/pynamicui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 21:16:25.978606 pynamicui-0.0.5/pynamicui/createDom/
--rw-rw-rw-   0        0        0       32 2023-07-18 06:04:50.000000 pynamicui-0.0.5/pynamicui/createDom/__init__.py
--rw-rw-rw-   0        0        0     1899 2023-07-18 01:43:07.000000 pynamicui-0.0.5/pynamicui/createDom/createDom.py
-drwxrwxrwx   0        0        0        0 2023-07-18 21:16:25.985607 pynamicui-0.0.5/pynamicui/createElement/
--rw-rw-rw-   0        0        0       40 2023-07-18 06:04:41.000000 pynamicui-0.0.5/pynamicui/createElement/__init__.py
--rw-rw-rw-   0        0        0     3302 2023-07-18 01:43:31.000000 pynamicui-0.0.5/pynamicui/createElement/createElement.py
-drwxrwxrwx   0        0        0        0 2023-07-18 21:16:25.993607 pynamicui-0.0.5/pynamicui/createStylesheet/
--rw-rw-rw-   0        0        0       46 2023-07-18 06:04:27.000000 pynamicui-0.0.5/pynamicui/createStylesheet/__init__.py
--rw-rw-rw-   0        0        0      522 2023-07-18 02:33:30.000000 pynamicui-0.0.5/pynamicui/createStylesheet/createStylesheet.py
-drwxrwxrwx   0        0        0        0 2023-07-18 21:16:25.970606 pynamicui-0.0.5/pynamicui.egg-info/
--rw-rw-rw-   0        0        0     4825 2023-07-18 21:16:25.000000 pynamicui-0.0.5/pynamicui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      455 2023-07-18 21:16:25.000000 pynamicui-0.0.5/pynamicui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 21:16:25.000000 pynamicui-0.0.5/pynamicui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-07-18 21:16:25.000000 pynamicui-0.0.5/pynamicui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-18 21:16:25.000000 pynamicui-0.0.5/pynamicui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      775 2023-07-18 21:13:35.000000 pynamicui-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-18 21:16:25.998607 pynamicui-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      808 2023-07-18 21:13:46.000000 pynamicui-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 00:46:39.845224 pynamicui-0.0.6/
+-rw-rw-rw-   0        0        0    11542 2023-07-18 06:19:12.000000 pynamicui-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     4803 2023-07-19 00:46:39.843224 pynamicui-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4320 2023-07-19 00:45:37.000000 pynamicui-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-19 00:46:39.775215 pynamicui-0.0.6/pynamicui/
+-rw-rw-rw-   0        0        0      386 2023-07-19 00:41:35.000000 pynamicui-0.0.6/pynamicui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 00:46:39.827214 pynamicui-0.0.6/pynamicui/createDom/
+-rw-rw-rw-   0        0        0       32 2023-07-18 06:04:50.000000 pynamicui-0.0.6/pynamicui/createDom/__init__.py
+-rw-rw-rw-   0        0        0     1961 2023-07-18 23:11:22.000000 pynamicui-0.0.6/pynamicui/createDom/createDom.py
+drwxrwxrwx   0        0        0        0 2023-07-19 00:46:39.833222 pynamicui-0.0.6/pynamicui/createElement/
+-rw-rw-rw-   0        0        0       40 2023-07-18 06:04:41.000000 pynamicui-0.0.6/pynamicui/createElement/__init__.py
+-rw-rw-rw-   0        0        0     3950 2023-07-18 23:08:32.000000 pynamicui-0.0.6/pynamicui/createElement/createElement.py
+drwxrwxrwx   0        0        0        0 2023-07-19 00:46:39.839235 pynamicui-0.0.6/pynamicui/createStylesheet/
+-rw-rw-rw-   0        0        0       46 2023-07-18 06:04:27.000000 pynamicui-0.0.6/pynamicui/createStylesheet/__init__.py
+-rw-rw-rw-   0        0        0      522 2023-07-18 02:33:30.000000 pynamicui-0.0.6/pynamicui/createStylesheet/createStylesheet.py
+drwxrwxrwx   0        0        0        0 2023-07-19 00:46:39.819212 pynamicui-0.0.6/pynamicui.egg-info/
+-rw-rw-rw-   0        0        0     4803 2023-07-19 00:46:39.000000 pynamicui-0.0.6/pynamicui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      455 2023-07-19 00:46:39.000000 pynamicui-0.0.6/pynamicui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 00:46:39.000000 pynamicui-0.0.6/pynamicui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-19 00:46:39.000000 pynamicui-0.0.6/pynamicui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-19 00:46:39.000000 pynamicui-0.0.6/pynamicui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      775 2023-07-19 00:41:41.000000 pynamicui-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-19 00:46:39.846225 pynamicui-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      808 2023-07-19 00:41:47.000000 pynamicui-0.0.6/setup.py
```

### Comparing `pynamicui-0.0.5/LICENSE` & `pynamicui-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pynamicui-0.0.5/PKG-INFO` & `pynamicui-0.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynamicui
-Version: 0.0.5
+Version: 0.0.6
 Summary: dynamic web-like UIs using a declarative syntax
 Home-page: https://github.com/zacharie410/PynamicUI
 Author: zacharie410
 License: Apache Software License
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -113,17 +113,17 @@
     App()
 ```
 
 ## Documentation
 
 For detailed documentation and usage examples, please refer to the [PynamicUI Wiki](https://github.com/zacharie410/PynamicUI/wiki).
 
-## Example
+## Examples
 
-Check out the [example.py](https://github.com/zacharie410/PynamicUI/blob/main/examples/example.py) script for a practical example of building a counter application with PynamicUI.
+Check out the [examples](https://github.com/zacharie410/PynamicUI/blob/main/examples/) folder for practical examples building an application with PynamicUI.
 
 ## Contributions
 
 Contributions to PynamicUI are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request on [GitHub](https://github.com/zacharie410/PynamicUI).
 
 ## License
```

### Comparing `pynamicui-0.0.5/README.md` & `pynamicui-0.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -99,17 +99,17 @@
     App()
 ```
 
 ## Documentation
 
 For detailed documentation and usage examples, please refer to the [PynamicUI Wiki](https://github.com/zacharie410/PynamicUI/wiki).
 
-## Example
+## Examples
 
-Check out the [example.py](https://github.com/zacharie410/PynamicUI/blob/main/examples/example.py) script for a practical example of building a counter application with PynamicUI.
+Check out the [examples](https://github.com/zacharie410/PynamicUI/blob/main/examples/) folder for practical examples building an application with PynamicUI.
 
 ## Contributions
 
 Contributions to PynamicUI are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request on [GitHub](https://github.com/zacharie410/PynamicUI).
 
 ## License
```

### Comparing `pynamicui-0.0.5/pynamicui/createDom/createDom.py` & `pynamicui-0.0.6/pynamicui/createDom/createDom.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,16 @@
         self.route = ""
         self.states = {}  # Dictionary to store state values and callbacks
         self.widget = self.root
         self.stylesheet = {}
 
     def render(self):
         for element in self.elements:
-            element.render(self)  # Render each element in the root window
+            element.render()  # Render each element in the root window
+            element.mount() # Mount the element and its children
         self.root.mainloop()  # Start the main event loop
 
     def getCurrentRoute(self):
         return self.route
 
     def addRoute(self, url, element):
         self.routes[url] = element
```

### Comparing `pynamicui-0.0.5/pynamicui/createElement/createElement.py` & `pynamicui-0.0.6/pynamicui/createElement/createElement.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,50 +1,63 @@
 import customtkinter as tk
 
+def findDom(parent):
+    if hasattr(parent, "root"):
+        return parent
+    elif hasattr(parent, "parent"):
+        return findDom(parent.parent)
+    else:
+        # If no "root" attribute is found and there is no "parent" attribute, return None or raise an exception
+        return None
+        
 class createElement:
-    def __init__(self, dom, tag, name=None, props=None, children=None, place=None, visible=True, hooks=None, style=None):
-        self.dom = dom
+    def __init__(self, parent, tag, name=None, props=None, children=None, place=None, visible=True, hooks=None, style=None):
+        self.parent = parent
         self.name = name or "Pynamic" + tag + "Element"  # Name of the virtual element
         self.tag = "CTk" + tag  # Tag name for tkinter widget
         self.props = props or {}  # Dictionary to store widget properties
         self.children = children or []  # List of child elements
         self.widget = None  # Reference to the tkinter widget instance
-        self.place = place  # Placement options for the widget
+        self.currentPlace = place or {}  # Placement options for the widget
         self.visible = visible  # Flag to indicate element visibility
         self.hooks = hooks or {}  # Dictionary to store hooks
-        self.parent = None  # Reference to the parent element
         self.style = style or ""
-
-    def render(self, parent):
-        self.parent = parent
         
+        if hasattr(self.parent, "root"):
+            self.dom = self.parent
+            self.dom.addElement(self)
+        elif self.parent:
+            self.dom = findDom(self.parent.parent)
+            self.parent.appendChild(self)
+        
+
+    def render(self):
         if self.visible:
 
-            self.widget = getattr(tk, self.tag)(parent.widget)  # Create the tkinter widget
+            self.widget = getattr(tk, self.tag)(self.parent.widget)  # Create the tkinter widget
             for prop, value in self.props.items():
                 self.widget.configure(**{prop: value})  # Configure widget properties
             
             self.updateStyle()
 
             for child in self.children:
                 if child.visible:
-                    child.render(self)  # Render each child element
+                    child.render()  # Render each child element
 
-            if self.place and self.visible:
-                self.widget.place(**self.place)  # Place the widget in the parent
+            self.widget.place(**self.currentPlace)  # Place the widget in the parent
 
     def unmount(self):
-        if self.widget:
-            self.widget.destroy()
-            self.widget = None
         for prop, hook in self.hooks.items():
             if hook[1] is not None:
                 hook[1](prop, self, self.props.get(prop))  # Invoke the unmount hook if present
         for child in self.children:
             child.unmount()  # Unmount each child element recursively
+        if self.widget:
+            self.widget.destroy()
+            self.widget = None
 
     def mount(self):
         if self.hooks.get("") and self.hooks[""][0]:
             self.hooks[""][0]("", self, True)  # Invoke the mount hook if present
         for child in self.children:
             child.mount()  # Mount each child element recursively
 
@@ -61,18 +74,26 @@
 
     def hide(self):
         self.visible = False
         self.unmount()  # Unmount the element and its children
     
     def show(self):
         self.visible = True
-        self.render(self.parent)  # Render the element in the parent
+        self.render()  # Render the element in the parent
         self.mount()  # Mount the element and its children
 
     def setStyle(self, style):
         self.style = style
         self.updateStyle()
 
+    def place(self, geometry):
+        self.currentPlace = geometry
+        if self.widget:
+            self.widget.place(**self.currentPlace)
+
     def updateStyle(self):
         if self.style != "" and self.widget:
             for item, value in self.dom.stylesheet[self.style].items():
                 self.widget.configure(**{item: value})
+
+    def appendChild(self, child):
+        self.children.append(child)
```

### Comparing `pynamicui-0.0.5/pynamicui/createStylesheet/createStylesheet.py` & `pynamicui-0.0.6/pynamicui/createStylesheet/createStylesheet.py`

 * *Files identical despite different names*

### Comparing `pynamicui-0.0.5/pynamicui.egg-info/PKG-INFO` & `pynamicui-0.0.6/pynamicui.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynamicui
-Version: 0.0.5
+Version: 0.0.6
 Summary: dynamic web-like UIs using a declarative syntax
 Home-page: https://github.com/zacharie410/PynamicUI
 Author: zacharie410
 License: Apache Software License
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -113,17 +113,17 @@
     App()
 ```
 
 ## Documentation
 
 For detailed documentation and usage examples, please refer to the [PynamicUI Wiki](https://github.com/zacharie410/PynamicUI/wiki).
 
-## Example
+## Examples
 
-Check out the [example.py](https://github.com/zacharie410/PynamicUI/blob/main/examples/example.py) script for a practical example of building a counter application with PynamicUI.
+Check out the [examples](https://github.com/zacharie410/PynamicUI/blob/main/examples/) folder for practical examples building an application with PynamicUI.
 
 ## Contributions
 
 Contributions to PynamicUI are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request on [GitHub](https://github.com/zacharie410/PynamicUI).
 
 ## License
```

### Comparing `pynamicui-0.0.5/pyproject.toml` & `pynamicui-0.0.6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.tbump]
 github_url = "https://github.com/zacharie410/PynamicUI"
 
 [tool.tbump.version]
-current = "0.0.5"
+current = "0.0.6"
 
 # Example of a semver regexp.
 # Make sure this matches current_version before
 # using tbump
 regex = '''
   (?P<major>\d+)
   \.
```

### Comparing `pynamicui-0.0.5/setup.py` & `pynamicui-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name='pynamicui',
-    version='0.0.5',
+    version='0.0.6',
     description='dynamic web-like UIs using a declarative syntax',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/zacharie410/PynamicUI',
     author='zacharie410',
     license='Apache Software License',
     classifiers=[
```

