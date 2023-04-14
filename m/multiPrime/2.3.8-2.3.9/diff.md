# Comparing `tmp/multiPrime-2.3.8.tar.gz` & `tmp/multiPrime-2.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multiPrime-2.3.8.tar", last modified: Thu Apr 13 01:46:23 2023, max compression
+gzip compressed data, was "multiPrime-2.3.9.tar", last modified: Fri Apr 14 05:17:30 2023, max compression
```

## Comparing `multiPrime-2.3.8.tar` & `multiPrime-2.3.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-04-13 01:46:23.810859 multiPrime-2.3.8/
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)     1126 2023-02-16 10:00:29.000000 multiPrime-2.3.8/LICENSE
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    12955 2023-04-13 01:46:23.809859 multiPrime-2.3.8/PKG-INFO
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    12802 2023-02-21 06:44:43.000000 multiPrime-2.3.8/README.md
-drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-04-13 01:46:23.796857 multiPrime-2.3.8/multiPrime.egg-info/
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    12955 2023-04-13 01:46:23.000000 multiPrime-2.3.8/multiPrime.egg-info/PKG-INFO
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)      267 2023-04-13 01:46:23.000000 multiPrime-2.3.8/multiPrime.egg-info/SOURCES.txt
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)        1 2023-04-13 01:46:23.000000 multiPrime-2.3.8/multiPrime.egg-info/dependency_links.txt
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       52 2023-04-13 01:46:23.000000 multiPrime-2.3.8/multiPrime.egg-info/entry_points.txt
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       11 2023-04-13 01:46:23.000000 multiPrime-2.3.8/multiPrime.egg-info/top_level.txt
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       38 2023-04-13 01:46:23.810859 multiPrime-2.3.8/setup.cfg
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)     1795 2023-02-16 10:00:57.000000 multiPrime-2.3.8/setup.py
-drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-04-13 01:46:23.809859 multiPrime-2.3.8/src/
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       35 2023-02-16 10:00:29.000000 multiPrime-2.3.8/src/__init__.py
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       23 2023-04-13 01:45:57.000000 multiPrime-2.3.8/src/_version.py
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)     2402 2023-04-13 01:45:21.000000 multiPrime-2.3.8/src/main.py
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    84525 2023-04-13 01:45:21.000000 multiPrime-2.3.8/src/src.py
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    24918 2023-04-13 01:45:21.000000 multiPrime-2.3.8/src/utils.py
+drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-04-14 05:17:30.014961 multiPrime-2.3.9/
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)     1126 2023-02-16 10:00:29.000000 multiPrime-2.3.9/LICENSE
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    12953 2023-04-14 05:17:30.014961 multiPrime-2.3.9/PKG-INFO
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    12800 2023-04-14 05:12:54.000000 multiPrime-2.3.9/README.md
+drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-04-14 05:17:29.575922 multiPrime-2.3.9/multiPrime.egg-info/
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    12953 2023-04-14 05:17:26.000000 multiPrime-2.3.9/multiPrime.egg-info/PKG-INFO
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)      267 2023-04-14 05:17:26.000000 multiPrime-2.3.9/multiPrime.egg-info/SOURCES.txt
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)        1 2023-04-14 05:17:26.000000 multiPrime-2.3.9/multiPrime.egg-info/dependency_links.txt
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       52 2023-04-14 05:17:26.000000 multiPrime-2.3.9/multiPrime.egg-info/entry_points.txt
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       11 2023-04-14 05:17:26.000000 multiPrime-2.3.9/multiPrime.egg-info/top_level.txt
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       38 2023-04-14 05:17:30.014961 multiPrime-2.3.9/setup.cfg
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)     1795 2023-02-16 10:00:57.000000 multiPrime-2.3.9/setup.py
+drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-04-14 05:17:30.013960 multiPrime-2.3.9/src/
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       35 2023-02-16 10:00:29.000000 multiPrime-2.3.9/src/__init__.py
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       23 2023-04-14 05:17:21.000000 multiPrime-2.3.9/src/_version.py
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)     2402 2023-04-13 01:45:21.000000 multiPrime-2.3.9/src/main.py
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    84525 2023-04-13 01:45:21.000000 multiPrime-2.3.9/src/src.py
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    24918 2023-04-13 01:45:21.000000 multiPrime-2.3.9/src/utils.py
```

### Comparing `multiPrime-2.3.8/LICENSE` & `multiPrime-2.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `multiPrime-2.3.8/PKG-INFO` & `multiPrime-2.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: multiPrime
-Version: 2.3.8
+Version: 2.3.9
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # multiPrime
 
 `multiPrime is an error-tolerant primer design tool for broad-spectrum pathogens detection. 
-It proposes a solution for the minimum degeneracy degenerate primer design with error (MD-EDPD).` 
+It proposes a solution for the maximal coverage degenerate primer design with error (MD-EDPD).` 
 
 ## 1. Install
 
 > pip
 
 ```
 pip3 install multiPrime
@@ -93,15 +93,15 @@
 multiPrime Errors -i [input] -r [bowtie index] -l [150,2000] -p [10]-o [output]
 ```
 Parameters：
 
 | Parameters   | Description                                                                                                                |
 |--------------|----------------------------------------------------------------------------------------------------------------------------|
 | -i/--input   | input file: primer.fa.                                                                                                     |
-| -r/--ref     | reference file: bowtie index.                                                                                              |
+| -r/--ref     | reference file: the fasta of raw input.                                                                                    |
 | -l/--len     | Length of primer, which is used for mapping. Default: 18                                                                   |
 | -t/--term    | Position of mismatch is not allowed in the 3 term of primer. Default: 4                                                    |
 | -b/--bowtie  | bowtie or bowtie2 was employed for mapping. Default: bowtie2                                                               |
 | -m/--seedmms | Bowtie: Mismatches in seed (can be 0 - 3, default: -n 1).Bowtie2: Gap or mismatches in seed (can be 0 - 1, default: -n 1). |
 | -p/--process | Number of process to launch. Default: 20.                                                                                  |
 | -o/--out     | Output file: PCR product with primers.                                                                                     |
```

### Comparing `multiPrime-2.3.8/README.md` & `multiPrime-2.3.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # multiPrime
 
 `multiPrime is an error-tolerant primer design tool for broad-spectrum pathogens detection. 
-It proposes a solution for the minimum degeneracy degenerate primer design with error (MD-EDPD).` 
+It proposes a solution for the maximal coverage degenerate primer design with error (MD-EDPD).` 
 
 ## 1. Install
 
 > pip
 
 ```
 pip3 install multiPrime
@@ -85,15 +85,15 @@
 multiPrime Errors -i [input] -r [bowtie index] -l [150,2000] -p [10]-o [output]
 ```
 Parameters：
 
 | Parameters   | Description                                                                                                                |
 |--------------|----------------------------------------------------------------------------------------------------------------------------|
 | -i/--input   | input file: primer.fa.                                                                                                     |
-| -r/--ref     | reference file: bowtie index.                                                                                              |
+| -r/--ref     | reference file: the fasta of raw input.                                                                                    |
 | -l/--len     | Length of primer, which is used for mapping. Default: 18                                                                   |
 | -t/--term    | Position of mismatch is not allowed in the 3 term of primer. Default: 4                                                    |
 | -b/--bowtie  | bowtie or bowtie2 was employed for mapping. Default: bowtie2                                                               |
 | -m/--seedmms | Bowtie: Mismatches in seed (can be 0 - 3, default: -n 1).Bowtie2: Gap or mismatches in seed (can be 0 - 1, default: -n 1). |
 | -p/--process | Number of process to launch. Default: 20.                                                                                  |
 | -o/--out     | Output file: PCR product with primers.                                                                                     |
```

### Comparing `multiPrime-2.3.8/multiPrime.egg-info/PKG-INFO` & `multiPrime-2.3.9/multiPrime.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: multiPrime
-Version: 2.3.8
+Version: 2.3.9
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # multiPrime
 
 `multiPrime is an error-tolerant primer design tool for broad-spectrum pathogens detection. 
-It proposes a solution for the minimum degeneracy degenerate primer design with error (MD-EDPD).` 
+It proposes a solution for the maximal coverage degenerate primer design with error (MD-EDPD).` 
 
 ## 1. Install
 
 > pip
 
 ```
 pip3 install multiPrime
@@ -93,15 +93,15 @@
 multiPrime Errors -i [input] -r [bowtie index] -l [150,2000] -p [10]-o [output]
 ```
 Parameters：
 
 | Parameters   | Description                                                                                                                |
 |--------------|----------------------------------------------------------------------------------------------------------------------------|
 | -i/--input   | input file: primer.fa.                                                                                                     |
-| -r/--ref     | reference file: bowtie index.                                                                                              |
+| -r/--ref     | reference file: the fasta of raw input.                                                                                    |
 | -l/--len     | Length of primer, which is used for mapping. Default: 18                                                                   |
 | -t/--term    | Position of mismatch is not allowed in the 3 term of primer. Default: 4                                                    |
 | -b/--bowtie  | bowtie or bowtie2 was employed for mapping. Default: bowtie2                                                               |
 | -m/--seedmms | Bowtie: Mismatches in seed (can be 0 - 3, default: -n 1).Bowtie2: Gap or mismatches in seed (can be 0 - 1, default: -n 1). |
 | -p/--process | Number of process to launch. Default: 20.                                                                                  |
 | -o/--out     | Output file: PCR product with primers.                                                                                     |
```

### Comparing `multiPrime-2.3.8/setup.py` & `multiPrime-2.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `multiPrime-2.3.8/src/main.py` & `multiPrime-2.3.9/src/main.py`

 * *Files identical despite different names*

### Comparing `multiPrime-2.3.8/src/src.py` & `multiPrime-2.3.9/src/src.py`

 * *Files identical despite different names*

### Comparing `multiPrime-2.3.8/src/utils.py` & `multiPrime-2.3.9/src/utils.py`

 * *Files identical despite different names*

