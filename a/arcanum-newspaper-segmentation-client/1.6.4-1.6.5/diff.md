# Comparing `tmp/arcanum-newspaper-segmentation-client-1.6.4.tar.gz` & `tmp/arcanum-newspaper-segmentation-client-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcanum-newspaper-segmentation-client-1.6.4.tar", last modified: Fri Apr 14 10:19:21 2023, max compression
+gzip compressed data, was "arcanum-newspaper-segmentation-client-1.6.5.tar", last modified: Fri Apr 14 14:45:37 2023, max compression
```

## Comparing `arcanum-newspaper-segmentation-client-1.6.4.tar` & `arcanum-newspaper-segmentation-client-1.6.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 10:19:21.627918 arcanum-newspaper-segmentation-client-1.6.4/
--rw-rw-rw-   0        0        0     1101 2022-01-17 15:03:50.000000 arcanum-newspaper-segmentation-client-1.6.4/LICENSE
--rw-rw-rw-   0        0        0      675 2023-04-14 10:19:21.626921 arcanum-newspaper-segmentation-client-1.6.4/PKG-INFO
--rw-rw-rw-   0        0        0      156 2022-01-17 15:03:50.000000 arcanum-newspaper-segmentation-client-1.6.4/README.md
--rw-rw-rw-   0        0        0      110 2022-01-17 15:03:50.000000 arcanum-newspaper-segmentation-client-1.6.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-14 10:19:21.627918 arcanum-newspaper-segmentation-client-1.6.4/setup.cfg
--rw-rw-rw-   0        0        0      937 2023-04-14 10:18:40.000000 arcanum-newspaper-segmentation-client-1.6.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 10:19:21.602986 arcanum-newspaper-segmentation-client-1.6.4/src/
-drwxrwxrwx   0        0        0        0 2023-04-14 10:19:21.621934 arcanum-newspaper-segmentation-client-1.6.4/src/arcanum_newspaper_segmentation_client.egg-info/
--rw-rw-rw-   0        0        0      675 2023-04-14 10:19:21.000000 arcanum-newspaper-segmentation-client-1.6.4/src/arcanum_newspaper_segmentation_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      578 2023-04-14 10:19:21.000000 arcanum-newspaper-segmentation-client-1.6.4/src/arcanum_newspaper_segmentation_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 10:19:21.000000 arcanum-newspaper-segmentation-client-1.6.4/src/arcanum_newspaper_segmentation_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-04-14 10:19:21.000000 arcanum-newspaper-segmentation-client-1.6.4/src/arcanum_newspaper_segmentation_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       30 2023-04-14 10:19:21.000000 arcanum-newspaper-segmentation-client-1.6.4/src/arcanum_newspaper_segmentation_client.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-14 10:19:21.626921 arcanum-newspaper-segmentation-client-1.6.4/src/newspaper_segmentation_client/
--rw-rw-rw-   0        0        0    13433 2023-04-14 09:54:45.000000 arcanum-newspaper-segmentation-client-1.6.4/src/newspaper_segmentation_client/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-04-07 19:07:15.000000 arcanum-newspaper-segmentation-client-1.6.4/src/newspaper_segmentation_client/clip.py
--rw-rw-rw-   0        0        0    16873 2022-08-01 09:09:51.000000 arcanum-newspaper-segmentation-client-1.6.4/src/newspaper_segmentation_client/mets.py
--rw-rw-rw-   0        0        0     3203 2023-04-14 10:03:07.000000 arcanum-newspaper-segmentation-client-1.6.4/src/newspaper_segmentation_client/pdf.py
--rw-rw-rw-   0        0        0      704 2023-04-07 18:17:10.000000 arcanum-newspaper-segmentation-client-1.6.4/src/newspaper_segmentation_client/text.py
+drwxrwxrwx   0        0        0        0 2023-04-14 14:45:37.779317 arcanum-newspaper-segmentation-client-1.6.5/
+-rw-rw-rw-   0        0        0     1101 2022-01-17 15:03:50.000000 arcanum-newspaper-segmentation-client-1.6.5/LICENSE
+-rw-rw-rw-   0        0        0      675 2023-04-14 14:45:37.779317 arcanum-newspaper-segmentation-client-1.6.5/PKG-INFO
+-rw-rw-rw-   0        0        0      156 2022-01-17 15:03:50.000000 arcanum-newspaper-segmentation-client-1.6.5/README.md
+-rw-rw-rw-   0        0        0      110 2022-01-17 15:03:50.000000 arcanum-newspaper-segmentation-client-1.6.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-14 14:45:37.779317 arcanum-newspaper-segmentation-client-1.6.5/setup.cfg
+-rw-rw-rw-   0        0        0      937 2023-04-14 14:44:59.000000 arcanum-newspaper-segmentation-client-1.6.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 14:45:37.747778 arcanum-newspaper-segmentation-client-1.6.5/src/
+drwxrwxrwx   0        0        0        0 2023-04-14 14:45:37.779317 arcanum-newspaper-segmentation-client-1.6.5/src/arcanum_newspaper_segmentation_client.egg-info/
+-rw-rw-rw-   0        0        0      675 2023-04-14 14:45:37.000000 arcanum-newspaper-segmentation-client-1.6.5/src/arcanum_newspaper_segmentation_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      578 2023-04-14 14:45:37.000000 arcanum-newspaper-segmentation-client-1.6.5/src/arcanum_newspaper_segmentation_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 14:45:37.000000 arcanum-newspaper-segmentation-client-1.6.5/src/arcanum_newspaper_segmentation_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-04-14 14:45:37.000000 arcanum-newspaper-segmentation-client-1.6.5/src/arcanum_newspaper_segmentation_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       30 2023-04-14 14:45:37.000000 arcanum-newspaper-segmentation-client-1.6.5/src/arcanum_newspaper_segmentation_client.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 14:45:37.779317 arcanum-newspaper-segmentation-client-1.6.5/src/newspaper_segmentation_client/
+-rw-rw-rw-   0        0        0    13433 2023-04-14 10:21:05.000000 arcanum-newspaper-segmentation-client-1.6.5/src/newspaper_segmentation_client/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-04-07 19:07:15.000000 arcanum-newspaper-segmentation-client-1.6.5/src/newspaper_segmentation_client/clip.py
+-rw-rw-rw-   0        0        0    16873 2022-08-01 09:09:51.000000 arcanum-newspaper-segmentation-client-1.6.5/src/newspaper_segmentation_client/mets.py
+-rw-rw-rw-   0        0        0     3203 2023-04-14 10:21:05.000000 arcanum-newspaper-segmentation-client-1.6.5/src/newspaper_segmentation_client/pdf.py
+-rw-rw-rw-   0        0        0      756 2023-04-14 14:44:20.000000 arcanum-newspaper-segmentation-client-1.6.5/src/newspaper_segmentation_client/text.py
```

### Comparing `arcanum-newspaper-segmentation-client-1.6.4/LICENSE` & `arcanum-newspaper-segmentation-client-1.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `arcanum-newspaper-segmentation-client-1.6.4/PKG-INFO` & `arcanum-newspaper-segmentation-client-1.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcanum-newspaper-segmentation-client
-Version: 1.6.4
+Version: 1.6.5
 Summary: Client for Arcanum's Newspaper Segmentation API
 Home-page: https://www.arcanum.com/en/newspaper-segmentation/
 Author: Biszak Előd (Arcanum Ltd)
 Author-email: elod.biszak@arcanum.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `arcanum-newspaper-segmentation-client-1.6.4/setup.py` & `arcanum-newspaper-segmentation-client-1.6.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="arcanum-newspaper-segmentation-client",
-    version="1.6.4",
+    version="1.6.5",
     author="Biszak Előd (Arcanum Ltd)",
     author_email="elod.biszak@arcanum.com",
     description="Client for Arcanum's Newspaper Segmentation API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.arcanum.com/en/newspaper-segmentation/",
     classifiers=[
```

### Comparing `arcanum-newspaper-segmentation-client-1.6.4/src/arcanum_newspaper_segmentation_client.egg-info/PKG-INFO` & `arcanum-newspaper-segmentation-client-1.6.5/src/arcanum_newspaper_segmentation_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcanum-newspaper-segmentation-client
-Version: 1.6.4
+Version: 1.6.5
 Summary: Client for Arcanum's Newspaper Segmentation API
 Home-page: https://www.arcanum.com/en/newspaper-segmentation/
 Author: Biszak Előd (Arcanum Ltd)
 Author-email: elod.biszak@arcanum.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `arcanum-newspaper-segmentation-client-1.6.4/src/arcanum_newspaper_segmentation_client.egg-info/SOURCES.txt` & `arcanum-newspaper-segmentation-client-1.6.5/src/arcanum_newspaper_segmentation_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arcanum-newspaper-segmentation-client-1.6.4/src/newspaper_segmentation_client/__init__.py` & `arcanum-newspaper-segmentation-client-1.6.5/src/newspaper_segmentation_client/__init__.py`

 * *Files identical despite different names*

### Comparing `arcanum-newspaper-segmentation-client-1.6.4/src/newspaper_segmentation_client/clip.py` & `arcanum-newspaper-segmentation-client-1.6.5/src/newspaper_segmentation_client/clip.py`

 * *Files identical despite different names*

### Comparing `arcanum-newspaper-segmentation-client-1.6.4/src/newspaper_segmentation_client/mets.py` & `arcanum-newspaper-segmentation-client-1.6.5/src/newspaper_segmentation_client/mets.py`

 * *Files identical despite different names*

### Comparing `arcanum-newspaper-segmentation-client-1.6.4/src/newspaper_segmentation_client/pdf.py` & `arcanum-newspaper-segmentation-client-1.6.5/src/newspaper_segmentation_client/pdf.py`

 * *Files identical despite different names*

### Comparing `arcanum-newspaper-segmentation-client-1.6.4/src/newspaper_segmentation_client/text.py` & `arcanum-newspaper-segmentation-client-1.6.5/src/newspaper_segmentation_client/text.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,13 +8,15 @@
         for textract_block in sorted(block["ocr_blocks"], key=lambda s: s["Geometry"]["BoundingBox"]["Top"]):
             if textract_block["BlockType"] != "LINE":
                 continue
             if block["label"] != last_label:
                 texts.append("")
                 last_label = block["label"]
             text = textract_block["Text"].rstrip()
+            if not text:
+                continue
             if text[-1] in "-\xad":
                 text = text[:-1]
             elif text[-1] != " ":
                 text += " "
             texts[-1] += text
     return "\n\n".join(texts)
```

