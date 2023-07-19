# Comparing `tmp/web3r-0.1.tar.gz` & `tmp/web3r-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web3r-0.1.tar", last modified: Tue Jul 18 23:22:35 2023, max compression
+gzip compressed data, was "web3r-0.2.tar", last modified: Wed Jul 19 11:24:59 2023, max compression
```

## Comparing `web3r-0.1.tar` & `web3r-0.2.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 23:22:35.111470 web3r-0.1/
--rw-rw-rw-   0        0        0      940 2023-07-18 23:22:35.111470 web3r-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2768 2023-07-18 22:33:12.000000 web3r-0.1/README.md
--rw-rw-rw-   0        0        0       86 2023-07-18 23:22:35.112470 web3r-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1284 2023-07-18 23:22:06.000000 web3r-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-18 23:22:35.105472 web3r-0.1/web3r/
--rw-rw-rw-   0        0        0     1708 2023-07-18 23:08:00.000000 web3r-0.1/web3r/Web3R.py
--rw-rw-rw-   0        0        0        0 2023-07-16 20:16:34.000000 web3r-0.1/web3r/__init__.py
--rw-rw-rw-   0        0        0     1248 2023-07-18 23:13:54.000000 web3r-0.1/web3r/uniswap_erc20_total.py
-drwxrwxrwx   0        0        0        0 2023-07-18 23:22:35.110471 web3r-0.1/web3r.egg-info/
--rw-rw-rw-   0        0        0      940 2023-07-18 23:22:35.000000 web3r-0.1/web3r.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-07-18 23:22:35.000000 web3r-0.1/web3r.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 23:22:35.000000 web3r-0.1/web3r.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-07-18 23:22:35.000000 web3r-0.1/web3r.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-18 23:22:35.000000 web3r-0.1/web3r.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-19 11:24:59.840850 web3r-0.2/
+-rw-rw-rw-   0        0        0      940 2023-07-19 11:24:59.841850 web3r-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2768 2023-07-18 22:33:12.000000 web3r-0.2/README.md
+-rw-rw-rw-   0        0        0       86 2023-07-19 11:24:59.841850 web3r-0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1284 2023-07-19 11:24:33.000000 web3r-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 11:24:59.832852 web3r-0.2/web3r/
+-rw-rw-rw-   0        0        0       30 2023-07-18 23:51:38.000000 web3r-0.2/web3r/__init__.py
+-rw-rw-rw-   0        0        0     1750 2023-07-19 11:14:27.000000 web3r-0.2/web3r/main.py
+drwxrwxrwx   0        0        0        0 2023-07-19 11:24:59.839851 web3r-0.2/web3r.egg-info/
+-rw-rw-rw-   0        0        0      940 2023-07-19 11:24:59.000000 web3r-0.2/web3r.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      204 2023-07-19 11:24:59.000000 web3r-0.2/web3r.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 11:24:59.000000 web3r-0.2/web3r.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-07-19 11:24:59.000000 web3r-0.2/web3r.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-19 11:24:59.000000 web3r-0.2/web3r.egg-info/top_level.txt
```

### Comparing `web3r-0.1/PKG-INFO` & `web3r-0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: web3r
-Version: 0.1
+Version: 0.2
 Summary: Web3R.py is a Python wrapper that enhances the functionality of Web3.py and integrates with Etherscan's API.
 Home-page: https://github.com/FinnCastro/Web3R.py
 Author: Finn Castro
 Author-email: your.email@domain.com
 License: MIT
-Download-URL: https://github.com/FinnCastro/Web3R.py/archive/refs/tags/0.01.tar.gz
+Download-URL: https://github.com/FinnCastro/Web3R.py/archive/refs/tags/0.02.tar.gz
 Description: UNKNOWN
 Keywords: web3.py,Etherscan,Ethereum,Blockchain,API
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `web3r-0.1/README.md` & `web3r-0.2/README.md`

 * *Files identical despite different names*

### Comparing `web3r-0.1/setup.py` & `web3r-0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup
 
 setup(
   name = 'web3r',
   packages = ['web3r'],
-  version = '0.01',
+  version = '0.02',
   license='MIT',
   description = 'Web3R.py is a Python wrapper that enhances the functionality of Web3.py and integrates with Etherscan\'s API.',
   author = 'Finn Castro',
   author_email = 'your.email@domain.com',  # Update with your email
   url = 'https://github.com/FinnCastro/Web3R.py',
-  download_url = 'https://github.com/FinnCastro/Web3R.py/archive/refs/tags/0.01.tar.gz',
+  download_url = 'https://github.com/FinnCastro/Web3R.py/archive/refs/tags/0.02.tar.gz',
   keywords = ['web3.py', 'Etherscan', 'Ethereum', 'Blockchain', 'API'],
   install_requires=[
           'web3',  # Assuming that your project depends on web3 and requests
           'requests',
           'pandas',
           'numpy',
           'etherscan-python',
```

### Comparing `web3r-0.1/web3r/Web3R.py` & `web3r-0.2/web3r/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+# Import the required modules and classes
 from web3 import Web3
-from Tokens.Tokens import Tokens
 from web3.providers import BaseProvider
 from etherscan import Etherscan
-from Utils.Utils import Utils
-from Pricer.Pricer import Pricer
-from TheGraphUniswapV3.TheGraphUniswapV3 import TheGraphUniswapV3
+from web3r.Pricer import Pricer
+from web3r.Utils import Utils
+from web3r.TheGraphUniswapV3 import TheGraphUniswapV3
+from web3r.Tokens import Tokens
 
 class Web3R(Web3):
     """
     Main client class that wraps Web3 and Etherscan, and adds additional functionality for research.
     """
     
     def __init__(self, web3_provider: BaseProvider, etherscan_api_token: str) -> None:
@@ -37,8 +38,10 @@
         Checks if the Web3 and Etherscan instances are connected and available.
 
         :return: True if both services are available, False otherwise.
         """
         try:
             return self.web3.isConnected() and self.etherscan.get_eth_supply() is not None
         except Exception:
-            return False
+            return False
+        
+#
```

### Comparing `web3r-0.1/web3r.egg-info/PKG-INFO` & `web3r-0.2/web3r.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: web3r
-Version: 0.1
+Version: 0.2
 Summary: Web3R.py is a Python wrapper that enhances the functionality of Web3.py and integrates with Etherscan's API.
 Home-page: https://github.com/FinnCastro/Web3R.py
 Author: Finn Castro
 Author-email: your.email@domain.com
 License: MIT
-Download-URL: https://github.com/FinnCastro/Web3R.py/archive/refs/tags/0.01.tar.gz
+Download-URL: https://github.com/FinnCastro/Web3R.py/archive/refs/tags/0.02.tar.gz
 Description: UNKNOWN
 Keywords: web3.py,Etherscan,Ethereum,Blockchain,API
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
```

