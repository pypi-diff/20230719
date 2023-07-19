# Comparing `tmp/bk-crypto-python-sdk-1.0.2.tar.gz` & `tmp/bk-crypto-python-sdk-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bk-crypto-python-sdk-1.0.2.tar", max compression
+gzip compressed data, was "bk-crypto-python-sdk-1.0.3.tar", max compression
```

## Comparing `bk-crypto-python-sdk-1.0.2.tar` & `bk-crypto-python-sdk-1.0.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1068 2023-07-11 12:33:30.719032 bk-crypto-python-sdk-1.0.2/LICENSE.txt
--rw-r--r--   0        0        0      757 2023-07-11 12:33:30.719032 bk-crypto-python-sdk-1.0.2/bkcrypto/__init__.py
--rw-r--r--   0        0        0      757 2023-07-11 12:33:30.719032 bk-crypto-python-sdk-1.0.2/bkcrypto/asymmetric/__init__.py
--rw-r--r--   0        0        0      953 2023-07-11 12:33:30.719032 bk-crypto-python-sdk-1.0.2/bkcrypto/asymmetric/ciphers/__init__.py
--rw-r--r--   0        0        0     9481 2023-07-11 12:33:30.719032 bk-crypto-python-sdk-1.0.2/bkcrypto/asymmetric/ciphers/base.py
--rw-r--r--   0        0        0     5426 2023-07-11 12:33:30.719032 bk-crypto-python-sdk-1.0.2/bkcrypto/asymmetric/ciphers/rsa.py
--rw-r--r--   0        0        0     4464 2023-07-11 12:33:30.719032 bk-crypto-python-sdk-1.0.2/bkcrypto/asymmetric/ciphers/sm2.py
--rw-r--r--   0        0        0     2543 2023-07-11 12:33:30.719032 bk-crypto-python-sdk-1.0.2/bkcrypto/asymmetric/configs.py
--rw-r--r--   0        0        0     1240 2023-07-11 12:33:30.719032 bk-crypto-python-sdk-1.0.2/bkcrypto/asymmetric/interceptors.py
--rw-r--r--   0        0        0     1114 2023-07-11 12:33:30.719032 bk-crypto-python-sdk-1.0.2/bkcrypto/asymmetric/options.py
--rw-r--r--   0        0        0     2324 2023-07-11 12:33:30.719032 bk-crypto-python-sdk-1.0.2/bkcrypto/constants.py
--rw-r--r--   0        0        0      757 2023-07-11 12:33:30.719032 bk-crypto-python-sdk-1.0.2/bkcrypto/contrib/__init__.py
--rw-r--r--   0        0        0      757 2023-07-11 12:33:30.719032 bk-crypto-python-sdk-1.0.2/bkcrypto/contrib/django/__init__.py
--rw-r--r--   0        0        0     3747 2023-07-11 12:33:30.719032 bk-crypto-python-sdk-1.0.2/bkcrypto/contrib/django/ciphers.py
--rw-r--r--   0        0        0     4856 2023-07-11 12:33:30.719032 bk-crypto-python-sdk-1.0.2/bkcrypto/contrib/django/fields.py
--rw-r--r--   0        0        0     2154 2023-07-11 12:33:30.719032 bk-crypto-python-sdk-1.0.2/bkcrypto/contrib/django/init_configs.py
--rw-r--r--   0        0        0     6493 2023-07-11 12:33:30.719032 bk-crypto-python-sdk-1.0.2/bkcrypto/contrib/django/settings.py
--rw-r--r--   0        0        0      757 2023-07-11 12:33:30.719032 bk-crypto-python-sdk-1.0.2/bkcrypto/contrib/drf/__init__.py
--rw-r--r--   0        0        0      757 2023-07-11 12:33:30.719032 bk-crypto-python-sdk-1.0.2/bkcrypto/symmetric/__init__.py
--rw-r--r--   0        0        0      947 2023-07-11 12:33:30.719032 bk-crypto-python-sdk-1.0.2/bkcrypto/symmetric/ciphers/__init__.py
--rw-r--r--   0        0        0     3461 2023-07-11 12:33:30.719032 bk-crypto-python-sdk-1.0.2/bkcrypto/symmetric/ciphers/aes.py
--rw-r--r--   0        0        0    11066 2023-07-11 12:33:30.719032 bk-crypto-python-sdk-1.0.2/bkcrypto/symmetric/ciphers/base.py
--rw-r--r--   0        0        0     4158 2023-07-11 12:33:30.719032 bk-crypto-python-sdk-1.0.2/bkcrypto/symmetric/ciphers/sm4.py
--rw-r--r--   0        0        0     3041 2023-07-11 12:33:30.723032 bk-crypto-python-sdk-1.0.2/bkcrypto/symmetric/configs.py
--rw-r--r--   0        0        0      881 2023-07-11 12:33:30.723032 bk-crypto-python-sdk-1.0.2/bkcrypto/symmetric/interceptors.py
--rw-r--r--   0        0        0     1106 2023-07-11 12:33:30.723032 bk-crypto-python-sdk-1.0.2/bkcrypto/symmetric/options.py
--rw-r--r--   0        0        0     1866 2023-07-11 12:33:30.723032 bk-crypto-python-sdk-1.0.2/bkcrypto/types.py
--rw-r--r--   0        0        0      757 2023-07-11 12:33:30.723032 bk-crypto-python-sdk-1.0.2/bkcrypto/utils/__init__.py
--rw-r--r--   0        0        0     1203 2023-07-11 12:33:30.723032 bk-crypto-python-sdk-1.0.2/bkcrypto/utils/base_interceptors.py
--rw-r--r--   0        0        0     2024 2023-07-11 12:33:30.723032 bk-crypto-python-sdk-1.0.2/bkcrypto/utils/convertors.py
--rw-r--r--   0        0        0     1539 2023-07-11 12:33:30.723032 bk-crypto-python-sdk-1.0.2/bkcrypto/utils/module_loding.py
--rw-r--r--   0        0        0     1756 2023-07-11 12:33:30.723032 bk-crypto-python-sdk-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     6019 2023-07-11 12:33:30.723032 bk-crypto-python-sdk-1.0.2/readme.md
--rw-r--r--   0        0        0     7215 1970-01-01 00:00:00.000000 bk-crypto-python-sdk-1.0.2/setup.py
--rw-r--r--   0        0        0     6800 1970-01-01 00:00:00.000000 bk-crypto-python-sdk-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-19 13:04:29.951151 bk-crypto-python-sdk-1.0.3/LICENSE.txt
+-rw-r--r--   0        0        0      757 2023-07-19 13:04:29.951151 bk-crypto-python-sdk-1.0.3/bkcrypto/__init__.py
+-rw-r--r--   0        0        0      757 2023-07-19 13:04:29.951151 bk-crypto-python-sdk-1.0.3/bkcrypto/asymmetric/__init__.py
+-rw-r--r--   0        0        0      953 2023-07-19 13:04:29.951151 bk-crypto-python-sdk-1.0.3/bkcrypto/asymmetric/ciphers/__init__.py
+-rw-r--r--   0        0        0     9481 2023-07-19 13:04:29.951151 bk-crypto-python-sdk-1.0.3/bkcrypto/asymmetric/ciphers/base.py
+-rw-r--r--   0        0        0     5426 2023-07-19 13:04:29.951151 bk-crypto-python-sdk-1.0.3/bkcrypto/asymmetric/ciphers/rsa.py
+-rw-r--r--   0        0        0     4464 2023-07-19 13:04:29.951151 bk-crypto-python-sdk-1.0.3/bkcrypto/asymmetric/ciphers/sm2.py
+-rw-r--r--   0        0        0     2543 2023-07-19 13:04:29.951151 bk-crypto-python-sdk-1.0.3/bkcrypto/asymmetric/configs.py
+-rw-r--r--   0        0        0     1240 2023-07-19 13:04:29.951151 bk-crypto-python-sdk-1.0.3/bkcrypto/asymmetric/interceptors.py
+-rw-r--r--   0        0        0     1114 2023-07-19 13:04:29.951151 bk-crypto-python-sdk-1.0.3/bkcrypto/asymmetric/options.py
+-rw-r--r--   0        0        0     2324 2023-07-19 13:04:29.955151 bk-crypto-python-sdk-1.0.3/bkcrypto/constants.py
+-rw-r--r--   0        0        0      757 2023-07-19 13:04:29.955151 bk-crypto-python-sdk-1.0.3/bkcrypto/contrib/__init__.py
+-rw-r--r--   0        0        0      757 2023-07-19 13:04:29.955151 bk-crypto-python-sdk-1.0.3/bkcrypto/contrib/django/__init__.py
+-rw-r--r--   0        0        0     4791 2023-07-19 13:04:29.955151 bk-crypto-python-sdk-1.0.3/bkcrypto/contrib/django/ciphers.py
+-rw-r--r--   0        0        0     4856 2023-07-19 13:04:29.955151 bk-crypto-python-sdk-1.0.3/bkcrypto/contrib/django/fields.py
+-rw-r--r--   0        0        0     2680 2023-07-19 13:04:29.955151 bk-crypto-python-sdk-1.0.3/bkcrypto/contrib/django/init_configs.py
+-rw-r--r--   0        0        0     7422 2023-07-19 13:04:29.955151 bk-crypto-python-sdk-1.0.3/bkcrypto/contrib/django/settings.py
+-rw-r--r--   0        0        0      757 2023-07-19 13:04:29.955151 bk-crypto-python-sdk-1.0.3/bkcrypto/contrib/drf/__init__.py
+-rw-r--r--   0        0        0      757 2023-07-19 13:04:29.955151 bk-crypto-python-sdk-1.0.3/bkcrypto/symmetric/__init__.py
+-rw-r--r--   0        0        0      947 2023-07-19 13:04:29.955151 bk-crypto-python-sdk-1.0.3/bkcrypto/symmetric/ciphers/__init__.py
+-rw-r--r--   0        0        0     3461 2023-07-19 13:04:29.955151 bk-crypto-python-sdk-1.0.3/bkcrypto/symmetric/ciphers/aes.py
+-rw-r--r--   0        0        0    11066 2023-07-19 13:04:29.955151 bk-crypto-python-sdk-1.0.3/bkcrypto/symmetric/ciphers/base.py
+-rw-r--r--   0        0        0     4158 2023-07-19 13:04:29.955151 bk-crypto-python-sdk-1.0.3/bkcrypto/symmetric/ciphers/sm4.py
+-rw-r--r--   0        0        0     3041 2023-07-19 13:04:29.955151 bk-crypto-python-sdk-1.0.3/bkcrypto/symmetric/configs.py
+-rw-r--r--   0        0        0      881 2023-07-19 13:04:29.955151 bk-crypto-python-sdk-1.0.3/bkcrypto/symmetric/interceptors.py
+-rw-r--r--   0        0        0     1106 2023-07-19 13:04:29.955151 bk-crypto-python-sdk-1.0.3/bkcrypto/symmetric/options.py
+-rw-r--r--   0        0        0     1866 2023-07-19 13:04:29.955151 bk-crypto-python-sdk-1.0.3/bkcrypto/types.py
+-rw-r--r--   0        0        0      757 2023-07-19 13:04:29.955151 bk-crypto-python-sdk-1.0.3/bkcrypto/utils/__init__.py
+-rw-r--r--   0        0        0     1203 2023-07-19 13:04:29.955151 bk-crypto-python-sdk-1.0.3/bkcrypto/utils/base_interceptors.py
+-rw-r--r--   0        0        0     2024 2023-07-19 13:04:29.955151 bk-crypto-python-sdk-1.0.3/bkcrypto/utils/convertors.py
+-rw-r--r--   0        0        0     1539 2023-07-19 13:04:29.955151 bk-crypto-python-sdk-1.0.3/bkcrypto/utils/module_loding.py
+-rw-r--r--   0        0        0     1756 2023-07-19 13:04:29.955151 bk-crypto-python-sdk-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     7505 2023-07-19 13:04:29.955151 bk-crypto-python-sdk-1.0.3/readme.md
+-rw-r--r--   0        0        0     8741 1970-01-01 00:00:00.000000 bk-crypto-python-sdk-1.0.3/setup.py
+-rw-r--r--   0        0        0     8286 1970-01-01 00:00:00.000000 bk-crypto-python-sdk-1.0.3/PKG-INFO
```

### Comparing `bk-crypto-python-sdk-1.0.2/LICENSE.txt` & `bk-crypto-python-sdk-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bk-crypto-python-sdk-1.0.2/bkcrypto/__init__.py` & `bk-crypto-python-sdk-1.0.3/bkcrypto/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-crypto-python-sdk-1.0.2/bkcrypto/asymmetric/__init__.py` & `bk-crypto-python-sdk-1.0.3/bkcrypto/asymmetric/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-crypto-python-sdk-1.0.2/bkcrypto/asymmetric/ciphers/__init__.py` & `bk-crypto-python-sdk-1.0.3/bkcrypto/asymmetric/ciphers/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-crypto-python-sdk-1.0.2/bkcrypto/asymmetric/ciphers/base.py` & `bk-crypto-python-sdk-1.0.3/bkcrypto/asymmetric/ciphers/base.py`

 * *Files identical despite different names*

### Comparing `bk-crypto-python-sdk-1.0.2/bkcrypto/asymmetric/ciphers/rsa.py` & `bk-crypto-python-sdk-1.0.3/bkcrypto/asymmetric/ciphers/rsa.py`

 * *Files identical despite different names*

### Comparing `bk-crypto-python-sdk-1.0.2/bkcrypto/asymmetric/ciphers/sm2.py` & `bk-crypto-python-sdk-1.0.3/bkcrypto/asymmetric/ciphers/sm2.py`

 * *Files identical despite different names*

### Comparing `bk-crypto-python-sdk-1.0.2/bkcrypto/asymmetric/configs.py` & `bk-crypto-python-sdk-1.0.3/bkcrypto/asymmetric/configs.py`

 * *Files identical despite different names*

### Comparing `bk-crypto-python-sdk-1.0.2/bkcrypto/asymmetric/interceptors.py` & `bk-crypto-python-sdk-1.0.3/bkcrypto/asymmetric/interceptors.py`

 * *Files identical despite different names*

### Comparing `bk-crypto-python-sdk-1.0.2/bkcrypto/asymmetric/options.py` & `bk-crypto-python-sdk-1.0.3/bkcrypto/asymmetric/options.py`

 * *Files identical despite different names*

### Comparing `bk-crypto-python-sdk-1.0.2/bkcrypto/constants.py` & `bk-crypto-python-sdk-1.0.3/bkcrypto/constants.py`

 * *Files identical despite different names*

### Comparing `bk-crypto-python-sdk-1.0.2/bkcrypto/contrib/__init__.py` & `bk-crypto-python-sdk-1.0.3/bkcrypto/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-crypto-python-sdk-1.0.2/bkcrypto/contrib/django/__init__.py` & `bk-crypto-python-sdk-1.0.3/bkcrypto/contrib/django/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-crypto-python-sdk-1.0.2/bkcrypto/contrib/django/ciphers.py` & `bk-crypto-python-sdk-1.0.3/bkcrypto/contrib/django/ciphers.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from dataclasses import asdict
 
 from bkcrypto.asymmetric.ciphers import BaseAsymmetricCipher
 from bkcrypto.asymmetric.options import AsymmetricOptions
 from bkcrypto.symmetric.ciphers import BaseSymmetricCipher
 from bkcrypto.symmetric.options import SymmetricOptions
 
-from .init_configs import SymmetricCipherInitConfig
+from .init_configs import AsymmetricCipherInitConfig, SymmetricCipherInitConfig
 from .settings import crypto_settings
 
 
 def get_asymmetric_cipher(
     cipher_type: typing.Optional[str] = None,
     common: typing.Optional[typing.Dict[str, typing.Any]] = None,
     cipher_options: typing.Optional[typing.Dict[str, typing.Optional[AsymmetricOptions]]] = None,
@@ -76,8 +76,36 @@
 
         init_config: SymmetricCipherInitConfig = crypto_settings.SYMMETRIC_CIPHERS[using]
         cipher: BaseSymmetricCipher = get_symmetric_cipher(**init_config.as_get_cipher_params(cipher_type))
         self._cache[cache_key] = cipher
         return cipher
 
 
+class AsymmetricCipherManager:
+    _cache: typing.Optional[typing.Dict[str, BaseAsymmetricCipher]] = None
+
+    def __init__(self):
+        self._cache: [str, BaseAsymmetricCipher] = {}
+
+    def cipher(
+        self, using: typing.Optional[str] = None, cipher_type: typing.Optional[str] = None
+    ) -> BaseAsymmetricCipher:
+
+        using: str = using or "default"
+        if using not in crypto_settings.ASYMMETRIC_CIPHERS:
+            raise RuntimeError(f"Invalid using {using}")
+
+        cipher_type: str = cipher_type or crypto_settings.ASYMMETRIC_CIPHER_TYPE
+        cache_key: str = f"{using}-{cipher_type}"
+        if cache_key in self._cache:
+            return self._cache[cache_key]
+
+        init_config: AsymmetricCipherInitConfig = crypto_settings.ASYMMETRIC_CIPHERS[using]
+        cipher: BaseAsymmetricCipher = get_asymmetric_cipher(**init_config.as_get_cipher_params(cipher_type))
+        self._cache[cache_key] = cipher
+        return cipher
+
+
 symmetric_cipher_manager = SymmetricCipherManager()
+
+
+asymmetric_cipher_manager = AsymmetricCipherManager()
```

### Comparing `bk-crypto-python-sdk-1.0.2/bkcrypto/contrib/django/fields.py` & `bk-crypto-python-sdk-1.0.3/bkcrypto/contrib/django/fields.py`

 * *Files identical despite different names*

### Comparing `bk-crypto-python-sdk-1.0.2/bkcrypto/contrib/django/init_configs.py` & `bk-crypto-python-sdk-1.0.3/bkcrypto/contrib/django/init_configs.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,39 +10,52 @@
 specific language governing permissions and limitations under the License.
 """
 
 
 import typing
 from dataclasses import asdict, dataclass
 
-from bkcrypto.symmetric.configs import KeyConfig
+from bkcrypto.asymmetric.configs import KeyConfig as AsymmetricKeyConfig
+from bkcrypto.asymmetric.options import AsymmetricOptions
+from bkcrypto.symmetric.configs import KeyConfig as SymmetricKeyConfig
 from bkcrypto.symmetric.options import SymmetricOptions
 from bkcrypto.utils.module_loding import import_string
 
 
 @dataclass
-class SymmetricCipherInitConfig:
-    get_key_config: typing.Optional[str] = None
+class CipherInitConfig:
     # 默认取值 f"{cipher_type}_str:::"
     db_prefix_map: typing.Dict[str, str] = None
     prefix_cipher_type_map: typing.Dict[str, str] = None
-    get_key_config_func: typing.Optional[typing.Callable[[str], KeyConfig]] = None
+    get_key_config: typing.Optional[str] = None
+    get_key_config_func: typing.Optional[
+        typing.Callable[[str], typing.Union[AsymmetricKeyConfig, SymmetricKeyConfig]]
+    ] = None
     common: typing.Optional[typing.Dict[str, typing.Any]] = None
-    cipher_options: typing.Optional[typing.Dict[str, typing.Optional[SymmetricOptions]]] = None
+    cipher_options: typing.Optional[typing.Dict[str, typing.Union[SymmetricOptions, AsymmetricOptions, None]]] = None
 
     def __post_init__(self):
-        self.db_prefix_map = self.db_prefix_map or {}
-
         if self.get_key_config:
             self.get_key_config_func = import_string(self.get_key_config)
+        self.db_prefix_map = self.db_prefix_map or {}
 
     def as_get_cipher_params(self, cipher_type: str):
         # get key hook 不为空，优先从此处取 key
         if self.get_key_config_func:
-            key_config: KeyConfig = self.get_key_config_func(cipher_type)
+            key_config = self.get_key_config_func(cipher_type)
             key_dict: typing.Dict = asdict(key_config)
         else:
             key_dict: typing.Dict = {}
 
         common = self.common or {}
         common.update(key_dict)
         return {"cipher_type": cipher_type, "common": common, "cipher_options": self.cipher_options}
+
+
+@dataclass
+class SymmetricCipherInitConfig(CipherInitConfig):
+    get_key_config_func: typing.Optional[typing.Callable[[str], SymmetricKeyConfig]] = None
+
+
+@dataclass
+class AsymmetricCipherInitConfig(CipherInitConfig):
+    get_key_config_func: typing.Optional[typing.Callable[[str], AsymmetricKeyConfig]] = None
```

### Comparing `bk-crypto-python-sdk-1.0.2/bkcrypto/contrib/django/settings.py` & `bk-crypto-python-sdk-1.0.3/bkcrypto/contrib/django/settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 from dacite import from_dict
 from django.conf import settings
 from django.test.signals import setting_changed
 
 from bkcrypto import constants
 from bkcrypto.asymmetric.ciphers import RSAAsymmetricCipher, SM2AsymmetricCipher
-from bkcrypto.contrib.django.init_configs import SymmetricCipherInitConfig
+from bkcrypto.contrib.django.init_configs import AsymmetricCipherInitConfig, CipherInitConfig, SymmetricCipherInitConfig
 from bkcrypto.symmetric.ciphers import AESSymmetricCipher, SM4SymmetricCipher
 from bkcrypto.utils import module_loding
 
 DEFAULTS = {
     "SYMMETRIC_CIPHER_TYPE": constants.SymmetricCipherType.AES.value,
     "ASYMMETRIC_CIPHER_TYPE": constants.AsymmetricCipherType.RSA.value,
     "SYMMETRIC_CIPHER_CLASSES": {
@@ -39,14 +39,25 @@
             # 前缀和 cipher type 必须一一对应，且不能有前缀匹配关系
             "db_prefix_map": {
                 constants.SymmetricCipherType.AES.value: f"{constants.SymmetricCipherType.AES.value.lower()}_str:::",
                 constants.SymmetricCipherType.SM4.value: f"{constants.SymmetricCipherType.SM4.value.lower()}_str:::",
             },
         },
     },
+    "ASYMMETRIC_CIPHERS": {
+        "default": {
+            # 可选，用于在 settings 没法直接获取 key 的情况
+            "get_key_config": None,
+            # 前缀和 cipher type 必须一一对应，且不能有前缀匹配关系
+            "db_prefix_map": {
+                constants.AsymmetricCipherType.RSA.value: f"{constants.AsymmetricCipherType.RSA.value.lower()}_str:::",
+                constants.AsymmetricCipherType.SM2.value: f"{constants.AsymmetricCipherType.SM2.value.lower()}_str:::",
+            },
+        },
+    },
 }
 
 IMPORT_STRINGS = []
 
 # List of settings that have been removed
 REMOVED_SETTINGS = []
 
@@ -103,28 +114,35 @@
 
         if attr in ["SYMMETRIC_CIPHER_CLASSES", "ASYMMETRIC_CIPHER_CLASSES"]:
             val = {
                 cipher_type: module_loding.import_string(cipher_import_path)
                 for cipher_type, cipher_import_path in val.items()
             }
 
-        if attr in ["SYMMETRIC_CIPHERS"]:
-            using__init_config_map: typing.Dict[str, SymmetricCipherInitConfig] = {}
+        if attr in ["SYMMETRIC_CIPHERS", "ASYMMETRIC_CIPHERS"]:
+            using__init_config_map: typing.Dict[str, CipherInitConfig] = {}
             for using, init_config_params in val.items():
                 prefix_cipher_type_map: typing.Dict[str, str] = {}
                 db_prefix_map: typing.Dict[str, str] = init_config_params.get("db_prefix_map") or {}
-                for cipher_type in self.SYMMETRIC_CIPHER_CLASSES.keys():
+                cipher_types: typing.List[str] = [
+                    self.SYMMETRIC_CIPHER_CLASSES.keys(),
+                    self.ASYMMETRIC_CIPHER_CLASSES.keys(),
+                ][attr == "ASYMMETRIC_CIPHERS"]
+                for cipher_type in cipher_types:
                     if cipher_type in db_prefix_map:
                         prefix_cipher_type_map[db_prefix_map[cipher_type]] = cipher_type
                         continue
                     db_prefix_map[cipher_type] = f"{cipher_type.lower()}_str:::"
                     prefix_cipher_type_map[f"{cipher_type.lower()}_str:::"] = cipher_type
                 init_config_params["db_prefix_map"] = db_prefix_map
                 init_config_params["prefix_cipher_type_map"] = prefix_cipher_type_map
-                using__init_config_map[using] = from_dict(SymmetricCipherInitConfig, init_config_params)
+                using__init_config_map[using] = from_dict(
+                    [SymmetricCipherInitConfig, AsymmetricCipherInitConfig][attr == "ASYMMETRIC_CIPHER_CLASSES"],
+                    init_config_params,
+                )
             val = using__init_config_map
 
         # Coerce import strings into classes
         if attr in self.import_strings:
             val = perform_import(val, attr)
 
         # Cache the result
```

### Comparing `bk-crypto-python-sdk-1.0.2/bkcrypto/contrib/drf/__init__.py` & `bk-crypto-python-sdk-1.0.3/bkcrypto/contrib/drf/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-crypto-python-sdk-1.0.2/bkcrypto/symmetric/__init__.py` & `bk-crypto-python-sdk-1.0.3/bkcrypto/symmetric/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-crypto-python-sdk-1.0.2/bkcrypto/symmetric/ciphers/__init__.py` & `bk-crypto-python-sdk-1.0.3/bkcrypto/symmetric/ciphers/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-crypto-python-sdk-1.0.2/bkcrypto/symmetric/ciphers/aes.py` & `bk-crypto-python-sdk-1.0.3/bkcrypto/symmetric/ciphers/aes.py`

 * *Files identical despite different names*

### Comparing `bk-crypto-python-sdk-1.0.2/bkcrypto/symmetric/ciphers/base.py` & `bk-crypto-python-sdk-1.0.3/bkcrypto/symmetric/ciphers/base.py`

 * *Files identical despite different names*

### Comparing `bk-crypto-python-sdk-1.0.2/bkcrypto/symmetric/ciphers/sm4.py` & `bk-crypto-python-sdk-1.0.3/bkcrypto/symmetric/ciphers/sm4.py`

 * *Files identical despite different names*

### Comparing `bk-crypto-python-sdk-1.0.2/bkcrypto/symmetric/configs.py` & `bk-crypto-python-sdk-1.0.3/bkcrypto/symmetric/configs.py`

 * *Files identical despite different names*

### Comparing `bk-crypto-python-sdk-1.0.2/bkcrypto/symmetric/interceptors.py` & `bk-crypto-python-sdk-1.0.3/bkcrypto/symmetric/interceptors.py`

 * *Files identical despite different names*

### Comparing `bk-crypto-python-sdk-1.0.2/bkcrypto/symmetric/options.py` & `bk-crypto-python-sdk-1.0.3/bkcrypto/symmetric/options.py`

 * *Files identical despite different names*

### Comparing `bk-crypto-python-sdk-1.0.2/bkcrypto/types.py` & `bk-crypto-python-sdk-1.0.3/bkcrypto/types.py`

 * *Files identical despite different names*

### Comparing `bk-crypto-python-sdk-1.0.2/bkcrypto/utils/__init__.py` & `bk-crypto-python-sdk-1.0.3/bkcrypto/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bk-crypto-python-sdk-1.0.2/bkcrypto/utils/base_interceptors.py` & `bk-crypto-python-sdk-1.0.3/bkcrypto/utils/base_interceptors.py`

 * *Files identical despite different names*

### Comparing `bk-crypto-python-sdk-1.0.2/bkcrypto/utils/convertors.py` & `bk-crypto-python-sdk-1.0.3/bkcrypto/utils/convertors.py`

 * *Files identical despite different names*

### Comparing `bk-crypto-python-sdk-1.0.2/bkcrypto/utils/module_loding.py` & `bk-crypto-python-sdk-1.0.3/bkcrypto/utils/module_loding.py`

 * *Files identical despite different names*

### Comparing `bk-crypto-python-sdk-1.0.2/pyproject.toml` & `bk-crypto-python-sdk-1.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bk-crypto-python-sdk"
-version = "1.0.2"
+version = "1.0.3"
 description = "bk-crypto-python-sdk is a lightweight cryptography toolkit for Python applications based on Cryptodome / tongsuopy and other encryption libraries."
 authors = ["TencentBlueKing <contactus_bk@tencent.com>"]
 readme = "readme.md"
 packages = [
     { include = "bkcrypto" },
 ]
```

### Comparing `bk-crypto-python-sdk-1.0.2/setup.py` & `bk-crypto-python-sdk-1.0.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,41 +1,199 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
-
-packages = \
-['bkcrypto',
- 'bkcrypto.asymmetric',
- 'bkcrypto.asymmetric.ciphers',
- 'bkcrypto.contrib',
- 'bkcrypto.contrib.django',
- 'bkcrypto.contrib.drf',
- 'bkcrypto.symmetric',
- 'bkcrypto.symmetric.ciphers',
- 'bkcrypto.utils']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['dacite>=1.8.1,<2.0.0',
- 'pycryptodomex>=3.18.0,<4.0.0',
- 'tongsuopy-crayon>=1.0.2b5,<2.0.0',
- 'wrapt>=1.15.0,<2.0.0']
-
-setup_kwargs = {
-    'name': 'bk-crypto-python-sdk',
-    'version': '1.0.2',
-    'description': 'bk-crypto-python-sdk is a lightweight cryptography toolkit for Python applications based on Cryptodome / tongsuopy and other encryption libraries.',
-    'long_description': '# BlueKing crypto-python-sdk\n\n---\n\n![Python](https://badgen.net/badge/python/%3E=3.6.2,%3C3.11/green?icon=github)\n![Django](https://badgen.net/badge/django/%3E=3.1.5,%3C=4.2.1/yellow?icon=github)\n[![License](https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat)](LICENSE.txt)\n\n![Release](https://badgen.net/github/release/TencentBlueKing/crypto-python-sdk)\n[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/TencentBlueKing/crypto-python-sdk/pulls)\n\n[![Publish to Pypi](https://github.com/TencentBlueKing/crypto-python-sdk/actions/workflows/release.yml/badge.svg)](https://github.com/TencentBlueKing/crypto-python-sdk/actions/workflows/release.yml)\n\n[(English Documents Available)](https://github.com/TencentBlueKing/crypto-python-sdk/blob/main/readme_en.md)\n\n## Overview\n\n️🔧 BlueKing crypto-python-sdk 是一个基于 pyCryptodome / tongsuopy 等加密库的轻量级密码学工具包，为 Python 应用统一的加解密实现，\n便于项目在不同的加密方式之间进行无侵入切换\n\n## Features\n\n* [Basic] 提供加密统一抽象层，对接 Cryptodome / tongsuopy 等加密库，提供统一的加解密实现\n* [Basic] 支持国际主流密码学算法：AES、RSA\n* [Basic] 支持中国商用密码学算法：SM2、SM4\n* [Basic] 非对称加密支持 CBC、CTR、GCM、CFB 作为块密码模式\n* [Contrib] Django Support，集成 Django settings、ModelField\n\n## Getting started\n\n### Installation\n\n```bash\n$ pip install bk-crypto-python-sdk\n```\n\n### Usage\n\n> 更多用法参考：[使用文档](https://github.com/TencentBlueKing/crypto-python-sdk/blob/main/docs/usage.md)\n\n在项目中配置\n\n```python\nimport os\nfrom bkcrypto import constants\nfrom bkcrypto.symmetric.options import AESSymmetricOptions, SM4SymmetricOptions\n\nBKCRYPTO = {\n    # 声明项目所使用的非对称加密算法\n    "ASYMMETRIC_CIPHER_TYPE": constants.AsymmetricCipherType.SM2.value,\n    # 声明项目所使用的对称加密算法\n    "SYMMETRIC_CIPHER_TYPE": constants.SymmetricCipherType.SM4.value,\n    "SYMMETRIC_CIPHERS": {\n        # default - 所配置的对称加密实例，根据项目需要可以配置多个\n        "default": {\n            # 可选，用于在 settings 没法直接获取 key 的情况\n            # "get_key_config": "apps.utils.encrypt.key.get_key_config",\n            # 可选，用于 ModelField，加密时携带该前缀入库，解密时分析该前缀并选择相应的解密算法\n            # ⚠️ 前缀和 cipher type 必须一一对应，且不能有前缀匹配关系\n            # "db_prefix_map": {\n            #     SymmetricCipherType.AES.value: "aes_str:::",\n            #     SymmetricCipherType.SM4.value: "sm4_str:::"\n            # },\n            # 公共参数配置，不同 cipher 初始化时共用这部分参数\n            "common": {"key": "your key"},\n            "cipher_options": {\n                constants.SymmetricCipherType.AES.value: AESSymmetricOptions(key_size=16),\n                # 蓝鲸推荐配置\n                constants.SymmetricCipherType.SM4.value: SM4SymmetricOptions(mode=constants.SymmetricMode.CTR)\n            }\n        },\n    }\n}\n```\n\n#### 非对称加密\n\n```python\nfrom bkcrypto.asymmetric.ciphers import BaseAsymmetricCipher\nfrom bkcrypto.contrib.django.ciphers import get_asymmetric_cipher\n\nasymmetric_cipher: BaseAsymmetricCipher = get_asymmetric_cipher()\n\n# 加解密\nassert "123" == asymmetric_cipher.decrypt(asymmetric_cipher.encrypt("123"))\n# 验签\nassert asymmetric_cipher.verify(plaintext="123", signature=asymmetric_cipher.sign("123"))\n```\n\n#### 对称加密\n\n```python\nfrom bkcrypto.symmetric.ciphers import BaseSymmetricCipher\nfrom bkcrypto.contrib.django.ciphers import symmetric_cipher_manager\n\n# using - 指定对称加密实例，默认使用 `default`\nsymmetric_cipher: BaseSymmetricCipher = symmetric_cipher_manager.cipher(using="default")\nassert "123" == symmetric_cipher.decrypt(symmetric_cipher.encrypt("123"))\n```\n\n#### SymmetricTextField\n\n```python\nfrom django.db import models\nfrom bkcrypto.contrib.django.fields import SymmetricTextField\n\n\nclass IdentityData(models.Model):\n    password = SymmetricTextField("密码", blank=True, null=True)\n```\n\n## Roadmap\n\n- [版本日志](https://github.com/TencentBlueKing/crypto-python-sdk/blob/main/release.md)\n\n## Support\n\n- [蓝鲸论坛](https://bk.tencent.com/s-mart/community)\n- [蓝鲸 DevOps 在线视频教程](https://bk.tencent.com/s-mart/video/)\n- [蓝鲸社区版交流群](https://jq.qq.com/?_wv=1027&k=5zk8F7G)\n\n## BlueKing Community\n\n- [BK-CMDB](https://github.com/Tencent/bk-cmdb)：蓝鲸配置平台（蓝鲸 CMDB）是一个面向资产及应用的企业级配置管理平台。\n- [BK-CI](https://github.com/Tencent/bk-ci)：蓝鲸持续集成平台是一个开源的持续集成和持续交付系统，可以轻松将你的研发流程呈现到你面前。\n- [BK-BCS](https://github.com/Tencent/bk-bcs)：蓝鲸容器管理平台是以容器技术为基础，为微服务业务提供编排管理的基础服务平台。\n- [BK-PaaS](https://github.com/Tencent/bk-paas)：蓝鲸 PaaS 平台是一个开放式的开发平台，让开发者可以方便快捷地创建、开发、部署和管理\n  SaaS 应用。\n- [BK-SOPS](https://github.com/Tencent/bk-sops)：标准运维（SOPS）是通过可视化的图形界面进行任务流程编排和执行的系统，是蓝鲸体系中一款轻量级的调度编排类\n  SaaS 产品。\n- [BK-JOB](https://github.com/Tencent/bk-job) 蓝鲸作业平台(Job)是一套运维脚本管理系统，具备海量任务并发处理能力。\n\n## Contributing\n\n如果你有好的意见或建议，欢迎给我们提 Issues 或 Pull Requests，为蓝鲸开源社区贡献力量。   \n[腾讯开源激励计划](https://opensource.tencent.com/contribution) 鼓励开发者的参与和贡献，期待你的加入。\n\n## License\n\n基于 MIT 协议， 详细请参考 [LICENSE](https://github.com/TencentBlueKing/crypto-python-sdk/blob/main/LICENSE.txt)\n',
-    'author': 'TencentBlueKing',
-    'author_email': 'contactus_bk@tencent.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.6.2,<3.11',
+Metadata-Version: 2.1
+Name: bk-crypto-python-sdk
+Version: 1.0.3
+Summary: bk-crypto-python-sdk is a lightweight cryptography toolkit for Python applications based on Cryptodome / tongsuopy and other encryption libraries.
+Author: TencentBlueKing
+Author-email: contactus_bk@tencent.com
+Requires-Python: >=3.6.2,<3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Dist: dacite (>=1.8.1,<2.0.0)
+Requires-Dist: pycryptodomex (>=3.18.0,<4.0.0)
+Requires-Dist: tongsuopy-crayon (>=1.0.2b5,<2.0.0)
+Requires-Dist: wrapt (>=1.15.0,<2.0.0)
+Description-Content-Type: text/markdown
+
+# BlueKing crypto-python-sdk
+
+---
+
+![Python](https://badgen.net/badge/python/%3E=3.6.2,%3C3.11/green?icon=github)
+![Django](https://badgen.net/badge/django/%3E=3.1.5,%3C=4.2.1/yellow?icon=github)
+[![License](https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat)](LICENSE.txt)
+
+![Release](https://badgen.net/github/release/TencentBlueKing/crypto-python-sdk)
+[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/TencentBlueKing/crypto-python-sdk/pulls)
+
+[![Publish to Pypi](https://github.com/TencentBlueKing/crypto-python-sdk/actions/workflows/release.yml/badge.svg)](https://github.com/TencentBlueKing/crypto-python-sdk/actions/workflows/release.yml)
+
+[(English Documents Available)](https://github.com/TencentBlueKing/crypto-python-sdk/blob/main/readme_en.md)
+
+## Overview
+
+️🔧 BlueKing crypto-python-sdk 是一个基于 pyCryptodome / tongsuopy 等加密库的轻量级密码学工具包，为 Python 应用统一的加解密实现，
+便于项目在不同的加密方式之间进行无侵入切换
+
+## Features
+
+* [Basic] 提供加密统一抽象层，对接 Cryptodome / tongsuopy 等加密库，提供统一的加解密实现
+* [Basic] 支持国际主流密码学算法：AES、RSA
+* [Basic] 支持中国商用密码学算法：SM2、SM4
+* [Basic] 非对称加密支持 CBC、CTR、GCM、CFB 作为块密码模式
+* [Contrib] Django Support，集成 Django settings、ModelField
+
+## Getting started
+
+### Installation
+
+```bash
+$ pip install bk-crypto-python-sdk
+```
+
+### Usage
+
+> 更多用法参考：[使用文档](https://github.com/TencentBlueKing/crypto-python-sdk/blob/main/docs/usage.md)
+
+在项目中配置
+
+```python
+from bkcrypto import constants
+from bkcrypto.symmetric.options import AESSymmetricOptions, SM4SymmetricOptions
+from bkcrypto.asymmetric.options import RSAAsymmetricOptions
+
+BKCRYPTO = {
+    # 声明项目所使用的非对称加密算法
+    "ASYMMETRIC_CIPHER_TYPE": constants.AsymmetricCipherType.SM2.value,
+    # 声明项目所使用的对称加密算法
+    "SYMMETRIC_CIPHER_TYPE": constants.SymmetricCipherType.SM4.value,
+    "SYMMETRIC_CIPHERS": {
+        # default - 所配置的对称加密实例，根据项目需要可以配置多个
+        "default": {
+            # 可选，用于在 settings 没法直接获取 key 的情况
+            # "get_key_config": "apps.utils.encrypt.key.get_key_config",
+            # 可选，用于 ModelField，加密时携带该前缀入库，解密时分析该前缀并选择相应的解密算法
+            # ⚠️ 前缀和 cipher type 必须一一对应，且不能有前缀匹配关系
+            # "db_prefix_map": {
+            #     SymmetricCipherType.AES.value: "aes_str:::",
+            #     SymmetricCipherType.SM4.value: "sm4_str:::"
+            # },
+            # 公共参数配置，不同 cipher 初始化时共用这部分参数
+            "common": {"key": "your key"},
+            "cipher_options": {
+                constants.SymmetricCipherType.AES.value: AESSymmetricOptions(key_size=16),
+                # 蓝鲸推荐配置
+                constants.SymmetricCipherType.SM4.value: SM4SymmetricOptions(mode=constants.SymmetricMode.CTR)
+            }
+        },
+    },
+    "ASYMMETRIC_CIPHERS": {
+        # 配置同 SYMMETRIC_CIPHERS
+        "default": {
+            "common": {"public_key_string": "your key"},
+            "cipher_options": {
+                constants.AsymmetricCipherType.RSA.value: RSAAsymmetricOptions(
+                    padding=constants.RSACipherPadding.PKCS1_OAEP
+                ),
+                constants.AsymmetricCipherType.SM2.value: SM4SymmetricOptions()
+            },
+        },
+    }
 }
+```
+
+#### 非对称加密
+
+使用 `get_asymmetric_cipher` 获取 `cipher`
+
+```python
+from bkcrypto.asymmetric.ciphers import BaseAsymmetricCipher
+from bkcrypto.contrib.django.ciphers import get_asymmetric_cipher
+
+asymmetric_cipher: BaseAsymmetricCipher = get_asymmetric_cipher()
+
+# 加解密
+assert "123" == asymmetric_cipher.decrypt(asymmetric_cipher.encrypt("123"))
+# 验签
+assert asymmetric_cipher.verify(plaintext="123", signature=asymmetric_cipher.sign("123"))
+```
+
+使用 `asymmetric_cipher_manager` 获取 `BKCRYPTO.ASYMMETRIC_CIPHERS` 配置的 `cipher`
+
+```python
+from bkcrypto.asymmetric.ciphers import BaseAsymmetricCipher
+from bkcrypto.contrib.django.ciphers import asymmetric_cipher_manager
+
+asymmetric_cipher: BaseAsymmetricCipher = asymmetric_cipher_manager.cipher(using="default")
+
+# 加解密
+assert "123" == asymmetric_cipher.decrypt(asymmetric_cipher.encrypt("123"))
+# 验签
+assert asymmetric_cipher.verify(plaintext="123", signature=asymmetric_cipher.sign("123"))
+```
+
+#### 对称加密
+
+使用 `get_symmetric_cipher` 获取 `cipher`
+
+```python
+from bkcrypto.symmetric.ciphers import BaseSymmetricCipher
+from bkcrypto.contrib.django.ciphers import get_symmetric_cipher
+
+symmetric_cipher: BaseSymmetricCipher = get_symmetric_cipher()
+assert "123" == symmetric_cipher.decrypt(symmetric_cipher.encrypt("123"))
+```
+
+使用 `symmetric_cipher_manager` 获取 `BKCRYPTO.SYMMETRIC_CIPHERS` 配置的 `cipher`
+
+```python
+from bkcrypto.symmetric.ciphers import BaseSymmetricCipher
+from bkcrypto.contrib.django.ciphers import symmetric_cipher_manager
+
+# using - 指定对称加密实例，默认使用 `default`
+symmetric_cipher: BaseSymmetricCipher = symmetric_cipher_manager.cipher(using="default")
+assert "123" == symmetric_cipher.decrypt(symmetric_cipher.encrypt("123"))
+```
+
+#### SymmetricTextField
+
+```python
+from django.db import models
+from bkcrypto.contrib.django.fields import SymmetricTextField
+
+
+class IdentityData(models.Model):
+    password = SymmetricTextField("密码", blank=True, null=True)
+```
+
+## Roadmap
+
+- [版本日志](https://github.com/TencentBlueKing/crypto-python-sdk/blob/main/release.md)
+
+## Support
+
+- [蓝鲸论坛](https://bk.tencent.com/s-mart/community)
+- [蓝鲸 DevOps 在线视频教程](https://bk.tencent.com/s-mart/video/)
+- [蓝鲸社区版交流群](https://jq.qq.com/?_wv=1027&k=5zk8F7G)
+
+## BlueKing Community
+
+- [BK-CMDB](https://github.com/Tencent/bk-cmdb)：蓝鲸配置平台（蓝鲸 CMDB）是一个面向资产及应用的企业级配置管理平台。
+- [BK-CI](https://github.com/Tencent/bk-ci)：蓝鲸持续集成平台是一个开源的持续集成和持续交付系统，可以轻松将你的研发流程呈现到你面前。
+- [BK-BCS](https://github.com/Tencent/bk-bcs)：蓝鲸容器管理平台是以容器技术为基础，为微服务业务提供编排管理的基础服务平台。
+- [BK-PaaS](https://github.com/Tencent/bk-paas)：蓝鲸 PaaS 平台是一个开放式的开发平台，让开发者可以方便快捷地创建、开发、部署和管理
+  SaaS 应用。
+- [BK-SOPS](https://github.com/Tencent/bk-sops)：标准运维（SOPS）是通过可视化的图形界面进行任务流程编排和执行的系统，是蓝鲸体系中一款轻量级的调度编排类
+  SaaS 产品。
+- [BK-JOB](https://github.com/Tencent/bk-job) 蓝鲸作业平台(Job)是一套运维脚本管理系统，具备海量任务并发处理能力。
+
+## Contributing
+
+如果你有好的意见或建议，欢迎给我们提 Issues 或 Pull Requests，为蓝鲸开源社区贡献力量。   
+[腾讯开源激励计划](https://opensource.tencent.com/contribution) 鼓励开发者的参与和贡献，期待你的加入。
+
+## License
 
+基于 MIT 协议， 详细请参考 [LICENSE](https://github.com/TencentBlueKing/crypto-python-sdk/blob/main/LICENSE.txt)
 
-setup(**setup_kwargs)
```

