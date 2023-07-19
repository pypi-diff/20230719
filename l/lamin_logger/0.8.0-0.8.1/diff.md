# Comparing `tmp/lamin_logger-0.8.0.tar.gz` & `tmp/lamin_logger-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamin_logger-0.8.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lamin_logger-0.8.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lamin_logger-0.8.0.tar` & `lamin_logger-0.8.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     2370 2023-06-15 15:21:07.826183 lamin_logger-0.8.0/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2022-07-20 09:06:09.796155 lamin_logger-0.8.0/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2022-07-20 09:06:09.796533 lamin_logger-0.8.0/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1199 2022-07-20 09:06:09.775542 lamin_logger-0.8.0/.gitignore
--rw-r--r--   0        0        0     1798 2023-06-15 19:45:48.148471 lamin_logger-0.8.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11357 2022-07-28 04:40:34.570134 lamin_logger-0.8.0/LICENSE
--rw-r--r--   0        0        0      357 2022-07-24 07:22:44.261019 lamin_logger-0.8.0/README.md
--rw-r--r--   0        0        0       54 2022-07-20 09:06:09.787660 lamin_logger-0.8.0/docs/api.md
--rw-r--r--   0        0        0     5443 2023-07-17 18:29:21.249400 lamin_logger-0.8.0/docs/changelog.md
--rw-r--r--   0        0        0      124 2022-07-24 07:22:44.261457 lamin_logger-0.8.0/docs/index.md
--rw-r--r--   0        0        0     1360 2022-07-24 07:22:44.261650 lamin_logger-0.8.0/docs/quickstart.ipynb
--rw-r--r--   0        0        0      138 2022-07-20 09:06:09.769122 lamin_logger-0.8.0/lamin-project.yaml
--rw-r--r--   0        0        0      291 2023-07-17 18:29:12.752109 lamin_logger-0.8.0/lamin_logger/__init__.py
--rw-r--r--   0        0        0     1357 2023-06-15 19:45:48.149902 lamin_logger-0.8.0/lamin_logger/_core.py
--rw-r--r--   0        0        0     3825 2023-06-29 16:02:11.111265 lamin_logger-0.8.0/lamin_logger/_inspect.py
--rw-r--r--   0        0        0     7332 2023-07-05 09:32:09.706797 lamin_logger-0.8.0/lamin_logger/_logger.py
--rw-r--r--   0        0        0     4202 2023-07-05 07:03:18.906964 lamin_logger-0.8.0/lamin_logger/_lookup.py
--rw-r--r--   0        0        0     7410 2023-07-14 11:45:47.889453 lamin_logger-0.8.0/lamin_logger/_map_synonyms.py
--rw-r--r--   0        0        0      683 2023-06-15 19:45:48.150822 lamin_logger-0.8.0/lamin_logger/_python_version.py
--rw-r--r--   0        0        0     3462 2023-07-17 18:27:14.475596 lamin_logger-0.8.0/lamin_logger/_search.py
--rw-r--r--   0        0        0      321 2023-06-17 12:43:22.077332 lamin_logger-0.8.0/noxfile.py
--rw-r--r--   0        0        0      898 2023-06-17 12:43:22.077532 lamin_logger-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      115 2023-06-15 19:45:48.151666 lamin_logger-0.8.0/tests/test_base.py
--rw-r--r--   0        0        0     4154 2023-06-22 14:19:30.503574 lamin_logger-0.8.0/tests/test_inspect.py
--rw-r--r--   0        0        0     1608 2023-06-19 17:49:41.483785 lamin_logger-0.8.0/tests/test_lookup.py
--rw-r--r--   0        0        0     6153 2023-07-14 11:45:47.889627 lamin_logger-0.8.0/tests/test_map_synonyms.py
--rw-r--r--   0        0        0      417 2023-06-15 15:21:07.828069 lamin_logger-0.8.0/tests/test_notebooks.py
--rw-r--r--   0        0        0     2450 2023-07-17 18:27:14.475937 lamin_logger-0.8.0/tests/test_search.py
--rw-r--r--   0        0        0     1216 1970-01-01 00:00:00.000000 lamin_logger-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     2370 2023-06-15 15:21:07.826183 lamin_logger-0.8.1/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2022-07-20 09:06:09.796155 lamin_logger-0.8.1/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2022-07-20 09:06:09.796533 lamin_logger-0.8.1/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1199 2022-07-20 09:06:09.775542 lamin_logger-0.8.1/.gitignore
+-rw-r--r--   0        0        0     1798 2023-06-15 19:45:48.148471 lamin_logger-0.8.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11357 2022-07-28 04:40:34.570134 lamin_logger-0.8.1/LICENSE
+-rw-r--r--   0        0        0      357 2022-07-24 07:22:44.261019 lamin_logger-0.8.1/README.md
+-rw-r--r--   0        0        0       54 2022-07-20 09:06:09.787660 lamin_logger-0.8.1/docs/api.md
+-rw-r--r--   0        0        0     5604 2023-07-18 17:33:40.235423 lamin_logger-0.8.1/docs/changelog.md
+-rw-r--r--   0        0        0      124 2022-07-24 07:22:44.261457 lamin_logger-0.8.1/docs/index.md
+-rw-r--r--   0        0        0     1360 2022-07-24 07:22:44.261650 lamin_logger-0.8.1/docs/quickstart.ipynb
+-rw-r--r--   0        0        0      138 2022-07-20 09:06:09.769122 lamin_logger-0.8.1/lamin-project.yaml
+-rw-r--r--   0        0        0      291 2023-07-18 17:33:43.850088 lamin_logger-0.8.1/lamin_logger/__init__.py
+-rw-r--r--   0        0        0     1357 2023-06-15 19:45:48.149902 lamin_logger-0.8.1/lamin_logger/_core.py
+-rw-r--r--   0        0        0     3825 2023-06-29 16:02:11.111265 lamin_logger-0.8.1/lamin_logger/_inspect.py
+-rw-r--r--   0        0        0     7332 2023-07-05 09:32:09.706797 lamin_logger-0.8.1/lamin_logger/_logger.py
+-rw-r--r--   0        0        0     4202 2023-07-05 07:03:18.906964 lamin_logger-0.8.1/lamin_logger/_lookup.py
+-rw-r--r--   0        0        0     7410 2023-07-14 11:45:47.889453 lamin_logger-0.8.1/lamin_logger/_map_synonyms.py
+-rw-r--r--   0        0        0      683 2023-06-15 19:45:48.150822 lamin_logger-0.8.1/lamin_logger/_python_version.py
+-rw-r--r--   0        0        0     3652 2023-07-18 17:33:12.340863 lamin_logger-0.8.1/lamin_logger/_search.py
+-rw-r--r--   0        0        0      321 2023-06-17 12:43:22.077332 lamin_logger-0.8.1/noxfile.py
+-rw-r--r--   0        0        0      898 2023-06-17 12:43:22.077532 lamin_logger-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0      115 2023-06-15 19:45:48.151666 lamin_logger-0.8.1/tests/test_base.py
+-rw-r--r--   0        0        0     4154 2023-06-22 14:19:30.503574 lamin_logger-0.8.1/tests/test_inspect.py
+-rw-r--r--   0        0        0     1608 2023-06-19 17:49:41.483785 lamin_logger-0.8.1/tests/test_lookup.py
+-rw-r--r--   0        0        0     6153 2023-07-14 11:45:47.889627 lamin_logger-0.8.1/tests/test_map_synonyms.py
+-rw-r--r--   0        0        0      417 2023-06-15 15:21:07.828069 lamin_logger-0.8.1/tests/test_notebooks.py
+-rw-r--r--   0        0        0     2450 2023-07-18 17:30:24.928873 lamin_logger-0.8.1/tests/test_search.py
+-rw-r--r--   0        0        0     1216 1970-01-01 00:00:00.000000 lamin_logger-0.8.1/PKG-INFO
```

### Comparing `lamin_logger-0.8.0/.github/workflows/build.yml` & `lamin_logger-0.8.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.8.0/.github/workflows/latest-changes.yml` & `lamin_logger-0.8.1/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.8.0/.gitignore` & `lamin_logger-0.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.8.0/.pre-commit-config.yaml` & `lamin_logger-0.8.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.8.0/LICENSE` & `lamin_logger-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.8.0/docs/changelog.md` & `lamin_logger-0.8.1/docs/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+🎨 Return None if searching against Nones | [38](https://github.com/laminlabs/lamin-logger/pull/38) | [sunnyosun](https://github.com/sunnyosun) | 2023-07-18 |
 🎨 Always return df for `search`, added `limit=` | [37](https://github.com/laminlabs/lamin-logger/pull/37) | [sunnyosun](https://github.com/sunnyosun) | 2023-07-17 | 0.8.0
 🐛 Fix map_synonyms bug | [36](https://github.com/laminlabs/lamin-logger/pull/36) | [sunnyosun](https://github.com/sunnyosun) | 2023-07-14 | 0.7.7
 ⚡️ Speed up search 150x | [35](https://github.com/laminlabs/lamin-logger/pull/35) | [sunnyosun](https://github.com/sunnyosun) | 2023-07-10 | 0.7.6
 🐛 Fix existing_categories for map_synonyms | [34](https://github.com/laminlabs/lamin-logger/pull/34) | [sunnyosun](https://github.com/sunnyosun) | 2023-07-05 | 0.7.5
 🚑️ Fix for multiple matches in map_synonyms | [33](https://github.com/laminlabs/lamin-logger/pull/33) | [sunnyosun](https://github.com/sunnyosun) | 2023-07-02 | 0.7.4
 🚑️ Handles categorical input | [32](https://github.com/laminlabs/lamin-logger/pull/32) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-30 | 0.7.3
 🐛 Fix case sensitivity in map_synonyms | [31](https://github.com/laminlabs/lamin-logger/pull/31) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-22 | 0.7.1
```

### Comparing `lamin_logger-0.8.0/docs/quickstart.ipynb` & `lamin_logger-0.8.1/docs/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.8.0/lamin_logger/_core.py` & `lamin_logger-0.8.1/lamin_logger/_core.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.8.0/lamin_logger/_inspect.py` & `lamin_logger-0.8.1/lamin_logger/_inspect.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.8.0/lamin_logger/_logger.py` & `lamin_logger-0.8.1/lamin_logger/_logger.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.8.0/lamin_logger/_lookup.py` & `lamin_logger-0.8.1/lamin_logger/_lookup.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.8.0/lamin_logger/_map_synonyms.py` & `lamin_logger-0.8.1/lamin_logger/_map_synonyms.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.8.0/lamin_logger/_python_version.py` & `lamin_logger-0.8.1/lamin_logger/_python_version.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.8.0/lamin_logger/_search.py` & `lamin_logger-0.8.1/lamin_logger/_search.py`

 * *Files 12% similar despite different names*

```diff
@@ -44,15 +44,19 @@
         results = process.extract(
             string,
             iterable,
             scorer=fuzz.ratio,
             limit=limit,
             processor=processor,
         )
-        return pd.DataFrame(results).set_index(2)[1]
+        try:
+            return pd.DataFrame(results).set_index(2)[1]
+        except KeyError:
+            # no search results
+            return None
 
     # empty DataFrame
     if df.shape[0] == 0:
         return df
 
     # search against each of the synonyms
     if (synonyms_field in df.columns) and (synonyms_field != field):
@@ -78,20 +82,24 @@
             logger.warning(
                 "Input field is the same as synonyms field, skipping synonyms matching"
             )
         df_exp = df[[field]].copy()
         target_column = field
 
     # add matching scores as a __ratio__ column
-    df_exp["__ratio__"] = _fuzz_ratio(
+    ratios = _fuzz_ratio(
         string=string,
         iterable=df_exp[target_column],
         case_sensitive=case_sensitive,
         limit=limit,
     )
+    if ratios is None:
+        return pd.DataFrame(columns=df.columns)
+    df_exp["__ratio__"] = ratios
+
     if limit is not None:
         df_exp = df_exp[~df_exp["__ratio__"].isna()]
     # only keep the max score between field and synonyms for each entry
     if target_column == synonyms_field:
         df_exp_grouped = df_exp.groupby(field).max("__ratio__")
         # subset to original field values (as synonyms were mixed in before)
         df_exp_grouped = df_exp_grouped[df_exp_grouped.index.isin(df[field])]
```

### Comparing `lamin_logger-0.8.0/pyproject.toml` & `lamin_logger-0.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.8.0/tests/test_inspect.py` & `lamin_logger-0.8.1/tests/test_inspect.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.8.0/tests/test_lookup.py` & `lamin_logger-0.8.1/tests/test_lookup.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.8.0/tests/test_map_synonyms.py` & `lamin_logger-0.8.1/tests/test_map_synonyms.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.8.0/tests/test_search.py` & `lamin_logger-0.8.1/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `lamin_logger-0.8.0/PKG-INFO` & `lamin_logger-0.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamin_logger
-Version: 0.8.0
+Version: 0.8.1
 Summary: Logging setup.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

