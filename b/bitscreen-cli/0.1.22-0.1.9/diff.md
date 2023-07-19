# Comparing `tmp/bitscreen-cli-0.1.22.tar.gz` & `tmp/bitscreen-cli-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitscreen-cli-0.1.22.tar", last modified: Wed Jul 19 09:27:00 2023, max compression
+gzip compressed data, was "bitscreen-cli-0.1.9.tar", last modified: Thu Oct 21 12:44:04 2021, max compression
```

## Comparing `bitscreen-cli-0.1.22.tar` & `bitscreen-cli-0.1.9.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:27:00.441711 bitscreen-cli-0.1.22/
--rw-r--r--   0 runner    (1001) docker     (123)     8349 2023-07-19 09:27:00.441711 bitscreen-cli-0.1.22/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-07-19 09:26:56.000000 bitscreen-cli-0.1.22/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:27:00.441711 bitscreen-cli-0.1.22/bitscreen_cli/
--rwxr-xr-x   0 runner    (1001) docker     (123)      467 2023-07-19 09:26:56.000000 bitscreen-cli-0.1.22/bitscreen_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-19 09:26:56.000000 bitscreen-cli-0.1.22/bitscreen_cli/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:27:00.441711 bitscreen-cli-0.1.22/bitscreen_cli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 09:26:56.000000 bitscreen-cli-0.1.22/bitscreen_cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-07-19 09:26:56.000000 bitscreen-cli-0.1.22/bitscreen_cli/commands/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-19 09:26:56.000000 bitscreen-cli-0.1.22/bitscreen_cli/commands/cid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-07-19 09:26:56.000000 bitscreen-cli-0.1.22/bitscreen_cli/commands/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-07-19 09:26:56.000000 bitscreen-cli-0.1.22/bitscreen_cli/commands/directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     8717 2023-07-19 09:26:56.000000 bitscreen-cli-0.1.22/bitscreen_cli/commands/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-07-19 09:26:56.000000 bitscreen-cli-0.1.22/bitscreen_cli/commands/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-07-19 09:26:56.000000 bitscreen-cli-0.1.22/bitscreen_cli/commands/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 09:27:00.441711 bitscreen-cli-0.1.22/bitscreen_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8349 2023-07-19 09:27:00.000000 bitscreen-cli-0.1.22/bitscreen_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-19 09:27:00.000000 bitscreen-cli-0.1.22/bitscreen_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-19 09:27:00.000000 bitscreen-cli-0.1.22/bitscreen_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-19 09:27:00.000000 bitscreen-cli-0.1.22/bitscreen_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-19 09:27:00.000000 bitscreen-cli-0.1.22/bitscreen_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-19 09:27:00.000000 bitscreen-cli-0.1.22/bitscreen_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-19 09:26:56.000000 bitscreen-cli-0.1.22/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 09:27:00.441711 bitscreen-cli-0.1.22/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-19 09:26:56.000000 bitscreen-cli-0.1.22/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-21 12:44:04.660169 bitscreen-cli-0.1.9/
+-rw-r--r--   0 root         (0) root         (0)     8060 2021-10-21 12:44:04.660169 bitscreen-cli-0.1.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7686 2021-10-19 10:06:47.000000 bitscreen-cli-0.1.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-21 12:44:04.656835 bitscreen-cli-0.1.9/bitscreen_cli/
+-rwxr-xr-x   0 root         (0) root         (0)      421 2021-10-08 11:14:11.000000 bitscreen-cli-0.1.9/bitscreen_cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       49 2021-09-28 09:09:15.000000 bitscreen-cli-0.1.9/bitscreen_cli/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-21 12:44:04.660169 bitscreen-cli-0.1.9/bitscreen_cli/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2021-09-28 09:06:52.000000 bitscreen-cli-0.1.9/bitscreen_cli/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4796 2021-10-13 10:57:40.000000 bitscreen-cli-0.1.9/bitscreen_cli/commands/auth.py
+-rw-r--r--   0 root         (0) root         (0)     1177 2021-10-08 14:14:49.000000 bitscreen-cli-0.1.9/bitscreen_cli/commands/cid.py
+-rw-r--r--   0 root         (0) root         (0)     1375 2021-09-28 09:06:52.000000 bitscreen-cli-0.1.9/bitscreen_cli/commands/dashboard.py
+-rw-r--r--   0 root         (0) root         (0)     4934 2021-09-28 09:06:52.000000 bitscreen-cli-0.1.9/bitscreen_cli/commands/directory.py
+-rw-r--r--   0 root         (0) root         (0)     9165 2021-10-08 11:13:34.000000 bitscreen-cli-0.1.9/bitscreen_cli/commands/filter.py
+-rw-r--r--   0 root         (0) root         (0)     3657 2021-09-28 09:06:52.000000 bitscreen-cli-0.1.9/bitscreen_cli/commands/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-10-21 12:44:04.656835 bitscreen-cli-0.1.9/bitscreen_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8060 2021-10-21 12:44:04.000000 bitscreen-cli-0.1.9/bitscreen_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      545 2021-10-21 12:44:04.000000 bitscreen-cli-0.1.9/bitscreen_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2021-10-21 12:44:04.000000 bitscreen-cli-0.1.9/bitscreen_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       71 2021-10-21 12:44:04.000000 bitscreen-cli-0.1.9/bitscreen_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      102 2021-10-21 12:44:04.000000 bitscreen-cli-0.1.9/bitscreen_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2021-10-21 12:44:04.000000 bitscreen-cli-0.1.9/bitscreen_cli.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      546 2021-10-19 08:25:49.000000 bitscreen-cli-0.1.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2021-10-21 12:44:04.660169 bitscreen-cli-0.1.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1285 2021-10-21 12:43:19.000000 bitscreen-cli-0.1.9/setup.py
```

### Comparing `bitscreen-cli-0.1.22/PKG-INFO` & `bitscreen-cli-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 Metadata-Version: 2.1
 Name: bitscreen-cli
-Version: 0.1.22
+Version: 0.1.9
 Summary: CLI client for BitScreen
 Home-page: UNKNOWN
 Author: Keyko
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 
-# BitScreen CLI Guide
+# BitScreen CLI
 
 ## Installation
-```console
+```console 
 pip install bitscreen-cli
 ```
 
 ## First steps
 Before starting to interact with BitScreen, you should first log in. You can do this two ways:
 
 ### Using a private key
 To obtain your private key from Metamask, you can check out [this](https://metamask.zendesk.com/hc/en-us/articles/360015289632-How-to-Export-an-Account-Private-Key) tutorial.
-```console
+```console 
 $ bitscreen-cli auth login
 What's you Ethereum wallet address?: <your wallet address>
 What's your private key?: <your private key>
 ```
 
 ### Using a mnemonic/seed phrase
 To obtain your seed phrase from Metamask, you can check out [this](https://metamask.zendesk.com/hc/en-us/articles/360015290032-How-to-reveal-your-Secret-Recovery-Phrase) tutorial.
-```console
+```console 
 $ bitscreen-cli auth login --from-seed
 Please provide your seed phrase: <your seed phrase>
 ```
 
 No matter which one of there two methods you pick, you will be asked if you want these credentials to be saved (locally) for future logins. These credentials are never leaving your machine through BitScreen CLI, they are only used to sign messages locally.
 
 ## Documentation
@@ -56,15 +56,14 @@
 
 * `auth`
 * `cid`
 * `dashboard`
 * `directory`
 * `filter`
 * `settings`
-* `setup`
 
 ## `bitscreen-cli auth`
 
 **Usage**:
 
 ```console
 $ bitscreen-cli auth [OPTIONS] COMMAND [ARGS]...
@@ -86,15 +85,15 @@
 
 ```console
 $ bitscreen-cli auth login [OPTIONS]
 ```
 
 **Options**:
 
-* `--fromseed`: Will require a seed phrase.
+* `--fromseed / --no-fromseed`: [default: False]
 * `--help`: Show this message and exit.
 
 ### `bitscreen-cli auth logout`
 
 **Usage**:
 
 ```console
@@ -117,38 +116,14 @@
 
 * `WALLET`: [required]
 
 **Options**:
 
 * `--help`: Show this message and exit.
 
-## `bitscreen-cli setup`
-
-**Usage**:
-
-```console
-$ bitscreen-cli setup [OPTIONS] COMMAND [ARGS]...
-```
-
-**Options**:
-
-* `--help`: Show this message and exit.
-
-**Commands**:
-
-* `install`
-
-### `bitscreen-cli setup install`
-
-**Usage**:
-
-```console
-$ bitscreen-cli setup install
-```
-
 ## `bitscreen-cli cid`
 
 **Usage**:
 
 ```console
 $ bitscreen-cli cid [OPTIONS] COMMAND [ARGS]...
 ```
```

### Comparing `bitscreen-cli-0.1.22/README.md` & `bitscreen-cli-0.1.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-# BitScreen CLI Guide
+# BitScreen CLI
 
 ## Installation
-```console
+```console 
 pip install bitscreen-cli
 ```
 
 ## First steps
 Before starting to interact with BitScreen, you should first log in. You can do this two ways:
 
 ### Using a private key
 To obtain your private key from Metamask, you can check out [this](https://metamask.zendesk.com/hc/en-us/articles/360015289632-How-to-Export-an-Account-Private-Key) tutorial.
-```console
+```console 
 $ bitscreen-cli auth login
 What's you Ethereum wallet address?: <your wallet address>
 What's your private key?: <your private key>
 ```
 
 ### Using a mnemonic/seed phrase
 To obtain your seed phrase from Metamask, you can check out [this](https://metamask.zendesk.com/hc/en-us/articles/360015290032-How-to-reveal-your-Secret-Recovery-Phrase) tutorial.
-```console
+```console 
 $ bitscreen-cli auth login --from-seed
 Please provide your seed phrase: <your seed phrase>
 ```
 
 No matter which one of there two methods you pick, you will be asked if you want these credentials to be saved (locally) for future logins. These credentials are never leaving your machine through BitScreen CLI, they are only used to sign messages locally.
 
 ## Documentation
@@ -42,15 +42,14 @@
 
 * `auth`
 * `cid`
 * `dashboard`
 * `directory`
 * `filter`
 * `settings`
-* `setup`
 
 ## `bitscreen-cli auth`
 
 **Usage**:
 
 ```console
 $ bitscreen-cli auth [OPTIONS] COMMAND [ARGS]...
@@ -72,15 +71,15 @@
 
 ```console
 $ bitscreen-cli auth login [OPTIONS]
 ```
 
 **Options**:
 
-* `--fromseed`: Will require a seed phrase.
+* `--fromseed / --no-fromseed`: [default: False]
 * `--help`: Show this message and exit.
 
 ### `bitscreen-cli auth logout`
 
 **Usage**:
 
 ```console
@@ -103,38 +102,14 @@
 
 * `WALLET`: [required]
 
 **Options**:
 
 * `--help`: Show this message and exit.
 
-## `bitscreen-cli setup`
-
-**Usage**:
-
-```console
-$ bitscreen-cli setup [OPTIONS] COMMAND [ARGS]...
-```
-
-**Options**:
-
-* `--help`: Show this message and exit.
-
-**Commands**:
-
-* `install`
-
-### `bitscreen-cli setup install`
-
-**Usage**:
-
-```console
-$ bitscreen-cli setup install
-```
-
 ## `bitscreen-cli cid`
 
 **Usage**:
 
 ```console
 $ bitscreen-cli cid [OPTIONS] COMMAND [ARGS]...
 ```
```

### Comparing `bitscreen-cli-0.1.22/bitscreen_cli/commands/auth.py` & `bitscreen-cli-0.1.9/bitscreen_cli/commands/auth.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,126 +4,106 @@
 import os
 from web3.auto import w3
 from eth_account.messages import encode_defunct
 from py_crypto_hd_wallet import HdWalletFactory, HdWalletCoins, HdWalletSpecs, HdWalletDataTypes, HdWalletKeyTypes
 
 app = typer.Typer()
 
-host = "http://172.30.1.3:3030"
+host = "https://bxn.mml.keyko.rocks"
 wallet = None
 privateKey = None
 accessToken = None
 provider = None
 
-
 class BearerAuth(requests.auth.AuthBase):
     def __init__(self, token):
         self.token = token
-
     def __call__(self, r):
         r.headers['Authorization'] = "Bearer " + self.token
         return r
 
-
 def getNonce():
-    response = requests.get(host + '/provider/auth_info/' + wallet)
+    response = requests.get(host + '/provider/' + wallet)
 
     if response.status_code == 200:
         try:
-            return response.json()['nonceMessage']
+            return response.json()['nonce']
         except:
             return None
 
     return None
 
-
 def signMessage(msg):
     message = encode_defunct(text=msg)
     signedMessage = w3.eth.account.sign_message(message, private_key=privateKey)
 
     return signedMessage.signature.hex()
 
-
 def authenticate(signature):
-    typer.echo('asd')
-    typer.secho(signature)
-    typer.echo('asd')
     global provider, accessToken
     payload = {'signature': signature}
-    response = requests.post(host + '/provider/auth/wallet/' + wallet, json=payload)
+    response = requests.post(host + '/provider/auth/' + wallet, json=payload)
     provider = response.json()
 
     if 'accessToken' in provider:
         accessToken = provider['accessToken']
 
         return True
     return False
 
-
 def getConfigDirectory():
     userHome = os.path.expanduser('~')
     return userHome + '/.bitscreen'
 
-
 def getConfigFile():
     configDir = getConfigDirectory()
     return configDir + '/.cli_config'
 
-
 def getConfigFromFile(configKey):
     cf = open(getConfigFile())
     config = json.load(cf)
     cf.close()
 
     if configKey not in config:
         return None
 
     return config[configKey]
 
-
 def getAuthDataFromSeed(seed: str):
     hd_wallet_fact = HdWalletFactory(HdWalletCoins.ETHEREUM)
     hd_wallet = hd_wallet_fact.CreateFromMnemonic("_my_wallet_", seed)
     hd_wallet.Generate(addr_num=1)
     hd_wallet_key = hd_wallet.GetData(HdWalletDataTypes.ADDRESSES)[0]
     address = hd_wallet_key.GetKey(HdWalletKeyTypes.ADDRESS)
     private_key = hd_wallet_key.GetKey(HdWalletKeyTypes.RAW_PRIV)
 
     return address.lower(), private_key
 
-
 @app.command()
 def login(fromSeed: bool = False):
     global wallet, privateKey, accessToken
     configDir = getConfigDirectory()
 
     if not os.path.isdir(configDir):
         os.mkdir(configDir)
         typer.secho("Created bitscreen config directory.")
 
     configFile = getConfigFile()
-    typer.secho(os.path.isfile(configFile))
     if not os.path.isfile(configFile):
         with open(configFile, 'w') as fp:
             fp.write('{}')
         typer.secho("Created bitscreen config file.")
 
     typer.echo(f"Checking credentials.")
 
     cf = open(configFile)
     config = json.load(cf)
     cf.close()
 
     if fromSeed:
-        typer.secho("""
-            Warning: when authenticating using a seed phrase, you will
-            automatically be logged on the main wallet address associated with
-            that seed phrase. If you do not wish to log into the main wallet
-            address, please log in with the private key.
-        """);
         seed = typer.prompt("Please provide your seed phrase: ")
         try:
             wallet, privateKey = getAuthDataFromSeed(seed)
         except:
             raise typer.Exit("Invalid seed phrase.")
     else:
         if 'eth_wallet' in config:
@@ -146,18 +126,15 @@
         raise typer.Exit("Invalid private key.")
 
     isAuthenticated = authenticate(signedNonce)
 
     if not isAuthenticated:
         raise typer.Exit("Login failed.")
 
-    if provider['businessName']:
-        typer.secho(f"Authenticated as " + provider['businessName'], fg=typer.colors.GREEN)
-    else:
-        typer.secho(f"Authenticated.", fg=typer.colors.GREEN)
+    typer.secho(f"Authenticated as " + provider['businessName'], fg=typer.colors.GREEN)
 
     saveCredentials = typer.confirm("Do you want to save credentials for future logins?")
 
     toSave = {
         'access_token': accessToken,
         'provider_id': provider['id']
     }
@@ -165,46 +142,31 @@
     if saveCredentials:
         toSave['eth_private_key'] = privateKey
         toSave['eth_wallet'] = wallet
 
     with open(configFile, 'w') as f:
         f.write(json.dumps(toSave))
 
-
 @app.command()
 def logout():
     configDir = getConfigDirectory()
     configFile = getConfigFile()
 
     if not os.path.isdir(configDir) or not os.path.isfile(configFile):
         typer.secho("Not logged in.")
         raise typer.Exit()
 
     with open(configFile, 'w') as f:
         f.write(json.dumps({}))
 
-
 @app.command()
-def register(wallet_address: str):
-    typer.secho("In order to register, you must first agree to the Terms of Service and Privacy Policy.");
-    typer.secho("Terms of Service: https://github.com/Murmuration-Labs/bitscreen/blob/master/terms_of_service.md");
-    typer.secho("Privacy Policy: https://github.com/Murmuration-Labs/bitscreen/blob/master/privacy_policy.md");
-    agreement = typer.confirm("Do you agree to the Terms of Service and Privacy Policy?");
-
-    if not agreement:
-        raise typer.Exit(
-            "You were not registered because you didn't agree to the Terms of Service and Privacy Policy.");
-
-    body = {
-        "accountType": '1'
-    }
-    response = requests.post(f'{host}/provider/wallet/{wallet_address}', json=body)
+def register(wallet: str):
+    response = requests.post(f'{host}/provider/{wallet}')
 
     if response.status_code == 200:
         typer.secho("Done. You can proceed to log in.", bg=typer.colors.GREEN, fg=typer.colors.BLACK)
     else:
         typer.secho("Error: ", bg=typer.colors.RED)
         print(response.json()['message'])
 
-
 if __name__ == "__main__":
     app()
```

### Comparing `bitscreen-cli-0.1.22/bitscreen_cli/commands/cid.py` & `bitscreen-cli-0.1.9/bitscreen_cli/commands/cid.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+import json
 import requests
 import typer
-from auth import host, getConfigFromFile, BearerAuth
+import os
+from .auth import host, getConfigFromFile, BearerAuth
+from typing import Optional
 
 state = {
     'accessToken': None,
     'providerId': None
 }
 
 app = typer.Typer()
```

### Comparing `bitscreen-cli-0.1.22/bitscreen_cli/commands/directory.py` & `bitscreen-cli-0.1.9/bitscreen_cli/commands/directory.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,143 +1,143 @@
+import json
 import requests
 import typer
+import os
 from tabulate import tabulate
-from auth import host, getConfigFromFile, BearerAuth
-from filter import getReadableVisibility
+from .auth import host, getConfigFromFile, BearerAuth
+from .filter import getReadableVisibility
 
 app = typer.Typer()
 
 state = {
     'accessToken': None,
     'providerId': None
 }
 
+def getPublicFilters(params = {}):
+    params['providerId'] = state['providerId'];
 
-def get_public_filters(params={}):
     response = requests.get(host + '/filter/public', params=params, auth=BearerAuth(state['accessToken']))
     filters = response.json()
 
     return filters['data']
 
+def getPublicFilterDetails(filterId, params = {}):
+    params['providerId'] = state['providerId'];
 
-def get_public_filter_details(filter_id):
-    response = requests.get(host + '/filter/public/details/' + filter_id,
-                            auth=BearerAuth(state['accessToken']))
+    response = requests.get(host + '/filter/public/details/' + filterId, params=params, auth=BearerAuth(state['accessToken']))
 
     if response.status_code == 200:
         data = response.json()
         data['filter']['isImported'] = data['isImported']
         data['filter']['provider'] = data['provider']
         return data['filter']
 
-    raise typer.Exit("Filter not found or is not public / shareable.")
+    raise typer.Exit("Filter not found.")
 
-
-def get_status_from_filter(public_filter):
+def getStatusFromFilter(filter):
     status = typer.style("Not imported", fg=typer.colors.WHITE, bg=typer.colors.RED)
-    if public_filter['isImported']:
+    if filter['isImported']:
         status = typer.style("Imported", fg=typer.colors.GREEN, bold=True)
-    elif public_filter['provider']['id'] == state['providerId']:
+    elif filter['provider']['id'] == state['providerId']:
         status = typer.style("Owned", fg=typer.colors.GREEN)
 
     return status
 
-
-def print_public_filter_lists(filter_list: list):
-    headers = ["ID", "Name", "Visibility", "Status", "Subscribers", "CIDs", "Provider", "Description"]
-    rows = []
-    typer.secho(filter_list)
-    for public_filter in filter_list:
-        status = get_status_from_filter(public_filter)
+def printPublicFilterLists(filterList: list):
+    headers = ["ID", "Name", "Visibility", "Status", "Subscribers", "CIDs", "Override", "Provider", "Description"]
+    rows = [];
+    for filter in filterList:
+        status = getStatusFromFilter(filter)
 
         rows.append([
-            public_filter['shareId'],
-            public_filter['name'],
-            getReadableVisibility(public_filter['visibility']),
+            filter['shareId'],
+            filter['name'],
+            getReadableVisibility(filter['visibility']),
             status,
-            public_filter['subs'],
-            public_filter['cids'],
-            public_filter['provider']['businessName'],
-            public_filter['description']
+            filter['subs'],
+            filter['cids'],
+            'Yes' if filter['override'] else 'No',
+            filter['provider']['businessName'],
+            filter['description']
         ])
     print(tabulate(rows, headers, tablefmt="fancy_grid"))
 
+def printPublicFilterDetails(filter):
+    typer.echo(getStatusFromFilter(filter))
+    typer.secho(f"Filter name:  {filter['name']}")
+    typer.secho(f"Description: {filter['description']}")
+    typer.secho(f"ID: {filter['shareId']}")
+    typer.secho(f"Subscribers: {len(filter['provider_Filters'])}")
+    typer.secho(f"Override: {('Yes' if filter['override'] else 'No')}")
+    typer.secho(f"CID count: {len(filter['cids'])}")
+    typer.secho(f"Business name: {filter['provider']['businessName']}")
+    typer.secho(f"Contact person: {filter['provider']['contactPerson']}")
+    typer.secho(f"Website: {filter['provider']['website']}")
+    typer.secho(f"Email: {filter['provider']['businessName']}")
+    typer.secho(f"Address: {filter['provider']['businessName']}")
+    typer.secho(f"City & Country: {filter['provider']['businessName']}")
 
-def print_public_filter_details(public_filter):
-    typer.echo(get_status_from_filter(public_filter))
-    typer.secho(f"Filter name:  {public_filter['name']}")
-    typer.secho(f"Description: {public_filter['description']}")
-    typer.secho(f"ID: {public_filter['shareId']}")
-    typer.secho(f"Subscribers: {len(public_filter['provider_Filters'])}")
-    typer.secho(f"CID count: {len(public_filter['cids'])}")
-    typer.secho(f"Business name: {public_filter['provider']['businessName']}")
-    typer.secho(f"Contact person: {public_filter['provider']['contactPerson']}")
-    typer.secho(f"Website: {public_filter['provider']['website']}")
-    typer.secho(f"Email: {public_filter['provider']['businessName']}")
-    typer.secho(f"Address: {public_filter['provider']['businessName']}")
-    typer.secho(f"City & Country: {public_filter['provider']['businessName']}")
-
-
-@app.command(name="list")
-def list_filters(search: str = ""):
-    params = {}
+@app.command()
+def list(search: str = ""):
+    params = {};
     if len(search) > 0:
         params['q'] = search
-    filters = get_public_filters(params)
+    filters = getPublicFilters(params)
 
     typer.secho(f"Found {len(filters)} filters.")
-    print_public_filter_lists(filters)
-
+    printPublicFilterLists(filters)
 
 @app.command()
-def details(filter_share_id: str):
-    public_filter = get_public_filter_details(filter_share_id)
-
-    print_public_filter_details(public_filter)
+def details(filter: str):
+    filter = getPublicFilterDetails(filter)
 
+    printPublicFilterDetails(filter)
 
 @app.command(name="import")
-def import_filter(filter_share_id: str):
-    public_filter = get_public_filter_details(filter_share_id)
-    if public_filter['isImported']:
+def importFilter(filter: str):
+    filter = getPublicFilterDetails(filter)
+    if filter['isImported']:
         raise typer.Exit("Filter already imported.")
 
-    provider_filter = {
+    if filter['provider']['id'] == state['providerId']:
+        raise typer.Exit("Cannot import your own filter.")
+
+    if filter['visibility'] == 1:
+        raise typer.Exit("Filter is not public or shareable.")
+
+    providerFilter = {
         'active': True,
-        'filterId': public_filter['id']
+        'filterId': filter['id'],
+        'providerId': state['providerId']
     }
-
-    response = requests.post(f"{host}/provider-filter", json=provider_filter, auth=BearerAuth(state['accessToken']))
+    response = requests.post(f"{host}/provider-filter", json=providerFilter, auth=BearerAuth(state['accessToken']))
     if response.status_code == 200:
         typer.secho("Imported.", bg=typer.colors.GREEN, fg=typer.colors.BLACK)
     else:
         typer.secho("Error: ", bg=typer.colors.RED)
         typer.secho(response.json())
 
-
 @app.command(name="discard")
-def discard_filter(filter_share_id: str):
-    public_filter = get_public_filter_details(filter_share_id)
+def discardFilter(filter: str):
+    filter = getPublicFilterDetails(filter)
 
-    if not public_filter['isImported']:
+    if not filter['isImported']:
         raise typer.Exit("This filter is not imported.")
 
-    response = requests.delete(f"{host}/provider-filter/{public_filter['id']}",
-                               auth=BearerAuth(state['accessToken']))
+    response = requests.delete(f"{host}/provider-filter/{state['providerId']}/{filter['id']}", auth=BearerAuth(state['accessToken']))
     if response.status_code == 200:
         typer.secho("Discarded.", bg=typer.colors.GREEN, fg=typer.colors.BLACK)
     else:
         typer.secho("Error: ", bg=typer.colors.RED)
         typer.secho(response.json())
 
-
 @app.callback()
-def get_auth_data():
+def getAuthData():
     state['accessToken'] = getConfigFromFile('access_token')
     state['providerId'] = getConfigFromFile('provider_id')
 
     if state['accessToken'] is None or state['providerId'] is None:
         raise typer.Exit("Not logged in.")
 
-
 if __name__ == "__main__":
     app()
```

### Comparing `bitscreen-cli-0.1.22/bitscreen_cli/commands/filter.py` & `bitscreen-cli-0.1.9/bitscreen_cli/commands/filter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,220 +1,216 @@
+import json
 import requests
 import typer
+import os
 from tabulate import tabulate
-from auth import host, getConfigFromFile, BearerAuth
+from .auth import host, getConfigFromFile, BearerAuth
+from typing import Optional
 
 VISIBILITY_TYPES = {
     1: 'Private',
     2: 'Public',
-    3: 'Shareable',
-    4: 'Exception'
+    3: 'Shareable'
 }
 
 app = typer.Typer()
 
 state = {
     'accessToken': None,
     'providerId': None
 }
 
+def getFilters(params = {}):
+    params['providerId'] = state['providerId'];
 
-def getFilters(params={}):
     response = requests.get(host + '/filter', params=params, auth=BearerAuth(state['accessToken']))
     filters = response.json()
 
     return filters
 
+def getFilterDetails(filterId, params = {}):
+    params['providerId'] = state['providerId'];
 
-def getFilterDetails(filterId):
-    response = requests.get(host + '/filter/' + filterId, auth=BearerAuth(state['accessToken']))
+    response = requests.get(host + '/filter/' + filterId, params=params, auth=BearerAuth(state['accessToken']))
     if response.status_code == 200:
-        filter_json = response.json()
-        return filter_json
-
-    raise typer.Exit(print(response.json()['message']))
+        filters = response.json()
+        return filters
 
+    raise typer.Exit("Filter not found.")
 
 def getReadableVisibility(visibilityId):
     return VISIBILITY_TYPES[visibilityId]
 
-
 def parseVisibilityCallback(value: str):
     if value is None:
         return None
 
     for key in VISIBILITY_TYPES:
         if VISIBILITY_TYPES[key].lower() == value.lower():
             return key
     raise typer.BadParameter("Invalid visibility type. Allowed types are: Private, Public, Shareable")
 
-
 def parseOverrideCallback(value: int):
     if value is None:
         return None
 
     if value >= 0 and value <= 1:
         return value
     raise typer.BadParameter("Invalid override value. Allowed types are: 0, 1")
 
-
 def printFilterLists(filterList):
-    headers = ["ID", "Name", "Visibility", "Status", "Subscribers", "CIDs", "Provider", "Description"]
+    headers = ["ID", "Name", "Visibility", "Status", "Subscribers", "CIDs", "Override", "Provider", "Description"]
     rows = [];
     for filter in filterList:
         rows.append([
             filter['shareId'],
             filter['name'],
             getReadableVisibility(filter['visibility']),
             'Enabled' if filter['enabled'] else 'Disabled',
             len(filter['provider_Filters']),
             filter['cidsCount'],
+            'Yes' if filter['override'] else 'No',
             filter['provider']['businessName'],
             filter['description']
         ])
     print(tabulate(rows, headers, tablefmt="fancy_grid"))
 
-
 def printCidLists(cidList):
     headers = ["CID", "Reference URL", "Created", "Updated"]
     rows = []
 
     for cid in cidList:
         rows.append([
             cid['cid'],
             cid['refUrl'],
             cid['created'],
             cid['updated']
         ])
 
     print(tabulate(rows, headers, tablefmt="fancy_grid"))
 
-
 def printFilterDetails(filter):
     if filter['enabled']:
         typer.secho("Enabled", bg=typer.colors.GREEN, fg=typer.colors.BLACK)
     else:
         typer.secho("Disabled", bg=typer.colors.RED)
     typer.secho(f"Filter name:  {filter['name']}")
     typer.secho(f"Description: {filter['description']}")
     typer.secho(f"ID: {filter['shareId']}")
     typer.secho(f"Visibility: {getReadableVisibility(filter['visibility'])}")
     typer.secho(f"Subscribers: {len(filter['provider_Filters'])}")
+    typer.secho(f"Override: {('Yes' if filter['override'] else 'No')}")
     typer.secho(f"Owner: {filter['provider']['businessName']}")
     typer.secho(f"CID count: {len(filter['cids'])}")
 
     printCidLists(filter['cids'])
 
-
 def setFilterStatus(filter: str, status: bool):
     filterDetails = getFilterDetails(filter)
 
-    typer.secho(filterDetails)
-    exit
-
     allowed = False
     for providerFilter in filterDetails['provider_Filters']:
         if providerFilter['provider']['id'] == state['providerId']:
             allowed = True
             if providerFilter['active'] == status:
                 raise typer.Exit("Status already set.")
 
     if allowed:
         params = {'active': status}
-        response = requests.put(f"{host}/provider-filter/{filterDetails['id']}", json=params,
-                                auth=BearerAuth(state['accessToken']))
+        response = requests.put(f"{host}/provider-filter/{state['providerId']}/{filterDetails['id']}", json=params, auth=BearerAuth(state['accessToken']))
         if response.status_code == 200:
             typer.secho("Done.", bg=typer.colors.GREEN, fg=typer.colors.BLACK)
         else:
             typer.secho("Error: ", bg=typer.colors.RED)
             typer.secho(response.json())
 
-
 @app.command()
 def list(search: str = ""):
     params = {};
     if len(search) > 0:
         params['q'] = search
     filters = getFilters(params)
 
     print("Found " + str(filters['count']) + " filters:")
 
     printFilterLists(filters['filters'])
 
-
 @app.command()
 def details(filter: str):
     filterDetails = getFilterDetails(filter)
     printFilterDetails(filterDetails)
 
-
 @app.command()
 def enable(filter: str):
     setFilterStatus(filter, True)
 
-
 @app.command()
 def disable(filter: str):
     setFilterStatus(filter, False)
 
-
 @app.command()
 def edit(
-        filter_list: str,
-        name: str = None,
-        description: str = None,
-        visibility: str = typer.Option(None, callback=parseVisibilityCallback)
+    filter: str,
+    name: str = None,
+    description: str = None,
+    override: int = typer.Option(None, callback=parseOverrideCallback),
+    visibility: str = typer.Option(None, callback=parseVisibilityCallback)
 ):
-    filter_json = getFilterDetails(filter_list)
-
-    if name is None and description is None and visibility is None:
-        return typer.secho("No changes were submitted.")
-
+    filter = getFilterDetails(filter)
     if name is not None:
-        filter_json['name'] = name
+        filter['name'] = name
 
     if description is not None:
-        filter_json['description'] = description
+        filter['description'] = description
+
+    if override is not None:
+        filter['override'] = (override == 1)
 
     if visibility is not None:
-        filter_json['visibility'] = visibility
+        filter['visibility'] = visibility
 
-    response = requests.put(f"{host}/filter/{filter_json['id']}", json=filter_json, auth=BearerAuth(state['accessToken']))
+    response = requests.put(f"{host}/filter/{filter['id']}", json=filter, auth=BearerAuth(state['accessToken']))
     if response.status_code == 200:
         typer.secho("Done.", bg=typer.colors.GREEN, fg=typer.colors.BLACK)
     else:
         typer.secho("Error: ", bg=typer.colors.RED)
         typer.secho(response.json())
 
-
 @app.command()
 def add(
-        name: str = typer.Option(..., prompt=True),
-        description: str = typer.Option(..., prompt=True),
-        visibility: str = typer.Option(..., prompt="What visibility should the filter have? [Private/Public/Shareable]"),
+    name: str = typer.Option(..., prompt=True),
+    description: str = typer.Option(..., prompt=True),
+    visibility: str = typer.Option(..., prompt="What visibility should the filter have? [Private/Public/Shareable]", callback=parseVisibilityCallback),
+    override: int = typer.Option(..., prompt="Is this an override filter? [0/1]", callback=parseOverrideCallback),
 ):
-    parsed_visibility = parseVisibilityCallback(visibility)
-
-    filter_json = {
+    filter = {
         'cids': [],
         'enabled': True,
         'name': name,
         'description': description,
-        'visibility': parsed_visibility,
+        'visibility': visibility,
+        'override': (override == 1),
+        'providerId': state['providerId'],
     }
 
-    response = requests.post(f"{host}/filter", json=filter_json, auth=BearerAuth(state['accessToken']))
+    response = requests.post(f"{host}/filter", json=filter, auth=BearerAuth(state['accessToken']))
 
-    filter_list = response.json()
+    filter = response.json()
 
+    providerFilter = {
+        'active': True,
+        'filterId': filter['id'],
+        'providerId': state['providerId']
+    }
+    response = requests.post(f"{host}/provider-filter", json=providerFilter, auth=BearerAuth(state['accessToken']))
     if response.status_code == 200:
         typer.secho("Done.", bg=typer.colors.GREEN, fg=typer.colors.BLACK)
-        filter_list['provider_Filters'] = []
-        filter_list['cids'] = []
-        printFilterDetails(filter_list)
+        filter['provider_Filters'] = []
+        filter['cids'] = []
+        printFilterDetails(filter)
     else:
         typer.secho("Error: ", bg=typer.colors.RED)
         typer.secho(response.json())
 
 
 @app.command(name="add-cid")
 def add_cid(filter: str, cid: str, refUrl: str = ""):
@@ -228,38 +224,33 @@
     response = requests.post(f"{host}/cid", json=cid, auth=BearerAuth(state['accessToken']))
     if response.status_code == 200:
         typer.secho("Done.", bg=typer.colors.GREEN, fg=typer.colors.BLACK)
     else:
         typer.secho("Error: ", bg=typer.colors.RED)
         typer.secho(response.json())
 
-
 @app.command(name="remove-cid")
 def remove_cid(filter: str, cid: str):
-    filter_json = getFilterDetails(filter)
+    filter = getFilterDetails(filter)
     id = None
-    for cidObj in filter_json['cids']:
+    for cidObj in filter['cids']:
         if cidObj['cid'] == cid:
             id = cidObj['id']
             break
 
     if id is None:
         raise typer.Exit("CID not found on provided filter.")
 
-    response = requests.post(f"{host}/filter/remove-cids-from-filter", json={
-        "filterId": filter_json['id'],
-        "cids": [id]
-    }, auth=BearerAuth(state['accessToken']))
+    response = requests.delete(f"{host}/cid/{id}", auth=BearerAuth(state['accessToken']))
     if response.status_code == 200:
         typer.secho("Done.", bg=typer.colors.GREEN, fg=typer.colors.BLACK)
     else:
         typer.secho("Error: ", bg=typer.colors.RED)
         typer.secho(response.json())
 
-
 @app.command()
 def delete(filter: str, confirm: bool = False):
     filter = getFilterDetails(filter)
 
     providerFilter = None
     for providerFilter in filter['provider_Filters']:
         if providerFilter['provider']['id'] == state['providerId']:
@@ -271,26 +262,24 @@
 
     if not confirm:
         confirm = typer.confirm(f"Are you sure you want to delete filter {filter['name']}?")
 
     if not confirm:
         raise typer.Exit("Aborting.");
 
-    response = requests.delete(f"{host}/provider-filter/{filter['id']}", auth=BearerAuth(state['accessToken']))
+    response = requests.delete(f"{host}/provider-filter/{state['providerId']}/{filter['id']}", auth=BearerAuth(state['accessToken']))
     if response.status_code == 200:
         typer.secho("Deleted.", bg=typer.colors.GREEN, fg=typer.colors.BLACK)
     else:
         typer.secho("Error: ", bg=typer.colors.RED)
         typer.secho(response.json())
 
-
 @app.callback()
 def getAuthData():
     state['accessToken'] = getConfigFromFile('access_token')
     state['providerId'] = getConfigFromFile('provider_id')
 
     if state['accessToken'] is None or state['providerId'] is None:
         raise typer.Exit("Not logged in.")
 
-
 if __name__ == "__main__":
     app()
```

### Comparing `bitscreen-cli-0.1.22/bitscreen_cli.egg-info/PKG-INFO` & `bitscreen-cli-0.1.9/bitscreen_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 Metadata-Version: 2.1
 Name: bitscreen-cli
-Version: 0.1.22
+Version: 0.1.9
 Summary: CLI client for BitScreen
 Home-page: UNKNOWN
 Author: Keyko
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 
-# BitScreen CLI Guide
+# BitScreen CLI
 
 ## Installation
-```console
+```console 
 pip install bitscreen-cli
 ```
 
 ## First steps
 Before starting to interact with BitScreen, you should first log in. You can do this two ways:
 
 ### Using a private key
 To obtain your private key from Metamask, you can check out [this](https://metamask.zendesk.com/hc/en-us/articles/360015289632-How-to-Export-an-Account-Private-Key) tutorial.
-```console
+```console 
 $ bitscreen-cli auth login
 What's you Ethereum wallet address?: <your wallet address>
 What's your private key?: <your private key>
 ```
 
 ### Using a mnemonic/seed phrase
 To obtain your seed phrase from Metamask, you can check out [this](https://metamask.zendesk.com/hc/en-us/articles/360015290032-How-to-reveal-your-Secret-Recovery-Phrase) tutorial.
-```console
+```console 
 $ bitscreen-cli auth login --from-seed
 Please provide your seed phrase: <your seed phrase>
 ```
 
 No matter which one of there two methods you pick, you will be asked if you want these credentials to be saved (locally) for future logins. These credentials are never leaving your machine through BitScreen CLI, they are only used to sign messages locally.
 
 ## Documentation
@@ -56,15 +56,14 @@
 
 * `auth`
 * `cid`
 * `dashboard`
 * `directory`
 * `filter`
 * `settings`
-* `setup`
 
 ## `bitscreen-cli auth`
 
 **Usage**:
 
 ```console
 $ bitscreen-cli auth [OPTIONS] COMMAND [ARGS]...
@@ -86,15 +85,15 @@
 
 ```console
 $ bitscreen-cli auth login [OPTIONS]
 ```
 
 **Options**:
 
-* `--fromseed`: Will require a seed phrase.
+* `--fromseed / --no-fromseed`: [default: False]
 * `--help`: Show this message and exit.
 
 ### `bitscreen-cli auth logout`
 
 **Usage**:
 
 ```console
@@ -117,38 +116,14 @@
 
 * `WALLET`: [required]
 
 **Options**:
 
 * `--help`: Show this message and exit.
 
-## `bitscreen-cli setup`
-
-**Usage**:
-
-```console
-$ bitscreen-cli setup [OPTIONS] COMMAND [ARGS]...
-```
-
-**Options**:
-
-* `--help`: Show this message and exit.
-
-**Commands**:
-
-* `install`
-
-### `bitscreen-cli setup install`
-
-**Usage**:
-
-```console
-$ bitscreen-cli setup install
-```
-
 ## `bitscreen-cli cid`
 
 **Usage**:
 
 ```console
 $ bitscreen-cli cid [OPTIONS] COMMAND [ARGS]...
 ```
```

### Comparing `bitscreen-cli-0.1.22/bitscreen_cli.egg-info/SOURCES.txt` & `bitscreen-cli-0.1.9/bitscreen_cli.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -11,9 +11,8 @@
 bitscreen_cli.egg-info/top_level.txt
 bitscreen_cli/commands/__init__.py
 bitscreen_cli/commands/auth.py
 bitscreen_cli/commands/cid.py
 bitscreen_cli/commands/dashboard.py
 bitscreen_cli/commands/directory.py
 bitscreen_cli/commands/filter.py
-bitscreen_cli/commands/settings.py
-bitscreen_cli/commands/setup.py
+bitscreen_cli/commands/settings.py
```

### Comparing `bitscreen-cli-0.1.22/pyproject.toml` & `bitscreen-cli-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bitscreen-cli-0.1.22/setup.py` & `bitscreen-cli-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 install_requires = [x.strip() for x in all_reqs if ('git+' not in x) and (
     not x.startswith('#')) and (not x.startswith('-'))]
 dependency_links = [x.strip().replace('git+', '') for x in all_reqs \
                     if 'git+' not in x]
 setup (
  name = 'bitscreen-cli',
  description = 'CLI client for BitScreen',
- version = '0.1.22',
+ version = '0.1.9',
  packages = find_packages(),
  install_requires = install_requires,
  python_requires='>=3.0',
  entry_points='''
         [console_scripts]
         bitscreen-cli=bitscreen_cli:app
     ''',
```

