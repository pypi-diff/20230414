# Comparing `tmp/loky-3.3.0.tar.gz` & `tmp/loky-3.4.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loky-3.3.0.tar", last modified: Thu Sep 15 15:56:04 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

