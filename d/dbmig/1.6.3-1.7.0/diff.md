# Comparing `tmp/dbmig-1.6.3.tar.gz` & `tmp/dbmig-1.7.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dbmig-1.6.3.tar", last modified: Sun Jun 25 12:25:27 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

