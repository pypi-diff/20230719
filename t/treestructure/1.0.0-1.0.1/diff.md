# Comparing `tmp/treestructure-1.0.0.tar.gz` & `tmp/treestructure-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "treestructure-1.0.0.tar", last modified: Sun Jul 16 11:08:03 2023, max compression
+gzip compressed data, was "treestructure-1.0.1.tar", last modified: Wed Jul 19 00:51:59 2023, max compression
```

## Comparing `treestructure-1.0.0.tar` & `treestructure-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 11:08:03.046896 treestructure-1.0.0/
--rw-rw-rw-   0        0        0    11558 2023-04-09 14:12:53.000000 treestructure-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     3485 2023-07-16 11:08:03.046896 treestructure-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2295 2023-07-16 07:48:57.000000 treestructure-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-16 11:08:03.047396 treestructure-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1090 2023-07-16 11:07:26.000000 treestructure-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-16 11:08:03.042396 treestructure-1.0.0/treestructure/
--rw-rw-rw-   0        0        0     1858 2023-07-16 09:53:10.000000 treestructure-1.0.0/treestructure/__init__.py
--rw-rw-rw-   0        0        0    26585 2023-07-14 18:26:38.000000 treestructure-1.0.0/treestructure/binaryHeap.py
--rw-rw-rw-   0        0        0      760 2023-07-14 18:26:38.000000 treestructure-1.0.0/treestructure/binaryHeapNode.py
--rw-rw-rw-   0        0        0     2394 2023-07-13 15:09:16.000000 treestructure-1.0.0/treestructure/binaryNode.py
--rw-rw-rw-   0        0        0    20791 2023-07-13 16:24:53.000000 treestructure-1.0.0/treestructure/binarySearchTree.py
--rw-rw-rw-   0        0        0      277 2023-07-10 17:22:13.000000 treestructure-1.0.0/treestructure/constants.py
--rw-rw-rw-   0        0        0       21 2023-07-13 12:25:27.000000 treestructure-1.0.0/treestructure/version.py
-drwxrwxrwx   0        0        0        0 2023-07-16 11:08:03.045896 treestructure-1.0.0/treestructure.egg-info/
--rw-rw-rw-   0        0        0     3485 2023-07-16 11:08:02.000000 treestructure-1.0.0/treestructure.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-07-16 11:08:03.000000 treestructure-1.0.0/treestructure.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 11:08:02.000000 treestructure-1.0.0/treestructure.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-07-16 11:08:02.000000 treestructure-1.0.0/treestructure.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-19 00:51:59.734155 treestructure-1.0.1/
+-rw-rw-rw-   0        0        0    11558 2023-04-09 14:12:53.000000 treestructure-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     3584 2023-07-19 00:51:59.733409 treestructure-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2378 2023-07-16 11:56:54.000000 treestructure-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-19 00:51:59.734680 treestructure-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1090 2023-07-16 11:07:26.000000 treestructure-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 00:51:59.728698 treestructure-1.0.1/treestructure/
+-rw-rw-rw-   0        0        0     1858 2023-07-16 09:53:10.000000 treestructure-1.0.1/treestructure/__init__.py
+-rw-rw-rw-   0        0        0    26675 2023-07-18 17:23:30.000000 treestructure-1.0.1/treestructure/binaryHeap.py
+-rw-rw-rw-   0        0        0      760 2023-07-14 18:26:38.000000 treestructure-1.0.1/treestructure/binaryHeapNode.py
+-rw-rw-rw-   0        0        0     2394 2023-07-13 15:09:16.000000 treestructure-1.0.1/treestructure/binaryNode.py
+-rw-rw-rw-   0        0        0    20791 2023-07-13 16:24:53.000000 treestructure-1.0.1/treestructure/binarySearchTree.py
+-rw-rw-rw-   0        0        0      277 2023-07-10 17:22:13.000000 treestructure-1.0.1/treestructure/constants.py
+-rw-rw-rw-   0        0        0       21 2023-07-19 00:51:19.000000 treestructure-1.0.1/treestructure/version.py
+drwxrwxrwx   0        0        0        0 2023-07-19 00:51:59.732901 treestructure-1.0.1/treestructure.egg-info/
+-rw-rw-rw-   0        0        0     3584 2023-07-19 00:51:59.000000 treestructure-1.0.1/treestructure.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-07-19 00:51:59.000000 treestructure-1.0.1/treestructure.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 00:51:59.000000 treestructure-1.0.1/treestructure.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-19 00:51:59.000000 treestructure-1.0.1/treestructure.egg-info/top_level.txt
```

### Comparing `treestructure-1.0.0/LICENSE` & `treestructure-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `treestructure-1.0.0/PKG-INFO` & `treestructure-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: treestructure
-Version: 1.0.0
+Version: 1.0.1
 Summary: Tree Structure is a module that implements some common trees in data structure.
 Home-page: https://github.com/Musicmathstudio/treeStructure
 Author: Tony Chiu
 Author-email: pi3141592676@yahoo.com.tw
 License: UNKNOWN
 Description: # Tree Structure
         
+        ![Pypi link](https://img.shields.io/pypi/v/treestructure.svg?style=flat-square)
+        
         Tree Structure is a module that implements some common trees in data structure.
         
         ## Quick Start
         
         There are two basic components in each type of tree structure: **Node** and **Tree**.  
         Each node has two basic attributes: **order** and **value**.  
         Order is the key to construct the tree structure. Default order is current timestamp.
```

### Comparing `treestructure-1.0.0/README.md` & `treestructure-1.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Tree Structure
 
+![Pypi link](https://img.shields.io/pypi/v/treestructure.svg?style=flat-square)
+
 Tree Structure is a module that implements some common trees in data structure.
 
 ## Quick Start
 
 There are two basic components in each type of tree structure: **Node** and **Tree**.  
 Each node has two basic attributes: **order** and **value**.  
 Order is the key to construct the tree structure. Default order is current timestamp.
```

### Comparing `treestructure-1.0.0/setup.py` & `treestructure-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `treestructure-1.0.0/treestructure/__init__.py` & `treestructure-1.0.1/treestructure/__init__.py`

 * *Files identical despite different names*

### Comparing `treestructure-1.0.0/treestructure/binaryHeap.py` & `treestructure-1.0.1/treestructure/binaryHeap.py`

 * *Files 1% similar despite different names*

```diff
@@ -535,43 +535,43 @@
             return None
         else:
             if self.heapStruct == Constants.BinaryHeap.max:
                 return min(islice(self.heapList, len(self.heapList) // 2, None), key=lambda node: node.order)
             elif self.heapStruct == Constants.BinaryHeap.min:
                 return self.heapList[0]
 
-    def deleteMaxNode(self):
+    def deleteMaxNode(self) -> Union[BinaryHeapNode, None]:
         """
         Delete max order node in tree.
 
         :return: The node that be removed. Return None if there's no node in tree.
         """
 
         if self.heapList:
             if self.heapStruct == Constants.BinaryHeap.max:
-                self.deleteNode(self.heapList[0].order)
+                return self.deleteNode(self.heapList[0].order)
             elif self.heapStruct == Constants.BinaryHeap.min:
                 maxNode = self.maxNode()
                 if maxNode:
-                    self.deleteNode(maxNode.order)
+                    return self.deleteNode(maxNode.order)
 
-    def deleteMinNode(self):
+    def deleteMinNode(self) -> Union[BinaryHeapNode, None]:
         """
         Delete min order node in tree.
 
         :return: The node that be removed. Return None if there's no node in tree.
         """
 
         if self.heapList:
             if self.heapStruct == Constants.BinaryHeap.min:
-                self.deleteNode(self.heapList[0].order)
+                return self.deleteNode(self.heapList[0].order)
             elif self.heapStruct == Constants.BinaryHeap.max:
                 minNode = self.minNode()
                 if minNode:
-                    self.deleteNode(minNode.order)
+                    return self.deleteNode(minNode.order)
 
     def package(self, onlyOrder: bool = False) -> Union[dict, list, None]:
         """
         Package tree structure and return.
 
         :param onlyOrder: Return tree only contains order in each node if onlyOrder is True. Default is False.
         :return: Tree structure as dictionary. Return type is list if onlyOrder is True. Return None if tree is empty.
```

### Comparing `treestructure-1.0.0/treestructure/binaryHeapNode.py` & `treestructure-1.0.1/treestructure/binaryHeapNode.py`

 * *Files identical despite different names*

### Comparing `treestructure-1.0.0/treestructure/binaryNode.py` & `treestructure-1.0.1/treestructure/binaryNode.py`

 * *Files identical despite different names*

### Comparing `treestructure-1.0.0/treestructure/binarySearchTree.py` & `treestructure-1.0.1/treestructure/binarySearchTree.py`

 * *Files identical despite different names*

### Comparing `treestructure-1.0.0/treestructure.egg-info/PKG-INFO` & `treestructure-1.0.1/treestructure.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: treestructure
-Version: 1.0.0
+Version: 1.0.1
 Summary: Tree Structure is a module that implements some common trees in data structure.
 Home-page: https://github.com/Musicmathstudio/treeStructure
 Author: Tony Chiu
 Author-email: pi3141592676@yahoo.com.tw
 License: UNKNOWN
 Description: # Tree Structure
         
+        ![Pypi link](https://img.shields.io/pypi/v/treestructure.svg?style=flat-square)
+        
         Tree Structure is a module that implements some common trees in data structure.
         
         ## Quick Start
         
         There are two basic components in each type of tree structure: **Node** and **Tree**.  
         Each node has two basic attributes: **order** and **value**.  
         Order is the key to construct the tree structure. Default order is current timestamp.
```

