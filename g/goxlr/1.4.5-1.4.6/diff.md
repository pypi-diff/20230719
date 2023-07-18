# Comparing `tmp/goxlr-1.4.5.tar.gz` & `tmp/goxlr-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goxlr-1.4.5.tar", last modified: Wed Jul 12 15:33:53 2023, max compression
+gzip compressed data, was "goxlr-1.4.6.tar", last modified: Tue Jul 18 22:12:49 2023, max compression
```

## Comparing `goxlr-1.4.5.tar` & `goxlr-1.4.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:33:53.472806 goxlr-1.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-12 15:33:41.000000 goxlr-1.4.5/LICENSE-3RD-PARTY.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-12 15:33:41.000000 goxlr-1.4.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-12 15:33:53.472806 goxlr-1.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-12 15:33:41.000000 goxlr-1.4.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:33:53.468806 goxlr-1.4.5/goxlr/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-12 15:33:41.000000 goxlr-1.4.5/goxlr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 15:33:41.000000 goxlr-1.4.5/goxlr/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:33:53.472806 goxlr-1.4.5/goxlr/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-12 15:33:41.000000 goxlr-1.4.5/goxlr/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-12 15:33:41.000000 goxlr-1.4.5/goxlr/commands/daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)    26580 2023-07-12 15:33:41.000000 goxlr-1.4.5/goxlr/commands/goxlr.py
--rw-r--r--   0 runner    (1001) docker     (123)    23933 2023-07-12 15:33:41.000000 goxlr-1.4.5/goxlr/commands/status.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-12 15:33:41.000000 goxlr-1.4.5/goxlr/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-07-12 15:33:41.000000 goxlr-1.4.5/goxlr/socket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:33:53.472806 goxlr-1.4.5/goxlr/types/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-12 15:33:41.000000 goxlr-1.4.5/goxlr/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11218 2023-07-12 15:33:41.000000 goxlr-1.4.5/goxlr/types/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    22890 2023-07-12 15:33:41.000000 goxlr-1.4.5/goxlr/types/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 15:33:53.472806 goxlr-1.4.5/goxlr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-12 15:33:53.000000 goxlr-1.4.5/goxlr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-12 15:33:53.000000 goxlr-1.4.5/goxlr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 15:33:53.000000 goxlr-1.4.5/goxlr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-12 15:33:53.000000 goxlr-1.4.5/goxlr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-12 15:33:53.000000 goxlr-1.4.5/goxlr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-12 15:33:41.000000 goxlr-1.4.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-12 15:33:53.472806 goxlr-1.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-12 15:33:41.000000 goxlr-1.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:12:49.734620 goxlr-1.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-18 22:12:38.000000 goxlr-1.4.6/LICENSE-3RD-PARTY.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-18 22:12:38.000000 goxlr-1.4.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-18 22:12:49.734620 goxlr-1.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-18 22:12:38.000000 goxlr-1.4.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:12:49.734620 goxlr-1.4.6/goxlr/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-18 22:12:38.000000 goxlr-1.4.6/goxlr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-18 22:12:38.000000 goxlr-1.4.6/goxlr/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:12:49.734620 goxlr-1.4.6/goxlr/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-18 22:12:38.000000 goxlr-1.4.6/goxlr/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-18 22:12:38.000000 goxlr-1.4.6/goxlr/commands/daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26580 2023-07-18 22:12:38.000000 goxlr-1.4.6/goxlr/commands/goxlr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23933 2023-07-18 22:12:38.000000 goxlr-1.4.6/goxlr/commands/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-18 22:12:38.000000 goxlr-1.4.6/goxlr/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-07-18 22:12:38.000000 goxlr-1.4.6/goxlr/socket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:12:49.734620 goxlr-1.4.6/goxlr/types/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-18 22:12:38.000000 goxlr-1.4.6/goxlr/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11218 2023-07-18 22:12:38.000000 goxlr-1.4.6/goxlr/types/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23109 2023-07-18 22:12:38.000000 goxlr-1.4.6/goxlr/types/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 22:12:49.734620 goxlr-1.4.6/goxlr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-18 22:12:49.000000 goxlr-1.4.6/goxlr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-18 22:12:49.000000 goxlr-1.4.6/goxlr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 22:12:49.000000 goxlr-1.4.6/goxlr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-18 22:12:49.000000 goxlr-1.4.6/goxlr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-18 22:12:49.000000 goxlr-1.4.6/goxlr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-18 22:12:38.000000 goxlr-1.4.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-18 22:12:49.734620 goxlr-1.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-18 22:12:38.000000 goxlr-1.4.6/setup.py
```

### Comparing `goxlr-1.4.5/LICENSE-3RD-PARTY.txt` & `goxlr-1.4.6/LICENSE-3RD-PARTY.txt`

 * *Files identical despite different names*

### Comparing `goxlr-1.4.5/LICENSE.txt` & `goxlr-1.4.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `goxlr-1.4.5/PKG-INFO` & `goxlr-1.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goxlr
-Version: 1.4.5
+Version: 1.4.6
 Summary: A Python wrapper for the GoXLR Utility API.
 Home-page: https://github.com/samcarsonx/goxlr-py
 Author: Sam Carson
 Author-email: sam@samcarson.co.uk
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `goxlr-1.4.5/README.md` & `goxlr-1.4.6/README.md`

 * *Files identical despite different names*

### Comparing `goxlr-1.4.5/goxlr/commands/daemon.py` & `goxlr-1.4.6/goxlr/commands/daemon.py`

 * *Files identical despite different names*

### Comparing `goxlr-1.4.5/goxlr/commands/goxlr.py` & `goxlr-1.4.6/goxlr/commands/goxlr.py`

 * *Files identical despite different names*

### Comparing `goxlr-1.4.5/goxlr/commands/status.py` & `goxlr-1.4.6/goxlr/commands/status.py`

 * *Files identical despite different names*

### Comparing `goxlr-1.4.5/goxlr/socket.py` & `goxlr-1.4.6/goxlr/socket.py`

 * *Files identical despite different names*

### Comparing `goxlr-1.4.5/goxlr/types/enums.py` & `goxlr-1.4.6/goxlr/types/enums.py`

 * *Files identical despite different names*

### Comparing `goxlr-1.4.5/goxlr/types/models.py` & `goxlr-1.4.6/goxlr/types/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -104,18 +104,19 @@
 class Scribble:
     file_name: str
     bottom_text: str
     left_text: str
     inverted: bool
 
     def __init__(self, scribble: dict):
-        self.file_name = scribble.get("file_name")
-        self.bottom_text = scribble.get("bottom_text")
-        self.left_text = scribble.get("left_text")
-        self.inverted = scribble.get("inverted")
+        if scribble:  # GoXLR Minis don't have scribbles
+            self.file_name = scribble.get("file_name")
+            self.bottom_text = scribble.get("bottom_text")
+            self.left_text = scribble.get("left_text")
+            self.inverted = scribble.get("inverted")
 
 
 @dataclass
 class FaderStatus:
     channel: Channel
     mute_type: MuteFunction
     scribble: Scribble
@@ -560,18 +561,19 @@
 class Effects:
     is_enabled: bool
     active_preset: EffectBankPreset
     preset_names: Dict[EffectBankPreset, str]
     current: CurrentEffects
 
     def __init__(self, effects: dict):
-        self.is_enabled = effects.get("is_enabled")
-        self.active_preset = EffectBankPreset[effects.get("active_preset")]
-        self.preset_names = effects.get("preset_names")
-        self.current = CurrentEffects(effects.get("current"))
+        if effects:  # GoXLR Minis don't have effects
+            self.is_enabled = effects.get("is_enabled")
+            self.active_preset = EffectBankPreset[effects.get("active_preset")]
+            self.preset_names = effects.get("preset_names")
+            self.current = CurrentEffects(effects.get("current"))
 
 
 # -------------------------------------------------------
 # Mixer - Sampler
 # -------------------------------------------------------
 
 
@@ -618,19 +620,20 @@
     processing_state: SamplerProcessState
     active_bank: SampleBank
     clear_active: bool
     record_buffer: int
     banks: Dict[SampleBank, Dict[SampleButton, SampleMetadata]]
 
     def __init__(self, sampler: dict):
-        self.processing_state = SamplerProcessState(sampler.get("processing_state"))
-        self.active_bank = SampleBank[sampler.get("active_bank")]
-        self.clear_active = sampler.get("clear_active")
-        self.record_buffer = sampler.get("record_buffer")
-        self.banks = sampler.get("banks")
+        if sampler:  # GoXLR Minis don't have a sampler
+            self.processing_state = SamplerProcessState(sampler.get("processing_state"))
+            self.active_bank = SampleBank[sampler.get("active_bank")]
+            self.clear_active = sampler.get("clear_active")
+            self.record_buffer = sampler.get("record_buffer")
+            self.banks = sampler.get("banks")
 
 
 # -------------------------------------------------------
 # Mixer - Settings
 # -------------------------------------------------------
```

### Comparing `goxlr-1.4.5/goxlr.egg-info/PKG-INFO` & `goxlr-1.4.6/goxlr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goxlr
-Version: 1.4.5
+Version: 1.4.6
 Summary: A Python wrapper for the GoXLR Utility API.
 Home-page: https://github.com/samcarsonx/goxlr-py
 Author: Sam Carson
 Author-email: sam@samcarson.co.uk
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `goxlr-1.4.5/setup.py` & `goxlr-1.4.6/setup.py`

 * *Files identical despite different names*

