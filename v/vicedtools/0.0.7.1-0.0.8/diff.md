# Comparing `tmp/vicedtools-0.0.7.1.tar.gz` & `tmp/vicedtools-0.0.8-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vicedtools-0.0.7.1.tar", last modified: Mon Jun 13 14:55:37 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

