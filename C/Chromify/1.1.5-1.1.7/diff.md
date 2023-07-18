# Comparing `tmp/Chromify-1.1.5.tar.gz` & `tmp/Chromify-1.1.7-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Chromify-1.1.5.tar", last modified: Tue Jul 18 15:01:25 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

