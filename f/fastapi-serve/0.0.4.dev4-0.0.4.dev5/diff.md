# Comparing `tmp/fastapi-serve-0.0.4.dev4.tar.gz` & `tmp/fastapi-serve-0.0.4.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-serve-0.0.4.dev4.tar", last modified: Wed Jul 19 06:07:16 2023, max compression
+gzip compressed data, was "fastapi-serve-0.0.4.dev5.tar", last modified: Wed Jul 19 06:08:34 2023, max compression
```

## Comparing `fastapi-serve-0.0.4.dev4.tar` & `fastapi-serve-0.0.4.dev5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 06:07:16.829574 fastapi-serve-0.0.4.dev4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-19 06:07:12.000000 fastapi-serve-0.0.4.dev4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-19 06:07:12.000000 fastapi-serve-0.0.4.dev4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-07-19 06:07:16.829574 fastapi-serve-0.0.4.dev4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-07-19 06:07:12.000000 fastapi-serve-0.0.4.dev4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 06:07:16.829574 fastapi-serve-0.0.4.dev4/fastapi_serve/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-19 06:07:16.000000 fastapi-serve-0.0.4.dev4/fastapi_serve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-19 06:07:12.000000 fastapi-serve-0.0.4.dev4/fastapi_serve/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 06:07:16.829574 fastapi-serve-0.0.4.dev4/fastapi_serve/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-19 06:07:12.000000 fastapi-serve-0.0.4.dev4/fastapi_serve/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-07-19 06:07:12.000000 fastapi-serve-0.0.4.dev4/fastapi_serve/cloud/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     7902 2023-07-19 06:07:12.000000 fastapi-serve-0.0.4.dev4/fastapi_serve/cloud/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-07-19 06:07:12.000000 fastapi-serve-0.0.4.dev4/fastapi_serve/cloud/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-19 06:07:12.000000 fastapi-serve-0.0.4.dev4/fastapi_serve/cloud/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-19 06:07:12.000000 fastapi-serve-0.0.4.dev4/fastapi_serve/cloud/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-07-19 06:07:12.000000 fastapi-serve-0.0.4.dev4/fastapi_serve/cloud/options.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-19 06:07:12.000000 fastapi-serve-0.0.4.dev4/fastapi_serve/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 06:07:16.829574 fastapi-serve-0.0.4.dev4/fastapi_serve/gateway/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-19 06:07:12.000000 fastapi-serve-0.0.4.dev4/fastapi_serve/gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-07-19 06:07:12.000000 fastapi-serve-0.0.4.dev4/fastapi_serve/gateway/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-07-19 06:07:12.000000 fastapi-serve-0.0.4.dev4/fastapi_serve/gateway/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-07-19 06:07:12.000000 fastapi-serve-0.0.4.dev4/fastapi_serve/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 06:07:16.829574 fastapi-serve-0.0.4.dev4/fastapi_serve/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-19 06:07:12.000000 fastapi-serve-0.0.4.dev4/fastapi_serve/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-19 06:07:12.000000 fastapi-serve-0.0.4.dev4/fastapi_serve/utils/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 06:07:16.829574 fastapi-serve-0.0.4.dev4/fastapi_serve/utils/blob/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-19 06:07:12.000000 fastapi-serve-0.0.4.dev4/fastapi_serve/utils/blob/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-07-19 06:07:12.000000 fastapi-serve-0.0.4.dev4/fastapi_serve/utils/blob/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-19 06:07:12.000000 fastapi-serve-0.0.4.dev4/fastapi_serve/utils/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 06:07:16.829574 fastapi-serve-0.0.4.dev4/fastapi_serve.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-07-19 06:07:16.000000 fastapi-serve-0.0.4.dev4/fastapi_serve.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-19 06:07:16.000000 fastapi-serve-0.0.4.dev4/fastapi_serve.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 06:07:16.000000 fastapi-serve-0.0.4.dev4/fastapi_serve.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-19 06:07:16.000000 fastapi-serve-0.0.4.dev4/fastapi_serve.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 06:07:16.000000 fastapi-serve-0.0.4.dev4/fastapi_serve.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-19 06:07:16.000000 fastapi-serve-0.0.4.dev4/fastapi_serve.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-19 06:07:16.000000 fastapi-serve-0.0.4.dev4/fastapi_serve.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-19 06:07:12.000000 fastapi-serve-0.0.4.dev4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 06:07:16.829574 fastapi-serve-0.0.4.dev4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-19 06:07:12.000000 fastapi-serve-0.0.4.dev4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 06:08:34.581248 fastapi-serve-0.0.4.dev5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-19 06:08:26.000000 fastapi-serve-0.0.4.dev5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-19 06:08:26.000000 fastapi-serve-0.0.4.dev5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-07-19 06:08:34.581248 fastapi-serve-0.0.4.dev5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-07-19 06:08:26.000000 fastapi-serve-0.0.4.dev5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 06:08:34.577248 fastapi-serve-0.0.4.dev5/fastapi_serve/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-19 06:08:34.000000 fastapi-serve-0.0.4.dev5/fastapi_serve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-19 06:08:26.000000 fastapi-serve-0.0.4.dev5/fastapi_serve/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 06:08:34.577248 fastapi-serve-0.0.4.dev5/fastapi_serve/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-19 06:08:26.000000 fastapi-serve-0.0.4.dev5/fastapi_serve/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-07-19 06:08:26.000000 fastapi-serve-0.0.4.dev5/fastapi_serve/cloud/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7902 2023-07-19 06:08:26.000000 fastapi-serve-0.0.4.dev5/fastapi_serve/cloud/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-07-19 06:08:26.000000 fastapi-serve-0.0.4.dev5/fastapi_serve/cloud/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-19 06:08:26.000000 fastapi-serve-0.0.4.dev5/fastapi_serve/cloud/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-19 06:08:26.000000 fastapi-serve-0.0.4.dev5/fastapi_serve/cloud/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-07-19 06:08:26.000000 fastapi-serve-0.0.4.dev5/fastapi_serve/cloud/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-19 06:08:26.000000 fastapi-serve-0.0.4.dev5/fastapi_serve/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 06:08:34.577248 fastapi-serve-0.0.4.dev5/fastapi_serve/gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-19 06:08:26.000000 fastapi-serve-0.0.4.dev5/fastapi_serve/gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-07-19 06:08:26.000000 fastapi-serve-0.0.4.dev5/fastapi_serve/gateway/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-07-19 06:08:26.000000 fastapi-serve-0.0.4.dev5/fastapi_serve/gateway/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-07-19 06:08:26.000000 fastapi-serve-0.0.4.dev5/fastapi_serve/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 06:08:34.577248 fastapi-serve-0.0.4.dev5/fastapi_serve/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-19 06:08:26.000000 fastapi-serve-0.0.4.dev5/fastapi_serve/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-19 06:08:26.000000 fastapi-serve-0.0.4.dev5/fastapi_serve/utils/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 06:08:34.577248 fastapi-serve-0.0.4.dev5/fastapi_serve/utils/blob/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-19 06:08:26.000000 fastapi-serve-0.0.4.dev5/fastapi_serve/utils/blob/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-07-19 06:08:26.000000 fastapi-serve-0.0.4.dev5/fastapi_serve/utils/blob/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-19 06:08:26.000000 fastapi-serve-0.0.4.dev5/fastapi_serve/utils/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 06:08:34.577248 fastapi-serve-0.0.4.dev5/fastapi_serve.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-07-19 06:08:34.000000 fastapi-serve-0.0.4.dev5/fastapi_serve.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-19 06:08:34.000000 fastapi-serve-0.0.4.dev5/fastapi_serve.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 06:08:34.000000 fastapi-serve-0.0.4.dev5/fastapi_serve.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-19 06:08:34.000000 fastapi-serve-0.0.4.dev5/fastapi_serve.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 06:08:34.000000 fastapi-serve-0.0.4.dev5/fastapi_serve.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-19 06:08:34.000000 fastapi-serve-0.0.4.dev5/fastapi_serve.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-19 06:08:34.000000 fastapi-serve-0.0.4.dev5/fastapi_serve.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-19 06:08:26.000000 fastapi-serve-0.0.4.dev5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 06:08:34.581248 fastapi-serve-0.0.4.dev5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-19 06:08:26.000000 fastapi-serve-0.0.4.dev5/setup.py
```

### Comparing `fastapi-serve-0.0.4.dev4/LICENSE` & `fastapi-serve-0.0.4.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.4.dev4/PKG-INFO` & `fastapi-serve-0.0.4.dev5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-serve
-Version: 0.0.4.dev4
+Version: 0.0.4.dev5
 Summary: FastAPI Serve - FastAPI to the Cloud, Batteries Included!
 Home-page: https://github.com/jina-ai/fastapi-serve/
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/fastapi-serve/tags
 Project-URL: Documentation, https://docs.jina.ai
@@ -76,27 +76,27 @@
 Dive into understanding `fastapi-serve` through our comprehensive documentation and examples:
 
 - 🚀 **Getting Started**
     - 🧱 [Deploy a Simple FastAPI Application](docs/simple/)
     - 🖥️ [Dig deep into the `fastapi-serve` CLI](docs/CLI.md)
     - ⚙️ [Understanding Configuration and Pricing](docs/CONFIG.MD)
 - ↕️ **Scaling**
-    - 💹 [**Auto-scaling** endpoints based on CPU usage](docs/autoscaling/cpu/)
-    - 📉 [**Serverless** (scale-to-zero) deployments based on requests-per-second](docs/autoscaling/serverless/) 
+    - 💹 [Auto-scaling endpoints based on CPU usage](docs/autoscaling/cpu/)
+    - 📉 [Serverless (scale-to-zero) deployments based on requests-per-second](docs/autoscaling/serverless/) 
 - 🧩 **Config & Credentials**
-    - 🌍 Leverage **Environment Variables** for app configuration (Example TBD!)
-    - 🗝️ [Use **Secrets** for Redis-Powered Rate Limiting](docs/rate_limit/)
+    - 🌍 Leverage Environment Variables for app configuration (Example TBD!)
+    - 🗝️ [Use Secrets for Redis-Powered Rate Limiting](docs/rate_limit/)
 - 💾 **Storage**
-    - 📁 [Handle File Uploads and Downloads with built-in **Blob Storage**](docs/file_handling/)
+    - 📁 [Handle File Uploads and Downloads with built-in Blob Storage](docs/file_handling/)
     - 🌐 Network Storage for persisting and securely accessing app data (Example TBD!)
 - 🔒 **Security**
-    - 👮‍♂️ [Secure Your Endpoints with built-in **OAuth2.0 Authorization**](docs/authorization/)
+    - 👮‍♂️ [Secure Your Endpoints with built-in OAuth2.0 Authorization](docs/authorization/)
 - 🐳 **Deployment Options**
-    - 🚢 Deployment with **Custom Dockerfile** (Coming Soon!)
-    - 🛠️ Export Your App for **Self-Hosting** with docker-compose / Kubernetes (Coming Soon!)
+    - 🚢 Deployment with Custom Dockerfile (Coming Soon!)
+    - 🛠️ Export Your App for Self-Hosting with docker-compose / Kubernetes (Coming Soon!)
 
 
 ## 💪 Support
 
 If you encounter any problems or have questions, feel free to open an issue on the GitHub repository. You can also join our [Discord](https://discord.jina.ai/) to get help from our community members and the Jina team.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi-serve Version: 0.0.4.dev4 Summary: FastAPI
+Metadata-Version: 2.1 Name: fastapi-serve Version: 0.0.4.dev5 Summary: FastAPI
 Serve - FastAPI to the Cloud, Batteries Included! Home-page: https://
 github.com/jina-ai/fastapi-serve/ Author: Jina AI Author-email: hello@jina.ai
 License: Apache 2.0 Download-URL: https://github.com/jina-ai/fastapi-serve/tags
 Project-URL: Documentation, https://docs.jina.ai Project-URL: Source, https://
 github.com/jina-ai/fastapi-serve/ Project-URL: Tracker, https://github.com/
 jina-ai/fastapi-serve/issues Keywords: jina fastapi restapi cloud docker
 kubernetes Platform: UNKNOWN Classifier: Development Status :: 5 - Production/
@@ -42,30 +42,30 @@
 use the `fastapi-serve` command to deploy your FastAPI application: ```bash
 fastapi-serve deploy jcloud app:app ``` You'll get a URL to access your newly
 deployed application along with the Swagger UI. ## ð Documentation Dive into
 understanding `fastapi-serve` through our comprehensive documentation and
 examples: - ð **Getting Started** - ð§± [Deploy a Simple FastAPI
 Application](docs/simple/) - ð¥ï¸ [Dig deep into the `fastapi-serve` CLI]
 (docs/CLI.md) - âï¸ [Understanding Configuration and Pricing](docs/
-CONFIG.MD) - âï¸ **Scaling** - ð¹ [**Auto-scaling** endpoints based on CPU
-usage](docs/autoscaling/cpu/) - ð [**Serverless** (scale-to-zero)
-deployments based on requests-per-second](docs/autoscaling/serverless/) - ð§©
-**Config & Credentials** - ð Leverage **Environment Variables** for app
-configuration (Example TBD!) - ðï¸ [Use **Secrets** for Redis-Powered Rate
-Limiting](docs/rate_limit/) - ð¾ **Storage** - ð [Handle File Uploads and
-Downloads with built-in **Blob Storage**](docs/file_handling/) - ð Network
-Storage for persisting and securely accessing app data (Example TBD!) - ð
-**Security** - ð®ââï¸ [Secure Your Endpoints with built-in **OAuth2.0
-Authorization**](docs/authorization/) - ð³ **Deployment Options** - ð¢
-Deployment with **Custom Dockerfile** (Coming Soon!) - ð ï¸ Export Your App
-for **Self-Hosting** with docker-compose / Kubernetes (Coming Soon!) ## ðª
-Support If you encounter any problems or have questions, feel free to open an
-issue on the GitHub repository. You can also join our [Discord](https://
-discord.jina.ai/) to get help from our community members and the Jina team. ##
-ð Our Cloud Platform `cloud.jina.ai` is our robust and scalable cloud
-platform designed to run your FastAPI applications with minimum hassle and
-maximum efficiency. With features like auto-scaling, integrated observability,
-and automated containerization, it provides a seamless and worry-free
-deployment experience. --- `fastapi-serve` is more than just a deployment tool,
-it's a bridge that connects your local development environment with our
-powerful cloud infrastructure. Start using `fastapi-serve` today, and
-experience the joy of effortless deployments! ð
+CONFIG.MD) - âï¸ **Scaling** - ð¹ [Auto-scaling endpoints based on CPU
+usage](docs/autoscaling/cpu/) - ð [Serverless (scale-to-zero) deployments
+based on requests-per-second](docs/autoscaling/serverless/) - ð§© **Config &
+Credentials** - ð Leverage Environment Variables for app configuration
+(Example TBD!) - ðï¸ [Use Secrets for Redis-Powered Rate Limiting](docs/
+rate_limit/) - ð¾ **Storage** - ð [Handle File Uploads and Downloads with
+built-in Blob Storage](docs/file_handling/) - ð Network Storage for
+persisting and securely accessing app data (Example TBD!) - ð **Security** -
+ð®ââï¸ [Secure Your Endpoints with built-in OAuth2.0 Authorization]
+(docs/authorization/) - ð³ **Deployment Options** - ð¢ Deployment with
+Custom Dockerfile (Coming Soon!) - ð ï¸ Export Your App for Self-Hosting
+with docker-compose / Kubernetes (Coming Soon!) ## ðª Support If you
+encounter any problems or have questions, feel free to open an issue on the
+GitHub repository. You can also join our [Discord](https://discord.jina.ai/) to
+get help from our community members and the Jina team. ## ð Our Cloud
+Platform `cloud.jina.ai` is our robust and scalable cloud platform designed to
+run your FastAPI applications with minimum hassle and maximum efficiency. With
+features like auto-scaling, integrated observability, and automated
+containerization, it provides a seamless and worry-free deployment experience.
+--- `fastapi-serve` is more than just a deployment tool, it's a bridge that
+connects your local development environment with our powerful cloud
+infrastructure. Start using `fastapi-serve` today, and experience the joy of
+effortless deployments! ð
```

### Comparing `fastapi-serve-0.0.4.dev4/README.md` & `fastapi-serve-0.0.4.dev5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -46,27 +46,27 @@
 Dive into understanding `fastapi-serve` through our comprehensive documentation and examples:
 
 - 🚀 **Getting Started**
     - 🧱 [Deploy a Simple FastAPI Application](docs/simple/)
     - 🖥️ [Dig deep into the `fastapi-serve` CLI](docs/CLI.md)
     - ⚙️ [Understanding Configuration and Pricing](docs/CONFIG.MD)
 - ↕️ **Scaling**
-    - 💹 [**Auto-scaling** endpoints based on CPU usage](docs/autoscaling/cpu/)
-    - 📉 [**Serverless** (scale-to-zero) deployments based on requests-per-second](docs/autoscaling/serverless/) 
+    - 💹 [Auto-scaling endpoints based on CPU usage](docs/autoscaling/cpu/)
+    - 📉 [Serverless (scale-to-zero) deployments based on requests-per-second](docs/autoscaling/serverless/) 
 - 🧩 **Config & Credentials**
-    - 🌍 Leverage **Environment Variables** for app configuration (Example TBD!)
-    - 🗝️ [Use **Secrets** for Redis-Powered Rate Limiting](docs/rate_limit/)
+    - 🌍 Leverage Environment Variables for app configuration (Example TBD!)
+    - 🗝️ [Use Secrets for Redis-Powered Rate Limiting](docs/rate_limit/)
 - 💾 **Storage**
-    - 📁 [Handle File Uploads and Downloads with built-in **Blob Storage**](docs/file_handling/)
+    - 📁 [Handle File Uploads and Downloads with built-in Blob Storage](docs/file_handling/)
     - 🌐 Network Storage for persisting and securely accessing app data (Example TBD!)
 - 🔒 **Security**
-    - 👮‍♂️ [Secure Your Endpoints with built-in **OAuth2.0 Authorization**](docs/authorization/)
+    - 👮‍♂️ [Secure Your Endpoints with built-in OAuth2.0 Authorization](docs/authorization/)
 - 🐳 **Deployment Options**
-    - 🚢 Deployment with **Custom Dockerfile** (Coming Soon!)
-    - 🛠️ Export Your App for **Self-Hosting** with docker-compose / Kubernetes (Coming Soon!)
+    - 🚢 Deployment with Custom Dockerfile (Coming Soon!)
+    - 🛠️ Export Your App for Self-Hosting with docker-compose / Kubernetes (Coming Soon!)
 
 
 ## 💪 Support
 
 If you encounter any problems or have questions, feel free to open an issue on the GitHub repository. You can also join our [Discord](https://discord.jina.ai/) to get help from our community members and the Jina team.
```

#### html2text {}

```diff
@@ -25,30 +25,30 @@
 use the `fastapi-serve` command to deploy your FastAPI application: ```bash
 fastapi-serve deploy jcloud app:app ``` You'll get a URL to access your newly
 deployed application along with the Swagger UI. ## ð Documentation Dive into
 understanding `fastapi-serve` through our comprehensive documentation and
 examples: - ð **Getting Started** - ð§± [Deploy a Simple FastAPI
 Application](docs/simple/) - ð¥ï¸ [Dig deep into the `fastapi-serve` CLI]
 (docs/CLI.md) - âï¸ [Understanding Configuration and Pricing](docs/
-CONFIG.MD) - âï¸ **Scaling** - ð¹ [**Auto-scaling** endpoints based on CPU
-usage](docs/autoscaling/cpu/) - ð [**Serverless** (scale-to-zero)
-deployments based on requests-per-second](docs/autoscaling/serverless/) - ð§©
-**Config & Credentials** - ð Leverage **Environment Variables** for app
-configuration (Example TBD!) - ðï¸ [Use **Secrets** for Redis-Powered Rate
-Limiting](docs/rate_limit/) - ð¾ **Storage** - ð [Handle File Uploads and
-Downloads with built-in **Blob Storage**](docs/file_handling/) - ð Network
-Storage for persisting and securely accessing app data (Example TBD!) - ð
-**Security** - ð®ââï¸ [Secure Your Endpoints with built-in **OAuth2.0
-Authorization**](docs/authorization/) - ð³ **Deployment Options** - ð¢
-Deployment with **Custom Dockerfile** (Coming Soon!) - ð ï¸ Export Your App
-for **Self-Hosting** with docker-compose / Kubernetes (Coming Soon!) ## ðª
-Support If you encounter any problems or have questions, feel free to open an
-issue on the GitHub repository. You can also join our [Discord](https://
-discord.jina.ai/) to get help from our community members and the Jina team. ##
-ð Our Cloud Platform `cloud.jina.ai` is our robust and scalable cloud
-platform designed to run your FastAPI applications with minimum hassle and
-maximum efficiency. With features like auto-scaling, integrated observability,
-and automated containerization, it provides a seamless and worry-free
-deployment experience. --- `fastapi-serve` is more than just a deployment tool,
-it's a bridge that connects your local development environment with our
-powerful cloud infrastructure. Start using `fastapi-serve` today, and
-experience the joy of effortless deployments! ð
+CONFIG.MD) - âï¸ **Scaling** - ð¹ [Auto-scaling endpoints based on CPU
+usage](docs/autoscaling/cpu/) - ð [Serverless (scale-to-zero) deployments
+based on requests-per-second](docs/autoscaling/serverless/) - ð§© **Config &
+Credentials** - ð Leverage Environment Variables for app configuration
+(Example TBD!) - ðï¸ [Use Secrets for Redis-Powered Rate Limiting](docs/
+rate_limit/) - ð¾ **Storage** - ð [Handle File Uploads and Downloads with
+built-in Blob Storage](docs/file_handling/) - ð Network Storage for
+persisting and securely accessing app data (Example TBD!) - ð **Security** -
+ð®ââï¸ [Secure Your Endpoints with built-in OAuth2.0 Authorization]
+(docs/authorization/) - ð³ **Deployment Options** - ð¢ Deployment with
+Custom Dockerfile (Coming Soon!) - ð ï¸ Export Your App for Self-Hosting
+with docker-compose / Kubernetes (Coming Soon!) ## ðª Support If you
+encounter any problems or have questions, feel free to open an issue on the
+GitHub repository. You can also join our [Discord](https://discord.jina.ai/) to
+get help from our community members and the Jina team. ## ð Our Cloud
+Platform `cloud.jina.ai` is our robust and scalable cloud platform designed to
+run your FastAPI applications with minimum hassle and maximum efficiency. With
+features like auto-scaling, integrated observability, and automated
+containerization, it provides a seamless and worry-free deployment experience.
+--- `fastapi-serve` is more than just a deployment tool, it's a bridge that
+connects your local development environment with our powerful cloud
+infrastructure. Start using `fastapi-serve` today, and experience the joy of
+effortless deployments! ð
```

### Comparing `fastapi-serve-0.0.4.dev4/fastapi_serve/__main__.py` & `fastapi-serve-0.0.4.dev5/fastapi_serve/__main__.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.4.dev4/fastapi_serve/cloud/build.py` & `fastapi-serve-0.0.4.dev5/fastapi_serve/cloud/build.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.4.dev4/fastapi_serve/cloud/config.py` & `fastapi-serve-0.0.4.dev5/fastapi_serve/cloud/config.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.4.dev4/fastapi_serve/cloud/deploy.py` & `fastapi-serve-0.0.4.dev5/fastapi_serve/cloud/deploy.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.4.dev4/fastapi_serve/cloud/errors.py` & `fastapi-serve-0.0.4.dev5/fastapi_serve/cloud/errors.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.4.dev4/fastapi_serve/cloud/helper.py` & `fastapi-serve-0.0.4.dev5/fastapi_serve/cloud/helper.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.4.dev4/fastapi_serve/cloud/options.py` & `fastapi-serve-0.0.4.dev5/fastapi_serve/cloud/options.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.4.dev4/fastapi_serve/gateway/gateway.py` & `fastapi-serve-0.0.4.dev5/fastapi_serve/gateway/gateway.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.4.dev4/fastapi_serve/gateway/helper.py` & `fastapi-serve-0.0.4.dev5/fastapi_serve/gateway/helper.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.4.dev4/fastapi_serve/helper.py` & `fastapi-serve-0.0.4.dev5/fastapi_serve/helper.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.4.dev4/fastapi_serve/utils/auth.py` & `fastapi-serve-0.0.4.dev5/fastapi_serve/utils/auth.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.4.dev4/fastapi_serve/utils/blob/storage.py` & `fastapi-serve-0.0.4.dev5/fastapi_serve/utils/blob/storage.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.4.dev4/fastapi_serve/utils/helper.py` & `fastapi-serve-0.0.4.dev5/fastapi_serve/utils/helper.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.4.dev4/fastapi_serve.egg-info/PKG-INFO` & `fastapi-serve-0.0.4.dev5/fastapi_serve.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-serve
-Version: 0.0.4.dev4
+Version: 0.0.4.dev5
 Summary: FastAPI Serve - FastAPI to the Cloud, Batteries Included!
 Home-page: https://github.com/jina-ai/fastapi-serve/
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Download-URL: https://github.com/jina-ai/fastapi-serve/tags
 Project-URL: Documentation, https://docs.jina.ai
@@ -76,27 +76,27 @@
 Dive into understanding `fastapi-serve` through our comprehensive documentation and examples:
 
 - 🚀 **Getting Started**
     - 🧱 [Deploy a Simple FastAPI Application](docs/simple/)
     - 🖥️ [Dig deep into the `fastapi-serve` CLI](docs/CLI.md)
     - ⚙️ [Understanding Configuration and Pricing](docs/CONFIG.MD)
 - ↕️ **Scaling**
-    - 💹 [**Auto-scaling** endpoints based on CPU usage](docs/autoscaling/cpu/)
-    - 📉 [**Serverless** (scale-to-zero) deployments based on requests-per-second](docs/autoscaling/serverless/) 
+    - 💹 [Auto-scaling endpoints based on CPU usage](docs/autoscaling/cpu/)
+    - 📉 [Serverless (scale-to-zero) deployments based on requests-per-second](docs/autoscaling/serverless/) 
 - 🧩 **Config & Credentials**
-    - 🌍 Leverage **Environment Variables** for app configuration (Example TBD!)
-    - 🗝️ [Use **Secrets** for Redis-Powered Rate Limiting](docs/rate_limit/)
+    - 🌍 Leverage Environment Variables for app configuration (Example TBD!)
+    - 🗝️ [Use Secrets for Redis-Powered Rate Limiting](docs/rate_limit/)
 - 💾 **Storage**
-    - 📁 [Handle File Uploads and Downloads with built-in **Blob Storage**](docs/file_handling/)
+    - 📁 [Handle File Uploads and Downloads with built-in Blob Storage](docs/file_handling/)
     - 🌐 Network Storage for persisting and securely accessing app data (Example TBD!)
 - 🔒 **Security**
-    - 👮‍♂️ [Secure Your Endpoints with built-in **OAuth2.0 Authorization**](docs/authorization/)
+    - 👮‍♂️ [Secure Your Endpoints with built-in OAuth2.0 Authorization](docs/authorization/)
 - 🐳 **Deployment Options**
-    - 🚢 Deployment with **Custom Dockerfile** (Coming Soon!)
-    - 🛠️ Export Your App for **Self-Hosting** with docker-compose / Kubernetes (Coming Soon!)
+    - 🚢 Deployment with Custom Dockerfile (Coming Soon!)
+    - 🛠️ Export Your App for Self-Hosting with docker-compose / Kubernetes (Coming Soon!)
 
 
 ## 💪 Support
 
 If you encounter any problems or have questions, feel free to open an issue on the GitHub repository. You can also join our [Discord](https://discord.jina.ai/) to get help from our community members and the Jina team.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi-serve Version: 0.0.4.dev4 Summary: FastAPI
+Metadata-Version: 2.1 Name: fastapi-serve Version: 0.0.4.dev5 Summary: FastAPI
 Serve - FastAPI to the Cloud, Batteries Included! Home-page: https://
 github.com/jina-ai/fastapi-serve/ Author: Jina AI Author-email: hello@jina.ai
 License: Apache 2.0 Download-URL: https://github.com/jina-ai/fastapi-serve/tags
 Project-URL: Documentation, https://docs.jina.ai Project-URL: Source, https://
 github.com/jina-ai/fastapi-serve/ Project-URL: Tracker, https://github.com/
 jina-ai/fastapi-serve/issues Keywords: jina fastapi restapi cloud docker
 kubernetes Platform: UNKNOWN Classifier: Development Status :: 5 - Production/
@@ -42,30 +42,30 @@
 use the `fastapi-serve` command to deploy your FastAPI application: ```bash
 fastapi-serve deploy jcloud app:app ``` You'll get a URL to access your newly
 deployed application along with the Swagger UI. ## ð Documentation Dive into
 understanding `fastapi-serve` through our comprehensive documentation and
 examples: - ð **Getting Started** - ð§± [Deploy a Simple FastAPI
 Application](docs/simple/) - ð¥ï¸ [Dig deep into the `fastapi-serve` CLI]
 (docs/CLI.md) - âï¸ [Understanding Configuration and Pricing](docs/
-CONFIG.MD) - âï¸ **Scaling** - ð¹ [**Auto-scaling** endpoints based on CPU
-usage](docs/autoscaling/cpu/) - ð [**Serverless** (scale-to-zero)
-deployments based on requests-per-second](docs/autoscaling/serverless/) - ð§©
-**Config & Credentials** - ð Leverage **Environment Variables** for app
-configuration (Example TBD!) - ðï¸ [Use **Secrets** for Redis-Powered Rate
-Limiting](docs/rate_limit/) - ð¾ **Storage** - ð [Handle File Uploads and
-Downloads with built-in **Blob Storage**](docs/file_handling/) - ð Network
-Storage for persisting and securely accessing app data (Example TBD!) - ð
-**Security** - ð®ââï¸ [Secure Your Endpoints with built-in **OAuth2.0
-Authorization**](docs/authorization/) - ð³ **Deployment Options** - ð¢
-Deployment with **Custom Dockerfile** (Coming Soon!) - ð ï¸ Export Your App
-for **Self-Hosting** with docker-compose / Kubernetes (Coming Soon!) ## ðª
-Support If you encounter any problems or have questions, feel free to open an
-issue on the GitHub repository. You can also join our [Discord](https://
-discord.jina.ai/) to get help from our community members and the Jina team. ##
-ð Our Cloud Platform `cloud.jina.ai` is our robust and scalable cloud
-platform designed to run your FastAPI applications with minimum hassle and
-maximum efficiency. With features like auto-scaling, integrated observability,
-and automated containerization, it provides a seamless and worry-free
-deployment experience. --- `fastapi-serve` is more than just a deployment tool,
-it's a bridge that connects your local development environment with our
-powerful cloud infrastructure. Start using `fastapi-serve` today, and
-experience the joy of effortless deployments! ð
+CONFIG.MD) - âï¸ **Scaling** - ð¹ [Auto-scaling endpoints based on CPU
+usage](docs/autoscaling/cpu/) - ð [Serverless (scale-to-zero) deployments
+based on requests-per-second](docs/autoscaling/serverless/) - ð§© **Config &
+Credentials** - ð Leverage Environment Variables for app configuration
+(Example TBD!) - ðï¸ [Use Secrets for Redis-Powered Rate Limiting](docs/
+rate_limit/) - ð¾ **Storage** - ð [Handle File Uploads and Downloads with
+built-in Blob Storage](docs/file_handling/) - ð Network Storage for
+persisting and securely accessing app data (Example TBD!) - ð **Security** -
+ð®ââï¸ [Secure Your Endpoints with built-in OAuth2.0 Authorization]
+(docs/authorization/) - ð³ **Deployment Options** - ð¢ Deployment with
+Custom Dockerfile (Coming Soon!) - ð ï¸ Export Your App for Self-Hosting
+with docker-compose / Kubernetes (Coming Soon!) ## ðª Support If you
+encounter any problems or have questions, feel free to open an issue on the
+GitHub repository. You can also join our [Discord](https://discord.jina.ai/) to
+get help from our community members and the Jina team. ## ð Our Cloud
+Platform `cloud.jina.ai` is our robust and scalable cloud platform designed to
+run your FastAPI applications with minimum hassle and maximum efficiency. With
+features like auto-scaling, integrated observability, and automated
+containerization, it provides a seamless and worry-free deployment experience.
+--- `fastapi-serve` is more than just a deployment tool, it's a bridge that
+connects your local development environment with our powerful cloud
+infrastructure. Start using `fastapi-serve` today, and experience the joy of
+effortless deployments! ð
```

### Comparing `fastapi-serve-0.0.4.dev4/fastapi_serve.egg-info/SOURCES.txt` & `fastapi-serve-0.0.4.dev5/fastapi_serve.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.4.dev4/setup.py` & `fastapi-serve-0.0.4.dev5/setup.py`

 * *Files identical despite different names*

