# Comparing `tmp/dfpyre-0.3.1.tar.gz` & `tmp/dfpyre-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dfpyre-0.3.1.tar", last modified: Sun Jul 16 23:37:30 2023, max compression
+gzip compressed data, was "dfpyre-0.3.3.tar", last modified: Wed Jul 19 03:40:23 2023, max compression
```

## Comparing `dfpyre-0.3.1.tar` & `dfpyre-0.3.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 23:37:30.622538 dfpyre-0.3.1/
--rw-rw-rw-   0        0        0     1081 2023-07-15 02:28:19.000000 dfpyre-0.3.1/LICENSE
--rw-rw-rw-   0        0        0      275 2023-07-16 23:37:30.621268 dfpyre-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0    10197 2023-07-14 03:50:47.000000 dfpyre-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-16 23:37:30.580906 dfpyre-0.3.1/dfpyre/
--rw-rw-rw-   0        0        0       25 2023-07-14 02:26:37.000000 dfpyre-0.3.1/dfpyre/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-16 23:37:30.620269 dfpyre-0.3.1/dfpyre/data/
--rw-rw-rw-   0        0        0    50261 2023-07-14 02:33:57.000000 dfpyre-0.3.1/dfpyre/data/data.json
--rw-rw-rw-   0        0        0     5555 2023-07-14 03:05:11.000000 dfpyre-0.3.1/dfpyre/items.py
--rw-rw-rw-   0        0        0    11831 2023-07-15 02:16:20.000000 dfpyre-0.3.1/dfpyre/pyre.py
-drwxrwxrwx   0        0        0        0 2023-07-16 23:37:30.606680 dfpyre-0.3.1/dfpyre.egg-info/
--rw-rw-rw-   0        0        0      275 2023-07-16 23:37:30.000000 dfpyre-0.3.1/dfpyre.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2023-07-16 23:37:30.000000 dfpyre-0.3.1/dfpyre.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 23:37:30.000000 dfpyre-0.3.1/dfpyre.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-16 23:37:30.000000 dfpyre-0.3.1/dfpyre.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-16 23:37:30.622538 dfpyre-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0      410 2023-07-16 23:37:24.000000 dfpyre-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-19 03:40:23.072375 dfpyre-0.3.3/
+-rw-rw-rw-   0        0        0     1081 2023-07-15 02:28:19.000000 dfpyre-0.3.3/LICENSE
+-rw-rw-rw-   0        0        0      275 2023-07-19 03:40:23.071371 dfpyre-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0    10197 2023-07-14 03:50:47.000000 dfpyre-0.3.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-19 03:40:23.050648 dfpyre-0.3.3/dfpyre/
+-rw-rw-rw-   0        0        0       25 2023-07-14 02:26:37.000000 dfpyre-0.3.3/dfpyre/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-19 03:40:23.069373 dfpyre-0.3.3/dfpyre/data/
+-rw-rw-rw-   0        0        0    50261 2023-07-14 02:33:57.000000 dfpyre-0.3.3/dfpyre/data/data.json
+-rw-rw-rw-   0        0        0     5555 2023-07-14 03:05:11.000000 dfpyre-0.3.3/dfpyre/items.py
+-rw-rw-rw-   0        0        0    12827 2023-07-19 03:37:10.000000 dfpyre-0.3.3/dfpyre/pyre.py
+drwxrwxrwx   0        0        0        0 2023-07-19 03:40:23.068371 dfpyre-0.3.3/dfpyre.egg-info/
+-rw-rw-rw-   0        0        0      275 2023-07-19 03:40:22.000000 dfpyre-0.3.3/dfpyre.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2023-07-19 03:40:22.000000 dfpyre-0.3.3/dfpyre.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-19 03:40:22.000000 dfpyre-0.3.3/dfpyre.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-19 03:40:22.000000 dfpyre-0.3.3/dfpyre.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-19 03:40:23.072375 dfpyre-0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      410 2023-07-19 03:39:33.000000 dfpyre-0.3.3/setup.py
```

### Comparing `dfpyre-0.3.1/LICENSE` & `dfpyre-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dfpyre-0.3.1/README.md` & `dfpyre-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `dfpyre-0.3.1/dfpyre/data/data.json` & `dfpyre-0.3.3/dfpyre/data/data.json`

 * *Files identical despite different names*

### Comparing `dfpyre-0.3.1/dfpyre/items.py` & `dfpyre-0.3.3/dfpyre/items.py`

 * *Files identical despite different names*

### Comparing `dfpyre-0.3.1/dfpyre/pyre.py` & `dfpyre-0.3.3/dfpyre/pyre.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from dfpyre.items import *
 
 COL_WARN = '\x1b[33m'
 COL_RESET = '\x1b[0m'
 COL_SUCCESS = '\x1b[32m'
 COL_ERROR = '\x1b[31m'
 
-CODEBLOCK_DATA_PATH = 'dfpyre/data/data.json'
+CODEBLOCK_DATA_PATH = os.path.join(os.path.dirname(__file__), 'data/data.json')
 
 VARIABLE_TYPES = {'txt', 'num', 'item', 'loc', 'var', 'snd', 'part', 'pot', 'g_val', 'vec'}
 TEMPLATE_STARTERS = {'event', 'entity_event', 'func', 'process'}
 
 
 def _warn(message):
     print(f'{COL_WARN}! WARNING ! {message}{COL_RESET}')
@@ -42,70 +42,103 @@
         tagData,
         set(tagData.keys()),
         set(tagData['extras'].keys())
     )
 
 TAGDATA, TAGDATA_KEYS, TAGDATA_EXTRAS_KEYS = _loadCodeblockData()
 
-def sendToDf(templateCode: str, name: str='Unnamed Template'):
+def sendToDf(templateCode: str, name: str='Unnamed Template', author: str='pyre'):
     """
     Sends a template to DiamondFire via recode item api.
 
-    :param str templateCode: The code for the template in base64 format.
+    :param str templateCode: The code for the template as a base64 string.
     :param str name: The name of the template.
+    :param str author: The author of this template.
     """
+    templateData = f"""{{\
+Count:1b,\
+id:"minecraft:yellow_shulker_box",\
+tag:{{\
+display:{{\
+Name:'{{"extra":[{{"italic":false,"color":"#FF5C00","text":">> "}},{{"italic":false,"color":"#FFC700","text":"{name}"}}],"text":""}}',\
+Lore:[
+'{{"extra":[{{"italic":false,"color":"gray","text":"This template was generated by "}},{{"italic":false,"color":"gold","text":"pyre"}},{{"italic":false,"color":"gray","text":"."}}],"text":""}}',\
+'{{"extra":[{{"italic":false,"color":"gray","text":"https://github.com/Amp63/pyre"}},{{"italic":false,"underlined":false,"strikethrough":false,"obfuscated":false,"color":"gray","text":""}}],"text":""}}'\
+]\
+}},\
+PublicBukkitValues:{{\
+"hypercube:codetemplatedata":'{{\
+"author":"{author}",\
+"name":"{name}",\
+"version":1,\
+"code":"{templateCode}"\
+}}'\
+}}\
+}}\
+}}\
+"""
     itemName = 'pyre Template - ' + name
-    templateData = f"{{\"name\":\"{itemName}\",\"data\":\"{templateCode}\"}}"
-    data = {"type": "template", "source": f"pyre - {name}","data": templateData}
+    data = {'type': 'nbt', 'source': itemName, 'data': templateData}
+
     s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
     try:
         s.connect(('127.0.0.1', 31372))
     except ConnectionRefusedError:
         print(f'{COL_ERROR}Could not connect to recode item API. (Minecraft is not open or something else has gone wrong){COL_RESET}')
         s.close()
         return
     
-    s.send((str(data) + '\n').encode())
+    s.send((str(data) + '\n').encode('utf_8'))
     received = json.loads(s.recv(1024).decode())
     status = received['status']
     if status == 'success':
         print(f'{COL_SUCCESS}Template sent to client successfully.{COL_RESET}')
     else:
         error = received['error']
         print(f'{COL_ERROR}Error sending template: {error}{COL_RESET}')
+    
     s.close()
     time.sleep(0.5)
 
 
+class CodeBlock:
+    def __init__(self, name: str, *args, target: str='Default', data={}):
+        self.name = name
+        self.args = args
+        self.target = target
+        self.data = data
+
+
 class DFTemplate:
     """
     Represents a DiamondFire code template.
     """
-    def __init__(self):
-        self.commands = []
+    def __init__(self, name=None):
+        self.codeBlocks = []
         self.closebracket = None
         self.definedVars = {}
+        self.name = name
 
 
     def build(self) -> Tuple[str, str]:
         """
         Build this template.
 
         :return: Tuple containing compressed template code and template name.
         """
         mainDict = {'blocks': []}
-        for cmd in self.commands:
+        for cmd in self.codeBlocks:
             block = {'args': {'items': []}}
             
             # add keys from cmd.data
             for key in cmd.data.keys():
                 block[key] = cmd.data[key]
 
             # bracket data
-            if cmd.data.get('direct') != None:
+            if cmd.data.get('direct') is not None:
                 block['direct'] = cmd.data['direct']
                 block['type'] = cmd.data['type']
             
             # add target if necessary
             if cmd.data.get('block') != 'event':
                 if cmd.target != 'Default':
                     block['target'] = cmd.target
@@ -142,16 +175,18 @@
                 block['args']['items'].extend(tags)  # add tags to end
 
             mainDict['blocks'].append(block)
 
         print(f'{COL_SUCCESS}Template built successfully.{COL_RESET}')
 
         templateName = 'Unnamed'
-        if not mainDict['blocks'][0]['block'] in TEMPLATE_STARTERS:
+        if mainDict['blocks'][0]['block'] not in TEMPLATE_STARTERS:
             _warn('Template does not start with an event, function, or process.')
+        elif self.name is not None:
+            templateName = self.name
         else:
             try:
                 templateName = mainDict['blocks'][0]['block'] + '_' + mainDict['blocks'][0]['action']
             except KeyError:
                 templateName = mainDict['blocks'][0]['data']
         
         return self._compress(str(mainDict)), templateName
@@ -190,151 +225,142 @@
         Clears this template's data.
         """
         self.__init__()
     
 
     def _openbracket(self, btype: str='norm'):
         bracket = CodeBlock('Bracket', data={'id': 'bracket', 'direct': 'open', 'type': btype})
-        self.commands.append(bracket)
+        self.codeBlocks.append(bracket)
         self.closebracket = btype
     
 
     # command methods
     def playerEvent(self, name: str):
         cmd = CodeBlock(name, data={'id': 'block', 'block': 'event', 'action': name})
-        self.commands.append(cmd)
+        self.codeBlocks.append(cmd)
     
 
     def entityEvent(self, name: str):
         cmd = CodeBlock(name, data={'id': 'block', 'block': 'entity_event', 'action': name})
-        self.commands.append(cmd)
+        self.codeBlocks.append(cmd)
     
 
     def function(self, name: str):
         cmd = CodeBlock('function', data={'id': 'block', 'block': 'func', 'data': name})
-        self.commands.append(cmd)
+        self.codeBlocks.append(cmd)
     
 
     def process(self, name: str):
         cmd = CodeBlock('process', data={'id': 'block', 'block': 'process', 'data': name})
-        self.commands.append(cmd)
+        self.codeBlocks.append(cmd)
     
 
     def callFunction(self, name: str, parameters={}):
         if parameters:
             for key in parameters.keys():
                 self.setVariable('=', var(key, scope='local'), parameters[key])
         
         cmd = CodeBlock('call_func', data={'id': 'block', 'block': 'call_func', 'data': name})
-        self.commands.append(cmd)
+        self.codeBlocks.append(cmd)
     
 
     def startProcess(self, name: str):
         cmd = CodeBlock('start_process', data={'id': 'block', 'block': 'start_process', 'data': name})
-        self.commands.append(cmd)
+        self.codeBlocks.append(cmd)
 
 
     def playerAction(self, name: str, *args, target: str='Default'):
         args = self._convertDataTypes(args)
         cmd = CodeBlock(name, args, target=target, data={'id': 'block', 'block': 'player_action', 'action': name})
-        self.commands.append(cmd)
+        self.codeBlocks.append(cmd)
     
 
     def gameAction(self, name: str, *args):
         args = self._convertDataTypes(args)
         cmd = CodeBlock(name, args, data={'id': 'block', 'block': 'game_action', 'action': name})
-        self.commands.append(cmd)
+        self.codeBlocks.append(cmd)
     
 
     def entityAction(self, name: str, *args):
         args = self._convertDataTypes(args)
         cmd = CodeBlock(name, args, data={'id': 'block', 'block': 'entity_action', 'action': name})
-        self.commands.append(cmd)
+        self.codeBlocks.append(cmd)
     
 
     def ifPlayer(self, name: str, *args, target: str='Default'):
         args = self._convertDataTypes(args)
         cmd = CodeBlock(name, args, target=target, data={'id': 'block', 'block': 'if_player', 'action': name})
-        self.commands.append(cmd)
+        self.codeBlocks.append(cmd)
         self._openbracket()
     
 
     def ifVariable(self, name: str, *args):
         args = self._convertDataTypes(args)
         cmd = CodeBlock(name, args, data={'id': 'block', 'block': 'if_var', 'action': name})
-        self.commands.append(cmd)
+        self.codeBlocks.append(cmd)
         self._openbracket()
     
 
     def ifGame(self, name: str, *args):
         args = self._convertDataTypes(args)
         cmd = CodeBlock(name, args, data={'id': 'block', 'block': 'if_game', 'action': name})
-        self.commands.append(cmd)
+        self.codeBlocks.append(cmd)
         self._openbracket()
     
 
     def ifEntity(self, name: str, *args):
         args = self._convertDataTypes(args)
         cmd = CodeBlock(name, args, data={'id': 'block', 'block': 'if_entity', 'action': name})
-        self.commands.append(cmd)
+        self.codeBlocks.append(cmd)
         self._openbracket()
 
 
     def else_(self):
         cmd = CodeBlock('else', data={'id': 'block', 'block': 'else'})
-        self.commands.append(cmd)
+        self.codeBlocks.append(cmd)
         self._openbracket()
     
 
     def repeat(self, name: str, *args, subAction: str=None):
         args = self._convertDataTypes(args)
         data = {'id': 'block', 'block': 'repeat', 'action': name}
         if subAction is not None:
             data['subAction'] = subAction
         cmd = CodeBlock(name, args, data=data)
-        self.commands.append(cmd)
+        self.codeBlocks.append(cmd)
         self._openbracket('repeat')
 
 
     def bracket(self, *args):
         args = self._convertDataTypes(args)
         cmd = CodeBlock('Bracket', data={'id': 'bracket', 'direct': 'close', 'type': self.closebracket})
-        self.commands.append(cmd)
+        self.codeBlocks.append(cmd)
     
 
     def control(self, name: str, *args):
         args = self._convertDataTypes(args)
         cmd = CodeBlock(name, args, data={'id': 'block', 'block': 'control', 'action': name})
-        self.commands.append(cmd)
+        self.codeBlocks.append(cmd)
     
 
     def selectObject(self, name: str, *args):
         args = self._convertDataTypes(args)
         cmd = CodeBlock(name, args, data={'id': 'block', 'block': 'select_obj', 'action': name})
-        self.commands.append(cmd)
+        self.codeBlocks.append(cmd)
     
 
     def setVariable(self, name: str, *args):
         args = self._convertDataTypes(args)
         cmd = CodeBlock(name, args, data={'id': 'block', 'block': 'set_var', 'action': name})
-        self.commands.append(cmd)
+        self.codeBlocks.append(cmd)
     
 
-    # extra methods
     def return_(self, returndata={}):
         for key in returndata:
             self.setVariable('=', var(key, scope='local'), returndata[key])
         self.control('Return')
     
 
     def define_(self, name: str, value=0, scope: str='unsaved', createSetVar: bool=True):
         if createSetVar:
             self.setVariable('=', var(name, scope=scope), value)
-        self.definedVars[name] = var(name, scope=scope)
-
-
-class CodeBlock:
-    def __init__(self, name: str, *args, target: str='Default', data={}):
-        self.name = name
-        self.args = args
-        self.target = target
-        self.data = data
+        self.definedVars[name] = var(name, scope=scope)
```

