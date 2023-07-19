# Comparing `tmp/kingunit_inspector-0.0.2.tar.gz` & `tmp/kingunit_inspector-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/jiayu/Documents/Kingstar/KingUnit-Inspector/dist/.tmp-29pikoe7/kingunit_inspector-0.0.2.tar", last modified: Wed Jul 19 07:09:00 2023, max compression
+gzip compressed data, was "/Users/jiayu/Documents/Kingstar/KingUnit-Inspector/dist/.tmp-232b7kbi/kingunit_inspector-0.0.3.tar", last modified: Wed Jul 19 08:08:54 2023, max compression
```

## Comparing `kingunit_inspector-0.0.2.tar` & `kingunit_inspector-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-19 07:09:00.987601 kingunit_inspector-0.0.2/
--rw-r--r--   0 jiayu      (501) staff       (20)     9161 2023-07-19 06:48:32.000000 kingunit_inspector-0.0.2/LICENSE
--rw-r--r--   0 jiayu      (501) staff       (20)    10135 2023-07-19 07:09:00.987363 kingunit_inspector-0.0.2/PKG-INFO
--rw-r--r--   0 jiayu      (501) staff       (20)      111 2023-07-19 06:51:51.000000 kingunit_inspector-0.0.2/README.md
-drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-19 07:09:00.985722 kingunit_inspector-0.0.2/kingunit_inspector/
--rw-r--r--   0 jiayu      (501) staff       (20)        0 2023-07-19 07:08:08.000000 kingunit_inspector-0.0.2/kingunit_inspector/__init__.py
--rw-r--r--   0 jiayu      (501) staff       (20)     3005 2023-07-19 06:49:06.000000 kingunit_inspector-0.0.2/kingunit_inspector/inspector.py
-drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-19 07:09:00.987038 kingunit_inspector-0.0.2/kingunit_inspector.egg-info/
--rw-r--r--   0 jiayu      (501) staff       (20)    10135 2023-07-19 07:09:00.000000 kingunit_inspector-0.0.2/kingunit_inspector.egg-info/PKG-INFO
--rw-r--r--   0 jiayu      (501) staff       (20)      304 2023-07-19 07:09:00.000000 kingunit_inspector-0.0.2/kingunit_inspector.egg-info/SOURCES.txt
--rw-r--r--   0 jiayu      (501) staff       (20)        1 2023-07-19 07:09:00.000000 kingunit_inspector-0.0.2/kingunit_inspector.egg-info/dependency_links.txt
--rw-r--r--   0 jiayu      (501) staff       (20)        9 2023-07-19 07:09:00.000000 kingunit_inspector-0.0.2/kingunit_inspector.egg-info/requires.txt
--rw-r--r--   0 jiayu      (501) staff       (20)       19 2023-07-19 07:09:00.000000 kingunit_inspector-0.0.2/kingunit_inspector.egg-info/top_level.txt
--rw-r--r--   0 jiayu      (501) staff       (20)      443 2023-07-19 07:08:15.000000 kingunit_inspector-0.0.2/pyproject.toml
--rw-r--r--   0 jiayu      (501) staff       (20)       38 2023-07-19 07:09:00.987676 kingunit_inspector-0.0.2/setup.cfg
+drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-19 08:08:54.540311 kingunit_inspector-0.0.3/
+-rw-r--r--   0 jiayu      (501) staff       (20)     9161 2023-07-19 06:48:32.000000 kingunit_inspector-0.0.3/LICENSE
+-rw-r--r--   0 jiayu      (501) staff       (20)    10135 2023-07-19 08:08:54.540122 kingunit_inspector-0.0.3/PKG-INFO
+-rw-r--r--   0 jiayu      (501) staff       (20)      111 2023-07-19 06:51:51.000000 kingunit_inspector-0.0.3/README.md
+drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-19 08:08:54.538858 kingunit_inspector-0.0.3/kingunit_inspector/
+-rw-r--r--   0 jiayu      (501) staff       (20)        0 2023-07-19 07:08:08.000000 kingunit_inspector-0.0.3/kingunit_inspector/__init__.py
+-rw-r--r--   0 jiayu      (501) staff       (20)     3089 2023-07-19 08:06:21.000000 kingunit_inspector-0.0.3/kingunit_inspector/inspector.py
+drwxr-xr-x   0 jiayu      (501) staff       (20)        0 2023-07-19 08:08:54.539797 kingunit_inspector-0.0.3/kingunit_inspector.egg-info/
+-rw-r--r--   0 jiayu      (501) staff       (20)    10135 2023-07-19 08:08:54.000000 kingunit_inspector-0.0.3/kingunit_inspector.egg-info/PKG-INFO
+-rw-r--r--   0 jiayu      (501) staff       (20)      304 2023-07-19 08:08:54.000000 kingunit_inspector-0.0.3/kingunit_inspector.egg-info/SOURCES.txt
+-rw-r--r--   0 jiayu      (501) staff       (20)        1 2023-07-19 08:08:54.000000 kingunit_inspector-0.0.3/kingunit_inspector.egg-info/dependency_links.txt
+-rw-r--r--   0 jiayu      (501) staff       (20)        9 2023-07-19 08:08:54.000000 kingunit_inspector-0.0.3/kingunit_inspector.egg-info/requires.txt
+-rw-r--r--   0 jiayu      (501) staff       (20)       19 2023-07-19 08:08:54.000000 kingunit_inspector-0.0.3/kingunit_inspector.egg-info/top_level.txt
+-rw-r--r--   0 jiayu      (501) staff       (20)      443 2023-07-19 08:08:47.000000 kingunit_inspector-0.0.3/pyproject.toml
+-rw-r--r--   0 jiayu      (501) staff       (20)       38 2023-07-19 08:08:54.540372 kingunit_inspector-0.0.3/setup.cfg
```

### Comparing `kingunit_inspector-0.0.2/LICENSE` & `kingunit_inspector-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kingunit_inspector-0.0.2/PKG-INFO` & `kingunit_inspector-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kingunit_inspector
-Version: 0.0.2
+Version: 0.0.3
 Summary: KingUnit Inspector
 Author-email: 东南dnf <zjy2414@outlook.com>
 License: Apache License
         Version 2.0, January 2004
         http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `kingunit_inspector-0.0.2/kingunit_inspector/inspector.py` & `kingunit_inspector-0.0.3/kingunit_inspector/inspector.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,16 +86,19 @@
     响应检查器
     检查响应数据是否符合预期，对每一个参数进行检查，如不匹配则输出错误信息
     :param response: 响应
     :param expected_data: 预期数据
     :return: None
     """
 
-    if "expected" not in test_case.keys():
+    if "expected" not in test_case.keys() or test_case["expected"] == {} :
         print("Expected data not configured, please check by yourself.")
-        # 输出响应结果
-        print(f"input: {test_case['input']}")
-        print(f"output: {response.json()}")
-    else:
+
+    # 输出响应结果
+    print(f"input: {test_case['input']}")
+    print(f"output: {response.json()}")
+
+
+    if "expected" in test_case.keys() and test_case["expected"] != {}:
         assert (
             response.json() == test_case["expected"]
         ), f"response expected: {str(test_case['expected'])}, actual: {str(response.json())}"
```

### Comparing `kingunit_inspector-0.0.2/kingunit_inspector.egg-info/PKG-INFO` & `kingunit_inspector-0.0.3/kingunit_inspector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kingunit-inspector
-Version: 0.0.2
+Version: 0.0.3
 Summary: KingUnit Inspector
 Author-email: 东南dnf <zjy2414@outlook.com>
 License: Apache License
         Version 2.0, January 2004
         http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

