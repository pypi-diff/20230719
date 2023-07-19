# Comparing `tmp/xnatuploader-1.1.2.tar.gz` & `tmp/xnatuploader-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xnatuploader-1.1.2.tar", last modified: Mon May 29 06:58:47 2023, max compression
+gzip compressed data, was "xnatuploader-1.1.3.tar", last modified: Wed Jul 19 05:36:13 2023, max compression
```

## Comparing `xnatuploader-1.1.2.tar` & `xnatuploader-1.1.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2023-05-29 06:58:47.590266 xnatuploader-1.1.2/
--rw-r--r--   0 mike       (501) staff       (20)    14372 2023-05-29 06:58:47.590507 xnatuploader-1.1.2/PKG-INFO
--rw-r--r--   0 mike       (501) staff       (20)    13805 2023-02-16 03:37:24.000000 xnatuploader-1.1.2/README.md
--rw-r--r--   0 mike       (501) staff       (20)       93 2022-06-16 06:56:16.000000 xnatuploader-1.1.2/pyproject.toml
--rw-r--r--   0 mike       (501) staff       (20)     1076 2023-05-29 06:58:47.591563 xnatuploader-1.1.2/setup.cfg
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2023-05-29 06:58:47.576581 xnatuploader-1.1.2/src/
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2023-05-29 06:58:47.583813 xnatuploader-1.1.2/src/xnatuploader/
--rw-r--r--   0 mike       (501) staff       (20)       72 2022-06-16 06:56:16.000000 xnatuploader-1.1.2/src/xnatuploader/__init__.py
--rw-r--r--   0 mike       (501) staff       (20)      283 2023-05-25 02:08:09.000000 xnatuploader-1.1.2/src/xnatuploader/dataclass.py
--rw-r--r--   0 mike       (501) staff       (20)     3202 2023-05-29 06:43:19.000000 xnatuploader-1.1.2/src/xnatuploader/dicoms.py
--rw-r--r--   0 mike       (501) staff       (20)    15000 2023-05-29 06:43:19.000000 xnatuploader-1.1.2/src/xnatuploader/matcher.py
--rw-r--r--   0 mike       (501) staff       (20)     8947 2023-03-15 03:09:46.000000 xnatuploader-1.1.2/src/xnatuploader/put.py
--rw-r--r--   0 mike       (501) staff       (20)     5358 2023-05-29 06:43:19.000000 xnatuploader-1.1.2/src/xnatuploader/upload.py
--rw-r--r--   0 mike       (501) staff       (20)      203 2023-04-05 06:48:06.000000 xnatuploader-1.1.2/src/xnatuploader/userdict.py
--rw-r--r--   0 mike       (501) staff       (20)     3898 2023-05-29 06:43:19.000000 xnatuploader-1.1.2/src/xnatuploader/workbook.py
--rwxr-xr-x   0 mike       (501) staff       (20)    17102 2023-05-29 06:43:19.000000 xnatuploader-1.1.2/src/xnatuploader/xnatuploader.py
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2023-05-29 06:58:47.586319 xnatuploader-1.1.2/src/xnatuploader.egg-info/
--rw-r--r--   0 mike       (501) staff       (20)    14372 2023-05-29 06:58:47.000000 xnatuploader-1.1.2/src/xnatuploader.egg-info/PKG-INFO
--rw-r--r--   0 mike       (501) staff       (20)      615 2023-05-29 06:58:47.000000 xnatuploader-1.1.2/src/xnatuploader.egg-info/SOURCES.txt
--rw-r--r--   0 mike       (501) staff       (20)        1 2023-05-29 06:58:47.000000 xnatuploader-1.1.2/src/xnatuploader.egg-info/dependency_links.txt
--rw-r--r--   0 mike       (501) staff       (20)       64 2023-05-29 06:58:47.000000 xnatuploader-1.1.2/src/xnatuploader.egg-info/entry_points.txt
--rw-r--r--   0 mike       (501) staff       (20)       98 2023-05-29 06:58:47.000000 xnatuploader-1.1.2/src/xnatuploader.egg-info/requires.txt
--rw-r--r--   0 mike       (501) staff       (20)       13 2023-05-29 06:58:47.000000 xnatuploader-1.1.2/src/xnatuploader.egg-info/top_level.txt
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2023-05-29 06:58:47.589486 xnatuploader-1.1.2/tests/
--rw-r--r--   0 mike       (501) staff       (20)      289 2022-11-17 02:49:16.000000 xnatuploader-1.1.2/tests/test_config.py
--rw-r--r--   0 mike       (501) staff       (20)     3117 2023-02-16 03:04:29.000000 xnatuploader-1.1.2/tests/test_matcher.py
--rw-r--r--   0 mike       (501) staff       (20)     5387 2023-05-29 06:43:19.000000 xnatuploader-1.1.2/tests/test_scan.py
--rw-r--r--   0 mike       (501) staff       (20)     5359 2023-05-29 06:43:19.000000 xnatuploader-1.1.2/tests/test_upload.py
+drwxr-xr-x   0 mike       (501) staff       (20)        0 2023-07-19 05:36:13.982586 xnatuploader-1.1.3/
+-rw-r--r--   0 mike       (501) staff       (20)    14372 2023-07-19 05:36:13.982877 xnatuploader-1.1.3/PKG-INFO
+-rw-r--r--   0 mike       (501) staff       (20)    13805 2023-02-16 03:37:24.000000 xnatuploader-1.1.3/README.md
+-rw-r--r--   0 mike       (501) staff       (20)       93 2022-06-16 06:56:16.000000 xnatuploader-1.1.3/pyproject.toml
+-rw-r--r--   0 mike       (501) staff       (20)     1104 2023-07-19 05:36:13.984877 xnatuploader-1.1.3/setup.cfg
+drwxr-xr-x   0 mike       (501) staff       (20)        0 2023-07-19 05:36:13.966743 xnatuploader-1.1.3/src/
+drwxr-xr-x   0 mike       (501) staff       (20)        0 2023-07-19 05:36:13.974344 xnatuploader-1.1.3/src/xnatuploader/
+-rw-r--r--   0 mike       (501) staff       (20)       72 2022-06-16 06:56:16.000000 xnatuploader-1.1.3/src/xnatuploader/__init__.py
+-rw-r--r--   0 mike       (501) staff       (20)      283 2023-05-25 02:08:09.000000 xnatuploader-1.1.3/src/xnatuploader/dataclass.py
+-rw-r--r--   0 mike       (501) staff       (20)     3202 2023-07-10 03:19:23.000000 xnatuploader-1.1.3/src/xnatuploader/dicoms.py
+-rw-r--r--   0 mike       (501) staff       (20)    15000 2023-05-29 06:43:19.000000 xnatuploader-1.1.3/src/xnatuploader/matcher.py
+-rw-r--r--   0 mike       (501) staff       (20)     8947 2023-03-15 03:09:46.000000 xnatuploader-1.1.3/src/xnatuploader/put.py
+-rw-r--r--   0 mike       (501) staff       (20)     6991 2023-07-19 05:32:22.000000 xnatuploader-1.1.3/src/xnatuploader/upload.py
+-rw-r--r--   0 mike       (501) staff       (20)      203 2023-04-05 06:48:06.000000 xnatuploader-1.1.3/src/xnatuploader/userdict.py
+-rw-r--r--   0 mike       (501) staff       (20)     4070 2023-07-19 05:32:22.000000 xnatuploader-1.1.3/src/xnatuploader/workbook.py
+-rwxr-xr-x   0 mike       (501) staff       (20)    17511 2023-07-19 05:32:22.000000 xnatuploader-1.1.3/src/xnatuploader/xnatuploader.py
+drwxr-xr-x   0 mike       (501) staff       (20)        0 2023-07-19 05:36:13.979163 xnatuploader-1.1.3/src/xnatuploader.egg-info/
+-rw-r--r--   0 mike       (501) staff       (20)    14372 2023-07-19 05:36:13.000000 xnatuploader-1.1.3/src/xnatuploader.egg-info/PKG-INFO
+-rw-r--r--   0 mike       (501) staff       (20)      615 2023-07-19 05:36:13.000000 xnatuploader-1.1.3/src/xnatuploader.egg-info/SOURCES.txt
+-rw-r--r--   0 mike       (501) staff       (20)        1 2023-07-19 05:36:13.000000 xnatuploader-1.1.3/src/xnatuploader.egg-info/dependency_links.txt
+-rw-r--r--   0 mike       (501) staff       (20)       64 2023-07-19 05:36:13.000000 xnatuploader-1.1.3/src/xnatuploader.egg-info/entry_points.txt
+-rw-r--r--   0 mike       (501) staff       (20)      123 2023-07-19 05:36:13.000000 xnatuploader-1.1.3/src/xnatuploader.egg-info/requires.txt
+-rw-r--r--   0 mike       (501) staff       (20)       13 2023-07-19 05:36:13.000000 xnatuploader-1.1.3/src/xnatuploader.egg-info/top_level.txt
+drwxr-xr-x   0 mike       (501) staff       (20)        0 2023-07-19 05:36:13.982001 xnatuploader-1.1.3/tests/
+-rw-r--r--   0 mike       (501) staff       (20)      289 2022-11-17 02:49:16.000000 xnatuploader-1.1.3/tests/test_config.py
+-rw-r--r--   0 mike       (501) staff       (20)     3117 2023-02-16 03:04:29.000000 xnatuploader-1.1.3/tests/test_matcher.py
+-rw-r--r--   0 mike       (501) staff       (20)     5387 2023-05-29 06:43:19.000000 xnatuploader-1.1.3/tests/test_scan.py
+-rw-r--r--   0 mike       (501) staff       (20)     5576 2023-07-19 05:32:22.000000 xnatuploader-1.1.3/tests/test_upload.py
```

### Comparing `xnatuploader-1.1.2/PKG-INFO` & `xnatuploader-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xnatuploader
-Version: 1.1.2
+Version: 1.1.3
 Summary: CLI tool for uploading multiple files to XNAT
 Home-page: https://github.com/SydneyInformaticsHub/xnatuploader
 Author: Mike Lynch
 Author-email: m.lynch@sydney.edu.au
 Project-URL: Bug Tracker, https://github.com/SydneyInformaticsHub/xnatuploader/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `xnatuploader-1.1.2/README.md` & `xnatuploader-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `xnatuploader-1.1.2/setup.cfg` & `xnatuploader-1.1.3/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = xnatuploader
-version = 1.1.2
+version = 1.1.3
 author = Mike Lynch
 author_email = m.lynch@sydney.edu.au
 description = CLI tool for uploading multiple files to XNAT
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/SydneyInformaticsHub/xnatuploader
 project_urls = 
@@ -20,14 +20,15 @@
 	= src
 packages = find:
 install_requires = 
 	xnatutils
 	xnat == 0.4.3
 	openpyxl >= 3.0.10
 	pydicom >= 2.3.0
+	dicom-anonymizer >= 1.0.11
 	tqdm
 	click
 
 [options.extras_require]
 test = 
 	pytest
 	xnat4tests >= 0.3.2
```

### Comparing `xnatuploader-1.1.2/src/xnatuploader/dicoms.py` & `xnatuploader-1.1.3/src/xnatuploader/dicoms.py`

 * *Files identical despite different names*

### Comparing `xnatuploader-1.1.2/src/xnatuploader/matcher.py` & `xnatuploader-1.1.3/src/xnatuploader/matcher.py`

 * *Files identical despite different names*

### Comparing `xnatuploader-1.1.2/src/xnatuploader/put.py` & `xnatuploader-1.1.3/src/xnatuploader/put.py`

 * *Files identical despite different names*

### Comparing `xnatuploader-1.1.2/src/xnatuploader/upload.py` & `xnatuploader-1.1.3/src/xnatuploader/upload.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 import xnatuploader.put
 import os.path
 import logging
+from pathlib import Path
+import tempfile
+from pydicom.tag import Tag
+from dicomanonymizer import anonymize, keep
 from dataclasses import dataclass
 
 logger = logging.getLogger(__name__)
 
+ANONRULES = {(0x0008, 0x0020): keep}
+
 
 @dataclass
 class Upload:
     """
     An Upload represents a session for a single patient and visit, which may
     have more than one file.
 
@@ -63,35 +69,50 @@
             scan_id=self.series_number,
             #            date=self.date,
             modality=self.modality,
             create_session=self.new_session,
             connection=xnat_session,
         )
 
-    def upload(self, files, overwrite=False):
+    def upload(self, files, overwrite=False, anon_rules=None):
         """
-        Upload a batch of files to the current resource and checks their
-        digests
+        Makes anonymised copies of a batch of files, uploads the anonymised
+        versions, checks the digests against the anonymised versions and then
+        cleans up. Returns a dict of success / error by the original filename
 
         Args:
             files: list of Matchfile
             overwrite: boolean
+            anon_rules: None or dict of anonymisation rules
         Returns:
             dict of { str: str } with a status message, "success" or an error
         ---
         """
-        for file in files:
-            fname = os.path.basename(file.file)
-            if fname in self.resource.files:
-                if overwrite:
-                    self.resource.files[fname].delete()  # I am not sure if this is good
-            self.resource.upload(file.file, fname)
-        return self.check_digests(files)
+        if anon_rules is None:
+            rules = {}
+        else:
+            rules = anon_rules
+        with tempfile.TemporaryDirectory() as tempdir:
+            for file in files:
+                fname = os.path.basename(file.file)
+                anon_file = str(Path(tempdir) / fname)
+                try:
+                    logger.debug(f"Anonymizing {file.file} -> {anon_file}")
+                    anonymize(file.file, anon_file, rules, True)
+                except Exception as e:
+                    logger.error(f"Error while anonymizing {file.file}")
+                    logger.error(str(e))
+                    return
+                if fname in self.resource.files:
+                    if overwrite:
+                        self.resource.files[fname].delete()
+                self.resource.upload(anon_file, fname)
+            return self.check_digests(tempdir, files)
 
-    def check_digests(self, files):
+    def check_digests(self, tempdir, files):
         """Check the digests of a batch of files, and returns a hash-by-filename
         of success or failure
         """
         result = self.xnat_session.get(self.resource.uri + "/files")
         if result.status_code != 200:
             logger.error(
                 f"Request for digests at {self.resource.uri} returned status {result.status_code}"
@@ -100,23 +121,24 @@
         else:
             digests = {
                 f["Name"]: f["digest"] for f in result.json()["ResultSet"]["Result"]
             }
         status = {}
         for file in files:
             xnat_filename = os.path.basename(file.file)
+            anon_file = Path(tempdir) / xnat_filename
             if xnat_filename not in digests:
                 status[
                     file.file
                 ] = f"File {file.file} {xnat_filename} not found in digests"
                 logger.error(status[file.file])
                 logger.error(digests)
             else:
                 remote_digest = digests[xnat_filename]
-                local_digest = xnatuploader.put.calculate_checksum(file.file)
+                local_digest = xnatuploader.put.calculate_checksum(anon_file)
                 if local_digest != remote_digest:
                     status[
                         file.file
                     ] = f"Digest mismatch {local_digest} {remote_digest}"
                     logger.error(file.file + ": " + status[file.file])
                 else:
                     status[file.file] = "success"
@@ -148,7 +170,26 @@
             uri = f"/data/projects/{project}/subjects/{subject}/experiments/{session}"
             xnat_session.put(f"{uri}?pullDataFromHeaders=true")
             xnat_session.put(f"{uri}?fixScanTypes=true")
             xnat_session.put(f"{uri}?triggerPipelines=true")
         except Exception as e:
             logger.info("Error while triggering metadata extraction / pipelines")
             logger.info(str(e))
+
+
+def parse_allow_fields(allow_fields):
+    """Takes a list of fields which we don't want stripped from the DICOMs
+    and tries to convert them to a custom ruleset for dicom-anonymiser. Raises
+    a ValueError on any tags which aren't in the DICOM spec."""
+
+    rules = {}
+
+    if allow_fields is not None:
+        for keyword in allow_fields.split(","):
+            try:
+                tag = Tag(keyword)
+                rules[(tag.group, tag.elem)] = keep
+            except ValueError:
+                raise ValueError(
+                    f"Unknown DICOM keyword {keyword} in AllowFields configuration"
+                )
+    return rules
```

### Comparing `xnatuploader-1.1.2/src/xnatuploader/workbook.py` & `xnatuploader-1.1.3/src/xnatuploader/workbook.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,16 @@
     ws["B12"] = "Dataset"
     ws["C12"] = "Directory"
     ws["A14"] = "XNAT"
     ws["B14"] = "Project"
     ws["C14"] = "Test001"
     ws["B15"] = "Server"
     ws["C15"] = "http://localhost:8080"
+    ws["B16"] = "AllowFields"
+    ws["C16"] = "AccessionNumber"
     wb.save(file)
 
 
 def add_filesheet(wb, matcher, debug):
     """
     Adds a worksheet to a workbook with headers from the matcher object
     and niceties such as a wider column for the file names.
@@ -113,14 +115,17 @@
             section = row[0].value.lower()
         var = row[1].value
         if var is not None and section is not None:
             if section not in config:
                 config[section] = OrderedDict()
             cells = [cell.value for cell in row[2:] if cell.value is not None]
             if section == "xnat":
-                config[section][var] = cells[0]
+                try:
+                    config[section][var] = cells[0]
+                except IndexError:
+                    config[section][var] = None
             else:
                 config[section][var] = cells
     missing = [s for s in sections if s not in config]
     if len(missing) > 0:
         raise WorkbookError(f"Missing config sections: {missing}")
     return config
```

### Comparing `xnatuploader-1.1.2/src/xnatuploader/xnatuploader.py` & `xnatuploader-1.1.3/src/xnatuploader/xnatuploader.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 __version__ = version("xnatuploader")
 
 from openpyxl import load_workbook
 
 from xnatuploader.matcher import Matcher
 from xnatuploader.dicoms import dicom_extractor, XNATFileMatch, SPREADSHEET_FIELDS
 from xnatuploader.workbook import new_workbook, add_filesheet, load_config
-from xnatuploader.upload import Upload, trigger_pipelines
+from xnatuploader.upload import Upload, trigger_pipelines, parse_allow_fields
 
 from xnatutils.base import sanitize_re
 
 FILE_COLUMN_WIDTH = 50
 
 DEBUG_MAX = 10
 
@@ -102,14 +102,15 @@
 
 
 def upload(
     xnat_session,
     matcher,
     project,
     spreadsheet,
+    anon_rules,
     test=False,
     overwrite=False,
     nopipeline=False,
 ):
     """
     Load an Excel spreadsheet created with scan and upload the files which the user
     has marked for upload, and which haven't been uploaded yet. Keeps track of
@@ -156,15 +157,19 @@
         for session_scan, upload in tqdm(uploads.items(), desc="Sessions"):
             logger.debug(f"Uploading {session_scan}")
             try:
                 upload.start_upload(xnat_session, project)
                 for file in tqdm(upload.files, desc=session_scan):
                     logger.debug(f"Uploading {file.file}")
                     try:
-                        status = upload.upload([file], overwrite=overwrite)
+                        status = upload.upload(
+                            [file],
+                            overwrite=overwrite,
+                            anon_rules=anon_rules,
+                        )
                         file.status = status[file.file]
                     except KeyboardInterrupt:
                         if click.confirm(CONFIRM_KEYBOARD_QUIT_MSG):
                             keyboard_quit = True
                             logger.warning(
                                 f"KeyboardInterrupt in file loop {file.file}"
                             )
@@ -499,22 +504,27 @@
             args.spreadsheet,
             include_unmatched=args.unmatched,
             debug=args.debug,
         )
     else:
         server = opt_or_config(args, config["xnat"], "Server")
         project = opt_or_config(args, config["xnat"], "Project")
+        # not using opt_or_config for AllowFields as it's not mandatory
+        anon_rules = {}
+        if "AllowFields" in config["xnat"]:
+            anon_rules = parse_allow_fields(config["xnat"]["AllowFields"])
         logger.debug(f"Server = {server}")
         logger.debug(f"Project = {project}")
         xnat_session = xnatutils.base.connect(server)
         upload(
             xnat_session,
             matcher,
             project,
             args.spreadsheet,
+            anon_rules,
             args.test,
             args.overwrite,
             args.nopipeline,
         )
 
 
 if __name__ == "__main__":
```

### Comparing `xnatuploader-1.1.2/src/xnatuploader.egg-info/PKG-INFO` & `xnatuploader-1.1.3/src/xnatuploader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xnatuploader
-Version: 1.1.2
+Version: 1.1.3
 Summary: CLI tool for uploading multiple files to XNAT
 Home-page: https://github.com/SydneyInformaticsHub/xnatuploader
 Author: Mike Lynch
 Author-email: m.lynch@sydney.edu.au
 Project-URL: Bug Tracker, https://github.com/SydneyInformaticsHub/xnatuploader/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `xnatuploader-1.1.2/src/xnatuploader.egg-info/SOURCES.txt` & `xnatuploader-1.1.3/src/xnatuploader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `xnatuploader-1.1.2/tests/test_matcher.py` & `xnatuploader-1.1.3/tests/test_matcher.py`

 * *Files identical despite different names*

### Comparing `xnatuploader-1.1.2/tests/test_scan.py` & `xnatuploader-1.1.3/tests/test_scan.py`

 * *Files identical despite different names*

### Comparing `xnatuploader-1.1.2/tests/test_upload.py` & `xnatuploader-1.1.3/tests/test_upload.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from pathlib import Path
 
 from xnatuploader.xnatuploader import scan, upload
 from xnatuploader.matcher import Matcher
 from xnatuploader.dicoms import dicom_extractor, XNATFileMatch, SPREADSHEET_FIELDS
 from xnatuploader.workbook import new_workbook
+from xnatuploader.upload import parse_allow_fields
 
 
 @pytest.mark.parametrize("source_dir", ["basic", "bad_paths"])
 def test_upload_from_spreadsheet(source_dir, xnat_connection, tmp_path, test_files):
     test_config = test_files[source_dir]["config"]
     test_dir = test_files[source_dir]["dir"]
     with open(test_config, "r") as fh:
@@ -22,25 +23,26 @@
         matcher = Matcher(
             config["paths"],
             config["mappings"],
             SPREADSHEET_FIELDS,
             dicom_extractor,
             XNATFileMatch,
         )
+        anon_rules = parse_allow_fields(config["xnat"]["AllowFields"])
     project = xnat_connection.classes.ProjectData(
         parent=xnat_connection,
         name="Test_" + source_dir,
     )
     log_scanned = tmp_path / "log_scanned.xlsx"
     log_uploaded = tmp_path / "log_uploaded.xlsx"
     downloads = tmp_path / "downloads"
     new_workbook(log_scanned)
     scan(matcher, Path(test_dir), log_scanned)
     shutil.copy(log_scanned, log_uploaded)
-    upload(xnat_connection, matcher, project.name, log_uploaded)
+    upload(xnat_connection, matcher, project.name, log_uploaded, anon_rules)
     uploaded_wb = load_workbook(log_uploaded)
     uploaded_ws = uploaded_wb["Files"]
     uploads = {}
     for row in uploaded_ws.values:
         if row[0] != "Recipe":
             upload_row = matcher.from_spreadsheet(row)
             if upload_row.selected:
@@ -107,14 +109,15 @@
         matcher = Matcher(
             config["paths"],
             config["mappings"],
             SPREADSHEET_FIELDS,
             dicom_extractor,
             XNATFileMatch,
         )
+        anon_rules = parse_allow_fields(config["xnat"]["AllowFields"])
     log_scanned = tmp_path / "log_scanned.xlsx"
     log_uploaded = tmp_path / "log_uploaded.xlsx"
     new_workbook(log_scanned)
     scan(matcher, Path(basic["dir"]), log_scanned)
     scanned_wb = load_workbook(log_scanned)
     ws = scanned_wb["Files"]
     # change the third filename to trigger an error
@@ -128,15 +131,15 @@
             if m.selected:
                 c += 1
                 if c == 3:
                     bad_file = ws.cell(i, 2).value + "broken"
                     ws.cell(i, 2).value = bad_file
 
     scanned_wb.save(log_uploaded)
-    upload(xnat_connection, matcher, project.name, log_uploaded)
+    upload(xnat_connection, matcher, project.name, log_uploaded, anon_rules)
     uploads = {}
     uploaded_wb = load_workbook(log_uploaded)
     uploaded_ws = uploaded_wb["Files"]
     for row in uploaded_ws.values:
         if row[0] != "Recipe":
             upload_row = matcher.from_spreadsheet(row)
             if upload_row.selected:
```

