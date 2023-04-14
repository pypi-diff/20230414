# Comparing `tmp/arcanum-newspaper-segmentation-client-1.6.3.tar.gz` & `tmp/arcanum-newspaper-segmentation-client-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcanum-newspaper-segmentation-client-1.6.3.tar", last modified: Thu Apr 13 14:35:15 2023, max compression
+gzip compressed data, was "arcanum-newspaper-segmentation-client-1.6.4.tar", last modified: Fri Apr 14 10:19:21 2023, max compression
```

## Comparing `arcanum-newspaper-segmentation-client-1.6.3.tar` & `arcanum-newspaper-segmentation-client-1.6.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 14:35:15.776889 arcanum-newspaper-segmentation-client-1.6.3/
--rw-rw-rw-   0        0        0     1101 2022-01-17 15:03:50.000000 arcanum-newspaper-segmentation-client-1.6.3/LICENSE
--rw-rw-rw-   0        0        0      675 2023-04-13 14:35:15.776889 arcanum-newspaper-segmentation-client-1.6.3/PKG-INFO
--rw-rw-rw-   0        0        0      156 2022-01-17 15:03:50.000000 arcanum-newspaper-segmentation-client-1.6.3/README.md
--rw-rw-rw-   0        0        0      110 2022-01-17 15:03:50.000000 arcanum-newspaper-segmentation-client-1.6.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-13 14:35:15.777886 arcanum-newspaper-segmentation-client-1.6.3/setup.cfg
--rw-rw-rw-   0        0        0      937 2023-04-13 14:34:12.000000 arcanum-newspaper-segmentation-client-1.6.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 14:35:15.754164 arcanum-newspaper-segmentation-client-1.6.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-13 14:35:15.771930 arcanum-newspaper-segmentation-client-1.6.3/src/arcanum_newspaper_segmentation_client.egg-info/
--rw-rw-rw-   0        0        0      675 2023-04-13 14:35:15.000000 arcanum-newspaper-segmentation-client-1.6.3/src/arcanum_newspaper_segmentation_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      578 2023-04-13 14:35:15.000000 arcanum-newspaper-segmentation-client-1.6.3/src/arcanum_newspaper_segmentation_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 14:35:15.000000 arcanum-newspaper-segmentation-client-1.6.3/src/arcanum_newspaper_segmentation_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-04-13 14:35:15.000000 arcanum-newspaper-segmentation-client-1.6.3/src/arcanum_newspaper_segmentation_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       30 2023-04-13 14:35:15.000000 arcanum-newspaper-segmentation-client-1.6.3/src/arcanum_newspaper_segmentation_client.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-13 14:35:15.775892 arcanum-newspaper-segmentation-client-1.6.3/src/newspaper_segmentation_client/
--rw-rw-rw-   0        0        0    12514 2023-04-12 11:33:38.000000 arcanum-newspaper-segmentation-client-1.6.3/src/newspaper_segmentation_client/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-04-07 19:07:15.000000 arcanum-newspaper-segmentation-client-1.6.3/src/newspaper_segmentation_client/clip.py
--rw-rw-rw-   0        0        0    16873 2022-08-01 09:09:51.000000 arcanum-newspaper-segmentation-client-1.6.3/src/newspaper_segmentation_client/mets.py
--rw-rw-rw-   0        0        0     2682 2023-04-13 14:31:28.000000 arcanum-newspaper-segmentation-client-1.6.3/src/newspaper_segmentation_client/pdf.py
--rw-rw-rw-   0        0        0      704 2023-04-07 18:17:10.000000 arcanum-newspaper-segmentation-client-1.6.3/src/newspaper_segmentation_client/text.py
+drwxrwxrwx   0        0        0        0 2023-04-14 10:19:21.627918 arcanum-newspaper-segmentation-client-1.6.4/
+-rw-rw-rw-   0        0        0     1101 2022-01-17 15:03:50.000000 arcanum-newspaper-segmentation-client-1.6.4/LICENSE
+-rw-rw-rw-   0        0        0      675 2023-04-14 10:19:21.626921 arcanum-newspaper-segmentation-client-1.6.4/PKG-INFO
+-rw-rw-rw-   0        0        0      156 2022-01-17 15:03:50.000000 arcanum-newspaper-segmentation-client-1.6.4/README.md
+-rw-rw-rw-   0        0        0      110 2022-01-17 15:03:50.000000 arcanum-newspaper-segmentation-client-1.6.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-14 10:19:21.627918 arcanum-newspaper-segmentation-client-1.6.4/setup.cfg
+-rw-rw-rw-   0        0        0      937 2023-04-14 10:18:40.000000 arcanum-newspaper-segmentation-client-1.6.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 10:19:21.602986 arcanum-newspaper-segmentation-client-1.6.4/src/
+drwxrwxrwx   0        0        0        0 2023-04-14 10:19:21.621934 arcanum-newspaper-segmentation-client-1.6.4/src/arcanum_newspaper_segmentation_client.egg-info/
+-rw-rw-rw-   0        0        0      675 2023-04-14 10:19:21.000000 arcanum-newspaper-segmentation-client-1.6.4/src/arcanum_newspaper_segmentation_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      578 2023-04-14 10:19:21.000000 arcanum-newspaper-segmentation-client-1.6.4/src/arcanum_newspaper_segmentation_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 10:19:21.000000 arcanum-newspaper-segmentation-client-1.6.4/src/arcanum_newspaper_segmentation_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-04-14 10:19:21.000000 arcanum-newspaper-segmentation-client-1.6.4/src/arcanum_newspaper_segmentation_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       30 2023-04-14 10:19:21.000000 arcanum-newspaper-segmentation-client-1.6.4/src/arcanum_newspaper_segmentation_client.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 10:19:21.626921 arcanum-newspaper-segmentation-client-1.6.4/src/newspaper_segmentation_client/
+-rw-rw-rw-   0        0        0    13433 2023-04-14 09:54:45.000000 arcanum-newspaper-segmentation-client-1.6.4/src/newspaper_segmentation_client/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-04-07 19:07:15.000000 arcanum-newspaper-segmentation-client-1.6.4/src/newspaper_segmentation_client/clip.py
+-rw-rw-rw-   0        0        0    16873 2022-08-01 09:09:51.000000 arcanum-newspaper-segmentation-client-1.6.4/src/newspaper_segmentation_client/mets.py
+-rw-rw-rw-   0        0        0     3203 2023-04-14 10:03:07.000000 arcanum-newspaper-segmentation-client-1.6.4/src/newspaper_segmentation_client/pdf.py
+-rw-rw-rw-   0        0        0      704 2023-04-07 18:17:10.000000 arcanum-newspaper-segmentation-client-1.6.4/src/newspaper_segmentation_client/text.py
```

### Comparing `arcanum-newspaper-segmentation-client-1.6.3/LICENSE` & `arcanum-newspaper-segmentation-client-1.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `arcanum-newspaper-segmentation-client-1.6.3/PKG-INFO` & `arcanum-newspaper-segmentation-client-1.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcanum-newspaper-segmentation-client
-Version: 1.6.3
+Version: 1.6.4
 Summary: Client for Arcanum's Newspaper Segmentation API
 Home-page: https://www.arcanum.com/en/newspaper-segmentation/
 Author: Biszak Előd (Arcanum Ltd)
 Author-email: elod.biszak@arcanum.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `arcanum-newspaper-segmentation-client-1.6.3/setup.py` & `arcanum-newspaper-segmentation-client-1.6.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="arcanum-newspaper-segmentation-client",
-    version="1.6.3",
+    version="1.6.4",
     author="Biszak Előd (Arcanum Ltd)",
     author_email="elod.biszak@arcanum.com",
     description="Client for Arcanum's Newspaper Segmentation API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.arcanum.com/en/newspaper-segmentation/",
     classifiers=[
```

### Comparing `arcanum-newspaper-segmentation-client-1.6.3/src/arcanum_newspaper_segmentation_client.egg-info/PKG-INFO` & `arcanum-newspaper-segmentation-client-1.6.4/src/arcanum_newspaper_segmentation_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcanum-newspaper-segmentation-client
-Version: 1.6.3
+Version: 1.6.4
 Summary: Client for Arcanum's Newspaper Segmentation API
 Home-page: https://www.arcanum.com/en/newspaper-segmentation/
 Author: Biszak Előd (Arcanum Ltd)
 Author-email: elod.biszak@arcanum.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `arcanum-newspaper-segmentation-client-1.6.3/src/arcanum_newspaper_segmentation_client.egg-info/SOURCES.txt` & `arcanum-newspaper-segmentation-client-1.6.4/src/arcanum_newspaper_segmentation_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arcanum-newspaper-segmentation-client-1.6.3/src/newspaper_segmentation_client/__init__.py` & `arcanum-newspaper-segmentation-client-1.6.4/src/newspaper_segmentation_client/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import math
 import json
 import io
+import base64
 import concurrent.futures
 from typing import BinaryIO
 
 import requests
 import numpy as np
 from PIL import Image, ImageDraw
 
@@ -221,15 +222,15 @@
 def visualize_textract_output(image, textract_output):
     new_image = image.copy()
     draw = ImageDraw.Draw(new_image)
     for block in textract_output["Blocks"]:
         if block["BlockType"] != "LINE":
             continue
         left, top, right, bottom = get_image_bounding_box(block, image)
-        draw.rectangle([int(left), int(top), int(right), int(bottom)], outline=(0, 255, 0), width=3)
+        draw.rectangle((int(left), int(top), int(right), int(bottom)), outline=(0, 255, 0), width=3)
     return new_image
 
 
 def should_split_page(page_image, textract_response):
     if page_image.height > 4000:
         return True
     min_height = min([block["Geometry"]["BoundingBox"]["Height"] for block in textract_response["Blocks"]])
@@ -254,35 +255,61 @@
         textract_response = split_page_and_run_textract(textract_client, image)
 
     textract_response["Rotation"] = np.degrees(rotation_angle)
 
     return textract_response
 
 
-def run_newspaper_segmentation(textract_client, image: BinaryIO, api_key: str):
-    image_bytes = image.read()
-
+def upload_to_s3(data):
     upload_url_response = requests.get("https://api.arcanum.com/v1/newspaper-segmentation/upload-url").json()
-    requests.put(upload_url_response["url"], data=image_bytes)
+    requests.put(upload_url_response["url"], data=data)
+    return upload_url_response["key"]
 
-    textract_response = run_textract(textract_client, image_bytes)
+
+def add_ocr_blocks(segmented_page: dict, textract_response: dict) -> None:
+    ocr_blocks_by_id = {ocr_block["Id"]: ocr_block for ocr_block in textract_response["Blocks"]}
+
+    for article in segmented_page["articles"]:
+        for block in article["blocks"]:
+            ocr_blocks = []
+            for ocr_block_id in block["ocr_blocks"]:
+                ocr_blocks.append(ocr_blocks_by_id[ocr_block_id])
+            block["ocr_blocks"] = ocr_blocks
+
+
+def run_newspaper_segmentation_on_image(image: Image, textract_response: dict, api_key: str) -> dict:
+    image.thumbnail((1024, 1024))
+    request_data = {"textract_response": textract_response}
+
+    with io.BytesIO() as image_io:
+        image.save(image_io, "JPEG")
+        request_data["image_base64"] = base64.b64encode(image_io.getvalue()).decode("ascii")
+
+    if len(json.dumps(request_data)) > 5500000:
+        request_data["textract_key"] = upload_to_s3(json.dumps(textract_response))
+        del request_data["textract_response"]
 
     response = requests.get("https://api.arcanum.com/v1/newspaper-segmentation/analyze-page",
-                            data=json.dumps(
-                                {"image": upload_url_response["key"], "textract_response": textract_response}),
-                            headers={"x-api-key": api_key})
+                            data=json.dumps(request_data), headers={"x-api-key": api_key})
 
-    return response.json()
+    if response.status_code != 200:
+        if response.status_code == 400:
+            raise RuntimeError(response.json()["error"])
+        raise RuntimeError("Error during API call")
+
+    segmented_page = response.json()
+    add_ocr_blocks(segmented_page, textract_response)
+    return segmented_page
 
 
 def run_newspaper_segmentation_without_textract(image: BinaryIO, textract_response, api_key: str):
-    image_bytes = image.read()
+    image = Image.open(image)
+    return run_newspaper_segmentation_on_image(image, textract_response, api_key)
 
-    upload_url_response = requests.get("https://api.arcanum.com/v1/newspaper-segmentation/upload-url").json()
-    requests.put(upload_url_response["url"], data=image_bytes)
 
-    response = requests.get("https://api.arcanum.com/v1/newspaper-segmentation/analyze-page",
-                            data=json.dumps(
-                                {"image": upload_url_response["key"], "textract_response": textract_response}),
-                            headers={"x-api-key": api_key})
+def run_newspaper_segmentation(textract_client, image: BinaryIO, api_key: str):
+    image_bytes = image.read()
+
+    textract_response = run_textract(textract_client, image_bytes)
+    image.seek(0)
 
-    return response.json()
+    return run_newspaper_segmentation_without_textract(image, textract_response, api_key)
```

### Comparing `arcanum-newspaper-segmentation-client-1.6.3/src/newspaper_segmentation_client/clip.py` & `arcanum-newspaper-segmentation-client-1.6.4/src/newspaper_segmentation_client/clip.py`

 * *Files identical despite different names*

### Comparing `arcanum-newspaper-segmentation-client-1.6.3/src/newspaper_segmentation_client/mets.py` & `arcanum-newspaper-segmentation-client-1.6.4/src/newspaper_segmentation_client/mets.py`

 * *Files identical despite different names*

### Comparing `arcanum-newspaper-segmentation-client-1.6.3/src/newspaper_segmentation_client/pdf.py` & `arcanum-newspaper-segmentation-client-1.6.4/src/newspaper_segmentation_client/pdf.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Dict, Tuple
 import io
 
 from PIL import Image
 import fitz
 
-from newspaper_segmentation_client import run_newspaper_segmentation_without_textract
+from newspaper_segmentation_client import run_newspaper_segmentation_on_image
 
 
 def render_pdf_page(page: fitz.Page, dpi: int = 150) -> Image:
     mat = fitz.Matrix(dpi / 72, dpi / 72)
     pix = page.get_pixmap(matrix=mat, annots=False, alpha=False)
     return Image.frombytes("RGB", (pix.width, pix.height), pix.samples)
 
@@ -25,46 +25,54 @@
     pdf_text_textract_format = {
         'Rotation': 0.0,
         'Blocks': [{
             'BlockType': 'PAGE',
             'Text': '',
             'Id': '1',
             'Geometry': {
-                'BoundingBox': {"Width": 1.0, "Height": 1.0, "Top": 0.0, "Left": 0.0}
+                'BoundingBox': {"Width": 1.0, "Height": 1.0, "Top": 0.0, "Left": 0.0},
+                'Polygon': [{'X': 0.0, 'Y': 0.0}, {'X': 1.0, 'Y': 0.0}, {'X': 1.0, 'Y': 1.0}, {'X': 0.0, 'Y': 1.0}]
             }
         }]
     }
     text_page_flags = fitz.TEXT_INHIBIT_SPACES | fitz.TEXT_PRESERVE_WHITESPACE
     page_text = page.get_text("dict", flags=text_page_flags)
     line_id = 2
     line_ids = []
     for block in page_text["blocks"]:
         for line in block["lines"]:
             line_text = "".join(span["text"] for span in line["spans"])
             if not line_text:
                 continue
             image_box = page.bound()
+            textract_bounding_box = bbox_to_textract_bounding_box(line["bbox"], image_box)
+            x_min, y_min, x_max, y_max = textract_bounding_box["Left"], textract_bounding_box["Top"], \
+                textract_bounding_box["Left"] + textract_bounding_box["Width"], \
+                textract_bounding_box["Top"] + textract_bounding_box["Height"]
+
+            polygon = [{'X': x_min, 'Y': y_min}, {'X': x_max, 'Y': y_min}, {'X': x_max, 'Y': y_max},
+                       {'X': x_min, 'Y': y_max}]
+
             pdf_text_textract_format["Blocks"].append({
                 'BlockType': 'LINE',
                 'Text': line_text,
                 'Id': str(line_id),
                 'Geometry': {
-                    'BoundingBox': bbox_to_textract_bounding_box(line["bbox"], image_box)
+                    'BoundingBox': textract_bounding_box,
+                    'Polygon': polygon
                 }
             })
+
             line_ids.append(str(line_id))
             line_id += 1
 
     pdf_text_textract_format["Blocks"][0]["Relationships"] = [
         {"Ids": line_ids, "Type": "CHILD"}
     ]
 
     return pdf_text_textract_format
 
 
 def run_newspaper_segmentation_on_pdf_page(page: fitz.Page, api_key: str):
     image = render_pdf_page(page)
     pdf_text = extract_pdf_text_to_textract_format(page)
-    with io.BytesIO() as image_io:
-        image.save(image_io, "JPEG")
-        image_io.seek(0)
-        return run_newspaper_segmentation_without_textract(image_io, pdf_text, api_key)
+    return run_newspaper_segmentation_on_image(image, pdf_text, api_key)
```

### Comparing `arcanum-newspaper-segmentation-client-1.6.3/src/newspaper_segmentation_client/text.py` & `arcanum-newspaper-segmentation-client-1.6.4/src/newspaper_segmentation_client/text.py`

 * *Files identical despite different names*

