# Comparing `tmp/liveramp_automation-0.0.1-py3-none-any.whl.zip` & `tmp/liveramp_automation-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 9380 bytes, number of entries: 15
+Zip file size: 9396 bytes, number of entries: 15
 -rw-r--r--  2.0 unx     1711 b- defN 23-Jul-19 08:04 liveramp_automation/helper_bucket.py
 -rw-r--r--  2.0 unx     2238 b- defN 23-Jul-17 09:37 liveramp_automation/helper_file.py
 -rw-r--r--  2.0 unx     3116 b- defN 23-Jul-17 09:39 liveramp_automation/helper_login.py
 -rw-r--r--  2.0 unx       70 b- defN 23-Jul-19 08:17 liveramp_automation/helper_notification.py
 -rw-r--r--  2.0 unx      692 b- defN 23-Jul-19 08:17 liveramp_automation/util_allure.py
 -rw-r--r--  2.0 unx     2541 b- defN 23-Jul-19 08:39 liveramp_automation/util_log.py
 -rw-r--r--  2.0 unx      723 b- defN 23-Jul-19 02:39 liveramp_automation/util_parsers.py
 -rw-r--r--  2.0 unx      742 b- defN 23-Jul-17 06:23 liveramp_automation/util_playwright.py
 -rw-r--r--  2.0 unx     7058 b- defN 23-Jul-19 08:17 liveramp_automation/util_request.py
 -rw-r--r--  2.0 unx      743 b- defN 23-Jul-17 06:23 liveramp_automation/util_selenium.py
 -rw-r--r--  2.0 unx      779 b- defN 23-Jul-17 02:34 liveramp_automation/util_time.py
--rw-r--r--  2.0 unx     2376 b- defN 23-Jul-19 08:39 liveramp_automation-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-19 08:39 liveramp_automation-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       20 b- defN 23-Jul-19 08:39 liveramp_automation-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1354 b- defN 23-Jul-19 08:39 liveramp_automation-0.0.1.dist-info/RECORD
-15 files, 24255 bytes uncompressed, 7090 bytes compressed:  70.8%
+-rw-r--r--  2.0 unx     2431 b- defN 23-Jul-19 08:48 liveramp_automation-0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-19 08:48 liveramp_automation-0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       20 b- defN 23-Jul-19 08:48 liveramp_automation-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1354 b- defN 23-Jul-19 08:48 liveramp_automation-0.0.2.dist-info/RECORD
+15 files, 24310 bytes uncompressed, 7106 bytes compressed:  70.8%
```

## zipnote {}

```diff
@@ -27,20 +27,20 @@
 
 Filename: liveramp_automation/util_selenium.py
 Comment: 
 
 Filename: liveramp_automation/util_time.py
 Comment: 
 
-Filename: liveramp_automation-0.0.1.dist-info/METADATA
+Filename: liveramp_automation-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: liveramp_automation-0.0.1.dist-info/WHEEL
+Filename: liveramp_automation-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: liveramp_automation-0.0.1.dist-info/top_level.txt
+Filename: liveramp_automation-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: liveramp_automation-0.0.1.dist-info/RECORD
+Filename: liveramp_automation-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `liveramp_automation-0.0.1.dist-info/METADATA` & `liveramp_automation-0.0.2.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liveramp-automation
-Version: 0.0.1
+Version: 0.0.2
 Summary: This is the base liveramp_automation_framework
 Home-page: https://github.com/LiveRamp/qe_api_framework
 Author: Jasmine Qian
 Author-email: jasmine.qian@liveramp.com
 Description-Content-Type: text/markdown
 Requires-Dist: pytest
 Requires-Dist: pytest-bdd
@@ -34,28 +34,35 @@
 # liveramp-automation
 an automation framework helps you qucikly author scripts for any automation testing 
 
 
 
 ### Background 
 
-    Do you want to create your own test project, but struggle with configuring the environment, feel lost in choosing a testing framework, confused about integration and execution, and helpless in displaying test reports or recording test results in the long run?
+    Do you want to create your own test project, 
+    but struggle with configuring the environment, 
+    feel lost in choosing a testing framework, 
+    confused about integration and execution, 
+    and helpless in displaying test reports or recording test results in the long run?
 
     Don't worry.
 
-    We provide an open-source and easy-to-use testing framework that helps QE/DEV and anyone interested in quickly getting started with various types of automation testing.
+    We provide an open-source and easy-to-use testing framework 
+    that helps QE/DEV and anyone interested in quickly getting started 
+    with various types of automation testing.
 
 
 ### 1. Descprition of the repository
         This repository is to build a base autoamtion framework. 
         We would like to integrate the common helpers and libraries here and then build a lib.
         Later the only thing is to add the cases according to the features. 
         Since most of the common helpers and libraries have been integrated to the lib, 
         you only need to import that lib and methods.
 
 ### 2. Things need to follow:  
 - [x] Create a python repository
 - [x] Create a file named [requirements.txt](requirements.txt) and only input to this file [liveramp-automation](liveramp-automation), you can ignore the version
 - [x] Copy [conftest.py](conftest.py) and [pytest.ini](pytest.ini) to your repository's root directory
-- [x] 
+- [x] Author scripts
+- [x] Done
```

## Comparing `liveramp_automation-0.0.1.dist-info/RECORD` & `liveramp_automation-0.0.2.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -5,11 +5,11 @@
 liveramp_automation/util_allure.py,sha256=BebIEXUQ_8Xb27yA-hiyivgOZSNh6OUM7EAfGpREO1I,692
 liveramp_automation/util_log.py,sha256=ESv5AJBpJjDr4JkR21tZfCsvz9Pck__hF6Gr-1ogGI0,2541
 liveramp_automation/util_parsers.py,sha256=NNf44SSYXop1w6klQmtnJj7rsgKAqTLiyh5YBzD1DZg,723
 liveramp_automation/util_playwright.py,sha256=Kbwt6T_2LW9VIos_93V_Dc0hSpYQdUCP2PeyjZXs-mI,742
 liveramp_automation/util_request.py,sha256=NRVpgR437xwV7XWh1A8q96XBL8PCTEgS58AfA1Z_ySQ,7058
 liveramp_automation/util_selenium.py,sha256=oW9DB6MZ1cqyqOg3PwtGqI-9kG2IJXUjaco1s31XTmI,743
 liveramp_automation/util_time.py,sha256=Pdc-mJnTw0x3PmqjF59PjpinJOxnDf42SrB9UhUETrQ,779
-liveramp_automation-0.0.1.dist-info/METADATA,sha256=kzjLQP1250izDfJBgTlIBsZGKiovz1iMyumDuPahHdE,2376
-liveramp_automation-0.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-liveramp_automation-0.0.1.dist-info/top_level.txt,sha256=qRUeD1KGKo6cTZuEFDPYmXmkHqSsRq1qcGnhUgk6IHI,20
-liveramp_automation-0.0.1.dist-info/RECORD,,
+liveramp_automation-0.0.2.dist-info/METADATA,sha256=EkY3dW9MMbF0GKNxEScdCCtgFULF-rOVuR50zS-9YJc,2431
+liveramp_automation-0.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+liveramp_automation-0.0.2.dist-info/top_level.txt,sha256=qRUeD1KGKo6cTZuEFDPYmXmkHqSsRq1qcGnhUgk6IHI,20
+liveramp_automation-0.0.2.dist-info/RECORD,,
```

