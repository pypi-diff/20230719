# Comparing `tmp/nsj_flask_auth-0.5.4.tar.gz` & `tmp/nsj_flask_auth-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsj_flask_auth-0.5.4.tar", max compression
+gzip compressed data, was "nsj_flask_auth-0.5.5.tar", max compression
```

## Comparing `nsj_flask_auth-0.5.4.tar` & `nsj_flask_auth-0.5.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       72 2023-07-19 11:36:22.331086 nsj_flask_auth-0.5.4/nsj_flask_auth/__init__.py
--rw-r--r--   0        0        0    18492 2023-07-19 13:32:27.167675 nsj_flask_auth-0.5.4/nsj_flask_auth/auth.py
--rw-r--r--   0        0        0      430 2023-07-19 11:36:22.331086 nsj_flask_auth-0.5.4/nsj_flask_auth/caching.py
--rw-r--r--   0        0        0      184 2023-07-19 12:06:37.612886 nsj_flask_auth-0.5.4/nsj_flask_auth/exceptions.py
--rw-r--r--   0        0        0      601 2023-07-19 11:36:22.331086 nsj_flask_auth-0.5.4/nsj_flask_auth/settings.py
--rw-r--r--   0        0        0      521 2023-07-19 13:32:37.019601 nsj_flask_auth-0.5.4/pyproject.toml
--rw-r--r--   0        0        0      630 1970-01-01 00:00:00.000000 nsj_flask_auth-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0       72 2023-07-19 11:36:22.331086 nsj_flask_auth-0.5.5/nsj_flask_auth/__init__.py
+-rw-r--r--   0        0        0    18487 2023-07-19 13:49:35.071924 nsj_flask_auth-0.5.5/nsj_flask_auth/auth.py
+-rw-r--r--   0        0        0      430 2023-07-19 11:36:22.331086 nsj_flask_auth-0.5.5/nsj_flask_auth/caching.py
+-rw-r--r--   0        0        0      184 2023-07-19 12:06:37.612886 nsj_flask_auth-0.5.5/nsj_flask_auth/exceptions.py
+-rw-r--r--   0        0        0      601 2023-07-19 11:36:22.331086 nsj_flask_auth-0.5.5/nsj_flask_auth/settings.py
+-rw-r--r--   0        0        0      521 2023-07-19 13:47:59.368646 nsj_flask_auth-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0      630 1970-01-01 00:00:00.000000 nsj_flask_auth-0.5.5/PKG-INFO
```

### Comparing `nsj_flask_auth-0.5.4/nsj_flask_auth/auth.py` & `nsj_flask_auth-0.5.5/nsj_flask_auth/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,15 +168,15 @@
                 raise InternalUnauthorized("A api-key do sistema não é válida")
             elif response.status_code != 200:
                 raise Exception(f"Erro desconhecido na recuperação do profile: {response.status_code}. Mensagem: {response.content.decode()}. URL: {url}")
 
         if user_profile:
             return user_profile
 
-        url = urljoin(self._diretorio_base_uri, f"/auth/v2/api/profile/{email}")
+        url = urljoin(self._diretorio_base_uri, f"/v2/api/profile/{email}")
         headers = {"apikey": self._diretorio_api_key}
 
         response = requests.get(url, headers=headers)
 
         if response.status_code == 401 or response.status_code == 403:
             raise InternalUnauthorized("A api-key do sistema não é válida")
         elif response.status_code != 200:
```

### Comparing `nsj_flask_auth-0.5.4/nsj_flask_auth/settings.py` & `nsj_flask_auth-0.5.5/nsj_flask_auth/settings.py`

 * *Files identical despite different names*

### Comparing `nsj_flask_auth-0.5.4/pyproject.toml` & `nsj_flask_auth-0.5.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nsj-flask-auth"
-version = "0.5.4"
+version = "0.5.5"
 description = "Modulo básico para autenticação de aplicações Flask no contexto da Nasajon"
 authors = ["Lucas Assis <lucasassis@nasajon.com.br>", "Sergio Silva <sergiosilva@nasajon.com.br>"]
 
 [tool.poetry.dependencies]
 python = "^3.6"
 Flask = "*"
 requests = "*"
```

### Comparing `nsj_flask_auth-0.5.4/PKG-INFO` & `nsj_flask_auth-0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsj-flask-auth
-Version: 0.5.4
+Version: 0.5.5
 Summary: Modulo básico para autenticação de aplicações Flask no contexto da Nasajon
 Author: Lucas Assis
 Author-email: lucasassis@nasajon.com.br
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

