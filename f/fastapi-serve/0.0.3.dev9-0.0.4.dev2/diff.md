# Comparing `tmp/fastapi-serve-0.0.3.dev9.tar.gz` & `tmp/fastapi-serve-0.0.4.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-serve-0.0.3.dev9.tar", last modified: Tue Jul 18 05:55:59 2023, max compression
+gzip compressed data, was "fastapi-serve-0.0.4.dev2.tar", last modified: Wed Jul 19 05:27:44 2023, max compression
```

## Comparing `fastapi-serve-0.0.3.dev9.tar` & `fastapi-serve-0.0.4.dev2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:55:59.619735 fastapi-serve-0.0.3.dev9/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-18 05:55:55.000000 fastapi-serve-0.0.3.dev9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-18 05:55:55.000000 fastapi-serve-0.0.3.dev9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-07-18 05:55:59.619735 fastapi-serve-0.0.3.dev9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-07-18 05:55:55.000000 fastapi-serve-0.0.3.dev9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:55:59.615735 fastapi-serve-0.0.3.dev9/fastapi_serve/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-18 05:55:59.000000 fastapi-serve-0.0.3.dev9/fastapi_serve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-18 05:55:55.000000 fastapi-serve-0.0.3.dev9/fastapi_serve/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:55:59.615735 fastapi-serve-0.0.3.dev9/fastapi_serve/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-18 05:55:55.000000 fastapi-serve-0.0.3.dev9/fastapi_serve/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-07-18 05:55:55.000000 fastapi-serve-0.0.3.dev9/fastapi_serve/cloud/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     8001 2023-07-18 05:55:55.000000 fastapi-serve-0.0.3.dev9/fastapi_serve/cloud/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-07-18 05:55:55.000000 fastapi-serve-0.0.3.dev9/fastapi_serve/cloud/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-18 05:55:55.000000 fastapi-serve-0.0.3.dev9/fastapi_serve/cloud/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-18 05:55:55.000000 fastapi-serve-0.0.3.dev9/fastapi_serve/cloud/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-07-18 05:55:55.000000 fastapi-serve-0.0.3.dev9/fastapi_serve/cloud/options.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-18 05:55:55.000000 fastapi-serve-0.0.3.dev9/fastapi_serve/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:55:59.615735 fastapi-serve-0.0.3.dev9/fastapi_serve/gateway/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-18 05:55:55.000000 fastapi-serve-0.0.3.dev9/fastapi_serve/gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-07-18 05:55:55.000000 fastapi-serve-0.0.3.dev9/fastapi_serve/gateway/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-07-18 05:55:55.000000 fastapi-serve-0.0.3.dev9/fastapi_serve/gateway/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-07-18 05:55:55.000000 fastapi-serve-0.0.3.dev9/fastapi_serve/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:55:59.615735 fastapi-serve-0.0.3.dev9/fastapi_serve/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-18 05:55:55.000000 fastapi-serve-0.0.3.dev9/fastapi_serve/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-18 05:55:55.000000 fastapi-serve-0.0.3.dev9/fastapi_serve/utils/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:55:59.619735 fastapi-serve-0.0.3.dev9/fastapi_serve/utils/blob/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-18 05:55:55.000000 fastapi-serve-0.0.3.dev9/fastapi_serve/utils/blob/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-07-18 05:55:55.000000 fastapi-serve-0.0.3.dev9/fastapi_serve/utils/blob/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-18 05:55:55.000000 fastapi-serve-0.0.3.dev9/fastapi_serve/utils/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:55:59.615735 fastapi-serve-0.0.3.dev9/fastapi_serve.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-07-18 05:55:59.000000 fastapi-serve-0.0.3.dev9/fastapi_serve.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-18 05:55:59.000000 fastapi-serve-0.0.3.dev9/fastapi_serve.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 05:55:59.000000 fastapi-serve-0.0.3.dev9/fastapi_serve.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-18 05:55:59.000000 fastapi-serve-0.0.3.dev9/fastapi_serve.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 05:55:59.000000 fastapi-serve-0.0.3.dev9/fastapi_serve.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-18 05:55:59.000000 fastapi-serve-0.0.3.dev9/fastapi_serve.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-18 05:55:59.000000 fastapi-serve-0.0.3.dev9/fastapi_serve.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-18 05:55:55.000000 fastapi-serve-0.0.3.dev9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 05:55:59.619735 fastapi-serve-0.0.3.dev9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-18 05:55:55.000000 fastapi-serve-0.0.3.dev9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:27:44.259667 fastapi-serve-0.0.4.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-19 05:27:39.000000 fastapi-serve-0.0.4.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-19 05:27:39.000000 fastapi-serve-0.0.4.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-07-19 05:27:44.259667 fastapi-serve-0.0.4.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-07-19 05:27:39.000000 fastapi-serve-0.0.4.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:27:44.259667 fastapi-serve-0.0.4.dev2/fastapi_serve/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-19 05:27:43.000000 fastapi-serve-0.0.4.dev2/fastapi_serve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-19 05:27:39.000000 fastapi-serve-0.0.4.dev2/fastapi_serve/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:27:44.259667 fastapi-serve-0.0.4.dev2/fastapi_serve/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-19 05:27:39.000000 fastapi-serve-0.0.4.dev2/fastapi_serve/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8787 2023-07-19 05:27:39.000000 fastapi-serve-0.0.4.dev2/fastapi_serve/cloud/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7902 2023-07-19 05:27:39.000000 fastapi-serve-0.0.4.dev2/fastapi_serve/cloud/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-07-19 05:27:39.000000 fastapi-serve-0.0.4.dev2/fastapi_serve/cloud/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-19 05:27:39.000000 fastapi-serve-0.0.4.dev2/fastapi_serve/cloud/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-19 05:27:39.000000 fastapi-serve-0.0.4.dev2/fastapi_serve/cloud/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-07-19 05:27:39.000000 fastapi-serve-0.0.4.dev2/fastapi_serve/cloud/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-19 05:27:39.000000 fastapi-serve-0.0.4.dev2/fastapi_serve/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:27:44.259667 fastapi-serve-0.0.4.dev2/fastapi_serve/gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-19 05:27:39.000000 fastapi-serve-0.0.4.dev2/fastapi_serve/gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-07-19 05:27:39.000000 fastapi-serve-0.0.4.dev2/fastapi_serve/gateway/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-07-19 05:27:39.000000 fastapi-serve-0.0.4.dev2/fastapi_serve/gateway/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-07-19 05:27:39.000000 fastapi-serve-0.0.4.dev2/fastapi_serve/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:27:44.259667 fastapi-serve-0.0.4.dev2/fastapi_serve/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-19 05:27:39.000000 fastapi-serve-0.0.4.dev2/fastapi_serve/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-19 05:27:39.000000 fastapi-serve-0.0.4.dev2/fastapi_serve/utils/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:27:44.259667 fastapi-serve-0.0.4.dev2/fastapi_serve/utils/blob/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-19 05:27:39.000000 fastapi-serve-0.0.4.dev2/fastapi_serve/utils/blob/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-07-19 05:27:39.000000 fastapi-serve-0.0.4.dev2/fastapi_serve/utils/blob/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-19 05:27:39.000000 fastapi-serve-0.0.4.dev2/fastapi_serve/utils/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 05:27:44.259667 fastapi-serve-0.0.4.dev2/fastapi_serve.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-07-19 05:27:44.000000 fastapi-serve-0.0.4.dev2/fastapi_serve.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-19 05:27:44.000000 fastapi-serve-0.0.4.dev2/fastapi_serve.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 05:27:44.000000 fastapi-serve-0.0.4.dev2/fastapi_serve.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-19 05:27:44.000000 fastapi-serve-0.0.4.dev2/fastapi_serve.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 05:27:44.000000 fastapi-serve-0.0.4.dev2/fastapi_serve.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-19 05:27:44.000000 fastapi-serve-0.0.4.dev2/fastapi_serve.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-19 05:27:44.000000 fastapi-serve-0.0.4.dev2/fastapi_serve.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-19 05:27:39.000000 fastapi-serve-0.0.4.dev2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 05:27:44.259667 fastapi-serve-0.0.4.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-19 05:27:39.000000 fastapi-serve-0.0.4.dev2/setup.py
```

### Comparing `fastapi-serve-0.0.3.dev9/LICENSE` & `fastapi-serve-0.0.4.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.3.dev9/README.md` & `fastapi-serve-0.0.4.dev2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -39,48 +39,41 @@
 fastapi-serve deploy jcloud app:app
 ```
 
 You'll get a URL to access your newly deployed application along with the Swagger UI.
 
 ## 📚 Documentation
 
-We have a few examples to help you get acquainted with `fastapi-serve`:
+Dive into understanding `fastapi-serve` through our comprehensive documentation and examples:
 
-- 🚀 [Deploy a Simple FastAPI Application](docs/simple/)
-- 💹 Auto-scaling endpoints based on RPS, CPU, and Memory (Coming Soon!)
-- 🗝️ [Use Secrets for Redis-Powered Rate Limiting](docs/rate_limit/)
-- 🔒 [Secure Your Endpoints with built-in OAuth2.0 Authorization](docs/authorization/)
-- 📁 [Handle File Uploads and Downloads with built-in Blob Storage](docs/file_handling/)
-- 🐳 Deployment with Custom Dockerfile (Coming Soon!)
-- 🛠️ Export Your App for Self-Hosting with docker-compose / Kubernetes (Coming Soon!)
+- 🚀 **Getting Started**
+    - 🧱 [Deploy a Simple FastAPI Application](docs/simple/)
+    - 🖥️ [Dig deep into the `fastapi-serve` CLI](docs/CLI.md)
+    - ⚙️ [Understanding Configuration and Pricing](docs/CONFIG.MD)
+- ↕️ **Scaling**
+    - 💹 [**Auto-scaling** endpoints based on CPU usage](docs/autoscaling/cpu/)
+    - 📉 **Serverless** (scale-to-zero) deployments based on requests-per-second (Example TBD!) 
+- 🧩 **Config & Credentials**
+    - 🌍 Leverage **Environment Variables** for app configuration (Example TBD!)
+    - 🗝️ [Use **Secrets** for Redis-Powered Rate Limiting](docs/rate_limit/)
+- 💾 **Storage**
+    - 📁 [Handle File Uploads and Downloads with built-in **Blob Storage**](docs/file_handling/)
+    - 🌐 Network Storage for persisting and securely accessing app data (Example TBD!)
+- 🔒 **Security**
+    - 👮‍♂️ [Secure Your Endpoints with built-in **OAuth2.0 Authorization**](docs/authorization/)
+- 🐳 **Deployment Options**
+    - 🚢 Deployment with **Custom Dockerfile** (Coming Soon!)
+    - 🛠️ Export Your App for **Self-Hosting** with docker-compose / Kubernetes (Coming Soon!)
 
 
-## 🖥️ `fastapi-serve` CLI 
-
-`fastapi-serve` comes with a simple CLI that allows you to deploy your FastAPI applications to the cloud with ease.
-
-| Description | Command | 
-| --- | ---: |
-| Deploy your app locally | `fastapi-serve deploy local app:app` |
-| Deploy your app on JCloud | `fastapi-serve deploy jcloud app:app` |
-| Update existing app on JCloud | `fastapi-serve deploy jcloud app:app --app-id <app-id>` |
-| Get app status on JCloud | `fastapi-serve status <app-id>` |
-| List all apps on JCloud | `fastapi-serve list` |
-| Remove app on JCloud | `fastapi-serve remove <app-id>` |
-
-
-## ⚙️💰 Configuration and Pricing
-
-Read our [Configuration & Pricing Guide](examples/CONFIG.MD) to learn more about the various configuration options available to you and the pricing model for `fastapi-serve`.
-
 ## 💪 Support
 
 If you encounter any problems or have questions, feel free to open an issue on the GitHub repository. You can also join our [Discord](https://discord.jina.ai/) to get help from our community members and the Jina team.
 
 
-## Our Cloud Platform 🌐 
+## 🌐 Our Cloud Platform  
 
 `cloud.jina.ai` is our robust and scalable cloud platform designed to run your FastAPI applications with minimum hassle and maximum efficiency. With features like auto-scaling, integrated observability, and automated containerization, it provides a seamless and worry-free deployment experience.
 
 ---
 
 `fastapi-serve` is more than just a deployment tool, it's a bridge that connects your local development environment with our powerful cloud infrastructure. Start using `fastapi-serve` today, and experience the joy of effortless deployments! 🎊
```

#### html2text {}

```diff
@@ -20,37 +20,34 @@
 metrics, and traces. - ð¦ **Containerization**: Effortless containerization
 of your Python codebase with our integrated registry. - ð ï¸ **Self-
 Hosting**: Export your app for self-hosting with ease, including docker-compose
 and Kubernetes yamls. ## ð¡ Getting Started First, install the `fastapi-
 serve` package using pip: ```bash pip install fastapi-serve ``` Then, simply
 use the `fastapi-serve` command to deploy your FastAPI application: ```bash
 fastapi-serve deploy jcloud app:app ``` You'll get a URL to access your newly
-deployed application along with the Swagger UI. ## ð Documentation We have a
-few examples to help you get acquainted with `fastapi-serve`: - ð [Deploy a
-Simple FastAPI Application](docs/simple/) - ð¹ Auto-scaling endpoints based
-on RPS, CPU, and Memory (Coming Soon!) - ðï¸ [Use Secrets for Redis-Powered
-Rate Limiting](docs/rate_limit/) - ð [Secure Your Endpoints with built-in
-OAuth2.0 Authorization](docs/authorization/) - ð [Handle File Uploads and
-Downloads with built-in Blob Storage](docs/file_handling/) - ð³ Deployment
-with Custom Dockerfile (Coming Soon!) - ð ï¸ Export Your App for Self-
-Hosting with docker-compose / Kubernetes (Coming Soon!) ## ð¥ï¸ `fastapi-
-serve` CLI `fastapi-serve` comes with a simple CLI that allows you to deploy
-your FastAPI applications to the cloud with ease. | Description | Command | | -
--- | ---: | | Deploy your app locally | `fastapi-serve deploy local app:app` |
-| Deploy your app on JCloud | `fastapi-serve deploy jcloud app:app` | | Update
-existing app on JCloud | `fastapi-serve deploy jcloud app:app --app-id ` | |
-Get app status on JCloud | `fastapi-serve status ` | | List all apps on JCloud
-| `fastapi-serve list` | | Remove app on JCloud | `fastapi-serve remove ` | ##
-âï¸ð° Configuration and Pricing Read our [Configuration & Pricing Guide]
-(examples/CONFIG.MD) to learn more about the various configuration options
-available to you and the pricing model for `fastapi-serve`. ## ðª Support If
-you encounter any problems or have questions, feel free to open an issue on the
-GitHub repository. You can also join our [Discord](https://discord.jina.ai/) to
-get help from our community members and the Jina team. ## Our Cloud Platform
-ð `cloud.jina.ai` is our robust and scalable cloud platform designed to run
-your FastAPI applications with minimum hassle and maximum efficiency. With
-features like auto-scaling, integrated observability, and automated
-containerization, it provides a seamless and worry-free deployment experience.
---- `fastapi-serve` is more than just a deployment tool, it's a bridge that
-connects your local development environment with our powerful cloud
-infrastructure. Start using `fastapi-serve` today, and experience the joy of
-effortless deployments! ð
+deployed application along with the Swagger UI. ## ð Documentation Dive into
+understanding `fastapi-serve` through our comprehensive documentation and
+examples: - ð **Getting Started** - ð§± [Deploy a Simple FastAPI
+Application](docs/simple/) - ð¥ï¸ [Dig deep into the `fastapi-serve` CLI]
+(docs/CLI.md) - âï¸ [Understanding Configuration and Pricing](docs/
+CONFIG.MD) - âï¸ **Scaling** - ð¹ [**Auto-scaling** endpoints based on CPU
+usage](docs/autoscaling/cpu/) - ð **Serverless** (scale-to-zero) deployments
+based on requests-per-second (Example TBD!) - ð§© **Config & Credentials** -
+ð Leverage **Environment Variables** for app configuration (Example TBD!) -
+ðï¸ [Use **Secrets** for Redis-Powered Rate Limiting](docs/rate_limit/) -
+ð¾ **Storage** - ð [Handle File Uploads and Downloads with built-in **Blob
+Storage**](docs/file_handling/) - ð Network Storage for persisting and
+securely accessing app data (Example TBD!) - ð **Security** - ð®ââï¸
+[Secure Your Endpoints with built-in **OAuth2.0 Authorization**](docs/
+authorization/) - ð³ **Deployment Options** - ð¢ Deployment with **Custom
+Dockerfile** (Coming Soon!) - ð ï¸ Export Your App for **Self-Hosting** with
+docker-compose / Kubernetes (Coming Soon!) ## ðª Support If you encounter any
+problems or have questions, feel free to open an issue on the GitHub
+repository. You can also join our [Discord](https://discord.jina.ai/) to get
+help from our community members and the Jina team. ## ð Our Cloud Platform
+`cloud.jina.ai` is our robust and scalable cloud platform designed to run your
+FastAPI applications with minimum hassle and maximum efficiency. With features
+like auto-scaling, integrated observability, and automated containerization, it
+provides a seamless and worry-free deployment experience. --- `fastapi-serve`
+is more than just a deployment tool, it's a bridge that connects your local
+development environment with our powerful cloud infrastructure. Start using
+`fastapi-serve` today, and experience the joy of effortless deployments! ð
```

### Comparing `fastapi-serve-0.0.3.dev9/fastapi_serve/__main__.py` & `fastapi-serve-0.0.4.dev2/fastapi_serve/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,14 @@
 async def jcloud(
     app,
     app_dir,
     name,
     uses,
     app_id,
     version,
-    timeout,
     platform,
     config,
     cors,
     env,
     secret,
     verbose,
     public,
@@ -77,15 +76,14 @@
     await serve_on_jcloud(
         app=app,
         app_dir=app_dir,
         name=name,
         uses=uses,
         app_id=app_id,
         version=version,
-        timeout=timeout,
         platform=platform,
         config=config,
         cors=cors,
         env=env,
         secret=secret,
         verbose=verbose,
         public=public,
```

### Comparing `fastapi-serve-0.0.3.dev9/fastapi_serve/cloud/build.py` & `fastapi-serve-0.0.4.dev2/fastapi_serve/cloud/build.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.3.dev9/fastapi_serve/cloud/config.py` & `fastapi-serve-0.0.4.dev2/fastapi_serve/cloud/config.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,98 +9,128 @@
     InvalidAutoscaleMaxError,
     InvalidAutoscaleMinError,
     InvalidDiskSizeError,
     InvalidInstanceError,
 )
 
 # jcloud args
-INSTANCE = 'instance'
-AUTOSCALE_MIN = 'autoscale_min'
-AUTOSCALE_MAX = 'autoscale_max'
-DISK_SIZE = 'disk_size'
-
-# config file
-JCloudConfigFile = 'jcloud_config.yml'
+VALID_AUTOSCALE_METRICS = ['cpu', 'memory', 'rps']
 
 # default values
-DEFAULT_TIMEOUT = 120
-DEFAULT_DISK_SIZE = '1G'
-DEFAULT_LABEL = 'fastapi-serve'
 APP_NAME = 'fastapi'
 JINA_VERSION = '3.18.0'
 DOCARRAY_VERSION = '0.21.0'
+DEFAULT_TIMEOUT = 120
+DEFAULT_LABEL = 'fastapi-serve'
+
+# jcloud urls
 APP_LOGS_URL = "[https://cloud.jina.ai/](https://cloud.jina.ai/user/flows?action=detail&id={app_id}&tab=logs)"
 PRICING_URL = "****{cph}**** ([Read about pricing here](https://github.com/jina-ai/langchain-serve#-pricing))"
 
 
 @dataclass
 class Defaults:
-    instance: str = 'C3'
-    autoscale_min: int = 1
-    autoscale_max: int = 10
-    autoscale_rps: int = 10
+    instance: str = 'C3'  # instance type
+    autoscale_min: int = 1  # min number of replicas
+    autoscale_max: int = 10  # max number of replicas
+    autoscale_metric: str = 'cpu'  # cpu, memory, rps
+    autoscale_cpu_target: int = 70  # 70% cpu usage
+    autoscale_rps_target: int = 10  # 10 requests per second
     autoscale_stable_window: int = DEFAULT_TIMEOUT
     autoscale_revision_timeout: int = DEFAULT_TIMEOUT
-    disk_size: str = DEFAULT_DISK_SIZE
-
-    def __post_init__(self):
-        _path = os.path.join(os.getcwd(), JCloudConfigFile)
-        if os.path.exists(_path):
-            # read from config yaml
-            with open(_path, 'r') as fp:
-                config = yaml.safe_load(fp.read())
-                self.instance = config.get('instance', self.instance)
-                self.autoscale_min = config.get('autoscale', {}).get(
-                    'min', self.autoscale_min
-                )
-                self.autoscale_max = config.get('autoscale', {}).get(
-                    'max', self.autoscale_max
-                )
-                self.autoscale_rps = config.get('autoscale', {}).get(
-                    'rps', self.autoscale_rps
-                )
-                self.autoscale_stable_window = config.get('autoscale', {}).get(
-                    'stable_window', self.autoscale_stable_window
-                )
-                self.autoscale_revision_timeout = config.get('autoscale', {}).get(
-                    'revision_timeout', self.autoscale_revision_timeout
-                )
-                self.disk_size = config.get('disk_size', self.disk_size)
+    disk_size: str = '1G'
 
 
 @dataclass
 class AutoscaleConfig:
     min: int = Defaults.autoscale_min
     max: int = Defaults.autoscale_max
-    rps: int = Defaults.autoscale_rps
+    metric: str = Defaults.autoscale_metric
+    target: int = Defaults.autoscale_cpu_target
     stable_window: int = Defaults.autoscale_stable_window
     revision_timeout: int = Defaults.autoscale_revision_timeout
 
+    def __post_init__(self):
+        try:
+            self.min = int(self.min)
+            if self.min < 0:
+                raise InvalidAutoscaleMinError(self.min)
+        except ValueError:
+            raise InvalidAutoscaleMinError(self.min)
+
+        try:
+            self.max = int(self.max)
+            if self.max < 1:
+                raise InvalidAutoscaleMaxError(self.max)
+        except ValueError:
+            raise InvalidAutoscaleMaxError(self.max)
+
+        if self.min > self.max:
+            raise InvalidAutoscaleMaxError(self.max)
+
+        if self.target < 1:
+            raise ValueError(
+                f'Invalid autoscale target {self.target}. Must be greater than 1'
+            )
+
+        if self.metric not in VALID_AUTOSCALE_METRICS:
+            raise ValueError(
+                f'Invalid autoscale metric {self.metric}. Valid options are {VALID_AUTOSCALE_METRICS}'
+            )
+
+        if self.metric in ['cpu', 'memory'] and self.min == 0:
+            print(f'Cannot autoscale to 0 for {self.metric}. Resetting it to 1')
+            self.min = 1
+
     def to_dict(self) -> Dict:
         return {
             'autoscale': {
                 'min': self.min,
                 'max': self.max,
-                'metric': 'rps',
-                'target': self.rps,
+                'metric': self.metric,
+                'target': self.target,
                 'stable_window': self.stable_window,
                 'revision_timeout': self.revision_timeout,
             }
         }
 
+    @classmethod
+    def from_dict(cls, config: Dict):
+        _autoscale = config.get('autoscale', {})
+        return cls(
+            min=_autoscale.get('min', cls.min),
+            max=_autoscale.get('max', cls.max),
+            metric=_autoscale.get('metric', cls.metric),
+            target=_autoscale.get('target', cls.target),
+        )
+
 
 @dataclass
 class JCloudConfig:
-    is_websocket: bool
     timeout: int = DEFAULT_TIMEOUT
     instance: str = Defaults.instance
     disk_size: str = Defaults.disk_size
     autoscale: AutoscaleConfig = field(init=False)
 
     def __post_init__(self):
+        if self.instance and not (
+            self.instance.startswith(("C", "G")) and self.instance[1:].isdigit()
+        ):
+            raise InvalidInstanceError(self.instance)
+
+        if self.disk_size is not None:
+            if (
+                isinstance(self.disk_size, str)
+                and not self.disk_size.endswith(("M", "MB", "Mi", "G", "GB", "Gi"))
+            ) or (isinstance(self.disk_size, int) and self.disk_size != 0):
+                raise InvalidDiskSizeError(self.disk_size)
+
+        if self.timeout < 1:
+            raise ValueError(f'Invalid timeout {self.timeout}. Must be greater than 1')
+
         self.autoscale = AutoscaleConfig(
             stable_window=self.timeout, revision_timeout=self.timeout
         )
 
     def to_dict(self) -> Dict:
         jcloud_dict = {
             'jcloud': {
@@ -120,57 +150,49 @@
             jcloud_dict['jcloud']['resources']['storage'] = {
                 'kind': 'efs',
                 'size': self.disk_size,
             }
 
         return jcloud_dict
 
+    @classmethod
+    def from_dict(cls, config: Dict):
+        '''Sample config
+        {
+            "instance": "C3",
+            "timeout": 120,
+            "autoscale": {
+                "min": 1,
+                "max": 10,
+                "metric": "cpu",
+                "target": 70,
+            },
+            "disk_size": "1G"
+        }
+        '''
+        jcloud_config = cls(
+            instance=config.get('instance', cls.instance),
+            disk_size=config.get('disk_size', cls.disk_size),
+            timeout=config.get('timeout', cls.timeout),
+        )
+        jcloud_config.autoscale = AutoscaleConfig.from_dict(config)
+        return jcloud_config
 
-def validate_jcloud_config(config_path):
-    with open(config_path, "r") as f:
-        config_data: Dict = yaml.safe_load(f)
-        instance: str = config_data.get(INSTANCE)
-        autoscale_min: str = config_data.get(AUTOSCALE_MIN)
-        autoscale_max: str = config_data.get(AUTOSCALE_MAX)
-        disk_size: str = config_data.get(DISK_SIZE)
-
-        if instance and not (
-            instance.startswith(("C", "G")) and instance[1:].isdigit()
-        ):
-            raise InvalidInstanceError(instance)
-
-        if autoscale_min:
-            try:
-                autoscale_min_int = int(autoscale_min)
-                if autoscale_min_int < 0:
-                    raise InvalidAutoscaleMinError(autoscale_min)
-            except ValueError:
-                raise InvalidAutoscaleMinError(autoscale_min)
-
-        if autoscale_max:
-            try:
-                autoscale_max_int = int(autoscale_max)
-                if autoscale_max_int < 0:
-                    raise InvalidAutoscaleMaxError(autoscale_max)
-            except ValueError:
-                raise InvalidAutoscaleMaxError(autoscale_max)
-
-        if disk_size is not None:
-            if (
-                isinstance(disk_size, str)
-                and not disk_size.endswith(("M", "MB", "Mi", "G", "GB", "Gi"))
-            ) or (isinstance(disk_size, int) and disk_size != 0):
-                raise InvalidDiskSizeError(disk_size)
+    @classmethod
+    def from_file(cls, config_path: str):
+        with open(config_path, "r") as f:
+            config_data: Dict = yaml.safe_load(f)
+            return cls.from_dict(config_data)
 
 
 def validate_jcloud_config_callback(ctx, param, value):
     if not value:
         return None
     try:
-        validate_jcloud_config(value)
+        JCloudConfig.from_file(value)
     except InvalidInstanceError as e:
         raise click.BadParameter(
             f"Invalid instance '{e.instance}' found in config file', please refer to https://docs.jina.ai/concepts/jcloud/configuration/#cpu-tiers for instance definition."
         )
     except InvalidAutoscaleMinError as e:
         raise click.BadParameter(
             f"Invalid instance '{e.min}' found in config file', it should be a number >= 0."
@@ -196,47 +218,31 @@
         config_path = config_path_yml
     elif os.path.exists(config_path_yaml):
         config_path = config_path_yaml
     else:
         return None
 
     try:
-        validate_jcloud_config(config_path)
-    except (InvalidAutoscaleMinError, InvalidInstanceError, InvalidDiskSizeError):
+        JCloudConfig.from_file(config_path)
+    except (InvalidAutoscaleMinError, InvalidInstanceError, InvalidDiskSizeError) as e:
         # If it's malformed, we treated as non-existed
+        print(f'config file {config_path} is malformed: {e}')
         return None
 
     print(f'JCloud config file at app directory will be applied: {config_path}')
     return config_path
 
 
-def get_jcloud_config(
-    config_path: str = None, timeout: int = DEFAULT_TIMEOUT, is_websocket: bool = False
-) -> JCloudConfig:
-    jcloud_config = JCloudConfig(is_websocket=is_websocket, timeout=timeout)
+def get_jcloud_config(config_path: str = None) -> JCloudConfig:
     if not config_path:
-        return jcloud_config
+        return JCloudConfig()
 
     if not os.path.exists(config_path):
         print(f'config file {config_path} not found')
-        return jcloud_config
+        return JCloudConfig()
 
     with open(config_path, 'r') as f:
         config_data: Dict = yaml.safe_load(f)
         if not config_data:
-            return jcloud_config
-
-        instance = config_data.get(INSTANCE)
-        autoscale_min = config_data.get(AUTOSCALE_MIN)
-        autoscale_max = config_data.get(AUTOSCALE_MAX)
-        disk_size = config_data.get(DISK_SIZE)
-
-        if instance:
-            jcloud_config.instance = instance
-        if autoscale_min is not None:
-            jcloud_config.autoscale.min = autoscale_min
-        if autoscale_max is not None:
-            jcloud_config.autoscale.max = autoscale_max
-        if disk_size is not None:
-            jcloud_config.disk_size = disk_size
+            return JCloudConfig()
 
-    return jcloud_config
+        return JCloudConfig.from_dict(config_data)
```

### Comparing `fastapi-serve-0.0.3.dev9/fastapi_serve/cloud/deploy.py` & `fastapi-serve-0.0.4.dev2/fastapi_serve/cloud/deploy.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import yaml
 from dotenv import dotenv_values
 
 from fastapi_serve.cloud.config import (
     APP_LOGS_URL,
     APP_NAME,
     DEFAULT_LABEL,
-    DEFAULT_TIMEOUT,
     DOCARRAY_VERSION,
     JINA_VERSION,
     PRICING_URL,
     get_jcloud_config,
 )
 from fastapi_serve.helper import (
     EnvironmentVarCtxtManager,
@@ -95,26 +94,23 @@
 
 
 def get_flow_dict(
     app: str,
     jcloud: bool = False,
     port: int = 8080,
     name: str = APP_NAME,
-    timeout: int = DEFAULT_TIMEOUT,
     app_id: str = None,
     gateway_id: str = None,
     is_websocket: bool = False,
     jcloud_config_path: str = None,
     cors: bool = True,
     env: str = None,
 ) -> Dict:
     if jcloud:
-        jcloud_config = get_jcloud_config(
-            config_path=jcloud_config_path, timeout=timeout, is_websocket=is_websocket
-        )
+        jcloud_config = get_jcloud_config(config_path=jcloud_config_path)
 
     _envs = {}
     if env is not None:
         # read env file and load to _envs dict
         _envs = dict(dotenv_values(env))
 
     # add userid to _envs dict
@@ -348,15 +344,14 @@
 async def serve_on_jcloud(
     app: str,
     app_dir: str = None,
     name: str = APP_NAME,
     uses: str = None,
     app_id: str = None,
     version: str = 'latest',
-    timeout: int = DEFAULT_TIMEOUT,
     platform: str = None,
     config: str = None,
     cors: bool = True,
     env: str = None,
     secret: str = None,  # TODO: add support for secret
     verbose: bool = False,
     public: bool = False,
@@ -385,15 +380,14 @@
 
     # Get the flow dict
     flow_dict = get_flow_dict(
         app=app,
         jcloud=True,
         port=8080,
         name=name,
-        timeout=timeout,
         app_id=app_id,
         gateway_id=gateway_id,
         is_websocket=is_websocket,
         jcloud_config_path=config,
         cors=cors,
         env=env,
     )
```

### Comparing `fastapi-serve-0.0.3.dev9/fastapi_serve/cloud/errors.py` & `fastapi-serve-0.0.4.dev2/fastapi_serve/cloud/errors.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.3.dev9/fastapi_serve/cloud/options.py` & `fastapi-serve-0.0.4.dev2/fastapi_serve/cloud/options.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 import click
 from jcloud.constants import Phase
 
-from fastapi_serve.cloud.config import (
-    APP_NAME,
-    DEFAULT_TIMEOUT,
-    validate_jcloud_config_callback,
-)
+from fastapi_serve.cloud.config import APP_NAME, validate_jcloud_config_callback
 
 _help_option = [click.help_option('-h', '--help')]
 
 _common_options = [
     click.argument(
         'app',
         type=str,
@@ -86,21 +82,14 @@
     click.option(
         '--app-id',
         type=str,
         default=None,
         help='AppID of the deployed app to be updated.',
     ),
     click.option(
-        '--timeout',
-        type=int,
-        default=DEFAULT_TIMEOUT,
-        help='Total request timeout in seconds.',
-        show_default=True,
-    ),
-    click.option(
         '--config',
         type=click.Path(exists=True),
         help='Path to the config file',
         callback=validate_jcloud_config_callback,
         show_default=False,
     ),
     click.option(
```

### Comparing `fastapi-serve-0.0.3.dev9/fastapi_serve/gateway/gateway.py` & `fastapi-serve-0.0.4.dev2/fastapi_serve/gateway/gateway.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.3.dev9/fastapi_serve/gateway/helper.py` & `fastapi-serve-0.0.4.dev2/fastapi_serve/gateway/helper.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.3.dev9/fastapi_serve/helper.py` & `fastapi-serve-0.0.4.dev2/fastapi_serve/helper.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.3.dev9/fastapi_serve/utils/auth.py` & `fastapi-serve-0.0.4.dev2/fastapi_serve/utils/auth.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.3.dev9/fastapi_serve/utils/blob/storage.py` & `fastapi-serve-0.0.4.dev2/fastapi_serve/utils/blob/storage.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.3.dev9/fastapi_serve/utils/helper.py` & `fastapi-serve-0.0.4.dev2/fastapi_serve/utils/helper.py`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.3.dev9/fastapi_serve.egg-info/SOURCES.txt` & `fastapi-serve-0.0.4.dev2/fastapi_serve.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastapi-serve-0.0.3.dev9/setup.py` & `fastapi-serve-0.0.4.dev2/setup.py`

 * *Files identical despite different names*

