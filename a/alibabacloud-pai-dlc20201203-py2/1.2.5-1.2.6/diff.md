# Comparing `tmp/alibabacloud_pai-dlc20201203_py2-1.2.5.tar.gz` & `tmp/alibabacloud_pai-dlc20201203_py2-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_pai-dlc20201203_py2-1.2.5.tar", last modified: Fri May 26 02:14:13 2023, max compression
+gzip compressed data, was "dist/alibabacloud_pai-dlc20201203_py2-1.2.6.tar", last modified: Wed Jul 19 04:52:20 2023, max compression
```

## Comparing `alibabacloud_pai-dlc20201203_py2-1.2.5.tar` & `alibabacloud_pai-dlc20201203_py2-1.2.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:14:13.000000 alibabacloud_pai-dlc20201203_py2-1.2.5/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-26 02:14:12.000000 alibabacloud_pai-dlc20201203_py2-1.2.5/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-05-26 02:14:12.000000 alibabacloud_pai-dlc20201203_py2-1.2.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-05-26 02:14:12.000000 alibabacloud_pai-dlc20201203_py2-1.2.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2496 2023-05-26 02:14:13.000000 alibabacloud_pai-dlc20201203_py2-1.2.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1045 2023-05-26 02:14:12.000000 alibabacloud_pai-dlc20201203_py2-1.2.5/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1128 2023-05-26 02:14:12.000000 alibabacloud_pai-dlc20201203_py2-1.2.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:14:13.000000 alibabacloud_pai-dlc20201203_py2-1.2.5/alibabacloud_pai_dlc20201203/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-26 02:14:12.000000 alibabacloud_pai-dlc20201203_py2-1.2.5/alibabacloud_pai_dlc20201203/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33393 2023-05-26 02:14:12.000000 alibabacloud_pai-dlc20201203_py2-1.2.5/alibabacloud_pai_dlc20201203/client.py
--rw-r--r--   0 root         (0) root         (0)   196179 2023-05-26 02:14:12.000000 alibabacloud_pai-dlc20201203_py2-1.2.5/alibabacloud_pai_dlc20201203/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 02:14:13.000000 alibabacloud_pai-dlc20201203_py2-1.2.5/alibabacloud_pai_dlc20201203_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2496 2023-05-26 02:14:13.000000 alibabacloud_pai-dlc20201203_py2-1.2.5/alibabacloud_pai_dlc20201203_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      472 2023-05-26 02:14:13.000000 alibabacloud_pai-dlc20201203_py2-1.2.5/alibabacloud_pai_dlc20201203_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 02:14:13.000000 alibabacloud_pai-dlc20201203_py2-1.2.5/alibabacloud_pai_dlc20201203_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-05-26 02:14:13.000000 alibabacloud_pai-dlc20201203_py2-1.2.5/alibabacloud_pai_dlc20201203_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-26 02:14:13.000000 alibabacloud_pai-dlc20201203_py2-1.2.5/alibabacloud_pai_dlc20201203_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-26 02:14:13.000000 alibabacloud_pai-dlc20201203_py2-1.2.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2925 2023-05-26 02:14:12.000000 alibabacloud_pai-dlc20201203_py2-1.2.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 04:52:20.000000 alibabacloud_pai-dlc20201203_py2-1.2.6/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-19 04:52:19.000000 alibabacloud_pai-dlc20201203_py2-1.2.6/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-07-19 04:52:19.000000 alibabacloud_pai-dlc20201203_py2-1.2.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-07-19 04:52:19.000000 alibabacloud_pai-dlc20201203_py2-1.2.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2496 2023-07-19 04:52:20.000000 alibabacloud_pai-dlc20201203_py2-1.2.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1045 2023-07-19 04:52:19.000000 alibabacloud_pai-dlc20201203_py2-1.2.6/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1128 2023-07-19 04:52:19.000000 alibabacloud_pai-dlc20201203_py2-1.2.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 04:52:20.000000 alibabacloud_pai-dlc20201203_py2-1.2.6/alibabacloud_pai_dlc20201203/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-19 04:52:19.000000 alibabacloud_pai-dlc20201203_py2-1.2.6/alibabacloud_pai_dlc20201203/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    34644 2023-07-19 04:52:19.000000 alibabacloud_pai-dlc20201203_py2-1.2.6/alibabacloud_pai_dlc20201203/client.py
+-rw-r--r--   0 root         (0) root         (0)   198965 2023-07-19 04:52:19.000000 alibabacloud_pai-dlc20201203_py2-1.2.6/alibabacloud_pai_dlc20201203/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 04:52:20.000000 alibabacloud_pai-dlc20201203_py2-1.2.6/alibabacloud_pai_dlc20201203_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2496 2023-07-19 04:52:20.000000 alibabacloud_pai-dlc20201203_py2-1.2.6/alibabacloud_pai_dlc20201203_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      472 2023-07-19 04:52:20.000000 alibabacloud_pai-dlc20201203_py2-1.2.6/alibabacloud_pai_dlc20201203_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 04:52:20.000000 alibabacloud_pai-dlc20201203_py2-1.2.6/alibabacloud_pai_dlc20201203_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-07-19 04:52:20.000000 alibabacloud_pai-dlc20201203_py2-1.2.6/alibabacloud_pai_dlc20201203_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-19 04:52:20.000000 alibabacloud_pai-dlc20201203_py2-1.2.6/alibabacloud_pai_dlc20201203_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-19 04:52:20.000000 alibabacloud_pai-dlc20201203_py2-1.2.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2925 2023-07-19 04:52:19.000000 alibabacloud_pai-dlc20201203_py2-1.2.6/setup.py
```

### Comparing `alibabacloud_pai-dlc20201203_py2-1.2.5/ChangeLog.md` & `alibabacloud_pai-dlc20201203_py2-1.2.6/ChangeLog.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-05-26 Version: 1.2.5
+- Add parameter in JobElasticSpec.
+
 2023-03-23 Version: 1.2.4
 - Change the type of RequestId to string in GetJobEvents API.
 
 2022-12-13 Version: 1.2.3
 - CreateJob supports params SuccessPolicy.
 
 2022-07-26 Version: 1.2.1
```

### Comparing `alibabacloud_pai-dlc20201203_py2-1.2.5/LICENSE` & `alibabacloud_pai-dlc20201203_py2-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_pai-dlc20201203_py2-1.2.5/PKG-INFO` & `alibabacloud_pai-dlc20201203_py2-1.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_pai-dlc20201203_py2
-Version: 1.2.5
+Version: 1.2.6
 Summary: Alibaba Cloud pai-dlc (20201203) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_pai-dlc20201203_py2-1.2.5/README-CN.md` & `alibabacloud_pai-dlc20201203_py2-1.2.6/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_pai-dlc20201203_py2-1.2.5/README.md` & `alibabacloud_pai-dlc20201203_py2-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_pai-dlc20201203_py2-1.2.5/alibabacloud_pai_dlc20201203/client.py` & `alibabacloud_pai-dlc20201203_py2-1.2.6/alibabacloud_pai_dlc20201203/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -466,14 +466,44 @@
         )
 
     def get_tensorboard(self, tensorboard_id, request):
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.get_tensorboard_with_options(tensorboard_id, request, headers, runtime)
 
+    def get_web_terminal_with_options(self, job_id, pod_id, request, headers, runtime):
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
+            pathname='/api/v1/jobs/%s/pods/%s/webterminal' % (TeaConverter.to_unicode(OpenApiUtilClient.get_encode_param(job_id)), TeaConverter.to_unicode(OpenApiUtilClient.get_encode_param(pod_id))),
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
+    def get_web_terminal(self, job_id, pod_id, request):
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.get_web_terminal_with_options(job_id, pod_id, request, headers, runtime)
+
     def list_ecs_specs_with_options(self, request, headers, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.accelerator_type):
             query['AcceleratorType'] = request.accelerator_type
         if not UtilClient.is_unset(request.order):
             query['Order'] = request.order
```

### Comparing `alibabacloud_pai-dlc20201203_py2-1.2.5/alibabacloud_pai_dlc20201203/models.py` & `alibabacloud_pai-dlc20201203_py2-1.2.6/alibabacloud_pai_dlc20201203/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -9913,2350 +9913,2524 @@
 00026b80: 0a20 2020 2020 2020 2020 2020 2074 656d  .            tem
 00026b90: 705f 6d6f 6465 6c20 3d20 5465 6e73 6f72  p_model = Tensor
 00026ba0: 626f 6172 6428 290a 2020 2020 2020 2020  board().        
 00026bb0: 2020 2020 7365 6c66 2e62 6f64 7920 3d20      self.body = 
 00026bc0: 7465 6d70 5f6d 6f64 656c 2e66 726f 6d5f  temp_model.from_
 00026bd0: 6d61 7028 6d5b 2762 6f64 7927 5d29 0a20  map(m['body']). 
 00026be0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00026bf0: 6c66 0a0a 0a63 6c61 7373 204c 6973 7445  lf...class ListE
-00026c00: 6373 5370 6563 7352 6571 7565 7374 2854  csSpecsRequest(T
-00026c10: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
-00026c20: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
-00026c30: 2061 6363 656c 6572 6174 6f72 5f74 7970   accelerator_typ
-00026c40: 653d 4e6f 6e65 2c20 6f72 6465 723d 4e6f  e=None, order=No
-00026c50: 6e65 2c20 7061 6765 5f6e 756d 6265 723d  ne, page_number=
-00026c60: 4e6f 6e65 2c20 7061 6765 5f73 697a 653d  None, page_size=
-00026c70: 4e6f 6e65 2c20 736f 7274 5f62 793d 4e6f  None, sort_by=No
-00026c80: 6e65 293a 0a20 2020 2020 2020 2073 656c  ne):.        sel
-00026c90: 662e 6163 6365 6c65 7261 746f 725f 7479  f.accelerator_ty
-00026ca0: 7065 203d 2061 6363 656c 6572 6174 6f72  pe = accelerator
-00026cb0: 5f74 7970 6520 2023 2074 7970 653a 2073  _type  # type: s
-00026cc0: 7472 0a20 2020 2020 2020 2073 656c 662e  tr.        self.
-00026cd0: 6f72 6465 7220 3d20 6f72 6465 7220 2023  order = order  #
-00026ce0: 2074 7970 653a 2073 7472 0a20 2020 2020   type: str.     
-00026cf0: 2020 2073 656c 662e 7061 6765 5f6e 756d     self.page_num
-00026d00: 6265 7220 3d20 7061 6765 5f6e 756d 6265  ber = page_numbe
-00026d10: 7220 2023 2074 7970 653a 2069 6e74 0a20  r  # type: int. 
-00026d20: 2020 2020 2020 2073 656c 662e 7061 6765         self.page
-00026d30: 5f73 697a 6520 3d20 7061 6765 5f73 697a  _size = page_siz
-00026d40: 6520 2023 2074 7970 653a 2069 6e74 0a20  e  # type: int. 
-00026d50: 2020 2020 2020 2073 656c 662e 736f 7274         self.sort
-00026d60: 5f62 7920 3d20 736f 7274 5f62 7920 2023  _by = sort_by  #
-00026d70: 2074 7970 653a 2073 7472 0a0a 2020 2020   type: str..    
-00026d80: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
-00026d90: 6629 3a0a 2020 2020 2020 2020 7061 7373  f):.        pass
-00026da0: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
-00026db0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00026dc0: 5f6d 6170 203d 2073 7570 6572 284c 6973  _map = super(Lis
-00026dd0: 7445 6373 5370 6563 7352 6571 7565 7374  tEcsSpecsRequest
-00026de0: 2c20 7365 6c66 292e 746f 5f6d 6170 2829  , self).to_map()
-00026df0: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
-00026e00: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00026e10: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00026e20: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
-00026e30: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
-00026e40: 2020 2020 2020 2069 6620 7365 6c66 2e61         if self.a
-00026e50: 6363 656c 6572 6174 6f72 5f74 7970 6520  ccelerator_type 
-00026e60: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00026e70: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-00026e80: 2741 6363 656c 6572 6174 6f72 5479 7065  'AcceleratorType
-00026e90: 275d 203d 2073 656c 662e 6163 6365 6c65  '] = self.accele
-00026ea0: 7261 746f 725f 7479 7065 0a20 2020 2020  rator_type.     
-00026eb0: 2020 2069 6620 7365 6c66 2e6f 7264 6572     if self.order
-00026ec0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00026ed0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00026ee0: 5b27 4f72 6465 7227 5d20 3d20 7365 6c66  ['Order'] = self
-00026ef0: 2e6f 7264 6572 0a20 2020 2020 2020 2069  .order.        i
-00026f00: 6620 7365 6c66 2e70 6167 655f 6e75 6d62  f self.page_numb
-00026f10: 6572 2069 7320 6e6f 7420 4e6f 6e65 3a0a  er is not None:.
-00026f20: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00026f30: 6c74 5b27 5061 6765 4e75 6d62 6572 275d  lt['PageNumber']
-00026f40: 203d 2073 656c 662e 7061 6765 5f6e 756d   = self.page_num
-00026f50: 6265 720a 2020 2020 2020 2020 6966 2073  ber.        if s
-00026f60: 656c 662e 7061 6765 5f73 697a 6520 6973  elf.page_size is
-00026f70: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00026f80: 2020 2020 2020 2072 6573 756c 745b 2750         result['P
-00026f90: 6167 6553 697a 6527 5d20 3d20 7365 6c66  ageSize'] = self
-00026fa0: 2e70 6167 655f 7369 7a65 0a20 2020 2020  .page_size.     
-00026fb0: 2020 2069 6620 7365 6c66 2e73 6f72 745f     if self.sort_
-00026fc0: 6279 2069 7320 6e6f 7420 4e6f 6e65 3a0a  by is not None:.
-00026fd0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00026fe0: 6c74 5b27 536f 7274 4279 275d 203d 2073  lt['SortBy'] = s
-00026ff0: 656c 662e 736f 7274 5f62 790a 2020 2020  elf.sort_by.    
-00027000: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
-00027010: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
-00027020: 6d61 7028 7365 6c66 2c20 6d3d 4e6f 6e65  map(self, m=None
-00027030: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
-00027040: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
-00027050: 2020 2069 6620 6d2e 6765 7428 2741 6363     if m.get('Acc
-00027060: 656c 6572 6174 6f72 5479 7065 2729 2069  eleratorType') i
-00027070: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00027080: 2020 2020 2020 2020 7365 6c66 2e61 6363          self.acc
-00027090: 656c 6572 6174 6f72 5f74 7970 6520 3d20  elerator_type = 
-000270a0: 6d2e 6765 7428 2741 6363 656c 6572 6174  m.get('Accelerat
-000270b0: 6f72 5479 7065 2729 0a20 2020 2020 2020  orType').       
-000270c0: 2069 6620 6d2e 6765 7428 274f 7264 6572   if m.get('Order
-000270d0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-000270e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000270f0: 2e6f 7264 6572 203d 206d 2e67 6574 2827  .order = m.get('
-00027100: 4f72 6465 7227 290a 2020 2020 2020 2020  Order').        
-00027110: 6966 206d 2e67 6574 2827 5061 6765 4e75  if m.get('PageNu
-00027120: 6d62 6572 2729 2069 7320 6e6f 7420 4e6f  mber') is not No
-00027130: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00027140: 7365 6c66 2e70 6167 655f 6e75 6d62 6572  self.page_number
-00027150: 203d 206d 2e67 6574 2827 5061 6765 4e75   = m.get('PageNu
-00027160: 6d62 6572 2729 0a20 2020 2020 2020 2069  mber').        i
-00027170: 6620 6d2e 6765 7428 2750 6167 6553 697a  f m.get('PageSiz
-00027180: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
-00027190: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000271a0: 662e 7061 6765 5f73 697a 6520 3d20 6d2e  f.page_size = m.
-000271b0: 6765 7428 2750 6167 6553 697a 6527 290a  get('PageSize').
-000271c0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-000271d0: 2827 536f 7274 4279 2729 2069 7320 6e6f  ('SortBy') is no
-000271e0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000271f0: 2020 2020 7365 6c66 2e73 6f72 745f 6279      self.sort_by
-00027200: 203d 206d 2e67 6574 2827 536f 7274 4279   = m.get('SortBy
-00027210: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
-00027220: 6e20 7365 6c66 0a0a 0a63 6c61 7373 204c  n self...class L
-00027230: 6973 7445 6373 5370 6563 7352 6573 706f  istEcsSpecsRespo
-00027240: 6e73 6542 6f64 7928 5465 614d 6f64 656c  nseBody(TeaModel
-00027250: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
-00027260: 745f 5f28 7365 6c66 2c20 6563 735f 7370  t__(self, ecs_sp
-00027270: 6563 733d 4e6f 6e65 2c20 7265 7175 6573  ecs=None, reques
-00027280: 745f 6964 3d4e 6f6e 652c 2074 6f74 616c  t_id=None, total
-00027290: 5f63 6f75 6e74 3d4e 6f6e 6529 3a0a 2020  _count=None):.  
-000272a0: 2020 2020 2020 7365 6c66 2e65 6373 5f73        self.ecs_s
-000272b0: 7065 6373 203d 2065 6373 5f73 7065 6373  pecs = ecs_specs
-000272c0: 2020 2320 7479 7065 3a20 6c69 7374 5b45    # type: list[E
-000272d0: 6373 5370 6563 5d0a 2020 2020 2020 2020  csSpec].        
-000272e0: 7365 6c66 2e72 6571 7565 7374 5f69 6420  self.request_id 
-000272f0: 3d20 7265 7175 6573 745f 6964 2020 2320  = request_id  # 
-00027300: 7479 7065 3a20 7374 720a 2020 2020 2020  type: str.      
-00027310: 2020 7365 6c66 2e74 6f74 616c 5f63 6f75    self.total_cou
-00027320: 6e74 203d 2074 6f74 616c 5f63 6f75 6e74  nt = total_count
-00027330: 2020 2320 7479 7065 3a20 6c6f 6e67 0a0a    # type: long..
-00027340: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
-00027350: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00027360: 6966 2073 656c 662e 6563 735f 7370 6563  if self.ecs_spec
-00027370: 733a 0a20 2020 2020 2020 2020 2020 2066  s:.            f
-00027380: 6f72 206b 2069 6e20 7365 6c66 2e65 6373  or k in self.ecs
-00027390: 5f73 7065 6373 3a0a 2020 2020 2020 2020  _specs:.        
-000273a0: 2020 2020 2020 2020 6966 206b 3a0a 2020          if k:.  
-000273b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000273c0: 2020 6b2e 7661 6c69 6461 7465 2829 0a0a    k.validate()..
-000273d0: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
-000273e0: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
-000273f0: 6170 203d 2073 7570 6572 284c 6973 7445  ap = super(ListE
-00027400: 6373 5370 6563 7352 6573 706f 6e73 6542  csSpecsResponseB
-00027410: 6f64 792c 2073 656c 6629 2e74 6f5f 6d61  ody, self).to_ma
-00027420: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
-00027430: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
-00027440: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00027450: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
-00027460: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
-00027470: 290a 2020 2020 2020 2020 7265 7375 6c74  ).        result
-00027480: 5b27 4563 7353 7065 6373 275d 203d 205b  ['EcsSpecs'] = [
-00027490: 5d0a 2020 2020 2020 2020 6966 2073 656c  ].        if sel
-000274a0: 662e 6563 735f 7370 6563 7320 6973 206e  f.ecs_specs is n
-000274b0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-000274c0: 2020 2020 2066 6f72 206b 2069 6e20 7365       for k in se
-000274d0: 6c66 2e65 6373 5f73 7065 6373 3a0a 2020  lf.ecs_specs:.  
-000274e0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-000274f0: 7375 6c74 5b27 4563 7353 7065 6373 275d  sult['EcsSpecs']
-00027500: 2e61 7070 656e 6428 6b2e 746f 5f6d 6170  .append(k.to_map
-00027510: 2829 2069 6620 6b20 656c 7365 204e 6f6e  () if k else Non
-00027520: 6529 0a20 2020 2020 2020 2069 6620 7365  e).        if se
-00027530: 6c66 2e72 6571 7565 7374 5f69 6420 6973  lf.request_id is
-00027540: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00027550: 2020 2020 2020 2072 6573 756c 745b 2752         result['R
-00027560: 6571 7565 7374 4964 275d 203d 2073 656c  equestId'] = sel
-00027570: 662e 7265 7175 6573 745f 6964 0a20 2020  f.request_id.   
-00027580: 2020 2020 2069 6620 7365 6c66 2e74 6f74       if self.tot
-00027590: 616c 5f63 6f75 6e74 2069 7320 6e6f 7420  al_count is not 
-000275a0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000275b0: 2020 7265 7375 6c74 5b27 546f 7461 6c43    result['TotalC
-000275c0: 6f75 6e74 275d 203d 2073 656c 662e 746f  ount'] = self.to
-000275d0: 7461 6c5f 636f 756e 740a 2020 2020 2020  tal_count.      
-000275e0: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
-000275f0: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
-00027600: 7028 7365 6c66 2c20 6d3d 4e6f 6e65 293a  p(self, m=None):
-00027610: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
-00027620: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
-00027630: 2073 656c 662e 6563 735f 7370 6563 7320   self.ecs_specs 
-00027640: 3d20 5b5d 0a20 2020 2020 2020 2069 6620  = [].        if 
-00027650: 6d2e 6765 7428 2745 6373 5370 6563 7327  m.get('EcsSpecs'
-00027660: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-00027670: 2020 2020 2020 2020 2020 2066 6f72 206b             for k
-00027680: 2069 6e20 6d2e 6765 7428 2745 6373 5370   in m.get('EcsSp
-00027690: 6563 7327 293a 0a20 2020 2020 2020 2020  ecs'):.         
-000276a0: 2020 2020 2020 2074 656d 705f 6d6f 6465         temp_mode
-000276b0: 6c20 3d20 4563 7353 7065 6328 290a 2020  l = EcsSpec().  
-000276c0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000276d0: 6c66 2e65 6373 5f73 7065 6373 2e61 7070  lf.ecs_specs.app
-000276e0: 656e 6428 7465 6d70 5f6d 6f64 656c 2e66  end(temp_model.f
-000276f0: 726f 6d5f 6d61 7028 6b29 290a 2020 2020  rom_map(k)).    
-00027700: 2020 2020 6966 206d 2e67 6574 2827 5265      if m.get('Re
-00027710: 7175 6573 7449 6427 2920 6973 206e 6f74  questId') is not
-00027720: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00027730: 2020 2073 656c 662e 7265 7175 6573 745f     self.request_
-00027740: 6964 203d 206d 2e67 6574 2827 5265 7175  id = m.get('Requ
-00027750: 6573 7449 6427 290a 2020 2020 2020 2020  estId').        
-00027760: 6966 206d 2e67 6574 2827 546f 7461 6c43  if m.get('TotalC
-00027770: 6f75 6e74 2729 2069 7320 6e6f 7420 4e6f  ount') is not No
-00027780: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00027790: 7365 6c66 2e74 6f74 616c 5f63 6f75 6e74  self.total_count
-000277a0: 203d 206d 2e67 6574 2827 546f 7461 6c43   = m.get('TotalC
-000277b0: 6f75 6e74 2729 0a20 2020 2020 2020 2072  ount').        r
-000277c0: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
-000277d0: 7373 204c 6973 7445 6373 5370 6563 7352  ss ListEcsSpecsR
-000277e0: 6573 706f 6e73 6528 5465 614d 6f64 656c  esponse(TeaModel
-000277f0: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
-00027800: 745f 5f28 7365 6c66 2c20 6865 6164 6572  t__(self, header
-00027810: 733d 4e6f 6e65 2c20 7374 6174 7573 5f63  s=None, status_c
-00027820: 6f64 653d 4e6f 6e65 2c20 626f 6479 3d4e  ode=None, body=N
-00027830: 6f6e 6529 3a0a 2020 2020 2020 2020 7365  one):.        se
-00027840: 6c66 2e68 6561 6465 7273 203d 2068 6561  lf.headers = hea
-00027850: 6465 7273 2020 2320 7479 7065 3a20 6469  ders  # type: di
-00027860: 6374 5b73 7472 2c20 7374 725d 0a20 2020  ct[str, str].   
-00027870: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
-00027880: 5f63 6f64 6520 3d20 7374 6174 7573 5f63  _code = status_c
-00027890: 6f64 6520 2023 2074 7970 653a 2069 6e74  ode  # type: int
-000278a0: 0a20 2020 2020 2020 2073 656c 662e 626f  .        self.bo
-000278b0: 6479 203d 2062 6f64 7920 2023 2074 7970  dy = body  # typ
-000278c0: 653a 204c 6973 7445 6373 5370 6563 7352  e: ListEcsSpecsR
-000278d0: 6573 706f 6e73 6542 6f64 790a 0a20 2020  esponseBody..   
-000278e0: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
-000278f0: 6c66 293a 0a20 2020 2020 2020 2073 656c  lf):.        sel
-00027900: 662e 7661 6c69 6461 7465 5f72 6571 7569  f.validate_requi
-00027910: 7265 6428 7365 6c66 2e68 6561 6465 7273  red(self.headers
-00027920: 2c20 2768 6561 6465 7273 2729 0a20 2020  , 'headers').   
-00027930: 2020 2020 2073 656c 662e 7661 6c69 6461       self.valida
-00027940: 7465 5f72 6571 7569 7265 6428 7365 6c66  te_required(self
-00027950: 2e73 7461 7475 735f 636f 6465 2c20 2773  .status_code, 's
-00027960: 7461 7475 735f 636f 6465 2729 0a20 2020  tatus_code').   
-00027970: 2020 2020 2073 656c 662e 7661 6c69 6461       self.valida
-00027980: 7465 5f72 6571 7569 7265 6428 7365 6c66  te_required(self
-00027990: 2e62 6f64 792c 2027 626f 6479 2729 0a20  .body, 'body'). 
-000279a0: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
-000279b0: 6f64 793a 0a20 2020 2020 2020 2020 2020  ody:.           
-000279c0: 2073 656c 662e 626f 6479 2e76 616c 6964   self.body.valid
-000279d0: 6174 6528 290a 0a20 2020 2064 6566 2074  ate()..    def t
-000279e0: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
-000279f0: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
-00027a00: 7228 4c69 7374 4563 7353 7065 6373 5265  r(ListEcsSpecsRe
-00027a10: 7370 6f6e 7365 2c20 7365 6c66 292e 746f  sponse, self).to
-00027a20: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
-00027a30: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
-00027a40: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00027a50: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
-00027a60: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
-00027a70: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
-00027a80: 7365 6c66 2e68 6561 6465 7273 2069 7320  self.headers is 
-00027a90: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00027aa0: 2020 2020 2020 7265 7375 6c74 5b27 6865        result['he
-00027ab0: 6164 6572 7327 5d20 3d20 7365 6c66 2e68  aders'] = self.h
-00027ac0: 6561 6465 7273 0a20 2020 2020 2020 2069  eaders.        i
-00027ad0: 6620 7365 6c66 2e73 7461 7475 735f 636f  f self.status_co
-00027ae0: 6465 2069 7320 6e6f 7420 4e6f 6e65 3a0a  de is not None:.
-00027af0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00027b00: 6c74 5b27 7374 6174 7573 436f 6465 275d  lt['statusCode']
-00027b10: 203d 2073 656c 662e 7374 6174 7573 5f63   = self.status_c
-00027b20: 6f64 650a 2020 2020 2020 2020 6966 2073  ode.        if s
-00027b30: 656c 662e 626f 6479 2069 7320 6e6f 7420  elf.body is not 
-00027b40: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00027b50: 2020 7265 7375 6c74 5b27 626f 6479 275d    result['body']
-00027b60: 203d 2073 656c 662e 626f 6479 2e74 6f5f   = self.body.to_
-00027b70: 6d61 7028 290a 2020 2020 2020 2020 7265  map().        re
-00027b80: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
-00027b90: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
-00027ba0: 6c66 2c20 6d3d 4e6f 6e65 293a 0a20 2020  lf, m=None):.   
-00027bb0: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
-00027bc0: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
-00027bd0: 6d2e 6765 7428 2768 6561 6465 7273 2729  m.get('headers')
-00027be0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00027bf0: 2020 2020 2020 2020 2020 7365 6c66 2e68            self.h
-00027c00: 6561 6465 7273 203d 206d 2e67 6574 2827  eaders = m.get('
-00027c10: 6865 6164 6572 7327 290a 2020 2020 2020  headers').      
-00027c20: 2020 6966 206d 2e67 6574 2827 7374 6174    if m.get('stat
-00027c30: 7573 436f 6465 2729 2069 7320 6e6f 7420  usCode') is not 
-00027c40: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00027c50: 2020 7365 6c66 2e73 7461 7475 735f 636f    self.status_co
-00027c60: 6465 203d 206d 2e67 6574 2827 7374 6174  de = m.get('stat
-00027c70: 7573 436f 6465 2729 0a20 2020 2020 2020  usCode').       
-00027c80: 2069 6620 6d2e 6765 7428 2762 6f64 7927   if m.get('body'
-00027c90: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-00027ca0: 2020 2020 2020 2020 2020 2074 656d 705f             temp_
-00027cb0: 6d6f 6465 6c20 3d20 4c69 7374 4563 7353  model = ListEcsS
-00027cc0: 7065 6373 5265 7370 6f6e 7365 426f 6479  pecsResponseBody
-00027cd0: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
-00027ce0: 656c 662e 626f 6479 203d 2074 656d 705f  elf.body = temp_
-00027cf0: 6d6f 6465 6c2e 6672 6f6d 5f6d 6170 286d  model.from_map(m
-00027d00: 5b27 626f 6479 275d 290a 2020 2020 2020  ['body']).      
-00027d10: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
-00027d20: 636c 6173 7320 4c69 7374 4a6f 6273 5265  class ListJobsRe
-00027d30: 7175 6573 7428 5465 614d 6f64 656c 293a  quest(TeaModel):
-00027d40: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-00027d50: 5f28 7365 6c66 2c20 6275 7369 6e65 7373  _(self, business
-00027d60: 5f75 7365 725f 6964 3d4e 6f6e 652c 2063  _user_id=None, c
-00027d70: 616c 6c65 723d 4e6f 6e65 2c20 6469 7370  aller=None, disp
-00027d80: 6c61 795f 6e61 6d65 3d4e 6f6e 652c 2065  lay_name=None, e
-00027d90: 6e64 5f74 696d 653d 4e6f 6e65 2c0a 2020  nd_time=None,.  
-00027da0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00027db0: 726f 6d5f 616c 6c5f 776f 726b 7370 6163  rom_all_workspac
-00027dc0: 6573 3d4e 6f6e 652c 206a 6f62 5f69 643d  es=None, job_id=
-00027dd0: 4e6f 6e65 2c20 6a6f 625f 7479 7065 3d4e  None, job_type=N
-00027de0: 6f6e 652c 206f 7264 6572 3d4e 6f6e 652c  one, order=None,
-00027df0: 2070 6167 655f 6e75 6d62 6572 3d4e 6f6e   page_number=Non
-00027e00: 652c 2070 6167 655f 7369 7a65 3d4e 6f6e  e, page_size=Non
-00027e10: 652c 2070 6970 656c 696e 655f 6964 3d4e  e, pipeline_id=N
-00027e20: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-00027e30: 2020 2020 2020 7265 736f 7572 6365 5f69        resource_i
-00027e40: 643d 4e6f 6e65 2c20 7368 6f77 5f6f 776e  d=None, show_own
-00027e50: 3d4e 6f6e 652c 2073 6f72 745f 6279 3d4e  =None, sort_by=N
-00027e60: 6f6e 652c 2073 7461 7274 5f74 696d 653d  one, start_time=
-00027e70: 4e6f 6e65 2c20 7374 6174 7573 3d4e 6f6e  None, status=Non
-00027e80: 652c 2074 6167 733d 4e6f 6e65 2c20 776f  e, tags=None, wo
-00027e90: 726b 7370 6163 655f 6964 3d4e 6f6e 6529  rkspace_id=None)
-00027ea0: 3a0a 2020 2020 2020 2020 7365 6c66 2e62  :.        self.b
-00027eb0: 7573 696e 6573 735f 7573 6572 5f69 6420  usiness_user_id 
-00027ec0: 3d20 6275 7369 6e65 7373 5f75 7365 725f  = business_user_
-00027ed0: 6964 2020 2320 7479 7065 3a20 7374 720a  id  # type: str.
-00027ee0: 2020 2020 2020 2020 7365 6c66 2e63 616c          self.cal
-00027ef0: 6c65 7220 3d20 6361 6c6c 6572 2020 2320  ler = caller  # 
-00027f00: 7479 7065 3a20 7374 720a 2020 2020 2020  type: str.      
-00027f10: 2020 7365 6c66 2e64 6973 706c 6179 5f6e    self.display_n
-00027f20: 616d 6520 3d20 6469 7370 6c61 795f 6e61  ame = display_na
-00027f30: 6d65 2020 2320 7479 7065 3a20 7374 720a  me  # type: str.
-00027f40: 2020 2020 2020 2020 7365 6c66 2e65 6e64          self.end
-00027f50: 5f74 696d 6520 3d20 656e 645f 7469 6d65  _time = end_time
-00027f60: 2020 2320 7479 7065 3a20 7374 720a 2020    # type: str.  
-00027f70: 2020 2020 2020 7365 6c66 2e66 726f 6d5f        self.from_
-00027f80: 616c 6c5f 776f 726b 7370 6163 6573 203d  all_workspaces =
-00027f90: 2066 726f 6d5f 616c 6c5f 776f 726b 7370   from_all_worksp
-00027fa0: 6163 6573 2020 2320 7479 7065 3a20 626f  aces  # type: bo
-00027fb0: 6f6c 0a20 2020 2020 2020 2073 656c 662e  ol.        self.
-00027fc0: 6a6f 625f 6964 203d 206a 6f62 5f69 6420  job_id = job_id 
-00027fd0: 2023 2074 7970 653a 2073 7472 0a20 2020   # type: str.   
-00027fe0: 2020 2020 2073 656c 662e 6a6f 625f 7479       self.job_ty
-00027ff0: 7065 203d 206a 6f62 5f74 7970 6520 2023  pe = job_type  #
-00028000: 2074 7970 653a 2073 7472 0a20 2020 2020   type: str.     
-00028010: 2020 2073 656c 662e 6f72 6465 7220 3d20     self.order = 
-00028020: 6f72 6465 7220 2023 2074 7970 653a 2073  order  # type: s
-00028030: 7472 0a20 2020 2020 2020 2073 656c 662e  tr.        self.
-00028040: 7061 6765 5f6e 756d 6265 7220 3d20 7061  page_number = pa
-00028050: 6765 5f6e 756d 6265 7220 2023 2074 7970  ge_number  # typ
-00028060: 653a 2069 6e74 0a20 2020 2020 2020 2073  e: int.        s
-00028070: 656c 662e 7061 6765 5f73 697a 6520 3d20  elf.page_size = 
-00028080: 7061 6765 5f73 697a 6520 2023 2074 7970  page_size  # typ
-00028090: 653a 2069 6e74 0a20 2020 2020 2020 2073  e: int.        s
-000280a0: 656c 662e 7069 7065 6c69 6e65 5f69 6420  elf.pipeline_id 
-000280b0: 3d20 7069 7065 6c69 6e65 5f69 6420 2023  = pipeline_id  #
-000280c0: 2074 7970 653a 2073 7472 0a20 2020 2020   type: str.     
-000280d0: 2020 2073 656c 662e 7265 736f 7572 6365     self.resource
-000280e0: 5f69 6420 3d20 7265 736f 7572 6365 5f69  _id = resource_i
-000280f0: 6420 2023 2074 7970 653a 2073 7472 0a20  d  # type: str. 
-00028100: 2020 2020 2020 2073 656c 662e 7368 6f77         self.show
-00028110: 5f6f 776e 203d 2073 686f 775f 6f77 6e20  _own = show_own 
-00028120: 2023 2074 7970 653a 2062 6f6f 6c0a 2020   # type: bool.  
-00028130: 2020 2020 2020 7365 6c66 2e73 6f72 745f        self.sort_
-00028140: 6279 203d 2073 6f72 745f 6279 2020 2320  by = sort_by  # 
-00028150: 7479 7065 3a20 7374 720a 2020 2020 2020  type: str.      
-00028160: 2020 7365 6c66 2e73 7461 7274 5f74 696d    self.start_tim
-00028170: 6520 3d20 7374 6172 745f 7469 6d65 2020  e = start_time  
-00028180: 2320 7479 7065 3a20 7374 720a 2020 2020  # type: str.    
-00028190: 2020 2020 7365 6c66 2e73 7461 7475 7320      self.status 
-000281a0: 3d20 7374 6174 7573 2020 2320 7479 7065  = status  # type
-000281b0: 3a20 7374 720a 2020 2020 2020 2020 7365  : str.        se
-000281c0: 6c66 2e74 6167 7320 3d20 7461 6773 2020  lf.tags = tags  
-000281d0: 2320 7479 7065 3a20 6469 6374 5b73 7472  # type: dict[str
-000281e0: 2c20 7374 725d 0a20 2020 2020 2020 2073  , str].        s
-000281f0: 656c 662e 776f 726b 7370 6163 655f 6964  elf.workspace_id
-00028200: 203d 2077 6f72 6b73 7061 6365 5f69 6420   = workspace_id 
-00028210: 2023 2074 7970 653a 2073 7472 0a0a 2020   # type: str..  
-00028220: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
-00028230: 656c 6629 3a0a 2020 2020 2020 2020 7061  elf):.        pa
-00028240: 7373 0a0a 2020 2020 6465 6620 746f 5f6d  ss..    def to_m
-00028250: 6170 2873 656c 6629 3a0a 2020 2020 2020  ap(self):.      
-00028260: 2020 5f6d 6170 203d 2073 7570 6572 284c    _map = super(L
-00028270: 6973 744a 6f62 7352 6571 7565 7374 2c20  istJobsRequest, 
-00028280: 7365 6c66 292e 746f 5f6d 6170 2829 0a20  self).to_map(). 
-00028290: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
-000282a0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000282b0: 2020 2020 2020 2020 7265 7475 726e 205f          return _
-000282c0: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
-000282d0: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
-000282e0: 2020 2020 2069 6620 7365 6c66 2e62 7573       if self.bus
-000282f0: 696e 6573 735f 7573 6572 5f69 6420 6973  iness_user_id is
-00028300: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00028310: 2020 2020 2020 2072 6573 756c 745b 2742         result['B
-00028320: 7573 696e 6573 7355 7365 7249 6427 5d20  usinessUserId'] 
-00028330: 3d20 7365 6c66 2e62 7573 696e 6573 735f  = self.business_
-00028340: 7573 6572 5f69 640a 2020 2020 2020 2020  user_id.        
-00028350: 6966 2073 656c 662e 6361 6c6c 6572 2069  if self.caller i
-00028360: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00028370: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-00028380: 4361 6c6c 6572 275d 203d 2073 656c 662e  Caller'] = self.
-00028390: 6361 6c6c 6572 0a20 2020 2020 2020 2069  caller.        i
-000283a0: 6620 7365 6c66 2e64 6973 706c 6179 5f6e  f self.display_n
-000283b0: 616d 6520 6973 206e 6f74 204e 6f6e 653a  ame is not None:
-000283c0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-000283d0: 756c 745b 2744 6973 706c 6179 4e61 6d65  ult['DisplayName
-000283e0: 275d 203d 2073 656c 662e 6469 7370 6c61  '] = self.displa
-000283f0: 795f 6e61 6d65 0a20 2020 2020 2020 2069  y_name.        i
-00028400: 6620 7365 6c66 2e65 6e64 5f74 696d 6520  f self.end_time 
-00028410: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00028420: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-00028430: 2745 6e64 5469 6d65 275d 203d 2073 656c  'EndTime'] = sel
-00028440: 662e 656e 645f 7469 6d65 0a20 2020 2020  f.end_time.     
-00028450: 2020 2069 6620 7365 6c66 2e66 726f 6d5f     if self.from_
-00028460: 616c 6c5f 776f 726b 7370 6163 6573 2069  all_workspaces i
-00028470: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00028480: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-00028490: 4672 6f6d 416c 6c57 6f72 6b73 7061 6365  FromAllWorkspace
-000284a0: 7327 5d20 3d20 7365 6c66 2e66 726f 6d5f  s'] = self.from_
-000284b0: 616c 6c5f 776f 726b 7370 6163 6573 0a20  all_workspaces. 
-000284c0: 2020 2020 2020 2069 6620 7365 6c66 2e6a         if self.j
-000284d0: 6f62 5f69 6420 6973 206e 6f74 204e 6f6e  ob_id is not Non
-000284e0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-000284f0: 6573 756c 745b 274a 6f62 4964 275d 203d  esult['JobId'] =
-00028500: 2073 656c 662e 6a6f 625f 6964 0a20 2020   self.job_id.   
-00028510: 2020 2020 2069 6620 7365 6c66 2e6a 6f62       if self.job
-00028520: 5f74 7970 6520 6973 206e 6f74 204e 6f6e  _type is not Non
-00028530: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00028540: 6573 756c 745b 274a 6f62 5479 7065 275d  esult['JobType']
-00028550: 203d 2073 656c 662e 6a6f 625f 7479 7065   = self.job_type
-00028560: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00028570: 2e6f 7264 6572 2069 7320 6e6f 7420 4e6f  .order is not No
-00028580: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00028590: 7265 7375 6c74 5b27 4f72 6465 7227 5d20  result['Order'] 
-000285a0: 3d20 7365 6c66 2e6f 7264 6572 0a20 2020  = self.order.   
-000285b0: 2020 2020 2069 6620 7365 6c66 2e70 6167       if self.pag
-000285c0: 655f 6e75 6d62 6572 2069 7320 6e6f 7420  e_number is not 
-000285d0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000285e0: 2020 7265 7375 6c74 5b27 5061 6765 4e75    result['PageNu
-000285f0: 6d62 6572 275d 203d 2073 656c 662e 7061  mber'] = self.pa
-00028600: 6765 5f6e 756d 6265 720a 2020 2020 2020  ge_number.      
-00028610: 2020 6966 2073 656c 662e 7061 6765 5f73    if self.page_s
-00028620: 697a 6520 6973 206e 6f74 204e 6f6e 653a  ize is not None:
-00028630: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00028640: 756c 745b 2750 6167 6553 697a 6527 5d20  ult['PageSize'] 
-00028650: 3d20 7365 6c66 2e70 6167 655f 7369 7a65  = self.page_size
-00028660: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00028670: 2e70 6970 656c 696e 655f 6964 2069 7320  .pipeline_id is 
-00028680: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00028690: 2020 2020 2020 7265 7375 6c74 5b27 5069        result['Pi
-000286a0: 7065 6c69 6e65 4964 275d 203d 2073 656c  pelineId'] = sel
-000286b0: 662e 7069 7065 6c69 6e65 5f69 640a 2020  f.pipeline_id.  
-000286c0: 2020 2020 2020 6966 2073 656c 662e 7265        if self.re
-000286d0: 736f 7572 6365 5f69 6420 6973 206e 6f74  source_id is not
-000286e0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000286f0: 2020 2072 6573 756c 745b 2752 6573 6f75     result['Resou
-00028700: 7263 6549 6427 5d20 3d20 7365 6c66 2e72  rceId'] = self.r
-00028710: 6573 6f75 7263 655f 6964 0a20 2020 2020  esource_id.     
-00028720: 2020 2069 6620 7365 6c66 2e73 686f 775f     if self.show_
-00028730: 6f77 6e20 6973 206e 6f74 204e 6f6e 653a  own is not None:
-00028740: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00028750: 756c 745b 2753 686f 774f 776e 275d 203d  ult['ShowOwn'] =
-00028760: 2073 656c 662e 7368 6f77 5f6f 776e 0a20   self.show_own. 
-00028770: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
-00028780: 6f72 745f 6279 2069 7320 6e6f 7420 4e6f  ort_by is not No
-00028790: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000287a0: 7265 7375 6c74 5b27 536f 7274 4279 275d  result['SortBy']
-000287b0: 203d 2073 656c 662e 736f 7274 5f62 790a   = self.sort_by.
-000287c0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000287d0: 7374 6172 745f 7469 6d65 2069 7320 6e6f  start_time is no
-000287e0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000287f0: 2020 2020 7265 7375 6c74 5b27 5374 6172      result['Star
-00028800: 7454 696d 6527 5d20 3d20 7365 6c66 2e73  tTime'] = self.s
-00028810: 7461 7274 5f74 696d 650a 2020 2020 2020  tart_time.      
-00028820: 2020 6966 2073 656c 662e 7374 6174 7573    if self.status
-00028830: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00028840: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00028850: 5b27 5374 6174 7573 275d 203d 2073 656c  ['Status'] = sel
-00028860: 662e 7374 6174 7573 0a20 2020 2020 2020  f.status.       
-00028870: 2069 6620 7365 6c66 2e74 6167 7320 6973   if self.tags is
-00028880: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00028890: 2020 2020 2020 2072 6573 756c 745b 2754         result['T
-000288a0: 6167 7327 5d20 3d20 7365 6c66 2e74 6167  ags'] = self.tag
-000288b0: 730a 2020 2020 2020 2020 6966 2073 656c  s.        if sel
-000288c0: 662e 776f 726b 7370 6163 655f 6964 2069  f.workspace_id i
-000288d0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000288e0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-000288f0: 576f 726b 7370 6163 6549 6427 5d20 3d20  WorkspaceId'] = 
-00028900: 7365 6c66 2e77 6f72 6b73 7061 6365 5f69  self.workspace_i
-00028910: 640a 2020 2020 2020 2020 7265 7475 726e  d.        return
-00028920: 2072 6573 756c 740a 0a20 2020 2064 6566   result..    def
-00028930: 2066 726f 6d5f 6d61 7028 7365 6c66 2c20   from_map(self, 
-00028940: 6d3d 4e6f 6e65 293a 0a20 2020 2020 2020  m=None):.       
-00028950: 206d 203d 206d 206f 7220 6469 6374 2829   m = m or dict()
-00028960: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-00028970: 7428 2742 7573 696e 6573 7355 7365 7249  t('BusinessUserI
-00028980: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
-00028990: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000289a0: 662e 6275 7369 6e65 7373 5f75 7365 725f  f.business_user_
-000289b0: 6964 203d 206d 2e67 6574 2827 4275 7369  id = m.get('Busi
-000289c0: 6e65 7373 5573 6572 4964 2729 0a20 2020  nessUserId').   
-000289d0: 2020 2020 2069 6620 6d2e 6765 7428 2743       if m.get('C
-000289e0: 616c 6c65 7227 2920 6973 206e 6f74 204e  aller') is not N
-000289f0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00028a00: 2073 656c 662e 6361 6c6c 6572 203d 206d   self.caller = m
-00028a10: 2e67 6574 2827 4361 6c6c 6572 2729 0a20  .get('Caller'). 
-00028a20: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-00028a30: 2744 6973 706c 6179 4e61 6d65 2729 2069  'DisplayName') i
-00028a40: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00028a50: 2020 2020 2020 2020 7365 6c66 2e64 6973          self.dis
-00028a60: 706c 6179 5f6e 616d 6520 3d20 6d2e 6765  play_name = m.ge
-00028a70: 7428 2744 6973 706c 6179 4e61 6d65 2729  t('DisplayName')
-00028a80: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-00028a90: 7428 2745 6e64 5469 6d65 2729 2069 7320  t('EndTime') is 
-00028aa0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00028ab0: 2020 2020 2020 7365 6c66 2e65 6e64 5f74        self.end_t
-00028ac0: 696d 6520 3d20 6d2e 6765 7428 2745 6e64  ime = m.get('End
-00028ad0: 5469 6d65 2729 0a20 2020 2020 2020 2069  Time').        i
-00028ae0: 6620 6d2e 6765 7428 2746 726f 6d41 6c6c  f m.get('FromAll
-00028af0: 576f 726b 7370 6163 6573 2729 2069 7320  Workspaces') is 
-00028b00: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00028b10: 2020 2020 2020 7365 6c66 2e66 726f 6d5f        self.from_
-00028b20: 616c 6c5f 776f 726b 7370 6163 6573 203d  all_workspaces =
-00028b30: 206d 2e67 6574 2827 4672 6f6d 416c 6c57   m.get('FromAllW
-00028b40: 6f72 6b73 7061 6365 7327 290a 2020 2020  orkspaces').    
-00028b50: 2020 2020 6966 206d 2e67 6574 2827 4a6f      if m.get('Jo
-00028b60: 6249 6427 2920 6973 206e 6f74 204e 6f6e  bId') is not Non
-00028b70: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00028b80: 656c 662e 6a6f 625f 6964 203d 206d 2e67  elf.job_id = m.g
-00028b90: 6574 2827 4a6f 6249 6427 290a 2020 2020  et('JobId').    
-00028ba0: 2020 2020 6966 206d 2e67 6574 2827 4a6f      if m.get('Jo
-00028bb0: 6254 7970 6527 2920 6973 206e 6f74 204e  bType') is not N
-00028bc0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00028bd0: 2073 656c 662e 6a6f 625f 7479 7065 203d   self.job_type =
-00028be0: 206d 2e67 6574 2827 4a6f 6254 7970 6527   m.get('JobType'
-00028bf0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-00028c00: 6574 2827 4f72 6465 7227 2920 6973 206e  et('Order') is n
-00028c10: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-00028c20: 2020 2020 2073 656c 662e 6f72 6465 7220       self.order 
-00028c30: 3d20 6d2e 6765 7428 274f 7264 6572 2729  = m.get('Order')
-00028c40: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
-00028c50: 7428 2750 6167 654e 756d 6265 7227 2920  t('PageNumber') 
-00028c60: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00028c70: 2020 2020 2020 2020 2073 656c 662e 7061           self.pa
-00028c80: 6765 5f6e 756d 6265 7220 3d20 6d2e 6765  ge_number = m.ge
-00028c90: 7428 2750 6167 654e 756d 6265 7227 290a  t('PageNumber').
-00028ca0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-00028cb0: 2827 5061 6765 5369 7a65 2729 2069 7320  ('PageSize') is 
-00028cc0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00028cd0: 2020 2020 2020 7365 6c66 2e70 6167 655f        self.page_
-00028ce0: 7369 7a65 203d 206d 2e67 6574 2827 5061  size = m.get('Pa
-00028cf0: 6765 5369 7a65 2729 0a20 2020 2020 2020  geSize').       
-00028d00: 2069 6620 6d2e 6765 7428 2750 6970 656c   if m.get('Pipel
-00028d10: 696e 6549 6427 2920 6973 206e 6f74 204e  ineId') is not N
-00028d20: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00028d30: 2073 656c 662e 7069 7065 6c69 6e65 5f69   self.pipeline_i
-00028d40: 6420 3d20 6d2e 6765 7428 2750 6970 656c  d = m.get('Pipel
-00028d50: 696e 6549 6427 290a 2020 2020 2020 2020  ineId').        
-00028d60: 6966 206d 2e67 6574 2827 5265 736f 7572  if m.get('Resour
-00028d70: 6365 4964 2729 2069 7320 6e6f 7420 4e6f  ceId') is not No
-00028d80: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00028d90: 7365 6c66 2e72 6573 6f75 7263 655f 6964  self.resource_id
-00028da0: 203d 206d 2e67 6574 2827 5265 736f 7572   = m.get('Resour
-00028db0: 6365 4964 2729 0a20 2020 2020 2020 2069  ceId').        i
-00028dc0: 6620 6d2e 6765 7428 2753 686f 774f 776e  f m.get('ShowOwn
-00028dd0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-00028de0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00028df0: 2e73 686f 775f 6f77 6e20 3d20 6d2e 6765  .show_own = m.ge
-00028e00: 7428 2753 686f 774f 776e 2729 0a20 2020  t('ShowOwn').   
-00028e10: 2020 2020 2069 6620 6d2e 6765 7428 2753       if m.get('S
-00028e20: 6f72 7442 7927 2920 6973 206e 6f74 204e  ortBy') is not N
-00028e30: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00028e40: 2073 656c 662e 736f 7274 5f62 7920 3d20   self.sort_by = 
-00028e50: 6d2e 6765 7428 2753 6f72 7442 7927 290a  m.get('SortBy').
-00028e60: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-00028e70: 2827 5374 6172 7454 696d 6527 2920 6973  ('StartTime') is
-00028e80: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00028e90: 2020 2020 2020 2073 656c 662e 7374 6172         self.star
-00028ea0: 745f 7469 6d65 203d 206d 2e67 6574 2827  t_time = m.get('
-00028eb0: 5374 6172 7454 696d 6527 290a 2020 2020  StartTime').    
-00028ec0: 2020 2020 6966 206d 2e67 6574 2827 5374      if m.get('St
-00028ed0: 6174 7573 2729 2069 7320 6e6f 7420 4e6f  atus') is not No
-00028ee0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00028ef0: 7365 6c66 2e73 7461 7475 7320 3d20 6d2e  self.status = m.
-00028f00: 6765 7428 2753 7461 7475 7327 290a 2020  get('Status').  
-00028f10: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-00028f20: 5461 6773 2729 2069 7320 6e6f 7420 4e6f  Tags') is not No
-00028f30: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00028f40: 7365 6c66 2e74 6167 7320 3d20 6d2e 6765  self.tags = m.ge
-00028f50: 7428 2754 6167 7327 290a 2020 2020 2020  t('Tags').      
-00028f60: 2020 6966 206d 2e67 6574 2827 576f 726b    if m.get('Work
-00028f70: 7370 6163 6549 6427 2920 6973 206e 6f74  spaceId') is not
-00028f80: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00028f90: 2020 2073 656c 662e 776f 726b 7370 6163     self.workspac
-00028fa0: 655f 6964 203d 206d 2e67 6574 2827 576f  e_id = m.get('Wo
-00028fb0: 726b 7370 6163 6549 6427 290a 2020 2020  rkspaceId').    
-00028fc0: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
-00028fd0: 0a0a 636c 6173 7320 4c69 7374 4a6f 6273  ..class ListJobs
-00028fe0: 5368 7269 6e6b 5265 7175 6573 7428 5465  ShrinkRequest(Te
-00028ff0: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
-00029000: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
-00029010: 6275 7369 6e65 7373 5f75 7365 725f 6964  business_user_id
-00029020: 3d4e 6f6e 652c 2063 616c 6c65 723d 4e6f  =None, caller=No
-00029030: 6e65 2c20 6469 7370 6c61 795f 6e61 6d65  ne, display_name
-00029040: 3d4e 6f6e 652c 2065 6e64 5f74 696d 653d  =None, end_time=
-00029050: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
-00029060: 2020 2020 2020 2066 726f 6d5f 616c 6c5f         from_all_
-00029070: 776f 726b 7370 6163 6573 3d4e 6f6e 652c  workspaces=None,
-00029080: 206a 6f62 5f69 643d 4e6f 6e65 2c20 6a6f   job_id=None, jo
-00029090: 625f 7479 7065 3d4e 6f6e 652c 206f 7264  b_type=None, ord
-000290a0: 6572 3d4e 6f6e 652c 2070 6167 655f 6e75  er=None, page_nu
-000290b0: 6d62 6572 3d4e 6f6e 652c 2070 6167 655f  mber=None, page_
-000290c0: 7369 7a65 3d4e 6f6e 652c 2070 6970 656c  size=None, pipel
-000290d0: 696e 655f 6964 3d4e 6f6e 652c 0a20 2020  ine_id=None,.   
-000290e0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-000290f0: 736f 7572 6365 5f69 643d 4e6f 6e65 2c20  source_id=None, 
-00029100: 7368 6f77 5f6f 776e 3d4e 6f6e 652c 2073  show_own=None, s
-00029110: 6f72 745f 6279 3d4e 6f6e 652c 2073 7461  ort_by=None, sta
-00029120: 7274 5f74 696d 653d 4e6f 6e65 2c20 7374  rt_time=None, st
-00029130: 6174 7573 3d4e 6f6e 652c 2074 6167 735f  atus=None, tags_
-00029140: 7368 7269 6e6b 3d4e 6f6e 652c 0a20 2020  shrink=None,.   
-00029150: 2020 2020 2020 2020 2020 2020 2020 776f                wo
-00029160: 726b 7370 6163 655f 6964 3d4e 6f6e 6529  rkspace_id=None)
-00029170: 3a0a 2020 2020 2020 2020 7365 6c66 2e62  :.        self.b
-00029180: 7573 696e 6573 735f 7573 6572 5f69 6420  usiness_user_id 
-00029190: 3d20 6275 7369 6e65 7373 5f75 7365 725f  = business_user_
-000291a0: 6964 2020 2320 7479 7065 3a20 7374 720a  id  # type: str.
-000291b0: 2020 2020 2020 2020 7365 6c66 2e63 616c          self.cal
-000291c0: 6c65 7220 3d20 6361 6c6c 6572 2020 2320  ler = caller  # 
-000291d0: 7479 7065 3a20 7374 720a 2020 2020 2020  type: str.      
-000291e0: 2020 7365 6c66 2e64 6973 706c 6179 5f6e    self.display_n
-000291f0: 616d 6520 3d20 6469 7370 6c61 795f 6e61  ame = display_na
-00029200: 6d65 2020 2320 7479 7065 3a20 7374 720a  me  # type: str.
-00029210: 2020 2020 2020 2020 7365 6c66 2e65 6e64          self.end
-00029220: 5f74 696d 6520 3d20 656e 645f 7469 6d65  _time = end_time
-00029230: 2020 2320 7479 7065 3a20 7374 720a 2020    # type: str.  
-00029240: 2020 2020 2020 7365 6c66 2e66 726f 6d5f        self.from_
-00029250: 616c 6c5f 776f 726b 7370 6163 6573 203d  all_workspaces =
-00029260: 2066 726f 6d5f 616c 6c5f 776f 726b 7370   from_all_worksp
-00029270: 6163 6573 2020 2320 7479 7065 3a20 626f  aces  # type: bo
-00029280: 6f6c 0a20 2020 2020 2020 2073 656c 662e  ol.        self.
-00029290: 6a6f 625f 6964 203d 206a 6f62 5f69 6420  job_id = job_id 
-000292a0: 2023 2074 7970 653a 2073 7472 0a20 2020   # type: str.   
-000292b0: 2020 2020 2073 656c 662e 6a6f 625f 7479       self.job_ty
-000292c0: 7065 203d 206a 6f62 5f74 7970 6520 2023  pe = job_type  #
-000292d0: 2074 7970 653a 2073 7472 0a20 2020 2020   type: str.     
-000292e0: 2020 2073 656c 662e 6f72 6465 7220 3d20     self.order = 
-000292f0: 6f72 6465 7220 2023 2074 7970 653a 2073  order  # type: s
-00029300: 7472 0a20 2020 2020 2020 2073 656c 662e  tr.        self.
-00029310: 7061 6765 5f6e 756d 6265 7220 3d20 7061  page_number = pa
-00029320: 6765 5f6e 756d 6265 7220 2023 2074 7970  ge_number  # typ
-00029330: 653a 2069 6e74 0a20 2020 2020 2020 2073  e: int.        s
-00029340: 656c 662e 7061 6765 5f73 697a 6520 3d20  elf.page_size = 
-00029350: 7061 6765 5f73 697a 6520 2023 2074 7970  page_size  # typ
-00029360: 653a 2069 6e74 0a20 2020 2020 2020 2073  e: int.        s
-00029370: 656c 662e 7069 7065 6c69 6e65 5f69 6420  elf.pipeline_id 
-00029380: 3d20 7069 7065 6c69 6e65 5f69 6420 2023  = pipeline_id  #
-00029390: 2074 7970 653a 2073 7472 0a20 2020 2020   type: str.     
-000293a0: 2020 2073 656c 662e 7265 736f 7572 6365     self.resource
-000293b0: 5f69 6420 3d20 7265 736f 7572 6365 5f69  _id = resource_i
-000293c0: 6420 2023 2074 7970 653a 2073 7472 0a20  d  # type: str. 
-000293d0: 2020 2020 2020 2073 656c 662e 7368 6f77         self.show
-000293e0: 5f6f 776e 203d 2073 686f 775f 6f77 6e20  _own = show_own 
-000293f0: 2023 2074 7970 653a 2062 6f6f 6c0a 2020   # type: bool.  
-00029400: 2020 2020 2020 7365 6c66 2e73 6f72 745f        self.sort_
-00029410: 6279 203d 2073 6f72 745f 6279 2020 2320  by = sort_by  # 
-00029420: 7479 7065 3a20 7374 720a 2020 2020 2020  type: str.      
-00029430: 2020 7365 6c66 2e73 7461 7274 5f74 696d    self.start_tim
-00029440: 6520 3d20 7374 6172 745f 7469 6d65 2020  e = start_time  
-00029450: 2320 7479 7065 3a20 7374 720a 2020 2020  # type: str.    
-00029460: 2020 2020 7365 6c66 2e73 7461 7475 7320      self.status 
-00029470: 3d20 7374 6174 7573 2020 2320 7479 7065  = status  # type
-00029480: 3a20 7374 720a 2020 2020 2020 2020 7365  : str.        se
-00029490: 6c66 2e74 6167 735f 7368 7269 6e6b 203d  lf.tags_shrink =
-000294a0: 2074 6167 735f 7368 7269 6e6b 2020 2320   tags_shrink  # 
-000294b0: 7479 7065 3a20 7374 720a 2020 2020 2020  type: str.      
-000294c0: 2020 7365 6c66 2e77 6f72 6b73 7061 6365    self.workspace
-000294d0: 5f69 6420 3d20 776f 726b 7370 6163 655f  _id = workspace_
-000294e0: 6964 2020 2320 7479 7065 3a20 7374 720a  id  # type: str.
-000294f0: 0a20 2020 2064 6566 2076 616c 6964 6174  .    def validat
-00029500: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
-00029510: 2070 6173 730a 0a20 2020 2064 6566 2074   pass..    def t
-00029520: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
-00029530: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
-00029540: 7228 4c69 7374 4a6f 6273 5368 7269 6e6b  r(ListJobsShrink
-00029550: 5265 7175 6573 742c 2073 656c 6629 2e74  Request, self).t
-00029560: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
-00029570: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
-00029580: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00029590: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
-000295a0: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
-000295b0: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-000295c0: 2073 656c 662e 6275 7369 6e65 7373 5f75   self.business_u
-000295d0: 7365 725f 6964 2069 7320 6e6f 7420 4e6f  ser_id is not No
-000295e0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-000295f0: 7265 7375 6c74 5b27 4275 7369 6e65 7373  result['Business
-00029600: 5573 6572 4964 275d 203d 2073 656c 662e  UserId'] = self.
-00029610: 6275 7369 6e65 7373 5f75 7365 725f 6964  business_user_id
-00029620: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00029630: 2e63 616c 6c65 7220 6973 206e 6f74 204e  .caller is not N
-00029640: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00029650: 2072 6573 756c 745b 2743 616c 6c65 7227   result['Caller'
-00029660: 5d20 3d20 7365 6c66 2e63 616c 6c65 720a  ] = self.caller.
-00029670: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00029680: 6469 7370 6c61 795f 6e61 6d65 2069 7320  display_name is 
-00029690: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-000296a0: 2020 2020 2020 7265 7375 6c74 5b27 4469        result['Di
-000296b0: 7370 6c61 794e 616d 6527 5d20 3d20 7365  splayName'] = se
-000296c0: 6c66 2e64 6973 706c 6179 5f6e 616d 650a  lf.display_name.
-000296d0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000296e0: 656e 645f 7469 6d65 2069 7320 6e6f 7420  end_time is not 
-000296f0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00029700: 2020 7265 7375 6c74 5b27 456e 6454 696d    result['EndTim
-00029710: 6527 5d20 3d20 7365 6c66 2e65 6e64 5f74  e'] = self.end_t
-00029720: 696d 650a 2020 2020 2020 2020 6966 2073  ime.        if s
-00029730: 656c 662e 6672 6f6d 5f61 6c6c 5f77 6f72  elf.from_all_wor
-00029740: 6b73 7061 6365 7320 6973 206e 6f74 204e  kspaces is not N
-00029750: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00029760: 2072 6573 756c 745b 2746 726f 6d41 6c6c   result['FromAll
-00029770: 576f 726b 7370 6163 6573 275d 203d 2073  Workspaces'] = s
-00029780: 656c 662e 6672 6f6d 5f61 6c6c 5f77 6f72  elf.from_all_wor
-00029790: 6b73 7061 6365 730a 2020 2020 2020 2020  kspaces.        
-000297a0: 6966 2073 656c 662e 6a6f 625f 6964 2069  if self.job_id i
-000297b0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000297c0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-000297d0: 4a6f 6249 6427 5d20 3d20 7365 6c66 2e6a  JobId'] = self.j
-000297e0: 6f62 5f69 640a 2020 2020 2020 2020 6966  ob_id.        if
-000297f0: 2073 656c 662e 6a6f 625f 7479 7065 2069   self.job_type i
-00029800: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00029810: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-00029820: 4a6f 6254 7970 6527 5d20 3d20 7365 6c66  JobType'] = self
-00029830: 2e6a 6f62 5f74 7970 650a 2020 2020 2020  .job_type.      
-00029840: 2020 6966 2073 656c 662e 6f72 6465 7220    if self.order 
-00029850: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00029860: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-00029870: 274f 7264 6572 275d 203d 2073 656c 662e  'Order'] = self.
-00029880: 6f72 6465 720a 2020 2020 2020 2020 6966  order.        if
-00029890: 2073 656c 662e 7061 6765 5f6e 756d 6265   self.page_numbe
-000298a0: 7220 6973 206e 6f74 204e 6f6e 653a 0a20  r is not None:. 
-000298b0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-000298c0: 745b 2750 6167 654e 756d 6265 7227 5d20  t['PageNumber'] 
-000298d0: 3d20 7365 6c66 2e70 6167 655f 6e75 6d62  = self.page_numb
-000298e0: 6572 0a20 2020 2020 2020 2069 6620 7365  er.        if se
-000298f0: 6c66 2e70 6167 655f 7369 7a65 2069 7320  lf.page_size is 
-00029900: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00029910: 2020 2020 2020 7265 7375 6c74 5b27 5061        result['Pa
-00029920: 6765 5369 7a65 275d 203d 2073 656c 662e  geSize'] = self.
-00029930: 7061 6765 5f73 697a 650a 2020 2020 2020  page_size.      
-00029940: 2020 6966 2073 656c 662e 7069 7065 6c69    if self.pipeli
-00029950: 6e65 5f69 6420 6973 206e 6f74 204e 6f6e  ne_id is not Non
-00029960: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00029970: 6573 756c 745b 2750 6970 656c 696e 6549  esult['PipelineI
-00029980: 6427 5d20 3d20 7365 6c66 2e70 6970 656c  d'] = self.pipel
-00029990: 696e 655f 6964 0a20 2020 2020 2020 2069  ine_id.        i
-000299a0: 6620 7365 6c66 2e72 6573 6f75 7263 655f  f self.resource_
-000299b0: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
-000299c0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-000299d0: 6c74 5b27 5265 736f 7572 6365 4964 275d  lt['ResourceId']
-000299e0: 203d 2073 656c 662e 7265 736f 7572 6365   = self.resource
-000299f0: 5f69 640a 2020 2020 2020 2020 6966 2073  _id.        if s
-00029a00: 656c 662e 7368 6f77 5f6f 776e 2069 7320  elf.show_own is 
-00029a10: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00029a20: 2020 2020 2020 7265 7375 6c74 5b27 5368        result['Sh
-00029a30: 6f77 4f77 6e27 5d20 3d20 7365 6c66 2e73  owOwn'] = self.s
-00029a40: 686f 775f 6f77 6e0a 2020 2020 2020 2020  how_own.        
-00029a50: 6966 2073 656c 662e 736f 7274 5f62 7920  if self.sort_by 
-00029a60: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00029a70: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-00029a80: 2753 6f72 7442 7927 5d20 3d20 7365 6c66  'SortBy'] = self
-00029a90: 2e73 6f72 745f 6279 0a20 2020 2020 2020  .sort_by.       
-00029aa0: 2069 6620 7365 6c66 2e73 7461 7274 5f74   if self.start_t
-00029ab0: 696d 6520 6973 206e 6f74 204e 6f6e 653a  ime is not None:
-00029ac0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00029ad0: 756c 745b 2753 7461 7274 5469 6d65 275d  ult['StartTime']
-00029ae0: 203d 2073 656c 662e 7374 6172 745f 7469   = self.start_ti
-00029af0: 6d65 0a20 2020 2020 2020 2069 6620 7365  me.        if se
-00029b00: 6c66 2e73 7461 7475 7320 6973 206e 6f74  lf.status is not
-00029b10: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00029b20: 2020 2072 6573 756c 745b 2753 7461 7475     result['Statu
-00029b30: 7327 5d20 3d20 7365 6c66 2e73 7461 7475  s'] = self.statu
-00029b40: 730a 2020 2020 2020 2020 6966 2073 656c  s.        if sel
-00029b50: 662e 7461 6773 5f73 6872 696e 6b20 6973  f.tags_shrink is
-00029b60: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00029b70: 2020 2020 2020 2072 6573 756c 745b 2754         result['T
-00029b80: 6167 7327 5d20 3d20 7365 6c66 2e74 6167  ags'] = self.tag
-00029b90: 735f 7368 7269 6e6b 0a20 2020 2020 2020  s_shrink.       
-00029ba0: 2069 6620 7365 6c66 2e77 6f72 6b73 7061   if self.workspa
-00029bb0: 6365 5f69 6420 6973 206e 6f74 204e 6f6e  ce_id is not Non
-00029bc0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00029bd0: 6573 756c 745b 2757 6f72 6b73 7061 6365  esult['Workspace
-00029be0: 4964 275d 203d 2073 656c 662e 776f 726b  Id'] = self.work
-00029bf0: 7370 6163 655f 6964 0a20 2020 2020 2020  space_id.       
-00029c00: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
-00029c10: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
-00029c20: 2873 656c 662c 206d 3d4e 6f6e 6529 3a0a  (self, m=None):.
-00029c30: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
-00029c40: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-00029c50: 6966 206d 2e67 6574 2827 4275 7369 6e65  if m.get('Busine
-00029c60: 7373 5573 6572 4964 2729 2069 7320 6e6f  ssUserId') is no
-00029c70: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00029c80: 2020 2020 7365 6c66 2e62 7573 696e 6573      self.busines
-00029c90: 735f 7573 6572 5f69 6420 3d20 6d2e 6765  s_user_id = m.ge
-00029ca0: 7428 2742 7573 696e 6573 7355 7365 7249  t('BusinessUserI
-00029cb0: 6427 290a 2020 2020 2020 2020 6966 206d  d').        if m
-00029cc0: 2e67 6574 2827 4361 6c6c 6572 2729 2069  .get('Caller') i
-00029cd0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00029ce0: 2020 2020 2020 2020 7365 6c66 2e63 616c          self.cal
-00029cf0: 6c65 7220 3d20 6d2e 6765 7428 2743 616c  ler = m.get('Cal
-00029d00: 6c65 7227 290a 2020 2020 2020 2020 6966  ler').        if
-00029d10: 206d 2e67 6574 2827 4469 7370 6c61 794e   m.get('DisplayN
-00029d20: 616d 6527 2920 6973 206e 6f74 204e 6f6e  ame') is not Non
-00029d30: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00029d40: 656c 662e 6469 7370 6c61 795f 6e61 6d65  elf.display_name
-00029d50: 203d 206d 2e67 6574 2827 4469 7370 6c61   = m.get('Displa
-00029d60: 794e 616d 6527 290a 2020 2020 2020 2020  yName').        
-00029d70: 6966 206d 2e67 6574 2827 456e 6454 696d  if m.get('EndTim
-00029d80: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
-00029d90: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00029da0: 662e 656e 645f 7469 6d65 203d 206d 2e67  f.end_time = m.g
-00029db0: 6574 2827 456e 6454 696d 6527 290a 2020  et('EndTime').  
-00029dc0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-00029dd0: 4672 6f6d 416c 6c57 6f72 6b73 7061 6365  FromAllWorkspace
-00029de0: 7327 2920 6973 206e 6f74 204e 6f6e 653a  s') is not None:
-00029df0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00029e00: 662e 6672 6f6d 5f61 6c6c 5f77 6f72 6b73  f.from_all_works
-00029e10: 7061 6365 7320 3d20 6d2e 6765 7428 2746  paces = m.get('F
-00029e20: 726f 6d41 6c6c 576f 726b 7370 6163 6573  romAllWorkspaces
-00029e30: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-00029e40: 6765 7428 274a 6f62 4964 2729 2069 7320  get('JobId') is 
-00029e50: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00029e60: 2020 2020 2020 7365 6c66 2e6a 6f62 5f69        self.job_i
-00029e70: 6420 3d20 6d2e 6765 7428 274a 6f62 4964  d = m.get('JobId
-00029e80: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-00029e90: 6765 7428 274a 6f62 5479 7065 2729 2069  get('JobType') i
-00029ea0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00029eb0: 2020 2020 2020 2020 7365 6c66 2e6a 6f62          self.job
-00029ec0: 5f74 7970 6520 3d20 6d2e 6765 7428 274a  _type = m.get('J
-00029ed0: 6f62 5479 7065 2729 0a20 2020 2020 2020  obType').       
-00029ee0: 2069 6620 6d2e 6765 7428 274f 7264 6572   if m.get('Order
-00029ef0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-00029f00: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00029f10: 2e6f 7264 6572 203d 206d 2e67 6574 2827  .order = m.get('
-00029f20: 4f72 6465 7227 290a 2020 2020 2020 2020  Order').        
-00029f30: 6966 206d 2e67 6574 2827 5061 6765 4e75  if m.get('PageNu
-00029f40: 6d62 6572 2729 2069 7320 6e6f 7420 4e6f  mber') is not No
-00029f50: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00029f60: 7365 6c66 2e70 6167 655f 6e75 6d62 6572  self.page_number
-00029f70: 203d 206d 2e67 6574 2827 5061 6765 4e75   = m.get('PageNu
-00029f80: 6d62 6572 2729 0a20 2020 2020 2020 2069  mber').        i
-00029f90: 6620 6d2e 6765 7428 2750 6167 6553 697a  f m.get('PageSiz
-00029fa0: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
-00029fb0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00029fc0: 662e 7061 6765 5f73 697a 6520 3d20 6d2e  f.page_size = m.
-00029fd0: 6765 7428 2750 6167 6553 697a 6527 290a  get('PageSize').
-00029fe0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-00029ff0: 2827 5069 7065 6c69 6e65 4964 2729 2069  ('PipelineId') i
-0002a000: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0002a010: 2020 2020 2020 2020 7365 6c66 2e70 6970          self.pip
-0002a020: 656c 696e 655f 6964 203d 206d 2e67 6574  eline_id = m.get
-0002a030: 2827 5069 7065 6c69 6e65 4964 2729 0a20  ('PipelineId'). 
-0002a040: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-0002a050: 2752 6573 6f75 7263 6549 6427 2920 6973  'ResourceId') is
-0002a060: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0002a070: 2020 2020 2020 2073 656c 662e 7265 736f         self.reso
-0002a080: 7572 6365 5f69 6420 3d20 6d2e 6765 7428  urce_id = m.get(
-0002a090: 2752 6573 6f75 7263 6549 6427 290a 2020  'ResourceId').  
-0002a0a0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-0002a0b0: 5368 6f77 4f77 6e27 2920 6973 206e 6f74  ShowOwn') is not
-0002a0c0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0002a0d0: 2020 2073 656c 662e 7368 6f77 5f6f 776e     self.show_own
-0002a0e0: 203d 206d 2e67 6574 2827 5368 6f77 4f77   = m.get('ShowOw
-0002a0f0: 6e27 290a 2020 2020 2020 2020 6966 206d  n').        if m
-0002a100: 2e67 6574 2827 536f 7274 4279 2729 2069  .get('SortBy') i
-0002a110: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0002a120: 2020 2020 2020 2020 7365 6c66 2e73 6f72          self.sor
-0002a130: 745f 6279 203d 206d 2e67 6574 2827 536f  t_by = m.get('So
-0002a140: 7274 4279 2729 0a20 2020 2020 2020 2069  rtBy').        i
-0002a150: 6620 6d2e 6765 7428 2753 7461 7274 5469  f m.get('StartTi
-0002a160: 6d65 2729 2069 7320 6e6f 7420 4e6f 6e65  me') is not None
-0002a170: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0002a180: 6c66 2e73 7461 7274 5f74 696d 6520 3d20  lf.start_time = 
-0002a190: 6d2e 6765 7428 2753 7461 7274 5469 6d65  m.get('StartTime
-0002a1a0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-0002a1b0: 6765 7428 2753 7461 7475 7327 2920 6973  get('Status') is
-0002a1c0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0002a1d0: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
-0002a1e0: 7573 203d 206d 2e67 6574 2827 5374 6174  us = m.get('Stat
-0002a1f0: 7573 2729 0a20 2020 2020 2020 2069 6620  us').        if 
-0002a200: 6d2e 6765 7428 2754 6167 7327 2920 6973  m.get('Tags') is
-0002a210: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0002a220: 2020 2020 2020 2073 656c 662e 7461 6773         self.tags
-0002a230: 5f73 6872 696e 6b20 3d20 6d2e 6765 7428  _shrink = m.get(
-0002a240: 2754 6167 7327 290a 2020 2020 2020 2020  'Tags').        
-0002a250: 6966 206d 2e67 6574 2827 576f 726b 7370  if m.get('Worksp
-0002a260: 6163 6549 6427 2920 6973 206e 6f74 204e  aceId') is not N
-0002a270: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0002a280: 2073 656c 662e 776f 726b 7370 6163 655f   self.workspace_
-0002a290: 6964 203d 206d 2e67 6574 2827 576f 726b  id = m.get('Work
-0002a2a0: 7370 6163 6549 6427 290a 2020 2020 2020  spaceId').      
-0002a2b0: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
-0002a2c0: 636c 6173 7320 4c69 7374 4a6f 6273 5265  class ListJobsRe
-0002a2d0: 7370 6f6e 7365 426f 6479 2854 6561 4d6f  sponseBody(TeaMo
-0002a2e0: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
-0002a2f0: 696e 6974 5f5f 2873 656c 662c 206a 6f62  init__(self, job
-0002a300: 733d 4e6f 6e65 2c20 7265 7175 6573 745f  s=None, request_
-0002a310: 6964 3d4e 6f6e 652c 2074 6f74 616c 5f63  id=None, total_c
-0002a320: 6f75 6e74 3d4e 6f6e 6529 3a0a 2020 2020  ount=None):.    
-0002a330: 2020 2020 7365 6c66 2e6a 6f62 7320 3d20      self.jobs = 
-0002a340: 6a6f 6273 2020 2320 7479 7065 3a20 6c69  jobs  # type: li
-0002a350: 7374 5b4a 6f62 4974 656d 5d0a 2020 2020  st[JobItem].    
-0002a360: 2020 2020 7365 6c66 2e72 6571 7565 7374      self.request
-0002a370: 5f69 6420 3d20 7265 7175 6573 745f 6964  _id = request_id
-0002a380: 2020 2320 7479 7065 3a20 7374 720a 2020    # type: str.  
-0002a390: 2020 2020 2020 7365 6c66 2e74 6f74 616c        self.total
-0002a3a0: 5f63 6f75 6e74 203d 2074 6f74 616c 5f63  _count = total_c
-0002a3b0: 6f75 6e74 2020 2320 7479 7065 3a20 6c6f  ount  # type: lo
-0002a3c0: 6e67 0a0a 2020 2020 6465 6620 7661 6c69  ng..    def vali
-0002a3d0: 6461 7465 2873 656c 6629 3a0a 2020 2020  date(self):.    
-0002a3e0: 2020 2020 6966 2073 656c 662e 6a6f 6273      if self.jobs
-0002a3f0: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
-0002a400: 7220 6b20 696e 2073 656c 662e 6a6f 6273  r k in self.jobs
-0002a410: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0002a420: 2020 6966 206b 3a0a 2020 2020 2020 2020    if k:.        
-0002a430: 2020 2020 2020 2020 2020 2020 6b2e 7661              k.va
-0002a440: 6c69 6461 7465 2829 0a0a 2020 2020 6465  lidate()..    de
-0002a450: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
-0002a460: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
-0002a470: 7570 6572 284c 6973 744a 6f62 7352 6573  uper(ListJobsRes
-0002a480: 706f 6e73 6542 6f64 792c 2073 656c 6629  ponseBody, self)
-0002a490: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
-0002a4a0: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
-0002a4b0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0002a4c0: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
-0002a4d0: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
-0002a4e0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-0002a4f0: 7265 7375 6c74 5b27 4a6f 6273 275d 203d  result['Jobs'] =
-0002a500: 205b 5d0a 2020 2020 2020 2020 6966 2073   [].        if s
-0002a510: 656c 662e 6a6f 6273 2069 7320 6e6f 7420  elf.jobs is not 
-0002a520: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0002a530: 2020 666f 7220 6b20 696e 2073 656c 662e    for k in self.
-0002a540: 6a6f 6273 3a0a 2020 2020 2020 2020 2020  jobs:.          
-0002a550: 2020 2020 2020 7265 7375 6c74 5b27 4a6f        result['Jo
-0002a560: 6273 275d 2e61 7070 656e 6428 6b2e 746f  bs'].append(k.to
-0002a570: 5f6d 6170 2829 2069 6620 6b20 656c 7365  _map() if k else
-0002a580: 204e 6f6e 6529 0a20 2020 2020 2020 2069   None).        i
-0002a590: 6620 7365 6c66 2e72 6571 7565 7374 5f69  f self.request_i
-0002a5a0: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
-0002a5b0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-0002a5c0: 745b 2752 6571 7565 7374 4964 275d 203d  t['RequestId'] =
-0002a5d0: 2073 656c 662e 7265 7175 6573 745f 6964   self.request_id
-0002a5e0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0002a5f0: 2e74 6f74 616c 5f63 6f75 6e74 2069 7320  .total_count is 
-0002a600: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0002a610: 2020 2020 2020 7265 7375 6c74 5b27 546f        result['To
-0002a620: 7461 6c43 6f75 6e74 275d 203d 2073 656c  talCount'] = sel
-0002a630: 662e 746f 7461 6c5f 636f 756e 740a 2020  f.total_count.  
-0002a640: 2020 2020 2020 7265 7475 726e 2072 6573        return res
-0002a650: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
-0002a660: 6d5f 6d61 7028 7365 6c66 2c20 6d3d 4e6f  m_map(self, m=No
-0002a670: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
-0002a680: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
-0002a690: 2020 2020 2073 656c 662e 6a6f 6273 203d       self.jobs =
-0002a6a0: 205b 5d0a 2020 2020 2020 2020 6966 206d   [].        if m
-0002a6b0: 2e67 6574 2827 4a6f 6273 2729 2069 7320  .get('Jobs') is 
-0002a6c0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0002a6d0: 2020 2020 2020 666f 7220 6b20 696e 206d        for k in m
-0002a6e0: 2e67 6574 2827 4a6f 6273 2729 3a0a 2020  .get('Jobs'):.  
-0002a6f0: 2020 2020 2020 2020 2020 2020 2020 7465                te
-0002a700: 6d70 5f6d 6f64 656c 203d 204a 6f62 4974  mp_model = JobIt
-0002a710: 656d 2829 0a20 2020 2020 2020 2020 2020  em().           
-0002a720: 2020 2020 2073 656c 662e 6a6f 6273 2e61       self.jobs.a
-0002a730: 7070 656e 6428 7465 6d70 5f6d 6f64 656c  ppend(temp_model
-0002a740: 2e66 726f 6d5f 6d61 7028 6b29 290a 2020  .from_map(k)).  
-0002a750: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-0002a760: 5265 7175 6573 7449 6427 2920 6973 206e  RequestId') is n
-0002a770: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0002a780: 2020 2020 2073 656c 662e 7265 7175 6573       self.reques
-0002a790: 745f 6964 203d 206d 2e67 6574 2827 5265  t_id = m.get('Re
-0002a7a0: 7175 6573 7449 6427 290a 2020 2020 2020  questId').      
-0002a7b0: 2020 6966 206d 2e67 6574 2827 546f 7461    if m.get('Tota
-0002a7c0: 6c43 6f75 6e74 2729 2069 7320 6e6f 7420  lCount') is not 
-0002a7d0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0002a7e0: 2020 7365 6c66 2e74 6f74 616c 5f63 6f75    self.total_cou
-0002a7f0: 6e74 203d 206d 2e67 6574 2827 546f 7461  nt = m.get('Tota
-0002a800: 6c43 6f75 6e74 2729 0a20 2020 2020 2020  lCount').       
-0002a810: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
-0002a820: 6c61 7373 204c 6973 744a 6f62 7352 6573  lass ListJobsRes
-0002a830: 706f 6e73 6528 5465 614d 6f64 656c 293a  ponse(TeaModel):
-0002a840: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-0002a850: 5f28 7365 6c66 2c20 6865 6164 6572 733d  _(self, headers=
-0002a860: 4e6f 6e65 2c20 7374 6174 7573 5f63 6f64  None, status_cod
-0002a870: 653d 4e6f 6e65 2c20 626f 6479 3d4e 6f6e  e=None, body=Non
-0002a880: 6529 3a0a 2020 2020 2020 2020 7365 6c66  e):.        self
-0002a890: 2e68 6561 6465 7273 203d 2068 6561 6465  .headers = heade
-0002a8a0: 7273 2020 2320 7479 7065 3a20 6469 6374  rs  # type: dict
-0002a8b0: 5b73 7472 2c20 7374 725d 0a20 2020 2020  [str, str].     
-0002a8c0: 2020 2073 656c 662e 7374 6174 7573 5f63     self.status_c
-0002a8d0: 6f64 6520 3d20 7374 6174 7573 5f63 6f64  ode = status_cod
-0002a8e0: 6520 2023 2074 7970 653a 2069 6e74 0a20  e  # type: int. 
-0002a8f0: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
-0002a900: 203d 2062 6f64 7920 2023 2074 7970 653a   = body  # type:
-0002a910: 204c 6973 744a 6f62 7352 6573 706f 6e73   ListJobsRespons
-0002a920: 6542 6f64 790a 0a20 2020 2064 6566 2076  eBody..    def v
-0002a930: 616c 6964 6174 6528 7365 6c66 293a 0a20  alidate(self):. 
-0002a940: 2020 2020 2020 2073 656c 662e 7661 6c69         self.vali
-0002a950: 6461 7465 5f72 6571 7569 7265 6428 7365  date_required(se
-0002a960: 6c66 2e68 6561 6465 7273 2c20 2768 6561  lf.headers, 'hea
-0002a970: 6465 7273 2729 0a20 2020 2020 2020 2073  ders').        s
-0002a980: 656c 662e 7661 6c69 6461 7465 5f72 6571  elf.validate_req
-0002a990: 7569 7265 6428 7365 6c66 2e73 7461 7475  uired(self.statu
-0002a9a0: 735f 636f 6465 2c20 2773 7461 7475 735f  s_code, 'status_
-0002a9b0: 636f 6465 2729 0a20 2020 2020 2020 2073  code').        s
-0002a9c0: 656c 662e 7661 6c69 6461 7465 5f72 6571  elf.validate_req
-0002a9d0: 7569 7265 6428 7365 6c66 2e62 6f64 792c  uired(self.body,
-0002a9e0: 2027 626f 6479 2729 0a20 2020 2020 2020   'body').       
-0002a9f0: 2069 6620 7365 6c66 2e62 6f64 793a 0a20   if self.body:. 
-0002aa00: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0002aa10: 626f 6479 2e76 616c 6964 6174 6528 290a  body.validate().
-0002aa20: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
-0002aa30: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
-0002aa40: 6d61 7020 3d20 7375 7065 7228 4c69 7374  map = super(List
-0002aa50: 4a6f 6273 5265 7370 6f6e 7365 2c20 7365  JobsResponse, se
-0002aa60: 6c66 292e 746f 5f6d 6170 2829 0a20 2020  lf).to_map().   
-0002aa70: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
-0002aa80: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0002aa90: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
-0002aaa0: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
-0002aab0: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
-0002aac0: 2020 2069 6620 7365 6c66 2e68 6561 6465     if self.heade
-0002aad0: 7273 2069 7320 6e6f 7420 4e6f 6e65 3a0a  rs is not None:.
-0002aae0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-0002aaf0: 6c74 5b27 6865 6164 6572 7327 5d20 3d20  lt['headers'] = 
-0002ab00: 7365 6c66 2e68 6561 6465 7273 0a20 2020  self.headers.   
-0002ab10: 2020 2020 2069 6620 7365 6c66 2e73 7461       if self.sta
-0002ab20: 7475 735f 636f 6465 2069 7320 6e6f 7420  tus_code is not 
-0002ab30: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0002ab40: 2020 7265 7375 6c74 5b27 7374 6174 7573    result['status
-0002ab50: 436f 6465 275d 203d 2073 656c 662e 7374  Code'] = self.st
-0002ab60: 6174 7573 5f63 6f64 650a 2020 2020 2020  atus_code.      
-0002ab70: 2020 6966 2073 656c 662e 626f 6479 2069    if self.body i
-0002ab80: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0002ab90: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-0002aba0: 626f 6479 275d 203d 2073 656c 662e 626f  body'] = self.bo
-0002abb0: 6479 2e74 6f5f 6d61 7028 290a 2020 2020  dy.to_map().    
-0002abc0: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
-0002abd0: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
-0002abe0: 6d61 7028 7365 6c66 2c20 6d3d 4e6f 6e65  map(self, m=None
-0002abf0: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
-0002ac00: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
-0002ac10: 2020 2069 6620 6d2e 6765 7428 2768 6561     if m.get('hea
-0002ac20: 6465 7273 2729 2069 7320 6e6f 7420 4e6f  ders') is not No
-0002ac30: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0002ac40: 7365 6c66 2e68 6561 6465 7273 203d 206d  self.headers = m
-0002ac50: 2e67 6574 2827 6865 6164 6572 7327 290a  .get('headers').
-0002ac60: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-0002ac70: 2827 7374 6174 7573 436f 6465 2729 2069  ('statusCode') i
-0002ac80: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0002ac90: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
-0002aca0: 7475 735f 636f 6465 203d 206d 2e67 6574  tus_code = m.get
-0002acb0: 2827 7374 6174 7573 436f 6465 2729 0a20  ('statusCode'). 
-0002acc0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-0002acd0: 2762 6f64 7927 2920 6973 206e 6f74 204e  'body') is not N
-0002ace0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0002acf0: 2074 656d 705f 6d6f 6465 6c20 3d20 4c69   temp_model = Li
-0002ad00: 7374 4a6f 6273 5265 7370 6f6e 7365 426f  stJobsResponseBo
-0002ad10: 6479 2829 0a20 2020 2020 2020 2020 2020  dy().           
-0002ad20: 2073 656c 662e 626f 6479 203d 2074 656d   self.body = tem
-0002ad30: 705f 6d6f 6465 6c2e 6672 6f6d 5f6d 6170  p_model.from_map
-0002ad40: 286d 5b27 626f 6479 275d 290a 2020 2020  (m['body']).    
-0002ad50: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
-0002ad60: 0a0a 636c 6173 7320 4c69 7374 5465 6e73  ..class ListTens
-0002ad70: 6f72 626f 6172 6473 5265 7175 6573 7428  orboardsRequest(
-0002ad80: 5465 614d 6f64 656c 293a 0a20 2020 2064  TeaModel):.    d
-0002ad90: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-0002ada0: 2c20 6469 7370 6c61 795f 6e61 6d65 3d4e  , display_name=N
-0002adb0: 6f6e 652c 2065 6e64 5f74 696d 653d 4e6f  one, end_time=No
-0002adc0: 6e65 2c20 6a6f 625f 6964 3d4e 6f6e 652c  ne, job_id=None,
-0002add0: 206f 7264 6572 3d4e 6f6e 652c 2070 6167   order=None, pag
-0002ade0: 655f 6e75 6d62 6572 3d4e 6f6e 652c 2070  e_number=None, p
-0002adf0: 6167 655f 7369 7a65 3d4e 6f6e 652c 0a20  age_size=None,. 
-0002ae00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002ae10: 736f 7274 5f62 793d 4e6f 6e65 2c20 736f  sort_by=None, so
-0002ae20: 7572 6365 5f69 643d 4e6f 6e65 2c20 736f  urce_id=None, so
-0002ae30: 7572 6365 5f74 7970 653d 4e6f 6e65 2c20  urce_type=None, 
-0002ae40: 7374 6172 745f 7469 6d65 3d4e 6f6e 652c  start_time=None,
-0002ae50: 2073 7461 7475 733d 4e6f 6e65 2c20 7465   status=None, te
-0002ae60: 6e73 6f72 626f 6172 645f 6964 3d4e 6f6e  nsorboard_id=Non
-0002ae70: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-0002ae80: 2020 2020 7665 7262 6f73 653d 4e6f 6e65      verbose=None
-0002ae90: 2c20 776f 726b 7370 6163 655f 6964 3d4e  , workspace_id=N
-0002aea0: 6f6e 6529 3a0a 2020 2020 2020 2020 7365  one):.        se
-0002aeb0: 6c66 2e64 6973 706c 6179 5f6e 616d 6520  lf.display_name 
-0002aec0: 3d20 6469 7370 6c61 795f 6e61 6d65 2020  = display_name  
-0002aed0: 2320 7479 7065 3a20 7374 720a 2020 2020  # type: str.    
-0002aee0: 2020 2020 7365 6c66 2e65 6e64 5f74 696d      self.end_tim
-0002aef0: 6520 3d20 656e 645f 7469 6d65 2020 2320  e = end_time  # 
-0002af00: 7479 7065 3a20 7374 720a 2020 2020 2020  type: str.      
-0002af10: 2020 7365 6c66 2e6a 6f62 5f69 6420 3d20    self.job_id = 
-0002af20: 6a6f 625f 6964 2020 2320 7479 7065 3a20  job_id  # type: 
-0002af30: 7374 720a 2020 2020 2020 2020 7365 6c66  str.        self
-0002af40: 2e6f 7264 6572 203d 206f 7264 6572 2020  .order = order  
-0002af50: 2320 7479 7065 3a20 7374 720a 2020 2020  # type: str.    
-0002af60: 2020 2020 7365 6c66 2e70 6167 655f 6e75      self.page_nu
-0002af70: 6d62 6572 203d 2070 6167 655f 6e75 6d62  mber = page_numb
-0002af80: 6572 2020 2320 7479 7065 3a20 696e 740a  er  # type: int.
-0002af90: 2020 2020 2020 2020 7365 6c66 2e70 6167          self.pag
-0002afa0: 655f 7369 7a65 203d 2070 6167 655f 7369  e_size = page_si
-0002afb0: 7a65 2020 2320 7479 7065 3a20 696e 740a  ze  # type: int.
-0002afc0: 2020 2020 2020 2020 7365 6c66 2e73 6f72          self.sor
-0002afd0: 745f 6279 203d 2073 6f72 745f 6279 2020  t_by = sort_by  
-0002afe0: 2320 7479 7065 3a20 7374 720a 2020 2020  # type: str.    
-0002aff0: 2020 2020 7365 6c66 2e73 6f75 7263 655f      self.source_
-0002b000: 6964 203d 2073 6f75 7263 655f 6964 2020  id = source_id  
-0002b010: 2320 7479 7065 3a20 7374 720a 2020 2020  # type: str.    
-0002b020: 2020 2020 7365 6c66 2e73 6f75 7263 655f      self.source_
-0002b030: 7479 7065 203d 2073 6f75 7263 655f 7479  type = source_ty
-0002b040: 7065 2020 2320 7479 7065 3a20 7374 720a  pe  # type: str.
-0002b050: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
-0002b060: 7274 5f74 696d 6520 3d20 7374 6172 745f  rt_time = start_
-0002b070: 7469 6d65 2020 2320 7479 7065 3a20 7374  time  # type: st
-0002b080: 720a 2020 2020 2020 2020 7365 6c66 2e73  r.        self.s
-0002b090: 7461 7475 7320 3d20 7374 6174 7573 2020  tatus = status  
-0002b0a0: 2320 7479 7065 3a20 7374 720a 2020 2020  # type: str.    
-0002b0b0: 2020 2020 7365 6c66 2e74 656e 736f 7262      self.tensorb
-0002b0c0: 6f61 7264 5f69 6420 3d20 7465 6e73 6f72  oard_id = tensor
-0002b0d0: 626f 6172 645f 6964 2020 2320 7479 7065  board_id  # type
-0002b0e0: 3a20 7374 720a 2020 2020 2020 2020 7365  : str.        se
-0002b0f0: 6c66 2e76 6572 626f 7365 203d 2076 6572  lf.verbose = ver
-0002b100: 626f 7365 2020 2320 7479 7065 3a20 626f  bose  # type: bo
-0002b110: 6f6c 0a20 2020 2020 2020 2073 656c 662e  ol.        self.
-0002b120: 776f 726b 7370 6163 655f 6964 203d 2077  workspace_id = w
-0002b130: 6f72 6b73 7061 6365 5f69 6420 2023 2074  orkspace_id  # t
-0002b140: 7970 653a 2073 7472 0a0a 2020 2020 6465  ype: str..    de
-0002b150: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
-0002b160: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
-0002b170: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
-0002b180: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
-0002b190: 6170 203d 2073 7570 6572 284c 6973 7454  ap = super(ListT
-0002b1a0: 656e 736f 7262 6f61 7264 7352 6571 7565  ensorboardsReque
-0002b1b0: 7374 2c20 7365 6c66 292e 746f 5f6d 6170  st, self).to_map
-0002b1c0: 2829 0a20 2020 2020 2020 2069 6620 5f6d  ().        if _m
-0002b1d0: 6170 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ap is not None:.
-0002b1e0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0002b1f0: 726e 205f 6d61 700a 0a20 2020 2020 2020  rn _map..       
-0002b200: 2072 6573 756c 7420 3d20 6469 6374 2829   result = dict()
-0002b210: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0002b220: 2e64 6973 706c 6179 5f6e 616d 6520 6973  .display_name is
-0002b230: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0002b240: 2020 2020 2020 2072 6573 756c 745b 2744         result['D
-0002b250: 6973 706c 6179 4e61 6d65 275d 203d 2073  isplayName'] = s
-0002b260: 656c 662e 6469 7370 6c61 795f 6e61 6d65  elf.display_name
-0002b270: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0002b280: 2e65 6e64 5f74 696d 6520 6973 206e 6f74  .end_time is not
-0002b290: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0002b2a0: 2020 2072 6573 756c 745b 2745 6e64 5469     result['EndTi
-0002b2b0: 6d65 275d 203d 2073 656c 662e 656e 645f  me'] = self.end_
-0002b2c0: 7469 6d65 0a20 2020 2020 2020 2069 6620  time.        if 
-0002b2d0: 7365 6c66 2e6a 6f62 5f69 6420 6973 206e  self.job_id is n
-0002b2e0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0002b2f0: 2020 2020 2072 6573 756c 745b 274a 6f62       result['Job
-0002b300: 4964 275d 203d 2073 656c 662e 6a6f 625f  Id'] = self.job_
-0002b310: 6964 0a20 2020 2020 2020 2069 6620 7365  id.        if se
-0002b320: 6c66 2e6f 7264 6572 2069 7320 6e6f 7420  lf.order is not 
-0002b330: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0002b340: 2020 7265 7375 6c74 5b27 4f72 6465 7227    result['Order'
-0002b350: 5d20 3d20 7365 6c66 2e6f 7264 6572 0a20  ] = self.order. 
-0002b360: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
-0002b370: 6167 655f 6e75 6d62 6572 2069 7320 6e6f  age_number is no
-0002b380: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0002b390: 2020 2020 7265 7375 6c74 5b27 5061 6765      result['Page
-0002b3a0: 4e75 6d62 6572 275d 203d 2073 656c 662e  Number'] = self.
-0002b3b0: 7061 6765 5f6e 756d 6265 720a 2020 2020  page_number.    
-0002b3c0: 2020 2020 6966 2073 656c 662e 7061 6765      if self.page
-0002b3d0: 5f73 697a 6520 6973 206e 6f74 204e 6f6e  _size is not Non
-0002b3e0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-0002b3f0: 6573 756c 745b 2750 6167 6553 697a 6527  esult['PageSize'
-0002b400: 5d20 3d20 7365 6c66 2e70 6167 655f 7369  ] = self.page_si
-0002b410: 7a65 0a20 2020 2020 2020 2069 6620 7365  ze.        if se
-0002b420: 6c66 2e73 6f72 745f 6279 2069 7320 6e6f  lf.sort_by is no
-0002b430: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0002b440: 2020 2020 7265 7375 6c74 5b27 536f 7274      result['Sort
-0002b450: 4279 275d 203d 2073 656c 662e 736f 7274  By'] = self.sort
-0002b460: 5f62 790a 2020 2020 2020 2020 6966 2073  _by.        if s
-0002b470: 656c 662e 736f 7572 6365 5f69 6420 6973  elf.source_id is
-0002b480: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0002b490: 2020 2020 2020 2072 6573 756c 745b 2753         result['S
-0002b4a0: 6f75 7263 6549 6427 5d20 3d20 7365 6c66  ourceId'] = self
-0002b4b0: 2e73 6f75 7263 655f 6964 0a20 2020 2020  .source_id.     
-0002b4c0: 2020 2069 6620 7365 6c66 2e73 6f75 7263     if self.sourc
-0002b4d0: 655f 7479 7065 2069 7320 6e6f 7420 4e6f  e_type is not No
-0002b4e0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0002b4f0: 7265 7375 6c74 5b27 536f 7572 6365 5479  result['SourceTy
-0002b500: 7065 275d 203d 2073 656c 662e 736f 7572  pe'] = self.sour
-0002b510: 6365 5f74 7970 650a 2020 2020 2020 2020  ce_type.        
-0002b520: 6966 2073 656c 662e 7374 6172 745f 7469  if self.start_ti
-0002b530: 6d65 2069 7320 6e6f 7420 4e6f 6e65 3a0a  me is not None:.
-0002b540: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-0002b550: 6c74 5b27 5374 6172 7454 696d 6527 5d20  lt['StartTime'] 
-0002b560: 3d20 7365 6c66 2e73 7461 7274 5f74 696d  = self.start_tim
-0002b570: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
-0002b580: 662e 7374 6174 7573 2069 7320 6e6f 7420  f.status is not 
-0002b590: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0002b5a0: 2020 7265 7375 6c74 5b27 5374 6174 7573    result['Status
-0002b5b0: 275d 203d 2073 656c 662e 7374 6174 7573  '] = self.status
-0002b5c0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0002b5d0: 2e74 656e 736f 7262 6f61 7264 5f69 6420  .tensorboard_id 
-0002b5e0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0002b5f0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-0002b600: 2754 656e 736f 7262 6f61 7264 4964 275d  'TensorboardId']
-0002b610: 203d 2073 656c 662e 7465 6e73 6f72 626f   = self.tensorbo
-0002b620: 6172 645f 6964 0a20 2020 2020 2020 2069  ard_id.        i
-0002b630: 6620 7365 6c66 2e76 6572 626f 7365 2069  f self.verbose i
-0002b640: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0002b650: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-0002b660: 5665 7262 6f73 6527 5d20 3d20 7365 6c66  Verbose'] = self
-0002b670: 2e76 6572 626f 7365 0a20 2020 2020 2020  .verbose.       
-0002b680: 2069 6620 7365 6c66 2e77 6f72 6b73 7061   if self.workspa
-0002b690: 6365 5f69 6420 6973 206e 6f74 204e 6f6e  ce_id is not Non
-0002b6a0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-0002b6b0: 6573 756c 745b 2757 6f72 6b73 7061 6365  esult['Workspace
-0002b6c0: 4964 275d 203d 2073 656c 662e 776f 726b  Id'] = self.work
-0002b6d0: 7370 6163 655f 6964 0a20 2020 2020 2020  space_id.       
-0002b6e0: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
-0002b6f0: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
-0002b700: 2873 656c 662c 206d 3d4e 6f6e 6529 3a0a  (self, m=None):.
-0002b710: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
-0002b720: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-0002b730: 6966 206d 2e67 6574 2827 4469 7370 6c61  if m.get('Displa
-0002b740: 794e 616d 6527 2920 6973 206e 6f74 204e  yName') is not N
-0002b750: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0002b760: 2073 656c 662e 6469 7370 6c61 795f 6e61   self.display_na
-0002b770: 6d65 203d 206d 2e67 6574 2827 4469 7370  me = m.get('Disp
-0002b780: 6c61 794e 616d 6527 290a 2020 2020 2020  layName').      
-0002b790: 2020 6966 206d 2e67 6574 2827 456e 6454    if m.get('EndT
-0002b7a0: 696d 6527 2920 6973 206e 6f74 204e 6f6e  ime') is not Non
-0002b7b0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-0002b7c0: 656c 662e 656e 645f 7469 6d65 203d 206d  elf.end_time = m
-0002b7d0: 2e67 6574 2827 456e 6454 696d 6527 290a  .get('EndTime').
-0002b7e0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-0002b7f0: 2827 4a6f 6249 6427 2920 6973 206e 6f74  ('JobId') is not
-0002b800: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0002b810: 2020 2073 656c 662e 6a6f 625f 6964 203d     self.job_id =
-0002b820: 206d 2e67 6574 2827 4a6f 6249 6427 290a   m.get('JobId').
-0002b830: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-0002b840: 2827 4f72 6465 7227 2920 6973 206e 6f74  ('Order') is not
-0002b850: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0002b860: 2020 2073 656c 662e 6f72 6465 7220 3d20     self.order = 
-0002b870: 6d2e 6765 7428 274f 7264 6572 2729 0a20  m.get('Order'). 
-0002b880: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-0002b890: 2750 6167 654e 756d 6265 7227 2920 6973  'PageNumber') is
-0002b8a0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0002b8b0: 2020 2020 2020 2073 656c 662e 7061 6765         self.page
-0002b8c0: 5f6e 756d 6265 7220 3d20 6d2e 6765 7428  _number = m.get(
-0002b8d0: 2750 6167 654e 756d 6265 7227 290a 2020  'PageNumber').  
-0002b8e0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-0002b8f0: 5061 6765 5369 7a65 2729 2069 7320 6e6f  PageSize') is no
-0002b900: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0002b910: 2020 2020 7365 6c66 2e70 6167 655f 7369      self.page_si
-0002b920: 7a65 203d 206d 2e67 6574 2827 5061 6765  ze = m.get('Page
-0002b930: 5369 7a65 2729 0a20 2020 2020 2020 2069  Size').        i
-0002b940: 6620 6d2e 6765 7428 2753 6f72 7442 7927  f m.get('SortBy'
-0002b950: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-0002b960: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0002b970: 736f 7274 5f62 7920 3d20 6d2e 6765 7428  sort_by = m.get(
-0002b980: 2753 6f72 7442 7927 290a 2020 2020 2020  'SortBy').      
-0002b990: 2020 6966 206d 2e67 6574 2827 536f 7572    if m.get('Sour
-0002b9a0: 6365 4964 2729 2069 7320 6e6f 7420 4e6f  ceId') is not No
-0002b9b0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0002b9c0: 7365 6c66 2e73 6f75 7263 655f 6964 203d  self.source_id =
-0002b9d0: 206d 2e67 6574 2827 536f 7572 6365 4964   m.get('SourceId
-0002b9e0: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-0002b9f0: 6765 7428 2753 6f75 7263 6554 7970 6527  get('SourceType'
-0002ba00: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-0002ba10: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0002ba20: 736f 7572 6365 5f74 7970 6520 3d20 6d2e  source_type = m.
-0002ba30: 6765 7428 2753 6f75 7263 6554 7970 6527  get('SourceType'
-0002ba40: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-0002ba50: 6574 2827 5374 6172 7454 696d 6527 2920  et('StartTime') 
-0002ba60: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0002ba70: 2020 2020 2020 2020 2073 656c 662e 7374           self.st
-0002ba80: 6172 745f 7469 6d65 203d 206d 2e67 6574  art_time = m.get
-0002ba90: 2827 5374 6172 7454 696d 6527 290a 2020  ('StartTime').  
-0002baa0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-0002bab0: 5374 6174 7573 2729 2069 7320 6e6f 7420  Status') is not 
-0002bac0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0002bad0: 2020 7365 6c66 2e73 7461 7475 7320 3d20    self.status = 
-0002bae0: 6d2e 6765 7428 2753 7461 7475 7327 290a  m.get('Status').
-0002baf0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-0002bb00: 2827 5465 6e73 6f72 626f 6172 6449 6427  ('TensorboardId'
-0002bb10: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-0002bb20: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0002bb30: 7465 6e73 6f72 626f 6172 645f 6964 203d  tensorboard_id =
-0002bb40: 206d 2e67 6574 2827 5465 6e73 6f72 626f   m.get('Tensorbo
-0002bb50: 6172 6449 6427 290a 2020 2020 2020 2020  ardId').        
-0002bb60: 6966 206d 2e67 6574 2827 5665 7262 6f73  if m.get('Verbos
-0002bb70: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
-0002bb80: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0002bb90: 662e 7665 7262 6f73 6520 3d20 6d2e 6765  f.verbose = m.ge
-0002bba0: 7428 2756 6572 626f 7365 2729 0a20 2020  t('Verbose').   
-0002bbb0: 2020 2020 2069 6620 6d2e 6765 7428 2757       if m.get('W
-0002bbc0: 6f72 6b73 7061 6365 4964 2729 2069 7320  orkspaceId') is 
-0002bbd0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0002bbe0: 2020 2020 2020 7365 6c66 2e77 6f72 6b73        self.works
-0002bbf0: 7061 6365 5f69 6420 3d20 6d2e 6765 7428  pace_id = m.get(
-0002bc00: 2757 6f72 6b73 7061 6365 4964 2729 0a20  'WorkspaceId'). 
-0002bc10: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0002bc20: 6c66 0a0a 0a63 6c61 7373 204c 6973 7454  lf...class ListT
-0002bc30: 656e 736f 7262 6f61 7264 7352 6573 706f  ensorboardsRespo
-0002bc40: 6e73 6542 6f64 7928 5465 614d 6f64 656c  nseBody(TeaModel
-0002bc50: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
-0002bc60: 745f 5f28 7365 6c66 2c20 7265 7175 6573  t__(self, reques
-0002bc70: 745f 6964 3d4e 6f6e 652c 2074 656e 736f  t_id=None, tenso
-0002bc80: 7262 6f61 7264 733d 4e6f 6e65 2c20 746f  rboards=None, to
-0002bc90: 7461 6c5f 636f 756e 743d 4e6f 6e65 293a  tal_count=None):
-0002bca0: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
-0002bcb0: 7175 6573 745f 6964 203d 2072 6571 7565  quest_id = reque
-0002bcc0: 7374 5f69 6420 2023 2074 7970 653a 2073  st_id  # type: s
-0002bcd0: 7472 0a20 2020 2020 2020 2073 656c 662e  tr.        self.
-0002bce0: 7465 6e73 6f72 626f 6172 6473 203d 2074  tensorboards = t
-0002bcf0: 656e 736f 7262 6f61 7264 7320 2023 2074  ensorboards  # t
-0002bd00: 7970 653a 206c 6973 745b 5465 6e73 6f72  ype: list[Tensor
-0002bd10: 626f 6172 645d 0a20 2020 2020 2020 2073  board].        s
-0002bd20: 656c 662e 746f 7461 6c5f 636f 756e 7420  elf.total_count 
-0002bd30: 3d20 746f 7461 6c5f 636f 756e 7420 2023  = total_count  #
-0002bd40: 2074 7970 653a 206c 6f6e 670a 0a20 2020   type: long..   
-0002bd50: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
-0002bd60: 6c66 293a 0a20 2020 2020 2020 2069 6620  lf):.        if 
-0002bd70: 7365 6c66 2e74 656e 736f 7262 6f61 7264  self.tensorboard
-0002bd80: 733a 0a20 2020 2020 2020 2020 2020 2066  s:.            f
-0002bd90: 6f72 206b 2069 6e20 7365 6c66 2e74 656e  or k in self.ten
-0002bda0: 736f 7262 6f61 7264 733a 0a20 2020 2020  sorboards:.     
-0002bdb0: 2020 2020 2020 2020 2020 2069 6620 6b3a             if k:
-0002bdc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0002bdd0: 2020 2020 206b 2e76 616c 6964 6174 6528       k.validate(
-0002bde0: 290a 0a20 2020 2064 6566 2074 6f5f 6d61  )..    def to_ma
-0002bdf0: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
-0002be00: 205f 6d61 7020 3d20 7375 7065 7228 4c69   _map = super(Li
-0002be10: 7374 5465 6e73 6f72 626f 6172 6473 5265  stTensorboardsRe
-0002be20: 7370 6f6e 7365 426f 6479 2c20 7365 6c66  sponseBody, self
-0002be30: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
-0002be40: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
-0002be50: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0002be60: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
-0002be70: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
-0002be80: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
-0002be90: 2069 6620 7365 6c66 2e72 6571 7565 7374   if self.request
-0002bea0: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
-0002beb0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-0002bec0: 756c 745b 2752 6571 7565 7374 4964 275d  ult['RequestId']
-0002bed0: 203d 2073 656c 662e 7265 7175 6573 745f   = self.request_
-0002bee0: 6964 0a20 2020 2020 2020 2072 6573 756c  id.        resul
-0002bef0: 745b 2754 656e 736f 7262 6f61 7264 7327  t['Tensorboards'
-0002bf00: 5d20 3d20 5b5d 0a20 2020 2020 2020 2069  ] = [].        i
-0002bf10: 6620 7365 6c66 2e74 656e 736f 7262 6f61  f self.tensorboa
-0002bf20: 7264 7320 6973 206e 6f74 204e 6f6e 653a  rds is not None:
-0002bf30: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-0002bf40: 206b 2069 6e20 7365 6c66 2e74 656e 736f   k in self.tenso
-0002bf50: 7262 6f61 7264 733a 0a20 2020 2020 2020  rboards:.       
-0002bf60: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-0002bf70: 2754 656e 736f 7262 6f61 7264 7327 5d2e  'Tensorboards'].
-0002bf80: 6170 7065 6e64 286b 2e74 6f5f 6d61 7028  append(k.to_map(
-0002bf90: 2920 6966 206b 2065 6c73 6520 4e6f 6e65  ) if k else None
-0002bfa0: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-0002bfb0: 662e 746f 7461 6c5f 636f 756e 7420 6973  f.total_count is
-0002bfc0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0002bfd0: 2020 2020 2020 2072 6573 756c 745b 2754         result['T
-0002bfe0: 6f74 616c 436f 756e 7427 5d20 3d20 7365  otalCount'] = se
-0002bff0: 6c66 2e74 6f74 616c 5f63 6f75 6e74 0a20  lf.total_count. 
-0002c000: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-0002c010: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
-0002c020: 6f6d 5f6d 6170 2873 656c 662c 206d 3d4e  om_map(self, m=N
-0002c030: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
-0002c040: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
-0002c050: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-0002c060: 5265 7175 6573 7449 6427 2920 6973 206e  RequestId') is n
-0002c070: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0002c080: 2020 2020 2073 656c 662e 7265 7175 6573       self.reques
-0002c090: 745f 6964 203d 206d 2e67 6574 2827 5265  t_id = m.get('Re
-0002c0a0: 7175 6573 7449 6427 290a 2020 2020 2020  questId').      
-0002c0b0: 2020 7365 6c66 2e74 656e 736f 7262 6f61    self.tensorboa
-0002c0c0: 7264 7320 3d20 5b5d 0a20 2020 2020 2020  rds = [].       
-0002c0d0: 2069 6620 6d2e 6765 7428 2754 656e 736f   if m.get('Tenso
-0002c0e0: 7262 6f61 7264 7327 2920 6973 206e 6f74  rboards') is not
-0002c0f0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0002c100: 2020 2066 6f72 206b 2069 6e20 6d2e 6765     for k in m.ge
-0002c110: 7428 2754 656e 736f 7262 6f61 7264 7327  t('Tensorboards'
-0002c120: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0002c130: 2020 2074 656d 705f 6d6f 6465 6c20 3d20     temp_model = 
-0002c140: 5465 6e73 6f72 626f 6172 6428 290a 2020  Tensorboard().  
-0002c150: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0002c160: 6c66 2e74 656e 736f 7262 6f61 7264 732e  lf.tensorboards.
-0002c170: 6170 7065 6e64 2874 656d 705f 6d6f 6465  append(temp_mode
-0002c180: 6c2e 6672 6f6d 5f6d 6170 286b 2929 0a20  l.from_map(k)). 
-0002c190: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
-0002c1a0: 2754 6f74 616c 436f 756e 7427 2920 6973  'TotalCount') is
-0002c1b0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0002c1c0: 2020 2020 2020 2073 656c 662e 746f 7461         self.tota
-0002c1d0: 6c5f 636f 756e 7420 3d20 6d2e 6765 7428  l_count = m.get(
-0002c1e0: 2754 6f74 616c 436f 756e 7427 290a 2020  'TotalCount').  
-0002c1f0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0002c200: 660a 0a0a 636c 6173 7320 4c69 7374 5465  f...class ListTe
-0002c210: 6e73 6f72 626f 6172 6473 5265 7370 6f6e  nsorboardsRespon
-0002c220: 7365 2854 6561 4d6f 6465 6c29 3a0a 2020  se(TeaModel):.  
-0002c230: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
-0002c240: 656c 662c 2068 6561 6465 7273 3d4e 6f6e  elf, headers=Non
-0002c250: 652c 2073 7461 7475 735f 636f 6465 3d4e  e, status_code=N
-0002c260: 6f6e 652c 2062 6f64 793d 4e6f 6e65 293a  one, body=None):
-0002c270: 0a20 2020 2020 2020 2073 656c 662e 6865  .        self.he
-0002c280: 6164 6572 7320 3d20 6865 6164 6572 7320  aders = headers 
-0002c290: 2023 2074 7970 653a 2064 6963 745b 7374   # type: dict[st
-0002c2a0: 722c 2073 7472 5d0a 2020 2020 2020 2020  r, str].        
-0002c2b0: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
-0002c2c0: 203d 2073 7461 7475 735f 636f 6465 2020   = status_code  
-0002c2d0: 2320 7479 7065 3a20 696e 740a 2020 2020  # type: int.    
-0002c2e0: 2020 2020 7365 6c66 2e62 6f64 7920 3d20      self.body = 
-0002c2f0: 626f 6479 2020 2320 7479 7065 3a20 4c69  body  # type: Li
-0002c300: 7374 5465 6e73 6f72 626f 6172 6473 5265  stTensorboardsRe
-0002c310: 7370 6f6e 7365 426f 6479 0a0a 2020 2020  sponseBody..    
-0002c320: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
-0002c330: 6629 3a0a 2020 2020 2020 2020 7365 6c66  f):.        self
-0002c340: 2e76 616c 6964 6174 655f 7265 7175 6972  .validate_requir
-0002c350: 6564 2873 656c 662e 6865 6164 6572 732c  ed(self.headers,
-0002c360: 2027 6865 6164 6572 7327 290a 2020 2020   'headers').    
-0002c370: 2020 2020 7365 6c66 2e76 616c 6964 6174      self.validat
-0002c380: 655f 7265 7175 6972 6564 2873 656c 662e  e_required(self.
-0002c390: 7374 6174 7573 5f63 6f64 652c 2027 7374  status_code, 'st
-0002c3a0: 6174 7573 5f63 6f64 6527 290a 2020 2020  atus_code').    
-0002c3b0: 2020 2020 7365 6c66 2e76 616c 6964 6174      self.validat
-0002c3c0: 655f 7265 7175 6972 6564 2873 656c 662e  e_required(self.
-0002c3d0: 626f 6479 2c20 2762 6f64 7927 290a 2020  body, 'body').  
-0002c3e0: 2020 2020 2020 6966 2073 656c 662e 626f        if self.bo
-0002c3f0: 6479 3a0a 2020 2020 2020 2020 2020 2020  dy:.            
-0002c400: 7365 6c66 2e62 6f64 792e 7661 6c69 6461  self.body.valida
-0002c410: 7465 2829 0a0a 2020 2020 6465 6620 746f  te()..    def to
-0002c420: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
-0002c430: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
-0002c440: 284c 6973 7454 656e 736f 7262 6f61 7264  (ListTensorboard
-0002c450: 7352 6573 706f 6e73 652c 2073 656c 6629  sResponse, self)
-0002c460: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
-0002c470: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
-0002c480: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0002c490: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
-0002c4a0: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
-0002c4b0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-0002c4c0: 6966 2073 656c 662e 6865 6164 6572 7320  if self.headers 
-0002c4d0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0002c4e0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-0002c4f0: 2768 6561 6465 7273 275d 203d 2073 656c  'headers'] = sel
-0002c500: 662e 6865 6164 6572 730a 2020 2020 2020  f.headers.      
-0002c510: 2020 6966 2073 656c 662e 7374 6174 7573    if self.status
-0002c520: 5f63 6f64 6520 6973 206e 6f74 204e 6f6e  _code is not Non
-0002c530: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-0002c540: 6573 756c 745b 2773 7461 7475 7343 6f64  esult['statusCod
-0002c550: 6527 5d20 3d20 7365 6c66 2e73 7461 7475  e'] = self.statu
-0002c560: 735f 636f 6465 0a20 2020 2020 2020 2069  s_code.        i
-0002c570: 6620 7365 6c66 2e62 6f64 7920 6973 206e  f self.body is n
-0002c580: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0002c590: 2020 2020 2072 6573 756c 745b 2762 6f64       result['bod
-0002c5a0: 7927 5d20 3d20 7365 6c66 2e62 6f64 792e  y'] = self.body.
-0002c5b0: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
-0002c5c0: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
-0002c5d0: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
-0002c5e0: 2873 656c 662c 206d 3d4e 6f6e 6529 3a0a  (self, m=None):.
-0002c5f0: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
-0002c600: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-0002c610: 6966 206d 2e67 6574 2827 6865 6164 6572  if m.get('header
-0002c620: 7327 2920 6973 206e 6f74 204e 6f6e 653a  s') is not None:
-0002c630: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0002c640: 662e 6865 6164 6572 7320 3d20 6d2e 6765  f.headers = m.ge
-0002c650: 7428 2768 6561 6465 7273 2729 0a20 2020  t('headers').   
-0002c660: 2020 2020 2069 6620 6d2e 6765 7428 2773       if m.get('s
-0002c670: 7461 7475 7343 6f64 6527 2920 6973 206e  tatusCode') is n
-0002c680: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0002c690: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
-0002c6a0: 5f63 6f64 6520 3d20 6d2e 6765 7428 2773  _code = m.get('s
-0002c6b0: 7461 7475 7343 6f64 6527 290a 2020 2020  tatusCode').    
-0002c6c0: 2020 2020 6966 206d 2e67 6574 2827 626f      if m.get('bo
-0002c6d0: 6479 2729 2069 7320 6e6f 7420 4e6f 6e65  dy') is not None
-0002c6e0: 3a0a 2020 2020 2020 2020 2020 2020 7465  :.            te
-0002c6f0: 6d70 5f6d 6f64 656c 203d 204c 6973 7454  mp_model = ListT
-0002c700: 656e 736f 7262 6f61 7264 7352 6573 706f  ensorboardsRespo
-0002c710: 6e73 6542 6f64 7928 290a 2020 2020 2020  nseBody().      
-0002c720: 2020 2020 2020 7365 6c66 2e62 6f64 7920        self.body 
-0002c730: 3d20 7465 6d70 5f6d 6f64 656c 2e66 726f  = temp_model.fro
-0002c740: 6d5f 6d61 7028 6d5b 2762 6f64 7927 5d29  m_map(m['body'])
-0002c750: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0002c760: 7365 6c66 0a0a 0a63 6c61 7373 2053 7461  self...class Sta
-0002c770: 7274 5465 6e73 6f72 626f 6172 6452 6571  rtTensorboardReq
-0002c780: 7565 7374 2854 6561 4d6f 6465 6c29 3a0a  uest(TeaModel):.
-0002c790: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-0002c7a0: 2873 656c 662c 2077 6f72 6b73 7061 6365  (self, workspace
-0002c7b0: 5f69 643d 4e6f 6e65 293a 0a20 2020 2020  _id=None):.     
-0002c7c0: 2020 2073 656c 662e 776f 726b 7370 6163     self.workspac
-0002c7d0: 655f 6964 203d 2077 6f72 6b73 7061 6365  e_id = workspace
-0002c7e0: 5f69 6420 2023 2074 7970 653a 2073 7472  _id  # type: str
-0002c7f0: 0a0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
-0002c800: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
-0002c810: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
-0002c820: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
-0002c830: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
-0002c840: 6572 2853 7461 7274 5465 6e73 6f72 626f  er(StartTensorbo
-0002c850: 6172 6452 6571 7565 7374 2c20 7365 6c66  ardRequest, self
-0002c860: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
-0002c870: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
-0002c880: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0002c890: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
-0002c8a0: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
-0002c8b0: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
-0002c8c0: 2069 6620 7365 6c66 2e77 6f72 6b73 7061   if self.workspa
-0002c8d0: 6365 5f69 6420 6973 206e 6f74 204e 6f6e  ce_id is not Non
-0002c8e0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-0002c8f0: 6573 756c 745b 2757 6f72 6b73 7061 6365  esult['Workspace
-0002c900: 4964 275d 203d 2073 656c 662e 776f 726b  Id'] = self.work
-0002c910: 7370 6163 655f 6964 0a20 2020 2020 2020  space_id.       
-0002c920: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
-0002c930: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
-0002c940: 2873 656c 662c 206d 3d4e 6f6e 6529 3a0a  (self, m=None):.
-0002c950: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
-0002c960: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-0002c970: 6966 206d 2e67 6574 2827 576f 726b 7370  if m.get('Worksp
-0002c980: 6163 6549 6427 2920 6973 206e 6f74 204e  aceId') is not N
-0002c990: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0002c9a0: 2073 656c 662e 776f 726b 7370 6163 655f   self.workspace_
-0002c9b0: 6964 203d 206d 2e67 6574 2827 576f 726b  id = m.get('Work
-0002c9c0: 7370 6163 6549 6427 290a 2020 2020 2020  spaceId').      
-0002c9d0: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
-0002c9e0: 636c 6173 7320 5374 6172 7454 656e 736f  class StartTenso
-0002c9f0: 7262 6f61 7264 5265 7370 6f6e 7365 426f  rboardResponseBo
-0002ca00: 6479 2854 6561 4d6f 6465 6c29 3a0a 2020  dy(TeaModel):.  
-0002ca10: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
-0002ca20: 656c 662c 2072 6571 7565 7374 5f69 643d  elf, request_id=
-0002ca30: 4e6f 6e65 2c20 7465 6e73 6f72 626f 6172  None, tensorboar
-0002ca40: 645f 6964 3d4e 6f6e 6529 3a0a 2020 2020  d_id=None):.    
-0002ca50: 2020 2020 7365 6c66 2e72 6571 7565 7374      self.request
-0002ca60: 5f69 6420 3d20 7265 7175 6573 745f 6964  _id = request_id
-0002ca70: 2020 2320 7479 7065 3a20 7374 720a 2020    # type: str.  
-0002ca80: 2020 2020 2020 7365 6c66 2e74 656e 736f        self.tenso
-0002ca90: 7262 6f61 7264 5f69 6420 3d20 7465 6e73  rboard_id = tens
-0002caa0: 6f72 626f 6172 645f 6964 2020 2320 7479  orboard_id  # ty
-0002cab0: 7065 3a20 7374 720a 0a20 2020 2064 6566  pe: str..    def
-0002cac0: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
-0002cad0: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
-0002cae0: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
-0002caf0: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
-0002cb00: 7020 3d20 7375 7065 7228 5374 6172 7454  p = super(StartT
-0002cb10: 656e 736f 7262 6f61 7264 5265 7370 6f6e  ensorboardRespon
-0002cb20: 7365 426f 6479 2c20 7365 6c66 292e 746f  seBody, self).to
-0002cb30: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
-0002cb40: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
-0002cb50: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0002cb60: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
-0002cb70: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
-0002cb80: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
-0002cb90: 7365 6c66 2e72 6571 7565 7374 5f69 6420  self.request_id 
-0002cba0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0002cbb0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-0002cbc0: 2752 6571 7565 7374 4964 275d 203d 2073  'RequestId'] = s
-0002cbd0: 656c 662e 7265 7175 6573 745f 6964 0a20  elf.request_id. 
-0002cbe0: 2020 2020 2020 2069 6620 7365 6c66 2e74         if self.t
-0002cbf0: 656e 736f 7262 6f61 7264 5f69 6420 6973  ensorboard_id is
-0002cc00: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0002cc10: 2020 2020 2020 2072 6573 756c 745b 2754         result['T
-0002cc20: 656e 736f 7262 6f61 7264 4964 275d 203d  ensorboardId'] =
-0002cc30: 2073 656c 662e 7465 6e73 6f72 626f 6172   self.tensorboar
-0002cc40: 645f 6964 0a20 2020 2020 2020 2072 6574  d_id.        ret
-0002cc50: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
-0002cc60: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
-0002cc70: 662c 206d 3d4e 6f6e 6529 3a0a 2020 2020  f, m=None):.    
-0002cc80: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
-0002cc90: 7428 290a 2020 2020 2020 2020 6966 206d  t().        if m
-0002cca0: 2e67 6574 2827 5265 7175 6573 7449 6427  .get('RequestId'
-0002ccb0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-0002ccc0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0002ccd0: 7265 7175 6573 745f 6964 203d 206d 2e67  request_id = m.g
-0002cce0: 6574 2827 5265 7175 6573 7449 6427 290a  et('RequestId').
-0002ccf0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
-0002cd00: 2827 5465 6e73 6f72 626f 6172 6449 6427  ('TensorboardId'
-0002cd10: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-0002cd20: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0002cd30: 7465 6e73 6f72 626f 6172 645f 6964 203d  tensorboard_id =
-0002cd40: 206d 2e67 6574 2827 5465 6e73 6f72 626f   m.get('Tensorbo
-0002cd50: 6172 6449 6427 290a 2020 2020 2020 2020  ardId').        
-0002cd60: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
-0002cd70: 6173 7320 5374 6172 7454 656e 736f 7262  ass StartTensorb
-0002cd80: 6f61 7264 5265 7370 6f6e 7365 2854 6561  oardResponse(Tea
-0002cd90: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
-0002cda0: 5f5f 696e 6974 5f5f 2873 656c 662c 2068  __init__(self, h
-0002cdb0: 6561 6465 7273 3d4e 6f6e 652c 2073 7461  eaders=None, sta
-0002cdc0: 7475 735f 636f 6465 3d4e 6f6e 652c 2062  tus_code=None, b
-0002cdd0: 6f64 793d 4e6f 6e65 293a 0a20 2020 2020  ody=None):.     
-0002cde0: 2020 2073 656c 662e 6865 6164 6572 7320     self.headers 
-0002cdf0: 3d20 6865 6164 6572 7320 2023 2074 7970  = headers  # typ
-0002ce00: 653a 2064 6963 745b 7374 722c 2073 7472  e: dict[str, str
-0002ce10: 5d0a 2020 2020 2020 2020 7365 6c66 2e73  ].        self.s
-0002ce20: 7461 7475 735f 636f 6465 203d 2073 7461  tatus_code = sta
-0002ce30: 7475 735f 636f 6465 2020 2320 7479 7065  tus_code  # type
-0002ce40: 3a20 696e 740a 2020 2020 2020 2020 7365  : int.        se
-0002ce50: 6c66 2e62 6f64 7920 3d20 626f 6479 2020  lf.body = body  
-0002ce60: 2320 7479 7065 3a20 5374 6172 7454 656e  # type: StartTen
-0002ce70: 736f 7262 6f61 7264 5265 7370 6f6e 7365  sorboardResponse
-0002ce80: 426f 6479 0a0a 2020 2020 6465 6620 7661  Body..    def va
-0002ce90: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
-0002cea0: 2020 2020 2020 7365 6c66 2e76 616c 6964        self.valid
-0002ceb0: 6174 655f 7265 7175 6972 6564 2873 656c  ate_required(sel
-0002cec0: 662e 6865 6164 6572 732c 2027 6865 6164  f.headers, 'head
-0002ced0: 6572 7327 290a 2020 2020 2020 2020 7365  ers').        se
-0002cee0: 6c66 2e76 616c 6964 6174 655f 7265 7175  lf.validate_requ
-0002cef0: 6972 6564 2873 656c 662e 7374 6174 7573  ired(self.status
-0002cf00: 5f63 6f64 652c 2027 7374 6174 7573 5f63  _code, 'status_c
-0002cf10: 6f64 6527 290a 2020 2020 2020 2020 7365  ode').        se
-0002cf20: 6c66 2e76 616c 6964 6174 655f 7265 7175  lf.validate_requ
-0002cf30: 6972 6564 2873 656c 662e 626f 6479 2c20  ired(self.body, 
-0002cf40: 2762 6f64 7927 290a 2020 2020 2020 2020  'body').        
-0002cf50: 6966 2073 656c 662e 626f 6479 3a0a 2020  if self.body:.  
-0002cf60: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
-0002cf70: 6f64 792e 7661 6c69 6461 7465 2829 0a0a  ody.validate()..
-0002cf80: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
-0002cf90: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
-0002cfa0: 6170 203d 2073 7570 6572 2853 7461 7274  ap = super(Start
-0002cfb0: 5465 6e73 6f72 626f 6172 6452 6573 706f  TensorboardRespo
-0002cfc0: 6e73 652c 2073 656c 6629 2e74 6f5f 6d61  nse, self).to_ma
-0002cfd0: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
-0002cfe0: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
-0002cff0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-0002d000: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
-0002d010: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
-0002d020: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-0002d030: 662e 6865 6164 6572 7320 6973 206e 6f74  f.headers is not
-0002d040: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0002d050: 2020 2072 6573 756c 745b 2768 6561 6465     result['heade
-0002d060: 7273 275d 203d 2073 656c 662e 6865 6164  rs'] = self.head
-0002d070: 6572 730a 2020 2020 2020 2020 6966 2073  ers.        if s
-0002d080: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
-0002d090: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0002d0a0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-0002d0b0: 2773 7461 7475 7343 6f64 6527 5d20 3d20  'statusCode'] = 
-0002d0c0: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
-0002d0d0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0002d0e0: 2e62 6f64 7920 6973 206e 6f74 204e 6f6e  .body is not Non
-0002d0f0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-0002d100: 6573 756c 745b 2762 6f64 7927 5d20 3d20  esult['body'] = 
-0002d110: 7365 6c66 2e62 6f64 792e 746f 5f6d 6170  self.body.to_map
-0002d120: 2829 0a20 2020 2020 2020 2072 6574 7572  ().        retur
-0002d130: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
-0002d140: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
-0002d150: 206d 3d4e 6f6e 6529 3a0a 2020 2020 2020   m=None):.      
-0002d160: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
-0002d170: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-0002d180: 6574 2827 6865 6164 6572 7327 2920 6973  et('headers') is
-0002d190: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0002d1a0: 2020 2020 2020 2073 656c 662e 6865 6164         self.head
-0002d1b0: 6572 7320 3d20 6d2e 6765 7428 2768 6561  ers = m.get('hea
-0002d1c0: 6465 7273 2729 0a20 2020 2020 2020 2069  ders').        i
-0002d1d0: 6620 6d2e 6765 7428 2773 7461 7475 7343  f m.get('statusC
-0002d1e0: 6f64 6527 2920 6973 206e 6f74 204e 6f6e  ode') is not Non
-0002d1f0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-0002d200: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
-0002d210: 3d20 6d2e 6765 7428 2773 7461 7475 7343  = m.get('statusC
-0002d220: 6f64 6527 290a 2020 2020 2020 2020 6966  ode').        if
-0002d230: 206d 2e67 6574 2827 626f 6479 2729 2069   m.get('body') i
-0002d240: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0002d250: 2020 2020 2020 2020 7465 6d70 5f6d 6f64          temp_mod
-0002d260: 656c 203d 2053 7461 7274 5465 6e73 6f72  el = StartTensor
-0002d270: 626f 6172 6452 6573 706f 6e73 6542 6f64  boardResponseBod
-0002d280: 7928 290a 2020 2020 2020 2020 2020 2020  y().            
-0002d290: 7365 6c66 2e62 6f64 7920 3d20 7465 6d70  self.body = temp
-0002d2a0: 5f6d 6f64 656c 2e66 726f 6d5f 6d61 7028  _model.from_map(
-0002d2b0: 6d5b 2762 6f64 7927 5d29 0a20 2020 2020  m['body']).     
-0002d2c0: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
-0002d2d0: 0a63 6c61 7373 2053 746f 704a 6f62 5265  .class StopJobRe
-0002d2e0: 7370 6f6e 7365 426f 6479 2854 6561 4d6f  sponseBody(TeaMo
-0002d2f0: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
-0002d300: 696e 6974 5f5f 2873 656c 662c 206a 6f62  init__(self, job
-0002d310: 5f69 643d 4e6f 6e65 2c20 7265 7175 6573  _id=None, reques
-0002d320: 745f 6964 3d4e 6f6e 6529 3a0a 2020 2020  t_id=None):.    
-0002d330: 2020 2020 7365 6c66 2e6a 6f62 5f69 6420      self.job_id 
-0002d340: 3d20 6a6f 625f 6964 2020 2320 7479 7065  = job_id  # type
-0002d350: 3a20 7374 720a 2020 2020 2020 2020 7365  : str.        se
-0002d360: 6c66 2e72 6571 7565 7374 5f69 6420 3d20  lf.request_id = 
-0002d370: 7265 7175 6573 745f 6964 2020 2320 7479  request_id  # ty
-0002d380: 7065 3a20 7374 720a 0a20 2020 2064 6566  pe: str..    def
-0002d390: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
-0002d3a0: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
-0002d3b0: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
-0002d3c0: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
-0002d3d0: 7020 3d20 7375 7065 7228 5374 6f70 4a6f  p = super(StopJo
-0002d3e0: 6252 6573 706f 6e73 6542 6f64 792c 2073  bResponseBody, s
-0002d3f0: 656c 6629 2e74 6f5f 6d61 7028 290a 2020  elf).to_map().  
-0002d400: 2020 2020 2020 6966 205f 6d61 7020 6973        if _map is
-0002d410: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0002d420: 2020 2020 2020 2072 6574 7572 6e20 5f6d         return _m
-0002d430: 6170 0a0a 2020 2020 2020 2020 7265 7375  ap..        resu
-0002d440: 6c74 203d 2064 6963 7428 290a 2020 2020  lt = dict().    
-0002d450: 2020 2020 6966 2073 656c 662e 6a6f 625f      if self.job_
-0002d460: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
-0002d470: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-0002d480: 6c74 5b27 4a6f 6249 6427 5d20 3d20 7365  lt['JobId'] = se
-0002d490: 6c66 2e6a 6f62 5f69 640a 2020 2020 2020  lf.job_id.      
-0002d4a0: 2020 6966 2073 656c 662e 7265 7175 6573    if self.reques
-0002d4b0: 745f 6964 2069 7320 6e6f 7420 4e6f 6e65  t_id is not None
-0002d4c0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0002d4d0: 7375 6c74 5b27 5265 7175 6573 7449 6427  sult['RequestId'
-0002d4e0: 5d20 3d20 7365 6c66 2e72 6571 7565 7374  ] = self.request
-0002d4f0: 5f69 640a 2020 2020 2020 2020 7265 7475  _id.        retu
-0002d500: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
-0002d510: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
-0002d520: 2c20 6d3d 4e6f 6e65 293a 0a20 2020 2020  , m=None):.     
-0002d530: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
-0002d540: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
-0002d550: 6765 7428 274a 6f62 4964 2729 2069 7320  get('JobId') is 
-0002d560: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-0002d570: 2020 2020 2020 7365 6c66 2e6a 6f62 5f69        self.job_i
-0002d580: 6420 3d20 6d2e 6765 7428 274a 6f62 4964  d = m.get('JobId
-0002d590: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-0002d5a0: 6765 7428 2752 6571 7565 7374 4964 2729  get('RequestId')
-0002d5b0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0002d5c0: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
-0002d5d0: 6571 7565 7374 5f69 6420 3d20 6d2e 6765  equest_id = m.ge
-0002d5e0: 7428 2752 6571 7565 7374 4964 2729 0a20  t('RequestId'). 
-0002d5f0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0002d600: 6c66 0a0a 0a63 6c61 7373 2053 746f 704a  lf...class StopJ
-0002d610: 6f62 5265 7370 6f6e 7365 2854 6561 4d6f  obResponse(TeaMo
-0002d620: 6465 6c29 3a0a 2020 2020 6465 6620 5f5f  del):.    def __
-0002d630: 696e 6974 5f5f 2873 656c 662c 2068 6561  init__(self, hea
-0002d640: 6465 7273 3d4e 6f6e 652c 2073 7461 7475  ders=None, statu
-0002d650: 735f 636f 6465 3d4e 6f6e 652c 2062 6f64  s_code=None, bod
-0002d660: 793d 4e6f 6e65 293a 0a20 2020 2020 2020  y=None):.       
-0002d670: 2073 656c 662e 6865 6164 6572 7320 3d20   self.headers = 
-0002d680: 6865 6164 6572 7320 2023 2074 7970 653a  headers  # type:
-0002d690: 2064 6963 745b 7374 722c 2073 7472 5d0a   dict[str, str].
-0002d6a0: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
-0002d6b0: 7475 735f 636f 6465 203d 2073 7461 7475  tus_code = statu
-0002d6c0: 735f 636f 6465 2020 2320 7479 7065 3a20  s_code  # type: 
-0002d6d0: 696e 740a 2020 2020 2020 2020 7365 6c66  int.        self
-0002d6e0: 2e62 6f64 7920 3d20 626f 6479 2020 2320  .body = body  # 
-0002d6f0: 7479 7065 3a20 5374 6f70 4a6f 6252 6573  type: StopJobRes
-0002d700: 706f 6e73 6542 6f64 790a 0a20 2020 2064  ponseBody..    d
-0002d710: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
-0002d720: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-0002d730: 7661 6c69 6461 7465 5f72 6571 7569 7265  validate_require
-0002d740: 6428 7365 6c66 2e68 6561 6465 7273 2c20  d(self.headers, 
-0002d750: 2768 6561 6465 7273 2729 0a20 2020 2020  'headers').     
-0002d760: 2020 2073 656c 662e 7661 6c69 6461 7465     self.validate
-0002d770: 5f72 6571 7569 7265 6428 7365 6c66 2e73  _required(self.s
-0002d780: 7461 7475 735f 636f 6465 2c20 2773 7461  tatus_code, 'sta
-0002d790: 7475 735f 636f 6465 2729 0a20 2020 2020  tus_code').     
-0002d7a0: 2020 2073 656c 662e 7661 6c69 6461 7465     self.validate
-0002d7b0: 5f72 6571 7569 7265 6428 7365 6c66 2e62  _required(self.b
-0002d7c0: 6f64 792c 2027 626f 6479 2729 0a20 2020  ody, 'body').   
-0002d7d0: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
-0002d7e0: 793a 0a20 2020 2020 2020 2020 2020 2073  y:.            s
-0002d7f0: 656c 662e 626f 6479 2e76 616c 6964 6174  elf.body.validat
-0002d800: 6528 290a 0a20 2020 2064 6566 2074 6f5f  e()..    def to_
-0002d810: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
-0002d820: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
-0002d830: 5374 6f70 4a6f 6252 6573 706f 6e73 652c  StopJobResponse,
-0002d840: 2073 656c 6629 2e74 6f5f 6d61 7028 290a   self).to_map().
-0002d850: 2020 2020 2020 2020 6966 205f 6d61 7020          if _map 
-0002d860: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0002d870: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0002d880: 5f6d 6170 0a0a 2020 2020 2020 2020 7265  _map..        re
-0002d890: 7375 6c74 203d 2064 6963 7428 290a 2020  sult = dict().  
-0002d8a0: 2020 2020 2020 6966 2073 656c 662e 6865        if self.he
-0002d8b0: 6164 6572 7320 6973 206e 6f74 204e 6f6e  aders is not Non
-0002d8c0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-0002d8d0: 6573 756c 745b 2768 6561 6465 7273 275d  esult['headers']
-0002d8e0: 203d 2073 656c 662e 6865 6164 6572 730a   = self.headers.
-0002d8f0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0002d900: 7374 6174 7573 5f63 6f64 6520 6973 206e  status_code is n
-0002d910: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0002d920: 2020 2020 2072 6573 756c 745b 2773 7461       result['sta
-0002d930: 7475 7343 6f64 6527 5d20 3d20 7365 6c66  tusCode'] = self
-0002d940: 2e73 7461 7475 735f 636f 6465 0a20 2020  .status_code.   
-0002d950: 2020 2020 2069 6620 7365 6c66 2e62 6f64       if self.bod
-0002d960: 7920 6973 206e 6f74 204e 6f6e 653a 0a20  y is not None:. 
-0002d970: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-0002d980: 745b 2762 6f64 7927 5d20 3d20 7365 6c66  t['body'] = self
-0002d990: 2e62 6f64 792e 746f 5f6d 6170 2829 0a20  .body.to_map(). 
-0002d9a0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-0002d9b0: 7375 6c74 0a0a 2020 2020 6465 6620 6672  sult..    def fr
-0002d9c0: 6f6d 5f6d 6170 2873 656c 662c 206d 3d4e  om_map(self, m=N
-0002d9d0: 6f6e 6529 3a0a 2020 2020 2020 2020 6d20  one):.        m 
-0002d9e0: 3d20 6d20 6f72 2064 6963 7428 290a 2020  = m or dict().  
-0002d9f0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-0002da00: 6865 6164 6572 7327 2920 6973 206e 6f74  headers') is not
-0002da10: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0002da20: 2020 2073 656c 662e 6865 6164 6572 7320     self.headers 
-0002da30: 3d20 6d2e 6765 7428 2768 6561 6465 7273  = m.get('headers
-0002da40: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
-0002da50: 6765 7428 2773 7461 7475 7343 6f64 6527  get('statusCode'
-0002da60: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-0002da70: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0002da80: 7374 6174 7573 5f63 6f64 6520 3d20 6d2e  status_code = m.
-0002da90: 6765 7428 2773 7461 7475 7343 6f64 6527  get('statusCode'
-0002daa0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-0002dab0: 6574 2827 626f 6479 2729 2069 7320 6e6f  et('body') is no
-0002dac0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0002dad0: 2020 2020 7465 6d70 5f6d 6f64 656c 203d      temp_model =
-0002dae0: 2053 746f 704a 6f62 5265 7370 6f6e 7365   StopJobResponse
-0002daf0: 426f 6479 2829 0a20 2020 2020 2020 2020  Body().         
-0002db00: 2020 2073 656c 662e 626f 6479 203d 2074     self.body = t
-0002db10: 656d 705f 6d6f 6465 6c2e 6672 6f6d 5f6d  emp_model.from_m
-0002db20: 6170 286d 5b27 626f 6479 275d 290a 2020  ap(m['body']).  
-0002db30: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0002db40: 660a 0a0a 636c 6173 7320 5374 6f70 5465  f...class StopTe
-0002db50: 6e73 6f72 626f 6172 6452 6571 7565 7374  nsorboardRequest
-0002db60: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
-0002db70: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-0002db80: 662c 2077 6f72 6b73 7061 6365 5f69 643d  f, workspace_id=
-0002db90: 4e6f 6e65 293a 0a20 2020 2020 2020 2073  None):.        s
-0002dba0: 656c 662e 776f 726b 7370 6163 655f 6964  elf.workspace_id
-0002dbb0: 203d 2077 6f72 6b73 7061 6365 5f69 6420   = workspace_id 
-0002dbc0: 2023 2074 7970 653a 2073 7472 0a0a 2020   # type: str..  
-0002dbd0: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
-0002dbe0: 656c 6629 3a0a 2020 2020 2020 2020 7061  elf):.        pa
-0002dbf0: 7373 0a0a 2020 2020 6465 6620 746f 5f6d  ss..    def to_m
-0002dc00: 6170 2873 656c 6629 3a0a 2020 2020 2020  ap(self):.      
-0002dc10: 2020 5f6d 6170 203d 2073 7570 6572 2853    _map = super(S
-0002dc20: 746f 7054 656e 736f 7262 6f61 7264 5265  topTensorboardRe
-0002dc30: 7175 6573 742c 2073 656c 6629 2e74 6f5f  quest, self).to_
-0002dc40: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
-0002dc50: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
-0002dc60: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-0002dc70: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
-0002dc80: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
-0002dc90: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
-0002dca0: 656c 662e 776f 726b 7370 6163 655f 6964  elf.workspace_id
-0002dcb0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0002dcc0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0002dcd0: 5b27 576f 726b 7370 6163 6549 6427 5d20  ['WorkspaceId'] 
-0002dce0: 3d20 7365 6c66 2e77 6f72 6b73 7061 6365  = self.workspace
-0002dcf0: 5f69 640a 2020 2020 2020 2020 7265 7475  _id.        retu
-0002dd00: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
-0002dd10: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
-0002dd20: 2c20 6d3d 4e6f 6e65 293a 0a20 2020 2020  , m=None):.     
-0002dd30: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
-0002dd40: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
-0002dd50: 6765 7428 2757 6f72 6b73 7061 6365 4964  get('WorkspaceId
-0002dd60: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-0002dd70: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0002dd80: 2e77 6f72 6b73 7061 6365 5f69 6420 3d20  .workspace_id = 
-0002dd90: 6d2e 6765 7428 2757 6f72 6b73 7061 6365  m.get('Workspace
-0002dda0: 4964 2729 0a20 2020 2020 2020 2072 6574  Id').        ret
-0002ddb0: 7572 6e20 7365 6c66 0a0a 0a63 6c61 7373  urn self...class
-0002ddc0: 2053 746f 7054 656e 736f 7262 6f61 7264   StopTensorboard
-0002ddd0: 5265 7370 6f6e 7365 426f 6479 2854 6561  ResponseBody(Tea
-0002dde0: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
-0002ddf0: 5f5f 696e 6974 5f5f 2873 656c 662c 2072  __init__(self, r
-0002de00: 6571 7565 7374 5f69 643d 4e6f 6e65 2c20  equest_id=None, 
-0002de10: 7465 6e73 6f72 626f 6172 645f 6964 3d4e  tensorboard_id=N
-0002de20: 6f6e 6529 3a0a 2020 2020 2020 2020 7365  one):.        se
-0002de30: 6c66 2e72 6571 7565 7374 5f69 6420 3d20  lf.request_id = 
-0002de40: 7265 7175 6573 745f 6964 2020 2320 7479  request_id  # ty
-0002de50: 7065 3a20 7374 720a 2020 2020 2020 2020  pe: str.        
-0002de60: 7365 6c66 2e74 656e 736f 7262 6f61 7264  self.tensorboard
-0002de70: 5f69 6420 3d20 7465 6e73 6f72 626f 6172  _id = tensorboar
-0002de80: 645f 6964 2020 2320 7479 7065 3a20 7374  d_id  # type: st
-0002de90: 720a 0a20 2020 2064 6566 2076 616c 6964  r..    def valid
-0002dea0: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
-0002deb0: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
-0002dec0: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
-0002ded0: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
-0002dee0: 7065 7228 5374 6f70 5465 6e73 6f72 626f  per(StopTensorbo
-0002def0: 6172 6452 6573 706f 6e73 6542 6f64 792c  ardResponseBody,
-0002df00: 2073 656c 6629 2e74 6f5f 6d61 7028 290a   self).to_map().
-0002df10: 2020 2020 2020 2020 6966 205f 6d61 7020          if _map 
-0002df20: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0002df30: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0002df40: 5f6d 6170 0a0a 2020 2020 2020 2020 7265  _map..        re
-0002df50: 7375 6c74 203d 2064 6963 7428 290a 2020  sult = dict().  
-0002df60: 2020 2020 2020 6966 2073 656c 662e 7265        if self.re
-0002df70: 7175 6573 745f 6964 2069 7320 6e6f 7420  quest_id is not 
-0002df80: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0002df90: 2020 7265 7375 6c74 5b27 5265 7175 6573    result['Reques
-0002dfa0: 7449 6427 5d20 3d20 7365 6c66 2e72 6571  tId'] = self.req
-0002dfb0: 7565 7374 5f69 640a 2020 2020 2020 2020  uest_id.        
-0002dfc0: 6966 2073 656c 662e 7465 6e73 6f72 626f  if self.tensorbo
-0002dfd0: 6172 645f 6964 2069 7320 6e6f 7420 4e6f  ard_id is not No
-0002dfe0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0002dff0: 7265 7375 6c74 5b27 5465 6e73 6f72 626f  result['Tensorbo
-0002e000: 6172 6449 6427 5d20 3d20 7365 6c66 2e74  ardId'] = self.t
-0002e010: 656e 736f 7262 6f61 7264 5f69 640a 2020  ensorboard_id.  
-0002e020: 2020 2020 2020 7265 7475 726e 2072 6573        return res
-0002e030: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
-0002e040: 6d5f 6d61 7028 7365 6c66 2c20 6d3d 4e6f  m_map(self, m=No
-0002e050: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
-0002e060: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
-0002e070: 2020 2020 2069 6620 6d2e 6765 7428 2752       if m.get('R
-0002e080: 6571 7565 7374 4964 2729 2069 7320 6e6f  equestId') is no
-0002e090: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0002e0a0: 2020 2020 7365 6c66 2e72 6571 7565 7374      self.request
-0002e0b0: 5f69 6420 3d20 6d2e 6765 7428 2752 6571  _id = m.get('Req
-0002e0c0: 7565 7374 4964 2729 0a20 2020 2020 2020  uestId').       
-0002e0d0: 2069 6620 6d2e 6765 7428 2754 656e 736f   if m.get('Tenso
-0002e0e0: 7262 6f61 7264 4964 2729 2069 7320 6e6f  rboardId') is no
-0002e0f0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0002e100: 2020 2020 7365 6c66 2e74 656e 736f 7262      self.tensorb
-0002e110: 6f61 7264 5f69 6420 3d20 6d2e 6765 7428  oard_id = m.get(
-0002e120: 2754 656e 736f 7262 6f61 7264 4964 2729  'TensorboardId')
-0002e130: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0002e140: 7365 6c66 0a0a 0a63 6c61 7373 2053 746f  self...class Sto
-0002e150: 7054 656e 736f 7262 6f61 7264 5265 7370  pTensorboardResp
-0002e160: 6f6e 7365 2854 6561 4d6f 6465 6c29 3a0a  onse(TeaModel):.
-0002e170: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-0002e180: 2873 656c 662c 2068 6561 6465 7273 3d4e  (self, headers=N
-0002e190: 6f6e 652c 2073 7461 7475 735f 636f 6465  one, status_code
-0002e1a0: 3d4e 6f6e 652c 2062 6f64 793d 4e6f 6e65  =None, body=None
-0002e1b0: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-0002e1c0: 6865 6164 6572 7320 3d20 6865 6164 6572  headers = header
-0002e1d0: 7320 2023 2074 7970 653a 2064 6963 745b  s  # type: dict[
-0002e1e0: 7374 722c 2073 7472 5d0a 2020 2020 2020  str, str].      
-0002e1f0: 2020 7365 6c66 2e73 7461 7475 735f 636f    self.status_co
-0002e200: 6465 203d 2073 7461 7475 735f 636f 6465  de = status_code
-0002e210: 2020 2320 7479 7065 3a20 696e 740a 2020    # type: int.  
-0002e220: 2020 2020 2020 7365 6c66 2e62 6f64 7920        self.body 
-0002e230: 3d20 626f 6479 2020 2320 7479 7065 3a20  = body  # type: 
-0002e240: 5374 6f70 5465 6e73 6f72 626f 6172 6452  StopTensorboardR
-0002e250: 6573 706f 6e73 6542 6f64 790a 0a20 2020  esponseBody..   
-0002e260: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
-0002e270: 6c66 293a 0a20 2020 2020 2020 2073 656c  lf):.        sel
-0002e280: 662e 7661 6c69 6461 7465 5f72 6571 7569  f.validate_requi
-0002e290: 7265 6428 7365 6c66 2e68 6561 6465 7273  red(self.headers
-0002e2a0: 2c20 2768 6561 6465 7273 2729 0a20 2020  , 'headers').   
-0002e2b0: 2020 2020 2073 656c 662e 7661 6c69 6461       self.valida
-0002e2c0: 7465 5f72 6571 7569 7265 6428 7365 6c66  te_required(self
-0002e2d0: 2e73 7461 7475 735f 636f 6465 2c20 2773  .status_code, 's
-0002e2e0: 7461 7475 735f 636f 6465 2729 0a20 2020  tatus_code').   
-0002e2f0: 2020 2020 2073 656c 662e 7661 6c69 6461       self.valida
-0002e300: 7465 5f72 6571 7569 7265 6428 7365 6c66  te_required(self
-0002e310: 2e62 6f64 792c 2027 626f 6479 2729 0a20  .body, 'body'). 
-0002e320: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
-0002e330: 6f64 793a 0a20 2020 2020 2020 2020 2020  ody:.           
-0002e340: 2073 656c 662e 626f 6479 2e76 616c 6964   self.body.valid
-0002e350: 6174 6528 290a 0a20 2020 2064 6566 2074  ate()..    def t
-0002e360: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
-0002e370: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
-0002e380: 7228 5374 6f70 5465 6e73 6f72 626f 6172  r(StopTensorboar
-0002e390: 6452 6573 706f 6e73 652c 2073 656c 6629  dResponse, self)
-0002e3a0: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
-0002e3b0: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
-0002e3c0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0002e3d0: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
-0002e3e0: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
-0002e3f0: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-0002e400: 6966 2073 656c 662e 6865 6164 6572 7320  if self.headers 
-0002e410: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0002e420: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-0002e430: 2768 6561 6465 7273 275d 203d 2073 656c  'headers'] = sel
-0002e440: 662e 6865 6164 6572 730a 2020 2020 2020  f.headers.      
-0002e450: 2020 6966 2073 656c 662e 7374 6174 7573    if self.status
-0002e460: 5f63 6f64 6520 6973 206e 6f74 204e 6f6e  _code is not Non
-0002e470: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-0002e480: 6573 756c 745b 2773 7461 7475 7343 6f64  esult['statusCod
-0002e490: 6527 5d20 3d20 7365 6c66 2e73 7461 7475  e'] = self.statu
-0002e4a0: 735f 636f 6465 0a20 2020 2020 2020 2069  s_code.        i
-0002e4b0: 6620 7365 6c66 2e62 6f64 7920 6973 206e  f self.body is n
-0002e4c0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0002e4d0: 2020 2020 2072 6573 756c 745b 2762 6f64       result['bod
-0002e4e0: 7927 5d20 3d20 7365 6c66 2e62 6f64 792e  y'] = self.body.
-0002e4f0: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
-0002e500: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
-0002e510: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
-0002e520: 2873 656c 662c 206d 3d4e 6f6e 6529 3a0a  (self, m=None):.
-0002e530: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
-0002e540: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
-0002e550: 6966 206d 2e67 6574 2827 6865 6164 6572  if m.get('header
-0002e560: 7327 2920 6973 206e 6f74 204e 6f6e 653a  s') is not None:
-0002e570: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0002e580: 662e 6865 6164 6572 7320 3d20 6d2e 6765  f.headers = m.ge
-0002e590: 7428 2768 6561 6465 7273 2729 0a20 2020  t('headers').   
-0002e5a0: 2020 2020 2069 6620 6d2e 6765 7428 2773       if m.get('s
-0002e5b0: 7461 7475 7343 6f64 6527 2920 6973 206e  tatusCode') is n
-0002e5c0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0002e5d0: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
-0002e5e0: 5f63 6f64 6520 3d20 6d2e 6765 7428 2773  _code = m.get('s
-0002e5f0: 7461 7475 7343 6f64 6527 290a 2020 2020  tatusCode').    
-0002e600: 2020 2020 6966 206d 2e67 6574 2827 626f      if m.get('bo
-0002e610: 6479 2729 2069 7320 6e6f 7420 4e6f 6e65  dy') is not None
-0002e620: 3a0a 2020 2020 2020 2020 2020 2020 7465  :.            te
-0002e630: 6d70 5f6d 6f64 656c 203d 2053 746f 7054  mp_model = StopT
-0002e640: 656e 736f 7262 6f61 7264 5265 7370 6f6e  ensorboardRespon
-0002e650: 7365 426f 6479 2829 0a20 2020 2020 2020  seBody().       
-0002e660: 2020 2020 2073 656c 662e 626f 6479 203d       self.body =
-0002e670: 2074 656d 705f 6d6f 6465 6c2e 6672 6f6d   temp_model.from
-0002e680: 5f6d 6170 286d 5b27 626f 6479 275d 290a  _map(m['body']).
-0002e690: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0002e6a0: 656c 660a 0a0a 636c 6173 7320 5570 6461  elf...class Upda
-0002e6b0: 7465 4a6f 6252 6571 7565 7374 2854 6561  teJobRequest(Tea
-0002e6c0: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
-0002e6d0: 5f5f 696e 6974 5f5f 2873 656c 662c 2070  __init__(self, p
-0002e6e0: 7269 6f72 6974 793d 4e6f 6e65 293a 0a20  riority=None):. 
-0002e6f0: 2020 2020 2020 2073 656c 662e 7072 696f         self.prio
-0002e700: 7269 7479 203d 2070 7269 6f72 6974 7920  rity = priority 
-0002e710: 2023 2074 7970 653a 2069 6e74 0a0a 2020   # type: int..  
-0002e720: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
-0002e730: 656c 6629 3a0a 2020 2020 2020 2020 7061  elf):.        pa
-0002e740: 7373 0a0a 2020 2020 6465 6620 746f 5f6d  ss..    def to_m
-0002e750: 6170 2873 656c 6629 3a0a 2020 2020 2020  ap(self):.      
-0002e760: 2020 5f6d 6170 203d 2073 7570 6572 2855    _map = super(U
-0002e770: 7064 6174 654a 6f62 5265 7175 6573 742c  pdateJobRequest,
-0002e780: 2073 656c 6629 2e74 6f5f 6d61 7028 290a   self).to_map().
-0002e790: 2020 2020 2020 2020 6966 205f 6d61 7020          if _map 
-0002e7a0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0002e7b0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0002e7c0: 5f6d 6170 0a0a 2020 2020 2020 2020 7265  _map..        re
-0002e7d0: 7375 6c74 203d 2064 6963 7428 290a 2020  sult = dict().  
-0002e7e0: 2020 2020 2020 6966 2073 656c 662e 7072        if self.pr
-0002e7f0: 696f 7269 7479 2069 7320 6e6f 7420 4e6f  iority is not No
-0002e800: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0002e810: 7265 7375 6c74 5b27 5072 696f 7269 7479  result['Priority
-0002e820: 275d 203d 2073 656c 662e 7072 696f 7269  '] = self.priori
-0002e830: 7479 0a20 2020 2020 2020 2072 6574 7572  ty.        retur
-0002e840: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
-0002e850: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
-0002e860: 206d 3d4e 6f6e 6529 3a0a 2020 2020 2020   m=None):.      
-0002e870: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
-0002e880: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-0002e890: 6574 2827 5072 696f 7269 7479 2729 2069  et('Priority') i
-0002e8a0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0002e8b0: 2020 2020 2020 2020 7365 6c66 2e70 7269          self.pri
-0002e8c0: 6f72 6974 7920 3d20 6d2e 6765 7428 2750  ority = m.get('P
-0002e8d0: 7269 6f72 6974 7927 290a 2020 2020 2020  riority').      
-0002e8e0: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
-0002e8f0: 636c 6173 7320 5570 6461 7465 4a6f 6252  class UpdateJobR
-0002e900: 6573 706f 6e73 6542 6f64 7928 5465 614d  esponseBody(TeaM
-0002e910: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
-0002e920: 5f69 6e69 745f 5f28 7365 6c66 2c20 6a6f  _init__(self, jo
-0002e930: 625f 6964 3d4e 6f6e 652c 2072 6571 7565  b_id=None, reque
-0002e940: 7374 5f69 643d 4e6f 6e65 293a 0a20 2020  st_id=None):.   
-0002e950: 2020 2020 2073 656c 662e 6a6f 625f 6964       self.job_id
-0002e960: 203d 206a 6f62 5f69 6420 2023 2074 7970   = job_id  # typ
-0002e970: 653a 2073 7472 0a20 2020 2020 2020 2073  e: str.        s
-0002e980: 656c 662e 7265 7175 6573 745f 6964 203d  elf.request_id =
-0002e990: 2072 6571 7565 7374 5f69 6420 2023 2074   request_id  # t
-0002e9a0: 7970 653a 2073 7472 0a0a 2020 2020 6465  ype: str..    de
-0002e9b0: 6620 7661 6c69 6461 7465 2873 656c 6629  f validate(self)
-0002e9c0: 3a0a 2020 2020 2020 2020 7061 7373 0a0a  :.        pass..
-0002e9d0: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
-0002e9e0: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
-0002e9f0: 6170 203d 2073 7570 6572 2855 7064 6174  ap = super(Updat
-0002ea00: 654a 6f62 5265 7370 6f6e 7365 426f 6479  eJobResponseBody
-0002ea10: 2c20 7365 6c66 292e 746f 5f6d 6170 2829  , self).to_map()
-0002ea20: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
-0002ea30: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0002ea40: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0002ea50: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
-0002ea60: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
-0002ea70: 2020 2020 2020 2069 6620 7365 6c66 2e6a         if self.j
-0002ea80: 6f62 5f69 6420 6973 206e 6f74 204e 6f6e  ob_id is not Non
-0002ea90: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-0002eaa0: 6573 756c 745b 274a 6f62 4964 275d 203d  esult['JobId'] =
-0002eab0: 2073 656c 662e 6a6f 625f 6964 0a20 2020   self.job_id.   
-0002eac0: 2020 2020 2069 6620 7365 6c66 2e72 6571       if self.req
-0002ead0: 7565 7374 5f69 6420 6973 206e 6f74 204e  uest_id is not N
-0002eae0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0002eaf0: 2072 6573 756c 745b 2752 6571 7565 7374   result['Request
-0002eb00: 4964 275d 203d 2073 656c 662e 7265 7175  Id'] = self.requ
-0002eb10: 6573 745f 6964 0a20 2020 2020 2020 2072  est_id.        r
-0002eb20: 6574 7572 6e20 7265 7375 6c74 0a0a 2020  eturn result..  
-0002eb30: 2020 6465 6620 6672 6f6d 5f6d 6170 2873    def from_map(s
-0002eb40: 656c 662c 206d 3d4e 6f6e 6529 3a0a 2020  elf, m=None):.  
-0002eb50: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
-0002eb60: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
-0002eb70: 206d 2e67 6574 2827 4a6f 6249 6427 2920   m.get('JobId') 
-0002eb80: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0002eb90: 2020 2020 2020 2020 2073 656c 662e 6a6f           self.jo
-0002eba0: 625f 6964 203d 206d 2e67 6574 2827 4a6f  b_id = m.get('Jo
-0002ebb0: 6249 6427 290a 2020 2020 2020 2020 6966  bId').        if
-0002ebc0: 206d 2e67 6574 2827 5265 7175 6573 7449   m.get('RequestI
-0002ebd0: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
-0002ebe0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0002ebf0: 662e 7265 7175 6573 745f 6964 203d 206d  f.request_id = m
-0002ec00: 2e67 6574 2827 5265 7175 6573 7449 6427  .get('RequestId'
-0002ec10: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-0002ec20: 2073 656c 660a 0a0a 636c 6173 7320 5570   self...class Up
-0002ec30: 6461 7465 4a6f 6252 6573 706f 6e73 6528  dateJobResponse(
-0002ec40: 5465 614d 6f64 656c 293a 0a20 2020 2064  TeaModel):.    d
-0002ec50: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-0002ec60: 2c20 6865 6164 6572 733d 4e6f 6e65 2c20  , headers=None, 
-0002ec70: 7374 6174 7573 5f63 6f64 653d 4e6f 6e65  status_code=None
-0002ec80: 2c20 626f 6479 3d4e 6f6e 6529 3a0a 2020  , body=None):.  
-0002ec90: 2020 2020 2020 7365 6c66 2e68 6561 6465        self.heade
-0002eca0: 7273 203d 2068 6561 6465 7273 2020 2320  rs = headers  # 
-0002ecb0: 7479 7065 3a20 6469 6374 5b73 7472 2c20  type: dict[str, 
-0002ecc0: 7374 725d 0a20 2020 2020 2020 2073 656c  str].        sel
-0002ecd0: 662e 7374 6174 7573 5f63 6f64 6520 3d20  f.status_code = 
-0002ece0: 7374 6174 7573 5f63 6f64 6520 2023 2074  status_code  # t
-0002ecf0: 7970 653a 2069 6e74 0a20 2020 2020 2020  ype: int.       
-0002ed00: 2073 656c 662e 626f 6479 203d 2062 6f64   self.body = bod
-0002ed10: 7920 2023 2074 7970 653a 2055 7064 6174  y  # type: Updat
-0002ed20: 654a 6f62 5265 7370 6f6e 7365 426f 6479  eJobResponseBody
-0002ed30: 0a0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
-0002ed40: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
-0002ed50: 2020 7365 6c66 2e76 616c 6964 6174 655f    self.validate_
-0002ed60: 7265 7175 6972 6564 2873 656c 662e 6865  required(self.he
-0002ed70: 6164 6572 732c 2027 6865 6164 6572 7327  aders, 'headers'
-0002ed80: 290a 2020 2020 2020 2020 7365 6c66 2e76  ).        self.v
-0002ed90: 616c 6964 6174 655f 7265 7175 6972 6564  alidate_required
-0002eda0: 2873 656c 662e 7374 6174 7573 5f63 6f64  (self.status_cod
-0002edb0: 652c 2027 7374 6174 7573 5f63 6f64 6527  e, 'status_code'
-0002edc0: 290a 2020 2020 2020 2020 7365 6c66 2e76  ).        self.v
-0002edd0: 616c 6964 6174 655f 7265 7175 6972 6564  alidate_required
-0002ede0: 2873 656c 662e 626f 6479 2c20 2762 6f64  (self.body, 'bod
-0002edf0: 7927 290a 2020 2020 2020 2020 6966 2073  y').        if s
-0002ee00: 656c 662e 626f 6479 3a0a 2020 2020 2020  elf.body:.      
-0002ee10: 2020 2020 2020 7365 6c66 2e62 6f64 792e        self.body.
-0002ee20: 7661 6c69 6461 7465 2829 0a0a 2020 2020  validate()..    
-0002ee30: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
-0002ee40: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
-0002ee50: 2073 7570 6572 2855 7064 6174 654a 6f62   super(UpdateJob
-0002ee60: 5265 7370 6f6e 7365 2c20 7365 6c66 292e  Response, self).
-0002ee70: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
-0002ee80: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
-0002ee90: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0002eea0: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
-0002eeb0: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-0002eec0: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
-0002eed0: 6620 7365 6c66 2e68 6561 6465 7273 2069  f self.headers i
-0002eee0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0002eef0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
-0002ef00: 6865 6164 6572 7327 5d20 3d20 7365 6c66  headers'] = self
-0002ef10: 2e68 6561 6465 7273 0a20 2020 2020 2020  .headers.       
-0002ef20: 2069 6620 7365 6c66 2e73 7461 7475 735f   if self.status_
-0002ef30: 636f 6465 2069 7320 6e6f 7420 4e6f 6e65  code is not None
-0002ef40: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0002ef50: 7375 6c74 5b27 7374 6174 7573 436f 6465  sult['statusCode
-0002ef60: 275d 203d 2073 656c 662e 7374 6174 7573  '] = self.status
-0002ef70: 5f63 6f64 650a 2020 2020 2020 2020 6966  _code.        if
-0002ef80: 2073 656c 662e 626f 6479 2069 7320 6e6f   self.body is no
-0002ef90: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0002efa0: 2020 2020 7265 7375 6c74 5b27 626f 6479      result['body
-0002efb0: 275d 203d 2073 656c 662e 626f 6479 2e74  '] = self.body.t
-0002efc0: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
-0002efd0: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
-0002efe0: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
-0002eff0: 7365 6c66 2c20 6d3d 4e6f 6e65 293a 0a20  self, m=None):. 
-0002f000: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
-0002f010: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
-0002f020: 6620 6d2e 6765 7428 2768 6561 6465 7273  f m.get('headers
-0002f030: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
-0002f040: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0002f050: 2e68 6561 6465 7273 203d 206d 2e67 6574  .headers = m.get
-0002f060: 2827 6865 6164 6572 7327 290a 2020 2020  ('headers').    
-0002f070: 2020 2020 6966 206d 2e67 6574 2827 7374      if m.get('st
-0002f080: 6174 7573 436f 6465 2729 2069 7320 6e6f  atusCode') is no
-0002f090: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0002f0a0: 2020 2020 7365 6c66 2e73 7461 7475 735f      self.status_
-0002f0b0: 636f 6465 203d 206d 2e67 6574 2827 7374  code = m.get('st
-0002f0c0: 6174 7573 436f 6465 2729 0a20 2020 2020  atusCode').     
-0002f0d0: 2020 2069 6620 6d2e 6765 7428 2762 6f64     if m.get('bod
-0002f0e0: 7927 2920 6973 206e 6f74 204e 6f6e 653a  y') is not None:
-0002f0f0: 0a20 2020 2020 2020 2020 2020 2074 656d  .            tem
-0002f100: 705f 6d6f 6465 6c20 3d20 5570 6461 7465  p_model = Update
-0002f110: 4a6f 6252 6573 706f 6e73 6542 6f64 7928  JobResponseBody(
-0002f120: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-0002f130: 6c66 2e62 6f64 7920 3d20 7465 6d70 5f6d  lf.body = temp_m
-0002f140: 6f64 656c 2e66 726f 6d5f 6d61 7028 6d5b  odel.from_map(m[
-0002f150: 2762 6f64 7927 5d29 0a20 2020 2020 2020  'body']).       
-0002f160: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
-0002f170: 6c61 7373 2055 7064 6174 6554 656e 736f  lass UpdateTenso
-0002f180: 7262 6f61 7264 5265 7175 6573 7428 5465  rboardRequest(Te
-0002f190: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
-0002f1a0: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
-0002f1b0: 6d61 785f 7275 6e6e 696e 675f 7469 6d65  max_running_time
-0002f1c0: 5f6d 696e 7574 6573 3d4e 6f6e 652c 2077  _minutes=None, w
-0002f1d0: 6f72 6b73 7061 6365 5f69 643d 4e6f 6e65  orkspace_id=None
-0002f1e0: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-0002f1f0: 6d61 785f 7275 6e6e 696e 675f 7469 6d65  max_running_time
-0002f200: 5f6d 696e 7574 6573 203d 206d 6178 5f72  _minutes = max_r
-0002f210: 756e 6e69 6e67 5f74 696d 655f 6d69 6e75  unning_time_minu
-0002f220: 7465 7320 2023 2074 7970 653a 206c 6f6e  tes  # type: lon
-0002f230: 670a 2020 2020 2020 2020 7365 6c66 2e77  g.        self.w
-0002f240: 6f72 6b73 7061 6365 5f69 6420 3d20 776f  orkspace_id = wo
-0002f250: 726b 7370 6163 655f 6964 2020 2320 7479  rkspace_id  # ty
-0002f260: 7065 3a20 7374 720a 0a20 2020 2064 6566  pe: str..    def
-0002f270: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
-0002f280: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
-0002f290: 2020 2064 6566 2074 6f5f 6d61 7028 7365     def to_map(se
-0002f2a0: 6c66 293a 0a20 2020 2020 2020 205f 6d61  lf):.        _ma
-0002f2b0: 7020 3d20 7375 7065 7228 5570 6461 7465  p = super(Update
-0002f2c0: 5465 6e73 6f72 626f 6172 6452 6571 7565  TensorboardReque
-0002f2d0: 7374 2c20 7365 6c66 292e 746f 5f6d 6170  st, self).to_map
-0002f2e0: 2829 0a20 2020 2020 2020 2069 6620 5f6d  ().        if _m
-0002f2f0: 6170 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ap is not None:.
-0002f300: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0002f310: 726e 205f 6d61 700a 0a20 2020 2020 2020  rn _map..       
-0002f320: 2072 6573 756c 7420 3d20 6469 6374 2829   result = dict()
-0002f330: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0002f340: 2e6d 6178 5f72 756e 6e69 6e67 5f74 696d  .max_running_tim
-0002f350: 655f 6d69 6e75 7465 7320 6973 206e 6f74  e_minutes is not
-0002f360: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0002f370: 2020 2072 6573 756c 745b 274d 6178 5275     result['MaxRu
-0002f380: 6e6e 696e 6754 696d 654d 696e 7574 6573  nningTimeMinutes
-0002f390: 275d 203d 2073 656c 662e 6d61 785f 7275  '] = self.max_ru
-0002f3a0: 6e6e 696e 675f 7469 6d65 5f6d 696e 7574  nning_time_minut
-0002f3b0: 6573 0a20 2020 2020 2020 2069 6620 7365  es.        if se
-0002f3c0: 6c66 2e77 6f72 6b73 7061 6365 5f69 6420  lf.workspace_id 
-0002f3d0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0002f3e0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
-0002f3f0: 2757 6f72 6b73 7061 6365 4964 275d 203d  'WorkspaceId'] =
-0002f400: 2073 656c 662e 776f 726b 7370 6163 655f   self.workspace_
-0002f410: 6964 0a20 2020 2020 2020 2072 6574 7572  id.        retur
-0002f420: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
-0002f430: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
-0002f440: 206d 3d4e 6f6e 6529 3a0a 2020 2020 2020   m=None):.      
-0002f450: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
-0002f460: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-0002f470: 6574 2827 4d61 7852 756e 6e69 6e67 5469  et('MaxRunningTi
-0002f480: 6d65 4d69 6e75 7465 7327 2920 6973 206e  meMinutes') is n
-0002f490: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0002f4a0: 2020 2020 2073 656c 662e 6d61 785f 7275       self.max_ru
-0002f4b0: 6e6e 696e 675f 7469 6d65 5f6d 696e 7574  nning_time_minut
-0002f4c0: 6573 203d 206d 2e67 6574 2827 4d61 7852  es = m.get('MaxR
-0002f4d0: 756e 6e69 6e67 5469 6d65 4d69 6e75 7465  unningTimeMinute
-0002f4e0: 7327 290a 2020 2020 2020 2020 6966 206d  s').        if m
-0002f4f0: 2e67 6574 2827 576f 726b 7370 6163 6549  .get('WorkspaceI
-0002f500: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
-0002f510: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0002f520: 662e 776f 726b 7370 6163 655f 6964 203d  f.workspace_id =
-0002f530: 206d 2e67 6574 2827 576f 726b 7370 6163   m.get('Workspac
-0002f540: 6549 6427 290a 2020 2020 2020 2020 7265  eId').        re
-0002f550: 7475 726e 2073 656c 660a 0a0a 636c 6173  turn self...clas
-0002f560: 7320 5570 6461 7465 5465 6e73 6f72 626f  s UpdateTensorbo
-0002f570: 6172 6452 6573 706f 6e73 6542 6f64 7928  ardResponseBody(
-0002f580: 5465 614d 6f64 656c 293a 0a20 2020 2064  TeaModel):.    d
-0002f590: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-0002f5a0: 2c20 7265 7175 6573 745f 6964 3d4e 6f6e  , request_id=Non
-0002f5b0: 652c 2074 656e 736f 7262 6f61 7264 5f69  e, tensorboard_i
-0002f5c0: 643d 4e6f 6e65 293a 0a20 2020 2020 2020  d=None):.       
-0002f5d0: 2073 656c 662e 7265 7175 6573 745f 6964   self.request_id
-0002f5e0: 203d 2072 6571 7565 7374 5f69 6420 2023   = request_id  #
-0002f5f0: 2074 7970 653a 2073 7472 0a20 2020 2020   type: str.     
-0002f600: 2020 2073 656c 662e 7465 6e73 6f72 626f     self.tensorbo
-0002f610: 6172 645f 6964 203d 2074 656e 736f 7262  ard_id = tensorb
-0002f620: 6f61 7264 5f69 6420 2023 2074 7970 653a  oard_id  # type:
-0002f630: 2073 7472 0a0a 2020 2020 6465 6620 7661   str..    def va
-0002f640: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
-0002f650: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
-0002f660: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
-0002f670: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
-0002f680: 2073 7570 6572 2855 7064 6174 6554 656e   super(UpdateTen
-0002f690: 736f 7262 6f61 7264 5265 7370 6f6e 7365  sorboardResponse
-0002f6a0: 426f 6479 2c20 7365 6c66 292e 746f 5f6d  Body, self).to_m
-0002f6b0: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
-0002f6c0: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
-0002f6d0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0002f6e0: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
-0002f6f0: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
-0002f700: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
-0002f710: 6c66 2e72 6571 7565 7374 5f69 6420 6973  lf.request_id is
-0002f720: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0002f730: 2020 2020 2020 2072 6573 756c 745b 2752         result['R
-0002f740: 6571 7565 7374 4964 275d 203d 2073 656c  equestId'] = sel
-0002f750: 662e 7265 7175 6573 745f 6964 0a20 2020  f.request_id.   
-0002f760: 2020 2020 2069 6620 7365 6c66 2e74 656e       if self.ten
-0002f770: 736f 7262 6f61 7264 5f69 6420 6973 206e  sorboard_id is n
-0002f780: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0002f790: 2020 2020 2072 6573 756c 745b 2754 656e       result['Ten
-0002f7a0: 736f 7262 6f61 7264 4964 275d 203d 2073  sorboardId'] = s
-0002f7b0: 656c 662e 7465 6e73 6f72 626f 6172 645f  elf.tensorboard_
-0002f7c0: 6964 0a20 2020 2020 2020 2072 6574 7572  id.        retur
-0002f7d0: 6e20 7265 7375 6c74 0a0a 2020 2020 6465  n result..    de
-0002f7e0: 6620 6672 6f6d 5f6d 6170 2873 656c 662c  f from_map(self,
-0002f7f0: 206d 3d4e 6f6e 6529 3a0a 2020 2020 2020   m=None):.      
-0002f800: 2020 6d20 3d20 6d20 6f72 2064 6963 7428    m = m or dict(
-0002f810: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
-0002f820: 6574 2827 5265 7175 6573 7449 6427 2920  et('RequestId') 
-0002f830: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0002f840: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
-0002f850: 7175 6573 745f 6964 203d 206d 2e67 6574  quest_id = m.get
-0002f860: 2827 5265 7175 6573 7449 6427 290a 2020  ('RequestId').  
-0002f870: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
-0002f880: 5465 6e73 6f72 626f 6172 6449 6427 2920  TensorboardId') 
-0002f890: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0002f8a0: 2020 2020 2020 2020 2073 656c 662e 7465           self.te
-0002f8b0: 6e73 6f72 626f 6172 645f 6964 203d 206d  nsorboard_id = m
-0002f8c0: 2e67 6574 2827 5465 6e73 6f72 626f 6172  .get('Tensorboar
-0002f8d0: 6449 6427 290a 2020 2020 2020 2020 7265  dId').        re
-0002f8e0: 7475 726e 2073 656c 660a 0a0a 636c 6173  turn self...clas
-0002f8f0: 7320 5570 6461 7465 5465 6e73 6f72 626f  s UpdateTensorbo
-0002f900: 6172 6452 6573 706f 6e73 6528 5465 614d  ardResponse(TeaM
-0002f910: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
-0002f920: 5f69 6e69 745f 5f28 7365 6c66 2c20 6865  _init__(self, he
-0002f930: 6164 6572 733d 4e6f 6e65 2c20 7374 6174  aders=None, stat
-0002f940: 7573 5f63 6f64 653d 4e6f 6e65 2c20 626f  us_code=None, bo
-0002f950: 6479 3d4e 6f6e 6529 3a0a 2020 2020 2020  dy=None):.      
-0002f960: 2020 7365 6c66 2e68 6561 6465 7273 203d    self.headers =
-0002f970: 2068 6561 6465 7273 2020 2320 7479 7065   headers  # type
-0002f980: 3a20 6469 6374 5b73 7472 2c20 7374 725d  : dict[str, str]
-0002f990: 0a20 2020 2020 2020 2073 656c 662e 7374  .        self.st
-0002f9a0: 6174 7573 5f63 6f64 6520 3d20 7374 6174  atus_code = stat
-0002f9b0: 7573 5f63 6f64 6520 2023 2074 7970 653a  us_code  # type:
-0002f9c0: 2069 6e74 0a20 2020 2020 2020 2073 656c   int.        sel
-0002f9d0: 662e 626f 6479 203d 2062 6f64 7920 2023  f.body = body  #
-0002f9e0: 2074 7970 653a 2055 7064 6174 6554 656e   type: UpdateTen
-0002f9f0: 736f 7262 6f61 7264 5265 7370 6f6e 7365  sorboardResponse
-0002fa00: 426f 6479 0a0a 2020 2020 6465 6620 7661  Body..    def va
-0002fa10: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
-0002fa20: 2020 2020 2020 7365 6c66 2e76 616c 6964        self.valid
-0002fa30: 6174 655f 7265 7175 6972 6564 2873 656c  ate_required(sel
-0002fa40: 662e 6865 6164 6572 732c 2027 6865 6164  f.headers, 'head
-0002fa50: 6572 7327 290a 2020 2020 2020 2020 7365  ers').        se
-0002fa60: 6c66 2e76 616c 6964 6174 655f 7265 7175  lf.validate_requ
-0002fa70: 6972 6564 2873 656c 662e 7374 6174 7573  ired(self.status
-0002fa80: 5f63 6f64 652c 2027 7374 6174 7573 5f63  _code, 'status_c
-0002fa90: 6f64 6527 290a 2020 2020 2020 2020 7365  ode').        se
-0002faa0: 6c66 2e76 616c 6964 6174 655f 7265 7175  lf.validate_requ
-0002fab0: 6972 6564 2873 656c 662e 626f 6479 2c20  ired(self.body, 
-0002fac0: 2762 6f64 7927 290a 2020 2020 2020 2020  'body').        
-0002fad0: 6966 2073 656c 662e 626f 6479 3a0a 2020  if self.body:.  
-0002fae0: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
-0002faf0: 6f64 792e 7661 6c69 6461 7465 2829 0a0a  ody.validate()..
-0002fb00: 2020 2020 6465 6620 746f 5f6d 6170 2873      def to_map(s
-0002fb10: 656c 6629 3a0a 2020 2020 2020 2020 5f6d  elf):.        _m
-0002fb20: 6170 203d 2073 7570 6572 2855 7064 6174  ap = super(Updat
-0002fb30: 6554 656e 736f 7262 6f61 7264 5265 7370  eTensorboardResp
-0002fb40: 6f6e 7365 2c20 7365 6c66 292e 746f 5f6d  onse, self).to_m
-0002fb50: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
-0002fb60: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
-0002fb70: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0002fb80: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
-0002fb90: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
-0002fba0: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
-0002fbb0: 6c66 2e68 6561 6465 7273 2069 7320 6e6f  lf.headers is no
-0002fbc0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-0002fbd0: 2020 2020 7265 7375 6c74 5b27 6865 6164      result['head
-0002fbe0: 6572 7327 5d20 3d20 7365 6c66 2e68 6561  ers'] = self.hea
-0002fbf0: 6465 7273 0a20 2020 2020 2020 2069 6620  ders.        if 
-0002fc00: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
-0002fc10: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0002fc20: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0002fc30: 5b27 7374 6174 7573 436f 6465 275d 203d  ['statusCode'] =
-0002fc40: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
-0002fc50: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
-0002fc60: 662e 626f 6479 2069 7320 6e6f 7420 4e6f  f.body is not No
-0002fc70: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0002fc80: 7265 7375 6c74 5b27 626f 6479 275d 203d  result['body'] =
-0002fc90: 2073 656c 662e 626f 6479 2e74 6f5f 6d61   self.body.to_ma
-0002fca0: 7028 290a 2020 2020 2020 2020 7265 7475  p().        retu
-0002fcb0: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
-0002fcc0: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
-0002fcd0: 2c20 6d3d 4e6f 6e65 293a 0a20 2020 2020  , m=None):.     
-0002fce0: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
-0002fcf0: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
-0002fd00: 6765 7428 2768 6561 6465 7273 2729 2069  get('headers') i
-0002fd10: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0002fd20: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
-0002fd30: 6465 7273 203d 206d 2e67 6574 2827 6865  ders = m.get('he
-0002fd40: 6164 6572 7327 290a 2020 2020 2020 2020  aders').        
-0002fd50: 6966 206d 2e67 6574 2827 7374 6174 7573  if m.get('status
-0002fd60: 436f 6465 2729 2069 7320 6e6f 7420 4e6f  Code') is not No
-0002fd70: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-0002fd80: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
-0002fd90: 203d 206d 2e67 6574 2827 7374 6174 7573   = m.get('status
-0002fda0: 436f 6465 2729 0a20 2020 2020 2020 2069  Code').        i
-0002fdb0: 6620 6d2e 6765 7428 2762 6f64 7927 2920  f m.get('body') 
-0002fdc0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0002fdd0: 2020 2020 2020 2020 2074 656d 705f 6d6f           temp_mo
-0002fde0: 6465 6c20 3d20 5570 6461 7465 5465 6e73  del = UpdateTens
-0002fdf0: 6f72 626f 6172 6452 6573 706f 6e73 6542  orboardResponseB
-0002fe00: 6f64 7928 290a 2020 2020 2020 2020 2020  ody().          
-0002fe10: 2020 7365 6c66 2e62 6f64 7920 3d20 7465    self.body = te
-0002fe20: 6d70 5f6d 6f64 656c 2e66 726f 6d5f 6d61  mp_model.from_ma
-0002fe30: 7028 6d5b 2762 6f64 7927 5d29 0a20 2020  p(m['body']).   
-0002fe40: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-0002fe50: 0a0a 0a                                  ...
+00026bf0: 6c66 0a0a 0a63 6c61 7373 2047 6574 5765  lf...class GetWe
+00026c00: 6254 6572 6d69 6e61 6c52 6571 7565 7374  bTerminalRequest
+00026c10: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
+00026c20: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+00026c30: 662c 2070 6f64 5f75 6964 3d4e 6f6e 6529  f, pod_uid=None)
+00026c40: 3a0a 2020 2020 2020 2020 2320 506f 6420  :.        # Pod 
+00026c50: 5549 44e3 8082 0a20 2020 2020 2020 2073  UID....        s
+00026c60: 656c 662e 706f 645f 7569 6420 3d20 706f  elf.pod_uid = po
+00026c70: 645f 7569 6420 2023 2074 7970 653a 2073  d_uid  # type: s
+00026c80: 7472 0a0a 2020 2020 6465 6620 7661 6c69  tr..    def vali
+00026c90: 6461 7465 2873 656c 6629 3a0a 2020 2020  date(self):.    
+00026ca0: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
+00026cb0: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
+00026cc0: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
+00026cd0: 7570 6572 2847 6574 5765 6254 6572 6d69  uper(GetWebTermi
+00026ce0: 6e61 6c52 6571 7565 7374 2c20 7365 6c66  nalRequest, self
+00026cf0: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
+00026d00: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
+00026d10: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00026d20: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
+00026d30: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
+00026d40: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
+00026d50: 2069 6620 7365 6c66 2e70 6f64 5f75 6964   if self.pod_uid
+00026d60: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00026d70: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00026d80: 5b27 506f 6455 6964 275d 203d 2073 656c  ['PodUid'] = sel
+00026d90: 662e 706f 645f 7569 640a 2020 2020 2020  f.pod_uid.      
+00026da0: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
+00026db0: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
+00026dc0: 7028 7365 6c66 2c20 6d3d 4e6f 6e65 293a  p(self, m=None):
+00026dd0: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
+00026de0: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
+00026df0: 2069 6620 6d2e 6765 7428 2750 6f64 5569   if m.get('PodUi
+00026e00: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
+00026e10: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00026e20: 662e 706f 645f 7569 6420 3d20 6d2e 6765  f.pod_uid = m.ge
+00026e30: 7428 2750 6f64 5569 6427 290a 2020 2020  t('PodUid').    
+00026e40: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
+00026e50: 0a0a 636c 6173 7320 4765 7457 6562 5465  ..class GetWebTe
+00026e60: 726d 696e 616c 5265 7370 6f6e 7365 426f  rminalResponseBo
+00026e70: 6479 2854 6561 4d6f 6465 6c29 3a0a 2020  dy(TeaModel):.  
+00026e80: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
+00026e90: 656c 662c 2075 726c 3d4e 6f6e 652c 2072  elf, url=None, r
+00026ea0: 6571 7565 7374 5f69 643d 4e6f 6e65 293a  equest_id=None):
+00026eb0: 0a20 2020 2020 2020 2073 656c 662e 7572  .        self.ur
+00026ec0: 6c20 3d20 7572 6c20 2023 2074 7970 653a  l = url  # type:
+00026ed0: 2073 7472 0a20 2020 2020 2020 2073 656c   str.        sel
+00026ee0: 662e 7265 7175 6573 745f 6964 203d 2072  f.request_id = r
+00026ef0: 6571 7565 7374 5f69 6420 2023 2074 7970  equest_id  # typ
+00026f00: 653a 2073 7472 0a0a 2020 2020 6465 6620  e: str..    def 
+00026f10: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
+00026f20: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
+00026f30: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
+00026f40: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
+00026f50: 203d 2073 7570 6572 2847 6574 5765 6254   = super(GetWebT
+00026f60: 6572 6d69 6e61 6c52 6573 706f 6e73 6542  erminalResponseB
+00026f70: 6f64 792c 2073 656c 6629 2e74 6f5f 6d61  ody, self).to_ma
+00026f80: 7028 290a 2020 2020 2020 2020 6966 205f  p().        if _
+00026f90: 6d61 7020 6973 206e 6f74 204e 6f6e 653a  map is not None:
+00026fa0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00026fb0: 7572 6e20 5f6d 6170 0a0a 2020 2020 2020  urn _map..      
+00026fc0: 2020 7265 7375 6c74 203d 2064 6963 7428    result = dict(
+00026fd0: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+00026fe0: 662e 7572 6c20 6973 206e 6f74 204e 6f6e  f.url is not Non
+00026ff0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00027000: 6573 756c 745b 2755 524c 275d 203d 2073  esult['URL'] = s
+00027010: 656c 662e 7572 6c0a 2020 2020 2020 2020  elf.url.        
+00027020: 6966 2073 656c 662e 7265 7175 6573 745f  if self.request_
+00027030: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
+00027040: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00027050: 6c74 5b27 7265 7175 6573 7449 6427 5d20  lt['requestId'] 
+00027060: 3d20 7365 6c66 2e72 6571 7565 7374 5f69  = self.request_i
+00027070: 640a 2020 2020 2020 2020 7265 7475 726e  d.        return
+00027080: 2072 6573 756c 740a 0a20 2020 2064 6566   result..    def
+00027090: 2066 726f 6d5f 6d61 7028 7365 6c66 2c20   from_map(self, 
+000270a0: 6d3d 4e6f 6e65 293a 0a20 2020 2020 2020  m=None):.       
+000270b0: 206d 203d 206d 206f 7220 6469 6374 2829   m = m or dict()
+000270c0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+000270d0: 7428 2755 524c 2729 2069 7320 6e6f 7420  t('URL') is not 
+000270e0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000270f0: 2020 7365 6c66 2e75 726c 203d 206d 2e67    self.url = m.g
+00027100: 6574 2827 5552 4c27 290a 2020 2020 2020  et('URL').      
+00027110: 2020 6966 206d 2e67 6574 2827 7265 7175    if m.get('requ
+00027120: 6573 7449 6427 2920 6973 206e 6f74 204e  estId') is not N
+00027130: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00027140: 2073 656c 662e 7265 7175 6573 745f 6964   self.request_id
+00027150: 203d 206d 2e67 6574 2827 7265 7175 6573   = m.get('reques
+00027160: 7449 6427 290a 2020 2020 2020 2020 7265  tId').        re
+00027170: 7475 726e 2073 656c 660a 0a0a 636c 6173  turn self...clas
+00027180: 7320 4765 7457 6562 5465 726d 696e 616c  s GetWebTerminal
+00027190: 5265 7370 6f6e 7365 2854 6561 4d6f 6465  Response(TeaMode
+000271a0: 6c29 3a0a 2020 2020 6465 6620 5f5f 696e  l):.    def __in
+000271b0: 6974 5f5f 2873 656c 662c 2068 6561 6465  it__(self, heade
+000271c0: 7273 3d4e 6f6e 652c 2073 7461 7475 735f  rs=None, status_
+000271d0: 636f 6465 3d4e 6f6e 652c 2062 6f64 793d  code=None, body=
+000271e0: 4e6f 6e65 293a 0a20 2020 2020 2020 2073  None):.        s
+000271f0: 656c 662e 6865 6164 6572 7320 3d20 6865  elf.headers = he
+00027200: 6164 6572 7320 2023 2074 7970 653a 2064  aders  # type: d
+00027210: 6963 745b 7374 722c 2073 7472 5d0a 2020  ict[str, str].  
+00027220: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
+00027230: 735f 636f 6465 203d 2073 7461 7475 735f  s_code = status_
+00027240: 636f 6465 2020 2320 7479 7065 3a20 696e  code  # type: in
+00027250: 740a 2020 2020 2020 2020 7365 6c66 2e62  t.        self.b
+00027260: 6f64 7920 3d20 626f 6479 2020 2320 7479  ody = body  # ty
+00027270: 7065 3a20 4765 7457 6562 5465 726d 696e  pe: GetWebTermin
+00027280: 616c 5265 7370 6f6e 7365 426f 6479 0a0a  alResponseBody..
+00027290: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
+000272a0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+000272b0: 7365 6c66 2e76 616c 6964 6174 655f 7265  self.validate_re
+000272c0: 7175 6972 6564 2873 656c 662e 6865 6164  quired(self.head
+000272d0: 6572 732c 2027 6865 6164 6572 7327 290a  ers, 'headers').
+000272e0: 2020 2020 2020 2020 7365 6c66 2e76 616c          self.val
+000272f0: 6964 6174 655f 7265 7175 6972 6564 2873  idate_required(s
+00027300: 656c 662e 7374 6174 7573 5f63 6f64 652c  elf.status_code,
+00027310: 2027 7374 6174 7573 5f63 6f64 6527 290a   'status_code').
+00027320: 2020 2020 2020 2020 7365 6c66 2e76 616c          self.val
+00027330: 6964 6174 655f 7265 7175 6972 6564 2873  idate_required(s
+00027340: 656c 662e 626f 6479 2c20 2762 6f64 7927  elf.body, 'body'
+00027350: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
+00027360: 662e 626f 6479 3a0a 2020 2020 2020 2020  f.body:.        
+00027370: 2020 2020 7365 6c66 2e62 6f64 792e 7661      self.body.va
+00027380: 6c69 6461 7465 2829 0a0a 2020 2020 6465  lidate()..    de
+00027390: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
+000273a0: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
+000273b0: 7570 6572 2847 6574 5765 6254 6572 6d69  uper(GetWebTermi
+000273c0: 6e61 6c52 6573 706f 6e73 652c 2073 656c  nalResponse, sel
+000273d0: 6629 2e74 6f5f 6d61 7028 290a 2020 2020  f).to_map().    
+000273e0: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
+000273f0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00027400: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
+00027410: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
+00027420: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
+00027430: 2020 6966 2073 656c 662e 6865 6164 6572    if self.header
+00027440: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
+00027450: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00027460: 745b 2768 6561 6465 7273 275d 203d 2073  t['headers'] = s
+00027470: 656c 662e 6865 6164 6572 730a 2020 2020  elf.headers.    
+00027480: 2020 2020 6966 2073 656c 662e 7374 6174      if self.stat
+00027490: 7573 5f63 6f64 6520 6973 206e 6f74 204e  us_code is not N
+000274a0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000274b0: 2072 6573 756c 745b 2773 7461 7475 7343   result['statusC
+000274c0: 6f64 6527 5d20 3d20 7365 6c66 2e73 7461  ode'] = self.sta
+000274d0: 7475 735f 636f 6465 0a20 2020 2020 2020  tus_code.       
+000274e0: 2069 6620 7365 6c66 2e62 6f64 7920 6973   if self.body is
+000274f0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00027500: 2020 2020 2020 2072 6573 756c 745b 2762         result['b
+00027510: 6f64 7927 5d20 3d20 7365 6c66 2e62 6f64  ody'] = self.bod
+00027520: 792e 746f 5f6d 6170 2829 0a20 2020 2020  y.to_map().     
+00027530: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
+00027540: 0a0a 2020 2020 6465 6620 6672 6f6d 5f6d  ..    def from_m
+00027550: 6170 2873 656c 662c 206d 3d4e 6f6e 6529  ap(self, m=None)
+00027560: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
+00027570: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
+00027580: 2020 6966 206d 2e67 6574 2827 6865 6164    if m.get('head
+00027590: 6572 7327 2920 6973 206e 6f74 204e 6f6e  ers') is not Non
+000275a0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+000275b0: 656c 662e 6865 6164 6572 7320 3d20 6d2e  elf.headers = m.
+000275c0: 6765 7428 2768 6561 6465 7273 2729 0a20  get('headers'). 
+000275d0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+000275e0: 2773 7461 7475 7343 6f64 6527 2920 6973  'statusCode') is
+000275f0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00027600: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
+00027610: 7573 5f63 6f64 6520 3d20 6d2e 6765 7428  us_code = m.get(
+00027620: 2773 7461 7475 7343 6f64 6527 290a 2020  'statusCode').  
+00027630: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00027640: 626f 6479 2729 2069 7320 6e6f 7420 4e6f  body') is not No
+00027650: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00027660: 7465 6d70 5f6d 6f64 656c 203d 2047 6574  temp_model = Get
+00027670: 5765 6254 6572 6d69 6e61 6c52 6573 706f  WebTerminalRespo
+00027680: 6e73 6542 6f64 7928 290a 2020 2020 2020  nseBody().      
+00027690: 2020 2020 2020 7365 6c66 2e62 6f64 7920        self.body 
+000276a0: 3d20 7465 6d70 5f6d 6f64 656c 2e66 726f  = temp_model.fro
+000276b0: 6d5f 6d61 7028 6d5b 2762 6f64 7927 5d29  m_map(m['body'])
+000276c0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000276d0: 7365 6c66 0a0a 0a63 6c61 7373 204c 6973  self...class Lis
+000276e0: 7445 6373 5370 6563 7352 6571 7565 7374  tEcsSpecsRequest
+000276f0: 2854 6561 4d6f 6465 6c29 3a0a 2020 2020  (TeaModel):.    
+00027700: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+00027710: 662c 2061 6363 656c 6572 6174 6f72 5f74  f, accelerator_t
+00027720: 7970 653d 4e6f 6e65 2c20 6f72 6465 723d  ype=None, order=
+00027730: 4e6f 6e65 2c20 7061 6765 5f6e 756d 6265  None, page_numbe
+00027740: 723d 4e6f 6e65 2c20 7061 6765 5f73 697a  r=None, page_siz
+00027750: 653d 4e6f 6e65 2c20 736f 7274 5f62 793d  e=None, sort_by=
+00027760: 4e6f 6e65 293a 0a20 2020 2020 2020 2073  None):.        s
+00027770: 656c 662e 6163 6365 6c65 7261 746f 725f  elf.accelerator_
+00027780: 7479 7065 203d 2061 6363 656c 6572 6174  type = accelerat
+00027790: 6f72 5f74 7970 6520 2023 2074 7970 653a  or_type  # type:
+000277a0: 2073 7472 0a20 2020 2020 2020 2073 656c   str.        sel
+000277b0: 662e 6f72 6465 7220 3d20 6f72 6465 7220  f.order = order 
+000277c0: 2023 2074 7970 653a 2073 7472 0a20 2020   # type: str.   
+000277d0: 2020 2020 2073 656c 662e 7061 6765 5f6e       self.page_n
+000277e0: 756d 6265 7220 3d20 7061 6765 5f6e 756d  umber = page_num
+000277f0: 6265 7220 2023 2074 7970 653a 2069 6e74  ber  # type: int
+00027800: 0a20 2020 2020 2020 2073 656c 662e 7061  .        self.pa
+00027810: 6765 5f73 697a 6520 3d20 7061 6765 5f73  ge_size = page_s
+00027820: 697a 6520 2023 2074 7970 653a 2069 6e74  ize  # type: int
+00027830: 0a20 2020 2020 2020 2073 656c 662e 736f  .        self.so
+00027840: 7274 5f62 7920 3d20 736f 7274 5f62 7920  rt_by = sort_by 
+00027850: 2023 2074 7970 653a 2073 7472 0a0a 2020   # type: str..  
+00027860: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
+00027870: 656c 6629 3a0a 2020 2020 2020 2020 7061  elf):.        pa
+00027880: 7373 0a0a 2020 2020 6465 6620 746f 5f6d  ss..    def to_m
+00027890: 6170 2873 656c 6629 3a0a 2020 2020 2020  ap(self):.      
+000278a0: 2020 5f6d 6170 203d 2073 7570 6572 284c    _map = super(L
+000278b0: 6973 7445 6373 5370 6563 7352 6571 7565  istEcsSpecsReque
+000278c0: 7374 2c20 7365 6c66 292e 746f 5f6d 6170  st, self).to_map
+000278d0: 2829 0a20 2020 2020 2020 2069 6620 5f6d  ().        if _m
+000278e0: 6170 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ap is not None:.
+000278f0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00027900: 726e 205f 6d61 700a 0a20 2020 2020 2020  rn _map..       
+00027910: 2072 6573 756c 7420 3d20 6469 6374 2829   result = dict()
+00027920: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00027930: 2e61 6363 656c 6572 6174 6f72 5f74 7970  .accelerator_typ
+00027940: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
+00027950: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00027960: 745b 2741 6363 656c 6572 6174 6f72 5479  t['AcceleratorTy
+00027970: 7065 275d 203d 2073 656c 662e 6163 6365  pe'] = self.acce
+00027980: 6c65 7261 746f 725f 7479 7065 0a20 2020  lerator_type.   
+00027990: 2020 2020 2069 6620 7365 6c66 2e6f 7264       if self.ord
+000279a0: 6572 2069 7320 6e6f 7420 4e6f 6e65 3a0a  er is not None:.
+000279b0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+000279c0: 6c74 5b27 4f72 6465 7227 5d20 3d20 7365  lt['Order'] = se
+000279d0: 6c66 2e6f 7264 6572 0a20 2020 2020 2020  lf.order.       
+000279e0: 2069 6620 7365 6c66 2e70 6167 655f 6e75   if self.page_nu
+000279f0: 6d62 6572 2069 7320 6e6f 7420 4e6f 6e65  mber is not None
+00027a00: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00027a10: 7375 6c74 5b27 5061 6765 4e75 6d62 6572  sult['PageNumber
+00027a20: 275d 203d 2073 656c 662e 7061 6765 5f6e  '] = self.page_n
+00027a30: 756d 6265 720a 2020 2020 2020 2020 6966  umber.        if
+00027a40: 2073 656c 662e 7061 6765 5f73 697a 6520   self.page_size 
+00027a50: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00027a60: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00027a70: 2750 6167 6553 697a 6527 5d20 3d20 7365  'PageSize'] = se
+00027a80: 6c66 2e70 6167 655f 7369 7a65 0a20 2020  lf.page_size.   
+00027a90: 2020 2020 2069 6620 7365 6c66 2e73 6f72       if self.sor
+00027aa0: 745f 6279 2069 7320 6e6f 7420 4e6f 6e65  t_by is not None
+00027ab0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00027ac0: 7375 6c74 5b27 536f 7274 4279 275d 203d  sult['SortBy'] =
+00027ad0: 2073 656c 662e 736f 7274 5f62 790a 2020   self.sort_by.  
+00027ae0: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+00027af0: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
+00027b00: 6d5f 6d61 7028 7365 6c66 2c20 6d3d 4e6f  m_map(self, m=No
+00027b10: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
+00027b20: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
+00027b30: 2020 2020 2069 6620 6d2e 6765 7428 2741       if m.get('A
+00027b40: 6363 656c 6572 6174 6f72 5479 7065 2729  cceleratorType')
+00027b50: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00027b60: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00027b70: 6363 656c 6572 6174 6f72 5f74 7970 6520  ccelerator_type 
+00027b80: 3d20 6d2e 6765 7428 2741 6363 656c 6572  = m.get('Acceler
+00027b90: 6174 6f72 5479 7065 2729 0a20 2020 2020  atorType').     
+00027ba0: 2020 2069 6620 6d2e 6765 7428 274f 7264     if m.get('Ord
+00027bb0: 6572 2729 2069 7320 6e6f 7420 4e6f 6e65  er') is not None
+00027bc0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00027bd0: 6c66 2e6f 7264 6572 203d 206d 2e67 6574  lf.order = m.get
+00027be0: 2827 4f72 6465 7227 290a 2020 2020 2020  ('Order').      
+00027bf0: 2020 6966 206d 2e67 6574 2827 5061 6765    if m.get('Page
+00027c00: 4e75 6d62 6572 2729 2069 7320 6e6f 7420  Number') is not 
+00027c10: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00027c20: 2020 7365 6c66 2e70 6167 655f 6e75 6d62    self.page_numb
+00027c30: 6572 203d 206d 2e67 6574 2827 5061 6765  er = m.get('Page
+00027c40: 4e75 6d62 6572 2729 0a20 2020 2020 2020  Number').       
+00027c50: 2069 6620 6d2e 6765 7428 2750 6167 6553   if m.get('PageS
+00027c60: 697a 6527 2920 6973 206e 6f74 204e 6f6e  ize') is not Non
+00027c70: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00027c80: 656c 662e 7061 6765 5f73 697a 6520 3d20  elf.page_size = 
+00027c90: 6d2e 6765 7428 2750 6167 6553 697a 6527  m.get('PageSize'
+00027ca0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+00027cb0: 6574 2827 536f 7274 4279 2729 2069 7320  et('SortBy') is 
+00027cc0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00027cd0: 2020 2020 2020 7365 6c66 2e73 6f72 745f        self.sort_
+00027ce0: 6279 203d 206d 2e67 6574 2827 536f 7274  by = m.get('Sort
+00027cf0: 4279 2729 0a20 2020 2020 2020 2072 6574  By').        ret
+00027d00: 7572 6e20 7365 6c66 0a0a 0a63 6c61 7373  urn self...class
+00027d10: 204c 6973 7445 6373 5370 6563 7352 6573   ListEcsSpecsRes
+00027d20: 706f 6e73 6542 6f64 7928 5465 614d 6f64  ponseBody(TeaMod
+00027d30: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
+00027d40: 6e69 745f 5f28 7365 6c66 2c20 6563 735f  nit__(self, ecs_
+00027d50: 7370 6563 733d 4e6f 6e65 2c20 7265 7175  specs=None, requ
+00027d60: 6573 745f 6964 3d4e 6f6e 652c 2074 6f74  est_id=None, tot
+00027d70: 616c 5f63 6f75 6e74 3d4e 6f6e 6529 3a0a  al_count=None):.
+00027d80: 2020 2020 2020 2020 7365 6c66 2e65 6373          self.ecs
+00027d90: 5f73 7065 6373 203d 2065 6373 5f73 7065  _specs = ecs_spe
+00027da0: 6373 2020 2320 7479 7065 3a20 6c69 7374  cs  # type: list
+00027db0: 5b45 6373 5370 6563 5d0a 2020 2020 2020  [EcsSpec].      
+00027dc0: 2020 7365 6c66 2e72 6571 7565 7374 5f69    self.request_i
+00027dd0: 6420 3d20 7265 7175 6573 745f 6964 2020  d = request_id  
+00027de0: 2320 7479 7065 3a20 7374 720a 2020 2020  # type: str.    
+00027df0: 2020 2020 7365 6c66 2e74 6f74 616c 5f63      self.total_c
+00027e00: 6f75 6e74 203d 2074 6f74 616c 5f63 6f75  ount = total_cou
+00027e10: 6e74 2020 2320 7479 7065 3a20 6c6f 6e67  nt  # type: long
+00027e20: 0a0a 2020 2020 6465 6620 7661 6c69 6461  ..    def valida
+00027e30: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
+00027e40: 2020 6966 2073 656c 662e 6563 735f 7370    if self.ecs_sp
+00027e50: 6563 733a 0a20 2020 2020 2020 2020 2020  ecs:.           
+00027e60: 2066 6f72 206b 2069 6e20 7365 6c66 2e65   for k in self.e
+00027e70: 6373 5f73 7065 6373 3a0a 2020 2020 2020  cs_specs:.      
+00027e80: 2020 2020 2020 2020 2020 6966 206b 3a0a            if k:.
+00027e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027ea0: 2020 2020 6b2e 7661 6c69 6461 7465 2829      k.validate()
+00027eb0: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
+00027ec0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00027ed0: 5f6d 6170 203d 2073 7570 6572 284c 6973  _map = super(Lis
+00027ee0: 7445 6373 5370 6563 7352 6573 706f 6e73  tEcsSpecsRespons
+00027ef0: 6542 6f64 792c 2073 656c 6629 2e74 6f5f  eBody, self).to_
+00027f00: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
+00027f10: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
+00027f20: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00027f30: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
+00027f40: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
+00027f50: 7428 290a 2020 2020 2020 2020 7265 7375  t().        resu
+00027f60: 6c74 5b27 4563 7353 7065 6373 275d 203d  lt['EcsSpecs'] =
+00027f70: 205b 5d0a 2020 2020 2020 2020 6966 2073   [].        if s
+00027f80: 656c 662e 6563 735f 7370 6563 7320 6973  elf.ecs_specs is
+00027f90: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00027fa0: 2020 2020 2020 2066 6f72 206b 2069 6e20         for k in 
+00027fb0: 7365 6c66 2e65 6373 5f73 7065 6373 3a0a  self.ecs_specs:.
+00027fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027fd0: 7265 7375 6c74 5b27 4563 7353 7065 6373  result['EcsSpecs
+00027fe0: 275d 2e61 7070 656e 6428 6b2e 746f 5f6d  '].append(k.to_m
+00027ff0: 6170 2829 2069 6620 6b20 656c 7365 204e  ap() if k else N
+00028000: 6f6e 6529 0a20 2020 2020 2020 2069 6620  one).        if 
+00028010: 7365 6c66 2e72 6571 7565 7374 5f69 6420  self.request_id 
+00028020: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00028030: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00028040: 2752 6571 7565 7374 4964 275d 203d 2073  'RequestId'] = s
+00028050: 656c 662e 7265 7175 6573 745f 6964 0a20  elf.request_id. 
+00028060: 2020 2020 2020 2069 6620 7365 6c66 2e74         if self.t
+00028070: 6f74 616c 5f63 6f75 6e74 2069 7320 6e6f  otal_count is no
+00028080: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00028090: 2020 2020 7265 7375 6c74 5b27 546f 7461      result['Tota
+000280a0: 6c43 6f75 6e74 275d 203d 2073 656c 662e  lCount'] = self.
+000280b0: 746f 7461 6c5f 636f 756e 740a 2020 2020  total_count.    
+000280c0: 2020 2020 7265 7475 726e 2072 6573 756c      return resul
+000280d0: 740a 0a20 2020 2064 6566 2066 726f 6d5f  t..    def from_
+000280e0: 6d61 7028 7365 6c66 2c20 6d3d 4e6f 6e65  map(self, m=None
+000280f0: 293a 0a20 2020 2020 2020 206d 203d 206d  ):.        m = m
+00028100: 206f 7220 6469 6374 2829 0a20 2020 2020   or dict().     
+00028110: 2020 2073 656c 662e 6563 735f 7370 6563     self.ecs_spec
+00028120: 7320 3d20 5b5d 0a20 2020 2020 2020 2069  s = [].        i
+00028130: 6620 6d2e 6765 7428 2745 6373 5370 6563  f m.get('EcsSpec
+00028140: 7327 2920 6973 206e 6f74 204e 6f6e 653a  s') is not None:
+00028150: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00028160: 206b 2069 6e20 6d2e 6765 7428 2745 6373   k in m.get('Ecs
+00028170: 5370 6563 7327 293a 0a20 2020 2020 2020  Specs'):.       
+00028180: 2020 2020 2020 2020 2074 656d 705f 6d6f           temp_mo
+00028190: 6465 6c20 3d20 4563 7353 7065 6328 290a  del = EcsSpec().
+000281a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000281b0: 7365 6c66 2e65 6373 5f73 7065 6373 2e61  self.ecs_specs.a
+000281c0: 7070 656e 6428 7465 6d70 5f6d 6f64 656c  ppend(temp_model
+000281d0: 2e66 726f 6d5f 6d61 7028 6b29 290a 2020  .from_map(k)).  
+000281e0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+000281f0: 5265 7175 6573 7449 6427 2920 6973 206e  RequestId') is n
+00028200: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00028210: 2020 2020 2073 656c 662e 7265 7175 6573       self.reques
+00028220: 745f 6964 203d 206d 2e67 6574 2827 5265  t_id = m.get('Re
+00028230: 7175 6573 7449 6427 290a 2020 2020 2020  questId').      
+00028240: 2020 6966 206d 2e67 6574 2827 546f 7461    if m.get('Tota
+00028250: 6c43 6f75 6e74 2729 2069 7320 6e6f 7420  lCount') is not 
+00028260: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00028270: 2020 7365 6c66 2e74 6f74 616c 5f63 6f75    self.total_cou
+00028280: 6e74 203d 206d 2e67 6574 2827 546f 7461  nt = m.get('Tota
+00028290: 6c43 6f75 6e74 2729 0a20 2020 2020 2020  lCount').       
+000282a0: 2072 6574 7572 6e20 7365 6c66 0a0a 0a63   return self...c
+000282b0: 6c61 7373 204c 6973 7445 6373 5370 6563  lass ListEcsSpec
+000282c0: 7352 6573 706f 6e73 6528 5465 614d 6f64  sResponse(TeaMod
+000282d0: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
+000282e0: 6e69 745f 5f28 7365 6c66 2c20 6865 6164  nit__(self, head
+000282f0: 6572 733d 4e6f 6e65 2c20 7374 6174 7573  ers=None, status
+00028300: 5f63 6f64 653d 4e6f 6e65 2c20 626f 6479  _code=None, body
+00028310: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
+00028320: 7365 6c66 2e68 6561 6465 7273 203d 2068  self.headers = h
+00028330: 6561 6465 7273 2020 2320 7479 7065 3a20  eaders  # type: 
+00028340: 6469 6374 5b73 7472 2c20 7374 725d 0a20  dict[str, str]. 
+00028350: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
+00028360: 7573 5f63 6f64 6520 3d20 7374 6174 7573  us_code = status
+00028370: 5f63 6f64 6520 2023 2074 7970 653a 2069  _code  # type: i
+00028380: 6e74 0a20 2020 2020 2020 2073 656c 662e  nt.        self.
+00028390: 626f 6479 203d 2062 6f64 7920 2023 2074  body = body  # t
+000283a0: 7970 653a 204c 6973 7445 6373 5370 6563  ype: ListEcsSpec
+000283b0: 7352 6573 706f 6e73 6542 6f64 790a 0a20  sResponseBody.. 
+000283c0: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
+000283d0: 7365 6c66 293a 0a20 2020 2020 2020 2073  self):.        s
+000283e0: 656c 662e 7661 6c69 6461 7465 5f72 6571  elf.validate_req
+000283f0: 7569 7265 6428 7365 6c66 2e68 6561 6465  uired(self.heade
+00028400: 7273 2c20 2768 6561 6465 7273 2729 0a20  rs, 'headers'). 
+00028410: 2020 2020 2020 2073 656c 662e 7661 6c69         self.vali
+00028420: 6461 7465 5f72 6571 7569 7265 6428 7365  date_required(se
+00028430: 6c66 2e73 7461 7475 735f 636f 6465 2c20  lf.status_code, 
+00028440: 2773 7461 7475 735f 636f 6465 2729 0a20  'status_code'). 
+00028450: 2020 2020 2020 2073 656c 662e 7661 6c69         self.vali
+00028460: 6461 7465 5f72 6571 7569 7265 6428 7365  date_required(se
+00028470: 6c66 2e62 6f64 792c 2027 626f 6479 2729  lf.body, 'body')
+00028480: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00028490: 2e62 6f64 793a 0a20 2020 2020 2020 2020  .body:.         
+000284a0: 2020 2073 656c 662e 626f 6479 2e76 616c     self.body.val
+000284b0: 6964 6174 6528 290a 0a20 2020 2064 6566  idate()..    def
+000284c0: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
+000284d0: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
+000284e0: 7065 7228 4c69 7374 4563 7353 7065 6373  per(ListEcsSpecs
+000284f0: 5265 7370 6f6e 7365 2c20 7365 6c66 292e  Response, self).
+00028500: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
+00028510: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
+00028520: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00028530: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
+00028540: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+00028550: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+00028560: 6620 7365 6c66 2e68 6561 6465 7273 2069  f self.headers i
+00028570: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00028580: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+00028590: 6865 6164 6572 7327 5d20 3d20 7365 6c66  headers'] = self
+000285a0: 2e68 6561 6465 7273 0a20 2020 2020 2020  .headers.       
+000285b0: 2069 6620 7365 6c66 2e73 7461 7475 735f   if self.status_
+000285c0: 636f 6465 2069 7320 6e6f 7420 4e6f 6e65  code is not None
+000285d0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+000285e0: 7375 6c74 5b27 7374 6174 7573 436f 6465  sult['statusCode
+000285f0: 275d 203d 2073 656c 662e 7374 6174 7573  '] = self.status
+00028600: 5f63 6f64 650a 2020 2020 2020 2020 6966  _code.        if
+00028610: 2073 656c 662e 626f 6479 2069 7320 6e6f   self.body is no
+00028620: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00028630: 2020 2020 7265 7375 6c74 5b27 626f 6479      result['body
+00028640: 275d 203d 2073 656c 662e 626f 6479 2e74  '] = self.body.t
+00028650: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
+00028660: 7265 7475 726e 2072 6573 756c 740a 0a20  return result.. 
+00028670: 2020 2064 6566 2066 726f 6d5f 6d61 7028     def from_map(
+00028680: 7365 6c66 2c20 6d3d 4e6f 6e65 293a 0a20  self, m=None):. 
+00028690: 2020 2020 2020 206d 203d 206d 206f 7220         m = m or 
+000286a0: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+000286b0: 6620 6d2e 6765 7428 2768 6561 6465 7273  f m.get('headers
+000286c0: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+000286d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000286e0: 2e68 6561 6465 7273 203d 206d 2e67 6574  .headers = m.get
+000286f0: 2827 6865 6164 6572 7327 290a 2020 2020  ('headers').    
+00028700: 2020 2020 6966 206d 2e67 6574 2827 7374      if m.get('st
+00028710: 6174 7573 436f 6465 2729 2069 7320 6e6f  atusCode') is no
+00028720: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00028730: 2020 2020 7365 6c66 2e73 7461 7475 735f      self.status_
+00028740: 636f 6465 203d 206d 2e67 6574 2827 7374  code = m.get('st
+00028750: 6174 7573 436f 6465 2729 0a20 2020 2020  atusCode').     
+00028760: 2020 2069 6620 6d2e 6765 7428 2762 6f64     if m.get('bod
+00028770: 7927 2920 6973 206e 6f74 204e 6f6e 653a  y') is not None:
+00028780: 0a20 2020 2020 2020 2020 2020 2074 656d  .            tem
+00028790: 705f 6d6f 6465 6c20 3d20 4c69 7374 4563  p_model = ListEc
+000287a0: 7353 7065 6373 5265 7370 6f6e 7365 426f  sSpecsResponseBo
+000287b0: 6479 2829 0a20 2020 2020 2020 2020 2020  dy().           
+000287c0: 2073 656c 662e 626f 6479 203d 2074 656d   self.body = tem
+000287d0: 705f 6d6f 6465 6c2e 6672 6f6d 5f6d 6170  p_model.from_map
+000287e0: 286d 5b27 626f 6479 275d 290a 2020 2020  (m['body']).    
+000287f0: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
+00028800: 0a0a 636c 6173 7320 4c69 7374 4a6f 6273  ..class ListJobs
+00028810: 5265 7175 6573 7428 5465 614d 6f64 656c  Request(TeaModel
+00028820: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
+00028830: 745f 5f28 7365 6c66 2c20 6275 7369 6e65  t__(self, busine
+00028840: 7373 5f75 7365 725f 6964 3d4e 6f6e 652c  ss_user_id=None,
+00028850: 2063 616c 6c65 723d 4e6f 6e65 2c20 6469   caller=None, di
+00028860: 7370 6c61 795f 6e61 6d65 3d4e 6f6e 652c  splay_name=None,
+00028870: 2065 6e64 5f74 696d 653d 4e6f 6e65 2c0a   end_time=None,.
+00028880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00028890: 2066 726f 6d5f 616c 6c5f 776f 726b 7370   from_all_worksp
+000288a0: 6163 6573 3d4e 6f6e 652c 206a 6f62 5f69  aces=None, job_i
+000288b0: 643d 4e6f 6e65 2c20 6a6f 625f 7479 7065  d=None, job_type
+000288c0: 3d4e 6f6e 652c 206f 7264 6572 3d4e 6f6e  =None, order=Non
+000288d0: 652c 2070 6167 655f 6e75 6d62 6572 3d4e  e, page_number=N
+000288e0: 6f6e 652c 2070 6167 655f 7369 7a65 3d4e  one, page_size=N
+000288f0: 6f6e 652c 2070 6970 656c 696e 655f 6964  one, pipeline_id
+00028900: 3d4e 6f6e 652c 0a20 2020 2020 2020 2020  =None,.         
+00028910: 2020 2020 2020 2020 7265 736f 7572 6365          resource
+00028920: 5f69 643d 4e6f 6e65 2c20 7368 6f77 5f6f  _id=None, show_o
+00028930: 776e 3d4e 6f6e 652c 2073 6f72 745f 6279  wn=None, sort_by
+00028940: 3d4e 6f6e 652c 2073 7461 7274 5f74 696d  =None, start_tim
+00028950: 653d 4e6f 6e65 2c20 7374 6174 7573 3d4e  e=None, status=N
+00028960: 6f6e 652c 2074 6167 733d 4e6f 6e65 2c20  one, tags=None, 
+00028970: 776f 726b 7370 6163 655f 6964 3d4e 6f6e  workspace_id=Non
+00028980: 6529 3a0a 2020 2020 2020 2020 7365 6c66  e):.        self
+00028990: 2e62 7573 696e 6573 735f 7573 6572 5f69  .business_user_i
+000289a0: 6420 3d20 6275 7369 6e65 7373 5f75 7365  d = business_use
+000289b0: 725f 6964 2020 2320 7479 7065 3a20 7374  r_id  # type: st
+000289c0: 720a 2020 2020 2020 2020 7365 6c66 2e63  r.        self.c
+000289d0: 616c 6c65 7220 3d20 6361 6c6c 6572 2020  aller = caller  
+000289e0: 2320 7479 7065 3a20 7374 720a 2020 2020  # type: str.    
+000289f0: 2020 2020 7365 6c66 2e64 6973 706c 6179      self.display
+00028a00: 5f6e 616d 6520 3d20 6469 7370 6c61 795f  _name = display_
+00028a10: 6e61 6d65 2020 2320 7479 7065 3a20 7374  name  # type: st
+00028a20: 720a 2020 2020 2020 2020 7365 6c66 2e65  r.        self.e
+00028a30: 6e64 5f74 696d 6520 3d20 656e 645f 7469  nd_time = end_ti
+00028a40: 6d65 2020 2320 7479 7065 3a20 7374 720a  me  # type: str.
+00028a50: 2020 2020 2020 2020 7365 6c66 2e66 726f          self.fro
+00028a60: 6d5f 616c 6c5f 776f 726b 7370 6163 6573  m_all_workspaces
+00028a70: 203d 2066 726f 6d5f 616c 6c5f 776f 726b   = from_all_work
+00028a80: 7370 6163 6573 2020 2320 7479 7065 3a20  spaces  # type: 
+00028a90: 626f 6f6c 0a20 2020 2020 2020 2073 656c  bool.        sel
+00028aa0: 662e 6a6f 625f 6964 203d 206a 6f62 5f69  f.job_id = job_i
+00028ab0: 6420 2023 2074 7970 653a 2073 7472 0a20  d  # type: str. 
+00028ac0: 2020 2020 2020 2073 656c 662e 6a6f 625f         self.job_
+00028ad0: 7479 7065 203d 206a 6f62 5f74 7970 6520  type = job_type 
+00028ae0: 2023 2074 7970 653a 2073 7472 0a20 2020   # type: str.   
+00028af0: 2020 2020 2073 656c 662e 6f72 6465 7220       self.order 
+00028b00: 3d20 6f72 6465 7220 2023 2074 7970 653a  = order  # type:
+00028b10: 2073 7472 0a20 2020 2020 2020 2073 656c   str.        sel
+00028b20: 662e 7061 6765 5f6e 756d 6265 7220 3d20  f.page_number = 
+00028b30: 7061 6765 5f6e 756d 6265 7220 2023 2074  page_number  # t
+00028b40: 7970 653a 2069 6e74 0a20 2020 2020 2020  ype: int.       
+00028b50: 2073 656c 662e 7061 6765 5f73 697a 6520   self.page_size 
+00028b60: 3d20 7061 6765 5f73 697a 6520 2023 2074  = page_size  # t
+00028b70: 7970 653a 2069 6e74 0a20 2020 2020 2020  ype: int.       
+00028b80: 2073 656c 662e 7069 7065 6c69 6e65 5f69   self.pipeline_i
+00028b90: 6420 3d20 7069 7065 6c69 6e65 5f69 6420  d = pipeline_id 
+00028ba0: 2023 2074 7970 653a 2073 7472 0a20 2020   # type: str.   
+00028bb0: 2020 2020 2073 656c 662e 7265 736f 7572       self.resour
+00028bc0: 6365 5f69 6420 3d20 7265 736f 7572 6365  ce_id = resource
+00028bd0: 5f69 6420 2023 2074 7970 653a 2073 7472  _id  # type: str
+00028be0: 0a20 2020 2020 2020 2073 656c 662e 7368  .        self.sh
+00028bf0: 6f77 5f6f 776e 203d 2073 686f 775f 6f77  ow_own = show_ow
+00028c00: 6e20 2023 2074 7970 653a 2062 6f6f 6c0a  n  # type: bool.
+00028c10: 2020 2020 2020 2020 7365 6c66 2e73 6f72          self.sor
+00028c20: 745f 6279 203d 2073 6f72 745f 6279 2020  t_by = sort_by  
+00028c30: 2320 7479 7065 3a20 7374 720a 2020 2020  # type: str.    
+00028c40: 2020 2020 7365 6c66 2e73 7461 7274 5f74      self.start_t
+00028c50: 696d 6520 3d20 7374 6172 745f 7469 6d65  ime = start_time
+00028c60: 2020 2320 7479 7065 3a20 7374 720a 2020    # type: str.  
+00028c70: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
+00028c80: 7320 3d20 7374 6174 7573 2020 2320 7479  s = status  # ty
+00028c90: 7065 3a20 7374 720a 2020 2020 2020 2020  pe: str.        
+00028ca0: 7365 6c66 2e74 6167 7320 3d20 7461 6773  self.tags = tags
+00028cb0: 2020 2320 7479 7065 3a20 6469 6374 5b73    # type: dict[s
+00028cc0: 7472 2c20 7374 725d 0a20 2020 2020 2020  tr, str].       
+00028cd0: 2073 656c 662e 776f 726b 7370 6163 655f   self.workspace_
+00028ce0: 6964 203d 2077 6f72 6b73 7061 6365 5f69  id = workspace_i
+00028cf0: 6420 2023 2074 7970 653a 2073 7472 0a0a  d  # type: str..
+00028d00: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
+00028d10: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00028d20: 7061 7373 0a0a 2020 2020 6465 6620 746f  pass..    def to
+00028d30: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
+00028d40: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
+00028d50: 284c 6973 744a 6f62 7352 6571 7565 7374  (ListJobsRequest
+00028d60: 2c20 7365 6c66 292e 746f 5f6d 6170 2829  , self).to_map()
+00028d70: 0a20 2020 2020 2020 2069 6620 5f6d 6170  .        if _map
+00028d80: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00028d90: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00028da0: 205f 6d61 700a 0a20 2020 2020 2020 2072   _map..        r
+00028db0: 6573 756c 7420 3d20 6469 6374 2829 0a20  esult = dict(). 
+00028dc0: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
+00028dd0: 7573 696e 6573 735f 7573 6572 5f69 6420  usiness_user_id 
+00028de0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00028df0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00028e00: 2742 7573 696e 6573 7355 7365 7249 6427  'BusinessUserId'
+00028e10: 5d20 3d20 7365 6c66 2e62 7573 696e 6573  ] = self.busines
+00028e20: 735f 7573 6572 5f69 640a 2020 2020 2020  s_user_id.      
+00028e30: 2020 6966 2073 656c 662e 6361 6c6c 6572    if self.caller
+00028e40: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00028e50: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00028e60: 5b27 4361 6c6c 6572 275d 203d 2073 656c  ['Caller'] = sel
+00028e70: 662e 6361 6c6c 6572 0a20 2020 2020 2020  f.caller.       
+00028e80: 2069 6620 7365 6c66 2e64 6973 706c 6179   if self.display
+00028e90: 5f6e 616d 6520 6973 206e 6f74 204e 6f6e  _name is not Non
+00028ea0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00028eb0: 6573 756c 745b 2744 6973 706c 6179 4e61  esult['DisplayNa
+00028ec0: 6d65 275d 203d 2073 656c 662e 6469 7370  me'] = self.disp
+00028ed0: 6c61 795f 6e61 6d65 0a20 2020 2020 2020  lay_name.       
+00028ee0: 2069 6620 7365 6c66 2e65 6e64 5f74 696d   if self.end_tim
+00028ef0: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
+00028f00: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00028f10: 745b 2745 6e64 5469 6d65 275d 203d 2073  t['EndTime'] = s
+00028f20: 656c 662e 656e 645f 7469 6d65 0a20 2020  elf.end_time.   
+00028f30: 2020 2020 2069 6620 7365 6c66 2e66 726f       if self.fro
+00028f40: 6d5f 616c 6c5f 776f 726b 7370 6163 6573  m_all_workspaces
+00028f50: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00028f60: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00028f70: 5b27 4672 6f6d 416c 6c57 6f72 6b73 7061  ['FromAllWorkspa
+00028f80: 6365 7327 5d20 3d20 7365 6c66 2e66 726f  ces'] = self.fro
+00028f90: 6d5f 616c 6c5f 776f 726b 7370 6163 6573  m_all_workspaces
+00028fa0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00028fb0: 2e6a 6f62 5f69 6420 6973 206e 6f74 204e  .job_id is not N
+00028fc0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00028fd0: 2072 6573 756c 745b 274a 6f62 4964 275d   result['JobId']
+00028fe0: 203d 2073 656c 662e 6a6f 625f 6964 0a20   = self.job_id. 
+00028ff0: 2020 2020 2020 2069 6620 7365 6c66 2e6a         if self.j
+00029000: 6f62 5f74 7970 6520 6973 206e 6f74 204e  ob_type is not N
+00029010: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00029020: 2072 6573 756c 745b 274a 6f62 5479 7065   result['JobType
+00029030: 275d 203d 2073 656c 662e 6a6f 625f 7479  '] = self.job_ty
+00029040: 7065 0a20 2020 2020 2020 2069 6620 7365  pe.        if se
+00029050: 6c66 2e6f 7264 6572 2069 7320 6e6f 7420  lf.order is not 
+00029060: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00029070: 2020 7265 7375 6c74 5b27 4f72 6465 7227    result['Order'
+00029080: 5d20 3d20 7365 6c66 2e6f 7264 6572 0a20  ] = self.order. 
+00029090: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
+000290a0: 6167 655f 6e75 6d62 6572 2069 7320 6e6f  age_number is no
+000290b0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+000290c0: 2020 2020 7265 7375 6c74 5b27 5061 6765      result['Page
+000290d0: 4e75 6d62 6572 275d 203d 2073 656c 662e  Number'] = self.
+000290e0: 7061 6765 5f6e 756d 6265 720a 2020 2020  page_number.    
+000290f0: 2020 2020 6966 2073 656c 662e 7061 6765      if self.page
+00029100: 5f73 697a 6520 6973 206e 6f74 204e 6f6e  _size is not Non
+00029110: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00029120: 6573 756c 745b 2750 6167 6553 697a 6527  esult['PageSize'
+00029130: 5d20 3d20 7365 6c66 2e70 6167 655f 7369  ] = self.page_si
+00029140: 7a65 0a20 2020 2020 2020 2069 6620 7365  ze.        if se
+00029150: 6c66 2e70 6970 656c 696e 655f 6964 2069  lf.pipeline_id i
+00029160: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00029170: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+00029180: 5069 7065 6c69 6e65 4964 275d 203d 2073  PipelineId'] = s
+00029190: 656c 662e 7069 7065 6c69 6e65 5f69 640a  elf.pipeline_id.
+000291a0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000291b0: 7265 736f 7572 6365 5f69 6420 6973 206e  resource_id is n
+000291c0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000291d0: 2020 2020 2072 6573 756c 745b 2752 6573       result['Res
+000291e0: 6f75 7263 6549 6427 5d20 3d20 7365 6c66  ourceId'] = self
+000291f0: 2e72 6573 6f75 7263 655f 6964 0a20 2020  .resource_id.   
+00029200: 2020 2020 2069 6620 7365 6c66 2e73 686f       if self.sho
+00029210: 775f 6f77 6e20 6973 206e 6f74 204e 6f6e  w_own is not Non
+00029220: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00029230: 6573 756c 745b 2753 686f 774f 776e 275d  esult['ShowOwn']
+00029240: 203d 2073 656c 662e 7368 6f77 5f6f 776e   = self.show_own
+00029250: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00029260: 2e73 6f72 745f 6279 2069 7320 6e6f 7420  .sort_by is not 
+00029270: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00029280: 2020 7265 7375 6c74 5b27 536f 7274 4279    result['SortBy
+00029290: 275d 203d 2073 656c 662e 736f 7274 5f62  '] = self.sort_b
+000292a0: 790a 2020 2020 2020 2020 6966 2073 656c  y.        if sel
+000292b0: 662e 7374 6172 745f 7469 6d65 2069 7320  f.start_time is 
+000292c0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000292d0: 2020 2020 2020 7265 7375 6c74 5b27 5374        result['St
+000292e0: 6172 7454 696d 6527 5d20 3d20 7365 6c66  artTime'] = self
+000292f0: 2e73 7461 7274 5f74 696d 650a 2020 2020  .start_time.    
+00029300: 2020 2020 6966 2073 656c 662e 7374 6174      if self.stat
+00029310: 7573 2069 7320 6e6f 7420 4e6f 6e65 3a0a  us is not None:.
+00029320: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00029330: 6c74 5b27 5374 6174 7573 275d 203d 2073  lt['Status'] = s
+00029340: 656c 662e 7374 6174 7573 0a20 2020 2020  elf.status.     
+00029350: 2020 2069 6620 7365 6c66 2e74 6167 7320     if self.tags 
+00029360: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00029370: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00029380: 2754 6167 7327 5d20 3d20 7365 6c66 2e74  'Tags'] = self.t
+00029390: 6167 730a 2020 2020 2020 2020 6966 2073  ags.        if s
+000293a0: 656c 662e 776f 726b 7370 6163 655f 6964  elf.workspace_id
+000293b0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000293c0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+000293d0: 5b27 576f 726b 7370 6163 6549 6427 5d20  ['WorkspaceId'] 
+000293e0: 3d20 7365 6c66 2e77 6f72 6b73 7061 6365  = self.workspace
+000293f0: 5f69 640a 2020 2020 2020 2020 7265 7475  _id.        retu
+00029400: 726e 2072 6573 756c 740a 0a20 2020 2064  rn result..    d
+00029410: 6566 2066 726f 6d5f 6d61 7028 7365 6c66  ef from_map(self
+00029420: 2c20 6d3d 4e6f 6e65 293a 0a20 2020 2020  , m=None):.     
+00029430: 2020 206d 203d 206d 206f 7220 6469 6374     m = m or dict
+00029440: 2829 0a20 2020 2020 2020 2069 6620 6d2e  ().        if m.
+00029450: 6765 7428 2742 7573 696e 6573 7355 7365  get('BusinessUse
+00029460: 7249 6427 2920 6973 206e 6f74 204e 6f6e  rId') is not Non
+00029470: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00029480: 656c 662e 6275 7369 6e65 7373 5f75 7365  elf.business_use
+00029490: 725f 6964 203d 206d 2e67 6574 2827 4275  r_id = m.get('Bu
+000294a0: 7369 6e65 7373 5573 6572 4964 2729 0a20  sinessUserId'). 
+000294b0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+000294c0: 2743 616c 6c65 7227 2920 6973 206e 6f74  'Caller') is not
+000294d0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000294e0: 2020 2073 656c 662e 6361 6c6c 6572 203d     self.caller =
+000294f0: 206d 2e67 6574 2827 4361 6c6c 6572 2729   m.get('Caller')
+00029500: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+00029510: 7428 2744 6973 706c 6179 4e61 6d65 2729  t('DisplayName')
+00029520: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00029530: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
+00029540: 6973 706c 6179 5f6e 616d 6520 3d20 6d2e  isplay_name = m.
+00029550: 6765 7428 2744 6973 706c 6179 4e61 6d65  get('DisplayName
+00029560: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+00029570: 6765 7428 2745 6e64 5469 6d65 2729 2069  get('EndTime') i
+00029580: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00029590: 2020 2020 2020 2020 7365 6c66 2e65 6e64          self.end
+000295a0: 5f74 696d 6520 3d20 6d2e 6765 7428 2745  _time = m.get('E
+000295b0: 6e64 5469 6d65 2729 0a20 2020 2020 2020  ndTime').       
+000295c0: 2069 6620 6d2e 6765 7428 2746 726f 6d41   if m.get('FromA
+000295d0: 6c6c 576f 726b 7370 6163 6573 2729 2069  llWorkspaces') i
+000295e0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000295f0: 2020 2020 2020 2020 7365 6c66 2e66 726f          self.fro
+00029600: 6d5f 616c 6c5f 776f 726b 7370 6163 6573  m_all_workspaces
+00029610: 203d 206d 2e67 6574 2827 4672 6f6d 416c   = m.get('FromAl
+00029620: 6c57 6f72 6b73 7061 6365 7327 290a 2020  lWorkspaces').  
+00029630: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00029640: 4a6f 6249 6427 2920 6973 206e 6f74 204e  JobId') is not N
+00029650: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00029660: 2073 656c 662e 6a6f 625f 6964 203d 206d   self.job_id = m
+00029670: 2e67 6574 2827 4a6f 6249 6427 290a 2020  .get('JobId').  
+00029680: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+00029690: 4a6f 6254 7970 6527 2920 6973 206e 6f74  JobType') is not
+000296a0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000296b0: 2020 2073 656c 662e 6a6f 625f 7479 7065     self.job_type
+000296c0: 203d 206d 2e67 6574 2827 4a6f 6254 7970   = m.get('JobTyp
+000296d0: 6527 290a 2020 2020 2020 2020 6966 206d  e').        if m
+000296e0: 2e67 6574 2827 4f72 6465 7227 2920 6973  .get('Order') is
+000296f0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00029700: 2020 2020 2020 2073 656c 662e 6f72 6465         self.orde
+00029710: 7220 3d20 6d2e 6765 7428 274f 7264 6572  r = m.get('Order
+00029720: 2729 0a20 2020 2020 2020 2069 6620 6d2e  ').        if m.
+00029730: 6765 7428 2750 6167 654e 756d 6265 7227  get('PageNumber'
+00029740: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+00029750: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00029760: 7061 6765 5f6e 756d 6265 7220 3d20 6d2e  page_number = m.
+00029770: 6765 7428 2750 6167 654e 756d 6265 7227  get('PageNumber'
+00029780: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+00029790: 6574 2827 5061 6765 5369 7a65 2729 2069  et('PageSize') i
+000297a0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+000297b0: 2020 2020 2020 2020 7365 6c66 2e70 6167          self.pag
+000297c0: 655f 7369 7a65 203d 206d 2e67 6574 2827  e_size = m.get('
+000297d0: 5061 6765 5369 7a65 2729 0a20 2020 2020  PageSize').     
+000297e0: 2020 2069 6620 6d2e 6765 7428 2750 6970     if m.get('Pip
+000297f0: 656c 696e 6549 6427 2920 6973 206e 6f74  elineId') is not
+00029800: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00029810: 2020 2073 656c 662e 7069 7065 6c69 6e65     self.pipeline
+00029820: 5f69 6420 3d20 6d2e 6765 7428 2750 6970  _id = m.get('Pip
+00029830: 656c 696e 6549 6427 290a 2020 2020 2020  elineId').      
+00029840: 2020 6966 206d 2e67 6574 2827 5265 736f    if m.get('Reso
+00029850: 7572 6365 4964 2729 2069 7320 6e6f 7420  urceId') is not 
+00029860: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00029870: 2020 7365 6c66 2e72 6573 6f75 7263 655f    self.resource_
+00029880: 6964 203d 206d 2e67 6574 2827 5265 736f  id = m.get('Reso
+00029890: 7572 6365 4964 2729 0a20 2020 2020 2020  urceId').       
+000298a0: 2069 6620 6d2e 6765 7428 2753 686f 774f   if m.get('ShowO
+000298b0: 776e 2729 2069 7320 6e6f 7420 4e6f 6e65  wn') is not None
+000298c0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+000298d0: 6c66 2e73 686f 775f 6f77 6e20 3d20 6d2e  lf.show_own = m.
+000298e0: 6765 7428 2753 686f 774f 776e 2729 0a20  get('ShowOwn'). 
+000298f0: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+00029900: 2753 6f72 7442 7927 2920 6973 206e 6f74  'SortBy') is not
+00029910: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00029920: 2020 2073 656c 662e 736f 7274 5f62 7920     self.sort_by 
+00029930: 3d20 6d2e 6765 7428 2753 6f72 7442 7927  = m.get('SortBy'
+00029940: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+00029950: 6574 2827 5374 6172 7454 696d 6527 2920  et('StartTime') 
+00029960: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00029970: 2020 2020 2020 2020 2073 656c 662e 7374           self.st
+00029980: 6172 745f 7469 6d65 203d 206d 2e67 6574  art_time = m.get
+00029990: 2827 5374 6172 7454 696d 6527 290a 2020  ('StartTime').  
+000299a0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+000299b0: 5374 6174 7573 2729 2069 7320 6e6f 7420  Status') is not 
+000299c0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000299d0: 2020 7365 6c66 2e73 7461 7475 7320 3d20    self.status = 
+000299e0: 6d2e 6765 7428 2753 7461 7475 7327 290a  m.get('Status').
+000299f0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+00029a00: 2827 5461 6773 2729 2069 7320 6e6f 7420  ('Tags') is not 
+00029a10: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00029a20: 2020 7365 6c66 2e74 6167 7320 3d20 6d2e    self.tags = m.
+00029a30: 6765 7428 2754 6167 7327 290a 2020 2020  get('Tags').    
+00029a40: 2020 2020 6966 206d 2e67 6574 2827 576f      if m.get('Wo
+00029a50: 726b 7370 6163 6549 6427 2920 6973 206e  rkspaceId') is n
+00029a60: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00029a70: 2020 2020 2073 656c 662e 776f 726b 7370       self.worksp
+00029a80: 6163 655f 6964 203d 206d 2e67 6574 2827  ace_id = m.get('
+00029a90: 576f 726b 7370 6163 6549 6427 290a 2020  WorkspaceId').  
+00029aa0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00029ab0: 660a 0a0a 636c 6173 7320 4c69 7374 4a6f  f...class ListJo
+00029ac0: 6273 5368 7269 6e6b 5265 7175 6573 7428  bsShrinkRequest(
+00029ad0: 5465 614d 6f64 656c 293a 0a20 2020 2064  TeaModel):.    d
+00029ae0: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+00029af0: 2c20 6275 7369 6e65 7373 5f75 7365 725f  , business_user_
+00029b00: 6964 3d4e 6f6e 652c 2063 616c 6c65 723d  id=None, caller=
+00029b10: 4e6f 6e65 2c20 6469 7370 6c61 795f 6e61  None, display_na
+00029b20: 6d65 3d4e 6f6e 652c 2065 6e64 5f74 696d  me=None, end_tim
+00029b30: 653d 4e6f 6e65 2c0a 2020 2020 2020 2020  e=None,.        
+00029b40: 2020 2020 2020 2020 2066 726f 6d5f 616c           from_al
+00029b50: 6c5f 776f 726b 7370 6163 6573 3d4e 6f6e  l_workspaces=Non
+00029b60: 652c 206a 6f62 5f69 643d 4e6f 6e65 2c20  e, job_id=None, 
+00029b70: 6a6f 625f 7479 7065 3d4e 6f6e 652c 206f  job_type=None, o
+00029b80: 7264 6572 3d4e 6f6e 652c 2070 6167 655f  rder=None, page_
+00029b90: 6e75 6d62 6572 3d4e 6f6e 652c 2070 6167  number=None, pag
+00029ba0: 655f 7369 7a65 3d4e 6f6e 652c 2070 6970  e_size=None, pip
+00029bb0: 656c 696e 655f 6964 3d4e 6f6e 652c 0a20  eline_id=None,. 
+00029bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029bd0: 7265 736f 7572 6365 5f69 643d 4e6f 6e65  resource_id=None
+00029be0: 2c20 7368 6f77 5f6f 776e 3d4e 6f6e 652c  , show_own=None,
+00029bf0: 2073 6f72 745f 6279 3d4e 6f6e 652c 2073   sort_by=None, s
+00029c00: 7461 7274 5f74 696d 653d 4e6f 6e65 2c20  tart_time=None, 
+00029c10: 7374 6174 7573 3d4e 6f6e 652c 2074 6167  status=None, tag
+00029c20: 735f 7368 7269 6e6b 3d4e 6f6e 652c 0a20  s_shrink=None,. 
+00029c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00029c40: 776f 726b 7370 6163 655f 6964 3d4e 6f6e  workspace_id=Non
+00029c50: 6529 3a0a 2020 2020 2020 2020 7365 6c66  e):.        self
+00029c60: 2e62 7573 696e 6573 735f 7573 6572 5f69  .business_user_i
+00029c70: 6420 3d20 6275 7369 6e65 7373 5f75 7365  d = business_use
+00029c80: 725f 6964 2020 2320 7479 7065 3a20 7374  r_id  # type: st
+00029c90: 720a 2020 2020 2020 2020 7365 6c66 2e63  r.        self.c
+00029ca0: 616c 6c65 7220 3d20 6361 6c6c 6572 2020  aller = caller  
+00029cb0: 2320 7479 7065 3a20 7374 720a 2020 2020  # type: str.    
+00029cc0: 2020 2020 7365 6c66 2e64 6973 706c 6179      self.display
+00029cd0: 5f6e 616d 6520 3d20 6469 7370 6c61 795f  _name = display_
+00029ce0: 6e61 6d65 2020 2320 7479 7065 3a20 7374  name  # type: st
+00029cf0: 720a 2020 2020 2020 2020 7365 6c66 2e65  r.        self.e
+00029d00: 6e64 5f74 696d 6520 3d20 656e 645f 7469  nd_time = end_ti
+00029d10: 6d65 2020 2320 7479 7065 3a20 7374 720a  me  # type: str.
+00029d20: 2020 2020 2020 2020 7365 6c66 2e66 726f          self.fro
+00029d30: 6d5f 616c 6c5f 776f 726b 7370 6163 6573  m_all_workspaces
+00029d40: 203d 2066 726f 6d5f 616c 6c5f 776f 726b   = from_all_work
+00029d50: 7370 6163 6573 2020 2320 7479 7065 3a20  spaces  # type: 
+00029d60: 626f 6f6c 0a20 2020 2020 2020 2073 656c  bool.        sel
+00029d70: 662e 6a6f 625f 6964 203d 206a 6f62 5f69  f.job_id = job_i
+00029d80: 6420 2023 2074 7970 653a 2073 7472 0a20  d  # type: str. 
+00029d90: 2020 2020 2020 2073 656c 662e 6a6f 625f         self.job_
+00029da0: 7479 7065 203d 206a 6f62 5f74 7970 6520  type = job_type 
+00029db0: 2023 2074 7970 653a 2073 7472 0a20 2020   # type: str.   
+00029dc0: 2020 2020 2073 656c 662e 6f72 6465 7220       self.order 
+00029dd0: 3d20 6f72 6465 7220 2023 2074 7970 653a  = order  # type:
+00029de0: 2073 7472 0a20 2020 2020 2020 2073 656c   str.        sel
+00029df0: 662e 7061 6765 5f6e 756d 6265 7220 3d20  f.page_number = 
+00029e00: 7061 6765 5f6e 756d 6265 7220 2023 2074  page_number  # t
+00029e10: 7970 653a 2069 6e74 0a20 2020 2020 2020  ype: int.       
+00029e20: 2073 656c 662e 7061 6765 5f73 697a 6520   self.page_size 
+00029e30: 3d20 7061 6765 5f73 697a 6520 2023 2074  = page_size  # t
+00029e40: 7970 653a 2069 6e74 0a20 2020 2020 2020  ype: int.       
+00029e50: 2073 656c 662e 7069 7065 6c69 6e65 5f69   self.pipeline_i
+00029e60: 6420 3d20 7069 7065 6c69 6e65 5f69 6420  d = pipeline_id 
+00029e70: 2023 2074 7970 653a 2073 7472 0a20 2020   # type: str.   
+00029e80: 2020 2020 2073 656c 662e 7265 736f 7572       self.resour
+00029e90: 6365 5f69 6420 3d20 7265 736f 7572 6365  ce_id = resource
+00029ea0: 5f69 6420 2023 2074 7970 653a 2073 7472  _id  # type: str
+00029eb0: 0a20 2020 2020 2020 2073 656c 662e 7368  .        self.sh
+00029ec0: 6f77 5f6f 776e 203d 2073 686f 775f 6f77  ow_own = show_ow
+00029ed0: 6e20 2023 2074 7970 653a 2062 6f6f 6c0a  n  # type: bool.
+00029ee0: 2020 2020 2020 2020 7365 6c66 2e73 6f72          self.sor
+00029ef0: 745f 6279 203d 2073 6f72 745f 6279 2020  t_by = sort_by  
+00029f00: 2320 7479 7065 3a20 7374 720a 2020 2020  # type: str.    
+00029f10: 2020 2020 7365 6c66 2e73 7461 7274 5f74      self.start_t
+00029f20: 696d 6520 3d20 7374 6172 745f 7469 6d65  ime = start_time
+00029f30: 2020 2320 7479 7065 3a20 7374 720a 2020    # type: str.  
+00029f40: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
+00029f50: 7320 3d20 7374 6174 7573 2020 2320 7479  s = status  # ty
+00029f60: 7065 3a20 7374 720a 2020 2020 2020 2020  pe: str.        
+00029f70: 7365 6c66 2e74 6167 735f 7368 7269 6e6b  self.tags_shrink
+00029f80: 203d 2074 6167 735f 7368 7269 6e6b 2020   = tags_shrink  
+00029f90: 2320 7479 7065 3a20 7374 720a 2020 2020  # type: str.    
+00029fa0: 2020 2020 7365 6c66 2e77 6f72 6b73 7061      self.workspa
+00029fb0: 6365 5f69 6420 3d20 776f 726b 7370 6163  ce_id = workspac
+00029fc0: 655f 6964 2020 2320 7479 7065 3a20 7374  e_id  # type: st
+00029fd0: 720a 0a20 2020 2064 6566 2076 616c 6964  r..    def valid
+00029fe0: 6174 6528 7365 6c66 293a 0a20 2020 2020  ate(self):.     
+00029ff0: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
+0002a000: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
+0002a010: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
+0002a020: 7065 7228 4c69 7374 4a6f 6273 5368 7269  per(ListJobsShri
+0002a030: 6e6b 5265 7175 6573 742c 2073 656c 6629  nkRequest, self)
+0002a040: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
+0002a050: 2020 6966 205f 6d61 7020 6973 206e 6f74    if _map is not
+0002a060: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0002a070: 2020 2072 6574 7572 6e20 5f6d 6170 0a0a     return _map..
+0002a080: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+0002a090: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+0002a0a0: 6966 2073 656c 662e 6275 7369 6e65 7373  if self.business
+0002a0b0: 5f75 7365 725f 6964 2069 7320 6e6f 7420  _user_id is not 
+0002a0c0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0002a0d0: 2020 7265 7375 6c74 5b27 4275 7369 6e65    result['Busine
+0002a0e0: 7373 5573 6572 4964 275d 203d 2073 656c  ssUserId'] = sel
+0002a0f0: 662e 6275 7369 6e65 7373 5f75 7365 725f  f.business_user_
+0002a100: 6964 0a20 2020 2020 2020 2069 6620 7365  id.        if se
+0002a110: 6c66 2e63 616c 6c65 7220 6973 206e 6f74  lf.caller is not
+0002a120: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0002a130: 2020 2072 6573 756c 745b 2743 616c 6c65     result['Calle
+0002a140: 7227 5d20 3d20 7365 6c66 2e63 616c 6c65  r'] = self.calle
+0002a150: 720a 2020 2020 2020 2020 6966 2073 656c  r.        if sel
+0002a160: 662e 6469 7370 6c61 795f 6e61 6d65 2069  f.display_name i
+0002a170: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0002a180: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+0002a190: 4469 7370 6c61 794e 616d 6527 5d20 3d20  DisplayName'] = 
+0002a1a0: 7365 6c66 2e64 6973 706c 6179 5f6e 616d  self.display_nam
+0002a1b0: 650a 2020 2020 2020 2020 6966 2073 656c  e.        if sel
+0002a1c0: 662e 656e 645f 7469 6d65 2069 7320 6e6f  f.end_time is no
+0002a1d0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0002a1e0: 2020 2020 7265 7375 6c74 5b27 456e 6454      result['EndT
+0002a1f0: 696d 6527 5d20 3d20 7365 6c66 2e65 6e64  ime'] = self.end
+0002a200: 5f74 696d 650a 2020 2020 2020 2020 6966  _time.        if
+0002a210: 2073 656c 662e 6672 6f6d 5f61 6c6c 5f77   self.from_all_w
+0002a220: 6f72 6b73 7061 6365 7320 6973 206e 6f74  orkspaces is not
+0002a230: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0002a240: 2020 2072 6573 756c 745b 2746 726f 6d41     result['FromA
+0002a250: 6c6c 576f 726b 7370 6163 6573 275d 203d  llWorkspaces'] =
+0002a260: 2073 656c 662e 6672 6f6d 5f61 6c6c 5f77   self.from_all_w
+0002a270: 6f72 6b73 7061 6365 730a 2020 2020 2020  orkspaces.      
+0002a280: 2020 6966 2073 656c 662e 6a6f 625f 6964    if self.job_id
+0002a290: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0002a2a0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+0002a2b0: 5b27 4a6f 6249 6427 5d20 3d20 7365 6c66  ['JobId'] = self
+0002a2c0: 2e6a 6f62 5f69 640a 2020 2020 2020 2020  .job_id.        
+0002a2d0: 6966 2073 656c 662e 6a6f 625f 7479 7065  if self.job_type
+0002a2e0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0002a2f0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+0002a300: 5b27 4a6f 6254 7970 6527 5d20 3d20 7365  ['JobType'] = se
+0002a310: 6c66 2e6a 6f62 5f74 7970 650a 2020 2020  lf.job_type.    
+0002a320: 2020 2020 6966 2073 656c 662e 6f72 6465      if self.orde
+0002a330: 7220 6973 206e 6f74 204e 6f6e 653a 0a20  r is not None:. 
+0002a340: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+0002a350: 745b 274f 7264 6572 275d 203d 2073 656c  t['Order'] = sel
+0002a360: 662e 6f72 6465 720a 2020 2020 2020 2020  f.order.        
+0002a370: 6966 2073 656c 662e 7061 6765 5f6e 756d  if self.page_num
+0002a380: 6265 7220 6973 206e 6f74 204e 6f6e 653a  ber is not None:
+0002a390: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+0002a3a0: 756c 745b 2750 6167 654e 756d 6265 7227  ult['PageNumber'
+0002a3b0: 5d20 3d20 7365 6c66 2e70 6167 655f 6e75  ] = self.page_nu
+0002a3c0: 6d62 6572 0a20 2020 2020 2020 2069 6620  mber.        if 
+0002a3d0: 7365 6c66 2e70 6167 655f 7369 7a65 2069  self.page_size i
+0002a3e0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0002a3f0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+0002a400: 5061 6765 5369 7a65 275d 203d 2073 656c  PageSize'] = sel
+0002a410: 662e 7061 6765 5f73 697a 650a 2020 2020  f.page_size.    
+0002a420: 2020 2020 6966 2073 656c 662e 7069 7065      if self.pipe
+0002a430: 6c69 6e65 5f69 6420 6973 206e 6f74 204e  line_id is not N
+0002a440: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0002a450: 2072 6573 756c 745b 2750 6970 656c 696e   result['Pipelin
+0002a460: 6549 6427 5d20 3d20 7365 6c66 2e70 6970  eId'] = self.pip
+0002a470: 656c 696e 655f 6964 0a20 2020 2020 2020  eline_id.       
+0002a480: 2069 6620 7365 6c66 2e72 6573 6f75 7263   if self.resourc
+0002a490: 655f 6964 2069 7320 6e6f 7420 4e6f 6e65  e_id is not None
+0002a4a0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0002a4b0: 7375 6c74 5b27 5265 736f 7572 6365 4964  sult['ResourceId
+0002a4c0: 275d 203d 2073 656c 662e 7265 736f 7572  '] = self.resour
+0002a4d0: 6365 5f69 640a 2020 2020 2020 2020 6966  ce_id.        if
+0002a4e0: 2073 656c 662e 7368 6f77 5f6f 776e 2069   self.show_own i
+0002a4f0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0002a500: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+0002a510: 5368 6f77 4f77 6e27 5d20 3d20 7365 6c66  ShowOwn'] = self
+0002a520: 2e73 686f 775f 6f77 6e0a 2020 2020 2020  .show_own.      
+0002a530: 2020 6966 2073 656c 662e 736f 7274 5f62    if self.sort_b
+0002a540: 7920 6973 206e 6f74 204e 6f6e 653a 0a20  y is not None:. 
+0002a550: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+0002a560: 745b 2753 6f72 7442 7927 5d20 3d20 7365  t['SortBy'] = se
+0002a570: 6c66 2e73 6f72 745f 6279 0a20 2020 2020  lf.sort_by.     
+0002a580: 2020 2069 6620 7365 6c66 2e73 7461 7274     if self.start
+0002a590: 5f74 696d 6520 6973 206e 6f74 204e 6f6e  _time is not Non
+0002a5a0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0002a5b0: 6573 756c 745b 2753 7461 7274 5469 6d65  esult['StartTime
+0002a5c0: 275d 203d 2073 656c 662e 7374 6172 745f  '] = self.start_
+0002a5d0: 7469 6d65 0a20 2020 2020 2020 2069 6620  time.        if 
+0002a5e0: 7365 6c66 2e73 7461 7475 7320 6973 206e  self.status is n
+0002a5f0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0002a600: 2020 2020 2072 6573 756c 745b 2753 7461       result['Sta
+0002a610: 7475 7327 5d20 3d20 7365 6c66 2e73 7461  tus'] = self.sta
+0002a620: 7475 730a 2020 2020 2020 2020 6966 2073  tus.        if s
+0002a630: 656c 662e 7461 6773 5f73 6872 696e 6b20  elf.tags_shrink 
+0002a640: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0002a650: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+0002a660: 2754 6167 7327 5d20 3d20 7365 6c66 2e74  'Tags'] = self.t
+0002a670: 6167 735f 7368 7269 6e6b 0a20 2020 2020  ags_shrink.     
+0002a680: 2020 2069 6620 7365 6c66 2e77 6f72 6b73     if self.works
+0002a690: 7061 6365 5f69 6420 6973 206e 6f74 204e  pace_id is not N
+0002a6a0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0002a6b0: 2072 6573 756c 745b 2757 6f72 6b73 7061   result['Workspa
+0002a6c0: 6365 4964 275d 203d 2073 656c 662e 776f  ceId'] = self.wo
+0002a6d0: 726b 7370 6163 655f 6964 0a20 2020 2020  rkspace_id.     
+0002a6e0: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
+0002a6f0: 0a0a 2020 2020 6465 6620 6672 6f6d 5f6d  ..    def from_m
+0002a700: 6170 2873 656c 662c 206d 3d4e 6f6e 6529  ap(self, m=None)
+0002a710: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
+0002a720: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
+0002a730: 2020 6966 206d 2e67 6574 2827 4275 7369    if m.get('Busi
+0002a740: 6e65 7373 5573 6572 4964 2729 2069 7320  nessUserId') is 
+0002a750: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0002a760: 2020 2020 2020 7365 6c66 2e62 7573 696e        self.busin
+0002a770: 6573 735f 7573 6572 5f69 6420 3d20 6d2e  ess_user_id = m.
+0002a780: 6765 7428 2742 7573 696e 6573 7355 7365  get('BusinessUse
+0002a790: 7249 6427 290a 2020 2020 2020 2020 6966  rId').        if
+0002a7a0: 206d 2e67 6574 2827 4361 6c6c 6572 2729   m.get('Caller')
+0002a7b0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0002a7c0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+0002a7d0: 616c 6c65 7220 3d20 6d2e 6765 7428 2743  aller = m.get('C
+0002a7e0: 616c 6c65 7227 290a 2020 2020 2020 2020  aller').        
+0002a7f0: 6966 206d 2e67 6574 2827 4469 7370 6c61  if m.get('Displa
+0002a800: 794e 616d 6527 2920 6973 206e 6f74 204e  yName') is not N
+0002a810: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0002a820: 2073 656c 662e 6469 7370 6c61 795f 6e61   self.display_na
+0002a830: 6d65 203d 206d 2e67 6574 2827 4469 7370  me = m.get('Disp
+0002a840: 6c61 794e 616d 6527 290a 2020 2020 2020  layName').      
+0002a850: 2020 6966 206d 2e67 6574 2827 456e 6454    if m.get('EndT
+0002a860: 696d 6527 2920 6973 206e 6f74 204e 6f6e  ime') is not Non
+0002a870: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0002a880: 656c 662e 656e 645f 7469 6d65 203d 206d  elf.end_time = m
+0002a890: 2e67 6574 2827 456e 6454 696d 6527 290a  .get('EndTime').
+0002a8a0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+0002a8b0: 2827 4672 6f6d 416c 6c57 6f72 6b73 7061  ('FromAllWorkspa
+0002a8c0: 6365 7327 2920 6973 206e 6f74 204e 6f6e  ces') is not Non
+0002a8d0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0002a8e0: 656c 662e 6672 6f6d 5f61 6c6c 5f77 6f72  elf.from_all_wor
+0002a8f0: 6b73 7061 6365 7320 3d20 6d2e 6765 7428  kspaces = m.get(
+0002a900: 2746 726f 6d41 6c6c 576f 726b 7370 6163  'FromAllWorkspac
+0002a910: 6573 2729 0a20 2020 2020 2020 2069 6620  es').        if 
+0002a920: 6d2e 6765 7428 274a 6f62 4964 2729 2069  m.get('JobId') i
+0002a930: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0002a940: 2020 2020 2020 2020 7365 6c66 2e6a 6f62          self.job
+0002a950: 5f69 6420 3d20 6d2e 6765 7428 274a 6f62  _id = m.get('Job
+0002a960: 4964 2729 0a20 2020 2020 2020 2069 6620  Id').        if 
+0002a970: 6d2e 6765 7428 274a 6f62 5479 7065 2729  m.get('JobType')
+0002a980: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0002a990: 2020 2020 2020 2020 2020 7365 6c66 2e6a            self.j
+0002a9a0: 6f62 5f74 7970 6520 3d20 6d2e 6765 7428  ob_type = m.get(
+0002a9b0: 274a 6f62 5479 7065 2729 0a20 2020 2020  'JobType').     
+0002a9c0: 2020 2069 6620 6d2e 6765 7428 274f 7264     if m.get('Ord
+0002a9d0: 6572 2729 2069 7320 6e6f 7420 4e6f 6e65  er') is not None
+0002a9e0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0002a9f0: 6c66 2e6f 7264 6572 203d 206d 2e67 6574  lf.order = m.get
+0002aa00: 2827 4f72 6465 7227 290a 2020 2020 2020  ('Order').      
+0002aa10: 2020 6966 206d 2e67 6574 2827 5061 6765    if m.get('Page
+0002aa20: 4e75 6d62 6572 2729 2069 7320 6e6f 7420  Number') is not 
+0002aa30: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0002aa40: 2020 7365 6c66 2e70 6167 655f 6e75 6d62    self.page_numb
+0002aa50: 6572 203d 206d 2e67 6574 2827 5061 6765  er = m.get('Page
+0002aa60: 4e75 6d62 6572 2729 0a20 2020 2020 2020  Number').       
+0002aa70: 2069 6620 6d2e 6765 7428 2750 6167 6553   if m.get('PageS
+0002aa80: 697a 6527 2920 6973 206e 6f74 204e 6f6e  ize') is not Non
+0002aa90: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0002aaa0: 656c 662e 7061 6765 5f73 697a 6520 3d20  elf.page_size = 
+0002aab0: 6d2e 6765 7428 2750 6167 6553 697a 6527  m.get('PageSize'
+0002aac0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+0002aad0: 6574 2827 5069 7065 6c69 6e65 4964 2729  et('PipelineId')
+0002aae0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0002aaf0: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
+0002ab00: 6970 656c 696e 655f 6964 203d 206d 2e67  ipeline_id = m.g
+0002ab10: 6574 2827 5069 7065 6c69 6e65 4964 2729  et('PipelineId')
+0002ab20: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+0002ab30: 7428 2752 6573 6f75 7263 6549 6427 2920  t('ResourceId') 
+0002ab40: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0002ab50: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
+0002ab60: 736f 7572 6365 5f69 6420 3d20 6d2e 6765  source_id = m.ge
+0002ab70: 7428 2752 6573 6f75 7263 6549 6427 290a  t('ResourceId').
+0002ab80: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+0002ab90: 2827 5368 6f77 4f77 6e27 2920 6973 206e  ('ShowOwn') is n
+0002aba0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0002abb0: 2020 2020 2073 656c 662e 7368 6f77 5f6f       self.show_o
+0002abc0: 776e 203d 206d 2e67 6574 2827 5368 6f77  wn = m.get('Show
+0002abd0: 4f77 6e27 290a 2020 2020 2020 2020 6966  Own').        if
+0002abe0: 206d 2e67 6574 2827 536f 7274 4279 2729   m.get('SortBy')
+0002abf0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0002ac00: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+0002ac10: 6f72 745f 6279 203d 206d 2e67 6574 2827  ort_by = m.get('
+0002ac20: 536f 7274 4279 2729 0a20 2020 2020 2020  SortBy').       
+0002ac30: 2069 6620 6d2e 6765 7428 2753 7461 7274   if m.get('Start
+0002ac40: 5469 6d65 2729 2069 7320 6e6f 7420 4e6f  Time') is not No
+0002ac50: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0002ac60: 7365 6c66 2e73 7461 7274 5f74 696d 6520  self.start_time 
+0002ac70: 3d20 6d2e 6765 7428 2753 7461 7274 5469  = m.get('StartTi
+0002ac80: 6d65 2729 0a20 2020 2020 2020 2069 6620  me').        if 
+0002ac90: 6d2e 6765 7428 2753 7461 7475 7327 2920  m.get('Status') 
+0002aca0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0002acb0: 2020 2020 2020 2020 2073 656c 662e 7374           self.st
+0002acc0: 6174 7573 203d 206d 2e67 6574 2827 5374  atus = m.get('St
+0002acd0: 6174 7573 2729 0a20 2020 2020 2020 2069  atus').        i
+0002ace0: 6620 6d2e 6765 7428 2754 6167 7327 2920  f m.get('Tags') 
+0002acf0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0002ad00: 2020 2020 2020 2020 2073 656c 662e 7461           self.ta
+0002ad10: 6773 5f73 6872 696e 6b20 3d20 6d2e 6765  gs_shrink = m.ge
+0002ad20: 7428 2754 6167 7327 290a 2020 2020 2020  t('Tags').      
+0002ad30: 2020 6966 206d 2e67 6574 2827 576f 726b    if m.get('Work
+0002ad40: 7370 6163 6549 6427 2920 6973 206e 6f74  spaceId') is not
+0002ad50: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0002ad60: 2020 2073 656c 662e 776f 726b 7370 6163     self.workspac
+0002ad70: 655f 6964 203d 206d 2e67 6574 2827 576f  e_id = m.get('Wo
+0002ad80: 726b 7370 6163 6549 6427 290a 2020 2020  rkspaceId').    
+0002ad90: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
+0002ada0: 0a0a 636c 6173 7320 4c69 7374 4a6f 6273  ..class ListJobs
+0002adb0: 5265 7370 6f6e 7365 426f 6479 2854 6561  ResponseBody(Tea
+0002adc0: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
+0002add0: 5f5f 696e 6974 5f5f 2873 656c 662c 206a  __init__(self, j
+0002ade0: 6f62 733d 4e6f 6e65 2c20 7265 7175 6573  obs=None, reques
+0002adf0: 745f 6964 3d4e 6f6e 652c 2074 6f74 616c  t_id=None, total
+0002ae00: 5f63 6f75 6e74 3d4e 6f6e 6529 3a0a 2020  _count=None):.  
+0002ae10: 2020 2020 2020 7365 6c66 2e6a 6f62 7320        self.jobs 
+0002ae20: 3d20 6a6f 6273 2020 2320 7479 7065 3a20  = jobs  # type: 
+0002ae30: 6c69 7374 5b4a 6f62 4974 656d 5d0a 2020  list[JobItem].  
+0002ae40: 2020 2020 2020 7365 6c66 2e72 6571 7565        self.reque
+0002ae50: 7374 5f69 6420 3d20 7265 7175 6573 745f  st_id = request_
+0002ae60: 6964 2020 2320 7479 7065 3a20 7374 720a  id  # type: str.
+0002ae70: 2020 2020 2020 2020 7365 6c66 2e74 6f74          self.tot
+0002ae80: 616c 5f63 6f75 6e74 203d 2074 6f74 616c  al_count = total
+0002ae90: 5f63 6f75 6e74 2020 2320 7479 7065 3a20  _count  # type: 
+0002aea0: 6c6f 6e67 0a0a 2020 2020 6465 6620 7661  long..    def va
+0002aeb0: 6c69 6461 7465 2873 656c 6629 3a0a 2020  lidate(self):.  
+0002aec0: 2020 2020 2020 6966 2073 656c 662e 6a6f        if self.jo
+0002aed0: 6273 3a0a 2020 2020 2020 2020 2020 2020  bs:.            
+0002aee0: 666f 7220 6b20 696e 2073 656c 662e 6a6f  for k in self.jo
+0002aef0: 6273 3a0a 2020 2020 2020 2020 2020 2020  bs:.            
+0002af00: 2020 2020 6966 206b 3a0a 2020 2020 2020      if k:.      
+0002af10: 2020 2020 2020 2020 2020 2020 2020 6b2e                k.
+0002af20: 7661 6c69 6461 7465 2829 0a0a 2020 2020  validate()..    
+0002af30: 6465 6620 746f 5f6d 6170 2873 656c 6629  def to_map(self)
+0002af40: 3a0a 2020 2020 2020 2020 5f6d 6170 203d  :.        _map =
+0002af50: 2073 7570 6572 284c 6973 744a 6f62 7352   super(ListJobsR
+0002af60: 6573 706f 6e73 6542 6f64 792c 2073 656c  esponseBody, sel
+0002af70: 6629 2e74 6f5f 6d61 7028 290a 2020 2020  f).to_map().    
+0002af80: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
+0002af90: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0002afa0: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
+0002afb0: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
+0002afc0: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
+0002afd0: 2020 7265 7375 6c74 5b27 4a6f 6273 275d    result['Jobs']
+0002afe0: 203d 205b 5d0a 2020 2020 2020 2020 6966   = [].        if
+0002aff0: 2073 656c 662e 6a6f 6273 2069 7320 6e6f   self.jobs is no
+0002b000: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0002b010: 2020 2020 666f 7220 6b20 696e 2073 656c      for k in sel
+0002b020: 662e 6a6f 6273 3a0a 2020 2020 2020 2020  f.jobs:.        
+0002b030: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+0002b040: 4a6f 6273 275d 2e61 7070 656e 6428 6b2e  Jobs'].append(k.
+0002b050: 746f 5f6d 6170 2829 2069 6620 6b20 656c  to_map() if k el
+0002b060: 7365 204e 6f6e 6529 0a20 2020 2020 2020  se None).       
+0002b070: 2069 6620 7365 6c66 2e72 6571 7565 7374   if self.request
+0002b080: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
+0002b090: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+0002b0a0: 756c 745b 2752 6571 7565 7374 4964 275d  ult['RequestId']
+0002b0b0: 203d 2073 656c 662e 7265 7175 6573 745f   = self.request_
+0002b0c0: 6964 0a20 2020 2020 2020 2069 6620 7365  id.        if se
+0002b0d0: 6c66 2e74 6f74 616c 5f63 6f75 6e74 2069  lf.total_count i
+0002b0e0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0002b0f0: 2020 2020 2020 2020 7265 7375 6c74 5b27          result['
+0002b100: 546f 7461 6c43 6f75 6e74 275d 203d 2073  TotalCount'] = s
+0002b110: 656c 662e 746f 7461 6c5f 636f 756e 740a  elf.total_count.
+0002b120: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+0002b130: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
+0002b140: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3d  rom_map(self, m=
+0002b150: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
+0002b160: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
+0002b170: 2020 2020 2020 2073 656c 662e 6a6f 6273         self.jobs
+0002b180: 203d 205b 5d0a 2020 2020 2020 2020 6966   = [].        if
+0002b190: 206d 2e67 6574 2827 4a6f 6273 2729 2069   m.get('Jobs') i
+0002b1a0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0002b1b0: 2020 2020 2020 2020 666f 7220 6b20 696e          for k in
+0002b1c0: 206d 2e67 6574 2827 4a6f 6273 2729 3a0a   m.get('Jobs'):.
+0002b1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002b1e0: 7465 6d70 5f6d 6f64 656c 203d 204a 6f62  temp_model = Job
+0002b1f0: 4974 656d 2829 0a20 2020 2020 2020 2020  Item().         
+0002b200: 2020 2020 2020 2073 656c 662e 6a6f 6273         self.jobs
+0002b210: 2e61 7070 656e 6428 7465 6d70 5f6d 6f64  .append(temp_mod
+0002b220: 656c 2e66 726f 6d5f 6d61 7028 6b29 290a  el.from_map(k)).
+0002b230: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+0002b240: 2827 5265 7175 6573 7449 6427 2920 6973  ('RequestId') is
+0002b250: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0002b260: 2020 2020 2020 2073 656c 662e 7265 7175         self.requ
+0002b270: 6573 745f 6964 203d 206d 2e67 6574 2827  est_id = m.get('
+0002b280: 5265 7175 6573 7449 6427 290a 2020 2020  RequestId').    
+0002b290: 2020 2020 6966 206d 2e67 6574 2827 546f      if m.get('To
+0002b2a0: 7461 6c43 6f75 6e74 2729 2069 7320 6e6f  talCount') is no
+0002b2b0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0002b2c0: 2020 2020 7365 6c66 2e74 6f74 616c 5f63      self.total_c
+0002b2d0: 6f75 6e74 203d 206d 2e67 6574 2827 546f  ount = m.get('To
+0002b2e0: 7461 6c43 6f75 6e74 2729 0a20 2020 2020  talCount').     
+0002b2f0: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
+0002b300: 0a63 6c61 7373 204c 6973 744a 6f62 7352  .class ListJobsR
+0002b310: 6573 706f 6e73 6528 5465 614d 6f64 656c  esponse(TeaModel
+0002b320: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
+0002b330: 745f 5f28 7365 6c66 2c20 6865 6164 6572  t__(self, header
+0002b340: 733d 4e6f 6e65 2c20 7374 6174 7573 5f63  s=None, status_c
+0002b350: 6f64 653d 4e6f 6e65 2c20 626f 6479 3d4e  ode=None, body=N
+0002b360: 6f6e 6529 3a0a 2020 2020 2020 2020 7365  one):.        se
+0002b370: 6c66 2e68 6561 6465 7273 203d 2068 6561  lf.headers = hea
+0002b380: 6465 7273 2020 2320 7479 7065 3a20 6469  ders  # type: di
+0002b390: 6374 5b73 7472 2c20 7374 725d 0a20 2020  ct[str, str].   
+0002b3a0: 2020 2020 2073 656c 662e 7374 6174 7573       self.status
+0002b3b0: 5f63 6f64 6520 3d20 7374 6174 7573 5f63  _code = status_c
+0002b3c0: 6f64 6520 2023 2074 7970 653a 2069 6e74  ode  # type: int
+0002b3d0: 0a20 2020 2020 2020 2073 656c 662e 626f  .        self.bo
+0002b3e0: 6479 203d 2062 6f64 7920 2023 2074 7970  dy = body  # typ
+0002b3f0: 653a 204c 6973 744a 6f62 7352 6573 706f  e: ListJobsRespo
+0002b400: 6e73 6542 6f64 790a 0a20 2020 2064 6566  nseBody..    def
+0002b410: 2076 616c 6964 6174 6528 7365 6c66 293a   validate(self):
+0002b420: 0a20 2020 2020 2020 2073 656c 662e 7661  .        self.va
+0002b430: 6c69 6461 7465 5f72 6571 7569 7265 6428  lidate_required(
+0002b440: 7365 6c66 2e68 6561 6465 7273 2c20 2768  self.headers, 'h
+0002b450: 6561 6465 7273 2729 0a20 2020 2020 2020  eaders').       
+0002b460: 2073 656c 662e 7661 6c69 6461 7465 5f72   self.validate_r
+0002b470: 6571 7569 7265 6428 7365 6c66 2e73 7461  equired(self.sta
+0002b480: 7475 735f 636f 6465 2c20 2773 7461 7475  tus_code, 'statu
+0002b490: 735f 636f 6465 2729 0a20 2020 2020 2020  s_code').       
+0002b4a0: 2073 656c 662e 7661 6c69 6461 7465 5f72   self.validate_r
+0002b4b0: 6571 7569 7265 6428 7365 6c66 2e62 6f64  equired(self.bod
+0002b4c0: 792c 2027 626f 6479 2729 0a20 2020 2020  y, 'body').     
+0002b4d0: 2020 2069 6620 7365 6c66 2e62 6f64 793a     if self.body:
+0002b4e0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0002b4f0: 662e 626f 6479 2e76 616c 6964 6174 6528  f.body.validate(
+0002b500: 290a 0a20 2020 2064 6566 2074 6f5f 6d61  )..    def to_ma
+0002b510: 7028 7365 6c66 293a 0a20 2020 2020 2020  p(self):.       
+0002b520: 205f 6d61 7020 3d20 7375 7065 7228 4c69   _map = super(Li
+0002b530: 7374 4a6f 6273 5265 7370 6f6e 7365 2c20  stJobsResponse, 
+0002b540: 7365 6c66 292e 746f 5f6d 6170 2829 0a20  self).to_map(). 
+0002b550: 2020 2020 2020 2069 6620 5f6d 6170 2069         if _map i
+0002b560: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0002b570: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+0002b580: 6d61 700a 0a20 2020 2020 2020 2072 6573  map..        res
+0002b590: 756c 7420 3d20 6469 6374 2829 0a20 2020  ult = dict().   
+0002b5a0: 2020 2020 2069 6620 7365 6c66 2e68 6561       if self.hea
+0002b5b0: 6465 7273 2069 7320 6e6f 7420 4e6f 6e65  ders is not None
+0002b5c0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0002b5d0: 7375 6c74 5b27 6865 6164 6572 7327 5d20  sult['headers'] 
+0002b5e0: 3d20 7365 6c66 2e68 6561 6465 7273 0a20  = self.headers. 
+0002b5f0: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
+0002b600: 7461 7475 735f 636f 6465 2069 7320 6e6f  tatus_code is no
+0002b610: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0002b620: 2020 2020 7265 7375 6c74 5b27 7374 6174      result['stat
+0002b630: 7573 436f 6465 275d 203d 2073 656c 662e  usCode'] = self.
+0002b640: 7374 6174 7573 5f63 6f64 650a 2020 2020  status_code.    
+0002b650: 2020 2020 6966 2073 656c 662e 626f 6479      if self.body
+0002b660: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0002b670: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+0002b680: 5b27 626f 6479 275d 203d 2073 656c 662e  ['body'] = self.
+0002b690: 626f 6479 2e74 6f5f 6d61 7028 290a 2020  body.to_map().  
+0002b6a0: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+0002b6b0: 756c 740a 0a20 2020 2064 6566 2066 726f  ult..    def fro
+0002b6c0: 6d5f 6d61 7028 7365 6c66 2c20 6d3d 4e6f  m_map(self, m=No
+0002b6d0: 6e65 293a 0a20 2020 2020 2020 206d 203d  ne):.        m =
+0002b6e0: 206d 206f 7220 6469 6374 2829 0a20 2020   m or dict().   
+0002b6f0: 2020 2020 2069 6620 6d2e 6765 7428 2768       if m.get('h
+0002b700: 6561 6465 7273 2729 2069 7320 6e6f 7420  eaders') is not 
+0002b710: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0002b720: 2020 7365 6c66 2e68 6561 6465 7273 203d    self.headers =
+0002b730: 206d 2e67 6574 2827 6865 6164 6572 7327   m.get('headers'
+0002b740: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+0002b750: 6574 2827 7374 6174 7573 436f 6465 2729  et('statusCode')
+0002b760: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0002b770: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+0002b780: 7461 7475 735f 636f 6465 203d 206d 2e67  tatus_code = m.g
+0002b790: 6574 2827 7374 6174 7573 436f 6465 2729  et('statusCode')
+0002b7a0: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+0002b7b0: 7428 2762 6f64 7927 2920 6973 206e 6f74  t('body') is not
+0002b7c0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0002b7d0: 2020 2074 656d 705f 6d6f 6465 6c20 3d20     temp_model = 
+0002b7e0: 4c69 7374 4a6f 6273 5265 7370 6f6e 7365  ListJobsResponse
+0002b7f0: 426f 6479 2829 0a20 2020 2020 2020 2020  Body().         
+0002b800: 2020 2073 656c 662e 626f 6479 203d 2074     self.body = t
+0002b810: 656d 705f 6d6f 6465 6c2e 6672 6f6d 5f6d  emp_model.from_m
+0002b820: 6170 286d 5b27 626f 6479 275d 290a 2020  ap(m['body']).  
+0002b830: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+0002b840: 660a 0a0a 636c 6173 7320 4c69 7374 5465  f...class ListTe
+0002b850: 6e73 6f72 626f 6172 6473 5265 7175 6573  nsorboardsReques
+0002b860: 7428 5465 614d 6f64 656c 293a 0a20 2020  t(TeaModel):.   
+0002b870: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
+0002b880: 6c66 2c20 6469 7370 6c61 795f 6e61 6d65  lf, display_name
+0002b890: 3d4e 6f6e 652c 2065 6e64 5f74 696d 653d  =None, end_time=
+0002b8a0: 4e6f 6e65 2c20 6a6f 625f 6964 3d4e 6f6e  None, job_id=Non
+0002b8b0: 652c 206f 7264 6572 3d4e 6f6e 652c 2070  e, order=None, p
+0002b8c0: 6167 655f 6e75 6d62 6572 3d4e 6f6e 652c  age_number=None,
+0002b8d0: 2070 6167 655f 7369 7a65 3d4e 6f6e 652c   page_size=None,
+0002b8e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0002b8f0: 2020 736f 7274 5f62 793d 4e6f 6e65 2c20    sort_by=None, 
+0002b900: 736f 7572 6365 5f69 643d 4e6f 6e65 2c20  source_id=None, 
+0002b910: 736f 7572 6365 5f74 7970 653d 4e6f 6e65  source_type=None
+0002b920: 2c20 7374 6172 745f 7469 6d65 3d4e 6f6e  , start_time=Non
+0002b930: 652c 2073 7461 7475 733d 4e6f 6e65 2c20  e, status=None, 
+0002b940: 7465 6e73 6f72 626f 6172 645f 6964 3d4e  tensorboard_id=N
+0002b950: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
+0002b960: 2020 2020 2020 7665 7262 6f73 653d 4e6f        verbose=No
+0002b970: 6e65 2c20 776f 726b 7370 6163 655f 6964  ne, workspace_id
+0002b980: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
+0002b990: 7365 6c66 2e64 6973 706c 6179 5f6e 616d  self.display_nam
+0002b9a0: 6520 3d20 6469 7370 6c61 795f 6e61 6d65  e = display_name
+0002b9b0: 2020 2320 7479 7065 3a20 7374 720a 2020    # type: str.  
+0002b9c0: 2020 2020 2020 7365 6c66 2e65 6e64 5f74        self.end_t
+0002b9d0: 696d 6520 3d20 656e 645f 7469 6d65 2020  ime = end_time  
+0002b9e0: 2320 7479 7065 3a20 7374 720a 2020 2020  # type: str.    
+0002b9f0: 2020 2020 7365 6c66 2e6a 6f62 5f69 6420      self.job_id 
+0002ba00: 3d20 6a6f 625f 6964 2020 2320 7479 7065  = job_id  # type
+0002ba10: 3a20 7374 720a 2020 2020 2020 2020 7365  : str.        se
+0002ba20: 6c66 2e6f 7264 6572 203d 206f 7264 6572  lf.order = order
+0002ba30: 2020 2320 7479 7065 3a20 7374 720a 2020    # type: str.  
+0002ba40: 2020 2020 2020 7365 6c66 2e70 6167 655f        self.page_
+0002ba50: 6e75 6d62 6572 203d 2070 6167 655f 6e75  number = page_nu
+0002ba60: 6d62 6572 2020 2320 7479 7065 3a20 696e  mber  # type: in
+0002ba70: 740a 2020 2020 2020 2020 7365 6c66 2e70  t.        self.p
+0002ba80: 6167 655f 7369 7a65 203d 2070 6167 655f  age_size = page_
+0002ba90: 7369 7a65 2020 2320 7479 7065 3a20 696e  size  # type: in
+0002baa0: 740a 2020 2020 2020 2020 7365 6c66 2e73  t.        self.s
+0002bab0: 6f72 745f 6279 203d 2073 6f72 745f 6279  ort_by = sort_by
+0002bac0: 2020 2320 7479 7065 3a20 7374 720a 2020    # type: str.  
+0002bad0: 2020 2020 2020 7365 6c66 2e73 6f75 7263        self.sourc
+0002bae0: 655f 6964 203d 2073 6f75 7263 655f 6964  e_id = source_id
+0002baf0: 2020 2320 7479 7065 3a20 7374 720a 2020    # type: str.  
+0002bb00: 2020 2020 2020 7365 6c66 2e73 6f75 7263        self.sourc
+0002bb10: 655f 7479 7065 203d 2073 6f75 7263 655f  e_type = source_
+0002bb20: 7479 7065 2020 2320 7479 7065 3a20 7374  type  # type: st
+0002bb30: 720a 2020 2020 2020 2020 7365 6c66 2e73  r.        self.s
+0002bb40: 7461 7274 5f74 696d 6520 3d20 7374 6172  tart_time = star
+0002bb50: 745f 7469 6d65 2020 2320 7479 7065 3a20  t_time  # type: 
+0002bb60: 7374 720a 2020 2020 2020 2020 7365 6c66  str.        self
+0002bb70: 2e73 7461 7475 7320 3d20 7374 6174 7573  .status = status
+0002bb80: 2020 2320 7479 7065 3a20 7374 720a 2020    # type: str.  
+0002bb90: 2020 2020 2020 7365 6c66 2e74 656e 736f        self.tenso
+0002bba0: 7262 6f61 7264 5f69 6420 3d20 7465 6e73  rboard_id = tens
+0002bbb0: 6f72 626f 6172 645f 6964 2020 2320 7479  orboard_id  # ty
+0002bbc0: 7065 3a20 7374 720a 2020 2020 2020 2020  pe: str.        
+0002bbd0: 7365 6c66 2e76 6572 626f 7365 203d 2076  self.verbose = v
+0002bbe0: 6572 626f 7365 2020 2320 7479 7065 3a20  erbose  # type: 
+0002bbf0: 626f 6f6c 0a20 2020 2020 2020 2073 656c  bool.        sel
+0002bc00: 662e 776f 726b 7370 6163 655f 6964 203d  f.workspace_id =
+0002bc10: 2077 6f72 6b73 7061 6365 5f69 6420 2023   workspace_id  #
+0002bc20: 2074 7970 653a 2073 7472 0a0a 2020 2020   type: str..    
+0002bc30: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
+0002bc40: 6629 3a0a 2020 2020 2020 2020 7061 7373  f):.        pass
+0002bc50: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
+0002bc60: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0002bc70: 5f6d 6170 203d 2073 7570 6572 284c 6973  _map = super(Lis
+0002bc80: 7454 656e 736f 7262 6f61 7264 7352 6571  tTensorboardsReq
+0002bc90: 7565 7374 2c20 7365 6c66 292e 746f 5f6d  uest, self).to_m
+0002bca0: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
+0002bcb0: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
+0002bcc0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0002bcd0: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
+0002bce0: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
+0002bcf0: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
+0002bd00: 6c66 2e64 6973 706c 6179 5f6e 616d 6520  lf.display_name 
+0002bd10: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0002bd20: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+0002bd30: 2744 6973 706c 6179 4e61 6d65 275d 203d  'DisplayName'] =
+0002bd40: 2073 656c 662e 6469 7370 6c61 795f 6e61   self.display_na
+0002bd50: 6d65 0a20 2020 2020 2020 2069 6620 7365  me.        if se
+0002bd60: 6c66 2e65 6e64 5f74 696d 6520 6973 206e  lf.end_time is n
+0002bd70: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0002bd80: 2020 2020 2072 6573 756c 745b 2745 6e64       result['End
+0002bd90: 5469 6d65 275d 203d 2073 656c 662e 656e  Time'] = self.en
+0002bda0: 645f 7469 6d65 0a20 2020 2020 2020 2069  d_time.        i
+0002bdb0: 6620 7365 6c66 2e6a 6f62 5f69 6420 6973  f self.job_id is
+0002bdc0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0002bdd0: 2020 2020 2020 2072 6573 756c 745b 274a         result['J
+0002bde0: 6f62 4964 275d 203d 2073 656c 662e 6a6f  obId'] = self.jo
+0002bdf0: 625f 6964 0a20 2020 2020 2020 2069 6620  b_id.        if 
+0002be00: 7365 6c66 2e6f 7264 6572 2069 7320 6e6f  self.order is no
+0002be10: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0002be20: 2020 2020 7265 7375 6c74 5b27 4f72 6465      result['Orde
+0002be30: 7227 5d20 3d20 7365 6c66 2e6f 7264 6572  r'] = self.order
+0002be40: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0002be50: 2e70 6167 655f 6e75 6d62 6572 2069 7320  .page_number is 
+0002be60: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0002be70: 2020 2020 2020 7265 7375 6c74 5b27 5061        result['Pa
+0002be80: 6765 4e75 6d62 6572 275d 203d 2073 656c  geNumber'] = sel
+0002be90: 662e 7061 6765 5f6e 756d 6265 720a 2020  f.page_number.  
+0002bea0: 2020 2020 2020 6966 2073 656c 662e 7061        if self.pa
+0002beb0: 6765 5f73 697a 6520 6973 206e 6f74 204e  ge_size is not N
+0002bec0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0002bed0: 2072 6573 756c 745b 2750 6167 6553 697a   result['PageSiz
+0002bee0: 6527 5d20 3d20 7365 6c66 2e70 6167 655f  e'] = self.page_
+0002bef0: 7369 7a65 0a20 2020 2020 2020 2069 6620  size.        if 
+0002bf00: 7365 6c66 2e73 6f72 745f 6279 2069 7320  self.sort_by is 
+0002bf10: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0002bf20: 2020 2020 2020 7265 7375 6c74 5b27 536f        result['So
+0002bf30: 7274 4279 275d 203d 2073 656c 662e 736f  rtBy'] = self.so
+0002bf40: 7274 5f62 790a 2020 2020 2020 2020 6966  rt_by.        if
+0002bf50: 2073 656c 662e 736f 7572 6365 5f69 6420   self.source_id 
+0002bf60: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0002bf70: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+0002bf80: 2753 6f75 7263 6549 6427 5d20 3d20 7365  'SourceId'] = se
+0002bf90: 6c66 2e73 6f75 7263 655f 6964 0a20 2020  lf.source_id.   
+0002bfa0: 2020 2020 2069 6620 7365 6c66 2e73 6f75       if self.sou
+0002bfb0: 7263 655f 7479 7065 2069 7320 6e6f 7420  rce_type is not 
+0002bfc0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0002bfd0: 2020 7265 7375 6c74 5b27 536f 7572 6365    result['Source
+0002bfe0: 5479 7065 275d 203d 2073 656c 662e 736f  Type'] = self.so
+0002bff0: 7572 6365 5f74 7970 650a 2020 2020 2020  urce_type.      
+0002c000: 2020 6966 2073 656c 662e 7374 6172 745f    if self.start_
+0002c010: 7469 6d65 2069 7320 6e6f 7420 4e6f 6e65  time is not None
+0002c020: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0002c030: 7375 6c74 5b27 5374 6172 7454 696d 6527  sult['StartTime'
+0002c040: 5d20 3d20 7365 6c66 2e73 7461 7274 5f74  ] = self.start_t
+0002c050: 696d 650a 2020 2020 2020 2020 6966 2073  ime.        if s
+0002c060: 656c 662e 7374 6174 7573 2069 7320 6e6f  elf.status is no
+0002c070: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0002c080: 2020 2020 7265 7375 6c74 5b27 5374 6174      result['Stat
+0002c090: 7573 275d 203d 2073 656c 662e 7374 6174  us'] = self.stat
+0002c0a0: 7573 0a20 2020 2020 2020 2069 6620 7365  us.        if se
+0002c0b0: 6c66 2e74 656e 736f 7262 6f61 7264 5f69  lf.tensorboard_i
+0002c0c0: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
+0002c0d0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+0002c0e0: 745b 2754 656e 736f 7262 6f61 7264 4964  t['TensorboardId
+0002c0f0: 275d 203d 2073 656c 662e 7465 6e73 6f72  '] = self.tensor
+0002c100: 626f 6172 645f 6964 0a20 2020 2020 2020  board_id.       
+0002c110: 2069 6620 7365 6c66 2e76 6572 626f 7365   if self.verbose
+0002c120: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0002c130: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+0002c140: 5b27 5665 7262 6f73 6527 5d20 3d20 7365  ['Verbose'] = se
+0002c150: 6c66 2e76 6572 626f 7365 0a20 2020 2020  lf.verbose.     
+0002c160: 2020 2069 6620 7365 6c66 2e77 6f72 6b73     if self.works
+0002c170: 7061 6365 5f69 6420 6973 206e 6f74 204e  pace_id is not N
+0002c180: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0002c190: 2072 6573 756c 745b 2757 6f72 6b73 7061   result['Workspa
+0002c1a0: 6365 4964 275d 203d 2073 656c 662e 776f  ceId'] = self.wo
+0002c1b0: 726b 7370 6163 655f 6964 0a20 2020 2020  rkspace_id.     
+0002c1c0: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
+0002c1d0: 0a0a 2020 2020 6465 6620 6672 6f6d 5f6d  ..    def from_m
+0002c1e0: 6170 2873 656c 662c 206d 3d4e 6f6e 6529  ap(self, m=None)
+0002c1f0: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
+0002c200: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
+0002c210: 2020 6966 206d 2e67 6574 2827 4469 7370    if m.get('Disp
+0002c220: 6c61 794e 616d 6527 2920 6973 206e 6f74  layName') is not
+0002c230: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0002c240: 2020 2073 656c 662e 6469 7370 6c61 795f     self.display_
+0002c250: 6e61 6d65 203d 206d 2e67 6574 2827 4469  name = m.get('Di
+0002c260: 7370 6c61 794e 616d 6527 290a 2020 2020  splayName').    
+0002c270: 2020 2020 6966 206d 2e67 6574 2827 456e      if m.get('En
+0002c280: 6454 696d 6527 2920 6973 206e 6f74 204e  dTime') is not N
+0002c290: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0002c2a0: 2073 656c 662e 656e 645f 7469 6d65 203d   self.end_time =
+0002c2b0: 206d 2e67 6574 2827 456e 6454 696d 6527   m.get('EndTime'
+0002c2c0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+0002c2d0: 6574 2827 4a6f 6249 6427 2920 6973 206e  et('JobId') is n
+0002c2e0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0002c2f0: 2020 2020 2073 656c 662e 6a6f 625f 6964       self.job_id
+0002c300: 203d 206d 2e67 6574 2827 4a6f 6249 6427   = m.get('JobId'
+0002c310: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+0002c320: 6574 2827 4f72 6465 7227 2920 6973 206e  et('Order') is n
+0002c330: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0002c340: 2020 2020 2073 656c 662e 6f72 6465 7220       self.order 
+0002c350: 3d20 6d2e 6765 7428 274f 7264 6572 2729  = m.get('Order')
+0002c360: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+0002c370: 7428 2750 6167 654e 756d 6265 7227 2920  t('PageNumber') 
+0002c380: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0002c390: 2020 2020 2020 2020 2073 656c 662e 7061           self.pa
+0002c3a0: 6765 5f6e 756d 6265 7220 3d20 6d2e 6765  ge_number = m.ge
+0002c3b0: 7428 2750 6167 654e 756d 6265 7227 290a  t('PageNumber').
+0002c3c0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+0002c3d0: 2827 5061 6765 5369 7a65 2729 2069 7320  ('PageSize') is 
+0002c3e0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0002c3f0: 2020 2020 2020 7365 6c66 2e70 6167 655f        self.page_
+0002c400: 7369 7a65 203d 206d 2e67 6574 2827 5061  size = m.get('Pa
+0002c410: 6765 5369 7a65 2729 0a20 2020 2020 2020  geSize').       
+0002c420: 2069 6620 6d2e 6765 7428 2753 6f72 7442   if m.get('SortB
+0002c430: 7927 2920 6973 206e 6f74 204e 6f6e 653a  y') is not None:
+0002c440: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0002c450: 662e 736f 7274 5f62 7920 3d20 6d2e 6765  f.sort_by = m.ge
+0002c460: 7428 2753 6f72 7442 7927 290a 2020 2020  t('SortBy').    
+0002c470: 2020 2020 6966 206d 2e67 6574 2827 536f      if m.get('So
+0002c480: 7572 6365 4964 2729 2069 7320 6e6f 7420  urceId') is not 
+0002c490: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0002c4a0: 2020 7365 6c66 2e73 6f75 7263 655f 6964    self.source_id
+0002c4b0: 203d 206d 2e67 6574 2827 536f 7572 6365   = m.get('Source
+0002c4c0: 4964 2729 0a20 2020 2020 2020 2069 6620  Id').        if 
+0002c4d0: 6d2e 6765 7428 2753 6f75 7263 6554 7970  m.get('SourceTyp
+0002c4e0: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
+0002c4f0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0002c500: 662e 736f 7572 6365 5f74 7970 6520 3d20  f.source_type = 
+0002c510: 6d2e 6765 7428 2753 6f75 7263 6554 7970  m.get('SourceTyp
+0002c520: 6527 290a 2020 2020 2020 2020 6966 206d  e').        if m
+0002c530: 2e67 6574 2827 5374 6172 7454 696d 6527  .get('StartTime'
+0002c540: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+0002c550: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0002c560: 7374 6172 745f 7469 6d65 203d 206d 2e67  start_time = m.g
+0002c570: 6574 2827 5374 6172 7454 696d 6527 290a  et('StartTime').
+0002c580: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+0002c590: 2827 5374 6174 7573 2729 2069 7320 6e6f  ('Status') is no
+0002c5a0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0002c5b0: 2020 2020 7365 6c66 2e73 7461 7475 7320      self.status 
+0002c5c0: 3d20 6d2e 6765 7428 2753 7461 7475 7327  = m.get('Status'
+0002c5d0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+0002c5e0: 6574 2827 5465 6e73 6f72 626f 6172 6449  et('TensorboardI
+0002c5f0: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
+0002c600: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0002c610: 662e 7465 6e73 6f72 626f 6172 645f 6964  f.tensorboard_id
+0002c620: 203d 206d 2e67 6574 2827 5465 6e73 6f72   = m.get('Tensor
+0002c630: 626f 6172 6449 6427 290a 2020 2020 2020  boardId').      
+0002c640: 2020 6966 206d 2e67 6574 2827 5665 7262    if m.get('Verb
+0002c650: 6f73 6527 2920 6973 206e 6f74 204e 6f6e  ose') is not Non
+0002c660: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0002c670: 656c 662e 7665 7262 6f73 6520 3d20 6d2e  elf.verbose = m.
+0002c680: 6765 7428 2756 6572 626f 7365 2729 0a20  get('Verbose'). 
+0002c690: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+0002c6a0: 2757 6f72 6b73 7061 6365 4964 2729 2069  'WorkspaceId') i
+0002c6b0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0002c6c0: 2020 2020 2020 2020 7365 6c66 2e77 6f72          self.wor
+0002c6d0: 6b73 7061 6365 5f69 6420 3d20 6d2e 6765  kspace_id = m.ge
+0002c6e0: 7428 2757 6f72 6b73 7061 6365 4964 2729  t('WorkspaceId')
+0002c6f0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0002c700: 7365 6c66 0a0a 0a63 6c61 7373 204c 6973  self...class Lis
+0002c710: 7454 656e 736f 7262 6f61 7264 7352 6573  tTensorboardsRes
+0002c720: 706f 6e73 6542 6f64 7928 5465 614d 6f64  ponseBody(TeaMod
+0002c730: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
+0002c740: 6e69 745f 5f28 7365 6c66 2c20 7265 7175  nit__(self, requ
+0002c750: 6573 745f 6964 3d4e 6f6e 652c 2074 656e  est_id=None, ten
+0002c760: 736f 7262 6f61 7264 733d 4e6f 6e65 2c20  sorboards=None, 
+0002c770: 746f 7461 6c5f 636f 756e 743d 4e6f 6e65  total_count=None
+0002c780: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+0002c790: 7265 7175 6573 745f 6964 203d 2072 6571  request_id = req
+0002c7a0: 7565 7374 5f69 6420 2023 2074 7970 653a  uest_id  # type:
+0002c7b0: 2073 7472 0a20 2020 2020 2020 2073 656c   str.        sel
+0002c7c0: 662e 7465 6e73 6f72 626f 6172 6473 203d  f.tensorboards =
+0002c7d0: 2074 656e 736f 7262 6f61 7264 7320 2023   tensorboards  #
+0002c7e0: 2074 7970 653a 206c 6973 745b 5465 6e73   type: list[Tens
+0002c7f0: 6f72 626f 6172 645d 0a20 2020 2020 2020  orboard].       
+0002c800: 2073 656c 662e 746f 7461 6c5f 636f 756e   self.total_coun
+0002c810: 7420 3d20 746f 7461 6c5f 636f 756e 7420  t = total_count 
+0002c820: 2023 2074 7970 653a 206c 6f6e 670a 0a20   # type: long.. 
+0002c830: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
+0002c840: 7365 6c66 293a 0a20 2020 2020 2020 2069  self):.        i
+0002c850: 6620 7365 6c66 2e74 656e 736f 7262 6f61  f self.tensorboa
+0002c860: 7264 733a 0a20 2020 2020 2020 2020 2020  rds:.           
+0002c870: 2066 6f72 206b 2069 6e20 7365 6c66 2e74   for k in self.t
+0002c880: 656e 736f 7262 6f61 7264 733a 0a20 2020  ensorboards:.   
+0002c890: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0002c8a0: 6b3a 0a20 2020 2020 2020 2020 2020 2020  k:.             
+0002c8b0: 2020 2020 2020 206b 2e76 616c 6964 6174         k.validat
+0002c8c0: 6528 290a 0a20 2020 2064 6566 2074 6f5f  e()..    def to_
+0002c8d0: 6d61 7028 7365 6c66 293a 0a20 2020 2020  map(self):.     
+0002c8e0: 2020 205f 6d61 7020 3d20 7375 7065 7228     _map = super(
+0002c8f0: 4c69 7374 5465 6e73 6f72 626f 6172 6473  ListTensorboards
+0002c900: 5265 7370 6f6e 7365 426f 6479 2c20 7365  ResponseBody, se
+0002c910: 6c66 292e 746f 5f6d 6170 2829 0a20 2020  lf).to_map().   
+0002c920: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
+0002c930: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0002c940: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
+0002c950: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
+0002c960: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
+0002c970: 2020 2069 6620 7365 6c66 2e72 6571 7565     if self.reque
+0002c980: 7374 5f69 6420 6973 206e 6f74 204e 6f6e  st_id is not Non
+0002c990: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0002c9a0: 6573 756c 745b 2752 6571 7565 7374 4964  esult['RequestId
+0002c9b0: 275d 203d 2073 656c 662e 7265 7175 6573  '] = self.reques
+0002c9c0: 745f 6964 0a20 2020 2020 2020 2072 6573  t_id.        res
+0002c9d0: 756c 745b 2754 656e 736f 7262 6f61 7264  ult['Tensorboard
+0002c9e0: 7327 5d20 3d20 5b5d 0a20 2020 2020 2020  s'] = [].       
+0002c9f0: 2069 6620 7365 6c66 2e74 656e 736f 7262   if self.tensorb
+0002ca00: 6f61 7264 7320 6973 206e 6f74 204e 6f6e  oards is not Non
+0002ca10: 653a 0a20 2020 2020 2020 2020 2020 2066  e:.            f
+0002ca20: 6f72 206b 2069 6e20 7365 6c66 2e74 656e  or k in self.ten
+0002ca30: 736f 7262 6f61 7264 733a 0a20 2020 2020  sorboards:.     
+0002ca40: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+0002ca50: 745b 2754 656e 736f 7262 6f61 7264 7327  t['Tensorboards'
+0002ca60: 5d2e 6170 7065 6e64 286b 2e74 6f5f 6d61  ].append(k.to_ma
+0002ca70: 7028 2920 6966 206b 2065 6c73 6520 4e6f  p() if k else No
+0002ca80: 6e65 290a 2020 2020 2020 2020 6966 2073  ne).        if s
+0002ca90: 656c 662e 746f 7461 6c5f 636f 756e 7420  elf.total_count 
+0002caa0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0002cab0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+0002cac0: 2754 6f74 616c 436f 756e 7427 5d20 3d20  'TotalCount'] = 
+0002cad0: 7365 6c66 2e74 6f74 616c 5f63 6f75 6e74  self.total_count
+0002cae0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0002caf0: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
+0002cb00: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
+0002cb10: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
+0002cb20: 6d20 3d20 6d20 6f72 2064 6963 7428 290a  m = m or dict().
+0002cb30: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+0002cb40: 2827 5265 7175 6573 7449 6427 2920 6973  ('RequestId') is
+0002cb50: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0002cb60: 2020 2020 2020 2073 656c 662e 7265 7175         self.requ
+0002cb70: 6573 745f 6964 203d 206d 2e67 6574 2827  est_id = m.get('
+0002cb80: 5265 7175 6573 7449 6427 290a 2020 2020  RequestId').    
+0002cb90: 2020 2020 7365 6c66 2e74 656e 736f 7262      self.tensorb
+0002cba0: 6f61 7264 7320 3d20 5b5d 0a20 2020 2020  oards = [].     
+0002cbb0: 2020 2069 6620 6d2e 6765 7428 2754 656e     if m.get('Ten
+0002cbc0: 736f 7262 6f61 7264 7327 2920 6973 206e  sorboards') is n
+0002cbd0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0002cbe0: 2020 2020 2066 6f72 206b 2069 6e20 6d2e       for k in m.
+0002cbf0: 6765 7428 2754 656e 736f 7262 6f61 7264  get('Tensorboard
+0002cc00: 7327 293a 0a20 2020 2020 2020 2020 2020  s'):.           
+0002cc10: 2020 2020 2074 656d 705f 6d6f 6465 6c20       temp_model 
+0002cc20: 3d20 5465 6e73 6f72 626f 6172 6428 290a  = Tensorboard().
+0002cc30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0002cc40: 7365 6c66 2e74 656e 736f 7262 6f61 7264  self.tensorboard
+0002cc50: 732e 6170 7065 6e64 2874 656d 705f 6d6f  s.append(temp_mo
+0002cc60: 6465 6c2e 6672 6f6d 5f6d 6170 286b 2929  del.from_map(k))
+0002cc70: 0a20 2020 2020 2020 2069 6620 6d2e 6765  .        if m.ge
+0002cc80: 7428 2754 6f74 616c 436f 756e 7427 2920  t('TotalCount') 
+0002cc90: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0002cca0: 2020 2020 2020 2020 2073 656c 662e 746f           self.to
+0002ccb0: 7461 6c5f 636f 756e 7420 3d20 6d2e 6765  tal_count = m.ge
+0002ccc0: 7428 2754 6f74 616c 436f 756e 7427 290a  t('TotalCount').
+0002ccd0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0002cce0: 656c 660a 0a0a 636c 6173 7320 4c69 7374  elf...class List
+0002ccf0: 5465 6e73 6f72 626f 6172 6473 5265 7370  TensorboardsResp
+0002cd00: 6f6e 7365 2854 6561 4d6f 6465 6c29 3a0a  onse(TeaModel):.
+0002cd10: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+0002cd20: 2873 656c 662c 2068 6561 6465 7273 3d4e  (self, headers=N
+0002cd30: 6f6e 652c 2073 7461 7475 735f 636f 6465  one, status_code
+0002cd40: 3d4e 6f6e 652c 2062 6f64 793d 4e6f 6e65  =None, body=None
+0002cd50: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+0002cd60: 6865 6164 6572 7320 3d20 6865 6164 6572  headers = header
+0002cd70: 7320 2023 2074 7970 653a 2064 6963 745b  s  # type: dict[
+0002cd80: 7374 722c 2073 7472 5d0a 2020 2020 2020  str, str].      
+0002cd90: 2020 7365 6c66 2e73 7461 7475 735f 636f    self.status_co
+0002cda0: 6465 203d 2073 7461 7475 735f 636f 6465  de = status_code
+0002cdb0: 2020 2320 7479 7065 3a20 696e 740a 2020    # type: int.  
+0002cdc0: 2020 2020 2020 7365 6c66 2e62 6f64 7920        self.body 
+0002cdd0: 3d20 626f 6479 2020 2320 7479 7065 3a20  = body  # type: 
+0002cde0: 4c69 7374 5465 6e73 6f72 626f 6172 6473  ListTensorboards
+0002cdf0: 5265 7370 6f6e 7365 426f 6479 0a0a 2020  ResponseBody..  
+0002ce00: 2020 6465 6620 7661 6c69 6461 7465 2873    def validate(s
+0002ce10: 656c 6629 3a0a 2020 2020 2020 2020 7365  elf):.        se
+0002ce20: 6c66 2e76 616c 6964 6174 655f 7265 7175  lf.validate_requ
+0002ce30: 6972 6564 2873 656c 662e 6865 6164 6572  ired(self.header
+0002ce40: 732c 2027 6865 6164 6572 7327 290a 2020  s, 'headers').  
+0002ce50: 2020 2020 2020 7365 6c66 2e76 616c 6964        self.valid
+0002ce60: 6174 655f 7265 7175 6972 6564 2873 656c  ate_required(sel
+0002ce70: 662e 7374 6174 7573 5f63 6f64 652c 2027  f.status_code, '
+0002ce80: 7374 6174 7573 5f63 6f64 6527 290a 2020  status_code').  
+0002ce90: 2020 2020 2020 7365 6c66 2e76 616c 6964        self.valid
+0002cea0: 6174 655f 7265 7175 6972 6564 2873 656c  ate_required(sel
+0002ceb0: 662e 626f 6479 2c20 2762 6f64 7927 290a  f.body, 'body').
+0002cec0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0002ced0: 626f 6479 3a0a 2020 2020 2020 2020 2020  body:.          
+0002cee0: 2020 7365 6c66 2e62 6f64 792e 7661 6c69    self.body.vali
+0002cef0: 6461 7465 2829 0a0a 2020 2020 6465 6620  date()..    def 
+0002cf00: 746f 5f6d 6170 2873 656c 6629 3a0a 2020  to_map(self):.  
+0002cf10: 2020 2020 2020 5f6d 6170 203d 2073 7570        _map = sup
+0002cf20: 6572 284c 6973 7454 656e 736f 7262 6f61  er(ListTensorboa
+0002cf30: 7264 7352 6573 706f 6e73 652c 2073 656c  rdsResponse, sel
+0002cf40: 6629 2e74 6f5f 6d61 7028 290a 2020 2020  f).to_map().    
+0002cf50: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
+0002cf60: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0002cf70: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
+0002cf80: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
+0002cf90: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
+0002cfa0: 2020 6966 2073 656c 662e 6865 6164 6572    if self.header
+0002cfb0: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
+0002cfc0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+0002cfd0: 745b 2768 6561 6465 7273 275d 203d 2073  t['headers'] = s
+0002cfe0: 656c 662e 6865 6164 6572 730a 2020 2020  elf.headers.    
+0002cff0: 2020 2020 6966 2073 656c 662e 7374 6174      if self.stat
+0002d000: 7573 5f63 6f64 6520 6973 206e 6f74 204e  us_code is not N
+0002d010: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0002d020: 2072 6573 756c 745b 2773 7461 7475 7343   result['statusC
+0002d030: 6f64 6527 5d20 3d20 7365 6c66 2e73 7461  ode'] = self.sta
+0002d040: 7475 735f 636f 6465 0a20 2020 2020 2020  tus_code.       
+0002d050: 2069 6620 7365 6c66 2e62 6f64 7920 6973   if self.body is
+0002d060: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0002d070: 2020 2020 2020 2072 6573 756c 745b 2762         result['b
+0002d080: 6f64 7927 5d20 3d20 7365 6c66 2e62 6f64  ody'] = self.bod
+0002d090: 792e 746f 5f6d 6170 2829 0a20 2020 2020  y.to_map().     
+0002d0a0: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
+0002d0b0: 0a0a 2020 2020 6465 6620 6672 6f6d 5f6d  ..    def from_m
+0002d0c0: 6170 2873 656c 662c 206d 3d4e 6f6e 6529  ap(self, m=None)
+0002d0d0: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
+0002d0e0: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
+0002d0f0: 2020 6966 206d 2e67 6574 2827 6865 6164    if m.get('head
+0002d100: 6572 7327 2920 6973 206e 6f74 204e 6f6e  ers') is not Non
+0002d110: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0002d120: 656c 662e 6865 6164 6572 7320 3d20 6d2e  elf.headers = m.
+0002d130: 6765 7428 2768 6561 6465 7273 2729 0a20  get('headers'). 
+0002d140: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+0002d150: 2773 7461 7475 7343 6f64 6527 2920 6973  'statusCode') is
+0002d160: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0002d170: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
+0002d180: 7573 5f63 6f64 6520 3d20 6d2e 6765 7428  us_code = m.get(
+0002d190: 2773 7461 7475 7343 6f64 6527 290a 2020  'statusCode').  
+0002d1a0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+0002d1b0: 626f 6479 2729 2069 7320 6e6f 7420 4e6f  body') is not No
+0002d1c0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0002d1d0: 7465 6d70 5f6d 6f64 656c 203d 204c 6973  temp_model = Lis
+0002d1e0: 7454 656e 736f 7262 6f61 7264 7352 6573  tTensorboardsRes
+0002d1f0: 706f 6e73 6542 6f64 7928 290a 2020 2020  ponseBody().    
+0002d200: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
+0002d210: 7920 3d20 7465 6d70 5f6d 6f64 656c 2e66  y = temp_model.f
+0002d220: 726f 6d5f 6d61 7028 6d5b 2762 6f64 7927  rom_map(m['body'
+0002d230: 5d29 0a20 2020 2020 2020 2072 6574 7572  ]).        retur
+0002d240: 6e20 7365 6c66 0a0a 0a63 6c61 7373 2053  n self...class S
+0002d250: 7461 7274 5465 6e73 6f72 626f 6172 6452  tartTensorboardR
+0002d260: 6571 7565 7374 2854 6561 4d6f 6465 6c29  equest(TeaModel)
+0002d270: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
+0002d280: 5f5f 2873 656c 662c 2077 6f72 6b73 7061  __(self, workspa
+0002d290: 6365 5f69 643d 4e6f 6e65 293a 0a20 2020  ce_id=None):.   
+0002d2a0: 2020 2020 2073 656c 662e 776f 726b 7370       self.worksp
+0002d2b0: 6163 655f 6964 203d 2077 6f72 6b73 7061  ace_id = workspa
+0002d2c0: 6365 5f69 6420 2023 2074 7970 653a 2073  ce_id  # type: s
+0002d2d0: 7472 0a0a 2020 2020 6465 6620 7661 6c69  tr..    def vali
+0002d2e0: 6461 7465 2873 656c 6629 3a0a 2020 2020  date(self):.    
+0002d2f0: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
+0002d300: 6620 746f 5f6d 6170 2873 656c 6629 3a0a  f to_map(self):.
+0002d310: 2020 2020 2020 2020 5f6d 6170 203d 2073          _map = s
+0002d320: 7570 6572 2853 7461 7274 5465 6e73 6f72  uper(StartTensor
+0002d330: 626f 6172 6452 6571 7565 7374 2c20 7365  boardRequest, se
+0002d340: 6c66 292e 746f 5f6d 6170 2829 0a20 2020  lf).to_map().   
+0002d350: 2020 2020 2069 6620 5f6d 6170 2069 7320       if _map is 
+0002d360: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0002d370: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
+0002d380: 700a 0a20 2020 2020 2020 2072 6573 756c  p..        resul
+0002d390: 7420 3d20 6469 6374 2829 0a20 2020 2020  t = dict().     
+0002d3a0: 2020 2069 6620 7365 6c66 2e77 6f72 6b73     if self.works
+0002d3b0: 7061 6365 5f69 6420 6973 206e 6f74 204e  pace_id is not N
+0002d3c0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0002d3d0: 2072 6573 756c 745b 2757 6f72 6b73 7061   result['Workspa
+0002d3e0: 6365 4964 275d 203d 2073 656c 662e 776f  ceId'] = self.wo
+0002d3f0: 726b 7370 6163 655f 6964 0a20 2020 2020  rkspace_id.     
+0002d400: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
+0002d410: 0a0a 2020 2020 6465 6620 6672 6f6d 5f6d  ..    def from_m
+0002d420: 6170 2873 656c 662c 206d 3d4e 6f6e 6529  ap(self, m=None)
+0002d430: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
+0002d440: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
+0002d450: 2020 6966 206d 2e67 6574 2827 576f 726b    if m.get('Work
+0002d460: 7370 6163 6549 6427 2920 6973 206e 6f74  spaceId') is not
+0002d470: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0002d480: 2020 2073 656c 662e 776f 726b 7370 6163     self.workspac
+0002d490: 655f 6964 203d 206d 2e67 6574 2827 576f  e_id = m.get('Wo
+0002d4a0: 726b 7370 6163 6549 6427 290a 2020 2020  rkspaceId').    
+0002d4b0: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
+0002d4c0: 0a0a 636c 6173 7320 5374 6172 7454 656e  ..class StartTen
+0002d4d0: 736f 7262 6f61 7264 5265 7370 6f6e 7365  sorboardResponse
+0002d4e0: 426f 6479 2854 6561 4d6f 6465 6c29 3a0a  Body(TeaModel):.
+0002d4f0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+0002d500: 2873 656c 662c 2072 6571 7565 7374 5f69  (self, request_i
+0002d510: 643d 4e6f 6e65 2c20 7465 6e73 6f72 626f  d=None, tensorbo
+0002d520: 6172 645f 6964 3d4e 6f6e 6529 3a0a 2020  ard_id=None):.  
+0002d530: 2020 2020 2020 7365 6c66 2e72 6571 7565        self.reque
+0002d540: 7374 5f69 6420 3d20 7265 7175 6573 745f  st_id = request_
+0002d550: 6964 2020 2320 7479 7065 3a20 7374 720a  id  # type: str.
+0002d560: 2020 2020 2020 2020 7365 6c66 2e74 656e          self.ten
+0002d570: 736f 7262 6f61 7264 5f69 6420 3d20 7465  sorboard_id = te
+0002d580: 6e73 6f72 626f 6172 645f 6964 2020 2320  nsorboard_id  # 
+0002d590: 7479 7065 3a20 7374 720a 0a20 2020 2064  type: str..    d
+0002d5a0: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
+0002d5b0: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
+0002d5c0: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
+0002d5d0: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
+0002d5e0: 6d61 7020 3d20 7375 7065 7228 5374 6172  map = super(Star
+0002d5f0: 7454 656e 736f 7262 6f61 7264 5265 7370  tTensorboardResp
+0002d600: 6f6e 7365 426f 6479 2c20 7365 6c66 292e  onseBody, self).
+0002d610: 746f 5f6d 6170 2829 0a20 2020 2020 2020  to_map().       
+0002d620: 2069 6620 5f6d 6170 2069 7320 6e6f 7420   if _map is not 
+0002d630: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0002d640: 2020 7265 7475 726e 205f 6d61 700a 0a20    return _map.. 
+0002d650: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+0002d660: 6469 6374 2829 0a20 2020 2020 2020 2069  dict().        i
+0002d670: 6620 7365 6c66 2e72 6571 7565 7374 5f69  f self.request_i
+0002d680: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
+0002d690: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+0002d6a0: 745b 2752 6571 7565 7374 4964 275d 203d  t['RequestId'] =
+0002d6b0: 2073 656c 662e 7265 7175 6573 745f 6964   self.request_id
+0002d6c0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0002d6d0: 2e74 656e 736f 7262 6f61 7264 5f69 6420  .tensorboard_id 
+0002d6e0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0002d6f0: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+0002d700: 2754 656e 736f 7262 6f61 7264 4964 275d  'TensorboardId']
+0002d710: 203d 2073 656c 662e 7465 6e73 6f72 626f   = self.tensorbo
+0002d720: 6172 645f 6964 0a20 2020 2020 2020 2072  ard_id.        r
+0002d730: 6574 7572 6e20 7265 7375 6c74 0a0a 2020  eturn result..  
+0002d740: 2020 6465 6620 6672 6f6d 5f6d 6170 2873    def from_map(s
+0002d750: 656c 662c 206d 3d4e 6f6e 6529 3a0a 2020  elf, m=None):.  
+0002d760: 2020 2020 2020 6d20 3d20 6d20 6f72 2064        m = m or d
+0002d770: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+0002d780: 206d 2e67 6574 2827 5265 7175 6573 7449   m.get('RequestI
+0002d790: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
+0002d7a0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0002d7b0: 662e 7265 7175 6573 745f 6964 203d 206d  f.request_id = m
+0002d7c0: 2e67 6574 2827 5265 7175 6573 7449 6427  .get('RequestId'
+0002d7d0: 290a 2020 2020 2020 2020 6966 206d 2e67  ).        if m.g
+0002d7e0: 6574 2827 5465 6e73 6f72 626f 6172 6449  et('TensorboardI
+0002d7f0: 6427 2920 6973 206e 6f74 204e 6f6e 653a  d') is not None:
+0002d800: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0002d810: 662e 7465 6e73 6f72 626f 6172 645f 6964  f.tensorboard_id
+0002d820: 203d 206d 2e67 6574 2827 5465 6e73 6f72   = m.get('Tensor
+0002d830: 626f 6172 6449 6427 290a 2020 2020 2020  boardId').      
+0002d840: 2020 7265 7475 726e 2073 656c 660a 0a0a    return self...
+0002d850: 636c 6173 7320 5374 6172 7454 656e 736f  class StartTenso
+0002d860: 7262 6f61 7264 5265 7370 6f6e 7365 2854  rboardResponse(T
+0002d870: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
+0002d880: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
+0002d890: 2068 6561 6465 7273 3d4e 6f6e 652c 2073   headers=None, s
+0002d8a0: 7461 7475 735f 636f 6465 3d4e 6f6e 652c  tatus_code=None,
+0002d8b0: 2062 6f64 793d 4e6f 6e65 293a 0a20 2020   body=None):.   
+0002d8c0: 2020 2020 2073 656c 662e 6865 6164 6572       self.header
+0002d8d0: 7320 3d20 6865 6164 6572 7320 2023 2074  s = headers  # t
+0002d8e0: 7970 653a 2064 6963 745b 7374 722c 2073  ype: dict[str, s
+0002d8f0: 7472 5d0a 2020 2020 2020 2020 7365 6c66  tr].        self
+0002d900: 2e73 7461 7475 735f 636f 6465 203d 2073  .status_code = s
+0002d910: 7461 7475 735f 636f 6465 2020 2320 7479  tatus_code  # ty
+0002d920: 7065 3a20 696e 740a 2020 2020 2020 2020  pe: int.        
+0002d930: 7365 6c66 2e62 6f64 7920 3d20 626f 6479  self.body = body
+0002d940: 2020 2320 7479 7065 3a20 5374 6172 7454    # type: StartT
+0002d950: 656e 736f 7262 6f61 7264 5265 7370 6f6e  ensorboardRespon
+0002d960: 7365 426f 6479 0a0a 2020 2020 6465 6620  seBody..    def 
+0002d970: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
+0002d980: 2020 2020 2020 2020 7365 6c66 2e76 616c          self.val
+0002d990: 6964 6174 655f 7265 7175 6972 6564 2873  idate_required(s
+0002d9a0: 656c 662e 6865 6164 6572 732c 2027 6865  elf.headers, 'he
+0002d9b0: 6164 6572 7327 290a 2020 2020 2020 2020  aders').        
+0002d9c0: 7365 6c66 2e76 616c 6964 6174 655f 7265  self.validate_re
+0002d9d0: 7175 6972 6564 2873 656c 662e 7374 6174  quired(self.stat
+0002d9e0: 7573 5f63 6f64 652c 2027 7374 6174 7573  us_code, 'status
+0002d9f0: 5f63 6f64 6527 290a 2020 2020 2020 2020  _code').        
+0002da00: 7365 6c66 2e76 616c 6964 6174 655f 7265  self.validate_re
+0002da10: 7175 6972 6564 2873 656c 662e 626f 6479  quired(self.body
+0002da20: 2c20 2762 6f64 7927 290a 2020 2020 2020  , 'body').      
+0002da30: 2020 6966 2073 656c 662e 626f 6479 3a0a    if self.body:.
+0002da40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0002da50: 2e62 6f64 792e 7661 6c69 6461 7465 2829  .body.validate()
+0002da60: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
+0002da70: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0002da80: 5f6d 6170 203d 2073 7570 6572 2853 7461  _map = super(Sta
+0002da90: 7274 5465 6e73 6f72 626f 6172 6452 6573  rtTensorboardRes
+0002daa0: 706f 6e73 652c 2073 656c 6629 2e74 6f5f  ponse, self).to_
+0002dab0: 6d61 7028 290a 2020 2020 2020 2020 6966  map().        if
+0002dac0: 205f 6d61 7020 6973 206e 6f74 204e 6f6e   _map is not Non
+0002dad0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0002dae0: 6574 7572 6e20 5f6d 6170 0a0a 2020 2020  eturn _map..    
+0002daf0: 2020 2020 7265 7375 6c74 203d 2064 6963      result = dic
+0002db00: 7428 290a 2020 2020 2020 2020 6966 2073  t().        if s
+0002db10: 656c 662e 6865 6164 6572 7320 6973 206e  elf.headers is n
+0002db20: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0002db30: 2020 2020 2072 6573 756c 745b 2768 6561       result['hea
+0002db40: 6465 7273 275d 203d 2073 656c 662e 6865  ders'] = self.he
+0002db50: 6164 6572 730a 2020 2020 2020 2020 6966  aders.        if
+0002db60: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
+0002db70: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
+0002db80: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+0002db90: 745b 2773 7461 7475 7343 6f64 6527 5d20  t['statusCode'] 
+0002dba0: 3d20 7365 6c66 2e73 7461 7475 735f 636f  = self.status_co
+0002dbb0: 6465 0a20 2020 2020 2020 2069 6620 7365  de.        if se
+0002dbc0: 6c66 2e62 6f64 7920 6973 206e 6f74 204e  lf.body is not N
+0002dbd0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0002dbe0: 2072 6573 756c 745b 2762 6f64 7927 5d20   result['body'] 
+0002dbf0: 3d20 7365 6c66 2e62 6f64 792e 746f 5f6d  = self.body.to_m
+0002dc00: 6170 2829 0a20 2020 2020 2020 2072 6574  ap().        ret
+0002dc10: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
+0002dc20: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
+0002dc30: 662c 206d 3d4e 6f6e 6529 3a0a 2020 2020  f, m=None):.    
+0002dc40: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
+0002dc50: 7428 290a 2020 2020 2020 2020 6966 206d  t().        if m
+0002dc60: 2e67 6574 2827 6865 6164 6572 7327 2920  .get('headers') 
+0002dc70: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0002dc80: 2020 2020 2020 2020 2073 656c 662e 6865           self.he
+0002dc90: 6164 6572 7320 3d20 6d2e 6765 7428 2768  aders = m.get('h
+0002dca0: 6561 6465 7273 2729 0a20 2020 2020 2020  eaders').       
+0002dcb0: 2069 6620 6d2e 6765 7428 2773 7461 7475   if m.get('statu
+0002dcc0: 7343 6f64 6527 2920 6973 206e 6f74 204e  sCode') is not N
+0002dcd0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0002dce0: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
+0002dcf0: 6520 3d20 6d2e 6765 7428 2773 7461 7475  e = m.get('statu
+0002dd00: 7343 6f64 6527 290a 2020 2020 2020 2020  sCode').        
+0002dd10: 6966 206d 2e67 6574 2827 626f 6479 2729  if m.get('body')
+0002dd20: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0002dd30: 2020 2020 2020 2020 2020 7465 6d70 5f6d            temp_m
+0002dd40: 6f64 656c 203d 2053 7461 7274 5465 6e73  odel = StartTens
+0002dd50: 6f72 626f 6172 6452 6573 706f 6e73 6542  orboardResponseB
+0002dd60: 6f64 7928 290a 2020 2020 2020 2020 2020  ody().          
+0002dd70: 2020 7365 6c66 2e62 6f64 7920 3d20 7465    self.body = te
+0002dd80: 6d70 5f6d 6f64 656c 2e66 726f 6d5f 6d61  mp_model.from_ma
+0002dd90: 7028 6d5b 2762 6f64 7927 5d29 0a20 2020  p(m['body']).   
+0002dda0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+0002ddb0: 0a0a 0a63 6c61 7373 2053 746f 704a 6f62  ...class StopJob
+0002ddc0: 5265 7370 6f6e 7365 426f 6479 2854 6561  ResponseBody(Tea
+0002ddd0: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
+0002dde0: 5f5f 696e 6974 5f5f 2873 656c 662c 206a  __init__(self, j
+0002ddf0: 6f62 5f69 643d 4e6f 6e65 2c20 7265 7175  ob_id=None, requ
+0002de00: 6573 745f 6964 3d4e 6f6e 6529 3a0a 2020  est_id=None):.  
+0002de10: 2020 2020 2020 7365 6c66 2e6a 6f62 5f69        self.job_i
+0002de20: 6420 3d20 6a6f 625f 6964 2020 2320 7479  d = job_id  # ty
+0002de30: 7065 3a20 7374 720a 2020 2020 2020 2020  pe: str.        
+0002de40: 7365 6c66 2e72 6571 7565 7374 5f69 6420  self.request_id 
+0002de50: 3d20 7265 7175 6573 745f 6964 2020 2320  = request_id  # 
+0002de60: 7479 7065 3a20 7374 720a 0a20 2020 2064  type: str..    d
+0002de70: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
+0002de80: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
+0002de90: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
+0002dea0: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
+0002deb0: 6d61 7020 3d20 7375 7065 7228 5374 6f70  map = super(Stop
+0002dec0: 4a6f 6252 6573 706f 6e73 6542 6f64 792c  JobResponseBody,
+0002ded0: 2073 656c 6629 2e74 6f5f 6d61 7028 290a   self).to_map().
+0002dee0: 2020 2020 2020 2020 6966 205f 6d61 7020          if _map 
+0002def0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0002df00: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0002df10: 5f6d 6170 0a0a 2020 2020 2020 2020 7265  _map..        re
+0002df20: 7375 6c74 203d 2064 6963 7428 290a 2020  sult = dict().  
+0002df30: 2020 2020 2020 6966 2073 656c 662e 6a6f        if self.jo
+0002df40: 625f 6964 2069 7320 6e6f 7420 4e6f 6e65  b_id is not None
+0002df50: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0002df60: 7375 6c74 5b27 4a6f 6249 6427 5d20 3d20  sult['JobId'] = 
+0002df70: 7365 6c66 2e6a 6f62 5f69 640a 2020 2020  self.job_id.    
+0002df80: 2020 2020 6966 2073 656c 662e 7265 7175      if self.requ
+0002df90: 6573 745f 6964 2069 7320 6e6f 7420 4e6f  est_id is not No
+0002dfa0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0002dfb0: 7265 7375 6c74 5b27 5265 7175 6573 7449  result['RequestI
+0002dfc0: 6427 5d20 3d20 7365 6c66 2e72 6571 7565  d'] = self.reque
+0002dfd0: 7374 5f69 640a 2020 2020 2020 2020 7265  st_id.        re
+0002dfe0: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
+0002dff0: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
+0002e000: 6c66 2c20 6d3d 4e6f 6e65 293a 0a20 2020  lf, m=None):.   
+0002e010: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
+0002e020: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+0002e030: 6d2e 6765 7428 274a 6f62 4964 2729 2069  m.get('JobId') i
+0002e040: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+0002e050: 2020 2020 2020 2020 7365 6c66 2e6a 6f62          self.job
+0002e060: 5f69 6420 3d20 6d2e 6765 7428 274a 6f62  _id = m.get('Job
+0002e070: 4964 2729 0a20 2020 2020 2020 2069 6620  Id').        if 
+0002e080: 6d2e 6765 7428 2752 6571 7565 7374 4964  m.get('RequestId
+0002e090: 2729 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ') is not None:.
+0002e0a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0002e0b0: 2e72 6571 7565 7374 5f69 6420 3d20 6d2e  .request_id = m.
+0002e0c0: 6765 7428 2752 6571 7565 7374 4964 2729  get('RequestId')
+0002e0d0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0002e0e0: 7365 6c66 0a0a 0a63 6c61 7373 2053 746f  self...class Sto
+0002e0f0: 704a 6f62 5265 7370 6f6e 7365 2854 6561  pJobResponse(Tea
+0002e100: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
+0002e110: 5f5f 696e 6974 5f5f 2873 656c 662c 2068  __init__(self, h
+0002e120: 6561 6465 7273 3d4e 6f6e 652c 2073 7461  eaders=None, sta
+0002e130: 7475 735f 636f 6465 3d4e 6f6e 652c 2062  tus_code=None, b
+0002e140: 6f64 793d 4e6f 6e65 293a 0a20 2020 2020  ody=None):.     
+0002e150: 2020 2073 656c 662e 6865 6164 6572 7320     self.headers 
+0002e160: 3d20 6865 6164 6572 7320 2023 2074 7970  = headers  # typ
+0002e170: 653a 2064 6963 745b 7374 722c 2073 7472  e: dict[str, str
+0002e180: 5d0a 2020 2020 2020 2020 7365 6c66 2e73  ].        self.s
+0002e190: 7461 7475 735f 636f 6465 203d 2073 7461  tatus_code = sta
+0002e1a0: 7475 735f 636f 6465 2020 2320 7479 7065  tus_code  # type
+0002e1b0: 3a20 696e 740a 2020 2020 2020 2020 7365  : int.        se
+0002e1c0: 6c66 2e62 6f64 7920 3d20 626f 6479 2020  lf.body = body  
+0002e1d0: 2320 7479 7065 3a20 5374 6f70 4a6f 6252  # type: StopJobR
+0002e1e0: 6573 706f 6e73 6542 6f64 790a 0a20 2020  esponseBody..   
+0002e1f0: 2064 6566 2076 616c 6964 6174 6528 7365   def validate(se
+0002e200: 6c66 293a 0a20 2020 2020 2020 2073 656c  lf):.        sel
+0002e210: 662e 7661 6c69 6461 7465 5f72 6571 7569  f.validate_requi
+0002e220: 7265 6428 7365 6c66 2e68 6561 6465 7273  red(self.headers
+0002e230: 2c20 2768 6561 6465 7273 2729 0a20 2020  , 'headers').   
+0002e240: 2020 2020 2073 656c 662e 7661 6c69 6461       self.valida
+0002e250: 7465 5f72 6571 7569 7265 6428 7365 6c66  te_required(self
+0002e260: 2e73 7461 7475 735f 636f 6465 2c20 2773  .status_code, 's
+0002e270: 7461 7475 735f 636f 6465 2729 0a20 2020  tatus_code').   
+0002e280: 2020 2020 2073 656c 662e 7661 6c69 6461       self.valida
+0002e290: 7465 5f72 6571 7569 7265 6428 7365 6c66  te_required(self
+0002e2a0: 2e62 6f64 792c 2027 626f 6479 2729 0a20  .body, 'body'). 
+0002e2b0: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
+0002e2c0: 6f64 793a 0a20 2020 2020 2020 2020 2020  ody:.           
+0002e2d0: 2073 656c 662e 626f 6479 2e76 616c 6964   self.body.valid
+0002e2e0: 6174 6528 290a 0a20 2020 2064 6566 2074  ate()..    def t
+0002e2f0: 6f5f 6d61 7028 7365 6c66 293a 0a20 2020  o_map(self):.   
+0002e300: 2020 2020 205f 6d61 7020 3d20 7375 7065       _map = supe
+0002e310: 7228 5374 6f70 4a6f 6252 6573 706f 6e73  r(StopJobRespons
+0002e320: 652c 2073 656c 6629 2e74 6f5f 6d61 7028  e, self).to_map(
+0002e330: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
+0002e340: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
+0002e350: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0002e360: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
+0002e370: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
+0002e380: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0002e390: 6865 6164 6572 7320 6973 206e 6f74 204e  headers is not N
+0002e3a0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0002e3b0: 2072 6573 756c 745b 2768 6561 6465 7273   result['headers
+0002e3c0: 275d 203d 2073 656c 662e 6865 6164 6572  '] = self.header
+0002e3d0: 730a 2020 2020 2020 2020 6966 2073 656c  s.        if sel
+0002e3e0: 662e 7374 6174 7573 5f63 6f64 6520 6973  f.status_code is
+0002e3f0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0002e400: 2020 2020 2020 2072 6573 756c 745b 2773         result['s
+0002e410: 7461 7475 7343 6f64 6527 5d20 3d20 7365  tatusCode'] = se
+0002e420: 6c66 2e73 7461 7475 735f 636f 6465 0a20  lf.status_code. 
+0002e430: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
+0002e440: 6f64 7920 6973 206e 6f74 204e 6f6e 653a  ody is not None:
+0002e450: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+0002e460: 756c 745b 2762 6f64 7927 5d20 3d20 7365  ult['body'] = se
+0002e470: 6c66 2e62 6f64 792e 746f 5f6d 6170 2829  lf.body.to_map()
+0002e480: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0002e490: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
+0002e4a0: 6672 6f6d 5f6d 6170 2873 656c 662c 206d  from_map(self, m
+0002e4b0: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
+0002e4c0: 6d20 3d20 6d20 6f72 2064 6963 7428 290a  m = m or dict().
+0002e4d0: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+0002e4e0: 2827 6865 6164 6572 7327 2920 6973 206e  ('headers') is n
+0002e4f0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0002e500: 2020 2020 2073 656c 662e 6865 6164 6572       self.header
+0002e510: 7320 3d20 6d2e 6765 7428 2768 6561 6465  s = m.get('heade
+0002e520: 7273 2729 0a20 2020 2020 2020 2069 6620  rs').        if 
+0002e530: 6d2e 6765 7428 2773 7461 7475 7343 6f64  m.get('statusCod
+0002e540: 6527 2920 6973 206e 6f74 204e 6f6e 653a  e') is not None:
+0002e550: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0002e560: 662e 7374 6174 7573 5f63 6f64 6520 3d20  f.status_code = 
+0002e570: 6d2e 6765 7428 2773 7461 7475 7343 6f64  m.get('statusCod
+0002e580: 6527 290a 2020 2020 2020 2020 6966 206d  e').        if m
+0002e590: 2e67 6574 2827 626f 6479 2729 2069 7320  .get('body') is 
+0002e5a0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0002e5b0: 2020 2020 2020 7465 6d70 5f6d 6f64 656c        temp_model
+0002e5c0: 203d 2053 746f 704a 6f62 5265 7370 6f6e   = StopJobRespon
+0002e5d0: 7365 426f 6479 2829 0a20 2020 2020 2020  seBody().       
+0002e5e0: 2020 2020 2073 656c 662e 626f 6479 203d       self.body =
+0002e5f0: 2074 656d 705f 6d6f 6465 6c2e 6672 6f6d   temp_model.from
+0002e600: 5f6d 6170 286d 5b27 626f 6479 275d 290a  _map(m['body']).
+0002e610: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+0002e620: 656c 660a 0a0a 636c 6173 7320 5374 6f70  elf...class Stop
+0002e630: 5465 6e73 6f72 626f 6172 6452 6571 7565  TensorboardReque
+0002e640: 7374 2854 6561 4d6f 6465 6c29 3a0a 2020  st(TeaModel):.  
+0002e650: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
+0002e660: 656c 662c 2077 6f72 6b73 7061 6365 5f69  elf, workspace_i
+0002e670: 643d 4e6f 6e65 293a 0a20 2020 2020 2020  d=None):.       
+0002e680: 2073 656c 662e 776f 726b 7370 6163 655f   self.workspace_
+0002e690: 6964 203d 2077 6f72 6b73 7061 6365 5f69  id = workspace_i
+0002e6a0: 6420 2023 2074 7970 653a 2073 7472 0a0a  d  # type: str..
+0002e6b0: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
+0002e6c0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0002e6d0: 7061 7373 0a0a 2020 2020 6465 6620 746f  pass..    def to
+0002e6e0: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
+0002e6f0: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
+0002e700: 2853 746f 7054 656e 736f 7262 6f61 7264  (StopTensorboard
+0002e710: 5265 7175 6573 742c 2073 656c 6629 2e74  Request, self).t
+0002e720: 6f5f 6d61 7028 290a 2020 2020 2020 2020  o_map().        
+0002e730: 6966 205f 6d61 7020 6973 206e 6f74 204e  if _map is not N
+0002e740: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0002e750: 2072 6574 7572 6e20 5f6d 6170 0a0a 2020   return _map..  
+0002e760: 2020 2020 2020 7265 7375 6c74 203d 2064        result = d
+0002e770: 6963 7428 290a 2020 2020 2020 2020 6966  ict().        if
+0002e780: 2073 656c 662e 776f 726b 7370 6163 655f   self.workspace_
+0002e790: 6964 2069 7320 6e6f 7420 4e6f 6e65 3a0a  id is not None:.
+0002e7a0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+0002e7b0: 6c74 5b27 576f 726b 7370 6163 6549 6427  lt['WorkspaceId'
+0002e7c0: 5d20 3d20 7365 6c66 2e77 6f72 6b73 7061  ] = self.workspa
+0002e7d0: 6365 5f69 640a 2020 2020 2020 2020 7265  ce_id.        re
+0002e7e0: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
+0002e7f0: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
+0002e800: 6c66 2c20 6d3d 4e6f 6e65 293a 0a20 2020  lf, m=None):.   
+0002e810: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
+0002e820: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+0002e830: 6d2e 6765 7428 2757 6f72 6b73 7061 6365  m.get('Workspace
+0002e840: 4964 2729 2069 7320 6e6f 7420 4e6f 6e65  Id') is not None
+0002e850: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0002e860: 6c66 2e77 6f72 6b73 7061 6365 5f69 6420  lf.workspace_id 
+0002e870: 3d20 6d2e 6765 7428 2757 6f72 6b73 7061  = m.get('Workspa
+0002e880: 6365 4964 2729 0a20 2020 2020 2020 2072  ceId').        r
+0002e890: 6574 7572 6e20 7365 6c66 0a0a 0a63 6c61  eturn self...cla
+0002e8a0: 7373 2053 746f 7054 656e 736f 7262 6f61  ss StopTensorboa
+0002e8b0: 7264 5265 7370 6f6e 7365 426f 6479 2854  rdResponseBody(T
+0002e8c0: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
+0002e8d0: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
+0002e8e0: 2072 6571 7565 7374 5f69 643d 4e6f 6e65   request_id=None
+0002e8f0: 2c20 7465 6e73 6f72 626f 6172 645f 6964  , tensorboard_id
+0002e900: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
+0002e910: 7365 6c66 2e72 6571 7565 7374 5f69 6420  self.request_id 
+0002e920: 3d20 7265 7175 6573 745f 6964 2020 2320  = request_id  # 
+0002e930: 7479 7065 3a20 7374 720a 2020 2020 2020  type: str.      
+0002e940: 2020 7365 6c66 2e74 656e 736f 7262 6f61    self.tensorboa
+0002e950: 7264 5f69 6420 3d20 7465 6e73 6f72 626f  rd_id = tensorbo
+0002e960: 6172 645f 6964 2020 2320 7479 7065 3a20  ard_id  # type: 
+0002e970: 7374 720a 0a20 2020 2064 6566 2076 616c  str..    def val
+0002e980: 6964 6174 6528 7365 6c66 293a 0a20 2020  idate(self):.   
+0002e990: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
+0002e9a0: 6566 2074 6f5f 6d61 7028 7365 6c66 293a  ef to_map(self):
+0002e9b0: 0a20 2020 2020 2020 205f 6d61 7020 3d20  .        _map = 
+0002e9c0: 7375 7065 7228 5374 6f70 5465 6e73 6f72  super(StopTensor
+0002e9d0: 626f 6172 6452 6573 706f 6e73 6542 6f64  boardResponseBod
+0002e9e0: 792c 2073 656c 6629 2e74 6f5f 6d61 7028  y, self).to_map(
+0002e9f0: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
+0002ea00: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
+0002ea10: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0002ea20: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
+0002ea30: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
+0002ea40: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0002ea50: 7265 7175 6573 745f 6964 2069 7320 6e6f  request_id is no
+0002ea60: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0002ea70: 2020 2020 7265 7375 6c74 5b27 5265 7175      result['Requ
+0002ea80: 6573 7449 6427 5d20 3d20 7365 6c66 2e72  estId'] = self.r
+0002ea90: 6571 7565 7374 5f69 640a 2020 2020 2020  equest_id.      
+0002eaa0: 2020 6966 2073 656c 662e 7465 6e73 6f72    if self.tensor
+0002eab0: 626f 6172 645f 6964 2069 7320 6e6f 7420  board_id is not 
+0002eac0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0002ead0: 2020 7265 7375 6c74 5b27 5465 6e73 6f72    result['Tensor
+0002eae0: 626f 6172 6449 6427 5d20 3d20 7365 6c66  boardId'] = self
+0002eaf0: 2e74 656e 736f 7262 6f61 7264 5f69 640a  .tensorboard_id.
+0002eb00: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+0002eb10: 6573 756c 740a 0a20 2020 2064 6566 2066  esult..    def f
+0002eb20: 726f 6d5f 6d61 7028 7365 6c66 2c20 6d3d  rom_map(self, m=
+0002eb30: 4e6f 6e65 293a 0a20 2020 2020 2020 206d  None):.        m
+0002eb40: 203d 206d 206f 7220 6469 6374 2829 0a20   = m or dict(). 
+0002eb50: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+0002eb60: 2752 6571 7565 7374 4964 2729 2069 7320  'RequestId') is 
+0002eb70: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0002eb80: 2020 2020 2020 7365 6c66 2e72 6571 7565        self.reque
+0002eb90: 7374 5f69 6420 3d20 6d2e 6765 7428 2752  st_id = m.get('R
+0002eba0: 6571 7565 7374 4964 2729 0a20 2020 2020  equestId').     
+0002ebb0: 2020 2069 6620 6d2e 6765 7428 2754 656e     if m.get('Ten
+0002ebc0: 736f 7262 6f61 7264 4964 2729 2069 7320  sorboardId') is 
+0002ebd0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0002ebe0: 2020 2020 2020 7365 6c66 2e74 656e 736f        self.tenso
+0002ebf0: 7262 6f61 7264 5f69 6420 3d20 6d2e 6765  rboard_id = m.ge
+0002ec00: 7428 2754 656e 736f 7262 6f61 7264 4964  t('TensorboardId
+0002ec10: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
+0002ec20: 6e20 7365 6c66 0a0a 0a63 6c61 7373 2053  n self...class S
+0002ec30: 746f 7054 656e 736f 7262 6f61 7264 5265  topTensorboardRe
+0002ec40: 7370 6f6e 7365 2854 6561 4d6f 6465 6c29  sponse(TeaModel)
+0002ec50: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
+0002ec60: 5f5f 2873 656c 662c 2068 6561 6465 7273  __(self, headers
+0002ec70: 3d4e 6f6e 652c 2073 7461 7475 735f 636f  =None, status_co
+0002ec80: 6465 3d4e 6f6e 652c 2062 6f64 793d 4e6f  de=None, body=No
+0002ec90: 6e65 293a 0a20 2020 2020 2020 2073 656c  ne):.        sel
+0002eca0: 662e 6865 6164 6572 7320 3d20 6865 6164  f.headers = head
+0002ecb0: 6572 7320 2023 2074 7970 653a 2064 6963  ers  # type: dic
+0002ecc0: 745b 7374 722c 2073 7472 5d0a 2020 2020  t[str, str].    
+0002ecd0: 2020 2020 7365 6c66 2e73 7461 7475 735f      self.status_
+0002ece0: 636f 6465 203d 2073 7461 7475 735f 636f  code = status_co
+0002ecf0: 6465 2020 2320 7479 7065 3a20 696e 740a  de  # type: int.
+0002ed00: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
+0002ed10: 7920 3d20 626f 6479 2020 2320 7479 7065  y = body  # type
+0002ed20: 3a20 5374 6f70 5465 6e73 6f72 626f 6172  : StopTensorboar
+0002ed30: 6452 6573 706f 6e73 6542 6f64 790a 0a20  dResponseBody.. 
+0002ed40: 2020 2064 6566 2076 616c 6964 6174 6528     def validate(
+0002ed50: 7365 6c66 293a 0a20 2020 2020 2020 2073  self):.        s
+0002ed60: 656c 662e 7661 6c69 6461 7465 5f72 6571  elf.validate_req
+0002ed70: 7569 7265 6428 7365 6c66 2e68 6561 6465  uired(self.heade
+0002ed80: 7273 2c20 2768 6561 6465 7273 2729 0a20  rs, 'headers'). 
+0002ed90: 2020 2020 2020 2073 656c 662e 7661 6c69         self.vali
+0002eda0: 6461 7465 5f72 6571 7569 7265 6428 7365  date_required(se
+0002edb0: 6c66 2e73 7461 7475 735f 636f 6465 2c20  lf.status_code, 
+0002edc0: 2773 7461 7475 735f 636f 6465 2729 0a20  'status_code'). 
+0002edd0: 2020 2020 2020 2073 656c 662e 7661 6c69         self.vali
+0002ede0: 6461 7465 5f72 6571 7569 7265 6428 7365  date_required(se
+0002edf0: 6c66 2e62 6f64 792c 2027 626f 6479 2729  lf.body, 'body')
+0002ee00: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0002ee10: 2e62 6f64 793a 0a20 2020 2020 2020 2020  .body:.         
+0002ee20: 2020 2073 656c 662e 626f 6479 2e76 616c     self.body.val
+0002ee30: 6964 6174 6528 290a 0a20 2020 2064 6566  idate()..    def
+0002ee40: 2074 6f5f 6d61 7028 7365 6c66 293a 0a20   to_map(self):. 
+0002ee50: 2020 2020 2020 205f 6d61 7020 3d20 7375         _map = su
+0002ee60: 7065 7228 5374 6f70 5465 6e73 6f72 626f  per(StopTensorbo
+0002ee70: 6172 6452 6573 706f 6e73 652c 2073 656c  ardResponse, sel
+0002ee80: 6629 2e74 6f5f 6d61 7028 290a 2020 2020  f).to_map().    
+0002ee90: 2020 2020 6966 205f 6d61 7020 6973 206e      if _map is n
+0002eea0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0002eeb0: 2020 2020 2072 6574 7572 6e20 5f6d 6170       return _map
+0002eec0: 0a0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
+0002eed0: 203d 2064 6963 7428 290a 2020 2020 2020   = dict().      
+0002eee0: 2020 6966 2073 656c 662e 6865 6164 6572    if self.header
+0002eef0: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
+0002ef00: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+0002ef10: 745b 2768 6561 6465 7273 275d 203d 2073  t['headers'] = s
+0002ef20: 656c 662e 6865 6164 6572 730a 2020 2020  elf.headers.    
+0002ef30: 2020 2020 6966 2073 656c 662e 7374 6174      if self.stat
+0002ef40: 7573 5f63 6f64 6520 6973 206e 6f74 204e  us_code is not N
+0002ef50: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0002ef60: 2072 6573 756c 745b 2773 7461 7475 7343   result['statusC
+0002ef70: 6f64 6527 5d20 3d20 7365 6c66 2e73 7461  ode'] = self.sta
+0002ef80: 7475 735f 636f 6465 0a20 2020 2020 2020  tus_code.       
+0002ef90: 2069 6620 7365 6c66 2e62 6f64 7920 6973   if self.body is
+0002efa0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0002efb0: 2020 2020 2020 2072 6573 756c 745b 2762         result['b
+0002efc0: 6f64 7927 5d20 3d20 7365 6c66 2e62 6f64  ody'] = self.bod
+0002efd0: 792e 746f 5f6d 6170 2829 0a20 2020 2020  y.to_map().     
+0002efe0: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
+0002eff0: 0a0a 2020 2020 6465 6620 6672 6f6d 5f6d  ..    def from_m
+0002f000: 6170 2873 656c 662c 206d 3d4e 6f6e 6529  ap(self, m=None)
+0002f010: 3a0a 2020 2020 2020 2020 6d20 3d20 6d20  :.        m = m 
+0002f020: 6f72 2064 6963 7428 290a 2020 2020 2020  or dict().      
+0002f030: 2020 6966 206d 2e67 6574 2827 6865 6164    if m.get('head
+0002f040: 6572 7327 2920 6973 206e 6f74 204e 6f6e  ers') is not Non
+0002f050: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0002f060: 656c 662e 6865 6164 6572 7320 3d20 6d2e  elf.headers = m.
+0002f070: 6765 7428 2768 6561 6465 7273 2729 0a20  get('headers'). 
+0002f080: 2020 2020 2020 2069 6620 6d2e 6765 7428         if m.get(
+0002f090: 2773 7461 7475 7343 6f64 6527 2920 6973  'statusCode') is
+0002f0a0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0002f0b0: 2020 2020 2020 2073 656c 662e 7374 6174         self.stat
+0002f0c0: 7573 5f63 6f64 6520 3d20 6d2e 6765 7428  us_code = m.get(
+0002f0d0: 2773 7461 7475 7343 6f64 6527 290a 2020  'statusCode').  
+0002f0e0: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+0002f0f0: 626f 6479 2729 2069 7320 6e6f 7420 4e6f  body') is not No
+0002f100: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0002f110: 7465 6d70 5f6d 6f64 656c 203d 2053 746f  temp_model = Sto
+0002f120: 7054 656e 736f 7262 6f61 7264 5265 7370  pTensorboardResp
+0002f130: 6f6e 7365 426f 6479 2829 0a20 2020 2020  onseBody().     
+0002f140: 2020 2020 2020 2073 656c 662e 626f 6479         self.body
+0002f150: 203d 2074 656d 705f 6d6f 6465 6c2e 6672   = temp_model.fr
+0002f160: 6f6d 5f6d 6170 286d 5b27 626f 6479 275d  om_map(m['body']
+0002f170: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+0002f180: 2073 656c 660a 0a0a 636c 6173 7320 5570   self...class Up
+0002f190: 6461 7465 4a6f 6252 6571 7565 7374 2854  dateJobRequest(T
+0002f1a0: 6561 4d6f 6465 6c29 3a0a 2020 2020 6465  eaModel):.    de
+0002f1b0: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
+0002f1c0: 2070 7269 6f72 6974 793d 4e6f 6e65 293a   priority=None):
+0002f1d0: 0a20 2020 2020 2020 2073 656c 662e 7072  .        self.pr
+0002f1e0: 696f 7269 7479 203d 2070 7269 6f72 6974  iority = priorit
+0002f1f0: 7920 2023 2074 7970 653a 2069 6e74 0a0a  y  # type: int..
+0002f200: 2020 2020 6465 6620 7661 6c69 6461 7465      def validate
+0002f210: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0002f220: 7061 7373 0a0a 2020 2020 6465 6620 746f  pass..    def to
+0002f230: 5f6d 6170 2873 656c 6629 3a0a 2020 2020  _map(self):.    
+0002f240: 2020 2020 5f6d 6170 203d 2073 7570 6572      _map = super
+0002f250: 2855 7064 6174 654a 6f62 5265 7175 6573  (UpdateJobReques
+0002f260: 742c 2073 656c 6629 2e74 6f5f 6d61 7028  t, self).to_map(
+0002f270: 290a 2020 2020 2020 2020 6966 205f 6d61  ).        if _ma
+0002f280: 7020 6973 206e 6f74 204e 6f6e 653a 0a20  p is not None:. 
+0002f290: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0002f2a0: 6e20 5f6d 6170 0a0a 2020 2020 2020 2020  n _map..        
+0002f2b0: 7265 7375 6c74 203d 2064 6963 7428 290a  result = dict().
+0002f2c0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0002f2d0: 7072 696f 7269 7479 2069 7320 6e6f 7420  priority is not 
+0002f2e0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0002f2f0: 2020 7265 7375 6c74 5b27 5072 696f 7269    result['Priori
+0002f300: 7479 275d 203d 2073 656c 662e 7072 696f  ty'] = self.prio
+0002f310: 7269 7479 0a20 2020 2020 2020 2072 6574  rity.        ret
+0002f320: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
+0002f330: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
+0002f340: 662c 206d 3d4e 6f6e 6529 3a0a 2020 2020  f, m=None):.    
+0002f350: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
+0002f360: 7428 290a 2020 2020 2020 2020 6966 206d  t().        if m
+0002f370: 2e67 6574 2827 5072 696f 7269 7479 2729  .get('Priority')
+0002f380: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0002f390: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
+0002f3a0: 7269 6f72 6974 7920 3d20 6d2e 6765 7428  riority = m.get(
+0002f3b0: 2750 7269 6f72 6974 7927 290a 2020 2020  'Priority').    
+0002f3c0: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
+0002f3d0: 0a0a 636c 6173 7320 5570 6461 7465 4a6f  ..class UpdateJo
+0002f3e0: 6252 6573 706f 6e73 6542 6f64 7928 5465  bResponseBody(Te
+0002f3f0: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
+0002f400: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
+0002f410: 6a6f 625f 6964 3d4e 6f6e 652c 2072 6571  job_id=None, req
+0002f420: 7565 7374 5f69 643d 4e6f 6e65 293a 0a20  uest_id=None):. 
+0002f430: 2020 2020 2020 2073 656c 662e 6a6f 625f         self.job_
+0002f440: 6964 203d 206a 6f62 5f69 6420 2023 2074  id = job_id  # t
+0002f450: 7970 653a 2073 7472 0a20 2020 2020 2020  ype: str.       
+0002f460: 2073 656c 662e 7265 7175 6573 745f 6964   self.request_id
+0002f470: 203d 2072 6571 7565 7374 5f69 6420 2023   = request_id  #
+0002f480: 2074 7970 653a 2073 7472 0a0a 2020 2020   type: str..    
+0002f490: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
+0002f4a0: 6629 3a0a 2020 2020 2020 2020 7061 7373  f):.        pass
+0002f4b0: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
+0002f4c0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0002f4d0: 5f6d 6170 203d 2073 7570 6572 2855 7064  _map = super(Upd
+0002f4e0: 6174 654a 6f62 5265 7370 6f6e 7365 426f  ateJobResponseBo
+0002f4f0: 6479 2c20 7365 6c66 292e 746f 5f6d 6170  dy, self).to_map
+0002f500: 2829 0a20 2020 2020 2020 2069 6620 5f6d  ().        if _m
+0002f510: 6170 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ap is not None:.
+0002f520: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0002f530: 726e 205f 6d61 700a 0a20 2020 2020 2020  rn _map..       
+0002f540: 2072 6573 756c 7420 3d20 6469 6374 2829   result = dict()
+0002f550: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0002f560: 2e6a 6f62 5f69 6420 6973 206e 6f74 204e  .job_id is not N
+0002f570: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0002f580: 2072 6573 756c 745b 274a 6f62 4964 275d   result['JobId']
+0002f590: 203d 2073 656c 662e 6a6f 625f 6964 0a20   = self.job_id. 
+0002f5a0: 2020 2020 2020 2069 6620 7365 6c66 2e72         if self.r
+0002f5b0: 6571 7565 7374 5f69 6420 6973 206e 6f74  equest_id is not
+0002f5c0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+0002f5d0: 2020 2072 6573 756c 745b 2752 6571 7565     result['Reque
+0002f5e0: 7374 4964 275d 203d 2073 656c 662e 7265  stId'] = self.re
+0002f5f0: 7175 6573 745f 6964 0a20 2020 2020 2020  quest_id.       
+0002f600: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
+0002f610: 2020 2020 6465 6620 6672 6f6d 5f6d 6170      def from_map
+0002f620: 2873 656c 662c 206d 3d4e 6f6e 6529 3a0a  (self, m=None):.
+0002f630: 2020 2020 2020 2020 6d20 3d20 6d20 6f72          m = m or
+0002f640: 2064 6963 7428 290a 2020 2020 2020 2020   dict().        
+0002f650: 6966 206d 2e67 6574 2827 4a6f 6249 6427  if m.get('JobId'
+0002f660: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+0002f670: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0002f680: 6a6f 625f 6964 203d 206d 2e67 6574 2827  job_id = m.get('
+0002f690: 4a6f 6249 6427 290a 2020 2020 2020 2020  JobId').        
+0002f6a0: 6966 206d 2e67 6574 2827 5265 7175 6573  if m.get('Reques
+0002f6b0: 7449 6427 2920 6973 206e 6f74 204e 6f6e  tId') is not Non
+0002f6c0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+0002f6d0: 656c 662e 7265 7175 6573 745f 6964 203d  elf.request_id =
+0002f6e0: 206d 2e67 6574 2827 5265 7175 6573 7449   m.get('RequestI
+0002f6f0: 6427 290a 2020 2020 2020 2020 7265 7475  d').        retu
+0002f700: 726e 2073 656c 660a 0a0a 636c 6173 7320  rn self...class 
+0002f710: 5570 6461 7465 4a6f 6252 6573 706f 6e73  UpdateJobRespons
+0002f720: 6528 5465 614d 6f64 656c 293a 0a20 2020  e(TeaModel):.   
+0002f730: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
+0002f740: 6c66 2c20 6865 6164 6572 733d 4e6f 6e65  lf, headers=None
+0002f750: 2c20 7374 6174 7573 5f63 6f64 653d 4e6f  , status_code=No
+0002f760: 6e65 2c20 626f 6479 3d4e 6f6e 6529 3a0a  ne, body=None):.
+0002f770: 2020 2020 2020 2020 7365 6c66 2e68 6561          self.hea
+0002f780: 6465 7273 203d 2068 6561 6465 7273 2020  ders = headers  
+0002f790: 2320 7479 7065 3a20 6469 6374 5b73 7472  # type: dict[str
+0002f7a0: 2c20 7374 725d 0a20 2020 2020 2020 2073  , str].        s
+0002f7b0: 656c 662e 7374 6174 7573 5f63 6f64 6520  elf.status_code 
+0002f7c0: 3d20 7374 6174 7573 5f63 6f64 6520 2023  = status_code  #
+0002f7d0: 2074 7970 653a 2069 6e74 0a20 2020 2020   type: int.     
+0002f7e0: 2020 2073 656c 662e 626f 6479 203d 2062     self.body = b
+0002f7f0: 6f64 7920 2023 2074 7970 653a 2055 7064  ody  # type: Upd
+0002f800: 6174 654a 6f62 5265 7370 6f6e 7365 426f  ateJobResponseBo
+0002f810: 6479 0a0a 2020 2020 6465 6620 7661 6c69  dy..    def vali
+0002f820: 6461 7465 2873 656c 6629 3a0a 2020 2020  date(self):.    
+0002f830: 2020 2020 7365 6c66 2e76 616c 6964 6174      self.validat
+0002f840: 655f 7265 7175 6972 6564 2873 656c 662e  e_required(self.
+0002f850: 6865 6164 6572 732c 2027 6865 6164 6572  headers, 'header
+0002f860: 7327 290a 2020 2020 2020 2020 7365 6c66  s').        self
+0002f870: 2e76 616c 6964 6174 655f 7265 7175 6972  .validate_requir
+0002f880: 6564 2873 656c 662e 7374 6174 7573 5f63  ed(self.status_c
+0002f890: 6f64 652c 2027 7374 6174 7573 5f63 6f64  ode, 'status_cod
+0002f8a0: 6527 290a 2020 2020 2020 2020 7365 6c66  e').        self
+0002f8b0: 2e76 616c 6964 6174 655f 7265 7175 6972  .validate_requir
+0002f8c0: 6564 2873 656c 662e 626f 6479 2c20 2762  ed(self.body, 'b
+0002f8d0: 6f64 7927 290a 2020 2020 2020 2020 6966  ody').        if
+0002f8e0: 2073 656c 662e 626f 6479 3a0a 2020 2020   self.body:.    
+0002f8f0: 2020 2020 2020 2020 7365 6c66 2e62 6f64          self.bod
+0002f900: 792e 7661 6c69 6461 7465 2829 0a0a 2020  y.validate()..  
+0002f910: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
+0002f920: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
+0002f930: 203d 2073 7570 6572 2855 7064 6174 654a   = super(UpdateJ
+0002f940: 6f62 5265 7370 6f6e 7365 2c20 7365 6c66  obResponse, self
+0002f950: 292e 746f 5f6d 6170 2829 0a20 2020 2020  ).to_map().     
+0002f960: 2020 2069 6620 5f6d 6170 2069 7320 6e6f     if _map is no
+0002f970: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0002f980: 2020 2020 7265 7475 726e 205f 6d61 700a      return _map.
+0002f990: 0a20 2020 2020 2020 2072 6573 756c 7420  .        result 
+0002f9a0: 3d20 6469 6374 2829 0a20 2020 2020 2020  = dict().       
+0002f9b0: 2069 6620 7365 6c66 2e68 6561 6465 7273   if self.headers
+0002f9c0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0002f9d0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+0002f9e0: 5b27 6865 6164 6572 7327 5d20 3d20 7365  ['headers'] = se
+0002f9f0: 6c66 2e68 6561 6465 7273 0a20 2020 2020  lf.headers.     
+0002fa00: 2020 2069 6620 7365 6c66 2e73 7461 7475     if self.statu
+0002fa10: 735f 636f 6465 2069 7320 6e6f 7420 4e6f  s_code is not No
+0002fa20: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0002fa30: 7265 7375 6c74 5b27 7374 6174 7573 436f  result['statusCo
+0002fa40: 6465 275d 203d 2073 656c 662e 7374 6174  de'] = self.stat
+0002fa50: 7573 5f63 6f64 650a 2020 2020 2020 2020  us_code.        
+0002fa60: 6966 2073 656c 662e 626f 6479 2069 7320  if self.body is 
+0002fa70: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0002fa80: 2020 2020 2020 7265 7375 6c74 5b27 626f        result['bo
+0002fa90: 6479 275d 203d 2073 656c 662e 626f 6479  dy'] = self.body
+0002faa0: 2e74 6f5f 6d61 7028 290a 2020 2020 2020  .to_map().      
+0002fab0: 2020 7265 7475 726e 2072 6573 756c 740a    return result.
+0002fac0: 0a20 2020 2064 6566 2066 726f 6d5f 6d61  .    def from_ma
+0002fad0: 7028 7365 6c66 2c20 6d3d 4e6f 6e65 293a  p(self, m=None):
+0002fae0: 0a20 2020 2020 2020 206d 203d 206d 206f  .        m = m o
+0002faf0: 7220 6469 6374 2829 0a20 2020 2020 2020  r dict().       
+0002fb00: 2069 6620 6d2e 6765 7428 2768 6561 6465   if m.get('heade
+0002fb10: 7273 2729 2069 7320 6e6f 7420 4e6f 6e65  rs') is not None
+0002fb20: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+0002fb30: 6c66 2e68 6561 6465 7273 203d 206d 2e67  lf.headers = m.g
+0002fb40: 6574 2827 6865 6164 6572 7327 290a 2020  et('headers').  
+0002fb50: 2020 2020 2020 6966 206d 2e67 6574 2827        if m.get('
+0002fb60: 7374 6174 7573 436f 6465 2729 2069 7320  statusCode') is 
+0002fb70: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0002fb80: 2020 2020 2020 7365 6c66 2e73 7461 7475        self.statu
+0002fb90: 735f 636f 6465 203d 206d 2e67 6574 2827  s_code = m.get('
+0002fba0: 7374 6174 7573 436f 6465 2729 0a20 2020  statusCode').   
+0002fbb0: 2020 2020 2069 6620 6d2e 6765 7428 2762       if m.get('b
+0002fbc0: 6f64 7927 2920 6973 206e 6f74 204e 6f6e  ody') is not Non
+0002fbd0: 653a 0a20 2020 2020 2020 2020 2020 2074  e:.            t
+0002fbe0: 656d 705f 6d6f 6465 6c20 3d20 5570 6461  emp_model = Upda
+0002fbf0: 7465 4a6f 6252 6573 706f 6e73 6542 6f64  teJobResponseBod
+0002fc00: 7928 290a 2020 2020 2020 2020 2020 2020  y().            
+0002fc10: 7365 6c66 2e62 6f64 7920 3d20 7465 6d70  self.body = temp
+0002fc20: 5f6d 6f64 656c 2e66 726f 6d5f 6d61 7028  _model.from_map(
+0002fc30: 6d5b 2762 6f64 7927 5d29 0a20 2020 2020  m['body']).     
+0002fc40: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
+0002fc50: 0a63 6c61 7373 2055 7064 6174 6554 656e  .class UpdateTen
+0002fc60: 736f 7262 6f61 7264 5265 7175 6573 7428  sorboardRequest(
+0002fc70: 5465 614d 6f64 656c 293a 0a20 2020 2064  TeaModel):.    d
+0002fc80: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+0002fc90: 2c20 6d61 785f 7275 6e6e 696e 675f 7469  , max_running_ti
+0002fca0: 6d65 5f6d 696e 7574 6573 3d4e 6f6e 652c  me_minutes=None,
+0002fcb0: 2077 6f72 6b73 7061 6365 5f69 643d 4e6f   workspace_id=No
+0002fcc0: 6e65 293a 0a20 2020 2020 2020 2073 656c  ne):.        sel
+0002fcd0: 662e 6d61 785f 7275 6e6e 696e 675f 7469  f.max_running_ti
+0002fce0: 6d65 5f6d 696e 7574 6573 203d 206d 6178  me_minutes = max
+0002fcf0: 5f72 756e 6e69 6e67 5f74 696d 655f 6d69  _running_time_mi
+0002fd00: 6e75 7465 7320 2023 2074 7970 653a 206c  nutes  # type: l
+0002fd10: 6f6e 670a 2020 2020 2020 2020 7365 6c66  ong.        self
+0002fd20: 2e77 6f72 6b73 7061 6365 5f69 6420 3d20  .workspace_id = 
+0002fd30: 776f 726b 7370 6163 655f 6964 2020 2320  workspace_id  # 
+0002fd40: 7479 7065 3a20 7374 720a 0a20 2020 2064  type: str..    d
+0002fd50: 6566 2076 616c 6964 6174 6528 7365 6c66  ef validate(self
+0002fd60: 293a 0a20 2020 2020 2020 2070 6173 730a  ):.        pass.
+0002fd70: 0a20 2020 2064 6566 2074 6f5f 6d61 7028  .    def to_map(
+0002fd80: 7365 6c66 293a 0a20 2020 2020 2020 205f  self):.        _
+0002fd90: 6d61 7020 3d20 7375 7065 7228 5570 6461  map = super(Upda
+0002fda0: 7465 5465 6e73 6f72 626f 6172 6452 6571  teTensorboardReq
+0002fdb0: 7565 7374 2c20 7365 6c66 292e 746f 5f6d  uest, self).to_m
+0002fdc0: 6170 2829 0a20 2020 2020 2020 2069 6620  ap().        if 
+0002fdd0: 5f6d 6170 2069 7320 6e6f 7420 4e6f 6e65  _map is not None
+0002fde0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0002fdf0: 7475 726e 205f 6d61 700a 0a20 2020 2020  turn _map..     
+0002fe00: 2020 2072 6573 756c 7420 3d20 6469 6374     result = dict
+0002fe10: 2829 0a20 2020 2020 2020 2069 6620 7365  ().        if se
+0002fe20: 6c66 2e6d 6178 5f72 756e 6e69 6e67 5f74  lf.max_running_t
+0002fe30: 696d 655f 6d69 6e75 7465 7320 6973 206e  ime_minutes is n
+0002fe40: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+0002fe50: 2020 2020 2072 6573 756c 745b 274d 6178       result['Max
+0002fe60: 5275 6e6e 696e 6754 696d 654d 696e 7574  RunningTimeMinut
+0002fe70: 6573 275d 203d 2073 656c 662e 6d61 785f  es'] = self.max_
+0002fe80: 7275 6e6e 696e 675f 7469 6d65 5f6d 696e  running_time_min
+0002fe90: 7574 6573 0a20 2020 2020 2020 2069 6620  utes.        if 
+0002fea0: 7365 6c66 2e77 6f72 6b73 7061 6365 5f69  self.workspace_i
+0002feb0: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
+0002fec0: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+0002fed0: 745b 2757 6f72 6b73 7061 6365 4964 275d  t['WorkspaceId']
+0002fee0: 203d 2073 656c 662e 776f 726b 7370 6163   = self.workspac
+0002fef0: 655f 6964 0a20 2020 2020 2020 2072 6574  e_id.        ret
+0002ff00: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
+0002ff10: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
+0002ff20: 662c 206d 3d4e 6f6e 6529 3a0a 2020 2020  f, m=None):.    
+0002ff30: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
+0002ff40: 7428 290a 2020 2020 2020 2020 6966 206d  t().        if m
+0002ff50: 2e67 6574 2827 4d61 7852 756e 6e69 6e67  .get('MaxRunning
+0002ff60: 5469 6d65 4d69 6e75 7465 7327 2920 6973  TimeMinutes') is
+0002ff70: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0002ff80: 2020 2020 2020 2073 656c 662e 6d61 785f         self.max_
+0002ff90: 7275 6e6e 696e 675f 7469 6d65 5f6d 696e  running_time_min
+0002ffa0: 7574 6573 203d 206d 2e67 6574 2827 4d61  utes = m.get('Ma
+0002ffb0: 7852 756e 6e69 6e67 5469 6d65 4d69 6e75  xRunningTimeMinu
+0002ffc0: 7465 7327 290a 2020 2020 2020 2020 6966  tes').        if
+0002ffd0: 206d 2e67 6574 2827 576f 726b 7370 6163   m.get('Workspac
+0002ffe0: 6549 6427 2920 6973 206e 6f74 204e 6f6e  eId') is not Non
+0002fff0: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00030000: 656c 662e 776f 726b 7370 6163 655f 6964  elf.workspace_id
+00030010: 203d 206d 2e67 6574 2827 576f 726b 7370   = m.get('Worksp
+00030020: 6163 6549 6427 290a 2020 2020 2020 2020  aceId').        
+00030030: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
+00030040: 6173 7320 5570 6461 7465 5465 6e73 6f72  ass UpdateTensor
+00030050: 626f 6172 6452 6573 706f 6e73 6542 6f64  boardResponseBod
+00030060: 7928 5465 614d 6f64 656c 293a 0a20 2020  y(TeaModel):.   
+00030070: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
+00030080: 6c66 2c20 7265 7175 6573 745f 6964 3d4e  lf, request_id=N
+00030090: 6f6e 652c 2074 656e 736f 7262 6f61 7264  one, tensorboard
+000300a0: 5f69 643d 4e6f 6e65 293a 0a20 2020 2020  _id=None):.     
+000300b0: 2020 2073 656c 662e 7265 7175 6573 745f     self.request_
+000300c0: 6964 203d 2072 6571 7565 7374 5f69 6420  id = request_id 
+000300d0: 2023 2074 7970 653a 2073 7472 0a20 2020   # type: str.   
+000300e0: 2020 2020 2073 656c 662e 7465 6e73 6f72       self.tensor
+000300f0: 626f 6172 645f 6964 203d 2074 656e 736f  board_id = tenso
+00030100: 7262 6f61 7264 5f69 6420 2023 2074 7970  rboard_id  # typ
+00030110: 653a 2073 7472 0a0a 2020 2020 6465 6620  e: str..    def 
+00030120: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
+00030130: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
+00030140: 2020 6465 6620 746f 5f6d 6170 2873 656c    def to_map(sel
+00030150: 6629 3a0a 2020 2020 2020 2020 5f6d 6170  f):.        _map
+00030160: 203d 2073 7570 6572 2855 7064 6174 6554   = super(UpdateT
+00030170: 656e 736f 7262 6f61 7264 5265 7370 6f6e  ensorboardRespon
+00030180: 7365 426f 6479 2c20 7365 6c66 292e 746f  seBody, self).to
+00030190: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
+000301a0: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
+000301b0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000301c0: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
+000301d0: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
+000301e0: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+000301f0: 7365 6c66 2e72 6571 7565 7374 5f69 6420  self.request_id 
+00030200: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00030210: 2020 2020 2020 2020 2072 6573 756c 745b           result[
+00030220: 2752 6571 7565 7374 4964 275d 203d 2073  'RequestId'] = s
+00030230: 656c 662e 7265 7175 6573 745f 6964 0a20  elf.request_id. 
+00030240: 2020 2020 2020 2069 6620 7365 6c66 2e74         if self.t
+00030250: 656e 736f 7262 6f61 7264 5f69 6420 6973  ensorboard_id is
+00030260: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00030270: 2020 2020 2020 2072 6573 756c 745b 2754         result['T
+00030280: 656e 736f 7262 6f61 7264 4964 275d 203d  ensorboardId'] =
+00030290: 2073 656c 662e 7465 6e73 6f72 626f 6172   self.tensorboar
+000302a0: 645f 6964 0a20 2020 2020 2020 2072 6574  d_id.        ret
+000302b0: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
+000302c0: 6465 6620 6672 6f6d 5f6d 6170 2873 656c  def from_map(sel
+000302d0: 662c 206d 3d4e 6f6e 6529 3a0a 2020 2020  f, m=None):.    
+000302e0: 2020 2020 6d20 3d20 6d20 6f72 2064 6963      m = m or dic
+000302f0: 7428 290a 2020 2020 2020 2020 6966 206d  t().        if m
+00030300: 2e67 6574 2827 5265 7175 6573 7449 6427  .get('RequestId'
+00030310: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+00030320: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00030330: 7265 7175 6573 745f 6964 203d 206d 2e67  request_id = m.g
+00030340: 6574 2827 5265 7175 6573 7449 6427 290a  et('RequestId').
+00030350: 2020 2020 2020 2020 6966 206d 2e67 6574          if m.get
+00030360: 2827 5465 6e73 6f72 626f 6172 6449 6427  ('TensorboardId'
+00030370: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+00030380: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00030390: 7465 6e73 6f72 626f 6172 645f 6964 203d  tensorboard_id =
+000303a0: 206d 2e67 6574 2827 5465 6e73 6f72 626f   m.get('Tensorbo
+000303b0: 6172 6449 6427 290a 2020 2020 2020 2020  ardId').        
+000303c0: 7265 7475 726e 2073 656c 660a 0a0a 636c  return self...cl
+000303d0: 6173 7320 5570 6461 7465 5465 6e73 6f72  ass UpdateTensor
+000303e0: 626f 6172 6452 6573 706f 6e73 6528 5465  boardResponse(Te
+000303f0: 614d 6f64 656c 293a 0a20 2020 2064 6566  aModel):.    def
+00030400: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
+00030410: 6865 6164 6572 733d 4e6f 6e65 2c20 7374  headers=None, st
+00030420: 6174 7573 5f63 6f64 653d 4e6f 6e65 2c20  atus_code=None, 
+00030430: 626f 6479 3d4e 6f6e 6529 3a0a 2020 2020  body=None):.    
+00030440: 2020 2020 7365 6c66 2e68 6561 6465 7273      self.headers
+00030450: 203d 2068 6561 6465 7273 2020 2320 7479   = headers  # ty
+00030460: 7065 3a20 6469 6374 5b73 7472 2c20 7374  pe: dict[str, st
+00030470: 725d 0a20 2020 2020 2020 2073 656c 662e  r].        self.
+00030480: 7374 6174 7573 5f63 6f64 6520 3d20 7374  status_code = st
+00030490: 6174 7573 5f63 6f64 6520 2023 2074 7970  atus_code  # typ
+000304a0: 653a 2069 6e74 0a20 2020 2020 2020 2073  e: int.        s
+000304b0: 656c 662e 626f 6479 203d 2062 6f64 7920  elf.body = body 
+000304c0: 2023 2074 7970 653a 2055 7064 6174 6554   # type: UpdateT
+000304d0: 656e 736f 7262 6f61 7264 5265 7370 6f6e  ensorboardRespon
+000304e0: 7365 426f 6479 0a0a 2020 2020 6465 6620  seBody..    def 
+000304f0: 7661 6c69 6461 7465 2873 656c 6629 3a0a  validate(self):.
+00030500: 2020 2020 2020 2020 7365 6c66 2e76 616c          self.val
+00030510: 6964 6174 655f 7265 7175 6972 6564 2873  idate_required(s
+00030520: 656c 662e 6865 6164 6572 732c 2027 6865  elf.headers, 'he
+00030530: 6164 6572 7327 290a 2020 2020 2020 2020  aders').        
+00030540: 7365 6c66 2e76 616c 6964 6174 655f 7265  self.validate_re
+00030550: 7175 6972 6564 2873 656c 662e 7374 6174  quired(self.stat
+00030560: 7573 5f63 6f64 652c 2027 7374 6174 7573  us_code, 'status
+00030570: 5f63 6f64 6527 290a 2020 2020 2020 2020  _code').        
+00030580: 7365 6c66 2e76 616c 6964 6174 655f 7265  self.validate_re
+00030590: 7175 6972 6564 2873 656c 662e 626f 6479  quired(self.body
+000305a0: 2c20 2762 6f64 7927 290a 2020 2020 2020  , 'body').      
+000305b0: 2020 6966 2073 656c 662e 626f 6479 3a0a    if self.body:.
+000305c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000305d0: 2e62 6f64 792e 7661 6c69 6461 7465 2829  .body.validate()
+000305e0: 0a0a 2020 2020 6465 6620 746f 5f6d 6170  ..    def to_map
+000305f0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00030600: 5f6d 6170 203d 2073 7570 6572 2855 7064  _map = super(Upd
+00030610: 6174 6554 656e 736f 7262 6f61 7264 5265  ateTensorboardRe
+00030620: 7370 6f6e 7365 2c20 7365 6c66 292e 746f  sponse, self).to
+00030630: 5f6d 6170 2829 0a20 2020 2020 2020 2069  _map().        i
+00030640: 6620 5f6d 6170 2069 7320 6e6f 7420 4e6f  f _map is not No
+00030650: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00030660: 7265 7475 726e 205f 6d61 700a 0a20 2020  return _map..   
+00030670: 2020 2020 2072 6573 756c 7420 3d20 6469       result = di
+00030680: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+00030690: 7365 6c66 2e68 6561 6465 7273 2069 7320  self.headers is 
+000306a0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000306b0: 2020 2020 2020 7265 7375 6c74 5b27 6865        result['he
+000306c0: 6164 6572 7327 5d20 3d20 7365 6c66 2e68  aders'] = self.h
+000306d0: 6561 6465 7273 0a20 2020 2020 2020 2069  eaders.        i
+000306e0: 6620 7365 6c66 2e73 7461 7475 735f 636f  f self.status_co
+000306f0: 6465 2069 7320 6e6f 7420 4e6f 6e65 3a0a  de is not None:.
+00030700: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00030710: 6c74 5b27 7374 6174 7573 436f 6465 275d  lt['statusCode']
+00030720: 203d 2073 656c 662e 7374 6174 7573 5f63   = self.status_c
+00030730: 6f64 650a 2020 2020 2020 2020 6966 2073  ode.        if s
+00030740: 656c 662e 626f 6479 2069 7320 6e6f 7420  elf.body is not 
+00030750: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00030760: 2020 7265 7375 6c74 5b27 626f 6479 275d    result['body']
+00030770: 203d 2073 656c 662e 626f 6479 2e74 6f5f   = self.body.to_
+00030780: 6d61 7028 290a 2020 2020 2020 2020 7265  map().        re
+00030790: 7475 726e 2072 6573 756c 740a 0a20 2020  turn result..   
+000307a0: 2064 6566 2066 726f 6d5f 6d61 7028 7365   def from_map(se
+000307b0: 6c66 2c20 6d3d 4e6f 6e65 293a 0a20 2020  lf, m=None):.   
+000307c0: 2020 2020 206d 203d 206d 206f 7220 6469       m = m or di
+000307d0: 6374 2829 0a20 2020 2020 2020 2069 6620  ct().        if 
+000307e0: 6d2e 6765 7428 2768 6561 6465 7273 2729  m.get('headers')
+000307f0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00030800: 2020 2020 2020 2020 2020 7365 6c66 2e68            self.h
+00030810: 6561 6465 7273 203d 206d 2e67 6574 2827  eaders = m.get('
+00030820: 6865 6164 6572 7327 290a 2020 2020 2020  headers').      
+00030830: 2020 6966 206d 2e67 6574 2827 7374 6174    if m.get('stat
+00030840: 7573 436f 6465 2729 2069 7320 6e6f 7420  usCode') is not 
+00030850: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00030860: 2020 7365 6c66 2e73 7461 7475 735f 636f    self.status_co
+00030870: 6465 203d 206d 2e67 6574 2827 7374 6174  de = m.get('stat
+00030880: 7573 436f 6465 2729 0a20 2020 2020 2020  usCode').       
+00030890: 2069 6620 6d2e 6765 7428 2762 6f64 7927   if m.get('body'
+000308a0: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
+000308b0: 2020 2020 2020 2020 2020 2074 656d 705f             temp_
+000308c0: 6d6f 6465 6c20 3d20 5570 6461 7465 5465  model = UpdateTe
+000308d0: 6e73 6f72 626f 6172 6452 6573 706f 6e73  nsorboardRespons
+000308e0: 6542 6f64 7928 290a 2020 2020 2020 2020  eBody().        
+000308f0: 2020 2020 7365 6c66 2e62 6f64 7920 3d20      self.body = 
+00030900: 7465 6d70 5f6d 6f64 656c 2e66 726f 6d5f  temp_model.from_
+00030910: 6d61 7028 6d5b 2762 6f64 7927 5d29 0a20  map(m['body']). 
+00030920: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00030930: 6c66 0a0a 0a                             lf...
```

### Comparing `alibabacloud_pai-dlc20201203_py2-1.2.5/alibabacloud_pai_dlc20201203_py2.egg-info/PKG-INFO` & `alibabacloud_pai-dlc20201203_py2-1.2.6/alibabacloud_pai_dlc20201203_py2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-pai-dlc20201203-py2
-Version: 1.2.5
+Version: 1.2.6
 Summary: Alibaba Cloud pai-dlc (20201203) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_pai-dlc20201203_py2-1.2.5/setup.py` & `alibabacloud_pai-dlc20201203_py2-1.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,28 +21,28 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_pai-dlc20201203_py2.
 
-Created on 26/05/2023
+Created on 19/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_pai_dlc20201203"
 NAME = "alibabacloud_pai-dlc20201203_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud pai-dlc (20201203) SDK Library for Python2"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python2-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util_py2>=0.0.7, <1.0.0",
+    "alibabacloud_tea_util_py2>=0.0.8, <1.0.0",
     "alibabacloud_tea_openapi_py2>=0.1.6, <1.0.0",
     "alibabacloud_openapi_util_py2>=0.1.1, <1.0.0",
     "alibabacloud_endpoint_util_py2>=0.0.2, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
```

