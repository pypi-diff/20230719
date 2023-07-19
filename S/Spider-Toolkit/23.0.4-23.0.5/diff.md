# Comparing `tmp/Spider_Toolkit-23.0.4.tar.gz` & `tmp/Spider_Toolkit-23.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Spider_Toolkit-23.0.4.tar", last modified: Thu Jun 15 04:11:58 2023, max compression
+gzip compressed data, was "Spider_Toolkit-23.0.5.tar", last modified: Wed Jul 19 07:24:48 2023, max compression
```

## Comparing `Spider_Toolkit-23.0.4.tar` & `Spider_Toolkit-23.0.5.tar`

### file list

```diff
@@ -1,29 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 04:11:58.324568 Spider_Toolkit-23.0.4/
--rw-rw-rw-   0        0        0     1079 2023-06-09 06:25:44.000000 Spider_Toolkit-23.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0      614 2023-06-15 04:11:58.325569 Spider_Toolkit-23.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      466 2023-06-10 12:16:19.000000 Spider_Toolkit-23.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 04:11:58.266554 Spider_Toolkit-23.0.4/Spider_Toolkit/
--rw-rw-rw-   0        0        0        0 2023-06-09 06:40:11.000000 Spider_Toolkit-23.0.4/Spider_Toolkit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 04:11:58.288560 Spider_Toolkit-23.0.4/Spider_Toolkit/engine/
--rw-rw-rw-   0        0        0        0 2023-06-09 06:40:11.000000 Spider_Toolkit-23.0.4/Spider_Toolkit/engine/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 04:11:58.307564 Spider_Toolkit-23.0.4/Spider_Toolkit/filtering/
--rw-rw-rw-   0        0        0     2995 2023-06-15 03:43:24.000000 Spider_Toolkit-23.0.4/Spider_Toolkit/filtering/Download_Byte_parameter_filtering.py
--rw-rw-rw-   0        0        0      233 2023-06-12 12:18:02.000000 Spider_Toolkit-23.0.4/Spider_Toolkit/filtering/Open_js_parameter_filtering.py
--rw-rw-rw-   0        0        0      250 2023-06-15 03:44:44.000000 Spider_Toolkit-23.0.4/Spider_Toolkit/filtering/Random_ua_parameter_filtering.py
--rw-rw-rw-   0        0        0     5290 2023-06-12 12:18:18.000000 Spider_Toolkit-23.0.4/Spider_Toolkit/filtering/Save_parameter_filtering.py
--rw-rw-rw-   0        0        0        0 2023-06-09 06:40:11.000000 Spider_Toolkit-23.0.4/Spider_Toolkit/filtering/__init__.py
--rw-rw-rw-   0        0        0    24027 2023-06-15 03:51:05.000000 Spider_Toolkit-23.0.4/Spider_Toolkit/spidertools.py
-drwxrwxrwx   0        0        0        0 2023-06-15 04:11:58.324568 Spider_Toolkit-23.0.4/Spider_Toolkit/tools/
--rw-rw-rw-   0        0        0     6738 2023-06-15 03:59:13.000000 Spider_Toolkit-23.0.4/Spider_Toolkit/tools/Download_byte.py
--rw-rw-rw-   0        0        0      314 2023-06-10 08:09:27.000000 Spider_Toolkit-23.0.4/Spider_Toolkit/tools/Open_js.py
--rw-rw-rw-   0        0        0    28628 2023-06-15 03:45:42.000000 Spider_Toolkit-23.0.4/Spider_Toolkit/tools/Random_ua.py
--rw-rw-rw-   0        0        0     4200 2023-06-10 09:36:32.000000 Spider_Toolkit-23.0.4/Spider_Toolkit/tools/Save.py
--rw-rw-rw-   0        0        0        0 2023-06-09 06:40:11.000000 Spider_Toolkit-23.0.4/Spider_Toolkit/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 04:11:58.287560 Spider_Toolkit-23.0.4/Spider_Toolkit.egg-info/
--rw-rw-rw-   0        0        0      614 2023-06-15 04:11:58.000000 Spider_Toolkit-23.0.4/Spider_Toolkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      752 2023-06-15 04:11:58.000000 Spider_Toolkit-23.0.4/Spider_Toolkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 04:11:58.000000 Spider_Toolkit-23.0.4/Spider_Toolkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-06-15 04:11:58.000000 Spider_Toolkit-23.0.4/Spider_Toolkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-15 04:11:58.000000 Spider_Toolkit-23.0.4/Spider_Toolkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-15 04:11:58.326569 Spider_Toolkit-23.0.4/setup.cfg
--rw-rw-rw-   0        0        0     2072 2023-06-15 04:11:34.000000 Spider_Toolkit-23.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 07:24:48.706834 Spider_Toolkit-23.0.5/
+-rw-rw-rw-   0        0        0     1080 2023-07-19 07:14:48.000000 Spider_Toolkit-23.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      622 2023-07-19 07:24:48.706834 Spider_Toolkit-23.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      444 2023-07-19 07:20:36.000000 Spider_Toolkit-23.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-19 07:24:48.652822 Spider_Toolkit-23.0.5/Spider_Toolkit/
+-rw-rw-rw-   0        0        0        0 2023-06-09 06:40:11.000000 Spider_Toolkit-23.0.5/Spider_Toolkit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 07:24:48.671827 Spider_Toolkit-23.0.5/Spider_Toolkit/engine/
+-rw-rw-rw-   0        0        0        0 2023-06-09 06:40:11.000000 Spider_Toolkit-23.0.5/Spider_Toolkit/engine/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 07:24:48.690831 Spider_Toolkit-23.0.5/Spider_Toolkit/filtering/
+-rw-rw-rw-   0        0        0     2158 2023-07-19 01:41:54.000000 Spider_Toolkit-23.0.5/Spider_Toolkit/filtering/Download_Byte_parameter_filtering.py
+-rw-rw-rw-   0        0        0     1350 2023-07-19 06:50:04.000000 Spider_Toolkit-23.0.5/Spider_Toolkit/filtering/Download_m3u8_parameter_filtering.py
+-rw-rw-rw-   0        0        0      233 2023-06-12 12:18:02.000000 Spider_Toolkit-23.0.5/Spider_Toolkit/filtering/Open_js_parameter_filtering.py
+-rw-rw-rw-   0        0        0      250 2023-06-15 03:44:44.000000 Spider_Toolkit-23.0.5/Spider_Toolkit/filtering/Random_ua_parameter_filtering.py
+-rw-rw-rw-   0        0        0     5290 2023-06-12 12:18:18.000000 Spider_Toolkit-23.0.5/Spider_Toolkit/filtering/Save_parameter_filtering.py
+-rw-rw-rw-   0        0        0        0 2023-06-09 06:40:11.000000 Spider_Toolkit-23.0.5/Spider_Toolkit/filtering/__init__.py
+-rw-rw-rw-   0        0        0    12327 2023-07-19 06:50:04.000000 Spider_Toolkit-23.0.5/Spider_Toolkit/spidertools.py
+drwxrwxrwx   0        0        0        0 2023-07-19 07:24:48.706834 Spider_Toolkit-23.0.5/Spider_Toolkit/tools/
+-rw-rw-rw-   0        0        0    13041 2023-07-19 07:05:24.000000 Spider_Toolkit-23.0.5/Spider_Toolkit/tools/Download_byte.py
+-rw-rw-rw-   0        0        0     9155 2023-07-19 07:21:35.000000 Spider_Toolkit-23.0.5/Spider_Toolkit/tools/Download_m3u8.py
+-rw-rw-rw-   0        0        0      312 2023-06-30 08:59:29.000000 Spider_Toolkit-23.0.5/Spider_Toolkit/tools/Open_js.py
+-rw-rw-rw-   0        0        0    28570 2023-07-19 06:50:22.000000 Spider_Toolkit-23.0.5/Spider_Toolkit/tools/Random_ua.py
+-rw-rw-rw-   0        0        0     4200 2023-06-10 09:36:32.000000 Spider_Toolkit-23.0.5/Spider_Toolkit/tools/Save.py
+-rw-rw-rw-   0        0        0        0 2023-06-09 06:40:11.000000 Spider_Toolkit-23.0.5/Spider_Toolkit/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 07:24:48.670826 Spider_Toolkit-23.0.5/Spider_Toolkit.egg-info/
+-rw-rw-rw-   0        0        0      622 2023-07-19 07:24:48.000000 Spider_Toolkit-23.0.5/Spider_Toolkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      914 2023-07-19 07:24:48.000000 Spider_Toolkit-23.0.5/Spider_Toolkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 07:24:48.000000 Spider_Toolkit-23.0.5/Spider_Toolkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-07-19 07:24:48.000000 Spider_Toolkit-23.0.5/Spider_Toolkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-19 07:24:48.000000 Spider_Toolkit-23.0.5/Spider_Toolkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-19 07:24:48.707835 Spider_Toolkit-23.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     2089 2023-07-19 07:24:25.000000 Spider_Toolkit-23.0.5/setup.py
```

### Comparing `Spider_Toolkit-23.0.4/LICENSE.txt` & `Spider_Toolkit-23.0.5/LICENSE.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 MIT License
-Copyright (c) 2018 YOUR NAME
+Copyright (c) 2018 Uncle_Ming
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
 The above copyright notice and this permission notice shall be included in all
```

### Comparing `Spider_Toolkit-23.0.4/PKG-INFO` & `Spider_Toolkit-23.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: Spider_Toolkit
-Version: 23.0.4
+Version: 23.0.5
 Summary: 爬虫辅助模块
-Home-page: https://github.com/pypa/sampleproject
+Home-page: 
 Author: Uncle_Ming
 Author-email: 2462711716@qq.com
 Keywords: tools spider requests download
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE.txt
 
-爬虫辅助模块0.0.4版本修复了bug
+爬虫辅助模块0.0.5版本修复了bug,更新了m3u8下载器,优化了部分功能
```

### Comparing `Spider_Toolkit-23.0.4/Spider_Toolkit/filtering/Download_Byte_parameter_filtering.py` & `Spider_Toolkit-23.0.5/Spider_Toolkit/filtering/Download_Byte_parameter_filtering.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,87 +2,54 @@
 
 
 def donwload_byte_filtering(
         Max_Thread: int = 0,
         Max_Rerty: int = 3,
         Time_Sleep: [float, int] = 0,
         Request_Timeout: [float, int] = 10,
-        urls: list = None,
-        headers: [list[dict[str, any], None]] = None,
-        cookie: [list[dict[str, any], None]] = None,
-        param: [list[dict[str, any], None]] = None,
-        data: [list[dict[str, any], None]] = None,
-        proxies: [list[dict[str, any], None]] = None,
-        verify: bool = True,
-        path_: str = './',
-        type_: str = '',
-        names: [list, None] = None,
         Save_Error_Log: bool = True,
         Show_Progress_Bar: bool = False,
         Show_Error_Info: bool = True
 ):
+
     if type(Max_Thread) != int:
         raise '设置的MAX_THREAD不为整型'
     else:
         pass
 
     if type(Max_Rerty) != int:
         raise '设置的MAX_RETRY不为整型'
     else:
         pass
 
-    if type(Time_Sleep) != float or type(Time_Sleep) != int or type(Time_Sleep)!=list:
+    if type(Time_Sleep) != float or type(Time_Sleep) != int or type(Time_Sleep) != list:
         pass
     else:
         raise '设置的Time_Sleep不为整型,浮点型或列表'
 
     if type(Request_Timeout) != float or type(Request_Timeout) != int:
         pass
     else:
         raise '设置的的Request_Timeout不为整型或浮点型'
 
-    if type(urls) != list:
-        raise '设置的的urls不为列表'
-    if names!=None:
-        if type(names) != list:
-            raise '设置的的names不为列表'
-
-    if names != None and len(names) != len(urls):
-        raise '当前传入的urls与titles的长度不符'
-    else:
-        pass
-
     if Save_Error_Log != True and Save_Error_Log != False:
-        raise '错误日志保存只支持传入布尔类型'
+        raise '错误日志保存设置只支持传入布尔类型'
     else:
         pass
 
     if Show_Progress_Bar != True and Show_Progress_Bar != False:
         raise '进度条设置只支持传入布尔类型'
     else:
         pass
 
     if Show_Error_Info != True and Show_Error_Info != False:
-        raise '错误信息显示只支持传入布尔类型'
+        raise '错误信息显示设置只支持传入布尔类型'
     else:
         pass
 
-    if len(urls) < 1 or urls == None:
-        raise '未传入urls或urls为空'
-    else:
-        pass
-
-    if type(type_) != str:
-        raise 'type_只支持传入字符串类型'
-
-    if os.path.exists(path_):
-        pass
-    else:
-        os.makedirs(path_)
-
     return True
 
 
 def donwload_byte_function_filtering(
         url: str = None,
         headers: [dict[str, any], None] = None,
         cookie: [dict[str, any], None] = None,
@@ -95,13 +62,19 @@
         type_: str = ''
 ):
     if len(url) < 1 or url == None:
         raise '未传入url或url为空'
     else:
         pass
 
+    if type(name) != str:
+        raise 'name只支持传入字符串类型'
+
+    if type(type_) != str:
+        raise 'type_只支持传入字符串类型'
+
     if os.path.exists(path_):
         pass
     else:
         os.makedirs(path_)
 
     return True
```

### Comparing `Spider_Toolkit-23.0.4/Spider_Toolkit/filtering/Save_parameter_filtering.py` & `Spider_Toolkit-23.0.5/Spider_Toolkit/filtering/Save_parameter_filtering.py`

 * *Files identical despite different names*

### Comparing `Spider_Toolkit-23.0.4/Spider_Toolkit/tools/Random_ua.py` & `Spider_Toolkit-23.0.5/Spider_Toolkit/tools/Random_ua.py`

 * *Files 1% similar despite different names*

```diff
@@ -275,9 +275,8 @@
     elif factory=='safari':
         return random.choice(ua_list['safari'])
     elif factory=='opera':
         return random.choice(ua_list['opera'])
     elif factory=='ie':
         return random.choice(ua_list['ie'])
     else:
-        return random.choice(ua_list[random.choice(ua_list.keys())])
-
+        pass
```

### Comparing `Spider_Toolkit-23.0.4/Spider_Toolkit/tools/Save.py` & `Spider_Toolkit-23.0.5/Spider_Toolkit/tools/Save.py`

 * *Files identical despite different names*

### Comparing `Spider_Toolkit-23.0.4/Spider_Toolkit.egg-info/PKG-INFO` & `Spider_Toolkit-23.0.5/Spider_Toolkit.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: Spider-Toolkit
-Version: 23.0.4
+Version: 23.0.5
 Summary: 爬虫辅助模块
-Home-page: https://github.com/pypa/sampleproject
+Home-page: 
 Author: Uncle_Ming
 Author-email: 2462711716@qq.com
 Keywords: tools spider requests download
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE.txt
 
-爬虫辅助模块0.0.4版本修复了bug
+爬虫辅助模块0.0.5版本修复了bug,更新了m3u8下载器,优化了部分功能
```

### Comparing `Spider_Toolkit-23.0.4/Spider_Toolkit.egg-info/SOURCES.txt` & `Spider_Toolkit-23.0.5/Spider_Toolkit.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -7,16 +7,19 @@
 Spider_Toolkit.egg-info/PKG-INFO
 Spider_Toolkit.egg-info/SOURCES.txt
 Spider_Toolkit.egg-info/dependency_links.txt
 Spider_Toolkit.egg-info/requires.txt
 Spider_Toolkit.egg-info/top_level.txt
 Spider_Toolkit/engine/__init__.py
 Spider_Toolkit/filtering/Download_Byte_parameter_filtering.py
+Spider_Toolkit/filtering/Download_byte_parameter_filtering.py
+Spider_Toolkit/filtering/Download_m3u8_parameter_filtering.py
 Spider_Toolkit/filtering/Open_js_parameter_filtering.py
 Spider_Toolkit/filtering/Random_ua_parameter_filtering.py
 Spider_Toolkit/filtering/Save_parameter_filtering.py
 Spider_Toolkit/filtering/__init__.py
 Spider_Toolkit/tools/Download_byte.py
+Spider_Toolkit/tools/Download_m3u8.py
 Spider_Toolkit/tools/Open_js.py
 Spider_Toolkit/tools/Random_ua.py
 Spider_Toolkit/tools/Save.py
 Spider_Toolkit/tools/__init__.py
```

### Comparing `Spider_Toolkit-23.0.4/setup.py` & `Spider_Toolkit-23.0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from setuptools import setup, find_packages
 
 setup(
     # 以下为必需参数
     name='Spider_Toolkit',  # 模块名
-    version='23.0.4',  # 当前版本
+    version='23.0.5',  # 当前版本
     description='爬虫辅助模块',  # 简短描述
     packages=find_packages(),  # 多文件模块写法 exclude=['contrib', 'docs', 'tests']
     # 以下均为可选参数
-    long_description="爬虫辅助模块0.0.4版本修复了bug",  # 长描述
-    url='https://github.com/pypa/sampleproject',  # 主页链接
+    long_description="爬虫辅助模块0.0.5版本修复了bug,更新了m3u8下载器,优化了部分功能",  # 长描述
+    url='',  # 主页链接
     author='Uncle_Ming',  # 作者名
     author_email='2462711716@qq.com',  # 作者邮箱
     classifiers=[
         'Development Status :: 1 - Planning',  # 当前开发进度等级（测试版，正式版等）
         'License :: OSI Approved :: MIT License',  # 模块的license
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
     ],
     keywords='tools spider requests download',  # 模块的关键词，使用空格分割
-    install_requires=['requests','pandas','PyExecJS','pymysql','redis','pymongo'],  # 依赖模块
+    install_requires=['requests','pandas','PyExecJS','pymysql','redis','pymongo','Crypto'],  # 依赖模块
     # extras_require={  # 分组依赖模块，可使用pip install sampleproject[dev] 安装分组内的依赖
     #     'dev': ['check-manifest'],
     #     'test': ['coverage'],
     # },
     # package_data={  # 模块所需的额外文件
     #     'sample': ['package_data.dat'],
     # },
```

