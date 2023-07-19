# Comparing `tmp/uncertainty-datatypes-1.0.7.tar.gz` & `tmp/uncertainty-datatypes-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uncertainty-datatypes-1.0.7.tar", last modified: Wed Jul 19 09:48:48 2023, max compression
+gzip compressed data, was "uncertainty-datatypes-1.0.8.tar", last modified: Wed Jul 19 09:57:56 2023, max compression
```

## Comparing `uncertainty-datatypes-1.0.7.tar` & `uncertainty-datatypes-1.0.8.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-19 09:48:48.167018 uncertainty-datatypes-1.0.7/
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     1099 2023-07-17 07:54:55.000000 uncertainty-datatypes-1.0.7/LICENSE
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    10586 2023-07-19 09:48:48.166854 uncertainty-datatypes-1.0.7/PKG-INFO
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     9815 2023-07-19 09:44:47.000000 uncertainty-datatypes-1.0.7/README.md
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)      854 2023-07-19 09:47:33.000000 uncertainty-datatypes-1.0.7/pyproject.toml
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)       38 2023-07-19 09:48:48.167052 uncertainty-datatypes-1.0.7/setup.cfg
-drwxr-xr-x   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-19 09:48:48.165512 uncertainty-datatypes-1.0.7/test/
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     4429 2023-07-19 09:42:56.000000 uncertainty-datatypes-1.0.7/test/test_ubool.py
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    19029 2023-07-19 09:43:27.000000 uncertainty-datatypes-1.0.7/test/test_ufloat.py
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    17973 2023-07-19 09:43:23.000000 uncertainty-datatypes-1.0.7/test/test_uint.py
-drwxr-xr-x   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-19 09:48:48.166104 uncertainty-datatypes-1.0.7/uncertainty/
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-14 08:59:58.000000 uncertainty-datatypes-1.0.7/uncertainty/__init__.py
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)      328 2023-07-17 11:29:42.000000 uncertainty-datatypes-1.0.7/uncertainty/result.py
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     4311 2023-07-19 09:11:10.000000 uncertainty-datatypes-1.0.7/uncertainty/ubool.py
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    20722 2023-07-19 09:45:39.000000 uncertainty-datatypes-1.0.7/uncertainty/unumbers.py
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     4306 2023-07-19 09:44:37.000000 uncertainty-datatypes-1.0.7/uncertainty/utypes.py
-drwxr-xr-x   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-19 09:48:48.166690 uncertainty-datatypes-1.0.7/uncertainty_datatypes.egg-info/
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    10586 2023-07-19 09:48:48.000000 uncertainty-datatypes-1.0.7/uncertainty_datatypes.egg-info/PKG-INFO
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)      426 2023-07-19 09:48:48.000000 uncertainty-datatypes-1.0.7/uncertainty_datatypes.egg-info/SOURCES.txt
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)        1 2023-07-19 09:48:48.000000 uncertainty-datatypes-1.0.7/uncertainty_datatypes.egg-info/dependency_links.txt
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)       14 2023-07-19 09:48:48.000000 uncertainty-datatypes-1.0.7/uncertainty_datatypes.egg-info/requires.txt
--rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)       12 2023-07-19 09:48:48.000000 uncertainty-datatypes-1.0.7/uncertainty_datatypes.egg-info/top_level.txt
+drwxr-xr-x   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-19 09:57:56.890350 uncertainty-datatypes-1.0.8/
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     1099 2023-07-17 07:54:55.000000 uncertainty-datatypes-1.0.8/LICENSE
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    10699 2023-07-19 09:57:56.890185 uncertainty-datatypes-1.0.8/PKG-INFO
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     9928 2023-07-19 09:57:21.000000 uncertainty-datatypes-1.0.8/README.md
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)      854 2023-07-19 09:57:40.000000 uncertainty-datatypes-1.0.8/pyproject.toml
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)       38 2023-07-19 09:57:56.890391 uncertainty-datatypes-1.0.8/setup.cfg
+drwxr-xr-x   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-19 09:57:56.888760 uncertainty-datatypes-1.0.8/test/
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     4429 2023-07-19 09:42:56.000000 uncertainty-datatypes-1.0.8/test/test_ubool.py
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    19029 2023-07-19 09:43:27.000000 uncertainty-datatypes-1.0.8/test/test_ufloat.py
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)      717 2023-07-19 09:43:54.000000 uncertainty-datatypes-1.0.8/test/test_ufuncs.py
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    17973 2023-07-19 09:43:23.000000 uncertainty-datatypes-1.0.8/test/test_uint.py
+drwxr-xr-x   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-19 09:57:56.889397 uncertainty-datatypes-1.0.8/uncertainty/
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-14 08:59:58.000000 uncertainty-datatypes-1.0.8/uncertainty/__init__.py
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)      328 2023-07-17 11:29:42.000000 uncertainty-datatypes-1.0.8/uncertainty/result.py
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     4311 2023-07-19 09:11:10.000000 uncertainty-datatypes-1.0.8/uncertainty/ubool.py
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    20722 2023-07-19 09:45:39.000000 uncertainty-datatypes-1.0.8/uncertainty/unumbers.py
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)     4306 2023-07-19 09:44:37.000000 uncertainty-datatypes-1.0.8/uncertainty/utypes.py
+drwxr-xr-x   0 carlosfernandezcandel   (501) staff       (20)        0 2023-07-19 09:57:56.890022 uncertainty-datatypes-1.0.8/uncertainty_datatypes.egg-info/
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)    10699 2023-07-19 09:57:56.000000 uncertainty-datatypes-1.0.8/uncertainty_datatypes.egg-info/PKG-INFO
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)      446 2023-07-19 09:57:56.000000 uncertainty-datatypes-1.0.8/uncertainty_datatypes.egg-info/SOURCES.txt
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)        1 2023-07-19 09:57:56.000000 uncertainty-datatypes-1.0.8/uncertainty_datatypes.egg-info/dependency_links.txt
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)       14 2023-07-19 09:57:56.000000 uncertainty-datatypes-1.0.8/uncertainty_datatypes.egg-info/requires.txt
+-rw-r--r--   0 carlosfernandezcandel   (501) staff       (20)       12 2023-07-19 09:57:56.000000 uncertainty-datatypes-1.0.8/uncertainty_datatypes.egg-info/top_level.txt
```

### Comparing `uncertainty-datatypes-1.0.7/LICENSE` & `uncertainty-datatypes-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `uncertainty-datatypes-1.0.7/PKG-INFO` & `uncertainty-datatypes-1.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uncertainty-datatypes
-Version: 1.0.7
+Version: 1.0.8
 Summary: Uncertainty Datatypes Library
 Author: Atenea Research Group, University of Malaga, Spain
 Project-URL: Homepage, https://github.com/atenearesearchgroup/uncertainty
 Project-URL: Bug Tracker, https://github.com/atenearesearchgroup/uncertainty/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -78,29 +78,28 @@
 * Operator: ``` x & y ``` 
 * Special operator: ``` x |AND| y ``` 
 * The ubool method: ``` x.AND(y) ``` 
 * A function: ``` AND(x, y) ```
 
 The table below summarizes all the possible usages.
 
-| Operation  | Operator       | Special <br/> Operator   | Method                  | Function                 |
+| Operation  | Operator       | Special Operator         | Method                  | Function                 |
 |:----------:|:--------------:|:------------------------:|:-----------------------:|:------------------------:|
 | AND        | ``` x & y ```  | ``` x |AND| y ```        | ``` x.AND(y) ```        | ``` AND(x, y) ```        |
 | OR         | ``` x | y ```  | ``` x |OR| y ```         | ``` x.OR(y) ```         | ``` OR(x, y) ```         |
 | XOR        | ``` x ^ y ```  | ``` x |XOR| y ```        | ``` x.XOR(y) ```        | ``` XOR(x, y) ```        |
 | NOT        | ``` ~ x ```    |                          | ``` x.NOT() ```         | ``` NOT(x) ```           |
 | IMPLIES    | ``` x >> y ``` | ``` x |IMPLIES| y ```    | ``` x.IMPLIES(y) ```    | ``` IMPLIES(x, y) ```    |
 | EQUIVALENT | ``` x == y ``` | ``` x |EQUIVALENT| y ``` | ``` x.EQUIVALENT(y) ``` | ``` EQUIVALENT(x, y) ``` |
 | EQUALS     | ``` x == y ``` |  ``` x |EQUALS| y ```    | ``` x.EQUALS(y) ```     | ``` EQUALS(x, y) ```     |
 | DISTINCT   | ``` x != y ``` | ``` x |DISTINCT| y ```   | ``` x.DISTINCT(y) ```   | ``` DISTINCT(x, y) ```   |
 
 <sub> Operators or special operators must be surrounded by parentheses due operator precedence. Meanwhile, using a method or the function provides the highest precedence. </sub>
 
 *ubool Code example:*
-
 ```python
 x = ubool(0.3)
 y = ubool(0.8)
 z = ubool(0.5)
 
 w = (~x & y) |IMPLIES| (y ^ z)
 # w = ubool(0.608)
@@ -151,23 +150,23 @@
 # y = ufloat(233.0, 0.7)
 ```
 
 #### Operators
 
 ufloat operators include: *ADD*, *SUB*, *MUL*, *DIV*, *FLOOR DIV*, *NEG*, *POWER*. The table below summarizes all the possible operations.
 
-| Operation | Operator      | Method | Function |
-|:---------:|:------------:|:-----------------:|:----------------:|
-| ADD      | ``` x + y ``` | ``` x.add(y) ```  | ``` add(x, y) ```|
-| SUB      | ``` x - y ``` | ``` x.sub(y) ```  | ``` sub(x, y) ```|
-| MUL      | ``` x * y ``` | ``` x.mul(y) ```  | ``` mul(x, y) ```|
-| DIV      | ``` x / y ``` | ``` x.div(y) ```  | ``` div(x, y) ```|
-| FLOOR DIV| ``` x // y ```| ``` x.floordiv(y) ``` | ``` floordiv(x, y) ```|
-| NEG      | ``` ~ x ```   | ``` x.neg(y) ```  | ``` neg(x, y) ```|
-| POW      | ``` x ** y ```| ``` x.power(y) ```| ``` pow(x, y) ```|
+| Operation | Operator      | Method                | Function               |
+|:---------:|:-------------:|:---------------------:|:----------------------:|
+| ADD       | ``` x + y ``` | ``` x.add(y) ```      | ``` add(x, y) ```      |
+| SUB       | ``` x - y ``` | ``` x.sub(y) ```      | ``` sub(x, y) ```      |
+| MUL       | ``` x * y ``` | ``` x.mul(y) ```      | ``` mul(x, y) ```      |
+| DIV       | ``` x / y ``` | ``` x.div(y) ```      | ``` div(x, y) ```      |
+| FLOOR DIV | ``` x // y ```| ``` x.floordiv(y) ``` | ``` floordiv(x, y) ``` |
+| NEG       | ``` ~ x ```   | ``` x.neg(y) ```      | ``` neg(x, y) ```      |
+| POW       | ``` x ** y ```| ``` x.power(y) ```    | ``` pow(x, y) ```      |
 
 <sub>Arithmetic operators are recommended. The usage of methods or functions changes the precedence of the operation at execution as if it were enclosed in parentheses.</sub>
 
 ##### Covariance methods
 
 Methods *add*, *sub*, *mul*, *div*, *floordiv* allows the usage of the covariance as an additional parameter.
 
@@ -178,15 +177,14 @@
 w = x.add(y, covariance = 0.0)
 # w = ufloat(149.190, 4.218)
 z = x.add(y, covariance = 12.4)
 # z = ufloat(149.190, 6.526)
 ```
 
 *ufloat operators Code example:*
-
 ```python
 x = ufloat(925.69, 23.8)
 y = ufloat(536.50, 31.83)
 z = ufloat(-3404, 4.76)
 
 w = (x / y)**2 - z
 # w = ufloat(3406.977, 5.946)
@@ -214,17 +212,17 @@
 # y = uint(432, 5.7)
 ```
 
 #### Operators
 
 The operator MOD is included for uint. The rest of the operators available for uint are the same than those provided for ufloat: *ADD*, *SUB*, *MUL*, *DIV*, *FLOOR DIV*, *NEG*, *POWER*. 
 
-| Operation | Operator      | Method | Function |
-|:---------:|:------------:|:-----------------:|:----------------:|
-| MOD      | ``` x % y ``` | ``` x.mod(y) ```  | ``` mod(x, y) ```|
+| Operation | Operator      | Method            | Function         |
+|:---------:|:-------------:|:-----------------:|:----------------:|
+| MOD       | ``` x % y ``` | ``` x.mod(y) ```  | ``` mod(x, y) ```|
 
 <sub>Arithmetic operators are recommended. The usage of methods or functions changes the precedence of the operation at execution as if it were enclosed in parentheses.</sub>
 
 ##### Covariance methods
 
 Covariance methods are also provided for the uint type.
 
@@ -252,27 +250,26 @@
 
 --- 
 
 ## Comparison Operators
 Comparison between uint and ufloat can be made using the comparison operators: <, <=, >, >=, == and != and the methods.
 
 
-| Operation | Operator      | Method | Function |
-|:-----------:|:---------------:|:-------------------:|:-------------:|
-| Less      | ``` x < y ``` | ``` x.lt(y) ```  | ``` lt(x, y) ```|
-| Less or Equals | ``` x <= y ``` | ``` x.le(y) ```  | ``` le(x, y) ```|
-| Greater | ``` x > y ``` | ``` x.gt(y) ```  | ``` gt(x, y) ```|
+| Operation         | Operator       | Method           | Function        |
+|:-----------------:|:--------------:|:----------------:|:---------------:|
+| Less              | ``` x < y ```  | ``` x.lt(y) ```  | ``` lt(x, y) ```|
+| Less or Equals    | ``` x <= y ``` | ``` x.le(y) ```  | ``` le(x, y) ```|
+| Greater           | ``` x > y ```  | ``` x.gt(y) ```  | ``` gt(x, y) ```|
 | Greater or Equals | ``` x >= y ``` | ``` x.ge(y) ```  | ``` ge(x, y) ```|
-| Equals | ``` x == y ``` | ``` x.eq(y) ```  | ``` eq(x, y) ```|
-| Not Equals | ``` x != y ``` | ``` x.ne(y) ```  | ``` ne(x, y) ```|
+| Equals            | ``` x == y ``` | ``` x.eq(y) ```  | ``` eq(x, y) ```|
+| Not Equals        | ``` x != y ``` | ``` x.ne(y) ```  | ``` ne(x, y) ```|
 
 <sub>Operators are recommended. The usage of methods or functions changes the precedence of the operation at execution as if it were enclosed in parentheses.</sub>
 
 *ufloat Comparison Code example:*
-
 ```python
 x = uint(100, 0.7)
 y = ufloat(900.45, 0.6)
 
 if y > x:
     w = y - x # ufloat - uint
     # w = ufloat(800.450, 0.922)
@@ -281,43 +278,28 @@
 ---
 
 ## Math functions
 
 The library provides the following math functions for uint and ufloat types: 
 *sqrt*(), *sin*(), *cos*(), *tan*(), *atan*(), *acos*(), *asin*(), *inverse*(), *floor*(), *round*(), *max*(...), *min*(...)
 
-Example usage of max for uint and ufloat.
+*Example usage of max for uint and ufloat:*
 ```python
 m = max( 
     sin(ufloat(53.34, 0.8)),
     cos(uint(2, 0.6)),
     uint(23, 0.6), 
     floor(ufloat(3.4, 0.8)),
     uint(84, 0.6)
 )
 # m = uint(84, 0.600)
 ``` 
 
 ---
 
-## The abool type
-
----
-
-## The afloat type
-
----
-
-## The aint type
-
----
-## sbool
-
----
-
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `uncertainty-datatypes-1.0.7/README.md` & `uncertainty-datatypes-1.0.8/uncertainty_datatypes.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: uncertainty-datatypes
+Version: 1.0.8
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
@@ -59,29 +78,28 @@
 * Operator: ``` x & y ``` 
 * Special operator: ``` x |AND| y ``` 
 * The ubool method: ``` x.AND(y) ``` 
 * A function: ``` AND(x, y) ```
 
 The table below summarizes all the possible usages.
 
-| Operation  | Operator       | Special <br/> Operator   | Method                  | Function                 |
+| Operation  | Operator       | Special Operator         | Method                  | Function                 |
 |:----------:|:--------------:|:------------------------:|:-----------------------:|:------------------------:|
 | AND        | ``` x & y ```  | ``` x |AND| y ```        | ``` x.AND(y) ```        | ``` AND(x, y) ```        |
 | OR         | ``` x | y ```  | ``` x |OR| y ```         | ``` x.OR(y) ```         | ``` OR(x, y) ```         |
 | XOR        | ``` x ^ y ```  | ``` x |XOR| y ```        | ``` x.XOR(y) ```        | ``` XOR(x, y) ```        |
 | NOT        | ``` ~ x ```    |                          | ``` x.NOT() ```         | ``` NOT(x) ```           |
 | IMPLIES    | ``` x >> y ``` | ``` x |IMPLIES| y ```    | ``` x.IMPLIES(y) ```    | ``` IMPLIES(x, y) ```    |
 | EQUIVALENT | ``` x == y ``` | ``` x |EQUIVALENT| y ``` | ``` x.EQUIVALENT(y) ``` | ``` EQUIVALENT(x, y) ``` |
 | EQUALS     | ``` x == y ``` |  ``` x |EQUALS| y ```    | ``` x.EQUALS(y) ```     | ``` EQUALS(x, y) ```     |
 | DISTINCT   | ``` x != y ``` | ``` x |DISTINCT| y ```   | ``` x.DISTINCT(y) ```   | ``` DISTINCT(x, y) ```   |
 
 <sub> Operators or special operators must be surrounded by parentheses due operator precedence. Meanwhile, using a method or the function provides the highest precedence. </sub>
 
 *ubool Code example:*
-
 ```python
 x = ubool(0.3)
 y = ubool(0.8)
 z = ubool(0.5)
 
 w = (~x & y) |IMPLIES| (y ^ z)
 # w = ubool(0.608)
@@ -132,23 +150,23 @@
 # y = ufloat(233.0, 0.7)
 ```
 
 #### Operators
 
 ufloat operators include: *ADD*, *SUB*, *MUL*, *DIV*, *FLOOR DIV*, *NEG*, *POWER*. The table below summarizes all the possible operations.
 
-| Operation | Operator      | Method | Function |
-|:---------:|:------------:|:-----------------:|:----------------:|
-| ADD      | ``` x + y ``` | ``` x.add(y) ```  | ``` add(x, y) ```|
-| SUB      | ``` x - y ``` | ``` x.sub(y) ```  | ``` sub(x, y) ```|
-| MUL      | ``` x * y ``` | ``` x.mul(y) ```  | ``` mul(x, y) ```|
-| DIV      | ``` x / y ``` | ``` x.div(y) ```  | ``` div(x, y) ```|
-| FLOOR DIV| ``` x // y ```| ``` x.floordiv(y) ``` | ``` floordiv(x, y) ```|
-| NEG      | ``` ~ x ```   | ``` x.neg(y) ```  | ``` neg(x, y) ```|
-| POW      | ``` x ** y ```| ``` x.power(y) ```| ``` pow(x, y) ```|
+| Operation | Operator      | Method                | Function               |
+|:---------:|:-------------:|:---------------------:|:----------------------:|
+| ADD       | ``` x + y ``` | ``` x.add(y) ```      | ``` add(x, y) ```      |
+| SUB       | ``` x - y ``` | ``` x.sub(y) ```      | ``` sub(x, y) ```      |
+| MUL       | ``` x * y ``` | ``` x.mul(y) ```      | ``` mul(x, y) ```      |
+| DIV       | ``` x / y ``` | ``` x.div(y) ```      | ``` div(x, y) ```      |
+| FLOOR DIV | ``` x // y ```| ``` x.floordiv(y) ``` | ``` floordiv(x, y) ``` |
+| NEG       | ``` ~ x ```   | ``` x.neg(y) ```      | ``` neg(x, y) ```      |
+| POW       | ``` x ** y ```| ``` x.power(y) ```    | ``` pow(x, y) ```      |
 
 <sub>Arithmetic operators are recommended. The usage of methods or functions changes the precedence of the operation at execution as if it were enclosed in parentheses.</sub>
 
 ##### Covariance methods
 
 Methods *add*, *sub*, *mul*, *div*, *floordiv* allows the usage of the covariance as an additional parameter.
 
@@ -159,15 +177,14 @@
 w = x.add(y, covariance = 0.0)
 # w = ufloat(149.190, 4.218)
 z = x.add(y, covariance = 12.4)
 # z = ufloat(149.190, 6.526)
 ```
 
 *ufloat operators Code example:*
-
 ```python
 x = ufloat(925.69, 23.8)
 y = ufloat(536.50, 31.83)
 z = ufloat(-3404, 4.76)
 
 w = (x / y)**2 - z
 # w = ufloat(3406.977, 5.946)
@@ -195,17 +212,17 @@
 # y = uint(432, 5.7)
 ```
 
 #### Operators
 
 The operator MOD is included for uint. The rest of the operators available for uint are the same than those provided for ufloat: *ADD*, *SUB*, *MUL*, *DIV*, *FLOOR DIV*, *NEG*, *POWER*. 
 
-| Operation | Operator      | Method | Function |
-|:---------:|:------------:|:-----------------:|:----------------:|
-| MOD      | ``` x % y ``` | ``` x.mod(y) ```  | ``` mod(x, y) ```|
+| Operation | Operator      | Method            | Function         |
+|:---------:|:-------------:|:-----------------:|:----------------:|
+| MOD       | ``` x % y ``` | ``` x.mod(y) ```  | ``` mod(x, y) ```|
 
 <sub>Arithmetic operators are recommended. The usage of methods or functions changes the precedence of the operation at execution as if it were enclosed in parentheses.</sub>
 
 ##### Covariance methods
 
 Covariance methods are also provided for the uint type.
 
@@ -233,27 +250,26 @@
 
 --- 
 
 ## Comparison Operators
 Comparison between uint and ufloat can be made using the comparison operators: <, <=, >, >=, == and != and the methods.
 
 
-| Operation | Operator      | Method | Function |
-|:-----------:|:---------------:|:-------------------:|:-------------:|
-| Less      | ``` x < y ``` | ``` x.lt(y) ```  | ``` lt(x, y) ```|
-| Less or Equals | ``` x <= y ``` | ``` x.le(y) ```  | ``` le(x, y) ```|
-| Greater | ``` x > y ``` | ``` x.gt(y) ```  | ``` gt(x, y) ```|
+| Operation         | Operator       | Method           | Function        |
+|:-----------------:|:--------------:|:----------------:|:---------------:|
+| Less              | ``` x < y ```  | ``` x.lt(y) ```  | ``` lt(x, y) ```|
+| Less or Equals    | ``` x <= y ``` | ``` x.le(y) ```  | ``` le(x, y) ```|
+| Greater           | ``` x > y ```  | ``` x.gt(y) ```  | ``` gt(x, y) ```|
 | Greater or Equals | ``` x >= y ``` | ``` x.ge(y) ```  | ``` ge(x, y) ```|
-| Equals | ``` x == y ``` | ``` x.eq(y) ```  | ``` eq(x, y) ```|
-| Not Equals | ``` x != y ``` | ``` x.ne(y) ```  | ``` ne(x, y) ```|
+| Equals            | ``` x == y ``` | ``` x.eq(y) ```  | ``` eq(x, y) ```|
+| Not Equals        | ``` x != y ``` | ``` x.ne(y) ```  | ``` ne(x, y) ```|
 
 <sub>Operators are recommended. The usage of methods or functions changes the precedence of the operation at execution as if it were enclosed in parentheses.</sub>
 
 *ufloat Comparison Code example:*
-
 ```python
 x = uint(100, 0.7)
 y = ufloat(900.45, 0.6)
 
 if y > x:
     w = y - x # ufloat - uint
     # w = ufloat(800.450, 0.922)
@@ -262,43 +278,28 @@
 ---
 
 ## Math functions
 
 The library provides the following math functions for uint and ufloat types: 
 *sqrt*(), *sin*(), *cos*(), *tan*(), *atan*(), *acos*(), *asin*(), *inverse*(), *floor*(), *round*(), *max*(...), *min*(...)
 
-Example usage of max for uint and ufloat.
+*Example usage of max for uint and ufloat:*
 ```python
 m = max( 
     sin(ufloat(53.34, 0.8)),
     cos(uint(2, 0.6)),
     uint(23, 0.6), 
     floor(ufloat(3.4, 0.8)),
     uint(84, 0.6)
 )
 # m = uint(84, 0.600)
 ``` 
 
 ---
 
-## The abool type
-
----
-
-## The afloat type
-
----
-
-## The aint type
-
----
-## sbool
-
----
-
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `uncertainty-datatypes-1.0.7/pyproject.toml` & `uncertainty-datatypes-1.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "uncertainty-datatypes"
-version = "1.0.7"
+version = "1.0.8"
 authors = [
   { name="Atenea Research Group, University of Malaga, Spain" },
 ]
 description = "Uncertainty Datatypes Library"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers=[
```

### Comparing `uncertainty-datatypes-1.0.7/test/test_ubool.py` & `uncertainty-datatypes-1.0.8/test/test_ubool.py`

 * *Files identical despite different names*

### Comparing `uncertainty-datatypes-1.0.7/test/test_ufloat.py` & `uncertainty-datatypes-1.0.8/test/test_ufloat.py`

 * *Files identical despite different names*

### Comparing `uncertainty-datatypes-1.0.7/test/test_uint.py` & `uncertainty-datatypes-1.0.8/test/test_uint.py`

 * *Files identical despite different names*

### Comparing `uncertainty-datatypes-1.0.7/uncertainty/ubool.py` & `uncertainty-datatypes-1.0.8/uncertainty/ubool.py`

 * *Files identical despite different names*

### Comparing `uncertainty-datatypes-1.0.7/uncertainty/unumbers.py` & `uncertainty-datatypes-1.0.8/uncertainty/unumbers.py`

 * *Files identical despite different names*

### Comparing `uncertainty-datatypes-1.0.7/uncertainty/utypes.py` & `uncertainty-datatypes-1.0.8/uncertainty/utypes.py`

 * *Files identical despite different names*

### Comparing `uncertainty-datatypes-1.0.7/uncertainty_datatypes.egg-info/PKG-INFO` & `uncertainty-datatypes-1.0.8/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: uncertainty-datatypes
-Version: 1.0.7
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
@@ -78,29 +59,28 @@
 * Operator: ``` x & y ``` 
 * Special operator: ``` x |AND| y ``` 
 * The ubool method: ``` x.AND(y) ``` 
 * A function: ``` AND(x, y) ```
 
 The table below summarizes all the possible usages.
 
-| Operation  | Operator       | Special <br/> Operator   | Method                  | Function                 |
+| Operation  | Operator       | Special Operator         | Method                  | Function                 |
 |:----------:|:--------------:|:------------------------:|:-----------------------:|:------------------------:|
 | AND        | ``` x & y ```  | ``` x |AND| y ```        | ``` x.AND(y) ```        | ``` AND(x, y) ```        |
 | OR         | ``` x | y ```  | ``` x |OR| y ```         | ``` x.OR(y) ```         | ``` OR(x, y) ```         |
 | XOR        | ``` x ^ y ```  | ``` x |XOR| y ```        | ``` x.XOR(y) ```        | ``` XOR(x, y) ```        |
 | NOT        | ``` ~ x ```    |                          | ``` x.NOT() ```         | ``` NOT(x) ```           |
 | IMPLIES    | ``` x >> y ``` | ``` x |IMPLIES| y ```    | ``` x.IMPLIES(y) ```    | ``` IMPLIES(x, y) ```    |
 | EQUIVALENT | ``` x == y ``` | ``` x |EQUIVALENT| y ``` | ``` x.EQUIVALENT(y) ``` | ``` EQUIVALENT(x, y) ``` |
 | EQUALS     | ``` x == y ``` |  ``` x |EQUALS| y ```    | ``` x.EQUALS(y) ```     | ``` EQUALS(x, y) ```     |
 | DISTINCT   | ``` x != y ``` | ``` x |DISTINCT| y ```   | ``` x.DISTINCT(y) ```   | ``` DISTINCT(x, y) ```   |
 
 <sub> Operators or special operators must be surrounded by parentheses due operator precedence. Meanwhile, using a method or the function provides the highest precedence. </sub>
 
 *ubool Code example:*
-
 ```python
 x = ubool(0.3)
 y = ubool(0.8)
 z = ubool(0.5)
 
 w = (~x & y) |IMPLIES| (y ^ z)
 # w = ubool(0.608)
@@ -151,23 +131,23 @@
 # y = ufloat(233.0, 0.7)
 ```
 
 #### Operators
 
 ufloat operators include: *ADD*, *SUB*, *MUL*, *DIV*, *FLOOR DIV*, *NEG*, *POWER*. The table below summarizes all the possible operations.
 
-| Operation | Operator      | Method | Function |
-|:---------:|:------------:|:-----------------:|:----------------:|
-| ADD      | ``` x + y ``` | ``` x.add(y) ```  | ``` add(x, y) ```|
-| SUB      | ``` x - y ``` | ``` x.sub(y) ```  | ``` sub(x, y) ```|
-| MUL      | ``` x * y ``` | ``` x.mul(y) ```  | ``` mul(x, y) ```|
-| DIV      | ``` x / y ``` | ``` x.div(y) ```  | ``` div(x, y) ```|
-| FLOOR DIV| ``` x // y ```| ``` x.floordiv(y) ``` | ``` floordiv(x, y) ```|
-| NEG      | ``` ~ x ```   | ``` x.neg(y) ```  | ``` neg(x, y) ```|
-| POW      | ``` x ** y ```| ``` x.power(y) ```| ``` pow(x, y) ```|
+| Operation | Operator      | Method                | Function               |
+|:---------:|:-------------:|:---------------------:|:----------------------:|
+| ADD       | ``` x + y ``` | ``` x.add(y) ```      | ``` add(x, y) ```      |
+| SUB       | ``` x - y ``` | ``` x.sub(y) ```      | ``` sub(x, y) ```      |
+| MUL       | ``` x * y ``` | ``` x.mul(y) ```      | ``` mul(x, y) ```      |
+| DIV       | ``` x / y ``` | ``` x.div(y) ```      | ``` div(x, y) ```      |
+| FLOOR DIV | ``` x // y ```| ``` x.floordiv(y) ``` | ``` floordiv(x, y) ``` |
+| NEG       | ``` ~ x ```   | ``` x.neg(y) ```      | ``` neg(x, y) ```      |
+| POW       | ``` x ** y ```| ``` x.power(y) ```    | ``` pow(x, y) ```      |
 
 <sub>Arithmetic operators are recommended. The usage of methods or functions changes the precedence of the operation at execution as if it were enclosed in parentheses.</sub>
 
 ##### Covariance methods
 
 Methods *add*, *sub*, *mul*, *div*, *floordiv* allows the usage of the covariance as an additional parameter.
 
@@ -178,15 +158,14 @@
 w = x.add(y, covariance = 0.0)
 # w = ufloat(149.190, 4.218)
 z = x.add(y, covariance = 12.4)
 # z = ufloat(149.190, 6.526)
 ```
 
 *ufloat operators Code example:*
-
 ```python
 x = ufloat(925.69, 23.8)
 y = ufloat(536.50, 31.83)
 z = ufloat(-3404, 4.76)
 
 w = (x / y)**2 - z
 # w = ufloat(3406.977, 5.946)
@@ -214,17 +193,17 @@
 # y = uint(432, 5.7)
 ```
 
 #### Operators
 
 The operator MOD is included for uint. The rest of the operators available for uint are the same than those provided for ufloat: *ADD*, *SUB*, *MUL*, *DIV*, *FLOOR DIV*, *NEG*, *POWER*. 
 
-| Operation | Operator      | Method | Function |
-|:---------:|:------------:|:-----------------:|:----------------:|
-| MOD      | ``` x % y ``` | ``` x.mod(y) ```  | ``` mod(x, y) ```|
+| Operation | Operator      | Method            | Function         |
+|:---------:|:-------------:|:-----------------:|:----------------:|
+| MOD       | ``` x % y ``` | ``` x.mod(y) ```  | ``` mod(x, y) ```|
 
 <sub>Arithmetic operators are recommended. The usage of methods or functions changes the precedence of the operation at execution as if it were enclosed in parentheses.</sub>
 
 ##### Covariance methods
 
 Covariance methods are also provided for the uint type.
 
@@ -252,27 +231,26 @@
 
 --- 
 
 ## Comparison Operators
 Comparison between uint and ufloat can be made using the comparison operators: <, <=, >, >=, == and != and the methods.
 
 
-| Operation | Operator      | Method | Function |
-|:-----------:|:---------------:|:-------------------:|:-------------:|
-| Less      | ``` x < y ``` | ``` x.lt(y) ```  | ``` lt(x, y) ```|
-| Less or Equals | ``` x <= y ``` | ``` x.le(y) ```  | ``` le(x, y) ```|
-| Greater | ``` x > y ``` | ``` x.gt(y) ```  | ``` gt(x, y) ```|
+| Operation         | Operator       | Method           | Function        |
+|:-----------------:|:--------------:|:----------------:|:---------------:|
+| Less              | ``` x < y ```  | ``` x.lt(y) ```  | ``` lt(x, y) ```|
+| Less or Equals    | ``` x <= y ``` | ``` x.le(y) ```  | ``` le(x, y) ```|
+| Greater           | ``` x > y ```  | ``` x.gt(y) ```  | ``` gt(x, y) ```|
 | Greater or Equals | ``` x >= y ``` | ``` x.ge(y) ```  | ``` ge(x, y) ```|
-| Equals | ``` x == y ``` | ``` x.eq(y) ```  | ``` eq(x, y) ```|
-| Not Equals | ``` x != y ``` | ``` x.ne(y) ```  | ``` ne(x, y) ```|
+| Equals            | ``` x == y ``` | ``` x.eq(y) ```  | ``` eq(x, y) ```|
+| Not Equals        | ``` x != y ``` | ``` x.ne(y) ```  | ``` ne(x, y) ```|
 
 <sub>Operators are recommended. The usage of methods or functions changes the precedence of the operation at execution as if it were enclosed in parentheses.</sub>
 
 *ufloat Comparison Code example:*
-
 ```python
 x = uint(100, 0.7)
 y = ufloat(900.45, 0.6)
 
 if y > x:
     w = y - x # ufloat - uint
     # w = ufloat(800.450, 0.922)
@@ -281,43 +259,28 @@
 ---
 
 ## Math functions
 
 The library provides the following math functions for uint and ufloat types: 
 *sqrt*(), *sin*(), *cos*(), *tan*(), *atan*(), *acos*(), *asin*(), *inverse*(), *floor*(), *round*(), *max*(...), *min*(...)
 
-Example usage of max for uint and ufloat.
+*Example usage of max for uint and ufloat:*
 ```python
 m = max( 
     sin(ufloat(53.34, 0.8)),
     cos(uint(2, 0.6)),
     uint(23, 0.6), 
     floor(ufloat(3.4, 0.8)),
     uint(84, 0.6)
 )
 # m = uint(84, 0.600)
 ``` 
 
 ---
 
-## The abool type
-
----
-
-## The afloat type
-
----
-
-## The aint type
-
----
-## sbool
-
----
-
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
```

