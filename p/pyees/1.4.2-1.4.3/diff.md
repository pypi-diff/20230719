# Comparing `tmp/pyees-1.4.2.tar.gz` & `tmp/pyees-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyees-1.4.2.tar", last modified: Tue Jul 18 11:18:32 2023, max compression
+gzip compressed data, was "pyees-1.4.3.tar", last modified: Tue Jul 18 12:28:45 2023, max compression
```

## Comparing `pyees-1.4.2.tar` & `pyees-1.4.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 11:18:32.047046 pyees-1.4.2/
--rw-rw-rw-   0        0        0     1085 2022-02-05 11:46:00.000000 pyees-1.4.2/LICENSE.txt
--rw-rw-rw-   0        0        0      768 2023-07-18 11:18:32.062670 pyees-1.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     1017 2023-03-10 10:19:19.000000 pyees-1.4.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-18 11:18:31.812663 pyees-1.4.2/pyees/
--rw-rw-rw-   0        0        0      320 2023-05-12 12:42:57.000000 pyees-1.4.2/pyees/__init__.py
--rw-rw-rw-   0        0        0    18504 2023-07-16 06:55:05.000000 pyees-1.4.2/pyees/fit.py
--rw-rw-rw-   0        0        0      662 2023-07-14 10:33:23.000000 pyees-1.4.2/pyees/profileFit.py
--rw-rw-rw-   0        0        0      812 2023-07-14 08:09:04.000000 pyees-1.4.2/pyees/profilePyees.py
--rw-rw-rw-   0        0        0    10022 2023-07-13 16:40:17.000000 pyees-1.4.2/pyees/prop.py
--rw-rw-rw-   0        0        0    18385 2023-06-29 06:34:38.000000 pyees-1.4.2/pyees/sheet.py
--rw-rw-rw-   0        0        0    10183 2023-07-13 16:48:56.000000 pyees-1.4.2/pyees/solve.py
--rw-rw-rw-   0        0        0     1406 2022-03-24 20:23:42.000000 pyees-1.4.2/pyees/stackOverflowODR.py
--rw-rw-rw-   0        0        0     7387 2023-07-17 06:54:59.000000 pyees-1.4.2/pyees/testFit.py
--rw-rw-rw-   0        0        0    13373 2023-07-13 16:26:12.000000 pyees-1.4.2/pyees/testProp.py
--rw-rw-rw-   0        0        0     1044 2023-07-17 07:24:43.000000 pyees-1.4.2/pyees/testPyees.py
--rw-rw-rw-   0        0        0    17783 2023-06-29 06:36:21.000000 pyees-1.4.2/pyees/testSheet.py
--rw-rw-rw-   0        0        0    20204 2023-07-13 16:49:32.000000 pyees-1.4.2/pyees/testSolve.py
--rw-rw-rw-   0        0        0    10782 2023-07-13 16:54:24.000000 pyees-1.4.2/pyees/testUnit.py
--rw-rw-rw-   0        0        0    84460 2023-07-18 11:17:21.000000 pyees-1.4.2/pyees/testVariable.py
--rw-rw-rw-   0        0        0    35486 2023-07-14 08:06:32.000000 pyees-1.4.2/pyees/unit.py
--rw-rw-rw-   0        0        0    36013 2023-07-18 11:17:32.000000 pyees-1.4.2/pyees/variable.py
-drwxrwxrwx   0        0        0        0 2023-07-18 11:18:32.015794 pyees-1.4.2/pyees.egg-info/
--rw-rw-rw-   0        0        0      768 2023-07-18 11:18:29.000000 pyees-1.4.2/pyees.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      491 2023-07-18 11:18:30.000000 pyees-1.4.2/pyees.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 11:18:30.000000 pyees-1.4.2/pyees.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-07-18 11:18:30.000000 pyees-1.4.2/pyees.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-18 11:18:30.000000 pyees-1.4.2/pyees.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-18 11:18:32.109547 pyees-1.4.2/setup.cfg
--rw-rw-rw-   0        0        0     1224 2023-07-18 11:18:23.000000 pyees-1.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 12:28:45.845096 pyees-1.4.3/
+-rw-rw-rw-   0        0        0     1085 2022-02-05 11:46:00.000000 pyees-1.4.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      768 2023-07-18 12:28:45.860722 pyees-1.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1017 2023-03-10 10:19:19.000000 pyees-1.4.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 12:28:45.610715 pyees-1.4.3/pyees/
+-rw-rw-rw-   0        0        0      320 2023-05-12 12:42:57.000000 pyees-1.4.3/pyees/__init__.py
+-rw-rw-rw-   0        0        0    18504 2023-07-16 06:55:05.000000 pyees-1.4.3/pyees/fit.py
+-rw-rw-rw-   0        0        0      662 2023-07-14 10:33:23.000000 pyees-1.4.3/pyees/profileFit.py
+-rw-rw-rw-   0        0        0      812 2023-07-18 11:26:45.000000 pyees-1.4.3/pyees/profilePyees.py
+-rw-rw-rw-   0        0        0    10022 2023-07-13 16:40:17.000000 pyees-1.4.3/pyees/prop.py
+-rw-rw-rw-   0        0        0    18385 2023-06-29 06:34:38.000000 pyees-1.4.3/pyees/sheet.py
+-rw-rw-rw-   0        0        0    10183 2023-07-13 16:48:56.000000 pyees-1.4.3/pyees/solve.py
+-rw-rw-rw-   0        0        0     1406 2022-03-24 20:23:42.000000 pyees-1.4.3/pyees/stackOverflowODR.py
+-rw-rw-rw-   0        0        0     7387 2023-07-17 06:54:59.000000 pyees-1.4.3/pyees/testFit.py
+-rw-rw-rw-   0        0        0    13373 2023-07-13 16:26:12.000000 pyees-1.4.3/pyees/testProp.py
+-rw-rw-rw-   0        0        0     1044 2023-07-17 07:24:43.000000 pyees-1.4.3/pyees/testPyees.py
+-rw-rw-rw-   0        0        0    17783 2023-06-29 06:36:21.000000 pyees-1.4.3/pyees/testSheet.py
+-rw-rw-rw-   0        0        0    20204 2023-07-13 16:49:32.000000 pyees-1.4.3/pyees/testSolve.py
+-rw-rw-rw-   0        0        0    10780 2023-07-18 12:12:39.000000 pyees-1.4.3/pyees/testUnit.py
+-rw-rw-rw-   0        0        0    84460 2023-07-18 11:17:21.000000 pyees-1.4.3/pyees/testVariable.py
+-rw-rw-rw-   0        0        0    36658 2023-07-18 12:28:16.000000 pyees-1.4.3/pyees/unit.py
+-rw-rw-rw-   0        0        0    35511 2023-07-18 12:28:23.000000 pyees-1.4.3/pyees/variable.py
+drwxrwxrwx   0        0        0        0 2023-07-18 12:28:45.798221 pyees-1.4.3/pyees.egg-info/
+-rw-rw-rw-   0        0        0      768 2023-07-18 12:28:43.000000 pyees-1.4.3/pyees.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      491 2023-07-18 12:28:44.000000 pyees-1.4.3/pyees.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 12:28:43.000000 pyees-1.4.3/pyees.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-07-18 12:28:43.000000 pyees-1.4.3/pyees.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-18 12:28:44.000000 pyees-1.4.3/pyees.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-18 12:28:45.891975 pyees-1.4.3/setup.cfg
+-rw-rw-rw-   0        0        0     1224 2023-07-18 12:28:32.000000 pyees-1.4.3/setup.py
```

### Comparing `pyees-1.4.2/LICENSE.txt` & `pyees-1.4.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyees-1.4.2/PKG-INFO` & `pyees-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyees
-Version: 1.4.2
+Version: 1.4.3
 Summary: EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.
 Home-page: https://github.com/jacobv95/pyees
 Download-URL: https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz
 Author: Jacob Vestergaard
 Author-email: jacobvestergaard95@gmail.com
 License: MIT
 Keywords: python,data processing,uncertanty,EES
```

### Comparing `pyees-1.4.2/README.md` & `pyees-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `pyees-1.4.2/pyees/fit.py` & `pyees-1.4.3/pyees/fit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.2/pyees/profileFit.py` & `pyees-1.4.3/pyees/profileFit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.2/pyees/profilePyees.py` & `pyees-1.4.3/pyees/profilePyees.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.2/pyees/prop.py` & `pyees-1.4.3/pyees/prop.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.2/pyees/sheet.py` & `pyees-1.4.3/pyees/sheet.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.2/pyees/solve.py` & `pyees-1.4.3/pyees/solve.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.2/pyees/stackOverflowODR.py` & `pyees-1.4.3/pyees/stackOverflowODR.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.2/pyees/testFit.py` & `pyees-1.4.3/pyees/testFit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.2/pyees/testProp.py` & `pyees-1.4.3/pyees/testProp.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.2/pyees/testPyees.py` & `pyees-1.4.3/pyees/testPyees.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.2/pyees/testSheet.py` & `pyees-1.4.3/pyees/testSheet.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.2/pyees/testSolve.py` & `pyees-1.4.3/pyees/testSolve.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.2/pyees/testUnit.py` & `pyees-1.4.3/pyees/testUnit.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,15 +191,14 @@
         converter = a.getConverter('F')
         self.assertAlmostEqual(converter.convert(300, useOffset=True), 80.33)
 
         a = unit('mm2')
         converter = a.getConverter('m2')
         self.assertAlmostEqual(converter.convert(1), 1/1000 * 1/1000)
 
-
         a = unit('A')
         b = unit('V')
         c = a * b
         converter = c.getConverter('W')
         
         a = unit('A')
         b = unit('ohm')
```

### Comparing `pyees-1.4.2/pyees/testVariable.py` & `pyees-1.4.3/pyees/testVariable.py`

 * *Files identical despite different names*

### Comparing `pyees-1.4.2/pyees/unit.py` & `pyees-1.4.3/pyees/unit.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from copy import copy
 
 class _unitConversion():
 
     def __init__(self, scale, offset=0) -> None:
         self.scale = scale
         self.offset = offset
-
+    
     def __mul__(self, other):
         if isinstance(other, _unitConversion):
             scale = self.scale * other.scale
             offset = self.scale * other.offset + self.offset
         else:
             scale = self.scale * other
             offset = self.offset
@@ -28,14 +28,34 @@
             
         return _unitConversion(scale, offset)
 
     def __truediv__(self, other):
         if isinstance(other, _unitConversion):
             return _unitConversion(1 / other.scale, - other.offset / other.scale) * self
         return self * _unitConversion(1 / other)
+    
+    @staticmethod
+    def staticMul(selfScale, selfOffset, otherScale, otherOffset = 0):
+        scale = selfScale * otherScale
+        offset = selfScale * otherOffset + selfOffset
+        return scale, offset
+    
+    @staticmethod
+    def staticPow(selfScale, selfOffset, pow):
+        if pow==1: return selfScale, selfOffset
+        scale, offset = selfScale, selfOffset
+        for _ in range(pow - 1):
+            selfScale *= scale
+            selfOffset*= scale
+            selfOffset += offset
+        return selfScale, selfOffset
+
+    @staticmethod
+    def staticTruediv(selfScale, selfOffset, otherScale, otherOffset = 0):
+        return _unitConversion.staticMul(1 / otherScale, - otherOffset / otherScale, selfScale, selfOffset)
 
     def convert(self, value, useOffset=True):
         if useOffset:
             return self.scale * value + self.offset
         else:
             return self.scale * value
 
@@ -348,21 +368,15 @@
             self.unitDict = self._getUnitDict(self._formatUnitStr(unitStr))
         else:
             self.unitDict = unitDict
             
         self.unitStr = self._getUnitStrFromDict(self.unitDict)
         self.unitDictSI = self._getUnitDictSI(self.unitDict)
         self.unitStrSI = self._getUnitStrFromDict(self.unitDictSI)
-        
-        # ## create a version of the self.unitDictSI that is formatted in the same way as a unitDict
-        # unitDictSI = {}
-        # for key, exp in self.unitDictSI.items():
-        #     u = knownUnits[key][0]
-        #     u,p,e = unit._splitUnitExponentAndPrefix(u)
-        #     unitDictSI[u] = {p: e*exp}
+
         self._converterToSI = self.getConverterFromDict(self.unitDictSI)
 
 
     @staticmethod
     def _getUnitStrFromDict(unitDict):
         upper, lower = [], []
         for u, item in unitDict.items():    
@@ -966,46 +980,49 @@
         if not (self.unitDictSI == newUnitDictSI):
             raise ValueError(f'You tried to convert from {self} to {newUnitStr}. But these do not have the same base units')
         return self.getConverterFromDict(newUnitDict)
     
     def getConverterFromDict(self, newUnitDict):    
         
         # initialize the scale and offset
-        out = _unitConversion(1, 0)
+        outScale, outOffset = 1,0
         
         ## loop over self.unitDict
         for u, item in self.unitDict.items():
             for pre, exp in item.items():
                 conv = knownUnits[u][1]
-                if not pre is None: conv *= knownPrefixes[pre]
+                convScale, convOffset = conv.scale, conv.offset
+                if not pre is None: convScale, convOffset = _unitConversion.staticMul(convScale, convOffset, knownPrefixes[pre])
                 isUpper = exp > 0
-                if not isUpper: exp *= -1                    
-                conv = conv ** exp
-                out = out * conv if isUpper else out / conv
+                if not isUpper: exp *= -1    
+                convScale, convOffset = _unitConversion.staticPow(convScale, convOffset, exp)
+                if isUpper:
+                    outScale, outOffset = _unitConversion.staticMul(outScale, outOffset, convScale, convOffset)
+                else:
+                    outScale, outOffset = _unitConversion.staticTruediv(outScale, outOffset, convScale, convOffset)      
 
         ## loop over newUnitDict
         for u, item in newUnitDict.items():
             for pre, exp in item.items():
                 conv = knownUnits[u][1]
-                if not pre is None: conv *= knownPrefixes[pre]
+                convScale, convOffset = conv.scale, conv.offset
+                if not pre is None: convScale, convOffset = _unitConversion.staticMul(convScale, convOffset, knownPrefixes[pre])
                 isUpper = exp > 0
-                if not isUpper: exp *= -1
-                conv = conv ** exp
-                out = out * conv if not isUpper else out / conv
-        
-        return out
+                if not isUpper: exp *= -1    
+                convScale, convOffset = _unitConversion.staticPow(convScale, convOffset, exp)
+                if not isUpper:
+                    outScale, outOffset = _unitConversion.staticMul(outScale, outOffset, convScale, convOffset)
+                else:
+                    outScale, outOffset = _unitConversion.staticTruediv(outScale, outOffset, convScale, convOffset)      
+                
+        return _unitConversion(outScale, outOffset)
 
     def isCombinationUnit(self):
         return len(list(self.unitDict.keys())) > 1
 
     def getLogarithmicConverter(self, unitStr = None):
         if unitStr is None:
             unitStr = self.unitStr
         u, _ = self._removePrefixFromUnit(unitStr)
         return knownUnits[u][1]
 
-    
-if __name__ == "__main__":
-    a = unit('K')
-    converter = a.getConverter('C')
-    print(converter.convert(300), 26.85)
```

### Comparing `pyees-1.4.2/pyees/variable.py` & `pyees-1.4.3/pyees/variable.py`

 * *Files 2% similar despite different names*

```diff
@@ -990,30 +990,9 @@
                 raise ValueError('The lenght of the value has to be equal to the lenght of the uncertanty')      
     
     if isinstance(value, np.ndarray):
         return arrayVariable(value = value, unitStr = unit, uncert = uncert, nDigits = nDigits)
     else:
         return scalarVariable(value, unit, uncert, nDigits)
 
-if __name__ == "__main__":
-
-    t_in = variable(50, 'C', 1.2)
-    t_out = variable([10, 15, 20, 25, 30, 35, 40], 'C', [0.9, 1.1, 1.0, 0.8, 0.9, 1.3, 1.1])
-    
-    dt = t_in - t_out
-    print(dt)
-    for elem in dt:
-        print(elem)
-
-    
-    t_in = variable(50, 'C', 1.2)
-    dt = variable([10, 15, 20, 25, 30, 35, 40], 'DELTAC', [0.9, 1.1, 1.0, 0.8, 0.9, 1.3, 1.1])
-    
-    t_out = t_in + dt
-    print(t_out)
-    for elem in t_out:
-        print(elem)
-        
-        
-
```

### Comparing `pyees-1.4.2/pyees.egg-info/PKG-INFO` & `pyees-1.4.3/pyees.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyees
-Version: 1.4.2
+Version: 1.4.3
 Summary: EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.
 Home-page: https://github.com/jacobv95/pyees
 Download-URL: https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz
 Author: Jacob Vestergaard
 Author-email: jacobvestergaard95@gmail.com
 License: MIT
 Keywords: python,data processing,uncertanty,EES
```

### Comparing `pyees-1.4.2/setup.py` & `pyees-1.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
     name='pyees',
     packages=['pyees'],
-    version='1.4.2',
+    version='1.4.3',
     license='MIT',
     description='EES but for python. Pyees can be used do perform uncertanty (error) propagation. Furthermore, it can solve nonlinear systems of equations and look up material properties.',
     author='Jacob Vestergaard',
     author_email='jacobvestergaard95@gmail.com',
     url='https://github.com/jacobv95/pyees',
     download_url='https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz',
     keywords=['python', 'data processing', 'uncertanty', 'EES'],
```

