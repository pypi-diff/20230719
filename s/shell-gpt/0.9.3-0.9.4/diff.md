# Comparing `tmp/shell_gpt-0.9.3.tar.gz` & `tmp/shell_gpt-0.9.4.tar.gz`

## Comparing `shell_gpt-0.9.3.tar` & `shell_gpt-0.9.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 shell_gpt-0.9.3/LICENSE
--rw-r--r--   0        0        0    20106 2020-02-02 00:00:00.000000 shell_gpt-0.9.3/README.md
--rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 shell_gpt-0.9.3/pyproject.toml
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 shell_gpt-0.9.3/sgpt/__init__.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 shell_gpt-0.9.3/sgpt/__main__.py
--rw-r--r--   0        0        0     6453 2020-02-02 00:00:00.000000 shell_gpt-0.9.3/sgpt/app.py
--rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 shell_gpt-0.9.3/sgpt/cache.py
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 shell_gpt-0.9.3/sgpt/client.py
--rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 shell_gpt-0.9.3/sgpt/config.py
--rw-r--r--   0        0        0     6956 2020-02-02 00:00:00.000000 shell_gpt-0.9.3/sgpt/role.py
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 shell_gpt-0.9.3/sgpt/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shell_gpt-0.9.3/sgpt/handlers/__init__.py
--rw-r--r--   0        0        0     6482 2020-02-02 00:00:00.000000 shell_gpt-0.9.3/sgpt/handlers/chat_handler.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 shell_gpt-0.9.3/sgpt/handlers/default_handler.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 shell_gpt-0.9.3/sgpt/handlers/handler.py
--rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 shell_gpt-0.9.3/sgpt/handlers/repl_handler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shell_gpt-0.9.3/tests/__init__.py
--rw-r--r--   0        0        0    17250 2020-02-02 00:00:00.000000 shell_gpt-0.9.3/tests/test_integration.py
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 shell_gpt-0.9.3/tests/test_unit.py
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 shell_gpt-0.9.3/LICENSE
--rw-r--r--   0        0        0    20106 2020-02-02 00:00:00.000000 shell_gpt-0.9.3/README.md
--rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 shell_gpt-0.9.3/pyproject.toml
--rw-r--r--   0        0        0    22133 2020-02-02 00:00:00.000000 shell_gpt-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 shell_gpt-0.9.4/LICENSE
+-rw-r--r--   0        0        0    22672 2020-02-02 00:00:00.000000 shell_gpt-0.9.4/README.md
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 shell_gpt-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 shell_gpt-0.9.4/sgpt/__init__.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 shell_gpt-0.9.4/sgpt/__main__.py
+-rw-r--r--   0        0        0     6013 2020-02-02 00:00:00.000000 shell_gpt-0.9.4/sgpt/app.py
+-rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 shell_gpt-0.9.4/sgpt/cache.py
+-rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 shell_gpt-0.9.4/sgpt/client.py
+-rw-r--r--   0        0        0     3304 2020-02-02 00:00:00.000000 shell_gpt-0.9.4/sgpt/config.py
+-rw-r--r--   0        0        0     6956 2020-02-02 00:00:00.000000 shell_gpt-0.9.4/sgpt/role.py
+-rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 shell_gpt-0.9.4/sgpt/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shell_gpt-0.9.4/sgpt/handlers/__init__.py
+-rw-r--r--   0        0        0     6482 2020-02-02 00:00:00.000000 shell_gpt-0.9.4/sgpt/handlers/chat_handler.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 shell_gpt-0.9.4/sgpt/handlers/default_handler.py
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 shell_gpt-0.9.4/sgpt/handlers/handler.py
+-rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 shell_gpt-0.9.4/sgpt/handlers/repl_handler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shell_gpt-0.9.4/tests/__init__.py
+-rw-r--r--   0        0        0    17413 2020-02-02 00:00:00.000000 shell_gpt-0.9.4/tests/test_integration.py
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 shell_gpt-0.9.4/tests/test_unit.py
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 shell_gpt-0.9.4/LICENSE
+-rw-r--r--   0        0        0    22672 2020-02-02 00:00:00.000000 shell_gpt-0.9.4/README.md
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 shell_gpt-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0    24755 2020-02-02 00:00:00.000000 shell_gpt-0.9.4/PKG-INFO
```

### Comparing `shell_gpt-0.9.3/LICENSE` & `shell_gpt-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.9.3/README.md` & `shell_gpt-0.9.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ShellGPT
-A command-line productivity tool powered by OpenAI's GPT models. As developers, we can leverage AI capabilities to generate shell commands, code snippets, comments, and documentation, among other things. Forget about cheat sheets and notes, with this tool you can get accurate answers right in your terminal, and you'll probably find yourself reducing your daily Google searches, saving you valuable time and effort. ShellGPT is cross-platform compatible and supports all major operating systems, including Linux, macOS, and Windows with all major shells, such as PowerShell, CMD, Bash, Zsh, Fish, and many others.
+A command-line productivity tool powered by AI large language models (LLM). As developers, we can leverage AI capabilities to generate shell commands, code snippets, comments, and documentation, among other things. Forget about cheat sheets and notes, with this tool you can get accurate answers right in your terminal, and you'll probably find yourself reducing your daily Google searches, saving you valuable time and effort. ShellGPT is cross-platform compatible and supports all major operating systems, including Linux, macOS, and Windows with all major shells, such as PowerShell, CMD, Bash, Zsh, Fish, and many others.
 
 https://user-images.githubusercontent.com/16740832/231569156-a3a9f9d4-18b1-4fff-a6e1-6807651aa894.mp4
 
 ## Installation
 ```shell
 pip install shell-gpt
 ```
@@ -130,15 +130,15 @@
 # 4
 # Buzz
 # Fizz
 # ...
 ```
 We can also use pipes to pass input to `sgpt`:
 ```shell
-cat fizz_buzz.py | python -m sgpt --code "Generate comments for each line of my code"
+cat fizz_buzz.py | sgpt --code "Generate comments for each line of my code"
 ```
 ```python
 # Loop through numbers 1 to 100
 for i in range(1, 101):
     # Check if number is divisible by both 3 and 5
     if i % 3 == 0 and i % 5 == 0:
         # Print "FizzBuzz" if number is divisible by both 3 and 5
@@ -152,15 +152,38 @@
         # Print "Buzz" if number is divisible by 5
         print("Buzz")
     # If number is not divisible by 3 or 5, print the number itself
     else:
         print(i)
 ```
 
-### Chat
+### Conversational Modes - Overview
+
+Often it is important to preserve and recall a conversation and this is kept track of locally. `sgpt` creates conversational dialogue with each llm completion requested. The dialogue can develop one-by-one (chat mode) or interactively, in a REPL loop (REPL mode). Both ways rely on the same underlying object, called a chat session. The session is located at the [configurable](#runtime-configuration-file) `CHAT_CACHE_PATH`.
+
+### Listing and Showing Chat Sessions 
+
+Dialogues had in both REPL and chat mode are saved as chat sessions.
+
+To list all the sessions from either conversational mode, use the `--list-chats` option:
+```shell
+sgpt --list-chats
+# .../shell_gpt/chat_cache/number
+# .../shell_gpt/chat_cache/python_request
+```
+To show all the messages related to a specific conversation, use the `--show-chat` option followed by the session name:
+```shell
+sgpt --show-chat number
+# user: please remember my favorite number: 4
+# assistant: I will remember that your favorite number is 4.
+# user: what would be my favorite number + 4?
+# assistant: Your favorite number is 4, so if we add 4 to it, the result would be 8.
+```
+
+### Chat Mode
 To start a chat session, use the `--chat` option followed by a unique session name and a prompt. You can also use "temp" as a session name to start a temporary chat session.
 ```shell
 sgpt --chat number "please remember my favorite number: 4"
 # -> I will remember that your favorite number is 4.
 sgpt --chat number "what would be my favorite number + 4?"
 # -> Your favorite number is 4, so if we add 4 to it, the result would be 8.
 ```
@@ -196,15 +219,15 @@
 # -> ls | sort
 sgpt --chat sh "Concatenate them using FFMPEG"
 # -> ffmpeg -i "concat:$(ls | sort | tr '\n' '|')" -codec copy output.mp4
 sgpt --chat sh "Convert the resulting file into an MP3"
 # -> ffmpeg -i output.mp4 -vn -acodec libmp3lame -ac 2 -ab 160k -ar 48000 final_output.mp3
 ```
 
-### REPL
+### REPL Mode
 There is very handy REPL (read–eval–print loop) mode, which allows you to interactively chat with GPT models. To start a chat session in REPL mode, use the `--repl` option followed by a unique session name. You can also use "temp" as a session name to start a temporary REPL session. Note that `--chat` and `--repl` are using same chat sessions, so you can use `--chat` to start a chat session and then use `--repl` to continue the conversation in REPL mode. REPL mode will also show history of your conversation in the beginning.
 
 <p align="center">
   <img src="https://s10.gifyu.com/images/repl-demo.gif" alt="gif">
 </p>
 
 ```text
@@ -238,30 +261,39 @@
 print(response.text)
 >>> Change port to 443
 import requests
 response = requests.get('https://localhost:443')
 print(response.text)
 ```
 
-### Chat sessions
-To list all the current chat sessions, use the `--list-chats` option:
-```shell
-sgpt --list-chats
-# .../shell_gpt/chat_cache/number
-# .../shell_gpt/chat_cache/python_request
-```
-To show all the messages related to a specific chat session, use the `--show-chat` option followed by the session name:
-```shell
-sgpt --show-chat number
-# user: please remember my favorite number: 4
-# assistant: I will remember that your favorite number is 4.
-# user: what would be my favorite number + 4?
-# assistant: Your favorite number is 4, so if we add 4 to it, the result would be 8.
+### Picking up on a chat mode conversation with REPL mode
+
+```text
+sgpt --repl number
+───── Chat History──────
+user: ###
+Role name: default
+You are Command Line App ShellGPT, a programming and system administration assistant.
+You are managing Darwin/MacOS 13.3.1 operating system with zsh shell.
+Provide only plain text without Markdown formatting.
+Do not show any warnings or information regarding your capabilities.
+If you need to store any data, assume it will be stored in the chat.
+
+Request: please remember my favorite number: 4
+###
+assistant: Sure, I have stored your favorite number as 4.
+user: what would be my favorite number raised to the power of 4
+assistant: Your favorite number raised to the power of 4 would be 256.
+────────────────────────────────────────────────────────
+Entering REPL mode, press Ctrl+C to exit.
+>>> What is the sum of my favorite number and your previous response?
+The sum of your favorite number (4) and my previous response (256) would be 260.
 ```
 
+
 ### Roles
 ShellGPT allows you to create custom roles, which can be utilized to generate code, shell commands, or to fulfill your specific needs. To create a new role, use the `--create-role` option followed by the role name. You will be prompted to provide a description for the role, along with other details. This will create a JSON file in `~/.config/shell_gpt/roles` with the role name. Inside this directory, you can also edit default `sgpt` roles, such as **shell**, **code**, and **default**. Use the `--list-roles` option to list all available roles, and the `--show-role` option to display the details of a specific role. Here's an example of a custom role:
 ```shell
 sgpt --create-role json
 # Enter role description: You are JSON generator, provide only valid json as response.
 # Enter expecting result, e.g. answer, code, shell command, etc.: json
 sgpt --role json "random: user, password, email, address"
@@ -309,26 +341,28 @@
 DEFAULT_MODEL=gpt-3.5-turbo
 # Default color for OpenAI completions.
 DEFAULT_COLOR=magenta
 # Force use system role messages (not recommended).
 SYSTEM_ROLES=false
 # When in --shell mode, default to "Y" for no input.
 DEFAULT_EXECUTE_SHELL_CMD=false
+# Disable streaming of responses
+DISABLE_STREAMING=false
 ```
 Possible options for `DEFAULT_COLOR`: black, red, green, yellow, blue, magenta, cyan, white, bright_black, bright_red, bright_green, bright_yellow, bright_blue, bright_magenta, bright_cyan, bright_white.
 
 Switch `SYSTEM_ROLES` to force use [system roles](https://help.openai.com/en/articles/7042661-chatgpt-api-transition-guide) messages, this is not recommended, since it doesn't perform well with current GPT models.
 
 ### Full list of arguments
 ```text
 ╭─ Arguments ─────────────────────────────────────────────────────────────────────────────────────────────────╮
 │   prompt      [PROMPT]  The prompt to generate completions for.                                             │
 ╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Options ───────────────────────────────────────────────────────────────────────────────────────────────────╮
-│ --model    [gpt-4|gpt-4-32k|gpt-3.5|gpt-3.5-16k]    OpenAI GPT model to use. [default: gpt-3.5-turbo]       │
+│ --model            TEXT                             OpenAI GPT model to use. [default: gpt-3.5-turbo]       │
 │ --temperature      FLOAT RANGE [0.0<=x<=2.0]        Randomness of generated output. [default: 0.1]          │
 │ --top-probability  FLOAT RANGE [0.1<=x<=1.0]        Limits highest probable tokens (words). [default: 1.0]  │
 │ --editor                                            Open $EDITOR to provide a prompt. [default: no-editor]  │
 │ --cache                                             Cache completion results. [default: cache]              │
 │ --help                                              Show this message and exit.                             │
 ╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Assistance Options ────────────────────────────────────────────────────────────────────────────────────────╮
@@ -346,14 +380,17 @@
 │ --role         TEXT  System role for GPT model. [default: None]                                             │
 │ --create-role  TEXT  Create role. [default: None]                                                           │
 │ --show-role    TEXT  Show role. [default: None]                                                             │
 │ --list-roles         List roles. [default: no-list-roles]                                                   │
 ╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 
+## LocalAI
+By default, ShellGPT leverages OpenAI's large language models. However, it also provides the flexibility to use locally hosted models, which can be a cost-effective alternative. To use local models, you will need to run your own API server. You can accomplish this by using [LocalAI](https://github.com/go-skynet/LocalAI), a self-hosted, OpenAI-compatible API. Setting up LocalAI allows you to run language models on your own hardware, potentially without the need for an internet connection, depending on your usage. To set up your LocalAI, please follow this comprehensive [guide](https://github.com/TheR1D/shell_gpt/wiki/LocalAI). Remember that the performance of your local models may depend on the specifications of your hardware and the specific language model you choose to deploy.
+
 ## Docker
 Run the container using the `OPENAI_API_KEY` environment variable, and a docker volume to store cache:
 ```shell
 docker run --rm \
            --env OPENAI_API_KEY="your OPENAI API key" \
            --volume gpt-cache:/tmp/shell_gpt \
        ghcr.io/ther1d/shell_gpt --chat rainbow "what are the colors of a rainbow"
```

### Comparing `shell_gpt-0.9.3/pyproject.toml` & `shell_gpt-0.9.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 test = [
     "pytest >= 7.2.2, < 8.0.0",
     "requests-mock[fixture] >= 1.10.0, < 2.0.0",
     "isort >= 5.12.0, < 6.0.0",
     "black == 23.1.0",
     "mypy == 1.1.1",
     "types-requests == 2.28.11.17",
+    "codespell  >= 2.2.5, < 3.0.0"
 ]
 dev = [
     "ruff == 0.0.256",
     "pre-commit >= 3.1.1, < 4.0.0",
 ]
 
 [tool.hatch.version]
@@ -89,7 +90,11 @@
     "B",  # flake8-bugbear.
 ]
 ignore = [
     "E501",  # line too long, handled by black.
     "C901",  # too complex.
     "B008",  # do not perform function calls in argument defaults.
 ]
+
+[tool.codespell]
+skip = '.git,venv'
+# ignore-words-list = ''
```

### Comparing `shell_gpt-0.9.3/sgpt/app.py` & `shell_gpt-0.9.4/sgpt/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,32 @@
-"""
-This module provides a simple interface for OpenAI API using Typer
-as the command line interface. It supports different modes of output including
-shell commands and code, and allows users to specify the desired OpenAI model
-and length and other options of the output. Additionally, it supports executing
-shell commands directly from the interface.
-"""
 # To allow users to use arrow keys in the REPL.
 import readline  # noqa: F401
 import sys
 
 import typer
 from click import BadArgumentUsage, MissingParameter
 from click.types import Choice
 
 from sgpt.config import cfg
 from sgpt.handlers.chat_handler import ChatHandler
 from sgpt.handlers.default_handler import DefaultHandler
 from sgpt.handlers.repl_handler import ReplHandler
 from sgpt.role import DefaultRoles, SystemRole
-from sgpt.utils import (
-    ModelOptions,
-    get_edited_prompt,
-    install_shell_integration,
-    run_command,
-)
+from sgpt.utils import get_edited_prompt, install_shell_integration, run_command
 
 
 def main(
     prompt: str = typer.Argument(
         None,
         show_default=False,
         help="The prompt to generate completions for.",
     ),
-    model: ModelOptions = typer.Option(
-        ModelOptions(cfg.get("DEFAULT_MODEL")).value,
-        help="OpenAI GPT model to use.",
+    model: str = typer.Option(
+        cfg.get("DEFAULT_MODEL"),
+        help="Large language model to use.",
     ),
     temperature: float = typer.Option(
         0.1,
         min=0.0,
         max=2.0,
         help="Randomness of generated output.",
     ),
@@ -155,34 +143,34 @@
         else SystemRole.get(role)
     )
 
     if repl:
         # Will be in infinite loop here until user exits with Ctrl+C.
         ReplHandler(repl, role_class).handle(
             prompt,
-            model=model.value,
+            model=model,
             temperature=temperature,
             top_probability=top_probability,
             chat_id=repl,
             caching=cache,
         )
 
     if chat:
         full_completion = ChatHandler(chat, role_class).handle(
             prompt,
-            model=model.value,
+            model=model,
             temperature=temperature,
             top_probability=top_probability,
             chat_id=chat,
             caching=cache,
         )
     else:
         full_completion = DefaultHandler(role_class).handle(
             prompt,
-            model=model.value,
+            model=model,
             temperature=temperature,
             top_probability=top_probability,
             caching=cache,
         )
 
     while shell and not stdin_passed:
         option = typer.prompt(
@@ -194,15 +182,15 @@
         )
         if option in ("e", "y"):
             # "y" option is for keeping compatibility with old version.
             run_command(full_completion)
         elif option == "d":
             DefaultHandler(DefaultRoles.DESCRIBE_SHELL.get_role()).handle(
                 full_completion,
-                model=model.value,
+                model=model,
                 temperature=temperature,
                 top_probability=top_probability,
                 caching=cache,
             )
             continue
         break
```

### Comparing `shell_gpt-0.9.3/sgpt/cache.py` & `shell_gpt-0.9.4/sgpt/cache.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.9.3/sgpt/client.py` & `shell_gpt-0.9.4/sgpt/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from .cache import Cache
 from .config import cfg
 
 CACHE_LENGTH = int(cfg.get("CACHE_LENGTH"))
 CACHE_PATH = Path(cfg.get("CACHE_PATH"))
 REQUEST_TIMEOUT = int(cfg.get("REQUEST_TIMEOUT"))
+DISABLE_STREAMING = str(cfg.get("DISABLE_STREAMING"))
 
 
 class OpenAIClient:
     cache = Cache(CACHE_LENGTH, CACHE_PATH)
 
     def __init__(self, api_host: str, api_key: str) -> None:
         self.__api_key = api_key
@@ -33,36 +34,41 @@
 
         :param messages: List of messages {"role": user or assistant, "content": message_string}
         :param model: String gpt-3.5-turbo or gpt-3.5-turbo-0301
         :param temperature: Float in 0.0 - 2.0 range.
         :param top_probability: Float in 0.0 - 1.0 range.
         :return: Response body JSON.
         """
+        stream = DISABLE_STREAMING == "false"
         data = {
             "messages": messages,
             "model": model,
             "temperature": temperature,
             "top_p": top_probability,
-            "stream": True,
+            "stream": stream,
         }
         endpoint = f"{self.api_host}/v1/chat/completions"
         response = requests.post(
             endpoint,
             # Hide API key from Rich traceback.
             headers={
                 "Content-Type": "application/json",
                 "Authorization": f"Bearer {self.__api_key}",
             },
             json=data,
             timeout=REQUEST_TIMEOUT,
-            stream=True,
+            stream=stream,
         )
         response.raise_for_status()
         # TODO: Optimise.
         # https://github.com/openai/openai-python/blob/237448dc072a2c062698da3f9f512fae38300c1c/openai/api_requestor.py#L98
+        if not stream:
+            data = response.json()
+            yield data["choices"][0]["message"]["content"]  # type: ignore
+            return
         for line in response.iter_lines():
             data = line.lstrip(b"data: ").decode("utf-8")
             if data == "[DONE]":  # type: ignore
                 break
             if not data:
                 continue
             data = json.loads(data)  # type: ignore
```

### Comparing `shell_gpt-0.9.3/sgpt/config.py` & `shell_gpt-0.9.4/sgpt/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 from getpass import getpass
 from pathlib import Path
 from tempfile import gettempdir
 from typing import Any
 
 from click import UsageError
 
-from .utils import ModelOptions
-
 CONFIG_FOLDER = os.path.expanduser("~/.config")
 SHELL_GPT_CONFIG_FOLDER = Path(CONFIG_FOLDER) / "shell_gpt"
 SHELL_GPT_CONFIG_PATH = SHELL_GPT_CONFIG_FOLDER / ".sgptrc"
 ROLE_STORAGE_PATH = SHELL_GPT_CONFIG_FOLDER / "roles"
 CHAT_CACHE_PATH = Path(gettempdir()) / "chat_cache"
 CACHE_PATH = Path(gettempdir()) / "cache"
 
@@ -19,20 +17,21 @@
 DEFAULT_CONFIG = {
     # TODO: Refactor it to CHAT_STORAGE_PATH.
     "CHAT_CACHE_PATH": os.getenv("CHAT_CACHE_PATH", str(CHAT_CACHE_PATH)),
     "CACHE_PATH": os.getenv("CACHE_PATH", str(CACHE_PATH)),
     "CHAT_CACHE_LENGTH": int(os.getenv("CHAT_CACHE_LENGTH", "100")),
     "CACHE_LENGTH": int(os.getenv("CHAT_CACHE_LENGTH", "100")),
     "REQUEST_TIMEOUT": int(os.getenv("REQUEST_TIMEOUT", "60")),
-    "DEFAULT_MODEL": os.getenv("DEFAULT_MODEL", ModelOptions.GPT35TURBO.value),
+    "DEFAULT_MODEL": os.getenv("DEFAULT_MODEL", "gpt-3.5-turbo"),
     "OPENAI_API_HOST": os.getenv("OPENAI_API_HOST", "https://api.openai.com"),
     "DEFAULT_COLOR": os.getenv("DEFAULT_COLOR", "magenta"),
     "ROLE_STORAGE_PATH": os.getenv("ROLE_STORAGE_PATH", str(ROLE_STORAGE_PATH)),
     "SYSTEM_ROLES": os.getenv("SYSTEM_ROLES", "false"),
     "DEFAULT_EXECUTE_SHELL_CMD": os.getenv("DEFAULT_EXECUTE_SHELL_CMD", "false"),
+    "DISABLE_STREAMING": os.getenv("DISABLE_STREAMING", "false")
     # New features might add their own config variables here.
 }
 
 
 class Config(dict):  # type: ignore
     def __init__(self, config_path: Path, **defaults: Any):
         self.config_path = config_path
```

### Comparing `shell_gpt-0.9.3/sgpt/role.py` & `shell_gpt-0.9.4/sgpt/role.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.9.3/sgpt/utils.py` & `shell_gpt-0.9.4/sgpt/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,17 @@
 import os
 import platform
 import shlex
-from enum import Enum
 from tempfile import NamedTemporaryFile
 from typing import Any, Callable
 
 import typer
 from click import BadParameter
 
 
-class ModelOptions(str, Enum):
-    """
-    Model endpoint compatibility
-    https://platform.openai.com/docs/models/model-endpoint-compatibility
-    """
-
-    GPT4 = "gpt-4"
-    GPT432k = "gpt-4-32k"
-    GPT35TURBO = "gpt-3.5-turbo"
-    GPT35TURBO16K = "gpt-3.5-turbo-16k"
-
-
 def get_edited_prompt() -> str:
     """
     Opens the user's default editor to let them
     input a prompt, and returns the edited text.
 
     :return: String prompt.
     """
```

### Comparing `shell_gpt-0.9.3/sgpt/handlers/chat_handler.py` & `shell_gpt-0.9.4/sgpt/handlers/chat_handler.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.9.3/sgpt/handlers/default_handler.py` & `shell_gpt-0.9.4/sgpt/handlers/default_handler.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.9.3/sgpt/handlers/repl_handler.py` & `shell_gpt-0.9.4/sgpt/handlers/repl_handler.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.9.3/tests/test_integration.py` & `shell_gpt-0.9.4/tests/test_integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,19 @@
 
 runner = CliRunner()
 app = typer.Typer()
 app.command()(main)
 
 
 class TestShellGpt(TestCase):
+    @classmethod
+    def setUpClass(cls):
+        # Response streaming should be enabled for these tests.
+        assert cfg.get("DISABLE_STREAMING") == "false"
+
     def setUp(self) -> None:
         # Just to not spam the API.
         sleep(1)
 
     @staticmethod
     def get_arguments(prompt, **kwargs):
         arguments = [prompt]
@@ -442,10 +447,10 @@
     def test_shell_command_run_description(self):
         dict_arguments = {
             "prompt": "say hello",
             "--shell": True,
         }
         result = runner.invoke(app, self.get_arguments(**dict_arguments), input="d\n")
         assert result.exit_code == 0
-        # Cant really test it since stdin in disable for --shell flag.
+        # Can't really test it since stdin in disable for --shell flag.
         # for word in ("prints", "hello", "console"):
         #     assert word in result.stdout
```

### Comparing `shell_gpt-0.9.3/tests/test_unit.py` & `shell_gpt-0.9.4/tests/test_unit.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.9.3/PKG-INFO` & `shell_gpt-0.9.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shell_gpt
-Version: 0.9.3
+Version: 0.9.4
 Summary: A command-line productivity tool powered by OpenAI GPT models, will help you accomplish your tasks faster and more efficiently.
 Project-URL: homepage, https://github.com/ther1d/shell_gpt
 Project-URL: repository, https://github.com/ther1d/shell_gpt
 Project-URL: documentation, https://github.com/TheR1D/shell_gpt/blob/main/README.md
 Author-email: Farkhod Sadykov <farkhod@sadykov.dev>
 License-Expression: MIT
 License-File: LICENSE
@@ -31,23 +31,24 @@
 Requires-Dist: rich<14.0.0,>=13.1.0
 Requires-Dist: typer<1.0.0,>=0.7.0
 Provides-Extra: dev
 Requires-Dist: pre-commit<4.0.0,>=3.1.1; extra == 'dev'
 Requires-Dist: ruff==0.0.256; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: black==23.1.0; extra == 'test'
+Requires-Dist: codespell<3.0.0,>=2.2.5; extra == 'test'
 Requires-Dist: isort<6.0.0,>=5.12.0; extra == 'test'
 Requires-Dist: mypy==1.1.1; extra == 'test'
 Requires-Dist: pytest<8.0.0,>=7.2.2; extra == 'test'
 Requires-Dist: requests-mock[fixture]<2.0.0,>=1.10.0; extra == 'test'
 Requires-Dist: types-requests==2.28.11.17; extra == 'test'
 Description-Content-Type: text/markdown
 
 # ShellGPT
-A command-line productivity tool powered by OpenAI's GPT models. As developers, we can leverage AI capabilities to generate shell commands, code snippets, comments, and documentation, among other things. Forget about cheat sheets and notes, with this tool you can get accurate answers right in your terminal, and you'll probably find yourself reducing your daily Google searches, saving you valuable time and effort. ShellGPT is cross-platform compatible and supports all major operating systems, including Linux, macOS, and Windows with all major shells, such as PowerShell, CMD, Bash, Zsh, Fish, and many others.
+A command-line productivity tool powered by AI large language models (LLM). As developers, we can leverage AI capabilities to generate shell commands, code snippets, comments, and documentation, among other things. Forget about cheat sheets and notes, with this tool you can get accurate answers right in your terminal, and you'll probably find yourself reducing your daily Google searches, saving you valuable time and effort. ShellGPT is cross-platform compatible and supports all major operating systems, including Linux, macOS, and Windows with all major shells, such as PowerShell, CMD, Bash, Zsh, Fish, and many others.
 
 https://user-images.githubusercontent.com/16740832/231569156-a3a9f9d4-18b1-4fff-a6e1-6807651aa894.mp4
 
 ## Installation
 ```shell
 pip install shell-gpt
 ```
@@ -174,15 +175,15 @@
 # 4
 # Buzz
 # Fizz
 # ...
 ```
 We can also use pipes to pass input to `sgpt`:
 ```shell
-cat fizz_buzz.py | python -m sgpt --code "Generate comments for each line of my code"
+cat fizz_buzz.py | sgpt --code "Generate comments for each line of my code"
 ```
 ```python
 # Loop through numbers 1 to 100
 for i in range(1, 101):
     # Check if number is divisible by both 3 and 5
     if i % 3 == 0 and i % 5 == 0:
         # Print "FizzBuzz" if number is divisible by both 3 and 5
@@ -196,15 +197,38 @@
         # Print "Buzz" if number is divisible by 5
         print("Buzz")
     # If number is not divisible by 3 or 5, print the number itself
     else:
         print(i)
 ```
 
-### Chat
+### Conversational Modes - Overview
+
+Often it is important to preserve and recall a conversation and this is kept track of locally. `sgpt` creates conversational dialogue with each llm completion requested. The dialogue can develop one-by-one (chat mode) or interactively, in a REPL loop (REPL mode). Both ways rely on the same underlying object, called a chat session. The session is located at the [configurable](#runtime-configuration-file) `CHAT_CACHE_PATH`.
+
+### Listing and Showing Chat Sessions 
+
+Dialogues had in both REPL and chat mode are saved as chat sessions.
+
+To list all the sessions from either conversational mode, use the `--list-chats` option:
+```shell
+sgpt --list-chats
+# .../shell_gpt/chat_cache/number
+# .../shell_gpt/chat_cache/python_request
+```
+To show all the messages related to a specific conversation, use the `--show-chat` option followed by the session name:
+```shell
+sgpt --show-chat number
+# user: please remember my favorite number: 4
+# assistant: I will remember that your favorite number is 4.
+# user: what would be my favorite number + 4?
+# assistant: Your favorite number is 4, so if we add 4 to it, the result would be 8.
+```
+
+### Chat Mode
 To start a chat session, use the `--chat` option followed by a unique session name and a prompt. You can also use "temp" as a session name to start a temporary chat session.
 ```shell
 sgpt --chat number "please remember my favorite number: 4"
 # -> I will remember that your favorite number is 4.
 sgpt --chat number "what would be my favorite number + 4?"
 # -> Your favorite number is 4, so if we add 4 to it, the result would be 8.
 ```
@@ -240,15 +264,15 @@
 # -> ls | sort
 sgpt --chat sh "Concatenate them using FFMPEG"
 # -> ffmpeg -i "concat:$(ls | sort | tr '\n' '|')" -codec copy output.mp4
 sgpt --chat sh "Convert the resulting file into an MP3"
 # -> ffmpeg -i output.mp4 -vn -acodec libmp3lame -ac 2 -ab 160k -ar 48000 final_output.mp3
 ```
 
-### REPL
+### REPL Mode
 There is very handy REPL (read–eval–print loop) mode, which allows you to interactively chat with GPT models. To start a chat session in REPL mode, use the `--repl` option followed by a unique session name. You can also use "temp" as a session name to start a temporary REPL session. Note that `--chat` and `--repl` are using same chat sessions, so you can use `--chat` to start a chat session and then use `--repl` to continue the conversation in REPL mode. REPL mode will also show history of your conversation in the beginning.
 
 <p align="center">
   <img src="https://s10.gifyu.com/images/repl-demo.gif" alt="gif">
 </p>
 
 ```text
@@ -282,30 +306,39 @@
 print(response.text)
 >>> Change port to 443
 import requests
 response = requests.get('https://localhost:443')
 print(response.text)
 ```
 
-### Chat sessions
-To list all the current chat sessions, use the `--list-chats` option:
-```shell
-sgpt --list-chats
-# .../shell_gpt/chat_cache/number
-# .../shell_gpt/chat_cache/python_request
-```
-To show all the messages related to a specific chat session, use the `--show-chat` option followed by the session name:
-```shell
-sgpt --show-chat number
-# user: please remember my favorite number: 4
-# assistant: I will remember that your favorite number is 4.
-# user: what would be my favorite number + 4?
-# assistant: Your favorite number is 4, so if we add 4 to it, the result would be 8.
+### Picking up on a chat mode conversation with REPL mode
+
+```text
+sgpt --repl number
+───── Chat History──────
+user: ###
+Role name: default
+You are Command Line App ShellGPT, a programming and system administration assistant.
+You are managing Darwin/MacOS 13.3.1 operating system with zsh shell.
+Provide only plain text without Markdown formatting.
+Do not show any warnings or information regarding your capabilities.
+If you need to store any data, assume it will be stored in the chat.
+
+Request: please remember my favorite number: 4
+###
+assistant: Sure, I have stored your favorite number as 4.
+user: what would be my favorite number raised to the power of 4
+assistant: Your favorite number raised to the power of 4 would be 256.
+────────────────────────────────────────────────────────
+Entering REPL mode, press Ctrl+C to exit.
+>>> What is the sum of my favorite number and your previous response?
+The sum of your favorite number (4) and my previous response (256) would be 260.
 ```
 
+
 ### Roles
 ShellGPT allows you to create custom roles, which can be utilized to generate code, shell commands, or to fulfill your specific needs. To create a new role, use the `--create-role` option followed by the role name. You will be prompted to provide a description for the role, along with other details. This will create a JSON file in `~/.config/shell_gpt/roles` with the role name. Inside this directory, you can also edit default `sgpt` roles, such as **shell**, **code**, and **default**. Use the `--list-roles` option to list all available roles, and the `--show-role` option to display the details of a specific role. Here's an example of a custom role:
 ```shell
 sgpt --create-role json
 # Enter role description: You are JSON generator, provide only valid json as response.
 # Enter expecting result, e.g. answer, code, shell command, etc.: json
 sgpt --role json "random: user, password, email, address"
@@ -353,26 +386,28 @@
 DEFAULT_MODEL=gpt-3.5-turbo
 # Default color for OpenAI completions.
 DEFAULT_COLOR=magenta
 # Force use system role messages (not recommended).
 SYSTEM_ROLES=false
 # When in --shell mode, default to "Y" for no input.
 DEFAULT_EXECUTE_SHELL_CMD=false
+# Disable streaming of responses
+DISABLE_STREAMING=false
 ```
 Possible options for `DEFAULT_COLOR`: black, red, green, yellow, blue, magenta, cyan, white, bright_black, bright_red, bright_green, bright_yellow, bright_blue, bright_magenta, bright_cyan, bright_white.
 
 Switch `SYSTEM_ROLES` to force use [system roles](https://help.openai.com/en/articles/7042661-chatgpt-api-transition-guide) messages, this is not recommended, since it doesn't perform well with current GPT models.
 
 ### Full list of arguments
 ```text
 ╭─ Arguments ─────────────────────────────────────────────────────────────────────────────────────────────────╮
 │   prompt      [PROMPT]  The prompt to generate completions for.                                             │
 ╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Options ───────────────────────────────────────────────────────────────────────────────────────────────────╮
-│ --model    [gpt-4|gpt-4-32k|gpt-3.5|gpt-3.5-16k]    OpenAI GPT model to use. [default: gpt-3.5-turbo]       │
+│ --model            TEXT                             OpenAI GPT model to use. [default: gpt-3.5-turbo]       │
 │ --temperature      FLOAT RANGE [0.0<=x<=2.0]        Randomness of generated output. [default: 0.1]          │
 │ --top-probability  FLOAT RANGE [0.1<=x<=1.0]        Limits highest probable tokens (words). [default: 1.0]  │
 │ --editor                                            Open $EDITOR to provide a prompt. [default: no-editor]  │
 │ --cache                                             Cache completion results. [default: cache]              │
 │ --help                                              Show this message and exit.                             │
 ╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Assistance Options ────────────────────────────────────────────────────────────────────────────────────────╮
@@ -390,14 +425,17 @@
 │ --role         TEXT  System role for GPT model. [default: None]                                             │
 │ --create-role  TEXT  Create role. [default: None]                                                           │
 │ --show-role    TEXT  Show role. [default: None]                                                             │
 │ --list-roles         List roles. [default: no-list-roles]                                                   │
 ╰─────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
 ```
 
+## LocalAI
+By default, ShellGPT leverages OpenAI's large language models. However, it also provides the flexibility to use locally hosted models, which can be a cost-effective alternative. To use local models, you will need to run your own API server. You can accomplish this by using [LocalAI](https://github.com/go-skynet/LocalAI), a self-hosted, OpenAI-compatible API. Setting up LocalAI allows you to run language models on your own hardware, potentially without the need for an internet connection, depending on your usage. To set up your LocalAI, please follow this comprehensive [guide](https://github.com/TheR1D/shell_gpt/wiki/LocalAI). Remember that the performance of your local models may depend on the specifications of your hardware and the specific language model you choose to deploy.
+
 ## Docker
 Run the container using the `OPENAI_API_KEY` environment variable, and a docker volume to store cache:
 ```shell
 docker run --rm \
            --env OPENAI_API_KEY="your OPENAI API key" \
            --volume gpt-cache:/tmp/shell_gpt \
        ghcr.io/ther1d/shell_gpt --chat rainbow "what are the colors of a rainbow"
```

