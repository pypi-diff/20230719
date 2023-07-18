# Comparing `tmp/mlservicewrapper-plugin-application-insights-0.1.2.tar.gz` & `tmp/mlservicewrapper-plugin-application-insights-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlservicewrapper-plugin-application-insights-0.1.2.tar", last modified: Tue May 11 17:07:56 2021, max compression
+gzip compressed data, was "mlservicewrapper-plugin-application-insights-0.2.0.tar", last modified: Tue Jul 18 22:02:48 2023, max compression
```

## Comparing `mlservicewrapper-plugin-application-insights-0.1.2.tar` & `mlservicewrapper-plugin-application-insights-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-11 17:07:56.258442 mlservicewrapper-plugin-application-insights-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-11 17:07:56.254442 mlservicewrapper-plugin-application-insights-0.1.2/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      501 2021-05-11 17:07:46.000000 mlservicewrapper-plugin-application-insights-0.1.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-11 17:07:56.254442 mlservicewrapper-plugin-application-insights-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2238 2021-05-11 17:07:46.000000 mlservicewrapper-plugin-application-insights-0.1.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1799 2021-05-11 17:07:46.000000 mlservicewrapper-plugin-application-insights-0.1.2/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-11 17:07:56.258442 mlservicewrapper-plugin-application-insights-0.1.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (121)      283 2021-05-11 17:07:46.000000 mlservicewrapper-plugin-application-insights-0.1.2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2021-05-11 17:07:46.000000 mlservicewrapper-plugin-application-insights-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      515 2021-05-11 17:07:56.258442 mlservicewrapper-plugin-application-insights-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       60 2021-05-11 17:07:46.000000 mlservicewrapper-plugin-application-insights-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      106 2021-05-11 17:07:46.000000 mlservicewrapper-plugin-application-insights-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       97 2021-05-11 17:07:46.000000 mlservicewrapper-plugin-application-insights-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-05-11 17:07:56.258442 mlservicewrapper-plugin-application-insights-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      990 2021-05-11 17:07:46.000000 mlservicewrapper-plugin-application-insights-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-11 17:07:56.254442 mlservicewrapper-plugin-application-insights-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-11 17:07:56.254442 mlservicewrapper-plugin-application-insights-0.1.2/src/mlservicewrapper/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-11 17:07:56.254442 mlservicewrapper-plugin-application-insights-0.1.2/src/mlservicewrapper/plugin/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-11 17:07:56.258442 mlservicewrapper-plugin-application-insights-0.1.2/src/mlservicewrapper/plugin/application_insights/
--rw-r--r--   0 runner    (1001) docker     (121)     2602 2021-05-11 17:07:46.000000 mlservicewrapper-plugin-application-insights-0.1.2/src/mlservicewrapper/plugin/application_insights/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-11 17:07:56.258442 mlservicewrapper-plugin-application-insights-0.1.2/src/mlservicewrapper_plugin_application_insights.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      515 2021-05-11 17:07:55.000000 mlservicewrapper-plugin-application-insights-0.1.2/src/mlservicewrapper_plugin_application_insights.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      635 2021-05-11 17:07:56.000000 mlservicewrapper-plugin-application-insights-0.1.2/src/mlservicewrapper_plugin_application_insights.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-11 17:07:55.000000 mlservicewrapper-plugin-application-insights-0.1.2/src/mlservicewrapper_plugin_application_insights.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-11 17:07:55.000000 mlservicewrapper-plugin-application-insights-0.1.2/src/mlservicewrapper_plugin_application_insights.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       97 2021-05-11 17:07:55.000000 mlservicewrapper-plugin-application-insights-0.1.2/src/mlservicewrapper_plugin_application_insights.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2021-05-11 17:07:55.000000 mlservicewrapper-plugin-application-insights-0.1.2/src/mlservicewrapper_plugin_application_insights.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:02:48.148638 mlservicewrapper-plugin-application-insights-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:02:48.144638 mlservicewrapper-plugin-application-insights-0.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-18 22:02:34.000000 mlservicewrapper-plugin-application-insights-0.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:02:48.144638 mlservicewrapper-plugin-application-insights-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-07-18 22:02:34.000000 mlservicewrapper-plugin-application-insights-0.2.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-18 22:02:34.000000 mlservicewrapper-plugin-application-insights-0.2.0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:02:48.144638 mlservicewrapper-plugin-application-insights-0.2.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-18 22:02:34.000000 mlservicewrapper-plugin-application-insights-0.2.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-18 22:02:34.000000 mlservicewrapper-plugin-application-insights-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-18 22:02:48.148638 mlservicewrapper-plugin-application-insights-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-18 22:02:34.000000 mlservicewrapper-plugin-application-insights-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-18 22:02:34.000000 mlservicewrapper-plugin-application-insights-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-18 22:02:34.000000 mlservicewrapper-plugin-application-insights-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 22:02:48.148638 mlservicewrapper-plugin-application-insights-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-18 22:02:34.000000 mlservicewrapper-plugin-application-insights-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:02:48.144638 mlservicewrapper-plugin-application-insights-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:02:48.144638 mlservicewrapper-plugin-application-insights-0.2.0/src/mlservicewrapper/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:02:48.144638 mlservicewrapper-plugin-application-insights-0.2.0/src/mlservicewrapper/plugin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:02:48.144638 mlservicewrapper-plugin-application-insights-0.2.0/src/mlservicewrapper/plugin/application_insights/
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-07-18 22:02:34.000000 mlservicewrapper-plugin-application-insights-0.2.0/src/mlservicewrapper/plugin/application_insights/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:02:48.148638 mlservicewrapper-plugin-application-insights-0.2.0/src/mlservicewrapper_plugin_application_insights.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-18 22:02:48.000000 mlservicewrapper-plugin-application-insights-0.2.0/src/mlservicewrapper_plugin_application_insights.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-18 22:02:48.000000 mlservicewrapper-plugin-application-insights-0.2.0/src/mlservicewrapper_plugin_application_insights.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 22:02:48.000000 mlservicewrapper-plugin-application-insights-0.2.0/src/mlservicewrapper_plugin_application_insights.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 22:02:48.000000 mlservicewrapper-plugin-application-insights-0.2.0/src/mlservicewrapper_plugin_application_insights.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-18 22:02:48.000000 mlservicewrapper-plugin-application-insights-0.2.0/src/mlservicewrapper_plugin_application_insights.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-18 22:02:48.000000 mlservicewrapper-plugin-application-insights-0.2.0/src/mlservicewrapper_plugin_application_insights.egg-info/top_level.txt
```

### Comparing `mlservicewrapper-plugin-application-insights-0.1.2/.github/workflows/release.yml` & `mlservicewrapper-plugin-application-insights-0.2.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `mlservicewrapper-plugin-application-insights-0.1.2/.gitignore` & `mlservicewrapper-plugin-application-insights-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mlservicewrapper-plugin-application-insights-0.1.2/LICENSE` & `mlservicewrapper-plugin-application-insights-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mlservicewrapper-plugin-application-insights-0.1.2/setup.py` & `mlservicewrapper-plugin-application-insights-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `mlservicewrapper-plugin-application-insights-0.1.2/src/mlservicewrapper/plugin/application_insights/__init__.py` & `mlservicewrapper-plugin-application-insights-0.2.0/src/mlservicewrapper/plugin/application_insights/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 
 import logging
+import os
 
 from mlservicewrapper.core import contexts, server, services
 from opencensus.ext.azure import metrics_exporter
 from opencensus.ext.azure.log_exporter import AzureLogHandler
 from opencensus.ext.azure.trace_exporter import AzureExporter
 from opencensus.trace import config_integration
 from opencensus.trace.samplers import AlwaysOnSampler
@@ -26,15 +27,18 @@
         
         logger.addHandler(self.__azure_handler)
 
     async def load(self, ctx: contexts.ServiceContext):
 
         config_integration.trace_integrations(['logging'])
 
-        connection_string = ctx.get_parameter_value("ApplicationInsightsConnectionString", required=False)
+        connection_string = os.environ.get("APPLICATIONINSIGHTS_CONNECTION_STRING")
+        
+        if connection_string is None:
+            connection_string = ctx.get_parameter_value("ApplicationInsightsConnectionString", required=False)
 
         if connection_string is None:
             logging.warn("Application Insights is not enabled, set the ApplicationInsightsConnectionString parameter to capture logs.")
 
             self.__azure_handler = None
         else:
             self.__azure_handler = AzureLogHandler(connection_string=connection_string)
```

### Comparing `mlservicewrapper-plugin-application-insights-0.1.2/src/mlservicewrapper_plugin_application_insights.egg-info/SOURCES.txt` & `mlservicewrapper-plugin-application-insights-0.2.0/src/mlservicewrapper_plugin_application_insights.egg-info/SOURCES.txt`

 * *Files identical despite different names*

