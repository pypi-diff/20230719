# Comparing `tmp/wbpUFO-0.2.1.tar.gz` & `tmp/wbpUFO-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wbpUFO-0.2.1.tar", last modified: Fri Jul 14 10:14:36 2023, max compression
+gzip compressed data, was "wbpUFO-0.2.2.tar", last modified: Wed Jul 19 14:25:21 2023, max compression
```

## Comparing `wbpUFO-0.2.1.tar` & `wbpUFO-0.2.2.tar`

### file list

```diff
@@ -1,166 +1,167 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:14:36.960619 wbpUFO-0.2.1/
--rw-rw-rw-   0 root         (0) root         (0)     1080 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:14:36.930619 wbpUFO-0.2.1/Lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:14:36.934619 wbpUFO-0.2.1/Lib/wbpUFO/
--rw-rw-rw-   0 root         (0) root         (0)    10601 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3025 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:14:36.938619 wbpUFO-0.2.1/Lib/wbpUFO/control/
--rw-rw-rw-   0 root         (0) root         (0)     1290 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/control/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1306 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/control/dialogItemPicker.py
--rw-rw-rw-   0 root         (0) root         (0)     1717 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/control/dialogItemPickerUI.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/control/findGlyphListCtrl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:14:36.939619 wbpUFO-0.2.1/Lib/wbpUFO/control/glyphEditor/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/control/glyphEditor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    23844 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/control/glyphEditor/canvas.py
--rw-rw-rw-   0 root         (0) root         (0)    20703 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/control/glyphEditor/cursor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:14:36.940619 wbpUFO-0.2.1/Lib/wbpUFO/control/glyphEditor/drawing/
--rw-rw-rw-   0 root         (0) root         (0)      140 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/control/glyphEditor/drawing/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8107 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/control/glyphEditor/drawing/base.py
--rw-rw-rw-   0 root         (0) root         (0)     3403 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/control/glyphEditor/drawing/font.py
--rw-rw-rw-   0 root         (0) root         (0)    27766 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/control/glyphEditor/drawing/glyph.py
--rw-rw-rw-   0 root         (0) root         (0)     5602 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/control/glyphEditor/editPanel.py
--rw-rw-rw-   0 root         (0) root         (0)    21569 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/control/glyphEditor/menu.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:14:36.943619 wbpUFO-0.2.1/Lib/wbpUFO/control/glyphEditor/tool/
--rw-rw-rw-   0 root         (0) root         (0)      512 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/control/glyphEditor/tool/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2399 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/control/glyphEditor/tool/addellipse.py
--rw-rw-rw-   0 root         (0) root         (0)     1507 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/control/glyphEditor/tool/addrectangle.py
--rw-rw-rw-   0 root         (0) root         (0)    13199 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/control/glyphEditor/tool/base.py
--rw-rw-rw-   0 root         (0) root         (0)     2079 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/control/glyphEditor/tool/magicwand.py
--rw-rw-rw-   0 root         (0) root         (0)     2953 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/control/glyphEditor/tool/tooldraw.py
--rw-rw-rw-   0 root         (0) root         (0)    16709 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/control/glyphEditor/tool/tooledit.py
--rw-rw-rw-   0 root         (0) root         (0)     3421 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/control/glyphEditor/tool/toolerase.py
--rw-rw-rw-   0 root         (0) root         (0)     7101 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/control/glyphEditor/tool/toolknife.py
--rw-rw-rw-   0 root         (0) root         (0)     5302 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/control/glyphEditor/tool/toolmeter.py
--rw-rw-rw-   0 root         (0) root         (0)      556 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/control/glyphEditor/tool/toolpan.py
--rw-rw-rw-   0 root         (0) root         (0)     1691 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/control/glyphEditor/tool/toolreverse.py
--rw-rw-rw-   0 root         (0) root         (0)     1848 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/control/glyphEditor/tool/toolrotate.py
--rw-rw-rw-   0 root         (0) root         (0)     2538 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/control/glyphEditor/tool/toolscale.py
--rw-rw-rw-   0 root         (0) root         (0)     1852 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/control/glyphEditor/tool/toolstartpoint.py
--rw-rw-rw-   0 root         (0) root         (0)     2756 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/control/glyphEditor/tool/toolzoom.py
--rw-rw-rw-   0 root         (0) root         (0)     4094 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/control/glyphGridStatusPanelUI.py
--rw-rw-rw-   0 root         (0) root         (0)     5122 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/control/kerningViewCanvas.py
--rw-rw-rw-   0 root         (0) root         (0)     3381 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/control/kerningViewPanelUI.py
--rw-rw-rw-   0 root         (0) root         (0)     5038 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/control/libControl.py
--rw-rw-rw-   0 root         (0) root         (0)     2798 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/control/panelItemPicker.py
--rw-rw-rw-   0 root         (0) root         (0)     5686 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/control/panelItemPickerUI.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:14:36.948619 wbpUFO-0.2.1/Lib/wbpUFO/dialog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/dialog/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1292 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/dialog/anchorDialog.py
--rw-rw-rw-   0 root         (0) root         (0)     4887 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/dialog/anchorDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)     1207 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/dialog/applyGlyphConstructionDialog.py
--rw-rw-rw-   0 root         (0) root         (0)     4147 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/dialog/applyGlyphConstructionDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)     3351 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/dialog/assignLayerDialog.py
--rw-rw-rw-   0 root         (0) root         (0)     6012 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/dialog/assignLayerDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)     1734 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/dialog/componentDialog.py
--rw-rw-rw-   0 root         (0) root         (0)     4425 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/dialog/componentDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)      573 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/dialog/deleteGlyphsDialog.py
--rw-rw-rw-   0 root         (0) root         (0)     2839 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/dialog/deleteGlyphsDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)     6084 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/dialog/findGlyphDialog.py
--rw-rw-rw-   0 root         (0) root         (0)     5036 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/dialog/findGlyphDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)      820 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/dialog/generateOTCFFoptionsDialog.py
--rw-rw-rw-   0 root         (0) root         (0)     3899 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/dialog/generateOTCFFoptionsDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)     1445 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/dialog/guidelineDialog.py
--rw-rw-rw-   0 root         (0) root         (0)     5816 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/dialog/guidelineDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)     1244 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/dialog/layerDialog.py
--rw-rw-rw-   0 root         (0) root         (0)     2511 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/dialog/layerDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)      441 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/dialog/newFontDialog.py
--rw-rw-rw-   0 root         (0) root         (0)     2797 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/dialog/newFontDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)     1957 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/dialog/newGlyphDialog.py
--rw-rw-rw-   0 root         (0) root         (0)     2355 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/dialog/newGlyphDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)     8386 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/dialog/renameGlyphDialog.py
--rw-rw-rw-   0 root         (0) root         (0)     9608 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/dialog/renameGlyphDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)     5367 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/dialog/revertFontDialog.py
--rw-rw-rw-   0 root         (0) root         (0)     7261 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/dialog/revertFontDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)     1549 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/dialog/selectFontsDialog.py
--rw-rw-rw-   0 root         (0) root         (0)     1967 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/dialog/selectFontsDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)    19455 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/document.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:14:36.950619 wbpUFO-0.2.1/Lib/wbpUFO/glyphCommand/
--rw-rw-rw-   0 root         (0) root         (0)     3040 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/glyphCommand/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1773 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/glyphCommand/anchor.py
--rw-rw-rw-   0 root         (0) root         (0)     4404 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/glyphCommand/base.py
--rw-rw-rw-   0 root         (0) root         (0)      957 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/glyphCommand/commandListCtrl.py
--rw-rw-rw-   0 root         (0) root         (0)    13260 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/glyphCommand/commandListDialog.py
--rw-rw-rw-   0 root         (0) root         (0)    12967 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/glyphCommand/commandListDialogUI.py
--rw-rw-rw-   0 root         (0) root         (0)     1770 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/glyphCommand/composite.py
--rw-rw-rw-   0 root         (0) root         (0)     4328 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/glyphCommand/contour.py
--rw-rw-rw-   0 root         (0) root         (0)     2070 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/glyphCommand/guideline.py
--rw-rw-rw-   0 root         (0) root         (0)     3274 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/glyphCommand/layer.py
--rw-rw-rw-   0 root         (0) root         (0)     7342 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/glyphCommand/metric.py
--rw-rw-rw-   0 root         (0) root         (0)     1685 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/glyphCommand/misc.py
--rw-rw-rw-   0 root         (0) root         (0)     5157 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/glyphCommand/parameter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:14:36.951619 wbpUFO-0.2.1/Lib/wbpUFO/panel/
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/panel/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16132 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/panel/glyphViewCanvas.py
--rw-rw-rw-   0 root         (0) root         (0)     2147 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/panel/glyphViewPanel.py
--rw-rw-rw-   0 root         (0) root         (0)     3718 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/panel/glyphViewPanelUI.py
--rw-rw-rw-   0 root         (0) root         (0)     3899 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:14:36.952619 wbpUFO-0.2.1/Lib/wbpUFO/toolbar/
--rw-rw-rw-   0 root         (0) root         (0)     1473 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/toolbar/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5259 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/toolbar/command.py
--rw-rw-rw-   0 root         (0) root         (0)     4790 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/toolbar/editTool.py
--rw-rw-rw-   0 root         (0) root         (0)     4628 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/toolbar/glyphLock.py
--rw-rw-rw-   0 root         (0) root         (0)     7625 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/toolbar/glyphShow.py
--rw-rw-rw-   0 root         (0) root         (0)    12968 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/toolbar/layer.py
--rw-rw-rw-   0 root         (0) root         (0)     4501 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/toolbar/markColor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:14:36.952619 wbpUFO-0.2.1/Lib/wbpUFO/view/
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/view/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:14:36.960619 wbpUFO-0.2.1/Lib/wbpUFO/view/font/
--rw-rw-rw-   0 root         (0) root         (0)     6921 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/view/font/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    19362 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/view/font/feature.py
--rw-rw-rw-   0 root         (0) root         (0)      529 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/view/font/fontInfoCaret.py
--rw-rw-rw-   0 root         (0) root         (0)     6071 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/view/font/fontInfoCaretUI.py
--rw-rw-rw-   0 root         (0) root         (0)      573 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/view/font/fontInfoClassification.py
--rw-rw-rw-   0 root         (0) root         (0)     4097 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/view/font/fontInfoClassificationUI.py
--rw-rw-rw-   0 root         (0) root         (0)      544 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/view/font/fontInfoCodepage.py
--rw-rw-rw-   0 root         (0) root         (0)     2493 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/view/font/fontInfoCodepageUI.py
--rw-rw-rw-   0 root         (0) root         (0)     8635 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/view/font/fontInfoControl.py
--rw-rw-rw-   0 root         (0) root         (0)      549 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/view/font/fontInfoEmbedding.py
--rw-rw-rw-   0 root         (0) root         (0)     3971 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/view/font/fontInfoEmbeddingUI.py
--rw-rw-rw-   0 root         (0) root         (0)      544 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/view/font/fontInfoEncoding.py
--rw-rw-rw-   0 root         (0) root         (0)     4222 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/view/font/fontInfoEncodingUI.py
--rw-rw-rw-   0 root         (0) root         (0)      539 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/view/font/fontInfoHinting.py
--rw-rw-rw-   0 root         (0) root         (0)     1749 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/view/font/fontInfoHintingPS.py
--rw-rw-rw-   0 root         (0) root         (0)    10760 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/view/font/fontInfoHintingPSUI.py
--rw-rw-rw-   0 root         (0) root         (0)     6861 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/view/font/fontInfoHintingUI.py
--rw-rw-rw-   0 root         (0) root         (0)      574 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/view/font/fontInfoIdentification.py
--rw-rw-rw-   0 root         (0) root         (0)     6677 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/view/font/fontInfoIdentificationUI.py
--rw-rw-rw-   0 root         (0) root         (0)      529 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/view/font/fontInfoLegal.py
--rw-rw-rw-   0 root         (0) root         (0)     7003 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/view/font/fontInfoLegalUI.py
--rw-rw-rw-   0 root         (0) root         (0)      524 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/view/font/fontInfoLine.py
--rw-rw-rw-   0 root         (0) root         (0)     4896 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/view/font/fontInfoLineUI.py
--rw-rw-rw-   0 root         (0) root         (0)      534 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/view/font/fontInfoMetric.py
--rw-rw-rw-   0 root         (0) root         (0)    13262 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/view/font/fontInfoMetricUI.py
--rw-rw-rw-   0 root         (0) root         (0)      524 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/view/font/fontInfoName.py
--rw-rw-rw-   0 root         (0) root         (0)    13781 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/view/font/fontInfoNameUI.py
--rw-rw-rw-   0 root         (0) root         (0)     2726 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/view/font/fontInfoNaviagtionPanelUI.py
--rw-rw-rw-   0 root         (0) root         (0)      524 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/view/font/fontInfoNote.py
--rw-rw-rw-   0 root         (0) root         (0)     1772 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/view/font/fontInfoNoteUI.py
--rw-rw-rw-   0 root         (0) root         (0)      574 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/view/font/fontInfoSuperSubscript.py
--rw-rw-rw-   0 root         (0) root         (0)     7229 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/view/font/fontInfoSuperSubscriptUI.py
--rw-rw-rw-   0 root         (0) root         (0)      539 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/view/font/fontInfoUnicode.py
--rw-rw-rw-   0 root         (0) root         (0)     2488 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/view/font/fontInfoUnicodeUI.py
--rw-rw-rw-   0 root         (0) root         (0)    11903 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/view/font/fontInfoValidator.py
--rw-rw-rw-   0 root         (0) root         (0)    42068 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/view/font/glyphGrid.py
--rw-rw-rw-   0 root         (0) root         (0)    13651 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/view/font/groups.py
--rw-rw-rw-   0 root         (0) root         (0)     3788 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/view/font/groupsStatusPanelUI.py
--rw-rw-rw-   0 root         (0) root         (0)     3140 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/view/font/hintPSlistCtrl.py
--rw-rw-rw-   0 root         (0) root         (0)     7097 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/view/font/hintPSpanel.py
--rw-rw-rw-   0 root         (0) root         (0)    16125 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/view/font/info.py
--rw-rw-rw-   0 root         (0) root         (0)     7085 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/view/font/kerning.py
--rw-rw-rw-   0 root         (0) root         (0)     2885 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/view/font/kerningStatusPanelUI.py
--rw-rw-rw-   0 root         (0) root         (0)     4342 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/view/font/stemPanelUI.py
--rw-rw-rw-   0 root         (0) root         (0)     4950 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/view/font/zonePanelUI.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:14:36.960619 wbpUFO-0.2.1/Lib/wbpUFO/view/fontinfo/
--rw-rw-rw-   0 root         (0) root         (0)     7067 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/view/fontinfo/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4794 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/Lib/wbpUFO/view/glyph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 10:14:36.936619 wbpUFO-0.2.1/Lib/wbpUFO.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2211 2023-07-14 10:14:36.000000 wbpUFO-0.2.1/Lib/wbpUFO.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5788 2023-07-14 10:14:36.000000 wbpUFO-0.2.1/Lib/wbpUFO.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 10:14:36.000000 wbpUFO-0.2.1/Lib/wbpUFO.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-14 10:14:36.000000 wbpUFO-0.2.1/Lib/wbpUFO.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-07-14 10:14:36.000000 wbpUFO-0.2.1/Lib/wbpUFO.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-14 10:14:36.000000 wbpUFO-0.2.1/Lib/wbpUFO.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2211 2023-07-14 10:14:36.960619 wbpUFO-0.2.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      635 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2221 2023-07-14 10:14:36.961619 wbpUFO-0.2.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-07-14 10:14:35.000000 wbpUFO-0.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:25:21.379218 wbpUFO-0.2.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1080 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:25:21.355219 wbpUFO-0.2.2/Lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:25:21.357219 wbpUFO-0.2.2/Lib/wbpUFO/
+-rw-rw-rw-   0 root         (0) root         (0)    10601 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3025 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:25:21.360219 wbpUFO-0.2.2/Lib/wbpUFO/control/
+-rw-rw-rw-   0 root         (0) root         (0)     1290 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1306 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/dialogItemPicker.py
+-rw-rw-rw-   0 root         (0) root         (0)     1717 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/dialogItemPickerUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/findGlyphListCtrl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:25:21.361219 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-19 14:25:20.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    24105 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/canvas.py
+-rw-rw-rw-   0 root         (0) root         (0)    20703 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/cursor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:25:21.361219 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/drawing/
+-rw-rw-rw-   0 root         (0) root         (0)      140 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/drawing/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8393 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/drawing/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3460 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/drawing/font.py
+-rw-rw-rw-   0 root         (0) root         (0)    28062 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/drawing/glyph.py
+-rw-rw-rw-   0 root         (0) root         (0)     5602 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/editPanel.py
+-rw-rw-rw-   0 root         (0) root         (0)    21609 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/menu.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:25:21.364219 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/
+-rw-rw-rw-   0 root         (0) root         (0)      512 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2399 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/addellipse.py
+-rw-rw-rw-   0 root         (0) root         (0)     1507 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/addrectangle.py
+-rw-rw-rw-   0 root         (0) root         (0)    13199 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2079 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/magicwand.py
+-rw-rw-rw-   0 root         (0) root         (0)     2953 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/tooldraw.py
+-rw-rw-rw-   0 root         (0) root         (0)    16709 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/tooledit.py
+-rw-rw-rw-   0 root         (0) root         (0)     3421 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/toolerase.py
+-rw-rw-rw-   0 root         (0) root         (0)     7101 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/toolknife.py
+-rw-rw-rw-   0 root         (0) root         (0)     5302 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/toolmeter.py
+-rw-rw-rw-   0 root         (0) root         (0)      556 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/toolpan.py
+-rw-rw-rw-   0 root         (0) root         (0)     1691 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/toolreverse.py
+-rw-rw-rw-   0 root         (0) root         (0)     1848 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/toolrotate.py
+-rw-rw-rw-   0 root         (0) root         (0)     2538 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/toolscale.py
+-rw-rw-rw-   0 root         (0) root         (0)     1852 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/toolstartpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     2756 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/toolzoom.py
+-rw-rw-rw-   0 root         (0) root         (0)     4094 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/glyphGridStatusPanelUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     5122 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/kerningViewCanvas.py
+-rw-rw-rw-   0 root         (0) root         (0)     3381 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/kerningViewPanelUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     5038 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/libControl.py
+-rw-rw-rw-   0 root         (0) root         (0)     2798 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/panelItemPicker.py
+-rw-rw-rw-   0 root         (0) root         (0)     5686 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/control/panelItemPickerUI.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:25:21.368219 wbpUFO-0.2.2/Lib/wbpUFO/dialog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-19 14:25:20.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1292 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/anchorDialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     4887 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/anchorDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     1207 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/applyGlyphConstructionDialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     4147 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/applyGlyphConstructionDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     3351 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/assignLayerDialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     6012 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/assignLayerDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     1734 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/componentDialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     4425 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/componentDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)      573 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/deleteGlyphsDialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     2839 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/deleteGlyphsDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     6084 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/findGlyphDialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     5036 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/findGlyphDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)      820 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/generateOTCFFoptionsDialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     3899 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/generateOTCFFoptionsDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     1445 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/guidelineDialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     5816 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/guidelineDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     1244 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/layerDialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     2511 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/layerDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)      441 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/newFontDialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     2797 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/newFontDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     1957 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/newGlyphDialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     2355 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/newGlyphDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     8386 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/renameGlyphDialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     9608 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/renameGlyphDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     5367 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/revertFontDialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     7261 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/revertFontDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     1549 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/selectFontsDialog.py
+-rw-rw-rw-   0 root         (0) root         (0)     1967 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/dialog/selectFontsDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)    19544 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/document.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:25:21.370219 wbpUFO-0.2.2/Lib/wbpUFO/glyphCommand/
+-rw-rw-rw-   0 root         (0) root         (0)     3040 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/glyphCommand/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1773 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/glyphCommand/anchor.py
+-rw-rw-rw-   0 root         (0) root         (0)     4404 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/glyphCommand/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      957 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/glyphCommand/commandListCtrl.py
+-rw-rw-rw-   0 root         (0) root         (0)    13260 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/glyphCommand/commandListDialog.py
+-rw-rw-rw-   0 root         (0) root         (0)    12967 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/glyphCommand/commandListDialogUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     1770 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/glyphCommand/composite.py
+-rw-rw-rw-   0 root         (0) root         (0)     4328 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/glyphCommand/contour.py
+-rw-rw-rw-   0 root         (0) root         (0)     2070 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/glyphCommand/guideline.py
+-rw-rw-rw-   0 root         (0) root         (0)     3274 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/glyphCommand/layer.py
+-rw-rw-rw-   0 root         (0) root         (0)     7342 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/glyphCommand/metric.py
+-rw-rw-rw-   0 root         (0) root         (0)     1685 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/glyphCommand/misc.py
+-rw-rw-rw-   0 root         (0) root         (0)     5157 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/glyphCommand/parameter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:25:21.370219 wbpUFO-0.2.2/Lib/wbpUFO/panel/
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/panel/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16132 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/panel/glyphViewCanvas.py
+-rw-rw-rw-   0 root         (0) root         (0)     2162 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/panel/glyphViewPanel.py
+-rw-rw-rw-   0 root         (0) root         (0)     3718 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/panel/glyphViewPanelUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     3899 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:25:21.371219 wbpUFO-0.2.2/Lib/wbpUFO/toolbar/
+-rw-rw-rw-   0 root         (0) root         (0)     1980 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/toolbar/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5259 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/toolbar/command.py
+-rw-rw-rw-   0 root         (0) root         (0)     4790 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/toolbar/editTool.py
+-rw-rw-rw-   0 root         (0) root         (0)     4521 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/toolbar/glyphLock.py
+-rw-rw-rw-   0 root         (0) root         (0)     7625 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/toolbar/glyphShow.py
+-rw-rw-rw-   0 root         (0) root         (0)    12968 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/toolbar/layer.py
+-rw-rw-rw-   0 root         (0) root         (0)     4501 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/toolbar/markColor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:25:21.372218 wbpUFO-0.2.2/Lib/wbpUFO/view/
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:25:21.379218 wbpUFO-0.2.2/Lib/wbpUFO/view/font/
+-rw-rw-rw-   0 root         (0) root         (0)     5480 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    19462 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/feature.py
+-rw-rw-rw-   0 root         (0) root         (0)      735 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoBase.py
+-rw-rw-rw-   0 root         (0) root         (0)      241 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoCaret.py
+-rw-rw-rw-   0 root         (0) root         (0)     6034 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoCaretUI.py
+-rw-rw-rw-   0 root         (0) root         (0)      295 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoClassification.py
+-rw-rw-rw-   0 root         (0) root         (0)     4073 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoClassificationUI.py
+-rw-rw-rw-   0 root         (0) root         (0)      259 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoCodepage.py
+-rw-rw-rw-   0 root         (0) root         (0)     2539 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoCodepageUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     8952 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoControl.py
+-rw-rw-rw-   0 root         (0) root         (0)      265 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoEmbedding.py
+-rw-rw-rw-   0 root         (0) root         (0)     3938 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoEmbeddingUI.py
+-rw-rw-rw-   0 root         (0) root         (0)      259 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoEncoding.py
+-rw-rw-rw-   0 root         (0) root         (0)     4188 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoEncodingUI.py
+-rw-rw-rw-   0 root         (0) root         (0)      253 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoHinting.py
+-rw-rw-rw-   0 root         (0) root         (0)     1910 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoHintingPS.py
+-rw-rw-rw-   0 root         (0) root         (0)    10731 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoHintingPSUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     6830 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoHintingUI.py
+-rw-rw-rw-   0 root         (0) root         (0)      295 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoIdentification.py
+-rw-rw-rw-   0 root         (0) root         (0)     6714 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoIdentificationUI.py
+-rw-rw-rw-   0 root         (0) root         (0)      241 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoLegal.py
+-rw-rw-rw-   0 root         (0) root         (0)     6955 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoLegalUI.py
+-rw-rw-rw-   0 root         (0) root         (0)      235 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoLine.py
+-rw-rw-rw-   0 root         (0) root         (0)     4862 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoLineUI.py
+-rw-rw-rw-   0 root         (0) root         (0)      246 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoMetric.py
+-rw-rw-rw-   0 root         (0) root         (0)    13226 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoMetricUI.py
+-rw-rw-rw-   0 root         (0) root         (0)      235 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoName.py
+-rw-rw-rw-   0 root         (0) root         (0)    13730 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoNameUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     2726 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoNaviagtionPanelUI.py
+-rw-rw-rw-   0 root         (0) root         (0)      235 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoNote.py
+-rw-rw-rw-   0 root         (0) root         (0)     1740 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoNoteUI.py
+-rw-rw-rw-   0 root         (0) root         (0)      301 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoSuperSubscript.py
+-rw-rw-rw-   0 root         (0) root         (0)     7207 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoSuperSubscriptUI.py
+-rw-rw-rw-   0 root         (0) root         (0)      253 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoUnicode.py
+-rw-rw-rw-   0 root         (0) root         (0)     2453 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoUnicodeUI.py
+-rw-rw-rw-   0 root         (0) root         (0)    11197 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoValidator.py
+-rw-rw-rw-   0 root         (0) root         (0)    42129 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/glyphGrid.py
+-rw-rw-rw-   0 root         (0) root         (0)    13747 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/groups.py
+-rw-rw-rw-   0 root         (0) root         (0)     3788 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/groupsStatusPanelUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     3244 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/hintPSlistCtrl.py
+-rw-rw-rw-   0 root         (0) root         (0)     7302 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/hintPSpanel.py
+-rw-rw-rw-   0 root         (0) root         (0)    16330 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/info.py
+-rw-rw-rw-   0 root         (0) root         (0)     7184 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/kerning.py
+-rw-rw-rw-   0 root         (0) root         (0)     2885 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/kerningStatusPanelUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     4342 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/stemPanelUI.py
+-rw-rw-rw-   0 root         (0) root         (0)     4950 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/font/zonePanelUI.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:25:21.379218 wbpUFO-0.2.2/Lib/wbpUFO/view/fontinfo/
+-rw-rw-rw-   0 root         (0) root         (0)     5646 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/fontinfo/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4794 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/Lib/wbpUFO/view/glyph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 14:25:21.358219 wbpUFO-0.2.2/Lib/wbpUFO.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2211 2023-07-19 14:25:21.000000 wbpUFO-0.2.2/Lib/wbpUFO.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5825 2023-07-19 14:25:21.000000 wbpUFO-0.2.2/Lib/wbpUFO.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 14:25:21.000000 wbpUFO-0.2.2/Lib/wbpUFO.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-19 14:25:21.000000 wbpUFO-0.2.2/Lib/wbpUFO.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-07-19 14:25:21.000000 wbpUFO-0.2.2/Lib/wbpUFO.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-19 14:25:21.000000 wbpUFO-0.2.2/Lib/wbpUFO.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2211 2023-07-19 14:25:21.379218 wbpUFO-0.2.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      635 2023-07-19 14:25:19.000000 wbpUFO-0.2.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2221 2023-07-19 14:25:21.380218 wbpUFO-0.2.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-07-19 14:25:20.000000 wbpUFO-0.2.2/setup.py
```

### Comparing `wbpUFO-0.2.1/LICENSE` & `wbpUFO-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/__init__.py` & `wbpUFO-0.2.2/Lib/wbpUFO/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 from .toolbar.markColor import GlyphMarkToolbar
 from .view.font import UfoFontView
 from .view.glyph import UfoGlyphView
 
 if TYPE_CHECKING:
     from wbBase.application import App
 
-__version__ = "0.2.1"
+__version__ = "0.2.2"
 
 
 def getApp() -> App:
     """
     The currently running Workbench application.
     """
     return wx.GetApp()
```

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/config.py` & `wbpUFO-0.2.2/Lib/wbpUFO/config.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/control/__init__.py` & `wbpUFO-0.2.2/Lib/wbpUFO/control/__init__.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/control/dialogItemPicker.py` & `wbpUFO-0.2.2/Lib/wbpUFO/control/dialogItemPicker.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/control/dialogItemPickerUI.py` & `wbpUFO-0.2.2/Lib/wbpUFO/control/dialogItemPickerUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/control/findGlyphListCtrl.py` & `wbpUFO-0.2.2/Lib/wbpUFO/control/findGlyphListCtrl.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/control/glyphEditor/canvas.py` & `wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/canvas.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Implementation of the Canvas in a Glyph View.
 """
 from __future__ import annotations
 
 import logging
 import os
 import weakref
-from typing import TYPE_CHECKING, Dict, Optional
+from typing import TYPE_CHECKING, Dict, Optional, Tuple
 
 import wx
 from fontTools.misc.transform import Transform
 from wbBase.document import dbg
 from wbDefcon import Color, Font, Glyph, Guideline
 
 from ...dialog.findGlyphDialog import FindGlyphDialog
@@ -33,16 +33,18 @@
     ToolScale,
     ToolStartpoint,
     ToolZoom,
 )
 from .tool.base import WORKING
 
 if TYPE_CHECKING:
+    from weakref import ReferenceType
     from .editPanel import GlyphEditPanel
     from .tool.base import GlyphTool
+    from .drawing.base import DrawingPlaneStack
 
 log = logging.getLogger(__name__)
 
 DISPLAY_NORMAL = 0
 DISPLAY_PREVIEW = 1
 
 
@@ -87,16 +89,16 @@
         self.SetBackgroundColour("WHITE")
         self.canvasSize = wx.Size(6000, 10000)  # in font units
         self.canvasOrigin = wx.Point(2000, 4000)  # in font units
         self.SetScrollRate(1, 1)
         self._zoom = 0.5  # screen pixel per font unit
         self._minZoom = 0.05
         self._maxZoom = 20
-        self._font: Optional[Font] = None
-        self._glyph: Optional[Glyph] = None
+        self._font: Optional[ReferenceType[Font]] = None
+        self._glyph: Optional[ReferenceType[Glyph]] = None
         self.transform = None
         self.drawingPlanes = []
         self.tools: Dict[str, GlyphTool] = {}
         self._tool = None
         self._prevTool = None
         self.glyphCommands = ["FlipHorizontal", "FlipVertical"]
         self.displayMode = DISPLAY_NORMAL
@@ -232,23 +234,24 @@
         glyphNames = self.font.document.frame.glyphGridPanel.glyphNames
         currentIndex = glyphNames.index(self.glyph.name)
         if currentIndex < len(self.font) - 1:
             self.view.glyph = self.font[glyphNames[currentIndex + 1]]
 
     def showPreviousGlyph(self) -> None:
         """Show previous glyph based on glyph order in glyphGridPanel."""
+        assert isinstance(self.font, Font)
         glyphNames = self.font.document.frame.glyphGridPanel.glyphNames
         currentIndex = glyphNames.index(self.glyph.name)
         if currentIndex > 0:
             self.view.glyph = self.font[glyphNames[currentIndex - 1]]
 
     # Drawing Planes ----------------------------
 
     @property
-    def layerPlanes(self) -> LayerPlanes:
+    def layerPlanes(self) -> Tuple[LayerPlanes]:
         return tuple(p for p in self.drawingPlanes if isinstance(p, LayerPlanes))
 
     @property
     def fontLevelPlanesStack(self):
         for planeStack in self.drawingPlanes:
             if isinstance(planeStack, FontLevelPlanes):
                 return planeStack
@@ -267,44 +270,44 @@
             if layerName in oldPlanes:
                 newPlanes.append(oldPlanes[layerName])
             else:
                 newPlanes.append(LayerPlanes(self, layerName))
         self.drawingPlanes = newPlanes
         self.getActiveDrawingPlaneStack()
 
-    def getDrawingPlaneStack(self, name):
+    def getDrawingPlaneStack(self, name) -> Optional[DrawingPlaneStack]:
         for planeStack in self.drawingPlanes:
             if planeStack.name == name:
                 return planeStack
 
     def getActiveDrawingPlaneStack(self):
         for planeStack in self.drawingPlanes:
             if planeStack.active:
                 return planeStack
         planeStack = self.getDrawingPlaneStack(self.font.layers.defaultLayer.name)
         planeStack.active = True
         return planeStack
 
     # UnDo / ReDo handling ----------------------------
 
-    def CanUndo(self):
+    def CanUndo(self) -> bool:
         return self.glyph.canUndo()
 
     def Undo(self):
         self.glyph.undo()
 
-    def CanRedo(self):
+    def CanRedo(self) -> bool:
         return self.glyph.canRedo()
 
     def Redo(self):
         self.glyph.redo()
 
     # Find ---------------------------------------
 
-    def CanFind(self):
+    def CanFind(self) -> bool:
         return True
 
     def doFind(self):
         # wx.LogInfo('Ctrl + F pressed')
         with FindGlyphDialog(self, self.glyph.layer) as findGlyphDialog:
             findGlyphDialog.layer = self.glyph.layer
             if findGlyphDialog.ShowModal() == wx.ID_OK:
@@ -318,15 +321,15 @@
                     if newGlyphName not in self.font:
                         newGlyph = self.font.newGlyph(newGlyphName)
                         newGlyph.show(view=self.view)
 
     # Zooming ---------------------------------------
 
     @property
-    def zoom(self):
+    def zoom(self) -> float:
         return self._zoom
 
     @zoom.setter
     def zoom(self, value):
         newVal = min(max(round(float(value), 2), self._minZoom), self._maxZoom)
         if newVal != self._zoom:
             self._zoom = newVal
@@ -334,37 +337,37 @@
                 wx.Size(round(self.canvasSize.width * newVal), round(self.canvasSize.height * newVal))
             )
 
     @zoom.deleter
     def zoom(self):
         self.zoom = 1
 
-    def CanZoomIn(self):
+    def CanZoomIn(self) -> bool:
         return self.zoom < self._maxZoom
 
     def ZoomIn(self):
         self.Freeze()
         x = self.screenToCanvasX(self.ClientSize.width / 2)
         y = self.screenToCanvasY(self.ClientSize.height / 2)
         self.zoom *= 1.2
         self.centerCanvasOnScreen(x, y)
         self.Thaw()
 
-    def CanZoomOut(self):
+    def CanZoomOut(self) -> bool:
         return self.zoom > self._minZoom
 
     def ZoomOut(self):
         self.Freeze()
         x = self.screenToCanvasX(self.ClientSize.width / 2)
         y = self.screenToCanvasY(self.ClientSize.height / 2)
         self.zoom *= 0.8
         self.centerCanvasOnScreen(x, y)
         self.Thaw()
 
-    def CanZoom100(self):
+    def CanZoom100(self) -> bool:
         return self.zoom != 1.0
 
     def Zoom100(self):
         self.Freeze()
         x = self.screenToCanvasX(self.ClientSize.width / 2)
         y = self.screenToCanvasY(self.ClientSize.height / 2)
         self.zoom = 1.0
```

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/control/glyphEditor/cursor.py` & `wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/cursor.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/control/glyphEditor/drawing/base.py` & `wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/drawing/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 base
 ===============================================================================
 
 Base classes related to drawing on the cnavas of the glyph editor
 """
-
+from __future__ import annotations
+from typing import TYPE_CHECKING, List
 import logging
 from math import cos, radians, sin
 
 import wx
 from fontTools.misc.transform import Identity
 from wbBase.tools import get_wxBrush, get_wxFont, get_wxPen
 
@@ -44,14 +45,21 @@
     def __repr__(self):
         return f'<{self.__class__.__name__}: "{self.name}">'
 
     @property
     def transform(self):
         return self.parent.transform
 
+    @property
+    def visible(self) -> bool:
+        """
+        Visibility of the plane.
+        """
+        return False
+
     def draw(self, gc):
         """
         should be overridden by subclass
         """
         raise NotImplementedError
 
 
@@ -110,63 +118,63 @@
     inactiveAlphaDflt = 128
 
     def __init__(self, parent, name):
         super().__init__(parent, name)
         self._active = self.activeDflt
         self._inactiveAlpha = self.inactiveAlphaDflt
         self.canvas = parent
-        self._drawingPlanes = []
+        self._drawingPlanes:List[DrawingPlane] = []
         self._hitTestOrder = None
 
     def __iter__(self):
         return iter(self._drawingPlanes)
 
     def __getitem__(self, key):
         for plane in self._drawingPlanes:
             if plane.name == key:
                 return plane
         raise KeyError
 
     @property
-    def active(self):
+    def active(self) -> bool:
         return self._active
 
     @active.setter
-    def active(self, value):
+    def active(self, value:bool):
         newVal = bool(value)
         if newVal != self._active:
             self._active = newVal
             self.canvas.Refresh()
 
     @property
-    def inactiveAlpha(self):
+    def inactiveAlpha(self) -> int:
         return self._inactiveAlpha
 
     @property
-    def hitTestOrder(self):
+    def hitTestOrder(self) -> List[str]:
         if self._hitTestOrder is None:
             return [p.name for p in self._drawingPlanes]
         return self._hitTestOrder
 
     def addPlane(self, plane):
         assert issubclass(plane, self.childType)
         newPlane = plane(self)
         newPlane.canvas = self.parent
         self._drawingPlanes.append(newPlane)
 
-    def keys(self):
+    def keys(self) -> List[str]:
         return [p.name for p in self._drawingPlanes]
 
     def get(self, name, default=None):
         for plane in self._drawingPlanes:
             if plane.name == name:
                 return plane
         return default
 
-    def draw(self, gc):
+    def draw(self, gc:wx.GraphicsContext):
         for plane in [p for p in self._drawingPlanes if p.visible]:
             plane.draw(gc)
 
 
 class GuidelinePlaneMixin:
     """
     Mixin class for font and glyph level guidelines
@@ -180,15 +188,15 @@
         gc.SetFont(self.LabelFont, wx.BLACK)
         d = 3  # distace between point and label
         s = 2  # space around text
         for guideline in guidelines:
             gc.SetBrush(wx.TRANSPARENT_BRUSH)
             line = ((-8000, 0), (8000, 0))
             if guideline.angle is None:
-                if guideline.x is None:
+                if guideline.x in (0, None):
                     guideline_x = 0
                     guideline_y = guideline.y
                     guideline_angle = 0
                 elif guideline.y is None:
                     guideline_x = guideline.x
                     guideline_y = 0
                     guideline_angle = 90
```

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/control/glyphEditor/drawing/font.py` & `wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/drawing/font.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     """
 
     pen = get_wxPen(color="gray", style=wx.PENSTYLE_LONG_DASH)
 
     def __init__(self, parent):
         super().__init__(parent, "VerticalMetric")
 
-    def draw(self, gc):
+    def draw(self, gc:wx.GraphicsContext):
         gc.SetPen(self.pen)
         transformPoint = self.transform.transformPoint
         w = gc.GetSize()[0]
         info = self.font.info
         for h in (info.ascender, info.capHeight, info.xHeight, 0, info.descender):
             if h is not None:
                 y = round(transformPoint((0, h))[1])
@@ -70,15 +70,15 @@
     visibleDflt = False
     pen = get_wxPen(color=wx.Colour(0, 0, 255, 128), style=wx.PENSTYLE_LONG_DASH)
     brush = get_wxBrush(color=wx.Colour(0, 0, 255, 32))
 
     def __init__(self, parent):
         super().__init__(parent, "AlignmentZones")
 
-    def draw(self, gc):
+    def draw(self, gc:wx.GraphicsContext):
         gc.SetPen(self.pen)
         gc.SetBrush(self.brush)
         transformPoint = self.transform.transformPoint
         w = gc.GetSize()[0] + 1
         x = -1
         blueValues = (
             self.font.info.postscriptBlueValues + self.font.info.postscriptOtherBlues
@@ -100,15 +100,15 @@
     selected_pen = get_wxPen(
         color=wx.Colour(255, 0, 0, 64), width=3, style=wx.PENSTYLE_SOLID
     )
 
     def __init__(self, parent):
         super().__init__(parent, "FontGuide")
 
-    def draw(self, gc):
+    def draw(self, gc:wx.GraphicsContext):
         self.drawGuidelines(gc, self.font.guidelines)
 
     def hitTest(self, x, y):
         return self.hitTestGuidelines(x, y, self.font.guidelines)
 
 
 class FontLevelPlanes(DrawingPlaneStack):
```

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/control/glyphEditor/drawing/glyph.py` & `wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/drawing/glyph.py`

 * *Files 5% similar despite different names*

```diff
@@ -114,15 +114,15 @@
         self.labelType = self.LT_POSITION
 
     @property
     def points(self):
         "Needs to be implemented by subclasses"
         raise NotImplementedError
 
-    def draw(self, gc):
+    def draw(self, gc:wx.GraphicsContext):
         gc.SetBrush(self.LabelBrush)
         gc.SetPen(self.LabelPen)
         gc.SetFont(self.LabelFont, wx.BLACK)
         d = 3  # distace between point and label
         s = 2  # space around text
         for point in self.points:
             if self.labelType == self.LT_POSITION:
@@ -144,15 +144,15 @@
             gc.DrawRoundedRectangle(x + d, y + d, w, h, d)
             gc.DrawText(text, x + d + s, y + d + s - 1)
 
 
 class ShapeDrawPlain(GlyphLevelPlain):
     """Base class for nodes and anchors"""
 
-    def drawShape(self, gc, point, node):
+    def drawShape(self, gc:wx.GraphicsContext, point, node):
         x, y = self.transform.transformPoint((point.x, point.y))
         x = round(x)
         y = round(y)
         if hasattr(point, "color") and point.color is not None:
             brush = get_wxBrush(point.color.wx)
         else:
             brush = node["brush"]
@@ -199,15 +199,15 @@
     """Draw left and right margin of glyph on Canvas"""
 
     pen = get_wxPen(color="gray", style=wx.PENSTYLE_LONG_DASH)
 
     def __init__(self, parent):
         super().__init__(parent, "GlyphMetric")
 
-    def draw(self, gc):
+    def draw(self, gc:wx.GraphicsContext):
         gc.SetPen(self.pen)
         for w in (0, self.glyph.width):
             x = round(self.transform.transformPoint((w, 0))[0])
             gc.StrokeLine(x, 0, x, gc.GetSize()[1])
 
 
 class GlyphGuidePlane(GlyphLevelPlain, GuidelinePlaneMixin):
@@ -216,15 +216,15 @@
     selected_pen = get_wxPen(
         color=wx.Colour(255, 0, 0, 64), width=3, style=wx.PENSTYLE_SOLID
     )
 
     def __init__(self, parent):
         super().__init__(parent, "GlyphGuide")
 
-    def draw(self, gc):
+    def draw(self, gc:wx.GraphicsContext):
         self.drawGuidelines(gc, self.glyph.guidelines)
 
     def hitTest(self, x, y):
         return self.hitTestGuidelines(x, y, self.glyph.guidelines)
 
 
 class GlyphOutlinePlane(GlyphLevelPlain):
@@ -243,15 +243,15 @@
     def getInactivePen(self, pen):
         if self.layer.color:
             return get_wxPen(
                 self.getInactiveColour(self.layer.color.wx), pen.Width, pen.Style
             )
         return super().getInactivePen(pen)
 
-    def draw(self, gc):
+    def draw(self, gc:wx.GraphicsContext):
         pen = TransformPen(graphicsRoundingPen, self.transform)
         gc.SetFont(self.LabelFont, wx.LIGHT_GREY)
         for contour in self.glyph:
             if len(contour) == 0:
                 continue
             if self.parent.active:
                 point = contour[0]
@@ -328,15 +328,15 @@
     ComponentPen = wx.GREY_PEN
     ComponentSelectionPen = wx.RED_PEN
     LabelFont = get_wxFont(pointSize=7, faceName="Small Fonts")
 
     def __init__(self, parent):
         super().__init__(parent, "GlyphComponent")
 
-    def draw(self, gc):
+    def draw(self, gc:wx.GraphicsContext):
         gc.SetBrush(self.ComponentBrush)
         gc.SetFont(self.LabelFont, wx.BLACK)
         graphicsRoundingPen.glyphSet = self.layer
         pen = TransformPen(graphicsRoundingPen, self.transform)
         for componentIndex, component in enumerate(self.glyph.components):
             graphicsRoundingPen.path = gc.CreatePath()
             component.draw(pen)
@@ -407,15 +407,15 @@
         "shape": cfgShape("TTcurve", NODESHAPE_SQUARE),
         "size": cfgSize("TTcurve", 3),
     }
 
     def __init__(self, parent):
         super().__init__(parent, "OnCurvePoints")
 
-    def draw(self, gc):
+    def draw(self, gc:wx.GraphicsContext):
         for contour in self.glyph:
             for point in contour.onCurvePoints:
                 if point.segmentType == "move":
                     node = self.Move
                 elif point.segmentType == "line":
                     if point.smooth:
                         node = self.LineSmooth
@@ -480,15 +480,15 @@
     }
 
     ConnectionPen = wx.LIGHT_GREY_PEN
 
     def __init__(self, parent):
         super().__init__(parent, "OffCurvePoints")
 
-    def draw(self, gc):
+    def draw(self, gc:wx.GraphicsContext):
         for contour in self.glyph:
             for segmentIndex, segment in enumerate(contour.segments):
                 segmentType = segment[-1].segmentType
                 if segmentType in ("curve", "qcurve"):
                     if segmentIndex == 0:
                         start = contour.segments[-1][-1]
                     else:
@@ -580,15 +580,15 @@
         "shape": cfgShape("Anchor", NODESHAPE_STAR),
         "size": cfgSize("Anchor", 7),
     }
 
     def __init__(self, parent):
         super().__init__(parent, "Anchors")
 
-    def draw(self, gc):
+    def draw(self, gc:wx.GraphicsContext):
         for anchor in self.glyph.anchors:
             x, y = self.transform.transformPoint((anchor.x, anchor.y))
             x = round(x)
             y = round(y)
             self.drawShape(gc, anchor, self.Anchor)
 
     def hitTest(self, x, y):
@@ -628,15 +628,15 @@
     lockedDflt = True
     GlyphFillBrush = wx.BLACK_BRUSH
     GlyphFillPen = wx.TRANSPARENT_PEN
 
     def __init__(self, parent):
         super().__init__(parent, "GlyphFill")
 
-    def draw(self, gc):
+    def draw(self, gc:wx.GraphicsContext):
         if self.parent.active:
             gc.SetBrush(self.GlyphFillBrush)
             gc.SetPen(self.GlyphFillPen)
         else:
             gc.SetBrush(self.getInactiveBrush(self.GlyphFillBrush))
             gc.SetPen(self.getInactivePen(self.GlyphFillPen))
         graphicsPen.path = gc.CreatePath()
@@ -659,15 +659,15 @@
         "shape": cfgShape("RedArrow", NODESHAPE_DIAMOND),
         "size": cfgSize("RedArrow", 18),
     }
 
     def __init__(self, parent):
         super().__init__(parent, "RedArrows")
 
-    def drawArrow(self, gc, position, errors):
+    def drawArrow(self, gc:wx.GraphicsContext, position, errors):
         message = []
         for error in errors:
             if error.vector:
                 vector = error.vector
             else:
                 vector = (-1, 1)
             angle = atan2(vector[0], -vector[1])
@@ -721,15 +721,15 @@
             text_y += size
         elif -0.6 > direction:  # right
             text_x += 1.2 * size
             text_y += size
 
         gc.DrawText(messageText, text_x, text_y)
 
-    def draw(self, gc):
+    def draw(self, gc:wx.GraphicsContext):
         errors_by_position = {}
         for error in self.glyph.getOutlineErrors():
             if error.position is not None:
                 if (error.position[0], error.position[1]) in errors_by_position:
                     errors_by_position[(error.position[0], error.position[1])].extend(
                         [error]
                     )
@@ -743,29 +743,29 @@
     """
     Not used yet!
     """
 
     def __init__(self, parent):
         super(AccentCloudPlane, self).__init__(parent, "AccentCloud")
 
-    def draw(self, gc):
+    def draw(self, gc:wx.GraphicsContext):
         for anchor in self.glyph.anchors:
             if anchor.name == "top":
                 pass
 
 
 class LayerPlanes(DrawingPlaneStack):
     """
     Collection of Glyph Level Plains
     """
 
     childType = GlyphLevelPlain
-    activeDflt = False
-    visibleInactiveDflt = True
-    inactiveAlphaDflt = 180
+    activeDflt:bool = False
+    visibleInactiveDflt:bool = True
+    inactiveAlphaDflt:int = 180
 
     def __init__(self, parent, name):
         super(LayerPlanes, self).__init__(parent, name)
         self._visibleInactive = self.visibleInactiveDflt
         self.addPlane(GlyphMetricPlane)
         self.addPlane(GlyphGuidePlane)
         self.addPlane(GlyphFillPlane)
@@ -785,19 +785,19 @@
             "GlyphComponent",
             "GlyphMetric",
             "GlyphGuide",
             "GlyphOutline",
         ]
 
     @property
-    def visible(self):
+    def visible(self) -> bool:
         return self.active or self._visibleInactive
 
     @property
-    def visibleInactive(self):
+    def visibleInactive(self) -> bool:
         return self._visibleInactive
 
     @visibleInactive.setter
     def visibleInactive(self, value):
         newValue = bool(value)
         if newValue != self._visibleInactive:
             visible = self.visible
@@ -813,15 +813,15 @@
     def glyph(self):
         g = self.parent.glyph
         if g is not None:
             glyphName = g.name
             if glyphName in self.layer:
                 return self.layer[glyphName]
 
-    def draw(self, gc):
+    def draw(self, gc:wx.GraphicsContext):
         if self.glyph is not None:
             for plane in [p for p in self._drawingPlanes if p.visible]:
                 plane.draw(gc)
         elif self.active:
             canvas = self.canvas
             g = canvas.glyph
             if g is None:
```

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/control/glyphEditor/editPanel.py` & `wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/editPanel.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/control/glyphEditor/menu.py` & `wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/menu.py`

 * *Files 1% similar despite different names*

```diff
@@ -542,14 +542,15 @@
             font.releaseHeldNotifications()
 
     def on_removeOverlap(self, event):
         font = self.font
         if font:
             font.holdNotifications()
         glyph = self.glyph
+        assert isinstance(glyph, Glyph)
         contours = [c for c in glyph]
         glyph.disableNotifications()
         glyph.clearContours()
         glyph.undoManager.saveState()
         Boolean.union(contours, glyph.getPointPen())
         glyph.round(roundAnchors=False, roundComponents=False)
         glyph.enableNotifications()
```

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/control/glyphEditor/tool/__init__.py` & `wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/__init__.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/control/glyphEditor/tool/addellipse.py` & `wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/addellipse.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/control/glyphEditor/tool/addrectangle.py` & `wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/addrectangle.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/control/glyphEditor/tool/base.py` & `wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/base.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/control/glyphEditor/tool/magicwand.py` & `wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/magicwand.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/control/glyphEditor/tool/tooldraw.py` & `wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/tooldraw.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/control/glyphEditor/tool/tooledit.py` & `wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/tooledit.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/control/glyphEditor/tool/toolerase.py` & `wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/toolerase.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/control/glyphEditor/tool/toolknife.py` & `wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/toolknife.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/control/glyphEditor/tool/toolmeter.py` & `wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/toolmeter.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/control/glyphEditor/tool/toolpan.py` & `wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/toolpan.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/control/glyphEditor/tool/toolreverse.py` & `wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/toolreverse.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/control/glyphEditor/tool/toolrotate.py` & `wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/toolrotate.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/control/glyphEditor/tool/toolscale.py` & `wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/toolscale.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/control/glyphEditor/tool/toolstartpoint.py` & `wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/toolstartpoint.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/control/glyphEditor/tool/toolzoom.py` & `wbpUFO-0.2.2/Lib/wbpUFO/control/glyphEditor/tool/toolzoom.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/control/glyphGridStatusPanelUI.py` & `wbpUFO-0.2.2/Lib/wbpUFO/control/glyphGridStatusPanelUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/control/kerningViewCanvas.py` & `wbpUFO-0.2.2/Lib/wbpUFO/control/kerningViewCanvas.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/control/kerningViewPanelUI.py` & `wbpUFO-0.2.2/Lib/wbpUFO/control/kerningViewPanelUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/control/libControl.py` & `wbpUFO-0.2.2/Lib/wbpUFO/control/libControl.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/control/panelItemPicker.py` & `wbpUFO-0.2.2/Lib/wbpUFO/control/panelItemPicker.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/control/panelItemPickerUI.py` & `wbpUFO-0.2.2/Lib/wbpUFO/control/panelItemPickerUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/dialog/anchorDialog.py` & `wbpUFO-0.2.2/Lib/wbpUFO/dialog/anchorDialog.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/dialog/anchorDialogUI.py` & `wbpUFO-0.2.2/Lib/wbpUFO/dialog/anchorDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/dialog/applyGlyphConstructionDialog.py` & `wbpUFO-0.2.2/Lib/wbpUFO/dialog/applyGlyphConstructionDialog.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/dialog/applyGlyphConstructionDialogUI.py` & `wbpUFO-0.2.2/Lib/wbpUFO/dialog/applyGlyphConstructionDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/dialog/assignLayerDialog.py` & `wbpUFO-0.2.2/Lib/wbpUFO/dialog/assignLayerDialog.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/dialog/assignLayerDialogUI.py` & `wbpUFO-0.2.2/Lib/wbpUFO/dialog/assignLayerDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/dialog/componentDialog.py` & `wbpUFO-0.2.2/Lib/wbpUFO/dialog/componentDialog.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/dialog/componentDialogUI.py` & `wbpUFO-0.2.2/Lib/wbpUFO/dialog/componentDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/dialog/deleteGlyphsDialog.py` & `wbpUFO-0.2.2/Lib/wbpUFO/dialog/deleteGlyphsDialog.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/dialog/deleteGlyphsDialogUI.py` & `wbpUFO-0.2.2/Lib/wbpUFO/dialog/deleteGlyphsDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/dialog/findGlyphDialog.py` & `wbpUFO-0.2.2/Lib/wbpUFO/dialog/findGlyphDialog.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/dialog/findGlyphDialogUI.py` & `wbpUFO-0.2.2/Lib/wbpUFO/dialog/findGlyphDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/dialog/generateOTCFFoptionsDialog.py` & `wbpUFO-0.2.2/Lib/wbpUFO/dialog/generateOTCFFoptionsDialog.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/dialog/generateOTCFFoptionsDialogUI.py` & `wbpUFO-0.2.2/Lib/wbpUFO/dialog/generateOTCFFoptionsDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/dialog/guidelineDialog.py` & `wbpUFO-0.2.2/Lib/wbpUFO/dialog/guidelineDialog.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/dialog/guidelineDialogUI.py` & `wbpUFO-0.2.2/Lib/wbpUFO/dialog/guidelineDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/dialog/layerDialog.py` & `wbpUFO-0.2.2/Lib/wbpUFO/dialog/layerDialog.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/dialog/layerDialogUI.py` & `wbpUFO-0.2.2/Lib/wbpUFO/dialog/layerDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/dialog/newFontDialogUI.py` & `wbpUFO-0.2.2/Lib/wbpUFO/dialog/newFontDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/dialog/newGlyphDialog.py` & `wbpUFO-0.2.2/Lib/wbpUFO/dialog/newGlyphDialog.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/dialog/newGlyphDialogUI.py` & `wbpUFO-0.2.2/Lib/wbpUFO/dialog/newGlyphDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/dialog/renameGlyphDialog.py` & `wbpUFO-0.2.2/Lib/wbpUFO/dialog/renameGlyphDialog.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/dialog/renameGlyphDialogUI.py` & `wbpUFO-0.2.2/Lib/wbpUFO/dialog/renameGlyphDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/dialog/revertFontDialog.py` & `wbpUFO-0.2.2/Lib/wbpUFO/dialog/revertFontDialog.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/dialog/revertFontDialogUI.py` & `wbpUFO-0.2.2/Lib/wbpUFO/dialog/revertFontDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/dialog/selectFontsDialog.py` & `wbpUFO-0.2.2/Lib/wbpUFO/dialog/selectFontsDialog.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/dialog/selectFontsDialogUI.py` & `wbpUFO-0.2.2/Lib/wbpUFO/dialog/selectFontsDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/document.py` & `wbpUFO-0.2.2/Lib/wbpUFO/document.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,18 @@
     canReload = True
 
     def __init__(self, template:UfoTemplate):
         super().__init__(template)
         self._rFont = None
 
     @property
-    def font(self) -> Font:
+    def font(self) -> Optional[Font]:
+        """
+        The Font object associated with this document.
+        """
         return self._data
 
     @font.setter
     def font(self, font: Font):
         assert isinstance(font, Font)
         assert self._data is None, "Can not replace font in UfoDoc"
         self._data = font
```

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/glyphCommand/__init__.py` & `wbpUFO-0.2.2/Lib/wbpUFO/glyphCommand/__init__.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/glyphCommand/anchor.py` & `wbpUFO-0.2.2/Lib/wbpUFO/glyphCommand/anchor.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/glyphCommand/base.py` & `wbpUFO-0.2.2/Lib/wbpUFO/glyphCommand/base.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/glyphCommand/commandListCtrl.py` & `wbpUFO-0.2.2/Lib/wbpUFO/glyphCommand/commandListCtrl.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/glyphCommand/commandListDialog.py` & `wbpUFO-0.2.2/Lib/wbpUFO/glyphCommand/commandListDialog.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/glyphCommand/commandListDialogUI.py` & `wbpUFO-0.2.2/Lib/wbpUFO/glyphCommand/commandListDialogUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/glyphCommand/composite.py` & `wbpUFO-0.2.2/Lib/wbpUFO/glyphCommand/composite.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/glyphCommand/contour.py` & `wbpUFO-0.2.2/Lib/wbpUFO/glyphCommand/contour.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/glyphCommand/guideline.py` & `wbpUFO-0.2.2/Lib/wbpUFO/glyphCommand/guideline.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/glyphCommand/layer.py` & `wbpUFO-0.2.2/Lib/wbpUFO/glyphCommand/layer.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/glyphCommand/metric.py` & `wbpUFO-0.2.2/Lib/wbpUFO/glyphCommand/metric.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/glyphCommand/misc.py` & `wbpUFO-0.2.2/Lib/wbpUFO/glyphCommand/misc.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/glyphCommand/parameter.py` & `wbpUFO-0.2.2/Lib/wbpUFO/glyphCommand/parameter.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/panel/glyphViewCanvas.py` & `wbpUFO-0.2.2/Lib/wbpUFO/panel/glyphViewCanvas.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/panel/glyphViewPanel.py` & `wbpUFO-0.2.2/Lib/wbpUFO/panel/glyphViewPanel.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import wx
-
+from wx import aui
 # from wbDefcon import Glyph
 # from wbFontParts import RGlyph
 
 from .glyphViewPanelUI import GlyphViewPanelUI
 
 name = "GlyphViewPanel"
 
@@ -58,15 +58,15 @@
     def on_checkBox_showKerning(self, event):
         self.glyphViewCanvas.Refresh()
 
     def on_btn_clear(self, event):
         self.clearGlyphs()
 
 
-glyphViewPanelInfo = wx.aui.AuiPaneInfo()
+glyphViewPanelInfo = aui.AuiPaneInfo()
 glyphViewPanelInfo.Name(name)
 glyphViewPanelInfo.Caption(name)
 glyphViewPanelInfo.Dock()
 glyphViewPanelInfo.Bottom()
 glyphViewPanelInfo.Resizable()
 glyphViewPanelInfo.MaximizeButton(True)
 glyphViewPanelInfo.MinimizeButton(True)
```

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/panel/glyphViewPanelUI.py` & `wbpUFO-0.2.2/Lib/wbpUFO/panel/glyphViewPanelUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/template.py` & `wbpUFO-0.2.2/Lib/wbpUFO/template.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/toolbar/__init__.py` & `wbpUFO-0.2.2/Lib/wbpUFO/toolbar/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,67 @@
+from __future__ import annotations
+
+from typing import TYPE_CHECKING, Optional
+
 import wx
 from wx import aui
 
+if TYPE_CHECKING:
+    from wbBase.application import App
+    from wbBase.document.view import View
+
 
 class BaseToolbar(aui.AuiToolBar):
+    """
+    Base class for all toolbars of the wbpUfo plugin.
+    """
+
     itemType = wx.ITEM_NORMAL
+
     def __init__(self, parent, name=None):
         id = wx.ID_ANY
         pos = wx.DefaultPosition
         size = wx.DefaultSize
-        style = (
-            wx.aui.AUI_TB_HORZ_LAYOUT | wx.aui.AUI_TB_PLAIN_BACKGROUND | wx.NO_BORDER
-        )
+        style = aui.AUI_TB_HORZ_LAYOUT | aui.AUI_TB_PLAIN_BACKGROUND | wx.NO_BORDER
         super().__init__(parent, id, pos, size, style)
         if isinstance(name, str):
             self.Name = name
         self.SetToolBitmapSize(wx.Size(16, 16))
 
     @property
-    def app(self):
+    def app(self) -> App:
+        """
+        The running Workbench application.
+        """
         return wx.GetApp()
 
     @property
-    def currentView(self):
+    def currentView(self) -> Optional[View]:
+        """
+        The currently active view, may be None.
+        """
         return self.app.documentManager.currentView
 
     @staticmethod
-    def bitmap(name):
+    def bitmap(name) -> wx.Bitmap:
         return wx.ArtProvider.GetBitmap(name, wx.ART_TOOLBAR)
 
     def appendTool(
-        self, label, bitmapName, helpText=wx.EmptyString, commandIndex=-1, kind=None
-    ):
+        self,
+        label: str,
+        bitmapName: str,
+        helpText: str = wx.EmptyString,
+        commandIndex: int = -1,
+        kind = None
+    ) -> aui.AuiToolBarItem:
         if not helpText:
             helpText = label
         if kind is None:
             kind = self.itemType
-        tool = self.AddTool(
+        tool: aui.AuiToolBarItem = self.AddTool(
             toolId=wx.ID_ANY,
             label=label,
             bitmap=self.bitmap(bitmapName),
             short_help_string=helpText,
             kind=kind,
         )
         tool.SetUserData(commandIndex)
```

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/toolbar/command.py` & `wbpUFO-0.2.2/Lib/wbpUFO/toolbar/command.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/toolbar/editTool.py` & `wbpUFO-0.2.2/Lib/wbpUFO/toolbar/editTool.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/toolbar/glyphLock.py` & `wbpUFO-0.2.2/Lib/wbpUFO/toolbar/glyphLock.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
             "Lock Components",
             "COMPONENT_LOCK",
             "Lock components in current glyph editor",
             component,
         )
 
     def on_Tool(self, event):
-        tool = self.FindTool(event.Id)
+        tool:aui.AuiToolBarItem = self.FindTool(event.Id)
         i = tool.GetUserData()
         planes = []
         if i in fontLevel:
             fontPlanes = self.currentView.frame.canvas.getDrawingPlaneStack("Font")
             if i == metric:
                 planes.append(fontPlanes.get("VerticalMetric"))
             elif i == zone:
@@ -88,41 +88,40 @@
             elif i == component:
                 planes.append(activePlanes.get("GlyphComponent"))
         for plane in planes:
             plane.locked = event.IsChecked()
 
     def on_update_Tool(self, event):
         view = self.currentView
-        if view and view.document:
-            if isinstance(view, UfoGlyphView):
-                canvas = view.frame.canvas
-                tool = self.FindTool(event.Id)
-                i = tool.GetUserData()
-                not_yet_supported = (margin, metric, zone)
-                planes = []
-                if i in not_yet_supported:
-                    event.Check(True)
-                    event.Enable(False)
-                    return
-                event.Enable(True)
-                if i in fontLevel:
-                    planes = canvas.getDrawingPlaneStack("Font")
-                    if i == guide:
-                        event.Check(planes.get("FontGuide").locked)
-                elif i in glyphLevel:
-                    planes = canvas.getActiveDrawingPlaneStack()
-                    if i == metric:
-                        event.Check(planes.get("VerticalMetric").locked)
-                    elif i == zone:
-                        event.Check(planes.get("AlignmentZones").locked)
-                    elif i == margin:
-                        event.Check(planes.get("GlyphMetric").locked)
-                    elif i == guide:
-                        event.Check(planes.get("GlyphGuide").locked)
-                    elif i == anchor:
-                        event.Check(planes.get("Anchors").locked)
-                    elif i == contour:
-                        event.Check(planes.get("GlyphOutline").locked)
-                    elif i == component:
-                        event.Check(planes.get("GlyphComponent").locked)
+        if isinstance(view, UfoGlyphView) and view.document:
+            canvas = view.frame.canvas
+            tool:aui.AuiToolBarItem = self.FindTool(event.Id)
+            i = tool.GetUserData()
+            not_yet_supported = (margin, metric, zone)
+            planes = []
+            if i in not_yet_supported:
+                event.Check(True)
+                event.Enable(False)
                 return
+            event.Enable(True)
+            if i in fontLevel:
+                planes = canvas.getDrawingPlaneStack("Font")
+                if i == guide:
+                    event.Check(planes.get("FontGuide").locked)
+            elif i in glyphLevel:
+                planes = canvas.getActiveDrawingPlaneStack()
+                if i == metric:
+                    event.Check(planes.get("VerticalMetric").locked)
+                elif i == zone:
+                    event.Check(planes.get("AlignmentZones").locked)
+                elif i == margin:
+                    event.Check(planes.get("GlyphMetric").locked)
+                elif i == guide:
+                    event.Check(planes.get("GlyphGuide").locked)
+                elif i == anchor:
+                    event.Check(planes.get("Anchors").locked)
+                elif i == contour:
+                    event.Check(planes.get("GlyphOutline").locked)
+                elif i == component:
+                    event.Check(planes.get("GlyphComponent").locked)
+            return
         event.Enable(False)
```

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/toolbar/glyphShow.py` & `wbpUFO-0.2.2/Lib/wbpUFO/toolbar/glyphShow.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/toolbar/layer.py` & `wbpUFO-0.2.2/Lib/wbpUFO/toolbar/layer.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/toolbar/markColor.py` & `wbpUFO-0.2.2/Lib/wbpUFO/toolbar/markColor.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/view/font/__init__.py` & `wbpUFO-0.2.2/Lib/wbpUFO/view/fontinfo/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 import logging
 
 import wx
 
 from wbDefcon import Font
-from wbBase.document import dbg
 from wbBase.document.notebook import DocumentPageMixin
 from wbBase.document.view import View
 
-# from .feature import FeaturePage
-from .glyphGrid import GlyphGridPage
-# from .groups import GroupsPage
-# from .info import InfoPage
-# from .kerning import KerningPage
+from ..font.feature import FeaturePage
+from ..font.groups import GroupsPage
+from ..font.info import InfoPage
+from ..font.kerning import KerningPage
 
 log = logging.getLogger(__name__)
 
 
-class UfoFontWindow(wx.Notebook, DocumentPageMixin):
+class UfoFontInfoWindow(wx.Notebook, DocumentPageMixin):
     """
-    The main Document Window for UFO Documents
+    Document Window for UFO Font Info
     """
 
     def __init__(self, parent, doc, view):
         ID = wx.ID_ANY
         pos = wx.DefaultPosition
         size = wx.DefaultSize
         wx.Notebook.__init__(
@@ -37,59 +35,49 @@
         DocumentPageMixin.__init__(self, doc, view)
         self.SetExtraStyle(wx.WS_EX_VALIDATE_RECURSIVELY)
         self._font = None
         notebookIndex = 0
         tabIcons = wx.ImageList(16, 16)
         self.AssignImageList(tabIcons)
 
-        # GlyphGrid page
-        self.glyphGridPage = GlyphGridPage(self)
-        self.glyphGridPanel = self.glyphGridPage.glyphGridPanel
-        self.AddPage(self.glyphGridPage, "Glyphs", True)
-        icon = wx.ArtProvider.GetBitmap("VIEW_ICON", wx.ART_FRAME_ICON)
+        # Info page
+        self.infoPage = InfoPage(self)
+        self.AddPage(self.infoPage, "Info", False)
+        icon = wx.ArtProvider.GetBitmap("VIEW_INFO", wx.ART_FRAME_ICON)
         if icon.IsOk():
             tabIcons.Add(icon)
             self.SetPageImage(notebookIndex, notebookIndex)
             notebookIndex += 1
 
-        # # Info page
-        # self.infoPage = InfoPage(self)
-        # self.AddPage(self.infoPage, "Info", False)
-        # icon = wx.ArtProvider.GetBitmap("VIEW_INFO", wx.ART_FRAME_ICON)
-        # if icon.IsOk():
-        #     tabIcons.Add(icon)
-        #     self.SetPageImage(notebookIndex, notebookIndex)
-        #     notebookIndex += 1
-
-        # # Feature page
-        # self.featurePage = FeaturePage(self)
-        # self.AddPage(self.featurePage, "Feature", False)
-        # icon = wx.ArtProvider.GetBitmap("BLANK", wx.ART_FRAME_ICON)
-        # if icon.IsOk():
-        #     tabIcons.Add(icon)
-        #     self.SetPageImage(notebookIndex, notebookIndex)
-        #     notebookIndex += 1
-
-        # # Groups page
-        # self.groupsPage = GroupsPage(self)
-        # self.AddPage(self.groupsPage, "Groups", False)
-        # icon = wx.ArtProvider.GetBitmap("VIEW_GROUP", wx.ART_FRAME_ICON)
-        # if icon.IsOk():
-        #     tabIcons.Add(icon)
-        #     self.SetPageImage(notebookIndex, notebookIndex)
-        #     notebookIndex += 1
-
-        # # Kerning page
-        # self.kerningPage = KerningPage(self)
-        # self.AddPage(self.kerningPage, "Kerning", False)
-        # icon = wx.ArtProvider.GetBitmap("VIEW_KERNING", wx.ART_FRAME_ICON)
-        # if icon.IsOk():
-        #     tabIcons.Add(icon)
-        #     self.SetPageImage(notebookIndex, notebookIndex)
-        #     notebookIndex += 1
+        # Feature page
+        self.featurePage = FeaturePage(self)
+        self.AddPage(self.featurePage, "Feature", False)
+        icon = wx.ArtProvider.GetBitmap("BLANK", wx.ART_FRAME_ICON)
+        if icon.IsOk():
+            tabIcons.Add(icon)
+            self.SetPageImage(notebookIndex, notebookIndex)
+            notebookIndex += 1
+
+        # Groups page
+        self.groupsPage = GroupsPage(self)
+        self.AddPage(self.groupsPage, "Groups", False)
+        icon = wx.ArtProvider.GetBitmap("VIEW_GROUP", wx.ART_FRAME_ICON)
+        if icon.IsOk():
+            tabIcons.Add(icon)
+            self.SetPageImage(notebookIndex, notebookIndex)
+            notebookIndex += 1
+
+        # Kerning page
+        self.kerningPage = KerningPage(self)
+        self.AddPage(self.kerningPage, "Kerning", False)
+        icon = wx.ArtProvider.GetBitmap("VIEW_KERNING", wx.ART_FRAME_ICON)
+        if icon.IsOk():
+            tabIcons.Add(icon)
+            self.SetPageImage(notebookIndex, notebookIndex)
+            notebookIndex += 1
 
         # # Connect Events
         self.Bind(wx.EVT_NOTEBOOK_PAGE_CHANGING, self.on_PAGE_CHANGING)
         #  Window
         self.Bind(wx.EVT_SET_FOCUS, self.on_SET_FOCUS)
 
     def __repr__(self):
@@ -102,20 +90,23 @@
     @property
     def font(self):
         """The wbDefcon Font object of this UfoFontWindow"""
         return self._font
 
     @font.setter
     def font(self, value):
+        if value == self._font:
+            return
         assert self._font is None
         assert isinstance(
             value, Font
         ), f"Expected Font, got {value}, type {type(value)}"
         assert value == self._document.font
         self._font = value
+        self.title = self._document.title.replace("Font", "Info", 1)
         log.debug("Font %r set for %r", self._font, self)
         for page in self.Children:
             page.font = value
 
     @font.deleter
     def font(self):
         for page in self.Children:
@@ -140,69 +131,46 @@
             event.Veto()
 
     def on_SET_FOCUS(self, event):
         self.CurrentPage.SetFocus()
         event.Skip()
 
 
-class UfoFontView(View):
-    frameType = UfoFontWindow
+class UfoFontInfoView(View):
+    frameType = UfoFontInfoWindow
+
+    def __init__(self):
+        super().__init__()
+        self._typeName = "UFO Font Info View"
 
     def __repr__(self):
         if self._document:
-            return '<%s of "%s">' % (
-                self.__class__.__name__,
-                self._document.printableName,
-            )
-        return "<%s of %s>" % (
-            self.__class__.__name__,
-            self._document.__class__.__name__,
-        )
+            return f'<{self.__class__.__name__} of "{self._document.printableName}">'
+        return f"<{self.__class__.__name__} of {self._document.__class__.__name__}>"
 
     @property
     def font(self):
         return self.document.font
 
     def OnCreate(self, doc, flags):
-        dbg(f'UfoFontView.OnCreate(doc="{doc}", flags={flags})', indent=1)
         self._document = doc
-        self._typeName = doc.template.viewTypeName
-        self._frame:UfoFontWindow = self.frameType(self.documentNotebook, doc, self)
+        # self._typeName = doc.template.viewTypeName
+        self._frame = self.frameType(self.documentNotebook, doc, self)
         self.documentNotebook.AddPage(
             self._frame,
-            doc.printableName,
+            doc.printableName.replace("Font", "Info", 1),
             True,
-            wx.ArtProvider.GetBitmap("F", wx.ART_FRAME_ICON),
+            wx.ArtProvider.GetBitmap("I", wx.ART_FRAME_ICON),
         )
-        dbg(indent=0)
         return True
 
     def OnUpdate(self, sender, hint):
-        dbg(f"UfoFontView.OnUpdate(sender={sender}, hint={hint})", indent=1)
         super().OnUpdate(sender, hint)
         if hint and hint[0] == "font loaded":
             frame = self._frame
             if frame.font is None:
                 frame.font = self.document.font
-            frame.title = self._document.title
+            frame.title = self._document.title.replace("Font", "Info", 1)
             if frame and hasattr(frame, "OnTitleIsModified"):
                 frame.OnTitleIsModified()
             frame.TransferDataToWindow()
-            frame.glyphGridPanel.SendSizeEvent()
-        dbg(indent=0)
-
-    def OnClose(self, deleteWindow=True):
-        dbg(f"UfoFontView.OnClose(deleteWindow={deleteWindow})", indent=1)
-        result = False
-        for view in self._document.views:
-            if view is not self:
-                dbg(f"UfoFontView.OnClose() closing child view {view}")
-                if not view.Close(deleteWindow=True):
-                    dbg(
-                        f"UfoFontView.OnClose() returns {result}, can not close {view}",
-                        indent=0,
-                    )
-                    return result
-                dbg("UfoFontView.OnClose() closing child view done")
-        result = super().OnClose(deleteWindow=deleteWindow)
-        dbg(indent=0)
-        return result
+            # frame.glyphGridPanel.SendSizeEvent()
```

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/view/font/feature.py` & `wbpUFO-0.2.2/Lib/wbpUFO/view/font/feature.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,21 @@
+"""
+feature
+===============================================================================
+
+"""
 import logging
 
 import fontTools.feaLib.ast as ast
 import wx
 import wx.stc as stc
 from feaASTools.inspect import isFeatureAutomatic, setFeatureAutomatic
-from wbDefcon import Font
-from wbBase.scripting import MacroButtonMixin
 from wbBase.control.textEditControl import STCfindReplaceMixin
+from wbBase.scripting import MacroButtonMixin
+from wbDefcon import Font
 
 log = logging.getLogger(__name__)
 
 feaKeywords = """
 anchor anchorDef anon anonymous by contour cursive device 
 enum enumerate excludeDFLT exclude_dflt feature featureNames from 
 ignore IgnoreBaseGlyphs IgnoreLigatures IgnoreMarks 
@@ -72,14 +77,15 @@
             # 	startPos += 1
 
 
 class FeatureTextCtrl(stc.StyledTextCtrl, STCfindReplaceMixin):
     """
     StyledTextCtrl to display the Feature Code.
     """
+
     def __init__(
         self,
         parent,
         id=wx.ID_ANY,
         pos=wx.DefaultPosition,
         size=wx.DefaultSize,
         style=wx.BORDER_NONE,
@@ -259,14 +265,15 @@
         event.Skip()
 
 
 class FeatureTreeCtrl(wx.TreeCtrl):
     """
     Tree Control in the Feature Panel
     """
+
     def __init__(
         self,
         parent,
         id=wx.ID_ANY,
         pos=wx.DefaultPosition,
         size=wx.DefaultSize,
         style=wx.BORDER_NONE
@@ -414,14 +421,15 @@
         #     wx.CallAfter(self.SelectItem, item)
 
 
 class FeatureStatusPanel(wx.Panel, MacroButtonMixin):
     """
     Tree Status Panel in the Feature Panel
     """
+
     def __init__(
         self,
         parent,
         id=wx.ID_ANY,
         pos=wx.DefaultPosition,
         size=wx.DefaultSize,
         style=wx.BORDER_NONE,
```

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/view/font/fontInfoCaretUI.py` & `wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoCaretUI.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 ###########################################################################
 ## Python code generated with wxFormBuilder (version 3.10.1-0-g8feb16b3)
 ## http://www.wxformbuilder.org/
 ##
 ## PLEASE DO *NOT* EDIT THIS FILE!
 ###########################################################################
 
+from .fontInfoBase import FontInfoBasePage
 import wx
 import wx.xrc
 
 ###########################################################################
 ## Class FontInfoCaretUI
 ###########################################################################
 
-class FontInfoCaretUI ( wx.ScrolledWindow ):
+class FontInfoCaretUI ( FontInfoBasePage ):
 
-    def __init__( self, parent, id = wx.ID_ANY, pos = wx.DefaultPosition, size = wx.Size( -1,-1 ), style = wx.HSCROLL|wx.VSCROLL, name = wx.EmptyString ):
-        wx.ScrolledWindow.__init__ ( self, parent, id = id, pos = pos, size = size, style = style, name = name )
+    def __init__( self, parent, id = wx.ID_ANY, pos = wx.DefaultPosition, size = wx.Size( -1,-1 ), style = 0, name = u"FontInfoCaret" ):
+        FontInfoBasePage.__init__ ( self, parent, id = id, pos = pos, size = size, style = style, name = name )
 
-        self.SetExtraStyle( wx.WS_EX_VALIDATE_RECURSIVELY )
         self.SetBackgroundColour( wx.SystemSettings.GetColour( wx.SYS_COLOUR_WINDOW ) )
 
         sizerMain = wx.BoxSizer( wx.VERTICAL )
 
         boxHhea = wx.StaticBoxSizer( wx.StaticBox( self, wx.ID_ANY, u"hhea" ), wx.VERTICAL )
 
         sizerHhea = wx.GridBagSizer( 0, 0 )
```

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/view/font/fontInfoClassificationUI.py` & `wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoClassificationUI.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # -*- coding: utf-8 -*-
 
 ###########################################################################
-## Python code generated with wxFormBuilder (version 3.10.0-4761b0c)
+## Python code generated with wxFormBuilder (version 3.10.1-0-g8feb16b3)
 ## http://www.wxformbuilder.org/
 ##
 ## PLEASE DO *NOT* EDIT THIS FILE!
 ###########################################################################
 
+from .fontInfoBase import FontInfoBasePage
 import wx
 import wx.xrc
 
 ###########################################################################
 ## Class FontInfoClassificationUI
 ###########################################################################
 
-class FontInfoClassificationUI ( wx.ScrolledWindow ):
+class FontInfoClassificationUI ( FontInfoBasePage ):
 
-    def __init__( self, parent, id = wx.ID_ANY, pos = wx.DefaultPosition, size = wx.Size( -1,-1 ), style = wx.HSCROLL|wx.VSCROLL, name = wx.EmptyString ):
-        wx.ScrolledWindow.__init__ ( self, parent, id = id, pos = pos, size = size, style = style, name = name )
+    def __init__( self, parent, id = wx.ID_ANY, pos = wx.DefaultPosition, size = wx.Size( -1,-1 ), style = 0, name = u"FontInfoClassification" ):
+        FontInfoBasePage.__init__ ( self, parent, id = id, pos = pos, size = size, style = style, name = name )
 
-        self.SetExtraStyle( wx.WS_EX_VALIDATE_RECURSIVELY )
         self.SetBackgroundColour( wx.SystemSettings.GetColour( wx.SYS_COLOUR_WINDOW ) )
 
         sizerMain = wx.BoxSizer( wx.VERTICAL )
 
         boxPostScript = wx.StaticBoxSizer( wx.StaticBox( self, wx.ID_ANY, u"PostScript" ), wx.VERTICAL )
 
         sizerPostScript = wx.GridBagSizer( 0, 0 )
```

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/view/font/fontInfoCodepageUI.py` & `wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoCodepageUI.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,25 +4,26 @@
 ## Python code generated with wxFormBuilder (version 3.10.1-0-g8feb16b3)
 ## http://www.wxformbuilder.org/
 ##
 ## PLEASE DO *NOT* EDIT THIS FILE!
 ###########################################################################
 
 from .fontInfoControl import CodePageBitList
+from .fontInfoBase import FontInfoBasePage
 import wx
 import wx.xrc
 
 ###########################################################################
 ## Class FontInfoCodepageUI
 ###########################################################################
 
-class FontInfoCodepageUI ( wx.ScrolledWindow ):
+class FontInfoCodepageUI ( FontInfoBasePage ):
 
-    def __init__( self, parent, id = wx.ID_ANY, pos = wx.DefaultPosition, size = wx.Size( -1,-1 ), style = wx.HSCROLL|wx.VSCROLL, name = wx.EmptyString ):
-        wx.ScrolledWindow.__init__ ( self, parent, id = id, pos = pos, size = size, style = style, name = name )
+    def __init__( self, parent, id = wx.ID_ANY, pos = wx.DefaultPosition, size = wx.Size( -1,-1 ), style = wx.HSCROLL|wx.VSCROLL, name = u"FontInfoCodepage" ):
+        FontInfoBasePage.__init__ ( self, parent, id = id, pos = pos, size = size, style = style, name = name )
 
         self.SetExtraStyle( wx.WS_EX_VALIDATE_RECURSIVELY )
         self.SetBackgroundColour( wx.SystemSettings.GetColour( wx.SYS_COLOUR_WINDOW ) )
 
         sizerMain = wx.BoxSizer( wx.VERTICAL )
 
         boxOS2 = wx.StaticBoxSizer( wx.StaticBox( self, wx.ID_ANY, u"OpenType OS/2 Table" ), wx.VERTICAL )
```

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/view/font/fontInfoControl.py` & `wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoControl.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-import logging
+"""
+fontInfoControl
+===============================================================================
 
+"""
 import wx
 from wx.lib.mixins.listctrl import ListCtrlAutoWidthMixin, TextEditMixin
 
-log = logging.getLogger(__name__)
-
 
 class BitList(wx.CheckListBox):
     def __init__(
         self,
-        parent,
-        id=wx.ID_ANY,
-        pos=wx.DefaultPosition,
-        size=wx.DefaultSize,
+        parent: wx.Window,
+        id: int = wx.ID_ANY,
+        pos: wx.Point = wx.DefaultPosition,
+        size: wx.Size = wx.DefaultSize,
         choices=None,
-        style=wx.LB_EXTENDED | wx.LB_NEEDED_SB,
-        validator=wx.DefaultValidator,
-        name="BitList",
+        style: int = wx.LB_EXTENDED | wx.LB_NEEDED_SB,
+        validator: wx.Validator = wx.DefaultValidator,
+        name: str = "BitList",
     ):
         if not choices:
             choices = []
         super().__init__(parent, id, pos, size, choices, style, validator, name)
 
     def GetValue(self):
         return list(self.GetCheckedItems())
@@ -30,22 +31,22 @@
 
     Value = property(GetValue, SetValue)
 
 
 class CodePageBitList(BitList):
     def __init__(
         self,
-        parent,
-        id=wx.ID_ANY,
-        pos=wx.DefaultPosition,
-        size=wx.DefaultSize,
+        parent: wx.Window,
+        id: int = wx.ID_ANY,
+        pos: wx.Point = wx.DefaultPosition,
+        size: wx.Size = wx.DefaultSize,
         choices=None,
-        style=wx.LB_EXTENDED | wx.LB_MULTIPLE | wx.LB_NEEDED_SB,
-        validator=wx.DefaultValidator,
-        name="openTypeOS2CodePageRanges",
+        style: int = wx.LB_EXTENDED | wx.LB_MULTIPLE | wx.LB_NEEDED_SB,
+        validator: wx.Validator = wx.DefaultValidator,
+        name: str = "openTypeOS2CodePageRanges",
     ):
         choices = [
             "Latin 1 (1252)",
             "Latin 2 Eastern Europe (1250)",
             "Cyrillic (1251)",
             "Greek (1253)",
             "Turkish (1254)",
@@ -112,22 +113,22 @@
 
         super().__init__(parent, id, pos, size, choices, style, validator, name)
 
 
 class UnicodeRangeBitList(BitList):
     def __init__(
         self,
-        parent,
-        id=wx.ID_ANY,
-        pos=wx.DefaultPosition,
-        size=wx.DefaultSize,
+        parent: wx.Window,
+        id: int = wx.ID_ANY,
+        pos: wx.Point = wx.DefaultPosition,
+        size: wx.Size = wx.DefaultSize,
         choices=None,
         style=wx.LB_EXTENDED | wx.LB_MULTIPLE | wx.LB_NEEDED_SB,
-        validator=wx.DefaultValidator,
-        name="openTypeOS2UnicodeRanges",
+        validator: wx.Validator = wx.DefaultValidator,
+        name: str = "openTypeOS2UnicodeRanges",
     ):
         choices = [
             "Basic Latin",
             "Latin-1 Supplement",
             "Latin Extended-A",
             "Latin Extended-B",
             "IPA Extensions",
@@ -254,24 +255,26 @@
             "Reserved for process-internal usage",
             "Reserved for process-internal usage",
             "Reserved for process-internal usage",
         ]
 
         super().__init__(parent, id, pos, size, choices, style, validator, name)
 
+
 class BlueListCtrl(wx.ListCtrl, ListCtrlAutoWidthMixin, TextEditMixin):
     maxItems = 7
+
     def __init__(
         self,
-        parent,
-        id=wx.ID_ANY,
-        pos=wx.DefaultPosition,
-        size=wx.DefaultSize,
-        style=wx.LC_REPORT | wx.LC_VIRTUAL,
-        name="BlueListCtrl",
+        parent: wx.Window,
+        id: int = wx.ID_ANY,
+        pos: wx.Point = wx.DefaultPosition,
+        size: wx.Size = wx.DefaultSize,
+        style: int = wx.LC_REPORT | wx.LC_VIRTUAL,
+        name: str = "BlueListCtrl",
     ):
         wx.ListCtrl.__init__(self, parent, id, pos, size, style, name=name)
         self._font = None
         ListCtrlAutoWidthMixin.__init__(self)
         self.InsertColumn(0, "Top")
         self.InsertColumn(1, "Bottom")
         self.InsertColumn(2, "Width")
```

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/view/font/fontInfoEmbeddingUI.py` & `wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoEmbeddingUI.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 ###########################################################################
 ## Python code generated with wxFormBuilder (version 3.10.1-0-g8feb16b3)
 ## http://www.wxformbuilder.org/
 ##
 ## PLEASE DO *NOT* EDIT THIS FILE!
 ###########################################################################
 
+from .fontInfoBase import FontInfoBasePage
 import wx
 import wx.xrc
 
 ###########################################################################
 ## Class FontInfoEmbeddingUI
 ###########################################################################
 
-class FontInfoEmbeddingUI ( wx.ScrolledWindow ):
+class FontInfoEmbeddingUI ( FontInfoBasePage ):
 
-    def __init__( self, parent, id = wx.ID_ANY, pos = wx.DefaultPosition, size = wx.Size( -1,-1 ), style = wx.HSCROLL|wx.VSCROLL, name = wx.EmptyString ):
-        wx.ScrolledWindow.__init__ ( self, parent, id = id, pos = pos, size = size, style = style, name = name )
+    def __init__( self, parent, id = wx.ID_ANY, pos = wx.DefaultPosition, size = wx.Size( -1,-1 ), style = 0, name = u"FontInfoEmbedding" ):
+        FontInfoBasePage.__init__ ( self, parent, id = id, pos = pos, size = size, style = style, name = name )
 
-        self.SetExtraStyle( wx.WS_EX_VALIDATE_RECURSIVELY )
         self.SetBackgroundColour( wx.SystemSettings.GetColour( wx.SYS_COLOUR_WINDOW ) )
 
         sizerMain = wx.BoxSizer( wx.VERTICAL )
 
         boxEmbedding = wx.StaticBoxSizer( wx.StaticBox( self, wx.ID_ANY, u"Embedding" ), wx.VERTICAL )
 
         sizerEmbedding = wx.GridBagSizer( 0, 0 )
```

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/view/font/fontInfoEncodingUI.py` & `wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoEncodingUI.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 ###########################################################################
 ## Python code generated with wxFormBuilder (version 3.10.1-0-g8feb16b3)
 ## http://www.wxformbuilder.org/
 ##
 ## PLEASE DO *NOT* EDIT THIS FILE!
 ###########################################################################
 
+from .fontInfoBase import FontInfoBasePage
 import wx
 import wx.xrc
 
 ###########################################################################
 ## Class FontInfoEncodingUI
 ###########################################################################
 
-class FontInfoEncodingUI ( wx.ScrolledWindow ):
+class FontInfoEncodingUI ( FontInfoBasePage ):
 
-    def __init__( self, parent, id = wx.ID_ANY, pos = wx.DefaultPosition, size = wx.Size( -1,-1 ), style = wx.HSCROLL|wx.VSCROLL, name = wx.EmptyString ):
-        wx.ScrolledWindow.__init__ ( self, parent, id = id, pos = pos, size = size, style = style, name = name )
+    def __init__( self, parent, id = wx.ID_ANY, pos = wx.DefaultPosition, size = wx.Size( -1,-1 ), style = 0, name = u"FontInfoEncoding" ):
+        FontInfoBasePage.__init__ ( self, parent, id = id, pos = pos, size = size, style = style, name = name )
 
-        self.SetExtraStyle( wx.WS_EX_VALIDATE_RECURSIVELY )
         self.SetBackgroundColour( wx.SystemSettings.GetColour( wx.SYS_COLOUR_WINDOW ) )
 
         sizerMain = wx.BoxSizer( wx.VERTICAL )
 
         boxPostScript = wx.StaticBoxSizer( wx.StaticBox( self, wx.ID_ANY, u"PostScript" ), wx.VERTICAL )
 
         sizerPostScript = wx.GridBagSizer( 0, 0 )
```

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/view/font/fontInfoHintingPS.py` & `wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoHintingPS.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,57 @@
+"""
+fontInfoHintingPS
+===============================================================================
 
-import logging
+"""
 
 import wx
 
 from .fontInfoHintingPSUI import FontInfoHintingPSUI
 
-log = logging.getLogger(__name__)
 
 class FontInfoHintingPS(FontInfoHintingPSUI):
     """
     Font Info page for PostScript hinting
     """
+
     def __init__(
         self,
-        parent,
-        id=wx.ID_ANY,
-        pos=wx.DefaultPosition,
-        size=wx.DefaultSize,
-        style=wx.BORDER_NONE | wx.TAB_TRAVERSAL,
+        parent: wx.Window,
+        id: int = wx.ID_ANY,
+        pos: wx.Point = wx.DefaultPosition,
+        size: wx.Size = wx.DefaultSize,
+        style: int = wx.TAB_TRAVERSAL,
+        name: str = "FontInfoHintingPS",
     ):
-        super().__init__(parent, id, pos, size, style, name="FontInfoHintingPS")
-        self.SetScrollRate(5, 5)
+        style = style | wx.BORDER_NONE | wx.TAB_TRAVERSAL | wx.HSCROLL | wx.VSCROLL
+        super().__init__(parent, id, pos, size, style, name)
         self.panel_postscriptBlueValues._maxValueLen = 14
         self.panel_postscriptOtherBlues._maxValueLen = 10
         self.panel_postscriptFamilyBlues._maxValueLen = 14
         self.panel_postscriptFamilyOtherBlues._maxValueLen = 10
 
-    def __repr__(self):
-        return f"<{self.__class__.__name__} of {self.Parent}>"
-
     def on_button_copy_localZones(self, event):
         self.panel_postscriptFamilyBlues.Value = self.panel_postscriptBlueValues.Value
-        self.panel_postscriptFamilyOtherBlues.Value = self.panel_postscriptOtherBlues.Value
+        self.panel_postscriptFamilyOtherBlues.Value = (
+            self.panel_postscriptOtherBlues.Value
+        )
 
     def on_button_copy_familyZones(self, event):
         from ... import AllFonts, SelectFonts
+
         fonts = [f for f in AllFonts() if f != self.Parent.font]
-        selectedFonts = SelectFonts("Select fonts to copy family zones to", "Copy Family Zones", fonts)
+        selectedFonts = SelectFonts(
+            "Select fonts to copy family zones to", "Copy Family Zones", fonts
+        )
         if selectedFonts:
             for font in selectedFonts:
                 info = font.info
                 info.postscriptFamilyBlues = self.panel_postscriptFamilyBlues.Value
-                info.postscriptFamilyOtherBlues = self.panel_postscriptFamilyOtherBlues.Value
+                info.postscriptFamilyOtherBlues = (
+                    self.panel_postscriptFamilyOtherBlues.Value
+                )
 
     def onUpdate_button_copy_familyZones(self, event):
         from ... import AllFonts
+
         event.Enable(len(AllFonts()) > 1)
```

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/view/font/fontInfoHintingPSUI.py` & `wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoHintingPSUI.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # -*- coding: utf-8 -*-
 
 ###########################################################################
-## Python code generated with wxFormBuilder (version 3.10.0-4761b0c)
+## Python code generated with wxFormBuilder (version 3.10.1-0-g8feb16b3)
 ## http://www.wxformbuilder.org/
 ##
 ## PLEASE DO *NOT* EDIT THIS FILE!
 ###########################################################################
 
 from .hintPSpanel import StemPanel
 from .hintPSpanel import ZonePanel
+from .fontInfoBase import FontInfoBasePage
 import wx
 import wx.xrc
 
 ###########################################################################
 ## Class FontInfoHintingPSUI
 ###########################################################################
 
-class FontInfoHintingPSUI ( wx.ScrolledWindow ):
+class FontInfoHintingPSUI ( FontInfoBasePage ):
 
-    def __init__( self, parent, id = wx.ID_ANY, pos = wx.DefaultPosition, size = wx.Size( 416,486 ), style = wx.HSCROLL|wx.VSCROLL, name = wx.EmptyString ):
-        wx.ScrolledWindow.__init__ ( self, parent, id = id, pos = pos, size = size, style = style, name = name )
+    def __init__( self, parent, id = wx.ID_ANY, pos = wx.DefaultPosition, size = wx.Size( 416,486 ), style = 0, name = u"FontInfoHintingPS" ):
+        FontInfoBasePage.__init__ ( self, parent, id = id, pos = pos, size = size, style = style, name = name )
 
-        self.SetExtraStyle( wx.WS_EX_VALIDATE_RECURSIVELY )
         self.SetBackgroundColour( wx.SystemSettings.GetColour( wx.SYS_COLOUR_WINDOW ) )
 
         sizer = wx.BoxSizer( wx.VERTICAL )
 
         boxMain = wx.StaticBoxSizer( wx.StaticBox( self, wx.ID_ANY, u"Main" ), wx.VERTICAL )
 
         sizerMain = wx.GridBagSizer( 0, 0 )
```

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/view/font/fontInfoHintingUI.py` & `wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoHintingUI.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # -*- coding: utf-8 -*-
 
 ###########################################################################
-## Python code generated with wxFormBuilder (version 3.10.0-4761b0c)
+## Python code generated with wxFormBuilder (version 3.10.1-0-g8feb16b3)
 ## http://www.wxformbuilder.org/
 ##
 ## PLEASE DO *NOT* EDIT THIS FILE!
 ###########################################################################
 
+from .fontInfoBase import FontInfoBasePage
 import wx
 import wx.xrc
 import wx.grid
 
 ###########################################################################
 ## Class FontInfoHintingUI
 ###########################################################################
 
-class FontInfoHintingUI ( wx.ScrolledWindow ):
+class FontInfoHintingUI ( FontInfoBasePage ):
 
-    def __init__( self, parent, id = wx.ID_ANY, pos = wx.DefaultPosition, size = wx.Size( -1,-1 ), style = wx.HSCROLL|wx.VSCROLL, name = wx.EmptyString ):
-        wx.ScrolledWindow.__init__ ( self, parent, id = id, pos = pos, size = size, style = style, name = name )
+    def __init__( self, parent, id = wx.ID_ANY, pos = wx.DefaultPosition, size = wx.Size( -1,-1 ), style = 0, name = u"FontInfoHinting" ):
+        FontInfoBasePage.__init__ ( self, parent, id = id, pos = pos, size = size, style = style, name = name )
 
-        self.SetExtraStyle( wx.WS_EX_VALIDATE_RECURSIVELY )
         self.SetBackgroundColour( wx.SystemSettings.GetColour( wx.SYS_COLOUR_WINDOW ) )
 
         sizerMain = wx.BoxSizer( wx.VERTICAL )
 
         boxHead = wx.StaticBoxSizer( wx.StaticBox( self, wx.ID_ANY, u"OpenType head Table" ), wx.VERTICAL )
 
         sizerHead = wx.GridBagSizer( 0, 0 )
```

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/view/font/fontInfoIdentificationUI.py` & `wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoIdentificationUI.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,25 +3,26 @@
 ###########################################################################
 ## Python code generated with wxFormBuilder (version 3.10.1-0-g8feb16b3)
 ## http://www.wxformbuilder.org/
 ##
 ## PLEASE DO *NOT* EDIT THIS FILE!
 ###########################################################################
 
+from .fontInfoBase import FontInfoBasePage
 import wx
 import wx.xrc
 
 ###########################################################################
 ## Class FontInfoIdentificationUI
 ###########################################################################
 
-class FontInfoIdentificationUI ( wx.ScrolledWindow ):
+class FontInfoIdentificationUI ( FontInfoBasePage ):
 
-	def __init__( self, parent, id = wx.ID_ANY, pos = wx.DefaultPosition, size = wx.Size( 500,438 ), style = wx.TAB_TRAVERSAL, name = wx.EmptyString ):
-		wx.ScrolledWindow.__init__ ( self, parent, id = id, pos = pos, size = size, style = style, name = name )
+	def __init__( self, parent, id = wx.ID_ANY, pos = wx.DefaultPosition, size = wx.Size( 500,438 ), style = 0, name = u"FontInfoIdentification" ):
+		FontInfoBasePage.__init__ ( self, parent, id = id, pos = pos, size = size, style = style, name = name )
 
 		self.SetBackgroundColour( wx.Colour( 255, 255, 255 ) )
 
 		sizer = wx.BoxSizer( wx.VERTICAL )
 
 		boxMain = wx.StaticBoxSizer( wx.StaticBox( self, wx.ID_ANY, u"Main" ), wx.VERTICAL )
```

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/view/font/fontInfoLegalUI.py` & `wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoLegalUI.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 ###########################################################################
 ## Python code generated with wxFormBuilder (version 3.10.1-0-g8feb16b3)
 ## http://www.wxformbuilder.org/
 ##
 ## PLEASE DO *NOT* EDIT THIS FILE!
 ###########################################################################
 
+from .fontInfoBase import FontInfoBasePage
 import wx
 import wx.xrc
 
 ###########################################################################
 ## Class FontInfoLegalUI
 ###########################################################################
 
-class FontInfoLegalUI ( wx.ScrolledWindow ):
+class FontInfoLegalUI ( FontInfoBasePage ):
 
-	def __init__( self, parent, id = wx.ID_ANY, pos = wx.DefaultPosition, size = wx.Size( 500,544 ), style = wx.HSCROLL|wx.TAB_TRAVERSAL|wx.VSCROLL, name = wx.EmptyString ):
-		wx.ScrolledWindow.__init__ ( self, parent, id = id, pos = pos, size = size, style = style, name = name )
+	def __init__( self, parent, id = wx.ID_ANY, pos = wx.DefaultPosition, size = wx.Size( 500,544 ), style = 0, name = u"FontInfoLegal" ):
+		FontInfoBasePage.__init__ ( self, parent, id = id, pos = pos, size = size, style = style, name = name )
 
-		self.SetExtraStyle( wx.WS_EX_VALIDATE_RECURSIVELY )
 		self.SetBackgroundColour( wx.Colour( 255, 255, 255 ) )
 
 		sizer = wx.BoxSizer( wx.VERTICAL )
 
 		boxMain = wx.StaticBoxSizer( wx.StaticBox( self, wx.ID_ANY, u"Main" ), wx.VERTICAL )
 
 		gridMain = wx.FlexGridSizer( 0, 2, 0, 0 )
```

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/view/font/fontInfoLineUI.py` & `wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoLineUI.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # -*- coding: utf-8 -*-
 
 ###########################################################################
-## Python code generated with wxFormBuilder (version 3.10.0-4761b0c)
+## Python code generated with wxFormBuilder (version 3.10.1-0-g8feb16b3)
 ## http://www.wxformbuilder.org/
 ##
 ## PLEASE DO *NOT* EDIT THIS FILE!
 ###########################################################################
 
+from .fontInfoBase import FontInfoBasePage
 import wx
 import wx.xrc
 
 ###########################################################################
 ## Class FontInfoLineUI
 ###########################################################################
 
-class FontInfoLineUI ( wx.ScrolledWindow ):
+class FontInfoLineUI ( FontInfoBasePage ):
 
-    def __init__( self, parent, id = wx.ID_ANY, pos = wx.DefaultPosition, size = wx.Size( -1,-1 ), style = wx.HSCROLL|wx.VSCROLL, name = wx.EmptyString ):
-        wx.ScrolledWindow.__init__ ( self, parent, id = id, pos = pos, size = size, style = style, name = name )
+    def __init__( self, parent, id = wx.ID_ANY, pos = wx.DefaultPosition, size = wx.Size( -1,-1 ), style = 0, name = u"FontInfoLine" ):
+        FontInfoBasePage.__init__ ( self, parent, id = id, pos = pos, size = size, style = style, name = name )
 
-        self.SetExtraStyle( wx.WS_EX_VALIDATE_RECURSIVELY )
         self.SetBackgroundColour( wx.SystemSettings.GetColour( wx.SYS_COLOUR_WINDOW ) )
 
         sizerMain = wx.BoxSizer( wx.VERTICAL )
 
         boxPostScript = wx.StaticBoxSizer( wx.StaticBox( self, wx.ID_ANY, u"PostScript" ), wx.VERTICAL )
 
         sizerPostScript = wx.GridBagSizer( 0, 0 )
```

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/view/font/fontInfoMetricUI.py` & `wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoMetricUI.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 ###########################################################################
 ## Python code generated with wxFormBuilder (version 3.10.1-0-g8feb16b3)
 ## http://www.wxformbuilder.org/
 ##
 ## PLEASE DO *NOT* EDIT THIS FILE!
 ###########################################################################
 
+from .fontInfoBase import FontInfoBasePage
 import wx
 import wx.xrc
 
 ###########################################################################
 ## Class FontInfoMetricUI
 ###########################################################################
 
-class FontInfoMetricUI ( wx.ScrolledWindow ):
+class FontInfoMetricUI ( FontInfoBasePage ):
 
-    def __init__( self, parent, id = wx.ID_ANY, pos = wx.DefaultPosition, size = wx.Size( -1,-1 ), style = wx.HSCROLL|wx.VSCROLL, name = wx.EmptyString ):
-        wx.ScrolledWindow.__init__ ( self, parent, id = id, pos = pos, size = size, style = style, name = name )
+    def __init__( self, parent, id = wx.ID_ANY, pos = wx.DefaultPosition, size = wx.Size( -1,-1 ), style = 0, name = u"FontInfoMetric" ):
+        FontInfoBasePage.__init__ ( self, parent, id = id, pos = pos, size = size, style = style, name = name )
 
-        self.SetExtraStyle( wx.WS_EX_VALIDATE_RECURSIVELY )
         self.SetBackgroundColour( wx.Colour( 255, 255, 255 ) )
 
         sizer = wx.BoxSizer( wx.VERTICAL )
 
         boxMain = wx.StaticBoxSizer( wx.StaticBox( self, wx.ID_ANY, u"Main" ), wx.VERTICAL )
 
         gridMain = wx.FlexGridSizer( 0, 2, 0, 0 )
```

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/view/font/fontInfoNameUI.py` & `wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoNameUI.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # -*- coding: utf-8 -*-
 
 ###########################################################################
-## Python code generated with wxFormBuilder (version 3.10.0-4761b0c)
+## Python code generated with wxFormBuilder (version 3.10.1-0-g8feb16b3)
 ## http://www.wxformbuilder.org/
 ##
 ## PLEASE DO *NOT* EDIT THIS FILE!
 ###########################################################################
 
+from .fontInfoBase import FontInfoBasePage
 import wx
 import wx.xrc
 
 ###########################################################################
 ## Class FontInfoNameUI
 ###########################################################################
 
-class FontInfoNameUI ( wx.ScrolledWindow ):
+class FontInfoNameUI ( FontInfoBasePage ):
 
-    def __init__( self, parent, id = wx.ID_ANY, pos = wx.DefaultPosition, size = wx.Size( 437,924 ), style = wx.HSCROLL|wx.TAB_TRAVERSAL|wx.VSCROLL, name = wx.EmptyString ):
-        wx.ScrolledWindow.__init__ ( self, parent, id = id, pos = pos, size = size, style = style, name = name )
+    def __init__( self, parent, id = wx.ID_ANY, pos = wx.DefaultPosition, size = wx.Size( 437,924 ), style = 0, name = u"FontInfoName" ):
+        FontInfoBasePage.__init__ ( self, parent, id = id, pos = pos, size = size, style = style, name = name )
 
-        self.SetExtraStyle( wx.WS_EX_VALIDATE_RECURSIVELY )
         self.SetBackgroundColour( wx.Colour( 255, 255, 255 ) )
 
         sizer = wx.BoxSizer( wx.VERTICAL )
 
         boxMain = wx.StaticBoxSizer( wx.StaticBox( self, wx.ID_ANY, u"Main" ), wx.VERTICAL )
 
         gridMain = wx.FlexGridSizer( 0, 2, 0, 0 )
```

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/view/font/fontInfoNaviagtionPanelUI.py` & `wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoNaviagtionPanelUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/view/font/fontInfoSuperSubscriptUI.py` & `wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoSuperSubscriptUI.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 ###########################################################################
 ## Python code generated with wxFormBuilder (version 3.10.1-0-g8feb16b3)
 ## http://www.wxformbuilder.org/
 ##
 ## PLEASE DO *NOT* EDIT THIS FILE!
 ###########################################################################
 
+from .fontInfoBase import FontInfoBasePage
 import wx
 import wx.xrc
 
 ###########################################################################
 ## Class FontInfoSuperSubscriptUI
 ###########################################################################
 
-class FontInfoSuperSubscriptUI ( wx.ScrolledWindow ):
+class FontInfoSuperSubscriptUI ( FontInfoBasePage ):
 
-	def __init__( self, parent, id = wx.ID_ANY, pos = wx.DefaultPosition, size = wx.Size( -1,-1 ), style = wx.HSCROLL|wx.VSCROLL, name = wx.EmptyString ):
-		wx.ScrolledWindow.__init__ ( self, parent, id = id, pos = pos, size = size, style = style, name = name )
+	def __init__( self, parent, id = wx.ID_ANY, pos = wx.DefaultPosition, size = wx.Size( -1,-1 ), style = 0, name = u"FontInfoSuperSubscript" ):
+		FontInfoBasePage.__init__ ( self, parent, id = id, pos = pos, size = size, style = style, name = name )
 
-		self.SetExtraStyle( wx.WS_EX_VALIDATE_RECURSIVELY )
 		self.SetBackgroundColour( wx.SystemSettings.GetColour( wx.SYS_COLOUR_WINDOW ) )
 
 		sizerMain = wx.BoxSizer( wx.VERTICAL )
 
 		sizerTop = wx.StaticBoxSizer( wx.StaticBox( self, wx.ID_ANY, u"Superscript" ), wx.VERTICAL )
 
 		sizerSuperscript = wx.GridBagSizer( 0, 0 )
```

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/view/font/fontInfoUnicodeUI.py` & `wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoUnicodeUI.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 ## Python code generated with wxFormBuilder (version 3.10.1-0-g8feb16b3)
 ## http://www.wxformbuilder.org/
 ##
 ## PLEASE DO *NOT* EDIT THIS FILE!
 ###########################################################################
 
 from .fontInfoControl import UnicodeRangeBitList
+from .fontInfoBase import FontInfoBasePage
 import wx
 import wx.xrc
 
 ###########################################################################
 ## Class FontInfoUnicodeUI
 ###########################################################################
 
-class FontInfoUnicodeUI ( wx.ScrolledWindow ):
+class FontInfoUnicodeUI ( FontInfoBasePage ):
 
-    def __init__( self, parent, id = wx.ID_ANY, pos = wx.DefaultPosition, size = wx.Size( -1,-1 ), style = wx.HSCROLL|wx.VSCROLL, name = wx.EmptyString ):
-        wx.ScrolledWindow.__init__ ( self, parent, id = id, pos = pos, size = size, style = style, name = name )
+    def __init__( self, parent, id = wx.ID_ANY, pos = wx.DefaultPosition, size = wx.Size( -1,-1 ), style = 0, name = u"FontInfoUnicode" ):
+        FontInfoBasePage.__init__ ( self, parent, id = id, pos = pos, size = size, style = style, name = name )
 
-        self.SetExtraStyle( wx.WS_EX_VALIDATE_RECURSIVELY )
         self.SetBackgroundColour( wx.SystemSettings.GetColour( wx.SYS_COLOUR_WINDOW ) )
 
         sizerMain = wx.BoxSizer( wx.VERTICAL )
 
         boxOS2 = wx.StaticBoxSizer( wx.StaticBox( self, wx.ID_ANY, u"OpenType OS/2 Table" ), wx.VERTICAL )
 
         sizerOS2 = wx.GridBagSizer( 0, 0 )
```

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/view/font/fontInfoValidator.py` & `wbpUFO-0.2.2/Lib/wbpUFO/view/font/fontInfoValidator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,16 @@
+"""
+fontInfoValidator
+===============================================================================
+
+"""
 import logging
 import re
 from string import digits, whitespace
+
 import wx
 from fontTools.ufoLib import (
     fontInfoAttributesVersion3ValueData,
     validateFontInfoVersion3ValueForAttribute,
 )
 
 log = logging.getLogger(__name__)
@@ -50,16 +56,16 @@
 
 class FontInfoTextCtrlValidator(FontInfoBaseValidator):
     def __init__(self, getFontInfo):
         super().__init__(getFontInfo)
         self.Bind(wx.EVT_CHAR, self.on_char)
 
     def _getValueFromControl(self):
-        ctrl = self.GetWindow()
-        value = ctrl.Value
+        ctrl:wx.TextCtrl = self.GetWindow()
+        value:str = ctrl.Value
         if value == wx.EmptyString:
             return None
         valueType = self.valueType
         if valueType == str:
             return value
         elif valueType == int:
             return int(value)
@@ -84,16 +90,16 @@
                 else:
                     return valFloat
         else:
             log.debug("valueType: %r, value: %r", valueType, value)
             raise ValueError(f"Can't get value '{ctrl.Name}' from control'")
 
     def Validate(self, win):
-        ctrl = self.GetWindow()
-        name = ctrl.Name
+        ctrl:wx.TextCtrl = self.GetWindow()
+        name:str = ctrl.Name
         # log.debug("Validate %r for %s", win, name)
         info = self.fontInfo
         if info:
             if hasattr(info, name):
                 try:
                     value = self._getValueFromControl()
                 except ValueError:
@@ -108,16 +114,16 @@
             else:
                 log.debug("name not found in fontInfo during Validate for %s", name)
         else:
             log.debug("No fontInfo during Validate for %s", name)
         return True
 
     def TransferToWindow(self):
-        ctrl = self.GetWindow()
-        name = ctrl.Name
+        ctrl:wx.TextCtrl = self.GetWindow()
+        name:str = ctrl.Name
         info = self.fontInfo
         if info and hasattr(info, name):
             value = getattr(info, name)
             if value is None:
                 ctrl.Value = wx.EmptyString
             elif isinstance(value, str):
                 ctrl.Value = value
@@ -127,16 +133,16 @@
                 except ValueError:
                     return False
         return True
         # log.debug("TransferToWindow: no fontInfo")
         # return False
 
     def TransferFromWindow(self):
-        ctrl = self.GetWindow()
-        name = ctrl.Name
+        ctrl:wx.TextCtrl = self.GetWindow()
+        name:str = ctrl.Name
         info = self.fontInfo
         if info and hasattr(info, name):
             try:
                 setattr(info, name, self._getValueFromControl())
                 return True
             except ValueError:
                 log.debug("ValueError during TransferFromWindow for %s", name)
@@ -163,51 +169,28 @@
 
 
 class FontInfoIntlistTextCtrlValidator(FontInfoTextCtrlValidator):
     # def __init__(self, getFontInfo):
     #     super().__init__(getFontInfo)
 
     def _getValueFromControl(self):
-        ctrl = self.GetWindow()
-        name = ctrl.Name
+        ctrl:wx.TextCtrl = self.GetWindow()
+        name:str = ctrl.Name
         info = self.fontInfo
         if info and hasattr(info, name):
             value = ctrl.Value
             if value == wx.EmptyString:
                 return []
             else:
                 return [int(v) for v in value.split()]
         raise ValueError(f"Can't get value '{name}' from control'")
 
-    # def Validate(self, win):
-    #     ctrl = self.GetWindow()
-    #     name = ctrl.Name
-    #     log.debug("Validate %r for %s", win, name)
-    #     info = self.fontInfo
-    #     if info:
-    #         if hasattr(info, name):
-    #             try:
-    #                 value = self._getValueFromControl()
-    #             except ValueError:
-    #                 log.debug("ValueError during Validate for %s", name)
-    #                 return False
-    #             if not value :
-    #                 return True
-    #             result = validateFontInfoVersion3ValueForAttribute(name, value)
-    #             log.debug("Validate for for %s returned %r", namer, esult)
-    #             return result
-    #         else:
-    #             log.debug("name not found in fontInfo during Validate for %s", name)
-    #     else:
-    #         log.debug("No fontInfo during Validate for %s", name)
-    #     return True
-
     def TransferToWindow(self):
-        ctrl = self.GetWindow()
-        name = ctrl.Name
+        ctrl:wx.TextCtrl = self.GetWindow()
+        name:str = ctrl.Name
         info = self.fontInfo
         if info and hasattr(info, name):
             value = getattr(info, name)
             if value is None:
                 ctrl.Value = wx.EmptyString
             elif isinstance(value, (list, tuple)):
                 if not value:
@@ -228,38 +211,37 @@
             return
         if not wx.Validator.IsSilent():
             wx.Bell()
         return
 
 
 class FontInfoPShintCtrlValidator(FontInfoBaseValidator):
-
     def _getValueFromControl(self):
         ctrl = self.GetWindow()
         value = ctrl.Value
         if value:
             return value
 
     def TransferToWindow(self):
         ctrl = self.GetWindow()
-        name = ctrl.Name
+        name:str = ctrl.Name
         info = self.fontInfo
         if info and hasattr(info, name):
             value = getattr(info, name)
             if value is None:
                 ctrl.Value = []
             elif isinstance(value, (list, tuple)):
                 ctrl.Value = value
             else:
                 return False
         return True
 
     def TransferFromWindow(self):
         ctrl = self.GetWindow()
-        name = ctrl.Name
+        name:str = ctrl.Name
         info = self.fontInfo
         if info and hasattr(info, name):
             oldValue = getattr(info, name)
             newValue = self._getValueFromControl()
             if newValue != oldValue:
                 try:
                     setattr(info, name, newValue)
@@ -285,16 +267,16 @@
                     attribute, __ = name.split(" ", 1)
                 else:
                     attribute = name
                 self._valueType = fontInfoAttributesVersion3ValueData[attribute]["type"]
         return self._valueType
 
     def TransferToWindow(self):
-        ctrl = self.GetWindow()
-        name = ctrl.Name
+        ctrl:wx.CheckBox = self.GetWindow()
+        name:str = ctrl.Name
         info = self.fontInfo
         if info:
             if self.flagsPattern.match(name):
                 attribute, value = name.split(" ", 1)
                 value = int(value)
                 if hasattr(info, attribute):
                     # log.debug(
```

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/view/font/glyphGrid.py` & `wbpUFO-0.2.2/Lib/wbpUFO/view/font/glyphGrid.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,22 @@
+"""
+glyphGrid
+===============================================================================
+
+"""
 import logging
 import os
 import pickle
 from math import sqrt
 
 import wx
 from defcon import registerRepresentationFactory
 from fontTools.misc.transform import Transform
 from fontTools.pens.boundsPen import ControlBoundsPen
 from fontTools.pens.transformPen import TransformPen
-
-# from wbBase.tools import MacroMenu
 from wbBase.scripting import MacroMenu
 from wbDefcon import Font, Glyph
 from wbDefcon.pens import graphicsPen
 from wbDefcon.tools.glyph import deleteGlyph, getSaveKeepName, renameGlyph
 
 from ...control.glyphGridStatusPanelUI import GlyphGridStatusPanelUI
 from ...dialog.deleteGlyphsDialog import DeleteGlyphsDialog
```

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/view/font/groups.py` & `wbpUFO-0.2.2/Lib/wbpUFO/view/font/groups.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,19 @@
+"""
+groups
+===============================================================================
+
+"""
 import pickle
 
 import wx
 import wx.grid as gridlib
-from wx.lib.mixins.listctrl import ListCtrlAutoWidthMixin, TextEditMixin
-
-from wbDefcon import Font
 from wbBase.scripting import MacroButtonMixin
+from wbDefcon import Font
+from wx.lib.mixins.listctrl import ListCtrlAutoWidthMixin, TextEditMixin
 
 from .groupsStatusPanelUI import GroupsStatusPanelUI
 
 
 class GroupsListDropTarget(wx.DropTarget):
     """
     DropTarget for GroupsListCtrl
@@ -345,15 +349,15 @@
 
     @property
     def font(self):
         """The wbDefcon Font object of this GroupsPage"""
         return self._font
 
     @font.setter
-    def font(self, value:Font):
+    def font(self, value: Font):
         assert self._font is None
         assert isinstance(value, Font)
         assert value == self.Parent.font
         self._font = value
         self.groupsListCtrl.font = value
         self._font.groups.addObserver(
             self,
```

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/view/font/groupsStatusPanelUI.py` & `wbpUFO-0.2.2/Lib/wbpUFO/view/font/groupsStatusPanelUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/view/font/hintPSlistCtrl.py` & `wbpUFO-0.2.2/Lib/wbpUFO/view/font/hintPSlistCtrl.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+"""
+hintPSlistCtrl
+===============================================================================
+
+"""
 import wx
 
 
 class ZoneListCtrl(wx.ListCtrl):
     def __init__(
         self,
         parent,
```

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/view/font/hintPSpanel.py` & `wbpUFO-0.2.2/Lib/wbpUFO/view/font/hintPSpanel.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,23 @@
+"""
+hintPSpanel
+===============================================================================
+
+"""
 import logging
 from string import digits
 
 import wx
 
-from .zonePanelUI import ZonePanelUI
 from .stemPanelUI import StemPanelUI
+from .zonePanelUI import ZonePanelUI
 
 log = logging.getLogger(__name__)
 
+
 class NumberValidator(wx.Validator):
     def __init__(self):
         super().__init__()
         self._validChars = digits + ".+-"
         self.Bind(wx.EVT_CHAR, self.OnChar)
 
     def Clone(self):
@@ -49,20 +55,20 @@
     def TransferFromWindow(self):
         return True
 
 
 class ZonePanel(ZonePanelUI):
     def __init__(
         self,
-        parent,
-        id=wx.ID_ANY,
-        pos=wx.DefaultPosition,
-        size=wx.DefaultSize,
-        style=wx.BORDER_NONE | wx.TAB_TRAVERSAL,
-        name=wx.EmptyString,
+        parent: wx.Window,
+        id: int = wx.ID_ANY,
+        pos: wx.Point = wx.DefaultPosition,
+        size: wx.Size = wx.DefaultSize,
+        style:int=wx.BORDER_NONE | wx.TAB_TRAVERSAL,
+        name: str = wx.EmptyString,
     ):
         ZonePanelUI.__init__(
             self, parent, id=id, pos=pos, size=size, style=style, name=name
         )
         self._value = []
         self._maxValueLen = 0
         self._newZone = False
@@ -150,20 +156,20 @@
     def onUpdate_button_remove(self, event):
         event.Enable(self.listCtrl_zone.SelectedItemCount > 0)
 
 
 class StemPanel(StemPanelUI):
     def __init__(
         self,
-        parent,
-        id=wx.ID_ANY,
-        pos=wx.DefaultPosition,
-        size=wx.DefaultSize,
-        style=wx.BORDER_NONE | wx.TAB_TRAVERSAL,
-        name=wx.EmptyString,
+        parent: wx.Window,
+        id: int = wx.ID_ANY,
+        pos: wx.Point = wx.DefaultPosition,
+        size: wx.Size = wx.DefaultSize,
+        style:int=wx.BORDER_NONE | wx.TAB_TRAVERSAL,
+        name: str = wx.EmptyString,
     ):
         StemPanelUI.__init__(
             self, parent, id=id, pos=pos, size=size, style=style, name=name
         )
         self._value = []
         self._maxValueLen = 12
         self._newStem = False
@@ -228,8 +234,7 @@
         stems = self.Value[:]
         idx = self.listCtrl_stem.FocusedItem
         del stems[idx]
         self.Value = stems
 
     def onUpdate_button_remove(self, event):
         event.Enable(self.listCtrl_stem.SelectedItemCount > 0)
-
```

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/view/font/info.py` & `wbpUFO-0.2.2/Lib/wbpUFO/view/font/info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 """
+info
+===============================================================================
+
 Font Info
 """
+from __future__ import annotations
 import logging
 import re
 
 import wx
 from fontTools.ufoLib import fontInfoAttributesVersion3ValueData
 from wbDefcon import Font, Info
 from wbBase.scripting import MacroButtonMixin
@@ -81,15 +85,15 @@
         itemID = self.AppendItem(hintingID, "PostScript Hinting", data=13)
         itemID = self.AppendItem(self.root, "Note", data=14)
         itemID = self.AppendItem(self.root, "Lib", data=15)
         self.Bind(wx.EVT_TREE_SEL_CHANGED, self.on_selectionChanged)
         self.Bind(wx.EVT_TREE_SEL_CHANGING, self.on_selectionChanging)
 
     @property
-    def infoBookCtrl(self):
+    def infoBookCtrl(self) -> InfoBookCtrl:
         return self.GrandParent.infoBookCtrl
 
     def on_selectionChanged(self, event):
         if self:
             pageNum = self.GetItemData(event.Item)
             self.infoBookCtrl.ChangeSelection(pageNum)
             self.infoBookCtrl.CurrentPage.TransferDataToWindow()
@@ -219,15 +223,15 @@
                 else:
                     control.Validator = FontInfoTextCtrlValidator(self.getFontInfo)
                     if valueType in (int, float, (int, float), (float, int)):
                         control.WindowStyle |= wx.TE_RIGHT
                     control.WindowStyle |= wx.TE_NOHIDESEL
                     if control.IsSingleLine():
                         control.SetHint("None")
-            elif isinstance(control, wx.CheckBox):
+            elif isinstance(control, (wx.CheckBox, wx.RadioButton)):
                 control.Validator = FontInfoCheckBoxValidator(self.getFontInfo)
             elif isinstance(control, BitList):
                 control.Validator = FontInfoBitListValidator(self.getFontInfo)
             elif isinstance(control, (ZonePanel, StemPanel)):
                 control.Validator = FontInfoPShintCtrlValidator(self.getFontInfo)
 
     def _bindControlEvents(self):
@@ -269,15 +273,16 @@
     def on_controlKillFocus(self, event):
         log.debug("on_controlKillFocus %r", event.EventObject.Name)
         control = event.EventObject
         if control.Validator and control.Validator.Validate(control.Parent):
             log.debug("%r valid", event.EventObject.Name)
             control.Validator.TransferFromWindow()
         else:
-            control.SelectAll()
+            if hasattr(control, "SelectAll"):
+                control.SelectAll()
             wx.CallAfter(control.SetFocus)
         event.Skip()
 
 
 class FontInfoNaviagtionPanel(FontInfoNaviagtionPanelUI, MacroButtonMixin):
     """
     Naviagtion Panel of InfoPage
```

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/view/font/kerning.py` & `wbpUFO-0.2.2/Lib/wbpUFO/view/font/kerning.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,27 @@
+"""
+kerning
+===============================================================================
+
+"""
 from __future__ import annotations
+
 import logging
-from typing import Optional, Tuple, TYPE_CHECKING
+from typing import TYPE_CHECKING, Optional, Tuple
 
 import wx
 import wx.grid as gridlib
-from wbDefcon import Font
 from wbBase.scripting import MacroButtonMixin
+from wbDefcon import Font
 
 from .kerningStatusPanelUI import KerningStatusPanelUI
 
 if TYPE_CHECKING:
     from wbDefcon import Kerning
+
     from ..fontinfo import UfoFontInfoWindow
 
 log = logging.getLogger(__name__)
 
 
 class KerningStatusPanel(KerningStatusPanelUI, MacroButtonMixin):
     def __init__(
```

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/view/font/kerningStatusPanelUI.py` & `wbpUFO-0.2.2/Lib/wbpUFO/view/font/kerningStatusPanelUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/view/font/stemPanelUI.py` & `wbpUFO-0.2.2/Lib/wbpUFO/view/font/stemPanelUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/view/font/zonePanelUI.py` & `wbpUFO-0.2.2/Lib/wbpUFO/view/font/zonePanelUI.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO/view/glyph.py` & `wbpUFO-0.2.2/Lib/wbpUFO/view/glyph.py`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO.egg-info/PKG-INFO` & `wbpUFO-0.2.2/Lib/wbpUFO.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wbpUFO
-Version: 0.2.1
+Version: 0.2.2
 Summary: FontTools font editor for Workbench applications.
 Home-page: https://gitlab.com/workbench2/workbench-plugins/wbpUFO
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/workbench-plugins/wbpUFO
 Project-URL: Documentation, https://workbench2.gitlab.io/workbench-plugins/wbpUFO
 Project-URL: Tracker, https://gitlab.com/workbench2/workbench-plugins/wbpUFO/-/issues
```

### Comparing `wbpUFO-0.2.1/Lib/wbpUFO.egg-info/SOURCES.txt` & `wbpUFO-0.2.2/Lib/wbpUFO.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -100,14 +100,15 @@
 Lib/wbpUFO/toolbar/glyphShow.py
 Lib/wbpUFO/toolbar/layer.py
 Lib/wbpUFO/toolbar/markColor.py
 Lib/wbpUFO/view/__init__.py
 Lib/wbpUFO/view/glyph.py
 Lib/wbpUFO/view/font/__init__.py
 Lib/wbpUFO/view/font/feature.py
+Lib/wbpUFO/view/font/fontInfoBase.py
 Lib/wbpUFO/view/font/fontInfoCaret.py
 Lib/wbpUFO/view/font/fontInfoCaretUI.py
 Lib/wbpUFO/view/font/fontInfoClassification.py
 Lib/wbpUFO/view/font/fontInfoClassificationUI.py
 Lib/wbpUFO/view/font/fontInfoCodepage.py
 Lib/wbpUFO/view/font/fontInfoCodepageUI.py
 Lib/wbpUFO/view/font/fontInfoControl.py
```

### Comparing `wbpUFO-0.2.1/PKG-INFO` & `wbpUFO-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wbpUFO
-Version: 0.2.1
+Version: 0.2.2
 Summary: FontTools font editor for Workbench applications.
 Home-page: https://gitlab.com/workbench2/workbench-plugins/wbpUFO
 Author: Andreas Eigendorf
 License: MIT
 Project-URL: Source, https://gitlab.com/workbench2/workbench-plugins/wbpUFO
 Project-URL: Documentation, https://workbench2.gitlab.io/workbench-plugins/wbpUFO
 Project-URL: Tracker, https://gitlab.com/workbench2/workbench-plugins/wbpUFO/-/issues
```

### Comparing `wbpUFO-0.2.1/README.md` & `wbpUFO-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `wbpUFO-0.2.1/setup.cfg` & `wbpUFO-0.2.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.2.1
+current_version = 0.2.2
 commit = True
 tag = True
 tag_name = {new_version}
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)?
 serialize = 
 	{major}.{minor}.{patch}
```

