# Comparing `tmp/omigo_ext-0.5.2.tar.gz` & `tmp/omigo_ext-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omigo_ext-0.5.2.tar", last modified: Thu May 25 19:17:08 2023, max compression
+gzip compressed data, was "omigo_ext-0.5.3.tar", last modified: Tue Jul 18 22:40:29 2023, max compression
```

## Comparing `omigo_ext-0.5.2.tar` & `omigo_ext-0.5.3.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:17:08.084353 omigo_ext-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-25 19:17:08.084353 omigo_ext-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:16:29.000000 omigo_ext-0.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-25 19:16:29.000000 omigo_ext-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-25 19:17:08.084353 omigo_ext-0.5.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:17:08.084353 omigo_ext-0.5.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:17:08.084353 omigo_ext-0.5.2/src/omigo_ext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:16:29.000000 omigo_ext-0.5.2/src/omigo_ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-25 19:16:29.000000 omigo_ext-0.5.2/src/omigo_ext/etl_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)    15651 2023-05-25 19:16:29.000000 omigo_ext-0.5.2/src/omigo_ext/graph_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     8535 2023-05-25 19:16:29.000000 omigo_ext-0.5.2/src/omigo_ext/graphviz_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-05-25 19:16:29.000000 omigo_ext-0.5.2/src/omigo_ext/kafka_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-05-25 19:16:29.000000 omigo_ext-0.5.2/src/omigo_ext/multithread_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)    10889 2023-05-25 19:16:29.000000 omigo_ext-0.5.2/src/omigo_ext/ws_ext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:17:08.084353 omigo_ext-0.5.2/src/omigo_ext.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-25 19:17:08.000000 omigo_ext-0.5.2/src/omigo_ext.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-25 19:17:08.000000 omigo_ext-0.5.2/src/omigo_ext.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 19:17:08.000000 omigo_ext-0.5.2/src/omigo_ext.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-25 19:17:08.000000 omigo_ext-0.5.2/src/omigo_ext.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-25 19:17:08.000000 omigo_ext-0.5.2/src/omigo_ext.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:40:29.459624 omigo_ext-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-18 22:40:29.459624 omigo_ext-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 22:39:56.000000 omigo_ext-0.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-18 22:39:56.000000 omigo_ext-0.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-18 22:40:29.459624 omigo_ext-0.5.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:40:29.455624 omigo_ext-0.5.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:40:29.459624 omigo_ext-0.5.3/src/omigo_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 22:39:56.000000 omigo_ext-0.5.3/src/omigo_ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-18 22:39:56.000000 omigo_ext-0.5.3/src/omigo_ext/etl_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6054 2023-07-18 22:39:56.000000 omigo_ext-0.5.3/src/omigo_ext/geomap_viz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16665 2023-07-18 22:39:56.000000 omigo_ext-0.5.3/src/omigo_ext/graph_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8535 2023-07-18 22:39:56.000000 omigo_ext-0.5.3/src/omigo_ext/graphviz_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8274 2023-07-18 22:39:56.000000 omigo_ext-0.5.3/src/omigo_ext/jira_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-07-18 22:39:56.000000 omigo_ext-0.5.3/src/omigo_ext/kafka_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-07-18 22:39:56.000000 omigo_ext-0.5.3/src/omigo_ext/multithread_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10889 2023-07-18 22:39:56.000000 omigo_ext-0.5.3/src/omigo_ext/ws_ext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:40:29.459624 omigo_ext-0.5.3/src/omigo_ext.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-18 22:40:29.000000 omigo_ext-0.5.3/src/omigo_ext.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-18 22:40:29.000000 omigo_ext-0.5.3/src/omigo_ext.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 22:40:29.000000 omigo_ext-0.5.3/src/omigo_ext.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-18 22:40:29.000000 omigo_ext-0.5.3/src/omigo_ext.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-18 22:40:29.000000 omigo_ext-0.5.3/src/omigo_ext.egg-info/top_level.txt
```

### Comparing `omigo_ext-0.5.2/setup.cfg` & `omigo_ext-0.5.3/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = omigo_ext
-version = 0.5.2
+version = 0.5.3
 author = amit jaiswal
 author_email = amit.jaiswal@gmail.com
 description = Extensions for omigo_core package
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/CrowdStrike/omigo-data-analytics
 project_urls = 
@@ -25,14 +25,16 @@
 	statistics
 	matplotlib
 	seaborn
 	omigo_core
 	kafka-python
 	google-api-python-client
 	graphviz
+	jira
+	bokeh
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `omigo_ext-0.5.2/src/omigo_ext/etl_ext.py` & `omigo_ext-0.5.3/src/omigo_ext/etl_ext.py`

 * *Files identical despite different names*

### Comparing `omigo_ext-0.5.2/src/omigo_ext/graph_ext.py` & `omigo_ext-0.5.3/src/omigo_ext/graph_ext.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,28 +18,28 @@
 
     def histogram(self, xcol, class_col = None, bins = 10, title = None, binwidth = None, xfigsize = 25, yfigsize = 5, max_class_col = 10, props = None):
         return __sns_histogram__(self, xcol, class_col, bins, title, binwidth, xfigsize, yfigsize, max_class_col, props)
 
     def ecdf(self, xcol, class_col = None, title = None, xfigsize = 25, yfigsize = 5, max_class_col = 10, props = None):
         return __sns_ecdf__(self, xcol, class_col, title, xfigsize, yfigsize, max_class_col, props)
 
-    def density(self, ycols, class_col = None, xfigsize = 25, yfigsize = 5, props = None):
-        return __sns_density__(self, ycols, class_col, xfigsize, yfigsize, props)
+    def density(self, ycols, class_col = None, title = None, xfigsize = 25, yfigsize = 5, props = None):
+        return __sns_density__(self, ycols, class_col, title, xfigsize, yfigsize, props)
 
-    def barchart(self, xcol, ycol, class_col = None, xfigsize = 25, yfigsize = 5, max_rows = 20, max_class_col = 10, props = None):
-        return __sns_barplot__(self, xcol, ycol, class_col, xfigsize, yfigsize, max_rows, max_class_col, props)
+    def barchart(self, xcol, ycol, class_col = None, title = None, xfigsize = 25, yfigsize = 5, max_rows = 20, max_class_col = 10, props = None):
+        return __sns_barplot__(self, xcol, ycol, class_col, title, xfigsize, yfigsize, max_rows, max_class_col, props)
 
-    def boxplot(self, xcol, ycol, class_col = None, xfigsize = 25, yfigsize = 5, max_rows = 20, max_class_col = 10, props = None):
-        return __sns_boxplot__(self, xcol, ycol, class_col, xfigsize, yfigsize, max_rows, max_class_col, props)
+    def boxplot(self, xcol, ycol, class_col = None, title = None, xfigsize = 25, yfigsize = 5, max_rows = 20, max_class_col = 10, props = None):
+        return __sns_boxplot__(self, xcol, ycol, class_col, title, xfigsize, yfigsize, max_rows, max_class_col, props)
 
-    def corr_heatmap(self, cols, xfigsize = 25, yfigsize = 5, max_rows = 6, props = None):
-        return __sns_corr_heatmp__(self, cols, xfigsize, yfigsize, max_rows, props)
+    def corr_heatmap(self, cols, title = None, xfigsize = 25, yfigsize = 5, max_rows = 6, props = None):
+        return __sns_corr_heatmp__(self, cols, title, xfigsize, yfigsize, max_rows, props)
 
-    def pairplot(self, cols, class_col = None, xfigsize = 5, yfigsize = 5, max_rows = 6, max_class_col = 6, props = None):
-        return __sns_pairplot__(self, cols, class_col, xfigsize, yfigsize, max_rows, max_class_col, props)
+    def pairplot(self, cols, class_col = None, title = None, xfigsize = 5, yfigsize = 5, max_rows = 6, max_class_col = 6, props = None):
+        return __sns_pairplot__(self, cols, class_col, title, xfigsize, yfigsize, max_rows, max_class_col, props)
 
 def __create_data_frame_with_types__(xtsv, xcol = None, ycols = None, zcol = None):
     # convert to array
     if (ycols is not None):
         if (utils.is_array_of_string_values(ycols) == False):
             ycols = [ycols]
 
@@ -146,15 +146,19 @@
         title = "{} vs {}".format(xcol, ycol)
 
     # take hue order
     hue_order = sorted(xtsv.col_as_array_uniq(class_col)) if (class_col is not None) else None
 
     # plot
     ax.set_title(title)
-    sns.scatterplot(ax = ax, x = xcol, y = ycol, hue = class_col, hue_order = hue_order, data = df, **props)
+    plt = sns.scatterplot(ax = ax, x = xcol, y = ycol, hue = class_col, hue_order = hue_order, data = df, **props)
+
+    # check for title
+    if (title is not None and title != ""):
+        plt.set(title = title)
 
     # return
     return VisualTSV(xtsv.get_header(), xtsv.get_data())
 
 def __sns_histogram__(xtsv, xcol, class_col, bins, title, binwidth, xfigsize, yfigsize, max_class_col, props):
     # default props
     default_props = dict(multiple = "dodge", shrink = 0.8, kde = False)
@@ -177,18 +181,23 @@
     figsize = (xfigsize, yfigsize)
     fig, ax = pyplot.subplots(figsize = figsize)
 
     # take hue order
     hue_order = sorted(xtsv.col_as_array_uniq(class_col)) if (class_col is not None) else None
 
     # binwidth overrides bins. TODO: This hue parameter is not giving class color consistently
+    plt = None
     if (binwidth is not None):
-        sns.histplot(data = df, x = xcol, hue = class_col, hue_order = hue_order, binwidth = binwidth, **props2)
+        plt = sns.histplot(data = df, x = xcol, hue = class_col, hue_order = hue_order, binwidth = binwidth, **props2)
     else:
-        sns.histplot(data = df, x = xcol, hue = class_col, hue_order = hue_order, bins = bins, **props2)
+        plt = sns.histplot(data = df, x = xcol, hue = class_col, hue_order = hue_order, bins = bins, **props2)
+
+    # check for title
+    if (title is not None and title != ""):
+        plt.set(title = title)
 
     # return
     return VisualTSV(xtsv.get_header(), xtsv.get_data())
 
 def __sns_ecdf__(xtsv, xcol, class_col, title, xfigsize, yfigsize, max_class_col, props):
     # default props
     default_props = dict()
@@ -211,21 +220,25 @@
     figsize = (xfigsize, yfigsize)
     fig, ax = pyplot.subplots(figsize = figsize)
 
     # take hue order
     hue_order = sorted(xtsv.col_as_array_uniq(class_col)) if (class_col is not None) else None
 
     # binwidth overrides bins. TODO: This hue parameter is not giving class color consistently
-    sns.ecdfplot(data = df, x = xcol, hue = class_col, hue_order = hue_order, **props2)
+    plt = sns.ecdfplot(data = df, x = xcol, hue = class_col, hue_order = hue_order, **props2)
+
+    # check for title
+    if (title is not None and title != ""):
+        plt.set(title = title)
 
     # return
     return VisualTSV(xtsv.get_header(), xtsv.get_data())
 
 # the syntax is non intuitive. need to follow row major or column major. splitting by class_col is not possible
-def __sns_density__(xtsv, ycols, class_col, xfigsize, yfigsize, props):
+def __sns_density__(xtsv, ycols, class_col, title, xfigsize, yfigsize, props):
     # default props
     default_props = dict(multiple = "layer")
     props2 = __merge_props__(props, default_props)
 
     # create df
     ycols = xtsv.__get_matching_cols__(ycols)
     df = __create_data_frame_with_types__(xtsv, None, ycols, class_col)
@@ -237,26 +250,31 @@
     # take hue order
     hue_order = sorted(xtsv.col_as_array_uniq(class_col)) if (class_col is not None) else None
 
     # TODO: This is not clean
     # multiple = props["multiple"] if (props is not None and "multiple" in props.keys()) else "layer"
 
     # check for class col
+    plt = None
     if (class_col is not None):
         if (len(ycols) == 1):
-            sns.kdeplot(data = df, x = ycols[0], hue = class_col, hue_order = hue_order, **props2)
+            plt = sns.kdeplot(data = df, x = ycols[0], hue = class_col, hue_order = hue_order, **props2)
         else:
             raise Exception("__sns_density__: class_col with multiple ycols is not supported: {}".format(ycols))
     else:
-       sns.kdeplot(data = df, **props2)
+       plt = sns.kdeplot(data = df, **props2)
+
+    # check for title
+    if (title is not None and title != ""):
+        plt.set(title = title)
 
     # return
     return VisualTSV(xtsv.get_header(), xtsv.get_data())
 
-def __sns_barplot__(xtsv, xcol, ycol, class_col, xfigsize, yfigsize, max_rows, max_class_col, props):
+def __sns_barplot__(xtsv, xcol, ycol, class_col, title, xfigsize, yfigsize, max_rows, max_class_col, props):
     # default props
     default_props = dict()
     props2 = __merge_props__(props, default_props)
 
     # check number of unique class values
     if (class_col is not None and len(xtsv.col_as_array_uniq(class_col)) >= max_class_col):
         raise Exception("Number of class column values is more than {}: {}. Probably not a class column. Try max_class_col".format(max_class_col, len(xtsv.col_as_array_uniq(class_col))))
@@ -279,20 +297,24 @@
     figsize = (xfigsize, yfigsize)
     fig, ax = pyplot.subplots(figsize = figsize)
 
     # take hue order
     hue_order = sorted(xtsv.col_as_array_uniq(class_col)) if (class_col is not None) else None
 
     # plot
-    sns.barplot(data = df, x = xcol, y = ycol, hue = class_col, hue_order = hue_order, **props2)
+    plt = sns.barplot(data = df, x = xcol, y = ycol, hue = class_col, hue_order = hue_order, **props2)
+
+    # check for title
+    if (title is not None and title != ""):
+        plt.set(title = title)
 
     # return
     return VisualTSV(xtsv.get_header(), xtsv.get_data())
 
-def __sns_boxplot__(xtsv, xcol, ycol, class_col, xfigsize, yfigsize, max_rows, max_class_col, props):
+def __sns_boxplot__(xtsv, xcol, ycol, class_col, title, xfigsize, yfigsize, max_rows, max_class_col, props):
     # default props
     default_props = dict()
     props2 = __merge_props__(props, default_props)
 
     # check number of unique class values
     if (class_col is not None and len(xtsv.col_as_array_uniq(class_col)) >= max_class_col):
         raise Exception("Number of class column values is more than {}: {}. Probably not a class column. Try max_class_col".format(max_class_col, len(xtsv.col_as_array_uniq(class_col))))
@@ -312,20 +334,24 @@
     figsize = (xfigsize, yfigsize)
     fig, ax = pyplot.subplots(figsize = figsize)
 
     # take hue order
     hue_order = sorted(xtsv.col_as_array_uniq(class_col)) if (class_col is not None) else None
 
     # plot 
-    sns.boxplot(data = df, x = xcol, y = ycol, hue = class_col, hue_order = hue_order, **props2)
+    plt = sns.boxplot(data = df, x = xcol, y = ycol, hue = class_col, hue_order = hue_order, **props2)
+
+    # check for title
+    if (title is not None and title != ""):
+        plt.set(title = title)
 
     # return
     return VisualTSV(xtsv.get_header(), xtsv.get_data())
 
-def __sns_corr_heatmp__(xtsv, cols, xfigsize, yfigsize, max_rows, props):
+def __sns_corr_heatmp__(xtsv, cols, title, xfigsize, yfigsize, max_rows, props):
     # default props
     default_props = dict(annot = True)
     props2 = __merge_props__(props, default_props)
 
     # get matching cols
     cols = xtsv.__get_matching_cols__(cols)
 
@@ -342,20 +368,24 @@
     df = __create_data_frame_with_types__(xtsv, None, cols, None)
 
     # create figure
     figsize = (xfigsize, yfigsize)
     fig, ax = pyplot.subplots(figsize = figsize)
 
     # plot
-    sns.heatmap(df.corr(), **props2)
+    plt = sns.heatmap(df.corr(), **props2)
+
+    # check for title
+    if (title is not None and title != ""):
+        plt.set(title = title)
 
     # return
     return VisualTSV(xtsv.get_header(), xtsv.get_data())
 
-def __sns_pairplot__(xtsv, cols, class_col, xfigsize, yfigsize, max_rows, max_class_col, props):
+def __sns_pairplot__(xtsv, cols, class_col, title, xfigsize, yfigsize, max_rows, max_class_col, props):
     # default props
     default_props = dict(kind = None, diag_kind = None)
     props2 = __merge_props__(props, default_props)
 
     # find matching cols
     cols = xtsv.__get_matching_cols__(cols)
 
@@ -376,12 +406,16 @@
     df = __create_data_frame_with_types__(xtsv, None, cols, class_col)
 
     # take hue order
     hue_order = sorted(xtsv.col_as_array_uniq(class_col)) if (class_col is not None) else None
 
     # define aspect and plot
     aspect = xfigsize / yfigsize
-    sns.pairplot(df, hue = class_col, hue_order = hue_order, kind = kind, diag_kind = diag_kind, aspect = aspect, height = yfigsize, **props2)
+    plt = sns.pairplot(df, hue = class_col, hue_order = hue_order, kind = kind, diag_kind = diag_kind, aspect = aspect, height = yfigsize, **props2)
+
+    # check for title
+    if (title is not None and title != ""):
+        plt.set(title = title)
 
     # return
     return VisualTSV(xtsv.get_header(), xtsv.get_data())
```

### Comparing `omigo_ext-0.5.2/src/omigo_ext/graphviz_ext.py` & `omigo_ext-0.5.3/src/omigo_ext/graphviz_ext.py`

 * *Files identical despite different names*

### Comparing `omigo_ext-0.5.2/src/omigo_ext/kafka_ext.py` & `omigo_ext-0.5.3/src/omigo_ext/kafka_ext.py`

 * *Files identical despite different names*

### Comparing `omigo_ext-0.5.2/src/omigo_ext/multithread_ext.py` & `omigo_ext-0.5.3/src/omigo_ext/multithread_ext.py`

 * *Files identical despite different names*

### Comparing `omigo_ext-0.5.2/src/omigo_ext/ws_ext.py` & `omigo_ext-0.5.3/src/omigo_ext/ws_ext.py`

 * *Files identical despite different names*

