# Comparing `tmp/dnadb-0.2.5.tar.gz` & `tmp/dnadb-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dnadb-0.2.5.tar", last modified: Fri Apr 14 13:48:07 2023, max compression
+gzip compressed data, was "dnadb-0.2.6.tar", last modified: Fri Apr 14 19:33:06 2023, max compression
```

## Comparing `dnadb-0.2.5.tar` & `dnadb-0.2.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-14 13:48:07.497718 dnadb-0.2.5/
--rw-r--r--   0 dwl2x     (1000) users      (100)     1070 2023-03-27 04:24:58.000000 dnadb-0.2.5/LICENSE
--rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-04-14 13:48:07.497718 dnadb-0.2.5/PKG-INFO
--rw-r--r--   0 dwl2x     (1000) users      (100)       43 2023-03-27 04:27:38.000000 dnadb-0.2.5/README.md
--rw-r--r--   0 dwl2x     (1000) users      (100)      712 2023-04-14 13:47:25.000000 dnadb-0.2.5/pyproject.toml
--rw-r--r--   0 dwl2x     (1000) users      (100)       38 2023-04-14 13:48:07.497718 dnadb-0.2.5/setup.cfg
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-14 13:48:07.497718 dnadb-0.2.5/src/
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-14 13:48:07.497718 dnadb-0.2.5/src/dnadb/
--rw-r--r--   0 dwl2x     (1000) users      (100)       22 2023-04-14 13:47:31.000000 dnadb-0.2.5/src/dnadb/__init__.py
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-14 13:48:07.497718 dnadb-0.2.5/src/dnadb/datasets/
--rw-r--r--   0 dwl2x     (1000) users      (100)      255 2023-03-27 05:49:34.000000 dnadb-0.2.5/src/dnadb/datasets/__init__.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     7303 2023-03-29 23:23:08.000000 dnadb-0.2.5/src/dnadb/datasets/dataset.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     1392 2023-04-03 19:22:40.000000 dnadb-0.2.5/src/dnadb/datasets/greengenes.py
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-14 13:48:07.497718 dnadb-0.2.5/src/dnadb/datasets/silva/
--rw-r--r--   0 dwl2x     (1000) users      (100)     5492 2023-04-14 13:32:31.000000 dnadb-0.2.5/src/dnadb/datasets/silva/__init__.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     6022 2023-03-27 05:43:12.000000 dnadb-0.2.5/src/dnadb/datasets/silva/taxonomy_map.py
--rw-r--r--   0 dwl2x     (1000) users      (100)      999 2023-04-12 05:30:41.000000 dnadb-0.2.5/src/dnadb/db.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     6027 2023-04-02 01:42:55.000000 dnadb-0.2.5/src/dnadb/dna.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     4773 2023-04-14 00:18:43.000000 dnadb-0.2.5/src/dnadb/fasta.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     6096 2023-04-14 00:19:30.000000 dnadb-0.2.5/src/dnadb/fastq.py
--rw-r--r--   0 dwl2x     (1000) users      (100)    14173 2023-04-14 00:20:19.000000 dnadb-0.2.5/src/dnadb/taxonomy.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     1473 2023-04-01 17:43:32.000000 dnadb-0.2.5/src/dnadb/utils.py
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-14 13:48:07.497718 dnadb-0.2.5/src/dnadb.egg-info/
--rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-04-14 13:48:07.000000 dnadb-0.2.5/src/dnadb.egg-info/PKG-INFO
--rw-r--r--   0 dwl2x     (1000) users      (100)      502 2023-04-14 13:48:07.000000 dnadb-0.2.5/src/dnadb.egg-info/SOURCES.txt
--rw-r--r--   0 dwl2x     (1000) users      (100)        1 2023-04-14 13:48:07.000000 dnadb-0.2.5/src/dnadb.egg-info/dependency_links.txt
--rw-r--r--   0 dwl2x     (1000) users      (100)       40 2023-04-14 13:48:07.000000 dnadb-0.2.5/src/dnadb.egg-info/requires.txt
--rw-r--r--   0 dwl2x     (1000) users      (100)        6 2023-04-14 13:48:07.000000 dnadb-0.2.5/src/dnadb.egg-info/top_level.txt
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-14 19:33:06.681676 dnadb-0.2.6/
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1070 2023-03-27 04:24:58.000000 dnadb-0.2.6/LICENSE
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-04-14 19:33:06.681676 dnadb-0.2.6/PKG-INFO
+-rw-r--r--   0 dwl2x     (1000) users      (100)       43 2023-03-27 04:27:38.000000 dnadb-0.2.6/README.md
+-rw-r--r--   0 dwl2x     (1000) users      (100)      712 2023-04-14 19:32:15.000000 dnadb-0.2.6/pyproject.toml
+-rw-r--r--   0 dwl2x     (1000) users      (100)       38 2023-04-14 19:33:06.681676 dnadb-0.2.6/setup.cfg
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-14 19:33:06.681676 dnadb-0.2.6/src/
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-14 19:33:06.681676 dnadb-0.2.6/src/dnadb/
+-rw-r--r--   0 dwl2x     (1000) users      (100)       22 2023-04-14 19:32:23.000000 dnadb-0.2.6/src/dnadb/__init__.py
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-14 19:33:06.681676 dnadb-0.2.6/src/dnadb/datasets/
+-rw-r--r--   0 dwl2x     (1000) users      (100)      255 2023-03-27 05:49:34.000000 dnadb-0.2.6/src/dnadb/datasets/__init__.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     7303 2023-03-29 23:23:08.000000 dnadb-0.2.6/src/dnadb/datasets/dataset.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1392 2023-04-03 19:22:40.000000 dnadb-0.2.6/src/dnadb/datasets/greengenes.py
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-14 19:33:06.681676 dnadb-0.2.6/src/dnadb/datasets/silva/
+-rw-r--r--   0 dwl2x     (1000) users      (100)     5492 2023-04-14 13:32:31.000000 dnadb-0.2.6/src/dnadb/datasets/silva/__init__.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     6022 2023-03-27 05:43:12.000000 dnadb-0.2.6/src/dnadb/datasets/silva/taxonomy_map.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)      999 2023-04-12 05:30:41.000000 dnadb-0.2.6/src/dnadb/db.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     6027 2023-04-02 01:42:55.000000 dnadb-0.2.6/src/dnadb/dna.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     4773 2023-04-14 00:18:43.000000 dnadb-0.2.6/src/dnadb/fasta.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     6096 2023-04-14 00:19:30.000000 dnadb-0.2.6/src/dnadb/fastq.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)    14308 2023-04-14 19:31:56.000000 dnadb-0.2.6/src/dnadb/taxonomy.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1473 2023-04-01 17:43:32.000000 dnadb-0.2.6/src/dnadb/utils.py
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-14 19:33:06.681676 dnadb-0.2.6/src/dnadb.egg-info/
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-04-14 19:33:06.000000 dnadb-0.2.6/src/dnadb.egg-info/PKG-INFO
+-rw-r--r--   0 dwl2x     (1000) users      (100)      502 2023-04-14 19:33:06.000000 dnadb-0.2.6/src/dnadb.egg-info/SOURCES.txt
+-rw-r--r--   0 dwl2x     (1000) users      (100)        1 2023-04-14 19:33:06.000000 dnadb-0.2.6/src/dnadb.egg-info/dependency_links.txt
+-rw-r--r--   0 dwl2x     (1000) users      (100)       40 2023-04-14 19:33:06.000000 dnadb-0.2.6/src/dnadb.egg-info/requires.txt
+-rw-r--r--   0 dwl2x     (1000) users      (100)        6 2023-04-14 19:33:06.000000 dnadb-0.2.6/src/dnadb.egg-info/top_level.txt
```

### Comparing `dnadb-0.2.5/LICENSE` & `dnadb-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dnadb-0.2.5/PKG-INFO` & `dnadb-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnadb
-Version: 0.2.5
+Version: 0.2.6
 Summary: A library for handling DNA files.
 Author-email: David Ludwig <davidludwigii@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 DLii-Research
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dnadb-0.2.5/pyproject.toml` & `dnadb-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dnadb"
-version = "0.2.5"
+version = "0.2.6"
 authors = [
   { name="David Ludwig", email="davidludwigii@gmail.com" },
 ]
 description = "A library for handling DNA files."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `dnadb-0.2.5/src/dnadb/datasets/dataset.py` & `dnadb-0.2.6/src/dnadb/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.2.5/src/dnadb/datasets/greengenes.py` & `dnadb-0.2.6/src/dnadb/datasets/greengenes.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.2.5/src/dnadb/datasets/silva/__init__.py` & `dnadb-0.2.6/src/dnadb/datasets/silva/__init__.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.2.5/src/dnadb/datasets/silva/taxonomy_map.py` & `dnadb-0.2.6/src/dnadb/datasets/silva/taxonomy_map.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.2.5/src/dnadb/db.py` & `dnadb-0.2.6/src/dnadb/db.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.2.5/src/dnadb/dna.py` & `dnadb-0.2.6/src/dnadb/dna.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.2.5/src/dnadb/fasta.py` & `dnadb-0.2.6/src/dnadb/fasta.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.2.5/src/dnadb/fastq.py` & `dnadb-0.2.6/src/dnadb/fastq.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.2.5/src/dnadb/taxonomy.py` & `dnadb-0.2.6/src/dnadb/taxonomy.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 from pathlib import Path
 import re
 from typing import Dict, Generator, Iterable, List, Optional, TextIO, Tuple, TypedDict, Set, Union
 
 from .db import DbFactory
 from .utils import open_file
 
-TAXON_PREFIXES = "kpcofgs"
+TAXON_LEVEL_NAMES = ("Kingdom", "Phylum", "Class", "Order", "Family", "Genus", "Species")
+TAXON_PREFIXES = ''.join(name[0] for name in TAXON_LEVEL_NAMES).lower()
 
 class TaxonHierarchyJson(TypedDict):
     parent_map: List[Dict[str, str]]
 
 # Utility Functions --------------------------------------------------------------------------------
 
 def split_taxonomy(taxonomy: str, max_depth: int = 7) -> Tuple[str, ...]:
```

### Comparing `dnadb-0.2.5/src/dnadb/utils.py` & `dnadb-0.2.6/src/dnadb/utils.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.2.5/src/dnadb.egg-info/PKG-INFO` & `dnadb-0.2.6/src/dnadb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnadb
-Version: 0.2.5
+Version: 0.2.6
 Summary: A library for handling DNA files.
 Author-email: David Ludwig <davidludwigii@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 DLii-Research
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

