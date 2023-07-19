# Comparing `tmp/panos_upgrade_assurance-0.1.1.tar.gz` & `tmp/panos_upgrade_assurance-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panos_upgrade_assurance-0.1.1.tar", max compression
+gzip compressed data, was "panos_upgrade_assurance-0.1.2.tar", max compression
```

## Comparing `panos_upgrade_assurance-0.1.1.tar` & `panos_upgrade_assurance-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1081 2023-07-05 01:34:01.761817 panos_upgrade_assurance-0.1.1/LICENSE
--rw-r--r--   0        0        0      930 2023-07-05 01:34:01.761817 panos_upgrade_assurance-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-07-05 01:34:01.765817 panos_upgrade_assurance-0.1.1/panos_upgrade_assurance/__init__.py
--rw-r--r--   0        0        0    44057 2023-07-05 01:34:01.765817 panos_upgrade_assurance-0.1.1/panos_upgrade_assurance/check_firewall.py
--rw-r--r--   0        0        0     2472 2023-07-05 01:34:01.765817 panos_upgrade_assurance-0.1.1/panos_upgrade_assurance/exceptions.py
--rw-r--r--   0        0        0    39216 2023-07-05 01:34:01.765817 panos_upgrade_assurance-0.1.1/panos_upgrade_assurance/firewall_proxy.py
--rw-r--r--   0        0        0    31244 2023-07-05 01:34:01.765817 panos_upgrade_assurance-0.1.1/panos_upgrade_assurance/snapshot_compare.py
--rw-r--r--   0        0        0    12349 2023-07-05 01:34:01.765817 panos_upgrade_assurance-0.1.1/panos_upgrade_assurance/utils.py
--rw-r--r--   0        0        0     1140 2023-07-05 01:34:23.706229 panos_upgrade_assurance-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1617 1970-01-01 00:00:00.000000 panos_upgrade_assurance-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-07-19 01:44:22.604991 panos_upgrade_assurance-0.1.2/LICENSE
+-rw-r--r--   0        0        0      930 2023-07-19 01:44:22.604991 panos_upgrade_assurance-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-19 01:44:22.604991 panos_upgrade_assurance-0.1.2/panos_upgrade_assurance/__init__.py
+-rw-r--r--   0        0        0    44638 2023-07-19 01:44:22.608991 panos_upgrade_assurance-0.1.2/panos_upgrade_assurance/check_firewall.py
+-rw-r--r--   0        0        0     2472 2023-07-19 01:44:22.608991 panos_upgrade_assurance-0.1.2/panos_upgrade_assurance/exceptions.py
+-rw-r--r--   0        0        0    39604 2023-07-19 01:44:22.608991 panos_upgrade_assurance-0.1.2/panos_upgrade_assurance/firewall_proxy.py
+-rw-r--r--   0        0        0    31684 2023-07-19 01:44:22.608991 panos_upgrade_assurance-0.1.2/panos_upgrade_assurance/snapshot_compare.py
+-rw-r--r--   0        0        0    12400 2023-07-19 01:44:22.608991 panos_upgrade_assurance-0.1.2/panos_upgrade_assurance/utils.py
+-rw-r--r--   0        0        0     1271 2023-07-19 01:44:40.161096 panos_upgrade_assurance-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1569 1970-01-01 00:00:00.000000 panos_upgrade_assurance-0.1.2/PKG-INFO
```

### Comparing `panos_upgrade_assurance-0.1.1/LICENSE` & `panos_upgrade_assurance-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `panos_upgrade_assurance-0.1.1/README.md` & `panos_upgrade_assurance-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `panos_upgrade_assurance-0.1.1/panos_upgrade_assurance/check_firewall.py` & `panos_upgrade_assurance-0.1.2/panos_upgrade_assurance/check_firewall.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,21 +54,23 @@
         This mapping is used to verify requested check types and to map a check with an actual method that will be eventually run.
         Keys in this dictionary are check names as defined in the
         [`CheckType`](/panos/docs/panos-upgrade-assurance/api/utils#class-checktype) class, values are references to methods that
         will be run.
 
     """
 
-    def __init__(self, node: FirewallProxy) -> None:
+    def __init__(self, node: FirewallProxy, skip_force_locale: Optional[bool] = False) -> None:
         """CheckFirewall constructor.
 
         # Parameters
 
         node (FirewallProxy): Object representing a device against which checks and/or snapshots are run. See
             [`FirewallProxy`](/panos/docs/panos-upgrade-assurance/api/firewall_proxy#class-firewallproxy) class' documentation.
+        skip_force_locale (bool, optional): (defaults to `False`) Use with caution, when set to `True` will skip setting locale to
+            en_US.UTF-8 for the module which will parse the datetime strings in checks with current locale setting.
 
         """
         self._node = node
         self._snapshot_method_mapping = {
             SnapType.NICS: self._node.get_nics,
             SnapType.ROUTES: self._node.get_routes,
             SnapType.LICENSE: self._node.get_licenses,
@@ -89,17 +91,18 @@
             CheckType.SESSION_EXIST: self.check_critical_session,
             CheckType.ARP_ENTRY_EXIST: self.check_arp_entry,
             CheckType.IPSEC_TUNNEL_STATUS: self.check_ipsec_tunnel_status,
             CheckType.FREE_DISK_SPACE: self.check_free_disk_space,
             CheckType.MP_DP_CLOCK_SYNC: self.check_mp_dp_sync,
             CheckType.CERTS: self.check_ssl_cert_requirements,
         }
-        locale.setlocale(
-            locale.LC_ALL, "en_US.UTF-8"
-        )  # force locale for datetime string parsing when non-English locale is set on host
+        if not skip_force_locale:
+            locale.setlocale(
+                locale.LC_ALL, "en_US.UTF-8"
+            )  # force locale for datetime string parsing when non-English locale is set on host
 
     def check_pending_changes(self) -> CheckResult:
         """Check if there are pending changes on device.
 
         It checks two states:
 
         1. if there is full commit required on the device,
@@ -471,15 +474,15 @@
                     if version:
                         result.status = CheckStatus.SUCCESS
                         result.reason = conditional_success_text
                     else:
                         result.status = CheckStatus.ERROR
                         result.reason = exception_text
 
-            if not result:
+            if result.status is CheckStatus.FAIL:  # NOTE skip for SUCCESS and ERROR
                 reason_suffix = (
                     f"older then the request one ({required_version})."
                     if version
                     else f"not the latest one ({required_version})."
                 )
                 result.reason = f"Installed content DB version ({installed_version}) is {reason_suffix}"
 
@@ -820,21 +823,21 @@
             result.status = CheckStatus.ERROR
             result.reason = f"The provided minimum ECDSA hashing method ({ecdsa_min_hash_method}) is not supported."
             return result
 
         rsa_min_key_size = rsa.get("key_size", 2048)
         if not (isinstance(rsa_min_key_size, int) and rsa_min_key_size > 0):
             result.status = CheckStatus.ERROR
-            result.reason = "The provided minimum RSA key size should be an integer grater than 0."
+            result.reason = "The provided minimum RSA key size should be an integer greater than 0."
             return result
 
         ecdsa_min_key_size = ecdsa.get("key_size", 256)
         if not (isinstance(ecdsa_min_key_size, int) and ecdsa_min_key_size > 0):
             result.status = CheckStatus.ERROR
-            result.reason = "The provided minimum ECDSA key size should be an integer grater than 0."
+            result.reason = "The provided minimum ECDSA key size should be an integer greater than 0."
             return result
 
         failed_certs = []
         for cert_name, certificate in certificates.items():
             cert = oSSL.load_certificate(oSSL.FILETYPE_PEM, certificate["public-key"])
 
             cert_key_size = cert.get_pubkey().bits()
@@ -846,15 +849,17 @@
                 return result
 
             cert_hash_method = cert.to_cryptography().signature_hash_algorithm.name.upper()
             if cert_hash_method in [member.name for member in SupportedHashes]:
                 cert_hash = SupportedHashes[cert_hash_method]
             else:
                 result.status = CheckStatus.ERROR
-                result.reason = f"The certificate's hashing method ({cert_hash}) is not supported? Please check the device."
+                result.reason = (
+                    f"The certificate's hashing method ({cert_hash_method}) is not supported? Please check the device."
+                )
                 return result
 
             if (cert_key_size < (rsa_min_key_size if cert_algorithm == "RSA" else ecdsa_min_key_size)) or (
                 cert_hash.value < (rsa_min_hash.value if cert_algorithm == "RSA" else ecdsa_min_hash.value)
             ):
                 failed_certs.append(f"{cert_name} (size: {cert_key_size}, hash: {cert_hash_method})")
 
@@ -945,15 +950,17 @@
             if isinstance(check, dict):
                 check_type, check_config = next(iter(check.items()))
                 # check_result = self._check_method_mapping[check_type](check_config)
             elif isinstance(check, str):
                 check_type, check_config = check, {}
                 # check_result = self._check_method_mapping[check_type]()
             else:
-                raise exceptions.WrongDataTypeException(f"Wrong configuration format for check: {check}.")
+                raise exceptions.WrongDataTypeException(
+                    f"Wrong configuration format for check: {check}."
+                )  # NOTE checks are already validated in ConfigParser._extrac_element_name - this is never executed.
 
             check_result = self._check_method_mapping[check_type](
                 **check_config
             )  # (**) would pass dict config values as separate parameters to method.
             result[check_type] = str(check_result) if report_style else {"state": bool(check_result), "reason": str(check_result)}
 
         return result
```

### Comparing `panos_upgrade_assurance-0.1.1/panos_upgrade_assurance/exceptions.py` & `panos_upgrade_assurance-0.1.2/panos_upgrade_assurance/exceptions.py`

 * *Files identical despite different names*

### Comparing `panos_upgrade_assurance-0.1.1/panos_upgrade_assurance/firewall_proxy.py` & `panos_upgrade_assurance-0.1.2/panos_upgrade_assurance/firewall_proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -867,31 +867,37 @@
         # we start with index 1 to skip header
         for i in range(1, len(disk_space_list)):
             row = disk_space_list[i]
             row_items = row.split(" ")
             row_items_trimmed = [item for item in row_items if item != ""]
 
             mount_point = row_items_trimmed[-1]
-            free_size_short = row_items_trimmed[3]
-            free_size_name = free_size_short[-1]
-            free_size_number = float(free_size_short[0:-1])
-
-            if isinstance(free_size_name, str):
-                if free_size_name == "G":
-                    free_size = free_size_number * 1024
-                elif free_size_name == "M":
-                    free_size = free_size_number
-                elif free_size_name == "K":
-                    free_size = free_size_number / 1024
-
-            elif isinstance(free_size_name, int):
-                free_size = free_size_short / 1024 / 1024
-
-            else:
-                raise exceptions.WrongDiskSizeFormatException("Free disk size has wrong format.")
+            try:
+                free_size_short = row_items_trimmed[3]
+                free_size_name = free_size_short[-1]
+                free_size_number = float(free_size_short[0:-1])
+
+                if not free_size_name.isnumeric():
+                    if free_size_name == "G":
+                        free_size = free_size_number * 1024
+                    elif free_size_name == "M":
+                        free_size = free_size_number
+                    elif free_size_name == "K":
+                        free_size = free_size_number / 1024
+                    else:
+                        raise exceptions.WrongDiskSizeFormatException("Free disk size has wrong format.")
+                else:
+                    free_size = float(free_size_short) / 1024 / 1024
+
+            except exceptions.WrongDiskSizeFormatException:
+                raise
+            except Exception:
+                raise exceptions.MalformedResponseException(
+                    f"Reported disk space block does not have typical structure: <{row}>."
+                )
 
             result[mount_point] = floor(free_size)
 
         return result
 
     def get_available_image_data(self) -> dict:
         """Get information on the available to download PanOS image versions.
@@ -943,15 +949,15 @@
 
         try:
             image_data = self.op_parser(cmd="request system software check")
         except PanXapiError as exp:
             if str(exp) == "Failed to check upgrade info due to Unknown error. Please check network connectivity and try again.":
                 raise exceptions.UpdateServerConnectivityException(str(exp)) from exp
             else:
-                raise exceptions.exp
+                raise
 
         images = dict(image_data["sw-updates"]["versions"])["entry"]
         for image in images if isinstance(images, list) else [images]:
             result[image["version"]] = dict(image)
 
         return result
 
@@ -1073,15 +1079,15 @@
 
         """
         configuration = self.op_parser(cmd="show config running")
         shared_config = configuration["config"]["shared"]
 
         result = dict()
 
-        if "certificate" in shared_config:
+        if "certificate" in shared_config:  # NOTE this causes exception if shared config has no sub-elements
             certificates = shared_config["certificate"]["entry"]
             for certificate in certificates if isinstance(certificates, list) else [certificates]:
                 certificate.pop("private-key")
                 cert_name = certificate.pop("@name")
                 result[cert_name] = certificate
 
         return result
```

### Comparing `panos_upgrade_assurance-0.1.1/panos_upgrade_assurance/snapshot_compare.py` & `panos_upgrade_assurance-0.1.2/panos_upgrade_assurance/snapshot_compare.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,17 @@
             if isinstance(report, dict):
                 report_type, report_config = list(report.items())[0]
                 report_config.update({"report_type": report_type})
             elif isinstance(report, str):
                 report_type = report
                 report_config = {"report_type": report_type}
             else:
-                raise exceptions.WrongDataTypeException(f"Wrong configuration format for report: {report}.")
+                raise exceptions.WrongDataTypeException(
+                    f"Wrong configuration format for report: {report}."
+                )  # NOTE checks are already validated in ConfigParser - this is never executed.
 
             self.key_checker(self.left_snap, self.right_snap, report_type)
             result.update({report_type: self._functions_mapping[report_type](**report_config)})
 
         return result
 
     @staticmethod
@@ -379,18 +381,14 @@
                 'passed': True,
                 'changed_raw': {}
             }
         }
         ```
 
         """
-
-        if not (left_side_to_compare and right_side_to_compare):
-            return {}
-
         result = dict(
             missing=dict(passed=True, missing_keys=[]),
             added=dict(passed=True, added_keys=[]),
             changed=dict(passed=True, changed_raw={}),
         )
 
         missing = left_side_to_compare.keys() - right_side_to_compare.keys()
@@ -402,44 +400,46 @@
         added = right_side_to_compare.keys() - left_side_to_compare.keys()
         if added:
             result["added"]["passed"] = False
             for key in added:
                 result["added"]["added_keys"].append(key)
 
         common_keys = left_side_to_compare.keys() & right_side_to_compare.keys()
-        at_lowest_level = True if isinstance(right_side_to_compare[list(common_keys)[0]], str) else False
-        keys_to_check = (
-            ConfigParser(valid_elements=set(common_keys), requested_config=properties).prepare_config()
-            if at_lowest_level
-            else common_keys
-        )
-
-        item_changed = False
-        for key in keys_to_check:
-            if right_side_to_compare[key] != left_side_to_compare[key]:
-                if isinstance(left_side_to_compare[key], str):
-                    result["changed"]["changed_raw"][key] = dict(
-                        left_snap=left_side_to_compare[key],
-                        right_snap=right_side_to_compare[key],
-                    )
-                    item_changed = True
-                elif isinstance(left_side_to_compare[key], dict):
-                    nested_results = SnapshotCompare.calculate_diff_on_dicts(
-                        left_side_to_compare=left_side_to_compare[key],
-                        right_side_to_compare=right_side_to_compare[key],
-                        properties=properties,
-                    )
+        if common_keys:
+            next_level_value = left_side_to_compare[next(iter(common_keys))]
+            at_lowest_level = True if not isinstance(next_level_value, dict) else False
+            keys_to_check = (
+                ConfigParser(valid_elements=set(common_keys), requested_config=properties).prepare_config()
+                if at_lowest_level
+                else common_keys
+            )
 
-                    SnapshotCompare.calculate_passed(nested_results)
-                    if not nested_results["passed"]:
-                        result["changed"]["changed_raw"][key] = nested_results
+            item_changed = False
+            for key in keys_to_check:
+                if right_side_to_compare[key] != left_side_to_compare[key]:
+                    if isinstance(left_side_to_compare[key], str):
+                        result["changed"]["changed_raw"][key] = dict(
+                            left_snap=left_side_to_compare[key],
+                            right_snap=right_side_to_compare[key],
+                        )
                         item_changed = True
-                else:
-                    raise exceptions.WrongDataTypeException(f"Unknown value format for key {key}.")
-            result["changed"]["passed"] = not item_changed
+                    elif isinstance(left_side_to_compare[key], dict):
+                        nested_results = SnapshotCompare.calculate_diff_on_dicts(
+                            left_side_to_compare=left_side_to_compare[key],
+                            right_side_to_compare=right_side_to_compare[key],
+                            properties=properties,
+                        )
+
+                        SnapshotCompare.calculate_passed(nested_results)
+                        if not nested_results["passed"]:
+                            result["changed"]["changed_raw"][key] = nested_results
+                            item_changed = True
+                    else:
+                        raise exceptions.WrongDataTypeException(f"Unknown value format for key {key}.")
+                result["changed"]["passed"] = not item_changed
 
         return result
 
     @staticmethod
     def calculate_passed(result: Dict[str, Union[dict, str]]) -> None:
         """The static method to calculate the upper level `passed` value.
 
@@ -581,31 +581,38 @@
         # Returns
 
         dict: Comparison results.
 
         """
         result = {}
 
-        diff = SnapshotCompare.calculate_diff_on_dicts(
+        diff = self.calculate_diff_on_dicts(
             left_side_to_compare=self.left_snap[report_type],
             right_side_to_compare=self.right_snap[report_type],
             properties=properties,
         )
         result.update(diff)
 
         if count_change_threshold and result:
             if count_change_threshold < 0 or count_change_threshold > 100:
                 raise exceptions.WrongDataTypeException("The threshold should be a percentage value between 0 and 100.")
 
             added_count = len(result["added"]["added_keys"])
             missing_count = len(result["missing"]["missing_keys"])
             changed_count = len(result["changed"]["changed_raw"])
             left_total_count = len(self.left_snap[report_type].keys())
+            right_total_count = len(self.right_snap[report_type].keys())
+
+            if left_total_count == 0 and right_total_count == 0:  # diff should be 0 when both sides are empty
+                diff = 0
+            elif left_total_count == 0:
+                diff = 1
+            else:
+                diff = (added_count + missing_count + changed_count) / left_total_count
 
-            diff = 1 if left_total_count == 0 else (added_count + missing_count + changed_count) / left_total_count
             diff_percentage = round(float(diff) * 100, 2)
 
             passed = diff_percentage <= count_change_threshold
 
             result.update(
                 {
                     "count_change_percentage": dict(
@@ -613,15 +620,15 @@
                         change_percentage=diff_percentage,
                         change_threshold=float(count_change_threshold),
                     )
                 }
             )
 
         if result:
-            SnapshotCompare.calculate_passed(result)
+            self.calculate_passed(result)
         else:
             result = None
         return result
 
     # custom compare methods
     def get_count_change_percentage(
         self,
@@ -748,17 +755,17 @@
             requested_config=thresholds,
         ).prepare_config()
 
         for element in elements:
             element_type, threshold_value = list(element.items())[0]
             result.update(
                 {
-                    element_type: SnapshotCompare.calculate_change_percentage(
+                    element_type: self.calculate_change_percentage(
                         first_value=self.left_snap[report_type][element_type],
                         second_value=self.right_snap[report_type][element_type],
                         threshold=threshold_value,
                     )
                 }
             )
 
-        SnapshotCompare.calculate_passed(result)
+        self.calculate_passed(result)
         return result
```

### Comparing `panos_upgrade_assurance-0.1.1/panos_upgrade_assurance/utils.py` & `panos_upgrade_assurance-0.1.2/panos_upgrade_assurance/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -305,15 +305,15 @@
     """
     if boolstr not in ["yes", "no"]:
         raise exceptions.WrongDataTypeException(f"Cannot interpret following string as boolean: {boolstr}.")
 
     return True if boolstr == "yes" else False
 
 
-def printer(report: dict, indent_level: int = 0) -> None:
+def printer(report: dict, indent_level: int = 0) -> None:  # pragma: no cover - exclude from pytest coverage
     """Print reports in human friendly format.
 
     # Parameters
 
     report (dict): Dict with reports from tests.
     indent_level (int): Indentation level.
```

### Comparing `panos_upgrade_assurance-0.1.1/pyproject.toml` & `panos_upgrade_assurance-0.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "panos-upgrade-assurance"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Palo Alto Networks"]
 readme = "README.md"
 packages = [
     { include = "panos_upgrade_assurance" }
 ]
 classifiers = [
@@ -26,22 +26,28 @@
 
 [tool.poetry.group.dev.dependencies]
 pydoc-markdown = "^4.6"
 flake8 = "^6.0"
 black = "^23.3"
 bandit = "^1.7"
 flake8-pyproject = "^1.2"
+pytest = "^7.2.1"
+pytest-cov = "^4.0.0"
+deepdiff = "^6.3.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.bandit]
 exclude_dirs = ["docs", ".venv", ".github", "docker_image", "dist"]
-skips = ["B405"]
+skips = ["B405", "B314"]
+
+[tool.bandit.assert_used]
+skips = ['*_test.py', '*test_*.py']
 
 [tool.black]
 line-length = 130
 
 [tool.flake8]
 select = ["C","E","F","W","B","D","B950"]
 ignore = ["E203","E501","W503","D203","D102","D103","D107","D400","E501"]
```

### Comparing `panos_upgrade_assurance-0.1.1/PKG-INFO` & `panos_upgrade_assurance-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: panos-upgrade-assurance
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Palo Alto Networks
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Requires-Dist: pan-os-python (>=1.8,<2.0)
 Requires-Dist: pan-python (>=0.17,<0.18)
 Requires-Dist: pyopenssl (>=23.2,<24.0)
 Requires-Dist: xmltodict (>=0.13,<0.14)
 Description-Content-Type: text/markdown
 
 # PAN-OS Upgrade Assurance
```

