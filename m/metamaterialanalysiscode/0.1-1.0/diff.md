# Comparing `tmp/metamaterialanalysiscode-0.1.tar.gz` & `tmp/metamaterialanalysiscode-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metamaterialanalysiscode-0.1.tar", last modified: Tue Jul 18 23:13:53 2023, max compression
+gzip compressed data, was "metamaterialanalysiscode-1.0.tar", last modified: Tue Jul 18 23:18:55 2023, max compression
```

## Comparing `metamaterialanalysiscode-0.1.tar` & `metamaterialanalysiscode-1.0.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 23:13:53.207565 metamaterialanalysiscode-0.1/
--rw-rw-rw-   0        0        0     1191 2023-06-26 22:03:03.000000 metamaterialanalysiscode-0.1/LICENSE
--rw-rw-rw-   0        0        0     5248 2023-07-18 23:13:53.207565 metamaterialanalysiscode-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3348 2023-06-26 20:57:16.000000 metamaterialanalysiscode-0.1/README.md
--rw-rw-rw-   0        0        0      783 2023-07-18 23:12:32.000000 metamaterialanalysiscode-0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-18 23:13:53.207565 metamaterialanalysiscode-0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-18 23:13:53.099516 metamaterialanalysiscode-0.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-18 23:13:53.110511 metamaterialanalysiscode-0.1/src/metamaterialanalysiscode/
--rw-rw-rw-   0        0        0      781 2023-05-25 18:48:47.000000 metamaterialanalysiscode-0.1/src/metamaterialanalysiscode/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 23:13:53.122503 metamaterialanalysiscode-0.1/src/metamaterialanalysiscode/_modules/
--rw-rw-rw-   0        0        0        0 2023-05-09 15:19:42.000000 metamaterialanalysiscode-0.1/src/metamaterialanalysiscode/_modules/__init__.py
--rw-rw-rw-   0        0        0     1036 2023-06-04 12:29:13.000000 metamaterialanalysiscode-0.1/src/metamaterialanalysiscode/_modules/_centers_RPA.py
-drwxrwxrwx   0        0        0        0 2023-07-18 23:13:53.191940 metamaterialanalysiscode-0.1/src/metamaterialanalysiscode/classes/
--rw-rw-rw-   0        0        0     5051 2023-05-28 11:36:43.000000 metamaterialanalysiscode-0.1/src/metamaterialanalysiscode/classes/MACAnalysis.py
--rw-rw-rw-   0        0        0     2096 2023-05-08 15:39:04.000000 metamaterialanalysiscode-0.1/src/metamaterialanalysiscode/classes/MACCell.py
--rw-rw-rw-   0        0        0     2725 2023-06-21 20:42:36.000000 metamaterialanalysiscode-0.1/src/metamaterialanalysiscode/classes/MACElement.py
--rw-rw-rw-   0        0        0      364 2023-05-12 09:04:56.000000 metamaterialanalysiscode-0.1/src/metamaterialanalysiscode/classes/MACGlobals.py
--rw-rw-rw-   0        0        0     8871 2023-05-22 18:16:23.000000 metamaterialanalysiscode-0.1/src/metamaterialanalysiscode/classes/MACLoadCase.py
--rw-rw-rw-   0        0        0     6027 2023-05-10 16:19:48.000000 metamaterialanalysiscode-0.1/src/metamaterialanalysiscode/classes/MACMaterial.py
--rw-rw-rw-   0        0        0     5679 2023-06-21 16:49:17.000000 metamaterialanalysiscode-0.1/src/metamaterialanalysiscode/classes/MACModel.py
--rw-rw-rw-   0        0        0     1734 2023-06-02 15:47:36.000000 metamaterialanalysiscode-0.1/src/metamaterialanalysiscode/classes/MACNode.py
--rw-rw-rw-   0        0        0     1591 2023-05-28 11:25:34.000000 metamaterialanalysiscode-0.1/src/metamaterialanalysiscode/classes/MACNonLinear.py
--rw-rw-rw-   0        0        0     4694 2023-05-10 15:07:32.000000 metamaterialanalysiscode-0.1/src/metamaterialanalysiscode/classes/MACProperty.py
--rw-rw-rw-   0        0        0    50022 2023-06-21 20:48:14.000000 metamaterialanalysiscode-0.1/src/metamaterialanalysiscode/classes/MACStructure.py
--rw-rw-rw-   0        0        0     4810 2023-06-18 10:04:36.000000 metamaterialanalysiscode-0.1/src/metamaterialanalysiscode/classes/MACSubcase.py
--rw-rw-rw-   0        0        0      690 2023-05-08 15:44:47.000000 metamaterialanalysiscode-0.1/src/metamaterialanalysiscode/classes/MACTable.py
--rw-rw-rw-   0        0        0        0 2023-05-04 06:18:05.000000 metamaterialanalysiscode-0.1/src/metamaterialanalysiscode/classes/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 23:13:53.207565 metamaterialanalysiscode-0.1/src/metamaterialanalysiscode/modules/
--rw-rw-rw-   0        0        0     1882 2023-06-13 21:24:05.000000 metamaterialanalysiscode-0.1/src/metamaterialanalysiscode/modules/MACRun.py
--rw-rw-rw-   0        0        0        0 2023-05-23 20:42:27.000000 metamaterialanalysiscode-0.1/src/metamaterialanalysiscode/modules/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 23:13:53.116508 metamaterialanalysiscode-0.1/src/metamaterialanalysiscode.egg-info/
--rw-rw-rw-   0        0        0     5248 2023-07-18 23:13:53.000000 metamaterialanalysiscode-0.1/src/metamaterialanalysiscode.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1191 2023-07-18 23:13:53.000000 metamaterialanalysiscode-0.1/src/metamaterialanalysiscode.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 23:13:53.000000 metamaterialanalysiscode-0.1/src/metamaterialanalysiscode.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-07-18 23:13:53.000000 metamaterialanalysiscode-0.1/src/metamaterialanalysiscode.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 23:18:55.356959 metamaterialanalysiscode-1.0/
+-rw-rw-rw-   0        0        0     1191 2023-06-26 22:03:03.000000 metamaterialanalysiscode-1.0/LICENSE
+-rw-rw-rw-   0        0        0     5574 2023-07-18 23:18:55.356959 metamaterialanalysiscode-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3476 2023-07-18 22:07:22.000000 metamaterialanalysiscode-1.0/README.md
+-rw-rw-rw-   0        0        0     1010 2023-07-18 23:13:21.000000 metamaterialanalysiscode-1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-18 23:18:55.356959 metamaterialanalysiscode-1.0/setup.cfg
+-rw-rw-rw-   0        0        0      134 2023-07-18 21:58:03.000000 metamaterialanalysiscode-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 23:18:55.319224 metamaterialanalysiscode-1.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-18 23:18:55.334829 metamaterialanalysiscode-1.0/src/metamaterialanalysiscode/
+-rw-rw-rw-   0        0        0      781 2023-05-25 18:48:47.000000 metamaterialanalysiscode-1.0/src/metamaterialanalysiscode/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 23:18:55.334829 metamaterialanalysiscode-1.0/src/metamaterialanalysiscode/_modules/
+-rw-rw-rw-   0        0        0        0 2023-05-09 15:19:42.000000 metamaterialanalysiscode-1.0/src/metamaterialanalysiscode/_modules/__init__.py
+-rw-rw-rw-   0        0        0     1036 2023-06-04 12:29:13.000000 metamaterialanalysiscode-1.0/src/metamaterialanalysiscode/_modules/_centers_RPA.py
+drwxrwxrwx   0        0        0        0 2023-07-18 23:18:55.356959 metamaterialanalysiscode-1.0/src/metamaterialanalysiscode/classes/
+-rw-rw-rw-   0        0        0     5055 2023-07-04 23:43:18.000000 metamaterialanalysiscode-1.0/src/metamaterialanalysiscode/classes/MACAnalysis.py
+-rw-rw-rw-   0        0        0     2096 2023-05-08 15:39:04.000000 metamaterialanalysiscode-1.0/src/metamaterialanalysiscode/classes/MACCell.py
+-rw-rw-rw-   0        0        0     2725 2023-06-21 20:42:36.000000 metamaterialanalysiscode-1.0/src/metamaterialanalysiscode/classes/MACElement.py
+-rw-rw-rw-   0        0        0      364 2023-07-04 18:38:16.000000 metamaterialanalysiscode-1.0/src/metamaterialanalysiscode/classes/MACGlobals.py
+-rw-rw-rw-   0        0        0     8871 2023-05-22 18:16:23.000000 metamaterialanalysiscode-1.0/src/metamaterialanalysiscode/classes/MACLoadCase.py
+-rw-rw-rw-   0        0        0     6027 2023-05-10 16:19:48.000000 metamaterialanalysiscode-1.0/src/metamaterialanalysiscode/classes/MACMaterial.py
+-rw-rw-rw-   0        0        0     5694 2023-07-04 18:43:28.000000 metamaterialanalysiscode-1.0/src/metamaterialanalysiscode/classes/MACModel.py
+-rw-rw-rw-   0        0        0     1734 2023-06-02 15:47:36.000000 metamaterialanalysiscode-1.0/src/metamaterialanalysiscode/classes/MACNode.py
+-rw-rw-rw-   0        0        0     1714 2023-07-03 22:01:13.000000 metamaterialanalysiscode-1.0/src/metamaterialanalysiscode/classes/MACNonLinear.py
+-rw-rw-rw-   0        0        0     4694 2023-05-10 15:07:32.000000 metamaterialanalysiscode-1.0/src/metamaterialanalysiscode/classes/MACProperty.py
+-rw-rw-rw-   0        0        0    50022 2023-06-21 20:48:14.000000 metamaterialanalysiscode-1.0/src/metamaterialanalysiscode/classes/MACStructure.py
+-rw-rw-rw-   0        0        0     4680 2023-07-04 23:43:18.000000 metamaterialanalysiscode-1.0/src/metamaterialanalysiscode/classes/MACSubcase.py
+-rw-rw-rw-   0        0        0      690 2023-05-08 15:44:47.000000 metamaterialanalysiscode-1.0/src/metamaterialanalysiscode/classes/MACTable.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 06:18:05.000000 metamaterialanalysiscode-1.0/src/metamaterialanalysiscode/classes/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 23:18:55.356959 metamaterialanalysiscode-1.0/src/metamaterialanalysiscode/modules/
+-rw-rw-rw-   0        0        0     1882 2023-06-13 21:24:05.000000 metamaterialanalysiscode-1.0/src/metamaterialanalysiscode/modules/MACRun.py
+-rw-rw-rw-   0        0        0        0 2023-05-23 20:42:27.000000 metamaterialanalysiscode-1.0/src/metamaterialanalysiscode/modules/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 23:18:55.334829 metamaterialanalysiscode-1.0/src/metamaterialanalysiscode.egg-info/
+-rw-rw-rw-   0        0        0     5574 2023-07-18 23:18:55.000000 metamaterialanalysiscode-1.0/src/metamaterialanalysiscode.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1251 2023-07-18 23:18:55.000000 metamaterialanalysiscode-1.0/src/metamaterialanalysiscode.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 23:18:55.000000 metamaterialanalysiscode-1.0/src/metamaterialanalysiscode.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-18 23:18:55.000000 metamaterialanalysiscode-1.0/src/metamaterialanalysiscode.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-07-18 23:18:55.000000 metamaterialanalysiscode-1.0/src/metamaterialanalysiscode.egg-info/top_level.txt
```

### Comparing `metamaterialanalysiscode-0.1/LICENSE` & `metamaterialanalysiscode-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metamaterialanalysiscode-0.1/PKG-INFO` & `metamaterialanalysiscode-1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: metamaterialanalysiscode
-Version: 0.1
-Summary: Package for generating FEM models based on cells
-Author-email: Manuel Sanchez Garcia <msg.aerospace@gmail.com>
+Version: 1.0
+Summary: Package that cretaes metamaterial FEM models
+Author-email: Manuel Sánchez García <msg.aerospace@gmail.com>
 License: Copyright 2023 Manuel Sánchez García
         
         The following license affect the code but not the intellectual property of the patents used in the code.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
         documentation files (the “Software”), to deal in the Software without restriction, including without limitation the
         rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
@@ -15,36 +15,46 @@
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of
         the Software.
         
         THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE
         WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
         COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
         OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-Keywords: mac,Preprocessing,FEM,Metamaterial
+Project-URL: ETSIAE, https://www.etsiae.upm.es/
+Project-URL: LinkedIn, https://www.linkedin.com/in/manuel-s%C3%A1nchez-garc%C3%ADa-8aa683232/
+Project-URL: GitHub, https://github.com/ManuelSG96/MAC
+Keywords: MAC,Preprocessing,Metamaterial,FEM
 Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+![](https://pbs.twimg.com/media/F1WYyq3WYAYEguI?format=png&name=900x900 "MAC")
+
+
 # Metamaterial Analysis Code
 
 ## 1. Introduction
 
 This code is the core of the TFM (Final Master Project) "Simulación Mediante  Elementos Finitos Del Comportamiento No
 Lineal De Metamateriales Auxéticos En Grandes Desplazamientos Para Uso Ingenieril." It is an OOP pacakage that
 allows the user to generate .fem files with the mesh of components based on metamaterial structure.
 This means that the material is not solid but consists of cells. Only works for Optistruct.
 
 ## 2. Version update
 
-As this is the first version, there are no updates.
+### v.1.0
+
+- Bug fixing
+- New classes for nonlinear analysis
+- Expansion of functionalities
 
 ## 3. Property and License
 
 The code is property of Manuel Sanchez and the ETSIAE. It follows the MIT license.
 
 The Patent used in the code is exclusively property of their creators. Copy or modifying are not allowed
 without permission of their owners.
@@ -81,23 +91,23 @@
 
 ````python
 modelo1.write_fem(r"C:\Users\admin\Desktop\test1_model.fem")
 ````
 
 Generating and printing an analyisis:
 ````python
-enforcedispl1 = MAC.set_load(id=1, type="SPC", nodes=nodesdisp, components=[3], displacement=-0.5, load=True)
+enforcedispl1 = mac.set_load(id=1, type="SPC", nodes=nodesdisp, components=[3], displacement=-0.5, load=True)
 
-constraint1 = MAC.set_constraint(id=2, nodes=nodesdisp, components=[3], displacement=-0.5)
+constraint1 = mac.set_constraint(id=2, nodes=nodesdisp, components=[3], displacement=-0.5)
 
-constraint2 = MAC.set_constraint(id=2, nodes=nodespc, components=[1, 2, 3, 4, 5, 6], displacement=0)
+constraint2 = mac.set_constraint(id=2, nodes=nodespc, components=[1, 2, 3, 4, 5, 6], displacement=0)
 
-subcase1 = MAC.set_subcase(id=1, label="linear", loads=[enforcedispl1], constraints=[constraint1, constraint2])
+subcase1 = mac.set_subcase(id=1, label="linear", loads=[enforcedispl1], constraints=[constraint1, constraint2])
 
-analysis2 = MAC.set_analysis(model=modelo1, subcases=[subcase1])
+analysis2 = mac.set_analysis(model=modelo1, subcases=[subcase1])
 
 analysis2.write_fem(r"C:\Users\admin\Desktop\test1_analysis.fem")
 ````
 
 As all the nodes and elements are saved in two dictionaries, the user can modify coords, properties, materials,
 etc.
```

### Comparing `metamaterialanalysiscode-0.1/README.md` & `metamaterialanalysiscode-1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,26 @@
+![](https://pbs.twimg.com/media/F1WYyq3WYAYEguI?format=png&name=900x900 "MAC")
+
+
 # Metamaterial Analysis Code
 
 ## 1. Introduction
 
 This code is the core of the TFM (Final Master Project) "Simulación Mediante  Elementos Finitos Del Comportamiento No
 Lineal De Metamateriales Auxéticos En Grandes Desplazamientos Para Uso Ingenieril." It is an OOP pacakage that
 allows the user to generate .fem files with the mesh of components based on metamaterial structure.
 This means that the material is not solid but consists of cells. Only works for Optistruct.
 
 ## 2. Version update
 
-As this is the first version, there are no updates.
+### v.1.0
+
+- Bug fixing
+- New classes for nonlinear analysis
+- Expansion of functionalities
 
 ## 3. Property and License
 
 The code is property of Manuel Sanchez and the ETSIAE. It follows the MIT license.
 
 The Patent used in the code is exclusively property of their creators. Copy or modifying are not allowed
 without permission of their owners.
@@ -50,23 +57,23 @@
 
 ````python
 modelo1.write_fem(r"C:\Users\admin\Desktop\test1_model.fem")
 ````
 
 Generating and printing an analyisis:
 ````python
-enforcedispl1 = MAC.set_load(id=1, type="SPC", nodes=nodesdisp, components=[3], displacement=-0.5, load=True)
+enforcedispl1 = mac.set_load(id=1, type="SPC", nodes=nodesdisp, components=[3], displacement=-0.5, load=True)
 
-constraint1 = MAC.set_constraint(id=2, nodes=nodesdisp, components=[3], displacement=-0.5)
+constraint1 = mac.set_constraint(id=2, nodes=nodesdisp, components=[3], displacement=-0.5)
 
-constraint2 = MAC.set_constraint(id=2, nodes=nodespc, components=[1, 2, 3, 4, 5, 6], displacement=0)
+constraint2 = mac.set_constraint(id=2, nodes=nodespc, components=[1, 2, 3, 4, 5, 6], displacement=0)
 
-subcase1 = MAC.set_subcase(id=1, label="linear", loads=[enforcedispl1], constraints=[constraint1, constraint2])
+subcase1 = mac.set_subcase(id=1, label="linear", loads=[enforcedispl1], constraints=[constraint1, constraint2])
 
-analysis2 = MAC.set_analysis(model=modelo1, subcases=[subcase1])
+analysis2 = mac.set_analysis(model=modelo1, subcases=[subcase1])
 
 analysis2.write_fem(r"C:\Users\admin\Desktop\test1_analysis.fem")
 ````
 
 As all the nodes and elements are saved in two dictionaries, the user can modify coords, properties, materials,
 etc.
```

### Comparing `metamaterialanalysiscode-0.1/pyproject.toml` & `metamaterialanalysiscode-1.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 [build-system]
 requires = ["setuptools>=67.8.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "metamaterialanalysiscode"
-version = "0.1"
+version = "1.0"
 license = {file = "LICENSE"}
 authors = [
-  { name="Manuel Sanchez Garcia", email="msg.aerospace@gmail.com" },
+  { name="Manuel Sánchez García", email="msg.aerospace@gmail.com" },
 ]
 requires-python = ">=3.10"
-description = "Package for generating FEM models based on cells"
+dependencies = ["numpy>=1.24.0",]
+description = "Package that cretaes metamaterial FEM models"
 readme = "README.md"
 classifiers = [
 	"Intended Audience :: Science/Research",
-    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 	"Topic :: Scientific/Engineering",
 ]
-keywords = ["mac", "Preprocessing", "FEM", "Metamaterial"]
+keywords = ["MAC", "Preprocessing", "Metamaterial", "FEM"]
+
+[project.urls]
+"ETSIAE" = "https://www.etsiae.upm.es/"
+"LinkedIn" = "https://www.linkedin.com/in/manuel-s%C3%A1nchez-garc%C3%ADa-8aa683232/"
+"GitHub" = "https://github.com/ManuelSG96/MAC"
 
 [tool.setuptools]
 package-dir = {"" = "src"}
 
 [tool.setuptools.packages.find]
 where = ["src"]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `metamaterialanalysiscode-0.1/src/metamaterialanalysiscode/__init__.py` & `metamaterialanalysiscode-1.0/src/metamaterialanalysiscode/__init__.py`

 * *Files identical despite different names*

### Comparing `metamaterialanalysiscode-0.1/src/metamaterialanalysiscode/_modules/_centers_RPA.py` & `metamaterialanalysiscode-1.0/src/metamaterialanalysiscode/_modules/_centers_RPA.py`

 * *Files identical despite different names*

### Comparing `metamaterialanalysiscode-0.1/src/metamaterialanalysiscode/classes/MACAnalysis.py` & `metamaterialanalysiscode-1.0/src/metamaterialanalysiscode/classes/MACAnalysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
             pathfem += ".fem"
 
         if path.exists(pathfem):
             remove(pathfem)
             print(f"File {pathfem} already exists. It has been overwritten.")
 
         today = datetime.now().strftime("%d/%m/%Y - %H:%M:%S")
-        analysis_name = pathfem.split("\\")[-1].split(".")[0]
+        analysis_name = pathfem.split("\\")[-1].rsplit(".", 1)[0]
         macverlen = 78 - (len(MAC_VERSION) + len("$ MAC version: "))
         analysis_namelen = 78 - (len(analysis_name) + len("$ Analysis Name: "))
 
         header = "$" * 82 + "\n" + \
                  "$" * 14 + "  File generated by Metamaterial Analysis Code (MAC)  " + "$" * 14 + "\n" + \
                  "$" * 82 + "\n" + \
                  "$$" + " " * 78 + "$$" + "\n" + \
```

### Comparing `metamaterialanalysiscode-0.1/src/metamaterialanalysiscode/classes/MACCell.py` & `metamaterialanalysiscode-1.0/src/metamaterialanalysiscode/classes/MACCell.py`

 * *Files identical despite different names*

### Comparing `metamaterialanalysiscode-0.1/src/metamaterialanalysiscode/classes/MACElement.py` & `metamaterialanalysiscode-1.0/src/metamaterialanalysiscode/classes/MACElement.py`

 * *Files identical despite different names*

### Comparing `metamaterialanalysiscode-0.1/src/metamaterialanalysiscode/classes/MACLoadCase.py` & `metamaterialanalysiscode-1.0/src/metamaterialanalysiscode/classes/MACLoadCase.py`

 * *Files identical despite different names*

### Comparing `metamaterialanalysiscode-0.1/src/metamaterialanalysiscode/classes/MACMaterial.py` & `metamaterialanalysiscode-1.0/src/metamaterialanalysiscode/classes/MACMaterial.py`

 * *Files identical despite different names*

### Comparing `metamaterialanalysiscode-0.1/src/metamaterialanalysiscode/classes/MACModel.py` & `metamaterialanalysiscode-1.0/src/metamaterialanalysiscode/classes/MACModel.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,30 +30,30 @@
         """
         Constructor for MACModel class
         """
         self.__modeldimensions = modeldimensions
         self.__cellstructure = cellstructure
         self.__cellmaterial = cellmaterial
         self.__cellproperty = cellproperty
-        self.__celldict = {}
+        self.CellDict: dict[MACCell] = {}
 
         # Function to generate the cells centers for auxetic structures
         cloud_set = _centers_RPA(a=round((3**0.5) * 0.5 * self.__cellstructure.Stepy, 4),
                                  h=round(self.__cellstructure.Hprisma, 4),
                                  stx=round(self.__cellstructure.Stepx, 4),
                                  dimensions=self.__modeldimensions
                                  )
 
         for i, center in enumerate(cloud_set):
             nodes, elements = self.__cellstructure.build(
                                                          cellcenter=center, mat=self.__cellmaterial[0],
                                                          prop=self.__cellproperty[0], vvector=(0.0, 0.0, 1.0)
                                                         )
 
-            self.__celldict[i] = MACCell(i, self.__cellstructure, center, elements, nodes, self.__cellmaterial,
+            self.CellDict[i] = MACCell(i, self.__cellstructure, center, elements, nodes, self.__cellmaterial,
                                          self.__cellproperty)
 
         self.NodeDict = {node.ID: node for node in NODES_DICT.values()}
         self.ElementDict: ElementDictType = {element.ID: element for element in ELEMENTS_SET}
 
     def write_fem(self, path: str, writeheader: bool = True) -> None:
         """
@@ -65,15 +65,15 @@
             path += ".fem"
 
         with open(path, "a") as w:
 
             if writeheader:
 
                 today = datetime.now().strftime("%d/%m/%Y - %H:%M:%S")
-                analysis_name = path.split("\\")[-1].split(".")[0]
+                analysis_name = path.split("\\")[-1].rsplit(".", 1)[0]
                 macverlen = 78 - (len(MAC_VERSION) + len("$$  MAC version: "))
                 analysis_namelen = 78 - (len(analysis_name) + len("$$  Analysis Name: "))
 
                 header = "$" * 80 + "\n" + \
                          "$" * 13 + "  File generated by Metamaterial Analysis Code (MAC)  " + "$" * 13 + "\n" + \
                          "$" * 80 + "\n" + \
                          "$$" + " " * 76 + "$$" + "\n" + \
```

### Comparing `metamaterialanalysiscode-0.1/src/metamaterialanalysiscode/classes/MACNode.py` & `metamaterialanalysiscode-1.0/src/metamaterialanalysiscode/classes/MACNode.py`

 * *Files identical despite different names*

### Comparing `metamaterialanalysiscode-0.1/src/metamaterialanalysiscode/classes/MACNonLinear.py` & `metamaterialanalysiscode-1.0/src/metamaterialanalysiscode/classes/MACNonLinear.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,28 +4,30 @@
 
 
 class MACNLparmLD:
     """
     Class for the NonLinear Parameters for Large Displacements (NLparmLD).
     """
 
-    def __init__(self, id: int, dt: float):
+    def __init__(self, id: int, ninc: int, dt: float):
         """
         Constructor for MACNLparmLD class
         """
         self.ID = id
         self.DT = dt
+        self.Ninc = ninc
 
     def __str__(self):
         """
         Method to print the NonLinear Parameters for Large Displacements (NLaprmLD) class.
         """
         idspaces = " " * (8 - len(str(self.ID)))
         dtspaces = " " * (8 - len(str(self.DT)))
-        return f"NLPARM  {idspaces}{self.ID}        {dtspaces}{self.DT}\n"
+        nincspaces = " " * (8 - len(str(self.Ninc)))
+        return f"NLPARM  {idspaces}{self.ID}{nincspaces}{self.Ninc}{dtspaces}{self.DT}\n"
 
 
 class MACNLout:
     """
     Class for the NonLinear Output (NLout).
     """
 
@@ -41,19 +43,19 @@
         Method to print the NonLinear Output (NLout) class.
         """
         idspaces = " " * (8 - len(str(self.ID)))
         nintspaces = " " * (8 - len(str(self.NINT)))
         return f"NLOUT   {idspaces}{self.ID}    NINT{nintspaces}{self.NINT}\n"
 
 
-def set_nlparmld(id: int, dt: float):
+def set_nlparmld(id: int, ninc: int, dt: float):
     """
     Function to create a NonLinear Parameters for Large Displacements (NLaprmLD) class.
     """
-    return MACNLparmLD(id, dt)
+    return MACNLparmLD(id, ninc, dt)
 
 
 def set_nlout(id: int, nint: int):
     """
     Function to create a NonLinear Output (NLout) class.
     """
     return MACNLout(id, nint)
```

### Comparing `metamaterialanalysiscode-0.1/src/metamaterialanalysiscode/classes/MACProperty.py` & `metamaterialanalysiscode-1.0/src/metamaterialanalysiscode/classes/MACProperty.py`

 * *Files identical despite different names*

### Comparing `metamaterialanalysiscode-0.1/src/metamaterialanalysiscode/classes/MACStructure.py` & `metamaterialanalysiscode-1.0/src/metamaterialanalysiscode/classes/MACStructure.py`

 * *Files identical despite different names*

### Comparing `metamaterialanalysiscode-0.1/src/metamaterialanalysiscode/classes/MACSubcase.py` & `metamaterialanalysiscode-1.0/src/metamaterialanalysiscode/classes/MACSubcase.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,51 +48,51 @@
         self.Output = output
 
     def __str__(self):
         """
         Method to print a subcase. It uses the 8 characters format of Optistruct.
         """
 
-        idspaces = " " * 8
+        idspaces = " "
         case = ""
         outstr = ""
         if isinstance(self.Output, list):
             for out in self.Output:
                 outstr += "  " + out + "\n"
 
         if not self.Label.startswith("buckling") and isinstance(self.Load[0], MACForce):
-            loadspaces = " " * (8 - len(str(self.Load[0].ID)))
-            case += f"  LOAD = {loadspaces}{self.Load[0].ID}\n"
+            loadspaces = " "
+            case += f"  LOAD ={loadspaces}{self.Load[0].ID}\n"
 
         elif not self.Label.startswith("buckling") and isinstance(self.Load[0], MACSpc):
-            loadspaces = " " * (8 - len(str(self.Load[0].ID)))
-            case += f"  LOAD = {loadspaces}{self.Load[0].ID}\n"
+            loadspaces = " "
+            case += f"  LOAD ={loadspaces}{self.Load[0].ID}\n"
 
-        loadspaces = " " * (8 - len(str(self.Spc[0].ID)))
-        case += f"  SPC = {loadspaces}{self.Spc[0].ID}\n"
+        loadspaces = " "
+        case += f"  SPC ={loadspaces}{self.Spc[0].ID}\n"
 
         # returns the subcase depending on its label -------------------------------------------------------------------
         if self.Label.startswith("linear"):
             return f"SUBCASE{idspaces}{self.ID}\n" + f"  LABEL {self.Label}\n" + case + outstr
 
         elif self.Label.startswith("buckling"):
             if self.StatSub is None:
                 raise ValueError("Buckling subcase needs a linear static subcase")
             else:
-                subspaces = " " * 8
-                methodspace = " " * 8
+                subspaces = " "
+                methodspace = " "
 
             return f"SUBCASE{idspaces}{self.ID}\n" + f"  LABEL {self.Label}\n" + "ANALYSIS BUCK\n" + case + \
                    f"  METHOD(STRUCTURE) ={methodspace}{self.Eigr.ID}\n" + \
                    f"  STATSUB(BUCKLING) ={subspaces}{self.StatSub.ID}\n" + outstr
 
         elif self.Label.startswith("nonlinear"):
             return f"SUBCASE{idspaces}{self.ID}\n" + f"  LABEL {self.Label}\n" + "ANALYSIS NLSTAT\n" + case + \
-                   f"  NLPARM(LGDISP) =        {self.NLaprmLD.ID}\n" + \
-                   f"  NLOUT =        {self.NLout.ID}\n" + outstr
+                   f"  NLPARM(LGDISP) = {self.NLaprmLD.ID}\n" + \
+                   f"  NLOUT = {self.NLout.ID}\n" + outstr
 
 
 def set_subcase(id: int, label: str, constraints: list[MACSpc, ...], loads: list[MACForce | MACSpc, ...] = None,
                 eigr: MACEigrl = None, stat_sub: object = None, nlparmld: MACNLparmLD = None, nlout: MACNLout = None,
                 output: list[str] = None):
     """
     Function to set a subcase. It returns a MACSubcase object.
```

### Comparing `metamaterialanalysiscode-0.1/src/metamaterialanalysiscode/classes/MACTable.py` & `metamaterialanalysiscode-1.0/src/metamaterialanalysiscode/classes/MACTable.py`

 * *Files identical despite different names*

### Comparing `metamaterialanalysiscode-0.1/src/metamaterialanalysiscode/modules/MACRun.py` & `metamaterialanalysiscode-1.0/src/metamaterialanalysiscode/modules/MACRun.py`

 * *Files identical despite different names*

### Comparing `metamaterialanalysiscode-0.1/src/metamaterialanalysiscode.egg-info/PKG-INFO` & `metamaterialanalysiscode-1.0/src/metamaterialanalysiscode.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: metamaterialanalysiscode
-Version: 0.1
-Summary: Package for generating FEM models based on cells
-Author-email: Manuel Sanchez Garcia <msg.aerospace@gmail.com>
+Version: 1.0
+Summary: Package that cretaes metamaterial FEM models
+Author-email: Manuel Sánchez García <msg.aerospace@gmail.com>
 License: Copyright 2023 Manuel Sánchez García
         
         The following license affect the code but not the intellectual property of the patents used in the code.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
         documentation files (the “Software”), to deal in the Software without restriction, including without limitation the
         rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit
@@ -15,36 +15,46 @@
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of
         the Software.
         
         THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE
         WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
         COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
         OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-Keywords: mac,Preprocessing,FEM,Metamaterial
+Project-URL: ETSIAE, https://www.etsiae.upm.es/
+Project-URL: LinkedIn, https://www.linkedin.com/in/manuel-s%C3%A1nchez-garc%C3%ADa-8aa683232/
+Project-URL: GitHub, https://github.com/ManuelSG96/MAC
+Keywords: MAC,Preprocessing,Metamaterial,FEM
 Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+![](https://pbs.twimg.com/media/F1WYyq3WYAYEguI?format=png&name=900x900 "MAC")
+
+
 # Metamaterial Analysis Code
 
 ## 1. Introduction
 
 This code is the core of the TFM (Final Master Project) "Simulación Mediante  Elementos Finitos Del Comportamiento No
 Lineal De Metamateriales Auxéticos En Grandes Desplazamientos Para Uso Ingenieril." It is an OOP pacakage that
 allows the user to generate .fem files with the mesh of components based on metamaterial structure.
 This means that the material is not solid but consists of cells. Only works for Optistruct.
 
 ## 2. Version update
 
-As this is the first version, there are no updates.
+### v.1.0
+
+- Bug fixing
+- New classes for nonlinear analysis
+- Expansion of functionalities
 
 ## 3. Property and License
 
 The code is property of Manuel Sanchez and the ETSIAE. It follows the MIT license.
 
 The Patent used in the code is exclusively property of their creators. Copy or modifying are not allowed
 without permission of their owners.
@@ -81,23 +91,23 @@
 
 ````python
 modelo1.write_fem(r"C:\Users\admin\Desktop\test1_model.fem")
 ````
 
 Generating and printing an analyisis:
 ````python
-enforcedispl1 = MAC.set_load(id=1, type="SPC", nodes=nodesdisp, components=[3], displacement=-0.5, load=True)
+enforcedispl1 = mac.set_load(id=1, type="SPC", nodes=nodesdisp, components=[3], displacement=-0.5, load=True)
 
-constraint1 = MAC.set_constraint(id=2, nodes=nodesdisp, components=[3], displacement=-0.5)
+constraint1 = mac.set_constraint(id=2, nodes=nodesdisp, components=[3], displacement=-0.5)
 
-constraint2 = MAC.set_constraint(id=2, nodes=nodespc, components=[1, 2, 3, 4, 5, 6], displacement=0)
+constraint2 = mac.set_constraint(id=2, nodes=nodespc, components=[1, 2, 3, 4, 5, 6], displacement=0)
 
-subcase1 = MAC.set_subcase(id=1, label="linear", loads=[enforcedispl1], constraints=[constraint1, constraint2])
+subcase1 = mac.set_subcase(id=1, label="linear", loads=[enforcedispl1], constraints=[constraint1, constraint2])
 
-analysis2 = MAC.set_analysis(model=modelo1, subcases=[subcase1])
+analysis2 = mac.set_analysis(model=modelo1, subcases=[subcase1])
 
 analysis2.write_fem(r"C:\Users\admin\Desktop\test1_analysis.fem")
 ````
 
 As all the nodes and elements are saved in two dictionaries, the user can modify coords, properties, materials,
 etc.
```

### Comparing `metamaterialanalysiscode-0.1/src/metamaterialanalysiscode.egg-info/SOURCES.txt` & `metamaterialanalysiscode-1.0/src/metamaterialanalysiscode.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 LICENSE
 README.md
 pyproject.toml
+setup.py
 src/metamaterialanalysiscode/__init__.py
 src/metamaterialanalysiscode.egg-info/PKG-INFO
 src/metamaterialanalysiscode.egg-info/SOURCES.txt
 src/metamaterialanalysiscode.egg-info/dependency_links.txt
+src/metamaterialanalysiscode.egg-info/requires.txt
 src/metamaterialanalysiscode.egg-info/top_level.txt
 src/metamaterialanalysiscode/_modules/__init__.py
 src/metamaterialanalysiscode/_modules/_centers_RPA.py
 src/metamaterialanalysiscode/classes/MACAnalysis.py
 src/metamaterialanalysiscode/classes/MACCell.py
 src/metamaterialanalysiscode/classes/MACElement.py
 src/metamaterialanalysiscode/classes/MACGlobals.py
```

