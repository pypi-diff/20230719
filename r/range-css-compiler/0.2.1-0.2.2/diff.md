# Comparing `tmp/range-css-compiler-0.2.1.tar.gz` & `tmp/range-css-compiler-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "range-css-compiler-0.2.1.tar", last modified: Sun Apr 23 17:24:38 2023, max compression
+gzip compressed data, was "dist\range-css-compiler-0.2.2.tar", last modified: Wed Jul 19 11:31:37 2023, max compression
```

## Comparing `range-css-compiler-0.2.1.tar` & `range-css-compiler-0.2.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 17:24:38.675748 range-css-compiler-0.2.1/
--rw-rw-rw-   0        0        0     7942 2023-04-23 17:24:38.673226 range-css-compiler-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     6126 2023-01-29 05:44:29.000000 range-css-compiler-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 17:24:38.640781 range-css-compiler-0.2.1/range_css_compiler/
--rw-rw-rw-   0        0        0     3522 2023-01-29 09:57:10.000000 range-css-compiler-0.2.1/range_css_compiler/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 17:24:38.673226 range-css-compiler-0.2.1/range_css_compiler/parts/
--rw-rw-rw-   0        0        0     1122 2023-01-21 06:56:04.000000 range-css-compiler-0.2.1/range_css_compiler/parts/gen_compiled_rcss.py
--rw-rw-rw-   0        0        0    27318 2023-04-23 17:23:47.000000 range-css-compiler-0.2.1/range_css_compiler/parts/pypi_tool_file_binder.py
--rw-rw-rw-   0        0        0     8153 2023-01-29 08:42:39.000000 range-css-compiler-0.2.1/range_css_compiler/parts/to_qp_mat_js.py
--rw-rw-rw-   0        0        0     8739 2023-01-14 05:33:36.000000 range-css-compiler-0.2.1/range_css_compiler/parts/yaml_style_to_equid.py
--rw-rw-rw-   0        0        0      434 2023-01-21 06:30:47.000000 range-css-compiler-0.2.1/range_css_compiler/test.py
-drwxrwxrwx   0        0        0        0 2023-04-23 17:24:38.655498 range-css-compiler-0.2.1/range_css_compiler.egg-info/
--rw-rw-rw-   0        0        0     7942 2023-04-23 17:24:38.000000 range-css-compiler-0.2.1/range_css_compiler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      515 2023-04-23 17:24:38.000000 range-css-compiler-0.2.1/range_css_compiler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 17:24:38.000000 range-css-compiler-0.2.1/range_css_compiler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-04-23 17:24:38.000000 range-css-compiler-0.2.1/range_css_compiler.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       57 2023-04-23 17:24:38.000000 range-css-compiler-0.2.1/range_css_compiler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       44 2023-04-23 17:24:38.000000 range-css-compiler-0.2.1/range_css_compiler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 17:24:38.675748 range-css-compiler-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      969 2023-04-23 17:24:32.000000 range-css-compiler-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 11:31:37.000000 range-css-compiler-0.2.2/
+-rw-rw-rw-   0        0        0     7942 2023-07-19 11:31:37.000000 range-css-compiler-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6272 2023-01-29 14:08:52.000000 range-css-compiler-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-19 11:31:37.000000 range-css-compiler-0.2.2/range_css_compiler/
+-rw-rw-rw-   0        0        0     3522 2023-01-29 14:08:52.000000 range-css-compiler-0.2.2/range_css_compiler/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 11:31:37.000000 range-css-compiler-0.2.2/range_css_compiler/parts/
+-rw-rw-rw-   0        0        0     1122 2023-01-29 08:49:58.000000 range-css-compiler-0.2.2/range_css_compiler/parts/gen_compiled_rcss.py
+-rw-rw-rw-   0        0        0    27791 2023-07-19 11:29:30.000000 range-css-compiler-0.2.2/range_css_compiler/parts/pypi_tool_file_binder.py
+-rw-rw-rw-   0        0        0     8153 2023-01-29 14:08:52.000000 range-css-compiler-0.2.2/range_css_compiler/parts/to_qp_mat_js.py
+-rw-rw-rw-   0        0        0     8739 2023-01-29 08:49:58.000000 range-css-compiler-0.2.2/range_css_compiler/parts/yaml_style_to_equid.py
+-rw-rw-rw-   0        0        0      434 2023-01-29 08:49:58.000000 range-css-compiler-0.2.2/range_css_compiler/test.py
+drwxrwxrwx   0        0        0        0 2023-07-19 11:31:37.000000 range-css-compiler-0.2.2/range_css_compiler.egg-info/
+-rw-rw-rw-   0        0        0     7942 2023-07-19 11:31:35.000000 range-css-compiler-0.2.2/range_css_compiler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      515 2023-07-19 11:31:35.000000 range-css-compiler-0.2.2/range_css_compiler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 11:31:35.000000 range-css-compiler-0.2.2/range_css_compiler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-07-19 11:31:35.000000 range-css-compiler-0.2.2/range_css_compiler.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       57 2023-07-19 11:31:35.000000 range-css-compiler-0.2.2/range_css_compiler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       44 2023-07-19 11:31:35.000000 range-css-compiler-0.2.2/range_css_compiler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-19 11:31:37.000000 range-css-compiler-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      998 2023-07-19 11:30:06.000000 range-css-compiler-0.2.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `range-css-compiler-0.2.1/PKG-INFO` & `range-css-compiler-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: range-css-compiler
-Version: 0.2.1
+Version: 0.2.2
 Summary: More intuitive HTML placement and assignment tool than CSS.
 Home-page: https://github.co.jp/
 Author: le_lattelle
 Author-email: g.tiger.ml@gmail.com
 License: CC0 v1.0
 Description: # range-css-compiler
```

### Comparing `range-css-compiler-0.2.1/README.md` & `range-css-compiler-0.2.2/README.md`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,146 +1,146 @@
-# range-css-compiler
-
-下の方に日本語の説明があります
-
-## Overview
-- More intuitive HTML placement and assignment tool than CSS.
-- Intuitive HTML alignment instructions with "Specify by Range".
-- Works by equational handling of assignment mutual binding of upper and lower levels of hierarchy like CAD.
-- under construction
-
-## Usage
-You can execute the following command in the console:
-```sh
-rcss -i RangeCSS_style_filename.yml
-```
-
-The detailed options of the `rcss` command are specified in the following syntax:
-
-```sh
-rcss -i [input yaml file path (RangeCSS style file)] [-o [output javascript file path]] [-l]
-```
-
-The explanations of each command line argument are as follows:
-
-- -i (--input) : Specifies the path of the input yaml file (RangeCSS style file). This is required.
-- -o (--output) : Specifies the path of the output javascript file. This is optional. If omitted, the file name will only change the extension from the input file path.
-- -l (--loop) : Enables loop compile mode. In loop compile mode, changes to the yaml file are detected and compilation is automatically executed. If this argument is not specified, it will only be compiled once.
-
-Please refer to `## How to write rcss_style.yml` for information on how to write a RangeCSS style file.
-
-## How to write rcss_style.yml
-```yaml
-rcss_frame: # The rcss_id of the element (the outermost element must be 'rcss_frame')
-  css_id: rcss_frame # The id of the element in html
-  children: [header, main] # List of rcss_id of child elements
-  align: vertical # Alignment of child elements (vertical(default) or horizontal)
-header:
-  children: []
-  css_id: header
-  margin_y0: 10px # Top margin in the vertical direction (omitted if 0. Not shared with the top element's margin)
-  width: "~" # Width of the element. Refer to `## Range-based specification format` for the method of specifying it.
-  height: 70px # Height of the element
-main:
-  children: [some_other_element]
-  align: horizontal
-  css_id: main
-  margin_y0: 10px
-  margin_y1: 10px # Bottom margin in the vertical direction
-  width: "~"
-  height: "~"
-```
-
-## Range-based specification format
-
-- Absolute value specification: `10px`
-- Range specification: `10px~20px`
-- Range specification without lower limit: `~20px`
-- Range specification without upper and lower limit: `~`
-- Basic value specification: `10px~100px[50px]`
-
-## Reference: List of attributes
-`(default: ...)` means default value without specification
-```
-css_id: The id of the element in html
-children: List of rcss_id of child elements (default: [])
-align: Alignment direction of child elements (default: vertical)
-width: Width of the element (default: ~)
-height: Height of the element (default: ~)
-margin_x0: Left margin in the horizontal direction (default: 0px)
-margin_x1: Right margin in the horizontal direction (default: 0px)
-margin_y0: Top margin in the vertical direction (default: 0px)
-margin_y1: Bottom margin in the vertical direction (default: 0px)
-```
-
-## license info
-The npm tool 'quadprog' is used under the MIT license. (https://www.npmjs.com/package/quadprog)
-
-
-## 概略
-- CSSよりも直感的なHTMLの配置・割り付けツール
-- 「範囲による指定」でHTMLの配置を直感的に指示できる
-- 上位・下位階層の割り付け相互束縛をCADのように方程式的に取り扱うことで動作する。
-- 説明文は執筆中です
-
-## 利用例
-コンソールから下記のように実行することができます
-```sh
-rcss -i RangeCSS_style_filename.yml
-```
-
-`rcss`コマンドの細かいオプションの指定は下記のような文法に従います:
-```sh
-rcss -i [入力yamlファイルパス(RangeCSSのスタイルファイル)] [-o [出力javascriptファイルパス]] [-l]
-```
-
-各コマンドライン引数の説明は下記の通りです:
-
-- -i (--input) : 入力yamlファイル(RangeCSSのスタイルファイル)のパスを指定します。これは必須です。
-- -o (--output) : 出力javascriptファイルのパスを指定します。これは任意です。省略された場合は入力ファイルパスから同ファイル名で拡張子のみ変更されます。
-- -l (--loop) : ループコンパイルモードを有効にします。ループコンパイルモードではyamlファイルの変更を検知して自動的にコンパイルが実行されます。この引数を指定しない場合、1回のみコンパイルされます
-
-RangeCSS スタイルファイルの書き方は `## rcss_style.yml の書き方` を参照してください
-
-## rcss_style.yml の書き方
-```yaml
-rcss_frame:	# その要素のrcss_id (一番外側は`rcss_frame`である必要がある)
-  css_id: rcss_frame	# html内のその要素のid
-  children: [header, main]	# 子要素のrcss_idのリスト
-  align: vertical	# 子要素の配置 (vertical(default) もしくは horizontal)
-header:
-  children: []
-  css_id: header
-  margin_y0: 10px	# 縦方向の上側のマージン (省略されると0となる。上要素のマージンと共有されない)
-  width: "~"	# 要素の幅。`~`などの指定方法は、`## 範囲による指定の形式` を参照
-  height: 70px	# 要素の高さ
-main:
-  children: [some_other_element]
-  align: horizontal
-  css_id: main
-  margin_y0: 10px
-  margin_y1: 10px	# 縦方向の下側のマージン
-  width: "~"
-  height: "~"
-```
-
-## 範囲による指定の形式
-- 絶対値指定: `10px`
-- 範囲指定: `10px~20px`
-- 下限のない範囲指定: `~20px`
-- 上限・下限なし: `~`
-- 基本値の指定: `10px~100px[50px]`
-
-## 参考: 属性の一覧
-`(default: ...)`は指定なしの場合のデフォルト値
-
-```
-css_id: html内のその要素のid
-children: 子要素のrcss_idのリスト (default: [])
-align: 子要素の配置方向 (default: vertical)
-width: 要素の幅 (default: ~)
-height: 要素の高さ (default: ~)
-margin_x0: 横方向の左側のマージン (default: 0px)
-margin_x1: 横方向の右側のマージン (default: 0px)
-margin_y0: 縦方向の上側のマージン (default: 0px)
-margin_y1: 縦方向の下側のマージン (default: 0px)
-```
+# range-css-compiler
+
+下の方に日本語の説明があります
+
+## Overview
+- More intuitive HTML placement and assignment tool than CSS.
+- Intuitive HTML alignment instructions with "Specify by Range".
+- Works by equational handling of assignment mutual binding of upper and lower levels of hierarchy like CAD.
+- under construction
+
+## Usage
+You can execute the following command in the console:
+```sh
+rcss -i RangeCSS_style_filename.yml
+```
+
+The detailed options of the `rcss` command are specified in the following syntax:
+
+```sh
+rcss -i [input yaml file path (RangeCSS style file)] [-o [output javascript file path]] [-l]
+```
+
+The explanations of each command line argument are as follows:
+
+- -i (--input) : Specifies the path of the input yaml file (RangeCSS style file). This is required.
+- -o (--output) : Specifies the path of the output javascript file. This is optional. If omitted, the file name will only change the extension from the input file path.
+- -l (--loop) : Enables loop compile mode. In loop compile mode, changes to the yaml file are detected and compilation is automatically executed. If this argument is not specified, it will only be compiled once.
+
+Please refer to `## How to write rcss_style.yml` for information on how to write a RangeCSS style file.
+
+## How to write rcss_style.yml
+```yaml
+rcss_frame: # The rcss_id of the element (the outermost element must be 'rcss_frame')
+  css_id: rcss_frame # The id of the element in html
+  children: [header, main] # List of rcss_id of child elements
+  align: vertical # Alignment of child elements (vertical(default) or horizontal)
+header:
+  children: []
+  css_id: header
+  margin_y0: 10px # Top margin in the vertical direction (omitted if 0. Not shared with the top element's margin)
+  width: "~" # Width of the element. Refer to `## Range-based specification format` for the method of specifying it.
+  height: 70px # Height of the element
+main:
+  children: [some_other_element]
+  align: horizontal
+  css_id: main
+  margin_y0: 10px
+  margin_y1: 10px # Bottom margin in the vertical direction
+  width: "~"
+  height: "~"
+```
+
+## Range-based specification format
+
+- Absolute value specification: `10px`
+- Range specification: `10px~20px`
+- Range specification without lower limit: `~20px`
+- Range specification without upper and lower limit: `~`
+- Basic value specification: `10px~100px[50px]`
+
+## Reference: List of attributes
+`(default: ...)` means default value without specification
+```
+css_id: The id of the element in html
+children: List of rcss_id of child elements (default: [])
+align: Alignment direction of child elements (default: vertical)
+width: Width of the element (default: ~)
+height: Height of the element (default: ~)
+margin_x0: Left margin in the horizontal direction (default: 0px)
+margin_x1: Right margin in the horizontal direction (default: 0px)
+margin_y0: Top margin in the vertical direction (default: 0px)
+margin_y1: Bottom margin in the vertical direction (default: 0px)
+```
+
+## license info
+The npm tool 'quadprog' is used under the MIT license. (https://www.npmjs.com/package/quadprog)
+
+
+## 概略
+- CSSよりも直感的なHTMLの配置・割り付けツール
+- 「範囲による指定」でHTMLの配置を直感的に指示できる
+- 上位・下位階層の割り付け相互束縛をCADのように方程式的に取り扱うことで動作する。
+- 説明文は執筆中です
+
+## 利用例
+コンソールから下記のように実行することができます
+```sh
+rcss -i RangeCSS_style_filename.yml
+```
+
+`rcss`コマンドの細かいオプションの指定は下記のような文法に従います:
+```sh
+rcss -i [入力yamlファイルパス(RangeCSSのスタイルファイル)] [-o [出力javascriptファイルパス]] [-l]
+```
+
+各コマンドライン引数の説明は下記の通りです:
+
+- -i (--input) : 入力yamlファイル(RangeCSSのスタイルファイル)のパスを指定します。これは必須です。
+- -o (--output) : 出力javascriptファイルのパスを指定します。これは任意です。省略された場合は入力ファイルパスから同ファイル名で拡張子のみ変更されます。
+- -l (--loop) : ループコンパイルモードを有効にします。ループコンパイルモードではyamlファイルの変更を検知して自動的にコンパイルが実行されます。この引数を指定しない場合、1回のみコンパイルされます
+
+RangeCSS スタイルファイルの書き方は `## rcss_style.yml の書き方` を参照してください
+
+## rcss_style.yml の書き方
+```yaml
+rcss_frame:	# その要素のrcss_id (一番外側は`rcss_frame`である必要がある)
+  css_id: rcss_frame	# html内のその要素のid
+  children: [header, main]	# 子要素のrcss_idのリスト
+  align: vertical	# 子要素の配置 (vertical(default) もしくは horizontal)
+header:
+  children: []
+  css_id: header
+  margin_y0: 10px	# 縦方向の上側のマージン (省略されると0となる。上要素のマージンと共有されない)
+  width: "~"	# 要素の幅。`~`などの指定方法は、`## 範囲による指定の形式` を参照
+  height: 70px	# 要素の高さ
+main:
+  children: [some_other_element]
+  align: horizontal
+  css_id: main
+  margin_y0: 10px
+  margin_y1: 10px	# 縦方向の下側のマージン
+  width: "~"
+  height: "~"
+```
+
+## 範囲による指定の形式
+- 絶対値指定: `10px`
+- 範囲指定: `10px~20px`
+- 下限のない範囲指定: `~20px`
+- 上限・下限なし: `~`
+- 基本値の指定: `10px~100px[50px]`
+
+## 参考: 属性の一覧
+`(default: ...)`は指定なしの場合のデフォルト値
+
+```
+css_id: html内のその要素のid
+children: 子要素のrcss_idのリスト (default: [])
+align: 子要素の配置方向 (default: vertical)
+width: 要素の幅 (default: ~)
+height: 要素の高さ (default: ~)
+margin_x0: 横方向の左側のマージン (default: 0px)
+margin_x1: 横方向の右側のマージン (default: 0px)
+margin_y0: 縦方向の上側のマージン (default: 0px)
+margin_y1: 縦方向の下側のマージン (default: 0px)
+```
```

### Comparing `range-css-compiler-0.2.1/range_css_compiler/__init__.py` & `range-css-compiler-0.2.2/range_css_compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `range-css-compiler-0.2.1/range_css_compiler/parts/gen_compiled_rcss.py` & `range-css-compiler-0.2.2/range_css_compiler/parts/gen_compiled_rcss.py`

 * *Files identical despite different names*

### Comparing `range-css-compiler-0.2.1/range_css_compiler/parts/pypi_tool_file_binder.py` & `range-css-compiler-0.2.2/range_css_compiler/parts/pypi_tool_file_binder.py`

 * *Files 5% similar despite different names*

```diff
@@ -915,26 +915,30 @@
 
 /* rcssのスタイルをhtmlの配置に適用するapplierの部品 */
 APPLIER_UTILS
 
 // スタイル適用関数 (部分適用・前回実行中に次回が呼び出されないように)
 wa_running = false;
 function wrapped_apply(){
-	// 前回の処理が未完了の場合に処理しない
-	if (wa_running == true) {return;}
-	// 処理中
-	wa_running = true;
-	// 最適化計算
-	var frame_info = calc_frame_info();	// frameのオフセット位置・サイズの計算
-	var rcss_solved_style = style_opt(frame_info);	// 配置最適化計算
-	// スタイル適用関数
-	apply_rcss_style(rcss_solved_style);
-	// 処理完了
-	wa_running = false;
+    // 前回の処理が未完了の場合に処理しない
+    if (wa_running == true) {return;}
+    // 処理中
+    wa_running = true;
+    // 配置最適化・スタイル適用の前処理関数を実行 (関数が存在しない場合・型が異なる場合はなにもしない)
+    if (typeof before_wa_func === 'function') {before_wa_func();}
+    // 最適化計算
+    var frame_info = calc_frame_info(); // frameのオフセット位置・サイズの計算
+    var rcss_solved_style = style_opt(frame_info);  // 配置最適化計算
+    // スタイル適用関数
+    apply_rcss_style(rcss_solved_style);
+    // 配置最適化・スタイル適用の後処理関数を実行 (関数が存在しない場合・型が異なる場合はなにもしない)
+    if (typeof after_wa_func === 'function') {after_wa_func();}
+    // 処理完了
+    wa_running = false;
 }
 
 // サイズ変更・スクロールイベントでスタイル再適用
-window.addEventListener('scroll', wrapped_apply);	// スタイル適用関数 (style情報を部分適用)
-window.addEventListener('resize', wrapped_apply);	// スタイル適用関数 (style情報を部分適用)
+window.addEventListener('scroll', wrapped_apply);   // スタイル適用関数 (style情報を部分適用)
+window.addEventListener('resize', wrapped_apply);   // スタイル適用関数 (style情報を部分適用)
 // 初回に1回スタイル適用
-wrapped_apply();	// スタイル適用関数 (style情報を部分適用)
+wrapped_apply();    // スタイル適用関数 (style情報を部分適用)
 """
```

### Comparing `range-css-compiler-0.2.1/range_css_compiler/parts/to_qp_mat_js.py` & `range-css-compiler-0.2.2/range_css_compiler/parts/to_qp_mat_js.py`

 * *Files identical despite different names*

### Comparing `range-css-compiler-0.2.1/range_css_compiler/parts/yaml_style_to_equid.py` & `range-css-compiler-0.2.2/range_css_compiler/parts/yaml_style_to_equid.py`

 * *Files identical despite different names*

### Comparing `range-css-compiler-0.2.1/range_css_compiler.egg-info/PKG-INFO` & `range-css-compiler-0.2.2/range_css_compiler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: range-css-compiler
-Version: 0.2.1
+Version: 0.2.2
 Summary: More intuitive HTML placement and assignment tool than CSS.
 Home-page: https://github.co.jp/
 Author: le_lattelle
 Author-email: g.tiger.ml@gmail.com
 License: CC0 v1.0
 Description: # range-css-compiler
```

### Comparing `range-css-compiler-0.2.1/range_css_compiler.egg-info/SOURCES.txt` & `range-css-compiler-0.2.2/range_css_compiler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `range-css-compiler-0.2.1/setup.py` & `range-css-compiler-0.2.2/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,61 +1,63 @@
-00000000: 0a66 726f 6d20 7365 7475 7074 6f6f 6c73  .from setuptools
-00000010: 2069 6d70 6f72 7420 7365 7475 700a 2320   import setup.# 
-00000020: e585 ace9 968b e794 a8e3 8391 e383 83e3  ................
-00000030: 82b1 e383 bce3 82b8 e381 aee4 bd9c e688  ................
-00000040: 9020 5b65 7a70 6970 5d0a 696d 706f 7274  . [ezpip].import
-00000050: 2065 7a70 6970 0a0a 2320 e585 ace9 968b   ezpip..# ......
-00000060: e794 a8e3 8391 e383 83e3 82b1 e383 bce3  ................
-00000070: 82b8 e381 aee4 bd9c e688 9020 5b65 7a70  ........... [ezp
-00000080: 6970 5d0a 7769 7468 2065 7a70 6970 2e70  ip].with ezpip.p
-00000090: 6163 6b61 6765 7228 6465 7665 6c6f 705f  ackager(develop_
-000000a0: 6469 7220 3d20 222e 2f5f 6465 7665 6c6f  dir = "./_develo
-000000b0: 705f 7261 6e67 655f 6373 735f 636f 6d70  p_range_css_comp
-000000c0: 696c 6572 2f22 2920 6173 2070 3a0a 0973  iler/") as p:..s
-000000d0: 6574 7570 280a 0909 6e61 6d65 203d 2022  etup(...name = "
-000000e0: 7261 6e67 652d 6373 732d 636f 6d70 696c  range-css-compil
-000000f0: 6572 222c 0a09 0976 6572 7369 6f6e 203d  er",...version =
-00000100: 2022 302e 322e 3122 2c0a 0909 6465 7363   "0.2.1",...desc
-00000110: 7269 7074 696f 6e20 3d20 224d 6f72 6520  ription = "More 
-00000120: 696e 7475 6974 6976 6520 4854 4d4c 2070  intuitive HTML p
-00000130: 6c61 6365 6d65 6e74 2061 6e64 2061 7373  lacement and ass
-00000140: 6967 6e6d 656e 7420 746f 6f6c 2074 6861  ignment tool tha
-00000150: 6e20 4353 532e 222c 0a09 0961 7574 686f  n CSS.",...autho
-00000160: 7220 3d20 226c 655f 6c61 7474 656c 6c65  r = "le_lattelle
-00000170: 222c 0a09 0961 7574 686f 725f 656d 6169  ",...author_emai
-00000180: 6c20 3d20 2267 2e74 6967 6572 2e6d 6c40  l = "g.tiger.ml@
-00000190: 676d 6169 6c2e 636f 6d22 2c0a 0909 7572  gmail.com",...ur
-000001a0: 6c20 3d20 2268 7474 7073 3a2f 2f67 6974  l = "https://git
-000001b0: 6875 622e 636f 2e6a 702f 222c 0a09 0970  hub.co.jp/",...p
-000001c0: 6163 6b61 6765 7320 3d20 702e 7061 636b  ackages = p.pack
-000001d0: 6167 6573 2c0a 0909 696e 7374 616c 6c5f  ages,...install_
-000001e0: 7265 7175 6972 6573 203d 205b 2272 656c  requires = ["rel
-000001f0: 7061 7468 222c 2022 657a 7069 7022 2c20  path", "ezpip", 
-00000200: 2273 6f75 7422 2c20 2266 6965 7322 2c20  "sout", "fies", 
-00000210: 2274 7164 6d22 2c20 2265 7175 6964 222c  "tqdm", "equid",
-00000220: 2022 696e 6465 6e74 2d74 656d 706c 6174   "indent-templat
-00000230: 6522 2c20 2265 7a70 746e 225d 2c0a 0909  e", "ezptn"],...
-00000240: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
-00000250: 203d 2070 2e6c 6f6e 675f 6465 7363 7269   = p.long_descri
-00000260: 7074 696f 6e2c 0a09 096c 6f6e 675f 6465  ption,...long_de
-00000270: 7363 7269 7074 696f 6e5f 636f 6e74 656e  scription_conten
-00000280: 745f 7479 7065 203d 2022 7465 7874 2f6d  t_type = "text/m
-00000290: 6172 6b64 6f77 6e22 2c0a 0909 6c69 6365  arkdown",...lice
-000002a0: 6e73 6520 3d20 2243 4330 2076 312e 3022  nse = "CC0 v1.0"
-000002b0: 2c0a 0909 636c 6173 7369 6669 6572 7320  ,...classifiers 
-000002c0: 3d20 5b0a 0909 0922 5072 6f67 7261 6d6d  = [...."Programm
-000002d0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-000002e0: 5079 7468 6f6e 203a 3a20 3322 2c0a 0909  Python :: 3",...
-000002f0: 0922 546f 7069 6320 3a3a 2053 6f66 7477  ."Topic :: Softw
-00000300: 6172 6520 4465 7665 6c6f 706d 656e 7420  are Development 
-00000310: 3a3a 204c 6962 7261 7269 6573 222c 0a09  :: Libraries",..
-00000320: 0909 224c 6963 656e 7365 203a 3a20 4343  .."License :: CC
-00000330: 3020 312e 3020 556e 6976 6572 7361 6c20  0 1.0 Universal 
-00000340: 2843 4330 2031 2e30 2920 5075 626c 6963  (CC0 1.0) Public
-00000350: 2044 6f6d 6169 6e20 4465 6469 6361 7469   Domain Dedicati
-00000360: 6f6e 220a 0909 5d2c 0a09 0965 6e74 7279  on"...],...entry
-00000370: 5f70 6f69 6e74 7320 3d20 2222 220a 0909  _points = """...
-00000380: 095b 636f 6e73 6f6c 655f 7363 7269 7074  .[console_script
-00000390: 735d 0a09 0909 7263 7373 203d 2072 616e  s]....rcss = ran
-000003a0: 6765 5f63 7373 5f63 6f6d 7069 6c65 723a  ge_css_compiler:
-000003b0: 636f 6e73 6f6c 655f 636f 6d6d 616e 640a  console_command.
-000003c0: 0909 2222 220a 0929 0a                   .."""..).
+00000000: 0d0a 6672 6f6d 2073 6574 7570 746f 6f6c  ..from setuptool
+00000010: 7320 696d 706f 7274 2073 6574 7570 0d0a  s import setup..
+00000020: 2320 e585 ace9 968b e794 a8e3 8391 e383  # ..............
+00000030: 83e3 82b1 e383 bce3 82b8 e381 aee4 bd9c  ................
+00000040: e688 9020 5b65 7a70 6970 5d0d 0a69 6d70  ... [ezpip]..imp
+00000050: 6f72 7420 657a 7069 700d 0a0d 0a23 20e5  ort ezpip....# .
+00000060: 85ac e996 8be7 94a8 e383 91e3 8383 e382  ................
+00000070: b1e3 83bc e382 b8e3 81ae e4bd 9ce6 8890  ................
+00000080: 205b 657a 7069 705d 0d0a 7769 7468 2065   [ezpip]..with e
+00000090: 7a70 6970 2e70 6163 6b61 6765 7228 6465  zpip.packager(de
+000000a0: 7665 6c6f 705f 6469 7220 3d20 222e 2f5f  velop_dir = "./_
+000000b0: 6465 7665 6c6f 705f 7261 6e67 655f 6373  develop_range_cs
+000000c0: 735f 636f 6d70 696c 6572 2f22 2920 6173  s_compiler/") as
+000000d0: 2070 3a0d 0a09 7365 7475 7028 0d0a 0909   p:...setup(....
+000000e0: 6e61 6d65 203d 2022 7261 6e67 652d 6373  name = "range-cs
+000000f0: 732d 636f 6d70 696c 6572 222c 0d0a 0909  s-compiler",....
+00000100: 7665 7273 696f 6e20 3d20 2230 2e32 2e32  version = "0.2.2
+00000110: 222c 0d0a 0909 6465 7363 7269 7074 696f  ",....descriptio
+00000120: 6e20 3d20 224d 6f72 6520 696e 7475 6974  n = "More intuit
+00000130: 6976 6520 4854 4d4c 2070 6c61 6365 6d65  ive HTML placeme
+00000140: 6e74 2061 6e64 2061 7373 6967 6e6d 656e  nt and assignmen
+00000150: 7420 746f 6f6c 2074 6861 6e20 4353 532e  t tool than CSS.
+00000160: 222c 0d0a 0909 6175 7468 6f72 203d 2022  ",....author = "
+00000170: 6c65 5f6c 6174 7465 6c6c 6522 2c0d 0a09  le_lattelle",...
+00000180: 0961 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
+00000190: 2267 2e74 6967 6572 2e6d 6c40 676d 6169  "g.tiger.ml@gmai
+000001a0: 6c2e 636f 6d22 2c0d 0a09 0975 726c 203d  l.com",....url =
+000001b0: 2022 6874 7470 733a 2f2f 6769 7468 7562   "https://github
+000001c0: 2e63 6f2e 6a70 2f22 2c0d 0a09 0970 6163  .co.jp/",....pac
+000001d0: 6b61 6765 7320 3d20 702e 7061 636b 6167  kages = p.packag
+000001e0: 6573 2c0d 0a09 0969 6e73 7461 6c6c 5f72  es,....install_r
+000001f0: 6571 7569 7265 7320 3d20 5b22 7265 6c70  equires = ["relp
+00000200: 6174 6822 2c20 2265 7a70 6970 222c 2022  ath", "ezpip", "
+00000210: 736f 7574 222c 2022 6669 6573 222c 2022  sout", "fies", "
+00000220: 7471 646d 222c 2022 6571 7569 6422 2c20  tqdm", "equid", 
+00000230: 2269 6e64 656e 742d 7465 6d70 6c61 7465  "indent-template
+00000240: 222c 2022 657a 7074 6e22 5d2c 0d0a 0909  ", "ezptn"],....
+00000250: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
+00000260: 203d 2070 2e6c 6f6e 675f 6465 7363 7269   = p.long_descri
+00000270: 7074 696f 6e2c 0d0a 0909 6c6f 6e67 5f64  ption,....long_d
+00000280: 6573 6372 6970 7469 6f6e 5f63 6f6e 7465  escription_conte
+00000290: 6e74 5f74 7970 6520 3d20 2274 6578 742f  nt_type = "text/
+000002a0: 6d61 726b 646f 776e 222c 0d0a 0909 6c69  markdown",....li
+000002b0: 6365 6e73 6520 3d20 2243 4330 2076 312e  cense = "CC0 v1.
+000002c0: 3022 2c0d 0a09 0963 6c61 7373 6966 6965  0",....classifie
+000002d0: 7273 203d 205b 0d0a 0909 0922 5072 6f67  rs = [....."Prog
+000002e0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+000002f0: 203a 3a20 5079 7468 6f6e 203a 3a20 3322   :: Python :: 3"
+00000300: 2c0d 0a09 0909 2254 6f70 6963 203a 3a20  ,....."Topic :: 
+00000310: 536f 6674 7761 7265 2044 6576 656c 6f70  Software Develop
+00000320: 6d65 6e74 203a 3a20 4c69 6272 6172 6965  ment :: Librarie
+00000330: 7322 2c0d 0a09 0909 224c 6963 656e 7365  s",....."License
+00000340: 203a 3a20 4343 3020 312e 3020 556e 6976   :: CC0 1.0 Univ
+00000350: 6572 7361 6c20 2843 4330 2031 2e30 2920  ersal (CC0 1.0) 
+00000360: 5075 626c 6963 2044 6f6d 6169 6e20 4465  Public Domain De
+00000370: 6469 6361 7469 6f6e 220d 0a09 095d 2c0d  dication"....],.
+00000380: 0a09 0965 6e74 7279 5f70 6f69 6e74 7320  ...entry_points 
+00000390: 3d20 2222 220d 0a09 0909 5b63 6f6e 736f  = """.....[conso
+000003a0: 6c65 5f73 6372 6970 7473 5d0d 0a09 0909  le_scripts].....
+000003b0: 7263 7373 203d 2072 616e 6765 5f63 7373  rcss = range_css
+000003c0: 5f63 6f6d 7069 6c65 723a 636f 6e73 6f6c  _compiler:consol
+000003d0: 655f 636f 6d6d 616e 640d 0a09 0922 2222  e_command...."""
+000003e0: 0d0a 0929 0d0a                           ...)..
```

