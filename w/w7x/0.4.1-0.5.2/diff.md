# Comparing `tmp/w7x-0.4.1.tar.gz` & `tmp/w7x-0.5.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/w7x-0.4.1.tar", last modified: Thu Sep  8 11:49:30 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

