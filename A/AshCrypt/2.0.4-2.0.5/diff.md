# Comparing `tmp/AshCrypt-2.0.4.tar.gz` & `tmp/AshCrypt-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/AshCrypt-2.0.4.tar", last modified: Tue Jul 18 22:06:09 2023, max compression
+gzip compressed data, was "dist/AshCrypt-2.0.5.tar", last modified: Wed Jul 19 09:53:15 2023, max compression
```

## Comparing `AshCrypt-2.0.4.tar` & `AshCrypt-2.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:06:09.000000 AshCrypt-2.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:06:09.000000 AshCrypt-2.0.4/AshCrypt/
--rw-r--r--   0 runner    (1001) docker     (123)    38210 2023-07-18 22:05:52.000000 AshCrypt-2.0.4/AshCrypt/AshCryptGUI.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-18 22:05:52.000000 AshCrypt-2.0.4/AshCrypt/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-18 22:05:52.000000 AshCrypt-2.0.4/AshCrypt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-07-18 22:05:52.000000 AshCrypt-2.0.4/AshCrypt/clicrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-07-18 22:05:52.000000 AshCrypt-2.0.4/AshCrypt/crypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-07-18 22:05:52.000000 AshCrypt-2.0.4/AshCrypt/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-07-18 22:05:52.000000 AshCrypt-2.0.4/AshCrypt/filecrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-18 22:05:52.000000 AshCrypt-2.0.4/AshCrypt/qr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-18 22:05:52.000000 AshCrypt-2.0.4/AshCrypt/textcrypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:06:09.000000 AshCrypt-2.0.4/AshCrypt/unittests/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-18 22:05:52.000000 AshCrypt-2.0.4/AshCrypt/unittests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-18 22:05:52.000000 AshCrypt-2.0.4/AshCrypt/unittests/unittest_crypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:06:09.000000 AshCrypt-2.0.4/AshCrypt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-18 22:06:08.000000 AshCrypt-2.0.4/AshCrypt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-18 22:06:08.000000 AshCrypt-2.0.4/AshCrypt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 22:06:08.000000 AshCrypt-2.0.4/AshCrypt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-18 22:06:08.000000 AshCrypt-2.0.4/AshCrypt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-18 22:06:08.000000 AshCrypt-2.0.4/AshCrypt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-18 22:06:09.000000 AshCrypt-2.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21175 2023-07-18 22:05:53.000000 AshCrypt-2.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 22:06:09.000000 AshCrypt-2.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-18 22:05:53.000000 AshCrypt-2.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:53:15.000000 AshCrypt-2.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:53:15.000000 AshCrypt-2.0.5/AshCrypt/
+-rw-r--r--   0 runner    (1001) docker     (123)    38210 2023-07-19 09:53:04.000000 AshCrypt-2.0.5/AshCrypt/AshCryptGUI.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-19 09:53:04.000000 AshCrypt-2.0.5/AshCrypt/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-19 09:53:04.000000 AshCrypt-2.0.5/AshCrypt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-07-19 09:53:04.000000 AshCrypt-2.0.5/AshCrypt/clicrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-07-19 09:53:04.000000 AshCrypt-2.0.5/AshCrypt/crypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-07-19 09:53:04.000000 AshCrypt-2.0.5/AshCrypt/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-07-19 09:53:04.000000 AshCrypt-2.0.5/AshCrypt/filecrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-19 09:53:04.000000 AshCrypt-2.0.5/AshCrypt/qr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-19 09:53:04.000000 AshCrypt-2.0.5/AshCrypt/textcrypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:53:15.000000 AshCrypt-2.0.5/AshCrypt/unittests/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-19 09:53:04.000000 AshCrypt-2.0.5/AshCrypt/unittests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-19 09:53:04.000000 AshCrypt-2.0.5/AshCrypt/unittests/unittest_crypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:53:15.000000 AshCrypt-2.0.5/AshCrypt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-19 09:53:15.000000 AshCrypt-2.0.5/AshCrypt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-19 09:53:15.000000 AshCrypt-2.0.5/AshCrypt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 09:53:15.000000 AshCrypt-2.0.5/AshCrypt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-19 09:53:15.000000 AshCrypt-2.0.5/AshCrypt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-19 09:53:15.000000 AshCrypt-2.0.5/AshCrypt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-19 09:53:15.000000 AshCrypt-2.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21164 2023-07-19 09:53:04.000000 AshCrypt-2.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 09:53:15.000000 AshCrypt-2.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-19 09:53:04.000000 AshCrypt-2.0.5/setup.py
```

### Comparing `AshCrypt-2.0.4/AshCrypt/AshCryptGUI.py` & `AshCrypt-2.0.5/AshCrypt/AshCryptGUI.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-2.0.4/AshCrypt/clicrypt.py` & `AshCrypt-2.0.5/AshCrypt/clicrypt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from AshCrypt import filecrypt as Af
-from AshCrypt import textcrypt as At
+from AshCrypt import filecrypt as af
+from AshCrypt import textcrypt as at
 import os.path
 import sys
 
 
 print('Welcome to the CLI')
 
 commands = 'Commands : \n' \
@@ -90,24 +90,24 @@
     while outer:
         global key
         key = ''
         i = input('Do you have a key ?(y/n) : ')
         input_wrap(i)
         if i.lower() == 'n':
             print("Here's your key : ")
-            key = At.Crypt.genkey()
+            key = at.Crypt.genkey()
             print(key)
             inner = False
             outer = False
         elif i.lower() == 'y':
             while inner:
                 print('insert your key here : ')
                 kk = input()
                 input_wrap(kk)
-                if At.Crypt.keyverify(kk) == 1:
+                if at.Crypt.keyverify(kk) == 1:
                     print('Key selected\n')
                     key = kk
                     inner = False
                     outer = False
                 else:
                     print('Enter a valid key !\n')
 
@@ -119,15 +119,15 @@
     keysetup()
     while encflag:
         print()
         global key
         print("press c to view commands.. ")
         message = input('Encrypt a message : ')
         input_wrap(message)
-        a = At.Crypt(message, key=key)
+        a = at.Crypt(message, key=key)
         enc = a.encrypt()
         if (enc[0]) == 1:
             print("Success ! Here's the message : ")
             print('\t', enc[1], '\n')
         else:
             print('Error occurred during the encryption process\n')
 
@@ -139,15 +139,15 @@
     keysetup()
     while decFlag:
         print()
         global key
         print("press c to view commands.. ")
         message = input('Decrypt a message : ')
         input_wrap(message)
-        a = At.Crypt(message, key=key)
+        a = at.Crypt(message, key=key)
         dec = a.decrypt()
         if (dec[0]) == 1:
             print("Success ! Here's the message : ")
             print('\t', dec[1], '\n')
         else:
             print('Error occurred during the decryption process\n')
 
@@ -160,21 +160,21 @@
 
 def file_dec():
     keysetup()
     while file_decFlag:
         print()
         global key
         pre = input(
-            "running file decryption mode , press the known commands or 'Enter' to continue.. : ")
+            "Running file decryption mode , press the known commands or 'Enter' to continue.. : ")
         print()
         input_wrap(pre)
         if pre == '':
             print("You can use the commands AFTER entering the file name.. ")
             filename = input('Enter full file name to be Decrypted : ')
-            target = Af.CryptFile(filename, key)
+            target = af.CryptFile(filename, key)
             a = target.decrypt()
             if a == 1:
                 print('File successfully decrypted + removed .crypt extension')
                 print(f'File is now named {os.path.splitext(filename)[0]}')
             if a == 2:
                 print('Cannot decrypt the file  when it is already empty')
             if a == 3:
@@ -196,24 +196,24 @@
 
 def file_enc():
     keysetup()
     while file_encFlag:
         print()
         global key
         pre = input(
-            "running file encryption mode, press the known commands or 'Enter' to continue.. : ")
+            "Running file encryption mode, press the known commands or 'Enter' to continue.. : ")
         print()
         input_wrap(pre)
         if pre == '':
             print("You can use the commands AFTER entering the file name.. ")
             filename = input('Enter full file name to be Encrypted : ')
-            target = Af.CryptFile(filename, key)
+            target = af.CryptFile(filename, key)
             a = target.encrypt()
             if a == 1:
-                print('File successfully encrypted + added .crypt extension')
+                print("File successfully encrypted + added '.crypt' extension")
                 print(f"File is now named : '{filename}.crypt' ")
             if a == 2:
                 print('Cannot encrypt the file  when it is already empty')
             if a == 3:
                 print(
                     f'The file named : "{filename}" does not exists , try specifying the whole sys path')
             if a == 0:
```

### Comparing `AshCrypt-2.0.4/AshCrypt/crypt.py` & `AshCrypt-2.0.5/AshCrypt/crypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-2.0.4/AshCrypt/database.py` & `AshCrypt-2.0.5/AshCrypt/database.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-2.0.4/AshCrypt/filecrypt.py` & `AshCrypt-2.0.5/AshCrypt/filecrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-2.0.4/AshCrypt/textcrypt.py` & `AshCrypt-2.0.5/AshCrypt/textcrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-2.0.4/AshCrypt/unittests/unittest_crypt.py` & `AshCrypt-2.0.5/AshCrypt/unittests/unittest_crypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-2.0.4/AshCrypt.egg-info/PKG-INFO` & `AshCrypt-2.0.5/AshCrypt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshCrypt
-Version: 2.0.4
+Version: 2.0.5
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 License: UNKNOWN
 Description: # Cryptography App &  Library : AES-256
         ##  Objective ##
```

### Comparing `AshCrypt-2.0.4/PKG-INFO` & `AshCrypt-2.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshCrypt
-Version: 2.0.4
+Version: 2.0.5
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 License: UNKNOWN
 Description: # Cryptography App &  Library : AES-256
         ##  Objective ##
```

### Comparing `AshCrypt-2.0.4/README.md` & `AshCrypt-2.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -99,24 +99,24 @@
 **After the library is installed** 
 <br>To run the GUI 
 ```shell
 python -m AshCrypt.AshCryptGUI
 ```
 
 **NOTE**:
-You  can use `CliCrypt.py` which is an innovative command line interface (CLI) designed to provide encryption and decryption capabilities for both text and file data with no constraints intended for use within systems where you can't use GUI's.
+You  can use `clicrypt.py` which is an innovative command line interface (CLI) designed to provide encryption and decryption capabilities for both text and file data with no constraints intended for use within systems where you can't use GUI's.
 
 
 To run the CLI 
 ```shell
-python -m AshCrypt.CliCrypt
+python -m AshCrypt.clicrypt
 ```
 
 ## "crypt" Module ##
-The `crypt.py` Module is a comprehensive collection of carefully designed functions and code modules that facilitate optimal performance and reliability in data encryption and decryption operations  while ensuring the utmost security and 
+The `crypt.py` Module is a comprehensive collection of carefully designed functions and code modules that facilitate optimal performance and reliability in data encryption and decryption operations  while ensuring security and 
 confidentiality.
 
 <br>It uses primitives from the `cryptography.py` library with added security features while keeping it simple and highly flexible to provide a head-ache free solution for developers. 
 
 <br>You can check [Features](https://github.com/AshGw/AES-256#features) tag below to learn more about the security features.
 <br>You can check the [unittesting file](AshCrypt/unittests/unittest_crypt.py) to verify how it works.
```

### Comparing `AshCrypt-2.0.4/setup.py` & `AshCrypt-2.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup , find_packages
 
 with open('AshCrypt/README.md','r') as f:
     readme = f.read()
 
 setup(
     name='AshCrypt',
-    version='2.0.4',
+    version='2.0.5',
     author='Ashref Gwader',
     author_email='AshrefGw@proton.me',
     python_requires='>=3.7',
     description="Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with"
                 " a database module to store encrypted content.",
     long_description_content_type='text/markdown',
     long_description=readme,
```

