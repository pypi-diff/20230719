# Comparing `tmp/lfinancial-0.3.0.tar.gz` & `tmp/lfinancial-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lfinancial-0.3.0.tar", last modified: Sat Jul 15 11:53:37 2023, max compression
+gzip compressed data, was "lfinancial-0.3.1.tar", last modified: Wed Jul 19 14:58:16 2023, max compression
```

## Comparing `lfinancial-0.3.0.tar` & `lfinancial-0.3.1.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 11:53:37.288041 lfinancial-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-15 11:53:18.000000 lfinancial-0.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-15 11:53:37.288041 lfinancial-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-15 11:53:18.000000 lfinancial-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 11:53:37.284042 lfinancial-0.3.0/lfinancial/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-15 11:53:18.000000 lfinancial-0.3.0/lfinancial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-07-15 11:53:18.000000 lfinancial-0.3.0/lfinancial/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-07-15 11:53:18.000000 lfinancial-0.3.0/lfinancial/financial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 11:53:37.288041 lfinancial-0.3.0/lfinancial/generators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 11:53:18.000000 lfinancial-0.3.0/lfinancial/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-07-15 11:53:18.000000 lfinancial-0.3.0/lfinancial/generators/bank.py
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-07-15 11:53:18.000000 lfinancial-0.3.0/lfinancial/generators/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-15 11:53:18.000000 lfinancial-0.3.0/lfinancial/generators/contry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-07-15 11:53:18.000000 lfinancial-0.3.0/lfinancial/generators/currency.py
--rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-07-15 11:53:18.000000 lfinancial-0.3.0/lfinancial/generators/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-15 11:53:18.000000 lfinancial-0.3.0/lfinancial/generators/gender.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-15 11:53:18.000000 lfinancial-0.3.0/lfinancial/generators/industry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-07-15 11:53:18.000000 lfinancial-0.3.0/lfinancial/generators/locale.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-15 11:53:18.000000 lfinancial-0.3.0/lfinancial/generators/mail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-07-15 11:53:18.000000 lfinancial-0.3.0/lfinancial/generators/name.py
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-15 11:53:18.000000 lfinancial-0.3.0/lfinancial/generators/phone.py
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-07-15 11:53:18.000000 lfinancial-0.3.0/lfinancial/generators/stock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-07-15 11:53:18.000000 lfinancial-0.3.0/lfinancial/generators/swift.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-15 11:53:18.000000 lfinancial-0.3.0/lfinancial/generators/timezone.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 11:53:37.288041 lfinancial-0.3.0/lfinancial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-15 11:53:37.000000 lfinancial-0.3.0/lfinancial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-15 11:53:37.000000 lfinancial-0.3.0/lfinancial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 11:53:37.000000 lfinancial-0.3.0/lfinancial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-15 11:53:37.000000 lfinancial-0.3.0/lfinancial.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 11:53:37.288041 lfinancial-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-15 11:53:18.000000 lfinancial-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 11:53:37.288041 lfinancial-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-15 11:53:18.000000 lfinancial-0.3.0/tests/test_document.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:58:16.339459 lfinancial-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-19 14:57:54.000000 lfinancial-0.3.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-19 14:58:16.339459 lfinancial-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-07-19 14:57:54.000000 lfinancial-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:58:16.339459 lfinancial-0.3.1/lfinancial/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-19 14:57:54.000000 lfinancial-0.3.1/lfinancial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-07-19 14:57:54.000000 lfinancial-0.3.1/lfinancial/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-07-19 14:57:54.000000 lfinancial-0.3.1/lfinancial/financial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:58:16.339459 lfinancial-0.3.1/lfinancial/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 14:57:54.000000 lfinancial-0.3.1/lfinancial/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-07-19 14:57:54.000000 lfinancial-0.3.1/lfinancial/generators/bank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-07-19 14:57:54.000000 lfinancial-0.3.1/lfinancial/generators/card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-07-19 14:57:54.000000 lfinancial-0.3.1/lfinancial/generators/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-19 14:57:54.000000 lfinancial-0.3.1/lfinancial/generators/contry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-07-19 14:57:54.000000 lfinancial-0.3.1/lfinancial/generators/currency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-07-19 14:57:54.000000 lfinancial-0.3.1/lfinancial/generators/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-19 14:57:54.000000 lfinancial-0.3.1/lfinancial/generators/gender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-19 14:57:54.000000 lfinancial-0.3.1/lfinancial/generators/industry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-07-19 14:57:54.000000 lfinancial-0.3.1/lfinancial/generators/locale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-19 14:57:54.000000 lfinancial-0.3.1/lfinancial/generators/mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-07-19 14:57:54.000000 lfinancial-0.3.1/lfinancial/generators/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-07-19 14:57:54.000000 lfinancial-0.3.1/lfinancial/generators/phone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-07-19 14:57:54.000000 lfinancial-0.3.1/lfinancial/generators/stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-07-19 14:57:54.000000 lfinancial-0.3.1/lfinancial/generators/swift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-19 14:57:54.000000 lfinancial-0.3.1/lfinancial/generators/timezone.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:58:16.339459 lfinancial-0.3.1/lfinancial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-19 14:58:16.000000 lfinancial-0.3.1/lfinancial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-19 14:58:16.000000 lfinancial-0.3.1/lfinancial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 14:58:16.000000 lfinancial-0.3.1/lfinancial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-19 14:58:16.000000 lfinancial-0.3.1/lfinancial.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 14:58:16.339459 lfinancial-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-19 14:57:54.000000 lfinancial-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 14:58:16.339459 lfinancial-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-19 14:57:54.000000 lfinancial-0.3.1/tests/test_document.py
```

### Comparing `lfinancial-0.3.0/LICENSE.txt` & `lfinancial-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lfinancial-0.3.0/PKG-INFO` & `lfinancial-0.3.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lfinancial
-Version: 0.3.0
+Version: 0.3.1
 Summary: Generate financial test data
 Author: zaneliu
 Author-email: lzy291980138@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -102,8 +102,29 @@
 # Shares
 
 f.gender()
 # Cis Man
 
 f.industry()
 # Software & Services
+
+f.CVD()
+# 252
+
+f.CVV()
+# 748
+
+f.CID()
+# 207
+
+f.CAV()
+# 459
+
+f.CVC()
+# 767
+
+f.CSC()
+# 3473
+
+f.CVN()
+# 541
 ```
```

### Comparing `lfinancial-0.3.0/README.md` & `lfinancial-0.3.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -90,8 +90,29 @@
 # Shares
 
 f.gender()
 # Cis Man
 
 f.industry()
 # Software & Services
+
+f.CVD()
+# 252
+
+f.CVV()
+# 748
+
+f.CID()
+# 207
+
+f.CAV()
+# 459
+
+f.CVC()
+# 767
+
+f.CSC()
+# 3473
+
+f.CVN()
+# 541
 ```
```

### Comparing `lfinancial-0.3.0/lfinancial/factory.py` & `lfinancial-0.3.1/lfinancial/factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from lfinancial.generators.bank import BankGenerator
+from lfinancial.generators.card import CardGenerator
 from lfinancial.generators.contry import CountryGenerator
 from lfinancial.generators.currency import CurrencyGenerator
 from lfinancial.generators.document import IDCodeGenerator
 from lfinancial.generators.gender import GenderGenerator
 from lfinancial.generators.industry import IndustryGenerator
 from lfinancial.generators.locale import LocaleGenerator
 from lfinancial.generators.mail import EmailGenerator
@@ -36,14 +37,21 @@
             "stock_exchange": StockGenerator(),
             "ticker_symbol": StockGenerator(),
             "tz_identifier": TimeZoneGenerator(),
             "locale": LocaleGenerator(),
             "product": StockGenerator(),
             "gender": GenderGenerator(),
             "industry": IndustryGenerator(),
+            "CSC": CardGenerator(),
+            "CID": CardGenerator(),
+            "CVC": CardGenerator(),
+            "CAV": CardGenerator(),
+            "CVV": CardGenerator(),
+            "CVD": CardGenerator(),
+            "CVN": CardGenerator(),
         }
 
     def register_generator(self, name, generator):
         self.generators[name] = generator
 
     def create_generator(self, name):
         if name in self.generators:
```

### Comparing `lfinancial-0.3.0/lfinancial/financial.py` & `lfinancial-0.3.1/lfinancial/financial.py`

 * *Files 15% similar despite different names*

```diff
@@ -77,14 +77,35 @@
 
     def gender(self, country=None):
         return self._generate("gender", country)
 
     def industry(self, country=None):
         return self._generate("industry", country)
 
+    def CSC(self, country=None):
+        return self._generate("CSC", country)
+
+    def CID(self, country=None):
+        return self._generate("CID", country)
+
+    def CVC(self, country=None):
+        return self._generate("CVC", country)
+
+    def CAV(self, country=None):
+        return self._generate("CAV", country)
+
+    def CVV(self, country=None):
+        return self._generate("CVV", country)
+
+    def CVD(self, country=None):
+        return self._generate("CVD", country)
+
+    def CVN(self, country=None):
+        return self._generate("CVN", country)
+
 
 if __name__ == '__main__':
     f = Financial()
     print(f.ssn())
     print(f.id_card())
     print(f.passport())
     print(f.nric())
@@ -104,7 +125,15 @@
     print(f.stock_exchange())
     print(f.ticker_symbol())
     print(f.tz_identifier())
     print(f.locale())
     print(f.product())
     print(f.gender())
     print(f.industry())
+    print(f.CVD())
+    print(f.CVV())
+    print(f.CID())
+    print(f.CAV())
+    print(f.CVC())
+    print(f.CSC())
+    print(f.CVN())
+
```

### Comparing `lfinancial-0.3.0/lfinancial/generators/bank.py` & `lfinancial-0.3.1/lfinancial/generators/bank.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.3.0/lfinancial/generators/const.py` & `lfinancial-0.3.1/lfinancial/generators/const.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.3.0/lfinancial/generators/contry.py` & `lfinancial-0.3.1/lfinancial/generators/contry.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.3.0/lfinancial/generators/currency.py` & `lfinancial-0.3.1/lfinancial/generators/currency.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.3.0/lfinancial/generators/document.py` & `lfinancial-0.3.1/lfinancial/generators/document.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.3.0/lfinancial/generators/gender.py` & `lfinancial-0.3.1/lfinancial/generators/gender.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.3.0/lfinancial/generators/industry.py` & `lfinancial-0.3.1/lfinancial/generators/industry.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.3.0/lfinancial/generators/locale.py` & `lfinancial-0.3.1/lfinancial/generators/locale.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.3.0/lfinancial/generators/mail.py` & `lfinancial-0.3.1/lfinancial/generators/mail.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.3.0/lfinancial/generators/name.py` & `lfinancial-0.3.1/lfinancial/generators/name.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.3.0/lfinancial/generators/phone.py` & `lfinancial-0.3.1/lfinancial/generators/phone.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.3.0/lfinancial/generators/stock.py` & `lfinancial-0.3.1/lfinancial/generators/stock.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.3.0/lfinancial/generators/swift.py` & `lfinancial-0.3.1/lfinancial/generators/swift.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.3.0/lfinancial/generators/timezone.py` & `lfinancial-0.3.1/lfinancial/generators/timezone.py`

 * *Files identical despite different names*

### Comparing `lfinancial-0.3.0/lfinancial.egg-info/PKG-INFO` & `lfinancial-0.3.1/lfinancial.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lfinancial
-Version: 0.3.0
+Version: 0.3.1
 Summary: Generate financial test data
 Author: zaneliu
 Author-email: lzy291980138@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -102,8 +102,29 @@
 # Shares
 
 f.gender()
 # Cis Man
 
 f.industry()
 # Software & Services
+
+f.CVD()
+# 252
+
+f.CVV()
+# 748
+
+f.CID()
+# 207
+
+f.CAV()
+# 459
+
+f.CVC()
+# 767
+
+f.CSC()
+# 3473
+
+f.CVN()
+# 541
 ```
```

### Comparing `lfinancial-0.3.0/lfinancial.egg-info/SOURCES.txt` & `lfinancial-0.3.1/lfinancial.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 lfinancial/financial.py
 lfinancial.egg-info/PKG-INFO
 lfinancial.egg-info/SOURCES.txt
 lfinancial.egg-info/dependency_links.txt
 lfinancial.egg-info/top_level.txt
 lfinancial/generators/__init__.py
 lfinancial/generators/bank.py
+lfinancial/generators/card.py
 lfinancial/generators/const.py
 lfinancial/generators/contry.py
 lfinancial/generators/currency.py
 lfinancial/generators/document.py
 lfinancial/generators/gender.py
 lfinancial/generators/industry.py
 lfinancial/generators/locale.py
```

### Comparing `lfinancial-0.3.0/setup.py` & `lfinancial-0.3.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 excluded_packages = ["docs", "tests", "tests.*"]
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='lfinancial',
-    version='0.3.0',
+    version='0.3.1',
     author='zaneliu',
     description='Generate financial test data',
     long_description=long_description,
     long_description_content_type="text/markdown",
     readme="README.md",
     author_email='lzy291980138@163.com',
     packages=find_packages(exclude=excluded_packages),
```

