# Comparing `tmp/mama-0.8.1.tar.gz` & `tmp/mama-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mama-0.8.1.tar", last modified: Tue Jul 18 11:14:33 2023, max compression
+gzip compressed data, was "mama-0.8.2.tar", last modified: Tue Jul 18 21:51:18 2023, max compression
```

## Comparing `mama-0.8.1.tar` & `mama-0.8.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2023-07-18 11:14:33.541546 mama-0.8.1/
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1062 2022-10-15 13:42:02.000000 mama-0.8.1/LICENSE
--rw-r--r--   0 jorma     (1000) jorma     (1000)    12164 2023-07-18 11:14:33.541546 mama-0.8.1/PKG-INFO
--rw-r--r--   0 jorma     (1000) jorma     (1000)    11354 2023-07-17 21:28:34.000000 mama-0.8.1/README.md
-drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2023-07-18 11:14:33.541546 mama-0.8.1/mama/
--rw-r--r--   0 jorma     (1000) jorma     (1000)      141 2022-10-15 12:52:32.000000 mama-0.8.1/mama/__init__.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    12572 2023-03-08 20:41:13.000000 mama-0.8.1/mama/artifactory.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    38745 2023-07-17 19:15:48.000000 mama-0.8.1/mama/build_config.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    23348 2023-07-14 21:51:07.000000 mama-0.8.1/mama/build_dependency.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    50914 2023-07-18 11:13:23.000000 mama-0.8.1/mama/build_target.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    13639 2023-07-17 13:34:28.000000 mama-0.8.1/mama/cmake_configure.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    14557 2023-07-17 12:51:12.000000 mama-0.8.1/mama/dependency_chain.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     5368 2022-10-14 21:28:27.000000 mama-0.8.1/mama/init_project.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    11372 2023-07-17 12:54:02.000000 mama-0.8.1/mama/main.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1796 2022-10-14 21:35:20.000000 mama-0.8.1/mama/msbuild.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     8133 2023-07-18 10:47:43.000000 mama-0.8.1/mama/package.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     6773 2023-03-08 20:52:02.000000 mama-0.8.1/mama/papa_deploy.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1732 2023-01-31 19:23:36.000000 mama-0.8.1/mama/parse_mamafile.py
-drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2023-07-18 11:14:33.541546 mama-0.8.1/mama/platforms/
--rw-r--r--   0 jorma     (1000) jorma     (1000)        0 2023-02-10 12:13:25.000000 mama-0.8.1/mama/platforms/__init__.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     3348 2023-07-17 21:12:25.000000 mama-0.8.1/mama/platforms/mips.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     4765 2023-07-17 19:14:06.000000 mama-0.8.1/mama/platforms/oclea.py
-drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2023-07-18 11:14:33.541546 mama-0.8.1/mama/types/
--rw-r--r--   0 jorma     (1000) jorma     (1000)        0 2022-10-14 22:47:55.000000 mama-0.8.1/mama/types/__init__.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1051 2023-01-31 19:23:36.000000 mama-0.8.1/mama/types/artifactory_pkg.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)      789 2022-10-13 07:46:30.000000 mama-0.8.1/mama/types/asset.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)      830 2023-01-31 19:23:36.000000 mama-0.8.1/mama/types/dep_source.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    12615 2023-07-14 21:38:06.000000 mama-0.8.1/mama/types/git.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1065 2022-10-13 16:33:15.000000 mama-0.8.1/mama/types/local_source.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    15932 2023-07-18 10:46:30.000000 mama-0.8.1/mama/util.py
-drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2023-07-18 11:14:33.541546 mama-0.8.1/mama/utils/
--rw-r--r--   0 jorma     (1000) jorma     (1000)        0 2022-10-14 22:47:54.000000 mama-0.8.1/mama/utils/__init__.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1795 2023-07-18 10:55:23.000000 mama-0.8.1/mama/utils/gdb.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)      922 2023-07-18 10:56:31.000000 mama-0.8.1/mama/utils/gtest.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1038 2022-10-14 18:37:11.000000 mama-0.8.1/mama/utils/nonblocking_io.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1002 2023-07-18 10:52:29.000000 mama-0.8.1/mama/utils/run.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     9784 2023-07-18 10:24:21.000000 mama-0.8.1/mama/utils/sub_process.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1439 2023-03-06 14:41:17.000000 mama-0.8.1/mama/utils/system.py
-drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2023-07-18 11:14:33.541546 mama-0.8.1/mama.egg-info/
--rw-r--r--   0 jorma     (1000) jorma     (1000)    12164 2023-07-18 11:14:33.000000 mama-0.8.1/mama.egg-info/PKG-INFO
--rw-r--r--   0 jorma     (1000) jorma     (1000)      849 2023-07-18 11:14:33.000000 mama-0.8.1/mama.egg-info/SOURCES.txt
--rw-r--r--   0 jorma     (1000) jorma     (1000)        1 2023-07-18 11:14:33.000000 mama-0.8.1/mama.egg-info/dependency_links.txt
--rw-r--r--   0 jorma     (1000) jorma     (1000)       40 2023-07-18 11:14:33.000000 mama-0.8.1/mama.egg-info/entry_points.txt
--rw-r--r--   0 jorma     (1000) jorma     (1000)       76 2023-07-18 11:14:33.000000 mama-0.8.1/mama.egg-info/requires.txt
--rw-r--r--   0 jorma     (1000) jorma     (1000)        5 2023-07-18 11:14:33.000000 mama-0.8.1/mama.egg-info/top_level.txt
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1181 2023-07-18 11:13:12.000000 mama-0.8.1/pyproject.toml
--rw-r--r--   0 jorma     (1000) jorma     (1000)       38 2023-07-18 11:14:33.541546 mama-0.8.1/setup.cfg
+drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2023-07-18 21:51:18.573703 mama-0.8.2/
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1062 2022-10-15 13:42:02.000000 mama-0.8.2/LICENSE
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    12164 2023-07-18 21:51:18.573703 mama-0.8.2/PKG-INFO
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    11354 2023-07-17 21:28:34.000000 mama-0.8.2/README.md
+drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2023-07-18 21:51:18.563703 mama-0.8.2/mama/
+-rw-r--r--   0 jorma     (1000) jorma     (1000)      141 2022-10-15 12:52:32.000000 mama-0.8.2/mama/__init__.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    12572 2023-03-08 20:41:13.000000 mama-0.8.2/mama/artifactory.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    38745 2023-07-17 19:15:48.000000 mama-0.8.2/mama/build_config.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    23348 2023-07-14 21:51:07.000000 mama-0.8.2/mama/build_dependency.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    51585 2023-07-18 14:39:21.000000 mama-0.8.2/mama/build_target.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    13639 2023-07-17 13:34:28.000000 mama-0.8.2/mama/cmake_configure.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    14557 2023-07-17 12:51:12.000000 mama-0.8.2/mama/dependency_chain.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     5368 2022-10-14 21:28:27.000000 mama-0.8.2/mama/init_project.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    11372 2023-07-17 12:54:02.000000 mama-0.8.2/mama/main.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1796 2022-10-14 21:35:20.000000 mama-0.8.2/mama/msbuild.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     8133 2023-07-18 10:47:43.000000 mama-0.8.2/mama/package.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     6773 2023-03-08 20:52:02.000000 mama-0.8.2/mama/papa_deploy.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1732 2023-01-31 19:23:36.000000 mama-0.8.2/mama/parse_mamafile.py
+drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2023-07-18 21:51:18.563703 mama-0.8.2/mama/platforms/
+-rw-r--r--   0 jorma     (1000) jorma     (1000)        0 2023-02-10 12:13:25.000000 mama-0.8.2/mama/platforms/__init__.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     3348 2023-07-17 21:12:25.000000 mama-0.8.2/mama/platforms/mips.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     4765 2023-07-17 19:14:06.000000 mama-0.8.2/mama/platforms/oclea.py
+drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2023-07-18 21:51:18.563703 mama-0.8.2/mama/types/
+-rw-r--r--   0 jorma     (1000) jorma     (1000)        0 2022-10-14 22:47:55.000000 mama-0.8.2/mama/types/__init__.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1051 2023-01-31 19:23:36.000000 mama-0.8.2/mama/types/artifactory_pkg.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)      789 2022-10-13 07:46:30.000000 mama-0.8.2/mama/types/asset.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)      830 2023-01-31 19:23:36.000000 mama-0.8.2/mama/types/dep_source.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    12615 2023-07-14 21:38:06.000000 mama-0.8.2/mama/types/git.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1065 2022-10-13 16:33:15.000000 mama-0.8.2/mama/types/local_source.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    15932 2023-07-18 10:46:30.000000 mama-0.8.2/mama/util.py
+drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2023-07-18 21:51:18.573703 mama-0.8.2/mama/utils/
+-rw-r--r--   0 jorma     (1000) jorma     (1000)        0 2022-10-14 22:47:54.000000 mama-0.8.2/mama/utils/__init__.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1636 2023-07-18 13:44:04.000000 mama-0.8.2/mama/utils/gdb.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)      922 2023-07-18 10:56:31.000000 mama-0.8.2/mama/utils/gtest.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1038 2022-10-14 18:37:11.000000 mama-0.8.2/mama/utils/nonblocking_io.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     2905 2023-07-18 14:08:12.000000 mama-0.8.2/mama/utils/run.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     9784 2023-07-18 14:07:49.000000 mama-0.8.2/mama/utils/sub_process.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1439 2023-03-06 14:41:17.000000 mama-0.8.2/mama/utils/system.py
+drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2023-07-18 21:51:18.563703 mama-0.8.2/mama.egg-info/
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    12164 2023-07-18 21:51:18.000000 mama-0.8.2/mama.egg-info/PKG-INFO
+-rw-r--r--   0 jorma     (1000) jorma     (1000)      849 2023-07-18 21:51:18.000000 mama-0.8.2/mama.egg-info/SOURCES.txt
+-rw-r--r--   0 jorma     (1000) jorma     (1000)        1 2023-07-18 21:51:18.000000 mama-0.8.2/mama.egg-info/dependency_links.txt
+-rw-r--r--   0 jorma     (1000) jorma     (1000)       40 2023-07-18 21:51:18.000000 mama-0.8.2/mama.egg-info/entry_points.txt
+-rw-r--r--   0 jorma     (1000) jorma     (1000)       76 2023-07-18 21:51:18.000000 mama-0.8.2/mama.egg-info/requires.txt
+-rw-r--r--   0 jorma     (1000) jorma     (1000)        5 2023-07-18 21:51:18.000000 mama-0.8.2/mama.egg-info/top_level.txt
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1181 2023-07-18 21:50:37.000000 mama-0.8.2/pyproject.toml
+-rw-r--r--   0 jorma     (1000) jorma     (1000)       38 2023-07-18 21:51:18.573703 mama-0.8.2/setup.cfg
```

### Comparing `mama-0.8.1/LICENSE` & `mama-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mama-0.8.1/PKG-INFO` & `mama-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mama
-Version: 0.8.1
+Version: 0.8.2
 Summary: A modular C++ build tool even your mama can use
 Author-email: Jorma Rebane <jorma.rebane@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/RedFox20/Mama
 Project-URL: Bug Tracker, https://github.com/RedFox20/Mama/issues
 Keywords: mama,build,mamabuild,c,c++,tool,cmake,simple,easy,package,manager,cross-platform
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mama-0.8.1/README.md` & `mama-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `mama-0.8.1/mama/artifactory.py` & `mama-0.8.2/mama/artifactory.py`

 * *Files identical despite different names*

### Comparing `mama-0.8.1/mama/build_config.py` & `mama-0.8.2/mama/build_config.py`

 * *Files identical despite different names*

### Comparing `mama-0.8.1/mama/build_dependency.py` & `mama-0.8.2/mama/build_dependency.py`

 * *Files identical despite different names*

### Comparing `mama-0.8.1/mama/build_target.py` & `mama-0.8.2/mama/build_target.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 from .types.git import Git
 from .types.local_source import LocalSource
 from .types.asset import Asset
 from .types.artifactory_pkg import ArtifactoryPkg
 
 from .artifactory import artifactory_fetch_and_reconfigure
 from .utils.system import System, console
-from .utils.gdb import run_gdb
+from .utils.gdb import run_gdb, filter_gdb_arg
 from .utils.gtest import run_gtest
-from .utils.run import run_in_project_dir, run_in_working_dir
+from .utils.run import run_in_project_dir, run_in_working_dir, run_in_command_dir
 from .papa_deploy import papa_deploy_to, papa_upload_to
 import mama.msbuild as msbuild
 import mama.util as util
 import mama.cmake_configure as cmake
 import mama.package as package
 
 if TYPE_CHECKING:
@@ -898,14 +898,28 @@
             self.run_program(self.source_dir('bin'), 
                              self.source_dir('bin/DbTool'))
         ```
         """
         run_in_working_dir(self, working_dir, command, exit_on_fail=exit_on_fail)
 
 
+    def run_with_gdb(self, command: str, args: str, src_dir=True, gdb_by_default=True):
+        """
+        Run a program with gdb if requested, otherwise run normally.
+        To control this, add 'gdb' or 'nogdb' to args.
+        The parameter `gdb` controls what the default behavior is.
+        If used inside start(), then `mama start=nogdb` or `mama start=gdb` will control GDB enablement
+        """
+        args, gdb = filter_gdb_arg(args, gdb_by_default)
+        if gdb:
+            run_gdb(self, f'{command} {args}', src_dir=src_dir)
+        else:
+            run_in_command_dir(self, f'{command} {args}', src_dir=src_dir)
+
+
     def gdb(self, command: str, src_dir=True):
         """
         Run a command with gdb in the build folder.
         ```
             self.gdb('bin/NanoMeshTests')
         ```
         """
```

### Comparing `mama-0.8.1/mama/cmake_configure.py` & `mama-0.8.2/mama/cmake_configure.py`

 * *Files identical despite different names*

### Comparing `mama-0.8.1/mama/dependency_chain.py` & `mama-0.8.2/mama/dependency_chain.py`

 * *Files identical despite different names*

### Comparing `mama-0.8.1/mama/init_project.py` & `mama-0.8.2/mama/init_project.py`

 * *Files identical despite different names*

### Comparing `mama-0.8.1/mama/main.py` & `mama-0.8.2/mama/main.py`

 * *Files identical despite different names*

### Comparing `mama-0.8.1/mama/msbuild.py` & `mama-0.8.2/mama/msbuild.py`

 * *Files identical despite different names*

### Comparing `mama-0.8.1/mama/package.py` & `mama-0.8.2/mama/package.py`

 * *Files identical despite different names*

### Comparing `mama-0.8.1/mama/papa_deploy.py` & `mama-0.8.2/mama/papa_deploy.py`

 * *Files identical despite different names*

### Comparing `mama-0.8.1/mama/parse_mamafile.py` & `mama-0.8.2/mama/parse_mamafile.py`

 * *Files identical despite different names*

### Comparing `mama-0.8.1/mama/platforms/mips.py` & `mama-0.8.2/mama/platforms/mips.py`

 * *Files identical despite different names*

### Comparing `mama-0.8.1/mama/platforms/oclea.py` & `mama-0.8.2/mama/platforms/oclea.py`

 * *Files identical despite different names*

### Comparing `mama-0.8.1/mama/types/artifactory_pkg.py` & `mama-0.8.2/mama/types/artifactory_pkg.py`

 * *Files identical despite different names*

### Comparing `mama-0.8.1/mama/types/asset.py` & `mama-0.8.2/mama/types/asset.py`

 * *Files identical despite different names*

### Comparing `mama-0.8.1/mama/types/dep_source.py` & `mama-0.8.2/mama/types/dep_source.py`

 * *Files identical despite different names*

### Comparing `mama-0.8.1/mama/types/git.py` & `mama-0.8.2/mama/types/git.py`

 * *Files identical despite different names*

### Comparing `mama-0.8.1/mama/types/local_source.py` & `mama-0.8.2/mama/types/local_source.py`

 * *Files identical despite different names*

### Comparing `mama-0.8.1/mama/util.py` & `mama-0.8.2/mama/util.py`

 * *Files identical despite different names*

### Comparing `mama-0.8.1/mama/utils/gtest.py` & `mama-0.8.2/mama/utils/gtest.py`

 * *Files identical despite different names*

### Comparing `mama-0.8.1/mama/utils/nonblocking_io.py` & `mama-0.8.2/mama/utils/nonblocking_io.py`

 * *Files identical despite different names*

### Comparing `mama-0.8.1/mama/utils/sub_process.py` & `mama-0.8.2/mama/utils/sub_process.py`

 * *Files identical despite different names*

### Comparing `mama-0.8.1/mama/utils/system.py` & `mama-0.8.2/mama/utils/system.py`

 * *Files identical despite different names*

### Comparing `mama-0.8.1/mama.egg-info/PKG-INFO` & `mama-0.8.2/mama.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mama
-Version: 0.8.1
+Version: 0.8.2
 Summary: A modular C++ build tool even your mama can use
 Author-email: Jorma Rebane <jorma.rebane@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/RedFox20/Mama
 Project-URL: Bug Tracker, https://github.com/RedFox20/Mama/issues
 Keywords: mama,build,mamabuild,c,c++,tool,cmake,simple,easy,package,manager,cross-platform
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mama-0.8.1/mama.egg-info/SOURCES.txt` & `mama-0.8.2/mama.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mama-0.8.1/pyproject.toml` & `mama-0.8.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mama"
-version = "0.8.01"
+version = "0.8.02"
 description = "A modular C++ build tool even your mama can use"
 license = { text = "MIT" }
 authors = [
     { name="Jorma Rebane", email="jorma.rebane@gmail.com" },
 ]
 readme = "README.md"
 requires-python = ">=3.6"
```

