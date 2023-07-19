# Comparing `tmp/disposable-email-domains-0.0.90.tar.gz` & `tmp/disposable-email-domains-0.0.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "disposable-email-domains-0.0.90.tar", last modified: Fri May 26 02:48:17 2023, max compression
+gzip compressed data, was "disposable-email-domains-0.0.91.tar", last modified: Tue Jul 18 15:48:39 2023, max compression
```

## Comparing `disposable-email-domains-0.0.90.tar` & `disposable-email-domains-0.0.91.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:48:17.945647 disposable-email-domains-0.0.90/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-26 02:48:05.000000 disposable-email-domains-0.0.90/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-26 02:48:05.000000 disposable-email-domains-0.0.90/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-26 02:48:05.000000 disposable-email-domains-0.0.90/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-26 02:48:17.945647 disposable-email-domains-0.0.90/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-26 02:48:05.000000 disposable-email-domains-0.0.90/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:48:17.945647 disposable-email-domains-0.0.90/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1171 2023-05-26 02:48:05.000000 disposable-email-domains-0.0.90/bin/check_for_differences
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-26 02:48:05.000000 disposable-email-domains-0.0.90/bin/parse_source_data
--rwxr-xr-x   0 runner    (1001) docker     (123)       83 2023-05-26 02:48:05.000000 disposable-email-domains-0.0.90/bin/prerelease
--rwxr-xr-x   0 runner    (1001) docker     (123)      119 2023-05-26 02:48:05.000000 disposable-email-domains-0.0.90/bin/release
--rwxr-xr-x   0 runner    (1001) docker     (123)      292 2023-05-26 02:48:05.000000 disposable-email-domains-0.0.90/bin/update
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:48:17.945647 disposable-email-domains-0.0.90/disposable_email_domains/
--rw-r--r--   0 runner    (1001) docker     (123)    74207 2023-05-26 02:48:05.000000 disposable-email-domains-0.0.90/disposable_email_domains/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:48:17.945647 disposable-email-domains-0.0.90/disposable_email_domains.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-26 02:48:17.000000 disposable-email-domains-0.0.90/disposable_email_domains.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-26 02:48:17.000000 disposable-email-domains-0.0.90/disposable_email_domains.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 02:48:17.000000 disposable-email-domains-0.0.90/disposable_email_domains.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-26 02:48:17.000000 disposable-email-domains-0.0.90/disposable_email_domains.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-26 02:48:17.000000 disposable-email-domains-0.0.90/disposable_email_domains.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-26 02:48:17.945647 disposable-email-domains-0.0.90/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-26 02:48:05.000000 disposable-email-domains-0.0.90/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:48:17.945647 disposable-email-domains-0.0.90/source_data/
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-26 02:48:05.000000 disposable-email-domains-0.0.90/source_data/allowlist.conf
--rw-r--r--   0 runner    (1001) docker     (123)    45996 2023-05-26 02:48:05.000000 disposable-email-domains-0.0.90/source_data/disposable_email_blocklist.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:48:17.945647 disposable-email-domains-0.0.90/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 02:48:05.000000 disposable-email-domains-0.0.90/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-26 02:48:05.000000 disposable-email-domains-0.0.90/tests/test_allowlist.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-26 02:48:05.000000 disposable-email-domains-0.0.90/tests/test_blocklist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:48:39.035858 disposable-email-domains-0.0.91/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-18 15:48:27.000000 disposable-email-domains-0.0.91/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-18 15:48:27.000000 disposable-email-domains-0.0.91/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-18 15:48:27.000000 disposable-email-domains-0.0.91/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-18 15:48:39.035858 disposable-email-domains-0.0.91/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-18 15:48:27.000000 disposable-email-domains-0.0.91/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:48:39.031858 disposable-email-domains-0.0.91/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1171 2023-07-18 15:48:27.000000 disposable-email-domains-0.0.91/bin/check_for_differences
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-18 15:48:27.000000 disposable-email-domains-0.0.91/bin/parse_source_data
+-rwxr-xr-x   0 runner    (1001) docker     (123)       83 2023-07-18 15:48:27.000000 disposable-email-domains-0.0.91/bin/prerelease
+-rwxr-xr-x   0 runner    (1001) docker     (123)      119 2023-07-18 15:48:27.000000 disposable-email-domains-0.0.91/bin/release
+-rwxr-xr-x   0 runner    (1001) docker     (123)      292 2023-07-18 15:48:27.000000 disposable-email-domains-0.0.91/bin/update
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:48:39.031858 disposable-email-domains-0.0.91/disposable_email_domains/
+-rw-r--r--   0 runner    (1001) docker     (123)    74407 2023-07-18 15:48:27.000000 disposable-email-domains-0.0.91/disposable_email_domains/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:48:27.000000 disposable-email-domains-0.0.91/disposable_email_domains/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:48:39.031858 disposable-email-domains-0.0.91/disposable_email_domains.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-18 15:48:39.000000 disposable-email-domains-0.0.91/disposable_email_domains.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-18 15:48:39.000000 disposable-email-domains-0.0.91/disposable_email_domains.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 15:48:39.000000 disposable-email-domains-0.0.91/disposable_email_domains.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-18 15:48:39.000000 disposable-email-domains-0.0.91/disposable_email_domains.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-18 15:48:39.000000 disposable-email-domains-0.0.91/disposable_email_domains.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-18 15:48:39.035858 disposable-email-domains-0.0.91/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-18 15:48:27.000000 disposable-email-domains-0.0.91/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:48:39.031858 disposable-email-domains-0.0.91/source_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-18 15:48:27.000000 disposable-email-domains-0.0.91/source_data/allowlist.conf
+-rw-r--r--   0 runner    (1001) docker     (123)    46119 2023-07-18 15:48:27.000000 disposable-email-domains-0.0.91/source_data/disposable_email_blocklist.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:48:39.035858 disposable-email-domains-0.0.91/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:48:27.000000 disposable-email-domains-0.0.91/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-18 15:48:27.000000 disposable-email-domains-0.0.91/tests/test_allowlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-18 15:48:27.000000 disposable-email-domains-0.0.91/tests/test_blocklist.py
```

### Comparing `disposable-email-domains-0.0.90/LICENSE.txt` & `disposable-email-domains-0.0.91/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `disposable-email-domains-0.0.90/PKG-INFO` & `disposable-email-domains-0.0.91/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: disposable-email-domains
-Version: 0.0.90
+Version: 0.0.91
 Summary: A set of disposable email domains
 Home-page: https://github.com/disposable-email-domains/disposable-email-domains
 Author: Dustin Ingram
 Author-email: github@dustingram.com
 License: MIT
 Keywords: disposable email domains blocklist
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Typing :: Typed
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 # Disposable Email Domains
 
 This module provides a set of known disposable email domains.
```

### Comparing `disposable-email-domains-0.0.90/README.md` & `disposable-email-domains-0.0.91/README.md`

 * *Files identical despite different names*

### Comparing `disposable-email-domains-0.0.90/bin/check_for_differences` & `disposable-email-domains-0.0.91/bin/check_for_differences`

 * *Files identical despite different names*

### Comparing `disposable-email-domains-0.0.90/bin/parse_source_data` & `disposable-email-domains-0.0.91/bin/parse_source_data`

 * *Files identical despite different names*

### Comparing `disposable-email-domains-0.0.90/disposable_email_domains/__init__.py` & `disposable-email-domains-0.0.91/disposable_email_domains/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -586,14 +586,15 @@
     'badoop.com',
     'badpotato.tk',
     'balaket.com',
     'banit.club',
     'banit.me',
     'bank-opros1.ru',
     'bareed.ws',
+    'barooko.com',
     'barryogorman.com',
     'bartdevos.be',
     'basscode.org',
     'bauwerke-online.com',
     'bazaaboom.com',
     'bbbbyyzz.info',
     'bbhost.us',
@@ -733,14 +734,15 @@
     'carbtc.net',
     'cars2.club',
     'carsencyclopedia.com',
     'cartelera.org',
     'caseedu.tk',
     'cashflow35.com',
     'casualdx.com',
+    'catgroup.uk',
     'cavi.mx',
     'cbair.com',
     'cbes.net',
     'cc.liamria',
     'ccmail.uk',
     'cdfaq.com',
     'cdpa.cc',
@@ -1177,14 +1179,15 @@
     'ephemail.net',
     'ephemeral.email',
     'eposta.buzz',
     'eposta.work',
     'eqiluxspam.ga',
     'ereplyzy.com',
     'ericjohnson.ml',
+    'eripo.net',
     'ero-tube.org',
     'esadverse.com',
     'esbano-ru.ru',
     'esc.la',
     'escapehatchapp.com',
     'esemay.com',
     'esgeneri.com',
@@ -1214,14 +1217,15 @@
     'extracurricularsociety.com',
     'extremail.ru',
     'eyepaste.com',
     'ez.lv',
     'ezehe.com',
     'ezfill.com',
     'ezstest.com',
+    'ezztt.com',
     'f4k.es',
     'f5.si',
     'facebook-email.cf',
     'facebook-email.ga',
     'facebook-email.ml',
     'facebookmail.gq',
     'facebookmail.ml',
@@ -1471,14 +1475,15 @@
     'gmial.com',
     'gmx1mail.top',
     'gmxmail.top',
     'gmxmail.win',
     'gnctr-calgary.com',
     'go2usa.info',
     'go2vpn.net',
+    'goatmail.uk',
     'goemailgo.com',
     'golemico.com',
     'gomail.in',
     'goonby.com',
     'goplaygame.ru',
     'gorillaswithdirtyarmpits.com',
     'goround.info',
@@ -1644,14 +1649,15 @@
     'iaoss.com',
     'ibnuh.bz',
     'icantbelieveineedtoexplainthisshit.com',
     'icemail.club',
     'ichigo.me',
     'icx.in',
     'icx.ro',
+    'icznn.com',
     'idx4.com',
     'idxue.com',
     'ieatspam.eu',
     'ieatspam.info',
     'ieh-mail.de',
     'iencm.com',
     'iffymedia.com',
@@ -1715,14 +1721,15 @@
     'insorg-mail.info',
     'instaddr.ch',
     'instance-email.com',
     'instant-mail.de',
     'instantblingmail.info',
     'instantemailaddress.com',
     'instantmail.fr',
+    'instmail.uk',
     'internet-v-stavropole.ru',
     'internetoftags.com',
     'interstats.org',
     'intersteller.com',
     'intopwa.com',
     'intopwa.net',
     'intopwa.org',
@@ -2442,14 +2449,15 @@
     'nutpa.net',
     'nuts2trade.com',
     'nvhrw.com',
     'nwldx.com',
     'nwytg.com',
     'nwytg.net',
     'ny7.me',
+    'nyasan.com',
     'nypato.com',
     'nyrmusic.com',
     'o2stk.org',
     'o7i.net',
     'oalsp.com',
     'obfusko.com',
     'objectmail.com',
@@ -2459,14 +2467,15 @@
     'octovie.com',
     'odaymail.com',
     'odem.com',
     'odnorazovoe.ru',
     'oepia.com',
     'oerpub.org',
     'offshore-proxies.net',
+    'ofisher.net',
     'ohaaa.de',
     'ohi.tw',
     'oida.icu',
     'oing.cf',
     'okclprojects.com',
     'okinawa.li',
     'okrent.us',
@@ -2818,14 +2827,15 @@
     'sexforswingers.com',
     'sexical.com',
     'sexyalwasmi.top',
     'shadap.org',
     'shalar.net',
     'sharedmailbox.org',
     'sharklasers.com',
+    'shchiba.uk',
     'sheryli.com',
     'shhmail.com',
     'shhuut.org',
     'shieldedmail.com',
     'shieldemail.com',
     'shiftmail.com',
     'shipfromto.com',
@@ -3663,14 +3673,15 @@
     'zcrcd.com',
     'zdenka.net',
     'ze.tc',
     'zebins.com',
     'zebins.eu',
     'zehnminuten.de',
     'zehnminutenmail.de',
+    'zemzar.net',
     'zepp.dk',
     'zetmail.com',
     'zfymail.com',
     'zhaoqian.ninja',
     'zhaoyuanedu.cn',
     'zhcne.com',
     'zhewei88.com',
```

### Comparing `disposable-email-domains-0.0.90/disposable_email_domains.egg-info/PKG-INFO` & `disposable-email-domains-0.0.91/disposable_email_domains.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: disposable-email-domains
-Version: 0.0.90
+Version: 0.0.91
 Summary: A set of disposable email domains
 Home-page: https://github.com/disposable-email-domains/disposable-email-domains
 Author: Dustin Ingram
 Author-email: github@dustingram.com
 License: MIT
 Keywords: disposable email domains blocklist
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Typing :: Typed
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 # Disposable Email Domains
 
 This module provides a set of known disposable email domains.
```

### Comparing `disposable-email-domains-0.0.90/disposable_email_domains.egg-info/SOURCES.txt` & `disposable-email-domains-0.0.91/disposable_email_domains.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 setup.py
 bin/check_for_differences
 bin/parse_source_data
 bin/prerelease
 bin/release
 bin/update
 disposable_email_domains/__init__.py
+disposable_email_domains/py.typed
 disposable_email_domains.egg-info/PKG-INFO
 disposable_email_domains.egg-info/SOURCES.txt
 disposable_email_domains.egg-info/dependency_links.txt
 disposable_email_domains.egg-info/requires.txt
 disposable_email_domains.egg-info/top_level.txt
 source_data/allowlist.conf
 source_data/disposable_email_blocklist.conf
```

### Comparing `disposable-email-domains-0.0.90/setup.py` & `disposable-email-domains-0.0.91/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 from codecs import open
 from os import path
 
 here = path.abspath(path.dirname(__file__))
 
-__version__ = "0.0.90"
+__version__ = "0.0.91"
 
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="disposable-email-domains",
     version=__version__,
@@ -20,18 +20,21 @@
     author_email="github@dustingram.com",
     license="MIT",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Typing :: Typed",
     ],
     keywords="disposable email domains blocklist",
     packages=["disposable_email_domains"],
+    package_data={"disposable_email_domains": ["py.typed"]},
     extras_require={
         "dev": ["check-manifest"],
     },
 )
```

### Comparing `disposable-email-domains-0.0.90/source_data/allowlist.conf` & `disposable-email-domains-0.0.91/source_data/allowlist.conf`

 * *Files identical despite different names*

### Comparing `disposable-email-domains-0.0.90/source_data/disposable_email_blocklist.conf` & `disposable-email-domains-0.0.91/source_data/disposable_email_blocklist.conf`

 * *Files 0% similar despite different names*

```diff
@@ -407,14 +407,15 @@
 badoop.com
 badpotato.tk
 balaket.com
 banit.club
 banit.me
 bank-opros1.ru
 bareed.ws
+barooko.com
 barryogorman.com
 bartdevos.be
 basscode.org
 bauwerke-online.com
 bazaaboom.com
 bbbbyyzz.info
 bbhost.us
@@ -554,14 +555,15 @@
 carbtc.net
 cars2.club
 carsencyclopedia.com
 cartelera.org
 caseedu.tk
 cashflow35.com
 casualdx.com
+catgroup.uk
 cavi.mx
 cbair.com
 cbes.net
 cc.liamria
 ccmail.uk
 cdfaq.com
 cdpa.cc
@@ -998,14 +1000,15 @@
 ephemail.net
 ephemeral.email
 eposta.buzz
 eposta.work
 eqiluxspam.ga
 ereplyzy.com
 ericjohnson.ml
+eripo.net
 ero-tube.org
 esadverse.com
 esbano-ru.ru
 esc.la
 escapehatchapp.com
 esemay.com
 esgeneri.com
@@ -1035,14 +1038,15 @@
 extracurricularsociety.com
 extremail.ru
 eyepaste.com
 ez.lv
 ezehe.com
 ezfill.com
 ezstest.com
+ezztt.com
 f4k.es
 f5.si
 facebook-email.cf
 facebook-email.ga
 facebook-email.ml
 facebookmail.gq
 facebookmail.ml
@@ -1292,14 +1296,15 @@
 gmial.com
 gmx1mail.top
 gmxmail.top
 gmxmail.win
 gnctr-calgary.com
 go2usa.info
 go2vpn.net
+goatmail.uk
 goemailgo.com
 golemico.com
 gomail.in
 goonby.com
 goplaygame.ru
 gorillaswithdirtyarmpits.com
 goround.info
@@ -1465,14 +1470,15 @@
 iaoss.com
 ibnuh.bz
 icantbelieveineedtoexplainthisshit.com
 icemail.club
 ichigo.me
 icx.in
 icx.ro
+icznn.com
 idx4.com
 idxue.com
 ieatspam.eu
 ieatspam.info
 ieh-mail.de
 iencm.com
 iffymedia.com
@@ -1536,14 +1542,15 @@
 insorg-mail.info
 instaddr.ch
 instance-email.com
 instant-mail.de
 instantblingmail.info
 instantemailaddress.com
 instantmail.fr
+instmail.uk
 internet-v-stavropole.ru
 internetoftags.com
 interstats.org
 intersteller.com
 intopwa.com
 intopwa.net
 intopwa.org
@@ -2263,14 +2270,15 @@
 nutpa.net
 nuts2trade.com
 nvhrw.com
 nwldx.com
 nwytg.com
 nwytg.net
 ny7.me
+nyasan.com
 nypato.com
 nyrmusic.com
 o2stk.org
 o7i.net
 oalsp.com
 obfusko.com
 objectmail.com
@@ -2280,14 +2288,15 @@
 octovie.com
 odaymail.com
 odem.com
 odnorazovoe.ru
 oepia.com
 oerpub.org
 offshore-proxies.net
+ofisher.net
 ohaaa.de
 ohi.tw
 oida.icu
 oing.cf
 okclprojects.com
 okinawa.li
 okrent.us
@@ -2639,14 +2648,15 @@
 sexforswingers.com
 sexical.com
 sexyalwasmi.top
 shadap.org
 shalar.net
 sharedmailbox.org
 sharklasers.com
+shchiba.uk
 sheryli.com
 shhmail.com
 shhuut.org
 shieldedmail.com
 shieldemail.com
 shiftmail.com
 shipfromto.com
@@ -3484,14 +3494,15 @@
 zcrcd.com
 zdenka.net
 ze.tc
 zebins.com
 zebins.eu
 zehnminuten.de
 zehnminutenmail.de
+zemzar.net
 zepp.dk
 zetmail.com
 zfymail.com
 zhaoqian.ninja
 zhaoyuanedu.cn
 zhcne.com
 zhewei88.com
```

