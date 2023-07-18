# Comparing `tmp/AshCrypt-2.0.3.tar.gz` & `tmp/AshCrypt-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/AshCrypt-2.0.3.tar", last modified: Tue Jul 18 21:33:49 2023, max compression
+gzip compressed data, was "dist/AshCrypt-2.0.4.tar", last modified: Tue Jul 18 22:06:09 2023, max compression
```

## Comparing `AshCrypt-2.0.3.tar` & `AshCrypt-2.0.4.tar`

### file list

```diff
@@ -1,34 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:33:49.000000 AshCrypt-2.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:33:49.000000 AshCrypt-2.0.3/AshCrypt/
--rw-r--r--   0 runner    (1001) docker     (123)    38210 2023-07-18 21:33:37.000000 AshCrypt-2.0.3/AshCrypt/AshCryptGUI.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-18 21:33:37.000000 AshCrypt-2.0.3/AshCrypt/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-18 21:33:37.000000 AshCrypt-2.0.3/AshCrypt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:33:49.000000 AshCrypt-2.0.3/AshCrypt/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-18 21:33:37.000000 AshCrypt-2.0.3/AshCrypt/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-07-18 21:33:37.000000 AshCrypt-2.0.3/AshCrypt/__pycache__/crypt.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     7371 2023-07-18 21:33:37.000000 AshCrypt-2.0.3/AshCrypt/__pycache__/database.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-07-18 21:33:37.000000 AshCrypt-2.0.3/AshCrypt/__pycache__/filecrypt.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-18 21:33:37.000000 AshCrypt-2.0.3/AshCrypt/__pycache__/qr.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-07-18 21:33:37.000000 AshCrypt-2.0.3/AshCrypt/__pycache__/textcrypt.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-07-18 21:33:37.000000 AshCrypt-2.0.3/AshCrypt/clicrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-07-18 21:33:37.000000 AshCrypt-2.0.3/AshCrypt/crypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-07-18 21:33:37.000000 AshCrypt-2.0.3/AshCrypt/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-07-18 21:33:37.000000 AshCrypt-2.0.3/AshCrypt/filecrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-18 21:33:37.000000 AshCrypt-2.0.3/AshCrypt/qr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-18 21:33:37.000000 AshCrypt-2.0.3/AshCrypt/textcrypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:33:49.000000 AshCrypt-2.0.3/AshCrypt/unittests/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-18 21:33:37.000000 AshCrypt-2.0.3/AshCrypt/unittests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:33:49.000000 AshCrypt-2.0.3/AshCrypt/unittests/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-07-18 21:33:37.000000 AshCrypt-2.0.3/AshCrypt/unittests/__pycache__/unittest_crypt.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-07-18 21:33:37.000000 AshCrypt-2.0.3/AshCrypt/unittests/unittest_crypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:33:49.000000 AshCrypt-2.0.3/AshCrypt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-18 21:33:49.000000 AshCrypt-2.0.3/AshCrypt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-18 21:33:49.000000 AshCrypt-2.0.3/AshCrypt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 21:33:49.000000 AshCrypt-2.0.3/AshCrypt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-18 21:33:49.000000 AshCrypt-2.0.3/AshCrypt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-18 21:33:49.000000 AshCrypt-2.0.3/AshCrypt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-18 21:33:37.000000 AshCrypt-2.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-18 21:33:49.000000 AshCrypt-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21175 2023-07-18 21:33:37.000000 AshCrypt-2.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 21:33:49.000000 AshCrypt-2.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-18 21:33:37.000000 AshCrypt-2.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:06:09.000000 AshCrypt-2.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:06:09.000000 AshCrypt-2.0.4/AshCrypt/
+-rw-r--r--   0 runner    (1001) docker     (123)    38210 2023-07-18 22:05:52.000000 AshCrypt-2.0.4/AshCrypt/AshCryptGUI.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-18 22:05:52.000000 AshCrypt-2.0.4/AshCrypt/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-18 22:05:52.000000 AshCrypt-2.0.4/AshCrypt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-07-18 22:05:52.000000 AshCrypt-2.0.4/AshCrypt/clicrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-07-18 22:05:52.000000 AshCrypt-2.0.4/AshCrypt/crypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-07-18 22:05:52.000000 AshCrypt-2.0.4/AshCrypt/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-07-18 22:05:52.000000 AshCrypt-2.0.4/AshCrypt/filecrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-18 22:05:52.000000 AshCrypt-2.0.4/AshCrypt/qr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-18 22:05:52.000000 AshCrypt-2.0.4/AshCrypt/textcrypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:06:09.000000 AshCrypt-2.0.4/AshCrypt/unittests/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-18 22:05:52.000000 AshCrypt-2.0.4/AshCrypt/unittests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-18 22:05:52.000000 AshCrypt-2.0.4/AshCrypt/unittests/unittest_crypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:06:09.000000 AshCrypt-2.0.4/AshCrypt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-18 22:06:08.000000 AshCrypt-2.0.4/AshCrypt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-18 22:06:08.000000 AshCrypt-2.0.4/AshCrypt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 22:06:08.000000 AshCrypt-2.0.4/AshCrypt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-18 22:06:08.000000 AshCrypt-2.0.4/AshCrypt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-18 22:06:08.000000 AshCrypt-2.0.4/AshCrypt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-18 22:06:09.000000 AshCrypt-2.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21175 2023-07-18 22:05:53.000000 AshCrypt-2.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 22:06:09.000000 AshCrypt-2.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-18 22:05:53.000000 AshCrypt-2.0.4/setup.py
```

### Comparing `AshCrypt-2.0.3/AshCrypt/AshCryptGUI.py` & `AshCrypt-2.0.4/AshCrypt/AshCryptGUI.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-2.0.3/AshCrypt/clicrypt.py` & `AshCrypt-2.0.4/AshCrypt/clicrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-2.0.3/AshCrypt/crypt.py` & `AshCrypt-2.0.4/AshCrypt/crypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-2.0.3/AshCrypt/database.py` & `AshCrypt-2.0.4/AshCrypt/database.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-2.0.3/AshCrypt/filecrypt.py` & `AshCrypt-2.0.4/AshCrypt/filecrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-2.0.3/AshCrypt/textcrypt.py` & `AshCrypt-2.0.4/AshCrypt/textcrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-2.0.3/AshCrypt/unittests/unittest_crypt.py` & `AshCrypt-2.0.4/AshCrypt/unittests/unittest_crypt.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import unittest
 import struct
-import AshCrypt.crypt as Ash
+import AshCrypt.crypt as cp
 
 
 class AshModuleTesting(unittest.TestCase):
     def setUp(self) -> None:
         self.message1 = 'Hello there testing if it works'
         self.message2 = b'this is bytes now'
         self.mainkey = '6ce113be19e898c2b98df82b7fa8efb166928925fc05574a54eb1114c3410900'
-        self.ins1 = Ash.Enc(message=self.message1, mainkey=self.mainkey)
+        self.ins1 = cp.Enc(message=self.message1, mainkey=self.mainkey)
         self.string_message = self.ins1.enc_to_str()
         self.bytes_message = self.ins1.enc_to_bytes()
-        self.ins2 = Ash.Dec(message=self.bytes_message, mainkey=self.mainkey)
+        self.ins2 = cp.Dec(message=self.bytes_message, mainkey=self.mainkey)
 
     def tearDown(self) -> None:
         pass
 
     def test_KeyLength(self):
-        self.assertEqual(32, bytes.fromhex(Ash.Enc.genkey()).__len__())
+        self.assertEqual(32, bytes.fromhex(cp.Enc.genkey()).__len__())
 
     def test_KeyType(self):
-        self.assertIs(str, type(Ash.Enc.genkey()))
+        self.assertIs(str, type(cp.Enc.genkey()))
 
     def test_HMAC(self):
         self.assertTrue(self.bytes_message[:64] == self.ins1.HMAC())
 
     def test_IV(self):
         self.assertTrue(self.bytes_message[64:80] == self.ins1.iv)
 
@@ -68,24 +68,24 @@
     def test_Iterations_Comp(self):
         self.assertEqual(self.ins1.iterations, self.ins2.rec_iterations)
 
     def test_Ciphertext_Comp(self):
         self.assertEqual(self.ins1.ciphertext(), self.ins2.rec_ciphertext)
 
     def test_HMAC_MismatchError(self):
-        tampered_HMAC = self.ins1.enc_to_bytes()[:63] + b'1'
-        tampered_message = tampered_HMAC + self.ins1.enc_to_bytes()[64:]
-        with self.assertRaises(Ash.MessageTamperingError):
-            Ash.Dec(message=tampered_message, mainkey=self.mainkey)
+        tampered_hmac = self.ins1.enc_to_bytes()[:63] + b'1'
+        tampered_message = tampered_hmac + self.ins1.enc_to_bytes()[64:]
+        with self.assertRaises(cp.MessageTamperingError):
+            cp.Dec(message=tampered_message, mainkey=self.mainkey)
 
     def test_IterationsOutOfRangeError2(self):
         enb = self.ins1.enc_to_bytes()
         tampered_message = enb[:112] + struct.pack('!I', 100001) + enb[116:]
-        with self.assertRaises(Ash.IterationsOutofaRangeError):
-            Ash.Dec(message=tampered_message, mainkey=self.mainkey)
+        with self.assertRaises(cp.IterationsOutofaRangeError):
+            cp.Dec(message=tampered_message, mainkey=self.mainkey)
 
     def test_DecOutputBytes(self):
         self.assertEqual(bytes, type(self.ins2.dec_to_bytes()))
 
     def test_DecOutputString(self):
         self.assertEqual(str, type(self.ins2.dec_to_str()))
```

### Comparing `AshCrypt-2.0.3/AshCrypt.egg-info/PKG-INFO` & `AshCrypt-2.0.4/AshCrypt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshCrypt
-Version: 2.0.3
+Version: 2.0.4
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 License: UNKNOWN
 Description: # Cryptography App &  Library : AES-256
         ##  Objective ##
```

### Comparing `AshCrypt-2.0.3/PKG-INFO` & `AshCrypt-2.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshCrypt
-Version: 2.0.3
+Version: 2.0.4
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 License: UNKNOWN
 Description: # Cryptography App &  Library : AES-256
         ##  Objective ##
```

### Comparing `AshCrypt-2.0.3/README.md` & `AshCrypt-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `AshCrypt-2.0.3/setup.py` & `AshCrypt-2.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup , find_packages
 
 with open('AshCrypt/README.md','r') as f:
     readme = f.read()
 
 setup(
     name='AshCrypt',
-    version='2.0.3',
+    version='2.0.4',
     author='Ashref Gwader',
     author_email='AshrefGw@proton.me',
     python_requires='>=3.7',
     description="Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with"
                 " a database module to store encrypted content.",
     long_description_content_type='text/markdown',
     long_description=readme,
```

