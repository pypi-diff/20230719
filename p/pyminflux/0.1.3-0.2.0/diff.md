# Comparing `tmp/pyminflux-0.1.3.tar.gz` & `tmp/pyminflux-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyminflux-0.1.3.tar", max compression
+gzip compressed data, was "pyminflux-0.2.0.tar", max compression
```

## Comparing `pyminflux-0.1.3.tar` & `pyminflux-0.2.0.tar`

### file list

```diff
@@ -1,67 +1,76 @@
--rw-r--r--   0        0        0    11358 2023-05-02 11:32:56.697662 pyminflux-0.1.3/LICENSE.txt
--rw-r--r--   0        0        0     2906 2023-05-26 06:57:45.887624 pyminflux-0.1.3/README.md
--rw-r--r--   0        0        0      778 2023-05-26 08:45:53.133825 pyminflux-0.1.3/pyminflux/__init__.py
--rw-r--r--   0        0        0      817 2023-05-02 11:32:56.701662 pyminflux-0.1.3/pyminflux/analysis/__init__.py
--rw-r--r--   0        0        0    14408 2023-05-02 11:32:56.701662 pyminflux-0.1.3/pyminflux/analysis/_analysis.py
--rw-r--r--   0        0        0      638 2023-05-02 11:32:56.701662 pyminflux-0.1.3/pyminflux/base/__init__.py
--rw-r--r--   0        0        0      918 2023-05-02 11:32:56.701662 pyminflux-0.1.3/pyminflux/base/_base.py
--rw-r--r--   0        0        0     1081 2023-05-03 07:24:53.358703 pyminflux-0.1.3/pyminflux/main.py
--rw-r--r--   0        0        0      650 2023-05-02 11:32:56.701662 pyminflux-0.1.3/pyminflux/processor/__init__.py
--rw-r--r--   0        0        0    27962 2023-05-08 08:01:47.198555 pyminflux-0.1.3/pyminflux/processor/_processor.py
--rw-r--r--   0        0        0      644 2023-05-02 11:32:56.701662 pyminflux-0.1.3/pyminflux/reader/__init__.py
--rw-r--r--   0        0        0    20819 2023-05-26 08:45:53.137825 pyminflux-0.1.3/pyminflux/reader/_reader.py
--rw-r--r--   0        0        0   139482 2023-05-02 11:32:56.705662 pyminflux-0.1.3/pyminflux/resources.py
--rw-r--r--   0        0        0      747 2023-05-02 11:32:56.705662 pyminflux-0.1.3/pyminflux/resources.qrc
--rw-r--r--   0        0        0      641 2023-05-02 11:32:56.705662 pyminflux-0.1.3/pyminflux/settings/__init__.py
--rw-r--r--   0        0        0     1679 2023-05-02 11:32:56.705662 pyminflux-0.1.3/pyminflux/settings/_settings.py
--rw-r--r--   0        0        0      646 2023-05-02 11:32:56.705662 pyminflux-0.1.3/pyminflux/state/__init__.py
--rw-r--r--   0        0        0     5875 2023-05-26 08:45:53.137825 pyminflux-0.1.3/pyminflux/state/_state.py
--rw-r--r--   0        0        0      633 2023-05-02 11:32:56.705662 pyminflux-0.1.3/pyminflux/threads/__init__.py
--rw-r--r--   0        0        0      875 2023-05-02 11:32:56.705662 pyminflux-0.1.3/pyminflux/threads/_threads.py
--rw-r--r--   0        0        0      608 2023-05-02 11:32:56.705662 pyminflux-0.1.3/pyminflux/ui/__init__.py
--rw-r--r--   0        0        0    31233 2023-05-26 08:45:53.137825 pyminflux-0.1.3/pyminflux/ui/analyzer.py
--rw-r--r--   0        0        0     9033 2023-05-26 08:45:53.137825 pyminflux-0.1.3/pyminflux/ui/analyzer.ui
--rw-r--r--   0        0        0   216854 2023-05-02 11:32:56.857662 pyminflux-0.1.3/pyminflux/ui/assets/Logo_v3.icns
--rw-r--r--   0        0        0  1143198 2023-05-02 11:32:56.861662 pyminflux-0.1.3/pyminflux/ui/assets/Logo_v3.ico
--rwxr-xr-x   0        0        0    43531 2023-05-02 11:32:56.861662 pyminflux-0.1.3/pyminflux/ui/assets/Logo_v3.png
--rw-r--r--   0        0        0     8998 2023-05-03 14:33:18.090905 pyminflux-0.1.3/pyminflux/ui/assets/Logo_v3_small.png
--rwxr-xr-x   0        0        0      670 2023-05-02 11:32:56.709662 pyminflux-0.1.3/pyminflux/ui/assets/create_resources.sh
--rwxr-xr-x   0        0        0     1805 2023-05-02 11:32:56.709662 pyminflux-0.1.3/pyminflux/ui/assets/png_to_icns.sh
--rw-r--r--   0        0        0    12299 2023-05-26 08:45:53.137825 pyminflux-0.1.3/pyminflux/ui/color_unmixer.py
--rw-r--r--   0        0        0     8732 2023-05-26 08:45:53.137825 pyminflux-0.1.3/pyminflux/ui/color_unmixer.ui
--rw-r--r--   0        0        0     2561 2023-05-02 11:57:29.698894 pyminflux-0.1.3/pyminflux/ui/dataviewer.py
--rw-r--r--   0        0        0     1008 2023-05-02 11:32:56.713662 pyminflux-0.1.3/pyminflux/ui/emittingstream.py
--rw-r--r--   0        0        0      670 2023-05-26 08:45:53.137825 pyminflux-0.1.3/pyminflux/ui/helpers/__init__.py
--rw-r--r--   0        0        0     2994 2023-05-26 08:45:53.137825 pyminflux-0.1.3/pyminflux/ui/helpers/_helpers.py
--rwxr-xr-x   0        0        0    43531 2023-05-02 11:32:56.861662 pyminflux-0.1.3/pyminflux/ui/icons/icon.png
--rw-r--r--   0        0        0    31809 2023-05-26 08:45:53.141826 pyminflux-0.1.3/pyminflux/ui/main_window.py
--rw-r--r--   0        0        0     4739 2023-05-26 08:45:53.141826 pyminflux-0.1.3/pyminflux/ui/main_window.ui
--rw-r--r--   0        0        0    18839 2023-05-26 08:45:53.141826 pyminflux-0.1.3/pyminflux/ui/options.py
--rw-r--r--   0        0        0    18392 2023-05-26 08:45:53.141826 pyminflux-0.1.3/pyminflux/ui/options.ui
--rw-r--r--   0        0        0     2057 2023-05-02 11:32:56.713662 pyminflux-0.1.3/pyminflux/ui/pandas_datamodel.py
--rw-r--r--   0        0        0    14082 2023-05-26 08:45:53.141826 pyminflux-0.1.3/pyminflux/ui/plotter.py
--rw-r--r--   0        0        0     3473 2023-05-12 11:10:11.402890 pyminflux-0.1.3/pyminflux/ui/plotter_3d.py
--rw-r--r--   0        0        0      544 2023-05-02 11:32:56.713662 pyminflux-0.1.3/pyminflux/ui/plotter_3d.ui
--rw-r--r--   0        0        0     4775 2023-05-02 11:32:56.713662 pyminflux-0.1.3/pyminflux/ui/plotter_toolbar.py
--rw-r--r--   0        0        0     3254 2023-05-02 11:32:56.713662 pyminflux-0.1.3/pyminflux/ui/plotter_toolbar.ui
--rw-r--r--   0        0        0     4125 2023-05-02 11:32:56.713662 pyminflux-0.1.3/pyminflux/ui/roi_ranges.py
--rw-r--r--   0        0        0     4422 2023-04-26 08:29:10.942459 pyminflux-0.1.3/pyminflux/ui/roi_ranges.ui
--rw-r--r--   0        0        0    18534 2023-05-26 08:45:53.141826 pyminflux-0.1.3/pyminflux/ui/time_inspector.py
--rw-r--r--   0        0        0     3128 2023-04-26 08:29:10.942459 pyminflux-0.1.3/pyminflux/ui/time_inspector.ui
--rw-r--r--   0        0        0    10646 2023-05-26 08:45:53.141826 pyminflux-0.1.3/pyminflux/ui/ui_analyzer.py
--rw-r--r--   0        0        0     9840 2023-05-26 08:45:53.141826 pyminflux-0.1.3/pyminflux/ui/ui_color_unmixer.py
--rw-r--r--   0        0        0     8318 2023-05-26 08:45:53.141826 pyminflux-0.1.3/pyminflux/ui/ui_main_window.py
--rw-r--r--   0        0        0    22391 2023-05-26 08:45:53.145825 pyminflux-0.1.3/pyminflux/ui/ui_options.py
--rw-r--r--   0        0        0     2276 2023-05-02 11:32:56.717662 pyminflux-0.1.3/pyminflux/ui/ui_plotter_3d.py
--rw-r--r--   0        0        0     5670 2023-05-02 11:32:56.717662 pyminflux-0.1.3/pyminflux/ui/ui_plotter_toolbar.py
--rw-r--r--   0        0        0     5773 2023-05-02 11:32:56.717662 pyminflux-0.1.3/pyminflux/ui/ui_roi_ranges.py
--rw-r--r--   0        0        0     5795 2023-05-02 11:32:56.717662 pyminflux-0.1.3/pyminflux/ui/ui_time_inspector.py
--rw-r--r--   0        0        0    12104 2023-05-26 08:45:53.145825 pyminflux-0.1.3/pyminflux/ui/ui_wizard.py
--rw-r--r--   0        0        0    12794 2023-05-26 08:45:53.145825 pyminflux-0.1.3/pyminflux/ui/wizard.py
--rw-r--r--   0        0        0     9205 2023-05-26 08:45:53.145825 pyminflux-0.1.3/pyminflux/ui/wizard.ui
--rw-r--r--   0        0        0      677 2023-05-02 11:32:56.717662 pyminflux-0.1.3/pyminflux/utils/__init__.py
--rw-r--r--   0        0        0     2614 2023-05-02 11:32:56.717662 pyminflux-0.1.3/pyminflux/utils/_utils.py
--rw-r--r--   0        0        0      644 2023-05-02 11:32:56.717662 pyminflux-0.1.3/pyminflux/writer/__init__.py
--rw-r--r--   0        0        0     1740 2023-05-08 08:01:47.198555 pyminflux-0.1.3/pyminflux/writer/_writer.py
--rw-r--r--   0        0        0     1880 2023-05-26 08:45:53.145825 pyminflux-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     4375 1970-01-01 00:00:00.000000 pyminflux-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-05-02 11:32:56.697662 pyminflux-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     3445 2023-07-18 15:01:43.368014 pyminflux-0.2.0/README.md
+-rw-r--r--   0        0        0     1471 2023-07-18 15:01:43.596015 pyminflux-0.2.0/pyminflux/__init__.py
+-rw-r--r--   0        0        0     1120 2023-07-18 15:01:43.600015 pyminflux-0.2.0/pyminflux/analysis/__init__.py
+-rw-r--r--   0        0        0    16121 2023-07-18 15:01:43.600015 pyminflux-0.2.0/pyminflux/analysis/_analysis.py
+-rw-r--r--   0        0        0      638 2023-05-02 11:32:56.701662 pyminflux-0.2.0/pyminflux/base/__init__.py
+-rw-r--r--   0        0        0      918 2023-05-02 11:32:56.701662 pyminflux-0.2.0/pyminflux/base/_base.py
+-rw-r--r--   0        0        0      837 2023-07-18 15:01:43.600015 pyminflux-0.2.0/pyminflux/correct/__init__.py
+-rw-r--r--   0        0        0    14374 2023-07-18 15:01:43.600015 pyminflux-0.2.0/pyminflux/correct/_correct.py
+-rw-r--r--   0        0        0      935 2023-07-18 15:01:43.600015 pyminflux-0.2.0/pyminflux/fourier/__init__.py
+-rw-r--r--   0        0        0    12885 2023-07-18 15:01:43.600015 pyminflux-0.2.0/pyminflux/fourier/_fourier.py
+-rw-r--r--   0        0        0     1081 2023-05-03 07:24:53.358703 pyminflux-0.2.0/pyminflux/main.py
+-rw-r--r--   0        0        0      728 2023-07-18 15:01:43.600015 pyminflux-0.2.0/pyminflux/processor/__init__.py
+-rw-r--r--   0        0        0    31883 2023-07-18 15:01:43.600015 pyminflux-0.2.0/pyminflux/processor/_processor.py
+-rw-r--r--   0        0        0      716 2023-07-18 15:01:43.600015 pyminflux-0.2.0/pyminflux/reader/__init__.py
+-rw-r--r--   0        0        0    20766 2023-07-18 15:01:43.600015 pyminflux-0.2.0/pyminflux/reader/_reader.py
+-rw-r--r--   0        0        0      733 2023-07-18 15:01:43.600015 pyminflux-0.2.0/pyminflux/render/__init__.py
+-rw-r--r--   0        0        0    12315 2023-07-18 15:01:43.600015 pyminflux-0.2.0/pyminflux/render/_render.py
+-rw-r--r--   0        0        0   139482 2023-05-02 11:32:56.705662 pyminflux-0.2.0/pyminflux/resources.py
+-rw-r--r--   0        0        0      747 2023-05-02 11:32:56.705662 pyminflux-0.2.0/pyminflux/resources.qrc
+-rw-r--r--   0        0        0      641 2023-05-02 11:32:56.705662 pyminflux-0.2.0/pyminflux/settings/__init__.py
+-rw-r--r--   0        0        0     1584 2023-07-18 15:01:43.600015 pyminflux-0.2.0/pyminflux/settings/_settings.py
+-rw-r--r--   0        0        0      725 2023-07-18 15:01:43.600015 pyminflux-0.2.0/pyminflux/state/__init__.py
+-rw-r--r--   0        0        0     6756 2023-07-18 15:01:43.600015 pyminflux-0.2.0/pyminflux/state/_state.py
+-rw-r--r--   0        0        0      633 2023-05-02 11:32:56.705662 pyminflux-0.2.0/pyminflux/threads/__init__.py
+-rw-r--r--   0        0        0      875 2023-05-02 11:32:56.705662 pyminflux-0.2.0/pyminflux/threads/_threads.py
+-rw-r--r--   0        0        0      608 2023-06-05 15:31:01.458161 pyminflux-0.2.0/pyminflux/ui/__init__.py
+-rw-r--r--   0        0        0    31065 2023-07-18 15:01:43.600015 pyminflux-0.2.0/pyminflux/ui/analyzer.py
+-rw-r--r--   0        0        0     9033 2023-05-26 08:45:53.137825 pyminflux-0.2.0/pyminflux/ui/analyzer.ui
+-rw-r--r--   0        0        0   216854 2023-05-02 11:32:56.857662 pyminflux-0.2.0/pyminflux/ui/assets/Logo_v3.icns
+-rw-r--r--   0        0        0  1143198 2023-05-02 11:32:56.861662 pyminflux-0.2.0/pyminflux/ui/assets/Logo_v3.ico
+-rwxr-xr-x   0        0        0    43531 2023-05-02 11:32:56.861662 pyminflux-0.2.0/pyminflux/ui/assets/Logo_v3.png
+-rw-r--r--   0        0        0     8998 2023-05-03 14:33:18.090905 pyminflux-0.2.0/pyminflux/ui/assets/Logo_v3_small.png
+-rwxr-xr-x   0        0        0      670 2023-05-02 11:32:56.709662 pyminflux-0.2.0/pyminflux/ui/assets/create_resources.sh
+-rwxr-xr-x   0        0        0     1805 2023-05-02 11:32:56.709662 pyminflux-0.2.0/pyminflux/ui/assets/png_to_icns.sh
+-rw-r--r--   0        0        0    11219 2023-07-18 15:01:43.600015 pyminflux-0.2.0/pyminflux/ui/color_unmixer.py
+-rw-r--r--   0        0        0     8732 2023-05-26 08:45:53.137825 pyminflux-0.2.0/pyminflux/ui/color_unmixer.ui
+-rw-r--r--   0        0        0     2561 2023-05-02 11:57:29.698894 pyminflux-0.2.0/pyminflux/ui/dataviewer.py
+-rw-r--r--   0        0        0     1008 2023-05-02 11:32:56.713662 pyminflux-0.2.0/pyminflux/ui/emittingstream.py
+-rw-r--r--   0        0        0    16821 2023-07-18 15:01:43.600015 pyminflux-0.2.0/pyminflux/ui/frc_tool.py
+-rw-r--r--   0        0        0     5267 2023-07-18 15:01:43.600015 pyminflux-0.2.0/pyminflux/ui/frc_tool.ui
+-rw-r--r--   0        0        0      670 2023-05-26 08:45:53.137825 pyminflux-0.2.0/pyminflux/ui/helpers/__init__.py
+-rw-r--r--   0        0        0     2994 2023-05-26 08:45:53.137825 pyminflux-0.2.0/pyminflux/ui/helpers/_helpers.py
+-rwxr-xr-x   0        0        0    43531 2023-05-02 11:32:56.861662 pyminflux-0.2.0/pyminflux/ui/icons/icon.png
+-rw-r--r--   0        0        0    36456 2023-07-18 15:01:43.600015 pyminflux-0.2.0/pyminflux/ui/main_window.py
+-rw-r--r--   0        0        0     5601 2023-07-18 15:01:43.600015 pyminflux-0.2.0/pyminflux/ui/main_window.ui
+-rw-r--r--   0        0        0    18839 2023-05-26 08:45:53.141826 pyminflux-0.2.0/pyminflux/ui/options.py
+-rw-r--r--   0        0        0    18392 2023-05-26 08:45:53.141826 pyminflux-0.2.0/pyminflux/ui/options.ui
+-rw-r--r--   0        0        0     2057 2023-05-02 11:32:56.713662 pyminflux-0.2.0/pyminflux/ui/pandas_datamodel.py
+-rw-r--r--   0        0        0    14049 2023-07-18 15:01:43.600015 pyminflux-0.2.0/pyminflux/ui/plotter.py
+-rw-r--r--   0        0        0     3473 2023-05-12 11:10:11.402890 pyminflux-0.2.0/pyminflux/ui/plotter_3d.py
+-rw-r--r--   0        0        0      544 2023-05-02 11:32:56.713662 pyminflux-0.2.0/pyminflux/ui/plotter_3d.ui
+-rw-r--r--   0        0        0     4775 2023-05-02 11:32:56.713662 pyminflux-0.2.0/pyminflux/ui/plotter_toolbar.py
+-rw-r--r--   0        0        0     3254 2023-05-02 11:32:56.713662 pyminflux-0.2.0/pyminflux/ui/plotter_toolbar.ui
+-rw-r--r--   0        0        0     4125 2023-05-02 11:32:56.713662 pyminflux-0.2.0/pyminflux/ui/roi_ranges.py
+-rw-r--r--   0        0        0     4422 2023-04-26 08:29:10.942459 pyminflux-0.2.0/pyminflux/ui/roi_ranges.ui
+-rw-r--r--   0        0        0    18384 2023-07-18 15:01:43.604015 pyminflux-0.2.0/pyminflux/ui/time_inspector.py
+-rw-r--r--   0        0        0     3128 2023-04-26 08:29:10.942459 pyminflux-0.2.0/pyminflux/ui/time_inspector.ui
+-rw-r--r--   0        0        0    10646 2023-05-26 08:45:53.141826 pyminflux-0.2.0/pyminflux/ui/ui_analyzer.py
+-rw-r--r--   0        0        0     9840 2023-05-26 08:45:53.141826 pyminflux-0.2.0/pyminflux/ui/ui_color_unmixer.py
+-rw-r--r--   0        0        0     6478 2023-07-18 15:01:43.604015 pyminflux-0.2.0/pyminflux/ui/ui_frc_tool.py
+-rw-r--r--   0        0        0     9880 2023-07-18 15:01:43.604015 pyminflux-0.2.0/pyminflux/ui/ui_main_window.py
+-rw-r--r--   0        0        0    22391 2023-05-26 08:45:53.145825 pyminflux-0.2.0/pyminflux/ui/ui_options.py
+-rw-r--r--   0        0        0     2276 2023-05-02 11:32:56.717662 pyminflux-0.2.0/pyminflux/ui/ui_plotter_3d.py
+-rw-r--r--   0        0        0     5670 2023-05-02 11:32:56.717662 pyminflux-0.2.0/pyminflux/ui/ui_plotter_toolbar.py
+-rw-r--r--   0        0        0     5773 2023-05-02 11:32:56.717662 pyminflux-0.2.0/pyminflux/ui/ui_roi_ranges.py
+-rw-r--r--   0        0        0     5795 2023-05-02 11:32:56.717662 pyminflux-0.2.0/pyminflux/ui/ui_time_inspector.py
+-rw-r--r--   0        0        0    12104 2023-05-26 08:45:53.145825 pyminflux-0.2.0/pyminflux/ui/ui_wizard.py
+-rw-r--r--   0        0        0    18719 2023-07-19 12:11:45.811283 pyminflux-0.2.0/pyminflux/ui/wizard.py
+-rw-r--r--   0        0        0     9205 2023-05-26 08:45:53.145825 pyminflux-0.2.0/pyminflux/ui/wizard.ui
+-rw-r--r--   0        0        0      647 2023-07-18 15:01:43.604015 pyminflux-0.2.0/pyminflux/utils/__init__.py
+-rw-r--r--   0        0        0     2498 2023-07-18 15:01:43.604015 pyminflux-0.2.0/pyminflux/utils/_utils.py
+-rw-r--r--   0        0        0      726 2023-07-18 15:01:43.604015 pyminflux-0.2.0/pyminflux/writer/__init__.py
+-rw-r--r--   0        0        0     1820 2023-07-18 15:01:43.604015 pyminflux-0.2.0/pyminflux/writer/_writer.py
+-rw-r--r--   0        0        0     1931 2023-07-18 15:01:43.604015 pyminflux-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4956 1970-01-01 00:00:00.000000 pyminflux-0.2.0/PKG-INFO
```

### Comparing `pyminflux-0.1.3/LICENSE.txt` & `pyminflux-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.3/README.md` & `pyminflux-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # ![](pyminflux/ui/assets/Logo_v3_small.png)&nbsp;&nbsp;&nbsp;pyMINFLUX
 
 Reader, analyzer, and viewer of MINFLUX raw data.
 
 <p align="center">
-  <img width="460" src="https://pyminflux.ethz.ch/img/pyminflux.png">
+  <img width="800" src="https://pyminflux.ethz.ch/img/pyminflux.png">
 </p>
 
 ## Installation
 
 ### Apps
 
 Compiled executables (apps) for Linux, macOS and Windows can be downloaded from the [release page](https://github.com/bsse-scf/pyMINFLUX/releases/latest). 
@@ -53,21 +53,26 @@
 $ conda activate pyminflux-env
 $ git clone https://github.com/bsse-scf/pyMINFLUX /path/to/pyminflux
 $ cd /path/to/pyminflux
 $ conda install pyopengl       # This is specific to macOS
 $ python -m pip install -e .
 ```
 
-### Running pyMinFlux from console
+### Running pyMINFLUX from console
 
 ```sh
 $ cd /path/to/pyminflux
-$ python pyminflux/main.py
+$ python pyminflux/main.py  # As a Python script, or
+$ pyminflux                 # as a standalone tool
 ```
 
+### Using the pyMINFLUX API from Python scripts or Jupyter Notebooks
+
+The graphical user interface is not the only way to use pyMINFLUX. Indeed, the pyMINFLUX core library can be integrated in Python scripts or Jupyter Notebooks. The documentation for the pyMIMFLUX core API can be found on [https://pyminflux.ethz.ch/api/pyminflux/](https://pyminflux.ethz.ch/api/pyminflux/); an example Jupyter Notebook is [bundled with the code](/examples/processing.ipynb).
+
 ## User manual
 
 The user manual is hosted in the [project wiki](https://github.com/bsse-scf/pyMINFLUX/wiki/pyMINFLUX-user-manual).
 
 ## Official website
 
 The official pyMINFLUX website is on https://pyminflux.ethz.ch.
```

### Comparing `pyminflux-0.1.3/pyminflux/__init__.py` & `pyminflux-0.2.0/pyminflux/utils/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,14 +9,8 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 
-import pyqtgraph as pg
-
-__APP_NAME__ = "pyMINFLUX"
-__version__ = "0.1.3"
-
-# PyQtGraph settings
-pg.setConfigOption("imageAxisOrder", "row-major")  # For best performance
+from ._utils import check_for_updates
```

### Comparing `pyminflux-0.1.3/pyminflux/analysis/__init__.py` & `pyminflux-0.2.0/pyminflux/settings/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,16 +9,8 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 
-from ._analysis import (
-    calculate_2d_histogram,
-    calculate_density_map,
-    find_cutoff_near_value,
-    find_first_peak_bounds,
-    get_robust_threshold,
-    ideal_hist_bins,
-    prepare_histogram,
-)
+from ._settings import Settings
```

### Comparing `pyminflux-0.1.3/pyminflux/analysis/_analysis.py` & `pyminflux-0.2.0/pyminflux/analysis/_analysis.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import math
 from typing import Optional
 
 import numpy as np
 from scipy import stats
 from scipy.ndimage import median_filter
 from scipy.signal import find_peaks
+from sklearn.mixture import BayesianGaussianMixture
 
 
 def hist_bins(values: np.ndarray, bin_size: float) -> tuple:
     """Return the bins to be used for the passed values and bin size.
 
     Parameters
     ----------
@@ -141,15 +142,15 @@
 
     return bin_edges, bin_centers, bin_size
 
 
 def get_robust_threshold(values: np.ndarray, factor: float = 2.0):
     """Calculate a robust threshold for the array of values.
 
-    The threshold is defines as median + thresh * median absolute deviation.
+    The threshold is defines as `median + thresh * median absolute deviation`.
 
     The median absolute deviation is divided by 0.67449 to bring it in the
     same scale as the (non-robust) standard deviation.
 
     Parameters
     ----------
 
@@ -507,7 +508,68 @@
         )
 
     # Create 2D histogram
     histogram = np.histogram2d(y, x, bins=(y_bin_edges, x_bin_edges))
 
     # Return histogram
     return histogram[0]
+
+
+def assign_data_to_clusters(
+    x: np.ndarray, num_clusters: int = 2, seed: Optional[int] = None
+):
+    """Use Gaussian Mixture Model fitting to assign data to the requested number of clusters.
+
+    Parameters
+    ----------
+
+    x: np.ndarray
+        Array of values to cluster.
+
+    num_clusters: int (Default = 2)
+        Number of clusters to be assigned.
+
+    seed: int (Optional)
+        Seed for the random number generator.
+
+    Returns
+    -------
+
+    ids: np.ndarray
+        Array of cluster ids for each value in x. The first cluster has ID 1.
+    """
+
+    # Make sure to work with a NumPy array
+    x = np.array(x)
+
+    # Make sure to work with a column vector
+    x = x.reshape(-1, 1)
+
+    # Fit a Bayesian Gaussian Mixture Model with self.state.num_fluorophores components
+    model = BayesianGaussianMixture(
+        n_components=num_clusters,
+        init_params="k-means++",
+        covariance_type="full",
+        max_iter=1000,
+        random_state=seed,
+    ).fit(x)
+
+    # Predict with the selected model
+    y_pred = model.predict(x)
+
+    # If num_clusters is > 1, sort the indices by mean values of x,
+    # from low to high (to match the assignment of the manual thresholding)
+    if num_clusters > 1:
+        means = [np.mean(x[y_pred == f_id]) for f_id in np.unique(y_pred)]
+        sorted_f = np.argsort(means)
+        for f in range(num_clusters):
+            if np.isnan(means[f]):
+                continue
+            n = sorted_f[f] + num_clusters
+            y_pred[y_pred == f] = n
+        y_pred -= num_clusters
+
+    # Now make the clusters ID start from 1 instead of 0.
+    ids = y_pred + 1
+
+    # Return
+    return ids
```

### Comparing `pyminflux-0.1.3/pyminflux/base/__init__.py` & `pyminflux-0.2.0/pyminflux/base/__init__.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.3/pyminflux/base/_base.py` & `pyminflux-0.2.0/pyminflux/base/_base.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.3/pyminflux/main.py` & `pyminflux-0.2.0/pyminflux/main.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.3/pyminflux/processor/__init__.py` & `pyminflux-0.2.0/pyminflux/state/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,8 +9,11 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 
-from ._processor import MinFluxProcessor
+__doc__ = "State machine with all settings."
+__all__ = ["ColorCode", "State"]
+
+from ._state import ColorCode, State
```

### Comparing `pyminflux-0.1.3/pyminflux/processor/_processor.py` & `pyminflux-0.2.0/pyminflux/processor/_processor.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,107 +9,126 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 
-from typing import Union
+from typing import Optional, Union
 
 import numpy as np
 import pandas as pd
 from scipy.stats import mode
 
 from pyminflux.reader import MinFluxReader
-from pyminflux.state import State
 
 
 class MinFluxProcessor:
     """Processor of MINFLUX data."""
 
+    __doc__ = """Allows for filtering and selecting data read by the underlying `MinFluxReader`. Please notice that
+     `MinFluxProcessor` makes use of `State.min_num_loc_per_trace` to make sure that at load and after every
+      filtering step, short traces are dropped."""
+
     __slots__ = [
         "state",
-        "__minfluxreader",
-        "__current_fluorophore_id",
-        "__filtered_stats_dataframe",
-        "__fluorophore_ids",
-        "__selected_rows_dict",
-        "__stats_to_be_recomputed",
-        "__weighted_localizations",
-        "__weighted_localizations_to_be_recomputed",
-        "__use_weighted_localizations",
+        "_reader",
+        "_current_fluorophore_id",
+        "_filtered_stats_dataframe",
+        "_min_trace_length",
+        "_selected_rows_dict",
+        "_stats_to_be_recomputed",
+        "_weighted_localizations",
+        "_weighted_localizations_to_be_recomputed",
+        "_use_weighted_localizations",
     ]
 
-    def __init__(self, minfluxreader: MinFluxReader):
+    def __init__(self, reader: MinFluxReader, min_trace_length: int = 1):
         """Constructor.
 
         Parameters
         ----------
 
-        minfluxreader: pyminflux.reader.MinFluxReader
+        reader: MinFluxReader
             MinFluxReader object.
+
+        min_trace_length: int (Default = 1)
+            Minimum number of localizations for a trace to be kept. Shorter traces are dropped.
         """
 
         # Store a reference to the MinFluxReader
-        self.__minfluxreader = minfluxreader
+        self._reader: MinFluxReader = reader
 
-        # Keep a reference to the state machine
-        self.state = State()
+        # Global options
+        self._min_trace_length: int = min_trace_length
 
         # Cache the filtered stats dataframe
-        self.__filtered_stats_dataframe = None
+        self._filtered_stats_dataframe = None
 
         # Keep separate arrays of booleans to cache selection state for all fluorophores IDs.
-        self.__selected_rows_dict = None
-        self.__init_selected_rows_dict()
+        self._selected_rows_dict = None
+        self._init_selected_rows_dict()
 
         # Keep track of the selected fluorophore
         # 0 - All (default)
         # 1 - Fluorophore 1
         # 2 - Fluorophore 2
-        self.__current_fluorophore_id = 0
+        self._current_fluorophore_id = 0
 
         # Cache the weighted, averaged TID positions
-        self.__weighted_localizations = None
+        self._weighted_localizations = None
 
         # Keep track whether the statistics and the weighted localizations need to be recomputed
-        self.__stats_to_be_recomputed = False
-        self.__weighted_localizations_to_be_recomputed = False
+        self._stats_to_be_recomputed = False
+        self._weighted_localizations_to_be_recomputed = False
 
         # Whether to use weighted average for localizations
-        self.__use_weighted_localizations = False
+        self._use_weighted_localizations = False
 
         # Apply the global filters
         self._apply_global_filters()
 
-    def __init_selected_rows_dict(self):
+    def _init_selected_rows_dict(self):
         """Initialize the selected rows array."""
         # How many fluorophores do we have?
-        self.__selected_rows_dict = {
+        self._selected_rows_dict = {
             1: pd.Series(
                 data=np.ones(len(self.full_dataframe.index), dtype=bool),
                 index=self.full_dataframe.index,
             ),
             2: pd.Series(
                 data=np.ones(len(self.full_dataframe.index), dtype=bool),
                 index=self.full_dataframe.index,
             ),
         }
 
     @property
+    def min_num_loc_per_trace(self):
+        """Minimum number of localizations for the trace to be kept."""
+        return self._min_trace_length
+
+    @min_num_loc_per_trace.setter
+    def min_num_loc_per_trace(self, value):
+        if value < 1 or int(value) != value:
+            raise ValueError(
+                "MinFluxProcessor.min_num_loc_per_trace must be a positive integer!"
+            )
+        self._min_trace_length = value
+
+    @property
     def is_3d(self) -> bool:
         """Return True if the acquisition is 3D.
 
         Returns
         -------
 
         is_3d: bool
             True if the acquisition is 3D, False otherwise.
         """
-        return self.__minfluxreader.is_3d
+        return self._reader.is_3d
 
     @property
     def num_values(self) -> int:
         """Return the number of values in the (filtered) dataframe.
 
         Returns
         -------
@@ -121,52 +140,52 @@
             return len(self.filtered_dataframe.index)
 
         return 0
 
     @property
     def current_fluorophore_id(self) -> int:
         """Return current fluorophore ID (0 for all)."""
-        return self.__current_fluorophore_id
+        return self._current_fluorophore_id
 
     @current_fluorophore_id.setter
     def current_fluorophore_id(self, fluorophore_id: int) -> None:
         """Set current fluorophore ID (0 for all)."""
 
         if fluorophore_id not in [0, 1, 2]:
             raise ValueError(f"Only 1 or 2 are valid fluorophore IDs.")
 
         # Set the new fluorophore_id
-        self.__current_fluorophore_id = fluorophore_id
+        self._current_fluorophore_id = fluorophore_id
 
         # Apply the global filters
         self._apply_global_filters()
 
         # Flag stats to be recomputed
-        self.__stats_to_be_recomputed = True
+        self._stats_to_be_recomputed = True
 
     @property
     def num_fluorophorses(self) -> int:
         """Return the number of fluorophores."""
         return len(np.unique(self.full_dataframe["fluo"].values))
 
     @property
     def filtered_numpy_array_all(self):
         """Return the raw NumPy array with applied filters (for all fluorphores)."""
 
         # Copy the raw NumPy array
-        raw_array = self.__minfluxreader.valid_raw_data
+        raw_array = self._reader.valid_raw_data
         if raw_array is None:
             return None
 
         # Append the fluorophore ID data
         raw_array["fluo"] = self.full_dataframe["fluo"].astype(np.uint8)
 
         # Extract combination of fluorophore 1 and 2 filtered dataframes
-        mask_1 = (self.full_dataframe["fluo"] == 1) & self.__selected_rows_dict[1]
-        mask_2 = (self.full_dataframe["fluo"] == 2) & self.__selected_rows_dict[2]
+        mask_1 = (self.full_dataframe["fluo"] == 1) & self._selected_rows_dict[1]
+        mask_2 = (self.full_dataframe["fluo"] == 2) & self._selected_rows_dict[2]
         return raw_array[mask_1 | mask_2]
 
     @property
     def filtered_numpy_array(self):
         """Return the raw NumPy array wit applied filters for the selected fluorophores."""
 
         # Copy the raw NumPy array
@@ -191,31 +210,31 @@
 
         Returns
         -------
 
         full_dataframe: Union[None, pd.DataFrame]
             A Pandas dataframe or None if no file was loaded.
         """
-        return self.__minfluxreader.processed_dataframe
+        return self._reader.processed_dataframe
 
     def _filtered_dataframe_all(self) -> Union[None, pd.DataFrame]:
         """Return joint dataframe for all fluorophores and with all filters applied.
 
         Returns
         -------
 
         filtered_dataframe_all: Union[None, pd.DataFrame]
             A Pandas dataframe or None if no file was loaded.
         """
         if self.full_dataframe is None:
             return None
 
         # Extract combination of fluorophore 1 and 2 filtered dataframes
-        mask_1 = (self.full_dataframe["fluo"] == 1) & self.__selected_rows_dict[1]
-        mask_2 = (self.full_dataframe["fluo"] == 2) & self.__selected_rows_dict[2]
+        mask_1 = (self.full_dataframe["fluo"] == 1) & self._selected_rows_dict[1]
+        mask_2 = (self.full_dataframe["fluo"] == 2) & self._selected_rows_dict[2]
         return self.full_dataframe.loc[mask_1 | mask_2]
 
     @property
     def filtered_dataframe(self) -> Union[None, pd.DataFrame]:
         """Return dataframe with all filters applied.
 
         Returns
@@ -228,77 +247,154 @@
             return None
         if self.current_fluorophore_id == 0:
             return self._filtered_dataframe_all()
         else:
             df = self.full_dataframe.loc[
                 self.full_dataframe["fluo"] == self.current_fluorophore_id
             ]
-            return df.loc[self.__selected_rows_dict[self.current_fluorophore_id]]
+            return df.loc[self._selected_rows_dict[self.current_fluorophore_id]]
 
     @property
     def filtered_dataframe_stats(self) -> Union[None, pd.DataFrame]:
         """Return dataframe stats with all filters applied.
 
         Returns
         -------
 
         filtered_dataframe_stats: Union[None, pd.DataFrame]
             A Pandas dataframe with all data statistics or None if no file was loaded.
         """
-        if self.__stats_to_be_recomputed:
+        if self._stats_to_be_recomputed:
             self._calculate_statistics()
-        return self.__filtered_stats_dataframe
+        return self._filtered_stats_dataframe
 
     @property
     def weighted_localizations(self) -> Union[None, pd.DataFrame]:
         """Return the average (x, y, z) position per TID weighted by the relative photon count."""
-        if self.__weighted_localizations_to_be_recomputed:
+        if self._weighted_localizations_to_be_recomputed:
             self._calculate_weighted_positions()
-        return self.__weighted_localizations
+        return self._weighted_localizations
 
     @property
     def use_weighted_localizations(self) -> bool:
         """Whether to use weighted average to calculate the mean localization per TID."""
-        return self.__use_weighted_localizations
+        return self._use_weighted_localizations
 
     @use_weighted_localizations.setter
     def use_weighted_localizations(self, value: bool):
         """Whether to use weighted average to calculate the mean localization per TID."""
-        self.__use_weighted_localizations = value
-        self.__weighted_localizations_to_be_recomputed = True
+        self._use_weighted_localizations = value
+        self._weighted_localizations_to_be_recomputed = True
 
     @classmethod
     def processed_properties(cls):
         """Return the processed dataframe columns."""
         return MinFluxReader.processed_properties()
 
     def reset(self):
         """Drops all dynamic filters and resets the data to the processed data frame with global filters."""
 
         # Clear the selection per fluorophore; they will be reinitialized as
         # all selected at the first access.
-        self.__init_selected_rows_dict()
+        self._init_selected_rows_dict()
 
         # Reset the mapping to the corresponding fluorophore
         self.full_dataframe["fluo"] = 1
 
         # Default fluorophore is 0 (no selection)
         self.current_fluorophore_id = 0
 
         # Apply global filters
         self._apply_global_filters()
 
+    def update_localizations(
+        self, x: np.ndarray, y: np.ndarray, z: Optional[np.ndarray] = None
+    ):
+        """Updates the localization coordinates of current filtered dataframe.
+
+        This can be used for instance after a drift correction.
+
+        Parameters
+        ----------
+
+        x: np.ndarray
+            Array of x coordinates.
+
+        y: np.ndarray
+            Array of y coordinates.
+
+        z: np.ndarray (Optional)
+            Optional array of z coordinates. Omit it to skip.
+            If the acquisition is 2D, it will be ignored in any case.
+        """
+
+        if self.full_dataframe is None:
+            return
+
+        # Make sure to work with NumPy arrays
+        x = np.array(x)
+        y = np.array(y)
+        if z is not None and self.is_3d:
+            z = np.array(z)
+
+        # Select the correct rows to update
+        if self.current_fluorophore_id == 0:
+            mask_1 = (self.full_dataframe["fluo"] == 1) & self._selected_rows_dict[1]
+            mask_2 = (self.full_dataframe["fluo"] == 2) & self._selected_rows_dict[2]
+            mask = mask_1 | mask_2
+        elif self.current_fluorophore_id == 1:
+            mask = (self.full_dataframe["fluo"] == 1) & self._selected_rows_dict[1]
+        else:
+            mask = (self.full_dataframe["fluo"] == 2) & self._selected_rows_dict[2]
+
+        # Make sure that the lengths match
+        assert np.sum(mask.values) == len(x), "Unexpected number of elements in x."
+        assert np.sum(mask.values) == len(y), "Unexpected number of elements in y."
+        if z is not None and self.is_3d:
+            assert np.sum(mask.values) == len(z), "Unexpected number of elements in z."
+
+        # Re-assign the data at the reader level
+        self._reader._data_df.loc[mask, "x"] = x
+        self._reader._data_df.loc[mask, "y"] = y
+        if z is not None and self.is_3d:
+            self._reader._data_df.loc[mask, "z"] = z
+
+        # Also update the raw structured NumPy array. Since NumPy
+        # will return a copy if we try to access the "loc" array
+        # directly using logical arrays, we need to iterate over
+        # all rows one by one!
+        #
+        # Furthermore, we need to scale the values by the factor
+        # self._reader._unit_scaling_factor
+        x_scaled = x / self._reader._unit_scaling_factor
+        y_scaled = y / self._reader._unit_scaling_factor
+        if z is not None and self.is_3d:
+            z_scaled = z / self._reader._unit_scaling_factor
+        idx = self._reader._loc_index
+        vld_indices = np.where(self._reader._valid_entries)[0]
+        mask_indices = np.where(mask)[0]
+        for i, I in enumerate(mask_indices):
+            if I in vld_indices:
+                self._reader._data_array[I]["itr"][idx]["loc"][0] = x_scaled[i]
+                self._reader._data_array[I]["itr"][idx]["loc"][1] = y_scaled[i]
+                if z is not None and self.is_3d:
+                    self._reader._data_array[I]["itr"][idx]["loc"][2] = z_scaled[i]
+
+        # Mark derived data to be recomputed
+        self._stats_to_be_recomputed = True
+        self._weighted_localizations_to_be_recomputed = True
+
     def set_fluorophore_ids(self, fluorophore_ids: np.ndarray[int]):
         """Assign the fluorophore IDs."""
         if len(fluorophore_ids) != len(self.full_dataframe.index):
             raise ValueError(
                 "The number of fluorophore IDs does not match the number of entries in the dataframe."
             )
         self.full_dataframe["fluo"] = fluorophore_ids
-        self.__init_selected_rows_dict()
+        self._init_selected_rows_dict()
         self._apply_global_filters()
 
     def select_by_indices(
         self, indices, from_weighted_locs: bool = False
     ) -> Union[None, pd.DataFrame]:
         """Return view on a subset of the filtered dataset or the weighted localisations defined by the passed indices.
 
@@ -316,17 +412,17 @@
         Returns
         -------
 
         subset: Union[None, pd.DataFrame]
             A view on a subset of the dataframe defined by the passed indices, or None if no file was loaded.
         """
         if from_weighted_locs:
-            if self.__weighted_localizations is None:
+            if self._weighted_localizations is None:
                 return None
-            return self.__weighted_localizations.iloc[indices]
+            return self._weighted_localizations.iloc[indices]
         else:
             if self.filtered_dataframe is None:
                 return None
             return self.filtered_dataframe.iloc[indices]
 
     def select_by_1d_range(
         self, x_prop, x_range, from_weighted_locs: bool = False
@@ -358,17 +454,17 @@
         # Make sure that the range is increasing
         x_min = x_range[0]
         x_max = x_range[1]
         if x_max < x_min:
             x_max, x_min = x_min, x_max
 
         if from_weighted_locs:
-            return self.__weighted_localizations.loc[
-                (self.__weighted_localizations[x_prop] >= x_min)
-                & (self.__weighted_localizations[x_prop] < x_max)
+            return self._weighted_localizations.loc[
+                (self._weighted_localizations[x_prop] >= x_min)
+                & (self._weighted_localizations[x_prop] < x_max)
             ]
         else:
             # Work with currently selected rows
             df = self.filtered_dataframe
 
             return df.loc[(df[x_prop] >= x_min) & (df[x_prop] < x_max)]
 
@@ -414,19 +510,19 @@
 
         y_min = y_range[0]
         y_max = y_range[1]
         if y_max < y_min:
             y_max, y_min = y_min, y_max
 
         if from_weighted_locs:
-            return self.__weighted_localizations.loc[
-                (self.__weighted_localizations[x_prop] >= x_min)
-                & (self.__weighted_localizations[x_prop] < x_max)
-                & (self.__weighted_localizations[y_prop] >= y_min)
-                & (self.__weighted_localizations[y_prop] < y_max)
+            return self._weighted_localizations.loc[
+                (self._weighted_localizations[x_prop] >= x_min)
+                & (self._weighted_localizations[x_prop] < x_max)
+                & (self._weighted_localizations[y_prop] >= y_min)
+                & (self._weighted_localizations[y_prop] < y_max)
             ]
         else:
             # Work with currently selected rows
             df = self.filtered_dataframe
 
             return df.loc[
                 (df[x_prop] >= x_min)
@@ -462,92 +558,92 @@
 
         y_min = y_range[0]
         y_max = y_range[1]
         if y_max < y_min:
             y_max, y_min = y_min, y_max
 
         if self.current_fluorophore_id == 0 or self.current_fluorophore_id == 1:
-            self.__selected_rows_dict[1] = (
-                self.__selected_rows_dict[1]
+            self._selected_rows_dict[1] = (
+                self._selected_rows_dict[1]
                 & (self.filtered_dataframe[x_prop] >= x_min)
                 & (self.filtered_dataframe[x_prop] < x_max)
                 & (self.filtered_dataframe[y_prop] >= y_min)
                 & (self.filtered_dataframe[y_prop] < y_max)
             )
 
         if self.current_fluorophore_id == 0 or self.current_fluorophore_id == 2:
-            self.__selected_rows_dict[2] = (
-                self.__selected_rows_dict[2]
+            self._selected_rows_dict[2] = (
+                self._selected_rows_dict[2]
                 & (self.filtered_dataframe[x_prop] >= x_min)
                 & (self.filtered_dataframe[x_prop] < x_max)
                 & (self.filtered_dataframe[y_prop] >= y_min)
                 & (self.filtered_dataframe[y_prop] < y_max)
             )
 
         # Make sure to always apply the global filters
         self._apply_global_filters()
 
         # Make sure to flag the derived data to be recomputed
-        self.__stats_to_be_recomputed = True
-        self.__weighted_localizations_to_be_recomputed = True
+        self._stats_to_be_recomputed = True
+        self._weighted_localizations_to_be_recomputed = True
 
     def _apply_global_filters(self):
         """Apply filters that are defined in the global application configuration."""
 
         if self.current_fluorophore_id == 0 or self.current_fluorophore_id == 1:
-            self.__selected_rows_dict[1] = self.__filter_by_tid_length(1)
+            self._selected_rows_dict[1] = self._filter_by_tid_length(1)
 
         if self.current_fluorophore_id == 0 or self.current_fluorophore_id == 2:
-            self.__selected_rows_dict[2] = self.__filter_by_tid_length(2)
+            self._selected_rows_dict[2] = self._filter_by_tid_length(2)
 
         # Make sure to flag the derived data to be recomputed
-        self.__stats_to_be_recomputed = True
-        self.__weighted_localizations_to_be_recomputed = True
+        self._stats_to_be_recomputed = True
+        self._weighted_localizations_to_be_recomputed = True
 
-    def __filter_by_tid_length(self, index):
+    def _filter_by_tid_length(self, index):
         # Make sure to count only currently selected rows
         df = self.full_dataframe.copy()
-        df.loc[np.invert(self.__selected_rows_dict[index]), "tid"] = np.nan
+        df.loc[np.invert(self._selected_rows_dict[index]), "tid"] = np.nan
 
         # Select all rows where the count of TIDs is larger than self._min_trace_num
         counts = df["tid"].value_counts(normalize=False)
-        return df["tid"].isin(counts[counts >= self.state.min_num_loc_per_trace].index)
+        return df["tid"].isin(counts[counts >= self.min_num_loc_per_trace].index)
 
     def filter_by_single_threshold(
         self, prop: str, threshold: Union[int, float], larger_than: bool = True
     ):
         """Apply single threshold to filter values either lower or higher (equal) than threshold for given property."""
 
         # Apply filter
         if self.current_fluorophore_id == 0 or self.current_fluorophore_id == 1:
             if larger_than:
-                self.__selected_rows_dict[1] = self.__selected_rows_dict[1] & (
+                self._selected_rows_dict[1] = self._selected_rows_dict[1] & (
                     self.filtered_dataframe[prop] >= threshold
                 )
             else:
-                self.__selected_rows_dict[1] = self.__selected_rows_dict[1] & (
+                self._selected_rows_dict[1] = self._selected_rows_dict[1] & (
                     self.filtered_dataframe[prop] < threshold
                 )
 
         if self.current_fluorophore_id == 0 or self.current_fluorophore_id == 2:
             if larger_than:
-                self.__selected_rows_dict[2] = self.__selected_rows_dict[2] & (
+                self._selected_rows_dict[2] = self._selected_rows_dict[2] & (
                     self.filtered_dataframe[prop] >= threshold
                 )
             else:
-                self.__selected_rows_dict[2] = self.__selected_rows_dict[2] & (
+                self._selected_rows_dict[2] = self._selected_rows_dict[2] & (
                     self.filtered_dataframe[prop] < threshold
                 )
 
         # Apply the global filters
         self._apply_global_filters()
 
         # Make sure to flag the derived data to be recomputed
-        self.__stats_to_be_recomputed = True
-        self.__weighted_localizations_to_be_recomputed = True
+        self._stats_to_be_recomputed = True
+        self._weighted_localizations_to_be_recomputed = True
 
     def filter_by_1d_range(self, x_prop: str, x_range: tuple):
         """Apply min and max thresholding to the given property.
 
         Parameters
         ----------
 
@@ -562,33 +658,33 @@
         x_min = x_range[0]
         x_max = x_range[1]
         if x_max < x_min:
             x_max, x_min = x_min, x_max
 
         # Apply filter
         if self.current_fluorophore_id == 0 or self.current_fluorophore_id == 1:
-            self.__selected_rows_dict[1] = (
-                self.__selected_rows_dict[1]
+            self._selected_rows_dict[1] = (
+                self._selected_rows_dict[1]
                 & (self.filtered_dataframe[x_prop] >= x_min)
                 & (self.filtered_dataframe[x_prop] < x_max)
             )
 
         if self.current_fluorophore_id == 0 or self.current_fluorophore_id == 2:
-            self.__selected_rows_dict[2] = (
-                self.__selected_rows_dict[2]
+            self._selected_rows_dict[2] = (
+                self._selected_rows_dict[2]
                 & (self.filtered_dataframe[x_prop] >= x_min)
                 & (self.filtered_dataframe[x_prop] < x_max)
             )
 
         # Apply the global filters
         self._apply_global_filters()
 
         # Make sure to flag the derived data to be recomputed
-        self.__stats_to_be_recomputed = True
-        self.__weighted_localizations_to_be_recomputed = True
+        self._stats_to_be_recomputed = True
+        self._weighted_localizations_to_be_recomputed = True
 
     def filter_by_1d_range_complement(self, prop: str, x_range: tuple):
         """Apply min and max thresholding to the given property but keep the
         data outside the range (i.e., crop the selected range).
 
         Parameters
         ----------
@@ -604,82 +700,54 @@
         x_min = x_range[0]
         x_max = x_range[1]
         if x_max < x_min:
             x_max, x_min = x_min, x_max
 
         # Apply filter
         if self.current_fluorophore_id == 0 or self.current_fluorophore_id == 1:
-            self.__selected_rows_dict[1] = self.__selected_rows_dict[1] & (
+            self._selected_rows_dict[1] = self._selected_rows_dict[1] & (
                 (self.filtered_dataframe[prop] < x_min)
                 | (self.filtered_dataframe[prop] >= x_max)
             )
 
         if self.current_fluorophore_id == 0 or self.current_fluorophore_id == 2:
-            self.__selected_rows_dict[2] = self.__selected_rows_dict[2] & (
+            self._selected_rows_dict[2] = self._selected_rows_dict[2] & (
                 (self.filtered_dataframe[prop] < x_min)
                 | (self.filtered_dataframe[prop] >= x_max)
             )
 
         # Apply the global filters
         self._apply_global_filters()
 
         # Make sure to flag the derived data to be recomputed
-        self.__stats_to_be_recomputed = True
-        self.__weighted_localizations_to_be_recomputed = True
+        self._stats_to_be_recomputed = True
+        self._weighted_localizations_to_be_recomputed = True
 
     def _calculate_statistics(self):
         """Calculate per-trace statistics."""
 
         # Make sure we have processed dataframe to work on
         if self.full_dataframe is None:
             return
 
         # Only recompute statistics if needed
-        if not self.__stats_to_be_recomputed:
+        if not self._stats_to_be_recomputed:
             return
 
         # Work with currently selected rows
         df = self.filtered_dataframe
 
-        # Calculate some statistics per TID on the processed dataframe
-        df_grouped = df.groupby("tid")
-
-        tid = df_grouped["tid"].first().values
-        n = df_grouped["tid"].count().values
-        mx = df_grouped["x"].mean().values
-        my = df_grouped["y"].mean().values
-        mz = df_grouped["z"].mean().values
-        sx = df_grouped["x"].std().values
-        sy = df_grouped["y"].std().values
-        sz = df_grouped["z"].std().values
-        fluo = df_grouped["fluo"].agg(lambda x: mode(x, keepdims=True)[0][0]).values
-
-        # Prepare a dataframe with the statistics
-        df_tid = pd.DataFrame(
-            columns=["tid", "n", "mx", "my", "mz", "sx", "sy", "sz", "fluo"]
-        )
-
-        df_tid["tid"] = tid
-        df_tid["n"] = n
-        df_tid["mx"] = mx
-        df_tid["my"] = my
-        df_tid["mz"] = mz
-        df_tid["sx"] = sx
-        df_tid["sy"] = sy
-        df_tid["sz"] = sz
-        df_tid["fluo"] = fluo
-
-        # sx, sy sz columns will contain np.nan if n == 1: we replace with 0.0
-        df_tid[["sx", "sy", "sz"]] = df_tid[["sx", "sy", "sz"]].fillna(value=0.0)
+        # Calculate the statistics
+        df_tid = self.calculate_statistics_on(df)
 
         # Store the results
-        self.__filtered_stats_dataframe = df_tid
+        self._filtered_stats_dataframe = df_tid
 
         # Flag the statistics to be computed
-        self.__stats_to_be_recomputed = False
+        self._stats_to_be_recomputed = False
 
     @staticmethod
     def calculate_statistics_on(df: pd.DataFrame) -> pd.DataFrame:
         """Calculate per-trace statistics for the selected dataframe.
 
         Parameters
         ----------
@@ -700,54 +768,81 @@
         n = df_grouped["tid"].count().values
         mx = df_grouped["x"].mean().values
         my = df_grouped["y"].mean().values
         mz = df_grouped["z"].mean().values
         sx = df_grouped["x"].std().values
         sy = df_grouped["y"].std().values
         sz = df_grouped["z"].std().values
+        tmp = np.power(sx, 2) + np.power(sy, 2)
+        sxy = np.sqrt(tmp)
+        rms_xy = np.sqrt(tmp / 2)
+        exy = sxy / np.sqrt(n)
+        ez = sz / np.sqrt(n)
         fluo = df_grouped["fluo"].agg(lambda x: mode(x, keepdims=True)[0][0]).values
 
         # Prepare a dataframe with the statistics
         df_tid = pd.DataFrame(
-            columns=["tid", "n", "mx", "my", "mz", "sx", "sy", "sz", "fluo"]
+            columns=[
+                "tid",
+                "n",
+                "mx",
+                "my",
+                "mz",
+                "sx",
+                "sy",
+                "sxy",
+                "exy",
+                "rms_xy",
+                "sz",
+                "ez",
+                "fluo",
+            ]
         )
 
-        df_tid["tid"] = tid
-        df_tid["n"] = n
-        df_tid["mx"] = mx
-        df_tid["my"] = my
-        df_tid["mz"] = mz
-        df_tid["sx"] = sx
-        df_tid["sy"] = sy
-        df_tid["sz"] = sz
-        df_tid["fluo"] = fluo
-
-        # sx, sy sz columns will contain np.nan is n == 1: we replace with 0.0
-        # @TODO: should this be changed?
-        df_tid[["sx", "sy", "sz"]] = df_tid[["sx", "sy", "sz"]].fillna(value=0.0)
+        # Store trace stats
+        df_tid["tid"] = tid  # Trace ID
+        df_tid["n"] = n  # Number of traces for given ID
+        df_tid["mx"] = mx  # x mean localization
+        df_tid["my"] = my  # y mean localization
+        df_tid["mz"] = mz  # z mean localization
+        df_tid["sx"] = sx  # x localization precision
+        df_tid["sy"] = sy  # y localization precision
+        df_tid["sxy"] = sxy  # Lateral (x, y) localization precision
+        df_tid["rms_xy"] = rms_xy  # Lateral root mean square
+        df_tid["exy"] = exy  # Standard error of sxy
+        df_tid["sz"] = sz  # z localization precision
+        df_tid["ez"] = ez  # Standard error of ez
+        df_tid["fluo"] = fluo  # Assigned fluorophore ID
+
+        # ["sx", "sy", "sxy", "rms_xy", "exy", "sz", "ez"] columns will contain
+        # np.nan if n == 1: we replace them with 0.0.
+        # @TODO: should this be changed? It could be a global option.
+        df_tid[["sx", "sy", "sxy", "rms_xy", "exy", "sz", "ez"]] = df_tid[
+            ["sx", "sy", "sxy", "rms_xy", "exy", "sz", "ez"]
+        ].fillna(value=0.0)
 
         # Return the results
         return df_tid
 
     def _calculate_weighted_positions(self):
         """Calculate per-trace localization weighted by relative photon count."""
 
         # Make sure we have processed dataframe to work on
         if self.full_dataframe is None:
             return
 
         # Only recompute weighted localizations if needed
-        if not self.__weighted_localizations_to_be_recomputed:
+        if not self._weighted_localizations_to_be_recomputed:
             return
 
         # Work with currently selected rows
         df = self.filtered_dataframe
 
         # Normal or weighted averaging?
-        if self.__use_weighted_localizations:
+        if self._use_weighted_localizations:
             # Calculate weighing factors for TIDs
             df = df.assign(
                 eco_rel=df["eco"].groupby(df["tid"]).transform(lambda x: x / x.sum())
             )
 
             # Calculate relative contributions of (x, y, z)_i for each TID
             df["x_rel"] = df["x"] * df["eco_rel"]
@@ -780,11 +875,11 @@
         df_loc["tid"] = tid
         df_loc["x"] = x_w
         df_loc["y"] = y_w
         df_loc["z"] = z_w
         df_loc["fluo"] = fluo
 
         # Store the results
-        self.__weighted_localizations = df_loc
+        self._weighted_localizations = df_loc
 
         # Make sure to flag the derived data to be recomputed
-        self.__weighted_localizations_to_be_recomputed = False
+        self._weighted_localizations_to_be_recomputed = False
```

### Comparing `pyminflux-0.1.3/pyminflux/reader/__init__.py` & `pyminflux-0.2.0/pyminflux/ui/helpers/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,10 +7,9 @@
 #       http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #   limitations under the License.
-#
 
-from ._reader import MinFluxReader
+from ._helpers import export_plot_interactive, export_to_image
```

### Comparing `pyminflux-0.1.3/pyminflux/reader/_reader.py` & `pyminflux-0.2.0/pyminflux/reader/_reader.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,34 +18,36 @@
 
 import numpy as np
 import pandas as pd
 from scipy.io import loadmat
 
 
 class MinFluxReader:
+    __docs__ = "Reader of MINFLUX data in `.npy` or `.mat` formats."
+
     __slots__ = [
-        "__filename",
-        "__valid",
-        "__unit_scaling_factor",
-        "__data_array",
-        "__data_df",
-        "__data_full_df",
-        "__valid_entries",
-        "__is_3d",
-        "__is_aggregated",
-        "__reps",
-        "__efo_index",
-        "__cfr_index",
-        "__eco_index",
-        "__dcr_index",
-        "__loc_index",
-        "__tid_index",
-        "__tim_index",
-        "__vld_index",
-        "__z_scaling_factor",
+        "_filename",
+        "_valid",
+        "_unit_scaling_factor",
+        "_data_array",
+        "_data_df",
+        "_data_full_df",
+        "_valid_entries",
+        "_is_3d",
+        "_is_aggregated",
+        "_reps",
+        "_efo_index",
+        "_cfr_index",
+        "_eco_index",
+        "_dcr_index",
+        "_loc_index",
+        "_tid_index",
+        "_tim_index",
+        "_vld_index",
+        "_z_scaling_factor",
     ]
 
     def __init__(
         self,
         filename: Union[Path, str],
         valid: bool = True,
         unit_scaling_factor: float = 1e9,
@@ -53,116 +55,116 @@
     ):
         """Constructor.
 
         Parameters
         ----------
 
         filename: Union[Path, str]
-            Full path to the .npy file to read
+            Full path to the `.npy` or `.mat` file to read
 
         valid: bool (optional, default = True)
             Whether to load only valid localizations.
 
         unit_scaling_factor: float (optional, default = 1e9)
             Measurement are stored in meters, and by default they are
             scaled to be in nanometers.
 
         z_scaling_factor: float (optional, default = 1.0)
             Refractive index mismatch correction factor to apply to the z coordinates.
         """
 
         # Store the filename
-        self.__filename: Path = Path(filename)
-        if not self.__filename.is_file():
-            raise IOError(f"The file {self.__filename} does not seem to exist.")
+        self._filename: Path = Path(filename)
+        if not self._filename.is_file():
+            raise IOError(f"The file {self._filename} does not seem to exist.")
 
         # Store the valid flag
-        self.__valid: bool = valid
+        self._valid: bool = valid
 
         # Store the scaling factor
-        self.__unit_scaling_factor: float = unit_scaling_factor
+        self._unit_scaling_factor: float = unit_scaling_factor
 
         # Store the z correction factor
-        self.__z_scaling_factor: float = z_scaling_factor
+        self._z_scaling_factor: float = z_scaling_factor
 
         # Initialize the data
-        self.__data_array = None
-        self.__data_df = None
-        self.__data_full_df = None
-        self.__valid_entries = None
+        self._data_array = None
+        self._data_df = None
+        self._data_full_df = None
+        self._valid_entries = None
 
         # Whether the acquisition is 2D or 3D
-        self.__is_3d: bool = False
+        self._is_3d: bool = False
 
         # Whether the file contains aggregate measurements
-        self.__is_aggregated: bool = False
+        self._is_aggregated: bool = False
 
         # Indices dependent on 2D or 3D acquisition
-        self.__reps: int = -1
-        self.__efo_index: int = -1
-        self.__cfr_index: int = -1
-        self.__dcr_index: int = -1
-        self.__eco_index: int = -1
-        self.__loc_index: int = -1
+        self._reps: int = -1
+        self._efo_index: int = -1
+        self._cfr_index: int = -1
+        self._dcr_index: int = -1
+        self._eco_index: int = -1
+        self._loc_index: int = -1
 
         # Constant indices
-        self.__tid_index: int = 0
-        self.__tim_index: int = 0
-        self.__vld_index: int = 0
+        self._tid_index: int = 0
+        self._tim_index: int = 0
+        self._vld_index: int = 0
 
         # Load the file
         self._load()
 
     @property
     def is_3d(self):
         """Returns True is the acquisition is 3D, False otherwise."""
-        return self.__is_3d
+        return self._is_3d
 
     @property
     def is_aggregated(self):
         """Returns True is the acquisition is aggregated, False otherwise."""
-        return self.__is_aggregated
+        return self._is_aggregated
 
     @property
     def num_valid_entries(self):
         """Number of valid entries."""
-        if self.__data_array is None:
+        if self._data_array is None:
             return 0
-        return self.__valid_entries.sum()
+        return self._valid_entries.sum()
 
     @property
     def num_invalid_entries(self):
         """Number of valid entries."""
-        if self.__data_array is None:
+        if self._data_array is None:
             return 0
-        return np.logical_not(self.__valid_entries).sum()
+        return np.logical_not(self._valid_entries).sum()
 
     @property
     def valid_raw_data(self) -> Union[None, np.ndarray]:
         """Return the raw data."""
-        if self.__data_array is None:
+        if self._data_array is None:
             return None
-        return self.__data_array[self.__valid_entries].copy()
+        return self._data_array[self._valid_entries].copy()
 
     @property
     def processed_dataframe(self) -> Union[None, pd.DataFrame]:
         """Return the raw data as dataframe (some properties only)."""
-        if self.__data_df is not None:
-            return self.__data_df
+        if self._data_df is not None:
+            return self._data_df
 
-        self.__data_df = self._process()
-        return self.__data_df
+        self._data_df = self._process()
+        return self._data_df
 
     @property
     def raw_data_dataframe(self) -> Union[None, pd.DataFrame]:
         """Return the raw data as dataframe (some properties only)."""
-        if self.__data_full_df is not None:
-            return self.__data_full_df
-        self.__data_full_df = self._raw_data_to_full_dataframe()
-        return self.__data_full_df
+        if self._data_full_df is not None:
+            return self._data_full_df
+        self._data_full_df = self._raw_data_to_full_dataframe()
+        return self._data_full_df
 
     @classmethod
     def processed_properties(cls):
         """Returns the properties read from the file that correspond to the processed dataframe column names."""
         return [
             "tid",
             "tim",
@@ -181,81 +183,81 @@
     def raw_properties(cls):
         """Returns the properties read from the file and dynamic that correspond to the raw dataframe column names."""
         return ["tid", "aid", "vld", "tim", "x", "y", "z", "efo", "cfr", "eco", "dcr"]
 
     def _load(self) -> bool:
         """Load the file."""
 
-        if not self.__filename.is_file():
-            print(f"File {self.__filename} does not exist.")
+        if not self._filename.is_file():
+            print(f"File {self._filename} does not exist.")
             return False
 
         # Call the specialized _load_*() function
-        if self.__filename.name.lower().endswith(".npy"):
+        if self._filename.name.lower().endswith(".npy"):
             try:
-                data_array = np.load(str(self.__filename))
+                data_array = np.load(str(self._filename))
                 if "fluo" in data_array.dtype.names:
-                    self.__data_array = data_array
+                    self._data_array = data_array
                 else:
-                    self.__data_array = self._migrate_npy_array(data_array)
+                    self._data_array = self._migrate_npy_array(data_array)
             except ValueError as e:
-                print(f"Could not open {self.__filename}: {e}")
+                print(f"Could not open {self._filename}: {e}")
                 return False
 
-        elif self.__filename.name.lower().endswith(".mat"):
+        elif self._filename.name.lower().endswith(".mat"):
             try:
-                self.__data_array = self._convert_from_mat()
+                self._data_array = self._convert_from_mat()
             except ValueError as e:
-                print(f"Could not open {self.__filename}: {e}")
+                print(f"Could not open {self._filename}: {e}")
                 return False
         else:
-            print(f"Unexpected file {self.__filename}.")
+            print(f"Unexpected file {self._filename}.")
             return False
 
         # Store a logical array with the valid entries
-        self.__valid_entries = self.__data_array["vld"]
+        self._valid_entries = self._data_array["vld"]
 
         # Cache whether the data is 2D or 3D and whether is aggregated
-        num_locs = self.__data_array["itr"].shape[1]
+        num_locs = self._data_array["itr"].shape[1]
         if num_locs == 10:
-            self.__is_aggregated = False
-            self.__is_3d = True
+            self._is_aggregated = False
+            self._is_3d = True
         elif num_locs == 5:
-            self.__is_aggregated = False
-            self.__is_3d = False
+            self._is_aggregated = False
+            self._is_3d = False
         elif num_locs == 1:
-            self.__is_aggregated = True
-            self.__is_3d = np.nanmean(self.__data_array["itr"]["loc"][:, :, 2]) != 0.0
+            self._is_aggregated = True
+            self._is_3d = np.nanmean(self._data_array["itr"]["loc"][:, :, 2]) != 0.0
         else:
             print(f"Unexpected number of localizations per trace ({num_locs}).")
             return False
 
         # Set all relevant indices
         self._set_all_indices()
 
         # Return success
         return True
 
     def _convert_from_mat(self) -> Union[np.ndarray, None]:
         """Load the MAT file."""
 
         try:
-            mat_array = loadmat(str(self.__filename))
+            mat_array = loadmat(str(self._filename))
         except ValueError as e:
-            print(f"Could not open {self.__filename}: {e}")
+            print(f"Could not open {self._filename}: {e}")
             return None
 
         # Number of entries
         n_entries = len(mat_array["itr"]["itr"][0][0])
 
         # Number of iterations
         n_iters = mat_array["itr"]["itr"][0][0].shape[-1]
 
         # Initialize an empty structure NumPy data array
-        data_array = self.create_empty_data_array(n_entries, n_iters)
+        data_array = self._create_empty_data_array(n_entries, n_iters)
 
         # Copy the data over
         data_array["vld"] = mat_array["vld"].ravel().astype(data_array.dtype["vld"])
         data_array["sqi"] = mat_array["sqi"].ravel().astype(data_array.dtype["sqi"])
         data_array["gri"] = mat_array["gri"].ravel().astype(data_array.dtype["gri"])
         data_array["tim"] = mat_array["tim"].ravel().astype(data_array.dtype["tim"])
         data_array["tid"] = mat_array["tid"].ravel().astype(data_array.dtype["tid"])
@@ -336,42 +338,42 @@
         -------
 
         df: pd.DataFrame
             Processed data as DataFrame.
         """
 
         # Do we have a data array to work on?
-        if self.__data_array is None:
+        if self._data_array is None:
             return None
 
-        if self.__valid:
-            indices = self.__valid_entries
+        if self._valid:
+            indices = self._valid_entries
         else:
-            indices = np.logical_not(self.__valid_entries)
+            indices = np.logical_not(self._valid_entries)
 
         # Extract the valid iterations
-        itr = self.__data_array["itr"][indices]
+        itr = self._data_array["itr"][indices]
 
         # Extract the valid identifiers
-        tid = self.__data_array["tid"][indices]
+        tid = self._data_array["tid"][indices]
 
         # Extract the valid time points
-        tim = self.__data_array["tim"][indices]
+        tim = self._data_array["tim"][indices]
 
         # Extract the fluorophore IDs
-        fluo = self.__data_array["fluo"][indices]
+        fluo = self._data_array["fluo"][indices]
         if np.all(fluo) == 0:
             fluo = np.ones(fluo.shape, dtype=fluo.dtype)
 
         # The following extraction pattern will change whether the
         # acquisition is normal or aggregated
         if self.is_aggregated:
             # Extract the locations
-            loc = itr["loc"].squeeze() * self.__unit_scaling_factor
-            loc[:, 2] = loc[:, 2] * self.__z_scaling_factor
+            loc = itr["loc"].squeeze() * self._unit_scaling_factor
+            loc[:, 2] = loc[:, 2] * self._z_scaling_factor
 
             # Extract EFO
             efo = itr["efo"]
 
             # Extract CFR
             cfr = itr["cfr"]
 
@@ -382,28 +384,28 @@
             dcr = itr["dcr"]
 
             # Dwell
             dwell = np.around(eco / (efo / 1000.0), decimals=0)
 
         else:
             # Extract the locations
-            loc = itr[:, self.__loc_index]["loc"] * self.__unit_scaling_factor
-            loc[:, 2] = loc[:, 2] * self.__z_scaling_factor
+            loc = itr[:, self._loc_index]["loc"] * self._unit_scaling_factor
+            loc[:, 2] = loc[:, 2] * self._z_scaling_factor
 
             # Extract EFO
-            efo = itr[:, self.__efo_index]["efo"]
+            efo = itr[:, self._efo_index]["efo"]
 
             # Extract CFR
-            cfr = itr[:, self.__cfr_index]["cfr"]
+            cfr = itr[:, self._cfr_index]["cfr"]
 
             # Extract ECO
-            eco = itr[:, self.__eco_index]["eco"]
+            eco = itr[:, self._eco_index]["eco"]
 
             # Extract DCR
-            dcr = itr[:, self.__dcr_index]["dcr"]
+            dcr = itr[:, self._dcr_index]["dcr"]
 
             # Calculate dwell
             dwell = np.around(eco / (efo / 1000.0), decimals=0)
 
         # Create a Pandas dataframe for the results
         df = pd.DataFrame(
             index=pd.RangeIndex(start=0, stop=len(tid)),
@@ -423,63 +425,63 @@
         df["dwell"] = dwell
         df["fluo"] = fluo
 
         return df
 
     def _raw_data_to_full_dataframe(self) -> Union[None, pd.DataFrame]:
         """Return raw data arranged into a dataframe."""
-        if self.__data_array is None:
+        if self._data_array is None:
             return None
 
         # Intialize output dataframe
         df = pd.DataFrame(columns=MinFluxReader.raw_properties())
 
         # Allocate space for the columns
-        n_rows = len(self.__data_array) * self.__reps
+        n_rows = len(self._data_array) * self._reps
 
         # Get all unique TIDs and their counts
-        _, tid_counts = np.unique(self.__data_array["tid"], return_counts=True)
+        _, tid_counts = np.unique(self._data_array["tid"], return_counts=True)
 
         # Get all tids (repeated over the repetitions)
-        tid = np.repeat(self.__data_array["tid"], self.__reps)
+        tid = np.repeat(self._data_array["tid"], self._reps)
 
         # Create virtual IDs to mark the measurements of repeated tids
         # @TODO Optimize this!
         aid = np.zeros((n_rows, 1), dtype=np.int32)
         index = 0
         for c in np.nditer(tid_counts):
-            tmp = np.repeat(np.arange(c), self.__reps)
+            tmp = np.repeat(np.arange(c), self._reps)
             n = len(tmp)
             aid[index : index + n, 0] = tmp
             index += n
 
         # Get all valid flags (repeated over the repetitions)
-        vld = np.repeat(self.__data_array["vld"], self.__reps)
+        vld = np.repeat(self._data_array["vld"], self._reps)
 
         # Get all timepoints (repeated over the repetitions)
-        tim = np.repeat(self.__data_array["tim"], self.__reps)
+        tim = np.repeat(self._data_array["tim"], self._reps)
 
         # Get all localizations (reshaped to drop the first dimension)
         loc = (
-            self.__data_array["itr"]["loc"].reshape((n_rows, 3))
-            * self.__unit_scaling_factor
+            self._data_array["itr"]["loc"].reshape((n_rows, 3))
+            * self._unit_scaling_factor
         )
-        loc[:, 2] = loc[:, 2] * self.__z_scaling_factor
+        loc[:, 2] = loc[:, 2] * self._z_scaling_factor
 
         # Get all efos (reshaped to drop the first dimension)
-        efo = self.__data_array["itr"]["efo"].reshape((n_rows, 1))
+        efo = self._data_array["itr"]["efo"].reshape((n_rows, 1))
 
         # Get all cfrs (reshaped to drop the first dimension)
-        cfr = self.__data_array["itr"]["cfr"].reshape((n_rows, 1))
+        cfr = self._data_array["itr"]["cfr"].reshape((n_rows, 1))
 
         # Get all ecos (reshaped to drop the first dimension)
-        eco = self.__data_array["itr"]["eco"].reshape((n_rows, 1))
+        eco = self._data_array["itr"]["eco"].reshape((n_rows, 1))
 
         # Get all dcrs (reshaped to drop the first dimension)
-        dcr = self.__data_array["itr"]["dcr"].reshape((n_rows, 1))
+        dcr = self._data_array["itr"]["dcr"].reshape((n_rows, 1))
 
         # Build the dataframe
         df["tid"] = tid.astype(np.int32)
         df["aid"] = aid.astype(np.int32)
         df["vld"] = vld
         df["tim"] = tim
         df["x"] = loc[:, 0]
@@ -490,41 +492,41 @@
         df["eco"] = eco
         df["dcr"] = dcr
 
         return df
 
     def _set_all_indices(self):
         """Set indices of properties to be read."""
-        if self.__data_array is None:
+        if self._data_array is None:
             return False
 
         if self.is_aggregated:
-            self.__reps = 1
-            self.__efo_index = -1  # Not used
-            self.__cfr_index = -1  # Not used
-            self.__dcr_index = -1  # Not used
-            self.__eco_index = -1  # Not used
-            self.__loc_index = -1  # Not used
+            self._reps = 1
+            self._efo_index = -1  # Not used
+            self._cfr_index = -1  # Not used
+            self._dcr_index = -1  # Not used
+            self._eco_index = -1  # Not used
+            self._loc_index = -1  # Not used
         else:
             if self.is_3d:
-                self.__reps = 10
-                self.__efo_index = 9
-                self.__cfr_index = 6
-                self.__dcr_index = 9
-                self.__eco_index = 9
-                self.__loc_index = 9
+                self._reps = 10
+                self._efo_index = 9
+                self._cfr_index = 6
+                self._dcr_index = 9
+                self._eco_index = 9
+                self._loc_index = 9
             else:
-                self.__reps = 5
-                self.__efo_index = 4
-                self.__cfr_index = 4
-                self.__dcr_index = 4
-                self.__eco_index = 4
-                self.__loc_index = 4
+                self._reps = 5
+                self._efo_index = 4
+                self._cfr_index = 4
+                self._dcr_index = 4
+                self._eco_index = 4
+                self._loc_index = 4
 
-    def create_empty_data_array(self, n_entries: int, n_iters: int):
+    def _create_empty_data_array(self, n_entries: int, n_iters: int):
         """Initializes a structured data array compatible with those exported from Imspector.
 
         Parameters
         ----------
 
         n_entries: int
             Number of localizations in the array.
@@ -586,40 +588,40 @@
             ),
         )
 
     def _migrate_npy_array(self, data_array):
         """Migrate the raw Imspector NumPy array into a pyMINFLUX raw array."""
 
         # Initialize the empty target array
-        new_array = self.create_empty_data_array(
+        new_array = self._create_empty_data_array(
             len(data_array), data_array["itr"].shape[-1]
         )
 
         # Copy the data over
         for field_name in data_array.dtype.names:
             new_array[field_name] = data_array[field_name]
 
         # Return the migrated array
         return new_array
 
     def __repr__(self):
         """String representation of the object."""
-        if self.__data_array is None:
+        if self._data_array is None:
             return "No file loaded."
 
         str_valid = (
             "all valid"
-            if len(self.__data_array) == self.num_valid_entries
+            if len(self._data_array) == self.num_valid_entries
             else f"{self.num_valid_entries} valid and {self.num_invalid_entries} non valid"
         )
 
         str_acq = "3D" if self.is_3d else "2D"
         aggr_str = "aggregated" if self.is_aggregated else "normal"
 
         return (
-            f"File: {self.__filename.name}: "
-            f"{str_acq} {aggr_str} acquisition with {len(self.__data_array)} entries ({str_valid})."
+            f"File: {self._filename.name}: "
+            f"{str_acq} {aggr_str} acquisition with {len(self._data_array)} entries ({str_valid})."
         )
 
     def __str__(self):
         """Human-friendly representation of the object."""
         return self.__repr__()
```

### Comparing `pyminflux-0.1.3/pyminflux/resources.py` & `pyminflux-0.2.0/pyminflux/resources.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.3/pyminflux/resources.qrc` & `pyminflux-0.2.0/pyminflux/resources.qrc`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.3/pyminflux/settings/__init__.py` & `pyminflux-0.2.0/pyminflux/threads/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 
-from ._settings import Settings
+from ._threads import *
```

### Comparing `pyminflux-0.1.3/pyminflux/settings/_settings.py` & `pyminflux-0.2.0/pyminflux/settings/_settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,24 +16,20 @@
 import os
 import platform
 from pathlib import Path
 
 from PySide6.QtCore import QSettings
 
 from pyminflux import __APP_NAME__
-from pyminflux.state import State
 
 
 class Settings:
     def __init__(self):
         """Constructor."""
 
-        # Initialize the State
-        self.state = State()
-
         # Define the organization and application names
         self.org_name = "ch.ethz"
         self.app_name = __APP_NAME__
 
         # Construct the file path for the INI file based on the platform
         if platform.system() == "Windows":
             config_folder = Path(os.environ["APPDATA"]) / self.org_name
```

### Comparing `pyminflux-0.1.3/pyminflux/state/__init__.py` & `pyminflux-0.2.0/pyminflux/ui/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,9 +8,7 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #   limitations under the License.
 #
-
-from ._state import ColorCode, State
```

### Comparing `pyminflux-0.1.3/pyminflux/state/_state.py` & `pyminflux-0.2.0/pyminflux/state/_state.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,28 +10,31 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 
 from enum import IntEnum
-from pprint import pprint
 from typing import Union
 
 from ..base import Singleton
 
 
 class ColorCode(IntEnum):
     NONE = 0
     BY_TID = 1
     BY_FLUO = 2
 
 
 class State(metaclass=Singleton):
-    """State machine (singleton class)."""
+    """State machine (singleton class).
+
+    This keeps the State for the user interface! That is, only classes under pyminflux.ui
+    should use State()! The core API must remain independent of State!
+    """
 
     __SLOTS__ = [
         "plot_average_localisations",
         "color_code",
         "min_num_loc_per_trace",
         "efo_expected_frequency",
         "efo_thresholds",
@@ -47,14 +50,18 @@
         "x_param",
         "y_param",
         "num_fluorophores",
         "dcr_bin_size",
         "dcr_manual_threshold",
         "z_scaling_factor",
         "plot_export_dpi",
+        "frc_lateral_resolution",
+        "frc_temporal_resolution",
+        "frc_num_repeats",
+        "frc_endpoint_only",
     ]
 
     def __init__(self):
         """Constructor.
 
         A singleton object of this dataclass acts as a state machine that allows various parts of the
         application to synchronize state among them.
@@ -103,14 +110,20 @@
 
         # Z scaling factor
         self.z_scaling_factor: float = 0.7
 
         # Resolution for exporting plots as images
         self.plot_export_dpi: int = 600
 
+        # FRC analysis
+        self.frc_lateral_resolution: float = 4.0
+        self.frc_temporal_resolution: float = 1800.0
+        self.frc_num_repeats: int = 5
+        self.frc_endpoint_only: bool = False
+
     def asdict(self) -> dict:
         """Return class as dictionary."""
         return {
             "min_num_loc_per_trace": self.min_num_loc_per_trace,
             "plot_average_localisations": self.plot_average_localisations,
             "color_code": str(ColorCode(self.color_code)),
             "efo_expected_frequency": self.efo_expected_frequency,
@@ -127,14 +140,18 @@
             "x_param": self.x_param,
             "y_param": self.y_param,
             "num_fluorophores": self.num_fluorophores,
             "dcr_bin_size": self.dcr_bin_size,
             "dcr_manual_threshold": self.dcr_manual_threshold,
             "z_scaling_factor": self.z_scaling_factor,
             "plot_export_dpi": self.plot_export_dpi,
+            "frc_lateral_resolution": self.frc_lateral_resolution,
+            "frc_temporal_resolution": self.frc_temporal_resolution,
+            "frc_num_repeats": self.frc_num_repeats,
+            "frc_endpoint_only": self.frc_endpoint_only,
         }
 
     def reset(self):
         """Reset to data-specific settings."""
 
         self.efo_thresholds = None
         self.cfr_thresholds = None
@@ -159,14 +176,18 @@
         self.x_param = "x"
         self.y_param = "y"
         self.num_fluorophores = 1
         self.dcr_bin_size = 0.0
         self.dcr_manual_threshold = 0.0
         self.z_scaling_factor = 0.7
         self.plot_export_dpi = 600
+        self.frc_lateral_resolution = 4.0
+        self.frc_temporal_resolution = 1800.0
+        self.frc_num_repeats = 5
+        self.frc_endpoint_only = False
 
     def __str__(self):
         """Human-readable representation."""
         self.__repr__()
 
     def __repr__(self):
         """State representation."""
```

### Comparing `pyminflux-0.1.3/pyminflux/threads/__init__.py` & `pyminflux-0.2.0/pyminflux/correct/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,10 +7,15 @@
 #       http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #   limitations under the License.
-#
 
-from ._threads import *
+__doc__ = "Correction/restoration functions."
+__all__ = [
+    "drift_correction_time_windows_2d",
+    "drift_correction_time_windows_3d",
+]
+
+from ._correct import drift_correction_time_windows_2d, drift_correction_time_windows_3d
```

### Comparing `pyminflux-0.1.3/pyminflux/threads/_threads.py` & `pyminflux-0.2.0/pyminflux/threads/_threads.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.3/pyminflux/ui/__init__.py` & `pyminflux-0.2.0/pyminflux/processor/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,7 +8,14 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #   limitations under the License.
 #
+
+__doc__ = "Processor of MINFLUX data."
+__all__ = [
+    "MinFluxProcessor",
+]
+
+from ._processor import MinFluxProcessor
```

### Comparing `pyminflux-0.1.3/pyminflux/ui/analyzer.py` & `pyminflux-0.2.0/pyminflux/ui/analyzer.py`

 * *Files 7% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         super().__init__(parent=parent)
 
         # Initialize the dialog
         self.ui = Ui_Analyzer()
         self.ui.setupUi(self)
 
         # Store the reference to the reader
-        self._minfluxprocessor = minfluxprocessor
+        self.processor = minfluxprocessor
 
         # Reference to the communications label
         self.communication_label = None
 
         # Keep references to the plots
         self.efo_plot = None
         self.cfr_plot = None
@@ -200,15 +200,15 @@
         """Key press event."""
 
         # Do not capture key events for now
         ev.ignore()
 
     def set_processor(self, minfluxprocessor: MinFluxProcessor):
         """Reset the internal state."""
-        self._minfluxprocessor = minfluxprocessor
+        self.processor = minfluxprocessor
         self.efo_region = None
         self.cfr_region = None
         self.efo_range = None
         self.cfr_range = None
 
     @Slot(name="run_efo_cutoff_frequency_detection")
     def run_efo_cutoff_frequency_detection(self):
@@ -218,30 +218,30 @@
         frequency = 2.0 * float(self.ui.leEFOExpectedCutoff.text())
 
         # Histogram bin settings
         efo_auto_bins = self.state.efo_bin_size_hz == 0
 
         # Calculate thresholds for EFO
         n_efo, _, b_efo, _ = prepare_histogram(
-            self._minfluxprocessor.filtered_dataframe["efo"].values,
+            self.processor.filtered_dataframe["efo"].values,
             auto_bins=efo_auto_bins,
             bin_size=self.state.efo_bin_size_hz,
         )
         cutoff_frequency = find_cutoff_near_value(
             counts=n_efo,
             bins=b_efo,
             expected_value=frequency,
         )
 
         # If the search failed, we return
         if cutoff_frequency is None:
             return
 
         # Set the new upper bound and reset the lower bound
-        min_efo = self._minfluxprocessor.filtered_dataframe["efo"].values.min()
+        min_efo = self.processor.filtered_dataframe["efo"].values.min()
         max_efo = cutoff_frequency
         self.state.efo_thresholds = (min_efo, max_efo)
 
         # Update plot
         self.efo_region.setRegion(self.state.efo_thresholds)
 
     @Slot(name="run_cfr_auto_threshold")
@@ -254,23 +254,23 @@
             and not self.state.enable_cfr_upper_threshold
         ):
             print("Both lower and upper CFR thresholds are disabled.")
             return
 
         # Initialize values
         if self.state.cfr_thresholds is None:
-            min_cfr = self._minfluxprocessor.filtered_dataframe["cfr"].values.min()
-            max_cfr = self._minfluxprocessor.filtered_dataframe["cfr"].values.max()
+            min_cfr = self.processor.filtered_dataframe["cfr"].values.min()
+            max_cfr = self.processor.filtered_dataframe["cfr"].values.max()
         else:
             min_cfr = self.state.cfr_thresholds[0]
             max_cfr = self.state.cfr_thresholds[1]
 
         # Calculate thresholds for CFR
         upper_thresh_cfr, lower_thresh_cfr, _, _ = get_robust_threshold(
-            self._minfluxprocessor.filtered_dataframe["cfr"].values,
+            self.processor.filtered_dataframe["cfr"].values,
             factor=self.state.cfr_threshold_factor,
         )
         if self.state.enable_cfr_lower_threshold:
             min_cfr = lower_thresh_cfr
         if self.state.enable_cfr_upper_threshold:
             max_cfr = upper_thresh_cfr
         self.state.cfr_thresholds = (min_cfr, max_cfr)
@@ -309,15 +309,15 @@
 
     @Slot(name="run_efo_filter_and_broadcast_viewers_update")
     def run_efo_filter_and_broadcast_viewers_update(self):
         """Apply the EFO filter and inform the rest of the application that the data viewers should be updated."""
 
         # Apply the EFO filter if needed
         if self.state.efo_thresholds is not None:
-            self._minfluxprocessor.filter_by_1d_range(
+            self.processor.filter_by_1d_range(
                 "efo", (self.state.efo_thresholds[0], self.state.efo_thresholds[1])
             )
 
         # Update the histograms
         self.plot()
 
         # Signal that the external viewers should be updated
@@ -325,15 +325,15 @@
 
     @Slot(name="run_cfr_filter_and_broadcast_viewers_update")
     def run_cfr_filter_and_broadcast_viewers_update(self):
         """Apply the CFR filter and inform the rest of the application that the data viewers should be updated."""
 
         # Apply the CFR filter if needed
         if self.state.cfr_thresholds is not None:
-            self._minfluxprocessor.filter_by_1d_range(
+            self.processor.filter_by_1d_range(
                 "cfr", (self.state.cfr_thresholds[0], self.state.cfr_thresholds[1])
             )
 
         # Update the histograms
         self.plot()
 
         # Signal that the external viewers should be updated
@@ -357,21 +357,21 @@
         """Plot histograms."""
 
         # Hide the communications label
         self.communication_label.hide()
 
         # Make sure there is data to plot
         is_data = True
-        if self._minfluxprocessor is None:
+        if self.processor is None:
             is_data = False
 
-        if self._minfluxprocessor.filtered_dataframe is None:
+        if self.processor.filtered_dataframe is None:
             is_data = False
 
-        if self._minfluxprocessor.num_values == 0:
+        if self.processor.num_values == 0:
             is_data = False
 
         # Announce that the plotting has started
         self.plotting_started.emit()
 
         for item in self.efo_plot.allChildItems():
             self.efo_plot.removeItem(item)
@@ -395,20 +395,20 @@
             return
 
         # Histogram bin settings
         efo_auto_bins = self.state.efo_bin_size_hz == 0
 
         # Calculate the proper aspect ratio and view ranges for the relevant plots
         n_efo, efo_bin_edges, efo_bin_centers, efo_bin_width = prepare_histogram(
-            self._minfluxprocessor.filtered_dataframe["efo"].values,
+            self.processor.filtered_dataframe["efo"].values,
             auto_bins=efo_auto_bins,
             bin_size=self.state.efo_bin_size_hz,
         )
         n_cfr, cfr_bin_edges, cfr_bin_centers, cfr_bin_width = prepare_histogram(
-            self._minfluxprocessor.filtered_dataframe["cfr"].values,
+            self.processor.filtered_dataframe["cfr"].values,
             auto_bins=True,
             bin_size=0.0,
         )
 
         #
         # Get "efo" and "cfr" measurements, and "sx", "sy" and "sz" localization jitter
         #
@@ -450,15 +450,15 @@
             thresholds=self.state.cfr_thresholds,
             force_min_x_range_to_zero=False,
         )
         self.cfr_plot.show()
 
         # sx
         n_sx, sx_bin_edges, sx_bin_centers, sx_bin_width = prepare_histogram(
-            self._minfluxprocessor.filtered_dataframe_stats["sx"].values,
+            self.processor.filtered_dataframe_stats["sx"].values,
             auto_bins=True,
             bin_size=0.0,
         )
         _ = self._create_histogram_plot(
             "sx",
             self.sx_plot,
             n_sx,
@@ -466,21 +466,21 @@
             sx_bin_centers,
             sx_bin_width,
             axis_range=self.loc_precision_range,
             brush="k",
             support_thresholding=False,
         )
         self._add_median_line(
-            self.sx_plot, self._minfluxprocessor.filtered_dataframe_stats["sx"].values
+            self.sx_plot, self.processor.filtered_dataframe_stats["sx"].values
         )
         self.sx_plot.show()
 
         # sy
         n_sy, sy_bin_edges, sy_bin_centers, sy_bin_width = prepare_histogram(
-            self._minfluxprocessor.filtered_dataframe_stats["sy"].values,
+            self.processor.filtered_dataframe_stats["sy"].values,
             auto_bins=True,
             bin_size=0.0,
         )
         _ = self._create_histogram_plot(
             "sy",
             self.sy_plot,
             n_sy,
@@ -488,22 +488,22 @@
             sy_bin_centers,
             sy_bin_width,
             axis_range=self.loc_precision_range,
             brush="k",
             support_thresholding=False,
         )
         self._add_median_line(
-            self.sy_plot, self._minfluxprocessor.filtered_dataframe_stats["sy"].values
+            self.sy_plot, self.processor.filtered_dataframe_stats["sy"].values
         )
         self.sy_plot.show()
 
         # sz
-        if self._minfluxprocessor.is_3d:
+        if self.processor.is_3d:
             n_sz, sz_bin_edges, sz_bin_centers, sz_bin_width = prepare_histogram(
-                self._minfluxprocessor.filtered_dataframe_stats["sz"].values,
+                self.processor.filtered_dataframe_stats["sz"].values,
                 auto_bins=True,
                 bin_size=0.0,
             )
             _ = self._create_histogram_plot(
                 "sz",
                 self.sz_plot,
                 n_sz,
@@ -512,15 +512,15 @@
                 sz_bin_width,
                 axis_range=self.loc_precision_range,
                 brush="k",
                 support_thresholding=False,
             )
             self._add_median_line(
                 self.sz_plot,
-                self._minfluxprocessor.filtered_dataframe_stats["sz"].values,
+                self.processor.filtered_dataframe_stats["sz"].values,
             )
             self.sz_plot.show()
         else:
             self.sz_plot.hide()
 
         # Announce that the plotting has completed
         self.plotting_completed.emit()
```

### Comparing `pyminflux-0.1.3/pyminflux/ui/analyzer.ui` & `pyminflux-0.2.0/pyminflux/ui/analyzer.ui`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.3/pyminflux/ui/assets/Logo_v3.icns` & `pyminflux-0.2.0/pyminflux/ui/assets/Logo_v3.icns`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.3/pyminflux/ui/assets/Logo_v3.ico` & `pyminflux-0.2.0/pyminflux/ui/assets/Logo_v3.ico`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.3/pyminflux/ui/assets/Logo_v3.png` & `pyminflux-0.2.0/pyminflux/ui/assets/Logo_v3.png`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.3/pyminflux/ui/assets/Logo_v3_small.png` & `pyminflux-0.2.0/pyminflux/ui/assets/Logo_v3_small.png`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.3/pyminflux/ui/assets/create_resources.sh` & `pyminflux-0.2.0/pyminflux/ui/assets/create_resources.sh`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.3/pyminflux/ui/assets/png_to_icns.sh` & `pyminflux-0.2.0/pyminflux/ui/assets/png_to_icns.sh`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.3/pyminflux/ui/color_unmixer.py` & `pyminflux-0.2.0/pyminflux/ui/color_unmixer.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,19 +13,18 @@
 #   limitations under the License.
 #
 
 import numpy as np
 import pyqtgraph as pg
 from pyqtgraph import PlotWidget
 from PySide6.QtCore import QPoint, Signal, Slot
-from PySide6.QtGui import QAction, QDoubleValidator, QIntValidator, Qt
+from PySide6.QtGui import QAction, QDoubleValidator, Qt
 from PySide6.QtWidgets import QDialog, QMenu
-from sklearn.mixture import BayesianGaussianMixture
 
-from pyminflux.analysis import prepare_histogram
+from pyminflux.analysis import assign_data_to_clusters, prepare_histogram
 from pyminflux.state import State
 from pyminflux.ui.helpers import export_plot_interactive
 from pyminflux.ui.ui_color_unmixer import Ui_ColorUnmixer
 
 
 class ColorUnmixer(QDialog, Ui_ColorUnmixer):
     """
@@ -55,15 +54,15 @@
         self.ui.leManualThreshold.setText(str(self.state.dcr_manual_threshold))
 
         # Constants
         self.brush = pg.mkBrush(0, 0, 0, 255)
         self.pen = pg.mkPen(None)
 
         # Keep a reference to the Processor
-        self._minfluxprocessor = processor
+        self.processor = processor
 
         # Keep track of the global data range and step
         self.n_dcr_max = None
         self.dcr_bin_edges = None
         self.dcr_bin_centers = None
         self.dcr_bin_width = None
 
@@ -114,30 +113,27 @@
         self.state.dcr_manual_threshold = float(dcr_manual_threshold)
 
     @Slot(None, name="plot_dcr_histogram")
     def plot_dcr_histogram(self):
         """Plot the dcr histogram. This is always performed assuming all data belongs to one fluorophore."""
 
         # Do we have something to plot?
-        if (
-            self._minfluxprocessor is None
-            or self._minfluxprocessor.full_dataframe is None
-        ):
+        if self.processor is None or self.processor.full_dataframe is None:
             return
 
         if self.state.dcr_bin_size == 0:
             # Calculate the dcr histogram
             n_dcr, dcr_bin_edges, dcr_bin_centers, dcr_bin_width = prepare_histogram(
-                self._minfluxprocessor.full_dataframe["dcr"].values,
+                self.processor.full_dataframe["dcr"].values,
                 auto_bins=True,
             )
         else:
             # Calculate the dcr histogram
             n_dcr, dcr_bin_edges, dcr_bin_centers, dcr_bin_width = prepare_histogram(
-                self._minfluxprocessor.full_dataframe["dcr"].values,
+                self.processor.full_dataframe["dcr"].values,
                 auto_bins=False,
                 bin_size=self.state.dcr_bin_size,
             )
 
         # Remember the global histogram range and step
         self.n_dcr_max = n_dcr.max()
         self.dcr_bin_edges = dcr_bin_edges
@@ -170,15 +166,15 @@
         )
 
     @Slot(None, name="preview_manual_assignment")
     def preview_manual_assignment(self):
         """Preview the manual assignment."""
 
         # Get the data
-        dcr = self._minfluxprocessor.full_dataframe["dcr"].values
+        dcr = self.processor.full_dataframe["dcr"].values
         if len(dcr) == 0:
             return
 
         # Get the threshold
         threshold = float(self.ui.leManualThreshold.text())
 
         # Keep track of the total number of elements for normalisation
@@ -227,96 +223,72 @@
         self.ui.pbManualAssign.setEnabled(True)
 
     @Slot(None, name="detect_fluorophores")
     def detect_fluorophores(self):
         """Detect fluorophores."""
 
         # Get the data
-        dcr = self._minfluxprocessor.full_dataframe["dcr"].values
+        dcr = self.processor.full_dataframe["dcr"].values
         if len(dcr) == 0:
             return
 
-        # Prepare the data
-        values = dcr.reshape(-1, 1)
-
-        # Keep track of the total number of elements for normalisation
-        n_total = len(values)
-
-        # Fit a Bayesian Gaussian Mixture Model with self.state.num_fluorophores components
-        model = BayesianGaussianMixture(
-            n_components=self.state.num_fluorophores,
-            init_params="k-means++",
-            covariance_type="full",
-            max_iter=1000,
-            random_state=42,
-        ).fit(values)
-
-        # Predict with the selected model
-        y_pred = model.predict(values)
+        # Fit the data to the requested number of clusters
+        fluo_ids = assign_data_to_clusters(dcr, self.state.num_fluorophores, seed=42)
 
         # It one or more charts already exists, remove them
         for item in self.plot_widget.allChildItems():
             self.plot_widget.removeItem(item)
 
         # Prepare some colors
         brushes = ["b", "r", "g", "m", "c"]
 
         # Calculate the bar width as a function of the number of fluorophores
         bar_width = 0.9 / self.state.num_fluorophores
         offset = self.dcr_bin_width / self.state.num_fluorophores
 
-        # If there is more than one fluorophore, sort the indices by mean dcr values,
-        # from low to high (to match the assignment of the manual thresholding)
-        if self.state.num_fluorophores > 1:
-            means = [np.mean(values[y_pred == f_id]) for f_id in np.unique(y_pred)]
-            sorted_f = np.argsort(means)
-            for f in range(self.state.num_fluorophores):
-                if np.isnan(means[f]):
-                    continue
-                n = sorted_f[f] + self.state.num_fluorophores
-                y_pred[y_pred == f] = n
-            y_pred -= self.state.num_fluorophores
+        # Keep track of the total number of values for histogrm normalization
+        n_values = len(dcr)
 
         # Create new histograms
-        for f in range(self.state.num_fluorophores):
-            data = values[y_pred == f]
+        for f in range(1, self.state.num_fluorophores + 1):
+            data = dcr[fluo_ids == f]
             if len(data) == 0:
                 continue
 
             # Calculate the dcr histogram using the global bins
             n_dcr, _ = np.histogram(data, bins=self.dcr_bin_edges, density=False)
 
             # Normalize by the total count
-            n_dcr = n_dcr / n_total
+            n_dcr = n_dcr / n_values
 
             # Create the bar chart
             chart = pg.BarGraphItem(
                 x=self.dcr_bin_centers + f * offset,
                 height=n_dcr,
                 width=bar_width * self.dcr_bin_width,
-                brush=brushes[f],
+                brush=brushes[f - 1],
                 alpha=0.5,
             )
             self.plot_widget.addItem(chart)
 
         # Store the predictions (1-shifted)
-        self.assigned_fluorophore_ids = y_pred + 1
+        self.assigned_fluorophore_ids = fluo_ids
 
         # Make sure to enable the assign button
         self.ui.pbAssign.setEnabled(True)
 
     @Slot(None, name="assign_fluorophores_ids")
     def assign_fluorophores_ids(self):
         """Assign the fluorophores ids."""
 
         if self.assigned_fluorophore_ids is None:
             return
 
         # Assign the IDs via the processor
-        self._minfluxprocessor.set_fluorophore_ids(self.assigned_fluorophore_ids)
+        self.processor.set_fluorophore_ids(self.assigned_fluorophore_ids)
 
         # Inform that the fluorophore IDs have been assigned
         self.fluorophore_ids_assigned.emit(
             len(np.unique(self.assigned_fluorophore_ids))
         )
 
         # Disable the button until the new detection is run
```

### Comparing `pyminflux-0.1.3/pyminflux/ui/color_unmixer.ui` & `pyminflux-0.2.0/pyminflux/ui/color_unmixer.ui`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.3/pyminflux/ui/dataviewer.py` & `pyminflux-0.2.0/pyminflux/ui/dataviewer.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.3/pyminflux/ui/emittingstream.py` & `pyminflux-0.2.0/pyminflux/ui/emittingstream.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.3/pyminflux/ui/helpers/__init__.py` & `pyminflux-0.2.0/pyminflux/fourier/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,8 +8,21 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #   limitations under the License.
 
-from ._helpers import export_plot_interactive, export_to_image
+__doc__ = "Fourier-based functions."
+__all__ = [
+    "img_fourier_grid",
+    "img_fourier_ring_correlation",
+    "estimate_resolution_by_frc",
+    "get_localization_boundaries",
+]
+
+from ._fourier import (
+    estimate_resolution_by_frc,
+    get_localization_boundaries,
+    img_fourier_grid,
+    img_fourier_ring_correlation,
+)
```

### Comparing `pyminflux-0.1.3/pyminflux/ui/helpers/_helpers.py` & `pyminflux-0.2.0/pyminflux/ui/helpers/_helpers.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.3/pyminflux/ui/icons/icon.png` & `pyminflux-0.2.0/pyminflux/ui/icons/icon.png`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.3/pyminflux/ui/main_window.py` & `pyminflux-0.2.0/pyminflux/ui/main_window.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,38 +18,44 @@
 from pathlib import Path
 
 from pyqtgraph import ViewBox
 from PySide6 import QtGui
 from PySide6.QtCore import Qt, Signal, Slot
 from PySide6.QtGui import QDesktopServices, QIcon
 from PySide6.QtWidgets import (
+    QDialog,
     QDockWidget,
     QFileDialog,
     QMainWindow,
     QMessageBox,
+    QPushButton,
+    QTextBrowser,
     QTextEdit,
+    QVBoxLayout,
 )
 
 import pyminflux.resources
 from pyminflux import __APP_NAME__, __version__
 from pyminflux.processor import MinFluxProcessor
 from pyminflux.reader import MinFluxReader
 from pyminflux.settings import Settings
 from pyminflux.state import State
 from pyminflux.ui.analyzer import Analyzer
 from pyminflux.ui.color_unmixer import ColorUnmixer
 from pyminflux.ui.dataviewer import DataViewer
 from pyminflux.ui.emittingstream import EmittingStream
+from pyminflux.ui.frc_tool import FRCTool
 from pyminflux.ui.options import Options
 from pyminflux.ui.plotter import Plotter
 from pyminflux.ui.plotter_3d import Plotter3D
 from pyminflux.ui.plotter_toolbar import PlotterToolbar
 from pyminflux.ui.time_inspector import TimeInspector
 from pyminflux.ui.ui_main_window import Ui_MainWindow
 from pyminflux.ui.wizard import WizardDialog
+from pyminflux.utils import check_for_updates
 from pyminflux.writer import MinFluxWriter
 
 
 class PyMinFluxMainWindow(QMainWindow, Ui_MainWindow):
     """
     Main application window.
     """
@@ -90,14 +96,15 @@
         # Dialogs and widgets
         self.data_viewer = None
         self.analyzer = None
         self.plotter = None
         self.plotter3D = None
         self.color_unmixer = None
         self.inspector = None
+        self.frc_tool = None
         self.options = Options()
 
         # Initialize widget and its dock
         self.wizard = WizardDialog()
         self.wizard_dock = QDockWidget("", self)
         self.wizard_dock.setAllowedAreas(Qt.LeftDockWidgetArea | Qt.RightDockWidgetArea)
         self.wizard_dock.setFeatures(
@@ -125,18 +132,15 @@
         self.ui.splitter_layout.addWidget(self.data_viewer)
         self.ui.splitter_layout.addWidget(self.txConsole)
 
         # Make sure to only show the console if requested
         self.toggle_console_visibility()
 
         # Set initial visibility and enabled states
-        self.plotter.show()
-        self.plotter_toolbar.hide()
-        self.data_viewer.show()
-        self.ui.actionExport_data.setEnabled(False)
+        self.enable_ui_components(False)
 
         # Set up signals and slots
         self.setup_conn()
 
         # Install the custom output stream
         sys.stdout = EmittingStream()
         sys.stdout.signal_textWritten.connect(self.print_to_console)
@@ -229,20 +233,22 @@
 
     def setup_conn(self):
         """Set up signals and slots."""
 
         # Menu actions
         self.ui.actionLoad.triggered.connect(self.select_and_open_data_file)
         self.ui.actionExport_data.triggered.connect(self.export_filtered_data)
+        self.ui.actionExport_stats.triggered.connect(self.export_filtered_stats)
         self.ui.actionOptions.triggered.connect(self.open_options_dialog)
         self.ui.actionQuit.triggered.connect(self.quit_application)
         self.ui.actionConsole.changed.connect(self.toggle_console_visibility)
         self.ui.actionData_viewer.changed.connect(self.toggle_dataviewer_visibility)
         self.ui.action3D_Plotter.triggered.connect(self.open_3d_plotter)
         self.ui.actionState.triggered.connect(self.print_current_state)
+        self.ui.actionEstimate_resolution.triggered.connect(self.open_frc_tool)
         self.ui.actionManual.triggered.connect(
             lambda _: QDesktopServices.openUrl(
                 "https://github.com/bsse-scf/pyMINFLUX/wiki/pyMINFLUX-user-manual"
             )
         )
         self.ui.actionWebsite.triggered.connect(
             lambda _: QDesktopServices.openUrl("https://pyminflux.ethz.ch")
@@ -256,64 +262,81 @@
             )
         )
         self.ui.actionMailing_list.triggered.connect(
             lambda _: QDesktopServices.openUrl(
                 "https://sympa.ethz.ch/sympa/subscribe/pyminflux"
             )
         )
+        self.ui.actionWhat_s_new.triggered.connect(
+            lambda _: QDesktopServices.openUrl(
+                "https://github.com/bsse-scf/pyMINFLUX/blob/master/CHANGELOG.md"
+            )
+        )
+        self.ui.actionCheck_for_updates.triggered.connect(self.check_four_updates)
         self.ui.actionAbout.triggered.connect(self.about)
 
         # Plotter toolbar
         self.plotter_toolbar.plot_requested_parameters.connect(
             self.plot_selected_parameters
         )
         self.plotter_toolbar.fluorophore_id_changed.connect(
             self.update_fluorophore_id_in_processor_and_broadcast
         )
         self.plotter_toolbar.plot_average_positions_state_changed.connect(
             self.full_update_ui
         )
 
-        # Other connections
+        # Plotter
         self.plotter.locations_selected.connect(
             self.show_selected_points_by_indices_in_dataviewer
         )
         self.plotter.locations_selected_by_range.connect(
             self.show_selected_points_by_range_in_dataviewer
         )
         self.plotter.crop_region_selected.connect(self.crop_data_by_range)
         self.plotter_toolbar.color_code_locs_changed.connect(
             self.plot_selected_parameters
         )
+
+        # Options
         self.options.weigh_avg_localization_by_eco_option_changed.connect(
             self.update_weighted_average_localization_option_and_plot
         )
+        self.options.min_num_loc_per_trace_option_changed.connect(
+            self.update_min_num_loc_per_trace
+        )
 
         # Wizard
         self.wizard.load_data_triggered.connect(self.select_and_open_data_file)
         self.wizard.reset_filters_triggered.connect(self.reset_filters_and_broadcast)
         self.wizard.open_unmixer_triggered.connect(self.open_color_unmixer)
         self.wizard.open_time_inspector_triggered.connect(self.open_inspector)
         self.wizard.open_analyzer_triggered.connect(self.open_analyzer)
         self.wizard.fluorophore_id_changed.connect(
             self.update_fluorophore_id_in_processor_and_broadcast
         )
         self.wizard.request_fluorophore_ids_reset.connect(self.reset_fluorophore_ids)
         self.wizard.wizard_filters_run.connect(self.full_update_ui)
         self.wizard.export_data_triggered.connect(self.export_filtered_data)
 
-    def enable_ui_components_on_loaded_data(self):
-        """Enable UI components."""
-        self.ui.actionExport_data.setEnabled(True)
-        self.plotter_toolbar.show()
-
-    def disable_ui_components_on_closed_data(self):
-        """Disable UI components."""
-        self.ui.actionExport_data.setEnabled(False)
-        self.plotter_toolbar.hide()
+    def enable_ui_components(self, enabled: bool):
+        """Enable/disable UI components."""
+        self.plotter.show()  # Always show
+        if enabled:
+            self.plotter_toolbar.show()
+            self.data_viewer.show()
+            self.plotter_toolbar.show()
+        else:
+            self.plotter_toolbar.hide()
+            self.data_viewer.hide()
+            self.plotter_toolbar.hide()
+        self.ui.actionExport_data.setEnabled(enabled)
+        self.ui.actionExport_data.setEnabled(enabled)
+        self.ui.actionExport_stats.setEnabled(enabled)
+        self.ui.actionEstimate_resolution.setEnabled(enabled)
 
     def full_update_ui(self):
         """
         Updates the UI completely (after a project load, for instance).
         :return:
         """
         self.plotter.clear()
@@ -371,14 +394,18 @@
                 self.inspector.close()
                 self.inspector = None
 
             if self.options is not None:
                 self.options.close()
                 self.options = None
 
+            if self.frc_tool is not None:
+                self.frc_tool.close()
+                self.frc_tool = None
+
             # Store the application settings
             if self.last_selected_path != "":
                 settings = Settings()
                 settings.instance.setValue(
                     "io/last_selected_path", str(self.last_selected_path)
                 )
 
@@ -451,24 +478,23 @@
                 filename, z_scaling_factor=self.state.z_scaling_factor
             )
 
             # Show some info
             print(minfluxreader)
 
             # Add initialize the processor with the reader
-            self.minfluxprocessor = MinFluxProcessor(minfluxreader)
+            self.minfluxprocessor = MinFluxProcessor(
+                minfluxreader, self.state.min_num_loc_per_trace
+            )
 
             # Make sure to set current value of use_weighted_localizations
             self.minfluxprocessor.use_weighted_localizations = (
                 self.state.weigh_avg_localization_by_eco
             )
 
-            # Set state properties from data
-            self.set_state_from_data()
-
             # Show the filename on the main window
             self.setWindowTitle(
                 f"{__APP_NAME__} v{__version__} - [{Path(filename).name}]"
             )
 
             # Close the Color Unmixer
             if self.color_unmixer is not None:
@@ -476,25 +502,30 @@
                 self.color_unmixer = None
 
             # Close the Temporal Inspector
             if self.inspector is not None:
                 self.inspector.close()
                 self.inspector = None
 
+            # Close the FRC Tool
+            if self.frc_tool is not None:
+                self.frc_tool.close
+                self.frc_tool = None
+
             # Update the ui
             self.full_update_ui()
 
             # Make sure to autoupdate the axis on load
             self.plotter.enableAutoRange(enable=True)
 
             # Reset the fluorophore list in the wizard
             self.wizard.set_fluorophore_list(self.minfluxprocessor.num_fluorophorses)
 
             # Enable selected ui components
-            self.enable_ui_components_on_loaded_data()
+            self.enable_ui_components(True)
 
             # Update the Analyzer
             if self.analyzer is not None:
                 self.analyzer.set_processor(self.minfluxprocessor)
                 self.analyzer.plot()
 
             # Attach the processor reference to the wizard
@@ -558,14 +589,61 @@
         else:
             QMessageBox.critical(
                 self,
                 "Error",
                 f"Could not export filtered data to {Path(filename).name}.",
             )
 
+    @Slot(None, name="export_filtered_stats")
+    def export_filtered_stats(self):
+        """Export filtered, per-trace statistics as CSV file."""
+        if (
+            self.minfluxprocessor is None
+            or len(self.minfluxprocessor.filtered_dataframe.index) == 0
+        ):
+            return
+
+        # Ask the user to pick a name
+        filename, ext = QFileDialog.getSaveFileName(
+            self,
+            "Export filtered statistics",
+            str(self.last_selected_path),
+            "Comma-separated value files (*.csv)",
+        )
+
+        # Did the user cancel?
+        if filename == "":
+            return
+
+        # Does the file name have the .csv extension?
+        if ext != "Comma-separated value files (*.csv)":
+            return
+
+        if not filename.lower().endswith(".csv"):
+            filename = Path(filename)
+            filename = filename.parent / f"{filename.stem}.csv"
+
+        # Collect stats
+        stats = self.minfluxprocessor.filtered_dataframe_stats
+        if stats is None:
+            return
+
+        # Write stats to disk
+        try:
+            stats.to_csv(filename, index=False)
+        except Exception as e:
+            QMessageBox.critical(
+                self,
+                "Error",
+                f"Could not export filtered stats to {Path(filename).name}.\n\n{str(e)}.",
+            )
+            return
+
+        print(f"Successfully exported stats for {len(stats.index)} localizations.")
+
     @Slot(None, name="print_current_state")
     def print_current_state(self):
         """Print current contents of the state machine (DEBUG)."""
         if self.txConsole.isHidden():
             self.txConsole.show()
             self.ui.actionConsole.setChecked(True)
         state_dict = self.state.asdict()
@@ -576,23 +654,61 @@
     @Slot(None, name="about")
     def about(self):
         """Show simple About dialog."""
         QMessageBox.about(
             self,
             "About",
             f"{__APP_NAME__} v{__version__}\n"
-            f'"Heidelberg"\n'
             f"\n"
             f"Copyright 2022 - {datetime.now().year}\n"
             f"Single Cell Facility\n"
             f"D-BSSE\n"
             f"ETH Zurich\n"
             f"Switzerland",
         )
 
+    @Slot(None, name="check_four_updates")
+    def check_four_updates(self):
+        """Check for application updates."""
+
+        # Check for updates
+        code, version, error = check_for_updates()
+
+        # Process the output
+        if code == -1:
+            # Something went wrong: report
+            html = f"<b>Error! {error}</b><br /><br /><br />Please make sure you are connected to the internet.<br />If this error persists, please <a href='https://github.com/bsse-scf/pyMINFLUX/issues/'>report it</a>."
+
+        elif code == 0:
+            # No new version
+            html = f"<b>Congratulations!</b><br /><br />You are running the latest version ({pyminflux.__version__}) of {pyminflux.__APP_NAME__}."
+
+        elif code == 1:
+            # Show a dialog with a link to the download page
+            html = f"<b>There is a new version ({version}) of {pyminflux.__APP_NAME__}!</b><br /><br />You can download it from the <a href='https://github.com/bsse-scf/pyMINFLUX/releases/latest'>release page</a>."
+
+        else:
+            raise ValueError("Unexpected code!")
+
+        # Show the dialog
+        dialog = QDialog()
+        dialog.setWindowTitle("Check for updates")
+        dialog.setMinimumSize(400, 180)
+        dialog.setFixedHeight(180)
+        layout = QVBoxLayout(dialog)
+        text_browser = QTextBrowser()
+        text_browser.setStyleSheet("background-color: transparent;")
+        text_browser.setOpenExternalLinks(True)
+        text_browser.insertHtml(html)
+        layout.addWidget(text_browser)
+        button = QPushButton("OK")
+        button.clicked.connect(dialog.close)
+        layout.addWidget(button)
+        dialog.exec_()
+
     @Slot(None, name="open_analyzer")
     def open_analyzer(self):
         """Initialize and open the analyzer."""
         if self.analyzer is None:
             self.analyzer = Analyzer(self.minfluxprocessor)
             self.wizard.wizard_filters_run.connect(self.analyzer.plot)
             self.request_sync_external_tools.connect(self.analyzer.plot)
@@ -641,17 +757,35 @@
         self.color_unmixer.activateWindow()
 
     @Slot(None, name="open_options_dialog")
     def open_options_dialog(self):
         """Open the options dialog."""
         if self.options is None:
             self.options = Options()
+            self.options.min_num_loc_per_trace_option_changed.connect(
+                self.update_min_num_loc_per_trace
+            )
         self.options.show()
         self.options.activateWindow()
 
+    @Slot(None, name="update_min_num_loc_per_trace")
+    def update_min_num_loc_per_trace(self):
+        if self.minfluxprocessor is not None:
+            self.minfluxprocessor.min_num_loc_per_trace = (
+                self.state.min_num_loc_per_trace
+            )
+
+    @Slot(None, name="open_frc_tool")
+    def open_frc_tool(self):
+        """Open the FRC tool."""
+        if self.frc_tool is None:
+            self.frc_tool = FRCTool(self.minfluxprocessor)
+        self.frc_tool.show()
+        self.frc_tool.activateWindow()
+
     @Slot(list, name="show_selected_points_by_indices_in_dataviewer")
     def show_selected_points_by_indices_in_dataviewer(self, points):
         """Show the data for the selected points in the dataframe viewer."""
 
         # Extract indices of the rows corresponding to the selected points
         indices = []
         for p in points:
@@ -726,21 +860,14 @@
 
         # Make sure to autoupdate the axis (on load only)
         self.plotter.getViewBox().enableAutoRange(axis=ViewBox.XYAxes, enable=True)
 
         # Signal that the external viewers and tools should be updated
         self.request_sync_external_tools.emit()
 
-    def set_state_from_data(self):
-        """Set state properties that depend on data."""
-        if self.minfluxprocessor.filtered_dataframe is not None:
-            self.state.gmm_efo_num_clusters = int(
-                self.minfluxprocessor.filtered_dataframe["dwell"].max()
-            )
-
     def update_weighted_average_localization_option_and_plot(self):
         """Update the weighted average localization option in the Processor and re-plot."""
         if self.minfluxprocessor is not None:
             self.minfluxprocessor.use_weighted_localizations = (
                 self.state.weigh_avg_localization_by_eco
             )
         self.plot_selected_parameters()
```

### Comparing `pyminflux-0.1.3/pyminflux/ui/main_window.ui` & `pyminflux-0.2.0/pyminflux/ui/main_window.ui`

 * *Files 12% similar despite different names*

#### Comparing `pyminflux-0.1.3/pyminflux/ui/main_window.ui` & `pyminflux-0.2.0/pyminflux/ui/main_window.ui`

```diff
@@ -47,14 +47,15 @@
       </property>
       <widget class="QMenu" name="menuFile">
         <property name="title">
           <string>File</string>
         </property>
         <addaction name="actionLoad"/>
         <addaction name="actionExport_data"/>
+        <addaction name="actionExport_stats"/>
         <addaction name="separator"/>
         <addaction name="actionOptions"/>
         <addaction name="separator"/>
         <addaction name="actionQuit"/>
       </widget>
       <widget class="QMenu" name="menuView">
         <property name="title">
@@ -74,18 +75,27 @@
         </property>
         <addaction name="actionManual"/>
         <addaction name="actionWebsite"/>
         <addaction name="actionCode_repository"/>
         <addaction name="actionIssues"/>
         <addaction name="actionMailing_list"/>
         <addaction name="separator"/>
+        <addaction name="actionWhat_s_new"/>
+        <addaction name="actionCheck_for_updates"/>
         <addaction name="actionAbout"/>
       </widget>
+      <widget class="QMenu" name="menuAnalysis">
+        <property name="title">
+          <string>Analysis</string>
+        </property>
+        <addaction name="actionEstimate_resolution"/>
+      </widget>
       <addaction name="menuFile"/>
       <addaction name="menuView"/>
+      <addaction name="menuAnalysis"/>
       <addaction name="menuHelp"/>
     </widget>
     <widget class="QStatusBar" name="statusbar"/>
     <action name="actionLoad">
       <property name="text">
         <string>&amp;Load data</string>
       </property>
@@ -178,11 +188,31 @@
       </property>
     </action>
     <action name="actionMailing_list">
       <property name="text">
         <string>Mailing list</string>
       </property>
     </action>
+    <action name="actionExport_stats">
+      <property name="text">
+        <string>Export stats</string>
+      </property>
+    </action>
+    <action name="actionCheck_for_updates">
+      <property name="text">
+        <string>Check for updates</string>
+      </property>
+    </action>
+    <action name="actionEstimate_resolution">
+      <property name="text">
+        <string>FRC Analyzer</string>
+      </property>
+    </action>
+    <action name="actionWhat_s_new">
+      <property name="text">
+        <string>What's new?</string>
+      </property>
+    </action>
   </widget>
   <resources/>
   <connections/>
 </ui>
```

### Comparing `pyminflux-0.1.3/pyminflux/ui/options.py` & `pyminflux-0.2.0/pyminflux/ui/options.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.3/pyminflux/ui/options.ui` & `pyminflux-0.2.0/pyminflux/ui/options.ui`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.3/pyminflux/ui/pandas_datamodel.py` & `pyminflux-0.2.0/pyminflux/ui/pandas_datamodel.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.3/pyminflux/ui/plotter.py` & `pyminflux-0.2.0/pyminflux/ui/plotter.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,22 +55,22 @@
         # Keep a reference to the scatter plot object
         self.scatter = None
 
         # ROI for localizations selection
         self.ROI = None
         self.line = None
         self.line_text = None
-        self.__roi_start_point = None
-        self.__roi_is_being_drawn = False
-        self.__line_start_point = None
-        self.__line_is_being_drawn = False
+        self._roi_start_point = None
+        self._roi_is_being_drawn = False
+        self._line_start_point = None
+        self._line_is_being_drawn = False
 
         # Keep track of last plot
-        self.__last_x_param = None
-        self.__last_y_param = None
+        self._last_x_param = None
+        self._last_y_param = None
 
     def enableAutoRange(self, enable: bool):
         """Enable/disable axes autorange."""
         self.getViewBox().enableAutoRange(axis=ViewBox.XYAxes, enable=enable)
 
     def mousePressEvent(self, ev):
         """Override mouse press event."""
@@ -84,20 +84,20 @@
             # Remove previous ROI if it exists
             if self.ROI is not None:
                 self.removeItem(self.ROI)
                 self.ROI.deleteLater()
                 self.ROI = None
 
             # Create ROI and keep track of position
-            self.__roi_is_being_drawn = True
-            self.__roi_start_point = (
+            self._roi_is_being_drawn = True
+            self._roi_start_point = (
                 self.getPlotItem().getViewBox().mapSceneToView(ev.position())
             )
             self.ROI = ROI(
-                pos=self.__roi_start_point,
+                pos=self._roi_start_point,
                 size=(0, 0),
                 resizable=False,
                 rotatable=False,
                 pen=(255, 0, 0),
             )
             self.ROI.setAcceptedMouseButtons(Qt.MouseButton.RightButton)
             self.addItem(self.ROI)
@@ -126,21 +126,21 @@
 
             if self.line_text is not None:
                 self.removeItem(self.line_text)
                 self.line_text.deleteLater()
                 self.line_text = None
 
             # Create ROI and keep track of position
-            self.__line_is_being_drawn = True
-            self.__line_start_point = (
+            self._line_is_being_drawn = True
+            self._line_start_point = (
                 self.getPlotItem().getViewBox().mapSceneToView(ev.position())
             )
             self.line = PlotCurveItem(
-                x=[self.__line_start_point.x(), self.__line_start_point.x()],
-                y=[self.__line_start_point.y(), self.__line_start_point.y()],
+                x=[self._line_start_point.x(), self._line_start_point.x()],
+                y=[self._line_start_point.y(), self._line_start_point.y()],
                 pen=mkPen(color=(255, 0, 0), width=2),
             )
             self.addItem(self.line)
             self.line.show()
 
             # Accept the event
             ev.accept()
@@ -170,53 +170,53 @@
                 super().mousePressEvent(ev)
 
     def mouseMoveEvent(self, ev):
         # Is the user drawing an ROI?
         if (
             self.scatter is not None
             and ev.buttons() == Qt.MouseButton.LeftButton
-            and self.__roi_is_being_drawn
+            and self._roi_is_being_drawn
         ):
             # Resize the ROI
             current_point = (
                 self.getPlotItem().getViewBox().mapSceneToView(ev.position())
             )
-            self.ROI.setSize(current_point - self.__roi_start_point)
+            self.ROI.setSize(current_point - self._roi_start_point)
 
             # Accept the event
             ev.accept()
 
         elif (
             self.scatter is not None
             and ev.buttons() == Qt.MouseButton.LeftButton
-            and self.__line_is_being_drawn
+            and self._line_is_being_drawn
         ):
             # Is the user drawing a line?
 
             # Resize the ROI
             current_point = (
                 self.getPlotItem().getViewBox().mapSceneToView(ev.position())
             )
             self.line.setData(
-                x=[self.__line_start_point.x(), current_point.x()],
-                y=[self.__line_start_point.y(), current_point.y()],
+                x=[self._line_start_point.x(), current_point.x()],
+                y=[self._line_start_point.y(), current_point.y()],
             )
 
             # Accept the event
             ev.accept()
         else:
             # Call the parent method
             ev.ignore()
             super().mouseMoveEvent(ev)
 
     def mouseReleaseEvent(self, ev):
         if (
             self.scatter is not None
             and ev.button() == Qt.MouseButton.LeftButton
-            and self.__roi_is_being_drawn
+            and self._roi_is_being_drawn
         ):
             # Extract the ranges
             x_range, y_range = self._get_ranges_from_roi()
 
             # Get current parameters
             x_param = self.state.x_param
             y_param = self.state.y_param
@@ -224,16 +224,16 @@
             # Update the DataViewer with current selection
             if x_range is not None and y_range is not None:
                 self.locations_selected_by_range.emit(
                     x_param, y_param, x_range, y_range
                 )
 
             # Reset flags
-            self.__roi_start_point = None
-            self.__roi_is_being_drawn = False
+            self._roi_start_point = None
+            self._roi_is_being_drawn = False
 
             # If the ROI has 0 size (when a shift-click has been used to remove a previous ROI),
             # clean it up properly.
             if (
                 np.abs(x_range[1] - x_range[0]) < 1e-4
                 or np.abs(y_range[1] - y_range[0]) < 1e-4
             ):
@@ -243,15 +243,15 @@
 
             # Accept the event
             ev.accept()
 
         elif (
             self.scatter is not None
             and ev.button() == Qt.MouseButton.LeftButton
-            and self.__line_is_being_drawn
+            and self._line_is_being_drawn
         ):
             # Display the measurement
             x_data, y_data = self.line.getData()
             center = np.array(
                 [0.5 * (x_data[0] + x_data[1]), 0.5 * (y_data[0] + y_data[1])]
             )
             delta_y = np.array(y_data[1] - y_data[0])
@@ -272,16 +272,16 @@
             else:
                 if self.line is not None:
                     self.removeItem(self.line)
                     self.line.deleteLater()
                     self.line = None
 
             # Reset flags
-            self.__line_start_point = None
-            self.__line_is_being_drawn = False
+            self._line_start_point = None
+            self._line_is_being_drawn = False
 
             # Accept the event
             ev.accept()
 
         else:
             # Call the parent method
             ev.ignore()
@@ -324,31 +324,31 @@
         self.addItem(self.scatter)
         self.setLabel("bottom", text=x_param)
         self.setLabel("left", text=y_param)
         self.showAxis("bottom")
         self.showAxis("left")
         self.setBackground("k")
 
-        if (self.__last_x_param is None or self.__last_x_param != x_param) or (
-            self.__last_y_param is None or self.__last_y_param != y_param
+        if (self._last_x_param is None or self._last_x_param != x_param) or (
+            self._last_y_param is None or self._last_y_param != y_param
         ):
             # Update range
             self.getViewBox().enableAutoRange(axis=ViewBox.XYAxes, enable=True)
 
             # Fix aspect ratio
             x_scale = (x.max() - x.min()) / (len(x) - 1)
             y_scale = (y.max() - y.min()) / (len(y) - 1)
             aspect_ratio = y_scale / x_scale
             self.getPlotItem().getViewBox().setAspectLocked(
                 lock=True, ratio=aspect_ratio
             )
 
         # Update last plotted parameters
-        self.__last_x_param = x_param
-        self.__last_y_param = y_param
+        self._last_x_param = x_param
+        self._last_y_param = y_param
 
     def crop_data_by_roi_selection(self, item):
         """Open dialog to manually set the filter ranges"""
 
         # Get the ROI bounds
         pos = self.ROI.pos()
         size = self.ROI.size()
@@ -368,15 +368,15 @@
         self.ROI.deleteLater()
         self.ROI = None
 
     def roi_moved(self):
         """Inform that the selection of localizations may have changed after the ROI was moved."""
 
         # If the ROI is being drawn now, do nothing
-        if self.__roi_is_being_drawn:
+        if self._roi_is_being_drawn:
             return
 
         # Extract the ranges
         x_range, y_range = self._get_ranges_from_roi()
 
         # Get current parameters
         x_param = self.state.x_param
```

### Comparing `pyminflux-0.1.3/pyminflux/ui/plotter_3d.py` & `pyminflux-0.2.0/pyminflux/ui/plotter_3d.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.3/pyminflux/ui/plotter_3d.ui` & `pyminflux-0.2.0/pyminflux/ui/plotter_3d.ui`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.3/pyminflux/ui/plotter_toolbar.py` & `pyminflux-0.2.0/pyminflux/ui/plotter_toolbar.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.3/pyminflux/ui/plotter_toolbar.ui` & `pyminflux-0.2.0/pyminflux/ui/plotter_toolbar.ui`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.3/pyminflux/ui/roi_ranges.py` & `pyminflux-0.2.0/pyminflux/ui/roi_ranges.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.3/pyminflux/ui/roi_ranges.ui` & `pyminflux-0.2.0/pyminflux/ui/roi_ranges.ui`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.3/pyminflux/ui/time_inspector.py` & `pyminflux-0.2.0/pyminflux/ui/time_inspector.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         self.ui = Ui_TimeInspector()
         self.ui.setupUi(self)
 
         # Initialize state
         self.state = State()
 
         # Keep a reference to the Processor
-        self._minfluxprocessor = processor
+        self.processor = processor
 
         # Constants
         self.brush = pg.mkBrush(0, 0, 0, 255)
         self.pen = pg.mkPen(None)
 
         # Keep track of the x-axis limits and the selection
         self.x_axis = None
@@ -84,16 +84,16 @@
         self.ui.main_layout.addWidget(self.plot_widget)
 
         # Add connections
         self.ui.pbPlot.clicked.connect(self.plot_selected)
         self.ui.pbAreaToggleVisibility.clicked.connect(self.toggle_region_visibility)
         self.ui.pbSelectionKeepData.clicked.connect(self.keep_time_region)
         self.ui.pbSelectionCropData.clicked.connect(self.crop_time_region)
-        self.processing_started.connect(self.change_ui_for_processing)
-        self.processing_completed.connect(self.change_ui_for_idle)
+        self.processing_started.connect(self.disable_ui_elements)
+        self.processing_completed.connect(self.enable_ui_elements)
 
         # Plot the dcr histogram
         self.plot_selected()
 
     def invalidate_cache(self):
         """Invalidate the cache."""
         self.localizations_per_unit_time_cache = None
@@ -118,18 +118,15 @@
         self.plot_selected()
 
     @Slot(None, name="plot_selected")
     def plot_selected(self):
         """Perform and plot the results of the selected analysis."""
 
         # Do we have something to plot?
-        if (
-            self._minfluxprocessor is None
-            or self._minfluxprocessor.full_dataframe is None
-        ):
+        if self.processor is None or self.processor.full_dataframe is None:
             return
 
         # Inform that processing started
         self.processing_started.emit()
 
         # It one or more charts already exists, remove them
         for item in self.plot_widget.allChildItems():
@@ -192,31 +189,31 @@
         self.processing_completed.emit()
 
     def plot_localizations_per_unit_time(self):
         """Plot number of localizations per unit time."""
 
         # Is the data cached?
         if self.localizations_per_unit_time_cache is None:
-            if len(self._minfluxprocessor.filtered_dataframe.index) == 0:
+            if len(self.processor.filtered_dataframe.index) == 0:
                 # No data to plot
                 return
 
             # Create `time_resolution_sec` bins starting at 0.0.
             bin_edges = np.arange(
                 start=0.0,
-                stop=self._minfluxprocessor.filtered_dataframe["tim"].max()
+                stop=self.processor.filtered_dataframe["tim"].max()
                 + self.time_resolution_sec,
                 step=self.time_resolution_sec,
             )
             bin_centers = bin_edges[:-1] + 0.5 * self.time_resolution_sec
             bin_width = self.time_resolution_sec
 
             # Calculate the histogram of localizations per unit time
             self.localizations_per_unit_time_cache, _ = np.histogram(
-                self._minfluxprocessor.filtered_dataframe["tim"].values,
+                self.processor.filtered_dataframe["tim"].values,
                 bins=bin_edges,
                 density=False,
             )
 
             # Cache the x range
             self.x_axis = (bin_centers - 0.5 * bin_width) / self.time_resolution_sec
 
@@ -253,32 +250,32 @@
             not std_err and self.localization_precision_per_unit_time_cache_x is None
         ) or (
             std_err and self.localization_precision_stderr_per_unit_time_cache_x is None
         ):
             # Create `time_resolution_sec` bins starting at 0.0.
             bin_edges = np.arange(
                 start=0.0,
-                stop=self._minfluxprocessor.filtered_dataframe["tim"].max()
+                stop=self.processor.filtered_dataframe["tim"].max()
                 + self.time_resolution_sec,
                 step=self.time_resolution_sec,
             )
             bin_centers = bin_edges[:-1] + 0.5 * self.time_resolution_sec
             bin_width = self.time_resolution_sec
 
             # Allocate space for the results
             x_pr = np.zeros(len(bin_edges) - 1)
             y_pr = np.zeros(len(bin_edges) - 1)
             z_pr = np.zeros(len(bin_edges) - 1)
 
             # Now process all bins
             for i in range(len(bin_edges) - 1):
                 time_range = (bin_edges[i], bin_edges[i + 1])
-                df = self._minfluxprocessor.select_by_1d_range("tim", time_range)
+                df = self.processor.select_by_1d_range("tim", time_range)
                 if len(df.index) > 0:
-                    stats = self._minfluxprocessor.calculate_statistics_on(df)
+                    stats = self.processor.calculate_statistics_on(df)
                     if std_err:
                         x_pr[i] = stats["sx"].mean() / np.sqrt(len(stats["sx"]))
                         y_pr[i] = stats["sy"].mean() / np.sqrt(len(stats["sy"]))
                         z_pr[i] = stats["sz"].mean() / np.sqrt(len(stats["sz"]))
                     else:
                         x_pr[i] = stats["sx"].mean()
                         y_pr[i] = stats["sy"].mean()
@@ -314,15 +311,15 @@
             x_pr = self.localization_precision_per_unit_time_cache_x
             y_pr = self.localization_precision_per_unit_time_cache_y
             z_pr = self.localization_precision_per_unit_time_cache_z
 
         # Get the max bin number for normalization
         n_max = np.max([x_pr.max(), y_pr.max(), z_pr.max()])
 
-        if self._minfluxprocessor.is_3d:
+        if self.processor.is_3d:
             offset = 1 / 3
             bar_width = 0.9 / 3
         else:
             offset = 1 / 2
             bar_width = 0.9 / 2
 
         # Create the sx bar charts
@@ -344,15 +341,15 @@
             brush="b",
             alpha=0.5,
             name="σy",
         )
         self.plot_widget.addItem(chart)
 
         # Create the sz bar charts if needed
-        if self._minfluxprocessor.is_3d:
+        if self.processor.is_3d:
             chart = pg.BarGraphItem(
                 x=self.x_axis + 2 * offset,
                 height=z_pr,
                 width=bar_width,
                 brush="k",
                 alpha=0.5,
                 name="σz",
@@ -419,15 +416,15 @@
         self.selection_range = (mn, mx)
 
         # Convert to seconds
         mn_s = mn * self.time_resolution_sec
         mx_s = mx * self.time_resolution_sec
 
         # Filter
-        self._minfluxprocessor.filter_by_1d_range_complement("tim", (mn_s, mx_s))
+        self.processor.filter_by_1d_range_complement("tim", (mn_s, mx_s))
 
         # Invalidate the cache
         self.invalidate_cache()
 
         # Inform that the data has been filtered
         self.dataset_time_filtered.emit()
 
@@ -444,36 +441,36 @@
         self.selection_range = (mn, mx)
 
         # Convert to seconds
         mn_s = mn * self.time_resolution_sec
         mx_s = mx * self.time_resolution_sec
 
         # Filter
-        self._minfluxprocessor.filter_by_1d_range("tim", (mn_s, mx_s))
+        self.processor.filter_by_1d_range("tim", (mn_s, mx_s))
 
         # Invalidate the cache
         self.invalidate_cache()
 
         # Inform that the data has been filtered
         self.dataset_time_filtered.emit()
 
         # Update the plot
         self.plot_selected()
 
-    def change_ui_for_processing(self):
+    def disable_ui_elements(self):
         """Disable elements and inform that a processing is ongoing."""
         self.ui.cbAnalysisSelection.setEnabled(False)
         self.ui.pbPlot.setEnabled(False)
         self.ui.lbSelectionActions.setEnabled(False)
         self.ui.pbAreaToggleVisibility.setEnabled(False)
         self.ui.pbSelectionCropData.setEnabled(False)
         self.ui.pbSelectionKeepData.setEnabled(False)
         self.repaint()
 
-    def change_ui_for_idle(self):
+    def enable_ui_elements(self):
         """Disable elements and inform that a processing is ongoing."""
         self.ui.cbAnalysisSelection.setEnabled(True)
         self.ui.pbPlot.setEnabled(True)
         self.ui.lbSelectionActions.setEnabled(True)
         self.ui.pbAreaToggleVisibility.setEnabled(True)
         self.ui.pbSelectionCropData.setEnabled(True)
         self.ui.pbSelectionKeepData.setEnabled(True)
```

### Comparing `pyminflux-0.1.3/pyminflux/ui/time_inspector.ui` & `pyminflux-0.2.0/pyminflux/ui/time_inspector.ui`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.3/pyminflux/ui/ui_analyzer.py` & `pyminflux-0.2.0/pyminflux/ui/ui_analyzer.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.3/pyminflux/ui/ui_color_unmixer.py` & `pyminflux-0.2.0/pyminflux/ui/ui_color_unmixer.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.3/pyminflux/ui/ui_main_window.py` & `pyminflux-0.2.0/pyminflux/ui/ui_main_window.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,14 +89,22 @@
         self.actionWebsite.setObjectName("actionWebsite")
         self.actionCode_repository = QAction(MainWindow)
         self.actionCode_repository.setObjectName("actionCode_repository")
         self.actionIssues = QAction(MainWindow)
         self.actionIssues.setObjectName("actionIssues")
         self.actionMailing_list = QAction(MainWindow)
         self.actionMailing_list.setObjectName("actionMailing_list")
+        self.actionExport_stats = QAction(MainWindow)
+        self.actionExport_stats.setObjectName("actionExport_stats")
+        self.actionCheck_for_updates = QAction(MainWindow)
+        self.actionCheck_for_updates.setObjectName("actionCheck_for_updates")
+        self.actionEstimate_resolution = QAction(MainWindow)
+        self.actionEstimate_resolution.setObjectName("actionEstimate_resolution")
+        self.actionWhat_s_new = QAction(MainWindow)
+        self.actionWhat_s_new.setObjectName("actionWhat_s_new")
         self.centralwidget = QWidget(MainWindow)
         self.centralwidget.setObjectName("centralwidget")
         self.gridLayout = QGridLayout(self.centralwidget)
         self.gridLayout.setObjectName("gridLayout")
         self.splitter_layout = QSplitter(self.centralwidget)
         self.splitter_layout.setObjectName("splitter_layout")
         self.splitter_layout.setMaximumSize(QSize(16777215, 16777215))
@@ -110,24 +118,28 @@
         self.menubar.setGeometry(QRect(0, 0, 1000, 23))
         self.menuFile = QMenu(self.menubar)
         self.menuFile.setObjectName("menuFile")
         self.menuView = QMenu(self.menubar)
         self.menuView.setObjectName("menuView")
         self.menuHelp = QMenu(self.menubar)
         self.menuHelp.setObjectName("menuHelp")
+        self.menuAnalysis = QMenu(self.menubar)
+        self.menuAnalysis.setObjectName("menuAnalysis")
         MainWindow.setMenuBar(self.menubar)
         self.statusbar = QStatusBar(MainWindow)
         self.statusbar.setObjectName("statusbar")
         MainWindow.setStatusBar(self.statusbar)
 
         self.menubar.addAction(self.menuFile.menuAction())
         self.menubar.addAction(self.menuView.menuAction())
+        self.menubar.addAction(self.menuAnalysis.menuAction())
         self.menubar.addAction(self.menuHelp.menuAction())
         self.menuFile.addAction(self.actionLoad)
         self.menuFile.addAction(self.actionExport_data)
+        self.menuFile.addAction(self.actionExport_stats)
         self.menuFile.addSeparator()
         self.menuFile.addAction(self.actionOptions)
         self.menuFile.addSeparator()
         self.menuFile.addAction(self.actionQuit)
         self.menuView.addAction(self.actionData_viewer)
         self.menuView.addAction(self.actionConsole)
         self.menuView.addSeparator()
@@ -137,15 +149,18 @@
         self.menuView.addAction(self.actionState)
         self.menuHelp.addAction(self.actionManual)
         self.menuHelp.addAction(self.actionWebsite)
         self.menuHelp.addAction(self.actionCode_repository)
         self.menuHelp.addAction(self.actionIssues)
         self.menuHelp.addAction(self.actionMailing_list)
         self.menuHelp.addSeparator()
+        self.menuHelp.addAction(self.actionWhat_s_new)
+        self.menuHelp.addAction(self.actionCheck_for_updates)
         self.menuHelp.addAction(self.actionAbout)
+        self.menuAnalysis.addAction(self.actionEstimate_resolution)
 
         self.retranslateUi(MainWindow)
 
         QMetaObject.connectSlotsByName(MainWindow)
 
     # setupUi
 
@@ -209,12 +224,27 @@
         )
         self.actionIssues.setText(
             QCoreApplication.translate("MainWindow", "Issues", None)
         )
         self.actionMailing_list.setText(
             QCoreApplication.translate("MainWindow", "Mailing list", None)
         )
+        self.actionExport_stats.setText(
+            QCoreApplication.translate("MainWindow", "Export stats", None)
+        )
+        self.actionCheck_for_updates.setText(
+            QCoreApplication.translate("MainWindow", "Check for updates", None)
+        )
+        self.actionEstimate_resolution.setText(
+            QCoreApplication.translate("MainWindow", "FRC Analyzer", None)
+        )
+        self.actionWhat_s_new.setText(
+            QCoreApplication.translate("MainWindow", "What's new?", None)
+        )
         self.menuFile.setTitle(QCoreApplication.translate("MainWindow", "File", None))
         self.menuView.setTitle(QCoreApplication.translate("MainWindow", "View", None))
         self.menuHelp.setTitle(QCoreApplication.translate("MainWindow", "Help", None))
+        self.menuAnalysis.setTitle(
+            QCoreApplication.translate("MainWindow", "Analysis", None)
+        )
 
     # retranslateUi
```

### Comparing `pyminflux-0.1.3/pyminflux/ui/ui_options.py` & `pyminflux-0.2.0/pyminflux/ui/ui_options.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.3/pyminflux/ui/ui_plotter_3d.py` & `pyminflux-0.2.0/pyminflux/ui/ui_plotter_3d.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.3/pyminflux/ui/ui_plotter_toolbar.py` & `pyminflux-0.2.0/pyminflux/ui/ui_plotter_toolbar.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.3/pyminflux/ui/ui_roi_ranges.py` & `pyminflux-0.2.0/pyminflux/ui/ui_roi_ranges.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.3/pyminflux/ui/ui_time_inspector.py` & `pyminflux-0.2.0/pyminflux/ui/ui_time_inspector.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.3/pyminflux/ui/ui_wizard.py` & `pyminflux-0.2.0/pyminflux/ui/ui_wizard.py`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.3/pyminflux/ui/wizard.ui` & `pyminflux-0.2.0/pyminflux/ui/wizard.ui`

 * *Files identical despite different names*

### Comparing `pyminflux-0.1.3/pyminflux/utils/__init__.py` & `pyminflux-0.2.0/pyminflux/writer/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,8 +9,13 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 
-from ._utils import calculate_common_bins, print_summary_statistics
+__doc__ = "Writer of processed MINFLUX data."
+__all__ = [
+    "MinFluxWriter",
+]
+
+from ._writer import MinFluxWriter
```

### Comparing `pyminflux-0.1.3/pyminflux/writer/__init__.py` & `pyminflux-0.2.0/pyminflux/reader/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,8 +9,13 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 
-from ._writer import MinFluxWriter
+__doc__ = "Reader of MINFLUX data."
+__all__ = [
+    "MinFluxReader",
+]
+
+from ._reader import MinFluxReader
```

### Comparing `pyminflux-0.1.3/pyminflux/writer/_writer.py` & `pyminflux-0.2.0/pyminflux/writer/_writer.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 
 import numpy as np
 
 from pyminflux.processor import MinFluxProcessor
 
 
 class MinFluxWriter:
+    __docs__ = "Writer of processed MINFLUX data tp `.npy` or `.csv` formats."
+
     @staticmethod
     def write_npy(processor: MinFluxProcessor, file_name: Union[Path, str]) -> bool:
         """Write an Imspector-compatible NumPy structured array."""
 
         # Get the raw data
         filtered_array = processor.filtered_numpy_array
         if filtered_array is None:
```

### Comparing `pyminflux-0.1.3/pyproject.toml` & `pyminflux-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyminflux"
-version = "0.1.3"
+version = "0.2.0"
 description = "Reader, processor, and viewer of MINFLUX raw data."
 authors = ["Aaron Ponti <aaron.ponti@bsse.ethz.ch>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/bsse-scf/pyMINFLUX"
 documentation = "https://github.com/bsse-scf/pyMINFLUX/wiki"
 keywords = ["MINFLUX", "Visualization", "Filtering", "Analysis", "Python"]
@@ -46,32 +46,34 @@
 py_version = 310
 multi_line_output = 3
 include_trailing_comma = true
 force_grid_wrap = 0
 use_parentheses = true
 line_length = 88
 combine_as_imports = true
-known_third_party = ["PySide6", "numpy", "pandas", "pyqtgraph", "pytest", "scipy", "sklearn"]
+known_third_party = ["PySide6", "numpy", "pandas", "pyqtgraph", "pytest", "requests", "scipy", "sklearn"]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
 numpy = "^1.23.4"
 pandas = "^1.5.1"
 pyside6 = ">=6.4.0.1,<6.5"
 pyqtgraph = "^0.13.2"
 scipy = "^1.9.3"
 pyopengl = "^3.1.6"
 scikit-learn = "^1.2.0"
+requests = "^2.31.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 ordered-set = "^4.1.0"
 pytest-cov = "^4.0.0"
 pre-commit = "^3.1.1"
 pyinstaller = "5.10.1"
+pdoc3 = "^0.10.0"
 
 [tool.poetry.scripts]
 pyminflux = "pyminflux.main:main"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pyminflux-0.1.3/PKG-INFO` & `pyminflux-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyminflux
-Version: 0.1.3
+Version: 0.2.0
 Summary: Reader, processor, and viewer of MINFLUX raw data.
 Home-page: https://github.com/bsse-scf/pyMINFLUX
 License: Apache-2.0
 Keywords: MINFLUX,Visualization,Filtering,Analysis,Python
 Author: Aaron Ponti
 Author-email: aaron.ponti@bsse.ethz.ch
 Requires-Python: >=3.10,<3.12
@@ -21,27 +21,28 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: numpy (>=1.23.4,<2.0.0)
 Requires-Dist: pandas (>=1.5.1,<2.0.0)
 Requires-Dist: pyopengl (>=3.1.6,<4.0.0)
 Requires-Dist: pyqtgraph (>=0.13.2,<0.14.0)
 Requires-Dist: pyside6 (>=6.4.0.1,<6.5)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: scikit-learn (>=1.2.0,<2.0.0)
 Requires-Dist: scipy (>=1.9.3,<2.0.0)
 Project-URL: Bug Tracker, https://github.com/bsse-scf/pyMINFLUX/issues
 Project-URL: Documentation, https://github.com/bsse-scf/pyMINFLUX/wiki
 Project-URL: Repository, https://github.com/bsse-scf/pyMINFLUX
 Description-Content-Type: text/markdown
 
 # ![](pyminflux/ui/assets/Logo_v3_small.png)&nbsp;&nbsp;&nbsp;pyMINFLUX
 
 Reader, analyzer, and viewer of MINFLUX raw data.
 
 <p align="center">
-  <img width="460" src="https://pyminflux.ethz.ch/img/pyminflux.png">
+  <img width="800" src="https://pyminflux.ethz.ch/img/pyminflux.png">
 </p>
 
 ## Installation
 
 ### Apps
 
 Compiled executables (apps) for Linux, macOS and Windows can be downloaded from the [release page](https://github.com/bsse-scf/pyMINFLUX/releases/latest). 
@@ -87,21 +88,26 @@
 $ conda activate pyminflux-env
 $ git clone https://github.com/bsse-scf/pyMINFLUX /path/to/pyminflux
 $ cd /path/to/pyminflux
 $ conda install pyopengl       # This is specific to macOS
 $ python -m pip install -e .
 ```
 
-### Running pyMinFlux from console
+### Running pyMINFLUX from console
 
 ```sh
 $ cd /path/to/pyminflux
-$ python pyminflux/main.py
+$ python pyminflux/main.py  # As a Python script, or
+$ pyminflux                 # as a standalone tool
 ```
 
+### Using the pyMINFLUX API from Python scripts or Jupyter Notebooks
+
+The graphical user interface is not the only way to use pyMINFLUX. Indeed, the pyMINFLUX core library can be integrated in Python scripts or Jupyter Notebooks. The documentation for the pyMIMFLUX core API can be found on [https://pyminflux.ethz.ch/api/pyminflux/](https://pyminflux.ethz.ch/api/pyminflux/); an example Jupyter Notebook is [bundled with the code](/examples/processing.ipynb).
+
 ## User manual
 
 The user manual is hosted in the [project wiki](https://github.com/bsse-scf/pyMINFLUX/wiki/pyMINFLUX-user-manual).
 
 ## Official website
 
 The official pyMINFLUX website is on https://pyminflux.ethz.ch.
```

