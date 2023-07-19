# Comparing `tmp/infusevideo-cli-0.2.2.tar.gz` & `tmp/infusevideo-cli-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infusevideo-cli-0.2.2.tar", last modified: Tue May 24 22:48:29 2022, max compression
+gzip compressed data, was "infusevideo-cli-0.2.3.tar", last modified: Wed Jul 19 14:14:20 2023, max compression
```

## Comparing `infusevideo-cli-0.2.2.tar` & `infusevideo-cli-0.2.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 dataghost  (1000) dataghost  (1000)        0 2022-05-24 22:48:29.974440 infusevideo-cli-0.2.2/
--rw-rw-r--   0 dataghost  (1000) dataghost  (1000)     1096 2022-03-03 13:50:02.000000 infusevideo-cli-0.2.2/LICENSE
--rw-rw-r--   0 dataghost  (1000) dataghost  (1000)     3026 2022-05-24 22:48:29.974440 infusevideo-cli-0.2.2/PKG-INFO
--rw-rw-r--   0 dataghost  (1000) dataghost  (1000)     2345 2022-05-10 11:40:26.000000 infusevideo-cli-0.2.2/README.md
-drwxrwxr-x   0 dataghost  (1000) dataghost  (1000)        0 2022-05-24 22:48:29.974440 infusevideo-cli-0.2.2/infusevideo_cli/
--rw-rw-r--   0 dataghost  (1000) dataghost  (1000)     6035 2022-05-19 23:22:15.000000 infusevideo-cli-0.2.2/infusevideo_cli/__init__.py
--rw-rw-r--   0 dataghost  (1000) dataghost  (1000)       53 2022-02-20 13:52:28.000000 infusevideo-cli-0.2.2/infusevideo_cli/__main__.py
-drwxrwxr-x   0 dataghost  (1000) dataghost  (1000)        0 2022-05-24 22:48:29.974440 infusevideo-cli-0.2.2/infusevideo_cli.egg-info/
--rw-rw-r--   0 dataghost  (1000) dataghost  (1000)     3026 2022-05-24 22:48:29.000000 infusevideo-cli-0.2.2/infusevideo_cli.egg-info/PKG-INFO
--rw-rw-r--   0 dataghost  (1000) dataghost  (1000)      334 2022-05-24 22:48:29.000000 infusevideo-cli-0.2.2/infusevideo_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 dataghost  (1000) dataghost  (1000)        1 2022-05-24 22:48:29.000000 infusevideo-cli-0.2.2/infusevideo_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 dataghost  (1000) dataghost  (1000)       70 2022-05-24 22:48:29.000000 infusevideo-cli-0.2.2/infusevideo_cli.egg-info/entry_points.txt
--rw-rw-r--   0 dataghost  (1000) dataghost  (1000)       53 2022-05-24 22:48:29.000000 infusevideo-cli-0.2.2/infusevideo_cli.egg-info/requires.txt
--rw-rw-r--   0 dataghost  (1000) dataghost  (1000)       16 2022-05-24 22:48:29.000000 infusevideo-cli-0.2.2/infusevideo_cli.egg-info/top_level.txt
--rw-rw-r--   0 dataghost  (1000) dataghost  (1000)       98 2022-03-03 23:16:34.000000 infusevideo-cli-0.2.2/pyproject.toml
--rw-rw-r--   0 dataghost  (1000) dataghost  (1000)      921 2022-05-24 22:48:29.974440 infusevideo-cli-0.2.2/setup.cfg
+drwxrwxr-x   0 dataghost  (1000) dataghost  (1000)        0 2023-07-19 14:14:20.960583 infusevideo-cli-0.2.3/
+-rw-rw-r--   0 dataghost  (1000) dataghost  (1000)     1096 2022-03-03 13:50:02.000000 infusevideo-cli-0.2.3/LICENSE
+-rw-rw-r--   0 dataghost  (1000) dataghost  (1000)     3026 2023-07-19 14:14:20.960583 infusevideo-cli-0.2.3/PKG-INFO
+-rw-rw-r--   0 dataghost  (1000) dataghost  (1000)     2345 2022-05-10 11:40:26.000000 infusevideo-cli-0.2.3/README.md
+drwxrwxr-x   0 dataghost  (1000) dataghost  (1000)        0 2023-07-19 14:14:20.960583 infusevideo-cli-0.2.3/infusevideo_cli/
+-rw-rw-r--   0 dataghost  (1000) dataghost  (1000)     6049 2023-05-15 08:26:03.000000 infusevideo-cli-0.2.3/infusevideo_cli/__init__.py
+-rw-rw-r--   0 dataghost  (1000) dataghost  (1000)       53 2022-02-20 13:52:28.000000 infusevideo-cli-0.2.3/infusevideo_cli/__main__.py
+drwxrwxr-x   0 dataghost  (1000) dataghost  (1000)        0 2023-07-19 14:14:20.960583 infusevideo-cli-0.2.3/infusevideo_cli.egg-info/
+-rw-rw-r--   0 dataghost  (1000) dataghost  (1000)     3026 2023-07-19 14:14:20.000000 infusevideo-cli-0.2.3/infusevideo_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 dataghost  (1000) dataghost  (1000)      334 2023-07-19 14:14:20.000000 infusevideo-cli-0.2.3/infusevideo_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 dataghost  (1000) dataghost  (1000)        1 2023-07-19 14:14:20.000000 infusevideo-cli-0.2.3/infusevideo_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 dataghost  (1000) dataghost  (1000)       70 2023-07-19 14:14:20.000000 infusevideo-cli-0.2.3/infusevideo_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 dataghost  (1000) dataghost  (1000)       56 2023-07-19 14:14:20.000000 infusevideo-cli-0.2.3/infusevideo_cli.egg-info/requires.txt
+-rw-rw-r--   0 dataghost  (1000) dataghost  (1000)       16 2023-07-19 14:14:20.000000 infusevideo-cli-0.2.3/infusevideo_cli.egg-info/top_level.txt
+-rw-rw-r--   0 dataghost  (1000) dataghost  (1000)       98 2022-03-03 23:16:34.000000 infusevideo-cli-0.2.3/pyproject.toml
+-rw-rw-r--   0 dataghost  (1000) dataghost  (1000)      924 2023-07-19 14:14:20.960583 infusevideo-cli-0.2.3/setup.cfg
```

### Comparing `infusevideo-cli-0.2.2/LICENSE` & `infusevideo-cli-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `infusevideo-cli-0.2.2/PKG-INFO` & `infusevideo-cli-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infusevideo-cli
-Version: 0.2.2
+Version: 0.2.3
 Summary: Command-line utility to interact with the Infuse Video API
 Home-page: https://www.infuse.video
 Author: Infuse Video
 Author-email: support@infuse.video
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `infusevideo-cli-0.2.2/README.md` & `infusevideo-cli-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `infusevideo-cli-0.2.2/infusevideo_cli/__init__.py` & `infusevideo-cli-0.2.3/infusevideo_cli/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,14 +162,15 @@
 			fileName=options.file,
 			fileField=options.fileField,
 		)
 		print(response)
 	except infusevideo.errors.ApiError as e:
 		print(f"!!! Request returned error code {e.response.code}", file=sys.stderr)
 		print(e)
+		sys.exit(1)
 	except infusevideo.errors.RequestedScopeError as e:
 		print(f"Authorization error: {e}", file=sys.stderr)
 		print(f"You can refresh your token by executing:", file=sys.stderr)
 		print(f"    {sys.argv[0]} --clear-token --profile {e.profile.name}", file=sys.stderr)
 		print(f"and then trying again.", file=sys.stderr)
 		sys.exit(1)
 	except infusevideo.errors.AuthorizationError as e:
```

### Comparing `infusevideo-cli-0.2.2/infusevideo_cli.egg-info/PKG-INFO` & `infusevideo-cli-0.2.3/infusevideo_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infusevideo-cli
-Version: 0.2.2
+Version: 0.2.3
 Summary: Command-line utility to interact with the Infuse Video API
 Home-page: https://www.infuse.video
 Author: Infuse Video
 Author-email: support@infuse.video
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `infusevideo-cli-0.2.2/setup.cfg` & `infusevideo-cli-0.2.3/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = infusevideo-cli
-version = 0.2.2
+version = 0.2.3
 author = Infuse Video
 author_email = support@infuse.video
 license = MIT
 description = Command-line utility to interact with the Infuse Video API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://www.infuse.video
@@ -21,16 +21,16 @@
 [options]
 python_requires = >=3.9
 package_dir = 
 	infusevideo_cli = infusevideo_cli
 packages = infusevideo_cli
 install_requires = 
 	docopt==0.6.2
-	pydantic>=1.9.0
-	infusevideo-sdk>=0.2.2
+	pydantic>=1.9.0,<2
+	infusevideo-sdk>=0.2.3
 
 [options.entry_points]
 console_scripts = 
 	ivc = infusevideo_cli:cli
 	ivs = infusevideo_cli:cli
 
 [egg_info]
```

