# Comparing `tmp/proteinflow-1.4.1.tar.gz` & `tmp/proteinflow-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteinflow-1.4.1.tar", last modified: Mon Jun 26 12:40:13 2023, max compression
+gzip compressed data, was "proteinflow-2.0.0.tar", last modified: Wed Jul 19 13:48:36 2023, max compression
```

## Comparing `proteinflow-1.4.1.tar` & `proteinflow-2.0.0.tar`

### file list

```diff
@@ -1,36 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:40:12.999473 proteinflow-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-26 12:40:01.000000 proteinflow-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11479 2023-06-26 12:40:12.999473 proteinflow-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11069 2023-06-26 12:40:01.000000 proteinflow-1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:40:12.999473 proteinflow-1.4.1/proteinflow/
--rw-r--r--   0 runner    (1001) docker     (123)    53052 2023-06-26 12:40:01.000000 proteinflow-1.4.1/proteinflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-06-26 12:40:01.000000 proteinflow-1.4.1/proteinflow/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-26 12:40:01.000000 proteinflow-1.4.1/proteinflow/custom_mmcif.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:40:12.999473 proteinflow-1.4.1/proteinflow/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-26 12:40:01.000000 proteinflow-1.4.1/proteinflow/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21978 2023-06-26 12:40:01.000000 proteinflow-1.4.1/proteinflow/pdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    39439 2023-06-26 12:40:01.000000 proteinflow-1.4.1/proteinflow/protein_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-06-26 12:40:01.000000 proteinflow-1.4.1/proteinflow/protein_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:40:12.999473 proteinflow-1.4.1/proteinflow/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 12:40:01.000000 proteinflow-1.4.1/proteinflow/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7881 2023-06-26 12:40:01.000000 proteinflow-1.4.1/proteinflow/scripts/proteinflow_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-06-26 12:40:01.000000 proteinflow-1.4.1/proteinflow/sequences.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:40:12.999473 proteinflow-1.4.1/proteinflow/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 12:40:01.000000 proteinflow-1.4.1/proteinflow/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-06-26 12:40:01.000000 proteinflow-1.4.1/proteinflow/utils/biotite_sse.py
--rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-06-26 12:40:01.000000 proteinflow-1.4.1/proteinflow/utils/boto_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    36950 2023-06-26 12:40:01.000000 proteinflow-1.4.1/proteinflow/utils/cluster_and_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-06-26 12:40:01.000000 proteinflow-1.4.1/proteinflow/utils/common_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:40:12.999473 proteinflow-1.4.1/proteinflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11479 2023-06-26 12:40:12.000000 proteinflow-1.4.1/proteinflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-26 12:40:12.000000 proteinflow-1.4.1/proteinflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 12:40:12.000000 proteinflow-1.4.1/proteinflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-26 12:40:12.000000 proteinflow-1.4.1/proteinflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-26 12:40:12.000000 proteinflow-1.4.1/proteinflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-26 12:40:12.000000 proteinflow-1.4.1/proteinflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-26 12:40:01.000000 proteinflow-1.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-26 12:40:12.999473 proteinflow-1.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:40:12.999473 proteinflow-1.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-06-26 12:40:01.000000 proteinflow-1.4.1/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-06-26 12:40:01.000000 proteinflow-1.4.1/tests/test_generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-06-26 12:40:01.000000 proteinflow-1.4.1/tests/test_sabdab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:48:36.956620 proteinflow-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-19 13:48:25.000000 proteinflow-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11677 2023-07-19 13:48:36.956620 proteinflow-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11267 2023-07-19 13:48:25.000000 proteinflow-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:48:36.952620 proteinflow-2.0.0/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-19 13:48:25.000000 proteinflow-2.0.0/dev/bump_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:48:36.956620 proteinflow-2.0.0/proteinflow/
+-rw-r--r--   0 runner    (1001) docker     (123)    25443 2023-07-19 13:48:25.000000 proteinflow-2.0.0/proteinflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-07-19 13:48:25.000000 proteinflow-2.0.0/proteinflow/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-07-19 13:48:25.000000 proteinflow-2.0.0/proteinflow/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:48:36.956620 proteinflow-2.0.0/proteinflow/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    55531 2023-07-19 13:48:25.000000 proteinflow-2.0.0/proteinflow/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39434 2023-07-19 13:48:25.000000 proteinflow-2.0.0/proteinflow/data/torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16881 2023-07-19 13:48:25.000000 proteinflow-2.0.0/proteinflow/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:48:36.956620 proteinflow-2.0.0/proteinflow/download/
+-rw-r--r--   0 runner    (1001) docker     (123)    20048 2023-07-19 13:48:25.000000 proteinflow-2.0.0/proteinflow/download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-07-19 13:48:25.000000 proteinflow-2.0.0/proteinflow/download/boto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:48:36.956620 proteinflow-2.0.0/proteinflow/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-07-19 13:48:25.000000 proteinflow-2.0.0/proteinflow/logging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:48:36.956620 proteinflow-2.0.0/proteinflow/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-19 13:48:25.000000 proteinflow-2.0.0/proteinflow/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:48:36.956620 proteinflow-2.0.0/proteinflow/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)    16875 2023-07-19 13:48:25.000000 proteinflow-2.0.0/proteinflow/processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:48:36.956620 proteinflow-2.0.0/proteinflow/split/
+-rw-r--r--   0 runner    (1001) docker     (123)    45990 2023-07-19 13:48:25.000000 proteinflow-2.0.0/proteinflow/split/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-07-19 13:48:25.000000 proteinflow-2.0.0/proteinflow/split/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:48:36.956620 proteinflow-2.0.0/proteinflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11677 2023-07-19 13:48:36.000000 proteinflow-2.0.0/proteinflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-19 13:48:36.000000 proteinflow-2.0.0/proteinflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 13:48:36.000000 proteinflow-2.0.0/proteinflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-19 13:48:36.000000 proteinflow-2.0.0/proteinflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-19 13:48:36.000000 proteinflow-2.0.0/proteinflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-19 13:48:36.000000 proteinflow-2.0.0/proteinflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-19 13:48:25.000000 proteinflow-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-19 13:48:36.956620 proteinflow-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:48:36.956620 proteinflow-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-07-19 13:48:25.000000 proteinflow-2.0.0/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-19 13:48:25.000000 proteinflow-2.0.0/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-19 13:48:25.000000 proteinflow-2.0.0/tests/test_generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-19 13:48:25.000000 proteinflow-2.0.0/tests/test_sabdab.py
```

### Comparing `proteinflow-1.4.1/LICENSE` & `proteinflow-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `proteinflow-1.4.1/PKG-INFO` & `proteinflow-2.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proteinflow
-Version: 1.4.1
+Version: 2.0.0
 Summary: Versatile pipeline for processing protein structure data for deep learning applications.
 Author-email: Liza Kozlova <liza@adaptyvbio.com>, Arthur Valentin <arthur@adaptyvbio.com>
 License: BSD-3-Clause
 Keywords: bioinformatics,dataset,protein,PDB,deep learning
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -57,15 +57,15 @@
 docker:
 ```bash
 docker pull adaptyvbio/proteinflow
 ```
 
 ### Troubleshooting
 - If you are using python 3.10 and encountering installation problems, try running `python -m pip install prody==2.4.0` before installing `proteinflow`.
-- If you are planning to generate new datasets and installed `proteinflow` with `pip`, you will need to additionally install [`mmseqs`](https://github.com/soedinglab/MMseqs2).
+- If you are planning to generate new datasets and installed `proteinflow` with `pip` (or with `conda` on Mac OS with an M1 processor), you will need to additionally install [`mmseqs`](https://github.com/soedinglab/MMseqs2).
 - Generating new datasets also depends on the `rcsbsearch` package and the latest release [v0.2.3](https://github.com/sbliven/rcsbsearch/releases/tag/v0.2.3) is currently not working correctly. The recommended fix is installing the version from [this pull request](https://github.com/sbliven/rcsbsearch/pull/6).
 ```bash
 python -m pip install "rcsbsearch @ git+https://github.com/sbliven/rcsbsearch@dbdfe3880cc88b0ce57163987db613d579400c8e"
 ```
 - The docker image can be accessed in interactive mode with this command.
 ```bash
 docker run -it -v /path/to/data:/media adaptyvbio/proteinflow bash
@@ -182,19 +182,20 @@
     ...
 ```
 See more details on available parameters and the data format in the [docs](https://adaptyvbio.github.io/ProteinFlow/) + [this repository](https://github.com/adaptyvbio/ProteinFlow-models) for a use case.
 
 ## ProteinFlow Stable Releases
 You can download them with `proteinflow download --tag {tag}` in the command line or browse in the [interface](https://proteinflow-datasets.s3.eu-west-1.amazonaws.com/index.html).
 
-|Tag    |Date    |Snapshot|Size|Min res|Min len|Max len|MMseqs thr|Split (train/val/test)|Missing thr (ends/middle)|Source|Remove redundancies|Note|
-|-------|--------|--------|----|-------|-------|-------|----------|----------------------|-------------------------|---|---|----|
-|paper|10.11.22|20220103|24G|3.5|30|10'000|0.3|90/5/5|0.3/0.1|PDB|yes|first release, no mmCIF files|
-|20230102_stable|27.02.23|20230102|28G|3.5|30|10'000|0.3|90/5/5|0.3/0.1|PDB|yes|v1.1.1|
-|20230623_sabdab|26.06.23|live 26.06.23|1.2G|3.5|30|10'000|0.3|96/3/1|0.3/0.1|SAbDab|no|v1.4.1|
+|Tag    |Date    |Snapshot|Size|Min res|Min len|Max len|Max chains|MMseqs thr|Split (train/val/test)|Missing thr (ends/middle)|Source|Remove redundancies|Note|
+|-------|--------|--------|----|-------|-------|-------|----------|----------|----------------------|-------------------------|---|---|----------------|
+|paper|10.11.22|20220103|24G|3.5|30|10'000|-|0.3|90/5/5|0.3/0.1|PDB|yes|first release, no mmCIF files|
+|20230102_stable|27.02.23|20230102|28G|3.5|30|10'000|-|0.3|90/5/5|0.3/0.1|PDB|yes|v1.1.1|
+|20230623_sabdab|26.06.23|live 26.06.23|1.4G|3.5|30|10'000|-|0.3|96/3/1|0.5/0.2|SAbDab|no|v1.4.1 (requires >= v1.4.0)|
+|20230102_v200|19.07.23|20230102|33G|3.5|30|10'000|10|0.3|90/5/5|0.3/0.1|PDB|no|v2.0.0|
 
 ## License
 The `proteinflow` package and data are released and distributed under the BSD 3-Clause License
 
 
 ## Contributions
 This is an open source project supported by [Adaptyv Bio](https://www.adaptyvbio.com/). Contributions, suggestions and bug-fixes are welcomed.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: proteinflow Version: 1.4.1 Summary: Versatile
+Metadata-Version: 2.1 Name: proteinflow Version: 2.0.0 Summary: Versatile
 pipeline for processing protein structure data for deep learning applications.
 Author-email: Liza Kozlova
 adaptyvbio.com>, Arthur Valentin
 adaptyvbio.com> License: BSD-3-Clause Keywords:
 bioinformatics,dataset,protein,PDB,deep learning Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE
   ProteinFlow - A data processing pipeline for all your protein design needs
@@ -30,21 +30,22 @@
 raw.githubusercontent.com/adaptyvbio/ProteinFlow/main/media/pf-1.png) --- ##
 Installation conda: ```bash # This should take a few minutes, be patient conda
 install -c conda-forge -c bioconda -c adaptyvbio proteinflow ``` pip: ```bash
 pip install proteinflow ``` docker: ```bash docker pull adaptyvbio/proteinflow
 ``` ### Troubleshooting - If you are using python 3.10 and encountering
 installation problems, try running `python -m pip install prody==2.4.0` before
 installing `proteinflow`. - If you are planning to generate new datasets and
-installed `proteinflow` with `pip`, you will need to additionally install
-[`mmseqs`](https://github.com/soedinglab/MMseqs2). - Generating new datasets
-also depends on the `rcsbsearch` package and the latest release [v0.2.3](https:
-//github.com/sbliven/rcsbsearch/releases/tag/v0.2.3) is currently not working
-correctly. The recommended fix is installing the version from [this pull
-request](https://github.com/sbliven/rcsbsearch/pull/6). ```bash python -m pip
-install "rcsbsearch @ git+https://github.com/sbliven/
+installed `proteinflow` with `pip` (or with `conda` on Mac OS with an M1
+processor), you will need to additionally install [`mmseqs`](https://
+github.com/soedinglab/MMseqs2). - Generating new datasets also depends on the
+`rcsbsearch` package and the latest release [v0.2.3](https://github.com/
+sbliven/rcsbsearch/releases/tag/v0.2.3) is currently not working correctly. The
+recommended fix is installing the version from [this pull request](https://
+github.com/sbliven/rcsbsearch/pull/6). ```bash python -m pip install
+"rcsbsearch @ git+https://github.com/sbliven/
 rcsbsearch@dbdfe3880cc88b0ce57163987db613d579400c8e" ``` - The docker image can
 be accessed in interactive mode with this command. ```bash docker run -it -v /
 path/to/data:/media adaptyvbio/proteinflow bash ``` ## Usage ### Downloading
 pre-computed datasets (stable) Already precomputed datasets with consensus set
 of parameters and can be accessed and downloaded using the `proteinflow`.
 package. Check the output of `proteinflow check_tags` for a list of available
 tags. ```bash proteinflow download --tag 20230102_stable ``` ### Running the
@@ -134,20 +135,20 @@
 #(B, L, 3) to_predict = batch["masked_res"] #(B, L), 1 where the residues
 should be masked, 0 otherwise ... ``` See more details on available parameters
 and the data format in the [docs](https://adaptyvbio.github.io/ProteinFlow/) +
 [this repository](https://github.com/adaptyvbio/ProteinFlow-models) for a use
 case. ## ProteinFlow Stable Releases You can download them with `proteinflow
 download --tag {tag}` in the command line or browse in the [interface](https://
 proteinflow-datasets.s3.eu-west-1.amazonaws.com/index.html). |Tag |Date
-|Snapshot|Size|Min res|Min len|Max len|MMseqs thr|Split (train/val/
+|Snapshot|Size|Min res|Min len|Max len|Max chains|MMseqs thr|Split (train/val/
 test)|Missing thr (ends/middle)|Source|Remove redundancies|Note| |-------|-----
----|--------|----|-------|-------|-------|----------|----------------------|---
-----------------------|---|---|----
-| |paper|10.11.22|20220103|24G|3.5|30|10'000|0.3|90/5/5|0.3/0.1|PDB|yes|first
-release, no mmCIF files|
-|20230102_stable|27.02.23|20230102|28G|3.5|30|10'000|0.3|90/5/5|0.3/
-0.1|PDB|yes|v1.1.1| |20230623_sabdab|26.06.23|live
-26.06.23|1.2G|3.5|30|10'000|0.3|96/3/1|0.3/0.1|SAbDab|no|v1.4.1| ## License The
-`proteinflow` package and data are released and distributed under the BSD 3-
-Clause License ## Contributions This is an open source project supported by
-[Adaptyv Bio](https://www.adaptyvbio.com/). Contributions, suggestions and bug-
-fixes are welcomed.
+---|--------|----|-------|-------|-------|----------|----------|---------------
+-------|-------------------------|---|---|----------------
+| |paper|10.11.22|20220103|24G|3.5|30|10'000|-|0.3|90/5/5|0.3/0.1|PDB|yes|first
+release, no mmCIF files| |20230102_stable|27.02.23|20230102|28G|3.5|30|10'000|-
+|0.3|90/5/5|0.3/0.1|PDB|yes|v1.1.1| |20230623_sabdab|26.06.23|live
+26.06.23|1.4G|3.5|30|10'000|-|0.3|96/3/1|0.5/0.2|SAbDab|no|v1.4.1 (requires >=
+v1.4.0)| |20230102_v200|19.07.23|20230102|33G|3.5|30|10'000|10|0.3|90/5/5|0.3/
+0.1|PDB|no|v2.0.0| ## License The `proteinflow` package and data are released
+and distributed under the BSD 3-Clause License ## Contributions This is an open
+source project supported by [Adaptyv Bio](https://www.adaptyvbio.com/).
+Contributions, suggestions and bug-fixes are welcomed.
```

### Comparing `proteinflow-1.4.1/README.md` & `proteinflow-2.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 docker:
 ```bash
 docker pull adaptyvbio/proteinflow
 ```
 
 ### Troubleshooting
 - If you are using python 3.10 and encountering installation problems, try running `python -m pip install prody==2.4.0` before installing `proteinflow`.
-- If you are planning to generate new datasets and installed `proteinflow` with `pip`, you will need to additionally install [`mmseqs`](https://github.com/soedinglab/MMseqs2).
+- If you are planning to generate new datasets and installed `proteinflow` with `pip` (or with `conda` on Mac OS with an M1 processor), you will need to additionally install [`mmseqs`](https://github.com/soedinglab/MMseqs2).
 - Generating new datasets also depends on the `rcsbsearch` package and the latest release [v0.2.3](https://github.com/sbliven/rcsbsearch/releases/tag/v0.2.3) is currently not working correctly. The recommended fix is installing the version from [this pull request](https://github.com/sbliven/rcsbsearch/pull/6).
 ```bash
 python -m pip install "rcsbsearch @ git+https://github.com/sbliven/rcsbsearch@dbdfe3880cc88b0ce57163987db613d579400c8e"
 ```
 - The docker image can be accessed in interactive mode with this command.
 ```bash
 docker run -it -v /path/to/data:/media adaptyvbio/proteinflow bash
@@ -171,19 +171,20 @@
     ...
 ```
 See more details on available parameters and the data format in the [docs](https://adaptyvbio.github.io/ProteinFlow/) + [this repository](https://github.com/adaptyvbio/ProteinFlow-models) for a use case.
 
 ## ProteinFlow Stable Releases
 You can download them with `proteinflow download --tag {tag}` in the command line or browse in the [interface](https://proteinflow-datasets.s3.eu-west-1.amazonaws.com/index.html).
 
-|Tag    |Date    |Snapshot|Size|Min res|Min len|Max len|MMseqs thr|Split (train/val/test)|Missing thr (ends/middle)|Source|Remove redundancies|Note|
-|-------|--------|--------|----|-------|-------|-------|----------|----------------------|-------------------------|---|---|----|
-|paper|10.11.22|20220103|24G|3.5|30|10'000|0.3|90/5/5|0.3/0.1|PDB|yes|first release, no mmCIF files|
-|20230102_stable|27.02.23|20230102|28G|3.5|30|10'000|0.3|90/5/5|0.3/0.1|PDB|yes|v1.1.1|
-|20230623_sabdab|26.06.23|live 26.06.23|1.2G|3.5|30|10'000|0.3|96/3/1|0.3/0.1|SAbDab|no|v1.4.1|
+|Tag    |Date    |Snapshot|Size|Min res|Min len|Max len|Max chains|MMseqs thr|Split (train/val/test)|Missing thr (ends/middle)|Source|Remove redundancies|Note|
+|-------|--------|--------|----|-------|-------|-------|----------|----------|----------------------|-------------------------|---|---|----------------|
+|paper|10.11.22|20220103|24G|3.5|30|10'000|-|0.3|90/5/5|0.3/0.1|PDB|yes|first release, no mmCIF files|
+|20230102_stable|27.02.23|20230102|28G|3.5|30|10'000|-|0.3|90/5/5|0.3/0.1|PDB|yes|v1.1.1|
+|20230623_sabdab|26.06.23|live 26.06.23|1.4G|3.5|30|10'000|-|0.3|96/3/1|0.5/0.2|SAbDab|no|v1.4.1 (requires >= v1.4.0)|
+|20230102_v200|19.07.23|20230102|33G|3.5|30|10'000|10|0.3|90/5/5|0.3/0.1|PDB|no|v2.0.0|
 
 ## License
 The `proteinflow` package and data are released and distributed under the BSD 3-Clause License
 
 
 ## Contributions
 This is an open source project supported by [Adaptyv Bio](https://www.adaptyvbio.com/). Contributions, suggestions and bug-fixes are welcomed.
```

#### html2text {}

```diff
@@ -23,21 +23,22 @@
 raw.githubusercontent.com/adaptyvbio/ProteinFlow/main/media/pf-1.png) --- ##
 Installation conda: ```bash # This should take a few minutes, be patient conda
 install -c conda-forge -c bioconda -c adaptyvbio proteinflow ``` pip: ```bash
 pip install proteinflow ``` docker: ```bash docker pull adaptyvbio/proteinflow
 ``` ### Troubleshooting - If you are using python 3.10 and encountering
 installation problems, try running `python -m pip install prody==2.4.0` before
 installing `proteinflow`. - If you are planning to generate new datasets and
-installed `proteinflow` with `pip`, you will need to additionally install
-[`mmseqs`](https://github.com/soedinglab/MMseqs2). - Generating new datasets
-also depends on the `rcsbsearch` package and the latest release [v0.2.3](https:
-//github.com/sbliven/rcsbsearch/releases/tag/v0.2.3) is currently not working
-correctly. The recommended fix is installing the version from [this pull
-request](https://github.com/sbliven/rcsbsearch/pull/6). ```bash python -m pip
-install "rcsbsearch @ git+https://github.com/sbliven/
+installed `proteinflow` with `pip` (or with `conda` on Mac OS with an M1
+processor), you will need to additionally install [`mmseqs`](https://
+github.com/soedinglab/MMseqs2). - Generating new datasets also depends on the
+`rcsbsearch` package and the latest release [v0.2.3](https://github.com/
+sbliven/rcsbsearch/releases/tag/v0.2.3) is currently not working correctly. The
+recommended fix is installing the version from [this pull request](https://
+github.com/sbliven/rcsbsearch/pull/6). ```bash python -m pip install
+"rcsbsearch @ git+https://github.com/sbliven/
 rcsbsearch@dbdfe3880cc88b0ce57163987db613d579400c8e" ``` - The docker image can
 be accessed in interactive mode with this command. ```bash docker run -it -v /
 path/to/data:/media adaptyvbio/proteinflow bash ``` ## Usage ### Downloading
 pre-computed datasets (stable) Already precomputed datasets with consensus set
 of parameters and can be accessed and downloaded using the `proteinflow`.
 package. Check the output of `proteinflow check_tags` for a list of available
 tags. ```bash proteinflow download --tag 20230102_stable ``` ### Running the
@@ -127,20 +128,20 @@
 #(B, L, 3) to_predict = batch["masked_res"] #(B, L), 1 where the residues
 should be masked, 0 otherwise ... ``` See more details on available parameters
 and the data format in the [docs](https://adaptyvbio.github.io/ProteinFlow/) +
 [this repository](https://github.com/adaptyvbio/ProteinFlow-models) for a use
 case. ## ProteinFlow Stable Releases You can download them with `proteinflow
 download --tag {tag}` in the command line or browse in the [interface](https://
 proteinflow-datasets.s3.eu-west-1.amazonaws.com/index.html). |Tag |Date
-|Snapshot|Size|Min res|Min len|Max len|MMseqs thr|Split (train/val/
+|Snapshot|Size|Min res|Min len|Max len|Max chains|MMseqs thr|Split (train/val/
 test)|Missing thr (ends/middle)|Source|Remove redundancies|Note| |-------|-----
----|--------|----|-------|-------|-------|----------|----------------------|---
-----------------------|---|---|----
-| |paper|10.11.22|20220103|24G|3.5|30|10'000|0.3|90/5/5|0.3/0.1|PDB|yes|first
-release, no mmCIF files|
-|20230102_stable|27.02.23|20230102|28G|3.5|30|10'000|0.3|90/5/5|0.3/
-0.1|PDB|yes|v1.1.1| |20230623_sabdab|26.06.23|live
-26.06.23|1.2G|3.5|30|10'000|0.3|96/3/1|0.3/0.1|SAbDab|no|v1.4.1| ## License The
-`proteinflow` package and data are released and distributed under the BSD 3-
-Clause License ## Contributions This is an open source project supported by
-[Adaptyv Bio](https://www.adaptyvbio.com/). Contributions, suggestions and bug-
-fixes are welcomed.
+---|--------|----|-------|-------|-------|----------|----------|---------------
+-------|-------------------------|---|---|----------------
+| |paper|10.11.22|20220103|24G|3.5|30|10'000|-|0.3|90/5/5|0.3/0.1|PDB|yes|first
+release, no mmCIF files| |20230102_stable|27.02.23|20230102|28G|3.5|30|10'000|-
+|0.3|90/5/5|0.3/0.1|PDB|yes|v1.1.1| |20230623_sabdab|26.06.23|live
+26.06.23|1.4G|3.5|30|10'000|-|0.3|96/3/1|0.5/0.2|SAbDab|no|v1.4.1 (requires >=
+v1.4.0)| |20230102_v200|19.07.23|20230102|33G|3.5|30|10'000|10|0.3|90/5/5|0.3/
+0.1|PDB|no|v2.0.0| ## License The `proteinflow` package and data are released
+and distributed under the BSD 3-Clause License ## Contributions This is an open
+source project supported by [Adaptyv Bio](https://www.adaptyvbio.com/).
+Contributions, suggestions and bug-fixes are welcomed.
```

### Comparing `proteinflow-1.4.1/proteinflow/constants.py` & `proteinflow-2.0.0/proteinflow/constants.py`

 * *Files 26% similar despite different names*

```diff
@@ -122,15 +122,16 @@
 )
 FEATURES_DICT["acceptor"].update(
     {**{x: 1 for x in "DENQHSTY"}, **{x: 0 for x in "RKWACGILMFPV-"}}
 )
 FEATURES_DICT["donor"].update(
     {**{x: 1 for x in "RKWNQHSTY"}, **{x: 0 for x in "DEACGILMFPV-"}}
 )
-CDR = {"-": 0, "H1": 1, "H2": 2, "H3": 3, "L1": 4, "L2": 5, "L3": 6}
+CDR_REVERSE = {"-": 0, "H1": 1, "H2": 2, "H3": 3, "L1": 4, "L2": 5, "L3": 6}
+CDR_ALPHABET = {v: k for k, v in CDR_REVERSE.items()}
 
 ALLOWED_AG_TYPES = {
     "protein",
     "protein | protein",
     "protein | protein | protein",
     "protein | protein | protein | protein | protein",
     "protein | protein | protein | protein",
@@ -158,14 +159,26 @@
     "GLU": ["CB", "CG", "CD", "OE1", "OE2"],
     "TYR": ["CB", "CG", "CD1", "CD2", "CE1", "CE2", "CZ", "OH"],
     "MET": ["CB", "CG", "SD", "CE"],
 }
 
 BACKBONE_ORDER = ["N", "C", "CA", "O"]
 
+MAIN_ATOM_DICT = defaultdict(lambda: None)
+d1to3 = {v: k for k, v in D3TO1.items()}
+for i, letter in enumerate(ALPHABET):
+    if i == 0:
+        continue
+    MAIN_ATOM_DICT[i] = MAIN_ATOMS[d1to3[letter]]
+
+ATOM_MASKS = dict()
+for k, v in SIDECHAIN_ORDER.items():
+    ATOM_MASKS[k] = np.ones(14)
+    ATOM_MASKS[k][len(v) + 4 :] = 0
+
 CDR_ENDS = {
     "L": {"L1": (24, 34), "L2": (50, 56), "L3": (89, 97)},
     "H": {"H1": (26, 32), "H2": (52, 56), "H3": (95, 102)},
 }  # wider definition from http://www.bioinf.org.uk/abs/info.html
 CDR_VALUES = {"L": defaultdict(lambda: "-"), "H": defaultdict(lambda: "-")}
 for chain_type in ["L", "H"]:
     for key, (start, end) in CDR_ENDS[chain_type].items():
@@ -181,14 +194,17 @@
 
 
 ###################################################################################
 ################################# PDB Constants ###################################
 ###################################################################################
 ALPHABET_PDB = "XACDEFGHIKLMNPQRSTVWY"
 
+ALPHABET_REVERSE = {x: i for i, x in enumerate(ALPHABET_PDB)}
+ALPHABET_REVERSE["-"] = 0
+
 GLOBAL_PAD_CHAR = 0
 ONE_TO_THREE_LETTER_MAP = {
     "R": "ARG",
     "H": "HIS",
     "K": "LYS",
     "D": "ASP",
     "E": "GLU",
@@ -207,14 +223,15 @@
     "F": "PHE",
     "Y": "TYR",
     "W": "TRP",
 }
 ATOM_MAP_4 = {a: ["N", "C", "CA", "O"] for a in ONE_TO_THREE_LETTER_MAP.keys()}
 ATOM_MAP_1 = {a: ["CA"] for a in ONE_TO_THREE_LETTER_MAP.keys()}
 ATOM_MAP_3 = {a: ["N", "C", "CA"] for a in ONE_TO_THREE_LETTER_MAP.keys()}
+ATOM_MAP_14 = {D3TO1[k]: BACKBONE_ORDER + v for k, v in SIDECHAIN_ORDER.items()}
 
 
 def _PMAP(x):
     return [
         FEATURES_DICT["hydropathy"][x] / 5,
         FEATURES_DICT["volume"][x] / 200,
         FEATURES_DICT["charge"][x],
```

### Comparing `proteinflow-1.4.1/proteinflow/metrics/__init__.py` & `proteinflow-2.0.0/proteinflow/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.4.1/proteinflow/protein_dataset.py` & `proteinflow-2.0.0/proteinflow/data/torch.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,256 @@
+"""Subclasses of `torch.utils.data.Dataset` and `torch.utils.data.DataLoader` that are tuned for loading proteinflow data."""
 import os
 import pickle
 import random
-import shutil
-import subprocess
-from collections import Counter, defaultdict
+from collections import defaultdict
 from copy import deepcopy
 from itertools import combinations
 
 import numpy as np
-import pandas as pd
 import torch
-from numpy import linalg
 from p_tqdm import p_map
-from torch.utils.data import Dataset
+from torch.utils.data import DataLoader, Dataset
 from tqdm import tqdm
 
-from proteinflow.constants import _PMAP, ALPHABET, CDR, D3TO1, MAIN_ATOMS
-from proteinflow.pdb import _check_biounits
-from proteinflow.utils.biotite_sse import _annotate_sse
-from proteinflow.utils.boto_utils import (
-    _download_dataset_dicts_from_s3,
-    _download_dataset_from_s3,
-    _get_s3_paths_from_tag,
-)
+from proteinflow.constants import ALPHABET, CDR_REVERSE, D3TO1, MAIN_ATOMS
+from proteinflow.data import ProteinEntry
 
 
-class ProteinDataset(Dataset):
+class _PadCollate:
+    """A variant of `collate_fn` that pads according to the longest sequence in a batch of sequences."""
+
+    def __init__(
+        self,
+        mask_residues=True,
+        lower_limit=15,
+        upper_limit=100,
+        mask_frac=None,
+        mask_whole_chains=False,
+        force_binding_sites_frac=0.15,
+        mask_all_cdrs=False,
+    ):
+        """Initialize a _PadCollate object.
+
+        Parameters
+        ----------
+        batch : dict
+            a batch generated by `ProteinDataset` and `PadCollate`
+        lower_limit : int, default 15
+            the minimum number of residues to mask
+        upper_limit : int, default 100
+            the maximum number of residues to mask
+        mask_frac : float, optional
+            if given, the `lower_limit` and `upper_limit` are ignored and the number of residues to mask is `mask_frac` times the length of the chain
+        mask_whole_chains : bool, default False
+            if `True`, `upper_limit`, `force_binding_sites` and `lower_limit` are ignored and the whole chain is masked instead
+        force_binding_sites_frac : float, default 0.15
+            if > 0, in the fraction of cases where a chain from a polymer is sampled, the center of the masked region will be
+            forced to be in a binding site
+        mask_all_cdrs : bool, default False
+            if `True`, all CDRs are masked
+
+        Returns
+        -------
+        chain_M : torch.Tensor
+            a `(B, L)` shaped binary tensor where 1 denotes the part that needs to be predicted and
+            0 is everything else
+
+        """
+        super().__init__()
+        self.mask_residues = mask_residues
+        self.lower_limit = lower_limit
+        self.upper_limit = upper_limit
+        self.mask_frac = mask_frac
+        self.mask_whole_chains = mask_whole_chains
+        self.force_binding_sites_frac = force_binding_sites_frac
+        self.mask_all_cdrs = mask_all_cdrs
+
+    def pad_collate(self, batch):
+        # find longest sequence
+        out = {}
+        max_len = max(map(lambda x: x["S"].shape[0], batch))
+
+        # pad according to max_len
+        to_pad = [max_len - b["S"].shape[0] for b in batch]
+        for key in batch[0].keys():
+            if key in ["chain_id", "chain_dict", "pdb_id", "cdr_id"]:
+                continue
+            out[key] = torch.stack(
+                [
+                    torch.cat([b[key], torch.zeros((pad, *b[key].shape[1:]))], 0)
+                    for b, pad in zip(batch, to_pad)
+                ],
+                0,
+            )
+        out["chain_id"] = torch.tensor([b["chain_id"] for b in batch])
+        if "cdr_id" in batch[0]:
+            out["cdr_id"] = torch.tensor([b["cdr_id"] for b in batch])
+        out["chain_dict"] = [b["chain_dict"] for b in batch]
+        out["pdb_id"] = [b["pdb_id"] for b in batch]
+        return out
+
+    def __call__(self, batch):
+        return self.pad_collate(batch)
+
+
+class ProteinLoader(DataLoader):
+    """A subclass of `torch.data.utils.DataLoader` tuned for the `proteinflow` dataset.
+
+    Creates and iterates over an instance of `ProteinDataset`, omitting the `'chain_dict'` keys.
+    See the `ProteinDataset` documentation for more information.
+
+    If batch size is larger than one, all objects are padded with zeros at the ends to reach the length of the
+    longest protein in the batch.
+
     """
-    Dataset to load proteinflow data
+
+    def __init__(
+        self,
+        dataset,
+        collate_func=_PadCollate,
+        shuffle_batches=True,
+        *args,
+        **kwargs,
+    ):
+        """Initialize a ProteinLoader instance.
+
+        Parameters
+        ----------
+        dataset : ProteinDataset
+            a ProteinDataset instance
+        shuffle_batches : bool, default True
+            if `True`, the batches are shuffled at each epoch
+        collate_func : callable, optional
+            a function that takes a list of samples and returns a batch and inherits from _PadCollate
+
+        """
+        super().__init__(
+            dataset,
+            collate_fn=collate_func(),
+            shuffle=shuffle_batches,
+            *args,
+            **kwargs,
+        )
+
+    @staticmethod
+    def from_args(
+        dataset_folder,
+        features_folder="./data/tmp/",
+        clustering_dict_path=None,
+        max_length=None,
+        rewrite=False,
+        use_fraction=1,
+        load_to_ram=False,
+        debug=False,
+        interpolate="none",
+        node_features_type=None,
+        entry_type="biounit",  # biounit, chain, pair
+        classes_to_exclude=None,
+        lower_limit=15,
+        upper_limit=100,
+        mask_residues=True,
+        mask_whole_chains=False,
+        mask_frac=None,
+        force_binding_sites_frac=0,
+        shuffle_clusters=True,
+        shuffle_batches=True,
+        mask_all_cdrs=False,
+        classes_dict_path=None,
+        *args,
+        **kwargs,
+    ) -> None:
+        """Create a `ProteinLoader` instance with a `ProteinDataset` from the given arguments.
+
+        Parameters
+        ----------
+        dataset_folder : str
+            the path to the folder with proteinflow format input files (assumes that files are named {biounit_id}.pickle)
+        features_folder : str
+            the path to the folder where the ProteinMPNN features will be saved
+        clustering_dict_path : str, optional
+            path to the pickled clustering dictionary (keys are cluster ids, values are (biounit id, chain id) tuples)
+        max_length : int, optional
+            entries with total length of chains larger than `max_length` will be disregarded
+        rewrite : bool, default False
+            if `False`, existing feature files are not overwritten
+        use_fraction : float, default 1
+            the fraction of the clusters to use (first N in alphabetic order)
+        load_to_ram : bool, default False
+            if `True`, the data will be stored in RAM (use with caution! if RAM isn't big enough the machine might crash)
+        debug : bool, default False
+            only process 1000 files
+        interpolate : {"none", "only_middle", "all"}
+            `"none"` for no interpolation, `"only_middle"` for only linear interpolation in the middle, `"all"` for linear interpolation + ends generation
+        node_features_type : {"dihedral", "sidechain_orientation", "chemical", "secondary_structure", "sidechain_coords", or combinations with "+"}, optional
+            the type of node features, e.g. `"dihedral"` or `"sidechain_orientation+chemical"`
+        entry_type : {"biounit", "chain", "pair"}
+            the type of entries to generate (`"biounit"` for biounit-level, `"chain"` for chain-level, `"pair"` for chain-chain pairs)
+        classes_to_exclude : list of str, optional
+            a list of classes to exclude from the dataset (select from `"single_chains"`, `"heteromers"`, `"homomers"`)
+        lower_limit : int, default 15
+            the minimum number of residues to mask
+        upper_limit : int, default 100
+            the maximum number of residues to mask
+        mask_residues : bool, default True
+            if `True`, generate a mask key
+        mask_whole_chains : bool, default False
+            if `True`, `upper_limit`, `force_binding_sites` and `lower_limit` are ignored and the whole chain is masked instead
+        mask_frac : float, optional
+            if given, the `lower_limit` and `upper_limit` are ignored and the number of residues to mask is `mask_frac` times the length of the chain
+        force_binding_sites_frac : float, default 0
+            if > 0, in the fraction of cases where a chain from a polymer is sampled, the center of the masked region will be
+            forced to be in a binding site
+        shuffle_clusters : bool, default True
+            if `True`, a new representative is randomly selected for each cluster at each epoch (if `clustering_dict_path` is given)
+        shuffle_batches : bool, default True
+            if `True`, the batches are shuffled at each epoch
+        mask_all_cdrs : bool, default False
+            if `True`, all CDRs are masked instead of just the sampled one
+        classes_dict_path : str, optional
+            path to the pickled classes dictionary
+        *args
+            additional arguments to `torch.utils.data.DataLoader`
+        **kwargs
+            additional keyword arguments to `torch.utils.data.DataLoader`
+
+        """
+        dataset = ProteinDataset(
+            dataset_folder=dataset_folder,
+            features_folder=features_folder,
+            clustering_dict_path=clustering_dict_path,
+            max_length=max_length,
+            rewrite=rewrite,
+            use_fraction=use_fraction,
+            load_to_ram=load_to_ram,
+            debug=debug,
+            interpolate=interpolate,
+            node_features_type=node_features_type,
+            entry_type=entry_type,
+            classes_to_exclude=classes_to_exclude,
+            shuffle_clusters=shuffle_clusters,
+            classes_dict_path=classes_dict_path,
+            lower_limit=lower_limit,
+            upper_limit=upper_limit,
+            mask_residues=mask_residues,
+            mask_whole_chains=mask_whole_chains,
+            mask_frac=mask_frac,
+            force_binding_sites_frac=force_binding_sites_frac,
+            mask_all_cdrs=mask_all_cdrs,
+        )
+        return ProteinLoader(
+            dataset=dataset,
+            shuffle_batches=shuffle_batches,
+            *args,
+            **kwargs,
+        )
+
+
+class ProteinDataset(Dataset):
+    """Dataset to load proteinflow data.
 
     Saves the model input tensors as pickle files in `features_folder`. When `clustering_dict_path` is provided,
     at each iteration a random biounit from a cluster is sampled.
 
     If a complex contains multiple chains, they are concatenated. The sequence identity information is preserved in the
     `'chain_encoding_all'` object and in the `'residue_idx'` arrays the chain change is denoted by a +100 jump.
 
@@ -58,16 +277,28 @@
     key with a CDR tensor of length `total_L`. In the array, the CDR residues are marked with the corresponding CDR type
     (H1=1, H2=2, H3=3, L1=4, L2=5, L3=6) and the rest of the residues are marked with 0s.
 
     Use the `set_cdr` method to only iterate over specific CDRs.
 
     In order to compute additional features, use the `feature_functions` parameter. It should be a dictionary with keys
     corresponding to the feature names and values corresponding to the functions that compute the features. The functions
-    should take a chain dictionary and an integer representation of the sequence as input (the dictionary is in `proteinflow` format,
-    see the docs for `generate_data` for details) and return a `numpy` array shaped as `(#residues, #features)`.
+    should take a `proteinflow.data.ProteinEntry` instance and a list of chains and return a `numpy` array shaped as `(#residues, #features)`
+    where `#residues` is the total number of residues in those chains and the features are concatenated in the order of the list:
+    `func(data_entry: ProteinEntry, chains: list) -> np.ndarray`.
+
+    If `mask_residues` is `True`, an additional `'masked_res'` key is added to the output. The value is a binary
+    tensor shaped `(B, L)` where 1 denotes the part that needs to be predicted and 0 is everything else. The tensors are generated
+    according to the following rulesd:
+    - if the dataset is generated from SAbDab files, the sampled CDR is masked,
+    - if `mask_whole_chains` is `True`, the whole chain is masked,
+    - if `mask_frac` is given, the number of residues to mask is `mask_frac` times the length of the chain,
+    - otherwise, the number of residues to mask is sampled uniformly from the range [`lower_limit`, `upper_limit`].
+
+    If `force_binding_sites_frac` > 0 and `mask_whole_chains` is `False`, in the fraction of cases where a chain
+    from a polymer is sampled, the center of the masked region will be forced to be in a binding site (in PDB datasets).
 
     """
 
     def __init__(
         self,
         dataset_folder,
         features_folder="./data/tmp/",
@@ -83,16 +314,24 @@
         entry_type="biounit",  # biounit, chain, pair
         classes_to_exclude=None,  # heteromers, homomers, single_chains
         shuffle_clusters=True,
         min_cdr_length=None,
         feature_functions=None,
         classes_dict_path=None,
         cut_edges=False,
+        mask_residues=True,
+        lower_limit=15,
+        upper_limit=100,
+        mask_frac=None,
+        mask_whole_chains=False,
+        force_binding_sites_frac=0.15,
+        mask_all_cdrs=False,
     ):
-        """
+        """Initialize the dataset.
+
         Parameters
         ----------
         dataset_folder : str
             the path to the folder with proteinflow format input files (assumes that files are named {biounit_id}.pickle)
         features_folder : str, default "./data/tmp/"
             the path to the folder where the ProteinMPNN features will be saved
         clustering_dict_path : str, optional
@@ -124,26 +363,48 @@
             for SAbDab datasets, biounits with CDRs shorter than `min_cdr_length` will be excluded
         feature_functions : dict, optional
             a dictionary of functions to compute additional features (keys are the names of the features, values are the functions)
         classes_dict_path : str, optional
             a path to a pickled dictionary with biounit classes (single chain / heteromer / homomer)
         cut_edges : bool, default False
             if `True`, missing values at the edges of the sequence will be cut off
+        mask_residues : bool, default True
+            if `True`, the masked residues will be added to the output
+        lower_limit : int, default 15
+            the lower limit of the number of residues to mask
+        upper_limit : int, default 100
+            the upper limit of the number of residues to mask
+        mask_frac : float, optional
+            if given, the number of residues to mask is `mask_frac` times the length of the chain
+        mask_whole_chains : bool, default False
+            if `True`, the whole chain is masked
+        force_binding_sites_frac : float, default 0.15
+            if `force_binding_sites_frac` > 0 and `mask_whole_chains` is `False`, in the fraction of cases where a chain
+            from a polymer is sampled, the center of the masked region will be forced to be in a binding site (in PDB datasets)
+        mask_all_cdrs : bool, default False
+            if `True`, all CDRs will be masked (in SAbDab datasets)
 
         """
         alphabet = ALPHABET
         self.alphabet_dict = defaultdict(lambda: 0)
         for i, letter in enumerate(alphabet):
             self.alphabet_dict[letter] = i
         self.alphabet_dict["X"] = 0
         self.files = defaultdict(lambda: defaultdict(list))  # file path by biounit id
         self.loaded = None
         self.dataset_folder = dataset_folder
         self.features_folder = features_folder
         self.cut_edges = cut_edges
+        self.mask_residues = mask_residues
+        self.lower_limit = lower_limit
+        self.upper_limit = upper_limit
+        self.mask_frac = mask_frac
+        self.mask_whole_chains = mask_whole_chains
+        self.force_binding_sites_frac = force_binding_sites_frac
+        self.mask_all_cdrs = mask_all_cdrs
         self.feature_types = []
         if node_features_type is not None:
             self.feature_types = node_features_type.split("+")
         self.entry_type = entry_type
         self.shuffle_clusters = shuffle_clusters
         self.feature_functions = {
             "sidechain_orientation": self._sidechain,
@@ -226,16 +487,17 @@
                 classes_to_exclude.add("single_chains")
                 classes_to_exclude = list(classes_to_exclude)
             with open(clustering_dict_path, "rb") as f:
                 self.clusters = pickle.load(f)  # list of biounit ids by cluster id
                 try:  # old way of storing class information
                     classes = pickle.load(f)
                 except EOFError:
-                    with open(classes_dict_path, "rb") as f:
-                        classes = pickle.load(f)
+                    if len(classes_to_exclude) > 0:
+                        with open(classes_dict_path, "rb") as f:
+                            classes = pickle.load(f)
             to_exclude = set()
             for c in classes_to_exclude:
                 for key, id_arr in classes.get(c, {}).items():
                     for id, _ in id_arr:
                         to_exclude.add(id)
             for key in list(self.clusters.keys()):
                 cluster_list = []
@@ -275,376 +537,268 @@
                             self.loaded[file] = pickle.load(f)
         sample_file = list(self.files.keys())[0]
         sample_chain = list(self.files[sample_file].keys())[0]
         self.sabdab = "__" in sample_chain
         self.cdr = 0
         self.set_cdr(None)
 
-    def _interpolate(self, crd_i, mask_i):
-        """
-        Fill in missing values in the middle with linear interpolation and (if fill_ends is true) build an initialization for the ends
+    def _get_masked_sequence(
+        self,
+        data,
+    ):
+        """Get the mask for the residues that need to be predicted.
 
-        For the ends, the first 10 residues are 3.6 A apart from each other on a straight line from the last known value away from the center.
-        Next they are 3.6 A apart in a random direction.
-        """
+        Depending on the parameters the residues are selected as follows:
+        - if `mask_whole_chains` is `True`, the whole chain is masked
+        - if `mask_frac` is given, the number of residues to mask is `mask_frac` times the length of the chain,
+        - otherwise, the number of residues to mask is sampled uniformly from the range [`lower_limit`, `upper_limit`].
 
-        if self.interpolate in ["all", "only_middle"]:
-            crd_i[(1 - mask_i).astype(bool)] = np.nan
-            df = pd.DataFrame(crd_i.reshape((crd_i.shape[0], -1)))
-            crd_i = df.interpolate(limit_area="inside").values.reshape(crd_i.shape)
-        if self.interpolate == "all":
-            non_nans = np.where(~np.isnan(crd_i[:, 0, 0]))[0]
-            known_start = non_nans[0]
-            known_end = non_nans[-1] + 1
-            if known_end < len(crd_i) or known_start > 0:
-                center = crd_i[non_nans, 2, :].mean(0)
-                if known_start > 0:
-                    direction = crd_i[known_start, 2, :] - center
-                    direction = direction / linalg.norm(direction)
-                    for i in range(0, min(known_start, 10)):
-                        crd_i[known_start - i - 1] = (
-                            crd_i[known_start - i] + direction * 3.6
-                        )
-                    for i in range(min(known_start, 10), known_start):
-                        v = np.random.rand(3)
-                        v = v / linalg.norm(v)
-                        crd_i[known_start - i - 1] = crd_i[known_start - i] + v * 3.6
-                if known_end < len(crd_i):
-                    to_add = len(crd_i) - known_end
-                    direction = crd_i[known_end - 1, 2, :] - center
-                    direction = direction / linalg.norm(direction)
-                    for i in range(0, min(to_add, 10)):
-                        crd_i[known_end + i] = (
-                            crd_i[known_end + i - 1] + direction * 3.6
-                        )
-                    for i in range(min(to_add, 10), to_add):
-                        v = np.random.rand(3)
-                        v = v / linalg.norm(v)
-                        crd_i[known_end + i] = crd_i[known_end + i - 1] + v * 3.6
-            mask_i = np.ones(mask_i.shape)
-        if self.interpolate in ["only_middle"]:
-            nan_mask = np.isnan(crd_i)  # in the middle the nans have been interpolated
-            mask_i[~np.isnan(crd_i[:, 0, 0])] = 1
-            crd_i[nan_mask] = 0
-        if self.interpolate == "zeros":
-            non_nans = np.where(mask_i != 0)[0]
-            known_start = non_nans[0]
-            known_end = non_nans[-1] + 1
-            mask_i[known_start:known_end] = 1
-        return crd_i, mask_i
-
-    def _dihedral_angle(self, crd, msk):
-        """Praxeolitic formula
-        1 sqrt, 1 cross product"""
-
-        p0 = crd[..., 0, :]
-        p1 = crd[..., 1, :]
-        p2 = crd[..., 2, :]
-        p3 = crd[..., 3, :]
-
-        b0 = -1.0 * (p1 - p0)
-        b1 = p2 - p1
-        b2 = p3 - p2
-
-        b1 /= np.expand_dims(np.linalg.norm(b1, axis=-1), -1) + 1e-7
-
-        v = b0 - np.expand_dims(np.einsum("bi,bi->b", b0, b1), -1) * b1
-        w = b2 - np.expand_dims(np.einsum("bi,bi->b", b2, b1), -1) * b1
-
-        x = np.einsum("bi,bi->b", v, w)
-        y = np.einsum("bi,bi->b", np.cross(b1, v), w)
-        dh = np.degrees(np.arctan2(y, x))
-        dh[1 - msk] = 0
-        return dh
+        If `force_binding_sites_frac` > 0 and `mask_whole_chains` is `False`, in the fraction of cases where a chain
+        from a polymer is sampled, the center of the masked region will be forced to be in a binding site.
 
-    def _dihedral(self, chain_dict, seq):
-        """
-        Dihedral angles
-        """
+        Parameters
+        ----------
+        data : dict
+            an entry generated by `ProteinDataset`
 
-        crd = chain_dict["crd_bb"]
-        msk = chain_dict["msk"]
-        angles = []
-        # N, C, Ca, O
-        # psi
-        p = crd[:-1, [0, 2, 1], :]
-        p = np.concatenate([p, crd[1:, [0], :]], 1)
-        p = np.pad(p, ((0, 1), (0, 0), (0, 0)))
-        angles.append(self._dihedral_angle(p, msk))
-        # phi
-        p = crd[:-1, [1], :]
-        p = np.concatenate([p, crd[1:, [0, 2, 1]]], 1)
-        p = np.pad(p, ((1, 0), (0, 0), (0, 0)))
-        angles.append(self._dihedral_angle(p, msk))
-        angles = np.stack(angles, -1)
-        return angles
+        Returns
+        -------
+        chain_M : torch.Tensor
+            a `(B, L)` shaped binary tensor where 1 denotes the part that needs to be predicted and
+            0 is everything else
 
-    def _sidechain(self, chain_dict, seq):
         """
-        Sidechain orientation (defined by the 'main atoms' in the `main_atom_dict` dictionary)
-        """
-
-        crd_sc = chain_dict["crd_sc"]
-        crd_bb = chain_dict["crd_bb"]
-        orientation = np.zeros((crd_sc.shape[0], 3))
-        for i in range(1, 21):
-            if self.main_atom_dict[i] is not None:
-                orientation[seq == i] = (
-                    crd_sc[seq == i, self.main_atom_dict[i], :] - crd_bb[seq == i, 2, :]
-                )
+        if "cdr" in data and "cdr_id" in data:
+            chain_M = torch.zeros_like(data["cdr"])
+            if self.mask_all_cdrs:
+                chain_M = data["cdr"] != CDR_REVERSE["-"]
             else:
-                S_mask = seq == i
-                orientation[S_mask] = np.random.rand(*orientation[S_mask].shape)
-        orientation /= np.expand_dims(linalg.norm(orientation, axis=-1), -1) + 1e-7
-        return orientation
-
-    def _chemical(self, chain_dict, seq):
-        """
-        Chemical features (hydropathy, volume, charge, polarity, acceptor/donor)
-        """
-
-        features = np.array([_PMAP(x) for x in seq])
-        return features
-
-    def _sse(self, chain_dict, seq):
-        """
-        Secondary structure features
-        """
+                chain_M = data["cdr"] == data["cdr_id"]
+        else:
+            chain_M = torch.zeros_like(data["S"])
+            chain_index = data["chain_id"]
+            chain_bool = data["chain_encoding_all"] == chain_index
 
-        sse_map = {"c": [0, 0, 1], "b": [0, 1, 0], "a": [1, 0, 0], "": [0, 0, 0]}
-        sse = _annotate_sse(chain_dict["crd_bb"])
-        sse = np.array([sse_map[x] for x in sse]) * chain_dict["msk"][:, None]
-        return sse
+            if self.mask_whole_chains:
+                chain_M[chain_bool] = 1
+            else:
+                chains = torch.unique(data["chain_encoding_all"])
+                chain_start = torch.where(chain_bool)[0][0]
+                chain = data["X"][chain_bool]
+                res_i = None
+                interface = []
+                non_masked_interface = []
+                if len(chains) > 1 and self.force_binding_sites_frac > 0:
+                    if random.uniform(0, 1) <= self.force_binding_sites_frac:
+                        X_copy = data["X"]
+
+                        i_indices = (chain_bool == 0).nonzero().flatten()
+                        j_indices = chain_bool.nonzero().flatten()
+
+                        distances = torch.norm(
+                            X_copy[i_indices, 2, :]
+                            - X_copy[j_indices, 2, :].unsqueeze(1),
+                            dim=-1,
+                        ).cpu()
+                        close_idx = (
+                            np.where(torch.min(distances, dim=1)[0] <= 10)[0]
+                            + chain_start.item()
+                        )
 
-    def _sidechain_coords(self, chain_dict, seq):
-        """
-        Sidechain coordinates
-        """
+                        no_mask_idx = np.where(data["mask"][chain_bool])[0]
+                        interface = np.intersect1d(close_idx, j_indices)
 
-        crd_sc = chain_dict["crd_sc"]
-        return crd_sc
+                        not_end_mask = np.where(
+                            (X_copy[:, 2, :].cpu() == 0).sum(-1) != 3
+                        )[0]
+                        interface = np.intersect1d(interface, not_end_mask)
+
+                        non_masked_interface = np.intersect1d(interface, no_mask_idx)
+                        interpolate = True
+                        if len(non_masked_interface) > 0:
+                            res_i = non_masked_interface[
+                                random.randint(0, len(non_masked_interface) - 1)
+                            ]
+                        elif len(interface) > 0 and interpolate:
+                            res_i = interface[random.randint(0, len(interface) - 1)]
+                        else:
+                            res_i = no_mask_idx[random.randint(0, len(no_mask_idx) - 1)]
+                if res_i is None:
+                    non_zero = torch.where(data["mask"][chain_bool])[0]
+                    res_i = non_zero[random.randint(0, len(non_zero) - 1)]
+                res_coords = data["X"][res_i, 2, :]
+                neighbor_indices = torch.where(data["mask"][chain_bool])[0]
+                if self.mask_frac is not None:
+                    assert self.mask_frac > 0 and self.mask_frac < 1
+                    k = int(len(neighbor_indices) * self.mask_frac)
+                    k = max(k, 10)
+                else:
+                    up = min(
+                        self.upper_limit, int(len(neighbor_indices) * 0.5)
+                    )  # do not mask more than half of the sequence
+                    low = min(up - 1, self.lower_limit)
+                    k = random.choice(range(low, up))
+                dist = torch.norm(
+                    chain[neighbor_indices, 2, :] - res_coords.unsqueeze(0), dim=-1
+                )
+                closest_indices = neighbor_indices[
+                    torch.topk(dist, k, largest=False)[1]
+                ]
+                chain_M[closest_indices + chain_start] = 1
+        return chain_M
+
+    def _dihedral(self, data_entry, chains):
+        """Return dihedral angles."""
+        return data_entry.dihedral_angles(chains)
+
+    def _sidechain(self, data_entry, chains):
+        """Return Sidechain orientation (defined by the 'main atoms' in the `main_atom_dict` dictionary)."""
+        return data_entry.sidechain_orientation(chains)
+
+    def _chemical(self, data_entry, chains):
+        """Return hemical features (hydropathy, volume, charge, polarity, acceptor/donor)."""
+        return data_entry.chemical_features(chains)
+
+    def _sse(self, data_entry, chains):
+        """Return secondary structure features."""
+        return data_entry.secondary_structure(chains)
+
+    def _sidechain_coords(self, data_entry, chains):
+        """Return idechain coordinates."""
+        return data_entry.sidechain_coordinates(chains)
 
     def _process(self, filename, rewrite=False, max_length=None, min_cdr_length=None):
-        """
-        Process a proteinflow file and save it as ProteinMPNN features
-        """
-
+        """Process a proteinflow file and save it as ProteinMPNN features."""
         input_file = os.path.join(self.dataset_folder, filename)
         no_extension_name = filename.split(".")[0]
-        with open(input_file, "rb") as f:
-            data = pickle.load(f)
-        chains = sorted(data.keys())
+        data_entry = ProteinEntry.from_pickle(input_file)
+        chains = data_entry.get_chains()
         if self.entry_type == "biounit":
             chain_sets = [chains]
         elif self.entry_type == "chain":
             chain_sets = [[x] for x in chains]
         elif self.entry_type == "pair":
             chain_sets = list(combinations(chains, 2))
         else:
             raise RuntimeError(
                 "Unknown entry type, please choose from ['biounit', 'chain', 'pair']"
             )
         output_names = []
+        if self.cut_edges:
+            data_entry.cut_missing_edges()
+        if self.interpolate != "none":
+            data_entry.interpolate_coords(fill_ends=(self.interpolate == "all"))
         for chains_i, chain_set in enumerate(chain_sets):
             output_file = os.path.join(
                 self.features_folder, no_extension_name + f"_{chains_i}.pickle"
             )
             pass_set = False
             add_name = True
             if os.path.exists(output_file) and not rewrite:
                 pass_set = True
                 if max_length is not None:
-                    if sum([len(data[x]["seq"]) for x in chain_set]) > max_length:
+                    if data_entry.get_length(chain_set) > max_length:
+                        add_name = False
+                if min_cdr_length is not None and data_entry.has_cdr():
+                    cdr_length = data_entry.get_cdr_length(chain_set)
+                    if not all(
+                        [
+                            length >= min_cdr_length
+                            for length in cdr_length.values()
+                            if length > 0
+                        ]
+                    ):
                         add_name = False
-                if min_cdr_length is not None:
-                    for chain in chain_set:
-                        if "cdr" not in data[chain]:
-                            continue
-                        u = np.unique(data[chain]["cdr"])
-                        for cdr_ in u:
-                            if (data[chain]["cdr"] == cdr_).sum() < min_cdr_length:
-                                add_name = False
             else:
-                X = []
-                S = []
-                mask = []
-                mask_original = []
-                chain_encoding_all = []
-                residue_idx = []
-                cdr = []
-                node_features = defaultdict(lambda: [])
-                last_idx = 0
-                chain_dict = {}
-
                 if max_length is not None:
-                    if sum([len(data[x]["seq"]) for x in chain_set]) > max_length:
+                    if data_entry.get_length(chains=chain_set) > max_length:
                         pass_set = True
                         add_name = False
-                if min_cdr_length is not None:
-                    for chain in chain_set:
-                        if "cdr" not in data[chain]:
-                            continue
-                        u = np.unique(data[chain]["cdr"])
-                        for cdr_ in u:
-                            if (data[chain]["cdr"] == cdr_).sum() < min_cdr_length:
-                                add_name = False
-                                pass_set = True
+                if min_cdr_length is not None and data_entry.has_cdr():
+                    cdr_length = data_entry.get_cdr_length(chain_set)
+                    if not all(
+                        [
+                            length >= min_cdr_length
+                            for length in cdr_length.values()
+                            if length > 0
+                        ]
+                    ):
+                        add_name = False
+                        pass_set = True
 
                 if self.entry_type == "pair":
                     # intersect = []
-                    X1 = data[chain_set[0]]["crd_bb"][
-                        data[chain_set[0]]["msk"].astype(bool)
-                    ]
-                    X2 = data[chain_set[1]]["crd_bb"][
-                        data[chain_set[1]]["msk"].astype(bool)
-                    ]
-                    intersect_dim_X1 = []
-                    intersect_dim_X2 = []
-                    intersect_X1 = np.zeros(len(X1))
-                    intersect_X2 = np.zeros(len(X2))
-                    margin = 30
-                    cutoff = 10
-                    for dim in range(3):
-                        min_dim_1 = X1[:, 2, dim].min()
-                        max_dim_1 = X1[:, 2, dim].max()
-                        min_dim_2 = X2[:, 2, dim].min()
-                        max_dim_2 = X2[:, 2, dim].max()
-                        intersect_dim_X1.append(
-                            np.where(
-                                np.logical_and(
-                                    X1[:, 2, dim] >= min_dim_2 - margin,
-                                    X1[:, 2, dim] <= max_dim_2 + margin,
-                                )
-                            )[0]
-                        )
-                        intersect_dim_X2.append(
-                            np.where(
-                                np.logical_and(
-                                    X2[:, 2, dim] >= min_dim_1 - margin,
-                                    X2[:, 2, dim] <= max_dim_1 + margin,
-                                )
-                            )[0]
-                        )
-
-                        # if min_dim_1 - 4 <= max_dim_2 and max_dim_1 >= min_dim_2 - 4:
-                        #     intersect.append(True)
-                        # else:
-                        #     intersect.append(False)
-                        #     break
-                    intersect_X1 = np.intersect1d(
-                        np.intersect1d(intersect_dim_X1[0], intersect_dim_X1[1]),
-                        intersect_dim_X1[2],
-                    )
-                    intersect_X2 = np.intersect1d(
-                        np.intersect1d(intersect_dim_X2[0], intersect_dim_X2[1]),
-                        intersect_dim_X2[2],
-                    )
-
-                    not_end_mask1 = np.where((X1[:, 2, :] == 0).sum(-1) != 3)[0]
-                    not_end_mask2 = np.where((X2[:, 2, :] == 0).sum(-1) != 3)[0]
-
-                    intersect_X1 = np.intersect1d(intersect_X1, not_end_mask1)
-                    intersect_X2 = np.intersect1d(intersect_X2, not_end_mask2)
-
-                    # distances = torch.norm(X1[intersect_X1, 2, :] - X2[intersect_X2, 2, :](1), dim=-1)
-                    diff = X1[intersect_X1, 2, np.newaxis, :] - X2[intersect_X2, 2, :]
-                    distances = np.sqrt(np.sum(diff**2, axis=2))
-
-                    intersect_X1 = torch.LongTensor(intersect_X1)
-                    intersect_X2 = torch.LongTensor(intersect_X2)
-                    if np.sum(distances < cutoff) < 3:
+                    if not data_entry.is_valid_pair(*chain_set):
                         # if not all(intersect):
                         pass_set = True
                         add_name = False
             if pass_set:
                 continue
 
+            out = {}
+            out["pdb_id"] = no_extension_name.split("-")[0]
+            out["mask_original"] = torch.tensor(
+                data_entry.get_mask(chain_set, original=True)
+            )
+            out["mask"] = torch.tensor(data_entry.get_mask(chain_set, original=False))
+            out["S"] = torch.tensor(data_entry.get_sequence(chain_set, encode=True))
+            out["X"] = torch.tensor(data_entry.get_coordinates(chain_set, bb_only=True))
+            out["residue_idx"] = torch.tensor(
+                data_entry.get_index_array(chain_set, index_bump=100)
+            )
+            out["chain_encoding_all"] = torch.tensor(
+                data_entry.get_chain_id_array(chain_set)
+            )
+            out["chain_dict"] = data_entry.get_chain_id_dict(chain_set)
             cdr_chain_set = set()
-            for chain_i, chain in enumerate(chain_set):
-                seq = torch.tensor([self.alphabet_dict[x] for x in data[chain]["seq"]])
-                S.append(seq)
-                mask_original.append(deepcopy(data[chain]["msk"]))
-                if self.interpolate != "none":
-                    data[chain]["crd_bb"], data[chain]["msk"] = self._interpolate(
-                        data[chain]["crd_bb"], data[chain]["msk"]
+            if data_entry.has_cdr():
+                out["cdr"] = torch.tensor(data_entry.get_cdr(chain_set, encode=True))
+                chain_type_dict = data_entry.get_chain_type_dict(chain_set)
+                if "heavy" in chain_type_dict:
+                    cdr_chain_set.update(
+                        [
+                            f"{chain_type_dict['heavy']}__{cdr}"
+                            for cdr in ["H1", "H2", "H3"]
+                        ]
                     )
-                X.append(data[chain]["crd_bb"])
-                mask.append(data[chain]["msk"])
-                residue_idx.append(torch.arange(len(data[chain]["seq"])) + last_idx)
-                if "cdr" in data[chain]:
-                    u, inv = np.unique(data[chain]["cdr"], return_inverse=True)
-                    cdr_chain = np.array([CDR[x] for x in u])[inv].reshape(
-                        data[chain]["cdr"].shape
+                if "light" in chain_type_dict:
+                    cdr_chain_set.update(
+                        [
+                            f"{chain_type_dict['light']}__{cdr}"
+                            for cdr in ["L1", "L2", "L3"]
+                        ]
                     )
-                    cdr.append(cdr_chain)
-                    cdr_chain_set.update([f"{chain}__{cdr}" for cdr in u])
-                last_idx = residue_idx[-1][-1] + 100
-                chain_encoding_all.append(torch.ones(len(data[chain]["seq"])) * chain_i)
-                chain_dict[chain] = chain_i
-                for name in self.feature_types:
-                    if name not in self.feature_functions:
-                        continue
-                    func = self.feature_functions[name]
-                    node_features[name].append(func(data[chain], seq))
+            for name in self.feature_types:
+                if name not in self.feature_functions:
+                    continue
+                func = self.feature_functions[name]
+                out[name] = torch.tensor(func(data_entry, chain_set))
 
             if add_name:
                 output_names.append(
                     (
                         os.path.basename(no_extension_name),
                         output_file,
                         chain_set if len(cdr_chain_set) == 0 else cdr_chain_set,
                     )
                 )
-
-            if self.cut_edges:
-                for chain_i, m in enumerate(mask):
-                    ind = np.where(m)[0]
-                    start, end = ind[0], ind[-1]
-                    X[chain_i] = X[chain_i][start : end + 1]
-                    S[chain_i] = S[chain_i][start : end + 1]
-                    mask[chain_i] = mask[chain_i][start : end + 1]
-                    mask_original[chain_i] = mask_original[chain_i][start : end + 1]
-                    residue_idx[chain_i] = residue_idx[chain_i][start : end + 1]
-                    chain_encoding_all[chain_i] = chain_encoding_all[chain_i][
-                        start : end + 1
-                    ]
-                    for key in node_features.keys():
-                        node_features[key][chain_i] = node_features[key][chain_i][
-                            start : end + 1
-                        ]
-                    if len(cdr) > 0:
-                        cdr[chain_i] = cdr[chain_i][start : end + 1]
-
-            out = {}
-            out["X"] = torch.from_numpy(np.concatenate(X, 0))
-            out["S"] = torch.cat(S)
-            out["mask"] = torch.from_numpy(np.concatenate(mask))
-            out["mask_original"] = torch.from_numpy(np.concatenate(mask_original))
-            out["chain_encoding_all"] = torch.cat(chain_encoding_all)
-            out["residue_idx"] = torch.cat(residue_idx)
-            out["chain_dict"] = chain_dict
-            out["pdb_id"] = no_extension_name.split("-")[0]
-            if len(cdr) != 0:
-                out["cdr"] = torch.from_numpy(np.concatenate(cdr))
-            for key, value_list in node_features.items():
-                out[key] = torch.from_numpy(np.concatenate(value_list))
             with open(output_file, "wb") as f:
                 pickle.dump(out, f)
+
         return output_names
 
     def set_cdr(self, cdr):
-        """
-        Set the CDR to be iterated over (only for SAbDab datasets).
+        """Set the CDR to be iterated over (only for SAbDab datasets).
 
         Parameters
         ----------
         cdr : {"H1", "H2", "H3", "L1", "L2", "L3"}
             The CDR to be iterated over. Set to `None` to go back to iterating over all chains.
-        """
 
+        """
         if not self.sabdab:
             cdr = None
         if cdr == self.cdr:
             return
         self.cdr = cdr
         if cdr is None:
             self.indices = list(range(len(self.data)))
@@ -661,17 +815,26 @@
                         if chain.split("__")[1] == cdr:
                             add = True
                             break
                     if add:
                         self.indices.append(i)
 
     def __len__(self):
+        """Return the number of clusters or data entries in the dataset."""
         return len(self.indices)
 
     def __getitem__(self, idx):
+        """Return an entry from the dataset.
+
+        If a clusters file is provided, then the idx is the index of the cluster
+        and the chain is randomly selected from the cluster. Otherwise, the idx
+        is the index of the data entry and the chain is randomly selected from
+        the data entry.
+
+        """
         chain_id = None
         cdr = None
         idx = self.indices[idx]
         if self.clusters is None:
             id = self.data[idx]  # data is already filtered by length
             chain_id = random.choice(list(self.files[id].keys()))
             if self.cdr is not None:
@@ -701,219 +864,11 @@
                 except EOFError:
                     print("EOFError", file)
                     raise
         else:
             data = deepcopy(self.loaded[file])
         data["chain_id"] = data["chain_dict"][chain_id]
         if cdr is not None:
-            data["cdr_id"] = CDR[cdr]
+            data["cdr_id"] = CDR_REVERSE[cdr]
+        if self.mask_residues:
+            data["masked_res"] = self._get_masked_sequence(data)
         return data
-
-
-def _download_dataset(tag, local_datasets_folder="./data/"):
-    """
-    Download the pre-processed data and the split dictionaries
-
-    Parameters
-    ----------
-    tag : str
-        name of the dataset (check `get_available_tags` to see the options)
-    local_dataset_folder : str, default "./data/"
-        the local folder that will contain proteinflow dataset folders, temporary files and logs
-
-    Returns
-    -------
-    data_folder : str
-        the path to the downloaded data folder
-    """
-
-    s3_data_path, s3_dict_path = _get_s3_paths_from_tag(tag)
-    data_folder = os.path.join(local_datasets_folder, f"proteinflow_{tag}")
-    dict_folder = os.path.join(
-        local_datasets_folder, f"proteinflow_{tag}", "splits_dict"
-    )
-
-    print("Downloading dictionaries for splitting the dataset...")
-    _download_dataset_dicts_from_s3(dict_folder, s3_dict_path)
-    print("Done!")
-
-    _download_dataset_from_s3(dataset_path=data_folder, s3_path=s3_data_path)
-    return data_folder
-
-
-def _biounits_in_clusters_dict(clusters_dict, excluded_files=None):
-    """
-    Return the list of all biounit files present in clusters_dict
-    """
-
-    if len(clusters_dict) == 0:
-        return np.array([])
-    if excluded_files is None:
-        excluded_files = []
-    return np.unique(
-        [
-            c[0]
-            for c in list(np.concatenate(list(clusters_dict.values())))
-            if c[0] not in excluded_files
-        ]
-    )
-
-
-def _exclude(clusters_dict, set_to_exclude, exclude_based_on_cdr=None):
-    """
-    Exclude biounits from clusters_dict
-
-    Parameters
-    ----------
-    clusters_dict : dict
-        dictionary of clusters
-    set_to_exclude : set
-        set of biounits to exclude
-    exclude_based_on_cdr : str, default None
-        if not None, exclude based only on clusters based on this CDR (e.g. "H3")
-
-    """
-    excluded_set = set()
-    excluded_dict = defaultdict(set)
-    for cluster in list(clusters_dict.keys()):
-        files = clusters_dict[cluster]
-        exclude = False
-        for biounit in files:
-            if biounit in set_to_exclude:
-                exclude = True
-                break
-        if exclude:
-            if exclude_based_on_cdr is not None:
-                if not cluster.endswith(exclude_based_on_cdr):
-                    continue
-            for biounit in files:
-                clusters_dict[cluster].remove(biounit)
-                excluded_dict[cluster].add(biounit)
-                excluded_set.add(biounit)
-    return excluded_dict, excluded_set
-
-
-def _split_data(
-    dataset_path="./data/proteinflow_20221110/",
-    excluded_files=None,
-    exclude_clusters=False,
-    exclude_based_on_cdr=None,
-):
-    """
-    Rearrange files into folders according to the dataset split dictionaries at `dataset_path/splits_dict`
-
-    Parameters
-    ----------
-    dataset_path : str, default "./data/proteinflow_20221110/"
-        The path to the dataset folder containing pre-processed entries and a `splits_dict` folder with split dictionaries (downloaded or generated with `get_split_dictionaries`)
-    excluded_files : list, optional
-        A list of files to exclude from the dataset
-    exclude_clusters : bool, default False
-        If True, exclude all files in a cluster if at least one file in the cluster is in `excluded_files`
-    exclude_based_on_cdr : str, optional
-        If not `None`, exclude all files in a cluster if the cluster name does not end with `exclude_based_on_cdr`
-    """
-
-    if excluded_files is None:
-        excluded_files = []
-
-    dict_folder = os.path.join(dataset_path, "splits_dict")
-    with open(os.path.join(dict_folder, "train.pickle"), "rb") as f:
-        train_clusters_dict = pickle.load(f)
-    with open(os.path.join(dict_folder, "valid.pickle"), "rb") as f:
-        valid_clusters_dict = pickle.load(f)
-    with open(os.path.join(dict_folder, "test.pickle"), "rb") as f:
-        test_clusters_dict = pickle.load(f)
-
-    train_biounits = _biounits_in_clusters_dict(train_clusters_dict, excluded_files)
-    valid_biounits = _biounits_in_clusters_dict(valid_clusters_dict, excluded_files)
-    test_biounits = _biounits_in_clusters_dict(test_clusters_dict, excluded_files)
-    train_path = os.path.join(dataset_path, "train")
-    valid_path = os.path.join(dataset_path, "valid")
-    test_path = os.path.join(dataset_path, "test")
-
-    if not os.path.exists(dataset_path):
-        os.makedirs(dataset_path)
-
-    if not os.path.exists(train_path):
-        os.makedirs(train_path)
-    if not os.path.exists(valid_path):
-        os.makedirs(valid_path)
-    if not os.path.exists(test_path):
-        os.makedirs(test_path)
-
-    if len(excluded_files) > 0:
-        set_to_exclude = set(excluded_files)
-        excluded_files = set()
-        excluded_clusters_dict = defaultdict(set)
-        if exclude_clusters:
-            for clusters_dict in [
-                train_clusters_dict,
-                valid_clusters_dict,
-                test_clusters_dict,
-            ]:
-                subset_excluded_set, subset_excluded_dict = _exclude(
-                    clusters_dict, set_to_exclude, exclude_based_on_cdr
-                )
-                excluded_files.update(subset_excluded_set)
-                excluded_clusters_dict.update(subset_excluded_dict)
-        excluded_files.update(set_to_exclude)
-        excluded_clusters_dict = {k: list(v) for k, v in excluded_clusters_dict.items()}
-        excluded_path = os.path.join(dataset_path, "excluded")
-        if not os.path.exists(excluded_path):
-            os.makedirs(excluded_path)
-        print("Updating the split dictionaries...")
-        with open(os.path.join(dict_folder, "train.pickle"), "wb") as f:
-            pickle.dump(train_clusters_dict, f)
-        with open(os.path.join(dict_folder, "excluded.pickle"), "wb") as f:
-            pickle.dump(excluded_clusters_dict, f)
-        print("Moving excluded files...")
-        for biounit in tqdm(excluded_files):
-            shutil.move(os.path.join(dataset_path, biounit), excluded_path)
-    print("Moving files in the train set...")
-    for biounit in tqdm(train_biounits):
-        shutil.move(os.path.join(dataset_path, biounit), train_path)
-    print("Moving files in the validation set...")
-    for biounit in tqdm(valid_biounits):
-        shutil.move(os.path.join(dataset_path, biounit), valid_path)
-    print("Moving files in the test set...")
-    for biounit in tqdm(test_biounits):
-        shutil.move(os.path.join(dataset_path, biounit), test_path)
-
-
-def _remove_database_redundancies(dir, seq_identity_threshold=0.9):
-    """
-    Remove all biounits in the database that are copies to another biounits in terms of sequence
-
-    Sequence identity is defined by the 'seq_identity_threshold' parameter for robust detection of sequence similarity (missing residues, point mutations, ...).
-
-    Parameters
-    ----------
-    dir : str
-        the path to the database where all the biounits are stored in pickle files after their processing
-    seq_identity_threshold : float, default .9
-        the threshold that determines up to what percentage identity sequences are considered as the same
-
-    Returns
-    -------
-    total_removed : int
-        the total number of removed biounits
-    """
-
-    all_files = np.array(os.listdir(dir))
-    all_pdbs = np.array([file[:4] for file in all_files])
-    pdb_counts = Counter(all_pdbs)
-    pdbs_to_check = [pdb for pdb in pdb_counts.keys() if pdb_counts[pdb] > 1]
-    total_removed = []
-
-    for pdb in tqdm(pdbs_to_check):
-        biounits_list = np.array(
-            [os.path.join(dir, file) for file in all_files[all_pdbs == pdb]]
-        )
-        biounits_list = sorted(biounits_list)
-        redundancies = _check_biounits(biounits_list, seq_identity_threshold)
-        if redundancies != []:
-            for k in redundancies:
-                total_removed.append(os.path.basename(biounits_list[k]).split(".")[0])
-                subprocess.run(["rm", biounits_list[k]])
-
-    return total_removed
```

### Comparing `proteinflow-1.4.1/proteinflow/scripts/proteinflow_cli.py` & `proteinflow-2.0.0/proteinflow/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,41 @@
-"""Command line interface for proteinflow"""
+"""Command line interface for proteinflow."""
 
 import os
 
 import click
 
 from proteinflow import (
     check_download_tags,
     check_pdb_snapshots,
     download_data,
     generate_data,
-    get_error_summary,
     split_data,
     unsplit_data,
 )
+from proteinflow.logging import get_error_summary
 
 
 @click.group(help="A data processing pipeline for protein design ML tasks")
 def cli():
+    """Use a data processing pipeline for protein design ML tasks."""
     pass
 
 
 @cli.command("check_tags", help="Print the available options for download tags")
 def check_tags():
+    """Print the available options for download tags."""
     print("Available tags:")
     for x in check_download_tags():
         print(f"    {x}")
 
 
 @cli.command("check_snapshots", help="Print the available options for PDB snapshots")
 def check_snapshots():
+    """Print the available options for PDB snapshots."""
     print("Available snapshots:")
     for x in check_pdb_snapshots():
         print(f"    {x}")
 
 
 @click.option(
     "--tag",
@@ -45,15 +48,15 @@
     help="The folder where proteinflow datasets, temporary files and logs will be stored",
 )
 @click.option(
     "--skip_splitting", is_flag=True, help="Use this flag to skip splitting the data"
 )
 @cli.command("download", help="Download an existing ProteinFlow dataset")
 def download(**kwargs):
-    """Download an existing ProteinFlow dataset"""
+    """Download an existing ProteinFlow dataset."""
     download_data(**kwargs)
 
 
 @click.option(
     "--tag",
     help="The name of the dataset",
 )
@@ -90,15 +93,15 @@
 )
 @click.option(
     "--not_remove_redundancies",
     is_flag=True,
     help="Unless this flag is used, removes biounits that are doubles of others sequence wise",
 )
 @click.option(
-    "--seq_identity_threshold",
+    "--redundancy_thr",
     default=0.9,
     type=float,
     help="The threshold upon which sequences are considered as one and the same (default: 90%)",
 )
 @click.option(
     "--valid_split",
     default=0.05,
@@ -162,17 +165,23 @@
 )
 @click.option(
     "--random_seed",
     default=42,
     type=int,
     help="The random seed to use for splitting",
 )
+@click.option(
+    "--max_chains",
+    default=10,
+    type=int,
+    help="The maximum number of chains per biounit",
+)
 @cli.command("generate", help="Generate a new ProteinFlow dataset")
 def generate(**kwargs):
-    """Generate a new ProteinFlow dataset"""
+    """Generate a new ProteinFlow dataset."""
     generate_data(**kwargs)
 
 
 @click.option(
     "--tag",
     help="The name of the dataset",
 )
@@ -240,15 +249,15 @@
     help="The random seed to use for splitting",
 )
 @cli.command(
     "split",
     help="Split an existing ProteinFlow dataset into training, validation and test subset according to MMseqs clustering and homomer/heteromer/single chain proportions",
 )
 def split(**kwargs):
-    """Split an existing ProteinFlow dataset into training, validation and test subset according to MMseqs clustering and homomer/heteromer/single chain proportions"""
+    """Split an existing ProteinFlow dataset into training, validation and test subset according to MMseqs clustering and homomer/heteromer/single chain proportions."""
     split_data(**kwargs)
 
 
 @click.option(
     "--tag",
     help="The name of the dataset",
 )
@@ -258,30 +267,30 @@
     help="The folder where proteinflow datasets are stored",
 )
 @cli.command(
     "unsplit",
     help="Move files from train, test, validation and excluded folders back into the main folder",
 )
 def unsplit(**kwargs):
-    """Move files from train, test, validation and excluded folders back into the main folder"""
+    """Move files from train, test, validation and excluded folders back into the main folder."""
     unsplit_data(**kwargs)
 
 
 @click.option(
     "--tag",
     help="The name of the dataset",
 )
 @click.option(
     "--local_datasets_folder",
     default="./data",
     help="The folder where proteinflow datasets are stored",
 )
 @cli.command("get_summary", help="Get a summary of filtering reasons from a log file")
 def get_summary(tag, local_datasets_folder):
-    """Get a summary of filtering reasons from a log file"""
+    """Get a summary of filtering reasons from a log file."""
     log_path = os.path.join(local_datasets_folder, f"proteinflow_{tag}", "log.txt")
     if not os.path.exists(log_path):
         raise ValueError(f"Log file does not exist at {log_path}")
     get_error_summary(log_path)
 
 
 if __name__ == "__main__":
```

### Comparing `proteinflow-1.4.1/proteinflow/sequences.py` & `proteinflow-2.0.0/proteinflow/split/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,119 +1,34 @@
+"""Splitting util functions."""
+
 import copy
 import os
 import pickle
 from collections import defaultdict
 
 import editdistance
 import numpy as np
 from tqdm import tqdm
 
-from proteinflow.constants import CDR_VALUES
-
-
-def _retrieve_author_chain(chain):
-    """
-    Retrieve the (author) chain names present in the chain section (delimited by '|' chars) of a header line in a fasta file
-    """
-
-    if "auth" in chain:
-        return chain.split(" ")[-1][:-1]
-
-    return chain
-
-
-def _retrieve_chain_names(entry):
-    """
-    Retrieve the (author) chain names present in one header line of a fasta file (line that begins with '>')
-    """
-
-    entry = entry.split("|")[1]
-
-    if "Chains" in entry:
-        return [_retrieve_author_chain(e) for e in entry[7:].split(", ")]
-
-    return [_retrieve_author_chain(entry[6:])]
-
-
-def _retrieve_fasta_chains(fasta_file):
-    """
-    Return a dictionary containing all the (author) chains in a fasta file (keys) and their corresponding sequence
-    """
-
-    with open(fasta_file) as f:
-        lines = np.array(f.readlines())
-
-    indexes = np.array([k for k, l in enumerate(lines) if l[0] == ">"])
-    starts = indexes + 1
-    ends = list(indexes[1:]) + [len(lines)]
-    names = lines[indexes]
-    seqs = ["".join(lines[s:e]).replace("\n", "") for s, e in zip(starts, ends)]
-
-    out_dict = {}
-    for name, seq in zip(names, seqs):
-        for chain in _retrieve_chain_names(name):
-            out_dict[chain] = seq
-
-    return out_dict
-
-
-def _get_chothia_cdr(num_array, chain_type):
-    arr = [CDR_VALUES[chain_type][int(x.split("_")[0])] for x in num_array]
-    return np.array(arr)
-
-
-def _compare_identity(seq, seqs, threshold):
-    """
-    Assess whether a sequence is in a list of sequences (in the sense that it shares at least 90% to one of the sequences in the list)
-    """
-
-    for s in seqs:
-        if editdistance.eval(s, seq) / max(len(s), len(seq)) <= (1 - threshold):
-            return True
-
-    return False
-
-
-def _compare_seqs(seqs1, seqs2, threshold):
-    """
-    Assess whether 2 lists of sequences contain exactly the same set of sequences
-    """
-
-    for seq in seqs1:
-        if not _compare_identity(seq, seqs2, threshold):
-            return False
-
-    for seq in seqs2:
-        if not _compare_identity(seq, seqs1, threshold):
-            return False
-
-    return True
-
 
 def _unique_chains(seqs_list):
-    """
-    Get unique chains
-    """
-
+    """Get unique chains."""
     new_seqs_list = [seqs_list[0]]
     chains = [new_seqs_list[0][0]]
 
     for seq in seqs_list[1:]:
         if seq[0] not in chains:
             new_seqs_list.append(seq)
             chains.append(seq[0])
 
     return new_seqs_list
 
 
 def _merge_chains(seqs_dict_):
-    """
-    Look into the chains of each PDB and regroup redundancies (at 90% sequence identity)
-    """
-
+    """Look into the chains of each PDB and regroup redundancies (at 90% sequence identity)."""
     seqs_dict = copy.deepcopy(seqs_dict_)
     pdbs_to_delete = []
 
     for pdb in tqdm(seqs_dict.keys()):
         if seqs_dict[pdb] == []:
             pdbs_to_delete.append(pdb)
             continue
@@ -152,18 +67,15 @@
     for pdb in pdbs_to_delete:
         del seqs_dict[pdb]
 
     return seqs_dict
 
 
 def _load_pdbs(dir, cdr=None):
-    """
-    Load biounits and group their sequences by PDB and similarity (90%)
-    """
-
+    """Load biounits and group their sequences by PDB and similarity (90%)."""
     seqs_dict = defaultdict(lambda: [])
 
     for file in tqdm([x for x in os.listdir(dir) if x.endswith(".pickle")]):
         load_path = os.path.join(dir, file)
         if os.path.isdir(load_path):
             continue
         with open(load_path, "rb") as f:
@@ -185,41 +97,102 @@
             seqs = [(chain, seq) for chain, seq in seqs if len(seq) > 0]
         seqs_dict[file[:4]] += seqs
 
     return seqs_dict
 
 
 def _write_fasta(fasta_path, merged_seqs_dict):
-    """
-    Write a fasta file containing all the sequences contained in the merged_seqs_dict dictionary
-    """
-
+    """Write a fasta file containing all the sequences contained in the merged_seqs_dict dictionary."""
     with open(fasta_path, "w") as f:
         for k in merged_seqs_dict.keys():
             for chain, seq in merged_seqs_dict[k]:
                 f.write(">" + k + "_" + chain + "\n")
                 f.write(seq + "\n")
 
 
 def _retrieve_seqs_names_list(merged_seqs_dict):
-    """
-    Retrieve all the sequences names that are contained in the merged_seqs_dict (same names as in the fasta file in input to MMSeqs2)
-    """
-
+    """Retrieve all the sequences names that are contained in the merged_seqs_dict (same names as in the fasta file in input to MMSeqs2)."""
     seqs_names = []
     for k in merged_seqs_dict.keys():
         for chain, _ in merged_seqs_dict[k]:
             seqs_names.append(k + "_" + chain)
 
     return seqs_names
 
 
 def _create_pdb_seqs_dict(seqs_names_list):
-    """
-    Return a dictionary that has the PDB ids as keys and the list of all the chain names that correspond to this PDB
-    """
-
+    """Return a dictionary that has the PDB ids as keys and the list of all the chain names that correspond to this PDB."""
     pdb_seqs_dict = defaultdict(lambda: [])
     for name in seqs_names_list:
         pdb_seqs_dict[name[:4]].append(name[5:])
 
     return pdb_seqs_dict
+
+
+def _test_availability(
+    size_array,
+    n_samples,
+):
+    """Test if there are enough groups in each class to construct a dataset with the required number of samples."""
+    present = np.sum(size_array != 0, axis=0)
+    return present[0] > n_samples, present[1] > n_samples, present[2] > n_samples
+
+
+def _find_correspondences(files, dataset_dir):
+    """Return a dictionary that contains all the biounits in the database (keys) and the list of all the chains that are in these biounits (values)."""
+    correspondences = defaultdict(lambda: [])
+    for file in files:
+        biounit = file
+        with open(os.path.join(dataset_dir, file), "rb") as f:
+            keys = pickle.load(f)
+            for k in keys:
+                correspondences[biounit].append(k)
+
+    return correspondences
+
+
+def _biounits_in_clusters_dict(clusters_dict, excluded_files=None):
+    """Return the list of all biounit files present in clusters_dict."""
+    if len(clusters_dict) == 0:
+        return np.array([])
+    if excluded_files is None:
+        excluded_files = []
+    return np.unique(
+        [
+            c[0]
+            for c in list(np.concatenate(list(clusters_dict.values())))
+            if c[0] not in excluded_files
+        ]
+    )
+
+
+def _exclude(clusters_dict, set_to_exclude, exclude_based_on_cdr=None):
+    """Exclude biounits from clusters_dict.
+
+    Parameters
+    ----------
+    clusters_dict : dict
+        dictionary of clusters
+    set_to_exclude : set
+        set of biounits to exclude
+    exclude_based_on_cdr : str, default None
+        if not None, exclude based only on clusters based on this CDR (e.g. "H3")
+
+    """
+    excluded_set = set()
+    excluded_dict = defaultdict(set)
+    for cluster in list(clusters_dict.keys()):
+        files = clusters_dict[cluster]
+        exclude = False
+        for biounit in files:
+            if biounit in set_to_exclude:
+                exclude = True
+                break
+        if exclude:
+            if exclude_based_on_cdr is not None:
+                if not cluster.endswith(exclude_based_on_cdr):
+                    continue
+            for biounit in files:
+                clusters_dict[cluster].remove(biounit)
+                excluded_dict[cluster].add(biounit)
+                excluded_set.add(biounit)
+    return excluded_dict, excluded_set
```

### Comparing `proteinflow-1.4.1/proteinflow/utils/boto_utils.py` & `proteinflow-2.0.0/proteinflow/download/boto.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,25 @@
+"""Boto3 helper functions for downloading files from S3."""
 import asyncio
 import os
 import shutil
 import subprocess
+import zipfile
 from operator import attrgetter
 
 from aiobotocore.session import get_session
 from botocore import UNSIGNED
 from botocore.config import Config
 from p_tqdm import p_map
 
 from proteinflow.constants import S3Obj
 
 
 def _download_dataset_dicts_from_s3(dict_folder_path, s3_path):
-    """
-    Download dictionaries containing database split information from s3 to a local folder
-    """
-
+    """Download dictionaries containing database split information from s3 to a local folder."""
     train_path = os.path.join(s3_path, "train.pickle")
     valid_path = os.path.join(s3_path, "valid.pickle")
     test_path = os.path.join(s3_path, "test.pickle")
     classes_path = os.path.join(s3_path, "classes.pickle")
 
     if not os.path.exists(dict_folder_path):
         os.makedirs(dict_folder_path)
@@ -45,15 +44,15 @@
     start=None,
     end=None,
     recursive=True,
     list_dirs=True,
     list_objs=True,
     limit=None,
 ):
-    """Iterator that lists a bucket's objects under path, (optionally) starting with start and ending before end.
+    """Return an iterator that lists a bucket's objects under path, (optionally) starting with start and ending before end.
 
     If recursive is False, then list only the "depth=0" items (dirs and objects).
 
     If recursive is True, then list recursively all objects (no dirs).
 
     Parameters
     ----------
@@ -78,16 +77,16 @@
     limit:
         optional. If specified, then lists at most this many items.
 
     Returns
     -------
     iterator
         an iterator of S3Obj.
-    """
 
+    """
     kwargs = dict()
     if start is not None:
         if not start.startswith(path):
             start = os.path.join(path, start)
     if end is not None:
         if not end.startswith(path):
             end = os.path.join(path, end)
@@ -119,40 +118,60 @@
             if end is not None and p.key >= end:
                 return
             yield p
 
 
 def _download_dataset_from_s3(
     dataset_path="./data/proteinflow_20221110/",
-    s3_path="s3://ml4-main-storage/proteinflow_20221110/",
+    s3_path="s3://ml4-main-storage/proteinflow_20221110/proteinflow_20221110.zip",
 ):
     """Download the pre-processed files."""
     if s3_path.startswith("s3"):
         print("Downloading the dataset from s3...")
+        local_zip_path = dataset_path.rstrip("/\\") + ".zip"
         subprocess.run(
-            ["aws", "s3", "sync", "--no-sign-request", s3_path, dataset_path]
+            ["aws", "s3", "cp", "--no-sign-request", s3_path, local_zip_path]
         )
         print("Done!")
     else:
         shutil.move(s3_path, dataset_path)
+    with zipfile.ZipFile(local_zip_path, "r") as zip_ref:
+        zip_ref.extractall(os.path.dirname(dataset_path))
 
 
 def _get_s3_paths_from_tag(tag):
     """Get the path to the data and split dictionary folders on S3 given a tag."""
     dict_path = f"s3://proteinflow-datasets/{tag}/proteinflow_{tag}_splits_dict/"
-    data_path = f"s3://proteinflow-datasets/{tag}/proteinflow_{tag}/"
+    data_path = f"s3://proteinflow-datasets/{tag}/proteinflow_{tag}.zip"
     return data_path, dict_path
 
 
+def _download_zip_dataset_from_s3(
+    dataset_path="./data/proteinflow_20221110/",
+    s3_path="s3://ml4-main-storage/proteinflow_20221110/",
+):
+    """Download the pre-processed files."""
+    if s3_path.startswith("s3"):
+        print("Downloading the dataset from s3...")
+        subprocess.run(
+            ["aws", "s3", "sync", "--no-sign-request", s3_path, dataset_path]
+        )
+        print("Done!")
+    else:
+        shutil.move(s3_path, dataset_path)
+
+
 async def _getobj(client, key):
+    """Get an object from S3."""
     resp = await client.get_object(Bucket="pdbsnapshots", Key=key)
     return await resp["Body"].read()
 
 
 async def _download_file(client, snapshots, tmp_folder, id):
+    """Download a file from S3."""
     pdb_id, biounit = id.lower().split("-")
     prefixes = [
         "/pub/pdb/data/biounit/PDB/all/",
         "/pub/pdb/data/biounit/mmCIF/all/",
         "/pub/pdb/data/assemblies/mmCIF/all/",
     ]
     types = ["pdb", "cif", "cif"]
@@ -171,14 +190,15 @@
                 return local_path
             except Exception:
                 pass
     return id
 
 
 async def _go(download_list, tmp_folder, snapshots):
+    """Download multiple files from S3."""
     session = get_session()
     async with session.create_client(
         "s3", config=Config(signature_version=UNSIGNED)
     ) as client:
         tasks = [
             _download_file(
                 client=client,
@@ -198,14 +218,15 @@
     loop = asyncio.new_event_loop()
     return loop.run_until_complete(
         _go(download_list, tmp_folder=tmp_folder, snapshots=snapshots)
     )
 
 
 def _download_s3_parallel(pdb_ids, tmp_folder, snapshots):
+    """Download files from S3 in parallel."""
     # number of process
     no_tasks = max(16, len(pdb_ids) // 5000)
 
     download_list_chunk = [pdb_ids[i::no_tasks] for i in range(no_tasks)]
     out = p_map(
         lambda x: _singleProcess(
             download_list=x, tmp_folder=tmp_folder, snapshots=snapshots
```

### Comparing `proteinflow-1.4.1/proteinflow/utils/cluster_and_partition.py` & `proteinflow-2.0.0/proteinflow/split/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,43 @@
+"""Functions used to split the dataset into train, validation and test sets."""
+
 import os
+import pickle
 import random as rd
+import shutil
 import subprocess
+import urllib
 from collections import defaultdict
 from itertools import combinations
 
+import editdistance
 import networkx as nx
 import numpy as np
 from tqdm import tqdm
 
-from proteinflow.sequences import (
+from proteinflow.data import PDBEntry
+from proteinflow.split.utils import (
+    _biounits_in_clusters_dict,
     _create_pdb_seqs_dict,
+    _exclude,
+    _find_correspondences,
     _load_pdbs,
     _merge_chains,
     _retrieve_seqs_names_list,
+    _test_availability,
     _write_fasta,
 )
-from proteinflow.utils.common_utils import _find_correspondences, _test_availability
 
 
 def _run_mmseqs2(fasta_file, tmp_folder, min_seq_id, cdr=None):
-    """
-    Run the MMSeqs2 command with the parameters we want
+    """Run the MMSeqs2 command with the parameters we want.
 
     Results are stored in the tmp_folder/MMSeqs2 directory.
-    """
 
+    """
     folder = "MMSeqs2_results" if cdr is None else os.path.join("MMSeqs2_results", cdr)
     os.makedirs(os.path.join(tmp_folder, folder), exist_ok=True)
     method = "easy-linclust" if cdr is not None else "easy-cluster"
     args = [
         "mmseqs",
         method,
         fasta_file,
@@ -50,20 +59,19 @@
             "--mask",
             "0",
         ]
     subprocess.run(args)
 
 
 def _read_clusters(tmp_folder, cdr=None):
-    """
-    Read the output from MMSeqs2 and produces 2 dictionaries that store the clusters information
+    """Read the output from MMSeqs2 and produces 2 dictionaries that store the clusters information.
 
     In cluster_dict, values are the full names (pdb + chains) whereas in cluster_pdb_dict, values are just the PDB ids (so less clusters but bigger).
-    """
 
+    """
     if cdr is None:
         cluster_file_fasta = os.path.join(
             tmp_folder, "MMSeqs2_results", "clusterRes_all_seqs.fasta"
         )
     else:
         cluster_file_fasta = os.path.join(
             tmp_folder, "MMSeqs2_results", cdr, "clusterRes_all_seqs.fasta"
@@ -93,20 +101,19 @@
         for k in cluster_pdb_dict.keys():
             cluster_pdb_dict[k] = np.unique(cluster_pdb_dict[k])
 
     return cluster_dict, cluster_pdb_dict
 
 
 def _make_graph(cluster_pdb_dict):
-    """
-    Produces a graph that relates clusters together
+    """Produce a graph that relates clusters together.
 
     Connections represent a PDB shared by 2 clusters. The more shared PDBs, the stronger the connection.
-    """
 
+    """
     keys = list(cluster_pdb_dict.keys())
     keys_mapping = {length: k for length, k in enumerate(keys)}
     adjacency_matrix = np.zeros((len(keys), len(keys)))
 
     seen_dict = defaultdict(set)
     for i, key in enumerate(keys):
         for pdb in cluster_pdb_dict[key]:
@@ -118,31 +125,25 @@
 
     graph = nx.from_numpy_matrix(adjacency_matrix)
     nx.relabel_nodes(graph, keys_mapping, copy=False)
     return graph
 
 
 def _check_for_heteromers(grouped_seqs, biounit_chains):
-    """
-    True if the chain names contained in grouped_seqs correspond to at least 2 different sequences
-    """
-
+    """Return True if the chain names contained in grouped_seqs correspond to at least 2 different sequences."""
     grouped_seqs = [group.split("-") for group in grouped_seqs]
     chain_seqs = [
         np.argmax([chain in group for group in grouped_seqs])
         for chain in biounit_chains
     ]
     return np.max(chain_seqs) != np.min(chain_seqs)
 
 
 def _divide_according_to_chains_interactions(pdb_seqs_dict, dataset_dir):
-    """
-    Divide all the biounit chains into 3 groups: single chains, homomers and heteromers, depending on the other chains present or not in the biounit
-    """
-
+    """Divide all the biounit chains into 3 groups: single chains, homomers and heteromers, depending on the other chains present or not in the biounit."""
     heteromers = []
     homomers = []
     single_chains = []
     all_files = np.array(list(os.listdir(dataset_dir)))
     all_pdb_files = np.array([f[:4] for f in all_files])
 
     for pdb in tqdm(pdb_seqs_dict.keys()):
@@ -181,20 +182,19 @@
 
     return single_chains, homomers, heteromers
 
 
 def _find_chains_in_graph(
     graph, clusters_dict, biounit_chains_array, pdbs_array, chains_array
 ):
-    """
-    Find all the biounit chains present in a given graph or subgraph
+    """Find all the biounit chains present in a given graph or subgraph.
 
     Return a dictionary for which each key is a cluster name (merged chains name) and the values are all the biounit chains contained in this cluster.
-    """
 
+    """
     res_dict = {}
     for k, node in enumerate(graph):
         grouped_chains = clusters_dict[node]
         split_chains = np.concatenate(
             [
                 [(pdb[:4], chain) for chain in pdb[5:].split("-")]
                 for pdb in grouped_chains
@@ -212,20 +212,20 @@
         res_dict[node] = biounits_chains
 
     return res_dict
 
 
 def _find_repartition(chains_dict, homomers, heteromers):
     """
-    Return a dictionary similar to the one created by find_chains_in_graph, with an additional level of classification for single chains, homomers and heteromers
+    Return a dictionary similar to the one created by find_chains_in_graph, with an additional level of classification for single chains, homomers and heteromers.
 
     Dictionary structure : `{'single_chains' : {cluster_name : [biounit chains]}, 'homomers' : {cluster_name : [biounit chains]}, 'heteromers' : {cluster_name : [biounit chains]}}`.
     Additionally return the number of chains in each class (single chains, ...).
-    """
 
+    """
     classes_dict = {
         "single_chains": defaultdict(lambda: []),
         "homomers": defaultdict(lambda: []),
         "heteromers": defaultdict(lambda: []),
     }
     n_single_chains, n_homomers, n_heteromers = 0, 0, 0
 
@@ -260,22 +260,21 @@
     clusters_dict,
     biounit_chains_array,
     pdbs_array,
     chains_array,
     homomers,
     heteromers,
 ):
-    """
-    Given a list of subgraphs, return a list of dictionaries and an array of sizes of the same length
+    """Given a list of subgraphs, return a list of dictionaries and an array of sizes of the same length.
 
     Dictionaries are the `chains_dict` and `classes_dict` corresponding to each subgraph, returned by the `find_chains_in_graph`
     and `find_repartition` functions respectively. The array of sizes is of shape (len(subgraph), 3). It gives the number of single chains,
     homomers and heteromers present in each subgraph.
-    """
 
+    """
     size_array = np.zeros((len(subgraphs), 3))
     dict_list = []
     for k, subgraph in tqdm(enumerate(subgraphs)):
         chains_dict = _find_chains_in_graph(
             subgraph, clusters_dict, biounit_chains_array, pdbs_array, chains_array
         )
         classes_dict, n_single_chains, n_homomers, n_heteromers = _find_repartition(
@@ -290,22 +289,21 @@
         int(np.sum(size_array[:, 0])),
         int(np.sum(size_array[:, 1])),
         int(np.sum(size_array[:, 2])),
     )
 
 
 def _construct_dataset(dict_list, size_array, indices):
-    """
-    Get a supergraph containing all subgraphs indicated by `indices`
+    """Get a supergraph containing all subgraphs indicated by `indices`.
 
     Given the `dict_list` and `size_array` returned by `find_subgraphs_info`, return the 2 dictionaries (`chains_dict` and `classes_dict`)
     corresponding to the graph encompassing all the subgraphs indicated by indices.
     Additionally return the number of single chains, homomers and heteromers in this supergraph.
-    """
 
+    """
     dataset_clusters_dict = {}
     dataset_classes_dict = {"single_chains": {}, "homomers": {}, "heteromers": {}}
     single_chains_size, homomers_size, heteromers_size = 0, 0, 0
     for k in indices:
         chains_dict, classes_dict = dict_list[k]
         n_single_chains, n_homomers, n_heteromers = size_array[k]
         single_chains_size += n_single_chains
@@ -330,20 +328,19 @@
     remaining_indices,
     chain_class,
     size_obj,
     current_sizes,
     size_array,
     tolerance=0.2,
 ):
-    """
-    Remove values from indices until we get the required (`size_obj`) number of chains in the class of interest (`chain_class`)
+    """Remove values from indices until we get the required (`size_obj`) number of chains in the class of interest (`chain_class`).
 
     Parameter `chain_class` corresponds to the single chain (0), homomer (1) or heteromer (2) class.
-    """
 
+    """
     sizes = [s[chain_class] for s in size_array[indices]]
     sorted_sizes_indices = np.argsort(sizes)[::-1]
 
     while current_sizes[chain_class] > size_obj and len(sorted_sizes_indices) > 0:
         if (
             current_sizes[chain_class]
             - size_array[indices[sorted_sizes_indices[0]], chain_class]
@@ -364,18 +361,15 @@
         current_sizes[0],
         current_sizes[1],
         current_sizes[2],
     )
 
 
 def _check_mmseqs():
-    """
-    Raise an error if MMseqs2 is not installed
-    """
-
+    """Raise an error if MMseqs2 is not installed."""
     devnull = open(os.devnull, "w")
     retval = subprocess.call(
         ["mmseqs", "--help"], stdout=devnull, stderr=subprocess.STDOUT
     )
     devnull.close()
     if retval != 0:
         raise RuntimeError(
@@ -388,20 +382,19 @@
     remaining_indices,
     chain_class,
     size_obj,
     current_sizes,
     size_array,
     tolerance=0.2,
 ):
-    """
-    Add values to indices until we get the required (`size_obj`) number of chains in the class of interest (`chain_class`)
+    """Add values to indices until we get the required (`size_obj`) number of chains in the class of interest (`chain_class`).
 
     Parameter `chain_class` corresponds to the single chain (0), homomer (1) or heteromer (2) class.
-    """
 
+    """
     sizes = [s[chain_class] for s in size_array[remaining_indices]]
     sorted_sizes_indices = np.argsort(sizes)[::-1]
 
     while current_sizes[chain_class] < size_obj and len(sorted_sizes_indices) > 0:
         if (
             current_sizes[chain_class]
             + size_array[remaining_indices[sorted_sizes_indices[0]], chain_class]
@@ -439,21 +432,20 @@
     homomers_size,
     heteromers_size,
     sc_available,
     hm_available,
     ht_available,
     tolerance=0.2,
 ):
-    """
-    If required, remove and add values in indices so that the number of chains in each class correspond to the required numbers within a tolerance
+    """If required, remove and add values in indices so that the number of chains in each class correspond to the required numbers within a tolerance.
 
     First remove and then add (if necessary, for each class separately).
     In the end, we might end up with more chains than desired in the first 2 classes but for a reasonable tolerance (~10-20 %), this should not happen.
-    """
 
+    """
     if single_chains_size > (1 + tolerance) * n_single_chains and sc_available:
         (
             indices,
             remaining_indices,
             single_chains_size,
             homomers_size,
             heteromers_size,
@@ -576,22 +568,21 @@
     n_single_chains,
     n_homomers,
     n_heteromers,
     remaining_indices,
     n_max_iter=50,
     tolerance=0.2,
 ):
-    """
-    Construct a dataset from subgraphs indicated by `indices`
+    """Construct a dataset from subgraphs indicated by `indices`.
 
     Given a list of indices to choose from (`remaining_indices`), choose a list of subgraphs to construct a dataset containing the required number of
     biounits for each class (single chains, ...) within a tolerance.
     Return the same outputs as the construct_dataset function, as long as the list of remaining indices after selection.
-    """
 
+    """
     single_chains_size, homomers_size, heteromers_size = 0, 0, 0
     sc_available, hm_available, ht_available = _test_availability(
         size_array, n_samples
     )  # rule of thumb to estimate if it is logical to try to fill the dataset with a given class
     distribution_satisfied = False
     n_iter = 0
 
@@ -658,18 +649,15 @@
 def _get_subgraph_files(
     subgraphs,
     clusters_dict,
     pdb_arr,
     chain_arr,
     files_arr,
 ):
-    """
-    Given a list of subgraphs, return a dictionary of the form {cluster: [(filename, chain__cdr)]}
-    """
-
+    """Given a list of subgraphs, return a dictionary of the form {cluster: [(filename, chain__cdr)]}."""
     out = {}  # cluster: [(file, chain__cdr)]
     for subgraph in subgraphs:
         for cluster in subgraph.nodes:
             chains = []
             _, cdr = cluster.split("__")
             for chain in clusters_dict[cluster]:
                 pdb, chain_ids = chain.split("_")
@@ -682,18 +670,15 @@
 
 def _split_subgraphs(
     lengths,
     num_clusters_valid,
     num_clusters_test,
     tolerance,
 ):
-    """
-    Split the list of subgraphs into three sets (train, valid, test) according to the number of biounits in each subgraph
-    """
-
+    """Split the list of subgraphs into three sets (train, valid, test) according to the number of biounits in each subgraph."""
     for _ in range(50):
         indices = np.random.permutation(np.arange(1, len(lengths)))
         valid_indices = []
         test_indices = []
         train_indices = [0]
         valid_sum = 0
         test_sum = 0
@@ -731,17 +716,17 @@
     clusters_dict,
     merged_seqs_dict,
     dataset_dir,
     valid_split=0.05,
     test_split=0.05,
     tolerance=0.2,
 ):
-    """
-    Given a graph representing connections between MMSeqs2 clusters, split the dataset between train, validation and test sets.
-    Each onnected component of the graph is considered as a group.
+    """Given a graph representing connections between MMSeqs2 clusters, split the dataset between train, validation and test sets.
+
+    Each connected component of the graph is considered as a group.
     Then, groups are split into the 3 sets so that each set has the right amount of biounits.
     It has been observed that the biggest group represents about 15-20 % of all the biounits and thus it is automatically assigned to the train set.
     It is difficult to have the exact ratio of biounits in each set since biounits are manipulated by groups.
     However, within an acceptable tolerance (default 20 % of the split ratio - but in theory it can be smaller), the split ratios are respected.
     The process first try to randomly assign the groups to a set.
     If after 50 trials the partition fails to comply to the requirements, the last partition is kept and small adjustments are made by moving groups from sets one by one until the ratios are approximately respected.
     Note that for very small datasets (around 250 biounits), this method will probably fail. But it also does not make much sense to use it for so few data.
@@ -779,16 +764,16 @@
         see train_classes_dict but for test set
     single_chains : list
         the list of all biounit chains (string names) that are in a single chain state (in their biounit)
     homomers : list
         the list of all biounit chains (string names) that are in a homomeric state (in their biounit)
     heteromers : list
         the list of all biounit chains (string names) that are in a heteromeric state (in their biounit)
-    """
 
+    """
     sample_cluster = list(clusters_dict.keys())[0]
     sabdab = "__" in sample_cluster
 
     subgraphs = np.array(
         [
             graph.subgraph(c)
             for c in sorted(nx.connected_components(graph), key=len, reverse=True)
@@ -1084,7 +1069,227 @@
         train_clusters_dict,
         train_classes_dict,
         valid_clusters_dict,
         valid_classes_dict,
         test_clusters_dict,
         test_classes_dict,
     )
+
+
+def _get_split_dictionaries(
+    tmp_folder="./data/tmp_pdb",
+    output_folder="./data/pdb",
+    split_tolerance=0.2,
+    test_split=0.05,
+    valid_split=0.05,
+    out_split_dict_folder="./data/dataset_splits_dict",
+    min_seq_id=0.3,
+):
+    """Split preprocessed data into training, validation and test.
+
+    Parameters
+    ----------
+    tmp_folder : str, default "./data/tmp_pdb"
+        The folder where temporary files will be saved
+    output_folder : str, default "./data/pdb"
+        The folder where the output files will be saved
+    split_tolerance : float, default 0.2
+        The tolerance on the split ratio (default 20%)
+    test_split : float, default 0.05
+        The percentage of chains to put in the test set (default 5%)
+    valid_split : float, default 0.05
+        The percentage of chains to put in the validation set (default 5%)
+    out_split_dict_folder : str, default "./data/dataset_splits_dict"
+        The folder where the dictionaries containing the train/validation/test splits information will be saved"
+    min_seq_id : float in [0, 1], default 0.3
+        minimum sequence identity for `mmseqs`
+
+    """
+    if len([x for x in os.listdir(output_folder) if x.endswith(".pickle")]) == 0:
+        raise RuntimeError("No preprocessed data found in the output folder")
+    sample_file = [x for x in os.listdir(output_folder) if x.endswith(".pickle")][0]
+    ind = sample_file.split(".")[0].split("-")[1]
+    sabdab = not ind.isnumeric()
+
+    os.makedirs(out_split_dict_folder, exist_ok=True)
+    (
+        train_clusters_dict,
+        train_classes_dict,
+        valid_clusters_dict,
+        valid_classes_dict,
+        test_clusters_dict,
+        test_classes_dict,
+    ) = _build_dataset_partition(
+        output_folder,
+        tmp_folder,
+        valid_split=valid_split,
+        test_split=test_split,
+        tolerance=split_tolerance,
+        min_seq_id=min_seq_id,
+        sabdab=sabdab,
+    )
+
+    classes_dict = train_classes_dict
+    for d in [valid_classes_dict, test_classes_dict]:
+        for k, v in d.items():
+            classes_dict[k].update(v)
+
+    with open(os.path.join(out_split_dict_folder, "classes.pickle"), "wb") as f:
+        pickle.dump(classes_dict, f)
+    with open(os.path.join(out_split_dict_folder, "train.pickle"), "wb") as f:
+        pickle.dump(train_clusters_dict, f)
+    with open(os.path.join(out_split_dict_folder, "valid.pickle"), "wb") as f:
+        pickle.dump(valid_clusters_dict, f)
+    with open(os.path.join(out_split_dict_folder, "test.pickle"), "wb") as f:
+        pickle.dump(test_clusters_dict, f)
+
+
+def _get_excluded_files(
+    tag, local_datasets_folder, tmp_folder, exclude_chains, exclude_threshold
+):
+    """Get a list of files to exclude from the dataset.
+
+    Biounits are excluded if they contain chains that are too similar
+    (above `exclude_threshold`) to chains in the list of excluded chains.
+
+    Parameters
+    ----------
+    tag : str
+        the name of the dataset
+    local_datasets_folder : str
+        the path to the folder that stores proteinflow datasets
+    tmp_folder : str
+        the path to the folder that stores temporary files
+    exclude_chains : list of str, optional
+        a list of chains (`{pdb_id}-{chain_id}`) to exclude from the splitting (e.g. `["1A2B-A", "1A2B-B"]`); chain id is the author chain id
+    exclude_threshold : float in [0, 1], default 0.7
+        the sequence similarity threshold for excluding chains
+
+    """
+    # download fasta files for excluded chains
+    if not os.path.exists(tmp_folder):
+        os.makedirs(tmp_folder)
+    sequences = []
+    for chain in exclude_chains:
+        pdb_id, chain_id = chain.split("-")
+        downloadurl = "https://www.rcsb.org/fasta/entry/"
+        pdbfn = pdb_id + "/download"
+        outfnm = os.path.join(tmp_folder, f"{pdb_id.lower()}.fasta")
+        url = downloadurl + pdbfn
+        urllib.request.urlretrieve(url, outfnm)
+        chains = PDBEntry.parse_fasta(outfnm)
+        sequences.append(chains[chain_id])
+        os.remove(outfnm)
+
+    # iterate over files in the dataset to check similarity
+    print("Checking excluded chains similarity...")
+    exclude_biounits = []
+    for fn in tqdm(
+        os.listdir(os.path.join(local_datasets_folder, f"proteinflow_{tag}"))
+    ):
+        if not fn.endswith(".pickle"):
+            continue
+        fp = os.path.join(local_datasets_folder, f"proteinflow_{tag}", fn)
+        with open(fp, "rb") as f:
+            entry = pickle.load(f)
+        break_flag = False
+        for chain, chain_data in entry.items():
+            for seq in sequences:
+                if (
+                    editdistance.eval(seq, chain_data["seq"]) / len(seq)
+                    < 1 - exclude_threshold
+                ):
+                    exclude_biounits.append(fn)
+                    break_flag = True
+                    break
+            if break_flag:
+                break
+
+    # return list of biounits to exclude
+    return exclude_biounits
+
+
+def _split_data(
+    dataset_path="./data/proteinflow_20221110/",
+    excluded_files=None,
+    exclude_clusters=False,
+    exclude_based_on_cdr=None,
+):
+    """Rearrange files into folders according to the dataset split dictionaries at `dataset_path/splits_dict`.
+
+    Parameters
+    ----------
+    dataset_path : str, default "./data/proteinflow_20221110/"
+        The path to the dataset folder containing pre-processed entries and a `splits_dict` folder with split dictionaries (downloaded or generated with `get_split_dictionaries`)
+    excluded_files : list, optional
+        A list of files to exclude from the dataset
+    exclude_clusters : bool, default False
+        If True, exclude all files in a cluster if at least one file in the cluster is in `excluded_files`
+    exclude_based_on_cdr : str, optional
+        If not `None`, exclude all files in a cluster if the cluster name does not end with `exclude_based_on_cdr`
+
+    """
+    if excluded_files is None:
+        excluded_files = []
+
+    dict_folder = os.path.join(dataset_path, "splits_dict")
+    with open(os.path.join(dict_folder, "train.pickle"), "rb") as f:
+        train_clusters_dict = pickle.load(f)
+    with open(os.path.join(dict_folder, "valid.pickle"), "rb") as f:
+        valid_clusters_dict = pickle.load(f)
+    with open(os.path.join(dict_folder, "test.pickle"), "rb") as f:
+        test_clusters_dict = pickle.load(f)
+
+    train_biounits = _biounits_in_clusters_dict(train_clusters_dict, excluded_files)
+    valid_biounits = _biounits_in_clusters_dict(valid_clusters_dict, excluded_files)
+    test_biounits = _biounits_in_clusters_dict(test_clusters_dict, excluded_files)
+    train_path = os.path.join(dataset_path, "train")
+    valid_path = os.path.join(dataset_path, "valid")
+    test_path = os.path.join(dataset_path, "test")
+
+    if not os.path.exists(dataset_path):
+        os.makedirs(dataset_path)
+
+    if not os.path.exists(train_path):
+        os.makedirs(train_path)
+    if not os.path.exists(valid_path):
+        os.makedirs(valid_path)
+    if not os.path.exists(test_path):
+        os.makedirs(test_path)
+
+    if len(excluded_files) > 0:
+        set_to_exclude = set(excluded_files)
+        excluded_files = set()
+        excluded_clusters_dict = defaultdict(set)
+        if exclude_clusters:
+            for clusters_dict in [
+                train_clusters_dict,
+                valid_clusters_dict,
+                test_clusters_dict,
+            ]:
+                subset_excluded_set, subset_excluded_dict = _exclude(
+                    clusters_dict, set_to_exclude, exclude_based_on_cdr
+                )
+                excluded_files.update(subset_excluded_set)
+                excluded_clusters_dict.update(subset_excluded_dict)
+        excluded_files.update(set_to_exclude)
+        excluded_clusters_dict = {k: list(v) for k, v in excluded_clusters_dict.items()}
+        excluded_path = os.path.join(dataset_path, "excluded")
+        if not os.path.exists(excluded_path):
+            os.makedirs(excluded_path)
+        print("Updating the split dictionaries...")
+        with open(os.path.join(dict_folder, "train.pickle"), "wb") as f:
+            pickle.dump(train_clusters_dict, f)
+        with open(os.path.join(dict_folder, "excluded.pickle"), "wb") as f:
+            pickle.dump(excluded_clusters_dict, f)
+        print("Moving excluded files...")
+        for biounit in tqdm(excluded_files):
+            shutil.move(os.path.join(dataset_path, biounit), excluded_path)
+    print("Moving files in the train set...")
+    for biounit in tqdm(train_biounits):
+        shutil.move(os.path.join(dataset_path, biounit), train_path)
+    print("Moving files in the validation set...")
+    for biounit in tqdm(valid_biounits):
+        shutil.move(os.path.join(dataset_path, biounit), valid_path)
+    print("Moving files in the test set...")
+    for biounit in tqdm(test_biounits):
+        shutil.move(os.path.join(dataset_path, biounit), test_path)
```

### Comparing `proteinflow-1.4.1/proteinflow.egg-info/PKG-INFO` & `proteinflow-2.0.0/proteinflow.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proteinflow
-Version: 1.4.1
+Version: 2.0.0
 Summary: Versatile pipeline for processing protein structure data for deep learning applications.
 Author-email: Liza Kozlova <liza@adaptyvbio.com>, Arthur Valentin <arthur@adaptyvbio.com>
 License: BSD-3-Clause
 Keywords: bioinformatics,dataset,protein,PDB,deep learning
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -57,15 +57,15 @@
 docker:
 ```bash
 docker pull adaptyvbio/proteinflow
 ```
 
 ### Troubleshooting
 - If you are using python 3.10 and encountering installation problems, try running `python -m pip install prody==2.4.0` before installing `proteinflow`.
-- If you are planning to generate new datasets and installed `proteinflow` with `pip`, you will need to additionally install [`mmseqs`](https://github.com/soedinglab/MMseqs2).
+- If you are planning to generate new datasets and installed `proteinflow` with `pip` (or with `conda` on Mac OS with an M1 processor), you will need to additionally install [`mmseqs`](https://github.com/soedinglab/MMseqs2).
 - Generating new datasets also depends on the `rcsbsearch` package and the latest release [v0.2.3](https://github.com/sbliven/rcsbsearch/releases/tag/v0.2.3) is currently not working correctly. The recommended fix is installing the version from [this pull request](https://github.com/sbliven/rcsbsearch/pull/6).
 ```bash
 python -m pip install "rcsbsearch @ git+https://github.com/sbliven/rcsbsearch@dbdfe3880cc88b0ce57163987db613d579400c8e"
 ```
 - The docker image can be accessed in interactive mode with this command.
 ```bash
 docker run -it -v /path/to/data:/media adaptyvbio/proteinflow bash
@@ -182,19 +182,20 @@
     ...
 ```
 See more details on available parameters and the data format in the [docs](https://adaptyvbio.github.io/ProteinFlow/) + [this repository](https://github.com/adaptyvbio/ProteinFlow-models) for a use case.
 
 ## ProteinFlow Stable Releases
 You can download them with `proteinflow download --tag {tag}` in the command line or browse in the [interface](https://proteinflow-datasets.s3.eu-west-1.amazonaws.com/index.html).
 
-|Tag    |Date    |Snapshot|Size|Min res|Min len|Max len|MMseqs thr|Split (train/val/test)|Missing thr (ends/middle)|Source|Remove redundancies|Note|
-|-------|--------|--------|----|-------|-------|-------|----------|----------------------|-------------------------|---|---|----|
-|paper|10.11.22|20220103|24G|3.5|30|10'000|0.3|90/5/5|0.3/0.1|PDB|yes|first release, no mmCIF files|
-|20230102_stable|27.02.23|20230102|28G|3.5|30|10'000|0.3|90/5/5|0.3/0.1|PDB|yes|v1.1.1|
-|20230623_sabdab|26.06.23|live 26.06.23|1.2G|3.5|30|10'000|0.3|96/3/1|0.3/0.1|SAbDab|no|v1.4.1|
+|Tag    |Date    |Snapshot|Size|Min res|Min len|Max len|Max chains|MMseqs thr|Split (train/val/test)|Missing thr (ends/middle)|Source|Remove redundancies|Note|
+|-------|--------|--------|----|-------|-------|-------|----------|----------|----------------------|-------------------------|---|---|----------------|
+|paper|10.11.22|20220103|24G|3.5|30|10'000|-|0.3|90/5/5|0.3/0.1|PDB|yes|first release, no mmCIF files|
+|20230102_stable|27.02.23|20230102|28G|3.5|30|10'000|-|0.3|90/5/5|0.3/0.1|PDB|yes|v1.1.1|
+|20230623_sabdab|26.06.23|live 26.06.23|1.4G|3.5|30|10'000|-|0.3|96/3/1|0.5/0.2|SAbDab|no|v1.4.1 (requires >= v1.4.0)|
+|20230102_v200|19.07.23|20230102|33G|3.5|30|10'000|10|0.3|90/5/5|0.3/0.1|PDB|no|v2.0.0|
 
 ## License
 The `proteinflow` package and data are released and distributed under the BSD 3-Clause License
 
 
 ## Contributions
 This is an open source project supported by [Adaptyv Bio](https://www.adaptyvbio.com/). Contributions, suggestions and bug-fixes are welcomed.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: proteinflow Version: 1.4.1 Summary: Versatile
+Metadata-Version: 2.1 Name: proteinflow Version: 2.0.0 Summary: Versatile
 pipeline for processing protein structure data for deep learning applications.
 Author-email: Liza Kozlova
 adaptyvbio.com>, Arthur Valentin
 adaptyvbio.com> License: BSD-3-Clause Keywords:
 bioinformatics,dataset,protein,PDB,deep learning Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE
   ProteinFlow - A data processing pipeline for all your protein design needs
@@ -30,21 +30,22 @@
 raw.githubusercontent.com/adaptyvbio/ProteinFlow/main/media/pf-1.png) --- ##
 Installation conda: ```bash # This should take a few minutes, be patient conda
 install -c conda-forge -c bioconda -c adaptyvbio proteinflow ``` pip: ```bash
 pip install proteinflow ``` docker: ```bash docker pull adaptyvbio/proteinflow
 ``` ### Troubleshooting - If you are using python 3.10 and encountering
 installation problems, try running `python -m pip install prody==2.4.0` before
 installing `proteinflow`. - If you are planning to generate new datasets and
-installed `proteinflow` with `pip`, you will need to additionally install
-[`mmseqs`](https://github.com/soedinglab/MMseqs2). - Generating new datasets
-also depends on the `rcsbsearch` package and the latest release [v0.2.3](https:
-//github.com/sbliven/rcsbsearch/releases/tag/v0.2.3) is currently not working
-correctly. The recommended fix is installing the version from [this pull
-request](https://github.com/sbliven/rcsbsearch/pull/6). ```bash python -m pip
-install "rcsbsearch @ git+https://github.com/sbliven/
+installed `proteinflow` with `pip` (or with `conda` on Mac OS with an M1
+processor), you will need to additionally install [`mmseqs`](https://
+github.com/soedinglab/MMseqs2). - Generating new datasets also depends on the
+`rcsbsearch` package and the latest release [v0.2.3](https://github.com/
+sbliven/rcsbsearch/releases/tag/v0.2.3) is currently not working correctly. The
+recommended fix is installing the version from [this pull request](https://
+github.com/sbliven/rcsbsearch/pull/6). ```bash python -m pip install
+"rcsbsearch @ git+https://github.com/sbliven/
 rcsbsearch@dbdfe3880cc88b0ce57163987db613d579400c8e" ``` - The docker image can
 be accessed in interactive mode with this command. ```bash docker run -it -v /
 path/to/data:/media adaptyvbio/proteinflow bash ``` ## Usage ### Downloading
 pre-computed datasets (stable) Already precomputed datasets with consensus set
 of parameters and can be accessed and downloaded using the `proteinflow`.
 package. Check the output of `proteinflow check_tags` for a list of available
 tags. ```bash proteinflow download --tag 20230102_stable ``` ### Running the
@@ -134,20 +135,20 @@
 #(B, L, 3) to_predict = batch["masked_res"] #(B, L), 1 where the residues
 should be masked, 0 otherwise ... ``` See more details on available parameters
 and the data format in the [docs](https://adaptyvbio.github.io/ProteinFlow/) +
 [this repository](https://github.com/adaptyvbio/ProteinFlow-models) for a use
 case. ## ProteinFlow Stable Releases You can download them with `proteinflow
 download --tag {tag}` in the command line or browse in the [interface](https://
 proteinflow-datasets.s3.eu-west-1.amazonaws.com/index.html). |Tag |Date
-|Snapshot|Size|Min res|Min len|Max len|MMseqs thr|Split (train/val/
+|Snapshot|Size|Min res|Min len|Max len|Max chains|MMseqs thr|Split (train/val/
 test)|Missing thr (ends/middle)|Source|Remove redundancies|Note| |-------|-----
----|--------|----|-------|-------|-------|----------|----------------------|---
-----------------------|---|---|----
-| |paper|10.11.22|20220103|24G|3.5|30|10'000|0.3|90/5/5|0.3/0.1|PDB|yes|first
-release, no mmCIF files|
-|20230102_stable|27.02.23|20230102|28G|3.5|30|10'000|0.3|90/5/5|0.3/
-0.1|PDB|yes|v1.1.1| |20230623_sabdab|26.06.23|live
-26.06.23|1.2G|3.5|30|10'000|0.3|96/3/1|0.3/0.1|SAbDab|no|v1.4.1| ## License The
-`proteinflow` package and data are released and distributed under the BSD 3-
-Clause License ## Contributions This is an open source project supported by
-[Adaptyv Bio](https://www.adaptyvbio.com/). Contributions, suggestions and bug-
-fixes are welcomed.
+---|--------|----|-------|-------|-------|----------|----------|---------------
+-------|-------------------------|---|---|----------------
+| |paper|10.11.22|20220103|24G|3.5|30|10'000|-|0.3|90/5/5|0.3/0.1|PDB|yes|first
+release, no mmCIF files| |20230102_stable|27.02.23|20230102|28G|3.5|30|10'000|-
+|0.3|90/5/5|0.3/0.1|PDB|yes|v1.1.1| |20230623_sabdab|26.06.23|live
+26.06.23|1.4G|3.5|30|10'000|-|0.3|96/3/1|0.5/0.2|SAbDab|no|v1.4.1 (requires >=
+v1.4.0)| |20230102_v200|19.07.23|20230102|33G|3.5|30|10'000|10|0.3|90/5/5|0.3/
+0.1|PDB|no|v2.0.0| ## License The `proteinflow` package and data are released
+and distributed under the BSD 3-Clause License ## Contributions This is an open
+source project supported by [Adaptyv Bio](https://www.adaptyvbio.com/).
+Contributions, suggestions and bug-fixes are welcomed.
```

### Comparing `proteinflow-1.4.1/tests/test_download.py` & `proteinflow-2.0.0/tests/test_download.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
+"""Test download."""
 import os
 import shutil
 import subprocess
 
 import pytest
 
-from proteinflow import ProteinLoader
+from proteinflow.data.torch import ProteinLoader
 
 
 @pytest.mark.parametrize("tag", ["test", "test_old"])
 def test_download(tag):
-    """Test download_data + split_data + ProteinLoader"""
-
+    """Test download_data + split_data + ProteinLoader."""
     folder = f"./data/proteinflow_{tag}"
     if os.path.exists(folder):
         shutil.rmtree(folder)
     subprocess.run(
         ["proteinflow", "download", "--tag", tag, "--skip_splitting"], check=True
     )
     subprocess.run(["proteinflow", "split", "--tag", tag], check=True)
@@ -58,8 +58,8 @@
         assert batch["sidechain_coords"].shape == (8, batch["X"].shape[1], 10, 3)
         assert batch["X"].shape[1] <= 1000
 
     shutil.rmtree(folder)
 
 
 if __name__ == "__main__":
-    test_download("test_old")
+    test_download("test")
```

### Comparing `proteinflow-1.4.1/tests/test_generate.py` & `proteinflow-2.0.0/tests/test_generate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
+"""Test generation."""
 import os
 import pickle
 import shutil
 from collections import defaultdict
 from time import time
 
 import editdistance
 
 from proteinflow import generate_data, split_data
 
 
 def get_class(seqs_dict):
-    """Check if the protein is a homomer, a heteromer or a single chain"""
-
+    """Check if the protein is a homomer, a heteromer or a single chain."""
     keys = list(seqs_dict.keys())
     if len(keys) == 1:
         return "single_chains"
     ref_seq = list(seqs_dict.values())[0]["seq"]
     for key in keys[1:]:
         value = seqs_dict[key]
         seq = value["seq"]
@@ -26,16 +26,15 @@
         ):
             return "heteromers"
     return "homomers"
 
 
 # @pytest.mark.skip()
 def test_generate():
-    """Test generate_data + split_data + chain class distribution"""
-
+    """Test generate_data + split_data + chain class distribution."""
     folder = "./data/proteinflow_test"
     if os.path.exists(folder):
         shutil.rmtree(folder)
     start = time()
     generate_data(tag="test", skip_splitting=True, n=50)
     end = time()
     num_files = len(os.listdir(folder))
```

### Comparing `proteinflow-1.4.1/tests/test_sabdab.py` & `proteinflow-2.0.0/tests/test_sabdab.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+"""Test generate_data with `sabdab=True`."""
 import os
 import shutil
 from time import time
 
-from proteinflow import ProteinLoader, generate_data
+from proteinflow import generate_data
+from proteinflow.data.torch import ProteinLoader
 
 
 # @pytest.mark.skip()
 def test_generate_sabdab():
-    """Test generate_data with `sabdab=True`"""
-
+    """Test generate_data with `sabdab=True`."""
     folder = "./data/proteinflow_test"
     if os.path.exists(folder):
         shutil.rmtree(folder)
     start = time()
     # generate_data(tag="test", n=50, sabdab=True, resolution_thr=1)
     generate_data(
         tag="test",
```

