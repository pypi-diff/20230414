# Comparing `tmp/sgd_dstc8_data_model-0.1.2.tar.gz` & `tmp/sgd_dstc8_data_model-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sgd_dstc8_data_model-0.1.2.tar", max compression
+gzip compressed data, was "sgd_dstc8_data_model-0.1.3.tar", max compression
```

## Comparing `sgd_dstc8_data_model-0.1.2.tar` & `sgd_dstc8_data_model-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0      194 2023-03-26 18:28:50.772270 sgd_dstc8_data_model-0.1.2/README.md
--rw-r--r--   0        0        0      907 2023-03-28 18:18:21.482672 sgd_dstc8_data_model-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-26 17:53:27.185714 sgd_dstc8_data_model-0.1.2/sgd_dstc8_data_model/__init__.py
--rw-r--r--   0        0        0       25 2023-03-26 16:13:34.000000 sgd_dstc8_data_model-0.1.2/sgd_dstc8_data_model/constants.yaml
--rw-r--r--   0        0        0     1386 2023-03-26 17:10:23.000000 sgd_dstc8_data_model-0.1.2/sgd_dstc8_data_model/dstc_constants.py
--rw-r--r--   0        0        0     7212 2023-03-25 21:15:03.000000 sgd_dstc8_data_model-0.1.2/sgd_dstc8_data_model/dstc_dataclasses.py
--rw-r--r--   0        0        0      775 2023-03-26 17:03:19.000000 sgd_dstc8_data_model-0.1.2/sgd_dstc8_data_model/dstc_utils.py
--rw-r--r--   0        0        0       80 2023-03-25 21:38:17.000000 sgd_dstc8_data_model-0.1.2/sgd_dstc8_data_model/example.py
--rw-r--r--   0        0        0      647 2023-03-25 21:03:30.000000 sgd_dstc8_data_model-0.1.2/sgd_dstc8_data_model/special_tokens.yaml
--rw-r--r--   0        0        0     1258 1970-01-01 00:00:00.000000 sgd_dstc8_data_model-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-14 06:22:51.949605 sgd_dstc8_data_model-0.1.3/LICENSE
+-rw-r--r--   0        0        0      194 2023-03-26 18:28:50.772270 sgd_dstc8_data_model-0.1.3/README.md
+-rw-r--r--   0        0        0     1033 2023-04-14 06:23:54.990259 sgd_dstc8_data_model-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-26 17:53:27.185714 sgd_dstc8_data_model-0.1.3/sgd_dstc8_data_model/__init__.py
+-rw-r--r--   0        0        0     1362 2023-04-14 06:18:23.366819 sgd_dstc8_data_model-0.1.3/sgd_dstc8_data_model/dstc_constants.py
+-rw-r--r--   0        0        0     7259 2023-04-14 06:18:08.046660 sgd_dstc8_data_model-0.1.3/sgd_dstc8_data_model/dstc_dataclasses.py
+-rw-r--r--   0        0        0      754 2023-04-14 06:18:19.518779 sgd_dstc8_data_model-0.1.3/sgd_dstc8_data_model/dstc_utils.py
+-rw-r--r--   0        0        0       80 2023-03-25 21:38:17.000000 sgd_dstc8_data_model-0.1.3/sgd_dstc8_data_model/example.py
+-rw-r--r--   0        0        0     1305 1970-01-01 00:00:00.000000 sgd_dstc8_data_model-0.1.3/PKG-INFO
```

### Comparing `sgd_dstc8_data_model-0.1.2/pyproject.toml` & `sgd_dstc8_data_model-0.1.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sgd-dstc8-data-model"
-version = "0.1.2"
+version = "0.1.3"
 description = "Model Classes for the SGD DSTC8 dataset"
 authors = ["Adib Mosharrof <adib.mosharrof@gmail.com>"]
 repository = "https://github.com/adibMosharrof/sgd_dstc8_data_model"
 readme = "README.md"
 packages = [{include = "sgd_dstc8_data_model"}]
 keywords = ["sgd", "dstc8", "data", "model", "classes"]
 classifiers = [
@@ -16,17 +16,19 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 dataclasses-json = "^0.5.7"
 pyyaml = "^6.0"
+class-registry = "^2.1.2"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 pytest = "^7.2.2"
 
-
+[tool.poetry.plugins."dstc_special_tokens"]
+dstc_special_tokens = "dstc_constants:DstcSpecialTokens"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `sgd_dstc8_data_model-0.1.2/sgd_dstc8_data_model/dstc_constants.py` & `sgd_dstc8_data_model-0.1.3/sgd_dstc8_data_model/dstc_constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from typing import Dict
 from enum import Enum
 
 
 class DstcSteps(str, Enum):
     TRAIN = "train"
     DEV = "dev"
     TEST = "test"
```

### Comparing `sgd_dstc8_data_model-0.1.2/sgd_dstc8_data_model/dstc_dataclasses.py` & `sgd_dstc8_data_model-0.1.3/sgd_dstc8_data_model/dstc_dataclasses.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from collections import defaultdict
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Dict, Optional, List
 
 from dataclasses_json import dataclass_json
-from dstc_constants import DstcSpecialTokens, DstcConstants, DstcSteps, DstcSpeaker
+from sgd_dstc8_data_model.dstc_constants import DstcSpecialTokens, DstcConstants, DstcSteps, DstcSpeaker
 
-import dstc_utils
+from sgd_dstc8_data_model import dstc_utils
 
 
 class DstcObjectAttributeException(Exception):
     pass
 
 
 @dataclass
```

### Comparing `sgd_dstc8_data_model-0.1.2/sgd_dstc8_data_model/dstc_utils.py` & `sgd_dstc8_data_model-0.1.3/sgd_dstc8_data_model/dstc_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from ast import Dict
 import json
 
 import yaml
 
 
 def get_dstc_service_name(service_name: str) -> str:
     return service_name[: service_name.find("_")]
```

### Comparing `sgd_dstc8_data_model-0.1.2/PKG-INFO` & `sgd_dstc8_data_model-0.1.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sgd-dstc8-data-model
-Version: 0.1.2
+Version: 0.1.3
 Summary: Model Classes for the SGD DSTC8 dataset
 Home-page: https://github.com/adibMosharrof/sgd_dstc8_data_model
 Keywords: sgd,dstc8,data,model,classes
 Author: Adib Mosharrof
 Author-email: adib.mosharrof@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: class-registry (>=2.1.2,<3.0.0)
 Requires-Dist: dataclasses-json (>=0.5.7,<0.6.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Project-URL: Repository, https://github.com/adibMosharrof/sgd_dstc8_data_model
 Description-Content-Type: text/markdown
 
 # SGD DSTC8 Data Model
```

