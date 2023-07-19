# Comparing `tmp/air2phin-0.0.22a3.tar.gz` & `tmp/air2phin-0.0.22a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "air2phin-0.0.22a3.tar", last modified: Wed Jul 19 03:13:13 2023, max compression
+gzip compressed data, was "air2phin-0.0.22a4.tar", last modified: Wed Jul 19 03:18:22 2023, max compression
```

## Comparing `air2phin-0.0.22a3.tar` & `air2phin-0.0.22a4.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:13:13.022354 air2phin-0.0.22a3/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     6640 2023-07-19 03:13:13.022458 air2phin-0.0.22a3/PKG-INFO
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     5189 2023-03-14 11:00:33.000000 air2phin-0.0.22a3/README.md
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2002 2023-07-19 03:13:13.022877 air2phin-0.0.22a3/setup.cfg
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1930 2023-02-27 06:29:27.000000 air2phin-0.0.22a3/setup.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:13:13.013080 air2phin-0.0.22a3/src/
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:13:13.015112 air2phin-0.0.22a3/src/air2phin/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)      841 2023-07-19 03:13:07.000000 air2phin-0.0.22a3/src/air2phin/__init__.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:13:13.016593 air2phin-0.0.22a3/src/air2phin/cli/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-02-27 06:29:27.000000 air2phin-0.0.22a3/src/air2phin/cli/__init__.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     6924 2023-07-18 12:06:57.000000 air2phin-0.0.22a3/src/air2phin/cli/command.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1390 2023-07-18 12:06:57.000000 air2phin-0.0.22a3/src/air2phin/constants.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:13:13.016750 air2phin-0.0.22a3/src/air2phin/core/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)      785 2023-02-27 06:29:27.000000 air2phin-0.0.22a3/src/air2phin/core/__init__.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:13:13.017128 air2phin-0.0.22a3/src/air2phin/core/rules/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-02-27 06:29:27.000000 air2phin-0.0.22a3/src/air2phin/core/rules/__init__.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)    10568 2023-07-19 02:34:17.000000 air2phin-0.0.22a3/src/air2phin/core/rules/config.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)      676 2023-07-18 12:06:57.000000 air2phin-0.0.22a3/src/air2phin/core/rules/loader.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:13:13.017717 air2phin-0.0.22a3/src/air2phin/core/transformer/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-02-27 06:29:27.000000 air2phin-0.0.22a3/src/air2phin/core/transformer/__init__.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     4135 2023-07-18 12:06:57.000000 air2phin-0.0.22a3/src/air2phin/core/transformer/imports.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     5602 2023-07-18 12:06:57.000000 air2phin-0.0.22a3/src/air2phin/core/transformer/operators.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     5286 2023-07-18 12:06:57.000000 air2phin-0.0.22a3/src/air2phin/core/transformer/route.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:13:13.017851 air2phin-0.0.22a3/src/air2phin/fake/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-02-27 06:29:27.000000 air2phin-0.0.22a3/src/air2phin/fake/__init__.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:13:13.018193 air2phin-0.0.22a3/src/air2phin/fake/core/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-02-27 06:29:27.000000 air2phin-0.0.22a3/src/air2phin/fake/core/__init__.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)      211 2023-02-27 06:29:27.000000 air2phin-0.0.22a3/src/air2phin/fake/core/connection.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     9328 2023-07-19 02:34:17.000000 air2phin-0.0.22a3/src/air2phin/fake/core/hook.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:13:13.018544 air2phin-0.0.22a3/src/air2phin/fake/hooks/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-02-27 06:29:27.000000 air2phin-0.0.22a3/src/air2phin/fake/hooks/__init__.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1264 2023-07-18 12:06:57.000000 air2phin-0.0.22a3/src/air2phin/fake/hooks/mysql.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1294 2023-07-18 12:06:57.000000 air2phin-0.0.22a3/src/air2phin/fake/hooks/postgres.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:13:13.018782 air2phin-0.0.22a3/src/air2phin/fake/models/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)      101 2023-03-14 11:00:33.000000 air2phin-0.0.22a3/src/air2phin/fake/models/__init__.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)      983 2023-03-15 02:15:19.000000 air2phin-0.0.22a3/src/air2phin/fake/models/variable.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:13:13.018989 air2phin-0.0.22a3/src/air2phin/fake/utils/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-03-14 11:00:33.000000 air2phin-0.0.22a3/src/air2phin/fake/utils/__init__.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)      875 2023-03-14 11:00:33.000000 air2phin-0.0.22a3/src/air2phin/fake/utils/trigger_rule.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:13:13.019197 air2phin-0.0.22a3/src/air2phin/patch/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-07-18 12:06:57.000000 air2phin-0.0.22a3/src/air2phin/patch/__init__.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1244 2023-07-19 03:12:27.000000 air2phin-0.0.22a3/src/air2phin/patch/marco_path.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:13:13.014180 air2phin-0.0.22a3/src/air2phin/rules/
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:13:13.019433 air2phin-0.0.22a3/src/air2phin/rules/core/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2170 2023-07-18 12:06:57.000000 air2phin-0.0.22a3/src/air2phin/rules/core/dagContext.yaml
--rw-r--r--   0 zhongjiajie   (501) staff       (20)      558 2023-07-18 12:06:57.000000 air2phin-0.0.22a3/src/air2phin/rules/core/removeModule.yaml
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:13:13.019686 air2phin-0.0.22a3/src/air2phin/rules/hooks/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)      658 2023-02-27 06:29:27.000000 air2phin-0.0.22a3/src/air2phin/rules/hooks/MySqlHook.yaml
--rw-r--r--   0 zhongjiajie   (501) staff       (20)      713 2023-02-27 06:29:27.000000 air2phin-0.0.22a3/src/air2phin/rules/hooks/PostgresHook.yaml
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:13:13.019814 air2phin-0.0.22a3/src/air2phin/rules/models/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1325 2023-03-14 11:00:33.000000 air2phin-0.0.22a3/src/air2phin/rules/models/Variable.yaml
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:13:13.021063 air2phin-0.0.22a3/src/air2phin/rules/operators/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1425 2023-03-15 02:15:19.000000 air2phin-0.0.22a3/src/air2phin/rules/operators/BashOperator.yaml
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1523 2023-07-17 08:27:58.000000 air2phin-0.0.22a3/src/air2phin/rules/operators/CheckOperator.yaml
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1771 2023-07-17 08:27:58.000000 air2phin-0.0.22a3/src/air2phin/rules/operators/CommonSensor.yaml
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1920 2023-07-17 08:27:58.000000 air2phin-0.0.22a3/src/air2phin/rules/operators/DataSyncOperator.yaml
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1149 2023-03-15 02:15:19.000000 air2phin-0.0.22a3/src/air2phin/rules/operators/DummyOperator.yaml
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1240 2023-07-17 08:27:58.000000 air2phin-0.0.22a3/src/air2phin/rules/operators/FbiRefreshOperator.yaml
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2105 2023-07-18 12:07:09.000000 air2phin-0.0.22a3/src/air2phin/rules/operators/PostgreOperator.yaml
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2057 2023-07-18 12:07:09.000000 air2phin-0.0.22a3/src/air2phin/rules/operators/PythonOperator.yaml
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1732 2023-07-18 12:07:09.000000 air2phin-0.0.22a3/src/air2phin/rules/operators/RedshiftOperator.yaml
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1604 2023-03-15 02:15:19.000000 air2phin-0.0.22a3/src/air2phin/rules/operators/SparkSqlOperator.yaml
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:13:13.021190 air2phin-0.0.22a3/src/air2phin/rules/utils/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)      616 2023-03-14 11:00:33.000000 air2phin-0.0.22a3/src/air2phin/rules/utils/TriggerRule.yaml
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     3519 2023-07-18 12:06:57.000000 air2phin-0.0.22a3/src/air2phin/runner.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:13:13.021649 air2phin-0.0.22a3/src/air2phin/utils/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-02-27 06:29:27.000000 air2phin-0.0.22a3/src/air2phin/utils/__init__.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2023 2023-07-18 12:06:57.000000 air2phin-0.0.22a3/src/air2phin/utils/file.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:13:13.021865 air2phin-0.0.22a3/src/air2phin/utils/marco/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-07-18 12:06:57.000000 air2phin-0.0.22a3/src/air2phin/utils/marco/__init__.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:13:13.022232 air2phin-0.0.22a3/src/air2phin/utils/marco/convertor/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-07-18 12:06:57.000000 air2phin-0.0.22a3/src/air2phin/utils/marco/convertor/__init__.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1713 2023-07-19 02:34:17.000000 air2phin-0.0.22a3/src/air2phin/utils/marco/convertor/base.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     3782 2023-07-18 12:06:57.000000 air2phin-0.0.22a3/src/air2phin/utils/marco/convertor/calculate.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     3636 2023-07-18 12:06:57.000000 air2phin-0.0.22a3/src/air2phin/utils/marco/helper.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     1838 2023-07-18 12:06:57.000000 air2phin-0.0.22a3/src/air2phin/utils/reshape.py
--rw-r--r--   0 zhongjiajie   (501) staff       (20)      763 2023-07-18 12:06:57.000000 air2phin-0.0.22a3/src/air2phin/utils/string.py
-drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:13:13.015946 air2phin-0.0.22a3/src/air2phin.egg-info/
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     6640 2023-07-19 03:13:13.000000 air2phin-0.0.22a3/src/air2phin.egg-info/PKG-INFO
--rw-r--r--   0 zhongjiajie   (501) staff       (20)     2228 2023-07-19 03:13:13.000000 air2phin-0.0.22a3/src/air2phin.egg-info/SOURCES.txt
--rw-r--r--   0 zhongjiajie   (501) staff       (20)        1 2023-07-19 03:13:13.000000 air2phin-0.0.22a3/src/air2phin.egg-info/dependency_links.txt
--rw-r--r--   0 zhongjiajie   (501) staff       (20)       55 2023-07-19 03:13:13.000000 air2phin-0.0.22a3/src/air2phin.egg-info/entry_points.txt
--rw-r--r--   0 zhongjiajie   (501) staff       (20)      287 2023-07-19 03:13:13.000000 air2phin-0.0.22a3/src/air2phin.egg-info/requires.txt
--rw-r--r--   0 zhongjiajie   (501) staff       (20)       14 2023-07-19 03:13:13.000000 air2phin-0.0.22a3/src/air2phin.egg-info/top_level.txt
--rw-r--r--   0 zhongjiajie   (501) staff       (20)        1 2023-02-24 09:08:53.000000 air2phin-0.0.22a3/src/air2phin.egg-info/zip-safe
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:18:22.961834 air2phin-0.0.22a4/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     6640 2023-07-19 03:18:22.961918 air2phin-0.0.22a4/PKG-INFO
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     5189 2023-03-14 11:00:33.000000 air2phin-0.0.22a4/README.md
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2002 2023-07-19 03:18:22.962305 air2phin-0.0.22a4/setup.cfg
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1930 2023-02-27 06:29:27.000000 air2phin-0.0.22a4/setup.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:18:22.952655 air2phin-0.0.22a4/src/
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:18:22.954783 air2phin-0.0.22a4/src/air2phin/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      841 2023-07-19 03:18:17.000000 air2phin-0.0.22a4/src/air2phin/__init__.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:18:22.955887 air2phin-0.0.22a4/src/air2phin/cli/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-02-27 06:29:27.000000 air2phin-0.0.22a4/src/air2phin/cli/__init__.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     6924 2023-07-18 12:06:57.000000 air2phin-0.0.22a4/src/air2phin/cli/command.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1390 2023-07-18 12:06:57.000000 air2phin-0.0.22a4/src/air2phin/constants.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:18:22.956008 air2phin-0.0.22a4/src/air2phin/core/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      785 2023-02-27 06:29:27.000000 air2phin-0.0.22a4/src/air2phin/core/__init__.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:18:22.956349 air2phin-0.0.22a4/src/air2phin/core/rules/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-02-27 06:29:27.000000 air2phin-0.0.22a4/src/air2phin/core/rules/__init__.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)    10568 2023-07-19 02:34:17.000000 air2phin-0.0.22a4/src/air2phin/core/rules/config.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      676 2023-07-18 12:06:57.000000 air2phin-0.0.22a4/src/air2phin/core/rules/loader.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:18:22.956821 air2phin-0.0.22a4/src/air2phin/core/transformer/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-02-27 06:29:27.000000 air2phin-0.0.22a4/src/air2phin/core/transformer/__init__.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     4135 2023-07-18 12:06:57.000000 air2phin-0.0.22a4/src/air2phin/core/transformer/imports.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     5602 2023-07-18 12:06:57.000000 air2phin-0.0.22a4/src/air2phin/core/transformer/operators.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     5286 2023-07-18 12:06:57.000000 air2phin-0.0.22a4/src/air2phin/core/transformer/route.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:18:22.956948 air2phin-0.0.22a4/src/air2phin/fake/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-02-27 06:29:27.000000 air2phin-0.0.22a4/src/air2phin/fake/__init__.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:18:22.957279 air2phin-0.0.22a4/src/air2phin/fake/core/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-02-27 06:29:27.000000 air2phin-0.0.22a4/src/air2phin/fake/core/__init__.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      211 2023-02-27 06:29:27.000000 air2phin-0.0.22a4/src/air2phin/fake/core/connection.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     9328 2023-07-19 02:34:17.000000 air2phin-0.0.22a4/src/air2phin/fake/core/hook.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:18:22.957641 air2phin-0.0.22a4/src/air2phin/fake/hooks/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-02-27 06:29:27.000000 air2phin-0.0.22a4/src/air2phin/fake/hooks/__init__.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1264 2023-07-18 12:06:57.000000 air2phin-0.0.22a4/src/air2phin/fake/hooks/mysql.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1294 2023-07-18 12:06:57.000000 air2phin-0.0.22a4/src/air2phin/fake/hooks/postgres.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:18:22.957869 air2phin-0.0.22a4/src/air2phin/fake/models/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      101 2023-03-14 11:00:33.000000 air2phin-0.0.22a4/src/air2phin/fake/models/__init__.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      983 2023-03-15 02:15:19.000000 air2phin-0.0.22a4/src/air2phin/fake/models/variable.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:18:22.958289 air2phin-0.0.22a4/src/air2phin/fake/utils/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-03-14 11:00:33.000000 air2phin-0.0.22a4/src/air2phin/fake/utils/__init__.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      875 2023-03-14 11:00:33.000000 air2phin-0.0.22a4/src/air2phin/fake/utils/trigger_rule.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:18:22.958525 air2phin-0.0.22a4/src/air2phin/patch/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-07-18 12:06:57.000000 air2phin-0.0.22a4/src/air2phin/patch/__init__.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1244 2023-07-19 03:12:27.000000 air2phin-0.0.22a4/src/air2phin/patch/marco_path.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:18:22.953848 air2phin-0.0.22a4/src/air2phin/rules/
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:18:22.958770 air2phin-0.0.22a4/src/air2phin/rules/core/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2170 2023-07-18 12:06:57.000000 air2phin-0.0.22a4/src/air2phin/rules/core/dagContext.yaml
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      558 2023-07-18 12:06:57.000000 air2phin-0.0.22a4/src/air2phin/rules/core/removeModule.yaml
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:18:22.959019 air2phin-0.0.22a4/src/air2phin/rules/hooks/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      658 2023-02-27 06:29:27.000000 air2phin-0.0.22a4/src/air2phin/rules/hooks/MySqlHook.yaml
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      713 2023-02-27 06:29:27.000000 air2phin-0.0.22a4/src/air2phin/rules/hooks/PostgresHook.yaml
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:18:22.959140 air2phin-0.0.22a4/src/air2phin/rules/models/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1325 2023-03-14 11:00:33.000000 air2phin-0.0.22a4/src/air2phin/rules/models/Variable.yaml
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:18:22.960415 air2phin-0.0.22a4/src/air2phin/rules/operators/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1425 2023-03-15 02:15:19.000000 air2phin-0.0.22a4/src/air2phin/rules/operators/BashOperator.yaml
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1523 2023-07-17 08:27:58.000000 air2phin-0.0.22a4/src/air2phin/rules/operators/CheckOperator.yaml
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1771 2023-07-17 08:27:58.000000 air2phin-0.0.22a4/src/air2phin/rules/operators/CommonSensor.yaml
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1920 2023-07-17 08:27:58.000000 air2phin-0.0.22a4/src/air2phin/rules/operators/DataSyncOperator.yaml
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1149 2023-03-15 02:15:19.000000 air2phin-0.0.22a4/src/air2phin/rules/operators/DummyOperator.yaml
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1240 2023-07-17 08:27:58.000000 air2phin-0.0.22a4/src/air2phin/rules/operators/FbiRefreshOperator.yaml
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2105 2023-07-18 12:07:09.000000 air2phin-0.0.22a4/src/air2phin/rules/operators/PostgreOperator.yaml
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2057 2023-07-18 12:07:09.000000 air2phin-0.0.22a4/src/air2phin/rules/operators/PythonOperator.yaml
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1732 2023-07-18 12:07:09.000000 air2phin-0.0.22a4/src/air2phin/rules/operators/RedshiftOperator.yaml
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1604 2023-03-15 02:15:19.000000 air2phin-0.0.22a4/src/air2phin/rules/operators/SparkSqlOperator.yaml
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:18:22.960553 air2phin-0.0.22a4/src/air2phin/rules/utils/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      616 2023-03-14 11:00:33.000000 air2phin-0.0.22a4/src/air2phin/rules/utils/TriggerRule.yaml
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     3519 2023-07-18 12:06:57.000000 air2phin-0.0.22a4/src/air2phin/runner.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:18:22.961071 air2phin-0.0.22a4/src/air2phin/utils/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-02-27 06:29:27.000000 air2phin-0.0.22a4/src/air2phin/utils/__init__.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2023 2023-07-18 12:06:57.000000 air2phin-0.0.22a4/src/air2phin/utils/file.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:18:22.961317 air2phin-0.0.22a4/src/air2phin/utils/marco/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-07-18 12:06:57.000000 air2phin-0.0.22a4/src/air2phin/utils/marco/__init__.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:18:22.961715 air2phin-0.0.22a4/src/air2phin/utils/marco/convertor/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)        0 2023-07-18 12:06:57.000000 air2phin-0.0.22a4/src/air2phin/utils/marco/convertor/__init__.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1713 2023-07-19 02:34:17.000000 air2phin-0.0.22a4/src/air2phin/utils/marco/convertor/base.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     3782 2023-07-18 12:06:57.000000 air2phin-0.0.22a4/src/air2phin/utils/marco/convertor/calculate.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     3663 2023-07-19 03:17:29.000000 air2phin-0.0.22a4/src/air2phin/utils/marco/helper.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     1838 2023-07-18 12:06:57.000000 air2phin-0.0.22a4/src/air2phin/utils/reshape.py
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      763 2023-07-18 12:06:57.000000 air2phin-0.0.22a4/src/air2phin/utils/string.py
+drwxr-xr-x   0 zhongjiajie   (501) staff       (20)        0 2023-07-19 03:18:22.955667 air2phin-0.0.22a4/src/air2phin.egg-info/
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     6640 2023-07-19 03:18:22.000000 air2phin-0.0.22a4/src/air2phin.egg-info/PKG-INFO
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)     2228 2023-07-19 03:18:22.000000 air2phin-0.0.22a4/src/air2phin.egg-info/SOURCES.txt
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)        1 2023-07-19 03:18:22.000000 air2phin-0.0.22a4/src/air2phin.egg-info/dependency_links.txt
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)       55 2023-07-19 03:18:22.000000 air2phin-0.0.22a4/src/air2phin.egg-info/entry_points.txt
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)      287 2023-07-19 03:18:22.000000 air2phin-0.0.22a4/src/air2phin.egg-info/requires.txt
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)       14 2023-07-19 03:18:22.000000 air2phin-0.0.22a4/src/air2phin.egg-info/top_level.txt
+-rw-r--r--   0 zhongjiajie   (501) staff       (20)        1 2023-02-24 09:08:53.000000 air2phin-0.0.22a4/src/air2phin.egg-info/zip-safe
```

### Comparing `air2phin-0.0.22a3/PKG-INFO` & `air2phin-0.0.22a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: air2phin
-Version: 0.0.22a3
+Version: 0.0.22a4
 Summary: Air2phin is a tool for migrating Airflow DAGs to DolphinScheduler Python API.
 Home-page: https://github.com/WhaleOps/air2phin
 Author: Jay Chung
 Author-email: zhongjiajie955@gmail.com
 License: Apache License 2.0
 Project-URL: Source, https://github.com/WhaleOps/air2phin
 Project-URL: Issue Tracker, https://github.com/WhaleOps/air2phin/issues
```

### Comparing `air2phin-0.0.22a3/README.md` & `air2phin-0.0.22a4/README.md`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a3/setup.cfg` & `air2phin-0.0.22a4/setup.cfg`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a3/setup.py` & `air2phin-0.0.22a4/setup.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a3/src/air2phin/__init__.py` & `air2phin-0.0.22a4/src/air2phin/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 __project_name__ = "Air2phin"
-__version__ = "0.0.22a3"
+__version__ = "0.0.22a4"
```

### Comparing `air2phin-0.0.22a3/src/air2phin/cli/command.py` & `air2phin-0.0.22a4/src/air2phin/cli/command.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a3/src/air2phin/constants.py` & `air2phin-0.0.22a4/src/air2phin/constants.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a3/src/air2phin/core/__init__.py` & `air2phin-0.0.22a4/src/air2phin/core/__init__.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a3/src/air2phin/core/rules/config.py` & `air2phin-0.0.22a4/src/air2phin/core/rules/config.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a3/src/air2phin/core/rules/loader.py` & `air2phin-0.0.22a4/src/air2phin/core/rules/loader.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a3/src/air2phin/core/transformer/imports.py` & `air2phin-0.0.22a4/src/air2phin/core/transformer/imports.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a3/src/air2phin/core/transformer/operators.py` & `air2phin-0.0.22a4/src/air2phin/core/transformer/operators.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a3/src/air2phin/core/transformer/route.py` & `air2phin-0.0.22a4/src/air2phin/core/transformer/route.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a3/src/air2phin/fake/core/hook.py` & `air2phin-0.0.22a4/src/air2phin/fake/core/hook.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a3/src/air2phin/fake/hooks/mysql.py` & `air2phin-0.0.22a4/src/air2phin/fake/hooks/mysql.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a3/src/air2phin/fake/hooks/postgres.py` & `air2phin-0.0.22a4/src/air2phin/fake/hooks/postgres.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a3/src/air2phin/fake/models/variable.py` & `air2phin-0.0.22a4/src/air2phin/fake/models/variable.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a3/src/air2phin/fake/utils/trigger_rule.py` & `air2phin-0.0.22a4/src/air2phin/fake/utils/trigger_rule.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a3/src/air2phin/patch/marco_path.py` & `air2phin-0.0.22a4/src/air2phin/patch/marco_path.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a3/src/air2phin/rules/core/dagContext.yaml` & `air2phin-0.0.22a4/src/air2phin/rules/core/dagContext.yaml`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a3/src/air2phin/rules/core/removeModule.yaml` & `air2phin-0.0.22a4/src/air2phin/rules/core/removeModule.yaml`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a3/src/air2phin/rules/hooks/MySqlHook.yaml` & `air2phin-0.0.22a4/src/air2phin/rules/hooks/MySqlHook.yaml`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a3/src/air2phin/rules/hooks/PostgresHook.yaml` & `air2phin-0.0.22a4/src/air2phin/rules/hooks/PostgresHook.yaml`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a3/src/air2phin/rules/models/Variable.yaml` & `air2phin-0.0.22a4/src/air2phin/rules/models/Variable.yaml`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a3/src/air2phin/rules/operators/BashOperator.yaml` & `air2phin-0.0.22a4/src/air2phin/rules/operators/BashOperator.yaml`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a3/src/air2phin/rules/operators/CheckOperator.yaml` & `air2phin-0.0.22a4/src/air2phin/rules/operators/CheckOperator.yaml`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a3/src/air2phin/rules/operators/CommonSensor.yaml` & `air2phin-0.0.22a4/src/air2phin/rules/operators/CommonSensor.yaml`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a3/src/air2phin/rules/operators/DataSyncOperator.yaml` & `air2phin-0.0.22a4/src/air2phin/rules/operators/DataSyncOperator.yaml`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a3/src/air2phin/rules/operators/DummyOperator.yaml` & `air2phin-0.0.22a4/src/air2phin/rules/operators/DummyOperator.yaml`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a3/src/air2phin/rules/operators/FbiRefreshOperator.yaml` & `air2phin-0.0.22a4/src/air2phin/rules/operators/FbiRefreshOperator.yaml`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a3/src/air2phin/rules/operators/PostgreOperator.yaml` & `air2phin-0.0.22a4/src/air2phin/rules/operators/PostgreOperator.yaml`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a3/src/air2phin/rules/operators/PythonOperator.yaml` & `air2phin-0.0.22a4/src/air2phin/rules/operators/PythonOperator.yaml`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a3/src/air2phin/rules/operators/RedshiftOperator.yaml` & `air2phin-0.0.22a4/src/air2phin/rules/operators/RedshiftOperator.yaml`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a3/src/air2phin/rules/operators/SparkSqlOperator.yaml` & `air2phin-0.0.22a4/src/air2phin/rules/operators/SparkSqlOperator.yaml`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a3/src/air2phin/rules/utils/TriggerRule.yaml` & `air2phin-0.0.22a4/src/air2phin/rules/utils/TriggerRule.yaml`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a3/src/air2phin/runner.py` & `air2phin-0.0.22a4/src/air2phin/runner.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a3/src/air2phin/utils/file.py` & `air2phin-0.0.22a4/src/air2phin/utils/file.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a3/src/air2phin/utils/marco/convertor/base.py` & `air2phin-0.0.22a4/src/air2phin/utils/marco/convertor/base.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a3/src/air2phin/utils/marco/convertor/calculate.py` & `air2phin-0.0.22a4/src/air2phin/utils/marco/convertor/calculate.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a3/src/air2phin/utils/marco/helper.py` & `air2phin-0.0.22a4/src/air2phin/utils/marco/helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,16 +99,16 @@
         return TaskContentWithMarco(content=content)
 
     marcos = set()
     for find in find_lst:
         if find is None:
             continue
         trim_key = find.strip()
-        ds_marco: DolphinHumanReadMarco = parse2ds_marco(trim_key, schedule)
-        if ds_marco.name is None:
+        ds_marco: DolphinHumanReadMarco | None = parse2ds_marco(trim_key, schedule)
+        if ds_marco is None or ds_marco.name is None:
             continue
         pattern = "\\{\\{ *" + escape_marco_bracket(trim_key) + " *\\}\\}"
         new_ds_marco = "${" + ds_marco.name + "}"
         content = re.compile(pattern).sub(new_ds_marco, content)
         marcos.add(ds_marco)
     return TaskContentWithMarco(
         content=content,
```

### Comparing `air2phin-0.0.22a3/src/air2phin/utils/reshape.py` & `air2phin-0.0.22a4/src/air2phin/utils/reshape.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a3/src/air2phin/utils/string.py` & `air2phin-0.0.22a4/src/air2phin/utils/string.py`

 * *Files identical despite different names*

### Comparing `air2phin-0.0.22a3/src/air2phin.egg-info/PKG-INFO` & `air2phin-0.0.22a4/src/air2phin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: air2phin
-Version: 0.0.22a3
+Version: 0.0.22a4
 Summary: Air2phin is a tool for migrating Airflow DAGs to DolphinScheduler Python API.
 Home-page: https://github.com/WhaleOps/air2phin
 Author: Jay Chung
 Author-email: zhongjiajie955@gmail.com
 License: Apache License 2.0
 Project-URL: Source, https://github.com/WhaleOps/air2phin
 Project-URL: Issue Tracker, https://github.com/WhaleOps/air2phin/issues
```

### Comparing `air2phin-0.0.22a3/src/air2phin.egg-info/SOURCES.txt` & `air2phin-0.0.22a4/src/air2phin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

