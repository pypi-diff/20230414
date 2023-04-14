# Comparing `tmp/unstructured_inference-0.3.2.tar.gz` & `tmp/unstructured_inference-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unstructured_inference-0.3.2.tar", last modified: Fri Mar 31 22:51:41 2023, max compression
+gzip compressed data, was "unstructured_inference-0.4.0.tar", last modified: Fri Apr 14 21:36:53 2023, max compression
```

## Comparing `unstructured_inference-0.3.2.tar` & `unstructured_inference-0.4.0.tar`

### file list

```diff
@@ -1,33 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 22:51:41.325973 unstructured_inference-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     6777 2023-03-31 22:51:41.325973 unstructured_inference-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-03-31 22:49:21.000000 unstructured_inference-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-03-31 22:51:41.325973 unstructured_inference-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-03-31 22:49:21.000000 unstructured_inference-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 22:51:41.317973 unstructured_inference-0.3.2/unstructured_inference/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 22:49:21.000000 unstructured_inference-0.3.2/unstructured_inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-31 22:49:21.000000 unstructured_inference-0.3.2/unstructured_inference/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-03-31 22:49:21.000000 unstructured_inference-0.3.2/unstructured_inference/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 22:51:41.317973 unstructured_inference-0.3.2/unstructured_inference/inference/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 22:49:21.000000 unstructured_inference-0.3.2/unstructured_inference/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-03-31 22:49:21.000000 unstructured_inference-0.3.2/unstructured_inference/inference/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    15651 2023-03-31 22:49:21.000000 unstructured_inference-0.3.2/unstructured_inference/inference/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-31 22:49:21.000000 unstructured_inference-0.3.2/unstructured_inference/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 22:51:41.321973 unstructured_inference-0.3.2/unstructured_inference/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 22:49:21.000000 unstructured_inference-0.3.2/unstructured_inference/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-03-31 22:49:21.000000 unstructured_inference-0.3.2/unstructured_inference/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-03-31 22:49:21.000000 unstructured_inference-0.3.2/unstructured_inference/models/detectron2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-03-31 22:49:21.000000 unstructured_inference-0.3.2/unstructured_inference/models/donut.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-03-31 22:49:21.000000 unstructured_inference-0.3.2/unstructured_inference/models/paddle_ocr.py
--rw-r--r--   0 runner    (1001) docker     (123)    24106 2023-03-31 22:49:21.000000 unstructured_inference-0.3.2/unstructured_inference/models/table_postprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    23850 2023-03-31 22:49:21.000000 unstructured_inference-0.3.2/unstructured_inference/models/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-03-31 22:49:21.000000 unstructured_inference-0.3.2/unstructured_inference/models/tesseract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-03-31 22:49:21.000000 unstructured_inference-0.3.2/unstructured_inference/models/unstructuredmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8072 2023-03-31 22:49:21.000000 unstructured_inference-0.3.2/unstructured_inference/models/yolox.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-03-31 22:49:21.000000 unstructured_inference-0.3.2/unstructured_inference/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-03-31 22:49:21.000000 unstructured_inference-0.3.2/unstructured_inference/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 22:51:41.317973 unstructured_inference-0.3.2/unstructured_inference.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6777 2023-03-31 22:51:41.000000 unstructured_inference-0.3.2/unstructured_inference.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-03-31 22:51:41.000000 unstructured_inference-0.3.2/unstructured_inference.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 22:51:41.000000 unstructured_inference-0.3.2/unstructured_inference.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-03-31 22:51:41.000000 unstructured_inference-0.3.2/unstructured_inference.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-31 22:51:41.000000 unstructured_inference-0.3.2/unstructured_inference.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:36:53.257323 unstructured_inference-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-14 21:34:56.000000 unstructured_inference-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-04-14 21:36:53.257323 unstructured_inference-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-04-14 21:34:56.000000 unstructured_inference-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:36:53.253322 unstructured_inference-0.4.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-14 21:34:56.000000 unstructured_inference-0.4.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-14 21:36:53.257323 unstructured_inference-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-04-14 21:34:56.000000 unstructured_inference-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:36:53.253322 unstructured_inference-0.4.0/unstructured_inference/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:34:56.000000 unstructured_inference-0.4.0/unstructured_inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-14 21:34:56.000000 unstructured_inference-0.4.0/unstructured_inference/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-04-14 21:34:56.000000 unstructured_inference-0.4.0/unstructured_inference/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:36:53.253322 unstructured_inference-0.4.0/unstructured_inference/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:34:56.000000 unstructured_inference-0.4.0/unstructured_inference/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10998 2023-04-14 21:34:56.000000 unstructured_inference-0.4.0/unstructured_inference/inference/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11123 2023-04-14 21:34:56.000000 unstructured_inference-0.4.0/unstructured_inference/inference/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-14 21:34:56.000000 unstructured_inference-0.4.0/unstructured_inference/inference/layoutelement.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-14 21:34:56.000000 unstructured_inference-0.4.0/unstructured_inference/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:36:53.257323 unstructured_inference-0.4.0/unstructured_inference/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:34:56.000000 unstructured_inference-0.4.0/unstructured_inference/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-14 21:34:56.000000 unstructured_inference-0.4.0/unstructured_inference/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-04-14 21:34:56.000000 unstructured_inference-0.4.0/unstructured_inference/models/detectron2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-04-14 21:34:56.000000 unstructured_inference-0.4.0/unstructured_inference/models/donut.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-14 21:34:56.000000 unstructured_inference-0.4.0/unstructured_inference/models/paddle_ocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24106 2023-04-14 21:34:56.000000 unstructured_inference-0.4.0/unstructured_inference/models/table_postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23850 2023-04-14 21:34:56.000000 unstructured_inference-0.4.0/unstructured_inference/models/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-14 21:34:56.000000 unstructured_inference-0.4.0/unstructured_inference/models/tesseract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-14 21:34:56.000000 unstructured_inference-0.4.0/unstructured_inference/models/unstructuredmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8077 2023-04-14 21:34:56.000000 unstructured_inference-0.4.0/unstructured_inference/models/yolox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-14 21:34:56.000000 unstructured_inference-0.4.0/unstructured_inference/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-04-14 21:34:56.000000 unstructured_inference-0.4.0/unstructured_inference/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:36:53.253322 unstructured_inference-0.4.0/unstructured_inference.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-04-14 21:36:53.000000 unstructured_inference-0.4.0/unstructured_inference.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-14 21:36:53.000000 unstructured_inference-0.4.0/unstructured_inference.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 21:36:53.000000 unstructured_inference-0.4.0/unstructured_inference.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-14 21:36:53.000000 unstructured_inference-0.4.0/unstructured_inference.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 21:36:53.000000 unstructured_inference-0.4.0/unstructured_inference.egg-info/top_level.txt
```

### Comparing `unstructured_inference-0.3.2/PKG-INFO` & `unstructured_inference-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured_inference
-Version: 0.3.2
+Version: 0.4.0
 Summary: A library for performing inference using trained models.
 Home-page: https://github.com/Unstructured-IO/unstructured-inference
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
@@ -29,15 +29,15 @@
         
         ### Detectron2
         
         [Detectron2](https://github.com/facebookresearch/detectron2) is required for most inference tasks 
         but is not automatically installed with this package. 
         For MacOS and Linux, build from source with:
         ```shell
-        pip install 'git+https://github.com/facebookresearch/detectron2.git@v0.4#egg=detectron2'
+        pip install 'git+https://github.com/facebookresearch/detectron2.git@e2ce8dc#egg=detectron2'
         ```
         Other install options can be found in the 
         [Detectron2 installation guide](https://detectron2.readthedocs.io/en/latest/tutorials/install.html).
         
         Windows is not officially supported by Detectron2, but some users are able to install it anyway. 
         See discussion [here](https://layout-parser.github.io/tutorials/installation#for-windows-users) for 
         tips on installing Detectron2 on Windows.
@@ -76,38 +76,38 @@
         
         To build the Docker container, run `make docker-build`. Note that Apple hardware with an M1 chip 
         has trouble building `Detectron2` on Docker and for best results you should build it on Linux. To 
         run the API locally, use `make start-app-local`. You can stop the API with `make stop-app-local`. 
         The API will run at `http:/localhost:5000`. 
         You can then `POST` a PDF file to the API endpoint to see its layout with the command:
         ```
-        curl -X 'POST' 'http://localhost:5000/layout/pdf' -F 'file=@<your_pdf_file>' | jq -C . | less -R
+        curl -X 'POST' 'http://localhost:5000/layout/default/pdf' -F 'file=@<your_pdf_file>' | jq -C . | less -R
         ```
         
         You can also choose the types of elements you want to return from the output of PDF parsing by 
         passing a list of types to the `include_elems` parameter. For example, if you only want to return 
         `Text` elements and `Title` elements, you can curl:
         ```
-        curl -X 'POST' 'http://localhost:5000/layout/pdf' \
+        curl -X 'POST' 'http://localhost:5000/layout/default/pdf' \
         -F 'file=@<your_pdf_file>' \
         -F include_elems=Text \
         -F include_elems=Title \
          | jq -C | less -R
         ```
         If you are using an Apple M1 chip, use `make run-app-dev` instead of `make start-app-local` to 
         start the API with hot reloading. The API will run at `http:/localhost:8000`.
         
         View the swagger documentation at `http://localhost:5000/docs`.
         
         ## YoloX model
         
         For using the YoloX model the endpoints are: 
         ```
-        http://localhost:8000/layout_v1/pdf
-        http://localhost:8000/layout_v1/image
+        http://localhost:8000/layout/yolox/pdf
+        http://localhost:8000/layout/yolox/image
         ```
         For example:
         ```
         curl -X 'POST' 'http://localhost:8000/layout/yolox/image' \
         -F 'file=@sample-docs/test-image.jpg' \
          | jq -C | less -R
```

### Comparing `unstructured_inference-0.3.2/README.md` & `unstructured_inference-0.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 ### Detectron2
 
 [Detectron2](https://github.com/facebookresearch/detectron2) is required for most inference tasks 
 but is not automatically installed with this package. 
 For MacOS and Linux, build from source with:
 ```shell
-pip install 'git+https://github.com/facebookresearch/detectron2.git@v0.4#egg=detectron2'
+pip install 'git+https://github.com/facebookresearch/detectron2.git@e2ce8dc#egg=detectron2'
 ```
 Other install options can be found in the 
 [Detectron2 installation guide](https://detectron2.readthedocs.io/en/latest/tutorials/install.html).
 
 Windows is not officially supported by Detectron2, but some users are able to install it anyway. 
 See discussion [here](https://layout-parser.github.io/tutorials/installation#for-windows-users) for 
 tips on installing Detectron2 on Windows.
@@ -68,38 +68,38 @@
 
 To build the Docker container, run `make docker-build`. Note that Apple hardware with an M1 chip 
 has trouble building `Detectron2` on Docker and for best results you should build it on Linux. To 
 run the API locally, use `make start-app-local`. You can stop the API with `make stop-app-local`. 
 The API will run at `http:/localhost:5000`. 
 You can then `POST` a PDF file to the API endpoint to see its layout with the command:
 ```
-curl -X 'POST' 'http://localhost:5000/layout/pdf' -F 'file=@<your_pdf_file>' | jq -C . | less -R
+curl -X 'POST' 'http://localhost:5000/layout/default/pdf' -F 'file=@<your_pdf_file>' | jq -C . | less -R
 ```
 
 You can also choose the types of elements you want to return from the output of PDF parsing by 
 passing a list of types to the `include_elems` parameter. For example, if you only want to return 
 `Text` elements and `Title` elements, you can curl:
 ```
-curl -X 'POST' 'http://localhost:5000/layout/pdf' \
+curl -X 'POST' 'http://localhost:5000/layout/default/pdf' \
 -F 'file=@<your_pdf_file>' \
 -F include_elems=Text \
 -F include_elems=Title \
  | jq -C | less -R
 ```
 If you are using an Apple M1 chip, use `make run-app-dev` instead of `make start-app-local` to 
 start the API with hot reloading. The API will run at `http:/localhost:8000`.
 
 View the swagger documentation at `http://localhost:5000/docs`.
 
 ## YoloX model
 
 For using the YoloX model the endpoints are: 
 ```
-http://localhost:8000/layout_v1/pdf
-http://localhost:8000/layout_v1/image
+http://localhost:8000/layout/yolox/pdf
+http://localhost:8000/layout/yolox/image
 ```
 For example:
 ```
 curl -X 'POST' 'http://localhost:8000/layout/yolox/image' \
 -F 'file=@sample-docs/test-image.jpg' \
  | jq -C | less -R
```

### Comparing `unstructured_inference-0.3.2/setup.py` & `unstructured_inference-0.4.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,14 +17,28 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 from setuptools import setup, find_packages
 
 from unstructured_inference.__version__ import __version__
 
+
+def load_requirements(file_list=None):
+    if file_list is None:
+        file_list = ["requirements/base.in"]
+    if isinstance(file_list, str):
+        file_list = [file_list]
+    requirements = []
+    for file in file_list:
+        if not file.startswith("#"):
+            with open(file, encoding="utf-8") as f:
+                requirements.extend(f.readlines())
+    return requirements
+
+
 setup(
     name="unstructured_inference",
     description="A library for performing inference using trained models.",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="NLP PDF HTML CV XML parsing preprocessing",
     url="https://github.com/Unstructured-IO/unstructured-inference",
@@ -43,38 +57,26 @@
     ],
     author="Unstructured Technologies",
     author_email="devops@unstructuredai.io",
     license="Apache-2.0",
     packages=find_packages(),
     version=__version__,
     entry_points={},
-    install_requires=[
-        "fastapi",
-        "layoutparser[layoutmodels,tesseract]",
-        "python-multipart",
-        "uvicorn",
-        "huggingface-hub",
-        # NOTE(robinson) - later versions of opencv-python cause installation issues
-        # on RHEL7. We can remove this pin once the following issue from 12/2022 is resolved
-        # ref: https://github.com/opencv/opencv-python/issues/772
-        "opencv-python==4.6.0.66",
-        "onnxruntime",
-        "transformers",
-    ],
+    install_requires=load_requirements(),
     extras_require={
         "tables": [
             'unstructured.PaddleOCR ; platform_machine=="x86_64"',
             # NOTE(crag): workaround issue for error output below
             # ERROR test_unstructured/partition/test_common.py - TypeError: Descriptors cannot not
             # be created directly.
             # If this call came from a _pb2.py file, your generated code is out of date and must be
             # regenerated with protoc >= 3.19.0.
             # If you cannot immediately regenerate your protos, some other possible workarounds are:
             #  1. Downgrade the protobuf package to 3.20.x or lower.
             #  2. Set PROTOCOL_BUFFERS_PYTHON_IMPLEMENTATION=python (but this will use pure-Python
             #     parsing and will be much slower).
-            "protobuf<3.21",
+            'protobuf<3.21 ; platform_machine=="x86_64"',
             # NOTE(alan): Pin to get around error: undefined symbol: _dl_sym, version GLIBC_PRIVATE
-            "paddlepaddle>=2.4",
+            'paddlepaddle>=2.4 ; platform_machine=="x86_64"',
         ]
     },
 )
```

### Comparing `unstructured_inference-0.3.2/unstructured_inference/api.py` & `unstructured_inference-0.4.0/unstructured_inference/api.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.3.2/unstructured_inference/inference/elements.py` & `unstructured_inference-0.4.0/unstructured_inference/inference/layoutelement.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,89 +1,44 @@
 from __future__ import annotations
-from copy import deepcopy
 from dataclasses import dataclass
-from typing import Optional
+from typing import List, Optional
 
 from layoutparser.elements.layout import TextBlock
+from PIL import Image
 
-
-@dataclass
-class Rectangle:
-    x1: int
-    y1: int
-    x2: int
-    y2: int
-
-    def pad(self, padding: int):
-        """Increases (or decreases, if padding is negative) the size of the rectangle by extending
-        the boundary outward (resp. inward)."""
-        out_object = deepcopy(self)
-        out_object.x1 -= padding
-        out_object.y1 -= padding
-        out_object.x2 += padding
-        out_object.y2 += padding
-        return out_object
-
-    @property
-    def width(self):
-        """Width of rectangle"""
-        return self.x2 - self.x1
-
-    @property
-    def height(self):
-        """Height of rectangle"""
-        return self.y2 - self.y1
-
-    def is_disjoint(self, other: Rectangle):
-        """Checks whether this rectangle is disjoint from another rectangle."""
-        return ((self.x2 < other.x1) or (self.x1 > other.x2)) and (
-            (self.y2 < other.y1) or (self.y1 > other.y2)
-        )
-
-    def intersects(self, other: Rectangle):
-        """Checks whether this rectangle intersects another rectangle."""
-        return not self.is_disjoint(other)
-
-    def is_in(self, other: Rectangle, error_margin: Optional[int] = None):
-        """Checks whether this rectangle is contained within another rectangle."""
-        if error_margin is not None:
-            padded_other = other.pad(error_margin)
-        else:
-            padded_other = other
-        return all(
-            [
-                (self.x1 >= padded_other.x1),
-                (self.x2 <= padded_other.x2),
-                (self.y1 >= padded_other.y1),
-                (self.y2 <= padded_other.y2),
-            ]
-        )
-
-    @property
-    def coordinates(self):
-        """Gets coordinates of the rectangle"""
-        return ((self.x1, self.y1), (self.x1, self.y2), (self.x2, self.y2), (self.x2, self.y1))
-
-
-@dataclass
-class TextRegion(Rectangle):
-    text: Optional[str] = None
-
-    def __str__(self) -> str:
-        return str(self.text)
-
-
-class ImageTextRegion(TextRegion):
-    pass
+from unstructured_inference.inference.elements import Rectangle, TextRegion
+from unstructured_inference.models import tables
 
 
 @dataclass
 class LayoutElement(TextRegion):
     type: Optional[str] = None
 
+    def extract_text(
+        self,
+        objects: Optional[List[TextRegion]],
+        image: Optional[Image.Image] = None,
+        extract_tables: bool = False,
+        ocr_strategy: str = "auto",
+    ):
+        """Extracts text contained in region"""
+        if self.text is not None:
+            # If block text is already populated, we'll assume it's correct
+            text = self.text
+        elif extract_tables and isinstance(self, LayoutElement) and self.type == "Table":
+            text = interprete_table_block(self, image)
+        else:
+            text = super().extract_text(
+                objects=objects,
+                image=image,
+                extract_tables=extract_tables,
+                ocr_strategy=ocr_strategy,
+            )
+        return text
+
     def to_dict(self) -> dict:
         """Converts the class instance to dictionary form."""
         out_dict = {
             "coordinates": self.coordinates,
             "text": self.text,
             "type": self.type,
         }
@@ -100,7 +55,17 @@
     @classmethod
     def from_lp_textblock(cls, textblock: TextBlock):
         """Create LayoutElement from layoutparser TextBlock object."""
         x1, y1, x2, y2 = textblock.coordinates
         text = textblock.text
         type = textblock.type
         return cls(x1, y1, x2, y2, text, type)
+
+
+def interprete_table_block(text_block: TextRegion, image: Image.Image) -> str:
+    """Extract the contents of a table."""
+    tables.load_agent()
+    if tables.tables_agent is None:
+        raise RuntimeError("Unable to load table extraction agent.")
+    padded_block = text_block.pad(12)
+    cropped_image = image.crop((padded_block.x1, padded_block.y1, padded_block.x2, padded_block.y2))
+    return tables.tables_agent.predict(cropped_image)
```

### Comparing `unstructured_inference-0.3.2/unstructured_inference/models/base.py` & `unstructured_inference-0.4.0/unstructured_inference/models/base.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.3.2/unstructured_inference/models/detectron2.py` & `unstructured_inference-0.4.0/unstructured_inference/models/detectron2.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     Detectron2LayoutModel,
 )
 from layoutparser.models.model_config import LayoutModelConfig
 from PIL import Image
 from huggingface_hub import hf_hub_download
 
 from unstructured_inference.logger import logger
-from unstructured_inference.inference.elements import LayoutElement
+from unstructured_inference.inference.layoutelement import LayoutElement
 from unstructured_inference.models.unstructuredmodel import UnstructuredModel
 from unstructured_inference.utils import LazyDict, LazyEvaluateInfo
 
 
 DETECTRON_CONFIG: Final = "lp://PubLayNet/faster_rcnn_R_50_FPN_3x/config"
 DEFAULT_LABEL_MAP: Final[Dict[int, str]] = {
     0: "Text",
```

### Comparing `unstructured_inference-0.3.2/unstructured_inference/models/donut.py` & `unstructured_inference-0.4.0/unstructured_inference/models/donut.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.3.2/unstructured_inference/models/table_postprocess.py` & `unstructured_inference-0.4.0/unstructured_inference/models/table_postprocess.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.3.2/unstructured_inference/models/tables.py` & `unstructured_inference-0.4.0/unstructured_inference/models/tables.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.3.2/unstructured_inference/models/tesseract.py` & `unstructured_inference-0.4.0/unstructured_inference/models/tesseract.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.3.2/unstructured_inference/models/unstructuredmodel.py` & `unstructured_inference-0.4.0/unstructured_inference/models/unstructuredmodel.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.3.2/unstructured_inference/models/yolox.py` & `unstructured_inference-0.4.0/unstructured_inference/models/yolox.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from PIL import Image
 import cv2
 from huggingface_hub import hf_hub_download
 import numpy as np
 import onnxruntime
 from typing import List
 
-from unstructured_inference.inference.elements import LayoutElement
+from unstructured_inference.inference.layoutelement import LayoutElement
 from unstructured_inference.models.unstructuredmodel import UnstructuredModel
 from unstructured_inference.visualize import draw_bounding_boxes
 from unstructured_inference.utils import LazyDict, LazyEvaluateInfo
 
 YOLOX_LABEL_MAP = {
     0: "Caption",
     1: "Footnote",
```

### Comparing `unstructured_inference-0.3.2/unstructured_inference/utils.py` & `unstructured_inference-0.4.0/unstructured_inference/utils.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.3.2/unstructured_inference/visualize.py` & `unstructured_inference-0.4.0/unstructured_inference/visualize.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.3.2/unstructured_inference.egg-info/PKG-INFO` & `unstructured_inference-0.4.0/unstructured_inference.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured-inference
-Version: 0.3.2
+Version: 0.4.0
 Summary: A library for performing inference using trained models.
 Home-page: https://github.com/Unstructured-IO/unstructured-inference
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
@@ -29,15 +29,15 @@
         
         ### Detectron2
         
         [Detectron2](https://github.com/facebookresearch/detectron2) is required for most inference tasks 
         but is not automatically installed with this package. 
         For MacOS and Linux, build from source with:
         ```shell
-        pip install 'git+https://github.com/facebookresearch/detectron2.git@v0.4#egg=detectron2'
+        pip install 'git+https://github.com/facebookresearch/detectron2.git@e2ce8dc#egg=detectron2'
         ```
         Other install options can be found in the 
         [Detectron2 installation guide](https://detectron2.readthedocs.io/en/latest/tutorials/install.html).
         
         Windows is not officially supported by Detectron2, but some users are able to install it anyway. 
         See discussion [here](https://layout-parser.github.io/tutorials/installation#for-windows-users) for 
         tips on installing Detectron2 on Windows.
@@ -76,38 +76,38 @@
         
         To build the Docker container, run `make docker-build`. Note that Apple hardware with an M1 chip 
         has trouble building `Detectron2` on Docker and for best results you should build it on Linux. To 
         run the API locally, use `make start-app-local`. You can stop the API with `make stop-app-local`. 
         The API will run at `http:/localhost:5000`. 
         You can then `POST` a PDF file to the API endpoint to see its layout with the command:
         ```
-        curl -X 'POST' 'http://localhost:5000/layout/pdf' -F 'file=@<your_pdf_file>' | jq -C . | less -R
+        curl -X 'POST' 'http://localhost:5000/layout/default/pdf' -F 'file=@<your_pdf_file>' | jq -C . | less -R
         ```
         
         You can also choose the types of elements you want to return from the output of PDF parsing by 
         passing a list of types to the `include_elems` parameter. For example, if you only want to return 
         `Text` elements and `Title` elements, you can curl:
         ```
-        curl -X 'POST' 'http://localhost:5000/layout/pdf' \
+        curl -X 'POST' 'http://localhost:5000/layout/default/pdf' \
         -F 'file=@<your_pdf_file>' \
         -F include_elems=Text \
         -F include_elems=Title \
          | jq -C | less -R
         ```
         If you are using an Apple M1 chip, use `make run-app-dev` instead of `make start-app-local` to 
         start the API with hot reloading. The API will run at `http:/localhost:8000`.
         
         View the swagger documentation at `http://localhost:5000/docs`.
         
         ## YoloX model
         
         For using the YoloX model the endpoints are: 
         ```
-        http://localhost:8000/layout_v1/pdf
-        http://localhost:8000/layout_v1/image
+        http://localhost:8000/layout/yolox/pdf
+        http://localhost:8000/layout/yolox/image
         ```
         For example:
         ```
         curl -X 'POST' 'http://localhost:8000/layout/yolox/image' \
         -F 'file=@sample-docs/test-image.jpg' \
          | jq -C | less -R
```

### Comparing `unstructured_inference-0.3.2/unstructured_inference.egg-info/SOURCES.txt` & `unstructured_inference-0.4.0/unstructured_inference.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,27 @@
+MANIFEST.in
 README.md
 setup.cfg
 setup.py
+requirements/base.in
 unstructured_inference/__init__.py
 unstructured_inference/__version__.py
 unstructured_inference/api.py
 unstructured_inference/logger.py
 unstructured_inference/utils.py
 unstructured_inference/visualize.py
 unstructured_inference.egg-info/PKG-INFO
 unstructured_inference.egg-info/SOURCES.txt
 unstructured_inference.egg-info/dependency_links.txt
 unstructured_inference.egg-info/requires.txt
 unstructured_inference.egg-info/top_level.txt
 unstructured_inference/inference/__init__.py
 unstructured_inference/inference/elements.py
 unstructured_inference/inference/layout.py
+unstructured_inference/inference/layoutelement.py
 unstructured_inference/models/__init__.py
 unstructured_inference/models/base.py
 unstructured_inference/models/detectron2.py
 unstructured_inference/models/donut.py
 unstructured_inference/models/paddle_ocr.py
 unstructured_inference/models/table_postprocess.py
 unstructured_inference/models/tables.py
```

