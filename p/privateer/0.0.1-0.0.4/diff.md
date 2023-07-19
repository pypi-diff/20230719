# Comparing `tmp/privateer-0.0.1.tar.gz` & `tmp/privateer-0.0.4.tar.gz`

## Comparing `privateer-0.0.1.tar` & `privateer-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,22 @@
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 privateer-0.0.1/.github/workflows/test.yml
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 privateer-0.0.1/config/privateer.json
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 privateer-0.0.1/config/invalid/privateer.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 privateer-0.0.1/src/__init__.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 privateer-0.0.1/src/privateer/__about__.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 privateer-0.0.1/src/privateer/__init__.py
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 privateer-0.0.1/src/privateer/cli.py
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 privateer-0.0.1/src/privateer/config.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 privateer-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 privateer-0.0.1/tests/test_cli.py
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 privateer-0.0.1/tests/test_config.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 privateer-0.0.1/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 privateer-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 privateer-0.0.1/README.md
--rw-r--r--   0        0        0     3320 2020-02-02 00:00:00.000000 privateer-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 privateer-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 privateer-0.0.4/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 privateer-0.0.4/config/privateer.json
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 privateer-0.0.4/config/invalid/privateer.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 privateer-0.0.4/src/__init__.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 privateer-0.0.4/src/privateer/__about__.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 privateer-0.0.4/src/privateer/__init__.py
+-rw-r--r--   0        0        0     5081 2020-02-02 00:00:00.000000 privateer-0.0.4/src/privateer/backup.py
+-rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 privateer-0.0.4/src/privateer/cli.py
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 privateer-0.0.4/src/privateer/config.py
+-rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 privateer-0.0.4/src/privateer/docker_helpers.py
+-rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 privateer-0.0.4/src/privateer/restore.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 privateer-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0     9328 2020-02-02 00:00:00.000000 privateer-0.0.4/tests/test_backup.py
+-rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 privateer-0.0.4/tests/test_cli.py
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 privateer-0.0.4/tests/test_config.py
+-rw-r--r--   0        0        0     5755 2020-02-02 00:00:00.000000 privateer-0.0.4/tests/test_integration.py
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 privateer-0.0.4/tests/test_schedule.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 privateer-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 privateer-0.0.4/LICENSE.txt
+-rw-r--r--   0        0        0     4915 2020-02-02 00:00:00.000000 privateer-0.0.4/README.md
+-rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 privateer-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     5929 2020-02-02 00:00:00.000000 privateer-0.0.4/PKG-INFO
```

### Comparing `privateer-0.0.1/.github/workflows/test.yml` & `privateer-0.0.4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `privateer-0.0.1/tests/test_config.py` & `privateer-0.0.4/tests/test_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,33 @@
+import os
+
 import pytest
 
 from src.privateer.config import PrivateerConfig, PrivateerHost, PrivateerTarget
 
 
 def test_config():
     cfg = PrivateerConfig("config")
     assert len(cfg.targets) == 2
     assert cfg.targets[0].name == "orderly_volume"
-    assert len(cfg.hosts) == 3
+    assert len(cfg.hosts) == 4
     assert cfg.hosts[0].name == "production"
     assert cfg.hosts[0].user is None
     assert cfg.hosts[0].port == 10022
     assert cfg.hosts[0].host_type == "remote"
     assert cfg.hosts[0].path == "starport"
     assert cfg.hosts[1].name == "uat"
     assert cfg.hosts[1].hostname == "uat.montagu.dide.ic.ac.uk"
     assert cfg.hosts[1].user == "vagrant"
     assert cfg.hosts[1].port is None
     assert cfg.hosts[1].host_type == "remote"
     assert cfg.hosts[1].path == "starport"
     assert cfg.hosts[2].name == "test"
-    assert cfg.hosts[2].path == "starport"
+    assert cfg.hosts[2].path.endswith("starport")
+    assert os.path.isabs(cfg.hosts[2].path)
     assert cfg.hosts[2].host_type == "local"
 
 
 def test_only_volume_targets_allowed():
     with pytest.raises(Exception) as err:
         PrivateerTarget({"name": "test", "type": "directory"})
     assert str(err.value) == "Only 'volume' targets are supported."
@@ -37,7 +40,14 @@
 
 
 def test_unique_hosts():
     cfg = PrivateerConfig("config/invalid")
     with pytest.raises(Exception) as err:
         cfg.get_host("annex")
     assert str(err.value) == "Invalid arguments: two hosts with the name 'annex' found."
+
+
+def test_existent_hosts():
+    cfg = PrivateerConfig("config/invalid")
+    with pytest.raises(Exception) as err:
+        cfg.get_host("badname")
+    assert str(err.value) == "Invalid arguments: no host with the name 'badname' found."
```

### Comparing `privateer-0.0.1/LICENSE.txt` & `privateer-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

