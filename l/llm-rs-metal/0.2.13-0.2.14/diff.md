# Comparing `tmp/llm_rs_metal-0.2.13.tar.gz` & `tmp/llm_rs_metal-0.2.14.tar.gz`

## Comparing `llm_rs_metal-0.2.13.tar` & `llm_rs_metal-0.2.14.tar`

### file list

```diff
@@ -1,54 +1,55 @@
--rw-r--r--   0        0        0      811 1970-01-01 00:00:00.000000 llm_rs_metal-0.2.13/Cargo.toml
--rw-r--r--   0     1001      123      610 2023-07-17 15:33:34.000000 llm_rs_metal-0.2.13/.github/workflows/BuildDoc.yml
--rw-r--r--   0     1001      123     3796 2023-07-17 15:33:34.000000 llm_rs_metal-0.2.13/.github/workflows/CI-CuBLAS.yml
--rw-r--r--   0     1001      123     2136 2023-07-17 15:33:34.000000 llm_rs_metal-0.2.13/.github/workflows/CI-Metal.yml
--rw-r--r--   0     1001      123     4173 2023-07-17 15:33:34.000000 llm_rs_metal-0.2.13/.github/workflows/CI-OpenCL.yml
--rw-r--r--   0     1001      123     6258 2023-07-17 15:33:34.000000 llm_rs_metal-0.2.13/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      564 2023-07-17 15:33:34.000000 llm_rs_metal-0.2.13/.github/workflows/Clippy.yml
--rw-r--r--   0     1001      123      602 2023-07-17 15:33:34.000000 llm_rs_metal-0.2.13/.github/workflows/PublishDocs.yml
--rw-r--r--   0     1001      123     3477 2023-07-17 15:33:34.000000 llm_rs_metal-0.2.13/.gitignore
--rw-r--r--   0     1001      123       72 2023-07-17 15:33:34.000000 llm_rs_metal-0.2.13/.vscode/settings.json
--rw-r--r--   0     1001      123     1071 2023-07-17 15:33:34.000000 llm_rs_metal-0.2.13/LICENSE
--rw-r--r--   0     1001      123     7034 2023-07-17 15:33:34.000000 llm_rs_metal-0.2.13/README.md
--rw-r--r--   0     1001      123      702 2023-07-17 15:33:34.000000 llm_rs_metal-0.2.13/build_scripts/pyproject_patcher.py
--rw-r--r--   0     1001      123     1016 2023-07-17 15:33:34.000000 llm_rs_metal-0.2.13/build_scripts/repair_windows_wheels.py
--rw-r--r--   0     1001      123       16 2023-07-17 15:33:34.000000 llm_rs_metal-0.2.13/build_scripts/requirements.txt
--rw-r--r--   0     1001      123     4799 2023-07-17 15:33:34.000000 llm_rs_metal-0.2.13/docs/docs/conversion.md
--rw-r--r--   0     1001      123     9355 2023-07-17 15:33:34.000000 llm_rs_metal-0.2.13/docs/docs/index.md
--rw-r--r--   0     1001      123     1181 2023-07-17 15:33:34.000000 llm_rs_metal-0.2.13/docs/mkdocs.yml
--rw-r--r--   0     1001      123       31 2023-07-17 15:33:34.000000 llm_rs_metal-0.2.13/docs/requirements.txt
--rw-r--r--   0     1001      123      424 2023-07-17 15:33:34.000000 llm_rs_metal-0.2.13/examples/haystack_example.py
--rw-r--r--   0     1001      123      764 2023-07-17 15:33:34.000000 llm_rs_metal-0.2.13/examples/langchain_example.py
--rw-r--r--   0     1001      123     1121 2023-07-17 15:33:34.000000 llm_rs_metal-0.2.13/llm_rs/__init__.py
--rw-r--r--   0     1001      123    17102 2023-07-17 15:33:34.000000 llm_rs_metal-0.2.13/llm_rs/auto.py
--rw-r--r--   0     1001      123     2129 2023-07-17 15:33:34.000000 llm_rs_metal-0.2.13/llm_rs/base_model.py
--rw-r--r--   0     1001      123     1728 2023-07-17 15:33:34.000000 llm_rs_metal-0.2.13/llm_rs/config.pyi
--rw-r--r--   0     1001      123       78 2023-07-17 15:33:34.000000 llm_rs_metal-0.2.13/llm_rs/convert/__init__.py
--rw-r--r--   0     1001      123     2305 2023-07-17 15:33:34.000000 llm_rs_metal-0.2.13/llm_rs/convert/auto_converter.py
--rw-r--r--   0     1001      123      199 2023-07-17 15:33:34.000000 llm_rs_metal-0.2.13/llm_rs/convert/models/__init__.py
--rw-r--r--   0     1001      123     5820 2023-07-17 15:33:34.000000 llm_rs_metal-0.2.13/llm_rs/convert/models/_base.py
--rw-r--r--   0     1001      123     3177 2023-07-17 15:33:34.000000 llm_rs_metal-0.2.13/llm_rs/convert/models/bloom.py
--rw-r--r--   0     1001      123     5221 2023-07-17 15:33:34.000000 llm_rs_metal-0.2.13/llm_rs/convert/models/gpt2.py
--rw-r--r--   0     1001      123     2032 2023-07-17 15:33:34.000000 llm_rs_metal-0.2.13/llm_rs/convert/models/gptj.py
--rw-r--r--   0     1001      123     2138 2023-07-17 15:33:34.000000 llm_rs_metal-0.2.13/llm_rs/convert/models/gptneox.py
--rw-r--r--   0     1001      123     6334 2023-07-17 15:33:34.000000 llm_rs_metal-0.2.13/llm_rs/convert/models/llama.py
--rw-r--r--   0     1001      123     1893 2023-07-17 15:33:34.000000 llm_rs_metal-0.2.13/llm_rs/convert/models/mpt.py
--rw-r--r--   0     1001      123       48 2023-07-17 15:33:34.000000 llm_rs_metal-0.2.13/llm_rs/haystack/__init__.py
--rw-r--r--   0     1001      123     4878 2023-07-17 15:33:34.000000 llm_rs_metal-0.2.13/llm_rs/haystack/haystack.py
--rw-r--r--   0     1001      123       37 2023-07-17 15:33:34.000000 llm_rs_metal-0.2.13/llm_rs/langchain/__init__.py
--rw-r--r--   0     1001      123     4268 2023-07-17 15:33:34.000000 llm_rs_metal-0.2.13/llm_rs/langchain/langchain.py
--rw-r--r--   0     1001      123      170 2023-07-17 15:33:34.000000 llm_rs_metal-0.2.13/llm_rs/llm_rs.pyi
--rw-r--r--   0     1001      123      579 2023-07-17 15:33:34.000000 llm_rs_metal-0.2.13/llm_rs/models.pyi
--rw-r--r--   0     1001      123        0 2023-07-17 15:33:34.000000 llm_rs_metal-0.2.13/llm_rs/py.typed
--rw-r--r--   0     1001      123     2915 2023-07-17 15:33:34.000000 llm_rs_metal-0.2.13/llm_rs/repository.py
--rw-r--r--   0     1001      123      697 2023-07-17 15:33:34.000000 llm_rs_metal-0.2.13/llm_rs/results.pyi
--rw-r--r--   0     1001      123     1030 2023-07-17 15:33:38.000000 llm_rs_metal-0.2.13/pyproject.toml
--rw-r--r--   0     1001      123     7824 2023-07-17 15:33:34.000000 llm_rs_metal-0.2.13/src/configs.rs
--rw-r--r--   0     1001      123     2164 2023-07-17 15:33:34.000000 llm_rs_metal-0.2.13/src/lib.rs
--rw-r--r--   0     1001      123    17704 2023-07-17 15:33:34.000000 llm_rs_metal-0.2.13/src/model_base.rs
--rw-r--r--   0     1001      123      300 2023-07-17 15:33:34.000000 llm_rs_metal-0.2.13/src/models.rs
--rw-r--r--   0     1001      123     3192 2023-07-17 15:33:34.000000 llm_rs_metal-0.2.13/src/quantize.rs
--rw-r--r--   0     1001      123     1352 2023-07-17 15:33:34.000000 llm_rs_metal-0.2.13/src/results.rs
--rw-r--r--   0     1001      123     1820 2023-07-17 15:33:34.000000 llm_rs_metal-0.2.13/src/stopwords.rs
--rw-r--r--   0     1001      123    59466 2023-07-17 15:33:45.000000 llm_rs_metal-0.2.13/Cargo.lock
--rw-r--r--   0        0        0     8303 1970-01-01 00:00:00.000000 llm_rs_metal-0.2.13/PKG-INFO
+-rw-r--r--   0        0        0      811 1970-01-01 00:00:00.000000 llm_rs_metal-0.2.14/Cargo.toml
+-rw-r--r--   0     1001      123      610 2023-07-19 15:30:56.000000 llm_rs_metal-0.2.14/.github/workflows/BuildDoc.yml
+-rw-r--r--   0     1001      123     3876 2023-07-19 15:30:56.000000 llm_rs_metal-0.2.14/.github/workflows/CI-CuBLAS.yml
+-rw-r--r--   0     1001      123     2136 2023-07-19 15:30:56.000000 llm_rs_metal-0.2.14/.github/workflows/CI-Metal.yml
+-rw-r--r--   0     1001      123     4173 2023-07-19 15:30:56.000000 llm_rs_metal-0.2.14/.github/workflows/CI-OpenCL.yml
+-rw-r--r--   0     1001      123     6258 2023-07-19 15:30:56.000000 llm_rs_metal-0.2.14/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      564 2023-07-19 15:30:56.000000 llm_rs_metal-0.2.14/.github/workflows/Clippy.yml
+-rw-r--r--   0     1001      123      602 2023-07-19 15:30:56.000000 llm_rs_metal-0.2.14/.github/workflows/PublishDocs.yml
+-rw-r--r--   0     1001      123     3477 2023-07-19 15:30:56.000000 llm_rs_metal-0.2.14/.gitignore
+-rw-r--r--   0     1001      123      496 2023-07-19 15:30:56.000000 llm_rs_metal-0.2.14/.vscode/launch.json
+-rw-r--r--   0     1001      123       72 2023-07-19 15:30:56.000000 llm_rs_metal-0.2.14/.vscode/settings.json
+-rw-r--r--   0     1001      123     1071 2023-07-19 15:30:56.000000 llm_rs_metal-0.2.14/LICENSE
+-rw-r--r--   0     1001      123     7034 2023-07-19 15:30:56.000000 llm_rs_metal-0.2.14/README.md
+-rw-r--r--   0     1001      123      702 2023-07-19 15:30:56.000000 llm_rs_metal-0.2.14/build_scripts/pyproject_patcher.py
+-rw-r--r--   0     1001      123     1016 2023-07-19 15:30:56.000000 llm_rs_metal-0.2.14/build_scripts/repair_windows_wheels.py
+-rw-r--r--   0     1001      123       16 2023-07-19 15:30:56.000000 llm_rs_metal-0.2.14/build_scripts/requirements.txt
+-rw-r--r--   0     1001      123     4799 2023-07-19 15:30:56.000000 llm_rs_metal-0.2.14/docs/docs/conversion.md
+-rw-r--r--   0     1001      123     9355 2023-07-19 15:30:56.000000 llm_rs_metal-0.2.14/docs/docs/index.md
+-rw-r--r--   0     1001      123     1181 2023-07-19 15:30:56.000000 llm_rs_metal-0.2.14/docs/mkdocs.yml
+-rw-r--r--   0     1001      123       31 2023-07-19 15:30:56.000000 llm_rs_metal-0.2.14/docs/requirements.txt
+-rw-r--r--   0     1001      123      840 2023-07-19 15:30:56.000000 llm_rs_metal-0.2.14/examples/haystack_example.py
+-rw-r--r--   0     1001      123     1095 2023-07-19 15:30:56.000000 llm_rs_metal-0.2.14/examples/langchain_example.py
+-rw-r--r--   0     1001      123     1121 2023-07-19 15:30:56.000000 llm_rs_metal-0.2.14/llm_rs/__init__.py
+-rw-r--r--   0     1001      123    18469 2023-07-19 15:30:56.000000 llm_rs_metal-0.2.14/llm_rs/auto.py
+-rw-r--r--   0     1001      123     2129 2023-07-19 15:30:56.000000 llm_rs_metal-0.2.14/llm_rs/base_model.py
+-rw-r--r--   0     1001      123     1728 2023-07-19 15:30:56.000000 llm_rs_metal-0.2.14/llm_rs/config.pyi
+-rw-r--r--   0     1001      123       78 2023-07-19 15:30:56.000000 llm_rs_metal-0.2.14/llm_rs/convert/__init__.py
+-rw-r--r--   0     1001      123     2305 2023-07-19 15:30:56.000000 llm_rs_metal-0.2.14/llm_rs/convert/auto_converter.py
+-rw-r--r--   0     1001      123      199 2023-07-19 15:30:56.000000 llm_rs_metal-0.2.14/llm_rs/convert/models/__init__.py
+-rw-r--r--   0     1001      123     5820 2023-07-19 15:30:56.000000 llm_rs_metal-0.2.14/llm_rs/convert/models/_base.py
+-rw-r--r--   0     1001      123     3177 2023-07-19 15:30:56.000000 llm_rs_metal-0.2.14/llm_rs/convert/models/bloom.py
+-rw-r--r--   0     1001      123     5221 2023-07-19 15:30:56.000000 llm_rs_metal-0.2.14/llm_rs/convert/models/gpt2.py
+-rw-r--r--   0     1001      123     2032 2023-07-19 15:30:56.000000 llm_rs_metal-0.2.14/llm_rs/convert/models/gptj.py
+-rw-r--r--   0     1001      123     2138 2023-07-19 15:30:56.000000 llm_rs_metal-0.2.14/llm_rs/convert/models/gptneox.py
+-rw-r--r--   0     1001      123     6334 2023-07-19 15:30:56.000000 llm_rs_metal-0.2.14/llm_rs/convert/models/llama.py
+-rw-r--r--   0     1001      123     1893 2023-07-19 15:30:56.000000 llm_rs_metal-0.2.14/llm_rs/convert/models/mpt.py
+-rw-r--r--   0     1001      123       48 2023-07-19 15:30:56.000000 llm_rs_metal-0.2.14/llm_rs/haystack/__init__.py
+-rw-r--r--   0     1001      123     4883 2023-07-19 15:30:56.000000 llm_rs_metal-0.2.14/llm_rs/haystack/haystack.py
+-rw-r--r--   0     1001      123       37 2023-07-19 15:30:56.000000 llm_rs_metal-0.2.14/llm_rs/langchain/__init__.py
+-rw-r--r--   0     1001      123     4268 2023-07-19 15:30:56.000000 llm_rs_metal-0.2.14/llm_rs/langchain/langchain.py
+-rw-r--r--   0     1001      123      170 2023-07-19 15:30:56.000000 llm_rs_metal-0.2.14/llm_rs/llm_rs.pyi
+-rw-r--r--   0     1001      123      579 2023-07-19 15:30:56.000000 llm_rs_metal-0.2.14/llm_rs/models.pyi
+-rw-r--r--   0     1001      123        0 2023-07-19 15:30:56.000000 llm_rs_metal-0.2.14/llm_rs/py.typed
+-rw-r--r--   0     1001      123     2915 2023-07-19 15:30:56.000000 llm_rs_metal-0.2.14/llm_rs/repository.py
+-rw-r--r--   0     1001      123      697 2023-07-19 15:30:56.000000 llm_rs_metal-0.2.14/llm_rs/results.pyi
+-rw-r--r--   0     1001      123     1030 2023-07-19 15:30:58.000000 llm_rs_metal-0.2.14/pyproject.toml
+-rw-r--r--   0     1001      123     7824 2023-07-19 15:30:56.000000 llm_rs_metal-0.2.14/src/configs.rs
+-rw-r--r--   0     1001      123     2164 2023-07-19 15:30:56.000000 llm_rs_metal-0.2.14/src/lib.rs
+-rw-r--r--   0     1001      123    17704 2023-07-19 15:30:56.000000 llm_rs_metal-0.2.14/src/model_base.rs
+-rw-r--r--   0     1001      123      300 2023-07-19 15:30:56.000000 llm_rs_metal-0.2.14/src/models.rs
+-rw-r--r--   0     1001      123     3192 2023-07-19 15:30:56.000000 llm_rs_metal-0.2.14/src/quantize.rs
+-rw-r--r--   0     1001      123     1352 2023-07-19 15:30:56.000000 llm_rs_metal-0.2.14/src/results.rs
+-rw-r--r--   0     1001      123     1820 2023-07-19 15:30:56.000000 llm_rs_metal-0.2.14/src/stopwords.rs
+-rw-r--r--   0     1001      123    59467 2023-07-19 15:31:06.000000 llm_rs_metal-0.2.14/Cargo.lock
+-rw-r--r--   0        0        0     8303 1970-01-01 00:00:00.000000 llm_rs_metal-0.2.14/PKG-INFO
```

### Comparing `llm_rs_metal-0.2.13/Cargo.toml` & `llm_rs_metal-0.2.14/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "llm-rs"
-version = "0.2.13"
+version = "0.2.14"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "llm_rs"
 crate-type = ["cdylib"]
```

### Comparing `llm_rs_metal-0.2.13/.github/workflows/BuildDoc.yml` & `llm_rs_metal-0.2.14/.github/workflows/BuildDoc.yml`

 * *Files identical despite different names*

### Comparing `llm_rs_metal-0.2.13/.github/workflows/CI-CuBLAS.yml` & `llm_rs_metal-0.2.14/.github/workflows/CI-CuBLAS.yml`

 * *Files 2% similar despite different names*

```diff
@@ -130,13 +130,16 @@
     runs-on: ubuntu-latest
     if: "startsWith(github.ref, 'refs/tags/')"
     needs: [linux, windows]
     steps:
       - uses: actions/download-artifact@v3
         with:
           name: wheels
+          path: wheels
+      - name: List wheel files
+        run: ls -l wheels
       - name: Upload wheels
         uses: softprops/action-gh-release@v1
         with:
           files: |
             wheels/*.whl
```

### Comparing `llm_rs_metal-0.2.13/.github/workflows/CI-Metal.yml` & `llm_rs_metal-0.2.14/.github/workflows/CI-Metal.yml`

 * *Files identical despite different names*

### Comparing `llm_rs_metal-0.2.13/.github/workflows/CI-OpenCL.yml` & `llm_rs_metal-0.2.14/.github/workflows/CI-OpenCL.yml`

 * *Files identical despite different names*

### Comparing `llm_rs_metal-0.2.13/.github/workflows/CI.yml` & `llm_rs_metal-0.2.14/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `llm_rs_metal-0.2.13/.github/workflows/Clippy.yml` & `llm_rs_metal-0.2.14/.github/workflows/Clippy.yml`

 * *Files identical despite different names*

### Comparing `llm_rs_metal-0.2.13/.github/workflows/PublishDocs.yml` & `llm_rs_metal-0.2.14/.github/workflows/PublishDocs.yml`

 * *Files identical despite different names*

### Comparing `llm_rs_metal-0.2.13/.gitignore` & `llm_rs_metal-0.2.14/.gitignore`

 * *Files identical despite different names*

### Comparing `llm_rs_metal-0.2.13/LICENSE` & `llm_rs_metal-0.2.14/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_rs_metal-0.2.13/README.md` & `llm_rs_metal-0.2.14/README.md`

 * *Files identical despite different names*

### Comparing `llm_rs_metal-0.2.13/build_scripts/pyproject_patcher.py` & `llm_rs_metal-0.2.14/build_scripts/pyproject_patcher.py`

 * *Files identical despite different names*

### Comparing `llm_rs_metal-0.2.13/build_scripts/repair_windows_wheels.py` & `llm_rs_metal-0.2.14/build_scripts/repair_windows_wheels.py`

 * *Files identical despite different names*

### Comparing `llm_rs_metal-0.2.13/docs/docs/conversion.md` & `llm_rs_metal-0.2.14/docs/docs/conversion.md`

 * *Files identical despite different names*

### Comparing `llm_rs_metal-0.2.13/docs/docs/index.md` & `llm_rs_metal-0.2.14/docs/docs/index.md`

 * *Files identical despite different names*

### Comparing `llm_rs_metal-0.2.13/docs/mkdocs.yml` & `llm_rs_metal-0.2.14/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `llm_rs_metal-0.2.13/examples/langchain_example.py` & `llm_rs_metal-0.2.14/examples/langchain_example.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 from llm_rs.langchain import RustformersLLM
+from llm_rs import KnownModels, SessionConfig
 from langchain import PromptTemplate
 from langchain.chains import LLMChain
 from langchain.callbacks.streaming_stdout import StreamingStdOutCallbackHandler
 
 template="""Below is an instruction that describes a task. Write a response that appropriately completes the request.
 ### Instruction:
 {instruction}
 ### Response:
 Answer:"""
 
 prompt = PromptTemplate(input_variables=["instruction"],template=template,)
 
-llm = RustformersLLM(model_path_or_repo_id="rustformers/mpt-7b-ggml",model_file="mpt-7b-instruct-q5_1-ggjt.bin",callbacks=[StreamingStdOutCallbackHandler()])
+llm = RustformersLLM(model_path_or_repo_id="TheBloke/Nous-Hermes-13B-GGML",
+                     model_file="nous-hermes-13b.ggmlv3.q4_K_S.bin",
+                     verbose=True,
+                     model_type=KnownModels.Llama,
+                     session_config=SessionConfig(use_gpu=True),
+                     callbacks=[StreamingStdOutCallbackHandler()]
+)
 
 chain = LLMChain(llm=llm, prompt=prompt)
 
-chain.run("Write a short post congratulating rustformers on their new release of their langchain integration.")
+chain.run("Write me some Cypher Querry language examples for Neo4j. Try to use the example movie dataset. Give me 5 examples of how to create nodes and relationships and how to query them.")
```

### Comparing `llm_rs_metal-0.2.13/llm_rs/__init__.py` & `llm_rs_metal-0.2.14/llm_rs/__init__.py`

 * *Files identical despite different names*

### Comparing `llm_rs_metal-0.2.13/llm_rs/auto.py` & `llm_rs_metal-0.2.14/llm_rs/auto.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,26 @@
     KnownModels.Mpt: Mpt,
     KnownModels.GptJ: GptJ,
     KnownModels.Gpt2: Gpt2,
     KnownModels.Bloom: Bloom,
     KnownModels.Llama: Llama
 }
 
+
+_STRING_TO_KNOWN_MODEL_MAP = {
+    "gpt2": KnownModels.Gpt2,
+    "starcoder": KnownModels.Gpt2,
+    "gpt_neox": KnownModels.GptNeoX,
+    "dolly-v2": KnownModels.GptNeoX,
+    "llama": KnownModels.Llama,
+    "mpt": KnownModels.Mpt,
+    "gptj": KnownModels.GptJ,
+    "bloom": KnownModels.Bloom,
+}
+
 CURRENT_QUANTIZATION_VERSION = QuantizationVersions.V2
 
 class PathType(Enum):
     DIR = auto()
     FILE = auto()
     REPO = auto()
     UNKNOWN = auto() 
@@ -127,25 +139,24 @@
     @classmethod
     def from_pretrained(
         cls,
         model_path_or_repo_id: Union[str, os.PathLike],
         **kwargs,
     ) -> 'AutoConfig':
         path_type = _get_path_type(model_path_or_repo_id)
+        path = pathlib.Path(model_path_or_repo_id)
         if path_type == PathType.UNKNOWN:
             raise ValueError(
                 f"Model path '{model_path_or_repo_id}' doesn't exist.")
         elif path_type == PathType.FILE:
-            raise ValueError(
-                f"Model path '{model_path_or_repo_id}' is a file. "
-                "Please provide a directory or a repo id.")
+            path = path.resolve().parent
         
         auto_config = AutoConfig()
         if path_type == PathType.DIR:
-            cls._update_from_dir(str(model_path_or_repo_id), auto_config)
+            cls._update_from_dir(str(path), auto_config)
         elif path_type == PathType.REPO:
             cls._update_from_repo(str(model_path_or_repo_id), auto_config)
 
         return auto_config
 
     @classmethod
     def _update_from_repo(
@@ -165,20 +176,34 @@
             raise ValueError(f"Config path '{resolved_path}' doesn't exist.")
 
     @classmethod
     def _update_from_file(cls, path: str, auto_config: 'AutoConfig') -> None:
         with open(path) as f:
             config = json.load(f)
         auto_config.model_type = config.get('model_type')
-        auto_config.repo_type = config.get('repo_type')
+        if 'repo_type' in config:
+            auto_config.repo_type = config.get('repo_type')
+        elif len(config) == 1:
+            auto_config.repo_type = "GGML"
+        else:
+            auto_config.repo_type = "HuggingFace"
+            
+        
 
 class AutoModel():
     """
     Utility to load models, without having to specify the model type.
     """
+
+    @classmethod
+    def has_metadata_file(cls,model_file:Union[str,os.PathLike])->bool:
+        path = pathlib.Path(model_file)
+        metadata_file = path.with_suffix(".meta")
+        return metadata_file.exists()
+
     @classmethod
     def load_metadata(cls,model_file:Union[str,os.PathLike])->ModelMetadata:
         path = pathlib.Path(model_file)
         if not path.is_file():
             raise ValueError(f"Model file '{model_file}' is not a file!")
         if not path.exists():
             raise ValueError(f"Model file '{model_file}' does not exist!")
@@ -187,30 +212,40 @@
         if not metadata_file.exists():
             raise ValueError(f"Model file '{model_file}' does not have a metadata file '{metadata_file}'! If you want to autoload this model, please specify the model type.")
         
         metadata = ModelMetadata.deserialize(json.loads(metadata_file.read_text()))
         return metadata
     
     @classmethod
-    def _infer_model_type(cls,model_file:Union[str,os.PathLike],known_model:Optional[KnownModels]=None)->Type[Model]:
+    def _infer_model_type(cls,model_file:Union[str,os.PathLike],known_model:Optional[KnownModels]=None,config:Optional[AutoConfig]=None)->Type[Model]:
         model_to_lookup = None
         if known_model:
             model_to_lookup = known_model
-        else:
+        elif cls.has_metadata_file(model_file):
             metadata = cls.load_metadata(model_file)
             model_to_lookup = metadata.model
+        elif config and config.model_type:
+            if config.model_type.lower() in _STRING_TO_KNOWN_MODEL_MAP:
+                model_to_lookup = _STRING_TO_KNOWN_MODEL_MAP[config.model_type.lower()]
+            else:
+                raise ValueError(f"Unknown model type '{config.model_type}' in config file '{model_file}'! Please specify the model type via `known_model`.")
+        else:
+            raise ValueError(f"Model file '{model_file}' does not have a metadata or config file and no model type was specified! Please specify the model type via `known_model`.")
+            
 
         if model_to_lookup in _KNOWN_MODELS_MAP:
             return _KNOWN_MODELS_MAP[model_to_lookup]
         else:
             raise ValueError(f"Unknown model type '{model_to_lookup}'")
             
         
     @classmethod
-    def from_file(cls, path:Union[str,os.PathLike],
+    def from_file(cls, 
+                  path:Union[str,os.PathLike],
+                  config:Optional[AutoConfig],
                   model_type: Optional[KnownModels] = None,
                   session_config:SessionConfig=SessionConfig(),
                   tokenizer_path_or_repo_id: Optional[Union[str,os.PathLike]]=None,
                   lora_paths:Optional[List[Union[str,os.PathLike]]]=None,
                   verbose:bool=False,
                   use_hf_tokenizer:bool=True)->Model:
         
@@ -221,15 +256,15 @@
                 tokenizer = metadata.base_model
             except Exception as e:
                 logging.warning(f"Could not load metadata for model '{path}'!")
 
             if tokenizer is None or tokenizer == "":
                 logging.warning(f"Model file '{path}' does not have a base_model specified in its metadata file but wants to use a huggingface-tokenizer! Please expilicitly specify a tokenizer via `tokenizer_path_or_repo_id` if you intend to use a huggingface-tokenizer.")
 
-        model = cls._infer_model_type(path,model_type)
+        model = cls._infer_model_type(path,model_type,config)
         return model(path,session_config,tokenizer_path_or_repo_id,lora_paths,verbose)
     
     @classmethod
     def from_pretrained(cls,
         model_path_or_repo_id: Union[str,os.PathLike],
         model_file: Optional[str] = None,
         model_type: Optional[KnownModels] = None,
@@ -237,42 +272,43 @@
         tokenizer_path_or_repo_id: Optional[Union[str,os.PathLike]]=None,
         lora_paths:Optional[List[Union[str,os.PathLike]]]=None,
         verbose:bool=False,
         use_hf_tokenizer:bool=True,
         default_quantization:QuantizationType=QuantizationType.Q4_0,
         default_container:ContainerType=ContainerType.GGJT)->Model:
 
+        try: 
+            config = AutoConfig.from_pretrained(
+                model_path_or_repo_id,
+            )
+        except ValueError:
+            logging.warning("Could not find config.json in repo, assuming GGML model...")
+            config = AutoConfig(repo_type="GGML")
+
+        if model_file:
+            config.repo_type = "GGML"
+        
         path_type = _get_path_type(model_path_or_repo_id)
 
         if path_type == PathType.UNKNOWN:
             raise ValueError(f"Unknown path type for '{model_path_or_repo_id}'")
         elif path_type == PathType.FILE:
-            return cls.from_file(model_path_or_repo_id,model_type,session_config,tokenizer_path_or_repo_id,lora_paths,verbose,use_hf_tokenizer)
+            return cls.from_file(model_path_or_repo_id,config,model_type,session_config,tokenizer_path_or_repo_id,lora_paths,verbose,use_hf_tokenizer)
         else:
             if path_type == PathType.REPO:
-
-                try: 
-                    config = AutoConfig.from_pretrained(
-                        model_path_or_repo_id,
-                    )
-                except ValueError:
-                    logging.warning("Could not find config.json in repo, assuming GGML model...")
-                    config = AutoConfig(repo_type="GGML")
-                       
-
                 if config.repo_type != "GGML":
                     logging.warning("Found normal HuggingFace model, starting conversion...")
                     return cls.from_transformer(model_path_or_repo_id, session_config, tokenizer_path_or_repo_id, lora_paths, verbose, use_hf_tokenizer,default_quantization, default_container)
             
                 resolved_path = cls._find_model_path_from_repo(str(model_path_or_repo_id),model_file)
-                return cls.from_file(resolved_path,model_type,session_config,tokenizer_path_or_repo_id,lora_paths,verbose,use_hf_tokenizer)
+                return cls.from_file(resolved_path,config,model_type,session_config,tokenizer_path_or_repo_id,lora_paths,verbose,use_hf_tokenizer)
             
             elif path_type == PathType.DIR:
                 resolved_path = cls._find_model_path_from_dir(str(model_path_or_repo_id),model_file)
-                return cls.from_file(resolved_path,model_type,session_config,tokenizer_path_or_repo_id,lora_paths,verbose,use_hf_tokenizer)
+                return cls.from_file(resolved_path,config,model_type,session_config,tokenizer_path_or_repo_id,lora_paths,verbose,use_hf_tokenizer)
             
             else:
                 raise ValueError(f"Unknown path type '{path_type}'")
 
 
     @classmethod
     def _find_model_path_from_dir(
```

### Comparing `llm_rs_metal-0.2.13/llm_rs/base_model.py` & `llm_rs_metal-0.2.14/llm_rs/base_model.py`

 * *Files identical despite different names*

### Comparing `llm_rs_metal-0.2.13/llm_rs/config.pyi` & `llm_rs_metal-0.2.14/llm_rs/config.pyi`

 * *Files identical despite different names*

### Comparing `llm_rs_metal-0.2.13/llm_rs/convert/auto_converter.py` & `llm_rs_metal-0.2.14/llm_rs/convert/auto_converter.py`

 * *Files identical despite different names*

### Comparing `llm_rs_metal-0.2.13/llm_rs/convert/models/_base.py` & `llm_rs_metal-0.2.14/llm_rs/convert/models/_base.py`

 * *Files identical despite different names*

### Comparing `llm_rs_metal-0.2.13/llm_rs/convert/models/bloom.py` & `llm_rs_metal-0.2.14/llm_rs/convert/models/bloom.py`

 * *Files identical despite different names*

### Comparing `llm_rs_metal-0.2.13/llm_rs/convert/models/gpt2.py` & `llm_rs_metal-0.2.14/llm_rs/convert/models/gpt2.py`

 * *Files identical despite different names*

### Comparing `llm_rs_metal-0.2.13/llm_rs/convert/models/gptj.py` & `llm_rs_metal-0.2.14/llm_rs/convert/models/gptj.py`

 * *Files identical despite different names*

### Comparing `llm_rs_metal-0.2.13/llm_rs/convert/models/gptneox.py` & `llm_rs_metal-0.2.14/llm_rs/convert/models/gptneox.py`

 * *Files identical despite different names*

### Comparing `llm_rs_metal-0.2.13/llm_rs/convert/models/llama.py` & `llm_rs_metal-0.2.14/llm_rs/convert/models/llama.py`

 * *Files identical despite different names*

### Comparing `llm_rs_metal-0.2.13/llm_rs/convert/models/mpt.py` & `llm_rs_metal-0.2.14/llm_rs/convert/models/mpt.py`

 * *Files identical despite different names*

### Comparing `llm_rs_metal-0.2.13/llm_rs/haystack/haystack.py` & `llm_rs_metal-0.2.14/llm_rs/haystack/haystack.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 try:
     from haystack.nodes import PromptModelInvocationLayer
     from haystack.nodes.prompt.invocation_layer import DefaultTokenStreamingHandler
 except ImportError:
      raise ImportError(
-        'To use the llm_rs.haystack module, please install llm-rs with the additional "haystack" dependencies via: pip install llm-rs[haystack]')
+        'To use the llm_rs.haystack module, please install llm-rs with the additional "haystack" dependencies e.g. via: pip install llm-rs[haystack]')
 
 import os
 from typing import Dict, List, Union, Type, Optional
 from ..auto import AutoModel,KnownModels
 from ..config import QuantizationType,ContainerType,SessionConfig,GenerationConfig
 from ..base_model import Model
 import logging
```

### Comparing `llm_rs_metal-0.2.13/llm_rs/langchain/langchain.py` & `llm_rs_metal-0.2.14/llm_rs/langchain/langchain.py`

 * *Files identical despite different names*

### Comparing `llm_rs_metal-0.2.13/llm_rs/models.pyi` & `llm_rs_metal-0.2.14/llm_rs/models.pyi`

 * *Files identical despite different names*

### Comparing `llm_rs_metal-0.2.13/llm_rs/repository.py` & `llm_rs_metal-0.2.14/llm_rs/repository.py`

 * *Files identical despite different names*

### Comparing `llm_rs_metal-0.2.13/llm_rs/results.pyi` & `llm_rs_metal-0.2.14/llm_rs/results.pyi`

 * *Files identical despite different names*

### Comparing `llm_rs_metal-0.2.13/pyproject.toml` & `llm_rs_metal-0.2.14/pyproject.toml`

 * *Files identical despite different names*

### Comparing `llm_rs_metal-0.2.13/src/configs.rs` & `llm_rs_metal-0.2.14/src/configs.rs`

 * *Files identical despite different names*

### Comparing `llm_rs_metal-0.2.13/src/lib.rs` & `llm_rs_metal-0.2.14/src/lib.rs`

 * *Files identical despite different names*

### Comparing `llm_rs_metal-0.2.13/src/model_base.rs` & `llm_rs_metal-0.2.14/src/model_base.rs`

 * *Files identical despite different names*

### Comparing `llm_rs_metal-0.2.13/src/quantize.rs` & `llm_rs_metal-0.2.14/src/quantize.rs`

 * *Files identical despite different names*

### Comparing `llm_rs_metal-0.2.13/src/results.rs` & `llm_rs_metal-0.2.14/src/results.rs`

 * *Files identical despite different names*

### Comparing `llm_rs_metal-0.2.13/src/stopwords.rs` & `llm_rs_metal-0.2.14/src/stopwords.rs`

 * *Files identical despite different names*

### Comparing `llm_rs_metal-0.2.13/Cargo.lock` & `llm_rs_metal-0.2.14/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -960,15 +960,15 @@
 source = "git+https://github.com/rustformers/llm.git?rev=5d09eed#5d09eed687f90466b5d6e883bc8de0c43d675cd9"
 dependencies = [
  "llm-base",
 ]
 
 [[package]]
 name = "llm-rs"
-version = "0.2.13"
+version = "0.2.14"
 dependencies = [
  "llm",
  "llm-base",
  "log",
  "pyo3",
  "rand",
  "rand_chacha",
@@ -1768,17 +1768,17 @@
  "filetime",
  "libc",
  "xattr",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.9"
+version = "0.12.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "df8e77cb757a61f51b947ec4a7e3646efd825b73561db1c232a8ccb639e611a0"
+checksum = "1d2faeef5759ab89935255b1a4cd98e0baf99d1085e37d36599c625dac49ae8e"
 
 [[package]]
 name = "tempfile"
 version = "3.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "31c0432476357e58790aaa47a8efb0c5138f137343f3b5f23bd36a27e3b0a6d6"
 dependencies = [
```

### Comparing `llm_rs_metal-0.2.13/PKG-INFO` & `llm_rs_metal-0.2.14/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-rs-metal
-Version: 0.2.13
+Version: 0.2.14
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: blake3
 Requires-Dist: huggingface-hub >= 0.14.1
```

