# Comparing `tmp/llm_client-0.6.2.tar.gz` & `tmp/llm_client-0.7.0.tar.gz`

## Comparing `llm_client-0.6.2.tar` & `llm_client-0.7.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 llm_client-0.6.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 llm_client-0.6.2/.github/workflows/test.yml
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 llm_client-0.6.2/llm_client/__init__.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 llm_client-0.6.2/llm_client/base_llm_client.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 llm_client-0.6.2/llm_client/consts.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.2/llm_client/llm_api_client/__init__.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 llm_client-0.6.2/llm_client/llm_api_client/ai21_client.py
--rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 llm_client-0.6.2/llm_client/llm_api_client/aleph_alpha_client.py
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 llm_client-0.6.2/llm_client/llm_api_client/anthropic_client.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 llm_client-0.6.2/llm_client/llm_api_client/base_llm_api_client.py
--rw-r--r--   0        0        0     4199 2020-02-02 00:00:00.000000 llm_client-0.6.2/llm_client/llm_api_client/google_client.py
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 llm_client-0.6.2/llm_client/llm_api_client/huggingface_client.py
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 llm_client-0.6.2/llm_client/llm_api_client/llm_api_client_factory.py
--rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 llm_client-0.6.2/llm_client/llm_api_client/openai_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.2/llm_client/llm_client/__init__.py
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 llm_client-0.6.2/llm_client/llm_client/local_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.2/llm_client/sync/__init__.py
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 llm_client-0.6.2/llm_client/sync/sync_llm_api_client_factory.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/llm_api_client/__init__.py
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/llm_api_client/conftest.py
--rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/llm_api_client/test_llm_api_client_factory.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/llm_api_client/ai21_client/__init__.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/llm_api_client/ai21_client/conftest.py
--rw-r--r--   0        0        0     4912 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/llm_api_client/ai21_client/test_ai21.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/llm_api_client/anthropic_client/__init__.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/llm_api_client/anthropic_client/conftest.py
--rw-r--r--   0        0        0     5677 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/llm_api_client/anthropic_client/test_anthropic_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/llm_api_client/google_client/__init__.py
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/llm_api_client/google_client/conftest.py
--rw-r--r--   0        0        0    10201 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/llm_api_client/google_client/test_google_client.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/llm_api_client/huggingface_client/__init__.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/llm_api_client/huggingface_client/conftest.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/llm_api_client/huggingface_client/test_huggingface.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/llm_api_client/openai_client/__init__.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/llm_api_client/openai_client/conftest.py
--rw-r--r--   0        0        0     8948 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/llm_api_client/openai_client/test_openai.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/llm_client/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/llm_client/local_client/__init__.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/llm_client/local_client/conftest.py
--rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/llm_client/local_client/test_local_client.py
--rw-r--r--   0        0        0    11156 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/resources/ai21/text_completion.json
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/resources/ai21/tokenize.json
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/resources/google/chat_completion.json
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/resources/google/embedding.json
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/resources/google/text_completion.json
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/resources/google/tokens_count.json
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/resources/huggingface/text_completion.json
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/resources/openai/chat_completion.json
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/resources/openai/text_completion.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/test_utils/__init__.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 llm_client-0.6.2/tests/test_utils/load_json_resource.py
--rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 llm_client-0.6.2/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 llm_client-0.6.2/LICENSE
--rw-r--r--   0        0        0     7870 2020-02-02 00:00:00.000000 llm_client-0.6.2/README.md
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 llm_client-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     9561 2020-02-02 00:00:00.000000 llm_client-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 llm_client-0.7.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 llm_client-0.7.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 llm_client-0.7.0/llm_client/__init__.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 llm_client-0.7.0/llm_client/base_llm_client.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 llm_client-0.7.0/llm_client/consts.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.7.0/llm_client/llm_api_client/__init__.py
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 llm_client-0.7.0/llm_client/llm_api_client/ai21_client.py
+-rw-r--r--   0        0        0     3159 2020-02-02 00:00:00.000000 llm_client-0.7.0/llm_client/llm_api_client/aleph_alpha_client.py
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 llm_client-0.7.0/llm_client/llm_api_client/anthropic_client.py
+-rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 llm_client-0.7.0/llm_client/llm_api_client/base_llm_api_client.py
+-rw-r--r--   0        0        0     4282 2020-02-02 00:00:00.000000 llm_client-0.7.0/llm_client/llm_api_client/google_client.py
+-rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 llm_client-0.7.0/llm_client/llm_api_client/huggingface_client.py
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 llm_client-0.7.0/llm_client/llm_api_client/llm_api_client_factory.py
+-rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 llm_client-0.7.0/llm_client/llm_api_client/openai_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.7.0/llm_client/llm_client/__init__.py
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 llm_client-0.7.0/llm_client/llm_client/local_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.7.0/llm_client/sync/__init__.py
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 llm_client-0.7.0/llm_client/sync/sync_llm_api_client_factory.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/llm_api_client/__init__.py
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/llm_api_client/conftest.py
+-rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/llm_api_client/test_llm_api_client_factory.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/llm_api_client/ai21_client/__init__.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/llm_api_client/ai21_client/conftest.py
+-rw-r--r--   0        0        0     4960 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/llm_api_client/ai21_client/test_ai21.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/llm_api_client/anthropic_client/__init__.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/llm_api_client/anthropic_client/conftest.py
+-rw-r--r--   0        0        0     5702 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/llm_api_client/anthropic_client/test_anthropic_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/llm_api_client/google_client/__init__.py
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/llm_api_client/google_client/conftest.py
+-rw-r--r--   0        0        0    10228 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/llm_api_client/google_client/test_google_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/llm_api_client/huggingface_client/__init__.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/llm_api_client/huggingface_client/conftest.py
+-rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/llm_api_client/huggingface_client/test_huggingface.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/llm_api_client/openai_client/__init__.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/llm_api_client/openai_client/conftest.py
+-rw-r--r--   0        0        0     9036 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/llm_api_client/openai_client/test_openai.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/llm_client/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/llm_client/local_client/__init__.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/llm_client/local_client/conftest.py
+-rw-r--r--   0        0        0     4659 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/llm_client/local_client/test_local_client.py
+-rw-r--r--   0        0        0    11156 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/resources/ai21/text_completion.json
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/resources/ai21/tokenize.json
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/resources/google/chat_completion.json
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/resources/google/embedding.json
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/resources/google/text_completion.json
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/resources/google/tokens_count.json
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/resources/huggingface/text_completion.json
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/resources/openai/chat_completion.json
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/resources/openai/text_completion.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/test_utils/__init__.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 llm_client-0.7.0/tests/test_utils/load_json_resource.py
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 llm_client-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 llm_client-0.7.0/LICENSE
+-rw-r--r--   0        0        0     7822 2020-02-02 00:00:00.000000 llm_client-0.7.0/README.md
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 llm_client-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     9513 2020-02-02 00:00:00.000000 llm_client-0.7.0/PKG-INFO
```

### Comparing `llm_client-0.6.2/.github/workflows/python-publish.yml` & `llm_client-0.7.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `llm_client-0.6.2/.github/workflows/test.yml` & `llm_client-0.7.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `llm_client-0.6.2/llm_client/__init__.py` & `llm_client-0.7.0/llm_client/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.6.2"
+__version__ = "0.7.0"
 
 from llm_client.base_llm_client import BaseLLMClient
 
 # load api clients
 try:
     from llm_client.llm_api_client.base_llm_api_client import BaseLLMAPIClient, LLMAPIClientConfig
     from llm_client.llm_api_client.llm_api_client_factory import LLMAPIClientFactory, LLMAPIClientType
```

### Comparing `llm_client-0.6.2/llm_client/llm_api_client/ai21_client.py` & `llm_client-0.7.0/llm_client/llm_api_client/ai21_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,17 +18,18 @@
     def __init__(self, config: LLMAPIClientConfig):
         super().__init__(config)
         if self._base_url is None:
             self._base_url = BASE_URL
         self._headers[AUTH_HEADER] = BEARER_TOKEN + self._api_key
 
     async def text_completion(self, prompt: str, model: Optional[str] = None, max_tokens: int = 16,
-                              temperature: float = 0.7, **kwargs) -> list[str]:
+                              temperature: float = 0.7, top_p: float = 1,**kwargs) -> list[str]:
         model = model or self._default_model
         kwargs[PROMPT_KEY] = prompt
+        kwargs["topP"] = kwargs.pop("topP", top_p)
         kwargs["maxTokens"] = kwargs.pop("maxTokens", max_tokens)
         kwargs["temperature"] = temperature
         response = await self._session.post(self._base_url + model + "/" + COMPLETE_PATH,
                                             json=kwargs,
                                             headers=self._headers,
                                             raise_for_status=True)
         response_json = await response.json()
```

### Comparing `llm_client-0.6.2/llm_client/llm_api_client/aleph_alpha_client.py` & `llm_client-0.7.0/llm_client/llm_api_client/aleph_alpha_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,20 +23,21 @@
     def __init__(self, config: LLMAPIClientConfig):
         super().__init__(config)
         if self._base_url is None:
             self._base_url = BASE_URL
         self._headers[AUTH_HEADER] = BEARER_TOKEN + self._api_key
 
     async def text_completion(self, prompt: str, model: Optional[str] = None, max_tokens: Optional[int] = None,
-                              temperature: float = 0, **kwargs) -> \
+                              temperature: float = 0,top_p: float = 0, **kwargs) -> \
             list[str]:
         self._set_model_in_kwargs(kwargs, model)
         if max_tokens is None:
             raise ValueError("max_tokens must be specified")
         kwargs[PROMPT_KEY] = prompt
+        kwargs["top_p"] = top_p
         kwargs["maximum_tokens"] = kwargs.pop("maximum_tokens", max_tokens)
         kwargs["temperature"] = temperature
         response = await self._session.post(self._base_url + COMPLETE_PATH,
                                             json=kwargs,
                                             headers=self._headers,
                                             raise_for_status=True)
         response_json = await response.json()
```

### Comparing `llm_client-0.6.2/llm_client/llm_api_client/anthropic_client.py` & `llm_client-0.7.0/llm_client/llm_api_client/anthropic_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,19 +23,21 @@
         self._anthropic = AsyncAnthropic()
         if self._headers.get(VERSION_HEADER) is None:
             self._headers[VERSION_HEADER] = self._anthropic.default_headers[VERSION_HEADER]
         self._headers[ACCEPT_HEADER] = ACCEPT_VALUE
         self._headers[AUTH_HEADER] = self._api_key
 
     async def text_completion(self, prompt: str, model: Optional[str] = None, max_tokens: Optional[int] = None,
-                              temperature: float = 1,
+                              temperature: float = 1, top_p: Optional[float] = None,
                               **kwargs) -> \
             list[str]:
         if max_tokens is None and kwargs.get(MAX_TOKENS_KEY) is None:
             raise ValueError(f"max_tokens or {MAX_TOKENS_KEY} must be specified")
+        if top_p:
+            kwargs["top_p"] = top_p
         self._set_model_in_kwargs(kwargs, model)
         kwargs[PROMPT_KEY] = prompt
         kwargs[MAX_TOKENS_KEY] = kwargs.pop(MAX_TOKENS_KEY, max_tokens)
         kwargs["temperature"] = temperature
         response = await self._session.post(self._base_url + COMPLETE_PATH,
                                             json=kwargs,
                                             headers=self._headers,
```

### Comparing `llm_client-0.6.2/llm_client/llm_api_client/base_llm_api_client.py` & `llm_client-0.7.0/llm_client/llm_api_client/base_llm_api_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         self._session: ClientSession = config.session
         self._base_url: str = config.base_url
         self._default_model: str = config.default_model
         self._headers: dict[str, str] = config.headers
 
     @abstractmethod
     async def text_completion(self, prompt: str, model: Optional[str] = None, max_tokens: Optional[int] = None,
-                              temperature: Optional[float] = None, **kwargs) -> list[str]:
+                              temperature: Optional[float] = None, top_p: Optional[float] = None, **kwargs) -> list[str]:
         raise NotImplementedError()
 
     async def embedding(self, text: str, model: Optional[str] = None, **kwargs) -> list[float]:
         raise NotImplementedError()
 
     def _set_model_in_kwargs(self, kwargs, model: Optional[str]) -> None:
         if model is not None:
```

### Comparing `llm_client-0.6.2/llm_client/llm_api_client/google_client.py` & `llm_client-0.7.0/llm_client/llm_api_client/google_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,18 +29,20 @@
     def __init__(self, config: LLMAPIClientConfig):
         super().__init__(config)
         if self._base_url is None:
             self._base_url = BASE_URL
         self._params = {AUTH_PARAM: self._api_key}
 
     async def text_completion(self, prompt: str, model: Optional[str] = None, max_tokens: Optional[int] = 64,
-                              temperature: Optional[float] = None, **kwargs) -> list[str]:
+                              temperature: Optional[float] = None,top_p: Optional[float] = None, **kwargs) -> list[str]:
         model = model or self._default_model
         kwargs[PROMPT_KEY] = {TEXT_KEY: prompt}
         kwargs[MAX_TOKENS_KEY] = kwargs.pop(MAX_TOKENS_KEY, max_tokens)
+        if top_p:
+            kwargs["topP"] = top_p
         kwargs["temperature"] = kwargs.pop("temperature", temperature)
         response = await self._session.post(self._base_url + model + ":" + COMPLETE_PATH,
                                             params=self._params,
                                             json=kwargs,
                                             headers=self._headers,
                                             raise_for_status=True)
         response_json = await response.json()
```

### Comparing `llm_client-0.6.2/llm_client/llm_api_client/huggingface_client.py` & `llm_client-0.7.0/llm_client/llm_api_client/huggingface_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,16 +25,17 @@
         if self._base_url is None:
             self._base_url = BASE_URL
         if self._default_model is None:
             self._default_model = DEFAULT_MODEL
         self._headers[AUTH_HEADER] = BEARER_TOKEN + self._api_key
 
     async def text_completion(self, prompt: str, max_tokens: Optional[int] = None, temperature: float = 1.0,
-                              model: Optional[str] = None, **kwargs) -> list[str]:
+                              model: Optional[str] = None, top_p: Optional[float] = None, **kwargs) -> list[str]:
         model = model or self._default_model
+        kwargs["top_p"] = top_p
         kwargs[INPUT_KEY] = prompt
         kwargs[TEMPERATURE_KEY] = temperature
         kwargs[TOKENS_KEY] = kwargs.pop(TOKENS_KEY, max_tokens)
         response = await self._session.post(self._base_url + model + CONST_SLASH,
                                             json=kwargs,
                                             headers=self._headers,
                                             raise_for_status=True)
```

### Comparing `llm_client-0.6.2/llm_client/llm_api_client/llm_api_client_factory.py` & `llm_client-0.7.0/llm_client/llm_api_client/llm_api_client_factory.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.6.2/llm_client/llm_api_client/openai_client.py` & `llm_client-0.7.0/llm_client/llm_api_client/openai_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,27 +32,29 @@
     def __init__(self, config: LLMAPIClientConfig):
         super().__init__(config)
         openai.api_key = self._api_key
         openai.aiosession.set(self._session)
         self._client = openai
 
     async def text_completion(self, prompt: str, model: Optional[str] = None, temperature: float = 0,
-                              max_tokens: int = 16, **kwargs) -> list[str]:
+                              max_tokens: int = 16, top_p: float = 1, **kwargs) -> list[str]:
         self._set_model_in_kwargs(kwargs, model)
         kwargs[PROMPT_KEY] = prompt
+        kwargs["top_p"] = top_p
         kwargs["temperature"] = temperature
         kwargs["max_tokens"] = max_tokens
         completions = await self._client.Completion.acreate(headers=self._headers, **kwargs)
         return [choice.text for choice in completions.choices]
 
     async def chat_completion(self, messages: list[ChatMessage], temperature: float = 0,
-                              max_tokens: int = 16, model: Optional[str] = None, **kwargs) -> list[str]:
+                              max_tokens: int = 16, top_p: float = 1, model: Optional[str] = None, **kwargs) -> list[str]:
         self._set_model_in_kwargs(kwargs, model)
         kwargs["messages"] = [message.to_dict() for message in messages]
         kwargs["temperature"] = temperature
+        kwargs["top_p"] = top_p
         kwargs["max_tokens"] = max_tokens
         completions = await self._client.ChatCompletion.acreate(headers=self._headers, **kwargs)
         return [choice.message.content for choice in completions.choices]
 
     async def embedding(self, text: str, model: Optional[str] = None, **kwargs) -> list[float]:
         self._set_model_in_kwargs(kwargs, model)
         kwargs[INPUT_KEY] = text
```

### Comparing `llm_client-0.6.2/llm_client/llm_client/local_client.py` & `llm_client-0.7.0/llm_client/llm_client/local_client.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.6.2/llm_client/sync/sync_llm_api_client_factory.py` & `llm_client-0.7.0/llm_client/sync/sync_llm_api_client_factory.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.6.2/tests/llm_api_client/test_llm_api_client_factory.py` & `llm_client-0.7.0/tests/llm_api_client/test_llm_api_client_factory.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.6.2/tests/llm_api_client/ai21_client/conftest.py` & `llm_client-0.7.0/tests/llm_api_client/ai21_client/conftest.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.6.2/tests/llm_api_client/ai21_client/test_ai21.py` & `llm_client-0.7.0/tests/llm_api_client/ai21_client/test_ai21.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     actual = await llm_client.text_completion(prompt="These are a few of my favorite")
 
     assert actual == [
         ' things!\n\nI love entertaining, entertaining and decorating my home, entertaining clients, entertaining '
         'friends, entertaining family...you get the point! One of my favorite things to do is plan parties']
     mock_aioresponse.assert_called_once_with(url, method='POST',
                                              headers={AUTH_HEADER: BEARER_TOKEN + llm_client._api_key },
-                                             json={'prompt': 'These are a few of my favorite', "maxTokens" : 16, "temperature" : 0.7 },
+                                             json={'prompt': 'These are a few of my favorite', "maxTokens" : 16, "temperature" : 0.7, "topP" : 1 },
                                              raise_for_status=True)
 
 
 @pytest.mark.asyncio
 async def test_text_completion__return_multiple_completions(mock_aioresponse, llm_client, url):
     payload = load_json_resource("ai21/text_completion.json")
     payload["completions"].append({DATA_KEY: {TEXT_KEY: "second completion"}})
@@ -45,15 +45,15 @@
     assert actual == [
         ' things!\n\nI love entertaining, entertaining and decorating my home, entertaining clients, entertaining '
         'friends, entertaining family...you get the point! One of my favorite things to do is plan parties',
         "second completion"
     ]
     mock_aioresponse.assert_called_once_with(url, method='POST',
                                              headers={AUTH_HEADER: BEARER_TOKEN + llm_client._api_key},
-                                             json={'prompt': 'These are a few of my favorite', "maxTokens" : 16, "temperature" : 0.7 },
+                                             json={'prompt': 'These are a few of my favorite', "maxTokens" : 16, "temperature" : 0.7, "topP" : 1  },
                                              raise_for_status=True)
 
 
 @pytest.mark.asyncio
 async def test_text_completion__override_model(mock_aioresponse, llm_client):
     new_model_name = "gpt3"
     url = build_url(new_model_name)
@@ -65,15 +65,15 @@
     actual = await llm_client.text_completion(prompt="These are a few of my favorite", model=new_model_name)
 
     assert actual == [
         ' things!\n\nI love entertaining, entertaining and decorating my home, entertaining clients, entertaining '
         'friends, entertaining family...you get the point! One of my favorite things to do is plan parties']
     mock_aioresponse.assert_called_once_with(url, method='POST',
                                              headers={AUTH_HEADER: BEARER_TOKEN + llm_client._api_key},
-                                             json={'prompt': 'These are a few of my favorite', "maxTokens" : 16, "temperature" : 0.7 },
+                                             json={'prompt': 'These are a few of my favorite', "maxTokens" : 16, "temperature" : 0.7, "topP" : 1 },
                                              raise_for_status=True)
 
 
 @pytest.mark.asyncio
 async def test_text_completion__with_kwargs(mock_aioresponse, llm_client, url):
     mock_aioresponse.post(
         url,
@@ -83,15 +83,15 @@
     actual = await llm_client.text_completion(prompt="These are a few of my favorite", max_tokens=10)
 
     assert actual == [
         ' things!\n\nI love entertaining, entertaining and decorating my home, entertaining clients, entertaining '
         'friends, entertaining family...you get the point! One of my favorite things to do is plan parties']
     mock_aioresponse.assert_called_once_with(url, method='POST',
                                              headers={AUTH_HEADER: BEARER_TOKEN + llm_client._api_key},
-                                             json={'prompt': 'These are a few of my favorite', "maxTokens" : 10, "temperature" : 0.7 },
+                                             json={'prompt': 'These are a few of my favorite', "maxTokens" : 10, "temperature" : 0.7 ,"topP" : 1},
                                              raise_for_status=True)
 
 
 @pytest.mark.asyncio
 async def test_get_tokens_count__sanity(mock_aioresponse, llm_client, url):
     mock_aioresponse.post(
         BASE_URL + TOKENIZE_PATH,
```

### Comparing `llm_client-0.6.2/tests/llm_api_client/anthropic_client/conftest.py` & `llm_client-0.7.0/tests/llm_api_client/anthropic_client/conftest.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.6.2/tests/llm_api_client/anthropic_client/test_anthropic_client.py` & `llm_client-0.7.0/tests/llm_api_client/anthropic_client/test_anthropic_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,23 +10,22 @@
 async def test_get_llm_api_client__with_anthropic(config):
     del config.session
     async with LLMAPIClientFactory() as llm_api_client_factory:
         actual = llm_api_client_factory.get_llm_api_client(LLMAPIClientType.ANTHROPIC, **config.__dict__)
 
     assert isinstance(actual, AnthropicClient)
 
-
 @pytest.mark.asyncio
 async def test_text_completion__sanity(mock_aioresponse, llm_client, complete_url, anthropic_version):
     mock_aioresponse.post(
         complete_url,
         payload={COMPLETIONS_KEY: "completion text"}
     )
 
-    actual = await llm_client.text_completion(prompt="These are a few of my favorite", max_tokens=10)
+    actual = await llm_client.text_completion(prompt="These are a few of my favorite", max_tokens=10,)
 
     assert actual == ["completion text"]
     mock_aioresponse.assert_called_once_with(complete_url, method='POST',
                                              headers={AUTH_HEADER: llm_client._api_key,
                                                       ACCEPT_HEADER: ACCEPT_VALUE,
                                                       VERSION_HEADER: anthropic_version},
                                              json={PROMPT_KEY: 'These are a few of my favorite',
@@ -88,25 +87,25 @@
 @pytest.mark.asyncio
 async def test_text_completion__with_kwargs(mock_aioresponse, llm_client, complete_url, anthropic_version):
     mock_aioresponse.post(
         complete_url,
         payload={COMPLETIONS_KEY: "completion text"}
     )
 
-    actual = await llm_client.text_completion(prompt="These are a few of my favorite", max_tokens=10, temperature=0.5)
+    actual = await llm_client.text_completion(prompt="These are a few of my favorite", max_tokens=10, temperature=0.5,top_p=0.5)
 
     assert actual == ["completion text"]
     mock_aioresponse.assert_called_once_with(complete_url, method='POST',
                                              headers={AUTH_HEADER: llm_client._api_key,
                                                       ACCEPT_HEADER: ACCEPT_VALUE,
                                                       VERSION_HEADER: anthropic_version},
                                              json={PROMPT_KEY: 'These are a few of my favorite',
                                                    MAX_TOKENS_KEY: 10,
                                                    MODEL_KEY: llm_client._default_model,
-                                                   "temperature": 0.5},
+                                                   "temperature": 0.5, "top_p" : 0.5},
                                              raise_for_status=True)
 
 
 @pytest.mark.asyncio
 async def test_get_tokens_count__sanity(llm_client, number_of_tokens, mock_anthropic):
     actual = await llm_client.get_tokens_count(text="These are a few of my favorite things!")
```

### Comparing `llm_client-0.6.2/tests/llm_api_client/google_client/conftest.py` & `llm_client-0.7.0/tests/llm_api_client/google_client/conftest.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.6.2/tests/llm_api_client/google_client/test_google_client.py` & `llm_client-0.7.0/tests/llm_api_client/google_client/test_google_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,23 +64,23 @@
 async def test_text_completion__with_kwargs(mock_aioresponse, llm_client, params):
     url = build_url(llm_client, COMPLETE_PATH)
     mock_aioresponse.post(
         url + params,
         payload=load_json_resource("google/text_completion.json")
     )
 
-    actual = await llm_client.text_completion(prompt="These are a few of my favorite", max_tokens=10, blabla="aaa")
+    actual = await llm_client.text_completion(prompt="These are a few of my favorite", max_tokens=10, blabla="aaa", top_p= 0.95)
 
     assert actual == ['Once upon a time, there was a young girl named Lily...',
                       'Once upon a time, there was a young boy named Billy...']
     mock_aioresponse.assert_called_once_with(url, method='POST', params={AUTH_PARAM: llm_client._api_key},
                                              json={PROMPT_KEY: {TEXT_KEY: 'These are a few of my favorite'},
                                                    MAX_TOKENS_KEY: 10,
                                                    'temperature': None,
-                                                   'blabla': 'aaa'},
+                                                   'blabla': 'aaa',"topP" : 0.95},
                                              headers=llm_client._headers,
                                              raise_for_status=True,
                                              )
 
 
 @pytest.mark.asyncio
 async def test_embedding__sanity(mock_aioresponse, llm_client, params):
```

### Comparing `llm_client-0.6.2/tests/llm_api_client/huggingface_client/conftest.py` & `llm_client-0.7.0/tests/llm_api_client/huggingface_client/conftest.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.6.2/tests/llm_api_client/huggingface_client/test_huggingface.py` & `llm_client-0.7.0/tests/llm_api_client/huggingface_client/test_huggingface.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     )
 
     actual = await llm_client.text_completion(prompt="who is kobe bryant")
 
     assert actual == ['Kobe Bryant is a retired professional basketball player who played for the Los Angeles Lakers of']
     mock_aioresponse.assert_called_once_with(url, method='POST',
                                              headers={AUTH_HEADER: BEARER_TOKEN + llm_client._api_key},
-                                             json={'inputs': 'who is kobe bryant',"max_length": None, "temperature": 1.0},
+                                             json={'inputs': 'who is kobe bryant',"max_length": None, "temperature": 1.0, "top_p" : None},
                                              raise_for_status=True)
 
 
 @pytest.mark.asyncio
 async def test_text_completion__with_kwargs(mock_aioresponse, llm_client, url):
     mock_aioresponse.post(
         url,
@@ -40,15 +40,15 @@
     )
 
     actual = await llm_client.text_completion(prompt="who is kobe bryant",max_tokens = 10)
 
     assert actual == ['Kobe Bryant is a retired professional basketball player who played for the Los Angeles Lakers of']
     mock_aioresponse.assert_called_once_with(url, method='POST',
                                              headers={AUTH_HEADER: BEARER_TOKEN + llm_client._api_key},
-                                             json={'inputs': 'who is kobe bryant',"max_length": 10, "temperature": 1.0},
+                                             json={'inputs': 'who is kobe bryant',"max_length": 10, "temperature": 1.0, "top_p" : None},
                                              raise_for_status=True)
 
 
 @pytest.mark.asyncio
 def test_get_tokens_count__sanity(mock_aioresponse, llm_client, url):
     actual = llm_client.get_tokens_count(text="is queen elisabeth alive?")
     assert actual == 7
```

### Comparing `llm_client-0.6.2/tests/llm_api_client/openai_client/conftest.py` & `llm_client-0.7.0/tests/llm_api_client/openai_client/conftest.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.6.2/tests/llm_api_client/openai_client/test_openai.py` & `llm_client-0.7.0/tests/llm_api_client/openai_client/test_openai.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,59 +33,59 @@
         return_value=OpenAIObject.construct_from(load_json_resource("openai/text_completion.json")))
     actual = await open_ai_client.text_completion(prompt="These are a few of my favorite")
 
     assert actual == ["\n\nThis is indeed a test"]
     openai_mock.Completion.acreate.assert_awaited_once_with(
         model=model_name,
         prompt="These are a few of my favorite",
-        headers={},temperature=0,max_tokens=16)
+        headers={},temperature=0,max_tokens=16,top_p=1)
 
 
 @pytest.mark.asyncio
 async def test_text_completion__return_multiple_completions(openai_mock, open_ai_client, model_name):
     open_ai_object = OpenAIObject.construct_from(load_json_resource("openai/text_completion.json"))
     open_ai_object.choices.append(OpenAIObject.construct_from({"text": "second completion"}))
     openai_mock.Completion.acreate = AsyncMock(return_value=open_ai_object)
 
     actual = await open_ai_client.text_completion(prompt="These are a few of my favorite")
 
     assert actual == ["\n\nThis is indeed a test", "second completion"]
     openai_mock.Completion.acreate.assert_awaited_once_with(
         model=model_name,
         prompt="These are a few of my favorite",
-        headers={},temperature=0,max_tokens=16)
+        headers={},temperature=0,max_tokens=16,top_p=1)
 
 
 @pytest.mark.asyncio
 async def test_text_completion__override_model(openai_mock, open_ai_client, model_name):
     new_model_name = "gpt3"
     openai_mock.Completion.acreate = AsyncMock(
         return_value=OpenAIObject.construct_from(load_json_resource("openai/text_completion.json")))
 
     actual = await open_ai_client.text_completion(prompt="These are a few of my favorite", model=new_model_name)
 
     assert actual == ["\n\nThis is indeed a test"]
     openai_mock.Completion.acreate.assert_awaited_once_with(
         model=new_model_name,
         prompt="These are a few of my favorite",
-        headers={},temperature=0,max_tokens=16)
+        headers={},temperature=0,max_tokens=16,top_p=1)
 
 
 @pytest.mark.asyncio
 async def test_text_completion__with_kwargs(openai_mock, open_ai_client, model_name):
     openai_mock.Completion.acreate = AsyncMock(
         return_value=OpenAIObject.construct_from(load_json_resource("openai/text_completion.json")))
 
     actual = await open_ai_client.text_completion(prompt="These are a few of my favorite", max_tokens=10)
 
     assert actual == ["\n\nThis is indeed a test"]
     openai_mock.Completion.acreate.assert_awaited_once_with(
         model=model_name,
         prompt="These are a few of my favorite",
-        temperature=0,max_tokens=10,
+        temperature=0,max_tokens=10,top_p=1,
         headers={})
 
 
 @pytest.mark.asyncio
 async def test_text_completion__with_headers(openai_mock, model_name):
     openai_mock.Completion.acreate = AsyncMock(
         return_value=OpenAIObject.construct_from(load_json_resource("openai/text_completion.json")))
@@ -94,74 +94,74 @@
 
     actual = await open_ai_client.text_completion(prompt="These are a few of my favorite")
 
     assert actual == ["\n\nThis is indeed a test"]
     openai_mock.Completion.acreate.assert_awaited_once_with(
         model=model_name,
         prompt="These are a few of my favorite",
-        headers={"header_name": "header_value"},temperature=0,max_tokens=16)
+        headers={"header_name": "header_value"},temperature=0,max_tokens=16,top_p=1)
 
 
 @pytest.mark.asyncio
 async def test_chat_completion__sanity(openai_mock, open_ai_client, model_name):
     openai_mock.ChatCompletion.acreate = AsyncMock(
         return_value=OpenAIObject.construct_from(load_json_resource("openai/chat_completion.json")))
 
     actual = await open_ai_client.chat_completion([ChatMessage(Role.USER, "Hello!")])
 
     assert actual == ["\n\nHello there, how may I assist you today?"]
     openai_mock.ChatCompletion.acreate.assert_awaited_once_with(
         model=model_name,
         messages=[{'content': 'Hello!', 'role': 'user'}],
-        headers={},temperature=0,max_tokens=16)
+        headers={},temperature=0,max_tokens=16,top_p=1)
 
 
 @pytest.mark.asyncio
 async def test_chat_completion__return_multiple_completions(openai_mock, open_ai_client, model_name):
     open_ai_object = OpenAIObject.construct_from(load_json_resource("openai/chat_completion.json"))
     open_ai_object.choices.append(OpenAIObject.construct_from({"message": {"content": "second completion"}}))
     openai_mock.ChatCompletion.acreate = AsyncMock(return_value=open_ai_object)
 
     actual = await open_ai_client.chat_completion([ChatMessage(Role.USER, "Hello!")])
 
     assert actual == ["\n\nHello there, how may I assist you today?", "second completion"]
     openai_mock.ChatCompletion.acreate.assert_awaited_once_with(
         model=model_name,
         messages=[{'content': 'Hello!', 'role': 'user'}],
-        headers={},temperature=0,max_tokens=16)
+        headers={},temperature=0,max_tokens=16,top_p=1)
 
 
 @pytest.mark.asyncio
 async def test_chat_completion__override_model(openai_mock, open_ai_client, model_name):
     new_model_name = "gpt3"
     openai_mock.ChatCompletion.acreate = AsyncMock(
         return_value=OpenAIObject.construct_from(load_json_resource("openai/chat_completion.json")))
 
     actual = await open_ai_client.chat_completion([ChatMessage(Role.USER, "Hello!")], model=new_model_name)
 
     assert actual == ["\n\nHello there, how may I assist you today?"]
     openai_mock.ChatCompletion.acreate.assert_awaited_once_with(
         model=new_model_name,
         messages=[{'content': 'Hello!', 'role': 'user'}],
-        headers={},temperature=0,max_tokens=16)
+        headers={},temperature=0,max_tokens=16,top_p=1)
 
 
 @pytest.mark.asyncio
 async def test_chat_completion__with_kwargs(openai_mock, open_ai_client, model_name):
     openai_mock.ChatCompletion.acreate = AsyncMock(
         return_value=OpenAIObject.construct_from(load_json_resource("openai/chat_completion.json")))
 
-    actual = await open_ai_client.chat_completion([ChatMessage(Role.USER, "Hello!")], max_tokens=10)
+    actual = await open_ai_client.chat_completion([ChatMessage(Role.USER, "Hello!")], max_tokens=10,top_p=1)
 
     assert actual == ["\n\nHello there, how may I assist you today?"]
     openai_mock.ChatCompletion.acreate.assert_awaited_once_with(
         model=model_name,
         messages=[{'content': 'Hello!', 'role': 'user'}],
         max_tokens=10,
-        headers={},temperature=0)
+        headers={},temperature=0,top_p=1)
 
 
 @pytest.mark.asyncio
 async def test_chat_completion__with_headers(openai_mock, model_name):
     openai_mock.ChatCompletion.acreate = AsyncMock(
         return_value=OpenAIObject.construct_from(load_json_resource("openai/chat_completion.json")))
     open_ai_client = OpenAIClient(LLMAPIClientConfig("fake_api_key", MagicMock(ClientSession), default_model=model_name,
@@ -169,15 +169,15 @@
 
     actual = await open_ai_client.chat_completion([ChatMessage(Role.USER, "Hello!")])
 
     assert actual == ["\n\nHello there, how may I assist you today?"]
     openai_mock.ChatCompletion.acreate.assert_awaited_once_with(
         model=model_name,
         messages=[{'content': 'Hello!', 'role': 'user'}],
-        headers={"header_name": "header_value"},temperature=0,max_tokens=16)
+        headers={"header_name": "header_value"},temperature=0,max_tokens=16,top_p=1)
 
 
 @pytest.mark.asyncio
 async def test_get_tokens_count__sanity(model_name, open_ai_client, tiktoken_mock):
     tokeniser_mock = tiktoken_mock.encoding_for_model.return_value
     tokeniser_mock.encode.return_value = [123, 456]
     text = "This is a test"
```

### Comparing `llm_client-0.6.2/tests/llm_client/local_client/conftest.py` & `llm_client-0.7.0/tests/llm_client/local_client/conftest.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.6.2/tests/llm_client/local_client/test_local_client.py` & `llm_client-0.7.0/tests/llm_client/local_client/test_local_client.py`

 * *Files identical despite different names*

### Comparing `llm_client-0.6.2/tests/resources/ai21/text_completion.json` & `llm_client-0.7.0/tests/resources/ai21/text_completion.json`

 * *Files identical despite different names*

### Comparing `llm_client-0.6.2/.gitignore` & `llm_client-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `llm_client-0.6.2/LICENSE` & `llm_client-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_client-0.6.2/README.md` & `llm_client-0.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,15 @@
 Our vision is to provide async native and production ready SDK while creating 
 a powerful and fast integration with different LLM without letting the user lose 
 any flexibility (API params, endpoints etc.). *We also provide sync version, see
 more details below in Usage section.
 
 ## Base Interface
 The package exposes two simple interfaces for communicating with LLMs (In the future, we 
-will expand the interface to support more tasks like embeddings, list models, edits, etc.
-and we will add a standardized for LLMs param like max_tokens, temperature, etc.):
+will expand the interface to support more tasks like list models, edits, etc.):
 ```python
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
 from typing import Any, Optional
 from aiohttp import ClientSession
 
 
@@ -43,15 +42,15 @@
 
 class BaseLLMAPIClient(BaseLLMClient, ABC):
     def __init__(self, config: LLMAPIClientConfig):
         ...
 
     @abstractmethod
     async def text_completion(self, prompt: str, model: Optional[str] = None, max_tokens: int | None = None,
-                              temperature: Optional[float] = None, **kwargs) -> list[str]:
+                              temperature: Optional[float] = None, top_p: Optional[float] = None, **kwargs) -> list[str]:
         raise NotImplementedError()
 
     async def embedding(self, text: str, model: Optional[str] = None, **kwargs) -> list[float]:
         raise NotImplementedError()
 ```
 
 ## Requirements
@@ -196,14 +195,15 @@
   - [ ] edits
   - [ ] more
 - [ ] Add contributing guidelines and linter
 - [ ] Create an easy way to run multiple LLMs in parallel with the same prompts
 - [x] Convert common models parameter
   - [x] temperature 
   - [x] max_tokens
+  - [x] top_p
   - [ ] more
 
 ### Development
 To install the package in development mode, run the following command:
 ```console
 $ pip install -e ".[all,test]"
 ```
```

### Comparing `llm_client-0.6.2/pyproject.toml` & `llm_client-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `llm_client-0.6.2/PKG-INFO` & `llm_client-0.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-client
-Version: 0.6.2
+Version: 0.7.0
 Summary: SDK for using LLM
 Project-URL: Homepage, https://github.com/uripeled2/llm-client-sdk
 Author-email: Uri Peled <uripeled2@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -52,16 +52,15 @@
 Our vision is to provide async native and production ready SDK while creating 
 a powerful and fast integration with different LLM without letting the user lose 
 any flexibility (API params, endpoints etc.). *We also provide sync version, see
 more details below in Usage section.
 
 ## Base Interface
 The package exposes two simple interfaces for communicating with LLMs (In the future, we 
-will expand the interface to support more tasks like embeddings, list models, edits, etc.
-and we will add a standardized for LLMs param like max_tokens, temperature, etc.):
+will expand the interface to support more tasks like list models, edits, etc.):
 ```python
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
 from typing import Any, Optional
 from aiohttp import ClientSession
 
 
@@ -86,15 +85,15 @@
 
 class BaseLLMAPIClient(BaseLLMClient, ABC):
     def __init__(self, config: LLMAPIClientConfig):
         ...
 
     @abstractmethod
     async def text_completion(self, prompt: str, model: Optional[str] = None, max_tokens: int | None = None,
-                              temperature: Optional[float] = None, **kwargs) -> list[str]:
+                              temperature: Optional[float] = None, top_p: Optional[float] = None, **kwargs) -> list[str]:
         raise NotImplementedError()
 
     async def embedding(self, text: str, model: Optional[str] = None, **kwargs) -> list[float]:
         raise NotImplementedError()
 ```
 
 ## Requirements
@@ -239,14 +238,15 @@
   - [ ] edits
   - [ ] more
 - [ ] Add contributing guidelines and linter
 - [ ] Create an easy way to run multiple LLMs in parallel with the same prompts
 - [x] Convert common models parameter
   - [x] temperature 
   - [x] max_tokens
+  - [x] top_p
   - [ ] more
 
 ### Development
 To install the package in development mode, run the following command:
 ```console
 $ pip install -e ".[all,test]"
 ```
```

