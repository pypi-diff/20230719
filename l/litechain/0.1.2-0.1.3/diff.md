# Comparing `tmp/litechain-0.1.2.tar.gz` & `tmp/litechain-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litechain-0.1.2.tar", last modified: Fri Jul 14 08:20:18 2023, max compression
+gzip compressed data, was "litechain-0.1.3.tar", last modified: Wed Jul 19 10:02:44 2023, max compression
```

## Comparing `litechain-0.1.2.tar` & `litechain-0.1.3.tar`

### file list

```diff
@@ -1,34 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:20:18.640052 litechain-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-14 08:20:02.000000 litechain-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-14 08:20:02.000000 litechain-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-07-14 08:20:18.640052 litechain-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10061 2023-07-14 08:20:02.000000 litechain-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:20:18.636052 litechain-0.1.2/litechain/
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-07-14 08:20:02.000000 litechain-0.1.2/litechain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:20:18.636052 litechain-0.1.2/litechain/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-14 08:20:02.000000 litechain-0.1.2/litechain/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:20:18.640052 litechain-0.1.2/litechain/contrib/llms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:20:02.000000 litechain-0.1.2/litechain/contrib/llms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-07-14 08:20:02.000000 litechain-0.1.2/litechain/contrib/llms/gpt4all_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)    15813 2023-07-14 08:20:02.000000 litechain-0.1.2/litechain/contrib/llms/open_ai.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:20:18.640052 litechain-0.1.2/litechain/contrib/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:20:02.000000 litechain-0.1.2/litechain/contrib/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-07-14 08:20:02.000000 litechain-0.1.2/litechain/contrib/utils/open_ai_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:20:18.640052 litechain-0.1.2/litechain/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:20:02.000000 litechain-0.1.2/litechain/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20678 2023-07-14 08:20:02.000000 litechain-0.1.2/litechain/core/chain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:20:18.640052 litechain-0.1.2/litechain/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:20:02.000000 litechain-0.1.2/litechain/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-14 08:20:02.000000 litechain-0.1.2/litechain/utils/async_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-07-14 08:20:02.000000 litechain-0.1.2/litechain/utils/chain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:20:18.636052 litechain-0.1.2/litechain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-07-14 08:20:18.000000 litechain-0.1.2/litechain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-14 08:20:18.000000 litechain-0.1.2/litechain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 08:20:18.000000 litechain-0.1.2/litechain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-14 08:20:18.000000 litechain-0.1.2/litechain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-14 08:20:18.000000 litechain-0.1.2/litechain.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-14 08:20:02.000000 litechain-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 08:20:18.640052 litechain-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-14 08:20:02.000000 litechain-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 08:20:18.640052 litechain-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 08:20:02.000000 litechain-0.1.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:02:44.139620 litechain-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-19 10:02:32.000000 litechain-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-19 10:02:32.000000 litechain-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11330 2023-07-19 10:02:44.139620 litechain-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10067 2023-07-19 10:02:32.000000 litechain-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:02:44.139620 litechain-0.1.3/litechain/
+-rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-07-19 10:02:32.000000 litechain-0.1.3/litechain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:02:44.139620 litechain-0.1.3/litechain/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-19 10:02:32.000000 litechain-0.1.3/litechain/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:02:44.139620 litechain-0.1.3/litechain/contrib/llms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 10:02:32.000000 litechain-0.1.3/litechain/contrib/llms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-07-19 10:02:32.000000 litechain-0.1.3/litechain/contrib/llms/gpt4all_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13667 2023-07-19 10:02:32.000000 litechain-0.1.3/litechain/contrib/llms/open_ai.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:02:44.139620 litechain-0.1.3/litechain/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 10:02:32.000000 litechain-0.1.3/litechain/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20737 2023-07-19 10:02:32.000000 litechain-0.1.3/litechain/core/chain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:02:44.139620 litechain-0.1.3/litechain/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 10:02:32.000000 litechain-0.1.3/litechain/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-19 10:02:32.000000 litechain-0.1.3/litechain/utils/async_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-07-19 10:02:32.000000 litechain-0.1.3/litechain/utils/chain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:02:44.139620 litechain-0.1.3/litechain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11330 2023-07-19 10:02:44.000000 litechain-0.1.3/litechain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-19 10:02:44.000000 litechain-0.1.3/litechain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 10:02:44.000000 litechain-0.1.3/litechain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-19 10:02:44.000000 litechain-0.1.3/litechain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-19 10:02:44.000000 litechain-0.1.3/litechain.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-19 10:02:32.000000 litechain-0.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 10:02:44.139620 litechain-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-19 10:02:32.000000 litechain-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:02:44.139620 litechain-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 10:02:32.000000 litechain-0.1.3/tests/__init__.py
```

### Comparing `litechain-0.1.2/LICENSE` & `litechain-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `litechain-0.1.2/PKG-INFO` & `litechain-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litechain
-Version: 0.1.2
+Version: 0.1.3
 Summary: Build robust LLM applications with true composability 🔗
 Home-page: https://github.com/rogeriochaves/litechain
 Author: Rogerio Chaves
 Author-email: rogeriocfj@gmail.com
 License: MIT
 Project-URL: Documentation, https://rogeriochaves.github.io/litechain/
 Project-URL: Source Code, https://github.com/rogeriochaves/litechain
@@ -25,15 +25,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🪽🔗 LiteChain
 
-[![](https://dcbadge.vercel.app/api/server/AmEMWmFG?style=flat)](https://discord.gg/AmEMWmFG)
+[![](https://dcbadge.vercel.app/api/server/48ZM5KkKgw?style=flat)](https://discord.gg/48ZM5KkKgw)
 [![Release Notes](https://img.shields.io/github/release/rogeriochaves/litechain)](https://pypi.org/project/litechain/)
 [![tests](https://github.com/rogeriochaves/litechain/actions/workflows/run_tests.yml/badge.svg)](https://github.com/rogeriochaves/litechain/actions/workflows/run_tests.yml)
 [![docs](https://github.com/rogeriochaves/litechain/actions/workflows/publish_docs.yml/badge.svg)](https://github.com/rogeriochaves/litechain/actions/workflows/publish_docs.yml)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/rogeriochaves/litechain/blob/main/LICENSE)
 
 LiteChain is a lighter alternative to LangChain for building LLMs application, instead of having a massive amount of features and classes, LiteChain focuses on having a single small core, that is easy to learn, easy to adapt, well documented, fully typed and truly composable.
 
@@ -138,15 +138,15 @@
 - Getting started
 - Detailed guides
 - How-to examples
 - Reference
 
 # 👥 Community
 
-[Join our discord](https://discord.gg/AmEMWmFG) community to connect with other LiteChain developers, ask questions, get support, and stay updated with the latest news and announcements.
+[Join our discord](https://discord.gg/48ZM5KkKgw) community to connect with other LiteChain developers, ask questions, get support, and stay updated with the latest news and announcements.
 
 [![Join our Discord community](https://img.shields.io/badge/Join-Discord-7289DA.svg)](https://discord.gg/AmEMWmFG)
 
 # 🚙 Roadmap
 
 - [ ] Add an example for document retrieval using vector search
 - [ ] Add a `filter` function
```

### Comparing `litechain-0.1.2/README.md` & `litechain-0.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # 🪽🔗 LiteChain
 
-[![](https://dcbadge.vercel.app/api/server/AmEMWmFG?style=flat)](https://discord.gg/AmEMWmFG)
+[![](https://dcbadge.vercel.app/api/server/48ZM5KkKgw?style=flat)](https://discord.gg/48ZM5KkKgw)
 [![Release Notes](https://img.shields.io/github/release/rogeriochaves/litechain)](https://pypi.org/project/litechain/)
 [![tests](https://github.com/rogeriochaves/litechain/actions/workflows/run_tests.yml/badge.svg)](https://github.com/rogeriochaves/litechain/actions/workflows/run_tests.yml)
 [![docs](https://github.com/rogeriochaves/litechain/actions/workflows/publish_docs.yml/badge.svg)](https://github.com/rogeriochaves/litechain/actions/workflows/publish_docs.yml)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/rogeriochaves/litechain/blob/main/LICENSE)
 
 LiteChain is a lighter alternative to LangChain for building LLMs application, instead of having a massive amount of features and classes, LiteChain focuses on having a single small core, that is easy to learn, easy to adapt, well documented, fully typed and truly composable.
 
@@ -109,15 +109,15 @@
 - Getting started
 - Detailed guides
 - How-to examples
 - Reference
 
 # 👥 Community
 
-[Join our discord](https://discord.gg/AmEMWmFG) community to connect with other LiteChain developers, ask questions, get support, and stay updated with the latest news and announcements.
+[Join our discord](https://discord.gg/48ZM5KkKgw) community to connect with other LiteChain developers, ask questions, get support, and stay updated with the latest news and announcements.
 
 [![Join our Discord community](https://img.shields.io/badge/Join-Discord-7289DA.svg)](https://discord.gg/AmEMWmFG)
 
 # 🚙 Roadmap
 
 - [ ] Add an example for document retrieval using vector search
 - [ ] Add a `filter` function
```

### Comparing `litechain-0.1.2/litechain/__init__.py` & `litechain-0.1.3/litechain/__init__.py`

 * *Files identical despite different names*

### Comparing `litechain-0.1.2/litechain/contrib/__init__.py` & `litechain-0.1.3/litechain/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `litechain-0.1.2/litechain/contrib/llms/gpt4all_chain.py` & `litechain-0.1.3/litechain/contrib/llms/gpt4all_chain.py`

 * *Files identical despite different names*

### Comparing `litechain-0.1.2/litechain/contrib/llms/open_ai.py` & `litechain-0.1.3/litechain/contrib/llms/open_ai.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import asyncio
 from dataclasses import dataclass
-import json
 from typing import (
     Any,
     AsyncGenerator,
     Callable,
     Dict,
     List,
     Literal,
@@ -12,15 +11,14 @@
     TypeVar,
     Union,
     cast,
 )
 
 import openai
 from colorama import Fore
-from litechain.contrib.utils.open_ai_functions import OpenAIFunction, py2gpt
 
 from litechain.core.chain import Chain, ChainOutput
 
 T = TypeVar("T")
 U = TypeVar("U")
 V = TypeVar("V")
 
@@ -116,20 +114,14 @@
     name: Optional[str] = None
 
     def to_dict(self):
         return {k: v for k, v in self.__dict__.items() if v is not None}
 
 
 @dataclass
-class _OpenAIFunctionCall:
-    name: str
-    arguments: str
-
-
-@dataclass
 class OpenAIChatDelta:
     """
     OpenAIChatDelta is a data class that represents the output of an `OpenAIChatChain`.
 
     Attributes
     ----------
     role : Optional[Literal["assistant", "function"]]
@@ -147,32 +139,24 @@
     """
 
     role: Optional[Literal["assistant", "function"]]
     content: str
     name: Optional[str] = None
 
     def __chain_debug__(self):
+        name = ""
+        if self.name:
+            name = f" {self.name}"
         if self.role is not None:
-            print(f"{Fore.YELLOW}{self.role.capitalize()}:{Fore.RESET} ", end="")
-        if self.role == "function":
-            arguments = json.loads(self.content)
-            stringified_keywords_list = ", ".join(
-                [f"{k}={repr(v)}" for k, v in arguments.items()]
-            )
-            print(
-                f"{self.name}({stringified_keywords_list})",
-                end="",
-                flush=True,
-            )
-        else:
-            print(
-                self.content,
-                end="",
-                flush=True,
-            )
+            print(f"{Fore.YELLOW}{self.role.capitalize()}{name}:{Fore.RESET} ", end="")
+        print(
+            self.content,
+            end="",
+            flush=True,
+        )
 
 
 class OpenAIChatChain(Chain[T, U]):
     """
     `OpenAIChatChain` gives you access to the more powerful LLMs from OpenAI, like `gpt-3.5-turbo` and `gpt-4`, they are structured in a chat format with roles.
 
     The `OpenAIChatChain` takes a lambda function that should return a list of `OpenAIChatMessage` for the assistant to reply, it is stateless, so it doesn't keep
@@ -210,59 +194,69 @@
     ...     ).map(lambda delta: delta.content)
     ...
     ...     return await join_final_output(recipe_chain("instant noodles"))
     ...
     >>> asyncio.run(example()) # doctest:+SKIP
     "Of course! Here's a simple and delicious recipe"
 
-    You can also pass python functions to be called by the model, LiteChain will convert those functions to OpenAI function schema and call it back automatically.
-    The functions you pass must have type signatures and doctypes including for the parameters, otherwise you will get a runtime error. The docs are important because
-    this is how you tell the model why should it use that function, and what each parameter means, for better results.
+    You can also pass OpenAI function schemas in the `function` argument with all parameter definitions, the model may then produce a `function` role `OpenAIChatDelta`,
+    using your function, with the `content` field as a json which you can parse to call an actual function.
 
-    The function you pass may return either a static value or an `AsyncGenerator`, which means you can call other chains from it. Take a look [at our guide](https://rogeriochaves.github.io/litechain/docs/llms/open_ai_functions)
-    to learn more about OpenAI function calls in LiteChain.
+    Take a look [at our guide](https://rogeriochaves.github.io/litechain/docs/llms/open_ai_functions) to learn more about OpenAI function calls in LiteChain.
 
     Function Call Example
     ---------------------
 
     >>> from litechain import Chain, collect_final_output
     >>> from litechain.contrib import OpenAIChatChain, OpenAIChatMessage, OpenAIChatDelta
     >>> from typing import Literal, Union, Dict
     >>> import asyncio
     ...
     >>> async def example():
     ...     def get_current_weather(
     ...         location: str, format: Literal["celsius", "fahrenheit"] = "celsius"
     ...     ) -> Dict[str, str]:
-    ...         \"""
-    ...         Gets the current weather in a given location, use this function for any questions related to the weather
-    ...
-    ...         Parameters
-    ...         ----------
-    ...         location
-    ...             The city to get the weather, e.g. San Francisco. Guess the location from user messages
-    ...
-    ...         format
-    ...             A string with the full content of what the given role said
-    ...         \"""
-    ...
     ...         return {
     ...             "location": location,
     ...             "forecast": "sunny",
     ...             "temperature": "25 C" if format == "celsius" else "77 F",
     ...         }
     ...
-    ...     chain = OpenAIChatChain[str, Union[OpenAIChatDelta, Dict[str, str]]](
+    ...     chain : Chain[str, Union[OpenAIChatDelta, Dict[str, str]]] = OpenAIChatChain[str, Union[OpenAIChatDelta, Dict[str, str]]](
     ...         "WeatherChain",
     ...         lambda user_input: [
     ...             OpenAIChatMessage(role="user", content=user_input),
     ...         ],
     ...         model="gpt-3.5-turbo",
-    ...         functions=[get_current_weather],
+    ...         functions=[
+    ...             {
+    ...                 "name": "get_current_weather",
+    ...                 "description": "Gets the current weather in a given location, use this function for any questions related to the weather",
+    ...                 "parameters": {
+    ...                     "type": "object",
+    ...                     "properties": {
+    ...                         "location": {
+    ...                             "description": "The city to get the weather, e.g. San Francisco. Guess the location from user messages",
+    ...                             "type": "string",
+    ...                         },
+    ...                         "format": {
+    ...                             "description": "A string with the full content of what the given role said",
+    ...                             "type": "string",
+    ...                             "enum": ("celsius", "fahrenheit"),
+    ...                         },
+    ...                     },
+    ...                 },
+    ...                 "required": ["location"],
+    ...             }
+    ...         ],
     ...         temperature=0,
+    ...     ).map(
+    ...         lambda delta: get_current_weather(**json.loads(delta.content))
+    ...         if delta.role == "function" and delta.name == "get_current_weather"
+    ...         else delta
     ...     )
     ...
     ...     return await collect_final_output(chain("how is the weather today in Rio de Janeiro?"))
     ...
     >>> asyncio.run(example()) # doctest:+SKIP
     [{'location': 'Rio de Janeiro', 'forecast': 'sunny', 'temperature': '25 C'}]
 
@@ -272,50 +266,45 @@
         self: "OpenAIChatChain[T, Union[OpenAIChatDelta, V]]",
         name: str,
         call: Callable[
             [T],
             List[OpenAIChatMessage],
         ],
         model: str,
-        functions: Union[
-            Optional[List[Callable[..., AsyncGenerator[ChainOutput[V, Any], Any]]]],
-            Optional[List[Callable[..., AsyncGenerator[V, Any]]]],
-            Optional[List[Callable[..., V]]],
-        ] = cast(List[Callable[..., OpenAIChatDelta]], None),
+        functions: Optional[List[Dict[str, Any]]] = None,
         function_call: Optional[Union[Literal["none", "auto"], str]] = None,
         temperature: Optional[float] = 0,
         max_tokens: Optional[int] = None,
     ) -> None:
         self.name = name
-        name_to_function, openai_functions = self._parse_functions(functions)
 
         async def chat_completion(
             messages: List[OpenAIChatMessage],
         ) -> AsyncGenerator[ChainOutput[Union[OpenAIChatDelta, V], Any], Any]:
             loop = asyncio.get_event_loop()
 
             def get_completions():
                 function_kwargs = {}
                 if functions is not None:
-                    function_kwargs["functions"] = openai_functions
+                    function_kwargs["functions"] = functions
                 if function_call is not None:
                     function_kwargs["function_call"] = function_call
 
                 return openai.ChatCompletion.create(
                     model=model,
                     messages=[m.to_dict() for m in messages],
                     temperature=temperature,
                     stream=True,
                     max_tokens=max_tokens,
                     **function_kwargs,
                 )
 
             completions = await loop.run_in_executor(None, get_completions)
 
-            pending_function_calls: List[_OpenAIFunctionCall] = []
+            pending_function_call: Optional[OpenAIChatDelta] = None
 
             for output in completions:
                 output = cast(dict, output)
                 if "choices" not in output:
                     continue
 
                 if len(output["choices"]) == 0:
@@ -329,83 +318,35 @@
                     role = delta["role"] if "role" in delta else None
                     function_name: Optional[str] = delta["function_call"].get("name")
                     function_arguments: Optional[str] = delta["function_call"].get(
                         "arguments"
                     )
 
                     if function_name is not None:
-                        pending_function_calls = [
-                            _OpenAIFunctionCall(
-                                name=function_name,
-                                arguments=function_arguments or "",
-                            )
-                        ]
+                        pending_function_call = OpenAIChatDelta(
+                            role="function",
+                            name=function_name,
+                            content=function_arguments or "",
+                        )
                     elif (
-                        len(pending_function_calls) > 0
+                        pending_function_call is not None
                         and function_arguments is not None
                     ):
-                        pending_function_calls[-1].arguments += function_arguments
+                        pending_function_call.content += function_arguments
                 elif "content" in output["choices"][0]["delta"]:
                     delta = output["choices"][0]["delta"]
                     role = delta["role"] if "role" in delta else None
                     yield self._output_wrap(
                         OpenAIChatDelta(
                             role=role,
                             content=delta["content"],
                         )
                     )
                 else:
-                    async for value in self._run_pending_function_call(
-                        name_to_function, pending_function_calls
-                    ):
-                        yield value
-            async for value in self._run_pending_function_call(
-                name_to_function, pending_function_calls
-            ):
-                yield value
+                    if pending_function_call:
+                        yield self._output_wrap(pending_function_call)
+                        pending_function_call = None
+            if pending_function_call:
+                yield self._output_wrap(pending_function_call)
+                pending_function_call = None
 
         self._call = lambda input: chat_completion(call(input))
-
-    def _parse_functions(self, functions: Optional[List[Callable]]):
-        name_to_function: Dict[str, Callable] = dict()
-        openai_functions: List[OpenAIFunction] = []
-        if functions is not None:
-            for fn in functions:
-                try:
-                    openai_functions = [py2gpt(fn) for fn in functions]
-                except ValueError as e:
-                    raise ValueError(
-                        f"The function {fn} that you passed in the 'functions' argument when creating a OpenAIChatChain could not be converted to a valid OpenAI function: {str(e)}"
-                    )
-            name_to_function = dict(
-                [
-                    (openai_fn["name"], fn)
-                    for fn, openai_fn in zip(functions, openai_functions)
-                ]
-            )
-
-        return name_to_function, openai_functions
-
-    async def _run_pending_function_call(
-        self,
-        name_to_function: Dict[str, Callable],
-        pending_function_calls: List[_OpenAIFunctionCall],
-    ) -> AsyncGenerator[ChainOutput, None]:
-        for function_call in pending_function_calls:
-            function_to_call = name_to_function[function_call.name]
-            arguments = json.loads(function_call.arguments)
-            output_chain_name = f"{self.name}@function_call->{function_call.name}"
-
-            yield self._output_wrap(
-                OpenAIChatDelta(
-                    role="function",
-                    name=function_call.name,
-                    content=function_call.arguments,
-                ),
-                final=False,
-            )
-
-            result = function_to_call(**arguments)
-            wrapped = self._wrap(result, name=output_chain_name)
-            async for output in wrapped:
-                yield output
-        pending_function_calls.clear()
```

### Comparing `litechain-0.1.2/litechain/core/chain.py` & `litechain-0.1.3/litechain/core/chain.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,15 +176,18 @@
                     prev_len_values = len(values)
                     yield cast(ChainOutput[V, Union[U, V]], fn(values[-1]))
 
         return Chain[T, V](f"{self.name}@map", lambda input: map(input))
 
     def and_then(
         self,
-        next: Callable[[Iterable[U]], Union[AsyncGenerator[ChainOutput[V, W], Any], V]],
+        next: Callable[
+            [Iterable[U]],
+            Union[AsyncGenerator[ChainOutput[V, W], Any], AsyncGenerator[V, Any], V],
+        ],
     ) -> "Chain[T, V]":
         """
         Processes the output of the current chain through a transformation function or another chain.
 
         Unlike the map method, which applies transformations to outputs as they arrive,
         the and_then method first collects all the outputs and then passes them to the transformation function or the next chain.
         This method is blocking and will wait for the entire chain to be processed before applying the transformation.
```

### Comparing `litechain-0.1.2/litechain/utils/async_generator.py` & `litechain-0.1.3/litechain/utils/async_generator.py`

 * *Files identical despite different names*

### Comparing `litechain-0.1.2/litechain/utils/chain.py` & `litechain-0.1.3/litechain/utils/chain.py`

 * *Files identical despite different names*

### Comparing `litechain-0.1.2/litechain.egg-info/PKG-INFO` & `litechain-0.1.3/litechain.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litechain
-Version: 0.1.2
+Version: 0.1.3
 Summary: Build robust LLM applications with true composability 🔗
 Home-page: https://github.com/rogeriochaves/litechain
 Author: Rogerio Chaves
 Author-email: rogeriocfj@gmail.com
 License: MIT
 Project-URL: Documentation, https://rogeriochaves.github.io/litechain/
 Project-URL: Source Code, https://github.com/rogeriochaves/litechain
@@ -25,15 +25,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🪽🔗 LiteChain
 
-[![](https://dcbadge.vercel.app/api/server/AmEMWmFG?style=flat)](https://discord.gg/AmEMWmFG)
+[![](https://dcbadge.vercel.app/api/server/48ZM5KkKgw?style=flat)](https://discord.gg/48ZM5KkKgw)
 [![Release Notes](https://img.shields.io/github/release/rogeriochaves/litechain)](https://pypi.org/project/litechain/)
 [![tests](https://github.com/rogeriochaves/litechain/actions/workflows/run_tests.yml/badge.svg)](https://github.com/rogeriochaves/litechain/actions/workflows/run_tests.yml)
 [![docs](https://github.com/rogeriochaves/litechain/actions/workflows/publish_docs.yml/badge.svg)](https://github.com/rogeriochaves/litechain/actions/workflows/publish_docs.yml)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/rogeriochaves/litechain/blob/main/LICENSE)
 
 LiteChain is a lighter alternative to LangChain for building LLMs application, instead of having a massive amount of features and classes, LiteChain focuses on having a single small core, that is easy to learn, easy to adapt, well documented, fully typed and truly composable.
 
@@ -138,15 +138,15 @@
 - Getting started
 - Detailed guides
 - How-to examples
 - Reference
 
 # 👥 Community
 
-[Join our discord](https://discord.gg/AmEMWmFG) community to connect with other LiteChain developers, ask questions, get support, and stay updated with the latest news and announcements.
+[Join our discord](https://discord.gg/48ZM5KkKgw) community to connect with other LiteChain developers, ask questions, get support, and stay updated with the latest news and announcements.
 
 [![Join our Discord community](https://img.shields.io/badge/Join-Discord-7289DA.svg)](https://discord.gg/AmEMWmFG)
 
 # 🚙 Roadmap
 
 - [ ] Add an example for document retrieval using vector search
 - [ ] Add a `filter` function
```

### Comparing `litechain-0.1.2/litechain.egg-info/SOURCES.txt` & `litechain-0.1.3/litechain.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -9,15 +9,13 @@
 litechain.egg-info/dependency_links.txt
 litechain.egg-info/requires.txt
 litechain.egg-info/top_level.txt
 litechain/contrib/__init__.py
 litechain/contrib/llms/__init__.py
 litechain/contrib/llms/gpt4all_chain.py
 litechain/contrib/llms/open_ai.py
-litechain/contrib/utils/__init__.py
-litechain/contrib/utils/open_ai_functions.py
 litechain/core/__init__.py
 litechain/core/chain.py
 litechain/utils/__init__.py
 litechain/utils/async_generator.py
 litechain/utils/chain.py
 tests/__init__.py
```

### Comparing `litechain-0.1.2/setup.py` & `litechain-0.1.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = f.read().splitlines()
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="litechain",
-    version="0.1.2",
+    version="0.1.3",
     packages=find_packages(),
     install_requires=requirements,
     author="Rogerio Chaves",
     author_email="rogeriocfj@gmail.com",
     description="Build robust LLM applications with true composability 🔗",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

