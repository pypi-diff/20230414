# Comparing `tmp/flwr_nightly-1.4.0.dev20230409.tar.gz` & `tmp/flwr_nightly-1.4.0.dev20230413-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flwr_nightly-1.4.0.dev20230409.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

