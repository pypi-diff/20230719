# Comparing `tmp/ex4nicegui-0.1.9.tar.gz` & `tmp/ex4nicegui-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ex4nicegui-0.1.9.tar", last modified: Mon Jul 17 16:37:56 2023, max compression
+gzip compressed data, was "ex4nicegui-0.2.0.tar", last modified: Tue Jul 18 11:03:07 2023, max compression
```

## Comparing `ex4nicegui-0.1.9.tar` & `ex4nicegui-0.2.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 16:37:56.665471 ex4nicegui-0.1.9/
--rw-rw-rw-   0        0        0     1094 2023-06-30 08:17:10.000000 ex4nicegui-0.1.9/LICENSE
--rw-rw-rw-   0        0        0      481 2023-07-17 16:37:56.664473 ex4nicegui-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     2200 2023-07-10 15:25:21.000000 ex4nicegui-0.1.9/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 16:37:56.599861 ex4nicegui-0.1.9/ex4nicegui/
--rw-rw-rw-   0        0        0      337 2023-07-17 16:36:37.000000 ex4nicegui-0.1.9/ex4nicegui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 16:37:56.620914 ex4nicegui-0.1.9/ex4nicegui/layout/
--rw-rw-rw-   0        0        0       31 2023-07-05 06:10:00.000000 ex4nicegui-0.1.9/ex4nicegui/layout/__init__.py
--rw-rw-rw-   0        0        0     2378 2023-07-05 06:10:00.000000 ex4nicegui-0.1.9/ex4nicegui/layout/gridbox.py
-drwxrwxrwx   0        0        0        0 2023-07-17 16:37:56.636149 ex4nicegui-0.1.9/ex4nicegui/reactive/
-drwxrwxrwx   0        0        0        0 2023-07-17 16:37:56.644816 ex4nicegui-0.1.9/ex4nicegui/reactive/ECharts/
--rw-rw-rw-   0        0        0  1581614 2023-07-17 15:29:41.000000 ex4nicegui-0.1.9/ex4nicegui/reactive/ECharts/ECharts.js
--rw-rw-rw-   0        0        0     2550 2023-07-17 16:36:22.000000 ex4nicegui-0.1.9/ex4nicegui/reactive/ECharts/ECharts.py
--rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.1.9/ex4nicegui/reactive/ECharts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 16:37:56.649806 ex4nicegui-0.1.9/ex4nicegui/reactive/UseDraggable/
--rw-rw-rw-   0        0        0     4857 2023-07-17 16:36:22.000000 ex4nicegui-0.1.9/ex4nicegui/reactive/UseDraggable/UseDraggable.js
--rw-rw-rw-   0        0        0     2888 2023-07-17 16:36:22.000000 ex4nicegui-0.1.9/ex4nicegui/reactive/UseDraggable/UseDraggable.py
--rw-rw-rw-   0        0        0        0 2023-07-17 16:36:22.000000 ex4nicegui-0.1.9/ex4nicegui/reactive/UseDraggable/__init__.py
--rw-rw-rw-   0        0        0     1303 2023-07-17 16:36:22.000000 ex4nicegui-0.1.9/ex4nicegui/reactive/__index.py
--rw-rw-rw-   0        0        0       24 2023-07-05 06:10:00.000000 ex4nicegui-0.1.9/ex4nicegui/reactive/__init__.py
--rw-rw-rw-   0        0        0     1356 2023-07-16 10:54:22.000000 ex4nicegui-0.1.9/ex4nicegui/reactive/drawer.py
--rw-rw-rw-   0        0        0     6093 2023-07-16 10:54:22.000000 ex4nicegui-0.1.9/ex4nicegui/reactive/local_file_picker.py
--rw-rw-rw-   0        0        0    38806 2023-07-17 16:36:22.000000 ex4nicegui-0.1.9/ex4nicegui/reactive/officials.py
--rw-rw-rw-   0        0        0     1217 2023-07-16 10:54:22.000000 ex4nicegui-0.1.9/ex4nicegui/reactive/q_pagination.py
--rw-rw-rw-   0        0        0       24 2023-07-09 14:56:08.000000 ex4nicegui-0.1.9/ex4nicegui/reactive/rxui.py
-drwxrwxrwx   0        0        0        0 2023-07-17 16:37:56.654792 ex4nicegui-0.1.9/ex4nicegui/reactive/useMouse/
--rw-rw-rw-   0        0        0     2722 2023-07-17 15:14:14.000000 ex4nicegui-0.1.9/ex4nicegui/reactive/useMouse/UseMouse.js
--rw-rw-rw-   0        0        0     2580 2023-07-17 16:36:22.000000 ex4nicegui-0.1.9/ex4nicegui/reactive/useMouse/UseMouse.py
--rw-rw-rw-   0        0        0        0 2023-07-08 17:55:18.000000 ex4nicegui-0.1.9/ex4nicegui/reactive/useMouse/__init__.py
--rw-rw-rw-   0        0        0     2093 2023-07-14 15:33:47.000000 ex4nicegui-0.1.9/ex4nicegui/reactive/usePagination.py
-drwxrwxrwx   0        0        0        0 2023-07-17 16:37:56.658458 ex4nicegui-0.1.9/ex4nicegui/tools/
--rw-rw-rw-   0        0        0       40 2023-07-08 17:55:18.000000 ex4nicegui-0.1.9/ex4nicegui/tools/__init__.py
--rw-rw-rw-   0        0        0     4887 2023-07-10 13:40:51.000000 ex4nicegui-0.1.9/ex4nicegui/tools/debug.py
-drwxrwxrwx   0        0        0        0 2023-07-17 16:37:56.663448 ex4nicegui-0.1.9/ex4nicegui/utils/
--rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.1.9/ex4nicegui/utils/__init__.py
--rw-rw-rw-   0        0        0      430 2023-07-08 17:55:18.000000 ex4nicegui-0.1.9/ex4nicegui/utils/common.py
--rw-rw-rw-   0        0        0     4807 2023-07-10 14:31:39.000000 ex4nicegui-0.1.9/ex4nicegui/utils/signals.py
-drwxrwxrwx   0        0        0        0 2023-07-17 16:37:56.615924 ex4nicegui-0.1.9/ex4nicegui.egg-info/
--rw-rw-rw-   0        0        0      481 2023-07-17 16:37:56.000000 ex4nicegui-0.1.9/ex4nicegui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1101 2023-07-17 16:37:56.000000 ex4nicegui-0.1.9/ex4nicegui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 16:37:56.000000 ex4nicegui-0.1.9/ex4nicegui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-17 16:37:56.000000 ex4nicegui-0.1.9/ex4nicegui.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       46 2023-07-17 16:37:56.000000 ex4nicegui-0.1.9/ex4nicegui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-17 16:37:56.000000 ex4nicegui-0.1.9/ex4nicegui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-17 16:37:56.666440 ex4nicegui-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0     1501 2023-07-16 10:54:22.000000 ex4nicegui-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 11:03:07.460701 ex4nicegui-0.2.0/
+-rw-rw-rw-   0        0        0     1094 2023-06-30 08:17:10.000000 ex4nicegui-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      481 2023-07-18 11:03:07.460350 ex4nicegui-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2200 2023-07-10 15:25:21.000000 ex4nicegui-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 11:03:07.391450 ex4nicegui-0.2.0/ex4nicegui/
+-rw-rw-rw-   0        0        0      337 2023-07-18 10:52:31.000000 ex4nicegui-0.2.0/ex4nicegui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 11:03:07.408824 ex4nicegui-0.2.0/ex4nicegui/layout/
+-rw-rw-rw-   0        0        0       31 2023-07-05 06:10:00.000000 ex4nicegui-0.2.0/ex4nicegui/layout/__init__.py
+-rw-rw-rw-   0        0        0     2378 2023-07-05 06:10:00.000000 ex4nicegui-0.2.0/ex4nicegui/layout/gridbox.py
+drwxrwxrwx   0        0        0        0 2023-07-18 11:03:07.425785 ex4nicegui-0.2.0/ex4nicegui/reactive/
+drwxrwxrwx   0        0        0        0 2023-07-18 11:03:07.435758 ex4nicegui-0.2.0/ex4nicegui/reactive/ECharts/
+-rw-rw-rw-   0        0        0  1581614 2023-07-17 15:29:41.000000 ex4nicegui-0.2.0/ex4nicegui/reactive/ECharts/ECharts.js
+-rw-rw-rw-   0        0        0     2550 2023-07-17 16:36:22.000000 ex4nicegui-0.2.0/ex4nicegui/reactive/ECharts/ECharts.py
+-rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.2.0/ex4nicegui/reactive/ECharts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 11:03:07.441742 ex4nicegui-0.2.0/ex4nicegui/reactive/UseDraggable/
+-rw-rw-rw-   0        0        0     4857 2023-07-17 16:36:22.000000 ex4nicegui-0.2.0/ex4nicegui/reactive/UseDraggable/UseDraggable.js
+-rw-rw-rw-   0        0        0     2888 2023-07-17 16:36:22.000000 ex4nicegui-0.2.0/ex4nicegui/reactive/UseDraggable/UseDraggable.py
+-rw-rw-rw-   0        0        0        0 2023-07-17 16:36:22.000000 ex4nicegui-0.2.0/ex4nicegui/reactive/UseDraggable/__init__.py
+-rw-rw-rw-   0        0        0     1340 2023-07-18 10:52:11.000000 ex4nicegui-0.2.0/ex4nicegui/reactive/__index.py
+-rw-rw-rw-   0        0        0       24 2023-07-05 06:10:00.000000 ex4nicegui-0.2.0/ex4nicegui/reactive/__init__.py
+-rw-rw-rw-   0        0        0     1356 2023-07-16 10:54:22.000000 ex4nicegui-0.2.0/ex4nicegui/reactive/drawer.py
+-rw-rw-rw-   0        0        0     6093 2023-07-16 10:54:22.000000 ex4nicegui-0.2.0/ex4nicegui/reactive/local_file_picker.py
+-rw-rw-rw-   0        0        0    40577 2023-07-18 10:52:11.000000 ex4nicegui-0.2.0/ex4nicegui/reactive/officials.py
+-rw-rw-rw-   0        0        0     1217 2023-07-16 10:54:22.000000 ex4nicegui-0.2.0/ex4nicegui/reactive/q_pagination.py
+-rw-rw-rw-   0        0        0       24 2023-07-09 14:56:08.000000 ex4nicegui-0.2.0/ex4nicegui/reactive/rxui.py
+drwxrwxrwx   0        0        0        0 2023-07-18 11:03:07.447727 ex4nicegui-0.2.0/ex4nicegui/reactive/useMouse/
+-rw-rw-rw-   0        0        0     2722 2023-07-17 15:14:14.000000 ex4nicegui-0.2.0/ex4nicegui/reactive/useMouse/UseMouse.js
+-rw-rw-rw-   0        0        0     2580 2023-07-17 16:36:22.000000 ex4nicegui-0.2.0/ex4nicegui/reactive/useMouse/UseMouse.py
+-rw-rw-rw-   0        0        0        0 2023-07-08 17:55:18.000000 ex4nicegui-0.2.0/ex4nicegui/reactive/useMouse/__init__.py
+-rw-rw-rw-   0        0        0     2093 2023-07-14 15:33:47.000000 ex4nicegui-0.2.0/ex4nicegui/reactive/usePagination.py
+drwxrwxrwx   0        0        0        0 2023-07-18 11:03:07.451717 ex4nicegui-0.2.0/ex4nicegui/tools/
+-rw-rw-rw-   0        0        0       40 2023-07-08 17:55:18.000000 ex4nicegui-0.2.0/ex4nicegui/tools/__init__.py
+-rw-rw-rw-   0        0        0     4887 2023-07-10 13:40:51.000000 ex4nicegui-0.2.0/ex4nicegui/tools/debug.py
+drwxrwxrwx   0        0        0        0 2023-07-18 11:03:07.458321 ex4nicegui-0.2.0/ex4nicegui/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-05 06:10:00.000000 ex4nicegui-0.2.0/ex4nicegui/utils/__init__.py
+-rw-rw-rw-   0        0        0      430 2023-07-08 17:55:18.000000 ex4nicegui-0.2.0/ex4nicegui/utils/common.py
+-rw-rw-rw-   0        0        0     4807 2023-07-10 14:31:39.000000 ex4nicegui-0.2.0/ex4nicegui/utils/signals.py
+drwxrwxrwx   0        0        0        0 2023-07-18 11:03:07.404836 ex4nicegui-0.2.0/ex4nicegui.egg-info/
+-rw-rw-rw-   0        0        0      481 2023-07-18 11:03:07.000000 ex4nicegui-0.2.0/ex4nicegui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1101 2023-07-18 11:03:07.000000 ex4nicegui-0.2.0/ex4nicegui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 11:03:07.000000 ex4nicegui-0.2.0/ex4nicegui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-18 11:03:07.000000 ex4nicegui-0.2.0/ex4nicegui.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       46 2023-07-18 11:03:07.000000 ex4nicegui-0.2.0/ex4nicegui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-18 11:03:07.000000 ex4nicegui-0.2.0/ex4nicegui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 11:03:07.461701 ex4nicegui-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1501 2023-07-18 10:52:21.000000 ex4nicegui-0.2.0/setup.py
```

### Comparing `ex4nicegui-0.1.9/LICENSE` & `ex4nicegui-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.9/README.md` & `ex4nicegui-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.9/ex4nicegui/layout/gridbox.py` & `ex4nicegui-0.2.0/ex4nicegui/layout/gridbox.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.9/ex4nicegui/reactive/ECharts/ECharts.js` & `ex4nicegui-0.2.0/ex4nicegui/reactive/ECharts/ECharts.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.9/ex4nicegui/reactive/ECharts/ECharts.py` & `ex4nicegui-0.2.0/ex4nicegui/reactive/ECharts/ECharts.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.9/ex4nicegui/reactive/UseDraggable/UseDraggable.js` & `ex4nicegui-0.2.0/ex4nicegui/reactive/UseDraggable/UseDraggable.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.9/ex4nicegui/reactive/UseDraggable/UseDraggable.py` & `ex4nicegui-0.2.0/ex4nicegui/reactive/UseDraggable/UseDraggable.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.9/ex4nicegui/reactive/__index.py` & `ex4nicegui-0.2.0/ex4nicegui/reactive/__index.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,18 @@
     CardActionsBindableUi as card_actions,
     SliderBindableUi as slider,
     LazySliderBindableUi as lazy_slider,
     HtmlBindableUi as html,
     ImageBindableUi as image,
     UploadBindableUi as upload,
     UploadResult,
+    DrawerBindableUi as drawer,
 )
 from .q_pagination import QPagination as q_pagination
 from .local_file_picker import local_file_picker
 from ex4nicegui.utils.signals import ref_computed
 from signe import effect
 from .UseDraggable.UseDraggable import use_draggable
 from .useMouse.UseMouse import use_mouse
-from .drawer import drawer
+
+# from .drawer import drawer
 from .usePagination import PaginationRef as use_pagination
```

### Comparing `ex4nicegui-0.1.9/ex4nicegui/reactive/drawer.py` & `ex4nicegui-0.2.0/ex4nicegui/reactive/drawer.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.9/ex4nicegui/reactive/local_file_picker.py` & `ex4nicegui-0.2.0/ex4nicegui/reactive/local_file_picker.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.9/ex4nicegui/reactive/officials.py` & `ex4nicegui-0.2.0/ex4nicegui/reactive/officials.py`

 * *Files 1% similar despite different names*

```diff
@@ -1105,18 +1105,81 @@
             ele = self.element
             ele._props["columns"] = ref_ui.value
             ele.update()
 
         return self
 
 
+_TDrawerSide = Literal["left", "right"]
+
+
 class DrawerBindableUi(SingleValueBindableUi[bool, Drawer]):
-    def __init__(self, value: bool, element: Drawer) -> None:
+    def __init__(
+        self,
+        side: TMaybeRef[_TDrawerSide] = "left",
+        overlay: TMaybeRef[bool] = False,
+        *,
+        value: TMaybeRef[bool] = True,
+        fixed: TMaybeRef[bool] = False,
+        bordered: TMaybeRef[bool] = True,
+        elevated: TMaybeRef[bool] = False,
+        top_corner: TMaybeRef[bool] = False,
+        bottom_corner: TMaybeRef[bool] = False,
+    ) -> None:
+        kws = {
+            "side": side,
+            "overlay": overlay,
+            "value": value,
+            "fixed": fixed,
+            "bordered": bordered,
+            "elevated": elevated,
+            "top_corner": top_corner,
+            "bottom_corner": bottom_corner,
+        }
+
+        value_kws = _convert_kws_ref2value(kws)
+        del value_kws["side"]
+        del value_kws["overlay"]
+
+        element = None
+
+        if to_value(side) == "left":
+            element = ui.left_drawer(**value_kws)
+        else:
+            element = ui.right_drawer(**value_kws)
+
+        element.style(f"background-color:rgba(25, 118, 210,0.3)")
+        element.classes("flex flex-col gap-4")
+
+        init_value = (
+            element._props["model-value"]
+            if "model-value" in element._props
+            else element._props["show-if-above"]
+        )
+
         super().__init__(value, element)
 
+        @effect
+        def _():
+            value = "true" if self.value else "false"
+            element.props(f":model-value={value}")
+
+        def on_update(e):
+            self._ref.value = e.args
+
+        element.on("update:modelValue", on_update)
+
+        for key, value in kws.items():
+            if is_ref(value):
+                self.bind_prop(key, value)  # type: ignore
+
+    def toggle(self):
+        self.element.toggle()
+        return self
+
     def __enter__(self):
         self.element.__enter__()
         return self
 
     def __exit__(self, *_: Any):
         self.element.__exit__(*_)
```

### Comparing `ex4nicegui-0.1.9/ex4nicegui/reactive/q_pagination.py` & `ex4nicegui-0.2.0/ex4nicegui/reactive/q_pagination.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.9/ex4nicegui/reactive/useMouse/UseMouse.js` & `ex4nicegui-0.2.0/ex4nicegui/reactive/useMouse/UseMouse.js`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.9/ex4nicegui/reactive/useMouse/UseMouse.py` & `ex4nicegui-0.2.0/ex4nicegui/reactive/useMouse/UseMouse.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.9/ex4nicegui/reactive/usePagination.py` & `ex4nicegui-0.2.0/ex4nicegui/reactive/usePagination.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.9/ex4nicegui/tools/debug.py` & `ex4nicegui-0.2.0/ex4nicegui/tools/debug.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.9/ex4nicegui/utils/signals.py` & `ex4nicegui-0.2.0/ex4nicegui/utils/signals.py`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.9/ex4nicegui.egg-info/SOURCES.txt` & `ex4nicegui-0.2.0/ex4nicegui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ex4nicegui-0.1.9/setup.py` & `ex4nicegui-0.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     return list(all_infos)
 
 
 with open("README.md", encoding="utf8") as readme_file:
     readme = readme_file.read()
 
-requirements = ["signe>=0.1.8", "nicegui>=1.3.3", "typing_extensions"]
+requirements = ["signe>=0.1.8", "nicegui>=1.3.4", "typing_extensions"]
 
 test_requirements = ["pytest>=3"]
 
 setup(
     author="carson_jia",
     author_email="568166495@qq.com",
     python_requires=">=3.7",
```

