# Comparing `tmp/intelmq-manager-3.1.0rc1.tar.gz` & `tmp/intelmq_manager-3.2.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intelmq-manager-3.1.0rc1.tar", last modified: Tue Aug  2 16:42:17 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

