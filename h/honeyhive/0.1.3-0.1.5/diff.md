# Comparing `tmp/honeyhive-0.1.3.tar.gz` & `tmp/honeyhive-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/honeyhive-0.1.3.tar", last modified: Tue Mar 28 05:51:24 2023, max compression
+gzip compressed data, was "honeyhive-0.1.5.tar", last modified: Wed Jul 19 15:35:31 2023, max compression
```

## Comparing `honeyhive-0.1.3.tar` & `honeyhive-0.1.5.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 dhruvsingh   (501) staff       (20)        0 2023-03-28 05:51:24.000000 honeyhive-0.1.3/
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     6614 2023-03-28 05:51:24.000000 honeyhive-0.1.3/PKG-INFO
--rw-r--r--   0 dhruvsingh   (501) staff       (20)      205 2022-12-13 17:06:38.000000 honeyhive-0.1.3/LICENSE
-drwxr-xr-x   0 dhruvsingh   (501) staff       (20)        0 2023-03-28 05:51:24.000000 honeyhive-0.1.3/honeyhive.egg-info/
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     6614 2023-03-28 05:51:24.000000 honeyhive-0.1.3/honeyhive.egg-info/PKG-INFO
--rw-r--r--   0 dhruvsingh   (501) staff       (20)      981 2023-03-28 05:51:24.000000 honeyhive-0.1.3/honeyhive.egg-info/SOURCES.txt
--rw-r--r--   0 dhruvsingh   (501) staff       (20)       55 2023-03-28 05:51:24.000000 honeyhive-0.1.3/honeyhive.egg-info/entry_points.txt
--rw-r--r--   0 dhruvsingh   (501) staff       (20)       75 2023-03-28 05:51:24.000000 honeyhive-0.1.3/honeyhive.egg-info/requires.txt
--rw-r--r--   0 dhruvsingh   (501) staff       (20)       10 2023-03-28 05:51:24.000000 honeyhive-0.1.3/honeyhive.egg-info/top_level.txt
--rw-r--r--   0 dhruvsingh   (501) staff       (20)        1 2023-03-28 05:51:24.000000 honeyhive-0.1.3/honeyhive.egg-info/dependency_links.txt
--rw-r--r--   0 dhruvsingh   (501) staff       (20)      340 2023-03-05 06:49:29.000000 honeyhive-0.1.3/pyproject.toml
--rw-r--r--   0 dhruvsingh   (501) staff       (20)       40 2022-12-09 00:56:14.000000 honeyhive-0.1.3/MANIFEST.in
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     4567 2023-03-05 07:17:37.000000 honeyhive-0.1.3/README.md
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     1634 2023-03-27 19:14:16.000000 honeyhive-0.1.3/setup.py
-drwxr-xr-x   0 dhruvsingh   (501) staff       (20)        0 2023-03-28 05:51:24.000000 honeyhive-0.1.3/honeyhive/
--rw-r--r--   0 dhruvsingh   (501) staff       (20)       19 2022-12-26 05:27:25.000000 honeyhive-0.1.3/honeyhive/__init__.py
-drwxr-xr-x   0 dhruvsingh   (501) staff       (20)        0 2023-03-28 05:51:24.000000 honeyhive-0.1.3/honeyhive/sdk/
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     5065 2023-03-26 17:31:47.000000 honeyhive-0.1.3/honeyhive/sdk/sdk-examples.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     1236 2023-03-27 19:28:28.000000 honeyhive-0.1.3/honeyhive/sdk/metrics.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     2863 2023-03-26 07:00:20.000000 honeyhive-0.1.3/honeyhive/sdk/Completion.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)        0 2022-12-31 04:55:35.000000 honeyhive-0.1.3/honeyhive/sdk/Untitled-3
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     1452 2023-03-27 19:26:12.000000 honeyhive-0.1.3/honeyhive/sdk/generations.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)      551 2023-03-05 06:42:19.000000 honeyhive-0.1.3/honeyhive/sdk/feedback.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     2798 2023-03-12 05:30:52.000000 honeyhive-0.1.3/honeyhive/sdk/ChatCompletion.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     1799 2023-03-27 19:26:27.000000 honeyhive-0.1.3/honeyhive/sdk/datasets.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     1192 2023-03-28 00:19:47.000000 honeyhive-0.1.3/honeyhive/sdk/__init__.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     2415 2023-03-27 19:28:09.000000 honeyhive-0.1.3/honeyhive/sdk/prompts.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)      711 2023-03-27 19:26:17.000000 honeyhive-0.1.3/honeyhive/sdk/fine_tuned_models.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)      247 2023-03-05 07:06:13.000000 honeyhive-0.1.3/honeyhive/sdk/init.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     2352 2023-03-28 00:20:20.000000 honeyhive-0.1.3/honeyhive/sdk/projects.py
-drwxr-xr-x   0 dhruvsingh   (501) staff       (20)        0 2023-03-28 05:51:24.000000 honeyhive-0.1.3/honeyhive/api/
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     6681 2023-03-05 06:41:14.000000 honeyhive-0.1.3/honeyhive/api/client.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)        0 2022-12-13 17:07:45.000000 honeyhive-0.1.3/honeyhive/api/__init__.py
-drwxr-xr-x   0 dhruvsingh   (501) staff       (20)        0 2023-03-28 05:51:24.000000 honeyhive-0.1.3/honeyhive/api/models/
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     1244 2023-03-05 07:45:16.000000 honeyhive-0.1.3/honeyhive/api/models/metrics.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     2638 2023-01-09 23:57:51.000000 honeyhive-0.1.3/honeyhive/api/models/tasks.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     5268 2023-03-26 06:58:02.000000 honeyhive-0.1.3/honeyhive/api/models/generations.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     1140 2022-12-18 14:25:26.000000 honeyhive-0.1.3/honeyhive/api/models/feedback.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     2299 2023-03-05 07:44:40.000000 honeyhive-0.1.3/honeyhive/api/models/datasets.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)        0 2022-12-13 17:08:09.000000 honeyhive-0.1.3/honeyhive/api/models/__init__.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     4415 2023-01-10 00:49:31.000000 honeyhive-0.1.3/honeyhive/api/models/prompts.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)     1899 2023-03-05 07:27:57.000000 honeyhive-0.1.3/honeyhive/api/models/fine_tuned_models.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)      257 2022-12-14 20:38:37.000000 honeyhive-0.1.3/honeyhive/api/models/utils.py
--rw-r--r--   0 dhruvsingh   (501) staff       (20)       38 2023-03-28 05:51:24.000000 honeyhive-0.1.3/setup.cfg
+drwxr-xr-x   0 dhruvsingh   (501) staff       (20)        0 2023-07-19 15:35:31.386546 honeyhive-0.1.5/
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)      205 2022-12-13 17:06:38.000000 honeyhive-0.1.5/LICENSE
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)       40 2022-12-09 00:56:14.000000 honeyhive-0.1.5/MANIFEST.in
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     5542 2023-07-19 15:35:31.386386 honeyhive-0.1.5/PKG-INFO
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     4567 2023-03-05 07:17:37.000000 honeyhive-0.1.5/README.md
+drwxr-xr-x   0 dhruvsingh   (501) staff       (20)        0 2023-07-19 15:35:31.377555 honeyhive-0.1.5/honeyhive/
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)       19 2022-12-26 05:27:25.000000 honeyhive-0.1.5/honeyhive/__init__.py
+drwxr-xr-x   0 dhruvsingh   (501) staff       (20)        0 2023-07-19 15:35:31.378839 honeyhive-0.1.5/honeyhive/api/
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)        0 2022-12-13 17:07:45.000000 honeyhive-0.1.5/honeyhive/api/__init__.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     6681 2023-03-05 06:41:14.000000 honeyhive-0.1.5/honeyhive/api/client.py
+drwxr-xr-x   0 dhruvsingh   (501) staff       (20)        0 2023-07-19 15:35:31.381994 honeyhive-0.1.5/honeyhive/api/models/
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)        0 2022-12-13 17:08:09.000000 honeyhive-0.1.5/honeyhive/api/models/__init__.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     2299 2023-03-05 07:44:40.000000 honeyhive-0.1.5/honeyhive/api/models/datasets.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     1140 2022-12-18 14:25:26.000000 honeyhive-0.1.5/honeyhive/api/models/feedback.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     1899 2023-03-05 07:27:57.000000 honeyhive-0.1.5/honeyhive/api/models/fine_tuned_models.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     5383 2023-06-09 15:55:54.000000 honeyhive-0.1.5/honeyhive/api/models/generations.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     1244 2023-03-05 07:45:16.000000 honeyhive-0.1.5/honeyhive/api/models/metrics.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     4415 2023-01-10 00:49:31.000000 honeyhive-0.1.5/honeyhive/api/models/prompts.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     2638 2023-01-09 23:57:51.000000 honeyhive-0.1.5/honeyhive/api/models/tasks.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)      257 2022-12-14 20:38:37.000000 honeyhive-0.1.5/honeyhive/api/models/utils.py
+drwxr-xr-x   0 dhruvsingh   (501) staff       (20)        0 2023-07-19 15:35:31.385884 honeyhive-0.1.5/honeyhive/sdk/
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     2798 2023-03-12 05:30:52.000000 honeyhive-0.1.5/honeyhive/sdk/ChatCompletion.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     2926 2023-06-09 15:56:04.000000 honeyhive-0.1.5/honeyhive/sdk/Completion.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)        0 2022-12-31 04:55:35.000000 honeyhive-0.1.5/honeyhive/sdk/Untitled-3
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     1192 2023-03-28 00:19:47.000000 honeyhive-0.1.5/honeyhive/sdk/__init__.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     1799 2023-03-27 19:26:27.000000 honeyhive-0.1.5/honeyhive/sdk/datasets.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)      551 2023-03-05 06:42:19.000000 honeyhive-0.1.5/honeyhive/sdk/feedback.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)      711 2023-03-27 19:26:17.000000 honeyhive-0.1.5/honeyhive/sdk/fine_tuned_models.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     2551 2023-04-19 00:44:46.000000 honeyhive-0.1.5/honeyhive/sdk/generations.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)      243 2023-06-09 15:56:42.000000 honeyhive-0.1.5/honeyhive/sdk/init.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     1236 2023-03-27 19:28:28.000000 honeyhive-0.1.5/honeyhive/sdk/metrics.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     2352 2023-03-28 00:20:20.000000 honeyhive-0.1.5/honeyhive/sdk/projects.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     2415 2023-03-27 19:28:09.000000 honeyhive-0.1.5/honeyhive/sdk/prompts.py
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     5065 2023-03-26 17:31:47.000000 honeyhive-0.1.5/honeyhive/sdk/sdk-examples.py
+drwxr-xr-x   0 dhruvsingh   (501) staff       (20)        0 2023-07-19 15:35:31.378575 honeyhive-0.1.5/honeyhive.egg-info/
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     5542 2023-07-19 15:35:31.000000 honeyhive-0.1.5/honeyhive.egg-info/PKG-INFO
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)      981 2023-07-19 15:35:31.000000 honeyhive-0.1.5/honeyhive.egg-info/SOURCES.txt
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)        1 2023-07-19 15:35:31.000000 honeyhive-0.1.5/honeyhive.egg-info/dependency_links.txt
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)       54 2023-07-19 15:35:31.000000 honeyhive-0.1.5/honeyhive.egg-info/entry_points.txt
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)       75 2023-07-19 15:35:31.000000 honeyhive-0.1.5/honeyhive.egg-info/requires.txt
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)       10 2023-07-19 15:35:31.000000 honeyhive-0.1.5/honeyhive.egg-info/top_level.txt
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)      340 2023-03-05 06:49:29.000000 honeyhive-0.1.5/pyproject.toml
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)       38 2023-07-19 15:35:31.386582 honeyhive-0.1.5/setup.cfg
+-rw-r--r--   0 dhruvsingh   (501) staff       (20)     1634 2023-07-19 15:34:43.000000 honeyhive-0.1.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `honeyhive-0.1.3/PKG-INFO` & `honeyhive-0.1.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,158 +1,159 @@
 Metadata-Version: 2.1
 Name: honeyhive
-Version: 0.1.3
+Version: 0.1.5
 Summary: The HoneyHive SDK for Python
 Home-page: https://github.com/codehruv/honeyhive-sdk
 Author: HoneyHive
 Author-email: dhruv@honeyhive.ai
 License: Apache License 2.0
-Project-URL: Source, https://github.com/codehruv/honeyhive-sdk
 Project-URL: Documentation, https://docs.honeyhive.ai/
-Description: # HoneyHive Python SDK
-        
-        <div align="center">
-           <img src="https://user-images.githubusercontent.com/6267663/220803812-cd7e27bd-06cb-49b0-87c1-d85fe21a3557.png" />
-           <p>HoneyHive is a model observability and evaluation platform that helps you continuously improve your models in production. We help you evaluate, deploy, monitor and fine-tune both closed and open-source large language models for production use-cases, allowing you to optimize model performance & align your models with your users’ preferences.</p>
-           <a href="https://docs.honeyhive.ai/introduction"><img src="https://img.shields.io/static/v1?label=Docs&message=API Ref&color=fc9434&style=for-the-badge" /></a>
-        </div> 
-        
-        
-        ## SDK Installation
-        
-        ```bash
-        pip install honeyhive
-        ```
-        
-        ## Authentication
-        
-        After signing up on the app, you can find your API key in the [Settings page](https://app.honeyhive.ai/settings/account).
-        
-        ```python
-        import honeyhive
-        honeyhive.api_key = "HONEYHIVE_API_KEY"
-        honeyhive.openai_api_key = "OPENAI_API_KEY"
-        ```
-        
-        ## Usage
-        
-        Here we are assuming that you have a project setup in HoneyHive. If you don't, you can create one [here](https://app.honeyhive.ai/) by clicking on the `New Project` button.
-        
-        ### Generating a text completion via HoneyHive
-        
-        
-        #### Custom Prompt
-        
-        Adding HoneyHive is as simple as changing `openai.Completions.create` to `honeyhive.Completions.create`. Just make sure to specify which project associated with the generation.
-        
-        It's recommended to move the prompt to a template in our platform so that we can analyze user input distributions better.
-        
-        ```python
-        response = honeyhive.Completions.create(
-          project="Sandbox - Email Writer",
-          model="text-davinci-003",
-          prompt="Write an email to a colleague named Jill congratulating her on her promotion. The tone should be warm yet professional. Mention how you admire the work she's been putting in.  Include a joke about how her pet lizard Max enjoys eating grasshoppers. Mention how you're looking forward to the team off-site next week.",
-          temperature=0,
-          max_tokens=256,
-          top_p=1,
-          frequency_penalty=0,
-          presence_penalty=0
-        )
-        
-        generation_id = response.generation_id
-        ```
-        
-        
-        #### Deployed Prompt
-        
-        Assuming you have a prompt deployed for your project, you can generate it by calling `honeyhive.generations.generate(`
-        
-        ```python
-        response = honeyhive.generations.generate(
-            task="PROJECT_NAME",
-            input={
-                "EXAMPLE1": "input",
-                "EXAMPLE2": "input"
-            }
-        )
-        ```
-        
-        #### Specific Prompt
-        
-        If you want to generate a completion for a specific prompt, you can do so by calling `honeyhive.generations.generate(`
-        
-        ```python
-        response = honeyhive.generations.generate(
-            task="PROJECT_NAME",
-            input={
-                "EXAMPLE1": "input",
-                "EXAMPLE2": "input"
-            },
-            prompts=["PROMPT_NAME"]
-        )
-        ```
-        
-        ### Evaluating a text completion via HoneyHive
-        
-        For providing feedback on a generation, you can call `honeyhive.feedback(`
-        
-        ```python
-        response = honeyhive.feedback(
-            task="PROJECT_NAME",
-            generation_id=generation_id,
-            feedback={
-                "EXAMPLE1": "feedback",
-                "EXAMPLE2": True,
-            }
-        )
-        ```
-        
-        
-        ## SDK Capabilities
-        
-        ### Completions
-        `honeyhive.Completions.create` - calls OpenAI and logs the generation in HoneyHive
-        
-        ### Generations
-        `honeyhive.generations.generate` - generates a completion via HoneyHive
-        `honeyhive.generations.get_generations` - gets a pandas dataframe of all generations for a project
-        
-        ### Feedback
-        `honeyhive.feedback` - provides feedback on a generation
-        
-        ### Projects
-        `honeyhive.tasks.get_tasks` - gets a list of all projects
-        `honeyhive.tasks.get_task` - gets a specific project
-        `honeyhive.tasks.create_task` - creates a new project
-        `honeyhive.tasks.update_task` - updates a project
-        `honeyhive.tasks.delete_task` - deletes a project
-        
-        ### Prompts
-        `honeyhive.prompts.get_prompts` - gets a list of all prompts for a project
-        `honeyhive.prompts.create_prompt` - creates a new prompt for a project
-        `honeyhive.prompts.update_prompt` - updates a prompt for a project
-        `honeyhive.prompts.delete_prompt` - deletes a prompt for a project
-        
-        ### Metrics
-        `honeyhive.metrics.get_metrics` - gets a list of all metrics for a project
-        `honeyhive.metrics.create_metric` - creates a new metric for a project
-        `honeyhive.metrics.delete_metric` - deletes a metric for a project
-        
-        ### Datasets
-        `honeyhive.datasets.get_datasets` - gets a list of all datasets for a project
-        `honeyhive.datasets.get_dataset` - gets a specific dataset for a project
-        `honeyhive.datasets.create_dataset` - creates a new dataset for a project
-        `honeyhive.datasets.delete_dataset` - deletes a dataset for a project
-Platform: UNKNOWN
+Project-URL: Source, https://github.com/codehruv/honeyhive-sdk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >= 3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# HoneyHive Python SDK
+
+<div align="center">
+   <img src="https://user-images.githubusercontent.com/6267663/220803812-cd7e27bd-06cb-49b0-87c1-d85fe21a3557.png" />
+   <p>HoneyHive is a model observability and evaluation platform that helps you continuously improve your models in production. We help you evaluate, deploy, monitor and fine-tune both closed and open-source large language models for production use-cases, allowing you to optimize model performance & align your models with your users’ preferences.</p>
+   <a href="https://docs.honeyhive.ai/introduction"><img src="https://img.shields.io/static/v1?label=Docs&message=API Ref&color=fc9434&style=for-the-badge" /></a>
+</div> 
+
+
+## SDK Installation
+
+```bash
+pip install honeyhive
+```
+
+## Authentication
+
+After signing up on the app, you can find your API key in the [Settings page](https://app.honeyhive.ai/settings/account).
+
+```python
+import honeyhive
+honeyhive.api_key = "HONEYHIVE_API_KEY"
+honeyhive.openai_api_key = "OPENAI_API_KEY"
+```
+
+## Usage
+
+Here we are assuming that you have a project setup in HoneyHive. If you don't, you can create one [here](https://app.honeyhive.ai/) by clicking on the `New Project` button.
+
+### Generating a text completion via HoneyHive
+
+
+#### Custom Prompt
+
+Adding HoneyHive is as simple as changing `openai.Completions.create` to `honeyhive.Completions.create`. Just make sure to specify which project associated with the generation.
+
+It's recommended to move the prompt to a template in our platform so that we can analyze user input distributions better.
+
+```python
+response = honeyhive.Completions.create(
+  project="Sandbox - Email Writer",
+  model="text-davinci-003",
+  prompt="Write an email to a colleague named Jill congratulating her on her promotion. The tone should be warm yet professional. Mention how you admire the work she's been putting in.  Include a joke about how her pet lizard Max enjoys eating grasshoppers. Mention how you're looking forward to the team off-site next week.",
+  temperature=0,
+  max_tokens=256,
+  top_p=1,
+  frequency_penalty=0,
+  presence_penalty=0
+)
+
+generation_id = response.generation_id
+```
+
+
+#### Deployed Prompt
+
+Assuming you have a prompt deployed for your project, you can generate it by calling `honeyhive.generations.generate(`
+
+```python
+response = honeyhive.generations.generate(
+    task="PROJECT_NAME",
+    input={
+        "EXAMPLE1": "input",
+        "EXAMPLE2": "input"
+    }
+)
+```
+
+#### Specific Prompt
+
+If you want to generate a completion for a specific prompt, you can do so by calling `honeyhive.generations.generate(`
+
+```python
+response = honeyhive.generations.generate(
+    task="PROJECT_NAME",
+    input={
+        "EXAMPLE1": "input",
+        "EXAMPLE2": "input"
+    },
+    prompts=["PROMPT_NAME"]
+)
+```
+
+### Evaluating a text completion via HoneyHive
+
+For providing feedback on a generation, you can call `honeyhive.feedback(`
+
+```python
+response = honeyhive.feedback(
+    task="PROJECT_NAME",
+    generation_id=generation_id,
+    feedback={
+        "EXAMPLE1": "feedback",
+        "EXAMPLE2": True,
+    }
+)
+```
+
+
+## SDK Capabilities
+
+### Completions
+`honeyhive.Completions.create` - calls OpenAI and logs the generation in HoneyHive
+
+### Generations
+`honeyhive.generations.generate` - generates a completion via HoneyHive
+`honeyhive.generations.get_generations` - gets a pandas dataframe of all generations for a project
+
+### Feedback
+`honeyhive.feedback` - provides feedback on a generation
+
+### Projects
+`honeyhive.tasks.get_tasks` - gets a list of all projects
+`honeyhive.tasks.get_task` - gets a specific project
+`honeyhive.tasks.create_task` - creates a new project
+`honeyhive.tasks.update_task` - updates a project
+`honeyhive.tasks.delete_task` - deletes a project
+
+### Prompts
+`honeyhive.prompts.get_prompts` - gets a list of all prompts for a project
+`honeyhive.prompts.create_prompt` - creates a new prompt for a project
+`honeyhive.prompts.update_prompt` - updates a prompt for a project
+`honeyhive.prompts.delete_prompt` - deletes a prompt for a project
+
+### Metrics
+`honeyhive.metrics.get_metrics` - gets a list of all metrics for a project
+`honeyhive.metrics.create_metric` - creates a new metric for a project
+`honeyhive.metrics.delete_metric` - deletes a metric for a project
+
+### Datasets
+`honeyhive.datasets.get_datasets` - gets a list of all datasets for a project
+`honeyhive.datasets.get_dataset` - gets a specific dataset for a project
+`honeyhive.datasets.create_dataset` - creates a new dataset for a project
+`honeyhive.datasets.delete_dataset` - deletes a dataset for a project
```

#### html2text {}

```diff
@@ -1,12 +1,21 @@
-Metadata-Version: 2.1 Name: honeyhive Version: 0.1.3 Summary: The HoneyHive SDK
+Metadata-Version: 2.1 Name: honeyhive Version: 0.1.5 Summary: The HoneyHive SDK
 for Python Home-page: https://github.com/codehruv/honeyhive-sdk Author:
 HoneyHive Author-email: dhruv@honeyhive.ai License: Apache License 2.0 Project-
-URL: Source, https://github.com/codehruv/honeyhive-sdk Project-URL:
-Documentation, https://docs.honeyhive.ai/ Description: # HoneyHive Python SDK
+URL: Documentation, https://docs.honeyhive.ai/ Project-URL: Source, https://
+github.com/codehruv/honeyhive-sdk Classifier: Development Status :: 5 -
+Production/Stable Classifier: Intended Audience :: Developers Classifier:
+Natural Language :: English Classifier: License :: OSI Approved :: Apache
+Software License Classifier: Programming Language :: Python Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
+Python: >= 3.7 Description-Content-Type: text/markdown License-File: LICENSE #
+HoneyHive Python SDK
   [https://user-images.githubusercontent.com/6267663/220803812-cd7e27bd-06cb-
                           49b0-87c1-d85fe21a3557.png]
    HoneyHive is a model observability and evaluation platform that helps you
  continuously improve your models in production. We help you evaluate, deploy,
   monitor and fine-tune both closed and open-source large language models for
  production use-cases, allowing you to optimize model performance & align your
                     models with your usersâ preferences.
@@ -59,17 +68,8 @@
 project `honeyhive.prompts.delete_prompt` - deletes a prompt for a project ###
 Metrics `honeyhive.metrics.get_metrics` - gets a list of all metrics for a
 project `honeyhive.metrics.create_metric` - creates a new metric for a project
 `honeyhive.metrics.delete_metric` - deletes a metric for a project ### Datasets
 `honeyhive.datasets.get_datasets` - gets a list of all datasets for a project
 `honeyhive.datasets.get_dataset` - gets a specific dataset for a project
 `honeyhive.datasets.create_dataset` - creates a new dataset for a project
-`honeyhive.datasets.delete_dataset` - deletes a dataset for a project Platform:
-UNKNOWN Classifier: Development Status :: 5 - Production/Stable Classifier:
-Intended Audience :: Developers Classifier: Natural Language :: English
-Classifier: License :: OSI Approved :: Apache Software License Classifier:
-Programming Language :: Python Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Requires-Python: >= 3.7 Description-Content-Type:
-text/markdown
+`honeyhive.datasets.delete_dataset` - deletes a dataset for a project
```

### Comparing `honeyhive-0.1.3/honeyhive.egg-info/PKG-INFO` & `honeyhive-0.1.5/honeyhive.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,158 +1,159 @@
 Metadata-Version: 2.1
 Name: honeyhive
-Version: 0.1.3
+Version: 0.1.5
 Summary: The HoneyHive SDK for Python
 Home-page: https://github.com/codehruv/honeyhive-sdk
 Author: HoneyHive
 Author-email: dhruv@honeyhive.ai
 License: Apache License 2.0
-Project-URL: Source, https://github.com/codehruv/honeyhive-sdk
 Project-URL: Documentation, https://docs.honeyhive.ai/
-Description: # HoneyHive Python SDK
-        
-        <div align="center">
-           <img src="https://user-images.githubusercontent.com/6267663/220803812-cd7e27bd-06cb-49b0-87c1-d85fe21a3557.png" />
-           <p>HoneyHive is a model observability and evaluation platform that helps you continuously improve your models in production. We help you evaluate, deploy, monitor and fine-tune both closed and open-source large language models for production use-cases, allowing you to optimize model performance & align your models with your users’ preferences.</p>
-           <a href="https://docs.honeyhive.ai/introduction"><img src="https://img.shields.io/static/v1?label=Docs&message=API Ref&color=fc9434&style=for-the-badge" /></a>
-        </div> 
-        
-        
-        ## SDK Installation
-        
-        ```bash
-        pip install honeyhive
-        ```
-        
-        ## Authentication
-        
-        After signing up on the app, you can find your API key in the [Settings page](https://app.honeyhive.ai/settings/account).
-        
-        ```python
-        import honeyhive
-        honeyhive.api_key = "HONEYHIVE_API_KEY"
-        honeyhive.openai_api_key = "OPENAI_API_KEY"
-        ```
-        
-        ## Usage
-        
-        Here we are assuming that you have a project setup in HoneyHive. If you don't, you can create one [here](https://app.honeyhive.ai/) by clicking on the `New Project` button.
-        
-        ### Generating a text completion via HoneyHive
-        
-        
-        #### Custom Prompt
-        
-        Adding HoneyHive is as simple as changing `openai.Completions.create` to `honeyhive.Completions.create`. Just make sure to specify which project associated with the generation.
-        
-        It's recommended to move the prompt to a template in our platform so that we can analyze user input distributions better.
-        
-        ```python
-        response = honeyhive.Completions.create(
-          project="Sandbox - Email Writer",
-          model="text-davinci-003",
-          prompt="Write an email to a colleague named Jill congratulating her on her promotion. The tone should be warm yet professional. Mention how you admire the work she's been putting in.  Include a joke about how her pet lizard Max enjoys eating grasshoppers. Mention how you're looking forward to the team off-site next week.",
-          temperature=0,
-          max_tokens=256,
-          top_p=1,
-          frequency_penalty=0,
-          presence_penalty=0
-        )
-        
-        generation_id = response.generation_id
-        ```
-        
-        
-        #### Deployed Prompt
-        
-        Assuming you have a prompt deployed for your project, you can generate it by calling `honeyhive.generations.generate(`
-        
-        ```python
-        response = honeyhive.generations.generate(
-            task="PROJECT_NAME",
-            input={
-                "EXAMPLE1": "input",
-                "EXAMPLE2": "input"
-            }
-        )
-        ```
-        
-        #### Specific Prompt
-        
-        If you want to generate a completion for a specific prompt, you can do so by calling `honeyhive.generations.generate(`
-        
-        ```python
-        response = honeyhive.generations.generate(
-            task="PROJECT_NAME",
-            input={
-                "EXAMPLE1": "input",
-                "EXAMPLE2": "input"
-            },
-            prompts=["PROMPT_NAME"]
-        )
-        ```
-        
-        ### Evaluating a text completion via HoneyHive
-        
-        For providing feedback on a generation, you can call `honeyhive.feedback(`
-        
-        ```python
-        response = honeyhive.feedback(
-            task="PROJECT_NAME",
-            generation_id=generation_id,
-            feedback={
-                "EXAMPLE1": "feedback",
-                "EXAMPLE2": True,
-            }
-        )
-        ```
-        
-        
-        ## SDK Capabilities
-        
-        ### Completions
-        `honeyhive.Completions.create` - calls OpenAI and logs the generation in HoneyHive
-        
-        ### Generations
-        `honeyhive.generations.generate` - generates a completion via HoneyHive
-        `honeyhive.generations.get_generations` - gets a pandas dataframe of all generations for a project
-        
-        ### Feedback
-        `honeyhive.feedback` - provides feedback on a generation
-        
-        ### Projects
-        `honeyhive.tasks.get_tasks` - gets a list of all projects
-        `honeyhive.tasks.get_task` - gets a specific project
-        `honeyhive.tasks.create_task` - creates a new project
-        `honeyhive.tasks.update_task` - updates a project
-        `honeyhive.tasks.delete_task` - deletes a project
-        
-        ### Prompts
-        `honeyhive.prompts.get_prompts` - gets a list of all prompts for a project
-        `honeyhive.prompts.create_prompt` - creates a new prompt for a project
-        `honeyhive.prompts.update_prompt` - updates a prompt for a project
-        `honeyhive.prompts.delete_prompt` - deletes a prompt for a project
-        
-        ### Metrics
-        `honeyhive.metrics.get_metrics` - gets a list of all metrics for a project
-        `honeyhive.metrics.create_metric` - creates a new metric for a project
-        `honeyhive.metrics.delete_metric` - deletes a metric for a project
-        
-        ### Datasets
-        `honeyhive.datasets.get_datasets` - gets a list of all datasets for a project
-        `honeyhive.datasets.get_dataset` - gets a specific dataset for a project
-        `honeyhive.datasets.create_dataset` - creates a new dataset for a project
-        `honeyhive.datasets.delete_dataset` - deletes a dataset for a project
-Platform: UNKNOWN
+Project-URL: Source, https://github.com/codehruv/honeyhive-sdk
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >= 3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# HoneyHive Python SDK
+
+<div align="center">
+   <img src="https://user-images.githubusercontent.com/6267663/220803812-cd7e27bd-06cb-49b0-87c1-d85fe21a3557.png" />
+   <p>HoneyHive is a model observability and evaluation platform that helps you continuously improve your models in production. We help you evaluate, deploy, monitor and fine-tune both closed and open-source large language models for production use-cases, allowing you to optimize model performance & align your models with your users’ preferences.</p>
+   <a href="https://docs.honeyhive.ai/introduction"><img src="https://img.shields.io/static/v1?label=Docs&message=API Ref&color=fc9434&style=for-the-badge" /></a>
+</div> 
+
+
+## SDK Installation
+
+```bash
+pip install honeyhive
+```
+
+## Authentication
+
+After signing up on the app, you can find your API key in the [Settings page](https://app.honeyhive.ai/settings/account).
+
+```python
+import honeyhive
+honeyhive.api_key = "HONEYHIVE_API_KEY"
+honeyhive.openai_api_key = "OPENAI_API_KEY"
+```
+
+## Usage
+
+Here we are assuming that you have a project setup in HoneyHive. If you don't, you can create one [here](https://app.honeyhive.ai/) by clicking on the `New Project` button.
+
+### Generating a text completion via HoneyHive
+
+
+#### Custom Prompt
+
+Adding HoneyHive is as simple as changing `openai.Completions.create` to `honeyhive.Completions.create`. Just make sure to specify which project associated with the generation.
+
+It's recommended to move the prompt to a template in our platform so that we can analyze user input distributions better.
+
+```python
+response = honeyhive.Completions.create(
+  project="Sandbox - Email Writer",
+  model="text-davinci-003",
+  prompt="Write an email to a colleague named Jill congratulating her on her promotion. The tone should be warm yet professional. Mention how you admire the work she's been putting in.  Include a joke about how her pet lizard Max enjoys eating grasshoppers. Mention how you're looking forward to the team off-site next week.",
+  temperature=0,
+  max_tokens=256,
+  top_p=1,
+  frequency_penalty=0,
+  presence_penalty=0
+)
+
+generation_id = response.generation_id
+```
+
+
+#### Deployed Prompt
+
+Assuming you have a prompt deployed for your project, you can generate it by calling `honeyhive.generations.generate(`
+
+```python
+response = honeyhive.generations.generate(
+    task="PROJECT_NAME",
+    input={
+        "EXAMPLE1": "input",
+        "EXAMPLE2": "input"
+    }
+)
+```
+
+#### Specific Prompt
+
+If you want to generate a completion for a specific prompt, you can do so by calling `honeyhive.generations.generate(`
+
+```python
+response = honeyhive.generations.generate(
+    task="PROJECT_NAME",
+    input={
+        "EXAMPLE1": "input",
+        "EXAMPLE2": "input"
+    },
+    prompts=["PROMPT_NAME"]
+)
+```
+
+### Evaluating a text completion via HoneyHive
+
+For providing feedback on a generation, you can call `honeyhive.feedback(`
+
+```python
+response = honeyhive.feedback(
+    task="PROJECT_NAME",
+    generation_id=generation_id,
+    feedback={
+        "EXAMPLE1": "feedback",
+        "EXAMPLE2": True,
+    }
+)
+```
+
+
+## SDK Capabilities
+
+### Completions
+`honeyhive.Completions.create` - calls OpenAI and logs the generation in HoneyHive
+
+### Generations
+`honeyhive.generations.generate` - generates a completion via HoneyHive
+`honeyhive.generations.get_generations` - gets a pandas dataframe of all generations for a project
+
+### Feedback
+`honeyhive.feedback` - provides feedback on a generation
+
+### Projects
+`honeyhive.tasks.get_tasks` - gets a list of all projects
+`honeyhive.tasks.get_task` - gets a specific project
+`honeyhive.tasks.create_task` - creates a new project
+`honeyhive.tasks.update_task` - updates a project
+`honeyhive.tasks.delete_task` - deletes a project
+
+### Prompts
+`honeyhive.prompts.get_prompts` - gets a list of all prompts for a project
+`honeyhive.prompts.create_prompt` - creates a new prompt for a project
+`honeyhive.prompts.update_prompt` - updates a prompt for a project
+`honeyhive.prompts.delete_prompt` - deletes a prompt for a project
+
+### Metrics
+`honeyhive.metrics.get_metrics` - gets a list of all metrics for a project
+`honeyhive.metrics.create_metric` - creates a new metric for a project
+`honeyhive.metrics.delete_metric` - deletes a metric for a project
+
+### Datasets
+`honeyhive.datasets.get_datasets` - gets a list of all datasets for a project
+`honeyhive.datasets.get_dataset` - gets a specific dataset for a project
+`honeyhive.datasets.create_dataset` - creates a new dataset for a project
+`honeyhive.datasets.delete_dataset` - deletes a dataset for a project
```

#### html2text {}

```diff
@@ -1,12 +1,21 @@
-Metadata-Version: 2.1 Name: honeyhive Version: 0.1.3 Summary: The HoneyHive SDK
+Metadata-Version: 2.1 Name: honeyhive Version: 0.1.5 Summary: The HoneyHive SDK
 for Python Home-page: https://github.com/codehruv/honeyhive-sdk Author:
 HoneyHive Author-email: dhruv@honeyhive.ai License: Apache License 2.0 Project-
-URL: Source, https://github.com/codehruv/honeyhive-sdk Project-URL:
-Documentation, https://docs.honeyhive.ai/ Description: # HoneyHive Python SDK
+URL: Documentation, https://docs.honeyhive.ai/ Project-URL: Source, https://
+github.com/codehruv/honeyhive-sdk Classifier: Development Status :: 5 -
+Production/Stable Classifier: Intended Audience :: Developers Classifier:
+Natural Language :: English Classifier: License :: OSI Approved :: Apache
+Software License Classifier: Programming Language :: Python Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
+Python: >= 3.7 Description-Content-Type: text/markdown License-File: LICENSE #
+HoneyHive Python SDK
   [https://user-images.githubusercontent.com/6267663/220803812-cd7e27bd-06cb-
                           49b0-87c1-d85fe21a3557.png]
    HoneyHive is a model observability and evaluation platform that helps you
  continuously improve your models in production. We help you evaluate, deploy,
   monitor and fine-tune both closed and open-source large language models for
  production use-cases, allowing you to optimize model performance & align your
                     models with your usersâ preferences.
@@ -59,17 +68,8 @@
 project `honeyhive.prompts.delete_prompt` - deletes a prompt for a project ###
 Metrics `honeyhive.metrics.get_metrics` - gets a list of all metrics for a
 project `honeyhive.metrics.create_metric` - creates a new metric for a project
 `honeyhive.metrics.delete_metric` - deletes a metric for a project ### Datasets
 `honeyhive.datasets.get_datasets` - gets a list of all datasets for a project
 `honeyhive.datasets.get_dataset` - gets a specific dataset for a project
 `honeyhive.datasets.create_dataset` - creates a new dataset for a project
-`honeyhive.datasets.delete_dataset` - deletes a dataset for a project Platform:
-UNKNOWN Classifier: Development Status :: 5 - Production/Stable Classifier:
-Intended Audience :: Developers Classifier: Natural Language :: English
-Classifier: License :: OSI Approved :: Apache Software License Classifier:
-Programming Language :: Python Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Requires-Python: >= 3.7 Description-Content-Type:
-text/markdown
+`honeyhive.datasets.delete_dataset` - deletes a dataset for a project
```

### Comparing `honeyhive-0.1.3/honeyhive.egg-info/SOURCES.txt` & `honeyhive-0.1.5/honeyhive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `honeyhive-0.1.3/README.md` & `honeyhive-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `honeyhive-0.1.3/setup.py` & `honeyhive-0.1.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     'console_scripts': [
         'honeyhive = honeyhive.cli:honeyhive'
     ]
 }
 
 setup(
     name='honeyhive',
-    version='0.1.3',
+    version='0.1.5',
     description='The HoneyHive SDK for Python',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='HoneyHive',
     author_email="dhruv@honeyhive.ai",
     scripts=[],
     url='https://github.com/codehruv/honeyhive-sdk',
```

### Comparing `honeyhive-0.1.3/honeyhive/sdk/sdk-examples.py` & `honeyhive-0.1.5/honeyhive/sdk/sdk-examples.py`

 * *Files identical despite different names*

### Comparing `honeyhive-0.1.3/honeyhive/sdk/metrics.py` & `honeyhive-0.1.5/honeyhive/sdk/metrics.py`

 * *Files identical despite different names*

### Comparing `honeyhive-0.1.3/honeyhive/sdk/Completion.py` & `honeyhive-0.1.5/honeyhive/sdk/Completion.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import honeyhive 
 
 def create(
     project: str,
     model: str,
     prompt: str or List[str],
     source: Optional[str] = None,
+    version: Optional[str] = None,
     engine: Optional[str] = None,
     max_tokens: Optional[int] = 16,
     temperature: Optional[float] = 1.0,
     top_p: Optional[float] = 1.0,
     suffix: Optional[str] = None,
     presence_penalty: Optional[float] = 0.0,
     frequency_penalty: Optional[float] = 0.0,
@@ -81,14 +82,15 @@
             model=model,
             prompt=prompt,
             hyperparameters=args_for_honeyhive,
             generation=response.choices[0].text,
             usage=response.usage,
             latency=latency,
             source=source,
+            version=version
         )
     )
     generation_id = honeyhive_response.generation_id
 
     # add generation_id to openai's response
     response.generation_id = generation_id
```

### Comparing `honeyhive-0.1.3/honeyhive/sdk/generations.py` & `honeyhive-0.1.5/honeyhive/sdk/generations.py`

 * *Files 15% similar despite different names*

```diff
@@ -39,11 +39,49 @@
     import pandas as pd
     df = pd.DataFrame(generations_list)
     df.columns = df.iloc[0].apply(lambda x: x[0])
     df = df.applymap(lambda x: x[1] if isinstance(x, tuple) else x)
 
     return df
 
+def log(
+    project: str,
+    model: str,
+    generation: str,
+    hyperparameters: Dict[str, Any],
+    prompt_template: Optional[str] = None,
+    inputs: Optional[Dict[str, Any]] = None,
+    prompt: Optional[str] = None,
+    usage: Optional[Dict[str, Any]] = None,
+    source: Optional[str] = None,
+    latency: Optional[float] = None,
+) -> GenerationResponse:
+    # log generation via honeyhive
+    client = honeyhive_client()
+
+    if prompt == None:
+        prompt = prompt_template
+        if inputs == None and prompt_template == None:
+            # throw an exception
+            return Exception("Please provide either a complete prompt or prompt template with inputs")
+    
+    honeyhive_response = client.log_generation(
+        generation=GenerationLoggingQuery(
+            task=project,
+            model=model,
+            prompt=prompt,
+            inputs=inputs,
+            hyperparameters=hyperparameters,
+            generation=generation,
+            usage=usage,
+            latency=latency,
+            source=source,
+        )
+    )
+
+    return honeyhive_response
+
 __all__ = [
     "generate",
+    "log",
     "get_generations"
 ]
```

### Comparing `honeyhive-0.1.3/honeyhive/sdk/feedback.py` & `honeyhive-0.1.5/honeyhive/sdk/feedback.py`

 * *Files identical despite different names*

### Comparing `honeyhive-0.1.3/honeyhive/sdk/ChatCompletion.py` & `honeyhive-0.1.5/honeyhive/sdk/ChatCompletion.py`

 * *Files identical despite different names*

### Comparing `honeyhive-0.1.3/honeyhive/sdk/datasets.py` & `honeyhive-0.1.5/honeyhive/sdk/datasets.py`

 * *Files identical despite different names*

### Comparing `honeyhive-0.1.3/honeyhive/sdk/__init__.py` & `honeyhive-0.1.5/honeyhive/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `honeyhive-0.1.3/honeyhive/sdk/prompts.py` & `honeyhive-0.1.5/honeyhive/sdk/prompts.py`

 * *Files identical despite different names*

### Comparing `honeyhive-0.1.3/honeyhive/sdk/fine_tuned_models.py` & `honeyhive-0.1.5/honeyhive/sdk/fine_tuned_models.py`

 * *Files identical despite different names*

### Comparing `honeyhive-0.1.3/honeyhive/sdk/projects.py` & `honeyhive-0.1.5/honeyhive/sdk/projects.py`

 * *Files identical despite different names*

### Comparing `honeyhive-0.1.3/honeyhive/api/client.py` & `honeyhive-0.1.5/honeyhive/api/client.py`

 * *Files identical despite different names*

### Comparing `honeyhive-0.1.3/honeyhive/api/models/metrics.py` & `honeyhive-0.1.5/honeyhive/api/models/metrics.py`

 * *Files identical despite different names*

### Comparing `honeyhive-0.1.3/honeyhive/api/models/tasks.py` & `honeyhive-0.1.5/honeyhive/api/models/tasks.py`

 * *Files identical despite different names*

### Comparing `honeyhive-0.1.3/honeyhive/api/models/generations.py` & `honeyhive-0.1.5/honeyhive/api/models/generations.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,14 +103,18 @@
         title="Usage",
         description="The token usage for the generation"
     )
     source: Optional[str] = Field(
         title="Source",
         description="The source of the generation"
     )
+    version: Optional[str] = Field(
+        title="Version",
+        description="The version of the prompt"
+    )
     latency: Optional[float] = Field(
         title="Latency",
         description="The latency of the generation in milliseconds"
     )
 
 
 class Generation(BaseModel):
```

### Comparing `honeyhive-0.1.3/honeyhive/api/models/feedback.py` & `honeyhive-0.1.5/honeyhive/api/models/feedback.py`

 * *Files identical despite different names*

### Comparing `honeyhive-0.1.3/honeyhive/api/models/datasets.py` & `honeyhive-0.1.5/honeyhive/api/models/datasets.py`

 * *Files identical despite different names*

### Comparing `honeyhive-0.1.3/honeyhive/api/models/prompts.py` & `honeyhive-0.1.5/honeyhive/api/models/prompts.py`

 * *Files identical despite different names*

### Comparing `honeyhive-0.1.3/honeyhive/api/models/fine_tuned_models.py` & `honeyhive-0.1.5/honeyhive/api/models/fine_tuned_models.py`

 * *Files identical despite different names*

