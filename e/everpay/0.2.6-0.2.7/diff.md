# Comparing `tmp/everpay-0.2.6.tar.gz` & `tmp/everpay-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "everpay-0.2.6.tar", last modified: Sat Dec  3 05:35:26 2022, max compression
+gzip compressed data, was "everpay-0.2.7.tar", last modified: Wed Jul 19 05:27:30 2023, max compression
```

## Comparing `everpay-0.2.6.tar` & `everpay-0.2.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-12-03 05:35:26.551346 everpay-0.2.6/
--rw-r--r--   0 jay        (501) staff       (20)     1068 2022-11-04 02:53:12.000000 everpay-0.2.6/LICENSE
--rw-r--r--   0 jay        (501) staff       (20)     1537 2022-12-03 05:35:26.551200 everpay-0.2.6/PKG-INFO
--rw-r--r--   0 jay        (501) staff       (20)      963 2022-11-04 02:53:12.000000 everpay-0.2.6/README.md
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-12-03 05:35:26.550418 everpay-0.2.6/everpay/
--rw-r--r--   0 jay        (501) staff       (20)      117 2022-11-04 02:53:12.000000 everpay-0.2.6/everpay/__init__.py
--rw-r--r--   0 jay        (501) staff       (20)     1852 2022-11-28 03:53:03.000000 everpay-0.2.6/everpay/account.py
--rw-r--r--   0 jay        (501) staff       (20)     5430 2022-11-14 15:47:58.000000 everpay-0.2.6/everpay/bundle.py
--rw-r--r--   0 jay        (501) staff       (20)     2839 2022-12-03 05:32:54.000000 everpay-0.2.6/everpay/client.py
--rw-r--r--   0 jay        (501) staff       (20)     1444 2022-11-14 15:24:46.000000 everpay-0.2.6/everpay/signer.py
--rw-r--r--   0 jay        (501) staff       (20)      969 2022-11-28 04:12:35.000000 everpay-0.2.6/everpay/token.py
--rw-r--r--   0 jay        (501) staff       (20)     2480 2022-11-04 02:53:12.000000 everpay-0.2.6/everpay/transaction.py
--rw-r--r--   0 jay        (501) staff       (20)     1567 2022-11-28 04:20:43.000000 everpay-0.2.6/everpay/utils.py
-drwxr-xr-x   0 jay        (501) staff       (20)        0 2022-12-03 05:35:26.551079 everpay-0.2.6/everpay.egg-info/
--rw-r--r--   0 jay        (501) staff       (20)     1537 2022-12-03 05:35:26.000000 everpay-0.2.6/everpay.egg-info/PKG-INFO
--rw-r--r--   0 jay        (501) staff       (20)      330 2022-12-03 05:35:26.000000 everpay-0.2.6/everpay.egg-info/SOURCES.txt
--rw-r--r--   0 jay        (501) staff       (20)        1 2022-12-03 05:35:26.000000 everpay-0.2.6/everpay.egg-info/dependency_links.txt
--rw-r--r--   0 jay        (501) staff       (20)       60 2022-12-03 05:35:26.000000 everpay-0.2.6/everpay.egg-info/requires.txt
--rw-r--r--   0 jay        (501) staff       (20)        8 2022-12-03 05:35:26.000000 everpay-0.2.6/everpay.egg-info/top_level.txt
--rw-r--r--   0 jay        (501) staff       (20)       38 2022-12-03 05:35:26.551379 everpay-0.2.6/setup.cfg
--rw-r--r--   0 jay        (501) staff       (20)      808 2022-12-03 05:34:00.000000 everpay-0.2.6/setup.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-07-19 05:27:30.848069 everpay-0.2.7/
+-rw-r--r--   0 jay        (501) staff       (20)     1068 2023-07-19 05:19:32.000000 everpay-0.2.7/LICENSE
+-rw-r--r--   0 jay        (501) staff       (20)     2272 2023-07-19 05:27:30.847959 everpay-0.2.7/PKG-INFO
+-rw-r--r--   0 jay        (501) staff       (20)     1718 2023-07-19 05:21:40.000000 everpay-0.2.7/README.md
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-07-19 05:27:30.847203 everpay-0.2.7/everpay/
+-rw-r--r--   0 jay        (501) staff       (20)      117 2023-07-19 05:19:32.000000 everpay-0.2.7/everpay/__init__.py
+-rw-r--r--   0 jay        (501) staff       (20)     1852 2023-07-19 05:19:32.000000 everpay-0.2.7/everpay/account.py
+-rw-r--r--   0 jay        (501) staff       (20)     5430 2023-07-19 05:19:32.000000 everpay-0.2.7/everpay/bundle.py
+-rw-r--r--   0 jay        (501) staff       (20)     2839 2023-07-19 05:19:32.000000 everpay-0.2.7/everpay/client.py
+-rw-r--r--   0 jay        (501) staff       (20)     1444 2023-07-19 05:19:32.000000 everpay-0.2.7/everpay/signer.py
+-rw-r--r--   0 jay        (501) staff       (20)      969 2023-07-19 05:19:32.000000 everpay-0.2.7/everpay/token.py
+-rw-r--r--   0 jay        (501) staff       (20)     2482 2023-07-19 05:20:15.000000 everpay-0.2.7/everpay/transaction.py
+-rw-r--r--   0 jay        (501) staff       (20)     1567 2023-07-19 05:19:32.000000 everpay-0.2.7/everpay/utils.py
+drwxr-xr-x   0 jay        (501) staff       (20)        0 2023-07-19 05:27:30.847818 everpay-0.2.7/everpay.egg-info/
+-rw-r--r--   0 jay        (501) staff       (20)     2272 2023-07-19 05:27:30.000000 everpay-0.2.7/everpay.egg-info/PKG-INFO
+-rw-r--r--   0 jay        (501) staff       (20)      330 2023-07-19 05:27:30.000000 everpay-0.2.7/everpay.egg-info/SOURCES.txt
+-rw-r--r--   0 jay        (501) staff       (20)        1 2023-07-19 05:27:30.000000 everpay-0.2.7/everpay.egg-info/dependency_links.txt
+-rw-r--r--   0 jay        (501) staff       (20)       60 2023-07-19 05:27:30.000000 everpay-0.2.7/everpay.egg-info/requires.txt
+-rw-r--r--   0 jay        (501) staff       (20)        8 2023-07-19 05:27:30.000000 everpay-0.2.7/everpay.egg-info/top_level.txt
+-rw-r--r--   0 jay        (501) staff       (20)       38 2023-07-19 05:27:30.848110 everpay-0.2.7/setup.cfg
+-rw-r--r--   0 jay        (501) staff       (20)      808 2023-07-19 05:25:49.000000 everpay-0.2.7/setup.py
```

### Comparing `everpay-0.2.6/LICENSE` & `everpay-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `everpay-0.2.6/PKG-INFO` & `everpay-0.2.7/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: everpay
-Version: 0.2.6
+Version: 0.2.7
 Summary: Python wrappers for everpay.io api
 Home-page: https://github.com/everFinance/everpay.py
+Download-URL: https://github.com/everFinance/everpay.py/archive/refs/tags/v0.2.7.tar.gz
 Author: xiaojay
 Author-email: xiaojay@gmail.com
 License: MIT
-Download-URL: https://github.com/everFinance/everpay.py/archive/refs/tags/v0.2.6.tar.gz
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 2
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -62,11 +61,31 @@
 
 ```
 
 - bundle
 
 see example/bundle_tx.py
 
-## todo
-- [] deposit/withdraw
+- token symbol or tag
+
+sometimes two token may have same token symbol in everpay. for example, usdc bridged from ethereum and usdc bridged from bsc have the same token symbol "usdc". 
+
+In this case, you should use token tag, which is always unique in everpay, to call api function.
+
+```python
+
+import everpay
+api_server = 'https://api-dev.everpay.io'
+c = everpay.Client(api_server)
+
+# get token tag list
+print(c.get_token_list())
 
+# get balance of usdc bridged from bsc
+c.get_balance('0x61EbF673c200646236B2c53465bcA0699455d5FA', 'bsc-usdc-0x64544969ed7ebf5f083679233325356ebe738930')
+# get balance of usdc bridged from ethereum
+c.get_balance('0x61EbF673c200646236B2c53465bcA0699455d5FA', 'ethereum-usdc-0xf044320bcc3cd1f6100cd197754c71941469e79c')
 
+```
+
+## todo
+- [] deposit/withdraw
```

### Comparing `everpay-0.2.6/everpay/account.py` & `everpay-0.2.7/everpay/account.py`

 * *Files identical despite different names*

### Comparing `everpay-0.2.6/everpay/bundle.py` & `everpay-0.2.7/everpay/bundle.py`

 * *Files identical despite different names*

### Comparing `everpay-0.2.6/everpay/client.py` & `everpay-0.2.7/everpay/client.py`

 * *Files identical despite different names*

### Comparing `everpay-0.2.6/everpay/signer.py` & `everpay-0.2.7/everpay/signer.py`

 * *Files identical despite different names*

### Comparing `everpay-0.2.6/everpay/token.py` & `everpay-0.2.7/everpay/token.py`

 * *Files identical despite different names*

### Comparing `everpay-0.2.6/everpay/transaction.py` & `everpay-0.2.7/everpay/transaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
                 'chainID:' + self.chain_id + '\n' + \
                 'data:' + self.data + '\n' + \
                 'version:' + self.version 
 
     def get_ever_hash(self):
         message = encode_defunct(text=str(self))
         message_hash = _hash_eip191_message(message)
-        return w3.toHex(message_hash)
+        return w3.to_hex(message_hash)
 
     def to_dict(self):
         return {
             'tx_id': self.tx_id,
             'tokenSymbol': self.token_symbol,
             'action': self.action,
             'from': self.from_,
@@ -62,8 +62,8 @@
         }
 
     def post(self, api_host):
         url = api_host + '/tx'
         if not self.sig:
             raise Exception(self.tx_id, 'no signature.')
         #print('post_data:', self.to_dict())
-        return requests.post(url, json=self.to_dict())
+        return requests.post(url, json=self.to_dict())
```

### Comparing `everpay-0.2.6/everpay/utils.py` & `everpay-0.2.7/everpay/utils.py`

 * *Files identical despite different names*

### Comparing `everpay-0.2.6/everpay.egg-info/PKG-INFO` & `everpay-0.2.7/everpay.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: everpay
-Version: 0.2.6
+Version: 0.2.7
 Summary: Python wrappers for everpay.io api
 Home-page: https://github.com/everFinance/everpay.py
+Download-URL: https://github.com/everFinance/everpay.py/archive/refs/tags/v0.2.7.tar.gz
 Author: xiaojay
 Author-email: xiaojay@gmail.com
 License: MIT
-Download-URL: https://github.com/everFinance/everpay.py/archive/refs/tags/v0.2.6.tar.gz
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 2
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -62,11 +61,31 @@
 
 ```
 
 - bundle
 
 see example/bundle_tx.py
 
-## todo
-- [] deposit/withdraw
+- token symbol or tag
+
+sometimes two token may have same token symbol in everpay. for example, usdc bridged from ethereum and usdc bridged from bsc have the same token symbol "usdc". 
+
+In this case, you should use token tag, which is always unique in everpay, to call api function.
+
+```python
+
+import everpay
+api_server = 'https://api-dev.everpay.io'
+c = everpay.Client(api_server)
+
+# get token tag list
+print(c.get_token_list())
 
+# get balance of usdc bridged from bsc
+c.get_balance('0x61EbF673c200646236B2c53465bcA0699455d5FA', 'bsc-usdc-0x64544969ed7ebf5f083679233325356ebe738930')
+# get balance of usdc bridged from ethereum
+c.get_balance('0x61EbF673c200646236B2c53465bcA0699455d5FA', 'ethereum-usdc-0xf044320bcc3cd1f6100cd197754c71941469e79c')
 
+```
+
+## todo
+- [] deposit/withdraw
```

### Comparing `everpay-0.2.6/setup.py` & `everpay-0.2.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 
 setuptools.setup(
     name='everpay',
-    version='0.2.6',
+    version='0.2.7',
     packages=['everpay',],
     license='MIT',
     description = 'Python wrappers for everpay.io api',
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     author = 'xiaojay',
     author_email = 'xiaojay@gmail.com',
     install_requires=['requests', 'web3', 'python-jose', 'arweave-python-client', 'eth_account'],
     url = 'https://github.com/everFinance/everpay.py',
-    download_url = 'https://github.com/everFinance/everpay.py/archive/refs/tags/v0.2.6.tar.gz',
+    download_url = 'https://github.com/everFinance/everpay.py/archive/refs/tags/v0.2.7.tar.gz',
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 2",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
```

