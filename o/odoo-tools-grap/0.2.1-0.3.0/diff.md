# Comparing `tmp/odoo-tools-grap-0.2.1.tar.gz` & `tmp/odoo-tools-grap-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/odoo-tools-grap-0.2.1.tar", last modified: Wed Jun 19 15:57:00 2019, max compression
+gzip compressed data, was "dist/odoo-tools-grap-0.3.0.tar", last modified: Wed Jul 19 15:39:00 2023, max compression
```

## Comparing `odoo-tools-grap-0.2.1.tar` & `odoo-tools-grap-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 sylvain   (1000) sylvain   (1000)        0 2019-06-19 15:57:00.000000 odoo-tools-grap-0.2.1/
-drwxrwxr-x   0 sylvain   (1000) sylvain   (1000)        0 2019-06-19 15:57:00.000000 odoo-tools-grap-0.2.1/odoo_tools/
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)       16 2019-06-19 15:12:43.000000 odoo-tools-grap-0.2.1/odoo_tools/__init__.py
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     4158 2019-06-19 15:13:00.000000 odoo-tools-grap-0.2.1/odoo_tools/__main__.py
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     3818 2019-06-19 15:57:00.000000 odoo-tools-grap-0.2.1/PKG-INFO
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     2529 2019-06-19 15:56:40.000000 odoo-tools-grap-0.2.1/README.rst
-drwxrwxr-x   0 sylvain   (1000) sylvain   (1000)        0 2019-06-19 15:57:00.000000 odoo-tools-grap-0.2.1/odoo_tools_grap.egg-info/
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     3818 2019-06-19 15:57:00.000000 odoo-tools-grap-0.2.1/odoo_tools_grap.egg-info/PKG-INFO
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)        1 2019-06-19 15:57:00.000000 odoo-tools-grap-0.2.1/odoo_tools_grap.egg-info/dependency_links.txt
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)       62 2019-06-19 15:57:00.000000 odoo-tools-grap-0.2.1/odoo_tools_grap.egg-info/entry_points.txt
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)       11 2019-06-19 15:57:00.000000 odoo-tools-grap-0.2.1/odoo_tools_grap.egg-info/top_level.txt
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)       19 2019-06-19 15:57:00.000000 odoo-tools-grap-0.2.1/odoo_tools_grap.egg-info/requires.txt
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)      301 2019-06-19 15:57:00.000000 odoo-tools-grap-0.2.1/odoo_tools_grap.egg-info/SOURCES.txt
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)      865 2019-06-19 15:56:52.000000 odoo-tools-grap-0.2.1/setup.py
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)       38 2019-06-19 15:57:00.000000 odoo-tools-grap-0.2.1/setup.cfg
+drwxrwxr-x   0 sylvain   (1000) sylvain   (1000)        0 2023-07-19 15:39:00.000000 odoo-tools-grap-0.3.0/
+-rw-rw-r--   0 sylvain   (1000) sylvain   (1000)       38 2023-07-19 15:39:00.000000 odoo-tools-grap-0.3.0/setup.cfg
+-rw-rw-r--   0 sylvain   (1000) sylvain   (1000)      865 2023-07-19 15:38:01.000000 odoo-tools-grap-0.3.0/setup.py
+drwxrwxr-x   0 sylvain   (1000) sylvain   (1000)        0 2023-07-19 15:39:00.000000 odoo-tools-grap-0.3.0/odoo_tools/
+-rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     4163 2023-07-19 15:30:25.000000 odoo-tools-grap-0.3.0/odoo_tools/__main__.py
+-rw-rw-r--   0 sylvain   (1000) sylvain   (1000)       16 2023-07-19 15:19:23.000000 odoo-tools-grap-0.3.0/odoo_tools/__init__.py
+-rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     2705 2023-07-19 15:39:00.000000 odoo-tools-grap-0.3.0/PKG-INFO
+drwxrwxr-x   0 sylvain   (1000) sylvain   (1000)        0 2023-07-19 15:39:00.000000 odoo-tools-grap-0.3.0/odoo_tools_grap.egg-info/
+-rw-rw-r--   0 sylvain   (1000) sylvain   (1000)      301 2023-07-19 15:39:00.000000 odoo-tools-grap-0.3.0/odoo_tools_grap.egg-info/SOURCES.txt
+-rw-rw-r--   0 sylvain   (1000) sylvain   (1000)       11 2023-07-19 15:39:00.000000 odoo-tools-grap-0.3.0/odoo_tools_grap.egg-info/top_level.txt
+-rw-rw-r--   0 sylvain   (1000) sylvain   (1000)        1 2023-07-19 15:39:00.000000 odoo-tools-grap-0.3.0/odoo_tools_grap.egg-info/dependency_links.txt
+-rw-rw-r--   0 sylvain   (1000) sylvain   (1000)       19 2023-07-19 15:39:00.000000 odoo-tools-grap-0.3.0/odoo_tools_grap.egg-info/requires.txt
+-rw-rw-r--   0 sylvain   (1000) sylvain   (1000)       62 2023-07-19 15:39:00.000000 odoo-tools-grap-0.3.0/odoo_tools_grap.egg-info/entry_points.txt
+-rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     2705 2023-07-19 15:39:00.000000 odoo-tools-grap-0.3.0/odoo_tools_grap.egg-info/PKG-INFO
+-rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     2323 2023-07-19 15:33:45.000000 odoo-tools-grap-0.3.0/README.rst
```

### Comparing `odoo-tools-grap-0.2.1/odoo_tools/__main__.py` & `odoo-tools-grap-0.3.0/odoo_tools/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import configparser
 import subprocess
 import yaml
 import os
 
 
 def _generate_odoo_config_file(args):
-    input_files = [os.path.join(args.folder, x) for x in args.input_files]
+    input_files = [os.path.join(args.folder, x) for x in args.input_files.split(",")]
     config_repo_file = os.path.join(args.folder, args.config_repo_file)
     output_file = os.path.join(args.folder, args.output_file)
 
     # Read Input Files
     parser = configparser.ConfigParser()
     parser.read(input_files)
 
@@ -95,16 +95,16 @@
     ).completer = argcomplete.completers.FilesCompleter(
         allowednames=('.yaml', '.yml', '.json'), directories=False
     )
 
     main_parser.add_argument(
         '-i', '--input-files',
         dest='input_files',
-        type=list,
-        default=["./common.odoo.cfg", "./custom.odoo.cfg"],
+        type=str,
+        default="./common.odoo.cfg,./custom.odoo.cfg",
         help='Template odoo Config File(s)'
     ).completer = argcomplete.completers.FilesCompleter(
         allowednames=('.cfg'), directories=False
     )
 
     main_parser.add_argument(
         '-o', '--output-file',
```

### Comparing `odoo-tools-grap-0.2.1/README.rst` & `odoo-tools-grap-0.3.0/README.rst`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,25 @@
+===============
+odoo-tools-grap
+===============
+
 .. image:: https://img.shields.io/badge/licence-AGPL--3-blue.svg
     :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
     :alt: License: AGPL-3
+
 .. image:: https://img.shields.io/badge/python-3.6-blue.svg
     :alt: Python support: 3.6
 
-===============
-odoo-tools-grap
-===============
-
 Installation
 ============
 
 .. code-block:: shell
 
-    # Install Stable Source
     pip3 install odoo-tools-grap
 
-    # Or, Install Test source
-    pip3 install odoo-tools-grap\
-        --upgrade\
-        --index-url https://test.pypi.org/simple\
-        --extra-index-url https://pypi.org/simple
-
 Usage
 =====
 
 Diff tools
 ----------
 
 
@@ -57,39 +51,39 @@
 
 .. code-block:: shell
 
     # Pull Code
     git clone https://gitlab.com/grap-rhone-alpes/odoo-tools-grap
     cd odoo-tools-grap
 
-    # Create virtual env and activate it
+    # Create virtual env and activate it
     virtualenv env --python=python3
     . ./env/bin/activate
 
     # Install dependencies
-    pip3 install -r requirements.txt
+    ./env/bin/pip install -r requirements.txt
 
     # Run the script
     python -m odoo_tools COMMAND OPTIONS
 
 Package deployment
 ==================
 
 .. code-block:: shell
 
     pip3 install --upgrade setuptools wheel
     pip3 install  --upgrade twine
 
-    # Generate wheel and package
+    # Generate wheel and package
     python3 setup.py sdist bdist_wheel
 
-    # Push on pyPi Test
+    # Push on pyPi Test
     twine upload --repository-url https://test.pypi.org/legacy/ dist/*
 
-    # Push on pyPi Production
+    # Push on pyPi Production
     twine upload dist/*
 
 Roadmap / Know issues
 =====================
 
 * odoo-tools-grap diff tools will not works in a non french context, because
   a test based on the result of ``git diff`` is hardcoded with french sentence.
```

### Comparing `odoo-tools-grap-0.2.1/setup.py` & `odoo-tools-grap-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # @author: Sylvain LE GAL (https://twitter.com/legalsylvain)
 # License AGPL-3.0 or later (http://www.gnu.org/licenses/agpl.html).
 
 import setuptools
 
 setuptools.setup(
     name="odoo-tools-grap",
-    version="0.2.1",
+    version="0.3.0",
     author="GRAP, Groupement Régional Alimentaire de Proximité",
     author_email="informatique@grap.coop",
     description="Small tools for Odoo",
     long_description=open('README.rst').read(),
     url="https://www.grap.coop",
     packages=['odoo_tools'],
     classifiers=[
```

