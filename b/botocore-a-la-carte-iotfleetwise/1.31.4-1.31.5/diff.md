# Comparing `tmp/botocore-a-la-carte-iotfleetwise-1.31.4.tar.gz` & `tmp/botocore_a_la_carte_iotfleetwise-1.31.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-iotfleetwise-1.31.4.tar", last modified: Tue Jul 18 01:55:14 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

