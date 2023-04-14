# Comparing `tmp/dnadb-0.2.4.tar.gz` & `tmp/dnadb-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dnadb-0.2.4.tar", last modified: Fri Apr 14 00:21:08 2023, max compression
+gzip compressed data, was "dnadb-0.2.5.tar", last modified: Fri Apr 14 13:48:07 2023, max compression
```

## Comparing `dnadb-0.2.4.tar` & `dnadb-0.2.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-14 00:21:08.504082 dnadb-0.2.4/
--rw-r--r--   0 dwl2x     (1000) users      (100)     1070 2023-03-27 04:24:58.000000 dnadb-0.2.4/LICENSE
--rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-04-14 00:21:08.504082 dnadb-0.2.4/PKG-INFO
--rw-r--r--   0 dwl2x     (1000) users      (100)       43 2023-03-27 04:27:38.000000 dnadb-0.2.4/README.md
--rw-r--r--   0 dwl2x     (1000) users      (100)      712 2023-04-14 00:20:30.000000 dnadb-0.2.4/pyproject.toml
--rw-r--r--   0 dwl2x     (1000) users      (100)       38 2023-04-14 00:21:08.504082 dnadb-0.2.4/setup.cfg
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-14 00:21:08.504082 dnadb-0.2.4/src/
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-14 00:21:08.504082 dnadb-0.2.4/src/dnadb/
--rw-r--r--   0 dwl2x     (1000) users      (100)       22 2023-04-14 00:20:35.000000 dnadb-0.2.4/src/dnadb/__init__.py
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-14 00:21:08.504082 dnadb-0.2.4/src/dnadb/datasets/
--rw-r--r--   0 dwl2x     (1000) users      (100)      255 2023-03-27 05:49:34.000000 dnadb-0.2.4/src/dnadb/datasets/__init__.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     7303 2023-03-29 23:23:08.000000 dnadb-0.2.4/src/dnadb/datasets/dataset.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     1392 2023-04-03 19:22:40.000000 dnadb-0.2.4/src/dnadb/datasets/greengenes.py
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-14 00:21:08.504082 dnadb-0.2.4/src/dnadb/datasets/silva/
--rw-r--r--   0 dwl2x     (1000) users      (100)     5446 2023-03-29 23:23:47.000000 dnadb-0.2.4/src/dnadb/datasets/silva/__init__.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     6022 2023-03-27 05:43:12.000000 dnadb-0.2.4/src/dnadb/datasets/silva/taxonomy_map.py
--rw-r--r--   0 dwl2x     (1000) users      (100)      999 2023-04-12 05:30:41.000000 dnadb-0.2.4/src/dnadb/db.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     6027 2023-04-02 01:42:55.000000 dnadb-0.2.4/src/dnadb/dna.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     4773 2023-04-14 00:18:43.000000 dnadb-0.2.4/src/dnadb/fasta.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     6096 2023-04-14 00:19:30.000000 dnadb-0.2.4/src/dnadb/fastq.py
--rw-r--r--   0 dwl2x     (1000) users      (100)    14173 2023-04-14 00:20:19.000000 dnadb-0.2.4/src/dnadb/taxonomy.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     1473 2023-04-01 17:43:32.000000 dnadb-0.2.4/src/dnadb/utils.py
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-14 00:21:08.504082 dnadb-0.2.4/src/dnadb.egg-info/
--rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-04-14 00:21:08.000000 dnadb-0.2.4/src/dnadb.egg-info/PKG-INFO
--rw-r--r--   0 dwl2x     (1000) users      (100)      502 2023-04-14 00:21:08.000000 dnadb-0.2.4/src/dnadb.egg-info/SOURCES.txt
--rw-r--r--   0 dwl2x     (1000) users      (100)        1 2023-04-14 00:21:08.000000 dnadb-0.2.4/src/dnadb.egg-info/dependency_links.txt
--rw-r--r--   0 dwl2x     (1000) users      (100)       40 2023-04-14 00:21:08.000000 dnadb-0.2.4/src/dnadb.egg-info/requires.txt
--rw-r--r--   0 dwl2x     (1000) users      (100)        6 2023-04-14 00:21:08.000000 dnadb-0.2.4/src/dnadb.egg-info/top_level.txt
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-14 13:48:07.497718 dnadb-0.2.5/
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1070 2023-03-27 04:24:58.000000 dnadb-0.2.5/LICENSE
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-04-14 13:48:07.497718 dnadb-0.2.5/PKG-INFO
+-rw-r--r--   0 dwl2x     (1000) users      (100)       43 2023-03-27 04:27:38.000000 dnadb-0.2.5/README.md
+-rw-r--r--   0 dwl2x     (1000) users      (100)      712 2023-04-14 13:47:25.000000 dnadb-0.2.5/pyproject.toml
+-rw-r--r--   0 dwl2x     (1000) users      (100)       38 2023-04-14 13:48:07.497718 dnadb-0.2.5/setup.cfg
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-14 13:48:07.497718 dnadb-0.2.5/src/
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-14 13:48:07.497718 dnadb-0.2.5/src/dnadb/
+-rw-r--r--   0 dwl2x     (1000) users      (100)       22 2023-04-14 13:47:31.000000 dnadb-0.2.5/src/dnadb/__init__.py
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-14 13:48:07.497718 dnadb-0.2.5/src/dnadb/datasets/
+-rw-r--r--   0 dwl2x     (1000) users      (100)      255 2023-03-27 05:49:34.000000 dnadb-0.2.5/src/dnadb/datasets/__init__.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     7303 2023-03-29 23:23:08.000000 dnadb-0.2.5/src/dnadb/datasets/dataset.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1392 2023-04-03 19:22:40.000000 dnadb-0.2.5/src/dnadb/datasets/greengenes.py
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-14 13:48:07.497718 dnadb-0.2.5/src/dnadb/datasets/silva/
+-rw-r--r--   0 dwl2x     (1000) users      (100)     5492 2023-04-14 13:32:31.000000 dnadb-0.2.5/src/dnadb/datasets/silva/__init__.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     6022 2023-03-27 05:43:12.000000 dnadb-0.2.5/src/dnadb/datasets/silva/taxonomy_map.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)      999 2023-04-12 05:30:41.000000 dnadb-0.2.5/src/dnadb/db.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     6027 2023-04-02 01:42:55.000000 dnadb-0.2.5/src/dnadb/dna.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     4773 2023-04-14 00:18:43.000000 dnadb-0.2.5/src/dnadb/fasta.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     6096 2023-04-14 00:19:30.000000 dnadb-0.2.5/src/dnadb/fastq.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)    14173 2023-04-14 00:20:19.000000 dnadb-0.2.5/src/dnadb/taxonomy.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1473 2023-04-01 17:43:32.000000 dnadb-0.2.5/src/dnadb/utils.py
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-14 13:48:07.497718 dnadb-0.2.5/src/dnadb.egg-info/
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-04-14 13:48:07.000000 dnadb-0.2.5/src/dnadb.egg-info/PKG-INFO
+-rw-r--r--   0 dwl2x     (1000) users      (100)      502 2023-04-14 13:48:07.000000 dnadb-0.2.5/src/dnadb.egg-info/SOURCES.txt
+-rw-r--r--   0 dwl2x     (1000) users      (100)        1 2023-04-14 13:48:07.000000 dnadb-0.2.5/src/dnadb.egg-info/dependency_links.txt
+-rw-r--r--   0 dwl2x     (1000) users      (100)       40 2023-04-14 13:48:07.000000 dnadb-0.2.5/src/dnadb.egg-info/requires.txt
+-rw-r--r--   0 dwl2x     (1000) users      (100)        6 2023-04-14 13:48:07.000000 dnadb-0.2.5/src/dnadb.egg-info/top_level.txt
```

### Comparing `dnadb-0.2.4/LICENSE` & `dnadb-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dnadb-0.2.4/PKG-INFO` & `dnadb-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnadb
-Version: 0.2.4
+Version: 0.2.5
 Summary: A library for handling DNA files.
 Author-email: David Ludwig <davidludwigii@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 DLii-Research
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dnadb-0.2.4/pyproject.toml` & `dnadb-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dnadb"
-version = "0.2.4"
+version = "0.2.5"
 authors = [
   { name="David Ludwig", email="davidludwigii@gmail.com" },
 ]
 description = "A library for handling DNA files."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `dnadb-0.2.4/src/dnadb/datasets/dataset.py` & `dnadb-0.2.5/src/dnadb/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.2.4/src/dnadb/datasets/greengenes.py` & `dnadb-0.2.5/src/dnadb/datasets/greengenes.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.2.4/src/dnadb/datasets/silva/__init__.py` & `dnadb-0.2.5/src/dnadb/datasets/silva/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,32 +49,32 @@
         if not (self.path / self.fasta_file).exists() or force_download:
             self.__build_dna_fasta()
         if not (self.path / self.taxonomy_file).exists() or force_download:
             self.__build_taxonomy_map()
 
     def __build_dna_fasta(self):
         print("Converting FASTA to DNA...")
-        fasta_path = str(self.path / self.fasta_file)[:-3] # remove .gz extension
+        fasta_path = Path((self.path / self.fasta_file).stem) # remove .gz extension
+        fasta_path.parent.mkdir(exist_ok=True)
 
         def map_to_dna(entry: fasta.FastaEntry) -> fasta.FastaEntry:
             entry.sequence = to_dna(entry.sequence)
             return entry
         entry_iterator = fasta.entries(self.path / self.__rna_fasta_file)
         entry_iterator = map(map_to_dna, entry_iterator)
         with open(fasta_path, 'w') as file:
             fasta.write(file, entry_iterator)
 
         print("Compressing FASTA...")
         compress(fasta_path)
 
     def __build_taxonomy_map(self):
         print("Building taxonomy map...")
-
-        taxonomy_file_path = str(self.path / self.taxonomy_file)[:-3] # remove .gz extension
-        Path(taxonomy_file_path).parent.mkdir(exist_ok=True)
+        taxonomy_file_path = Path((self.path / self.taxonomy_file).stem) # remove .gz extension
+        taxonomy_file_path.parent.mkdir(exist_ok=True)
 
         input_taxonomy = open_file(self.path / self.__taxonomy_file, 'r')
         input_taxonomy_tree = open_file(self.path / self.__taxonomy_tree_file, 'r')
         input_taxonomy_map = open_file(self.path / self.__taxonomy_map_file, 'r')
         ouput_taxonomy = open(taxonomy_file_path, 'w')
 
         tax_dict = taxmap.make_taxid_dict(input_taxonomy)
```

### Comparing `dnadb-0.2.4/src/dnadb/datasets/silva/taxonomy_map.py` & `dnadb-0.2.5/src/dnadb/datasets/silva/taxonomy_map.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.2.4/src/dnadb/db.py` & `dnadb-0.2.5/src/dnadb/db.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.2.4/src/dnadb/dna.py` & `dnadb-0.2.5/src/dnadb/dna.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.2.4/src/dnadb/fasta.py` & `dnadb-0.2.5/src/dnadb/fasta.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.2.4/src/dnadb/fastq.py` & `dnadb-0.2.5/src/dnadb/fastq.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.2.4/src/dnadb/taxonomy.py` & `dnadb-0.2.5/src/dnadb/taxonomy.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.2.4/src/dnadb/utils.py` & `dnadb-0.2.5/src/dnadb/utils.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.2.4/src/dnadb.egg-info/PKG-INFO` & `dnadb-0.2.5/src/dnadb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnadb
-Version: 0.2.4
+Version: 0.2.5
 Summary: A library for handling DNA files.
 Author-email: David Ludwig <davidludwigii@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 DLii-Research
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

