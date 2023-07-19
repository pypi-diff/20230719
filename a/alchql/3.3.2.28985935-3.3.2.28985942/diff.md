# Comparing `tmp/alchql-3.3.2.28985935.tar.gz` & `tmp/alchql-3.3.2.28985942-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alchql-3.3.2.28985935.tar", last modified: Wed Jul 19 09:15:56 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

