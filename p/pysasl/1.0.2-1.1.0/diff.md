# Comparing `tmp/pysasl-1.0.2.tar.gz` & `tmp/pysasl-1.1.0.tar.gz`

## Comparing `pysasl-1.0.2.tar` & `pysasl-1.1.0.tar`

### file list

```diff
@@ -1,32 +1,31 @@
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 pysasl-1.0.2/.flake8
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 pysasl-1.0.2/importlib_metadata.pyi
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 pysasl-1.0.2/pysasl/__about__.py
--rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 pysasl-1.0.2/pysasl/__init__.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pysasl-1.0.2/pysasl/config.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 pysasl-1.0.2/pysasl/exception.py
--rw-r--r--   0        0        0     8051 2020-02-02 00:00:00.000000 pysasl-1.0.2/pysasl/hashing.py
--rw-r--r--   0        0        0     4453 2020-02-02 00:00:00.000000 pysasl-1.0.2/pysasl/identity.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 pysasl-1.0.2/pysasl/prep.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pysasl-1.0.2/pysasl/py.typed
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 pysasl-1.0.2/pysasl/creds/__init__.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 pysasl-1.0.2/pysasl/creds/client.py
--rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 pysasl-1.0.2/pysasl/creds/external.py
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 pysasl-1.0.2/pysasl/creds/plain.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 pysasl-1.0.2/pysasl/creds/server.py
--rw-r--r--   0        0        0     4841 2020-02-02 00:00:00.000000 pysasl-1.0.2/pysasl/mechanism/__init__.py
--rw-r--r--   0        0        0     3904 2020-02-02 00:00:00.000000 pysasl-1.0.2/pysasl/mechanism/crammd5.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 pysasl-1.0.2/pysasl/mechanism/external.py
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 pysasl-1.0.2/pysasl/mechanism/login.py
--rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 pysasl-1.0.2/pysasl/mechanism/oauth.py
--rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 pysasl-1.0.2/pysasl/mechanism/plain.py
--rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 pysasl-1.0.2/test/test_crammd5.py
--rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 pysasl-1.0.2/test/test_creds.py
--rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 pysasl-1.0.2/test/test_external.py
--rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 pysasl-1.0.2/test/test_login.py
--rw-r--r--   0        0        0     3471 2020-02-02 00:00:00.000000 pysasl-1.0.2/test/test_oauth.py
--rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 pysasl-1.0.2/test/test_plain.py
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 pysasl-1.0.2/.gitignore
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 pysasl-1.0.2/LICENSE.md
--rw-r--r--   0        0        0     6217 2020-02-02 00:00:00.000000 pysasl-1.0.2/README.md
--rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 pysasl-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     8476 2020-02-02 00:00:00.000000 pysasl-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 pysasl-1.1.0/importlib_metadata.pyi
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 pysasl-1.1.0/pysasl/__about__.py
+-rw-r--r--   0        0        0     3251 2020-02-02 00:00:00.000000 pysasl-1.1.0/pysasl/__init__.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 pysasl-1.1.0/pysasl/exception.py
+-rw-r--r--   0        0        0     6373 2020-02-02 00:00:00.000000 pysasl-1.1.0/pysasl/hashing.py
+-rw-r--r--   0        0        0     4981 2020-02-02 00:00:00.000000 pysasl-1.1.0/pysasl/identity.py
+-rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 pysasl-1.1.0/pysasl/prep.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pysasl-1.1.0/pysasl/py.typed
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 pysasl-1.1.0/pysasl/creds/__init__.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 pysasl-1.1.0/pysasl/creds/client.py
+-rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 pysasl-1.1.0/pysasl/creds/external.py
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 pysasl-1.1.0/pysasl/creds/plain.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 pysasl-1.1.0/pysasl/creds/server.py
+-rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 pysasl-1.1.0/pysasl/mechanism/__init__.py
+-rw-r--r--   0        0        0     3460 2020-02-02 00:00:00.000000 pysasl-1.1.0/pysasl/mechanism/crammd5.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 pysasl-1.1.0/pysasl/mechanism/external.py
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 pysasl-1.1.0/pysasl/mechanism/login.py
+-rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 pysasl-1.1.0/pysasl/mechanism/oauth.py
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 pysasl-1.1.0/pysasl/mechanism/plain.py
+-rw-r--r--   0        0        0     3766 2020-02-02 00:00:00.000000 pysasl-1.1.0/test/test_crammd5.py
+-rw-r--r--   0        0        0     6060 2020-02-02 00:00:00.000000 pysasl-1.1.0/test/test_creds.py
+-rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 pysasl-1.1.0/test/test_external.py
+-rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 pysasl-1.1.0/test/test_login.py
+-rw-r--r--   0        0        0     3473 2020-02-02 00:00:00.000000 pysasl-1.1.0/test/test_oauth.py
+-rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 pysasl-1.1.0/test/test_plain.py
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 pysasl-1.1.0/test/test_prep.py
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 pysasl-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 pysasl-1.1.0/LICENSE.md
+-rw-r--r--   0        0        0     6177 2020-02-02 00:00:00.000000 pysasl-1.1.0/README.md
+-rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 pysasl-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     8369 2020-02-02 00:00:00.000000 pysasl-1.1.0/PKG-INFO
```

### Comparing `pysasl-1.0.2/pysasl/__init__.py` & `pysasl-1.1.0/pysasl/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,89 +1,79 @@
 
 import sys
 from collections import OrderedDict
 from typing import Iterable, Optional, Sequence
-from typing_extensions import Final, Self
+from typing_extensions import Self
 
 if sys.version_info >= (3, 10):  # pragma: no cover
     from importlib.metadata import entry_points
 else:  # pragma: no cover
     from importlib_metadata import entry_points
 
 from . import mechanism
 from .__about__ import __version__
-from .config import default_config, SASLConfig
 from .mechanism import Mechanism, ServerMechanism, ClientMechanism
 
 __all__ = ['__version__', 'SASLAuth']
 
 
-class SASLAuth(SASLConfig):
+class SASLAuth:
     """Manages the mechanisms available for authentication attempts.
 
     Args:
         mechanisms: List of available SASL mechanism objects.
-        config: The configuration object.
 
     """
 
-    __slots__ = ['config', '_server_mechanisms', '_client_mechanisms']
+    __slots__ = ['_server_mechanisms', '_client_mechanisms']
 
-    def __init__(self, mechanisms: Sequence[Mechanism], *,
-                 config: SASLConfig = default_config) -> None:
+    def __init__(self, mechanisms: Sequence[Mechanism]) -> None:
         super().__init__()
-        self.config: Final = config
         self._server_mechanisms = OrderedDict(
             (mech.name, mech)
             for mech in mechanisms if isinstance(mech, ServerMechanism))
         self._client_mechanisms = OrderedDict(
             (mech.name, mech)
             for mech in mechanisms if isinstance(mech, ClientMechanism))
 
     @classmethod
-    def defaults(cls, *, config: SASLConfig = default_config) -> Self:
+    def defaults(cls) -> Self:
         """Uses the default built-in authentication mechanisms, ``PLAIN`` and
         ``LOGIN``.
 
-        Args:
-            config: The configuration object.
-
         Returns:
             A new :class:`SASLAuth` object.
 
         """
         return cls.named([b'PLAIN', b'LOGIN'])
 
     @classmethod
-    def named(cls, names: Iterable[bytes], *,
-              config: SASLConfig = default_config) -> Self:
+    def named(cls, names: Iterable[bytes]) -> Self:
         """Uses the built-in authentication mechanisms that match a provided
         name.
 
         Args:
             names: The authentication mechanism names.
-            config: The configuration object.
 
         Returns:
             A new :class:`SASLAuth` object.
 
         Raises:
             KeyError: A mechanism name was not recognized.
 
         """
-        builtin = {m.name: m for m in cls._get_builtin_mechanisms(config)}
+        builtin = {m.name: m for m in cls._get_builtin_mechanisms()}
         return cls([builtin[name] for name in names])
 
     @classmethod
-    def _get_builtin_mechanisms(cls, config: SASLConfig) \
-            -> Iterable[Mechanism]:
+    def _get_builtin_mechanisms(cls) -> Iterable[Mechanism]:
         group = mechanism.__package__
         for entry_point in entry_points(group=group):
             mech_cls = entry_point.load()
-            yield mech_cls(entry_point.name, config)
+            yield mech_cls(entry_point.name)
 
     @property
     def server_mechanisms(self) -> Sequence[ServerMechanism]:
         """List of available :class:`~pysasl.mechanism.ServerMechanism`
         objects.
 
         """
```

### Comparing `pysasl-1.0.2/pysasl/exception.py` & `pysasl-1.1.0/pysasl/exception.py`

 * *Files identical despite different names*

### Comparing `pysasl-1.0.2/pysasl/hashing.py` & `pysasl-1.1.0/pysasl/hashing.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,22 +7,15 @@
 import hashlib
 import secrets
 from abc import abstractmethod
 from base64 import b64encode, b64decode
 from typing import TypeVar, Any, Optional, Sequence, Dict
 from typing_extensions import Literal, Protocol, Final, TypeAlias
 
-try:
-    from passlib.context import CryptContext
-except ImportError as _exc:  # pragma: no cover
-    _passlib_import_exc: Optional[ImportError] = _exc
-else:
-    _passlib_import_exc = None
-
-__all__ = ['HashT', 'HashInterface', 'BuiltinHash', 'Cleartext', 'get_hash']
+__all__ = ['HashT', 'HashInterface', 'BuiltinHash', 'Cleartext']
 
 _Pbkdf2Hashes: TypeAlias = Literal['sha1', 'sha256', 'sha512']
 
 #: Type variable for a :class:`HashInterface`.
 HashT = TypeVar('HashT', bound='HashInterface')
 
 
@@ -194,46 +187,7 @@
         return secret
 
     def verify(self, secret: str, hash: str) -> bool:
         return secrets.compare_digest(secret, hash)
 
     def __repr__(self) -> str:
         return 'Cleartext()'
-
-
-def get_hash(*, passlib_config: Optional[str] = None) \
-        -> HashInterface:  # pragma: no cover
-    """Provide a secure, default :class:`HashInterface` implementation.
-
-    If *passlib_config* is given, a :class:`~passlib.context.CryptContext` is
-    loaded from it. Otherwise, the returned implementation depends on whether
-    :mod:`passlib` is available.
-
-    If :mod:`passlib` is available, a :class:`~passlib.context.CryptContext` is
-    created with a set of `active hashes
-    <https://passlib.readthedocs.io/en/stable/lib/passlib.hash.html#active-hashes>`_,
-    defaulting to ``pbkdf2_sha256`` for new digests.
-
-    If :mod:`passlib` is not available, a :class:`BuiltinHash` with default
-    settings is created. This is intended to be compatible with the
-    :mod:`passlib` default if it is installed later.
-
-    Args:
-        passlib_config: A passlib config file.
-
-    See Also:
-        :meth:`passlib.context.CryptContext.from_path`
-
-    """
-    context: HashInterface
-    if passlib_config is not None:
-        if _passlib_import_exc is not None:
-            raise _passlib_import_exc
-        context = CryptContext.from_path(passlib_config)
-    elif CryptContext is not None:
-        context = CryptContext(
-            schemes=['argon2', 'bcrypt_sha256', 'phpass', 'pbkdf2_sha1',
-                     'pbkdf2_sha256', 'pbkdf2_sha512', 'scram', 'scrypt'],
-            default='pbkdf2_sha256')
-    else:
-        context = BuiltinHash()
-    return context
```

### Comparing `pysasl-1.0.2/pysasl/identity.py` & `pysasl-1.1.0/pysasl/identity.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 
 import secrets
 from abc import abstractmethod
 from typing import Optional, Sequence
 from typing_extensions import Protocol, Self
 
 from .hashing import HashInterface, Cleartext
-from .prep import default_prep, Preparation
+from .prep import saslprep, Preparation
 
 __all__ = ['Identity', 'ClearIdentity', 'HashedIdentity']
 
 
 class Identity(Protocol):
     """Represents an server-side identity that credentials will be
     authenticated against.
 
     """
 
     __slots__: Sequence[str] = []
 
-    @property
     @abstractmethod
-    def authcid(self) -> str:
-        """The authentication identity, e.g. a login username."""
+    def compare_authcid(self, authcid: str) -> bool:
+        """Compare the identity's authcid with the given *authcid*.
+
+        Args:
+            authcid: The authentication identity string value.
+
+        """
         ...
 
     @abstractmethod
     def compare_secret(self, secret: str) -> bool:
         """Compare the identity's secret with the given *secret*. The
         comparison must account for things like hashing or token algorithms.
 
@@ -33,117 +37,123 @@
             secret: The authentication secret string value.
 
         """
         ...
 
     @abstractmethod
     def get_clear_secret(self) -> Optional[str]:
-        """Return the cleartext secret string if it is available. This value
-        has already been prepared with a :class:`~pysasl.prep.Preparation`
-        function.
-
-        """
+        """Return the cleartext secret string if it is available."""
         ...
 
 
 class ClearIdentity(Identity):
     """An :class:`Identity` that stores the secret string in cleartext.
 
     Args:
         authcid: The authentication identity, e.g. a login username.
-        secret: The cleartext secret string.
-        prepare: The preparation algorithm function.
+        secret: The authentication secret string value, e.g. a login password.
+        prepare: The string preparation function.
 
     """
 
-    __slots__: Sequence[str] = ['_authcid', '_secret', '_prepare']
+    __slots__ = ['_authcid', '_secret', '_prepare']
 
     def __init__(self, authcid: str, secret: str, *,
-                 prepare: Preparation = default_prep) -> None:
+                 prepare: Preparation = saslprep) -> None:
         super().__init__()
         self._authcid = authcid
-        self._secret = prepare(secret)
+        self._secret = secret
         self._prepare = prepare
 
-    @property
-    def authcid(self) -> str:
-        return self._authcid
+    def _compare(self, this: str, that: str) -> bool:
+        prepare = self._prepare
+        prepared_this = prepare(this).encode('utf-8')
+        prepared_that = prepare(that).encode('utf-8')
+        return secrets.compare_digest(prepared_this, prepared_that)
+
+    def compare_authcid(self, authcid: str) -> bool:
+        return self._compare(self._authcid, authcid)
 
     def compare_secret(self, secret: str) -> bool:
-        return secrets.compare_digest(self._secret, self._prepare(secret))
+        return self._compare(self._secret, secret)
 
     def get_clear_secret(self) -> str:
         """Return the cleartext secret string."""
         return self._secret
 
     def __repr__(self) -> str:
-        return f'ClearIdentity({self.authcid!r}, ...)'
+        return f'ClearIdentity({self._authcid!r}, ...)'
 
 
 class HashedIdentity(Identity):
     """An :class:`Identity` where the secret has been hashed for storage.
 
     Args:
         authcid: The authentication identity, e.g. a login username.
         digest: The hashed secret string, using :attr:`.hash`.
         hash: The hash algorithm to use to verify the secret.
-        prepare: The preparation algorithm function.
+        prepare: The string preparation function.
 
     """
 
-    __slots__: Sequence[str] = ['_authcid', '_digest', '_hash', '_prepare']
+    __slots__ = ['_authcid', '_digest', '_hash', '_prepare']
 
     def __init__(self, authcid: str, digest: str, *,
                  hash: HashInterface,
-                 prepare: Preparation = default_prep) -> None:
+                 prepare: Preparation = saslprep) -> None:
         super().__init__()
         self._authcid = authcid
         self._digest = digest
         self._hash = hash
         self._prepare = prepare
 
     @classmethod
     def create(cls, authcid: str, secret: str, *,
                hash: HashInterface,
-               prepare: Preparation = default_prep) -> Self:
+               prepare: Preparation = saslprep) -> Self:
         """Prepare and hash the given *secret*, returning a
         :class:`HashedIdentity`.
 
         Args:
             authcid: The authentication identity, e.g. a login username.
             secret: The cleartext secret string.
             hash: The hash algorithm to use to verify the secret.
-            prepare: The preparation algorithm function.
+            prepare: The string preparation function.
 
         """
         digest = hash.hash(prepare(secret))
         return cls(authcid, digest, hash=hash, prepare=prepare)
 
     @property
-    def authcid(self) -> str:
-        return self._authcid
-
-    @property
     def digest(self) -> str:
         """The hashed secret string, using :attr:`.hash`."""
         return self._digest
 
     @property
     def hash(self) -> HashInterface:
         """The hash implementation to use to verify the secret."""
         return self._hash
 
+    def _compare(self, this: str, that: str) -> bool:
+        prepare = self._prepare
+        prepared_this = prepare(this).encode('utf-8')
+        prepared_that = prepare(that).encode('utf-8')
+        return secrets.compare_digest(prepared_this, prepared_that)
+
+    def compare_authcid(self, authcid: str) -> bool:
+        return self._compare(self._authcid, authcid)
+
     def compare_secret(self, secret: str) -> bool:
         return self._hash.verify(self._prepare(secret), self._digest)
 
     def get_clear_secret(self) -> Optional[str]:
         """Return the cleartext secret string, only if :attr:`.hash` is
         :class:`~pysasl.hashing.Cleartext`.
 
         """
         if isinstance(self.hash, Cleartext):
             return self.digest
         else:
             return None
 
     def __repr__(self) -> str:
-        return f'HashedIdentity({self.authcid}, ..., hash={self._hash!r})'
+        return f'HashedIdentity({self._authcid}, ..., hash={self._hash!r})'
```

### Comparing `pysasl-1.0.2/pysasl/creds/__init__.py` & `pysasl-1.1.0/pysasl/creds/__init__.py`

 * *Files identical despite different names*

### Comparing `pysasl-1.0.2/pysasl/creds/client.py` & `pysasl-1.1.0/pysasl/creds/client.py`

 * *Files identical despite different names*

### Comparing `pysasl-1.0.2/pysasl/creds/external.py` & `pysasl-1.1.0/pysasl/creds/external.py`

 * *Files identical despite different names*

### Comparing `pysasl-1.0.2/pysasl/creds/plain.py` & `pysasl-1.1.0/pysasl/creds/plain.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,54 +1,46 @@
 
-import secrets
 from typing import Optional
 
 from .server import ServerCredentials
 from ..identity import Identity
-from ..prep import default_prep, Preparation
 
 __all__ = ['PlainCredentials']
 
 
 class PlainCredentials(ServerCredentials):
     """Implementation of :class:`~pysasl.creds.server.ServerCredentials` for
     typical SASL mechanisms like
     :class:`~pysasl.mechanism.plain.PlainMechanism` where the mechanism
     operates on the *secret* string in cleartext.
 
     Args:
         authcid: Authentication ID string (the username).
         secret: Secret string (the password).
         authzid: Authorization ID string, if provided.
-        prepare: The preparation algorithm function.
 
     """
 
-    __slots__ = ['_authcid', '_secret', '_authzid', '_prepare']
+    __slots__ = ['_authcid', '_secret', '_authzid']
 
-    def __init__(self, authcid: str, secret: str, authzid: str = '', *,
-                 prepare: Preparation = default_prep) -> None:
+    def __init__(self, authcid: str, secret: str, authzid: str = '') -> None:
         super().__init__()
         self._authcid = authcid
         self._secret = secret
-        self._authzid = authzid or prepare(authcid)
-        self._prepare = prepare
+        self._authzid = authzid or authcid
 
     @property
     def authcid(self) -> str:
         return self._authcid
 
     @property
     def authzid(self) -> str:
         return self._authzid
 
     def verify(self, identity: Optional[Identity]) -> bool:
         if identity is not None:
-            prepare = self._prepare
-            self_authcid = prepare(self.authcid)
-            other_authcid = prepare(identity.authcid)
-            return secrets.compare_digest(self_authcid, other_authcid)  \
+            return identity.compare_authcid(self.authcid)  \
                 and identity.compare_secret(self._secret)
         return False
 
     def __repr__(self) -> str:
         return f'PlainCredentials({self.authcid!r}, ..., {self.authzid!r})'
```

### Comparing `pysasl-1.0.2/pysasl/creds/server.py` & `pysasl-1.1.0/pysasl/creds/server.py`

 * *Files identical despite different names*

### Comparing `pysasl-1.0.2/pysasl/mechanism/__init__.py` & `pysasl-1.1.0/pysasl/mechanism/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 
 
 from abc import abstractmethod, ABCMeta
 from typing import Union, Optional, Tuple, Sequence
 from typing_extensions import TypeAlias
 
-from ..config import SASLConfig
 from ..creds.client import ClientCredentials
 from ..creds.server import ServerCredentials
 
 __all__ = ['Mechanism', 'ServerChallenge', 'ChallengeResponse',
            'ServerMechanism', 'ClientMechanism']
 
 #: A type alias for either server or client mechanisms.
@@ -67,36 +66,30 @@
 
     def __repr__(self) -> str:
         return f'ChallengeResponse({self.challenge!r}, {self.response!r})'
 
 
 class _BaseMechanism:
 
-    __slots__: Sequence[str] = ['_name', '_config']
+    __slots__: Sequence[str] = ['_name']
 
-    def __init__(self, name: Union[str, bytes], config: SASLConfig) -> None:
+    def __init__(self, name: Union[str, bytes]) -> None:
         super().__init__()
         if isinstance(name, str):
             name = name.encode('ascii')
         self._name = name
-        self._config = config
 
     @property
     def name(self) -> bytes:
         """The SASL name for this mechanism."""
         return self._name
 
-    @property
-    def config(self) -> SASLConfig:
-        """The configuration object."""
-        return self._config
-
     def __eq__(self, other: object) -> bool:
         if isinstance(other, _BaseMechanism):
-            return self.name == other.name and self.config == other.config
+            return self.name == other.name
         return NotImplemented
 
 
 class ServerMechanism(_BaseMechanism, metaclass=ABCMeta):
     """Base class for implementing SASL mechanisms that support server-side
     credential verification.
```

### Comparing `pysasl-1.0.2/pysasl/mechanism/crammd5.py` & `pysasl-1.1.0/pysasl/mechanism/crammd5.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,39 @@
 
 import re
 import hmac
 import hashlib
-import secrets
 import email.utils
 from typing import Union, Optional, Tuple, Sequence
 
 from . import (ServerMechanism, ClientMechanism, ServerChallenge,
                ChallengeResponse)
-from ..config import default_config, SASLConfig
 from ..creds.client import ClientCredentials
 from ..creds.server import ServerCredentials
 from ..exception import InvalidResponse, MechanismUnusable, UnexpectedChallenge
 from ..identity import Identity
+from ..prep import saslprep
 
 __all__ = ['CramMD5Result', 'CramMD5Mechanism']
 
 
 class CramMD5Result(ServerCredentials):
     """Because this mechanism uses hash algorithms to compare secrets, the
     :meth:`~CramMD5Mechanism.server_attempt` method returns this sub-class
     which overrides the :meth:`.verify` method.
 
     """
 
-    __slots__: Sequence[str] = ['_username', '_challenge', '_digest',
-                                '_config']
+    __slots__: Sequence[str] = ['_username', '_challenge', '_digest']
 
-    def __init__(self, username: str, challenge: bytes,
-                 digest: bytes, *, config: SASLConfig) -> None:
+    def __init__(self, username: str, challenge: bytes, digest: bytes) -> None:
         super().__init__()
         self._username = username
         self._challenge = challenge
         self._digest = digest
-        self._config = config
 
     @property
     def authcid(self) -> str:
         return self._username
 
     @property
     def authzid(self) -> str:
@@ -48,18 +44,15 @@
             return False
         clear_secret = identity.get_clear_secret()
         if clear_secret is None:
             raise MechanismUnusable('CRAM-MD5')
         secret_b = clear_secret.encode('utf-8')
         expected_hmac = hmac.new(secret_b, self._challenge, hashlib.md5)
         expected_digest = expected_hmac.hexdigest().encode('ascii')
-        prepare = self._config.prepare
-        self_authcid = prepare(self.authcid)
-        other_authcid = prepare(identity.authcid)
-        return secrets.compare_digest(self_authcid, other_authcid) \
+        return identity.compare_authcid(self.authcid) \
             and hmac.compare_digest(expected_digest, self._digest)
 
 
 class CramMD5Mechanism(ServerMechanism, ClientMechanism):
     """Implements the CRAM-MD5 authentication mechanism.
 
     Warning:
@@ -67,17 +60,16 @@
         dangerous, as it can have implications about how the credentials are
         stored server-side.
 
     """
 
     _pattern = re.compile(br'^(.*) ([^ ]+)$')
 
-    def __init__(self, name: Union[str, bytes] = b'CRAM-MD5',
-                 config: SASLConfig = default_config) -> None:
-        super().__init__(name, config)
+    def __init__(self, name: Union[str, bytes] = b'CRAM-MD5') -> None:
+        super().__init__(name)
 
     def server_attempt(self, responses: Sequence[ChallengeResponse]) \
             -> Tuple[CramMD5Result, None]:
         try:
             first = responses[0]
         except IndexError as exc:
             challenge = email.utils.make_msgid().encode('utf-8')
@@ -85,25 +77,23 @@
 
         match = re.match(self._pattern, first.response)
         if not match:
             raise InvalidResponse()
         username, digest = match.groups()
 
         username_str = username.decode('utf-8')
-        result = CramMD5Result(username_str, first.challenge, digest,
-                               config=self.config)
+        result = CramMD5Result(username_str, first.challenge, digest)
         return result, None
 
     def client_attempt(self, creds: ClientCredentials,
                        challenges: Sequence[ServerChallenge]) \
             -> ChallengeResponse:
         if len(challenges) < 1:
             return ChallengeResponse(b'', b'')
         elif len(challenges) > 1:
             raise UnexpectedChallenge()
         challenge = challenges[0].data
-        prepare = self.config.prepare
-        authcid = prepare(creds.authcid).encode('utf-8')
-        secret = prepare(creds.secret).encode('utf-8')
+        authcid = saslprep(creds.authcid).encode('utf-8')
+        secret = saslprep(creds.secret).encode('utf-8')
         digest = hmac.new(secret, challenge, hashlib.md5).hexdigest()
         response = b' '.join((authcid, digest.encode('ascii')))
         return ChallengeResponse(challenge, response)
```

### Comparing `pysasl-1.0.2/pysasl/mechanism/external.py` & `pysasl-1.1.0/pysasl/mechanism/external.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 
 from typing import Union, Tuple, Sequence
 
 from . import (ServerMechanism, ClientMechanism, ServerChallenge,
                ChallengeResponse)
-from ..config import default_config, SASLConfig
 from ..creds.client import ClientCredentials
 from ..creds.external import ExternalCredentials
 from ..exception import UnexpectedChallenge
 
 __all__ = ['ExternalMechanism']
 
 
@@ -15,17 +14,16 @@
     """Implements the EXTERNAL authentication mechanism.
 
     See Also:
         `RFC 4422 Appendix A <https://tools.ietf.org/html/rfc4422#appendix-A>`_
 
     """
 
-    def __init__(self, name: Union[str, bytes] = b'EXTERNAL',
-                 config: SASLConfig = default_config) -> None:
-        super().__init__(name, config)
+    def __init__(self, name: Union[str, bytes] = b'EXTERNAL') -> None:
+        super().__init__(name)
 
     def server_attempt(self, responses: Sequence[ChallengeResponse]) \
             -> Tuple[ExternalCredentials, None]:
         try:
             first = responses[0]
         except IndexError as exc:
             raise ServerChallenge(b'') from exc
```

### Comparing `pysasl-1.0.2/pysasl/mechanism/login.py` & `pysasl-1.1.0/pysasl/mechanism/login.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 
 from typing import Union, Tuple, Sequence
 
 from . import (ServerMechanism, ClientMechanism, ServerChallenge,
                ChallengeResponse)
-from ..config import default_config, SASLConfig
 from ..creds.client import ClientCredentials
 from ..creds.plain import PlainCredentials
 from ..exception import UnexpectedChallenge
 
 __all__ = ['LoginMechanism']
 
 
 class LoginMechanism(ServerMechanism, ClientMechanism):
     """Implements the LOGIN authentication mechanism."""
 
-    def __init__(self, name: Union[str, bytes] = b'LOGIN',
-                 config: SASLConfig = default_config) -> None:
-        super().__init__(name, config)
+    def __init__(self, name: Union[str, bytes] = b'LOGIN') -> None:
+        super().__init__(name)
 
     def server_attempt(self, responses: Sequence[ChallengeResponse]) \
             -> Tuple[PlainCredentials, None]:
         try:
             first = responses[0]
         except (IndexError, ValueError) as exc:
             raise ServerChallenge(b'Username:') from exc
```

### Comparing `pysasl-1.0.2/pysasl/mechanism/oauth.py` & `pysasl-1.1.0/pysasl/mechanism/oauth.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 
 import re
 from typing import Union, Tuple, Sequence
 
 from . import (ServerMechanism, ClientMechanism, ServerChallenge,
                ChallengeResponse)
-from ..config import default_config, SASLConfig
 from ..creds.client import ClientCredentials
 from ..creds.external import ExternalCredentials
 from ..exception import InvalidResponse, UnexpectedChallenge
 
 __all__ = ['OAuth2Mechanism']
 
 
@@ -20,17 +19,16 @@
     .. _OAuth 2.0: https://tools.ietf.org/html/rfc6749
 
     """
 
     _pattern = re.compile(br'^user=(.*?)\x01auth=[bB][eE][aA][rR][eE][rR] '
                           br'(.*?)\x01\x01$')
 
-    def __init__(self, name: Union[str, bytes] = b'XOAUTH2',
-                 config: SASLConfig = default_config) -> None:
-        super().__init__(name, config)
+    def __init__(self, name: Union[str, bytes] = b'XOAUTH2') -> None:
+        super().__init__(name)
 
     def server_attempt(self, responses: Sequence[ChallengeResponse]) \
             -> Tuple[ExternalCredentials, None]:
         try:
             first = responses[0]
         except IndexError as exc:
             raise ServerChallenge(b'') from exc
```

### Comparing `pysasl-1.0.2/pysasl/mechanism/plain.py` & `pysasl-1.1.0/pysasl/mechanism/plain.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 
 import re
 from typing import Union, Tuple, Sequence
 
 from . import (ServerMechanism, ClientMechanism, ServerChallenge,
                ChallengeResponse)
-from ..config import default_config, SASLConfig
 from ..creds.client import ClientCredentials
 from ..creds.plain import PlainCredentials
 from ..exception import InvalidResponse, UnexpectedChallenge
 
 __all__ = ['PlainMechanism']
 
 
 class PlainMechanism(ServerMechanism, ClientMechanism):
     """Implements the PLAIN authentication mechanism."""
 
     _pattern = re.compile(br'^([^\x00]*)\x00([^\x00]+)\x00([^\x00]*)$')
 
     __slots__: Sequence[str] = []
 
-    def __init__(self, name: Union[str, bytes] = b'PLAIN',
-                 config: SASLConfig = default_config) -> None:
-        super().__init__(name, config)
+    def __init__(self, name: Union[str, bytes] = b'PLAIN') -> None:
+        super().__init__(name)
 
     def server_attempt(self, responses: Sequence[ChallengeResponse]) \
             -> Tuple[PlainCredentials, None]:
         try:
             first = responses[0]
         except IndexError as exc:
             raise ServerChallenge(b'') from exc
```

### Comparing `pysasl-1.0.2/test/test_crammd5.py` & `pysasl-1.1.0/test/test_crammd5.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 import unittest
 import email.utils
 
 from unittest.mock import patch, Mock
 
 from pysasl import SASLAuth
-from pysasl.config import default_config
 from pysasl.creds.client import ClientCredentials
 from pysasl.exception import (InvalidResponse, MechanismUnusable,
                               UnexpectedChallenge)
 from pysasl.hashing import BuiltinHash
 from pysasl.identity import ClearIdentity, HashedIdentity
 from pysasl.mechanism import ServerChallenge, ChallengeResponse
 from pysasl.mechanism.crammd5 import CramMD5Result, CramMD5Mechanism
@@ -32,15 +31,15 @@
         self.assertEqual(self.mech, sasl.get_server(b'CRAM-MD5'))
         self.assertEqual(self.mech, sasl.get_client(b'CRAM-MD5'))
         sasl = SASLAuth([self.mech])
         self.assertEqual([self.mech], sasl.client_mechanisms)
         self.assertEqual([self.mech], sasl.server_mechanisms)
 
     def test_result_verify_impossible(self) -> None:
-        result = CramMD5Result('testuser', b'', b'', config=default_config)
+        result = CramMD5Result('testuser', b'', b'')
         identity = HashedIdentity('testuser', 'digest',
                                   hash=builtin_hash.copy())
         with self.assertRaises(MechanismUnusable):
             result.verify(identity)
 
     @patch.object(email.utils, 'make_msgid')
     def test_server_attempt_issues_challenge(
@@ -79,8 +78,8 @@
         self.assertEqual(b'', resp1.response)
         resp2 = self.mech.client_attempt(creds, [
             ServerChallenge(b'<abc123.1234@testhost>')])
         self.assertEqual(b'testuser 3a569c3950e95c490fd42f5d89e1ef67',
                          resp2.response)
         self.assertRaises(UnexpectedChallenge,
                           self.mech.client_attempt,
-                          creds, [ServerChallenge(b'')]*2)
+                          creds, [ServerChallenge(b'')] * 2)
```

### Comparing `pysasl-1.0.2/test/test_creds.py` & `pysasl-1.1.0/test/test_creds.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import base64
 import unittest
 
 from pysasl.creds.plain import PlainCredentials
 from pysasl.hashing import BuiltinHash, Cleartext
 from pysasl.identity import ClearIdentity, HashedIdentity
+from pysasl.prep import noprep
 
 builtin_hash = BuiltinHash(rounds=1000)
 
 b64_salt = 'bzstsT0hfnnXDUPTJqbkhQ=='
 password_sha1 = '$pbkdf2$1000$' + b64_salt + '$ZreCYDHwQD8P81LbstmBx15gBgo='
 password_sha256 = '$pbkdf2-sha256$1000$' + b64_salt + '$dWvL4bTpWfPobA2eti+k' \
     'CjUsF4sfwwiW58SE10p4Vh0='
@@ -23,19 +24,34 @@
     def test_hashed_builtin_good(self) -> None:
         creds = PlainCredentials('username', 'password')
         stored = HashedIdentity('username', password_sha256, hash=builtin_hash)
         self.assertEqual(password_sha256, stored.digest)
         self.assertTrue(creds.verify(stored))
         self.assertIsNone(stored.get_clear_secret())
 
+    def test_hashed_builtin_good_prepare(self) -> None:
+        creds = PlainCredentials('user\u00ADname', 'pass\u00ADword')
+        stored = HashedIdentity.create('us\u200Bername',
+                                       'pa\u200Bssword',
+                                       hash=builtin_hash)
+        self.assertTrue(creds.verify(stored))
+
     def test_hashed_builtin_invalid(self) -> None:
         creds = PlainCredentials('username', 'invalid')
         stored = HashedIdentity('username', password_sha256, hash=builtin_hash)
         self.assertFalse(creds.verify(stored))
 
+    def test_hashed_builtin_invalid_noprep(self) -> None:
+        creds = PlainCredentials('user\u00ADname', 'pass\u00ADword')
+        stored = HashedIdentity.create('us\u200Bername',
+                                       'pa\u200Bssword',
+                                       hash=builtin_hash,
+                                       prepare=noprep)
+        self.assertFalse(creds.verify(stored))
+
     def test_hashed_builtin_copy(self) -> None:
         creds = PlainCredentials('username', 'password')
         builtin_copy = builtin_hash.copy()
         stored = HashedIdentity.create('username', 'password',
                                        hash=builtin_copy)
         self.assertTrue(creds.verify(stored))
         builtin_copy = builtin_hash.copy()
@@ -70,19 +86,30 @@
                                 password_sha256.replace('pbkdf2-', '', 1))
 
     def test_cleartext_good(self) -> None:
         creds = PlainCredentials('username', 'password')
         stored = ClearIdentity('username', 'password')
         self.assertTrue(creds.verify(stored))
 
+    def test_cleartext_good_prepare(self) -> None:
+        creds = PlainCredentials('user\u00ADname', 'pass\u00ADword')
+        stored = ClearIdentity('us\u200Bername', 'pa\u200Bssword')
+        self.assertTrue(creds.verify(stored))
+
     def test_cleartext_invalid(self) -> None:
         creds = PlainCredentials('username', 'password')
         self.assertFalse(creds.verify(ClearIdentity('username', 'invalid')))
         self.assertFalse(creds.verify(ClearIdentity('invalid', 'password')))
 
+    def test_cleartext_invalid_noprep(self) -> None:
+        creds = PlainCredentials('user\u00ADname', 'pass\u00ADword')
+        stored = ClearIdentity('us\u200Bername', 'pa\u200Bssword',
+                               prepare=noprep)
+        self.assertFalse(creds.verify(stored))
+
     def test_cleartext_copy(self) -> None:
         creds = PlainCredentials('username', 'password')
         stored = HashedIdentity('username', 'password',
                                 hash=Cleartext())
         self.assertTrue(creds.verify(stored))
         stored = HashedIdentity('username', 'password',
                                 hash=stored.hash.copy())
```

### Comparing `pysasl-1.0.2/test/test_external.py` & `pysasl-1.1.0/test/test_external.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,8 +61,8 @@
         creds = ClientCredentials('', '', 'testzid')
         resp1 = self.mech.client_attempt(creds, [])
         self.assertEqual(b'testzid', resp1.response)
         resp2 = self.mech.client_attempt(creds, [ServerChallenge(b'')])
         self.assertEqual(b'testzid', resp2.response)
         self.assertRaises(UnexpectedChallenge,
                           self.mech.client_attempt,
-                          creds, [ServerChallenge(b'')]*2)
+                          creds, [ServerChallenge(b'')] * 2)
```

### Comparing `pysasl-1.0.2/test/test_login.py` & `pysasl-1.1.0/test/test_login.py`

 * *Files identical despite different names*

### Comparing `pysasl-1.0.2/test/test_oauth.py` & `pysasl-1.1.0/test/test_oauth.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         self.assertEqual(b'user=testuser\x01auth=Bearer testtoken\x01\x01',
                          resp1.response)
         resp2 = self.mech.client_attempt(creds, [ServerChallenge(b'')])
         self.assertEqual(b'user=testuser\x01auth=Bearer testtoken\x01\x01',
                          resp2.response)
         self.assertRaises(UnexpectedChallenge,
                           self.mech.client_attempt,
-                          creds, [ServerChallenge(b'')]*2)
+                          creds, [ServerChallenge(b'')] * 2)
 
     def test_client_attempt_error(self) -> None:
         creds = ClientCredentials('testuser', 'testtoken')
         resp1 = self.mech.client_attempt(creds, [])
         self.assertEqual(b'user=testuser\x01auth=Bearer testtoken\x01\x01',
                          resp1.response)
         resp2 = self.mech.client_attempt(creds, [
```

### Comparing `pysasl-1.0.2/test/test_plain.py` & `pysasl-1.1.0/test/test_plain.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,8 +56,8 @@
         creds = ClientCredentials('testuser', 'testpass', 'testzid')
         resp1 = self.mech.client_attempt(creds, [])
         self.assertEqual(b'testzid\x00testuser\x00testpass', resp1.response)
         resp2 = self.mech.client_attempt(creds, [ServerChallenge(b'')])
         self.assertEqual(b'testzid\x00testuser\x00testpass', resp2.response)
         self.assertRaises(UnexpectedChallenge,
                           self.mech.client_attempt,
-                          creds, [ServerChallenge(b'')]*2)
+                          creds, [ServerChallenge(b'')] * 2)
```

### Comparing `pysasl-1.0.2/.gitignore` & `pysasl-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pysasl-1.0.2/LICENSE.md` & `pysasl-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pysasl-1.0.2/README.md` & `pysasl-1.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 `CRAM-MD5`, `EXTERNAL`, and `XOAUTH2` mechanisms are also available for special
 circumstances.
 
 There are currently no plans to implement
 [security layer](https://datatracker.ietf.org/doc/html/rfc4422#section-3.7)
 negotiation support.
 
-[![build](https://github.com/icgood/pysasl/actions/workflows/python-package.yml/badge.svg)](https://github.com/icgood/pysasl/actions/workflows/python-package.yml)
-[![Coverage Status](https://coveralls.io/repos/icgood/pysasl/badge.svg?branch=main)](https://coveralls.io/r/icgood/pysasl?branch=main)
+[![build](https://github.com/icgood/pysasl/actions/workflows/python-check.yml/badge.svg)](https://github.com/icgood/pysasl/actions/workflows/python-check.yml)
 [![PyPI](https://img.shields.io/pypi/v/pysasl.svg)](https://pypi.python.org/pypi/pysasl)
 [![PyPI](https://img.shields.io/pypi/pyversions/pysasl.svg)](https://pypi.python.org/pypi/pysasl)
+![platforms](https://img.shields.io/badge/platform-linux%20%7C%20macOS%20%7C%20windows-blueviolet)
 [![PyPI](https://img.shields.io/pypi/l/pysasl.svg)](https://pypi.python.org/pypi/pysasl)
 
 #### [API Documentation](https://icgood.github.io/pysasl/)
 
 Installation
 ============
```

### Comparing `pysasl-1.0.2/pyproject.toml` & `pysasl-1.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -46,17 +46,14 @@
     'Programming Language :: Python :: 3.11',
 ]
 dependencies = [
     'typing-extensions',
     'importlib-metadata; python_version < "3.10"',
 ]
 
-[project.optional-dependencies]
-hashing = ['passlib']
-
 [project.urls]
 'Homepage' = 'https://github.com/icgood/pysasl/'
 'API Documentation' = 'https://icgood.github.io/pysasl/'
 
 [project.entry-points.'pysasl.mechanism']
 CRAM-MD5 = 'pysasl.mechanism.crammd5:CramMD5Mechanism'
 EXTERNAL = 'pysasl.mechanism.external:ExternalMechanism'
@@ -77,16 +74,24 @@
 strict = true
 files = ['pysasl', 'test']
 
 [[tool.mypy.overrides]]
 module = 'importlib_metadata.*'
 ignore_missing_imports = true
 
-[tool.bandit]
-skips = ['B101']
+[tool.ruff]
+select = ['ANN', 'B', 'E', 'F', 'N', 'S', 'W']
+ignore = ['ANN101', 'ANN102', 'ANN401', 'N818', 'S101']
+line-length = 79
+
+[tool.ruff.per-file-ignores]
+"test/*" = ['ANN', 'S104']
+
+[tool.autopep8]
+aggressive = 1
 
 [tool.pytest.ini_options]
 testpaths = 'test'
 norecursedirs = 'doc'
 
 [tool.coverage.report]
 fail_under = 100
@@ -99,29 +104,26 @@
 
 [tool.hatch.envs.default]
 dependencies = [
     'mypy',
     'pyright',
     'pytest',
     'pytest-cov',
-    'flake8',
-    'flake8-annotations',
-    'flake8-bugbear',
-    'bandit[toml]',
-    'types-passlib',
+    'ruff',
+    'pycodestyle',
+    'autopep8',
 ]
-features = ['hashing']
 
 [tool.hatch.envs.default.scripts]
 run-pytest = 'py.test --cov-report=term-missing --cov=pysasl'
 run-mypy = 'mypy pysasl test'
 run-pyright = 'pyright pysasl test'
-run-flake8 = 'flake8 pysasl test'
-run-bandit = 'bandit -c pyproject.toml -qr pysasl'
-check = ['run-pytest', 'run-mypy', 'run-pyright', 'run-flake8', 'run-bandit']
+run-ruff = 'ruff pysasl test'
+run-autopep8 = 'autopep8 --exit-code -dr pysasl test'
+check = ['run-pytest', 'run-autopep8', 'run-mypy', 'run-pyright', 'run-ruff']
 
 [[tool.hatch.envs.all.matrix]]
 python = ['3.7', '3.8', '3.9', '3.10', '3.11']
 
 [tool.hatch.envs.doc]
 dependencies = [
     'sphinx',
```

### Comparing `pysasl-1.0.2/PKG-INFO` & `pysasl-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysasl
-Version: 1.0.2
+Version: 1.1.0
 Summary: Pure Python SASL client and server library.
 Project-URL: Homepage, https://github.com/icgood/pysasl/
 Project-URL: API Documentation, https://icgood.github.io/pysasl/
 Author-email: Ian Good <ian@icgood.net>
 License: ## The MIT License (MIT)
         
         Copyright (c) 2022 Ian Good
@@ -37,16 +37,14 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: ~=3.7
 Requires-Dist: importlib-metadata; python_version < '3.10'
 Requires-Dist: typing-extensions
-Provides-Extra: hashing
-Requires-Dist: passlib; extra == 'hashing'
 Description-Content-Type: text/markdown
 
 pysasl
 ======
 
 Pure Python SASL client and server library. The design of the library is
 intended to be agnostic of the protocol or network library.
@@ -55,18 +53,18 @@
 `CRAM-MD5`, `EXTERNAL`, and `XOAUTH2` mechanisms are also available for special
 circumstances.
 
 There are currently no plans to implement
 [security layer](https://datatracker.ietf.org/doc/html/rfc4422#section-3.7)
 negotiation support.
 
-[![build](https://github.com/icgood/pysasl/actions/workflows/python-package.yml/badge.svg)](https://github.com/icgood/pysasl/actions/workflows/python-package.yml)
-[![Coverage Status](https://coveralls.io/repos/icgood/pysasl/badge.svg?branch=main)](https://coveralls.io/r/icgood/pysasl?branch=main)
+[![build](https://github.com/icgood/pysasl/actions/workflows/python-check.yml/badge.svg)](https://github.com/icgood/pysasl/actions/workflows/python-check.yml)
 [![PyPI](https://img.shields.io/pypi/v/pysasl.svg)](https://pypi.python.org/pypi/pysasl)
 [![PyPI](https://img.shields.io/pypi/pyversions/pysasl.svg)](https://pypi.python.org/pypi/pysasl)
+![platforms](https://img.shields.io/badge/platform-linux%20%7C%20macOS%20%7C%20windows-blueviolet)
 [![PyPI](https://img.shields.io/pypi/l/pysasl.svg)](https://pypi.python.org/pypi/pysasl)
 
 #### [API Documentation](https://icgood.github.io/pysasl/)
 
 Installation
 ============
```

