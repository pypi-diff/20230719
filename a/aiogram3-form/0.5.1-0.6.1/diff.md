# Comparing `tmp/aiogram3_form-0.5.1.tar.gz` & `tmp/aiogram3_form-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiogram3_form-0.5.1.tar", max compression
+gzip compressed data, was "aiogram3_form-0.6.1.tar", max compression
```

## Comparing `aiogram3_form-0.5.1.tar` & `aiogram3_form-0.6.1.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0      294 2023-05-28 20:07:11.098853 aiogram3_form-0.5.1/aiogram3_form/__init__.py
--rw-r--r--   0        0        0     1383 2023-04-13 18:33:34.599104 aiogram3_form-0.5.1/aiogram3_form/field.py
--rw-r--r--   0        0        0      843 2023-01-24 00:46:35.276915 aiogram3_form-0.5.1/aiogram3_form/filters.py
--rw-r--r--   0        0        0     8500 2023-06-22 21:12:33.945649 aiogram3_form-0.5.1/aiogram3_form/form.py
--rw-r--r--   0        0        0      120 2023-01-24 00:23:37.244911 aiogram3_form-0.5.1/aiogram3_form/state.py
--rw-r--r--   0        0        0     1092 2023-01-24 00:20:12.265098 aiogram3_form-0.5.1/LICENSE
--rw-r--r--   0        0        0      520 2023-06-23 00:19:42.272913 aiogram3_form-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     1372 2023-06-22 20:59:34.559238 aiogram3_form-0.5.1/README.md
--rw-r--r--   0        0        0     1918 1970-01-01 00:00:00.000000 aiogram3_form-0.5.1/setup.py
--rw-r--r--   0        0        0     1861 1970-01-01 00:00:00.000000 aiogram3_form-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-18 22:37:19.411827 aiogram3_form-0.6.1/LICENSE
+-rw-r--r--   0        0        0     1323 2023-07-19 12:10:22.823416 aiogram3_form-0.6.1/README.md
+-rw-r--r--   0        0        0      281 2023-07-18 22:37:19.412382 aiogram3_form-0.6.1/aiogram3_form/__init__.py
+-rw-r--r--   0        0        0     1539 2023-07-18 23:23:33.831108 aiogram3_form-0.6.1/aiogram3_form/field.py
+-rw-r--r--   0        0        0      865 2023-07-18 23:36:48.112204 aiogram3_form-0.6.1/aiogram3_form/filters.py
+-rw-r--r--   0        0        0     8287 2023-07-19 12:14:19.744334 aiogram3_form-0.6.1/aiogram3_form/form.py
+-rw-r--r--   0        0        0      282 2023-07-18 23:15:44.172457 aiogram3_form-0.6.1/aiogram3_form/state.py
+-rw-r--r--   0        0        0      502 2023-07-19 12:18:18.398271 aiogram3_form-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     1865 1970-01-01 00:00:00.000000 aiogram3_form-0.6.1/PKG-INFO
```

### Comparing `aiogram3_form-0.5.1/aiogram3_form/field.py` & `aiogram3_form-0.6.1/aiogram3_form/field.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,50 @@
-from dataclasses import dataclass
-from typing import Any, Awaitable, Callable, Dict, Optional, Type, Union
-
-from aiogram import types
-from aiogram.utils.magic_filter import MagicFilter
-
-Markup = Union[types.ReplyKeyboardMarkup, types.InlineKeyboardMarkup]
-FormFilter = Union[MagicFilter, Callable[..., Awaitable[Any]]]
-
-EnterCallback = Callable[[int, int, Dict[str, Any]], Awaitable[Any]]
-
-
-@dataclass(frozen=True)
-class FormFieldInfo:
-    enter_message_text: Optional[str]
-    error_message_text: Optional[str]
-    filter: Optional[FormFilter]
-    reply_markup: Optional[Markup]
-    enter_callback: Optional[EnterCallback]
-
-
-@dataclass
-class FormFieldData:
-    name: str
-    type: Type
-    info: FormFieldInfo
-
-
-def FormField(
-    *,
-    enter_message_text: Optional[str] = None,
-    filter: Optional[FormFilter] = None,
-    error_message_text: Optional[str] = None,
-    reply_markup: Optional[Markup] = None,
-    enter_callback: Optional[EnterCallback] = None
-) -> Any:
-    if enter_message_text is None and enter_callback is None:
-        raise ValueError("enter_message_text or enter_callback should be set")
-
-    return FormFieldInfo(
-        enter_message_text=enter_message_text,
-        error_message_text=error_message_text,
-        filter=filter,
-        reply_markup=reply_markup,
-        enter_callback=enter_callback,
-    )
+from dataclasses import dataclass
+from typing import Any, Awaitable, Callable, Dict, Optional, Type, Union
+
+from aiogram import types
+from aiogram.utils.magic_filter import MagicFilter
+
+Markup = Union[types.ReplyKeyboardMarkup, types.InlineKeyboardMarkup]
+FormFilter = Union[MagicFilter, Callable[..., Awaitable[Any]]]
+
+EnterCallback = Callable[[int, int, Dict[str, Any]], Awaitable[Any]]
+
+
+@dataclass(frozen=True)
+class FormFieldInfo:
+    enter_message_text: Optional[str]
+    error_message_text: Optional[str]
+    filter: Optional[FormFilter]
+    reply_markup: Optional[Markup]
+    enter_callback: Optional[EnterCallback]
+
+    def __post_init__(self):
+        if self.enter_message_text is None and self.enter_callback is None:
+            raise ValueError("enter_message_text or enter_callback should be set")
+
+
+@dataclass(frozen=True)
+class FormFieldData:
+    name: str
+    type: Type
+    info: FormFieldInfo
+
+
+def FormField(
+    *,
+    enter_message_text: Optional[str] = None,
+    filter: Optional[FormFilter] = None,
+    error_message_text: Optional[str] = None,
+    reply_markup: Optional[Markup] = None,
+    enter_callback: Optional[EnterCallback] = None
+) -> Any:
+    if enter_message_text is None and enter_callback is None:
+        raise ValueError("enter_message_text or enter_callback should be set")
+
+    return FormFieldInfo(
+        enter_message_text=enter_message_text,
+        error_message_text=error_message_text,
+        filter=filter,
+        reply_markup=reply_markup,
+        enter_callback=enter_callback,
+    )
```

### Comparing `aiogram3_form-0.5.1/aiogram3_form/filters.py` & `aiogram3_form-0.6.1/aiogram3_form/filters.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,29 @@
-import datetime
-from typing import Any, Awaitable, Callable, Union
-
-from aiogram import F, types
-from aiogram.utils.magic_filter import MagicFilter
-
-FormFilter = Union[MagicFilter, Callable[..., Awaitable[Any]]]
-
-DEFAULT_FORM_FILTERS = {
-    str: F.text,
-    int: F.text.func(int),
-    float: F.text.func(float),
-    datetime.date: F.text.func(
-        lambda text: datetime.datetime.strptime(text, r"%d.%m.%Y").date()
-    ),
-    datetime.datetime: F.text.func(
-        lambda text: datetime.datetime.strptime(text, r"%d.%m.%Y %H:%M")
-    ),
-    datetime.time: F.text.func(
-        lambda text: datetime.datetime.strptime(text, r"%H:%M").time()
-    ),
-    types.PhotoSize: F.photo.func(lambda photo: photo[-1]),
-    types.Document: F.document.func(lambda document: document),
-    types.Message: F.func(lambda m: m),
-}
+import datetime
+from typing import Any, Awaitable, Callable, Union
+
+from aiogram import F, types
+from aiogram.utils.magic_filter import MagicFilter
+
+FormFilter = Union[
+    MagicFilter,
+    Callable[..., Awaitable[Any]],
+    Callable[[types.Message], Any],
+]
+
+DEFAULT_FORM_FILTERS = {
+    str: F.text,
+    int: F.text.func(int),
+    float: F.text.func(float),
+    datetime.date: F.text.func(
+        lambda text: datetime.datetime.strptime(text, r"%d.%m.%Y").date()
+    ),
+    datetime.datetime: F.text.func(
+        lambda text: datetime.datetime.strptime(text, r"%d.%m.%Y %H:%M")
+    ),
+    datetime.time: F.text.func(
+        lambda text: datetime.datetime.strptime(text, r"%H:%M").time()
+    ),
+    types.PhotoSize: F.photo.func(lambda photo: photo[-1]),
+    types.Document: F.document.func(lambda document: document),
+    types.Message: F.func(lambda m: m),
+}
```

### Comparing `aiogram3_form-0.5.1/LICENSE` & `aiogram3_form-0.6.1/LICENSE`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 Andrei Morozov
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 Andrei Morozov
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `aiogram3_form-0.5.1/README.md` & `aiogram3_form-0.6.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-# aiogram3-form
-A library to create forms in aiogram3
-
-```shell
-pip install aiogram3-form
-```
-
-# Example
-```Python
-import asyncio
-
-from aiogram import Bot, Dispatcher, F, Router, types
-from aiogram3_form import Form, FormField
-from aiogram.fsm.context import FSMContext
-
-bot = Bot(token=YOUR_TOKEN)
-dispatcher = Dispatcher()
-router = Router()
-dispatcher.include_router(router)
-
-
-class NameForm(Form, router=router):
-    first_name: str = FormField(enter_message_text="Enter your first name please")
-    second_name: str = FormField(
-        enter_message_text="Enter your second name please",
-        filter=F.text.len() > 10 & F.text,
-    )
-    age: int = FormField(
-        enter_message_text="Enter age as integer",
-        error_message_text="Age should be numeric!",
-    )
-
-
-@NameForm.submit()
-async def name_form_submit_handler(form: NameForm, event_chat: types.Chat):
-    # handle form data
-    # also supports aiogram standart DI (e. g. middlewares, filters, etc)
-    await form.answer(
-        f"{form.first_name} {form.second_name} of age {form.age} in chat {event_chat.title}"
-    )
-
-
-@router.message(F.text == "/form")
-async def form_handler(_, state: FSMContext):
-    await NameForm.start(bot, state)  # start your form
-
-
-async def main():
-    await dispatcher.start_polling(bot)
-
-
-asyncio.run(main())
-```
+# aiogram3-form
+A library to create forms in aiogram3
+
+```shell
+pip install aiogram3-form
+```
+
+# Example
+```Python
+import asyncio
+
+from aiogram import Bot, Dispatcher, F, Router, types
+from aiogram3_form import Form, FormField
+from aiogram.fsm.context import FSMContext
+
+bot = Bot(token="YOUR_TOKEN")
+dispatcher = Dispatcher()
+router = Router()
+dispatcher.include_router(router)
+
+
+class NameForm(Form, router=router):
+    first_name: str = FormField(enter_message_text="Enter your first name please")
+    second_name: str = FormField(
+        enter_message_text="Enter your second name please",
+        filter=(F.text.len() > 10) & F.text,
+    )
+    age: int = FormField(
+        enter_message_text="Enter age as integer",
+        error_message_text="Age should be numeric!",
+    )
+
+
+@NameForm.submit()
+async def name_form_submit_handler(form: NameForm, event_chat: types.Chat):
+    # handle form data
+    # also supports aiogram standart DI (e. g. middlewares, filters, etc)
+    await form.answer(
+        f"{form.first_name} {form.second_name} of age {form.age} in chat {event_chat.title}"
+    )
+
+
+@router.message(F.text == "/form")
+async def form_handler(_, state: FSMContext):
+    await NameForm.start(bot, state)  # start your form
+
+
+async def main():
+    await dispatcher.start_polling(bot)
+
+
+asyncio.run(main())
+```
```

### Comparing `aiogram3_form-0.5.1/PKG-INFO` & `aiogram3_form-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiogram3-form
-Version: 0.5.1
+Version: 0.6.1
 Summary: A library to create forms in aiogram3
 License: MIT
 Author: TrixiS
 Author-email: oficialmorozov@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -25,25 +25,25 @@
 ```Python
 import asyncio
 
 from aiogram import Bot, Dispatcher, F, Router, types
 from aiogram3_form import Form, FormField
 from aiogram.fsm.context import FSMContext
 
-bot = Bot(token=YOUR_TOKEN)
+bot = Bot(token="YOUR_TOKEN")
 dispatcher = Dispatcher()
 router = Router()
 dispatcher.include_router(router)
 
 
 class NameForm(Form, router=router):
     first_name: str = FormField(enter_message_text="Enter your first name please")
     second_name: str = FormField(
         enter_message_text="Enter your second name please",
-        filter=F.text.len() > 10 & F.text,
+        filter=(F.text.len() > 10) & F.text,
     )
     age: int = FormField(
         enter_message_text="Enter age as integer",
         error_message_text="Age should be numeric!",
     )
```

