# Comparing `tmp/avclass-malicialab-2.8.3.tar.gz` & `tmp/avclass-malicialab-2.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avclass-malicialab-2.8.3.tar", last modified: Fri May 26 13:04:36 2023, max compression
+gzip compressed data, was "avclass-malicialab-2.8.4.tar", last modified: Wed Jul 19 12:49:25 2023, max compression
```

## Comparing `avclass-malicialab-2.8.3.tar` & `avclass-malicialab-2.8.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 juanca    (1000) juanca    (1000)        0 2023-05-26 13:04:36.697236 avclass-malicialab-2.8.3/
--rw-rw-r--   0 juanca    (1000) juanca    (1000)     1100 2020-09-01 17:16:19.000000 avclass-malicialab-2.8.3/LICENSE
--rw-rw-r--   0 juanca    (1000) juanca    (1000)       23 2023-02-23 10:39:34.000000 avclass-malicialab-2.8.3/MANIFEST.in
--rw-rw-r--   0 juanca    (1000) juanca    (1000)    17117 2023-05-26 13:04:36.697236 avclass-malicialab-2.8.3/PKG-INFO
--rw-rw-r--   0 juanca    (1000) juanca    (1000)    15317 2023-04-10 14:11:52.000000 avclass-malicialab-2.8.3/README.md
-drwxrwxr-x   0 juanca    (1000) juanca    (1000)        0 2023-05-26 13:04:36.697236 avclass-malicialab-2.8.3/avclass/
--rw-rw-r--   0 juanca    (1000) juanca    (1000)      401 2023-02-23 10:09:56.000000 avclass-malicialab-2.8.3/avclass/__init__.py
--rw-rw-r--   0 juanca    (1000) juanca    (1000)    20596 2023-05-05 15:16:06.000000 avclass-malicialab-2.8.3/avclass/common.py
-drwxrwxr-x   0 juanca    (1000) juanca    (1000)        0 2023-05-26 13:04:36.697236 avclass-malicialab-2.8.3/avclass/data/
--rw-rw-r--   0 juanca    (1000) juanca    (1000)     6823 2023-02-23 10:09:56.000000 avclass-malicialab-2.8.3/avclass/data/andropup.expansion
--rw-rw-r--   0 juanca    (1000) juanca    (1000)      308 2023-04-10 14:08:05.000000 avclass-malicialab-2.8.3/avclass/data/default.expansion
--rw-rw-r--   0 juanca    (1000) juanca    (1000)    56429 2023-04-10 14:08:05.000000 avclass-malicialab-2.8.3/avclass/data/default.tagging
--rw-rw-r--   0 juanca    (1000) juanca    (1000)    41254 2023-04-10 14:08:05.000000 avclass-malicialab-2.8.3/avclass/data/default.taxonomy
--rwxrwxr-x   0 juanca    (1000) juanca    (1000)     4202 2023-02-26 07:44:35.000000 avclass-malicialab-2.8.3/avclass/evaluate.py
--rwxrwxr-x   0 juanca    (1000) juanca    (1000)    23609 2023-05-26 13:02:48.000000 avclass-malicialab-2.8.3/avclass/labeler.py
--rwxrwxr-x   0 juanca    (1000) juanca    (1000)     3996 2023-03-04 13:05:26.000000 avclass-malicialab-2.8.3/avclass/misp.py
--rwxrwxr-x   0 juanca    (1000) juanca    (1000)     1704 2023-02-26 07:00:49.000000 avclass-malicialab-2.8.3/avclass/normalize.py
--rwxrwxr-x   0 juanca    (1000) juanca    (1000)    17636 2023-02-23 10:26:36.000000 avclass-malicialab-2.8.3/avclass/update.py
-drwxrwxr-x   0 juanca    (1000) juanca    (1000)        0 2023-05-26 13:04:36.697236 avclass-malicialab-2.8.3/avclass_malicialab.egg-info/
--rw-rw-r--   0 juanca    (1000) juanca    (1000)    17117 2023-05-26 13:04:36.000000 avclass-malicialab-2.8.3/avclass_malicialab.egg-info/PKG-INFO
--rw-rw-r--   0 juanca    (1000) juanca    (1000)      511 2023-05-26 13:04:36.000000 avclass-malicialab-2.8.3/avclass_malicialab.egg-info/SOURCES.txt
--rw-rw-r--   0 juanca    (1000) juanca    (1000)        1 2023-05-26 13:04:36.000000 avclass-malicialab-2.8.3/avclass_malicialab.egg-info/dependency_links.txt
--rw-rw-r--   0 juanca    (1000) juanca    (1000)      162 2023-05-26 13:04:36.000000 avclass-malicialab-2.8.3/avclass_malicialab.egg-info/entry_points.txt
--rw-rw-r--   0 juanca    (1000) juanca    (1000)        8 2023-05-26 13:04:36.000000 avclass-malicialab-2.8.3/avclass_malicialab.egg-info/top_level.txt
--rw-rw-r--   0 juanca    (1000) juanca    (1000)      831 2023-05-26 13:03:02.000000 avclass-malicialab-2.8.3/pyproject.toml
--rw-rw-r--   0 juanca    (1000) juanca    (1000)       38 2023-05-26 13:04:36.697236 avclass-malicialab-2.8.3/setup.cfg
+drwxrwxr-x   0 juanca    (1000) juanca    (1000)        0 2023-07-19 12:49:25.289572 avclass-malicialab-2.8.4/
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)     1100 2020-09-01 17:16:19.000000 avclass-malicialab-2.8.4/LICENSE
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)       23 2023-02-23 10:39:34.000000 avclass-malicialab-2.8.4/MANIFEST.in
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)    17117 2023-07-19 12:49:25.289572 avclass-malicialab-2.8.4/PKG-INFO
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)    15317 2023-04-10 14:11:52.000000 avclass-malicialab-2.8.4/README.md
+drwxrwxr-x   0 juanca    (1000) juanca    (1000)        0 2023-07-19 12:49:25.289572 avclass-malicialab-2.8.4/avclass/
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)      401 2023-02-23 10:09:56.000000 avclass-malicialab-2.8.4/avclass/__init__.py
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)    20596 2023-05-05 15:16:06.000000 avclass-malicialab-2.8.4/avclass/common.py
+drwxrwxr-x   0 juanca    (1000) juanca    (1000)        0 2023-07-19 12:49:25.289572 avclass-malicialab-2.8.4/avclass/data/
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)     6823 2023-02-23 10:09:56.000000 avclass-malicialab-2.8.4/avclass/data/andropup.expansion
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)      308 2023-04-10 14:08:05.000000 avclass-malicialab-2.8.4/avclass/data/default.expansion
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)    56454 2023-07-19 12:45:37.000000 avclass-malicialab-2.8.4/avclass/data/default.tagging
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)    41330 2023-07-19 12:44:59.000000 avclass-malicialab-2.8.4/avclass/data/default.taxonomy
+-rwxrwxr-x   0 juanca    (1000) juanca    (1000)     4202 2023-02-26 07:44:35.000000 avclass-malicialab-2.8.4/avclass/evaluate.py
+-rwxrwxr-x   0 juanca    (1000) juanca    (1000)    23609 2023-05-26 13:02:48.000000 avclass-malicialab-2.8.4/avclass/labeler.py
+-rwxrwxr-x   0 juanca    (1000) juanca    (1000)     3996 2023-03-04 13:05:26.000000 avclass-malicialab-2.8.4/avclass/misp.py
+-rwxrwxr-x   0 juanca    (1000) juanca    (1000)     1704 2023-02-26 07:00:49.000000 avclass-malicialab-2.8.4/avclass/normalize.py
+-rwxrwxr-x   0 juanca    (1000) juanca    (1000)    17636 2023-02-23 10:26:36.000000 avclass-malicialab-2.8.4/avclass/update.py
+drwxrwxr-x   0 juanca    (1000) juanca    (1000)        0 2023-07-19 12:49:25.289572 avclass-malicialab-2.8.4/avclass_malicialab.egg-info/
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)    17117 2023-07-19 12:49:25.000000 avclass-malicialab-2.8.4/avclass_malicialab.egg-info/PKG-INFO
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)      511 2023-07-19 12:49:25.000000 avclass-malicialab-2.8.4/avclass_malicialab.egg-info/SOURCES.txt
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)        1 2023-07-19 12:49:25.000000 avclass-malicialab-2.8.4/avclass_malicialab.egg-info/dependency_links.txt
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)      162 2023-07-19 12:49:25.000000 avclass-malicialab-2.8.4/avclass_malicialab.egg-info/entry_points.txt
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)        8 2023-07-19 12:49:25.000000 avclass-malicialab-2.8.4/avclass_malicialab.egg-info/top_level.txt
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)      831 2023-07-19 12:48:34.000000 avclass-malicialab-2.8.4/pyproject.toml
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)       38 2023-07-19 12:49:25.289572 avclass-malicialab-2.8.4/setup.cfg
```

### Comparing `avclass-malicialab-2.8.3/LICENSE` & `avclass-malicialab-2.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `avclass-malicialab-2.8.3/PKG-INFO` & `avclass-malicialab-2.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avclass-malicialab
-Version: 2.8.3
+Version: 2.8.4
 Summary: AVClass is a Python package and command line tool to tag / label malware samples.
 Author: MaliciaLab
 License: MIT License
         
         Copyright (c) 2016-2020 MaliciaLab @ IMDEA Software Institute
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `avclass-malicialab-2.8.3/README.md` & `avclass-malicialab-2.8.4/README.md`

 * *Files identical despite different names*

### Comparing `avclass-malicialab-2.8.3/avclass/common.py` & `avclass-malicialab-2.8.4/avclass/common.py`

 * *Files identical despite different names*

### Comparing `avclass-malicialab-2.8.3/avclass/data/andropup.expansion` & `avclass-malicialab-2.8.4/avclass/data/andropup.expansion`

 * *Files identical despite different names*

### Comparing `avclass-malicialab-2.8.3/avclass/data/default.tagging` & `avclass-malicialab-2.8.4/avclass/data/default.tagging`

 * *Files 1% similar despite different names*

```diff
@@ -2179,14 +2179,15 @@
 prifou	dealply
 priplut	opensupdater
 privacyrisk	grayware
 privitize	techsnab
 prizona	webalta
 processhider	prochider
 prochack	processhacker
+prochijack	processhijack
 prochid	prochider
 prochide	prochider
 prockill	killproc
 prodatect	fakesysdef
 progent	proagent
 proinstall	winwrapper
 projectcryptxxx	cryptxxx
```

### Comparing `avclass-malicialab-2.8.3/avclass/data/default.taxonomy` & `avclass-malicialab-2.8.4/avclass/data/default.taxonomy`

 * *Files 0% similar despite different names*

```diff
@@ -3074,20 +3074,23 @@
 GEN:based
 GEN:behav
 GEN:behaveslike
 GEN:bloodhound
 GEN:bscope
 GEN:cloud
 GEN:confidence
+GEN:content
 GEN:copiet
 GEN:dangerousobject
 GEN:dangeroussig
 GEN:deepscan
+GEN:detection
 GEN:eheur
 GEN:encodefeature
+GEN:error
 GEN:file
 GEN:filerepmalware
 GEN:gen
 GEN:gena
 GEN:generic
 GEN:generica
 GEN:generickd
@@ -3129,24 +3132,26 @@
 GEN:heuristic
 GEN:high
 GEN:highconfidence
 GEN:igeneric
 GEN:kcloud
 GEN:lookslike
 GEN:malagent
+GEN:malcode
 GEN:maldroid
 GEN:malicious
 GEN:maltrec
 GEN:malware
 GEN:memscan
 GEN:mlwr
 GEN:moderate
 GEN:multi
 GEN:multiple
 GEN:normal
+GEN:notsuspicious
 GEN:onion
 GEN:optional
 GEN:other
 GEN:password
 GEN:posible
 GEN:possible
 GEN:possiblemalware
@@ -3155,14 +3160,15 @@
 GEN:reputation
 GEN:sape
 GEN:score
 GEN:securityrisk
 GEN:siggen
 GEN:singleton
 GEN:software
+GEN:sonar
 GEN:static
 GEN:susp
 GEN:suspect
 GEN:suspectcrc
 GEN:suspected
 GEN:suspic
 GEN:suspicious
```

### Comparing `avclass-malicialab-2.8.3/avclass/evaluate.py` & `avclass-malicialab-2.8.4/avclass/evaluate.py`

 * *Files identical despite different names*

### Comparing `avclass-malicialab-2.8.3/avclass/labeler.py` & `avclass-malicialab-2.8.4/avclass/labeler.py`

 * *Files identical despite different names*

### Comparing `avclass-malicialab-2.8.3/avclass/misp.py` & `avclass-malicialab-2.8.4/avclass/misp.py`

 * *Files identical despite different names*

### Comparing `avclass-malicialab-2.8.3/avclass/normalize.py` & `avclass-malicialab-2.8.4/avclass/normalize.py`

 * *Files identical despite different names*

### Comparing `avclass-malicialab-2.8.3/avclass/update.py` & `avclass-malicialab-2.8.4/avclass/update.py`

 * *Files identical despite different names*

### Comparing `avclass-malicialab-2.8.3/avclass_malicialab.egg-info/PKG-INFO` & `avclass-malicialab-2.8.4/avclass_malicialab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avclass-malicialab
-Version: 2.8.3
+Version: 2.8.4
 Summary: AVClass is a Python package and command line tool to tag / label malware samples.
 Author: MaliciaLab
 License: MIT License
         
         Copyright (c) 2016-2020 MaliciaLab @ IMDEA Software Institute
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `avclass-malicialab-2.8.3/pyproject.toml` & `avclass-malicialab-2.8.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "avclass-malicialab"
-version = "2.8.3"
+version = "2.8.4"
 description = "AVClass is a Python package and command line tool to tag / label malware samples."
 readme = "README.md"
 authors = [{ name = "MaliciaLab" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

