# Comparing `tmp/alchql-3.3.3.28991729.tar.gz` & `tmp/alchql-3.3.3.28991737-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alchql-3.3.3.28991729.tar", last modified: Wed Jul 19 10:52:30 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

