# Comparing `tmp/fundialogues-0.0.6.tar.gz` & `tmp/fundialogues-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fundialogues-0.0.6.tar", last modified: Wed Jul 19 05:03:15 2023, max compression
+gzip compressed data, was "fundialogues-0.0.7.tar", last modified: Wed Jul 19 05:09:30 2023, max compression
```

## Comparing `fundialogues-0.0.6.tar` & `fundialogues-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 05:03:15.768939 fundialogues-0.0.6/
--rw-rw-rw-   0        0        0    11558 2023-07-15 20:46:39.000000 fundialogues-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     5986 2023-07-19 05:03:15.769939 fundialogues-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     5331 2023-07-19 04:51:14.000000 fundialogues-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-19 05:03:15.750923 fundialogues-0.0.6/fun_dialogues/
-drwxrwxrwx   0        0        0        0 2023-07-19 05:03:15.766937 fundialogues-0.0.6/fun_dialogues/fundialogues.egg-info/
--rw-rw-rw-   0        0        0     5986 2023-07-19 05:03:15.000000 fundialogues-0.0.6/fun_dialogues/fundialogues.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-07-19 05:03:15.000000 fundialogues-0.0.6/fun_dialogues/fundialogues.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-19 05:03:15.000000 fundialogues-0.0.6/fun_dialogues/fundialogues.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-19 05:03:15.000000 fundialogues-0.0.6/fun_dialogues/fundialogues.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-19 05:03:15.768939 fundialogues-0.0.6/fun_dialogues/utils/
--rw-rw-rw-   0        0        0       35 2023-07-19 05:02:09.000000 fundialogues-0.0.6/fun_dialogues/utils/__init__.py
--rw-rw-rw-   0        0        0      783 2023-07-17 04:02:00.000000 fundialogues-0.0.6/fun_dialogues/utils/dialoader.py
--rw-rw-rw-   0        0        0       86 2023-07-17 04:42:30.000000 fundialogues-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0      814 2023-07-19 05:03:15.770940 fundialogues-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-19 05:09:30.343152 fundialogues-0.0.7/
+-rw-rw-rw-   0        0        0    11558 2023-07-15 20:46:39.000000 fundialogues-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     5986 2023-07-19 05:09:30.344153 fundialogues-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     5331 2023-07-19 04:51:14.000000 fundialogues-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-19 05:09:30.317129 fundialogues-0.0.7/fundialogues/
+drwxrwxrwx   0        0        0        0 2023-07-19 05:09:30.340149 fundialogues-0.0.7/fundialogues/fundialogues.egg-info/
+-rw-rw-rw-   0        0        0     5986 2023-07-19 05:09:30.000000 fundialogues-0.0.7/fundialogues/fundialogues.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      301 2023-07-19 05:09:30.000000 fundialogues-0.0.7/fundialogues/fundialogues.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 05:09:30.000000 fundialogues-0.0.7/fundialogues/fundialogues.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-19 05:09:30.000000 fundialogues-0.0.7/fundialogues/fundialogues.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-19 05:09:30.343152 fundialogues-0.0.7/fundialogues/utils/
+-rw-rw-rw-   0        0        0       35 2023-07-19 05:02:09.000000 fundialogues-0.0.7/fundialogues/utils/__init__.py
+-rw-rw-rw-   0        0        0      783 2023-07-17 04:02:00.000000 fundialogues-0.0.7/fundialogues/utils/dialoader.py
+-rw-rw-rw-   0        0        0       86 2023-07-17 04:42:30.000000 fundialogues-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0      812 2023-07-19 05:09:30.350159 fundialogues-0.0.7/setup.cfg
```

### Comparing `fundialogues-0.0.6/LICENSE` & `fundialogues-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `fundialogues-0.0.6/PKG-INFO` & `fundialogues-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fundialogues
-Version: 0.0.6
+Version: 0.0.7
 Summary: a package with fictitous dialogue datasets and tools to help learn how to build chatbots and do basic prototyping.
 Home-page: https://github.com/eduand-alvarez/fun-dialogues/tree/main
 Author: Eduardo Alvarez
 Author-email: eduand.alvarez@gmail.com
 Project-URL: Bug Tracker, https://github.com/eduand-alvarez/fun-dialogues/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `fundialogues-0.0.6/README.md` & `fundialogues-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `fundialogues-0.0.6/fun_dialogues/fundialogues.egg-info/PKG-INFO` & `fundialogues-0.0.7/fundialogues/fundialogues.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fundialogues
-Version: 0.0.6
+Version: 0.0.7
 Summary: a package with fictitous dialogue datasets and tools to help learn how to build chatbots and do basic prototyping.
 Home-page: https://github.com/eduand-alvarez/fun-dialogues/tree/main
 Author: Eduardo Alvarez
 Author-email: eduand.alvarez@gmail.com
 Project-URL: Bug Tracker, https://github.com/eduand-alvarez/fun-dialogues/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `fundialogues-0.0.6/fun_dialogues/utils/dialoader.py` & `fundialogues-0.0.7/fundialogues/utils/dialoader.py`

 * *Files identical despite different names*

### Comparing `fundialogues-0.0.6/setup.cfg` & `fundialogues-0.0.7/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2066 756e 6469 616c 6f67 7565 730d   = fundialogues.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e30 2e36  .version = 0.0.6
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e30 2e37  .version = 0.0.7
 00000030: 0d0a 6175 7468 6f72 203d 2045 6475 6172  ..author = Eduar
 00000040: 646f 2041 6c76 6172 657a 0d0a 6175 7468  do Alvarez..auth
 00000050: 6f72 5f65 6d61 696c 203d 2065 6475 616e  or_email = eduan
 00000060: 642e 616c 7661 7265 7a40 676d 6169 6c2e  d.alvarez@gmail.
 00000070: 636f 6d0d 0a64 6573 6372 6970 7469 6f6e  com..description
 00000080: 203d 2061 2070 6163 6b61 6765 2077 6974   = a package wit
 00000090: 6820 6669 6374 6974 6f75 7320 6469 616c  h fictitous dial
@@ -35,17 +35,17 @@
 00000220: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
 00000230: 6420 3a3a 2041 7061 6368 6520 536f 6674  d :: Apache Soft
 00000240: 7761 7265 204c 6963 656e 7365 0d0a 094f  ware License...O
 00000250: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
 00000260: 3a3a 204f 5320 496e 6465 7065 6e64 656e  :: OS Independen
 00000270: 740d 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a  t....[options]..
 00000280: 7061 636b 6167 655f 6469 7220 3d20 0d0a  package_dir = ..
-00000290: 093d 2066 756e 5f64 6961 6c6f 6775 6573  .= fun_dialogues
-000002a0: 0d0a 7061 636b 6167 6573 203d 2066 696e  ..packages = fin
-000002b0: 643a 0d0a 7079 7468 6f6e 5f72 6571 7569  d:..python_requi
-000002c0: 7265 7320 3d20 3e3d 332e 382e 3130 0d0a  res = >=3.8.10..
-000002d0: 0d0a 5b6f 7074 696f 6e73 2e70 6163 6b61  ..[options.packa
-000002e0: 6765 732e 6669 6e64 5d0d 0a77 6865 7265  ges.find]..where
-000002f0: 203d 2066 756e 5f64 6961 6c6f 6775 6573   = fun_dialogues
-00000300: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
-00000310: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
-00000320: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
+00000290: 093d 2066 756e 6469 616c 6f67 7565 730d  .= fundialogues.
+000002a0: 0a70 6163 6b61 6765 7320 3d20 6669 6e64  .packages = find
+000002b0: 3a0d 0a70 7974 686f 6e5f 7265 7175 6972  :..python_requir
+000002c0: 6573 203d 203e 3d33 2e38 2e31 300d 0a0d  es = >=3.8.10...
+000002d0: 0a5b 6f70 7469 6f6e 732e 7061 636b 6167  .[options.packag
+000002e0: 6573 2e66 696e 645d 0d0a 7768 6572 6520  es.find]..where 
+000002f0: 3d20 6675 6e64 6961 6c6f 6775 6573 0d0a  = fundialogues..
+00000300: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
+00000310: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
+00000320: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
```

