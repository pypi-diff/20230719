# Comparing `tmp/easy-ernie-0.1.5.tar.gz` & `tmp/easy-ernie-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy-ernie-0.1.5.tar", last modified: Mon Jun 26 11:28:14 2023, max compression
+gzip compressed data, was "easy-ernie-0.1.6.tar", last modified: Wed Jul 19 06:43:40 2023, max compression
```

## Comparing `easy-ernie-0.1.5.tar` & `easy-ernie-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 11:28:14.929861 easy-ernie-0.1.5/
--rw-rw-rw-   0        0        0     1065 2023-04-26 08:52:25.000000 easy-ernie-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     2226 2023-06-26 11:28:14.929371 easy-ernie-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1548 2023-05-12 11:13:36.000000 easy-ernie-0.1.5/README.md
--rw-rw-rw-   0        0        0       42 2023-06-26 11:28:14.929861 easy-ernie-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      936 2023-05-06 11:29:36.000000 easy-ernie-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-26 11:28:14.922357 easy-ernie-0.1.5/src/
-drwxrwxrwx   0        0        0        0 2023-06-26 11:28:14.928871 easy-ernie-0.1.5/src/easy_ernie/
--rw-rw-rw-   0        0        0      126 2023-05-06 11:29:23.000000 easy-ernie-0.1.5/src/easy_ernie/__init__.py
--rw-rw-rw-   0        0        0     7248 2023-06-26 09:57:08.000000 easy-ernie-0.1.5/src/easy_ernie/ernie.py
--rw-rw-rw-   0        0        0      985 2023-05-13 09:56:44.000000 easy-ernie-0.1.5/src/easy_ernie/fast_ernie.py
-drwxrwxrwx   0        0        0        0 2023-06-26 11:28:14.927371 easy-ernie-0.1.5/src/easy_ernie.egg-info/
--rw-rw-rw-   0        0        0     2226 2023-06-26 11:28:14.000000 easy-ernie-0.1.5/src/easy_ernie.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      341 2023-06-26 11:28:14.000000 easy-ernie-0.1.5/src/easy_ernie.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 11:28:14.000000 easy-ernie-0.1.5/src/easy_ernie.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-26 11:28:14.000000 easy-ernie-0.1.5/src/easy_ernie.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-26 11:28:14.000000 easy-ernie-0.1.5/src/easy_ernie.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-19 06:43:40.510419 easy-ernie-0.1.6/
+-rw-rw-rw-   0        0        0     1065 2023-04-26 08:52:25.000000 easy-ernie-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     2226 2023-07-19 06:43:40.509928 easy-ernie-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1548 2023-07-19 06:37:02.000000 easy-ernie-0.1.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-19 06:43:40.510419 easy-ernie-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      936 2023-07-19 06:37:05.000000 easy-ernie-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 06:43:40.502920 easy-ernie-0.1.6/src/
+drwxrwxrwx   0        0        0        0 2023-07-19 06:43:40.509418 easy-ernie-0.1.6/src/easy_ernie/
+-rw-rw-rw-   0        0        0      126 2023-07-19 06:37:12.000000 easy-ernie-0.1.6/src/easy_ernie/__init__.py
+-rw-rw-rw-   0        0        0     7577 2023-07-19 06:40:50.000000 easy-ernie-0.1.6/src/easy_ernie/ernie.py
+-rw-rw-rw-   0        0        0      985 2023-07-19 06:33:57.000000 easy-ernie-0.1.6/src/easy_ernie/fast_ernie.py
+drwxrwxrwx   0        0        0        0 2023-07-19 06:43:40.507919 easy-ernie-0.1.6/src/easy_ernie.egg-info/
+-rw-rw-rw-   0        0        0     2226 2023-07-19 06:43:40.000000 easy-ernie-0.1.6/src/easy_ernie.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      494 2023-07-19 06:43:40.000000 easy-ernie-0.1.6/src/easy_ernie.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 06:43:40.000000 easy-ernie-0.1.6/src/easy_ernie.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-19 06:43:40.000000 easy-ernie-0.1.6/src/easy_ernie.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-19 06:43:40.000000 easy-ernie-0.1.6/src/easy_ernie.egg-info/top_level.txt
```

### Comparing `easy-ernie-0.1.5/LICENSE` & `easy-ernie-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `easy-ernie-0.1.5/PKG-INFO` & `easy-ernie-0.1.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-ernie
-Version: 0.1.5
+Version: 0.1.6
 Summary: 简洁的调用文心一言的WebAPI
 Home-page: https://github.com/XiaoXinYo/Easy-Ernie
 Author: XiaoXinYo
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -17,15 +17,15 @@
 License-File: LICENSE
 
 ## 提示
 1. 有封号风险.
 2. 由于文心一言的Acs-Token算法的参数不定时的变化,所以包里调用了API.感兴趣的或有自动更新方法的可以联系我.
 3. 若出现了`用户访问被限制`请到[Isuue](https://github.com/XiaoXinYo/Easy-Ernie/issues/6)回复,我会及时更新Acs-Token算法的参数.
 ---
-![Release](https://img.shields.io/badge/Release-0.1.5-blue)
+![Release](https://img.shields.io/badge/Release-0.1.6-blue)
 ---
 ## 介绍
 简洁的调用文心一言的WebAPI
 ## 需求
 1. 语言: Python3.8+.
 2. 包: requests.
 3. 其他: 文心一言账户.
```

### Comparing `easy-ernie-0.1.5/README.md` & `easy-ernie-0.1.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ## 提示
 1. 有封号风险.
 2. 由于文心一言的Acs-Token算法的参数不定时的变化,所以包里调用了API.感兴趣的或有自动更新方法的可以联系我.
 3. 若出现了`用户访问被限制`请到[Isuue](https://github.com/XiaoXinYo/Easy-Ernie/issues/6)回复,我会及时更新Acs-Token算法的参数.
 ---
-![Release](https://img.shields.io/badge/Release-0.1.5-blue)
+![Release](https://img.shields.io/badge/Release-0.1.6-blue)
 ---
 ## 介绍
 简洁的调用文心一言的WebAPI
 ## 需求
 1. 语言: Python3.8+.
 2. 包: requests.
 3. 其他: 文心一言账户.
```

### Comparing `easy-ernie-0.1.5/setup.py` & `easy-ernie-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 with open('./README.md', 'r', encoding='utf-8') as file:
     long_description = file.read()
 
 setup(
     name='easy-ernie',
-    version='0.1.5',
+    version='0.1.6',
     description='简洁的调用文心一言的WebAPI',
     long_description=long_description,
-    long_description_content_type="text/markdown",
+    long_description_content_type='text/markdown',
     author='XiaoXinYo',
     url='https://github.com/XiaoXinYo/Easy-Ernie',
     packages=find_packages('./src'),
     license='MIT',
     package_dir={'': './src'},
     classifiers=[
         'License :: OSI Approved :: MIT License',
```

### Comparing `easy-ernie-0.1.5/src/easy_ernie/ernie.py` & `easy-ernie-0.1.6/src/easy_ernie/ernie.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,49 +10,49 @@
     return int(time.time() * 1000)
 
 class Ernie:
     def __init__(self, BAIDUID: str, BDUSS_BFESS: str):
         self.BAIDUID = BAIDUID
         self.session = requests.Session()
         self.session.headers = {
-            'Host': 'yiyan.baidu.com',
+            'Accept': '*/*',
+            'Accept-Encoding': 'gzip, deflate, br',
+            'Accept-Language': 'zh-CN,zh;q=0.9,en;q=0.8,en-GB;q=0.7,en-US;q=0.6',
+            'Acs-Token': '',
             'Connection': 'keep-alive',
             'Content-Length': '0',
-            'sec-ch-ua': '"Chromium";v="112", "Microsoft Edge";v="112", "Not:A-Brand";v="99"',
             'Content-Type': 'application/json',
-            'Acs-Token': '',
-            'sec-ch-ua-mobile': '?0',
-            'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36 Edg/112.0.1722.58',
-            'sec-ch-ua-platform': '"macOS"',
-            'Accept': '*/*',
+            'Cookie': f'BDUSS_BFESS={BDUSS_BFESS};',
+            'Host': 'yiyan.baidu.com',
             'Origin': 'https://yiyan.baidu.com',
-            'Sec-Fetch-Site': 'same-site',
-            'Sec-Fetch-Mode': 'cors',
-            'Sec-Fetch-Dest': 'empty',
             'Referer': 'https://yiyan.baidu.com/',
-            'Accept-Encoding': 'gzip, deflate, br',
-            'Accept-Language': 'zh-CN,zh;q=0.9,en;q=0.8,en-GB;q=0.7,en-US;q=0.6',
-            'Cookie': f'BDUSS_BFESS={BDUSS_BFESS};'
+            'Sec-Ch-Ua': '"Not.A/Brand";v="8", "Chromium";v="114", "Microsoft Edge";v="114"',
+            'Sec-Ch-Ua-Mobile': '?0',
+            'Sec-Ch-Ua-Platform': '"Windows"',
+            'Sec-Fetch-Dest': 'empty',
+            'Sec-Fetch-Mode': 'cors',
+            'Sec-Fetch-Site': 'same-site',
+            'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36 Edg/114.0.1823.67'
         }
     
-    def getSign(self) -> str:
+    def getAcsToken(self) -> str:
         data = requests.get(f'https://api.hack-er.cn/ernie/acs_token?BAIDUID={self.BAIDUID}',).json()
         return data['data']
     
     def checkRequest(self) -> None:
         if self.request.status_code != 200:
-            raise Exception('请求失败,请检查网络')
+            raise Exception('请求失败,检查网络')
         
         try:
-            self.request.json()
+            data = self.request.json()
         except:
             raise Exception('请求失败,响应格式错误')
         
-        if self.request.json()['code'] != 0:
-            raise Exception(f'请求失败,{self.request.json()["msg"]}')
+        if data['code'] != 0:
+            raise Exception(f'请求失败,{data["msg"]}')
 
     def get(self, url: str, check=True) -> requests:
         self.request = self.session.get(url)
         if check:
             self.checkRequest()
         return self.request
     
@@ -63,151 +63,159 @@
             self.checkRequest()
         return self.request
     
     def getConversation(self) -> Union[None, list]:
         data = self.post(
             f'https://yiyan.baidu.com/eb/session/list',
             {
-                'pageSize': 1000,
                 'deviceType': 'pc',
+                'pageSize': 1000,
                 'timestamp': getTimestamp()
             }
         ).json()
         return data['data']['sessions']
 
     def newConversation(self, name: str) -> str:
         data = self.post(
             'https://yiyan.baidu.com/eb/session/new',
             {
-                'sessionName': name,
-                'timestamp': getTimestamp(),
                 'deviceType': 'pc',
-                'plugins': []
+                'plugins': [],
+                'sessionName': name,
+                'timestamp': getTimestamp()
             }
         ).json()
         return data['data']['sessionId']
     
     def deleteConversation(self, sessionId: str) -> bool:
         data = self.post(
             'https://yiyan.baidu.com/eb/session/delete',
             {
+                'deviceType': 'pc',
                 'sessionId': sessionId,
-                'timestamp': getTimestamp(),
-                'deviceType': 'pc'
+                'timestamp': getTimestamp()
             },
-            False
+            check=False
         ).json()
         return True if data['code'] == 0 else False
 
     def renameConversation(self, sessionId: str, name: str) -> bool:
         self.post(
             'https://yiyan.baidu.com/eb/session/new',
             {
+                'deviceType': 'pc',
                 'sessionId': sessionId,
                 'sessionName': name,
-                'timestamp': getTimestamp(),
-                'deviceType': 'pc'
+                'timestamp': getTimestamp()
             }
         )
         return True
     
-    def getParentChatId(self, sessionId: str) -> Union[None, str]:
+    def getConversationHistory(self, sessionId: str) -> Union[None, dict]:
         data = self.post(
             'https://yiyan.baidu.com/eb/chat/history',
             {
-                'sessionId': sessionId,
+                'deviceType': 'pc',
                 'pageSize': 2000,
+                'sessionId': sessionId,
                 'timestamp': getTimestamp(),
-                'deviceType': 'pc'
             }
         ).json()
-        return data['data']['currentChatId']
+        chats = data['data']['chats']
+        if not chats:
+            return None
+        histories = []
+        for chat in chats.values():
+            histories.append({
+                'id': chat['id'],
+                'role': chat['role'],
+                'text': chat['message'][0]['content']
+            })
+        return {
+            'histories': histories,
+            'currentChatId': str(data['data']['currentChatId'])
+        }
 
     def askStream(self, question: str, sessionId: str, parentChatId: str) -> Generator:
         self.post(
             'https://yiyan.baidu.com/eb/chat/checkAndBan',
             {
+                'deviceType': 'pc',
                 'text': question,
                 'timestamp': getTimestamp(),
-                'deviceType': 'pc'
             }
         )
 
-        sign = self.getSign()
-        self.session.headers['Acs-Token'] = sign
+        acsToken = self.getAcsToken()
+        self.session.headers['Acs-Token'] = acsToken
         data = self.post(
             'https://yiyan.baidu.com/eb/chat/new',
             {
-                'sessionId': sessionId,
-                'text': question,
-                'parentChatId': parentChatId,
-                'type': 10,
-                'timestamp': getTimestamp(),
-                'deviceType': 'pc',
                 'code': 0,
-                'msg': '',
+                'deviceType': 'pc',
                 'jt': '',
-                'sign': sign,
+                'msg': '',
+                'parentChatId': parentChatId,
                 'pluginInfo': [],
-                'plugins': []
+                'plugins': [],
+                'sessionId': sessionId,
+                'sign': acsToken,
+                'text': question,
+                'timestamp': getTimestamp(),
+                'type': 10
             }
         ).json()
         botChatId = data['data']['botChat']['id']
         botParentChatId = data['data']['botChat']['parent']
 
-        fullAnswer = ''
-        pattern = r'<img[^>]*\ssrc=[\'"]([^\'"]+)[\'"][^>]*\s/>'
-        urls = []
+        imagePattern = r'<img[^>]*\ssrc=[\'"]([^\'"]+)[\'"][^>]*\s/>'
         sentenceId = 0
+        stop = 0
         while True:
-            sign = self.getSign()
-            self.session.headers['Acs-Token'] = sign
+            acsToken = self.getAcsToken()
+            self.session.headers['Acs-Token'] = acsToken
             data = self.post(
                 'https://yiyan.baidu.com/eb/chat/query',
                 {
                     'chatId': botChatId,
+                    'deviceType': 'pc',
                     'parentChatId': botParentChatId,
                     'sentenceId': sentenceId,
-                    'sessionId': '',
-                    'stop': 0,
+                    'sessionId': sessionId,
+                    'sign': acsToken,
+                    'stop': stop,
                     'timestamp': getTimestamp(),
-                    'deviceType': 'pc',
-                    'sign': sign
                 }
             ).json()
+
             data = data['data']
             sentenceId = data['sent_id']
-            content = data['content']
-            
-            if content.strip():
-                fullAnswer += content
-                content = re.sub(pattern, '', content)
-                content = content.replace('<br>', '\n')
-                content = content.strip()
-
+            stop = data['stop']
+            answer = data['content']
+            if answer.strip():
+                answer = re.sub(imagePattern, '', answer)
+                answer = answer.replace('<br>', '\n')
+                answer = answer.strip()
                 yield {
-                    'answer': content,
-                    'urls': urls,
-                    'sessionId': sessionId,
+                    'answer': answer,
+                    'urls': re.findall(imagePattern, data['content']),
                     'botChatId': botChatId,
                     'done': False
                 }
 
-            if data['stop'] == 1 or data['is_end'] == 1:
+            if data['is_end'] == 1:
                 break
-        
-        urls.extend(re.findall(pattern, fullAnswer))
-        fullAnswer = re.sub(pattern, '', fullAnswer)
+
+        fullAnswer = data['tokens_all']
+        fullAnswer = re.sub(imagePattern, '', fullAnswer)
         fullAnswer = fullAnswer.replace('<br>', '\n')
         fullAnswer = fullAnswer.strip()
-        
         yield {
             'answer': fullAnswer,
-            'urls': urls,
-            'sessionId': sessionId,
+            'urls': re.findall(imagePattern, fullAnswer),
             'botChatId': botChatId,
             'done': True
         }
 
     def ask(self, question: str, sessionId: str='', parentChatId: str='') -> dict:
         result = {}
         for data in self.askStream(question, sessionId, parentChatId):
```

### Comparing `easy-ernie-0.1.5/src/easy_ernie/fast_ernie.py` & `easy-ernie-0.1.6/src/easy_ernie/fast_ernie.py`

 * *Files identical despite different names*

### Comparing `easy-ernie-0.1.5/src/easy_ernie.egg-info/PKG-INFO` & `easy-ernie-0.1.6/src/easy_ernie.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-ernie
-Version: 0.1.5
+Version: 0.1.6
 Summary: 简洁的调用文心一言的WebAPI
 Home-page: https://github.com/XiaoXinYo/Easy-Ernie
 Author: XiaoXinYo
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -17,15 +17,15 @@
 License-File: LICENSE
 
 ## 提示
 1. 有封号风险.
 2. 由于文心一言的Acs-Token算法的参数不定时的变化,所以包里调用了API.感兴趣的或有自动更新方法的可以联系我.
 3. 若出现了`用户访问被限制`请到[Isuue](https://github.com/XiaoXinYo/Easy-Ernie/issues/6)回复,我会及时更新Acs-Token算法的参数.
 ---
-![Release](https://img.shields.io/badge/Release-0.1.5-blue)
+![Release](https://img.shields.io/badge/Release-0.1.6-blue)
 ---
 ## 介绍
 简洁的调用文心一言的WebAPI
 ## 需求
 1. 语言: Python3.8+.
 2. 包: requests.
 3. 其他: 文心一言账户.
```

