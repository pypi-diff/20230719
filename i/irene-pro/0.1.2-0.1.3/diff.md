# Comparing `tmp/irene_pro-0.1.2.tar.gz` & `tmp/irene_pro-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irene_pro-0.1.2.tar", last modified: Wed Jul 19 06:37:44 2023, max compression
+gzip compressed data, was "irene_pro-0.1.3.tar", last modified: Wed Jul 19 06:42:10 2023, max compression
```

## Comparing `irene_pro-0.1.2.tar` & `irene_pro-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 06:37:44.701433 irene_pro-0.1.2/
--rw-rw-rw-   0        0        0      227 2023-06-30 07:10:26.000000 irene_pro-0.1.2/LICENSE
--rw-rw-rw-   0        0        0       14 2023-06-30 07:10:26.000000 irene_pro-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1279 2023-07-19 06:37:44.698441 irene_pro-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      715 2023-06-30 07:10:26.000000 irene_pro-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-19 06:37:44.655560 irene_pro-0.1.2/irene_pro/
--rw-rw-rw-   0        0        0        0 2023-06-30 07:27:47.000000 irene_pro-0.1.2/irene_pro/__init__.py
--rw-rw-rw-   0        0        0     8186 2023-07-18 07:06:36.000000 irene_pro-0.1.2/irene_pro/logics.py
--rw-rw-rw-   0        0        0    38373 2023-07-19 06:36:00.000000 irene_pro-0.1.2/irene_pro/widgets.py
-drwxrwxrwx   0        0        0        0 2023-07-19 06:37:44.689551 irene_pro-0.1.2/irene_pro.egg-info/
--rw-rw-rw-   0        0        0     1279 2023-07-19 06:37:44.000000 irene_pro-0.1.2/irene_pro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-07-19 06:37:44.000000 irene_pro-0.1.2/irene_pro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-19 06:37:44.000000 irene_pro-0.1.2/irene_pro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-07-19 06:37:44.000000 irene_pro-0.1.2/irene_pro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-19 06:37:44.000000 irene_pro-0.1.2/irene_pro.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-19 06:37:44.703527 irene_pro-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1206 2023-07-19 06:36:54.000000 irene_pro-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 06:42:10.038712 irene_pro-0.1.3/
+-rw-rw-rw-   0        0        0      227 2023-06-30 07:10:26.000000 irene_pro-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0       14 2023-06-30 07:10:26.000000 irene_pro-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1279 2023-07-19 06:42:10.035720 irene_pro-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      715 2023-06-30 07:10:26.000000 irene_pro-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-19 06:42:09.970893 irene_pro-0.1.3/irene_pro/
+-rw-rw-rw-   0        0        0        0 2023-06-30 07:27:47.000000 irene_pro-0.1.3/irene_pro/__init__.py
+-rw-rw-rw-   0        0        0     8186 2023-07-18 07:06:36.000000 irene_pro-0.1.3/irene_pro/logics.py
+-rw-rw-rw-   0        0        0    38373 2023-07-19 06:36:00.000000 irene_pro-0.1.3/irene_pro/widgets.py
+drwxrwxrwx   0        0        0        0 2023-07-19 06:42:10.030734 irene_pro-0.1.3/irene_pro.egg-info/
+-rw-rw-rw-   0        0        0     1279 2023-07-19 06:42:09.000000 irene_pro-0.1.3/irene_pro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-07-19 06:42:09.000000 irene_pro-0.1.3/irene_pro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 06:42:09.000000 irene_pro-0.1.3/irene_pro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2023-07-19 06:42:09.000000 irene_pro-0.1.3/irene_pro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-19 06:42:09.000000 irene_pro-0.1.3/irene_pro.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-19 06:42:10.038712 irene_pro-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1219 2023-07-19 06:41:32.000000 irene_pro-0.1.3/setup.py
```

### Comparing `irene_pro-0.1.2/PKG-INFO` & `irene_pro-0.1.3/irene_pro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: irene_pro
-Version: 0.1.2
+Name: irene-pro
+Version: 0.1.3
 Summary: Use customized GUI
 Author: Irene coldsober
 Author-email: <irene.study.2023@gmail.com>
 Keywords: tkinter,widget,gui
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `irene_pro-0.1.2/README.md` & `irene_pro-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `irene_pro-0.1.2/irene_pro/logics.py` & `irene_pro-0.1.3/irene_pro/logics.py`

 * *Files identical despite different names*

### Comparing `irene_pro-0.1.2/irene_pro/widgets.py` & `irene_pro-0.1.3/irene_pro/widgets.py`

 * *Files identical despite different names*

### Comparing `irene_pro-0.1.2/irene_pro.egg-info/PKG-INFO` & `irene_pro-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: irene-pro
-Version: 0.1.2
+Name: irene_pro
+Version: 0.1.3
 Summary: Use customized GUI
 Author: Irene coldsober
 Author-email: <irene.study.2023@gmail.com>
 Keywords: tkinter,widget,gui
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `irene_pro-0.1.2/setup.py` & `irene_pro-0.1.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 00000090: 286f 732e 7061 7468 2e6a 6f69 6e28 6865  (os.path.join(he
 000000a0: 7265 2c20 2252 4541 444d 452e 6d64 2229  re, "README.md")
 000000b0: 2c20 656e 636f 6469 6e67 3d22 7574 662d  , encoding="utf-
 000000c0: 3822 2920 6173 2066 683a 0d0a 2020 2020  8") as fh:..    
 000000d0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 000000e0: 203d 2022 5c6e 2220 2b20 6668 2e72 6561   = "\n" + fh.rea
 000000f0: 6428 290d 0a0d 0a56 4552 5349 4f4e 203d  d()....VERSION =
-00000100: 2027 302e 3031 2e32 270d 0a44 4553 4352   '0.01.2'..DESCR
+00000100: 2027 302e 3031 2e33 270d 0a44 4553 4352   '0.01.3'..DESCR
 00000110: 4950 5449 4f4e 203d 2027 5573 6520 6375  IPTION = 'Use cu
 00000120: 7374 6f6d 697a 6564 2047 5549 270d 0a4c  stomized GUI'..L
 00000130: 4f4e 475f 4445 5343 5249 5054 494f 4e20  ONG_DESCRIPTION 
 00000140: 3d20 2741 2070 6163 6b61 6765 2074 6861  = 'A package tha
 00000150: 7420 616c 6c6f 7773 2079 6f75 2074 6f20  t allows you to 
 00000160: 7573 6520 7374 796c 6573 2061 6e64 2077  use styles and w
 00000170: 6964 6765 7420 6f66 2073 7570 6572 206c  idget of super l
@@ -46,31 +46,32 @@
 000002d0: 7061 636b 6167 6573 3d66 696e 645f 7061  packages=find_pa
 000002e0: 636b 6167 6573 2829 2c0d 0a20 2020 2069  ckages(),..    i
 000002f0: 6e73 7461 6c6c 5f72 6571 7569 7265 733d  nstall_requires=
 00000300: 5b22 7079 7769 6e33 3222 2c20 226f 7065  ["pywin32", "ope
 00000310: 6e63 762d 7079 7468 6f6e 222c 2022 7079  ncv-python", "py
 00000320: 7065 7263 6c69 7022 2c20 2274 6b63 616c  perclip", "tkcal
 00000330: 656e 6461 7222 2c20 2274 746b 7468 656d  endar", "ttkthem
-00000340: 6573 222c 2022 6e75 6d70 7922 5d2c 0d0a  es", "numpy"],..
-00000350: 2020 2020 6b65 7977 6f72 6473 3d5b 2774      keywords=['t
-00000360: 6b69 6e74 6572 272c 2027 7769 6467 6574  kinter', 'widget
-00000370: 272c 2027 6775 6927 5d2c 0d0a 2020 2020  ', 'gui'],..    
-00000380: 636c 6173 7369 6669 6572 733d 5b0d 0a20  classifiers=[.. 
-00000390: 2020 2020 2020 2022 4465 7665 6c6f 706d         "Developm
-000003a0: 656e 7420 5374 6174 7573 203a 3a20 3520  ent Status :: 5 
-000003b0: 2d20 5072 6f64 7563 7469 6f6e 2f53 7461  - Production/Sta
-000003c0: 626c 6522 2c0d 0a20 2020 2020 2020 2022  ble",..        "
-000003d0: 496e 7465 6e64 6564 2041 7564 6965 6e63  Intended Audienc
-000003e0: 6520 3a3a 2044 6576 656c 6f70 6572 7322  e :: Developers"
-000003f0: 2c0d 0a20 2020 2020 2020 2022 5072 6f67  ,..        "Prog
-00000400: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000410: 203a 3a20 5079 7468 6f6e 203a 3a20 3322   :: Python :: 3"
-00000420: 2c0d 0a20 2020 2020 2020 2022 4f70 6572  ,..        "Oper
-00000430: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
-00000440: 556e 6978 222c 0d0a 2020 2020 2020 2020  Unix",..        
-00000450: 224f 7065 7261 7469 6e67 2053 7973 7465  "Operating Syste
-00000460: 6d20 3a3a 204d 6163 4f53 203a 3a20 4d61  m :: MacOS :: Ma
-00000470: 634f 5320 5822 2c0d 0a20 2020 2020 2020  cOS X",..       
-00000480: 2022 4f70 6572 6174 696e 6720 5379 7374   "Operating Syst
-00000490: 656d 203a 3a20 4d69 6372 6f73 6f66 7420  em :: Microsoft 
-000004a0: 3a3a 2057 696e 646f 7773 222c 0d0a 2020  :: Windows",..  
-000004b0: 2020 5d0d 0a29                             ]..)
+00000340: 6573 222c 2022 6e75 6d70 7922 2c27 7363  es", "numpy",'sc
+00000350: 7265 656e 696e 666f 275d 2c0d 0a20 2020  reeninfo'],..   
+00000360: 206b 6579 776f 7264 733d 5b27 746b 696e   keywords=['tkin
+00000370: 7465 7227 2c20 2777 6964 6765 7427 2c20  ter', 'widget', 
+00000380: 2767 7569 275d 2c0d 0a20 2020 2063 6c61  'gui'],..    cla
+00000390: 7373 6966 6965 7273 3d5b 0d0a 2020 2020  ssifiers=[..    
+000003a0: 2020 2020 2244 6576 656c 6f70 6d65 6e74      "Development
+000003b0: 2053 7461 7475 7320 3a3a 2035 202d 2050   Status :: 5 - P
+000003c0: 726f 6475 6374 696f 6e2f 5374 6162 6c65  roduction/Stable
+000003d0: 222c 0d0a 2020 2020 2020 2020 2249 6e74  ",..        "Int
+000003e0: 656e 6465 6420 4175 6469 656e 6365 203a  ended Audience :
+000003f0: 3a20 4465 7665 6c6f 7065 7273 222c 0d0a  : Developers",..
+00000400: 2020 2020 2020 2020 2250 726f 6772 616d          "Program
+00000410: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000420: 2050 7974 686f 6e20 3a3a 2033 222c 0d0a   Python :: 3",..
+00000430: 2020 2020 2020 2020 224f 7065 7261 7469          "Operati
+00000440: 6e67 2053 7973 7465 6d20 3a3a 2055 6e69  ng System :: Uni
+00000450: 7822 2c0d 0a20 2020 2020 2020 2022 4f70  x",..        "Op
+00000460: 6572 6174 696e 6720 5379 7374 656d 203a  erating System :
+00000470: 3a20 4d61 634f 5320 3a3a 204d 6163 4f53  : MacOS :: MacOS
+00000480: 2058 222c 0d0a 2020 2020 2020 2020 224f   X",..        "O
+00000490: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
+000004a0: 3a3a 204d 6963 726f 736f 6674 203a 3a20  :: Microsoft :: 
+000004b0: 5769 6e64 6f77 7322 2c0d 0a20 2020 205d  Windows",..    ]
+000004c0: 0d0a 29                                  ..)
```

