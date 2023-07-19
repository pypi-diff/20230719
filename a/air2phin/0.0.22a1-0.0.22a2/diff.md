# Comparing `tmp/air2phin-0.0.22a1.tar.gz` & `tmp/air2phin-0.0.22a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "air2phin-0.0.22a1.tar", last modified: Wed Jul 19 02:35:24 2023, max compression
+gzip compressed data, was "air2phin-0.0.22a2.tar", last modified: Wed Jul 19 03:10:34 2023, max compression
```

## Comparing `air2phin-0.0.22a1.tar` & `air2phin-0.0.22a2.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 02:35:24.665345 air2phin-0.0.22a1/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     6640 2023-07-19 02:35:24.665478 air2phin-0.0.22a1/PKG-INFO
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     5189 2023-03-14 11:00:33.000000 air2phin-0.0.22a1/README.md
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2002 2023-07-19 02:35:24.665959 air2phin-0.0.22a1/setup.cfg
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1930 2023-02-27 06:29:27.000000 air2phin-0.0.22a1/setup.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 02:35:24.648187 air2phin-0.0.22a1/src/
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 02:35:24.650648 air2phin-0.0.22a1/src/air2phin/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)      841 2023-07-19 02:35:14.000000 air2phin-0.0.22a1/src/air2phin/__init__.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 02:35:24.652874 air2phin-0.0.22a1/src/air2phin/cli/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-02-27 06:29:27.000000 air2phin-0.0.22a1/src/air2phin/cli/__init__.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     6924 2023-07-18 12:06:57.000000 air2phin-0.0.22a1/src/air2phin/cli/command.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1390 2023-07-18 12:06:57.000000 air2phin-0.0.22a1/src/air2phin/constants.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 02:35:24.653049 air2phin-0.0.22a1/src/air2phin/core/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)      785 2023-02-27 06:29:27.000000 air2phin-0.0.22a1/src/air2phin/core/__init__.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 02:35:24.653885 air2phin-0.0.22a1/src/air2phin/core/rules/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-02-27 06:29:27.000000 air2phin-0.0.22a1/src/air2phin/core/rules/__init__.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)    10568 2023-07-19 02:34:17.000000 air2phin-0.0.22a1/src/air2phin/core/rules/config.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)      676 2023-07-18 12:06:57.000000 air2phin-0.0.22a1/src/air2phin/core/rules/loader.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 02:35:24.655001 air2phin-0.0.22a1/src/air2phin/core/transformer/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-02-27 06:29:27.000000 air2phin-0.0.22a1/src/air2phin/core/transformer/__init__.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     4135 2023-07-18 12:06:57.000000 air2phin-0.0.22a1/src/air2phin/core/transformer/imports.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     5602 2023-07-18 12:06:57.000000 air2phin-0.0.22a1/src/air2phin/core/transformer/operators.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     5286 2023-07-18 12:06:57.000000 air2phin-0.0.22a1/src/air2phin/core/transformer/route.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 02:35:24.655181 air2phin-0.0.22a1/src/air2phin/fake/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-02-27 06:29:27.000000 air2phin-0.0.22a1/src/air2phin/fake/__init__.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 02:35:24.655689 air2phin-0.0.22a1/src/air2phin/fake/core/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-02-27 06:29:27.000000 air2phin-0.0.22a1/src/air2phin/fake/core/__init__.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)      211 2023-02-27 06:29:27.000000 air2phin-0.0.22a1/src/air2phin/fake/core/connection.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     9328 2023-07-19 02:34:17.000000 air2phin-0.0.22a1/src/air2phin/fake/core/hook.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 02:35:24.656190 air2phin-0.0.22a1/src/air2phin/fake/hooks/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-02-27 06:29:27.000000 air2phin-0.0.22a1/src/air2phin/fake/hooks/__init__.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1264 2023-07-18 12:06:57.000000 air2phin-0.0.22a1/src/air2phin/fake/hooks/mysql.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1294 2023-07-18 12:06:57.000000 air2phin-0.0.22a1/src/air2phin/fake/hooks/postgres.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 02:35:24.656592 air2phin-0.0.22a1/src/air2phin/fake/models/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)      101 2023-03-14 11:00:33.000000 air2phin-0.0.22a1/src/air2phin/fake/models/__init__.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)      983 2023-03-15 02:15:19.000000 air2phin-0.0.22a1/src/air2phin/fake/models/variable.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 02:35:24.656960 air2phin-0.0.22a1/src/air2phin/fake/utils/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-03-14 11:00:33.000000 air2phin-0.0.22a1/src/air2phin/fake/utils/__init__.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)      875 2023-03-14 11:00:33.000000 air2phin-0.0.22a1/src/air2phin/fake/utils/trigger_rule.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 02:35:24.657511 air2phin-0.0.22a1/src/air2phin/patch/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-07-18 12:06:57.000000 air2phin-0.0.22a1/src/air2phin/patch/__init__.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1157 2023-07-18 12:06:57.000000 air2phin-0.0.22a1/src/air2phin/patch/marco_path.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 02:35:24.649359 air2phin-0.0.22a1/src/air2phin/rules/
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 02:35:24.657978 air2phin-0.0.22a1/src/air2phin/rules/core/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2170 2023-07-18 12:06:57.000000 air2phin-0.0.22a1/src/air2phin/rules/core/dagContext.yaml
--rw-r--r--   0 zhongjiajie   (501) staff       (20)      558 2023-07-18 12:06:57.000000 air2phin-0.0.22a1/src/air2phin/rules/core/removeModule.yaml
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 02:35:24.658516 air2phin-0.0.22a1/src/air2phin/rules/hooks/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)      658 2023-02-27 06:29:27.000000 air2phin-0.0.22a1/src/air2phin/rules/hooks/MySqlHook.yaml
--rw-r--r--   0 zhongjiajie   (501) staff       (20)      713 2023-02-27 06:29:27.000000 air2phin-0.0.22a1/src/air2phin/rules/hooks/PostgresHook.yaml
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 02:35:24.658884 air2phin-0.0.22a1/src/air2phin/rules/models/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1325 2023-03-14 11:00:33.000000 air2phin-0.0.22a1/src/air2phin/rules/models/Variable.yaml
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 02:35:24.663428 air2phin-0.0.22a1/src/air2phin/rules/operators/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1425 2023-03-15 02:15:19.000000 air2phin-0.0.22a1/src/air2phin/rules/operators/BashOperator.yaml
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1523 2023-07-17 08:27:58.000000 air2phin-0.0.22a1/src/air2phin/rules/operators/CheckOperator.yaml
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1771 2023-07-17 08:27:58.000000 air2phin-0.0.22a1/src/air2phin/rules/operators/CommonSensor.yaml
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1920 2023-07-17 08:27:58.000000 air2phin-0.0.22a1/src/air2phin/rules/operators/DataSyncOperator.yaml
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1149 2023-03-15 02:15:19.000000 air2phin-0.0.22a1/src/air2phin/rules/operators/DummyOperator.yaml
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1240 2023-07-17 08:27:58.000000 air2phin-0.0.22a1/src/air2phin/rules/operators/FbiRefreshOperator.yaml
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2105 2023-07-18 12:07:09.000000 air2phin-0.0.22a1/src/air2phin/rules/operators/PostgreOperator.yaml
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2057 2023-07-18 12:07:09.000000 air2phin-0.0.22a1/src/air2phin/rules/operators/PythonOperator.yaml
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1732 2023-07-18 12:07:09.000000 air2phin-0.0.22a1/src/air2phin/rules/operators/RedshiftOperator.yaml
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1604 2023-03-15 02:15:19.000000 air2phin-0.0.22a1/src/air2phin/rules/operators/SparkSqlOperator.yaml
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 02:35:24.663653 air2phin-0.0.22a1/src/air2phin/rules/utils/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)      616 2023-03-14 11:00:33.000000 air2phin-0.0.22a1/src/air2phin/rules/utils/TriggerRule.yaml
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     3519 2023-07-18 12:06:57.000000 air2phin-0.0.22a1/src/air2phin/runner.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 02:35:24.664349 air2phin-0.0.22a1/src/air2phin/utils/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-02-27 06:29:27.000000 air2phin-0.0.22a1/src/air2phin/utils/__init__.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2023 2023-07-18 12:06:57.000000 air2phin-0.0.22a1/src/air2phin/utils/file.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 02:35:24.664690 air2phin-0.0.22a1/src/air2phin/utils/marco/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-07-18 12:06:57.000000 air2phin-0.0.22a1/src/air2phin/utils/marco/__init__.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 02:35:24.665176 air2phin-0.0.22a1/src/air2phin/utils/marco/convertor/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-07-18 12:06:57.000000 air2phin-0.0.22a1/src/air2phin/utils/marco/convertor/__init__.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1713 2023-07-19 02:34:17.000000 air2phin-0.0.22a1/src/air2phin/utils/marco/convertor/base.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     3782 2023-07-18 12:06:57.000000 air2phin-0.0.22a1/src/air2phin/utils/marco/convertor/calculate.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     3636 2023-07-18 12:06:57.000000 air2phin-0.0.22a1/src/air2phin/utils/marco/helper.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1838 2023-07-18 12:06:57.000000 air2phin-0.0.22a1/src/air2phin/utils/reshape.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)      763 2023-07-18 12:06:57.000000 air2phin-0.0.22a1/src/air2phin/utils/string.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 02:35:24.652379 air2phin-0.0.22a1/src/air2phin.egg-info/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     6640 2023-07-19 02:35:24.000000 air2phin-0.0.22a1/src/air2phin.egg-info/PKG-INFO
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2228 2023-07-19 02:35:24.000000 air2phin-0.0.22a1/src/air2phin.egg-info/SOURCES.txt
--rw-r--r--   0 zhongjiajie   (501) staff       (20)        1 2023-07-19 02:35:24.000000 air2phin-0.0.22a1/src/air2phin.egg-info/dependency_links.txt
--rw-r--r--   0 zhongjiajie   (501) staff       (20)       55 2023-07-19 02:35:24.000000 air2phin-0.0.22a1/src/air2phin.egg-info/entry_points.txt
--rw-r--r--   0 zhongjiajie   (501) staff       (20)      287 2023-07-19 02:35:24.000000 air2phin-0.0.22a1/src/air2phin.egg-info/requires.txt
--rw-r--r--   0 zhongjiajie   (501) staff       (20)       14 2023-07-19 02:35:24.000000 air2phin-0.0.22a1/src/air2phin.egg-info/top_level.txt
--rw-r--r--   0 zhongjiajie   (501) staff       (20)        1 2023-02-24 09:08:53.000000 air2phin-0.0.22a1/src/air2phin.egg-info/zip-safe
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:10:34.249900 air2phin-0.0.22a2/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     6640 2023-07-19 03:10:34.250015 air2phin-0.0.22a2/PKG-INFO
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     5189 2023-03-14 11:00:33.000000 air2phin-0.0.22a2/README.md
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2002 2023-07-19 03:10:34.250489 air2phin-0.0.22a2/setup.cfg
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1930 2023-02-27 06:29:27.000000 air2phin-0.0.22a2/setup.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:10:34.232539 air2phin-0.0.22a2/src/
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:10:34.236140 air2phin-0.0.22a2/src/air2phin/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      841 2023-07-19 03:10:28.000000 air2phin-0.0.22a2/src/air2phin/__init__.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:10:34.237975 air2phin-0.0.22a2/src/air2phin/cli/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-02-27 06:29:27.000000 air2phin-0.0.22a2/src/air2phin/cli/__init__.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     6924 2023-07-18 12:06:57.000000 air2phin-0.0.22a2/src/air2phin/cli/command.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1390 2023-07-18 12:06:57.000000 air2phin-0.0.22a2/src/air2phin/constants.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:10:34.238139 air2phin-0.0.22a2/src/air2phin/core/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      785 2023-02-27 06:29:27.000000 air2phin-0.0.22a2/src/air2phin/core/__init__.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:10:34.238631 air2phin-0.0.22a2/src/air2phin/core/rules/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-02-27 06:29:27.000000 air2phin-0.0.22a2/src/air2phin/core/rules/__init__.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)    10568 2023-07-19 02:34:17.000000 air2phin-0.0.22a2/src/air2phin/core/rules/config.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      676 2023-07-18 12:06:57.000000 air2phin-0.0.22a2/src/air2phin/core/rules/loader.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:10:34.239324 air2phin-0.0.22a2/src/air2phin/core/transformer/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-02-27 06:29:27.000000 air2phin-0.0.22a2/src/air2phin/core/transformer/__init__.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     4135 2023-07-18 12:06:57.000000 air2phin-0.0.22a2/src/air2phin/core/transformer/imports.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     5602 2023-07-18 12:06:57.000000 air2phin-0.0.22a2/src/air2phin/core/transformer/operators.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     5286 2023-07-18 12:06:57.000000 air2phin-0.0.22a2/src/air2phin/core/transformer/route.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:10:34.239517 air2phin-0.0.22a2/src/air2phin/fake/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-02-27 06:29:27.000000 air2phin-0.0.22a2/src/air2phin/fake/__init__.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:10:34.240005 air2phin-0.0.22a2/src/air2phin/fake/core/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-02-27 06:29:27.000000 air2phin-0.0.22a2/src/air2phin/fake/core/__init__.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      211 2023-02-27 06:29:27.000000 air2phin-0.0.22a2/src/air2phin/fake/core/connection.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     9328 2023-07-19 02:34:17.000000 air2phin-0.0.22a2/src/air2phin/fake/core/hook.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:10:34.240643 air2phin-0.0.22a2/src/air2phin/fake/hooks/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-02-27 06:29:27.000000 air2phin-0.0.22a2/src/air2phin/fake/hooks/__init__.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1264 2023-07-18 12:06:57.000000 air2phin-0.0.22a2/src/air2phin/fake/hooks/mysql.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1294 2023-07-18 12:06:57.000000 air2phin-0.0.22a2/src/air2phin/fake/hooks/postgres.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:10:34.241208 air2phin-0.0.22a2/src/air2phin/fake/models/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      101 2023-03-14 11:00:33.000000 air2phin-0.0.22a2/src/air2phin/fake/models/__init__.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      983 2023-03-15 02:15:19.000000 air2phin-0.0.22a2/src/air2phin/fake/models/variable.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:10:34.241520 air2phin-0.0.22a2/src/air2phin/fake/utils/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-03-14 11:00:33.000000 air2phin-0.0.22a2/src/air2phin/fake/utils/__init__.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      875 2023-03-14 11:00:33.000000 air2phin-0.0.22a2/src/air2phin/fake/utils/trigger_rule.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:10:34.241899 air2phin-0.0.22a2/src/air2phin/patch/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-07-18 12:06:57.000000 air2phin-0.0.22a2/src/air2phin/patch/__init__.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1243 2023-07-19 03:09:25.000000 air2phin-0.0.22a2/src/air2phin/patch/marco_path.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:10:34.234685 air2phin-0.0.22a2/src/air2phin/rules/
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:10:34.242207 air2phin-0.0.22a2/src/air2phin/rules/core/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2170 2023-07-18 12:06:57.000000 air2phin-0.0.22a2/src/air2phin/rules/core/dagContext.yaml
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      558 2023-07-18 12:06:57.000000 air2phin-0.0.22a2/src/air2phin/rules/core/removeModule.yaml
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:10:34.242466 air2phin-0.0.22a2/src/air2phin/rules/hooks/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      658 2023-02-27 06:29:27.000000 air2phin-0.0.22a2/src/air2phin/rules/hooks/MySqlHook.yaml
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      713 2023-02-27 06:29:27.000000 air2phin-0.0.22a2/src/air2phin/rules/hooks/PostgresHook.yaml
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:10:34.242602 air2phin-0.0.22a2/src/air2phin/rules/models/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1325 2023-03-14 11:00:33.000000 air2phin-0.0.22a2/src/air2phin/rules/models/Variable.yaml
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:10:34.244860 air2phin-0.0.22a2/src/air2phin/rules/operators/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1425 2023-03-15 02:15:19.000000 air2phin-0.0.22a2/src/air2phin/rules/operators/BashOperator.yaml
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1523 2023-07-17 08:27:58.000000 air2phin-0.0.22a2/src/air2phin/rules/operators/CheckOperator.yaml
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1771 2023-07-17 08:27:58.000000 air2phin-0.0.22a2/src/air2phin/rules/operators/CommonSensor.yaml
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1920 2023-07-17 08:27:58.000000 air2phin-0.0.22a2/src/air2phin/rules/operators/DataSyncOperator.yaml
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1149 2023-03-15 02:15:19.000000 air2phin-0.0.22a2/src/air2phin/rules/operators/DummyOperator.yaml
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1240 2023-07-17 08:27:58.000000 air2phin-0.0.22a2/src/air2phin/rules/operators/FbiRefreshOperator.yaml
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2105 2023-07-18 12:07:09.000000 air2phin-0.0.22a2/src/air2phin/rules/operators/PostgreOperator.yaml
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2057 2023-07-18 12:07:09.000000 air2phin-0.0.22a2/src/air2phin/rules/operators/PythonOperator.yaml
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1732 2023-07-18 12:07:09.000000 air2phin-0.0.22a2/src/air2phin/rules/operators/RedshiftOperator.yaml
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1604 2023-03-15 02:15:19.000000 air2phin-0.0.22a2/src/air2phin/rules/operators/SparkSqlOperator.yaml
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:10:34.245023 air2phin-0.0.22a2/src/air2phin/rules/utils/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      616 2023-03-14 11:00:33.000000 air2phin-0.0.22a2/src/air2phin/rules/utils/TriggerRule.yaml
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     3519 2023-07-18 12:06:57.000000 air2phin-0.0.22a2/src/air2phin/runner.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:10:34.245609 air2phin-0.0.22a2/src/air2phin/utils/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-02-27 06:29:27.000000 air2phin-0.0.22a2/src/air2phin/utils/__init__.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2023 2023-07-18 12:06:57.000000 air2phin-0.0.22a2/src/air2phin/utils/file.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:10:34.245860 air2phin-0.0.22a2/src/air2phin/utils/marco/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-07-18 12:06:57.000000 air2phin-0.0.22a2/src/air2phin/utils/marco/__init__.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:10:34.249739 air2phin-0.0.22a2/src/air2phin/utils/marco/convertor/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-07-18 12:06:57.000000 air2phin-0.0.22a2/src/air2phin/utils/marco/convertor/__init__.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1713 2023-07-19 02:34:17.000000 air2phin-0.0.22a2/src/air2phin/utils/marco/convertor/base.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     3782 2023-07-18 12:06:57.000000 air2phin-0.0.22a2/src/air2phin/utils/marco/convertor/calculate.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     3636 2023-07-18 12:06:57.000000 air2phin-0.0.22a2/src/air2phin/utils/marco/helper.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1838 2023-07-18 12:06:57.000000 air2phin-0.0.22a2/src/air2phin/utils/reshape.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      763 2023-07-18 12:06:57.000000 air2phin-0.0.22a2/src/air2phin/utils/string.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:10:34.237530 air2phin-0.0.22a2/src/air2phin.egg-info/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     6640 2023-07-19 03:10:34.000000 air2phin-0.0.22a2/src/air2phin.egg-info/PKG-INFO
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2228 2023-07-19 03:10:34.000000 air2phin-0.0.22a2/src/air2phin.egg-info/SOURCES.txt
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)        1 2023-07-19 03:10:34.000000 air2phin-0.0.22a2/src/air2phin.egg-info/dependency_links.txt
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)       55 2023-07-19 03:10:34.000000 air2phin-0.0.22a2/src/air2phin.egg-info/entry_points.txt
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      287 2023-07-19 03:10:34.000000 air2phin-0.0.22a2/src/air2phin.egg-info/requires.txt
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)       14 2023-07-19 03:10:34.000000 air2phin-0.0.22a2/src/air2phin.egg-info/top_level.txt
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)        1 2023-02-24 09:08:53.000000 air2phin-0.0.22a2/src/air2phin.egg-info/zip-safe
```

### Comparing `air2phin-0.0.22a1/PKG-INFO` & `air2phin-0.0.22a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: air2phin
-Version: 0.0.22a1
+Version: 0.0.22a2
 Summary: Air2phin is a tool for migrating Airflow DAGs to DolphinScheduler Python API.
 Home-page: https://github.com/WhaleOps/air2phin
 Author: Jay Chung
 Author-email: zhongjiajie955@gmail.com
 License: Apache License 2.0
 Project-URL: Source, https://github.com/WhaleOps/air2phin
 Project-URL: Issue Tracker, https://github.com/WhaleOps/air2phin/issues
```

### Comparing `air2phin-0.0.22a1/README.md` & `air2phin-0.0.22a2/README.md`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a1/setup.cfg` & `air2phin-0.0.22a2/setup.cfg`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a1/setup.py` & `air2phin-0.0.22a2/setup.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a1/src/air2phin/__init__.py` & `air2phin-0.0.22a2/src/air2phin/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 __project_name__ = "Air2phin"
-__version__ = "0.0.22a1"
+__version__ = "0.0.22a2"
```

### Comparing `air2phin-0.0.22a1/src/air2phin/cli/command.py` & `air2phin-0.0.22a2/src/air2phin/cli/command.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a1/src/air2phin/constants.py` & `air2phin-0.0.22a2/src/air2phin/constants.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a1/src/air2phin/core/__init__.py` & `air2phin-0.0.22a2/src/air2phin/core/__init__.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a1/src/air2phin/core/rules/config.py` & `air2phin-0.0.22a2/src/air2phin/core/rules/config.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a1/src/air2phin/core/rules/loader.py` & `air2phin-0.0.22a2/src/air2phin/core/rules/loader.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a1/src/air2phin/core/transformer/imports.py` & `air2phin-0.0.22a2/src/air2phin/core/transformer/imports.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a1/src/air2phin/core/transformer/operators.py` & `air2phin-0.0.22a2/src/air2phin/core/transformer/operators.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a1/src/air2phin/core/transformer/route.py` & `air2phin-0.0.22a2/src/air2phin/core/transformer/route.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a1/src/air2phin/fake/core/hook.py` & `air2phin-0.0.22a2/src/air2phin/fake/core/hook.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a1/src/air2phin/fake/hooks/mysql.py` & `air2phin-0.0.22a2/src/air2phin/fake/hooks/mysql.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a1/src/air2phin/fake/hooks/postgres.py` & `air2phin-0.0.22a2/src/air2phin/fake/hooks/postgres.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a1/src/air2phin/fake/models/variable.py` & `air2phin-0.0.22a2/src/air2phin/fake/models/variable.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a1/src/air2phin/fake/utils/trigger_rule.py` & `air2phin-0.0.22a2/src/air2phin/fake/utils/trigger_rule.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a1/src/air2phin/patch/marco_path.py` & `air2phin-0.0.22a2/src/air2phin/patch/marco_path.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,16 @@
         td: timedelta = schedule2timedelta(schedule)
 
         marcos: set[DolphinHumanReadMarco] = set()
         for task_name, task in self.workflow.tasks.items():
             if task.ext_attr is not None:
                 render_field = task.ext_attr.lstrip("_")
                 srv_val = getattr(task, render_field)
+                if not isinstance(srv_val, str | bytes):
+                    continue
                 task_define_marco = helper.replace_marco(srv_val, td)
                 setattr(task, render_field, task_define_marco.content)
 
                 if task_define_marco.marco is not None:
                     marcos |= task_define_marco.marco
 
         if marcos:
```

### Comparing `air2phin-0.0.22a1/src/air2phin/rules/core/dagContext.yaml` & `air2phin-0.0.22a2/src/air2phin/rules/core/dagContext.yaml`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a1/src/air2phin/rules/core/removeModule.yaml` & `air2phin-0.0.22a2/src/air2phin/rules/core/removeModule.yaml`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a1/src/air2phin/rules/hooks/MySqlHook.yaml` & `air2phin-0.0.22a2/src/air2phin/rules/hooks/MySqlHook.yaml`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a1/src/air2phin/rules/hooks/PostgresHook.yaml` & `air2phin-0.0.22a2/src/air2phin/rules/hooks/PostgresHook.yaml`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a1/src/air2phin/rules/models/Variable.yaml` & `air2phin-0.0.22a2/src/air2phin/rules/models/Variable.yaml`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a1/src/air2phin/rules/operators/BashOperator.yaml` & `air2phin-0.0.22a2/src/air2phin/rules/operators/BashOperator.yaml`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a1/src/air2phin/rules/operators/CheckOperator.yaml` & `air2phin-0.0.22a2/src/air2phin/rules/operators/CheckOperator.yaml`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a1/src/air2phin/rules/operators/CommonSensor.yaml` & `air2phin-0.0.22a2/src/air2phin/rules/operators/CommonSensor.yaml`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a1/src/air2phin/rules/operators/DataSyncOperator.yaml` & `air2phin-0.0.22a2/src/air2phin/rules/operators/DataSyncOperator.yaml`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a1/src/air2phin/rules/operators/DummyOperator.yaml` & `air2phin-0.0.22a2/src/air2phin/rules/operators/DummyOperator.yaml`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a1/src/air2phin/rules/operators/FbiRefreshOperator.yaml` & `air2phin-0.0.22a2/src/air2phin/rules/operators/FbiRefreshOperator.yaml`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a1/src/air2phin/rules/operators/PostgreOperator.yaml` & `air2phin-0.0.22a2/src/air2phin/rules/operators/PostgreOperator.yaml`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a1/src/air2phin/rules/operators/PythonOperator.yaml` & `air2phin-0.0.22a2/src/air2phin/rules/operators/PythonOperator.yaml`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a1/src/air2phin/rules/operators/RedshiftOperator.yaml` & `air2phin-0.0.22a2/src/air2phin/rules/operators/RedshiftOperator.yaml`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a1/src/air2phin/rules/operators/SparkSqlOperator.yaml` & `air2phin-0.0.22a2/src/air2phin/rules/operators/SparkSqlOperator.yaml`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a1/src/air2phin/rules/utils/TriggerRule.yaml` & `air2phin-0.0.22a2/src/air2phin/rules/utils/TriggerRule.yaml`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a1/src/air2phin/runner.py` & `air2phin-0.0.22a2/src/air2phin/runner.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a1/src/air2phin/utils/file.py` & `air2phin-0.0.22a2/src/air2phin/utils/file.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a1/src/air2phin/utils/marco/convertor/base.py` & `air2phin-0.0.22a2/src/air2phin/utils/marco/convertor/base.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a1/src/air2phin/utils/marco/convertor/calculate.py` & `air2phin-0.0.22a2/src/air2phin/utils/marco/convertor/calculate.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a1/src/air2phin/utils/marco/helper.py` & `air2phin-0.0.22a2/src/air2phin/utils/marco/helper.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a1/src/air2phin/utils/reshape.py` & `air2phin-0.0.22a2/src/air2phin/utils/reshape.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a1/src/air2phin/utils/string.py` & `air2phin-0.0.22a2/src/air2phin/utils/string.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a1/src/air2phin.egg-info/PKG-INFO` & `air2phin-0.0.22a2/src/air2phin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: air2phin
-Version: 0.0.22a1
+Version: 0.0.22a2
 Summary: Air2phin is a tool for migrating Airflow DAGs to DolphinScheduler Python API.
 Home-page: https://github.com/WhaleOps/air2phin
 Author: Jay Chung
 Author-email: zhongjiajie955@gmail.com
 License: Apache License 2.0
 Project-URL: Source, https://github.com/WhaleOps/air2phin
 Project-URL: Issue Tracker, https://github.com/WhaleOps/air2phin/issues
```

### Comparing `air2phin-0.0.22a1/src/air2phin.egg-info/SOURCES.txt` & `air2phin-0.0.22a2/src/air2phin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

