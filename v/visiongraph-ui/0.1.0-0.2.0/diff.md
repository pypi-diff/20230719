# Comparing `tmp/visiongraph_ui-0.1.0-py3-none-any.whl.zip` & `tmp/visiongraph_ui-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,22 @@
-Zip file size: 8722 bytes, number of entries: 17
--rw-r--r--  2.0 unx      476 b- defN 23-Apr-28 10:43 visiongui/AppContext.py
--rw-r--r--  2.0 unx      218 b- defN 23-Apr-28 10:43 visiongui/__init__.py
--rw-r--r--  2.0 unx     3880 b- defN 23-Apr-28 10:43 visiongui/app/BaseApp.py
--rw-r--r--  2.0 unx     1252 b- defN 23-Apr-28 10:43 visiongui/app/VisionGraphApp.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-28 10:43 visiongui/app/__init__.py
--rw-r--r--  2.0 unx     1344 b- defN 23-Apr-28 10:43 visiongui/configuration/ConfigurationDialog.py
--rw-r--r--  2.0 unx      742 b- defN 23-Apr-28 10:43 visiongui/configuration/InputConfiguration.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-28 10:43 visiongui/configuration/__init__.py
--rw-r--r--  2.0 unx     1105 b- defN 23-Apr-28 10:43 visiongui/utils/ImageWidgetHelper.py
--rw-r--r--  2.0 unx     1329 b- defN 23-Apr-28 10:43 visiongui/utils/KeyStrokeDetector.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-28 10:43 visiongui/utils/__init__.py
--rw-r--r--  2.0 unx     3519 b- defN 23-Apr-28 10:43 visiongui/widgets/ApplicationMenu.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-28 10:43 visiongui/widgets/__init__.py
--rw-r--r--  2.0 unx     1147 b- defN 23-Apr-28 10:43 visiongraph_ui-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-28 10:43 visiongraph_ui-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Apr-28 10:43 visiongraph_ui-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1466 b- defN 23-Apr-28 10:43 visiongraph_ui-0.1.0.dist-info/RECORD
-17 files, 16580 bytes uncompressed, 6268 bytes compressed:  62.2%
+Zip file size: 10832 bytes, number of entries: 20
+-rw-r--r--  2.0 unx      218 b- defN 23-Jul-19 08:57 visiongui/__init__.py
+-rw-r--r--  2.0 unx      921 b- defN 23-Jul-19 08:57 visiongui/app/VisiongraphApp.py
+-rw-r--r--  2.0 unx     2070 b- defN 23-Jul-19 08:57 visiongui/app/VisiongraphAppLauncher.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 08:57 visiongui/app/__init__.py
+-rw-r--r--  2.0 unx     1344 b- defN 23-Jul-19 08:57 visiongui/configuration/ConfigurationDialog.py
+-rw-r--r--  2.0 unx      742 b- defN 23-Jul-19 08:57 visiongui/configuration/InputConfiguration.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 08:57 visiongui/configuration/__init__.py
+-rw-r--r--  2.0 unx     3960 b- defN 23-Jul-19 08:57 visiongui/ui/BaseUserInterface.py
+-rw-r--r--  2.0 unx      475 b- defN 23-Jul-19 08:57 visiongui/ui/UIContext.py
+-rw-r--r--  2.0 unx     1601 b- defN 23-Jul-19 08:57 visiongui/ui/VisiongraphUserInterface.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 08:57 visiongui/ui/__init__.py
+-rw-r--r--  2.0 unx     1105 b- defN 23-Jul-19 08:57 visiongui/utils/ImageWidgetHelper.py
+-rw-r--r--  2.0 unx     1329 b- defN 23-Jul-19 08:57 visiongui/utils/KeyStrokeDetector.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 08:57 visiongui/utils/__init__.py
+-rw-r--r--  2.0 unx     3517 b- defN 23-Jul-19 08:57 visiongui/widgets/ApplicationMenu.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-19 08:57 visiongui/widgets/__init__.py
+-rw-r--r--  2.0 unx     2327 b- defN 23-Jul-19 08:57 visiongraph_ui-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-19 08:57 visiongraph_ui-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Jul-19 08:57 visiongraph_ui-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1747 b- defN 23-Jul-19 08:57 visiongraph_ui-0.2.0.dist-info/RECORD
+20 files, 21458 bytes uncompressed, 7922 bytes compressed:  63.1%
```

## zipnote {}

```diff
@@ -1,31 +1,40 @@
-Filename: visiongui/AppContext.py
-Comment: 
-
 Filename: visiongui/__init__.py
 Comment: 
 
-Filename: visiongui/app/BaseApp.py
+Filename: visiongui/app/VisiongraphApp.py
 Comment: 
 
-Filename: visiongui/app/VisionGraphApp.py
+Filename: visiongui/app/VisiongraphAppLauncher.py
 Comment: 
 
 Filename: visiongui/app/__init__.py
 Comment: 
 
 Filename: visiongui/configuration/ConfigurationDialog.py
 Comment: 
 
 Filename: visiongui/configuration/InputConfiguration.py
 Comment: 
 
 Filename: visiongui/configuration/__init__.py
 Comment: 
 
+Filename: visiongui/ui/BaseUserInterface.py
+Comment: 
+
+Filename: visiongui/ui/UIContext.py
+Comment: 
+
+Filename: visiongui/ui/VisiongraphUserInterface.py
+Comment: 
+
+Filename: visiongui/ui/__init__.py
+Comment: 
+
 Filename: visiongui/utils/ImageWidgetHelper.py
 Comment: 
 
 Filename: visiongui/utils/KeyStrokeDetector.py
 Comment: 
 
 Filename: visiongui/utils/__init__.py
@@ -33,20 +42,20 @@
 
 Filename: visiongui/widgets/ApplicationMenu.py
 Comment: 
 
 Filename: visiongui/widgets/__init__.py
 Comment: 
 
-Filename: visiongraph_ui-0.1.0.dist-info/METADATA
+Filename: visiongraph_ui-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: visiongraph_ui-0.1.0.dist-info/WHEEL
+Filename: visiongraph_ui-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: visiongraph_ui-0.1.0.dist-info/top_level.txt
+Filename: visiongraph_ui-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: visiongraph_ui-0.1.0.dist-info/RECORD
+Filename: visiongraph_ui-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## visiongui/widgets/ApplicationMenu.py

```diff
@@ -21,20 +21,20 @@
         self.window: Optional[gui.Window] = None
 
         self.on_open_settings: Event[Path] = Event()
         self.on_save_settings: Event[Path] = Event()
         self.on_about: Event[ApplicationMenu] = Event()
 
     def __enter__(self):
-        # on windows & linux attach before app creation
+        # on windows & linux attach before ui creation
         if not OSUtils.isMacOSX():
             gui.Application.instance.menubar = self.create_menu_bar()
 
     def __exit__(self, exc_type: Any, exc_val: Any, exc_tb: Any):
-        # on macOS attach after app creation
+        # on macOS attach after ui creation
         if OSUtils.isMacOSX():
             gui.Application.instance.menubar = self.create_menu_bar()
 
     def create_menu_bar(self) -> Optional[gui.Menu]:
         if gui.Application.instance.menubar is not None:
             return None
```

## Comparing `visiongui/app/BaseApp.py` & `visiongui/ui/BaseUserInterface.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,31 +11,31 @@
 
 from visiongui.utils.KeyStrokeDetector import KeyStrokeDetector
 from visiongui.widgets.ApplicationMenu import ApplicationMenu
 
 T = TypeVar("T", bound=Any)
 
 
-class BaseApp(Generic[T], ABC):
+class BaseUserInterface(Generic[T], ABC):
 
     def __init__(self, config: T, title: str, width: int = 800, height: int = 600,
                  attach_interrupt_handler: bool = False):
         self.config = config
         self.title = title
 
-        # setup app and menu
+        # setup ui and menu
         self.menu = ApplicationMenu(title)
         with self.menu:
             self.window: gui.Window = gui.Application.instance.create_window(title, width, height)
         self.menu.attach_menu_handlers(self.window)
         self.menu.on_about = self._on_menu_about
 
         self.em = self.window.theme.font_size
 
-        # setup app hooks
+        # setup ui hooks
         self.window.set_on_layout(self._on_layout)
         self.window.set_on_close(self._on_close)
 
         # setup hot keys
         self.key_detector = KeyStrokeDetector()
         self._setup_hotkeys(self.key_detector)
 
@@ -94,8 +94,12 @@
     def placeholder_image(self) -> np.ndarray:
         return np.zeros(shape=(1, 1, 3), dtype="uint8")
 
     def invoke_on_gui(self, callback: Callable[[], None]):
         gui.Application.instance.post_to_main_thread(self.window, callback)
 
     def _on_menu_about(self, sender: Any):
-        self.window.show_message_box("About", f"Hello from {self.title}")
+        self.window.show_message_box("About", self.about_text)
+
+    @property
+    def about_text(self):
+        return f"Hello from {self.title}"
```

