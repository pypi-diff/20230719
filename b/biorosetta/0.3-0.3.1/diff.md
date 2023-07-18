# Comparing `tmp/biorosetta-0.3.tar.gz` & `tmp/biorosetta-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biorosetta-0.3.tar", last modified: Tue Mar 28 18:52:39 2023, max compression
+gzip compressed data, was "biorosetta-0.3.1.tar", last modified: Tue Jul 18 23:01:57 2023, max compression
```

## Comparing `biorosetta-0.3.tar` & `biorosetta-0.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 reema      (502) staff       (20)        0 2023-03-28 18:52:39.360830 biorosetta-0.3/
--rw-r--r--   0 reema      (502) staff       (20)     1071 2022-12-29 20:58:47.000000 biorosetta-0.3/LICENSE
--rw-r--r--   0 reema      (502) staff       (20)       23 2023-01-24 19:39:30.000000 biorosetta-0.3/MANIFEST.in
--rw-r--r--   0 reema      (502) staff       (20)     3172 2023-03-28 18:52:39.360310 biorosetta-0.3/PKG-INFO
--rw-r--r--   0 reema      (502) staff       (20)    11846 2023-03-28 18:10:03.000000 biorosetta-0.3/README.md
--rw-r--r--   0 reema      (502) staff       (20)     2859 2023-01-24 19:33:26.000000 biorosetta-0.3/README_pypi.md
-drwxr-xr-x   0 reema      (502) staff       (20)        0 2023-03-28 18:52:39.355272 biorosetta-0.3/biorosetta/
--rw-r--r--   0 reema      (502) staff       (20)     1386 2023-02-12 23:45:42.000000 biorosetta-0.3/biorosetta/__init__.py
--rw-r--r--   0 reema      (502) staff       (20)    16420 2023-03-28 18:07:20.000000 biorosetta-0.3/biorosetta/classes.py
--rw-r--r--   0 reema      (502) staff       (20)     1203 2023-01-19 01:03:09.000000 biorosetta-0.3/biorosetta/queries.py
--rw-r--r--   0 reema      (502) staff       (20)     2474 2023-02-20 21:10:18.000000 biorosetta-0.3/biorosetta/utils.py
-drwxr-xr-x   0 reema      (502) staff       (20)        0 2023-03-28 18:52:39.359499 biorosetta-0.3/biorosetta.egg-info/
--rw-r--r--   0 reema      (502) staff       (20)     3172 2023-03-28 18:52:39.000000 biorosetta-0.3/biorosetta.egg-info/PKG-INFO
--rw-r--r--   0 reema      (502) staff       (20)      309 2023-03-28 18:52:39.000000 biorosetta-0.3/biorosetta.egg-info/SOURCES.txt
--rw-r--r--   0 reema      (502) staff       (20)        1 2023-03-28 18:52:39.000000 biorosetta-0.3/biorosetta.egg-info/dependency_links.txt
--rw-r--r--   0 reema      (502) staff       (20)       29 2023-03-28 18:52:39.000000 biorosetta-0.3/biorosetta.egg-info/requires.txt
--rw-r--r--   0 reema      (502) staff       (20)       11 2023-03-28 18:52:39.000000 biorosetta-0.3/biorosetta.egg-info/top_level.txt
--rw-r--r--   0 reema      (502) staff       (20)       38 2023-03-28 18:52:39.360954 biorosetta-0.3/setup.cfg
--rw-r--r--   0 reema      (502) staff       (20)      722 2023-03-28 18:52:26.000000 biorosetta-0.3/setup.py
+drwxr-xr-x   0 enricomaiorino   (503) staff       (20)        0 2023-07-18 23:01:57.207154 biorosetta-0.3.1/
+-rwxrwxrwx   0 enricomaiorino   (503) staff       (20)     1071 2022-12-29 20:58:47.000000 biorosetta-0.3.1/LICENSE
+-rwxrwxrwx   0 enricomaiorino   (503) staff       (20)       23 2023-01-24 19:39:30.000000 biorosetta-0.3.1/MANIFEST.in
+-rw-r--r--   0 enricomaiorino   (503) staff       (20)     3190 2023-07-18 23:01:57.207048 biorosetta-0.3.1/PKG-INFO
+-rwxrwxrwx   0 enricomaiorino   (503) staff       (20)    11846 2023-03-28 18:10:03.000000 biorosetta-0.3.1/README.md
+-rwxrwxrwx   0 enricomaiorino   (503) staff       (20)     2875 2023-07-18 22:39:52.000000 biorosetta-0.3.1/README_pypi.md
+drwxr-xr-x   0 enricomaiorino   (503) staff       (20)        0 2023-07-18 23:01:57.206061 biorosetta-0.3.1/biorosetta/
+-rwxrwxrwx   0 enricomaiorino   (503) staff       (20)     1386 2023-02-12 23:45:42.000000 biorosetta-0.3.1/biorosetta/__init__.py
+-rwxrwxrwx   0 enricomaiorino   (503) staff       (20)    16418 2023-07-18 22:41:27.000000 biorosetta-0.3.1/biorosetta/classes.py
+-rwxrwxrwx   0 enricomaiorino   (503) staff       (20)     1203 2023-01-19 01:03:09.000000 biorosetta-0.3.1/biorosetta/queries.py
+-rwxrwxrwx   0 enricomaiorino   (503) staff       (20)     2474 2023-02-20 21:10:18.000000 biorosetta-0.3.1/biorosetta/utils.py
+drwxr-xr-x   0 enricomaiorino   (503) staff       (20)        0 2023-07-18 23:01:57.206863 biorosetta-0.3.1/biorosetta.egg-info/
+-rwxrwxrwx   0 enricomaiorino   (503) staff       (20)     3190 2023-07-18 23:01:57.000000 biorosetta-0.3.1/biorosetta.egg-info/PKG-INFO
+-rwxrwxrwx   0 enricomaiorino   (503) staff       (20)      309 2023-07-18 23:01:57.000000 biorosetta-0.3.1/biorosetta.egg-info/SOURCES.txt
+-rwxrwxrwx   0 enricomaiorino   (503) staff       (20)        1 2023-07-18 23:01:57.000000 biorosetta-0.3.1/biorosetta.egg-info/dependency_links.txt
+-rwxrwxrwx   0 enricomaiorino   (503) staff       (20)       29 2023-07-18 23:01:57.000000 biorosetta-0.3.1/biorosetta.egg-info/requires.txt
+-rwxrwxrwx   0 enricomaiorino   (503) staff       (20)       11 2023-07-18 23:01:57.000000 biorosetta-0.3.1/biorosetta.egg-info/top_level.txt
+-rw-r--r--   0 enricomaiorino   (503) staff       (20)       38 2023-07-18 23:01:57.207202 biorosetta-0.3.1/setup.cfg
+-rwxrwxrwx   0 enricomaiorino   (503) staff       (20)      724 2023-07-18 22:40:01.000000 biorosetta-0.3.1/setup.py
```

### Comparing `biorosetta-0.3/LICENSE` & `biorosetta-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `biorosetta-0.3/PKG-INFO` & `biorosetta-0.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biorosetta
-Version: 0.3
+Version: 0.3.1
 Summary: A package to convert gene identifiers between different naming conventions
 Home-page: https://github.com/reemagit/biorosetta
 Author: Enrico Maiorino
 Author-email: enrico.maiorino@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -40,9 +40,9 @@
 - "entr": NCBI gene ID (entrezgene, all sources)
 - "symb": Gene name (symbol, all sources)
 - "ensp": Ensembl protein ID (ENSP, Ensembl Biomart only)
 - "hgnc": HGNC ID (Ensembl Biomart and HGNC Biomart only)
 
 ## Usage
 
-See up-to-date documentation and examples at [github repo](https://www.google.com).
+See up-to-date documentation and examples at [github repo](https://github.com/reemagit/biorosetta).
```

### Comparing `biorosetta-0.3/README.md` & `biorosetta-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `biorosetta-0.3/README_pypi.md` & `biorosetta-0.3.1/README_pypi.md`

 * *Files 2% similar despite different names*

```diff
@@ -30,9 +30,9 @@
 - "entr": NCBI gene ID (entrezgene, all sources)
 - "symb": Gene name (symbol, all sources)
 - "ensp": Ensembl protein ID (ENSP, Ensembl Biomart only)
 - "hgnc": HGNC ID (Ensembl Biomart and HGNC Biomart only)
 
 ## Usage
 
-See up-to-date documentation and examples at [github repo](https://www.google.com).
+See up-to-date documentation and examples at [github repo](https://github.com/reemagit/biorosetta).
```

### Comparing `biorosetta-0.3/biorosetta/__init__.py` & `biorosetta-0.3.1/biorosetta/__init__.py`

 * *Files identical despite different names*

### Comparing `biorosetta-0.3/biorosetta/classes.py` & `biorosetta-0.3.1/biorosetta/classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -338,15 +338,15 @@
 		id_list = make_list(id_list)
 		src_ids = [src_id for src_id, src in zip(self._src_ids, self._sources) if src.has_id_in_type(id_in) and src.has_id_out_type(id_out)]
 		if len(src_ids) < len(self._src_ids):
 			print('One or more sources do not support the requested input/output ID type mapping: {}'.format(','.join(src_id for src_id in self._src_ids if src_id not in src_ids)))
 			print('Mapping will be executed using the following source(s): {}'.format(','.join(src_ids)))
 		if len(src_ids) == 0:
 			raise ValueError('Input or output ID type not supported by selected sources')
-		out_df = pd.DataFrame([], columns=[src_ids])
+		out_df = pd.DataFrame([], columns=src_ids)
 		out_df['input'] = id_list
 		for src_id in src_ids:
 			out_df[src_id] = self.get_source(src_id).convert(id_list, id_in, id_out, multi_hits='all' if multi_hits == 'consensus' else multi_hits, df=False)
 
 		if multi_hits == 'consensus':
 			def get_consensus(x):
 				if (x != self._fill_value).sum() > 0:
```

### Comparing `biorosetta-0.3/biorosetta/queries.py` & `biorosetta-0.3.1/biorosetta/queries.py`

 * *Files identical despite different names*

### Comparing `biorosetta-0.3/biorosetta/utils.py` & `biorosetta-0.3.1/biorosetta/utils.py`

 * *Files identical despite different names*

### Comparing `biorosetta-0.3/biorosetta.egg-info/PKG-INFO` & `biorosetta-0.3.1/biorosetta.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biorosetta
-Version: 0.3
+Version: 0.3.1
 Summary: A package to convert gene identifiers between different naming conventions
 Home-page: https://github.com/reemagit/biorosetta
 Author: Enrico Maiorino
 Author-email: enrico.maiorino@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -40,9 +40,9 @@
 - "entr": NCBI gene ID (entrezgene, all sources)
 - "symb": Gene name (symbol, all sources)
 - "ensp": Ensembl protein ID (ENSP, Ensembl Biomart only)
 - "hgnc": HGNC ID (Ensembl Biomart and HGNC Biomart only)
 
 ## Usage
 
-See up-to-date documentation and examples at [github repo](https://www.google.com).
+See up-to-date documentation and examples at [github repo](https://github.com/reemagit/biorosetta).
```

### Comparing `biorosetta-0.3/setup.py` & `biorosetta-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README_pypi.md").read_text()
 
 setup(
 	name='biorosetta',
-	version='0.3',
+	version='0.3.1',
 	#packages=find_packages(include=['classes','queries','utils']),
 	packages=['biorosetta'],
 	url='https://github.com/reemagit/biorosetta',
 	author='Enrico Maiorino',
 	author_email='enrico.maiorino@gmail.com',
 	description='A package to convert gene identifiers between different naming conventions',
 	install_requires=['biothings_client','tqdm','pandas'],
```

