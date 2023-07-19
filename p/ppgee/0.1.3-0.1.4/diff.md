# Comparing `tmp/ppgee-0.1.3.tar.gz` & `tmp/ppgee-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ppgee-0.1.3.tar", max compression
+gzip compressed data, was "ppgee-0.1.4.tar", max compression
```

## Comparing `ppgee-0.1.3.tar` & `ppgee-0.1.4.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0       77 2023-07-19 05:31:14.682666 ppgee-0.1.3/ppgee/__init__.py
--rw-r--r--   0        0        0     1206 2023-07-19 04:28:34.984494 ppgee-0.1.3/ppgee/__main__.py
--rw-r--r--   0        0        0     2005 2023-07-19 05:30:13.889154 ppgee-0.1.3/ppgee/client.py
--rw-r--r--   0        0        0       99 2023-07-19 04:04:24.485053 ppgee-0.1.3/ppgee/errors.py
--rw-r--r--   0        0        0     1478 2023-07-19 04:04:24.485053 ppgee-0.1.3/ppgee/http.py
--rw-r--r--   0        0        0       73 2023-07-19 05:26:14.954583 ppgee-0.1.3/ppgee/pages/__init__.py
--rw-r--r--   0        0        0     1356 2023-07-19 04:04:24.488386 ppgee-0.1.3/ppgee/pages/frequency.py
--rw-r--r--   0        0        0     1191 2023-07-19 04:04:24.488386 ppgee-0.1.3/ppgee/parser.py
--rw-r--r--   0        0        0      412 2023-07-19 05:30:58.723497 ppgee-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      325 1970-01-01 00:00:00.000000 ppgee-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       77 2023-07-19 06:48:42.464866 ppgee-0.1.4/ppgee/__init__.py
+-rw-r--r--   0        0        0     1210 2023-07-19 06:40:18.981737 ppgee-0.1.4/ppgee/__main__.py
+-rw-r--r--   0        0        0     2069 2023-07-19 06:47:33.838249 ppgee-0.1.4/ppgee/client.py
+-rw-r--r--   0        0        0       99 2023-07-19 04:04:24.485053 ppgee-0.1.4/ppgee/errors.py
+-rw-r--r--   0        0        0     1480 2023-07-19 06:41:18.023233 ppgee-0.1.4/ppgee/http.py
+-rw-r--r--   0        0        0      159 2023-07-19 06:38:45.073293 ppgee-0.1.4/ppgee/pages/__init__.py
+-rw-r--r--   0        0        0     1198 2023-07-19 06:41:01.811319 ppgee-0.1.4/ppgee/pages/attendency.py
+-rw-r--r--   0        0        0       80 2023-07-19 06:40:48.722466 ppgee-0.1.4/ppgee/parsers/__init__.py
+-rw-r--r--   0        0        0     1472 2023-07-19 06:39:54.783856 ppgee-0.1.4/ppgee/parsers/attendency.py
+-rw-r--r--   0        0        0      286 2023-07-19 06:45:02.573564 ppgee-0.1.4/ppgee/permissions.py
+-rw-r--r--   0        0        0      412 2023-07-19 06:48:34.168239 ppgee-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      325 1970-01-01 00:00:00.000000 ppgee-0.1.4/PKG-INFO
```

### Comparing `ppgee-0.1.3/ppgee/__main__.py` & `ppgee-0.1.4/ppgee/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 
 
 async def cli():
     args = get_args()
     user, password = args.username, args.password
     try:
         async with PPGEE(user=user, password=password) as ppgee:
-            frequency_page = await ppgee.frequency()
+            attendency_page = await ppgee.attendency()
             await asyncio.sleep(1)
-            if frequency_page.is_available():
+            if attendency_page.is_available():
                 print("Attendency confirmed.")
-                await frequency_page.confirm()
+                await attendency_page.confirm()
             else:
                 eprint("Attendency not available yet.")
             await asyncio.sleep(1)
     except errors.InvalidCredentialsException:
         eprint("Invalid credentials.")
```

### Comparing `ppgee-0.1.3/ppgee/client.py` & `ppgee-0.1.4/ppgee/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,18 @@
-import aiohttp
 import logging
-from ppgee.http import HttpClient
-from ppgee.pages import FrequencyPage
-from functools import wraps
-from ppgee import errors
-
-logger = logging.getLogger(__name__)
 
+import aiohttp
 
-def is_logged_check(method):
-    @wraps(method)
-    def wrapper(self, *args, **kwargs):
-        if not self.is_logged:
-            raise Exception("You must be logged in to use this method")
-        return method(self, *args, **kwargs)
+from ppgee import errors
+from ppgee.http import HttpClient
+from ppgee.pages import AttendencyPage, AttendencyHistory, AttendencyHistoryEntry
+from ppgee.parsers import AttendencyParser
+from ppgee.permissions import is_logged_check
 
-    return wrapper
+logger = logging.getLogger(__name__)
 
 
 class PPGEE:
     def __init__(self, user: str | None = None, password: str | None = None) -> None:
         self.user = user
         self.password = password
         self.session: aiohttp.ClientSession
@@ -52,17 +45,23 @@
                 await self.close()
                 raise errors.InvalidCredentialsException()
             self.is_logged = True
         else:
             logger.info("Logged in without credentials")
 
     @is_logged_check
-    async def frequency(self) -> FrequencyPage:
-        logger.info("Requesting frequency page...")
-        html = await self.http.frequency()
-        return FrequencyPage(html, self.http.frequency_confirmation)
+    async def attendency(self) -> AttendencyPage:
+        logger.info("Requesting attendency page...")
+        html = await self.http.attendency()
+        parser = AttendencyParser(html)
+        history = AttendencyHistory(
+            (AttendencyHistoryEntry(**item) for item in parser.history())
+        )
+        return AttendencyPage(
+            history, self.http.attendency_confirmation, parser.availability()
+        )
 
     @is_logged_check
     async def logoff(self) -> None:
         logger.info("Logging off...")
         self.is_logged = False
         await self.http.logoff()
```

### Comparing `ppgee-0.1.3/ppgee/http.py` & `ppgee-0.1.4/ppgee/http.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,18 +22,18 @@
                 )
             return await resp.text()
 
     async def login(self, user: str, password: str) -> str:
         data: dict[str, str] = {"login": user, "senha": password}
         return await self._request("post", f"{URL_BASE}/login.php", data=data)
 
-    async def frequency(self) -> str:
+    async def attendency(self) -> str:
         return await self._request("get", f"{URL_BASE}/afreq.php")
 
-    async def frequency_confirmation(self) -> str:
+    async def attendency_confirmation(self) -> str:
         today = date.today()
         data: dict[str, str] = {
             "freqano": str(today.year),
             "freqmes": str(today.month),
             "confirma": "checkbox",
         }
         return await self._request("POST", f"{URL_BASE}/afreqpasso2.php", data=data)
```

### Comparing `ppgee-0.1.3/ppgee/pages/frequency.py` & `ppgee-0.1.4/ppgee/pages/attendency.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,51 +1,46 @@
 from dataclasses import dataclass
 from datetime import datetime
+from typing import Callable, Awaitable
 import logging
 
-from ppgee.parser import parse_frequency_history
-
 logger = logging.getLogger(__name__)
 
 
 @dataclass
-class HistoryEntry:
+class AttendencyHistoryEntry:
     year: int
     month: int
     asked: datetime
     confirmed: datetime | None
 
 
-class History(list[HistoryEntry]):
+class AttendencyHistory(list[AttendencyHistoryEntry]):
     def __str__(self) -> str:
         out: list[str] = []
         for entry in self:
             e = [entry.year, entry.month, entry.asked, entry.confirmed]
             out.append("\t".join(map(str, e)))
         return "\n".join(out)
 
 
-class FrequencyPage:
-    def __init__(self, html, confirmation_callback):
-        self.html = html
-        self._history = History()
+class AttendencyPage:
+    def __init__(
+        self,
+        history: AttendencyHistory,
+        confirmation_callback: Callable[[], Awaitable[str]],
+        available: bool,
+    ):
+        self._history = history
+        self._available = available
         self.confirmation_callback = confirmation_callback
 
-    def _build_history(self):
-        result_list = parse_frequency_history(self.html)
-        for item in result_list:
-            self._history.append(HistoryEntry(**item))
-
-    def history(self) -> History:
-        if not self._history:
-            self._build_history()
+    def history(self) -> AttendencyHistory:
         return self._history
 
     def is_available(self):
-        if "Opção não disponível" in self.html:
-            return False
-        return True
+        return self._available
 
     async def confirm(self) -> None:
         if self.is_available():
-            logger.info("Requesting frequency confirmation...")
+            logger.info("Requesting attendency confirmation...")
             await self.confirmation_callback()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ppgee-0.1.3/ppgee/parser.py` & `ppgee-0.1.4/ppgee/parsers/attendency.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,32 +15,39 @@
     "Setembro": 9,
     "Outubro": 10,
     "Novembro": 11,
     "Dezembro": 12,
 }
 
 
-def parse_frequency_history(html) -> list[dict]:
-    history = []
-    soup = BeautifulSoup(html, "html.parser")
-    table = soup.find_all("table")[2].find_all("table")[-1]
-    rows = table.find_all("tr")
-    for row in rows[1:]:
-        cols = row.find_all("td")
-        data = [ele.text.strip() for ele in cols]
-        year = int(data[0])
-        month = MONTH_MAP[data[1]]
-        date_asked = datetime.strptime(data[2], "%d/%m/%Y%H:%M")
-        date_confirmed = re.sub(r"[^[0-9:/]]*", "", data[3])
-        if date_confirmed == "":
-            date_confirmed = None
-        else:
-            date_confirmed = datetime.strptime(date_confirmed, "%d/%m/%Y%H:%M")
-        history.append(
-            {
-                "year": year,
-                "month": month,
-                "asked": date_asked,
-                "confirmed": date_confirmed,
-            }
-        )
-    return history
+class AttendencyParser:
+    def __init__(self, html: str) -> None:
+        self._html = html
+
+    def history(self) -> list[dict]:
+        history = []
+        soup = BeautifulSoup(self._html, "html.parser")
+        table = soup.find_all("table")[2].find_all("table")[-1]
+        rows = table.find_all("tr")
+        for row in rows[1:]:
+            cols = row.find_all("td")
+            data = [ele.text.strip() for ele in cols]
+            year = int(data[0])
+            month = MONTH_MAP[data[1]]
+            date_asked = datetime.strptime(data[2], "%d/%m/%Y%H:%M")
+            date_confirmed = re.sub(r"[^[0-9:/]]*", "", data[3])
+            if date_confirmed == "":
+                date_confirmed = None
+            else:
+                date_confirmed = datetime.strptime(date_confirmed, "%d/%m/%Y%H:%M")
+            history.append(
+                {
+                    "year": year,
+                    "month": month,
+                    "asked": date_asked,
+                    "confirmed": date_confirmed,
+                }
+            )
+        return history
+
+    def availability(self) -> bool:
+        return "Opção não disponível" not in self._html
```

