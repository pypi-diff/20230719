# Comparing `tmp/pyISBO-1.0.3.tar.gz` & `tmp/pyISBO-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyISBO-1.0.3.tar", last modified: Thu Jul 13 08:48:23 2023, max compression
+gzip compressed data, was "dist\pyISBO-1.0.4.tar", last modified: Wed Jul 19 02:05:13 2023, max compression
```

## Comparing `pyISBO-1.0.3.tar` & `pyISBO-1.0.4.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 08:48:23.000000 pyISBO-1.0.3/
--rw-rw-rw-   0        0        0      304 2023-07-13 08:48:23.000000 pyISBO-1.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-13 08:48:23.000000 pyISBO-1.0.3/pyISBO/
-drwxrwxrwx   0        0        0        0 2023-07-13 08:48:23.000000 pyISBO-1.0.3/pyISBO/SBO_grb/
--rw-rw-rw-   0        0        0     5130 2023-07-13 08:37:17.000000 pyISBO-1.0.3/pyISBO/SBO_grb/AutoRegression.py
--rw-rw-rw-   0        0        0     7086 2023-07-13 01:54:16.000000 pyISBO-1.0.3/pyISBO/SBO_grb/DecisionTree.py
--rw-rw-rw-   0        0        0     4126 2023-07-13 01:54:17.000000 pyISBO-1.0.3/pyISBO/SBO_grb/LinearRegression.py
--rw-rw-rw-   0        0        0     5362 2023-07-13 01:54:17.000000 pyISBO-1.0.3/pyISBO/SBO_grb/LogisticRegression.py
--rw-rw-rw-   0        0        0     7019 2023-07-13 02:10:21.000000 pyISBO-1.0.3/pyISBO/SBO_grb/NeuralNetwork.py
--rw-rw-rw-   0        0        0     4496 2023-07-13 01:54:17.000000 pyISBO-1.0.3/pyISBO/SBO_grb/QuadraticRegression.py
--rw-rw-rw-   0        0        0     6895 2023-07-13 01:54:17.000000 pyISBO-1.0.3/pyISBO/SBO_grb/RandomForest.py
--rw-rw-rw-   0        0        0     6548 2023-07-13 01:57:32.000000 pyISBO-1.0.3/pyISBO/SBO_grb/RegressionSplines.py
--rw-rw-rw-   0        0        0        0 2023-04-03 12:01:13.000000 pyISBO-1.0.3/pyISBO/SBO_grb/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 08:48:23.000000 pyISBO-1.0.3/pyISBO/SBO_pulp/
--rw-rw-rw-   0        0        0     4766 2023-07-13 08:39:23.000000 pyISBO-1.0.3/pyISBO/SBO_pulp/AutoRegression.py
--rw-rw-rw-   0        0        0     7072 2023-07-13 07:59:54.000000 pyISBO-1.0.3/pyISBO/SBO_pulp/DecisionTree.py
--rw-rw-rw-   0        0        0     4584 2023-07-13 08:15:08.000000 pyISBO-1.0.3/pyISBO/SBO_pulp/LinearRegression.py
--rw-rw-rw-   0        0        0     5897 2023-07-13 08:15:08.000000 pyISBO-1.0.3/pyISBO/SBO_pulp/LogisticRegression.py
--rw-rw-rw-   0        0        0     7581 2023-07-13 08:21:24.000000 pyISBO-1.0.3/pyISBO/SBO_pulp/NeuralNetwork.py
--rw-rw-rw-   0        0        0     7854 2023-07-13 08:25:59.000000 pyISBO-1.0.3/pyISBO/SBO_pulp/RandomForest.py
--rw-rw-rw-   0        0        0     6982 2023-07-13 08:15:08.000000 pyISBO-1.0.3/pyISBO/SBO_pulp/RegressionSplines.py
--rw-rw-rw-   0        0        0        0 2023-04-03 12:01:13.000000 pyISBO-1.0.3/pyISBO/SBO_pulp/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-03 12:01:13.000000 pyISBO-1.0.3/pyISBO/__init__.py
--rw-rw-rw-   0        0        0      324 2023-07-13 08:35:34.000000 pyISBO-1.0.3/pyISBO/main.py
-drwxrwxrwx   0        0        0        0 2023-07-13 08:48:23.000000 pyISBO-1.0.3/pyISBO.egg-info/
--rw-rw-rw-   0        0        0      304 2023-07-13 08:48:23.000000 pyISBO-1.0.3/pyISBO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      732 2023-07-13 08:48:23.000000 pyISBO-1.0.3/pyISBO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 08:48:23.000000 pyISBO-1.0.3/pyISBO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-13 08:48:23.000000 pyISBO-1.0.3/pyISBO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-13 08:48:23.000000 pyISBO-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      736 2023-07-13 08:47:55.000000 pyISBO-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 02:05:13.000000 pyISBO-1.0.4/
+-rw-rw-rw-   0        0        0      304 2023-07-19 02:05:13.000000 pyISBO-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6627 2023-07-19 02:02:39.000000 pyISBO-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-19 02:05:13.000000 pyISBO-1.0.4/pyISBO/
+drwxrwxrwx   0        0        0        0 2023-07-19 02:05:13.000000 pyISBO-1.0.4/pyISBO/SBO_grb/
+-rw-rw-rw-   0        0        0     5130 2023-07-13 08:37:17.000000 pyISBO-1.0.4/pyISBO/SBO_grb/AutoRegression.py
+-rw-rw-rw-   0        0        0     7086 2023-07-13 01:54:16.000000 pyISBO-1.0.4/pyISBO/SBO_grb/DecisionTree.py
+-rw-rw-rw-   0        0        0     4126 2023-07-13 01:54:17.000000 pyISBO-1.0.4/pyISBO/SBO_grb/LinearRegression.py
+-rw-rw-rw-   0        0        0     5362 2023-07-13 01:54:17.000000 pyISBO-1.0.4/pyISBO/SBO_grb/LogisticRegression.py
+-rw-rw-rw-   0        0        0     7019 2023-07-13 02:10:21.000000 pyISBO-1.0.4/pyISBO/SBO_grb/NeuralNetwork.py
+-rw-rw-rw-   0        0        0     4496 2023-07-13 01:54:17.000000 pyISBO-1.0.4/pyISBO/SBO_grb/QuadraticRegression.py
+-rw-rw-rw-   0        0        0     6895 2023-07-13 01:54:17.000000 pyISBO-1.0.4/pyISBO/SBO_grb/RandomForest.py
+-rw-rw-rw-   0        0        0     6548 2023-07-13 01:57:32.000000 pyISBO-1.0.4/pyISBO/SBO_grb/RegressionSplines.py
+-rw-rw-rw-   0        0        0        0 2023-04-03 12:01:13.000000 pyISBO-1.0.4/pyISBO/SBO_grb/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 02:05:13.000000 pyISBO-1.0.4/pyISBO/SBO_pulp/
+-rw-rw-rw-   0        0        0     4766 2023-07-13 08:39:23.000000 pyISBO-1.0.4/pyISBO/SBO_pulp/AutoRegression.py
+-rw-rw-rw-   0        0        0     6602 2023-07-15 09:21:53.000000 pyISBO-1.0.4/pyISBO/SBO_pulp/DecisionTree.py
+-rw-rw-rw-   0        0        0     3876 2023-07-14 13:58:57.000000 pyISBO-1.0.4/pyISBO/SBO_pulp/LinearRegression.py
+-rw-rw-rw-   0        0        0     5171 2023-07-15 09:21:53.000000 pyISBO-1.0.4/pyISBO/SBO_pulp/LogisticRegression.py
+-rw-rw-rw-   0        0        0     6819 2023-07-15 09:21:53.000000 pyISBO-1.0.4/pyISBO/SBO_pulp/NeuralNetwork.py
+-rw-rw-rw-   0        0        0     7416 2023-07-15 09:13:40.000000 pyISBO-1.0.4/pyISBO/SBO_pulp/RandomForest.py
+-rw-rw-rw-   0        0        0     6436 2023-07-15 09:21:53.000000 pyISBO-1.0.4/pyISBO/SBO_pulp/RegressionSplines.py
+-rw-rw-rw-   0        0        0        0 2023-04-03 12:01:13.000000 pyISBO-1.0.4/pyISBO/SBO_pulp/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-04-03 12:01:13.000000 pyISBO-1.0.4/pyISBO/__init__.py
+-rw-rw-rw-   0        0        0      514 2023-07-14 13:30:01.000000 pyISBO-1.0.4/pyISBO/main.py
+drwxrwxrwx   0        0        0        0 2023-07-19 02:05:13.000000 pyISBO-1.0.4/pyISBO.egg-info/
+-rw-rw-rw-   0        0        0      304 2023-07-19 02:05:13.000000 pyISBO-1.0.4/pyISBO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      742 2023-07-19 02:05:13.000000 pyISBO-1.0.4/pyISBO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 02:05:13.000000 pyISBO-1.0.4/pyISBO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-19 02:05:13.000000 pyISBO-1.0.4/pyISBO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-19 02:05:13.000000 pyISBO-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      736 2023-07-19 02:04:50.000000 pyISBO-1.0.4/setup.py
```

### Comparing `pyISBO-1.0.3/pyISBO/SBO_grb/AutoRegression.py` & `pyISBO-1.0.4/pyISBO/SBO_grb/AutoRegression.py`

 * *Files identical despite different names*

### Comparing `pyISBO-1.0.3/pyISBO/SBO_grb/DecisionTree.py` & `pyISBO-1.0.4/pyISBO/SBO_grb/DecisionTree.py`

 * *Files identical despite different names*

### Comparing `pyISBO-1.0.3/pyISBO/SBO_grb/LinearRegression.py` & `pyISBO-1.0.4/pyISBO/SBO_grb/LinearRegression.py`

 * *Files identical despite different names*

### Comparing `pyISBO-1.0.3/pyISBO/SBO_grb/LogisticRegression.py` & `pyISBO-1.0.4/pyISBO/SBO_grb/LogisticRegression.py`

 * *Files identical despite different names*

### Comparing `pyISBO-1.0.3/pyISBO/SBO_grb/NeuralNetwork.py` & `pyISBO-1.0.4/pyISBO/SBO_grb/NeuralNetwork.py`

 * *Files identical despite different names*

### Comparing `pyISBO-1.0.3/pyISBO/SBO_grb/QuadraticRegression.py` & `pyISBO-1.0.4/pyISBO/SBO_grb/QuadraticRegression.py`

 * *Files identical despite different names*

### Comparing `pyISBO-1.0.3/pyISBO/SBO_grb/RandomForest.py` & `pyISBO-1.0.4/pyISBO/SBO_grb/RandomForest.py`

 * *Files identical despite different names*

### Comparing `pyISBO-1.0.3/pyISBO/SBO_grb/RegressionSplines.py` & `pyISBO-1.0.4/pyISBO/SBO_grb/RegressionSplines.py`

 * *Files identical despite different names*

### Comparing `pyISBO-1.0.3/pyISBO/SBO_pulp/AutoRegression.py` & `pyISBO-1.0.4/pyISBO/SBO_pulp/AutoRegression.py`

 * *Files identical despite different names*

### Comparing `pyISBO-1.0.3/pyISBO/SBO_pulp/DecisionTree.py` & `pyISBO-1.0.4/pyISBO/SBO_pulp/DecisionTree.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 from pulp import *
 import numpy as np
 from sklearn.tree import DecisionTreeRegressor
 from sklearn.model_selection import cross_val_score
-import random
 
 
 def local_section_generator(bounds):
-    '''
+    """
     Transform the structure of bounds for later algorithm implementation.
-    '''
-    max = []
-    min = []
+    """
+    Upper = []
+    Lower = []
     for i in range(len(bounds)):
-        max.append(bounds[i][1])
-        min.append(bounds[i][0])
+        Upper.append(bounds[i][1])
+        Lower.append(bounds[i][0])
     return [min, max]
 
 
 def find_leaves(node_id, tree_):
-    '''
+    """
     return all leaves of a specific node in list form.
-    '''
+    """
     if tree_.children_left[node_id] == -1:
         return [node_id]
     else:
         return find_leaves(tree_.children_left[node_id], tree_) + find_leaves(tree_.children_right[node_id], tree_)
 
 
 class DT:
@@ -106,15 +105,15 @@
         '''
         Adding variables:
             Each input parameter corresponds to a variable (x_variable).
             Each leaf node corresponds to a binary variable (y_variable).
         '''
         for i in range(x_len):
             x_variable[i] = LpVariable('x_{}'.format(i), lowBound=local_section[0][i], upBound=local_section[1][i],
-                                          cat=self.types[i])
+                                       cat=self.types[i])
 
         y_variable = LpVariable.dict('y', range(len(leaves_num)), cat=LpBinary)
 
         '''
         Setting a dictionary: with the effect of finding the corresponding decision
         variable by the index of the leaf node.
         '''
@@ -137,43 +136,32 @@
         # Note that since pulp does not allow large numbers with high
         # precision, float(inf) is not allowed.
         M = 10000
         for i in range(tree_.node_count):
             if tree_.children_left[i] != -1:
                 cons_leaves_1 = find_leaves(tree_.children_left[i], tree_)
                 MIP += M * (lpSum(y_dict[j] for j in cons_leaves_1) - 1) - (
-                    tree_.threshold[i] - x_variable[tree_.feature[i]]) <= 0
+                        tree_.threshold[i] - x_variable[tree_.feature[i]]) <= 0,
+                "node_{}_left".format(i)
                 cons_leaves_2 = find_leaves(tree_.children_right[i], tree_)
                 MIP += M * (lpSum(y_dict[j] for j in cons_leaves_2) - 1) + (
-                    tree_.threshold[i] - x_variable[
-                        tree_.feature[i]]) + 1 / M <= 0
-        MIP += lpSum(y_variable[i] for i in range(len(y_variable))) == 1
-
+                        tree_.threshold[i] - x_variable[
+                    tree_.feature[i]]) + 1 / M <= 0,
+                "node_{}_right".format(i)
+        MIP += lpSum(y_variable[i] for i in range(len(y_variable))) == 1, "leaf"
+        for i in range(x_len):
+            MIP += x_variable[i] >= local_section[0][i], "x_{}_lb".format(i)
+            MIP += x_variable[i] <= local_section[1][i], "x_{}_ub".format(i)
         self.MIP = MIP
 
     def optimize(self):
         """
         solve the Pulp mix integer program
         :return: None.
         """
         if self.MIP is None:
             self.MIP_transform()
 
-        local_section = local_section_generator(self.bounds)
-        MIP = self.MIP
-        MIP.solve()
-        solved_variables = {}
-        for v in MIP.variables():
-            solved_variables[v.name] = v.varValue
-        solved_variables_dict = {}
-        for i in range(len(self.types)):
-            try:
-                solved_variables_dict['x_{}'.format(i)] = solved_variables['x_{}'.format(i)]
-            except:
-                solved_variables_dict['x_{}'.format(i)] = random.uniform(local_section[0][i], local_section[1][i])
-                if self.types[i] == LpInteger:
-                    solved_variables_dict['x_{}'.format(i)] = int(solved_variables_dict['x_{}'.format(i)] + 0.5)
-        optimizedParameter = []
-        for i in solved_variables_dict:
-            optimizedParameter.append(solved_variables_dict[i])
-        self.output = value(MIP.objective)
-        self.optimizedParameter = optimizedParameter
+        self.MIP.solve()
+        self.output = value(self.MIP.objective)
+        self.optimizedParameter = \
+            [self.MIP.variablesDict()["x_%d" % i].varValue for i in range(len(self.types))]
```

### Comparing `pyISBO-1.0.3/pyISBO/SBO_pulp/LinearRegression.py` & `pyISBO-1.0.4/pyISBO/SBO_pulp/LinearRegression.py`

 * *Files 15% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         Transform the surrogate into a pulp linear program
         :return: None.
             You can access the transformed linear model by MIP object.
         """
         assert self.model is not None, "You haven't build a surrogate yet. Try using fit() to create one."
 
         n = len(self.types)
-        self.MIP = LpProblem("神经网络优化", LpMinimize)
+        self.MIP = LpProblem("LinearRegression", LpMinimize)
 
         x = {}
         for i in range(len(self.types)):
             x[i] = LpVariable("x_%d" % i, self.bounds[i][0], self.bounds[i][1], cat=self.types[i])
         y = LpVariable("y")
 
         self.MIP += y
@@ -85,24 +85,9 @@
         Optimize over the MIP
         :return: None.
             You can get the optimized value and the optimized parameters by "output" and  "optimizedParameter" object.
         """
         if self.MIP is None:
             self.MIP_transform()
         self.MIP.solve()
-        result = []
-        solved_variables = {}
-        solved_variables_dict = {}
-        for v in self.MIP.variables():
-            solved_variables[v.name] = v.varValue
-        for i in range(len(self.types)):
-            try:
-                solved_variables_dict['x_{}'.format(i)] = solved_variables['x_{}'.format(i)]
-            except:
-                solved_variables_dict['x_{}'.format(i)] = random.uniform(self.bounds[i][0], self.bounds[i][1])
-                if self.types[i] == LpInteger:
-                    solved_variables_dict['x_{}'.format(i)] = int(solved_variables_dict['x_{}'.format(i)] + 0.5)
-        optimizedParameter = []
-        for i in solved_variables_dict:
-            optimizedParameter.append(solved_variables_dict[i])
-        self.optimizedParameter = optimizedParameter
+        self.optimizedParameter = [self.MIP.variablesDict()["x_%d" % i].varValue for i in range(len(self.types))]
         self.output = value(self.MIP.objective)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyISBO-1.0.3/pyISBO/SBO_pulp/LogisticRegression.py` & `pyISBO-1.0.4/pyISBO/SBO_pulp/LogisticRegression.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import random
 import numpy as np
 from sklearn.linear_model import LogisticRegression
 from sklearn.model_selection import cross_val_score
 from pulp import *
 
 
 class LogR:
@@ -78,24 +77,24 @@
         n = len(self.types)
         x = {}
         for i in range(len(self.types)):
             x[i] = LpVariable("x_%d" % i, self.bounds[i][0], self.bounds[i][1], cat=self.types[i])
         y = LpVariable("y")
         k = {}
         for i in range(len(self.model.classes_)):
-            k[i] = LpVariable("k_%d"%i, cat=LpBinary)
+            k[i] = LpVariable("k_%d" % i, cat=LpBinary)
 
         self.MIP += y
         self.MIP += y == lpSum(k[i] * float(self.model.classes_[i])
-                                          for i in range(len(self.model.classes_))), "objective"
+                               for i in range(len(self.model.classes_))), "objective"
         self.MIP += lpSum(k[i] for i in range(len(self.model.classes_))) == 1, "integrity"
         M = 1e5
 
         if len(self.model.classes_) == 2:
-            self.MIP += M*k[1] >= lpSum(self.model.coef_[0][i] * x[i] for i in range(n)) + self.model.intercept_, "k1"
+            self.MIP += M * k[1] >= lpSum(self.model.coef_[0][i] * x[i] for i in range(n)) + self.model.intercept_, "k1"
             self.MIP += M * (1 - k[0]) >= -lpSum(
                 self.model.coef_[0][i] * x[i] for i in range(n)) - self.model.intercept_, "k0"
         else:
             for l in range(len(self.model.classes_)):
                 for j in range(len(self.model.classes_)):
                     if l != j:
                         self.MIP += M * (1 - k[j]) >= lpSum(
@@ -108,24 +107,9 @@
         Optimize over the MIP
         :return: None.
             You can get the optimized value and the optimized parameters by "output" and  "optimizedParameter" object.
         """
         if self.MIP is None:
             self.MIP_transform()
         self.MIP.solve()
-        result = []
-        solved_variables = {}
-        solved_variables_dict = {}
-        for v in self.MIP.variables():
-            solved_variables[v.name] = v.varValue
-        for i in range(len(self.types)):
-            try:
-                solved_variables_dict['x_{}'.format(i)] = solved_variables['x_{}'.format(i)]
-            except:
-                solved_variables_dict['x_{}'.format(i)] = random.uniform(self.bounds[i][0], self.bounds[i][1])
-                if self.types[i] == LpInteger:
-                    solved_variables_dict['x_{}'.format(i)] = int(solved_variables_dict['x_{}'.format(i)] + 0.5)
-        optimizedParameter = []
-        for i in solved_variables_dict:
-            optimizedParameter.append(solved_variables_dict[i])
-        self.optimizedParameter = optimizedParameter
-        self.output = value(self.MIP.objective)
+        self.optimizedParameter = [self.MIP.variablesDict()["x_%d" % i].varValue for i in range(len(self.types))]
+        self.output = value(self.MIP.objective)
```

### Comparing `pyISBO-1.0.3/pyISBO/SBO_pulp/NeuralNetwork.py` & `pyISBO-1.0.4/pyISBO/SBO_pulp/NeuralNetwork.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from sklearn.metrics import get_scorer
 import tensorflow as tf
 from tensorflow import keras
 from sklearn.model_selection import KFold
 from tensorflow.keras import layers
 from pulp import *
-import random
 
 
 
 class NN:
     """
     Neural Network. Based on tensorflow2.0.
     """
@@ -38,15 +37,16 @@
             self.bounds.append((parameterInfo["lb"][i], parameterInfo["ub"][i]))
         self.types = list(parameterInfo.pop("type"))
         self.types = [LpContinuous if self.types[i] == "Continuous" else LpInteger for i in range(len(self.types))]
 
     def norm(self, x):
         return (x - self.mean) / self.std
 
-    def __create_model(self, k, n):
+    def __create_model(self, k):
+        n = len(self.types)
         model = keras.Sequential()
         model.add(layers.Dense(n, activation='relu', input_shape=[n]))
         for i in range(1, k - 1):
             model.add(layers.Dense(n, activation='relu'))
         model.add(layers.Dense(1))
         optimizer = tf.keras.optimizers.RMSprop(0.001)
         model.compile(loss="mse", optimizer=optimizer, metrics=['mae', 'mse'])
@@ -59,34 +59,33 @@
             Training data.
         :param y:array-like of shape (n_samples,) or (n_samples, n_targets)
             Target values. Will be cast to X's dtype if necessary.
         :return: A float number.
             The cross-validation score of the fitted model based on the scoring metric you choose.
         """
         print("Now fitting neural network.")
-        n = len(self.types)
         stats = X.describe().transpose()
         self.mean = stats['mean']
         self.std = stats['std']
         normed_X = self.norm(X)
         scorer = get_scorer(self.scoring)
         Scores = []
         for K in range(2, 7):
             score = 0
             kfold = KFold(5, shuffle=True)
             for train_index, test_index in kfold.split(X):
                 X_train, X_test = X.iloc[train_index], X.iloc[test_index]
                 y_train, y_test = y.iloc[train_index], y.iloc[test_index]
-                model = self.__create_model(K, n)
+                model = self.__create_model(K)
                 model.fit(X_train, y_train, epochs=100, verbose=None)
                 score += scorer(model, X_test, y_test)
             Scores.append(score/5)
 
         k = Scores.index(max(Scores)) + 2
-        self.model = self.__create_model(k, n)
+        self.model = self.__create_model(k)
         self.model.fit(normed_X, y)
         return max(Scores)
 
     def predict(self, X):
         """
         Predict using the surrogate.
         :param X:{array-like, sparse matrix} of shape (n_samples, n_features)T
@@ -113,25 +112,25 @@
         weights = self.model.get_weights()
         w = []
         b = []
         for k in range(K):
             w.append(weights[2 * k])
             b.append(weights[2 * k + 1])
 
-        lpmodel = LpProblem("神经网络优化", LpMinimize)
+        lpmodel = LpProblem("NeuralNetwork", LpMinimize)
         neuron_index = []
         for i in range(input_dim):
             neuron_index.append((0, i))
         for k in range(K):
             for i in range(nk[k]):
                 neuron_index.append((k + 1, i))
 
-        x_input = {}
+        x = {}
         for i in range(len(self.types)):
-            x_input[i] = LpVariable("x_input_%d" % i, self.bounds[i][0], self.bounds[i][1], cat=self.types[i])
+            x[i] = LpVariable("x_%d" % i, self.bounds[i][0], self.bounds[i][1], cat=self.types[i])
 
         neuron = {}
         for t in neuron_index:
             neuron[t] = LpVariable("neuron_%d_%d" % t, 0, cat=LpContinuous)
 
         s_ki = {}
         for t in neuron_index:
@@ -139,18 +138,18 @@
 
         z_ki = {}
         for t in neuron_index:
             z_ki[t] = LpVariable("z_ki_%d_%d" % t, 0, cat=LpBinary)
 
         M = 1e5
 
-        lpmodel += neuron[(K, 0)], "输出结果"
+        lpmodel += neuron[(K, 0)], "objective"
 
         for i in range(input_dim):
-            lpmodel += x_input[i] - self.mean[i] == self.std[i] * neuron[0, i], "firstLayer_" + str(i)
+            lpmodel += x[i] - self.mean[i] == self.std[i] * neuron[0, i], "firstLayer_" + str(i)
         for k in range(1, K + 1):
             for j in range(nk[k - 1]):
                 lpmodel += lpSum(neuron[k - 1, i] * w[k - 1][i, j] for i in range(w[k - 1].shape[0])) \
                            + b[k - 1][j] - neuron[k, j] + s_ki[k, j] == 0, "neuronTransmit_" + str(k) + "_" + str(j)
         for k in range(1, K + 1):
             for i in range(nk[k - 1]):
                 lpmodel += z_ki[k, i] * M + neuron[k, i] <= M, "ReLUx" + str(k) + "_" + str(i)
@@ -165,24 +164,9 @@
         Optimize over the MIP
         :return: None.
             You can get the optimized value and the optimized parameters by "output" and  "optimizedParameter" object.
         """
         if self.MIP is None:
             self.MIP_transform()
         self.MIP.solve()
-        result = []
-        solved_variables = {}
-        solved_variables_dict = {}
-        for v in self.MIP.variables():
-            solved_variables[v.name] = v.varValue
-        for i in range(len(self.types)):
-            try:
-                solved_variables_dict['x_{}'.format(i)] = solved_variables['x_{}'.format(i)]
-            except:
-                solved_variables_dict['x_{}'.format(i)] = random.uniform(self.bounds[i][0], self.bounds[i][1])
-                if self.types[i] == LpInteger:
-                    solved_variables_dict['x_{}'.format(i)] = int(solved_variables_dict['x_{}'.format(i)] + 0.5)
-        optimizedParameter = []
-        for i in solved_variables_dict:
-            optimizedParameter.append(solved_variables_dict[i])
-        self.optimizedParameter = optimizedParameter
+        self.optimizedParameter = [self.MIP.variablesDict()["x_%d" % i].varValue for i in range(len(self.types))]
         self.output = value(self.MIP.objective)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyISBO-1.0.3/pyISBO/SBO_pulp/RandomForest.py` & `pyISBO-1.0.4/pyISBO/SBO_pulp/RandomForest.py`

 * *Files 8% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         '''
         Adding variables:
             Each input parameter corresponds to a variable (x_variable).
             Each leaf node corresponds to a binary variable (y_variable).
         '''
         for i in range(x_len):
             x_variable[i] = LpVariable('x_{}'.format(i), lowBound=local_section[0][i], upBound=local_section[1][i],
-                                          cat=self.types[i])
+                                       cat=self.types[i])
 
         y_variable = {}
         for j in range(len(estimators_)):
             y_variable[j] = LpVariable.dict('y_{}'.format(j), range(len(leaves_num[j])), cat=LpBinary)
 
         '''
         Setting a dictionary: with the effect of finding the corresponding decision
@@ -146,45 +146,33 @@
         # precision, float(inf) is not allowed.
         M = 10000
         for m in range(len(estimators_)):
             for i in range(estimators_[m].tree_.node_count):
                 if estimators_[m].tree_.children_left[i] != -1:
                     cons_leaves_1 = find_leaves(estimators_[m].tree_.children_left[i], estimators_[m].tree_)
                     MIP += M * (lpSum(y_dict_list[m][j] for j in cons_leaves_1) - 1) - (
-                                estimators_[m].tree_.threshold[i] - x_variable[estimators_[m].tree_.feature[i]]) <= 0
+                            estimators_[m].tree_.threshold[i] - x_variable[estimators_[m].tree_.feature[i]]) <= 0, \
+                           "tree_{}_node_{}_left".format(m, i)
                     cons_leaves_2 = find_leaves(estimators_[m].tree_.children_right[i], estimators_[m].tree_)
                     MIP += M * (lpSum(y_dict_list[m][j] for j in cons_leaves_2) - 1) + (
-                                estimators_[m].tree_.threshold[i] - x_variable[
-                            estimators_[m].tree_.feature[i]]) + 1 / M <= 0
-            MIP += lpSum(y_variable[m][i] for i in range(len(y_variable[m]))) == 1
-
+                            estimators_[m].tree_.threshold[i] - x_variable[
+                        estimators_[m].tree_.feature[i]]) + 1 / M <= 0, \
+                           "tree_{}_node_{}_right".format(m, i)
+            MIP += lpSum(y_variable[m][i] for i in range(len(y_variable[m]))) == 1, "tree_{}_leaf".format(m)
+        for i in range(x_len):
+            MIP += x_variable[i] >= local_section[0][i], "x_lb_{}".format(i)
+            MIP += x_variable[i] <= local_section[1][i], "x_ub_{}".format(i)
         self.MIP = MIP
-        
+
     def optimize(self):
         """
         solve the Pulp mix integer program
         :return: None.
         """
         if self.MIP is None:
             self.MIP_transform()
 
-        local_section = local_section_generator(self.bounds)
-        MIP = self.MIP
-        MIP.solve()
-        solved_variables = {}
-        for v in MIP.variables():
-            solved_variables[v.name] = v.varValue
-        solved_variables_dict = {}
-        for i in range(len(self.types)):
-            try:
-                solved_variables_dict['x_{}'.format(i)] = solved_variables['x_{}'.format(i)]
-            except:
-                solved_variables_dict['x_{}'.format(i)] = random.uniform(local_section[0][i], local_section[1][i])
-                if self.types[i] == LpInteger:
-                    solved_variables_dict['x_{}'.format(i)] = int(solved_variables_dict['x_{}'.format(i)] + 0.5)
-        optimizedParameter = []
-        for i in solved_variables_dict:
-            optimizedParameter.append(solved_variables_dict[i])
+        self.MIP.solve()
+        self.optimizedParameter = [self.MIP.variablesDict()["x_%d" % i].varValue for i in range(len(self.types))]
         # The objective function of the random forest is to sum the values of
         # all trees, averaging on return to maintain consistency with y.
-        self.output = value(MIP.objective) / len(self.model.estimators_)
-        self.optimizedParameter = optimizedParameter
+        self.output = value(self.MIP.objective) / len(self.model.estimators_)
```

### Comparing `pyISBO-1.0.3/pyISBO/SBO_pulp/RegressionSplines.py` & `pyISBO-1.0.4/pyISBO/SBO_pulp/RegressionSplines.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import numpy as np
 from sklearn.model_selection import cross_val_score
 from pyearth import Earth
 from pulp import *
-import random
 
 
 class MARS:
     """
     Linear Surrogate. Based on sklearn.linear_model.LinearRegression.
     """
     model = None
@@ -86,72 +85,61 @@
         branch_index = [i for i in range(len(summary))]
         intercept = self.model.coef_[0][0]
 
         self.MIP = LpProblem("MARS", LpMinimize)
         x = {}
         for i in range(len(self.types)):
             x[i] = LpVariable("x_%d" % i, self.bounds[i][0], self.bounds[i][1], cat=self.types[i])
+            self.MIP.addVariable(x[i])
         y = LpVariable("y")
         branch = {}
         for i in range(len(branch_index)):
             branch[i] = LpVariable("branch_%d" % i, cat=LpContinuous)
         z = {}
         for i in range(len(branch_index)):
             z[i] = LpVariable("z_%d" % i, lowBound=0, cat=LpBinary)
 
         M = 1e5
         self.MIP += y, "Objective"
         self.MIP += y == intercept + lpSum(branch[i] for i in range(len(summary))), "y"
+        for i in range(len(self.types)):
+            self.MIP += x[i] >= self.bounds[i][0]
+            self.MIP += x[i] <= self.bounds[i][1]
         for col in range(len(self.colName)):
             colname = self.colName[col]
             for i in range(len(summary)):
                 coef = float(summary[i][2])
                 if summary[i][0] == colname:  # 没有分割点
-                    self.MIP += branch[i] == coef * x[col], "branch[%d]" % i
+                    self.MIP += branch[i] == coef * x[col], "branch_%d" % i
                 if summary[i][0][2:2 + len(colname)] == colname:
                     point = summary[i][0][3 + len(colname):len(summary[i][0]) - 1]
                     try:
                         point = float(point)
-                        self.MIP += branch[i] >= x[col] - point, "h1[%d]" % i
-                        self.MIP += branch[i] >= 0, "h2[%d]" % i
-                        self.MIP += branch[i] <= x[col] - point + M*(1-z[i]), "h3[%d]" % i
-                        self.MIP += branch[i] <= M * z[i], "h4[%d]" % i
+                        self.MIP += branch[i] >= x[col] - point, "h1_%d" % i
+                        self.MIP += branch[i] >= 0, "h2_%d" % i
+                        self.MIP += branch[i] <= x[col] - point + M*(1-z[i]), "h3_%d" % i
+                        self.MIP += branch[i] <= M * z[i], "h4_%d" % i
                     except ValueError:
                         pass
 
                 if summary[i][0][len(summary[i][0]) - 1 - len(colname):len(summary[i][0]) - 1] == colname:
                     point = summary[i][0][2:len(summary[i][0]) - 2 - len(colname)]
                     try:
                         point = float(point)
-                        self.MIP += branch[i] >= point - x[col], "h1[%d]" % i
-                        self.MIP += branch[i] >= 0, "h2[%d]" % i
-                        self.MIP += branch[i] <= point - x[col] + M * (1 - z[i]), "h3[%d]" % i
-                        self.MIP += branch[i] <= M * z[i], "h4[%d]" % i
+                        self.MIP += branch[i] >= point - x[col], "h1_%d" % i
+                        self.MIP += branch[i] >= 0, "h2_%d" % i
+                        self.MIP += branch[i] <= point - x[col] + M * (1 - z[i]), "h3_%d" % i
+                        self.MIP += branch[i] <= M * z[i], "h4_%d" % i
                     except ValueError:
                         pass
 
     def optimize(self):
         """
         Optimize over the MIP
         :return: None.
             You can get the optimized value and the optimized parameters by "output" and  "optimizedParameter" object.
         """
         if self.MIP is None:
             self.MIP_transform()
         self.MIP.solve()
-        result = []
-        solved_variables = {}
-        solved_variables_dict = {}
-        for v in self.MIP.variables():
-            solved_variables[v.name] = v.varValue
-        for i in range(len(self.types)):
-            try:
-                solved_variables_dict['x_{}'.format(i)] = solved_variables['x_{}'.format(i)]
-            except:
-                solved_variables_dict['x_{}'.format(i)] = random.uniform(self.bounds[i][0], self.bounds[i][1])
-                if self.types[i] == LpInteger:
-                    solved_variables_dict['x_{}'.format(i)] = int(solved_variables_dict['x_{}'.format(i)] + 0.5)
-        optimizedParameter = []
-        for i in solved_variables_dict:
-            optimizedParameter.append(solved_variables_dict[i])
-        self.optimizedParameter = optimizedParameter
+        self.optimizedParameter = [self.MIP.variablesDict()["x_%d" % i].varValue for i in range(len(self.types))]
         self.output = value(self.MIP.objective)
```

### Comparing `pyISBO-1.0.3/pyISBO.egg-info/SOURCES.txt` & `pyISBO-1.0.4/pyISBO.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+README.md
 setup.py
 pyISBO/__init__.py
 pyISBO/main.py
 pyISBO.egg-info/PKG-INFO
 pyISBO.egg-info/SOURCES.txt
 pyISBO.egg-info/dependency_links.txt
 pyISBO.egg-info/top_level.txt
```

### Comparing `pyISBO-1.0.3/setup.py` & `pyISBO-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 setup(name="pyISBO",
-      version="1.0.3",
+      version="1.0.4",
       author="Liu Xiangting and Zhu Zesheng",
       author_email="liu-xt22@mails.tsinghua.edu.cn",
       packages = find_packages(),
       description="An integrated Surrogate-Base Optimization Toolbox",
       package_dir={"pyISBO":"pyISBO"},
       package_data={"pyISBO":['pyISBO/OperationData.xlsx']},
       url="https://github.com/Shawn1eo/pyISBO",
```

