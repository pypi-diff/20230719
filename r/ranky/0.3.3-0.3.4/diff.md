# Comparing `tmp/ranky-0.3.3-py3-none-any.whl.zip` & `tmp/ranky-0.3.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 25413 bytes, number of entries: 13
--rw-r--r--  2.0 unx      272 b- defN 23-Mar-24 16:36 ranky/__init__.py
+Zip file size: 25573 bytes, number of entries: 13
+-rw-r--r--  2.0 unx      272 b- defN 23-Jul-19 12:12 ranky/__init__.py
 -rw-r--r--  2.0 unx     5368 b- defN 23-Jan-10 14:15 ranky/duel.py
 -rw-r--r--  2.0 unx     3498 b- defN 22-Nov-07 14:45 ranky/generator.py
 -rw-r--r--  2.0 unx    23788 b- defN 23-Mar-24 16:18 ranky/metric.py
 -rwxr-xr-x  2.0 unx     4390 b- defN 21-Apr-30 10:14 ranky/pairwise.py
 -rw-r--r--  2.0 unx    15445 b- defN 23-Jan-10 13:52 ranky/ranking.py
--rw-r--r--  2.0 unx      737 b- defN 22-Nov-07 14:45 ranky/utilities.py
+-rw-r--r--  2.0 unx     1174 b- defN 23-Jul-19 12:12 ranky/utilities.py
 -rw-r--r--  2.0 unx    13087 b- defN 23-Jan-24 12:42 ranky/visualization.py
--rw-r--r--  2.0 unx      288 b- defN 23-Mar-24 16:36 ranky-0.3.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     6009 b- defN 23-Mar-24 16:36 ranky-0.3.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-24 16:36 ranky-0.3.3.dist-info/WHEEL
--rwxr-xr-x  2.0 unx        6 b- defN 23-Mar-24 16:36 ranky-0.3.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      967 b- defN 23-Mar-24 16:36 ranky-0.3.3.dist-info/RECORD
-13 files, 73947 bytes uncompressed, 23833 bytes compressed:  67.8%
+-rw-r--r--  2.0 unx      288 b- defN 23-Jul-19 12:14 ranky-0.3.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6009 b- defN 23-Jul-19 12:14 ranky-0.3.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-19 12:14 ranky-0.3.4.dist-info/WHEEL
+-rwxr-xr-x  2.0 unx        6 b- defN 23-Jul-19 12:14 ranky-0.3.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      968 b- defN 23-Jul-19 12:14 ranky-0.3.4.dist-info/RECORD
+13 files, 74385 bytes uncompressed, 23993 bytes compressed:  67.7%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: ranky/utilities.py
 Comment: 
 
 Filename: ranky/visualization.py
 Comment: 
 
-Filename: ranky-0.3.3.dist-info/LICENSE
+Filename: ranky-0.3.4.dist-info/LICENSE
 Comment: 
 
-Filename: ranky-0.3.3.dist-info/METADATA
+Filename: ranky-0.3.4.dist-info/METADATA
 Comment: 
 
-Filename: ranky-0.3.3.dist-info/WHEEL
+Filename: ranky-0.3.4.dist-info/WHEEL
 Comment: 
 
-Filename: ranky-0.3.3.dist-info/top_level.txt
+Filename: ranky-0.3.4.dist-info/top_level.txt
 Comment: 
 
-Filename: ranky-0.3.3.dist-info/RECORD
+Filename: ranky-0.3.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ranky/__init__.py

```diff
@@ -8,8 +8,8 @@
 from .ranking import *
 from .metric import *
 from .duel import *
 from .visualization import *
 from .generator import *
 from .utilities import *
 
-__version__ = '0.3.3'
+__version__ = '0.3.4'
```

## ranky/utilities.py

```diff
@@ -18,11 +18,21 @@
 
 def read_codalab_csv(csv_file):
     """ Read a leaderboard generated by Codalab as a CSV file.
 
     Args:
         csv_file: The leaderboard downloaded from Codalab.
     """
-    m = pd.read_csv(csv_file, usecols=np.arange(0,5), index_col=1)
+    # Read the CSV file just to get the column names
+    df_temp = pd.read_csv(csv_file, nrows=0)  # Read no rows, but it does read the header row
+    col_names = df_temp.columns.tolist()
+    # Add a name for the extra column
+    col_names.append('extra')
+    # Read the CSV file again with the updated column names
+    m = pd.read_csv(csv_file, names=col_names, skiprows=1)
+    # Now you can drop the extra column
+    m = m.drop(columns=['extra'])
     m = m.drop('submission_pk', axis=1)
+    m.index = m['User']
+    m = m.drop('User', axis=1)
     m = m.applymap(str_to_float)
     return m
```

## Comparing `ranky-0.3.3.dist-info/METADATA` & `ranky-0.3.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ranky
-Version: 0.3.3
+Version: 0.3.4
 Summary: Compute rankings in Python.
 Home-page: https://github.com/didayolo/ranky
 Author: Adrien Pavao
 Author-email: adrien.pavao@gmail.com
 Project-URL: Bug Tracker, https://github.com/didayolo/ranky/issues
 Project-URL: Documentation, https://didayolo.github.io/ranky/
 Project-URL: Source Code, https://github.com/didayolo/ranky
```

## Comparing `ranky-0.3.3.dist-info/RECORD` & `ranky-0.3.4.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-ranky/__init__.py,sha256=FhzKgS0KgvtDlRX0t4YwO8gU0xIaq-vQhDQXyfe4uVw,272
+ranky/__init__.py,sha256=oxj8_gFXfxpkKHko3yReeVsfdDrRWMIPNmC7VTdIP7M,272
 ranky/duel.py,sha256=329VKRPg7VJKqP4EDkPtyitijzPZz5zhuBHNsVPsE7I,5368
 ranky/generator.py,sha256=hpw_lCcdQkVZ-3JzBHY8_00sPKnLgZKOoxwejEmfS_c,3498
 ranky/metric.py,sha256=sYRXiPhfhsPlHWC5vOyJlW-s_4BFXLHemc2RZpGCOgU,23788
 ranky/pairwise.py,sha256=7JLCogiiDaDFkfFI_yK_5_e7sLHXhDyfEciKWipsSbo,4390
 ranky/ranking.py,sha256=_CBU0VP-__5TPw1ppS6a0Vqwwy0qaWER07O5VYS7BUc,15445
-ranky/utilities.py,sha256=eA42UyKDShAv7OtMpzFiIJ1izT93e9MVlkLzjxQfjNw,737
+ranky/utilities.py,sha256=dOuyuDXDF2LZGvd1C_eChK1XdynLi5m1ca6CD0yIDp0,1174
 ranky/visualization.py,sha256=05hIn4NMtObN5mfTqPT4KGND0BQdHxElP8IrgmUrsRg,13087
-ranky-0.3.3.dist-info/LICENSE,sha256=7q1djQBYDky9IVSt7c2p0hmRjAULWLZ02lnlOOL7HQk,288
-ranky-0.3.3.dist-info/METADATA,sha256=pEAzez9fCc3dYueEZseRr0ytxZil3bha9bCopfPuvok,6009
-ranky-0.3.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-ranky-0.3.3.dist-info/top_level.txt,sha256=xigcWGcaY2Cz1FawzzbHZL9Rmuz0fvJYLSoqKY4ilP4,6
-ranky-0.3.3.dist-info/RECORD,,
+ranky-0.3.4.dist-info/LICENSE,sha256=7q1djQBYDky9IVSt7c2p0hmRjAULWLZ02lnlOOL7HQk,288
+ranky-0.3.4.dist-info/METADATA,sha256=0BQSm-Mu8PNtTVLgj6si_y2mPEfPyDcvOHS7Pu8ZDSQ,6009
+ranky-0.3.4.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+ranky-0.3.4.dist-info/top_level.txt,sha256=xigcWGcaY2Cz1FawzzbHZL9Rmuz0fvJYLSoqKY4ilP4,6
+ranky-0.3.4.dist-info/RECORD,,
```
