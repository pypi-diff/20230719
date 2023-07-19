# Comparing `tmp/piezo-0.5.tar.gz` & `tmp/piezo-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piezo-0.5.tar", last modified: Thu Jun 29 15:52:33 2023, max compression
+gzip compressed data, was "piezo-0.6.tar", last modified: Wed Jul 19 11:20:16 2023, max compression
```

## Comparing `piezo-0.5.tar` & `piezo-0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:52:33.199128 piezo-0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-06-29 15:52:03.000000 piezo-0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-06-29 15:52:33.199128 piezo-0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-06-29 15:52:03.000000 piezo-0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-29 15:52:03.000000 piezo-0.5/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:52:33.195128 piezo-0.5/bin/
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-29 15:52:03.000000 piezo-0.5/bin/piezo-predict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:52:33.195128 piezo-0.5/piezo/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-29 15:52:03.000000 piezo-0.5/piezo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-06-29 15:52:03.000000 piezo-0.5/piezo/catalogue.py
--rw-r--r--   0 runner    (1001) docker     (123)    33912 2023-06-29 15:52:03.000000 piezo-0.5/piezo/grammar_GARC1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:52:33.199128 piezo-0.5/piezo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-06-29 15:52:33.000000 piezo-0.5/piezo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-29 15:52:33.000000 piezo-0.5/piezo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 15:52:33.000000 piezo-0.5/piezo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 15:52:12.000000 piezo-0.5/piezo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-29 15:52:33.000000 piezo-0.5/piezo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 15:52:33.000000 piezo-0.5/piezo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-29 15:52:03.000000 piezo-0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-29 15:52:33.199128 piezo-0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:52:33.199128 piezo-0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    14266 2023-06-29 15:52:03.000000 piezo-0.5/tests/test_catalogue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:20:16.852744 piezo-0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-07-19 11:19:49.000000 piezo-0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-07-19 11:20:16.852744 piezo-0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-07-19 11:19:49.000000 piezo-0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-19 11:19:49.000000 piezo-0.6/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:20:16.852744 piezo-0.6/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-19 11:19:49.000000 piezo-0.6/bin/piezo-predict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:20:16.852744 piezo-0.6/piezo/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-19 11:19:49.000000 piezo-0.6/piezo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-07-19 11:19:49.000000 piezo-0.6/piezo/catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33985 2023-07-19 11:19:49.000000 piezo-0.6/piezo/grammar_GARC1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:20:16.852744 piezo-0.6/piezo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-07-19 11:20:16.000000 piezo-0.6/piezo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-19 11:20:16.000000 piezo-0.6/piezo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 11:20:16.000000 piezo-0.6/piezo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 11:19:55.000000 piezo-0.6/piezo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-19 11:20:16.000000 piezo-0.6/piezo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-19 11:20:16.000000 piezo-0.6/piezo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-19 11:19:49.000000 piezo-0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-19 11:20:16.852744 piezo-0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 11:20:16.852744 piezo-0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    14266 2023-07-19 11:19:49.000000 piezo-0.6/tests/test_catalogue.py
```

### Comparing `piezo-0.5/LICENSE` & `piezo-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `piezo-0.5/PKG-INFO` & `piezo-0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piezo
-Version: 0.5
+Version: 0.6
 Summary: Predicting the effect of an antibiotic from gene mutations
 Home-page: https://github.com/oxfordmmm/piezo
 Author: Philip W Fowler
 Author-email: philip.fowler@ndm.ox.ac.uk
 License: University of Oxford, see LICENSE.md
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
```

### Comparing `piezo-0.5/README.md` & `piezo-0.6/README.md`

 * *Files identical despite different names*

### Comparing `piezo-0.5/bin/piezo-predict.py` & `piezo-0.6/bin/piezo-predict.py`

 * *Files identical despite different names*

### Comparing `piezo-0.5/piezo/catalogue.py` & `piezo-0.6/piezo/catalogue.py`

 * *Files identical despite different names*

### Comparing `piezo-0.5/piezo/grammar_GARC1.py` & `piezo-0.6/piezo/grammar_GARC1.py`

 * *Files 0% similar despite different names*

```diff
@@ -552,17 +552,17 @@
     '''
     if mutation_affects == "GENE":
         #Large deletions are priority 1
         large_del(predictions, rules.loc[rules_mutation_type_vector], indel_length, minor)
 
     # PRIORITY 1: any insertion or deletion in the CDS or PROM (e.g. rpoB_*_indel or rpoB_-*_indel)
     if mutation_affects == "CDS":
-        row=rules.loc[rules_mutation_type_vector & (rules.MUTATION=="*_indel")]
+        row=rules.loc[rules_mutation_type_vector & ((rules.MUTATION=="*_indel") | (rules.MUTATION=="*_mixed"))]
     else:
-        row=rules.loc[rules_mutation_type_vector & (rules.MUTATION=="-*_indel")]
+        row=rules.loc[rules_mutation_type_vector & ((rules.MUTATION=="-*_indel") | (rules.MUTATION=="-*mixed"))]
     #any insertion or deletion in the CDS or PROM
     row_prediction(row, predictions, 1, minor)
 
     # PRIORITY 2: rpoB_*_ins, rpoB_*_del any insertion (or deletion) in the CDS or PROM
     if mutation_affects == "CDS":
         row=rules.loc[rules_mutation_type_vector & (rules.MUTATION.isin(["*_ins","*_del"]))]
     else:
@@ -681,15 +681,15 @@
             except ValueError:
                 assert False, "Invalid mutation: " + mutation
             mutation_affects=infer_mutation_affects(position)
 
             # the third element is one of indel, ins, del or the special case fs
             indel_type=cols[1]
 
-            assert indel_type in ['indel','ins','del','fs'], "form of indel not recognised: "+indel_type
+            assert indel_type in ['indel','ins','del','fs', 'mixed'], "form of indel not recognised: "+indel_type
 
             # if there is a fourth and final element to an INDEL it is either _4 or _ctgc
             if len(cols)==3:
                 assert indel_type in ['ins','del'], "form of indel does not make sense when length or bases specified!: "+indel_type
                 try:
                     indel_length=int(cols[2])
                 except:
```

### Comparing `piezo-0.5/piezo.egg-info/PKG-INFO` & `piezo-0.6/piezo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piezo
-Version: 0.5
+Version: 0.6
 Summary: Predicting the effect of an antibiotic from gene mutations
 Home-page: https://github.com/oxfordmmm/piezo
 Author: Philip W Fowler
 Author-email: philip.fowler@ndm.ox.ac.uk
 License: University of Oxford, see LICENSE.md
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
```

### Comparing `piezo-0.5/setup.cfg` & `piezo-0.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `piezo-0.5/tests/test_catalogue.py` & `piezo-0.6/tests/test_catalogue.py`

 * *Files identical despite different names*

