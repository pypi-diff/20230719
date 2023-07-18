# Comparing `tmp/schemachange-3.5.2.tar.gz` & `tmp/schemachange-3.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schemachange-3.5.2.tar", last modified: Wed Feb 15 05:48:25 2023, max compression
+gzip compressed data, was "schemachange-3.5.3.tar", last modified: Tue Jul 18 22:53:23 2023, max compression
```

## Comparing `schemachange-3.5.2.tar` & `schemachange-3.5.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 jhansen    (501) staff       (20)        0 2023-02-15 05:48:25.035005 schemachange-3.5.2/
--rw-r--r--   0 jhansen    (501) staff       (20)    11357 2021-10-28 21:28:24.000000 schemachange-3.5.2/LICENSE
--rw-r--r--   0 jhansen    (501) staff       (20)     1193 2021-10-28 21:28:24.000000 schemachange-3.5.2/NOTICE
--rw-r--r--   0 jhansen    (501) staff       (20)    32235 2023-02-15 05:48:25.035163 schemachange-3.5.2/PKG-INFO
--rw-r--r--   0 jhansen    (501) staff       (20)    31704 2023-02-06 19:25:20.000000 schemachange-3.5.2/README.md
--rw-r--r--   0 jhansen    (501) staff       (20)      106 2021-11-08 20:07:59.000000 schemachange-3.5.2/pyproject.toml
-drwxr-xr-x   0 jhansen    (501) staff       (20)        0 2023-02-15 05:48:25.027972 schemachange-3.5.2/schemachange/
--rw-r--r--   0 jhansen    (501) staff       (20)        0 2021-10-28 21:28:24.000000 schemachange-3.5.2/schemachange/__init__.py
--rw-r--r--   0 jhansen    (501) staff       (20)    39070 2023-02-15 05:35:21.000000 schemachange-3.5.2/schemachange/cli.py
-drwxr-xr-x   0 jhansen    (501) staff       (20)        0 2023-02-15 05:48:25.030723 schemachange-3.5.2/schemachange.egg-info/
--rw-r--r--   0 jhansen    (501) staff       (20)    32235 2023-02-15 05:48:25.000000 schemachange-3.5.2/schemachange.egg-info/PKG-INFO
--rw-r--r--   0 jhansen    (501) staff       (20)      577 2023-02-15 05:48:25.000000 schemachange-3.5.2/schemachange.egg-info/SOURCES.txt
--rw-r--r--   0 jhansen    (501) staff       (20)        1 2023-02-15 05:48:25.000000 schemachange-3.5.2/schemachange.egg-info/dependency_links.txt
--rw-r--r--   0 jhansen    (501) staff       (20)       55 2023-02-15 05:48:25.000000 schemachange-3.5.2/schemachange.egg-info/entry_points.txt
--rw-r--r--   0 jhansen    (501) staff       (20)       82 2023-02-15 05:48:25.000000 schemachange-3.5.2/schemachange.egg-info/requires.txt
--rw-r--r--   0 jhansen    (501) staff       (20)       13 2023-02-15 05:48:25.000000 schemachange-3.5.2/schemachange.egg-info/top_level.txt
--rw-r--r--   0 jhansen    (501) staff       (20)      788 2023-02-15 05:48:25.035764 schemachange-3.5.2/setup.cfg
-drwxr-xr-x   0 jhansen    (501) staff       (20)        0 2023-02-15 05:48:25.034572 schemachange-3.5.2/tests/
--rw-r--r--   0 jhansen    (501) staff       (20)     1419 2023-02-06 19:25:20.000000 schemachange-3.5.2/tests/test_JinjaEnvVar.py
--rw-r--r--   0 jhansen    (501) staff       (20)     1896 2023-02-06 19:25:20.000000 schemachange-3.5.2/tests/test_JinjaTemplateProcessor.py
--rw-r--r--   0 jhansen    (501) staff       (20)     2241 2023-02-06 19:25:20.000000 schemachange-3.5.2/tests/test_SecretManager.py
--rw-r--r--   0 jhansen    (501) staff       (20)     2231 2021-12-01 04:17:40.000000 schemachange-3.5.2/tests/test_extract_config_secrets.py
--rw-r--r--   0 jhansen    (501) staff       (20)    10755 2023-02-06 19:25:20.000000 schemachange-3.5.2/tests/test_get_all_scripts_recursively.py
--rw-r--r--   0 jhansen    (501) staff       (20)     1417 2021-11-09 21:18:31.000000 schemachange-3.5.2/tests/test_jinja_env_var_template.py
--rw-r--r--   0 jhansen    (501) staff       (20)     1988 2023-02-08 23:37:59.000000 schemachange-3.5.2/tests/test_load_schemachange_config.py
--rw-r--r--   0 jhansen    (501) staff       (20)     5555 2023-02-08 23:37:59.000000 schemachange-3.5.2/tests/test_main.py
+drwxr-xr-x   0 jhansen    (501) staff       (20)        0 2023-07-18 22:53:23.950817 schemachange-3.5.3/
+-rw-r--r--   0 jhansen    (501) staff       (20)    11357 2021-10-28 21:28:24.000000 schemachange-3.5.3/LICENSE
+-rw-r--r--   0 jhansen    (501) staff       (20)     1193 2021-10-28 21:28:24.000000 schemachange-3.5.3/NOTICE
+-rw-r--r--   0 jhansen    (501) staff       (20)    32589 2023-07-18 22:53:23.950955 schemachange-3.5.3/PKG-INFO
+-rw-r--r--   0 jhansen    (501) staff       (20)    32007 2023-07-18 22:35:11.000000 schemachange-3.5.3/README.md
+-rw-r--r--   0 jhansen    (501) staff       (20)      106 2021-11-08 20:07:59.000000 schemachange-3.5.3/pyproject.toml
+drwxr-xr-x   0 jhansen    (501) staff       (20)        0 2023-07-18 22:53:23.942693 schemachange-3.5.3/schemachange/
+-rw-r--r--   0 jhansen    (501) staff       (20)        0 2021-10-28 21:28:24.000000 schemachange-3.5.3/schemachange/__init__.py
+-rw-r--r--   0 jhansen    (501) staff       (20)    39070 2023-07-18 21:58:39.000000 schemachange-3.5.3/schemachange/cli.py
+drwxr-xr-x   0 jhansen    (501) staff       (20)        0 2023-07-18 22:53:23.946274 schemachange-3.5.3/schemachange.egg-info/
+-rw-r--r--   0 jhansen    (501) staff       (20)    32589 2023-07-18 22:53:23.000000 schemachange-3.5.3/schemachange.egg-info/PKG-INFO
+-rw-r--r--   0 jhansen    (501) staff       (20)      577 2023-07-18 22:53:23.000000 schemachange-3.5.3/schemachange.egg-info/SOURCES.txt
+-rw-r--r--   0 jhansen    (501) staff       (20)        1 2023-07-18 22:53:23.000000 schemachange-3.5.3/schemachange.egg-info/dependency_links.txt
+-rw-r--r--   0 jhansen    (501) staff       (20)       55 2023-07-18 22:53:23.000000 schemachange-3.5.3/schemachange.egg-info/entry_points.txt
+-rw-r--r--   0 jhansen    (501) staff       (20)       87 2023-07-18 22:53:23.000000 schemachange-3.5.3/schemachange.egg-info/requires.txt
+-rw-r--r--   0 jhansen    (501) staff       (20)       13 2023-07-18 22:53:23.000000 schemachange-3.5.3/schemachange.egg-info/top_level.txt
+-rw-r--r--   0 jhansen    (501) staff       (20)      833 2023-07-18 22:53:23.951584 schemachange-3.5.3/setup.cfg
+drwxr-xr-x   0 jhansen    (501) staff       (20)        0 2023-07-18 22:53:23.950357 schemachange-3.5.3/tests/
+-rw-r--r--   0 jhansen    (501) staff       (20)     1419 2023-02-06 19:25:20.000000 schemachange-3.5.3/tests/test_JinjaEnvVar.py
+-rw-r--r--   0 jhansen    (501) staff       (20)     1896 2023-02-06 19:25:20.000000 schemachange-3.5.3/tests/test_JinjaTemplateProcessor.py
+-rw-r--r--   0 jhansen    (501) staff       (20)     2241 2023-02-06 19:25:20.000000 schemachange-3.5.3/tests/test_SecretManager.py
+-rw-r--r--   0 jhansen    (501) staff       (20)     2231 2021-12-01 04:17:40.000000 schemachange-3.5.3/tests/test_extract_config_secrets.py
+-rw-r--r--   0 jhansen    (501) staff       (20)    10755 2023-02-06 19:25:20.000000 schemachange-3.5.3/tests/test_get_all_scripts_recursively.py
+-rw-r--r--   0 jhansen    (501) staff       (20)     1417 2021-11-09 21:18:31.000000 schemachange-3.5.3/tests/test_jinja_env_var_template.py
+-rw-r--r--   0 jhansen    (501) staff       (20)     1988 2023-02-08 23:37:59.000000 schemachange-3.5.3/tests/test_load_schemachange_config.py
+-rw-r--r--   0 jhansen    (501) staff       (20)     5555 2023-02-08 23:37:59.000000 schemachange-3.5.3/tests/test_main.py
```

### Comparing `schemachange-3.5.2/LICENSE` & `schemachange-3.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `schemachange-3.5.2/NOTICE` & `schemachange-3.5.3/NOTICE`

 * *Files identical despite different names*

### Comparing `schemachange-3.5.2/PKG-INFO` & `schemachange-3.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: schemachange
-Version: 3.5.2
+Version: 3.5.3
 Summary: A Database Change Management tool for Snowflake
 Home-page: https://github.com/Snowflake-Labs/schemachange
 Author: jamesweakley/jeremiahhansen
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 License-File: NOTICE
 
@@ -38,14 +39,15 @@
    1. [Versioned Script Naming](#versioned-script-naming)
    1. [Repeatable Script Naming](#repeatable-script-naming)
    1. [Always Script Naming](#always-script-naming)
    1. [Script Requirements](#script-requirements)
    1. [Using Variables in Scripts](#using-variables-in-scripts)
       1. [Secrets filtering](#secrets-filtering)
    1. [Jinja templating engine](#jinja-templating-engine)
+   1. [Gotchas](#gotchas)
 1. [Change History Table](#change-history-table)
 1. [Authentication](#authentication)
    1. [Password Authentication](#password-authentication)
    1. [Private Key Authentication](#private-key-authentication)
    1. [Oauth Authentication](#oauth-authentication)
    1. [External Browser Authentication](#external-browser-authentication)
    1. [Okta Authentication](#okta-authentication)
@@ -181,14 +183,20 @@
 ### Jinja templating engine
 schemachange uses the Jinja templating engine internally and supports: [expressions](https://jinja.palletsprojects.com/en/3.0.x/templates/#expressions), [macros](https://jinja.palletsprojects.com/en/3.0.x/templates/#macros), [includes](https://jinja.palletsprojects.com/en/3.0.x/templates/#include) and [template inheritance](https://jinja.palletsprojects.com/en/3.0.x/templates/#template-inheritance).
 
 These files can be stored in the root-folder but schemachange also provides a separate modules folder `--modules-folder`. This allows common logic to be stored outside of the main changes scripts. The [demo/citibike_jinja](demo/citibike_jinja) has a simple example that demonstrates this.
 
 The Jinja autoescaping feature is disabled in schemachange, this feature in Jinja is currently designed for where the output language is HTML/XML. So if you are using schemachange with untrusted inputs you will need to handle this within your change scripts.
 
+### Gotchas
+
+Within change scripts:
+- [Snowflake Scripting blocks need delimiters](https://docs.snowflake.com/en/developer-guide/snowflake-scripting/running-examples#introduction)
+- [The last line can't be a comment](https://github.com/Snowflake-Labs/schemachange/issues/130)
+
 ## Change History Table
 
 schemachange records all applied changes scripts to the change history table. By default schemachange will attempt to log all activities to the `METADATA.SCHEMACHANGE.CHANGE_HISTORY` table. The name and location of the change history table can be overriden by using the `-c` (or `--change-history-table`) parameter. The value passed to the parameter can have a one, two, or three part name (e.g. "TABLE_NAME", or "SCHEMA_NAME.TABLE_NAME", or "DATABASE_NAME.SCHEMA_NAME.TABLE_NAME"). This can be used to support multiple environments (dev, test, prod) or multiple subject areas within the same Snowflake account. By default schemachange will not try to create the change history table, and will fail if the table does not exist.
 
 Additionally, if the `--create-change-history-table` parameter is given, then schemachange will attempt to create the schema and table associated with the change history table. schemachange will not attempt to create the database for the change history table, so that must be created ahead of time, even when using the `--create-change-history-table` parameter.
 
 The structure of the `CHANGE_HISTORY` table is as follows:
```

### Comparing `schemachange-3.5.2/README.md` & `schemachange-3.5.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
    1. [Versioned Script Naming](#versioned-script-naming)
    1. [Repeatable Script Naming](#repeatable-script-naming)
    1. [Always Script Naming](#always-script-naming)
    1. [Script Requirements](#script-requirements)
    1. [Using Variables in Scripts](#using-variables-in-scripts)
       1. [Secrets filtering](#secrets-filtering)
    1. [Jinja templating engine](#jinja-templating-engine)
+   1. [Gotchas](#gotchas)
 1. [Change History Table](#change-history-table)
 1. [Authentication](#authentication)
    1. [Password Authentication](#password-authentication)
    1. [Private Key Authentication](#private-key-authentication)
    1. [Oauth Authentication](#oauth-authentication)
    1. [External Browser Authentication](#external-browser-authentication)
    1. [Okta Authentication](#okta-authentication)
@@ -165,14 +166,20 @@
 ### Jinja templating engine
 schemachange uses the Jinja templating engine internally and supports: [expressions](https://jinja.palletsprojects.com/en/3.0.x/templates/#expressions), [macros](https://jinja.palletsprojects.com/en/3.0.x/templates/#macros), [includes](https://jinja.palletsprojects.com/en/3.0.x/templates/#include) and [template inheritance](https://jinja.palletsprojects.com/en/3.0.x/templates/#template-inheritance).
 
 These files can be stored in the root-folder but schemachange also provides a separate modules folder `--modules-folder`. This allows common logic to be stored outside of the main changes scripts. The [demo/citibike_jinja](demo/citibike_jinja) has a simple example that demonstrates this.
 
 The Jinja autoescaping feature is disabled in schemachange, this feature in Jinja is currently designed for where the output language is HTML/XML. So if you are using schemachange with untrusted inputs you will need to handle this within your change scripts.
 
+### Gotchas
+
+Within change scripts:
+- [Snowflake Scripting blocks need delimiters](https://docs.snowflake.com/en/developer-guide/snowflake-scripting/running-examples#introduction)
+- [The last line can't be a comment](https://github.com/Snowflake-Labs/schemachange/issues/130)
+
 ## Change History Table
 
 schemachange records all applied changes scripts to the change history table. By default schemachange will attempt to log all activities to the `METADATA.SCHEMACHANGE.CHANGE_HISTORY` table. The name and location of the change history table can be overriden by using the `-c` (or `--change-history-table`) parameter. The value passed to the parameter can have a one, two, or three part name (e.g. "TABLE_NAME", or "SCHEMA_NAME.TABLE_NAME", or "DATABASE_NAME.SCHEMA_NAME.TABLE_NAME"). This can be used to support multiple environments (dev, test, prod) or multiple subject areas within the same Snowflake account. By default schemachange will not try to create the change history table, and will fail if the table does not exist.
 
 Additionally, if the `--create-change-history-table` parameter is given, then schemachange will attempt to create the schema and table associated with the change history table. schemachange will not attempt to create the database for the change history table, so that must be created ahead of time, even when using the `--create-change-history-table` parameter.
 
 The structure of the `CHANGE_HISTORY` table is as follows:
```

### Comparing `schemachange-3.5.2/schemachange/cli.py` & `schemachange-3.5.3/schemachange/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import serialization
 from jinja2.loaders import BaseLoader
 from pandas import DataFrame
 
 #region Global Variables 
 # metadata
-_schemachange_version = '3.5.2'
+_schemachange_version = '3.5.3'
 _config_file_name = 'schemachange-config.yml'
 _metadata_database_name = 'METADATA'
 _metadata_schema_name = 'SCHEMACHANGE'
 _metadata_table_name = 'CHANGE_HISTORY'
 _snowflake_application_name = 'schemachange'
 
 # messages
```

### Comparing `schemachange-3.5.2/schemachange.egg-info/PKG-INFO` & `schemachange-3.5.3/schemachange.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: schemachange
-Version: 3.5.2
+Version: 3.5.3
 Summary: A Database Change Management tool for Snowflake
 Home-page: https://github.com/Snowflake-Labs/schemachange
 Author: jamesweakley/jeremiahhansen
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 License-File: NOTICE
 
@@ -38,14 +39,15 @@
    1. [Versioned Script Naming](#versioned-script-naming)
    1. [Repeatable Script Naming](#repeatable-script-naming)
    1. [Always Script Naming](#always-script-naming)
    1. [Script Requirements](#script-requirements)
    1. [Using Variables in Scripts](#using-variables-in-scripts)
       1. [Secrets filtering](#secrets-filtering)
    1. [Jinja templating engine](#jinja-templating-engine)
+   1. [Gotchas](#gotchas)
 1. [Change History Table](#change-history-table)
 1. [Authentication](#authentication)
    1. [Password Authentication](#password-authentication)
    1. [Private Key Authentication](#private-key-authentication)
    1. [Oauth Authentication](#oauth-authentication)
    1. [External Browser Authentication](#external-browser-authentication)
    1. [Okta Authentication](#okta-authentication)
@@ -181,14 +183,20 @@
 ### Jinja templating engine
 schemachange uses the Jinja templating engine internally and supports: [expressions](https://jinja.palletsprojects.com/en/3.0.x/templates/#expressions), [macros](https://jinja.palletsprojects.com/en/3.0.x/templates/#macros), [includes](https://jinja.palletsprojects.com/en/3.0.x/templates/#include) and [template inheritance](https://jinja.palletsprojects.com/en/3.0.x/templates/#template-inheritance).
 
 These files can be stored in the root-folder but schemachange also provides a separate modules folder `--modules-folder`. This allows common logic to be stored outside of the main changes scripts. The [demo/citibike_jinja](demo/citibike_jinja) has a simple example that demonstrates this.
 
 The Jinja autoescaping feature is disabled in schemachange, this feature in Jinja is currently designed for where the output language is HTML/XML. So if you are using schemachange with untrusted inputs you will need to handle this within your change scripts.
 
+### Gotchas
+
+Within change scripts:
+- [Snowflake Scripting blocks need delimiters](https://docs.snowflake.com/en/developer-guide/snowflake-scripting/running-examples#introduction)
+- [The last line can't be a comment](https://github.com/Snowflake-Labs/schemachange/issues/130)
+
 ## Change History Table
 
 schemachange records all applied changes scripts to the change history table. By default schemachange will attempt to log all activities to the `METADATA.SCHEMACHANGE.CHANGE_HISTORY` table. The name and location of the change history table can be overriden by using the `-c` (or `--change-history-table`) parameter. The value passed to the parameter can have a one, two, or three part name (e.g. "TABLE_NAME", or "SCHEMA_NAME.TABLE_NAME", or "DATABASE_NAME.SCHEMA_NAME.TABLE_NAME"). This can be used to support multiple environments (dev, test, prod) or multiple subject areas within the same Snowflake account. By default schemachange will not try to create the change history table, and will fail if the table does not exist.
 
 Additionally, if the `--create-change-history-table` parameter is given, then schemachange will attempt to create the schema and table associated with the change history table. schemachange will not attempt to create the database for the change history table, so that must be created ahead of time, even when using the `--create-change-history-table` parameter.
 
 The structure of the `CHANGE_HISTORY` table is as follows:
```

### Comparing `schemachange-3.5.2/schemachange.egg-info/SOURCES.txt` & `schemachange-3.5.3/schemachange.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `schemachange-3.5.2/setup.cfg` & `schemachange-3.5.3/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [metadata]
 name = schemachange
-version = 3.5.2
+version = 3.5.3
 author = jamesweakley/jeremiahhansen
 description = A Database Change Management tool for Snowflake
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Snowflake-Labs/schemachange
 classifiers = 
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
 	Operating System :: OS Independent
 
 [options]
 packages = schemachange
 python_requires = >=3.7
 install_requires = 
-	snowflake-connector-python~=2.8
+	snowflake-connector-python>=2.8,<4.0
 	pandas~=1.3
-	pyyaml~=5.4
+	pyyaml~=6.0
 	jinja2~=3.0
 include_package_data = True
 
 [options.entry_points]
 console_scripts = 
 	schemachange = schemachange.cli:main
```

### Comparing `schemachange-3.5.2/tests/test_JinjaEnvVar.py` & `schemachange-3.5.3/tests/test_JinjaEnvVar.py`

 * *Files identical despite different names*

### Comparing `schemachange-3.5.2/tests/test_JinjaTemplateProcessor.py` & `schemachange-3.5.3/tests/test_JinjaTemplateProcessor.py`

 * *Files identical despite different names*

### Comparing `schemachange-3.5.2/tests/test_SecretManager.py` & `schemachange-3.5.3/tests/test_SecretManager.py`

 * *Files identical despite different names*

### Comparing `schemachange-3.5.2/tests/test_extract_config_secrets.py` & `schemachange-3.5.3/tests/test_extract_config_secrets.py`

 * *Files identical despite different names*

### Comparing `schemachange-3.5.2/tests/test_get_all_scripts_recursively.py` & `schemachange-3.5.3/tests/test_get_all_scripts_recursively.py`

 * *Files identical despite different names*

### Comparing `schemachange-3.5.2/tests/test_jinja_env_var_template.py` & `schemachange-3.5.3/tests/test_jinja_env_var_template.py`

 * *Files identical despite different names*

### Comparing `schemachange-3.5.2/tests/test_load_schemachange_config.py` & `schemachange-3.5.3/tests/test_load_schemachange_config.py`

 * *Files identical despite different names*

### Comparing `schemachange-3.5.2/tests/test_main.py` & `schemachange-3.5.3/tests/test_main.py`

 * *Files identical despite different names*

