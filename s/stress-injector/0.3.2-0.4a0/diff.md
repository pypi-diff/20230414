# Comparing `tmp/stress-injector-0.3.2.tar.gz` & `tmp/stress_injector-0.4a0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stress-injector-0.3.2.tar", last modified: Mon May 23 20:37:24 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

