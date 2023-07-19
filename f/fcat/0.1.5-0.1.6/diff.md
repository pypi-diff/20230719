# Comparing `tmp/fcat-0.1.5.tar.gz` & `tmp/fcat-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fcat-0.1.5.tar", last modified: Thu Feb  2 10:25:56 2023, max compression
+gzip compressed data, was "fcat-0.1.6.tar", last modified: Wed Jul 19 12:38:39 2023, max compression
```

## Comparing `fcat-0.1.5.tar` & `fcat-0.1.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 10:25:56.320360 fcat-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-02-02 10:24:47.000000 fcat-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-02 10:24:47.000000 fcat-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-02-02 10:25:56.320360 fcat-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7550 2023-02-02 10:24:47.000000 fcat-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 10:25:56.320360 fcat-0.1.5/fcat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-02 10:24:47.000000 fcat-0.1.5/fcat/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       54 2023-02-02 10:24:47.000000 fcat-0.1.5/fcat/annoToolsFcat.txt
--rw-r--r--   0 runner    (1001) docker     (123)    22946 2023-02-02 10:24:47.000000 fcat-0.1.5/fcat/assessCompleteness.py
--rw-r--r--   0 runner    (1001) docker     (123)    18192 2023-02-02 10:24:47.000000 fcat-0.1.5/fcat/calcCutoff.py
--rw-r--r--   0 runner    (1001) docker     (123)    20624 2023-02-02 10:24:47.000000 fcat-0.1.5/fcat/createPhyloprofile.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7121 2023-02-02 10:24:47.000000 fcat-0.1.5/fcat/fcat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-02-02 10:24:47.000000 fcat-0.1.5/fcat/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-02-02 10:24:47.000000 fcat-0.1.5/fcat/mergePhyloprofile.py
--rw-r--r--   0 runner    (1001) docker     (123)    25750 2023-02-02 10:24:47.000000 fcat-0.1.5/fcat/searchOrtho.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-02-02 10:24:47.000000 fcat-0.1.5/fcat/showTaxa.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 10:25:56.320360 fcat-0.1.5/fcat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-02-02 10:25:56.000000 fcat-0.1.5/fcat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-02-02 10:25:56.000000 fcat-0.1.5/fcat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-02 10:25:56.000000 fcat-0.1.5/fcat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-02-02 10:25:56.000000 fcat-0.1.5/fcat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-02-02 10:25:56.000000 fcat-0.1.5/fcat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-02 10:25:56.000000 fcat-0.1.5/fcat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-02 10:25:56.320360 fcat-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-02-02 10:24:47.000000 fcat-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:38:39.356801 fcat-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-19 12:37:25.000000 fcat-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-19 12:37:25.000000 fcat-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-07-19 12:38:39.356801 fcat-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7550 2023-07-19 12:37:25.000000 fcat-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:38:39.356801 fcat-0.1.6/fcat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 12:37:25.000000 fcat-0.1.6/fcat/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       54 2023-07-19 12:37:25.000000 fcat-0.1.6/fcat/annoToolsFcat.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    22946 2023-07-19 12:37:25.000000 fcat-0.1.6/fcat/assessCompleteness.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18192 2023-07-19 12:37:25.000000 fcat-0.1.6/fcat/calcCutoff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20624 2023-07-19 12:37:25.000000 fcat-0.1.6/fcat/createPhyloprofile.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7121 2023-07-19 12:37:25.000000 fcat-0.1.6/fcat/fcat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-19 12:37:25.000000 fcat-0.1.6/fcat/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-07-19 12:37:25.000000 fcat-0.1.6/fcat/mergePhyloprofile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26390 2023-07-19 12:37:25.000000 fcat-0.1.6/fcat/searchOrtho.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-19 12:37:25.000000 fcat-0.1.6/fcat/showTaxa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:38:39.356801 fcat-0.1.6/fcat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-07-19 12:38:39.000000 fcat-0.1.6/fcat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-19 12:38:39.000000 fcat-0.1.6/fcat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 12:38:39.000000 fcat-0.1.6/fcat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-19 12:38:39.000000 fcat-0.1.6/fcat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-19 12:38:39.000000 fcat-0.1.6/fcat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-19 12:38:39.000000 fcat-0.1.6/fcat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 12:38:39.356801 fcat-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-19 12:37:25.000000 fcat-0.1.6/setup.py
```

### Comparing `fcat-0.1.5/LICENSE` & `fcat-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fcat-0.1.5/PKG-INFO` & `fcat-0.1.6/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,118 +1,118 @@
 Metadata-Version: 2.1
 Name: fcat
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python package for fCAT, a feature-aware completeness assessment tool
 Home-page: https://github.com/BIONF/fCAT
 Author: Vinh Tran
 Author-email: tran@bio.uni-frankfurt.de
 License: GPL-3.0
-Description: # fCAT
-        [![PyPI version](https://badge.fury.io/py/fcat.svg)](https://pypi.org/project/fcat/)
-        [![Poster at: ECCB2022](https://img.shields.io/badge/Poster%20at-ECCB2022-orange)](https://doi.org/10.7490/f1000research.1119126.1)
-        [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
-        [![Build Status](https://travis-ci.com/BIONF/fCAT.svg?branch=main)](https://travis-ci.com/BIONF/fCAT)
-        ![Github Build](https://github.com/BIONF/fCAT/workflows/build/badge.svg)
-        
-        One of the critical steps in a genome sequencing project is to assess the completeness of the predicted gene set. The standard workflow starts with the identification of a set of core genes for the taxonomic group, in which the target species belongs to. The fraction of missing core genes serves then as a proxy of the target gene set completeness.
-        
-        fCAT is a **f**eature-aware **C**ompleteness **A**ssessment **T**ool, that helps to answer the question "How complete is my gene set?". In particularly, fCAT checks for the presence of conserved genes (the core genes) of a specific taxonomy clade in the target gene set using feature-aware directed ortholog search [fDOG](https://github.com/BIONF/fDOG). In addition to the length criteria for classifying the found orthologs (as same as [BUSCO](https://busco.ezlab.org)), fCAT utilizes the domain architecture similarity [FAS scores](https://github.com/BIONF/FAS) to further validate the orthologs. The later gives an alternative view on the accuracy of the target gene models, which shows how different the target orthologs in comparison to the core genes in their domain architecture.
-        
-        fCAT outputs both the summary result in a tabular text file and the phylogenetic profile of the core genes, which can be visualized using the tool [PhyloProfile](https://github.com/BIONF/PhyloProfile). By analyzing the profiles of the entire orthologous groups within a specific taxonomy clade, we can further identify and ultimately correct erroneous gene annotations.
-        
-        [Click here for the full PDF version of the ECCB2022 poster](https://doi.org/10.7490/f1000research.1119126.1)
-        
-        <p align="center">
-          <img width="500" alt="image" src="https://user-images.githubusercontent.com/19269760/202210213-5ed72144-fa43-4d60-8e90-a95df5afcca5.png">
-        </p>
-        
-        # Table of Contents
-        * [How to install](#how-to-install)
-        * [Usage](#usage)
-        * [Output](#output)
-        * [fCAT score modes](#fcat-score-modes)
-        * [Bugs](#bugs)
-        * [Contributors](#contributors)
-        * [How-To Cite](#how-to-cite)
-        * [Contact](#contact)
-        
-        # How to install
-        
-        *fCAT* tool is distributed as a python package called *fcat*. It is compatible with [Python ≥ v3.9](https://www.python.org/downloads/).
-        
-        You can install *fcat* using `pip`:
-        ```
-        python3 -m pip install fcat
-        ```
-        
-        or, in case you do not have admin rights, and don't use package systems like [Anaconda](https://docs.conda.io/projects/conda/en/latest/user-guide/install/) to manage environments you need to use the `--user` option:
-        ```
-        python3 -m pip install --user fcat
-        ```
-        
-        and then add the following line to the end of your **~/.bashrc** or **~/.bash_profile** file, restart the current terminal to apply the change (or type `source ~/.bashrc`):
-        
-        ```
-        export PATH=$HOME/.local/bin:$PATH
-        ```
-        
-        *__Note:__ fCAT requires [R](https://cran.r-project.org) to be present! Please make sure that you have R installed on your computer.*
-        
-        # Usage
-        
-        The complete process of *fCAT* can be done using one function `fcat`
-        ```
-        fcat --coreDir /path/to/fcat_data --coreSet eukaryota --refspecList "HOMSA@9606@2" --querySpecies /path/to/query.fa [--annoQuery /path/to/query.json] [--outDir /path/to/fcat/output]
-        ```
-        
-        where **eukaryota** is name of the fCAT core set (equivalent to [BUSCO](https://busco.ezlab.org/) set); **HOMSA@9606@2** is the reference species from that core set that will be used for the ortholog search; **query** is the name of species of interest. If `--annoQuery` not specified, *fCAT* fill do the feature annotation for the query proteins using [FAS tool](https://github.com/BIONF/FAS).
-        
-        # Output
-        You will find the output in the */path/to/fcat/output/fcatOutput/eukaryota/query/* folder, where */path/to/fcat/output/* could be your current directory if you not specified `--outDir` when running `fcat`. The following important output files/folders can be found:
-        
-        - *all_summary.txt*: summary of the completeness assessment using all 4 score modes
-        - *all_full.txt*: the complete assessment of 4 score modes in tab delimited file
-        - *fdogOutput.tar.gz*: a zipped file of the ortholog search result
-        - *mode_1*, *mode_2*, *mode_3* and *mode_4*: detailed output for each score mode
-        - *phyloprofileOutput*: folder contains output phylogenetic profile data that can be used with [PhyloProfile tool](https://github.com/BIONF/PhyloProfile)
-        
-        Besides, if you have already run *fCAT* for several query taxa with the same fCAT core set, you can find the merged phylogentic profiles for all of those taxa within the corresponding core set output (e.g. _/path/to/fcat/output/fcatOutput/eukaryota/*.phyloprofile_).
-        
-        # fCAT score modes
-        
-        The table below explains how the *specific ortholog group cutoffs* for each fCAT core set were calculated, and which *value of the query ortholog* is used to assess its completeness, or more precisely, its functional equivalence to the ortholog group it belongs to. If the value of a query ortholog is *not less than* its ortholog group cutoff, that group will be evaluated as **similar** or **complete**. In case co-orthologs have been predicted, the assessment for the core group will be **duplicated**. Depending on the value of each single ortholog, a *duplicated* group can be seen as **duplicated (similar)** or **duplicated (dissimilar)** in the full report (e.g. *all_full.txt*).
-        
-        | Score mode | Cutoff | Value used for comparing |
-        |---|---|---|
-        | Mode 1 - Strict mode | Mean of FAS scores between all core orthologs | Mean of FAS scores between query ortholog and all core proteins |
-        | Mode 2 - Reference mode | Mean of FAS scores between refspec and all other core orthologs | Mean of FAS scores between query ortholog and refspec protein |
-        | Mode 3 - Relaxed mode | The lower bound of the confidence interval calculated by the distribution of all-vs-all FAS score in a core group | Mean of FAS scores between query ortholog and all core proteins |
-        | Mode 4 - Length mode | Mean and standard deviation of all core protein lengths | Length of query ortholog |
-        
-        <p align="center">
-          <img width="500" alt="image" src="https://user-images.githubusercontent.com/19269760/202210343-aefbdf7b-4a38-44bf-9862-f74cc3bdd52a.png">
-        </p>
-        
-        *Note: __FAS scores__ are bidirectional FAS scors; __core protein__ or __core ortholog__ is protein in the core ortholog groups; __query protein__ or __query ortholog__ is ortholog protein of query species; __refspec__ is the specified reference species*
-        
-        # Bugs
-        Any bug reports or comments, suggestions are highly appreciated. Please [open an issue on GitHub](https://github.com/BIONF/fCAT/issues/new) or be in touch via email.
-        
-        # Contributors
-        - [Vinh Tran](https://github.com/trvinh)
-        - [Giang Nguyen](https://github.com/giangnguyen0709)
-        - [Ingo Ebersberger](https://github.com/ebersber)
-        
-        # How-To Cite
-        Tran V and Ebersberger I. fCAT: Assessing gene set completeness using domain-architecture aware targeted ortholog searches. F1000Research 2022, 11:1091 (poster) (doi: [10.7490/f1000research.1119126.1](https://doi.org/10.7490/f1000research.1119126.1))
-        
-        # Contact
-        For further support or bug reports please contact: tran@bio.uni-frankfurt.de
-        
-Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# fCAT
+[![PyPI version](https://badge.fury.io/py/fcat.svg)](https://pypi.org/project/fcat/)
+[![Poster at: ECCB2022](https://img.shields.io/badge/Poster%20at-ECCB2022-orange)](https://doi.org/10.7490/f1000research.1119126.1)
+[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
+[![Build Status](https://travis-ci.com/BIONF/fCAT.svg?branch=main)](https://travis-ci.com/BIONF/fCAT)
+![Github Build](https://github.com/BIONF/fCAT/workflows/build/badge.svg)
+
+One of the critical steps in a genome sequencing project is to assess the completeness of the predicted gene set. The standard workflow starts with the identification of a set of core genes for the taxonomic group, in which the target species belongs to. The fraction of missing core genes serves then as a proxy of the target gene set completeness.
+
+fCAT is a **f**eature-aware **C**ompleteness **A**ssessment **T**ool, that helps to answer the question "How complete is my gene set?". In particularly, fCAT checks for the presence of conserved genes (the core genes) of a specific taxonomy clade in the target gene set using feature-aware directed ortholog search [fDOG](https://github.com/BIONF/fDOG). In addition to the length criteria for classifying the found orthologs (as same as [BUSCO](https://busco.ezlab.org)), fCAT utilizes the domain architecture similarity [FAS scores](https://github.com/BIONF/FAS) to further validate the orthologs. The later gives an alternative view on the accuracy of the target gene models, which shows how different the target orthologs in comparison to the core genes in their domain architecture.
+
+fCAT outputs both the summary result in a tabular text file and the phylogenetic profile of the core genes, which can be visualized using the tool [PhyloProfile](https://github.com/BIONF/PhyloProfile). By analyzing the profiles of the entire orthologous groups within a specific taxonomy clade, we can further identify and ultimately correct erroneous gene annotations.
+
+[Click here for the full PDF version of the ECCB2022 poster](https://doi.org/10.7490/f1000research.1119126.1)
+
+<p align="center">
+  <img width="500" alt="image" src="https://user-images.githubusercontent.com/19269760/202210213-5ed72144-fa43-4d60-8e90-a95df5afcca5.png">
+</p>
+
+# Table of Contents
+* [How to install](#how-to-install)
+* [Usage](#usage)
+* [Output](#output)
+* [fCAT score modes](#fcat-score-modes)
+* [Bugs](#bugs)
+* [Contributors](#contributors)
+* [How-To Cite](#how-to-cite)
+* [Contact](#contact)
+
+# How to install
+
+*fCAT* tool is distributed as a python package called *fcat*. It is compatible with [Python ≥ v3.9](https://www.python.org/downloads/).
+
+You can install *fcat* using `pip`:
+```
+python3 -m pip install fcat
+```
+
+or, in case you do not have admin rights, and don't use package systems like [Anaconda](https://docs.conda.io/projects/conda/en/latest/user-guide/install/) to manage environments you need to use the `--user` option:
+```
+python3 -m pip install --user fcat
+```
+
+and then add the following line to the end of your **~/.bashrc** or **~/.bash_profile** file, restart the current terminal to apply the change (or type `source ~/.bashrc`):
+
+```
+export PATH=$HOME/.local/bin:$PATH
+```
+
+*__Note:__ fCAT requires [R](https://cran.r-project.org) to be present! Please make sure that you have R installed on your computer.*
+
+# Usage
+
+The complete process of *fCAT* can be done using one function `fcat`
+```
+fcat --coreDir /path/to/fcat_data --coreSet eukaryota --refspecList "HOMSA@9606@2" --querySpecies /path/to/query.fa [--annoQuery /path/to/query.json] [--outDir /path/to/fcat/output]
+```
+
+where **eukaryota** is name of the fCAT core set (equivalent to [BUSCO](https://busco.ezlab.org/) set); **HOMSA@9606@2** is the reference species from that core set that will be used for the ortholog search; **query** is the name of species of interest. If `--annoQuery` not specified, *fCAT* fill do the feature annotation for the query proteins using [FAS tool](https://github.com/BIONF/FAS).
+
+# Output
+You will find the output in the */path/to/fcat/output/fcatOutput/eukaryota/query/* folder, where */path/to/fcat/output/* could be your current directory if you not specified `--outDir` when running `fcat`. The following important output files/folders can be found:
+
+- *all_summary.txt*: summary of the completeness assessment using all 4 score modes
+- *all_full.txt*: the complete assessment of 4 score modes in tab delimited file
+- *fdogOutput.tar.gz*: a zipped file of the ortholog search result
+- *mode_1*, *mode_2*, *mode_3* and *mode_4*: detailed output for each score mode
+- *phyloprofileOutput*: folder contains output phylogenetic profile data that can be used with [PhyloProfile tool](https://github.com/BIONF/PhyloProfile)
+
+Besides, if you have already run *fCAT* for several query taxa with the same fCAT core set, you can find the merged phylogentic profiles for all of those taxa within the corresponding core set output (e.g. _/path/to/fcat/output/fcatOutput/eukaryota/*.phyloprofile_).
+
+# fCAT score modes
+
+The table below explains how the *specific ortholog group cutoffs* for each fCAT core set were calculated, and which *value of the query ortholog* is used to assess its completeness, or more precisely, its functional equivalence to the ortholog group it belongs to. If the value of a query ortholog is *not less than* its ortholog group cutoff, that group will be evaluated as **similar** or **complete**. In case co-orthologs have been predicted, the assessment for the core group will be **duplicated**. Depending on the value of each single ortholog, a *duplicated* group can be seen as **duplicated (similar)** or **duplicated (dissimilar)** in the full report (e.g. *all_full.txt*).
+
+| Score mode | Cutoff | Value used for comparing |
+|---|---|---|
+| Mode 1 - Strict mode | Mean of FAS scores between all core orthologs | Mean of FAS scores between query ortholog and all core proteins |
+| Mode 2 - Reference mode | Mean of FAS scores between refspec and all other core orthologs | Mean of FAS scores between query ortholog and refspec protein |
+| Mode 3 - Relaxed mode | The lower bound of the confidence interval calculated by the distribution of all-vs-all FAS score in a core group | Mean of FAS scores between query ortholog and all core proteins |
+| Mode 4 - Length mode | Mean and standard deviation of all core protein lengths | Length of query ortholog |
+
+<p align="center">
+  <img width="500" alt="image" src="https://user-images.githubusercontent.com/19269760/202210343-aefbdf7b-4a38-44bf-9862-f74cc3bdd52a.png">
+</p>
+
+*Note: __FAS scores__ are bidirectional FAS scors; __core protein__ or __core ortholog__ is protein in the core ortholog groups; __query protein__ or __query ortholog__ is ortholog protein of query species; __refspec__ is the specified reference species*
+
+# Bugs
+Any bug reports or comments, suggestions are highly appreciated. Please [open an issue on GitHub](https://github.com/BIONF/fCAT/issues/new) or be in touch via email.
+
+# Contributors
+- [Vinh Tran](https://github.com/trvinh)
+- [Giang Nguyen](https://github.com/giangnguyen0709)
+- [Ingo Ebersberger](https://github.com/ebersber)
+
+# How-To Cite
+Tran V and Ebersberger I. fCAT: Assessing gene set completeness using domain-architecture aware targeted ortholog searches. F1000Research 2022, 11:1091 (poster) (doi: [10.7490/f1000research.1119126.1](https://doi.org/10.7490/f1000research.1119126.1))
+
+# Contact
+For further support or bug reports please contact: tran@bio.uni-frankfurt.de
```

### Comparing `fcat-0.1.5/README.md` & `fcat-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `fcat-0.1.5/fcat/assessCompleteness.py` & `fcat-0.1.6/fcat/assessCompleteness.py`

 * *Files identical despite different names*

### Comparing `fcat-0.1.5/fcat/calcCutoff.py` & `fcat-0.1.6/fcat/calcCutoff.py`

 * *Files identical despite different names*

### Comparing `fcat-0.1.5/fcat/createPhyloprofile.py` & `fcat-0.1.6/fcat/createPhyloprofile.py`

 * *Files identical despite different names*

### Comparing `fcat-0.1.5/fcat/fcat.py` & `fcat-0.1.6/fcat/fcat.py`

 * *Files identical despite different names*

### Comparing `fcat-0.1.5/fcat/functions.py` & `fcat-0.1.6/fcat/functions.py`

 * *Files identical despite different names*

### Comparing `fcat-0.1.5/fcat/mergePhyloprofile.py` & `fcat-0.1.6/fcat/mergePhyloprofile.py`

 * *Files identical despite different names*

### Comparing `fcat-0.1.5/fcat/searchOrtho.py` & `fcat-0.1.6/fcat/searchOrtho.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,16 +154,16 @@
         sys.exit('No core group found at %s' % (coreDir + '/core_orthologs/' + coreSet))
     return(fdogJobs, ignored, groupRefspec)
 
 def runFdog(args):
     (seqFile, jobName, refSpec, outPath, coreTaxa_path, hmmPath, searchTaxa_path, force) = args
     fdog = 'fdog.run --seqFile %s --jobName %s --refspec %s --outpath %s --corepath %s --hmmpath %s --searchpath %s --fasOff --reuseCore --cpu 1' % (seqFile, jobName, refSpec, outPath, coreTaxa_path, hmmPath, searchTaxa_path)
     if force:
-        fdog = fdog + ' --force'
-    fdog = fdog + ' > /dev/null 2>&1'
+        fdog += ' --force'
+    fdog += ' > /dev/null 2>&1'
     try:
         subprocess.run([fdog], shell=True, check=True)
     except Exception as e:
         print(f'\033[91mProblem occurred while running fDOG for \'{jobName}\' core group:\033[0m\n{e}\nCommand used:\n{fdog}')
 
 
 def outputMode(outDir, coreSet, queryID, force, approach):
@@ -200,14 +200,15 @@
                                 if not queryID in f.read():
                                     missing.append(groupID)
                             shutil.copyfileobj(open(singleFa, 'rb'), mergedFaFile)
                         else:
                             missing.append(groupID)
                 mergedFaFile.close()
                 # calculate fas scores for merged extended.fa using fas.runFdogFas
+                print('Calculating pairwise FAS scores between query orthologs and sequences of refspec...')
                 fdogFAS = 'fas.runFdogFas -i %s -w %s --cores %s --redo_anno --featuretypes %s' % (mergedFa, annoDir, cpus, annoToolsFcat)
                 try:
                     subprocess.run([fdogFAS], shell=True, check=True)
                 except:
                     print('\033[91mProblem occurred while running fas.runFdogFas for \'%s\'\033[0m\n%s' % (mergedFa, fdogFAS))
     return(missing)
 
@@ -239,15 +240,18 @@
                                 else:
                                     count[groupID] = count[groupID]  + 1
                                 id  = str(count[groupID]) + '_' + s.id
                                 mergedFaFile.write('>%s\n%s\n' % (id, s.seq))
                                 for c in SeqIO.parse(groupFa, 'fasta'):
                                     mergedFaFile.write('>%s_%s|1\n%s\n' % (count[groupID], c.id, c.seq))
         mergedFaFile.close()
+        if os.stat(mergedFa).st_size == 0:
+            sys.exit('WARNING: No ortholog for any core gene found!')
         # calculate fas scores for merged _all.extended.fa using fas.runFdogFas
+        print('Calculating FAS scores between query orthologs and all sequences in each core group...')
         fdogFAS = 'fas.runFdogFas -i %s -w %s --cores %s --redo_anno --featuretypes %s' % (mergedFa, annoDir, cpus, annoToolsFcat)
         # print(fdogFAS)
         try:
             subprocess.run([fdogFAS], shell=True, check=True)
         except:
             print('\033[91mProblem occurred while running fas.runFdogFas for \'%s\'\033[0m\n%s' % (mergedFa, fdogFAS))
 
@@ -404,20 +408,26 @@
     cpus = args.cpus
     if cpus >= mp.cpu_count():
         cpus = mp.cpu_count()-1
     force = args.force
     keep = args.keep
 
     currDir = os.getcwd()
+
     # check annotation of query species and get query ID
     (doAnno, queryTaxId) = checkQueryAnno(annoQuery, annoDir, taxid, query)
     queryID = parseQueryFa(coreSet, query, annoQuery, taxid, outDir, doAnno, annoDir, cpus)
     if doAnno == False:
         if os.path.exists( '%s/query_%s.json' % (annoDir, queryTaxId)):
             os.rename('%s/query_%s.json' % (annoDir, queryTaxId), annoDir+'/'+queryID+'.json')
+    # empty old directory if force is specified
+    if force:
+        fcatFn.deleteFolder(f'{outDir}/fcatOutput/{coreSet}/{queryID}')
+        # if os.path.exists(f'{outDir}/fcatOutput/{coreSet}/{queryID}'):
+        #     shutil.rmtree(f'{outDir}/fcatOutput/{coreSet}/{queryID}')
     # move searchTaxa_dir into fcatOutput/coreSet/query folder
     src = '%s/searchTaxa_dir/%s' % (outDir, queryID)
     dest = '%s/fcatOutput/%s/%s/searchTaxa_dir/%s' % (outDir, coreSet, queryID, queryID)
     if not os.path.exists(dest):
         shutil.move(src, dest)
     # check old output files
     fcatOut = '%s/fcatOutput/%s/%s' % (outDir, coreSet, queryID)
@@ -433,34 +443,34 @@
             for job in fdogJobs:
                 tmp = runFdog(job)
                 fdogOut.append(tmp)
         else:
             pool = mp.Pool(cpus)
             for _ in tqdm(pool.imap_unordered(runFdog, fdogJobs), total=len(fdogJobs)):
                 fdogOut.append(_)
+            pool.close()
+            pool.join()
         # write ignored groups and refspec for each group based on given refspec list
         ignoredFile = open('%s/fcatOutput/%s/%s/ignored.txt' % (outDir, coreSet, queryID), 'w')
         if len(ignored) > 0:
             # print('\033[92mNo species in %s found in core set(s): %s\033[0m' % (refspecList, ','.join(ignored)))
             ignoredFile.write('\n'.join(ignored))
             ignoredFile.write('\n')
         ignoredFile.close()
         if len(groupRefspec) > 0:
             refspecFile = open('%s/fcatOutput/%s/%s/last_refspec.txt' % (outDir, coreSet, queryID), 'w')
             for g in groupRefspec:
                 refspecFile.write('%s\t%s\n' % (g, groupRefspec[g]))
             refspecFile.close()
-        pool.close()
-        pool.join()
 
     # if not status == 2:
-        print('Calculating pairwise FAS scores between query orthologs and sequences of refspec...')
-        missing = calcFAS(coreDir, outDir, coreSet, queryID, annoDir, cpus, force)
-        print('Calculating FAS scores between query orthologs and all sequences in each core group...')
+        # Calculating FAS scores between query orthologs and all sequences in each core group
         calcFASall(coreDir, outDir, coreSet, queryID, annoDir, cpus, force)
+        # Calculating pairwise FAS scores between query orthologs and sequences of refspec
+        missing = calcFAS(coreDir, outDir, coreSet, queryID, annoDir, cpus, force)
         # print('Calculating FAS scores between query orthologs and consensus sequence in each core group...')
         # calcFAScons(coreDir, outDir, coreSet, queryID, annoDir, cpus, force)
         # remove tmp folder
         if os.path.exists('%s/tmp' % fcatOut):
             shutil.rmtree('%s/tmp' % fcatOut)
         # write missing groups
         missingFile = open('%s/fcatOutput/%s/%s/missing.txt' % (outDir, coreSet, queryID), 'w')
@@ -473,14 +483,15 @@
         try:
             make_archive('%s/fdogOutput' % fcatOut, '%s/fdogOutput.tar.gz' % fcatOut, 'gztar')
         except:
             print('Cannot archiving fdog output!')
 
     if keep == False:
         fcatFn.deleteFolder('%s/fcatOutput/%s/%s/searchTaxa_dir' % (outDir, coreSet, queryID))
+        fcatFn.deleteFolder('%s/searchTaxa_dir' % outDir)
         # # print('Cleaning up...') ### no idea why rmtree not works :(
         # if os.path.exists('%s/fcatOutput/%s/%s/searchTaxa_dir' % (outDir, coreSet, queryID)):
         #     shutil.rmtree('%s/fcatOutput/%s/%s/searchTaxa_dir' % (outDir, coreSet, queryID))
     os.chdir(currDir)
     print('Done! Check output in %s' % fcatOut)
 
 def main():
```

### Comparing `fcat-0.1.5/fcat/showTaxa.py` & `fcat-0.1.6/fcat/showTaxa.py`

 * *Files identical despite different names*

### Comparing `fcat-0.1.5/fcat.egg-info/PKG-INFO` & `fcat-0.1.6/fcat.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,118 +1,118 @@
 Metadata-Version: 2.1
 Name: fcat
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python package for fCAT, a feature-aware completeness assessment tool
 Home-page: https://github.com/BIONF/fCAT
 Author: Vinh Tran
 Author-email: tran@bio.uni-frankfurt.de
 License: GPL-3.0
-Description: # fCAT
-        [![PyPI version](https://badge.fury.io/py/fcat.svg)](https://pypi.org/project/fcat/)
-        [![Poster at: ECCB2022](https://img.shields.io/badge/Poster%20at-ECCB2022-orange)](https://doi.org/10.7490/f1000research.1119126.1)
-        [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
-        [![Build Status](https://travis-ci.com/BIONF/fCAT.svg?branch=main)](https://travis-ci.com/BIONF/fCAT)
-        ![Github Build](https://github.com/BIONF/fCAT/workflows/build/badge.svg)
-        
-        One of the critical steps in a genome sequencing project is to assess the completeness of the predicted gene set. The standard workflow starts with the identification of a set of core genes for the taxonomic group, in which the target species belongs to. The fraction of missing core genes serves then as a proxy of the target gene set completeness.
-        
-        fCAT is a **f**eature-aware **C**ompleteness **A**ssessment **T**ool, that helps to answer the question "How complete is my gene set?". In particularly, fCAT checks for the presence of conserved genes (the core genes) of a specific taxonomy clade in the target gene set using feature-aware directed ortholog search [fDOG](https://github.com/BIONF/fDOG). In addition to the length criteria for classifying the found orthologs (as same as [BUSCO](https://busco.ezlab.org)), fCAT utilizes the domain architecture similarity [FAS scores](https://github.com/BIONF/FAS) to further validate the orthologs. The later gives an alternative view on the accuracy of the target gene models, which shows how different the target orthologs in comparison to the core genes in their domain architecture.
-        
-        fCAT outputs both the summary result in a tabular text file and the phylogenetic profile of the core genes, which can be visualized using the tool [PhyloProfile](https://github.com/BIONF/PhyloProfile). By analyzing the profiles of the entire orthologous groups within a specific taxonomy clade, we can further identify and ultimately correct erroneous gene annotations.
-        
-        [Click here for the full PDF version of the ECCB2022 poster](https://doi.org/10.7490/f1000research.1119126.1)
-        
-        <p align="center">
-          <img width="500" alt="image" src="https://user-images.githubusercontent.com/19269760/202210213-5ed72144-fa43-4d60-8e90-a95df5afcca5.png">
-        </p>
-        
-        # Table of Contents
-        * [How to install](#how-to-install)
-        * [Usage](#usage)
-        * [Output](#output)
-        * [fCAT score modes](#fcat-score-modes)
-        * [Bugs](#bugs)
-        * [Contributors](#contributors)
-        * [How-To Cite](#how-to-cite)
-        * [Contact](#contact)
-        
-        # How to install
-        
-        *fCAT* tool is distributed as a python package called *fcat*. It is compatible with [Python ≥ v3.9](https://www.python.org/downloads/).
-        
-        You can install *fcat* using `pip`:
-        ```
-        python3 -m pip install fcat
-        ```
-        
-        or, in case you do not have admin rights, and don't use package systems like [Anaconda](https://docs.conda.io/projects/conda/en/latest/user-guide/install/) to manage environments you need to use the `--user` option:
-        ```
-        python3 -m pip install --user fcat
-        ```
-        
-        and then add the following line to the end of your **~/.bashrc** or **~/.bash_profile** file, restart the current terminal to apply the change (or type `source ~/.bashrc`):
-        
-        ```
-        export PATH=$HOME/.local/bin:$PATH
-        ```
-        
-        *__Note:__ fCAT requires [R](https://cran.r-project.org) to be present! Please make sure that you have R installed on your computer.*
-        
-        # Usage
-        
-        The complete process of *fCAT* can be done using one function `fcat`
-        ```
-        fcat --coreDir /path/to/fcat_data --coreSet eukaryota --refspecList "HOMSA@9606@2" --querySpecies /path/to/query.fa [--annoQuery /path/to/query.json] [--outDir /path/to/fcat/output]
-        ```
-        
-        where **eukaryota** is name of the fCAT core set (equivalent to [BUSCO](https://busco.ezlab.org/) set); **HOMSA@9606@2** is the reference species from that core set that will be used for the ortholog search; **query** is the name of species of interest. If `--annoQuery` not specified, *fCAT* fill do the feature annotation for the query proteins using [FAS tool](https://github.com/BIONF/FAS).
-        
-        # Output
-        You will find the output in the */path/to/fcat/output/fcatOutput/eukaryota/query/* folder, where */path/to/fcat/output/* could be your current directory if you not specified `--outDir` when running `fcat`. The following important output files/folders can be found:
-        
-        - *all_summary.txt*: summary of the completeness assessment using all 4 score modes
-        - *all_full.txt*: the complete assessment of 4 score modes in tab delimited file
-        - *fdogOutput.tar.gz*: a zipped file of the ortholog search result
-        - *mode_1*, *mode_2*, *mode_3* and *mode_4*: detailed output for each score mode
-        - *phyloprofileOutput*: folder contains output phylogenetic profile data that can be used with [PhyloProfile tool](https://github.com/BIONF/PhyloProfile)
-        
-        Besides, if you have already run *fCAT* for several query taxa with the same fCAT core set, you can find the merged phylogentic profiles for all of those taxa within the corresponding core set output (e.g. _/path/to/fcat/output/fcatOutput/eukaryota/*.phyloprofile_).
-        
-        # fCAT score modes
-        
-        The table below explains how the *specific ortholog group cutoffs* for each fCAT core set were calculated, and which *value of the query ortholog* is used to assess its completeness, or more precisely, its functional equivalence to the ortholog group it belongs to. If the value of a query ortholog is *not less than* its ortholog group cutoff, that group will be evaluated as **similar** or **complete**. In case co-orthologs have been predicted, the assessment for the core group will be **duplicated**. Depending on the value of each single ortholog, a *duplicated* group can be seen as **duplicated (similar)** or **duplicated (dissimilar)** in the full report (e.g. *all_full.txt*).
-        
-        | Score mode | Cutoff | Value used for comparing |
-        |---|---|---|
-        | Mode 1 - Strict mode | Mean of FAS scores between all core orthologs | Mean of FAS scores between query ortholog and all core proteins |
-        | Mode 2 - Reference mode | Mean of FAS scores between refspec and all other core orthologs | Mean of FAS scores between query ortholog and refspec protein |
-        | Mode 3 - Relaxed mode | The lower bound of the confidence interval calculated by the distribution of all-vs-all FAS score in a core group | Mean of FAS scores between query ortholog and all core proteins |
-        | Mode 4 - Length mode | Mean and standard deviation of all core protein lengths | Length of query ortholog |
-        
-        <p align="center">
-          <img width="500" alt="image" src="https://user-images.githubusercontent.com/19269760/202210343-aefbdf7b-4a38-44bf-9862-f74cc3bdd52a.png">
-        </p>
-        
-        *Note: __FAS scores__ are bidirectional FAS scors; __core protein__ or __core ortholog__ is protein in the core ortholog groups; __query protein__ or __query ortholog__ is ortholog protein of query species; __refspec__ is the specified reference species*
-        
-        # Bugs
-        Any bug reports or comments, suggestions are highly appreciated. Please [open an issue on GitHub](https://github.com/BIONF/fCAT/issues/new) or be in touch via email.
-        
-        # Contributors
-        - [Vinh Tran](https://github.com/trvinh)
-        - [Giang Nguyen](https://github.com/giangnguyen0709)
-        - [Ingo Ebersberger](https://github.com/ebersber)
-        
-        # How-To Cite
-        Tran V and Ebersberger I. fCAT: Assessing gene set completeness using domain-architecture aware targeted ortholog searches. F1000Research 2022, 11:1091 (poster) (doi: [10.7490/f1000research.1119126.1](https://doi.org/10.7490/f1000research.1119126.1))
-        
-        # Contact
-        For further support or bug reports please contact: tran@bio.uni-frankfurt.de
-        
-Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# fCAT
+[![PyPI version](https://badge.fury.io/py/fcat.svg)](https://pypi.org/project/fcat/)
+[![Poster at: ECCB2022](https://img.shields.io/badge/Poster%20at-ECCB2022-orange)](https://doi.org/10.7490/f1000research.1119126.1)
+[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
+[![Build Status](https://travis-ci.com/BIONF/fCAT.svg?branch=main)](https://travis-ci.com/BIONF/fCAT)
+![Github Build](https://github.com/BIONF/fCAT/workflows/build/badge.svg)
+
+One of the critical steps in a genome sequencing project is to assess the completeness of the predicted gene set. The standard workflow starts with the identification of a set of core genes for the taxonomic group, in which the target species belongs to. The fraction of missing core genes serves then as a proxy of the target gene set completeness.
+
+fCAT is a **f**eature-aware **C**ompleteness **A**ssessment **T**ool, that helps to answer the question "How complete is my gene set?". In particularly, fCAT checks for the presence of conserved genes (the core genes) of a specific taxonomy clade in the target gene set using feature-aware directed ortholog search [fDOG](https://github.com/BIONF/fDOG). In addition to the length criteria for classifying the found orthologs (as same as [BUSCO](https://busco.ezlab.org)), fCAT utilizes the domain architecture similarity [FAS scores](https://github.com/BIONF/FAS) to further validate the orthologs. The later gives an alternative view on the accuracy of the target gene models, which shows how different the target orthologs in comparison to the core genes in their domain architecture.
+
+fCAT outputs both the summary result in a tabular text file and the phylogenetic profile of the core genes, which can be visualized using the tool [PhyloProfile](https://github.com/BIONF/PhyloProfile). By analyzing the profiles of the entire orthologous groups within a specific taxonomy clade, we can further identify and ultimately correct erroneous gene annotations.
+
+[Click here for the full PDF version of the ECCB2022 poster](https://doi.org/10.7490/f1000research.1119126.1)
+
+<p align="center">
+  <img width="500" alt="image" src="https://user-images.githubusercontent.com/19269760/202210213-5ed72144-fa43-4d60-8e90-a95df5afcca5.png">
+</p>
+
+# Table of Contents
+* [How to install](#how-to-install)
+* [Usage](#usage)
+* [Output](#output)
+* [fCAT score modes](#fcat-score-modes)
+* [Bugs](#bugs)
+* [Contributors](#contributors)
+* [How-To Cite](#how-to-cite)
+* [Contact](#contact)
+
+# How to install
+
+*fCAT* tool is distributed as a python package called *fcat*. It is compatible with [Python ≥ v3.9](https://www.python.org/downloads/).
+
+You can install *fcat* using `pip`:
+```
+python3 -m pip install fcat
+```
+
+or, in case you do not have admin rights, and don't use package systems like [Anaconda](https://docs.conda.io/projects/conda/en/latest/user-guide/install/) to manage environments you need to use the `--user` option:
+```
+python3 -m pip install --user fcat
+```
+
+and then add the following line to the end of your **~/.bashrc** or **~/.bash_profile** file, restart the current terminal to apply the change (or type `source ~/.bashrc`):
+
+```
+export PATH=$HOME/.local/bin:$PATH
+```
+
+*__Note:__ fCAT requires [R](https://cran.r-project.org) to be present! Please make sure that you have R installed on your computer.*
+
+# Usage
+
+The complete process of *fCAT* can be done using one function `fcat`
+```
+fcat --coreDir /path/to/fcat_data --coreSet eukaryota --refspecList "HOMSA@9606@2" --querySpecies /path/to/query.fa [--annoQuery /path/to/query.json] [--outDir /path/to/fcat/output]
+```
+
+where **eukaryota** is name of the fCAT core set (equivalent to [BUSCO](https://busco.ezlab.org/) set); **HOMSA@9606@2** is the reference species from that core set that will be used for the ortholog search; **query** is the name of species of interest. If `--annoQuery` not specified, *fCAT* fill do the feature annotation for the query proteins using [FAS tool](https://github.com/BIONF/FAS).
+
+# Output
+You will find the output in the */path/to/fcat/output/fcatOutput/eukaryota/query/* folder, where */path/to/fcat/output/* could be your current directory if you not specified `--outDir` when running `fcat`. The following important output files/folders can be found:
+
+- *all_summary.txt*: summary of the completeness assessment using all 4 score modes
+- *all_full.txt*: the complete assessment of 4 score modes in tab delimited file
+- *fdogOutput.tar.gz*: a zipped file of the ortholog search result
+- *mode_1*, *mode_2*, *mode_3* and *mode_4*: detailed output for each score mode
+- *phyloprofileOutput*: folder contains output phylogenetic profile data that can be used with [PhyloProfile tool](https://github.com/BIONF/PhyloProfile)
+
+Besides, if you have already run *fCAT* for several query taxa with the same fCAT core set, you can find the merged phylogentic profiles for all of those taxa within the corresponding core set output (e.g. _/path/to/fcat/output/fcatOutput/eukaryota/*.phyloprofile_).
+
+# fCAT score modes
+
+The table below explains how the *specific ortholog group cutoffs* for each fCAT core set were calculated, and which *value of the query ortholog* is used to assess its completeness, or more precisely, its functional equivalence to the ortholog group it belongs to. If the value of a query ortholog is *not less than* its ortholog group cutoff, that group will be evaluated as **similar** or **complete**. In case co-orthologs have been predicted, the assessment for the core group will be **duplicated**. Depending on the value of each single ortholog, a *duplicated* group can be seen as **duplicated (similar)** or **duplicated (dissimilar)** in the full report (e.g. *all_full.txt*).
+
+| Score mode | Cutoff | Value used for comparing |
+|---|---|---|
+| Mode 1 - Strict mode | Mean of FAS scores between all core orthologs | Mean of FAS scores between query ortholog and all core proteins |
+| Mode 2 - Reference mode | Mean of FAS scores between refspec and all other core orthologs | Mean of FAS scores between query ortholog and refspec protein |
+| Mode 3 - Relaxed mode | The lower bound of the confidence interval calculated by the distribution of all-vs-all FAS score in a core group | Mean of FAS scores between query ortholog and all core proteins |
+| Mode 4 - Length mode | Mean and standard deviation of all core protein lengths | Length of query ortholog |
+
+<p align="center">
+  <img width="500" alt="image" src="https://user-images.githubusercontent.com/19269760/202210343-aefbdf7b-4a38-44bf-9862-f74cc3bdd52a.png">
+</p>
+
+*Note: __FAS scores__ are bidirectional FAS scors; __core protein__ or __core ortholog__ is protein in the core ortholog groups; __query protein__ or __query ortholog__ is ortholog protein of query species; __refspec__ is the specified reference species*
+
+# Bugs
+Any bug reports or comments, suggestions are highly appreciated. Please [open an issue on GitHub](https://github.com/BIONF/fCAT/issues/new) or be in touch via email.
+
+# Contributors
+- [Vinh Tran](https://github.com/trvinh)
+- [Giang Nguyen](https://github.com/giangnguyen0709)
+- [Ingo Ebersberger](https://github.com/ebersber)
+
+# How-To Cite
+Tran V and Ebersberger I. fCAT: Assessing gene set completeness using domain-architecture aware targeted ortholog searches. F1000Research 2022, 11:1091 (poster) (doi: [10.7490/f1000research.1119126.1](https://doi.org/10.7490/f1000research.1119126.1))
+
+# Contact
+For further support or bug reports please contact: tran@bio.uni-frankfurt.de
```

### Comparing `fcat-0.1.5/setup.py` & `fcat-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as input:
     long_description = input.read()
 
 setup(
     name="fcat",
-    version="0.1.5",
+    version="0.1.6",
     python_requires='>=3.7.0',
     description="Python package for fCAT, a feature-aware completeness assessment tool",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Vinh Tran",
     author_email="tran@bio.uni-frankfurt.de",
     url="https://github.com/BIONF/fCAT",
```

