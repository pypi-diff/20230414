# Comparing `tmp/Tectonic_Utils-0.0.9.tar.gz` & `tmp/Tectonic_Utils-0.1.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Tectonic_Utils-0.0.9.tar", last modified: Sat Jul 30 22:02:42 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

