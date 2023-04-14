# Comparing `tmp/libasd-1.5.5.tar.gz` & `tmp/libasd-1.5.6-cp39-cp39-macosx_12_0_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libasd-1.5.5.tar", last modified: Fri Nov 11 12:57:00 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

