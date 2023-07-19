# Comparing `tmp/pystval-1.0.0-cp37-abi3-win_arm64.whl.zip` & `tmp/pystval-1.1.0-cp37-abi3-win_arm64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 809574 bytes, number of entries: 8
--rw-r--r--  4.6 unx    27118 b- defN 23-Jul-09 20:07 pystval-1.0.0.dist-info/METADATA
--rw-r--r--  4.6 unx       94 b- defN 23-Jul-09 20:07 pystval-1.0.0.dist-info/WHEEL
--rw-r--r--  4.6 unx     1071 b- defN 23-Jul-09 20:07 pystval-1.0.0.dist-info/license_files/LICENSE
--rw-r--r--  4.6 unx      111 b- defN 23-Jul-09 20:07 pystval/__init__.py
--rw-r--r--  4.6 unx     4316 b- defN 23-Jul-09 20:07 pystval/__init__.pyi
--rw-r--r--  4.6 unx        0 b- defN 23-Jul-09 20:07 pystval/py.typed
--rwxr-xr-x  4.6 unx  2077184 b- defN 23-Jul-09 20:07 pystval/pystval.pyd
--rw-r--r--  4.6 unx      610 b- defN 23-Jul-09 20:07 pystval-1.0.0.dist-info/RECORD
-8 files, 2110504 bytes uncompressed, 808524 bytes compressed:  61.7%
+Zip file size: 960894 bytes, number of entries: 8
+-rw-r--r--  4.6 unx     4564 b- defN 23-Jul-19 08:25 pystval-1.1.0.dist-info/METADATA
+-rw-r--r--  4.6 unx       94 b- defN 23-Jul-19 08:25 pystval-1.1.0.dist-info/WHEEL
+-rw-r--r--  4.6 unx     1071 b- defN 23-Jul-19 08:25 pystval-1.1.0.dist-info/license_files/LICENSE
+-rw-r--r--  4.6 unx      111 b- defN 23-Jul-19 08:25 pystval/__init__.py
+-rw-r--r--  4.6 unx     4671 b- defN 23-Jul-19 08:25 pystval/__init__.pyi
+-rw-r--r--  4.6 unx        0 b- defN 23-Jul-19 08:25 pystval/py.typed
+-rwxr-xr-x  4.6 unx  2462208 b- defN 23-Jul-19 08:25 pystval/pystval.pyd
+-rw-r--r--  4.6 unx      609 b- defN 23-Jul-19 08:25 pystval-1.1.0.dist-info/RECORD
+8 files, 2473328 bytes uncompressed, 959844 bytes compressed:  61.2%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
-Filename: pystval-1.0.0.dist-info/METADATA
+Filename: pystval-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: pystval-1.0.0.dist-info/WHEEL
+Filename: pystval-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: pystval-1.0.0.dist-info/license_files/LICENSE
+Filename: pystval-1.1.0.dist-info/license_files/LICENSE
 Comment: 
 
 Filename: pystval/__init__.py
 Comment: 
 
 Filename: pystval/__init__.pyi
 Comment: 
 
 Filename: pystval/py.typed
 Comment: 
 
 Filename: pystval/pystval.pyd
 Comment: 
 
-Filename: pystval-1.0.0.dist-info/RECORD
+Filename: pystval-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pystval/__init__.pyi

```diff
@@ -1,9 +1,9 @@
 import enum
-from typing import Optional, Type, TypeVar, List, Any
+from typing import Optional, Type, List, Any
 
 
 class PystvalErrorMeta(type):
     def __new__(cls, name: str, bases: tuple[type], attrs: dict[str, Any]) -> type:
         ...
 
 
@@ -64,14 +64,22 @@
         ------
         `TypeError`
             If the inner parameter is not a string
 
         """
         ...
 
+    @staticmethod
+    def auto_generate(requirements: MatchRequirement, texts: List[str]) -> Rule:
+        """
+        Automatically generate a rule based on the inner value
+        > Recommendation : use for pattern prototyping
+        """
+        ...
+
     def extend(self, nested_rules: List['Rule']) -> Rule:
         """
         Extend the rule with nested rules.
 
         Parameters
         ----------
         `nested_rules` : `List[Rule]`
@@ -123,14 +131,20 @@
 
     def mode_at_least_one_rule_for_at_least_one_match(self) -> Rule:
         """
         At least one rule should work successfully for at least one match
         """
         ...
 
+    def duplicate_matches(self) -> Rule:
+        """
+        Allow duplicate matches
+        """
+        ...
+
 
 class TemplateValidator:
     """
     A class for creating a validator
     """
 
     def __init__(self, flags: List[Type[Any]]) -> None:
```

## Comparing `pystval-1.0.0.dist-info/license_files/LICENSE` & `pystval-1.1.0.dist-info/license_files/LICENSE`

 * *Files identical despite different names*

## Comparing `pystval-1.0.0.dist-info/RECORD` & `pystval-1.1.0.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-pystval-1.0.0.dist-info/METADATA,sha256=Lgrw7HI1YoA2QLQ8WJsxeqFw50ZYtrfMFQ28QRi212E,27118
-pystval-1.0.0.dist-info/WHEEL,sha256=CJxeJmlkyomzfztRUbeYqqZey3825J0zu3mvgonjsBI,94
-pystval-1.0.0.dist-info/license_files/LICENSE,sha256=CDfNhGanHI40sn6JTFci9nfYcbUHHkWNEL0YtWeiejI,1071
+pystval-1.1.0.dist-info/METADATA,sha256=AKiB8_oVolnnQYh3PkrmIQMQZllDekTcFqq_zOcroyw,4564
+pystval-1.1.0.dist-info/WHEEL,sha256=CJxeJmlkyomzfztRUbeYqqZey3825J0zu3mvgonjsBI,94
+pystval-1.1.0.dist-info/license_files/LICENSE,sha256=CDfNhGanHI40sn6JTFci9nfYcbUHHkWNEL0YtWeiejI,1071
 pystval/__init__.py,sha256=6I5B67a3bnUpTZsF-BZxAbx5v-PSLV45rlgrbyXoep0,111
-pystval/__init__.pyi,sha256=xoH21jtk8NnHKuAlPG2FpqMeQBvSwjB3x0Mq6RScM2Q,4316
+pystval/__init__.pyi,sha256=APavJcVAF6O7VekDqgro9Yt3w5tPL0gmw4OxoFB4J0g,4671
 pystval/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pystval/pystval.pyd,sha256=IL2UWyNI4BHvTaooiAhgpXER1ZpjlB5HZ9WX7NVX2fU,2077184
-pystval-1.0.0.dist-info/RECORD,,
+pystval/pystval.pyd,sha256=o_yCgsayStMxy2WU6iphinEHw-XC6kPAnyyNCHF7Ye8,2462208
+pystval-1.1.0.dist-info/RECORD,,
```

