# Comparing `tmp/seqlog-0.3.8.tar.gz` & `tmp/seqlog-0.3.9-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/seqlog-0.3.8.tar", last modified: Sat Jan  6 21:11:10 2018, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

