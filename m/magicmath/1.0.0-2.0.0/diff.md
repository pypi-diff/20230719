# Comparing `tmp/magicmath-1.0.0.tar.gz` & `tmp/magicmath-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magicmath-1.0.0.tar", last modified: Tue Jul 18 22:18:50 2023, max compression
+gzip compressed data, was "magicmath-2.0.0.tar", last modified: Wed Jul 19 02:39:10 2023, max compression
```

## Comparing `magicmath-1.0.0.tar` & `magicmath-2.0.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 22:18:50.446187 magicmath-1.0.0/
--rw-rw-rw-   0        0        0      736 2023-07-18 22:18:50.444192 magicmath-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-18 22:18:50.402208 magicmath-1.0.0/magicmath/
--rw-rw-rw-   0        0        0       43 2023-07-18 22:18:24.000000 magicmath-1.0.0/magicmath/__init__.py
--rw-rw-rw-   0        0        0     2178 2023-07-18 21:59:23.000000 magicmath-1.0.0/magicmath/magicmath.py
-drwxrwxrwx   0        0        0        0 2023-07-18 22:18:50.441871 magicmath-1.0.0/magicmath.egg-info/
--rw-rw-rw-   0        0        0      736 2023-07-18 22:18:50.000000 magicmath-1.0.0/magicmath.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      185 2023-07-18 22:18:50.000000 magicmath-1.0.0/magicmath.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 22:18:50.000000 magicmath-1.0.0/magicmath.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-18 22:18:50.000000 magicmath-1.0.0/magicmath.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-18 22:18:50.446187 magicmath-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      854 2023-07-18 22:12:37.000000 magicmath-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 02:39:10.868478 magicmath-2.0.0/
+-rw-rw-rw-   0        0        0      812 2023-07-19 02:39:10.867517 magicmath-2.0.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-19 02:39:10.843476 magicmath-2.0.0/magicmath/
+-rw-rw-rw-   0        0        0       43 2023-07-18 22:18:24.000000 magicmath-2.0.0/magicmath/__init__.py
+-rw-rw-rw-   0        0        0     2181 2023-07-19 02:33:43.000000 magicmath-2.0.0/magicmath/magicmath.py
+drwxrwxrwx   0        0        0        0 2023-07-19 02:39:10.865558 magicmath-2.0.0/magicmath.egg-info/
+-rw-rw-rw-   0        0        0      812 2023-07-19 02:39:10.000000 magicmath-2.0.0/magicmath.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      185 2023-07-19 02:39:10.000000 magicmath-2.0.0/magicmath.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 02:39:10.000000 magicmath-2.0.0/magicmath.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-19 02:39:10.000000 magicmath-2.0.0/magicmath.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-19 02:39:10.869476 magicmath-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      930 2023-07-19 02:36:37.000000 magicmath-2.0.0/setup.py
```

### Comparing `magicmath-1.0.0/PKG-INFO` & `magicmath-2.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: magicmath
-Version: 1.0.0
-Summary: A simple package to do basic math with lists
-Home-page: https://github.com/marcosrosa/magicmath
+Version: 2.0.0
+Summary: The power of compiling lists with sequential mathematical operations. Useful for lists with long sets of numbers.
+Home-page: https://github.com/marcosleandrorosa/magicmath
 Author: Marcos Leandro Rosa
 Author-email: marcosfac@gmail.com
 License: MIT
 Keywords: math,list,magicmath,math with lists,invert lists
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `magicmath-1.0.0/magicmath/magicmath.py` & `magicmath-2.0.0/magicmath/magicmath.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,27 +9,27 @@
     The methods will return the result
     You can also call the numberlist attribute to see the numbers
     in the list
     You can also call the invert attribute to see if the numbers
     are reversed or not
     Example:
         listA = [21, 22, 23, 24, 25, 26, 27, 28, 29]
-        mynewnumber = Magicmath(listA, invert=True)
+        mynewnumber = Magicmath(listA, invert=True, showerrors=True)
         print(mynewnumber.add())
         print(mynewnumber.sub())
         print(mynewnumber.mul())
-        print(mynewnumber.div(showerror=True))
         print(mynewnumber.getgreater())
         print(mynewnumber.numberlist)
         print(mynewnumber.invert)
-        print(mynewnumber.div(showerror=True))
+        print(mynewnumber.div())
         print(mynewnumber.getgreater())
     """
-    def __init__(self, numberlist:list, invert:bool=False):
+    def __init__(self, numberlist:list, invert:bool=False, showerrors:bool=False):
         self.numberlist = numberlist
+        self.showerrors = showerrors
         self.invert = invert
         if invert == True:
             self.numberlist.reverse()
 
     def add(self):
         return sum(self.numberlist)
 
@@ -43,27 +43,26 @@
 
     def mul(self):
         result = 1
         for n in self.numberlist:
             result *= n
         return result
 
-    def div(self, showerror=False):
+    def div(self):
         for n in self.numberlist:
                 if n != 0:
                     if n == self.numberlist[0]:
                         result = n
                     else:
                         result /= n
                 else:
-                    if showerror:
+                    if self.showerrors:
                         raise TypeError("Your list contains 0 and cannot be divided")
                     else:
                         result = 0
         return result
 
     def getgreater(self):
         return max(self.numberlist)
 
     def getminor(self):
         return min(self.numberlist)
-
```

### Comparing `magicmath-1.0.0/magicmath.egg-info/PKG-INFO` & `magicmath-2.0.0/magicmath.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: magicmath
-Version: 1.0.0
-Summary: A simple package to do basic math with lists
-Home-page: https://github.com/marcosrosa/magicmath
+Version: 2.0.0
+Summary: The power of compiling lists with sequential mathematical operations. Useful for lists with long sets of numbers.
+Home-page: https://github.com/marcosleandrorosa/magicmath
 Author: Marcos Leandro Rosa
 Author-email: marcosfac@gmail.com
 License: MIT
 Keywords: math,list,magicmath,math with lists,invert lists
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `magicmath-1.0.0/setup.py` & `magicmath-2.0.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup
 setup(
     name='magicmath',
     packages=['magicmath'],
-    version='1.0.0',
+    version='2.0.0',
     license='MIT',
-    description='A simple package to do basic math with lists',
+    description='The power of compiling lists with sequential mathematical operations. Useful for lists with long sets of numbers.',
     author='Marcos Leandro Rosa',
     author_email='marcosfac@gmail.com',
-    url='https://github.com/marcosrosa/magicmath',
+    url='https://github.com/marcosleandrorosa/magicmath',
     keywords=['math', 'list', 'magicmath', 'math with lists', 'invert lists'],
     install_requires=[],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',
```

