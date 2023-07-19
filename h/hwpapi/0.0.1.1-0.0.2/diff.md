# Comparing `tmp/hwpapi-0.0.1.1-py3-none-win_amd64.whl.zip` & `tmp/hwpapi-0.0.2-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,25 @@
-Zip file size: 117508 bytes, number of entries: 21
+Zip file size: 125043 bytes, number of entries: 23
 -rw-rw-rw-  2.0 fat   217229 b- defN 07-Jan-09 10:22 hwpapi/FilePathCheckerModuleExample.dll
--rw-rw-rw-  2.0 fat       23 b- defN 23-May-22 13:14 hwpapi/__init__.py
--rw-rw-rw-  2.0 fat     6531 b- defN 23-May-22 13:14 hwpapi/_modidx.py
--rw-rw-rw-  2.0 fat    61638 b- defN 23-May-22 13:14 hwpapi/actions.py
--rw-rw-rw-  2.0 fat    31561 b- defN 23-May-22 13:14 hwpapi/core.py
--rw-rw-rw-  2.0 fat    11113 b- defN 23-May-22 13:14 hwpapi/functions.py
+-rw-rw-rw-  2.0 fat       25 b- defN 23-Jul-19 04:32 hwpapi/__init__.py
+-rw-rw-rw-  2.0 fat    26411 b- defN 23-Jul-19 04:32 hwpapi/_modidx.py
+-rw-rw-rw-  2.0 fat    61804 b- defN 23-Jul-19 04:32 hwpapi/actions.py
+-rw-rw-rw-  2.0 fat    10305 b- defN 23-Jul-19 04:32 hwpapi/constants.py
+-rw-rw-rw-  2.0 fat    31136 b- defN 23-Jul-19 04:32 hwpapi/core.py
+-rw-rw-rw-  2.0 fat    25341 b- defN 23-Jul-19 04:32 hwpapi/dataclasses.py
+-rw-rw-rw-  2.0 fat    10260 b- defN 23-Jul-19 04:32 hwpapi/functions.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-17 05:40 nbs/__init__.py
 -rw-rw-rw-  2.0 fat    55657 b- defN 23-Feb-17 05:34 nbs/action_info.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-17 05:40 ~bs/__init__.py
 -rw-rw-rw-  2.0 fat       23 b- defN 23-Apr-19 03:28 ~wpapi/__init__.py
 -rw-rw-rw-  2.0 fat     5485 b- defN 23-Apr-19 03:28 ~wpapi/_modidx.py
 -rw-rw-rw-  2.0 fat    58407 b- defN 23-Apr-19 03:28 ~wpapi/actions.py
 -rw-rw-rw-  2.0 fat    22744 b- defN 23-Apr-19 03:28 ~wpapi/core.py
 -rw-rw-rw-  2.0 fat     7026 b- defN 23-Apr-19 03:28 ~wpapi/functions.py
 -rw-rw-rw-  2.0 fat      409 b- defN 23-Mar-21 04:57 ~wpapi/methods.py
--rw-rw-rw-  2.0 fat     1087 b- defN 23-May-22 14:19 hwpapi-0.0.1.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3892 b- defN 23-May-22 14:19 hwpapi-0.0.1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       98 b- defN 23-May-22 14:19 hwpapi-0.0.1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       55 b- defN 23-May-22 14:19 hwpapi-0.0.1.1.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       22 b- defN 23-May-22 14:19 hwpapi-0.0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1613 b- defN 23-May-22 14:19 hwpapi-0.0.1.1.dist-info/RECORD
-21 files, 484613 bytes uncompressed, 114932 bytes compressed:  76.3%
+-rw-rw-rw-  2.0 fat     1087 b- defN 23-Jul-19 08:19 hwpapi-0.0.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3890 b- defN 23-Jul-19 08:19 hwpapi-0.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       98 b- defN 23-Jul-19 08:19 hwpapi-0.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       55 b- defN 23-Jul-19 08:19 hwpapi-0.0.2.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Jul-19 08:19 hwpapi-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1758 b- defN 23-Jul-19 08:19 hwpapi-0.0.2.dist-info/RECORD
+23 files, 539161 bytes uncompressed, 122259 bytes compressed:  77.3%
```

## zipnote {}

```diff
@@ -6,17 +6,23 @@
 
 Filename: hwpapi/_modidx.py
 Comment: 
 
 Filename: hwpapi/actions.py
 Comment: 
 
+Filename: hwpapi/constants.py
+Comment: 
+
 Filename: hwpapi/core.py
 Comment: 
 
+Filename: hwpapi/dataclasses.py
+Comment: 
+
 Filename: hwpapi/functions.py
 Comment: 
 
 Filename: nbs/__init__.py
 Comment: 
 
 Filename: nbs/action_info.py
@@ -39,26 +45,26 @@
 
 Filename: ~wpapi/functions.py
 Comment: 
 
 Filename: ~wpapi/methods.py
 Comment: 
 
-Filename: hwpapi-0.0.1.1.dist-info/LICENSE
+Filename: hwpapi-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: hwpapi-0.0.1.1.dist-info/METADATA
+Filename: hwpapi-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: hwpapi-0.0.1.1.dist-info/WHEEL
+Filename: hwpapi-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: hwpapi-0.0.1.1.dist-info/entry_points.txt
+Filename: hwpapi-0.0.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: hwpapi-0.0.1.1.dist-info/top_level.txt
+Filename: hwpapi-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: hwpapi-0.0.1.1.dist-info/RECORD
+Filename: hwpapi-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hwpapi/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "0.0.1"
+__version__ = "0.0.1.1"
```

## hwpapi/_modidx.py

```diff
@@ -11,50 +11,215 @@
                                 'hwpapi.actions._Action.get_pset': ('02_api/actions.html#_action.get_pset', 'hwpapi/actions.py'),
                                 'hwpapi.actions._Action.run': ('02_api/actions.html#_action.run', 'hwpapi/actions.py'),
                                 'hwpapi.actions._Action.set_parameter': ('02_api/actions.html#_action.set_parameter', 'hwpapi/actions.py'),
                                 'hwpapi.actions._Actions': ('02_api/actions.html#_actions', 'hwpapi/actions.py'),
                                 'hwpapi.actions._Actions.__dir__': ('02_api/actions.html#_actions.__dir__', 'hwpapi/actions.py'),
                                 'hwpapi.actions._Actions.__getattr__': ('02_api/actions.html#_actions.__getattr__', 'hwpapi/actions.py'),
                                 'hwpapi.actions._Actions.__init__': ('02_api/actions.html#_actions.__init__', 'hwpapi/actions.py')},
+            'hwpapi.constants': {},
             'hwpapi.core': { 'hwpapi.core.App': ('02_api/core.html#app', 'hwpapi/core.py'),
                              'hwpapi.core.App.__init__': ('02_api/core.html#app.__init__', 'hwpapi/core.py'),
                              'hwpapi.core.App.__str__': ('02_api/core.html#app.__str__', 'hwpapi/core.py'),
                              'hwpapi.core.App.close': ('02_api/core.html#app.close', 'hwpapi/core.py'),
                              'hwpapi.core.App.create_action': ('02_api/core.html#app.create_action', 'hwpapi/core.py'),
                              'hwpapi.core.App.create_parameterset': ('02_api/core.html#app.create_parameterset', 'hwpapi/core.py'),
                              'hwpapi.core.App.find_text': ('02_api/core.html#app.find_text', 'hwpapi/core.py'),
+                             'hwpapi.core.App.get_charshape': ('02_api/core.html#app.get_charshape', 'hwpapi/core.py'),
                              'hwpapi.core.App.get_filepath': ('02_api/core.html#app.get_filepath', 'hwpapi/core.py'),
+                             'hwpapi.core.App.get_hwnd': ('02_api/core.html#app.get_hwnd', 'hwpapi/core.py'),
+                             'hwpapi.core.App.get_parashape': ('02_api/core.html#app.get_parashape', 'hwpapi/core.py'),
                              'hwpapi.core.App.get_selected_text': ('02_api/core.html#app.get_selected_text', 'hwpapi/core.py'),
                              'hwpapi.core.App.get_text': ('02_api/core.html#app.get_text', 'hwpapi/core.py'),
                              'hwpapi.core.App.insert_file': ('02_api/core.html#app.insert_file', 'hwpapi/core.py'),
                              'hwpapi.core.App.insert_picture': ('02_api/core.html#app.insert_picture', 'hwpapi/core.py'),
                              'hwpapi.core.App.insert_text': ('02_api/core.html#app.insert_text', 'hwpapi/core.py'),
                              'hwpapi.core.App.move': ('02_api/core.html#app.move', 'hwpapi/core.py'),
                              'hwpapi.core.App.open': ('02_api/core.html#app.open', 'hwpapi/core.py'),
                              'hwpapi.core.App.quit': ('02_api/core.html#app.quit', 'hwpapi/core.py'),
                              'hwpapi.core.App.reload': ('02_api/core.html#app.reload', 'hwpapi/core.py'),
                              'hwpapi.core.App.replace_all': ('02_api/core.html#app.replace_all', 'hwpapi/core.py'),
                              'hwpapi.core.App.save': ('02_api/core.html#app.save', 'hwpapi/core.py'),
+                             'hwpapi.core.App.save_block': ('02_api/core.html#app.save_block', 'hwpapi/core.py'),
                              'hwpapi.core.App.scan': ('02_api/core.html#app.scan', 'hwpapi/core.py'),
                              'hwpapi.core.App.select_text': ('02_api/core.html#app.select_text', 'hwpapi/core.py'),
                              'hwpapi.core.App.set_cell_border': ('02_api/core.html#app.set_cell_border', 'hwpapi/core.py'),
                              'hwpapi.core.App.set_cell_color': ('02_api/core.html#app.set_cell_color', 'hwpapi/core.py'),
                              'hwpapi.core.App.set_charshape': ('02_api/core.html#app.set_charshape', 'hwpapi/core.py'),
                              'hwpapi.core.App.set_parashape': ('02_api/core.html#app.set_parashape', 'hwpapi/core.py'),
                              'hwpapi.core.App.set_visible': ('02_api/core.html#app.set_visible', 'hwpapi/core.py'),
+                             'hwpapi.core.App.setup_page': ('02_api/core.html#app.setup_page', 'hwpapi/core.py'),
                              'hwpapi.core._get_text': ('02_api/core.html#_get_text', 'hwpapi/core.py'),
                              'hwpapi.core.move_to_line': ('02_api/core.html#move_to_line', 'hwpapi/core.py')},
+            'hwpapi.dataclasses': { 'hwpapi.dataclasses.CharShape': ('02_api/dataclasses.html#charshape', 'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.CharShape.__init__': ( '02_api/dataclasses.html#charshape.__init__',
+                                                                               'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.CharShape.__repr__': ( '02_api/dataclasses.html#charshape.__repr__',
+                                                                               'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.CharShape.__str__': ( '02_api/dataclasses.html#charshape.__str__',
+                                                                              'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.CharShape._get_font': ( '02_api/dataclasses.html#charshape._get_font',
+                                                                                'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.CharShape._set_font': ( '02_api/dataclasses.html#charshape._set_font',
+                                                                                'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.CharShape.bold': ( '02_api/dataclasses.html#charshape.bold',
+                                                                           'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.CharShape.font': ( '02_api/dataclasses.html#charshape.font',
+                                                                           'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.CharShape.fontsize': ( '02_api/dataclasses.html#charshape.fontsize',
+                                                                               'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.CharShape.fromdict': ( '02_api/dataclasses.html#charshape.fromdict',
+                                                                               'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.CharShape.get_from_pset': ( '02_api/dataclasses.html#charshape.get_from_pset',
+                                                                                    'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.CharShape.hangul_font': ( '02_api/dataclasses.html#charshape.hangul_font',
+                                                                                  'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.CharShape.hanja_font': ( '02_api/dataclasses.html#charshape.hanja_font',
+                                                                                 'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.CharShape.italic': ( '02_api/dataclasses.html#charshape.italic',
+                                                                             'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.CharShape.japanese_font': ( '02_api/dataclasses.html#charshape.japanese_font',
+                                                                                    'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.CharShape.latin_font': ( '02_api/dataclasses.html#charshape.latin_font',
+                                                                                 'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.CharShape.offset': ( '02_api/dataclasses.html#charshape.offset',
+                                                                             'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.CharShape.other_font': ( '02_api/dataclasses.html#charshape.other_font',
+                                                                                 'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.CharShape.out_line_type': ( '02_api/dataclasses.html#charshape.out_line_type',
+                                                                                    'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.CharShape.ratio': ( '02_api/dataclasses.html#charshape.ratio',
+                                                                            'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.CharShape.shade_color': ( '02_api/dataclasses.html#charshape.shade_color',
+                                                                                  'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.CharShape.shadow_color': ( '02_api/dataclasses.html#charshape.shadow_color',
+                                                                                   'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.CharShape.shadow_offset_x': ( '02_api/dataclasses.html#charshape.shadow_offset_x',
+                                                                                      'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.CharShape.shadow_offset_y': ( '02_api/dataclasses.html#charshape.shadow_offset_y',
+                                                                                      'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.CharShape.shadow_type': ( '02_api/dataclasses.html#charshape.shadow_type',
+                                                                                  'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.CharShape.spacing': ( '02_api/dataclasses.html#charshape.spacing',
+                                                                              'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.CharShape.strike_out_color': ( '02_api/dataclasses.html#charshape.strike_out_color',
+                                                                                       'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.CharShape.strike_out_type': ( '02_api/dataclasses.html#charshape.strike_out_type',
+                                                                                      'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.CharShape.sub_script': ( '02_api/dataclasses.html#charshape.sub_script',
+                                                                                 'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.CharShape.super_script': ( '02_api/dataclasses.html#charshape.super_script',
+                                                                                   'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.CharShape.symbol_font': ( '02_api/dataclasses.html#charshape.symbol_font',
+                                                                                  'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.CharShape.text_color': ( '02_api/dataclasses.html#charshape.text_color',
+                                                                                 'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.CharShape.todict': ( '02_api/dataclasses.html#charshape.todict',
+                                                                             'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.CharShape.underline_color': ( '02_api/dataclasses.html#charshape.underline_color',
+                                                                                      'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.CharShape.underline_shape': ( '02_api/dataclasses.html#charshape.underline_shape',
+                                                                                      'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.CharShape.underline_type': ( '02_api/dataclasses.html#charshape.underline_type',
+                                                                                     'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.CharShape.user_font': ( '02_api/dataclasses.html#charshape.user_font',
+                                                                                'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.Character': ('02_api/dataclasses.html#character', 'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.PageShape': ('02_api/dataclasses.html#pageshape', 'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.ParaShape': ('02_api/dataclasses.html#parashape', 'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.ParaShape.__init__': ( '02_api/dataclasses.html#parashape.__init__',
+                                                                               'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.ParaShape.__repr__': ( '02_api/dataclasses.html#parashape.__repr__',
+                                                                               'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.ParaShape.__str__': ( '02_api/dataclasses.html#parashape.__str__',
+                                                                              'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.ParaShape.align_type': ( '02_api/dataclasses.html#parashape.align_type',
+                                                                                 'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.ParaShape.border_connect': ( '02_api/dataclasses.html#parashape.border_connect',
+                                                                                     'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.ParaShape.border_offset_bottom': ( '02_api/dataclasses.html#parashape.border_offset_bottom',
+                                                                                           'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.ParaShape.border_offset_left': ( '02_api/dataclasses.html#parashape.border_offset_left',
+                                                                                         'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.ParaShape.border_offset_right': ( '02_api/dataclasses.html#parashape.border_offset_right',
+                                                                                          'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.ParaShape.border_offset_top': ( '02_api/dataclasses.html#parashape.border_offset_top',
+                                                                                        'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.ParaShape.border_text': ( '02_api/dataclasses.html#parashape.border_text',
+                                                                                  'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.ParaShape.break_latin_word': ( '02_api/dataclasses.html#parashape.break_latin_word',
+                                                                                       'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.ParaShape.break_non_latin_word': ( '02_api/dataclasses.html#parashape.break_non_latin_word',
+                                                                                           'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.ParaShape.condense': ( '02_api/dataclasses.html#parashape.condense',
+                                                                               'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.ParaShape.font_line_height': ( '02_api/dataclasses.html#parashape.font_line_height',
+                                                                                       'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.ParaShape.fromdict': ( '02_api/dataclasses.html#parashape.fromdict',
+                                                                               'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.ParaShape.get_from_pset': ( '02_api/dataclasses.html#parashape.get_from_pset',
+                                                                                    'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.ParaShape.heading_type': ( '02_api/dataclasses.html#parashape.heading_type',
+                                                                                   'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.ParaShape.indentation': ( '02_api/dataclasses.html#parashape.indentation',
+                                                                                  'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.ParaShape.keep_with_next': ( '02_api/dataclasses.html#parashape.keep_with_next',
+                                                                                     'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.ParaShape.left_margin': ( '02_api/dataclasses.html#parashape.left_margin',
+                                                                                  'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.ParaShape.level': ( '02_api/dataclasses.html#parashape.level',
+                                                                            'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.ParaShape.line_spacing': ( '02_api/dataclasses.html#parashape.line_spacing',
+                                                                                   'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.ParaShape.line_spacing_type': ( '02_api/dataclasses.html#parashape.line_spacing_type',
+                                                                                        'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.ParaShape.line_wrap': ( '02_api/dataclasses.html#parashape.line_wrap',
+                                                                                'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.ParaShape.next_spacing': ( '02_api/dataclasses.html#parashape.next_spacing',
+                                                                                   'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.ParaShape.page_break_before': ( '02_api/dataclasses.html#parashape.page_break_before',
+                                                                                        'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.ParaShape.prev_spacing': ( '02_api/dataclasses.html#parashape.prev_spacing',
+                                                                                   'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.ParaShape.right_margin': ( '02_api/dataclasses.html#parashape.right_margin',
+                                                                                   'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.ParaShape.snap_to_grid': ( '02_api/dataclasses.html#parashape.snap_to_grid',
+                                                                                   'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.ParaShape.tail_type': ( '02_api/dataclasses.html#parashape.tail_type',
+                                                                                'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.ParaShape.text_alignment': ( '02_api/dataclasses.html#parashape.text_alignment',
+                                                                                     'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.ParaShape.todict': ( '02_api/dataclasses.html#parashape.todict',
+                                                                             'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.ParaShape.widow_orphan': ( '02_api/dataclasses.html#parashape.widow_orphan',
+                                                                                   'hwpapi/dataclasses.py'),
+                                    'hwpapi.dataclasses.Paragraph': ('02_api/dataclasses.html#paragraph', 'hwpapi/dataclasses.py')},
             'hwpapi.functions': { 'hwpapi.functions.add_dll_to_registry': ( '02_api/functions.html#add_dll_to_registry',
                                                                             'hwpapi/functions.py'),
                                   'hwpapi.functions.check_dll': ('02_api/functions.html#check_dll', 'hwpapi/functions.py'),
+                                  'hwpapi.functions.convert2int': ('02_api/functions.html#convert2int', 'hwpapi/functions.py'),
+                                  'hwpapi.functions.convert_hwp_color_to_hex': ( '02_api/functions.html#convert_hwp_color_to_hex',
+                                                                                 'hwpapi/functions.py'),
+                                  'hwpapi.functions.convert_to_hwp_color': ( '02_api/functions.html#convert_to_hwp_color',
+                                                                             'hwpapi/functions.py'),
                                   'hwpapi.functions.dispatch': ('02_api/functions.html#dispatch', 'hwpapi/functions.py'),
                                   'hwpapi.functions.get_absolute_path': ('02_api/functions.html#get_absolute_path', 'hwpapi/functions.py'),
+                                  'hwpapi.functions.get_charshape_pset': ( '02_api/functions.html#get_charshape_pset',
+                                                                           'hwpapi/functions.py'),
                                   'hwpapi.functions.get_dll_path': ('02_api/functions.html#get_dll_path', 'hwpapi/functions.py'),
+                                  'hwpapi.functions.get_font_name': ('02_api/functions.html#get_font_name', 'hwpapi/functions.py'),
+                                  'hwpapi.functions.get_key': ('02_api/functions.html#get_key', 'hwpapi/functions.py'),
+                                  'hwpapi.functions.get_parashape_pset': ( '02_api/functions.html#get_parashape_pset',
+                                                                           'hwpapi/functions.py'),
                                   'hwpapi.functions.get_registry_value': ( '02_api/functions.html#get_registry_value',
                                                                            'hwpapi/functions.py'),
                                   'hwpapi.functions.get_rgb_tuple': ('02_api/functions.html#get_rgb_tuple', 'hwpapi/functions.py'),
                                   'hwpapi.functions.get_value': ('02_api/functions.html#get_value', 'hwpapi/functions.py'),
                                   'hwpapi.functions.hex_to_rgb': ('02_api/functions.html#hex_to_rgb', 'hwpapi/functions.py'),
+                                  'hwpapi.functions.mili2unit': ('02_api/functions.html#mili2unit', 'hwpapi/functions.py'),
+                                  'hwpapi.functions.point2unit': ('02_api/functions.html#point2unit', 'hwpapi/functions.py'),
                                   'hwpapi.functions.set_charshape_pset': ( '02_api/functions.html#set_charshape_pset',
                                                                            'hwpapi/functions.py'),
                                   'hwpapi.functions.set_parashape_pset': ( '02_api/functions.html#set_parashape_pset',
-                                                                           'hwpapi/functions.py')}}}
+                                                                           'hwpapi/functions.py'),
+                                  'hwpapi.functions.set_pset': ('02_api/functions.html#set_pset', 'hwpapi/functions.py'),
+                                  'hwpapi.functions.unit2mili': ('02_api/functions.html#unit2mili', 'hwpapi/functions.py'),
+                                  'hwpapi.functions.unit2point': ('02_api/functions.html#unit2point', 'hwpapi/functions.py')}}}
```

## hwpapi/actions.py

```diff
@@ -57,22 +57,22 @@
     "CharShapeShadow": [None, "그림자"],
     "CharShapeSpacing": [None, "자간(글자 모양 대화상자에서 Focus이동용으로 사용)"],
     "CharShapeSpacingDecrease": [None, "자간 좁게 ALT+SHIFT+N"],
     "CharShapeSpacingIncrease": [None, "자간 넓게 ALT+SHIFT+W"],
     "CharShapeSubscript": [None, "아래첨자 ALT+SHIFT+S"],
     "CharShapeSuperscript": [None, "위첨자 ALT+SHIFT+P"],
     "CharShapeSuperSubscript": [None, '첨자 : "위첨자 -> 아래첨자 -> 보통" 반복'],
-    "CharShapeTextColorBlack": [None, "글자색을 검정"],
-    "CharShapeTextColorBlue": [None, "글자색을 파랑"],
-    "CharShapeTextColorBluish": [None, "글자색을 청록"],
-    "CharShapeTextColorGreen": [None, "글자색을 초록"],
-    "CharShapeTextColorRed": [None, "글자색을 빨강"],
-    "CharShapeTextColorViolet": [None, "글자색을 자주"],
-    "CharShapeTextColorWhite": [None, "글자색을 흰색"],
-    "CharShapeTextColorYellow": [None, "글자색을 노랑"],
+    "CharShapeTextColorBlack": ["CharShape", "글자색을 검정"],
+    "CharShapeTextColorBlue": ["CharShape", "글자색을 파랑"],
+    "CharShapeTextColorBluish": ["CharShape", "글자색을 청록"],
+    "CharShapeTextColorGreen": ["CharShape", "글자색을 초록"],
+    "CharShapeTextColorRed": ["CharShape", "글자색을 빨강"],
+    "CharShapeTextColorViolet": ["CharShape", "글자색을 자주"],
+    "CharShapeTextColorWhite": ["CharShape", "글자색을 흰색"],
+    "CharShapeTextColorYellow": ["CharShape", "글자색을 노랑"],
     "CharShapeTypeFace": [None, "글꼴 이름(글자 모양 대화상자에서 Focus이동용으로 사용)"],
     "CharShapeUnderline": [None, "밑줄 ALT+SHIFT+U"],
     "CharShapeWidth": [None, "장평(글자 모양 대화상자에서 Focus이동용으로 사용)"],
     "CharShapeWidthDecrease": [None, "장평 좁게 ALT+SHIFT+J"],
     "CharShapeWidthIncrease": [None, "장평 넓게 ALT+SHIFT+K"],
     "Close": [None, "현재 리스트를 닫고 상위 리스트로 이동."],
     "CloseEx": [
@@ -85,14 +85,15 @@
     "ComposeChars": ["ChCompose", "글자 겹침"],
     "ConvertCase": ["ConvertCase", "대소문자 바꾸기"],
     "ConvertFullHalfWidth": ["ConvertFullHalf", "전각 반각 바꾸기"],
     "ConvertHiraGata": ["ConvertHiraToGata", "일어 바꾸기"],
     "ConvertJianFan": ["ConvertJianFan", "간/번체 바꾸기 \tText가 선택된 상태에서만 동작"],
     "ConvertToHangul": ["ConvertToHangul", "한글로"],
     "Copy": [None, "복사하기"],
+    "CopyPage": [None, "페이지 복사하기"],
     "Cut": [None, "오려두기"],
     "Delete": [None, "Delete"],
     "DeleteBack": [None, "Backspace"],
     "DeleteCtrls": ["DeleteCtrls", "조판 부호 지우기"],
     "DeleteDutmal": [None, "덧말 지우기"],
     "DeleteField": [None, "누름틀/메모지우기 \t누름틀/메모 안의 내용은 지우지 않고, 단순히 누름틀만 지운다."],
     "DeleteFieldMemo": [None, "메모 지우기"],
@@ -572,15 +573,16 @@
     "ParagraphShapeIndentPositive": [None, "첫 줄을 한 글자 들여 씀"],
     "ParagraphShapeProtect": [None, "문단 보호"],
     "ParagraphShapeWithNext": [None, "다음 문단과 함께"],
     "ParaNumberBullet": ["ParaShape", "문단번호/글머리표 한 수준 위로"],
     "ParaNumberBulletLevelDown": ["ParaShape", "문단번호/글머리표 한 수준 아래로"],
     "ParaNumberBulletLevelUp": ["ParaShape", "문단번호/글머리표 한 수준 위로"],
     "ParaShapeDialog": ["ParaShape", "문단 모양 대화상자(내부 구현용)"],
-    "Paste": [None, "붙이기"],
+    "Paste": ["SelectionOpt", "붙이기"],
+    "PastePage": [None, "페이지 붙이기"],
     "PasteSpecial": [None, "골라 붙이기"],
     "PictureEffect1": [None, "그림 그레이 스케일"],
     "PictureEffect2": [None, "그림 흑백으로"],
     "PictureEffect3": [None, "그림 워터마크"],
     "PictureEffect4": [None, "그림 효과 없음"],
     "PictureEffect5": [None, "그림 밝기 증가"],
     "PictureEffect6": [None, "그림 밝기 감소"],
```

## hwpapi/core.py

```diff
@@ -1,34 +1,57 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/02_api/00_core.ipynb.
 
 # %% auto 0
 __all__ = ['mask_options', 'scan_spos_keys', 'scan_epos_keys', 'scan_directions', 'move_ids', 'size_options', 'effects',
-           'directions', 'App', 'move_to_line']
+           'directions', 'thickness_dict', 'App', 'move_to_line']
 
 # %% ../nbs/02_api/00_core.ipynb 4
 from contextlib import contextmanager
 from pathlib import Path
 
 from fastcore.basics import patch
 
 # %% ../nbs/02_api/00_core.ipynb 5
 from .actions import _Action, _Actions
+from .dataclasses import CharShape, ParaShape
 from hwpapi.functions import (
     check_dll,
     dispatch,
     get_absolute_path,
+    get_charshape_pset,
+    get_parashape_pset,
     get_rgb_tuple,
     get_value,
+    mili2unit,
+    point2unit,
     set_charshape_pset,
     set_parashape_pset,
+    set_pset,
+    unit2mili,
+    unit2point,
 )
 
 # %% ../nbs/02_api/00_core.ipynb 6
 class App:
-    """App 클래스는 한컴오피스의 한/글 프로그램과 상호작용하기 위한 인터페이스를 제공합니다."""
+    """`App` 클래스는 한컴오피스의 한/글 프로그램과 상호작용하기 위한 인터페이스를 제공합니다.
+
+    메소드
+    ----------
+    __init__(api=None, is_visible=True) : None
+        `App` 클래스의 객체를 초기화합니다. 이 메소드에서는 `api` 객체를 인자로 받습니다.
+        만약 `api`가 제공되지 않았을 경우, `wc.gencache.EnsureDispatch("HWPFrame.HwpObject")`를 호출하여
+        기본값으로 한/글 프로그램의 COM 객체를 생성합니다. 그리고 `self.api` 속성에 이 객체를 할당합니다.
+        `_Actions` 클래스의 객체를 생성하여 `self.actions` 속성에 할당하고, `self.set_visible()` 함수를 호출합니다.
+
+    __str__() : str
+        `App` 클래스의 객체를 문자열로 변환하여 반환합니다. 반환되는 문자열은 `"<Hwp App: {self.get_filepath()}>"` 형식을 가집니다.
+
+    __repr__() : str
+        `__repr__` 메소드는 `__str__` 메소드와 동일한 기능을 수행합니다.
+    """
 
     def __init__(self, api=None, is_visible=True):
         """`__init__` 함수에서는 `api` 객체를 인자로 받습니다.
         만약 `api`가 제공되지 않았을 경우, `wc.gencache.EnsureDispatch("HWPFrame.HwpObject")`를 호출하여
         기본값으로 한/글 프로그램의 COM 객체를 생성합니다. 그리고 `self.api` 속성에 이 객체를 할당합니다.
         `_Actions` 클래스의 객체를 생성하여 `self.actions` 속성에 할당하고, `self.set_visible()` 함수를 호출합니다.
         """
@@ -66,31 +89,83 @@
 # %% ../nbs/02_api/00_core.ipynb 9
 @patch
 def get_filepath(app: App):
     """`get_filepath()` 함수는 현재 열려있는 한/글 문서의 경로를 반환합니다."""
     doc = app.api.XHwpDocuments.Active_XHwpDocument
     return doc.FullName
 
+# %% ../nbs/02_api/00_core.ipynb 10
+@patch
+def create_action(app: App, action_key: str):
+    """
+    `create_action` 함수는 `_Action` 클래스의 인스턴스를 생성하고 반환합니다.
+
+    매개변수
+    ----------
+    app : App
+        액션을 생성할 애플리케이션 객체입니다.
+
+    action_key : str
+        생성할 액션의 키입니다.
+
+    반환
+    ------
+    _Action(app, action_key) : _Action object
+        입력받은 애플리케이션 객체와 액션 키를 사용하여 생성된 _Action 클래스의 인스턴스를 반환합니다.
+    """
+    return _Action(app, action_key)
+
 # %% ../nbs/02_api/00_core.ipynb 11
 @patch
+def create_parameterset(app: App, action_key: str):
+    """
+    `create_parameterset` 함수는 특정 액션에 대한 파라미터셋을 생성하고 반환합니다.
+
+    `_action_info` 딕셔너리를 사용하여 주어진 액션 키에 대한 파라미터셋 정보를 조회합니다.
+    파라미터셋 정보가 있으면 해당 파라미터셋 객체를 생성하고 반환합니다.
+
+    매개변수
+    ----------
+    app : App
+        파라미터셋을 생성할 애플리케이션 객체입니다.
+
+    action_key : str
+        파라미터셋을 생성할 액션의 키입니다.
+
+    반환
+    ------
+    getattr(app.api.HParameterSet, f"H{pset_key}") : HParameterSet object or None
+        해당 액션 키에 대한 파라미터셋 객체를 반환합니다.
+        만약 액션 키에 대한 파라미터셋 정보가 없으면 None를 반환합니다.
+    """
+    pset_key, description = _action_info.get(action_key, None)
+    if not pset_key:
+        return None
+    return getattr(app.api.HParameterSet, f"H{pset_key}")
+
+# %% ../nbs/02_api/00_core.ipynb 13
+@patch
 def open(app: App, path: str):
     """`open()` 함수는 파일 경로를 인자로 받아 해당 파일을 한/글 프로그램에서 엽니다.
     `get_absolute_path()` 함수를 호출하여 절대 경로로 변환한 후, `api.Open()` 함수를 호출하여 파일을 엽니다.
     열린 파일의 경로를 반환합니다."""
     name = get_absolute_path(path)
     app.api.Open(name)
     return name
 
-# %% ../nbs/02_api/00_core.ipynb 13
+# %% ../nbs/02_api/00_core.ipynb 15
+@patch
+def get_hwnd(app:App):
+    return app.api.XHwpWindows.Active_XHwpWindow.WindowHandle
+
+# %% ../nbs/02_api/00_core.ipynb 17
 @patch
 def save(app: App, path=None):
-    """`save()` 함수는 현재 열려있는 문서를 저장하거나 다른 이름으로 저장합니다.
-    `path` 인자가 주어지지 않은 경우 현재 문서를 덮어쓰기로 저장하고, 저장된 파일의 경로를 반환합니다.
-    `path` 인자가 주어진 경우, `Path` 모듈을 이용하여 파일 확장자를 추출한 후, 해당 확장자에 맞게 문서를 저장합니다.
-    저장된 파일의 경로를 반환합니다."""
+    """
+    """
 
     if not path:
         app.api.Save()
         return app.get_filepath()
     name = get_absolute_path(path)
     extension = Path(name).suffix
     format_ = {
@@ -99,289 +174,194 @@
         ".hwpx": "HWPML2X",
         ".png": "PNG",
     }.get(extension)
 
     app.api.SaveAs(name, format_)
     return name
 
-# %% ../nbs/02_api/00_core.ipynb 14
+# %% ../nbs/02_api/00_core.ipynb 19
+@patch
+def save_block(app: App, path: Path):
+    """
+    `save_block` 함수는 블록을 저장하고 주소를 반환합니다.
+
+    매개변수
+    ----------
+    app : App
+        액션을 생성할 애플리케이션 객체입니다.
+
+    path : Path
+        저장할 주소 입니다.
+
+    반환
+    ------
+    path : 생성이 성공하면 주소를 반환합니다. 실패하면 None을 반환합니다.
+    """
+
+    name = get_absolute_path(path)
+    extension = Path(name).suffix
+    format_ = {
+        ".hwp": "HWP",
+        ".pdf": "PDF",
+        ".hwpx": "HWPML2X",
+        ".png": "PNG",
+    }.get(extension)
+
+    action = app.actions.SaveBlockAction()
+    p = action.pset
+    
+    p.filename = name
+    p.Format = format_
+    action.run()
+    return name if Path(name).exists() else None
+
+# %% ../nbs/02_api/00_core.ipynb 21
 @patch
 def close(app: App):
     """`close()` 함수는 현재 열려있는 문서를 닫습니다."""
     app.api.Run("FileClose")
 
-# %% ../nbs/02_api/00_core.ipynb 15
+# %% ../nbs/02_api/00_core.ipynb 23
 @patch
 def quit(app: App):
     """`quit()` 함수는 한/글 프로그램을 종료합니다."""
     app.api.Run("FileQuit")
 
-# %% ../nbs/02_api/00_core.ipynb 16
+# %% ../nbs/02_api/00_core.ipynb 24
 @patch
-def create_action(app: App, action_key: str):
-    """`create_action()` 함수는 `_Action` 클래스의 객체를 생성하여 반환합니다."""
-    return _Action(app, action_key)
+def get_charshape(app: App):
+    """
+    `get_charshape` 메소드는 현재 애플리케이션에서 문자 모양을 가져오는 함수입니다.
 
-# %% ../nbs/02_api/00_core.ipynb 17
-@patch
-def create_parameterset(app: App, action_key: str):
-    """`create_parameterset()` 함수는 특정 액션의 파라미터셋을 반환합니다.
-    `_action_info` 딕셔너리에서 액션에 대한 정보를 찾아서 파라미터셋의 키 값을 가져옵니다. 파라미터셋 객체를 반환합니다."""
-    pset_key, description = _action_info.get(action_key, None)
-    if not pset_key:
-        return None
-    return getattr(app.api.HParameterSet, f"H{pset_key}")
+    매개변수
+    ----------
+    app : App
+        문자 모양을 가져올 애플리케이션 객체입니다.
 
-# %% ../nbs/02_api/00_core.ipynb 18
+    반환
+    ------
+    CharShape
+        애플리케이션에서 가져온 문자 모양입니다.
+    """
+    action = app.actions.CharShape()
+    p = action.pset
+    return CharShape(p)
+
+# %% ../nbs/02_api/00_core.ipynb 26
 @patch
-def set_charshape(
-    app: App,
-    fontname: str = None,
-    font_type: int = 1,
-    size: int = None,
-    ratio: int = None,
-    spacing: int = None,
-    offset: int = None,
-    bold: bool = None,
-    italic: bool = None,
-    small_caps: bool = None,
-    emboss: bool = None,
-    super_script: bool = None,
-    sub_script: bool = None,
-    underline_type: int = None,
-    outline_type: int = None,
-    text_color=None,
-    shade_color=None,
-    underline_shape: int = None,
-    underline_color=None,
-    shadow_offset_x: int = None,
-    shadow_offset_y: int = None,
-    shadow_color=None,
-    strike_out_type=None,
-    diac_sym_mark=None,
-    use_font_space=None,
-    use_kerning=None,
-    height: int = None,
-):
-    """`현재 위치의 글자 모양을 조정합니다."""
-    charshape = app.actions.CharShape()
+def set_charshape(app: App, charshape: CharShape=None, **kwargs):
+    """`set_charshape` 함수는 주어진 `CharShape`를 사용하여 애플리케이션의 현재 문단 모양을 설정합니다.
 
-    if height:
-        height = app.api.PointToHwpUnit(height)
+    만약 `charshape`가 `None`인 경우, `CharShape`의 기본 인스턴스를 생성합니다.
 
-    if text_color:
-        text_color = app.api.RGBColor(*get_rgb_tuple(text_color))
-    if shade_color:
-        shade_color = app.api.RGBColor(*get_rgb_tuple(shade_color))
-    if shadow_color:
-        shadow_color = app.api.RGBColor(*get_rgb_tuple(shadow_color))
-
-    set_charshape_pset(
-        charshape.pset,
-        face_name=fontname,
-        font_type=font_type,
-        size=size,
-        ratio=ratio,
-        spacing=spacing,
-        offset=offset,
-        bold=bold,
-        italic=italic,
-        small_caps=small_caps,
-        emboss=emboss,
-        super_script=super_script,
-        sub_script=sub_script,
-        underline_type=underline_type,
-        outline_type=outline_type,
-        text_color=text_color,
-        shade_color=shade_color,
-        underline_shape=underline_shape,
-        underline_color=underline_color,
-        shadow_offset_x=shadow_offset_x,
-        shadow_offset_y=shadow_offset_y,
-        shadow_color=shadow_color,
-        strike_out_type=strike_out_type,
-        diac_sym_mark=diac_sym_mark,
-        use_font_space=use_font_space,
-        use_kerning=use_kerning,
-        height=height,  # 포인트를 한글 유닛으로 변경합니다.
-    )
-    return charshape.run()
+    이 함수는 추가로 `kwargs`를 인자로 받아, 이를 `parashape`의 속성에 할당합니다.
+    이렇게 수정된 `parashape`는 한/글 문서의 현재 문단 모양을 변경하는데 사용됩니다.
 
-# %% ../nbs/02_api/00_core.ipynb 19
+    Parameters
+    ----------
+    app : App
+        `App` 객체입니다. 한/글 애플리케이션에 접근하는데 사용됩니다.
+    charshape : CharShape, optional
+        한/글 글자 모양을 설정하는데 사용될 `CharShape` 객체입니다. 기본값은 `None`입니다.
+    **kwargs :
+        `CharShape`의 속성에 할당될 추가 키워드 인자입니다.
+
+    Returns
+    -------
+    bool
+        `set_charshape` 작업의 성공 여부를 나타내는 부울 값입니다.
+    """
+    if charshape is None:
+        charshape = CharShape()
+
+    for key, value in kwargs.items():
+        setattr(charshape, key, value)
+        
+    action = app.actions.CharShape()
+    set_pset(action.pset, charshape.todict())
+    return action.run()
+
+# %% ../nbs/02_api/00_core.ipynb 30
 @patch
-def set_parashape(
-    app: App,
-    left_margin: int = None,
-    right_margin: int = None,
-    indentation: int = None,
-    prev_spacing: int = None,
-    next_spacing: int = None,
-    line_spacing_type: str = None,
-    line_spacing: int = None,
-    align_type: str = None,
-    break_latin_word: str = None,
-    break_non_latin_word: bool = None,
-    snap_to_grid: bool = None,
-    condense: float = None,
-    widow_orphan: bool = None,
-    keep_with_next: bool = None,
-    page_break_before: bool = None,
-    text_alignment: str = None,
-    font_line_height: int = None,
-    heading_type: str = None,
-    level: int = None,
-    border_connect: bool = None,
-    border_text: bool = None,
-    border_offset_left: int = None,
-    border_offset_right: int = None,
-    border_offset_top: int = None,
-    border_offset_bottom: int = None,
-    tail_type: bool = None,
-    line_wrap: bool = None,
-    tab_def=None,
-    numbering=None,
-    bullet=None,
-    borderfill=None,
-):
-    parashape = app.actions.ParagraphShape()
+def get_parashape(app: App):
+    """
+    `get_parashape` 메소드는 현재 애플리케이션에서 문단 모양을 가져오는 함수입니다.
 
-    # enum 스타일
-    spacing_types = {
-        "Word": 0,
-        "Fixed": 1,
-        "Margin": 2,
-    }
-    if line_spacing_type:
-        line_spacing_type = get_value(spacing_types, line_spacing_type)
+    매개변수
+    ----------
+    app : App
+        문단 모양을 가져올 애플리케이션 객체입니다.
 
-    align_types = {
-        "Both": 0,
-        "Left": 1,
-        "Right": 2,
-        "Center": 3,
-        "Distributed": 4,
-        "SpaceOnly": 5,
-    }
-    if align_type:
-        align_type = get_value(align_types, align_type)
+    반환
+    ------
+    ParaShape
+        애플리케이션에서 가져온 문단 모양입니다.
+    """
+    action = app.actions.ParagraphShape()
+    p = action.pset
 
-    break_latin_words = {
-        "Word": 0,
-        "Hyphen": 1,
-        "Letter": 2,
-    }
-    if break_latin_word:
-        break_latin_word = get_value(break_latin_words, break_latin_word)
+    return ParaShape(p)
 
-    text_alignments = {
-        "Font": 0,
-        "Upper": 1,
-        "Middle": 2,
-        "Lower": 3,
-    }
-    if text_alignment:
-        text_alignment = get_value(text_alignments, text_alignment)
+# %% ../nbs/02_api/00_core.ipynb 32
+@patch
+def set_parashape(app: App, parashape: ParaShape = None, **kwargs):
+    """`set_parashape` 함수는 주어진 `ParaShape`를 사용하여 애플리케이션의 현재 문단 모양을 설정합니다.
 
-    heading_types = {
-        "None": 0,
-        "Content": 1,
-        "Numbering": 2,
-        "Bullet": 3,
-    }
-    if heading_type:
-        heading_type = get_value(heading_types, heading_type)
+    만약 `parashape`가 `None`인 경우, `ParaShape`의 기본 인스턴스를 생성합니다.
 
-    # 유닛 조정
-    mili_units = [
-        border_offset_left,
-        border_offset_right,
-        border_offset_top,
-        border_offset_bottom,
-    ]
-    convert_mili = lambda value: app.api.MiliToHwpUnit(value) if value else None
-    mili_units = list(map(convert_mili, mili_units))
-    (
-        border_offset_left,
-        border_offset_right,
-        border_offset_top,
-        border_offset_bottom,
-    ) = mili_units
-
-    point_units = [left_margin, right_margin]
-    convert_point = lambda value: app.api.PointToHwpUnit(value) * 2 if value else None
-    point_units = list(map(convert_point, point_units))
-    left_margin, right_margin = point_units
-
-    set_parashape_pset(
-        parashape.pset,
-        left_margin=left_margin,
-        right_margin=right_margin,
-        indentation=indentation,
-        prev_spacing=prev_spacing,
-        next_spacing=next_spacing,
-        line_spacing_type=line_spacing_type,
-        line_spacing=line_spacing,
-        align_type=align_type,
-        break_latin_word=break_latin_word,
-        break_non_latin_word=break_non_latin_word,
-        snap_to_grid=snap_to_grid,
-        condense=condense,
-        widow_orphan=widow_orphan,
-        keep_with_next=keep_with_next,
-        page_break_before=page_break_before,
-        text_alignment=text_alignment,
-        font_line_height=font_line_height,
-        heading_type=heading_type,
-        level=level,
-        border_connect=border_connect,
-        border_text=border_text,
-        border_offset_left=border_offset_left,
-        border_offset_right=border_offset_right,
-        border_offset_top=border_offset_top,
-        border_offset_bottom=border_offset_bottom,
-        tail_type=tail_type,
-        line_wrap=line_wrap,
-    )
+    이 함수는 추가로 `kwargs`를 인자로 받아, 이를 `parashape`의 속성에 할당합니다.
+    이렇게 수정된 `parashape`는 한/글 문서의 현재 문단 모양을 변경하는데 사용됩니다.
+
+    Parameters
+    ----------
+    app : App
+        `App` 객체입니다. 한/글 애플리케이션에 접근하는데 사용됩니다.
+    parashape : ParaShape, optional
+        한/글 문단 모양을 설정하는데 사용될 `ParaShape` 객체입니다. 기본값은 `None`입니다.
+    **kwargs :
+        `ParaShape`의 속성에 할당될 추가 키워드 인자입니다.
 
-    return parashape.run()
+    Returns
+    -------
+    bool
+        `set_parashape` 작업의 성공 여부를 나타내는 부울 값입니다.
+    """
+    if parashape is None:
+        parashape = ParaShape()
+
+    for key, value in kwargs.items():
+        setattr(parashape, key, value)
+
+    action = app.actions.ParagraphShape()
+    set_pset(action.pset, parashape.todict())
+    return action.run()
 
-# %% ../nbs/02_api/00_core.ipynb 20
+# %% ../nbs/02_api/00_core.ipynb 34
 @patch
 def insert_text(
     app: App,
     text: str,
-    fontname=None,
-    font_type=1,
-    bold=None,
-    italic=None,
-    strike_out_type=None,
-    underline_type=None,
-    ratio=None,
-    height=None,
-    text_color=None,
+    charshape: CharShape = None, 
+    **kwargs,
 ):
     """`text를 입력합니다."""
-    app.set_charshape(
-        fontname=fontname,
-        font_type=font_type,
-        bold=bold,
-        italic=italic,
-        strike_out_type=strike_out_type,
-        underline_type=underline_type,
-        ratio=ratio,
-        height=height,
-        text_color=text_color,
-    )
+    if not charshape:
+        charshape = CharShape()
+    for key, value in kwargs.items():
+        setattr(charshape, key, value)
+    app.set_charshape(charshape)
+    
     insert_text = app.actions.InsertText()
     p = insert_text.pset
     p.Text = text
+    
     insert_text.run()
     return
 
-# %% ../nbs/02_api/00_core.ipynb 25
+# %% ../nbs/02_api/00_core.ipynb 39
 mask_options = {
     "Normal": 0x00,  # "본문을 대상으로 검색한다.(서브리스트를 검색하지 않는다.)"
     "Char": 0x01,  # "char 타입 컨트롤 마스크를 대상으로 한다.(강제줄나눔, 문단 끝, 하이픈, 묶움빈칸, 고정폭빈칸, 등...)"
     "Inline": 0x02,  # "inline 타입 컨트롤 마스크를 대상으로 한다.(누름틀 필드 끝, 등...)"
     "Ctrl": 0x04,  # "extende 타입 컨트롤 마스크를 대상으로 한다.(바탕쪽, 프레젠테이션, 다단, 누름틀 필드 시작, Shape Object, 머리말, 꼬리말, 각주, 미주, 번호관련 컨트롤, 새 번호 관련 컨트롤, 감추기, 찾아보기, 글자 겹침, 등...)"
     "All": None,
 }
@@ -454,24 +434,24 @@
         spos=spos,
         epara=epara,
         epos=epos,
     )
     yield _get_text(app)
     app.api.ReleaseScan()
 
-# %% ../nbs/02_api/00_core.ipynb 26
+# %% ../nbs/02_api/00_core.ipynb 40
 def move_to_line(app: App, text):
     """인자로 전달한 텍스트가 있는 줄의 시작지점으로 이동합니다."""
     with app.scan(scan_spos="Line") as scan:
         for line in scan:
             if text in line:
                 return app.move(key="ScanPos")
     return False
 
-# %% ../nbs/02_api/00_core.ipynb 27
+# %% ../nbs/02_api/00_core.ipynb 41
 move_ids = {
     "Main": 0,  # 루트 리스트의 특정 위치.(para pos로 위치 지정)
     "CurList": 1,  # 현재 리스트의 특정 위치.(para pos로 위치 지정)
     "TopOfFile": 2,  # 문서의 시작으로 이동.
     "BottomOfFile": 3,  # 문서의 끝으로 이동.
     "TopOfList": 4,  # 현재 리스트의 시작으로 이동
     "BottomOfList": 5,  # 현재 리스트의 끝으로 이동
@@ -513,15 +493,43 @@
 @patch
 def move(app: App, key="ScanPos", para=None, pos=None):
     """키워드를 바탕으로 캐럿 위치를 이동시킵니다."""
 
     move_id = get_value(move_ids, key)
     return app.api.MovePos(moveID=move_id, Para=para, pos=pos)
 
-# %% ../nbs/02_api/00_core.ipynb 30
+# %% ../nbs/02_api/00_core.ipynb 43
+@patch
+def setup_page(
+    app: App,  # app
+    top=20,  # 윗 여백
+    bottom=10,  # 아래 여백
+    right=20,  # 오른쪽 여백
+    left=20,  # 왼쪽 여백
+    header=15,  # 머릿말
+    footer=5,  # 꼬릿말
+    gutter=0,
+):  # 제본
+    """
+    페이지를 설정합니다.
+    """
+    action = app.actions.PageSetup()
+    p = action.pset
+
+    p.PageDef.TopMargin = app.api.MiliToHwpUnit(top)
+    p.PageDef.HeaderLen = app.api.MiliToHwpUnit(header)
+    p.PageDef.RightMargin = app.api.MiliToHwpUnit(right)
+    p.PageDef.BottomMargin = app.api.MiliToHwpUnit(bottom)
+    p.PageDef.FooterLen = app.api.MiliToHwpUnit(footer)
+    p.PageDef.LeftMargin = app.api.MiliToHwpUnit(left)
+    p.PageDef.GutterLen = app.api.MiliToHwpUnit(gutter)
+
+    return action.run()
+
+# %% ../nbs/02_api/00_core.ipynb 44
 size_options = {
     "realSize": 0,  # 이미지를 원래의 크기로 삽입한다.
     "specificSize": 1,  # width와 height에 지정한 크기로 그림을 삽입한다.
     "cellSize": 2,  # 현재 캐럿이 표의 셀안에 있을 경우, 셀의 크기에 맞게 자동 조정하여 삽입한다.
     "cellSizeWithSameRatio": 3,  # 현재 캐럿이 표의 셀 안에 있을 경우, 셀의 크기에 맞추어 원본 이미지의 가로 세로 비율이 동일하게 확대/축소하여 삽입한다.
 }
 
@@ -555,68 +563,66 @@
         Height=height,
         sizeoption=sizeoption,
         reverse=reverse,
         watermark=watermark,
         effect=effect,
     )
 
-# %% ../nbs/02_api/00_core.ipynb 31
+# %% ../nbs/02_api/00_core.ipynb 45
 @patch
 def select_text(app: App, option: str = "Line"):
     """
     한줄을 선택합니다.
     """
     select_options = {
         "Doc": (app.actions.MoveDocBegin, app.actions.MoveSelDocEnd),
         "Para": (app.actions.MoveParaBegin, app.actions.MoveSelParaEnd),
         "Line": (app.actions.MoveLineBegin, app.actions.MoveSelLineEnd),
         "Word": (app.actions.MoveWordBegin, app.actions.MoveSelWordEnd),
     }
     begin, end = select_options.get(option)
     return begin().run(), end().run()
 
-# %% ../nbs/02_api/00_core.ipynb 34
+# %% ../nbs/02_api/00_core.ipynb 48
 @patch
 def get_selected_text(app: App):
     """
     선택된 영역의 텍스트를 불러온다.
     """
     with app.scan(selection=True) as scan:
         text = "\n".join(scan)
     return text
 
-# %% ../nbs/02_api/00_core.ipynb 36
+# %% ../nbs/02_api/00_core.ipynb 50
 @patch
 def get_text(app: App, spos="Line", epos="Line"):
     """
     텍스트를 가져옵니다. 기본은 현재 문장입니다.
+    "Current":  # "캐럿 위치부터. (현재 위치까지)",
+    "Specified": 0x0010,  # "특정 위치부터. (특정 위치까지)",
+    "Line": 0x0020,  # "줄의 시작부터. (줄 끝까지)",
+    "Paragraph": 0x0030,  # "문단의 시작부터. (문단 끝까지)"
+    "Section": 0x0040,  # "구역의 시작부터. (구역의 끝까지)"
+    "List": 0x0050,  # "리스트의 시작부터. (리스트 끝까지)"
+    "Control": 0x0060,  # "컨트롤의 시작부터. (컨트롤 끝까지)"
+    "Document": 0x0070,  # "문서의 시작부터. (문서 끝까지)"
     """
     with app.scan(scan_spos=spos, scan_epos=epos) as txts:
         text = "".join(txts)
     return text
 
-# %% ../nbs/02_api/00_core.ipynb 38
+# %% ../nbs/02_api/00_core.ipynb 52
 directions = {"Forward": 0, "Backward": 1, "All": 2}
 
-# %% ../nbs/02_api/00_core.ipynb 39
+# %% ../nbs/02_api/00_core.ipynb 53
 @patch
 def find_text(
     app: App,
     text="",
-    text_fontcolor=None,  # 찾을 폰트 색
-    fontsize=None,  # 찾을 폰트 크기(height)
-    fontname="",  # 찾을 글꼴
-    fonttype=1,  # 찾을 글꼴 타입 TTF = 1, HTF = 2
-    fontratio=None,  # 찾을 장평
-    text_color=None,
-    spacing=None,  # 찾을 자간
-    bold=None,  # 찾을 볼드
-    italic=None,  # 찾을 이텔릭
-    underline=None,  # 찾을 밑줄
-    strike_out=None,  # 찾을 취소선
+    charshape: CharShape = None,
     ignore_message=True,  # 메시지 무시 여부
     direction="Forward",  # 찾을 방향
     match_case=False,  # 대소문자 구분
     all_word_forms=False,  # 문자열 결합
     several_words=False,  #  여러 단어 찾기
     use_wild_cards=False,  # 아무개 문자
     whole_word_only=False,  # 온전한 낱말
@@ -651,56 +657,28 @@
     p.IgnoreReplaceString = ignore_replace_string
     p.FindStyle = find_style
     p.ReplaceStyle = replace_style
     p.FindJaso = find_jaso
     p.FindRegExp = find_reg_exp
     p.FindType = find_type
 
-    # set old charshape
-    set_charshape_pset(
-        p.FindCharShape,
-        face_name=fontname,
-        font_type=fonttype,
-        text_color=text_color,
-        bold=bold,
-        italic=italic,
-        strike_out_type=strike_out,
-        underline_type=underline,
-        ratio=fontratio,
-        spacing=spacing,
-    )
+    # set charshape
+    if charshape:
+        set_pset(p.FindCharShape, charshape.todict())
 
     return action.run()
 
-# %% ../nbs/02_api/00_core.ipynb 41
+# %% ../nbs/02_api/00_core.ipynb 55
 @patch
 def replace_all(
     app: App,
-    old="",
-    new="",
-    old_text_color=None,  # 찾을 폰트 색
-    new_text_color=None,  # 바꿀 폰트 색
-    old_fontsize=None,  # 찾을 폰트 크기(height)
-    new_fontsize=None,  # 바꿀 폰트 크기(height)
-    old_fontname="",  # 찾을 글꼴
-    old_fonttype=1,  # 찾을 글꼴 타입 TTF = 1, HTF = 2
-    new_fontname="",  # 바꿀 글꼴
-    new_fonttype=1,  # 바꿀 글꼴 타입 TTF = 1, HTF = 2
-    old_fontratio=None,  # 찾을 장평
-    new_fontratio=None,  # 바꿀 장평
-    old_spacing=None,  # 찾을 자간
-    new_spacing=None,  # 바꿀 자간
-    old_bold=None,  # 찾을 볼드
-    new_bold=None,  # 바꿀 볼드
-    old_italic=None,  # 찾을 이텔릭
-    new_italic=None,  # 바꿀 이텔릭
-    old_underline=None,  # 찾을 밑줄
-    new_underline=None,  # 바꿀 밑줄
-    old_strike_out=None,  # 찾을 취소선
-    new_strike_out=None,  # 바꿀 취소선
+    old_text="",
+    new_text="",
+    old_charshape: CharShape = None,
+    new_charshape: CharShape = None,
     ignore_message=True,  # 메시지 무시 여부
     direction="All",  # 찾을 방향
     match_case=False,  # 대소문자 구분
     all_word_forms=False,  # 문자열 결합
     several_words=False,  #  여러 단어 찾기
     use_wild_cards=False,  # 아무개 문자
     whole_word_only=False,  # 온전한 낱말
@@ -714,16 +692,16 @@
     find_reg_exp=False,  # 정규표현식으로 찾기
     find_type=True,  # 다시 찾기를 할 때 마지막으로 실한 찾기를 할 경우 True, 찾아가기를 할경우 False
 ):
     action = app.actions.AllReplace()
     p = action.pset
 
     # set options
-    p.FindString = old
-    p.ReplaceString = new
+    p.FindString = old_text
+    p.ReplaceString = new_text
     p.IgnoreMessage = ignore_message
     p.MatchCase = match_case
     p.AllWordForms = all_word_forms
     p.Direction = get_value(directions, direction)
     p.SeveralWords = several_words
     p.UseWildCards = use_wild_cards
     p.WholeWordOnly = whole_word_only
@@ -734,42 +712,23 @@
     p.FindStyle = find_style
     p.ReplaceStyle = replace_style
     p.FindJaso = find_jaso
     p.FindRegExp = find_reg_exp
     p.FindType = find_type
 
     # set old charshape
-    set_charshape_pset(
-        p.FindCharShape,
-        face_name=old_fontname,
-        text_color=old_text_color,
-        font_type=old_fonttype,
-        bold=old_bold,
-        italic=old_italic,
-        strike_out_type=old_strike_out,
-        underline_type=old_underline,
-        ratio=old_fontratio,
-        spacing=old_spacing,
-    )
-    set_charshape_pset(
-        p.ReplaceCharShape,
-        face_name=new_fontname,
-        text_color=new_text_color,
-        font_type=new_fonttype,
-        bold=new_bold,
-        italic=new_italic,
-        strike_out_type=new_strike_out,
-        underline_type=new_underline,
-        ratio=new_fontratio,
-        spacing=new_spacing,
-    )
+
+    if old_charshape:
+        set_pset(p.FindCharShape, old_charshape.todict())
+    if new_charshape:
+        set_charshape_pset(p.ReplaceCharShape, new_charshape.todict())
 
     return action.run()
 
-# %% ../nbs/02_api/00_core.ipynb 44
+# %% ../nbs/02_api/00_core.ipynb 58
 @patch
 def insert_file(
     app: App,
     fpath,
     keep_charshape=False,
     keep_parashape=False,
     keep_section=False,
@@ -785,15 +744,37 @@
     p.KeepCharshape = keep_charshape
     p.KeepParashape = keep_parashape
     p.KeepSection = keep_section
     p.KeepStyle = keep_style
 
     return action.run()
 
-# %% ../nbs/02_api/00_core.ipynb 45
+# %% ../nbs/02_api/00_core.ipynb 59
+thickness_dict = {
+    -1: "최소값 (=0.1 mm)",
+    0: "0.1 mm",
+    1: "0.12 mm",
+    2: "0.15 mm",
+    3: "0.2 mm",
+    4: "0.25 mm",
+    5: "0.3 mm",
+    6: "0.4 mm",
+    7: "0.5 mm",
+    8: "0.6 mm",
+    9: "0.7 mm",
+    10: "1.0 mm",
+    11: "1.5 mm",
+    12: "2.0 mm",
+    13: "3.0 mm",
+    14: "4.0 mm",
+    15: "5.0 mm",
+    16: "최대값 (=5.0 mm)"
+}
+
+
 @patch
 def set_cell_border(
     app: App,
     top=None,
     right=None,
     left=None,
     bottom=None,
@@ -815,30 +796,20 @@
     attrs = {
         "BorderTypeTop": top,
         "BorderTypeRight": right,
         "BorderTypeLeft": left,
         "BorderTypeBottom": bottom,
         "TypeHorz": horizontal,
         "TypeVert": vertical,
-        "BorderWidthTop": app.api.HwpLineWidth(f"{top_width}mm") if top_width else None,
-        "BorderWidthRight": app.api.HwpLineWidth(f"{right_width}mm")
-        if right_width
-        else None,
-        "BorderWidthLeft": app.api.HwpLineWidth(f"{left_width}mm")
-        if left_width
-        else None,
-        "BorderWidthBottom": app.api.HwpLineWidth(f"{bottom_width}mm")
-        if bottom_width
-        else None,
-        "WidthHorz": app.api.HwpLineWidth(f"{horizontal_width}mm")
-        if horizontal_width
-        else None,
-        "WidthVert": app.api.HwpLineWidth(f"{vertical_width}mm")
-        if vertical_width
-        else None,
+        "BorderWidthTop": get_value(thickness_dict, top_width),
+        "BorderWidthRight": get_value(thickness_dict, right_width),
+        "BorderWidthLeft": get_value(thickness_dict, left_width),
+        "BorderWidthBottom": get_value(thickness_dict, bottom_width),
+        "WidthHorz": get_value(thickness_dict, horizontal_width),
+        "WidthVert": get_value(thickness_dict, vertical_width),
         "BorderColorTop": app.api.RGBColor(get_rgb_tuple(top_color))
         if top_color
         else None,
         "BorderColorRight": app.api.RGBColor(get_rgb_tuple(right_color))
         if right_color
         else None,
         "BorderColorLeft": app.api.RGBColor(get_rgb_tuple(left_color))
@@ -861,15 +832,15 @@
     for key, value in attrs.items():
         if value is None:
             continue
         setattr(p, key, value)
 
     return action.run()
 
-# %% ../nbs/02_api/00_core.ipynb 46
+# %% ../nbs/02_api/00_core.ipynb 60
 @patch
 def set_cell_color(
     app: App, bg_color=None, hatch_color="#000000", hatch_style=6, alpha=None
 ):
     fill_type = windows_brush = None
     if bg_color:
         fill_type = 1
```

## hwpapi/functions.py

```diff
@@ -1,21 +1,30 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/02_api/02_functions.ipynb.
 
 # %% auto 0
-__all__ = ['dispatch', 'get_absolute_path', 'get_dll_path', 'add_dll_to_registry', 'get_registry_value', 'check_dll', 'get_value',
-           'set_charshape_pset', 'set_parashape_pset', 'hex_to_rgb', 'get_rgb_tuple']
+__all__ = ['get_font_name', 'dispatch', 'get_absolute_path', 'get_dll_path', 'add_dll_to_registry', 'get_registry_value',
+           'check_dll', 'get_value', 'get_key', 'convert2int', 'set_pset', 'get_charshape_pset', 'set_charshape_pset',
+           'get_parashape_pset', 'set_parashape_pset', 'hex_to_rgb', 'get_rgb_tuple', 'convert_to_hwp_color',
+           'convert_hwp_color_to_hex', 'mili2unit', 'unit2mili', 'point2unit', 'unit2point']
 
 # %% ../nbs/02_api/02_functions.ipynb 3
 import importlib.resources
 import os
 import shutil
 import winreg
 from pathlib import Path
+import re
+from .constants import char_fields, para_fields
 
 # %% ../nbs/02_api/02_functions.ipynb 4
+def get_font_name(text):
+    m = re.search("(^.+?)\s[A-Z0-9]+\.HFT", text)
+    return m.group(1) if m else None
+
+# %% ../nbs/02_api/02_functions.ipynb 5
 def dispatch(app_name: str):
     """캐시가 충돌하는 문제를 해결하기 위해 실행합니다. 에러가 발생할 경우 기존 캐시를 삭제하고 다시 불러옵니다."""
     try:
         from win32com import client
 
         app = client.gencache.EnsureDispatch(app_name)
     except AttributeError:
@@ -32,32 +41,32 @@
                 del sys.modules[module]
         shutil.rmtree(os.path.join(os.environ.get("LOCALAPPDATA"), "Temp", "gen_py"))
         from win32com import client
 
         app = client.gencache.EnsureDispatch(app_name)
     return app
 
-# %% ../nbs/02_api/02_functions.ipynb 5
+# %% ../nbs/02_api/02_functions.ipynb 6
 def get_absolute_path(path):
     """파일 절대 경로를 반환합니다."""
     name = Path(path)
     return name.absolute().as_posix()
 
-# %% ../nbs/02_api/02_functions.ipynb 6
+# %% ../nbs/02_api/02_functions.ipynb 7
 def get_dll_path(package_name, dll_filename):
     """패키지에서 dll 경로를 확보합니다."""
     try:
         with importlib.resources.path(package_name, dll_filename) as dll_path:
             return str(dll_path)
     except FileNotFoundError as e:
         raise FileNotFoundError(
             f"The DLL file '{dll_filename}' was not found in the package '{package_name}'."
         ) from e
 
-# %% ../nbs/02_api/02_functions.ipynb 7
+# %% ../nbs/02_api/02_functions.ipynb 8
 def add_dll_to_registry(dll_path, key_path):
     """레지스트리에 dll을 등록합니다."""
     try:
         # Connect to the registry and open the specified key
         registry_key = winreg.OpenKey(
             winreg.HKEY_CURRENT_USER, key_path, 0, winreg.KEY_SET_VALUE
         )
@@ -69,194 +78,123 @@
 
         # Close the registry key
         winreg.CloseKey(registry_key)
         print("DLL path added to registry as a string value successfully.")
     except WindowsError as e:
         print("Error while adding DLL path to registry: ", e)
 
-# %% ../nbs/02_api/02_functions.ipynb 8
+# %% ../nbs/02_api/02_functions.ipynb 9
 def get_registry_value(key_path, value_name):
     """레지스트리에 값이 있는지 확인해 봅니다."""
     try:
         with winreg.OpenKey(winreg.HKEY_CURRENT_USER, key_path) as key:
             value, value_type = winreg.QueryValueEx(key, value_name)
             return value
     except FileNotFoundError:
         return None
 
-# %% ../nbs/02_api/02_functions.ipynb 9
+# %% ../nbs/02_api/02_functions.ipynb 10
 def check_dll():
     """dll 모듈을 등록합니다."""
     dll_path = get_dll_path("hwpapi", "FilePathCheckerModuleExample.dll")
     key_path = "SOFTWARE\\HNC\\HwpAutomation\\Modules"
     value_name = "FilePathCheckerModule"
 
     value = get_registry_value(key_path, value_name)
 
     if value is None:
         add_dll_to_registry(dll_path, key_path)
     return True
 
-# %% ../nbs/02_api/02_functions.ipynb 10
+# %% ../nbs/02_api/02_functions.ipynb 11
 def get_value(dict_, key):
     """딕셔너리에서 키를 찾아 값을 반환합니다. 반환할 값이 없으면 키에러와 함께 가능한 키를 알려줍니다."""
+    if key is None:
+        return None
     try:
         return dict_[key]
     except KeyError:
         raise KeyError(
             f"{key}를 해당하는 키 중 찾을 수 없습니다. 키는 {', '.join(dict_.keys())} 중에 있어야 합니다."
         )
 
-# %% ../nbs/02_api/02_functions.ipynb 11
+# %% ../nbs/02_api/02_functions.ipynb 12
+def get_key(dict_, value):
+    """딕셔너리에서 값를 찾아 키를 반환합니다. 반환할 값이 없으면 키에러와 함께 가능한 키를 알려줍니다."""
+    if value is None:
+        return None
+    try:
+        return dict([(v, k) for k, v in dict_.items()])[value]
+    except KeyError:
+        raise KeyError(
+            f"{value}를 해당하는 키 중 찾을 수 없습니다. 키는 {', '.join(dict_.values())} 중에 있어야 합니다."
+        )
+
+# %% ../nbs/02_api/02_functions.ipynb 13
+def convert2int(_dict, value):
+    if value is None:
+        return value
+    if isinstance(value, str):
+        return get_value(_dict, value)
+    if isinstance(value, int):
+        return value
+    if isinstance(value, float):
+        return int(value)
+
+# %% ../nbs/02_api/02_functions.ipynb 14
+def set_pset(p, value_dict:dict):
+    for field in dir(p):
+        value = value_dict.get(field, None)
+        if value is None:
+            continue
+        setattr(p, field, value)
+
+    return p
+
+# %% ../nbs/02_api/02_functions.ipynb 15
+def get_charshape_pset(p):
+    return {field: getattr(p, field) for field in char_fields}
+
+# %% ../nbs/02_api/02_functions.ipynb 16
 def set_charshape_pset(
-    charshape,
-    face_name: str = None,
-    font_type: int = None,
-    size: int = None,
-    ratio: int = None,
-    spacing: int = None,
-    offset: int = None,
-    bold: bool = None,
-    italic: bool = None,
-    small_caps: bool = None,
-    emboss: bool = None,
-    super_script: bool = None,
-    sub_script: bool = None,
-    underline_type: int = None,
-    outline_type: int = None,
-    text_color=None,
-    shade_color=None,
-    underline_shape: int = None,
-    underline_color=None,
-    shadow_offset_x: int = None,
-    shadow_offset_y: int = None,
-    shadow_color=None,
-    strike_out_type=None,
-    diac_sym_mark=None,
-    use_font_space=None,
-    use_kerning=None,
-    height: int = None,
+    charshape_pset, value_dict:dict
 ):
     """
     CharShape값을 입력하기 위한 함수입니다.
-    `BorderFill`은 별도로 "BorderFill"타입을 사용하기 때문에 제외하였습니다.
+    char_fields에 정의된 키 값을 기반으로 파라미터를 세팅합니다.
     """
-    params = []
-    categories = ["Hangul", "Latin", "Hanja", "Japanese", "Other", "Symbol", "User"]
+    
+    for field in char_fields:
+        value = value_dict.get(field, None)
+        if not value:
+            continue
+        setattr(charshape_pset, field, value)
 
-    params += [("FaceName" + cat, face_name) for cat in categories] if face_name else []
-    params += [("FontType" + cat, font_type) for cat in categories] if face_name else []
-    params += [("Size" + cat, size) for cat in categories] if size else []
-    params += [("Ratio" + cat, ratio) for cat in categories] if ratio else []
-    params += [("Spacing" + cat, spacing) for cat in categories] if spacing else []
-    params += [("Offset" + cat, offset) for cat in categories] if offset else []
-
-    params += list(
-        filter(
-            lambda x: x[1] is not None,
-            [
-                ("Bold", bold),
-                ("Italic", italic),
-                ("SmallCaps", small_caps),
-                ("Emboss", emboss),
-                ("SuperScript", super_script),
-                ("SubScript", sub_script),
-                ("UnderlineType", underline_type),
-                ("OutlineType", outline_type),
-                ("TextColor", text_color),
-                ("ShadeColor", shade_color),
-                ("UnderlineShape", underline_shape),
-                ("UnderlineColor", underline_color),
-                ("ShadowOffsetX", shadow_offset_x),
-                ("ShadowOffsetY", shadow_offset_y),
-                ("ShadowColor", shadow_color),
-                ("StrikeOutType", strike_out_type),
-                ("DiacSymMark", diac_sym_mark),
-                ("UseFontSpace", use_font_space),
-                ("UseKerning", use_kerning),
-                ("Height", height),
-            ],
-        )
-    )
-    for key, value in params:
-        setattr(charshape, key, value)
+    return charshape_pset
 
-    return charshape
+# %% ../nbs/02_api/02_functions.ipynb 17
+def get_parashape_pset(p):
 
-# %% ../nbs/02_api/02_functions.ipynb 12
+    return {field: getattr(p, field) for field in para_fields}
+
+# %% ../nbs/02_api/02_functions.ipynb 18
 def set_parashape_pset(
-    parashape,
-    left_margin: int = None,
-    right_margin: int = None,
-    indentation: int = None,
-    prev_spacing: int = None,
-    next_spacing: int = None,
-    line_spacing_type: int = None,
-    line_spacing: int = None,
-    align_type: int = None,
-    break_latin_word: int = None,
-    break_non_latin_word: bool = None,
-    snap_to_grid: bool = None,
-    condense: float = None,
-    widow_orphan: bool = None,
-    keep_with_next: bool = None,
-    page_break_before: bool = None,
-    text_alignment: int = None,
-    font_line_height: int = None,
-    heading_type: int = None,
-    level: int = None,
-    border_connect: bool = None,
-    border_text: bool = None,
-    border_offset_left: int = None,
-    border_offset_right: int = None,
-    border_offset_top: int = None,
-    border_offset_bottom: int = None,
-    tail_type: bool = None,
-    line_wrap: bool = None,
+    parashape_pset, value_dict:dict,
 ):
-    params = list(
-        filter(
-            lambda x: x[1] is not None,
-            [
-                ("LeftMargin", left_margin),
-                ("RightMargin", right_margin),
-                ("Indentation", indentation),
-                ("PrevSpacing", prev_spacing),
-                ("NextSpacing", next_spacing),
-                ("LineSpacingType", line_spacing_type),
-                ("LineSpacing", line_spacing),
-                ("AlignType", align_type),
-                ("BreakLatinWord", break_latin_word),
-                ("BreakNonLatinWord", break_non_latin_word),
-                ("SnapToGrid", snap_to_grid),
-                ("Condense", condense),
-                ("WidowOrphan", widow_orphan),
-                ("KeepWithNext", keep_with_next),
-                ("PageBreakBefore", page_break_before),
-                ("TextAlignment", text_alignment),
-                ("FontLineHeight", font_line_height),
-                ("HeadingType", heading_type),
-                ("Level", level),
-                ("BorderConnect", border_connect),
-                ("BorderText", border_text),
-                ("BorderOffsetLeft", border_offset_left),
-                ("BorderOffsetRight", border_offset_right),
-                ("BorderOffsetTop", border_offset_top),
-                ("BorderOffsetBottom", border_offset_bottom),
-                ("TailType", tail_type),
-                ("LineWrap", line_wrap),
-            ],
-        )
-    )
-    for key, value in params:
-        setattr(parashape, key, value)
+ 
+    for field in para_fields:
+        value = value_dict.get(field, None)
+        if not value:
+            continue
+        setattr(parashape_pset, field, value)
 
-    return parashape
+    
+    return parashape_pset
 
-# %% ../nbs/02_api/02_functions.ipynb 13
+# %% ../nbs/02_api/02_functions.ipynb 19
 def hex_to_rgb(hex_string):
     # Remove the "#" symbol if it exists
     if hex_string.startswith("#"):
         hex_string = hex_string[1:]
 
     # Convert the hex string to decimal integers
     red = int(hex_string[0:2], 16)
@@ -305,7 +243,67 @@
             raise ValueError(f"'{color}' is not a valid hexadecimal color.")
 
         # convert the list to a tuple and return it
         return hex_to_rgb(color)
 
     else:
         raise TypeError("Input must be a string or a tuple of colors.")
+
+# %% ../nbs/02_api/02_functions.ipynb 20
+def convert_to_hwp_color(color):
+    
+    if isinstance(color, int):
+        return color 
+    
+    if isinstance(color, str):  # if the color is a string, we assume it's a hex string
+        #hwp use bgr order
+        colors = {
+            "red": "0000FF",
+            "green": "00FF00",
+            "blue": "FF0000",
+            "black": "000000",
+            "white": "FFFFFF",
+        }
+            
+        if color in colors.keys():
+            return int(colors.get(color), 16)
+        
+        # handle hex
+        m = re.search("^#?([0-9A-Fa-f]{6})$", color)
+        if m:
+            color = m.group(1)
+            return int(f"{color[4:6]}{color[2:4]}{color[0:2]}", 16)
+        
+    elif type(color) == tuple and len(color) == 3:  # if the color is a tuple, we assume it's an (R,G,B) tuple
+        return color[2]*65536 + color[1]*256 + color[0]
+    else:
+        raise ValueError(f"Unsupported color format: {color}")
+
+# %% ../nbs/02_api/02_functions.ipynb 21
+def convert_hwp_color_to_hex(color:int):
+    if not color:
+        return color
+    text = f"{color:06x}"
+    return f"#{text[4:6]}{text[2:4]}{text[:2]}"
+
+
+# %% ../nbs/02_api/02_functions.ipynb 23
+def mili2unit(value):
+    """
+    1 밀리는 283 hwpunit 입니다.
+    """
+    return int(round(value*283, 0)) if value else value
+
+# %% ../nbs/02_api/02_functions.ipynb 24
+def unit2mili(value):
+    return value/283 if value else value
+
+# %% ../nbs/02_api/02_functions.ipynb 25
+def point2unit(value):
+    """
+    1point는 100 hwpunit입니다.
+    """
+    return int(round(value*100, 0)) if value else value
+
+# %% ../nbs/02_api/02_functions.ipynb 26
+def unit2point(value):
+    return value / 100 if value else value
```

## Comparing `hwpapi-0.0.1.1.dist-info/LICENSE` & `hwpapi-0.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `hwpapi-0.0.1.1.dist-info/METADATA` & `hwpapi-0.0.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hwpapi
-Version: 0.0.1.1
+Version: 0.0.2
 Summary: python wrapper for HWPFrame.HwpObject using win32com
 Home-page: https://github.com/JunDamin/hwpapi
 Author: JunDamin
 Author-email: freedomgod@gmail.com
 License: MIT License
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

## Comparing `hwpapi-0.0.1.1.dist-info/RECORD` & `hwpapi-0.0.2.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 hwpapi/FilePathCheckerModuleExample.dll,sha256=msW5fEesiu0ei8ono-7zlBE2HY9owmJQnwxAqPnSG7Y,217229
-hwpapi/__init__.py,sha256=ry5O5SW74ugwOUMKSV2_LbWjYa8B0IEvUm7S-lHPA2c,23
-hwpapi/_modidx.py,sha256=_HBgxFjUPbA7wcPpqHMnZbVMaMzQxd4NUiCgLsKMHl8,6531
-hwpapi/actions.py,sha256=ZPXYeII1E_svHtTDsioq9kwamPk0mCjXrAa9RTHY4ZM,61638
-hwpapi/core.py,sha256=8ihDvD-uGGovpIuNuAhjt3zTtC6wx9aVbBLDP7mHWZE,31561
-hwpapi/functions.py,sha256=26Gf5D0KEHLOR86Oh6JmNq7_0_TIKgzV4ouHt_Nap6w,11113
+hwpapi/__init__.py,sha256=WNdjSeUmCefaakdgR6Iem3KXgYw8emSyMWynULSvAdY,25
+hwpapi/_modidx.py,sha256=nnEPx_-Ol8bzq9Vx57yGPMWda8cbob86sn1jl-KslxQ,26411
+hwpapi/actions.py,sha256=0NQ5uT4sPUBmhGRuuTKN-QZcsFlEsnIZ2pSQ_LLivTU,61804
+hwpapi/constants.py,sha256=KORDsh3m5xfpLvXc7cH2JGT7joT1e13NOKO7e_mlhsg,10305
+hwpapi/core.py,sha256=dxV7o5sp1l-i3xgnzlPnJOzlqsiY1l3N4UI67CEZshg,31136
+hwpapi/dataclasses.py,sha256=IsMvCD5tFJx5JJDYGDb4XIHi89gK4NA5pi0PofU5I7c,25341
+hwpapi/functions.py,sha256=p2q6TezupY_cMx-QyEikCcNDbUFfO4VfleTwWU9DrEw,10260
 nbs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 nbs/action_info.py,sha256=RJn5U63ZwPM8QIiF2FWc9r5qKwTNidwz14qVq17se70,55657
 ~bs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ~wpapi/__init__.py,sha256=ry5O5SW74ugwOUMKSV2_LbWjYa8B0IEvUm7S-lHPA2c,23
 ~wpapi/_modidx.py,sha256=Kr7Pft8mv-xCl7AOjTBNZGJu2mKKVcYZV8VyPszc8iI,5485
 ~wpapi/actions.py,sha256=wEwOfDJOvE5PwFEqWDk1OReY74SIGI3PCNKQbfUX4f8,58407
 ~wpapi/core.py,sha256=U2s3Xmz4D1zeS-B8QaZTCKKVr2WcE3HK0mndBypeilQ,22744
 ~wpapi/functions.py,sha256=5gB4HL57MeViIAi3XNS4ZwKAFaYtZKSMGS3baVfbUyY,7026
 ~wpapi/methods.py,sha256=eC375drOUIzSByAlRF84RskSX-gTJcnc469xliDljng,409
-hwpapi-0.0.1.1.dist-info/LICENSE,sha256=E9DdfH_ZB20gnAEYQSpw42Jcldul4ddSYHPJ6-nNjcI,1087
-hwpapi-0.0.1.1.dist-info/METADATA,sha256=PsVu47G5ypDvmp_KHcbkNjqw6A7mKkkmItgPcjficyc,3892
-hwpapi-0.0.1.1.dist-info/WHEEL,sha256=bC8mYJUOJCh5KnyEeT6W_BCQYi3v39D3z64Vy_sFvVg,98
-hwpapi-0.0.1.1.dist-info/entry_points.txt,sha256=FkjjiJr-NVqQoGOMIlo-SIs9wIX0TEbSDBqKUBH16p8,55
-hwpapi-0.0.1.1.dist-info/top_level.txt,sha256=8Ol3RJdZrpDEJxtcqEURTzo0K8oQGVbkXnfEWEgi-C0,22
-hwpapi-0.0.1.1.dist-info/RECORD,,
+hwpapi-0.0.2.dist-info/LICENSE,sha256=E9DdfH_ZB20gnAEYQSpw42Jcldul4ddSYHPJ6-nNjcI,1087
+hwpapi-0.0.2.dist-info/METADATA,sha256=xOLrVZ8d_RPK3kaVZe8Z97WfNAmN1YWjA8axCJ8ZsjQ,3890
+hwpapi-0.0.2.dist-info/WHEEL,sha256=bC8mYJUOJCh5KnyEeT6W_BCQYi3v39D3z64Vy_sFvVg,98
+hwpapi-0.0.2.dist-info/entry_points.txt,sha256=FkjjiJr-NVqQoGOMIlo-SIs9wIX0TEbSDBqKUBH16p8,55
+hwpapi-0.0.2.dist-info/top_level.txt,sha256=lJDupDly3vk89h3r5rthp6qv2D4438uD5TcdEawYrmg,11
+hwpapi-0.0.2.dist-info/RECORD,,
```

