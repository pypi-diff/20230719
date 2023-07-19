# Comparing `tmp/alibabacloud_pai-dlc20201203-1.2.6.tar.gz` & `tmp/alibabacloud_pai-dlc20201203-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_pai-dlc20201203-1.2.6.tar", last modified: Fri May 26 02:14:31 2023, max compression
+gzip compressed data, was "dist/alibabacloud_pai-dlc20201203-1.2.7.tar", last modified: Wed Jul 19 04:52:56 2023, max compression
```

## Comparing `alibabacloud_pai-dlc20201203-1.2.6.tar` & `alibabacloud_pai-dlc20201203-1.2.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:14:31.000000 alibabacloud_pai-dlc20201203-1.2.6/
--rw-r--r--   0 root         (0) root         (0)      750 2023-05-26 02:14:31.000000 alibabacloud_pai-dlc20201203-1.2.6/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-05-26 02:14:31.000000 alibabacloud_pai-dlc20201203-1.2.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-26 02:14:31.000000 alibabacloud_pai-dlc20201203-1.2.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2352 2023-05-26 02:14:31.000000 alibabacloud_pai-dlc20201203-1.2.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1034 2023-05-26 02:14:31.000000 alibabacloud_pai-dlc20201203-1.2.6/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1119 2023-05-26 02:14:31.000000 alibabacloud_pai-dlc20201203-1.2.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:14:31.000000 alibabacloud_pai-dlc20201203-1.2.6/alibabacloud_pai_dlc20201203/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-26 02:14:31.000000 alibabacloud_pai-dlc20201203-1.2.6/alibabacloud_pai_dlc20201203/__init__.py
--rw-r--r--   0 root         (0) root         (0)    73550 2023-05-26 02:14:31.000000 alibabacloud_pai-dlc20201203-1.2.6/alibabacloud_pai_dlc20201203/client.py
--rw-r--r--   0 root         (0) root         (0)   196320 2023-05-26 02:14:31.000000 alibabacloud_pai-dlc20201203-1.2.6/alibabacloud_pai_dlc20201203/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:14:31.000000 alibabacloud_pai-dlc20201203-1.2.6/alibabacloud_pai_dlc20201203.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2352 2023-05-26 02:14:31.000000 alibabacloud_pai-dlc20201203-1.2.6/alibabacloud_pai_dlc20201203.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      452 2023-05-26 02:14:31.000000 alibabacloud_pai-dlc20201203-1.2.6/alibabacloud_pai_dlc20201203.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 02:14:31.000000 alibabacloud_pai-dlc20201203-1.2.6/alibabacloud_pai_dlc20201203.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-05-26 02:14:31.000000 alibabacloud_pai-dlc20201203-1.2.6/alibabacloud_pai_dlc20201203.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-26 02:14:31.000000 alibabacloud_pai-dlc20201203-1.2.6/alibabacloud_pai_dlc20201203.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-26 02:14:31.000000 alibabacloud_pai-dlc20201203-1.2.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2632 2023-05-26 02:14:31.000000 alibabacloud_pai-dlc20201203-1.2.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 04:52:56.000000 alibabacloud_pai-dlc20201203-1.2.7/
+-rw-r--r--   0 root         (0) root         (0)      812 2023-07-19 04:52:56.000000 alibabacloud_pai-dlc20201203-1.2.7/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-19 04:52:56.000000 alibabacloud_pai-dlc20201203-1.2.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-19 04:52:56.000000 alibabacloud_pai-dlc20201203-1.2.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2352 2023-07-19 04:52:56.000000 alibabacloud_pai-dlc20201203-1.2.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1034 2023-07-19 04:52:56.000000 alibabacloud_pai-dlc20201203-1.2.7/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1119 2023-07-19 04:52:56.000000 alibabacloud_pai-dlc20201203-1.2.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 04:52:56.000000 alibabacloud_pai-dlc20201203-1.2.7/alibabacloud_pai_dlc20201203/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-19 04:52:56.000000 alibabacloud_pai-dlc20201203-1.2.7/alibabacloud_pai_dlc20201203/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    76692 2023-07-19 04:52:56.000000 alibabacloud_pai-dlc20201203-1.2.7/alibabacloud_pai_dlc20201203/client.py
+-rw-r--r--   0 root         (0) root         (0)   199100 2023-07-19 04:52:56.000000 alibabacloud_pai-dlc20201203-1.2.7/alibabacloud_pai_dlc20201203/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 04:52:56.000000 alibabacloud_pai-dlc20201203-1.2.7/alibabacloud_pai_dlc20201203.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2352 2023-07-19 04:52:56.000000 alibabacloud_pai-dlc20201203-1.2.7/alibabacloud_pai_dlc20201203.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      452 2023-07-19 04:52:56.000000 alibabacloud_pai-dlc20201203-1.2.7/alibabacloud_pai_dlc20201203.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 04:52:56.000000 alibabacloud_pai-dlc20201203-1.2.7/alibabacloud_pai_dlc20201203.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2023-07-19 04:52:56.000000 alibabacloud_pai-dlc20201203-1.2.7/alibabacloud_pai_dlc20201203.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-19 04:52:56.000000 alibabacloud_pai-dlc20201203-1.2.7/alibabacloud_pai_dlc20201203.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-19 04:52:56.000000 alibabacloud_pai-dlc20201203-1.2.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2633 2023-07-19 04:52:56.000000 alibabacloud_pai-dlc20201203-1.2.7/setup.py
```

### Comparing `alibabacloud_pai-dlc20201203-1.2.6/ChangeLog.md` & `alibabacloud_pai-dlc20201203-1.2.7/ChangeLog.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-05-26 Version: 1.2.6
+- Add parameter in JobElasticSpec.
+
 2023-03-23 Version: 1.2.5
 - Change the type of RequestId to string in GetJobEvents API.
 
 2023-01-04 Version: 1.2.4
 - Support images from private docker registry.
 
 2022-12-13 Version: 1.2.3
```

### Comparing `alibabacloud_pai-dlc20201203-1.2.6/LICENSE` & `alibabacloud_pai-dlc20201203-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_pai-dlc20201203-1.2.6/PKG-INFO` & `alibabacloud_pai-dlc20201203-1.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_pai-dlc20201203
-Version: 1.2.6
+Version: 1.2.7
 Summary: Alibaba Cloud pai-dlc (20201203) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_pai-dlc20201203-1.2.6/README-CN.md` & `alibabacloud_pai-dlc20201203-1.2.7/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_pai-dlc20201203-1.2.6/README.md` & `alibabacloud_pai-dlc20201203-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_pai-dlc20201203-1.2.6/alibabacloud_pai_dlc20201203/client.py` & `alibabacloud_pai-dlc20201203-1.2.7/alibabacloud_pai_dlc20201203/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1059,14 +1059,98 @@
         tensorboard_id: str,
         request: pai_dlc_20201203_models.GetTensorboardRequest,
     ) -> pai_dlc_20201203_models.GetTensorboardResponse:
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.get_tensorboard_with_options_async(tensorboard_id, request, headers, runtime)
 
+    def get_web_terminal_with_options(
+        self,
+        job_id: str,
+        pod_id: str,
+        request: pai_dlc_20201203_models.GetWebTerminalRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> pai_dlc_20201203_models.GetWebTerminalResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.pod_uid):
+            query['PodUid'] = request.pod_uid
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetWebTerminal',
+            version='2020-12-03',
+            protocol='HTTPS',
+            pathname=f'/api/v1/jobs/{OpenApiUtilClient.get_encode_param(job_id)}/pods/{OpenApiUtilClient.get_encode_param(pod_id)}/webterminal',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            pai_dlc_20201203_models.GetWebTerminalResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def get_web_terminal_with_options_async(
+        self,
+        job_id: str,
+        pod_id: str,
+        request: pai_dlc_20201203_models.GetWebTerminalRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> pai_dlc_20201203_models.GetWebTerminalResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.pod_uid):
+            query['PodUid'] = request.pod_uid
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetWebTerminal',
+            version='2020-12-03',
+            protocol='HTTPS',
+            pathname=f'/api/v1/jobs/{OpenApiUtilClient.get_encode_param(job_id)}/pods/{OpenApiUtilClient.get_encode_param(pod_id)}/webterminal',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            pai_dlc_20201203_models.GetWebTerminalResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def get_web_terminal(
+        self,
+        job_id: str,
+        pod_id: str,
+        request: pai_dlc_20201203_models.GetWebTerminalRequest,
+    ) -> pai_dlc_20201203_models.GetWebTerminalResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.get_web_terminal_with_options(job_id, pod_id, request, headers, runtime)
+
+    async def get_web_terminal_async(
+        self,
+        job_id: str,
+        pod_id: str,
+        request: pai_dlc_20201203_models.GetWebTerminalRequest,
+    ) -> pai_dlc_20201203_models.GetWebTerminalResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.get_web_terminal_with_options_async(job_id, pod_id, request, headers, runtime)
+
     def list_ecs_specs_with_options(
         self,
         request: pai_dlc_20201203_models.ListEcsSpecsRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> pai_dlc_20201203_models.ListEcsSpecsResponse:
         UtilClient.validate_model(request)
```

### Comparing `alibabacloud_pai-dlc20201203-1.2.6/alibabacloud_pai_dlc20201203/models.py` & `alibabacloud_pai-dlc20201203-1.2.7/alibabacloud_pai_dlc20201203/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -9924,2347 +9924,2521 @@
 00026c30: 2020 2020 2020 2020 2020 7465 6d70 5f6d            temp_m
 00026c40: 6f64 656c 203d 2054 656e 736f 7262 6f61  odel = Tensorboa
 00026c50: 7264 2829 0a20 2020 2020 2020 2020 2020  rd().           
 00026c60: 2073 656c 662e 626f 6479 203d 2074 656d   self.body = tem
 00026c70: 705f 6d6f 6465 6c2e 6672 6f6d 5f6d 6170  p_model.from_map
 00026c80: 286d 5b27 626f 6479 275d 290a 2020 2020  (m['body']).    
 00026c90: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
-00026ca0: 0a0a 636c 6173 7320 4c69 7374 4563 7353  ..class ListEcsS
-00026cb0: 7065 6373 5265 7175 6573 7428 5465 614d  pecsRequest(TeaM
-00026cc0: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
-00026cd0: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
-00026ce0: 2073 656c 662c 0a20 2020 2020 2020 2061   self,.        a
-00026cf0: 6363 656c 6572 6174 6f72 5f74 7970 653a  ccelerator_type:
-00026d00: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
-00026d10: 2020 2020 206f 7264 6572 3a20 7374 7220       order: str 
-00026d20: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00026d30: 7061 6765 5f6e 756d 6265 723a 2069 6e74  page_number: int
-00026d40: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00026d50: 2070 6167 655f 7369 7a65 3a20 696e 7420   page_size: int 
-00026d60: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00026d70: 736f 7274 5f62 793a 2073 7472 203d 204e  sort_by: str = N
-00026d80: 6f6e 652c 0a20 2020 2029 3a0a 2020 2020  one,.    ):.    
-00026d90: 2020 2020 7365 6c66 2e61 6363 656c 6572      self.acceler
-00026da0: 6174 6f72 5f74 7970 6520 3d20 6163 6365  ator_type = acce
-00026db0: 6c65 7261 746f 725f 7479 7065 0a20 2020  lerator_type.   
-00026dc0: 2020 2020 2073 656c 662e 6f72 6465 7220       self.order 
-00026dd0: 3d20 6f72 6465 720a 2020 2020 2020 2020  = order.        
-00026de0: 7365 6c66 2e70 6167 655f 6e75 6d62 6572  self.page_number
-00026df0: 203d 2070 6167 655f 6e75 6d62 6572 0a20   = page_number. 
-00026e00: 2020 2020 2020 2073 656c 662e 7061 6765         self.page
-00026e10: 5f73 697a 6520 3d20 7061 6765 5f73 697a  _size = page_siz
-00026e20: 650a 2020 2020 2020 2020 7365 6c66 2e73  e.        self.s
-00026e30: 6f72 745f 6279 203d 2073 6f72 745f 6279  ort_by = sort_by
-00026e40: 0a0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
-00026e50: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
-00026e60: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
-00026e70: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
-00026e80: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
-00026e90: 6572 2829 2e74 6f5f 6d61 7028 290a 2020  er().to_map().  
-00026ea0: 2020 2020 2020 6966 205f 6d61 7020 6973        if _map is
-00026eb0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00026ec0: 2020 2020 2020 2072 6574 7572 6e20 5f6d         return _m
-00026ed0: 6170 0a0a 2020 2020 2020 2020 7265 7375  ap..        resu
-00026ee0: 6c74 203d 2064 6963 7428 290a 2020 2020  lt = dict().    
-00026ef0: 2020 2020 6966 2073 656c 662e 6163 6365      if self.acce
-00026f00: 6c65 7261 746f 725f 7479 7065 2069 7320  lerator_type is 
-00026f10: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00026f20: 2020 2020 2020 7265 7375 6c74 5b27 4163        result['Ac
-00026f30: 6365 6c65 7261 746f 7254 7970 6527 5d20  celeratorType'] 
-00026f40: 3d20 7365 6c66 2e61 6363 656c 6572 6174  = self.accelerat
-00026f50: 6f72 5f74 7970 650a 2020 2020 2020 2020  or_type.        
-00026f60: 6966 2073 656c 662e 6f72 6465 7220 6973  if self.order is
-00026f70: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00026f80: 2020 2020 2020 2072 6573 756c 745b 274f         result['O
-00026f90: 7264 6572 275d 203d 2073 656c 662e 6f72  rder'] = self.or
-00026fa0: 6465 720a 2020 2020 2020 2020 6966 2073  der.        if s
-00026fb0: 656c 662e 7061 6765 5f6e 756d 6265 7220  elf.page_number 
-00026fc0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00026fd0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-00026fe0: 2750 6167 654e 756d 6265 7227 5d20 3d20  'PageNumber'] = 
-00026ff0: 7365 6c66 2e70 6167 655f 6e75 6d62 6572  self.page_number
-00027000: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00027010: 2e70 6167 655f 7369 7a65 2069 7320 6e6f  .page_size is no
-00027020: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00027030: 2020 2020 7265 7375 6c74 5b27 5061 6765      result['Page
-00027040: 5369 7a65 275d 203d 2073 656c 662e 7061  Size'] = self.pa
-00027050: 6765 5f73 697a 650a 2020 2020 2020 2020  ge_size.        
-00027060: 6966 2073 656c 662e 736f 7274 5f62 7920  if self.sort_by 
-00027070: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00027080: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-00027090: 2753 6f72 7442 7927 5d20 3d20 7365 6c66  'SortBy'] = self
-000270a0: 2e73 6f72 745f 6279 0a20 2020 2020 2020  .sort_by.       
-000270b0: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
-000270c0: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
-000270d0: 2873 656c 662c 206d 3a20 6469 6374 203d  (self, m: dict =
-000270e0: 204e 6f6e 6529 3a0a 2020 2020 2020 2020   None):.        
-000270f0: 6d20 3d20 6d20 6f72 2064 6963 7428 290a  m = m or dict().
-00027100: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-00027110: 2827 4163 6365 6c65 7261 746f 7254 7970  ('AcceleratorTyp
-00027120: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
-00027130: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00027140: 662e 6163 6365 6c65 7261 746f 725f 7479  f.accelerator_ty
-00027150: 7065 203d 206d 2e67 6574 2827 4163 6365  pe = m.get('Acce
-00027160: 6c65 7261 746f 7254 7970 6527 290a 2020  leratorType').  
-00027170: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-00027180: 4f72 6465 7227 2920 6973 206e 6f74 204e  Order') is not N
-00027190: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000271a0: 2073 656c 662e 6f72 6465 7220 3d20 6d2e   self.order = m.
-000271b0: 6765 7428 274f 7264 6572 2729 0a20 2020  get('Order').   
-000271c0: 2020 2020 2069 6620 6d2e 6765 7428 2750       if m.get('P
-000271d0: 6167 654e 756d 6265 7227 2920 6973 206e  ageNumber') is n
-000271e0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000271f0: 2020 2020 2073 656c 662e 7061 6765 5f6e       self.page_n
-00027200: 756d 6265 7220 3d20 6d2e 6765 7428 2750  umber = m.get('P
-00027210: 6167 654e 756d 6265 7227 290a 2020 2020  ageNumber').    
-00027220: 2020 2020 6966 206d 2e67 6574 2827 5061      if m.get('Pa
-00027230: 6765 5369 7a65 2729 2069 7320 6e6f 7420  geSize') is not 
-00027240: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00027250: 2020 7365 6c66 2e70 6167 655f 7369 7a65    self.page_size
-00027260: 203d 206d 2e67 6574 2827 5061 6765 5369   = m.get('PageSi
-00027270: 7a65 2729 0a20 2020 2020 2020 2069 6620  ze').        if 
-00027280: 6d2e 6765 7428 2753 6f72 7442 7927 2920  m.get('SortBy') 
-00027290: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000272a0: 2020 2020 2020 2020 2073 656c 662e 736f           self.so
-000272b0: 7274 5f62 7920 3d20 6d2e 6765 7428 2753  rt_by = m.get('S
-000272c0: 6f72 7442 7927 290a 2020 2020 2020 2020  ortBy').        
-000272d0: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
-000272e0: 6173 7320 4c69 7374 4563 7353 7065 6373  ass ListEcsSpecs
-000272f0: 5265 7370 6f6e 7365 426f 6479 2854 6561  ResponseBody(Tea
-00027300: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
-00027310: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
-00027320: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-00027330: 6563 735f 7370 6563 733a 204c 6973 745b  ecs_specs: List[
-00027340: 4563 7353 7065 635d 203d 204e 6f6e 652c  EcsSpec] = None,
-00027350: 0a20 2020 2020 2020 2072 6571 7565 7374  .        request
-00027360: 5f69 643a 2073 7472 203d 204e 6f6e 652c  _id: str = None,
-00027370: 0a20 2020 2020 2020 2074 6f74 616c 5f63  .        total_c
-00027380: 6f75 6e74 3a20 696e 7420 3d20 4e6f 6e65  ount: int = None
-00027390: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
-000273a0: 2073 656c 662e 6563 735f 7370 6563 7320   self.ecs_specs 
-000273b0: 3d20 6563 735f 7370 6563 730a 2020 2020  = ecs_specs.    
-000273c0: 2020 2020 7365 6c66 2e72 6571 7565 7374      self.request
-000273d0: 5f69 6420 3d20 7265 7175 6573 745f 6964  _id = request_id
-000273e0: 0a20 2020 2020 2020 2073 656c 662e 746f  .        self.to
-000273f0: 7461 6c5f 636f 756e 7420 3d20 746f 7461  tal_count = tota
-00027400: 6c5f 636f 756e 740a 0a20 2020 2064 6566  l_count..    def
-00027410: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
-00027420: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00027430: 2e65 6373 5f73 7065 6373 3a0a 2020 2020  .ecs_specs:.    
-00027440: 2020 2020 2020 2020 666f 7220 6b20 696e          for k in
-00027450: 2073 656c 662e 6563 735f 7370 6563 733a   self.ecs_specs:
-00027460: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00027470: 2069 6620 6b3a 0a20 2020 2020 2020 2020   if k:.         
-00027480: 2020 2020 2020 2020 2020 206b 2e76 616c             k.val
-00027490: 6964 6174 6528 290a 0a20 2020 2064 6566  idate()..    def
-000274a0: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
-000274b0: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
-000274c0: 7065 7228 292e 746f 5f6d 6170 2829 0a20  per().to_map(). 
-000274d0: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
-000274e0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000274f0: 2020 2020 2020 2020 7265 7475 726e 205f          return _
-00027500: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
-00027510: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
-00027520: 2020 2020 2072 6573 756c 745b 2745 6373       result['Ecs
-00027530: 5370 6563 7327 5d20 3d20 5b5d 0a20 2020  Specs'] = [].   
-00027540: 2020 2020 2069 6620 7365 6c66 2e65 6373       if self.ecs
-00027550: 5f73 7065 6373 2069 7320 6e6f 7420 4e6f  _specs is not No
-00027560: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00027570: 666f 7220 6b20 696e 2073 656c 662e 6563  for k in self.ec
-00027580: 735f 7370 6563 733a 0a20 2020 2020 2020  s_specs:.       
-00027590: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-000275a0: 2745 6373 5370 6563 7327 5d2e 6170 7065  'EcsSpecs'].appe
-000275b0: 6e64 286b 2e74 6f5f 6d61 7028 2920 6966  nd(k.to_map() if
-000275c0: 206b 2065 6c73 6520 4e6f 6e65 290a 2020   k else None).  
-000275d0: 2020 2020 2020 6966 2073 656c 662e 7265        if self.re
-000275e0: 7175 6573 745f 6964 2069 7320 6e6f 7420  quest_id is not 
-000275f0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00027600: 2020 7265 7375 6c74 5b27 5265 7175 6573    result['Reques
-00027610: 7449 6427 5d20 3d20 7365 6c66 2e72 6571  tId'] = self.req
-00027620: 7565 7374 5f69 640a 2020 2020 2020 2020  uest_id.        
-00027630: 6966 2073 656c 662e 746f 7461 6c5f 636f  if self.total_co
-00027640: 756e 7420 6973 206e 6f74 204e 6f6e 653a  unt is not None:
-00027650: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00027660: 756c 745b 2754 6f74 616c 436f 756e 7427  ult['TotalCount'
-00027670: 5d20 3d20 7365 6c66 2e74 6f74 616c 5f63  ] = self.total_c
-00027680: 6f75 6e74 0a20 2020 2020 2020 2072 6574  ount.        ret
-00027690: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
-000276a0: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
-000276b0: 662c 206d 3a20 6469 6374 203d 204e 6f6e  f, m: dict = Non
-000276c0: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
-000276d0: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
-000276e0: 2020 2020 7365 6c66 2e65 6373 5f73 7065      self.ecs_spe
-000276f0: 6373 203d 205b 5d0a 2020 2020 2020 2020  cs = [].        
-00027700: 6966 206d 2e67 6574 2827 4563 7353 7065  if m.get('EcsSpe
-00027710: 6373 2729 2069 7320 6e6f 7420 4e6f 6e65  cs') is not None
-00027720: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
-00027730: 7220 6b20 696e 206d 2e67 6574 2827 4563  r k in m.get('Ec
-00027740: 7353 7065 6373 2729 3a0a 2020 2020 2020  sSpecs'):.      
-00027750: 2020 2020 2020 2020 2020 7465 6d70 5f6d            temp_m
-00027760: 6f64 656c 203d 2045 6373 5370 6563 2829  odel = EcsSpec()
-00027770: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00027780: 2073 656c 662e 6563 735f 7370 6563 732e   self.ecs_specs.
-00027790: 6170 7065 6e64 2874 656d 705f 6d6f 6465  append(temp_mode
-000277a0: 6c2e 6672 6f6d 5f6d 6170 286b 2929 0a20  l.from_map(k)). 
-000277b0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-000277c0: 2752 6571 7565 7374 4964 2729 2069 7320  'RequestId') is 
-000277d0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000277e0: 2020 2020 2020 7365 6c66 2e72 6571 7565        self.reque
-000277f0: 7374 5f69 6420 3d20 6d2e 6765 7428 2752  st_id = m.get('R
-00027800: 6571 7565 7374 4964 2729 0a20 2020 2020  equestId').     
-00027810: 2020 2069 6620 6d2e 6765 7428 2754 6f74     if m.get('Tot
-00027820: 616c 436f 756e 7427 2920 6973 206e 6f74  alCount') is not
-00027830: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00027840: 2020 2073 656c 662e 746f 7461 6c5f 636f     self.total_co
-00027850: 756e 7420 3d20 6d2e 6765 7428 2754 6f74  unt = m.get('Tot
-00027860: 616c 436f 756e 7427 290a 2020 2020 2020  alCount').      
-00027870: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
-00027880: 636c 6173 7320 4c69 7374 4563 7353 7065  class ListEcsSpe
-00027890: 6373 5265 7370 6f6e 7365 2854 6561 4d6f  csResponse(TeaMo
-000278a0: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
-000278b0: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
-000278c0: 7365 6c66 2c0a 2020 2020 2020 2020 6865  self,.        he
-000278d0: 6164 6572 733a 2044 6963 745b 7374 722c  aders: Dict[str,
-000278e0: 2073 7472 5d20 3d20 4e6f 6e65 2c0a 2020   str] = None,.  
-000278f0: 2020 2020 2020 7374 6174 7573 5f63 6f64        status_cod
-00027900: 653a 2069 6e74 203d 204e 6f6e 652c 0a20  e: int = None,. 
-00027910: 2020 2020 2020 2062 6f64 793a 204c 6973         body: Lis
-00027920: 7445 6373 5370 6563 7352 6573 706f 6e73  tEcsSpecsRespons
-00027930: 6542 6f64 7920 3d20 4e6f 6e65 2c0a 2020  eBody = None,.  
-00027940: 2020 293a 0a20 2020 2020 2020 2073 656c    ):.        sel
-00027950: 662e 6865 6164 6572 7320 3d20 6865 6164  f.headers = head
-00027960: 6572 730a 2020 2020 2020 2020 7365 6c66  ers.        self
-00027970: 2e73 7461 7475 735f 636f 6465 203d 2073  .status_code = s
-00027980: 7461 7475 735f 636f 6465 0a20 2020 2020  tatus_code.     
-00027990: 2020 2073 656c 662e 626f 6479 203d 2062     self.body = b
-000279a0: 6f64 790a 0a20 2020 2064 6566 2076 616c  ody..    def val
-000279b0: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
-000279c0: 2020 2020 2073 656c 662e 7661 6c69 6461       self.valida
-000279d0: 7465 5f72 6571 7569 7265 6428 7365 6c66  te_required(self
-000279e0: 2e68 6561 6465 7273 2c20 2768 6561 6465  .headers, 'heade
-000279f0: 7273 2729 0a20 2020 2020 2020 2073 656c  rs').        sel
-00027a00: 662e 7661 6c69 6461 7465 5f72 6571 7569  f.validate_requi
-00027a10: 7265 6428 7365 6c66 2e73 7461 7475 735f  red(self.status_
-00027a20: 636f 6465 2c20 2773 7461 7475 735f 636f  code, 'status_co
-00027a30: 6465 2729 0a20 2020 2020 2020 2073 656c  de').        sel
-00027a40: 662e 7661 6c69 6461 7465 5f72 6571 7569  f.validate_requi
-00027a50: 7265 6428 7365 6c66 2e62 6f64 792c 2027  red(self.body, '
-00027a60: 626f 6479 2729 0a20 2020 2020 2020 2069  body').        i
-00027a70: 6620 7365 6c66 2e62 6f64 793a 0a20 2020  f self.body:.   
-00027a80: 2020 2020 2020 2020 2073 656c 662e 626f           self.bo
-00027a90: 6479 2e76 616c 6964 6174 6528 290a 0a20  dy.validate().. 
-00027aa0: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
-00027ab0: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
-00027ac0: 7020 3d20 7375 7065 7228 292e 746f 5f6d  p = super().to_m
-00027ad0: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
-00027ae0: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
-00027af0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00027b00: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
-00027b10: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
-00027b20: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
-00027b30: 6c66 2e68 6561 6465 7273 2069 7320 6e6f  lf.headers is no
-00027b40: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00027b50: 2020 2020 7265 7375 6c74 5b27 6865 6164      result['head
-00027b60: 6572 7327 5d20 3d20 7365 6c66 2e68 6561  ers'] = self.hea
-00027b70: 6465 7273 0a20 2020 2020 2020 2069 6620  ders.        if 
-00027b80: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
-00027b90: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00027ba0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00027bb0: 5b27 7374 6174 7573 436f 6465 275d 203d  ['statusCode'] =
-00027bc0: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
-00027bd0: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
-00027be0: 662e 626f 6479 2069 7320 6e6f 7420 4e6f  f.body is not No
-00027bf0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00027c00: 7265 7375 6c74 5b27 626f 6479 275d 203d  result['body'] =
-00027c10: 2073 656c 662e 626f 6479 2e74 6f5f 6d61   self.body.to_ma
-00027c20: 7028 290a 2020 2020 2020 2020 7265 7475  p().        retu
-00027c30: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
-00027c40: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
-00027c50: 2c20 6d3a 2064 6963 7420 3d20 4e6f 6e65  , m: dict = None
-00027c60: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
-00027c70: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
-00027c80: 2020 2069 6620 6d2e 6765 7428 2768 6561     if m.get('hea
-00027c90: 6465 7273 2729 2069 7320 6e6f 7420 4e6f  ders') is not No
-00027ca0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00027cb0: 7365 6c66 2e68 6561 6465 7273 203d 206d  self.headers = m
-00027cc0: 2e67 6574 2827 6865 6164 6572 7327 290a  .get('headers').
-00027cd0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-00027ce0: 2827 7374 6174 7573 436f 6465 2729 2069  ('statusCode') i
-00027cf0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00027d00: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
-00027d10: 7475 735f 636f 6465 203d 206d 2e67 6574  tus_code = m.get
-00027d20: 2827 7374 6174 7573 436f 6465 2729 0a20  ('statusCode'). 
-00027d30: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-00027d40: 2762 6f64 7927 2920 6973 206e 6f74 204e  'body') is not N
-00027d50: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00027d60: 2074 656d 705f 6d6f 6465 6c20 3d20 4c69   temp_model = Li
-00027d70: 7374 4563 7353 7065 6373 5265 7370 6f6e  stEcsSpecsRespon
-00027d80: 7365 426f 6479 2829 0a20 2020 2020 2020  seBody().       
-00027d90: 2020 2020 2073 656c 662e 626f 6479 203d       self.body =
-00027da0: 2074 656d 705f 6d6f 6465 6c2e 6672 6f6d   temp_model.from
-00027db0: 5f6d 6170 286d 5b27 626f 6479 275d 290a  _map(m['body']).
-00027dc0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00027dd0: 656c 660a 0a0a 636c 6173 7320 4c69 7374  elf...class List
-00027de0: 4a6f 6273 5265 7175 6573 7428 5465 614d  JobsRequest(TeaM
-00027df0: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
-00027e00: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
-00027e10: 2073 656c 662c 0a20 2020 2020 2020 2062   self,.        b
-00027e20: 7573 696e 6573 735f 7573 6572 5f69 643a  usiness_user_id:
-00027e30: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
-00027e40: 2020 2020 2063 616c 6c65 723a 2073 7472       caller: str
-00027e50: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00027e60: 2064 6973 706c 6179 5f6e 616d 653a 2073   display_name: s
-00027e70: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
-00027e80: 2020 2065 6e64 5f74 696d 653a 2073 7472     end_time: str
-00027e90: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00027ea0: 2066 726f 6d5f 616c 6c5f 776f 726b 7370   from_all_worksp
-00027eb0: 6163 6573 3a20 626f 6f6c 203d 204e 6f6e  aces: bool = Non
-00027ec0: 652c 0a20 2020 2020 2020 206a 6f62 5f69  e,.        job_i
-00027ed0: 643a 2073 7472 203d 204e 6f6e 652c 0a20  d: str = None,. 
-00027ee0: 2020 2020 2020 206a 6f62 5f74 7970 653a         job_type:
-00027ef0: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
-00027f00: 2020 2020 206f 7264 6572 3a20 7374 7220       order: str 
-00027f10: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00027f20: 7061 6765 5f6e 756d 6265 723a 2069 6e74  page_number: int
-00027f30: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00027f40: 2070 6167 655f 7369 7a65 3a20 696e 7420   page_size: int 
-00027f50: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00027f60: 7069 7065 6c69 6e65 5f69 643a 2073 7472  pipeline_id: str
-00027f70: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00027f80: 2072 6573 6f75 7263 655f 6964 3a20 7374   resource_id: st
-00027f90: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
-00027fa0: 2020 7368 6f77 5f6f 776e 3a20 626f 6f6c    show_own: bool
-00027fb0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00027fc0: 2073 6f72 745f 6279 3a20 7374 7220 3d20   sort_by: str = 
-00027fd0: 4e6f 6e65 2c0a 2020 2020 2020 2020 7374  None,.        st
-00027fe0: 6172 745f 7469 6d65 3a20 7374 7220 3d20  art_time: str = 
-00027ff0: 4e6f 6e65 2c0a 2020 2020 2020 2020 7374  None,.        st
-00028000: 6174 7573 3a20 7374 7220 3d20 4e6f 6e65  atus: str = None
-00028010: 2c0a 2020 2020 2020 2020 7461 6773 3a20  ,.        tags: 
-00028020: 4469 6374 5b73 7472 2c20 7374 725d 203d  Dict[str, str] =
-00028030: 204e 6f6e 652c 0a20 2020 2020 2020 2077   None,.        w
-00028040: 6f72 6b73 7061 6365 5f69 643a 2073 7472  orkspace_id: str
-00028050: 203d 204e 6f6e 652c 0a20 2020 2029 3a0a   = None,.    ):.
-00028060: 2020 2020 2020 2020 7365 6c66 2e62 7573          self.bus
-00028070: 696e 6573 735f 7573 6572 5f69 6420 3d20  iness_user_id = 
-00028080: 6275 7369 6e65 7373 5f75 7365 725f 6964  business_user_id
-00028090: 0a20 2020 2020 2020 2073 656c 662e 6361  .        self.ca
-000280a0: 6c6c 6572 203d 2063 616c 6c65 720a 2020  ller = caller.  
-000280b0: 2020 2020 2020 7365 6c66 2e64 6973 706c        self.displ
-000280c0: 6179 5f6e 616d 6520 3d20 6469 7370 6c61  ay_name = displa
-000280d0: 795f 6e61 6d65 0a20 2020 2020 2020 2073  y_name.        s
-000280e0: 656c 662e 656e 645f 7469 6d65 203d 2065  elf.end_time = e
-000280f0: 6e64 5f74 696d 650a 2020 2020 2020 2020  nd_time.        
-00028100: 7365 6c66 2e66 726f 6d5f 616c 6c5f 776f  self.from_all_wo
-00028110: 726b 7370 6163 6573 203d 2066 726f 6d5f  rkspaces = from_
-00028120: 616c 6c5f 776f 726b 7370 6163 6573 0a20  all_workspaces. 
-00028130: 2020 2020 2020 2073 656c 662e 6a6f 625f         self.job_
-00028140: 6964 203d 206a 6f62 5f69 640a 2020 2020  id = job_id.    
-00028150: 2020 2020 7365 6c66 2e6a 6f62 5f74 7970      self.job_typ
-00028160: 6520 3d20 6a6f 625f 7479 7065 0a20 2020  e = job_type.   
-00028170: 2020 2020 2073 656c 662e 6f72 6465 7220       self.order 
-00028180: 3d20 6f72 6465 720a 2020 2020 2020 2020  = order.        
-00028190: 7365 6c66 2e70 6167 655f 6e75 6d62 6572  self.page_number
-000281a0: 203d 2070 6167 655f 6e75 6d62 6572 0a20   = page_number. 
-000281b0: 2020 2020 2020 2073 656c 662e 7061 6765         self.page
-000281c0: 5f73 697a 6520 3d20 7061 6765 5f73 697a  _size = page_siz
-000281d0: 650a 2020 2020 2020 2020 7365 6c66 2e70  e.        self.p
-000281e0: 6970 656c 696e 655f 6964 203d 2070 6970  ipeline_id = pip
-000281f0: 656c 696e 655f 6964 0a20 2020 2020 2020  eline_id.       
-00028200: 2073 656c 662e 7265 736f 7572 6365 5f69   self.resource_i
-00028210: 6420 3d20 7265 736f 7572 6365 5f69 640a  d = resource_id.
-00028220: 2020 2020 2020 2020 7365 6c66 2e73 686f          self.sho
-00028230: 775f 6f77 6e20 3d20 7368 6f77 5f6f 776e  w_own = show_own
-00028240: 0a20 2020 2020 2020 2073 656c 662e 736f  .        self.so
-00028250: 7274 5f62 7920 3d20 736f 7274 5f62 790a  rt_by = sort_by.
-00028260: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
-00028270: 7274 5f74 696d 6520 3d20 7374 6172 745f  rt_time = start_
-00028280: 7469 6d65 0a20 2020 2020 2020 2073 656c  time.        sel
-00028290: 662e 7374 6174 7573 203d 2073 7461 7475  f.status = statu
-000282a0: 730a 2020 2020 2020 2020 7365 6c66 2e74  s.        self.t
-000282b0: 6167 7320 3d20 7461 6773 0a20 2020 2020  ags = tags.     
-000282c0: 2020 2073 656c 662e 776f 726b 7370 6163     self.workspac
-000282d0: 655f 6964 203d 2077 6f72 6b73 7061 6365  e_id = workspace
-000282e0: 5f69 640a 0a20 2020 2064 6566 2076 616c  _id..    def val
-000282f0: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
-00028300: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
-00028310: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
-00028320: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
-00028330: 7375 7065 7228 292e 746f 5f6d 6170 2829  super().to_map()
-00028340: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
-00028350: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00028360: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00028370: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
-00028380: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
-00028390: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
-000283a0: 7573 696e 6573 735f 7573 6572 5f69 6420  usiness_user_id 
-000283b0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-000283c0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-000283d0: 2742 7573 696e 6573 7355 7365 7249 6427  'BusinessUserId'
-000283e0: 5d20 3d20 7365 6c66 2e62 7573 696e 6573  ] = self.busines
-000283f0: 735f 7573 6572 5f69 640a 2020 2020 2020  s_user_id.      
-00028400: 2020 6966 2073 656c 662e 6361 6c6c 6572    if self.caller
-00028410: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00028420: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00028430: 5b27 4361 6c6c 6572 275d 203d 2073 656c  ['Caller'] = sel
-00028440: 662e 6361 6c6c 6572 0a20 2020 2020 2020  f.caller.       
-00028450: 2069 6620 7365 6c66 2e64 6973 706c 6179   if self.display
-00028460: 5f6e 616d 6520 6973 206e 6f74 204e 6f6e  _name is not Non
-00028470: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00028480: 6573 756c 745b 2744 6973 706c 6179 4e61  esult['DisplayNa
-00028490: 6d65 275d 203d 2073 656c 662e 6469 7370  me'] = self.disp
-000284a0: 6c61 795f 6e61 6d65 0a20 2020 2020 2020  lay_name.       
-000284b0: 2069 6620 7365 6c66 2e65 6e64 5f74 696d   if self.end_tim
-000284c0: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
-000284d0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-000284e0: 745b 2745 6e64 5469 6d65 275d 203d 2073  t['EndTime'] = s
-000284f0: 656c 662e 656e 645f 7469 6d65 0a20 2020  elf.end_time.   
-00028500: 2020 2020 2069 6620 7365 6c66 2e66 726f       if self.fro
-00028510: 6d5f 616c 6c5f 776f 726b 7370 6163 6573  m_all_workspaces
-00028520: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00028530: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00028540: 5b27 4672 6f6d 416c 6c57 6f72 6b73 7061  ['FromAllWorkspa
-00028550: 6365 7327 5d20 3d20 7365 6c66 2e66 726f  ces'] = self.fro
-00028560: 6d5f 616c 6c5f 776f 726b 7370 6163 6573  m_all_workspaces
-00028570: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00028580: 2e6a 6f62 5f69 6420 6973 206e 6f74 204e  .job_id is not N
-00028590: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000285a0: 2072 6573 756c 745b 274a 6f62 4964 275d   result['JobId']
-000285b0: 203d 2073 656c 662e 6a6f 625f 6964 0a20   = self.job_id. 
-000285c0: 2020 2020 2020 2069 6620 7365 6c66 2e6a         if self.j
-000285d0: 6f62 5f74 7970 6520 6973 206e 6f74 204e  ob_type is not N
-000285e0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000285f0: 2072 6573 756c 745b 274a 6f62 5479 7065   result['JobType
-00028600: 275d 203d 2073 656c 662e 6a6f 625f 7479  '] = self.job_ty
-00028610: 7065 0a20 2020 2020 2020 2069 6620 7365  pe.        if se
-00028620: 6c66 2e6f 7264 6572 2069 7320 6e6f 7420  lf.order is not 
-00028630: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00028640: 2020 7265 7375 6c74 5b27 4f72 6465 7227    result['Order'
-00028650: 5d20 3d20 7365 6c66 2e6f 7264 6572 0a20  ] = self.order. 
-00028660: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
-00028670: 6167 655f 6e75 6d62 6572 2069 7320 6e6f  age_number is no
-00028680: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00028690: 2020 2020 7265 7375 6c74 5b27 5061 6765      result['Page
-000286a0: 4e75 6d62 6572 275d 203d 2073 656c 662e  Number'] = self.
-000286b0: 7061 6765 5f6e 756d 6265 720a 2020 2020  page_number.    
-000286c0: 2020 2020 6966 2073 656c 662e 7061 6765      if self.page
-000286d0: 5f73 697a 6520 6973 206e 6f74 204e 6f6e  _size is not Non
-000286e0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-000286f0: 6573 756c 745b 2750 6167 6553 697a 6527  esult['PageSize'
-00028700: 5d20 3d20 7365 6c66 2e70 6167 655f 7369  ] = self.page_si
-00028710: 7a65 0a20 2020 2020 2020 2069 6620 7365  ze.        if se
-00028720: 6c66 2e70 6970 656c 696e 655f 6964 2069  lf.pipeline_id i
-00028730: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00028740: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-00028750: 5069 7065 6c69 6e65 4964 275d 203d 2073  PipelineId'] = s
-00028760: 656c 662e 7069 7065 6c69 6e65 5f69 640a  elf.pipeline_id.
-00028770: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00028780: 7265 736f 7572 6365 5f69 6420 6973 206e  resource_id is n
-00028790: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000287a0: 2020 2020 2072 6573 756c 745b 2752 6573       result['Res
-000287b0: 6f75 7263 6549 6427 5d20 3d20 7365 6c66  ourceId'] = self
-000287c0: 2e72 6573 6f75 7263 655f 6964 0a20 2020  .resource_id.   
-000287d0: 2020 2020 2069 6620 7365 6c66 2e73 686f       if self.sho
-000287e0: 775f 6f77 6e20 6973 206e 6f74 204e 6f6e  w_own is not Non
-000287f0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00028800: 6573 756c 745b 2753 686f 774f 776e 275d  esult['ShowOwn']
-00028810: 203d 2073 656c 662e 7368 6f77 5f6f 776e   = self.show_own
-00028820: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00028830: 2e73 6f72 745f 6279 2069 7320 6e6f 7420  .sort_by is not 
-00028840: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00028850: 2020 7265 7375 6c74 5b27 536f 7274 4279    result['SortBy
-00028860: 275d 203d 2073 656c 662e 736f 7274 5f62  '] = self.sort_b
-00028870: 790a 2020 2020 2020 2020 6966 2073 656c  y.        if sel
-00028880: 662e 7374 6172 745f 7469 6d65 2069 7320  f.start_time is 
-00028890: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000288a0: 2020 2020 2020 7265 7375 6c74 5b27 5374        result['St
-000288b0: 6172 7454 696d 6527 5d20 3d20 7365 6c66  artTime'] = self
-000288c0: 2e73 7461 7274 5f74 696d 650a 2020 2020  .start_time.    
-000288d0: 2020 2020 6966 2073 656c 662e 7374 6174      if self.stat
-000288e0: 7573 2069 7320 6e6f 7420 4e6f 6e65 3a0a  us is not None:.
-000288f0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00028900: 6c74 5b27 5374 6174 7573 275d 203d 2073  lt['Status'] = s
-00028910: 656c 662e 7374 6174 7573 0a20 2020 2020  elf.status.     
-00028920: 2020 2069 6620 7365 6c66 2e74 6167 7320     if self.tags 
-00028930: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00028940: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-00028950: 2754 6167 7327 5d20 3d20 7365 6c66 2e74  'Tags'] = self.t
-00028960: 6167 730a 2020 2020 2020 2020 6966 2073  ags.        if s
-00028970: 656c 662e 776f 726b 7370 6163 655f 6964  elf.workspace_id
-00028980: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00028990: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-000289a0: 5b27 576f 726b 7370 6163 6549 6427 5d20  ['WorkspaceId'] 
-000289b0: 3d20 7365 6c66 2e77 6f72 6b73 7061 6365  = self.workspace
-000289c0: 5f69 640a 2020 2020 2020 2020 7265 7475  _id.        retu
-000289d0: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
-000289e0: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
-000289f0: 2c20 6d3a 2064 6963 7420 3d20 4e6f 6e65  , m: dict = None
-00028a00: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
-00028a10: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
-00028a20: 2020 2069 6620 6d2e 6765 7428 2742 7573     if m.get('Bus
-00028a30: 696e 6573 7355 7365 7249 6427 2920 6973  inessUserId') is
-00028a40: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00028a50: 2020 2020 2020 2073 656c 662e 6275 7369         self.busi
-00028a60: 6e65 7373 5f75 7365 725f 6964 203d 206d  ness_user_id = m
-00028a70: 2e67 6574 2827 4275 7369 6e65 7373 5573  .get('BusinessUs
-00028a80: 6572 4964 2729 0a20 2020 2020 2020 2069  erId').        i
-00028a90: 6620 6d2e 6765 7428 2743 616c 6c65 7227  f m.get('Caller'
-00028aa0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-00028ab0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00028ac0: 6361 6c6c 6572 203d 206d 2e67 6574 2827  caller = m.get('
-00028ad0: 4361 6c6c 6572 2729 0a20 2020 2020 2020  Caller').       
-00028ae0: 2069 6620 6d2e 6765 7428 2744 6973 706c   if m.get('Displ
-00028af0: 6179 4e61 6d65 2729 2069 7320 6e6f 7420  ayName') is not 
-00028b00: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00028b10: 2020 7365 6c66 2e64 6973 706c 6179 5f6e    self.display_n
-00028b20: 616d 6520 3d20 6d2e 6765 7428 2744 6973  ame = m.get('Dis
-00028b30: 706c 6179 4e61 6d65 2729 0a20 2020 2020  playName').     
-00028b40: 2020 2069 6620 6d2e 6765 7428 2745 6e64     if m.get('End
-00028b50: 5469 6d65 2729 2069 7320 6e6f 7420 4e6f  Time') is not No
-00028b60: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00028b70: 7365 6c66 2e65 6e64 5f74 696d 6520 3d20  self.end_time = 
-00028b80: 6d2e 6765 7428 2745 6e64 5469 6d65 2729  m.get('EndTime')
-00028b90: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-00028ba0: 7428 2746 726f 6d41 6c6c 576f 726b 7370  t('FromAllWorksp
-00028bb0: 6163 6573 2729 2069 7320 6e6f 7420 4e6f  aces') is not No
-00028bc0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00028bd0: 7365 6c66 2e66 726f 6d5f 616c 6c5f 776f  self.from_all_wo
-00028be0: 726b 7370 6163 6573 203d 206d 2e67 6574  rkspaces = m.get
-00028bf0: 2827 4672 6f6d 416c 6c57 6f72 6b73 7061  ('FromAllWorkspa
-00028c00: 6365 7327 290a 2020 2020 2020 2020 6966  ces').        if
-00028c10: 206d 2e67 6574 2827 4a6f 6249 6427 2920   m.get('JobId') 
-00028c20: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00028c30: 2020 2020 2020 2020 2073 656c 662e 6a6f           self.jo
-00028c40: 625f 6964 203d 206d 2e67 6574 2827 4a6f  b_id = m.get('Jo
-00028c50: 6249 6427 290a 2020 2020 2020 2020 6966  bId').        if
-00028c60: 206d 2e67 6574 2827 4a6f 6254 7970 6527   m.get('JobType'
-00028c70: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-00028c80: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00028c90: 6a6f 625f 7479 7065 203d 206d 2e67 6574  job_type = m.get
-00028ca0: 2827 4a6f 6254 7970 6527 290a 2020 2020  ('JobType').    
-00028cb0: 2020 2020 6966 206d 2e67 6574 2827 4f72      if m.get('Or
-00028cc0: 6465 7227 2920 6973 206e 6f74 204e 6f6e  der') is not Non
-00028cd0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00028ce0: 656c 662e 6f72 6465 7220 3d20 6d2e 6765  elf.order = m.ge
-00028cf0: 7428 274f 7264 6572 2729 0a20 2020 2020  t('Order').     
-00028d00: 2020 2069 6620 6d2e 6765 7428 2750 6167     if m.get('Pag
-00028d10: 654e 756d 6265 7227 2920 6973 206e 6f74  eNumber') is not
-00028d20: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00028d30: 2020 2073 656c 662e 7061 6765 5f6e 756d     self.page_num
-00028d40: 6265 7220 3d20 6d2e 6765 7428 2750 6167  ber = m.get('Pag
-00028d50: 654e 756d 6265 7227 290a 2020 2020 2020  eNumber').      
-00028d60: 2020 6966 206d 2e67 6574 2827 5061 6765    if m.get('Page
-00028d70: 5369 7a65 2729 2069 7320 6e6f 7420 4e6f  Size') is not No
-00028d80: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00028d90: 7365 6c66 2e70 6167 655f 7369 7a65 203d  self.page_size =
-00028da0: 206d 2e67 6574 2827 5061 6765 5369 7a65   m.get('PageSize
-00028db0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-00028dc0: 6765 7428 2750 6970 656c 696e 6549 6427  get('PipelineId'
-00028dd0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-00028de0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00028df0: 7069 7065 6c69 6e65 5f69 6420 3d20 6d2e  pipeline_id = m.
-00028e00: 6765 7428 2750 6970 656c 696e 6549 6427  get('PipelineId'
-00028e10: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-00028e20: 6574 2827 5265 736f 7572 6365 4964 2729  et('ResourceId')
-00028e30: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00028e40: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-00028e50: 6573 6f75 7263 655f 6964 203d 206d 2e67  esource_id = m.g
-00028e60: 6574 2827 5265 736f 7572 6365 4964 2729  et('ResourceId')
-00028e70: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-00028e80: 7428 2753 686f 774f 776e 2729 2069 7320  t('ShowOwn') is 
-00028e90: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00028ea0: 2020 2020 2020 7365 6c66 2e73 686f 775f        self.show_
-00028eb0: 6f77 6e20 3d20 6d2e 6765 7428 2753 686f  own = m.get('Sho
-00028ec0: 774f 776e 2729 0a20 2020 2020 2020 2069  wOwn').        i
-00028ed0: 6620 6d2e 6765 7428 2753 6f72 7442 7927  f m.get('SortBy'
-00028ee0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-00028ef0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00028f00: 736f 7274 5f62 7920 3d20 6d2e 6765 7428  sort_by = m.get(
-00028f10: 2753 6f72 7442 7927 290a 2020 2020 2020  'SortBy').      
-00028f20: 2020 6966 206d 2e67 6574 2827 5374 6172    if m.get('Star
-00028f30: 7454 696d 6527 2920 6973 206e 6f74 204e  tTime') is not N
-00028f40: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00028f50: 2073 656c 662e 7374 6172 745f 7469 6d65   self.start_time
-00028f60: 203d 206d 2e67 6574 2827 5374 6172 7454   = m.get('StartT
-00028f70: 696d 6527 290a 2020 2020 2020 2020 6966  ime').        if
-00028f80: 206d 2e67 6574 2827 5374 6174 7573 2729   m.get('Status')
-00028f90: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00028fa0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-00028fb0: 7461 7475 7320 3d20 6d2e 6765 7428 2753  tatus = m.get('S
-00028fc0: 7461 7475 7327 290a 2020 2020 2020 2020  tatus').        
-00028fd0: 6966 206d 2e67 6574 2827 5461 6773 2729  if m.get('Tags')
-00028fe0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00028ff0: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
-00029000: 6167 7320 3d20 6d2e 6765 7428 2754 6167  ags = m.get('Tag
-00029010: 7327 290a 2020 2020 2020 2020 6966 206d  s').        if m
-00029020: 2e67 6574 2827 576f 726b 7370 6163 6549  .get('WorkspaceI
-00029030: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
-00029040: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00029050: 662e 776f 726b 7370 6163 655f 6964 203d  f.workspace_id =
-00029060: 206d 2e67 6574 2827 576f 726b 7370 6163   m.get('Workspac
-00029070: 6549 6427 290a 2020 2020 2020 2020 7265  eId').        re
-00029080: 7475 726e 2073 656c 660a 0a0a 636c 6173  turn self...clas
-00029090: 7320 4c69 7374 4a6f 6273 5368 7269 6e6b  s ListJobsShrink
-000290a0: 5265 7175 6573 7428 5465 614d 6f64 656c  Request(TeaModel
-000290b0: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
-000290c0: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
-000290d0: 662c 0a20 2020 2020 2020 2062 7573 696e  f,.        busin
-000290e0: 6573 735f 7573 6572 5f69 643a 2073 7472  ess_user_id: str
-000290f0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00029100: 2063 616c 6c65 723a 2073 7472 203d 204e   caller: str = N
-00029110: 6f6e 652c 0a20 2020 2020 2020 2064 6973  one,.        dis
-00029120: 706c 6179 5f6e 616d 653a 2073 7472 203d  play_name: str =
-00029130: 204e 6f6e 652c 0a20 2020 2020 2020 2065   None,.        e
-00029140: 6e64 5f74 696d 653a 2073 7472 203d 204e  nd_time: str = N
-00029150: 6f6e 652c 0a20 2020 2020 2020 2066 726f  one,.        fro
-00029160: 6d5f 616c 6c5f 776f 726b 7370 6163 6573  m_all_workspaces
-00029170: 3a20 626f 6f6c 203d 204e 6f6e 652c 0a20  : bool = None,. 
-00029180: 2020 2020 2020 206a 6f62 5f69 643a 2073         job_id: s
-00029190: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
-000291a0: 2020 206a 6f62 5f74 7970 653a 2073 7472     job_type: str
-000291b0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-000291c0: 206f 7264 6572 3a20 7374 7220 3d20 4e6f   order: str = No
-000291d0: 6e65 2c0a 2020 2020 2020 2020 7061 6765  ne,.        page
-000291e0: 5f6e 756d 6265 723a 2069 6e74 203d 204e  _number: int = N
-000291f0: 6f6e 652c 0a20 2020 2020 2020 2070 6167  one,.        pag
-00029200: 655f 7369 7a65 3a20 696e 7420 3d20 4e6f  e_size: int = No
-00029210: 6e65 2c0a 2020 2020 2020 2020 7069 7065  ne,.        pipe
-00029220: 6c69 6e65 5f69 643a 2073 7472 203d 204e  line_id: str = N
-00029230: 6f6e 652c 0a20 2020 2020 2020 2072 6573  one,.        res
-00029240: 6f75 7263 655f 6964 3a20 7374 7220 3d20  ource_id: str = 
-00029250: 4e6f 6e65 2c0a 2020 2020 2020 2020 7368  None,.        sh
-00029260: 6f77 5f6f 776e 3a20 626f 6f6c 203d 204e  ow_own: bool = N
-00029270: 6f6e 652c 0a20 2020 2020 2020 2073 6f72  one,.        sor
-00029280: 745f 6279 3a20 7374 7220 3d20 4e6f 6e65  t_by: str = None
-00029290: 2c0a 2020 2020 2020 2020 7374 6172 745f  ,.        start_
-000292a0: 7469 6d65 3a20 7374 7220 3d20 4e6f 6e65  time: str = None
-000292b0: 2c0a 2020 2020 2020 2020 7374 6174 7573  ,.        status
-000292c0: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
-000292d0: 2020 2020 2020 7461 6773 5f73 6872 696e        tags_shrin
-000292e0: 6b3a 2073 7472 203d 204e 6f6e 652c 0a20  k: str = None,. 
-000292f0: 2020 2020 2020 2077 6f72 6b73 7061 6365         workspace
-00029300: 5f69 643a 2073 7472 203d 204e 6f6e 652c  _id: str = None,
-00029310: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
-00029320: 7365 6c66 2e62 7573 696e 6573 735f 7573  self.business_us
-00029330: 6572 5f69 6420 3d20 6275 7369 6e65 7373  er_id = business
-00029340: 5f75 7365 725f 6964 0a20 2020 2020 2020  _user_id.       
-00029350: 2073 656c 662e 6361 6c6c 6572 203d 2063   self.caller = c
-00029360: 616c 6c65 720a 2020 2020 2020 2020 7365  aller.        se
-00029370: 6c66 2e64 6973 706c 6179 5f6e 616d 6520  lf.display_name 
-00029380: 3d20 6469 7370 6c61 795f 6e61 6d65 0a20  = display_name. 
-00029390: 2020 2020 2020 2073 656c 662e 656e 645f         self.end_
-000293a0: 7469 6d65 203d 2065 6e64 5f74 696d 650a  time = end_time.
-000293b0: 2020 2020 2020 2020 7365 6c66 2e66 726f          self.fro
-000293c0: 6d5f 616c 6c5f 776f 726b 7370 6163 6573  m_all_workspaces
-000293d0: 203d 2066 726f 6d5f 616c 6c5f 776f 726b   = from_all_work
-000293e0: 7370 6163 6573 0a20 2020 2020 2020 2073  spaces.        s
-000293f0: 656c 662e 6a6f 625f 6964 203d 206a 6f62  elf.job_id = job
-00029400: 5f69 640a 2020 2020 2020 2020 7365 6c66  _id.        self
-00029410: 2e6a 6f62 5f74 7970 6520 3d20 6a6f 625f  .job_type = job_
-00029420: 7479 7065 0a20 2020 2020 2020 2073 656c  type.        sel
-00029430: 662e 6f72 6465 7220 3d20 6f72 6465 720a  f.order = order.
-00029440: 2020 2020 2020 2020 7365 6c66 2e70 6167          self.pag
-00029450: 655f 6e75 6d62 6572 203d 2070 6167 655f  e_number = page_
-00029460: 6e75 6d62 6572 0a20 2020 2020 2020 2073  number.        s
-00029470: 656c 662e 7061 6765 5f73 697a 6520 3d20  elf.page_size = 
-00029480: 7061 6765 5f73 697a 650a 2020 2020 2020  page_size.      
-00029490: 2020 7365 6c66 2e70 6970 656c 696e 655f    self.pipeline_
-000294a0: 6964 203d 2070 6970 656c 696e 655f 6964  id = pipeline_id
-000294b0: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
-000294c0: 736f 7572 6365 5f69 6420 3d20 7265 736f  source_id = reso
-000294d0: 7572 6365 5f69 640a 2020 2020 2020 2020  urce_id.        
-000294e0: 7365 6c66 2e73 686f 775f 6f77 6e20 3d20  self.show_own = 
-000294f0: 7368 6f77 5f6f 776e 0a20 2020 2020 2020  show_own.       
-00029500: 2073 656c 662e 736f 7274 5f62 7920 3d20   self.sort_by = 
-00029510: 736f 7274 5f62 790a 2020 2020 2020 2020  sort_by.        
-00029520: 7365 6c66 2e73 7461 7274 5f74 696d 6520  self.start_time 
-00029530: 3d20 7374 6172 745f 7469 6d65 0a20 2020  = start_time.   
-00029540: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
-00029550: 203d 2073 7461 7475 730a 2020 2020 2020   = status.      
-00029560: 2020 7365 6c66 2e74 6167 735f 7368 7269    self.tags_shri
-00029570: 6e6b 203d 2074 6167 735f 7368 7269 6e6b  nk = tags_shrink
-00029580: 0a20 2020 2020 2020 2073 656c 662e 776f  .        self.wo
-00029590: 726b 7370 6163 655f 6964 203d 2077 6f72  rkspace_id = wor
-000295a0: 6b73 7061 6365 5f69 640a 0a20 2020 2064  kspace_id..    d
-000295b0: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
-000295c0: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
-000295d0: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
-000295e0: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
-000295f0: 6d61 7020 3d20 7375 7065 7228 292e 746f  map = super().to
-00029600: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
-00029610: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
-00029620: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00029630: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
-00029640: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
-00029650: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
-00029660: 7365 6c66 2e62 7573 696e 6573 735f 7573  self.business_us
-00029670: 6572 5f69 6420 6973 206e 6f74 204e 6f6e  er_id is not Non
-00029680: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00029690: 6573 756c 745b 2742 7573 696e 6573 7355  esult['BusinessU
-000296a0: 7365 7249 6427 5d20 3d20 7365 6c66 2e62  serId'] = self.b
-000296b0: 7573 696e 6573 735f 7573 6572 5f69 640a  usiness_user_id.
-000296c0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000296d0: 6361 6c6c 6572 2069 7320 6e6f 7420 4e6f  caller is not No
-000296e0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000296f0: 7265 7375 6c74 5b27 4361 6c6c 6572 275d  result['Caller']
-00029700: 203d 2073 656c 662e 6361 6c6c 6572 0a20   = self.caller. 
-00029710: 2020 2020 2020 2069 6620 7365 6c66 2e64         if self.d
-00029720: 6973 706c 6179 5f6e 616d 6520 6973 206e  isplay_name is n
-00029730: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00029740: 2020 2020 2072 6573 756c 745b 2744 6973       result['Dis
-00029750: 706c 6179 4e61 6d65 275d 203d 2073 656c  playName'] = sel
-00029760: 662e 6469 7370 6c61 795f 6e61 6d65 0a20  f.display_name. 
-00029770: 2020 2020 2020 2069 6620 7365 6c66 2e65         if self.e
-00029780: 6e64 5f74 696d 6520 6973 206e 6f74 204e  nd_time is not N
-00029790: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000297a0: 2072 6573 756c 745b 2745 6e64 5469 6d65   result['EndTime
-000297b0: 275d 203d 2073 656c 662e 656e 645f 7469  '] = self.end_ti
-000297c0: 6d65 0a20 2020 2020 2020 2069 6620 7365  me.        if se
-000297d0: 6c66 2e66 726f 6d5f 616c 6c5f 776f 726b  lf.from_all_work
-000297e0: 7370 6163 6573 2069 7320 6e6f 7420 4e6f  spaces is not No
-000297f0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00029800: 7265 7375 6c74 5b27 4672 6f6d 416c 6c57  result['FromAllW
-00029810: 6f72 6b73 7061 6365 7327 5d20 3d20 7365  orkspaces'] = se
-00029820: 6c66 2e66 726f 6d5f 616c 6c5f 776f 726b  lf.from_all_work
-00029830: 7370 6163 6573 0a20 2020 2020 2020 2069  spaces.        i
-00029840: 6620 7365 6c66 2e6a 6f62 5f69 6420 6973  f self.job_id is
-00029850: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00029860: 2020 2020 2020 2072 6573 756c 745b 274a         result['J
-00029870: 6f62 4964 275d 203d 2073 656c 662e 6a6f  obId'] = self.jo
-00029880: 625f 6964 0a20 2020 2020 2020 2069 6620  b_id.        if 
-00029890: 7365 6c66 2e6a 6f62 5f74 7970 6520 6973  self.job_type is
-000298a0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000298b0: 2020 2020 2020 2072 6573 756c 745b 274a         result['J
-000298c0: 6f62 5479 7065 275d 203d 2073 656c 662e  obType'] = self.
-000298d0: 6a6f 625f 7479 7065 0a20 2020 2020 2020  job_type.       
-000298e0: 2069 6620 7365 6c66 2e6f 7264 6572 2069   if self.order i
-000298f0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00029900: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-00029910: 4f72 6465 7227 5d20 3d20 7365 6c66 2e6f  Order'] = self.o
-00029920: 7264 6572 0a20 2020 2020 2020 2069 6620  rder.        if 
-00029930: 7365 6c66 2e70 6167 655f 6e75 6d62 6572  self.page_number
-00029940: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00029950: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00029960: 5b27 5061 6765 4e75 6d62 6572 275d 203d  ['PageNumber'] =
-00029970: 2073 656c 662e 7061 6765 5f6e 756d 6265   self.page_numbe
-00029980: 720a 2020 2020 2020 2020 6966 2073 656c  r.        if sel
-00029990: 662e 7061 6765 5f73 697a 6520 6973 206e  f.page_size is n
-000299a0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000299b0: 2020 2020 2072 6573 756c 745b 2750 6167       result['Pag
-000299c0: 6553 697a 6527 5d20 3d20 7365 6c66 2e70  eSize'] = self.p
-000299d0: 6167 655f 7369 7a65 0a20 2020 2020 2020  age_size.       
-000299e0: 2069 6620 7365 6c66 2e70 6970 656c 696e   if self.pipelin
-000299f0: 655f 6964 2069 7320 6e6f 7420 4e6f 6e65  e_id is not None
-00029a00: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00029a10: 7375 6c74 5b27 5069 7065 6c69 6e65 4964  sult['PipelineId
-00029a20: 275d 203d 2073 656c 662e 7069 7065 6c69  '] = self.pipeli
-00029a30: 6e65 5f69 640a 2020 2020 2020 2020 6966  ne_id.        if
-00029a40: 2073 656c 662e 7265 736f 7572 6365 5f69   self.resource_i
-00029a50: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
-00029a60: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00029a70: 745b 2752 6573 6f75 7263 6549 6427 5d20  t['ResourceId'] 
-00029a80: 3d20 7365 6c66 2e72 6573 6f75 7263 655f  = self.resource_
-00029a90: 6964 0a20 2020 2020 2020 2069 6620 7365  id.        if se
-00029aa0: 6c66 2e73 686f 775f 6f77 6e20 6973 206e  lf.show_own is n
-00029ab0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00029ac0: 2020 2020 2072 6573 756c 745b 2753 686f       result['Sho
-00029ad0: 774f 776e 275d 203d 2073 656c 662e 7368  wOwn'] = self.sh
-00029ae0: 6f77 5f6f 776e 0a20 2020 2020 2020 2069  ow_own.        i
-00029af0: 6620 7365 6c66 2e73 6f72 745f 6279 2069  f self.sort_by i
-00029b00: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00029b10: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-00029b20: 536f 7274 4279 275d 203d 2073 656c 662e  SortBy'] = self.
-00029b30: 736f 7274 5f62 790a 2020 2020 2020 2020  sort_by.        
-00029b40: 6966 2073 656c 662e 7374 6172 745f 7469  if self.start_ti
-00029b50: 6d65 2069 7320 6e6f 7420 4e6f 6e65 3a0a  me is not None:.
-00029b60: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00029b70: 6c74 5b27 5374 6172 7454 696d 6527 5d20  lt['StartTime'] 
-00029b80: 3d20 7365 6c66 2e73 7461 7274 5f74 696d  = self.start_tim
-00029b90: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
-00029ba0: 662e 7374 6174 7573 2069 7320 6e6f 7420  f.status is not 
-00029bb0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00029bc0: 2020 7265 7375 6c74 5b27 5374 6174 7573    result['Status
-00029bd0: 275d 203d 2073 656c 662e 7374 6174 7573  '] = self.status
-00029be0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00029bf0: 2e74 6167 735f 7368 7269 6e6b 2069 7320  .tags_shrink is 
-00029c00: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00029c10: 2020 2020 2020 7265 7375 6c74 5b27 5461        result['Ta
-00029c20: 6773 275d 203d 2073 656c 662e 7461 6773  gs'] = self.tags
-00029c30: 5f73 6872 696e 6b0a 2020 2020 2020 2020  _shrink.        
-00029c40: 6966 2073 656c 662e 776f 726b 7370 6163  if self.workspac
-00029c50: 655f 6964 2069 7320 6e6f 7420 4e6f 6e65  e_id is not None
-00029c60: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00029c70: 7375 6c74 5b27 576f 726b 7370 6163 6549  sult['WorkspaceI
-00029c80: 6427 5d20 3d20 7365 6c66 2e77 6f72 6b73  d'] = self.works
-00029c90: 7061 6365 5f69 640a 2020 2020 2020 2020  pace_id.        
-00029ca0: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
-00029cb0: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
-00029cc0: 7365 6c66 2c20 6d3a 2064 6963 7420 3d20  self, m: dict = 
-00029cd0: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
-00029ce0: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
-00029cf0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-00029d00: 2742 7573 696e 6573 7355 7365 7249 6427  'BusinessUserId'
-00029d10: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-00029d20: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00029d30: 6275 7369 6e65 7373 5f75 7365 725f 6964  business_user_id
-00029d40: 203d 206d 2e67 6574 2827 4275 7369 6e65   = m.get('Busine
-00029d50: 7373 5573 6572 4964 2729 0a20 2020 2020  ssUserId').     
-00029d60: 2020 2069 6620 6d2e 6765 7428 2743 616c     if m.get('Cal
-00029d70: 6c65 7227 2920 6973 206e 6f74 204e 6f6e  ler') is not Non
-00029d80: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00029d90: 656c 662e 6361 6c6c 6572 203d 206d 2e67  elf.caller = m.g
-00029da0: 6574 2827 4361 6c6c 6572 2729 0a20 2020  et('Caller').   
-00029db0: 2020 2020 2069 6620 6d2e 6765 7428 2744       if m.get('D
-00029dc0: 6973 706c 6179 4e61 6d65 2729 2069 7320  isplayName') is 
-00029dd0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00029de0: 2020 2020 2020 7365 6c66 2e64 6973 706c        self.displ
-00029df0: 6179 5f6e 616d 6520 3d20 6d2e 6765 7428  ay_name = m.get(
-00029e00: 2744 6973 706c 6179 4e61 6d65 2729 0a20  'DisplayName'). 
-00029e10: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-00029e20: 2745 6e64 5469 6d65 2729 2069 7320 6e6f  'EndTime') is no
-00029e30: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00029e40: 2020 2020 7365 6c66 2e65 6e64 5f74 696d      self.end_tim
-00029e50: 6520 3d20 6d2e 6765 7428 2745 6e64 5469  e = m.get('EndTi
-00029e60: 6d65 2729 0a20 2020 2020 2020 2069 6620  me').        if 
-00029e70: 6d2e 6765 7428 2746 726f 6d41 6c6c 576f  m.get('FromAllWo
-00029e80: 726b 7370 6163 6573 2729 2069 7320 6e6f  rkspaces') is no
-00029e90: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00029ea0: 2020 2020 7365 6c66 2e66 726f 6d5f 616c      self.from_al
-00029eb0: 6c5f 776f 726b 7370 6163 6573 203d 206d  l_workspaces = m
-00029ec0: 2e67 6574 2827 4672 6f6d 416c 6c57 6f72  .get('FromAllWor
-00029ed0: 6b73 7061 6365 7327 290a 2020 2020 2020  kspaces').      
-00029ee0: 2020 6966 206d 2e67 6574 2827 4a6f 6249    if m.get('JobI
-00029ef0: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
-00029f00: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00029f10: 662e 6a6f 625f 6964 203d 206d 2e67 6574  f.job_id = m.get
-00029f20: 2827 4a6f 6249 6427 290a 2020 2020 2020  ('JobId').      
-00029f30: 2020 6966 206d 2e67 6574 2827 4a6f 6254    if m.get('JobT
-00029f40: 7970 6527 2920 6973 206e 6f74 204e 6f6e  ype') is not Non
-00029f50: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00029f60: 656c 662e 6a6f 625f 7479 7065 203d 206d  elf.job_type = m
-00029f70: 2e67 6574 2827 4a6f 6254 7970 6527 290a  .get('JobType').
-00029f80: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-00029f90: 2827 4f72 6465 7227 2920 6973 206e 6f74  ('Order') is not
-00029fa0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00029fb0: 2020 2073 656c 662e 6f72 6465 7220 3d20     self.order = 
-00029fc0: 6d2e 6765 7428 274f 7264 6572 2729 0a20  m.get('Order'). 
-00029fd0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-00029fe0: 2750 6167 654e 756d 6265 7227 2920 6973  'PageNumber') is
-00029ff0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0002a000: 2020 2020 2020 2073 656c 662e 7061 6765         self.page
-0002a010: 5f6e 756d 6265 7220 3d20 6d2e 6765 7428  _number = m.get(
-0002a020: 2750 6167 654e 756d 6265 7227 290a 2020  'PageNumber').  
-0002a030: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-0002a040: 5061 6765 5369 7a65 2729 2069 7320 6e6f  PageSize') is no
-0002a050: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0002a060: 2020 2020 7365 6c66 2e70 6167 655f 7369      self.page_si
-0002a070: 7a65 203d 206d 2e67 6574 2827 5061 6765  ze = m.get('Page
-0002a080: 5369 7a65 2729 0a20 2020 2020 2020 2069  Size').        i
-0002a090: 6620 6d2e 6765 7428 2750 6970 656c 696e  f m.get('Pipelin
-0002a0a0: 6549 6427 2920 6973 206e 6f74 204e 6f6e  eId') is not Non
-0002a0b0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-0002a0c0: 656c 662e 7069 7065 6c69 6e65 5f69 6420  elf.pipeline_id 
-0002a0d0: 3d20 6d2e 6765 7428 2750 6970 656c 696e  = m.get('Pipelin
-0002a0e0: 6549 6427 290a 2020 2020 2020 2020 6966  eId').        if
-0002a0f0: 206d 2e67 6574 2827 5265 736f 7572 6365   m.get('Resource
-0002a100: 4964 2729 2069 7320 6e6f 7420 4e6f 6e65  Id') is not None
-0002a110: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0002a120: 6c66 2e72 6573 6f75 7263 655f 6964 203d  lf.resource_id =
-0002a130: 206d 2e67 6574 2827 5265 736f 7572 6365   m.get('Resource
-0002a140: 4964 2729 0a20 2020 2020 2020 2069 6620  Id').        if 
-0002a150: 6d2e 6765 7428 2753 686f 774f 776e 2729  m.get('ShowOwn')
-0002a160: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0002a170: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-0002a180: 686f 775f 6f77 6e20 3d20 6d2e 6765 7428  how_own = m.get(
-0002a190: 2753 686f 774f 776e 2729 0a20 2020 2020  'ShowOwn').     
-0002a1a0: 2020 2069 6620 6d2e 6765 7428 2753 6f72     if m.get('Sor
-0002a1b0: 7442 7927 2920 6973 206e 6f74 204e 6f6e  tBy') is not Non
-0002a1c0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-0002a1d0: 656c 662e 736f 7274 5f62 7920 3d20 6d2e  elf.sort_by = m.
-0002a1e0: 6765 7428 2753 6f72 7442 7927 290a 2020  get('SortBy').  
-0002a1f0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-0002a200: 5374 6172 7454 696d 6527 2920 6973 206e  StartTime') is n
-0002a210: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0002a220: 2020 2020 2073 656c 662e 7374 6172 745f       self.start_
-0002a230: 7469 6d65 203d 206d 2e67 6574 2827 5374  time = m.get('St
-0002a240: 6172 7454 696d 6527 290a 2020 2020 2020  artTime').      
-0002a250: 2020 6966 206d 2e67 6574 2827 5374 6174    if m.get('Stat
-0002a260: 7573 2729 2069 7320 6e6f 7420 4e6f 6e65  us') is not None
-0002a270: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0002a280: 6c66 2e73 7461 7475 7320 3d20 6d2e 6765  lf.status = m.ge
-0002a290: 7428 2753 7461 7475 7327 290a 2020 2020  t('Status').    
-0002a2a0: 2020 2020 6966 206d 2e67 6574 2827 5461      if m.get('Ta
-0002a2b0: 6773 2729 2069 7320 6e6f 7420 4e6f 6e65  gs') is not None
-0002a2c0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0002a2d0: 6c66 2e74 6167 735f 7368 7269 6e6b 203d  lf.tags_shrink =
-0002a2e0: 206d 2e67 6574 2827 5461 6773 2729 0a20   m.get('Tags'). 
-0002a2f0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-0002a300: 2757 6f72 6b73 7061 6365 4964 2729 2069  'WorkspaceId') i
-0002a310: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0002a320: 2020 2020 2020 2020 7365 6c66 2e77 6f72          self.wor
-0002a330: 6b73 7061 6365 5f69 6420 3d20 6d2e 6765  kspace_id = m.ge
-0002a340: 7428 2757 6f72 6b73 7061 6365 4964 2729  t('WorkspaceId')
-0002a350: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0002a360: 7365 6c66 0a0a 0a63 6c61 7373 204c 6973  self...class Lis
-0002a370: 744a 6f62 7352 6573 706f 6e73 6542 6f64  tJobsResponseBod
-0002a380: 7928 5465 614d 6f64 656c 293a 0a20 2020  y(TeaModel):.   
-0002a390: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
-0002a3a0: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-0002a3b0: 2020 2020 206a 6f62 733a 204c 6973 745b       jobs: List[
-0002a3c0: 4a6f 6249 7465 6d5d 203d 204e 6f6e 652c  JobItem] = None,
-0002a3d0: 0a20 2020 2020 2020 2072 6571 7565 7374  .        request
-0002a3e0: 5f69 643a 2073 7472 203d 204e 6f6e 652c  _id: str = None,
-0002a3f0: 0a20 2020 2020 2020 2074 6f74 616c 5f63  .        total_c
-0002a400: 6f75 6e74 3a20 696e 7420 3d20 4e6f 6e65  ount: int = None
-0002a410: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
-0002a420: 2073 656c 662e 6a6f 6273 203d 206a 6f62   self.jobs = job
-0002a430: 730a 2020 2020 2020 2020 7365 6c66 2e72  s.        self.r
-0002a440: 6571 7565 7374 5f69 6420 3d20 7265 7175  equest_id = requ
-0002a450: 6573 745f 6964 0a20 2020 2020 2020 2073  est_id.        s
-0002a460: 656c 662e 746f 7461 6c5f 636f 756e 7420  elf.total_count 
-0002a470: 3d20 746f 7461 6c5f 636f 756e 740a 0a20  = total_count.. 
-0002a480: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
-0002a490: 7365 6c66 293a 0a20 2020 2020 2020 2069  self):.        i
-0002a4a0: 6620 7365 6c66 2e6a 6f62 733a 0a20 2020  f self.jobs:.   
-0002a4b0: 2020 2020 2020 2020 2066 6f72 206b 2069           for k i
-0002a4c0: 6e20 7365 6c66 2e6a 6f62 733a 0a20 2020  n self.jobs:.   
-0002a4d0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0002a4e0: 6b3a 0a20 2020 2020 2020 2020 2020 2020  k:.             
-0002a4f0: 2020 2020 2020 206b 2e76 616c 6964 6174         k.validat
-0002a500: 6528 290a 0a20 2020 2064 6566 2074 6f5f  e()..    def to_
-0002a510: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
-0002a520: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
-0002a530: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
-0002a540: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
-0002a550: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0002a560: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
-0002a570: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
-0002a580: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
-0002a590: 2072 6573 756c 745b 274a 6f62 7327 5d20   result['Jobs'] 
-0002a5a0: 3d20 5b5d 0a20 2020 2020 2020 2069 6620  = [].        if 
-0002a5b0: 7365 6c66 2e6a 6f62 7320 6973 206e 6f74  self.jobs is not
-0002a5c0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0002a5d0: 2020 2066 6f72 206b 2069 6e20 7365 6c66     for k in self
-0002a5e0: 2e6a 6f62 733a 0a20 2020 2020 2020 2020  .jobs:.         
-0002a5f0: 2020 2020 2020 2072 6573 756c 745b 274a         result['J
-0002a600: 6f62 7327 5d2e 6170 7065 6e64 286b 2e74  obs'].append(k.t
-0002a610: 6f5f 6d61 7028 2920 6966 206b 2065 6c73  o_map() if k els
-0002a620: 6520 4e6f 6e65 290a 2020 2020 2020 2020  e None).        
-0002a630: 6966 2073 656c 662e 7265 7175 6573 745f  if self.request_
-0002a640: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
-0002a650: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-0002a660: 6c74 5b27 5265 7175 6573 7449 6427 5d20  lt['RequestId'] 
-0002a670: 3d20 7365 6c66 2e72 6571 7565 7374 5f69  = self.request_i
-0002a680: 640a 2020 2020 2020 2020 6966 2073 656c  d.        if sel
-0002a690: 662e 746f 7461 6c5f 636f 756e 7420 6973  f.total_count is
-0002a6a0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0002a6b0: 2020 2020 2020 2072 6573 756c 745b 2754         result['T
-0002a6c0: 6f74 616c 436f 756e 7427 5d20 3d20 7365  otalCount'] = se
-0002a6d0: 6c66 2e74 6f74 616c 5f63 6f75 6e74 0a20  lf.total_count. 
-0002a6e0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-0002a6f0: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
-0002a700: 6f6d 5f6d 6170 2873 656c 662c 206d 3a20  om_map(self, m: 
-0002a710: 6469 6374 203d 204e 6f6e 6529 3a0a 2020  dict = None):.  
-0002a720: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
-0002a730: 6963 7428 290a 2020 2020 2020 2020 7365  ict().        se
-0002a740: 6c66 2e6a 6f62 7320 3d20 5b5d 0a20 2020  lf.jobs = [].   
-0002a750: 2020 2020 2069 6620 6d2e 6765 7428 274a       if m.get('J
-0002a760: 6f62 7327 2920 6973 206e 6f74 204e 6f6e  obs') is not Non
-0002a770: 653a 0a20 2020 2020 2020 2020 2020 2066  e:.            f
-0002a780: 6f72 206b 2069 6e20 6d2e 6765 7428 274a  or k in m.get('J
-0002a790: 6f62 7327 293a 0a20 2020 2020 2020 2020  obs'):.         
-0002a7a0: 2020 2020 2020 2074 656d 705f 6d6f 6465         temp_mode
-0002a7b0: 6c20 3d20 4a6f 6249 7465 6d28 290a 2020  l = JobItem().  
-0002a7c0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0002a7d0: 6c66 2e6a 6f62 732e 6170 7065 6e64 2874  lf.jobs.append(t
-0002a7e0: 656d 705f 6d6f 6465 6c2e 6672 6f6d 5f6d  emp_model.from_m
-0002a7f0: 6170 286b 2929 0a20 2020 2020 2020 2069  ap(k)).        i
-0002a800: 6620 6d2e 6765 7428 2752 6571 7565 7374  f m.get('Request
-0002a810: 4964 2729 2069 7320 6e6f 7420 4e6f 6e65  Id') is not None
-0002a820: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0002a830: 6c66 2e72 6571 7565 7374 5f69 6420 3d20  lf.request_id = 
-0002a840: 6d2e 6765 7428 2752 6571 7565 7374 4964  m.get('RequestId
-0002a850: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-0002a860: 6765 7428 2754 6f74 616c 436f 756e 7427  get('TotalCount'
-0002a870: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-0002a880: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0002a890: 746f 7461 6c5f 636f 756e 7420 3d20 6d2e  total_count = m.
-0002a8a0: 6765 7428 2754 6f74 616c 436f 756e 7427  get('TotalCount'
-0002a8b0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-0002a8c0: 2073 656c 660a 0a0a 636c 6173 7320 4c69   self...class Li
-0002a8d0: 7374 4a6f 6273 5265 7370 6f6e 7365 2854  stJobsResponse(T
-0002a8e0: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
-0002a8f0: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
-0002a900: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-0002a910: 2020 6865 6164 6572 733a 2044 6963 745b    headers: Dict[
-0002a920: 7374 722c 2073 7472 5d20 3d20 4e6f 6e65  str, str] = None
-0002a930: 2c0a 2020 2020 2020 2020 7374 6174 7573  ,.        status
-0002a940: 5f63 6f64 653a 2069 6e74 203d 204e 6f6e  _code: int = Non
-0002a950: 652c 0a20 2020 2020 2020 2062 6f64 793a  e,.        body:
-0002a960: 204c 6973 744a 6f62 7352 6573 706f 6e73   ListJobsRespons
-0002a970: 6542 6f64 7920 3d20 4e6f 6e65 2c0a 2020  eBody = None,.  
-0002a980: 2020 293a 0a20 2020 2020 2020 2073 656c    ):.        sel
-0002a990: 662e 6865 6164 6572 7320 3d20 6865 6164  f.headers = head
-0002a9a0: 6572 730a 2020 2020 2020 2020 7365 6c66  ers.        self
-0002a9b0: 2e73 7461 7475 735f 636f 6465 203d 2073  .status_code = s
-0002a9c0: 7461 7475 735f 636f 6465 0a20 2020 2020  tatus_code.     
-0002a9d0: 2020 2073 656c 662e 626f 6479 203d 2062     self.body = b
-0002a9e0: 6f64 790a 0a20 2020 2064 6566 2076 616c  ody..    def val
-0002a9f0: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
-0002aa00: 2020 2020 2073 656c 662e 7661 6c69 6461       self.valida
-0002aa10: 7465 5f72 6571 7569 7265 6428 7365 6c66  te_required(self
-0002aa20: 2e68 6561 6465 7273 2c20 2768 6561 6465  .headers, 'heade
-0002aa30: 7273 2729 0a20 2020 2020 2020 2073 656c  rs').        sel
-0002aa40: 662e 7661 6c69 6461 7465 5f72 6571 7569  f.validate_requi
-0002aa50: 7265 6428 7365 6c66 2e73 7461 7475 735f  red(self.status_
-0002aa60: 636f 6465 2c20 2773 7461 7475 735f 636f  code, 'status_co
-0002aa70: 6465 2729 0a20 2020 2020 2020 2073 656c  de').        sel
-0002aa80: 662e 7661 6c69 6461 7465 5f72 6571 7569  f.validate_requi
-0002aa90: 7265 6428 7365 6c66 2e62 6f64 792c 2027  red(self.body, '
-0002aaa0: 626f 6479 2729 0a20 2020 2020 2020 2069  body').        i
-0002aab0: 6620 7365 6c66 2e62 6f64 793a 0a20 2020  f self.body:.   
-0002aac0: 2020 2020 2020 2020 2073 656c 662e 626f           self.bo
-0002aad0: 6479 2e76 616c 6964 6174 6528 290a 0a20  dy.validate().. 
-0002aae0: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
-0002aaf0: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
-0002ab00: 7020 3d20 7375 7065 7228 292e 746f 5f6d  p = super().to_m
-0002ab10: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
-0002ab20: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
-0002ab30: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0002ab40: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
-0002ab50: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
-0002ab60: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
-0002ab70: 6c66 2e68 6561 6465 7273 2069 7320 6e6f  lf.headers is no
-0002ab80: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0002ab90: 2020 2020 7265 7375 6c74 5b27 6865 6164      result['head
-0002aba0: 6572 7327 5d20 3d20 7365 6c66 2e68 6561  ers'] = self.hea
-0002abb0: 6465 7273 0a20 2020 2020 2020 2069 6620  ders.        if 
-0002abc0: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
-0002abd0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0002abe0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0002abf0: 5b27 7374 6174 7573 436f 6465 275d 203d  ['statusCode'] =
-0002ac00: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
-0002ac10: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
-0002ac20: 662e 626f 6479 2069 7320 6e6f 7420 4e6f  f.body is not No
-0002ac30: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0002ac40: 7265 7375 6c74 5b27 626f 6479 275d 203d  result['body'] =
-0002ac50: 2073 656c 662e 626f 6479 2e74 6f5f 6d61   self.body.to_ma
-0002ac60: 7028 290a 2020 2020 2020 2020 7265 7475  p().        retu
-0002ac70: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
-0002ac80: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
-0002ac90: 2c20 6d3a 2064 6963 7420 3d20 4e6f 6e65  , m: dict = None
-0002aca0: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
-0002acb0: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
-0002acc0: 2020 2069 6620 6d2e 6765 7428 2768 6561     if m.get('hea
-0002acd0: 6465 7273 2729 2069 7320 6e6f 7420 4e6f  ders') is not No
-0002ace0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0002acf0: 7365 6c66 2e68 6561 6465 7273 203d 206d  self.headers = m
-0002ad00: 2e67 6574 2827 6865 6164 6572 7327 290a  .get('headers').
-0002ad10: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-0002ad20: 2827 7374 6174 7573 436f 6465 2729 2069  ('statusCode') i
-0002ad30: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0002ad40: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
-0002ad50: 7475 735f 636f 6465 203d 206d 2e67 6574  tus_code = m.get
-0002ad60: 2827 7374 6174 7573 436f 6465 2729 0a20  ('statusCode'). 
-0002ad70: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-0002ad80: 2762 6f64 7927 2920 6973 206e 6f74 204e  'body') is not N
-0002ad90: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0002ada0: 2074 656d 705f 6d6f 6465 6c20 3d20 4c69   temp_model = Li
-0002adb0: 7374 4a6f 6273 5265 7370 6f6e 7365 426f  stJobsResponseBo
-0002adc0: 6479 2829 0a20 2020 2020 2020 2020 2020  dy().           
-0002add0: 2073 656c 662e 626f 6479 203d 2074 656d   self.body = tem
-0002ade0: 705f 6d6f 6465 6c2e 6672 6f6d 5f6d 6170  p_model.from_map
-0002adf0: 286d 5b27 626f 6479 275d 290a 2020 2020  (m['body']).    
-0002ae00: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
-0002ae10: 0a0a 636c 6173 7320 4c69 7374 5465 6e73  ..class ListTens
-0002ae20: 6f72 626f 6172 6473 5265 7175 6573 7428  orboardsRequest(
-0002ae30: 5465 614d 6f64 656c 293a 0a20 2020 2064  TeaModel):.    d
-0002ae40: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
-0002ae50: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
-0002ae60: 2020 2064 6973 706c 6179 5f6e 616d 653a     display_name:
-0002ae70: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
-0002ae80: 2020 2020 2065 6e64 5f74 696d 653a 2073       end_time: s
-0002ae90: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
-0002aea0: 2020 206a 6f62 5f69 643a 2073 7472 203d     job_id: str =
-0002aeb0: 204e 6f6e 652c 0a20 2020 2020 2020 206f   None,.        o
-0002aec0: 7264 6572 3a20 7374 7220 3d20 4e6f 6e65  rder: str = None
-0002aed0: 2c0a 2020 2020 2020 2020 7061 6765 5f6e  ,.        page_n
-0002aee0: 756d 6265 723a 2069 6e74 203d 204e 6f6e  umber: int = Non
-0002aef0: 652c 0a20 2020 2020 2020 2070 6167 655f  e,.        page_
-0002af00: 7369 7a65 3a20 696e 7420 3d20 4e6f 6e65  size: int = None
-0002af10: 2c0a 2020 2020 2020 2020 736f 7274 5f62  ,.        sort_b
-0002af20: 793a 2073 7472 203d 204e 6f6e 652c 0a20  y: str = None,. 
-0002af30: 2020 2020 2020 2073 6f75 7263 655f 6964         source_id
-0002af40: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
-0002af50: 2020 2020 2020 736f 7572 6365 5f74 7970        source_typ
-0002af60: 653a 2073 7472 203d 204e 6f6e 652c 0a20  e: str = None,. 
-0002af70: 2020 2020 2020 2073 7461 7274 5f74 696d         start_tim
-0002af80: 653a 2073 7472 203d 204e 6f6e 652c 0a20  e: str = None,. 
-0002af90: 2020 2020 2020 2073 7461 7475 733a 2073         status: s
-0002afa0: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
-0002afb0: 2020 2074 656e 736f 7262 6f61 7264 5f69     tensorboard_i
-0002afc0: 643a 2073 7472 203d 204e 6f6e 652c 0a20  d: str = None,. 
-0002afd0: 2020 2020 2020 2076 6572 626f 7365 3a20         verbose: 
-0002afe0: 626f 6f6c 203d 204e 6f6e 652c 0a20 2020  bool = None,.   
-0002aff0: 2020 2020 2077 6f72 6b73 7061 6365 5f69       workspace_i
-0002b000: 643a 2073 7472 203d 204e 6f6e 652c 0a20  d: str = None,. 
-0002b010: 2020 2029 3a0a 2020 2020 2020 2020 7365     ):.        se
-0002b020: 6c66 2e64 6973 706c 6179 5f6e 616d 6520  lf.display_name 
-0002b030: 3d20 6469 7370 6c61 795f 6e61 6d65 0a20  = display_name. 
-0002b040: 2020 2020 2020 2073 656c 662e 656e 645f         self.end_
-0002b050: 7469 6d65 203d 2065 6e64 5f74 696d 650a  time = end_time.
-0002b060: 2020 2020 2020 2020 7365 6c66 2e6a 6f62          self.job
-0002b070: 5f69 6420 3d20 6a6f 625f 6964 0a20 2020  _id = job_id.   
-0002b080: 2020 2020 2073 656c 662e 6f72 6465 7220       self.order 
-0002b090: 3d20 6f72 6465 720a 2020 2020 2020 2020  = order.        
-0002b0a0: 7365 6c66 2e70 6167 655f 6e75 6d62 6572  self.page_number
-0002b0b0: 203d 2070 6167 655f 6e75 6d62 6572 0a20   = page_number. 
-0002b0c0: 2020 2020 2020 2073 656c 662e 7061 6765         self.page
-0002b0d0: 5f73 697a 6520 3d20 7061 6765 5f73 697a  _size = page_siz
-0002b0e0: 650a 2020 2020 2020 2020 7365 6c66 2e73  e.        self.s
-0002b0f0: 6f72 745f 6279 203d 2073 6f72 745f 6279  ort_by = sort_by
-0002b100: 0a20 2020 2020 2020 2073 656c 662e 736f  .        self.so
-0002b110: 7572 6365 5f69 6420 3d20 736f 7572 6365  urce_id = source
-0002b120: 5f69 640a 2020 2020 2020 2020 7365 6c66  _id.        self
-0002b130: 2e73 6f75 7263 655f 7479 7065 203d 2073  .source_type = s
-0002b140: 6f75 7263 655f 7479 7065 0a20 2020 2020  ource_type.     
-0002b150: 2020 2073 656c 662e 7374 6172 745f 7469     self.start_ti
-0002b160: 6d65 203d 2073 7461 7274 5f74 696d 650a  me = start_time.
-0002b170: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
-0002b180: 7475 7320 3d20 7374 6174 7573 0a20 2020  tus = status.   
-0002b190: 2020 2020 2073 656c 662e 7465 6e73 6f72       self.tensor
-0002b1a0: 626f 6172 645f 6964 203d 2074 656e 736f  board_id = tenso
-0002b1b0: 7262 6f61 7264 5f69 640a 2020 2020 2020  rboard_id.      
-0002b1c0: 2020 7365 6c66 2e76 6572 626f 7365 203d    self.verbose =
-0002b1d0: 2076 6572 626f 7365 0a20 2020 2020 2020   verbose.       
-0002b1e0: 2073 656c 662e 776f 726b 7370 6163 655f   self.workspace_
-0002b1f0: 6964 203d 2077 6f72 6b73 7061 6365 5f69  id = workspace_i
-0002b200: 640a 0a20 2020 2064 6566 2076 616c 6964  d..    def valid
-0002b210: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
-0002b220: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
-0002b230: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
-0002b240: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
-0002b250: 7065 7228 292e 746f 5f6d 6170 2829 0a20  per().to_map(). 
-0002b260: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
-0002b270: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0002b280: 2020 2020 2020 2020 7265 7475 726e 205f          return _
-0002b290: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
-0002b2a0: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
-0002b2b0: 2020 2020 2069 6620 7365 6c66 2e64 6973       if self.dis
-0002b2c0: 706c 6179 5f6e 616d 6520 6973 206e 6f74  play_name is not
-0002b2d0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0002b2e0: 2020 2072 6573 756c 745b 2744 6973 706c     result['Displ
-0002b2f0: 6179 4e61 6d65 275d 203d 2073 656c 662e  ayName'] = self.
-0002b300: 6469 7370 6c61 795f 6e61 6d65 0a20 2020  display_name.   
-0002b310: 2020 2020 2069 6620 7365 6c66 2e65 6e64       if self.end
-0002b320: 5f74 696d 6520 6973 206e 6f74 204e 6f6e  _time is not Non
-0002b330: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-0002b340: 6573 756c 745b 2745 6e64 5469 6d65 275d  esult['EndTime']
-0002b350: 203d 2073 656c 662e 656e 645f 7469 6d65   = self.end_time
-0002b360: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0002b370: 2e6a 6f62 5f69 6420 6973 206e 6f74 204e  .job_id is not N
-0002b380: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0002b390: 2072 6573 756c 745b 274a 6f62 4964 275d   result['JobId']
-0002b3a0: 203d 2073 656c 662e 6a6f 625f 6964 0a20   = self.job_id. 
-0002b3b0: 2020 2020 2020 2069 6620 7365 6c66 2e6f         if self.o
-0002b3c0: 7264 6572 2069 7320 6e6f 7420 4e6f 6e65  rder is not None
-0002b3d0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0002b3e0: 7375 6c74 5b27 4f72 6465 7227 5d20 3d20  sult['Order'] = 
-0002b3f0: 7365 6c66 2e6f 7264 6572 0a20 2020 2020  self.order.     
-0002b400: 2020 2069 6620 7365 6c66 2e70 6167 655f     if self.page_
-0002b410: 6e75 6d62 6572 2069 7320 6e6f 7420 4e6f  number is not No
-0002b420: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0002b430: 7265 7375 6c74 5b27 5061 6765 4e75 6d62  result['PageNumb
-0002b440: 6572 275d 203d 2073 656c 662e 7061 6765  er'] = self.page
-0002b450: 5f6e 756d 6265 720a 2020 2020 2020 2020  _number.        
-0002b460: 6966 2073 656c 662e 7061 6765 5f73 697a  if self.page_siz
-0002b470: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
-0002b480: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-0002b490: 745b 2750 6167 6553 697a 6527 5d20 3d20  t['PageSize'] = 
-0002b4a0: 7365 6c66 2e70 6167 655f 7369 7a65 0a20  self.page_size. 
-0002b4b0: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
-0002b4c0: 6f72 745f 6279 2069 7320 6e6f 7420 4e6f  ort_by is not No
-0002b4d0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0002b4e0: 7265 7375 6c74 5b27 536f 7274 4279 275d  result['SortBy']
-0002b4f0: 203d 2073 656c 662e 736f 7274 5f62 790a   = self.sort_by.
-0002b500: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0002b510: 736f 7572 6365 5f69 6420 6973 206e 6f74  source_id is not
-0002b520: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0002b530: 2020 2072 6573 756c 745b 2753 6f75 7263     result['Sourc
-0002b540: 6549 6427 5d20 3d20 7365 6c66 2e73 6f75  eId'] = self.sou
-0002b550: 7263 655f 6964 0a20 2020 2020 2020 2069  rce_id.        i
-0002b560: 6620 7365 6c66 2e73 6f75 7263 655f 7479  f self.source_ty
-0002b570: 7065 2069 7320 6e6f 7420 4e6f 6e65 3a0a  pe is not None:.
-0002b580: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-0002b590: 6c74 5b27 536f 7572 6365 5479 7065 275d  lt['SourceType']
-0002b5a0: 203d 2073 656c 662e 736f 7572 6365 5f74   = self.source_t
-0002b5b0: 7970 650a 2020 2020 2020 2020 6966 2073  ype.        if s
-0002b5c0: 656c 662e 7374 6172 745f 7469 6d65 2069  elf.start_time i
-0002b5d0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0002b5e0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-0002b5f0: 5374 6172 7454 696d 6527 5d20 3d20 7365  StartTime'] = se
-0002b600: 6c66 2e73 7461 7274 5f74 696d 650a 2020  lf.start_time.  
-0002b610: 2020 2020 2020 6966 2073 656c 662e 7374        if self.st
-0002b620: 6174 7573 2069 7320 6e6f 7420 4e6f 6e65  atus is not None
-0002b630: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0002b640: 7375 6c74 5b27 5374 6174 7573 275d 203d  sult['Status'] =
-0002b650: 2073 656c 662e 7374 6174 7573 0a20 2020   self.status.   
-0002b660: 2020 2020 2069 6620 7365 6c66 2e74 656e       if self.ten
-0002b670: 736f 7262 6f61 7264 5f69 6420 6973 206e  sorboard_id is n
-0002b680: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0002b690: 2020 2020 2072 6573 756c 745b 2754 656e       result['Ten
-0002b6a0: 736f 7262 6f61 7264 4964 275d 203d 2073  sorboardId'] = s
-0002b6b0: 656c 662e 7465 6e73 6f72 626f 6172 645f  elf.tensorboard_
-0002b6c0: 6964 0a20 2020 2020 2020 2069 6620 7365  id.        if se
-0002b6d0: 6c66 2e76 6572 626f 7365 2069 7320 6e6f  lf.verbose is no
-0002b6e0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0002b6f0: 2020 2020 7265 7375 6c74 5b27 5665 7262      result['Verb
-0002b700: 6f73 6527 5d20 3d20 7365 6c66 2e76 6572  ose'] = self.ver
-0002b710: 626f 7365 0a20 2020 2020 2020 2069 6620  bose.        if 
-0002b720: 7365 6c66 2e77 6f72 6b73 7061 6365 5f69  self.workspace_i
-0002b730: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
-0002b740: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-0002b750: 745b 2757 6f72 6b73 7061 6365 4964 275d  t['WorkspaceId']
-0002b760: 203d 2073 656c 662e 776f 726b 7370 6163   = self.workspac
-0002b770: 655f 6964 0a20 2020 2020 2020 2072 6574  e_id.        ret
-0002b780: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
-0002b790: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
-0002b7a0: 662c 206d 3a20 6469 6374 203d 204e 6f6e  f, m: dict = Non
-0002b7b0: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
-0002b7c0: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
-0002b7d0: 2020 2020 6966 206d 2e67 6574 2827 4469      if m.get('Di
-0002b7e0: 7370 6c61 794e 616d 6527 2920 6973 206e  splayName') is n
-0002b7f0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0002b800: 2020 2020 2073 656c 662e 6469 7370 6c61       self.displa
-0002b810: 795f 6e61 6d65 203d 206d 2e67 6574 2827  y_name = m.get('
-0002b820: 4469 7370 6c61 794e 616d 6527 290a 2020  DisplayName').  
-0002b830: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-0002b840: 456e 6454 696d 6527 2920 6973 206e 6f74  EndTime') is not
-0002b850: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0002b860: 2020 2073 656c 662e 656e 645f 7469 6d65     self.end_time
-0002b870: 203d 206d 2e67 6574 2827 456e 6454 696d   = m.get('EndTim
-0002b880: 6527 290a 2020 2020 2020 2020 6966 206d  e').        if m
-0002b890: 2e67 6574 2827 4a6f 6249 6427 2920 6973  .get('JobId') is
-0002b8a0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0002b8b0: 2020 2020 2020 2073 656c 662e 6a6f 625f         self.job_
-0002b8c0: 6964 203d 206d 2e67 6574 2827 4a6f 6249  id = m.get('JobI
-0002b8d0: 6427 290a 2020 2020 2020 2020 6966 206d  d').        if m
-0002b8e0: 2e67 6574 2827 4f72 6465 7227 2920 6973  .get('Order') is
-0002b8f0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0002b900: 2020 2020 2020 2073 656c 662e 6f72 6465         self.orde
-0002b910: 7220 3d20 6d2e 6765 7428 274f 7264 6572  r = m.get('Order
-0002b920: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-0002b930: 6765 7428 2750 6167 654e 756d 6265 7227  get('PageNumber'
-0002b940: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-0002b950: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0002b960: 7061 6765 5f6e 756d 6265 7220 3d20 6d2e  page_number = m.
-0002b970: 6765 7428 2750 6167 654e 756d 6265 7227  get('PageNumber'
-0002b980: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-0002b990: 6574 2827 5061 6765 5369 7a65 2729 2069  et('PageSize') i
-0002b9a0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0002b9b0: 2020 2020 2020 2020 7365 6c66 2e70 6167          self.pag
-0002b9c0: 655f 7369 7a65 203d 206d 2e67 6574 2827  e_size = m.get('
-0002b9d0: 5061 6765 5369 7a65 2729 0a20 2020 2020  PageSize').     
-0002b9e0: 2020 2069 6620 6d2e 6765 7428 2753 6f72     if m.get('Sor
-0002b9f0: 7442 7927 2920 6973 206e 6f74 204e 6f6e  tBy') is not Non
-0002ba00: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-0002ba10: 656c 662e 736f 7274 5f62 7920 3d20 6d2e  elf.sort_by = m.
-0002ba20: 6765 7428 2753 6f72 7442 7927 290a 2020  get('SortBy').  
-0002ba30: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-0002ba40: 536f 7572 6365 4964 2729 2069 7320 6e6f  SourceId') is no
-0002ba50: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0002ba60: 2020 2020 7365 6c66 2e73 6f75 7263 655f      self.source_
-0002ba70: 6964 203d 206d 2e67 6574 2827 536f 7572  id = m.get('Sour
-0002ba80: 6365 4964 2729 0a20 2020 2020 2020 2069  ceId').        i
-0002ba90: 6620 6d2e 6765 7428 2753 6f75 7263 6554  f m.get('SourceT
-0002baa0: 7970 6527 2920 6973 206e 6f74 204e 6f6e  ype') is not Non
-0002bab0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-0002bac0: 656c 662e 736f 7572 6365 5f74 7970 6520  elf.source_type 
-0002bad0: 3d20 6d2e 6765 7428 2753 6f75 7263 6554  = m.get('SourceT
-0002bae0: 7970 6527 290a 2020 2020 2020 2020 6966  ype').        if
-0002baf0: 206d 2e67 6574 2827 5374 6172 7454 696d   m.get('StartTim
-0002bb00: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
-0002bb10: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0002bb20: 662e 7374 6172 745f 7469 6d65 203d 206d  f.start_time = m
-0002bb30: 2e67 6574 2827 5374 6172 7454 696d 6527  .get('StartTime'
-0002bb40: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-0002bb50: 6574 2827 5374 6174 7573 2729 2069 7320  et('Status') is 
-0002bb60: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0002bb70: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
-0002bb80: 7320 3d20 6d2e 6765 7428 2753 7461 7475  s = m.get('Statu
-0002bb90: 7327 290a 2020 2020 2020 2020 6966 206d  s').        if m
-0002bba0: 2e67 6574 2827 5465 6e73 6f72 626f 6172  .get('Tensorboar
-0002bbb0: 6449 6427 2920 6973 206e 6f74 204e 6f6e  dId') is not Non
-0002bbc0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-0002bbd0: 656c 662e 7465 6e73 6f72 626f 6172 645f  elf.tensorboard_
-0002bbe0: 6964 203d 206d 2e67 6574 2827 5465 6e73  id = m.get('Tens
-0002bbf0: 6f72 626f 6172 6449 6427 290a 2020 2020  orboardId').    
-0002bc00: 2020 2020 6966 206d 2e67 6574 2827 5665      if m.get('Ve
-0002bc10: 7262 6f73 6527 2920 6973 206e 6f74 204e  rbose') is not N
-0002bc20: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0002bc30: 2073 656c 662e 7665 7262 6f73 6520 3d20   self.verbose = 
-0002bc40: 6d2e 6765 7428 2756 6572 626f 7365 2729  m.get('Verbose')
-0002bc50: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-0002bc60: 7428 2757 6f72 6b73 7061 6365 4964 2729  t('WorkspaceId')
-0002bc70: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0002bc80: 2020 2020 2020 2020 2020 7365 6c66 2e77            self.w
-0002bc90: 6f72 6b73 7061 6365 5f69 6420 3d20 6d2e  orkspace_id = m.
-0002bca0: 6765 7428 2757 6f72 6b73 7061 6365 4964  get('WorkspaceId
-0002bcb0: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
-0002bcc0: 6e20 7365 6c66 0a0a 0a63 6c61 7373 204c  n self...class L
-0002bcd0: 6973 7454 656e 736f 7262 6f61 7264 7352  istTensorboardsR
-0002bce0: 6573 706f 6e73 6542 6f64 7928 5465 614d  esponseBody(TeaM
-0002bcf0: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
-0002bd00: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
-0002bd10: 2073 656c 662c 0a20 2020 2020 2020 2072   self,.        r
-0002bd20: 6571 7565 7374 5f69 643a 2073 7472 203d  equest_id: str =
-0002bd30: 204e 6f6e 652c 0a20 2020 2020 2020 2074   None,.        t
-0002bd40: 656e 736f 7262 6f61 7264 733a 204c 6973  ensorboards: Lis
-0002bd50: 745b 5465 6e73 6f72 626f 6172 645d 203d  t[Tensorboard] =
-0002bd60: 204e 6f6e 652c 0a20 2020 2020 2020 2074   None,.        t
-0002bd70: 6f74 616c 5f63 6f75 6e74 3a20 696e 7420  otal_count: int 
-0002bd80: 3d20 4e6f 6e65 2c0a 2020 2020 293a 0a20  = None,.    ):. 
-0002bd90: 2020 2020 2020 2073 656c 662e 7265 7175         self.requ
-0002bda0: 6573 745f 6964 203d 2072 6571 7565 7374  est_id = request
-0002bdb0: 5f69 640a 2020 2020 2020 2020 7365 6c66  _id.        self
-0002bdc0: 2e74 656e 736f 7262 6f61 7264 7320 3d20  .tensorboards = 
-0002bdd0: 7465 6e73 6f72 626f 6172 6473 0a20 2020  tensorboards.   
-0002bde0: 2020 2020 2073 656c 662e 746f 7461 6c5f       self.total_
-0002bdf0: 636f 756e 7420 3d20 746f 7461 6c5f 636f  count = total_co
-0002be00: 756e 740a 0a20 2020 2064 6566 2076 616c  unt..    def val
-0002be10: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
-0002be20: 2020 2020 2069 6620 7365 6c66 2e74 656e       if self.ten
-0002be30: 736f 7262 6f61 7264 733a 0a20 2020 2020  sorboards:.     
-0002be40: 2020 2020 2020 2066 6f72 206b 2069 6e20         for k in 
-0002be50: 7365 6c66 2e74 656e 736f 7262 6f61 7264  self.tensorboard
-0002be60: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-0002be70: 2020 2069 6620 6b3a 0a20 2020 2020 2020     if k:.       
-0002be80: 2020 2020 2020 2020 2020 2020 206b 2e76               k.v
-0002be90: 616c 6964 6174 6528 290a 0a20 2020 2064  alidate()..    d
-0002bea0: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
-0002beb0: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
-0002bec0: 7375 7065 7228 292e 746f 5f6d 6170 2829  super().to_map()
-0002bed0: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
-0002bee0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0002bef0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0002bf00: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
-0002bf10: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
-0002bf20: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
-0002bf30: 6571 7565 7374 5f69 6420 6973 206e 6f74  equest_id is not
-0002bf40: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0002bf50: 2020 2072 6573 756c 745b 2752 6571 7565     result['Reque
-0002bf60: 7374 4964 275d 203d 2073 656c 662e 7265  stId'] = self.re
-0002bf70: 7175 6573 745f 6964 0a20 2020 2020 2020  quest_id.       
-0002bf80: 2072 6573 756c 745b 2754 656e 736f 7262   result['Tensorb
-0002bf90: 6f61 7264 7327 5d20 3d20 5b5d 0a20 2020  oards'] = [].   
-0002bfa0: 2020 2020 2069 6620 7365 6c66 2e74 656e       if self.ten
-0002bfb0: 736f 7262 6f61 7264 7320 6973 206e 6f74  sorboards is not
-0002bfc0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0002bfd0: 2020 2066 6f72 206b 2069 6e20 7365 6c66     for k in self
-0002bfe0: 2e74 656e 736f 7262 6f61 7264 733a 0a20  .tensorboards:. 
-0002bff0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0002c000: 6573 756c 745b 2754 656e 736f 7262 6f61  esult['Tensorboa
-0002c010: 7264 7327 5d2e 6170 7065 6e64 286b 2e74  rds'].append(k.t
-0002c020: 6f5f 6d61 7028 2920 6966 206b 2065 6c73  o_map() if k els
-0002c030: 6520 4e6f 6e65 290a 2020 2020 2020 2020  e None).        
-0002c040: 6966 2073 656c 662e 746f 7461 6c5f 636f  if self.total_co
-0002c050: 756e 7420 6973 206e 6f74 204e 6f6e 653a  unt is not None:
-0002c060: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-0002c070: 756c 745b 2754 6f74 616c 436f 756e 7427  ult['TotalCount'
-0002c080: 5d20 3d20 7365 6c66 2e74 6f74 616c 5f63  ] = self.total_c
-0002c090: 6f75 6e74 0a20 2020 2020 2020 2072 6574  ount.        ret
-0002c0a0: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
-0002c0b0: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
-0002c0c0: 662c 206d 3a20 6469 6374 203d 204e 6f6e  f, m: dict = Non
-0002c0d0: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
-0002c0e0: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
-0002c0f0: 2020 2020 6966 206d 2e67 6574 2827 5265      if m.get('Re
-0002c100: 7175 6573 7449 6427 2920 6973 206e 6f74  questId') is not
-0002c110: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0002c120: 2020 2073 656c 662e 7265 7175 6573 745f     self.request_
-0002c130: 6964 203d 206d 2e67 6574 2827 5265 7175  id = m.get('Requ
-0002c140: 6573 7449 6427 290a 2020 2020 2020 2020  estId').        
-0002c150: 7365 6c66 2e74 656e 736f 7262 6f61 7264  self.tensorboard
-0002c160: 7320 3d20 5b5d 0a20 2020 2020 2020 2069  s = [].        i
-0002c170: 6620 6d2e 6765 7428 2754 656e 736f 7262  f m.get('Tensorb
-0002c180: 6f61 7264 7327 2920 6973 206e 6f74 204e  oards') is not N
-0002c190: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0002c1a0: 2066 6f72 206b 2069 6e20 6d2e 6765 7428   for k in m.get(
-0002c1b0: 2754 656e 736f 7262 6f61 7264 7327 293a  'Tensorboards'):
-0002c1c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002c1d0: 2074 656d 705f 6d6f 6465 6c20 3d20 5465   temp_model = Te
-0002c1e0: 6e73 6f72 626f 6172 6428 290a 2020 2020  nsorboard().    
-0002c1f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0002c200: 2e74 656e 736f 7262 6f61 7264 732e 6170  .tensorboards.ap
-0002c210: 7065 6e64 2874 656d 705f 6d6f 6465 6c2e  pend(temp_model.
-0002c220: 6672 6f6d 5f6d 6170 286b 2929 0a20 2020  from_map(k)).   
-0002c230: 2020 2020 2069 6620 6d2e 6765 7428 2754       if m.get('T
-0002c240: 6f74 616c 436f 756e 7427 2920 6973 206e  otalCount') is n
-0002c250: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0002c260: 2020 2020 2073 656c 662e 746f 7461 6c5f       self.total_
-0002c270: 636f 756e 7420 3d20 6d2e 6765 7428 2754  count = m.get('T
-0002c280: 6f74 616c 436f 756e 7427 290a 2020 2020  otalCount').    
-0002c290: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
-0002c2a0: 0a0a 636c 6173 7320 4c69 7374 5465 6e73  ..class ListTens
-0002c2b0: 6f72 626f 6172 6473 5265 7370 6f6e 7365  orboardsResponse
-0002c2c0: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
-0002c2d0: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
-0002c2e0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-0002c2f0: 2020 2020 6865 6164 6572 733a 2044 6963      headers: Dic
-0002c300: 745b 7374 722c 2073 7472 5d20 3d20 4e6f  t[str, str] = No
-0002c310: 6e65 2c0a 2020 2020 2020 2020 7374 6174  ne,.        stat
-0002c320: 7573 5f63 6f64 653a 2069 6e74 203d 204e  us_code: int = N
-0002c330: 6f6e 652c 0a20 2020 2020 2020 2062 6f64  one,.        bod
-0002c340: 793a 204c 6973 7454 656e 736f 7262 6f61  y: ListTensorboa
-0002c350: 7264 7352 6573 706f 6e73 6542 6f64 7920  rdsResponseBody 
-0002c360: 3d20 4e6f 6e65 2c0a 2020 2020 293a 0a20  = None,.    ):. 
-0002c370: 2020 2020 2020 2073 656c 662e 6865 6164         self.head
-0002c380: 6572 7320 3d20 6865 6164 6572 730a 2020  ers = headers.  
-0002c390: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
-0002c3a0: 735f 636f 6465 203d 2073 7461 7475 735f  s_code = status_
-0002c3b0: 636f 6465 0a20 2020 2020 2020 2073 656c  code.        sel
-0002c3c0: 662e 626f 6479 203d 2062 6f64 790a 0a20  f.body = body.. 
-0002c3d0: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
-0002c3e0: 7365 6c66 293a 0a20 2020 2020 2020 2073  self):.        s
-0002c3f0: 656c 662e 7661 6c69 6461 7465 5f72 6571  elf.validate_req
-0002c400: 7569 7265 6428 7365 6c66 2e68 6561 6465  uired(self.heade
-0002c410: 7273 2c20 2768 6561 6465 7273 2729 0a20  rs, 'headers'). 
-0002c420: 2020 2020 2020 2073 656c 662e 7661 6c69         self.vali
-0002c430: 6461 7465 5f72 6571 7569 7265 6428 7365  date_required(se
-0002c440: 6c66 2e73 7461 7475 735f 636f 6465 2c20  lf.status_code, 
-0002c450: 2773 7461 7475 735f 636f 6465 2729 0a20  'status_code'). 
-0002c460: 2020 2020 2020 2073 656c 662e 7661 6c69         self.vali
-0002c470: 6461 7465 5f72 6571 7569 7265 6428 7365  date_required(se
-0002c480: 6c66 2e62 6f64 792c 2027 626f 6479 2729  lf.body, 'body')
-0002c490: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0002c4a0: 2e62 6f64 793a 0a20 2020 2020 2020 2020  .body:.         
-0002c4b0: 2020 2073 656c 662e 626f 6479 2e76 616c     self.body.val
-0002c4c0: 6964 6174 6528 290a 0a20 2020 2064 6566  idate()..    def
-0002c4d0: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
-0002c4e0: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
-0002c4f0: 7065 7228 292e 746f 5f6d 6170 2829 0a20  per().to_map(). 
-0002c500: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
-0002c510: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0002c520: 2020 2020 2020 2020 7265 7475 726e 205f          return _
-0002c530: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
-0002c540: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
-0002c550: 2020 2020 2069 6620 7365 6c66 2e68 6561       if self.hea
-0002c560: 6465 7273 2069 7320 6e6f 7420 4e6f 6e65  ders is not None
-0002c570: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0002c580: 7375 6c74 5b27 6865 6164 6572 7327 5d20  sult['headers'] 
-0002c590: 3d20 7365 6c66 2e68 6561 6465 7273 0a20  = self.headers. 
-0002c5a0: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
-0002c5b0: 7461 7475 735f 636f 6465 2069 7320 6e6f  tatus_code is no
-0002c5c0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0002c5d0: 2020 2020 7265 7375 6c74 5b27 7374 6174      result['stat
-0002c5e0: 7573 436f 6465 275d 203d 2073 656c 662e  usCode'] = self.
-0002c5f0: 7374 6174 7573 5f63 6f64 650a 2020 2020  status_code.    
-0002c600: 2020 2020 6966 2073 656c 662e 626f 6479      if self.body
-0002c610: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0002c620: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0002c630: 5b27 626f 6479 275d 203d 2073 656c 662e  ['body'] = self.
-0002c640: 626f 6479 2e74 6f5f 6d61 7028 290a 2020  body.to_map().  
-0002c650: 2020 2020 2020 7265 7475 726e 2072 6573        return res
-0002c660: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
-0002c670: 6d5f 6d61 7028 7365 6c66 2c20 6d3a 2064  m_map(self, m: d
-0002c680: 6963 7420 3d20 4e6f 6e65 293a 0a20 2020  ict = None):.   
-0002c690: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
-0002c6a0: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
-0002c6b0: 6d2e 6765 7428 2768 6561 6465 7273 2729  m.get('headers')
-0002c6c0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0002c6d0: 2020 2020 2020 2020 2020 7365 6c66 2e68            self.h
-0002c6e0: 6561 6465 7273 203d 206d 2e67 6574 2827  eaders = m.get('
-0002c6f0: 6865 6164 6572 7327 290a 2020 2020 2020  headers').      
-0002c700: 2020 6966 206d 2e67 6574 2827 7374 6174    if m.get('stat
-0002c710: 7573 436f 6465 2729 2069 7320 6e6f 7420  usCode') is not 
-0002c720: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0002c730: 2020 7365 6c66 2e73 7461 7475 735f 636f    self.status_co
-0002c740: 6465 203d 206d 2e67 6574 2827 7374 6174  de = m.get('stat
-0002c750: 7573 436f 6465 2729 0a20 2020 2020 2020  usCode').       
-0002c760: 2069 6620 6d2e 6765 7428 2762 6f64 7927   if m.get('body'
-0002c770: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-0002c780: 2020 2020 2020 2020 2020 2074 656d 705f             temp_
-0002c790: 6d6f 6465 6c20 3d20 4c69 7374 5465 6e73  model = ListTens
-0002c7a0: 6f72 626f 6172 6473 5265 7370 6f6e 7365  orboardsResponse
-0002c7b0: 426f 6479 2829 0a20 2020 2020 2020 2020  Body().         
-0002c7c0: 2020 2073 656c 662e 626f 6479 203d 2074     self.body = t
-0002c7d0: 656d 705f 6d6f 6465 6c2e 6672 6f6d 5f6d  emp_model.from_m
-0002c7e0: 6170 286d 5b27 626f 6479 275d 290a 2020  ap(m['body']).  
-0002c7f0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0002c800: 660a 0a0a 636c 6173 7320 5374 6172 7454  f...class StartT
-0002c810: 656e 736f 7262 6f61 7264 5265 7175 6573  ensorboardReques
-0002c820: 7428 5465 614d 6f64 656c 293a 0a20 2020  t(TeaModel):.   
-0002c830: 2064 6566 205f 5f69 6e69 745f 5f28 0a20   def __init__(. 
-0002c840: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-0002c850: 2020 2020 2077 6f72 6b73 7061 6365 5f69       workspace_i
-0002c860: 643a 2073 7472 203d 204e 6f6e 652c 0a20  d: str = None,. 
-0002c870: 2020 2029 3a0a 2020 2020 2020 2020 7365     ):.        se
-0002c880: 6c66 2e77 6f72 6b73 7061 6365 5f69 6420  lf.workspace_id 
-0002c890: 3d20 776f 726b 7370 6163 655f 6964 0a0a  = workspace_id..
-0002c8a0: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
-0002c8b0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0002c8c0: 7061 7373 0a0a 2020 2020 6465 6620 746f  pass..    def to
-0002c8d0: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
-0002c8e0: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
-0002c8f0: 2829 2e74 6f5f 6d61 7028 290a 2020 2020  ().to_map().    
-0002c900: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
-0002c910: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0002c920: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
-0002c930: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
-0002c940: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
-0002c950: 2020 6966 2073 656c 662e 776f 726b 7370    if self.worksp
-0002c960: 6163 655f 6964 2069 7320 6e6f 7420 4e6f  ace_id is not No
-0002c970: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0002c980: 7265 7375 6c74 5b27 576f 726b 7370 6163  result['Workspac
-0002c990: 6549 6427 5d20 3d20 7365 6c66 2e77 6f72  eId'] = self.wor
-0002c9a0: 6b73 7061 6365 5f69 640a 2020 2020 2020  kspace_id.      
-0002c9b0: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
-0002c9c0: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
-0002c9d0: 7028 7365 6c66 2c20 6d3a 2064 6963 7420  p(self, m: dict 
-0002c9e0: 3d20 4e6f 6e65 293a 0a20 2020 2020 2020  = None):.       
-0002c9f0: 206d 203d 206d 206f 7220 6469 6374 2829   m = m or dict()
-0002ca00: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-0002ca10: 7428 2757 6f72 6b73 7061 6365 4964 2729  t('WorkspaceId')
-0002ca20: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0002ca30: 2020 2020 2020 2020 2020 7365 6c66 2e77            self.w
-0002ca40: 6f72 6b73 7061 6365 5f69 6420 3d20 6d2e  orkspace_id = m.
-0002ca50: 6765 7428 2757 6f72 6b73 7061 6365 4964  get('WorkspaceId
-0002ca60: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
-0002ca70: 6e20 7365 6c66 0a0a 0a63 6c61 7373 2053  n self...class S
-0002ca80: 7461 7274 5465 6e73 6f72 626f 6172 6452  tartTensorboardR
-0002ca90: 6573 706f 6e73 6542 6f64 7928 5465 614d  esponseBody(TeaM
-0002caa0: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
-0002cab0: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
-0002cac0: 2073 656c 662c 0a20 2020 2020 2020 2072   self,.        r
-0002cad0: 6571 7565 7374 5f69 643a 2073 7472 203d  equest_id: str =
-0002cae0: 204e 6f6e 652c 0a20 2020 2020 2020 2074   None,.        t
-0002caf0: 656e 736f 7262 6f61 7264 5f69 643a 2073  ensorboard_id: s
-0002cb00: 7472 203d 204e 6f6e 652c 0a20 2020 2029  tr = None,.    )
-0002cb10: 3a0a 2020 2020 2020 2020 7365 6c66 2e72  :.        self.r
-0002cb20: 6571 7565 7374 5f69 6420 3d20 7265 7175  equest_id = requ
-0002cb30: 6573 745f 6964 0a20 2020 2020 2020 2073  est_id.        s
-0002cb40: 656c 662e 7465 6e73 6f72 626f 6172 645f  elf.tensorboard_
-0002cb50: 6964 203d 2074 656e 736f 7262 6f61 7264  id = tensorboard
-0002cb60: 5f69 640a 0a20 2020 2064 6566 2076 616c  _id..    def val
-0002cb70: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
-0002cb80: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
-0002cb90: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
-0002cba0: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
-0002cbb0: 7375 7065 7228 292e 746f 5f6d 6170 2829  super().to_map()
-0002cbc0: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
-0002cbd0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0002cbe0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0002cbf0: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
-0002cc00: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
-0002cc10: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
-0002cc20: 6571 7565 7374 5f69 6420 6973 206e 6f74  equest_id is not
-0002cc30: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0002cc40: 2020 2072 6573 756c 745b 2752 6571 7565     result['Reque
-0002cc50: 7374 4964 275d 203d 2073 656c 662e 7265  stId'] = self.re
-0002cc60: 7175 6573 745f 6964 0a20 2020 2020 2020  quest_id.       
-0002cc70: 2069 6620 7365 6c66 2e74 656e 736f 7262   if self.tensorb
-0002cc80: 6f61 7264 5f69 6420 6973 206e 6f74 204e  oard_id is not N
-0002cc90: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0002cca0: 2072 6573 756c 745b 2754 656e 736f 7262   result['Tensorb
-0002ccb0: 6f61 7264 4964 275d 203d 2073 656c 662e  oardId'] = self.
-0002ccc0: 7465 6e73 6f72 626f 6172 645f 6964 0a20  tensorboard_id. 
-0002ccd0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-0002cce0: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
-0002ccf0: 6f6d 5f6d 6170 2873 656c 662c 206d 3a20  om_map(self, m: 
-0002cd00: 6469 6374 203d 204e 6f6e 6529 3a0a 2020  dict = None):.  
-0002cd10: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
-0002cd20: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-0002cd30: 206d 2e67 6574 2827 5265 7175 6573 7449   m.get('RequestI
-0002cd40: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
-0002cd50: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0002cd60: 662e 7265 7175 6573 745f 6964 203d 206d  f.request_id = m
-0002cd70: 2e67 6574 2827 5265 7175 6573 7449 6427  .get('RequestId'
-0002cd80: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-0002cd90: 6574 2827 5465 6e73 6f72 626f 6172 6449  et('TensorboardI
-0002cda0: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
-0002cdb0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0002cdc0: 662e 7465 6e73 6f72 626f 6172 645f 6964  f.tensorboard_id
-0002cdd0: 203d 206d 2e67 6574 2827 5465 6e73 6f72   = m.get('Tensor
-0002cde0: 626f 6172 6449 6427 290a 2020 2020 2020  boardId').      
-0002cdf0: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
-0002ce00: 636c 6173 7320 5374 6172 7454 656e 736f  class StartTenso
-0002ce10: 7262 6f61 7264 5265 7370 6f6e 7365 2854  rboardResponse(T
-0002ce20: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
-0002ce30: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
-0002ce40: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-0002ce50: 2020 6865 6164 6572 733a 2044 6963 745b    headers: Dict[
-0002ce60: 7374 722c 2073 7472 5d20 3d20 4e6f 6e65  str, str] = None
-0002ce70: 2c0a 2020 2020 2020 2020 7374 6174 7573  ,.        status
-0002ce80: 5f63 6f64 653a 2069 6e74 203d 204e 6f6e  _code: int = Non
-0002ce90: 652c 0a20 2020 2020 2020 2062 6f64 793a  e,.        body:
-0002cea0: 2053 7461 7274 5465 6e73 6f72 626f 6172   StartTensorboar
-0002ceb0: 6452 6573 706f 6e73 6542 6f64 7920 3d20  dResponseBody = 
-0002cec0: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
-0002ced0: 2020 2020 2073 656c 662e 6865 6164 6572       self.header
-0002cee0: 7320 3d20 6865 6164 6572 730a 2020 2020  s = headers.    
-0002cef0: 2020 2020 7365 6c66 2e73 7461 7475 735f      self.status_
-0002cf00: 636f 6465 203d 2073 7461 7475 735f 636f  code = status_co
-0002cf10: 6465 0a20 2020 2020 2020 2073 656c 662e  de.        self.
-0002cf20: 626f 6479 203d 2062 6f64 790a 0a20 2020  body = body..   
-0002cf30: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
-0002cf40: 6c66 293a 0a20 2020 2020 2020 2073 656c  lf):.        sel
-0002cf50: 662e 7661 6c69 6461 7465 5f72 6571 7569  f.validate_requi
-0002cf60: 7265 6428 7365 6c66 2e68 6561 6465 7273  red(self.headers
-0002cf70: 2c20 2768 6561 6465 7273 2729 0a20 2020  , 'headers').   
-0002cf80: 2020 2020 2073 656c 662e 7661 6c69 6461       self.valida
-0002cf90: 7465 5f72 6571 7569 7265 6428 7365 6c66  te_required(self
-0002cfa0: 2e73 7461 7475 735f 636f 6465 2c20 2773  .status_code, 's
-0002cfb0: 7461 7475 735f 636f 6465 2729 0a20 2020  tatus_code').   
-0002cfc0: 2020 2020 2073 656c 662e 7661 6c69 6461       self.valida
-0002cfd0: 7465 5f72 6571 7569 7265 6428 7365 6c66  te_required(self
-0002cfe0: 2e62 6f64 792c 2027 626f 6479 2729 0a20  .body, 'body'). 
-0002cff0: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
-0002d000: 6f64 793a 0a20 2020 2020 2020 2020 2020  ody:.           
-0002d010: 2073 656c 662e 626f 6479 2e76 616c 6964   self.body.valid
-0002d020: 6174 6528 290a 0a20 2020 2064 6566 2074  ate()..    def t
-0002d030: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
-0002d040: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
-0002d050: 7228 292e 746f 5f6d 6170 2829 0a20 2020  r().to_map().   
-0002d060: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
-0002d070: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0002d080: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
-0002d090: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
-0002d0a0: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
-0002d0b0: 2020 2069 6620 7365 6c66 2e68 6561 6465     if self.heade
-0002d0c0: 7273 2069 7320 6e6f 7420 4e6f 6e65 3a0a  rs is not None:.
-0002d0d0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-0002d0e0: 6c74 5b27 6865 6164 6572 7327 5d20 3d20  lt['headers'] = 
-0002d0f0: 7365 6c66 2e68 6561 6465 7273 0a20 2020  self.headers.   
-0002d100: 2020 2020 2069 6620 7365 6c66 2e73 7461       if self.sta
-0002d110: 7475 735f 636f 6465 2069 7320 6e6f 7420  tus_code is not 
-0002d120: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0002d130: 2020 7265 7375 6c74 5b27 7374 6174 7573    result['status
-0002d140: 436f 6465 275d 203d 2073 656c 662e 7374  Code'] = self.st
-0002d150: 6174 7573 5f63 6f64 650a 2020 2020 2020  atus_code.      
-0002d160: 2020 6966 2073 656c 662e 626f 6479 2069    if self.body i
-0002d170: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0002d180: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-0002d190: 626f 6479 275d 203d 2073 656c 662e 626f  body'] = self.bo
-0002d1a0: 6479 2e74 6f5f 6d61 7028 290a 2020 2020  dy.to_map().    
-0002d1b0: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
-0002d1c0: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
-0002d1d0: 6d61 7028 7365 6c66 2c20 6d3a 2064 6963  map(self, m: dic
-0002d1e0: 7420 3d20 4e6f 6e65 293a 0a20 2020 2020  t = None):.     
-0002d1f0: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
-0002d200: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
-0002d210: 6765 7428 2768 6561 6465 7273 2729 2069  get('headers') i
-0002d220: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0002d230: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
-0002d240: 6465 7273 203d 206d 2e67 6574 2827 6865  ders = m.get('he
-0002d250: 6164 6572 7327 290a 2020 2020 2020 2020  aders').        
-0002d260: 6966 206d 2e67 6574 2827 7374 6174 7573  if m.get('status
-0002d270: 436f 6465 2729 2069 7320 6e6f 7420 4e6f  Code') is not No
-0002d280: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0002d290: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
-0002d2a0: 203d 206d 2e67 6574 2827 7374 6174 7573   = m.get('status
-0002d2b0: 436f 6465 2729 0a20 2020 2020 2020 2069  Code').        i
-0002d2c0: 6620 6d2e 6765 7428 2762 6f64 7927 2920  f m.get('body') 
-0002d2d0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0002d2e0: 2020 2020 2020 2020 2074 656d 705f 6d6f           temp_mo
-0002d2f0: 6465 6c20 3d20 5374 6172 7454 656e 736f  del = StartTenso
-0002d300: 7262 6f61 7264 5265 7370 6f6e 7365 426f  rboardResponseBo
-0002d310: 6479 2829 0a20 2020 2020 2020 2020 2020  dy().           
-0002d320: 2073 656c 662e 626f 6479 203d 2074 656d   self.body = tem
-0002d330: 705f 6d6f 6465 6c2e 6672 6f6d 5f6d 6170  p_model.from_map
-0002d340: 286d 5b27 626f 6479 275d 290a 2020 2020  (m['body']).    
-0002d350: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
-0002d360: 0a0a 636c 6173 7320 5374 6f70 4a6f 6252  ..class StopJobR
-0002d370: 6573 706f 6e73 6542 6f64 7928 5465 614d  esponseBody(TeaM
-0002d380: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
-0002d390: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
-0002d3a0: 2073 656c 662c 0a20 2020 2020 2020 206a   self,.        j
-0002d3b0: 6f62 5f69 643a 2073 7472 203d 204e 6f6e  ob_id: str = Non
-0002d3c0: 652c 0a20 2020 2020 2020 2072 6571 7565  e,.        reque
-0002d3d0: 7374 5f69 643a 2073 7472 203d 204e 6f6e  st_id: str = Non
-0002d3e0: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
-0002d3f0: 2020 7365 6c66 2e6a 6f62 5f69 6420 3d20    self.job_id = 
-0002d400: 6a6f 625f 6964 0a20 2020 2020 2020 2073  job_id.        s
-0002d410: 656c 662e 7265 7175 6573 745f 6964 203d  elf.request_id =
-0002d420: 2072 6571 7565 7374 5f69 640a 0a20 2020   request_id..   
-0002d430: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
-0002d440: 6c66 293a 0a20 2020 2020 2020 2070 6173  lf):.        pas
-0002d450: 730a 0a20 2020 2064 6566 2074 6f5f 6d61  s..    def to_ma
-0002d460: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
-0002d470: 205f 6d61 7020 3d20 7375 7065 7228 292e   _map = super().
-0002d480: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
-0002d490: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
-0002d4a0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0002d4b0: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
-0002d4c0: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-0002d4d0: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
-0002d4e0: 6620 7365 6c66 2e6a 6f62 5f69 6420 6973  f self.job_id is
-0002d4f0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0002d500: 2020 2020 2020 2072 6573 756c 745b 274a         result['J
-0002d510: 6f62 4964 275d 203d 2073 656c 662e 6a6f  obId'] = self.jo
-0002d520: 625f 6964 0a20 2020 2020 2020 2069 6620  b_id.        if 
-0002d530: 7365 6c66 2e72 6571 7565 7374 5f69 6420  self.request_id 
-0002d540: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0002d550: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-0002d560: 2752 6571 7565 7374 4964 275d 203d 2073  'RequestId'] = s
-0002d570: 656c 662e 7265 7175 6573 745f 6964 0a20  elf.request_id. 
-0002d580: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-0002d590: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
-0002d5a0: 6f6d 5f6d 6170 2873 656c 662c 206d 3a20  om_map(self, m: 
-0002d5b0: 6469 6374 203d 204e 6f6e 6529 3a0a 2020  dict = None):.  
-0002d5c0: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
-0002d5d0: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-0002d5e0: 206d 2e67 6574 2827 4a6f 6249 6427 2920   m.get('JobId') 
-0002d5f0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0002d600: 2020 2020 2020 2020 2073 656c 662e 6a6f           self.jo
-0002d610: 625f 6964 203d 206d 2e67 6574 2827 4a6f  b_id = m.get('Jo
-0002d620: 6249 6427 290a 2020 2020 2020 2020 6966  bId').        if
-0002d630: 206d 2e67 6574 2827 5265 7175 6573 7449   m.get('RequestI
-0002d640: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
-0002d650: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0002d660: 662e 7265 7175 6573 745f 6964 203d 206d  f.request_id = m
-0002d670: 2e67 6574 2827 5265 7175 6573 7449 6427  .get('RequestId'
-0002d680: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-0002d690: 2073 656c 660a 0a0a 636c 6173 7320 5374   self...class St
-0002d6a0: 6f70 4a6f 6252 6573 706f 6e73 6528 5465  opJobResponse(Te
-0002d6b0: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
-0002d6c0: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
-0002d6d0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-0002d6e0: 2068 6561 6465 7273 3a20 4469 6374 5b73   headers: Dict[s
-0002d6f0: 7472 2c20 7374 725d 203d 204e 6f6e 652c  tr, str] = None,
-0002d700: 0a20 2020 2020 2020 2073 7461 7475 735f  .        status_
-0002d710: 636f 6465 3a20 696e 7420 3d20 4e6f 6e65  code: int = None
-0002d720: 2c0a 2020 2020 2020 2020 626f 6479 3a20  ,.        body: 
-0002d730: 5374 6f70 4a6f 6252 6573 706f 6e73 6542  StopJobResponseB
-0002d740: 6f64 7920 3d20 4e6f 6e65 2c0a 2020 2020  ody = None,.    
-0002d750: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-0002d760: 6865 6164 6572 7320 3d20 6865 6164 6572  headers = header
-0002d770: 730a 2020 2020 2020 2020 7365 6c66 2e73  s.        self.s
-0002d780: 7461 7475 735f 636f 6465 203d 2073 7461  tatus_code = sta
-0002d790: 7475 735f 636f 6465 0a20 2020 2020 2020  tus_code.       
-0002d7a0: 2073 656c 662e 626f 6479 203d 2062 6f64   self.body = bod
-0002d7b0: 790a 0a20 2020 2064 6566 2076 616c 6964  y..    def valid
-0002d7c0: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
-0002d7d0: 2020 2073 656c 662e 7661 6c69 6461 7465     self.validate
-0002d7e0: 5f72 6571 7569 7265 6428 7365 6c66 2e68  _required(self.h
-0002d7f0: 6561 6465 7273 2c20 2768 6561 6465 7273  eaders, 'headers
-0002d800: 2729 0a20 2020 2020 2020 2073 656c 662e  ').        self.
-0002d810: 7661 6c69 6461 7465 5f72 6571 7569 7265  validate_require
-0002d820: 6428 7365 6c66 2e73 7461 7475 735f 636f  d(self.status_co
-0002d830: 6465 2c20 2773 7461 7475 735f 636f 6465  de, 'status_code
-0002d840: 2729 0a20 2020 2020 2020 2073 656c 662e  ').        self.
-0002d850: 7661 6c69 6461 7465 5f72 6571 7569 7265  validate_require
-0002d860: 6428 7365 6c66 2e62 6f64 792c 2027 626f  d(self.body, 'bo
-0002d870: 6479 2729 0a20 2020 2020 2020 2069 6620  dy').        if 
-0002d880: 7365 6c66 2e62 6f64 793a 0a20 2020 2020  self.body:.     
-0002d890: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
-0002d8a0: 2e76 616c 6964 6174 6528 290a 0a20 2020  .validate()..   
-0002d8b0: 2064 6566 2074 6f5f 6d61 7028 7365 6c66   def to_map(self
-0002d8c0: 293a 0a20 2020 2020 2020 205f 6d61 7020  ):.        _map 
-0002d8d0: 3d20 7375 7065 7228 292e 746f 5f6d 6170  = super().to_map
-0002d8e0: 2829 0a20 2020 2020 2020 2069 6620 5f6d  ().        if _m
-0002d8f0: 6170 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ap is not None:.
-0002d900: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0002d910: 726e 205f 6d61 700a 0a20 2020 2020 2020  rn _map..       
-0002d920: 2072 6573 756c 7420 3d20 6469 6374 2829   result = dict()
-0002d930: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0002d940: 2e68 6561 6465 7273 2069 7320 6e6f 7420  .headers is not 
-0002d950: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0002d960: 2020 7265 7375 6c74 5b27 6865 6164 6572    result['header
-0002d970: 7327 5d20 3d20 7365 6c66 2e68 6561 6465  s'] = self.heade
-0002d980: 7273 0a20 2020 2020 2020 2069 6620 7365  rs.        if se
-0002d990: 6c66 2e73 7461 7475 735f 636f 6465 2069  lf.status_code i
-0002d9a0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0002d9b0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-0002d9c0: 7374 6174 7573 436f 6465 275d 203d 2073  statusCode'] = s
-0002d9d0: 656c 662e 7374 6174 7573 5f63 6f64 650a  elf.status_code.
-0002d9e0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0002d9f0: 626f 6479 2069 7320 6e6f 7420 4e6f 6e65  body is not None
-0002da00: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0002da10: 7375 6c74 5b27 626f 6479 275d 203d 2073  sult['body'] = s
-0002da20: 656c 662e 626f 6479 2e74 6f5f 6d61 7028  elf.body.to_map(
-0002da30: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-0002da40: 2072 6573 756c 740a 0a20 2020 2064 6566   result..    def
-0002da50: 2066 726f 6d5f 6d61 7028 7365 6c66 2c20   from_map(self, 
-0002da60: 6d3a 2064 6963 7420 3d20 4e6f 6e65 293a  m: dict = None):
-0002da70: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
-0002da80: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
-0002da90: 2069 6620 6d2e 6765 7428 2768 6561 6465   if m.get('heade
-0002daa0: 7273 2729 2069 7320 6e6f 7420 4e6f 6e65  rs') is not None
-0002dab0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0002dac0: 6c66 2e68 6561 6465 7273 203d 206d 2e67  lf.headers = m.g
-0002dad0: 6574 2827 6865 6164 6572 7327 290a 2020  et('headers').  
-0002dae0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-0002daf0: 7374 6174 7573 436f 6465 2729 2069 7320  statusCode') is 
-0002db00: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0002db10: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
-0002db20: 735f 636f 6465 203d 206d 2e67 6574 2827  s_code = m.get('
-0002db30: 7374 6174 7573 436f 6465 2729 0a20 2020  statusCode').   
-0002db40: 2020 2020 2069 6620 6d2e 6765 7428 2762       if m.get('b
-0002db50: 6f64 7927 2920 6973 206e 6f74 204e 6f6e  ody') is not Non
-0002db60: 653a 0a20 2020 2020 2020 2020 2020 2074  e:.            t
-0002db70: 656d 705f 6d6f 6465 6c20 3d20 5374 6f70  emp_model = Stop
-0002db80: 4a6f 6252 6573 706f 6e73 6542 6f64 7928  JobResponseBody(
-0002db90: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-0002dba0: 6c66 2e62 6f64 7920 3d20 7465 6d70 5f6d  lf.body = temp_m
-0002dbb0: 6f64 656c 2e66 726f 6d5f 6d61 7028 6d5b  odel.from_map(m[
-0002dbc0: 2762 6f64 7927 5d29 0a20 2020 2020 2020  'body']).       
-0002dbd0: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
-0002dbe0: 6c61 7373 2053 746f 7054 656e 736f 7262  lass StopTensorb
-0002dbf0: 6f61 7264 5265 7175 6573 7428 5465 614d  oardRequest(TeaM
-0002dc00: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
-0002dc10: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
-0002dc20: 2073 656c 662c 0a20 2020 2020 2020 2077   self,.        w
-0002dc30: 6f72 6b73 7061 6365 5f69 643a 2073 7472  orkspace_id: str
-0002dc40: 203d 204e 6f6e 652c 0a20 2020 2029 3a0a   = None,.    ):.
-0002dc50: 2020 2020 2020 2020 7365 6c66 2e77 6f72          self.wor
-0002dc60: 6b73 7061 6365 5f69 6420 3d20 776f 726b  kspace_id = work
-0002dc70: 7370 6163 655f 6964 0a0a 2020 2020 6465  space_id..    de
-0002dc80: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
-0002dc90: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
-0002dca0: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
-0002dcb0: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
-0002dcc0: 6170 203d 2073 7570 6572 2829 2e74 6f5f  ap = super().to_
-0002dcd0: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
-0002dce0: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
-0002dcf0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-0002dd00: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
-0002dd10: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
-0002dd20: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
-0002dd30: 656c 662e 776f 726b 7370 6163 655f 6964  elf.workspace_id
-0002dd40: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0002dd50: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0002dd60: 5b27 576f 726b 7370 6163 6549 6427 5d20  ['WorkspaceId'] 
-0002dd70: 3d20 7365 6c66 2e77 6f72 6b73 7061 6365  = self.workspace
-0002dd80: 5f69 640a 2020 2020 2020 2020 7265 7475  _id.        retu
-0002dd90: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
-0002dda0: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
-0002ddb0: 2c20 6d3a 2064 6963 7420 3d20 4e6f 6e65  , m: dict = None
-0002ddc0: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
-0002ddd0: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
-0002dde0: 2020 2069 6620 6d2e 6765 7428 2757 6f72     if m.get('Wor
-0002ddf0: 6b73 7061 6365 4964 2729 2069 7320 6e6f  kspaceId') is no
-0002de00: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0002de10: 2020 2020 7365 6c66 2e77 6f72 6b73 7061      self.workspa
-0002de20: 6365 5f69 6420 3d20 6d2e 6765 7428 2757  ce_id = m.get('W
-0002de30: 6f72 6b73 7061 6365 4964 2729 0a20 2020  orkspaceId').   
-0002de40: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0002de50: 0a0a 0a63 6c61 7373 2053 746f 7054 656e  ...class StopTen
-0002de60: 736f 7262 6f61 7264 5265 7370 6f6e 7365  sorboardResponse
-0002de70: 426f 6479 2854 6561 4d6f 6465 6c29 3a0a  Body(TeaModel):.
-0002de80: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-0002de90: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-0002dea0: 2020 2020 2020 2020 7265 7175 6573 745f          request_
-0002deb0: 6964 3a20 7374 7220 3d20 4e6f 6e65 2c0a  id: str = None,.
-0002dec0: 2020 2020 2020 2020 7465 6e73 6f72 626f          tensorbo
-0002ded0: 6172 645f 6964 3a20 7374 7220 3d20 4e6f  ard_id: str = No
-0002dee0: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
-0002def0: 2020 2073 656c 662e 7265 7175 6573 745f     self.request_
-0002df00: 6964 203d 2072 6571 7565 7374 5f69 640a  id = request_id.
-0002df10: 2020 2020 2020 2020 7365 6c66 2e74 656e          self.ten
-0002df20: 736f 7262 6f61 7264 5f69 6420 3d20 7465  sorboard_id = te
-0002df30: 6e73 6f72 626f 6172 645f 6964 0a0a 2020  nsorboard_id..  
-0002df40: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
-0002df50: 656c 6629 3a0a 2020 2020 2020 2020 7061  elf):.        pa
-0002df60: 7373 0a0a 2020 2020 6465 6620 746f 5f6d  ss..    def to_m
-0002df70: 6170 2873 656c 6629 3a0a 2020 2020 2020  ap(self):.      
-0002df80: 2020 5f6d 6170 203d 2073 7570 6572 2829    _map = super()
-0002df90: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
-0002dfa0: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
-0002dfb0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0002dfc0: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
-0002dfd0: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
-0002dfe0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-0002dff0: 6966 2073 656c 662e 7265 7175 6573 745f  if self.request_
-0002e000: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
-0002e010: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-0002e020: 6c74 5b27 5265 7175 6573 7449 6427 5d20  lt['RequestId'] 
-0002e030: 3d20 7365 6c66 2e72 6571 7565 7374 5f69  = self.request_i
-0002e040: 640a 2020 2020 2020 2020 6966 2073 656c  d.        if sel
-0002e050: 662e 7465 6e73 6f72 626f 6172 645f 6964  f.tensorboard_id
-0002e060: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0002e070: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0002e080: 5b27 5465 6e73 6f72 626f 6172 6449 6427  ['TensorboardId'
-0002e090: 5d20 3d20 7365 6c66 2e74 656e 736f 7262  ] = self.tensorb
-0002e0a0: 6f61 7264 5f69 640a 2020 2020 2020 2020  oard_id.        
-0002e0b0: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
-0002e0c0: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
-0002e0d0: 7365 6c66 2c20 6d3a 2064 6963 7420 3d20  self, m: dict = 
-0002e0e0: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
-0002e0f0: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
-0002e100: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-0002e110: 2752 6571 7565 7374 4964 2729 2069 7320  'RequestId') is 
-0002e120: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0002e130: 2020 2020 2020 7365 6c66 2e72 6571 7565        self.reque
-0002e140: 7374 5f69 6420 3d20 6d2e 6765 7428 2752  st_id = m.get('R
-0002e150: 6571 7565 7374 4964 2729 0a20 2020 2020  equestId').     
-0002e160: 2020 2069 6620 6d2e 6765 7428 2754 656e     if m.get('Ten
-0002e170: 736f 7262 6f61 7264 4964 2729 2069 7320  sorboardId') is 
-0002e180: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0002e190: 2020 2020 2020 7365 6c66 2e74 656e 736f        self.tenso
-0002e1a0: 7262 6f61 7264 5f69 6420 3d20 6d2e 6765  rboard_id = m.ge
-0002e1b0: 7428 2754 656e 736f 7262 6f61 7264 4964  t('TensorboardId
-0002e1c0: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
-0002e1d0: 6e20 7365 6c66 0a0a 0a63 6c61 7373 2053  n self...class S
-0002e1e0: 746f 7054 656e 736f 7262 6f61 7264 5265  topTensorboardRe
-0002e1f0: 7370 6f6e 7365 2854 6561 4d6f 6465 6c29  sponse(TeaModel)
-0002e200: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
-0002e210: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
-0002e220: 2c0a 2020 2020 2020 2020 6865 6164 6572  ,.        header
-0002e230: 733a 2044 6963 745b 7374 722c 2073 7472  s: Dict[str, str
-0002e240: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-0002e250: 2020 7374 6174 7573 5f63 6f64 653a 2069    status_code: i
-0002e260: 6e74 203d 204e 6f6e 652c 0a20 2020 2020  nt = None,.     
-0002e270: 2020 2062 6f64 793a 2053 746f 7054 656e     body: StopTen
-0002e280: 736f 7262 6f61 7264 5265 7370 6f6e 7365  sorboardResponse
-0002e290: 426f 6479 203d 204e 6f6e 652c 0a20 2020  Body = None,.   
-0002e2a0: 2029 3a0a 2020 2020 2020 2020 7365 6c66   ):.        self
-0002e2b0: 2e68 6561 6465 7273 203d 2068 6561 6465  .headers = heade
-0002e2c0: 7273 0a20 2020 2020 2020 2073 656c 662e  rs.        self.
-0002e2d0: 7374 6174 7573 5f63 6f64 6520 3d20 7374  status_code = st
-0002e2e0: 6174 7573 5f63 6f64 650a 2020 2020 2020  atus_code.      
-0002e2f0: 2020 7365 6c66 2e62 6f64 7920 3d20 626f    self.body = bo
-0002e300: 6479 0a0a 2020 2020 6465 6620 7661 6c69  dy..    def vali
-0002e310: 6461 7465 2873 656c 6629 3a0a 2020 2020  date(self):.    
-0002e320: 2020 2020 7365 6c66 2e76 616c 6964 6174      self.validat
-0002e330: 655f 7265 7175 6972 6564 2873 656c 662e  e_required(self.
-0002e340: 6865 6164 6572 732c 2027 6865 6164 6572  headers, 'header
-0002e350: 7327 290a 2020 2020 2020 2020 7365 6c66  s').        self
-0002e360: 2e76 616c 6964 6174 655f 7265 7175 6972  .validate_requir
-0002e370: 6564 2873 656c 662e 7374 6174 7573 5f63  ed(self.status_c
-0002e380: 6f64 652c 2027 7374 6174 7573 5f63 6f64  ode, 'status_cod
-0002e390: 6527 290a 2020 2020 2020 2020 7365 6c66  e').        self
-0002e3a0: 2e76 616c 6964 6174 655f 7265 7175 6972  .validate_requir
-0002e3b0: 6564 2873 656c 662e 626f 6479 2c20 2762  ed(self.body, 'b
-0002e3c0: 6f64 7927 290a 2020 2020 2020 2020 6966  ody').        if
-0002e3d0: 2073 656c 662e 626f 6479 3a0a 2020 2020   self.body:.    
-0002e3e0: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
-0002e3f0: 792e 7661 6c69 6461 7465 2829 0a0a 2020  y.validate()..  
-0002e400: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
-0002e410: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
-0002e420: 203d 2073 7570 6572 2829 2e74 6f5f 6d61   = super().to_ma
-0002e430: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
-0002e440: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
-0002e450: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0002e460: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
-0002e470: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
-0002e480: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-0002e490: 662e 6865 6164 6572 7320 6973 206e 6f74  f.headers is not
-0002e4a0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0002e4b0: 2020 2072 6573 756c 745b 2768 6561 6465     result['heade
-0002e4c0: 7273 275d 203d 2073 656c 662e 6865 6164  rs'] = self.head
-0002e4d0: 6572 730a 2020 2020 2020 2020 6966 2073  ers.        if s
-0002e4e0: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
-0002e4f0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0002e500: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-0002e510: 2773 7461 7475 7343 6f64 6527 5d20 3d20  'statusCode'] = 
-0002e520: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
-0002e530: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0002e540: 2e62 6f64 7920 6973 206e 6f74 204e 6f6e  .body is not Non
-0002e550: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-0002e560: 6573 756c 745b 2762 6f64 7927 5d20 3d20  esult['body'] = 
-0002e570: 7365 6c66 2e62 6f64 792e 746f 5f6d 6170  self.body.to_map
-0002e580: 2829 0a20 2020 2020 2020 2072 6574 7572  ().        retur
-0002e590: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
-0002e5a0: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
-0002e5b0: 206d 3a20 6469 6374 203d 204e 6f6e 6529   m: dict = None)
-0002e5c0: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
-0002e5d0: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
-0002e5e0: 2020 6966 206d 2e67 6574 2827 6865 6164    if m.get('head
-0002e5f0: 6572 7327 2920 6973 206e 6f74 204e 6f6e  ers') is not Non
-0002e600: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-0002e610: 656c 662e 6865 6164 6572 7320 3d20 6d2e  elf.headers = m.
-0002e620: 6765 7428 2768 6561 6465 7273 2729 0a20  get('headers'). 
-0002e630: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-0002e640: 2773 7461 7475 7343 6f64 6527 2920 6973  'statusCode') is
-0002e650: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0002e660: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
-0002e670: 7573 5f63 6f64 6520 3d20 6d2e 6765 7428  us_code = m.get(
-0002e680: 2773 7461 7475 7343 6f64 6527 290a 2020  'statusCode').  
-0002e690: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-0002e6a0: 626f 6479 2729 2069 7320 6e6f 7420 4e6f  body') is not No
-0002e6b0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0002e6c0: 7465 6d70 5f6d 6f64 656c 203d 2053 746f  temp_model = Sto
-0002e6d0: 7054 656e 736f 7262 6f61 7264 5265 7370  pTensorboardResp
-0002e6e0: 6f6e 7365 426f 6479 2829 0a20 2020 2020  onseBody().     
-0002e6f0: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
-0002e700: 203d 2074 656d 705f 6d6f 6465 6c2e 6672   = temp_model.fr
-0002e710: 6f6d 5f6d 6170 286d 5b27 626f 6479 275d  om_map(m['body']
-0002e720: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-0002e730: 2073 656c 660a 0a0a 636c 6173 7320 5570   self...class Up
-0002e740: 6461 7465 4a6f 6252 6571 7565 7374 2854  dateJobRequest(T
-0002e750: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
-0002e760: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
-0002e770: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-0002e780: 2020 7072 696f 7269 7479 3a20 696e 7420    priority: int 
-0002e790: 3d20 4e6f 6e65 2c0a 2020 2020 293a 0a20  = None,.    ):. 
-0002e7a0: 2020 2020 2020 2073 656c 662e 7072 696f         self.prio
-0002e7b0: 7269 7479 203d 2070 7269 6f72 6974 790a  rity = priority.
-0002e7c0: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
-0002e7d0: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
-0002e7e0: 2070 6173 730a 0a20 2020 2064 6566 2074   pass..    def t
-0002e7f0: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
-0002e800: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
-0002e810: 7228 292e 746f 5f6d 6170 2829 0a20 2020  r().to_map().   
-0002e820: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
-0002e830: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0002e840: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
-0002e850: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
-0002e860: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
-0002e870: 2020 2069 6620 7365 6c66 2e70 7269 6f72     if self.prior
-0002e880: 6974 7920 6973 206e 6f74 204e 6f6e 653a  ity is not None:
-0002e890: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-0002e8a0: 756c 745b 2750 7269 6f72 6974 7927 5d20  ult['Priority'] 
-0002e8b0: 3d20 7365 6c66 2e70 7269 6f72 6974 790a  = self.priority.
-0002e8c0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-0002e8d0: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
-0002e8e0: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3a  rom_map(self, m:
-0002e8f0: 2064 6963 7420 3d20 4e6f 6e65 293a 0a20   dict = None):. 
-0002e900: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
-0002e910: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
-0002e920: 6620 6d2e 6765 7428 2750 7269 6f72 6974  f m.get('Priorit
-0002e930: 7927 2920 6973 206e 6f74 204e 6f6e 653a  y') is not None:
-0002e940: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0002e950: 662e 7072 696f 7269 7479 203d 206d 2e67  f.priority = m.g
-0002e960: 6574 2827 5072 696f 7269 7479 2729 0a20  et('Priority'). 
-0002e970: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0002e980: 6c66 0a0a 0a63 6c61 7373 2055 7064 6174  lf...class Updat
-0002e990: 654a 6f62 5265 7370 6f6e 7365 426f 6479  eJobResponseBody
-0002e9a0: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
-0002e9b0: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
-0002e9c0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-0002e9d0: 2020 2020 6a6f 625f 6964 3a20 7374 7220      job_id: str 
-0002e9e0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-0002e9f0: 7265 7175 6573 745f 6964 3a20 7374 7220  request_id: str 
-0002ea00: 3d20 4e6f 6e65 2c0a 2020 2020 293a 0a20  = None,.    ):. 
-0002ea10: 2020 2020 2020 2073 656c 662e 6a6f 625f         self.job_
-0002ea20: 6964 203d 206a 6f62 5f69 640a 2020 2020  id = job_id.    
-0002ea30: 2020 2020 7365 6c66 2e72 6571 7565 7374      self.request
-0002ea40: 5f69 6420 3d20 7265 7175 6573 745f 6964  _id = request_id
-0002ea50: 0a0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
-0002ea60: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
-0002ea70: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
-0002ea80: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
-0002ea90: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
-0002eaa0: 6572 2829 2e74 6f5f 6d61 7028 290a 2020  er().to_map().  
-0002eab0: 2020 2020 2020 6966 205f 6d61 7020 6973        if _map is
-0002eac0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0002ead0: 2020 2020 2020 2072 6574 7572 6e20 5f6d         return _m
-0002eae0: 6170 0a0a 2020 2020 2020 2020 7265 7375  ap..        resu
-0002eaf0: 6c74 203d 2064 6963 7428 290a 2020 2020  lt = dict().    
-0002eb00: 2020 2020 6966 2073 656c 662e 6a6f 625f      if self.job_
-0002eb10: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
-0002eb20: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-0002eb30: 6c74 5b27 4a6f 6249 6427 5d20 3d20 7365  lt['JobId'] = se
-0002eb40: 6c66 2e6a 6f62 5f69 640a 2020 2020 2020  lf.job_id.      
-0002eb50: 2020 6966 2073 656c 662e 7265 7175 6573    if self.reques
-0002eb60: 745f 6964 2069 7320 6e6f 7420 4e6f 6e65  t_id is not None
-0002eb70: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0002eb80: 7375 6c74 5b27 5265 7175 6573 7449 6427  sult['RequestId'
-0002eb90: 5d20 3d20 7365 6c66 2e72 6571 7565 7374  ] = self.request
-0002eba0: 5f69 640a 2020 2020 2020 2020 7265 7475  _id.        retu
-0002ebb0: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
-0002ebc0: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
-0002ebd0: 2c20 6d3a 2064 6963 7420 3d20 4e6f 6e65  , m: dict = None
-0002ebe0: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
-0002ebf0: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
-0002ec00: 2020 2069 6620 6d2e 6765 7428 274a 6f62     if m.get('Job
-0002ec10: 4964 2729 2069 7320 6e6f 7420 4e6f 6e65  Id') is not None
-0002ec20: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0002ec30: 6c66 2e6a 6f62 5f69 6420 3d20 6d2e 6765  lf.job_id = m.ge
-0002ec40: 7428 274a 6f62 4964 2729 0a20 2020 2020  t('JobId').     
-0002ec50: 2020 2069 6620 6d2e 6765 7428 2752 6571     if m.get('Req
-0002ec60: 7565 7374 4964 2729 2069 7320 6e6f 7420  uestId') is not 
-0002ec70: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0002ec80: 2020 7365 6c66 2e72 6571 7565 7374 5f69    self.request_i
-0002ec90: 6420 3d20 6d2e 6765 7428 2752 6571 7565  d = m.get('Reque
-0002eca0: 7374 4964 2729 0a20 2020 2020 2020 2072  stId').        r
-0002ecb0: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
-0002ecc0: 7373 2055 7064 6174 654a 6f62 5265 7370  ss UpdateJobResp
-0002ecd0: 6f6e 7365 2854 6561 4d6f 6465 6c29 3a0a  onse(TeaModel):.
-0002ece0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-0002ecf0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-0002ed00: 2020 2020 2020 2020 6865 6164 6572 733a          headers:
-0002ed10: 2044 6963 745b 7374 722c 2073 7472 5d20   Dict[str, str] 
-0002ed20: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-0002ed30: 7374 6174 7573 5f63 6f64 653a 2069 6e74  status_code: int
-0002ed40: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-0002ed50: 2062 6f64 793a 2055 7064 6174 654a 6f62   body: UpdateJob
-0002ed60: 5265 7370 6f6e 7365 426f 6479 203d 204e  ResponseBody = N
-0002ed70: 6f6e 652c 0a20 2020 2029 3a0a 2020 2020  one,.    ):.    
-0002ed80: 2020 2020 7365 6c66 2e68 6561 6465 7273      self.headers
-0002ed90: 203d 2068 6561 6465 7273 0a20 2020 2020   = headers.     
-0002eda0: 2020 2073 656c 662e 7374 6174 7573 5f63     self.status_c
-0002edb0: 6f64 6520 3d20 7374 6174 7573 5f63 6f64  ode = status_cod
-0002edc0: 650a 2020 2020 2020 2020 7365 6c66 2e62  e.        self.b
-0002edd0: 6f64 7920 3d20 626f 6479 0a0a 2020 2020  ody = body..    
-0002ede0: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
-0002edf0: 6629 3a0a 2020 2020 2020 2020 7365 6c66  f):.        self
-0002ee00: 2e76 616c 6964 6174 655f 7265 7175 6972  .validate_requir
-0002ee10: 6564 2873 656c 662e 6865 6164 6572 732c  ed(self.headers,
-0002ee20: 2027 6865 6164 6572 7327 290a 2020 2020   'headers').    
-0002ee30: 2020 2020 7365 6c66 2e76 616c 6964 6174      self.validat
-0002ee40: 655f 7265 7175 6972 6564 2873 656c 662e  e_required(self.
-0002ee50: 7374 6174 7573 5f63 6f64 652c 2027 7374  status_code, 'st
-0002ee60: 6174 7573 5f63 6f64 6527 290a 2020 2020  atus_code').    
-0002ee70: 2020 2020 7365 6c66 2e76 616c 6964 6174      self.validat
-0002ee80: 655f 7265 7175 6972 6564 2873 656c 662e  e_required(self.
-0002ee90: 626f 6479 2c20 2762 6f64 7927 290a 2020  body, 'body').  
-0002eea0: 2020 2020 2020 6966 2073 656c 662e 626f        if self.bo
-0002eeb0: 6479 3a0a 2020 2020 2020 2020 2020 2020  dy:.            
-0002eec0: 7365 6c66 2e62 6f64 792e 7661 6c69 6461  self.body.valida
-0002eed0: 7465 2829 0a0a 2020 2020 6465 6620 746f  te()..    def to
-0002eee0: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
-0002eef0: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
-0002ef00: 2829 2e74 6f5f 6d61 7028 290a 2020 2020  ().to_map().    
-0002ef10: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
-0002ef20: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0002ef30: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
-0002ef40: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
-0002ef50: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
-0002ef60: 2020 6966 2073 656c 662e 6865 6164 6572    if self.header
-0002ef70: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
-0002ef80: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-0002ef90: 745b 2768 6561 6465 7273 275d 203d 2073  t['headers'] = s
-0002efa0: 656c 662e 6865 6164 6572 730a 2020 2020  elf.headers.    
-0002efb0: 2020 2020 6966 2073 656c 662e 7374 6174      if self.stat
-0002efc0: 7573 5f63 6f64 6520 6973 206e 6f74 204e  us_code is not N
-0002efd0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0002efe0: 2072 6573 756c 745b 2773 7461 7475 7343   result['statusC
-0002eff0: 6f64 6527 5d20 3d20 7365 6c66 2e73 7461  ode'] = self.sta
-0002f000: 7475 735f 636f 6465 0a20 2020 2020 2020  tus_code.       
-0002f010: 2069 6620 7365 6c66 2e62 6f64 7920 6973   if self.body is
-0002f020: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0002f030: 2020 2020 2020 2072 6573 756c 745b 2762         result['b
-0002f040: 6f64 7927 5d20 3d20 7365 6c66 2e62 6f64  ody'] = self.bod
-0002f050: 792e 746f 5f6d 6170 2829 0a20 2020 2020  y.to_map().     
-0002f060: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
-0002f070: 0a0a 2020 2020 6465 6620 6672 6f6d 5f6d  ..    def from_m
-0002f080: 6170 2873 656c 662c 206d 3a20 6469 6374  ap(self, m: dict
-0002f090: 203d 204e 6f6e 6529 3a0a 2020 2020 2020   = None):.      
-0002f0a0: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
-0002f0b0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-0002f0c0: 6574 2827 6865 6164 6572 7327 2920 6973  et('headers') is
-0002f0d0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0002f0e0: 2020 2020 2020 2073 656c 662e 6865 6164         self.head
-0002f0f0: 6572 7320 3d20 6d2e 6765 7428 2768 6561  ers = m.get('hea
-0002f100: 6465 7273 2729 0a20 2020 2020 2020 2069  ders').        i
-0002f110: 6620 6d2e 6765 7428 2773 7461 7475 7343  f m.get('statusC
-0002f120: 6f64 6527 2920 6973 206e 6f74 204e 6f6e  ode') is not Non
-0002f130: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-0002f140: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
-0002f150: 3d20 6d2e 6765 7428 2773 7461 7475 7343  = m.get('statusC
-0002f160: 6f64 6527 290a 2020 2020 2020 2020 6966  ode').        if
-0002f170: 206d 2e67 6574 2827 626f 6479 2729 2069   m.get('body') i
-0002f180: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0002f190: 2020 2020 2020 2020 7465 6d70 5f6d 6f64          temp_mod
-0002f1a0: 656c 203d 2055 7064 6174 654a 6f62 5265  el = UpdateJobRe
-0002f1b0: 7370 6f6e 7365 426f 6479 2829 0a20 2020  sponseBody().   
-0002f1c0: 2020 2020 2020 2020 2073 656c 662e 626f           self.bo
-0002f1d0: 6479 203d 2074 656d 705f 6d6f 6465 6c2e  dy = temp_model.
-0002f1e0: 6672 6f6d 5f6d 6170 286d 5b27 626f 6479  from_map(m['body
-0002f1f0: 275d 290a 2020 2020 2020 2020 7265 7475  ']).        retu
-0002f200: 726e 2073 656c 660a 0a0a 636c 6173 7320  rn self...class 
-0002f210: 5570 6461 7465 5465 6e73 6f72 626f 6172  UpdateTensorboar
-0002f220: 6452 6571 7565 7374 2854 6561 4d6f 6465  dRequest(TeaMode
-0002f230: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
-0002f240: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
-0002f250: 6c66 2c0a 2020 2020 2020 2020 6d61 785f  lf,.        max_
-0002f260: 7275 6e6e 696e 675f 7469 6d65 5f6d 696e  running_time_min
-0002f270: 7574 6573 3a20 696e 7420 3d20 4e6f 6e65  utes: int = None
-0002f280: 2c0a 2020 2020 2020 2020 776f 726b 7370  ,.        worksp
-0002f290: 6163 655f 6964 3a20 7374 7220 3d20 4e6f  ace_id: str = No
-0002f2a0: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
-0002f2b0: 2020 2073 656c 662e 6d61 785f 7275 6e6e     self.max_runn
-0002f2c0: 696e 675f 7469 6d65 5f6d 696e 7574 6573  ing_time_minutes
-0002f2d0: 203d 206d 6178 5f72 756e 6e69 6e67 5f74   = max_running_t
-0002f2e0: 696d 655f 6d69 6e75 7465 730a 2020 2020  ime_minutes.    
-0002f2f0: 2020 2020 7365 6c66 2e77 6f72 6b73 7061      self.workspa
-0002f300: 6365 5f69 6420 3d20 776f 726b 7370 6163  ce_id = workspac
-0002f310: 655f 6964 0a0a 2020 2020 6465 6620 7661  e_id..    def va
-0002f320: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
-0002f330: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
-0002f340: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
-0002f350: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
-0002f360: 2073 7570 6572 2829 2e74 6f5f 6d61 7028   super().to_map(
-0002f370: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
-0002f380: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
-0002f390: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0002f3a0: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
-0002f3b0: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
-0002f3c0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0002f3d0: 6d61 785f 7275 6e6e 696e 675f 7469 6d65  max_running_time
-0002f3e0: 5f6d 696e 7574 6573 2069 7320 6e6f 7420  _minutes is not 
-0002f3f0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0002f400: 2020 7265 7375 6c74 5b27 4d61 7852 756e    result['MaxRun
-0002f410: 6e69 6e67 5469 6d65 4d69 6e75 7465 7327  ningTimeMinutes'
-0002f420: 5d20 3d20 7365 6c66 2e6d 6178 5f72 756e  ] = self.max_run
-0002f430: 6e69 6e67 5f74 696d 655f 6d69 6e75 7465  ning_time_minute
-0002f440: 730a 2020 2020 2020 2020 6966 2073 656c  s.        if sel
-0002f450: 662e 776f 726b 7370 6163 655f 6964 2069  f.workspace_id i
-0002f460: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0002f470: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-0002f480: 576f 726b 7370 6163 6549 6427 5d20 3d20  WorkspaceId'] = 
-0002f490: 7365 6c66 2e77 6f72 6b73 7061 6365 5f69  self.workspace_i
-0002f4a0: 640a 2020 2020 2020 2020 7265 7475 726e  d.        return
-0002f4b0: 2072 6573 756c 740a 0a20 2020 2064 6566   result..    def
-0002f4c0: 2066 726f 6d5f 6d61 7028 7365 6c66 2c20   from_map(self, 
-0002f4d0: 6d3a 2064 6963 7420 3d20 4e6f 6e65 293a  m: dict = None):
-0002f4e0: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
-0002f4f0: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
-0002f500: 2069 6620 6d2e 6765 7428 274d 6178 5275   if m.get('MaxRu
-0002f510: 6e6e 696e 6754 696d 654d 696e 7574 6573  nningTimeMinutes
-0002f520: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-0002f530: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0002f540: 2e6d 6178 5f72 756e 6e69 6e67 5f74 696d  .max_running_tim
-0002f550: 655f 6d69 6e75 7465 7320 3d20 6d2e 6765  e_minutes = m.ge
-0002f560: 7428 274d 6178 5275 6e6e 696e 6754 696d  t('MaxRunningTim
-0002f570: 654d 696e 7574 6573 2729 0a20 2020 2020  eMinutes').     
-0002f580: 2020 2069 6620 6d2e 6765 7428 2757 6f72     if m.get('Wor
-0002f590: 6b73 7061 6365 4964 2729 2069 7320 6e6f  kspaceId') is no
-0002f5a0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0002f5b0: 2020 2020 7365 6c66 2e77 6f72 6b73 7061      self.workspa
-0002f5c0: 6365 5f69 6420 3d20 6d2e 6765 7428 2757  ce_id = m.get('W
-0002f5d0: 6f72 6b73 7061 6365 4964 2729 0a20 2020  orkspaceId').   
-0002f5e0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0002f5f0: 0a0a 0a63 6c61 7373 2055 7064 6174 6554  ...class UpdateT
-0002f600: 656e 736f 7262 6f61 7264 5265 7370 6f6e  ensorboardRespon
-0002f610: 7365 426f 6479 2854 6561 4d6f 6465 6c29  seBody(TeaModel)
-0002f620: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
-0002f630: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
-0002f640: 2c0a 2020 2020 2020 2020 7265 7175 6573  ,.        reques
-0002f650: 745f 6964 3a20 7374 7220 3d20 4e6f 6e65  t_id: str = None
-0002f660: 2c0a 2020 2020 2020 2020 7465 6e73 6f72  ,.        tensor
-0002f670: 626f 6172 645f 6964 3a20 7374 7220 3d20  board_id: str = 
-0002f680: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
-0002f690: 2020 2020 2073 656c 662e 7265 7175 6573       self.reques
-0002f6a0: 745f 6964 203d 2072 6571 7565 7374 5f69  t_id = request_i
-0002f6b0: 640a 2020 2020 2020 2020 7365 6c66 2e74  d.        self.t
-0002f6c0: 656e 736f 7262 6f61 7264 5f69 6420 3d20  ensorboard_id = 
-0002f6d0: 7465 6e73 6f72 626f 6172 645f 6964 0a0a  tensorboard_id..
-0002f6e0: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
-0002f6f0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0002f700: 7061 7373 0a0a 2020 2020 6465 6620 746f  pass..    def to
-0002f710: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
-0002f720: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
-0002f730: 2829 2e74 6f5f 6d61 7028 290a 2020 2020  ().to_map().    
-0002f740: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
-0002f750: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0002f760: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
-0002f770: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
-0002f780: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
-0002f790: 2020 6966 2073 656c 662e 7265 7175 6573    if self.reques
-0002f7a0: 745f 6964 2069 7320 6e6f 7420 4e6f 6e65  t_id is not None
-0002f7b0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0002f7c0: 7375 6c74 5b27 5265 7175 6573 7449 6427  sult['RequestId'
-0002f7d0: 5d20 3d20 7365 6c66 2e72 6571 7565 7374  ] = self.request
-0002f7e0: 5f69 640a 2020 2020 2020 2020 6966 2073  _id.        if s
-0002f7f0: 656c 662e 7465 6e73 6f72 626f 6172 645f  elf.tensorboard_
-0002f800: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
-0002f810: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-0002f820: 6c74 5b27 5465 6e73 6f72 626f 6172 6449  lt['TensorboardI
-0002f830: 6427 5d20 3d20 7365 6c66 2e74 656e 736f  d'] = self.tenso
-0002f840: 7262 6f61 7264 5f69 640a 2020 2020 2020  rboard_id.      
-0002f850: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
-0002f860: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
-0002f870: 7028 7365 6c66 2c20 6d3a 2064 6963 7420  p(self, m: dict 
-0002f880: 3d20 4e6f 6e65 293a 0a20 2020 2020 2020  = None):.       
-0002f890: 206d 203d 206d 206f 7220 6469 6374 2829   m = m or dict()
-0002f8a0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-0002f8b0: 7428 2752 6571 7565 7374 4964 2729 2069  t('RequestId') i
-0002f8c0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0002f8d0: 2020 2020 2020 2020 7365 6c66 2e72 6571          self.req
-0002f8e0: 7565 7374 5f69 6420 3d20 6d2e 6765 7428  uest_id = m.get(
-0002f8f0: 2752 6571 7565 7374 4964 2729 0a20 2020  'RequestId').   
-0002f900: 2020 2020 2069 6620 6d2e 6765 7428 2754       if m.get('T
-0002f910: 656e 736f 7262 6f61 7264 4964 2729 2069  ensorboardId') i
-0002f920: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0002f930: 2020 2020 2020 2020 7365 6c66 2e74 656e          self.ten
-0002f940: 736f 7262 6f61 7264 5f69 6420 3d20 6d2e  sorboard_id = m.
-0002f950: 6765 7428 2754 656e 736f 7262 6f61 7264  get('Tensorboard
-0002f960: 4964 2729 0a20 2020 2020 2020 2072 6574  Id').        ret
-0002f970: 7572 6e20 7365 6c66 0a0a 0a63 6c61 7373  urn self...class
-0002f980: 2055 7064 6174 6554 656e 736f 7262 6f61   UpdateTensorboa
-0002f990: 7264 5265 7370 6f6e 7365 2854 6561 4d6f  rdResponse(TeaMo
-0002f9a0: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
-0002f9b0: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
-0002f9c0: 7365 6c66 2c0a 2020 2020 2020 2020 6865  self,.        he
-0002f9d0: 6164 6572 733a 2044 6963 745b 7374 722c  aders: Dict[str,
-0002f9e0: 2073 7472 5d20 3d20 4e6f 6e65 2c0a 2020   str] = None,.  
-0002f9f0: 2020 2020 2020 7374 6174 7573 5f63 6f64        status_cod
-0002fa00: 653a 2069 6e74 203d 204e 6f6e 652c 0a20  e: int = None,. 
-0002fa10: 2020 2020 2020 2062 6f64 793a 2055 7064         body: Upd
-0002fa20: 6174 6554 656e 736f 7262 6f61 7264 5265  ateTensorboardRe
-0002fa30: 7370 6f6e 7365 426f 6479 203d 204e 6f6e  sponseBody = Non
-0002fa40: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
-0002fa50: 2020 7365 6c66 2e68 6561 6465 7273 203d    self.headers =
-0002fa60: 2068 6561 6465 7273 0a20 2020 2020 2020   headers.       
-0002fa70: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
-0002fa80: 6520 3d20 7374 6174 7573 5f63 6f64 650a  e = status_code.
-0002fa90: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
-0002faa0: 7920 3d20 626f 6479 0a0a 2020 2020 6465  y = body..    de
-0002fab0: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
-0002fac0: 3a0a 2020 2020 2020 2020 7365 6c66 2e76  :.        self.v
-0002fad0: 616c 6964 6174 655f 7265 7175 6972 6564  alidate_required
-0002fae0: 2873 656c 662e 6865 6164 6572 732c 2027  (self.headers, '
-0002faf0: 6865 6164 6572 7327 290a 2020 2020 2020  headers').      
-0002fb00: 2020 7365 6c66 2e76 616c 6964 6174 655f    self.validate_
-0002fb10: 7265 7175 6972 6564 2873 656c 662e 7374  required(self.st
-0002fb20: 6174 7573 5f63 6f64 652c 2027 7374 6174  atus_code, 'stat
-0002fb30: 7573 5f63 6f64 6527 290a 2020 2020 2020  us_code').      
-0002fb40: 2020 7365 6c66 2e76 616c 6964 6174 655f    self.validate_
-0002fb50: 7265 7175 6972 6564 2873 656c 662e 626f  required(self.bo
-0002fb60: 6479 2c20 2762 6f64 7927 290a 2020 2020  dy, 'body').    
-0002fb70: 2020 2020 6966 2073 656c 662e 626f 6479      if self.body
-0002fb80: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0002fb90: 6c66 2e62 6f64 792e 7661 6c69 6461 7465  lf.body.validate
-0002fba0: 2829 0a0a 2020 2020 6465 6620 746f 5f6d  ()..    def to_m
-0002fbb0: 6170 2873 656c 6629 3a0a 2020 2020 2020  ap(self):.      
-0002fbc0: 2020 5f6d 6170 203d 2073 7570 6572 2829    _map = super()
-0002fbd0: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
-0002fbe0: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
-0002fbf0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0002fc00: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
-0002fc10: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
-0002fc20: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-0002fc30: 6966 2073 656c 662e 6865 6164 6572 7320  if self.headers 
-0002fc40: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0002fc50: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-0002fc60: 2768 6561 6465 7273 275d 203d 2073 656c  'headers'] = sel
-0002fc70: 662e 6865 6164 6572 730a 2020 2020 2020  f.headers.      
-0002fc80: 2020 6966 2073 656c 662e 7374 6174 7573    if self.status
-0002fc90: 5f63 6f64 6520 6973 206e 6f74 204e 6f6e  _code is not Non
-0002fca0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-0002fcb0: 6573 756c 745b 2773 7461 7475 7343 6f64  esult['statusCod
-0002fcc0: 6527 5d20 3d20 7365 6c66 2e73 7461 7475  e'] = self.statu
-0002fcd0: 735f 636f 6465 0a20 2020 2020 2020 2069  s_code.        i
-0002fce0: 6620 7365 6c66 2e62 6f64 7920 6973 206e  f self.body is n
-0002fcf0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0002fd00: 2020 2020 2072 6573 756c 745b 2762 6f64       result['bod
-0002fd10: 7927 5d20 3d20 7365 6c66 2e62 6f64 792e  y'] = self.body.
-0002fd20: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
-0002fd30: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
-0002fd40: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
-0002fd50: 2873 656c 662c 206d 3a20 6469 6374 203d  (self, m: dict =
-0002fd60: 204e 6f6e 6529 3a0a 2020 2020 2020 2020   None):.        
-0002fd70: 6d20 3d20 6d20 6f72 2064 6963 7428 290a  m = m or dict().
-0002fd80: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-0002fd90: 2827 6865 6164 6572 7327 2920 6973 206e  ('headers') is n
-0002fda0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0002fdb0: 2020 2020 2073 656c 662e 6865 6164 6572       self.header
-0002fdc0: 7320 3d20 6d2e 6765 7428 2768 6561 6465  s = m.get('heade
-0002fdd0: 7273 2729 0a20 2020 2020 2020 2069 6620  rs').        if 
-0002fde0: 6d2e 6765 7428 2773 7461 7475 7343 6f64  m.get('statusCod
-0002fdf0: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
-0002fe00: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0002fe10: 662e 7374 6174 7573 5f63 6f64 6520 3d20  f.status_code = 
-0002fe20: 6d2e 6765 7428 2773 7461 7475 7343 6f64  m.get('statusCod
-0002fe30: 6527 290a 2020 2020 2020 2020 6966 206d  e').        if m
-0002fe40: 2e67 6574 2827 626f 6479 2729 2069 7320  .get('body') is 
-0002fe50: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0002fe60: 2020 2020 2020 7465 6d70 5f6d 6f64 656c        temp_model
-0002fe70: 203d 2055 7064 6174 6554 656e 736f 7262   = UpdateTensorb
-0002fe80: 6f61 7264 5265 7370 6f6e 7365 426f 6479  oardResponseBody
-0002fe90: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
-0002fea0: 656c 662e 626f 6479 203d 2074 656d 705f  elf.body = temp_
-0002feb0: 6d6f 6465 6c2e 6672 6f6d 5f6d 6170 286d  model.from_map(m
-0002fec0: 5b27 626f 6479 275d 290a 2020 2020 2020  ['body']).      
-0002fed0: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
+00026ca0: 0a0a 636c 6173 7320 4765 7457 6562 5465  ..class GetWebTe
+00026cb0: 726d 696e 616c 5265 7175 6573 7428 5465  rminalRequest(Te
+00026cc0: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
+00026cd0: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
+00026ce0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+00026cf0: 2070 6f64 5f75 6964 3a20 7374 7220 3d20   pod_uid: str = 
+00026d00: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
+00026d10: 2020 2020 2023 2050 6f64 2055 4944 e380       # Pod UID..
+00026d20: 820a 2020 2020 2020 2020 7365 6c66 2e70  ..        self.p
+00026d30: 6f64 5f75 6964 203d 2070 6f64 5f75 6964  od_uid = pod_uid
+00026d40: 0a0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
+00026d50: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
+00026d60: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
+00026d70: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
+00026d80: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
+00026d90: 6572 2829 2e74 6f5f 6d61 7028 290a 2020  er().to_map().  
+00026da0: 2020 2020 2020 6966 205f 6d61 7020 6973        if _map is
+00026db0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00026dc0: 2020 2020 2020 2072 6574 7572 6e20 5f6d         return _m
+00026dd0: 6170 0a0a 2020 2020 2020 2020 7265 7375  ap..        resu
+00026de0: 6c74 203d 2064 6963 7428 290a 2020 2020  lt = dict().    
+00026df0: 2020 2020 6966 2073 656c 662e 706f 645f      if self.pod_
+00026e00: 7569 6420 6973 206e 6f74 204e 6f6e 653a  uid is not None:
+00026e10: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00026e20: 756c 745b 2750 6f64 5569 6427 5d20 3d20  ult['PodUid'] = 
+00026e30: 7365 6c66 2e70 6f64 5f75 6964 0a20 2020  self.pod_uid.   
+00026e40: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
+00026e50: 6c74 0a0a 2020 2020 6465 6620 6672 6f6d  lt..    def from
+00026e60: 5f6d 6170 2873 656c 662c 206d 3a20 6469  _map(self, m: di
+00026e70: 6374 203d 204e 6f6e 6529 3a0a 2020 2020  ct = None):.    
+00026e80: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
+00026e90: 7428 290a 2020 2020 2020 2020 6966 206d  t().        if m
+00026ea0: 2e67 6574 2827 506f 6455 6964 2729 2069  .get('PodUid') i
+00026eb0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00026ec0: 2020 2020 2020 2020 7365 6c66 2e70 6f64          self.pod
+00026ed0: 5f75 6964 203d 206d 2e67 6574 2827 506f  _uid = m.get('Po
+00026ee0: 6455 6964 2729 0a20 2020 2020 2020 2072  dUid').        r
+00026ef0: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
+00026f00: 7373 2047 6574 5765 6254 6572 6d69 6e61  ss GetWebTermina
+00026f10: 6c52 6573 706f 6e73 6542 6f64 7928 5465  lResponseBody(Te
+00026f20: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
+00026f30: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
+00026f40: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+00026f50: 2075 726c 3a20 7374 7220 3d20 4e6f 6e65   url: str = None
+00026f60: 2c0a 2020 2020 2020 2020 7265 7175 6573  ,.        reques
+00026f70: 745f 6964 3a20 7374 7220 3d20 4e6f 6e65  t_id: str = None
+00026f80: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
+00026f90: 2073 656c 662e 7572 6c20 3d20 7572 6c0a   self.url = url.
+00026fa0: 2020 2020 2020 2020 7365 6c66 2e72 6571          self.req
+00026fb0: 7565 7374 5f69 6420 3d20 7265 7175 6573  uest_id = reques
+00026fc0: 745f 6964 0a0a 2020 2020 6465 6620 7661  t_id..    def va
+00026fd0: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
+00026fe0: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
+00026ff0: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
+00027000: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
+00027010: 2073 7570 6572 2829 2e74 6f5f 6d61 7028   super().to_map(
+00027020: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
+00027030: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
+00027040: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00027050: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
+00027060: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
+00027070: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00027080: 7572 6c20 6973 206e 6f74 204e 6f6e 653a  url is not None:
+00027090: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+000270a0: 756c 745b 2755 524c 275d 203d 2073 656c  ult['URL'] = sel
+000270b0: 662e 7572 6c0a 2020 2020 2020 2020 6966  f.url.        if
+000270c0: 2073 656c 662e 7265 7175 6573 745f 6964   self.request_id
+000270d0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000270e0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+000270f0: 5b27 7265 7175 6573 7449 6427 5d20 3d20  ['requestId'] = 
+00027100: 7365 6c66 2e72 6571 7565 7374 5f69 640a  self.request_id.
+00027110: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+00027120: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
+00027130: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3a  rom_map(self, m:
+00027140: 2064 6963 7420 3d20 4e6f 6e65 293a 0a20   dict = None):. 
+00027150: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
+00027160: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+00027170: 6620 6d2e 6765 7428 2755 524c 2729 2069  f m.get('URL') i
+00027180: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00027190: 2020 2020 2020 2020 7365 6c66 2e75 726c          self.url
+000271a0: 203d 206d 2e67 6574 2827 5552 4c27 290a   = m.get('URL').
+000271b0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+000271c0: 2827 7265 7175 6573 7449 6427 2920 6973  ('requestId') is
+000271d0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000271e0: 2020 2020 2020 2073 656c 662e 7265 7175         self.requ
+000271f0: 6573 745f 6964 203d 206d 2e67 6574 2827  est_id = m.get('
+00027200: 7265 7175 6573 7449 6427 290a 2020 2020  requestId').    
+00027210: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
+00027220: 0a0a 636c 6173 7320 4765 7457 6562 5465  ..class GetWebTe
+00027230: 726d 696e 616c 5265 7370 6f6e 7365 2854  rminalResponse(T
+00027240: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
+00027250: 6620 5f5f 696e 6974 5f5f 280a 2020 2020  f __init__(.    
+00027260: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+00027270: 2020 6865 6164 6572 733a 2044 6963 745b    headers: Dict[
+00027280: 7374 722c 2073 7472 5d20 3d20 4e6f 6e65  str, str] = None
+00027290: 2c0a 2020 2020 2020 2020 7374 6174 7573  ,.        status
+000272a0: 5f63 6f64 653a 2069 6e74 203d 204e 6f6e  _code: int = Non
+000272b0: 652c 0a20 2020 2020 2020 2062 6f64 793a  e,.        body:
+000272c0: 2047 6574 5765 6254 6572 6d69 6e61 6c52   GetWebTerminalR
+000272d0: 6573 706f 6e73 6542 6f64 7920 3d20 4e6f  esponseBody = No
+000272e0: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
+000272f0: 2020 2073 656c 662e 6865 6164 6572 7320     self.headers 
+00027300: 3d20 6865 6164 6572 730a 2020 2020 2020  = headers.      
+00027310: 2020 7365 6c66 2e73 7461 7475 735f 636f    self.status_co
+00027320: 6465 203d 2073 7461 7475 735f 636f 6465  de = status_code
+00027330: 0a20 2020 2020 2020 2073 656c 662e 626f  .        self.bo
+00027340: 6479 203d 2062 6f64 790a 0a20 2020 2064  dy = body..    d
+00027350: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
+00027360: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+00027370: 7661 6c69 6461 7465 5f72 6571 7569 7265  validate_require
+00027380: 6428 7365 6c66 2e68 6561 6465 7273 2c20  d(self.headers, 
+00027390: 2768 6561 6465 7273 2729 0a20 2020 2020  'headers').     
+000273a0: 2020 2073 656c 662e 7661 6c69 6461 7465     self.validate
+000273b0: 5f72 6571 7569 7265 6428 7365 6c66 2e73  _required(self.s
+000273c0: 7461 7475 735f 636f 6465 2c20 2773 7461  tatus_code, 'sta
+000273d0: 7475 735f 636f 6465 2729 0a20 2020 2020  tus_code').     
+000273e0: 2020 2073 656c 662e 7661 6c69 6461 7465     self.validate
+000273f0: 5f72 6571 7569 7265 6428 7365 6c66 2e62  _required(self.b
+00027400: 6f64 792c 2027 626f 6479 2729 0a20 2020  ody, 'body').   
+00027410: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
+00027420: 793a 0a20 2020 2020 2020 2020 2020 2073  y:.            s
+00027430: 656c 662e 626f 6479 2e76 616c 6964 6174  elf.body.validat
+00027440: 6528 290a 0a20 2020 2064 6566 2074 6f5f  e()..    def to_
+00027450: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
+00027460: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
+00027470: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
+00027480: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
+00027490: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000274a0: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
+000274b0: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
+000274c0: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
+000274d0: 2069 6620 7365 6c66 2e68 6561 6465 7273   if self.headers
+000274e0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000274f0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00027500: 5b27 6865 6164 6572 7327 5d20 3d20 7365  ['headers'] = se
+00027510: 6c66 2e68 6561 6465 7273 0a20 2020 2020  lf.headers.     
+00027520: 2020 2069 6620 7365 6c66 2e73 7461 7475     if self.statu
+00027530: 735f 636f 6465 2069 7320 6e6f 7420 4e6f  s_code is not No
+00027540: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00027550: 7265 7375 6c74 5b27 7374 6174 7573 436f  result['statusCo
+00027560: 6465 275d 203d 2073 656c 662e 7374 6174  de'] = self.stat
+00027570: 7573 5f63 6f64 650a 2020 2020 2020 2020  us_code.        
+00027580: 6966 2073 656c 662e 626f 6479 2069 7320  if self.body is 
+00027590: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000275a0: 2020 2020 2020 7265 7375 6c74 5b27 626f        result['bo
+000275b0: 6479 275d 203d 2073 656c 662e 626f 6479  dy'] = self.body
+000275c0: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
+000275d0: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
+000275e0: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
+000275f0: 7028 7365 6c66 2c20 6d3a 2064 6963 7420  p(self, m: dict 
+00027600: 3d20 4e6f 6e65 293a 0a20 2020 2020 2020  = None):.       
+00027610: 206d 203d 206d 206f 7220 6469 6374 2829   m = m or dict()
+00027620: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00027630: 7428 2768 6561 6465 7273 2729 2069 7320  t('headers') is 
+00027640: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00027650: 2020 2020 2020 7365 6c66 2e68 6561 6465        self.heade
+00027660: 7273 203d 206d 2e67 6574 2827 6865 6164  rs = m.get('head
+00027670: 6572 7327 290a 2020 2020 2020 2020 6966  ers').        if
+00027680: 206d 2e67 6574 2827 7374 6174 7573 436f   m.get('statusCo
+00027690: 6465 2729 2069 7320 6e6f 7420 4e6f 6e65  de') is not None
+000276a0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+000276b0: 6c66 2e73 7461 7475 735f 636f 6465 203d  lf.status_code =
+000276c0: 206d 2e67 6574 2827 7374 6174 7573 436f   m.get('statusCo
+000276d0: 6465 2729 0a20 2020 2020 2020 2069 6620  de').        if 
+000276e0: 6d2e 6765 7428 2762 6f64 7927 2920 6973  m.get('body') is
+000276f0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00027700: 2020 2020 2020 2074 656d 705f 6d6f 6465         temp_mode
+00027710: 6c20 3d20 4765 7457 6562 5465 726d 696e  l = GetWebTermin
+00027720: 616c 5265 7370 6f6e 7365 426f 6479 2829  alResponseBody()
+00027730: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00027740: 662e 626f 6479 203d 2074 656d 705f 6d6f  f.body = temp_mo
+00027750: 6465 6c2e 6672 6f6d 5f6d 6170 286d 5b27  del.from_map(m['
+00027760: 626f 6479 275d 290a 2020 2020 2020 2020  body']).        
+00027770: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
+00027780: 6173 7320 4c69 7374 4563 7353 7065 6373  ass ListEcsSpecs
+00027790: 5265 7175 6573 7428 5465 614d 6f64 656c  Request(TeaModel
+000277a0: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
+000277b0: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
+000277c0: 662c 0a20 2020 2020 2020 2061 6363 656c  f,.        accel
+000277d0: 6572 6174 6f72 5f74 7970 653a 2073 7472  erator_type: str
+000277e0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+000277f0: 206f 7264 6572 3a20 7374 7220 3d20 4e6f   order: str = No
+00027800: 6e65 2c0a 2020 2020 2020 2020 7061 6765  ne,.        page
+00027810: 5f6e 756d 6265 723a 2069 6e74 203d 204e  _number: int = N
+00027820: 6f6e 652c 0a20 2020 2020 2020 2070 6167  one,.        pag
+00027830: 655f 7369 7a65 3a20 696e 7420 3d20 4e6f  e_size: int = No
+00027840: 6e65 2c0a 2020 2020 2020 2020 736f 7274  ne,.        sort
+00027850: 5f62 793a 2073 7472 203d 204e 6f6e 652c  _by: str = None,
+00027860: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
+00027870: 7365 6c66 2e61 6363 656c 6572 6174 6f72  self.accelerator
+00027880: 5f74 7970 6520 3d20 6163 6365 6c65 7261  _type = accelera
+00027890: 746f 725f 7479 7065 0a20 2020 2020 2020  tor_type.       
+000278a0: 2073 656c 662e 6f72 6465 7220 3d20 6f72   self.order = or
+000278b0: 6465 720a 2020 2020 2020 2020 7365 6c66  der.        self
+000278c0: 2e70 6167 655f 6e75 6d62 6572 203d 2070  .page_number = p
+000278d0: 6167 655f 6e75 6d62 6572 0a20 2020 2020  age_number.     
+000278e0: 2020 2073 656c 662e 7061 6765 5f73 697a     self.page_siz
+000278f0: 6520 3d20 7061 6765 5f73 697a 650a 2020  e = page_size.  
+00027900: 2020 2020 2020 7365 6c66 2e73 6f72 745f        self.sort_
+00027910: 6279 203d 2073 6f72 745f 6279 0a0a 2020  by = sort_by..  
+00027920: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
+00027930: 656c 6629 3a0a 2020 2020 2020 2020 7061  elf):.        pa
+00027940: 7373 0a0a 2020 2020 6465 6620 746f 5f6d  ss..    def to_m
+00027950: 6170 2873 656c 6629 3a0a 2020 2020 2020  ap(self):.      
+00027960: 2020 5f6d 6170 203d 2073 7570 6572 2829    _map = super()
+00027970: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
+00027980: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
+00027990: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000279a0: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
+000279b0: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+000279c0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+000279d0: 6966 2073 656c 662e 6163 6365 6c65 7261  if self.accelera
+000279e0: 746f 725f 7479 7065 2069 7320 6e6f 7420  tor_type is not 
+000279f0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00027a00: 2020 7265 7375 6c74 5b27 4163 6365 6c65    result['Accele
+00027a10: 7261 746f 7254 7970 6527 5d20 3d20 7365  ratorType'] = se
+00027a20: 6c66 2e61 6363 656c 6572 6174 6f72 5f74  lf.accelerator_t
+00027a30: 7970 650a 2020 2020 2020 2020 6966 2073  ype.        if s
+00027a40: 656c 662e 6f72 6465 7220 6973 206e 6f74  elf.order is not
+00027a50: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00027a60: 2020 2072 6573 756c 745b 274f 7264 6572     result['Order
+00027a70: 275d 203d 2073 656c 662e 6f72 6465 720a  '] = self.order.
+00027a80: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00027a90: 7061 6765 5f6e 756d 6265 7220 6973 206e  page_number is n
+00027aa0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00027ab0: 2020 2020 2072 6573 756c 745b 2750 6167       result['Pag
+00027ac0: 654e 756d 6265 7227 5d20 3d20 7365 6c66  eNumber'] = self
+00027ad0: 2e70 6167 655f 6e75 6d62 6572 0a20 2020  .page_number.   
+00027ae0: 2020 2020 2069 6620 7365 6c66 2e70 6167       if self.pag
+00027af0: 655f 7369 7a65 2069 7320 6e6f 7420 4e6f  e_size is not No
+00027b00: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00027b10: 7265 7375 6c74 5b27 5061 6765 5369 7a65  result['PageSize
+00027b20: 275d 203d 2073 656c 662e 7061 6765 5f73  '] = self.page_s
+00027b30: 697a 650a 2020 2020 2020 2020 6966 2073  ize.        if s
+00027b40: 656c 662e 736f 7274 5f62 7920 6973 206e  elf.sort_by is n
+00027b50: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00027b60: 2020 2020 2072 6573 756c 745b 2753 6f72       result['Sor
+00027b70: 7442 7927 5d20 3d20 7365 6c66 2e73 6f72  tBy'] = self.sor
+00027b80: 745f 6279 0a20 2020 2020 2020 2072 6574  t_by.        ret
+00027b90: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
+00027ba0: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
+00027bb0: 662c 206d 3a20 6469 6374 203d 204e 6f6e  f, m: dict = Non
+00027bc0: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
+00027bd0: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
+00027be0: 2020 2020 6966 206d 2e67 6574 2827 4163      if m.get('Ac
+00027bf0: 6365 6c65 7261 746f 7254 7970 6527 2920  celeratorType') 
+00027c00: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00027c10: 2020 2020 2020 2020 2073 656c 662e 6163           self.ac
+00027c20: 6365 6c65 7261 746f 725f 7479 7065 203d  celerator_type =
+00027c30: 206d 2e67 6574 2827 4163 6365 6c65 7261   m.get('Accelera
+00027c40: 746f 7254 7970 6527 290a 2020 2020 2020  torType').      
+00027c50: 2020 6966 206d 2e67 6574 2827 4f72 6465    if m.get('Orde
+00027c60: 7227 2920 6973 206e 6f74 204e 6f6e 653a  r') is not None:
+00027c70: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00027c80: 662e 6f72 6465 7220 3d20 6d2e 6765 7428  f.order = m.get(
+00027c90: 274f 7264 6572 2729 0a20 2020 2020 2020  'Order').       
+00027ca0: 2069 6620 6d2e 6765 7428 2750 6167 654e   if m.get('PageN
+00027cb0: 756d 6265 7227 2920 6973 206e 6f74 204e  umber') is not N
+00027cc0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00027cd0: 2073 656c 662e 7061 6765 5f6e 756d 6265   self.page_numbe
+00027ce0: 7220 3d20 6d2e 6765 7428 2750 6167 654e  r = m.get('PageN
+00027cf0: 756d 6265 7227 290a 2020 2020 2020 2020  umber').        
+00027d00: 6966 206d 2e67 6574 2827 5061 6765 5369  if m.get('PageSi
+00027d10: 7a65 2729 2069 7320 6e6f 7420 4e6f 6e65  ze') is not None
+00027d20: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00027d30: 6c66 2e70 6167 655f 7369 7a65 203d 206d  lf.page_size = m
+00027d40: 2e67 6574 2827 5061 6765 5369 7a65 2729  .get('PageSize')
+00027d50: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00027d60: 7428 2753 6f72 7442 7927 2920 6973 206e  t('SortBy') is n
+00027d70: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00027d80: 2020 2020 2073 656c 662e 736f 7274 5f62       self.sort_b
+00027d90: 7920 3d20 6d2e 6765 7428 2753 6f72 7442  y = m.get('SortB
+00027da0: 7927 290a 2020 2020 2020 2020 7265 7475  y').        retu
+00027db0: 726e 2073 656c 660a 0a0a 636c 6173 7320  rn self...class 
+00027dc0: 4c69 7374 4563 7353 7065 6373 5265 7370  ListEcsSpecsResp
+00027dd0: 6f6e 7365 426f 6479 2854 6561 4d6f 6465  onseBody(TeaMode
+00027de0: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
+00027df0: 6974 5f5f 280a 2020 2020 2020 2020 7365  it__(.        se
+00027e00: 6c66 2c0a 2020 2020 2020 2020 6563 735f  lf,.        ecs_
+00027e10: 7370 6563 733a 204c 6973 745b 4563 7353  specs: List[EcsS
+00027e20: 7065 635d 203d 204e 6f6e 652c 0a20 2020  pec] = None,.   
+00027e30: 2020 2020 2072 6571 7565 7374 5f69 643a       request_id:
+00027e40: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+00027e50: 2020 2020 2074 6f74 616c 5f63 6f75 6e74       total_count
+00027e60: 3a20 696e 7420 3d20 4e6f 6e65 2c0a 2020  : int = None,.  
+00027e70: 2020 293a 0a20 2020 2020 2020 2073 656c    ):.        sel
+00027e80: 662e 6563 735f 7370 6563 7320 3d20 6563  f.ecs_specs = ec
+00027e90: 735f 7370 6563 730a 2020 2020 2020 2020  s_specs.        
+00027ea0: 7365 6c66 2e72 6571 7565 7374 5f69 6420  self.request_id 
+00027eb0: 3d20 7265 7175 6573 745f 6964 0a20 2020  = request_id.   
+00027ec0: 2020 2020 2073 656c 662e 746f 7461 6c5f       self.total_
+00027ed0: 636f 756e 7420 3d20 746f 7461 6c5f 636f  count = total_co
+00027ee0: 756e 740a 0a20 2020 2064 6566 2076 616c  unt..    def val
+00027ef0: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
+00027f00: 2020 2020 2069 6620 7365 6c66 2e65 6373       if self.ecs
+00027f10: 5f73 7065 6373 3a0a 2020 2020 2020 2020  _specs:.        
+00027f20: 2020 2020 666f 7220 6b20 696e 2073 656c      for k in sel
+00027f30: 662e 6563 735f 7370 6563 733a 0a20 2020  f.ecs_specs:.   
+00027f40: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00027f50: 6b3a 0a20 2020 2020 2020 2020 2020 2020  k:.             
+00027f60: 2020 2020 2020 206b 2e76 616c 6964 6174         k.validat
+00027f70: 6528 290a 0a20 2020 2064 6566 2074 6f5f  e()..    def to_
+00027f80: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
+00027f90: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
+00027fa0: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
+00027fb0: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
+00027fc0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00027fd0: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
+00027fe0: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
+00027ff0: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
+00028000: 2072 6573 756c 745b 2745 6373 5370 6563   result['EcsSpec
+00028010: 7327 5d20 3d20 5b5d 0a20 2020 2020 2020  s'] = [].       
+00028020: 2069 6620 7365 6c66 2e65 6373 5f73 7065   if self.ecs_spe
+00028030: 6373 2069 7320 6e6f 7420 4e6f 6e65 3a0a  cs is not None:.
+00028040: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00028050: 6b20 696e 2073 656c 662e 6563 735f 7370  k in self.ecs_sp
+00028060: 6563 733a 0a20 2020 2020 2020 2020 2020  ecs:.           
+00028070: 2020 2020 2072 6573 756c 745b 2745 6373       result['Ecs
+00028080: 5370 6563 7327 5d2e 6170 7065 6e64 286b  Specs'].append(k
+00028090: 2e74 6f5f 6d61 7028 2920 6966 206b 2065  .to_map() if k e
+000280a0: 6c73 6520 4e6f 6e65 290a 2020 2020 2020  lse None).      
+000280b0: 2020 6966 2073 656c 662e 7265 7175 6573    if self.reques
+000280c0: 745f 6964 2069 7320 6e6f 7420 4e6f 6e65  t_id is not None
+000280d0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+000280e0: 7375 6c74 5b27 5265 7175 6573 7449 6427  sult['RequestId'
+000280f0: 5d20 3d20 7365 6c66 2e72 6571 7565 7374  ] = self.request
+00028100: 5f69 640a 2020 2020 2020 2020 6966 2073  _id.        if s
+00028110: 656c 662e 746f 7461 6c5f 636f 756e 7420  elf.total_count 
+00028120: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00028130: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00028140: 2754 6f74 616c 436f 756e 7427 5d20 3d20  'TotalCount'] = 
+00028150: 7365 6c66 2e74 6f74 616c 5f63 6f75 6e74  self.total_count
+00028160: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00028170: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
+00028180: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
+00028190: 3a20 6469 6374 203d 204e 6f6e 6529 3a0a  : dict = None):.
+000281a0: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
+000281b0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+000281c0: 7365 6c66 2e65 6373 5f73 7065 6373 203d  self.ecs_specs =
+000281d0: 205b 5d0a 2020 2020 2020 2020 6966 206d   [].        if m
+000281e0: 2e67 6574 2827 4563 7353 7065 6373 2729  .get('EcsSpecs')
+000281f0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00028200: 2020 2020 2020 2020 2020 666f 7220 6b20            for k 
+00028210: 696e 206d 2e67 6574 2827 4563 7353 7065  in m.get('EcsSpe
+00028220: 6373 2729 3a0a 2020 2020 2020 2020 2020  cs'):.          
+00028230: 2020 2020 2020 7465 6d70 5f6d 6f64 656c        temp_model
+00028240: 203d 2045 6373 5370 6563 2829 0a20 2020   = EcsSpec().   
+00028250: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00028260: 662e 6563 735f 7370 6563 732e 6170 7065  f.ecs_specs.appe
+00028270: 6e64 2874 656d 705f 6d6f 6465 6c2e 6672  nd(temp_model.fr
+00028280: 6f6d 5f6d 6170 286b 2929 0a20 2020 2020  om_map(k)).     
+00028290: 2020 2069 6620 6d2e 6765 7428 2752 6571     if m.get('Req
+000282a0: 7565 7374 4964 2729 2069 7320 6e6f 7420  uestId') is not 
+000282b0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000282c0: 2020 7365 6c66 2e72 6571 7565 7374 5f69    self.request_i
+000282d0: 6420 3d20 6d2e 6765 7428 2752 6571 7565  d = m.get('Reque
+000282e0: 7374 4964 2729 0a20 2020 2020 2020 2069  stId').        i
+000282f0: 6620 6d2e 6765 7428 2754 6f74 616c 436f  f m.get('TotalCo
+00028300: 756e 7427 2920 6973 206e 6f74 204e 6f6e  unt') is not Non
+00028310: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00028320: 656c 662e 746f 7461 6c5f 636f 756e 7420  elf.total_count 
+00028330: 3d20 6d2e 6765 7428 2754 6f74 616c 436f  = m.get('TotalCo
+00028340: 756e 7427 290a 2020 2020 2020 2020 7265  unt').        re
+00028350: 7475 726e 2073 656c 660a 0a0a 636c 6173  turn self...clas
+00028360: 7320 4c69 7374 4563 7353 7065 6373 5265  s ListEcsSpecsRe
+00028370: 7370 6f6e 7365 2854 6561 4d6f 6465 6c29  sponse(TeaModel)
+00028380: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
+00028390: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
+000283a0: 2c0a 2020 2020 2020 2020 6865 6164 6572  ,.        header
+000283b0: 733a 2044 6963 745b 7374 722c 2073 7472  s: Dict[str, str
+000283c0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+000283d0: 2020 7374 6174 7573 5f63 6f64 653a 2069    status_code: i
+000283e0: 6e74 203d 204e 6f6e 652c 0a20 2020 2020  nt = None,.     
+000283f0: 2020 2062 6f64 793a 204c 6973 7445 6373     body: ListEcs
+00028400: 5370 6563 7352 6573 706f 6e73 6542 6f64  SpecsResponseBod
+00028410: 7920 3d20 4e6f 6e65 2c0a 2020 2020 293a  y = None,.    ):
+00028420: 0a20 2020 2020 2020 2073 656c 662e 6865  .        self.he
+00028430: 6164 6572 7320 3d20 6865 6164 6572 730a  aders = headers.
+00028440: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
+00028450: 7475 735f 636f 6465 203d 2073 7461 7475  tus_code = statu
+00028460: 735f 636f 6465 0a20 2020 2020 2020 2073  s_code.        s
+00028470: 656c 662e 626f 6479 203d 2062 6f64 790a  elf.body = body.
+00028480: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
+00028490: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+000284a0: 2073 656c 662e 7661 6c69 6461 7465 5f72   self.validate_r
+000284b0: 6571 7569 7265 6428 7365 6c66 2e68 6561  equired(self.hea
+000284c0: 6465 7273 2c20 2768 6561 6465 7273 2729  ders, 'headers')
+000284d0: 0a20 2020 2020 2020 2073 656c 662e 7661  .        self.va
+000284e0: 6c69 6461 7465 5f72 6571 7569 7265 6428  lidate_required(
+000284f0: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
+00028500: 2c20 2773 7461 7475 735f 636f 6465 2729  , 'status_code')
+00028510: 0a20 2020 2020 2020 2073 656c 662e 7661  .        self.va
+00028520: 6c69 6461 7465 5f72 6571 7569 7265 6428  lidate_required(
+00028530: 7365 6c66 2e62 6f64 792c 2027 626f 6479  self.body, 'body
+00028540: 2729 0a20 2020 2020 2020 2069 6620 7365  ').        if se
+00028550: 6c66 2e62 6f64 793a 0a20 2020 2020 2020  lf.body:.       
+00028560: 2020 2020 2073 656c 662e 626f 6479 2e76       self.body.v
+00028570: 616c 6964 6174 6528 290a 0a20 2020 2064  alidate()..    d
+00028580: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
+00028590: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
+000285a0: 7375 7065 7228 292e 746f 5f6d 6170 2829  super().to_map()
+000285b0: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
+000285c0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000285d0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000285e0: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
+000285f0: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
+00028600: 2020 2020 2020 2069 6620 7365 6c66 2e68         if self.h
+00028610: 6561 6465 7273 2069 7320 6e6f 7420 4e6f  eaders is not No
+00028620: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00028630: 7265 7375 6c74 5b27 6865 6164 6572 7327  result['headers'
+00028640: 5d20 3d20 7365 6c66 2e68 6561 6465 7273  ] = self.headers
+00028650: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00028660: 2e73 7461 7475 735f 636f 6465 2069 7320  .status_code is 
+00028670: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00028680: 2020 2020 2020 7265 7375 6c74 5b27 7374        result['st
+00028690: 6174 7573 436f 6465 275d 203d 2073 656c  atusCode'] = sel
+000286a0: 662e 7374 6174 7573 5f63 6f64 650a 2020  f.status_code.  
+000286b0: 2020 2020 2020 6966 2073 656c 662e 626f        if self.bo
+000286c0: 6479 2069 7320 6e6f 7420 4e6f 6e65 3a0a  dy is not None:.
+000286d0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+000286e0: 6c74 5b27 626f 6479 275d 203d 2073 656c  lt['body'] = sel
+000286f0: 662e 626f 6479 2e74 6f5f 6d61 7028 290a  f.body.to_map().
+00028700: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+00028710: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
+00028720: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3a  rom_map(self, m:
+00028730: 2064 6963 7420 3d20 4e6f 6e65 293a 0a20   dict = None):. 
+00028740: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
+00028750: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+00028760: 6620 6d2e 6765 7428 2768 6561 6465 7273  f m.get('headers
+00028770: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+00028780: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00028790: 2e68 6561 6465 7273 203d 206d 2e67 6574  .headers = m.get
+000287a0: 2827 6865 6164 6572 7327 290a 2020 2020  ('headers').    
+000287b0: 2020 2020 6966 206d 2e67 6574 2827 7374      if m.get('st
+000287c0: 6174 7573 436f 6465 2729 2069 7320 6e6f  atusCode') is no
+000287d0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000287e0: 2020 2020 7365 6c66 2e73 7461 7475 735f      self.status_
+000287f0: 636f 6465 203d 206d 2e67 6574 2827 7374  code = m.get('st
+00028800: 6174 7573 436f 6465 2729 0a20 2020 2020  atusCode').     
+00028810: 2020 2069 6620 6d2e 6765 7428 2762 6f64     if m.get('bod
+00028820: 7927 2920 6973 206e 6f74 204e 6f6e 653a  y') is not None:
+00028830: 0a20 2020 2020 2020 2020 2020 2074 656d  .            tem
+00028840: 705f 6d6f 6465 6c20 3d20 4c69 7374 4563  p_model = ListEc
+00028850: 7353 7065 6373 5265 7370 6f6e 7365 426f  sSpecsResponseBo
+00028860: 6479 2829 0a20 2020 2020 2020 2020 2020  dy().           
+00028870: 2073 656c 662e 626f 6479 203d 2074 656d   self.body = tem
+00028880: 705f 6d6f 6465 6c2e 6672 6f6d 5f6d 6170  p_model.from_map
+00028890: 286d 5b27 626f 6479 275d 290a 2020 2020  (m['body']).    
+000288a0: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
+000288b0: 0a0a 636c 6173 7320 4c69 7374 4a6f 6273  ..class ListJobs
+000288c0: 5265 7175 6573 7428 5465 614d 6f64 656c  Request(TeaModel
+000288d0: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
+000288e0: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
+000288f0: 662c 0a20 2020 2020 2020 2062 7573 696e  f,.        busin
+00028900: 6573 735f 7573 6572 5f69 643a 2073 7472  ess_user_id: str
+00028910: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+00028920: 2063 616c 6c65 723a 2073 7472 203d 204e   caller: str = N
+00028930: 6f6e 652c 0a20 2020 2020 2020 2064 6973  one,.        dis
+00028940: 706c 6179 5f6e 616d 653a 2073 7472 203d  play_name: str =
+00028950: 204e 6f6e 652c 0a20 2020 2020 2020 2065   None,.        e
+00028960: 6e64 5f74 696d 653a 2073 7472 203d 204e  nd_time: str = N
+00028970: 6f6e 652c 0a20 2020 2020 2020 2066 726f  one,.        fro
+00028980: 6d5f 616c 6c5f 776f 726b 7370 6163 6573  m_all_workspaces
+00028990: 3a20 626f 6f6c 203d 204e 6f6e 652c 0a20  : bool = None,. 
+000289a0: 2020 2020 2020 206a 6f62 5f69 643a 2073         job_id: s
+000289b0: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
+000289c0: 2020 206a 6f62 5f74 7970 653a 2073 7472     job_type: str
+000289d0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+000289e0: 206f 7264 6572 3a20 7374 7220 3d20 4e6f   order: str = No
+000289f0: 6e65 2c0a 2020 2020 2020 2020 7061 6765  ne,.        page
+00028a00: 5f6e 756d 6265 723a 2069 6e74 203d 204e  _number: int = N
+00028a10: 6f6e 652c 0a20 2020 2020 2020 2070 6167  one,.        pag
+00028a20: 655f 7369 7a65 3a20 696e 7420 3d20 4e6f  e_size: int = No
+00028a30: 6e65 2c0a 2020 2020 2020 2020 7069 7065  ne,.        pipe
+00028a40: 6c69 6e65 5f69 643a 2073 7472 203d 204e  line_id: str = N
+00028a50: 6f6e 652c 0a20 2020 2020 2020 2072 6573  one,.        res
+00028a60: 6f75 7263 655f 6964 3a20 7374 7220 3d20  ource_id: str = 
+00028a70: 4e6f 6e65 2c0a 2020 2020 2020 2020 7368  None,.        sh
+00028a80: 6f77 5f6f 776e 3a20 626f 6f6c 203d 204e  ow_own: bool = N
+00028a90: 6f6e 652c 0a20 2020 2020 2020 2073 6f72  one,.        sor
+00028aa0: 745f 6279 3a20 7374 7220 3d20 4e6f 6e65  t_by: str = None
+00028ab0: 2c0a 2020 2020 2020 2020 7374 6172 745f  ,.        start_
+00028ac0: 7469 6d65 3a20 7374 7220 3d20 4e6f 6e65  time: str = None
+00028ad0: 2c0a 2020 2020 2020 2020 7374 6174 7573  ,.        status
+00028ae0: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+00028af0: 2020 2020 2020 7461 6773 3a20 4469 6374        tags: Dict
+00028b00: 5b73 7472 2c20 7374 725d 203d 204e 6f6e  [str, str] = Non
+00028b10: 652c 0a20 2020 2020 2020 2077 6f72 6b73  e,.        works
+00028b20: 7061 6365 5f69 643a 2073 7472 203d 204e  pace_id: str = N
+00028b30: 6f6e 652c 0a20 2020 2029 3a0a 2020 2020  one,.    ):.    
+00028b40: 2020 2020 7365 6c66 2e62 7573 696e 6573      self.busines
+00028b50: 735f 7573 6572 5f69 6420 3d20 6275 7369  s_user_id = busi
+00028b60: 6e65 7373 5f75 7365 725f 6964 0a20 2020  ness_user_id.   
+00028b70: 2020 2020 2073 656c 662e 6361 6c6c 6572       self.caller
+00028b80: 203d 2063 616c 6c65 720a 2020 2020 2020   = caller.      
+00028b90: 2020 7365 6c66 2e64 6973 706c 6179 5f6e    self.display_n
+00028ba0: 616d 6520 3d20 6469 7370 6c61 795f 6e61  ame = display_na
+00028bb0: 6d65 0a20 2020 2020 2020 2073 656c 662e  me.        self.
+00028bc0: 656e 645f 7469 6d65 203d 2065 6e64 5f74  end_time = end_t
+00028bd0: 696d 650a 2020 2020 2020 2020 7365 6c66  ime.        self
+00028be0: 2e66 726f 6d5f 616c 6c5f 776f 726b 7370  .from_all_worksp
+00028bf0: 6163 6573 203d 2066 726f 6d5f 616c 6c5f  aces = from_all_
+00028c00: 776f 726b 7370 6163 6573 0a20 2020 2020  workspaces.     
+00028c10: 2020 2073 656c 662e 6a6f 625f 6964 203d     self.job_id =
+00028c20: 206a 6f62 5f69 640a 2020 2020 2020 2020   job_id.        
+00028c30: 7365 6c66 2e6a 6f62 5f74 7970 6520 3d20  self.job_type = 
+00028c40: 6a6f 625f 7479 7065 0a20 2020 2020 2020  job_type.       
+00028c50: 2073 656c 662e 6f72 6465 7220 3d20 6f72   self.order = or
+00028c60: 6465 720a 2020 2020 2020 2020 7365 6c66  der.        self
+00028c70: 2e70 6167 655f 6e75 6d62 6572 203d 2070  .page_number = p
+00028c80: 6167 655f 6e75 6d62 6572 0a20 2020 2020  age_number.     
+00028c90: 2020 2073 656c 662e 7061 6765 5f73 697a     self.page_siz
+00028ca0: 6520 3d20 7061 6765 5f73 697a 650a 2020  e = page_size.  
+00028cb0: 2020 2020 2020 7365 6c66 2e70 6970 656c        self.pipel
+00028cc0: 696e 655f 6964 203d 2070 6970 656c 696e  ine_id = pipelin
+00028cd0: 655f 6964 0a20 2020 2020 2020 2073 656c  e_id.        sel
+00028ce0: 662e 7265 736f 7572 6365 5f69 6420 3d20  f.resource_id = 
+00028cf0: 7265 736f 7572 6365 5f69 640a 2020 2020  resource_id.    
+00028d00: 2020 2020 7365 6c66 2e73 686f 775f 6f77      self.show_ow
+00028d10: 6e20 3d20 7368 6f77 5f6f 776e 0a20 2020  n = show_own.   
+00028d20: 2020 2020 2073 656c 662e 736f 7274 5f62       self.sort_b
+00028d30: 7920 3d20 736f 7274 5f62 790a 2020 2020  y = sort_by.    
+00028d40: 2020 2020 7365 6c66 2e73 7461 7274 5f74      self.start_t
+00028d50: 696d 6520 3d20 7374 6172 745f 7469 6d65  ime = start_time
+00028d60: 0a20 2020 2020 2020 2073 656c 662e 7374  .        self.st
+00028d70: 6174 7573 203d 2073 7461 7475 730a 2020  atus = status.  
+00028d80: 2020 2020 2020 7365 6c66 2e74 6167 7320        self.tags 
+00028d90: 3d20 7461 6773 0a20 2020 2020 2020 2073  = tags.        s
+00028da0: 656c 662e 776f 726b 7370 6163 655f 6964  elf.workspace_id
+00028db0: 203d 2077 6f72 6b73 7061 6365 5f69 640a   = workspace_id.
+00028dc0: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
+00028dd0: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+00028de0: 2070 6173 730a 0a20 2020 2064 6566 2074   pass..    def t
+00028df0: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
+00028e00: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
+00028e10: 7228 292e 746f 5f6d 6170 2829 0a20 2020  r().to_map().   
+00028e20: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
+00028e30: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00028e40: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
+00028e50: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
+00028e60: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
+00028e70: 2020 2069 6620 7365 6c66 2e62 7573 696e     if self.busin
+00028e80: 6573 735f 7573 6572 5f69 6420 6973 206e  ess_user_id is n
+00028e90: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00028ea0: 2020 2020 2072 6573 756c 745b 2742 7573       result['Bus
+00028eb0: 696e 6573 7355 7365 7249 6427 5d20 3d20  inessUserId'] = 
+00028ec0: 7365 6c66 2e62 7573 696e 6573 735f 7573  self.business_us
+00028ed0: 6572 5f69 640a 2020 2020 2020 2020 6966  er_id.        if
+00028ee0: 2073 656c 662e 6361 6c6c 6572 2069 7320   self.caller is 
+00028ef0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00028f00: 2020 2020 2020 7265 7375 6c74 5b27 4361        result['Ca
+00028f10: 6c6c 6572 275d 203d 2073 656c 662e 6361  ller'] = self.ca
+00028f20: 6c6c 6572 0a20 2020 2020 2020 2069 6620  ller.        if 
+00028f30: 7365 6c66 2e64 6973 706c 6179 5f6e 616d  self.display_nam
+00028f40: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
+00028f50: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00028f60: 745b 2744 6973 706c 6179 4e61 6d65 275d  t['DisplayName']
+00028f70: 203d 2073 656c 662e 6469 7370 6c61 795f   = self.display_
+00028f80: 6e61 6d65 0a20 2020 2020 2020 2069 6620  name.        if 
+00028f90: 7365 6c66 2e65 6e64 5f74 696d 6520 6973  self.end_time is
+00028fa0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00028fb0: 2020 2020 2020 2072 6573 756c 745b 2745         result['E
+00028fc0: 6e64 5469 6d65 275d 203d 2073 656c 662e  ndTime'] = self.
+00028fd0: 656e 645f 7469 6d65 0a20 2020 2020 2020  end_time.       
+00028fe0: 2069 6620 7365 6c66 2e66 726f 6d5f 616c   if self.from_al
+00028ff0: 6c5f 776f 726b 7370 6163 6573 2069 7320  l_workspaces is 
+00029000: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00029010: 2020 2020 2020 7265 7375 6c74 5b27 4672        result['Fr
+00029020: 6f6d 416c 6c57 6f72 6b73 7061 6365 7327  omAllWorkspaces'
+00029030: 5d20 3d20 7365 6c66 2e66 726f 6d5f 616c  ] = self.from_al
+00029040: 6c5f 776f 726b 7370 6163 6573 0a20 2020  l_workspaces.   
+00029050: 2020 2020 2069 6620 7365 6c66 2e6a 6f62       if self.job
+00029060: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
+00029070: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00029080: 756c 745b 274a 6f62 4964 275d 203d 2073  ult['JobId'] = s
+00029090: 656c 662e 6a6f 625f 6964 0a20 2020 2020  elf.job_id.     
+000290a0: 2020 2069 6620 7365 6c66 2e6a 6f62 5f74     if self.job_t
+000290b0: 7970 6520 6973 206e 6f74 204e 6f6e 653a  ype is not None:
+000290c0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+000290d0: 756c 745b 274a 6f62 5479 7065 275d 203d  ult['JobType'] =
+000290e0: 2073 656c 662e 6a6f 625f 7479 7065 0a20   self.job_type. 
+000290f0: 2020 2020 2020 2069 6620 7365 6c66 2e6f         if self.o
+00029100: 7264 6572 2069 7320 6e6f 7420 4e6f 6e65  rder is not None
+00029110: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00029120: 7375 6c74 5b27 4f72 6465 7227 5d20 3d20  sult['Order'] = 
+00029130: 7365 6c66 2e6f 7264 6572 0a20 2020 2020  self.order.     
+00029140: 2020 2069 6620 7365 6c66 2e70 6167 655f     if self.page_
+00029150: 6e75 6d62 6572 2069 7320 6e6f 7420 4e6f  number is not No
+00029160: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00029170: 7265 7375 6c74 5b27 5061 6765 4e75 6d62  result['PageNumb
+00029180: 6572 275d 203d 2073 656c 662e 7061 6765  er'] = self.page
+00029190: 5f6e 756d 6265 720a 2020 2020 2020 2020  _number.        
+000291a0: 6966 2073 656c 662e 7061 6765 5f73 697a  if self.page_siz
+000291b0: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
+000291c0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+000291d0: 745b 2750 6167 6553 697a 6527 5d20 3d20  t['PageSize'] = 
+000291e0: 7365 6c66 2e70 6167 655f 7369 7a65 0a20  self.page_size. 
+000291f0: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
+00029200: 6970 656c 696e 655f 6964 2069 7320 6e6f  ipeline_id is no
+00029210: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00029220: 2020 2020 7265 7375 6c74 5b27 5069 7065      result['Pipe
+00029230: 6c69 6e65 4964 275d 203d 2073 656c 662e  lineId'] = self.
+00029240: 7069 7065 6c69 6e65 5f69 640a 2020 2020  pipeline_id.    
+00029250: 2020 2020 6966 2073 656c 662e 7265 736f      if self.reso
+00029260: 7572 6365 5f69 6420 6973 206e 6f74 204e  urce_id is not N
+00029270: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00029280: 2072 6573 756c 745b 2752 6573 6f75 7263   result['Resourc
+00029290: 6549 6427 5d20 3d20 7365 6c66 2e72 6573  eId'] = self.res
+000292a0: 6f75 7263 655f 6964 0a20 2020 2020 2020  ource_id.       
+000292b0: 2069 6620 7365 6c66 2e73 686f 775f 6f77   if self.show_ow
+000292c0: 6e20 6973 206e 6f74 204e 6f6e 653a 0a20  n is not None:. 
+000292d0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+000292e0: 745b 2753 686f 774f 776e 275d 203d 2073  t['ShowOwn'] = s
+000292f0: 656c 662e 7368 6f77 5f6f 776e 0a20 2020  elf.show_own.   
+00029300: 2020 2020 2069 6620 7365 6c66 2e73 6f72       if self.sor
+00029310: 745f 6279 2069 7320 6e6f 7420 4e6f 6e65  t_by is not None
+00029320: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00029330: 7375 6c74 5b27 536f 7274 4279 275d 203d  sult['SortBy'] =
+00029340: 2073 656c 662e 736f 7274 5f62 790a 2020   self.sort_by.  
+00029350: 2020 2020 2020 6966 2073 656c 662e 7374        if self.st
+00029360: 6172 745f 7469 6d65 2069 7320 6e6f 7420  art_time is not 
+00029370: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00029380: 2020 7265 7375 6c74 5b27 5374 6172 7454    result['StartT
+00029390: 696d 6527 5d20 3d20 7365 6c66 2e73 7461  ime'] = self.sta
+000293a0: 7274 5f74 696d 650a 2020 2020 2020 2020  rt_time.        
+000293b0: 6966 2073 656c 662e 7374 6174 7573 2069  if self.status i
+000293c0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000293d0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+000293e0: 5374 6174 7573 275d 203d 2073 656c 662e  Status'] = self.
+000293f0: 7374 6174 7573 0a20 2020 2020 2020 2069  status.        i
+00029400: 6620 7365 6c66 2e74 6167 7320 6973 206e  f self.tags is n
+00029410: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00029420: 2020 2020 2072 6573 756c 745b 2754 6167       result['Tag
+00029430: 7327 5d20 3d20 7365 6c66 2e74 6167 730a  s'] = self.tags.
+00029440: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00029450: 776f 726b 7370 6163 655f 6964 2069 7320  workspace_id is 
+00029460: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00029470: 2020 2020 2020 7265 7375 6c74 5b27 576f        result['Wo
+00029480: 726b 7370 6163 6549 6427 5d20 3d20 7365  rkspaceId'] = se
+00029490: 6c66 2e77 6f72 6b73 7061 6365 5f69 640a  lf.workspace_id.
+000294a0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+000294b0: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
+000294c0: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3a  rom_map(self, m:
+000294d0: 2064 6963 7420 3d20 4e6f 6e65 293a 0a20   dict = None):. 
+000294e0: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
+000294f0: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+00029500: 6620 6d2e 6765 7428 2742 7573 696e 6573  f m.get('Busines
+00029510: 7355 7365 7249 6427 2920 6973 206e 6f74  sUserId') is not
+00029520: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00029530: 2020 2073 656c 662e 6275 7369 6e65 7373     self.business
+00029540: 5f75 7365 725f 6964 203d 206d 2e67 6574  _user_id = m.get
+00029550: 2827 4275 7369 6e65 7373 5573 6572 4964  ('BusinessUserId
+00029560: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+00029570: 6765 7428 2743 616c 6c65 7227 2920 6973  get('Caller') is
+00029580: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00029590: 2020 2020 2020 2073 656c 662e 6361 6c6c         self.call
+000295a0: 6572 203d 206d 2e67 6574 2827 4361 6c6c  er = m.get('Call
+000295b0: 6572 2729 0a20 2020 2020 2020 2069 6620  er').        if 
+000295c0: 6d2e 6765 7428 2744 6973 706c 6179 4e61  m.get('DisplayNa
+000295d0: 6d65 2729 2069 7320 6e6f 7420 4e6f 6e65  me') is not None
+000295e0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+000295f0: 6c66 2e64 6973 706c 6179 5f6e 616d 6520  lf.display_name 
+00029600: 3d20 6d2e 6765 7428 2744 6973 706c 6179  = m.get('Display
+00029610: 4e61 6d65 2729 0a20 2020 2020 2020 2069  Name').        i
+00029620: 6620 6d2e 6765 7428 2745 6e64 5469 6d65  f m.get('EndTime
+00029630: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+00029640: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00029650: 2e65 6e64 5f74 696d 6520 3d20 6d2e 6765  .end_time = m.ge
+00029660: 7428 2745 6e64 5469 6d65 2729 0a20 2020  t('EndTime').   
+00029670: 2020 2020 2069 6620 6d2e 6765 7428 2746       if m.get('F
+00029680: 726f 6d41 6c6c 576f 726b 7370 6163 6573  romAllWorkspaces
+00029690: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+000296a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000296b0: 2e66 726f 6d5f 616c 6c5f 776f 726b 7370  .from_all_worksp
+000296c0: 6163 6573 203d 206d 2e67 6574 2827 4672  aces = m.get('Fr
+000296d0: 6f6d 416c 6c57 6f72 6b73 7061 6365 7327  omAllWorkspaces'
+000296e0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+000296f0: 6574 2827 4a6f 6249 6427 2920 6973 206e  et('JobId') is n
+00029700: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00029710: 2020 2020 2073 656c 662e 6a6f 625f 6964       self.job_id
+00029720: 203d 206d 2e67 6574 2827 4a6f 6249 6427   = m.get('JobId'
+00029730: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+00029740: 6574 2827 4a6f 6254 7970 6527 2920 6973  et('JobType') is
+00029750: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00029760: 2020 2020 2020 2073 656c 662e 6a6f 625f         self.job_
+00029770: 7479 7065 203d 206d 2e67 6574 2827 4a6f  type = m.get('Jo
+00029780: 6254 7970 6527 290a 2020 2020 2020 2020  bType').        
+00029790: 6966 206d 2e67 6574 2827 4f72 6465 7227  if m.get('Order'
+000297a0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+000297b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000297c0: 6f72 6465 7220 3d20 6d2e 6765 7428 274f  order = m.get('O
+000297d0: 7264 6572 2729 0a20 2020 2020 2020 2069  rder').        i
+000297e0: 6620 6d2e 6765 7428 2750 6167 654e 756d  f m.get('PageNum
+000297f0: 6265 7227 2920 6973 206e 6f74 204e 6f6e  ber') is not Non
+00029800: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00029810: 656c 662e 7061 6765 5f6e 756d 6265 7220  elf.page_number 
+00029820: 3d20 6d2e 6765 7428 2750 6167 654e 756d  = m.get('PageNum
+00029830: 6265 7227 290a 2020 2020 2020 2020 6966  ber').        if
+00029840: 206d 2e67 6574 2827 5061 6765 5369 7a65   m.get('PageSize
+00029850: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+00029860: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00029870: 2e70 6167 655f 7369 7a65 203d 206d 2e67  .page_size = m.g
+00029880: 6574 2827 5061 6765 5369 7a65 2729 0a20  et('PageSize'). 
+00029890: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+000298a0: 2750 6970 656c 696e 6549 6427 2920 6973  'PipelineId') is
+000298b0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000298c0: 2020 2020 2020 2073 656c 662e 7069 7065         self.pipe
+000298d0: 6c69 6e65 5f69 6420 3d20 6d2e 6765 7428  line_id = m.get(
+000298e0: 2750 6970 656c 696e 6549 6427 290a 2020  'PipelineId').  
+000298f0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00029900: 5265 736f 7572 6365 4964 2729 2069 7320  ResourceId') is 
+00029910: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00029920: 2020 2020 2020 7365 6c66 2e72 6573 6f75        self.resou
+00029930: 7263 655f 6964 203d 206d 2e67 6574 2827  rce_id = m.get('
+00029940: 5265 736f 7572 6365 4964 2729 0a20 2020  ResourceId').   
+00029950: 2020 2020 2069 6620 6d2e 6765 7428 2753       if m.get('S
+00029960: 686f 774f 776e 2729 2069 7320 6e6f 7420  howOwn') is not 
+00029970: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00029980: 2020 7365 6c66 2e73 686f 775f 6f77 6e20    self.show_own 
+00029990: 3d20 6d2e 6765 7428 2753 686f 774f 776e  = m.get('ShowOwn
+000299a0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+000299b0: 6765 7428 2753 6f72 7442 7927 2920 6973  get('SortBy') is
+000299c0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000299d0: 2020 2020 2020 2073 656c 662e 736f 7274         self.sort
+000299e0: 5f62 7920 3d20 6d2e 6765 7428 2753 6f72  _by = m.get('Sor
+000299f0: 7442 7927 290a 2020 2020 2020 2020 6966  tBy').        if
+00029a00: 206d 2e67 6574 2827 5374 6172 7454 696d   m.get('StartTim
+00029a10: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
+00029a20: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00029a30: 662e 7374 6172 745f 7469 6d65 203d 206d  f.start_time = m
+00029a40: 2e67 6574 2827 5374 6172 7454 696d 6527  .get('StartTime'
+00029a50: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+00029a60: 6574 2827 5374 6174 7573 2729 2069 7320  et('Status') is 
+00029a70: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00029a80: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
+00029a90: 7320 3d20 6d2e 6765 7428 2753 7461 7475  s = m.get('Statu
+00029aa0: 7327 290a 2020 2020 2020 2020 6966 206d  s').        if m
+00029ab0: 2e67 6574 2827 5461 6773 2729 2069 7320  .get('Tags') is 
+00029ac0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00029ad0: 2020 2020 2020 7365 6c66 2e74 6167 7320        self.tags 
+00029ae0: 3d20 6d2e 6765 7428 2754 6167 7327 290a  = m.get('Tags').
+00029af0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+00029b00: 2827 576f 726b 7370 6163 6549 6427 2920  ('WorkspaceId') 
+00029b10: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00029b20: 2020 2020 2020 2020 2073 656c 662e 776f           self.wo
+00029b30: 726b 7370 6163 655f 6964 203d 206d 2e67  rkspace_id = m.g
+00029b40: 6574 2827 576f 726b 7370 6163 6549 6427  et('WorkspaceId'
+00029b50: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00029b60: 2073 656c 660a 0a0a 636c 6173 7320 4c69   self...class Li
+00029b70: 7374 4a6f 6273 5368 7269 6e6b 5265 7175  stJobsShrinkRequ
+00029b80: 6573 7428 5465 614d 6f64 656c 293a 0a20  est(TeaModel):. 
+00029b90: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+00029ba0: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+00029bb0: 2020 2020 2020 2062 7573 696e 6573 735f         business_
+00029bc0: 7573 6572 5f69 643a 2073 7472 203d 204e  user_id: str = N
+00029bd0: 6f6e 652c 0a20 2020 2020 2020 2063 616c  one,.        cal
+00029be0: 6c65 723a 2073 7472 203d 204e 6f6e 652c  ler: str = None,
+00029bf0: 0a20 2020 2020 2020 2064 6973 706c 6179  .        display
+00029c00: 5f6e 616d 653a 2073 7472 203d 204e 6f6e  _name: str = Non
+00029c10: 652c 0a20 2020 2020 2020 2065 6e64 5f74  e,.        end_t
+00029c20: 696d 653a 2073 7472 203d 204e 6f6e 652c  ime: str = None,
+00029c30: 0a20 2020 2020 2020 2066 726f 6d5f 616c  .        from_al
+00029c40: 6c5f 776f 726b 7370 6163 6573 3a20 626f  l_workspaces: bo
+00029c50: 6f6c 203d 204e 6f6e 652c 0a20 2020 2020  ol = None,.     
+00029c60: 2020 206a 6f62 5f69 643a 2073 7472 203d     job_id: str =
+00029c70: 204e 6f6e 652c 0a20 2020 2020 2020 206a   None,.        j
+00029c80: 6f62 5f74 7970 653a 2073 7472 203d 204e  ob_type: str = N
+00029c90: 6f6e 652c 0a20 2020 2020 2020 206f 7264  one,.        ord
+00029ca0: 6572 3a20 7374 7220 3d20 4e6f 6e65 2c0a  er: str = None,.
+00029cb0: 2020 2020 2020 2020 7061 6765 5f6e 756d          page_num
+00029cc0: 6265 723a 2069 6e74 203d 204e 6f6e 652c  ber: int = None,
+00029cd0: 0a20 2020 2020 2020 2070 6167 655f 7369  .        page_si
+00029ce0: 7a65 3a20 696e 7420 3d20 4e6f 6e65 2c0a  ze: int = None,.
+00029cf0: 2020 2020 2020 2020 7069 7065 6c69 6e65          pipeline
+00029d00: 5f69 643a 2073 7472 203d 204e 6f6e 652c  _id: str = None,
+00029d10: 0a20 2020 2020 2020 2072 6573 6f75 7263  .        resourc
+00029d20: 655f 6964 3a20 7374 7220 3d20 4e6f 6e65  e_id: str = None
+00029d30: 2c0a 2020 2020 2020 2020 7368 6f77 5f6f  ,.        show_o
+00029d40: 776e 3a20 626f 6f6c 203d 204e 6f6e 652c  wn: bool = None,
+00029d50: 0a20 2020 2020 2020 2073 6f72 745f 6279  .        sort_by
+00029d60: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+00029d70: 2020 2020 2020 7374 6172 745f 7469 6d65        start_time
+00029d80: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+00029d90: 2020 2020 2020 7374 6174 7573 3a20 7374        status: st
+00029da0: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
+00029db0: 2020 7461 6773 5f73 6872 696e 6b3a 2073    tags_shrink: s
+00029dc0: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
+00029dd0: 2020 2077 6f72 6b73 7061 6365 5f69 643a     workspace_id:
+00029de0: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+00029df0: 2029 3a0a 2020 2020 2020 2020 7365 6c66   ):.        self
+00029e00: 2e62 7573 696e 6573 735f 7573 6572 5f69  .business_user_i
+00029e10: 6420 3d20 6275 7369 6e65 7373 5f75 7365  d = business_use
+00029e20: 725f 6964 0a20 2020 2020 2020 2073 656c  r_id.        sel
+00029e30: 662e 6361 6c6c 6572 203d 2063 616c 6c65  f.caller = calle
+00029e40: 720a 2020 2020 2020 2020 7365 6c66 2e64  r.        self.d
+00029e50: 6973 706c 6179 5f6e 616d 6520 3d20 6469  isplay_name = di
+00029e60: 7370 6c61 795f 6e61 6d65 0a20 2020 2020  splay_name.     
+00029e70: 2020 2073 656c 662e 656e 645f 7469 6d65     self.end_time
+00029e80: 203d 2065 6e64 5f74 696d 650a 2020 2020   = end_time.    
+00029e90: 2020 2020 7365 6c66 2e66 726f 6d5f 616c      self.from_al
+00029ea0: 6c5f 776f 726b 7370 6163 6573 203d 2066  l_workspaces = f
+00029eb0: 726f 6d5f 616c 6c5f 776f 726b 7370 6163  rom_all_workspac
+00029ec0: 6573 0a20 2020 2020 2020 2073 656c 662e  es.        self.
+00029ed0: 6a6f 625f 6964 203d 206a 6f62 5f69 640a  job_id = job_id.
+00029ee0: 2020 2020 2020 2020 7365 6c66 2e6a 6f62          self.job
+00029ef0: 5f74 7970 6520 3d20 6a6f 625f 7479 7065  _type = job_type
+00029f00: 0a20 2020 2020 2020 2073 656c 662e 6f72  .        self.or
+00029f10: 6465 7220 3d20 6f72 6465 720a 2020 2020  der = order.    
+00029f20: 2020 2020 7365 6c66 2e70 6167 655f 6e75      self.page_nu
+00029f30: 6d62 6572 203d 2070 6167 655f 6e75 6d62  mber = page_numb
+00029f40: 6572 0a20 2020 2020 2020 2073 656c 662e  er.        self.
+00029f50: 7061 6765 5f73 697a 6520 3d20 7061 6765  page_size = page
+00029f60: 5f73 697a 650a 2020 2020 2020 2020 7365  _size.        se
+00029f70: 6c66 2e70 6970 656c 696e 655f 6964 203d  lf.pipeline_id =
+00029f80: 2070 6970 656c 696e 655f 6964 0a20 2020   pipeline_id.   
+00029f90: 2020 2020 2073 656c 662e 7265 736f 7572       self.resour
+00029fa0: 6365 5f69 6420 3d20 7265 736f 7572 6365  ce_id = resource
+00029fb0: 5f69 640a 2020 2020 2020 2020 7365 6c66  _id.        self
+00029fc0: 2e73 686f 775f 6f77 6e20 3d20 7368 6f77  .show_own = show
+00029fd0: 5f6f 776e 0a20 2020 2020 2020 2073 656c  _own.        sel
+00029fe0: 662e 736f 7274 5f62 7920 3d20 736f 7274  f.sort_by = sort
+00029ff0: 5f62 790a 2020 2020 2020 2020 7365 6c66  _by.        self
+0002a000: 2e73 7461 7274 5f74 696d 6520 3d20 7374  .start_time = st
+0002a010: 6172 745f 7469 6d65 0a20 2020 2020 2020  art_time.       
+0002a020: 2073 656c 662e 7374 6174 7573 203d 2073   self.status = s
+0002a030: 7461 7475 730a 2020 2020 2020 2020 7365  tatus.        se
+0002a040: 6c66 2e74 6167 735f 7368 7269 6e6b 203d  lf.tags_shrink =
+0002a050: 2074 6167 735f 7368 7269 6e6b 0a20 2020   tags_shrink.   
+0002a060: 2020 2020 2073 656c 662e 776f 726b 7370       self.worksp
+0002a070: 6163 655f 6964 203d 2077 6f72 6b73 7061  ace_id = workspa
+0002a080: 6365 5f69 640a 0a20 2020 2064 6566 2076  ce_id..    def v
+0002a090: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
+0002a0a0: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
+0002a0b0: 2064 6566 2074 6f5f 6d61 7028 7365 6c66   def to_map(self
+0002a0c0: 293a 0a20 2020 2020 2020 205f 6d61 7020  ):.        _map 
+0002a0d0: 3d20 7375 7065 7228 292e 746f 5f6d 6170  = super().to_map
+0002a0e0: 2829 0a20 2020 2020 2020 2069 6620 5f6d  ().        if _m
+0002a0f0: 6170 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ap is not None:.
+0002a100: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0002a110: 726e 205f 6d61 700a 0a20 2020 2020 2020  rn _map..       
+0002a120: 2072 6573 756c 7420 3d20 6469 6374 2829   result = dict()
+0002a130: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0002a140: 2e62 7573 696e 6573 735f 7573 6572 5f69  .business_user_i
+0002a150: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
+0002a160: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+0002a170: 745b 2742 7573 696e 6573 7355 7365 7249  t['BusinessUserI
+0002a180: 6427 5d20 3d20 7365 6c66 2e62 7573 696e  d'] = self.busin
+0002a190: 6573 735f 7573 6572 5f69 640a 2020 2020  ess_user_id.    
+0002a1a0: 2020 2020 6966 2073 656c 662e 6361 6c6c      if self.call
+0002a1b0: 6572 2069 7320 6e6f 7420 4e6f 6e65 3a0a  er is not None:.
+0002a1c0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+0002a1d0: 6c74 5b27 4361 6c6c 6572 275d 203d 2073  lt['Caller'] = s
+0002a1e0: 656c 662e 6361 6c6c 6572 0a20 2020 2020  elf.caller.     
+0002a1f0: 2020 2069 6620 7365 6c66 2e64 6973 706c     if self.displ
+0002a200: 6179 5f6e 616d 6520 6973 206e 6f74 204e  ay_name is not N
+0002a210: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0002a220: 2072 6573 756c 745b 2744 6973 706c 6179   result['Display
+0002a230: 4e61 6d65 275d 203d 2073 656c 662e 6469  Name'] = self.di
+0002a240: 7370 6c61 795f 6e61 6d65 0a20 2020 2020  splay_name.     
+0002a250: 2020 2069 6620 7365 6c66 2e65 6e64 5f74     if self.end_t
+0002a260: 696d 6520 6973 206e 6f74 204e 6f6e 653a  ime is not None:
+0002a270: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+0002a280: 756c 745b 2745 6e64 5469 6d65 275d 203d  ult['EndTime'] =
+0002a290: 2073 656c 662e 656e 645f 7469 6d65 0a20   self.end_time. 
+0002a2a0: 2020 2020 2020 2069 6620 7365 6c66 2e66         if self.f
+0002a2b0: 726f 6d5f 616c 6c5f 776f 726b 7370 6163  rom_all_workspac
+0002a2c0: 6573 2069 7320 6e6f 7420 4e6f 6e65 3a0a  es is not None:.
+0002a2d0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+0002a2e0: 6c74 5b27 4672 6f6d 416c 6c57 6f72 6b73  lt['FromAllWorks
+0002a2f0: 7061 6365 7327 5d20 3d20 7365 6c66 2e66  paces'] = self.f
+0002a300: 726f 6d5f 616c 6c5f 776f 726b 7370 6163  rom_all_workspac
+0002a310: 6573 0a20 2020 2020 2020 2069 6620 7365  es.        if se
+0002a320: 6c66 2e6a 6f62 5f69 6420 6973 206e 6f74  lf.job_id is not
+0002a330: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0002a340: 2020 2072 6573 756c 745b 274a 6f62 4964     result['JobId
+0002a350: 275d 203d 2073 656c 662e 6a6f 625f 6964  '] = self.job_id
+0002a360: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0002a370: 2e6a 6f62 5f74 7970 6520 6973 206e 6f74  .job_type is not
+0002a380: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0002a390: 2020 2072 6573 756c 745b 274a 6f62 5479     result['JobTy
+0002a3a0: 7065 275d 203d 2073 656c 662e 6a6f 625f  pe'] = self.job_
+0002a3b0: 7479 7065 0a20 2020 2020 2020 2069 6620  type.        if 
+0002a3c0: 7365 6c66 2e6f 7264 6572 2069 7320 6e6f  self.order is no
+0002a3d0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0002a3e0: 2020 2020 7265 7375 6c74 5b27 4f72 6465      result['Orde
+0002a3f0: 7227 5d20 3d20 7365 6c66 2e6f 7264 6572  r'] = self.order
+0002a400: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0002a410: 2e70 6167 655f 6e75 6d62 6572 2069 7320  .page_number is 
+0002a420: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0002a430: 2020 2020 2020 7265 7375 6c74 5b27 5061        result['Pa
+0002a440: 6765 4e75 6d62 6572 275d 203d 2073 656c  geNumber'] = sel
+0002a450: 662e 7061 6765 5f6e 756d 6265 720a 2020  f.page_number.  
+0002a460: 2020 2020 2020 6966 2073 656c 662e 7061        if self.pa
+0002a470: 6765 5f73 697a 6520 6973 206e 6f74 204e  ge_size is not N
+0002a480: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0002a490: 2072 6573 756c 745b 2750 6167 6553 697a   result['PageSiz
+0002a4a0: 6527 5d20 3d20 7365 6c66 2e70 6167 655f  e'] = self.page_
+0002a4b0: 7369 7a65 0a20 2020 2020 2020 2069 6620  size.        if 
+0002a4c0: 7365 6c66 2e70 6970 656c 696e 655f 6964  self.pipeline_id
+0002a4d0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0002a4e0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+0002a4f0: 5b27 5069 7065 6c69 6e65 4964 275d 203d  ['PipelineId'] =
+0002a500: 2073 656c 662e 7069 7065 6c69 6e65 5f69   self.pipeline_i
+0002a510: 640a 2020 2020 2020 2020 6966 2073 656c  d.        if sel
+0002a520: 662e 7265 736f 7572 6365 5f69 6420 6973  f.resource_id is
+0002a530: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0002a540: 2020 2020 2020 2072 6573 756c 745b 2752         result['R
+0002a550: 6573 6f75 7263 6549 6427 5d20 3d20 7365  esourceId'] = se
+0002a560: 6c66 2e72 6573 6f75 7263 655f 6964 0a20  lf.resource_id. 
+0002a570: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
+0002a580: 686f 775f 6f77 6e20 6973 206e 6f74 204e  how_own is not N
+0002a590: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0002a5a0: 2072 6573 756c 745b 2753 686f 774f 776e   result['ShowOwn
+0002a5b0: 275d 203d 2073 656c 662e 7368 6f77 5f6f  '] = self.show_o
+0002a5c0: 776e 0a20 2020 2020 2020 2069 6620 7365  wn.        if se
+0002a5d0: 6c66 2e73 6f72 745f 6279 2069 7320 6e6f  lf.sort_by is no
+0002a5e0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0002a5f0: 2020 2020 7265 7375 6c74 5b27 536f 7274      result['Sort
+0002a600: 4279 275d 203d 2073 656c 662e 736f 7274  By'] = self.sort
+0002a610: 5f62 790a 2020 2020 2020 2020 6966 2073  _by.        if s
+0002a620: 656c 662e 7374 6172 745f 7469 6d65 2069  elf.start_time i
+0002a630: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0002a640: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+0002a650: 5374 6172 7454 696d 6527 5d20 3d20 7365  StartTime'] = se
+0002a660: 6c66 2e73 7461 7274 5f74 696d 650a 2020  lf.start_time.  
+0002a670: 2020 2020 2020 6966 2073 656c 662e 7374        if self.st
+0002a680: 6174 7573 2069 7320 6e6f 7420 4e6f 6e65  atus is not None
+0002a690: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0002a6a0: 7375 6c74 5b27 5374 6174 7573 275d 203d  sult['Status'] =
+0002a6b0: 2073 656c 662e 7374 6174 7573 0a20 2020   self.status.   
+0002a6c0: 2020 2020 2069 6620 7365 6c66 2e74 6167       if self.tag
+0002a6d0: 735f 7368 7269 6e6b 2069 7320 6e6f 7420  s_shrink is not 
+0002a6e0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0002a6f0: 2020 7265 7375 6c74 5b27 5461 6773 275d    result['Tags']
+0002a700: 203d 2073 656c 662e 7461 6773 5f73 6872   = self.tags_shr
+0002a710: 696e 6b0a 2020 2020 2020 2020 6966 2073  ink.        if s
+0002a720: 656c 662e 776f 726b 7370 6163 655f 6964  elf.workspace_id
+0002a730: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0002a740: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+0002a750: 5b27 576f 726b 7370 6163 6549 6427 5d20  ['WorkspaceId'] 
+0002a760: 3d20 7365 6c66 2e77 6f72 6b73 7061 6365  = self.workspace
+0002a770: 5f69 640a 2020 2020 2020 2020 7265 7475  _id.        retu
+0002a780: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
+0002a790: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
+0002a7a0: 2c20 6d3a 2064 6963 7420 3d20 4e6f 6e65  , m: dict = None
+0002a7b0: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
+0002a7c0: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
+0002a7d0: 2020 2069 6620 6d2e 6765 7428 2742 7573     if m.get('Bus
+0002a7e0: 696e 6573 7355 7365 7249 6427 2920 6973  inessUserId') is
+0002a7f0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0002a800: 2020 2020 2020 2073 656c 662e 6275 7369         self.busi
+0002a810: 6e65 7373 5f75 7365 725f 6964 203d 206d  ness_user_id = m
+0002a820: 2e67 6574 2827 4275 7369 6e65 7373 5573  .get('BusinessUs
+0002a830: 6572 4964 2729 0a20 2020 2020 2020 2069  erId').        i
+0002a840: 6620 6d2e 6765 7428 2743 616c 6c65 7227  f m.get('Caller'
+0002a850: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+0002a860: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0002a870: 6361 6c6c 6572 203d 206d 2e67 6574 2827  caller = m.get('
+0002a880: 4361 6c6c 6572 2729 0a20 2020 2020 2020  Caller').       
+0002a890: 2069 6620 6d2e 6765 7428 2744 6973 706c   if m.get('Displ
+0002a8a0: 6179 4e61 6d65 2729 2069 7320 6e6f 7420  ayName') is not 
+0002a8b0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0002a8c0: 2020 7365 6c66 2e64 6973 706c 6179 5f6e    self.display_n
+0002a8d0: 616d 6520 3d20 6d2e 6765 7428 2744 6973  ame = m.get('Dis
+0002a8e0: 706c 6179 4e61 6d65 2729 0a20 2020 2020  playName').     
+0002a8f0: 2020 2069 6620 6d2e 6765 7428 2745 6e64     if m.get('End
+0002a900: 5469 6d65 2729 2069 7320 6e6f 7420 4e6f  Time') is not No
+0002a910: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0002a920: 7365 6c66 2e65 6e64 5f74 696d 6520 3d20  self.end_time = 
+0002a930: 6d2e 6765 7428 2745 6e64 5469 6d65 2729  m.get('EndTime')
+0002a940: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+0002a950: 7428 2746 726f 6d41 6c6c 576f 726b 7370  t('FromAllWorksp
+0002a960: 6163 6573 2729 2069 7320 6e6f 7420 4e6f  aces') is not No
+0002a970: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0002a980: 7365 6c66 2e66 726f 6d5f 616c 6c5f 776f  self.from_all_wo
+0002a990: 726b 7370 6163 6573 203d 206d 2e67 6574  rkspaces = m.get
+0002a9a0: 2827 4672 6f6d 416c 6c57 6f72 6b73 7061  ('FromAllWorkspa
+0002a9b0: 6365 7327 290a 2020 2020 2020 2020 6966  ces').        if
+0002a9c0: 206d 2e67 6574 2827 4a6f 6249 6427 2920   m.get('JobId') 
+0002a9d0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0002a9e0: 2020 2020 2020 2020 2073 656c 662e 6a6f           self.jo
+0002a9f0: 625f 6964 203d 206d 2e67 6574 2827 4a6f  b_id = m.get('Jo
+0002aa00: 6249 6427 290a 2020 2020 2020 2020 6966  bId').        if
+0002aa10: 206d 2e67 6574 2827 4a6f 6254 7970 6527   m.get('JobType'
+0002aa20: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+0002aa30: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0002aa40: 6a6f 625f 7479 7065 203d 206d 2e67 6574  job_type = m.get
+0002aa50: 2827 4a6f 6254 7970 6527 290a 2020 2020  ('JobType').    
+0002aa60: 2020 2020 6966 206d 2e67 6574 2827 4f72      if m.get('Or
+0002aa70: 6465 7227 2920 6973 206e 6f74 204e 6f6e  der') is not Non
+0002aa80: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0002aa90: 656c 662e 6f72 6465 7220 3d20 6d2e 6765  elf.order = m.ge
+0002aaa0: 7428 274f 7264 6572 2729 0a20 2020 2020  t('Order').     
+0002aab0: 2020 2069 6620 6d2e 6765 7428 2750 6167     if m.get('Pag
+0002aac0: 654e 756d 6265 7227 2920 6973 206e 6f74  eNumber') is not
+0002aad0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0002aae0: 2020 2073 656c 662e 7061 6765 5f6e 756d     self.page_num
+0002aaf0: 6265 7220 3d20 6d2e 6765 7428 2750 6167  ber = m.get('Pag
+0002ab00: 654e 756d 6265 7227 290a 2020 2020 2020  eNumber').      
+0002ab10: 2020 6966 206d 2e67 6574 2827 5061 6765    if m.get('Page
+0002ab20: 5369 7a65 2729 2069 7320 6e6f 7420 4e6f  Size') is not No
+0002ab30: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0002ab40: 7365 6c66 2e70 6167 655f 7369 7a65 203d  self.page_size =
+0002ab50: 206d 2e67 6574 2827 5061 6765 5369 7a65   m.get('PageSize
+0002ab60: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+0002ab70: 6765 7428 2750 6970 656c 696e 6549 6427  get('PipelineId'
+0002ab80: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+0002ab90: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0002aba0: 7069 7065 6c69 6e65 5f69 6420 3d20 6d2e  pipeline_id = m.
+0002abb0: 6765 7428 2750 6970 656c 696e 6549 6427  get('PipelineId'
+0002abc0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+0002abd0: 6574 2827 5265 736f 7572 6365 4964 2729  et('ResourceId')
+0002abe0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0002abf0: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+0002ac00: 6573 6f75 7263 655f 6964 203d 206d 2e67  esource_id = m.g
+0002ac10: 6574 2827 5265 736f 7572 6365 4964 2729  et('ResourceId')
+0002ac20: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+0002ac30: 7428 2753 686f 774f 776e 2729 2069 7320  t('ShowOwn') is 
+0002ac40: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0002ac50: 2020 2020 2020 7365 6c66 2e73 686f 775f        self.show_
+0002ac60: 6f77 6e20 3d20 6d2e 6765 7428 2753 686f  own = m.get('Sho
+0002ac70: 774f 776e 2729 0a20 2020 2020 2020 2069  wOwn').        i
+0002ac80: 6620 6d2e 6765 7428 2753 6f72 7442 7927  f m.get('SortBy'
+0002ac90: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+0002aca0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0002acb0: 736f 7274 5f62 7920 3d20 6d2e 6765 7428  sort_by = m.get(
+0002acc0: 2753 6f72 7442 7927 290a 2020 2020 2020  'SortBy').      
+0002acd0: 2020 6966 206d 2e67 6574 2827 5374 6172    if m.get('Star
+0002ace0: 7454 696d 6527 2920 6973 206e 6f74 204e  tTime') is not N
+0002acf0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0002ad00: 2073 656c 662e 7374 6172 745f 7469 6d65   self.start_time
+0002ad10: 203d 206d 2e67 6574 2827 5374 6172 7454   = m.get('StartT
+0002ad20: 696d 6527 290a 2020 2020 2020 2020 6966  ime').        if
+0002ad30: 206d 2e67 6574 2827 5374 6174 7573 2729   m.get('Status')
+0002ad40: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0002ad50: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+0002ad60: 7461 7475 7320 3d20 6d2e 6765 7428 2753  tatus = m.get('S
+0002ad70: 7461 7475 7327 290a 2020 2020 2020 2020  tatus').        
+0002ad80: 6966 206d 2e67 6574 2827 5461 6773 2729  if m.get('Tags')
+0002ad90: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0002ada0: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
+0002adb0: 6167 735f 7368 7269 6e6b 203d 206d 2e67  ags_shrink = m.g
+0002adc0: 6574 2827 5461 6773 2729 0a20 2020 2020  et('Tags').     
+0002add0: 2020 2069 6620 6d2e 6765 7428 2757 6f72     if m.get('Wor
+0002ade0: 6b73 7061 6365 4964 2729 2069 7320 6e6f  kspaceId') is no
+0002adf0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0002ae00: 2020 2020 7365 6c66 2e77 6f72 6b73 7061      self.workspa
+0002ae10: 6365 5f69 6420 3d20 6d2e 6765 7428 2757  ce_id = m.get('W
+0002ae20: 6f72 6b73 7061 6365 4964 2729 0a20 2020  orkspaceId').   
+0002ae30: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+0002ae40: 0a0a 0a63 6c61 7373 204c 6973 744a 6f62  ...class ListJob
+0002ae50: 7352 6573 706f 6e73 6542 6f64 7928 5465  sResponseBody(Te
+0002ae60: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
+0002ae70: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
+0002ae80: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+0002ae90: 206a 6f62 733a 204c 6973 745b 4a6f 6249   jobs: List[JobI
+0002aea0: 7465 6d5d 203d 204e 6f6e 652c 0a20 2020  tem] = None,.   
+0002aeb0: 2020 2020 2072 6571 7565 7374 5f69 643a       request_id:
+0002aec0: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
+0002aed0: 2020 2020 2074 6f74 616c 5f63 6f75 6e74       total_count
+0002aee0: 3a20 696e 7420 3d20 4e6f 6e65 2c0a 2020  : int = None,.  
+0002aef0: 2020 293a 0a20 2020 2020 2020 2073 656c    ):.        sel
+0002af00: 662e 6a6f 6273 203d 206a 6f62 730a 2020  f.jobs = jobs.  
+0002af10: 2020 2020 2020 7365 6c66 2e72 6571 7565        self.reque
+0002af20: 7374 5f69 6420 3d20 7265 7175 6573 745f  st_id = request_
+0002af30: 6964 0a20 2020 2020 2020 2073 656c 662e  id.        self.
+0002af40: 746f 7461 6c5f 636f 756e 7420 3d20 746f  total_count = to
+0002af50: 7461 6c5f 636f 756e 740a 0a20 2020 2064  tal_count..    d
+0002af60: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
+0002af70: 293a 0a20 2020 2020 2020 2069 6620 7365  ):.        if se
+0002af80: 6c66 2e6a 6f62 733a 0a20 2020 2020 2020  lf.jobs:.       
+0002af90: 2020 2020 2066 6f72 206b 2069 6e20 7365       for k in se
+0002afa0: 6c66 2e6a 6f62 733a 0a20 2020 2020 2020  lf.jobs:.       
+0002afb0: 2020 2020 2020 2020 2069 6620 6b3a 0a20           if k:. 
+0002afc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002afd0: 2020 206b 2e76 616c 6964 6174 6528 290a     k.validate().
+0002afe0: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
+0002aff0: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
+0002b000: 6d61 7020 3d20 7375 7065 7228 292e 746f  map = super().to
+0002b010: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
+0002b020: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
+0002b030: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0002b040: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
+0002b050: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
+0002b060: 6374 2829 0a20 2020 2020 2020 2072 6573  ct().        res
+0002b070: 756c 745b 274a 6f62 7327 5d20 3d20 5b5d  ult['Jobs'] = []
+0002b080: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0002b090: 2e6a 6f62 7320 6973 206e 6f74 204e 6f6e  .jobs is not Non
+0002b0a0: 653a 0a20 2020 2020 2020 2020 2020 2066  e:.            f
+0002b0b0: 6f72 206b 2069 6e20 7365 6c66 2e6a 6f62  or k in self.job
+0002b0c0: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+0002b0d0: 2020 2072 6573 756c 745b 274a 6f62 7327     result['Jobs'
+0002b0e0: 5d2e 6170 7065 6e64 286b 2e74 6f5f 6d61  ].append(k.to_ma
+0002b0f0: 7028 2920 6966 206b 2065 6c73 6520 4e6f  p() if k else No
+0002b100: 6e65 290a 2020 2020 2020 2020 6966 2073  ne).        if s
+0002b110: 656c 662e 7265 7175 6573 745f 6964 2069  elf.request_id i
+0002b120: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0002b130: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+0002b140: 5265 7175 6573 7449 6427 5d20 3d20 7365  RequestId'] = se
+0002b150: 6c66 2e72 6571 7565 7374 5f69 640a 2020  lf.request_id.  
+0002b160: 2020 2020 2020 6966 2073 656c 662e 746f        if self.to
+0002b170: 7461 6c5f 636f 756e 7420 6973 206e 6f74  tal_count is not
+0002b180: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0002b190: 2020 2072 6573 756c 745b 2754 6f74 616c     result['Total
+0002b1a0: 436f 756e 7427 5d20 3d20 7365 6c66 2e74  Count'] = self.t
+0002b1b0: 6f74 616c 5f63 6f75 6e74 0a20 2020 2020  otal_count.     
+0002b1c0: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
+0002b1d0: 0a0a 2020 2020 6465 6620 6672 6f6d 5f6d  ..    def from_m
+0002b1e0: 6170 2873 656c 662c 206d 3a20 6469 6374  ap(self, m: dict
+0002b1f0: 203d 204e 6f6e 6529 3a0a 2020 2020 2020   = None):.      
+0002b200: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
+0002b210: 290a 2020 2020 2020 2020 7365 6c66 2e6a  ).        self.j
+0002b220: 6f62 7320 3d20 5b5d 0a20 2020 2020 2020  obs = [].       
+0002b230: 2069 6620 6d2e 6765 7428 274a 6f62 7327   if m.get('Jobs'
+0002b240: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+0002b250: 2020 2020 2020 2020 2020 2066 6f72 206b             for k
+0002b260: 2069 6e20 6d2e 6765 7428 274a 6f62 7327   in m.get('Jobs'
+0002b270: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0002b280: 2020 2074 656d 705f 6d6f 6465 6c20 3d20     temp_model = 
+0002b290: 4a6f 6249 7465 6d28 290a 2020 2020 2020  JobItem().      
+0002b2a0: 2020 2020 2020 2020 2020 7365 6c66 2e6a            self.j
+0002b2b0: 6f62 732e 6170 7065 6e64 2874 656d 705f  obs.append(temp_
+0002b2c0: 6d6f 6465 6c2e 6672 6f6d 5f6d 6170 286b  model.from_map(k
+0002b2d0: 2929 0a20 2020 2020 2020 2069 6620 6d2e  )).        if m.
+0002b2e0: 6765 7428 2752 6571 7565 7374 4964 2729  get('RequestId')
+0002b2f0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0002b300: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+0002b310: 6571 7565 7374 5f69 6420 3d20 6d2e 6765  equest_id = m.ge
+0002b320: 7428 2752 6571 7565 7374 4964 2729 0a20  t('RequestId'). 
+0002b330: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+0002b340: 2754 6f74 616c 436f 756e 7427 2920 6973  'TotalCount') is
+0002b350: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0002b360: 2020 2020 2020 2073 656c 662e 746f 7461         self.tota
+0002b370: 6c5f 636f 756e 7420 3d20 6d2e 6765 7428  l_count = m.get(
+0002b380: 2754 6f74 616c 436f 756e 7427 290a 2020  'TotalCount').  
+0002b390: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0002b3a0: 660a 0a0a 636c 6173 7320 4c69 7374 4a6f  f...class ListJo
+0002b3b0: 6273 5265 7370 6f6e 7365 2854 6561 4d6f  bsResponse(TeaMo
+0002b3c0: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
+0002b3d0: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
+0002b3e0: 7365 6c66 2c0a 2020 2020 2020 2020 6865  self,.        he
+0002b3f0: 6164 6572 733a 2044 6963 745b 7374 722c  aders: Dict[str,
+0002b400: 2073 7472 5d20 3d20 4e6f 6e65 2c0a 2020   str] = None,.  
+0002b410: 2020 2020 2020 7374 6174 7573 5f63 6f64        status_cod
+0002b420: 653a 2069 6e74 203d 204e 6f6e 652c 0a20  e: int = None,. 
+0002b430: 2020 2020 2020 2062 6f64 793a 204c 6973         body: Lis
+0002b440: 744a 6f62 7352 6573 706f 6e73 6542 6f64  tJobsResponseBod
+0002b450: 7920 3d20 4e6f 6e65 2c0a 2020 2020 293a  y = None,.    ):
+0002b460: 0a20 2020 2020 2020 2073 656c 662e 6865  .        self.he
+0002b470: 6164 6572 7320 3d20 6865 6164 6572 730a  aders = headers.
+0002b480: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
+0002b490: 7475 735f 636f 6465 203d 2073 7461 7475  tus_code = statu
+0002b4a0: 735f 636f 6465 0a20 2020 2020 2020 2073  s_code.        s
+0002b4b0: 656c 662e 626f 6479 203d 2062 6f64 790a  elf.body = body.
+0002b4c0: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
+0002b4d0: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+0002b4e0: 2073 656c 662e 7661 6c69 6461 7465 5f72   self.validate_r
+0002b4f0: 6571 7569 7265 6428 7365 6c66 2e68 6561  equired(self.hea
+0002b500: 6465 7273 2c20 2768 6561 6465 7273 2729  ders, 'headers')
+0002b510: 0a20 2020 2020 2020 2073 656c 662e 7661  .        self.va
+0002b520: 6c69 6461 7465 5f72 6571 7569 7265 6428  lidate_required(
+0002b530: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
+0002b540: 2c20 2773 7461 7475 735f 636f 6465 2729  , 'status_code')
+0002b550: 0a20 2020 2020 2020 2073 656c 662e 7661  .        self.va
+0002b560: 6c69 6461 7465 5f72 6571 7569 7265 6428  lidate_required(
+0002b570: 7365 6c66 2e62 6f64 792c 2027 626f 6479  self.body, 'body
+0002b580: 2729 0a20 2020 2020 2020 2069 6620 7365  ').        if se
+0002b590: 6c66 2e62 6f64 793a 0a20 2020 2020 2020  lf.body:.       
+0002b5a0: 2020 2020 2073 656c 662e 626f 6479 2e76       self.body.v
+0002b5b0: 616c 6964 6174 6528 290a 0a20 2020 2064  alidate()..    d
+0002b5c0: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
+0002b5d0: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
+0002b5e0: 7375 7065 7228 292e 746f 5f6d 6170 2829  super().to_map()
+0002b5f0: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
+0002b600: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0002b610: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0002b620: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
+0002b630: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
+0002b640: 2020 2020 2020 2069 6620 7365 6c66 2e68         if self.h
+0002b650: 6561 6465 7273 2069 7320 6e6f 7420 4e6f  eaders is not No
+0002b660: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0002b670: 7265 7375 6c74 5b27 6865 6164 6572 7327  result['headers'
+0002b680: 5d20 3d20 7365 6c66 2e68 6561 6465 7273  ] = self.headers
+0002b690: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0002b6a0: 2e73 7461 7475 735f 636f 6465 2069 7320  .status_code is 
+0002b6b0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0002b6c0: 2020 2020 2020 7265 7375 6c74 5b27 7374        result['st
+0002b6d0: 6174 7573 436f 6465 275d 203d 2073 656c  atusCode'] = sel
+0002b6e0: 662e 7374 6174 7573 5f63 6f64 650a 2020  f.status_code.  
+0002b6f0: 2020 2020 2020 6966 2073 656c 662e 626f        if self.bo
+0002b700: 6479 2069 7320 6e6f 7420 4e6f 6e65 3a0a  dy is not None:.
+0002b710: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+0002b720: 6c74 5b27 626f 6479 275d 203d 2073 656c  lt['body'] = sel
+0002b730: 662e 626f 6479 2e74 6f5f 6d61 7028 290a  f.body.to_map().
+0002b740: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+0002b750: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
+0002b760: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3a  rom_map(self, m:
+0002b770: 2064 6963 7420 3d20 4e6f 6e65 293a 0a20   dict = None):. 
+0002b780: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
+0002b790: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+0002b7a0: 6620 6d2e 6765 7428 2768 6561 6465 7273  f m.get('headers
+0002b7b0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+0002b7c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0002b7d0: 2e68 6561 6465 7273 203d 206d 2e67 6574  .headers = m.get
+0002b7e0: 2827 6865 6164 6572 7327 290a 2020 2020  ('headers').    
+0002b7f0: 2020 2020 6966 206d 2e67 6574 2827 7374      if m.get('st
+0002b800: 6174 7573 436f 6465 2729 2069 7320 6e6f  atusCode') is no
+0002b810: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0002b820: 2020 2020 7365 6c66 2e73 7461 7475 735f      self.status_
+0002b830: 636f 6465 203d 206d 2e67 6574 2827 7374  code = m.get('st
+0002b840: 6174 7573 436f 6465 2729 0a20 2020 2020  atusCode').     
+0002b850: 2020 2069 6620 6d2e 6765 7428 2762 6f64     if m.get('bod
+0002b860: 7927 2920 6973 206e 6f74 204e 6f6e 653a  y') is not None:
+0002b870: 0a20 2020 2020 2020 2020 2020 2074 656d  .            tem
+0002b880: 705f 6d6f 6465 6c20 3d20 4c69 7374 4a6f  p_model = ListJo
+0002b890: 6273 5265 7370 6f6e 7365 426f 6479 2829  bsResponseBody()
+0002b8a0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0002b8b0: 662e 626f 6479 203d 2074 656d 705f 6d6f  f.body = temp_mo
+0002b8c0: 6465 6c2e 6672 6f6d 5f6d 6170 286d 5b27  del.from_map(m['
+0002b8d0: 626f 6479 275d 290a 2020 2020 2020 2020  body']).        
+0002b8e0: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
+0002b8f0: 6173 7320 4c69 7374 5465 6e73 6f72 626f  ass ListTensorbo
+0002b900: 6172 6473 5265 7175 6573 7428 5465 614d  ardsRequest(TeaM
+0002b910: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
+0002b920: 5f69 6e69 745f 5f28 0a20 2020 2020 2020  _init__(.       
+0002b930: 2073 656c 662c 0a20 2020 2020 2020 2064   self,.        d
+0002b940: 6973 706c 6179 5f6e 616d 653a 2073 7472  isplay_name: str
+0002b950: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+0002b960: 2065 6e64 5f74 696d 653a 2073 7472 203d   end_time: str =
+0002b970: 204e 6f6e 652c 0a20 2020 2020 2020 206a   None,.        j
+0002b980: 6f62 5f69 643a 2073 7472 203d 204e 6f6e  ob_id: str = Non
+0002b990: 652c 0a20 2020 2020 2020 206f 7264 6572  e,.        order
+0002b9a0: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+0002b9b0: 2020 2020 2020 7061 6765 5f6e 756d 6265        page_numbe
+0002b9c0: 723a 2069 6e74 203d 204e 6f6e 652c 0a20  r: int = None,. 
+0002b9d0: 2020 2020 2020 2070 6167 655f 7369 7a65         page_size
+0002b9e0: 3a20 696e 7420 3d20 4e6f 6e65 2c0a 2020  : int = None,.  
+0002b9f0: 2020 2020 2020 736f 7274 5f62 793a 2073        sort_by: s
+0002ba00: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
+0002ba10: 2020 2073 6f75 7263 655f 6964 3a20 7374     source_id: st
+0002ba20: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
+0002ba30: 2020 736f 7572 6365 5f74 7970 653a 2073    source_type: s
+0002ba40: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
+0002ba50: 2020 2073 7461 7274 5f74 696d 653a 2073     start_time: s
+0002ba60: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
+0002ba70: 2020 2073 7461 7475 733a 2073 7472 203d     status: str =
+0002ba80: 204e 6f6e 652c 0a20 2020 2020 2020 2074   None,.        t
+0002ba90: 656e 736f 7262 6f61 7264 5f69 643a 2073  ensorboard_id: s
+0002baa0: 7472 203d 204e 6f6e 652c 0a20 2020 2020  tr = None,.     
+0002bab0: 2020 2076 6572 626f 7365 3a20 626f 6f6c     verbose: bool
+0002bac0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+0002bad0: 2077 6f72 6b73 7061 6365 5f69 643a 2073   workspace_id: s
+0002bae0: 7472 203d 204e 6f6e 652c 0a20 2020 2029  tr = None,.    )
+0002baf0: 3a0a 2020 2020 2020 2020 7365 6c66 2e64  :.        self.d
+0002bb00: 6973 706c 6179 5f6e 616d 6520 3d20 6469  isplay_name = di
+0002bb10: 7370 6c61 795f 6e61 6d65 0a20 2020 2020  splay_name.     
+0002bb20: 2020 2073 656c 662e 656e 645f 7469 6d65     self.end_time
+0002bb30: 203d 2065 6e64 5f74 696d 650a 2020 2020   = end_time.    
+0002bb40: 2020 2020 7365 6c66 2e6a 6f62 5f69 6420      self.job_id 
+0002bb50: 3d20 6a6f 625f 6964 0a20 2020 2020 2020  = job_id.       
+0002bb60: 2073 656c 662e 6f72 6465 7220 3d20 6f72   self.order = or
+0002bb70: 6465 720a 2020 2020 2020 2020 7365 6c66  der.        self
+0002bb80: 2e70 6167 655f 6e75 6d62 6572 203d 2070  .page_number = p
+0002bb90: 6167 655f 6e75 6d62 6572 0a20 2020 2020  age_number.     
+0002bba0: 2020 2073 656c 662e 7061 6765 5f73 697a     self.page_siz
+0002bbb0: 6520 3d20 7061 6765 5f73 697a 650a 2020  e = page_size.  
+0002bbc0: 2020 2020 2020 7365 6c66 2e73 6f72 745f        self.sort_
+0002bbd0: 6279 203d 2073 6f72 745f 6279 0a20 2020  by = sort_by.   
+0002bbe0: 2020 2020 2073 656c 662e 736f 7572 6365       self.source
+0002bbf0: 5f69 6420 3d20 736f 7572 6365 5f69 640a  _id = source_id.
+0002bc00: 2020 2020 2020 2020 7365 6c66 2e73 6f75          self.sou
+0002bc10: 7263 655f 7479 7065 203d 2073 6f75 7263  rce_type = sourc
+0002bc20: 655f 7479 7065 0a20 2020 2020 2020 2073  e_type.        s
+0002bc30: 656c 662e 7374 6172 745f 7469 6d65 203d  elf.start_time =
+0002bc40: 2073 7461 7274 5f74 696d 650a 2020 2020   start_time.    
+0002bc50: 2020 2020 7365 6c66 2e73 7461 7475 7320      self.status 
+0002bc60: 3d20 7374 6174 7573 0a20 2020 2020 2020  = status.       
+0002bc70: 2073 656c 662e 7465 6e73 6f72 626f 6172   self.tensorboar
+0002bc80: 645f 6964 203d 2074 656e 736f 7262 6f61  d_id = tensorboa
+0002bc90: 7264 5f69 640a 2020 2020 2020 2020 7365  rd_id.        se
+0002bca0: 6c66 2e76 6572 626f 7365 203d 2076 6572  lf.verbose = ver
+0002bcb0: 626f 7365 0a20 2020 2020 2020 2073 656c  bose.        sel
+0002bcc0: 662e 776f 726b 7370 6163 655f 6964 203d  f.workspace_id =
+0002bcd0: 2077 6f72 6b73 7061 6365 5f69 640a 0a20   workspace_id.. 
+0002bce0: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
+0002bcf0: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
+0002bd00: 6173 730a 0a20 2020 2064 6566 2074 6f5f  ass..    def to_
+0002bd10: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
+0002bd20: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
+0002bd30: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
+0002bd40: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
+0002bd50: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0002bd60: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
+0002bd70: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
+0002bd80: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
+0002bd90: 2069 6620 7365 6c66 2e64 6973 706c 6179   if self.display
+0002bda0: 5f6e 616d 6520 6973 206e 6f74 204e 6f6e  _name is not Non
+0002bdb0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0002bdc0: 6573 756c 745b 2744 6973 706c 6179 4e61  esult['DisplayNa
+0002bdd0: 6d65 275d 203d 2073 656c 662e 6469 7370  me'] = self.disp
+0002bde0: 6c61 795f 6e61 6d65 0a20 2020 2020 2020  lay_name.       
+0002bdf0: 2069 6620 7365 6c66 2e65 6e64 5f74 696d   if self.end_tim
+0002be00: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
+0002be10: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+0002be20: 745b 2745 6e64 5469 6d65 275d 203d 2073  t['EndTime'] = s
+0002be30: 656c 662e 656e 645f 7469 6d65 0a20 2020  elf.end_time.   
+0002be40: 2020 2020 2069 6620 7365 6c66 2e6a 6f62       if self.job
+0002be50: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
+0002be60: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+0002be70: 756c 745b 274a 6f62 4964 275d 203d 2073  ult['JobId'] = s
+0002be80: 656c 662e 6a6f 625f 6964 0a20 2020 2020  elf.job_id.     
+0002be90: 2020 2069 6620 7365 6c66 2e6f 7264 6572     if self.order
+0002bea0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0002beb0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+0002bec0: 5b27 4f72 6465 7227 5d20 3d20 7365 6c66  ['Order'] = self
+0002bed0: 2e6f 7264 6572 0a20 2020 2020 2020 2069  .order.        i
+0002bee0: 6620 7365 6c66 2e70 6167 655f 6e75 6d62  f self.page_numb
+0002bef0: 6572 2069 7320 6e6f 7420 4e6f 6e65 3a0a  er is not None:.
+0002bf00: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+0002bf10: 6c74 5b27 5061 6765 4e75 6d62 6572 275d  lt['PageNumber']
+0002bf20: 203d 2073 656c 662e 7061 6765 5f6e 756d   = self.page_num
+0002bf30: 6265 720a 2020 2020 2020 2020 6966 2073  ber.        if s
+0002bf40: 656c 662e 7061 6765 5f73 697a 6520 6973  elf.page_size is
+0002bf50: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0002bf60: 2020 2020 2020 2072 6573 756c 745b 2750         result['P
+0002bf70: 6167 6553 697a 6527 5d20 3d20 7365 6c66  ageSize'] = self
+0002bf80: 2e70 6167 655f 7369 7a65 0a20 2020 2020  .page_size.     
+0002bf90: 2020 2069 6620 7365 6c66 2e73 6f72 745f     if self.sort_
+0002bfa0: 6279 2069 7320 6e6f 7420 4e6f 6e65 3a0a  by is not None:.
+0002bfb0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+0002bfc0: 6c74 5b27 536f 7274 4279 275d 203d 2073  lt['SortBy'] = s
+0002bfd0: 656c 662e 736f 7274 5f62 790a 2020 2020  elf.sort_by.    
+0002bfe0: 2020 2020 6966 2073 656c 662e 736f 7572      if self.sour
+0002bff0: 6365 5f69 6420 6973 206e 6f74 204e 6f6e  ce_id is not Non
+0002c000: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0002c010: 6573 756c 745b 2753 6f75 7263 6549 6427  esult['SourceId'
+0002c020: 5d20 3d20 7365 6c66 2e73 6f75 7263 655f  ] = self.source_
+0002c030: 6964 0a20 2020 2020 2020 2069 6620 7365  id.        if se
+0002c040: 6c66 2e73 6f75 7263 655f 7479 7065 2069  lf.source_type i
+0002c050: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0002c060: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+0002c070: 536f 7572 6365 5479 7065 275d 203d 2073  SourceType'] = s
+0002c080: 656c 662e 736f 7572 6365 5f74 7970 650a  elf.source_type.
+0002c090: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0002c0a0: 7374 6172 745f 7469 6d65 2069 7320 6e6f  start_time is no
+0002c0b0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0002c0c0: 2020 2020 7265 7375 6c74 5b27 5374 6172      result['Star
+0002c0d0: 7454 696d 6527 5d20 3d20 7365 6c66 2e73  tTime'] = self.s
+0002c0e0: 7461 7274 5f74 696d 650a 2020 2020 2020  tart_time.      
+0002c0f0: 2020 6966 2073 656c 662e 7374 6174 7573    if self.status
+0002c100: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0002c110: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+0002c120: 5b27 5374 6174 7573 275d 203d 2073 656c  ['Status'] = sel
+0002c130: 662e 7374 6174 7573 0a20 2020 2020 2020  f.status.       
+0002c140: 2069 6620 7365 6c66 2e74 656e 736f 7262   if self.tensorb
+0002c150: 6f61 7264 5f69 6420 6973 206e 6f74 204e  oard_id is not N
+0002c160: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0002c170: 2072 6573 756c 745b 2754 656e 736f 7262   result['Tensorb
+0002c180: 6f61 7264 4964 275d 203d 2073 656c 662e  oardId'] = self.
+0002c190: 7465 6e73 6f72 626f 6172 645f 6964 0a20  tensorboard_id. 
+0002c1a0: 2020 2020 2020 2069 6620 7365 6c66 2e76         if self.v
+0002c1b0: 6572 626f 7365 2069 7320 6e6f 7420 4e6f  erbose is not No
+0002c1c0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0002c1d0: 7265 7375 6c74 5b27 5665 7262 6f73 6527  result['Verbose'
+0002c1e0: 5d20 3d20 7365 6c66 2e76 6572 626f 7365  ] = self.verbose
+0002c1f0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0002c200: 2e77 6f72 6b73 7061 6365 5f69 6420 6973  .workspace_id is
+0002c210: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0002c220: 2020 2020 2020 2072 6573 756c 745b 2757         result['W
+0002c230: 6f72 6b73 7061 6365 4964 275d 203d 2073  orkspaceId'] = s
+0002c240: 656c 662e 776f 726b 7370 6163 655f 6964  elf.workspace_id
+0002c250: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0002c260: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
+0002c270: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
+0002c280: 3a20 6469 6374 203d 204e 6f6e 6529 3a0a  : dict = None):.
+0002c290: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
+0002c2a0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+0002c2b0: 6966 206d 2e67 6574 2827 4469 7370 6c61  if m.get('Displa
+0002c2c0: 794e 616d 6527 2920 6973 206e 6f74 204e  yName') is not N
+0002c2d0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0002c2e0: 2073 656c 662e 6469 7370 6c61 795f 6e61   self.display_na
+0002c2f0: 6d65 203d 206d 2e67 6574 2827 4469 7370  me = m.get('Disp
+0002c300: 6c61 794e 616d 6527 290a 2020 2020 2020  layName').      
+0002c310: 2020 6966 206d 2e67 6574 2827 456e 6454    if m.get('EndT
+0002c320: 696d 6527 2920 6973 206e 6f74 204e 6f6e  ime') is not Non
+0002c330: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0002c340: 656c 662e 656e 645f 7469 6d65 203d 206d  elf.end_time = m
+0002c350: 2e67 6574 2827 456e 6454 696d 6527 290a  .get('EndTime').
+0002c360: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+0002c370: 2827 4a6f 6249 6427 2920 6973 206e 6f74  ('JobId') is not
+0002c380: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0002c390: 2020 2073 656c 662e 6a6f 625f 6964 203d     self.job_id =
+0002c3a0: 206d 2e67 6574 2827 4a6f 6249 6427 290a   m.get('JobId').
+0002c3b0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+0002c3c0: 2827 4f72 6465 7227 2920 6973 206e 6f74  ('Order') is not
+0002c3d0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0002c3e0: 2020 2073 656c 662e 6f72 6465 7220 3d20     self.order = 
+0002c3f0: 6d2e 6765 7428 274f 7264 6572 2729 0a20  m.get('Order'). 
+0002c400: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+0002c410: 2750 6167 654e 756d 6265 7227 2920 6973  'PageNumber') is
+0002c420: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0002c430: 2020 2020 2020 2073 656c 662e 7061 6765         self.page
+0002c440: 5f6e 756d 6265 7220 3d20 6d2e 6765 7428  _number = m.get(
+0002c450: 2750 6167 654e 756d 6265 7227 290a 2020  'PageNumber').  
+0002c460: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+0002c470: 5061 6765 5369 7a65 2729 2069 7320 6e6f  PageSize') is no
+0002c480: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0002c490: 2020 2020 7365 6c66 2e70 6167 655f 7369      self.page_si
+0002c4a0: 7a65 203d 206d 2e67 6574 2827 5061 6765  ze = m.get('Page
+0002c4b0: 5369 7a65 2729 0a20 2020 2020 2020 2069  Size').        i
+0002c4c0: 6620 6d2e 6765 7428 2753 6f72 7442 7927  f m.get('SortBy'
+0002c4d0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+0002c4e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0002c4f0: 736f 7274 5f62 7920 3d20 6d2e 6765 7428  sort_by = m.get(
+0002c500: 2753 6f72 7442 7927 290a 2020 2020 2020  'SortBy').      
+0002c510: 2020 6966 206d 2e67 6574 2827 536f 7572    if m.get('Sour
+0002c520: 6365 4964 2729 2069 7320 6e6f 7420 4e6f  ceId') is not No
+0002c530: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0002c540: 7365 6c66 2e73 6f75 7263 655f 6964 203d  self.source_id =
+0002c550: 206d 2e67 6574 2827 536f 7572 6365 4964   m.get('SourceId
+0002c560: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+0002c570: 6765 7428 2753 6f75 7263 6554 7970 6527  get('SourceType'
+0002c580: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+0002c590: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0002c5a0: 736f 7572 6365 5f74 7970 6520 3d20 6d2e  source_type = m.
+0002c5b0: 6765 7428 2753 6f75 7263 6554 7970 6527  get('SourceType'
+0002c5c0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+0002c5d0: 6574 2827 5374 6172 7454 696d 6527 2920  et('StartTime') 
+0002c5e0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0002c5f0: 2020 2020 2020 2020 2073 656c 662e 7374           self.st
+0002c600: 6172 745f 7469 6d65 203d 206d 2e67 6574  art_time = m.get
+0002c610: 2827 5374 6172 7454 696d 6527 290a 2020  ('StartTime').  
+0002c620: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+0002c630: 5374 6174 7573 2729 2069 7320 6e6f 7420  Status') is not 
+0002c640: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0002c650: 2020 7365 6c66 2e73 7461 7475 7320 3d20    self.status = 
+0002c660: 6d2e 6765 7428 2753 7461 7475 7327 290a  m.get('Status').
+0002c670: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+0002c680: 2827 5465 6e73 6f72 626f 6172 6449 6427  ('TensorboardId'
+0002c690: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+0002c6a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0002c6b0: 7465 6e73 6f72 626f 6172 645f 6964 203d  tensorboard_id =
+0002c6c0: 206d 2e67 6574 2827 5465 6e73 6f72 626f   m.get('Tensorbo
+0002c6d0: 6172 6449 6427 290a 2020 2020 2020 2020  ardId').        
+0002c6e0: 6966 206d 2e67 6574 2827 5665 7262 6f73  if m.get('Verbos
+0002c6f0: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
+0002c700: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0002c710: 662e 7665 7262 6f73 6520 3d20 6d2e 6765  f.verbose = m.ge
+0002c720: 7428 2756 6572 626f 7365 2729 0a20 2020  t('Verbose').   
+0002c730: 2020 2020 2069 6620 6d2e 6765 7428 2757       if m.get('W
+0002c740: 6f72 6b73 7061 6365 4964 2729 2069 7320  orkspaceId') is 
+0002c750: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0002c760: 2020 2020 2020 7365 6c66 2e77 6f72 6b73        self.works
+0002c770: 7061 6365 5f69 6420 3d20 6d2e 6765 7428  pace_id = m.get(
+0002c780: 2757 6f72 6b73 7061 6365 4964 2729 0a20  'WorkspaceId'). 
+0002c790: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0002c7a0: 6c66 0a0a 0a63 6c61 7373 204c 6973 7454  lf...class ListT
+0002c7b0: 656e 736f 7262 6f61 7264 7352 6573 706f  ensorboardsRespo
+0002c7c0: 6e73 6542 6f64 7928 5465 614d 6f64 656c  nseBody(TeaModel
+0002c7d0: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
+0002c7e0: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
+0002c7f0: 662c 0a20 2020 2020 2020 2072 6571 7565  f,.        reque
+0002c800: 7374 5f69 643a 2073 7472 203d 204e 6f6e  st_id: str = Non
+0002c810: 652c 0a20 2020 2020 2020 2074 656e 736f  e,.        tenso
+0002c820: 7262 6f61 7264 733a 204c 6973 745b 5465  rboards: List[Te
+0002c830: 6e73 6f72 626f 6172 645d 203d 204e 6f6e  nsorboard] = Non
+0002c840: 652c 0a20 2020 2020 2020 2074 6f74 616c  e,.        total
+0002c850: 5f63 6f75 6e74 3a20 696e 7420 3d20 4e6f  _count: int = No
+0002c860: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
+0002c870: 2020 2073 656c 662e 7265 7175 6573 745f     self.request_
+0002c880: 6964 203d 2072 6571 7565 7374 5f69 640a  id = request_id.
+0002c890: 2020 2020 2020 2020 7365 6c66 2e74 656e          self.ten
+0002c8a0: 736f 7262 6f61 7264 7320 3d20 7465 6e73  sorboards = tens
+0002c8b0: 6f72 626f 6172 6473 0a20 2020 2020 2020  orboards.       
+0002c8c0: 2073 656c 662e 746f 7461 6c5f 636f 756e   self.total_coun
+0002c8d0: 7420 3d20 746f 7461 6c5f 636f 756e 740a  t = total_count.
+0002c8e0: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
+0002c8f0: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+0002c900: 2069 6620 7365 6c66 2e74 656e 736f 7262   if self.tensorb
+0002c910: 6f61 7264 733a 0a20 2020 2020 2020 2020  oards:.         
+0002c920: 2020 2066 6f72 206b 2069 6e20 7365 6c66     for k in self
+0002c930: 2e74 656e 736f 7262 6f61 7264 733a 0a20  .tensorboards:. 
+0002c940: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0002c950: 6620 6b3a 0a20 2020 2020 2020 2020 2020  f k:.           
+0002c960: 2020 2020 2020 2020 206b 2e76 616c 6964           k.valid
+0002c970: 6174 6528 290a 0a20 2020 2064 6566 2074  ate()..    def t
+0002c980: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
+0002c990: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
+0002c9a0: 7228 292e 746f 5f6d 6170 2829 0a20 2020  r().to_map().   
+0002c9b0: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
+0002c9c0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0002c9d0: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
+0002c9e0: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
+0002c9f0: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
+0002ca00: 2020 2069 6620 7365 6c66 2e72 6571 7565     if self.reque
+0002ca10: 7374 5f69 6420 6973 206e 6f74 204e 6f6e  st_id is not Non
+0002ca20: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0002ca30: 6573 756c 745b 2752 6571 7565 7374 4964  esult['RequestId
+0002ca40: 275d 203d 2073 656c 662e 7265 7175 6573  '] = self.reques
+0002ca50: 745f 6964 0a20 2020 2020 2020 2072 6573  t_id.        res
+0002ca60: 756c 745b 2754 656e 736f 7262 6f61 7264  ult['Tensorboard
+0002ca70: 7327 5d20 3d20 5b5d 0a20 2020 2020 2020  s'] = [].       
+0002ca80: 2069 6620 7365 6c66 2e74 656e 736f 7262   if self.tensorb
+0002ca90: 6f61 7264 7320 6973 206e 6f74 204e 6f6e  oards is not Non
+0002caa0: 653a 0a20 2020 2020 2020 2020 2020 2066  e:.            f
+0002cab0: 6f72 206b 2069 6e20 7365 6c66 2e74 656e  or k in self.ten
+0002cac0: 736f 7262 6f61 7264 733a 0a20 2020 2020  sorboards:.     
+0002cad0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+0002cae0: 745b 2754 656e 736f 7262 6f61 7264 7327  t['Tensorboards'
+0002caf0: 5d2e 6170 7065 6e64 286b 2e74 6f5f 6d61  ].append(k.to_ma
+0002cb00: 7028 2920 6966 206b 2065 6c73 6520 4e6f  p() if k else No
+0002cb10: 6e65 290a 2020 2020 2020 2020 6966 2073  ne).        if s
+0002cb20: 656c 662e 746f 7461 6c5f 636f 756e 7420  elf.total_count 
+0002cb30: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0002cb40: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+0002cb50: 2754 6f74 616c 436f 756e 7427 5d20 3d20  'TotalCount'] = 
+0002cb60: 7365 6c66 2e74 6f74 616c 5f63 6f75 6e74  self.total_count
+0002cb70: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0002cb80: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
+0002cb90: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
+0002cba0: 3a20 6469 6374 203d 204e 6f6e 6529 3a0a  : dict = None):.
+0002cbb0: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
+0002cbc0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+0002cbd0: 6966 206d 2e67 6574 2827 5265 7175 6573  if m.get('Reques
+0002cbe0: 7449 6427 2920 6973 206e 6f74 204e 6f6e  tId') is not Non
+0002cbf0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0002cc00: 656c 662e 7265 7175 6573 745f 6964 203d  elf.request_id =
+0002cc10: 206d 2e67 6574 2827 5265 7175 6573 7449   m.get('RequestI
+0002cc20: 6427 290a 2020 2020 2020 2020 7365 6c66  d').        self
+0002cc30: 2e74 656e 736f 7262 6f61 7264 7320 3d20  .tensorboards = 
+0002cc40: 5b5d 0a20 2020 2020 2020 2069 6620 6d2e  [].        if m.
+0002cc50: 6765 7428 2754 656e 736f 7262 6f61 7264  get('Tensorboard
+0002cc60: 7327 2920 6973 206e 6f74 204e 6f6e 653a  s') is not None:
+0002cc70: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+0002cc80: 206b 2069 6e20 6d2e 6765 7428 2754 656e   k in m.get('Ten
+0002cc90: 736f 7262 6f61 7264 7327 293a 0a20 2020  sorboards'):.   
+0002cca0: 2020 2020 2020 2020 2020 2020 2074 656d               tem
+0002ccb0: 705f 6d6f 6465 6c20 3d20 5465 6e73 6f72  p_model = Tensor
+0002ccc0: 626f 6172 6428 290a 2020 2020 2020 2020  board().        
+0002ccd0: 2020 2020 2020 2020 7365 6c66 2e74 656e          self.ten
+0002cce0: 736f 7262 6f61 7264 732e 6170 7065 6e64  sorboards.append
+0002ccf0: 2874 656d 705f 6d6f 6465 6c2e 6672 6f6d  (temp_model.from
+0002cd00: 5f6d 6170 286b 2929 0a20 2020 2020 2020  _map(k)).       
+0002cd10: 2069 6620 6d2e 6765 7428 2754 6f74 616c   if m.get('Total
+0002cd20: 436f 756e 7427 2920 6973 206e 6f74 204e  Count') is not N
+0002cd30: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0002cd40: 2073 656c 662e 746f 7461 6c5f 636f 756e   self.total_coun
+0002cd50: 7420 3d20 6d2e 6765 7428 2754 6f74 616c  t = m.get('Total
+0002cd60: 436f 756e 7427 290a 2020 2020 2020 2020  Count').        
+0002cd70: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
+0002cd80: 6173 7320 4c69 7374 5465 6e73 6f72 626f  ass ListTensorbo
+0002cd90: 6172 6473 5265 7370 6f6e 7365 2854 6561  ardsResponse(Tea
+0002cda0: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
+0002cdb0: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
+0002cdc0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+0002cdd0: 6865 6164 6572 733a 2044 6963 745b 7374  headers: Dict[st
+0002cde0: 722c 2073 7472 5d20 3d20 4e6f 6e65 2c0a  r, str] = None,.
+0002cdf0: 2020 2020 2020 2020 7374 6174 7573 5f63          status_c
+0002ce00: 6f64 653a 2069 6e74 203d 204e 6f6e 652c  ode: int = None,
+0002ce10: 0a20 2020 2020 2020 2062 6f64 793a 204c  .        body: L
+0002ce20: 6973 7454 656e 736f 7262 6f61 7264 7352  istTensorboardsR
+0002ce30: 6573 706f 6e73 6542 6f64 7920 3d20 4e6f  esponseBody = No
+0002ce40: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
+0002ce50: 2020 2073 656c 662e 6865 6164 6572 7320     self.headers 
+0002ce60: 3d20 6865 6164 6572 730a 2020 2020 2020  = headers.      
+0002ce70: 2020 7365 6c66 2e73 7461 7475 735f 636f    self.status_co
+0002ce80: 6465 203d 2073 7461 7475 735f 636f 6465  de = status_code
+0002ce90: 0a20 2020 2020 2020 2073 656c 662e 626f  .        self.bo
+0002cea0: 6479 203d 2062 6f64 790a 0a20 2020 2064  dy = body..    d
+0002ceb0: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
+0002cec0: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+0002ced0: 7661 6c69 6461 7465 5f72 6571 7569 7265  validate_require
+0002cee0: 6428 7365 6c66 2e68 6561 6465 7273 2c20  d(self.headers, 
+0002cef0: 2768 6561 6465 7273 2729 0a20 2020 2020  'headers').     
+0002cf00: 2020 2073 656c 662e 7661 6c69 6461 7465     self.validate
+0002cf10: 5f72 6571 7569 7265 6428 7365 6c66 2e73  _required(self.s
+0002cf20: 7461 7475 735f 636f 6465 2c20 2773 7461  tatus_code, 'sta
+0002cf30: 7475 735f 636f 6465 2729 0a20 2020 2020  tus_code').     
+0002cf40: 2020 2073 656c 662e 7661 6c69 6461 7465     self.validate
+0002cf50: 5f72 6571 7569 7265 6428 7365 6c66 2e62  _required(self.b
+0002cf60: 6f64 792c 2027 626f 6479 2729 0a20 2020  ody, 'body').   
+0002cf70: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
+0002cf80: 793a 0a20 2020 2020 2020 2020 2020 2073  y:.            s
+0002cf90: 656c 662e 626f 6479 2e76 616c 6964 6174  elf.body.validat
+0002cfa0: 6528 290a 0a20 2020 2064 6566 2074 6f5f  e()..    def to_
+0002cfb0: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
+0002cfc0: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
+0002cfd0: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
+0002cfe0: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
+0002cff0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0002d000: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
+0002d010: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
+0002d020: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
+0002d030: 2069 6620 7365 6c66 2e68 6561 6465 7273   if self.headers
+0002d040: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0002d050: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+0002d060: 5b27 6865 6164 6572 7327 5d20 3d20 7365  ['headers'] = se
+0002d070: 6c66 2e68 6561 6465 7273 0a20 2020 2020  lf.headers.     
+0002d080: 2020 2069 6620 7365 6c66 2e73 7461 7475     if self.statu
+0002d090: 735f 636f 6465 2069 7320 6e6f 7420 4e6f  s_code is not No
+0002d0a0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0002d0b0: 7265 7375 6c74 5b27 7374 6174 7573 436f  result['statusCo
+0002d0c0: 6465 275d 203d 2073 656c 662e 7374 6174  de'] = self.stat
+0002d0d0: 7573 5f63 6f64 650a 2020 2020 2020 2020  us_code.        
+0002d0e0: 6966 2073 656c 662e 626f 6479 2069 7320  if self.body is 
+0002d0f0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0002d100: 2020 2020 2020 7265 7375 6c74 5b27 626f        result['bo
+0002d110: 6479 275d 203d 2073 656c 662e 626f 6479  dy'] = self.body
+0002d120: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
+0002d130: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
+0002d140: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
+0002d150: 7028 7365 6c66 2c20 6d3a 2064 6963 7420  p(self, m: dict 
+0002d160: 3d20 4e6f 6e65 293a 0a20 2020 2020 2020  = None):.       
+0002d170: 206d 203d 206d 206f 7220 6469 6374 2829   m = m or dict()
+0002d180: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+0002d190: 7428 2768 6561 6465 7273 2729 2069 7320  t('headers') is 
+0002d1a0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0002d1b0: 2020 2020 2020 7365 6c66 2e68 6561 6465        self.heade
+0002d1c0: 7273 203d 206d 2e67 6574 2827 6865 6164  rs = m.get('head
+0002d1d0: 6572 7327 290a 2020 2020 2020 2020 6966  ers').        if
+0002d1e0: 206d 2e67 6574 2827 7374 6174 7573 436f   m.get('statusCo
+0002d1f0: 6465 2729 2069 7320 6e6f 7420 4e6f 6e65  de') is not None
+0002d200: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0002d210: 6c66 2e73 7461 7475 735f 636f 6465 203d  lf.status_code =
+0002d220: 206d 2e67 6574 2827 7374 6174 7573 436f   m.get('statusCo
+0002d230: 6465 2729 0a20 2020 2020 2020 2069 6620  de').        if 
+0002d240: 6d2e 6765 7428 2762 6f64 7927 2920 6973  m.get('body') is
+0002d250: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0002d260: 2020 2020 2020 2074 656d 705f 6d6f 6465         temp_mode
+0002d270: 6c20 3d20 4c69 7374 5465 6e73 6f72 626f  l = ListTensorbo
+0002d280: 6172 6473 5265 7370 6f6e 7365 426f 6479  ardsResponseBody
+0002d290: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
+0002d2a0: 656c 662e 626f 6479 203d 2074 656d 705f  elf.body = temp_
+0002d2b0: 6d6f 6465 6c2e 6672 6f6d 5f6d 6170 286d  model.from_map(m
+0002d2c0: 5b27 626f 6479 275d 290a 2020 2020 2020  ['body']).      
+0002d2d0: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
+0002d2e0: 636c 6173 7320 5374 6172 7454 656e 736f  class StartTenso
+0002d2f0: 7262 6f61 7264 5265 7175 6573 7428 5465  rboardRequest(Te
+0002d300: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
+0002d310: 205f 5f69 6e69 745f 5f28 0a20 2020 2020   __init__(.     
+0002d320: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+0002d330: 2077 6f72 6b73 7061 6365 5f69 643a 2073   workspace_id: s
+0002d340: 7472 203d 204e 6f6e 652c 0a20 2020 2029  tr = None,.    )
+0002d350: 3a0a 2020 2020 2020 2020 7365 6c66 2e77  :.        self.w
+0002d360: 6f72 6b73 7061 6365 5f69 6420 3d20 776f  orkspace_id = wo
+0002d370: 726b 7370 6163 655f 6964 0a0a 2020 2020  rkspace_id..    
+0002d380: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
+0002d390: 6629 3a0a 2020 2020 2020 2020 7061 7373  f):.        pass
+0002d3a0: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
+0002d3b0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0002d3c0: 5f6d 6170 203d 2073 7570 6572 2829 2e74  _map = super().t
+0002d3d0: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
+0002d3e0: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
+0002d3f0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0002d400: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
+0002d410: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
+0002d420: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+0002d430: 2073 656c 662e 776f 726b 7370 6163 655f   self.workspace_
+0002d440: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
+0002d450: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+0002d460: 6c74 5b27 576f 726b 7370 6163 6549 6427  lt['WorkspaceId'
+0002d470: 5d20 3d20 7365 6c66 2e77 6f72 6b73 7061  ] = self.workspa
+0002d480: 6365 5f69 640a 2020 2020 2020 2020 7265  ce_id.        re
+0002d490: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
+0002d4a0: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
+0002d4b0: 6c66 2c20 6d3a 2064 6963 7420 3d20 4e6f  lf, m: dict = No
+0002d4c0: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
+0002d4d0: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
+0002d4e0: 2020 2020 2069 6620 6d2e 6765 7428 2757       if m.get('W
+0002d4f0: 6f72 6b73 7061 6365 4964 2729 2069 7320  orkspaceId') is 
+0002d500: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0002d510: 2020 2020 2020 7365 6c66 2e77 6f72 6b73        self.works
+0002d520: 7061 6365 5f69 6420 3d20 6d2e 6765 7428  pace_id = m.get(
+0002d530: 2757 6f72 6b73 7061 6365 4964 2729 0a20  'WorkspaceId'). 
+0002d540: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0002d550: 6c66 0a0a 0a63 6c61 7373 2053 7461 7274  lf...class Start
+0002d560: 5465 6e73 6f72 626f 6172 6452 6573 706f  TensorboardRespo
+0002d570: 6e73 6542 6f64 7928 5465 614d 6f64 656c  nseBody(TeaModel
+0002d580: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
+0002d590: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
+0002d5a0: 662c 0a20 2020 2020 2020 2072 6571 7565  f,.        reque
+0002d5b0: 7374 5f69 643a 2073 7472 203d 204e 6f6e  st_id: str = Non
+0002d5c0: 652c 0a20 2020 2020 2020 2074 656e 736f  e,.        tenso
+0002d5d0: 7262 6f61 7264 5f69 643a 2073 7472 203d  rboard_id: str =
+0002d5e0: 204e 6f6e 652c 0a20 2020 2029 3a0a 2020   None,.    ):.  
+0002d5f0: 2020 2020 2020 7365 6c66 2e72 6571 7565        self.reque
+0002d600: 7374 5f69 6420 3d20 7265 7175 6573 745f  st_id = request_
+0002d610: 6964 0a20 2020 2020 2020 2073 656c 662e  id.        self.
+0002d620: 7465 6e73 6f72 626f 6172 645f 6964 203d  tensorboard_id =
+0002d630: 2074 656e 736f 7262 6f61 7264 5f69 640a   tensorboard_id.
+0002d640: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
+0002d650: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
+0002d660: 2070 6173 730a 0a20 2020 2064 6566 2074   pass..    def t
+0002d670: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
+0002d680: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
+0002d690: 7228 292e 746f 5f6d 6170 2829 0a20 2020  r().to_map().   
+0002d6a0: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
+0002d6b0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0002d6c0: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
+0002d6d0: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
+0002d6e0: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
+0002d6f0: 2020 2069 6620 7365 6c66 2e72 6571 7565     if self.reque
+0002d700: 7374 5f69 6420 6973 206e 6f74 204e 6f6e  st_id is not Non
+0002d710: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0002d720: 6573 756c 745b 2752 6571 7565 7374 4964  esult['RequestId
+0002d730: 275d 203d 2073 656c 662e 7265 7175 6573  '] = self.reques
+0002d740: 745f 6964 0a20 2020 2020 2020 2069 6620  t_id.        if 
+0002d750: 7365 6c66 2e74 656e 736f 7262 6f61 7264  self.tensorboard
+0002d760: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
+0002d770: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+0002d780: 756c 745b 2754 656e 736f 7262 6f61 7264  ult['Tensorboard
+0002d790: 4964 275d 203d 2073 656c 662e 7465 6e73  Id'] = self.tens
+0002d7a0: 6f72 626f 6172 645f 6964 0a20 2020 2020  orboard_id.     
+0002d7b0: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
+0002d7c0: 0a0a 2020 2020 6465 6620 6672 6f6d 5f6d  ..    def from_m
+0002d7d0: 6170 2873 656c 662c 206d 3a20 6469 6374  ap(self, m: dict
+0002d7e0: 203d 204e 6f6e 6529 3a0a 2020 2020 2020   = None):.      
+0002d7f0: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
+0002d800: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+0002d810: 6574 2827 5265 7175 6573 7449 6427 2920  et('RequestId') 
+0002d820: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0002d830: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
+0002d840: 7175 6573 745f 6964 203d 206d 2e67 6574  quest_id = m.get
+0002d850: 2827 5265 7175 6573 7449 6427 290a 2020  ('RequestId').  
+0002d860: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+0002d870: 5465 6e73 6f72 626f 6172 6449 6427 2920  TensorboardId') 
+0002d880: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0002d890: 2020 2020 2020 2020 2073 656c 662e 7465           self.te
+0002d8a0: 6e73 6f72 626f 6172 645f 6964 203d 206d  nsorboard_id = m
+0002d8b0: 2e67 6574 2827 5465 6e73 6f72 626f 6172  .get('Tensorboar
+0002d8c0: 6449 6427 290a 2020 2020 2020 2020 7265  dId').        re
+0002d8d0: 7475 726e 2073 656c 660a 0a0a 636c 6173  turn self...clas
+0002d8e0: 7320 5374 6172 7454 656e 736f 7262 6f61  s StartTensorboa
+0002d8f0: 7264 5265 7370 6f6e 7365 2854 6561 4d6f  rdResponse(TeaMo
+0002d900: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
+0002d910: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
+0002d920: 7365 6c66 2c0a 2020 2020 2020 2020 6865  self,.        he
+0002d930: 6164 6572 733a 2044 6963 745b 7374 722c  aders: Dict[str,
+0002d940: 2073 7472 5d20 3d20 4e6f 6e65 2c0a 2020   str] = None,.  
+0002d950: 2020 2020 2020 7374 6174 7573 5f63 6f64        status_cod
+0002d960: 653a 2069 6e74 203d 204e 6f6e 652c 0a20  e: int = None,. 
+0002d970: 2020 2020 2020 2062 6f64 793a 2053 7461         body: Sta
+0002d980: 7274 5465 6e73 6f72 626f 6172 6452 6573  rtTensorboardRes
+0002d990: 706f 6e73 6542 6f64 7920 3d20 4e6f 6e65  ponseBody = None
+0002d9a0: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
+0002d9b0: 2073 656c 662e 6865 6164 6572 7320 3d20   self.headers = 
+0002d9c0: 6865 6164 6572 730a 2020 2020 2020 2020  headers.        
+0002d9d0: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
+0002d9e0: 203d 2073 7461 7475 735f 636f 6465 0a20   = status_code. 
+0002d9f0: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
+0002da00: 203d 2062 6f64 790a 0a20 2020 2064 6566   = body..    def
+0002da10: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
+0002da20: 0a20 2020 2020 2020 2073 656c 662e 7661  .        self.va
+0002da30: 6c69 6461 7465 5f72 6571 7569 7265 6428  lidate_required(
+0002da40: 7365 6c66 2e68 6561 6465 7273 2c20 2768  self.headers, 'h
+0002da50: 6561 6465 7273 2729 0a20 2020 2020 2020  eaders').       
+0002da60: 2073 656c 662e 7661 6c69 6461 7465 5f72   self.validate_r
+0002da70: 6571 7569 7265 6428 7365 6c66 2e73 7461  equired(self.sta
+0002da80: 7475 735f 636f 6465 2c20 2773 7461 7475  tus_code, 'statu
+0002da90: 735f 636f 6465 2729 0a20 2020 2020 2020  s_code').       
+0002daa0: 2073 656c 662e 7661 6c69 6461 7465 5f72   self.validate_r
+0002dab0: 6571 7569 7265 6428 7365 6c66 2e62 6f64  equired(self.bod
+0002dac0: 792c 2027 626f 6479 2729 0a20 2020 2020  y, 'body').     
+0002dad0: 2020 2069 6620 7365 6c66 2e62 6f64 793a     if self.body:
+0002dae0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0002daf0: 662e 626f 6479 2e76 616c 6964 6174 6528  f.body.validate(
+0002db00: 290a 0a20 2020 2064 6566 2074 6f5f 6d61  )..    def to_ma
+0002db10: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
+0002db20: 205f 6d61 7020 3d20 7375 7065 7228 292e   _map = super().
+0002db30: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
+0002db40: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
+0002db50: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0002db60: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
+0002db70: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+0002db80: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+0002db90: 6620 7365 6c66 2e68 6561 6465 7273 2069  f self.headers i
+0002dba0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0002dbb0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+0002dbc0: 6865 6164 6572 7327 5d20 3d20 7365 6c66  headers'] = self
+0002dbd0: 2e68 6561 6465 7273 0a20 2020 2020 2020  .headers.       
+0002dbe0: 2069 6620 7365 6c66 2e73 7461 7475 735f   if self.status_
+0002dbf0: 636f 6465 2069 7320 6e6f 7420 4e6f 6e65  code is not None
+0002dc00: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0002dc10: 7375 6c74 5b27 7374 6174 7573 436f 6465  sult['statusCode
+0002dc20: 275d 203d 2073 656c 662e 7374 6174 7573  '] = self.status
+0002dc30: 5f63 6f64 650a 2020 2020 2020 2020 6966  _code.        if
+0002dc40: 2073 656c 662e 626f 6479 2069 7320 6e6f   self.body is no
+0002dc50: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0002dc60: 2020 2020 7265 7375 6c74 5b27 626f 6479      result['body
+0002dc70: 275d 203d 2073 656c 662e 626f 6479 2e74  '] = self.body.t
+0002dc80: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
+0002dc90: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
+0002dca0: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
+0002dcb0: 7365 6c66 2c20 6d3a 2064 6963 7420 3d20  self, m: dict = 
+0002dcc0: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
+0002dcd0: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
+0002dce0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+0002dcf0: 2768 6561 6465 7273 2729 2069 7320 6e6f  'headers') is no
+0002dd00: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0002dd10: 2020 2020 7365 6c66 2e68 6561 6465 7273      self.headers
+0002dd20: 203d 206d 2e67 6574 2827 6865 6164 6572   = m.get('header
+0002dd30: 7327 290a 2020 2020 2020 2020 6966 206d  s').        if m
+0002dd40: 2e67 6574 2827 7374 6174 7573 436f 6465  .get('statusCode
+0002dd50: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+0002dd60: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0002dd70: 2e73 7461 7475 735f 636f 6465 203d 206d  .status_code = m
+0002dd80: 2e67 6574 2827 7374 6174 7573 436f 6465  .get('statusCode
+0002dd90: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+0002dda0: 6765 7428 2762 6f64 7927 2920 6973 206e  get('body') is n
+0002ddb0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0002ddc0: 2020 2020 2074 656d 705f 6d6f 6465 6c20       temp_model 
+0002ddd0: 3d20 5374 6172 7454 656e 736f 7262 6f61  = StartTensorboa
+0002dde0: 7264 5265 7370 6f6e 7365 426f 6479 2829  rdResponseBody()
+0002ddf0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0002de00: 662e 626f 6479 203d 2074 656d 705f 6d6f  f.body = temp_mo
+0002de10: 6465 6c2e 6672 6f6d 5f6d 6170 286d 5b27  del.from_map(m['
+0002de20: 626f 6479 275d 290a 2020 2020 2020 2020  body']).        
+0002de30: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
+0002de40: 6173 7320 5374 6f70 4a6f 6252 6573 706f  ass StopJobRespo
+0002de50: 6e73 6542 6f64 7928 5465 614d 6f64 656c  nseBody(TeaModel
+0002de60: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
+0002de70: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
+0002de80: 662c 0a20 2020 2020 2020 206a 6f62 5f69  f,.        job_i
+0002de90: 643a 2073 7472 203d 204e 6f6e 652c 0a20  d: str = None,. 
+0002dea0: 2020 2020 2020 2072 6571 7565 7374 5f69         request_i
+0002deb0: 643a 2073 7472 203d 204e 6f6e 652c 0a20  d: str = None,. 
+0002dec0: 2020 2029 3a0a 2020 2020 2020 2020 7365     ):.        se
+0002ded0: 6c66 2e6a 6f62 5f69 6420 3d20 6a6f 625f  lf.job_id = job_
+0002dee0: 6964 0a20 2020 2020 2020 2073 656c 662e  id.        self.
+0002def0: 7265 7175 6573 745f 6964 203d 2072 6571  request_id = req
+0002df00: 7565 7374 5f69 640a 0a20 2020 2064 6566  uest_id..    def
+0002df10: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
+0002df20: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
+0002df30: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
+0002df40: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
+0002df50: 7020 3d20 7375 7065 7228 292e 746f 5f6d  p = super().to_m
+0002df60: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
+0002df70: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
+0002df80: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0002df90: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
+0002dfa0: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
+0002dfb0: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
+0002dfc0: 6c66 2e6a 6f62 5f69 6420 6973 206e 6f74  lf.job_id is not
+0002dfd0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0002dfe0: 2020 2072 6573 756c 745b 274a 6f62 4964     result['JobId
+0002dff0: 275d 203d 2073 656c 662e 6a6f 625f 6964  '] = self.job_id
+0002e000: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0002e010: 2e72 6571 7565 7374 5f69 6420 6973 206e  .request_id is n
+0002e020: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0002e030: 2020 2020 2072 6573 756c 745b 2752 6571       result['Req
+0002e040: 7565 7374 4964 275d 203d 2073 656c 662e  uestId'] = self.
+0002e050: 7265 7175 6573 745f 6964 0a20 2020 2020  request_id.     
+0002e060: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
+0002e070: 0a0a 2020 2020 6465 6620 6672 6f6d 5f6d  ..    def from_m
+0002e080: 6170 2873 656c 662c 206d 3a20 6469 6374  ap(self, m: dict
+0002e090: 203d 204e 6f6e 6529 3a0a 2020 2020 2020   = None):.      
+0002e0a0: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
+0002e0b0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+0002e0c0: 6574 2827 4a6f 6249 6427 2920 6973 206e  et('JobId') is n
+0002e0d0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0002e0e0: 2020 2020 2073 656c 662e 6a6f 625f 6964       self.job_id
+0002e0f0: 203d 206d 2e67 6574 2827 4a6f 6249 6427   = m.get('JobId'
+0002e100: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+0002e110: 6574 2827 5265 7175 6573 7449 6427 2920  et('RequestId') 
+0002e120: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0002e130: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
+0002e140: 7175 6573 745f 6964 203d 206d 2e67 6574  quest_id = m.get
+0002e150: 2827 5265 7175 6573 7449 6427 290a 2020  ('RequestId').  
+0002e160: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0002e170: 660a 0a0a 636c 6173 7320 5374 6f70 4a6f  f...class StopJo
+0002e180: 6252 6573 706f 6e73 6528 5465 614d 6f64  bResponse(TeaMod
+0002e190: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
+0002e1a0: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
+0002e1b0: 656c 662c 0a20 2020 2020 2020 2068 6561  elf,.        hea
+0002e1c0: 6465 7273 3a20 4469 6374 5b73 7472 2c20  ders: Dict[str, 
+0002e1d0: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
+0002e1e0: 2020 2020 2073 7461 7475 735f 636f 6465       status_code
+0002e1f0: 3a20 696e 7420 3d20 4e6f 6e65 2c0a 2020  : int = None,.  
+0002e200: 2020 2020 2020 626f 6479 3a20 5374 6f70        body: Stop
+0002e210: 4a6f 6252 6573 706f 6e73 6542 6f64 7920  JobResponseBody 
+0002e220: 3d20 4e6f 6e65 2c0a 2020 2020 293a 0a20  = None,.    ):. 
+0002e230: 2020 2020 2020 2073 656c 662e 6865 6164         self.head
+0002e240: 6572 7320 3d20 6865 6164 6572 730a 2020  ers = headers.  
+0002e250: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
+0002e260: 735f 636f 6465 203d 2073 7461 7475 735f  s_code = status_
+0002e270: 636f 6465 0a20 2020 2020 2020 2073 656c  code.        sel
+0002e280: 662e 626f 6479 203d 2062 6f64 790a 0a20  f.body = body.. 
+0002e290: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
+0002e2a0: 7365 6c66 293a 0a20 2020 2020 2020 2073  self):.        s
+0002e2b0: 656c 662e 7661 6c69 6461 7465 5f72 6571  elf.validate_req
+0002e2c0: 7569 7265 6428 7365 6c66 2e68 6561 6465  uired(self.heade
+0002e2d0: 7273 2c20 2768 6561 6465 7273 2729 0a20  rs, 'headers'). 
+0002e2e0: 2020 2020 2020 2073 656c 662e 7661 6c69         self.vali
+0002e2f0: 6461 7465 5f72 6571 7569 7265 6428 7365  date_required(se
+0002e300: 6c66 2e73 7461 7475 735f 636f 6465 2c20  lf.status_code, 
+0002e310: 2773 7461 7475 735f 636f 6465 2729 0a20  'status_code'). 
+0002e320: 2020 2020 2020 2073 656c 662e 7661 6c69         self.vali
+0002e330: 6461 7465 5f72 6571 7569 7265 6428 7365  date_required(se
+0002e340: 6c66 2e62 6f64 792c 2027 626f 6479 2729  lf.body, 'body')
+0002e350: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0002e360: 2e62 6f64 793a 0a20 2020 2020 2020 2020  .body:.         
+0002e370: 2020 2073 656c 662e 626f 6479 2e76 616c     self.body.val
+0002e380: 6964 6174 6528 290a 0a20 2020 2064 6566  idate()..    def
+0002e390: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
+0002e3a0: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
+0002e3b0: 7065 7228 292e 746f 5f6d 6170 2829 0a20  per().to_map(). 
+0002e3c0: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
+0002e3d0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0002e3e0: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+0002e3f0: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
+0002e400: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
+0002e410: 2020 2020 2069 6620 7365 6c66 2e68 6561       if self.hea
+0002e420: 6465 7273 2069 7320 6e6f 7420 4e6f 6e65  ders is not None
+0002e430: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0002e440: 7375 6c74 5b27 6865 6164 6572 7327 5d20  sult['headers'] 
+0002e450: 3d20 7365 6c66 2e68 6561 6465 7273 0a20  = self.headers. 
+0002e460: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
+0002e470: 7461 7475 735f 636f 6465 2069 7320 6e6f  tatus_code is no
+0002e480: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0002e490: 2020 2020 7265 7375 6c74 5b27 7374 6174      result['stat
+0002e4a0: 7573 436f 6465 275d 203d 2073 656c 662e  usCode'] = self.
+0002e4b0: 7374 6174 7573 5f63 6f64 650a 2020 2020  status_code.    
+0002e4c0: 2020 2020 6966 2073 656c 662e 626f 6479      if self.body
+0002e4d0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0002e4e0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+0002e4f0: 5b27 626f 6479 275d 203d 2073 656c 662e  ['body'] = self.
+0002e500: 626f 6479 2e74 6f5f 6d61 7028 290a 2020  body.to_map().  
+0002e510: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+0002e520: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
+0002e530: 6d5f 6d61 7028 7365 6c66 2c20 6d3a 2064  m_map(self, m: d
+0002e540: 6963 7420 3d20 4e6f 6e65 293a 0a20 2020  ict = None):.   
+0002e550: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
+0002e560: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+0002e570: 6d2e 6765 7428 2768 6561 6465 7273 2729  m.get('headers')
+0002e580: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0002e590: 2020 2020 2020 2020 2020 7365 6c66 2e68            self.h
+0002e5a0: 6561 6465 7273 203d 206d 2e67 6574 2827  eaders = m.get('
+0002e5b0: 6865 6164 6572 7327 290a 2020 2020 2020  headers').      
+0002e5c0: 2020 6966 206d 2e67 6574 2827 7374 6174    if m.get('stat
+0002e5d0: 7573 436f 6465 2729 2069 7320 6e6f 7420  usCode') is not 
+0002e5e0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0002e5f0: 2020 7365 6c66 2e73 7461 7475 735f 636f    self.status_co
+0002e600: 6465 203d 206d 2e67 6574 2827 7374 6174  de = m.get('stat
+0002e610: 7573 436f 6465 2729 0a20 2020 2020 2020  usCode').       
+0002e620: 2069 6620 6d2e 6765 7428 2762 6f64 7927   if m.get('body'
+0002e630: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+0002e640: 2020 2020 2020 2020 2020 2074 656d 705f             temp_
+0002e650: 6d6f 6465 6c20 3d20 5374 6f70 4a6f 6252  model = StopJobR
+0002e660: 6573 706f 6e73 6542 6f64 7928 290a 2020  esponseBody().  
+0002e670: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
+0002e680: 6f64 7920 3d20 7465 6d70 5f6d 6f64 656c  ody = temp_model
+0002e690: 2e66 726f 6d5f 6d61 7028 6d5b 2762 6f64  .from_map(m['bod
+0002e6a0: 7927 5d29 0a20 2020 2020 2020 2072 6574  y']).        ret
+0002e6b0: 7572 6e20 7365 6c66 0a0a 0a63 6c61 7373  urn self...class
+0002e6c0: 2053 746f 7054 656e 736f 7262 6f61 7264   StopTensorboard
+0002e6d0: 5265 7175 6573 7428 5465 614d 6f64 656c  Request(TeaModel
+0002e6e0: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
+0002e6f0: 745f 5f28 0a20 2020 2020 2020 2073 656c  t__(.        sel
+0002e700: 662c 0a20 2020 2020 2020 2077 6f72 6b73  f,.        works
+0002e710: 7061 6365 5f69 643a 2073 7472 203d 204e  pace_id: str = N
+0002e720: 6f6e 652c 0a20 2020 2029 3a0a 2020 2020  one,.    ):.    
+0002e730: 2020 2020 7365 6c66 2e77 6f72 6b73 7061      self.workspa
+0002e740: 6365 5f69 6420 3d20 776f 726b 7370 6163  ce_id = workspac
+0002e750: 655f 6964 0a0a 2020 2020 6465 6620 7661  e_id..    def va
+0002e760: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
+0002e770: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
+0002e780: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
+0002e790: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
+0002e7a0: 2073 7570 6572 2829 2e74 6f5f 6d61 7028   super().to_map(
+0002e7b0: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
+0002e7c0: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
+0002e7d0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0002e7e0: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
+0002e7f0: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
+0002e800: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0002e810: 776f 726b 7370 6163 655f 6964 2069 7320  workspace_id is 
+0002e820: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0002e830: 2020 2020 2020 7265 7375 6c74 5b27 576f        result['Wo
+0002e840: 726b 7370 6163 6549 6427 5d20 3d20 7365  rkspaceId'] = se
+0002e850: 6c66 2e77 6f72 6b73 7061 6365 5f69 640a  lf.workspace_id.
+0002e860: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+0002e870: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
+0002e880: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3a  rom_map(self, m:
+0002e890: 2064 6963 7420 3d20 4e6f 6e65 293a 0a20   dict = None):. 
+0002e8a0: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
+0002e8b0: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+0002e8c0: 6620 6d2e 6765 7428 2757 6f72 6b73 7061  f m.get('Workspa
+0002e8d0: 6365 4964 2729 2069 7320 6e6f 7420 4e6f  ceId') is not No
+0002e8e0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0002e8f0: 7365 6c66 2e77 6f72 6b73 7061 6365 5f69  self.workspace_i
+0002e900: 6420 3d20 6d2e 6765 7428 2757 6f72 6b73  d = m.get('Works
+0002e910: 7061 6365 4964 2729 0a20 2020 2020 2020  paceId').       
+0002e920: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
+0002e930: 6c61 7373 2053 746f 7054 656e 736f 7262  lass StopTensorb
+0002e940: 6f61 7264 5265 7370 6f6e 7365 426f 6479  oardResponseBody
+0002e950: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
+0002e960: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
+0002e970: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+0002e980: 2020 2020 7265 7175 6573 745f 6964 3a20      request_id: 
+0002e990: 7374 7220 3d20 4e6f 6e65 2c0a 2020 2020  str = None,.    
+0002e9a0: 2020 2020 7465 6e73 6f72 626f 6172 645f      tensorboard_
+0002e9b0: 6964 3a20 7374 7220 3d20 4e6f 6e65 2c0a  id: str = None,.
+0002e9c0: 2020 2020 293a 0a20 2020 2020 2020 2073      ):.        s
+0002e9d0: 656c 662e 7265 7175 6573 745f 6964 203d  elf.request_id =
+0002e9e0: 2072 6571 7565 7374 5f69 640a 2020 2020   request_id.    
+0002e9f0: 2020 2020 7365 6c66 2e74 656e 736f 7262      self.tensorb
+0002ea00: 6f61 7264 5f69 6420 3d20 7465 6e73 6f72  oard_id = tensor
+0002ea10: 626f 6172 645f 6964 0a0a 2020 2020 6465  board_id..    de
+0002ea20: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
+0002ea30: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
+0002ea40: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
+0002ea50: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
+0002ea60: 6170 203d 2073 7570 6572 2829 2e74 6f5f  ap = super().to_
+0002ea70: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
+0002ea80: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
+0002ea90: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0002eaa0: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
+0002eab0: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
+0002eac0: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
+0002ead0: 656c 662e 7265 7175 6573 745f 6964 2069  elf.request_id i
+0002eae0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0002eaf0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+0002eb00: 5265 7175 6573 7449 6427 5d20 3d20 7365  RequestId'] = se
+0002eb10: 6c66 2e72 6571 7565 7374 5f69 640a 2020  lf.request_id.  
+0002eb20: 2020 2020 2020 6966 2073 656c 662e 7465        if self.te
+0002eb30: 6e73 6f72 626f 6172 645f 6964 2069 7320  nsorboard_id is 
+0002eb40: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0002eb50: 2020 2020 2020 7265 7375 6c74 5b27 5465        result['Te
+0002eb60: 6e73 6f72 626f 6172 6449 6427 5d20 3d20  nsorboardId'] = 
+0002eb70: 7365 6c66 2e74 656e 736f 7262 6f61 7264  self.tensorboard
+0002eb80: 5f69 640a 2020 2020 2020 2020 7265 7475  _id.        retu
+0002eb90: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
+0002eba0: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
+0002ebb0: 2c20 6d3a 2064 6963 7420 3d20 4e6f 6e65  , m: dict = None
+0002ebc0: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
+0002ebd0: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
+0002ebe0: 2020 2069 6620 6d2e 6765 7428 2752 6571     if m.get('Req
+0002ebf0: 7565 7374 4964 2729 2069 7320 6e6f 7420  uestId') is not 
+0002ec00: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0002ec10: 2020 7365 6c66 2e72 6571 7565 7374 5f69    self.request_i
+0002ec20: 6420 3d20 6d2e 6765 7428 2752 6571 7565  d = m.get('Reque
+0002ec30: 7374 4964 2729 0a20 2020 2020 2020 2069  stId').        i
+0002ec40: 6620 6d2e 6765 7428 2754 656e 736f 7262  f m.get('Tensorb
+0002ec50: 6f61 7264 4964 2729 2069 7320 6e6f 7420  oardId') is not 
+0002ec60: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0002ec70: 2020 7365 6c66 2e74 656e 736f 7262 6f61    self.tensorboa
+0002ec80: 7264 5f69 6420 3d20 6d2e 6765 7428 2754  rd_id = m.get('T
+0002ec90: 656e 736f 7262 6f61 7264 4964 2729 0a20  ensorboardId'). 
+0002eca0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0002ecb0: 6c66 0a0a 0a63 6c61 7373 2053 746f 7054  lf...class StopT
+0002ecc0: 656e 736f 7262 6f61 7264 5265 7370 6f6e  ensorboardRespon
+0002ecd0: 7365 2854 6561 4d6f 6465 6c29 3a0a 2020  se(TeaModel):.  
+0002ece0: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
+0002ecf0: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+0002ed00: 2020 2020 2020 6865 6164 6572 733a 2044        headers: D
+0002ed10: 6963 745b 7374 722c 2073 7472 5d20 3d20  ict[str, str] = 
+0002ed20: 4e6f 6e65 2c0a 2020 2020 2020 2020 7374  None,.        st
+0002ed30: 6174 7573 5f63 6f64 653a 2069 6e74 203d  atus_code: int =
+0002ed40: 204e 6f6e 652c 0a20 2020 2020 2020 2062   None,.        b
+0002ed50: 6f64 793a 2053 746f 7054 656e 736f 7262  ody: StopTensorb
+0002ed60: 6f61 7264 5265 7370 6f6e 7365 426f 6479  oardResponseBody
+0002ed70: 203d 204e 6f6e 652c 0a20 2020 2029 3a0a   = None,.    ):.
+0002ed80: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
+0002ed90: 6465 7273 203d 2068 6561 6465 7273 0a20  ders = headers. 
+0002eda0: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
+0002edb0: 7573 5f63 6f64 6520 3d20 7374 6174 7573  us_code = status
+0002edc0: 5f63 6f64 650a 2020 2020 2020 2020 7365  _code.        se
+0002edd0: 6c66 2e62 6f64 7920 3d20 626f 6479 0a0a  lf.body = body..
+0002ede0: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
+0002edf0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0002ee00: 7365 6c66 2e76 616c 6964 6174 655f 7265  self.validate_re
+0002ee10: 7175 6972 6564 2873 656c 662e 6865 6164  quired(self.head
+0002ee20: 6572 732c 2027 6865 6164 6572 7327 290a  ers, 'headers').
+0002ee30: 2020 2020 2020 2020 7365 6c66 2e76 616c          self.val
+0002ee40: 6964 6174 655f 7265 7175 6972 6564 2873  idate_required(s
+0002ee50: 656c 662e 7374 6174 7573 5f63 6f64 652c  elf.status_code,
+0002ee60: 2027 7374 6174 7573 5f63 6f64 6527 290a   'status_code').
+0002ee70: 2020 2020 2020 2020 7365 6c66 2e76 616c          self.val
+0002ee80: 6964 6174 655f 7265 7175 6972 6564 2873  idate_required(s
+0002ee90: 656c 662e 626f 6479 2c20 2762 6f64 7927  elf.body, 'body'
+0002eea0: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+0002eeb0: 662e 626f 6479 3a0a 2020 2020 2020 2020  f.body:.        
+0002eec0: 2020 2020 7365 6c66 2e62 6f64 792e 7661      self.body.va
+0002eed0: 6c69 6461 7465 2829 0a0a 2020 2020 6465  lidate()..    de
+0002eee0: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
+0002eef0: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
+0002ef00: 7570 6572 2829 2e74 6f5f 6d61 7028 290a  uper().to_map().
+0002ef10: 2020 2020 2020 2020 6966 205f 6d61 7020          if _map 
+0002ef20: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0002ef30: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0002ef40: 5f6d 6170 0a0a 2020 2020 2020 2020 7265  _map..        re
+0002ef50: 7375 6c74 203d 2064 6963 7428 290a 2020  sult = dict().  
+0002ef60: 2020 2020 2020 6966 2073 656c 662e 6865        if self.he
+0002ef70: 6164 6572 7320 6973 206e 6f74 204e 6f6e  aders is not Non
+0002ef80: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0002ef90: 6573 756c 745b 2768 6561 6465 7273 275d  esult['headers']
+0002efa0: 203d 2073 656c 662e 6865 6164 6572 730a   = self.headers.
+0002efb0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0002efc0: 7374 6174 7573 5f63 6f64 6520 6973 206e  status_code is n
+0002efd0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0002efe0: 2020 2020 2072 6573 756c 745b 2773 7461       result['sta
+0002eff0: 7475 7343 6f64 6527 5d20 3d20 7365 6c66  tusCode'] = self
+0002f000: 2e73 7461 7475 735f 636f 6465 0a20 2020  .status_code.   
+0002f010: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
+0002f020: 7920 6973 206e 6f74 204e 6f6e 653a 0a20  y is not None:. 
+0002f030: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+0002f040: 745b 2762 6f64 7927 5d20 3d20 7365 6c66  t['body'] = self
+0002f050: 2e62 6f64 792e 746f 5f6d 6170 2829 0a20  .body.to_map(). 
+0002f060: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+0002f070: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
+0002f080: 6f6d 5f6d 6170 2873 656c 662c 206d 3a20  om_map(self, m: 
+0002f090: 6469 6374 203d 204e 6f6e 6529 3a0a 2020  dict = None):.  
+0002f0a0: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
+0002f0b0: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+0002f0c0: 206d 2e67 6574 2827 6865 6164 6572 7327   m.get('headers'
+0002f0d0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+0002f0e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0002f0f0: 6865 6164 6572 7320 3d20 6d2e 6765 7428  headers = m.get(
+0002f100: 2768 6561 6465 7273 2729 0a20 2020 2020  'headers').     
+0002f110: 2020 2069 6620 6d2e 6765 7428 2773 7461     if m.get('sta
+0002f120: 7475 7343 6f64 6527 2920 6973 206e 6f74  tusCode') is not
+0002f130: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0002f140: 2020 2073 656c 662e 7374 6174 7573 5f63     self.status_c
+0002f150: 6f64 6520 3d20 6d2e 6765 7428 2773 7461  ode = m.get('sta
+0002f160: 7475 7343 6f64 6527 290a 2020 2020 2020  tusCode').      
+0002f170: 2020 6966 206d 2e67 6574 2827 626f 6479    if m.get('body
+0002f180: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+0002f190: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
+0002f1a0: 5f6d 6f64 656c 203d 2053 746f 7054 656e  _model = StopTen
+0002f1b0: 736f 7262 6f61 7264 5265 7370 6f6e 7365  sorboardResponse
+0002f1c0: 426f 6479 2829 0a20 2020 2020 2020 2020  Body().         
+0002f1d0: 2020 2073 656c 662e 626f 6479 203d 2074     self.body = t
+0002f1e0: 656d 705f 6d6f 6465 6c2e 6672 6f6d 5f6d  emp_model.from_m
+0002f1f0: 6170 286d 5b27 626f 6479 275d 290a 2020  ap(m['body']).  
+0002f200: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0002f210: 660a 0a0a 636c 6173 7320 5570 6461 7465  f...class Update
+0002f220: 4a6f 6252 6571 7565 7374 2854 6561 4d6f  JobRequest(TeaMo
+0002f230: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
+0002f240: 696e 6974 5f5f 280a 2020 2020 2020 2020  init__(.        
+0002f250: 7365 6c66 2c0a 2020 2020 2020 2020 7072  self,.        pr
+0002f260: 696f 7269 7479 3a20 696e 7420 3d20 4e6f  iority: int = No
+0002f270: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
+0002f280: 2020 2073 656c 662e 7072 696f 7269 7479     self.priority
+0002f290: 203d 2070 7269 6f72 6974 790a 0a20 2020   = priority..   
+0002f2a0: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
+0002f2b0: 6c66 293a 0a20 2020 2020 2020 2070 6173  lf):.        pas
+0002f2c0: 730a 0a20 2020 2064 6566 2074 6f5f 6d61  s..    def to_ma
+0002f2d0: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
+0002f2e0: 205f 6d61 7020 3d20 7375 7065 7228 292e   _map = super().
+0002f2f0: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
+0002f300: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
+0002f310: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0002f320: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
+0002f330: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+0002f340: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+0002f350: 6620 7365 6c66 2e70 7269 6f72 6974 7920  f self.priority 
+0002f360: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0002f370: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+0002f380: 2750 7269 6f72 6974 7927 5d20 3d20 7365  'Priority'] = se
+0002f390: 6c66 2e70 7269 6f72 6974 790a 2020 2020  lf.priority.    
+0002f3a0: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
+0002f3b0: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
+0002f3c0: 6d61 7028 7365 6c66 2c20 6d3a 2064 6963  map(self, m: dic
+0002f3d0: 7420 3d20 4e6f 6e65 293a 0a20 2020 2020  t = None):.     
+0002f3e0: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
+0002f3f0: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
+0002f400: 6765 7428 2750 7269 6f72 6974 7927 2920  get('Priority') 
+0002f410: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0002f420: 2020 2020 2020 2020 2073 656c 662e 7072           self.pr
+0002f430: 696f 7269 7479 203d 206d 2e67 6574 2827  iority = m.get('
+0002f440: 5072 696f 7269 7479 2729 0a20 2020 2020  Priority').     
+0002f450: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
+0002f460: 0a63 6c61 7373 2055 7064 6174 654a 6f62  .class UpdateJob
+0002f470: 5265 7370 6f6e 7365 426f 6479 2854 6561  ResponseBody(Tea
+0002f480: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
+0002f490: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
+0002f4a0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+0002f4b0: 6a6f 625f 6964 3a20 7374 7220 3d20 4e6f  job_id: str = No
+0002f4c0: 6e65 2c0a 2020 2020 2020 2020 7265 7175  ne,.        requ
+0002f4d0: 6573 745f 6964 3a20 7374 7220 3d20 4e6f  est_id: str = No
+0002f4e0: 6e65 2c0a 2020 2020 293a 0a20 2020 2020  ne,.    ):.     
+0002f4f0: 2020 2073 656c 662e 6a6f 625f 6964 203d     self.job_id =
+0002f500: 206a 6f62 5f69 640a 2020 2020 2020 2020   job_id.        
+0002f510: 7365 6c66 2e72 6571 7565 7374 5f69 6420  self.request_id 
+0002f520: 3d20 7265 7175 6573 745f 6964 0a0a 2020  = request_id..  
+0002f530: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
+0002f540: 656c 6629 3a0a 2020 2020 2020 2020 7061  elf):.        pa
+0002f550: 7373 0a0a 2020 2020 6465 6620 746f 5f6d  ss..    def to_m
+0002f560: 6170 2873 656c 6629 3a0a 2020 2020 2020  ap(self):.      
+0002f570: 2020 5f6d 6170 203d 2073 7570 6572 2829    _map = super()
+0002f580: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
+0002f590: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
+0002f5a0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0002f5b0: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
+0002f5c0: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+0002f5d0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+0002f5e0: 6966 2073 656c 662e 6a6f 625f 6964 2069  if self.job_id i
+0002f5f0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0002f600: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+0002f610: 4a6f 6249 6427 5d20 3d20 7365 6c66 2e6a  JobId'] = self.j
+0002f620: 6f62 5f69 640a 2020 2020 2020 2020 6966  ob_id.        if
+0002f630: 2073 656c 662e 7265 7175 6573 745f 6964   self.request_id
+0002f640: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0002f650: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+0002f660: 5b27 5265 7175 6573 7449 6427 5d20 3d20  ['RequestId'] = 
+0002f670: 7365 6c66 2e72 6571 7565 7374 5f69 640a  self.request_id.
+0002f680: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+0002f690: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
+0002f6a0: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3a  rom_map(self, m:
+0002f6b0: 2064 6963 7420 3d20 4e6f 6e65 293a 0a20   dict = None):. 
+0002f6c0: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
+0002f6d0: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+0002f6e0: 6620 6d2e 6765 7428 274a 6f62 4964 2729  f m.get('JobId')
+0002f6f0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0002f700: 2020 2020 2020 2020 2020 7365 6c66 2e6a            self.j
+0002f710: 6f62 5f69 6420 3d20 6d2e 6765 7428 274a  ob_id = m.get('J
+0002f720: 6f62 4964 2729 0a20 2020 2020 2020 2069  obId').        i
+0002f730: 6620 6d2e 6765 7428 2752 6571 7565 7374  f m.get('Request
+0002f740: 4964 2729 2069 7320 6e6f 7420 4e6f 6e65  Id') is not None
+0002f750: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0002f760: 6c66 2e72 6571 7565 7374 5f69 6420 3d20  lf.request_id = 
+0002f770: 6d2e 6765 7428 2752 6571 7565 7374 4964  m.get('RequestId
+0002f780: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
+0002f790: 6e20 7365 6c66 0a0a 0a63 6c61 7373 2055  n self...class U
+0002f7a0: 7064 6174 654a 6f62 5265 7370 6f6e 7365  pdateJobResponse
+0002f7b0: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
+0002f7c0: 6465 6620 5f5f 696e 6974 5f5f 280a 2020  def __init__(.  
+0002f7d0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+0002f7e0: 2020 2020 6865 6164 6572 733a 2044 6963      headers: Dic
+0002f7f0: 745b 7374 722c 2073 7472 5d20 3d20 4e6f  t[str, str] = No
+0002f800: 6e65 2c0a 2020 2020 2020 2020 7374 6174  ne,.        stat
+0002f810: 7573 5f63 6f64 653a 2069 6e74 203d 204e  us_code: int = N
+0002f820: 6f6e 652c 0a20 2020 2020 2020 2062 6f64  one,.        bod
+0002f830: 793a 2055 7064 6174 654a 6f62 5265 7370  y: UpdateJobResp
+0002f840: 6f6e 7365 426f 6479 203d 204e 6f6e 652c  onseBody = None,
+0002f850: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
+0002f860: 7365 6c66 2e68 6561 6465 7273 203d 2068  self.headers = h
+0002f870: 6561 6465 7273 0a20 2020 2020 2020 2073  eaders.        s
+0002f880: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
+0002f890: 3d20 7374 6174 7573 5f63 6f64 650a 2020  = status_code.  
+0002f8a0: 2020 2020 2020 7365 6c66 2e62 6f64 7920        self.body 
+0002f8b0: 3d20 626f 6479 0a0a 2020 2020 6465 6620  = body..    def 
+0002f8c0: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
+0002f8d0: 2020 2020 2020 2020 7365 6c66 2e76 616c          self.val
+0002f8e0: 6964 6174 655f 7265 7175 6972 6564 2873  idate_required(s
+0002f8f0: 656c 662e 6865 6164 6572 732c 2027 6865  elf.headers, 'he
+0002f900: 6164 6572 7327 290a 2020 2020 2020 2020  aders').        
+0002f910: 7365 6c66 2e76 616c 6964 6174 655f 7265  self.validate_re
+0002f920: 7175 6972 6564 2873 656c 662e 7374 6174  quired(self.stat
+0002f930: 7573 5f63 6f64 652c 2027 7374 6174 7573  us_code, 'status
+0002f940: 5f63 6f64 6527 290a 2020 2020 2020 2020  _code').        
+0002f950: 7365 6c66 2e76 616c 6964 6174 655f 7265  self.validate_re
+0002f960: 7175 6972 6564 2873 656c 662e 626f 6479  quired(self.body
+0002f970: 2c20 2762 6f64 7927 290a 2020 2020 2020  , 'body').      
+0002f980: 2020 6966 2073 656c 662e 626f 6479 3a0a    if self.body:.
+0002f990: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0002f9a0: 2e62 6f64 792e 7661 6c69 6461 7465 2829  .body.validate()
+0002f9b0: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
+0002f9c0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0002f9d0: 5f6d 6170 203d 2073 7570 6572 2829 2e74  _map = super().t
+0002f9e0: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
+0002f9f0: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
+0002fa00: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0002fa10: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
+0002fa20: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
+0002fa30: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+0002fa40: 2073 656c 662e 6865 6164 6572 7320 6973   self.headers is
+0002fa50: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0002fa60: 2020 2020 2020 2072 6573 756c 745b 2768         result['h
+0002fa70: 6561 6465 7273 275d 203d 2073 656c 662e  eaders'] = self.
+0002fa80: 6865 6164 6572 730a 2020 2020 2020 2020  headers.        
+0002fa90: 6966 2073 656c 662e 7374 6174 7573 5f63  if self.status_c
+0002faa0: 6f64 6520 6973 206e 6f74 204e 6f6e 653a  ode is not None:
+0002fab0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+0002fac0: 756c 745b 2773 7461 7475 7343 6f64 6527  ult['statusCode'
+0002fad0: 5d20 3d20 7365 6c66 2e73 7461 7475 735f  ] = self.status_
+0002fae0: 636f 6465 0a20 2020 2020 2020 2069 6620  code.        if 
+0002faf0: 7365 6c66 2e62 6f64 7920 6973 206e 6f74  self.body is not
+0002fb00: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0002fb10: 2020 2072 6573 756c 745b 2762 6f64 7927     result['body'
+0002fb20: 5d20 3d20 7365 6c66 2e62 6f64 792e 746f  ] = self.body.to
+0002fb30: 5f6d 6170 2829 0a20 2020 2020 2020 2072  _map().        r
+0002fb40: 6574 7572 6e20 7265 7375 6c74 0a0a 2020  eturn result..  
+0002fb50: 2020 6465 6620 6672 6f6d 5f6d 6170 2873    def from_map(s
+0002fb60: 656c 662c 206d 3a20 6469 6374 203d 204e  elf, m: dict = N
+0002fb70: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
+0002fb80: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
+0002fb90: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+0002fba0: 6865 6164 6572 7327 2920 6973 206e 6f74  headers') is not
+0002fbb0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0002fbc0: 2020 2073 656c 662e 6865 6164 6572 7320     self.headers 
+0002fbd0: 3d20 6d2e 6765 7428 2768 6561 6465 7273  = m.get('headers
+0002fbe0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+0002fbf0: 6765 7428 2773 7461 7475 7343 6f64 6527  get('statusCode'
+0002fc00: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+0002fc10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0002fc20: 7374 6174 7573 5f63 6f64 6520 3d20 6d2e  status_code = m.
+0002fc30: 6765 7428 2773 7461 7475 7343 6f64 6527  get('statusCode'
+0002fc40: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+0002fc50: 6574 2827 626f 6479 2729 2069 7320 6e6f  et('body') is no
+0002fc60: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0002fc70: 2020 2020 7465 6d70 5f6d 6f64 656c 203d      temp_model =
+0002fc80: 2055 7064 6174 654a 6f62 5265 7370 6f6e   UpdateJobRespon
+0002fc90: 7365 426f 6479 2829 0a20 2020 2020 2020  seBody().       
+0002fca0: 2020 2020 2073 656c 662e 626f 6479 203d       self.body =
+0002fcb0: 2074 656d 705f 6d6f 6465 6c2e 6672 6f6d   temp_model.from
+0002fcc0: 5f6d 6170 286d 5b27 626f 6479 275d 290a  _map(m['body']).
+0002fcd0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0002fce0: 656c 660a 0a0a 636c 6173 7320 5570 6461  elf...class Upda
+0002fcf0: 7465 5465 6e73 6f72 626f 6172 6452 6571  teTensorboardReq
+0002fd00: 7565 7374 2854 6561 4d6f 6465 6c29 3a0a  uest(TeaModel):.
+0002fd10: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+0002fd20: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+0002fd30: 2020 2020 2020 2020 6d61 785f 7275 6e6e          max_runn
+0002fd40: 696e 675f 7469 6d65 5f6d 696e 7574 6573  ing_time_minutes
+0002fd50: 3a20 696e 7420 3d20 4e6f 6e65 2c0a 2020  : int = None,.  
+0002fd60: 2020 2020 2020 776f 726b 7370 6163 655f        workspace_
+0002fd70: 6964 3a20 7374 7220 3d20 4e6f 6e65 2c0a  id: str = None,.
+0002fd80: 2020 2020 293a 0a20 2020 2020 2020 2073      ):.        s
+0002fd90: 656c 662e 6d61 785f 7275 6e6e 696e 675f  elf.max_running_
+0002fda0: 7469 6d65 5f6d 696e 7574 6573 203d 206d  time_minutes = m
+0002fdb0: 6178 5f72 756e 6e69 6e67 5f74 696d 655f  ax_running_time_
+0002fdc0: 6d69 6e75 7465 730a 2020 2020 2020 2020  minutes.        
+0002fdd0: 7365 6c66 2e77 6f72 6b73 7061 6365 5f69  self.workspace_i
+0002fde0: 6420 3d20 776f 726b 7370 6163 655f 6964  d = workspace_id
+0002fdf0: 0a0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
+0002fe00: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
+0002fe10: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
+0002fe20: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
+0002fe30: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
+0002fe40: 6572 2829 2e74 6f5f 6d61 7028 290a 2020  er().to_map().  
+0002fe50: 2020 2020 2020 6966 205f 6d61 7020 6973        if _map is
+0002fe60: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0002fe70: 2020 2020 2020 2072 6574 7572 6e20 5f6d         return _m
+0002fe80: 6170 0a0a 2020 2020 2020 2020 7265 7375  ap..        resu
+0002fe90: 6c74 203d 2064 6963 7428 290a 2020 2020  lt = dict().    
+0002fea0: 2020 2020 6966 2073 656c 662e 6d61 785f      if self.max_
+0002feb0: 7275 6e6e 696e 675f 7469 6d65 5f6d 696e  running_time_min
+0002fec0: 7574 6573 2069 7320 6e6f 7420 4e6f 6e65  utes is not None
+0002fed0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0002fee0: 7375 6c74 5b27 4d61 7852 756e 6e69 6e67  sult['MaxRunning
+0002fef0: 5469 6d65 4d69 6e75 7465 7327 5d20 3d20  TimeMinutes'] = 
+0002ff00: 7365 6c66 2e6d 6178 5f72 756e 6e69 6e67  self.max_running
+0002ff10: 5f74 696d 655f 6d69 6e75 7465 730a 2020  _time_minutes.  
+0002ff20: 2020 2020 2020 6966 2073 656c 662e 776f        if self.wo
+0002ff30: 726b 7370 6163 655f 6964 2069 7320 6e6f  rkspace_id is no
+0002ff40: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0002ff50: 2020 2020 7265 7375 6c74 5b27 576f 726b      result['Work
+0002ff60: 7370 6163 6549 6427 5d20 3d20 7365 6c66  spaceId'] = self
+0002ff70: 2e77 6f72 6b73 7061 6365 5f69 640a 2020  .workspace_id.  
+0002ff80: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+0002ff90: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
+0002ffa0: 6d5f 6d61 7028 7365 6c66 2c20 6d3a 2064  m_map(self, m: d
+0002ffb0: 6963 7420 3d20 4e6f 6e65 293a 0a20 2020  ict = None):.   
+0002ffc0: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
+0002ffd0: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+0002ffe0: 6d2e 6765 7428 274d 6178 5275 6e6e 696e  m.get('MaxRunnin
+0002fff0: 6754 696d 654d 696e 7574 6573 2729 2069  gTimeMinutes') i
+00030000: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00030010: 2020 2020 2020 2020 7365 6c66 2e6d 6178          self.max
+00030020: 5f72 756e 6e69 6e67 5f74 696d 655f 6d69  _running_time_mi
+00030030: 6e75 7465 7320 3d20 6d2e 6765 7428 274d  nutes = m.get('M
+00030040: 6178 5275 6e6e 696e 6754 696d 654d 696e  axRunningTimeMin
+00030050: 7574 6573 2729 0a20 2020 2020 2020 2069  utes').        i
+00030060: 6620 6d2e 6765 7428 2757 6f72 6b73 7061  f m.get('Workspa
+00030070: 6365 4964 2729 2069 7320 6e6f 7420 4e6f  ceId') is not No
+00030080: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00030090: 7365 6c66 2e77 6f72 6b73 7061 6365 5f69  self.workspace_i
+000300a0: 6420 3d20 6d2e 6765 7428 2757 6f72 6b73  d = m.get('Works
+000300b0: 7061 6365 4964 2729 0a20 2020 2020 2020  paceId').       
+000300c0: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
+000300d0: 6c61 7373 2055 7064 6174 6554 656e 736f  lass UpdateTenso
+000300e0: 7262 6f61 7264 5265 7370 6f6e 7365 426f  rboardResponseBo
+000300f0: 6479 2854 6561 4d6f 6465 6c29 3a0a 2020  dy(TeaModel):.  
+00030100: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
+00030110: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+00030120: 2020 2020 2020 7265 7175 6573 745f 6964        request_id
+00030130: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+00030140: 2020 2020 2020 7465 6e73 6f72 626f 6172        tensorboar
+00030150: 645f 6964 3a20 7374 7220 3d20 4e6f 6e65  d_id: str = None
+00030160: 2c0a 2020 2020 293a 0a20 2020 2020 2020  ,.    ):.       
+00030170: 2073 656c 662e 7265 7175 6573 745f 6964   self.request_id
+00030180: 203d 2072 6571 7565 7374 5f69 640a 2020   = request_id.  
+00030190: 2020 2020 2020 7365 6c66 2e74 656e 736f        self.tenso
+000301a0: 7262 6f61 7264 5f69 6420 3d20 7465 6e73  rboard_id = tens
+000301b0: 6f72 626f 6172 645f 6964 0a0a 2020 2020  orboard_id..    
+000301c0: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
+000301d0: 6629 3a0a 2020 2020 2020 2020 7061 7373  f):.        pass
+000301e0: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
+000301f0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00030200: 5f6d 6170 203d 2073 7570 6572 2829 2e74  _map = super().t
+00030210: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
+00030220: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
+00030230: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00030240: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
+00030250: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
+00030260: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+00030270: 2073 656c 662e 7265 7175 6573 745f 6964   self.request_id
+00030280: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00030290: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+000302a0: 5b27 5265 7175 6573 7449 6427 5d20 3d20  ['RequestId'] = 
+000302b0: 7365 6c66 2e72 6571 7565 7374 5f69 640a  self.request_id.
+000302c0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000302d0: 7465 6e73 6f72 626f 6172 645f 6964 2069  tensorboard_id i
+000302e0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000302f0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+00030300: 5465 6e73 6f72 626f 6172 6449 6427 5d20  TensorboardId'] 
+00030310: 3d20 7365 6c66 2e74 656e 736f 7262 6f61  = self.tensorboa
+00030320: 7264 5f69 640a 2020 2020 2020 2020 7265  rd_id.        re
+00030330: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
+00030340: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
+00030350: 6c66 2c20 6d3a 2064 6963 7420 3d20 4e6f  lf, m: dict = No
+00030360: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
+00030370: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
+00030380: 2020 2020 2069 6620 6d2e 6765 7428 2752       if m.get('R
+00030390: 6571 7565 7374 4964 2729 2069 7320 6e6f  equestId') is no
+000303a0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000303b0: 2020 2020 7365 6c66 2e72 6571 7565 7374      self.request
+000303c0: 5f69 6420 3d20 6d2e 6765 7428 2752 6571  _id = m.get('Req
+000303d0: 7565 7374 4964 2729 0a20 2020 2020 2020  uestId').       
+000303e0: 2069 6620 6d2e 6765 7428 2754 656e 736f   if m.get('Tenso
+000303f0: 7262 6f61 7264 4964 2729 2069 7320 6e6f  rboardId') is no
+00030400: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00030410: 2020 2020 7365 6c66 2e74 656e 736f 7262      self.tensorb
+00030420: 6f61 7264 5f69 6420 3d20 6d2e 6765 7428  oard_id = m.get(
+00030430: 2754 656e 736f 7262 6f61 7264 4964 2729  'TensorboardId')
+00030440: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00030450: 7365 6c66 0a0a 0a63 6c61 7373 2055 7064  self...class Upd
+00030460: 6174 6554 656e 736f 7262 6f61 7264 5265  ateTensorboardRe
+00030470: 7370 6f6e 7365 2854 6561 4d6f 6465 6c29  sponse(TeaModel)
+00030480: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
+00030490: 5f5f 280a 2020 2020 2020 2020 7365 6c66  __(.        self
+000304a0: 2c0a 2020 2020 2020 2020 6865 6164 6572  ,.        header
+000304b0: 733a 2044 6963 745b 7374 722c 2073 7472  s: Dict[str, str
+000304c0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+000304d0: 2020 7374 6174 7573 5f63 6f64 653a 2069    status_code: i
+000304e0: 6e74 203d 204e 6f6e 652c 0a20 2020 2020  nt = None,.     
+000304f0: 2020 2062 6f64 793a 2055 7064 6174 6554     body: UpdateT
+00030500: 656e 736f 7262 6f61 7264 5265 7370 6f6e  ensorboardRespon
+00030510: 7365 426f 6479 203d 204e 6f6e 652c 0a20  seBody = None,. 
+00030520: 2020 2029 3a0a 2020 2020 2020 2020 7365     ):.        se
+00030530: 6c66 2e68 6561 6465 7273 203d 2068 6561  lf.headers = hea
+00030540: 6465 7273 0a20 2020 2020 2020 2073 656c  ders.        sel
+00030550: 662e 7374 6174 7573 5f63 6f64 6520 3d20  f.status_code = 
+00030560: 7374 6174 7573 5f63 6f64 650a 2020 2020  status_code.    
+00030570: 2020 2020 7365 6c66 2e62 6f64 7920 3d20      self.body = 
+00030580: 626f 6479 0a0a 2020 2020 6465 6620 7661  body..    def va
+00030590: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
+000305a0: 2020 2020 2020 7365 6c66 2e76 616c 6964        self.valid
+000305b0: 6174 655f 7265 7175 6972 6564 2873 656c  ate_required(sel
+000305c0: 662e 6865 6164 6572 732c 2027 6865 6164  f.headers, 'head
+000305d0: 6572 7327 290a 2020 2020 2020 2020 7365  ers').        se
+000305e0: 6c66 2e76 616c 6964 6174 655f 7265 7175  lf.validate_requ
+000305f0: 6972 6564 2873 656c 662e 7374 6174 7573  ired(self.status
+00030600: 5f63 6f64 652c 2027 7374 6174 7573 5f63  _code, 'status_c
+00030610: 6f64 6527 290a 2020 2020 2020 2020 7365  ode').        se
+00030620: 6c66 2e76 616c 6964 6174 655f 7265 7175  lf.validate_requ
+00030630: 6972 6564 2873 656c 662e 626f 6479 2c20  ired(self.body, 
+00030640: 2762 6f64 7927 290a 2020 2020 2020 2020  'body').        
+00030650: 6966 2073 656c 662e 626f 6479 3a0a 2020  if self.body:.  
+00030660: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
+00030670: 6f64 792e 7661 6c69 6461 7465 2829 0a0a  ody.validate()..
+00030680: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
+00030690: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
+000306a0: 6170 203d 2073 7570 6572 2829 2e74 6f5f  ap = super().to_
+000306b0: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
+000306c0: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
+000306d0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+000306e0: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
+000306f0: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
+00030700: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
+00030710: 656c 662e 6865 6164 6572 7320 6973 206e  elf.headers is n
+00030720: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00030730: 2020 2020 2072 6573 756c 745b 2768 6561       result['hea
+00030740: 6465 7273 275d 203d 2073 656c 662e 6865  ders'] = self.he
+00030750: 6164 6572 730a 2020 2020 2020 2020 6966  aders.        if
+00030760: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
+00030770: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
+00030780: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00030790: 745b 2773 7461 7475 7343 6f64 6527 5d20  t['statusCode'] 
+000307a0: 3d20 7365 6c66 2e73 7461 7475 735f 636f  = self.status_co
+000307b0: 6465 0a20 2020 2020 2020 2069 6620 7365  de.        if se
+000307c0: 6c66 2e62 6f64 7920 6973 206e 6f74 204e  lf.body is not N
+000307d0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000307e0: 2072 6573 756c 745b 2762 6f64 7927 5d20   result['body'] 
+000307f0: 3d20 7365 6c66 2e62 6f64 792e 746f 5f6d  = self.body.to_m
+00030800: 6170 2829 0a20 2020 2020 2020 2072 6574  ap().        ret
+00030810: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
+00030820: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
+00030830: 662c 206d 3a20 6469 6374 203d 204e 6f6e  f, m: dict = Non
+00030840: 6529 3a0a 2020 2020 2020 2020 6d20 3d20  e):.        m = 
+00030850: 6d20 6f72 2064 6963 7428 290a 2020 2020  m or dict().    
+00030860: 2020 2020 6966 206d 2e67 6574 2827 6865      if m.get('he
+00030870: 6164 6572 7327 2920 6973 206e 6f74 204e  aders') is not N
+00030880: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00030890: 2073 656c 662e 6865 6164 6572 7320 3d20   self.headers = 
+000308a0: 6d2e 6765 7428 2768 6561 6465 7273 2729  m.get('headers')
+000308b0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+000308c0: 7428 2773 7461 7475 7343 6f64 6527 2920  t('statusCode') 
+000308d0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000308e0: 2020 2020 2020 2020 2073 656c 662e 7374           self.st
+000308f0: 6174 7573 5f63 6f64 6520 3d20 6d2e 6765  atus_code = m.ge
+00030900: 7428 2773 7461 7475 7343 6f64 6527 290a  t('statusCode').
+00030910: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+00030920: 2827 626f 6479 2729 2069 7320 6e6f 7420  ('body') is not 
+00030930: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00030940: 2020 7465 6d70 5f6d 6f64 656c 203d 2055    temp_model = U
+00030950: 7064 6174 6554 656e 736f 7262 6f61 7264  pdateTensorboard
+00030960: 5265 7370 6f6e 7365 426f 6479 2829 0a20  ResponseBody(). 
+00030970: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00030980: 626f 6479 203d 2074 656d 705f 6d6f 6465  body = temp_mode
+00030990: 6c2e 6672 6f6d 5f6d 6170 286d 5b27 626f  l.from_map(m['bo
+000309a0: 6479 275d 290a 2020 2020 2020 2020 7265  dy']).        re
+000309b0: 7475 726e 2073 656c 660a 0a0a            turn self...
```

### Comparing `alibabacloud_pai-dlc20201203-1.2.6/alibabacloud_pai_dlc20201203.egg-info/PKG-INFO` & `alibabacloud_pai-dlc20201203-1.2.7/alibabacloud_pai_dlc20201203.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-pai-dlc20201203
-Version: 1.2.6
+Version: 1.2.7
 Summary: Alibaba Cloud pai-dlc (20201203) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_pai-dlc20201203-1.2.6/setup.py` & `alibabacloud_pai-dlc20201203-1.2.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,28 +20,28 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_pai-dlc20201203.
 
-Created on 26/05/2023
+Created on 19/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_pai_dlc20201203"
 NAME = "alibabacloud_pai-dlc20201203" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud pai-dlc (20201203) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.8, <1.0.0",
+    "alibabacloud_tea_util>=0.3.10, <1.0.0",
     "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
     "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
```

