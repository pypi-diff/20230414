# Comparing `tmp/point-cloud-utils-0.29.1.tar.gz` & `tmp/point_cloud_utils-0.29.3-cp310-cp310-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "point-cloud-utils-0.29.1.tar", last modified: Wed Jan 18 04:49:35 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

