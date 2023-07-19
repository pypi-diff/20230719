# Comparing `tmp/orca_parser-0.1.1-py2.py3-none-any.whl.zip` & `tmp/orca_parser-0.1.2-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 6515 bytes, number of entries: 8
+Zip file size: 6588 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat     3325 b- defN 23-Jul-06 09:45 orca_parser/HessianTools.py
--rw-rw-rw-  2.0 fat     9761 b- defN 23-Jul-06 09:45 orca_parser/ORCAParse.py
+-rw-rw-rw-  2.0 fat    10132 b- defN 23-Jul-19 00:14 orca_parser/ORCAParse.py
 -rw-rw-rw-  2.0 fat      287 b- defN 23-Jul-06 09:50 orca_parser/__init__.py
--rw-rw-rw-  2.0 fat     1235 b- defN 23-Jul-06 10:26 orca_parser-0.1.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      482 b- defN 23-Jul-06 10:26 orca_parser-0.1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Jul-06 10:26 orca_parser-0.1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 23-Jul-06 10:26 orca_parser-0.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      650 b- defN 23-Jul-06 10:26 orca_parser-0.1.1.dist-info/RECORD
-8 files, 15862 bytes uncompressed, 5379 bytes compressed:  66.1%
+-rw-rw-rw-  2.0 fat     1235 b- defN 23-Jul-19 00:15 orca_parser-0.1.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      482 b- defN 23-Jul-19 00:15 orca_parser-0.1.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Jul-19 00:15 orca_parser-0.1.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-Jul-19 00:15 orca_parser-0.1.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      651 b- defN 23-Jul-19 00:15 orca_parser-0.1.2.dist-info/RECORD
+8 files, 16234 bytes uncompressed, 5452 bytes compressed:  66.4%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: orca_parser/ORCAParse.py
 Comment: 
 
 Filename: orca_parser/__init__.py
 Comment: 
 
-Filename: orca_parser-0.1.1.dist-info/LICENSE
+Filename: orca_parser-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: orca_parser-0.1.1.dist-info/METADATA
+Filename: orca_parser-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: orca_parser-0.1.1.dist-info/WHEEL
+Filename: orca_parser-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: orca_parser-0.1.1.dist-info/top_level.txt
+Filename: orca_parser-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: orca_parser-0.1.1.dist-info/RECORD
+Filename: orca_parser-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## orca_parser/ORCAParse.py

```diff
@@ -79,16 +79,23 @@
             
     def thermodynamics(self):
         #Search for the INNER ENERGY section
         pass
     
     def parse_energies(self):
         self.energies = np.ndarray((0,), np.float64)
+        self.energy_warnings = np.ndarray((0,), np.bool_)
         for part in self.raw.split("FINAL SINGLE POINT ENERGY")[1:]:
-            part = float(part.split("\n")[0].strip())
+            part = part.split("\n")[0].strip()
+            if "(Wavefunction not fully converged!)" in part:
+                part = part.split()[0]
+                self.energy_warnings = np.hstack((self.energy_warnings, [False]))
+            else:
+                self.energy_warnings = np.hstack((self.energy_warnings, [True]))
+            part = float(part)
             self.energies = np.hstack((self.energies, [part]))
         #self.r_energies = self.energies - self.energies.min()
     def parse_dispersion(self):
         splits = self.raw.split("\nDispersion correction")[1:]
         self.dispersions = np.ndarray((len(splits),))
         for i in range(len(splits)):
             E_disp = splits[i].split("\n")[0].strip()
```

## Comparing `orca_parser-0.1.1.dist-info/LICENSE` & `orca_parser-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

