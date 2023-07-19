# Comparing `tmp/orca_parser-0.1.2-py2.py3-none-any.whl.zip` & `tmp/orca_parser-0.1.3-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 6588 bytes, number of entries: 8
+Zip file size: 6589 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat     3325 b- defN 23-Jul-06 09:45 orca_parser/HessianTools.py
--rw-rw-rw-  2.0 fat    10132 b- defN 23-Jul-19 00:14 orca_parser/ORCAParse.py
+-rw-rw-rw-  2.0 fat    10132 b- defN 23-Jul-19 09:53 orca_parser/ORCAParse.py
 -rw-rw-rw-  2.0 fat      287 b- defN 23-Jul-06 09:50 orca_parser/__init__.py
--rw-rw-rw-  2.0 fat     1235 b- defN 23-Jul-19 00:15 orca_parser-0.1.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      482 b- defN 23-Jul-19 00:15 orca_parser-0.1.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Jul-19 00:15 orca_parser-0.1.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 23-Jul-19 00:15 orca_parser-0.1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      651 b- defN 23-Jul-19 00:15 orca_parser-0.1.2.dist-info/RECORD
-8 files, 16234 bytes uncompressed, 5452 bytes compressed:  66.4%
+-rw-rw-rw-  2.0 fat     1235 b- defN 23-Jul-19 09:55 orca_parser-0.1.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      482 b- defN 23-Jul-19 09:55 orca_parser-0.1.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Jul-19 09:55 orca_parser-0.1.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-Jul-19 09:55 orca_parser-0.1.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      651 b- defN 23-Jul-19 09:55 orca_parser-0.1.3.dist-info/RECORD
+8 files, 16234 bytes uncompressed, 5453 bytes compressed:  66.4%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: orca_parser/ORCAParse.py
 Comment: 
 
 Filename: orca_parser/__init__.py
 Comment: 
 
-Filename: orca_parser-0.1.2.dist-info/LICENSE
+Filename: orca_parser-0.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: orca_parser-0.1.2.dist-info/METADATA
+Filename: orca_parser-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: orca_parser-0.1.2.dist-info/WHEEL
+Filename: orca_parser-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: orca_parser-0.1.2.dist-info/top_level.txt
+Filename: orca_parser-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: orca_parser-0.1.2.dist-info/RECORD
+Filename: orca_parser-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## orca_parser/ORCAParse.py

 * *Ordering differences only*

```diff
@@ -84,17 +84,17 @@
     def parse_energies(self):
         self.energies = np.ndarray((0,), np.float64)
         self.energy_warnings = np.ndarray((0,), np.bool_)
         for part in self.raw.split("FINAL SINGLE POINT ENERGY")[1:]:
             part = part.split("\n")[0].strip()
             if "(Wavefunction not fully converged!)" in part:
                 part = part.split()[0]
-                self.energy_warnings = np.hstack((self.energy_warnings, [False]))
-            else:
                 self.energy_warnings = np.hstack((self.energy_warnings, [True]))
+            else:
+                self.energy_warnings = np.hstack((self.energy_warnings, [False]))
             part = float(part)
             self.energies = np.hstack((self.energies, [part]))
         #self.r_energies = self.energies - self.energies.min()
     def parse_dispersion(self):
         splits = self.raw.split("\nDispersion correction")[1:]
         self.dispersions = np.ndarray((len(splits),))
         for i in range(len(splits)):
```

## Comparing `orca_parser-0.1.2.dist-info/LICENSE` & `orca_parser-0.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `orca_parser-0.1.2.dist-info/RECORD` & `orca_parser-0.1.3.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 orca_parser/HessianTools.py,sha256=y936_LzZ3DGpnlElVQY96RtLPaKtRbEG5zPE4T-7VYY,3325
-orca_parser/ORCAParse.py,sha256=QQ8rPNTc_Ol3EoaLNGvZ2kz1BijFR-8AFAsuwWJRnmk,10132
+orca_parser/ORCAParse.py,sha256=Lyg4bi3u3C72iRctP2XaK92dtXfWUK3M_TYVZwgdMZ0,10132
 orca_parser/__init__.py,sha256=MlYoARmgG3uEVqcMY6rIRRYLHm0-4rh6WiSVGx-ngK4,287
-orca_parser-0.1.2.dist-info/LICENSE,sha256=Q2ptU2E48gOsMzhYz_kqVovmJ5d1KzrblLyqD2_-fvY,1235
-orca_parser-0.1.2.dist-info/METADATA,sha256=JIDfg72-E92VTkyHZqFk1E-feEmOoq0ODkmP6bE5Gf8,482
-orca_parser-0.1.2.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-orca_parser-0.1.2.dist-info/top_level.txt,sha256=8n8h8nQznt6NRgMjI0VijQ6cY5Nu7A0UUuc1M-GHe40,12
-orca_parser-0.1.2.dist-info/RECORD,,
+orca_parser-0.1.3.dist-info/LICENSE,sha256=Q2ptU2E48gOsMzhYz_kqVovmJ5d1KzrblLyqD2_-fvY,1235
+orca_parser-0.1.3.dist-info/METADATA,sha256=VWRPjvcRRm-YAM_ZAFmeJmu9iPtGmpIKq1L4s33slt4,482
+orca_parser-0.1.3.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+orca_parser-0.1.3.dist-info/top_level.txt,sha256=8n8h8nQznt6NRgMjI0VijQ6cY5Nu7A0UUuc1M-GHe40,12
+orca_parser-0.1.3.dist-info/RECORD,,
```

