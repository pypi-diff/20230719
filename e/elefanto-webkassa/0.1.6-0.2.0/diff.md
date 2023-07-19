# Comparing `tmp/elefanto_webkassa-0.1.6.tar.gz` & `tmp/elefanto_webkassa-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elefanto_webkassa-0.1.6.tar", max compression
+gzip compressed data, was "elefanto_webkassa-0.2.0.tar", max compression
```

## Comparing `elefanto_webkassa-0.1.6.tar` & `elefanto_webkassa-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      172 2023-07-19 04:25:23.836094 elefanto_webkassa-0.1.6/README.md
--rw-r--r--   0        0        0      847 2023-07-19 08:43:19.261221 elefanto_webkassa-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      488 2023-07-19 07:43:50.241606 elefanto_webkassa-0.1.6/webkassa/__init__.py
--rw-r--r--   0        0        0     1384 2023-07-19 08:43:13.901335 elefanto_webkassa-0.1.6/webkassa/admin.py
--rw-r--r--   0        0        0      236 2023-07-18 06:59:32.374169 elefanto_webkassa-0.1.6/webkassa/apps.py
--rw-r--r--   0        0        0     3472 2023-07-19 08:01:54.584953 elefanto_webkassa-0.1.6/webkassa/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-07-18 04:42:18.150603 elefanto_webkassa-0.1.6/webkassa/migrations/__init__.py
--rw-r--r--   0        0        0     2930 2023-07-19 07:57:57.205902 elefanto_webkassa-0.1.6/webkassa/models.py
--rw-r--r--   0        0        0     1204 2023-07-19 04:21:28.132448 elefanto_webkassa-0.1.6/webkassa/serializers.py
--rw-r--r--   0        0        0        0 2023-07-18 05:20:52.720032 elefanto_webkassa-0.1.6/webkassa/services/__init__.py
--rw-r--r--   0        0        0     6024 2023-07-19 07:41:47.463341 elefanto_webkassa-0.1.6/webkassa/services/manager.py
--rw-r--r--   0        0        0      392 2023-07-19 04:23:29.588415 elefanto_webkassa-0.1.6/webkassa/services/password_encryption.py
--rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 elefanto_webkassa-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      172 2023-07-19 04:25:23.836094 elefanto_webkassa-0.2.0/README.md
+-rw-r--r--   0        0        0      847 2023-07-19 09:37:05.807374 elefanto_webkassa-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      488 2023-07-19 07:43:50.241606 elefanto_webkassa-0.2.0/webkassa/__init__.py
+-rw-r--r--   0        0        0     1384 2023-07-19 08:43:13.901335 elefanto_webkassa-0.2.0/webkassa/admin.py
+-rw-r--r--   0        0        0      236 2023-07-18 06:59:32.374169 elefanto_webkassa-0.2.0/webkassa/apps.py
+-rw-r--r--   0        0        0     3472 2023-07-19 08:01:54.584953 elefanto_webkassa-0.2.0/webkassa/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-07-18 04:42:18.150603 elefanto_webkassa-0.2.0/webkassa/migrations/__init__.py
+-rw-r--r--   0        0        0     2930 2023-07-19 07:57:57.205902 elefanto_webkassa-0.2.0/webkassa/models.py
+-rw-r--r--   0        0        0     1204 2023-07-19 04:21:28.132448 elefanto_webkassa-0.2.0/webkassa/serializers.py
+-rw-r--r--   0        0        0        0 2023-07-18 05:20:52.720032 elefanto_webkassa-0.2.0/webkassa/services/__init__.py
+-rw-r--r--   0        0        0     6849 2023-07-19 09:36:43.771822 elefanto_webkassa-0.2.0/webkassa/services/manager.py
+-rw-r--r--   0        0        0      392 2023-07-19 04:23:29.588415 elefanto_webkassa-0.2.0/webkassa/services/password_encryption.py
+-rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 elefanto_webkassa-0.2.0/PKG-INFO
```

### Comparing `elefanto_webkassa-0.1.6/pyproject.toml` & `elefanto_webkassa-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "elefanto-webkassa"
-version = "0.1.6"
+version = "0.2.0"
 description = ""
 authors = ["Zhanibek <gglassota2@gmail.com>"]
 readme = "README.md"
 packages = [{include = "webkassa"}]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
```

### Comparing `elefanto_webkassa-0.1.6/webkassa/admin.py` & `elefanto_webkassa-0.2.0/webkassa/admin.py`

 * *Files identical despite different names*

### Comparing `elefanto_webkassa-0.1.6/webkassa/migrations/0001_initial.py` & `elefanto_webkassa-0.2.0/webkassa/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `elefanto_webkassa-0.1.6/webkassa/models.py` & `elefanto_webkassa-0.2.0/webkassa/models.py`

 * *Files identical despite different names*

### Comparing `elefanto_webkassa-0.1.6/webkassa/serializers.py` & `elefanto_webkassa-0.2.0/webkassa/serializers.py`

 * *Files identical despite different names*

### Comparing `elefanto_webkassa-0.1.6/webkassa/services/manager.py` & `elefanto_webkassa-0.2.0/webkassa/services/manager.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,57 +13,72 @@
 
 WEBKASSA_CONFIG = settings.WEBKASSA_CONFIG
 URL = WEBKASSA_CONFIG['url']
 HEADERS = {'X-API-KEY': WEBKASSA_CONFIG['api_key'], 'Content-Type': 'application/json'}
 
 
 class WebKassaManager:
-    _token: str = None
-    _email: str = None
+    _token: str = ''
+    _email: str = ''
     cashier: WebKassaAccount = None
     _client: httpx.Client = None
     _url: str = URL
     _headers: dict = HEADERS
+    _cashbox_unique_number: str = ''
 
-    def __init__(self, email: str, url: str = URL, headers: dict = HEADERS): # noqa
+    def __init__(self, email: str, cashbox_unique_number: str, url: str = URL, headers: dict = HEADERS): # noqa
         self._email = email
+        self._cashbox_unique_number = cashbox_unique_number
         self.cashier = self._get_cashier()
         self._token = self.cashier.token
         self._client = httpx.Client()
         self._url = url
         self._headers = headers
 
     def _get_cashier(self) -> WebKassaAccount:
         try:
             return WebKassaAccount.objects.get(
                 email=self._email,
+                cashbox_unique_number=self._cashbox_unique_number
             )
         except WebKassaAccount.DoesNotExist:
-            raise ValidationError(_('WebKassaAccount does not exist ({email})'.format(email=self._email)))
+            WebkassaErrorLog.objects.create(
+                code=-1,
+                text='WebKassaAccount does not exist ({email}, {number})'.format(
+                    email=self._email, number=self._cashbox_unique_number),
+            )
 
     def login(self):
-        url = f'{URL}/api/Authorize'
-        data = {'Login': self.cashier.email,
-                'Password': self.cashier.decrypted_password}
-
-        response = self._client.post(url, json=data, headers=self._headers, timeout=30)
-
-        if response.status_code == 200:
-
-            if 'Data' not in response.json():
-                raise AuthenticationFailed(
-                    detail={'detail': _('Error in login to web kassa: {email}'.format(email=self._email))})
-
-            self._token = response.json()['Data']['Token']
-
-            self.cashier.token = self._token
-            self.cashier.save()
-        else:
-            raise AuthenticationFailed(
-                detail={'detail': _('Error in login to web kassa: {email}'.format(email=self._email))})
+        if self.cashier:
+            url = f'{URL}/api/Authorize'
+            data = {'Login': self.cashier.email,
+                    'Password': self.cashier.decrypted_password}
+
+            response = self._client.post(url, json=data, headers=self._headers, timeout=30)
+
+            if response.status_code == 200:
+
+                if 'Data' not in response.json():
+                    WebkassaErrorLog.objects.create(
+                        code=-2,
+                        text='Error in login to web kassa: {email}'.format(email=self._email),
+                    )
+                    self._token = '-1'
+                    return
+
+                self._token = response.json()['Data']['Token']
+
+                self.cashier.token = self._token
+                self.cashier.save()
+            else:
+                WebkassaErrorLog.objects.create(
+                    code=-2,
+                    text='Error in login to web kassa: {email}'.format(email=self._email),
+                )
+                self._token = '-1'
 
     def close_cash_box(self):
         try:
             url = f'{self._url}/api/ZReport'
 
             data = {
                 'Token': self._token,
@@ -71,15 +86,14 @@
             }
             self._client.post(url, json=data, headers=self._headers, timeout=30)
         except ConnectTimeout:
             WebkassaErrorLog.objects.create(
                 code=-1,
                 text='Connect Timeout on close_cash_box',
             )
-            pass
 
     def _get_web_kassa_token(self):
         if not self._token:
             self.login()
             return self._get_web_kassa_token()
         return self._token
 
@@ -119,16 +133,21 @@
             'ExternalCheckNumber': str(check_obj.id),
         })
         try:
             response = self._client.post(url, json=data, headers=HEADERS, timeout=30).json()
             if 'Data' in response:
                 check = response['Data']
                 check_serializer = CheckSerializer(check_obj, data=check, partial=True)
-                check_serializer.is_valid(raise_exception=True)
-                check_serializer.save()
+                if check_serializer.is_valid():
+                    check_serializer.save()
+                else:
+                    WebkassaErrorLog.objects.create(
+                        code=-4,
+                        text='CheckSerializer validation: {data}'.format(data=check),
+                    )
             elif 'Errors' in response:
                 errors = response['Errors']
                 for error in errors:
                     if error['Code'] in [3, 2, 1]:
                         self.login()
                         data.update({
                             'Token': self._get_web_kassa_token(),
@@ -158,10 +177,12 @@
                 text=str(e),
             )
         return check_obj
 
     def get_check(self, data: dict):
         data = self._set_positions_default(data)
         data['Token'] = self._get_web_kassa_token()
+        if self._token == '-1':
+            return None
         data['CashboxUniqueNumber'] = self.cashier.cashbox_unique_number
         data = self._calculate_tax(data)
         return self._create_check(data)
```

### Comparing `elefanto_webkassa-0.1.6/PKG-INFO` & `elefanto_webkassa-0.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elefanto-webkassa
-Version: 0.1.6
+Version: 0.2.0
 Summary: 
 Author: Zhanibek
 Author-email: gglassota2@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

