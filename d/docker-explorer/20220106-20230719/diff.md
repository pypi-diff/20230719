# Comparing `tmp/docker_explorer-20220106.tar.gz` & `tmp/docker_explorer-20230719.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker_explorer-20220106.tar", last modified: Thu Jan  6 16:41:10 2022, max compression
+gzip compressed data, was "docker_explorer-20230719.tar", last modified: Wed Jul 19 11:15:23 2023, max compression
```

## Comparing `docker_explorer-20220106.tar` & `docker_explorer-20230719.tar`

### file list

```diff
@@ -1,43 +1,23 @@
-drwxr-x---   0 romaing  (338377) primarygroup (89939)        0 2022-01-06 16:41:10.891012 docker_explorer-20220106/
-drwxr-x---   0 romaing  (338377) primarygroup (89939)        0 2022-01-06 16:41:10.883012 docker_explorer-20220106/.github/
-drwxr-x---   0 romaing  (338377) primarygroup (89939)        0 2022-01-06 16:41:10.883012 docker_explorer-20220106/.github/workflows/
--rw-r-----   0 romaing  (338377) primarygroup (89939)      858 2021-11-25 15:48:56.000000 docker_explorer-20220106/.github/workflows/python-app.yml
--rw-r-----   0 romaing  (338377) primarygroup (89939)      379 2021-01-25 14:35:24.000000 docker_explorer-20220106/.gitignore
--rw-r-----   0 romaing  (338377) primarygroup (89939)    19609 2022-01-05 15:47:33.000000 docker_explorer-20220106/.pylintrc
--rw-r-----   0 romaing  (338377) primarygroup (89939)      210 2021-01-25 14:35:24.000000 docker_explorer-20220106/.style.yapf
--rw-r-----   0 romaing  (338377) primarygroup (89939)     2306 2021-01-25 14:35:24.000000 docker_explorer-20220106/CONTRIBUTING.md
--rw-r-----   0 romaing  (338377) primarygroup (89939)    11358 2021-01-25 14:35:24.000000 docker_explorer-20220106/LICENSE
--rw-r-----   0 romaing  (338377) primarygroup (89939)      480 2022-01-06 16:41:10.891012 docker_explorer-20220106/PKG-INFO
--rw-r-----   0 romaing  (338377) primarygroup (89939)     7489 2022-01-06 16:33:54.000000 docker_explorer-20220106/README.md
-drwxr-x---   0 romaing  (338377) primarygroup (89939)        0 2022-01-06 16:41:10.883012 docker_explorer-20220106/config/
-drwxr-x---   0 romaing  (338377) primarygroup (89939)        0 2022-01-06 16:41:10.883012 docker_explorer-20220106/config/jenkins/
--rw-r-----   0 romaing  (338377) primarygroup (89939)     2886 2021-01-25 14:35:24.000000 docker_explorer-20220106/config/jenkins/e2e.sh
-drwxr-x---   0 romaing  (338377) primarygroup (89939)        0 2022-01-06 16:41:10.883012 docker_explorer-20220106/docker_explorer/
--rw-r-----   0 romaing  (338377) primarygroup (89939)      699 2022-01-06 16:33:54.000000 docker_explorer-20220106/docker_explorer/__init__.py
--rw-r-----   0 romaing  (338377) primarygroup (89939)    14040 2022-01-05 15:47:33.000000 docker_explorer-20220106/docker_explorer/container.py
--rw-r-----   0 romaing  (338377) primarygroup (89939)     6381 2022-01-05 15:47:33.000000 docker_explorer-20220106/docker_explorer/downloader.py
--rw-r-----   0 romaing  (338377) primarygroup (89939)     1546 2021-01-25 14:35:24.000000 docker_explorer-20220106/docker_explorer/errors.py
--rw-r-----   0 romaing  (338377) primarygroup (89939)    10000 2022-01-05 15:47:33.000000 docker_explorer-20220106/docker_explorer/explorer.py
--rw-r-----   0 romaing  (338377) primarygroup (89939)     9933 2022-01-05 15:47:33.000000 docker_explorer-20220106/docker_explorer/storage.py
--rw-r-----   0 romaing  (338377) primarygroup (89939)     1812 2022-01-05 15:47:33.000000 docker_explorer-20220106/docker_explorer/utils.py
-drwxr-x---   0 romaing  (338377) primarygroup (89939)        0 2022-01-06 16:41:10.883012 docker_explorer-20220106/docker_explorer.egg-info/
--rw-r-----   0 romaing  (338377) primarygroup (89939)      480 2022-01-06 16:41:10.000000 docker_explorer-20220106/docker_explorer.egg-info/PKG-INFO
--rw-r-----   0 romaing  (338377) primarygroup (89939)      732 2022-01-06 16:41:10.000000 docker_explorer-20220106/docker_explorer.egg-info/SOURCES.txt
--rw-r-----   0 romaing  (338377) primarygroup (89939)        1 2022-01-06 16:41:10.000000 docker_explorer-20220106/docker_explorer.egg-info/dependency_links.txt
--rw-r-----   0 romaing  (338377) primarygroup (89939)        9 2022-01-06 16:41:10.000000 docker_explorer-20220106/docker_explorer.egg-info/requires.txt
--rw-r-----   0 romaing  (338377) primarygroup (89939)       16 2022-01-06 16:41:10.000000 docker_explorer-20220106/docker_explorer.egg-info/top_level.txt
--rw-r-----   0 romaing  (338377) primarygroup (89939)       38 2022-01-06 16:41:10.891012 docker_explorer-20220106/setup.cfg
--rw-r-----   0 romaing  (338377) primarygroup (89939)     1000 2021-01-25 14:35:24.000000 docker_explorer-20220106/setup.py
-drwxr-x---   0 romaing  (338377) primarygroup (89939)        0 2022-01-06 16:41:10.887012 docker_explorer-20220106/test_data/
--rw-r-----   0 romaing  (338377) primarygroup (89939)  1432753 2021-01-25 14:35:24.000000 docker_explorer-20220106/test_data/aufs.v1.tgz
--rw-r-----   0 romaing  (338377) primarygroup (89939)   703251 2021-01-25 14:35:24.000000 docker_explorer-20220106/test_data/aufs.v2.tgz
--rw-r-----   0 romaing  (338377) primarygroup (89939)  1431275 2021-01-25 14:35:24.000000 docker_explorer-20220106/test_data/overlay.v2.tgz
--rw-r-----   0 romaing  (338377) primarygroup (89939)  1430626 2022-01-05 15:47:33.000000 docker_explorer-20220106/test_data/overlay2.v2.tgz
--rw-r-----   0 romaing  (338377) primarygroup (89939)   166740 2021-01-25 14:35:24.000000 docker_explorer-20220106/test_data/vhdx_files.tgz
--rw-r-----   0 romaing  (338377) primarygroup (89939)  2759998 2021-01-25 14:35:24.000000 docker_explorer-20220106/test_data/vols.v2.tgz
--rw-r-----   0 romaing  (338377) primarygroup (89939)    41063 2022-01-05 15:47:33.000000 docker_explorer-20220106/tests.py
-drwxr-x---   0 romaing  (338377) primarygroup (89939)        0 2022-01-06 16:41:10.891012 docker_explorer-20220106/tools/
--rw-r-----   0 romaing  (338377) primarygroup (89939)       24 2021-01-25 14:35:24.000000 docker_explorer-20220106/tools/__init__.py
--rw-r-----   0 romaing  (338377) primarygroup (89939)     9429 2022-01-06 16:33:54.000000 docker_explorer-20220106/tools/de.py
--rw-r-----   0 romaing  (338377) primarygroup (89939)    20523 2022-01-05 15:47:33.000000 docker_explorer-20220106/tools/merge_vhdx.py
--rw-r-----   0 romaing  (338377) primarygroup (89939)     7650 2021-01-25 14:35:24.000000 docker_explorer-20220106/vhdx_tests.py
+drwxr-xr-x   0 romaing  (338377) primarygroup (89939)        0 2023-07-19 11:15:23.976409 docker_explorer-20230719/
+-rw-r--r--   0 romaing  (338377) primarygroup (89939)    11358 2023-04-05 14:34:01.000000 docker_explorer-20230719/LICENSE
+-rw-r--r--   0 romaing  (338377) primarygroup (89939)      461 2023-07-19 11:15:23.976409 docker_explorer-20230719/PKG-INFO
+-rw-r--r--   0 romaing  (338377) primarygroup (89939)     7489 2023-04-05 14:34:01.000000 docker_explorer-20230719/README.md
+drwxr-xr-x   0 romaing  (338377) primarygroup (89939)        0 2023-07-19 11:15:23.976409 docker_explorer-20230719/docker_explorer/
+-rw-r--r--   0 romaing  (338377) primarygroup (89939)      699 2023-07-19 11:00:28.000000 docker_explorer-20230719/docker_explorer/__init__.py
+-rw-r--r--   0 romaing  (338377) primarygroup (89939)    14267 2023-07-19 11:00:28.000000 docker_explorer-20230719/docker_explorer/container.py
+-rw-r--r--   0 romaing  (338377) primarygroup (89939)     6414 2023-07-19 10:30:10.000000 docker_explorer-20230719/docker_explorer/downloader.py
+-rw-r--r--   0 romaing  (338377) primarygroup (89939)     1546 2023-04-05 14:34:01.000000 docker_explorer-20230719/docker_explorer/errors.py
+-rw-r--r--   0 romaing  (338377) primarygroup (89939)    10000 2023-04-05 14:34:01.000000 docker_explorer-20230719/docker_explorer/explorer.py
+-rw-r--r--   0 romaing  (338377) primarygroup (89939)     9935 2023-04-05 14:34:01.000000 docker_explorer-20230719/docker_explorer/storage.py
+-rw-r--r--   0 romaing  (338377) primarygroup (89939)     1619 2023-07-19 11:00:28.000000 docker_explorer-20230719/docker_explorer/utils.py
+drwxr-xr-x   0 romaing  (338377) primarygroup (89939)        0 2023-07-19 11:15:23.976409 docker_explorer-20230719/docker_explorer.egg-info/
+-rw-r--r--   0 romaing  (338377) primarygroup (89939)      461 2023-07-19 11:15:23.000000 docker_explorer-20230719/docker_explorer.egg-info/PKG-INFO
+-rw-r--r--   0 romaing  (338377) primarygroup (89939)      445 2023-07-19 11:15:23.000000 docker_explorer-20230719/docker_explorer.egg-info/SOURCES.txt
+-rw-r--r--   0 romaing  (338377) primarygroup (89939)        1 2023-07-19 11:15:23.000000 docker_explorer-20230719/docker_explorer.egg-info/dependency_links.txt
+-rw-r--r--   0 romaing  (338377) primarygroup (89939)        9 2023-07-19 11:15:23.000000 docker_explorer-20230719/docker_explorer.egg-info/requires.txt
+-rw-r--r--   0 romaing  (338377) primarygroup (89939)       16 2023-07-19 11:15:23.000000 docker_explorer-20230719/docker_explorer.egg-info/top_level.txt
+-rw-r--r--   0 romaing  (338377) primarygroup (89939)       38 2023-07-19 11:15:23.976409 docker_explorer-20230719/setup.cfg
+-rw-r--r--   0 romaing  (338377) primarygroup (89939)     1000 2023-04-05 14:34:01.000000 docker_explorer-20230719/setup.py
+drwxr-xr-x   0 romaing  (338377) primarygroup (89939)        0 2023-07-19 11:15:23.976409 docker_explorer-20230719/tools/
+-rw-r--r--   0 romaing  (338377) primarygroup (89939)     9429 2023-04-05 14:34:01.000000 docker_explorer-20230719/tools/de.py
+-rw-r--r--   0 romaing  (338377) primarygroup (89939)    20523 2023-04-05 14:34:01.000000 docker_explorer-20230719/tools/merge_vhdx.py
```

### Comparing `docker_explorer-20220106/LICENSE` & `docker_explorer-20230719/LICENSE`

 * *Files identical despite different names*

### Comparing `docker_explorer-20220106/README.md` & `docker_explorer-20230719/README.md`

 * *Files identical despite different names*

### Comparing `docker_explorer-20220106/docker_explorer/container.py` & `docker_explorer-20230719/docker_explorer/container.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,20 @@
     if not os.path.isfile(container_info_json_path):
       raise errors.BadContainerException(
           'Unable to find container configuration file: '
           f'{container_info_json_path}'
       )
     with open(
         container_info_json_path, encoding='utf-8') as container_info_json_file:
-      container_info_dict = json.load(container_info_json_file)
+      try:
+        container_info_dict = json.load(container_info_json_file)
+      except (json.decoder.JSONDecodeError, OSError) as error:
+        raise errors.BadContainerException(
+            'Could not parse JSON configuration file '
+            f'{container_info_json_path}: {error}')
 
     if container_info_dict is None:
       raise errors.BadContainerException(
           'Could not load container configuration file: '
           f'{container_info_json_path}')
 
     self.container_id = container_info_dict.get('ID', None)
```

### Comparing `docker_explorer-20220106/docker_explorer/downloader.py` & `docker_explorer-20230719/docker_explorer/downloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
   def _GetToken(self):
     """Requests an access token from Docker registry."""
     if not self.repository:
       self._SetupRepository(self.image_name)
     auth_url = (
         'https://auth.docker.io/token?service=registry.docker.io'
         f'&scope=repository:{self.repository}:pull')
-    response = requests.get(auth_url)
+    response = requests.get(auth_url, timeout=60)
     self._access_token = response.json().get('access_token', None)
 
   def _RegistryAPIGet(self, url):
     """Calls the Docker registry API.
 
     Args:
       url(str): the API method to call (ie: '/manifest/tag').
@@ -86,15 +86,16 @@
     if not self.repository_url:
       self._SetupRepository(self.image_name)
     if not self._access_token:
       self._GetToken()
     headers = {
         'Authorization':'Bearer '+ self._access_token,
         'Accept':'application/vnd.docker.distribution.manifest.v2+json'}
-    response = requests.get(self.repository_url+url, headers=headers)
+    response = requests.get(
+        self.repository_url+url, headers=headers, timeout=60)
     if response.status_code != 200:
       api_error = errors.DownloaderException(
           f'Error querying Docker Hub API: "{self.repository_url+url}"')
       api_error.http_code = response.status_code
       api_error.http_message = response.content
       raise api_error
     return response
```

### Comparing `docker_explorer-20220106/docker_explorer/errors.py` & `docker_explorer-20230719/docker_explorer/errors.py`

 * *Files identical despite different names*

### Comparing `docker_explorer-20220106/docker_explorer/explorer.py` & `docker_explorer-20230719/docker_explorer/explorer.py`

 * *Files identical despite different names*

### Comparing `docker_explorer-20220106/docker_explorer/storage.py` & `docker_explorer-20230719/docker_explorer/storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
       for source, destination in mount_points:
         storage_path = os.path.join(self.root_directory, source)
         extra_commands.append(
             ['/bin/mount', '--bind', '-o', 'ro', storage_path, destination]
         )
     elif self.docker_version == 2:
       for source, destination in mount_points:
-        storage_path = os.path.join(self.root_directory, source)
+        storage_path = os.path.join(self.docker_directory, source)
         volume_mountpoint = os.path.join(mount_dir, destination)
         extra_commands.append(
             ['/bin/mount', '--bind', '-o', 'ro', storage_path,
              volume_mountpoint])
 
     return extra_commands
```

### Comparing `docker_explorer-20220106/docker_explorer/utils.py` & `docker_explorer-20230719/docker_explorer/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -27,18 +27,14 @@
     timestamp (str): the Docker timestamp.
 
   Returns:
     str: Human readable timestamp.
   """
   try:
     time = datetime.datetime.fromisoformat(timestamp)
-  except AttributeError:
-    # datetime.fromisoformat() is only present in python >= 3.6
-    timestamp = timestamp[:26]
-    time = datetime.datetime.strptime(timestamp, '%Y-%m-%dT%H:%M:%S.%f')
   except ValueError:
     # Strip non-ISO compliant precision and time zone designator.
     timestamp = timestamp[:26]
     if timestamp[-1].isalpha():
       timestamp = timestamp[:-1]
     time = datetime.datetime.fromisoformat(timestamp)
   return time.isoformat()
```

### Comparing `docker_explorer-20220106/setup.py` & `docker_explorer-20230719/setup.py`

 * *Files identical despite different names*

### Comparing `docker_explorer-20220106/tools/de.py` & `docker_explorer-20230719/tools/de.py`

 * *Files identical despite different names*

### Comparing `docker_explorer-20220106/tools/merge_vhdx.py` & `docker_explorer-20230719/tools/merge_vhdx.py`

 * *Files identical despite different names*

