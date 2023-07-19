# Comparing `tmp/neo-fairy-client-3.5.0.7.tar.gz` & `tmp/neo-fairy-client-3.5.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neo-fairy-client-3.5.0.7.tar", last modified: Tue Jul 18 08:39:36 2023, max compression
+gzip compressed data, was "neo-fairy-client-3.5.0.8.tar", last modified: Wed Jul 19 10:06:41 2023, max compression
```

## Comparing `neo-fairy-client-3.5.0.7.tar` & `neo-fairy-client-3.5.0.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 08:39:36.832974 neo-fairy-client-3.5.0.7/
--rw-rw-rw-   0        0        0     1085 2022-05-05 03:19:19.000000 neo-fairy-client-3.5.0.7/LICENSE
--rw-rw-rw-   0        0        0   139301 2023-07-18 08:39:36.832974 neo-fairy-client-3.5.0.7/PKG-INFO
--rw-rw-rw-   0        0        0   138843 2023-06-14 05:42:43.000000 neo-fairy-client-3.5.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-18 08:39:36.789777 neo-fairy-client-3.5.0.7/neo_fairy_client/
--rw-rw-rw-   0        0        0      109 2022-09-22 08:08:31.000000 neo-fairy-client-3.5.0.7/neo_fairy_client/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 08:39:36.805259 neo-fairy-client-3.5.0.7/neo_fairy_client/rpc/
--rw-rw-rw-   0        0        0       74 2022-09-21 02:51:06.000000 neo-fairy-client-3.5.0.7/neo_fairy_client/rpc/__init__.py
--rw-rw-rw-   0        0        0    55864 2023-07-18 08:27:33.000000 neo-fairy-client-3.5.0.7/neo_fairy_client/rpc/fairy_client.py
-drwxrwxrwx   0        0        0        0 2023-07-18 08:39:36.819873 neo-fairy-client-3.5.0.7/neo_fairy_client/utils/
--rw-rw-rw-   0        0        0     1379 2022-09-21 06:25:56.000000 neo-fairy-client-3.5.0.7/neo_fairy_client/utils/WitnessRule.py
--rw-rw-rw-   0        0        0      293 2023-04-26 05:30:10.000000 neo-fairy-client-3.5.0.7/neo_fairy_client/utils/__init__.py
--rw-rw-rw-   0        0        0     1588 2022-10-25 06:12:11.000000 neo-fairy-client-3.5.0.7/neo_fairy_client/utils/interpreters.py
--rw-rw-rw-   0        0        0      195 2022-09-28 04:32:29.000000 neo-fairy-client-3.5.0.7/neo_fairy_client/utils/misc.py
--rw-rw-rw-   0        0        0     1319 2022-10-25 06:12:11.000000 neo-fairy-client-3.5.0.7/neo_fairy_client/utils/timers.py
--rw-rw-rw-   0        0        0     5625 2022-10-10 02:34:50.000000 neo-fairy-client-3.5.0.7/neo_fairy_client/utils/types.py
-drwxrwxrwx   0        0        0        0 2023-07-18 08:39:36.823922 neo-fairy-client-3.5.0.7/neo_fairy_client/vm/
--rw-rw-rw-   0        0        0       58 2022-09-21 02:49:39.000000 neo-fairy-client-3.5.0.7/neo_fairy_client/vm/__init__.py
--rw-rw-rw-   0        0        0    15030 2022-09-22 08:50:45.000000 neo-fairy-client-3.5.0.7/neo_fairy_client/vm/fairy_engine.py
-drwxrwxrwx   0        0        0        0 2023-07-18 08:39:36.829815 neo-fairy-client-3.5.0.7/neo_fairy_client/websocket/
--rw-rw-rw-   0        0        0        0 2023-01-04 02:00:53.000000 neo-fairy-client-3.5.0.7/neo_fairy_client/websocket/__init__.py
--rw-rw-rw-   0        0        0     4694 2023-03-06 02:47:25.000000 neo-fairy-client-3.5.0.7/neo_fairy_client/websocket/fairy_websocket.py
-drwxrwxrwx   0        0        0        0 2023-07-18 08:39:36.802220 neo-fairy-client-3.5.0.7/neo_fairy_client.egg-info/
--rw-rw-rw-   0        0        0   139301 2023-07-18 08:39:36.000000 neo-fairy-client-3.5.0.7/neo_fairy_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      685 2023-07-18 08:39:36.000000 neo-fairy-client-3.5.0.7/neo_fairy_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 08:39:36.000000 neo-fairy-client-3.5.0.7/neo_fairy_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-07-18 08:39:36.000000 neo-fairy-client-3.5.0.7/neo_fairy_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-18 08:39:36.000000 neo-fairy-client-3.5.0.7/neo_fairy_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-18 08:39:36.833852 neo-fairy-client-3.5.0.7/setup.cfg
--rw-rw-rw-   0        0        0      762 2023-07-18 08:38:53.000000 neo-fairy-client-3.5.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 10:06:41.107616 neo-fairy-client-3.5.0.8/
+-rw-rw-rw-   0        0        0     1085 2022-05-05 03:19:19.000000 neo-fairy-client-3.5.0.8/LICENSE
+-rw-rw-rw-   0        0        0   139301 2023-07-19 10:06:41.107616 neo-fairy-client-3.5.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0   138843 2023-06-14 05:42:43.000000 neo-fairy-client-3.5.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-19 10:06:41.075965 neo-fairy-client-3.5.0.8/neo_fairy_client/
+-rw-rw-rw-   0        0        0      109 2022-09-22 08:08:31.000000 neo-fairy-client-3.5.0.8/neo_fairy_client/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 10:06:41.088590 neo-fairy-client-3.5.0.8/neo_fairy_client/rpc/
+-rw-rw-rw-   0        0        0       74 2022-09-21 02:51:06.000000 neo-fairy-client-3.5.0.8/neo_fairy_client/rpc/__init__.py
+-rw-rw-rw-   0        0        0    55900 2023-07-19 08:33:35.000000 neo-fairy-client-3.5.0.8/neo_fairy_client/rpc/fairy_client.py
+drwxrwxrwx   0        0        0        0 2023-07-19 10:06:41.099521 neo-fairy-client-3.5.0.8/neo_fairy_client/utils/
+-rw-rw-rw-   0        0        0     1379 2022-09-21 06:25:56.000000 neo-fairy-client-3.5.0.8/neo_fairy_client/utils/WitnessRule.py
+-rw-rw-rw-   0        0        0      293 2023-04-26 05:30:10.000000 neo-fairy-client-3.5.0.8/neo_fairy_client/utils/__init__.py
+-rw-rw-rw-   0        0        0     1588 2022-10-25 06:12:11.000000 neo-fairy-client-3.5.0.8/neo_fairy_client/utils/interpreters.py
+-rw-rw-rw-   0        0        0      195 2022-09-28 04:32:29.000000 neo-fairy-client-3.5.0.8/neo_fairy_client/utils/misc.py
+-rw-rw-rw-   0        0        0     1319 2022-10-25 06:12:11.000000 neo-fairy-client-3.5.0.8/neo_fairy_client/utils/timers.py
+-rw-rw-rw-   0        0        0     5625 2022-10-10 02:34:50.000000 neo-fairy-client-3.5.0.8/neo_fairy_client/utils/types.py
+drwxrwxrwx   0        0        0        0 2023-07-19 10:06:41.102563 neo-fairy-client-3.5.0.8/neo_fairy_client/vm/
+-rw-rw-rw-   0        0        0       58 2022-09-21 02:49:39.000000 neo-fairy-client-3.5.0.8/neo_fairy_client/vm/__init__.py
+-rw-rw-rw-   0        0        0    15030 2022-09-22 08:50:45.000000 neo-fairy-client-3.5.0.8/neo_fairy_client/vm/fairy_engine.py
+drwxrwxrwx   0        0        0        0 2023-07-19 10:06:41.105567 neo-fairy-client-3.5.0.8/neo_fairy_client/websocket/
+-rw-rw-rw-   0        0        0        0 2023-01-04 02:00:53.000000 neo-fairy-client-3.5.0.8/neo_fairy_client/websocket/__init__.py
+-rw-rw-rw-   0        0        0     4694 2023-03-06 02:47:25.000000 neo-fairy-client-3.5.0.8/neo_fairy_client/websocket/fairy_websocket.py
+drwxrwxrwx   0        0        0        0 2023-07-19 10:06:41.085550 neo-fairy-client-3.5.0.8/neo_fairy_client.egg-info/
+-rw-rw-rw-   0        0        0   139301 2023-07-19 10:06:41.000000 neo-fairy-client-3.5.0.8/neo_fairy_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      685 2023-07-19 10:06:41.000000 neo-fairy-client-3.5.0.8/neo_fairy_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 10:06:41.000000 neo-fairy-client-3.5.0.8/neo_fairy_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-07-19 10:06:41.000000 neo-fairy-client-3.5.0.8/neo_fairy_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-19 10:06:41.000000 neo-fairy-client-3.5.0.8/neo_fairy_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-19 10:06:41.108619 neo-fairy-client-3.5.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      762 2023-07-19 08:33:50.000000 neo-fairy-client-3.5.0.8/setup.py
```

### Comparing `neo-fairy-client-3.5.0.7/LICENSE` & `neo-fairy-client-3.5.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `neo-fairy-client-3.5.0.7/PKG-INFO` & `neo-fairy-client-3.5.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neo-fairy-client
-Version: 3.5.0.7
+Version: 3.5.0.8
 Summary: Test & debug your Neo3 smart contracts
 Home-page: https://github.com/Hecate2/neo-fairy-client
 Author: Hecate2
 Author-email: hecate2@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `neo-fairy-client-3.5.0.7/README.md` & `neo-fairy-client-3.5.0.8/README.md`

 * *Files identical despite different names*

### Comparing `neo-fairy-client-3.5.0.7/neo_fairy_client/rpc/fairy_client.py` & `neo-fairy-client-3.5.0.8/neo_fairy_client/rpc/fairy_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -589,21 +589,21 @@
         else:
             close_wallet_result = self.meta_rpc_method("resetdefaultfairywallet", [])
         if not close_wallet_result:
             raise ValueError(f'Failed to reset default wallet.')
         return close_wallet_result
 
     def set_session_fairy_wallet_with_NEP2(self, nep2: str, password: str, fairy_session: str = None) -> dict:
-        open_wallet_result = self.meta_rpc_method("setsessionfairywalletwithnep2", [nep2, password, fairy_session or self.fairy_session])
+        open_wallet_result = self.meta_rpc_method("setsessionfairywalletwithnep2", [fairy_session or self.fairy_session, nep2, password])
         if not open_wallet_result:
             raise ValueError(f'Failed to open NEP2 wallet {nep2} with given password.')
         return open_wallet_result
 
     def set_session_fairy_wallet_with_WIF(self, wif: str, password: str, fairy_session: str = None) -> dict:
-        open_wallet_result = self.meta_rpc_method("setsessionfairywalletwithwif", [wif, password, fairy_session or self.fairy_session])
+        open_wallet_result = self.meta_rpc_method("setsessionfairywalletwithwif", [fairy_session or self.fairy_session, wif, password])
         if not open_wallet_result:
             raise ValueError(f'Failed to open WIF wallet {wif} with given password.')
         return open_wallet_result
 
     def get_time_milliseconds(self) -> int:
         """
         :return: blockchain timestamp in milliseconds
@@ -872,15 +872,15 @@
         return self.meta_rpc_method("listdebugsnapshots", [])
 
     def get_method_by_instruction_pointer(self, instruction_pointer: int, scripthash: Hash160Str = None):
         scripthash = scripthash or self.contract_scripthash
         return self.meta_rpc_method("getmethodbyinstructionpointer", [scripthash, instruction_pointer])
 
     def debug_any_function_with_session(self, scripthash: Hash160Str, operation: str,
-                                       params: List[Union[str, int, dict, Hash160Str, UInt160]] = None,
+                                       params: List[Union[str, int, dict, Hash160Str, UInt160, bytes, bytearray]] = None,
                                        signers: Union[Signer, List[Signer]] = None, relay: bool = None, do_not_raise_on_result=False,
                                        with_print=True, fairy_session: str = None) -> RpcBreakpoint:
         scripthash = scripthash or self.contract_scripthash
         fairy_session = fairy_session or self.fairy_session
         if self.with_print and with_print:
             if fairy_session:
                 print(f'{fairy_session}::debugfunction {operation}')
@@ -901,15 +901,15 @@
         result = raw_result['result']
         return RpcBreakpoint(result['state'], result['breakreason'],
                              result['scripthash'], result['contractname'], result['instructionpointer'],
                              result['sourcefilename'], result['sourcelinenum'], result['sourcecontent'],
                              exception=result['exception'], result_stack=self.parse_stack_from_raw_result(raw_result))
 
     def debug_function_with_session(self, operation: str,
-                                        params: List[Union[str, int, dict, Hash160Str, UInt160]] = None,
+                                        params: List[Union[str, int, dict, Hash160Str, UInt160, bytes, bytearray]] = None,
                                         signers: List[Signer] = None, relay: bool = None, do_not_raise_on_result=False,
                                         with_print=True, fairy_session: str = None) -> RpcBreakpoint:
         return self.debug_any_function_with_session(
             self.contract_scripthash, operation,
             params=params, signers=signers, relay=relay, do_not_raise_on_result=do_not_raise_on_result,
             with_print=with_print, fairy_session=fairy_session)
```

### Comparing `neo-fairy-client-3.5.0.7/neo_fairy_client/utils/WitnessRule.py` & `neo-fairy-client-3.5.0.8/neo_fairy_client/utils/WitnessRule.py`

 * *Files identical despite different names*

### Comparing `neo-fairy-client-3.5.0.7/neo_fairy_client/utils/interpreters.py` & `neo-fairy-client-3.5.0.8/neo_fairy_client/utils/interpreters.py`

 * *Files identical despite different names*

### Comparing `neo-fairy-client-3.5.0.7/neo_fairy_client/utils/timers.py` & `neo-fairy-client-3.5.0.8/neo_fairy_client/utils/timers.py`

 * *Files identical despite different names*

### Comparing `neo-fairy-client-3.5.0.7/neo_fairy_client/utils/types.py` & `neo-fairy-client-3.5.0.8/neo_fairy_client/utils/types.py`

 * *Files identical despite different names*

### Comparing `neo-fairy-client-3.5.0.7/neo_fairy_client/vm/fairy_engine.py` & `neo-fairy-client-3.5.0.8/neo_fairy_client/vm/fairy_engine.py`

 * *Files identical despite different names*

### Comparing `neo-fairy-client-3.5.0.7/neo_fairy_client/websocket/fairy_websocket.py` & `neo-fairy-client-3.5.0.8/neo_fairy_client/websocket/fairy_websocket.py`

 * *Files identical despite different names*

### Comparing `neo-fairy-client-3.5.0.7/neo_fairy_client.egg-info/PKG-INFO` & `neo-fairy-client-3.5.0.8/neo_fairy_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neo-fairy-client
-Version: 3.5.0.7
+Version: 3.5.0.8
 Summary: Test & debug your Neo3 smart contracts
 Home-page: https://github.com/Hecate2/neo-fairy-client
 Author: Hecate2
 Author-email: hecate2@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `neo-fairy-client-3.5.0.7/neo_fairy_client.egg-info/SOURCES.txt` & `neo-fairy-client-3.5.0.8/neo_fairy_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neo-fairy-client-3.5.0.7/setup.py` & `neo-fairy-client-3.5.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="neo-fairy-client",
-    version="3.5.0.7",
+    version="3.5.0.8",
     author="Hecate2",
     author_email="hecate2@qq.com",
     description="Test & debug your Neo3 smart contracts",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Hecate2/neo-fairy-client",
     packages=setuptools.find_packages(),
```

