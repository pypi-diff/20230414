# Comparing `tmp/synchrony-0.1.0.tar.gz` & `tmp/synchrony-0.1.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\synchrony-0.1.0.tar", last modified: Thu Jan 13 17:56:53 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

