# Comparing `tmp/schoolware_api-1.1.9.tar.gz` & `tmp/schoolware_api-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schoolware_api-1.1.9.tar", last modified: Fri May  5 13:08:24 2023, max compression
+gzip compressed data, was "schoolware_api-1.2.0.tar", last modified: Wed Jul 19 15:03:50 2023, max compression
```

## Comparing `schoolware_api-1.1.9.tar` & `schoolware_api-1.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:08:24.287369 schoolware_api-1.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-05 13:08:24.287369 schoolware_api-1.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-05 13:08:10.000000 schoolware_api-1.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-05 13:08:10.000000 schoolware_api-1.1.9/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:08:24.287369 schoolware_api-1.1.9/schoolware_api/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-05 13:08:10.000000 schoolware_api-1.1.9/schoolware_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14418 2023-05-05 13:08:10.000000 schoolware_api-1.1.9/schoolware_api/schoolware_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:08:24.287369 schoolware_api-1.1.9/schoolware_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-05 13:08:24.000000 schoolware_api-1.1.9/schoolware_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-05 13:08:24.000000 schoolware_api-1.1.9/schoolware_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 13:08:24.000000 schoolware_api-1.1.9/schoolware_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-05 13:08:24.000000 schoolware_api-1.1.9/schoolware_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-05 13:08:24.000000 schoolware_api-1.1.9/schoolware_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 13:08:24.287369 schoolware_api-1.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-05 13:08:10.000000 schoolware_api-1.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:03:50.691182 schoolware_api-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-19 15:03:50.691182 schoolware_api-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-07-19 15:03:39.000000 schoolware_api-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-19 15:03:39.000000 schoolware_api-1.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:03:50.691182 schoolware_api-1.2.0/schoolware_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-19 15:03:39.000000 schoolware_api-1.2.0/schoolware_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16064 2023-07-19 15:03:39.000000 schoolware_api-1.2.0/schoolware_api/schoolware_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:03:50.691182 schoolware_api-1.2.0/schoolware_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-19 15:03:50.000000 schoolware_api-1.2.0/schoolware_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-19 15:03:50.000000 schoolware_api-1.2.0/schoolware_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 15:03:50.000000 schoolware_api-1.2.0/schoolware_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-19 15:03:50.000000 schoolware_api-1.2.0/schoolware_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-19 15:03:50.000000 schoolware_api-1.2.0/schoolware_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 15:03:50.691182 schoolware_api-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-19 15:03:39.000000 schoolware_api-1.2.0/setup.py
```

### Comparing `schoolware_api-1.1.9/PKG-INFO` & `schoolware_api-1.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schoolware_api
-Version: 1.1.9
+Version: 1.2.0
 Summary: A api for schoolware written in python
 Author: Maarten Buelens
 Author-email: MB <schoolware_api@mb-server.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Maarten-buelens/schoolware_api
 Project-URL: Bug Tracker, https://github.com/Maarten-buelens/schoolware_api/issues
 Classifier: Programming Language :: Python :: 3
@@ -18,34 +18,35 @@
 An api for schoolware written in python
 
 ## Capabilities
 * get agenda points
 * get scores
 * get todo items
 * send telegram message for new scores
-
-### only microsoft login supported for now
+* support for microsoft and schoolware login
 
 ## Config
 | Key | Description |
 | --- | --- |
 | domain | domain name of schoolware
 | user | school microsoft email
 | password | school microsoft password
+| schoolware_login | set true if using schoolware login
 | bg | background procces to keep token valid
 | bot_token | telegram bot token to enable telegram bot
 | chat_id | id to send messages to
-| verbose | show a lot more info
+| verbose | show a some more info
+| debug | show a some more info
 
 ## Install
 * `pip3 install schoolware_api --upgrade `
 * `playwright install &&  playwright install-deps`
 
 ## optional
-* `pip3 install python-telegram-bot`
+* `pip3 install python-telegram-bot` needed for telegram
 
 ## Simple example
 
 ```python
 from schoolware_api import schoolware
 
 config = {"domain":"", "user":"", "password":""} #example domain: kov.schoolware.be user: name.lastname@leerling.kov.be password: password 
@@ -56,13 +57,13 @@
 print(Schoolware.punten()) # Returns all scores this schoolyear
 print(Schoolware.agenda()) # Returns agenda points today
 print(Schoolware.agenda(datum="2023-03-06 00:00:00")) # Returns agenda points for 2023-03-06
 ```
 ## Complete example
 ```python
 from schoolware_api import schoolware
-config = {"domain":"","password":"","user":"","verbose": false, "bg": true, "bot_token": "", "chat_id": ""}
+config = {"domain":"","password":"","user":"","schoolware_login": "false","verbose": false, "bg": true, "bot_token": "", "chat_id": ""}
 
 Schoolware = schoolware(config)
 
 # same as other
 ```
```

### Comparing `schoolware_api-1.1.9/README.md` & `schoolware_api-1.2.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -3,34 +3,35 @@
 An api for schoolware written in python
 
 ## Capabilities
 * get agenda points
 * get scores
 * get todo items
 * send telegram message for new scores
-
-### only microsoft login supported for now
+* support for microsoft and schoolware login
 
 ## Config
 | Key | Description |
 | --- | --- |
 | domain | domain name of schoolware
 | user | school microsoft email
 | password | school microsoft password
+| schoolware_login | set true if using schoolware login
 | bg | background procces to keep token valid
 | bot_token | telegram bot token to enable telegram bot
 | chat_id | id to send messages to
-| verbose | show a lot more info
+| verbose | show a some more info
+| debug | show a some more info
 
 ## Install
 * `pip3 install schoolware_api --upgrade `
 * `playwright install &&  playwright install-deps`
 
 ## optional
-* `pip3 install python-telegram-bot`
+* `pip3 install python-telegram-bot` needed for telegram
 
 ## Simple example
 
 ```python
 from schoolware_api import schoolware
 
 config = {"domain":"", "user":"", "password":""} #example domain: kov.schoolware.be user: name.lastname@leerling.kov.be password: password 
@@ -41,13 +42,13 @@
 print(Schoolware.punten()) # Returns all scores this schoolyear
 print(Schoolware.agenda()) # Returns agenda points today
 print(Schoolware.agenda(datum="2023-03-06 00:00:00")) # Returns agenda points for 2023-03-06
 ```
 ## Complete example
 ```python
 from schoolware_api import schoolware
-config = {"domain":"","password":"","user":"","verbose": false, "bg": true, "bot_token": "", "chat_id": ""}
+config = {"domain":"","password":"","user":"","schoolware_login": "false","verbose": false, "bg": true, "bot_token": "", "chat_id": ""}
 
 Schoolware = schoolware(config)
 
 # same as other
 ```
```

### Comparing `schoolware_api-1.1.9/pyproject.toml` & `schoolware_api-1.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "schoolware_api"
-version = "1.1.9"
+version = "1.2.0"
 authors = [
   { name="MB", email="schoolware_api@mb-server.com" },
 ]
 description = "A api for schoolware written in python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
   'requests>=2.25.1',
-  'playwright>=1.31.1',
-  'termcolor>=2.2.0'
+  'playwright>=1.31.1'
 ]
 [project.urls]
 "Homepage" = "https://github.com/Maarten-buelens/schoolware_api"
 "Bug Tracker" = "https://github.com/Maarten-buelens/schoolware_api/issues"
```

### Comparing `schoolware_api-1.1.9/schoolware_api/schoolware_api.py` & `schoolware_api-1.2.0/schoolware_api/schoolware_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import requests
 from datetime import date, datetime, timedelta
 from playwright.sync_api import sync_playwright
-import time
-from termcolor import colored
 import threading
 import logging
 
 class schoolware:
 
     def __init__(self, config) -> None:
         """Pass config dict to init class
@@ -15,65 +13,72 @@
         | --- | --- |
         | domain | domain name of schoolware
         | user | school microsoft email
         | password | school microsoft password
         | bg | background procces to keep token valid
         | bot_token | telegram bot token to enable telegram bot
         | chat_id | id to send messages to
-        | verbose | show a lot more info
+        | verbose | show a some more info
+        | debug | show a lot more info
         """
 
         
         self.config = config
         if("debug" in config):
-            self.verbose = config["debug"]
+            self.debug = config["debug"]
+            if(self.debug):
+                logging.basicConfig(format='[%(levelname)s] %(asctime)s - %(message)s', level=logging.DEBUG)
         else:
-            self.verbose = False
+            self.debug = False
+
         if("verbose" in config):
             self.verbose = config["verbose"]
             if(self.verbose):
-                logging.basicConfig(format='[%(levelname)s] %(asctime)s - %(message)s', level=logging.DEBUG)
-            else:
                 logging.basicConfig(format='[%(levelname)s] %(asctime)s - %(message)s', level=logging.INFO)
+            else:
+                logging.basicConfig(format='[%(levelname)s] %(asctime)s - %(message)s', level=logging.WARNING)
         else:
             self.verbose = False
-            logging.basicConfig(format='[%(levelname)s] %(asctime)s - %(message)s', level=logging.INFO)
+            logging.basicConfig(format='[%(levelname)s] %(asctime)s - %(message)s', level=logging.WARNING)
+
         if("bg" in config):
             self.bg = config["bg"]
         else:
             self.bg = False
         
         if(self.bg):
-            self.bg_p = threading.Thread(target=self.bg, args=(self,))
-            print("start bg")
+            self.bg_p = threading.Thread(target=self.bg_funtion, args=(0,))
             self.bg_p.start()
 
-        if("bot_token" in config):
-            self.telegram_bg = threading.Thread(target=self.telegram_def, args=(self,))
-            self.telegram_bg.start()
-            
+        if("schoolware_login" in config):
+            self.schoolware_login = config["schoolware_login"]
+        else:
+            self.schoolware_login = False
+
         self.domain = self.config["domain"]
         self.user = self.config["user"]
         self.password = self.config["password"]
+        
         self.token = ""
         self.cookie = ""
         self.rooster = []
         self.todo_list = []
         self.scores = []
-        self.verbose_print(self , message="starting schoolware_api",level=1)        
-        if(self.verbose):
-            print("getting startup token")
-        self.check_if_valid()
-        self.num_points = len(self.punten())
-        self.scores_prev = self.scores
+        self.verbose_print(message="starting schoolware_api",level=1)        
+
+        if("bot_token" in config):
+            self.num_points = len(self.punten())
+            self.scores_prev = self.scores
+            self.telegram_bg = threading.Thread(target=self.telegram_def, args=(0,))
+            self.telegram_bg.start()
         
 #Token&cookie stuff
     def get_new_token(self):
         ##########VERBOSE##########
-        self.verbose_print(self,"get_token")
+        self.verbose_print("get_token")
         ##########VERBOSE##########
 
         with sync_playwright() as p:
             browser = p.chromium.launch()
             context = browser.new_context(user_agent="Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:108.0) Gecko/20100101 Firefox/108.0")
             page = context.new_page()
             page.goto(f"https://{self.domain}/webleerling/start.html#!fn=llagenda")
@@ -84,50 +89,71 @@
             page.get_by_text("Sign In").click()
             page.wait_for_load_state()
             if(context.cookies()[0]["name"] == "FPWebSession"):
                 self.token = context.cookies()[0]["value"]
                 self.cookie = dict(FPWebSession=self.token)
             browser.close()
             ##########VERBOSE##########
-            self.verbose_end(self,"get_token")
+            self.verbose_end("get_token")
             ##########VERBOSE##########
             return self.token
     
+    def get_new_token_schoolware(self):
+        ##########VERBOSE##########
+        self.verbose_print("get_token_schoolware")
+        ##########VERBOSE##########
+        url = f"https://{self.domain}/webleerling/bin/server.fcgi/RPC/ROUTER/"
+        payload = "{action: \"WisaUserAPI\", method: \"Authenticate\", data: [\""+self.user+"\",\""+self.password+"\"], type: \"rpc\", tid: 1}"
+        r = requests.request("POST", url, data=payload)
+        self.cookie = requests.utils.dict_from_cookiejar(r.cookies)
+        self.token = self.cookie["FPWebSession"]
+        ##########VERBOSE##########
+        self.verbose_end("get_token_schoolware")
+        ##########VERBOSE##########
+        return self.token
+
+
+
     def check_if_valid(self):
         ##########VERBOSE##########
-        self.verbose_print(self,"check_token")
+        self.verbose_print("check_token")
         ##########VERBOSE##########
 
         r = requests.get(f"https://{self.domain}/webleerling/bin/server.fcgi/REST/myschoolwareaccount", cookies=self.cookie)
 
 
         if (r.status_code != 200):
             if(r.status_code == 401):
                 ##########VERBOSE##########
-                self.verbose_end(self,"check_token invalid")
+                self.verbose_end("check_token invalid")
                 ##########VERBOSE##########
-                self.get_new_token()
+                if(not self.schoolware_login):
+                    self.verbose_end("Using Microsoft login")
+                    self.get_new_token()
+                else:
+                    self.verbose_end("Using Schoolware login")
+                    self.get_new_token_schoolware()
             else:
-                self.verbose_end(self,f"check_token error {r.status_code}")
+                self.verbose_end(f"check_token error {r.status_code}")
                 raise "error with token"
         else:
             ##########VERBOSE##########
-            self.verbose_end(self,"check_token")
+            self.verbose_end("check_token")
             ##########VERBOSE##########
             return True
 
 #todo
     def todo(self):
         """gets all todo items from schoolware
 
         Returns:
             list: returns all todo items in a list ordered by descending date
         """
         ##########VERBOSE##########
-        self.verbose_print(self,"todo")
+        self.verbose_print("todo")
         ##########VERBOSE##########
 
         self.check_if_valid()
         task_data = requests.get(f"https://{self.domain}/webleerling/bin/server.fcgi/REST/AgendaPunt/?_dc=1665240724814&MinVan={date.today()}T00:00:00&IsTaakOfToets=true", cookies=self.cookie).json()["data"]
         self.todo_list = []
 
         for taak in task_data:
@@ -150,120 +176,132 @@
                 "vak": vak,
                 "titel": titel,
                 "onderwerp": onderwerp,
                 "eind_time": eind_time,
                 "day": day
             })
         ##########VERBOSE##########
-        self.verbose_end(self,"todo")
+        self.verbose_end("todo")
         ##########VERBOSE##########
         return self.todo_list
 
 #punten
     def punten(self):
         """Gets points from the whole year
 
         Returns:
             list: A list containing the points orderd by descending date
         """
         ##########VERBOSE##########
-        self.verbose_print(self,"punten")
+        self.verbose_print("punten")
         ##########VERBOSE##########
         self.check_if_valid()
-        punten_data = requests.get(f"https://{self.domain}/webleerling/bin/server.fcgi/REST/PuntenbladGridLeerling?&Leerling=15201&?BeoordelingMomentVan=1990-09-01+00:00:00", cookies=self.cookie).json()["data"]
+        punten_data = requests.get(f"https://{self.domain}/webleerling/bin/server.fcgi/REST/PuntenbladGridLeerling?BeoordelingMomentVan=1990-09-01+00:00:00", cookies=self.cookie)
+        punten_data = punten_data.json()["data"]
         self.scores = []
         for vak in punten_data:
 
             for punt in vak["Beoordelingen"]:
-                vak = punt["IngerichtVakNaamgebruiker"]
-                DW = punt["DagelijksWerkCode"]
-                totale_score = float(punt["BeoordelingMomentNoemer"])
-                gewenste_score = float(punt["BeoordelingMomentGewenstAsString"])
                 try:
-                    behaalde_score = float(punt["BeoordelingWaarde"]["NumeriekAsString"])
+                    vak = punt["IngerichtVakNaamgebruiker"]
+                    try:
+                        DW = punt["DagelijksWerkCode"]
+                        EX = None
+                    except:
+                        DW = None
+                        EX = punt["ExamenCode"]
+                    totale_score = float(punt["BeoordelingMomentNoemer"])
+                    gewenste_score = float(punt["BeoordelingMomentGewenstAsString"])
+                    try:
+                        behaalde_score = float(punt["BeoordelingWaarde"]["NumeriekAsString"])
+                    except:
+                        behaalde_score = "n/a"
+                    publicatie_datum = punt["BeoordelingMomentPublicatieDatum"]
+                    datum = punt["BeoordelingMomentDatum"]
+                    titel = punt["BeoordelingMomentOmschrijving"]
+                    dt = datetime.strptime(punt["BeoordelingMomentDatum"].split(' ')[0], '%Y-%m-%d')
+                    day = dt.strftime('%A')
+
+                    pub_dt = datetime.strptime(punt["BeoordelingMomentPublicatieDatum"].split(' ')[0], '%Y-%m-%d')
+                    pub_day = pub_dt.strftime('%A')
+                    if(punt["BeoordelingMomentType_"] == "bmtToets"):
+                        soort = "toets"
+                    else:
+                        soort = "taak"
+
+                    try:
+                        cat = punt["BeoordelingMomentCategorieOmschrijving"]
+                    except:
+                        cat = None
+
+                    self.scores.append({
+                        "soort": soort,
+                        "vak": vak,
+                        "titel": titel,
+                        "DW": DW,
+                        "EX": EX,
+                        "tot_sc": totale_score,
+                        "gew_sc": gewenste_score,
+                        "score": behaalde_score,
+                        "datum": datum,
+                        "pub_datum": publicatie_datum,
+                        "day": day,
+                        "pub_day": pub_day,
+                        "cat": cat
+                    })
                 except:
-                    behaalde_score = "n/a"
-                publicatie_datum = punt["BeoordelingMomentPublicatieDatum"]
-                datum = punt["BeoordelingMomentDatum"]
-                titel = punt["BeoordelingMomentOmschrijving"]
-                dt = datetime.strptime(punt["BeoordelingMomentDatum"].split(' ')[0], '%Y-%m-%d')
-                day = dt.strftime('%A')
-
-                pub_dt = datetime.strptime(punt["BeoordelingMomentPublicatieDatum"].split(' ')[0], '%Y-%m-%d')
-                pub_day = pub_dt.strftime('%A')
-                if(punt["BeoordelingMomentType_"] == "bmtToets"):
-                    soort = "toets"
-                else:
-                    soort = "taak"
-
-                self.scores.append({
-                    "soort": soort,
-                    "vak": vak,
-                    "titel": titel,
-                    "DW": DW,
-                    "tot_sc": totale_score,
-                    "gew_sc": gewenste_score,
-                    "score": behaalde_score,
-                    "datum": datum,
-                    "pub_datum": publicatie_datum,
-                    "day": day,
-                    "pub_day": pub_day,
-                })
+                    pass
         self.scores.sort(key=lambda x: datetime.strptime(x['datum'], '%Y-%m-%d %H:%M:%S'), reverse=True)
         ##########VERBOSE##########
-        self.verbose_end(self,"punten")
+        self.verbose_end("punten")
         ##########VERBOSE##########
         return self.scores
 
 #agenda
     def agenda(self, datum=""):
         """Gets all agenda points of a given date from schoolware
 
         Args:
             datum (str, optional): Date to get agenda for. Defaults to "".
 
         Returns:
             list: returns output from filter_agenda
         """
         ##########VERBOSE##########
-        self.verbose_print(self,"agenda")
+        self.verbose_print("agenda")
         ##########VERBOSE##########
         self.check_if_valid()
         #begin en einde week
         day = str(date.today())
         dt = datetime.strptime(day, '%Y-%m-%d')
         start = (dt - timedelta(days=dt.weekday())).strftime('%Y-%m-%d')
-        if(self.verbose):
-            print(colored("#"*50, "grey"))
-            print(f"start date: {start}")
-            print(colored("#"*50, "grey"))
         end = ((dt - timedelta(days=dt.weekday())) + timedelta(days=6)).strftime('%Y-%m-%d')
         ####
-        agenda_data = requests.get(f"https://kov.schoolware.be/webleerling/bin/server.fcgi/REST/AgendaPunt/?_MaxVan={end}&MinTot={start}", cookies=self.cookie).json()["data"]
+        agenda_data = requests.get(f"https://{self.domain}/webleerling/bin/server.fcgi/REST/AgendaPunt/?_MaxVan={end}&MinTot={start}", cookies=self.cookie).json()["data"]
         self.rooster = []
         for agenda in agenda_data:
             if(agenda["TypePunt"]==1 or agenda["TypePunt"]==2):
                 self.rooster.append(agenda)
         ##########VERBOSE##########
-        self.verbose_end(self,"agenda")
+        self.verbose_end("agenda")
         ##########VERBOSE##########
         return self.filter_rooster(self.rooster, datum)
 
     def filter_rooster(self, rooster, datum=""):
         """Internal function to filter a agenda rooster of a given date
 
         Args:
             rooster (list): The agenda points to filter
             datum (str, optional): The date to filter agenda points for. Defaults to "".
 
         Returns:
             list: Filters agenda points for a given date and points
         """
         ##########VERBOSE##########
-        self.verbose_print(self,"filter_agenda")
+        self.verbose_print("filter_agenda")
         ##########VERBOSE##########
         today = []
         if(datum == ""):
             datum = datetime.today()
         datum = str(datum).split(' ')[0]
         for agenda in rooster:
             if(str(agenda['Van'].split(' ')[0]) == datum):
@@ -294,78 +332,80 @@
                         agenda["skip"] = True
                     elif(today[index+1]["vak"] == today[index+1]["titel"]):
                         today[index+1]["skip"] = True
                         today_filterd.append(agenda)
                 else:
                     today_filterd.append(agenda)
         ##########VERBOSE##########
-        self.verbose_end(self,"filter-agenda")
+        self.verbose_end("filter-agenda")
         ##########VERBOSE##########
 
         return today_filterd
     
     def telegram_manual_send(self, msg):
         """Manualy send a telegram message
 
         Args:
             msg (String): Message to send
         """
         import asyncio
-        asyncio.run(self.telegram_send_msg(self, msg))
+        asyncio.run(self.telegram_send_msg(msg))
 
     ##########OTHER##########
 
     #bg procces
-    def bg(self):
+    def bg_funtion(self, none):
         """Function to keep token valid
         """
         from time import sleep
-        if(self.verbose):
-            print(colored("background procces started","blue"))
+        self.verbose_print(message="background procces started")  
+
         while True:
             sleep(5*60)
-            if(self.verbose):
-                print(colored("background task: checking token","blue"))
+            self.verbose_print(message="background task: checking token")  
             self.check_if_valid()
     #telegram bot
-    def telegram_def(self):
+    def telegram_def(self, none):
         """The setup function for Telegram
         """
-        import telegram
-        from time import sleep
-        
         
-        self.bot = telegram.Bot(self.config["bot_token"])
-        
-        self.num_prev = len(self.scores)
+        from time import sleep
+        self.num_prev = len(self.punten())
         self.scores_prev = self.scores
         while True:
             sleep(5*60)
-            if(self.verbose):
-                self.verbose_print(message=f"telegram checking")
-            self.telegram_point_diff(self)
+            try:
+                if(self.verbose):
+                    self.verbose_print(message=f"telegram checking")
+                self.telegram_point_diff()
+            except:
+                logging.warning(f"error in telegram loop")
 
 
 
     def telegram_point_diff(self):
 
             import asyncio
+            import telegram
             scores_now = self.punten()
             num_now = len(scores_now)
             if(self.num_prev < num_now):
-                diff_list = [i for i in scores_now if i not in self.scores_prev]
-                diff = len(diff_list)
-                self.num_prev = num_now
-                self.scores_prev = scores_now
                 
-                msg = f"{diff} New points for:\n"
-                for item in diff_list:
-                    msg = msg + f"{item['vak']}\n"
-                self.verbose_print(message=f"telegram send msg msg={msg}", level=1)
-                asyncio.run(self.telegram_send_msg(self, msg))
+                    diff_list = [i for i in scores_now if i not in self.scores_prev]
+                    diff = len(diff_list)
+                    self.num_prev = num_now
+                    self.scores_prev = scores_now
+                    
+                    msg = f"{diff} New points for:\n"
+                    for item in diff_list:
+                        msg = msg + f"{item['vak']}\n"
+                    self.verbose_print(message=f"telegram send msg msg={msg}", level=1)
+                    self.bot = telegram.Bot(self.config["bot_token"])
+                    asyncio.run(self.telegram_send_msg(msg))
+
 
     async def telegram_send_msg(self, msg):
         """Function to send a telegram message to a set message-id
 
         Args:
             msg (string): the message to send in telegram msg
         """
```

### Comparing `schoolware_api-1.1.9/schoolware_api.egg-info/PKG-INFO` & `schoolware_api-1.2.0/schoolware_api.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schoolware-api
-Version: 1.1.9
+Version: 1.2.0
 Summary: A api for schoolware written in python
 Author: Maarten Buelens
 Author-email: MB <schoolware_api@mb-server.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Maarten-buelens/schoolware_api
 Project-URL: Bug Tracker, https://github.com/Maarten-buelens/schoolware_api/issues
 Classifier: Programming Language :: Python :: 3
@@ -18,34 +18,35 @@
 An api for schoolware written in python
 
 ## Capabilities
 * get agenda points
 * get scores
 * get todo items
 * send telegram message for new scores
-
-### only microsoft login supported for now
+* support for microsoft and schoolware login
 
 ## Config
 | Key | Description |
 | --- | --- |
 | domain | domain name of schoolware
 | user | school microsoft email
 | password | school microsoft password
+| schoolware_login | set true if using schoolware login
 | bg | background procces to keep token valid
 | bot_token | telegram bot token to enable telegram bot
 | chat_id | id to send messages to
-| verbose | show a lot more info
+| verbose | show a some more info
+| debug | show a some more info
 
 ## Install
 * `pip3 install schoolware_api --upgrade `
 * `playwright install &&  playwright install-deps`
 
 ## optional
-* `pip3 install python-telegram-bot`
+* `pip3 install python-telegram-bot` needed for telegram
 
 ## Simple example
 
 ```python
 from schoolware_api import schoolware
 
 config = {"domain":"", "user":"", "password":""} #example domain: kov.schoolware.be user: name.lastname@leerling.kov.be password: password 
@@ -56,13 +57,13 @@
 print(Schoolware.punten()) # Returns all scores this schoolyear
 print(Schoolware.agenda()) # Returns agenda points today
 print(Schoolware.agenda(datum="2023-03-06 00:00:00")) # Returns agenda points for 2023-03-06
 ```
 ## Complete example
 ```python
 from schoolware_api import schoolware
-config = {"domain":"","password":"","user":"","verbose": false, "bg": true, "bot_token": "", "chat_id": ""}
+config = {"domain":"","password":"","user":"","schoolware_login": "false","verbose": false, "bg": true, "bot_token": "", "chat_id": ""}
 
 Schoolware = schoolware(config)
 
 # same as other
 ```
```

