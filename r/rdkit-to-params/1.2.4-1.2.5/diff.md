# Comparing `tmp/rdkit_to_params-1.2.4.tar.gz` & `tmp/rdkit_to_params-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdkit_to_params-1.2.4.tar", last modified: Sun May 21 16:16:33 2023, max compression
+gzip compressed data, was "rdkit_to_params-1.2.5.tar", last modified: Wed Jul 19 06:28:05 2023, max compression
```

## Comparing `rdkit_to_params-1.2.4.tar` & `rdkit_to_params-1.2.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 user       (502) staff       (20)        0 2023-05-21 16:16:33.329975 rdkit_to_params-1.2.4/
--rw-r--r--   0 user       (502) staff       (20)     1069 2023-05-21 13:24:25.000000 rdkit_to_params-1.2.4/LICENSE
--rw-r--r--   0 user       (502) staff       (20)    18257 2023-05-21 16:16:33.329233 rdkit_to_params-1.2.4/PKG-INFO
--rw-r--r--   0 user       (502) staff       (20)    17342 2023-05-21 13:24:25.000000 rdkit_to_params-1.2.4/README.md
-drwxr-xr-x   0 user       (502) staff       (20)        0 2023-05-21 16:16:33.307039 rdkit_to_params-1.2.4/rdkit_to_params/
--rw-r--r--   0 user       (502) staff       (20)    17168 2023-05-21 13:24:25.000000 rdkit_to_params-1.2.4/rdkit_to_params/__init__.py
--rw-r--r--   0 user       (502) staff       (20)     3120 2023-05-21 13:24:25.000000 rdkit_to_params-1.2.4/rdkit_to_params/_init_mixin.py
--rw-r--r--   0 user       (502) staff       (20)     3945 2023-05-21 13:24:25.000000 rdkit_to_params-1.2.4/rdkit_to_params/_io_mixin.py
--rw-r--r--   0 user       (502) staff       (20)     3827 2023-05-21 13:24:25.000000 rdkit_to_params-1.2.4/rdkit_to_params/_pyrosetta_mixin.py
-drwxr-xr-x   0 user       (502) staff       (20)        0 2023-05-21 16:16:33.315839 rdkit_to_params-1.2.4/rdkit_to_params/cli/
--rw-r--r--   0 user       (502) staff       (20)     1114 2023-05-21 13:24:25.000000 rdkit_to_params-1.2.4/rdkit_to_params/cli/__init__.py
--rw-r--r--   0 user       (502) staff       (20)    17294 2023-05-21 13:24:25.000000 rdkit_to_params-1.2.4/rdkit_to_params/constraint.py
--rw-r--r--   0 user       (502) staff       (20)    23873 2023-05-21 13:24:25.000000 rdkit_to_params-1.2.4/rdkit_to_params/entries.py
-drwxr-xr-x   0 user       (502) staff       (20)        0 2023-05-21 16:16:33.327493 rdkit_to_params-1.2.4/rdkit_to_params/rdkitside/
--rw-r--r--   0 user       (502) staff       (20)      877 2023-05-21 13:24:25.000000 rdkit_to_params-1.2.4/rdkit_to_params/rdkitside/__init__.py
--rw-r--r--   0 user       (502) staff       (20)    22111 2023-05-21 16:12:20.000000 rdkit_to_params-1.2.4/rdkit_to_params/rdkitside/_rdkit_convert.py
--rw-r--r--   0 user       (502) staff       (20)     6316 2023-05-21 13:24:25.000000 rdkit_to_params-1.2.4/rdkit_to_params/rdkitside/_rdkit_inits.py
--rw-r--r--   0 user       (502) staff       (20)    31173 2023-05-21 14:07:44.000000 rdkit_to_params-1.2.4/rdkit_to_params/rdkitside/_rdkit_prep.py
--rw-r--r--   0 user       (502) staff       (20)     9736 2023-05-21 13:24:25.000000 rdkit_to_params-1.2.4/rdkit_to_params/rdkitside/_rdkit_rename.py
--rw-r--r--   0 user       (502) staff       (20)     3695 2023-05-21 13:24:25.000000 rdkit_to_params-1.2.4/rdkit_to_params/rdkitside/utilities.py
--rw-r--r--   0 user       (502) staff       (20)      217 2023-05-21 16:15:44.000000 rdkit_to_params-1.2.4/rdkit_to_params/version.py
-drwxr-xr-x   0 user       (502) staff       (20)        0 2023-05-21 16:16:33.313614 rdkit_to_params-1.2.4/rdkit_to_params.egg-info/
--rw-r--r--   0 user       (502) staff       (20)    18257 2023-05-21 16:16:33.000000 rdkit_to_params-1.2.4/rdkit_to_params.egg-info/PKG-INFO
--rw-r--r--   0 user       (502) staff       (20)      729 2023-05-21 16:16:33.000000 rdkit_to_params-1.2.4/rdkit_to_params.egg-info/SOURCES.txt
--rw-r--r--   0 user       (502) staff       (20)        1 2023-05-21 16:16:33.000000 rdkit_to_params-1.2.4/rdkit_to_params.egg-info/dependency_links.txt
--rw-r--r--   0 user       (502) staff       (20)       64 2023-05-21 16:16:33.000000 rdkit_to_params-1.2.4/rdkit_to_params.egg-info/entry_points.txt
--rw-r--r--   0 user       (502) staff       (20)       22 2023-05-21 16:16:33.000000 rdkit_to_params-1.2.4/rdkit_to_params.egg-info/top_level.txt
--rw-r--r--   0 user       (502) staff       (20)       38 2023-05-21 16:16:33.330109 rdkit_to_params-1.2.4/setup.cfg
--rw-r--r--   0 user       (502) staff       (20)     2802 2023-05-21 16:15:44.000000 rdkit_to_params-1.2.4/setup.py
-drwxr-xr-x   0 user       (502) staff       (20)        0 2023-05-21 16:16:33.328262 rdkit_to_params-1.2.4/tests/
--rw-r--r--   0 user       (502) staff       (20)     1644 2023-05-21 14:06:49.000000 rdkit_to_params-1.2.4/tests/__init__.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2023-07-19 06:28:05.648646 rdkit_to_params-1.2.5/
+-rw-r--r--   0 user       (502) staff       (20)     1069 2023-05-21 13:24:25.000000 rdkit_to_params-1.2.5/LICENSE
+-rw-r--r--   0 user       (502) staff       (20)    18257 2023-07-19 06:28:05.646564 rdkit_to_params-1.2.5/PKG-INFO
+-rw-r--r--   0 user       (502) staff       (20)    17342 2023-05-21 13:24:25.000000 rdkit_to_params-1.2.5/README.md
+drwxr-xr-x   0 user       (502) staff       (20)        0 2023-07-19 06:28:05.584291 rdkit_to_params-1.2.5/rdkit_to_params/
+-rw-r--r--   0 user       (502) staff       (20)    17168 2023-05-21 13:24:25.000000 rdkit_to_params-1.2.5/rdkit_to_params/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)     3120 2023-05-21 13:24:25.000000 rdkit_to_params-1.2.5/rdkit_to_params/_init_mixin.py
+-rw-r--r--   0 user       (502) staff       (20)     3945 2023-05-21 13:24:25.000000 rdkit_to_params-1.2.5/rdkit_to_params/_io_mixin.py
+-rw-r--r--   0 user       (502) staff       (20)     3827 2023-05-21 13:24:25.000000 rdkit_to_params-1.2.5/rdkit_to_params/_pyrosetta_mixin.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2023-07-19 06:28:05.619775 rdkit_to_params-1.2.5/rdkit_to_params/cli/
+-rw-r--r--   0 user       (502) staff       (20)     1114 2023-05-21 13:24:25.000000 rdkit_to_params-1.2.5/rdkit_to_params/cli/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)    17294 2023-05-21 13:24:25.000000 rdkit_to_params-1.2.5/rdkit_to_params/constraint.py
+-rw-r--r--   0 user       (502) staff       (20)    23873 2023-05-21 13:24:25.000000 rdkit_to_params-1.2.5/rdkit_to_params/entries.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2023-07-19 06:28:05.640492 rdkit_to_params-1.2.5/rdkit_to_params/rdkitside/
+-rw-r--r--   0 user       (502) staff       (20)      877 2023-05-21 13:24:25.000000 rdkit_to_params-1.2.5/rdkit_to_params/rdkitside/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)    22111 2023-05-21 16:12:20.000000 rdkit_to_params-1.2.5/rdkit_to_params/rdkitside/_rdkit_convert.py
+-rw-r--r--   0 user       (502) staff       (20)     6316 2023-05-21 13:24:25.000000 rdkit_to_params-1.2.5/rdkit_to_params/rdkitside/_rdkit_inits.py
+-rw-r--r--   0 user       (502) staff       (20)    31173 2023-07-19 06:24:39.000000 rdkit_to_params-1.2.5/rdkit_to_params/rdkitside/_rdkit_prep.py
+-rw-r--r--   0 user       (502) staff       (20)     9736 2023-05-21 13:24:25.000000 rdkit_to_params-1.2.5/rdkit_to_params/rdkitside/_rdkit_rename.py
+-rw-r--r--   0 user       (502) staff       (20)     3695 2023-05-21 13:24:25.000000 rdkit_to_params-1.2.5/rdkit_to_params/rdkitside/utilities.py
+-rw-r--r--   0 user       (502) staff       (20)      217 2023-07-19 06:25:17.000000 rdkit_to_params-1.2.5/rdkit_to_params/version.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2023-07-19 06:28:05.617452 rdkit_to_params-1.2.5/rdkit_to_params.egg-info/
+-rw-r--r--   0 user       (502) staff       (20)    18257 2023-07-19 06:28:05.000000 rdkit_to_params-1.2.5/rdkit_to_params.egg-info/PKG-INFO
+-rw-r--r--   0 user       (502) staff       (20)      729 2023-07-19 06:28:05.000000 rdkit_to_params-1.2.5/rdkit_to_params.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (502) staff       (20)        1 2023-07-19 06:28:05.000000 rdkit_to_params-1.2.5/rdkit_to_params.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (502) staff       (20)       64 2023-07-19 06:28:05.000000 rdkit_to_params-1.2.5/rdkit_to_params.egg-info/entry_points.txt
+-rw-r--r--   0 user       (502) staff       (20)       22 2023-07-19 06:28:05.000000 rdkit_to_params-1.2.5/rdkit_to_params.egg-info/top_level.txt
+-rw-r--r--   0 user       (502) staff       (20)       38 2023-07-19 06:28:05.649067 rdkit_to_params-1.2.5/setup.cfg
+-rw-r--r--   0 user       (502) staff       (20)     2802 2023-07-19 06:25:02.000000 rdkit_to_params-1.2.5/setup.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2023-07-19 06:28:05.643582 rdkit_to_params-1.2.5/tests/
+-rw-r--r--   0 user       (502) staff       (20)     1644 2023-05-21 14:06:49.000000 rdkit_to_params-1.2.5/tests/__init__.py
```

### Comparing `rdkit_to_params-1.2.4/LICENSE` & `rdkit_to_params-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rdkit_to_params-1.2.4/PKG-INFO` & `rdkit_to_params-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdkit_to_params
-Version: 1.2.4
+Version: 1.2.5
 Summary: Create or modify Rosetta params files (topology files) from scratch, RDKit mols or another params file.
 Home-page: https://github.com/matteoferla/rdkit_to_params
 Author: Matteo Ferla
 Author-email: matteo.ferla@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `rdkit_to_params-1.2.4/README.md` & `rdkit_to_params-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `rdkit_to_params-1.2.4/rdkit_to_params/__init__.py` & `rdkit_to_params-1.2.5/rdkit_to_params/__init__.py`

 * *Files identical despite different names*

### Comparing `rdkit_to_params-1.2.4/rdkit_to_params/_init_mixin.py` & `rdkit_to_params-1.2.5/rdkit_to_params/_init_mixin.py`

 * *Files identical despite different names*

### Comparing `rdkit_to_params-1.2.4/rdkit_to_params/_io_mixin.py` & `rdkit_to_params-1.2.5/rdkit_to_params/_io_mixin.py`

 * *Files identical despite different names*

### Comparing `rdkit_to_params-1.2.4/rdkit_to_params/_pyrosetta_mixin.py` & `rdkit_to_params-1.2.5/rdkit_to_params/_pyrosetta_mixin.py`

 * *Files identical despite different names*

### Comparing `rdkit_to_params-1.2.4/rdkit_to_params/cli/__init__.py` & `rdkit_to_params-1.2.5/rdkit_to_params/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `rdkit_to_params-1.2.4/rdkit_to_params/constraint.py` & `rdkit_to_params-1.2.5/rdkit_to_params/constraint.py`

 * *Files identical despite different names*

### Comparing `rdkit_to_params-1.2.4/rdkit_to_params/entries.py` & `rdkit_to_params-1.2.5/rdkit_to_params/entries.py`

 * *Files identical despite different names*

### Comparing `rdkit_to_params-1.2.4/rdkit_to_params/rdkitside/__init__.py` & `rdkit_to_params-1.2.5/rdkit_to_params/rdkitside/__init__.py`

 * *Files identical despite different names*

### Comparing `rdkit_to_params-1.2.4/rdkit_to_params/rdkitside/_rdkit_convert.py` & `rdkit_to_params-1.2.5/rdkit_to_params/rdkitside/_rdkit_convert.py`

 * *Files identical despite different names*

### Comparing `rdkit_to_params-1.2.4/rdkit_to_params/rdkitside/_rdkit_inits.py` & `rdkit_to_params-1.2.5/rdkit_to_params/rdkitside/_rdkit_inits.py`

 * *Files identical despite different names*

### Comparing `rdkit_to_params-1.2.4/rdkit_to_params/rdkitside/_rdkit_prep.py` & `rdkit_to_params-1.2.5/rdkit_to_params/rdkitside/_rdkit_prep.py`

 * *Files 0% similar despite different names*

```diff
@@ -596,15 +596,15 @@
         :return:
         """
         for i in range(self.mol.GetNumAtoms()):
             atom = self.mol.GetAtomWithIdx(i)
             atomname = self._get_PDBInfo_atomname(atom, throw=False)
             if atomname:
                 atom.SetProp('_OriginalName', atomname)
-            if atom.GetAtomicNum() == 0:
+            if atom.GetAtomicNum() != 0:
                 self._set_PDBInfo_atomname(atom, f'XX{i: <2}', overwrite=True)
 
     def move_back(self):
         """
         Removes the ugly XX!
 
         :return:
```

### Comparing `rdkit_to_params-1.2.4/rdkit_to_params/rdkitside/_rdkit_rename.py` & `rdkit_to_params-1.2.5/rdkit_to_params/rdkitside/_rdkit_rename.py`

 * *Files identical despite different names*

### Comparing `rdkit_to_params-1.2.4/rdkit_to_params/rdkitside/utilities.py` & `rdkit_to_params-1.2.5/rdkit_to_params/rdkitside/utilities.py`

 * *Files identical despite different names*

### Comparing `rdkit_to_params-1.2.4/rdkit_to_params.egg-info/PKG-INFO` & `rdkit_to_params-1.2.5/rdkit_to_params.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdkit-to-params
-Version: 1.2.4
+Version: 1.2.5
 Summary: Create or modify Rosetta params files (topology files) from scratch, RDKit mols or another params file.
 Home-page: https://github.com/matteoferla/rdkit_to_params
 Author: Matteo Ferla
 Author-email: matteo.ferla@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

### Comparing `rdkit_to_params-1.2.4/rdkit_to_params.egg-info/SOURCES.txt` & `rdkit_to_params-1.2.5/rdkit_to_params.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rdkit_to_params-1.2.4/setup.py` & `rdkit_to_params-1.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ########################################################################################################################
 __doc__ = 'README.md'
 __author__ = "Matteo Ferla"
 __url__ = "https://github.com/matteoferla/rdkit_to_params"
 __email__ = "matteo.ferla@gmail.com"
 __date__ = "29 January 2021 A.D."
 __license__ = "MIT"
-__version__ = "1.2.4"
+__version__ = "1.2.5"
 __citation__ = "https://advances.sciencemag.org/content/7/16/eabf8711 (Fragmenstein)"
 
 # ---------- imports  --------------------------------------------------------------------------------------------------
 # remember it's `python setup.py sdist` and `python -m twine upload dist/rdkit_to_params-1.0.5.tar.gz`
 
 from setuptools import setup, find_packages
 from warnings import warn
```

### Comparing `rdkit_to_params-1.2.4/tests/__init__.py` & `rdkit_to_params-1.2.5/tests/__init__.py`

 * *Files identical despite different names*

