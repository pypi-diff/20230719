# Comparing `tmp/metathing-0.2.2.tar.gz` & `tmp/metathing-0.3.1-py3.11.egg`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metathing-0.2.2.tar", last modified: Thu May  4 23:27:20 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

