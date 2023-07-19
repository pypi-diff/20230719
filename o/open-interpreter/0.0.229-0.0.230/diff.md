# Comparing `tmp/open_interpreter-0.0.229.tar.gz` & `tmp/open_interpreter-0.0.230.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_interpreter-0.0.229.tar", max compression
+gzip compressed data, was "open_interpreter-0.0.230.tar", max compression
```

## Comparing `open_interpreter-0.0.229.tar` & `open_interpreter-0.0.230.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.229/LICENSE
--rw-r--r--   0        0        0     4310 2023-07-16 23:26:22.204308 open_interpreter-0.0.229/README.md
--rw-r--r--   0        0        0      135 2023-07-14 08:44:08.027686 open_interpreter-0.0.229/interpreter/__init__.py
--rw-r--r--   0        0        0     5703 2023-07-16 23:55:18.448937 open_interpreter-0.0.229/interpreter/exec.py
--rw-r--r--   0        0        0     5847 2023-07-15 17:55:30.625029 open_interpreter-0.0.229/interpreter/interpreter.py
--rw-r--r--   0        0        0     2735 2023-07-14 07:41:45.322446 open_interpreter-0.0.229/interpreter/json_utils.py
--rw-r--r--   0        0        0     3850 2023-07-16 18:00:27.412921 open_interpreter-0.0.229/interpreter/openai_utils.py
--rw-r--r--   0        0        0     1379 2023-07-16 09:25:30.855857 open_interpreter-0.0.229/interpreter/system_message.txt
--rw-r--r--   0        0        0     3322 2023-07-14 07:41:46.414527 open_interpreter-0.0.229/interpreter/view.py
--rw-r--r--   0        0        0      542 2023-07-17 00:55:57.159467 open_interpreter-0.0.229/pyproject.toml
--rw-r--r--   0        0        0     4891 1970-01-01 00:00:00.000000 open_interpreter-0.0.229/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.230/LICENSE
+-rw-r--r--   0        0        0     5627 2023-07-18 19:30:20.415609 open_interpreter-0.0.230/README.md
+-rw-r--r--   0        0        0      135 2023-07-14 08:44:08.027686 open_interpreter-0.0.230/interpreter/__init__.py
+-rw-r--r--   0        0        0     5921 2023-07-19 00:31:13.036280 open_interpreter-0.0.230/interpreter/exec.py
+-rw-r--r--   0        0        0     6186 2023-07-19 00:32:29.437831 open_interpreter-0.0.230/interpreter/interpreter.py
+-rw-r--r--   0        0        0     2735 2023-07-14 07:41:45.322446 open_interpreter-0.0.230/interpreter/json_utils.py
+-rw-r--r--   0        0        0     3850 2023-07-16 18:00:27.412921 open_interpreter-0.0.230/interpreter/openai_utils.py
+-rw-r--r--   0        0        0     1994 2023-07-18 23:08:17.436870 open_interpreter-0.0.230/interpreter/system_message.txt
+-rw-r--r--   0        0        0     3322 2023-07-19 00:31:12.448238 open_interpreter-0.0.230/interpreter/view.py
+-rw-r--r--   0        0        0      542 2023-07-19 00:31:19.296735 open_interpreter-0.0.230/pyproject.toml
+-rw-r--r--   0        0        0     6208 1970-01-01 00:00:00.000000 open_interpreter-0.0.230/PKG-INFO
```

### Comparing `open_interpreter-0.0.229/LICENSE` & `open_interpreter-0.0.230/LICENSE`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.229/README.md` & `open_interpreter-0.0.230/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,59 +1,83 @@
 # Open Interpreter
 
-Open Interpreter is a lightweight, open-source implementation of OpenAI's Code Interpreter.
+A lightweight, open-source implementation of OpenAI's code interpreter.
 
 ```python
-interpreter.chat("Add subtitles to video.mp4 on my Desktop.")
+interpreter.chat('Hey, can you add subtitles to video.mp4 on my Desktop?')
 ```
 ```
->>> On it. First, I'll check if any speech-to-text libraries are installed...
+Absolutely. First, let's check if any speech-to-text libraries are installed...
 ```
 
 <br>
 
 ![Banner Image](https://github.com/KillianLucas/open-interpreter/blob/main/misc/banner.png)
 
 <p align="right">
-    <sub><i>Illustration created by Open Interpreter. Inspired by <a href="https://rubywjchen.com/">Ruby Chen's</a> GPT-4 artwork.</i></sub>
+    <sub><i>Illustration by Open Interpreter. Inspired by <a href="https://rubywjchen.com/">Ruby Chen's</a> GPT-4 artwork.</i></sub>
 </p>
 
-## Demo Notebook
+## What is this?
 
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1WKmRXZgsErej2xUriKzxrEAXdxMSgWbb?usp=sharing)
+<br>
+
+> Having access to a junior programmer working at the speed of your fingertips ... can make new workflows effortless and efficient, as well as open the benefits of programming to new audiences.
+>
+> — _OpenAI's Code Interpreter Release_
+
+<br>
+
+**Open Interpreter** lets GPT-4 run Python code locally. You can chat with Open Interpreter through a ChatGPT-like interface in your terminal by running `$ interpreter` after installing.
+
+This provides a natural language interface to Python's general-purpose capabilities:
+
+- Create and edit photos, videos, PDFs, etc.
+- Run `selenium` to control a Chrome browser.
+- Modify files/folders on your local system.
+- ...etc.
+
+<br>
+
+[How does this compare to OpenAI's code interpreter?](https://github.com/KillianLucas/open-interpreter#comparison-to-chatgpts-code-interpreter)
+
+<br>
 
 ## Features
 
 - Generated code runs locally.
 - Uses `pip` and `apt-get` to extend itself.
 - Interactive, streaming chat inside your terminal.
 
+## Demo Notebook
+
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1WKmRXZgsErej2xUriKzxrEAXdxMSgWbb?usp=sharing)
+
 ## Quick Start
 
 ```shell
 pip install open-interpreter
 ```
 
-```python
-import interpreter
-interpreter.api_key = "<your_openai_api_key>"
+### Terminal
 
-# Start an interactive chat in your terminal
-interpreter.chat()
-```
+After installation, set your `OPENAI_API_KEY` environment variable, then simply run `interpreter`:
 
-## Use Cases
+```shell
+interpreter
+```
 
-Open Interpreter acts as a seasoned programmer that can execute code snippets to accomplish tasks.
+### Python
 
-1. Add subtitles to all videos in a folder.
-2. Blur all faces in a photo or video.
-4. Edit a large batch of documents.
+```python
+import interpreter
 
-...
+interpreter.api_key = "<openai_api_key>"
+interpreter.chat() # Starts an interactive chat
+```
 
 ## Comparison to ChatGPT's Code Interpreter
 
 OpenAI's recent release of [Code Interpreter](https://openai.com/blog/chatgpt-plugins#code-interpreter) with GPT-4 presents a fantastic opportunity to accomplish real-world tasks with ChatGPT.
 
 However, OpenAI's service is hosted, closed-source, and heavily restricted:
 - No internet access.
@@ -65,23 +89,29 @@
 
 Open Interpreter overcomes these limitations by running in a stateful Jupyter notebook on your local environment. It has full access to the internet, isn't restricted by time or file size, and can utilize any package or library.
 
 **Open Interpreter combines the power of GPT-4's Code Interpreter with the flexibility of your local development environment.**
 
 ## Commands
 
-#### Terminal Chat
+#### Interactive Chat
 
-Running `.chat()` will start an interactive session in your terminal:
+To start an interactive chat in your terminal, either run `interpreter` from the command line:
+
+```shell
+interpreter
+```
+
+Or `interpreter.chat()` from a .py file:
 
 ```python
 interpreter.chat()
 ```
 
-#### Python Chat
+#### Programmatic Chat
 
 For more precise control, you can pass messages directly to `.chat(message)`:
 
 ```python
 interpreter.chat("Add subtitles to all videos in /videos.")
 
 # ... Streams output to your terminal, completes task ...
@@ -89,28 +119,29 @@
 interpreter.chat("These look great but can you make the subtitles bigger?")
 
 # ...
 ```
 
 #### Start a New Chat
 
-By default, Open Interpreter remembers conversation history. If you want to start fresh, you can reset it:
+In Python, Open Interpreter remembers conversation history. If you want to start fresh, you can reset it:
 
 ```python
 interpreter.reset()
 ```
 
-Then [start a chat as described above](https://github.com/KillianLucas/open-interpreter#terminal-chat).
-
 #### Save and Restore Chats
 
 `interpreter.chat()` returns a List of messages, which can be restored with `interpreter.load(messages)`:
 
 ```python
-interpreter.load(chat)
+messages = interpreter.chat() # Save chat to 'messages'
+interpreter.reset() # Reset interpreter
+
+interpreter.load(messages) # Resume chat from 'messages'
 ```
 
 #### Customize System Message
 
 You can inspect and configure Open Interpreter's system message to extend its functionality, modify permissions, or give it more context.
 
 ```python
@@ -118,22 +149,30 @@
 Run shell commands with -y so the user doesn't have to confirm them.
 """
 print(interpreter.system_message)
 ```
 
 ## How Does it Work?
 
-Open Interpreter equips a [function-calling](https://platform.openai.com/docs/guides/gpt/function-calling) GPT-4 with the `exec()` function.
+Open Interpreter equips a [function-calling GPT-4](https://platform.openai.com/docs/guides/gpt/function-calling) with the `exec()` function.
 
 We then stream the model's messages, code, and your system's outputs to the terminal as Markdown.
 
 Only the last `model_max_tokens` of the conversation are shown to the model, so conversations can be any length, but older messages may be forgotten.
 
+## Safety Notice
+
+Since generated code is executed in your local environment, it can interact with your files and system settings, potentially leading to unexpected outcomes like data loss or security risks.
+
+- Be cautious when requesting commands that modify files or system settings.
+- Watch Open Interpreter like a self-driving car, and be prepared to end the process by closing your terminal.
+- Regularly back up your data and work in a virtual environment.
+
 ## Contributing
 
 As an open-source project, we are extremely open to contributions, whether it be in the form of a new feature, improved infrastructure, or better documentation.
 
 ## License
 
 Open Interpreter is licensed under the MIT License. You are permitted to use, copy, modify, distribute, sublicense and sell copies of the software.
 
-**Note**: This software is not affiliated with OpenAI.
+**Note**: This software is not affiliated with OpenAI.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,57 +1,76 @@
-# Open Interpreter Open Interpreter is a lightweight, open-source
-implementation of OpenAI's Code Interpreter. ```python interpreter.chat("Add
-subtitles to video.mp4 on my Desktop.") ``` ``` >>> On it. First, I'll check if
-any speech-to-text libraries are installed... ```
+# Open Interpreter A lightweight, open-source implementation of OpenAI's code
+interpreter. ```python interpreter.chat('Hey, can you add subtitles to
+video.mp4 on my Desktop?') ``` ``` Absolutely. First, let's check if any
+speech-to-text libraries are installed... ```
 ![Banner Image](https://github.com/KillianLucas/open-interpreter/blob/main/
 misc/banner.png)
-         Illustration created by Open Interpreter. Inspired by Ruby_Chen's GPT-
-                                                                     4 artwork.
-## Demo Notebook [![Open In Colab](https://colab.research.google.com/assets/
-colab-badge.svg)](https://colab.research.google.com/drive/
-1WKmRXZgsErej2xUriKzxrEAXdxMSgWbb?usp=sharing) ## Features - Generated code
-runs locally. - Uses `pip` and `apt-get` to extend itself. - Interactive,
-streaming chat inside your terminal. ## Quick Start ```shell pip install open-
-interpreter ``` ```python import interpreter interpreter.api_key = "" # Start
-an interactive chat in your terminal interpreter.chat() ``` ## Use Cases Open
-Interpreter acts as a seasoned programmer that can execute code snippets to
-accomplish tasks. 1. Add subtitles to all videos in a folder. 2. Blur all faces
-in a photo or video. 4. Edit a large batch of documents. ... ## Comparison to
+       Illustration by Open Interpreter. Inspired by Ruby_Chen's GPT-4 artwork.
+## What is this?
+> Having access to a junior programmer working at the speed of your fingertips
+... can make new workflows effortless and efficient, as well as open the
+benefits of programming to new audiences. > > â _OpenAI's Code Interpreter
+Release_
+**Open Interpreter** lets GPT-4 run Python code locally. You can chat with Open
+Interpreter through a ChatGPT-like interface in your terminal by running `$
+interpreter` after installing. This provides a natural language interface to
+Python's general-purpose capabilities: - Create and edit photos, videos, PDFs,
+etc. - Run `selenium` to control a Chrome browser. - Modify files/folders on
+your local system. - ...etc.
+[How does this compare to OpenAI's code interpreter?](https://github.com/
+KillianLucas/open-interpreter#comparison-to-chatgpts-code-interpreter)
+## Features - Generated code runs locally. - Uses `pip` and `apt-get` to extend
+itself. - Interactive, streaming chat inside your terminal. ## Demo Notebook [!
+[Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
+(https://colab.research.google.com/drive/
+1WKmRXZgsErej2xUriKzxrEAXdxMSgWbb?usp=sharing) ## Quick Start ```shell pip
+install open-interpreter ``` ### Terminal After installation, set your
+`OPENAI_API_KEY` environment variable, then simply run `interpreter`: ```shell
+interpreter ``` ### Python ```python import interpreter interpreter.api_key =
+"" interpreter.chat() # Starts an interactive chat ``` ## Comparison to
 ChatGPT's Code Interpreter OpenAI's recent release of [Code Interpreter](https:
 //openai.com/blog/chatgpt-plugins#code-interpreter) with GPT-4 presents a
 fantastic opportunity to accomplish real-world tasks with ChatGPT. However,
 OpenAI's service is hosted, closed-source, and heavily restricted: - No
 internet access. - [Limited set of pre-installed packages](https://
 wfhbrian.com/mastering-chatgpts-code-interpreter-list-of-python-packages/). -
 100 MB maximum upload, 120.0 second runtime limit. - State is cleared (along
 with any generated files or links) when the environment dies. --- Open
 Interpreter overcomes these limitations by running in a stateful Jupyter
 notebook on your local environment. It has full access to the internet, isn't
 restricted by time or file size, and can utilize any package or library. **Open
 Interpreter combines the power of GPT-4's Code Interpreter with the flexibility
-of your local development environment.** ## Commands #### Terminal Chat Running
-`.chat()` will start an interactive session in your terminal: ```python
-interpreter.chat() ``` #### Python Chat For more precise control, you can pass
-messages directly to `.chat(message)`: ```python interpreter.chat("Add
-subtitles to all videos in /videos.") # ... Streams output to your terminal,
-completes task ... interpreter.chat("These look great but can you make the
-subtitles bigger?") # ... ``` #### Start a New Chat By default, Open
-Interpreter remembers conversation history. If you want to start fresh, you can
-reset it: ```python interpreter.reset() ``` Then [start a chat as described
-above](https://github.com/KillianLucas/open-interpreter#terminal-chat). ####
-Save and Restore Chats `interpreter.chat()` returns a List of messages, which
-can be restored with `interpreter.load(messages)`: ```python interpreter.load
-(chat) ``` #### Customize System Message You can inspect and configure Open
-Interpreter's system message to extend its functionality, modify permissions,
-or give it more context. ```python interpreter.system_message += """ Run shell
-commands with -y so the user doesn't have to confirm them. """ print
+of your local development environment.** ## Commands #### Interactive Chat To
+start an interactive chat in your terminal, either run `interpreter` from the
+command line: ```shell interpreter ``` Or `interpreter.chat()` from a .py file:
+```python interpreter.chat() ``` #### Programmatic Chat For more precise
+control, you can pass messages directly to `.chat(message)`: ```python
+interpreter.chat("Add subtitles to all videos in /videos.") # ... Streams
+output to your terminal, completes task ... interpreter.chat("These look great
+but can you make the subtitles bigger?") # ... ``` #### Start a New Chat In
+Python, Open Interpreter remembers conversation history. If you want to start
+fresh, you can reset it: ```python interpreter.reset() ``` #### Save and
+Restore Chats `interpreter.chat()` returns a List of messages, which can be
+restored with `interpreter.load(messages)`: ```python messages =
+interpreter.chat() # Save chat to 'messages' interpreter.reset() # Reset
+interpreter interpreter.load(messages) # Resume chat from 'messages' ``` ####
+Customize System Message You can inspect and configure Open Interpreter's
+system message to extend its functionality, modify permissions, or give it more
+context. ```python interpreter.system_message += """ Run shell commands with -
+y so the user doesn't have to confirm them. """ print
 (interpreter.system_message) ``` ## How Does it Work? Open Interpreter equips a
-[function-calling](https://platform.openai.com/docs/guides/gpt/function-
-calling) GPT-4 with the `exec()` function. We then stream the model's messages,
-code, and your system's outputs to the terminal as Markdown. Only the last
+[function-calling GPT-4](https://platform.openai.com/docs/guides/gpt/function-
+calling) with the `exec()` function. We then stream the model's messages, code,
+and your system's outputs to the terminal as Markdown. Only the last
 `model_max_tokens` of the conversation are shown to the model, so conversations
-can be any length, but older messages may be forgotten. ## Contributing As an
-open-source project, we are extremely open to contributions, whether it be in
-the form of a new feature, improved infrastructure, or better documentation. ##
-License Open Interpreter is licensed under the MIT License. You are permitted
-to use, copy, modify, distribute, sublicense and sell copies of the software.
-**Note**: This software is not affiliated with OpenAI.
+can be any length, but older messages may be forgotten. ## Safety Notice Since
+generated code is executed in your local environment, it can interact with your
+files and system settings, potentially leading to unexpected outcomes like data
+loss or security risks. - Be cautious when requesting commands that modify
+files or system settings. - Watch Open Interpreter like a self-driving car, and
+be prepared to end the process by closing your terminal. - Regularly back up
+your data and work in a virtual environment. ## Contributing As an open-source
+project, we are extremely open to contributions, whether it be in the form of a
+new feature, improved infrastructure, or better documentation. ## License Open
+Interpreter is licensed under the MIT License. You are permitted to use, copy,
+modify, distribute, sublicense and sell copies of the software. **Note**: This
+software is not affiliated with OpenAI.
```

### Comparing `open_interpreter-0.0.229/interpreter/exec.py` & `open_interpreter-0.0.230/interpreter/exec.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,45 +16,45 @@
 def check_for_syntax_errors(code):
     # Needs to happen before we execute.
     lines = code.split('\n')
     filtered_lines = [line for line in lines if not re.match(r'^[!%]', line.strip())]
     cleaned_code = '\n'.join(filtered_lines)
     compile(cleaned_code, '<string>', 'exec')
 
-def truncate_output(data):
-    max_length = 7000
-    message = f'Output truncated. Showing the last {max_length} characters:\n\n'
+def truncate_output(data, max_output_chars):
+    message = f'Output truncated. Showing the last {max_output_chars} characters (change this number by setting interpreter.max_output_chars):\n\n'
 
     # Remove previous truncation message if it exists
     if data.startswith(message):
         data = data[len(message):]
 
     # If data exceeds max length, truncate it and add message
-    if len(data) > max_length:
-        data = message + data[-max_length:]
+    if len(data) > max_output_chars:
+        data = message + data[-max_output_chars:]
     return data
 
 class RichOutStream:
 
-    def __init__(self, live):
+    def __init__(self, live, max_output_chars):
         self.live = live
         self.data = ""
+        self.max_output_chars = max_output_chars
 
     def write(self, data):
         self.data += data
 
         # Clean ANSI color codes
         self.data = re.sub(r'\x1b\[[0-9;]*m', '', self.data)
       
         # Clean ANSI escape sequences
         ansi_escape = re.compile(r'\x1B(?:[@-Z\\-_]|\[[0-?]*[ -/]*[@-~])')
         self.data = ansi_escape.sub('', self.data)
 
         # Truncate and prepend a message if truncated
-        self.data = truncate_output(self.data)
+        self.data = truncate_output(self.data, max_output_chars=self.max_output_chars)
 
         # None outputs should be empty, they happen with things like plt.show()
         if self.data.strip() == "None" or self.data.strip() == "":
             self.data = ""
             self.live.update("", refresh=True)
         else:
             panel = Panel(self.data.strip(), box=MINIMAL, style="#FFFFFF on #3b3b37")
@@ -64,15 +64,15 @@
         pass
 
     # Some things (like youtube-dl) will check if this is "isatty()"
     # then fail if it isn't present, so. If this is True it breaks the CLI, so we set it to False (I don't know what it means).
     def isatty(self):
         return False
 
-def exec_and_capture_output(code):
+def exec_and_capture_output(code, max_output_chars):
     # Store the original stdout and stderr
     old_stdout = sys.stdout
     old_stderr = sys.stderr
 
     # Create new instance of InteractiveShell
     shell = InteractiveShell.instance()
 
@@ -91,15 +91,15 @@
     shell.showtraceback = custom_showtraceback
 
     code = jupyterify_code(code)
 
     live = Live(console=Console(), auto_refresh=False)  # Set auto_refresh to False to update manually
     try:
         live.start()
-        rich_stdout = RichOutStream(live)
+        rich_stdout = RichOutStream(live, max_output_chars)
 
         # Check syntax before attempting to execute
         try:
             check_for_syntax_errors(code)
         except SyntaxError:
             # Do the same thing you do in custom_showtraceback
             etype, value, tb = sys.exc_info()
```

### Comparing `open_interpreter-0.0.229/interpreter/interpreter.py` & `open_interpreter-0.0.230/interpreter/interpreter.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 class Interpreter:
     def __init__(self):
         self.messages = []
         self._logs = []
         self.system_message = system_message
         self.temperature = 0.2
         self.api_key = None
+        self.max_output_chars = 2000
 
     def reset(self):
         self.messages = []
         self._logs = []
 
     def load(self, messages):
         self.messages = messages
@@ -49,15 +50,15 @@
 
         else:
             print("Type 'exit' to leave the chat.\n")
 
             while True:
                 user_input = input("> ")
 
-                if user_input == 'exit':
+                if user_input == 'exit' or user_input == 'exit()':
                     break
 
                 self.messages.append({"role": "user", "content": user_input})
                 self.respond()
 
         if return_chat:
             return self.messages
@@ -153,14 +154,19 @@
                       function_args = json.loads(func_call["arguments"])
                     except:
                       function_args = {"code": func_call["arguments"]}
 
                     # The output might use a rich Live display so we need to finalize ours.
                     self.view.finalize()
 
+                    # For interpreter. This should always be true:
+                    if func_call["name"] == "run_code":
+                      # Pass in max_output_chars to truncate the output
+                      function_args["max_output_chars"] = self.max_output_chars
+
                     output = function(**function_args)
 
                     event = {
                         "role": "function",
                         "name": func_call["name"],
                         "content": output
                     }
```

### Comparing `open_interpreter-0.0.229/interpreter/json_utils.py` & `open_interpreter-0.0.230/interpreter/json_utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.229/interpreter/openai_utils.py` & `open_interpreter-0.0.230/interpreter/openai_utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.229/interpreter/view.py` & `open_interpreter-0.0.230/interpreter/view.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.229/pyproject.toml` & `open_interpreter-0.0.230/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "open-interpreter"
 packages = [
     {include = "interpreter"}
 ]
-version = "0.0.229"
+version = "0.0.230"
 description = "Ask GPT-4 to run code locally."
 authors = ["Killian Lucas <killian@drinkwater.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 openai = "^0.27.8"
```

### Comparing `open_interpreter-0.0.229/PKG-INFO` & `open_interpreter-0.0.230/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-interpreter
-Version: 0.0.229
+Version: 0.0.230
 Summary: Ask GPT-4 to run code locally.
 Author: Killian Lucas
 Author-email: killian@drinkwater.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -13,64 +13,88 @@
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: rich (>=13.4.2,<14.0.0)
 Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
 Description-Content-Type: text/markdown
 
 # Open Interpreter
 
-Open Interpreter is a lightweight, open-source implementation of OpenAI's Code Interpreter.
+A lightweight, open-source implementation of OpenAI's code interpreter.
 
 ```python
-interpreter.chat("Add subtitles to video.mp4 on my Desktop.")
+interpreter.chat('Hey, can you add subtitles to video.mp4 on my Desktop?')
 ```
 ```
->>> On it. First, I'll check if any speech-to-text libraries are installed...
+Absolutely. First, let's check if any speech-to-text libraries are installed...
 ```
 
 <br>
 
 ![Banner Image](https://github.com/KillianLucas/open-interpreter/blob/main/misc/banner.png)
 
 <p align="right">
-    <sub><i>Illustration created by Open Interpreter. Inspired by <a href="https://rubywjchen.com/">Ruby Chen's</a> GPT-4 artwork.</i></sub>
+    <sub><i>Illustration by Open Interpreter. Inspired by <a href="https://rubywjchen.com/">Ruby Chen's</a> GPT-4 artwork.</i></sub>
 </p>
 
-## Demo Notebook
+## What is this?
 
-[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1WKmRXZgsErej2xUriKzxrEAXdxMSgWbb?usp=sharing)
+<br>
+
+> Having access to a junior programmer working at the speed of your fingertips ... can make new workflows effortless and efficient, as well as open the benefits of programming to new audiences.
+>
+> — _OpenAI's Code Interpreter Release_
+
+<br>
+
+**Open Interpreter** lets GPT-4 run Python code locally. You can chat with Open Interpreter through a ChatGPT-like interface in your terminal by running `$ interpreter` after installing.
+
+This provides a natural language interface to Python's general-purpose capabilities:
+
+- Create and edit photos, videos, PDFs, etc.
+- Run `selenium` to control a Chrome browser.
+- Modify files/folders on your local system.
+- ...etc.
+
+<br>
+
+[How does this compare to OpenAI's code interpreter?](https://github.com/KillianLucas/open-interpreter#comparison-to-chatgpts-code-interpreter)
+
+<br>
 
 ## Features
 
 - Generated code runs locally.
 - Uses `pip` and `apt-get` to extend itself.
 - Interactive, streaming chat inside your terminal.
 
+## Demo Notebook
+
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1WKmRXZgsErej2xUriKzxrEAXdxMSgWbb?usp=sharing)
+
 ## Quick Start
 
 ```shell
 pip install open-interpreter
 ```
 
-```python
-import interpreter
-interpreter.api_key = "<your_openai_api_key>"
+### Terminal
 
-# Start an interactive chat in your terminal
-interpreter.chat()
-```
+After installation, set your `OPENAI_API_KEY` environment variable, then simply run `interpreter`:
 
-## Use Cases
+```shell
+interpreter
+```
 
-Open Interpreter acts as a seasoned programmer that can execute code snippets to accomplish tasks.
+### Python
 
-1. Add subtitles to all videos in a folder.
-2. Blur all faces in a photo or video.
-4. Edit a large batch of documents.
+```python
+import interpreter
 
-...
+interpreter.api_key = "<openai_api_key>"
+interpreter.chat() # Starts an interactive chat
+```
 
 ## Comparison to ChatGPT's Code Interpreter
 
 OpenAI's recent release of [Code Interpreter](https://openai.com/blog/chatgpt-plugins#code-interpreter) with GPT-4 presents a fantastic opportunity to accomplish real-world tasks with ChatGPT.
 
 However, OpenAI's service is hosted, closed-source, and heavily restricted:
 - No internet access.
@@ -82,23 +106,29 @@
 
 Open Interpreter overcomes these limitations by running in a stateful Jupyter notebook on your local environment. It has full access to the internet, isn't restricted by time or file size, and can utilize any package or library.
 
 **Open Interpreter combines the power of GPT-4's Code Interpreter with the flexibility of your local development environment.**
 
 ## Commands
 
-#### Terminal Chat
+#### Interactive Chat
+
+To start an interactive chat in your terminal, either run `interpreter` from the command line:
 
-Running `.chat()` will start an interactive session in your terminal:
+```shell
+interpreter
+```
+
+Or `interpreter.chat()` from a .py file:
 
 ```python
 interpreter.chat()
 ```
 
-#### Python Chat
+#### Programmatic Chat
 
 For more precise control, you can pass messages directly to `.chat(message)`:
 
 ```python
 interpreter.chat("Add subtitles to all videos in /videos.")
 
 # ... Streams output to your terminal, completes task ...
@@ -106,28 +136,29 @@
 interpreter.chat("These look great but can you make the subtitles bigger?")
 
 # ...
 ```
 
 #### Start a New Chat
 
-By default, Open Interpreter remembers conversation history. If you want to start fresh, you can reset it:
+In Python, Open Interpreter remembers conversation history. If you want to start fresh, you can reset it:
 
 ```python
 interpreter.reset()
 ```
 
-Then [start a chat as described above](https://github.com/KillianLucas/open-interpreter#terminal-chat).
-
 #### Save and Restore Chats
 
 `interpreter.chat()` returns a List of messages, which can be restored with `interpreter.load(messages)`:
 
 ```python
-interpreter.load(chat)
+messages = interpreter.chat() # Save chat to 'messages'
+interpreter.reset() # Reset interpreter
+
+interpreter.load(messages) # Resume chat from 'messages'
 ```
 
 #### Customize System Message
 
 You can inspect and configure Open Interpreter's system message to extend its functionality, modify permissions, or give it more context.
 
 ```python
@@ -135,22 +166,31 @@
 Run shell commands with -y so the user doesn't have to confirm them.
 """
 print(interpreter.system_message)
 ```
 
 ## How Does it Work?
 
-Open Interpreter equips a [function-calling](https://platform.openai.com/docs/guides/gpt/function-calling) GPT-4 with the `exec()` function.
+Open Interpreter equips a [function-calling GPT-4](https://platform.openai.com/docs/guides/gpt/function-calling) with the `exec()` function.
 
 We then stream the model's messages, code, and your system's outputs to the terminal as Markdown.
 
 Only the last `model_max_tokens` of the conversation are shown to the model, so conversations can be any length, but older messages may be forgotten.
 
+## Safety Notice
+
+Since generated code is executed in your local environment, it can interact with your files and system settings, potentially leading to unexpected outcomes like data loss or security risks.
+
+- Be cautious when requesting commands that modify files or system settings.
+- Watch Open Interpreter like a self-driving car, and be prepared to end the process by closing your terminal.
+- Regularly back up your data and work in a virtual environment.
+
 ## Contributing
 
 As an open-source project, we are extremely open to contributions, whether it be in the form of a new feature, improved infrastructure, or better documentation.
 
 ## License
 
 Open Interpreter is licensed under the MIT License. You are permitted to use, copy, modify, distribute, sublicense and sell copies of the software.
 
 **Note**: This software is not affiliated with OpenAI.
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,65 +1,84 @@
-Metadata-Version: 2.1 Name: open-interpreter Version: 0.0.229 Summary: Ask GPT-
+Metadata-Version: 2.1 Name: open-interpreter Version: 0.0.230 Summary: Ask GPT-
 4 to run code locally. Author: Killian Lucas Author-email:
 killian@drinkwater.ai Requires-Python: >=3.10,<4.0 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: astor
 (>=0.8.1,<0.9.0) Requires-Dist: ipython (>=8.14.0,<9.0.0) Requires-Dist: openai
 (>=0.27.8,<0.28.0) Requires-Dist: rich (>=13.4.2,<14.0.0) Requires-Dist:
 tiktoken (>=0.4.0,<0.5.0) Description-Content-Type: text/markdown # Open
-Interpreter Open Interpreter is a lightweight, open-source implementation of
-OpenAI's Code Interpreter. ```python interpreter.chat("Add subtitles to
-video.mp4 on my Desktop.") ``` ``` >>> On it. First, I'll check if any speech-
-to-text libraries are installed... ```
+Interpreter A lightweight, open-source implementation of OpenAI's code
+interpreter. ```python interpreter.chat('Hey, can you add subtitles to
+video.mp4 on my Desktop?') ``` ``` Absolutely. First, let's check if any
+speech-to-text libraries are installed... ```
 ![Banner Image](https://github.com/KillianLucas/open-interpreter/blob/main/
 misc/banner.png)
-         Illustration created by Open Interpreter. Inspired by Ruby_Chen's GPT-
-                                                                     4 artwork.
-## Demo Notebook [![Open In Colab](https://colab.research.google.com/assets/
-colab-badge.svg)](https://colab.research.google.com/drive/
-1WKmRXZgsErej2xUriKzxrEAXdxMSgWbb?usp=sharing) ## Features - Generated code
-runs locally. - Uses `pip` and `apt-get` to extend itself. - Interactive,
-streaming chat inside your terminal. ## Quick Start ```shell pip install open-
-interpreter ``` ```python import interpreter interpreter.api_key = "" # Start
-an interactive chat in your terminal interpreter.chat() ``` ## Use Cases Open
-Interpreter acts as a seasoned programmer that can execute code snippets to
-accomplish tasks. 1. Add subtitles to all videos in a folder. 2. Blur all faces
-in a photo or video. 4. Edit a large batch of documents. ... ## Comparison to
+       Illustration by Open Interpreter. Inspired by Ruby_Chen's GPT-4 artwork.
+## What is this?
+> Having access to a junior programmer working at the speed of your fingertips
+... can make new workflows effortless and efficient, as well as open the
+benefits of programming to new audiences. > > â _OpenAI's Code Interpreter
+Release_
+**Open Interpreter** lets GPT-4 run Python code locally. You can chat with Open
+Interpreter through a ChatGPT-like interface in your terminal by running `$
+interpreter` after installing. This provides a natural language interface to
+Python's general-purpose capabilities: - Create and edit photos, videos, PDFs,
+etc. - Run `selenium` to control a Chrome browser. - Modify files/folders on
+your local system. - ...etc.
+[How does this compare to OpenAI's code interpreter?](https://github.com/
+KillianLucas/open-interpreter#comparison-to-chatgpts-code-interpreter)
+## Features - Generated code runs locally. - Uses `pip` and `apt-get` to extend
+itself. - Interactive, streaming chat inside your terminal. ## Demo Notebook [!
+[Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
+(https://colab.research.google.com/drive/
+1WKmRXZgsErej2xUriKzxrEAXdxMSgWbb?usp=sharing) ## Quick Start ```shell pip
+install open-interpreter ``` ### Terminal After installation, set your
+`OPENAI_API_KEY` environment variable, then simply run `interpreter`: ```shell
+interpreter ``` ### Python ```python import interpreter interpreter.api_key =
+"" interpreter.chat() # Starts an interactive chat ``` ## Comparison to
 ChatGPT's Code Interpreter OpenAI's recent release of [Code Interpreter](https:
 //openai.com/blog/chatgpt-plugins#code-interpreter) with GPT-4 presents a
 fantastic opportunity to accomplish real-world tasks with ChatGPT. However,
 OpenAI's service is hosted, closed-source, and heavily restricted: - No
 internet access. - [Limited set of pre-installed packages](https://
 wfhbrian.com/mastering-chatgpts-code-interpreter-list-of-python-packages/). -
 100 MB maximum upload, 120.0 second runtime limit. - State is cleared (along
 with any generated files or links) when the environment dies. --- Open
 Interpreter overcomes these limitations by running in a stateful Jupyter
 notebook on your local environment. It has full access to the internet, isn't
 restricted by time or file size, and can utilize any package or library. **Open
 Interpreter combines the power of GPT-4's Code Interpreter with the flexibility
-of your local development environment.** ## Commands #### Terminal Chat Running
-`.chat()` will start an interactive session in your terminal: ```python
-interpreter.chat() ``` #### Python Chat For more precise control, you can pass
-messages directly to `.chat(message)`: ```python interpreter.chat("Add
-subtitles to all videos in /videos.") # ... Streams output to your terminal,
-completes task ... interpreter.chat("These look great but can you make the
-subtitles bigger?") # ... ``` #### Start a New Chat By default, Open
-Interpreter remembers conversation history. If you want to start fresh, you can
-reset it: ```python interpreter.reset() ``` Then [start a chat as described
-above](https://github.com/KillianLucas/open-interpreter#terminal-chat). ####
-Save and Restore Chats `interpreter.chat()` returns a List of messages, which
-can be restored with `interpreter.load(messages)`: ```python interpreter.load
-(chat) ``` #### Customize System Message You can inspect and configure Open
-Interpreter's system message to extend its functionality, modify permissions,
-or give it more context. ```python interpreter.system_message += """ Run shell
-commands with -y so the user doesn't have to confirm them. """ print
+of your local development environment.** ## Commands #### Interactive Chat To
+start an interactive chat in your terminal, either run `interpreter` from the
+command line: ```shell interpreter ``` Or `interpreter.chat()` from a .py file:
+```python interpreter.chat() ``` #### Programmatic Chat For more precise
+control, you can pass messages directly to `.chat(message)`: ```python
+interpreter.chat("Add subtitles to all videos in /videos.") # ... Streams
+output to your terminal, completes task ... interpreter.chat("These look great
+but can you make the subtitles bigger?") # ... ``` #### Start a New Chat In
+Python, Open Interpreter remembers conversation history. If you want to start
+fresh, you can reset it: ```python interpreter.reset() ``` #### Save and
+Restore Chats `interpreter.chat()` returns a List of messages, which can be
+restored with `interpreter.load(messages)`: ```python messages =
+interpreter.chat() # Save chat to 'messages' interpreter.reset() # Reset
+interpreter interpreter.load(messages) # Resume chat from 'messages' ``` ####
+Customize System Message You can inspect and configure Open Interpreter's
+system message to extend its functionality, modify permissions, or give it more
+context. ```python interpreter.system_message += """ Run shell commands with -
+y so the user doesn't have to confirm them. """ print
 (interpreter.system_message) ``` ## How Does it Work? Open Interpreter equips a
-[function-calling](https://platform.openai.com/docs/guides/gpt/function-
-calling) GPT-4 with the `exec()` function. We then stream the model's messages,
-code, and your system's outputs to the terminal as Markdown. Only the last
+[function-calling GPT-4](https://platform.openai.com/docs/guides/gpt/function-
+calling) with the `exec()` function. We then stream the model's messages, code,
+and your system's outputs to the terminal as Markdown. Only the last
 `model_max_tokens` of the conversation are shown to the model, so conversations
-can be any length, but older messages may be forgotten. ## Contributing As an
-open-source project, we are extremely open to contributions, whether it be in
-the form of a new feature, improved infrastructure, or better documentation. ##
-License Open Interpreter is licensed under the MIT License. You are permitted
-to use, copy, modify, distribute, sublicense and sell copies of the software.
-**Note**: This software is not affiliated with OpenAI.
+can be any length, but older messages may be forgotten. ## Safety Notice Since
+generated code is executed in your local environment, it can interact with your
+files and system settings, potentially leading to unexpected outcomes like data
+loss or security risks. - Be cautious when requesting commands that modify
+files or system settings. - Watch Open Interpreter like a self-driving car, and
+be prepared to end the process by closing your terminal. - Regularly back up
+your data and work in a virtual environment. ## Contributing As an open-source
+project, we are extremely open to contributions, whether it be in the form of a
+new feature, improved infrastructure, or better documentation. ## License Open
+Interpreter is licensed under the MIT License. You are permitted to use, copy,
+modify, distribute, sublicense and sell copies of the software. **Note**: This
+software is not affiliated with OpenAI.
```

