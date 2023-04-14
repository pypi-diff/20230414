# Comparing `tmp/xxtea-2.0.0.post0.tar.gz` & `tmp/xxtea-3.0.0-cp311-cp311-macosx_11_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/xxtea-2.0.0.post0.tar", last modified: Fri May 15 04:52:01 2020, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

