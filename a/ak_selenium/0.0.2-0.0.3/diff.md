# Comparing `tmp/ak_selenium-0.0.2.tar.gz` & `tmp/ak_selenium-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ak_selenium-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ak_selenium-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ak_selenium-0.0.2.tar` & `ak_selenium-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      694 2023-06-21 15:27:04.024515 ak_selenium-0.0.2/.github/workflows/test.yml
--rw-r--r--   0        0        0     2003 2023-06-21 08:31:27.810982 ak_selenium-0.0.2/.gitignore
--rw-r--r--   0        0        0     1100 2023-06-21 07:45:53.041694 ak_selenium-0.0.2/LICENSE
--rw-r--r--   0        0        0     2980 2023-06-21 15:23:54.097594 ak_selenium-0.0.2/README.md
--rw-r--r--   0        0        0    46704 2023-06-21 09:05:19.849182 ak_selenium-0.0.2/assets/Addl_Options.png
--rw-r--r--   0        0        0    80746 2023-06-21 08:59:29.420231 ak_selenium-0.0.2/assets/usage.png
--rw-r--r--   0        0        0      578 2023-06-21 08:36:54.049853 ak_selenium-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      155 2023-06-21 23:49:54.241562 ak_selenium-0.0.2/src/ak_selenium/__init__.py
--rw-r--r--   0        0        0     7171 2023-06-21 18:14:28.539445 ak_selenium-0.0.2/src/ak_selenium/browser.py
--rw-r--r--   0        0        0        0 2023-06-21 07:45:53.042694 ak_selenium-0.0.2/src/tests/__init__.py
--rw-r--r--   0        0        0     1260 2023-06-21 08:45:02.471607 ak_selenium-0.0.2/src/tests/test_browser.py
--rw-r--r--   0        0        0     3389 1970-01-01 00:00:00.000000 ak_selenium-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      700 2023-07-18 23:12:31.448394 ak_selenium-0.0.3/.github/workflows/test.yml
+-rw-r--r--   0        0        0     2004 2023-07-18 23:12:31.455511 ak_selenium-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1100 2023-04-21 15:49:54.583006 ak_selenium-0.0.3/LICENSE
+-rw-r--r--   0        0        0     3596 2023-07-18 23:28:48.146334 ak_selenium-0.0.3/README.md
+-rw-r--r--   0        0        0    46704 2023-07-18 23:12:31.472797 ak_selenium-0.0.3/assets/Addl_Options.png
+-rw-r--r--   0        0        0    80746 2023-07-18 23:12:31.482825 ak_selenium-0.0.3/assets/usage.png
+-rw-r--r--   0        0        0      576 2023-07-18 23:13:20.553573 ak_selenium-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      239 2023-07-18 23:34:22.876989 ak_selenium-0.0.3/src/ak_selenium/__init__.py
+-rw-r--r--   0        0        0     8235 2023-07-18 23:31:55.901692 ak_selenium-0.0.3/src/ak_selenium/browser.py
+-rw-r--r--   0        0        0        0 2023-04-21 17:00:43.559845 ak_selenium-0.0.3/src/tests/__init__.py
+-rw-r--r--   0        0        0     1260 2023-07-18 23:20:16.831814 ak_selenium-0.0.3/src/tests/test_browser.py
+-rw-r--r--   0        0        0     3983 1970-01-01 00:00:00.000000 ak_selenium-0.0.3/PKG-INFO
```

### Comparing `ak_selenium-0.0.2/.github/workflows/test.yml` & `ak_selenium-0.0.3/.github/workflows/test.yml`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 name: tests
 
-on: [push]
+on:
+  push:
+    paths-ignore:
+      - '**/README.md'
 
 jobs:
   build:
-    runs-on: ${{ matrix.os }}
-    paths-ignore:
-      - '**/README.md'
+    runs-on: '${{ matrix.os }}'
     strategy:
       matrix:
         python-version: ["3.9", "3.10"]
         os: [ubuntu-latest, macos-latest, windows-latest]
 
     steps:
       - uses: actions/checkout@v3
@@ -21,8 +22,8 @@
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           python -m pip install flit
           flit install
       - name: Test with pytest
         run: |
-          pytest .
+          pytest .
```

### Comparing `ak_selenium-0.0.2/.gitignore` & `ak_selenium-0.0.3/.gitignore`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -127,8 +127,8 @@
 
 # Pyre type checker
 .pyre/
 .vscode/settings.json
 WebDriver/chromedriver.exe
 nosync*
 *.pkl
-.pypirc
+.pypirc
```

### Comparing `ak_selenium-0.0.2/LICENSE` & `ak_selenium-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ak_selenium-0.0.2/README.md` & `ak_selenium-0.0.3/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -85,15 +85,37 @@
 ```bash
   flit install --pth-file
 ```
 
 <!-- Usage -->
 ## 3. Usage
 
-![Usage](assets/usage.png)
+```python
+from ak_selenium import Chrome, By, Keys
+chrome = Chrome(
+    headless=False, # Start Chrome in headless mode
+    chrome_userdata_path=r"path\to\user\data", #Defaults to correct location in windows
+    half_screen=True, # Set the browser to half the screen size (Only applicable if NOT `headless`)
+    )
+
+#Get Chromedriver
+driver = chrome.init_chrome()
+
+#Get the website
+driver.get("https://example.com")
+
+#Wait for elements to load
+locator = (By.TAG_NAME, "h1")
+chrome.Wait_for_locator(locator)
+
+#Get requests Session
+s = chrome.update_req_headers_cookies()
+s.get("https://www.iana.org/domains/reserved")
+
+```
 
 ### Additional Options
 
 ![Additional Options](assets/Addl_Options.png)
 <!-- Roadmap -->
 ## 4. Roadmap
```

#### html2text {}

```diff
@@ -18,17 +18,25 @@
 with custom options - Automatically try to add Chrome UserData - Add anti-bot
 detection measures - Pass selenium headers/cookies to requests library  ## 2.
 Getting Started ### 2.1. Dependencies Create the virutual environment and
 install dependencies ```bash python -m venv .venv .venv\Scripts\activate.bat
 pip install flit ```  ### 2.3. Installation #### 2.3.1. Production Install with
 flit ```bash flit install --deps production ``` Alternatively, you can use pip
 ```bash pip install ak_selenium ``` #### 2.3.2. Development Install with flit
-```bash flit install --pth-file ```  ## 3. Usage ![Usage](assets/usage.png) ###
-Additional Options ![Additional Options](assets/Addl_Options.png)  ## 4.
-Roadmap - [ ] Add beautifulsoup integration - [ ] Proxy  ## 5. License See
-LICENSE.txt for more information.  ## 6. Contact Arun Kishore - [@rpakishore]
-(mailto:pypi@rpakishore.co.in) Project Link: [https://github.com/rpakishore/
+```bash flit install --pth-file ```  ## 3. Usage ```python from ak_selenium
+import Chrome, By, Keys chrome = Chrome( headless=False, # Start Chrome in
+headless mode chrome_userdata_path=r"path\to\user\data", #Defaults to correct
+location in windows half_screen=True, # Set the browser to half the screen size
+(Only applicable if NOT `headless`) ) #Get Chromedriver driver =
+chrome.init_chrome() #Get the website driver.get("https://example.com") #Wait
+for elements to load locator = (By.TAG_NAME, "h1") chrome.Wait_for_locator
+(locator) #Get requests Session s = chrome.update_req_headers_cookies() s.get
+("https://www.iana.org/domains/reserved") ``` ### Additional Options !
+[Additional Options](assets/Addl_Options.png)  ## 4. Roadmap - [ ] Add
+beautifulsoup integration - [ ] Proxy  ## 5. License See LICENSE.txt for more
+information.  ## 6. Contact Arun Kishore - [@rpakishore](mailto:
+pypi@rpakishore.co.in) Project Link: [https://github.com/rpakishore/
 ak_selenium](https://github.com/rpakishore/ak_selenium)  ## 7. Acknowledgements
 - [Awesome README Template](https://github.com/Louis3797/awesome-readme-
 template/blob/main/README-WITHOUT-EMOJI.md) - [Banner Maker](https://
 banner.godori.dev/) - [Shields.io](https://shields.io/) - [Carbon](https://
 carbon.now.sh/)
```

### Comparing `ak_selenium-0.0.2/assets/Addl_Options.png` & `ak_selenium-0.0.3/assets/Addl_Options.png`

 * *Files identical despite different names*

### Comparing `ak_selenium-0.0.2/assets/usage.png` & `ak_selenium-0.0.3/assets/usage.png`

 * *Files identical despite different names*

### Comparing `ak_selenium-0.0.2/pyproject.toml` & `ak_selenium-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -25,13 +25,12 @@
 00000180: 6472 6976 6572 2d6d 616e 6167 6572 222c  driver-manager",
 00000190: 200d 0a20 2020 2022 7265 7175 6573 7473   ..    "requests
 000001a0: 220d 0a20 2020 205d 0d0a 0d0a 5b70 726f  "..    ]....[pro
 000001b0: 6a65 6374 2e6f 7074 696f 6e61 6c2d 6465  ject.optional-de
 000001c0: 7065 6e64 656e 6369 6573 5d0d 0a74 6573  pendencies]..tes
 000001d0: 7420 3d20 5b0d 0a20 2020 2022 7079 7465  t = [..    "pyte
 000001e0: 7374 222c 0d0a 2020 2020 2269 7079 6b65  st",..    "ipyke
-000001f0: 726e 656c 220d 0a5d 0d0a 0d0a 0d0a 5b70  rnel"..]......[p
-00000200: 726f 6a65 6374 2e75 726c 735d 0d0a 486f  roject.urls]..Ho
-00000210: 6d65 203d 2022 6874 7470 733a 2f2f 6769  me = "https://gi
-00000220: 7468 7562 2e63 6f6d 2f72 7061 6b69 7368  thub.com/rpakish
-00000230: 6f72 652f 616b 5f73 656c 656e 6975 6d22  ore/ak_selenium"
-00000240: 0d0a                                     ..
+000001f0: 726e 656c 220d 0a5d 0d0a 0d0a 5b70 726f  rnel"..]....[pro
+00000200: 6a65 6374 2e75 726c 735d 0d0a 486f 6d65  ject.urls]..Home
+00000210: 203d 2022 6874 7470 733a 2f2f 6769 7468   = "https://gith
+00000220: 7562 2e63 6f6d 2f72 7061 6b69 7368 6f72  ub.com/rpakishor
+00000230: 652f 616b 5f73 656c 656e 6975 6d22 0d0a  e/ak_selenium"..
```

### Comparing `ak_selenium-0.0.2/src/ak_selenium/browser.py` & `ak_selenium-0.0.3/src/ak_selenium/browser.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,73 +1,89 @@
 from selenium import webdriver
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.support.wait import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.common.by import By
-from selenium.common.exceptions import TimeoutException
-from selenium.common.exceptions import NoSuchElementException
+from selenium.common import exceptions
 from selenium.webdriver.chrome.service import Service
 from selenium.webdriver.chrome.options import Options
-
-
 from selenium.webdriver.remote.webelement import WebElement
-
-
 from webdriver_manager.chrome import ChromeDriverManager
-
 from pathlib import Path
 import sys
+from typing import Literal
+import requests
 
 class Chrome:
     USERAGENT = 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) \
                 AppleWebKit/537.36 (KHTML, like Gecko) \
                 Chrome/83.0.4103.53 Safari/537.36'
     IMPLICITLY_WAIT_TIME = 3
     MAX_WAIT_TIME = 5
+    EXCEPTIONS = exceptions
 
-    def __init__(
-            self, headless:bool = False, 
-            Chrome_userdata_path:str=None, 
-            half_screen:bool=True):
+    def __init__(self, headless:bool = False, chrome_userdata_path:str=None, half_screen:bool=True):
+        
         self.headless = headless
         
-        if not Chrome_userdata_path and sys.platform=="win32":
-            Chrome_userdata_path = Path.home() / 'AppData' / 'Local' / 'Google' / 'Chrome' / 'User Data'
-            if not Chrome_userdata_path.exists():
-                Chrome_userdata_path = None
+        if not chrome_userdata_path and sys.platform=="win32":
+            chrome_userdata_path = Path.home() / 'AppData' / 'Local' / 'Google' / 'Chrome' / 'User Data'
+            if not chrome_userdata_path.exists():
+                chrome_userdata_path = None
             else:
-                Chrome_userdata_path = str(Chrome_userdata_path)
-        self.Chrome_userdata_path = Chrome_userdata_path
+                chrome_userdata_path = str(chrome_userdata_path)
+        self.chrome_userdata_path = chrome_userdata_path
         self.half_screen = half_screen
         self.s = None
+        self.driver = None
         return None
-
+    
+    def __str__(self) -> str:
+        return f"""
+        Chrome.Object
+        UserAgent:{self.USERAGENT}
+        Implicit Wait Time: {self.IMPLICITLY_WAIT_TIME:.2f}s
+        Max Wait Time: {self.MAX_WAIT_TIME:.2f}s
+        Headless: {self.headless}
+        Chrome Userdata Path: {self.chrome_userdata_path}
+        Half Screen View: {self.half_screen}
+        """
+    
+    def __repr__(self) -> str:
+        return f"Chrome(headless={self.headless},\
+                chrome_userdata_path={self.chrome_userdata_path},\
+                half_screen={self.half_screen})"
+    
+    def __del__(self) -> None:
+        if self.driver:
+            self.driver.quit()
+        return None
+    
     def init_chrome(self) -> webdriver.Chrome:
         """
         Initializes a Chrome web driver with specific options and configurations.
         
         Returns:
             webdriver.Chrome: The initialized Chrome driver object.
         """
         options = webdriver.ChromeOptions()
         options.add_argument('--disable-gpu')
         if self.headless:
             options.add_argument('--headless')
             options.add_argument("--window-size=1920,1080")
         options.add_argument("start-maximized")
         options.add_experimental_option("excludeSwitches", ["enable-logging"])
-        if self.Chrome_userdata_path:
-            options.add_argument('--user-data-dir=' + self.Chrome_userdata_path)
+        if self.chrome_userdata_path:
+            options.add_argument('--user-data-dir=' + self.chrome_userdata_path)
         options.add_experimental_option('useAutomationExtension', False)
     
-        options = _ram_optimization_browser_options(options)
+        options = self._ram_optimization_browser_options(options)
 
-        self.driver = webdriver.Chrome(service=Service(ChromeDriverManager().install()),
+        driver = webdriver.Chrome(service=Service(ChromeDriverManager().install()),
                                        options=options)
-        driver = self.driver
 
         driver.implicitly_wait(self.IMPLICITLY_WAIT_TIME) 
 
         driver.execute_script('window.focus()')
         driver.execute_cdp_cmd('Network.setUserAgentOverride',
                                {"userAgent": self.USERAGENT})
 
@@ -83,67 +99,74 @@
         driver.execute_cdp_cmd("Network.setExtraHTTPHeaders",
                                {"headers": {"User-Agent": "browser1"}})
 
         if self.half_screen:
             size = driver.get_window_size()
             driver.set_window_size(size['width']/2, size['height'])
             driver.set_window_position(size['width']/2-13, 0)
+            
         self.driver = driver
+        
         return driver
 
-    def __str__(self) -> str:
-        return f"""
-        Chrome.Object
-        UserAgent:{self.USERAGENT}
-        Implicit Wait Time: {self.IMPLICITLY_WAIT_TIME:.2f}s
-        Max Wait Time: {self.MAX_WAIT_TIME:.2f}s
-        Headless: {self.headless}
-        Chrome Userdata Path: {self.Chrome_userdata_path}
-        Half Screen View: {self.half_screen}
-        """
-    
-    def __repr__(self) -> str:
-        return f"Chrome(headless={self.headless},\
-                Chrome_userdata_path={self.Chrome_userdata_path},\
-                half_screen={self.half_screen})"
-    
-    def __del__(self) -> None:
-        driver = self.driver
-        try:
-            driver.quit()
-        except Exception as e:
-            print(str(e))
+    @staticmethod
+    def _ram_optimization_browser_options(options: Options) -> Options:
+        options.add_argument("disable-infobars")
+        options.add_experimental_option("excludeSwitches", 
+                                        ['enable-automation', "enable-logging"])
+        options.add_argument("--no-sandbox")
+        options.add_argument("--disable-extensions")
+        options.add_argument("--disable-application-cache")
+        options.add_argument("--disable-gpu")
+        options.add_argument("--disable-dev-shm-usage")
+        options.add_argument("--lang=en-US")
         
-        return None
-
+        # Based on https://stackoverflow.com/questions/59514049/unable-to-sign-into-google-with-selenium-automation-because-of-this-browser-or
+        options.add_argument("--allow-running-insecure-content")
+        options.add_argument("--disable-web-security")
+        return options
+    
     def Wait_for_locator(self,locator: tuple) -> None:
+        """
+        Wait until the element with the specified locator is present.
+
+        Args:
+            locator (tuple): The locator tuple (By, value) of the element to wait for.
+        """
         (
             WebDriverWait(self.driver, self.MAX_WAIT_TIME, 0.5)
             .until(EC.presence_of_element_located(locator))
         )
         return None
 
     @staticmethod
-    def fill_userinput_form(element, text, clear_existing=True) -> None:
+    def fill_userinput_form(element: WebElement, text: str, clear_existing: bool=True) -> None:
+        """
+        Fill a user input form element with the specified text.
+
+        Args:
+            element (WebElement): The input form element.
+            text (str): The text to fill in the form element.
+            clear_existing (bool): Whether to clear existing text before filling. Defaults to True.
+        """
         if clear_existing:
             element.clear()
         element.send_keys(text)
-        
-    def get_By_and_Keys(self):
-        return By, Keys
     
-    def init_requests(self):
-        import requests
+    def init_requests(self) -> requests.Session:
+        
         self.s = requests.Session()
         return self.s
     
-    def update_req_headers_cookies(self):
+    def update_req_headers_cookies(self) -> requests.Session:
         driver = self.driver
         if not self.s:
             s = self.init_requests()
+        else:
+            s = self.s
         s.cookies.update({c['name']: c['value'] for c in driver.get_cookies()})
         s.headers.update({
             "Accept-Language": driver.execute_script("return window.navigator.language;"),
             "X-Forwarded-For": driver.execute_script("return window.navigator.ip;"),
             "X-Timezone": driver.execute_script("return window.navigator.timezone;"),
             "User-Agent": driver.execute_script("return window.navigator.userAgent;"),
             "Connection": "keep-alive"
@@ -164,24 +187,19 @@
             WebElement or None: The first WebElement that matches the provided text, or None if no match is found.
         """
         for element in elements:
             if element.text.strip() == text:
                 return element
         return None
     
-
-def _ram_optimization_browser_options(options: Options) -> Options:
-    options.add_argument("disable-infobars")
-    options.add_experimental_option("excludeSwitches", 
-                                    ['enable-automation', "enable-logging"])
-    options.add_argument("--no-sandbox")
-    options.add_argument("--disable-extensions")
-    options.add_argument("--no-sandbox")
-    options.add_argument("--disable-application-cache")
-    options.add_argument("--disable-gpu")
-    options.add_argument("--disable-dev-shm-usage")
-    options.add_argument("--lang=en-US")
-    
-    # Based on https://stackoverflow.com/questions/59514049/unable-to-sign-into-google-with-selenium-automation-because-of-this-browser-or
-    options.add_argument("--allow-running-insecure-content")
-    options.add_argument("--disable-web-security")
-    return options
+    def scroll(self, direction: Literal["top", "bottom"] = "bottom") -> None:
+        """
+        Scroll the webpage to the specified direction.
+        Args:
+            direction (Literal["top", "bottom"]): The direction to scroll. Valid 
+                values are "top" and "bottom". Defaults to "bottom"
+        """
+        match direction:
+            case "top":
+                self.driver.execute_script("window.scrollTo(0, 0)")
+            case "bottom":
+                self.driver.execute_script("window.scrollTo(0, document.body.scrollHeight);")
```

### Comparing `ak_selenium-0.0.2/src/tests/test_browser.py` & `ak_selenium-0.0.3/src/tests/test_browser.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,10 +27,10 @@
 def test_str_method(chrome_instance):
     assert str(chrome_instance) == f"""
         Chrome.Object
         UserAgent:{chrome_instance.USERAGENT}
         Implicit Wait Time: {chrome_instance.IMPLICITLY_WAIT_TIME:.2f}s
         Max Wait Time: {chrome_instance.MAX_WAIT_TIME:.2f}s
         Headless: {chrome_instance.headless}
-        Chrome Userdata Path: {chrome_instance.Chrome_userdata_path}
+        Chrome Userdata Path: {chrome_instance.chrome_userdata_path}
         Half Screen View: {chrome_instance.half_screen}
         """
```

### Comparing `ak_selenium-0.0.2/PKG-INFO` & `ak_selenium-0.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ak_selenium
-Version: 0.0.2
+Version: 0.0.3
 Summary: Selenium package with requests integration and anti-bot detection measures
 Author-email: Arun Kishore <pypi@rpakishore.co.in>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: selenium
 Requires-Dist: webdriver-manager
 Requires-Dist: requests
@@ -100,15 +100,37 @@
 ```bash
   flit install --pth-file
 ```
 
 <!-- Usage -->
 ## 3. Usage
 
-![Usage](assets/usage.png)
+```python
+from ak_selenium import Chrome, By, Keys
+chrome = Chrome(
+    headless=False, # Start Chrome in headless mode
+    chrome_userdata_path=r"path\to\user\data", #Defaults to correct location in windows
+    half_screen=True, # Set the browser to half the screen size (Only applicable if NOT `headless`)
+    )
+
+#Get Chromedriver
+driver = chrome.init_chrome()
+
+#Get the website
+driver.get("https://example.com")
+
+#Wait for elements to load
+locator = (By.TAG_NAME, "h1")
+chrome.Wait_for_locator(locator)
+
+#Get requests Session
+s = chrome.update_req_headers_cookies()
+s.get("https://www.iana.org/domains/reserved")
+
+```
 
 ### Additional Options
 
 ![Additional Options](assets/Addl_Options.png)
 <!-- Roadmap -->
 ## 4. Roadmap
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ak_selenium Version: 0.0.2 Summary: Selenium
+Metadata-Version: 2.1 Name: ak_selenium Version: 0.0.3 Summary: Selenium
 package with requests integration and anti-bot detection measures Author-email:
 Arun Kishore
 rpakishore.co.in> Description-Content-Type: text/markdown Classifier: License
 :: OSI Approved :: MIT License Requires-Dist: selenium Requires-Dist:
 webdriver-manager Requires-Dist: requests Requires-Dist: pytest ; extra ==
 "test" Requires-Dist: ipykernel ; extra == "test" Project-URL: Home, https://
 github.com/rpakishore/ak_selenium Provides-Extra: test
@@ -26,17 +26,25 @@
 with custom options - Automatically try to add Chrome UserData - Add anti-bot
 detection measures - Pass selenium headers/cookies to requests library  ## 2.
 Getting Started ### 2.1. Dependencies Create the virutual environment and
 install dependencies ```bash python -m venv .venv .venv\Scripts\activate.bat
 pip install flit ```  ### 2.3. Installation #### 2.3.1. Production Install with
 flit ```bash flit install --deps production ``` Alternatively, you can use pip
 ```bash pip install ak_selenium ``` #### 2.3.2. Development Install with flit
-```bash flit install --pth-file ```  ## 3. Usage ![Usage](assets/usage.png) ###
-Additional Options ![Additional Options](assets/Addl_Options.png)  ## 4.
-Roadmap - [ ] Add beautifulsoup integration - [ ] Proxy  ## 5. License See
-LICENSE.txt for more information.  ## 6. Contact Arun Kishore - [@rpakishore]
-(mailto:pypi@rpakishore.co.in) Project Link: [https://github.com/rpakishore/
+```bash flit install --pth-file ```  ## 3. Usage ```python from ak_selenium
+import Chrome, By, Keys chrome = Chrome( headless=False, # Start Chrome in
+headless mode chrome_userdata_path=r"path\to\user\data", #Defaults to correct
+location in windows half_screen=True, # Set the browser to half the screen size
+(Only applicable if NOT `headless`) ) #Get Chromedriver driver =
+chrome.init_chrome() #Get the website driver.get("https://example.com") #Wait
+for elements to load locator = (By.TAG_NAME, "h1") chrome.Wait_for_locator
+(locator) #Get requests Session s = chrome.update_req_headers_cookies() s.get
+("https://www.iana.org/domains/reserved") ``` ### Additional Options !
+[Additional Options](assets/Addl_Options.png)  ## 4. Roadmap - [ ] Add
+beautifulsoup integration - [ ] Proxy  ## 5. License See LICENSE.txt for more
+information.  ## 6. Contact Arun Kishore - [@rpakishore](mailto:
+pypi@rpakishore.co.in) Project Link: [https://github.com/rpakishore/
 ak_selenium](https://github.com/rpakishore/ak_selenium)  ## 7. Acknowledgements
 - [Awesome README Template](https://github.com/Louis3797/awesome-readme-
 template/blob/main/README-WITHOUT-EMOJI.md) - [Banner Maker](https://
 banner.godori.dev/) - [Shields.io](https://shields.io/) - [Carbon](https://
 carbon.now.sh/)
```

