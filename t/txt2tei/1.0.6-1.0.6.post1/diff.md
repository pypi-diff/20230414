# Comparing `tmp/txt2tei-1.0.6.tar.gz` & `tmp/txt2tei-1.0.6.post1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "txt2tei-1.0.6.tar", last modified: Tue Apr 11 06:31:16 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

