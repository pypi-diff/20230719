# Comparing `tmp/TapisCL-ICICLE-1.0.1.tar.gz` & `tmp/TapisCL-ICICLE-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TapisCL-ICICLE-1.0.1.tar", last modified: Tue Jul 18 21:01:28 2023, max compression
+gzip compressed data, was "TapisCL-ICICLE-1.0.2.tar", last modified: Tue Jul 18 22:45:12 2023, max compression
```

## Comparing `TapisCL-ICICLE-1.0.1.tar` & `TapisCL-ICICLE-1.0.2.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 21:01:28.135121 TapisCL-ICICLE-1.0.1/
--rw-rw-rw-   0        0        0    35823 2023-04-12 23:35:22.000000 TapisCL-ICICLE-1.0.1/LICENSE
--rw-rw-rw-   0        0        0    58862 2023-07-18 21:01:28.135121 TapisCL-ICICLE-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    16981 2023-07-18 20:02:58.000000 TapisCL-ICICLE-1.0.1/README.md
--rw-rw-rw-   0        0        0     1227 2023-07-18 21:00:49.000000 TapisCL-ICICLE-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-18 21:01:28.135121 TapisCL-ICICLE-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-18 21:01:28.100664 TapisCL-ICICLE-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-18 21:01:28.102656 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/
--rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/__init__.py
--rw-rw-rw-   0        0        0      321 2023-06-29 16:14:59.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 21:01:28.104649 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/client/
--rw-rw-rw-   0        0        0       84 2023-05-23 19:58:53.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/client/__init__.py
--rw-rw-rw-   0        0        0    10738 2023-07-18 20:56:23.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/client/cli.py
--rw-rw-rw-   0        0        0    16008 2023-07-17 19:00:49.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/client/handlers.py
-drwxrwxrwx   0        0        0        0 2023-07-18 21:01:28.111155 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/
-drwxrwxrwx   0        0        0        0 2023-07-18 21:01:28.115142 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/Apps/
--rw-rw-rw-   0        0        0        0 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/Apps/__init__.py
--rw-rw-rw-   0        0        0    11096 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/Apps/appCommands.py
--rw-rw-rw-   0        0        0      259 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/Apps/appConfigGenerator.py
--rw-rw-rw-   0        0        0     4859 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/Apps/appForms.py
-drwxrwxrwx   0        0        0        0 2023-07-18 21:01:28.116643 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/Systems/
--rw-rw-rw-   0        0        0        0 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/Systems/__init__.py
--rw-rw-rw-   0        0        0    23546 2023-07-17 15:51:32.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/Systems/systemCommands.py
--rw-rw-rw-   0        0        0     3940 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/Systems/systemForms.py
--rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 21:01:28.119154 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/arguments/
--rw-rw-rw-   0        0        0        0 2023-06-16 01:12:43.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/arguments/__init__.py
--rw-rw-rw-   0        0        0     9298 2023-07-18 20:47:15.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/arguments/argument.py
--rw-rw-rw-   0        0        0     4772 2023-07-18 16:34:22.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/arguments/argumentValidators.py
--rw-rw-rw-   0        0        0    20942 2023-07-18 20:46:18.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/baseCommand.py
--rw-rw-rw-   0        0        0    10976 2023-07-18 20:01:13.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/commandMap.py
--rw-rw-rw-   0        0        0     2221 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/commandOpts.py
--rw-rw-rw-   0        0        0     1867 2023-07-18 20:33:33.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/dataFormatters.py
--rw-rw-rw-   0        0        0     4947 2023-07-10 21:26:23.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/decorators.py
--rw-rw-rw-   0        0        0    12824 2023-07-18 20:04:51.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/fileCommands.py
--rw-rw-rw-   0        0        0     7522 2023-07-18 20:00:48.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/jobCommands.py
--rw-rw-rw-   0        0        0    13236 2023-07-18 18:01:26.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/podCommands.py
-drwxrwxrwx   0        0        0        0 2023-07-18 21:01:28.121150 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/query/
--rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/query/__init__.py
--rw-rw-rw-   0        0        0     1615 2023-07-11 17:42:26.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/query/neo4j.py
--rw-rw-rw-   0        0        0      871 2023-06-16 01:12:43.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/query/postgres.py
--rw-rw-rw-   0        0        0     4412 2023-07-17 15:54:36.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/serverCommands.py
--rw-rw-rw-   0        0        0     7990 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/volumeCommands.py
-drwxrwxrwx   0        0        0        0 2023-07-18 21:01:28.123144 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/server/
--rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/server/__init__.py
--rw-rw-rw-   0        0        0    10928 2023-07-06 00:52:04.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/server/auth.py
--rw-rw-rw-   0        0        0    10402 2023-07-17 16:55:28.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/server/server.py
--rw-rw-rw-   0        0        0      290 2023-07-05 15:04:52.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/serverRun.py
-drwxrwxrwx   0        0        0        0 2023-07-18 21:01:28.125138 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/socketopts/
--rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/socketopts/__init__.py
--rw-rw-rw-   0        0        0     2233 2023-07-10 21:26:16.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/socketopts/schemas.py
--rw-rw-rw-   0        0        0     4810 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/socketopts/socketOpts.py
-drwxrwxrwx   0        0        0        0 2023-07-18 21:01:28.128629 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/utilities/
--rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/utilities/__init__.py
--rw-rw-rw-   0        0        0     2457 2023-06-16 02:31:56.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/utilities/exceptions.py
--rw-rw-rw-   0        0        0     1044 2023-06-29 21:33:53.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/utilities/killableThread.py
--rw-rw-rw-   0        0        0     2328 2023-07-08 04:38:18.000000 TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/utilities/logger.py
-drwxrwxrwx   0        0        0        0 2023-07-18 21:01:28.133129 TapisCL-ICICLE-1.0.1/src/TapisCL_ICICLE.egg-info/
--rw-rw-rw-   0        0        0    58862 2023-07-18 21:01:28.000000 TapisCL-ICICLE-1.0.1/src/TapisCL_ICICLE.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2003 2023-07-18 21:01:28.000000 TapisCL-ICICLE-1.0.1/src/TapisCL_ICICLE.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 21:01:28.000000 TapisCL-ICICLE-1.0.1/src/TapisCL_ICICLE.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-07-18 21:01:28.000000 TapisCL-ICICLE-1.0.1/src/TapisCL_ICICLE.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-07-18 21:01:28.000000 TapisCL-ICICLE-1.0.1/src/TapisCL_ICICLE.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-07-18 21:01:28.000000 TapisCL-ICICLE-1.0.1/src/TapisCL_ICICLE.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-06-29 16:14:59.000000 TapisCL-ICICLE-1.0.1/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 21:01:28.134125 TapisCL-ICICLE-1.0.1/tests/
--rw-rw-rw-   0        0        0       48 2023-07-18 20:13:22.000000 TapisCL-ICICLE-1.0.1/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-07-18 22:45:12.561767 TapisCL-ICICLE-1.0.2/
+-rw-rw-rw-   0        0        0    35823 2023-04-12 23:35:22.000000 TapisCL-ICICLE-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0    58862 2023-07-18 22:45:12.561767 TapisCL-ICICLE-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    16981 2023-07-18 20:02:58.000000 TapisCL-ICICLE-1.0.2/README.md
+-rw-rw-rw-   0        0        0     1227 2023-07-18 22:44:29.000000 TapisCL-ICICLE-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-18 22:45:12.561767 TapisCL-ICICLE-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-18 22:45:12.526553 TapisCL-ICICLE-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-18 22:45:12.528851 TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/
+-rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/__init__.py
+-rw-rw-rw-   0        0        0      321 2023-06-29 16:14:59.000000 TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 22:45:12.530845 TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/client/
+-rw-rw-rw-   0        0        0       84 2023-05-23 19:58:53.000000 TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/client/__init__.py
+-rw-rw-rw-   0        0        0    10916 2023-07-18 21:38:48.000000 TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/client/cli.py
+-rw-rw-rw-   0        0        0    16008 2023-07-17 19:00:49.000000 TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/client/handlers.py
+drwxrwxrwx   0        0        0        0 2023-07-18 22:45:12.539496 TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/commands/
+drwxrwxrwx   0        0        0        0 2023-07-18 22:45:12.542486 TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/commands/Apps/
+-rw-rw-rw-   0        0        0        0 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/commands/Apps/__init__.py
+-rw-rw-rw-   0        0        0    11096 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/commands/Apps/appCommands.py
+-rw-rw-rw-   0        0        0      259 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/commands/Apps/appConfigGenerator.py
+-rw-rw-rw-   0        0        0     4859 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/commands/Apps/appForms.py
+drwxrwxrwx   0        0        0        0 2023-07-18 22:45:12.545494 TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/commands/Systems/
+-rw-rw-rw-   0        0        0        0 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/commands/Systems/__init__.py
+-rw-rw-rw-   0        0        0    23546 2023-07-17 15:51:32.000000 TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/commands/Systems/systemCommands.py
+-rw-rw-rw-   0        0        0     3940 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/commands/Systems/systemForms.py
+-rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/commands/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 22:45:12.546506 TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/commands/arguments/
+-rw-rw-rw-   0        0        0        0 2023-06-16 01:12:43.000000 TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/commands/arguments/__init__.py
+-rw-rw-rw-   0        0        0     9383 2023-07-18 22:42:58.000000 TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/commands/arguments/argument.py
+-rw-rw-rw-   0        0        0     4772 2023-07-18 16:34:22.000000 TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/commands/arguments/argumentValidators.py
+-rw-rw-rw-   0        0        0    20942 2023-07-18 20:46:18.000000 TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/commands/baseCommand.py
+-rw-rw-rw-   0        0        0    10976 2023-07-18 20:01:13.000000 TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/commands/commandMap.py
+-rw-rw-rw-   0        0        0     2221 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/commands/commandOpts.py
+-rw-rw-rw-   0        0        0     1828 2023-07-18 22:42:23.000000 TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/commands/dataFormatters.py
+-rw-rw-rw-   0        0        0     4947 2023-07-10 21:26:23.000000 TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/commands/decorators.py
+-rw-rw-rw-   0        0        0    12824 2023-07-18 20:04:51.000000 TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/commands/fileCommands.py
+-rw-rw-rw-   0        0        0     7522 2023-07-18 20:00:48.000000 TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/commands/jobCommands.py
+-rw-rw-rw-   0        0        0    13236 2023-07-18 18:01:26.000000 TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/commands/podCommands.py
+drwxrwxrwx   0        0        0        0 2023-07-18 22:45:12.548898 TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/commands/query/
+-rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/commands/query/__init__.py
+-rw-rw-rw-   0        0        0     1615 2023-07-11 17:42:26.000000 TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/commands/query/neo4j.py
+-rw-rw-rw-   0        0        0      871 2023-06-16 01:12:43.000000 TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/commands/query/postgres.py
+-rw-rw-rw-   0        0        0     4412 2023-07-17 15:54:36.000000 TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/commands/serverCommands.py
+-rw-rw-rw-   0        0        0     7990 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/commands/volumeCommands.py
+drwxrwxrwx   0        0        0        0 2023-07-18 22:45:12.550893 TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/server/
+-rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/server/__init__.py
+-rw-rw-rw-   0        0        0    10928 2023-07-06 00:52:04.000000 TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/server/auth.py
+-rw-rw-rw-   0        0        0    10402 2023-07-17 16:55:28.000000 TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/server/server.py
+-rw-rw-rw-   0        0        0      290 2023-07-05 15:04:52.000000 TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/serverRun.py
+drwxrwxrwx   0        0        0        0 2023-07-18 22:45:12.552885 TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/socketopts/
+-rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/socketopts/__init__.py
+-rw-rw-rw-   0        0        0     2233 2023-07-10 21:26:16.000000 TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/socketopts/schemas.py
+-rw-rw-rw-   0        0        0     4810 2023-07-17 15:25:07.000000 TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/socketopts/socketOpts.py
+drwxrwxrwx   0        0        0        0 2023-07-18 22:45:12.556395 TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/utilities/
+-rw-rw-rw-   0        0        0        0 2023-05-23 19:58:53.000000 TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/utilities/__init__.py
+-rw-rw-rw-   0        0        0     2457 2023-06-16 02:31:56.000000 TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/utilities/exceptions.py
+-rw-rw-rw-   0        0        0     1044 2023-06-29 21:33:53.000000 TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/utilities/killableThread.py
+-rw-rw-rw-   0        0        0     2328 2023-07-08 04:38:18.000000 TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/utilities/logger.py
+drwxrwxrwx   0        0        0        0 2023-07-18 22:45:12.559774 TapisCL-ICICLE-1.0.2/src/TapisCL_ICICLE.egg-info/
+-rw-rw-rw-   0        0        0    58862 2023-07-18 22:45:12.000000 TapisCL-ICICLE-1.0.2/src/TapisCL_ICICLE.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2003 2023-07-18 22:45:12.000000 TapisCL-ICICLE-1.0.2/src/TapisCL_ICICLE.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 22:45:12.000000 TapisCL-ICICLE-1.0.2/src/TapisCL_ICICLE.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-18 22:45:12.000000 TapisCL-ICICLE-1.0.2/src/TapisCL_ICICLE.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-07-18 22:45:12.000000 TapisCL-ICICLE-1.0.2/src/TapisCL_ICICLE.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-07-18 22:45:12.000000 TapisCL-ICICLE-1.0.2/src/TapisCL_ICICLE.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-06-29 16:14:59.000000 TapisCL-ICICLE-1.0.2/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 22:45:12.560770 TapisCL-ICICLE-1.0.2/tests/
+-rw-rw-rw-   0        0        0       48 2023-07-18 20:13:22.000000 TapisCL-ICICLE-1.0.2/tests/test.py
```

### Comparing `TapisCL-ICICLE-1.0.1/LICENSE` & `TapisCL-ICICLE-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.1/PKG-INFO` & `TapisCL-ICICLE-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 1.0.1
+Version: 1.0.2
 Summary: Provide good performance command line user interface for Tapis services hosted on HPC clusters
 Author-email: Michael Ray <m.ray37990@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `TapisCL-ICICLE-1.0.1/README.md` & `TapisCL-ICICLE-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.1/pyproject.toml` & `TapisCL-ICICLE-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel", "poetry-core>=1.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "TapisCL-ICICLE"
-version = "1.0.1"
+version = "1.0.2"
 description = "Provide good performance command line user interface for Tapis services hosted on HPC clusters"
 readme = "README.md"
 authors = [{ name = "Michael Ray", email = "m.ray37990@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License (GPL)",
     "Programming Language :: Python",
```

### Comparing `TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/client/cli.py` & `TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/client/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,14 +99,16 @@
 
     def initialize_server(self): 
         """
         detect client operating system. The local server intitialization is different between unix and windows based systems
         """
         if 'win' in sys.platform:
             os.system(rf"pythonw {server_path} 1>stdout.txt 2>stderr.txt")
+        elif 'darwin' in sys.platform:
+            subprocess.Popen(['python3', server_path], stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True, preexec_fn=os.setsid)
         else: # unix based
             subprocess.Popen(['nohup', 'python3', server_path, '&'], stdout=subprocess.PIPE, stderr=subprocess.PIPE)
 
     #@decorators.AnimatedLoading
     def connection_initialization(self):
         """
         start the local server through the client
```

### Comparing `TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/client/handlers.py` & `TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/client/handlers.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/Apps/appCommands.py` & `TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/commands/Apps/appCommands.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/Apps/appForms.py` & `TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/commands/Apps/appForms.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/Systems/systemCommands.py` & `TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/commands/Systems/systemCommands.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/Systems/systemForms.py` & `TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/commands/Systems/systemForms.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/arguments/argument.py` & `TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/commands/arguments/argument.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,15 +161,18 @@
                 flattened_form_info = {self.argument:True}
                 flattened_form_info.update(**{arg_name:arg_value for arg_name, arg_value in value[self.argument].items()})
                 return flattened_form_info
             if self.flattening_type == 'RETRIEVE':
                 exctracted_form_data = {arg_name:arg for arg_name, arg in value[self.argument].items()}
                 return exctracted_form_data
             else:
-                return value[self.argument]
+                try:
+                    return value[self.argument]
+                except:
+                    return value
 
     def json(self):
         fields = {argument_name:argument.json() for argument_name, argument in self.arguments_list.items()}
         json = {
             'name':self.argument,
             'arg_type':self.arg_type,
             'data_type':self.data_type,
```

### Comparing `TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/arguments/argumentValidators.py` & `TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/commands/arguments/argumentValidators.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/baseCommand.py` & `TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/commands/baseCommand.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/commandMap.py` & `TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/commands/commandMap.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/commandOpts.py` & `TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/commands/commandOpts.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/dataFormatters.py` & `TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/commands/dataFormatters.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,12 +39,11 @@
                 return_data = list()
                 for fragment in serialized:
                     non_verbose_fragment = self.non_verbose_formatter(fragment)
                     return_data.append(non_verbose_fragment)
                 return return_data
             return self.non_verbose_formatter(serialized)
         else:
-            print("ASSFUCK IMMINENT")
             return data
```

### Comparing `TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/decorators.py` & `TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/commands/decorators.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/fileCommands.py` & `TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/commands/fileCommands.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/jobCommands.py` & `TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/commands/jobCommands.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/podCommands.py` & `TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/commands/podCommands.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/query/neo4j.py` & `TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/commands/query/neo4j.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/query/postgres.py` & `TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/commands/query/postgres.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/serverCommands.py` & `TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/commands/serverCommands.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/commands/volumeCommands.py` & `TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/commands/volumeCommands.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/server/auth.py` & `TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/server/auth.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/server/server.py` & `TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/server/server.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/socketopts/schemas.py` & `TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/socketopts/schemas.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/socketopts/socketOpts.py` & `TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/socketopts/socketOpts.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/utilities/exceptions.py` & `TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/utilities/killableThread.py` & `TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/utilities/killableThread.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.1/src/TapisCLICICLE/utilities/logger.py` & `TapisCL-ICICLE-1.0.2/src/TapisCLICICLE/utilities/logger.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-1.0.1/src/TapisCL_ICICLE.egg-info/PKG-INFO` & `TapisCL-ICICLE-1.0.2/src/TapisCL_ICICLE.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 1.0.1
+Version: 1.0.2
 Summary: Provide good performance command line user interface for Tapis services hosted on HPC clusters
 Author-email: Michael Ray <m.ray37990@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `TapisCL-ICICLE-1.0.1/src/TapisCL_ICICLE.egg-info/SOURCES.txt` & `TapisCL-ICICLE-1.0.2/src/TapisCL_ICICLE.egg-info/SOURCES.txt`

 * *Files identical despite different names*

