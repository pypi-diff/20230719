# Comparing `tmp/cre-0.4.1.tar.gz` & `tmp/cre-0.4.2-cp39-cp39-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cre-0.4.1.tar", last modified: Tue Jul 18 18:12:36 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

