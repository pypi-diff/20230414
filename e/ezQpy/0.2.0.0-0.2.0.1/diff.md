# Comparing `tmp/ezQpy-0.2.0.0.tar.gz` & `tmp/ezQpy-0.2.0.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezQpy-0.2.0.0.tar", last modified: Fri Jan  6 15:13:43 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

