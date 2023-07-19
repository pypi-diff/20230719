# Comparing `tmp/llmreflect-0.0.9.tar.gz` & `tmp/llmreflect-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmreflect-0.0.9.tar", max compression
+gzip compressed data, was "llmreflect-0.1.4.tar", max compression
```

## Comparing `llmreflect-0.0.9.tar` & `llmreflect-0.1.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     4061 2023-07-13 17:26:37.828872 llmreflect-0.0.9/README.md
--rw-r--r--   0        0        0     3957 2023-07-13 17:26:37.828872 llmreflect-0.0.9/llmreflect/Agents/BasicAgent.py
--rw-r--r--   0        0        0     2570 2023-07-13 17:26:37.828872 llmreflect-0.0.9/llmreflect/Agents/EvaluationAgent.py
--rw-r--r--   0        0        0     3092 2023-07-13 17:26:37.828872 llmreflect-0.0.9/llmreflect/Agents/ModerateAgent.py
--rw-r--r--   0        0        0     9630 2023-07-13 17:26:37.828872 llmreflect-0.0.9/llmreflect/Agents/PostgresqlAgent.py
--rw-r--r--   0        0        0     2278 2023-07-13 17:26:37.828872 llmreflect-0.0.9/llmreflect/Agents/QuestionAgent.py
--rw-r--r--   0        0        0        0 2023-07-13 17:26:37.828872 llmreflect-0.0.9/llmreflect/Agents/__init__.py
--rw-r--r--   0        0        0     2679 2023-07-13 17:26:37.828872 llmreflect-0.0.9/llmreflect/Chains/BasicChain.py
--rw-r--r--   0        0        0    21670 2023-07-13 17:26:37.828872 llmreflect-0.0.9/llmreflect/Chains/DatabaseChain.py
--rw-r--r--   0        0        0     1786 2023-07-13 17:26:37.828872 llmreflect-0.0.9/llmreflect/Chains/ModerateChain.py
--rw-r--r--   0        0        0        0 2023-07-13 17:26:37.828872 llmreflect-0.0.9/llmreflect/Chains/__init__.py
--rw-r--r--   0        0        0     8457 2023-07-13 17:26:37.828872 llmreflect-0.0.9/llmreflect/Prompt/BasicPrompt.py
--rw-r--r--   0        0        0        0 2023-07-13 17:26:37.828872 llmreflect-0.0.9/llmreflect/Prompt/__init__.py
--rw-r--r--   0        0        0     2807 2023-07-13 17:26:37.828872 llmreflect-0.0.9/llmreflect/Prompt/promptbase/gradingpostgresql.json
--rw-r--r--   0        0        0     2366 2023-07-13 17:26:37.828872 llmreflect-0.0.9/llmreflect/Prompt/promptbase/moderatepostgresql.json
--rw-r--r--   0        0        0     4951 2023-07-13 17:26:37.828872 llmreflect-0.0.9/llmreflect/Prompt/promptbase/postgresql.json
--rw-r--r--   0        0        0     1119 2023-07-13 17:26:37.828872 llmreflect-0.0.9/llmreflect/Prompt/promptbase/postgresqlfix.json
--rw-r--r--   0        0        0     2084 2023-07-13 17:26:37.828872 llmreflect-0.0.9/llmreflect/Prompt/promptbase/questionpostgresql.json
--rw-r--r--   0        0        0     2079 2023-07-13 17:26:37.828872 llmreflect-0.0.9/llmreflect/Retriever/BasicRetriever.py
--rw-r--r--   0        0        0     4219 2023-07-13 17:26:37.828872 llmreflect-0.0.9/llmreflect/Retriever/DatabaseRetriever.py
--rw-r--r--   0        0        0        0 2023-07-13 17:26:37.828872 llmreflect-0.0.9/llmreflect/Retriever/__init__.py
--rw-r--r--   0        0        0        0 2023-07-13 17:26:37.828872 llmreflect-0.0.9/llmreflect/Tests/__init__.py
--rw-r--r--   0        0        0     8035 2023-07-13 17:26:37.828872 llmreflect-0.0.9/llmreflect/Tests/test_chains.py
--rw-r--r--   0        0        0      442 2023-07-13 17:26:37.828872 llmreflect-0.0.9/llmreflect/Tests/test_prompt.py
--rw-r--r--   0        0        0        0 2023-07-13 17:26:37.828872 llmreflect-0.0.9/llmreflect/Utils/__init__.py
--rw-r--r--   0        0        0      690 2023-07-13 17:26:37.828872 llmreflect-0.0.9/llmreflect/Utils/database.py
--rw-r--r--   0        0        0     9631 2023-07-13 17:26:37.828872 llmreflect-0.0.9/llmreflect/Utils/log.py
--rw-r--r--   0        0        0        0 2023-07-13 17:26:37.828872 llmreflect-0.0.9/llmreflect/__init__.py
--rw-r--r--   0        0        0      478 2023-07-13 17:26:37.832872 llmreflect-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     4779 1970-01-01 00:00:00.000000 llmreflect-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     4061 2023-07-19 14:48:46.233593 llmreflect-0.1.4/README.md
+-rw-r--r--   0        0        0     9214 2023-07-19 14:48:46.233593 llmreflect-0.1.4/llmreflect/Agents/BasicAgent.py
+-rw-r--r--   0        0        0     9611 2023-07-19 14:48:46.233593 llmreflect-0.1.4/llmreflect/Agents/DatabaseAgent.py
+-rw-r--r--   0        0        0     2602 2023-07-19 14:48:46.233593 llmreflect-0.1.4/llmreflect/Agents/EvaluationAgent.py
+-rw-r--r--   0        0        0     3204 2023-07-19 14:48:46.233593 llmreflect-0.1.4/llmreflect/Agents/ModerateAgent.py
+-rw-r--r--   0        0        0     2331 2023-07-19 14:48:46.233593 llmreflect-0.1.4/llmreflect/Agents/QuestionAgent.py
+-rw-r--r--   0        0        0        0 2023-07-19 14:48:46.233593 llmreflect-0.1.4/llmreflect/Agents/__init__.py
+-rw-r--r--   0        0        0     3230 2023-07-19 14:48:46.233593 llmreflect-0.1.4/llmreflect/Chains/BasicChain.py
+-rw-r--r--   0        0        0    31092 2023-07-19 14:48:46.233593 llmreflect-0.1.4/llmreflect/Chains/DatabaseChain.py
+-rw-r--r--   0        0        0     2675 2023-07-19 14:48:46.233593 llmreflect-0.1.4/llmreflect/Chains/ModerateChain.py
+-rw-r--r--   0        0        0        0 2023-07-19 14:48:46.233593 llmreflect-0.1.4/llmreflect/Chains/__init__.py
+-rw-r--r--   0        0        0     8457 2023-07-19 14:48:46.233593 llmreflect-0.1.4/llmreflect/Prompt/BasicPrompt.py
+-rw-r--r--   0        0        0        0 2023-07-19 14:48:46.233593 llmreflect-0.1.4/llmreflect/Prompt/__init__.py
+-rw-r--r--   0        0        0     4950 2023-07-19 14:48:46.233593 llmreflect-0.1.4/llmreflect/Prompt/promptbase/answer_database.json
+-rw-r--r--   0        0        0     1119 2023-07-19 14:48:46.233593 llmreflect-0.1.4/llmreflect/Prompt/promptbase/fix_database.json
+-rw-r--r--   0        0        0     2803 2023-07-19 14:48:46.233593 llmreflect-0.1.4/llmreflect/Prompt/promptbase/grading_database.json
+-rw-r--r--   0        0        0     2366 2023-07-19 14:48:46.233593 llmreflect-0.1.4/llmreflect/Prompt/promptbase/moderate_database.json
+-rw-r--r--   0        0        0     2082 2023-07-19 14:48:46.233593 llmreflect-0.1.4/llmreflect/Prompt/promptbase/question_database.json
+-rw-r--r--   0        0        0     2079 2023-07-19 14:48:46.233593 llmreflect-0.1.4/llmreflect/Retriever/BasicRetriever.py
+-rw-r--r--   0        0        0     7298 2023-07-19 14:48:46.233593 llmreflect-0.1.4/llmreflect/Retriever/DatabaseRetriever.py
+-rw-r--r--   0        0        0        0 2023-07-19 14:48:46.233593 llmreflect-0.1.4/llmreflect/Retriever/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-19 14:48:46.233593 llmreflect-0.1.4/llmreflect/Tests/__init__.py
+-rw-r--r--   0        0        0     8996 2023-07-19 14:48:46.233593 llmreflect-0.1.4/llmreflect/Tests/test_chains.py
+-rw-r--r--   0        0        0      444 2023-07-19 14:48:46.233593 llmreflect-0.1.4/llmreflect/Tests/test_prompt.py
+-rw-r--r--   0        0        0        0 2023-07-19 14:48:46.233593 llmreflect-0.1.4/llmreflect/Utils/__init__.py
+-rw-r--r--   0        0        0      688 2023-07-19 14:48:46.233593 llmreflect-0.1.4/llmreflect/Utils/database.py
+-rw-r--r--   0        0        0    12398 2023-07-19 14:48:46.233593 llmreflect-0.1.4/llmreflect/Utils/log.py
+-rw-r--r--   0        0        0        0 2023-07-19 14:48:46.233593 llmreflect-0.1.4/llmreflect/__init__.py
+-rw-r--r--   0        0        0      499 2023-07-19 14:48:46.233593 llmreflect-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4820 1970-01-01 00:00:00.000000 llmreflect-0.1.4/PKG-INFO
```

### Comparing `llmreflect-0.0.9/README.md` & `llmreflect-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.9/llmreflect/Agents/EvaluationAgent.py` & `llmreflect-0.1.4/llmreflect/Agents/EvaluationAgent.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,42 @@
 from llmreflect.Agents.BasicAgent import OpenAIAgent
-from llmreflect.Retriever.BasicRetriever import BasicEvaluationRetriever
+from llmreflect.Retriever.DatabaseRetriever import DatabaseEvaluationRetriever
 
 
-class PostgressqlGradingAgent(OpenAIAgent):
+class DatabaseGradingAgent(OpenAIAgent):
     """
-    This is the agent class use for grading postgresql generation.
-    Args:
-        Agent (_type_): _description_
+    This is the agent class use for grading database command generation.
     """
     def __init__(self, open_ai_key: str,
-                 prompt_name: str = 'gradingpostgresql',
+                 prompt_name: str = 'grading_database',
                  max_output_tokens: int = 512,
                  temperature: float = 0.0):
         """
-        Agent class for grading the performance of postgresql generator.
+        Agent class for grading the performance of database command generator.
         Args:
             open_ai_key (str): API key to connect to chatgpt service.
             prompt_name (str, optional): name for the prompt json file.
-                Defaults to 'gradingpostgresql'.
+                Defaults to 'grading_database'.
             max_output_tokens (int, optional): maximum completion length.
                 Defaults to 512.
             temperature (float, optional): how consistent the llm performs.
                 The lower the more consistent. Defaults to 0.0.
         """
         super().__init__(open_ai_key=open_ai_key,
                          prompt_name=prompt_name,
                          max_output_tokens=max_output_tokens,
                          temperature=temperature)
 
-    def equip_retriever(self, retriever: BasicEvaluationRetriever):
+    def equip_retriever(self, retriever: DatabaseEvaluationRetriever):
         object.__setattr__(self, 'retriever', retriever)
 
     def grade(self, request: str, sql_cmd: str, db_summary: str) -> dict:
         """
         Convert LLM output into a score and an explanation.
-        Detailed work done by the BasicEvaluationRetriever.
+        Detailed work done by the DatabaseEvaluationRetriever.
         Args:
             request (str): user's input, natural language for querying db
             sql_cmd (str): sql command generated from LLM
             db_summary (str): a brief report for the query summarized by
             retriever.
 
         Returns:
@@ -48,15 +46,16 @@
         if self.retriever is None:
             self.logger.error("Error: Retriever is not equipped.")
         else:
             try:
                 llm_output = self.predict(
                     request=request,
                     command=sql_cmd,
-                    summary=db_summary
+                    summary=db_summary,
+                    dialect=self.retriever.database_dialect
                 )
                 self.logger.debug(llm_output)
                 result = self.retriever.retrieve(llm_output)
             except Exception as e:
                 self.logger.error(str(e))
                 self.logger.error(llm_output)
         return result
```

### Comparing `llmreflect-0.0.9/llmreflect/Agents/ModerateAgent.py` & `llmreflect-0.1.4/llmreflect/Agents/ModerateAgent.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,81 +1,81 @@
 from llmreflect.Agents.BasicAgent import OpenAIAgent
 from llmreflect.Retriever.BasicRetriever import \
     BasicQuestionModerateRetriever
 
 
-class PostgresqlModerateAgent(OpenAIAgent):
+class DatabaseModerateAgent(OpenAIAgent):
     """
     Agent for filtering out illegal and malicious requests.
-    Args:
-        Agent (_type_): _description_
     """
     def __init__(self, open_ai_key: str,
-                 prompt_name: str = 'moderatepostgresql',
+                 prompt_name: str = 'moderate_database',
                  max_output_tokens: int = 512,
-                 temperature: float = 0.0):
+                 temperature: float = 0.0,
+                 database_topic: str = 'patient data'):
         """
         Agent for filtering out illegal and malicious requests.
         Args:
             open_ai_key (str): API key to connect to chatgpt service.
             prompt_name (str, optional): name for the prompt json file.
-                Defaults to 'moderatepostgresql'.
+                Defaults to 'moderate_database'.
             max_output_tokens (int, optional): maximum completion length.
                 Defaults to 512.
             temperature (float, optional): how consistent the llm performs.
                 The lower the more consistent. To obtain diverse questions,
                 a high temperature is recommended.
                 Defaults to 0.0.
         """
         super().__init__(open_ai_key=open_ai_key,
                          prompt_name=prompt_name,
                          max_output_tokens=max_output_tokens,
                          temperature=temperature)
+        object.__setattr__(self, 'database_topic', database_topic)
 
     def equip_retriever(self, retriever: BasicQuestionModerateRetriever):
         # notice it requires DatabaseQuestionModerateRetriever
         object.__setattr__(self, 'retriever', retriever)
 
     def predict_decision_only(self, user_input: str) -> bool:
         """
         predict whether accept the request or not
         Args:
-            user_input (str): _description_
+            user_input (str): User's natural language input
 
         Returns:
             bool: boolean answer, true or false
         """
         result = "Failed, no output from LLM."
         if self.retriever is None:
             self.logger.error("Error: Retriever is not equipped.")
         else:
             llm_output = self.predict(
-                topic="patient data",
+                topic=self.database_topic,
                 included_tables=self.retriever.include_tables,
                 request=user_input
             )
             self.logger.debug(llm_output)
             result = self.retriever.retrieve(llm_output)['decision']
         return result
 
     def predict_decision_explained(self, user_input: str) -> dict:
         """
         predict judgement with explanation
         Args:
-            user_input (str): _description_
+            user_input (str): User's natural language input
 
         Returns:
             dict: {'decision': bool, 'explanation': str}
         """
         result = "Failed, no output from LLM."
         if self.retriever is None:
             self.logger.error("Error: Retriever is not equipped.")
         else:
             llm_output = self.predict(
-                topic="patient data",
+                topic=self.database_topic,
                 included_tables=self.retriever.include_tables,
                 request=user_input
             )
             self.logger.debug(llm_output)
             result = self.retriever.retrieve(llm_output,
                                              explanation=True)
         return result
```

### Comparing `llmreflect-0.0.9/llmreflect/Agents/PostgresqlAgent.py` & `llmreflect-0.1.4/llmreflect/Agents/DatabaseAgent.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 from llmreflect.Agents.BasicAgent import OpenAIAgent
 from llmreflect.Retriever.DatabaseRetriever import DatabaseRetriever
 from typing import Any
 
 
-class PostgresqlAgent(OpenAIAgent):
+class DatabaseAgent(OpenAIAgent):
     """
-    Agent class for executing postgresql command
+    Agent class for executing database query command
     Args:
         Agent (_type_): _description_
     """
     def __init__(self, open_ai_key: str,
-                 prompt_name: str = 'postgresql',
+                 prompt_name: str = 'answer_database',
                  max_output_tokens: int = 512,
                  temperature: float = 0.0,
                  split_symbol="[answer]"):
         """
         Agent class for querying database.
         Args:
             open_ai_key (str): API key to connect to chatgpt service.
             prompt_name (str, optional): name for the prompt json file.
-                Defaults to 'postgressql'.
+                Defaults to 'answer_database'.
             max_output_tokens (int, optional): maximum completion length.
                 Defaults to 512.
             temperature (float, optional): how consistent the llm performs.
                 The lower the more consistent. Defaults to 0.0.
+            split_symbol (str, optional): the string used for splitting answers
         """
         super().__init__(open_ai_key=open_ai_key,
                          prompt_name=prompt_name,
                          max_output_tokens=max_output_tokens,
                          temperature=temperature)
         object.__setattr__(self, 'split_symbol', split_symbol)
 
@@ -37,15 +38,15 @@
         Args:
             retriever (DatabaseRetriever): use database retriever
         """
         object.__setattr__(self, 'retriever', retriever)
 
     def predict_sql_cmd(self, user_input: str) -> str:
         """
-        Generate the postgresql command, it is a gross output which means
+        Generate the database command, it is a gross output which means
         no post processing. It could be a wrong format that not executable.
         Need extraction and cleaning and formatting.
         Args:
             user_input (str): users description for the query.
 
         Returns:
             str: gross output of the llm attempt for generating sql cmd.
@@ -78,16 +79,14 @@
         Returns:
             str: I know its odd but it is a string. It converts the
             database cursor result into a string. Not very useful, I dont
             know why Im keeping this method.
         """
         assert get_cmd or get_summary or get_db, "At least get one thing"
         llm_output = self.predict_sql_cmd(user_input=user_input)
-        # llm_output = llm_output.replace("tb_", "")
-        # # intentionally causing error for testing
         cmd_n_summary = self.retriever.retrieve_summary(
             llm_output=llm_output,
             return_cmd=True,
             split_symbol=self.split_symbol)
 
         cmd = cmd_n_summary['cmd']
         summary = cmd_n_summary['summary']
@@ -128,20 +127,19 @@
         result = self.retriever.retrieve_summary(
             llm_output=llm_output,
             return_cmd=return_cmd,
             split_symbol=self.split_symbol)
         return result
 
 
-class PostgresqlSelfFixAgent(PostgresqlAgent):
-
+class DatabaseSelfFixAgent(DatabaseAgent):
     def predict_sql_cmd(self, user_input: str, history: str,
                         his_error: str) -> str:
         """
-        Generate the postgresql command, it is a gross output which means
+        Generate a database query command, it is a gross output which means
         no post processing. It could be a wrong format that not executable.
         Need extraction and cleaning and formatting.
         Args:
             user_input (str): users description for the query.
             history (str): history command used for query
             his_error (str): the errors raised from executing the history cmd
         Returns:
```

### Comparing `llmreflect-0.0.9/llmreflect/Agents/QuestionAgent.py` & `llmreflect-0.1.4/llmreflect/Agents/QuestionAgent.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from llmreflect.Agents.BasicAgent import OpenAIAgent
 from llmreflect.Retriever.DatabaseRetriever import DatabaseQuestionRetriever
 
 
-class PostgresqlQuestionAgent(OpenAIAgent):
+class DatabaseQuestionAgent(OpenAIAgent):
     """
     Agent for creating questions based on a given database
     Args:
         Agent (_type_): _description_
     """
     def __init__(self, open_ai_key: str,
-                 prompt_name: str = 'questionpostgresql',
+                 prompt_name: str = 'question_database',
                  max_output_tokens: int = 512,
                  temperature: float = 0.7):
         """
         Agent for creating questions based on a given database
         Args:
             open_ai_key (str): API key to connect to chatgpt service.
             prompt_name (str, optional): name for the prompt json file.
-                Defaults to 'questionpostgresql'.
+                Defaults to 'question_database'.
             max_output_tokens (int, optional): maximum completion length.
                 Defaults to 512.
             temperature (float, optional): how consistent the llm performs.
                 The lower the more consistent. To obtain diverse questions,
                 a high temperature is recommended.
                 Defaults to 0.0.
         """
@@ -46,12 +46,13 @@
         """
         result = "Failed, no output from LLM."
         if self.retriever is None:
             self.logger.error("Error: Retriever is not equipped.")
         else:
             llm_output = self.predict(
                 table_info=self.retriever.table_info,
-                n_questions=n_questions
+                n_questions=n_questions,
+                dialect=self.retriever.database_dialect
             )
             self.logger.debug(llm_output)
             result = self.retriever.retrieve(llm_output)
         return result
```

### Comparing `llmreflect-0.0.9/llmreflect/Chains/BasicChain.py` & `llmreflect-0.1.4/llmreflect/Chains/BasicChain.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,46 +11,68 @@
 class BasicChain(ABC):
     '''
     Abstract class for Chain class.
     A chain class should be the atomic unit for completing a job.
     A chain contains at least two components:
     1. an agent 2. a retriever
     A chain object must have the function to perform a job.
+    Each chain is also equipped with a logger
     '''
     def __init__(self, agent: Agent, retriever: BasicRetriever):
         object.__setattr__(self, 'agent', agent)
         object.__setattr__(self, 'retriever', retriever)
         self.agent.equip_retriever(self.retriever)
         object.__setattr__(self, 'logger', get_logger(self.__class__.__name__))
 
     @abstractclassmethod
     def from_config(cls,
                     open_ai_key: str,
-                    prompt_name: str = 'questionpostgresql',
-                    temperature: float = 0.0):
+                    prompt_name: str = 'question_database',
+                    temperature: float = 0.0) -> Any:
+        """
+        Initialize a BasicChain class from configurations
+        Args:
+            open_ai_key (str): openai api key
+            prompt_name (str, optional): prompt to use.
+            temperature (float, optional): how unstable the llm should behave.
+                Defaults to 0.0.
+
+        Returns:
+            BasicChain: the Basic Chain class itself.
+        """
         llm = OpenAI(temperature=temperature, openai_api_key=open_ai_key)
         agent = Agent(prompt=BasicPrompt.
                       load_prompt_from_json_file(prompt_name),
                       llm=llm)
         retriever = BasicRetriever()
         return cls(agent=agent, retriever=retriever)
 
     @abstractclassmethod
-    def perform(self, **kwargs: Any):
+    def perform(self, **kwargs: Any) -> Any:
+        """
+        Core function to perform.
+        Returns:
+            Any: the chain execution result.
+        """
         result = self.agent.predict(kwargs)
         return result
 
-    def perform_cost_monitor(self, **kwargs: Any):
-        with get_openai_tracer(id=self.__class__.__name__) as cb:
-            result = self.perform(**kwargs)
+    def perform_cost_monitor(self, budget: float = 100, **kwargs: Any):
+        with get_openai_tracer(id=self.__class__.__name__,
+                               budget=budget) as cb:
+            try:
+                result = self.perform(**kwargs)
+            except Exception as e:
+                result = str(e)
+                self.logger.warning(cb.cur_trace.output)
         self.logger.cost(openai_cb_2_str(cb))
         return result, cb
 
 
-class BasicCombinedChain(ABC):
+class BasicCombinedChain(BasicChain, ABC):
     '''
     Abstract class for combined Chain class.
     A combined chain is a chain with multiple chains
     A chain class should be the atomic unit for completing a job.
     A chain object must have the function to perform a job.
     '''
     def __init__(self, chains: List[BasicChain]):
@@ -60,13 +82,7 @@
     @abstractclassmethod
     def from_config(cls, **kwargs: Any):
         return
 
     @abstractclassmethod
     def perform(self, **kwargs: Any):
         return
-
-    def perform_cost_monitor(self, **kwargs: Any):
-        with get_openai_tracer(id=self.__class__.__name__) as cb:
-            result = self.perform(**kwargs)
-        self.logger.cost(openai_cb_2_str(cb))
-        return result, cb
```

### Comparing `llmreflect-0.0.9/llmreflect/Chains/DatabaseChain.py` & `llmreflect-0.1.4/llmreflect/Chains/DatabaseChain.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,57 @@
 from llmreflect.Chains.BasicChain import BasicChain, BasicCombinedChain
-from llmreflect.Agents.QuestionAgent import PostgresqlQuestionAgent
-from llmreflect.Agents.PostgresqlAgent import PostgresqlAgent, \
-    PostgresqlSelfFixAgent
-from llmreflect.Agents.EvaluationAgent import PostgressqlGradingAgent
+from llmreflect.Agents.QuestionAgent import DatabaseQuestionAgent
+from llmreflect.Agents.DatabaseAgent import DatabaseAgent, \
+    DatabaseSelfFixAgent
+from llmreflect.Agents.EvaluationAgent import DatabaseGradingAgent
 from llmreflect.Retriever.DatabaseRetriever import DatabaseQuestionRetriever, \
-    DatabaseRetriever
-from llmreflect.Retriever.BasicRetriever import BasicEvaluationRetriever
+    DatabaseRetriever, DatabaseEvaluationRetriever
 from llmreflect.Chains.ModerateChain import ModerateChain
 from typing import List
 
 
 class DatabaseQuestionChain(BasicChain):
-    def __init__(self, agent: PostgresqlQuestionAgent,
+    def __init__(self, agent: DatabaseQuestionAgent,
                  retriever: DatabaseQuestionRetriever):
         """
         A chain for creating questions given by a dataset.
         Args:
-            agent (PostgresqlQuestionAgent): _description_
-            retriever (DatabaseQuestionRetriever): _description_
+            agent (DatabaseQuestionAgent): DatabaseQuestionAgent
+            retriever (DatabaseQuestionRetriever): DatabaseQuestionRetriever
         """
         super().__init__(agent, retriever)
 
     @classmethod
     def from_config(cls, uri: str,
                     include_tables: List,
                     open_ai_key: str,
-                    prompt_name: str = 'questionpostgresql',
+                    prompt_name: str = 'question_database',
                     max_output_tokens: int = 512,
                     temperature: float = 0.7,
-                    sample_rows: int = 0):
-        agent = PostgresqlQuestionAgent(
+                    sample_rows: int = 0) -> BasicChain:
+        """
+        Initialize class from configurations
+        Args:
+            uri (str): uri to connect to the database
+            include_tables (List): a list of names of database tables
+                to include
+            open_ai_key (str): openai api key
+            prompt_name (str, optional): prompt file name without json.
+            max_output_tokens (int, optional): maximum completion tokens.
+                Defaults to 512.
+            temperature (float, optional): how unstable the llm is.
+                Defaults to 0.7. Since this chain is used for generating
+                random questions. We would like it to be creative.
+            sample_rows (int, optional): rows from db provided to llm
+                as a sample. Defaults to 0.
+
+        Returns:
+            BasicChain: A DatabaseQuestionChain object.
+        """
+        agent = DatabaseQuestionAgent(
             open_ai_key=open_ai_key,
             prompt_name=prompt_name,
             max_output_tokens=max_output_tokens,
             temperature=temperature)
 
         retriever = DatabaseQuestionRetriever(
             uri=uri,
@@ -43,44 +61,66 @@
         return cls(agent=agent, retriever=retriever)
 
     def perform(self, n_questions: int = 5) -> list:
         """
         Overwrite perform function.
         Generate n questions.
         Args:
-            n_questions (int, optional): _description_. Defaults to 5.
+            n_questions (int, optional): number of questions to generate.
+                Defaults to 5.
 
         Returns:
             list: a list of questions, each question is a str object.
         """
         result = self.agent.predict_n_questions(n_questions=n_questions)
         return result
 
 
 class DatabaseAnswerChain(BasicChain):
-    def __init__(self, agent: PostgresqlAgent, retriever: DatabaseRetriever):
+    def __init__(self, agent: DatabaseAgent, retriever: DatabaseRetriever):
         """
-        Chain for generating postgresql cmd based on questions in natural
+        Chain for generating database query cmd based on questions in natural
         language.
         Args:
-            agent (PostgresqlAgent): _description_
-            retriever (DatabaseRetriever): _description_
+            agent (DatabaseAgent): DatabaseAgent
+            retriever (DatabaseRetriever): DatabaseRetriever
         """
         super().__init__(agent, retriever)
 
     @classmethod
     def from_config(cls, uri: str,
                     include_tables: List,
                     open_ai_key: str,
-                    prompt_name: str = 'postgresql',
+                    prompt_name: str = 'answer_database',
                     max_output_tokens: int = 512,
                     temperature: float = 0.0,
                     sample_rows: int = 0,
-                    max_rows_return=500):
-        agent = PostgresqlAgent(
+                    max_rows_return=500) -> BasicChain:
+        """
+        Initialize class from configurations
+        Args:
+            uri (str): uri to connect to the database
+            include_tables (List): a list of names of database tables
+                to include
+            open_ai_key (str): openai api key
+            prompt_name (str, optional): prompt file name.
+                Defaults to 'answer_database'.
+            max_output_tokens (int, optional): Maximum completion tokens.
+                Defaults to 512.
+            temperature (float, optional): How unstable the llm is.
+                Defaults to 0.0.
+            sample_rows (int, optional): Rows from db provided to llm
+                as a sample. Defaults to 0.
+            max_rows_return (int, optional): Maximum rows retrieve from db.
+                Defaults to 500.
+
+        Returns:
+            BasicChain: A DatabaseAnswerChain object.
+        """
+        agent = DatabaseAgent(
             open_ai_key=open_ai_key,
             prompt_name=prompt_name,
             max_output_tokens=max_output_tokens,
             temperature=temperature)
 
         retriever = DatabaseRetriever(
             uri=uri,
@@ -112,54 +152,59 @@
             user_input=user_input,
             get_cmd=get_cmd,
             get_summary=get_summary,
             get_db=get_db)
 
 
 class DatabaseGradingChain(BasicChain):
-    def __init__(self, agent: PostgressqlGradingAgent,
-                 retriever: BasicEvaluationRetriever):
-        """_summary_
+    def __init__(self, agent: DatabaseGradingAgent,
+                 retriever: DatabaseEvaluationRetriever):
+        """
         A chain for the following workflow:
         1. given by questions about a database and according
-            postgresql solutions for questions
+            database query solutions for questions
         2. evaluate the generated solutions
         Args:
-            agent (PostgressqlGradingAgent): _description_
-            retriever (BasicEvaluationRetriever): _description_
+            agent (PostgressqlGradingAgent): PostgressqlGradingAgent
+            retriever (DatabaseEvaluationRetriever):
+                DatabaseEvaluationRetriever
         """
         super().__init__(agent, retriever)
 
     @classmethod
     def from_config(cls,
                     open_ai_key: str,
+                    uri: str,
+                    include_tables: list,
                     max_output_tokens: int = 256,
-                    prompt_name: str = "gradingpostgresql",
-                    temperature: float = 0.7):
-        """_summary_
-
+                    prompt_name: str = "grading_database",
+                    temperature: float = 0.0,
+                    ) -> BasicChain:
+        """
+        Initialize an object of DatabaseGradingChain from configurations.
         Args:
-            open_ai_key (str): _description_
-            max_output_tokens (int, optional): dont need to be long.
-                Defaults to 256.
-            prompt_name (str, optional): _description_.
-                Defaults to "gradingpostgresql".
-            temperature (float, optional): questions should be diverse.
-                Set this to a high value but lower than 1. Defaults to 0.7.
+            open_ai_key (str): openai api key.
+            max_output_tokens (int, optional): Maximum completion tokens.
+                Dont need to be long. Defaults to 256.
+            prompt_name (str, optional): Prompt file name.
+                Defaults to "grading_database".
+            temperature (float, optional): How unstable the llm is.
+                Defaults to 0.0.
 
         Returns:
-            _type_: _description_
+            BasicChain: A DatabaseGradingChain object.
         """
-        agent = PostgressqlGradingAgent(
+        agent = DatabaseGradingAgent(
             open_ai_key=open_ai_key,
             prompt_name=prompt_name,
             max_output_tokens=max_output_tokens,
             temperature=temperature)
 
-        retriever = BasicEvaluationRetriever()
+        retriever = DatabaseEvaluationRetriever(uri=uri,
+                                                include_tables=include_tables)
         return cls(agent=agent, retriever=retriever)
 
     def perform(self, question: str,
                 query: str,
                 db_summary: str) -> dict:
         """_summary_
 
@@ -176,14 +221,32 @@
                                      sql_cmd=query,
                                      db_summary=db_summary)
         return grad_dict
 
 
 class DatabaseQnAGradingChain(BasicCombinedChain):
     def __init__(self, chains: List[BasicChain], q_batch_size: int = 5):
+        """
+        A combined chain for following workflow:
+        1. creating questions given by a dataset.
+        2. answering the questions by generating database queries.
+        3. evaluating the generated answers.
+        Args:
+            chains (List[BasicChain]): a list of chains to complete the job.
+                Expecting three exact chain: DatabaseQuestionChain,
+                DatabaseAnswerChain, DatabaseGradingChain
+            q_batch_size (int, optional): size of batch for generating
+                questions. Defaults to 5. The reasons for generating questions
+                by batch is that I found generating too many questions all at
+                once, the questions become repetitive.
+
+        Raises:
+            Exception: Illegal chain error when the list of chains do not meet
+                requirements.
+        """
         super().__init__(chains)
         assert len(chains) == 3
 
         for chain in self.chains:
             if chain.__class__ == DatabaseAnswerChain:
                 self.db_a_chain = chain
             elif chain.__class__ == DatabaseQuestionChain:
@@ -194,26 +257,57 @@
                 raise Exception("Illegal chains!")
         self.q_batch_size = q_batch_size
 
     @classmethod
     def from_config(cls, uri: str,
                     include_tables: List,
                     open_ai_key: str,
-                    question_chain_prompt_name: str = 'questionpostgresql',
-                    answer_chain_prompt_name: str = 'postgresql',
-                    grading_chain_prompt_name: str = 'gradingpostgresql',
+                    question_chain_prompt_name: str = 'question_database',
+                    answer_chain_prompt_name: str = 'answer_database',
+                    grading_chain_prompt_name: str = 'grading_database',
                     q_max_output_tokens: int = 256,
-                    q_temperature: float = 0.7,
                     a_max_output_tokens: int = 512,
                     g_max_output_tokens: int = 256,
+                    q_temperature: float = 0.7,
                     a_temperature: float = 0.0,
                     g_temperature: float = 0.0,
                     sample_rows: int = 0,
-                    max_rows_return=500):
-
+                    max_rows_return=500) -> BasicCombinedChain:
+        """
+        Initialize a DatabaseQnAGradingChain object.
+        Args:
+            uri (str): A uri to connect to the database.
+            include_tables (List): a list of names of database tables
+                to include.
+            open_ai_key (str): openai api key.
+            question_chain_prompt_name (str, optional): Prompt file name for
+                question chain. Defaults to 'question_database'.
+            answer_chain_prompt_name (str, optional): Prompt file name for
+                answer chain. Defaults to 'answer_database'.
+            grading_chain_prompt_name (str, optional): Prompt file name for
+                grading chain. Defaults to 'grading_database'.
+            q_max_output_tokens (int, optional): Maximum completion tokens for
+                generating questions. Defaults to 256.
+            a_max_output_tokens (int, optional): Maximum completion tokens for
+                generating answers. Defaults to 512.
+            g_max_output_tokens (int, optional): Maximum completion tokens for
+                evaluating answers. Defaults to 256.
+            q_temperature (float, optional): temperature for question.
+                Defaults to 0.7.
+            a_temperature (float, optional): temperature for answer.
+                Defaults to 0.0.
+            g_temperature (float, optional): temperature for grading.
+                Defaults to 0.0.
+            sample_rows (int, optional): Rows from db provided to llm
+                as a sample. Defaults to 0.
+            max_rows_return (int, optional): Maximum rows retrieve from db.
+                Defaults to 500.
+        Returns:
+            BasicCombinedChain: _description_
+        """
         db_q_chain = DatabaseQuestionChain.from_config(
             uri=uri,
             include_tables=include_tables,
             open_ai_key=open_ai_key,
             prompt_name=question_chain_prompt_name,
             max_output_tokens=q_max_output_tokens,
             temperature=q_temperature,
@@ -228,27 +322,30 @@
             max_output_tokens=a_max_output_tokens,
             temperature=a_temperature,
             sample_rows=sample_rows,
             max_rows_return=max_rows_return
         )
 
         db_g_chain = DatabaseGradingChain.from_config(
+            uri=uri,
+            include_tables=include_tables,
             open_ai_key=open_ai_key,
             prompt_name=grading_chain_prompt_name,
             max_output_tokens=g_max_output_tokens,
             temperature=g_temperature)
 
         return cls(chains=[db_q_chain, db_a_chain, db_g_chain],
                    q_batch_size=5)
 
     def perform(self, n_question: int = 5) -> dict:
-        """_summary_
-
+        """
+        perform the q and a and grading chain.
         Args:
-            n_question (int, optional): _description_. Defaults to 5.
+            n_question (int, optional): number of questions to create.
+                Defaults to 5.
 
         Returns:
             dict: {
                 'question': str, question generated,
                 'cmd': str, generated cmd,
                 'summary': str, summary from executing the cmd,
                 'grading': float, scores by grading agent
@@ -288,14 +385,30 @@
             })
 
         return t_logs
 
 
 class DatabaseAnswerNFixChain(BasicCombinedChain):
     def __init__(self, chains: List[BasicChain], fix_patience: int = 3):
+        """
+        A combined chain with two sub-basic chains, database answer chain
+        and self-fix chain. This chain is responsible for the following work:
+        1. answering natural language questions by creating database queries.
+        2. try executing the query, if encounter error, fix the query.
+        Args:
+            chains (List[BasicChain]): a list of chains,
+                Supposed to be 2 chains. DatabaseAnswerChain and
+                DatabaseSelfFixChain.
+            fix_patience (int, optional): maximum self-fix attempts allowed.
+                Defaults to 3.
+
+        Raises:
+            Exception: Illegal chain error when the list of chains do not meet
+                requirements.
+        """
         super().__init__(chains)
         assert len(chains) == 2
         self.fix_patience = fix_patience
         for chain in self.chains:
             if chain.__class__ == DatabaseAnswerChain:
                 self.answer_chain = chain
             elif chain.__class__ == DatabaseSelfFixChain:
@@ -344,22 +457,26 @@
 
     def perform(self,
                 user_input: str,
                 get_cmd: bool = True,
                 get_db: bool = False,
                 get_summary: bool = True,
                 log_fix: bool = True) -> dict:
-        """_summary_
-
+        """
+        Perform the main function for this chain.
         Args:
-            user_input (str): _description_
-            get_cmd (bool, optional): _description_. Defaults to True.
-            get_db (bool, optional): _description_. Defaults to False.
-            get_summary (bool, optional): _description_. Defaults to True.
-            log_fix (bool, optional): _description_. Defaults to True.
+            user_input (str): user's natural language question.
+            get_cmd (bool, optional): Flag, if return the database query
+                command. Defaults to True.
+            get_db (bool, optional): Flag, if return database execution
+                results. Defaults to False.
+            get_summary (bool, optional): Flag, if return a summary of
+                the database execution results. Defaults to True.
+            log_fix (bool, optional): Flag, if log the fix attempts by
+                logger. Defaults to True.
 
         Returns:
             dict: 'cmd': str, sql_cmd,
                 'summary': str, summary,
                 'db': str, db_result,
                 'error': dict, error_logs: 'cmd', what sql cmd caused error,
                                             'error', what is the error
@@ -417,34 +534,56 @@
         return {'cmd': sql_cmd,
                 'summary': summary,
                 'db': db_result,
                 'error': error_logs}
 
 
 class DatabaseSelfFixChain(BasicChain):
-    """
-    A chain class for fixing sql errors
-    Args:
-        BasicChain (_type_): _description_
-    """
     def __init__(self,
-                 agent: PostgresqlSelfFixAgent,
+                 agent: DatabaseSelfFixAgent,
                  retriever: DatabaseRetriever):
+        """
+        A Basic chain class for fix database queries.
+        Args:
+            agent (DatabaseSelfFixAgent): DatabaseSelfFixAgent
+            retriever (DatabaseRetriever): DatabaseRetriever
+        """
         super().__init__(agent, retriever)
 
     @classmethod
     def from_config(cls, uri: str,
                     include_tables: List,
                     open_ai_key: str,
-                    prompt_name: str = 'postgresqlfix',
+                    prompt_name: str = 'fix_database',
                     max_output_tokens: int = 512,
                     temperature: float = 0.0,
                     sample_rows: int = 0,
-                    max_rows_return: int = 500):
-        agent = PostgresqlSelfFixAgent(
+                    max_rows_return: int = 500) -> BasicChain:
+        """
+        Initialize a DatabaseSelfFixChain object from configurations.
+        Args:
+            uri (str): A uri to connect to the database.
+            include_tables (List): A list of names of database tables
+                to include.
+            open_ai_key (str): openai api key.
+            prompt_name (str, optional): Prompt file name.
+                Defaults to 'fix_database'.
+            max_output_tokens (int, optional): Maximum completion tokens.
+                Defaults to 512.
+            temperature (float, optional): How unstable the llm is.
+                Defaults to 0.0.
+            sample_rows (int, optional): Rows from db provided to llm
+                as a sample. Defaults to 0.
+            max_rows_return (int, optional): Maximum rows retrieve from db.
+                Defaults to 500.
+
+        Returns:
+            BasicChain: A DatabaseSelfFixChain object.
+        """
+        agent = DatabaseSelfFixAgent(
             open_ai_key=open_ai_key,
             prompt_name=prompt_name,
             max_output_tokens=max_output_tokens,
             temperature=temperature)
 
         retriever = DatabaseRetriever(
             uri=uri,
@@ -457,16 +596,16 @@
     def perform(self,
                 user_input: str,
                 history: str,
                 his_error: str,
                 get_cmd: bool = True,
                 get_db: bool = False,
                 get_summary: bool = True) -> dict:
-        """_summary_
-
+        """
+        Perform chain function.
         Args:
             user_input (str): user's description
             history (str): history command used for query
             his_error (str): the errors raised from executing the history cmd
             get_cmd (bool, optional): if return cmd. Defaults to True.
             get_db (bool, optional): if return queried db gross result.
                 Defaults to False.
@@ -483,14 +622,30 @@
             get_cmd=get_cmd,
             get_summary=get_summary,
             get_db=get_db)
 
 
 class DatabaseModerateNAnswerNFixChain(BasicCombinedChain):
     def __init__(self, chains: List[BasicChain], fix_patience: int = 3):
+        """
+        A combined chain for: moderating user input, generating
+        database query to solve the question, when encounter an
+        error during execution, fix the query.
+        Args:
+            chains (List[BasicChain]): A list of chains.
+            Should be two chain, a basic chain and a combined chain.
+            The basic chain is the ModerateChain. And the combined
+            chain should be DatabaseAnswerNFixChain.
+            fix_patience (int, optional): maximum self-fix attempts allowed.
+                Defaults to 3.
+
+        Raises:
+            Exception: Illegal chain error when the list of chains do not meet
+                requirements.
+        """
         super().__init__(chains)
         assert len(chains) == 2
         self.fix_patience = fix_patience
         for chain in self.chains:
             if chain.__class__ == ModerateChain:
                 self.moderate_chain = chain
             elif chain.__class__ == DatabaseAnswerNFixChain:
@@ -500,26 +655,62 @@
 
     @classmethod
     def from_config(
             cls,
             uri: str,
             include_tables: list,
             open_ai_key: str,
-            answer_chain_prompt_name: str = "postgresql",
-            fix_chain_prompt_name: str = "postgresqlfix",
-            moderate_chain_prompt_name: str = "moderatepostgresql",
+            answer_chain_prompt_name: str = "answer_database",
+            fix_chain_prompt_name: str = "fix_database",
+            moderate_chain_prompt_name: str = "moderate_database",
             max_output_tokens_a: int = 512,
             max_output_tokens_f: int = 512,
             max_output_tokens_m: int = 256,
             temperature_a: float = 0.0,
             temperature_f: float = 0.0,
             temperature_m: float = 0.0,
-            sample_row: int = 0,
+            sample_rows: int = 0,
             max_rows_return: int = 500,
-            fix_patience: int = 3):
+            fix_patience: int = 3) -> BasicCombinedChain:
+        """
+        Initialize a DatabaseModerateNAnswerNFixChain object from
+        configuration.
+        Args:
+            uri (str): A uri to connect to the database.
+            include_tables (list): A list of names of database tables
+                to include.
+            open_ai_key (str): openai api key.
+            answer_chain_prompt_name (str, optional): Prompt file for answer
+                chain. Defaults to "answer_database".
+            fix_chain_prompt_name (str, optional): Prompt file for fix chain.
+                Defaults to "fix_database".
+            moderate_chain_prompt_name (str, optional): prompt file for
+                moderate chain . Defaults to "moderate_database".
+            max_output_tokens_a (int, optional): Maximum completion tokens for
+                answering. Defaults to 512.
+            max_output_tokens_f (int, optional): Maximum completion tokens for
+                fixing. Defaults to 512.
+            max_output_tokens_m (int, optional): Maximum completion tokens for
+                moderation. Defaults to 512.
+            temperature_a (float, optional): temperature for answering chain.
+                Defaults to 0.0.
+            temperature_f (float, optional): temperature for fixing chain.
+                Defaults to 0.0.
+            temperature_m (float, optional): temperature for moderation chain.
+                Defaults to 0.0.
+            sample_rows (int, optional): Rows from db provided to llm
+                as a sample. Defaults to 0.
+            max_rows_return (int, optional): Maximum rows retrieve from db.
+                Defaults to 500.
+            fix_patience (int, optional): Maximum self-fix attempts allowed.
+                Defaults to 3.
+
+        Returns:
+            BasicCombinedChain: An object of DatabaseModerateNAnswerNFixChain.
+        """
 
         db_m_chain = ModerateChain.from_config(
             open_ai_key=open_ai_key,
             include_tables=include_tables,
             prompt_name=moderate_chain_prompt_name,
             max_output_tokens=max_output_tokens_m,
             temperature=temperature_m
@@ -530,31 +721,31 @@
             open_ai_key=open_ai_key,
             answer_chain_prompt_name=answer_chain_prompt_name,
             fix_chain_prompt_name=fix_chain_prompt_name,
             max_output_tokens_a=max_output_tokens_a,
             max_output_tokens_f=max_output_tokens_f,
             temperature_a=temperature_a,
             temperature_f=temperature_f,
-            sample_row=sample_row,
+            sample_row=sample_rows,
             max_rows_return=max_rows_return,
             fix_patience=fix_patience
         )
 
         return cls(chains=[db_m_chain, db_a_fix_chain],
                    fix_patience=fix_patience)
 
     def perform(self,
                 user_input: str,
                 get_cmd: bool = True,
                 get_db: bool = False,
                 get_summary: bool = True,
                 log_fix: bool = True,
                 explain_moderate: bool = True) -> dict:
-        """_summary_
-
+        """
+        Perform chain function.
         Args:
             user_input (str): _description_
             get_cmd (bool, optional): _description_. Defaults to True.
             get_db (bool, optional): _description_. Defaults to False.
             get_summary (bool, optional): _description_. Defaults to True.
             log_fix (bool, optional): _description_. Defaults to True.
```

### Comparing `llmreflect-0.0.9/llmreflect/Chains/ModerateChain.py` & `llmreflect-0.1.4/llmreflect/Chains/ModerateChain.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,48 @@
-from llmreflect.Agents.ModerateAgent import PostgresqlModerateAgent
+from llmreflect.Agents.ModerateAgent import DatabaseModerateAgent
 from llmreflect.Chains.BasicChain import BasicChain
 from llmreflect.Retriever.BasicRetriever import BasicQuestionModerateRetriever
 from typing import Any
 
 
 class ModerateChain(BasicChain):
-    def __init__(self, agent: PostgresqlModerateAgent,
+    def __init__(self, agent: DatabaseModerateAgent,
                  retriever: BasicQuestionModerateRetriever):
+        """
+        A chain for filtering out toxic questions and injection attacks.
+        Args:
+            agent (DatabaseModerateAgent): DatabaseModerateAgent
+            retriever (BasicQuestionModerateRetriever):
+                BasicQuestionModerateRetriever
+        """
         super().__init__(agent, retriever)
 
     @classmethod
     def from_config(cls,
                     open_ai_key: str,
                     include_tables: list,
-                    prompt_name: str = 'moderatepostgresql',
+                    prompt_name: str = 'moderate_database',
                     max_output_tokens: int = 512,
-                    temperature: float = 0.0):
+                    temperature: float = 0.0) -> BasicChain:
+        """
+        Initialize a ModerateChain object from configurations.
+        Args:
+            open_ai_key (str): Openai api key.
+            include_tables (list): A list of database tables names to include.
+            prompt_name (str, optional): Prompt file name.
+                Defaults to 'moderate_database'.
+            max_output_tokens (int, optional): Maximum completion tokens.
+                Defaults to 512.
+            temperature (float, optional): The higher the more unstable.
+                Defaults to 0.0.
 
-        agent = PostgresqlModerateAgent(
+        Returns:
+            BasicChain: _description_
+        """
+        agent = DatabaseModerateAgent(
             open_ai_key=open_ai_key,
             prompt_name=prompt_name,
             max_output_tokens=max_output_tokens,
             temperature=temperature
         )
         retriever = BasicQuestionModerateRetriever(
             include_tables=include_tables)
```

### Comparing `llmreflect-0.0.9/llmreflect/Prompt/BasicPrompt.py` & `llmreflect-0.1.4/llmreflect/Prompt/BasicPrompt.py`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.9/llmreflect/Prompt/promptbase/gradingpostgresql.json` & `llmreflect-0.1.4/llmreflect/Prompt/promptbase/grading_database.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.865625%*

 * *Differences: {"'FORMAT'": "{'command': {'explanation': 'the generated {dialect} command'}, 'summary': "*

 * *             "{'explanation': 'a summary for the execution result from database'}, 'grading': "*

 * *             "{'explanation': 'the score you assign to the {dialect} command, a number range from "*

 * *             "0 to 10'}}",*

 * * "'HARD'": "'You are a data engineer who work in an alzheimer clinic. Your job is to evaluate if a "*

 * *           '{dialect} command satisfies the request.You will be given a request,an associated '*

 * *  […]*

```diff
@@ -1,31 +1,31 @@
 {
     "FORMAT": {
         "command": {
-            "explanation": "the generated postgresql command",
+            "explanation": "the generated {dialect} command",
             "type": "INPUT"
         },
         "explanation": {
             "explanation": "the reason for your scoring",
             "type": "OUTPUT"
         },
         "grading": {
-            "explanation": "the score you assign to the postgresql command, a number range from 0 to 10",
+            "explanation": "the score you assign to the {dialect} command, a number range from 0 to 10",
             "type": "OUTPUT"
         },
         "request": {
             "explanation": "User's natural language request",
             "type": "INPUT"
         },
         "summary": {
-            "explanation": "a summary for the excution result from database",
+            "explanation": "a summary for the execution result from database",
             "type": "INPUT"
         }
     },
-    "HARD": "You are a data engineer who work in an alzheimer clinic. Your job is to evaluate if a postgresql command satisfies the request.You will be given a request,an associated postgresql command,a summary for the execution result retrieved from the database.\nGrade the postgresql command by a score from 0 (worst) to 10 (best) and explain why.\n",
+    "HARD": "You are a data engineer who work in an alzheimer clinic. Your job is to evaluate if a {dialect} command satisfies the request.You will be given a request,an associated {dialect} command,a summary for the execution result retrieved from the database.\nGrade the {dialect} command by a score from 0 (worst) to 10 (best) and explain why.\n",
     "INCONTEXT": [
         {
             "command": "select count(*)\nfrom tb_patient\ninner join tb_patient_medications\non tb_patient.uuid_patient = tb_patient_medications.patient\nwhere (\"medication_name\" similar to '%alzheimer%'\nor \"patient_treatment\" similar to '%alzheimer%');",
             "explanation": "The query is syntactically correct. It can be successfully executed. But 'alzheimer' is name of disease therefore should not be queried in the column 'medication_name'. However, the question is too hard since it requires strong background knowledge for alzheimer",
             "grading": "5",
             "request": "How many patients are taking medications for alzheimer?",
             "summary": "You retrieved 1 entries with 1 columns from the database.The columns are count. An example of entries is: 0."
```

### Comparing `llmreflect-0.0.9/llmreflect/Prompt/promptbase/moderatepostgresql.json` & `llmreflect-0.1.4/llmreflect/Prompt/promptbase/moderate_database.json`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.9/llmreflect/Prompt/promptbase/postgresql.json` & `llmreflect-0.1.4/llmreflect/Prompt/promptbase/answer_database.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9921875%*

 * *Differences: {"'FORMAT'": "{'answer': {'explanation': 'the {dialect} query you created'}}"}*

```diff
@@ -1,11 +1,11 @@
 {
     "FORMAT": {
         "answer": {
-            "explanation": "the postgresql query you created",
+            "explanation": "the {dialect} query you created",
             "type": "OUTPUT"
         },
         "request": {
             "explanation": "user's request",
             "type": "INPUT"
         }
     },
```

### Comparing `llmreflect-0.0.9/llmreflect/Prompt/promptbase/postgresqlfix.json` & `llmreflect-0.1.4/llmreflect/Prompt/promptbase/fix_database.json`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.9/llmreflect/Prompt/promptbase/questionpostgresql.json` & `llmreflect-0.1.4/llmreflect/Prompt/promptbase/question_database.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.875%*

 * *Differences: {"'HARD'": "'You are a smart assistant designed to help with testing a {dialect} AI.\\nGiven by "*

 * *           'information about a database, you must come up with questions in natural language. '*

 * *           'There are two things that you want to exam. First,it is the comprehensive ability that '*

 * *           'how well the AI understands the question.Second, it is the {dialect} query ability '*

 * *           'that how well the AI designs complicated queries. Therefore, you must phrase your '*

 * *           'questions i […]*

```diff
@@ -5,15 +5,15 @@
             "type": "INPUT"
         },
         "questions": {
             "explanation": "\n[1.] the first question created by you. \n[2.] the second question \n... \n[n.] the nth question",
             "type": "OUTPUT"
         }
     },
-    "HARD": "You are a smart assistant designed to help with testing a postgresql AI.\nGiven by information about a database, you must come up with questions in natural language. There are two things that you want to exam. First,it is the comprehensive ability that how well the AI understands the question.Second, it is the postgresql query ability that how well the AI designs complicated queries. Therefore, you must phrase your questions in diverse ways and the questions require sophisticated logic to be solved.\n\nThe information about the database is:\n{table_info}\n",
+    "HARD": "You are a smart assistant designed to help with testing a {dialect} AI.\nGiven by information about a database, you must come up with questions in natural language. There are two things that you want to exam. First,it is the comprehensive ability that how well the AI understands the question.Second, it is the {dialect} query ability that how well the AI designs complicated queries. Therefore, you must phrase your questions in diverse ways and the questions require sophisticated logic to be solved.\n\nThe information about the database is:\n{table_info}\n",
     "INCONTEXT": [
         {
             "n_questions": "2",
             "questions": "\n[1.] Give me a list of 5 patients\n[2.] what is the lowest mmse score in the records\n"
         },
         {
             "n_questions": "1",
```

### Comparing `llmreflect-0.0.9/llmreflect/Retriever/BasicRetriever.py` & `llmreflect-0.1.4/llmreflect/Retriever/BasicRetriever.py`

 * *Files identical despite different names*

### Comparing `llmreflect-0.0.9/llmreflect/Tests/test_chains.py` & `llmreflect-0.1.4/llmreflect/Tests/test_chains.py`

 * *Files 4% similar despite different names*

```diff
@@ -150,36 +150,36 @@
     open_ai_key = config('OPENAI_API_KEY')
     max_output_tokens = 512
 
     q_ch = DatabaseQuestionChain.from_config(
         uri=uri,
         include_tables=include_tables,
         open_ai_key=open_ai_key,
-        prompt_name="questionpostgresql",
+        prompt_name="question_database",
         max_output_tokens=max_output_tokens,
         temperature=0.7,
         sample_rows=0
     )
 
     a_ch = DatabaseAnswerChain.from_config(
         uri=uri,
         include_tables=include_tables,
         open_ai_key=open_ai_key,
-        prompt_name="postgresql",
+        prompt_name="answer_database",
         max_output_tokens=max_output_tokens,
         temperature=0.0,
         sample_rows=0,
         max_rows_return=500
     )
 
     self_fix_ch = DatabaseSelfFixChain.from_config(
         uri=uri,
         include_tables=include_tables,
         open_ai_key=open_ai_key,
-        prompt_name="postgresqlfix",
+        prompt_name="fix_database",
         max_output_tokens=max_output_tokens,
         temperature=0.1,
         sample_rows=0,
         max_rows_return=500
     )
 
     questions, traces = q_ch.perform_cost_monitor(n_questions=5)
@@ -227,15 +227,45 @@
             'tb_patient',
             'tb_patients_allergies',
             'tb_appointment_patients',
             'tb_patient_mmse_and_moca_scores',
             'tb_patient_medications'
         ],
         open_ai_key=config('OPENAI_API_KEY'),
-        answer_chain_prompt_name="postgresql",
-        fix_chain_prompt_name="postgresqlfix"
+        answer_chain_prompt_name="answer_database",
+        fix_chain_prompt_name="fix_database"
     )
     result_dict, traces = ch.perform_cost_monitor(
         user_input="give me a list overweight patients")
     assert len(result_dict['summary']) > 0
     assert type(result_dict['error']) is list
     LOGGER.debug(traces_2_str(traces))
+
+
+@pytest.mark.skipif(bool(in_workflow()),
+                    reason="Only test database operations \
+                    in local env")
+def test_budget_limitation():
+    from llmreflect.Chains.DatabaseChain import DatabaseQnAGradingChain
+    from decouple import config
+
+    N_QUESTIONS = 100
+
+    uri = f"postgresql+psycopg2://{config('DBUSERNAME')}:\
+{config('DBPASSWORD')}@{config('DBHOST')}:{config('DBPORT')}/postgres"
+
+    ch = DatabaseQnAGradingChain.from_config(
+        uri=uri,
+        include_tables=[
+            'tb_patient',
+            'tb_patients_allergies',
+            'tb_appointment_patients',
+            'tb_patient_mmse_and_moca_scores',
+            'tb_patient_medications'
+        ],
+        a_max_output_tokens=512,
+        g_max_output_tokens=256,
+        open_ai_key=config('OPENAI_API_KEY')
+    )
+
+    logs, traces = ch.perform_cost_monitor(n_question=N_QUESTIONS,
+                                           budget=0.005)
```

### Comparing `llmreflect-0.0.9/llmreflect/Utils/database.py` & `llmreflect-0.1.4/llmreflect/Utils/database.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import re
 
 
 def upper_boundary_maximum_records(sql_cmd: str, max_present: int) -> str:
     """
     replace the LIMIT in a query
     Args:
-        sql_cmd (_type_): original sql command
-        max_present (_type_): maximum number of returned entries
+        sql_cmd (str): original sql command
+        max_present (max_present): maximum number of returned entries
 
     Returns:
-        sql_cmd: bounded sql command
+        str: bounded sql command
     """
     re_pattern = 'LIMIT [0-9]*'
     limit_number_found = re.findall(re_pattern, sql_cmd, re.IGNORECASE)
     if len(limit_number_found) > 0:
         limit_number_sub = limit_number_found[0]
         limit_number = int(limit_number_sub.split(" ")[-1])
         if limit_number > max_present:
```

### Comparing `llmreflect-0.0.9/llmreflect/Utils/log.py` & `llmreflect-0.1.4/llmreflect/Utils/log.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,53 @@
 import logging
 import os
 import shutil
+from uuid import UUID
 from langchain.callbacks import OpenAICallbackHandler
 from langchain.callbacks.openai_info import standardize_model_name
 from langchain.callbacks.openai_info import MODEL_COST_PER_1K_TOKENS
 from langchain.callbacks.openai_info import get_openai_token_cost_for_model
 from typing import Dict, Any, List, Generator, Optional
 from langchain.schema import LLMResult
 from contextlib import contextmanager
 from contextvars import ContextVar
+import tiktoken
 
 
 class OpenAITracer(OpenAICallbackHandler):
-    def __init__(self, id: str = "") -> None:
+    def __init__(self, id: str = "", budget: float = 0.01) -> None:
         super().__init__()
         self.traces = []
         self.id = id
+        self.raise_error = True
+        self._budget = budget
+
+    @property
+    def budget(self):
+        return self._budget
+
+    @property
+    def budget_rest(self):
+        return self._budget - self.total_cost
 
     def on_llm_start(
         self, serialized: Dict[str, Any], prompts: List[str], **kwargs: Any
     ) -> None:
         self.cur_trace = LLMTRACE(input=prompts[0])
 
+    def on_chain_error(self, error: Exception | KeyboardInterrupt, *,
+                       run_id: UUID, parent_run_id: UUID | None = None,
+                       **kwargs: Any) -> Any:
+        self.cur_trace.output = str(error)
+        self.traces.append(self.cur_trace)
+        return super().on_chain_error(error,
+                                      run_id=run_id,
+                                      parent_run_id=parent_run_id,
+                                      **kwargs)
+
     def on_llm_end(self, response: LLMResult, **kwargs: Any) -> None:
         """Collect token usage."""
         if response.llm_output is None:
             return None
         else:
             self.cur_trace.output = response.generations[0][0].text
         self.successful_requests += 1
@@ -80,22 +102,62 @@
 
 openai_trace_var: ContextVar[Optional[OpenAITracer]] = ContextVar(
     "openai_trace", default=None
 )
 
 
 @contextmanager
-def get_openai_tracer(id: str = "") -> Generator[OpenAITracer, None, None]:
+def get_openai_tracer(id: str = "",
+                      budget: float = 0.1) -> \
+        Generator[OpenAITracer, None, None]:
     """Get OpenAI callback handler in a context manager."""
-    cb = OpenAITracer(id=id)
+    cb = OpenAITracer(id=id, budget=budget)
     openai_trace_var.set(cb)
     yield cb
     openai_trace_var.set(None)
 
 
+def check_current_openai_balance(input_prompt: str,
+                                 max_output_tokens: int,
+                                 model_name: str,
+                                 logger: Any = None) -> bool:
+    """Check if the budget balance can cover this round of llm run.
+
+    Args:
+        input_prompt (str): the input prompt for the llm
+        max_output_tokens (int): the maximum number of completion tokens,
+            configured in llm class.
+        model_name (str): the model name used for referencing,
+            Check LLM_BACKBONE_MODEL.
+        logger (Any, optional): Log predicted cost information
+            when logger provided.
+
+    Returns:
+        bool: _description_
+    """
+    openai_tracer = openai_trace_var.get()
+    encoding = tiktoken.get_encoding("cl100k_base")
+    input_tokens = len(encoding.encode(input_prompt))
+    input_cost = get_openai_token_cost_for_model(
+        model_name=model_name,
+        num_tokens=input_tokens,
+        is_completion=False
+    )
+    possible_output_cost = get_openai_token_cost_for_model(
+        model_name=model_name,
+        num_tokens=max_output_tokens,
+        is_completion=True
+    )
+    next_possible_cost = input_cost + possible_output_cost
+    if logger:
+        logger.debug(f"Total cost now: {openai_tracer.total_cost}")
+        logger.debug(f"Next round possible cost: {next_possible_cost}")
+    return openai_tracer.budget_rest >= next_possible_cost
+
+
 class CustomFormatter(logging.Formatter):
     """Logging colored formatter,
     adapted from https://stackoverflow.com/a/56944256/3638629"""
 
     grey = '\x1b[38;21m'
     blue = '\x1b[38;5;39m'
     yellow = '\x1b[38;5;226m'
@@ -206,15 +268,15 @@
 
     logger.addHandler(handler_std)
     logger.addHandler(handler_file)
     return logger
 
 
 def export_log(dir: str):
-    """A simple interface copying the log file to a designated place.
+    """A simple interface copying the log file to a designated directory.
 
     Args:
         file_path (_type_): designated directory
     """
     tmp_log_dir = os.path.join(os.path.dirname(__file__), '..', 'logs')
     logger = get_logger("log export")
     n_s = 0
@@ -248,22 +310,39 @@
     if color not in COLORS.keys():
         color = 'reset'
 
     print(f'{COLORS[color]}{msg}{COLORS["reset"]}')
 
 
 def openai_cb_2_str(cb: OpenAITracer) -> str:
+    """
+    converting openai tracer info to one string.
+    Args:
+        cb (OpenAITracer): tracer/callback handlers for openai
+
+    Returns:
+        str: A string describing the cost
+    """
     tmp_str = ""
     tmp_str += f"[Total Tokens] {cb.total_tokens}, "
     tmp_str += f"[Successful Requests] {cb.successful_requests}, "
     tmp_str += f"[Total Cost (USD) $] {cb.total_cost}"
     return tmp_str
 
 
 def traces_2_str(cb: OpenAITracer) -> str:
+    """
+    converting openai tracer info to one string.
+    Similar to openai_cb_2_str function but with more details
+    Args:
+        cb (OpenAITracer): tracer/callback handlers for openai
+
+    Returns:
+        str: A string describing the cost
+    """
     total_str = "\n"
     for trace in cb.traces:
         tmp_str = ""
         tmp_str += f"[Model Name] {trace.model_name}\n"
         tmp_str += f"[Brief Input] {trace.input[0:100]}\n"
         tmp_str += f"[Total Tokens] {trace.total_tokens}\n"
         tmp_str += f"[Completion Tokens] {trace.completion_tokens}\n"
@@ -272,8 +351,8 @@
         tmp_str += f"[Prompt Cost] {trace.prompt_cost}\n"
         tmp_str += f"[Total Cost] {trace.total_cost}\n"
         tmp_str += "====================================\n\n"
         total_str += tmp_str
     return total_str
 
 
-addLoggingLevel("COST", 25)
+addLoggingLevel("COST", 25)  # add a logging level for cost
```

### Comparing `llmreflect-0.0.9/PKG-INFO` & `llmreflect-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmreflect
-Version: 0.0.9
+Version: 0.1.4
 Summary: a package for llm self-reflection
 Author: alchemistwu
 Author-email: alchemistwu0521@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -12,14 +12,15 @@
 Requires-Dist: flake8 (>=6.0.0,<7.0.0)
 Requires-Dist: langchain (>=0.0.219,<0.0.220)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.6,<3.0.0)
 Requires-Dist: pytest (>=7.4.0,<8.0.0)
 Requires-Dist: python-decouple (>=3.8,<4.0)
+Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
 Description-Content-Type: text/markdown
 
 # llmReflect
 [![PyPI version](https://badge.fury.io/py/llmreflect.svg)](https://badge.fury.io/py/llmreflect)
 [![Python](https://img.shields.io/badge/python-3.11-blue.svg)](https://img.shields.io/badge/python-3.11-blue.svg)
 [![Python package](https://github.com/Recherches-Neuro-Hippocampe/llmReflect/actions/workflows/python-package.yml/badge.svg)](https://github.com/Recherches-Neuro-Hippocampe/llmReflect/actions/workflows/python-package.yml)
 [![Upload Python Package](https://github.com/Recherches-Neuro-Hippocampe/llmReflect/actions/workflows/python-publish.yml/badge.svg)](https://github.com/Recherches-Neuro-Hippocampe/llmReflect/actions/workflows/python-publish.yml)
```

