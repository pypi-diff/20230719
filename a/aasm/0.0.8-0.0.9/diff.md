# Comparing `tmp/aasm-0.0.8.tar.gz` & `tmp/aasm-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aasm-0.0.8.tar", last modified: Sun Dec 26 01:07:06 2021, max compression
+gzip compressed data, was "aasm-0.0.9.tar", last modified: Sun Dec 26 01:26:51 2021, max compression
```

## Comparing `aasm-0.0.8.tar` & `aasm-0.0.9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0       25 2021-12-08 01:21:36.000000 aasm-0.0.8/.gitignore
--rw-r--r--   0        0        0      281 2021-12-23 00:23:12.642979 aasm-0.0.8/Pipfile
--rw-r--r--   0        0        0    45740 2021-12-23 00:23:12.646312 aasm-0.0.8/Pipfile.lock
--rw-r--r--   0        0        0     1927 2021-12-24 00:13:54.375367 aasm-0.0.8/README.md
--rw-r--r--   0        0        0      199 2021-12-26 01:06:40.501656 aasm-0.0.8/aasm/__init__.py
--rw-r--r--   0        0        0        0 2021-12-08 01:37:55.000000 aasm-0.0.8/aasm/generating/__init__.py
--rw-r--r--   0        0        0      841 2021-12-25 20:05:31.052167 aasm-0.0.8/aasm/generating/code.py
--rw-r--r--   0        0        0      696 2021-12-25 20:05:31.052167 aasm-0.0.8/aasm/generating/python_code.py
--rw-r--r--   0        0        0     3173 2021-12-26 01:06:40.504990 aasm-0.0.8/aasm/generating/python_graph.py
--rw-r--r--   0        0        0    20486 2021-12-25 21:43:20.387973 aasm-0.0.8/aasm/generating/python_spade.py
--rw-r--r--   0        0        0        0 2021-12-08 01:37:55.000000 aasm-0.0.8/aasm/intermediate/__init__.py
--rw-r--r--   0        0        0     1993 2021-12-08 01:37:55.000000 aasm-0.0.8/aasm/intermediate/action.py
--rw-r--r--   0        0        0     7612 2021-12-25 20:05:31.052167 aasm-0.0.8/aasm/intermediate/agent.py
--rw-r--r--   0        0        0    11623 2021-12-24 00:13:54.375367 aasm-0.0.8/aasm/intermediate/argument.py
--rw-r--r--   0        0        0     1391 2021-12-08 01:37:55.000000 aasm-0.0.8/aasm/intermediate/behaviour.py
--rw-r--r--   0        0        0     1065 2021-12-08 01:37:55.000000 aasm-0.0.8/aasm/intermediate/block.py
--rw-r--r--   0        0        0      400 2021-12-08 01:37:55.000000 aasm-0.0.8/aasm/intermediate/declaration.py
--rw-r--r--   0        0        0     2484 2021-12-24 00:13:54.375367 aasm-0.0.8/aasm/intermediate/graph.py
--rw-r--r--   0        0        0     7019 2021-12-08 01:37:55.000000 aasm-0.0.8/aasm/intermediate/instruction.py
--rw-r--r--   0        0        0     1790 2021-12-08 01:37:55.000000 aasm-0.0.8/aasm/intermediate/message.py
--rw-r--r--   0        0        0        0 2021-12-08 01:37:55.000000 aasm-0.0.8/aasm/parsing/__init__.py
--rw-r--r--   0        0        0        0 2021-12-08 01:37:55.000000 aasm-0.0.8/aasm/parsing/op/__init__.py
--rw-r--r--   0        0        0     2060 2021-12-08 01:37:55.000000 aasm-0.0.8/aasm/parsing/op/action.py
--rw-r--r--   0        0        0     1389 2021-12-24 00:13:54.375367 aasm-0.0.8/aasm/parsing/op/agent.py
--rw-r--r--   0        0        0     2917 2021-12-25 20:05:31.052167 aasm-0.0.8/aasm/parsing/op/behav.py
--rw-r--r--   0        0        0      574 2021-12-08 01:37:55.000000 aasm-0.0.8/aasm/parsing/op/clr.py
--rw-r--r--   0        0        0     3002 2021-12-08 01:37:55.000000 aasm-0.0.8/aasm/parsing/op/conditional.py
--rw-r--r--   0        0        0     1220 2021-12-08 01:37:55.000000 aasm-0.0.8/aasm/parsing/op/decl.py
--rw-r--r--   0        0        0     2662 2021-12-24 00:13:54.375367 aasm-0.0.8/aasm/parsing/op/defg.py
--rw-r--r--   0        0        0      413 2021-12-08 01:37:55.000000 aasm-0.0.8/aasm/parsing/op/eblock.py
--rw-r--r--   0        0        0     1392 2021-12-24 00:13:54.375367 aasm-0.0.8/aasm/parsing/op/graph.py
--rw-r--r--   0        0        0      681 2021-12-08 01:37:55.000000 aasm-0.0.8/aasm/parsing/op/len.py
--rw-r--r--   0        0        0     1801 2021-12-08 01:37:55.000000 aasm-0.0.8/aasm/parsing/op/list.py
--rw-r--r--   0        0        0     1096 2021-12-08 01:37:55.000000 aasm-0.0.8/aasm/parsing/op/math.py
--rw-r--r--   0        0        0     1570 2021-12-24 00:13:54.375367 aasm-0.0.8/aasm/parsing/op/message.py
--rw-r--r--   0        0        0     4013 2021-12-25 20:05:31.052167 aasm-0.0.8/aasm/parsing/op/prm.py
--rw-r--r--   0        0        0     2284 2021-12-08 01:37:55.000000 aasm-0.0.8/aasm/parsing/op/rand.py
--rw-r--r--   0        0        0      722 2021-12-08 01:37:55.000000 aasm-0.0.8/aasm/parsing/op/remen.py
--rw-r--r--   0        0        0      575 2021-12-08 01:37:55.000000 aasm-0.0.8/aasm/parsing/op/round.py
--rw-r--r--   0        0        0      819 2021-12-08 01:37:55.000000 aasm-0.0.8/aasm/parsing/op/send.py
--rw-r--r--   0        0        0      678 2021-12-08 01:37:55.000000 aasm-0.0.8/aasm/parsing/op/set.py
--rw-r--r--   0        0        0      579 2021-12-24 00:13:54.375367 aasm-0.0.8/aasm/parsing/op/size.py
--rw-r--r--   0        0        0      794 2021-12-08 01:37:55.000000 aasm-0.0.8/aasm/parsing/op/subs.py
--rw-r--r--   0        0        0     4891 2021-12-24 00:13:54.375367 aasm-0.0.8/aasm/parsing/parse.py
--rw-r--r--   0        0        0     4227 2021-12-24 00:13:54.375367 aasm-0.0.8/aasm/parsing/state.py
--rw-r--r--   0        0        0     1632 2021-12-25 20:05:31.055501 aasm-0.0.8/aasm/translate.py
--rw-r--r--   0        0        0        0 2021-12-08 01:37:55.000000 aasm-0.0.8/aasm/utils/__init__.py
--rw-r--r--   0        0        0      428 2021-12-08 02:46:46.000000 aasm-0.0.8/aasm/utils/exception.py
--rw-r--r--   0        0        0     1302 2021-12-25 20:05:31.055501 aasm-0.0.8/aasm/utils/validation.py
--rw-r--r--   0        0        0     2243 2021-12-26 01:06:40.504990 aasm-0.0.8/out
--rw-r--r--   0        0        0      273 2021-12-08 01:19:10.000000 aasm-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      413 2021-12-25 21:36:52.089081 aasm-0.0.8/test.aa
--rw-r--r--   0        0        0     2085 1970-01-01 00:00:00.000000 aasm-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       25 2021-12-08 01:21:36.000000 aasm-0.0.9/.gitignore
+-rw-r--r--   0        0        0      281 2021-12-23 00:23:12.642979 aasm-0.0.9/Pipfile
+-rw-r--r--   0        0        0    45740 2021-12-23 00:23:12.646312 aasm-0.0.9/Pipfile.lock
+-rw-r--r--   0        0        0     2116 2021-12-26 01:22:21.030054 aasm-0.0.9/README.md
+-rw-r--r--   0        0        0      199 2021-12-26 01:23:38.713816 aasm-0.0.9/aasm/__init__.py
+-rw-r--r--   0        0        0        0 2021-12-08 01:37:55.000000 aasm-0.0.9/aasm/generating/__init__.py
+-rw-r--r--   0        0        0      841 2021-12-25 20:05:31.052167 aasm-0.0.9/aasm/generating/code.py
+-rw-r--r--   0        0        0      696 2021-12-25 20:05:31.052167 aasm-0.0.9/aasm/generating/python_code.py
+-rw-r--r--   0        0        0     3112 2021-12-26 01:16:06.464684 aasm-0.0.9/aasm/generating/python_graph.py
+-rw-r--r--   0        0        0    20486 2021-12-25 21:43:20.387973 aasm-0.0.9/aasm/generating/python_spade.py
+-rw-r--r--   0        0        0        0 2021-12-08 01:37:55.000000 aasm-0.0.9/aasm/intermediate/__init__.py
+-rw-r--r--   0        0        0     1993 2021-12-08 01:37:55.000000 aasm-0.0.9/aasm/intermediate/action.py
+-rw-r--r--   0        0        0     7612 2021-12-25 20:05:31.052167 aasm-0.0.9/aasm/intermediate/agent.py
+-rw-r--r--   0        0        0    11623 2021-12-24 00:13:54.375367 aasm-0.0.9/aasm/intermediate/argument.py
+-rw-r--r--   0        0        0     1391 2021-12-08 01:37:55.000000 aasm-0.0.9/aasm/intermediate/behaviour.py
+-rw-r--r--   0        0        0     1065 2021-12-08 01:37:55.000000 aasm-0.0.9/aasm/intermediate/block.py
+-rw-r--r--   0        0        0      400 2021-12-08 01:37:55.000000 aasm-0.0.9/aasm/intermediate/declaration.py
+-rw-r--r--   0        0        0     2484 2021-12-24 00:13:54.375367 aasm-0.0.9/aasm/intermediate/graph.py
+-rw-r--r--   0        0        0     7019 2021-12-08 01:37:55.000000 aasm-0.0.9/aasm/intermediate/instruction.py
+-rw-r--r--   0        0        0     1790 2021-12-08 01:37:55.000000 aasm-0.0.9/aasm/intermediate/message.py
+-rw-r--r--   0        0        0        0 2021-12-08 01:37:55.000000 aasm-0.0.9/aasm/parsing/__init__.py
+-rw-r--r--   0        0        0        0 2021-12-08 01:37:55.000000 aasm-0.0.9/aasm/parsing/op/__init__.py
+-rw-r--r--   0        0        0     2060 2021-12-08 01:37:55.000000 aasm-0.0.9/aasm/parsing/op/action.py
+-rw-r--r--   0        0        0     1389 2021-12-24 00:13:54.375367 aasm-0.0.9/aasm/parsing/op/agent.py
+-rw-r--r--   0        0        0     2917 2021-12-25 20:05:31.052167 aasm-0.0.9/aasm/parsing/op/behav.py
+-rw-r--r--   0        0        0      574 2021-12-08 01:37:55.000000 aasm-0.0.9/aasm/parsing/op/clr.py
+-rw-r--r--   0        0        0     3002 2021-12-08 01:37:55.000000 aasm-0.0.9/aasm/parsing/op/conditional.py
+-rw-r--r--   0        0        0     1220 2021-12-08 01:37:55.000000 aasm-0.0.9/aasm/parsing/op/decl.py
+-rw-r--r--   0        0        0     2662 2021-12-24 00:13:54.375367 aasm-0.0.9/aasm/parsing/op/defg.py
+-rw-r--r--   0        0        0      413 2021-12-08 01:37:55.000000 aasm-0.0.9/aasm/parsing/op/eblock.py
+-rw-r--r--   0        0        0     1392 2021-12-24 00:13:54.375367 aasm-0.0.9/aasm/parsing/op/graph.py
+-rw-r--r--   0        0        0      681 2021-12-08 01:37:55.000000 aasm-0.0.9/aasm/parsing/op/len.py
+-rw-r--r--   0        0        0     1801 2021-12-08 01:37:55.000000 aasm-0.0.9/aasm/parsing/op/list.py
+-rw-r--r--   0        0        0     1096 2021-12-08 01:37:55.000000 aasm-0.0.9/aasm/parsing/op/math.py
+-rw-r--r--   0        0        0     1570 2021-12-24 00:13:54.375367 aasm-0.0.9/aasm/parsing/op/message.py
+-rw-r--r--   0        0        0     4013 2021-12-25 20:05:31.052167 aasm-0.0.9/aasm/parsing/op/prm.py
+-rw-r--r--   0        0        0     2284 2021-12-08 01:37:55.000000 aasm-0.0.9/aasm/parsing/op/rand.py
+-rw-r--r--   0        0        0      722 2021-12-08 01:37:55.000000 aasm-0.0.9/aasm/parsing/op/remen.py
+-rw-r--r--   0        0        0      575 2021-12-08 01:37:55.000000 aasm-0.0.9/aasm/parsing/op/round.py
+-rw-r--r--   0        0        0      819 2021-12-08 01:37:55.000000 aasm-0.0.9/aasm/parsing/op/send.py
+-rw-r--r--   0        0        0      678 2021-12-08 01:37:55.000000 aasm-0.0.9/aasm/parsing/op/set.py
+-rw-r--r--   0        0        0      579 2021-12-24 00:13:54.375367 aasm-0.0.9/aasm/parsing/op/size.py
+-rw-r--r--   0        0        0      794 2021-12-08 01:37:55.000000 aasm-0.0.9/aasm/parsing/op/subs.py
+-rw-r--r--   0        0        0     4891 2021-12-24 00:13:54.375367 aasm-0.0.9/aasm/parsing/parse.py
+-rw-r--r--   0        0        0     4227 2021-12-24 00:13:54.375367 aasm-0.0.9/aasm/parsing/state.py
+-rw-r--r--   0        0        0     1632 2021-12-25 20:05:31.055501 aasm-0.0.9/aasm/translate.py
+-rw-r--r--   0        0        0        0 2021-12-08 01:37:55.000000 aasm-0.0.9/aasm/utils/__init__.py
+-rw-r--r--   0        0        0      428 2021-12-08 02:46:46.000000 aasm-0.0.9/aasm/utils/exception.py
+-rw-r--r--   0        0        0     1302 2021-12-25 20:05:31.055501 aasm-0.0.9/aasm/utils/validation.py
+-rw-r--r--   0        0        0     2219 2021-12-26 01:25:27.754420 aasm-0.0.9/out
+-rw-r--r--   0        0        0      273 2021-12-08 01:19:10.000000 aasm-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      413 2021-12-25 21:36:52.089081 aasm-0.0.9/test.aa
+-rw-r--r--   0        0        0     2271 1970-01-01 00:00:00.000000 aasm-0.0.9/PKG-INFO
```

### Comparing `aasm-0.0.8/Pipfile.lock` & `aasm-0.0.9/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `aasm-0.0.8/README.md` & `aasm-0.0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,18 @@
 ```
 python -m aasm.translate --help
 ```
 
 ## Structure <a name = "structure"></a>
 
 * `generating`
-    * `spade.py` - SPADE code generation from the intermediate representation
+    * `code.py` - generated code
+    * `python_code.py` - Python code base class
+    * `python_graph.py` - Python graph code generation from the intermediate representation
+    * `python_spade.py` - SPADE agent code generation from the intermediate representation
 * `intermediate`
     * `action.py`
     * `agent.py`
     * `argument.py` - arguments used in instructions
     * `behaviour.py`
     * `block.py` - block of code representation
     * `declaration.py` - declarations used in actions
```

### Comparing `aasm-0.0.8/aasm/generating/code.py` & `aasm-0.0.9/aasm/generating/code.py`

 * *Files identical despite different names*

### Comparing `aasm-0.0.8/aasm/generating/python_code.py` & `aasm-0.0.9/aasm/generating/python_code.py`

 * *Files identical despite different names*

### Comparing `aasm-0.0.8/aasm/generating/python_graph.py` & `aasm-0.0.9/aasm/generating/python_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,29 +17,28 @@
         super().__init__(indent_size)
         if graph:
             self.add_required_imports()
             self.add_newlines(2)
             self.generate_graph(graph)
 
     def add_required_imports(self) -> List[str]:
-        self.add_line('import json')
         self.add_line('import random')
         self.add_line('import uuid')
         self.add_line('import numpy')
         
     def generate_graph(self, graph: Graph) -> None:
         if isinstance(graph, StatisticalGraph):
             self.add_statistical_graph(graph)
 
     def add_statistical_graph(self, graph: StatisticalGraph) -> None:
         self.add_line('def generate_graph_structure(domain):')
         self.indent_right()
 
         if not graph.agents:
-            self.add_line('return json.dumps([])')
+            self.add_line('return []')
             self.indent_left()
             return
         
         num_agents = []
         for agent in graph.agents.values():
             if isinstance(agent.amount, AgentConstantAmount):
                 self.add_line(f'_num_{agent.name} = {agent.amount.value}')
@@ -67,9 +66,9 @@
             self.add_line(f'"type": "{agent.name}",')
             self.add_line('"connections": random.sample(jids, num_connections),')
             self.indent_left()
             self.add_line('})')
             self.add_line('next_agent_idx += 1')
             self.indent_left()
         
-        self.add_line('return json.dumps(agents)')
+        self.add_line('return agents')
         self.indent_left()
```

### Comparing `aasm-0.0.8/aasm/generating/python_spade.py` & `aasm-0.0.9/aasm/generating/python_spade.py`

 * *Files identical despite different names*

### Comparing `aasm-0.0.8/aasm/intermediate/action.py` & `aasm-0.0.9/aasm/intermediate/action.py`

 * *Files identical despite different names*

### Comparing `aasm-0.0.8/aasm/intermediate/agent.py` & `aasm-0.0.9/aasm/intermediate/agent.py`

 * *Files identical despite different names*

### Comparing `aasm-0.0.8/aasm/intermediate/argument.py` & `aasm-0.0.9/aasm/intermediate/argument.py`

 * *Files identical despite different names*

### Comparing `aasm-0.0.8/aasm/intermediate/behaviour.py` & `aasm-0.0.9/aasm/intermediate/behaviour.py`

 * *Files identical despite different names*

### Comparing `aasm-0.0.8/aasm/intermediate/block.py` & `aasm-0.0.9/aasm/intermediate/block.py`

 * *Files identical despite different names*

### Comparing `aasm-0.0.8/aasm/intermediate/graph.py` & `aasm-0.0.9/aasm/intermediate/graph.py`

 * *Files identical despite different names*

### Comparing `aasm-0.0.8/aasm/intermediate/instruction.py` & `aasm-0.0.9/aasm/intermediate/instruction.py`

 * *Files identical despite different names*

### Comparing `aasm-0.0.8/aasm/intermediate/message.py` & `aasm-0.0.9/aasm/intermediate/message.py`

 * *Files identical despite different names*

### Comparing `aasm-0.0.8/aasm/parsing/op/action.py` & `aasm-0.0.9/aasm/parsing/op/action.py`

 * *Files identical despite different names*

### Comparing `aasm-0.0.8/aasm/parsing/op/agent.py` & `aasm-0.0.9/aasm/parsing/op/agent.py`

 * *Files identical despite different names*

### Comparing `aasm-0.0.8/aasm/parsing/op/behav.py` & `aasm-0.0.9/aasm/parsing/op/behav.py`

 * *Files identical despite different names*

### Comparing `aasm-0.0.8/aasm/parsing/op/clr.py` & `aasm-0.0.9/aasm/parsing/op/clr.py`

 * *Files identical despite different names*

### Comparing `aasm-0.0.8/aasm/parsing/op/conditional.py` & `aasm-0.0.9/aasm/parsing/op/conditional.py`

 * *Files identical despite different names*

### Comparing `aasm-0.0.8/aasm/parsing/op/decl.py` & `aasm-0.0.9/aasm/parsing/op/decl.py`

 * *Files identical despite different names*

### Comparing `aasm-0.0.8/aasm/parsing/op/defg.py` & `aasm-0.0.9/aasm/parsing/op/defg.py`

 * *Files identical despite different names*

### Comparing `aasm-0.0.8/aasm/parsing/op/graph.py` & `aasm-0.0.9/aasm/parsing/op/graph.py`

 * *Files identical despite different names*

### Comparing `aasm-0.0.8/aasm/parsing/op/len.py` & `aasm-0.0.9/aasm/parsing/op/len.py`

 * *Files identical despite different names*

### Comparing `aasm-0.0.8/aasm/parsing/op/list.py` & `aasm-0.0.9/aasm/parsing/op/list.py`

 * *Files identical despite different names*

### Comparing `aasm-0.0.8/aasm/parsing/op/math.py` & `aasm-0.0.9/aasm/parsing/op/math.py`

 * *Files identical despite different names*

### Comparing `aasm-0.0.8/aasm/parsing/op/message.py` & `aasm-0.0.9/aasm/parsing/op/message.py`

 * *Files identical despite different names*

### Comparing `aasm-0.0.8/aasm/parsing/op/prm.py` & `aasm-0.0.9/aasm/parsing/op/prm.py`

 * *Files identical despite different names*

### Comparing `aasm-0.0.8/aasm/parsing/op/rand.py` & `aasm-0.0.9/aasm/parsing/op/rand.py`

 * *Files identical despite different names*

### Comparing `aasm-0.0.8/aasm/parsing/op/remen.py` & `aasm-0.0.9/aasm/parsing/op/remen.py`

 * *Files identical despite different names*

### Comparing `aasm-0.0.8/aasm/parsing/op/round.py` & `aasm-0.0.9/aasm/parsing/op/round.py`

 * *Files identical despite different names*

### Comparing `aasm-0.0.8/aasm/parsing/op/send.py` & `aasm-0.0.9/aasm/parsing/op/send.py`

 * *Files identical despite different names*

### Comparing `aasm-0.0.8/aasm/parsing/op/set.py` & `aasm-0.0.9/aasm/parsing/op/set.py`

 * *Files identical despite different names*

### Comparing `aasm-0.0.8/aasm/parsing/op/size.py` & `aasm-0.0.9/aasm/parsing/op/size.py`

 * *Files identical despite different names*

### Comparing `aasm-0.0.8/aasm/parsing/op/subs.py` & `aasm-0.0.9/aasm/parsing/op/subs.py`

 * *Files identical despite different names*

### Comparing `aasm-0.0.8/aasm/parsing/parse.py` & `aasm-0.0.9/aasm/parsing/parse.py`

 * *Files identical despite different names*

### Comparing `aasm-0.0.8/aasm/parsing/state.py` & `aasm-0.0.9/aasm/parsing/state.py`

 * *Files identical despite different names*

### Comparing `aasm-0.0.8/aasm/translate.py` & `aasm-0.0.9/aasm/translate.py`

 * *Files identical despite different names*

### Comparing `aasm-0.0.8/aasm/utils/validation.py` & `aasm-0.0.9/aasm/utils/validation.py`

 * *Files identical despite different names*

### Comparing `aasm-0.0.8/out` & `aasm-0.0.9/out`

 * *Files 3% similar despite different names*

```diff
@@ -42,15 +42,14 @@
             for receiver in self.agent.friends:
                 await self.send(self.agent.get_spade_message(receiver, send))
                 self.agent.msgSCount += 1
         
         async def run(self):
             await self.post_photos()
     
-import json
 import random
 import uuid
 import numpy
 
 
 def generate_graph_structure(domain):
     _num_average_user = round(100 / 100 * 150)
@@ -64,8 +63,8 @@
         num_connections = max(min(num_connections, len(jids)), 0)
         agents.append({
             "jid": jids[next_agent_idx],
             "type": "average_user",
             "connections": random.sample(jids, num_connections),
         })
         next_agent_idx += 1
-    return json.dumps(agents)
+    return agents
```

### Comparing `aasm-0.0.8/PKG-INFO` & `aasm-0.0.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aasm
-Version: 0.0.8
+Version: 0.0.9
 Summary: Agents Assembly translator
 Home-page: https://github.com/agent-based-information-flow-simulation/agents-assembly-translator
 Author: unknown
 Description-Content-Type: text/markdown
 
 # Agents Assembly Translator
 
@@ -39,15 +39,18 @@
 ```
 python -m aasm.translate --help
 ```
 
 ## Structure <a name = "structure"></a>
 
 * `generating`
-    * `spade.py` - SPADE code generation from the intermediate representation
+    * `code.py` - generated code
+    * `python_code.py` - Python code base class
+    * `python_graph.py` - Python graph code generation from the intermediate representation
+    * `python_spade.py` - SPADE agent code generation from the intermediate representation
 * `intermediate`
     * `action.py`
     * `agent.py`
     * `argument.py` - arguments used in instructions
     * `behaviour.py`
     * `block.py` - block of code representation
     * `declaration.py` - declarations used in actions
```

