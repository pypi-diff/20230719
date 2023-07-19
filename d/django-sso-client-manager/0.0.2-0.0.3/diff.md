# Comparing `tmp/django-sso-client-manager-0.0.2.tar.gz` & `tmp/django-sso-client-manager-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-sso-client-manager-0.0.2.tar", last modified: Fri Jul 14 12:11:54 2023, max compression
+gzip compressed data, was "django-sso-client-manager-0.0.3.tar", last modified: Wed Jul 19 06:10:47 2023, max compression
```

## Comparing `django-sso-client-manager-0.0.2.tar` & `django-sso-client-manager-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 yil       (1000) yil       (1000)        0 2023-07-14 12:11:54.474221 django-sso-client-manager-0.0.2/
--rw-rw-r--   0 yil       (1000) yil       (1000)     1500 2023-07-14 12:11:54.474221 django-sso-client-manager-0.0.2/PKG-INFO
-drwxrwxr-x   0 yil       (1000) yil       (1000)        0 2023-07-14 12:11:54.474221 django-sso-client-manager-0.0.2/django_sso_client_manager.egg-info/
--rw-rw-r--   0 yil       (1000) yil       (1000)     1500 2023-07-14 12:11:54.000000 django-sso-client-manager-0.0.2/django_sso_client_manager.egg-info/PKG-INFO
--rw-rw-r--   0 yil       (1000) yil       (1000)      427 2023-07-14 12:11:54.000000 django-sso-client-manager-0.0.2/django_sso_client_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 yil       (1000) yil       (1000)        1 2023-07-14 12:11:54.000000 django-sso-client-manager-0.0.2/django_sso_client_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 yil       (1000) yil       (1000)       57 2023-07-14 12:11:54.000000 django-sso-client-manager-0.0.2/django_sso_client_manager.egg-info/requires.txt
--rw-rw-r--   0 yil       (1000) yil       (1000)       19 2023-07-14 12:11:54.000000 django-sso-client-manager-0.0.2/django_sso_client_manager.egg-info/top_level.txt
--rw-rw-r--   0 yil       (1000) yil       (1000)       38 2023-07-14 12:11:54.474221 django-sso-client-manager-0.0.2/setup.cfg
--rw-rw-r--   0 yil       (1000) yil       (1000)     1320 2023-07-14 12:08:08.000000 django-sso-client-manager-0.0.2/setup.py
-drwxrwxr-x   0 yil       (1000) yil       (1000)        0 2023-07-14 12:11:54.474221 django-sso-client-manager-0.0.2/sso_client_manager/
--rw-rw-r--   0 yil       (1000) yil       (1000)        0 2023-06-13 14:37:55.000000 django-sso-client-manager-0.0.2/sso_client_manager/__init__.py
--rw-rw-r--   0 yil       (1000) yil       (1000)      171 2023-07-07 05:33:04.000000 django-sso-client-manager-0.0.2/sso_client_manager/apps.py
--rw-rw-r--   0 yil       (1000) yil       (1000)     2370 2023-07-10 03:50:17.000000 django-sso-client-manager-0.0.2/sso_client_manager/middlewares.py
--rw-rw-r--   0 yil       (1000) yil       (1000)      295 2023-07-07 06:07:39.000000 django-sso-client-manager-0.0.2/sso_client_manager/urls.py
--rw-rw-r--   0 yil       (1000) yil       (1000)      229 2023-07-07 05:35:01.000000 django-sso-client-manager-0.0.2/sso_client_manager/utils.py
--rw-rw-r--   0 yil       (1000) yil       (1000)     4849 2023-07-10 03:45:31.000000 django-sso-client-manager-0.0.2/sso_client_manager/views.py
+drwxrwxr-x   0 yil       (1000) yil       (1000)        0 2023-07-19 06:10:47.186351 django-sso-client-manager-0.0.3/
+-rw-rw-r--   0 yil       (1000) yil       (1000)     1500 2023-07-19 06:10:47.186351 django-sso-client-manager-0.0.3/PKG-INFO
+drwxrwxr-x   0 yil       (1000) yil       (1000)        0 2023-07-19 06:10:47.186351 django-sso-client-manager-0.0.3/django_sso_client_manager.egg-info/
+-rw-rw-r--   0 yil       (1000) yil       (1000)     1500 2023-07-19 06:10:47.000000 django-sso-client-manager-0.0.3/django_sso_client_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 yil       (1000) yil       (1000)      427 2023-07-19 06:10:47.000000 django-sso-client-manager-0.0.3/django_sso_client_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 yil       (1000) yil       (1000)        1 2023-07-19 06:10:47.000000 django-sso-client-manager-0.0.3/django_sso_client_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 yil       (1000) yil       (1000)       58 2023-07-19 06:10:47.000000 django-sso-client-manager-0.0.3/django_sso_client_manager.egg-info/requires.txt
+-rw-rw-r--   0 yil       (1000) yil       (1000)       19 2023-07-19 06:10:47.000000 django-sso-client-manager-0.0.3/django_sso_client_manager.egg-info/top_level.txt
+-rw-rw-r--   0 yil       (1000) yil       (1000)       38 2023-07-19 06:10:47.186351 django-sso-client-manager-0.0.3/setup.cfg
+-rw-rw-r--   0 yil       (1000) yil       (1000)     1321 2023-07-19 05:58:22.000000 django-sso-client-manager-0.0.3/setup.py
+drwxrwxr-x   0 yil       (1000) yil       (1000)        0 2023-07-19 06:10:47.186351 django-sso-client-manager-0.0.3/sso_client_manager/
+-rw-rw-r--   0 yil       (1000) yil       (1000)        0 2023-06-13 14:37:55.000000 django-sso-client-manager-0.0.3/sso_client_manager/__init__.py
+-rw-rw-r--   0 yil       (1000) yil       (1000)      171 2023-07-07 05:33:04.000000 django-sso-client-manager-0.0.3/sso_client_manager/apps.py
+-rw-rw-r--   0 yil       (1000) yil       (1000)     2417 2023-07-18 11:30:58.000000 django-sso-client-manager-0.0.3/sso_client_manager/middlewares.py
+-rw-rw-r--   0 yil       (1000) yil       (1000)      295 2023-07-07 06:07:39.000000 django-sso-client-manager-0.0.3/sso_client_manager/urls.py
+-rw-rw-r--   0 yil       (1000) yil       (1000)      229 2023-07-07 05:35:01.000000 django-sso-client-manager-0.0.3/sso_client_manager/utils.py
+-rw-rw-r--   0 yil       (1000) yil       (1000)     6129 2023-07-19 05:54:20.000000 django-sso-client-manager-0.0.3/sso_client_manager/views.py
```

### Comparing `django-sso-client-manager-0.0.2/PKG-INFO` & `django-sso-client-manager-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sso-client-manager
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Django app for the managing sso client that have login, logout and set code a in cookies.
 Home-page: https://github.com/rjnp2/django-sso-client-manager
 Author: rjnp2
 Author-email: rjnp2@outlook.com
 License: MIT License
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `django-sso-client-manager-0.0.2/django_sso_client_manager.egg-info/PKG-INFO` & `django-sso-client-manager-0.0.3/django_sso_client_manager.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-sso-client-manager
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Django app for the managing sso client that have login, logout and set code a in cookies.
 Home-page: https://github.com/rjnp2/django-sso-client-manager
 Author: rjnp2
 Author-email: rjnp2@outlook.com
 License: MIT License
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `django-sso-client-manager-0.0.2/setup.py` & `django-sso-client-manager-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 README = open(os.path.join(os.path.dirname(__file__), 'readme.md')).read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='django-sso-client-manager',
-    version='0.0.2',
+    version='0.0.3',
     packages=['sso_client_manager'],
     include_package_data=True,
     license='MIT License',
     description='A Django app for the managing sso client that have login, logout and set code a in cookies.',
     long_description=README,
     long_description_content_type="text/markdown",
     url='https://github.com/rjnp2/django-sso-client-manager',
@@ -27,14 +27,14 @@
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.10',
         'Topic :: Internet :: WWW/HTTP',
         'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
     ],
     python_requires=">=3.10",
     install_requires=[
-        'cryptography>=1.0.1',
+        'cryptography>=41.0.1',
         'requests>=2.31.0',
     ],
     extras_require={
         "dev": ['twine>=4.0.2',]
     }
 )
```

### Comparing `django-sso-client-manager-0.0.2/sso_client_manager/middlewares.py` & `django-sso-client-manager-0.0.3/sso_client_manager/middlewares.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 class ParseCodeDataMiddleware(MiddlewareMixin):
     
     def __call__(self, request):
         code = request.COOKIES.get('code')
         my_code_mod = None
 
         if (not request.user.is_authenticated and 
-            code and 'set-code/' not in request.path):    
+            code and ('set-code/' not in request.path or 
+            'login/' not in request.path)):    
 
             my_code = request.COOKIES.get('my_code')
             try:
                 my_code = signer.unsign_object(my_code)
                 username = my_code['username']
                 my_code = code == my_code['code'] 
             except:
```

