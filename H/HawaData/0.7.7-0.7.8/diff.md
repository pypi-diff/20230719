# Comparing `tmp/HawaData-0.7.7.tar.gz` & `tmp/HawaData-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HawaData-0.7.7.tar", last modified: Mon Jul 17 07:07:39 2023, max compression
+gzip compressed data, was "HawaData-0.7.8.tar", last modified: Wed Jul 19 03:31:19 2023, max compression
```

## Comparing `HawaData-0.7.7.tar` & `HawaData-0.7.8.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-17 07:07:39.796785 HawaData-0.7.7/
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-17 07:07:39.784547 HawaData-0.7.7/HawaData.egg-info/
--rw-r--r--   0 wangzhou   (501) staff       (20)     3239 2023-07-17 07:07:39.000000 HawaData-0.7.7/HawaData.egg-info/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      584 2023-07-17 07:07:39.000000 HawaData-0.7.7/HawaData.egg-info/SOURCES.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-07-17 07:07:39.000000 HawaData-0.7.7/HawaData.egg-info/dependency_links.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-07-17 07:07:39.000000 HawaData-0.7.7/HawaData.egg-info/top_level.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)     3239 2023-07-17 07:07:39.796414 HawaData-0.7.7/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.7.7/README.md
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-17 07:07:39.785225 HawaData-0.7.7/hawa/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.7.7/hawa/__init__.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-17 07:07:39.788105 HawaData-0.7.7/hawa/base/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.7.7/hawa/base/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2627 2023-06-19 08:54:42.000000 HawaData-0.7.7/hawa/base/db.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.7.7/hawa/base/decos.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       98 2023-05-24 07:06:51.000000 HawaData-0.7.7/hawa/base/errors.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.7.7/hawa/base/init.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-17 07:07:39.789379 HawaData-0.7.7/hawa/common/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.7.7/hawa/common/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)    15412 2023-07-17 07:06:20.000000 HawaData-0.7.7/hawa/common/data.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     6169 2023-07-17 07:07:13.000000 HawaData-0.7.7/hawa/common/query.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     3098 2023-06-19 08:54:42.000000 HawaData-0.7.7/hawa/common/utils.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2696 2023-06-26 02:08:50.000000 HawaData-0.7.7/hawa/config.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-17 07:07:39.793272 HawaData-0.7.7/hawa/data/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.7.7/hawa/data/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      311 2023-05-22 06:36:14.000000 HawaData-0.7.7/hawa/data/city.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      432 2023-05-22 06:36:14.000000 HawaData-0.7.7/hawa/data/district.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1592 2023-05-23 08:41:21.000000 HawaData-0.7.7/hawa/data/klass.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      711 2023-06-26 06:27:54.000000 HawaData-0.7.7/hawa/data/province.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1055 2023-07-17 06:57:10.000000 HawaData-0.7.7/hawa/data/school.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1197 2023-06-13 03:42:10.000000 HawaData-0.7.7/hawa/data/student.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-17 07:07:39.795181 HawaData-0.7.7/hawa/paper/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.7.7/hawa/paper/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)    28407 2023-06-26 01:39:47.000000 HawaData-0.7.7/hawa/paper/health.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5373 2023-07-17 07:05:31.000000 HawaData-0.7.7/hawa/paper/mht.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-07-17 07:07:39.796893 HawaData-0.7.7/setup.cfg
--rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.7.7/setup.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-17 07:07:39.795535 HawaData-0.7.7/test/
--rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.7.7/test/test_query.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-19 03:31:19.335677 HawaData-0.7.8/
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-19 03:31:19.321685 HawaData-0.7.8/HawaData.egg-info/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3273 2023-07-19 03:31:19.000000 HawaData-0.7.8/HawaData.egg-info/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      584 2023-07-19 03:31:19.000000 HawaData-0.7.8/HawaData.egg-info/SOURCES.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-07-19 03:31:19.000000 HawaData-0.7.8/HawaData.egg-info/dependency_links.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-07-19 03:31:19.000000 HawaData-0.7.8/HawaData.egg-info/top_level.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3273 2023-07-19 03:31:19.335390 HawaData-0.7.8/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.7.8/README.md
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-19 03:31:19.322294 HawaData-0.7.8/hawa/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.7.8/hawa/__init__.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-19 03:31:19.325497 HawaData-0.7.8/hawa/base/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.7.8/hawa/base/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2627 2023-06-19 08:54:42.000000 HawaData-0.7.8/hawa/base/db.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.7.8/hawa/base/decos.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       98 2023-05-24 07:06:51.000000 HawaData-0.7.8/hawa/base/errors.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.7.8/hawa/base/init.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-19 03:31:19.327809 HawaData-0.7.8/hawa/common/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.7.8/hawa/common/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)    15412 2023-07-17 07:06:20.000000 HawaData-0.7.8/hawa/common/data.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     6268 2023-07-19 03:27:45.000000 HawaData-0.7.8/hawa/common/query.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3098 2023-06-19 08:54:42.000000 HawaData-0.7.8/hawa/common/utils.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2696 2023-06-26 02:08:50.000000 HawaData-0.7.8/hawa/config.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-19 03:31:19.332352 HawaData-0.7.8/hawa/data/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.7.8/hawa/data/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      311 2023-05-22 06:36:14.000000 HawaData-0.7.8/hawa/data/city.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      432 2023-05-22 06:36:14.000000 HawaData-0.7.8/hawa/data/district.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1592 2023-05-23 08:41:21.000000 HawaData-0.7.8/hawa/data/klass.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      711 2023-06-26 06:27:54.000000 HawaData-0.7.8/hawa/data/province.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1055 2023-07-17 06:57:10.000000 HawaData-0.7.8/hawa/data/school.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1015 2023-07-19 03:28:20.000000 HawaData-0.7.8/hawa/data/student.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-19 03:31:19.333976 HawaData-0.7.8/hawa/paper/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.7.8/hawa/paper/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)    28407 2023-06-26 01:39:47.000000 HawaData-0.7.8/hawa/paper/health.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5373 2023-07-17 07:05:31.000000 HawaData-0.7.8/hawa/paper/mht.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-07-19 03:31:19.335756 HawaData-0.7.8/setup.cfg
+-rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.7.8/setup.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-07-19 03:31:19.334667 HawaData-0.7.8/test/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.7.8/test/test_query.py
```

### Comparing `HawaData-0.7.7/HawaData.egg-info/PKG-INFO` & `HawaData-0.7.8/HawaData.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.7.7
+Version: 0.7.8
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -109,7 +109,8 @@
 - 0.7.1 count score rank with gender
 - 0.7.2 add cascade students
 - 0.7.3 add is_leaf to cascade students
 - 0.7.4 add ch key for dim_field data
 - 0.7.5 add ch key for dim_field data
 - 0.7.6 add ProvinceHealthApiDataLess for cascade schools
 - 0.7.7 add school mht api data
+- 0.7.8 optimization student data
```

### Comparing `HawaData-0.7.7/HawaData.egg-info/SOURCES.txt` & `HawaData-0.7.8/HawaData.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.7/PKG-INFO` & `HawaData-0.7.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.7.7
+Version: 0.7.8
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -109,7 +109,8 @@
 - 0.7.1 count score rank with gender
 - 0.7.2 add cascade students
 - 0.7.3 add is_leaf to cascade students
 - 0.7.4 add ch key for dim_field data
 - 0.7.5 add ch key for dim_field data
 - 0.7.6 add ProvinceHealthApiDataLess for cascade schools
 - 0.7.7 add school mht api data
+- 0.7.8 optimization student data
```

### Comparing `HawaData-0.7.7/README.md` & `HawaData-0.7.8/README.md`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.7/hawa/base/db.py` & `HawaData-0.7.8/hawa/base/db.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.7/hawa/base/init.py` & `HawaData-0.7.8/hawa/base/init.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.7/hawa/common/data.py` & `HawaData-0.7.8/hawa/common/data.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.7/hawa/common/query.py` & `HawaData-0.7.8/hawa/common/query.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,22 +88,24 @@
               f"inner join case_projects cp on c.project_id=cp.id " \
               f"where  is_cleared=1 and valid_to between '{valid_to_start}' and '{valid_to_end}'" \
               f" {school_sql} {paper_sql};"
         with self.db.engine_conn() as conn:
             cases = pd.read_sql(text(sql), conn).drop_duplicates(subset=['id'])
         return cases
 
-    def query_answers(self, case_ids: list[int]):
+    def query_answers(self, case_ids: list[int], student_id: int = None):
         answer_cols = "id, student_id, item_id, case_id, answer, score, created, valid"
         if len(case_ids) == 0:
             return []
         elif len(case_ids) == 1:
             sql = f"select {answer_cols} from answers where case_id={case_ids[0]} and valid=1;"
         else:
             sql = f"select {answer_cols} from answers where case_id in {tuple(case_ids)} and valid=1;"
+        if student_id:
+            sql += f" and student_id={student_id};"
         with self.db.engine_conn() as conn:
             answers = pd.read_sql(text(sql), conn).drop_duplicates(
                 subset=['case_id', 'student_id', 'item_id'])
         return answers
 
     def query_students(self, student_ids: list[int]):
         user_cols = "id, username, first_name, last_name, nickname, gender, role, source, created, " \
```

### Comparing `HawaData-0.7.7/hawa/common/utils.py` & `HawaData-0.7.8/hawa/common/utils.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.7/hawa/config.py` & `HawaData-0.7.8/hawa/config.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.7/hawa/data/klass.py` & `HawaData-0.7.8/hawa/data/klass.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.7/hawa/data/province.py` & `HawaData-0.7.8/hawa/data/province.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.7/hawa/data/school.py` & `HawaData-0.7.8/hawa/data/school.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.7/hawa/paper/health.py` & `HawaData-0.7.8/hawa/paper/health.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.7/hawa/paper/mht.py` & `HawaData-0.7.8/hawa/paper/mht.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.7/setup.py` & `HawaData-0.7.8/setup.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.7.7/test/test_query.py` & `HawaData-0.7.8/test/test_query.py`

 * *Files identical despite different names*

