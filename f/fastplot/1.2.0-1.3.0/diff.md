# Comparing `tmp/fastplot-1.2.0.tar.gz` & `tmp/fastplot-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastplot-1.2.0.tar", last modified: Tue Sep  6 08:30:50 2022, max compression
+gzip compressed data, was "fastplot-1.3.0.tar", last modified: Wed Jul 19 11:33:06 2023, max compression
```

## Comparing `fastplot-1.2.0.tar` & `fastplot-1.3.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxr-x   0 martino   (1000) martino   (1000)        0 2022-09-06 08:30:50.036181 fastplot-1.2.0/
--rw-rw-r--   0 martino   (1000) martino   (1000)      512 2022-09-06 08:30:50.036181 fastplot-1.2.0/PKG-INFO
--rw-rw-r--   0 martino   (1000) martino   (1000)    19855 2022-09-06 08:08:07.000000 fastplot-1.2.0/README.md
-drwxrwxr-x   0 martino   (1000) martino   (1000)        0 2022-09-06 08:30:50.036181 fastplot-1.2.0/fastplot/
--rw-rw-r--   0 martino   (1000) martino   (1000)    14898 2022-09-06 08:29:54.000000 fastplot-1.2.0/fastplot/__init__.py
-drwxrwxr-x   0 martino   (1000) martino   (1000)        0 2022-09-06 08:30:50.036181 fastplot-1.2.0/fastplot.egg-info/
--rw-rw-r--   0 martino   (1000) martino   (1000)      512 2022-09-06 08:30:50.000000 fastplot-1.2.0/fastplot.egg-info/PKG-INFO
--rw-rw-r--   0 martino   (1000) martino   (1000)      198 2022-09-06 08:30:50.000000 fastplot-1.2.0/fastplot.egg-info/SOURCES.txt
--rw-rw-r--   0 martino   (1000) martino   (1000)        1 2022-09-06 08:30:50.000000 fastplot-1.2.0/fastplot.egg-info/dependency_links.txt
--rw-rw-r--   0 martino   (1000) martino   (1000)       50 2022-09-06 08:30:50.000000 fastplot-1.2.0/fastplot.egg-info/requires.txt
--rw-rw-r--   0 martino   (1000) martino   (1000)        9 2022-09-06 08:30:50.000000 fastplot-1.2.0/fastplot.egg-info/top_level.txt
--rw-rw-r--   0 martino   (1000) martino   (1000)       38 2022-09-06 08:30:50.036181 fastplot-1.2.0/setup.cfg
--rw-rw-r--   0 martino   (1000) martino   (1000)      874 2022-09-06 08:30:25.000000 fastplot-1.2.0/setup.py
+drwxrwxr-x   0 martino   (1000) martino   (1000)        0 2023-07-19 11:33:06.247505 fastplot-1.3.0/
+-rw-rw-r--   0 martino   (1000) martino   (1000)    35149 2023-04-03 13:22:45.000000 fastplot-1.3.0/LICENSE
+-rw-rw-r--   0 martino   (1000) martino   (1000)      495 2023-07-19 11:33:06.247505 fastplot-1.3.0/PKG-INFO
+-rw-rw-r--   0 martino   (1000) martino   (1000)    19855 2023-04-03 13:22:45.000000 fastplot-1.3.0/README.md
+drwxrwxr-x   0 martino   (1000) martino   (1000)        0 2023-07-19 11:33:06.247505 fastplot-1.3.0/fastplot/
+-rw-rw-r--   0 martino   (1000) martino   (1000)    14923 2023-07-19 11:30:29.000000 fastplot-1.3.0/fastplot/__init__.py
+drwxrwxr-x   0 martino   (1000) martino   (1000)        0 2023-07-19 11:33:06.247505 fastplot-1.3.0/fastplot.egg-info/
+-rw-rw-r--   0 martino   (1000) martino   (1000)      495 2023-07-19 11:33:06.000000 fastplot-1.3.0/fastplot.egg-info/PKG-INFO
+-rw-rw-r--   0 martino   (1000) martino   (1000)      206 2023-07-19 11:33:06.000000 fastplot-1.3.0/fastplot.egg-info/SOURCES.txt
+-rw-rw-r--   0 martino   (1000) martino   (1000)        1 2023-07-19 11:33:06.000000 fastplot-1.3.0/fastplot.egg-info/dependency_links.txt
+-rw-rw-r--   0 martino   (1000) martino   (1000)       50 2023-07-19 11:33:06.000000 fastplot-1.3.0/fastplot.egg-info/requires.txt
+-rw-rw-r--   0 martino   (1000) martino   (1000)        9 2023-07-19 11:33:06.000000 fastplot-1.3.0/fastplot.egg-info/top_level.txt
+-rw-rw-r--   0 martino   (1000) martino   (1000)       38 2023-07-19 11:33:06.247505 fastplot-1.3.0/setup.cfg
+-rw-rw-r--   0 martino   (1000) martino   (1000)      874 2023-07-19 11:32:55.000000 fastplot-1.3.0/setup.py
```

### Comparing `fastplot-1.2.0/README.md` & `fastplot-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `fastplot-1.2.0/fastplot/__init__.py` & `fastplot-1.3.0/fastplot/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/python3
 import matplotlib.pyplot as plt
-
 import matplotlib as mpl
 mpl.use('Agg')
 import matplotlib.pyplot as plt
 import matplotlib.dates as mdates
 from cycler import cycler
+from itertools import cycle
 import seaborn as sns
 import numpy as np
 import pandas as pd
 import re
 from statsmodels.distributions.empirical_distribution import ECDF
 
 # Register Pandas Converters
@@ -176,15 +176,15 @@
         if boxplot_empty:
             plt.setp(plt.gca().artists, edgecolor = 'k', facecolor='w', linewidth =1)
             plt.setp(plt.gca().lines, color='k', linewidth =1)
 
     elif mode == 'boxplot_multi':
         new_data = []
         for c in data:
-            for i, l in data[c].iteritems():
+            for i, l in data[c].items():
                 for e in l:
                     new_data.append( {"x":i, "y":e, "hue":c })
         new_data = pd.DataFrame(new_data)
         p = sns.boxplot(x="x", y="y", hue="hue", data=new_data, whis=boxplot_whis, order=data.index,
                     sym=boxplot_sym, ax=plt.gca(), palette= boxplot_palette, **plot_args)
         p.legend().remove()
         plt.xlabel("")
@@ -212,28 +212,28 @@
         plt.xlim((-0.5, len(xx) -0.5 )) # Default pretty xlim
 
     elif mode == 'bars_multi':
         xticks_labels_from_data = list(data.index)
         num_rows = len(data.index)
         num_columns = len(data.columns)
         bars_width_real=bars_width/num_columns
-        prop_iter = iter(plt.rcParams['axes.prop_cycle'])
+        prop_iter = cycle(plt.rcParams['axes.prop_cycle'])
         for i, column in enumerate( data ):
             delta = -bars_width/2 + i*bars_width_real + bars_width_real/2
             plt.bar( [e + delta for e in range(num_rows)], list(data[column]), linewidth = linewidth,
                      align = 'center', width = bars_width_real, label = column,
                      color=next(prop_iter)['color'], **plot_args)
         plt.xticks(range(num_rows), xticks_labels_from_data)
         plt.xlim((-0.5, num_rows -0.5 )) # Default pretty xlim
 
     elif mode == 'bars_stacked':
         xticks_labels_from_data = list(data.index)
         num_rows = len(data.index)
         num_columns = len(data.columns)
-        prop_iter = iter(plt.rcParams['axes.prop_cycle'])
+        prop_iter = cycle(plt.rcParams['axes.prop_cycle'])
         bottom = np.zeros(num_rows)
         for i, column in enumerate( data ):
             plt.bar(range(num_rows), list(data[column]), bottom=bottom, linewidth = linewidth,
                      align = 'center', width = bars_width, label = column,
                      color=next(prop_iter)['color'], **plot_args)
             bottom = np.add(bottom, list(data[column]))
```

### Comparing `fastplot-1.2.0/setup.py` & `fastplot-1.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 except ImportError:
     from distutils.core import setup
 
 setup(
     name="fastplot",
     description="Are you bored of re-writing code for each plot? Create publication-quality plots with a simple interface over matplotlib.",
     license="GNU GENERAL PUBLIC LICENSE v3",
-    version="1.2.0",
+    version="1.3.0",
     author="Martino Trevisan",
     author_email="martino.trevisan@polito.it",
     maintainer="Martino Trevisan",
     maintainer_email="martino.trevisan@polito.it",
     url="https://github.com/marty90/fastplot",
-    download_url = 'https://github.com/marty90/fastplot/tarball/1.2.0',
+    download_url = 'https://github.com/marty90/fastplot/tarball/1.3.0',
     packages=['fastplot'],
     install_requires=['matplotlib', 'numpy', 'pandas', 'statsmodels', 'scipy', 'seaborn']
 )
 
 # Upload on pip with:
 # Create new version
 # python setup.py sdist
```

