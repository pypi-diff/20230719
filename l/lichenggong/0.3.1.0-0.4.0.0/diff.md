# Comparing `tmp/lichenggong-0.3.1.0.tar.gz` & `tmp/lichenggong-0.4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lichenggong-0.3.1.0.tar", last modified: Sun Jul 16 12:51:25 2023, max compression
+gzip compressed data, was "lichenggong-0.4.0.0.tar", last modified: Wed Jul 19 12:27:42 2023, max compression
```

## Comparing `lichenggong-0.3.1.0.tar` & `lichenggong-0.4.0.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 12:51:25.456477 lichenggong-0.3.1.0/
--rw-rw-rw-   0        0        0      619 2023-07-16 12:51:25.456477 lichenggong-0.3.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-07-08 10:18:48.000000 lichenggong-0.3.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-16 12:51:25.409278 lichenggong-0.3.1.0/lichenggong/
-drwxrwxrwx   0        0        0        0 2023-07-16 12:51:25.425223 lichenggong-0.3.1.0/lichenggong/Noodows/
--rw-rw-rw-   0        0        0     2776 2023-07-16 06:32:41.000000 lichenggong-0.3.1.0/lichenggong/Noodows/__bios__.py
--rw-rw-rw-   0        0        0      130 2023-07-16 10:50:48.000000 lichenggong-0.3.1.0/lichenggong/Noodows/__init__.py
--rw-rw-rw-   0        0        0     8595 2023-07-16 11:51:15.000000 lichenggong-0.3.1.0/lichenggong/Noodows/__noodows__.py
--rw-rw-rw-   0        0        0        4 2023-05-01 01:01:06.000000 lichenggong-0.3.1.0/lichenggong/Noodows/first.txt
--rw-rw-rw-   0        0        0      372 2023-07-16 06:12:46.000000 lichenggong-0.3.1.0/lichenggong/Noodows/practice.py
--rw-rw-rw-   0        0        0        0 2023-07-16 12:12:38.000000 lichenggong-0.3.1.0/lichenggong/Noodows/python.txt
--rw-rw-rw-   0        0        0     2270 2023-07-16 12:50:31.000000 lichenggong-0.3.1.0/lichenggong/Noodows/update.log
-drwxrwxrwx   0        0        0        0 2023-07-16 12:51:25.440852 lichenggong-0.3.1.0/lichenggong/Noodows/version/
--rw-rw-rw-   0        0        0        9 2023-07-16 12:50:10.000000 lichenggong-0.3.1.0/lichenggong/Noodows/version/build_version.txt
--rw-rw-rw-   0        0        0        7 2023-07-16 12:49:08.000000 lichenggong-0.3.1.0/lichenggong/Noodows/version/version.txt
-drwxrwxrwx   0        0        0        0 2023-07-16 12:51:25.393657 lichenggong-0.3.1.0/lichenggong/Program_Files/
-drwxrwxrwx   0        0        0        0 2023-07-16 12:51:25.456477 lichenggong-0.3.1.0/lichenggong/Program_Files/System/
--rw-rw-rw-   0        0        0     5802 2023-07-16 06:32:41.000000 lichenggong-0.3.1.0/lichenggong/Program_Files/System/__calc__.py
--rw-rw-rw-   0        0        0     1699 2023-07-16 06:40:01.000000 lichenggong-0.3.1.0/lichenggong/Program_Files/System/__logo__.py
--rw-rw-rw-   0        0        0     2476 2023-07-16 06:32:41.000000 lichenggong-0.3.1.0/lichenggong/Program_Files/System/__n_time__.py
--rw-rw-rw-   0        0        0       16 2023-01-13 12:59:12.000000 lichenggong-0.3.1.0/lichenggong/Program_Files/System/__start_menu__.py
--rw-rw-rw-   0        0        0      263 2023-01-15 04:33:21.000000 lichenggong-0.3.1.0/lichenggong/Program_Files/System/__thanks__.py
--rw-rw-rw-   0        0        0    15973 2023-07-16 11:51:15.000000 lichenggong-0.3.1.0/lichenggong/Program_Files/System/__user__.py
-drwxrwxrwx   0        0        0        0 2023-07-16 12:51:25.456477 lichenggong-0.3.1.0/lichenggong/Program_Files/User/
--rw-rw-rw-   0        0        0        3 2023-07-08 09:50:30.000000 lichenggong-0.3.1.0/lichenggong/Program_Files/User/_.py
--rw-rw-rw-   0        0        0      870 2023-07-16 12:47:21.000000 lichenggong-0.3.1.0/lichenggong/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-16 12:51:25.409278 lichenggong-0.3.1.0/lichenggong.egg-info/
--rw-rw-rw-   0        0        0      619 2023-07-16 12:51:25.000000 lichenggong-0.3.1.0/lichenggong.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      807 2023-07-16 12:51:25.000000 lichenggong-0.3.1.0/lichenggong.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 12:51:25.000000 lichenggong-0.3.1.0/lichenggong.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-16 12:51:25.000000 lichenggong-0.3.1.0/lichenggong.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-16 12:51:25.456477 lichenggong-0.3.1.0/setup.cfg
--rw-rw-rw-   0        0        0      907 2023-07-16 10:40:05.000000 lichenggong-0.3.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 12:27:42.371322 lichenggong-0.4.0.0/
+-rw-rw-rw-   0        0        0      794 2023-07-19 12:27:42.371322 lichenggong-0.4.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      466 2023-07-18 06:15:27.000000 lichenggong-0.4.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-19 12:27:42.261937 lichenggong-0.4.0.0/lichenggong/
+drwxrwxrwx   0        0        0        0 2023-07-19 12:27:42.308816 lichenggong-0.4.0.0/lichenggong/Noodows/
+-rw-rw-rw-   0        0        0     3051 2023-07-18 07:03:53.000000 lichenggong-0.4.0.0/lichenggong/Noodows/__bios__.py
+-rw-rw-rw-   0        0        0        0 2023-07-18 10:50:27.000000 lichenggong-0.4.0.0/lichenggong/Noodows/__init__.py
+-rw-rw-rw-   0        0        0    11069 2023-07-18 14:11:36.000000 lichenggong-0.4.0.0/lichenggong/Noodows/__noodows__.py
+-rw-rw-rw-   0        0        0        4 2023-05-01 01:01:06.000000 lichenggong-0.4.0.0/lichenggong/Noodows/first.txt
+-rw-rw-rw-   0        0        0      372 2023-07-16 06:12:46.000000 lichenggong-0.4.0.0/lichenggong/Noodows/practice.py
+-rw-rw-rw-   0        0        0        0 2023-07-16 12:12:38.000000 lichenggong-0.4.0.0/lichenggong/Noodows/python.txt
+-rw-rw-rw-   0        0        0     2270 2023-07-16 12:50:31.000000 lichenggong-0.4.0.0/lichenggong/Noodows/update.log
+drwxrwxrwx   0        0        0        0 2023-07-19 12:27:42.324444 lichenggong-0.4.0.0/lichenggong/Noodows/version/
+-rw-rw-rw-   0        0        0        9 2023-07-19 12:24:31.000000 lichenggong-0.4.0.0/lichenggong/Noodows/version/build_version.txt
+-rw-rw-rw-   0        0        0        7 2023-07-19 12:24:04.000000 lichenggong-0.4.0.0/lichenggong/Noodows/version/version.txt
+drwxrwxrwx   0        0        0        0 2023-07-19 12:27:42.259787 lichenggong-0.4.0.0/lichenggong/Program_Files/
+drwxrwxrwx   0        0        0        0 2023-07-19 12:27:42.355693 lichenggong-0.4.0.0/lichenggong/Program_Files/System/
+-rw-rw-rw-   0        0        0     5766 2023-07-18 07:03:53.000000 lichenggong-0.4.0.0/lichenggong/Program_Files/System/__calc__.py
+-rw-rw-rw-   0        0        0     1699 2023-07-16 06:40:01.000000 lichenggong-0.4.0.0/lichenggong/Program_Files/System/__logo__.py
+-rw-rw-rw-   0        0        0        0 2023-07-18 06:49:18.000000 lichenggong-0.4.0.0/lichenggong/Program_Files/System/__n_explorer__.py
+-rw-rw-rw-   0        0        0     2468 2023-07-18 07:03:53.000000 lichenggong-0.4.0.0/lichenggong/Program_Files/System/__n_time__.py
+-rw-rw-rw-   0        0        0      233 2023-07-18 06:21:05.000000 lichenggong-0.4.0.0/lichenggong/Program_Files/System/__thanks__.py
+-rw-rw-rw-   0        0        0    24766 2023-07-19 12:21:14.000000 lichenggong-0.4.0.0/lichenggong/Program_Files/System/__user__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 12:27:42.355693 lichenggong-0.4.0.0/lichenggong/Program_Files/User/
+-rw-rw-rw-   0        0        0        3 2023-07-08 09:50:30.000000 lichenggong-0.4.0.0/lichenggong/Program_Files/User/_.py
+-rw-rw-rw-   0        0        0      874 2023-07-18 08:47:14.000000 lichenggong-0.4.0.0/lichenggong/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 12:27:42.261937 lichenggong-0.4.0.0/lichenggong.egg-info/
+-rw-rw-rw-   0        0        0      794 2023-07-19 12:27:42.000000 lichenggong-0.4.0.0/lichenggong.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      807 2023-07-19 12:27:42.000000 lichenggong-0.4.0.0/lichenggong.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 12:27:42.000000 lichenggong-0.4.0.0/lichenggong.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-19 12:27:42.000000 lichenggong-0.4.0.0/lichenggong.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-19 12:27:42.371322 lichenggong-0.4.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      914 2023-07-18 10:24:28.000000 lichenggong-0.4.0.0/setup.py
```

### Comparing `lichenggong-0.3.1.0/lichenggong/Noodows/__bios__.py` & `lichenggong-0.4.0.0/lichenggong/Noodows/__bios__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 # coding=utf-8
-import gc
-import os
+import gc, os, sys
 import time as t
 
+sys.path.append('../Program_Files/System')
+import __logo__
+
 
 def file_dir(files_dir):
     # 测量文件的路径与大小
     count = 0
     size = 0
     total_code_num = 0  # 统计文件代码行数计数变量
     total_blank_num = 0  # 统计文件空行数计数变量
     total_annotate_num = 0  # 统计文件注释行数计数变量
     file_list = []
     for parent, dir_names, filenames in os.walk(files_dir):
         for filename in filenames:
             if filename.endswith('.py'):
                 file_list.append(os.path.join(parent, filename))
                 # 将文件名和目录名拼成绝对路径，添加到列表里
+            elif filename.endswith('.txt'):
+                file_list.append(os.path.join(parent, filename))
+                # txt文件存储也算上
     for root, dirs, files in os.walk(files_dir):
         for file in files:
             size += os.path.getsize(os.path.join(root, file))
         count += len(files)
     for f in file_list:
         with open(f, encoding='UTF-8') as fp:
             code_num = 0  # 当前文件代码行数计数变量
@@ -46,30 +51,33 @@
     del size, count, fp, content, f
     del file_list, total_code_num, code_num, total_blank_num, blank_num, total_annotate_num, annotate_num
     gc.collect()
     return files
 
 
 def bios():
+    __logo__.logo3_0()
     file_name = r'../'
     scale = 20
     start = t.perf_counter()
     for i in range(scale + 1):
         a = "|" * i
         b = "-" * (scale - i)
         c = (i / scale) * 100
         dur = t.perf_counter() - start
         print("Loading {:^3.0f}%[{}{}]{:.2f}s Noodows is coming".format(c, a, b, dur))
     print()
-    a = file_dir('./')
+    a = file_dir('../')
     print(' p() : {}'.format(a[0][0]))  # 返回代码行数
     print(" ' '   : {}".format(a[0][1]))  # 返回空行数
     print(' #   : {}'.format(a[0][2]))  # 返回注释行数
-    for root, dirs, files in os.walk(file_name):
+    for root, dirs, file in os.walk(file_name):
         print(root)
         print(dirs)
-        print(files, '\n')
+        print(file)
     print('files:', a[1])
     print('large(MB)', a[2] / (1024 ** 2))
-    del a, root, dirs, files
+    print('hallo,world =) ')
+    print()
+    del a, root, dirs, file
     del i, scale, start, dur, b, c
     gc.collect()
```

### Comparing `lichenggong-0.3.1.0/lichenggong/Noodows/__noodows__.py` & `lichenggong-0.4.0.0/lichenggong/Noodows/__noodows__.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,38 +4,43 @@
 import sys
 
 # 系统包
 
 sys.path.append('../Program_Files/System')
 
 import __bios__
-import __calc__
-import __logo__
-import __user__
 import __thanks__
+import __calc__
 import __n_time__
+import __user__
 
 
 # 自建包
 
 # import some modules
 
-# 优雅
-
 def __n_start__():
     def __first_choose__():
         with open('first.txt', 'r') as First:
             first = First.readline()
+        # 检查是否为初始
         if first == 'True':
-            __user__.__u_first__(0)
+            # 如果是
+            __user__.u_first()
+            # 创建用户
             first = 'False'
             with open('first.txt', "w", encoding="utf-8") as First:
                 First.write(first)
+            # 然后清除初始状态
             del first
             gc.collect()
+        # 如果不是，就啥事也不做
+
+    with open('.//now//language.txt', 'r') as lan:
+        users_language = lan.readline()
 
     def __language__(model, us_en, zn_cn, zn_tw):
         if users_language == 'US_en':
             if model == 'print':
                 print(us_en)
             elif model == 'input':
                 print(us_en, end='')
@@ -73,25 +78,23 @@
             else:
                 print('error: input an undefined thing')
         else:
             print('error: your language is wrong ')
 
     __first_choose__()
     __bios__.bios()
-    print('hallo,world =) ')
-    print()
-    __logo__.logo3_0()
     __user__.user()
-    with open('.//now//language.txt', 'r') as language:
-        users_language = language.readline()
+
     with open('.//now//power.txt', 'r') as power:
         users_power = power.readline()
-    del language, power
+
+    del power, lan
     gc.collect()
     while 1:
+        __language__('()', '-Desktop-', '-桌面-', '-桌面-')
         __language__('()', '0: Start', '0: 开始菜单', '0: 開始菜單')
         __language__('()', '1: Explorer', '1: 此电脑', '1: 我的電腦')
         __language__('()', '2: Log out', '2: 退出账号', '2: 退出賬號')
         if users_power == 'admin':
             __language__('()', '3: thanks', '3: 致谢名单', '3: 致謝名單')
         __language__('()', '99: Exit', '99：关机', '99：關機')
         choose = __language__('input', 'want?', '你干嘛', '你幹嘛')
@@ -113,51 +116,81 @@
                         elif choose == '2':
                             while 1:
                                 __language__('()', '-sys software-', '-汐筒软件-', '-系統軟件-')
                                 __language__('()', '0: back', '0: 退出', '0: 退出')
                                 __language__('()', '1: calc', '1: 计算器', '1: 計算器')
                                 __language__('()', '2: Time', '2: 时间', '2: 時間')
                                 if users_power == 'admin':
-                                    __language__('()', '3: user change', '3: 用户更改', '3: 用戶更改')
+                                    __language__('()', '3: user', '3: 用户', '3: 用戶')
                                 choose = __language__('input', 'want?', '你干嘛', '你幹嘛')
                                 if choose == '0':
                                     print("Good bye!")
                                     break
                                 elif choose == '1':
                                     __calc__.calc()
                                 elif choose == '2':
-                                    choose = __language__('input', '1:back,2:continue', '1:返回,2:继续',
+                                    choose = __language__('input',
+                                                          '1:back,2:continue',
+                                                          '1:返回,2:继续',
                                                           '1:返回,2:繼續')
                                     if choose == '1':
                                         print("Good bye!")
                                     elif choose == '2':
-                                        __noodows_time__.time(1)
+                                        __n_time__.time(1)
                                     else:
                                         print('error: input an undefined thing')
                                 elif choose == '3':
                                     if users_power != 'admin':
                                         print('error: input an undefined thing')
-                                    choose = __language__('input', '1:back,2:continue', '1:返回,2:继续',
+                                    choose = __language__('input',
+                                                          '1:back,2:continue',
+                                                          '1:返回,2:继续',
                                                           '1:返回,2:繼續')
                                     if choose == '1':
                                         print("Good bye!")
                                     elif choose == '2':
-                                        with open('.//now//password.txt', 'r') as password:
-                                            users_password = password.readline()  # read the Password
-                                        while 1:
-                                            input_password = __language__('input',
-                                                                          'admin,please input your password:',
-                                                                          '管理员,请输入密码:',
-                                                                          '管理员,請輸入密碼:')
-                                            if input_password != users_password:
-                                                __language__('print',
-                                                             'the password you input is wrong',
-                                                             '密码错误',
-                                                             '密碼錯誤')
-                                            __user__.change()
+                                        __language__('print',
+                                                     '1.change the current user',
+                                                     '1.更改当前用户',
+                                                     '1.更改當前用戶')
+                                        __language__('print',
+                                                     '2.create a new user',
+                                                     '2.创建新用户',
+                                                     '2.創建新用戶')
+                                        choose = __language__('input', 'want?', '你干嘛', '你幹嘛')
+                                        if choose == '1':
+                                            with open('.//now//password.txt', 'r') as password:
+                                                users_password = password.readline()
+                                            # read the Password
+                                            while 1:
+                                                input_password = __language__('input',
+                                                                              'administrator,input your password:',
+                                                                              '管理员,请输入密码:',
+                                                                              '管理员,請輸入密碼:')
+                                                if input_password != users_password:
+                                                    __language__('print',
+                                                                 'the password you input is wrong',
+                                                                 '密码错误',
+                                                                 '密碼錯誤')
+                                                __user__.change()
+                                        if choose == '2':
+                                            with open('.//now//password.txt', 'r') as password:
+                                                users_password = password.readline()
+                                            # read the Password
+                                            while 1:
+                                                input_password = __language__('input',
+                                                                              'administrator,input your password:',
+                                                                              '管理员,请输入密码:',
+                                                                              '管理员,請輸入密碼:')
+                                                if input_password != users_password:
+                                                    __language__('print',
+                                                                 'the password you input is wrong',
+                                                                 '密码错误',
+                                                                 '密碼錯誤')
+                                                __user__.u_new()
                                             del users_password, input_password
                                             gc.collect()
                                     else:
                                         print('error')
 
                         else:
                             print('error: input an undefined thing')
@@ -187,8 +220,10 @@
                 print("Good bye!")
             elif choose == '2':
                 __thanks__.thanks()
         elif choose == '99':
             exit(0)
         else:
             print('error: input an undefined thing')
-__n_start__()
+
+
+__n_start__()
```

### Comparing `lichenggong-0.3.1.0/lichenggong/Noodows/update.log` & `lichenggong-0.4.0.0/lichenggong/Noodows/update.log`

 * *Files identical despite different names*

### Comparing `lichenggong-0.3.1.0/lichenggong/Program_Files/System/__calc__.py` & `lichenggong-0.4.0.0/lichenggong/Program_Files/System/__calc__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,12 @@
 # coding=utf-8
 import gc
 
 
 def calc():
-    """
-
-    :return:
-    """
-
     def sqrt(number):
         num0 = number / 2
         num1 = number / 2 + number / (num0 * 2)
         while abs(num1 - num0) > 1e-5:
             num0 = num1
             num1 = num0 / 2 + number / num0 * 2
         del num0, num1
```

### Comparing `lichenggong-0.3.1.0/lichenggong/Program_Files/System/__logo__.py` & `lichenggong-0.4.0.0/lichenggong/Program_Files/System/__logo__.py`

 * *Files identical despite different names*

### Comparing `lichenggong-0.3.1.0/lichenggong/Program_Files/System/__n_time__.py` & `lichenggong-0.4.0.0/lichenggong/Program_Files/System/__n_time__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding=utf-8
 import gc
 
 
-def noodows_time(choose):
+def time(choose):
     def get_month_days(year, month):
         if month > 12 or month <= 0:
             return -1
         if month == 2:
             return 29 if year % 4 == 0 and year % 100 != 0 or year % 400 == 0 else 28
         if month in (4, 6, 9, 11):
             return 30
```

### Comparing `lichenggong-0.3.1.0/lichenggong/Program_Files/System/__user__.py` & `lichenggong-0.4.0.0/lichenggong/Program_Files/System/__user__.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,23 +3,25 @@
 # 祖宗之法不可变 切记
 
 import gc
 import os
 import shutil
 
 
-def __u_first__(__first):
+def u_first():
     with open('../Noodows//version//version.txt', 'r') as Version_version:
         version = Version_version.readline()  # read the version
     with open('../Noodows//version//build_version.txt', 'r') as Build_version:
         build_version = Build_version.readline()  # read the version
     print()
     print('您正在使用巨硬产品 noodows yee{0}(测试{1}) 无图像版 (用户创建区)'.format(version, build_version))
     print("You're use noodows yee{0}(build{1}) no Image by Big-hard (setup user)".format(version, build_version))
     print()
+    print("本系统基于交互环境")
+    print()
     print('设置语言')
     print('Setup language')
     print()
     while 1:
         input_language = input('language(first):      1.English 2.简体中文 3.繁體中文')
         if input_language != '1' and input_language != '2' and input_language != '3':
             print()
@@ -45,40 +47,40 @@
         print('您两次输入的语言不一样！')
         print('the first language is not the second one!')
         print()
 
     # setup language
     def first_language_packager(the_language, model, language_choose):
         # how to use the language
-
+        # 语言包，早期的无奈之举
         language_package = [
             'setup a user',
             '创造用户',
-            '创造用户',
+            '創建用戶',
             'name(first):',
             '名(第一次):',
-            '名(初次):',
+            '用戶名(初次):',
             'name(again):',
             '名(第二次):',
-            '名(再次):',
+            '用戶名(再次):',
             'do you want to have  a password?         1.yes 2.no',
             '是否需要密码？         1.是的 2.不需要',
-            '是否需要密码？         1.是 2.否',
+            '需要密碼？         1.是 2.否',
             'password(first):',
             '密码(第一次):',
-            '密码(初次):',
+            '用戶密碼(初次):',
             'password(again):',
             '密码(第二次):',
-            '密码(再次):',
+            '用戶密碼(再次):',
             "what's the user's power?         1.admin 2.user 3.visitor",
             '此用户的权限是？         1.管理员 2.用户 3.游客',
-            '此用户的权限？         1.管理 2.用户 3.旅者',
+            '用戶權限？         1.管理 2.用戶 3.旅者',
             "that's your user,right?         1.yes 2.no",
             '这是否是你的用户？         1.是的 2.不是',
-            '此是否是此用户？         1.是 2.否'
+            '此是否是你的用戶？         1.是 2.否'
         ]
         if the_language == right_language:
             if model == 'print':
                 print(language_package[language_choose])
             elif model == 'input':
                 print(language_package[language_choose], end='')
             else:
@@ -128,18 +130,14 @@
             check_password = input()
             if check_password == '1':
                 print()
                 first_language_packager('US_en', 'input', 12)
                 first_language_packager('ZN_cn', 'input', 13)
                 first_language_packager('Zn_tw', 'input', 14)
                 input_password = input()
-                if input_password == 'nothing':
-                    print("are you serious?")
-                    print("error: input a nul thing")
-                    continue
                 print()
                 first_language_packager('US_en', 'input', 15)
                 first_language_packager('ZN_cn', 'input', 16)
                 first_language_packager('ZN_tw', 'input', 17)
                 check_password = input()
                 if check_password == input_password:
                     print()
@@ -152,40 +150,19 @@
             elif check_password == '2':
                 print()
                 right_password = "nothing"
                 break
             else:
                 print("error: input an undefined thing")
         # setup user password
-        while 1:
-            if __first == 0:
-                right_power = 'admin'
-            else:
-                first_language_packager('US_en', 'input', 18)
-                first_language_packager('ZN_cn', 'input', 19)
-                first_language_packager('ZN_tw', 'input', 20)
-                power = input()
-                if power == '1':
-                    right_power = 'admin'
-                elif power == '2':
-                    right_power = 'user'
-                elif power == '3':
-                    right_power = 'visitor'
-                else:
-                    print()
-                    print("error: input an undefined thing")
-                    print()
-                    continue
-            break
-        # set up the field of power
         print()
         print('ID:{0}'.format(right_id))
         print('name:{0}'.format(right_name))
         print('password:{0}'.format(right_password))
-        print('power:{0}'.format(power))
+        print('power:{0}'.format('admin'))
         print()
         first_language_packager('US_en', 'input', 21)
         first_language_packager('ZN_cn', 'input', 22)
         first_language_packager('ZN_tw', 'input', 23)
         choice = input()
         if choice == "1":
             print()
@@ -197,22 +174,38 @@
             folder_user_used = folder + 'User_used'
             users_language = folder + 'language.txt'
             users_name = folder + 'name.txt'
             users_password = folder + 'password.txt'
             users_power = folder + 'power.txt'
             print()
             print('10%', end=" ")
-            if __first == 0:
+            try:
                 os.makedirs(folder)
+            except FileExistsError:
+                pass
+            try:
                 os.makedirs(folder_user_used)
-                if __first == 0:
-                    os.makedirs('./now')
-                    os.makedirs('../User')
-                    os.makedirs('../User//UserPE')
-                    os.makedirs('../User//UserPE//User_used')
+            except FileExistsError:
+                pass
+            try:
+                os.makedirs('./now')
+            except FileExistsError:
+                pass
+            try:
+                os.makedirs('../User')
+            except FileExistsError:
+                pass
+            try:
+                os.makedirs('../User//UserPE')
+            except FileExistsError:
+                pass
+            try:
+                os.makedirs('../User//UserPE//User_used')
+            except FileExistsError:
+                pass
             print()
             print('20%', end=" ")
             with open(users_language, 'w', encoding="utf-8") as Language:
                 Language.write(right_language)
             with open('../User//UserPE//language.txt', 'w', encoding="utf-8") as Language:
                 Language.write('US_en')
             print()
@@ -223,41 +216,38 @@
                 Name.write(right_name)
             with open('../User//UserPE//name.txt', 'w', encoding="utf-8") as Name:
                 Name.write('PE')
             print()
             print('50%', end=" ")
             with open(users_password, 'w', encoding="utf-8") as Password:
                 Password.write(right_password)
-            with open(users_password, 'w', encoding="utf-8") as Password:
+            with open('../User//UserPE//password.txt', 'w', encoding="utf-8") as Password:
                 Password.write('nothing')
             print()
             print('60%', end=" ")
             with open(users_power, 'w', encoding="utf-8") as Power:
-                Power.write(right_power)
-            with open(users_power, 'w', encoding="utf-8") as Power:
-                Power.write(right_power)
+                Power.write('admin')
+            with open('../User//UserPE//password.txt', 'w', encoding="utf-8") as Power:
+                Power.write('admin')
             print()
             print('100%')
             break
         elif choice == '2':
             print("OK!let's back")
     print()
     print('欢迎使用')
     print('Thank you for your support!')
     del Version_version, version, Build_version, build_version, input_language, check_language, first_language_packager
     del input_id, check_id, input_name, check_name, check_password
-    del right_language, right_id, right_name, right_password, power
+    del right_language, right_id, right_name, right_password
     del choice, users_language, users_name, users_password, users_power, Language, Name, Password, Power
     gc.collect()
 
 
 def change():
-    """
-
-    """
     with open('../Noodows//version//version.txt', 'r') as Version_version:
         version = Version_version.readline()  # read the version
     with open('../Noodows//version//build_version.txt', 'r') as Build_version:
         build_version = Build_version.readline()  # read the version
     print('您正在使用巨硬产品 noodows yee{0}(测试{1}) 无图像版 (用户更改区)'.format(version, build_version))
     print("You're use noodows yee{0}(build{1}) no Image by Big-hard (setup user)".format(version, build_version))
     print('操作风险,数据至上')
@@ -293,17 +283,14 @@
         print("error: input an undefined thing")
     del change_thing, ID, right_id, users_language, language, right_language, users_name, name, right_name
     del users_password, password, right_password, users_power, power, right_power
     gc.collect()
 
 
 def user():
-    """
-
-    """
     user_list = []
     for root, dirs, file in os.walk('..//User//'):
         try:
             with open(root + '//name.txt', 'r', encoding="utf-8") as name:
                 user_list.append(['ID:' + root.lstrip('..//User//User'), 'name:' + name.readline()])
         except FileNotFoundError:
             pass
@@ -378,7 +365,237 @@
                 break
     del user_list, root, dirs, file, name
     del i, input_id, right_id, choose, folder
     del user_language, user_name, user_password, user_power, language, password, power
     del users_language, users_name, users_password, users_power
     del Language, Name, Password, Power
     gc.collect()
+
+
+def u_new():
+    with open('../Noodows//version//version.txt', 'r') as Version_version:
+        version = Version_version.readline()  # read the version
+    with open('../Noodows//version//build_version.txt', 'r') as Build_version:
+        build_version = Build_version.readline()  # read the version
+    print()
+    print('您正在使用巨硬产品 noodows yee{0}(测试{1}) 无图像版 (用户创建区)'.format(version, build_version))
+    print("You're use noodows yee{0}(build{1}) no Image by Big-hard (setup user)".format(version, build_version))
+    print()
+    print("本系统基于交互环境")
+    print()
+    print('设置语言')
+    print('Setup language')
+    print()
+    while 1:
+        input_language = input('language(first):      1.English 2.简体中文 3.繁體中文')
+        if input_language != '1' and input_language != '2' and input_language != '3':
+            print()
+            print("error: input an undefined thing")
+            continue
+        print()
+        check_language = input('language(again):      1.English 2.简体中文 3.繁體中文')
+        if check_language != '1' and check_language != '2' and check_language != '3':
+            print()
+            print("error: input an undefined thing")
+            print()
+            continue
+        if check_language == input_language:
+            right_language = input_language
+            if right_language == '1':
+                right_language = 'US_en'
+            elif right_language == '2':
+                right_language = 'ZN_cn'
+            elif right_language == '3':
+                right_language = 'ZN_tw'
+            break
+        print()
+        print('您两次输入的语言不一样！')
+        print('the first language is not the second one!')
+        print()
+
+    # setup language
+    def language_packager(the_language, model, language_choose):
+        # how to use the language
+        # 语言包，早期的无奈之举
+        language_package = [
+            'setup a user',
+            '创造用户',
+            '創建用戶',
+            'name(first):',
+            '名(第一次):',
+            '用戶名(初次):',
+            'name(again):',
+            '名(第二次):',
+            '用戶名(再次):',
+            'do you want to have  a password?         1.yes 2.no',
+            '是否需要密码？         1.是的 2.不需要',
+            '需要密碼？         1.是 2.否',
+            'password(first):',
+            '密码(第一次):',
+            '用戶密碼(初次):',
+            'password(again):',
+            '密码(第二次):',
+            '用戶密碼(再次):',
+            "what's the user's power?         1.admin 2.user 3.visitor",
+            '此用户的权限是？         1.管理员 2.用户 3.游客',
+            '用戶權限？         1.管理 2.用戶 3.旅者',
+            "that's your user,right?         1.yes 2.no",
+            '这是否是你的用户？         1.是的 2.不是',
+            '此是否是你的用戶？         1.是 2.否'
+        ]
+        if the_language == right_language:
+            if model == 'print':
+                print(language_package[language_choose])
+            elif model == 'input':
+                print(language_package[language_choose], end='')
+            else:
+                print('error: input an undefined thing')
+
+    print()
+    language_packager('US_en', 'print', 0)
+    language_packager('ZN_cn', 'print', 1)
+    language_packager('ZN_tw', 'print', 2)
+    while 1:
+        while 1:
+            print()
+            input_id = input('ID(1st):')
+            print()
+            check_id = input('ID(2nd):')
+            if check_id == input_id:
+                right_id = input_id
+                print()
+                break
+            print()
+            print('错误: 您两次输入的ID不一样！')
+            print('error: the first ID you input is not the second one!')
+        # setup user ID
+        while 1:
+            language_packager('US_en', 'input', 3)
+            language_packager('ZN_cn', 'input', 4)
+            language_packager('ZN_tw', 'input', 5)
+            input_name = input()
+            print()
+            language_packager('US_en', 'input', 6)
+            language_packager('ZN_cn', 'input', 7)
+            language_packager('ZN_tw', 'input', 8)
+            check_name = input()
+            if check_name == input_name:
+                print()
+                right_name = input_name
+                break
+            print()
+            print('错误: 您两次输入的名字不一样！')
+            print('error: the first name you input is not the second one!')
+            print()
+        # setup username
+        while 1:
+            language_packager('US_en', 'input', 9)
+            language_packager('ZN_cn', 'input', 10)
+            language_packager('ZN_tw', 'input', 11)
+            check_password = input()
+            if check_password == '1':
+                print()
+                language_packager('US_en', 'input', 12)
+                language_packager('ZN_cn', 'input', 13)
+                language_packager('Zn_tw', 'input', 14)
+                input_password = input()
+                print()
+                language_packager('US_en', 'input', 15)
+                language_packager('ZN_cn', 'input', 16)
+                language_packager('ZN_tw', 'input', 17)
+                check_password = input()
+                if check_password == input_password:
+                    print()
+                    right_password = input_password
+                    break
+                print()
+                print('错误: 您两次输入的密码不一样！')
+                print('error: the first password you input is not the second one!')
+                print()
+            elif check_password == '2':
+                print()
+                right_password = "nothing"
+                break
+            else:
+                print("error: input an undefined thing")
+        # setup user password
+        while 1:
+            language_packager('US_en', 'input', 18)
+            language_packager('ZN_cn', 'input', 19)
+            language_packager('ZN_tw', 'input', 20)
+            power = input()
+            if power == '1':
+                right_power = 'admin'
+            elif power == '2':
+                right_power = 'user'
+            elif power == '3':
+                right_power = 'visitor'
+            else:
+                print()
+                print("error: input an undefined thing")
+                print()
+                continue
+            break
+        # set up the field of power
+        print()
+        print('ID:{0}'.format(right_id))
+        print('name:{0}'.format(right_name))
+        print('password:{0}'.format(right_password))
+        print('power:{0}'.format(right_power))
+        print()
+        language_packager('US_en', 'input', 21)
+        language_packager('ZN_cn', 'input', 22)
+        language_packager('ZN_tw', 'input', 23)
+        choice = input()
+        if choice == "1":
+            print()
+            print('马上就好')
+            print("It'll only take a second")
+            print()
+            print('0%', end=" ")
+            folder = '../User//User' + right_id + '//'
+            folder_user_used = folder + 'User_used'
+            users_language = folder + 'language.txt'
+            users_name = folder + 'name.txt'
+            users_password = folder + 'password.txt'
+            users_power = folder + 'power.txt'
+            print()
+            print('10%', end=" ")
+            try:
+                os.makedirs(folder)
+            except FileExistsError:
+                pass
+            try:
+                os.makedirs(folder_user_used)
+            except FileExistsError:
+                pass
+            print()
+            print('20%', end=" ")
+            with open(users_language, 'w', encoding="utf-8") as Language:
+                Language.write(right_language)
+            print()
+            print('30%')
+            print()
+            print('40%', end=" ")
+            with open(users_name, 'w', encoding="utf-8") as Name:
+                Name.write(right_name)
+            print()
+            print('50%', end=" ")
+            with open(users_password, 'w', encoding="utf-8") as Password:
+                Password.write(right_password)
+            print()
+            print('60%', end=" ")
+            with open(users_power, 'w', encoding="utf-8") as Power:
+                Power.write(right_power)
+            print()
+            print('100%')
+            break
+        elif choice == '2':
+            print("OK!let's back")
+    print()
+    print('欢迎使用')
+    print('Thank you for your support!')
+    del Version_version, version, Build_version, build_version, input_language, check_language, language_packager
+    del input_id, check_id, input_name, check_name, check_password
+    del right_language, right_id, right_name, right_password, right_power
+    del choice, users_language, users_name, users_password, users_power, Language, Name, Password, Power
+    gc.collect()
```

### Comparing `lichenggong-0.3.1.0/lichenggong/__init__.py` & `lichenggong-0.4.0.0/lichenggong/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 def start():
-    import platform, sys,os
+    import platform, sys, os
     if platform.system() == "Windows":
         print('Windows :(')
     elif platform.system() == "Linux":
         print('!!!!Linux!!!!!')
     elif platform.system() == "Cygwin":
         print('!!!Cygwin!!!')
     elif platform.system() == "Darwin":
         print('!!!!!Mac!!!!!!')
     elif platform.system() == "Java":
         print('Java????!!!')
     else:
         print("?!")
     with open(sys.path[-2] + '//Lib//site-packages//lichenggong//Noodows//python.txt', "w", encoding="utf-8") as python:
         python.write(sys.path[-2])
-    print('change dir to {0}{1}'.format(sys.path[-2],'//Lib//site-packages//lichenggong//Noodows'))
+    print('change dir to {0}{1}'.format(sys.path[-2], '//Lib//site-packages//lichenggong//Noodows'))
     os.chdir(sys.path[-2] + '//Lib//site-packages//lichenggong//Noodows')
     print(os.getcwd())
     sys.path.append('./')
     import __noodows__
-    __noodows__.__n_start__()
+    __noodows__.__n_start__()
```

### Comparing `lichenggong-0.3.1.0/lichenggong.egg-info/SOURCES.txt` & `lichenggong-0.4.0.0/lichenggong.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -12,12 +12,12 @@
 lichenggong/Noodows/practice.py
 lichenggong/Noodows/python.txt
 lichenggong/Noodows/update.log
 lichenggong/Noodows/version/build_version.txt
 lichenggong/Noodows/version/version.txt
 lichenggong/Program_Files/System/__calc__.py
 lichenggong/Program_Files/System/__logo__.py
+lichenggong/Program_Files/System/__n_explorer__.py
 lichenggong/Program_Files/System/__n_time__.py
-lichenggong/Program_Files/System/__start_menu__.py
 lichenggong/Program_Files/System/__thanks__.py
 lichenggong/Program_Files/System/__user__.py
 lichenggong/Program_Files/User/_.py
```

### Comparing `lichenggong-0.3.1.0/setup.py` & `lichenggong-0.4.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 # coding=utf-8
 from setuptools import setup
+
 with open(".\\lichenggong\\Noodows\\version\\version.txt", 'r') as f1:
     version = f1.readline()
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
+
 setup(
     packages=['lichenggong',
               'lichenggong.Noodows',
               'lichenggong.Noodows.version',
               'lichenggong.Program_Files.System',
               'lichenggong.Program_Files.User'],
     name="lichenggong",
     version=version,
     description="python 3   windows 10 (best)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='',
-    package_data={'':['*.py','*.txt','*.log']},
+    package_data={'': ['*.py', '*.txt', '*.log']},
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3")
```

