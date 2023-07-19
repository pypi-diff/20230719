# Comparing `tmp/zoho-client-django-1.2.1.tar.gz` & `tmp/zoho-client-django-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zoho-client-django-1.2.1.tar", last modified: Tue Jul 18 12:02:45 2023, max compression
+gzip compressed data, was "zoho-client-django-1.2.2.tar", last modified: Wed Jul 19 10:39:43 2023, max compression
```

## Comparing `zoho-client-django-1.2.1.tar` & `zoho-client-django-1.2.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 guy        (501) staff       (20)        0 2023-07-18 12:02:45.012724 zoho-client-django-1.2.1/
--rw-r--r--   0 guy        (501) staff       (20)     1067 2023-07-15 09:20:03.000000 zoho-client-django-1.2.1/LICENSE
--rw-r--r--   0 guy        (501) staff       (20)     2570 2023-07-18 12:02:45.012583 zoho-client-django-1.2.1/PKG-INFO
--rw-r--r--   0 guy        (501) staff       (20)     2234 2023-07-15 15:22:00.000000 zoho-client-django-1.2.1/README.md
--rw-r--r--   0 guy        (501) staff       (20)       38 2023-07-18 12:02:45.012766 zoho-client-django-1.2.1/setup.cfg
--rw-r--r--   0 guy        (501) staff       (20)      865 2023-07-18 12:01:26.000000 zoho-client-django-1.2.1/setup.py
-drwxr-xr-x   0 guy        (501) staff       (20)        0 2023-07-18 12:02:45.008905 zoho-client-django-1.2.1/zoho_client/
--rw-r--r--   0 guy        (501) staff       (20)        0 2023-07-14 11:11:08.000000 zoho-client-django-1.2.1/zoho_client/__init__.py
--rw-r--r--   0 guy        (501) staff       (20)     1445 2023-07-15 13:55:44.000000 zoho-client-django-1.2.1/zoho_client/admin.py
--rw-r--r--   0 guy        (501) staff       (20)      153 2023-07-14 11:11:09.000000 zoho-client-django-1.2.1/zoho_client/apps.py
-drwxr-xr-x   0 guy        (501) staff       (20)        0 2023-07-18 12:02:45.009413 zoho-client-django-1.2.1/zoho_client/migrations/
--rw-r--r--   0 guy        (501) staff       (20)      782 2023-07-14 12:22:01.000000 zoho-client-django-1.2.1/zoho_client/migrations/0001_initial.py
--rw-r--r--   0 guy        (501) staff       (20)        0 2023-07-14 11:11:08.000000 zoho-client-django-1.2.1/zoho_client/migrations/__init__.py
--rw-r--r--   0 guy        (501) staff       (20)      191 2023-07-14 11:17:43.000000 zoho-client-django-1.2.1/zoho_client/models.py
-drwxr-xr-x   0 guy        (501) staff       (20)        0 2023-07-18 12:02:45.006365 zoho-client-django-1.2.1/zoho_client/templates/
-drwxr-xr-x   0 guy        (501) staff       (20)        0 2023-07-18 12:02:45.006405 zoho-client-django-1.2.1/zoho_client/templates/admin/
-drwxr-xr-x   0 guy        (501) staff       (20)        0 2023-07-18 12:02:45.006446 zoho-client-django-1.2.1/zoho_client/templates/admin/zoho_client/
-drwxr-xr-x   0 guy        (501) staff       (20)        0 2023-07-18 12:02:45.009826 zoho-client-django-1.2.1/zoho_client/templates/admin/zoho_client/zohotoken/
--rw-r--r--   0 guy        (501) staff       (20)      242 2023-07-15 11:22:51.000000 zoho-client-django-1.2.1/zoho_client/templates/admin/zoho_client/zohotoken/fetch_tokens.html
--rw-r--r--   0 guy        (501) staff       (20)      320 2023-07-15 13:56:34.000000 zoho-client-django-1.2.1/zoho_client/templates/admin/zoho_client/zohotoken/zoho_token_change_list.html
--rw-r--r--   0 guy        (501) staff       (20)       60 2023-07-14 11:11:08.000000 zoho-client-django-1.2.1/zoho_client/tests.py
--rw-r--r--   0 guy        (501) staff       (20)       63 2023-07-14 11:11:08.000000 zoho-client-django-1.2.1/zoho_client/views.py
--rw-r--r--   0 guy        (501) staff       (20)     2998 2023-07-14 22:11:49.000000 zoho-client-django-1.2.1/zoho_client/zoho.py
-drwxr-xr-x   0 guy        (501) staff       (20)        0 2023-07-18 12:02:45.011313 zoho-client-django-1.2.1/zoho_client_django.egg-info/
--rw-r--r--   0 guy        (501) staff       (20)     2570 2023-07-18 12:02:44.000000 zoho-client-django-1.2.1/zoho_client_django.egg-info/PKG-INFO
--rw-r--r--   0 guy        (501) staff       (20)      742 2023-07-18 12:02:44.000000 zoho-client-django-1.2.1/zoho_client_django.egg-info/SOURCES.txt
--rw-r--r--   0 guy        (501) staff       (20)        1 2023-07-18 12:02:44.000000 zoho-client-django-1.2.1/zoho_client_django.egg-info/dependency_links.txt
--rw-r--r--   0 guy        (501) staff       (20)       39 2023-07-18 12:02:44.000000 zoho-client-django-1.2.1/zoho_client_django.egg-info/requires.txt
--rw-r--r--   0 guy        (501) staff       (20)       30 2023-07-18 12:02:44.000000 zoho-client-django-1.2.1/zoho_client_django.egg-info/top_level.txt
-drwxr-xr-x   0 guy        (501) staff       (20)        0 2023-07-18 12:02:45.012301 zoho-client-django-1.2.1/zoho_test_project/
--rw-r--r--   0 guy        (501) staff       (20)        0 2023-07-14 11:10:45.000000 zoho-client-django-1.2.1/zoho_test_project/__init__.py
--rw-r--r--   0 guy        (501) staff       (20)      411 2023-07-14 11:10:46.000000 zoho-client-django-1.2.1/zoho_test_project/asgi.py
--rw-r--r--   0 guy        (501) staff       (20)     3639 2023-07-15 10:11:01.000000 zoho-client-django-1.2.1/zoho_test_project/settings.py
--rw-r--r--   0 guy        (501) staff       (20)      759 2023-07-14 11:10:46.000000 zoho-client-django-1.2.1/zoho_test_project/urls.py
--rw-r--r--   0 guy        (501) staff       (20)      411 2023-07-14 11:10:46.000000 zoho-client-django-1.2.1/zoho_test_project/wsgi.py
+drwxr-xr-x   0 guy        (501) staff       (20)        0 2023-07-19 10:39:43.323550 zoho-client-django-1.2.2/
+-rw-r--r--   0 guy        (501) staff       (20)     1067 2023-07-15 09:20:03.000000 zoho-client-django-1.2.2/LICENSE
+-rw-r--r--   0 guy        (501) staff       (20)     3204 2023-07-19 10:39:43.323321 zoho-client-django-1.2.2/PKG-INFO
+-rw-r--r--   0 guy        (501) staff       (20)     2868 2023-07-19 10:38:10.000000 zoho-client-django-1.2.2/README.md
+-rw-r--r--   0 guy        (501) staff       (20)       38 2023-07-19 10:39:43.323616 zoho-client-django-1.2.2/setup.cfg
+-rw-r--r--   0 guy        (501) staff       (20)      865 2023-07-19 09:24:49.000000 zoho-client-django-1.2.2/setup.py
+drwxr-xr-x   0 guy        (501) staff       (20)        0 2023-07-19 10:39:43.313640 zoho-client-django-1.2.2/zoho_client/
+-rw-r--r--   0 guy        (501) staff       (20)        0 2023-07-14 11:11:08.000000 zoho-client-django-1.2.2/zoho_client/__init__.py
+-rw-r--r--   0 guy        (501) staff       (20)     1445 2023-07-15 13:55:44.000000 zoho-client-django-1.2.2/zoho_client/admin.py
+-rw-r--r--   0 guy        (501) staff       (20)      153 2023-07-14 11:11:09.000000 zoho-client-django-1.2.2/zoho_client/apps.py
+drwxr-xr-x   0 guy        (501) staff       (20)        0 2023-07-19 10:39:43.314292 zoho-client-django-1.2.2/zoho_client/migrations/
+-rw-r--r--   0 guy        (501) staff       (20)      782 2023-07-14 12:22:01.000000 zoho-client-django-1.2.2/zoho_client/migrations/0001_initial.py
+-rw-r--r--   0 guy        (501) staff       (20)        0 2023-07-14 11:11:08.000000 zoho-client-django-1.2.2/zoho_client/migrations/__init__.py
+-rw-r--r--   0 guy        (501) staff       (20)      191 2023-07-14 11:17:43.000000 zoho-client-django-1.2.2/zoho_client/models.py
+drwxr-xr-x   0 guy        (501) staff       (20)        0 2023-07-19 10:39:43.310181 zoho-client-django-1.2.2/zoho_client/templates/
+drwxr-xr-x   0 guy        (501) staff       (20)        0 2023-07-19 10:39:43.310225 zoho-client-django-1.2.2/zoho_client/templates/admin/
+drwxr-xr-x   0 guy        (501) staff       (20)        0 2023-07-19 10:39:43.310269 zoho-client-django-1.2.2/zoho_client/templates/admin/zoho_client/
+drwxr-xr-x   0 guy        (501) staff       (20)        0 2023-07-19 10:39:43.315117 zoho-client-django-1.2.2/zoho_client/templates/admin/zoho_client/zohotoken/
+-rw-r--r--   0 guy        (501) staff       (20)      242 2023-07-15 11:22:51.000000 zoho-client-django-1.2.2/zoho_client/templates/admin/zoho_client/zohotoken/fetch_tokens.html
+-rw-r--r--   0 guy        (501) staff       (20)      320 2023-07-15 13:56:34.000000 zoho-client-django-1.2.2/zoho_client/templates/admin/zoho_client/zohotoken/zoho_token_change_list.html
+-rw-r--r--   0 guy        (501) staff       (20)       60 2023-07-14 11:11:08.000000 zoho-client-django-1.2.2/zoho_client/tests.py
+-rw-r--r--   0 guy        (501) staff       (20)       63 2023-07-14 11:11:08.000000 zoho-client-django-1.2.2/zoho_client/views.py
+-rw-r--r--   0 guy        (501) staff       (20)     3035 2023-07-19 09:33:30.000000 zoho-client-django-1.2.2/zoho_client/zoho.py
+drwxr-xr-x   0 guy        (501) staff       (20)        0 2023-07-19 10:39:43.317956 zoho-client-django-1.2.2/zoho_client_django.egg-info/
+-rw-r--r--   0 guy        (501) staff       (20)     3204 2023-07-19 10:39:43.000000 zoho-client-django-1.2.2/zoho_client_django.egg-info/PKG-INFO
+-rw-r--r--   0 guy        (501) staff       (20)      742 2023-07-19 10:39:43.000000 zoho-client-django-1.2.2/zoho_client_django.egg-info/SOURCES.txt
+-rw-r--r--   0 guy        (501) staff       (20)        1 2023-07-19 10:39:43.000000 zoho-client-django-1.2.2/zoho_client_django.egg-info/dependency_links.txt
+-rw-r--r--   0 guy        (501) staff       (20)       39 2023-07-19 10:39:43.000000 zoho-client-django-1.2.2/zoho_client_django.egg-info/requires.txt
+-rw-r--r--   0 guy        (501) staff       (20)       30 2023-07-19 10:39:43.000000 zoho-client-django-1.2.2/zoho_client_django.egg-info/top_level.txt
+drwxr-xr-x   0 guy        (501) staff       (20)        0 2023-07-19 10:39:43.322609 zoho-client-django-1.2.2/zoho_test_project/
+-rw-r--r--   0 guy        (501) staff       (20)        0 2023-07-14 11:10:45.000000 zoho-client-django-1.2.2/zoho_test_project/__init__.py
+-rw-r--r--   0 guy        (501) staff       (20)      411 2023-07-14 11:10:46.000000 zoho-client-django-1.2.2/zoho_test_project/asgi.py
+-rw-r--r--   0 guy        (501) staff       (20)     3639 2023-07-15 10:11:01.000000 zoho-client-django-1.2.2/zoho_test_project/settings.py
+-rw-r--r--   0 guy        (501) staff       (20)      759 2023-07-14 11:10:46.000000 zoho-client-django-1.2.2/zoho_test_project/urls.py
+-rw-r--r--   0 guy        (501) staff       (20)      411 2023-07-14 11:10:46.000000 zoho-client-django-1.2.2/zoho_test_project/wsgi.py
```

### Comparing `zoho-client-django-1.2.1/LICENSE` & `zoho-client-django-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zoho-client-django-1.2.1/PKG-INFO` & `zoho-client-django-1.2.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zoho-client-django
-Version: 1.2.1
+Version: 1.2.2
 Summary: Django app which is a client for the Zoho CRM API
 Home-page: https://github.com/gosourcellc/zoho-client-django
 Author: Guy Moller
 Author-email: guy.moller@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -17,26 +17,37 @@
 ## Usage
 
 ```python
  from zoho_client.zoho import ZohoClient
  client = ZohoClient()
  # GET all Sales_Orders
  res = client.make_request(api_endpoint="Sales_Orders")
- for sales_order in res['data']:
+ # res is an instance of requests.Response
+ for sales_order in res.json()['data']:
     print(f"sales order #{sales_order['id']}")
 
  # find the first record
- sales_order_id = res['data'][0]['id']
+ sales_order_id = res.json()['data'][0]['id']
 
  # update the sales order's subject
- payload = {'data': [ {'Subject': 'CHNAGED'}]}
- res = client.make_request(method='PUT', api_endpoint=f"Sales_Orders/{sales_order_id}", data=payload)
- print(res['data'][0]['status'])
+ payload = {'data': [ {'Subject': 'CHANGED'}]}
+ # the make_request accpet any kwargs which the requests.request() method accpets
+ res = client.make_request(method='PUT', api_endpoint=f"Sales_Orders/{sales_order_id}", json=payload)
+ print(res.json()['data'][0]['status'])
  # => success
 
+ # search for a record. the params are automatically encoded
+ res = client.make_request("GET", "Accounts/search", params= {"criteria": "(Account_Name:equals:Guy Moller)"})
+ print(f"found {resp.json()['info']['count']} records")
+
+ # create a record
+ account_data={'Account_Name': 'John Doe', 'Email': 'joe@example.com'}
+ res = client.make_request(method='POST', api_endpoint='Accounts',json={'data':[account_data]})
+ print(res.json()['data'][0]['details']['id'])
+ # => 5599334000006242002
 ```
 
 # Setup
 
 ## ENV
 
 the package expects to have it's configuration in the settings.py:
```

### Comparing `zoho-client-django-1.2.1/README.md` & `zoho-client-django-1.2.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -5,26 +5,37 @@
 ## Usage
 
 ```python
  from zoho_client.zoho import ZohoClient
  client = ZohoClient()
  # GET all Sales_Orders
  res = client.make_request(api_endpoint="Sales_Orders")
- for sales_order in res['data']:
+ # res is an instance of requests.Response
+ for sales_order in res.json()['data']:
     print(f"sales order #{sales_order['id']}")
 
  # find the first record
- sales_order_id = res['data'][0]['id']
+ sales_order_id = res.json()['data'][0]['id']
 
  # update the sales order's subject
- payload = {'data': [ {'Subject': 'CHNAGED'}]}
- res = client.make_request(method='PUT', api_endpoint=f"Sales_Orders/{sales_order_id}", data=payload)
- print(res['data'][0]['status'])
+ payload = {'data': [ {'Subject': 'CHANGED'}]}
+ # the make_request accpet any kwargs which the requests.request() method accpets
+ res = client.make_request(method='PUT', api_endpoint=f"Sales_Orders/{sales_order_id}", json=payload)
+ print(res.json()['data'][0]['status'])
  # => success
 
+ # search for a record. the params are automatically encoded
+ res = client.make_request("GET", "Accounts/search", params= {"criteria": "(Account_Name:equals:Guy Moller)"})
+ print(f"found {resp.json()['info']['count']} records")
+
+ # create a record
+ account_data={'Account_Name': 'John Doe', 'Email': 'joe@example.com'}
+ res = client.make_request(method='POST', api_endpoint='Accounts',json={'data':[account_data]})
+ print(res.json()['data'][0]['details']['id'])
+ # => 5599334000006242002
 ```
 
 # Setup
 
 ## ENV
 
 the package expects to have it's configuration in the settings.py:
```

### Comparing `zoho-client-django-1.2.1/setup.py` & `zoho-client-django-1.2.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Read the contents of your README file
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="zoho-client-django",
-    version="1.2.1",  # Update this for new versions
+    version="1.2.2",  # Update this for new versions
     description="Django app which is a client for the Zoho CRM API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Guy Moller",
     author_email="guy.moller@gmail.com",
     url="https://github.com/gosourcellc/zoho-client-django",
     packages=find_packages(),
```

### Comparing `zoho-client-django-1.2.1/zoho_client/admin.py` & `zoho-client-django-1.2.2/zoho_client/admin.py`

 * *Files identical despite different names*

### Comparing `zoho-client-django-1.2.1/zoho_client/migrations/0001_initial.py` & `zoho-client-django-1.2.2/zoho_client/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `zoho-client-django-1.2.1/zoho_client/zoho.py` & `zoho-client-django-1.2.2/zoho_client/zoho.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import requests
+from requests import Response
 from .models import ZohoToken
 from django.conf import settings
 
 
 class ZohoClient:
     def __init__(self):
         self.client_id = settings.ZOHO_CLIENT_ID
@@ -16,27 +17,27 @@
             token = ZohoToken.objects.latest("timestamp")
             self.refresh_token = token.refresh_token
             self.access_token = token.access_token
         except ZohoToken.DoesNotExist:
             self.refresh_token = None
             self.access_token = None
 
-    def make_request(self, method="GET", api_endpoint=None, data=None):
+    def make_request(self, method="GET", api_endpoint=None, **kwargs) -> Response:
         if not self.access_token:
             self.refresh_access_token()
         url = f"{self.base_url}/crm/{self.api_version}/{api_endpoint}"
         print(url)
-        response = requests.request(method, url, headers=self.headers, json=data)
+        response = requests.request(method, url, headers=self.headers, **kwargs)
 
         # If the access token has expired, refresh it and try the request again
         if response.status_code == 401:
             self.refresh_access_token()
-            return self.make_request(method, api_endpoint, data)
+            return self.make_request(method, api_endpoint, **kwargs)
 
-        return response.json()
+        return response
 
     def refresh_access_token(self):
         data = {
             "refresh_token": self.refresh_token,
             "client_id": self.client_id,
             "client_secret": self.client_secret,
             "grant_type": "refresh_token",
```

### Comparing `zoho-client-django-1.2.1/zoho_client_django.egg-info/PKG-INFO` & `zoho-client-django-1.2.2/zoho_client_django.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zoho-client-django
-Version: 1.2.1
+Version: 1.2.2
 Summary: Django app which is a client for the Zoho CRM API
 Home-page: https://github.com/gosourcellc/zoho-client-django
 Author: Guy Moller
 Author-email: guy.moller@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -17,26 +17,37 @@
 ## Usage
 
 ```python
  from zoho_client.zoho import ZohoClient
  client = ZohoClient()
  # GET all Sales_Orders
  res = client.make_request(api_endpoint="Sales_Orders")
- for sales_order in res['data']:
+ # res is an instance of requests.Response
+ for sales_order in res.json()['data']:
     print(f"sales order #{sales_order['id']}")
 
  # find the first record
- sales_order_id = res['data'][0]['id']
+ sales_order_id = res.json()['data'][0]['id']
 
  # update the sales order's subject
- payload = {'data': [ {'Subject': 'CHNAGED'}]}
- res = client.make_request(method='PUT', api_endpoint=f"Sales_Orders/{sales_order_id}", data=payload)
- print(res['data'][0]['status'])
+ payload = {'data': [ {'Subject': 'CHANGED'}]}
+ # the make_request accpet any kwargs which the requests.request() method accpets
+ res = client.make_request(method='PUT', api_endpoint=f"Sales_Orders/{sales_order_id}", json=payload)
+ print(res.json()['data'][0]['status'])
  # => success
 
+ # search for a record. the params are automatically encoded
+ res = client.make_request("GET", "Accounts/search", params= {"criteria": "(Account_Name:equals:Guy Moller)"})
+ print(f"found {resp.json()['info']['count']} records")
+
+ # create a record
+ account_data={'Account_Name': 'John Doe', 'Email': 'joe@example.com'}
+ res = client.make_request(method='POST', api_endpoint='Accounts',json={'data':[account_data]})
+ print(res.json()['data'][0]['details']['id'])
+ # => 5599334000006242002
 ```
 
 # Setup
 
 ## ENV
 
 the package expects to have it's configuration in the settings.py:
```

### Comparing `zoho-client-django-1.2.1/zoho_client_django.egg-info/SOURCES.txt` & `zoho-client-django-1.2.2/zoho_client_django.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zoho-client-django-1.2.1/zoho_test_project/settings.py` & `zoho-client-django-1.2.2/zoho_test_project/settings.py`

 * *Files identical despite different names*

### Comparing `zoho-client-django-1.2.1/zoho_test_project/urls.py` & `zoho-client-django-1.2.2/zoho_test_project/urls.py`

 * *Files identical despite different names*

