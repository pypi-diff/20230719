# Comparing `tmp/SALTISE_components-0.2.7.1.tar.gz` & `tmp/SALTISE_components-0.2.8.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SALTISE_components-0.2.7.1.tar", last modified: Wed May 17 04:03:58 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

