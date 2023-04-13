# Comparing `tmp/pysparkler-0.3.dev1681170435.tar.gz` & `tmp/pysparkler-0.3.dev1681426546-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysparkler-0.3.dev1681170435.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

