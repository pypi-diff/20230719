# Comparing `tmp/ignos-internal-api-client-20230702.0.5514.tar.gz` & `tmp/ignos-internal-api-client-20230719.0.5642.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ignos-internal-api-client-20230702.0.5514.tar", last modified: Sun Jul  2 17:29:03 2023, max compression
+gzip compressed data, was "ignos-internal-api-client-20230719.0.5642.tar", last modified: Wed Jul 19 08:34:34 2023, max compression
```

## Comparing `ignos-internal-api-client-20230702.0.5514.tar` & `ignos-internal-api-client-20230719.0.5642.tar`

### file list

```diff
@@ -1,42 +1,41 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-02 17:29:03.846091 ignos-internal-api-client-20230702.0.5514/
--rw-r--r--   0 vsts      (1001) docker     (123)      195 2023-07-02 17:29:03.846091 ignos-internal-api-client-20230702.0.5514/PKG-INFO
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-02 17:29:03.842091 ignos-internal-api-client-20230702.0.5514/ignos/
--rw-r--r--   0 vsts      (1001) docker     (123)       81 2023-07-02 17:28:48.000000 ignos-internal-api-client-20230702.0.5514/ignos/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-02 17:29:03.842091 ignos-internal-api-client-20230702.0.5514/ignos/internal/
--rw-r--r--   0 vsts      (1001) docker     (123)       81 2023-07-02 17:28:48.000000 ignos-internal-api-client-20230702.0.5514/ignos/internal/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-02 17:29:03.842091 ignos-internal-api-client-20230702.0.5514/ignos/internal/api/
--rw-r--r--   0 vsts      (1001) docker     (123)       81 2023-07-02 17:28:48.000000 ignos-internal-api-client-20230702.0.5514/ignos/internal/api/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-02 17:29:03.846091 ignos-internal-api-client-20230702.0.5514/ignos/internal/api/client/
--rw-r--r--   0 vsts      (1001) docker     (123)      876 2023-07-02 17:28:48.000000 ignos-internal-api-client-20230702.0.5514/ignos/internal/api/client/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6182 2023-07-02 17:28:48.000000 ignos-internal-api-client-20230702.0.5514/ignos/internal/api/client/_client.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2966 2023-07-02 17:28:48.000000 ignos-internal-api-client-20230702.0.5514/ignos/internal/api/client/_configuration.py
--rw-r--r--   0 vsts      (1001) docker     (123)      674 2023-07-02 17:28:48.000000 ignos-internal-api-client-20230702.0.5514/ignos/internal/api/client/_patch.py
--rw-r--r--   0 vsts      (1001) docker     (123)    78836 2023-07-02 17:28:48.000000 ignos-internal-api-client-20230702.0.5514/ignos/internal/api/client/_serialization.py
--rw-r--r--   0 vsts      (1001) docker     (123)      976 2023-07-02 17:28:48.000000 ignos-internal-api-client-20230702.0.5514/ignos/internal/api/client/_vendor.py
--rw-r--r--   0 vsts      (1001) docker     (123)      496 2023-07-02 17:28:48.000000 ignos-internal-api-client-20230702.0.5514/ignos/internal/api/client/_version.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-02 17:29:03.846091 ignos-internal-api-client-20230702.0.5514/ignos/internal/api/client/aio/
--rw-r--r--   0 vsts      (1001) docker     (123)      823 2023-07-02 17:28:48.000000 ignos-internal-api-client-20230702.0.5514/ignos/internal/api/client/aio/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6358 2023-07-02 17:28:48.000000 ignos-internal-api-client-20230702.0.5514/ignos/internal/api/client/aio/_client.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3009 2023-07-02 17:28:48.000000 ignos-internal-api-client-20230702.0.5514/ignos/internal/api/client/aio/_configuration.py
--rw-r--r--   0 vsts      (1001) docker     (123)      674 2023-07-02 17:28:48.000000 ignos-internal-api-client-20230702.0.5514/ignos/internal/api/client/aio/_patch.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-02 17:29:03.846091 ignos-internal-api-client-20230702.0.5514/ignos/internal/api/client/aio/operations/
--rw-r--r--   0 vsts      (1001) docker     (123)     1503 2023-07-02 17:28:48.000000 ignos-internal-api-client-20230702.0.5514/ignos/internal/api/client/aio/operations/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)   102360 2023-07-02 17:28:48.000000 ignos-internal-api-client-20230702.0.5514/ignos/internal/api/client/aio/operations/_operations.py
--rw-r--r--   0 vsts      (1001) docker     (123)      674 2023-07-02 17:28:48.000000 ignos-internal-api-client-20230702.0.5514/ignos/internal/api/client/aio/operations/_patch.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-02 17:29:03.846091 ignos-internal-api-client-20230702.0.5514/ignos/internal/api/client/models/
--rw-r--r--   0 vsts      (1001) docker     (123)     2768 2023-07-02 17:28:48.000000 ignos-internal-api-client-20230702.0.5514/ignos/internal/api/client/models/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1054 2023-07-02 17:28:48.000000 ignos-internal-api-client-20230702.0.5514/ignos/internal/api/client/models/_enums.py
--rw-r--r--   0 vsts      (1001) docker     (123)    59535 2023-07-02 17:28:48.000000 ignos-internal-api-client-20230702.0.5514/ignos/internal/api/client/models/_models.py
--rw-r--r--   0 vsts      (1001) docker     (123)      674 2023-07-02 17:28:48.000000 ignos-internal-api-client-20230702.0.5514/ignos/internal/api/client/models/_patch.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-02 17:29:03.846091 ignos-internal-api-client-20230702.0.5514/ignos/internal/api/client/operations/
--rw-r--r--   0 vsts      (1001) docker     (123)     1503 2023-07-02 17:28:48.000000 ignos-internal-api-client-20230702.0.5514/ignos/internal/api/client/operations/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)   120947 2023-07-02 17:28:48.000000 ignos-internal-api-client-20230702.0.5514/ignos/internal/api/client/operations/_operations.py
--rw-r--r--   0 vsts      (1001) docker     (123)      674 2023-07-02 17:28:48.000000 ignos-internal-api-client-20230702.0.5514/ignos/internal/api/client/operations/_patch.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-02 17:29:03.846091 ignos-internal-api-client-20230702.0.5514/ignos_internal_api_client.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      195 2023-07-02 17:29:03.000000 ignos-internal-api-client-20230702.0.5514/ignos_internal_api_client.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     1256 2023-07-02 17:29:03.000000 ignos-internal-api-client-20230702.0.5514/ignos_internal_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-02 17:29:03.000000 ignos-internal-api-client-20230702.0.5514/ignos_internal_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       48 2023-07-02 17:29:03.000000 ignos-internal-api-client-20230702.0.5514/ignos_internal_api_client.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-07-02 17:29:03.000000 ignos-internal-api-client-20230702.0.5514/ignos_internal_api_client.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-07-02 17:29:03.846091 ignos-internal-api-client-20230702.0.5514/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)      982 2023-07-02 17:28:48.000000 ignos-internal-api-client-20230702.0.5514/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-19 08:34:34.816003 ignos-internal-api-client-20230719.0.5642/
+-rw-r--r--   0 vsts      (1001) docker     (123)      195 2023-07-19 08:34:34.816003 ignos-internal-api-client-20230719.0.5642/PKG-INFO
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-19 08:34:34.812003 ignos-internal-api-client-20230719.0.5642/ignos/
+-rw-r--r--   0 vsts      (1001) docker     (123)       81 2023-07-19 08:34:19.000000 ignos-internal-api-client-20230719.0.5642/ignos/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-19 08:34:34.812003 ignos-internal-api-client-20230719.0.5642/ignos/internal/
+-rw-r--r--   0 vsts      (1001) docker     (123)       81 2023-07-19 08:34:19.000000 ignos-internal-api-client-20230719.0.5642/ignos/internal/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-19 08:34:34.816003 ignos-internal-api-client-20230719.0.5642/ignos/internal/api/
+-rw-r--r--   0 vsts      (1001) docker     (123)       81 2023-07-19 08:34:19.000000 ignos-internal-api-client-20230719.0.5642/ignos/internal/api/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-19 08:34:34.816003 ignos-internal-api-client-20230719.0.5642/ignos/internal/api/client/
+-rw-r--r--   0 vsts      (1001) docker     (123)      876 2023-07-19 08:34:19.000000 ignos-internal-api-client-20230719.0.5642/ignos/internal/api/client/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6438 2023-07-19 08:34:19.000000 ignos-internal-api-client-20230719.0.5642/ignos/internal/api/client/_client.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2966 2023-07-19 08:34:19.000000 ignos-internal-api-client-20230719.0.5642/ignos/internal/api/client/_configuration.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      674 2023-07-19 08:34:19.000000 ignos-internal-api-client-20230719.0.5642/ignos/internal/api/client/_patch.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    79082 2023-07-19 08:34:19.000000 ignos-internal-api-client-20230719.0.5642/ignos/internal/api/client/_serialization.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      496 2023-07-19 08:34:19.000000 ignos-internal-api-client-20230719.0.5642/ignos/internal/api/client/_version.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-19 08:34:34.816003 ignos-internal-api-client-20230719.0.5642/ignos/internal/api/client/aio/
+-rw-r--r--   0 vsts      (1001) docker     (123)      823 2023-07-19 08:34:19.000000 ignos-internal-api-client-20230719.0.5642/ignos/internal/api/client/aio/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6618 2023-07-19 08:34:19.000000 ignos-internal-api-client-20230719.0.5642/ignos/internal/api/client/aio/_client.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3009 2023-07-19 08:34:19.000000 ignos-internal-api-client-20230719.0.5642/ignos/internal/api/client/aio/_configuration.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      674 2023-07-19 08:34:19.000000 ignos-internal-api-client-20230719.0.5642/ignos/internal/api/client/aio/_patch.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-19 08:34:34.816003 ignos-internal-api-client-20230719.0.5642/ignos/internal/api/client/aio/operations/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1571 2023-07-19 08:34:19.000000 ignos-internal-api-client-20230719.0.5642/ignos/internal/api/client/aio/operations/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   117128 2023-07-19 08:34:19.000000 ignos-internal-api-client-20230719.0.5642/ignos/internal/api/client/aio/operations/_operations.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      674 2023-07-19 08:34:19.000000 ignos-internal-api-client-20230719.0.5642/ignos/internal/api/client/aio/operations/_patch.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-19 08:34:34.816003 ignos-internal-api-client-20230719.0.5642/ignos/internal/api/client/models/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3108 2023-07-19 08:34:19.000000 ignos-internal-api-client-20230719.0.5642/ignos/internal/api/client/models/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1054 2023-07-19 08:34:19.000000 ignos-internal-api-client-20230719.0.5642/ignos/internal/api/client/models/_enums.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    66499 2023-07-19 08:34:19.000000 ignos-internal-api-client-20230719.0.5642/ignos/internal/api/client/models/_models.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      674 2023-07-19 08:34:19.000000 ignos-internal-api-client-20230719.0.5642/ignos/internal/api/client/models/_patch.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-19 08:34:34.816003 ignos-internal-api-client-20230719.0.5642/ignos/internal/api/client/operations/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1571 2023-07-19 08:34:19.000000 ignos-internal-api-client-20230719.0.5642/ignos/internal/api/client/operations/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   138610 2023-07-19 08:34:19.000000 ignos-internal-api-client-20230719.0.5642/ignos/internal/api/client/operations/_operations.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      674 2023-07-19 08:34:19.000000 ignos-internal-api-client-20230719.0.5642/ignos/internal/api/client/operations/_patch.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-19 08:34:34.816003 ignos-internal-api-client-20230719.0.5642/ignos_internal_api_client.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      195 2023-07-19 08:34:34.000000 ignos-internal-api-client-20230719.0.5642/ignos_internal_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     1219 2023-07-19 08:34:34.000000 ignos-internal-api-client-20230719.0.5642/ignos_internal_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-19 08:34:34.000000 ignos-internal-api-client-20230719.0.5642/ignos_internal_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       48 2023-07-19 08:34:34.000000 ignos-internal-api-client-20230719.0.5642/ignos_internal_api_client.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-07-19 08:34:34.000000 ignos-internal-api-client-20230719.0.5642/ignos_internal_api_client.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-07-19 08:34:34.816003 ignos-internal-api-client-20230719.0.5642/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)      982 2023-07-19 08:34:19.000000 ignos-internal-api-client-20230719.0.5642/setup.py
```

### Comparing `ignos-internal-api-client-20230702.0.5514/ignos/internal/api/client/__init__.py` & `ignos-internal-api-client-20230719.0.5642/ignos/internal/api/client/__init__.py`

 * *Files identical despite different names*

### Comparing `ignos-internal-api-client-20230702.0.5514/ignos/internal/api/client/_client.py` & `ignos-internal-api-client-20230719.0.5642/ignos/internal/api/client/_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from .operations import (
     AppsOperations,
     AzureRegionsOperations,
     CdfClustersOperations,
     CountriesOperations,
     CustomersOperations,
     DatabasesOperations,
+    ErpSyncOperations,
     PowerOperations,
     PresentationOperations,
     SustainabilitySetupOperations,
     TenantsOperations,
     UserOperations,
 )
 
@@ -45,14 +46,16 @@
     :vartype cdf_clusters: ignos.internal.api.client.operations.CdfClustersOperations
     :ivar countries: CountriesOperations operations
     :vartype countries: ignos.internal.api.client.operations.CountriesOperations
     :ivar customers: CustomersOperations operations
     :vartype customers: ignos.internal.api.client.operations.CustomersOperations
     :ivar databases: DatabasesOperations operations
     :vartype databases: ignos.internal.api.client.operations.DatabasesOperations
+    :ivar erp_sync: ErpSyncOperations operations
+    :vartype erp_sync: ignos.internal.api.client.operations.ErpSyncOperations
     :ivar power: PowerOperations operations
     :vartype power: ignos.internal.api.client.operations.PowerOperations
     :ivar presentation: PresentationOperations operations
     :vartype presentation: ignos.internal.api.client.operations.PresentationOperations
     :ivar sustainability_setup: SustainabilitySetupOperations operations
     :vartype sustainability_setup:
      ignos.internal.api.client.operations.SustainabilitySetupOperations
@@ -76,14 +79,15 @@
         self._serialize.client_side_validation = False
         self.apps = AppsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.azure_regions = AzureRegionsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.cdf_clusters = CdfClustersOperations(self._client, self._config, self._serialize, self._deserialize)
         self.countries = CountriesOperations(self._client, self._config, self._serialize, self._deserialize)
         self.customers = CustomersOperations(self._client, self._config, self._serialize, self._deserialize)
         self.databases = DatabasesOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.erp_sync = ErpSyncOperations(self._client, self._config, self._serialize, self._deserialize)
         self.power = PowerOperations(self._client, self._config, self._serialize, self._deserialize)
         self.presentation = PresentationOperations(self._client, self._config, self._serialize, self._deserialize)
         self.sustainability_setup = SustainabilitySetupOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.tenants = TenantsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.user = UserOperations(self._client, self._config, self._serialize, self._deserialize)
```

### Comparing `ignos-internal-api-client-20230702.0.5514/ignos/internal/api/client/_configuration.py` & `ignos-internal-api-client-20230719.0.5642/ignos/internal/api/client/_configuration.py`

 * *Files identical despite different names*

### Comparing `ignos-internal-api-client-20230702.0.5514/ignos/internal/api/client/_patch.py` & `ignos-internal-api-client-20230719.0.5642/ignos/internal/api/client/_patch.py`

 * *Files identical despite different names*

### Comparing `ignos-internal-api-client-20230702.0.5514/ignos/internal/api/client/_serialization.py` & `ignos-internal-api-client-20230719.0.5642/ignos/internal/api/client/_serialization.py`

 * *Files 1% similar despite different names*

```diff
@@ -658,16 +658,17 @@
                         _new_attr = new_attr
                         _serialized = serialized
                         for k in keys:  # type: ignore
                             if k not in _serialized:
                                 _serialized.update(_new_attr)  # type: ignore
                             _new_attr = _new_attr[k]  # type: ignore
                             _serialized = _serialized[k]
-                except ValueError:
-                    continue
+                except ValueError as err:
+                    if isinstance(err, SerializationError):
+                        raise
 
         except (AttributeError, KeyError, TypeError) as err:
             msg = "Attribute {} in object {} cannot be serialized.\n{}".format(attr_name, class_name, str(target_obj))
             raise_with_traceback(SerializationError, msg, err)
         else:
             return serialized
 
@@ -899,15 +900,17 @@
         serialization_ctxt = kwargs.get("serialization_ctxt", {})
         is_xml = kwargs.get("is_xml", False)
 
         serialized = []
         for d in data:
             try:
                 serialized.append(self.serialize_data(d, iter_type, **kwargs))
-            except ValueError:
+            except ValueError as err:
+                if isinstance(err, SerializationError):
+                    raise
                 serialized.append(None)
 
         if div:
             serialized = ["" if s is None else str(s) for s in serialized]
             serialized = div.join(serialized)
 
         if "xml" in serialization_ctxt or is_xml:
@@ -946,15 +949,17 @@
         :rtype: dict
         """
         serialization_ctxt = kwargs.get("serialization_ctxt", {})
         serialized = {}
         for key, value in attr.items():
             try:
                 serialized[self.serialize_unicode(key)] = self.serialize_data(value, dict_type, **kwargs)
-            except ValueError:
+            except ValueError as err:
+                if isinstance(err, SerializationError):
+                    raise
                 serialized[self.serialize_unicode(key)] = None
 
         if "xml" in serialization_ctxt:
             # XML serialization is more complicated
             xml_desc = serialization_ctxt["xml"]
             xml_name = xml_desc["name"]
```

### Comparing `ignos-internal-api-client-20230702.0.5514/ignos/internal/api/client/aio/__init__.py` & `ignos-internal-api-client-20230719.0.5642/ignos/internal/api/client/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `ignos-internal-api-client-20230702.0.5514/ignos/internal/api/client/aio/_client.py` & `ignos-internal-api-client-20230719.0.5642/ignos/internal/api/client/aio/_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from .operations import (
     AppsOperations,
     AzureRegionsOperations,
     CdfClustersOperations,
     CountriesOperations,
     CustomersOperations,
     DatabasesOperations,
+    ErpSyncOperations,
     PowerOperations,
     PresentationOperations,
     SustainabilitySetupOperations,
     TenantsOperations,
     UserOperations,
 )
 
@@ -45,14 +46,16 @@
     :vartype cdf_clusters: ignos.internal.api.client.aio.operations.CdfClustersOperations
     :ivar countries: CountriesOperations operations
     :vartype countries: ignos.internal.api.client.aio.operations.CountriesOperations
     :ivar customers: CustomersOperations operations
     :vartype customers: ignos.internal.api.client.aio.operations.CustomersOperations
     :ivar databases: DatabasesOperations operations
     :vartype databases: ignos.internal.api.client.aio.operations.DatabasesOperations
+    :ivar erp_sync: ErpSyncOperations operations
+    :vartype erp_sync: ignos.internal.api.client.aio.operations.ErpSyncOperations
     :ivar power: PowerOperations operations
     :vartype power: ignos.internal.api.client.aio.operations.PowerOperations
     :ivar presentation: PresentationOperations operations
     :vartype presentation: ignos.internal.api.client.aio.operations.PresentationOperations
     :ivar sustainability_setup: SustainabilitySetupOperations operations
     :vartype sustainability_setup:
      ignos.internal.api.client.aio.operations.SustainabilitySetupOperations
@@ -76,14 +79,15 @@
         self._serialize.client_side_validation = False
         self.apps = AppsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.azure_regions = AzureRegionsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.cdf_clusters = CdfClustersOperations(self._client, self._config, self._serialize, self._deserialize)
         self.countries = CountriesOperations(self._client, self._config, self._serialize, self._deserialize)
         self.customers = CustomersOperations(self._client, self._config, self._serialize, self._deserialize)
         self.databases = DatabasesOperations(self._client, self._config, self._serialize, self._deserialize)
+        self.erp_sync = ErpSyncOperations(self._client, self._config, self._serialize, self._deserialize)
         self.power = PowerOperations(self._client, self._config, self._serialize, self._deserialize)
         self.presentation = PresentationOperations(self._client, self._config, self._serialize, self._deserialize)
         self.sustainability_setup = SustainabilitySetupOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.tenants = TenantsOperations(self._client, self._config, self._serialize, self._deserialize)
         self.user = UserOperations(self._client, self._config, self._serialize, self._deserialize)
```

### Comparing `ignos-internal-api-client-20230702.0.5514/ignos/internal/api/client/aio/_configuration.py` & `ignos-internal-api-client-20230719.0.5642/ignos/internal/api/client/aio/_configuration.py`

 * *Files identical despite different names*

### Comparing `ignos-internal-api-client-20230702.0.5514/ignos/internal/api/client/aio/_patch.py` & `ignos-internal-api-client-20230719.0.5642/ignos/internal/api/client/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `ignos-internal-api-client-20230702.0.5514/ignos/internal/api/client/aio/operations/__init__.py` & `ignos-internal-api-client-20230719.0.5642/ignos/internal/api/client/aio/operations/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 from ._operations import AppsOperations
 from ._operations import AzureRegionsOperations
 from ._operations import CdfClustersOperations
 from ._operations import CountriesOperations
 from ._operations import CustomersOperations
 from ._operations import DatabasesOperations
+from ._operations import ErpSyncOperations
 from ._operations import PowerOperations
 from ._operations import PresentationOperations
 from ._operations import SustainabilitySetupOperations
 from ._operations import TenantsOperations
 from ._operations import UserOperations
 
 from ._patch import __all__ as _patch_all
@@ -25,14 +26,15 @@
 __all__ = [
     "AppsOperations",
     "AzureRegionsOperations",
     "CdfClustersOperations",
     "CountriesOperations",
     "CustomersOperations",
     "DatabasesOperations",
+    "ErpSyncOperations",
     "PowerOperations",
     "PresentationOperations",
     "SustainabilitySetupOperations",
     "TenantsOperations",
     "UserOperations",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
```

### Comparing `ignos-internal-api-client-20230702.0.5514/ignos/internal/api/client/aio/operations/_operations.py` & `ignos-internal-api-client-20230719.0.5642/ignos/internal/api/client/aio/operations/_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,15 @@
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
     map_error,
 )
 from azure.core.pipeline import PipelineResponse
-from azure.core.pipeline.transport import AsyncHttpResponse
-from azure.core.rest import HttpRequest
+from azure.core.rest import AsyncHttpResponse, HttpRequest
 from azure.core.tracing.decorator_async import distributed_trace_async
 from azure.core.utils import case_insensitive_dict
 
 from ... import models as _models
 from ...operations._operations import (
     build_apps_create_app_request,
     build_apps_list_apps_request,
@@ -43,14 +42,19 @@
     build_customers_list_customers_request,
     build_customers_list_tenant_keys_request,
     build_customers_remove_customer_app_request,
     build_customers_update_cdf_config_request,
     build_customers_update_customer_request,
     build_customers_update_tenant_request,
     build_databases_update_databases_request,
+    build_erp_sync_delete_erp_sync_error_request,
+    build_erp_sync_get_stack_trace_request,
+    build_erp_sync_list_erp_sync_errors_request,
+    build_erp_sync_start_full_sync_request,
+    build_erp_sync_sync_single_work_order_request,
     build_power_create_power_region_request,
     build_power_list_power_regions_by_country_request,
     build_presentation_delete_component_settings_request,
     build_presentation_save_component_settings_request,
     build_sustainability_setup_init_ferro_amp_request,
     build_sustainability_setup_map_factory_template_ferro_amp_request,
     build_sustainability_setup_map_factory_template_request,
@@ -1841,14 +1845,405 @@
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})
+
+
+class ErpSyncOperations:
+    """
+    .. warning::
+        **DO NOT** instantiate this class directly.
+
+        Instead, you should access the following operations through
+        :class:`~ignos.internal.api.client.aio.IgnosInternalApi`'s
+        :attr:`erp_sync` attribute.
+    """
+
+    models = _models
+
+    def __init__(self, *args, **kwargs) -> None:
+        input_args = list(args)
+        self._client = input_args.pop(0) if input_args else kwargs.pop("client")
+        self._config = input_args.pop(0) if input_args else kwargs.pop("config")
+        self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
+        self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
+
+    @distributed_trace_async
+    async def list_erp_sync_errors(self, tenant_id: str, **kwargs: Any) -> List[_models.ErpSyncErrorDto]:
+        """list_erp_sync_errors.
+
+        :param tenant_id: Required.
+        :type tenant_id: str
+        :return: list of ErpSyncErrorDto
+        :rtype: list[~ignos.internal.api.client.models.ErpSyncErrorDto]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[List[_models.ErpSyncErrorDto]] = kwargs.pop("cls", None)
+
+        request = build_erp_sync_list_erp_sync_errors_request(
+            tenant_id=tenant_id,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        deserialized = self._deserialize("[ErpSyncErrorDto]", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})
+
+        return deserialized
+
+    @distributed_trace_async
+    async def get_stack_trace(self, tenant_id: str, row_key: str, **kwargs: Any) -> _models.ErpSyncErrorMessage:
+        """get_stack_trace.
+
+        :param tenant_id: Required.
+        :type tenant_id: str
+        :param row_key: Required.
+        :type row_key: str
+        :return: ErpSyncErrorMessage
+        :rtype: ~ignos.internal.api.client.models.ErpSyncErrorMessage
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[_models.ErpSyncErrorMessage] = kwargs.pop("cls", None)
+
+        request = build_erp_sync_get_stack_trace_request(
+            tenant_id=tenant_id,
+            row_key=row_key,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        deserialized = self._deserialize("ErpSyncErrorMessage", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})
+
+        return deserialized
+
+    @distributed_trace_async
+    async def delete_erp_sync_error(  # pylint: disable=inconsistent-return-statements
+        self, tenant_id: str, partition_key: str, row_key: str, **kwargs: Any
+    ) -> None:
+        """delete_erp_sync_error.
+
+        :param tenant_id: Required.
+        :type tenant_id: str
+        :param partition_key: Required.
+        :type partition_key: str
+        :param row_key: Required.
+        :type row_key: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        request = build_erp_sync_delete_erp_sync_error_request(
+            tenant_id=tenant_id,
+            partition_key=partition_key,
+            row_key=row_key,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})
+
+    @overload
+    async def start_full_sync(
+        self,
+        tenant_id: str,
+        body: Optional[_models.StartFullSync] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> _models.DataSyncOrchestrationInstance:
+        """start_full_sync.
+
+        :param tenant_id: Required.
+        :type tenant_id: str
+        :param body: Default value is None.
+        :type body: ~ignos.internal.api.client.models.StartFullSync
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: DataSyncOrchestrationInstance
+        :rtype: ~ignos.internal.api.client.models.DataSyncOrchestrationInstance
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    async def start_full_sync(
+        self, tenant_id: str, body: Optional[IO] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> _models.DataSyncOrchestrationInstance:
+        """start_full_sync.
+
+        :param tenant_id: Required.
+        :type tenant_id: str
+        :param body: Default value is None.
+        :type body: IO
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: DataSyncOrchestrationInstance
+        :rtype: ~ignos.internal.api.client.models.DataSyncOrchestrationInstance
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace_async
+    async def start_full_sync(
+        self, tenant_id: str, body: Optional[Union[_models.StartFullSync, IO]] = None, **kwargs: Any
+    ) -> _models.DataSyncOrchestrationInstance:
+        """start_full_sync.
+
+        :param tenant_id: Required.
+        :type tenant_id: str
+        :param body: Is either a StartFullSync type or a IO type. Default value is None.
+        :type body: ~ignos.internal.api.client.models.StartFullSync or IO
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/*+json',
+         'application/json', 'text/json'. Default value is None.
+        :paramtype content_type: str
+        :return: DataSyncOrchestrationInstance
+        :rtype: ~ignos.internal.api.client.models.DataSyncOrchestrationInstance
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.DataSyncOrchestrationInstance] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "StartFullSync")
+            else:
+                _json = None
+
+        request = build_erp_sync_start_full_sync_request(
+            tenant_id=tenant_id,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        deserialized = self._deserialize("DataSyncOrchestrationInstance", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})
+
+        return deserialized
+
+    @overload
+    async def sync_single_work_order(  # pylint: disable=inconsistent-return-statements
+        self,
+        tenant_id: str,
+        body: Optional[_models.SyncSingleWorkOrder] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> None:
+        """sync_single_work_order.
+
+        :param tenant_id: Required.
+        :type tenant_id: str
+        :param body: Default value is None.
+        :type body: ~ignos.internal.api.client.models.SyncSingleWorkOrder
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    async def sync_single_work_order(  # pylint: disable=inconsistent-return-statements
+        self, tenant_id: str, body: Optional[IO] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> None:
+        """sync_single_work_order.
+
+        :param tenant_id: Required.
+        :type tenant_id: str
+        :param body: Default value is None.
+        :type body: IO
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace_async
+    async def sync_single_work_order(  # pylint: disable=inconsistent-return-statements
+        self, tenant_id: str, body: Optional[Union[_models.SyncSingleWorkOrder, IO]] = None, **kwargs: Any
+    ) -> None:
+        """sync_single_work_order.
+
+        :param tenant_id: Required.
+        :type tenant_id: str
+        :param body: Is either a SyncSingleWorkOrder type or a IO type. Default value is None.
+        :type body: ~ignos.internal.api.client.models.SyncSingleWorkOrder or IO
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/*+json',
+         'application/json', 'text/json'. Default value is None.
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "SyncSingleWorkOrder")
+            else:
+                _json = None
+
+        request = build_erp_sync_sync_single_work_order_request(
+            tenant_id=tenant_id,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
             request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
```

### Comparing `ignos-internal-api-client-20230702.0.5514/ignos/internal/api/client/aio/operations/_patch.py` & `ignos-internal-api-client-20230719.0.5642/ignos/internal/api/client/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `ignos-internal-api-client-20230702.0.5514/ignos/internal/api/client/models/__init__.py` & `ignos-internal-api-client-20230719.0.5642/ignos/internal/api/client/models/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,20 +16,25 @@
 from ._models import CountryDto
 from ._models import CreateApp
 from ._models import CreateCdfCluster
 from ._models import CreateIgnosCustomer
 from ._models import CreatePowerRegion
 from ._models import CreateTenantRequest
 from ._models import CustomerAppDto
+from ._models import DataSyncOrchestrationInstance
+from ._models import ErpSyncErrorDto
+from ._models import ErpSyncErrorMessage
 from ._models import IgnosCustomerDto
 from ._models import InitFactoryTemplateFerroAmpRequest
 from ._models import InitFactoryTemplateRequest
 from ._models import InitFerroAmpRequest
 from ._models import PowerRegionDto
 from ._models import SaveComponentSettingsRequest
+from ._models import StartFullSync
+from ._models import SyncSingleWorkOrder
 from ._models import TenantDetailDto
 from ._models import TenantDto
 from ._models import TenantKeyDto
 from ._models import UpdateAppRequest
 from ._models import UpdateCdfClusterRequest
 from ._models import UpdateCustomerRequest
 from ._models import UpdateTenantCdfConfigRequest
@@ -54,20 +59,25 @@
     "CountryDto",
     "CreateApp",
     "CreateCdfCluster",
     "CreateIgnosCustomer",
     "CreatePowerRegion",
     "CreateTenantRequest",
     "CustomerAppDto",
+    "DataSyncOrchestrationInstance",
+    "ErpSyncErrorDto",
+    "ErpSyncErrorMessage",
     "IgnosCustomerDto",
     "InitFactoryTemplateFerroAmpRequest",
     "InitFactoryTemplateRequest",
     "InitFerroAmpRequest",
     "PowerRegionDto",
     "SaveComponentSettingsRequest",
+    "StartFullSync",
+    "SyncSingleWorkOrder",
     "TenantDetailDto",
     "TenantDto",
     "TenantKeyDto",
     "UpdateAppRequest",
     "UpdateCdfClusterRequest",
     "UpdateCustomerRequest",
     "UpdateTenantCdfConfigRequest",
```

### Comparing `ignos-internal-api-client-20230702.0.5514/ignos/internal/api/client/models/_enums.py` & `ignos-internal-api-client-20230719.0.5642/ignos/internal/api/client/models/_enums.py`

 * *Files identical despite different names*

### Comparing `ignos-internal-api-client-20230702.0.5514/ignos/internal/api/client/models/_models.py` & `ignos-internal-api-client-20230719.0.5642/ignos/internal/api/client/models/_models.py`

 * *Files 3% similar despite different names*

```diff
@@ -794,14 +794,154 @@
         self.id = id
         self.key = key
         self.name = name
         self.description = description
         self.private_app = private_app
 
 
+class DataSyncOrchestrationInstance(_serialization.Model):
+    """DataSyncOrchestrationInstance.
+
+    :ivar id:
+    :vartype id: str
+    :ivar purge_history_delete_uri:
+    :vartype purge_history_delete_uri: str
+    :ivar send_event_post_uri:
+    :vartype send_event_post_uri: str
+    :ivar status_query_get_uri:
+    :vartype status_query_get_uri: str
+    :ivar terminate_post_uri:
+    :vartype terminate_post_uri: str
+    """
+
+    _attribute_map = {
+        "id": {"key": "id", "type": "str"},
+        "purge_history_delete_uri": {"key": "purgeHistoryDeleteUri", "type": "str"},
+        "send_event_post_uri": {"key": "sendEventPostUri", "type": "str"},
+        "status_query_get_uri": {"key": "statusQueryGetUri", "type": "str"},
+        "terminate_post_uri": {"key": "terminatePostUri", "type": "str"},
+    }
+
+    def __init__(
+        self,
+        *,
+        id: Optional[str] = None,  # pylint: disable=redefined-builtin
+        purge_history_delete_uri: Optional[str] = None,
+        send_event_post_uri: Optional[str] = None,
+        status_query_get_uri: Optional[str] = None,
+        terminate_post_uri: Optional[str] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword id:
+        :paramtype id: str
+        :keyword purge_history_delete_uri:
+        :paramtype purge_history_delete_uri: str
+        :keyword send_event_post_uri:
+        :paramtype send_event_post_uri: str
+        :keyword status_query_get_uri:
+        :paramtype status_query_get_uri: str
+        :keyword terminate_post_uri:
+        :paramtype terminate_post_uri: str
+        """
+        super().__init__(**kwargs)
+        self.id = id
+        self.purge_history_delete_uri = purge_history_delete_uri
+        self.send_event_post_uri = send_event_post_uri
+        self.status_query_get_uri = status_query_get_uri
+        self.terminate_post_uri = terminate_post_uri
+
+
+class ErpSyncErrorDto(_serialization.Model):
+    """ErpSyncErrorDto.
+
+    :ivar entity:
+    :vartype entity: str
+    :ivar id:
+    :vartype id: str
+    :ivar company_id:
+    :vartype company_id: str
+    :ivar retry_attempts:
+    :vartype retry_attempts: int
+    :ivar row_key:
+    :vartype row_key: str
+    :ivar partition_key:
+    :vartype partition_key: str
+    :ivar timestamp:
+    :vartype timestamp: ~datetime.datetime
+    """
+
+    _attribute_map = {
+        "entity": {"key": "entity", "type": "str"},
+        "id": {"key": "id", "type": "str"},
+        "company_id": {"key": "companyId", "type": "str"},
+        "retry_attempts": {"key": "retryAttempts", "type": "int"},
+        "row_key": {"key": "rowKey", "type": "str"},
+        "partition_key": {"key": "partitionKey", "type": "str"},
+        "timestamp": {"key": "timestamp", "type": "iso-8601"},
+    }
+
+    def __init__(
+        self,
+        *,
+        entity: Optional[str] = None,
+        id: Optional[str] = None,  # pylint: disable=redefined-builtin
+        company_id: Optional[str] = None,
+        retry_attempts: Optional[int] = None,
+        row_key: Optional[str] = None,
+        partition_key: Optional[str] = None,
+        timestamp: Optional[datetime.datetime] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword entity:
+        :paramtype entity: str
+        :keyword id:
+        :paramtype id: str
+        :keyword company_id:
+        :paramtype company_id: str
+        :keyword retry_attempts:
+        :paramtype retry_attempts: int
+        :keyword row_key:
+        :paramtype row_key: str
+        :keyword partition_key:
+        :paramtype partition_key: str
+        :keyword timestamp:
+        :paramtype timestamp: ~datetime.datetime
+        """
+        super().__init__(**kwargs)
+        self.entity = entity
+        self.id = id
+        self.company_id = company_id
+        self.retry_attempts = retry_attempts
+        self.row_key = row_key
+        self.partition_key = partition_key
+        self.timestamp = timestamp
+
+
+class ErpSyncErrorMessage(_serialization.Model):
+    """ErpSyncErrorMessage.
+
+    :ivar stack_trace:
+    :vartype stack_trace: str
+    """
+
+    _attribute_map = {
+        "stack_trace": {"key": "stackTrace", "type": "str"},
+    }
+
+    def __init__(self, *, stack_trace: Optional[str] = None, **kwargs: Any) -> None:
+        """
+        :keyword stack_trace:
+        :paramtype stack_trace: str
+        """
+        super().__init__(**kwargs)
+        self.stack_trace = stack_trace
+
+
 class IgnosCustomerDto(_serialization.Model):  # pylint: disable=too-many-instance-attributes
     """IgnosCustomerDto.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar id: Required.
     :vartype id: str
@@ -1125,14 +1265,93 @@
         :keyword disabled_fields: Required.
         :paramtype disabled_fields: list[str]
         """
         super().__init__(**kwargs)
         self.disabled_fields = disabled_fields
 
 
+class StartFullSync(_serialization.Model):
+    """StartFullSync.
+
+    :ivar sync_companies:
+    :vartype sync_companies: bool
+    :ivar sync_resources:
+    :vartype sync_resources: bool
+    :ivar sync_work_orders:
+    :vartype sync_work_orders: bool
+    :ivar sync_deviations:
+    :vartype sync_deviations: bool
+    :ivar work_order_sync_batch_size:
+    :vartype work_order_sync_batch_size: int
+    """
+
+    _attribute_map = {
+        "sync_companies": {"key": "syncCompanies", "type": "bool"},
+        "sync_resources": {"key": "syncResources", "type": "bool"},
+        "sync_work_orders": {"key": "syncWorkOrders", "type": "bool"},
+        "sync_deviations": {"key": "syncDeviations", "type": "bool"},
+        "work_order_sync_batch_size": {"key": "workOrderSyncBatchSize", "type": "int"},
+    }
+
+    def __init__(
+        self,
+        *,
+        sync_companies: Optional[bool] = None,
+        sync_resources: Optional[bool] = None,
+        sync_work_orders: Optional[bool] = None,
+        sync_deviations: Optional[bool] = None,
+        work_order_sync_batch_size: Optional[int] = None,
+        **kwargs: Any
+    ) -> None:
+        """
+        :keyword sync_companies:
+        :paramtype sync_companies: bool
+        :keyword sync_resources:
+        :paramtype sync_resources: bool
+        :keyword sync_work_orders:
+        :paramtype sync_work_orders: bool
+        :keyword sync_deviations:
+        :paramtype sync_deviations: bool
+        :keyword work_order_sync_batch_size:
+        :paramtype work_order_sync_batch_size: int
+        """
+        super().__init__(**kwargs)
+        self.sync_companies = sync_companies
+        self.sync_resources = sync_resources
+        self.sync_work_orders = sync_work_orders
+        self.sync_deviations = sync_deviations
+        self.work_order_sync_batch_size = work_order_sync_batch_size
+
+
+class SyncSingleWorkOrder(_serialization.Model):
+    """SyncSingleWorkOrder.
+
+    :ivar company_id:
+    :vartype company_id: str
+    :ivar work_order_id:
+    :vartype work_order_id: str
+    """
+
+    _attribute_map = {
+        "company_id": {"key": "companyId", "type": "str"},
+        "work_order_id": {"key": "workOrderId", "type": "str"},
+    }
+
+    def __init__(self, *, company_id: Optional[str] = None, work_order_id: Optional[str] = None, **kwargs: Any) -> None:
+        """
+        :keyword company_id:
+        :paramtype company_id: str
+        :keyword work_order_id:
+        :paramtype work_order_id: str
+        """
+        super().__init__(**kwargs)
+        self.company_id = company_id
+        self.work_order_id = work_order_id
+
+
 class TenantDetailDto(_serialization.Model):
     """TenantDetailDto.
 
     All required parameters must be populated in order to send to Azure.
 
     :ivar tenant_id: Required.
     :vartype tenant_id: str
```

### Comparing `ignos-internal-api-client-20230702.0.5514/ignos/internal/api/client/models/_patch.py` & `ignos-internal-api-client-20230719.0.5642/ignos/internal/api/client/models/_patch.py`

 * *Files identical despite different names*

### Comparing `ignos-internal-api-client-20230702.0.5514/ignos/internal/api/client/operations/__init__.py` & `ignos-internal-api-client-20230719.0.5642/ignos/internal/api/client/operations/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 from ._operations import AppsOperations
 from ._operations import AzureRegionsOperations
 from ._operations import CdfClustersOperations
 from ._operations import CountriesOperations
 from ._operations import CustomersOperations
 from ._operations import DatabasesOperations
+from ._operations import ErpSyncOperations
 from ._operations import PowerOperations
 from ._operations import PresentationOperations
 from ._operations import SustainabilitySetupOperations
 from ._operations import TenantsOperations
 from ._operations import UserOperations
 
 from ._patch import __all__ as _patch_all
@@ -25,14 +26,15 @@
 __all__ = [
     "AppsOperations",
     "AzureRegionsOperations",
     "CdfClustersOperations",
     "CountriesOperations",
     "CustomersOperations",
     "DatabasesOperations",
+    "ErpSyncOperations",
     "PowerOperations",
     "PresentationOperations",
     "SustainabilitySetupOperations",
     "TenantsOperations",
     "UserOperations",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
```

### Comparing `ignos-internal-api-client-20230702.0.5514/ignos/internal/api/client/operations/_operations.py` & `ignos-internal-api-client-20230719.0.5642/ignos/internal/api/client/operations/_operations.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,22 +14,20 @@
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
     map_error,
 )
 from azure.core.pipeline import PipelineResponse
-from azure.core.pipeline.transport import HttpResponse
-from azure.core.rest import HttpRequest
+from azure.core.rest import HttpRequest, HttpResponse
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 
 from .. import models as _models
 from .._serialization import Serializer
-from .._vendor import _format_url_section
 
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
@@ -73,15 +71,15 @@
 
     # Construct URL
     _url = "/apps/{id}"
     path_format_arguments = {
         "id": _SERIALIZER.url("id", id, "str"),
     }
 
-    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct headers
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="PUT", url=_url, headers=_headers, **kwargs)
@@ -140,15 +138,15 @@
 
     # Construct URL
     _url = "/cdfclusters/{id}"
     path_format_arguments = {
         "id": _SERIALIZER.url("id", id, "str"),
     }
 
-    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct headers
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="PUT", url=_url, headers=_headers, **kwargs)
@@ -217,15 +215,15 @@
 
     # Construct URL
     _url = "/customers/{id}"
     path_format_arguments = {
         "id": _SERIALIZER.url("id", id, "str"),
     }
 
-    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, headers=_headers, **kwargs)
 
 
@@ -237,15 +235,15 @@
 
     # Construct URL
     _url = "/customers/{id}"
     path_format_arguments = {
         "id": _SERIALIZER.url("id", id, "str"),
     }
 
-    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct headers
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="PUT", url=_url, headers=_headers, **kwargs)
@@ -258,15 +256,15 @@
 
     # Construct URL
     _url = "/customers/{id}/tenants"
     path_format_arguments = {
         "id": _SERIALIZER.url("id", id, "str"),
     }
 
-    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, headers=_headers, **kwargs)
 
 
@@ -278,15 +276,15 @@
 
     # Construct URL
     _url = "/customers/{id}/tenants"
     path_format_arguments = {
         "id": _SERIALIZER.url("id", id, "str"),
     }
 
-    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct headers
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
@@ -301,15 +299,15 @@
     # Construct URL
     _url = "/customers/{id}/tenants/{tenantId}"
     path_format_arguments = {
         "id": _SERIALIZER.url("id", id, "str"),
         "tenantId": _SERIALIZER.url("tenant_id", tenant_id, "str"),
     }
 
-    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct headers
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="PUT", url=_url, headers=_headers, **kwargs)
@@ -323,15 +321,15 @@
     # Construct URL
     _url = "/customers/{id}/tenants/{tenantId}/config"
     path_format_arguments = {
         "id": _SERIALIZER.url("id", id, "str"),
         "tenantId": _SERIALIZER.url("tenant_id", tenant_id, "str"),
     }
 
-    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, headers=_headers, **kwargs)
 
 
@@ -344,15 +342,15 @@
     # Construct URL
     _url = "/customers/{id}/tenants/{tenantId}/config"
     path_format_arguments = {
         "id": _SERIALIZER.url("id", id, "str"),
         "tenantId": _SERIALIZER.url("tenant_id", tenant_id, "str"),
     }
 
-    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct headers
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
@@ -365,15 +363,15 @@
 
     # Construct URL
     _url = "/customers/{id}/apps"
     path_format_arguments = {
         "id": _SERIALIZER.url("id", id, "str"),
     }
 
-    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, headers=_headers, **kwargs)
 
 
@@ -381,28 +379,28 @@
     # Construct URL
     _url = "/customers/{id}/apps/{appId}"
     path_format_arguments = {
         "id": _SERIALIZER.url("id", id, "str"),
         "appId": _SERIALIZER.url("app_id", app_id, "str"),
     }
 
-    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     return HttpRequest(method="POST", url=_url, **kwargs)
 
 
 def build_customers_remove_customer_app_request(id: str, app_id: str, **kwargs: Any) -> HttpRequest:
     # Construct URL
     _url = "/customers/{id}/apps/{appId}"
     path_format_arguments = {
         "id": _SERIALIZER.url("id", id, "str"),
         "appId": _SERIALIZER.url("app_id", app_id, "str"),
     }
 
-    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     return HttpRequest(method="DELETE", url=_url, **kwargs)
 
 
 def build_customers_list_tenant_keys_request(**kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
@@ -420,14 +418,110 @@
 def build_databases_update_databases_request(**kwargs: Any) -> HttpRequest:
     # Construct URL
     _url = "/databases"
 
     return HttpRequest(method="POST", url=_url, **kwargs)
 
 
+def build_erp_sync_list_erp_sync_errors_request(tenant_id: str, **kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/erpsync/{tenantId}/errors"
+    path_format_arguments = {
+        "tenantId": _SERIALIZER.url("tenant_id", tenant_id, "str"),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, headers=_headers, **kwargs)
+
+
+def build_erp_sync_get_stack_trace_request(tenant_id: str, row_key: str, **kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/erpsync/{tenantId}/errors/{rowKey}/stacktrace"
+    path_format_arguments = {
+        "tenantId": _SERIALIZER.url("tenant_id", tenant_id, "str"),
+        "rowKey": _SERIALIZER.url("row_key", row_key, "str"),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, headers=_headers, **kwargs)
+
+
+def build_erp_sync_delete_erp_sync_error_request(
+    tenant_id: str, partition_key: str, row_key: str, **kwargs: Any
+) -> HttpRequest:
+    # Construct URL
+    _url = "/erpsync/{tenantId}/errors/{partitionKey}/{rowKey}"
+    path_format_arguments = {
+        "tenantId": _SERIALIZER.url("tenant_id", tenant_id, "str"),
+        "partitionKey": _SERIALIZER.url("partition_key", partition_key, "str"),
+        "rowKey": _SERIALIZER.url("row_key", row_key, "str"),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    return HttpRequest(method="DELETE", url=_url, **kwargs)
+
+
+def build_erp_sync_start_full_sync_request(tenant_id: str, **kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/erpsync/{tenantId}/start-full-sync"
+    path_format_arguments = {
+        "tenantId": _SERIALIZER.url("tenant_id", tenant_id, "str"),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
+
+
+def build_erp_sync_sync_single_work_order_request(tenant_id: str, **kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+    # Construct URL
+    _url = "/erpsync/{tenantId}/sync-work-order"
+    path_format_arguments = {
+        "tenantId": _SERIALIZER.url("tenant_id", tenant_id, "str"),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
+
+    return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
+
+
 def build_power_list_power_regions_by_country_request(*, country: Optional[str] = None, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
@@ -467,15 +561,15 @@
     _url = "/presentation/components/{azureAdTenantId}/{tenantId}/{componentId}"
     path_format_arguments = {
         "azureAdTenantId": _SERIALIZER.url("azure_ad_tenant_id", azure_ad_tenant_id, "str"),
         "tenantId": _SERIALIZER.url("tenant_id", tenant_id, "str"),
         "componentId": _SERIALIZER.url("component_id", component_id, "str"),
     }
 
-    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     return HttpRequest(method="DELETE", url=_url, **kwargs)
 
 
 def build_presentation_save_component_settings_request(
     azure_ad_tenant_id: str, tenant_id: str, component_id: str, **kwargs: Any
 ) -> HttpRequest:
@@ -488,15 +582,15 @@
     _url = "/presentation/components/{azureAdTenantId}/{tenantId}/{componentId}"
     path_format_arguments = {
         "azureAdTenantId": _SERIALIZER.url("azure_ad_tenant_id", azure_ad_tenant_id, "str"),
         "tenantId": _SERIALIZER.url("tenant_id", tenant_id, "str"),
         "componentId": _SERIALIZER.url("component_id", component_id, "str"),
     }
 
-    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct headers
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="PUT", url=_url, headers=_headers, **kwargs)
@@ -511,15 +605,15 @@
     # Construct URL
     _url = "/sustainabilitysetup/{azureAdTenantId}/{tenantId}/ferroamp"
     path_format_arguments = {
         "azureAdTenantId": _SERIALIZER.url("azure_ad_tenant_id", azure_ad_tenant_id, "str"),
         "tenantId": _SERIALIZER.url("tenant_id", tenant_id, "str"),
     }
 
-    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct headers
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
 
     return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
 
@@ -533,15 +627,15 @@
     # Construct URL
     _url = "/sustainabilitysetup/{azureAdTenantId}/{tenantId}/factorytemplate"
     path_format_arguments = {
         "azureAdTenantId": _SERIALIZER.url("azure_ad_tenant_id", azure_ad_tenant_id, "str"),
         "tenantId": _SERIALIZER.url("tenant_id", tenant_id, "str"),
     }
 
-    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct headers
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
 
     return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
 
@@ -555,15 +649,15 @@
     # Construct URL
     _url = "/sustainabilitysetup/{azureAdTenantId}/{tenantId}/factorytemplate/ferroamp"
     path_format_arguments = {
         "azureAdTenantId": _SERIALIZER.url("azure_ad_tenant_id", azure_ad_tenant_id, "str"),
         "tenantId": _SERIALIZER.url("tenant_id", tenant_id, "str"),
     }
 
-    _url: str = _format_url_section(_url, **path_format_arguments)  # type: ignore
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
 
     # Construct headers
     if content_type is not None:
         _headers["Content-Type"] = _SERIALIZER.header("content_type", content_type, "str")
 
     return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
 
@@ -2384,14 +2478,405 @@
             headers=_headers,
             params=_params,
         )
         request.url = self._client.format_url(request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})
+
+
+class ErpSyncOperations:
+    """
+    .. warning::
+        **DO NOT** instantiate this class directly.
+
+        Instead, you should access the following operations through
+        :class:`~ignos.internal.api.client.IgnosInternalApi`'s
+        :attr:`erp_sync` attribute.
+    """
+
+    models = _models
+
+    def __init__(self, *args, **kwargs):
+        input_args = list(args)
+        self._client = input_args.pop(0) if input_args else kwargs.pop("client")
+        self._config = input_args.pop(0) if input_args else kwargs.pop("config")
+        self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
+        self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
+
+    @distributed_trace
+    def list_erp_sync_errors(self, tenant_id: str, **kwargs: Any) -> List[_models.ErpSyncErrorDto]:
+        """list_erp_sync_errors.
+
+        :param tenant_id: Required.
+        :type tenant_id: str
+        :return: list of ErpSyncErrorDto
+        :rtype: list[~ignos.internal.api.client.models.ErpSyncErrorDto]
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[List[_models.ErpSyncErrorDto]] = kwargs.pop("cls", None)
+
+        request = build_erp_sync_list_erp_sync_errors_request(
+            tenant_id=tenant_id,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        deserialized = self._deserialize("[ErpSyncErrorDto]", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})
+
+        return deserialized
+
+    @distributed_trace
+    def get_stack_trace(self, tenant_id: str, row_key: str, **kwargs: Any) -> _models.ErpSyncErrorMessage:
+        """get_stack_trace.
+
+        :param tenant_id: Required.
+        :type tenant_id: str
+        :param row_key: Required.
+        :type row_key: str
+        :return: ErpSyncErrorMessage
+        :rtype: ~ignos.internal.api.client.models.ErpSyncErrorMessage
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[_models.ErpSyncErrorMessage] = kwargs.pop("cls", None)
+
+        request = build_erp_sync_get_stack_trace_request(
+            tenant_id=tenant_id,
+            row_key=row_key,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        deserialized = self._deserialize("ErpSyncErrorMessage", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})
+
+        return deserialized
+
+    @distributed_trace
+    def delete_erp_sync_error(  # pylint: disable=inconsistent-return-statements
+        self, tenant_id: str, partition_key: str, row_key: str, **kwargs: Any
+    ) -> None:
+        """delete_erp_sync_error.
+
+        :param tenant_id: Required.
+        :type tenant_id: str
+        :param partition_key: Required.
+        :type partition_key: str
+        :param row_key: Required.
+        :type row_key: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        request = build_erp_sync_delete_erp_sync_error_request(
+            tenant_id=tenant_id,
+            partition_key=partition_key,
+            row_key=row_key,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        if cls:
+            return cls(pipeline_response, None, {})
+
+    @overload
+    def start_full_sync(
+        self,
+        tenant_id: str,
+        body: Optional[_models.StartFullSync] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> _models.DataSyncOrchestrationInstance:
+        """start_full_sync.
+
+        :param tenant_id: Required.
+        :type tenant_id: str
+        :param body: Default value is None.
+        :type body: ~ignos.internal.api.client.models.StartFullSync
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: DataSyncOrchestrationInstance
+        :rtype: ~ignos.internal.api.client.models.DataSyncOrchestrationInstance
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    def start_full_sync(
+        self, tenant_id: str, body: Optional[IO] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> _models.DataSyncOrchestrationInstance:
+        """start_full_sync.
+
+        :param tenant_id: Required.
+        :type tenant_id: str
+        :param body: Default value is None.
+        :type body: IO
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: DataSyncOrchestrationInstance
+        :rtype: ~ignos.internal.api.client.models.DataSyncOrchestrationInstance
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace
+    def start_full_sync(
+        self, tenant_id: str, body: Optional[Union[_models.StartFullSync, IO]] = None, **kwargs: Any
+    ) -> _models.DataSyncOrchestrationInstance:
+        """start_full_sync.
+
+        :param tenant_id: Required.
+        :type tenant_id: str
+        :param body: Is either a StartFullSync type or a IO type. Default value is None.
+        :type body: ~ignos.internal.api.client.models.StartFullSync or IO
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/*+json',
+         'application/json', 'text/json'. Default value is None.
+        :paramtype content_type: str
+        :return: DataSyncOrchestrationInstance
+        :rtype: ~ignos.internal.api.client.models.DataSyncOrchestrationInstance
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[_models.DataSyncOrchestrationInstance] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "StartFullSync")
+            else:
+                _json = None
+
+        request = build_erp_sync_start_full_sync_request(
+            tenant_id=tenant_id,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+            request, stream=_stream, **kwargs
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200]:
+            map_error(status_code=response.status_code, response=response, error_map=error_map)
+            raise HttpResponseError(response=response)
+
+        deserialized = self._deserialize("DataSyncOrchestrationInstance", pipeline_response)
+
+        if cls:
+            return cls(pipeline_response, deserialized, {})
+
+        return deserialized
+
+    @overload
+    def sync_single_work_order(  # pylint: disable=inconsistent-return-statements
+        self,
+        tenant_id: str,
+        body: Optional[_models.SyncSingleWorkOrder] = None,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any
+    ) -> None:
+        """sync_single_work_order.
+
+        :param tenant_id: Required.
+        :type tenant_id: str
+        :param body: Default value is None.
+        :type body: ~ignos.internal.api.client.models.SyncSingleWorkOrder
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @overload
+    def sync_single_work_order(  # pylint: disable=inconsistent-return-statements
+        self, tenant_id: str, body: Optional[IO] = None, *, content_type: str = "application/json", **kwargs: Any
+    ) -> None:
+        """sync_single_work_order.
+
+        :param tenant_id: Required.
+        :type tenant_id: str
+        :param body: Default value is None.
+        :type body: IO
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Known values are: 'application/*+json', 'application/json', 'text/json'. Default value is
+         "application/json".
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+
+    @distributed_trace
+    def sync_single_work_order(  # pylint: disable=inconsistent-return-statements
+        self, tenant_id: str, body: Optional[Union[_models.SyncSingleWorkOrder, IO]] = None, **kwargs: Any
+    ) -> None:
+        """sync_single_work_order.
+
+        :param tenant_id: Required.
+        :type tenant_id: str
+        :param body: Is either a SyncSingleWorkOrder type or a IO type. Default value is None.
+        :type body: ~ignos.internal.api.client.models.SyncSingleWorkOrder or IO
+        :keyword content_type: Body Parameter content-type. Known values are: 'application/*+json',
+         'application/json', 'text/json'. Default value is None.
+        :paramtype content_type: str
+        :return: None
+        :rtype: None
+        :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        error_map = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
+        cls: ClsType[None] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            if body is not None:
+                _json = self._serialize.body(body, "SyncSingleWorkOrder")
+            else:
+                _json = None
+
+        request = build_erp_sync_sync_single_work_order_request(
+            tenant_id=tenant_id,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        request.url = self._client.format_url(request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
             request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
```

### Comparing `ignos-internal-api-client-20230702.0.5514/ignos/internal/api/client/operations/_patch.py` & `ignos-internal-api-client-20230719.0.5642/ignos/internal/api/client/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `ignos-internal-api-client-20230702.0.5514/ignos_internal_api_client.egg-info/SOURCES.txt` & `ignos-internal-api-client-20230719.0.5642/ignos_internal_api_client.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 ignos/internal/__init__.py
 ignos/internal/api/__init__.py
 ignos/internal/api/client/__init__.py
 ignos/internal/api/client/_client.py
 ignos/internal/api/client/_configuration.py
 ignos/internal/api/client/_patch.py
 ignos/internal/api/client/_serialization.py
-ignos/internal/api/client/_vendor.py
 ignos/internal/api/client/_version.py
 ignos/internal/api/client/aio/__init__.py
 ignos/internal/api/client/aio/_client.py
 ignos/internal/api/client/aio/_configuration.py
 ignos/internal/api/client/aio/_patch.py
 ignos/internal/api/client/aio/operations/__init__.py
 ignos/internal/api/client/aio/operations/_operations.py
```

### Comparing `ignos-internal-api-client-20230702.0.5514/setup.py` & `ignos-internal-api-client-20230719.0.5642/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 # coding: utf-8
 from setuptools import setup, find_packages
 
 
 PACKAGE_NAME = "ignos-internal-api-client"
-version = "20230702.0.5514"
+version = "20230719.0.5642"
 setup(
     name=PACKAGE_NAME,
     version=version,
     description="ignos-internal-api-client",
     author_email="",
     url="",
     keywords="azure, azure sdk",
```

