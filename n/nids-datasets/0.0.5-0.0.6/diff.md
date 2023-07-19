# Comparing `tmp/nids_datasets-0.0.5.tar.gz` & `tmp/nids_datasets-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nids_datasets-0.0.5.tar", last modified: Tue Jul 18 17:26:24 2023, max compression
+gzip compressed data, was "nids_datasets-0.0.6.tar", last modified: Tue Jul 18 17:47:28 2023, max compression
```

## Comparing `nids_datasets-0.0.5.tar` & `nids_datasets-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-18 17:26:24.867790 nids_datasets-0.0.5/
--rw-r--r--   0 rdp        (501) staff       (20)      515 2023-07-18 17:26:24.867555 nids_datasets-0.0.5/PKG-INFO
--rw-r--r--   0 rdp        (501) staff       (20)        0 2023-07-17 06:06:29.000000 nids_datasets-0.0.5/README.md
-drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-18 17:26:24.866478 nids_datasets-0.0.5/nids_datasets/
--rw-r--r--   0 rdp        (501) staff       (20)       41 2023-07-17 06:28:22.000000 nids_datasets-0.0.5/nids_datasets/__init__.py
--rw-r--r--   0 rdp        (501) staff       (20)    12810 2023-07-18 17:19:50.000000 nids_datasets-0.0.5/nids_datasets/dataset.py
-drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-18 17:26:24.867348 nids_datasets-0.0.5/nids_datasets.egg-info/
--rw-r--r--   0 rdp        (501) staff       (20)      515 2023-07-18 17:26:24.000000 nids_datasets-0.0.5/nids_datasets.egg-info/PKG-INFO
--rw-r--r--   0 rdp        (501) staff       (20)      253 2023-07-18 17:26:24.000000 nids_datasets-0.0.5/nids_datasets.egg-info/SOURCES.txt
--rw-r--r--   0 rdp        (501) staff       (20)        1 2023-07-18 17:26:24.000000 nids_datasets-0.0.5/nids_datasets.egg-info/dependency_links.txt
--rw-r--r--   0 rdp        (501) staff       (20)      117 2023-07-18 17:26:24.000000 nids_datasets-0.0.5/nids_datasets.egg-info/requires.txt
--rw-r--r--   0 rdp        (501) staff       (20)       14 2023-07-18 17:26:24.000000 nids_datasets-0.0.5/nids_datasets.egg-info/top_level.txt
--rw-r--r--   0 rdp        (501) staff       (20)       38 2023-07-18 17:26:24.867840 nids_datasets-0.0.5/setup.cfg
--rw-r--r--   0 rdp        (501) staff       (20)      889 2023-07-18 17:26:11.000000 nids_datasets-0.0.5/setup.py
+drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-18 17:47:28.812922 nids_datasets-0.0.6/
+-rw-r--r--   0 rdp        (501) staff       (20)      515 2023-07-18 17:47:28.812672 nids_datasets-0.0.6/PKG-INFO
+-rw-r--r--   0 rdp        (501) staff       (20)        0 2023-07-17 06:06:29.000000 nids_datasets-0.0.6/README.md
+drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-18 17:47:28.811406 nids_datasets-0.0.6/nids_datasets/
+-rw-r--r--   0 rdp        (501) staff       (20)       41 2023-07-17 06:28:22.000000 nids_datasets-0.0.6/nids_datasets/__init__.py
+-rw-r--r--   0 rdp        (501) staff       (20)    12831 2023-07-18 17:46:45.000000 nids_datasets-0.0.6/nids_datasets/dataset.py
+drwxr-xr-x   0 rdp        (501) staff       (20)        0 2023-07-18 17:47:28.812461 nids_datasets-0.0.6/nids_datasets.egg-info/
+-rw-r--r--   0 rdp        (501) staff       (20)      515 2023-07-18 17:47:28.000000 nids_datasets-0.0.6/nids_datasets.egg-info/PKG-INFO
+-rw-r--r--   0 rdp        (501) staff       (20)      253 2023-07-18 17:47:28.000000 nids_datasets-0.0.6/nids_datasets.egg-info/SOURCES.txt
+-rw-r--r--   0 rdp        (501) staff       (20)        1 2023-07-18 17:47:28.000000 nids_datasets-0.0.6/nids_datasets.egg-info/dependency_links.txt
+-rw-r--r--   0 rdp        (501) staff       (20)      117 2023-07-18 17:47:28.000000 nids_datasets-0.0.6/nids_datasets.egg-info/requires.txt
+-rw-r--r--   0 rdp        (501) staff       (20)       14 2023-07-18 17:47:28.000000 nids_datasets-0.0.6/nids_datasets.egg-info/top_level.txt
+-rw-r--r--   0 rdp        (501) staff       (20)       38 2023-07-18 17:47:28.812971 nids_datasets-0.0.6/setup.cfg
+-rw-r--r--   0 rdp        (501) staff       (20)      889 2023-07-18 17:47:17.000000 nids_datasets-0.0.6/setup.py
```

### Comparing `nids_datasets-0.0.5/PKG-INFO` & `nids_datasets-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nids_datasets
-Version: 0.0.5
+Version: 0.0.6
 Summary: Download UNSW-NB15 and CIC-IDS2017 Datasets for Network Intrusion Detection (NIDS)
 Home-page: https://github.com/rdpahalavan/BERTSimilarWords
 Author: Pahalavan R D
 Author-email: rdpahalavan24@gmail.com
 License: MIT
 Keywords: Dataset NIDS
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nids_datasets-0.0.5/nids_datasets/dataset.py` & `nids_datasets-0.0.6/nids_datasets/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 import pandas as pd
 from datasets import load_dataset
 from huggingface_hub import hf_hub_download, snapshot_download
 try:
     ipython = get_ipython()
-    from tqdm.notebook import tqdm
+    from tqdm.notebook import tqdm as tqdmn
 except:
-    from tqdm import tqdm
+    from tqdm import tqdm as tqdmn
 
 
 def DatasetInfo(dataset):
     UNSW_NB15_INFO = '{"normal": {"1": 9597932, "2": 9771699, "3": 9980200, "4": 9979823, "5": 9982881, "6": 9983244, "7": 9984416, "8": 9986659, "9": 9987598, "10": 9672644, "11": 9625429, "12": 9583173, "13": 9618777, "14": 9636038, "15": 9643297, "16": 9623646, "17": 9584978, "18": 9403900}, "exploits": {"1": 219231, "2": 121153, "3": 0, "4": 0, "5": 0, "6": 0, "7": 0, "8": 0, "9": 0, "10": 208672, "11": 216055, "12": 231463, "13": 226910, "14": 199265, "15": 222618, "16": 216629, "17": 231583, "18": 217538}, "dos": {"1": 66031, "2": 33817, "3": 0, "4": 0, "5": 0, "6": 0, "7": 0, "8": 0, "9": 0, "10": 46811, "11": 69137, "12": 71735, "13": 57220, "14": 72111, "15": 44221, "16": 70959, "17": 73005, "18": 46603}, "fuzzers": {"1": 61609, "2": 17397, "3": 0, "4": 0, "5": 0, "6": 0, "7": 0, "8": 0, "9": 0, "10": 26704, "11": 38687, "12": 42034, "13": 44183, "14": 40441, "15": 32462, "16": 38901, "17": 44524, "18": 34134}, "generic": {"1": 28211, "2": 17799, "3": 0, "4": 0, "5": 0, "6": 0, "7": 0, "8": 0, "9": 0, "10": 25510, "11": 29047, "12": 36914, "13": 29415, "14": 28263, "15": 33660, "16": 28577, "17": 41717, "18": 33750}, "reconnaissance": {"1": 12572, "2": 6820, "3": 0, "4": 0, "5": 0, "6": 0, "7": 0, "8": 0, "9": 0, "10": 12166, "11": 13541, "12": 24232, "13": 14069, "14": 13001, "15": 13400, "16": 12487, "17": 13645, "18": 14262}, "worms": {"1": 1732, "2": 324, "3": 0, "4": 0, "5": 0, "6": 0, "7": 0, "8": 0, "9": 0, "10": 1168, "11": 1298, "12": 1214, "13": 1688, "14": 1202, "15": 878, "16": 1780, "17": 1490, "18": 858}, "shellcode": {"1": 1459, "2": 598, "3": 0, "4": 0, "5": 0, "6": 0, "7": 0, "8": 0, "9": 0, "10": 1262, "11": 1306, "12": 1434, "13": 1396, "14": 1272, "15": 1300, "16": 1332, "17": 1268, "18": 1356}, "backdoor": {"1": 953, "2": 572, "3": 0, "4": 0, "5": 0, "6": 0, "7": 0, "8": 0, "9": 0, "10": 1418, "11": 1263, "12": 1688, "13": 1809, "14": 1427, "15": 1928, "16": 1473, "17": 1821, "18": 1932}, "analysis": {"1": 388, "2": 1086, "3": 0, "4": 0, "5": 0, "6": 0, "7": 0, "8": 0, "9": 0, "10": 478, "11": 1520, "12": 2024, "13": 436, "14": 1784, "15": 2224, "16": 650, "17": 2009, "18": 1476}, "total": {"1": 9990118, "2": 9971265, "3": 9980200, "4": 9979823, "5": 9982881, "6": 9983244, "7": 9984416, "8": 9986659, "9": 9987598, "10": 9996833, "11": 9997283, "12": 9995911, "13": 9995903, "14": 9994804, "15": 9995988, "16": 9996434, "17": 9996040, "18": 9755809}}'
     CIC_IDS2017_INFO = '{"BENIGN": {"1": 4822905, "2": 3571097, "3": 3556526, "4": 2575904, "5": 3007086, "6": 2637797, "7": 2612615, "8": 2649076, "9": 2948428, "10": 422225, "11": 4418585, "12": 2651388, "13": 3109436, "14": 2845250, "15": 2558990, "16": 3182740, "17": 1920222, "18": 528653}, "FTP-Patator": {"1": 0, "2": 0, "3": 1953, "4": 12803, "5": 68205, "6": 28602, "7": 0, "8": 0, "9": 0, "10": 0, "11": 0, "12": 0, "13": 0, "14": 0, "15": 0, "16": 0, "17": 0, "18": 0}, "SSH-Patator": {"1": 0, "2": 0, "3": 0, "4": 0, "5": 0, "6": 38680, "7": 124631, "8": 0, "9": 0, "10": 0, "11": 0, "12": 0, "13": 0, "14": 0, "15": 0, "16": 0, "17": 0, "18": 0}, "DoS slowloris": {"1": 0, "2": 0, "3": 0, "4": 0, "5": 0, "6": 0, "7": 0, "8": 0, "9": 47519, "10": 0, "11": 41, "12": 0, "13": 0, "14": 0, "15": 0, "16": 0, "17": 0, "18": 0}, "DoS Slowhttptest": {"1": 0, "2": 0, "3": 0, "4": 0, "5": 0, "6": 0, "7": 0, "8": 0, "9": 19866, "10": 19675, "11": 0, "12": 0, "13": 0, "14": 0, "15": 0, "16": 0, "17": 0, "18": 0}, "DoS Hulk": {"1": 0, "2": 0, "3": 0, "4": 0, "5": 0, "6": 0, "7": 0, "8": 0, "9": 0, "10": 1459567, "11": 786683, "12": 0, "13": 0, "14": 0, "15": 0, "16": 0, "17": 0, "18": 0}, "Heartbleed": {"1": 0, "2": 0, "3": 0, "4": 0, "5": 0, "6": 0, "7": 0, "8": 0, "9": 0, "10": 0, "11": 49296, "12": 0, "13": 0, "14": 0, "15": 0, "16": 0, "17": 0, "18": 0}, "Web Attack \\u2013 Brute Force": {"1": 0, "2": 0, "3": 0, "4": 0, "5": 0, "6": 0, "7": 0, "8": 0, "9": 0, "10": 0, "11": 0, "12": 12370, "13": 17873, "14": 0, "15": 0, "16": 0, "17": 0, "18": 0}, "Web Attack \\u2013 XSS": {"1": 0, "2": 0, "3": 0, "4": 0, "5": 0, "6": 0, "7": 0, "8": 0, "9": 0, "10": 0, "11": 0, "12": 0, "13": 9344, "14": 0, "15": 0, "16": 0, "17": 0, "18": 0}, "Web Attack \\u2013 SQL Injection": {"1": 0, "2": 0, "3": 0, "4": 0, "5": 0, "6": 0, "7": 0, "8": 0, "9": 0, "10": 0, "11": 0, "12": 0, "13": 126, "14": 0, "15": 0, "16": 0, "17": 0, "18": 0}, "Infiltration": {"1": 0, "2": 0, "3": 0, "4": 0, "5": 0, "6": 0, "7": 0, "8": 0, "9": 0, "10": 0, "11": 0, "12": 0, "13": 0, "14": 59754, "15": 0, "16": 0, "17": 0, "18": 0}, "Bot": {"1": 0, "2": 0, "3": 0, "4": 0, "5": 0, "6": 0, "7": 0, "8": 0, "9": 0, "10": 0, "11": 0, "12": 0, "13": 0, "14": 0, "15": 0, "16": 12853, "17": 0, "18": 0}, "PortScan": {"1": 0, "2": 0, "3": 0, "4": 0, "5": 0, "6": 0, "7": 0, "8": 0, "9": 0, "10": 0, "11": 0, "12": 0, "13": 0, "14": 0, "15": 0, "16": 45, "17": 321386, "18": 0}, "DDoS": {"1": 0, "2": 0, "3": 0, "4": 0, "5": 0, "6": 0, "7": 0, "8": 0, "9": 0, "10": 0, "11": 0, "12": 0, "13": 0, "14": 0, "15": 0, "16": 0, "17": 942879, "18": 289211}, "normal": {"1": 0, "2": 0, "3": 0, "4": 0, "5": 0, "6": 0, "7": 0, "8": 0, "9": 0, "10": 0, "11": 0, "12": 0, "13": 0, "14": 0, "15": 0, "16": 0, "17": 0, "18": 0}, "exploits": {"1": 0, "2": 0, "3": 0, "4": 0, "5": 0, "6": 0, "7": 0, "8": 0, "9": 0, "10": 0, "11": 0, "12": 0, "13": 0, "14": 0, "15": 0, "16": 0, "17": 0, "18": 0}, "dos": {"1": 0, "2": 0, "3": 0, "4": 0, "5": 0, "6": 0, "7": 0, "8": 0, "9": 0, "10": 0, "11": 0, "12": 0, "13": 0, "14": 0, "15": 0, "16": 0, "17": 0, "18": 0}, "fuzzers": {"1": 0, "2": 0, "3": 0, "4": 0, "5": 0, "6": 0, "7": 0, "8": 0, "9": 0, "10": 0, "11": 0, "12": 0, "13": 0, "14": 0, "15": 0, "16": 0, "17": 0, "18": 0}, "generic": {"1": 0, "2": 0, "3": 0, "4": 0, "5": 0, "6": 0, "7": 0, "8": 0, "9": 0, "10": 0, "11": 0, "12": 0, "13": 0, "14": 0, "15": 0, "16": 0, "17": 0, "18": 0}, "reconnaissance": {"1": 0, "2": 0, "3": 0, "4": 0, "5": 0, "6": 0, "7": 0, "8": 0, "9": 0, "10": 0, "11": 0, "12": 0, "13": 0, "14": 0, "15": 0, "16": 0, "17": 0, "18": 0}, "worms": {"1": 0, "2": 0, "3": 0, "4": 0, "5": 0, "6": 0, "7": 0, "8": 0, "9": 0, "10": 0, "11": 0, "12": 0, "13": 0, "14": 0, "15": 0, "16": 0, "17": 0, "18": 0}, "shellcode": {"1": 0, "2": 0, "3": 0, "4": 0, "5": 0, "6": 0, "7": 0, "8": 0, "9": 0, "10": 0, "11": 0, "12": 0, "13": 0, "14": 0, "15": 0, "16": 0, "17": 0, "18": 0}, "backdoor": {"1": 0, "2": 0, "3": 0, "4": 0, "5": 0, "6": 0, "7": 0, "8": 0, "9": 0, "10": 0, "11": 0, "12": 0, "13": 0, "14": 0, "15": 0, "16": 0, "17": 0, "18": 0}, "analysis": {"1": 0, "2": 0, "3": 0, "4": 0, "5": 0, "6": 0, "7": 0, "8": 0, "9": 0, "10": 0, "11": 0, "12": 0, "13": 0, "14": 0, "15": 0, "16": 0, "17": 0, "18": 0}, "DoS GoldenEye": {"1": 0, "2": 0, "3": 0, "4": 0, "5": 0, "6": 0, "7": 0, "8": 0, "9": 0, "10": 0, "11": 104513, "12": 0, "13": 0, "14": 0, "15": 0, "16": 0, "17": 0, "18": 0}, "total": {"1": 4822905, "2": 3571097, "3": 3558479, "4": 2588707, "5": 3075291, "6": 2705079, "7": 2737246, "8": 2649076, "9": 3015813, "10": 1901467, "11": 5359118, "12": 2663758, "13": 3136779, "14": 2905004, "15": 2558990, "16": 3195638, "17": 3184487, "18": 817864}}'
     if dataset=='UNSW-NB15':
         df = pd.DataFrame(eval(UNSW_NB15_INFO))
@@ -57,17 +57,17 @@
             files = self.files
         on_columns = ['packet_id', 'flow_id', 'source_ip', 'source_port', 'destination_ip', 'destination_port',
                       'protocol', 'attack_label']
         if 'Network-Flows' in subset:
             flow_df = pd.read_parquet(f"{self.dataset}/Network-Flows/{self.flow_file}.parquet")
             flow_df.drop(columns=on_columns[2:], inplace=True)
         os.makedirs(f"{self.dataset}/{'+'.join(subset)}", exist_ok=True)
-        for file in tqdm(files, desc='Merging Files'):
+        for file in tqdmn(files, desc='Merging Files'):
             k = 0
-            for sub in tqdm(subset, desc='Merging Subsets'):
+            for sub in tqdmn(subset, desc='Merging Subsets'):
                 if sub != 'Network-Flows':
                     if k == 0:
                         df = pd.read_parquet(f"{self.dataset}/{sub}/{sub.replace('-', '_')}_File_{file}.parquet")
                     else:
                         df = df.merge(
                             pd.read_parquet(f"{self.dataset}/{sub}/{sub.replace('-', '_')}_File_{file}.parquet"),
                             how='inner', on=on_columns)
@@ -87,15 +87,15 @@
         if files is None:
             files = self.files
         if packet:
             col_name = "packet_hex"
         elif payload:
             col_name = "payload_hex"
         os.makedirs(f"{self.dataset}/{col_name.split('_')[0].capitalize()}-Bytes-{max_bytes}", exist_ok=True)
-        for file in tqdm(files, desc='Extracting Bytes'):
+        for file in tqdmn(files, desc='Extracting Bytes'):
             df = pd.read_parquet(f"{self.dataset}/Packet-Fields/Packet_Fields_File_{file}.parquet")
             df = df.dropna(subset=col_name)
             df.reset_index(drop=True, inplace=True)
             dec_data = df[col_name].apply(lambda x: self._hex_to_dec(str(x)[:int(max_bytes * 2)]))
             max_len = dec_data.apply(len).max()
             df_final = pd.DataFrame(dec_data.tolist(),
                                     columns=[f"{col_name.split('_')[0]}_byte_{i}" for i in range(1, max_len + 1)])
```

### Comparing `nids_datasets-0.0.5/nids_datasets.egg-info/PKG-INFO` & `nids_datasets-0.0.6/nids_datasets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nids-datasets
-Version: 0.0.5
+Version: 0.0.6
 Summary: Download UNSW-NB15 and CIC-IDS2017 Datasets for Network Intrusion Detection (NIDS)
 Home-page: https://github.com/rdpahalavan/BERTSimilarWords
 Author: Pahalavan R D
 Author-email: rdpahalavan24@gmail.com
 License: MIT
 Keywords: Dataset NIDS
 Classifier: Programming Language :: Python :: 3
```

### Comparing `nids_datasets-0.0.5/setup.py` & `nids_datasets-0.0.6/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = f.read().splitlines()
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name='nids_datasets',
-    version='0.0.5',
+    version='0.0.6',
     description="Download UNSW-NB15 and CIC-IDS2017 Datasets for Network Intrusion Detection (NIDS)",
     keywords="Dataset NIDS",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
     author="Pahalavan R D",
     author_email='rdpahalavan24@gmail.com',
```

