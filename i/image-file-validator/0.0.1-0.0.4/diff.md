# Comparing `tmp/image-file-validator-0.0.1.tar.gz` & `tmp/image_file_validator-0.0.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image-file-validator-0.0.1.tar", last modified: Sat Apr 22 13:47:53 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

