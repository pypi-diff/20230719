# Comparing `tmp/sardine-web-1.0.0.tar.gz` & `tmp/sardine-web-1.0.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sardine-web-1.0.0.tar", last modified: Tue Jul 18 21:55:36 2023, max compression
+gzip compressed data, was "sardine-web-1.0.0.post1.tar", last modified: Tue Jul 18 23:11:21 2023, max compression
```

## Comparing `sardine-web-1.0.0.tar` & `sardine-web-1.0.0.post1.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:55:36.302252 sardine-web-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35150 2023-07-18 21:55:22.000000 sardine-web-1.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-18 21:55:22.000000 sardine-web-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-18 21:55:36.302252 sardine-web-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-18 21:55:22.000000 sardine-web-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-18 21:55:22.000000 sardine-web-1.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:55:36.286251 sardine-web-1.0.0/sardine_web/
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:55:36.290251 sardine-web-1.0.0/sardine_web/client/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:55:36.286251 sardine-web-1.0.0/sardine_web/client/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:55:36.290251 sardine-web-1.0.0/sardine_web/client/assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)   113421 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/client/assets/css/fontawesome.css
--rw-r--r--   0 runner    (1001) docker     (123)    80823 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/client/assets/css/fontawesome.min.css
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/client/assets/css/solid.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:55:36.290251 sardine-web-1.0.0/sardine_web/client/assets/webfonts/
--rw-r--r--   0 runner    (1001) docker     (123)   187208 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/client/assets/webfonts/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   108020 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/client/assets/webfonts/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    63952 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/client/assets/webfonts/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    24948 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/client/assets/webfonts/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   394628 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/client/assets/webfonts/fa-solid-900.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   150124 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/client/assets/webfonts/fa-solid-900.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/client/assets/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/client/assets/webfonts/fa-v4compatibility.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:55:36.286251 sardine-web-1.0.0/sardine_web/client/fonts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:55:36.294251 sardine-web-1.0.0/sardine_web/client/fonts/Droid/
--rw-r--r--   0 runner    (1001) docker     (123)    18968 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/client/fonts/Droid/DroidSansMono-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/client/fonts/Droid/stylesheet.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:55:36.294251 sardine-web-1.0.0/sardine_web/client/fonts/Fira/
--rw-r--r--   0 runner    (1001) docker     (123)   188876 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/client/fonts/Fira/FiraCode-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   188468 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/client/fonts/Fira/FiraCode-Light.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   188244 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/client/fonts/Fira/FiraCode-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   188252 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/client/fonts/Fira/FiraCode-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   188604 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/client/fonts/Fira/FiraCode-SemiBold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/client/fonts/Fira/stylesheet.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:55:36.298251 sardine-web-1.0.0/sardine_web/client/fonts/JGSfont/
--rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/client/fonts/JGSfont/jgs5.woff
--rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/client/fonts/JGSfont/jgs5.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     9968 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/client/fonts/JGSfont/jgs7.woff
--rw-r--r--   0 runner    (1001) docker     (123)     6820 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/client/fonts/JGSfont/jgs7.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     8940 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/client/fonts/JGSfont/jgs9.woff
--rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/client/fonts/JGSfont/jgs9.woff2
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/client/fonts/JGSfont/stylesheet.css
--rw-r--r--   0 runner    (1001) docker     (123)  1605860 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/client/fonts/JGSfont/unifont-12.0.01.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   283288 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/client/fonts/JGSfont/unifont_upper-12.0.01.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:55:36.298251 sardine-web-1.0.0/sardine_web/client/fonts/SpaceMono/
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/client/fonts/SpaceMono/OFL.txt
--rw-r--r--   0 runner    (1001) docker     (123)    86636 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/client/fonts/SpaceMono/SpaceMono-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    95292 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/client/fonts/SpaceMono/SpaceMono-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   103524 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/client/fonts/SpaceMono/SpaceMono-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    90904 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/client/fonts/SpaceMono/SpaceMono-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/client/fonts/SpaceMono/stylesheet.css
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/client/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    45086 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/client/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/client/package.json
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/client/postcss.config.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:55:36.302252 sardine-web-1.0.0/sardine_web/client/src/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/client/src/AppSettings.ts
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/client/src/Editor.ts
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/client/src/EditorSetup.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/client/src/RunnerService.ts
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/client/src/counter.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:55:36.302252 sardine-web-1.0.0/sardine_web/client/src/help/
--rw-r--r--   0 runner    (1001) docker     (123)    13348 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/client/src/help/generalHelp.ts
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/client/src/help/keybindingsHelp.ts
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/client/src/highlightSelection.ts
--rw-r--r--   0 runner    (1001) docker     (123)    14437 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/client/src/main.ts
--rw-r--r--   0 runner    (1001) docker     (123)    14136 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/client/src/output.css
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/client/src/style copy.css
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/client/src/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:55:36.302252 sardine-web-1.0.0/sardine_web/client/src/themes/
--rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/client/src/themes/sardineTheme.ts
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/client/src/vite-env.d.ts
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/client/tailwind.config.js
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/client/tsconfig.json
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/client/vite.config.ts
--rw-r--r--   0 runner    (1001) docker     (123)    58844 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/client/yarn.lock
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:55:36.302252 sardine-web-1.0.0/sardine_web/server/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8621 2023-07-18 21:55:22.000000 sardine-web-1.0.0/sardine_web/server/flask_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:55:36.286251 sardine-web-1.0.0/sardine_web.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-18 21:55:36.000000 sardine-web-1.0.0/sardine_web.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-07-18 21:55:36.000000 sardine-web-1.0.0/sardine_web.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 21:55:36.000000 sardine-web-1.0.0/sardine_web.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-18 21:55:36.000000 sardine-web-1.0.0/sardine_web.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-18 21:55:36.000000 sardine-web-1.0.0/sardine_web.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-18 21:55:36.000000 sardine-web-1.0.0/sardine_web.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 21:55:36.302252 sardine-web-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-07-18 21:55:22.000000 sardine-web-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:11:21.568925 sardine-web-1.0.0.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35150 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-07-18 23:11:21.564925 sardine-web-1.0.0.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:11:21.552925 sardine-web-1.0.0.post1/sardine_web/
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:11:21.556925 sardine-web-1.0.0.post1/sardine_web/client/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:11:21.552925 sardine-web-1.0.0.post1/sardine_web/client/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:11:21.556925 sardine-web-1.0.0.post1/sardine_web/client/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   113421 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/assets/css/fontawesome.css
+-rw-r--r--   0 runner    (1001) docker     (123)    80823 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/assets/css/fontawesome.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/assets/css/solid.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:11:21.556925 sardine-web-1.0.0.post1/sardine_web/client/assets/webfonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   187208 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/assets/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   108020 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/assets/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    63952 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/assets/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    24948 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/assets/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   394628 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/assets/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   150124 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/assets/webfonts/fa-solid-900.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/assets/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/assets/webfonts/fa-v4compatibility.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:11:21.552925 sardine-web-1.0.0.post1/sardine_web/client/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:11:21.560925 sardine-web-1.0.0.post1/sardine_web/client/fonts/Droid/
+-rw-r--r--   0 runner    (1001) docker     (123)    18968 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/fonts/Droid/DroidSansMono-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/fonts/Droid/stylesheet.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:11:21.560925 sardine-web-1.0.0.post1/sardine_web/client/fonts/Fira/
+-rw-r--r--   0 runner    (1001) docker     (123)   188876 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/fonts/Fira/FiraCode-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   188468 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/fonts/Fira/FiraCode-Light.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   188244 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/fonts/Fira/FiraCode-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   188252 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/fonts/Fira/FiraCode-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   188604 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/fonts/Fira/FiraCode-SemiBold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/fonts/Fira/stylesheet.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:11:21.564925 sardine-web-1.0.0.post1/sardine_web/client/fonts/JGSfont/
+-rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/fonts/JGSfont/jgs5.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/fonts/JGSfont/jgs5.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     9968 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/fonts/JGSfont/jgs7.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     6820 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/fonts/JGSfont/jgs7.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     8940 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/fonts/JGSfont/jgs9.woff
+-rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/fonts/JGSfont/jgs9.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/fonts/JGSfont/stylesheet.css
+-rw-r--r--   0 runner    (1001) docker     (123)  1605860 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/fonts/JGSfont/unifont-12.0.01.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   283288 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/fonts/JGSfont/unifont_upper-12.0.01.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:11:21.564925 sardine-web-1.0.0.post1/sardine_web/client/fonts/SpaceMono/
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/fonts/SpaceMono/OFL.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    86636 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/fonts/SpaceMono/SpaceMono-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    95292 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/fonts/SpaceMono/SpaceMono-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   103524 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/fonts/SpaceMono/SpaceMono-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    90904 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/fonts/SpaceMono/SpaceMono-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/fonts/SpaceMono/stylesheet.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    45086 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/postcss.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:11:21.564925 sardine-web-1.0.0.post1/sardine_web/client/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/src/AppSettings.ts
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/src/Editor.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/src/EditorSetup.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/src/RunnerService.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/src/counter.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:11:21.564925 sardine-web-1.0.0.post1/sardine_web/client/src/help/
+-rw-r--r--   0 runner    (1001) docker     (123)    13348 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/src/help/generalHelp.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/src/help/keybindingsHelp.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/src/highlightSelection.ts
+-rw-r--r--   0 runner    (1001) docker     (123)    14437 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/src/main.ts
+-rw-r--r--   0 runner    (1001) docker     (123)    14136 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/src/output.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/src/style copy.css
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/src/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:11:21.564925 sardine-web-1.0.0.post1/sardine_web/client/src/themes/
+-rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/src/themes/sardineTheme.ts
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/src/vite-env.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/tailwind.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/tsconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/vite.config.ts
+-rw-r--r--   0 runner    (1001) docker     (123)    58844 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/client/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:11:21.564925 sardine-web-1.0.0.post1/sardine_web/server/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8621 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/sardine_web/server/flask_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 23:11:21.556925 sardine-web-1.0.0.post1/sardine_web.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-07-18 23:11:21.000000 sardine-web-1.0.0.post1/sardine_web.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-07-18 23:11:21.000000 sardine-web-1.0.0.post1/sardine_web.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 23:11:21.000000 sardine-web-1.0.0.post1/sardine_web.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-18 23:11:21.000000 sardine-web-1.0.0.post1/sardine_web.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-18 23:11:21.000000 sardine-web-1.0.0.post1/sardine_web.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-18 23:11:21.000000 sardine-web-1.0.0.post1/sardine_web.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 23:11:21.568925 sardine-web-1.0.0.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-07-18 23:11:09.000000 sardine-web-1.0.0.post1/setup.py
```

### Comparing `sardine-web-1.0.0/LICENSE.txt` & `sardine-web-1.0.0.post1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0/PKG-INFO` & `sardine-web-1.0.0.post1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sardine-web
-Version: 1.0.0
+Version: 1.0.0.post1
 Summary: Official web editor plugin for sardine-system
 Author: Raphaël Forment, thegamecracks
 Author-email: raphael.forment@gmail.com
 License: GPL-3.0-only
 Project-URL: Homepage, https://sardine.raphaelforment.fr
 Project-URL: Documentation, https://sardine.raphaelforment.fr
 Project-URL: Source Code, https://github.com/sardine-system/sardine-web
@@ -31,29 +31,41 @@
 
 # sardine-web
 
 The official web editor plugin for the [sardine-system] library!
 
 ## Installation
 
-The main repository has not yet merged CLI plugin support into the main repo.
-First follow the [installation guide] in the documentation, then install Sardine
-on the sardine-web-plugin branch like so:
+If you already have sardine-system v0.4.0+ installed or you are fine with
+the stable version of Sardine, you can go straight to installing
+this package from [PyPI]:
 
 ```sh
-# From remote:
-pip install "git+https://github.com/Bubobubobubobubo/sardine@sardine-web-plugin"
-# Or from local clone which is set to the sardine-web-plugin branch:
-pip install -e <PATH_TO_REPO>
+pip install sardine-web
 ```
 
-With Node.js / Yarn installed as per the guide, you can then install this package:
+If you do want the Sardine development version, install the repository before
+this package following their [installation guide]:
+
+```sh
+pip install git+https://github.com/Bubobubobubobubo/sardine
+pip install sardine-web
+```
+
+If you want to install the development version of *this* repository,
+make sure you have [Node.js] and [Yarn] installed:
 
 ```sh
-# From remote:
 pip install git+https://github.com/sardine-system/sardine-web
-# Or from local clone in current working directory:
-pip install -e .[dev]
 ```
 
+## Usage
+
+Documentation: https://sardine.raphaelforment.fr/editors/fishery.html
+
+This adds a `sardine web` command to Sardine to start the web editor.
+
 [sardine-system]: https://github.com/Bubobubobubobubo/sardine
+[PyPI]: https://pypi.org/project/sardine-web/
 [installation guide]: https://sardine.raphaelforment.fr/installation.html
+[Node.js]: https://nodejs.org/
+[Yarn]: https://yarnpkg.com/
```

### Comparing `sardine-web-1.0.0/pyproject.toml` & `sardine-web-1.0.0.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0/sardine_web/__init__.py` & `sardine-web-1.0.0.post1/sardine_web/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import click
 
-__version__ = "1.0.0"
+__version__ = "1.0.0.post1"
 
 
 def install_web(main: click.Group):
     from sardine.console import ConsoleManager
 
     @main.command(
         short_help="Starts sardine as a web server",
```

### Comparing `sardine-web-1.0.0/sardine_web/client/assets/css/fontawesome.css` & `sardine-web-1.0.0.post1/sardine_web/client/assets/css/fontawesome.css`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0/sardine_web/client/assets/css/fontawesome.min.css` & `sardine-web-1.0.0.post1/sardine_web/client/assets/css/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0/sardine_web/client/assets/css/solid.css` & `sardine-web-1.0.0.post1/sardine_web/client/assets/css/solid.css`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0/sardine_web/client/assets/webfonts/fa-brands-400.ttf` & `sardine-web-1.0.0.post1/sardine_web/client/assets/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0/sardine_web/client/assets/webfonts/fa-brands-400.woff2` & `sardine-web-1.0.0.post1/sardine_web/client/assets/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0/sardine_web/client/assets/webfonts/fa-regular-400.ttf` & `sardine-web-1.0.0.post1/sardine_web/client/assets/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0/sardine_web/client/assets/webfonts/fa-regular-400.woff2` & `sardine-web-1.0.0.post1/sardine_web/client/assets/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0/sardine_web/client/assets/webfonts/fa-solid-900.ttf` & `sardine-web-1.0.0.post1/sardine_web/client/assets/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0/sardine_web/client/assets/webfonts/fa-solid-900.woff2` & `sardine-web-1.0.0.post1/sardine_web/client/assets/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0/sardine_web/client/assets/webfonts/fa-v4compatibility.ttf` & `sardine-web-1.0.0.post1/sardine_web/client/assets/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0/sardine_web/client/assets/webfonts/fa-v4compatibility.woff2` & `sardine-web-1.0.0.post1/sardine_web/client/assets/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0/sardine_web/client/fonts/Droid/DroidSansMono-webfont.woff` & `sardine-web-1.0.0.post1/sardine_web/client/fonts/Droid/DroidSansMono-webfont.woff`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0/sardine_web/client/fonts/Fira/FiraCode-Bold.ttf` & `sardine-web-1.0.0.post1/sardine_web/client/fonts/Fira/FiraCode-Bold.ttf`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0/sardine_web/client/fonts/Fira/FiraCode-Light.ttf` & `sardine-web-1.0.0.post1/sardine_web/client/fonts/Fira/FiraCode-Light.ttf`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0/sardine_web/client/fonts/Fira/FiraCode-Medium.ttf` & `sardine-web-1.0.0.post1/sardine_web/client/fonts/Fira/FiraCode-Medium.ttf`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0/sardine_web/client/fonts/Fira/FiraCode-Regular.ttf` & `sardine-web-1.0.0.post1/sardine_web/client/fonts/Fira/FiraCode-Regular.ttf`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0/sardine_web/client/fonts/Fira/FiraCode-SemiBold.ttf` & `sardine-web-1.0.0.post1/sardine_web/client/fonts/Fira/FiraCode-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0/sardine_web/client/fonts/Fira/stylesheet.css` & `sardine-web-1.0.0.post1/sardine_web/client/fonts/Fira/stylesheet.css`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0/sardine_web/client/fonts/JGSfont/jgs5.woff` & `sardine-web-1.0.0.post1/sardine_web/client/fonts/JGSfont/jgs5.woff`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0/sardine_web/client/fonts/JGSfont/jgs5.woff2` & `sardine-web-1.0.0.post1/sardine_web/client/fonts/JGSfont/jgs5.woff2`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0/sardine_web/client/fonts/JGSfont/jgs7.woff` & `sardine-web-1.0.0.post1/sardine_web/client/fonts/JGSfont/jgs7.woff`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0/sardine_web/client/fonts/JGSfont/jgs7.woff2` & `sardine-web-1.0.0.post1/sardine_web/client/fonts/JGSfont/jgs7.woff2`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0/sardine_web/client/fonts/JGSfont/jgs9.woff` & `sardine-web-1.0.0.post1/sardine_web/client/fonts/JGSfont/jgs9.woff`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0/sardine_web/client/fonts/JGSfont/jgs9.woff2` & `sardine-web-1.0.0.post1/sardine_web/client/fonts/JGSfont/jgs9.woff2`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0/sardine_web/client/fonts/JGSfont/stylesheet.css` & `sardine-web-1.0.0.post1/sardine_web/client/fonts/JGSfont/stylesheet.css`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0/sardine_web/client/fonts/JGSfont/unifont-12.0.01.woff2` & `sardine-web-1.0.0.post1/sardine_web/client/fonts/JGSfont/unifont-12.0.01.woff2`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0/sardine_web/client/fonts/JGSfont/unifont_upper-12.0.01.woff2` & `sardine-web-1.0.0.post1/sardine_web/client/fonts/JGSfont/unifont_upper-12.0.01.woff2`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0/sardine_web/client/fonts/SpaceMono/OFL.txt` & `sardine-web-1.0.0.post1/sardine_web/client/fonts/SpaceMono/OFL.txt`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0/sardine_web/client/fonts/SpaceMono/SpaceMono-Bold.ttf` & `sardine-web-1.0.0.post1/sardine_web/client/fonts/SpaceMono/SpaceMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0/sardine_web/client/fonts/SpaceMono/SpaceMono-BoldItalic.ttf` & `sardine-web-1.0.0.post1/sardine_web/client/fonts/SpaceMono/SpaceMono-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0/sardine_web/client/fonts/SpaceMono/SpaceMono-Italic.ttf` & `sardine-web-1.0.0.post1/sardine_web/client/fonts/SpaceMono/SpaceMono-Italic.ttf`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0/sardine_web/client/fonts/SpaceMono/SpaceMono-Regular.ttf` & `sardine-web-1.0.0.post1/sardine_web/client/fonts/SpaceMono/SpaceMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0/sardine_web/client/index.html` & `sardine-web-1.0.0.post1/sardine_web/client/index.html`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0/sardine_web/client/package-lock.json` & `sardine-web-1.0.0.post1/sardine_web/client/package-lock.json`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0/sardine_web/client/package.json` & `sardine-web-1.0.0.post1/sardine_web/client/package.json`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0/sardine_web/client/src/AppSettings.ts` & `sardine-web-1.0.0.post1/sardine_web/client/src/AppSettings.ts`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0/sardine_web/client/src/EditorSetup.ts` & `sardine-web-1.0.0.post1/sardine_web/client/src/EditorSetup.ts`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0/sardine_web/client/src/RunnerService.ts` & `sardine-web-1.0.0.post1/sardine_web/client/src/RunnerService.ts`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0/sardine_web/client/src/help/generalHelp.ts` & `sardine-web-1.0.0.post1/sardine_web/client/src/help/generalHelp.ts`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0/sardine_web/client/src/help/keybindingsHelp.ts` & `sardine-web-1.0.0.post1/sardine_web/client/src/help/keybindingsHelp.ts`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0/sardine_web/client/src/highlightSelection.ts` & `sardine-web-1.0.0.post1/sardine_web/client/src/highlightSelection.ts`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0/sardine_web/client/src/main.ts` & `sardine-web-1.0.0.post1/sardine_web/client/src/main.ts`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0/sardine_web/client/src/output.css` & `sardine-web-1.0.0.post1/sardine_web/client/src/output.css`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0/sardine_web/client/src/style copy.css` & `sardine-web-1.0.0.post1/sardine_web/client/src/style copy.css`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0/sardine_web/client/src/themes/sardineTheme.ts` & `sardine-web-1.0.0.post1/sardine_web/client/src/themes/sardineTheme.ts`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0/sardine_web/client/tsconfig.json` & `sardine-web-1.0.0.post1/sardine_web/client/tsconfig.json`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0/sardine_web/client/yarn.lock` & `sardine-web-1.0.0.post1/sardine_web/client/yarn.lock`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0/sardine_web/server/flask_server.py` & `sardine-web-1.0.0.post1/sardine_web/server/flask_server.py`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0/sardine_web.egg-info/PKG-INFO` & `sardine-web-1.0.0.post1/sardine_web.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sardine-web
-Version: 1.0.0
+Version: 1.0.0.post1
 Summary: Official web editor plugin for sardine-system
 Author: Raphaël Forment, thegamecracks
 Author-email: raphael.forment@gmail.com
 License: GPL-3.0-only
 Project-URL: Homepage, https://sardine.raphaelforment.fr
 Project-URL: Documentation, https://sardine.raphaelforment.fr
 Project-URL: Source Code, https://github.com/sardine-system/sardine-web
@@ -31,29 +31,41 @@
 
 # sardine-web
 
 The official web editor plugin for the [sardine-system] library!
 
 ## Installation
 
-The main repository has not yet merged CLI plugin support into the main repo.
-First follow the [installation guide] in the documentation, then install Sardine
-on the sardine-web-plugin branch like so:
+If you already have sardine-system v0.4.0+ installed or you are fine with
+the stable version of Sardine, you can go straight to installing
+this package from [PyPI]:
 
 ```sh
-# From remote:
-pip install "git+https://github.com/Bubobubobubobubo/sardine@sardine-web-plugin"
-# Or from local clone which is set to the sardine-web-plugin branch:
-pip install -e <PATH_TO_REPO>
+pip install sardine-web
 ```
 
-With Node.js / Yarn installed as per the guide, you can then install this package:
+If you do want the Sardine development version, install the repository before
+this package following their [installation guide]:
+
+```sh
+pip install git+https://github.com/Bubobubobubobubo/sardine
+pip install sardine-web
+```
+
+If you want to install the development version of *this* repository,
+make sure you have [Node.js] and [Yarn] installed:
 
 ```sh
-# From remote:
 pip install git+https://github.com/sardine-system/sardine-web
-# Or from local clone in current working directory:
-pip install -e .[dev]
 ```
 
+## Usage
+
+Documentation: https://sardine.raphaelforment.fr/editors/fishery.html
+
+This adds a `sardine web` command to Sardine to start the web editor.
+
 [sardine-system]: https://github.com/Bubobubobubobubo/sardine
+[PyPI]: https://pypi.org/project/sardine-web/
 [installation guide]: https://sardine.raphaelforment.fr/installation.html
+[Node.js]: https://nodejs.org/
+[Yarn]: https://yarnpkg.com/
```

### Comparing `sardine-web-1.0.0/sardine_web.egg-info/SOURCES.txt` & `sardine-web-1.0.0.post1/sardine_web.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sardine-web-1.0.0/setup.py` & `sardine-web-1.0.0.post1/setup.py`

 * *Files identical despite different names*

