# Comparing `tmp/air2phin-0.0.22a4.tar.gz` & `tmp/air2phin-0.0.22a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "air2phin-0.0.22a4.tar", last modified: Wed Jul 19 03:18:22 2023, max compression
+gzip compressed data, was "air2phin-0.0.22a5.tar", last modified: Wed Jul 19 06:44:57 2023, max compression
```

## Comparing `air2phin-0.0.22a4.tar` & `air2phin-0.0.22a5.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:18:22.961834 air2phin-0.0.22a4/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     6640 2023-07-19 03:18:22.961918 air2phin-0.0.22a4/PKG-INFO
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     5189 2023-03-14 11:00:33.000000 air2phin-0.0.22a4/README.md
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2002 2023-07-19 03:18:22.962305 air2phin-0.0.22a4/setup.cfg
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1930 2023-02-27 06:29:27.000000 air2phin-0.0.22a4/setup.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:18:22.952655 air2phin-0.0.22a4/src/
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:18:22.954783 air2phin-0.0.22a4/src/air2phin/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)      841 2023-07-19 03:18:17.000000 air2phin-0.0.22a4/src/air2phin/__init__.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:18:22.955887 air2phin-0.0.22a4/src/air2phin/cli/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-02-27 06:29:27.000000 air2phin-0.0.22a4/src/air2phin/cli/__init__.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     6924 2023-07-18 12:06:57.000000 air2phin-0.0.22a4/src/air2phin/cli/command.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1390 2023-07-18 12:06:57.000000 air2phin-0.0.22a4/src/air2phin/constants.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:18:22.956008 air2phin-0.0.22a4/src/air2phin/core/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)      785 2023-02-27 06:29:27.000000 air2phin-0.0.22a4/src/air2phin/core/__init__.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:18:22.956349 air2phin-0.0.22a4/src/air2phin/core/rules/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-02-27 06:29:27.000000 air2phin-0.0.22a4/src/air2phin/core/rules/__init__.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)    10568 2023-07-19 02:34:17.000000 air2phin-0.0.22a4/src/air2phin/core/rules/config.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)      676 2023-07-18 12:06:57.000000 air2phin-0.0.22a4/src/air2phin/core/rules/loader.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:18:22.956821 air2phin-0.0.22a4/src/air2phin/core/transformer/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-02-27 06:29:27.000000 air2phin-0.0.22a4/src/air2phin/core/transformer/__init__.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     4135 2023-07-18 12:06:57.000000 air2phin-0.0.22a4/src/air2phin/core/transformer/imports.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     5602 2023-07-18 12:06:57.000000 air2phin-0.0.22a4/src/air2phin/core/transformer/operators.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     5286 2023-07-18 12:06:57.000000 air2phin-0.0.22a4/src/air2phin/core/transformer/route.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:18:22.956948 air2phin-0.0.22a4/src/air2phin/fake/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-02-27 06:29:27.000000 air2phin-0.0.22a4/src/air2phin/fake/__init__.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:18:22.957279 air2phin-0.0.22a4/src/air2phin/fake/core/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-02-27 06:29:27.000000 air2phin-0.0.22a4/src/air2phin/fake/core/__init__.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)      211 2023-02-27 06:29:27.000000 air2phin-0.0.22a4/src/air2phin/fake/core/connection.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     9328 2023-07-19 02:34:17.000000 air2phin-0.0.22a4/src/air2phin/fake/core/hook.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:18:22.957641 air2phin-0.0.22a4/src/air2phin/fake/hooks/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-02-27 06:29:27.000000 air2phin-0.0.22a4/src/air2phin/fake/hooks/__init__.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1264 2023-07-18 12:06:57.000000 air2phin-0.0.22a4/src/air2phin/fake/hooks/mysql.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1294 2023-07-18 12:06:57.000000 air2phin-0.0.22a4/src/air2phin/fake/hooks/postgres.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:18:22.957869 air2phin-0.0.22a4/src/air2phin/fake/models/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)      101 2023-03-14 11:00:33.000000 air2phin-0.0.22a4/src/air2phin/fake/models/__init__.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)      983 2023-03-15 02:15:19.000000 air2phin-0.0.22a4/src/air2phin/fake/models/variable.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:18:22.958289 air2phin-0.0.22a4/src/air2phin/fake/utils/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-03-14 11:00:33.000000 air2phin-0.0.22a4/src/air2phin/fake/utils/__init__.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)      875 2023-03-14 11:00:33.000000 air2phin-0.0.22a4/src/air2phin/fake/utils/trigger_rule.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:18:22.958525 air2phin-0.0.22a4/src/air2phin/patch/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-07-18 12:06:57.000000 air2phin-0.0.22a4/src/air2phin/patch/__init__.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1244 2023-07-19 03:12:27.000000 air2phin-0.0.22a4/src/air2phin/patch/marco_path.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:18:22.953848 air2phin-0.0.22a4/src/air2phin/rules/
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:18:22.958770 air2phin-0.0.22a4/src/air2phin/rules/core/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2170 2023-07-18 12:06:57.000000 air2phin-0.0.22a4/src/air2phin/rules/core/dagContext.yaml
--rw-r--r--   0 zhongjiajie   (501) staff       (20)      558 2023-07-18 12:06:57.000000 air2phin-0.0.22a4/src/air2phin/rules/core/removeModule.yaml
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:18:22.959019 air2phin-0.0.22a4/src/air2phin/rules/hooks/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)      658 2023-02-27 06:29:27.000000 air2phin-0.0.22a4/src/air2phin/rules/hooks/MySqlHook.yaml
--rw-r--r--   0 zhongjiajie   (501) staff       (20)      713 2023-02-27 06:29:27.000000 air2phin-0.0.22a4/src/air2phin/rules/hooks/PostgresHook.yaml
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:18:22.959140 air2phin-0.0.22a4/src/air2phin/rules/models/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1325 2023-03-14 11:00:33.000000 air2phin-0.0.22a4/src/air2phin/rules/models/Variable.yaml
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:18:22.960415 air2phin-0.0.22a4/src/air2phin/rules/operators/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1425 2023-03-15 02:15:19.000000 air2phin-0.0.22a4/src/air2phin/rules/operators/BashOperator.yaml
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1523 2023-07-17 08:27:58.000000 air2phin-0.0.22a4/src/air2phin/rules/operators/CheckOperator.yaml
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1771 2023-07-17 08:27:58.000000 air2phin-0.0.22a4/src/air2phin/rules/operators/CommonSensor.yaml
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1920 2023-07-17 08:27:58.000000 air2phin-0.0.22a4/src/air2phin/rules/operators/DataSyncOperator.yaml
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1149 2023-03-15 02:15:19.000000 air2phin-0.0.22a4/src/air2phin/rules/operators/DummyOperator.yaml
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1240 2023-07-17 08:27:58.000000 air2phin-0.0.22a4/src/air2phin/rules/operators/FbiRefreshOperator.yaml
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2105 2023-07-18 12:07:09.000000 air2phin-0.0.22a4/src/air2phin/rules/operators/PostgreOperator.yaml
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2057 2023-07-18 12:07:09.000000 air2phin-0.0.22a4/src/air2phin/rules/operators/PythonOperator.yaml
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1732 2023-07-18 12:07:09.000000 air2phin-0.0.22a4/src/air2phin/rules/operators/RedshiftOperator.yaml
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1604 2023-03-15 02:15:19.000000 air2phin-0.0.22a4/src/air2phin/rules/operators/SparkSqlOperator.yaml
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:18:22.960553 air2phin-0.0.22a4/src/air2phin/rules/utils/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)      616 2023-03-14 11:00:33.000000 air2phin-0.0.22a4/src/air2phin/rules/utils/TriggerRule.yaml
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     3519 2023-07-18 12:06:57.000000 air2phin-0.0.22a4/src/air2phin/runner.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:18:22.961071 air2phin-0.0.22a4/src/air2phin/utils/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-02-27 06:29:27.000000 air2phin-0.0.22a4/src/air2phin/utils/__init__.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2023 2023-07-18 12:06:57.000000 air2phin-0.0.22a4/src/air2phin/utils/file.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:18:22.961317 air2phin-0.0.22a4/src/air2phin/utils/marco/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-07-18 12:06:57.000000 air2phin-0.0.22a4/src/air2phin/utils/marco/__init__.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:18:22.961715 air2phin-0.0.22a4/src/air2phin/utils/marco/convertor/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-07-18 12:06:57.000000 air2phin-0.0.22a4/src/air2phin/utils/marco/convertor/__init__.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1713 2023-07-19 02:34:17.000000 air2phin-0.0.22a4/src/air2phin/utils/marco/convertor/base.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     3782 2023-07-18 12:06:57.000000 air2phin-0.0.22a4/src/air2phin/utils/marco/convertor/calculate.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     3663 2023-07-19 03:17:29.000000 air2phin-0.0.22a4/src/air2phin/utils/marco/helper.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1838 2023-07-18 12:06:57.000000 air2phin-0.0.22a4/src/air2phin/utils/reshape.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)      763 2023-07-18 12:06:57.000000 air2phin-0.0.22a4/src/air2phin/utils/string.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:18:22.955667 air2phin-0.0.22a4/src/air2phin.egg-info/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     6640 2023-07-19 03:18:22.000000 air2phin-0.0.22a4/src/air2phin.egg-info/PKG-INFO
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2228 2023-07-19 03:18:22.000000 air2phin-0.0.22a4/src/air2phin.egg-info/SOURCES.txt
--rw-r--r--   0 zhongjiajie   (501) staff       (20)        1 2023-07-19 03:18:22.000000 air2phin-0.0.22a4/src/air2phin.egg-info/dependency_links.txt
--rw-r--r--   0 zhongjiajie   (501) staff       (20)       55 2023-07-19 03:18:22.000000 air2phin-0.0.22a4/src/air2phin.egg-info/entry_points.txt
--rw-r--r--   0 zhongjiajie   (501) staff       (20)      287 2023-07-19 03:18:22.000000 air2phin-0.0.22a4/src/air2phin.egg-info/requires.txt
--rw-r--r--   0 zhongjiajie   (501) staff       (20)       14 2023-07-19 03:18:22.000000 air2phin-0.0.22a4/src/air2phin.egg-info/top_level.txt
--rw-r--r--   0 zhongjiajie   (501) staff       (20)        1 2023-02-24 09:08:53.000000 air2phin-0.0.22a4/src/air2phin.egg-info/zip-safe
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 06:44:57.255622 air2phin-0.0.22a5/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     6640 2023-07-19 06:44:57.255707 air2phin-0.0.22a5/PKG-INFO
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     5189 2023-03-14 11:00:33.000000 air2phin-0.0.22a5/README.md
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2002 2023-07-19 06:44:57.256113 air2phin-0.0.22a5/setup.cfg
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1930 2023-02-27 06:29:27.000000 air2phin-0.0.22a5/setup.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 06:44:57.241184 air2phin-0.0.22a5/src/
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 06:44:57.243901 air2phin-0.0.22a5/src/air2phin/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      841 2023-07-19 06:44:50.000000 air2phin-0.0.22a5/src/air2phin/__init__.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 06:44:57.245722 air2phin-0.0.22a5/src/air2phin/cli/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-02-27 06:29:27.000000 air2phin-0.0.22a5/src/air2phin/cli/__init__.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     6924 2023-07-18 12:06:57.000000 air2phin-0.0.22a5/src/air2phin/cli/command.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1390 2023-07-18 12:06:57.000000 air2phin-0.0.22a5/src/air2phin/constants.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 06:44:57.245900 air2phin-0.0.22a5/src/air2phin/core/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      785 2023-02-27 06:29:27.000000 air2phin-0.0.22a5/src/air2phin/core/__init__.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 06:44:57.246568 air2phin-0.0.22a5/src/air2phin/core/rules/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-02-27 06:29:27.000000 air2phin-0.0.22a5/src/air2phin/core/rules/__init__.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)    10568 2023-07-19 02:34:17.000000 air2phin-0.0.22a5/src/air2phin/core/rules/config.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      676 2023-07-18 12:06:57.000000 air2phin-0.0.22a5/src/air2phin/core/rules/loader.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 06:44:57.247207 air2phin-0.0.22a5/src/air2phin/core/transformer/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-02-27 06:29:27.000000 air2phin-0.0.22a5/src/air2phin/core/transformer/__init__.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     4135 2023-07-18 12:06:57.000000 air2phin-0.0.22a5/src/air2phin/core/transformer/imports.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     5602 2023-07-18 12:06:57.000000 air2phin-0.0.22a5/src/air2phin/core/transformer/operators.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     5286 2023-07-18 12:06:57.000000 air2phin-0.0.22a5/src/air2phin/core/transformer/route.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 06:44:57.247378 air2phin-0.0.22a5/src/air2phin/fake/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-02-27 06:29:27.000000 air2phin-0.0.22a5/src/air2phin/fake/__init__.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 06:44:57.247936 air2phin-0.0.22a5/src/air2phin/fake/core/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-02-27 06:29:27.000000 air2phin-0.0.22a5/src/air2phin/fake/core/__init__.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      211 2023-02-27 06:29:27.000000 air2phin-0.0.22a5/src/air2phin/fake/core/connection.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     9328 2023-07-19 02:34:17.000000 air2phin-0.0.22a5/src/air2phin/fake/core/hook.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 06:44:57.248714 air2phin-0.0.22a5/src/air2phin/fake/hooks/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-02-27 06:29:27.000000 air2phin-0.0.22a5/src/air2phin/fake/hooks/__init__.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1264 2023-07-18 12:06:57.000000 air2phin-0.0.22a5/src/air2phin/fake/hooks/mysql.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1294 2023-07-18 12:06:57.000000 air2phin-0.0.22a5/src/air2phin/fake/hooks/postgres.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 06:44:57.249146 air2phin-0.0.22a5/src/air2phin/fake/models/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      101 2023-03-14 11:00:33.000000 air2phin-0.0.22a5/src/air2phin/fake/models/__init__.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      983 2023-03-15 02:15:19.000000 air2phin-0.0.22a5/src/air2phin/fake/models/variable.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 06:44:57.249619 air2phin-0.0.22a5/src/air2phin/fake/utils/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-03-14 11:00:33.000000 air2phin-0.0.22a5/src/air2phin/fake/utils/__init__.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      875 2023-03-14 11:00:33.000000 air2phin-0.0.22a5/src/air2phin/fake/utils/trigger_rule.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 06:44:57.250039 air2phin-0.0.22a5/src/air2phin/patch/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-07-18 12:06:57.000000 air2phin-0.0.22a5/src/air2phin/patch/__init__.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1244 2023-07-19 03:12:27.000000 air2phin-0.0.22a5/src/air2phin/patch/marco_path.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 06:44:57.242528 air2phin-0.0.22a5/src/air2phin/rules/
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 06:44:57.250444 air2phin-0.0.22a5/src/air2phin/rules/core/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2170 2023-07-18 12:06:57.000000 air2phin-0.0.22a5/src/air2phin/rules/core/dagContext.yaml
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      558 2023-07-18 12:06:57.000000 air2phin-0.0.22a5/src/air2phin/rules/core/removeModule.yaml
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 06:44:57.250818 air2phin-0.0.22a5/src/air2phin/rules/hooks/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      658 2023-02-27 06:29:27.000000 air2phin-0.0.22a5/src/air2phin/rules/hooks/MySqlHook.yaml
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      713 2023-02-27 06:29:27.000000 air2phin-0.0.22a5/src/air2phin/rules/hooks/PostgresHook.yaml
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 06:44:57.251121 air2phin-0.0.22a5/src/air2phin/rules/models/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1325 2023-03-14 11:00:33.000000 air2phin-0.0.22a5/src/air2phin/rules/models/Variable.yaml
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 06:44:57.253515 air2phin-0.0.22a5/src/air2phin/rules/operators/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1425 2023-03-15 02:15:19.000000 air2phin-0.0.22a5/src/air2phin/rules/operators/BashOperator.yaml
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1523 2023-07-17 08:27:58.000000 air2phin-0.0.22a5/src/air2phin/rules/operators/CheckOperator.yaml
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1771 2023-07-17 08:27:58.000000 air2phin-0.0.22a5/src/air2phin/rules/operators/CommonSensor.yaml
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1920 2023-07-17 08:27:58.000000 air2phin-0.0.22a5/src/air2phin/rules/operators/DataSyncOperator.yaml
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1149 2023-03-15 02:15:19.000000 air2phin-0.0.22a5/src/air2phin/rules/operators/DummyOperator.yaml
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1240 2023-07-17 08:27:58.000000 air2phin-0.0.22a5/src/air2phin/rules/operators/FbiRefreshOperator.yaml
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2105 2023-07-18 12:07:09.000000 air2phin-0.0.22a5/src/air2phin/rules/operators/PostgreOperator.yaml
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2057 2023-07-18 12:07:09.000000 air2phin-0.0.22a5/src/air2phin/rules/operators/PythonOperator.yaml
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1732 2023-07-18 12:07:09.000000 air2phin-0.0.22a5/src/air2phin/rules/operators/RedshiftOperator.yaml
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1604 2023-03-15 02:15:19.000000 air2phin-0.0.22a5/src/air2phin/rules/operators/SparkSqlOperator.yaml
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 06:44:57.253718 air2phin-0.0.22a5/src/air2phin/rules/utils/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      616 2023-03-14 11:00:33.000000 air2phin-0.0.22a5/src/air2phin/rules/utils/TriggerRule.yaml
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     3519 2023-07-18 12:06:57.000000 air2phin-0.0.22a5/src/air2phin/runner.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 06:44:57.254346 air2phin-0.0.22a5/src/air2phin/utils/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-02-27 06:29:27.000000 air2phin-0.0.22a5/src/air2phin/utils/__init__.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2023 2023-07-18 12:06:57.000000 air2phin-0.0.22a5/src/air2phin/utils/file.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 06:44:57.254722 air2phin-0.0.22a5/src/air2phin/utils/marco/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-07-18 12:06:57.000000 air2phin-0.0.22a5/src/air2phin/utils/marco/__init__.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 06:44:57.255379 air2phin-0.0.22a5/src/air2phin/utils/marco/convertor/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-07-18 12:06:57.000000 air2phin-0.0.22a5/src/air2phin/utils/marco/convertor/__init__.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1716 2023-07-19 04:16:53.000000 air2phin-0.0.22a5/src/air2phin/utils/marco/convertor/base.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     3790 2023-07-19 06:41:14.000000 air2phin-0.0.22a5/src/air2phin/utils/marco/convertor/calculate.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     3705 2023-07-19 06:40:47.000000 air2phin-0.0.22a5/src/air2phin/utils/marco/helper.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1899 2023-07-19 06:43:51.000000 air2phin-0.0.22a5/src/air2phin/utils/reshape.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      763 2023-07-18 12:06:57.000000 air2phin-0.0.22a5/src/air2phin/utils/string.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 06:44:57.245314 air2phin-0.0.22a5/src/air2phin.egg-info/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     6640 2023-07-19 06:44:57.000000 air2phin-0.0.22a5/src/air2phin.egg-info/PKG-INFO
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2228 2023-07-19 06:44:57.000000 air2phin-0.0.22a5/src/air2phin.egg-info/SOURCES.txt
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)        1 2023-07-19 06:44:57.000000 air2phin-0.0.22a5/src/air2phin.egg-info/dependency_links.txt
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)       55 2023-07-19 06:44:57.000000 air2phin-0.0.22a5/src/air2phin.egg-info/entry_points.txt
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      287 2023-07-19 06:44:57.000000 air2phin-0.0.22a5/src/air2phin.egg-info/requires.txt
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)       14 2023-07-19 06:44:57.000000 air2phin-0.0.22a5/src/air2phin.egg-info/top_level.txt
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)        1 2023-02-24 09:08:53.000000 air2phin-0.0.22a5/src/air2phin.egg-info/zip-safe
```

### Comparing `air2phin-0.0.22a4/PKG-INFO` & `air2phin-0.0.22a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: air2phin
-Version: 0.0.22a4
+Version: 0.0.22a5
 Summary: Air2phin is a tool for migrating Airflow DAGs to DolphinScheduler Python API.
 Home-page: https://github.com/WhaleOps/air2phin
 Author: Jay Chung
 Author-email: zhongjiajie955@gmail.com
 License: Apache License 2.0
 Project-URL: Source, https://github.com/WhaleOps/air2phin
 Project-URL: Issue Tracker, https://github.com/WhaleOps/air2phin/issues
```

### Comparing `air2phin-0.0.22a4/README.md` & `air2phin-0.0.22a5/README.md`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a4/setup.cfg` & `air2phin-0.0.22a5/setup.cfg`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a4/setup.py` & `air2phin-0.0.22a5/setup.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a4/src/air2phin/__init__.py` & `air2phin-0.0.22a5/src/air2phin/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 __project_name__ = "Air2phin"
-__version__ = "0.0.22a4"
+__version__ = "0.0.22a5"
```

### Comparing `air2phin-0.0.22a4/src/air2phin/cli/command.py` & `air2phin-0.0.22a5/src/air2phin/cli/command.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a4/src/air2phin/constants.py` & `air2phin-0.0.22a5/src/air2phin/constants.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a4/src/air2phin/core/__init__.py` & `air2phin-0.0.22a5/src/air2phin/core/__init__.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a4/src/air2phin/core/rules/config.py` & `air2phin-0.0.22a5/src/air2phin/core/rules/config.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a4/src/air2phin/core/rules/loader.py` & `air2phin-0.0.22a5/src/air2phin/core/rules/loader.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a4/src/air2phin/core/transformer/imports.py` & `air2phin-0.0.22a5/src/air2phin/core/transformer/imports.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a4/src/air2phin/core/transformer/operators.py` & `air2phin-0.0.22a5/src/air2phin/core/transformer/operators.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a4/src/air2phin/core/transformer/route.py` & `air2phin-0.0.22a5/src/air2phin/core/transformer/route.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a4/src/air2phin/fake/core/hook.py` & `air2phin-0.0.22a5/src/air2phin/fake/core/hook.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a4/src/air2phin/fake/hooks/mysql.py` & `air2phin-0.0.22a5/src/air2phin/fake/hooks/mysql.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a4/src/air2phin/fake/hooks/postgres.py` & `air2phin-0.0.22a5/src/air2phin/fake/hooks/postgres.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a4/src/air2phin/fake/models/variable.py` & `air2phin-0.0.22a5/src/air2phin/fake/models/variable.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a4/src/air2phin/fake/utils/trigger_rule.py` & `air2phin-0.0.22a5/src/air2phin/fake/utils/trigger_rule.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a4/src/air2phin/patch/marco_path.py` & `air2phin-0.0.22a5/src/air2phin/patch/marco_path.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a4/src/air2phin/rules/core/dagContext.yaml` & `air2phin-0.0.22a5/src/air2phin/rules/core/dagContext.yaml`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a4/src/air2phin/rules/core/removeModule.yaml` & `air2phin-0.0.22a5/src/air2phin/rules/core/removeModule.yaml`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a4/src/air2phin/rules/hooks/MySqlHook.yaml` & `air2phin-0.0.22a5/src/air2phin/rules/hooks/MySqlHook.yaml`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a4/src/air2phin/rules/hooks/PostgresHook.yaml` & `air2phin-0.0.22a5/src/air2phin/rules/hooks/PostgresHook.yaml`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a4/src/air2phin/rules/models/Variable.yaml` & `air2phin-0.0.22a5/src/air2phin/rules/models/Variable.yaml`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a4/src/air2phin/rules/operators/BashOperator.yaml` & `air2phin-0.0.22a5/src/air2phin/rules/operators/BashOperator.yaml`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a4/src/air2phin/rules/operators/CheckOperator.yaml` & `air2phin-0.0.22a5/src/air2phin/rules/operators/CheckOperator.yaml`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a4/src/air2phin/rules/operators/CommonSensor.yaml` & `air2phin-0.0.22a5/src/air2phin/rules/operators/CommonSensor.yaml`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a4/src/air2phin/rules/operators/DataSyncOperator.yaml` & `air2phin-0.0.22a5/src/air2phin/rules/operators/DataSyncOperator.yaml`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a4/src/air2phin/rules/operators/DummyOperator.yaml` & `air2phin-0.0.22a5/src/air2phin/rules/operators/DummyOperator.yaml`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a4/src/air2phin/rules/operators/FbiRefreshOperator.yaml` & `air2phin-0.0.22a5/src/air2phin/rules/operators/FbiRefreshOperator.yaml`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a4/src/air2phin/rules/operators/PostgreOperator.yaml` & `air2phin-0.0.22a5/src/air2phin/rules/operators/PostgreOperator.yaml`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a4/src/air2phin/rules/operators/PythonOperator.yaml` & `air2phin-0.0.22a5/src/air2phin/rules/operators/PythonOperator.yaml`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a4/src/air2phin/rules/operators/RedshiftOperator.yaml` & `air2phin-0.0.22a5/src/air2phin/rules/operators/RedshiftOperator.yaml`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a4/src/air2phin/rules/operators/SparkSqlOperator.yaml` & `air2phin-0.0.22a5/src/air2phin/rules/operators/SparkSqlOperator.yaml`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a4/src/air2phin/rules/utils/TriggerRule.yaml` & `air2phin-0.0.22a5/src/air2phin/rules/utils/TriggerRule.yaml`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a4/src/air2phin/runner.py` & `air2phin-0.0.22a5/src/air2phin/runner.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a4/src/air2phin/utils/file.py` & `air2phin-0.0.22a5/src/air2phin/utils/file.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a4/src/air2phin/utils/marco/convertor/base.py` & `air2phin-0.0.22a5/src/air2phin/utils/marco/convertor/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
     def __init__(self, macro_func: str):
         self.macro_func = macro_func
 
     def parse_ds_base_date(self) -> None:
         self.ds_base_date = self.MACRO_FUNC_CONVERT.get(self.macro_func)
         if self.ds_base_date is None:
-            log.info(f"get unexpect macro func {self.macro_func}")
+            log.warning(f"get unexpect macro func {self.macro_func}")
 
     def parse_ds_offset(self) -> None:
         pass
 
     def get_human_read_name(self) -> str:
         return self.macro_func
```

### Comparing `air2phin-0.0.22a4/src/air2phin/utils/marco/convertor/calculate.py` & `air2phin-0.0.22a5/src/air2phin/utils/marco/convertor/calculate.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,17 +58,17 @@
         base_date_convert = {
             "execution_date": self.DEFAULT_OFFSET,
             "next_execution_date": self.schedule,
         }
 
         # hint
         if self.offset_unit is not None and self.offset_unit not in day2unit_convert:
-            log.error(f"get unexpect offset unit {self.offset_unit}")
+            log.warning(f"get unexpect offset unit {self.offset_unit}")
         if self.base_date not in base_date_convert:
-            log.error(f"get unexpect macro func {self.base_date}")
+            log.warning(f"get unexpect macro func {self.base_date}")
 
         # parse offset
         offset = base_date_convert.get(self.base_date, self.DEFAULT_OFFSET)
         if self.offset_unit is not None:
             offset += timedelta(**{self.offset_unit: self.offset_num})
 
         structure_timedelta = timedelta2structure(offset)
@@ -81,17 +81,17 @@
         base_date_convert = {
             "execution_date": self.DEFAULT_OFFSET,
             "next_execution_date": self.schedule,
         }
 
         # hint
         if self.offset_unit is not None and self.offset_unit not in day2unit_convert:
-            log.error(f"get unexpect offset unit {self.offset_unit}")
+            log.warning(f"get unexpect offset unit {self.offset_unit}")
         if self.base_date not in base_date_convert:
-            log.error(f"get unexpect macro func {self.base_date}")
+            log.warning(f"get unexpect macro func {self.base_date}")
 
         # parse offset
         offset = base_date_convert.get(self.base_date, self.DEFAULT_OFFSET)
         if self.offset_unit is not None:
             offset += timedelta(**{self.offset_unit: self.offset_num})
 
         structure_timedelta = timedelta2structure(offset)
```

### Comparing `air2phin-0.0.22a4/src/air2phin/utils/marco/helper.py` & `air2phin-0.0.22a5/src/air2phin/utils/marco/helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,27 +34,29 @@
 
     def parse2marco(self) -> BaseMacroConvertor | CalculateMacroConvertor | None:
         if "(" not in self.macro:
             return BaseMacroConvertor(macro_func=self.macro)
         if "," in self.macro:
             match = pattern_unit.match(self.macro)
             if match is None:
-                log.error(f"get unexpect macro func {self.macro} and can not parse it")
+                log.warning(
+                    f"get unexpect macro func {self.macro} and can not parse it"
+                )
                 return
             return CalculateMacroConvertor(
                 macro_func=match.group("macro_func"),
                 base_date=match.group("base_date"),
                 offset_unit=match.group("offset_unit"),
                 offset_num=int(match.group("offset_num")),
                 schedule=self.schedule,
             )
 
         match = pattern_no_unit.match(self.macro)
         if match is None:
-            log.error(f"get unexpect macro func {self.macro} and can not parse it")
+            log.warning(f"get unexpect macro func {self.macro} and can not parse it")
             return
         return CalculateMacroConvertor(
             macro_func=match.group("macro_func"),
             base_date=match.group("base_date"),
             offset_unit=None,
             offset_num=0,
             schedule=self.schedule,
```

### Comparing `air2phin-0.0.22a4/src/air2phin/utils/reshape.py` & `air2phin-0.0.22a5/src/air2phin/utils/reshape.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,16 @@
     else:
         return StructureTimedelta(
             unit="days", value=days, convert=day2unit_convert.get("days")
         )
 
 
 def schedule2timedelta(schedule: str | timedelta) -> timedelta:
+    if schedule is None:
+        return timedelta(seconds=0)
     if isinstance(schedule, timedelta):
         return schedule
     if schedule.startswith("@"):
         raise NotImplementedError("Airflow shortcut schedule not support, currently")
 
     now = datetime.now()
     cron = croniter.croniter(schedule, now)
```

### Comparing `air2phin-0.0.22a4/src/air2phin/utils/string.py` & `air2phin-0.0.22a5/src/air2phin/utils/string.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a4/src/air2phin.egg-info/PKG-INFO` & `air2phin-0.0.22a5/src/air2phin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: air2phin
-Version: 0.0.22a4
+Version: 0.0.22a5
 Summary: Air2phin is a tool for migrating Airflow DAGs to DolphinScheduler Python API.
 Home-page: https://github.com/WhaleOps/air2phin
 Author: Jay Chung
 Author-email: zhongjiajie955@gmail.com
 License: Apache License 2.0
 Project-URL: Source, https://github.com/WhaleOps/air2phin
 Project-URL: Issue Tracker, https://github.com/WhaleOps/air2phin/issues
```

### Comparing `air2phin-0.0.22a4/src/air2phin.egg-info/SOURCES.txt` & `air2phin-0.0.22a5/src/air2phin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

