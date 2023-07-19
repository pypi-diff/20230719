# Comparing `tmp/alibabacloud_ddoscoo20200101-1.0.2.tar.gz` & `tmp/alibabacloud_ddoscoo20200101-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_ddoscoo20200101-1.0.2.tar", last modified: Thu Jun 30 07:39:51 2022, max compression
+gzip compressed data, was "dist/alibabacloud_ddoscoo20200101-1.0.3.tar", last modified: Wed Jul 19 02:37:33 2023, max compression
```

## Comparing `alibabacloud_ddoscoo20200101-1.0.2.tar` & `alibabacloud_ddoscoo20200101-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-30 07:39:51.000000 alibabacloud_ddoscoo20200101-1.0.2/
--rw-r--r--   0 root         (0) root         (0)      119 2022-06-30 07:39:51.000000 alibabacloud_ddoscoo20200101-1.0.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2022-06-30 07:39:51.000000 alibabacloud_ddoscoo20200101-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-06-30 07:39:51.000000 alibabacloud_ddoscoo20200101-1.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2352 2022-06-30 07:39:51.000000 alibabacloud_ddoscoo20200101-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1034 2022-06-30 07:39:51.000000 alibabacloud_ddoscoo20200101-1.0.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1119 2022-06-30 07:39:51.000000 alibabacloud_ddoscoo20200101-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-30 07:39:51.000000 alibabacloud_ddoscoo20200101-1.0.2/alibabacloud_ddoscoo20200101/
--rw-r--r--   0 root         (0) root         (0)       21 2022-06-30 07:39:51.000000 alibabacloud_ddoscoo20200101-1.0.2/alibabacloud_ddoscoo20200101/__init__.py
--rw-r--r--   0 root         (0) root         (0)   505769 2022-06-30 07:39:51.000000 alibabacloud_ddoscoo20200101-1.0.2/alibabacloud_ddoscoo20200101/client.py
--rw-r--r--   0 root         (0) root         (0)   727173 2022-06-30 07:39:51.000000 alibabacloud_ddoscoo20200101-1.0.2/alibabacloud_ddoscoo20200101/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-30 07:39:51.000000 alibabacloud_ddoscoo20200101-1.0.2/alibabacloud_ddoscoo20200101.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2352 2022-06-30 07:39:51.000000 alibabacloud_ddoscoo20200101-1.0.2/alibabacloud_ddoscoo20200101.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      452 2022-06-30 07:39:51.000000 alibabacloud_ddoscoo20200101-1.0.2/alibabacloud_ddoscoo20200101.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-06-30 07:39:51.000000 alibabacloud_ddoscoo20200101-1.0.2/alibabacloud_ddoscoo20200101.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2022-06-30 07:39:51.000000 alibabacloud_ddoscoo20200101-1.0.2/alibabacloud_ddoscoo20200101.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2022-06-30 07:39:51.000000 alibabacloud_ddoscoo20200101-1.0.2/alibabacloud_ddoscoo20200101.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-06-30 07:39:51.000000 alibabacloud_ddoscoo20200101-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2630 2022-06-30 07:39:51.000000 alibabacloud_ddoscoo20200101-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 02:37:33.000000 alibabacloud_ddoscoo20200101-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)      160 2023-07-19 02:37:33.000000 alibabacloud_ddoscoo20200101-1.0.3/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-19 02:37:33.000000 alibabacloud_ddoscoo20200101-1.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-19 02:37:33.000000 alibabacloud_ddoscoo20200101-1.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2352 2023-07-19 02:37:33.000000 alibabacloud_ddoscoo20200101-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1034 2023-07-19 02:37:33.000000 alibabacloud_ddoscoo20200101-1.0.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1119 2023-07-19 02:37:33.000000 alibabacloud_ddoscoo20200101-1.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 02:37:33.000000 alibabacloud_ddoscoo20200101-1.0.3/alibabacloud_ddoscoo20200101/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-19 02:37:33.000000 alibabacloud_ddoscoo20200101-1.0.3/alibabacloud_ddoscoo20200101/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   635839 2023-07-19 02:37:33.000000 alibabacloud_ddoscoo20200101-1.0.3/alibabacloud_ddoscoo20200101/client.py
+-rw-r--r--   0 root         (0) root         (0)   961220 2023-07-19 02:37:33.000000 alibabacloud_ddoscoo20200101-1.0.3/alibabacloud_ddoscoo20200101/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 02:37:33.000000 alibabacloud_ddoscoo20200101-1.0.3/alibabacloud_ddoscoo20200101.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2352 2023-07-19 02:37:33.000000 alibabacloud_ddoscoo20200101-1.0.3/alibabacloud_ddoscoo20200101.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      452 2023-07-19 02:37:33.000000 alibabacloud_ddoscoo20200101-1.0.3/alibabacloud_ddoscoo20200101.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 02:37:33.000000 alibabacloud_ddoscoo20200101-1.0.3/alibabacloud_ddoscoo20200101.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2023-07-19 02:37:33.000000 alibabacloud_ddoscoo20200101-1.0.3/alibabacloud_ddoscoo20200101.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-19 02:37:33.000000 alibabacloud_ddoscoo20200101-1.0.3/alibabacloud_ddoscoo20200101.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-19 02:37:33.000000 alibabacloud_ddoscoo20200101-1.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2631 2023-07-19 02:37:33.000000 alibabacloud_ddoscoo20200101-1.0.3/setup.py
```

### Comparing `alibabacloud_ddoscoo20200101-1.0.2/LICENSE` & `alibabacloud_ddoscoo20200101-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_ddoscoo20200101-1.0.2/PKG-INFO` & `alibabacloud_ddoscoo20200101-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_ddoscoo20200101
-Version: 1.0.2
+Version: 1.0.3
 Summary: Alibaba Cloud ddoscoo (20200101) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_ddoscoo20200101-1.0.2/README-CN.md` & `alibabacloud_ddoscoo20200101-1.0.3/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_ddoscoo20200101-1.0.2/README.md` & `alibabacloud_ddoscoo20200101-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_ddoscoo20200101-1.0.2/alibabacloud_ddoscoo20200101/client.py` & `alibabacloud_ddoscoo20200101-1.0.3/alibabacloud_ddoscoo20200101/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -120,14 +120,24 @@
         return await self.add_auto_cc_blacklist_with_options_async(request, runtime)
 
     def add_auto_cc_whitelist_with_options(
         self,
         request: ddoscoo_20200101_models.AddAutoCcWhitelistRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.AddAutoCcWhitelistResponse:
+        """
+        You can call the AddAutoCcWhitelist operation to add IP addresses to the whitelist of an Anti-DDoS Pro or Anti-DDoS Premium instance. This way, the Anti-DDoS Pro or Anti-DDoS Premium instance allows traffic from the IP addresses.
+        By default, the traffic from the IP addresses that you add to the whitelist is always allowed. If you no longer use the whitelist, you can call the [EmptyAutoCcWhitelist](~~157505~~) operation to remove the IP addresses from the whitelist.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: AddAutoCcWhitelistRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: AddAutoCcWhitelistResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.expire_time):
             query['ExpireTime'] = request.expire_time
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.whitelist):
@@ -152,14 +162,24 @@
         )
 
     async def add_auto_cc_whitelist_with_options_async(
         self,
         request: ddoscoo_20200101_models.AddAutoCcWhitelistRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.AddAutoCcWhitelistResponse:
+        """
+        You can call the AddAutoCcWhitelist operation to add IP addresses to the whitelist of an Anti-DDoS Pro or Anti-DDoS Premium instance. This way, the Anti-DDoS Pro or Anti-DDoS Premium instance allows traffic from the IP addresses.
+        By default, the traffic from the IP addresses that you add to the whitelist is always allowed. If you no longer use the whitelist, you can call the [EmptyAutoCcWhitelist](~~157505~~) operation to remove the IP addresses from the whitelist.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: AddAutoCcWhitelistRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: AddAutoCcWhitelistResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.expire_time):
             query['ExpireTime'] = request.expire_time
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.whitelist):
@@ -183,37 +203,59 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def add_auto_cc_whitelist(
         self,
         request: ddoscoo_20200101_models.AddAutoCcWhitelistRequest,
     ) -> ddoscoo_20200101_models.AddAutoCcWhitelistResponse:
+        """
+        You can call the AddAutoCcWhitelist operation to add IP addresses to the whitelist of an Anti-DDoS Pro or Anti-DDoS Premium instance. This way, the Anti-DDoS Pro or Anti-DDoS Premium instance allows traffic from the IP addresses.
+        By default, the traffic from the IP addresses that you add to the whitelist is always allowed. If you no longer use the whitelist, you can call the [EmptyAutoCcWhitelist](~~157505~~) operation to remove the IP addresses from the whitelist.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: AddAutoCcWhitelistRequest
+        @return: AddAutoCcWhitelistResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.add_auto_cc_whitelist_with_options(request, runtime)
 
     async def add_auto_cc_whitelist_async(
         self,
         request: ddoscoo_20200101_models.AddAutoCcWhitelistRequest,
     ) -> ddoscoo_20200101_models.AddAutoCcWhitelistResponse:
+        """
+        You can call the AddAutoCcWhitelist operation to add IP addresses to the whitelist of an Anti-DDoS Pro or Anti-DDoS Premium instance. This way, the Anti-DDoS Pro or Anti-DDoS Premium instance allows traffic from the IP addresses.
+        By default, the traffic from the IP addresses that you add to the whitelist is always allowed. If you no longer use the whitelist, you can call the [EmptyAutoCcWhitelist](~~157505~~) operation to remove the IP addresses from the whitelist.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: AddAutoCcWhitelistRequest
+        @return: AddAutoCcWhitelistResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.add_auto_cc_whitelist_with_options_async(request, runtime)
 
     def associate_web_cert_with_options(
         self,
         request: ddoscoo_20200101_models.AssociateWebCertRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.AssociateWebCertResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.cert):
             query['Cert'] = request.cert
         if not UtilClient.is_unset(request.cert_id):
             query['CertId'] = request.cert_id
+        if not UtilClient.is_unset(request.cert_identifier):
+            query['CertIdentifier'] = request.cert_identifier
         if not UtilClient.is_unset(request.cert_name):
             query['CertName'] = request.cert_name
+        if not UtilClient.is_unset(request.cert_region):
+            query['CertRegion'] = request.cert_region
         if not UtilClient.is_unset(request.domain):
             query['Domain'] = request.domain
         if not UtilClient.is_unset(request.key):
             query['Key'] = request.key
         if not UtilClient.is_unset(request.resource_group_id):
             query['ResourceGroupId'] = request.resource_group_id
         req = open_api_models.OpenApiRequest(
@@ -242,16 +284,20 @@
     ) -> ddoscoo_20200101_models.AssociateWebCertResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.cert):
             query['Cert'] = request.cert
         if not UtilClient.is_unset(request.cert_id):
             query['CertId'] = request.cert_id
+        if not UtilClient.is_unset(request.cert_identifier):
+            query['CertIdentifier'] = request.cert_identifier
         if not UtilClient.is_unset(request.cert_name):
             query['CertName'] = request.cert_name
+        if not UtilClient.is_unset(request.cert_region):
+            query['CertRegion'] = request.cert_region
         if not UtilClient.is_unset(request.domain):
             query['Domain'] = request.domain
         if not UtilClient.is_unset(request.key):
             query['Key'] = request.key
         if not UtilClient.is_unset(request.resource_group_id):
             query['ResourceGroupId'] = request.resource_group_id
         req = open_api_models.OpenApiRequest(
@@ -366,14 +412,21 @@
         return await self.attach_scene_defense_object_with_options_async(request, runtime)
 
     def config_l7rs_policy_with_options(
         self,
         request: ddoscoo_20200101_models.ConfigL7RsPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.ConfigL7RsPolicyResponse:
+        """
+        If multiple origin servers are configured for a website that is added to Anti-DDoS Pro or Anti-DDoS Premium, you can modify the load balancing algorithms for back-to-origin traffic based on back-to-origin policies. The IP hash algorithm is used by default. You can change the algorithm to the round-robin or least response time algorithm. For more information, see the description of the *Policy** parameter in the "Request parameters" section of this topic.
+        
+        @param request: ConfigL7RsPolicyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ConfigL7RsPolicyResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.domain):
             query['Domain'] = request.domain
         if not UtilClient.is_unset(request.policy):
             query['Policy'] = request.policy
         if not UtilClient.is_unset(request.resource_group_id):
@@ -398,14 +451,21 @@
         )
 
     async def config_l7rs_policy_with_options_async(
         self,
         request: ddoscoo_20200101_models.ConfigL7RsPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.ConfigL7RsPolicyResponse:
+        """
+        If multiple origin servers are configured for a website that is added to Anti-DDoS Pro or Anti-DDoS Premium, you can modify the load balancing algorithms for back-to-origin traffic based on back-to-origin policies. The IP hash algorithm is used by default. You can change the algorithm to the round-robin or least response time algorithm. For more information, see the description of the *Policy** parameter in the "Request parameters" section of this topic.
+        
+        @param request: ConfigL7RsPolicyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ConfigL7RsPolicyResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.domain):
             query['Domain'] = request.domain
         if not UtilClient.is_unset(request.policy):
             query['Policy'] = request.policy
         if not UtilClient.is_unset(request.resource_group_id):
@@ -429,24 +489,110 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def config_l7rs_policy(
         self,
         request: ddoscoo_20200101_models.ConfigL7RsPolicyRequest,
     ) -> ddoscoo_20200101_models.ConfigL7RsPolicyResponse:
+        """
+        If multiple origin servers are configured for a website that is added to Anti-DDoS Pro or Anti-DDoS Premium, you can modify the load balancing algorithms for back-to-origin traffic based on back-to-origin policies. The IP hash algorithm is used by default. You can change the algorithm to the round-robin or least response time algorithm. For more information, see the description of the *Policy** parameter in the "Request parameters" section of this topic.
+        
+        @param request: ConfigL7RsPolicyRequest
+        @return: ConfigL7RsPolicyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.config_l7rs_policy_with_options(request, runtime)
 
     async def config_l7rs_policy_async(
         self,
         request: ddoscoo_20200101_models.ConfigL7RsPolicyRequest,
     ) -> ddoscoo_20200101_models.ConfigL7RsPolicyResponse:
+        """
+        If multiple origin servers are configured for a website that is added to Anti-DDoS Pro or Anti-DDoS Premium, you can modify the load balancing algorithms for back-to-origin traffic based on back-to-origin policies. The IP hash algorithm is used by default. You can change the algorithm to the round-robin or least response time algorithm. For more information, see the description of the *Policy** parameter in the "Request parameters" section of this topic.
+        
+        @param request: ConfigL7RsPolicyRequest
+        @return: ConfigL7RsPolicyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.config_l7rs_policy_with_options_async(request, runtime)
 
+    def config_layer_4real_limit_with_options(
+        self,
+        request: ddoscoo_20200101_models.ConfigLayer4RealLimitRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ddoscoo_20200101_models.ConfigLayer4RealLimitResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.limit_value):
+            query['LimitValue'] = request.limit_value
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ConfigLayer4RealLimit',
+            version='2020-01-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ddoscoo_20200101_models.ConfigLayer4RealLimitResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def config_layer_4real_limit_with_options_async(
+        self,
+        request: ddoscoo_20200101_models.ConfigLayer4RealLimitRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ddoscoo_20200101_models.ConfigLayer4RealLimitResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.limit_value):
+            query['LimitValue'] = request.limit_value
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ConfigLayer4RealLimit',
+            version='2020-01-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ddoscoo_20200101_models.ConfigLayer4RealLimitResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def config_layer_4real_limit(
+        self,
+        request: ddoscoo_20200101_models.ConfigLayer4RealLimitRequest,
+    ) -> ddoscoo_20200101_models.ConfigLayer4RealLimitResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.config_layer_4real_limit_with_options(request, runtime)
+
+    async def config_layer_4real_limit_async(
+        self,
+        request: ddoscoo_20200101_models.ConfigLayer4RealLimitRequest,
+    ) -> ddoscoo_20200101_models.ConfigLayer4RealLimitResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.config_layer_4real_limit_with_options_async(request, runtime)
+
     def config_layer_4remark_with_options(
         self,
         request: ddoscoo_20200101_models.ConfigLayer4RemarkRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.ConfigLayer4RemarkResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -802,14 +948,23 @@
         return await self.config_network_rules_with_options_async(request, runtime)
 
     def config_udp_reflect_with_options(
         self,
         request: ddoscoo_20200101_models.ConfigUdpReflectRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.ConfigUdpReflectResponse:
+        """
+        You can call this operation to configure filtering policies to filter out UDP traffic from specific ports. This helps defend against UDP reflection attacks.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: ConfigUdpReflectRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ConfigUdpReflectResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.config):
             query['Config'] = request.config
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_id):
@@ -834,14 +989,23 @@
         )
 
     async def config_udp_reflect_with_options_async(
         self,
         request: ddoscoo_20200101_models.ConfigUdpReflectRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.ConfigUdpReflectResponse:
+        """
+        You can call this operation to configure filtering policies to filter out UDP traffic from specific ports. This helps defend against UDP reflection attacks.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: ConfigUdpReflectRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ConfigUdpReflectResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.config):
             query['Config'] = request.config
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_id):
@@ -865,21 +1029,37 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def config_udp_reflect(
         self,
         request: ddoscoo_20200101_models.ConfigUdpReflectRequest,
     ) -> ddoscoo_20200101_models.ConfigUdpReflectResponse:
+        """
+        You can call this operation to configure filtering policies to filter out UDP traffic from specific ports. This helps defend against UDP reflection attacks.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: ConfigUdpReflectRequest
+        @return: ConfigUdpReflectResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.config_udp_reflect_with_options(request, runtime)
 
     async def config_udp_reflect_async(
         self,
         request: ddoscoo_20200101_models.ConfigUdpReflectRequest,
     ) -> ddoscoo_20200101_models.ConfigUdpReflectResponse:
+        """
+        You can call this operation to configure filtering policies to filter out UDP traffic from specific ports. This helps defend against UDP reflection attacks.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: ConfigUdpReflectRequest
+        @return: ConfigUdpReflectResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.config_udp_reflect_with_options_async(request, runtime)
 
     def config_web_cctemplate_with_options(
         self,
         request: ddoscoo_20200101_models.ConfigWebCCTemplateRequest,
         runtime: util_models.RuntimeOptions,
@@ -1278,14 +1458,21 @@
         return await self.create_network_rules_with_options_async(request, runtime)
 
     def create_port_with_options(
         self,
         request: ddoscoo_20200101_models.CreatePortRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.CreatePortResponse:
+        """
+        You can call this operation by using Terraform. For more information about Terraform, see [What is Terraform?](~~95820~~).
+        
+        @param request: CreatePortRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreatePortResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.backend_port):
             query['BackendPort'] = request.backend_port
         if not UtilClient.is_unset(request.frontend_port):
             query['FrontendPort'] = request.frontend_port
         if not UtilClient.is_unset(request.frontend_protocol):
@@ -1314,14 +1501,21 @@
         )
 
     async def create_port_with_options_async(
         self,
         request: ddoscoo_20200101_models.CreatePortRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.CreatePortResponse:
+        """
+        You can call this operation by using Terraform. For more information about Terraform, see [What is Terraform?](~~95820~~).
+        
+        @param request: CreatePortRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreatePortResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.backend_port):
             query['BackendPort'] = request.backend_port
         if not UtilClient.is_unset(request.frontend_port):
             query['FrontendPort'] = request.frontend_port
         if not UtilClient.is_unset(request.frontend_protocol):
@@ -1349,21 +1543,33 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_port(
         self,
         request: ddoscoo_20200101_models.CreatePortRequest,
     ) -> ddoscoo_20200101_models.CreatePortResponse:
+        """
+        You can call this operation by using Terraform. For more information about Terraform, see [What is Terraform?](~~95820~~).
+        
+        @param request: CreatePortRequest
+        @return: CreatePortResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_port_with_options(request, runtime)
 
     async def create_port_async(
         self,
         request: ddoscoo_20200101_models.CreatePortRequest,
     ) -> ddoscoo_20200101_models.CreatePortResponse:
+        """
+        You can call this operation by using Terraform. For more information about Terraform, see [What is Terraform?](~~95820~~).
+        
+        @param request: CreatePortRequest
+        @return: CreatePortResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_port_with_options_async(request, runtime)
 
     def create_scene_defense_policy_with_options(
         self,
         request: ddoscoo_20200101_models.CreateSceneDefensePolicyRequest,
         runtime: util_models.RuntimeOptions,
@@ -1532,14 +1738,24 @@
         return await self.create_scheduler_rule_with_options_async(request, runtime)
 
     def create_tag_resources_with_options(
         self,
         request: ddoscoo_20200101_models.CreateTagResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.CreateTagResourcesResponse:
+        """
+        You can call the CreateTagResources operation to add a tag to multiple Anti-DDoS Pro instances at a time.
+        > Anti-DDoS Premium does not support the tag feature.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: CreateTagResourcesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateTagResourcesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_group_id):
             query['ResourceGroupId'] = request.resource_group_id
         if not UtilClient.is_unset(request.resource_ids):
@@ -1568,14 +1784,24 @@
         )
 
     async def create_tag_resources_with_options_async(
         self,
         request: ddoscoo_20200101_models.CreateTagResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.CreateTagResourcesResponse:
+        """
+        You can call the CreateTagResources operation to add a tag to multiple Anti-DDoS Pro instances at a time.
+        > Anti-DDoS Premium does not support the tag feature.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: CreateTagResourcesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateTagResourcesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_group_id):
             query['ResourceGroupId'] = request.resource_group_id
         if not UtilClient.is_unset(request.resource_ids):
@@ -1603,21 +1829,39 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_tag_resources(
         self,
         request: ddoscoo_20200101_models.CreateTagResourcesRequest,
     ) -> ddoscoo_20200101_models.CreateTagResourcesResponse:
+        """
+        You can call the CreateTagResources operation to add a tag to multiple Anti-DDoS Pro instances at a time.
+        > Anti-DDoS Premium does not support the tag feature.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: CreateTagResourcesRequest
+        @return: CreateTagResourcesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_tag_resources_with_options(request, runtime)
 
     async def create_tag_resources_async(
         self,
         request: ddoscoo_20200101_models.CreateTagResourcesRequest,
     ) -> ddoscoo_20200101_models.CreateTagResourcesResponse:
+        """
+        You can call the CreateTagResources operation to add a tag to multiple Anti-DDoS Pro instances at a time.
+        > Anti-DDoS Premium does not support the tag feature.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: CreateTagResourcesRequest
+        @return: CreateTagResourcesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_tag_resources_with_options_async(request, runtime)
 
     def create_web_ccrule_with_options(
         self,
         request: ddoscoo_20200101_models.CreateWebCCRuleRequest,
         runtime: util_models.RuntimeOptions,
@@ -2176,14 +2420,22 @@
         return await self.delete_network_rule_with_options_async(request, runtime)
 
     def delete_port_with_options(
         self,
         request: ddoscoo_20200101_models.DeletePortRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DeletePortResponse:
+        """
+        After you delete a port forwarding rule, the Anti-DDoS Pro or Anti-DDoS Premium instance no longer forwards service traffic on the Layer 4 port. Before you delete a specific port forwarding rule, make sure that the service traffic destined for the Layer 4 port is redirected to the origin server. This can prevent negative impacts on your services.
+        > You can call this operation by using Terraform. For more information about Terraform, see [What is Terraform?](~~95820~~).
+        
+        @param request: DeletePortRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeletePortResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.backend_port):
             query['BackendPort'] = request.backend_port
         if not UtilClient.is_unset(request.frontend_port):
             query['FrontendPort'] = request.frontend_port
         if not UtilClient.is_unset(request.frontend_protocol):
@@ -2212,14 +2464,22 @@
         )
 
     async def delete_port_with_options_async(
         self,
         request: ddoscoo_20200101_models.DeletePortRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DeletePortResponse:
+        """
+        After you delete a port forwarding rule, the Anti-DDoS Pro or Anti-DDoS Premium instance no longer forwards service traffic on the Layer 4 port. Before you delete a specific port forwarding rule, make sure that the service traffic destined for the Layer 4 port is redirected to the origin server. This can prevent negative impacts on your services.
+        > You can call this operation by using Terraform. For more information about Terraform, see [What is Terraform?](~~95820~~).
+        
+        @param request: DeletePortRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeletePortResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.backend_port):
             query['BackendPort'] = request.backend_port
         if not UtilClient.is_unset(request.frontend_port):
             query['FrontendPort'] = request.frontend_port
         if not UtilClient.is_unset(request.frontend_protocol):
@@ -2247,21 +2507,35 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_port(
         self,
         request: ddoscoo_20200101_models.DeletePortRequest,
     ) -> ddoscoo_20200101_models.DeletePortResponse:
+        """
+        After you delete a port forwarding rule, the Anti-DDoS Pro or Anti-DDoS Premium instance no longer forwards service traffic on the Layer 4 port. Before you delete a specific port forwarding rule, make sure that the service traffic destined for the Layer 4 port is redirected to the origin server. This can prevent negative impacts on your services.
+        > You can call this operation by using Terraform. For more information about Terraform, see [What is Terraform?](~~95820~~).
+        
+        @param request: DeletePortRequest
+        @return: DeletePortResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_port_with_options(request, runtime)
 
     async def delete_port_async(
         self,
         request: ddoscoo_20200101_models.DeletePortRequest,
     ) -> ddoscoo_20200101_models.DeletePortResponse:
+        """
+        After you delete a port forwarding rule, the Anti-DDoS Pro or Anti-DDoS Premium instance no longer forwards service traffic on the Layer 4 port. Before you delete a specific port forwarding rule, make sure that the service traffic destined for the Layer 4 port is redirected to the origin server. This can prevent negative impacts on your services.
+        > You can call this operation by using Terraform. For more information about Terraform, see [What is Terraform?](~~95820~~).
+        
+        @param request: DeletePortRequest
+        @return: DeletePortResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_port_with_options_async(request, runtime)
 
     def delete_scene_defense_policy_with_options(
         self,
         request: ddoscoo_20200101_models.DeleteSceneDefensePolicyRequest,
         runtime: util_models.RuntimeOptions,
@@ -2406,14 +2680,24 @@
         return await self.delete_scheduler_rule_with_options_async(request, runtime)
 
     def delete_tag_resources_with_options(
         self,
         request: ddoscoo_20200101_models.DeleteTagResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DeleteTagResourcesResponse:
+        """
+        You can call the DeleteTagResources operation to remove tags from Anti-DDoS Pro instances.
+        > Only Anti-DDoS Pro supports tags.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DeleteTagResourcesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteTagResourcesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.all):
             query['All'] = request.all
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_group_id):
@@ -2444,14 +2728,24 @@
         )
 
     async def delete_tag_resources_with_options_async(
         self,
         request: ddoscoo_20200101_models.DeleteTagResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DeleteTagResourcesResponse:
+        """
+        You can call the DeleteTagResources operation to remove tags from Anti-DDoS Pro instances.
+        > Only Anti-DDoS Pro supports tags.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DeleteTagResourcesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteTagResourcesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.all):
             query['All'] = request.all
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_group_id):
@@ -2481,21 +2775,39 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_tag_resources(
         self,
         request: ddoscoo_20200101_models.DeleteTagResourcesRequest,
     ) -> ddoscoo_20200101_models.DeleteTagResourcesResponse:
+        """
+        You can call the DeleteTagResources operation to remove tags from Anti-DDoS Pro instances.
+        > Only Anti-DDoS Pro supports tags.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DeleteTagResourcesRequest
+        @return: DeleteTagResourcesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_tag_resources_with_options(request, runtime)
 
     async def delete_tag_resources_async(
         self,
         request: ddoscoo_20200101_models.DeleteTagResourcesRequest,
     ) -> ddoscoo_20200101_models.DeleteTagResourcesResponse:
+        """
+        You can call the DeleteTagResources operation to remove tags from Anti-DDoS Pro instances.
+        > Only Anti-DDoS Pro supports tags.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DeleteTagResourcesRequest
+        @return: DeleteTagResourcesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_tag_resources_with_options_async(request, runtime)
 
     def delete_web_ccrule_with_options(
         self,
         request: ddoscoo_20200101_models.DeleteWebCCRuleRequest,
         runtime: util_models.RuntimeOptions,
@@ -2574,14 +2886,23 @@
         return await self.delete_web_ccrule_with_options_async(request, runtime)
 
     def delete_web_cache_custom_rule_with_options(
         self,
         request: ddoscoo_20200101_models.DeleteWebCacheCustomRuleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DeleteWebCacheCustomRuleResponse:
+        """
+        You can call the DeleteWebCacheCustomRule operation to delete the custom rules of the Static Page Caching policy for a website.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DeleteWebCacheCustomRuleRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteWebCacheCustomRuleResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.domain):
             query['Domain'] = request.domain
         if not UtilClient.is_unset(request.resource_group_id):
             query['ResourceGroupId'] = request.resource_group_id
         if not UtilClient.is_unset(request.rule_names):
@@ -2606,14 +2927,23 @@
         )
 
     async def delete_web_cache_custom_rule_with_options_async(
         self,
         request: ddoscoo_20200101_models.DeleteWebCacheCustomRuleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DeleteWebCacheCustomRuleResponse:
+        """
+        You can call the DeleteWebCacheCustomRule operation to delete the custom rules of the Static Page Caching policy for a website.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DeleteWebCacheCustomRuleRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteWebCacheCustomRuleResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.domain):
             query['Domain'] = request.domain
         if not UtilClient.is_unset(request.resource_group_id):
             query['ResourceGroupId'] = request.resource_group_id
         if not UtilClient.is_unset(request.rule_names):
@@ -2637,21 +2967,37 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_web_cache_custom_rule(
         self,
         request: ddoscoo_20200101_models.DeleteWebCacheCustomRuleRequest,
     ) -> ddoscoo_20200101_models.DeleteWebCacheCustomRuleResponse:
+        """
+        You can call the DeleteWebCacheCustomRule operation to delete the custom rules of the Static Page Caching policy for a website.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DeleteWebCacheCustomRuleRequest
+        @return: DeleteWebCacheCustomRuleResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_web_cache_custom_rule_with_options(request, runtime)
 
     async def delete_web_cache_custom_rule_async(
         self,
         request: ddoscoo_20200101_models.DeleteWebCacheCustomRuleRequest,
     ) -> ddoscoo_20200101_models.DeleteWebCacheCustomRuleResponse:
+        """
+        You can call the DeleteWebCacheCustomRule operation to delete the custom rules of the Static Page Caching policy for a website.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DeleteWebCacheCustomRuleRequest
+        @return: DeleteWebCacheCustomRuleResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_web_cache_custom_rule_with_options_async(request, runtime)
 
     def delete_web_precise_access_rule_with_options(
         self,
         request: ddoscoo_20200101_models.DeleteWebPreciseAccessRuleRequest,
         runtime: util_models.RuntimeOptions,
@@ -2804,14 +3150,23 @@
         return await self.delete_web_rule_with_options_async(request, runtime)
 
     def describe_async_tasks_with_options(
         self,
         request: ddoscoo_20200101_models.DescribeAsyncTasksRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribeAsyncTasksResponse:
+        """
+        You can call the DescribeAsyncTasks operation to query the details of asynchronous export tasks, such as the IDs, start time, end time, status, parameters, and results.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeAsyncTasksRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeAsyncTasksResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.resource_group_id):
@@ -2836,14 +3191,23 @@
         )
 
     async def describe_async_tasks_with_options_async(
         self,
         request: ddoscoo_20200101_models.DescribeAsyncTasksRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribeAsyncTasksResponse:
+        """
+        You can call the DescribeAsyncTasks operation to query the details of asynchronous export tasks, such as the IDs, start time, end time, status, parameters, and results.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeAsyncTasksRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeAsyncTasksResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.resource_group_id):
@@ -2867,21 +3231,37 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_async_tasks(
         self,
         request: ddoscoo_20200101_models.DescribeAsyncTasksRequest,
     ) -> ddoscoo_20200101_models.DescribeAsyncTasksResponse:
+        """
+        You can call the DescribeAsyncTasks operation to query the details of asynchronous export tasks, such as the IDs, start time, end time, status, parameters, and results.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeAsyncTasksRequest
+        @return: DescribeAsyncTasksResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_async_tasks_with_options(request, runtime)
 
     async def describe_async_tasks_async(
         self,
         request: ddoscoo_20200101_models.DescribeAsyncTasksRequest,
     ) -> ddoscoo_20200101_models.DescribeAsyncTasksResponse:
+        """
+        You can call the DescribeAsyncTasks operation to query the details of asynchronous export tasks, such as the IDs, start time, end time, status, parameters, and results.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeAsyncTasksRequest
+        @return: DescribeAsyncTasksResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_async_tasks_with_options_async(request, runtime)
 
     def describe_attack_analysis_max_qps_with_options(
         self,
         request: ddoscoo_20200101_models.DescribeAttackAnalysisMaxQpsRequest,
         runtime: util_models.RuntimeOptions,
@@ -3196,14 +3576,16 @@
     def describe_back_source_cidr_with_options(
         self,
         request: ddoscoo_20200101_models.DescribeBackSourceCidrRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribeBackSourceCidrResponse:
         UtilClient.validate_model(request)
         query = {}
+        if not UtilClient.is_unset(request.ip_version):
+            query['IpVersion'] = request.ip_version
         if not UtilClient.is_unset(request.line):
             query['Line'] = request.line
         if not UtilClient.is_unset(request.resource_group_id):
             query['ResourceGroupId'] = request.resource_group_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -3226,14 +3608,16 @@
     async def describe_back_source_cidr_with_options_async(
         self,
         request: ddoscoo_20200101_models.DescribeBackSourceCidrRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribeBackSourceCidrResponse:
         UtilClient.validate_model(request)
         query = {}
+        if not UtilClient.is_unset(request.ip_version):
+            query['IpVersion'] = request.ip_version
         if not UtilClient.is_unset(request.line):
             query['Line'] = request.line
         if not UtilClient.is_unset(request.resource_group_id):
             query['ResourceGroupId'] = request.resource_group_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -3338,14 +3722,24 @@
         return await self.describe_blackhole_status_with_options_async(request, runtime)
 
     def describe_block_status_with_options(
         self,
         request: ddoscoo_20200101_models.DescribeBlockStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribeBlockStatusResponse:
+        """
+        This operation is used to query the Diversion from Origin Server configurations of one or more Anti-DDoS Pro instances.
+        > This operation is suitable only for Anti-DDoS Pro.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeBlockStatusRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeBlockStatusResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_ids):
             query['InstanceIds'] = request.instance_ids
         if not UtilClient.is_unset(request.resource_group_id):
             query['ResourceGroupId'] = request.resource_group_id
         req = open_api_models.OpenApiRequest(
@@ -3368,14 +3762,24 @@
         )
 
     async def describe_block_status_with_options_async(
         self,
         request: ddoscoo_20200101_models.DescribeBlockStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribeBlockStatusResponse:
+        """
+        This operation is used to query the Diversion from Origin Server configurations of one or more Anti-DDoS Pro instances.
+        > This operation is suitable only for Anti-DDoS Pro.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeBlockStatusRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeBlockStatusResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_ids):
             query['InstanceIds'] = request.instance_ids
         if not UtilClient.is_unset(request.resource_group_id):
             query['ResourceGroupId'] = request.resource_group_id
         req = open_api_models.OpenApiRequest(
@@ -3397,21 +3801,39 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_block_status(
         self,
         request: ddoscoo_20200101_models.DescribeBlockStatusRequest,
     ) -> ddoscoo_20200101_models.DescribeBlockStatusResponse:
+        """
+        This operation is used to query the Diversion from Origin Server configurations of one or more Anti-DDoS Pro instances.
+        > This operation is suitable only for Anti-DDoS Pro.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeBlockStatusRequest
+        @return: DescribeBlockStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_block_status_with_options(request, runtime)
 
     async def describe_block_status_async(
         self,
         request: ddoscoo_20200101_models.DescribeBlockStatusRequest,
     ) -> ddoscoo_20200101_models.DescribeBlockStatusResponse:
+        """
+        This operation is used to query the Diversion from Origin Server configurations of one or more Anti-DDoS Pro instances.
+        > This operation is suitable only for Anti-DDoS Pro.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeBlockStatusRequest
+        @return: DescribeBlockStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_block_status_with_options_async(request, runtime)
 
     def describe_certs_with_options(
         self,
         request: ddoscoo_20200101_models.DescribeCertsRequest,
         runtime: util_models.RuntimeOptions,
@@ -3650,14 +4072,23 @@
         return await self.describe_ddo_sevents_with_options_async(request, runtime)
 
     def describe_ddos_all_event_list_with_options(
         self,
         request: ddoscoo_20200101_models.DescribeDDosAllEventListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribeDDosAllEventListResponse:
+        """
+        You can call the DescribeDDosAllEventList operation to query DDoS attack events within a specific time range by page. The information about a DDoS attack event includes the start time and end time of the attack, attack event type, attacked object, peak bandwidth of attack traffic, and peak packet forwarding rate.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeDDosAllEventListRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDDosAllEventListResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.end_time):
             query['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.event_type):
             query['EventType'] = request.event_type
         if not UtilClient.is_unset(request.page_number):
@@ -3686,14 +4117,23 @@
         )
 
     async def describe_ddos_all_event_list_with_options_async(
         self,
         request: ddoscoo_20200101_models.DescribeDDosAllEventListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribeDDosAllEventListResponse:
+        """
+        You can call the DescribeDDosAllEventList operation to query DDoS attack events within a specific time range by page. The information about a DDoS attack event includes the start time and end time of the attack, attack event type, attacked object, peak bandwidth of attack traffic, and peak packet forwarding rate.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeDDosAllEventListRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDDosAllEventListResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.end_time):
             query['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.event_type):
             query['EventType'] = request.event_type
         if not UtilClient.is_unset(request.page_number):
@@ -3721,29 +4161,52 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_ddos_all_event_list(
         self,
         request: ddoscoo_20200101_models.DescribeDDosAllEventListRequest,
     ) -> ddoscoo_20200101_models.DescribeDDosAllEventListResponse:
+        """
+        You can call the DescribeDDosAllEventList operation to query DDoS attack events within a specific time range by page. The information about a DDoS attack event includes the start time and end time of the attack, attack event type, attacked object, peak bandwidth of attack traffic, and peak packet forwarding rate.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeDDosAllEventListRequest
+        @return: DescribeDDosAllEventListResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_ddos_all_event_list_with_options(request, runtime)
 
     async def describe_ddos_all_event_list_async(
         self,
         request: ddoscoo_20200101_models.DescribeDDosAllEventListRequest,
     ) -> ddoscoo_20200101_models.DescribeDDosAllEventListResponse:
+        """
+        You can call the DescribeDDosAllEventList operation to query DDoS attack events within a specific time range by page. The information about a DDoS attack event includes the start time and end time of the attack, attack event type, attacked object, peak bandwidth of attack traffic, and peak packet forwarding rate.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeDDosAllEventListRequest
+        @return: DescribeDDosAllEventListResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_ddos_all_event_list_with_options_async(request, runtime)
 
     def describe_ddos_event_area_with_options(
         self,
         request: ddoscoo_20200101_models.DescribeDDosEventAreaRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribeDDosEventAreaResponse:
+        """
+        > This operation is suitable only for volumetric attacks.
+        
+        @param request: DescribeDDosEventAreaRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDDosEventAreaResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.event_type):
             query['EventType'] = request.event_type
         if not UtilClient.is_unset(request.ip):
             query['Ip'] = request.ip
         if not UtilClient.is_unset(request.start_time):
@@ -3768,14 +4231,21 @@
         )
 
     async def describe_ddos_event_area_with_options_async(
         self,
         request: ddoscoo_20200101_models.DescribeDDosEventAreaRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribeDDosEventAreaResponse:
+        """
+        > This operation is suitable only for volumetric attacks.
+        
+        @param request: DescribeDDosEventAreaRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDDosEventAreaResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.event_type):
             query['EventType'] = request.event_type
         if not UtilClient.is_unset(request.ip):
             query['Ip'] = request.ip
         if not UtilClient.is_unset(request.start_time):
@@ -3799,29 +4269,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_ddos_event_area(
         self,
         request: ddoscoo_20200101_models.DescribeDDosEventAreaRequest,
     ) -> ddoscoo_20200101_models.DescribeDDosEventAreaResponse:
+        """
+        > This operation is suitable only for volumetric attacks.
+        
+        @param request: DescribeDDosEventAreaRequest
+        @return: DescribeDDosEventAreaResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_ddos_event_area_with_options(request, runtime)
 
     async def describe_ddos_event_area_async(
         self,
         request: ddoscoo_20200101_models.DescribeDDosEventAreaRequest,
     ) -> ddoscoo_20200101_models.DescribeDDosEventAreaResponse:
+        """
+        > This operation is suitable only for volumetric attacks.
+        
+        @param request: DescribeDDosEventAreaRequest
+        @return: DescribeDDosEventAreaResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_ddos_event_area_with_options_async(request, runtime)
 
     def describe_ddos_event_attack_type_with_options(
         self,
         request: ddoscoo_20200101_models.DescribeDDosEventAttackTypeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribeDDosEventAttackTypeResponse:
+        """
+        > This operation is suitable only for volumetric attacks.
+        
+        @param request: DescribeDDosEventAttackTypeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDDosEventAttackTypeResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.event_type):
             query['EventType'] = request.event_type
         if not UtilClient.is_unset(request.ip):
             query['Ip'] = request.ip
         if not UtilClient.is_unset(request.start_time):
@@ -3846,14 +4335,21 @@
         )
 
     async def describe_ddos_event_attack_type_with_options_async(
         self,
         request: ddoscoo_20200101_models.DescribeDDosEventAttackTypeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribeDDosEventAttackTypeResponse:
+        """
+        > This operation is suitable only for volumetric attacks.
+        
+        @param request: DescribeDDosEventAttackTypeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDDosEventAttackTypeResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.event_type):
             query['EventType'] = request.event_type
         if not UtilClient.is_unset(request.ip):
             query['Ip'] = request.ip
         if not UtilClient.is_unset(request.start_time):
@@ -3877,29 +4373,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_ddos_event_attack_type(
         self,
         request: ddoscoo_20200101_models.DescribeDDosEventAttackTypeRequest,
     ) -> ddoscoo_20200101_models.DescribeDDosEventAttackTypeResponse:
+        """
+        > This operation is suitable only for volumetric attacks.
+        
+        @param request: DescribeDDosEventAttackTypeRequest
+        @return: DescribeDDosEventAttackTypeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_ddos_event_attack_type_with_options(request, runtime)
 
     async def describe_ddos_event_attack_type_async(
         self,
         request: ddoscoo_20200101_models.DescribeDDosEventAttackTypeRequest,
     ) -> ddoscoo_20200101_models.DescribeDDosEventAttackTypeResponse:
+        """
+        > This operation is suitable only for volumetric attacks.
+        
+        @param request: DescribeDDosEventAttackTypeRequest
+        @return: DescribeDDosEventAttackTypeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_ddos_event_attack_type_with_options_async(request, runtime)
 
     def describe_ddos_event_isp_with_options(
         self,
         request: ddoscoo_20200101_models.DescribeDDosEventIspRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribeDDosEventIspResponse:
+        """
+        > This operation is suitable only for volumetric attacks.
+        
+        @param request: DescribeDDosEventIspRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDDosEventIspResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.event_type):
             query['EventType'] = request.event_type
         if not UtilClient.is_unset(request.ip):
             query['Ip'] = request.ip
         if not UtilClient.is_unset(request.start_time):
@@ -3924,14 +4439,21 @@
         )
 
     async def describe_ddos_event_isp_with_options_async(
         self,
         request: ddoscoo_20200101_models.DescribeDDosEventIspRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribeDDosEventIspResponse:
+        """
+        > This operation is suitable only for volumetric attacks.
+        
+        @param request: DescribeDDosEventIspRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDDosEventIspResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.event_type):
             query['EventType'] = request.event_type
         if not UtilClient.is_unset(request.ip):
             query['Ip'] = request.ip
         if not UtilClient.is_unset(request.start_time):
@@ -3955,21 +4477,33 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_ddos_event_isp(
         self,
         request: ddoscoo_20200101_models.DescribeDDosEventIspRequest,
     ) -> ddoscoo_20200101_models.DescribeDDosEventIspResponse:
+        """
+        > This operation is suitable only for volumetric attacks.
+        
+        @param request: DescribeDDosEventIspRequest
+        @return: DescribeDDosEventIspResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_ddos_event_isp_with_options(request, runtime)
 
     async def describe_ddos_event_isp_async(
         self,
         request: ddoscoo_20200101_models.DescribeDDosEventIspRequest,
     ) -> ddoscoo_20200101_models.DescribeDDosEventIspResponse:
+        """
+        > This operation is suitable only for volumetric attacks.
+        
+        @param request: DescribeDDosEventIspRequest
+        @return: DescribeDDosEventIspResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_ddos_event_isp_with_options_async(request, runtime)
 
     def describe_ddos_event_max_with_options(
         self,
         request: ddoscoo_20200101_models.DescribeDDosEventMaxRequest,
         runtime: util_models.RuntimeOptions,
@@ -4044,14 +4578,21 @@
         return await self.describe_ddos_event_max_with_options_async(request, runtime)
 
     def describe_ddos_event_src_ip_with_options(
         self,
         request: ddoscoo_20200101_models.DescribeDDosEventSrcIpRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribeDDosEventSrcIpResponse:
+        """
+        > This operation is suitable only for volumetric attacks.
+        
+        @param request: DescribeDDosEventSrcIpRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDDosEventSrcIpResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.event_type):
             query['EventType'] = request.event_type
         if not UtilClient.is_unset(request.ip):
             query['Ip'] = request.ip
         if not UtilClient.is_unset(request.range):
@@ -4078,14 +4619,21 @@
         )
 
     async def describe_ddos_event_src_ip_with_options_async(
         self,
         request: ddoscoo_20200101_models.DescribeDDosEventSrcIpRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribeDDosEventSrcIpResponse:
+        """
+        > This operation is suitable only for volumetric attacks.
+        
+        @param request: DescribeDDosEventSrcIpRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDDosEventSrcIpResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.event_type):
             query['EventType'] = request.event_type
         if not UtilClient.is_unset(request.ip):
             query['Ip'] = request.ip
         if not UtilClient.is_unset(request.range):
@@ -4111,29 +4659,51 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_ddos_event_src_ip(
         self,
         request: ddoscoo_20200101_models.DescribeDDosEventSrcIpRequest,
     ) -> ddoscoo_20200101_models.DescribeDDosEventSrcIpResponse:
+        """
+        > This operation is suitable only for volumetric attacks.
+        
+        @param request: DescribeDDosEventSrcIpRequest
+        @return: DescribeDDosEventSrcIpResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_ddos_event_src_ip_with_options(request, runtime)
 
     async def describe_ddos_event_src_ip_async(
         self,
         request: ddoscoo_20200101_models.DescribeDDosEventSrcIpRequest,
     ) -> ddoscoo_20200101_models.DescribeDDosEventSrcIpResponse:
+        """
+        > This operation is suitable only for volumetric attacks.
+        
+        @param request: DescribeDDosEventSrcIpRequest
+        @return: DescribeDDosEventSrcIpResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_ddos_event_src_ip_with_options_async(request, runtime)
 
     def describe_defense_count_statistics_with_options(
         self,
         request: ddoscoo_20200101_models.DescribeDefenseCountStatisticsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribeDefenseCountStatisticsResponse:
+        """
+        You can call the DescribeDefenseCountStatistics operation to query the information about advanced mitigation sessions of an Anti-DDoS Premium instance. For example, you can query the number of advanced mitigation sessions that are used within the current calendar month and the number of available global advanced mitigation sessions.
+        > This operation is suitable only for Anti-DDoS Premium.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeDefenseCountStatisticsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDefenseCountStatisticsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.resource_group_id):
             query['ResourceGroupId'] = request.resource_group_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -4154,14 +4724,24 @@
         )
 
     async def describe_defense_count_statistics_with_options_async(
         self,
         request: ddoscoo_20200101_models.DescribeDefenseCountStatisticsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribeDefenseCountStatisticsResponse:
+        """
+        You can call the DescribeDefenseCountStatistics operation to query the information about advanced mitigation sessions of an Anti-DDoS Premium instance. For example, you can query the number of advanced mitigation sessions that are used within the current calendar month and the number of available global advanced mitigation sessions.
+        > This operation is suitable only for Anti-DDoS Premium.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeDefenseCountStatisticsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDefenseCountStatisticsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.resource_group_id):
             query['ResourceGroupId'] = request.resource_group_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -4181,29 +4761,54 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_defense_count_statistics(
         self,
         request: ddoscoo_20200101_models.DescribeDefenseCountStatisticsRequest,
     ) -> ddoscoo_20200101_models.DescribeDefenseCountStatisticsResponse:
+        """
+        You can call the DescribeDefenseCountStatistics operation to query the information about advanced mitigation sessions of an Anti-DDoS Premium instance. For example, you can query the number of advanced mitigation sessions that are used within the current calendar month and the number of available global advanced mitigation sessions.
+        > This operation is suitable only for Anti-DDoS Premium.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeDefenseCountStatisticsRequest
+        @return: DescribeDefenseCountStatisticsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_defense_count_statistics_with_options(request, runtime)
 
     async def describe_defense_count_statistics_async(
         self,
         request: ddoscoo_20200101_models.DescribeDefenseCountStatisticsRequest,
     ) -> ddoscoo_20200101_models.DescribeDefenseCountStatisticsResponse:
+        """
+        You can call the DescribeDefenseCountStatistics operation to query the information about advanced mitigation sessions of an Anti-DDoS Premium instance. For example, you can query the number of advanced mitigation sessions that are used within the current calendar month and the number of available global advanced mitigation sessions.
+        > This operation is suitable only for Anti-DDoS Premium.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeDefenseCountStatisticsRequest
+        @return: DescribeDefenseCountStatisticsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_defense_count_statistics_with_options_async(request, runtime)
 
     def describe_defense_records_with_options(
         self,
         request: ddoscoo_20200101_models.DescribeDefenseRecordsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribeDefenseRecordsResponse:
+        """
+        > This operation is suitable only for Anti-DDoS Premium.
+        
+        @param request: DescribeDefenseRecordsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDefenseRecordsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.end_time):
             query['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.page_number):
@@ -4234,14 +4839,21 @@
         )
 
     async def describe_defense_records_with_options_async(
         self,
         request: ddoscoo_20200101_models.DescribeDefenseRecordsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribeDefenseRecordsResponse:
+        """
+        > This operation is suitable only for Anti-DDoS Premium.
+        
+        @param request: DescribeDefenseRecordsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDefenseRecordsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.end_time):
             query['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.page_number):
@@ -4271,21 +4883,33 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_defense_records(
         self,
         request: ddoscoo_20200101_models.DescribeDefenseRecordsRequest,
     ) -> ddoscoo_20200101_models.DescribeDefenseRecordsResponse:
+        """
+        > This operation is suitable only for Anti-DDoS Premium.
+        
+        @param request: DescribeDefenseRecordsRequest
+        @return: DescribeDefenseRecordsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_defense_records_with_options(request, runtime)
 
     async def describe_defense_records_async(
         self,
         request: ddoscoo_20200101_models.DescribeDefenseRecordsRequest,
     ) -> ddoscoo_20200101_models.DescribeDefenseRecordsResponse:
+        """
+        > This operation is suitable only for Anti-DDoS Premium.
+        
+        @param request: DescribeDefenseRecordsRequest
+        @return: DescribeDefenseRecordsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_defense_records_with_options_async(request, runtime)
 
     def describe_domain_attack_events_with_options(
         self,
         request: ddoscoo_20200101_models.DescribeDomainAttackEventsRequest,
         runtime: util_models.RuntimeOptions,
@@ -4626,14 +5250,24 @@
         return await self.describe_domain_qps_with_cache_with_options_async(request, runtime)
 
     def describe_domain_resource_with_options(
         self,
         request: ddoscoo_20200101_models.DescribeDomainResourceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribeDomainResourceResponse:
+        """
+        You can call the DescribeDomainResource operation to query the configurations of the forwarding rules that you create for a website by page. The configurations include the domain name-related configurations, protocol-related configurations, HTTPS-related configurations, and configurations that are used to mitigate HTTP flood attacks.
+        You can call this operation by using Terraform. For more information about Terraform, see [What is Terraform?](~~95820~~).
+        ### Limits
+        You can call this operation up to 50 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeDomainResourceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDomainResourceResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.domain):
             query['Domain'] = request.domain
         if not UtilClient.is_unset(request.instance_ids):
             query['InstanceIds'] = request.instance_ids
         if not UtilClient.is_unset(request.page_number):
@@ -4662,14 +5296,24 @@
         )
 
     async def describe_domain_resource_with_options_async(
         self,
         request: ddoscoo_20200101_models.DescribeDomainResourceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribeDomainResourceResponse:
+        """
+        You can call the DescribeDomainResource operation to query the configurations of the forwarding rules that you create for a website by page. The configurations include the domain name-related configurations, protocol-related configurations, HTTPS-related configurations, and configurations that are used to mitigate HTTP flood attacks.
+        You can call this operation by using Terraform. For more information about Terraform, see [What is Terraform?](~~95820~~).
+        ### Limits
+        You can call this operation up to 50 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeDomainResourceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDomainResourceResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.domain):
             query['Domain'] = request.domain
         if not UtilClient.is_unset(request.instance_ids):
             query['InstanceIds'] = request.instance_ids
         if not UtilClient.is_unset(request.page_number):
@@ -4697,24 +5341,112 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_domain_resource(
         self,
         request: ddoscoo_20200101_models.DescribeDomainResourceRequest,
     ) -> ddoscoo_20200101_models.DescribeDomainResourceResponse:
+        """
+        You can call the DescribeDomainResource operation to query the configurations of the forwarding rules that you create for a website by page. The configurations include the domain name-related configurations, protocol-related configurations, HTTPS-related configurations, and configurations that are used to mitigate HTTP flood attacks.
+        You can call this operation by using Terraform. For more information about Terraform, see [What is Terraform?](~~95820~~).
+        ### Limits
+        You can call this operation up to 50 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeDomainResourceRequest
+        @return: DescribeDomainResourceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_domain_resource_with_options(request, runtime)
 
     async def describe_domain_resource_async(
         self,
         request: ddoscoo_20200101_models.DescribeDomainResourceRequest,
     ) -> ddoscoo_20200101_models.DescribeDomainResourceResponse:
+        """
+        You can call the DescribeDomainResource operation to query the configurations of the forwarding rules that you create for a website by page. The configurations include the domain name-related configurations, protocol-related configurations, HTTPS-related configurations, and configurations that are used to mitigate HTTP flood attacks.
+        You can call this operation by using Terraform. For more information about Terraform, see [What is Terraform?](~~95820~~).
+        ### Limits
+        You can call this operation up to 50 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeDomainResourceRequest
+        @return: DescribeDomainResourceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_domain_resource_with_options_async(request, runtime)
 
+    def describe_domain_security_profile_with_options(
+        self,
+        request: ddoscoo_20200101_models.DescribeDomainSecurityProfileRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ddoscoo_20200101_models.DescribeDomainSecurityProfileResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.domain):
+            query['Domain'] = request.domain
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeDomainSecurityProfile',
+            version='2020-01-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ddoscoo_20200101_models.DescribeDomainSecurityProfileResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def describe_domain_security_profile_with_options_async(
+        self,
+        request: ddoscoo_20200101_models.DescribeDomainSecurityProfileRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ddoscoo_20200101_models.DescribeDomainSecurityProfileResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.domain):
+            query['Domain'] = request.domain
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeDomainSecurityProfile',
+            version='2020-01-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ddoscoo_20200101_models.DescribeDomainSecurityProfileResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_domain_security_profile(
+        self,
+        request: ddoscoo_20200101_models.DescribeDomainSecurityProfileRequest,
+    ) -> ddoscoo_20200101_models.DescribeDomainSecurityProfileResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_domain_security_profile_with_options(request, runtime)
+
+    async def describe_domain_security_profile_async(
+        self,
+        request: ddoscoo_20200101_models.DescribeDomainSecurityProfileRequest,
+    ) -> ddoscoo_20200101_models.DescribeDomainSecurityProfileResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_domain_security_profile_with_options_async(request, runtime)
+
     def describe_domain_status_code_count_with_options(
         self,
         request: ddoscoo_20200101_models.DescribeDomainStatusCodeCountRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribeDomainStatusCodeCountResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -5372,14 +6104,21 @@
         return await self.describe_domains_with_options_async(request, runtime)
 
     def describe_elastic_bandwidth_spec_with_options(
         self,
         request: ddoscoo_20200101_models.DescribeElasticBandwidthSpecRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribeElasticBandwidthSpecResponse:
+        """
+        > This operation is suitable only for Anti-DDoS Pro.
+        
+        @param request: DescribeElasticBandwidthSpecRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeElasticBandwidthSpecResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -5400,14 +6139,21 @@
         )
 
     async def describe_elastic_bandwidth_spec_with_options_async(
         self,
         request: ddoscoo_20200101_models.DescribeElasticBandwidthSpecRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribeElasticBandwidthSpecResponse:
+        """
+        > This operation is suitable only for Anti-DDoS Pro.
+        
+        @param request: DescribeElasticBandwidthSpecRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeElasticBandwidthSpecResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -5427,24 +6173,110 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_elastic_bandwidth_spec(
         self,
         request: ddoscoo_20200101_models.DescribeElasticBandwidthSpecRequest,
     ) -> ddoscoo_20200101_models.DescribeElasticBandwidthSpecResponse:
+        """
+        > This operation is suitable only for Anti-DDoS Pro.
+        
+        @param request: DescribeElasticBandwidthSpecRequest
+        @return: DescribeElasticBandwidthSpecResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_elastic_bandwidth_spec_with_options(request, runtime)
 
     async def describe_elastic_bandwidth_spec_async(
         self,
         request: ddoscoo_20200101_models.DescribeElasticBandwidthSpecRequest,
     ) -> ddoscoo_20200101_models.DescribeElasticBandwidthSpecResponse:
+        """
+        > This operation is suitable only for Anti-DDoS Pro.
+        
+        @param request: DescribeElasticBandwidthSpecRequest
+        @return: DescribeElasticBandwidthSpecResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_elastic_bandwidth_spec_with_options_async(request, runtime)
 
+    def describe_headers_with_options(
+        self,
+        request: ddoscoo_20200101_models.DescribeHeadersRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ddoscoo_20200101_models.DescribeHeadersResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.domain):
+            query['Domain'] = request.domain
+        if not UtilClient.is_unset(request.resource_group_id):
+            query['ResourceGroupId'] = request.resource_group_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeHeaders',
+            version='2020-01-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ddoscoo_20200101_models.DescribeHeadersResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def describe_headers_with_options_async(
+        self,
+        request: ddoscoo_20200101_models.DescribeHeadersRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ddoscoo_20200101_models.DescribeHeadersResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.domain):
+            query['Domain'] = request.domain
+        if not UtilClient.is_unset(request.resource_group_id):
+            query['ResourceGroupId'] = request.resource_group_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeHeaders',
+            version='2020-01-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ddoscoo_20200101_models.DescribeHeadersResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_headers(
+        self,
+        request: ddoscoo_20200101_models.DescribeHeadersRequest,
+    ) -> ddoscoo_20200101_models.DescribeHeadersResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_headers_with_options(request, runtime)
+
+    async def describe_headers_async(
+        self,
+        request: ddoscoo_20200101_models.DescribeHeadersRequest,
+    ) -> ddoscoo_20200101_models.DescribeHeadersResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_headers_with_options_async(request, runtime)
+
     def describe_health_check_list_with_options(
         self,
         request: ddoscoo_20200101_models.DescribeHealthCheckListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribeHealthCheckListResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -5582,14 +6414,23 @@
         return await self.describe_health_check_status_with_options_async(request, runtime)
 
     def describe_instance_details_with_options(
         self,
         request: ddoscoo_20200101_models.DescribeInstanceDetailsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribeInstanceDetailsResponse:
+        """
+        You can call the DescribeInstanceDetails operation to query the information about the IP addresses and ISP lines of the instances. The information includes the IP address, status, and protection line.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeInstanceDetailsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeInstanceDetailsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_ids):
             query['InstanceIds'] = request.instance_ids
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -5610,14 +6451,23 @@
         )
 
     async def describe_instance_details_with_options_async(
         self,
         request: ddoscoo_20200101_models.DescribeInstanceDetailsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribeInstanceDetailsResponse:
+        """
+        You can call the DescribeInstanceDetails operation to query the information about the IP addresses and ISP lines of the instances. The information includes the IP address, status, and protection line.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeInstanceDetailsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeInstanceDetailsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_ids):
             query['InstanceIds'] = request.instance_ids
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -5637,21 +6487,37 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_instance_details(
         self,
         request: ddoscoo_20200101_models.DescribeInstanceDetailsRequest,
     ) -> ddoscoo_20200101_models.DescribeInstanceDetailsResponse:
+        """
+        You can call the DescribeInstanceDetails operation to query the information about the IP addresses and ISP lines of the instances. The information includes the IP address, status, and protection line.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeInstanceDetailsRequest
+        @return: DescribeInstanceDetailsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_instance_details_with_options(request, runtime)
 
     async def describe_instance_details_async(
         self,
         request: ddoscoo_20200101_models.DescribeInstanceDetailsRequest,
     ) -> ddoscoo_20200101_models.DescribeInstanceDetailsResponse:
+        """
+        You can call the DescribeInstanceDetails operation to query the information about the IP addresses and ISP lines of the instances. The information includes the IP address, status, and protection line.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeInstanceDetailsRequest
+        @return: DescribeInstanceDetailsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_instance_details_with_options_async(request, runtime)
 
     def describe_instance_ids_with_options(
         self,
         request: ddoscoo_20200101_models.DescribeInstanceIdsRequest,
         runtime: util_models.RuntimeOptions,
@@ -5730,14 +6596,23 @@
         return await self.describe_instance_ids_with_options_async(request, runtime)
 
     def describe_instance_specs_with_options(
         self,
         request: ddoscoo_20200101_models.DescribeInstanceSpecsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribeInstanceSpecsResponse:
+        """
+        You can call the DescribeInstanceSpecs operation to query the specifications of multiple Anti-DDoS Pro or Anti-DDoS Premium instances at a time. The specifications include the clean bandwidth, protection bandwidth, function plan, and the numbers of domain names and ports that can be protected.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeInstanceSpecsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeInstanceSpecsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_ids):
             query['InstanceIds'] = request.instance_ids
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -5758,14 +6633,23 @@
         )
 
     async def describe_instance_specs_with_options_async(
         self,
         request: ddoscoo_20200101_models.DescribeInstanceSpecsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribeInstanceSpecsResponse:
+        """
+        You can call the DescribeInstanceSpecs operation to query the specifications of multiple Anti-DDoS Pro or Anti-DDoS Premium instances at a time. The specifications include the clean bandwidth, protection bandwidth, function plan, and the numbers of domain names and ports that can be protected.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeInstanceSpecsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeInstanceSpecsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_ids):
             query['InstanceIds'] = request.instance_ids
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -5785,21 +6669,37 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_instance_specs(
         self,
         request: ddoscoo_20200101_models.DescribeInstanceSpecsRequest,
     ) -> ddoscoo_20200101_models.DescribeInstanceSpecsResponse:
+        """
+        You can call the DescribeInstanceSpecs operation to query the specifications of multiple Anti-DDoS Pro or Anti-DDoS Premium instances at a time. The specifications include the clean bandwidth, protection bandwidth, function plan, and the numbers of domain names and ports that can be protected.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeInstanceSpecsRequest
+        @return: DescribeInstanceSpecsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_instance_specs_with_options(request, runtime)
 
     async def describe_instance_specs_async(
         self,
         request: ddoscoo_20200101_models.DescribeInstanceSpecsRequest,
     ) -> ddoscoo_20200101_models.DescribeInstanceSpecsResponse:
+        """
+        You can call the DescribeInstanceSpecs operation to query the specifications of multiple Anti-DDoS Pro or Anti-DDoS Premium instances at a time. The specifications include the clean bandwidth, protection bandwidth, function plan, and the numbers of domain names and ports that can be protected.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeInstanceSpecsRequest
+        @return: DescribeInstanceSpecsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_instance_specs_with_options_async(request, runtime)
 
     def describe_instance_statistics_with_options(
         self,
         request: ddoscoo_20200101_models.DescribeInstanceStatisticsRequest,
         runtime: util_models.RuntimeOptions,
@@ -5944,14 +6844,21 @@
         return await self.describe_instance_status_with_options_async(request, runtime)
 
     def describe_instances_with_options(
         self,
         request: ddoscoo_20200101_models.DescribeInstancesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribeInstancesResponse:
+        """
+        You can call the DescribeInstances operation to query the details of Anti-DDoS Pro or Anti-DDoS Premium instances within the Alibaba Cloud account by page. The details include the ID, mitigation plan, expiration time, and forwarding status.
+        
+        @param request: DescribeInstancesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeInstancesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.edition):
             query['Edition'] = request.edition
         if not UtilClient.is_unset(request.enabled):
             query['Enabled'] = request.enabled
         if not UtilClient.is_unset(request.expire_end_time):
@@ -5994,14 +6901,21 @@
         )
 
     async def describe_instances_with_options_async(
         self,
         request: ddoscoo_20200101_models.DescribeInstancesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribeInstancesResponse:
+        """
+        You can call the DescribeInstances operation to query the details of Anti-DDoS Pro or Anti-DDoS Premium instances within the Alibaba Cloud account by page. The details include the ID, mitigation plan, expiration time, and forwarding status.
+        
+        @param request: DescribeInstancesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeInstancesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.edition):
             query['Edition'] = request.edition
         if not UtilClient.is_unset(request.enabled):
             query['Enabled'] = request.enabled
         if not UtilClient.is_unset(request.expire_end_time):
@@ -6043,21 +6957,33 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_instances(
         self,
         request: ddoscoo_20200101_models.DescribeInstancesRequest,
     ) -> ddoscoo_20200101_models.DescribeInstancesResponse:
+        """
+        You can call the DescribeInstances operation to query the details of Anti-DDoS Pro or Anti-DDoS Premium instances within the Alibaba Cloud account by page. The details include the ID, mitigation plan, expiration time, and forwarding status.
+        
+        @param request: DescribeInstancesRequest
+        @return: DescribeInstancesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_instances_with_options(request, runtime)
 
     async def describe_instances_async(
         self,
         request: ddoscoo_20200101_models.DescribeInstancesRequest,
     ) -> ddoscoo_20200101_models.DescribeInstancesResponse:
+        """
+        You can call the DescribeInstances operation to query the details of Anti-DDoS Pro or Anti-DDoS Premium instances within the Alibaba Cloud account by page. The details include the ID, mitigation plan, expiration time, and forwarding status.
+        
+        @param request: DescribeInstancesRequest
+        @return: DescribeInstancesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_instances_with_options_async(request, runtime)
 
     def describe_l7rs_policy_with_options(
         self,
         request: ddoscoo_20200101_models.DescribeL7RsPolicyRequest,
         runtime: util_models.RuntimeOptions,
@@ -6502,14 +7428,22 @@
         return await self.describe_network_rules_with_options_async(request, runtime)
 
     def describe_op_entities_with_options(
         self,
         request: ddoscoo_20200101_models.DescribeOpEntitiesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribeOpEntitiesResponse:
+        """
+        > This operation is suitable only for Anti-DDoS Pro.
+        You can query operations performed on Anti-DDoS Pro, such as configuring burstable protection bandwidth, deactivating blackhole filtering, configuring the Diversion from Origin Server policy, using Anti-DDoS plans, changing the IP addresses of Elastic Compute Service (ECS) instances, and clearing all logs.
+        
+        @param request: DescribeOpEntitiesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeOpEntitiesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.end_time):
             query['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.entity_object):
             query['EntityObject'] = request.entity_object
         if not UtilClient.is_unset(request.entity_type):
@@ -6542,14 +7476,22 @@
         )
 
     async def describe_op_entities_with_options_async(
         self,
         request: ddoscoo_20200101_models.DescribeOpEntitiesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribeOpEntitiesResponse:
+        """
+        > This operation is suitable only for Anti-DDoS Pro.
+        You can query operations performed on Anti-DDoS Pro, such as configuring burstable protection bandwidth, deactivating blackhole filtering, configuring the Diversion from Origin Server policy, using Anti-DDoS plans, changing the IP addresses of Elastic Compute Service (ECS) instances, and clearing all logs.
+        
+        @param request: DescribeOpEntitiesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeOpEntitiesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.end_time):
             query['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.entity_object):
             query['EntityObject'] = request.entity_object
         if not UtilClient.is_unset(request.entity_type):
@@ -6581,29 +7523,50 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_op_entities(
         self,
         request: ddoscoo_20200101_models.DescribeOpEntitiesRequest,
     ) -> ddoscoo_20200101_models.DescribeOpEntitiesResponse:
+        """
+        > This operation is suitable only for Anti-DDoS Pro.
+        You can query operations performed on Anti-DDoS Pro, such as configuring burstable protection bandwidth, deactivating blackhole filtering, configuring the Diversion from Origin Server policy, using Anti-DDoS plans, changing the IP addresses of Elastic Compute Service (ECS) instances, and clearing all logs.
+        
+        @param request: DescribeOpEntitiesRequest
+        @return: DescribeOpEntitiesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_op_entities_with_options(request, runtime)
 
     async def describe_op_entities_async(
         self,
         request: ddoscoo_20200101_models.DescribeOpEntitiesRequest,
     ) -> ddoscoo_20200101_models.DescribeOpEntitiesResponse:
+        """
+        > This operation is suitable only for Anti-DDoS Pro.
+        You can query operations performed on Anti-DDoS Pro, such as configuring burstable protection bandwidth, deactivating blackhole filtering, configuring the Diversion from Origin Server policy, using Anti-DDoS plans, changing the IP addresses of Elastic Compute Service (ECS) instances, and clearing all logs.
+        
+        @param request: DescribeOpEntitiesRequest
+        @return: DescribeOpEntitiesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_op_entities_with_options_async(request, runtime)
 
     def describe_port_with_options(
         self,
         request: ddoscoo_20200101_models.DescribePortRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribePortResponse:
+        """
+        You can call this operation by using Terraform. For more information about Terraform, see [What is Terraform?](~~95820~~).
+        
+        @param request: DescribePortRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribePortResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.frontend_port):
             query['FrontendPort'] = request.frontend_port
         if not UtilClient.is_unset(request.frontend_protocol):
             query['FrontendProtocol'] = request.frontend_protocol
         if not UtilClient.is_unset(request.instance_id):
@@ -6632,14 +7595,21 @@
         )
 
     async def describe_port_with_options_async(
         self,
         request: ddoscoo_20200101_models.DescribePortRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribePortResponse:
+        """
+        You can call this operation by using Terraform. For more information about Terraform, see [What is Terraform?](~~95820~~).
+        
+        @param request: DescribePortRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribePortResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.frontend_port):
             query['FrontendPort'] = request.frontend_port
         if not UtilClient.is_unset(request.frontend_protocol):
             query['FrontendProtocol'] = request.frontend_protocol
         if not UtilClient.is_unset(request.instance_id):
@@ -6667,29 +7637,50 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_port(
         self,
         request: ddoscoo_20200101_models.DescribePortRequest,
     ) -> ddoscoo_20200101_models.DescribePortResponse:
+        """
+        You can call this operation by using Terraform. For more information about Terraform, see [What is Terraform?](~~95820~~).
+        
+        @param request: DescribePortRequest
+        @return: DescribePortResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_port_with_options(request, runtime)
 
     async def describe_port_async(
         self,
         request: ddoscoo_20200101_models.DescribePortRequest,
     ) -> ddoscoo_20200101_models.DescribePortResponse:
+        """
+        You can call this operation by using Terraform. For more information about Terraform, see [What is Terraform?](~~95820~~).
+        
+        @param request: DescribePortRequest
+        @return: DescribePortResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_port_with_options_async(request, runtime)
 
     def describe_port_attack_max_flow_with_options(
         self,
         request: ddoscoo_20200101_models.DescribePortAttackMaxFlowRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribePortAttackMaxFlowResponse:
+        """
+        You can call this operation to query the peak bandwidth and peak packet rate of attack traffic on one or more Anti-DDoS Pro or Anti-DDoS Premium instances within a specific period of time.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribePortAttackMaxFlowRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribePortAttackMaxFlowResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.end_time):
             query['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.instance_ids):
             query['InstanceIds'] = request.instance_ids
         if not UtilClient.is_unset(request.resource_group_id):
@@ -6716,14 +7707,23 @@
         )
 
     async def describe_port_attack_max_flow_with_options_async(
         self,
         request: ddoscoo_20200101_models.DescribePortAttackMaxFlowRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribePortAttackMaxFlowResponse:
+        """
+        You can call this operation to query the peak bandwidth and peak packet rate of attack traffic on one or more Anti-DDoS Pro or Anti-DDoS Premium instances within a specific period of time.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribePortAttackMaxFlowRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribePortAttackMaxFlowResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.end_time):
             query['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.instance_ids):
             query['InstanceIds'] = request.instance_ids
         if not UtilClient.is_unset(request.resource_group_id):
@@ -6749,21 +7749,37 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_port_attack_max_flow(
         self,
         request: ddoscoo_20200101_models.DescribePortAttackMaxFlowRequest,
     ) -> ddoscoo_20200101_models.DescribePortAttackMaxFlowResponse:
+        """
+        You can call this operation to query the peak bandwidth and peak packet rate of attack traffic on one or more Anti-DDoS Pro or Anti-DDoS Premium instances within a specific period of time.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribePortAttackMaxFlowRequest
+        @return: DescribePortAttackMaxFlowResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_port_attack_max_flow_with_options(request, runtime)
 
     async def describe_port_attack_max_flow_async(
         self,
         request: ddoscoo_20200101_models.DescribePortAttackMaxFlowRequest,
     ) -> ddoscoo_20200101_models.DescribePortAttackMaxFlowResponse:
+        """
+        You can call this operation to query the peak bandwidth and peak packet rate of attack traffic on one or more Anti-DDoS Pro or Anti-DDoS Premium instances within a specific period of time.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribePortAttackMaxFlowRequest
+        @return: DescribePortAttackMaxFlowResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_port_attack_max_flow_with_options_async(request, runtime)
 
     def describe_port_auto_cc_status_with_options(
         self,
         request: ddoscoo_20200101_models.DescribePortAutoCcStatusRequest,
         runtime: util_models.RuntimeOptions,
@@ -7260,14 +8276,24 @@
         return await self.describe_port_view_source_countries_with_options_async(request, runtime)
 
     def describe_port_view_source_isps_with_options(
         self,
         request: ddoscoo_20200101_models.DescribePortViewSourceIspsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribePortViewSourceIspsResponse:
+        """
+        You can call the DescribePortViewSourceIsps operation to query the ISPs from which requests are sent to one or more Anti-DDoS Pro or Anti-DDoS Premium instances within a specific period of time.
+        > The data returned for this operation cannot reflect the actual traffic volume because Layer 4 identity authentication algorithms are updated for Anti-DDoS Pro and Anti-DDoS Premium. You can call this operation to calculate only the proportion of requests sent from different ISPs. If you want to query the request traffic volume, we recommend that you call the [DescribePortFlowList](~~157460~~) operation.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribePortViewSourceIspsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribePortViewSourceIspsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.end_time):
             query['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.instance_ids):
             query['InstanceIds'] = request.instance_ids
         if not UtilClient.is_unset(request.resource_group_id):
@@ -7294,14 +8320,24 @@
         )
 
     async def describe_port_view_source_isps_with_options_async(
         self,
         request: ddoscoo_20200101_models.DescribePortViewSourceIspsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribePortViewSourceIspsResponse:
+        """
+        You can call the DescribePortViewSourceIsps operation to query the ISPs from which requests are sent to one or more Anti-DDoS Pro or Anti-DDoS Premium instances within a specific period of time.
+        > The data returned for this operation cannot reflect the actual traffic volume because Layer 4 identity authentication algorithms are updated for Anti-DDoS Pro and Anti-DDoS Premium. You can call this operation to calculate only the proportion of requests sent from different ISPs. If you want to query the request traffic volume, we recommend that you call the [DescribePortFlowList](~~157460~~) operation.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribePortViewSourceIspsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribePortViewSourceIspsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.end_time):
             query['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.instance_ids):
             query['InstanceIds'] = request.instance_ids
         if not UtilClient.is_unset(request.resource_group_id):
@@ -7327,21 +8363,39 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_port_view_source_isps(
         self,
         request: ddoscoo_20200101_models.DescribePortViewSourceIspsRequest,
     ) -> ddoscoo_20200101_models.DescribePortViewSourceIspsResponse:
+        """
+        You can call the DescribePortViewSourceIsps operation to query the ISPs from which requests are sent to one or more Anti-DDoS Pro or Anti-DDoS Premium instances within a specific period of time.
+        > The data returned for this operation cannot reflect the actual traffic volume because Layer 4 identity authentication algorithms are updated for Anti-DDoS Pro and Anti-DDoS Premium. You can call this operation to calculate only the proportion of requests sent from different ISPs. If you want to query the request traffic volume, we recommend that you call the [DescribePortFlowList](~~157460~~) operation.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribePortViewSourceIspsRequest
+        @return: DescribePortViewSourceIspsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_port_view_source_isps_with_options(request, runtime)
 
     async def describe_port_view_source_isps_async(
         self,
         request: ddoscoo_20200101_models.DescribePortViewSourceIspsRequest,
     ) -> ddoscoo_20200101_models.DescribePortViewSourceIspsResponse:
+        """
+        You can call the DescribePortViewSourceIsps operation to query the ISPs from which requests are sent to one or more Anti-DDoS Pro or Anti-DDoS Premium instances within a specific period of time.
+        > The data returned for this operation cannot reflect the actual traffic volume because Layer 4 identity authentication algorithms are updated for Anti-DDoS Pro and Anti-DDoS Premium. You can call this operation to calculate only the proportion of requests sent from different ISPs. If you want to query the request traffic volume, we recommend that you call the [DescribePortFlowList](~~157460~~) operation.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribePortViewSourceIspsRequest
+        @return: DescribePortViewSourceIspsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_port_view_source_isps_with_options_async(request, runtime)
 
     def describe_port_view_source_provinces_with_options(
         self,
         request: ddoscoo_20200101_models.DescribePortViewSourceProvincesRequest,
         runtime: util_models.RuntimeOptions,
@@ -7424,14 +8478,24 @@
         return await self.describe_port_view_source_provinces_with_options_async(request, runtime)
 
     def describe_scene_defense_objects_with_options(
         self,
         request: ddoscoo_20200101_models.DescribeSceneDefenseObjectsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribeSceneDefenseObjectsResponse:
+        """
+        You can call the DescribeSceneDefenseObjects operation to query the protected objects of a scenario-specific custom policy.
+        Before you call this operation, make sure that you have created a scenario-specific custom policy by calling the [CreateSceneDefensePolicy](~~159779~~) operation.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeSceneDefenseObjectsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeSceneDefenseObjectsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.policy_id):
             query['PolicyId'] = request.policy_id
         if not UtilClient.is_unset(request.resource_group_id):
             query['ResourceGroupId'] = request.resource_group_id
         req = open_api_models.OpenApiRequest(
@@ -7454,14 +8518,24 @@
         )
 
     async def describe_scene_defense_objects_with_options_async(
         self,
         request: ddoscoo_20200101_models.DescribeSceneDefenseObjectsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribeSceneDefenseObjectsResponse:
+        """
+        You can call the DescribeSceneDefenseObjects operation to query the protected objects of a scenario-specific custom policy.
+        Before you call this operation, make sure that you have created a scenario-specific custom policy by calling the [CreateSceneDefensePolicy](~~159779~~) operation.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeSceneDefenseObjectsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeSceneDefenseObjectsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.policy_id):
             query['PolicyId'] = request.policy_id
         if not UtilClient.is_unset(request.resource_group_id):
             query['ResourceGroupId'] = request.resource_group_id
         req = open_api_models.OpenApiRequest(
@@ -7483,29 +8557,56 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_scene_defense_objects(
         self,
         request: ddoscoo_20200101_models.DescribeSceneDefenseObjectsRequest,
     ) -> ddoscoo_20200101_models.DescribeSceneDefenseObjectsResponse:
+        """
+        You can call the DescribeSceneDefenseObjects operation to query the protected objects of a scenario-specific custom policy.
+        Before you call this operation, make sure that you have created a scenario-specific custom policy by calling the [CreateSceneDefensePolicy](~~159779~~) operation.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeSceneDefenseObjectsRequest
+        @return: DescribeSceneDefenseObjectsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_scene_defense_objects_with_options(request, runtime)
 
     async def describe_scene_defense_objects_async(
         self,
         request: ddoscoo_20200101_models.DescribeSceneDefenseObjectsRequest,
     ) -> ddoscoo_20200101_models.DescribeSceneDefenseObjectsResponse:
+        """
+        You can call the DescribeSceneDefenseObjects operation to query the protected objects of a scenario-specific custom policy.
+        Before you call this operation, make sure that you have created a scenario-specific custom policy by calling the [CreateSceneDefensePolicy](~~159779~~) operation.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeSceneDefenseObjectsRequest
+        @return: DescribeSceneDefenseObjectsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_scene_defense_objects_with_options_async(request, runtime)
 
     def describe_scene_defense_policies_with_options(
         self,
         request: ddoscoo_20200101_models.DescribeSceneDefensePoliciesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribeSceneDefensePoliciesResponse:
+        """
+        You can call the DescribeSceneDefensePolicies operation to query the configurations of a scenario-specific custom policy that is created. For example, you can query the status, protected objects, and protection rules of the policy.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeSceneDefensePoliciesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeSceneDefensePoliciesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.resource_group_id):
             query['ResourceGroupId'] = request.resource_group_id
         if not UtilClient.is_unset(request.status):
             query['Status'] = request.status
         if not UtilClient.is_unset(request.template):
@@ -7530,14 +8631,23 @@
         )
 
     async def describe_scene_defense_policies_with_options_async(
         self,
         request: ddoscoo_20200101_models.DescribeSceneDefensePoliciesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribeSceneDefensePoliciesResponse:
+        """
+        You can call the DescribeSceneDefensePolicies operation to query the configurations of a scenario-specific custom policy that is created. For example, you can query the status, protected objects, and protection rules of the policy.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeSceneDefensePoliciesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeSceneDefensePoliciesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.resource_group_id):
             query['ResourceGroupId'] = request.resource_group_id
         if not UtilClient.is_unset(request.status):
             query['Status'] = request.status
         if not UtilClient.is_unset(request.template):
@@ -7561,21 +8671,37 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_scene_defense_policies(
         self,
         request: ddoscoo_20200101_models.DescribeSceneDefensePoliciesRequest,
     ) -> ddoscoo_20200101_models.DescribeSceneDefensePoliciesResponse:
+        """
+        You can call the DescribeSceneDefensePolicies operation to query the configurations of a scenario-specific custom policy that is created. For example, you can query the status, protected objects, and protection rules of the policy.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeSceneDefensePoliciesRequest
+        @return: DescribeSceneDefensePoliciesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_scene_defense_policies_with_options(request, runtime)
 
     async def describe_scene_defense_policies_async(
         self,
         request: ddoscoo_20200101_models.DescribeSceneDefensePoliciesRequest,
     ) -> ddoscoo_20200101_models.DescribeSceneDefensePoliciesResponse:
+        """
+        You can call the DescribeSceneDefensePolicies operation to query the configurations of a scenario-specific custom policy that is created. For example, you can query the status, protected objects, and protection rules of the policy.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeSceneDefensePoliciesRequest
+        @return: DescribeSceneDefensePoliciesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_scene_defense_policies_with_options_async(request, runtime)
 
     def describe_scheduler_rules_with_options(
         self,
         request: ddoscoo_20200101_models.DescribeSchedulerRulesRequest,
         runtime: util_models.RuntimeOptions,
@@ -7653,14 +8779,104 @@
     async def describe_scheduler_rules_async(
         self,
         request: ddoscoo_20200101_models.DescribeSchedulerRulesRequest,
     ) -> ddoscoo_20200101_models.DescribeSchedulerRulesResponse:
         runtime = util_models.RuntimeOptions()
         return await self.describe_scheduler_rules_with_options_async(request, runtime)
 
+    def describe_sla_event_list_with_options(
+        self,
+        request: ddoscoo_20200101_models.DescribeSlaEventListRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ddoscoo_20200101_models.DescribeSlaEventListResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.end_time):
+            query['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.ip):
+            query['Ip'] = request.ip
+        if not UtilClient.is_unset(request.page):
+            query['Page'] = request.page
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.region):
+            query['Region'] = request.region
+        if not UtilClient.is_unset(request.start_time):
+            query['StartTime'] = request.start_time
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeSlaEventList',
+            version='2020-01-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ddoscoo_20200101_models.DescribeSlaEventListResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def describe_sla_event_list_with_options_async(
+        self,
+        request: ddoscoo_20200101_models.DescribeSlaEventListRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ddoscoo_20200101_models.DescribeSlaEventListResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.end_time):
+            query['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.ip):
+            query['Ip'] = request.ip
+        if not UtilClient.is_unset(request.page):
+            query['Page'] = request.page
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.region):
+            query['Region'] = request.region
+        if not UtilClient.is_unset(request.start_time):
+            query['StartTime'] = request.start_time
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeSlaEventList',
+            version='2020-01-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ddoscoo_20200101_models.DescribeSlaEventListResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_sla_event_list(
+        self,
+        request: ddoscoo_20200101_models.DescribeSlaEventListRequest,
+    ) -> ddoscoo_20200101_models.DescribeSlaEventListResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_sla_event_list_with_options(request, runtime)
+
+    async def describe_sla_event_list_async(
+        self,
+        request: ddoscoo_20200101_models.DescribeSlaEventListRequest,
+    ) -> ddoscoo_20200101_models.DescribeSlaEventListResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_sla_event_list_with_options_async(request, runtime)
+
     def describe_sls_auth_status_with_options(
         self,
         request: ddoscoo_20200101_models.DescribeSlsAuthStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribeSlsAuthStatusResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -7868,14 +9084,23 @@
         return await self.describe_sls_open_status_with_options_async(request, runtime)
 
     def describe_sts_grant_status_with_options(
         self,
         request: ddoscoo_20200101_models.DescribeStsGrantStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribeStsGrantStatusResponse:
+        """
+        You can call the DescribeStsGrantStatus operation to query whether Anti-DDoS Pro or Anti-DDoS Premium of the current Alibaba Cloud account is authorized to access other cloud services.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeStsGrantStatusRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeStsGrantStatusResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.resource_group_id):
             query['ResourceGroupId'] = request.resource_group_id
         if not UtilClient.is_unset(request.role):
             query['Role'] = request.role
         req = open_api_models.OpenApiRequest(
@@ -7898,14 +9123,23 @@
         )
 
     async def describe_sts_grant_status_with_options_async(
         self,
         request: ddoscoo_20200101_models.DescribeStsGrantStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribeStsGrantStatusResponse:
+        """
+        You can call the DescribeStsGrantStatus operation to query whether Anti-DDoS Pro or Anti-DDoS Premium of the current Alibaba Cloud account is authorized to access other cloud services.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeStsGrantStatusRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeStsGrantStatusResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.resource_group_id):
             query['ResourceGroupId'] = request.resource_group_id
         if not UtilClient.is_unset(request.role):
             query['Role'] = request.role
         req = open_api_models.OpenApiRequest(
@@ -7927,29 +9161,55 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_sts_grant_status(
         self,
         request: ddoscoo_20200101_models.DescribeStsGrantStatusRequest,
     ) -> ddoscoo_20200101_models.DescribeStsGrantStatusResponse:
+        """
+        You can call the DescribeStsGrantStatus operation to query whether Anti-DDoS Pro or Anti-DDoS Premium of the current Alibaba Cloud account is authorized to access other cloud services.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeStsGrantStatusRequest
+        @return: DescribeStsGrantStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_sts_grant_status_with_options(request, runtime)
 
     async def describe_sts_grant_status_async(
         self,
         request: ddoscoo_20200101_models.DescribeStsGrantStatusRequest,
     ) -> ddoscoo_20200101_models.DescribeStsGrantStatusResponse:
+        """
+        You can call the DescribeStsGrantStatus operation to query whether Anti-DDoS Pro or Anti-DDoS Premium of the current Alibaba Cloud account is authorized to access other cloud services.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeStsGrantStatusRequest
+        @return: DescribeStsGrantStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_sts_grant_status_with_options_async(request, runtime)
 
     def describe_system_log_with_options(
         self,
         request: ddoscoo_20200101_models.DescribeSystemLogRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribeSystemLogResponse:
+        """
+        You can call the DescribeSystemLog operation to query the system logs of Anti-DDoS Pro or Anti-DDoS Premium. The system logs contain only billing logs for the burstable clean bandwidth.
+        If you have enabled the burstable clean bandwidth feature, you can call this operation to query the details of the bills of the burstable clean bandwidth.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeSystemLogRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeSystemLogResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.end_time):
             query['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.entity_object):
             query['EntityObject'] = request.entity_object
         if not UtilClient.is_unset(request.entity_type):
@@ -7980,14 +9240,24 @@
         )
 
     async def describe_system_log_with_options_async(
         self,
         request: ddoscoo_20200101_models.DescribeSystemLogRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribeSystemLogResponse:
+        """
+        You can call the DescribeSystemLog operation to query the system logs of Anti-DDoS Pro or Anti-DDoS Premium. The system logs contain only billing logs for the burstable clean bandwidth.
+        If you have enabled the burstable clean bandwidth feature, you can call this operation to query the details of the bills of the burstable clean bandwidth.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeSystemLogRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeSystemLogResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.end_time):
             query['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.entity_object):
             query['EntityObject'] = request.entity_object
         if not UtilClient.is_unset(request.entity_type):
@@ -8017,29 +9287,57 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_system_log(
         self,
         request: ddoscoo_20200101_models.DescribeSystemLogRequest,
     ) -> ddoscoo_20200101_models.DescribeSystemLogResponse:
+        """
+        You can call the DescribeSystemLog operation to query the system logs of Anti-DDoS Pro or Anti-DDoS Premium. The system logs contain only billing logs for the burstable clean bandwidth.
+        If you have enabled the burstable clean bandwidth feature, you can call this operation to query the details of the bills of the burstable clean bandwidth.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeSystemLogRequest
+        @return: DescribeSystemLogResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_system_log_with_options(request, runtime)
 
     async def describe_system_log_async(
         self,
         request: ddoscoo_20200101_models.DescribeSystemLogRequest,
     ) -> ddoscoo_20200101_models.DescribeSystemLogResponse:
+        """
+        You can call the DescribeSystemLog operation to query the system logs of Anti-DDoS Pro or Anti-DDoS Premium. The system logs contain only billing logs for the burstable clean bandwidth.
+        If you have enabled the burstable clean bandwidth feature, you can call this operation to query the details of the bills of the burstable clean bandwidth.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeSystemLogRequest
+        @return: DescribeSystemLogResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_system_log_with_options_async(request, runtime)
 
     def describe_tag_keys_with_options(
         self,
         request: ddoscoo_20200101_models.DescribeTagKeysRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribeTagKeysResponse:
+        """
+        You can call this operation to query all tag keys and the Anti-DDoS Pro instances to which the tag keys are added by page.
+        > The tag feature is suitable only for Anti-DDoS Pro.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeTagKeysRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeTagKeysResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.region_id):
@@ -8068,14 +9366,24 @@
         )
 
     async def describe_tag_keys_with_options_async(
         self,
         request: ddoscoo_20200101_models.DescribeTagKeysRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribeTagKeysResponse:
+        """
+        You can call this operation to query all tag keys and the Anti-DDoS Pro instances to which the tag keys are added by page.
+        > The tag feature is suitable only for Anti-DDoS Pro.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeTagKeysRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeTagKeysResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.region_id):
@@ -8103,29 +9411,57 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_tag_keys(
         self,
         request: ddoscoo_20200101_models.DescribeTagKeysRequest,
     ) -> ddoscoo_20200101_models.DescribeTagKeysResponse:
+        """
+        You can call this operation to query all tag keys and the Anti-DDoS Pro instances to which the tag keys are added by page.
+        > The tag feature is suitable only for Anti-DDoS Pro.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeTagKeysRequest
+        @return: DescribeTagKeysResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_tag_keys_with_options(request, runtime)
 
     async def describe_tag_keys_async(
         self,
         request: ddoscoo_20200101_models.DescribeTagKeysRequest,
     ) -> ddoscoo_20200101_models.DescribeTagKeysResponse:
+        """
+        You can call this operation to query all tag keys and the Anti-DDoS Pro instances to which the tag keys are added by page.
+        > The tag feature is suitable only for Anti-DDoS Pro.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeTagKeysRequest
+        @return: DescribeTagKeysResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_tag_keys_with_options_async(request, runtime)
 
     def describe_tag_resources_with_options(
         self,
         request: ddoscoo_20200101_models.DescribeTagResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribeTagResourcesResponse:
+        """
+        You can call the DescribeTagResources operation to query the information about the tags that are added to an Anti-DDoS Pro instance.
+        > Only Anti-DDoS Pro supports tags.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeTagResourcesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeTagResourcesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.next_token):
             query['NextToken'] = request.next_token
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_group_id):
@@ -8156,14 +9492,24 @@
         )
 
     async def describe_tag_resources_with_options_async(
         self,
         request: ddoscoo_20200101_models.DescribeTagResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribeTagResourcesResponse:
+        """
+        You can call the DescribeTagResources operation to query the information about the tags that are added to an Anti-DDoS Pro instance.
+        > Only Anti-DDoS Pro supports tags.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeTagResourcesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeTagResourcesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.next_token):
             query['NextToken'] = request.next_token
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_group_id):
@@ -8193,24 +9539,124 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_tag_resources(
         self,
         request: ddoscoo_20200101_models.DescribeTagResourcesRequest,
     ) -> ddoscoo_20200101_models.DescribeTagResourcesResponse:
+        """
+        You can call the DescribeTagResources operation to query the information about the tags that are added to an Anti-DDoS Pro instance.
+        > Only Anti-DDoS Pro supports tags.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeTagResourcesRequest
+        @return: DescribeTagResourcesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_tag_resources_with_options(request, runtime)
 
     async def describe_tag_resources_async(
         self,
         request: ddoscoo_20200101_models.DescribeTagResourcesRequest,
     ) -> ddoscoo_20200101_models.DescribeTagResourcesResponse:
+        """
+        You can call the DescribeTagResources operation to query the information about the tags that are added to an Anti-DDoS Pro instance.
+        > Only Anti-DDoS Pro supports tags.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeTagResourcesRequest
+        @return: DescribeTagResourcesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_tag_resources_with_options_async(request, runtime)
 
+    def describe_total_attack_max_flow_with_options(
+        self,
+        request: ddoscoo_20200101_models.DescribeTotalAttackMaxFlowRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ddoscoo_20200101_models.DescribeTotalAttackMaxFlowResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.end_time):
+            query['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.instance_ids):
+            query['InstanceIds'] = request.instance_ids
+        if not UtilClient.is_unset(request.resource_group_id):
+            query['ResourceGroupId'] = request.resource_group_id
+        if not UtilClient.is_unset(request.start_time):
+            query['StartTime'] = request.start_time
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeTotalAttackMaxFlow',
+            version='2020-01-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ddoscoo_20200101_models.DescribeTotalAttackMaxFlowResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def describe_total_attack_max_flow_with_options_async(
+        self,
+        request: ddoscoo_20200101_models.DescribeTotalAttackMaxFlowRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ddoscoo_20200101_models.DescribeTotalAttackMaxFlowResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.end_time):
+            query['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.instance_ids):
+            query['InstanceIds'] = request.instance_ids
+        if not UtilClient.is_unset(request.resource_group_id):
+            query['ResourceGroupId'] = request.resource_group_id
+        if not UtilClient.is_unset(request.start_time):
+            query['StartTime'] = request.start_time
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeTotalAttackMaxFlow',
+            version='2020-01-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ddoscoo_20200101_models.DescribeTotalAttackMaxFlowResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_total_attack_max_flow(
+        self,
+        request: ddoscoo_20200101_models.DescribeTotalAttackMaxFlowRequest,
+    ) -> ddoscoo_20200101_models.DescribeTotalAttackMaxFlowResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_total_attack_max_flow_with_options(request, runtime)
+
+    async def describe_total_attack_max_flow_async(
+        self,
+        request: ddoscoo_20200101_models.DescribeTotalAttackMaxFlowRequest,
+    ) -> ddoscoo_20200101_models.DescribeTotalAttackMaxFlowResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_total_attack_max_flow_with_options_async(request, runtime)
+
     def describe_udp_reflect_with_options(
         self,
         request: ddoscoo_20200101_models.DescribeUdpReflectRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribeUdpReflectResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -8352,14 +9798,21 @@
         return await self.describe_un_blackhole_count_with_options_async(request, runtime)
 
     def describe_un_block_count_with_options(
         self,
         request: ddoscoo_20200101_models.DescribeUnBlockCountRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribeUnBlockCountResponse:
+        """
+        > This operation is suitable only for Anti-DDoS Pro.
+        
+        @param request: DescribeUnBlockCountRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeUnBlockCountResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.resource_group_id):
             query['ResourceGroupId'] = request.resource_group_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -8380,14 +9833,21 @@
         )
 
     async def describe_un_block_count_with_options_async(
         self,
         request: ddoscoo_20200101_models.DescribeUnBlockCountRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribeUnBlockCountResponse:
+        """
+        > This operation is suitable only for Anti-DDoS Pro.
+        
+        @param request: DescribeUnBlockCountRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeUnBlockCountResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.resource_group_id):
             query['ResourceGroupId'] = request.resource_group_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -8407,29 +9867,50 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_un_block_count(
         self,
         request: ddoscoo_20200101_models.DescribeUnBlockCountRequest,
     ) -> ddoscoo_20200101_models.DescribeUnBlockCountResponse:
+        """
+        > This operation is suitable only for Anti-DDoS Pro.
+        
+        @param request: DescribeUnBlockCountRequest
+        @return: DescribeUnBlockCountResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_un_block_count_with_options(request, runtime)
 
     async def describe_un_block_count_async(
         self,
         request: ddoscoo_20200101_models.DescribeUnBlockCountRequest,
     ) -> ddoscoo_20200101_models.DescribeUnBlockCountResponse:
+        """
+        > This operation is suitable only for Anti-DDoS Pro.
+        
+        @param request: DescribeUnBlockCountRequest
+        @return: DescribeUnBlockCountResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_un_block_count_with_options_async(request, runtime)
 
     def describe_web_access_log_dispatch_status_with_options(
         self,
         request: ddoscoo_20200101_models.DescribeWebAccessLogDispatchStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribeWebAccessLogDispatchStatusResponse:
+        """
+        You can call the DescribeWebAccessLogDispatchStatus operation to check whether the log analysis feature is enabled for all domain names that are added to your Anti-DDoS Pro or Anti-DDoS Premium instance.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeWebAccessLogDispatchStatusRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeWebAccessLogDispatchStatusResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.resource_group_id):
@@ -8454,14 +9935,23 @@
         )
 
     async def describe_web_access_log_dispatch_status_with_options_async(
         self,
         request: ddoscoo_20200101_models.DescribeWebAccessLogDispatchStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribeWebAccessLogDispatchStatusResponse:
+        """
+        You can call the DescribeWebAccessLogDispatchStatus operation to check whether the log analysis feature is enabled for all domain names that are added to your Anti-DDoS Pro or Anti-DDoS Premium instance.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeWebAccessLogDispatchStatusRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeWebAccessLogDispatchStatusResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             query['PageSize'] = request.page_size
         if not UtilClient.is_unset(request.resource_group_id):
@@ -8485,21 +9975,37 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_web_access_log_dispatch_status(
         self,
         request: ddoscoo_20200101_models.DescribeWebAccessLogDispatchStatusRequest,
     ) -> ddoscoo_20200101_models.DescribeWebAccessLogDispatchStatusResponse:
+        """
+        You can call the DescribeWebAccessLogDispatchStatus operation to check whether the log analysis feature is enabled for all domain names that are added to your Anti-DDoS Pro or Anti-DDoS Premium instance.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeWebAccessLogDispatchStatusRequest
+        @return: DescribeWebAccessLogDispatchStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_web_access_log_dispatch_status_with_options(request, runtime)
 
     async def describe_web_access_log_dispatch_status_async(
         self,
         request: ddoscoo_20200101_models.DescribeWebAccessLogDispatchStatusRequest,
     ) -> ddoscoo_20200101_models.DescribeWebAccessLogDispatchStatusResponse:
+        """
+        You can call the DescribeWebAccessLogDispatchStatus operation to check whether the log analysis feature is enabled for all domain names that are added to your Anti-DDoS Pro or Anti-DDoS Premium instance.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeWebAccessLogDispatchStatusRequest
+        @return: DescribeWebAccessLogDispatchStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_web_access_log_dispatch_status_with_options_async(request, runtime)
 
     def describe_web_access_log_empty_count_with_options(
         self,
         request: ddoscoo_20200101_models.DescribeWebAccessLogEmptyCountRequest,
         runtime: util_models.RuntimeOptions,
@@ -8870,14 +10376,23 @@
         return await self.describe_web_ccrules_with_options_async(request, runtime)
 
     def describe_web_cache_configs_with_options(
         self,
         request: ddoscoo_20200101_models.DescribeWebCacheConfigsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribeWebCacheConfigsResponse:
+        """
+        You can call the DescribeWebCacheConfigs operation to query the Static Page Caching configurations of websites. The configurations include cache modes and custom caching rules.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeWebCacheConfigsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeWebCacheConfigsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.domains):
             query['Domains'] = request.domains
         if not UtilClient.is_unset(request.resource_group_id):
             query['ResourceGroupId'] = request.resource_group_id
         req = open_api_models.OpenApiRequest(
@@ -8900,14 +10415,23 @@
         )
 
     async def describe_web_cache_configs_with_options_async(
         self,
         request: ddoscoo_20200101_models.DescribeWebCacheConfigsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.DescribeWebCacheConfigsResponse:
+        """
+        You can call the DescribeWebCacheConfigs operation to query the Static Page Caching configurations of websites. The configurations include cache modes and custom caching rules.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeWebCacheConfigsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeWebCacheConfigsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.domains):
             query['Domains'] = request.domains
         if not UtilClient.is_unset(request.resource_group_id):
             query['ResourceGroupId'] = request.resource_group_id
         req = open_api_models.OpenApiRequest(
@@ -8929,21 +10453,37 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_web_cache_configs(
         self,
         request: ddoscoo_20200101_models.DescribeWebCacheConfigsRequest,
     ) -> ddoscoo_20200101_models.DescribeWebCacheConfigsResponse:
+        """
+        You can call the DescribeWebCacheConfigs operation to query the Static Page Caching configurations of websites. The configurations include cache modes and custom caching rules.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeWebCacheConfigsRequest
+        @return: DescribeWebCacheConfigsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_web_cache_configs_with_options(request, runtime)
 
     async def describe_web_cache_configs_async(
         self,
         request: ddoscoo_20200101_models.DescribeWebCacheConfigsRequest,
     ) -> ddoscoo_20200101_models.DescribeWebCacheConfigsResponse:
+        """
+        You can call the DescribeWebCacheConfigs operation to query the Static Page Caching configurations of websites. The configurations include cache modes and custom caching rules.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: DescribeWebCacheConfigsRequest
+        @return: DescribeWebCacheConfigsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_web_cache_configs_with_options_async(request, runtime)
 
     def describe_web_cc_protect_switch_with_options(
         self,
         request: ddoscoo_20200101_models.DescribeWebCcProtectSwitchRequest,
         runtime: util_models.RuntimeOptions,
@@ -10197,14 +11737,114 @@
     async def enable_web_ccrule_async(
         self,
         request: ddoscoo_20200101_models.EnableWebCCRuleRequest,
     ) -> ddoscoo_20200101_models.EnableWebCCRuleResponse:
         runtime = util_models.RuntimeOptions()
         return await self.enable_web_ccrule_with_options_async(request, runtime)
 
+    def modify_biz_band_width_mode_with_options(
+        self,
+        request: ddoscoo_20200101_models.ModifyBizBandWidthModeRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ddoscoo_20200101_models.ModifyBizBandWidthModeResponse:
+        """
+        You can switch between the metering methods of the burstable clean bandwidth feature. The new metering method takes effect from 00:00 on the first day of the next month. You can change the metering method up to three times each calendar month. The most recent metering method that you select takes effect in the next month. You cannot change the metering method on the last day of each calendar month.
+        
+        @param request: ModifyBizBandWidthModeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyBizBandWidthModeResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.mode):
+            query['Mode'] = request.mode
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ModifyBizBandWidthMode',
+            version='2020-01-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ddoscoo_20200101_models.ModifyBizBandWidthModeResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def modify_biz_band_width_mode_with_options_async(
+        self,
+        request: ddoscoo_20200101_models.ModifyBizBandWidthModeRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ddoscoo_20200101_models.ModifyBizBandWidthModeResponse:
+        """
+        You can switch between the metering methods of the burstable clean bandwidth feature. The new metering method takes effect from 00:00 on the first day of the next month. You can change the metering method up to three times each calendar month. The most recent metering method that you select takes effect in the next month. You cannot change the metering method on the last day of each calendar month.
+        
+        @param request: ModifyBizBandWidthModeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyBizBandWidthModeResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.mode):
+            query['Mode'] = request.mode
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ModifyBizBandWidthMode',
+            version='2020-01-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ddoscoo_20200101_models.ModifyBizBandWidthModeResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def modify_biz_band_width_mode(
+        self,
+        request: ddoscoo_20200101_models.ModifyBizBandWidthModeRequest,
+    ) -> ddoscoo_20200101_models.ModifyBizBandWidthModeResponse:
+        """
+        You can switch between the metering methods of the burstable clean bandwidth feature. The new metering method takes effect from 00:00 on the first day of the next month. You can change the metering method up to three times each calendar month. The most recent metering method that you select takes effect in the next month. You cannot change the metering method on the last day of each calendar month.
+        
+        @param request: ModifyBizBandWidthModeRequest
+        @return: ModifyBizBandWidthModeResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return self.modify_biz_band_width_mode_with_options(request, runtime)
+
+    async def modify_biz_band_width_mode_async(
+        self,
+        request: ddoscoo_20200101_models.ModifyBizBandWidthModeRequest,
+    ) -> ddoscoo_20200101_models.ModifyBizBandWidthModeResponse:
+        """
+        You can switch between the metering methods of the burstable clean bandwidth feature. The new metering method takes effect from 00:00 on the first day of the next month. You can change the metering method up to three times each calendar month. The most recent metering method that you select takes effect in the next month. You cannot change the metering method on the last day of each calendar month.
+        
+        @param request: ModifyBizBandWidthModeRequest
+        @return: ModifyBizBandWidthModeResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return await self.modify_biz_band_width_mode_with_options_async(request, runtime)
+
     def modify_blackhole_status_with_options(
         self,
         request: ddoscoo_20200101_models.ModifyBlackholeStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.ModifyBlackholeStatusResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -10276,14 +11916,21 @@
         return await self.modify_blackhole_status_with_options_async(request, runtime)
 
     def modify_block_status_with_options(
         self,
         request: ddoscoo_20200101_models.ModifyBlockStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.ModifyBlockStatusResponse:
+        """
+        > This operation is suitable only for Anti-DDoS Pro.
+        
+        @param request: ModifyBlockStatusRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyBlockStatusResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.duration):
             query['Duration'] = request.duration
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.lines):
@@ -10310,14 +11957,21 @@
         )
 
     async def modify_block_status_with_options_async(
         self,
         request: ddoscoo_20200101_models.ModifyBlockStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.ModifyBlockStatusResponse:
+        """
+        > This operation is suitable only for Anti-DDoS Pro.
+        
+        @param request: ModifyBlockStatusRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyBlockStatusResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.duration):
             query['Duration'] = request.duration
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.lines):
@@ -10343,29 +11997,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_block_status(
         self,
         request: ddoscoo_20200101_models.ModifyBlockStatusRequest,
     ) -> ddoscoo_20200101_models.ModifyBlockStatusResponse:
+        """
+        > This operation is suitable only for Anti-DDoS Pro.
+        
+        @param request: ModifyBlockStatusRequest
+        @return: ModifyBlockStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_block_status_with_options(request, runtime)
 
     async def modify_block_status_async(
         self,
         request: ddoscoo_20200101_models.ModifyBlockStatusRequest,
     ) -> ddoscoo_20200101_models.ModifyBlockStatusResponse:
+        """
+        > This operation is suitable only for Anti-DDoS Pro.
+        
+        @param request: ModifyBlockStatusRequest
+        @return: ModifyBlockStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_block_status_with_options_async(request, runtime)
 
     def modify_cname_reuse_with_options(
         self,
         request: ddoscoo_20200101_models.ModifyCnameReuseRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.ModifyCnameReuseResponse:
+        """
+        > This operation is suitable only for Anti-DDoS Premium.
+        
+        @param request: ModifyCnameReuseRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyCnameReuseResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.cname):
             query['Cname'] = request.cname
         if not UtilClient.is_unset(request.domain):
             query['Domain'] = request.domain
         if not UtilClient.is_unset(request.enable):
@@ -10392,14 +12065,21 @@
         )
 
     async def modify_cname_reuse_with_options_async(
         self,
         request: ddoscoo_20200101_models.ModifyCnameReuseRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.ModifyCnameReuseResponse:
+        """
+        > This operation is suitable only for Anti-DDoS Premium.
+        
+        @param request: ModifyCnameReuseRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyCnameReuseResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.cname):
             query['Cname'] = request.cname
         if not UtilClient.is_unset(request.domain):
             query['Domain'] = request.domain
         if not UtilClient.is_unset(request.enable):
@@ -10425,21 +12105,33 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_cname_reuse(
         self,
         request: ddoscoo_20200101_models.ModifyCnameReuseRequest,
     ) -> ddoscoo_20200101_models.ModifyCnameReuseResponse:
+        """
+        > This operation is suitable only for Anti-DDoS Premium.
+        
+        @param request: ModifyCnameReuseRequest
+        @return: ModifyCnameReuseResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_cname_reuse_with_options(request, runtime)
 
     async def modify_cname_reuse_async(
         self,
         request: ddoscoo_20200101_models.ModifyCnameReuseRequest,
     ) -> ddoscoo_20200101_models.ModifyCnameReuseResponse:
+        """
+        > This operation is suitable only for Anti-DDoS Premium.
+        
+        @param request: ModifyCnameReuseRequest
+        @return: ModifyCnameReuseResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_cname_reuse_with_options_async(request, runtime)
 
     def modify_domain_resource_with_options(
         self,
         request: ddoscoo_20200101_models.ModifyDomainResourceRequest,
         runtime: util_models.RuntimeOptions,
@@ -10530,14 +12222,21 @@
         return await self.modify_domain_resource_with_options_async(request, runtime)
 
     def modify_elastic_band_width_with_options(
         self,
         request: ddoscoo_20200101_models.ModifyElasticBandWidthRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.ModifyElasticBandWidthResponse:
+        """
+        > This operation is suitable only for Anti-DDoS Pro.
+        
+        @param request: ModifyElasticBandWidthRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyElasticBandWidthResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.elastic_bandwidth):
             query['ElasticBandwidth'] = request.elastic_bandwidth
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         req = open_api_models.OpenApiRequest(
@@ -10560,14 +12259,21 @@
         )
 
     async def modify_elastic_band_width_with_options_async(
         self,
         request: ddoscoo_20200101_models.ModifyElasticBandWidthRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.ModifyElasticBandWidthResponse:
+        """
+        > This operation is suitable only for Anti-DDoS Pro.
+        
+        @param request: ModifyElasticBandWidthRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyElasticBandWidthResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.elastic_bandwidth):
             query['ElasticBandwidth'] = request.elastic_bandwidth
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         req = open_api_models.OpenApiRequest(
@@ -10589,24 +12295,140 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_elastic_band_width(
         self,
         request: ddoscoo_20200101_models.ModifyElasticBandWidthRequest,
     ) -> ddoscoo_20200101_models.ModifyElasticBandWidthResponse:
+        """
+        > This operation is suitable only for Anti-DDoS Pro.
+        
+        @param request: ModifyElasticBandWidthRequest
+        @return: ModifyElasticBandWidthResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_elastic_band_width_with_options(request, runtime)
 
     async def modify_elastic_band_width_async(
         self,
         request: ddoscoo_20200101_models.ModifyElasticBandWidthRequest,
     ) -> ddoscoo_20200101_models.ModifyElasticBandWidthResponse:
+        """
+        > This operation is suitable only for Anti-DDoS Pro.
+        
+        @param request: ModifyElasticBandWidthRequest
+        @return: ModifyElasticBandWidthResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_elastic_band_width_with_options_async(request, runtime)
 
+    def modify_elastic_biz_band_width_with_options(
+        self,
+        request: ddoscoo_20200101_models.ModifyElasticBizBandWidthRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ddoscoo_20200101_models.ModifyElasticBizBandWidthResponse:
+        """
+        Before you call this operation, make sure that you have fully understood the billing method and [pricing](https://help.aliyun.com/document_detail/283754.html) of the burstable clean bandwidth feature. After you call this operation for the first time, the modification immediately takes effect.
+        
+        @param request: ModifyElasticBizBandWidthRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyElasticBizBandWidthResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.elastic_biz_bandwidth):
+            query['ElasticBizBandwidth'] = request.elastic_biz_bandwidth
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.mode):
+            query['Mode'] = request.mode
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ModifyElasticBizBandWidth',
+            version='2020-01-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ddoscoo_20200101_models.ModifyElasticBizBandWidthResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def modify_elastic_biz_band_width_with_options_async(
+        self,
+        request: ddoscoo_20200101_models.ModifyElasticBizBandWidthRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ddoscoo_20200101_models.ModifyElasticBizBandWidthResponse:
+        """
+        Before you call this operation, make sure that you have fully understood the billing method and [pricing](https://help.aliyun.com/document_detail/283754.html) of the burstable clean bandwidth feature. After you call this operation for the first time, the modification immediately takes effect.
+        
+        @param request: ModifyElasticBizBandWidthRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyElasticBizBandWidthResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.elastic_biz_bandwidth):
+            query['ElasticBizBandwidth'] = request.elastic_biz_bandwidth
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.mode):
+            query['Mode'] = request.mode
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ModifyElasticBizBandWidth',
+            version='2020-01-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ddoscoo_20200101_models.ModifyElasticBizBandWidthResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def modify_elastic_biz_band_width(
+        self,
+        request: ddoscoo_20200101_models.ModifyElasticBizBandWidthRequest,
+    ) -> ddoscoo_20200101_models.ModifyElasticBizBandWidthResponse:
+        """
+        Before you call this operation, make sure that you have fully understood the billing method and [pricing](https://help.aliyun.com/document_detail/283754.html) of the burstable clean bandwidth feature. After you call this operation for the first time, the modification immediately takes effect.
+        
+        @param request: ModifyElasticBizBandWidthRequest
+        @return: ModifyElasticBizBandWidthResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return self.modify_elastic_biz_band_width_with_options(request, runtime)
+
+    async def modify_elastic_biz_band_width_async(
+        self,
+        request: ddoscoo_20200101_models.ModifyElasticBizBandWidthRequest,
+    ) -> ddoscoo_20200101_models.ModifyElasticBizBandWidthResponse:
+        """
+        Before you call this operation, make sure that you have fully understood the billing method and [pricing](https://help.aliyun.com/document_detail/283754.html) of the burstable clean bandwidth feature. After you call this operation for the first time, the modification immediately takes effect.
+        
+        @param request: ModifyElasticBizBandWidthRequest
+        @return: ModifyElasticBizBandWidthResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return await self.modify_elastic_biz_band_width_with_options_async(request, runtime)
+
     def modify_full_log_ttl_with_options(
         self,
         request: ddoscoo_20200101_models.ModifyFullLogTtlRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.ModifyFullLogTtlResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -10673,14 +12495,92 @@
     async def modify_full_log_ttl_async(
         self,
         request: ddoscoo_20200101_models.ModifyFullLogTtlRequest,
     ) -> ddoscoo_20200101_models.ModifyFullLogTtlResponse:
         runtime = util_models.RuntimeOptions()
         return await self.modify_full_log_ttl_with_options_async(request, runtime)
 
+    def modify_headers_with_options(
+        self,
+        request: ddoscoo_20200101_models.ModifyHeadersRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ddoscoo_20200101_models.ModifyHeadersResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.custom_headers):
+            query['CustomHeaders'] = request.custom_headers
+        if not UtilClient.is_unset(request.domain):
+            query['Domain'] = request.domain
+        if not UtilClient.is_unset(request.resource_group_id):
+            query['ResourceGroupId'] = request.resource_group_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ModifyHeaders',
+            version='2020-01-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ddoscoo_20200101_models.ModifyHeadersResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def modify_headers_with_options_async(
+        self,
+        request: ddoscoo_20200101_models.ModifyHeadersRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ddoscoo_20200101_models.ModifyHeadersResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.custom_headers):
+            query['CustomHeaders'] = request.custom_headers
+        if not UtilClient.is_unset(request.domain):
+            query['Domain'] = request.domain
+        if not UtilClient.is_unset(request.resource_group_id):
+            query['ResourceGroupId'] = request.resource_group_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ModifyHeaders',
+            version='2020-01-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ddoscoo_20200101_models.ModifyHeadersResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def modify_headers(
+        self,
+        request: ddoscoo_20200101_models.ModifyHeadersRequest,
+    ) -> ddoscoo_20200101_models.ModifyHeadersResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.modify_headers_with_options(request, runtime)
+
+    async def modify_headers_async(
+        self,
+        request: ddoscoo_20200101_models.ModifyHeadersRequest,
+    ) -> ddoscoo_20200101_models.ModifyHeadersResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.modify_headers_with_options_async(request, runtime)
+
     def modify_health_check_config_with_options(
         self,
         request: ddoscoo_20200101_models.ModifyHealthCheckConfigRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.ModifyHealthCheckConfigResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -10760,14 +12660,21 @@
         return await self.modify_health_check_config_with_options_async(request, runtime)
 
     def modify_http_2enable_with_options(
         self,
         request: ddoscoo_20200101_models.ModifyHttp2EnableRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.ModifyHttp2EnableResponse:
+        """
+        > This operation is suitable only for Anti-DDoS Pro.
+        
+        @param request: ModifyHttp2EnableRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyHttp2EnableResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.domain):
             query['Domain'] = request.domain
         if not UtilClient.is_unset(request.enable):
             query['Enable'] = request.enable
         if not UtilClient.is_unset(request.resource_group_id):
@@ -10792,14 +12699,21 @@
         )
 
     async def modify_http_2enable_with_options_async(
         self,
         request: ddoscoo_20200101_models.ModifyHttp2EnableRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.ModifyHttp2EnableResponse:
+        """
+        > This operation is suitable only for Anti-DDoS Pro.
+        
+        @param request: ModifyHttp2EnableRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyHttp2EnableResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.domain):
             query['Domain'] = request.domain
         if not UtilClient.is_unset(request.enable):
             query['Enable'] = request.enable
         if not UtilClient.is_unset(request.resource_group_id):
@@ -10823,21 +12737,33 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_http_2enable(
         self,
         request: ddoscoo_20200101_models.ModifyHttp2EnableRequest,
     ) -> ddoscoo_20200101_models.ModifyHttp2EnableResponse:
+        """
+        > This operation is suitable only for Anti-DDoS Pro.
+        
+        @param request: ModifyHttp2EnableRequest
+        @return: ModifyHttp2EnableResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_http_2enable_with_options(request, runtime)
 
     async def modify_http_2enable_async(
         self,
         request: ddoscoo_20200101_models.ModifyHttp2EnableRequest,
     ) -> ddoscoo_20200101_models.ModifyHttp2EnableResponse:
+        """
+        > This operation is suitable only for Anti-DDoS Pro.
+        
+        @param request: ModifyHttp2EnableRequest
+        @return: ModifyHttp2EnableResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_http_2enable_with_options_async(request, runtime)
 
     def modify_instance_remark_with_options(
         self,
         request: ddoscoo_20200101_models.ModifyInstanceRemarkRequest,
         runtime: util_models.RuntimeOptions,
@@ -10989,19 +12915,126 @@
     async def modify_network_rule_attribute_async(
         self,
         request: ddoscoo_20200101_models.ModifyNetworkRuleAttributeRequest,
     ) -> ddoscoo_20200101_models.ModifyNetworkRuleAttributeResponse:
         runtime = util_models.RuntimeOptions()
         return await self.modify_network_rule_attribute_with_options_async(request, runtime)
 
+    def modify_ocsp_status_with_options(
+        self,
+        request: ddoscoo_20200101_models.ModifyOcspStatusRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ddoscoo_20200101_models.ModifyOcspStatusResponse:
+        """
+        This feature is available only for a website that supports HTTPS. If HTTPS is selected for Protocol, we recommend that you enable this feature.
+        
+        @param request: ModifyOcspStatusRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyOcspStatusResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.domain):
+            query['Domain'] = request.domain
+        if not UtilClient.is_unset(request.enable):
+            query['Enable'] = request.enable
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ModifyOcspStatus',
+            version='2020-01-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ddoscoo_20200101_models.ModifyOcspStatusResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def modify_ocsp_status_with_options_async(
+        self,
+        request: ddoscoo_20200101_models.ModifyOcspStatusRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ddoscoo_20200101_models.ModifyOcspStatusResponse:
+        """
+        This feature is available only for a website that supports HTTPS. If HTTPS is selected for Protocol, we recommend that you enable this feature.
+        
+        @param request: ModifyOcspStatusRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyOcspStatusResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.domain):
+            query['Domain'] = request.domain
+        if not UtilClient.is_unset(request.enable):
+            query['Enable'] = request.enable
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ModifyOcspStatus',
+            version='2020-01-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ddoscoo_20200101_models.ModifyOcspStatusResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def modify_ocsp_status(
+        self,
+        request: ddoscoo_20200101_models.ModifyOcspStatusRequest,
+    ) -> ddoscoo_20200101_models.ModifyOcspStatusResponse:
+        """
+        This feature is available only for a website that supports HTTPS. If HTTPS is selected for Protocol, we recommend that you enable this feature.
+        
+        @param request: ModifyOcspStatusRequest
+        @return: ModifyOcspStatusResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return self.modify_ocsp_status_with_options(request, runtime)
+
+    async def modify_ocsp_status_async(
+        self,
+        request: ddoscoo_20200101_models.ModifyOcspStatusRequest,
+    ) -> ddoscoo_20200101_models.ModifyOcspStatusResponse:
+        """
+        This feature is available only for a website that supports HTTPS. If HTTPS is selected for Protocol, we recommend that you enable this feature.
+        
+        @param request: ModifyOcspStatusRequest
+        @return: ModifyOcspStatusResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return await self.modify_ocsp_status_with_options_async(request, runtime)
+
     def modify_port_with_options(
         self,
         request: ddoscoo_20200101_models.ModifyPortRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.ModifyPortResponse:
+        """
+        You can call the ModifyPort operation by using Terraform. For more information about Terraform, see [What is Terraform?](~~95820~~).
+        
+        @param request: ModifyPortRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyPortResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.backend_port):
             query['BackendPort'] = request.backend_port
         if not UtilClient.is_unset(request.frontend_port):
             query['FrontendPort'] = request.frontend_port
         if not UtilClient.is_unset(request.frontend_protocol):
@@ -11030,14 +13063,21 @@
         )
 
     async def modify_port_with_options_async(
         self,
         request: ddoscoo_20200101_models.ModifyPortRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.ModifyPortResponse:
+        """
+        You can call the ModifyPort operation by using Terraform. For more information about Terraform, see [What is Terraform?](~~95820~~).
+        
+        @param request: ModifyPortRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyPortResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.backend_port):
             query['BackendPort'] = request.backend_port
         if not UtilClient.is_unset(request.frontend_port):
             query['FrontendPort'] = request.frontend_port
         if not UtilClient.is_unset(request.frontend_protocol):
@@ -11065,21 +13105,33 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_port(
         self,
         request: ddoscoo_20200101_models.ModifyPortRequest,
     ) -> ddoscoo_20200101_models.ModifyPortResponse:
+        """
+        You can call the ModifyPort operation by using Terraform. For more information about Terraform, see [What is Terraform?](~~95820~~).
+        
+        @param request: ModifyPortRequest
+        @return: ModifyPortResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_port_with_options(request, runtime)
 
     async def modify_port_async(
         self,
         request: ddoscoo_20200101_models.ModifyPortRequest,
     ) -> ddoscoo_20200101_models.ModifyPortResponse:
+        """
+        You can call the ModifyPort operation by using Terraform. For more information about Terraform, see [What is Terraform?](~~95820~~).
+        
+        @param request: ModifyPortRequest
+        @return: ModifyPortResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_port_with_options_async(request, runtime)
 
     def modify_port_auto_cc_status_with_options(
         self,
         request: ddoscoo_20200101_models.ModifyPortAutoCcStatusRequest,
         runtime: util_models.RuntimeOptions,
@@ -11716,14 +13768,23 @@
         return await self.modify_web_area_block_with_options_async(request, runtime)
 
     def modify_web_area_block_switch_with_options(
         self,
         request: ddoscoo_20200101_models.ModifyWebAreaBlockSwitchRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.ModifyWebAreaBlockSwitchResponse:
+        """
+        You can call the ModifyWebAreaBlockSwitch operation to enable or disable the Location Blacklist (Domain Names) policy for a domain name.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: ModifyWebAreaBlockSwitchRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyWebAreaBlockSwitchResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.config):
             query['Config'] = request.config
         if not UtilClient.is_unset(request.domain):
             query['Domain'] = request.domain
         if not UtilClient.is_unset(request.resource_group_id):
@@ -11748,14 +13809,23 @@
         )
 
     async def modify_web_area_block_switch_with_options_async(
         self,
         request: ddoscoo_20200101_models.ModifyWebAreaBlockSwitchRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.ModifyWebAreaBlockSwitchResponse:
+        """
+        You can call the ModifyWebAreaBlockSwitch operation to enable or disable the Location Blacklist (Domain Names) policy for a domain name.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: ModifyWebAreaBlockSwitchRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyWebAreaBlockSwitchResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.config):
             query['Config'] = request.config
         if not UtilClient.is_unset(request.domain):
             query['Domain'] = request.domain
         if not UtilClient.is_unset(request.resource_group_id):
@@ -11779,21 +13849,37 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_web_area_block_switch(
         self,
         request: ddoscoo_20200101_models.ModifyWebAreaBlockSwitchRequest,
     ) -> ddoscoo_20200101_models.ModifyWebAreaBlockSwitchResponse:
+        """
+        You can call the ModifyWebAreaBlockSwitch operation to enable or disable the Location Blacklist (Domain Names) policy for a domain name.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: ModifyWebAreaBlockSwitchRequest
+        @return: ModifyWebAreaBlockSwitchResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_web_area_block_switch_with_options(request, runtime)
 
     async def modify_web_area_block_switch_async(
         self,
         request: ddoscoo_20200101_models.ModifyWebAreaBlockSwitchRequest,
     ) -> ddoscoo_20200101_models.ModifyWebAreaBlockSwitchResponse:
+        """
+        You can call the ModifyWebAreaBlockSwitch operation to enable or disable the Location Blacklist (Domain Names) policy for a domain name.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: ModifyWebAreaBlockSwitchRequest
+        @return: ModifyWebAreaBlockSwitchResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_web_area_block_switch_with_options_async(request, runtime)
 
     def modify_web_ccrule_with_options(
         self,
         request: ddoscoo_20200101_models.ModifyWebCCRuleRequest,
         runtime: util_models.RuntimeOptions,
@@ -12052,14 +14138,23 @@
         return await self.modify_web_cache_mode_with_options_async(request, runtime)
 
     def modify_web_cache_switch_with_options(
         self,
         request: ddoscoo_20200101_models.ModifyWebCacheSwitchRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.ModifyWebCacheSwitchResponse:
+        """
+        You can call the ModifyWebCacheSwitch operation to enable or disable the Static Page Caching policy for a website.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: ModifyWebCacheSwitchRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyWebCacheSwitchResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.domain):
             query['Domain'] = request.domain
         if not UtilClient.is_unset(request.enable):
             query['Enable'] = request.enable
         if not UtilClient.is_unset(request.resource_group_id):
@@ -12084,14 +14179,23 @@
         )
 
     async def modify_web_cache_switch_with_options_async(
         self,
         request: ddoscoo_20200101_models.ModifyWebCacheSwitchRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.ModifyWebCacheSwitchResponse:
+        """
+        You can call the ModifyWebCacheSwitch operation to enable or disable the Static Page Caching policy for a website.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: ModifyWebCacheSwitchRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyWebCacheSwitchResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.domain):
             query['Domain'] = request.domain
         if not UtilClient.is_unset(request.enable):
             query['Enable'] = request.enable
         if not UtilClient.is_unset(request.resource_group_id):
@@ -12115,21 +14219,37 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_web_cache_switch(
         self,
         request: ddoscoo_20200101_models.ModifyWebCacheSwitchRequest,
     ) -> ddoscoo_20200101_models.ModifyWebCacheSwitchResponse:
+        """
+        You can call the ModifyWebCacheSwitch operation to enable or disable the Static Page Caching policy for a website.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: ModifyWebCacheSwitchRequest
+        @return: ModifyWebCacheSwitchResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_web_cache_switch_with_options(request, runtime)
 
     async def modify_web_cache_switch_async(
         self,
         request: ddoscoo_20200101_models.ModifyWebCacheSwitchRequest,
     ) -> ddoscoo_20200101_models.ModifyWebCacheSwitchResponse:
+        """
+        You can call the ModifyWebCacheSwitch operation to enable or disable the Static Page Caching policy for a website.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: ModifyWebCacheSwitchRequest
+        @return: ModifyWebCacheSwitchResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_web_cache_switch_with_options_async(request, runtime)
 
     def modify_web_ip_set_switch_with_options(
         self,
         request: ddoscoo_20200101_models.ModifyWebIpSetSwitchRequest,
         runtime: util_models.RuntimeOptions,
@@ -12462,14 +14582,21 @@
         return await self.modify_web_rule_with_options_async(request, runtime)
 
     def release_instance_with_options(
         self,
         request: ddoscoo_20200101_models.ReleaseInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.ReleaseInstanceResponse:
+        """
+        The ID of the request, which is used to locate and troubleshoot issues.
+        
+        @param request: ReleaseInstanceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ReleaseInstanceResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -12490,14 +14617,21 @@
         )
 
     async def release_instance_with_options_async(
         self,
         request: ddoscoo_20200101_models.ReleaseInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.ReleaseInstanceResponse:
+        """
+        The ID of the request, which is used to locate and troubleshoot issues.
+        
+        @param request: ReleaseInstanceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ReleaseInstanceResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -12517,29 +14651,51 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def release_instance(
         self,
         request: ddoscoo_20200101_models.ReleaseInstanceRequest,
     ) -> ddoscoo_20200101_models.ReleaseInstanceResponse:
+        """
+        The ID of the request, which is used to locate and troubleshoot issues.
+        
+        @param request: ReleaseInstanceRequest
+        @return: ReleaseInstanceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.release_instance_with_options(request, runtime)
 
     async def release_instance_async(
         self,
         request: ddoscoo_20200101_models.ReleaseInstanceRequest,
     ) -> ddoscoo_20200101_models.ReleaseInstanceResponse:
+        """
+        The ID of the request, which is used to locate and troubleshoot issues.
+        
+        @param request: ReleaseInstanceRequest
+        @return: ReleaseInstanceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.release_instance_with_options_async(request, runtime)
 
     def switch_scheduler_rule_with_options(
         self,
         request: ddoscoo_20200101_models.SwitchSchedulerRuleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.SwitchSchedulerRuleResponse:
+        """
+        You can call the SwitchSchedulerRule operation to modify the resources to which service traffic is switched for a scheduling rule. For example, you can switch service traffic to an Anti-DDoS Pro or Anti-DDoS Premium instance for scrubbing or switch the service traffic back to the associated cloud resources.
+        Before you call this operation, you must have created a scheduling rule by calling the [CreateSchedulerRule](~~157479~~) operation.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: SwitchSchedulerRuleRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SwitchSchedulerRuleResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.rule_name):
             query['RuleName'] = request.rule_name
         if not UtilClient.is_unset(request.rule_type):
             query['RuleType'] = request.rule_type
         if not UtilClient.is_unset(request.switch_data):
@@ -12564,14 +14720,24 @@
         )
 
     async def switch_scheduler_rule_with_options_async(
         self,
         request: ddoscoo_20200101_models.SwitchSchedulerRuleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ddoscoo_20200101_models.SwitchSchedulerRuleResponse:
+        """
+        You can call the SwitchSchedulerRule operation to modify the resources to which service traffic is switched for a scheduling rule. For example, you can switch service traffic to an Anti-DDoS Pro or Anti-DDoS Premium instance for scrubbing or switch the service traffic back to the associated cloud resources.
+        Before you call this operation, you must have created a scheduling rule by calling the [CreateSchedulerRule](~~157479~~) operation.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: SwitchSchedulerRuleRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SwitchSchedulerRuleResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.rule_name):
             query['RuleName'] = request.rule_name
         if not UtilClient.is_unset(request.rule_type):
             query['RuleType'] = request.rule_type
         if not UtilClient.is_unset(request.switch_data):
@@ -12595,16 +14761,34 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def switch_scheduler_rule(
         self,
         request: ddoscoo_20200101_models.SwitchSchedulerRuleRequest,
     ) -> ddoscoo_20200101_models.SwitchSchedulerRuleResponse:
+        """
+        You can call the SwitchSchedulerRule operation to modify the resources to which service traffic is switched for a scheduling rule. For example, you can switch service traffic to an Anti-DDoS Pro or Anti-DDoS Premium instance for scrubbing or switch the service traffic back to the associated cloud resources.
+        Before you call this operation, you must have created a scheduling rule by calling the [CreateSchedulerRule](~~157479~~) operation.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: SwitchSchedulerRuleRequest
+        @return: SwitchSchedulerRuleResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.switch_scheduler_rule_with_options(request, runtime)
 
     async def switch_scheduler_rule_async(
         self,
         request: ddoscoo_20200101_models.SwitchSchedulerRuleRequest,
     ) -> ddoscoo_20200101_models.SwitchSchedulerRuleResponse:
+        """
+        You can call the SwitchSchedulerRule operation to modify the resources to which service traffic is switched for a scheduling rule. For example, you can switch service traffic to an Anti-DDoS Pro or Anti-DDoS Premium instance for scrubbing or switch the service traffic back to the associated cloud resources.
+        Before you call this operation, you must have created a scheduling rule by calling the [CreateSchedulerRule](~~157479~~) operation.
+        ### Limits
+        You can call this operation up to 10 times per second per account. If the number of the calls per second exceeds the limit, throttling is triggered. As a result, your business may be affected. We recommend that you take note of the limit when you call this operation.
+        
+        @param request: SwitchSchedulerRuleRequest
+        @return: SwitchSchedulerRuleResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.switch_scheduler_rule_with_options_async(request, runtime)
```

### Comparing `alibabacloud_ddoscoo20200101-1.0.2/alibabacloud_ddoscoo20200101.egg-info/PKG-INFO` & `alibabacloud_ddoscoo20200101-1.0.3/alibabacloud_ddoscoo20200101.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-ddoscoo20200101
-Version: 1.0.2
+Version: 1.0.3
 Summary: Alibaba Cloud ddoscoo (20200101) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_ddoscoo20200101-1.0.2/setup.py` & `alibabacloud_ddoscoo20200101-1.0.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_ddoscoo20200101.
 
-Created on 30/06/2022
+Created on 19/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_ddoscoo20200101"
 NAME = "alibabacloud_ddoscoo20200101" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud ddoscoo (20200101) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.5, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.3, <1.0.0",
-    "alibabacloud_openapi_util>=0.1.6, <1.0.0",
+    "alibabacloud_tea_util>=0.3.10, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
+    "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

