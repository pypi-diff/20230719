# Comparing `tmp/TapisCL-ICICLE-1.0.0.tar.gz` & `tmp/TapisCL-ICICLE-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TapisCL-ICICLE-1.0.0.tar", last modified: Tue Jul 18 18:12:53 2023, max compression
+gzip compressed data, was "TapisCL-ICICLE-1.0.1.tar", last modified: Tue Jul 18 21:01:28 2023, max compression
```

## Comparing `TapisCL-ICICLE-1.0.0.tar` & `TapisCL-ICICLE-1.0.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 18:12:53.760612 TapisCL-ICICLE-1.0.0/
--rw-rw-rw-   0        0        0    35823 2023-04-12 23:35:22.000000 TapisCL-ICICLE-1.0.0/LICENSE
--rw-rw-rw-   0        0        0    50383 2023-07-18 18:12:53.760612 TapisCL-ICICLE-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     8502 2023-07-12 23:36:44.000000 TapisCL-ICICLE-1.0.0/README.md
--rw-rw-rw-   0        0        0     1227 2023-07-18 18:09:08.000000 TapisCL-ICICLE-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-18 18:12:53.760612 TapisCL-ICICLE-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-18 18:12:53.727013 TapisCL-ICICLE-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-18 18:12:53.729007 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/
--rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/__init__.py
--rw-rw-rw-   0        0        0      321 2023-06-29 16:14:59.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 18:12:53.731078 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/client/
--rw-rw-rw-   0        0        0       84 2023-05-23 19:58:53.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/client/__init__.py
--rw-rw-rw-   0        0        0    10788 2023-07-18 17:46:54.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/client/cli.py
--rw-rw-rw-   0        0        0    16008 2023-07-17 19:00:49.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/client/handlers.py
-drwxrwxrwx   0        0        0        0 2023-07-18 18:12:53.737564 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/
-drwxrwxrwx   0        0        0        0 2023-07-18 18:12:53.740555 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/Apps/
--rw-rw-rw-   0        0        0        0 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/Apps/__init__.py
--rw-rw-rw-   0        0        0    11096 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/Apps/appCommands.py
--rw-rw-rw-   0        0        0      259 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/Apps/appConfigGenerator.py
--rw-rw-rw-   0        0        0     4859 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/Apps/appForms.py
-drwxrwxrwx   0        0        0        0 2023-07-18 18:12:53.742548 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/Systems/
--rw-rw-rw-   0        0        0        0 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/Systems/__init__.py
--rw-rw-rw-   0        0        0    23546 2023-07-17 15:51:32.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/Systems/systemCommands.py
--rw-rw-rw-   0        0        0     3940 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/Systems/systemForms.py
--rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 18:12:53.745058 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/arguments/
--rw-rw-rw-   0        0        0        0 2023-06-16 01:12:43.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/arguments/__init__.py
--rw-rw-rw-   0        0        0     9283 2023-07-18 16:53:44.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/arguments/argument.py
--rw-rw-rw-   0        0        0     4772 2023-07-18 16:34:22.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/arguments/argumentValidators.py
--rw-rw-rw-   0        0        0    20827 2023-07-18 17:33:56.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/baseCommand.py
--rw-rw-rw-   0        0        0    10791 2023-07-18 16:22:47.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/commandMap.py
--rw-rw-rw-   0        0        0     2221 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/commandOpts.py
--rw-rw-rw-   0        0        0     1828 2023-07-18 17:57:50.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/dataFormatters.py
--rw-rw-rw-   0        0        0     4947 2023-07-10 21:26:23.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/decorators.py
--rw-rw-rw-   0        0        0    11399 2023-07-17 16:26:08.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/fileCommands.py
--rw-rw-rw-   0        0        0     7191 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/jobCommands.py
--rw-rw-rw-   0        0        0    13236 2023-07-18 18:01:26.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/podCommands.py
-drwxrwxrwx   0        0        0        0 2023-07-18 18:12:53.747413 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/query/
--rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/query/__init__.py
--rw-rw-rw-   0        0        0     1615 2023-07-11 17:42:26.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/query/neo4j.py
--rw-rw-rw-   0        0        0      871 2023-06-16 01:12:43.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/query/postgres.py
--rw-rw-rw-   0        0        0     4412 2023-07-17 15:54:36.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/serverCommands.py
--rw-rw-rw-   0        0        0     7990 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/volumeCommands.py
-drwxrwxrwx   0        0        0        0 2023-07-18 18:12:53.749406 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/server/
--rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/server/__init__.py
--rw-rw-rw-   0        0        0    10928 2023-07-06 00:52:04.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/server/auth.py
--rw-rw-rw-   0        0        0    10402 2023-07-17 16:55:28.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/server/server.py
--rw-rw-rw-   0        0        0      290 2023-07-05 15:04:52.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/serverRun.py
-drwxrwxrwx   0        0        0        0 2023-07-18 18:12:53.751400 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/socketopts/
--rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/socketopts/__init__.py
--rw-rw-rw-   0        0        0     2233 2023-07-10 21:26:16.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/socketopts/schemas.py
--rw-rw-rw-   0        0        0     4810 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/socketopts/socketOpts.py
-drwxrwxrwx   0        0        0        0 2023-07-18 18:12:53.754909 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/utilities/
--rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/utilities/__init__.py
--rw-rw-rw-   0        0        0     2457 2023-06-16 02:31:56.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/utilities/exceptions.py
--rw-rw-rw-   0        0        0     1044 2023-06-29 21:33:53.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/utilities/killableThread.py
--rw-rw-rw-   0        0        0     2328 2023-07-08 04:38:18.000000 TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/utilities/logger.py
-drwxrwxrwx   0        0        0        0 2023-07-18 18:12:53.759110 TapisCL-ICICLE-1.0.0/src/TapisCL_ICICLE.egg-info/
--rw-rw-rw-   0        0        0    50383 2023-07-18 18:12:53.000000 TapisCL-ICICLE-1.0.0/src/TapisCL_ICICLE.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2003 2023-07-18 18:12:53.000000 TapisCL-ICICLE-1.0.0/src/TapisCL_ICICLE.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 18:12:53.000000 TapisCL-ICICLE-1.0.0/src/TapisCL_ICICLE.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-07-18 18:12:53.000000 TapisCL-ICICLE-1.0.0/src/TapisCL_ICICLE.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-07-18 18:12:53.000000 TapisCL-ICICLE-1.0.0/src/TapisCL_ICICLE.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-07-18 18:12:53.000000 TapisCL-ICICLE-1.0.0/src/TapisCL_ICICLE.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-06-29 16:14:59.000000 TapisCL-ICICLE-1.0.0/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 18:12:53.759110 TapisCL-ICICLE-1.0.0/tests/
--rw-rw-rw-   0        0        0       81 2023-07-17 16:51:58.000000 TapisCL-ICICLE-1.0.0/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-07-18 21:01:28.135121 TapisCL-ICICLE-1.0.1/
+-rw-rw-rw-   0        0        0    35823 2023-04-12 23:35:22.000000 TapisCL-ICICLE-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0    58862 2023-07-18 21:01:28.135121 TapisCL-ICICLE-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0    16981 2023-07-18 20:02:58.000000 TapisCL-ICICLE-1.0.1/README.md
+-rw-rw-rw-   0        0        0     1227 2023-07-18 21:00:49.000000 TapisCL-ICICLE-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-18 21:01:28.135121 TapisCL-ICICLE-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-18 21:01:28.100664 TapisCL-ICICLE-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-18 21:01:28.102656 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/
+-rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/__init__.py
+-rw-rw-rw-   0        0        0      321 2023-06-29 16:14:59.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 21:01:28.104649 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/client/
+-rw-rw-rw-   0        0        0       84 2023-05-23 19:58:53.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/client/__init__.py
+-rw-rw-rw-   0        0        0    10738 2023-07-18 20:56:23.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/client/cli.py
+-rw-rw-rw-   0        0        0    16008 2023-07-17 19:00:49.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/client/handlers.py
+drwxrwxrwx   0        0        0        0 2023-07-18 21:01:28.111155 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/
+drwxrwxrwx   0        0        0        0 2023-07-18 21:01:28.115142 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/Apps/
+-rw-rw-rw-   0        0        0        0 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/Apps/__init__.py
+-rw-rw-rw-   0        0        0    11096 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/Apps/appCommands.py
+-rw-rw-rw-   0        0        0      259 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/Apps/appConfigGenerator.py
+-rw-rw-rw-   0        0        0     4859 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/Apps/appForms.py
+drwxrwxrwx   0        0        0        0 2023-07-18 21:01:28.116643 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/Systems/
+-rw-rw-rw-   0        0        0        0 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/Systems/__init__.py
+-rw-rw-rw-   0        0        0    23546 2023-07-17 15:51:32.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/Systems/systemCommands.py
+-rw-rw-rw-   0        0        0     3940 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/Systems/systemForms.py
+-rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 21:01:28.119154 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/arguments/
+-rw-rw-rw-   0        0        0        0 2023-06-16 01:12:43.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/arguments/__init__.py
+-rw-rw-rw-   0        0        0     9298 2023-07-18 20:47:15.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/arguments/argument.py
+-rw-rw-rw-   0        0        0     4772 2023-07-18 16:34:22.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/arguments/argumentValidators.py
+-rw-rw-rw-   0        0        0    20942 2023-07-18 20:46:18.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/baseCommand.py
+-rw-rw-rw-   0        0        0    10976 2023-07-18 20:01:13.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/commandMap.py
+-rw-rw-rw-   0        0        0     2221 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/commandOpts.py
+-rw-rw-rw-   0        0        0     1867 2023-07-18 20:33:33.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/dataFormatters.py
+-rw-rw-rw-   0        0        0     4947 2023-07-10 21:26:23.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/decorators.py
+-rw-rw-rw-   0        0        0    12824 2023-07-18 20:04:51.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/fileCommands.py
+-rw-rw-rw-   0        0        0     7522 2023-07-18 20:00:48.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/jobCommands.py
+-rw-rw-rw-   0        0        0    13236 2023-07-18 18:01:26.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/podCommands.py
+drwxrwxrwx   0        0        0        0 2023-07-18 21:01:28.121150 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/query/
+-rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/query/__init__.py
+-rw-rw-rw-   0        0        0     1615 2023-07-11 17:42:26.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/query/neo4j.py
+-rw-rw-rw-   0        0        0      871 2023-06-16 01:12:43.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/query/postgres.py
+-rw-rw-rw-   0        0        0     4412 2023-07-17 15:54:36.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/serverCommands.py
+-rw-rw-rw-   0        0        0     7990 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/volumeCommands.py
+drwxrwxrwx   0        0        0        0 2023-07-18 21:01:28.123144 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/server/
+-rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/server/__init__.py
+-rw-rw-rw-   0        0        0    10928 2023-07-06 00:52:04.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/server/auth.py
+-rw-rw-rw-   0        0        0    10402 2023-07-17 16:55:28.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/server/server.py
+-rw-rw-rw-   0        0        0      290 2023-07-05 15:04:52.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/serverRun.py
+drwxrwxrwx   0        0        0        0 2023-07-18 21:01:28.125138 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/socketopts/
+-rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/socketopts/__init__.py
+-rw-rw-rw-   0        0        0     2233 2023-07-10 21:26:16.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/socketopts/schemas.py
+-rw-rw-rw-   0        0        0     4810 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/socketopts/socketOpts.py
+drwxrwxrwx   0        0        0        0 2023-07-18 21:01:28.128629 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/utilities/
+-rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/utilities/__init__.py
+-rw-rw-rw-   0        0        0     2457 2023-06-16 02:31:56.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/utilities/exceptions.py
+-rw-rw-rw-   0        0        0     1044 2023-06-29 21:33:53.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/utilities/killableThread.py
+-rw-rw-rw-   0        0        0     2328 2023-07-08 04:38:18.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/utilities/logger.py
+drwxrwxrwx   0        0        0        0 2023-07-18 21:01:28.133129 TapisCL-ICICLE-1.0.1/src/TapisCL_ICICLE.egg-info/
+-rw-rw-rw-   0        0        0    58862 2023-07-18 21:01:28.000000 TapisCL-ICICLE-1.0.1/src/TapisCL_ICICLE.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2003 2023-07-18 21:01:28.000000 TapisCL-ICICLE-1.0.1/src/TapisCL_ICICLE.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 21:01:28.000000 TapisCL-ICICLE-1.0.1/src/TapisCL_ICICLE.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-18 21:01:28.000000 TapisCL-ICICLE-1.0.1/src/TapisCL_ICICLE.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-07-18 21:01:28.000000 TapisCL-ICICLE-1.0.1/src/TapisCL_ICICLE.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-07-18 21:01:28.000000 TapisCL-ICICLE-1.0.1/src/TapisCL_ICICLE.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-06-29 16:14:59.000000 TapisCL-ICICLE-1.0.1/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 21:01:28.134125 TapisCL-ICICLE-1.0.1/tests/
+-rw-rw-rw-   0        0        0       48 2023-07-18 20:13:22.000000 TapisCL-ICICLE-1.0.1/tests/test.py
```

### Comparing `TapisCL-ICICLE-1.0.0/LICENSE` & `TapisCL-ICICLE-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.0/PKG-INFO` & `TapisCL-ICICLE-1.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 1.0.0
+Version: 1.0.1
 Summary: Provide good performance command line user interface for Tapis services hosted on HPC clusters
 Author-email: Michael Ray <m.ray37990@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -768,18 +768,15 @@
 * create_volume
 * update_volume
 * create_snapshot
 * update_snapshot
 * create_app
 * update_app
 * submit_job
-
-##### Generating Config Files
-WIP
-
+  
 #### Managerial
 Managerial commands are generally for getting information about the Tapis services you have access to, managing permissions, state, and sharing for those services. These wont usually have more than 3 arguments. 
 
 ### Services
 Each Tapis service has their own command group which allows you to interface with that service. Currently, TapisCLICICLE supports 7 services:
 * Systems
 * Files
@@ -791,13 +788,101 @@
 
 #### Systems
 Systems lie at the core of most workflows in Tapis, and TapisCLICICLE. They are representations of your account on an HPC system, and interface with HPC resources using SSH. You can read more specifics about Tapis systems [here](https://tapis.readthedocs.io/en/latest/technical/systems.html). Systems enable the user to store and access files on as well as run jobs on that resource. 
 Each system has 4 key characteristics:
 * id: the identifier for the system
 * systemType: What type of system are you interfacing with? LINUX, IRODS, or GLOBUS
 * host: What is the hostname of the system you are trying to connect to? This can be anything that supports Tapis systems, whether it be a url or IP address. SOmething like stampede2.tacc.utexas.edu
-* defaultAuthnMethod: What authentication method will you use on this system?
+* defaultAuthnMethod: What authentication method will you use on this system? 
+  * LINUX: PASSWORD or PKI_KEYS
+  * IRODS: PASSWORD
+  * GLOBUS: TOKEN
+
+##### Important System Fields
+* canExec: If you want to execute jobs on your system, you will have to specify this flag and fill out the form
+* canRunBatch: similar to canExec, if you want to run your jobs using a batch scheduler, you must specify this flag and fill out the batch form
+* jobEnvVariables: Environment variables to be passed to job containers when theyre run on your system
+* jobCapabilities: add descriptors and configurations to jobs by default
+* jobConstraints: specify how many jobs can be run at once on a system, or by a user on that system
+* rootDir: if you want to use your system for storage, this is the root directory from which file operations will be conducted on the system
 
 ##### S3 Bucket Systems
-Tapis also supports interfacing with AWS S3 Bucket systems
+Tapis also supports interfacing with AWS S3 Bucket systems. These only support the Access key authentication method. Out of the fields mentioned previously, s3 bucket systems only support the canRunBatch field
+
+##### Child Systems
+You can create child systems which inherit all attributes from the parent on creation using the create_child_system command. These children can be unlinked later, and act as standalone systems
+
+#### Files
+File commands allow the user to interface with the file system of a select system. To a limited extent, for file system navigation, and basic file management, the application replicates the linux bash environment.
+
+In order to 'enter' a system and its gain more direct access to its files, use the command `system (system_id)`. Although all the file commands have the option of specifying the system_id you are accessing the files of, entering the system using the system command makes this unecessary. You can then run commands like ls, as you would on a linux system
+
+Files can only be accessed if you are authenticated to the system the files are on. If the system does not have a rootDir attribute, files will be inaccessible
+
+you can read more about Tapis files [here](https://tapis.readthedocs.io/en/latest/technical/files.html)
+
+##### File Permissions and Sharing
+You have two options for permissions and sharing:
+* permissions: the more traditional way, granting read or modify permissions to an individual for a file or path. This is governed by grant_permissions and delete_permissions in the app
+* Postits: postits are a service for securely sharing individual file paths with large groups on a tenant or with individuals. These are interoperable between tenants as well. Postits are not persistent and die after a set period of time, and must be redeemed in order to access the files contained within. You can limit the number of times a postit can be redeemed, after which it will be deleted.
+
+#### Apps
+Apps are persistent representations of containers stored on a specific tenant. They require a systemId, for a system which has the canExec and canRunBatch flags set to true, and they are required for running jobs. The container for the job you want to run must be stored in an app. Using apps you can specify default job attributes, like environment variables or runtime characteristics. You can read more about Tapis applications [here](https://tapis.readthedocs.io/en/latest/technical/files.html).
+
+Creating an app requires an app id, a version, container image (from docker or singularity hub), and the execSystemId (the default system on which jobs derived from this app will be executed). When creating an app, you can use the same app id as an already created app, as long as you specify a new version.
+
+some important fields for app creation include:
+* configureRuntime: specify runtime options, like the runtime type (singularity or docker), as well as runtime options (SINGULARITY_START, SINGULARITY_RUN, and or NONE)
+* jobConstraints: place limits on how many jobs can be run, and specify if the job is batch or fork
+* defaultSystemConfig: specify system id for running jobs, and system filepaths for input and output files
+* appArgs: create a list of arguments that must be passed at runtime to the job for it to run
+* containerArgs: create a list of arguments for configuring the job's container
+* envVariables: create a list of environment variables to be passed to the job at runtime
+* jobAllocationConfiguration: configure features of the app like nodeCount and memory allocation.
+
+App permissions can be managed the same as files.
+
+#### Jobs
+The jobs service allows the execution of programs, 'jobs', on a system. A job must be derived from an app and run on a system with canExec (and often with canRunBatch) enabled.
+
+Submitting a job only requires an appId and job name, provided default job characteristics were specified in the app's definition. You can specify, or override these settings by specifying them directly in the submit_job command. For important job submission fields, see the important fields for app creation. To manage a job, at job creation you will be given a job Uuid. Most Job commands require this Uuid. 
+
+While a job is running you can use get_job to see it status and information. After it finishes you can see its history using get_job_history.
+
+In order to share a job, you can use the share_job command. You can list who the job is being shared with using the get_job_share command, and delete sharing with delete_job_share
+
+##### Job Subscriptions
+If you want to be notified of certain events on a job via email or webhook, you can create a subscription to a job. You can do this with the subscribe_to_job command
+
+#### Pods
+Pods are a semi-persistent way of storing data or running servers on HPC. Pods are not system dependent, and are standalone. You can read more about Tapis pods [here](https://tapis.readthedocs.io/en/latest/technical/pods.html)
+
+These are kubernetes pods running specific applications. What application is run on the pod depends on the 'template' field specified at creation time of the pod. Currently, the only publically available templates are neo4j and postgres, however you can run your own custom pod with approval from admin. If you want your own custom pod template, send a message in the Tapis slack server [here](http://bit.ly/join-tapis).
+
+Creating a pod only requires a pod id and template. Other important fields include:
+* volume_mounts: attach a kubernetes volume to backup data from pod to
+* command: list of commands to be run in the pod at runtime
+* environment_variables: environment variables for a custom pod
+* time_to_stop_default/instance: specify how long the pod will live. If set to -1 the pod lives forever, until manually stopped. If a pod stops, the data is lost unless backed up!
+
+##### Data Persistence for Pods
+As mentioned, the data on pods is semi-persistent. You could set the pod to live forever and data will persist as long as it doesnt run into any errors. If you want true data persistence you will have to use the Volumes service. When creating a pod, you can specify a volume mount, which if the volume id doesnt exist will create a new one for you. Alternatively, you can create a volume yourself.
+
+#### Volumes
+The volumes service provides an interface to kubernetes volumes, which unlike pods are fully persistent. During pod configuration, you can backup certain directories in your pod to the volume, which will be loaded to the pod if it ever restarts. You can read more about Tapis volumes [here](https://tapis-project.github.io/live-docs/?service=Pods#tag/Volumes)
+
+creating a volume only requires a volume id.
+
+If you want to create a sort of archive for a volume to save data at a certain state, you can create a snapshot using the crate_snapshot command
+
+#### Query
+Query allows direct command line interfacing with pod hosted database services, currently only neo4j and postgres. All it requires is a pod id, and you will be able to send queries to either database service. For neo4j you can also use Sahil Samar's [here](https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/tree/main/icicle_rel_03_2023/CLI/ICICONSOLE), which supports natural language parsing for neo4j
+
+### Issues
+As of right now, Im about to head off to college and wont have time to actively maintain TapisCL-ICICLE. Whether or not it gets picked up by another intern, im not sure. In any case, if you encounter an issue with app submit a bug report to [our github page](https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/issues). I will do my best to fix it for you. I do not plan on adding any major new features in future.
+
+
+
+
+
```

### Comparing `TapisCL-ICICLE-1.0.0/pyproject.toml` & `TapisCL-ICICLE-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel", "poetry-core>=1.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "TapisCL-ICICLE"
-version = "1.0.0"
+version = "1.0.1"
 description = "Provide good performance command line user interface for Tapis services hosted on HPC clusters"
 readme = "README.md"
 authors = [{ name = "Michael Ray", email = "m.ray37990@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License (GPL)",
     "Programming Language :: Python",
```

### Comparing `TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/client/cli.py` & `TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/client/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,14 @@
 
     def initialize_server(self): 
         """
         detect client operating system. The local server intitialization is different between unix and windows based systems
         """
         if 'win' in sys.platform:
             os.system(rf"pythonw {server_path} 1>stdout.txt 2>stderr.txt")
-            #os.system(rf"python {server_path}")
         else: # unix based
             subprocess.Popen(['nohup', 'python3', server_path, '&'], stdout=subprocess.PIPE, stderr=subprocess.PIPE)
 
     #@decorators.AnimatedLoading
     def connection_initialization(self):
         """
         start the local server through the client
```

### Comparing `TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/client/handlers.py` & `TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/client/handlers.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/Apps/appCommands.py` & `TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/Apps/appCommands.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/Apps/appForms.py` & `TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/Apps/appForms.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/Systems/systemCommands.py` & `TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/Systems/systemCommands.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/Systems/systemForms.py` & `TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/Systems/systemForms.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/arguments/argument.py` & `TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/arguments/argument.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,15 +161,15 @@
                 flattened_form_info = {self.argument:True}
                 flattened_form_info.update(**{arg_name:arg_value for arg_name, arg_value in value[self.argument].items()})
                 return flattened_form_info
             if self.flattening_type == 'RETRIEVE':
                 exctracted_form_data = {arg_name:arg for arg_name, arg in value[self.argument].items()}
                 return exctracted_form_data
             else:
-                return value
+                return value[self.argument]
 
     def json(self):
         fields = {argument_name:argument.json() for argument_name, argument in self.arguments_list.items()}
         json = {
             'name':self.argument,
             'arg_type':self.arg_type,
             'data_type':self.data_type,
```

### Comparing `TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/arguments/argumentValidators.py` & `TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/arguments/argumentValidators.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/baseCommand.py` & `TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/baseCommand.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,14 +208,16 @@
                 response_value = argument.verify_rules_followed(response_value)
                 if argument.arg_type == 'form' and argument.flattening_type in ('FLATTEN', 'RETRIEVE'):
                     kwargs.pop(arg_name)
                 if argument.part_of:
                     if argument.part_of not in kwargs:
                         kwargs[argument.part_of] = dict()
                     kwargs[argument.part_of][argument.argument] = response_value
+                elif argument.arg_type != 'form':
+                    kwargs.update(**{arg_name:response_value})
                 else:
                     kwargs.update(**response_value)
         return kwargs
 
     async def handle_arg_opts(self, kwargs):
         """
         arg opts handle special operations, like supporting relative file paths, and system entry
```

### Comparing `TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/commandMap.py` & `TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/commandMap.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,15 +117,17 @@
         'pwd':fileCommands.pwd(),
         'showme':fileCommands.showme(),
         'cat':fileCommands.cat(),
         'mkdir':fileCommands.mkdir(),
         'mv':fileCommands.mv(),
         'cp':fileCommands.cp(),
         'rm':fileCommands.rm(),
-        #'get_recent_transfers':fileCommands.get_recent_transfers(),
+        'get_permissions':fileCommands.get_permissions(),
+        'grant_permissions':fileCommands.grant_permissions(),
+        'delete_permissions':fileCommands.delete_permissions(),
         'create_postit':fileCommands.create_postit(),
         'list_postits':fileCommands.list_postits(),
         'get_postit':fileCommands.get_postit(),
         'delete_postit':fileCommands.delete_postit(),
         'redeem_postit':fileCommands.redeem_postit(),
         'upload':fileCommands.upload(),
         'download':fileCommands.download(),
@@ -163,14 +165,15 @@
         'unhide_job':jobCommands.unhide_job(),
         'cancel_job':jobCommands.cancel_job(),
         'get_job':jobCommands.get_job(),
         'get_job_history':jobCommands.get_job_history(),
         'get_jobs':jobCommands.get_jobs(),
         'download_job_output':jobCommands.download_job_output(),
         'get_job_status':jobCommands.get_job_status(),
+        'get_job_last_message':jobCommands.get_job_last_message(),
         'resubmit_job':jobCommands.resubmit_job(),
         'submit_job':jobCommands.submit_job(),
         'share_job':jobCommands.share_job(),
         'get_job_share':jobCommands.get_job_share(),
         'delete_job_share':jobCommands.delete_job_share(),
         'subscribe_to_job':jobCommands.subscribe_to_job(),
         'get_subscriptions':jobCommands.get_subscriptions(),
```

### Comparing `TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/commandOpts.py` & `TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/commandOpts.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/dataFormatters.py` & `TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/dataFormatters.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,11 +39,12 @@
                 return_data = list()
                 for fragment in serialized:
                     non_verbose_fragment = self.non_verbose_formatter(fragment)
                     return_data.append(non_verbose_fragment)
                 return return_data
             return self.non_verbose_formatter(serialized)
         else:
+            print("ASSFUCK IMMINENT")
             return data
```

### Comparing `TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/decorators.py` & `TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/decorators.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/fileCommands.py` & `TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/fileCommands.py`

 * *Files 3% similar despite different names*

```diff
@@ -153,16 +153,58 @@
         Argument('source_file_path', positional=True),
         Argument('source_system_id', positional=True),
         Argument('destination_system_id'),
         Argument('destination_file_path')
     ]
     async def run(self, *args, **kwargs):
         pass
+
+
+class grant_permissions(baseCommand.BaseCommand):
+    """
+    @help: grant permission to a file path for a user
+    """
+    return_fields = ['username', 'permission', 'path']
+    command_opt = [commandOpts.CHECK_PWD(('path',)), commandOpts.CHECK_EXPLICIT_ID('systemId')]
+    required_arguments = [
+        Argument('path', positional=True),
+        Argument('systemId', positional=True),
+        Argument('username'),
+        Argument('permission', choices=['READ', 'MODIFY'])
+    ]
+    async def run(self, *args, **kwargs):
+        return self.t.files.grantPermissions(**kwargs)
+    
+
+class get_permissions(grant_permissions):
+    """
+    @help: see what permissions users have on a file or path
+    """
+    required_arguments = [
+        Argument('path', positional=True),
+        Argument('systemId', positional=True)
+    ]
+    async def run(self, *args, **kwargs):
+        return self.t.files.getPermissions(**kwargs)
     
 
+class delete_permissions(baseCommand.BaseCommand):
+    """
+    @help: delete permissions to a filepath
+    """
+    command_opt = [commandOpts.CHECK_PWD(('path',)), commandOpts.CHECK_EXPLICIT_ID('systemId')]
+    required_arguments = [
+        Argument('path', positional=True),
+        Argument('systemId', positional=True),
+        Argument('username')
+    ]
+    async def run(self, *args, **kwargs):
+        return self.t.files.deletePermissions(**kwargs)
+
+
 class create_postit(baseCommand.BaseCommand):
     """
     @help: create a postit to easily share file with other users
     """
     return_fields = ['postitId', 'systemId', 'path', 'redeemUrl']
     command_opt = [commandOpts.CHECK_PWD(('file_path',)), commandOpts.CHECK_EXPLICIT_ID('systemId')]
     required_arguments = [
```

### Comparing `TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/jobCommands.py` & `TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/jobCommands.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,14 +92,24 @@
     required_arguments = [
         Argument('jobUuid')
     ]
     async def run(self, *args, **kwargs):
         return self.t.jobs.getJobStatus(**kwargs)
     
 
+class get_job_last_message(baseCommand.BaseCommand):
+    """
+    @help: retrieve the last message of a job
+    """
+    required_arguments = [
+        Argument('jobUuid')
+    ]
+    async def run(self, *args, **kwargs):
+        return self.t.jobs.getJob(**kwargs).lastMessage
+
 class resubmit_job(baseCommand.BaseCommand):
     """
     @help: resubmit a job with the same arguments as the original submission
     """
     return_fields = ['name', 'status', 'uuid', 'appId', 'execSystemId']
     required_arguments = [
         Argument('jobUuid'),
@@ -127,15 +137,15 @@
     """
     @help: share a job with the select grantee user
     """
     required_arguments = [
         Argument('jobUuid')
     ]
     optional_arguments = [
-        Argument('grantee'),
+        Argument('grantee', description='Who are you sharing this with?'),
         Argument('jobResource', choices=['JOB_HISTORY', 'JOB_RESUBMIT_REQUEST', 'JOB_OUTPUT', 'JOB_INPUT']),
         Argument('jobPermission', choices=['READ'])
     ]
     async def run(self, *args, **kwargs):
         return self.t.jobs.shareJob(**kwargs)
```

### Comparing `TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/podCommands.py` & `TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/podCommands.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/query/neo4j.py` & `TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/query/neo4j.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/query/postgres.py` & `TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/query/postgres.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/serverCommands.py` & `TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/serverCommands.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/commands/volumeCommands.py` & `TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/volumeCommands.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/server/auth.py` & `TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/server/auth.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/server/server.py` & `TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/server/server.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/socketopts/schemas.py` & `TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/socketopts/schemas.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/socketopts/socketOpts.py` & `TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/socketopts/socketOpts.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/utilities/exceptions.py` & `TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/utilities/killableThread.py` & `TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/utilities/killableThread.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.0/src/TapisCLICICLE/utilities/logger.py` & `TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/utilities/logger.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.0/src/TapisCL_ICICLE.egg-info/PKG-INFO` & `TapisCL-ICICLE-1.0.1/src/TapisCL_ICICLE.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 1.0.0
+Version: 1.0.1
 Summary: Provide good performance command line user interface for Tapis services hosted on HPC clusters
 Author-email: Michael Ray <m.ray37990@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -768,18 +768,15 @@
 * create_volume
 * update_volume
 * create_snapshot
 * update_snapshot
 * create_app
 * update_app
 * submit_job
-
-##### Generating Config Files
-WIP
-
+  
 #### Managerial
 Managerial commands are generally for getting information about the Tapis services you have access to, managing permissions, state, and sharing for those services. These wont usually have more than 3 arguments. 
 
 ### Services
 Each Tapis service has their own command group which allows you to interface with that service. Currently, TapisCLICICLE supports 7 services:
 * Systems
 * Files
@@ -791,13 +788,101 @@
 
 #### Systems
 Systems lie at the core of most workflows in Tapis, and TapisCLICICLE. They are representations of your account on an HPC system, and interface with HPC resources using SSH. You can read more specifics about Tapis systems [here](https://tapis.readthedocs.io/en/latest/technical/systems.html). Systems enable the user to store and access files on as well as run jobs on that resource. 
 Each system has 4 key characteristics:
 * id: the identifier for the system
 * systemType: What type of system are you interfacing with? LINUX, IRODS, or GLOBUS
 * host: What is the hostname of the system you are trying to connect to? This can be anything that supports Tapis systems, whether it be a url or IP address. SOmething like stampede2.tacc.utexas.edu
-* defaultAuthnMethod: What authentication method will you use on this system?
+* defaultAuthnMethod: What authentication method will you use on this system? 
+  * LINUX: PASSWORD or PKI_KEYS
+  * IRODS: PASSWORD
+  * GLOBUS: TOKEN
+
+##### Important System Fields
+* canExec: If you want to execute jobs on your system, you will have to specify this flag and fill out the form
+* canRunBatch: similar to canExec, if you want to run your jobs using a batch scheduler, you must specify this flag and fill out the batch form
+* jobEnvVariables: Environment variables to be passed to job containers when theyre run on your system
+* jobCapabilities: add descriptors and configurations to jobs by default
+* jobConstraints: specify how many jobs can be run at once on a system, or by a user on that system
+* rootDir: if you want to use your system for storage, this is the root directory from which file operations will be conducted on the system
 
 ##### S3 Bucket Systems
-Tapis also supports interfacing with AWS S3 Bucket systems
+Tapis also supports interfacing with AWS S3 Bucket systems. These only support the Access key authentication method. Out of the fields mentioned previously, s3 bucket systems only support the canRunBatch field
+
+##### Child Systems
+You can create child systems which inherit all attributes from the parent on creation using the create_child_system command. These children can be unlinked later, and act as standalone systems
+
+#### Files
+File commands allow the user to interface with the file system of a select system. To a limited extent, for file system navigation, and basic file management, the application replicates the linux bash environment.
+
+In order to 'enter' a system and its gain more direct access to its files, use the command `system (system_id)`. Although all the file commands have the option of specifying the system_id you are accessing the files of, entering the system using the system command makes this unecessary. You can then run commands like ls, as you would on a linux system
+
+Files can only be accessed if you are authenticated to the system the files are on. If the system does not have a rootDir attribute, files will be inaccessible
+
+you can read more about Tapis files [here](https://tapis.readthedocs.io/en/latest/technical/files.html)
+
+##### File Permissions and Sharing
+You have two options for permissions and sharing:
+* permissions: the more traditional way, granting read or modify permissions to an individual for a file or path. This is governed by grant_permissions and delete_permissions in the app
+* Postits: postits are a service for securely sharing individual file paths with large groups on a tenant or with individuals. These are interoperable between tenants as well. Postits are not persistent and die after a set period of time, and must be redeemed in order to access the files contained within. You can limit the number of times a postit can be redeemed, after which it will be deleted.
+
+#### Apps
+Apps are persistent representations of containers stored on a specific tenant. They require a systemId, for a system which has the canExec and canRunBatch flags set to true, and they are required for running jobs. The container for the job you want to run must be stored in an app. Using apps you can specify default job attributes, like environment variables or runtime characteristics. You can read more about Tapis applications [here](https://tapis.readthedocs.io/en/latest/technical/files.html).
+
+Creating an app requires an app id, a version, container image (from docker or singularity hub), and the execSystemId (the default system on which jobs derived from this app will be executed). When creating an app, you can use the same app id as an already created app, as long as you specify a new version.
+
+some important fields for app creation include:
+* configureRuntime: specify runtime options, like the runtime type (singularity or docker), as well as runtime options (SINGULARITY_START, SINGULARITY_RUN, and or NONE)
+* jobConstraints: place limits on how many jobs can be run, and specify if the job is batch or fork
+* defaultSystemConfig: specify system id for running jobs, and system filepaths for input and output files
+* appArgs: create a list of arguments that must be passed at runtime to the job for it to run
+* containerArgs: create a list of arguments for configuring the job's container
+* envVariables: create a list of environment variables to be passed to the job at runtime
+* jobAllocationConfiguration: configure features of the app like nodeCount and memory allocation.
+
+App permissions can be managed the same as files.
+
+#### Jobs
+The jobs service allows the execution of programs, 'jobs', on a system. A job must be derived from an app and run on a system with canExec (and often with canRunBatch) enabled.
+
+Submitting a job only requires an appId and job name, provided default job characteristics were specified in the app's definition. You can specify, or override these settings by specifying them directly in the submit_job command. For important job submission fields, see the important fields for app creation. To manage a job, at job creation you will be given a job Uuid. Most Job commands require this Uuid. 
+
+While a job is running you can use get_job to see it status and information. After it finishes you can see its history using get_job_history.
+
+In order to share a job, you can use the share_job command. You can list who the job is being shared with using the get_job_share command, and delete sharing with delete_job_share
+
+##### Job Subscriptions
+If you want to be notified of certain events on a job via email or webhook, you can create a subscription to a job. You can do this with the subscribe_to_job command
+
+#### Pods
+Pods are a semi-persistent way of storing data or running servers on HPC. Pods are not system dependent, and are standalone. You can read more about Tapis pods [here](https://tapis.readthedocs.io/en/latest/technical/pods.html)
+
+These are kubernetes pods running specific applications. What application is run on the pod depends on the 'template' field specified at creation time of the pod. Currently, the only publically available templates are neo4j and postgres, however you can run your own custom pod with approval from admin. If you want your own custom pod template, send a message in the Tapis slack server [here](http://bit.ly/join-tapis).
+
+Creating a pod only requires a pod id and template. Other important fields include:
+* volume_mounts: attach a kubernetes volume to backup data from pod to
+* command: list of commands to be run in the pod at runtime
+* environment_variables: environment variables for a custom pod
+* time_to_stop_default/instance: specify how long the pod will live. If set to -1 the pod lives forever, until manually stopped. If a pod stops, the data is lost unless backed up!
+
+##### Data Persistence for Pods
+As mentioned, the data on pods is semi-persistent. You could set the pod to live forever and data will persist as long as it doesnt run into any errors. If you want true data persistence you will have to use the Volumes service. When creating a pod, you can specify a volume mount, which if the volume id doesnt exist will create a new one for you. Alternatively, you can create a volume yourself.
+
+#### Volumes
+The volumes service provides an interface to kubernetes volumes, which unlike pods are fully persistent. During pod configuration, you can backup certain directories in your pod to the volume, which will be loaded to the pod if it ever restarts. You can read more about Tapis volumes [here](https://tapis-project.github.io/live-docs/?service=Pods#tag/Volumes)
+
+creating a volume only requires a volume id.
+
+If you want to create a sort of archive for a volume to save data at a certain state, you can create a snapshot using the crate_snapshot command
+
+#### Query
+Query allows direct command line interfacing with pod hosted database services, currently only neo4j and postgres. All it requires is a pod id, and you will be able to send queries to either database service. For neo4j you can also use Sahil Samar's [here](https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/tree/main/icicle_rel_03_2023/CLI/ICICONSOLE), which supports natural language parsing for neo4j
+
+### Issues
+As of right now, Im about to head off to college and wont have time to actively maintain TapisCL-ICICLE. Whether or not it gets picked up by another intern, im not sure. In any case, if you encounter an issue with app submit a bug report to [our github page](https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/issues). I will do my best to fix it for you. I do not plan on adding any major new features in future.
+
+
+
+
+
```

### Comparing `TapisCL-ICICLE-1.0.0/src/TapisCL_ICICLE.egg-info/SOURCES.txt` & `TapisCL-ICICLE-1.0.1/src/TapisCL_ICICLE.egg-info/SOURCES.txt`

 * *Files identical despite different names*

