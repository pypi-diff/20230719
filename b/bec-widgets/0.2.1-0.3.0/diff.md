# Comparing `tmp/bec_widgets-0.2.1.tar.gz` & `tmp/bec_widgets-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bec_widgets-0.2.1.tar", last modified: Thu Jul 13 16:38:43 2023, max compression
+gzip compressed data, was "bec_widgets-0.3.0.tar", last modified: Wed Jul 19 08:46:04 2023, max compression
```

## Comparing `bec_widgets-0.2.1.tar` & `bec_widgets-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 16:38:43.157457 bec_widgets-0.2.1/
--rw-r--r--   0 root         (0) root         (0)      452 2023-07-13 16:38:43.157457 bec_widgets-0.2.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       15 2023-07-11 13:21:08.000000 bec_widgets-0.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 16:38:43.156457 bec_widgets-0.2.1/bec_widgets/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 16:17:29.000000 bec_widgets-0.2.1/bec_widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2928 2023-07-13 15:18:08.000000 bec_widgets-0.2.1/bec_widgets/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     3926 2023-07-13 16:32:38.000000 bec_widgets-0.2.1/bec_widgets/config_plotter.py
--rw-r--r--   0 root         (0) root         (0)     3345 2023-07-13 16:38:30.000000 bec_widgets-0.2.1/bec_widgets/scan_plot.py
--rw-r--r--   0 root         (0) root         (0)     1355 2023-07-13 15:18:08.000000 bec_widgets-0.2.1/bec_widgets/scan_plot_plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 16:38:43.157457 bec_widgets-0.2.1/bec_widgets.egg-info/
--rw-r--r--   0 root         (0) root         (0)      452 2023-07-13 16:38:43.000000 bec_widgets-0.2.1/bec_widgets.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      342 2023-07-13 16:38:43.000000 bec_widgets-0.2.1/bec_widgets.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 16:38:43.000000 bec_widgets-0.2.1/bec_widgets.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       83 2023-07-13 16:38:43.000000 bec_widgets-0.2.1/bec_widgets.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-13 16:38:43.000000 bec_widgets-0.2.1/bec_widgets.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      505 2023-07-13 16:38:43.157457 bec_widgets-0.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      287 2023-07-13 16:38:41.000000 bec_widgets-0.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 08:46:04.002132 bec_widgets-0.3.0/
+-rw-r--r--   0 root         (0) root         (0)     1511 2023-07-13 20:38:14.000000 bec_widgets-0.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      490 2023-07-19 08:46:04.002132 bec_widgets-0.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       15 2023-07-11 13:21:47.000000 bec_widgets-0.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 08:46:04.000132 bec_widgets-0.3.0/bec_widgets/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-11 16:17:30.000000 bec_widgets-0.3.0/bec_widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2929 2023-07-13 20:24:17.000000 bec_widgets-0.3.0/bec_widgets/cli.py
+-rw-r--r--   0 root         (0) root         (0)     3963 2023-07-13 20:24:17.000000 bec_widgets-0.3.0/bec_widgets/config_plotter.py
+-rw-r--r--   0 root         (0) root         (0)     1067 2023-07-19 08:45:51.000000 bec_widgets-0.3.0/bec_widgets/ctrl_c.py
+-rw-r--r--   0 root         (0) root         (0)     9980 2023-07-19 08:45:51.000000 bec_widgets-0.3.0/bec_widgets/line_plot.py
+-rw-rw-rw-   0 root         (0) root         (0)     3345 2023-07-13 16:32:38.000000 bec_widgets-0.3.0/bec_widgets/scan_plot.py
+-rw-r--r--   0 root         (0) root         (0)     1357 2023-07-13 20:24:17.000000 bec_widgets-0.3.0/bec_widgets/scan_plot_plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 08:46:04.001132 bec_widgets-0.3.0/bec_widgets.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      490 2023-07-19 08:46:03.000000 bec_widgets-0.3.0/bec_widgets.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      401 2023-07-19 08:46:03.000000 bec_widgets-0.3.0/bec_widgets.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 08:46:03.000000 bec_widgets-0.3.0/bec_widgets.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       83 2023-07-19 08:46:03.000000 bec_widgets-0.3.0/bec_widgets.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-19 08:46:03.000000 bec_widgets-0.3.0/bec_widgets.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      521 2023-07-19 08:46:04.002132 bec_widgets-0.3.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      287 2023-07-19 08:46:02.000000 bec_widgets-0.3.0/setup.py
```

### Comparing `bec_widgets-0.2.1/bec_widgets/cli.py` & `bec_widgets-0.3.0/bec_widgets/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import argparse
 import os
 from threading import RLock
 
+from bec_lib.core import BECMessage, MessageEndpoints, RedisConnector
 from PyQt5 import uic
 from PyQt5.QtCore import pyqtSignal
 from PyQt5.QtWidgets import QApplication, QMainWindow
-from scan_plot import BECScanPlot
 
-from bec_lib.core import BECMessage, MessageEndpoints, RedisConnector
+from .scan_plot import BECScanPlot
 
 
 class BEC_UI(QMainWindow):
     new_scan_data = pyqtSignal(dict)
     new_dap_data = pyqtSignal(dict)  # signal per proc instance?
     new_scan = pyqtSignal()
```

### Comparing `bec_widgets-0.2.1/bec_widgets/config_plotter.py` & `bec_widgets-0.3.0/bec_widgets/config_plotter.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,16 @@
         self.plots = {}
         self._init_ui()
         self._init_plots()
 
     def _init_ui(self):
         pg.setConfigOption("background", "w")
         pg.setConfigOption("foreground", "k")
+
+        # pylint: disable=no-member
         self.pen = mkPen(color=(56, 76, 107), width=4, style=QtCore.Qt.SolidLine)
 
         self.view = pg.GraphicsView()
         self.view.setAntialiasing(True)
         self.view.show()
 
         self.layout = pg.GraphicsLayout()
```

### Comparing `bec_widgets-0.2.1/bec_widgets/scan_plot.py` & `bec_widgets-0.3.0/bec_widgets/scan_plot.py`

 * *Files identical despite different names*

### Comparing `bec_widgets-0.2.1/bec_widgets/scan_plot_plugin.py` & `bec_widgets-0.3.0/bec_widgets/scan_plot_plugin.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from PyQt5.QtDesigner import QPyDesignerCustomWidgetPlugin
 from PyQt5.QtGui import QIcon
-from scan_plot import BECScanPlot
+
+from .scan_plot import BECScanPlot
 
 
 class BECScanPlotPlugin(QPyDesignerCustomWidgetPlugin):
     def __init__(self, parent=None):
         super(BECScanPlotPlugin, self).__init__(parent)
 
         self._initialized = False
```

