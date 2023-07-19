# Comparing `tmp/uncertainty-datatypes-1.0.5.tar.gz` & `tmp/uncertainty-datatypes-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uncertainty-datatypes-1.0.5.tar", last modified: Wed Jul 19 09:14:20 2023, max compression
+gzip compressed data, was "uncertainty-datatypes-1.0.6.tar", last modified: Wed Jul 19 09:36:54 2023, max compression
```

## Comparing `uncertainty-datatypes-1.0.5.tar` & `uncertainty-datatypes-1.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-19 09:14:20.622406 uncertainty-datatypes-1.0.5/
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     1099 2023-07-17 07:54:55.000000 uncertainty-datatypes-1.0.5/LICENSE
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    10214 2023-07-19 09:14:20.622248 uncertainty-datatypes-1.0.5/PKG-INFO
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     9443 2023-07-19 09:12:21.000000 uncertainty-datatypes-1.0.5/README.md
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)      854 2023-07-19 09:12:39.000000 uncertainty-datatypes-1.0.5/pyproject.toml
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)       38 2023-07-19 09:14:20.622441 uncertainty-datatypes-1.0.5/setup.cfg
-drwxr-xr-x   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-19 09:14:20.620681 uncertainty-datatypes-1.0.5/test/
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     4428 2023-07-18 10:58:49.000000 uncertainty-datatypes-1.0.5/test/test_ubool.py
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    19028 2023-07-19 08:55:34.000000 uncertainty-datatypes-1.0.5/test/test_ufloat.py
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    17972 2023-07-19 08:39:29.000000 uncertainty-datatypes-1.0.5/test/test_uint.py
-drwxr-xr-x   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-19 09:14:20.621519 uncertainty-datatypes-1.0.5/udatatypes/
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-14 08:59:58.000000 uncertainty-datatypes-1.0.5/udatatypes/__init__.py
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)      328 2023-07-17 11:29:42.000000 uncertainty-datatypes-1.0.5/udatatypes/result.py
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     4311 2023-07-19 09:11:30.000000 uncertainty-datatypes-1.0.5/udatatypes/ubool.py
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    20720 2023-07-19 08:56:16.000000 uncertainty-datatypes-1.0.5/udatatypes/unumbers.py
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     4302 2023-07-19 08:56:26.000000 uncertainty-datatypes-1.0.5/udatatypes/utypes.py
-drwxr-xr-x   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-19 09:14:20.622092 uncertainty-datatypes-1.0.5/uncertainty_datatypes.egg-info/
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    10214 2023-07-19 09:14:20.000000 uncertainty-datatypes-1.0.5/uncertainty_datatypes.egg-info/PKG-INFO
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)      421 2023-07-19 09:14:20.000000 uncertainty-datatypes-1.0.5/uncertainty_datatypes.egg-info/SOURCES.txt
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)        1 2023-07-19 09:14:20.000000 uncertainty-datatypes-1.0.5/uncertainty_datatypes.egg-info/dependency_links.txt
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)       14 2023-07-19 09:14:20.000000 uncertainty-datatypes-1.0.5/uncertainty_datatypes.egg-info/requires.txt
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)       11 2023-07-19 09:14:20.000000 uncertainty-datatypes-1.0.5/uncertainty_datatypes.egg-info/top_level.txt
+drwxr-xr-x   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-19 09:36:54.106305 uncertainty-datatypes-1.0.6/
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     1099 2023-07-17 07:54:55.000000 uncertainty-datatypes-1.0.6/LICENSE
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    10499 2023-07-19 09:36:54.106145 uncertainty-datatypes-1.0.6/PKG-INFO
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     9728 2023-07-19 09:35:28.000000 uncertainty-datatypes-1.0.6/README.md
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)      854 2023-07-19 09:32:10.000000 uncertainty-datatypes-1.0.6/pyproject.toml
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)       38 2023-07-19 09:36:54.106338 uncertainty-datatypes-1.0.6/setup.cfg
+drwxr-xr-x   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-19 09:36:54.104719 uncertainty-datatypes-1.0.6/test/
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     4428 2023-07-18 10:58:49.000000 uncertainty-datatypes-1.0.6/test/test_ubool.py
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    19028 2023-07-19 08:55:34.000000 uncertainty-datatypes-1.0.6/test/test_ufloat.py
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    17972 2023-07-19 08:39:29.000000 uncertainty-datatypes-1.0.6/test/test_uint.py
+drwxr-xr-x   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-19 09:36:54.105320 uncertainty-datatypes-1.0.6/udatatypes/
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-14 08:59:58.000000 uncertainty-datatypes-1.0.6/udatatypes/__init__.py
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)      328 2023-07-17 11:29:42.000000 uncertainty-datatypes-1.0.6/udatatypes/result.py
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     4311 2023-07-19 09:11:30.000000 uncertainty-datatypes-1.0.6/udatatypes/ubool.py
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    20720 2023-07-19 08:56:16.000000 uncertainty-datatypes-1.0.6/udatatypes/unumbers.py
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     4302 2023-07-19 08:56:26.000000 uncertainty-datatypes-1.0.6/udatatypes/utypes.py
+drwxr-xr-x   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-19 09:36:54.105962 uncertainty-datatypes-1.0.6/uncertainty_datatypes.egg-info/
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    10499 2023-07-19 09:36:54.000000 uncertainty-datatypes-1.0.6/uncertainty_datatypes.egg-info/PKG-INFO
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)      421 2023-07-19 09:36:54.000000 uncertainty-datatypes-1.0.6/uncertainty_datatypes.egg-info/SOURCES.txt
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)        1 2023-07-19 09:36:54.000000 uncertainty-datatypes-1.0.6/uncertainty_datatypes.egg-info/dependency_links.txt
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)       14 2023-07-19 09:36:54.000000 uncertainty-datatypes-1.0.6/uncertainty_datatypes.egg-info/requires.txt
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)       11 2023-07-19 09:36:54.000000 uncertainty-datatypes-1.0.6/uncertainty_datatypes.egg-info/top_level.txt
```

### Comparing `uncertainty-datatypes-1.0.5/LICENSE` & `uncertainty-datatypes-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `uncertainty-datatypes-1.0.5/PKG-INFO` & `uncertainty-datatypes-1.0.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: uncertainty-datatypes
-Version: 1.0.5
-Summary: Uncertainty Datatypes Library
-Author: Atenea Research Group, University of Malaga, Spain
-Project-URL: Homepage, https://github.com/atenearesearchgroup/uncertainty
-Project-URL: Bug Tracker, https://github.com/atenearesearchgroup/uncertainty/issues
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Education
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Uncertainty Python Library
 
 Uncertainty is a Python library providing uncertainty datatypes including u-type, a-type and s-type: 
 1. **u-type** datatypes: ubool, uint, ufloat, ustr, uenum.
     Type U is a pair (x, u), noted x ± u, that represents a random variable whose average is x and standard deviation is u.
 2. **a-type** datatypes: abool, aint, afloat.
     Type A, maintain the set of the measured values as X = {x1,...,xn}, x ± u could be calculated as the mean and standard deviation.
@@ -32,19 +13,21 @@
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install foobar.
 
 ```bash
 pip install uncertainty-datatypes
 ```
+
 <sub>Note pip3 may be used instead of pip</sub> 
 
 ## Usage
 
 Import all the datatypes and functions using:
+
 ```python
 from udatatypes.utypes import *
 ```
 
 ---
 
 ## The ubool type
@@ -56,96 +39,105 @@
 y = ubool('0.7')  # A str can be used if it represent a float[0, 1]
 z = ubool(1)      # int 0 or 1 can be used too.
 w = ubool(False)  # True or False can be also used. 
                    #True -> ubool(1.0) and False -> ubool(0.0).
 ```
 
 ubools can be used as conditional statements.
+
 ```python
 if x:
     'executed'
 ```
+
 **ubool never should be used with python logical operators** (and, or and not keywords). **ubool special logical operators must be used** (see below.)
 
 #### Logical operators
+
 The python logical operators ('and', 'or', and 'not' keywords)  have a different meaning when they are being used with objects. Therefore, **ubool special logical operators must be used**. 
 
 ubool logical operators include: *AND*, *OR*, *NOT*, *XOR*, *IMPLIES, and *EQUIVALENT*. The library offers the following four ways of using logical operators: 
 * Operator: ``` x & y ``` 
 * Special operator: ``` x |AND| y ``` 
 * The ubool method: ``` x.AND(y) ``` 
 * A function: ``` AND(x, y) ```
 
 The table below summarizes all the possible usages.
 
-| Logical <br/> Operation | Operator      | Special <br/> Operator  | Method | Function |
-|:-----------:|:---------------:|:-------------------:|:-------------:|:----------:|
-| AND      | ``` x & y ``` | ``` x |AND| y ``` | ``` x.AND(y) ```  | ``` AND(x, y) ```|
-| OR       | ``` x | y ``` | ``` x |OR| y ``` | ``` x.OR(y) ```  | ``` OR(x, y) ```|
-| XOR      | ``` x ^ y ``` | ``` x |XOR| y ```| ``` x.XOR(y) ``` | ``` XOR(x, y) ```|
-| NOT      | ``` ~ x ``` | | ``` x.NOT() ``` | ``` NOT(x) ```|
-| IMPLIES      | ``` x >> y ``` | ``` x |IMPLIES| y ```| ``` x.IMPLIES(y) ``` | ``` IMPLIES(x, y) ```|
-| EQUIVALENT      | ``` x == y ``` | ``` x |EQUIVALENT| y ```<br />``` x |EQUALS| y ```| ``` x.EQUIVALENT(y) ```<br />``` x.EQUALS(y) ```| ``` EQUIVALENT(x, y) ```<br />``` EQUALS(x, y) ```|
-| DISTINCT      | ``` x != y ``` | ``` x |DISTINCT| y ```| ``` x.DISTINCT(y) ```| ``` DISTINCT(x, y) ```|
+| Operation  | Operator       | Special <br/> Operator   | Method                  | Function                 |
+|:----------:|:--------------:|:------------------------:|:-----------------------:|:------------------------:|
+| AND        | ``` x & y ```  | ``` x |AND| y ```        | ``` x.AND(y) ```        | ``` AND(x, y) ```        |
+| OR         | ``` x | y ```  | ``` x |OR| y ```         | ``` x.OR(y) ```         | ``` OR(x, y) ```         |
+| XOR        | ``` x ^ y ```  | ``` x |XOR| y ```        | ``` x.XOR(y) ```        | ``` XOR(x, y) ```        |
+| NOT        | ``` ~ x ```    |                          | ``` x.NOT() ```         | ``` NOT(x) ```           |
+| IMPLIES    | ``` x >> y ``` | ``` x |IMPLIES| y ```    | ``` x.IMPLIES(y) ```    | ``` IMPLIES(x, y) ```    |
+| EQUIVALENT | ``` x == y ``` | ``` x |EQUIVALENT| y ``` | ``` x.EQUIVALENT(y) ``` | ``` EQUIVALENT(x, y) ``` |
+| EQUALS     | ``` x == y ``` |  ``` x |EQUALS| y ```    | ``` x.EQUALS(y) ```     | ``` EQUALS(x, y) ```     |
+| DISTINCT   | ``` x != y ``` | ``` x |DISTINCT| y ```   | ``` x.DISTINCT(y) ```   | ``` DISTINCT(x, y) ```   |
 
-Operators or special operators must be surrounded by parentheses due operator precedence. Meanwhile, using a method or the function provides the highest precedence.
+<sub> Operators or special operators must be surrounded by parentheses due operator precedence. Meanwhile, using a method or the function provides the highest precedence. </sub>
+
+*ubool Code example:*
 
-*Code example:*
 ```python
 x = ubool(0.3)
 y = ubool(0.8)
 z = ubool(0.5)
 
 w = (~x & y) |IMPLIES| (y ^ z)
 # w = ubool(0.608)
 ```
 
 #### Usage with bool
+
 ubools can be used together with python's bools, but ubool operators must be used. 
 
 ```python
 if x & (3 > 2): 
     # do something
 elif OR(x, 3 > 2): 
     # do something
 elif x |XOR| (3 > 2):
     # do something
 while x.AND(3 > 2):
     # do something
 ```
+
 <sub>Note that, python logical operations (3 > 2) must be enclosed by paretheses. True values (result of 3 > 2) are converted into a ubool(1.0) and False into ubool(0.0).</sub>
 
 #### Level of certainty
-The level of certainty changes when a ubool is evaluated to True. 
-The level of certainty can be set using **ubool.setCertainty()** function. By default, 0.9 is used.
+
+The level of certainty changes when a ubool is evaluated to True. The level of certainty can be set using **ubool.setCertainty()** function. By default, 0.9 is used.
 
 ```python
 y = ubool(0.7)
 
 # Certainty by default: 0.9
 if y:   # y is ubool(0.7) < 0.9
     'not executed'
 
 ubool.setCertainty(0.5)
 if y:   # y is ubool(0.7) >= 0.5
     'executed'
 ```
+
 ---
 
 ## The ufloat type
 
 A ufloat can be instantiated providing the value and the certainty. Value is any float and Certainty is a float[0, 1] where 1 is the highest possible certainty while 0 is the lowest.
 
 ```python
 x = ufloat(-230.30, 0.7) 
 y = ufloat(233, '0.7')  # Data can be provided as str, int or float.
 # y = ufloat(233.0, 0.7)
 ```
 
 #### Operators
+
 ufloat operators include: *ADD*, *SUB*, *MUL*, *DIV*, *FLOOR DIV*, *NEG*, *POWER*. The table below summarizes all the possible operations.
 
 | Operation | Operator      | Method | Function |
 |:---------:|:------------:|:-----------------:|:----------------:|
 | ADD      | ``` x + y ``` | ``` x.add(y) ```  | ``` add(x, y) ```|
 | SUB      | ``` x - y ``` | ``` x.sub(y) ```  | ``` sub(x, y) ```|
 | MUL      | ``` x * y ``` | ``` x.mul(y) ```  | ``` mul(x, y) ```|
@@ -153,26 +145,29 @@
 | FLOOR DIV| ``` x // y ```| ``` x.floordiv(y) ``` | ``` floordiv(x, y) ```|
 | NEG      | ``` ~ x ```   | ``` x.neg(y) ```  | ``` neg(x, y) ```|
 | POW      | ``` x ** y ```| ``` x.power(y) ```| ``` pow(x, y) ```|
 
 <sub>Arithmetic operators are recommended. The usage of methods or functions changes the precedence of the operation at execution as if it were enclosed in parentheses.</sub>
 
 ##### Covariance methods
+
 Methods *add*, *sub*, *mul*, *div*, *floordiv* allows the usage of the covariance as an additional parameter.
+
 ```python
 x = ufloat(92.69, 3.8)
 y = ufloat(56.50, 1.83)
 
 w = x.add(y, covariance = 0.0)
 # w = ufloat(149.190, 4.218)
 z = x.add(y, covariance = 12.4)
 # z = ufloat(149.190, 6.526)
 ```
 
 *ufloat operators Code example:*
+
 ```python
 x = ufloat(925.69, 23.8)
 y = ufloat(536.50, 31.83)
 z = ufloat(-3404, 4.76)
 
 w = (x / y)**2 - z
 # w = ufloat(3406.977, 5.946)
@@ -197,25 +192,29 @@
 x = uint(-654, 2.4) 
 # y = uint(-654, 2.4)
 y = uint(432, '5.7')  # Data can be provided as str, int or float.
 # y = uint(432, 5.7)
 ```
 
 #### Operators
+
 The operator MOD is included for uint. The rest of the operators available for uint are the same than those provided for ufloat: *ADD*, *SUB*, *MUL*, *DIV*, *FLOOR DIV*, *NEG*, *POWER*. 
 
 | Operation | Operator      | Method | Function |
 |:---------:|:------------:|:-----------------:|:----------------:|
 | MOD      | ``` x % y ``` | ``` x.mod(y) ```  | ``` mod(x, y) ```|
+
 <sub>Arithmetic operators are recommended. The usage of methods or functions changes the precedence of the operation at execution as if it were enclosed in parentheses.</sub>
 
 ##### Covariance methods
+
 Covariance methods are also provided for the uint type.
 
 *uint operators Code example:*
+
 ```python
 x = uint(145, 3.4)
 y = uint(56, 4.35)
 z = uint(23, 5.2)
 
 w = (x // y)**3 % z
 # w = uint(8, 1.246)
@@ -227,14 +226,15 @@
 ```python
 x = uint(5, 23.8)
 y = x - 3
 # y = ufloat(2, 23.800)
 z = y - ufloat(0.3, 10.3)
 # z = ufloat(1.700, 25.933)
 ```
+
 --- 
 
 ## Comparison Operators
 Comparison between uint and ufloat can be made using the comparison operators: <, <=, >, >=, == and != and the methods.
 
 
 | Operation | Operator      | Method | Function |
@@ -244,23 +244,25 @@
 | Greater | ``` x > y ``` | ``` x.gt(y) ```  | ``` gt(x, y) ```|
 | Greater or Equals | ``` x >= y ``` | ``` x.ge(y) ```  | ``` ge(x, y) ```|
 | Equals | ``` x == y ``` | ``` x.eq(y) ```  | ``` eq(x, y) ```|
 | Not Equals | ``` x != y ``` | ``` x.ne(y) ```  | ``` ne(x, y) ```|
 
 <sub>Operators are recommended. The usage of methods or functions changes the precedence of the operation at execution as if it were enclosed in parentheses.</sub>
 
-*Code example:*
+*ufloat Comparison Code example:*
+
 ```python
 x = uint(100, 0.7)
 y = ufloat(900.45, 0.6)
 
 if y > x:
     w = y - x # ufloat - uint
     # w = ufloat(800.450, 0.922)
 ```
+
 ---
 
 ## Math functions
 
 The library provides the following math functions for uint and ufloat types: 
 *sqrt*(), *sin*(), *cos*(), *tan*(), *atan*(), *acos*(), *asin*(), *inverse*(), *floor*(), *round*(), *max*(...), *min*(...)
 
@@ -272,14 +274,16 @@
     uint(23, 0.6), 
     floor(ufloat(3.4, 0.8)),
     uint(84, 0.6)
 )
 # m = uint(84, 0.600)
 ``` 
 
+---
+
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `uncertainty-datatypes-1.0.5/README.md` & `uncertainty-datatypes-1.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: uncertainty-datatypes
+Version: 1.0.6
+Summary: Uncertainty Datatypes Library
+Author: Atenea Research Group, University of Malaga, Spain
+Project-URL: Homepage, https://github.com/atenearesearchgroup/uncertainty
+Project-URL: Bug Tracker, https://github.com/atenearesearchgroup/uncertainty/issues
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Education
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Uncertainty Python Library
 
 Uncertainty is a Python library providing uncertainty datatypes including u-type, a-type and s-type: 
 1. **u-type** datatypes: ubool, uint, ufloat, ustr, uenum.
     Type U is a pair (x, u), noted x ± u, that represents a random variable whose average is x and standard deviation is u.
 2. **a-type** datatypes: abool, aint, afloat.
     Type A, maintain the set of the measured values as X = {x1,...,xn}, x ± u could be calculated as the mean and standard deviation.
@@ -13,19 +32,21 @@
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install foobar.
 
 ```bash
 pip install uncertainty-datatypes
 ```
+
 <sub>Note pip3 may be used instead of pip</sub> 
 
 ## Usage
 
 Import all the datatypes and functions using:
+
 ```python
 from udatatypes.utypes import *
 ```
 
 ---
 
 ## The ubool type
@@ -37,96 +58,105 @@
 y = ubool('0.7')  # A str can be used if it represent a float[0, 1]
 z = ubool(1)      # int 0 or 1 can be used too.
 w = ubool(False)  # True or False can be also used. 
                    #True -> ubool(1.0) and False -> ubool(0.0).
 ```
 
 ubools can be used as conditional statements.
+
 ```python
 if x:
     'executed'
 ```
+
 **ubool never should be used with python logical operators** (and, or and not keywords). **ubool special logical operators must be used** (see below.)
 
 #### Logical operators
+
 The python logical operators ('and', 'or', and 'not' keywords)  have a different meaning when they are being used with objects. Therefore, **ubool special logical operators must be used**. 
 
 ubool logical operators include: *AND*, *OR*, *NOT*, *XOR*, *IMPLIES, and *EQUIVALENT*. The library offers the following four ways of using logical operators: 
 * Operator: ``` x & y ``` 
 * Special operator: ``` x |AND| y ``` 
 * The ubool method: ``` x.AND(y) ``` 
 * A function: ``` AND(x, y) ```
 
 The table below summarizes all the possible usages.
 
-| Logical <br/> Operation | Operator      | Special <br/> Operator  | Method | Function |
-|:-----------:|:---------------:|:-------------------:|:-------------:|:----------:|
-| AND      | ``` x & y ``` | ``` x |AND| y ``` | ``` x.AND(y) ```  | ``` AND(x, y) ```|
-| OR       | ``` x | y ``` | ``` x |OR| y ``` | ``` x.OR(y) ```  | ``` OR(x, y) ```|
-| XOR      | ``` x ^ y ``` | ``` x |XOR| y ```| ``` x.XOR(y) ``` | ``` XOR(x, y) ```|
-| NOT      | ``` ~ x ``` | | ``` x.NOT() ``` | ``` NOT(x) ```|
-| IMPLIES      | ``` x >> y ``` | ``` x |IMPLIES| y ```| ``` x.IMPLIES(y) ``` | ``` IMPLIES(x, y) ```|
-| EQUIVALENT      | ``` x == y ``` | ``` x |EQUIVALENT| y ```<br />``` x |EQUALS| y ```| ``` x.EQUIVALENT(y) ```<br />``` x.EQUALS(y) ```| ``` EQUIVALENT(x, y) ```<br />``` EQUALS(x, y) ```|
-| DISTINCT      | ``` x != y ``` | ``` x |DISTINCT| y ```| ``` x.DISTINCT(y) ```| ``` DISTINCT(x, y) ```|
+| Operation  | Operator       | Special <br/> Operator   | Method                  | Function                 |
+|:----------:|:--------------:|:------------------------:|:-----------------------:|:------------------------:|
+| AND        | ``` x & y ```  | ``` x |AND| y ```        | ``` x.AND(y) ```        | ``` AND(x, y) ```        |
+| OR         | ``` x | y ```  | ``` x |OR| y ```         | ``` x.OR(y) ```         | ``` OR(x, y) ```         |
+| XOR        | ``` x ^ y ```  | ``` x |XOR| y ```        | ``` x.XOR(y) ```        | ``` XOR(x, y) ```        |
+| NOT        | ``` ~ x ```    |                          | ``` x.NOT() ```         | ``` NOT(x) ```           |
+| IMPLIES    | ``` x >> y ``` | ``` x |IMPLIES| y ```    | ``` x.IMPLIES(y) ```    | ``` IMPLIES(x, y) ```    |
+| EQUIVALENT | ``` x == y ``` | ``` x |EQUIVALENT| y ``` | ``` x.EQUIVALENT(y) ``` | ``` EQUIVALENT(x, y) ``` |
+| EQUALS     | ``` x == y ``` |  ``` x |EQUALS| y ```    | ``` x.EQUALS(y) ```     | ``` EQUALS(x, y) ```     |
+| DISTINCT   | ``` x != y ``` | ``` x |DISTINCT| y ```   | ``` x.DISTINCT(y) ```   | ``` DISTINCT(x, y) ```   |
 
-Operators or special operators must be surrounded by parentheses due operator precedence. Meanwhile, using a method or the function provides the highest precedence.
+<sub> Operators or special operators must be surrounded by parentheses due operator precedence. Meanwhile, using a method or the function provides the highest precedence. </sub>
+
+*ubool Code example:*
 
-*Code example:*
 ```python
 x = ubool(0.3)
 y = ubool(0.8)
 z = ubool(0.5)
 
 w = (~x & y) |IMPLIES| (y ^ z)
 # w = ubool(0.608)
 ```
 
 #### Usage with bool
+
 ubools can be used together with python's bools, but ubool operators must be used. 
 
 ```python
 if x & (3 > 2): 
     # do something
 elif OR(x, 3 > 2): 
     # do something
 elif x |XOR| (3 > 2):
     # do something
 while x.AND(3 > 2):
     # do something
 ```
+
 <sub>Note that, python logical operations (3 > 2) must be enclosed by paretheses. True values (result of 3 > 2) are converted into a ubool(1.0) and False into ubool(0.0).</sub>
 
 #### Level of certainty
-The level of certainty changes when a ubool is evaluated to True. 
-The level of certainty can be set using **ubool.setCertainty()** function. By default, 0.9 is used.
+
+The level of certainty changes when a ubool is evaluated to True. The level of certainty can be set using **ubool.setCertainty()** function. By default, 0.9 is used.
 
 ```python
 y = ubool(0.7)
 
 # Certainty by default: 0.9
 if y:   # y is ubool(0.7) < 0.9
     'not executed'
 
 ubool.setCertainty(0.5)
 if y:   # y is ubool(0.7) >= 0.5
     'executed'
 ```
+
 ---
 
 ## The ufloat type
 
 A ufloat can be instantiated providing the value and the certainty. Value is any float and Certainty is a float[0, 1] where 1 is the highest possible certainty while 0 is the lowest.
 
 ```python
 x = ufloat(-230.30, 0.7) 
 y = ufloat(233, '0.7')  # Data can be provided as str, int or float.
 # y = ufloat(233.0, 0.7)
 ```
 
 #### Operators
+
 ufloat operators include: *ADD*, *SUB*, *MUL*, *DIV*, *FLOOR DIV*, *NEG*, *POWER*. The table below summarizes all the possible operations.
 
 | Operation | Operator      | Method | Function |
 |:---------:|:------------:|:-----------------:|:----------------:|
 | ADD      | ``` x + y ``` | ``` x.add(y) ```  | ``` add(x, y) ```|
 | SUB      | ``` x - y ``` | ``` x.sub(y) ```  | ``` sub(x, y) ```|
 | MUL      | ``` x * y ``` | ``` x.mul(y) ```  | ``` mul(x, y) ```|
@@ -134,26 +164,29 @@
 | FLOOR DIV| ``` x // y ```| ``` x.floordiv(y) ``` | ``` floordiv(x, y) ```|
 | NEG      | ``` ~ x ```   | ``` x.neg(y) ```  | ``` neg(x, y) ```|
 | POW      | ``` x ** y ```| ``` x.power(y) ```| ``` pow(x, y) ```|
 
 <sub>Arithmetic operators are recommended. The usage of methods or functions changes the precedence of the operation at execution as if it were enclosed in parentheses.</sub>
 
 ##### Covariance methods
+
 Methods *add*, *sub*, *mul*, *div*, *floordiv* allows the usage of the covariance as an additional parameter.
+
 ```python
 x = ufloat(92.69, 3.8)
 y = ufloat(56.50, 1.83)
 
 w = x.add(y, covariance = 0.0)
 # w = ufloat(149.190, 4.218)
 z = x.add(y, covariance = 12.4)
 # z = ufloat(149.190, 6.526)
 ```
 
 *ufloat operators Code example:*
+
 ```python
 x = ufloat(925.69, 23.8)
 y = ufloat(536.50, 31.83)
 z = ufloat(-3404, 4.76)
 
 w = (x / y)**2 - z
 # w = ufloat(3406.977, 5.946)
@@ -178,25 +211,29 @@
 x = uint(-654, 2.4) 
 # y = uint(-654, 2.4)
 y = uint(432, '5.7')  # Data can be provided as str, int or float.
 # y = uint(432, 5.7)
 ```
 
 #### Operators
+
 The operator MOD is included for uint. The rest of the operators available for uint are the same than those provided for ufloat: *ADD*, *SUB*, *MUL*, *DIV*, *FLOOR DIV*, *NEG*, *POWER*. 
 
 | Operation | Operator      | Method | Function |
 |:---------:|:------------:|:-----------------:|:----------------:|
 | MOD      | ``` x % y ``` | ``` x.mod(y) ```  | ``` mod(x, y) ```|
+
 <sub>Arithmetic operators are recommended. The usage of methods or functions changes the precedence of the operation at execution as if it were enclosed in parentheses.</sub>
 
 ##### Covariance methods
+
 Covariance methods are also provided for the uint type.
 
 *uint operators Code example:*
+
 ```python
 x = uint(145, 3.4)
 y = uint(56, 4.35)
 z = uint(23, 5.2)
 
 w = (x // y)**3 % z
 # w = uint(8, 1.246)
@@ -208,14 +245,15 @@
 ```python
 x = uint(5, 23.8)
 y = x - 3
 # y = ufloat(2, 23.800)
 z = y - ufloat(0.3, 10.3)
 # z = ufloat(1.700, 25.933)
 ```
+
 --- 
 
 ## Comparison Operators
 Comparison between uint and ufloat can be made using the comparison operators: <, <=, >, >=, == and != and the methods.
 
 
 | Operation | Operator      | Method | Function |
@@ -225,23 +263,25 @@
 | Greater | ``` x > y ``` | ``` x.gt(y) ```  | ``` gt(x, y) ```|
 | Greater or Equals | ``` x >= y ``` | ``` x.ge(y) ```  | ``` ge(x, y) ```|
 | Equals | ``` x == y ``` | ``` x.eq(y) ```  | ``` eq(x, y) ```|
 | Not Equals | ``` x != y ``` | ``` x.ne(y) ```  | ``` ne(x, y) ```|
 
 <sub>Operators are recommended. The usage of methods or functions changes the precedence of the operation at execution as if it were enclosed in parentheses.</sub>
 
-*Code example:*
+*ufloat Comparison Code example:*
+
 ```python
 x = uint(100, 0.7)
 y = ufloat(900.45, 0.6)
 
 if y > x:
     w = y - x # ufloat - uint
     # w = ufloat(800.450, 0.922)
 ```
+
 ---
 
 ## Math functions
 
 The library provides the following math functions for uint and ufloat types: 
 *sqrt*(), *sin*(), *cos*(), *tan*(), *atan*(), *acos*(), *asin*(), *inverse*(), *floor*(), *round*(), *max*(...), *min*(...)
 
@@ -253,14 +293,16 @@
     uint(23, 0.6), 
     floor(ufloat(3.4, 0.8)),
     uint(84, 0.6)
 )
 # m = uint(84, 0.600)
 ``` 
 
+---
+
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `uncertainty-datatypes-1.0.5/pyproject.toml` & `uncertainty-datatypes-1.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "uncertainty-datatypes"
-version = "1.0.5"
+version = "1.0.6"
 authors = [
   { name="Atenea Research Group, University of Malaga, Spain" },
 ]
 description = "Uncertainty Datatypes Library"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers=[
```

### Comparing `uncertainty-datatypes-1.0.5/test/test_ubool.py` & `uncertainty-datatypes-1.0.6/test/test_ubool.py`

 * *Files identical despite different names*

### Comparing `uncertainty-datatypes-1.0.5/test/test_ufloat.py` & `uncertainty-datatypes-1.0.6/test/test_ufloat.py`

 * *Files identical despite different names*

### Comparing `uncertainty-datatypes-1.0.5/test/test_uint.py` & `uncertainty-datatypes-1.0.6/test/test_uint.py`

 * *Files identical despite different names*

### Comparing `uncertainty-datatypes-1.0.5/udatatypes/ubool.py` & `uncertainty-datatypes-1.0.6/udatatypes/ubool.py`

 * *Files identical despite different names*

### Comparing `uncertainty-datatypes-1.0.5/udatatypes/unumbers.py` & `uncertainty-datatypes-1.0.6/udatatypes/unumbers.py`

 * *Files identical despite different names*

### Comparing `uncertainty-datatypes-1.0.5/udatatypes/utypes.py` & `uncertainty-datatypes-1.0.6/udatatypes/utypes.py`

 * *Files identical despite different names*

### Comparing `uncertainty-datatypes-1.0.5/uncertainty_datatypes.egg-info/PKG-INFO` & `uncertainty-datatypes-1.0.6/uncertainty_datatypes.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uncertainty-datatypes
-Version: 1.0.5
+Version: 1.0.6
 Summary: Uncertainty Datatypes Library
 Author: Atenea Research Group, University of Malaga, Spain
 Project-URL: Homepage, https://github.com/atenearesearchgroup/uncertainty
 Project-URL: Bug Tracker, https://github.com/atenearesearchgroup/uncertainty/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -32,19 +32,21 @@
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install foobar.
 
 ```bash
 pip install uncertainty-datatypes
 ```
+
 <sub>Note pip3 may be used instead of pip</sub> 
 
 ## Usage
 
 Import all the datatypes and functions using:
+
 ```python
 from udatatypes.utypes import *
 ```
 
 ---
 
 ## The ubool type
@@ -56,96 +58,105 @@
 y = ubool('0.7')  # A str can be used if it represent a float[0, 1]
 z = ubool(1)      # int 0 or 1 can be used too.
 w = ubool(False)  # True or False can be also used. 
                    #True -> ubool(1.0) and False -> ubool(0.0).
 ```
 
 ubools can be used as conditional statements.
+
 ```python
 if x:
     'executed'
 ```
+
 **ubool never should be used with python logical operators** (and, or and not keywords). **ubool special logical operators must be used** (see below.)
 
 #### Logical operators
+
 The python logical operators ('and', 'or', and 'not' keywords)  have a different meaning when they are being used with objects. Therefore, **ubool special logical operators must be used**. 
 
 ubool logical operators include: *AND*, *OR*, *NOT*, *XOR*, *IMPLIES, and *EQUIVALENT*. The library offers the following four ways of using logical operators: 
 * Operator: ``` x & y ``` 
 * Special operator: ``` x |AND| y ``` 
 * The ubool method: ``` x.AND(y) ``` 
 * A function: ``` AND(x, y) ```
 
 The table below summarizes all the possible usages.
 
-| Logical <br/> Operation | Operator      | Special <br/> Operator  | Method | Function |
-|:-----------:|:---------------:|:-------------------:|:-------------:|:----------:|
-| AND      | ``` x & y ``` | ``` x |AND| y ``` | ``` x.AND(y) ```  | ``` AND(x, y) ```|
-| OR       | ``` x | y ``` | ``` x |OR| y ``` | ``` x.OR(y) ```  | ``` OR(x, y) ```|
-| XOR      | ``` x ^ y ``` | ``` x |XOR| y ```| ``` x.XOR(y) ``` | ``` XOR(x, y) ```|
-| NOT      | ``` ~ x ``` | | ``` x.NOT() ``` | ``` NOT(x) ```|
-| IMPLIES      | ``` x >> y ``` | ``` x |IMPLIES| y ```| ``` x.IMPLIES(y) ``` | ``` IMPLIES(x, y) ```|
-| EQUIVALENT      | ``` x == y ``` | ``` x |EQUIVALENT| y ```<br />``` x |EQUALS| y ```| ``` x.EQUIVALENT(y) ```<br />``` x.EQUALS(y) ```| ``` EQUIVALENT(x, y) ```<br />``` EQUALS(x, y) ```|
-| DISTINCT      | ``` x != y ``` | ``` x |DISTINCT| y ```| ``` x.DISTINCT(y) ```| ``` DISTINCT(x, y) ```|
+| Operation  | Operator       | Special <br/> Operator   | Method                  | Function                 |
+|:----------:|:--------------:|:------------------------:|:-----------------------:|:------------------------:|
+| AND        | ``` x & y ```  | ``` x |AND| y ```        | ``` x.AND(y) ```        | ``` AND(x, y) ```        |
+| OR         | ``` x | y ```  | ``` x |OR| y ```         | ``` x.OR(y) ```         | ``` OR(x, y) ```         |
+| XOR        | ``` x ^ y ```  | ``` x |XOR| y ```        | ``` x.XOR(y) ```        | ``` XOR(x, y) ```        |
+| NOT        | ``` ~ x ```    |                          | ``` x.NOT() ```         | ``` NOT(x) ```           |
+| IMPLIES    | ``` x >> y ``` | ``` x |IMPLIES| y ```    | ``` x.IMPLIES(y) ```    | ``` IMPLIES(x, y) ```    |
+| EQUIVALENT | ``` x == y ``` | ``` x |EQUIVALENT| y ``` | ``` x.EQUIVALENT(y) ``` | ``` EQUIVALENT(x, y) ``` |
+| EQUALS     | ``` x == y ``` |  ``` x |EQUALS| y ```    | ``` x.EQUALS(y) ```     | ``` EQUALS(x, y) ```     |
+| DISTINCT   | ``` x != y ``` | ``` x |DISTINCT| y ```   | ``` x.DISTINCT(y) ```   | ``` DISTINCT(x, y) ```   |
+
+<sub> Operators or special operators must be surrounded by parentheses due operator precedence. Meanwhile, using a method or the function provides the highest precedence. </sub>
 
-Operators or special operators must be surrounded by parentheses due operator precedence. Meanwhile, using a method or the function provides the highest precedence.
+*ubool Code example:*
 
-*Code example:*
 ```python
 x = ubool(0.3)
 y = ubool(0.8)
 z = ubool(0.5)
 
 w = (~x & y) |IMPLIES| (y ^ z)
 # w = ubool(0.608)
 ```
 
 #### Usage with bool
+
 ubools can be used together with python's bools, but ubool operators must be used. 
 
 ```python
 if x & (3 > 2): 
     # do something
 elif OR(x, 3 > 2): 
     # do something
 elif x |XOR| (3 > 2):
     # do something
 while x.AND(3 > 2):
     # do something
 ```
+
 <sub>Note that, python logical operations (3 > 2) must be enclosed by paretheses. True values (result of 3 > 2) are converted into a ubool(1.0) and False into ubool(0.0).</sub>
 
 #### Level of certainty
-The level of certainty changes when a ubool is evaluated to True. 
-The level of certainty can be set using **ubool.setCertainty()** function. By default, 0.9 is used.
+
+The level of certainty changes when a ubool is evaluated to True. The level of certainty can be set using **ubool.setCertainty()** function. By default, 0.9 is used.
 
 ```python
 y = ubool(0.7)
 
 # Certainty by default: 0.9
 if y:   # y is ubool(0.7) < 0.9
     'not executed'
 
 ubool.setCertainty(0.5)
 if y:   # y is ubool(0.7) >= 0.5
     'executed'
 ```
+
 ---
 
 ## The ufloat type
 
 A ufloat can be instantiated providing the value and the certainty. Value is any float and Certainty is a float[0, 1] where 1 is the highest possible certainty while 0 is the lowest.
 
 ```python
 x = ufloat(-230.30, 0.7) 
 y = ufloat(233, '0.7')  # Data can be provided as str, int or float.
 # y = ufloat(233.0, 0.7)
 ```
 
 #### Operators
+
 ufloat operators include: *ADD*, *SUB*, *MUL*, *DIV*, *FLOOR DIV*, *NEG*, *POWER*. The table below summarizes all the possible operations.
 
 | Operation | Operator      | Method | Function |
 |:---------:|:------------:|:-----------------:|:----------------:|
 | ADD      | ``` x + y ``` | ``` x.add(y) ```  | ``` add(x, y) ```|
 | SUB      | ``` x - y ``` | ``` x.sub(y) ```  | ``` sub(x, y) ```|
 | MUL      | ``` x * y ``` | ``` x.mul(y) ```  | ``` mul(x, y) ```|
@@ -153,26 +164,29 @@
 | FLOOR DIV| ``` x // y ```| ``` x.floordiv(y) ``` | ``` floordiv(x, y) ```|
 | NEG      | ``` ~ x ```   | ``` x.neg(y) ```  | ``` neg(x, y) ```|
 | POW      | ``` x ** y ```| ``` x.power(y) ```| ``` pow(x, y) ```|
 
 <sub>Arithmetic operators are recommended. The usage of methods or functions changes the precedence of the operation at execution as if it were enclosed in parentheses.</sub>
 
 ##### Covariance methods
+
 Methods *add*, *sub*, *mul*, *div*, *floordiv* allows the usage of the covariance as an additional parameter.
+
 ```python
 x = ufloat(92.69, 3.8)
 y = ufloat(56.50, 1.83)
 
 w = x.add(y, covariance = 0.0)
 # w = ufloat(149.190, 4.218)
 z = x.add(y, covariance = 12.4)
 # z = ufloat(149.190, 6.526)
 ```
 
 *ufloat operators Code example:*
+
 ```python
 x = ufloat(925.69, 23.8)
 y = ufloat(536.50, 31.83)
 z = ufloat(-3404, 4.76)
 
 w = (x / y)**2 - z
 # w = ufloat(3406.977, 5.946)
@@ -197,25 +211,29 @@
 x = uint(-654, 2.4) 
 # y = uint(-654, 2.4)
 y = uint(432, '5.7')  # Data can be provided as str, int or float.
 # y = uint(432, 5.7)
 ```
 
 #### Operators
+
 The operator MOD is included for uint. The rest of the operators available for uint are the same than those provided for ufloat: *ADD*, *SUB*, *MUL*, *DIV*, *FLOOR DIV*, *NEG*, *POWER*. 
 
 | Operation | Operator      | Method | Function |
 |:---------:|:------------:|:-----------------:|:----------------:|
 | MOD      | ``` x % y ``` | ``` x.mod(y) ```  | ``` mod(x, y) ```|
+
 <sub>Arithmetic operators are recommended. The usage of methods or functions changes the precedence of the operation at execution as if it were enclosed in parentheses.</sub>
 
 ##### Covariance methods
+
 Covariance methods are also provided for the uint type.
 
 *uint operators Code example:*
+
 ```python
 x = uint(145, 3.4)
 y = uint(56, 4.35)
 z = uint(23, 5.2)
 
 w = (x // y)**3 % z
 # w = uint(8, 1.246)
@@ -227,14 +245,15 @@
 ```python
 x = uint(5, 23.8)
 y = x - 3
 # y = ufloat(2, 23.800)
 z = y - ufloat(0.3, 10.3)
 # z = ufloat(1.700, 25.933)
 ```
+
 --- 
 
 ## Comparison Operators
 Comparison between uint and ufloat can be made using the comparison operators: <, <=, >, >=, == and != and the methods.
 
 
 | Operation | Operator      | Method | Function |
@@ -244,23 +263,25 @@
 | Greater | ``` x > y ``` | ``` x.gt(y) ```  | ``` gt(x, y) ```|
 | Greater or Equals | ``` x >= y ``` | ``` x.ge(y) ```  | ``` ge(x, y) ```|
 | Equals | ``` x == y ``` | ``` x.eq(y) ```  | ``` eq(x, y) ```|
 | Not Equals | ``` x != y ``` | ``` x.ne(y) ```  | ``` ne(x, y) ```|
 
 <sub>Operators are recommended. The usage of methods or functions changes the precedence of the operation at execution as if it were enclosed in parentheses.</sub>
 
-*Code example:*
+*ufloat Comparison Code example:*
+
 ```python
 x = uint(100, 0.7)
 y = ufloat(900.45, 0.6)
 
 if y > x:
     w = y - x # ufloat - uint
     # w = ufloat(800.450, 0.922)
 ```
+
 ---
 
 ## Math functions
 
 The library provides the following math functions for uint and ufloat types: 
 *sqrt*(), *sin*(), *cos*(), *tan*(), *atan*(), *acos*(), *asin*(), *inverse*(), *floor*(), *round*(), *max*(...), *min*(...)
 
@@ -272,14 +293,16 @@
     uint(23, 0.6), 
     floor(ufloat(3.4, 0.8)),
     uint(84, 0.6)
 )
 # m = uint(84, 0.600)
 ``` 
 
+---
+
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
```

