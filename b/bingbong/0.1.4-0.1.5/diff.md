# Comparing `tmp/bingbong-0.1.4.tar.gz` & `tmp/bingbong-0.1.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bingbong-0.1.4.tar", last modified: Wed Apr 12 15:50:15 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

