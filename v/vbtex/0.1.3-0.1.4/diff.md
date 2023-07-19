# Comparing `tmp/vbtex-0.1.3.tar.gz` & `tmp/vbtex-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbtex-0.1.3.tar", max compression
+gzip compressed data, was "vbtex-0.1.4.tar", max compression
```

## Comparing `vbtex-0.1.3.tar` & `vbtex-0.1.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2023-06-21 16:42:53.861422 vbtex-0.1.3/README.md
--rw-r--r--   0        0        0      368 2023-07-19 12:26:41.671947 vbtex-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-07-19 12:19:39.103602 vbtex-0.1.3/vbtex/.DS_Store
--rw-r--r--   0        0        0        0 2023-06-21 16:42:53.861342 vbtex-0.1.3/vbtex/__init__.py
--rw-r--r--   0        0        0       47 2023-06-21 16:47:15.593234 vbtex-0.1.3/vbtex/__main__.py
--rw-r--r--   0        0        0     1236 2023-07-19 10:33:59.070206 vbtex-0.1.3/vbtex/choice_option.py
--rw-r--r--   0        0        0     1547 2023-07-19 12:19:19.372901 vbtex-0.1.3/vbtex/framed.py
--rw-r--r--   0        0        0      299 2023-07-19 12:20:17.191249 vbtex-0.1.3/vbtex/main.py
--rw-r--r--   0        0        0     1191 2023-07-19 12:25:10.783333 vbtex-0.1.3/vbtex/padded.py
--rw-r--r--   0        0        0      338 1970-01-01 00:00:00.000000 vbtex-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-21 16:42:53.861422 vbtex-0.1.4/README.md
+-rw-r--r--   0        0        0      368 2023-07-19 12:29:25.059051 vbtex-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-07-19 12:19:39.103602 vbtex-0.1.4/vbtex/.DS_Store
+-rw-r--r--   0        0        0        0 2023-06-21 16:42:53.861342 vbtex-0.1.4/vbtex/__init__.py
+-rw-r--r--   0        0        0       47 2023-06-21 16:47:15.593234 vbtex-0.1.4/vbtex/__main__.py
+-rw-r--r--   0        0        0     1236 2023-07-19 10:33:59.070206 vbtex-0.1.4/vbtex/choice_option.py
+-rw-r--r--   0        0        0     1547 2023-07-19 12:19:19.372901 vbtex-0.1.4/vbtex/framed.py
+-rw-r--r--   0        0        0      299 2023-07-19 12:20:17.191249 vbtex-0.1.4/vbtex/main.py
+-rw-r--r--   0        0        0     1191 2023-07-19 12:29:13.505367 vbtex-0.1.4/vbtex/padded.py
+-rw-r--r--   0        0        0      338 1970-01-01 00:00:00.000000 vbtex-0.1.4/PKG-INFO
```

### Comparing `vbtex-0.1.3/vbtex/.DS_Store` & `vbtex-0.1.4/vbtex/.DS_Store`

 * *Files identical despite different names*

### Comparing `vbtex-0.1.3/vbtex/choice_option.py` & `vbtex-0.1.4/vbtex/choice_option.py`

 * *Files identical despite different names*

### Comparing `vbtex-0.1.3/vbtex/framed.py` & `vbtex-0.1.4/vbtex/framed.py`

 * *Files identical despite different names*

### Comparing `vbtex-0.1.3/vbtex/padded.py` & `vbtex-0.1.4/vbtex/padded.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     '-p',
     '--padding',
     type = click.INT,
     default=1,
     show_default=True,
     help="Format of the output"
 )
-def framed(padding):
+def padded(padding):
     tex = click.edit()
     click.echo(tex)
     
     os.makedirs(f'./vbtex', exist_ok=True)
     path_main = os.path.join(f'./vbtex', 'main.tex')
```

