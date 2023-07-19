# Comparing `tmp/teamscale-client-9.0.tar.gz` & `tmp/teamscale_client-9.0.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teamscale-client-9.0.tar", last modified: Mon Mar 13 06:28:34 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

