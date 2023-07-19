# Comparing `tmp/pysasl-1.1.0.tar.gz` & `tmp/pysasl-1.2.0.tar.gz`

## Comparing `pysasl-1.1.0.tar` & `pysasl-1.2.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 pysasl-1.1.0/importlib_metadata.pyi
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 pysasl-1.1.0/pysasl/__about__.py
--rw-r--r--   0        0        0     3251 2020-02-02 00:00:00.000000 pysasl-1.1.0/pysasl/__init__.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 pysasl-1.1.0/pysasl/exception.py
--rw-r--r--   0        0        0     6373 2020-02-02 00:00:00.000000 pysasl-1.1.0/pysasl/hashing.py
--rw-r--r--   0        0        0     4981 2020-02-02 00:00:00.000000 pysasl-1.1.0/pysasl/identity.py
--rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 pysasl-1.1.0/pysasl/prep.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pysasl-1.1.0/pysasl/py.typed
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 pysasl-1.1.0/pysasl/creds/__init__.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 pysasl-1.1.0/pysasl/creds/client.py
--rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 pysasl-1.1.0/pysasl/creds/external.py
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 pysasl-1.1.0/pysasl/creds/plain.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 pysasl-1.1.0/pysasl/creds/server.py
--rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 pysasl-1.1.0/pysasl/mechanism/__init__.py
--rw-r--r--   0        0        0     3460 2020-02-02 00:00:00.000000 pysasl-1.1.0/pysasl/mechanism/crammd5.py
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 pysasl-1.1.0/pysasl/mechanism/external.py
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 pysasl-1.1.0/pysasl/mechanism/login.py
--rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 pysasl-1.1.0/pysasl/mechanism/oauth.py
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 pysasl-1.1.0/pysasl/mechanism/plain.py
--rw-r--r--   0        0        0     3766 2020-02-02 00:00:00.000000 pysasl-1.1.0/test/test_crammd5.py
--rw-r--r--   0        0        0     6060 2020-02-02 00:00:00.000000 pysasl-1.1.0/test/test_creds.py
--rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 pysasl-1.1.0/test/test_external.py
--rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 pysasl-1.1.0/test/test_login.py
--rw-r--r--   0        0        0     3473 2020-02-02 00:00:00.000000 pysasl-1.1.0/test/test_oauth.py
--rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 pysasl-1.1.0/test/test_plain.py
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 pysasl-1.1.0/test/test_prep.py
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 pysasl-1.1.0/.gitignore
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 pysasl-1.1.0/LICENSE.md
--rw-r--r--   0        0        0     6177 2020-02-02 00:00:00.000000 pysasl-1.1.0/README.md
--rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 pysasl-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     8369 2020-02-02 00:00:00.000000 pysasl-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 pysasl-1.2.0/importlib_metadata.pyi
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 pysasl-1.2.0/pysasl/__about__.py
+-rw-r--r--   0        0        0     3251 2020-02-02 00:00:00.000000 pysasl-1.2.0/pysasl/__init__.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 pysasl-1.2.0/pysasl/exception.py
+-rw-r--r--   0        0        0     6373 2020-02-02 00:00:00.000000 pysasl-1.2.0/pysasl/hashing.py
+-rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 pysasl-1.2.0/pysasl/identity.py
+-rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 pysasl-1.2.0/pysasl/prep.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pysasl-1.2.0/pysasl/py.typed
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 pysasl-1.2.0/pysasl/creds/__init__.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 pysasl-1.2.0/pysasl/creds/client.py
+-rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 pysasl-1.2.0/pysasl/creds/external.py
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 pysasl-1.2.0/pysasl/creds/plain.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 pysasl-1.2.0/pysasl/creds/server.py
+-rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 pysasl-1.2.0/pysasl/mechanism/__init__.py
+-rw-r--r--   0        0        0     3460 2020-02-02 00:00:00.000000 pysasl-1.2.0/pysasl/mechanism/crammd5.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 pysasl-1.2.0/pysasl/mechanism/external.py
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 pysasl-1.2.0/pysasl/mechanism/login.py
+-rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 pysasl-1.2.0/pysasl/mechanism/oauth.py
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 pysasl-1.2.0/pysasl/mechanism/plain.py
+-rw-r--r--   0        0        0     3766 2020-02-02 00:00:00.000000 pysasl-1.2.0/test/test_crammd5.py
+-rw-r--r--   0        0        0     6166 2020-02-02 00:00:00.000000 pysasl-1.2.0/test/test_creds.py
+-rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 pysasl-1.2.0/test/test_external.py
+-rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 pysasl-1.2.0/test/test_login.py
+-rw-r--r--   0        0        0     3473 2020-02-02 00:00:00.000000 pysasl-1.2.0/test/test_oauth.py
+-rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 pysasl-1.2.0/test/test_plain.py
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 pysasl-1.2.0/test/test_prep.py
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 pysasl-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 pysasl-1.2.0/LICENSE.md
+-rw-r--r--   0        0        0     6177 2020-02-02 00:00:00.000000 pysasl-1.2.0/README.md
+-rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 pysasl-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     8369 2020-02-02 00:00:00.000000 pysasl-1.2.0/PKG-INFO
```

### Comparing `pysasl-1.1.0/pysasl/__init__.py` & `pysasl-1.2.0/pysasl/__init__.py`

 * *Files identical despite different names*

### Comparing `pysasl-1.1.0/pysasl/exception.py` & `pysasl-1.2.0/pysasl/exception.py`

 * *Files identical despite different names*

### Comparing `pysasl-1.1.0/pysasl/hashing.py` & `pysasl-1.2.0/pysasl/hashing.py`

 * *Files identical despite different names*

### Comparing `pysasl-1.1.0/pysasl/identity.py` & `pysasl-1.2.0/pysasl/identity.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,20 @@
     """Represents an server-side identity that credentials will be
     authenticated against.
 
     """
 
     __slots__: Sequence[str] = []
 
+    @property
+    @abstractmethod
+    def authcid(self) -> str:
+        """The authentication identity, e.g. a login username."""
+        ...
+
     @abstractmethod
     def compare_authcid(self, authcid: str) -> bool:
         """Compare the identity's authcid with the given *authcid*.
 
         Args:
             authcid: The authentication identity string value.
 
@@ -60,32 +66,36 @@
     def __init__(self, authcid: str, secret: str, *,
                  prepare: Preparation = saslprep) -> None:
         super().__init__()
         self._authcid = authcid
         self._secret = secret
         self._prepare = prepare
 
+    @property
+    def authcid(self) -> str:
+        return self._authcid
+
     def _compare(self, this: str, that: str) -> bool:
         prepare = self._prepare
         prepared_this = prepare(this).encode('utf-8')
         prepared_that = prepare(that).encode('utf-8')
         return secrets.compare_digest(prepared_this, prepared_that)
 
     def compare_authcid(self, authcid: str) -> bool:
-        return self._compare(self._authcid, authcid)
+        return self._compare(self.authcid, authcid)
 
     def compare_secret(self, secret: str) -> bool:
         return self._compare(self._secret, secret)
 
     def get_clear_secret(self) -> str:
         """Return the cleartext secret string."""
         return self._secret
 
     def __repr__(self) -> str:
-        return f'ClearIdentity({self._authcid!r}, ...)'
+        return f'ClearIdentity({self.authcid!r}, ...)'
 
 
 class HashedIdentity(Identity):
     """An :class:`Identity` where the secret has been hashed for storage.
 
     Args:
         authcid: The authentication identity, e.g. a login username.
@@ -102,14 +112,18 @@
                  prepare: Preparation = saslprep) -> None:
         super().__init__()
         self._authcid = authcid
         self._digest = digest
         self._hash = hash
         self._prepare = prepare
 
+    @property
+    def authcid(self) -> str:
+        return self._authcid
+
     @classmethod
     def create(cls, authcid: str, secret: str, *,
                hash: HashInterface,
                prepare: Preparation = saslprep) -> Self:
         """Prepare and hash the given *secret*, returning a
         :class:`HashedIdentity`.
 
@@ -136,15 +150,15 @@
     def _compare(self, this: str, that: str) -> bool:
         prepare = self._prepare
         prepared_this = prepare(this).encode('utf-8')
         prepared_that = prepare(that).encode('utf-8')
         return secrets.compare_digest(prepared_this, prepared_that)
 
     def compare_authcid(self, authcid: str) -> bool:
-        return self._compare(self._authcid, authcid)
+        return self._compare(self.authcid, authcid)
 
     def compare_secret(self, secret: str) -> bool:
         return self._hash.verify(self._prepare(secret), self._digest)
 
     def get_clear_secret(self) -> Optional[str]:
         """Return the cleartext secret string, only if :attr:`.hash` is
         :class:`~pysasl.hashing.Cleartext`.
@@ -152,8 +166,8 @@
         """
         if isinstance(self.hash, Cleartext):
             return self.digest
         else:
             return None
 
     def __repr__(self) -> str:
-        return f'HashedIdentity({self._authcid}, ..., hash={self._hash!r})'
+        return f'HashedIdentity({self.authcid}, ..., hash={self._hash!r})'
```

### Comparing `pysasl-1.1.0/pysasl/prep.py` & `pysasl-1.2.0/pysasl/prep.py`

 * *Files identical despite different names*

### Comparing `pysasl-1.1.0/pysasl/creds/__init__.py` & `pysasl-1.2.0/pysasl/creds/__init__.py`

 * *Files identical despite different names*

### Comparing `pysasl-1.1.0/pysasl/creds/client.py` & `pysasl-1.2.0/pysasl/creds/client.py`

 * *Files identical despite different names*

### Comparing `pysasl-1.1.0/pysasl/creds/external.py` & `pysasl-1.2.0/pysasl/creds/external.py`

 * *Files identical despite different names*

### Comparing `pysasl-1.1.0/pysasl/creds/plain.py` & `pysasl-1.2.0/pysasl/creds/plain.py`

 * *Files identical despite different names*

### Comparing `pysasl-1.1.0/pysasl/creds/server.py` & `pysasl-1.2.0/pysasl/creds/server.py`

 * *Files identical despite different names*

### Comparing `pysasl-1.1.0/pysasl/mechanism/__init__.py` & `pysasl-1.2.0/pysasl/mechanism/__init__.py`

 * *Files identical despite different names*

### Comparing `pysasl-1.1.0/pysasl/mechanism/crammd5.py` & `pysasl-1.2.0/pysasl/mechanism/crammd5.py`

 * *Files identical despite different names*

### Comparing `pysasl-1.1.0/pysasl/mechanism/external.py` & `pysasl-1.2.0/pysasl/mechanism/external.py`

 * *Files identical despite different names*

### Comparing `pysasl-1.1.0/pysasl/mechanism/login.py` & `pysasl-1.2.0/pysasl/mechanism/login.py`

 * *Files identical despite different names*

### Comparing `pysasl-1.1.0/pysasl/mechanism/oauth.py` & `pysasl-1.2.0/pysasl/mechanism/oauth.py`

 * *Files identical despite different names*

### Comparing `pysasl-1.1.0/pysasl/mechanism/plain.py` & `pysasl-1.2.0/pysasl/mechanism/plain.py`

 * *Files identical despite different names*

### Comparing `pysasl-1.1.0/test/test_crammd5.py` & `pysasl-1.2.0/test/test_crammd5.py`

 * *Files identical despite different names*

### Comparing `pysasl-1.1.0/test/test_creds.py` & `pysasl-1.2.0/test/test_creds.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 
 class TestCreds(unittest.TestCase):
 
     def test_hashed_builtin_good(self) -> None:
         creds = PlainCredentials('username', 'password')
         stored = HashedIdentity('username', password_sha256, hash=builtin_hash)
+        self.assertEqual('username', stored.authcid)
         self.assertEqual(password_sha256, stored.digest)
         self.assertTrue(creds.verify(stored))
         self.assertIsNone(stored.get_clear_secret())
 
     def test_hashed_builtin_good_prepare(self) -> None:
         creds = PlainCredentials('user\u00ADname', 'pass\u00ADword')
         stored = HashedIdentity.create('us\u200Bername',
@@ -84,14 +85,15 @@
         with self.assertRaises(ValueError):
             builtin_hash.verify('password',
                                 password_sha256.replace('pbkdf2-', '', 1))
 
     def test_cleartext_good(self) -> None:
         creds = PlainCredentials('username', 'password')
         stored = ClearIdentity('username', 'password')
+        self.assertEqual('username', stored.authcid)
         self.assertTrue(creds.verify(stored))
 
     def test_cleartext_good_prepare(self) -> None:
         creds = PlainCredentials('user\u00ADname', 'pass\u00ADword')
         stored = ClearIdentity('us\u200Bername', 'pa\u200Bssword')
         self.assertTrue(creds.verify(stored))
```

### Comparing `pysasl-1.1.0/test/test_external.py` & `pysasl-1.2.0/test/test_external.py`

 * *Files identical despite different names*

### Comparing `pysasl-1.1.0/test/test_login.py` & `pysasl-1.2.0/test/test_login.py`

 * *Files identical despite different names*

### Comparing `pysasl-1.1.0/test/test_oauth.py` & `pysasl-1.2.0/test/test_oauth.py`

 * *Files identical despite different names*

### Comparing `pysasl-1.1.0/test/test_plain.py` & `pysasl-1.2.0/test/test_plain.py`

 * *Files identical despite different names*

### Comparing `pysasl-1.1.0/test/test_prep.py` & `pysasl-1.2.0/test/test_prep.py`

 * *Files identical despite different names*

### Comparing `pysasl-1.1.0/.gitignore` & `pysasl-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pysasl-1.1.0/LICENSE.md` & `pysasl-1.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pysasl-1.1.0/README.md` & `pysasl-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pysasl-1.1.0/pyproject.toml` & `pysasl-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pysasl-1.1.0/PKG-INFO` & `pysasl-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysasl
-Version: 1.1.0
+Version: 1.2.0
 Summary: Pure Python SASL client and server library.
 Project-URL: Homepage, https://github.com/icgood/pysasl/
 Project-URL: API Documentation, https://icgood.github.io/pysasl/
 Author-email: Ian Good <ian@icgood.net>
 License: ## The MIT License (MIT)
         
         Copyright (c) 2022 Ian Good
```

