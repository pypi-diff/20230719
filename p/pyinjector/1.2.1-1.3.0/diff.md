# Comparing `tmp/pyinjector-1.2.1.tar.gz` & `tmp/pyinjector-1.3.0-cp37-cp37m-win32.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyinjector-1.2.1.tar", last modified: Tue Jul 11 21:59:02 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

