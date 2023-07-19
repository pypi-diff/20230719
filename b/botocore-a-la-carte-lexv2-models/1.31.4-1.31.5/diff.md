# Comparing `tmp/botocore-a-la-carte-lexv2-models-1.31.4.tar.gz` & `tmp/botocore-a-la-carte-lexv2-models-1.31.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-lexv2-models-1.31.4.tar", last modified: Tue Jul 18 01:55:21 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-lexv2-models-1.31.5.tar", last modified: Wed Jul 19 02:44:02 2023, max compression
```

## Comparing `botocore-a-la-carte-lexv2-models-1.31.4.tar` & `botocore-a-la-carte-lexv2-models-1.31.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:55:21.368269 botocore-a-la-carte-lexv2-models-1.31.4/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-18 01:55:21.000000 botocore-a-la-carte-lexv2-models-1.31.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-18 01:55:21.368269 botocore-a-la-carte-lexv2-models-1.31.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:55:21.368269 botocore-a-la-carte-lexv2-models-1.31.4/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:55:21.368269 botocore-a-la-carte-lexv2-models-1.31.4/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:55:21.368269 botocore-a-la-carte-lexv2-models-1.31.4/botocore/data/lexv2-models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:55:21.368269 botocore-a-la-carte-lexv2-models-1.31.4/botocore/data/lexv2-models/2020-08-07/
--rw-r--r--   0 runner    (1001) docker     (123)    17652 2023-07-18 01:54:50.000000 botocore-a-la-carte-lexv2-models-1.31.4/botocore/data/lexv2-models/2020-08-07/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-18 01:54:50.000000 botocore-a-la-carte-lexv2-models-1.31.4/botocore/data/lexv2-models/2020-08-07/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-18 01:54:50.000000 botocore-a-la-carte-lexv2-models-1.31.4/botocore/data/lexv2-models/2020-08-07/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   492607 2023-07-18 01:54:50.000000 botocore-a-la-carte-lexv2-models-1.31.4/botocore/data/lexv2-models/2020-08-07/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     7231 2023-07-18 01:54:50.000000 botocore-a-la-carte-lexv2-models-1.31.4/botocore/data/lexv2-models/2020-08-07/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 01:55:21.368269 botocore-a-la-carte-lexv2-models-1.31.4/botocore_a_la_carte_lexv2_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-18 01:55:21.000000 botocore-a-la-carte-lexv2-models-1.31.4/botocore_a_la_carte_lexv2_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-18 01:55:21.000000 botocore-a-la-carte-lexv2-models-1.31.4/botocore_a_la_carte_lexv2_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 01:55:21.000000 botocore-a-la-carte-lexv2-models-1.31.4/botocore_a_la_carte_lexv2_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-18 01:55:21.000000 botocore-a-la-carte-lexv2-models-1.31.4/botocore_a_la_carte_lexv2_models.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 01:55:21.368269 botocore-a-la-carte-lexv2-models-1.31.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-18 01:55:21.000000 botocore-a-la-carte-lexv2-models-1.31.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:44:02.423577 botocore-a-la-carte-lexv2-models-1.31.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-19 02:44:02.000000 botocore-a-la-carte-lexv2-models-1.31.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-19 02:44:02.423577 botocore-a-la-carte-lexv2-models-1.31.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:44:02.419577 botocore-a-la-carte-lexv2-models-1.31.5/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:44:02.419577 botocore-a-la-carte-lexv2-models-1.31.5/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:44:02.419577 botocore-a-la-carte-lexv2-models-1.31.5/botocore/data/lexv2-models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:44:02.419577 botocore-a-la-carte-lexv2-models-1.31.5/botocore/data/lexv2-models/2020-08-07/
+-rw-r--r--   0 runner    (1001) docker     (123)    17652 2023-07-19 02:43:32.000000 botocore-a-la-carte-lexv2-models-1.31.5/botocore/data/lexv2-models/2020-08-07/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-19 02:43:32.000000 botocore-a-la-carte-lexv2-models-1.31.5/botocore/data/lexv2-models/2020-08-07/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-19 02:43:32.000000 botocore-a-la-carte-lexv2-models-1.31.5/botocore/data/lexv2-models/2020-08-07/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   594234 2023-07-19 02:43:32.000000 botocore-a-la-carte-lexv2-models-1.31.5/botocore/data/lexv2-models/2020-08-07/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7231 2023-07-19 02:43:32.000000 botocore-a-la-carte-lexv2-models-1.31.5/botocore/data/lexv2-models/2020-08-07/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 02:44:02.419577 botocore-a-la-carte-lexv2-models-1.31.5/botocore_a_la_carte_lexv2_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-19 02:44:02.000000 botocore-a-la-carte-lexv2-models-1.31.5/botocore_a_la_carte_lexv2_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-19 02:44:02.000000 botocore-a-la-carte-lexv2-models-1.31.5/botocore_a_la_carte_lexv2_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 02:44:02.000000 botocore-a-la-carte-lexv2-models-1.31.5/botocore_a_la_carte_lexv2_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-19 02:44:02.000000 botocore-a-la-carte-lexv2-models-1.31.5/botocore_a_la_carte_lexv2_models.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 02:44:02.423577 botocore-a-la-carte-lexv2-models-1.31.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-19 02:44:02.000000 botocore-a-la-carte-lexv2-models-1.31.5/setup.py
```

### Comparing `botocore-a-la-carte-lexv2-models-1.31.4/LICENSE.txt` & `botocore-a-la-carte-lexv2-models-1.31.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-lexv2-models-1.31.4/PKG-INFO` & `botocore-a-la-carte-lexv2-models-1.31.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-lexv2-models
-Version: 1.31.4
+Version: 1.31.5
 Summary: lexv2-models data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-lexv2-models-1.31.4/botocore/data/lexv2-models/2020-08-07/endpoint-rule-set-1.json` & `botocore-a-la-carte-lexv2-models-1.31.5/botocore/data/lexv2-models/2020-08-07/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-lexv2-models-1.31.4/botocore/data/lexv2-models/2020-08-07/service-2.json` & `botocore-a-la-carte-lexv2-models-1.31.5/botocore/data/lexv2-models/2020-08-07/service-2.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975991304347826%*

 * *Differences: {"'operations'": "{'ListIntentMetrics': OrderedDict([('name', 'ListIntentMetrics'), ('http', "*

 * *                 "OrderedDict([('method', 'POST'), ('requestUri', "*

 * *                 "'/bots/{botId}/analytics/intentmetrics'), ('responseCode', 200)])), ('input', "*

 * *                 "OrderedDict([('shape', 'ListIntentMetricsRequest')])), ('output', "*

 * *                 "OrderedDict([('shape', 'ListIntentMetricsResponse')])), ('errors', "*

 * *                 "[OrderedDict([('shape', 'ThrottlingException')]), OrderedDic […]*

```diff
@@ -1857,14 +1857,110 @@
                 "shape": "ListImportsRequest"
             },
             "name": "ListImports",
             "output": {
                 "shape": "ListImportsResponse"
             }
         },
+        "ListIntentMetrics": {
+            "documentation": "<p>Retrieves summary metrics for the intents in your bot. The following fields are required:</p> <ul> <li> <p> <code>metrics</code> \u2013 A list of <a href=\"https://docs.aws.amazon.com/lexv2/latest/APIReference/API_AnalyticsIntentMetric.html\">AnalyticsIntentMetric</a> objects. In each object, use the <code>name</code> field to specify the metric to calculate, the <code>statistic</code> field to specify whether to calculate the <code>Sum</code>, <code>Average</code>, or <code>Max</code> number, and the <code>order</code> field to specify whether to sort the results in <code>Ascending</code> or <code>Descending</code> order.</p> </li> <li> <p> <code>startDateTime</code> and <code>endDateTime</code> \u2013 Define a time range for which you want to retrieve results.</p> </li> </ul> <p>Of the optional fields, you can organize the results in the following ways:</p> <ul> <li> <p>Use the <code>filters</code> field to filter the results, the <code>groupBy</code> field to specify categories by which to group the results, and the <code>binBy</code> field to specify time intervals by which to group the results.</p> </li> <li> <p>Use the <code>maxResults</code> field to limit the number of results to return in a single response and the <code>nextToken</code> field to return the next batch of results if the response does not return the full set of results.</p> </li> </ul> <p>Note that an <code>order</code> field exists in both <code>binBy</code> and <code>metrics</code>. You can specify only one <code>order</code> in a given request.</p>",
+            "errors": [
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "ValidationException"
+                },
+                {
+                    "shape": "PreconditionFailedException"
+                },
+                {
+                    "shape": "ServiceQuotaExceededException"
+                },
+                {
+                    "shape": "InternalServerException"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/bots/{botId}/analytics/intentmetrics",
+                "responseCode": 200
+            },
+            "input": {
+                "shape": "ListIntentMetricsRequest"
+            },
+            "name": "ListIntentMetrics",
+            "output": {
+                "shape": "ListIntentMetricsResponse"
+            }
+        },
+        "ListIntentPaths": {
+            "documentation": "<p>Retrieves summary statistics for a path of intents that users take over sessions with your bot. The following fields are required:</p> <ul> <li> <p> <code>startDateTime</code> and <code>endDateTime</code> \u2013 Define a time range for which you want to retrieve results.</p> </li> <li> <p> <code>intentPath</code> \u2013 Define an order of intents for which you want to retrieve metrics. Separate intents in the path with a forward slash. For example, populate the <code>intentPath</code> field with <code>/BookCar/BookHotel</code> to see details about how many times users invoked the <code>BookCar</code> and <code>BookHotel</code> intents in that order.</p> </li> </ul> <p>Use the optional <code>filters</code> field to filter the results.</p>",
+            "errors": [
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "ValidationException"
+                },
+                {
+                    "shape": "PreconditionFailedException"
+                },
+                {
+                    "shape": "ServiceQuotaExceededException"
+                },
+                {
+                    "shape": "InternalServerException"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/bots/{botId}/analytics/intentpaths",
+                "responseCode": 200
+            },
+            "input": {
+                "shape": "ListIntentPathsRequest"
+            },
+            "name": "ListIntentPaths",
+            "output": {
+                "shape": "ListIntentPathsResponse"
+            }
+        },
+        "ListIntentStageMetrics": {
+            "documentation": "<p>Retrieves summary metrics for the intent stages in your bot. The following fields are required:</p> <ul> <li> <p> <code>metrics</code> \u2013 A list of <a href=\"https://docs.aws.amazon.com/lexv2/latest/APIReference/API_AnalyticsIntentStageMetric.html\">AnalyticsIntentStageMetric</a> objects. In each object, use the <code>name</code> field to specify the metric to calculate, the <code>statistic</code> field to specify whether to calculate the <code>Sum</code>, <code>Average</code>, or <code>Max</code> number, and the <code>order</code> field to specify whether to sort the results in <code>Ascending</code> or <code>Descending</code> order.</p> </li> <li> <p> <code>startDateTime</code> and <code>endDateTime</code> \u2013 Define a time range for which you want to retrieve results.</p> </li> </ul> <p>Of the optional fields, you can organize the results in the following ways:</p> <ul> <li> <p>Use the <code>filters</code> field to filter the results, the <code>groupBy</code> field to specify categories by which to group the results, and the <code>binBy</code> field to specify time intervals by which to group the results.</p> </li> <li> <p>Use the <code>maxResults</code> field to limit the number of results to return in a single response and the <code>nextToken</code> field to return the next batch of results if the response does not return the full set of results.</p> </li> </ul> <p>Note that an <code>order</code> field exists in both <code>binBy</code> and <code>metrics</code>. You can only specify one <code>order</code> in a given request.</p>",
+            "errors": [
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "ValidationException"
+                },
+                {
+                    "shape": "PreconditionFailedException"
+                },
+                {
+                    "shape": "ServiceQuotaExceededException"
+                },
+                {
+                    "shape": "InternalServerException"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/bots/{botId}/analytics/intentstagemetrics",
+                "responseCode": 200
+            },
+            "input": {
+                "shape": "ListIntentStageMetricsRequest"
+            },
+            "name": "ListIntentStageMetrics",
+            "output": {
+                "shape": "ListIntentStageMetricsResponse"
+            }
+        },
         "ListIntents": {
             "documentation": "<p>Get a list of intents that meet the specified criteria.</p>",
             "errors": [
                 {
                     "shape": "ThrottlingException"
                 },
                 {
@@ -1918,14 +2014,78 @@
                 "shape": "ListRecommendedIntentsRequest"
             },
             "name": "ListRecommendedIntents",
             "output": {
                 "shape": "ListRecommendedIntentsResponse"
             }
         },
+        "ListSessionAnalyticsData": {
+            "documentation": "<p>Retrieves a list of metadata for individual user sessions with your bot. The <code>startDateTime</code> and <code>endDateTime</code> fields are required. These fields define a time range for which you want to retrieve results. Of the optional fields, you can organize the results in the following ways:</p> <ul> <li> <p>Use the <code>filters</code> field to filter the results and the <code>sortBy</code> field to specify the values by which to sort the results.</p> </li> <li> <p>Use the <code>maxResults</code> field to limit the number of results to return in a single response and the <code>nextToken</code> field to return the next batch of results if the response does not return the full set of results.</p> </li> </ul>",
+            "errors": [
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "ValidationException"
+                },
+                {
+                    "shape": "PreconditionFailedException"
+                },
+                {
+                    "shape": "ServiceQuotaExceededException"
+                },
+                {
+                    "shape": "InternalServerException"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/bots/{botId}/analytics/sessions",
+                "responseCode": 200
+            },
+            "input": {
+                "shape": "ListSessionAnalyticsDataRequest"
+            },
+            "name": "ListSessionAnalyticsData",
+            "output": {
+                "shape": "ListSessionAnalyticsDataResponse"
+            }
+        },
+        "ListSessionMetrics": {
+            "documentation": "<p>Retrieves summary metrics for the user sessions with your bot. The following fields are required:</p> <ul> <li> <p> <code>metrics</code> \u2013 A list of <a href=\"https://docs.aws.amazon.com/lexv2/latest/APIReference/API_AnalyticsSessionMetric.html\">AnalyticsSessionMetric</a> objects. In each object, use the <code>name</code> field to specify the metric to calculate, the <code>statistic</code> field to specify whether to calculate the <code>Sum</code>, <code>Average</code>, or <code>Max</code> number, and the <code>order</code> field to specify whether to sort the results in <code>Ascending</code> or <code>Descending</code> order.</p> </li> <li> <p> <code>startDateTime</code> and <code>endDateTime</code> \u2013 Define a time range for which you want to retrieve results.</p> </li> </ul> <p>Of the optional fields, you can organize the results in the following ways:</p> <ul> <li> <p>Use the <code>filters</code> field to filter the results, the <code>groupBy</code> field to specify categories by which to group the results, and the <code>binBy</code> field to specify time intervals by which to group the results.</p> </li> <li> <p>Use the <code>maxResults</code> field to limit the number of results to return in a single response and the <code>nextToken</code> field to return the next batch of results if the response does not return the full set of results.</p> </li> </ul> <p>Note that an <code>order</code> field exists in both <code>binBy</code> and <code>metrics</code>. Currently, you can specify it in either field, but not in both.</p>",
+            "errors": [
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "ValidationException"
+                },
+                {
+                    "shape": "PreconditionFailedException"
+                },
+                {
+                    "shape": "ServiceQuotaExceededException"
+                },
+                {
+                    "shape": "InternalServerException"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/bots/{botId}/analytics/sessionmetrics",
+                "responseCode": 200
+            },
+            "input": {
+                "shape": "ListSessionMetricsRequest"
+            },
+            "name": "ListSessionMetrics",
+            "output": {
+                "shape": "ListSessionMetricsResponse"
+            }
+        },
         "ListSlotTypes": {
             "documentation": "<p>Gets a list of slot types that match the specified criteria.</p>",
             "errors": [
                 {
                     "shape": "ThrottlingException"
                 },
                 {
@@ -2127,14 +2287,78 @@
                 "shape": "ListTestSetsRequest"
             },
             "name": "ListTestSets",
             "output": {
                 "shape": "ListTestSetsResponse"
             }
         },
+        "ListUtteranceAnalyticsData": {
+            "documentation": "<p>Retrieves a list of metadata for individual user utterances to your bot. The <code>startDateTime</code> and <code>endDateTime</code> fields are required. These fields define a time range for which you want to retrieve results. Of the optional fields, you can organize the results in the following ways:</p> <ul> <li> <p>Use the <code>filters</code> field to filter the results and the <code>sortBy</code> field to specify the values by which to sort the results.</p> </li> <li> <p>Use the <code>maxResults</code> field to limit the number of results to return in a single response and the <code>nextToken</code> field to return the next batch of results if the response does not return the full set of results.</p> </li> </ul>",
+            "errors": [
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "ValidationException"
+                },
+                {
+                    "shape": "PreconditionFailedException"
+                },
+                {
+                    "shape": "ServiceQuotaExceededException"
+                },
+                {
+                    "shape": "InternalServerException"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/bots/{botId}/analytics/utterances",
+                "responseCode": 200
+            },
+            "input": {
+                "shape": "ListUtteranceAnalyticsDataRequest"
+            },
+            "name": "ListUtteranceAnalyticsData",
+            "output": {
+                "shape": "ListUtteranceAnalyticsDataResponse"
+            }
+        },
+        "ListUtteranceMetrics": {
+            "documentation": "<p>Retrieves summary metrics for the utterances in your bot. The following fields are required:</p> <ul> <li> <p> <code>metrics</code> \u2013 A list of <a href=\"https://docs.aws.amazon.com/lexv2/latest/APIReference/API_AnalyticsUtteranceMetric.html\">AnalyticsUtteranceMetric</a> objects. In each object, use the <code>name</code> field to specify the metric to calculate, the <code>statistic</code> field to specify whether to calculate the <code>Sum</code>, <code>Average</code>, or <code>Max</code> number, and the <code>order</code> field to specify whether to sort the results in <code>Ascending</code> or <code>Descending</code> order.</p> </li> <li> <p> <code>startDateTime</code> and <code>endDateTime</code> \u2013 Define a time range for which you want to retrieve results.</p> </li> </ul> <p>Of the optional fields, you can organize the results in the following ways:</p> <ul> <li> <p>Use the <code>filters</code> field to filter the results, the <code>groupBy</code> field to specify categories by which to group the results, and the <code>binBy</code> field to specify time intervals by which to group the results.</p> </li> <li> <p>Use the <code>maxResults</code> field to limit the number of results to return in a single response and the <code>nextToken</code> field to return the next batch of results if the response does not return the full set of results.</p> </li> </ul> <p>Note that an <code>order</code> field exists in both <code>binBy</code> and <code>metrics</code>. Currently, you can specify it in either field, but not in both.</p>",
+            "errors": [
+                {
+                    "shape": "ThrottlingException"
+                },
+                {
+                    "shape": "ValidationException"
+                },
+                {
+                    "shape": "PreconditionFailedException"
+                },
+                {
+                    "shape": "ServiceQuotaExceededException"
+                },
+                {
+                    "shape": "InternalServerException"
+                }
+            ],
+            "http": {
+                "method": "POST",
+                "requestUri": "/bots/{botId}/analytics/utterancemetrics",
+                "responseCode": 200
+            },
+            "input": {
+                "shape": "ListUtteranceMetricsRequest"
+            },
+            "name": "ListUtteranceMetrics",
+            "output": {
+                "shape": "ListUtteranceMetricsResponse"
+            }
+        },
         "SearchAssociatedTranscripts": {
             "documentation": "<p>Search for associated transcripts that meet the specified criteria.</p>",
             "errors": [
                 {
                     "shape": "ThrottlingException"
                 },
                 {
@@ -2970,14 +3194,1025 @@
             "type": "structure"
         },
         "AmazonResourceName": {
             "max": 1011,
             "min": 1,
             "type": "string"
         },
+        "AnalyticsBinByList": {
+            "max": 1,
+            "member": {
+                "shape": "AnalyticsBinBySpecification"
+            },
+            "min": 1,
+            "type": "list"
+        },
+        "AnalyticsBinByName": {
+            "enum": [
+                "ConversationStartTime",
+                "UtteranceTimestamp"
+            ],
+            "type": "string"
+        },
+        "AnalyticsBinBySpecification": {
+            "documentation": "<p>Contains the time metric, interval, and method by which to bin the analytics data.</p>",
+            "members": {
+                "interval": {
+                    "documentation": "<p>Specifies the interval of time by which to bin the analytics data.</p>",
+                    "shape": "AnalyticsInterval"
+                },
+                "name": {
+                    "documentation": "<p>Specifies the time metric by which to bin the analytics data.</p>",
+                    "shape": "AnalyticsBinByName"
+                },
+                "order": {
+                    "documentation": "<p>Specifies whether to bin the analytics data in ascending or descending order. If this field is left blank, the default order is by the key of the bin in descending order.</p>",
+                    "shape": "AnalyticsSortOrder"
+                }
+            },
+            "required": [
+                "name",
+                "interval"
+            ],
+            "type": "structure"
+        },
+        "AnalyticsBinKey": {
+            "documentation": "<p>An object containing the criterion by which to bin the results and the value that defines that bin.</p>",
+            "members": {
+                "name": {
+                    "documentation": "<p>The criterion by which to bin the results.</p>",
+                    "shape": "AnalyticsBinByName"
+                },
+                "value": {
+                    "documentation": "<p>The value of the criterion that defines the bin.</p>",
+                    "shape": "AnalyticsBinValue"
+                }
+            },
+            "type": "structure"
+        },
+        "AnalyticsBinKeys": {
+            "max": 1,
+            "member": {
+                "shape": "AnalyticsBinKey"
+            },
+            "min": 1,
+            "type": "list"
+        },
+        "AnalyticsBinValue": {
+            "type": "long"
+        },
+        "AnalyticsCommonFilterName": {
+            "enum": [
+                "BotAliasId",
+                "BotVersion",
+                "LocaleId",
+                "Modality",
+                "Channel"
+            ],
+            "type": "string"
+        },
+        "AnalyticsFilterOperator": {
+            "enum": [
+                "EQ",
+                "GT",
+                "LT"
+            ],
+            "type": "string"
+        },
+        "AnalyticsFilterValue": {
+            "type": "string"
+        },
+        "AnalyticsFilterValues": {
+            "max": 5,
+            "member": {
+                "shape": "AnalyticsFilterValue"
+            },
+            "min": 1,
+            "type": "list"
+        },
+        "AnalyticsGroupByValue": {
+            "type": "string"
+        },
+        "AnalyticsIntentField": {
+            "enum": [
+                "IntentName",
+                "IntentEndState",
+                "IntentLevel"
+            ],
+            "type": "string"
+        },
+        "AnalyticsIntentFilter": {
+            "documentation": "<p>Contains fields describing a condition by which to filter the intents. The expression may be understood as <code>name</code> <code>operator</code> <code>values</code>. For example:</p> <ul> <li> <p> <code>IntentName CO Book</code> \u2013 The intent name contains the string \"Book.\"</p> </li> <li> <p> <code>BotVersion EQ 2</code> \u2013 The bot version is equal to two.</p> </li> </ul> <p>The operators that each filter supports are listed below:</p> <ul> <li> <p> <code>BotAlias</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>BotVersion</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>LocaleId</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>Modality</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>Channel</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>SessionId</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>OriginatingRequestId</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>IntentName</code> \u2013 <code>EQ</code>, <code>CO</code>.</p> </li> <li> <p> <code>IntentEndState</code> \u2013 <code>EQ</code>, <code>CO</code>.</p> </li> </ul>",
+            "members": {
+                "name": {
+                    "documentation": "<p>The category by which to filter the intents. The descriptions for each option are as follows:</p> <ul> <li> <p> <code>BotAlias</code> \u2013 The name of the bot alias.</p> </li> <li> <p> <code>BotVersion</code> \u2013 The version of the bot.</p> </li> <li> <p> <code>LocaleId</code> \u2013 The locale of the bot.</p> </li> <li> <p> <code>Modality</code> \u2013 The modality of the session with the bot (audio, DTMF, or text).</p> </li> <li> <p> <code>Channel</code> \u2013 The channel that the bot is integrated with.</p> </li> <li> <p> <code>SessionId</code> \u2013 The identifier of the session with the bot.</p> </li> <li> <p> <code>OriginatingRequestId</code> \u2013 The identifier of the first request in a session.</p> </li> <li> <p> <code>IntentName</code> \u2013 The name of the intent.</p> </li> <li> <p> <code>IntentEndState</code> \u2013 The final state of the intent.</p> </li> </ul>",
+                    "shape": "AnalyticsIntentFilterName"
+                },
+                "operator": {
+                    "documentation": "<p>The operation by which to filter the category. The following operations are possible:</p> <ul> <li> <p> <code>CO</code> \u2013 Contains</p> </li> <li> <p> <code>EQ</code> \u2013 Equals</p> </li> <li> <p> <code>GT</code> \u2013 Greater than</p> </li> <li> <p> <code>LT</code> \u2013 Less than</p> </li> </ul> <p>The operators that each filter supports are listed below:</p> <ul> <li> <p> <code>BotAlias</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>BotVersion</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>LocaleId</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>Modality</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>Channel</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>SessionId</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>OriginatingRequestId</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>IntentName</code> \u2013 <code>EQ</code>, <code>CO</code>.</p> </li> <li> <p> <code>IntentEndState</code> \u2013 <code>EQ</code>, <code>CO</code>.</p> </li> </ul>",
+                    "shape": "AnalyticsFilterOperator"
+                },
+                "values": {
+                    "documentation": "<p>An array containing the values of the category by which to apply the operator to filter the results. You can provide multiple values if the operator is <code>EQ</code> or <code>CO</code>. If you provide multiple values, you filter for results that equal/contain any of the values. For example, if the <code>name</code>, <code>operator</code>, and <code>values</code> fields are <code>Modality</code>, <code>EQ</code>, and <code>[Speech, Text]</code>, the operation filters for results where the modality was either <code>Speech</code> or <code>Text</code>.</p>",
+                    "shape": "AnalyticsFilterValues"
+                }
+            },
+            "required": [
+                "name",
+                "operator",
+                "values"
+            ],
+            "type": "structure"
+        },
+        "AnalyticsIntentFilterName": {
+            "enum": [
+                "BotAliasId",
+                "BotVersion",
+                "LocaleId",
+                "Modality",
+                "Channel",
+                "SessionId",
+                "OriginatingRequestId",
+                "IntentName",
+                "IntentEndState"
+            ],
+            "type": "string"
+        },
+        "AnalyticsIntentFilters": {
+            "max": 9,
+            "member": {
+                "shape": "AnalyticsIntentFilter"
+            },
+            "min": 1,
+            "type": "list"
+        },
+        "AnalyticsIntentGroupByKey": {
+            "documentation": "<p>Contains the category by which the intent analytics were grouped and a member of that category.</p>",
+            "members": {
+                "name": {
+                    "documentation": "<p>A category by which the intent analytics were grouped.</p>",
+                    "shape": "AnalyticsIntentField"
+                },
+                "value": {
+                    "documentation": "<p>A member of the category by which the intent analytics were grouped.</p>",
+                    "shape": "AnalyticsGroupByValue"
+                }
+            },
+            "type": "structure"
+        },
+        "AnalyticsIntentGroupByKeys": {
+            "member": {
+                "shape": "AnalyticsIntentGroupByKey"
+            },
+            "type": "list"
+        },
+        "AnalyticsIntentGroupByList": {
+            "max": 3,
+            "member": {
+                "shape": "AnalyticsIntentGroupBySpecification"
+            },
+            "min": 1,
+            "type": "list"
+        },
+        "AnalyticsIntentGroupBySpecification": {
+            "documentation": "<p>Contains the category by which to group the intents.</p>",
+            "members": {
+                "name": {
+                    "documentation": "<p>Specifies whether to group the intent stages by their name or their end state.</p>",
+                    "shape": "AnalyticsIntentField"
+                }
+            },
+            "required": [
+                "name"
+            ],
+            "type": "structure"
+        },
+        "AnalyticsIntentMetric": {
+            "documentation": "<p>Contains the metric and the summary statistic you want to calculate, and the order in which to sort the results, for the intents in the bot.</p>",
+            "members": {
+                "name": {
+                    "documentation": "<p>The metric for which you want to get intent summary statistics.</p> <ul> <li> <p> <code>Count</code> \u2013 The number of times the intent was invoked.</p> </li> <li> <p> <code>Success</code> \u2013 The number of times the intent succeeded.</p> </li> <li> <p> <code>Failure</code> \u2013 The number of times the intent failed.</p> </li> <li> <p> <code>Switched</code> \u2013 The number of times there was a switch to a different intent.</p> </li> <li> <p> <code>Dropped</code> \u2013 The number of times the user dropped the intent.</p> </li> </ul>",
+                    "shape": "AnalyticsIntentMetricName"
+                },
+                "order": {
+                    "documentation": "<p>Specifies whether to sort the results in ascending or descending order.</p>",
+                    "shape": "AnalyticsSortOrder"
+                },
+                "statistic": {
+                    "documentation": "<p>The summary statistic to calculate.</p> <ul> <li> <p> <code>Sum</code> \u2013 The total count for the category you provide in <code>name</code>.</p> </li> <li> <p> <code>Average</code> \u2013 The total count divided by the number of intents in the category you provide in <code>name</code>.</p> </li> <li> <p> <code>Max</code> \u2013 The highest count in the category you provide in <code>name</code>.</p> </li> </ul>",
+                    "shape": "AnalyticsMetricStatistic"
+                }
+            },
+            "required": [
+                "name",
+                "statistic"
+            ],
+            "type": "structure"
+        },
+        "AnalyticsIntentMetricName": {
+            "enum": [
+                "Count",
+                "Success",
+                "Failure",
+                "Switched",
+                "Dropped"
+            ],
+            "type": "string"
+        },
+        "AnalyticsIntentMetricResult": {
+            "documentation": "<p>An object containing the results for the intent metric you requested.</p>",
+            "members": {
+                "name": {
+                    "documentation": "<p>The metric that you requested. See <a href=\"https://docs.aws.amazon.com/lexv2/latest/dg/analytics-key-definitions.html\">Key definitions</a> for more details about these metrics.</p> <ul> <li> <p> <code>Count</code> \u2013 The number of times the intent was invoked.</p> </li> <li> <p> <code>Success</code> \u2013 The number of times the intent succeeded.</p> </li> <li> <p> <code>Failure</code> \u2013 The number of times the intent failed.</p> </li> <li> <p> <code>Switched</code> \u2013 The number of times there was a switch to a different intent.</p> </li> <li> <p> <code>Dropped</code> \u2013 The number of times the user dropped the intent.</p> </li> </ul>",
+                    "shape": "AnalyticsIntentMetricName"
+                },
+                "statistic": {
+                    "documentation": "<p>The statistic that you requested to calculate.</p> <ul> <li> <p> <code>Sum</code> \u2013 The total count for the category you provide in <code>name</code>.</p> </li> <li> <p> <code>Average</code> \u2013 The total count divided by the number of intents in the category you provide in <code>name</code>.</p> </li> <li> <p> <code>Max</code> \u2013 The highest count in the category you provide in <code>name</code>.</p> </li> </ul>",
+                    "shape": "AnalyticsMetricStatistic"
+                },
+                "value": {
+                    "documentation": "<p>The value of the summary statistic for the metric that you requested.</p>",
+                    "shape": "AnalyticsMetricValue"
+                }
+            },
+            "type": "structure"
+        },
+        "AnalyticsIntentMetricResults": {
+            "member": {
+                "shape": "AnalyticsIntentMetricResult"
+            },
+            "type": "list"
+        },
+        "AnalyticsIntentMetrics": {
+            "max": 5,
+            "member": {
+                "shape": "AnalyticsIntentMetric"
+            },
+            "min": 1,
+            "type": "list"
+        },
+        "AnalyticsIntentNodeSummaries": {
+            "max": 100,
+            "member": {
+                "shape": "AnalyticsIntentNodeSummary"
+            },
+            "min": 1,
+            "type": "list"
+        },
+        "AnalyticsIntentNodeSummary": {
+            "documentation": "<p>An object containing information about the requested path.</p>",
+            "members": {
+                "intentCount": {
+                    "documentation": "<p>The total number of sessions that follow the given path to the given intent.</p>",
+                    "shape": "AnalyticsNodeCount"
+                },
+                "intentLevel": {
+                    "documentation": "<p>The number of intents up to and including the requested path.</p>",
+                    "shape": "AnalyticsNodeLevel"
+                },
+                "intentName": {
+                    "documentation": "<p>The name of the intent at the end of the requested path.</p>",
+                    "shape": "Name"
+                },
+                "intentPath": {
+                    "documentation": "<p>The path.</p>",
+                    "shape": "AnalyticsPath"
+                },
+                "nodeType": {
+                    "documentation": "<p>Specifies whether the node is the end of a path (<code>Exit</code>) or not (<code>Inner</code>).</p>",
+                    "shape": "AnalyticsNodeType"
+                }
+            },
+            "type": "structure"
+        },
+        "AnalyticsIntentResult": {
+            "documentation": "<p>An object containing the results for the intent metrics you requested and the bin and/or group(s) they refer to, if applicable.</p>",
+            "members": {
+                "binKeys": {
+                    "documentation": "<p>A list of objects containing the criteria you requested for binning results and the values of the bins.</p>",
+                    "shape": "AnalyticsBinKeys"
+                },
+                "groupByKeys": {
+                    "documentation": "<p>A list of objects containing the criteria you requested for grouping results and the values of the groups.</p>",
+                    "shape": "AnalyticsIntentGroupByKeys"
+                },
+                "metricsResults": {
+                    "documentation": "<p>A list of objects, each of which contains a metric you want to list, the statistic for the metric you want to return, and the method by which to organize the results.</p>",
+                    "shape": "AnalyticsIntentMetricResults"
+                }
+            },
+            "type": "structure"
+        },
+        "AnalyticsIntentResults": {
+            "member": {
+                "shape": "AnalyticsIntentResult"
+            },
+            "type": "list"
+        },
+        "AnalyticsIntentStageField": {
+            "enum": [
+                "IntentStageName",
+                "SwitchedToIntent"
+            ],
+            "type": "string"
+        },
+        "AnalyticsIntentStageFilter": {
+            "documentation": "<p>Contains fields describing a condition by which to filter the intent stages. The expression may be understood as <code>name</code> <code>operator</code> <code>values</code>. For example:</p> <ul> <li> <p> <code>IntentName CO Book</code> \u2013 The intent name contains the string \"Book.\"</p> </li> <li> <p> <code>BotVersion EQ 2</code> \u2013 The bot version is equal to two.</p> </li> </ul> <p>The operators that each filter supports are listed below:</p> <ul> <li> <p> <code>BotAlias</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>BotVersion</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>LocaleId</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>Modality</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>Channel</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>SessionId</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>OriginatingRequestId</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>IntentName</code> \u2013 <code>EQ</code>, <code>CO</code>.</p> </li> <li> <p> <code>IntentStageName</code> \u2013 <code>EQ</code>, <code>CO</code>.</p> </li> </ul>",
+            "members": {
+                "name": {
+                    "documentation": "<p>The category by which to filter the intent stages. The descriptions for each option are as follows:</p> <ul> <li> <p> <code>BotAlias</code> \u2013 The name of the bot alias.</p> </li> <li> <p> <code>BotVersion</code> \u2013 The version of the bot.</p> </li> <li> <p> <code>LocaleId</code> \u2013 The locale of the bot.</p> </li> <li> <p> <code>Modality</code> \u2013 The modality of the session with the bot (audio, DTMF, or text).</p> </li> <li> <p> <code>Channel</code> \u2013 The channel that the bot is integrated with.</p> </li> <li> <p> <code>SessionId</code> \u2013 The identifier of the session with the bot.</p> </li> <li> <p> <code>OriginatingRequestId</code> \u2013 The identifier of the first request in a session.</p> </li> <li> <p> <code>IntentName</code> \u2013 The name of the intent.</p> </li> <li> <p> <code>IntentStageName</code> \u2013 The stage in the intent.</p> </li> </ul>",
+                    "shape": "AnalyticsIntentStageFilterName"
+                },
+                "operator": {
+                    "documentation": "<p>The operation by which to filter the category. The following operations are possible:</p> <ul> <li> <p> <code>CO</code> \u2013 Contains</p> </li> <li> <p> <code>EQ</code> \u2013 Equals</p> </li> <li> <p> <code>GT</code> \u2013 Greater than</p> </li> <li> <p> <code>LT</code> \u2013 Less than</p> </li> </ul> <p>The operators that each filter supports are listed below:</p> <ul> <li> <p> <code>BotAlias</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>BotVersion</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>LocaleId</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>Modality</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>Channel</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>SessionId</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>OriginatingRequestId</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>IntentName</code> \u2013 <code>EQ</code>, <code>CO</code>.</p> </li> <li> <p> <code>IntentStageName</code> \u2013 <code>EQ</code>, <code>CO</code>.</p> </li> </ul>",
+                    "shape": "AnalyticsFilterOperator"
+                },
+                "values": {
+                    "documentation": "<p>An array containing the values of the category by which to apply the operator to filter the results. You can provide multiple values if the operator is <code>EQ</code> or <code>CO</code>. If you provide multiple values, you filter for results that equal/contain any of the values. For example, if the <code>name</code>, <code>operator</code>, and <code>values</code> fields are <code>Modality</code>, <code>EQ</code>, and <code>[Speech, Text]</code>, the operation filters for results where the modality was either <code>Speech</code> or <code>Text</code>.</p>",
+                    "shape": "AnalyticsFilterValues"
+                }
+            },
+            "required": [
+                "name",
+                "operator",
+                "values"
+            ],
+            "type": "structure"
+        },
+        "AnalyticsIntentStageFilterName": {
+            "enum": [
+                "BotAliasId",
+                "BotVersion",
+                "LocaleId",
+                "Modality",
+                "Channel",
+                "SessionId",
+                "OriginatingRequestId",
+                "IntentName",
+                "IntentStageName"
+            ],
+            "type": "string"
+        },
+        "AnalyticsIntentStageFilters": {
+            "max": 9,
+            "member": {
+                "shape": "AnalyticsIntentStageFilter"
+            },
+            "min": 1,
+            "type": "list"
+        },
+        "AnalyticsIntentStageGroupByKey": {
+            "documentation": "<p>Contains the category by which the intent stage analytics and the values for that category were grouped.</p>",
+            "members": {
+                "name": {
+                    "documentation": "<p>A category by which the intent stage analytics were grouped.</p>",
+                    "shape": "AnalyticsIntentStageField"
+                },
+                "value": {
+                    "documentation": "<p>A member of the category by which the intent stage analytics were grouped.</p>",
+                    "shape": "AnalyticsGroupByValue"
+                }
+            },
+            "type": "structure"
+        },
+        "AnalyticsIntentStageGroupByKeys": {
+            "member": {
+                "shape": "AnalyticsIntentStageGroupByKey"
+            },
+            "type": "list"
+        },
+        "AnalyticsIntentStageGroupByList": {
+            "max": 2,
+            "member": {
+                "shape": "AnalyticsIntentStageGroupBySpecification"
+            },
+            "min": 1,
+            "type": "list"
+        },
+        "AnalyticsIntentStageGroupBySpecification": {
+            "documentation": "<p>Contains the category by which to group the intent stages.</p>",
+            "members": {
+                "name": {
+                    "documentation": "<p>Specifies whether to group the intent stages by their name or the intent to which the session was switched.</p>",
+                    "shape": "AnalyticsIntentStageField"
+                }
+            },
+            "required": [
+                "name"
+            ],
+            "type": "structure"
+        },
+        "AnalyticsIntentStageMetric": {
+            "documentation": "<p>Contains the metric and the summary statistic you want to calculate, and the order in which to sort the results, for the intent stages across the user sessions with the bot.</p>",
+            "members": {
+                "name": {
+                    "documentation": "<p>The metric for which you want to get intent stage summary statistics. See <a href=\"https://docs.aws.amazon.com/lexv2/latest/dg/analytics-key-definitions.html\">Key definitions</a> for more details about these metrics.</p> <ul> <li> <p> <code>Count</code> \u2013 The number of times the intent stage occurred.</p> </li> <li> <p> <code>Success</code> \u2013 The number of times the intent stage succeeded.</p> </li> <li> <p> <code>Failure</code> \u2013 The number of times the intent stage failed.</p> </li> <li> <p> <code>Dropped</code> \u2013 The number of times the user dropped the intent stage.</p> </li> <li> <p> <code>Retry</code> \u2013 The number of times the bot tried to elicit a response from the user at this stage.</p> </li> </ul>",
+                    "shape": "AnalyticsIntentStageMetricName"
+                },
+                "order": {
+                    "documentation": "<p>Specifies whether to sort the results in ascending or descending order of the summary statistic (<code>value</code> in the response).</p>",
+                    "shape": "AnalyticsSortOrder"
+                },
+                "statistic": {
+                    "documentation": "<p>The summary statistic to calculate.</p> <ul> <li> <p> <code>Sum</code> \u2013 The total count for the category you provide in <code>name</code>.</p> </li> <li> <p> <code>Average</code> \u2013 The total count divided by the number of intent stages in the category you provide in <code>name</code>.</p> </li> <li> <p> <code>Max</code> \u2013 The highest count in the category you provide in <code>name</code>.</p> </li> </ul>",
+                    "shape": "AnalyticsMetricStatistic"
+                }
+            },
+            "required": [
+                "name",
+                "statistic"
+            ],
+            "type": "structure"
+        },
+        "AnalyticsIntentStageMetricName": {
+            "enum": [
+                "Count",
+                "Success",
+                "Failed",
+                "Dropped",
+                "Retry"
+            ],
+            "type": "string"
+        },
+        "AnalyticsIntentStageMetricResult": {
+            "documentation": "<p>An object containing the results for an intent stage metric you requested.</p>",
+            "members": {
+                "name": {
+                    "documentation": "<p>The metric that you requested.</p> <ul> <li> <p> <code>Count</code> \u2013 The number of times the intent stage occurred.</p> </li> <li> <p> <code>Success</code> \u2013 The number of times the intent stage succeeded.</p> </li> <li> <p> <code>Failure</code> \u2013 The number of times the intent stage failed.</p> </li> <li> <p> <code>Dropped</code> \u2013 The number of times the user dropped the intent stage.</p> </li> <li> <p> <code>Retry</code> \u2013 The number of times the bot tried to elicit a response from the user at this stage.</p> </li> </ul>",
+                    "shape": "AnalyticsIntentStageMetricName"
+                },
+                "statistic": {
+                    "documentation": "<p>The summary statistic that you requested to calculate.</p> <ul> <li> <p> <code>Sum</code> \u2013 The total count for the category you provide in <code>name</code>.</p> </li> <li> <p> <code>Average</code> \u2013 The total count divided by the number of intent stages in the category you provide in <code>name</code>.</p> </li> <li> <p> <code>Max</code> \u2013 The highest count in the category you provide in <code>name</code>.</p> </li> </ul>",
+                    "shape": "AnalyticsMetricStatistic"
+                },
+                "value": {
+                    "documentation": "<p>The value of the summary statistic for the metric that you requested.</p>",
+                    "shape": "AnalyticsMetricValue"
+                }
+            },
+            "type": "structure"
+        },
+        "AnalyticsIntentStageMetricResults": {
+            "member": {
+                "shape": "AnalyticsIntentStageMetricResult"
+            },
+            "type": "list"
+        },
+        "AnalyticsIntentStageMetrics": {
+            "max": 5,
+            "member": {
+                "shape": "AnalyticsIntentStageMetric"
+            },
+            "min": 1,
+            "type": "list"
+        },
+        "AnalyticsIntentStageResult": {
+            "documentation": "<p>An object containing the results for the intent stage metrics you requested and the bin and/or group they refer to, if applicable.</p>",
+            "members": {
+                "binKeys": {
+                    "documentation": "<p>A list of objects containing the criteria you requested for binning results and the values of the bins.</p>",
+                    "shape": "AnalyticsBinKeys"
+                },
+                "groupByKeys": {
+                    "documentation": "<p>A list of objects containing the criteria you requested for grouping results and the values of the bins.</p>",
+                    "shape": "AnalyticsIntentStageGroupByKeys"
+                },
+                "metricsResults": {
+                    "documentation": "<p>A list of objects, each of which contains a metric you want to list, the statistic for the metric you want to return, and the method by which to organize the results.</p>",
+                    "shape": "AnalyticsIntentStageMetricResults"
+                }
+            },
+            "type": "structure"
+        },
+        "AnalyticsIntentStageResults": {
+            "member": {
+                "shape": "AnalyticsIntentStageResult"
+            },
+            "type": "list"
+        },
+        "AnalyticsInterval": {
+            "enum": [
+                "OneHour",
+                "OneDay"
+            ],
+            "type": "string"
+        },
+        "AnalyticsLongValue": {
+            "type": "long"
+        },
+        "AnalyticsMetricStatistic": {
+            "enum": [
+                "Sum",
+                "Avg",
+                "Max"
+            ],
+            "type": "string"
+        },
+        "AnalyticsMetricValue": {
+            "type": "double"
+        },
+        "AnalyticsModality": {
+            "enum": [
+                "Speech",
+                "Text",
+                "DTMF",
+                "MultiMode"
+            ],
+            "type": "string"
+        },
+        "AnalyticsNodeCount": {
+            "type": "integer"
+        },
+        "AnalyticsNodeLevel": {
+            "max": 100,
+            "min": 0,
+            "type": "integer"
+        },
+        "AnalyticsNodeType": {
+            "enum": [
+                "Inner",
+                "Exit"
+            ],
+            "type": "string"
+        },
+        "AnalyticsOriginatingRequestId": {
+            "type": "string"
+        },
+        "AnalyticsPath": {
+            "max": 1024,
+            "min": 1,
+            "type": "string"
+        },
+        "AnalyticsPathFilter": {
+            "documentation": "<p>Contains fields describing a condition by which to filter the paths. The expression may be understood as <code>name</code> <code>operator</code> <code>values</code>. For example:</p> <ul> <li> <p> <code>LocaleId EQ en</code> \u2013 The locale is \"en\".</p> </li> <li> <p> <code>BotVersion EQ 2</code> \u2013 The bot version is equal to two.</p> </li> </ul> <p>The operators that each filter supports are listed below:</p> <ul> <li> <p> <code>BotAlias</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>BotVersion</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>LocaleId</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>Modality</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>Channel</code> \u2013 <code>EQ</code>.</p> </li> </ul>",
+            "members": {
+                "name": {
+                    "documentation": "<p>The category by which to filter the intent paths. The descriptions for each option are as follows:</p> <ul> <li> <p> <code>BotAlias</code> \u2013 The name of the bot alias.</p> </li> <li> <p> <code>BotVersion</code> \u2013 The version of the bot.</p> </li> <li> <p> <code>LocaleId</code> \u2013 The locale of the bot.</p> </li> <li> <p> <code>Modality</code> \u2013 The modality of the session with the bot (audio, DTMF, or text).</p> </li> <li> <p> <code>Channel</code> \u2013 The channel that the bot is integrated with.</p> </li> </ul>",
+                    "shape": "AnalyticsCommonFilterName"
+                },
+                "operator": {
+                    "documentation": "<p>The operation by which to filter the category. The following operations are possible:</p> <ul> <li> <p> <code>CO</code> \u2013 Contains</p> </li> <li> <p> <code>EQ</code> \u2013 Equals</p> </li> <li> <p> <code>GT</code> \u2013 Greater than</p> </li> <li> <p> <code>LT</code> \u2013 Less than</p> </li> </ul> <p>The operators that each filter supports are listed below:</p> <ul> <li> <p> <code>BotAlias</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>BotVersion</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>LocaleId</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>Modality</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>Channel</code> \u2013 <code>EQ</code>.</p> </li> </ul>",
+                    "shape": "AnalyticsFilterOperator"
+                },
+                "values": {
+                    "documentation": "<p>An array containing the values of the category by which to apply the operator to filter the results. You can provide multiple values if the operator is <code>EQ</code> or <code>CO</code>. If you provide multiple values, you filter for results that equal/contain any of the values. For example, if the <code>name</code>, <code>operator</code>, and <code>values</code> fields are <code>Modality</code>, <code>EQ</code>, and <code>[Speech, Text]</code>, the operation filters for results where the modality was either <code>Speech</code> or <code>Text</code>.</p>",
+                    "shape": "AnalyticsFilterValues"
+                }
+            },
+            "required": [
+                "name",
+                "operator",
+                "values"
+            ],
+            "type": "structure"
+        },
+        "AnalyticsPathFilters": {
+            "max": 5,
+            "member": {
+                "shape": "AnalyticsPathFilter"
+            },
+            "min": 1,
+            "type": "list"
+        },
+        "AnalyticsSessionField": {
+            "enum": [
+                "ConversationEndState",
+                "LocaleId"
+            ],
+            "type": "string"
+        },
+        "AnalyticsSessionFilter": {
+            "documentation": "<p>Contains fields describing a condition by which to filter the sessions. The expression may be understood as <code>name</code> <code>operator</code> <code>values</code>. For example:</p> <ul> <li> <p> <code>LocaleId EQ en</code> \u2013 The locale is \"en\".</p> </li> <li> <p> <code>Duration GT 200</code> \u2013 The duration is greater than 200 seconds.</p> </li> </ul> <p>The operators that each filter supports are listed below:</p> <ul> <li> <p> <code>BotAlias</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>BotVersion</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>LocaleId</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>Modality</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>Channel</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>Duration</code> \u2013 <code>EQ</code>, <code>GT</code>, <code>LT</code>.</p> </li> <li> <p> <code>conversationEndState</code> \u2013 <code>EQ</code>, <code>CO</code>.</p> </li> <li> <p> <code>SessionId</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>OriginatingRequestId</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>IntentPath</code> \u2013 <code>EQ</code>.</p> </li> </ul>",
+            "members": {
+                "name": {
+                    "documentation": "<p>The category by which to filter the sessions. The descriptions for each option are as follows:</p> <ul> <li> <p> <code>BotAlias</code> \u2013 The name of the bot alias.</p> </li> <li> <p> <code>BotVersion</code> \u2013 The version of the bot.</p> </li> <li> <p> <code>LocaleId</code> \u2013 The locale of the bot.</p> </li> <li> <p> <code>Modality</code> \u2013 The modality of the session with the bot (audio, DTMF, or text).</p> </li> <li> <p> <code>Channel</code> \u2013 The channel that the bot is integrated with.</p> </li> <li> <p> <code>Duration</code> \u2013 The duration of the session.</p> </li> <li> <p> <code>conversationEndState</code> \u2013 The final state of the session.</p> </li> <li> <p> <code>SessionId</code> \u2013 The identifier of the session with the bot.</p> </li> <li> <p> <code>OriginatingRequestId</code> \u2013 The identifier of the first request in a session.</p> </li> <li> <p> <code>IntentPath</code> \u2013 The order of intents taken in a session.</p> </li> </ul>",
+                    "shape": "AnalyticsSessionFilterName"
+                },
+                "operator": {
+                    "documentation": "<p>The operation by which to filter the category. The following operations are possible:</p> <ul> <li> <p> <code>CO</code> \u2013 Contains</p> </li> <li> <p> <code>EQ</code> \u2013 Equals</p> </li> <li> <p> <code>GT</code> \u2013 Greater than</p> </li> <li> <p> <code>LT</code> \u2013 Less than</p> </li> </ul> <p>The operators that each filter supports are listed below:</p> <ul> <li> <p> <code>BotAlias</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>BotVersion</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>LocaleId</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>Modality</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>Channel</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>Duration</code> \u2013 <code>EQ</code>, <code>GT</code>, <code>LT</code>.</p> </li> <li> <p> <code>conversationEndState</code> \u2013 <code>EQ</code>, <code>CO</code>.</p> </li> <li> <p> <code>SessionId</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>OriginatingRequestId</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>IntentPath</code> \u2013 <code>EQ</code>.</p> </li> </ul>",
+                    "shape": "AnalyticsFilterOperator"
+                },
+                "values": {
+                    "documentation": "<p>An array containing the values of the category by which to apply the operator to filter the results. You can provide multiple values if the operator is <code>EQ</code> or <code>CO</code>. If you provide multiple values, you filter for results that equal/contain any of the values. For example, if the <code>name</code>, <code>operator</code>, and <code>values</code> fields are <code>Modality</code>, <code>EQ</code>, and <code>[Speech, Text]</code>, the operation filters for results where the modality was either <code>Speech</code> or <code>Text</code>.</p>",
+                    "shape": "AnalyticsFilterValues"
+                }
+            },
+            "required": [
+                "name",
+                "operator",
+                "values"
+            ],
+            "type": "structure"
+        },
+        "AnalyticsSessionFilterName": {
+            "enum": [
+                "BotAliasId",
+                "BotVersion",
+                "LocaleId",
+                "Modality",
+                "Channel",
+                "Duration",
+                "ConversationEndState",
+                "SessionId",
+                "OriginatingRequestId",
+                "IntentPath"
+            ],
+            "type": "string"
+        },
+        "AnalyticsSessionFilters": {
+            "max": 10,
+            "member": {
+                "shape": "AnalyticsSessionFilter"
+            },
+            "min": 1,
+            "type": "list"
+        },
+        "AnalyticsSessionGroupByKey": {
+            "documentation": "<p>Contains the category by which the session analytics were grouped and a member of that category.</p>",
+            "members": {
+                "name": {
+                    "documentation": "<p>The category by which the session analytics were grouped.</p>",
+                    "shape": "AnalyticsSessionField"
+                },
+                "value": {
+                    "documentation": "<p>A member of the category by which the session analytics were grouped.</p>",
+                    "shape": "AnalyticsGroupByValue"
+                }
+            },
+            "type": "structure"
+        },
+        "AnalyticsSessionGroupByKeys": {
+            "member": {
+                "shape": "AnalyticsSessionGroupByKey"
+            },
+            "type": "list"
+        },
+        "AnalyticsSessionGroupByList": {
+            "max": 2,
+            "member": {
+                "shape": "AnalyticsSessionGroupBySpecification"
+            },
+            "min": 1,
+            "type": "list"
+        },
+        "AnalyticsSessionGroupBySpecification": {
+            "documentation": "<p>Contains the category by which to group the sessions.</p>",
+            "members": {
+                "name": {
+                    "documentation": "<p>Specifies whether to group the session by their end state or their locale.</p>",
+                    "shape": "AnalyticsSessionField"
+                }
+            },
+            "required": [
+                "name"
+            ],
+            "type": "structure"
+        },
+        "AnalyticsSessionId": {
+            "pattern": "[0-9a-zA-Z._:-]",
+            "type": "string"
+        },
+        "AnalyticsSessionMetric": {
+            "documentation": "<p>Contains the metric and the summary statistic you want to calculate, and the order in which to sort the results, for the user sessions with the bot.</p>",
+            "members": {
+                "name": {
+                    "documentation": "<p>The metric for which you want to get session summary statistics.</p> <ul> <li> <p> <code>Count</code> \u2013 The number of sessions.</p> </li> <li> <p> <code>Success</code> \u2013 The number of sessions that succeeded.</p> </li> <li> <p> <code>Failure</code> \u2013 The number of sessions that failed.</p> </li> <li> <p> <code>Dropped</code> \u2013 The number of sessions that the user dropped.</p> </li> <li> <p> <code>Duration</code> \u2013 The duration of sessions.</p> </li> <li> <p> <code>TurnsPerSession</code> \u2013 The number of turns in the sessions.</p> </li> <li> <p> <code>Concurrency</code> \u2013 The number of sessions occurring in the same period of time.</p> </li> </ul>",
+                    "shape": "AnalyticsSessionMetricName"
+                },
+                "order": {
+                    "documentation": "<p>Specifies whether to sort the results in ascending or descending order.</p>",
+                    "shape": "AnalyticsSortOrder"
+                },
+                "statistic": {
+                    "documentation": "<p>The summary statistic to calculate.</p> <ul> <li> <p> <code>Sum</code> \u2013 The total count for the category you provide in <code>name</code>.</p> </li> <li> <p> <code>Average</code> \u2013 The total count divided by the number of sessions in the category you provide in <code>name</code>.</p> </li> <li> <p> <code>Max</code> \u2013 The highest count in the category you provide in <code>name</code>.</p> </li> </ul>",
+                    "shape": "AnalyticsMetricStatistic"
+                }
+            },
+            "required": [
+                "name",
+                "statistic"
+            ],
+            "type": "structure"
+        },
+        "AnalyticsSessionMetricName": {
+            "enum": [
+                "Count",
+                "Success",
+                "Failure",
+                "Dropped",
+                "Duration",
+                "TurnsPerConversation",
+                "Concurrency"
+            ],
+            "type": "string"
+        },
+        "AnalyticsSessionMetricResult": {
+            "documentation": "<p>An object containing the results for a session metric you requested.</p>",
+            "members": {
+                "name": {
+                    "documentation": "<p>The metric that you requested.</p> <ul> <li> <p> <code>Count</code> \u2013 The number of sessions.</p> </li> <li> <p> <code>Success</code> \u2013 The number of sessions that succeeded.</p> </li> <li> <p> <code>Failure</code> \u2013 The number of sessions that failed.</p> </li> <li> <p> <code>Dropped</code> \u2013 The number of sessions that the user dropped.</p> </li> <li> <p> <code>Duration</code> \u2013 The duration of sessions.</p> </li> <li> <p> <code>TurnPersession</code> \u2013 The number of turns in the sessions.</p> </li> <li> <p> <code>Concurrency</code> \u2013 The number of sessions occurring in the same period of time.</p> </li> </ul>",
+                    "shape": "AnalyticsSessionMetricName"
+                },
+                "statistic": {
+                    "documentation": "<p>The summary statistic that you requested to calculate.</p> <ul> <li> <p> <code>Sum</code> \u2013 The total count for the category you provide in <code>name</code>.</p> </li> <li> <p> <code>Average</code> \u2013 The total count divided by the number of sessions in the category you provide in <code>name</code>.</p> </li> <li> <p> <code>Max</code> \u2013 The highest count in the category you provide in <code>name</code>.</p> </li> </ul>",
+                    "shape": "AnalyticsMetricStatistic"
+                },
+                "value": {
+                    "documentation": "<p>The value of the summary statistic for the metric that you requested.</p>",
+                    "shape": "AnalyticsMetricValue"
+                }
+            },
+            "type": "structure"
+        },
+        "AnalyticsSessionMetricResults": {
+            "member": {
+                "shape": "AnalyticsSessionMetricResult"
+            },
+            "type": "list"
+        },
+        "AnalyticsSessionMetrics": {
+            "max": 7,
+            "member": {
+                "shape": "AnalyticsSessionMetric"
+            },
+            "min": 1,
+            "type": "list"
+        },
+        "AnalyticsSessionResult": {
+            "documentation": "<p>An object containing the results for the session metrics you requested and the bin and/or group(s) they refer to, if applicable.</p>",
+            "members": {
+                "binKeys": {
+                    "documentation": "<p>A list of objects containing the criteria you requested for binning results and the values of the bins.</p>",
+                    "shape": "AnalyticsBinKeys"
+                },
+                "groupByKeys": {
+                    "documentation": "<p>A list of objects containing the criteria you requested for grouping results and the values of the bins.</p>",
+                    "shape": "AnalyticsSessionGroupByKeys"
+                },
+                "metricsResults": {
+                    "documentation": "<p>A list of objects, each of which contains a metric you want to list, the statistic for the metric you want to return, and the method by which to organize the results.</p>",
+                    "shape": "AnalyticsSessionMetricResults"
+                }
+            },
+            "type": "structure"
+        },
+        "AnalyticsSessionResults": {
+            "member": {
+                "shape": "AnalyticsSessionResult"
+            },
+            "type": "list"
+        },
+        "AnalyticsSessionSortByName": {
+            "enum": [
+                "ConversationStartTime",
+                "NumberOfTurns",
+                "Duration"
+            ],
+            "type": "string"
+        },
+        "AnalyticsSortOrder": {
+            "enum": [
+                "Ascending",
+                "Descending"
+            ],
+            "type": "string"
+        },
+        "AnalyticsUtteranceAttribute": {
+            "documentation": "<p>An object that specifies the last used intent at the time of the utterance as an attribute to return.</p>",
+            "members": {
+                "name": {
+                    "documentation": "<p>An attribute to return. The only available attribute is the intent that the bot mapped the utterance to.</p>",
+                    "shape": "AnalyticsUtteranceAttributeName"
+                }
+            },
+            "required": [
+                "name"
+            ],
+            "type": "structure"
+        },
+        "AnalyticsUtteranceAttributeName": {
+            "enum": [
+                "LastUsedIntent"
+            ],
+            "type": "string"
+        },
+        "AnalyticsUtteranceAttributeResult": {
+            "documentation": "<p>An object containing the intent that the bot mapped the utterance to.</p>",
+            "members": {
+                "lastUsedIntent": {
+                    "documentation": "<p>The intent that the bot mapped the utterance to.</p>",
+                    "shape": "Name"
+                }
+            },
+            "type": "structure"
+        },
+        "AnalyticsUtteranceAttributeResults": {
+            "member": {
+                "shape": "AnalyticsUtteranceAttributeResult"
+            },
+            "type": "list"
+        },
+        "AnalyticsUtteranceAttributes": {
+            "max": 1,
+            "member": {
+                "shape": "AnalyticsUtteranceAttribute"
+            },
+            "min": 1,
+            "type": "list"
+        },
+        "AnalyticsUtteranceField": {
+            "enum": [
+                "UtteranceText",
+                "UtteranceState"
+            ],
+            "type": "string"
+        },
+        "AnalyticsUtteranceFilter": {
+            "documentation": "<p>Contains fields describing a condition by which to filter the utterances. The expression may be understood as <code>name</code> <code>operator</code> <code>values</code>. For example:</p> <ul> <li> <p> <code>LocaleId EQ Book</code> \u2013 The locale is the string \"en\".</p> </li> <li> <p> <code>UtteranceText CO help</code> \u2013 The text of the utterance contains the string \"help\".</p> </li> </ul> <p>The operators that each filter supports are listed below:</p> <ul> <li> <p> <code>BotAlias</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>BotVersion</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>LocaleId</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>Modality</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>Channel</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>SessionId</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>OriginatingRequestId</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>UtteranceState</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>UtteranceText</code> \u2013 <code>EQ</code>, <code>CO</code>.</p> </li> </ul>",
+            "members": {
+                "name": {
+                    "documentation": "<p>The category by which to filter the utterances. The descriptions for each option are as follows:</p> <ul> <li> <p> <code>BotAlias</code> \u2013 The name of the bot alias.</p> </li> <li> <p> <code>BotVersion</code> \u2013 The version of the bot.</p> </li> <li> <p> <code>LocaleId</code> \u2013 The locale of the bot.</p> </li> <li> <p> <code>Modality</code> \u2013 The modality of the session with the bot (audio, DTMF, or text).</p> </li> <li> <p> <code>Channel</code> \u2013 The channel that the bot is integrated with.</p> </li> <li> <p> <code>SessionId</code> \u2013 The identifier of the session with the bot.</p> </li> <li> <p> <code>OriginatingRequestId</code> \u2013 The identifier of the first request in a session.</p> </li> <li> <p> <code>UtteranceState</code> \u2013 The state of the utterance.</p> </li> <li> <p> <code>UtteranceText</code> \u2013 The text in the utterance.</p> </li> </ul>",
+                    "shape": "AnalyticsUtteranceFilterName"
+                },
+                "operator": {
+                    "documentation": "<p>The operation by which to filter the category. The following operations are possible:</p> <ul> <li> <p> <code>CO</code> \u2013 Contains</p> </li> <li> <p> <code>EQ</code> \u2013 Equals</p> </li> <li> <p> <code>GT</code> \u2013 Greater than</p> </li> <li> <p> <code>LT</code> \u2013 Less than</p> </li> </ul> <p>The operators that each filter supports are listed below:</p> <ul> <li> <p> <code>BotAlias</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>BotVersion</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>LocaleId</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>Modality</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>Channel</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>SessionId</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>OriginatingRequestId</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>UtteranceState</code> \u2013 <code>EQ</code>.</p> </li> <li> <p> <code>UtteranceText</code> \u2013 <code>EQ</code>, <code>CO</code>.</p> </li> </ul>",
+                    "shape": "AnalyticsFilterOperator"
+                },
+                "values": {
+                    "documentation": "<p>An array containing the values of the category by which to apply the operator to filter the results. You can provide multiple values if the operator is <code>EQ</code> or <code>CO</code>. If you provide multiple values, you filter for results that equal/contain any of the values. For example, if the <code>name</code>, <code>operator</code>, and <code>values</code> fields are <code>Modality</code>, <code>EQ</code>, and <code>[Speech, Text]</code>, the operation filters for results where the modality was either <code>Speech</code> or <code>Text</code>.</p>",
+                    "shape": "AnalyticsFilterValues"
+                }
+            },
+            "required": [
+                "name",
+                "operator",
+                "values"
+            ],
+            "type": "structure"
+        },
+        "AnalyticsUtteranceFilterName": {
+            "enum": [
+                "BotAliasId",
+                "BotVersion",
+                "LocaleId",
+                "Modality",
+                "Channel",
+                "SessionId",
+                "OriginatingRequestId",
+                "UtteranceState",
+                "UtteranceText"
+            ],
+            "type": "string"
+        },
+        "AnalyticsUtteranceFilters": {
+            "max": 9,
+            "member": {
+                "shape": "AnalyticsUtteranceFilter"
+            },
+            "min": 1,
+            "type": "list"
+        },
+        "AnalyticsUtteranceGroupByKey": {
+            "documentation": "<p>Contains the category by which the utterance analytics were grouped and the values for that category.</p>",
+            "members": {
+                "name": {
+                    "documentation": "<p>The category by which the utterance analytics were grouped.</p>",
+                    "shape": "AnalyticsUtteranceField"
+                },
+                "value": {
+                    "documentation": "<p>A member of the category by which the utterance analytics were grouped.</p>",
+                    "shape": "AnalyticsGroupByValue"
+                }
+            },
+            "type": "structure"
+        },
+        "AnalyticsUtteranceGroupByKeys": {
+            "member": {
+                "shape": "AnalyticsUtteranceGroupByKey"
+            },
+            "type": "list"
+        },
+        "AnalyticsUtteranceGroupByList": {
+            "max": 2,
+            "member": {
+                "shape": "AnalyticsUtteranceGroupBySpecification"
+            },
+            "min": 1,
+            "type": "list"
+        },
+        "AnalyticsUtteranceGroupBySpecification": {
+            "documentation": "<p>Contains the category by which to group the utterances.</p>",
+            "members": {
+                "name": {
+                    "documentation": "<p>Specifies whether to group the utterances by their text or their state.</p>",
+                    "shape": "AnalyticsUtteranceField"
+                }
+            },
+            "required": [
+                "name"
+            ],
+            "type": "structure"
+        },
+        "AnalyticsUtteranceMetric": {
+            "documentation": "<p>Contains the metric and the summary statistic you want to calculate, and the order in which to sort the results, for the utterances across the user sessions with the bot.</p>",
+            "members": {
+                "name": {
+                    "documentation": "<p>The metric for which you want to get utterance summary statistics.</p> <ul> <li> <p> <code>Count</code> \u2013 The number of utterances.</p> </li> <li> <p> <code>Missed</code> \u2013 The number of utterances that Amazon Lex failed to recognize.</p> </li> <li> <p> <code>Detected</code> \u2013 The number of utterances that Amazon Lex managed to detect.</p> </li> <li> <p> <code>UtteranceTimestamp</code> \u2013 The date and time of the utterance.</p> </li> </ul>",
+                    "shape": "AnalyticsUtteranceMetricName"
+                },
+                "order": {
+                    "documentation": "<p>Specifies whether to sort the results in ascending or descending order.</p>",
+                    "shape": "AnalyticsSortOrder"
+                },
+                "statistic": {
+                    "documentation": "<p>The summary statistic to calculate.</p> <ul> <li> <p> <code>Sum</code> \u2013 The total count for the category you provide in <code>name</code>.</p> </li> <li> <p> <code>Average</code> \u2013 The total count divided by the number of utterances in the category you provide in <code>name</code>.</p> </li> <li> <p> <code>Max</code> \u2013 The highest count in the category you provide in <code>name</code>.</p> </li> </ul>",
+                    "shape": "AnalyticsMetricStatistic"
+                }
+            },
+            "required": [
+                "name",
+                "statistic"
+            ],
+            "type": "structure"
+        },
+        "AnalyticsUtteranceMetricName": {
+            "enum": [
+                "Count",
+                "Missed",
+                "Detected",
+                "UtteranceTimestamp"
+            ],
+            "type": "string"
+        },
+        "AnalyticsUtteranceMetricResult": {
+            "documentation": "<p>An object containing the results for the utterance metric you requested.</p>",
+            "members": {
+                "name": {
+                    "documentation": "<p>The metric that you requested.</p> <ul> <li> <p> <code>Count</code> \u2013 The number of utterances.</p> </li> <li> <p> <code>Missed</code> \u2013 The number of utterances that Amazon Lex failed to recognize.</p> </li> <li> <p> <code>Detected</code> \u2013 The number of utterances that Amazon Lex managed to detect.</p> </li> <li> <p> <code>UtteranceTimeStamp</code> \u2013 The date and time of the utterance.</p> </li> </ul>",
+                    "shape": "AnalyticsUtteranceMetricName"
+                },
+                "statistic": {
+                    "documentation": "<p>The summary statistic that you requested to calculate.</p> <ul> <li> <p> <code>Sum</code> \u2013 The total count for the category you provide in <code>name</code>.</p> </li> <li> <p> <code>Average</code> \u2013 The total count divided by the number of utterances in the category you provide in <code>name</code>.</p> </li> <li> <p> <code>Max</code> \u2013 The highest count in the category you provide in <code>name</code>.</p> </li> </ul>",
+                    "shape": "AnalyticsMetricStatistic"
+                },
+                "value": {
+                    "documentation": "<p>The value of the summary statistic for the metric that you requested.</p>",
+                    "shape": "AnalyticsMetricValue"
+                }
+            },
+            "type": "structure"
+        },
+        "AnalyticsUtteranceMetricResults": {
+            "member": {
+                "shape": "AnalyticsUtteranceMetricResult"
+            },
+            "type": "list"
+        },
+        "AnalyticsUtteranceMetrics": {
+            "max": 4,
+            "member": {
+                "shape": "AnalyticsUtteranceMetric"
+            },
+            "min": 1,
+            "type": "list"
+        },
+        "AnalyticsUtteranceResult": {
+            "documentation": "<p>An object containing the results for the utterance metrics you requested and the bin and/or group(s) they refer to, if applicable.</p>",
+            "members": {
+                "attributeResults": {
+                    "documentation": "<p>A list of objects containing information about the last used intent at the time of an utterance.</p>",
+                    "shape": "AnalyticsUtteranceAttributeResults"
+                },
+                "binKeys": {
+                    "documentation": "<p>A list of objects containing the criteria you requested for binning results and the values of the bins.</p>",
+                    "shape": "AnalyticsBinKeys"
+                },
+                "groupByKeys": {
+                    "documentation": "<p>A list of objects containing the criteria you requested for grouping results and the values of the bins.</p>",
+                    "shape": "AnalyticsUtteranceGroupByKeys"
+                },
+                "metricsResults": {
+                    "documentation": "<p>A list of objects, each of which contains a metric you want to list, the statistic for the metric you want to return, and the method by which to organize the results.</p>",
+                    "shape": "AnalyticsUtteranceMetricResults"
+                }
+            },
+            "type": "structure"
+        },
+        "AnalyticsUtteranceResults": {
+            "member": {
+                "shape": "AnalyticsUtteranceResult"
+            },
+            "type": "list"
+        },
+        "AnalyticsUtteranceSortByName": {
+            "enum": [
+                "UtteranceTimestamp"
+            ],
+            "type": "string"
+        },
         "AssociatedTranscript": {
             "documentation": "<p>The object containing information that associates the recommended intent/slot type with a conversation.</p>",
             "members": {
                 "transcript": {
                     "documentation": "<p>The content of the transcript that meets the search filter criteria. For the JSON format of the transcript, see <a href=\"https://docs.aws.amazon.com/lexv2/latest/dg/designing-output-format.html\">Output transcript format</a>.</p>",
                     "shape": "Transcript"
                 }
@@ -3430,14 +4665,22 @@
             "required": [
                 "botId",
                 "botAliasId",
                 "localeId"
             ],
             "type": "structure"
         },
+        "BotChannelType": {
+            "enum": [
+                "Facebook",
+                "Slack",
+                "TwilioSms"
+            ],
+            "type": "string"
+        },
         "BotExportSpecification": {
             "documentation": "<p>Provides the identity of a the bot that was exported.</p>",
             "members": {
                 "botId": {
                     "documentation": "<p>The identifier of the bot assigned by Amazon Lex.</p>",
                     "shape": "Id"
                 },
@@ -4400,14 +5643,22 @@
             "type": "integer"
         },
         "ContextTurnsToLive": {
             "max": 20,
             "min": 1,
             "type": "integer"
         },
+        "ConversationEndState": {
+            "enum": [
+                "Success",
+                "Failure",
+                "Dropped"
+            ],
+            "type": "string"
+        },
         "ConversationLevelIntentClassificationResultItem": {
             "documentation": "<p>The item listing the evaluation of intent level success or failure.</p>",
             "members": {
                 "intentName": {
                     "documentation": "<p>The intent name used in the evaluation of intent level success or failure.</p>",
                     "shape": "Name"
                 },
@@ -8442,14 +9693,25 @@
             },
             "required": [
                 "attribute",
                 "order"
             ],
             "type": "structure"
         },
+        "IntentState": {
+            "enum": [
+                "Failed",
+                "Fulfilled",
+                "InProgress",
+                "ReadyForFulfillment",
+                "Waiting",
+                "FulfillmentInProgress"
+            ],
+            "type": "string"
+        },
         "IntentStatistics": {
             "documentation": "<p>The object that contains the statistical summary of recommended intents associated with the bot recommendation.</p>",
             "members": {
                 "discoveredIntentCount": {
                     "documentation": "<p>The number of recommended intents associated with the bot recommendation.</p>",
                     "shape": "Count"
                 }
@@ -8506,14 +9768,30 @@
             "members": {
                 "message": {
                     "shape": "ExceptionMessage"
                 }
             },
             "type": "structure"
         },
+        "InvokedIntentSample": {
+            "documentation": "<p>An object containing the name of an intent that was invoked.</p>",
+            "members": {
+                "intentName": {
+                    "documentation": "<p>The name of an intent that was invoked.</p>",
+                    "shape": "Name"
+                }
+            },
+            "type": "structure"
+        },
+        "InvokedIntentSamples": {
+            "member": {
+                "shape": "InvokedIntentSample"
+            },
+            "type": "list"
+        },
         "ItemId": {
             "max": 32,
             "min": 1,
             "type": "string"
         },
         "KendraConfiguration": {
             "documentation": "<p>Provides configuration information for the <code>AMAZON.KendraSearchIntent</code> intent. When you use this intent, Amazon Lex searches the specified Amazon Kendra index and returns documents from the index that match the user's utterance.</p>",
@@ -9169,14 +10447,188 @@
                 "nextToken": {
                     "documentation": "<p>A token that indicates whether there are more results to return in a response to the <code>ListImports</code> operation. If the <code>nextToken</code> field is present, you send the contents as the <code>nextToken</code> parameter of a <code>ListImports</code> operation request to get the next page of results.</p>",
                     "shape": "NextToken"
                 }
             },
             "type": "structure"
         },
+        "ListIntentMetricsRequest": {
+            "members": {
+                "binBy": {
+                    "documentation": "<p>A list of objects, each of which contains specifications for organizing the results by time.</p>",
+                    "shape": "AnalyticsBinByList"
+                },
+                "botId": {
+                    "documentation": "<p>The identifier for the bot for which you want to retrieve intent metrics.</p>",
+                    "location": "uri",
+                    "locationName": "botId",
+                    "shape": "Id"
+                },
+                "endDateTime": {
+                    "documentation": "<p>The date and time that marks the end of the range of time for which you want to see intent metrics.</p>",
+                    "shape": "Timestamp"
+                },
+                "filters": {
+                    "documentation": "<p>A list of objects, each of which describes a condition by which you want to filter the results.</p>",
+                    "shape": "AnalyticsIntentFilters"
+                },
+                "groupBy": {
+                    "documentation": "<p>A list of objects, each of which specifies how to group the results. You can group by the following criteria:</p> <ul> <li> <p> <code>IntentName</code> \u2013 The name of the intent.</p> </li> <li> <p> <code>IntentEndState</code> \u2013 The final state of the intent. The possible end states are detailed in <a href=\"https://docs.aws.amazon.com/analytics-key-definitions-intents\">Key definitions</a> in the user guide.</p> </li> </ul>",
+                    "shape": "AnalyticsIntentGroupByList"
+                },
+                "maxResults": {
+                    "documentation": "<p>The maximum number of results to return in each page of results. If there are fewer results than the maximum page size, only the actual number of results are returned.</p>",
+                    "shape": "MaxResults"
+                },
+                "metrics": {
+                    "documentation": "<p>A list of objects, each of which contains a metric you want to list, the statistic for the metric you want to return, and the order by which to organize the results.</p>",
+                    "shape": "AnalyticsIntentMetrics"
+                },
+                "nextToken": {
+                    "documentation": "<p>If the response from the ListIntentMetrics operation contains more results than specified in the maxResults parameter, a token is returned in the response.</p> <p>Use the returned token in the nextToken parameter of a ListIntentMetrics request to return the next page of results. For a complete set of results, call the ListIntentMetrics operation until the nextToken returned in the response is null.</p>",
+                    "shape": "NextToken"
+                },
+                "startDateTime": {
+                    "documentation": "<p>The timestamp that marks the beginning of the range of time for which you want to see intent metrics.</p>",
+                    "shape": "Timestamp"
+                }
+            },
+            "required": [
+                "botId",
+                "startDateTime",
+                "endDateTime",
+                "metrics"
+            ],
+            "type": "structure"
+        },
+        "ListIntentMetricsResponse": {
+            "members": {
+                "botId": {
+                    "documentation": "<p>The identifier for the bot for which you retrieved intent metrics.</p>",
+                    "shape": "Id"
+                },
+                "nextToken": {
+                    "documentation": "<p>If the response from the ListIntentMetrics operation contains more results than specified in the maxResults parameter, a token is returned in the response.</p> <p>Use the returned token in the nextToken parameter of a ListIntentMetrics request to return the next page of results. For a complete set of results, call the ListIntentMetrics operation until the nextToken returned in the response is null.</p>",
+                    "shape": "NextToken"
+                },
+                "results": {
+                    "documentation": "<p>The results for the intent metrics.</p>",
+                    "shape": "AnalyticsIntentResults"
+                }
+            },
+            "type": "structure"
+        },
+        "ListIntentPathsRequest": {
+            "members": {
+                "botId": {
+                    "documentation": "<p>The identifier for the bot for which you want to retrieve intent path metrics.</p>",
+                    "location": "uri",
+                    "locationName": "botId",
+                    "shape": "Id"
+                },
+                "endDateTime": {
+                    "documentation": "<p>The date and time that marks the end of the range of time for which you want to see intent path metrics.</p>",
+                    "shape": "Timestamp"
+                },
+                "filters": {
+                    "documentation": "<p>A list of objects, each describes a condition by which you want to filter the results.</p>",
+                    "shape": "AnalyticsPathFilters"
+                },
+                "intentPath": {
+                    "documentation": "<p>The intent path for which you want to retrieve metrics. Use a forward slash to separate intents in the path. For example:</p> <ul> <li> <p>/BookCar</p> </li> <li> <p>/BookCar/BookHotel</p> </li> <li> <p>/BookHotel/BookCar</p> </li> </ul>",
+                    "shape": "AnalyticsPath"
+                },
+                "startDateTime": {
+                    "documentation": "<p>The date and time that marks the beginning of the range of time for which you want to see intent path metrics.</p>",
+                    "shape": "Timestamp"
+                }
+            },
+            "required": [
+                "botId",
+                "startDateTime",
+                "endDateTime",
+                "intentPath"
+            ],
+            "type": "structure"
+        },
+        "ListIntentPathsResponse": {
+            "members": {
+                "nodeSummaries": {
+                    "documentation": "<p>A list of objects, each of which contains information about a node in the intent path for which you requested metrics.</p>",
+                    "shape": "AnalyticsIntentNodeSummaries"
+                }
+            },
+            "type": "structure"
+        },
+        "ListIntentStageMetricsRequest": {
+            "members": {
+                "binBy": {
+                    "documentation": "<p>A list of objects, each of which contains specifications for organizing the results by time.</p>",
+                    "shape": "AnalyticsBinByList"
+                },
+                "botId": {
+                    "documentation": "<p>The identifier for the bot for which you want to retrieve intent stage metrics.</p>",
+                    "location": "uri",
+                    "locationName": "botId",
+                    "shape": "Id"
+                },
+                "endDateTime": {
+                    "documentation": "<p>The date and time that marks the end of the range of time for which you want to see intent stage metrics.</p>",
+                    "shape": "Timestamp"
+                },
+                "filters": {
+                    "documentation": "<p>A list of objects, each of which describes a condition by which you want to filter the results.</p>",
+                    "shape": "AnalyticsIntentStageFilters"
+                },
+                "groupBy": {
+                    "documentation": "<p>A list of objects, each of which specifies how to group the results. You can group by the following criteria:</p> <ul> <li> <p> <code>IntentStageName</code> \u2013 The name of the intent stage.</p> </li> <li> <p> <code>SwitchedToIntent</code> \u2013 The intent to which the conversation was switched (if any).</p> </li> </ul>",
+                    "shape": "AnalyticsIntentStageGroupByList"
+                },
+                "maxResults": {
+                    "documentation": "<p>The maximum number of results to return in each page of results. If there are fewer results than the maximum page size, only the actual number of results are returned.</p>",
+                    "shape": "MaxResults"
+                },
+                "metrics": {
+                    "documentation": "<p>A list of objects, each of which contains a metric you want to list, the statistic for the metric you want to return, and the method by which to organize the results.</p>",
+                    "shape": "AnalyticsIntentStageMetrics"
+                },
+                "nextToken": {
+                    "documentation": "<p>If the response from the ListIntentStageMetrics operation contains more results than specified in the maxResults parameter, a token is returned in the response.</p> <p>Use the returned token in the nextToken parameter of a ListIntentStageMetrics request to return the next page of results. For a complete set of results, call the ListIntentStageMetrics operation until the nextToken returned in the response is null.</p>",
+                    "shape": "NextToken"
+                },
+                "startDateTime": {
+                    "documentation": "<p>The date and time that marks the beginning of the range of time for which you want to see intent stage metrics.</p>",
+                    "shape": "Timestamp"
+                }
+            },
+            "required": [
+                "botId",
+                "startDateTime",
+                "endDateTime",
+                "metrics"
+            ],
+            "type": "structure"
+        },
+        "ListIntentStageMetricsResponse": {
+            "members": {
+                "botId": {
+                    "documentation": "<p>The identifier for the bot for which you retrieved intent stage metrics.</p>",
+                    "shape": "Id"
+                },
+                "nextToken": {
+                    "documentation": "<p>If the response from the ListIntentStageMetrics operation contains more results than specified in the maxResults parameter, a token is returned in the response.</p> <p>Use the returned token in the nextToken parameter of a ListIntentStageMetrics request to return the next page of results. For a complete set of results, call the ListIntentStageMetrics operation until the nextToken returned in the response is null.</p>",
+                    "shape": "NextToken"
+                },
+                "results": {
+                    "documentation": "<p>The results for the intent stage metrics.</p>",
+                    "shape": "AnalyticsIntentStageResults"
+                }
+            },
+            "type": "structure"
+        },
         "ListIntentsRequest": {
             "members": {
                 "botId": {
                     "documentation": "<p>The unique identifier of the bot that contains the intent.</p>",
                     "location": "uri",
                     "locationName": "botId",
                     "shape": "Id"
@@ -9310,14 +10762,137 @@
                 "summaryList": {
                     "documentation": "<p>Summary information for the intents that meet the filter criteria specified in the request. The length of the list is specified in the maxResults parameter of the request. If there are more intents available, the nextToken field contains a token to get the next page of results.</p>",
                     "shape": "RecommendedIntentSummaryList"
                 }
             },
             "type": "structure"
         },
+        "ListSessionAnalyticsDataRequest": {
+            "members": {
+                "botId": {
+                    "documentation": "<p>The identifier for the bot for which you want to retrieve session analytics.</p>",
+                    "location": "uri",
+                    "locationName": "botId",
+                    "shape": "Id"
+                },
+                "endDateTime": {
+                    "documentation": "<p>The date and time that marks the end of the range of time for which you want to see session analytics.</p>",
+                    "shape": "Timestamp"
+                },
+                "filters": {
+                    "documentation": "<p>A list of objects, each of which describes a condition by which you want to filter the results.</p>",
+                    "shape": "AnalyticsSessionFilters"
+                },
+                "maxResults": {
+                    "documentation": "<p>The maximum number of results to return in each page of results. If there are fewer results than the maximum page size, only the actual number of results are returned.</p>",
+                    "shape": "MaxResults"
+                },
+                "nextToken": {
+                    "documentation": "<p>If the response from the ListSessionAnalyticsData operation contains more results than specified in the maxResults parameter, a token is returned in the response.</p> <p>Use the returned token in the nextToken parameter of a ListSessionAnalyticsData request to return the next page of results. For a complete set of results, call the ListSessionAnalyticsData operation until the nextToken returned in the response is null.</p>",
+                    "shape": "NextToken"
+                },
+                "sortBy": {
+                    "documentation": "<p>An object specifying the measure and method by which to sort the session analytics data.</p>",
+                    "shape": "SessionDataSortBy"
+                },
+                "startDateTime": {
+                    "documentation": "<p>The date and time that marks the beginning of the range of time for which you want to see session analytics.</p>",
+                    "shape": "Timestamp"
+                }
+            },
+            "required": [
+                "botId",
+                "startDateTime",
+                "endDateTime"
+            ],
+            "type": "structure"
+        },
+        "ListSessionAnalyticsDataResponse": {
+            "members": {
+                "botId": {
+                    "documentation": "<p>The unique identifier of the bot that the sessions belong to.</p>",
+                    "shape": "Id"
+                },
+                "nextToken": {
+                    "documentation": "<p>If the response from the ListSessionAnalyticsData operation contains more results than specified in the maxResults parameter, a token is returned in the response.</p> <p>Use the returned token in the nextToken parameter of a ListSessionAnalyticsData request to return the next page of results. For a complete set of results, call the ListSessionAnalyticsData operation until the nextToken returned in the response is null.</p>",
+                    "shape": "NextToken"
+                },
+                "sessions": {
+                    "documentation": "<p>A list of objects, each of which contains information about a session with the bot.</p>",
+                    "shape": "SessionSpecifications"
+                }
+            },
+            "type": "structure"
+        },
+        "ListSessionMetricsRequest": {
+            "members": {
+                "binBy": {
+                    "documentation": "<p>A list of objects, each of which contains specifications for organizing the results by time.</p>",
+                    "shape": "AnalyticsBinByList"
+                },
+                "botId": {
+                    "documentation": "<p>The identifier for the bot for which you want to retrieve session metrics.</p>",
+                    "location": "uri",
+                    "locationName": "botId",
+                    "shape": "Id"
+                },
+                "endDateTime": {
+                    "documentation": "<p>The date and time that marks the end of the range of time for which you want to see session metrics.</p>",
+                    "shape": "Timestamp"
+                },
+                "filters": {
+                    "documentation": "<p>A list of objects, each of which describes a condition by which you want to filter the results.</p>",
+                    "shape": "AnalyticsSessionFilters"
+                },
+                "groupBy": {
+                    "documentation": "<p>A list of objects, each of which specifies how to group the results. You can group by the following criteria:</p> <ul> <li> <p> <code>ConversationEndState</code> \u2013 The final state of the conversation. The possible end states are detailed in <a href=\"https://docs.aws.amazon.com/analytics-key-definitions-conversations\">Key definitions</a> in the user guide.</p> </li> <li> <p> <code>LocaleId</code> \u2013 The unique identifier of the bot locale.</p> </li> </ul>",
+                    "shape": "AnalyticsSessionGroupByList"
+                },
+                "maxResults": {
+                    "documentation": "<p>The maximum number of results to return in each page of results. If there are fewer results than the maximum page size, only the actual number of results are returned.</p>",
+                    "shape": "MaxResults"
+                },
+                "metrics": {
+                    "documentation": "<p>A list of objects, each of which contains a metric you want to list, the statistic for the metric you want to return, and the method by which to organize the results.</p>",
+                    "shape": "AnalyticsSessionMetrics"
+                },
+                "nextToken": {
+                    "documentation": "<p>If the response from the ListSessionMetrics operation contains more results than specified in the maxResults parameter, a token is returned in the response.</p> <p>Use the returned token in the nextToken parameter of a ListSessionMetrics request to return the next page of results. For a complete set of results, call the ListSessionMetrics operation until the nextToken returned in the response is null.</p>",
+                    "shape": "NextToken"
+                },
+                "startDateTime": {
+                    "documentation": "<p>The date and time that marks the beginning of the range of time for which you want to see session metrics.</p>",
+                    "shape": "Timestamp"
+                }
+            },
+            "required": [
+                "botId",
+                "startDateTime",
+                "endDateTime",
+                "metrics"
+            ],
+            "type": "structure"
+        },
+        "ListSessionMetricsResponse": {
+            "members": {
+                "botId": {
+                    "documentation": "<p>The identifier for the bot for which you retrieved session metrics.</p>",
+                    "shape": "Id"
+                },
+                "nextToken": {
+                    "documentation": "<p>If the response from the ListSessionMetrics operation contains more results than specified in the maxResults parameter, a token is returned in the response.</p> <p>Use the returned token in the nextToken parameter of a ListSessionMetrics request to return the next page of results. For a complete set of results, call the ListSessionMetrics operation until the nextToken returned in the response is null.</p>",
+                    "shape": "NextToken"
+                },
+                "results": {
+                    "documentation": "<p>The results for the session metrics.</p>",
+                    "shape": "AnalyticsSessionResults"
+                }
+            },
+            "type": "structure"
+        },
         "ListSlotTypesRequest": {
             "members": {
                 "botId": {
                     "documentation": "<p>The unique identifier of the bot that contains the slot types.</p>",
                     "location": "uri",
                     "locationName": "botId",
                     "shape": "Id"
@@ -9617,14 +11192,141 @@
                 "testSets": {
                     "documentation": "<p>The selected test sets in a list of test sets.</p>",
                     "shape": "TestSetSummaryList"
                 }
             },
             "type": "structure"
         },
+        "ListUtteranceAnalyticsDataRequest": {
+            "members": {
+                "botId": {
+                    "documentation": "<p>The identifier for the bot for which you want to retrieve utterance analytics.</p>",
+                    "location": "uri",
+                    "locationName": "botId",
+                    "shape": "Id"
+                },
+                "endDateTime": {
+                    "documentation": "<p>The date and time that marks the end of the range of time for which you want to see utterance analytics.</p>",
+                    "shape": "Timestamp"
+                },
+                "filters": {
+                    "documentation": "<p>A list of objects, each of which describes a condition by which you want to filter the results.</p>",
+                    "shape": "AnalyticsUtteranceFilters"
+                },
+                "maxResults": {
+                    "documentation": "<p>The maximum number of results to return in each page of results. If there are fewer results than the maximum page size, only the actual number of results are returned.</p>",
+                    "shape": "MaxResults"
+                },
+                "nextToken": {
+                    "documentation": "<p>If the response from the ListUtteranceAnalyticsData operation contains more results than specified in the maxResults parameter, a token is returned in the response.</p> <p>Use the returned token in the nextToken parameter of a ListUtteranceAnalyticsData request to return the next page of results. For a complete set of results, call the ListUtteranceAnalyticsData operation until the nextToken returned in the response is null.</p>",
+                    "shape": "NextToken"
+                },
+                "sortBy": {
+                    "documentation": "<p>An object specifying the measure and method by which to sort the utterance analytics data.</p>",
+                    "shape": "UtteranceDataSortBy"
+                },
+                "startDateTime": {
+                    "documentation": "<p>The date and time that marks the beginning of the range of time for which you want to see utterance analytics.</p>",
+                    "shape": "Timestamp"
+                }
+            },
+            "required": [
+                "botId",
+                "startDateTime",
+                "endDateTime"
+            ],
+            "type": "structure"
+        },
+        "ListUtteranceAnalyticsDataResponse": {
+            "members": {
+                "botId": {
+                    "documentation": "<p>The unique identifier of the bot that the utterances belong to.</p>",
+                    "shape": "Id"
+                },
+                "nextToken": {
+                    "documentation": "<p>If the response from the ListUtteranceAnalyticsData operation contains more results than specified in the maxResults parameter, a token is returned in the response.</p> <p>Use the returned token in the nextToken parameter of a ListUtteranceAnalyticsData request to return the next page of results. For a complete set of results, call the ListUtteranceAnalyticsData operation until the nextToken returned in the response is null.</p>",
+                    "shape": "NextToken"
+                },
+                "utterances": {
+                    "documentation": "<p>A list of objects, each of which contains information about an utterance in a user session with your bot.</p>",
+                    "shape": "UtteranceSpecifications"
+                }
+            },
+            "type": "structure"
+        },
+        "ListUtteranceMetricsRequest": {
+            "members": {
+                "attributes": {
+                    "documentation": "<p>A list containing attributes related to the utterance that you want the response to return. The following attributes are possible:</p> <ul> <li> <p> <code>LastUsedIntent</code> \u2013 The last used intent at the time of the utterance.</p> </li> </ul>",
+                    "shape": "AnalyticsUtteranceAttributes"
+                },
+                "binBy": {
+                    "documentation": "<p>A list of objects, each of which contains specifications for organizing the results by time.</p>",
+                    "shape": "AnalyticsBinByList"
+                },
+                "botId": {
+                    "documentation": "<p>The identifier for the bot for which you want to retrieve utterance metrics.</p>",
+                    "location": "uri",
+                    "locationName": "botId",
+                    "shape": "Id"
+                },
+                "endDateTime": {
+                    "documentation": "<p>The date and time that marks the end of the range of time for which you want to see utterance metrics.</p>",
+                    "shape": "Timestamp"
+                },
+                "filters": {
+                    "documentation": "<p>A list of objects, each of which describes a condition by which you want to filter the results.</p>",
+                    "shape": "AnalyticsUtteranceFilters"
+                },
+                "groupBy": {
+                    "documentation": "<p>A list of objects, each of which specifies how to group the results. You can group by the following criteria:</p> <ul> <li> <p> <code>UtteranceText</code> \u2013 The transcription of the utterance.</p> </li> <li> <p> <code>UtteranceState</code> \u2013 The state of the utterance. The possible states are detailed in <a href=\"https://docs.aws.amazon.com/analytics-key-definitions-utterances\">Key definitions</a> in the user guide.</p> </li> </ul>",
+                    "shape": "AnalyticsUtteranceGroupByList"
+                },
+                "maxResults": {
+                    "documentation": "<p>The maximum number of results to return in each page of results. If there are fewer results than the maximum page size, only the actual number of results are returned.</p>",
+                    "shape": "MaxResults"
+                },
+                "metrics": {
+                    "documentation": "<p>A list of objects, each of which contains a metric you want to list, the statistic for the metric you want to return, and the method by which to organize the results.</p>",
+                    "shape": "AnalyticsUtteranceMetrics"
+                },
+                "nextToken": {
+                    "documentation": "<p>If the response from the ListUtteranceMetrics operation contains more results than specified in the maxResults parameter, a token is returned in the response.</p> <p>Use the returned token in the nextToken parameter of a ListUtteranceMetrics request to return the next page of results. For a complete set of results, call the ListUtteranceMetrics operation until the nextToken returned in the response is null.</p>",
+                    "shape": "NextToken"
+                },
+                "startDateTime": {
+                    "documentation": "<p>The date and time that marks the beginning of the range of time for which you want to see utterance metrics.</p>",
+                    "shape": "Timestamp"
+                }
+            },
+            "required": [
+                "botId",
+                "startDateTime",
+                "endDateTime",
+                "metrics"
+            ],
+            "type": "structure"
+        },
+        "ListUtteranceMetricsResponse": {
+            "members": {
+                "botId": {
+                    "documentation": "<p>The identifier for the bot for which you retrieved utterance metrics.</p>",
+                    "shape": "Id"
+                },
+                "nextToken": {
+                    "documentation": "<p>If the response from the ListUtteranceMetrics operation contains more results than specified in the maxResults parameter, a token is returned in the response.</p> <p>Use the returned token in the nextToken parameter of a ListUtteranceMetrics request to return the next page of results. For a complete set of results, call the ListUtteranceMetrics operation until the nextToken returned in the response is null.</p>",
+                    "shape": "NextToken"
+                },
+                "results": {
+                    "documentation": "<p>The results for the utterance metrics.</p>",
+                    "shape": "AnalyticsUtteranceResults"
+                }
+            },
+            "type": "structure"
+        },
         "LocaleId": {
             "type": "string"
         },
         "LocaleName": {
             "type": "string"
         },
         "LogPrefix": {
@@ -10571,20 +12273,102 @@
             "members": {
                 "message": {
                     "shape": "ExceptionMessage"
                 }
             },
             "type": "structure"
         },
+        "SessionDataSortBy": {
+            "documentation": "<p>An object specifying the measure and method by which to sort the session analytics data.</p>",
+            "members": {
+                "name": {
+                    "documentation": "<p>The measure by which to sort the session analytics data.</p> <ul> <li> <p> <code>conversationStartTime</code> \u2013 The date and time when the conversation began. A conversation is defined as a unique combination of a <code>sessionId</code> and an <code>originatingRequestId</code>.</p> </li> <li> <p> <code>numberOfTurns</code> \u2013 The number of turns that the session took.</p> </li> <li> <p> <code>conversationDurationSeconds</code> \u2013 The duration of the conversation in seconds.</p> </li> </ul>",
+                    "shape": "AnalyticsSessionSortByName"
+                },
+                "order": {
+                    "documentation": "<p>Specifies whether to sort the results in ascending or descending order.</p>",
+                    "shape": "AnalyticsSortOrder"
+                }
+            },
+            "required": [
+                "name",
+                "order"
+            ],
+            "type": "structure"
+        },
         "SessionId": {
             "max": 100,
             "min": 2,
             "pattern": "[0-9a-zA-Z._:-]+",
             "type": "string"
         },
+        "SessionSpecification": {
+            "documentation": "<p>An object containing information about a specific session.</p>",
+            "members": {
+                "botAliasId": {
+                    "documentation": "<p>The identifier of the alias of the bot that the session was held with.</p>",
+                    "shape": "BotAliasId"
+                },
+                "botVersion": {
+                    "documentation": "<p>The version of the bot that the session was held with.</p>",
+                    "shape": "NumericalBotVersion"
+                },
+                "channel": {
+                    "documentation": "<p>The channel that is integrated with the bot that the session was held with.</p>",
+                    "shape": "BotChannelType"
+                },
+                "conversationDurationSeconds": {
+                    "documentation": "<p>The duration of the conversation in seconds. A conversation is defined as a unique combination of a <code>sessionId</code> and an <code>originatingRequestId</code>.</p>",
+                    "shape": "AnalyticsLongValue"
+                },
+                "conversationEndState": {
+                    "documentation": "<p>The final state of the conversation. A conversation is defined as a unique combination of a <code>sessionId</code> and an <code>originatingRequestId</code>.</p>",
+                    "shape": "ConversationEndState"
+                },
+                "conversationEndTime": {
+                    "documentation": "<p>The date and time when the conversation ended. A conversation is defined as a unique combination of a <code>sessionId</code> and an <code>originatingRequestId</code>.</p>",
+                    "shape": "Timestamp"
+                },
+                "conversationStartTime": {
+                    "documentation": "<p>The date and time when the conversation began. A conversation is defined as a unique combination of a <code>sessionId</code> and an <code>originatingRequestId</code>.</p>",
+                    "shape": "Timestamp"
+                },
+                "invokedIntentSamples": {
+                    "documentation": "<p>A list of objects containing the name of an intent that was invoked.</p>",
+                    "shape": "InvokedIntentSamples"
+                },
+                "localeId": {
+                    "documentation": "<p>The locale of the bot that the session was held with.</p>",
+                    "shape": "LocaleId"
+                },
+                "mode": {
+                    "documentation": "<p>The mode of the session. The possible values are as follows:</p> <ul> <li> <p> <code>Speech</code> \u2013 The session was spoken.</p> </li> <li> <p> <code>Text</code> \u2013 The session was written.</p> </li> <li> <p> <code>DTMF</code> \u2013 The session used a touch-tone keypad (Dual Tone Multi-Frequency).</p> </li> <li> <p> <code>MultiMode</code> \u2013 The session used multiple modes.</p> </li> </ul>",
+                    "shape": "AnalyticsModality"
+                },
+                "numberOfTurns": {
+                    "documentation": "<p>The number of turns that the session took.</p>",
+                    "shape": "AnalyticsLongValue"
+                },
+                "originatingRequestId": {
+                    "documentation": "<p>The identifier of the first request in a session.</p>",
+                    "shape": "AnalyticsOriginatingRequestId"
+                },
+                "sessionId": {
+                    "documentation": "<p>The identifier of the session.</p>",
+                    "shape": "AnalyticsSessionId"
+                }
+            },
+            "type": "structure"
+        },
+        "SessionSpecifications": {
+            "member": {
+                "shape": "SessionSpecification"
+            },
+            "type": "list"
+        },
         "SessionTTL": {
             "max": 86400,
             "min": 60,
             "type": "integer"
         },
         "SkipResourceInUseCheck": {
             "type": "boolean"
@@ -13530,14 +15314,64 @@
                 }
             },
             "required": [
                 "audioFileS3Location"
             ],
             "type": "structure"
         },
+        "UtteranceBotResponse": {
+            "documentation": "<p>An object that contains a response to the utterance from the bot.</p>",
+            "members": {
+                "content": {
+                    "documentation": "<p>The text of the response to the utterance from the bot.</p>",
+                    "shape": "String"
+                },
+                "contentType": {
+                    "documentation": "<p>The type of the response. The following values are possible:</p> <ul> <li> <p> <code>PlainText</code> \u2013 A plain text string.</p> </li> <li> <p> <code>CustomPayload</code> \u2013 A response string that you can customize to include data or metadata for your application.</p> </li> <li> <p> <code>SSML</code> \u2013 A string that includes Speech Synthesis Markup Language to customize the audio response.</p> </li> <li> <p> <code>ImageResponseCard</code> \u2013 An image with buttons that the customer can select. See <a href=\"https://docs.aws.amazon.com/lexv2/latest/APIReference/API_runtime_ImageResponseCard.html\">ImageResponseCard</a> for more information.</p> </li> </ul>",
+                    "shape": "UtteranceContentType"
+                },
+                "imageResponseCard": {
+                    "shape": "ImageResponseCard"
+                }
+            },
+            "type": "structure"
+        },
+        "UtteranceBotResponses": {
+            "member": {
+                "shape": "UtteranceBotResponse"
+            },
+            "type": "list"
+        },
+        "UtteranceContentType": {
+            "enum": [
+                "PlainText",
+                "CustomPayload",
+                "SSML",
+                "ImageResponseCard"
+            ],
+            "type": "string"
+        },
+        "UtteranceDataSortBy": {
+            "documentation": "<p>An object specifying the measure and method by which to sort the utterance data.</p>",
+            "members": {
+                "name": {
+                    "documentation": "<p>The measure by which to sort the utterance analytics data.</p> <ul> <li> <p> <code>Count</code> \u2013 The number of utterances.</p> </li> <li> <p> <code>UtteranceTimeStamp</code> \u2013 The date and time of the utterance.</p> </li> </ul>",
+                    "shape": "AnalyticsUtteranceSortByName"
+                },
+                "order": {
+                    "documentation": "<p>Specifies whether to sort the results in ascending or descending order.</p>",
+                    "shape": "AnalyticsSortOrder"
+                }
+            },
+            "required": [
+                "name",
+                "order"
+            ],
+            "type": "structure"
+        },
         "UtteranceInputSpecification": {
             "documentation": "<p>Contains information about input of an utterance.</p>",
             "members": {
                 "audioInput": {
                     "documentation": "<p>Contains information about the audio input for an utterance.</p>",
                     "shape": "UtteranceAudioInputSpecification"
                 },
@@ -13585,14 +15419,117 @@
                 }
             },
             "required": [
                 "items"
             ],
             "type": "structure"
         },
+        "UtteranceSpecification": {
+            "documentation": "<p>An object containing information about a specific utterance.</p>",
+            "members": {
+                "associatedIntentName": {
+                    "documentation": "<p>The name of the intent that the utterance is associated to.</p>",
+                    "shape": "Name"
+                },
+                "associatedSlotName": {
+                    "documentation": "<p>The name of the slot that the utterance is associated to.</p>",
+                    "shape": "Name"
+                },
+                "audioVoiceDurationMillis": {
+                    "documentation": "<p>The duration in milliseconds of the audio associated with the utterance.</p>",
+                    "shape": "AnalyticsLongValue"
+                },
+                "botAliasId": {
+                    "documentation": "<p>The identifier of the alias of the bot that the utterance was made to.</p>",
+                    "shape": "BotAliasId"
+                },
+                "botResponseAudioVoiceId": {
+                    "documentation": "<p>The identifier for the audio of the bot response.</p>",
+                    "shape": "String"
+                },
+                "botResponses": {
+                    "documentation": "<p>A list of objects containing information about the bot response to the utterance.</p>",
+                    "shape": "UtteranceBotResponses"
+                },
+                "botVersion": {
+                    "documentation": "<p>The version of the bot that the utterance was made to.</p>",
+                    "shape": "NumericalBotVersion"
+                },
+                "channel": {
+                    "documentation": "<p>The channel that is integrated with the bot that the utterance was made to.</p>",
+                    "shape": "BotChannelType"
+                },
+                "conversationEndTime": {
+                    "documentation": "<p>The date and time when the conversation in which the utterance took place ended. A conversation is defined as a unique combination of a <code>sessionId</code> and an <code>originatingRequestId</code>.</p>",
+                    "shape": "Timestamp"
+                },
+                "conversationStartTime": {
+                    "documentation": "<p>The date and time when the conversation in which the utterance took place began. A conversation is defined as a unique combination of a <code>sessionId</code> and an <code>originatingRequestId</code>.</p>",
+                    "shape": "Timestamp"
+                },
+                "dialogActionType": {
+                    "documentation": "<p>The type of dialog action that the utterance is associated to. See the <code>type</code> field in <a href=\"https://docs.aws.amazon.com/lexv2/latest/APIReference/API_runtime_DialogAction.html\">DialogAction</a> for more information.</p>",
+                    "shape": "String"
+                },
+                "inputType": {
+                    "documentation": "<p>The input type of the utterance. The possible values are as follows:</p> <ul> <li> <p>PCM format: audio data must be in little-endian byte order.</p> <ul> <li> <p> <code>audio/l16; rate=16000; channels=1</code> </p> </li> <li> <p> <code>audio/x-l16; sample-rate=16000; channel-count=1</code> </p> </li> <li> <p> <code>audio/lpcm; sample-rate=8000; sample-size-bits=16; channel-count=1; is-big-endian=false</code> </p> </li> </ul> </li> <li> <p>Opus format</p> <ul> <li> <p> <code>audio/x-cbr-opus-with-preamble;preamble-size=0;bit-rate=256000;frame-size-milliseconds=4</code> </p> </li> </ul> </li> <li> <p>Text format</p> <ul> <li> <p> <code>text/plain; charset=utf-8</code> </p> </li> </ul> </li> </ul>",
+                    "shape": "String"
+                },
+                "intentState": {
+                    "documentation": "<p>The state of the intent that the utterance is associated to.</p>",
+                    "shape": "IntentState"
+                },
+                "localeId": {
+                    "documentation": "<p>The locale of the bot that the utterance was made to.</p>",
+                    "shape": "LocaleId"
+                },
+                "mode": {
+                    "documentation": "<p>The mode of the session. The possible values are as follows:</p> <ul> <li> <p> <code>Speech</code> \u2013 The session consisted of spoken dialogue.</p> </li> <li> <p> <code>Text</code> \u2013 The session consisted of written dialogue.</p> </li> <li> <p> <code>DTMF</code> \u2013 The session consisted of touch-tone keypad (Dual Tone Multi-Frequency) key presses.</p> </li> <li> <p> <code>MultiMode</code> \u2013 The session consisted of multiple modes.</p> </li> </ul>",
+                    "shape": "AnalyticsModality"
+                },
+                "outputType": {
+                    "documentation": "<p>The output type of the utterance. The possible values are as follows:</p> <ul> <li> <p> <code>audio/mpeg</code> </p> </li> <li> <p> <code>audio/ogg</code> </p> </li> <li> <p> <code>audio/pcm (16 KHz)</code> </p> </li> <li> <p> <code>audio/</code> (defaults to <code>mpeg</code>)</p> </li> <li> <p> <code>text/plain; charset=utf-8</code> </p> </li> </ul>",
+                    "shape": "String"
+                },
+                "sessionId": {
+                    "documentation": "<p>The identifier of the session that the utterance was made in.</p>",
+                    "shape": "AnalyticsSessionId"
+                },
+                "slotsFilledInSession": {
+                    "documentation": "<p>The slots that have been filled in the session by the time of the utterance.</p>",
+                    "shape": "String"
+                },
+                "utterance": {
+                    "documentation": "<p>The text of the utterance.</p>",
+                    "shape": "String"
+                },
+                "utteranceRequestId": {
+                    "documentation": "<p>The identifier of the request associated with the utterance.</p>",
+                    "shape": "Id"
+                },
+                "utteranceTimestamp": {
+                    "documentation": "<p>The date and time when the utterance took place.</p>",
+                    "shape": "Timestamp"
+                },
+                "utteranceUnderstood": {
+                    "documentation": "<p>Specifies whether the bot understood the utterance or not.</p>",
+                    "shape": "UtteranceUnderstood"
+                }
+            },
+            "type": "structure"
+        },
+        "UtteranceSpecifications": {
+            "member": {
+                "shape": "UtteranceSpecification"
+            },
+            "type": "list"
+        },
+        "UtteranceUnderstood": {
+            "type": "boolean"
+        },
         "ValidationException": {
             "documentation": "<p>One of the input parameters in your request isn't valid. Check the parameters and try your request again.</p>",
             "error": {
                 "httpStatusCode": 400
             },
             "exception": true,
             "members": {
```

### Comparing `botocore-a-la-carte-lexv2-models-1.31.4/botocore/data/lexv2-models/2020-08-07/waiters-2.json` & `botocore-a-la-carte-lexv2-models-1.31.5/botocore/data/lexv2-models/2020-08-07/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-lexv2-models-1.31.4/botocore_a_la_carte_lexv2_models.egg-info/PKG-INFO` & `botocore-a-la-carte-lexv2-models-1.31.5/botocore_a_la_carte_lexv2_models.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-lexv2-models
-Version: 1.31.4
+Version: 1.31.5
 Summary: lexv2-models data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-lexv2-models-1.31.4/botocore_a_la_carte_lexv2_models.egg-info/SOURCES.txt` & `botocore-a-la-carte-lexv2-models-1.31.5/botocore_a_la_carte_lexv2_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-lexv2-models-1.31.4/setup.py` & `botocore-a-la-carte-lexv2-models-1.31.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-lexv2-models',
-    version="1.31.4",
+    version="1.31.5",
     description='lexv2-models data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/lexv2-models/*/*.json'],
```

