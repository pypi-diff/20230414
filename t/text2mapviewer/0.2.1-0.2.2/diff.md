# Comparing `tmp/text2mapviewer-0.2.1.tar.gz` & `tmp/text2mapviewer-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text2mapviewer-0.2.1.tar", last modified: Thu Apr 13 13:09:34 2023, max compression
+gzip compressed data, was "text2mapviewer-0.2.2.tar", last modified: Fri Apr 14 12:09:38 2023, max compression
```

## Comparing `text2mapviewer-0.2.1.tar` & `text2mapviewer-0.2.2.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxrwxr-x   0 hpzn1899  (1000) hpzn1899  (1000)        0 2023-04-13 13:09:34.300559 text2mapviewer-0.2.1/
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     1077 2023-04-13 08:39:45.000000 text2mapviewer-0.2.1/LICENSE
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)       40 2023-04-13 11:39:22.000000 text2mapviewer-0.2.1/MANIFEST.in
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     2457 2023-04-13 13:09:34.300559 text2mapviewer-0.2.1/PKG-INFO
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     1889 2023-04-13 12:35:34.000000 text2mapviewer-0.2.1/README.md
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)      801 2023-04-13 13:09:22.000000 text2mapviewer-0.2.1/pyproject.toml
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     4626 2023-04-13 13:08:51.000000 text2mapviewer-0.2.1/requirements.txt
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)       38 2023-04-13 13:09:34.300559 text2mapviewer-0.2.1/setup.cfg
-drwxrwxr-x   0 hpzn1899  (1000) hpzn1899  (1000)        0 2023-04-13 13:09:34.300559 text2mapviewer-0.2.1/text2mapviewer/
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)       76 2023-04-13 08:30:11.000000 text2mapviewer-0.2.1/text2mapviewer/__init__.py
-drwxrwxr-x   0 hpzn1899  (1000) hpzn1899  (1000)        0 2023-04-13 13:09:34.300559 text2mapviewer-0.2.1/text2mapviewer/examples/
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)      170 2023-04-13 08:39:45.000000 text2mapviewer-0.2.1/text2mapviewer/examples/map_embedding.py
-drwxrwxr-x   0 hpzn1899  (1000) hpzn1899  (1000)        0 2023-04-13 13:09:34.300559 text2mapviewer-0.2.1/text2mapviewer/fondamental/
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     2011 2023-04-13 08:39:45.000000 text2mapviewer-0.2.1/text2mapviewer/fondamental/bases.py
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     1894 2023-04-13 08:39:45.000000 text2mapviewer-0.2.1/text2mapviewer/main.py
-drwxrwxr-x   0 hpzn1899  (1000) hpzn1899  (1000)        0 2023-04-13 13:09:34.300559 text2mapviewer-0.2.1/text2mapviewer.egg-info/
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     2457 2023-04-13 13:09:34.000000 text2mapviewer-0.2.1/text2mapviewer.egg-info/PKG-INFO
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)      377 2023-04-13 13:09:34.000000 text2mapviewer-0.2.1/text2mapviewer.egg-info/SOURCES.txt
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)        1 2023-04-13 13:09:34.000000 text2mapviewer-0.2.1/text2mapviewer.egg-info/dependency_links.txt
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)       66 2023-04-13 13:09:34.000000 text2mapviewer-0.2.1/text2mapviewer.egg-info/requires.txt
--rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)       15 2023-04-13 13:09:34.000000 text2mapviewer-0.2.1/text2mapviewer.egg-info/top_level.txt
+drwxrwxr-x   0 hpzn1899  (1000) hpzn1899  (1000)        0 2023-04-14 12:09:38.829453 text2mapviewer-0.2.2/
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     1077 2023-04-13 08:39:45.000000 text2mapviewer-0.2.2/LICENSE
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)       40 2023-04-13 11:39:22.000000 text2mapviewer-0.2.2/MANIFEST.in
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     3115 2023-04-14 12:09:38.829453 text2mapviewer-0.2.2/PKG-INFO
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     2546 2023-04-14 11:46:26.000000 text2mapviewer-0.2.2/README.md
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)      801 2023-04-14 11:47:21.000000 text2mapviewer-0.2.2/pyproject.toml
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     4626 2023-04-13 13:08:51.000000 text2mapviewer-0.2.2/requirements.txt
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)       38 2023-04-14 12:09:38.829453 text2mapviewer-0.2.2/setup.cfg
+drwxrwxr-x   0 hpzn1899  (1000) hpzn1899  (1000)        0 2023-04-14 12:09:38.829453 text2mapviewer-0.2.2/text2mapviewer/
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)       76 2023-04-13 08:30:11.000000 text2mapviewer-0.2.2/text2mapviewer/__init__.py
+drwxrwxr-x   0 hpzn1899  (1000) hpzn1899  (1000)        0 2023-04-14 12:09:38.829453 text2mapviewer-0.2.2/text2mapviewer/examples/
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)      233 2023-04-14 12:04:59.000000 text2mapviewer-0.2.2/text2mapviewer/examples/map_embedding.py
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)      613 2023-04-14 12:07:38.000000 text2mapviewer-0.2.2/text2mapviewer/examples/map_embedding_click.py
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     2929 2023-04-14 12:06:13.000000 text2mapviewer-0.2.2/text2mapviewer/examples/map_text_embedding.py
+drwxrwxr-x   0 hpzn1899  (1000) hpzn1899  (1000)        0 2023-04-14 12:09:38.829453 text2mapviewer-0.2.2/text2mapviewer/fondamental/
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     2019 2023-04-14 12:07:09.000000 text2mapviewer-0.2.2/text2mapviewer/fondamental/bases.py
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     1902 2023-04-14 12:06:44.000000 text2mapviewer-0.2.2/text2mapviewer/main.py
+drwxrwxr-x   0 hpzn1899  (1000) hpzn1899  (1000)        0 2023-04-14 12:09:38.829453 text2mapviewer-0.2.2/text2mapviewer.egg-info/
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)     3115 2023-04-14 12:09:38.000000 text2mapviewer-0.2.2/text2mapviewer.egg-info/PKG-INFO
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)      470 2023-04-14 12:09:38.000000 text2mapviewer-0.2.2/text2mapviewer.egg-info/SOURCES.txt
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)        1 2023-04-14 12:09:38.000000 text2mapviewer-0.2.2/text2mapviewer.egg-info/dependency_links.txt
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)       66 2023-04-14 12:09:38.000000 text2mapviewer-0.2.2/text2mapviewer.egg-info/requires.txt
+-rw-rw-r--   0 hpzn1899  (1000) hpzn1899  (1000)       15 2023-04-14 12:09:38.000000 text2mapviewer-0.2.2/text2mapviewer.egg-info/top_level.txt
```

### Comparing `text2mapviewer-0.2.1/LICENSE` & `text2mapviewer-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `text2mapviewer-0.2.1/PKG-INFO` & `text2mapviewer-0.2.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,81 @@
 Metadata-Version: 2.1
 Name: text2mapviewer
-Version: 0.2.1
+Version: 0.2.2
 Summary: A python package to map your own csv files data using Atlas from NOMIC
 Author-email: Papa Séga WADE <pasega.wade@gmail.com>
 Project-URL: Homepage, https://github.com/papasega/text2mapviewer
 Keywords: Embedding, Visualization, Map, Text, CSV,  Search keywords, Dynamic
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-This is a vesy simple way to map your text data using [Altas from NOMIC](https://docs.nomic.ai/index.html) using the lib `click`. 
+This is a vesy simple way to map your text data using [Altas from NOMIC](https://docs.nomic.ai/index.html) using the lib `click`.
 
 You have to create an account to get API_KEY NOMIC. 
 
-Atlas enables you to:
-
-Store, update and organize multi-million point datasets of unstructured text, images and embeddings.
-
-Visually interact with your datasets from a web browser.
-
-Run semantic search and vector operations over your datasets.
-
+<< Atlas enables you to:
+* Store, update and organize multi-million point datasets of unstructured text, images and embeddings.
+* Visually interact with your datasets from a web browser.
+* Run semantic search and vector operations over your datasets.
 Use Atlas to:
 
     - Visualize, interact, collaborate and share large datasets of text and embeddings.
-    
     - Collaboratively clean, tag and label your datasets
-    
     - Build high-availability apps powered by semantic search
-    
-    - Understand and debug the latent space of your AI model trains
+    - Understand and debug the latent space of your AI model trains  >>
+
 
 # How to use
 ### Installation
 
 To install the necessary dependencies, run the following command:
 
 ```bash
 python -m venv mymapenv 
 source mymapenv/bin/activate
 pip install --upgrade pip 
 pip install text2mapviewer
 ```
 
+### Login NOMIC server
+
+Login/create your Nomic account:
+
+```bash
+nomic login
+```
+If you have already your account : 
+
+```bash
+nomic login [YOUR_API_TOKEN_NOMIC_HERE] 
+```
+## Examples : 
+#### from NOMIC and with lib text2mapviewer 
+```python
+from text2mapviewer.examples.map_embedding import project
+
+# Use the projet from the lib text2mapviewer 
+print(project) 
+```
+
+#### With the lib `click` after clone this ripo
+
+```python
+python scr/text2mapviewer/examples/map_embedding_click.py --num_embeddings 10000 --embedding_dim 256
+```
+
+#### [ The Animation Ouput](https://atlas.nomic.ai/map/0b4c0459-98f2-4aab-8d47-875765832049/54017477-907d-46e8-8d56-dddf7ab7fcfc)
+
+
+
+
 ## Supported Transformer Models from Hugging Face 
 
 This project supports a variety of transformer models, including models from the Hugging Face Model Hub and sentence-transformers. Below are some examples:
     - Hugging Face Model: 'prajjwal1/bert-mini'
     - Hugging Face Model: 'Sahajtomar/french_semantic'  (french version for semantic search embedding) 
     - Sentence-Transformers Model: 'sentence-transformers/all-MiniLM-L6-v2' etc...
 
@@ -57,14 +83,14 @@
 
 ## To map your text/csv  files
 
 ```bash
 pip install -r requirements.txt
 python main.py --transformer-model-name MODEL_NAME --cache_dir CACHE_DIR --batch-size BATCH_SIZE --file-path FILE_PATH
 ```
-Remarque for the CACHE_DIR : you can setup it like ==> 
+NOTE: for the CACHE_DIR : you can setup it like ==> 
 
 ```bash
 export TRANSFORMERS_CACHE=/path_to_your/transformers_cache
 ```
 
 Give a fidback.
```

### Comparing `text2mapviewer-0.2.1/README.md` & `text2mapviewer-0.2.2/text2mapviewer.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,81 @@
-This is a vesy simple way to map your text data using [Altas from NOMIC](https://docs.nomic.ai/index.html) using the lib `click`. 
+Metadata-Version: 2.1
+Name: text2mapviewer
+Version: 0.2.2
+Summary: A python package to map your own csv files data using Atlas from NOMIC
+Author-email: Papa Séga WADE <pasega.wade@gmail.com>
+Project-URL: Homepage, https://github.com/papasega/text2mapviewer
+Keywords: Embedding, Visualization, Map, Text, CSV,  Search keywords, Dynamic
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
 
-You have to create an account to get API_KEY NOMIC. 
-
-Atlas enables you to:
-
-Store, update and organize multi-million point datasets of unstructured text, images and embeddings.
+This is a vesy simple way to map your text data using [Altas from NOMIC](https://docs.nomic.ai/index.html) using the lib `click`.
 
-Visually interact with your datasets from a web browser.
-
-Run semantic search and vector operations over your datasets.
+You have to create an account to get API_KEY NOMIC. 
 
+<< Atlas enables you to:
+* Store, update and organize multi-million point datasets of unstructured text, images and embeddings.
+* Visually interact with your datasets from a web browser.
+* Run semantic search and vector operations over your datasets.
 Use Atlas to:
 
     - Visualize, interact, collaborate and share large datasets of text and embeddings.
-    
     - Collaboratively clean, tag and label your datasets
-    
     - Build high-availability apps powered by semantic search
-    
-    - Understand and debug the latent space of your AI model trains
+    - Understand and debug the latent space of your AI model trains  >>
+
 
 # How to use
 ### Installation
 
 To install the necessary dependencies, run the following command:
 
 ```bash
 python -m venv mymapenv 
 source mymapenv/bin/activate
 pip install --upgrade pip 
 pip install text2mapviewer
 ```
 
+### Login NOMIC server
+
+Login/create your Nomic account:
+
+```bash
+nomic login
+```
+If you have already your account : 
+
+```bash
+nomic login [YOUR_API_TOKEN_NOMIC_HERE] 
+```
+## Examples : 
+#### from NOMIC and with lib text2mapviewer 
+```python
+from text2mapviewer.examples.map_embedding import project
+
+# Use the projet from the lib text2mapviewer 
+print(project) 
+```
+
+#### With the lib `click` after clone this ripo
+
+```python
+python scr/text2mapviewer/examples/map_embedding_click.py --num_embeddings 10000 --embedding_dim 256
+```
+
+#### [ The Animation Ouput](https://atlas.nomic.ai/map/0b4c0459-98f2-4aab-8d47-875765832049/54017477-907d-46e8-8d56-dddf7ab7fcfc)
+
+
+
+
 ## Supported Transformer Models from Hugging Face 
 
 This project supports a variety of transformer models, including models from the Hugging Face Model Hub and sentence-transformers. Below are some examples:
     - Hugging Face Model: 'prajjwal1/bert-mini'
     - Hugging Face Model: 'Sahajtomar/french_semantic'  (french version for semantic search embedding) 
     - Sentence-Transformers Model: 'sentence-transformers/all-MiniLM-L6-v2' etc...
 
@@ -43,14 +83,14 @@
 
 ## To map your text/csv  files
 
 ```bash
 pip install -r requirements.txt
 python main.py --transformer-model-name MODEL_NAME --cache_dir CACHE_DIR --batch-size BATCH_SIZE --file-path FILE_PATH
 ```
-Remarque for the CACHE_DIR : you can setup it like ==> 
+NOTE: for the CACHE_DIR : you can setup it like ==> 
 
 ```bash
 export TRANSFORMERS_CACHE=/path_to_your/transformers_cache
 ```
 
 Give a fidback.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `text2mapviewer-0.2.1/pyproject.toml` & `text2mapviewer-0.2.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "text2mapviewer"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
     {name= "Papa Séga WADE", email= "pasega.wade@gmail.com"}
 ]
 
 description = "A python package to map your own csv files data using Atlas from NOMIC"
 readme={file = "README.md", content-type = "text/markdown"} 
 keywords=[
```

### Comparing `text2mapviewer-0.2.1/requirements.txt` & `text2mapviewer-0.2.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `text2mapviewer-0.2.1/text2mapviewer/fondamental/bases.py` & `text2mapviewer-0.2.2/text2mapviewer/fondamental/bases.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-# -- Papa Séga WADE 13/04/2023 --
+""" 
+-- Papa Séga WADE 13/04/2023 --
+""" 
 from transformers import AutoTokenizer, AutoModel
 import numpy as np
 import torch
 import csv
 from typing import List, Dict,  Any, Optional, Tuple
 from nomic import atlas
```

### Comparing `text2mapviewer-0.2.1/text2mapviewer/main.py` & `text2mapviewer-0.2.2/text2mapviewer/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-# -- Papa Séga WADE 13/04/2023 --
+"""
+ -- Papa Séga WADE 13/04/2023 --
+"""
+
 import click
 import torch as th 
 from typing import List, Dict
 from fondamental.bases import * # or import --> load_documents, encode_documents, map_embeddings_to_atlas
 
 @click.command()
 @click.option('--transformer-model-name' , required=True, type=str, help='The name of the transformer model to load.')
```

### Comparing `text2mapviewer-0.2.1/text2mapviewer.egg-info/PKG-INFO` & `text2mapviewer-0.2.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,55 +1,67 @@
-Metadata-Version: 2.1
-Name: text2mapviewer
-Version: 0.2.1
-Summary: A python package to map your own csv files data using Atlas from NOMIC
-Author-email: Papa Séga WADE <pasega.wade@gmail.com>
-Project-URL: Homepage, https://github.com/papasega/text2mapviewer
-Keywords: Embedding, Visualization, Map, Text, CSV,  Search keywords, Dynamic
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-This is a vesy simple way to map your text data using [Altas from NOMIC](https://docs.nomic.ai/index.html) using the lib `click`. 
+This is a vesy simple way to map your text data using [Altas from NOMIC](https://docs.nomic.ai/index.html) using the lib `click`.
 
 You have to create an account to get API_KEY NOMIC. 
 
-Atlas enables you to:
-
-Store, update and organize multi-million point datasets of unstructured text, images and embeddings.
-
-Visually interact with your datasets from a web browser.
-
-Run semantic search and vector operations over your datasets.
-
+<< Atlas enables you to:
+* Store, update and organize multi-million point datasets of unstructured text, images and embeddings.
+* Visually interact with your datasets from a web browser.
+* Run semantic search and vector operations over your datasets.
 Use Atlas to:
 
     - Visualize, interact, collaborate and share large datasets of text and embeddings.
-    
     - Collaboratively clean, tag and label your datasets
-    
     - Build high-availability apps powered by semantic search
-    
-    - Understand and debug the latent space of your AI model trains
+    - Understand and debug the latent space of your AI model trains  >>
+
 
 # How to use
 ### Installation
 
 To install the necessary dependencies, run the following command:
 
 ```bash
 python -m venv mymapenv 
 source mymapenv/bin/activate
 pip install --upgrade pip 
 pip install text2mapviewer
 ```
 
+### Login NOMIC server
+
+Login/create your Nomic account:
+
+```bash
+nomic login
+```
+If you have already your account : 
+
+```bash
+nomic login [YOUR_API_TOKEN_NOMIC_HERE] 
+```
+## Examples : 
+#### from NOMIC and with lib text2mapviewer 
+```python
+from text2mapviewer.examples.map_embedding import project
+
+# Use the projet from the lib text2mapviewer 
+print(project) 
+```
+
+#### With the lib `click` after clone this ripo
+
+```python
+python scr/text2mapviewer/examples/map_embedding_click.py --num_embeddings 10000 --embedding_dim 256
+```
+
+#### [ The Animation Ouput](https://atlas.nomic.ai/map/0b4c0459-98f2-4aab-8d47-875765832049/54017477-907d-46e8-8d56-dddf7ab7fcfc)
+
+
+
+
 ## Supported Transformer Models from Hugging Face 
 
 This project supports a variety of transformer models, including models from the Hugging Face Model Hub and sentence-transformers. Below are some examples:
     - Hugging Face Model: 'prajjwal1/bert-mini'
     - Hugging Face Model: 'Sahajtomar/french_semantic'  (french version for semantic search embedding) 
     - Sentence-Transformers Model: 'sentence-transformers/all-MiniLM-L6-v2' etc...
 
@@ -57,14 +69,14 @@
 
 ## To map your text/csv  files
 
 ```bash
 pip install -r requirements.txt
 python main.py --transformer-model-name MODEL_NAME --cache_dir CACHE_DIR --batch-size BATCH_SIZE --file-path FILE_PATH
 ```
-Remarque for the CACHE_DIR : you can setup it like ==> 
+NOTE: for the CACHE_DIR : you can setup it like ==> 
 
 ```bash
 export TRANSFORMERS_CACHE=/path_to_your/transformers_cache
 ```
 
-Give a fidback. 
+Give a fidback.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

