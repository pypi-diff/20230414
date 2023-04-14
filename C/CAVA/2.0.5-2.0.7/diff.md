# Comparing `tmp/CAVA-2.0.5.tar.gz` & `tmp/CAVA-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CAVA-2.0.5.tar", last modified: Fri Feb 18 17:21:30 2022, max compression
+gzip compressed data, was "CAVA-2.0.7.tar", last modified: Wed Mar 23 20:01:01 2022, max compression
```

## Comparing `CAVA-2.0.5.tar` & `CAVA-2.0.7.tar`

### file list

```diff
@@ -1,43 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 17:21:30.125949 CAVA-2.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 17:21:30.121949 CAVA-2.0.5/CAVA.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      265 2022-02-18 17:21:29.000000 CAVA-2.0.5/CAVA.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      704 2022-02-18 17:21:30.000000 CAVA-2.0.5/CAVA.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-18 17:21:29.000000 CAVA-2.0.5/CAVA.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-18 17:21:28.000000 CAVA-2.0.5/CAVA.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-02-18 17:21:30.000000 CAVA-2.0.5/CAVA.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-02-18 17:21:30.000000 CAVA-2.0.5/CAVA.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1125 2022-02-18 17:21:17.000000 CAVA-2.0.5/LICENCE
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-02-18 17:21:17.000000 CAVA-2.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      265 2022-02-18 17:21:30.125949 CAVA-2.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3424 2022-02-18 17:21:17.000000 CAVA-2.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 17:21:30.125949 CAVA-2.0.5/cava/
--rw-r--r--   0 runner    (1001) docker     (121)     1564 2022-02-18 17:21:17.000000 CAVA-2.0.5/cava/CAVA.py
--rw-r--r--   0 runner    (1001) docker     (121)     1629 2022-02-18 17:21:17.000000 CAVA-2.0.5/cava/EnsemblDB.py
--rw-r--r--   0 runner    (1001) docker     (121)     1180 2022-02-18 17:21:17.000000 CAVA-2.0.5/cava/MANE.py
--rw-r--r--   0 runner    (1001) docker     (121)     1852 2022-02-18 17:21:17.000000 CAVA-2.0.5/cava/RefSeqDB.py
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-02-18 17:21:17.000000 CAVA-2.0.5/cava/VERSION
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-18 17:21:17.000000 CAVA-2.0.5/cava/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5464 2022-02-18 17:21:17.000000 CAVA-2.0.5/cava/dbSNPDB.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 17:21:30.125949 CAVA-2.0.5/cava/ensembldb/
--rw-r--r--   0 runner    (1001) docker     (121)     4194 2022-02-18 17:21:17.000000 CAVA-2.0.5/cava/ensembldb/README.md
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-18 17:21:17.000000 CAVA-2.0.5/cava/ensembldb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1826 2022-02-18 17:21:17.000000 CAVA-2.0.5/cava/ensembldb/customdb_prep.py
--rw-r--r--   0 runner    (1001) docker     (121)    27152 2022-02-18 17:21:17.000000 CAVA-2.0.5/cava/ensembldb/main.py
--rw-r--r--   0 runner    (1001) docker     (121)    27649 2022-02-18 17:21:17.000000 CAVA-2.0.5/cava/ensembldb/main_refseq.py
--rw-r--r--   0 runner    (1001) docker     (121)    27415 2022-02-18 17:21:17.000000 CAVA-2.0.5/cava/ensembldb/mane_db_prep.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 17:21:30.125949 CAVA-2.0.5/cava/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-18 17:21:17.000000 CAVA-2.0.5/cava/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8169 2022-02-18 17:21:17.000000 CAVA-2.0.5/cava/utils/conseq.py
--rw-r--r--   0 runner    (1001) docker     (121)    66793 2022-02-18 17:21:17.000000 CAVA-2.0.5/cava/utils/core.py
--rw-r--r--   0 runner    (1001) docker     (121)    48628 2022-02-18 17:21:17.000000 CAVA-2.0.5/cava/utils/csn.py
--rw-r--r--   0 runner    (1001) docker     (121)    25744 2022-02-18 17:21:17.000000 CAVA-2.0.5/cava/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (121)      344 2022-02-18 17:21:17.000000 CAVA-2.0.5/cava/utils/helper.py
--rw-r--r--   0 runner    (1001) docker     (121)    15476 2022-02-18 17:21:17.000000 CAVA-2.0.5/cava/utils/main.py
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-02-18 17:21:17.000000 CAVA-2.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-18 17:21:30.129949 CAVA-2.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      697 2022-02-18 17:21:17.000000 CAVA-2.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 17:21:30.125949 CAVA-2.0.5/test/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-18 17:21:17.000000 CAVA-2.0.5/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3897 2022-02-18 17:21:17.000000 CAVA-2.0.5/test/test.sh
--rw-r--r--   0 runner    (1001) docker     (121)    15264 2022-02-18 17:21:17.000000 CAVA-2.0.5/test/test_csn.py
--rw-r--r--   0 runner    (1001) docker     (121)     9515 2022-02-18 17:21:17.000000 CAVA-2.0.5/test/test_end2end.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 20:01:01.707938 CAVA-2.0.7/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 20:01:01.699938 CAVA-2.0.7/CAVA.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      329 2022-03-23 20:01:01.000000 CAVA-2.0.7/CAVA.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      889 2022-03-23 20:01:01.000000 CAVA-2.0.7/CAVA.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-23 20:01:01.000000 CAVA-2.0.7/CAVA.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-23 20:00:59.000000 CAVA-2.0.7/CAVA.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       80 2022-03-23 20:01:01.000000 CAVA-2.0.7/CAVA.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2022-03-23 20:01:01.000000 CAVA-2.0.7/CAVA.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1125 2022-03-23 20:00:46.000000 CAVA-2.0.7/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2022-03-23 20:00:46.000000 CAVA-2.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)      329 2022-03-23 20:01:01.707938 CAVA-2.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3650 2022-03-23 20:00:46.000000 CAVA-2.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 20:01:01.699938 CAVA-2.0.7/cava/
+-rw-r--r--   0 runner    (1001) docker     (121)     1564 2022-03-23 20:00:46.000000 CAVA-2.0.7/cava/CAVA.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6634 2022-03-23 20:00:46.000000 CAVA-2.0.7/cava/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (121)     1629 2022-03-23 20:00:46.000000 CAVA-2.0.7/cava/EnsemblDB.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1180 2022-03-23 20:00:46.000000 CAVA-2.0.7/cava/MANE.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1852 2022-03-23 20:00:46.000000 CAVA-2.0.7/cava/RefSeqDB.py
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2022-03-23 20:00:46.000000 CAVA-2.0.7/cava/VERSION
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-23 20:00:46.000000 CAVA-2.0.7/cava/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 20:01:01.703938 CAVA-2.0.7/cava/data/
+-rw-r--r--   0 runner    (1001) docker     (121)  1956028 2022-03-23 20:00:46.000000 CAVA-2.0.7/cava/data/cava_db.GRCh38.MANE.sorted.gz
+-rw-r--r--   0 runner    (1001) docker     (121)    73455 2022-03-23 20:00:46.000000 CAVA-2.0.7/cava/data/cava_db.GRCh38.MANE.sorted.gz.tbi
+-rwxr-xr-x   0 runner    (1001) docker     (121)   643426 2022-03-23 20:00:46.000000 CAVA-2.0.7/cava/data/cava_db.GRCh38.MANE.sorted.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     5464 2022-03-23 20:00:46.000000 CAVA-2.0.7/cava/dbSNPDB.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 20:01:01.703938 CAVA-2.0.7/cava/ensembldb/
+-rw-r--r--   0 runner    (1001) docker     (121)     4194 2022-03-23 20:00:46.000000 CAVA-2.0.7/cava/ensembldb/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-23 20:00:46.000000 CAVA-2.0.7/cava/ensembldb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1826 2022-03-23 20:00:46.000000 CAVA-2.0.7/cava/ensembldb/customdb_prep.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27152 2022-03-23 20:00:46.000000 CAVA-2.0.7/cava/ensembldb/main.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27649 2022-03-23 20:00:46.000000 CAVA-2.0.7/cava/ensembldb/main_refseq.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27414 2022-03-23 20:00:46.000000 CAVA-2.0.7/cava/ensembldb/mane_db_prep.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 20:01:01.703938 CAVA-2.0.7/cava/test/
+-rw-r--r--   0 runner    (1001) docker     (121)       47 2022-03-23 20:00:46.000000 CAVA-2.0.7/cava/test/CustomTX.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-23 20:00:46.000000 CAVA-2.0.7/cava/test/CustomTX2.txt
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2131 2022-03-23 20:00:46.000000 CAVA-2.0.7/cava/test/test.sh
+-rw-r--r--   0 runner    (1001) docker     (121)    15367 2022-03-23 20:00:46.000000 CAVA-2.0.7/cava/test/test_csn.py
+-rw-r--r--   0 runner    (1001) docker     (121)    43061 2022-03-23 20:00:46.000000 CAVA-2.0.7/cava/test/test_end2end.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-23 20:01:01.707938 CAVA-2.0.7/cava/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-23 20:00:46.000000 CAVA-2.0.7/cava/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8862 2022-03-23 20:00:46.000000 CAVA-2.0.7/cava/utils/conseq.py
+-rw-r--r--   0 runner    (1001) docker     (121)    96632 2022-03-23 20:00:46.000000 CAVA-2.0.7/cava/utils/core.py
+-rw-r--r--   0 runner    (1001) docker     (121)    96435 2022-03-23 20:00:46.000000 CAVA-2.0.7/cava/utils/csn.py
+-rw-r--r--   0 runner    (1001) docker     (121)    41107 2022-03-23 20:00:46.000000 CAVA-2.0.7/cava/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (121)      344 2022-03-23 20:00:46.000000 CAVA-2.0.7/cava/utils/helper.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16237 2022-03-23 20:00:46.000000 CAVA-2.0.7/cava/utils/main.py
+-rw-r--r--   0 runner    (1001) docker     (121)       84 2022-03-23 20:00:46.000000 CAVA-2.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-23 20:01:01.707938 CAVA-2.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      767 2022-03-23 20:00:46.000000 CAVA-2.0.7/setup.py
```

### Comparing `CAVA-2.0.5/LICENCE` & `CAVA-2.0.7/LICENCE`

 * *Files identical despite different names*

### Comparing `CAVA-2.0.5/README.md` & `CAVA-2.0.7/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -64,14 +64,20 @@
 # - or -
 git clone git@github.com:Steven-N-Hart/CAVA.git
 # optional to checkout release
 # e.g. git checkout v.1.2.4
 python setup.py install
 ```
 
+If you get an error with pycurl, run the following command before running the setup.py
+```bash
+pip uninstall pycurl
+export PYCURL_SSL_LIBRARY=nss
+pip install --compile --install-option="--with-nss" --no-cache-dir pycurl  
+```
 
 
 5 RUNNING CAVA
 --------------
 
 Before using CAVA, you will need to create a database of transcripts for which to base your annotations from.
 Details can be found in [this README](cava/ensembldb/README.md). In short, we reccomend using MANE transcripts,
```

### Comparing `CAVA-2.0.5/cava/CAVA.py` & `CAVA-2.0.7/cava/CAVA.py`

 * *Files identical despite different names*

### Comparing `CAVA-2.0.5/cava/EnsemblDB.py` & `CAVA-2.0.7/cava/EnsemblDB.py`

 * *Files identical despite different names*

### Comparing `CAVA-2.0.5/cava/MANE.py` & `CAVA-2.0.7/cava/MANE.py`

 * *Files identical despite different names*

### Comparing `CAVA-2.0.5/cava/RefSeqDB.py` & `CAVA-2.0.7/cava/RefSeqDB.py`

 * *Files identical despite different names*

### Comparing `CAVA-2.0.5/cava/dbSNPDB.py` & `CAVA-2.0.7/cava/dbSNPDB.py`

 * *Files identical despite different names*

### Comparing `CAVA-2.0.5/cava/ensembldb/README.md` & `CAVA-2.0.7/cava/ensembldb/README.md`

 * *Files identical despite different names*

### Comparing `CAVA-2.0.5/cava/ensembldb/customdb_prep.py` & `CAVA-2.0.7/cava/ensembldb/customdb_prep.py`

 * *Files identical despite different names*

### Comparing `CAVA-2.0.5/cava/ensembldb/main.py` & `CAVA-2.0.7/cava/ensembldb/main.py`

 * *Files identical despite different names*

### Comparing `CAVA-2.0.5/cava/ensembldb/main_refseq.py` & `CAVA-2.0.7/cava/ensembldb/main_refseq.py`

 * *Files identical despite different names*

### Comparing `CAVA-2.0.5/cava/ensembldb/mane_db_prep.py` & `CAVA-2.0.7/cava/ensembldb/mane_db_prep.py`

 * *Files 0% similar despite different names*

```diff
@@ -481,14 +481,15 @@
         download_gtf(source_compressed_gtf_ens, options.ensembl)
         download_gtf(source_compressed_gtf_ref, options.ensembl)
     except Exception as e:
         print('\n\nCannot connect to FTP site. No internet connection?\n')
         print(f'{e}\n{url}')
         exit(1)
 
+
     # Parse the entries & return the number of transcripts found
     genesdata = dict()
     transIDs = None
     enst_records = parse_gtf_loop(source_compressed_gtf_ens, options, genesdata, transIDs)
     print(f'Completed {enst_records} ENSEMBL records')
 
     genesdata = dict()
@@ -611,16 +612,14 @@
         try:
             wget.download(url)
             os.rename(os.path.basename(source_compressed_gtf), source_compressed_gtf)
 
         except Exception as e:
             print('\n\nCannot connect to FTP site, even after removing select. No internet connection?\n')
             print(f'{e}\n{url}')
-
-
     print('')
     sys.stdout.flush()
 
 
 def crossmap(source_compressed_gtf, output_dir):
     requests.packages.urllib3.util.ssl_.DEFAULT_CIPHERS += 'HIGH:!DH:!aNULL'  # Needed for UCSC
     # only download if necessary
```

### Comparing `CAVA-2.0.5/cava/utils/conseq.py` & `CAVA-2.0.7/cava/utils/conseq.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 #######################################################################################################################
 
 # Getting CLASS annotation of a given variant
 def getClassAnnotation(variant, transcript, protein, mutprotein, loc, ssrange):
     # Variants in UTR
     chkutr = checkUTR(transcript, variant)
     if chkutr == 'UTR5':
-        if 'Ex' in loc and (variant.isDeletion() or variant.isComplex()): return 'IM'
+        if 'Ex' in loc and (variant.is_deletion or variant.is_complex): return 'IM'
         return '5PU'
     elif chkutr == 'UTR3':
-        if 'Ex' in loc and (variant.isDeletion() or variant.isComplex()): return 'SL'
+        if 'Ex' in loc and (variant.is_deletion or variant.is_complex): return 'SL'
         return '3PU'
 
     # Variants crossing exon-intron boundaries
     if '-' in loc: return 'ESS'
 
     # Intronic, splice site and essential splice site variants
     if 'In' in loc:
@@ -37,43 +37,52 @@
         if potSS: return 'EE'
         return 'SY'
 
     # Variants affecting the initiation amino acid
     if protein[0] != mutprotein[0]: return 'IM'
 
     # Stop gain and stop lost variants
-    while len(protein) > 0 and len(mutprotein) > 0:
-        if protein[0] == mutprotein[0]:
-            protein = protein[1:]
-            mutprotein = mutprotein[1:]
+    # XXX-HS rewrote because this was the 3rd sink of time.
+    isame = -1
+    while len(protein) > isame+1 and len(mutprotein) > isame+1:
+        if protein[isame+1] == mutprotein[isame+1]:
+            isame = isame + 1
         else:
             break
+    if isame>=0:
+        protein = protein[isame+1:]
+        mutprotein = mutprotein[isame+1:]
+
 
     if protein == '': return '3PU'
 
     if protein[0] == 'X' and len(mutprotein) == 0: return 'SL'
     if protein[0] == 'X' and mutprotein[0] != 'X': return 'SL'
 
     if len(mutprotein) > 0 and \
             mutprotein[0] == 'X' and \
             len(protein) > 0 and \
             mutprotein[0] != protein[0] and \
-            not variant.isInFrame():
+            variant.is_in_frame is False:
         return 'SG'
 
     # Frame-shift coding variants
-    if not variant.isInFrame():
+    if variant.is_in_frame is False:
         return 'FS'
 
-    while len(protein) > 0 and len(mutprotein) > 0:
-        if protein[-1] == mutprotein[-1]:
-            protein = protein[:-1]
-            mutprotein = mutprotein[:-1]
+    # XXX-HS rewrote this section because it was 3rd slowest
+    ilast  = 0
+    while ilast<len(protein) and ilast<len(mutprotein) :
+        if protein[-(ilast+1)] == mutprotein[-(ilast+1)]:
+            ilast = ilast +1
         else:
             break
+    if ilast >0:
+        protein = protein[:-ilast]
+        mutprotein = mutprotein[:-ilast]
 
     if 'X' in mutprotein:
         return 'SG'
 
     # Non-synonymous coding variants
     if protL == mutprotL:
         if potSS:
@@ -93,18 +102,18 @@
 #######################################################################################################################
 
 
 def getSequenceOntologyAnnotation(variant, transcript, protein, mutprotein, loc):
     # Variants in UTR
     chkutr = checkUTR(transcript, variant)
     if chkutr == 'UTR5':
-        if 'Ex' in loc and (variant.isDeletion() or variant.isComplex()): return 'initiator_codon_variant'
+        if 'Ex' in loc and (variant.is_deletion or variant.is_complex): return 'initiator_codon_variant'
         return '5_prime_UTR_variant'
     elif chkutr == 'UTR3':
-        if 'Ex' in loc and (variant.isDeletion() or variant.isComplex()): return 'stop_lost'
+        if 'Ex' in loc and (variant.is_deletion or variant.is_complex): return 'stop_lost'
         return '3_prime_UTR_variant'
 
     where = transcript.whereIsThisVariant(variant)
 
     if '-' in where:
         first = where[:where.find('-')]
         if first.startswith('In'): return 'splice_acceptor_variant'
@@ -125,84 +134,101 @@
         if where.startswith('In') or where.startswith('fsIn'):
             return 'intron_variant|splice_region_variant'
         else:
             out.append('splice_region_variant')
 
     if where.startswith('In') or where.startswith('fsIn'): return 'intron_variant'
 
-    if variant.isInFrame():
-        if variant.isDeletion(): out.append('inframe_deletion')
-        if variant.isInsertion(): out.append('inframe_insertion')
-        if variant.isComplex():    out.append('inframe_indel')
+    if variant.is_in_frame is True:
+        if variant.is_deletion:
+            out.append('inframe_deletion')
+        if variant.is_insertion:
+            out.append('inframe_insertion')
+        if variant.is_complex:
+            out.append('inframe_indel')
     else:
         out.append('frameshift_variant')
         return '|'.join(out)
 
     if protein == mutprotein:
         out.append('synonymous_variant')
         return '|'.join(out)
 
     if protein[0] != mutprotein[0]:
         out.append('initiator_codon_variant')
         return '|'.join(out)
 
     if (not protein == mutprotein) and len(protein) == len(mutprotein): out.append('missense_variant')
 
-    while len(protein) > 0 and len(mutprotein) > 0:
-        if protein[0] == mutprotein[0]:
-            protein = protein[1:]
-            mutprotein = mutprotein[1:]
+    # XXX-HS rewrote because this was the 3rd sink of time.
+    isame = -1
+    while len(protein) > isame+1 and len(mutprotein) > isame+1:
+        if protein[isame+1] == mutprotein[isame+1]:
+            isame = isame + 1
         else:
             break
+    if isame>=0:
+        protein = protein[isame+1:]
+        mutprotein = mutprotein[isame+1:]
 
     if protein == '': return '3_prime_UTR_variant'
 
     if protein[0] == 'X' and len(mutprotein) == 0:
         out.append('stop_lost')
     else:
         if protein[0] == 'X' and mutprotein[0] != 'X': out.append('stop_lost')
 
-    while len(protein) > 0 and len(mutprotein) > 0:
-        if protein[-1] == mutprotein[-1]:
-            protein = protein[:-1]
-            mutprotein = mutprotein[:-1]
+# XXX rewrote because it was among top slowest parts of CAVA
+#
+
+    ilast  = 0
+    while ilast<len(protein) and ilast<len(mutprotein) :
+        if protein[-(ilast+1)] == mutprotein[-(ilast+1)]:
+            ilast = ilast +1
         else:
             break
+    if ilast >0:
+        protein = protein[:-ilast]
+        mutprotein = mutprotein[:-ilast]
 
     if 'X' in mutprotein: out.append('stop_gained')
 
     if ('stop_gained' in out) or ('stop_lost' in out):
         if 'missense_variant' in out: out.remove('missense_variant')
 
     return '|'.join(out)
 
 
 def isInSpliceDonor(transcript, variant):
     if transcript.strand == 1:
         for exon in transcript.exons:
             isLastExon = (exon.index == len(transcript.exons))
-            if not isLastExon and variant.overlap(exon.end + 1, exon.end + 2): return True
+            if not isLastExon and variant.overlap(exon.end + 1, exon.end + 2):
+                return True
         return False
     else:
         for exon in transcript.exons:
             isLastExon = (exon.index == len(transcript.exons))
-            if not isLastExon and variant.overlap(exon.start - 1, exon.start): return True
+            if not isLastExon and variant.overlap(exon.start - 1, exon.start):
+                return True
         return False
 
 
 def isInSpliceAcceptor(transcript, variant):
     if transcript.strand == 1:
         for exon in transcript.exons:
             isFirstExon = (exon.index == 1)
-            if not isFirstExon and variant.overlap(exon.start - 1, exon.start): return True
+            if not isFirstExon and variant.overlap(exon.start - 1, exon.start):
+                return True
         return False
     else:
         for exon in transcript.exons:
             isFirstExon = (exon.index == 1)
-            if not isFirstExon and variant.overlap(exon.end + 1, exon.end + 2): return True
+            if not isFirstExon and variant.overlap(exon.end + 1, exon.end + 2):
+                return True
 
         return False
 
 
 def isInSplicingRegion(transcript, variant):
     if transcript.strand == 1:
         for exon in transcript.exons:
@@ -219,15 +245,15 @@
             if not isFirstExon and variant.overlap(exon.end - 2, exon.end + 8): return True
         return False
 
 
 #######################################################################################################################
 
 def checkUTR(transcript, variant):
-    if variant.isInsertion():
+    if variant.is_insertion:
         x = variant.pos - 1
         y = variant.pos
     else:
         x = variant.pos
         y = variant.pos + len(variant.ref) - 1
     if transcript.isPositionOutsideCDS_5prime(x) or transcript.isPositionOutsideCDS_5prime(y): return 'UTR5'
     if transcript.isPositionOutsideCDS_3prime(x) or transcript.isPositionOutsideCDS_3prime(y): return 'UTR3'
```

### Comparing `CAVA-2.0.5/cava/utils/core.py` & `CAVA-2.0.7/cava/utils/core.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,126 +6,264 @@
 
 
 import gzip
 import logging
 import os
 import sys
 import time
+import re
+from . import csn
 
 
 #######################################################################################################################
 
 # Class representing a single variant call
 class Variant(object):
     # Constructor
-    def __init__(self, chrom, pos, ref, alt):
+    def __init__(self, chrom, pos, vcf_ref, vcf_alt):
+        vcf_ref = vcf_ref.upper()
+        vcf_alt = vcf_alt.upper()
         self.chrom = chrom
+        self.id = chrom + ":" + str(pos) + ":" + vcf_ref + "/" + vcf_alt
         self.pos = pos
-        self.ref = Sequence(ref)
-        self.alt = Sequence(alt)
-        shiftpos, a, b = self.trimCommonStart(self.ref, self.alt)
-        self.pos = self.pos + shiftpos
-        shiftpos, x, y = self.trimCommonEnd(a, b)
+        self.vcf_padded_base = ''
+        shift_pos, a, b = self.trimCommonStart(vcf_ref, vcf_alt)
+        self.pos = self.pos + shift_pos
+        shiftpos2, x, y = self.trimCommonEnd(a, b)
+        if (len(x) == 0 or len(y) == 0) and shift_pos > 0:
+            self.vcf_padded_base = vcf_ref[shift_pos - 1]
+
         self.ref = Sequence(x)
         self.alt = Sequence(y)
         self.flags = []
         self.flagvalues = []
+        self.alignonplus = None  # Cache the result of alignment because it is expensive and can be done many times.
+        self.alignonminus = None
+        lx = len(x)
+        ly = len(y)
+        if lx==1 and ly ==1:
+            self.is_substitution = True
+            self.is_deletion = False
+            self.is_insertion = False
+            self.is_complex = False
+            self.is_in_frame = True
+        elif lx==0 and ly>0:
+            self.is_substitution = False
+            self.is_deletion = False
+            self.is_insertion = True
+            self.is_complex = False
+            self.is_in_frame = ((lx -ly) % 3 == 0)
+        elif lx >0 and ly == 0:
+            self.is_substitution = False
+            self.is_deletion = True
+            self.is_insertion = False
+            self.is_complex = False
+            self.is_in_frame = ((lx - ly) % 3 == 0)
+        else:
+            self.is_substitution = False
+            self.is_deletion = False
+            self.is_insertion = False
+            self.is_complex = True
+            self.is_in_frame = ((lx - ly) % 3 == 0)
+        self.left_result = None
+        self.right_result = None
+        self.full_result = None
+
 
     # Getting basic information about variant
     def info(self):
         return self.getFullPosition() + '_' + self.ref + '>' + self.alt
 
     # Getting chromosome name and position combined
     def getFullPosition(self):
         return self.chrom + ':' + str(self.pos)
 
     # Checking if the variant is a base substitution
     def isSubstitution(self):
         return len(self.ref) == 1 and len(self.alt) == 1
 
     # Checking if the variant is an insertion
-    def isInsertion(self):
-        return len(self.ref) == 0 and len(self.alt) > 0
+    #def isInsertion(self):
+    #    return len(self.ref) == 0 and len(self.alt) > 0
 
     # Checking if the variant is a deletion
-    def isDeletion(self):
-        return len(self.ref) > 0 and len(self.alt) == 0
+    #def isDeletion(self):
+    #    return len(self.ref) > 0 and len(self.alt) == 0
 
-    # Checking if the variant is a complex indel
+    # Checking if the variant is a complex indel (pre-computed.. not used)
     def isComplex(self):
-        return len(self.ref) > 0 and len(self.alt) > 0 and not self.isSubstitution()
+        return len(self.ref) > 0 and len(self.alt) > 0 and not self.is_substitution
 
-    # Checking if the variant is in-frame
+
+    # Checking if the variant is in-frame (pre-computed .. not used)
     def isInFrame(self):
         return (len(self.alt) - len(self.ref)) % 3 == 0
 
     # Checking if the variant overlaps with a genomic region
     def overlap(self, start, end):
-        if self.isInsertion(): return (self.pos - 1 >= start) and (self.pos <= end)
-        int1_start = self.pos
-        int1_end = self.pos + len(self.ref) - 1
-        int2_start = start
-        int2_end = end
-        if int1_start == int2_start: return True
-        if int1_start > int2_start:
-            return int2_end >= int1_start
-        else:
-            return int1_end >= int2_start
+        if self.is_insertion:
+            return (self.pos - 1 >= start) and (self.pos <= end)
+        if self.pos > start:
+            return end >= self.pos
+        if self.pos == start:
+            return True
+        return self.pos + len(self.ref) - 1 >= start
 
     # Getting the value of a given annotation flag
     def getFlag(self, flag):
         return self.flagvalues[self.flags.index(flag)]
 
     # Adding annotation flag to variant
     def addFlag(self, flag, value):
         self.flags.append(flag)
         self.flagvalues.append(value)
 
     # Annotating variant
     def annotate(self, ensembl, dbsnp, reference, impactdir):
         self.annotateWithType()
-        if not ensembl is None: self = ensembl.annotate(self, reference, impactdir)
-        if not dbsnp is None: dbsnp.annotate(self)
+        if ensembl is not None:
+            self = ensembl.annotate(self, reference, impactdir)
+        if dbsnp is not None:
+            dbsnp.annotate(self)
 
     # Annotating variant with its type
     def annotateWithType(self):
-        if self.isSubstitution(): self.addFlag('TYPE', 'Substitution')
-        if self.isInsertion(): self.addFlag('TYPE', 'Insertion')
-        if self.isDeletion(): self.addFlag('TYPE', 'Deletion')
-        if self.isComplex(): self.addFlag('TYPE', 'Complex')
+        if self.is_substitution:
+            self.addFlag('TYPE', 'Substitution')
+        elif self.is_insertion:
+            self.addFlag('TYPE', 'Insertion')
+        elif self.is_deletion:
+            self.addFlag('TYPE', 'Deletion')
+        elif self.is_complex:
+            self.addFlag('TYPE', 'Complex')
+
+    def remove_same_bases_ref_alt(self):  # Only apply for SNV or MNP with padded bases to remove.
+        if self.is_substitution or self.is_insertion or self.is_deletion:
+            return [self.pos, self.ref, self.alt]
+        if self.ref == self.alt:
+            return [self.pos, self.ref[0], self.alt[0]]
+        left, seq1, seq2 = self.trimCommonStart(self.ref, self.alt)
+        right, newref, newalt = self.trimCommonEnd(seq1, seq2)
+        return [self.pos + left, newref, newalt]
 
-    # Aligning variant on the plus strand
+    # Aligning variant on the GENOMIC plus strand, shifting 3' (right) on DNA (NOT cDNA)
     def alignOnPlusStrand(self, reference):
-        seq1 = reference.getReference(self.chrom, self.pos, self.pos + len(self.ref) - 1 + 100)
-        seq2 = self.alt + reference.getReference(self.chrom, self.pos + len(self.ref),
-                                                 self.pos + len(self.ref) + 100 - 1)
-        left, seq1, seq2 = self.rightAlign(seq1, seq2)
-        if len(seq1) == 0 or len(seq2) == 0:
-            left -= 1
-            base = reference.getReference(self.chrom, self.pos + left, self.pos + left)
+        if self.alignonplus is not None:
+            return self.alignonplus
+        if self.chrom not in reference.reflens or not (self.is_insertion or self.is_deletion):
+            [self.pos, self.ref, self.alt] = self.remove_same_bases_ref_alt()  # Trime redundant bases from SNP/MNP
+            self.alignononplus = self
+            return self
+        reflen = reference.reflens[self.chrom]
+        maxreplen = abs(len(self.ref)-len(self.alt))
+        PADLEN = max(100,1+5*maxreplen) # the bigger the repeat, the less likely there are multiple exact copies, so 5 is OKfSequence
+#        seq1_0 = reference.getReference(self.chrom, self.pos, self.pos + len(self.ref) - 1 + PADLEN)
+#        seq2_0 = self.alt + reference.getReference(self.chrom, self.pos + len(self.ref),
+#                                                 self.pos + len(self.ref) + PADLEN - 1)
+        maxpos = self.pos + len(self.ref) - 1 + PADLEN
+        if maxpos > reflen:
+            maxpos = reflen
+        EXTRA_PREBASE = 1
+        if self.pos == 1:
+            EXTRA_PREBASE = 0
+        seq12_0 = reference.getReference(self.chrom, self.pos-EXTRA_PREBASE, maxpos)
+        seq1_0 = seq12_0[EXTRA_PREBASE:]
+        seq2_0 = self.alt+seq12_0[len(self.ref)+EXTRA_PREBASE:]
+        left, seq1, seq2 = self.rightAlign(seq1_0, seq2_0)
+        while left >= PADLEN - (maxreplen -  1) and maxpos!=reflen:  # Shifted almost all the way to the end, make sure there is not more to shift
+            PADLEN += PADLEN
+            maxpos = self.pos + len(self.ref) - 1 + PADLEN
+            if maxpos > reflen:
+                maxpos = reflen
+#            seq1_0 = reference.getReference(self.chrom, self.pos, maxpos)
+#            seq2_0 = self.alt + reference.getReference(self.chrom, self.pos + len(self.ref),
+#                                                       self.pos + len(self.ref) + PADLEN - 1)
+            seq12_0 = reference.getReference(self.chrom, self.pos-EXTRA_PREBASE, maxpos)
+            seq1_0 = seq12_0[EXTRA_PREBASE:]
+            seq2_0 = seq12_0[len(self.ref)+EXTRA_PREBASE:]
+            left, seq1, seq2 = self.rightAlign(seq1_0, seq2_0)
+
+        base = ''
+        if len(seq1) == 0 or len(seq2) == 0:  # e.g. if insertion/deletion .. should always be the case
+            if (left >= 1 and EXTRA_PREBASE == 1):
+                # base = reference.getReference(self.chrom, self.pos + left, self.pos + left)
+                base = seq12_0[left]
+            elif left == 0 and EXTRA_PREBASE == 1:
+                base = seq12_0[0]
+            else:  # Variant on First base of chrom (currently only Mitochorndria has first base not an 'N')
+                base = ""
             seq1, seq2 = base + seq1, base + seq2
-        ret = Variant(self.chrom, self.pos + left, seq1, seq2)
+        ret = Variant(self.chrom, self.pos + left-len(base), seq1, seq2)  # have to use VCF padded coordinates
         ret.flags = self.flags
-        ret.flagvalues = self.flagvalues
+        self_flagvalues = self.flagvalues
+        ret.flagvalues = self_flagvalues
+        self.alignonplus = ret
         return ret
 
     # Aligning variant on the minus strand
     def alignOnMinusStrand(self, reference):
-        seq1 = reference.getReference(self.chrom, self.pos - 100, self.pos + len(self.ref) - 1)
-        s = reference.getReference(self.chrom, self.pos - 100, self.pos - 1)
-        seq2 = s + self.alt
+        if self.alignonminus is not None:
+            return self.alignonminus
+        if self.pos == 1 or (self.chrom not in reference.reflens or not (self.is_insertion or self.is_deletion)):
+            [self.pos, self.ref, self.alt] = self.remove_same_bases_ref_alt()
+            self.alignonminus = self
+            return self
+        else:
+            if self.is_insertion:
+                if not len(self.vcf_padded_base) == 0:
+                    if self.vcf_padded_base[0] != self.alt[-1]:  # See if there is the potential for another copy of the alt allele
+                        self.alignonminus = self
+                        return self
+            elif self.is_deletion:
+                if not len(self.vcf_padded_base) == 0:  # Skip cases where initial VCF was invalid and did not have pre-base as can happen after splitting multiple alleles
+                    if self.vcf_padded_base[0] != self.ref[-1]:
+                        self.alignonminus = self
+                        return self
+
+        reflen = reference.reflens[self.chrom]
+
+        maxreplen = abs(len(self.ref)-len(self.alt))
+        PADLEN = max(100,1+5*maxreplen)
+        if self.pos - PADLEN<1:
+            PADLEN = self.pos -1
+        seq1_0 = reference.getReference(self.chrom, self.pos - PADLEN, self.pos + len(self.ref) - 1)
+        #s = reference.getReference(self.chrom, self.pos - PADLEN, self.pos - 1)
+        s = seq1_0[0:PADLEN]
+        seq2_0 = s + self.alt
         N = len(s)
-        left, seq1, seq2 = self.leftAlign(seq1, seq2)
+        left, seq1, seq2 = self.leftAlign(seq1_0, seq2_0)
+        while left <= maxreplen and self.pos-PADLEN > 0:  # Shifted  all the way to the beginning, make sure there is not more to shift
+            PADLEN += PADLEN
+            if self.pos - PADLEN < 1:  # This will only occur for Mitochondria
+                PADLEN = self.pos-1
+            seq1_0 = reference.getReference(self.chrom, self.pos - PADLEN, self.pos + len(self.ref) - 1)
+            #s = reference.getReference(self.chrom, self.pos - PADLEN, self.pos - 1)
+            s = seq1_0[0:PADLEN]
+            seq2_0 = s + self.alt
+            left, seq1, seq2 = self.leftAlign(seq1_0, seq2_0)
+            N = len(s)
+
         if len(seq1) == 0 or len(seq2) == 0:
-            left = left - 1
-            base = reference.getReference(self.chrom, self.pos + left - N, self.pos + left - N)
+            # Unless Variant got shifted all the way to position 1(left==0), there should be enough bases for padding.
+            if left > 0:
+                left = left - 1
+                #            base = reference.getReference(self.chrom, self.pos + left - PADLEN, self.pos + left - PADLEN)
+                base = seq1_0[left]  # if eliminate 1st common base, take seq1_0[0] ..etc
+            else:  # left == 0 means no shared bases in chunk, so it means variant fills the chunk .. all the way to the first base
+                base = ''
             seq1, seq2 = base + seq1, base + seq2
+        else:
+            sys.stderr.write(
+                "WARNING: Attempted to left shift non-indel variant .. bug? for variant:" + self.id + "\n")
+
+
         ret = Variant(self.chrom, self.pos + left - N, seq1, seq2)
         ret.flags = self.flags
         ret.flagvalues = self.flagvalues
+        self.alignonminus = ret
         return ret
 
     # Right-aligning two sequences
     def rightAlign(self, seq1, seq2):
         left, seq1, seq2 = self.trimCommonStart(seq1, seq2)
         right, seq1, seq2 = self.trimCommonEnd(seq1, seq2)
         return left, seq1, seq2
@@ -136,266 +274,412 @@
         left, seq1, seq2 = self.trimCommonStart(seq1, seq2)
         return left, seq1, seq2
 
     # Trimming common starting subsequence of two sequences
     def trimCommonStart(self, s1, s2):
         counter = 0
         while True:
-            if len(s1) == 0 or len(s2) == 0: return counter, s1, s2
-            if s1[0] != s2[0]: return counter, s1, s2
-            s1, s2 = s1[1:], s2[1:]
+            if len(s1)<= counter or len(s2) <=counter or s1[counter] != s2[counter]:
+                return counter, s1[counter:], s2[counter:]
+            #s1, s2 = s1[1:], s2[1:]
             counter += 1
 
     # Trimming common ending subsequence of two sequences
     def trimCommonEnd(self, s1, s2):
-        counter = 0
+        counter = 1
+        if len(s1) == 0 or len(s2) ==0 or (s1[-1]!=s2[-1]):
+            return 0, s1, s2
         while True:
-            if len(s1) == 0 or len(s2) == 0: return counter, s1, s2
-            if s1[-1] != s2[-1]: return counter, s1, s2
-            s1, s2 = s1[:-1], s2[:-1]
+            if counter > len(s1) or counter > len(s2):  # implicitely counter != 1
+                return counter-1, s1[:-(counter-1)], s2[:-(counter-1)]
+            if s1[-counter] != s2[-counter]:
+                    return counter-1, s1[:-(counter-1)], s2[:-(counter-1)]
             counter += 1
 
 
+
 #######################################################################################################################
+def trim_all_alleles(ref,alts): # This is a VCF-style trimming, must leave 1 base
+    ntrim = 0
+    if len(ref)==1:
+        return 0
+    for ir in range(0, len(ref)-1):
+        refbase = ref[ir]
+        for ia in range(0, len(alts)): # loop over alleles
+            if ntrim >= len(alts[ia])-1:  # Don't trim to the point of leaving empty alleles
+                return ntrim
+            if refbase != alts[ia][ir]:
+                return ntrim
+        ntrim = ntrim +1
+    return ntrim
+
+
 
 # Class representing a single VCF record     
 class Record(object):
     # Constructor
-    def __init__(self, line, options, targetBED):
+    def __init__(self, line, options, targetBED, reference):
 
         self.targetBED = targetBED
-
+        # Reference genome pysam/tabix object
+        self.reference = reference
         # Parsing VCF format
+        if 'build' in options.args:
+            self.build = options.args['build']
+        else:
+            self.build = 'GRCh38'
         if options.args['inputformat'].upper() == 'VCF':
             cols = line.strip().split("\t")
             self.chrom = cols[0]
 
             if self.chrom.startswith('chr'):
                 self.chrom_chr_prefix = True
                 self.chrom = self.chrom[3:]
             else:
                 self.chrom_chr_prefix = False
 
             self.pos = int(cols[1])
             self.id = cols[2]
             self.ref = cols[3]
             alts = cols[4].split(",")
-            self.alts = []
             self.qual = cols[5]
             self.filter = cols[6]
             if len(cols) > 7:
                 self.info = cols[7]
             else:
                 self.info = ''
             if len(cols) > 8:
                 self.rest = cols[8:]
             else:
                 self.rest = []
-
-        # Parsing TXT format
-        if options.args['inputformat'].upper() == 'TXT':
+        elif options.args['inputformat'].upper() == 'TXT':  # Parsing TXT format
             cols = line.strip().split("\t")
             self.id = cols[0]
             self.chrom = cols[1]
             self.pos = int(cols[2])
             self.ref = cols[3]
-            self.alts = []
             alts = cols[4].split(",")
+
             self.qual = ''
             self.filter = 'PASS'
             self.info = ''
             self.rest = []
+        else:
+            raise Exception("Invalid Input format type")
 
-        # Creating a Variant object for each variant call in the record
+        altsclean = []
+        for alt in alts:
+            if not alt.startswith('<'):
+                altsclean.append(alt)
+        # Creating a Variant object for each variant/alt-allele  in the record
+        # as long as they pass filtering.
+        #
+        # Trim only if all alleles have an extra base.. but this really should be done by a normalizing code
+        # And one should really remove all ale alleles.
         self.variants = []
+        self.alts = []
+        in_target_region = False
+
+        ntrim = trim_all_alleles(self.ref,altsclean)
+        if ntrim > 0:
+            self.ref = self.ref[ntrim:]
+            self.pos += ntrim
+            for ia in range(0,len(alts)):
+                alt = alts[ia]
+                if not alt.startswith('<'):
+                    alts[ia] = alts[ia][ntrim:]
+
         for alt in alts:
+            # Keep original alt alleles because each alt-allele may normalize differently and have different positions
+            self.alts.append(alt)
             # Initializing each Variant object with different alt allele
-            var = Variant(self.chrom, self.pos, self.ref, alt)
-            # DO  NOT FILTER
-            """
-            if 'N' in self.ref or 'N' in alt:
-                logging.info('Variant ignored as allele contains unknown base (\'N\'): ' + self.chrom + ':' + str(
-                    self.pos) + ' ' + self.ref + '>' + alt)
-                continue
-           
-            if alt == '.':
-                logging.info("Variant ignored because it is monomorphic reference: " + self.chrom + ':' + str(
-                    self.pos) + ' ' + self.ref + '>' + alt)
-                continue
+            if alt.startswith('<'):
+                var = None
+            else:
+                var = Variant(self.chrom, self.pos, self.ref, alt)
 
-            if not alt.strip('ACGT') is '' or not self.ref.strip('ACGT') is '':
-                logging.info("Variant ignored as format of alt allele is not supported: " + self.chrom + ':' + str(
-                    self.pos) + ' ' + self.ref + '>' + alt)
-                continue
-            """
-            # Filtering by variant type (i.e. substitution, indel, insertion, deletion, complex indel), if required
-            if options.args['type'].upper() == 'SUBSTITUTION' and not var.isSubstitution():
-                continue
-            if options.args[
-                'type'].upper() == 'INDEL' and not var.isInsertion() and not var.isDeletion() and not var.isComplex():
-                continue
-            if options.args['type'].upper() == 'INSERTION' and not var.isInsertion():
-                continue
-            if options.args['type'].upper() == 'DELETION' and not var.isDeletion():
-                continue
-            if options.args['type'].upper() == 'COMPLEX' and not var.isComplex():
-                continue
+                # DO  NOT FILTER
+                """
+                if 'N' in self.ref or 'N' in alt:
+                    logging.info('Variant ignored as allele contains unknown base (\'N\'): ' + self.chrom + ':' + str(
+                        self.pos) + ' ' + self.ref + '>' + alt)
+                    continue
+               
+                if alt == '.':
+                    logging.info("Variant ignored because it is monomorphic reference: " + self.chrom + ':' + str(
+                        self.pos) + ' ' + self.ref + '>' + alt)
+                    continue
+    
+                if not alt.strip('ACGT') is '' or not self.ref.strip('ACGT') is '':
+                    logging.info("Variant ignored as format of alt allele is not supported: " + self.chrom + ':' + str(
+                        self.pos) + ' ' + self.ref + '>' + alt)
+                    continue
+                """
+                # Filtering by variant type (i.e. substitution, indel, insertion, deletion, complex indel), if required
+                # Filtering via those options is NOT recommended, especially when dealing with multiple alt-alleles.
+
+                if options.args['type'].upper() == 'SUBSTITUTION' and not var.is_substitution:
+                    continue
+                if options.args['type'].upper() == 'INDEL' and not var.is_insertion and not var.is_deletion \
+                        and not var.is_complex:
+                    continue
+                if options.args['type'].upper() == 'INSERTION' and not var.is_insertion:
+                    continue
+                if options.args['type'].upper() == 'DELETION' and not var.is_deletion:
+                    continue
+                if options.args['type'].upper() == 'COMPLEX' and not var.is_complex:
+                    continue
+                # Adding Variant object to this record
+                # 10/2021-New benavior, adding all alt-alleles variants if any of the alleles is in the target region .. and is not explicitely filtered out by type
+                # The logic is that the user should be able to decide which variant has the best support in the sequencing data (read count)
+                # .. and not be biased by the most deleterious option.
+                # At least 1 must pass the BED filtering - if requested (otherwise all alt-alleles (whole variant) are excluded)
+            self.variants.append(var)
 
             # Filtering by BED file, if required
-            if not targetBED is None:
-                goodchrom = var.chrom
-                if not goodchrom in targetBED.contigs:
-                    goodchrom = 'chr' + goodchrom
-                    if not goodchrom in targetBED.contigs: continue
-                if not var.isInsertion():
-                    start = var.pos
+            if targetBED is not None and var is not None:
+                goodchrom = convert_chrom(var.chrom+"", targetBED.contigs)
+                if goodchrom is None:
+                    continue
+                if not var.is_insertion:
+                    start = var.pos - 1  # correct for 0-base
                     end = var.pos + len(var.ref) - 1
                 else:
-                    start = var.pos - 1
+                    start = var.pos - 2 # correct for insertion AND 0-base
                     end = var.pos
                 foundstart = False
-                for _ in self.targetBED.fetch(region=goodchrom + ':' + str(start) + '-' + str(start)): foundstart = True
+                for _ in self.targetBED.fetch(region=goodchrom + ':' + str(start) + '-' + str(start)):
+                    foundstart = True
                 foundend = False
-                for _ in self.targetBED.fetch(region=goodchrom + ':' + str(end) + '-' + str(end)): foundend = True
-                if not (foundstart and foundend): continue
+                for _ in self.targetBED.fetch(region=goodchrom + ':' + str(end) + '-' + str(end)):
+                    foundend = True
+                if not (foundstart or foundend):
+                    if not (var.is_deletion or var.is_insertion):
+                        continue  # No shifting possible, so definitively outside bed region.
+                    else:
+                        var_plus = var.alignOnPlusStrand(self.reference)
+                        var_minus = var.alignOnMinusStrand(self.reference)
+                        if var_plus.pos == var_minus.pos:  # No change, so no shifting
+                            continue
+                        else:
+                            if not var_plus.is_insertion:
+                                start = var_plus.pos -1 # correct for -base
+                                end = var_plus.pos + len(var_plus.ref) - 1
+                            else:
+                                start = var_plus.pos - 2 # correct for insertion and 0-base
+                                end = var_plus.pos
+                            foundstart = False
+                            for _ in self.targetBED.fetch(region=goodchrom + ':' + str(start) + '-' + str(start)):
+                                foundstart = True
+                            foundend = False
+                            for _ in self.targetBED.fetch(region=goodchrom + ':' + str(end) + '-' + str(end)):
+                                foundend = True
+                            if not (foundstart or foundend):
+                                if not var_minus.is_insertion:
+                                    start = var_minus.pos -1  # correct for 0-base
+                                    end = var_minus.pos + len(var_minus.ref) - 1
+                                else:
+                                    start = var_minus.pos - 2 # correct for 0-base and insertion
+                                    end = var_minus.pos
+                                foundstart = False
+                                for _ in self.targetBED.fetch(region=goodchrom + ':' + str(start) + '-' + str(start)): foundstart = True
+                                foundend = False
+                                for _ in self.targetBED.fetch(region=goodchrom + ':' + str(end) + '-' + str(end)): foundend = True
+                                if not (foundstart or foundend):
+                                    continue
+                in_target_region = True
+            else:
+                in_target_region = True
 
-            # Adding Variant object to this record
-            self.variants.append(var)
-            self.alts.append(alt)
+        if in_target_region is False:
+            self.variants = []
 
     # Annotating record
     def annotate(self, ensembl, dbsnp, reference, impactdir):
         # Annotating each variant in the record
         for variant in self.variants:
-            variant.annotate(ensembl, dbsnp, reference, impactdir)
+            if variant is not None:
+                variant.annotate(ensembl, dbsnp, reference, impactdir)
+                if variant.alignonplus is not None:
+                    variant.addFlag('HGVSg', csn.get_genomic_Annotation(variant.alignonplus, self.build ,reference))
+                else:
+                    variant.addFlag('HGVSg', csn.get_genomic_Annotation(variant, self.build, reference))
 
     # Writing record (a ref, multiple alts) to output file
     def output(self, outformat, outfile, options, genelist, transcriptlist, snplist, stdout):
         outvariants = []
         outalts = []
+        build = "GRCh38"
+        if "build" in options.args:
+            build = options.args["build"]
+
         # Values of Entries for Separate Alleles are separated by ','
         # Entries for Multiple transcripts (for 1 allele) are separated by ':'
+        #  This allows each allele to have different transcripts
+        #  (for multiple allele, shifting may lead to different alleles in shifted vs non-shifted alt-alleles)
 
         for i in range(len(self.variants)):
             variant = self.variants[i]
-            alt = self.alts[i]
-
-            isTRANSCRIPT = ('TRANSCRIPT' in variant.flags)
-            if isTRANSCRIPT:
-                annTRANSCRIPT = variant.flagvalues[variant.flags.index('TRANSCRIPT')]
-            else:
-                annTRANSCRIPT = ''
-            isDBSNP = ('DBSNP' in variant.flags)
-            if isDBSNP:
-                annDBSNP = variant.flagvalues[variant.flags.index('DBSNP')]
+            if variant is None:
+                outalts.append(self.alts[i])
             else:
-                annDBSNP = ''
+                isTRANSCRIPT = ('TRANSCRIPT' in variant.flags)
+                if isTRANSCRIPT:
+                    annTRANSCRIPT = variant.flagvalues[variant.flags.index('TRANSCRIPT')]
+                else:
+                    annTRANSCRIPT = ''
+                isDBSNP = ('DBSNP' in variant.flags)
+                if isDBSNP:
+                    annDBSNP = variant.flagvalues[variant.flags.index('DBSNP')]
+                else:
+                    annDBSNP = ''
 
-            if len(genelist) > 0 or len(transcriptlist) > 0:
-                if annTRANSCRIPT == '': continue
+                if len(genelist) > 0 or len(transcriptlist) > 0:
+                    if annTRANSCRIPT == '':
+                        continue
+
+                # Removing non-annotated variants/alleles, if required
+                if 'nonannot' in options.args and options.args['nonannot'] is False and \
+                        not ((isTRANSCRIPT and not annTRANSCRIPT == '') or (isDBSNP and not annDBSNP == '')):
+                    continue
 
-            # Removing non-annotated variants, if required
-            if not options.args['nonannot'] and not (
-                    (isTRANSCRIPT and not annTRANSCRIPT == '') or (isDBSNP and not annDBSNP == '')):
-                continue
+                # Filtering by gene, transcript or snp list, if required
+                if isDBSNP:
+                    if len(snplist) > 0 and annDBSNP not in snplist: continue
 
-            # Filtering by gene, transcript or snp list, if required
-            if isDBSNP:
-                if len(snplist) > 0 and annDBSNP not in snplist: continue
 
-            outvariants.append(variant)
-            outalts.append(alt)
+                outvariants.append(variant)
+                outalts.append(self.alts[i])  # Original Alts.
 
-        # Skipping record if all variants have been removed
-        if len(outvariants) == 0: return
+        # Skipping record if all alt-allelic variants have been removed
+        if len(outvariants) == 0 or len(outalts)==1 and outalts[0].startswith("<"):
+            return
 
         # Writing output in VCF format
         if outformat.upper() == 'VCF':
+            infos = self.info.split(';')
+            newinfos = []
+            rmfields = ['HGVSg','CAVA_HGVSg','HGVSp','CAVA_HGVSp','HGVSc','CAVA_HGVSc',
+                'TYPE', 'TRANSCRIPT', 'GENE', 'GENEID', 'TRINFO', 'LOC', 'CSN',
+                        'PROTPOS', 'PROTREF', 'PROTALT', 'CLASS', 'SO', 'ALTFLAG',
+                        'CAVA_TYPE', 'CAVA_TRANSCRIPT', 'CAVA_GENE', 'CAVA_GENEID', 'CAVA_TRINFO',
+                        'CAVA_LOC', 'CAVA_CSN',
+                        'CAVA_PROTPOS', 'CAVA_PROTREF', 'CAVA_PROTALT', 'CAVA_CLASS', 'CAVA_SO', 'CAVA_ALTFLAG']
+            for item in infos:
+                items = item.split("=")
+                if not ( items[0] in rmfields):
+                    newinfos.append(item)
+            self.info = ';'.join(newinfos)
+
 
             # Creating first part of the VCF record (up to FILTER field)
 
             chromstr = 'chr' + self.chrom if self.chrom_chr_prefix else self.chrom
             record = [chromstr, str(self.pos), self.id, self.ref, ",".join(outalts), self.qual, self.filter]
 
             # Preparing components of the String to be added to the INFO field
             flags = []
             flagvalues = []
             for variant in outvariants:
                 for i in range(len(variant.flags)):
                     key = variant.flags[i]
                     value = variant.flagvalues[i]
-                    if value == '': value = '.'
+                    if value == '':
+                        value = '.'
                     if key in flags:
                         flagvalues[flags.index(key)].append(value)
                     else:
                         flags.append(key)
                         flagvalues.append([value])
 
             # Creating String added to the INFO field, separating multiple alleles by ',' (within alt alleles, multiple
             # transcripts separated by ':')
             added = ''
             for i in range(len(flags)):
                 key = flags[i]
                 value = ','.join(flagvalues[i])
-                if len(added) > 0: added += ';'
-                if options.args['prefix']:
+                if len(added) > 0:
+                    added += ';'
+                if 'prefix' in options.args and options.args['prefix']:
                     added += 'CAVA_' + key + '=' + value
                 else:
                     added += key + '=' + value
 
             ########################################################################
             # Add HGVS
             # HS: 10/21/2020 Added HGVSP and multi-transcript support to HGVSc
             #                added prefix support
 
-            if options.args['prefix']:
+            if 'prefix' in options.args and options.args['prefix'] is True:
                 HGVSC_key = 'CAVA_HGVSc='
                 HGVSP_key = 'CAVA_HGVSp='
+ #               HGVSG_key = 'CAVA_HGVSg='
+
             else:
                 HGVSC_key = 'HGVSc='
                 HGVSP_key = 'HGVSp='
+ #               HGVSG_key = 'HGVSg='
 
             HGVSC = ''
             HGVSP = ''
+            # hgvsgs = flagvalues[flags.index('HGVSg')]
+            # HGVSG = ''
+            # if hgvsgs is not None:
+            #     HGVSG = hgvsgs[0]
+            contig = csn.get_contig_from_build(outvariants[0].chrom,build)
             if ('TRANSCRIPT' in flags) and ('GENE' in flags) and ('CSN' in flags):
-                # List of 1 entry per variant (alt-allele) .. and whithin each multiple transcripts are separated by ','
+                # List of 1 entry per variant (alt-allele) .. and within each multiple transcripts are separated by ','
                 transcripts_list = flagvalues[flags.index('TRANSCRIPT')]
                 gene_list = flagvalues[flags.index('GENE')]
                 csn_list = flagvalues[flags.index('CSN')]
+                #repeats_list = flagvalues[flags.index('REPEATS')]
                 csn_hgvs_list = csn_list
                 #csn_hgvs_list = flagvalues[flags.index('CSNHGVS')]
                 if not (len(transcripts_list) == 0 or len(gene_list) != len(transcripts_list) or len(gene_list) != len(
                         csn_list)):
                     for ihg in range(0, len(transcripts_list)):  # Loop over alt-alleles
-                        hgtranscripts = transcripts_list[ihg].split(":")
+                        hgtranscripts = transcripts_list[ihg].split(":")  # split over alt-alleles
                         hggenes = gene_list[ihg].split(":")
                         hgcsns = csn_list[ihg].split(":")
                         hgcsns_hgvs = csn_hgvs_list[ihg].split(":")
+                        #hgrepeats = repeats_list[ihg].split(":")
+
                         if not (len(hgtranscripts) == len(hggenes) and len(hgtranscripts) == len(hgcsns)):
                             print("ERROR transcripts GENE and CSN not same length\n")
                             print("--------------------------------------------------------------------\n")
                             if options.args['logfile']:
                                 logging.error("Bug: TRANSCRIPT GENE and CSN not same length\n")
                             sys.exit(1)
                         else:
                             trHGVSC = ''
                             trHGVSP = ''
                             for itr in range(0, len(hgtranscripts)):  # Loop over transcripts within each alt-alleles
                                 hgtranscript = hgtranscripts[itr]
                                 hggene = hggenes[itr]
                                 hgcsn_hgvs = hgcsns_hgvs[itr]
-                                tHGVSC = hgtranscript
-                                tHGVSC += '(' + hggene + '):'
+                                #hgrepeat = hgrepeats[itr]
+                                if len(hgtranscript)==0 or hgtranscript == '.':
+                                    tHGVSC = '.(.):'
+                                else:
+                                    tHGVSC = contig + '(' + hgtranscript + '):'
                                 try:
                                     cdna, prot = hgcsn_hgvs.split('_p.')
                                 except ValueError:  # Example c.802-51_802-14del38, splice
                                     cdna = hgcsn_hgvs
                                     prot = '.'
+                                # HGVS does not allow nucs after del c.21_22delAA
+                                del_nuc = re.match(r"^(.*del[ACGTacgtnN]+)$", cdna)
+                                if del_nuc:
+                                    cdna = del_nuc.group(1)
+                                #if len(hgrepeat)>1:
+                                #    tHGVSC += hgrepeat
+                                #else:
+                                #   tHGVSC += cdna
                                 tHGVSC += cdna
-                                if tHGVSC == '.(.):.':
+                                if cdna == '.' or  len(cdna)==0 or tHGVSC == '.(.):.' or tHGVSC == '.(.):':
                                     tHGVSC = '.'
                                 if prot == '.' or prot == '':
                                     tHGVSP = '.'
                                 else:
                                     # Get Protein matching Transcript from options
                                     if hgtranscript in options.transcript2protein:
                                         protid = options.transcript2protein[hgtranscript]
@@ -526,38 +810,41 @@
                     for j in range(len(variant.flags)):
                         # First, do not split annotation that is not transcript specific
                         if not variant.flags[j] in ['TRANSCRIPT', 'GENE', 'GENEID', 'TRINFO', 'LOC', 'CSN', 'CLASS',
                                                     'SO',
                                                     'IMPACT', 'ALTANN', 'ALTCLASS', 'ALTSO', 'ALTFLAG', 'PROTPOS',
                                                     'PROTREF', 'PROTALT']:
                             value = variant.flagvalues[j]
-                            if value == '': value = '.'
+                            if value == '':
+                                value = '.'
                             rest += '\t' + value
                             continue
 
                         values = variant.flagvalues[j].split(':')
                         value = values[i]
                         if value == '': value = '.'
                         rest += '\t' + value
                     if len(transcripts_list) == 0 or len(gene_list) != len(transcripts_list) or len(gene_list) != len(
                             csn_list) or len(transcripts_list) != N:
                         HGVSC = 'None'
                         HGVSP = 'None'
                     else:
                         hgtranscript = transcripts_list[i]
-                        HGVSC = hgtranscript
-                        HGVSC += '(' + gene_list[i] + '):'
+                        if len(hgtranscript) == 0 or hgtranscript == '.':
+                            HGVSC = '.(.):'
+                        else:
+                            HGVSC = contig + '(' + hgtranscript + '):'
                         try:
                             cdna, prot = csn_list[i].split('_p.')
                             prot = prot.replace('X', "Ter")
                         except ValueError:  # Example c.802-51_802-14del38, splice
                             cdna = csn_list[i]
                             prot = '.'
                         HGVSC += cdna
-                        if HGVSC == '.(.):.' or HGVSC == '():':
+                        if len(cdna)==0 or cdna == '.' or HGVSC == '.(.):.' or HGVSC == '():' or HGVSC == '.(.):':
                             HGVSC = '.'
                         if prot == '.' or prot == '':
                             HGVSP = '.'
                         else:
                             # Get Protein matching Transcript from options
                             if hgtranscript in options.transcript2protein:
                                 protid = options.transcript2protein[hgtranscript]
@@ -571,103 +858,218 @@
                                         "WARNING: transcript " + hgtranscript + " not in transcript2protein file, HGVSp will be invalid\n")
                                     print("--------------------------------------------------------------------\n")
                                     if options.args['logfile']:
                                         logging.info(
                                             "WARNING: transcript " + hgtranscript + " not in transcript2protein file\n")
                     # Writing record to the output file
                     if stdout:
-                        print(record + rest + "\t" + HGVSC + "\t" + HGVSP)
+                        print(record + rest + "\t" + HGVSC + "\t" + HGVSP )
                     else:
                         outfile.write(record + rest + "\t" + HGVSC + "\t" + HGVSP + '\n')
 
                 c += 1
 
 
 #######################################################################################################################
-
+class Tr_store:
+    lasttr = dict
+    
 # Class representing a single Ensembl transcript
 class Transcript(object):
     # Constructor
     def __init__(self, line):
         self.exons = []
         cols = line.split('\t')
         self.TRANSCRIPT = cols[0]
         self.geneSymbol = cols[1]
         self.geneID = cols[2]
         self.TRINFO = cols[3]
         self.chrom = cols[4]
         self.strand = int(cols[5])
-        self.transcriptStart = int(cols[6])
-        self.transcriptEnd = int(cols[7])
-        self.codingStart = int(cols[8])
-        self.codingStartGenomic = int(cols[9])
-        self.codingEndGenomic = int(cols[10])
+        self.transcriptStart = int(cols[6])  # 0-based, lowest coordinate
+        self.transcriptEnd = int(cols[7])   # 1-bases upper coordinate
+        self.codingStart = int(cols[8])  # in cDNA coordinated (1st base is 1)
+        self.codingStartGenomic = int(cols[9])# coding start genomic 1-based
+        self.codingEndGenomic = int(cols[10])# coding end genomic 1-based
         # Initializing and adding exons
         for i in range(1, len(cols) - 11, 2):
-            self.exons.append(Exon(int((i + 1) / 2), int(cols[10 + i]), int(cols[11 + i])))
+            self.exons.append(Exon(int((i + 1) / 2), int(cols[10 + i]), int(cols[11 + i])))   # Start is 0-based, ENd is 1-based -- like a bed file
+        self.three_prime_len = 0
+        self.exonseqs = None  # list of the exons for the reference sequence
+        self.cds_len = 0
+        foundStart = False
+        for ex in self.exons:
+            if self.strand == 1:
+                if self.codingStartGenomic > ex.start and self.codingStartGenomic<=ex.end: # CDS starts within exon
+                    if self.codingEndGenomic<=ex.end: # Both start and end within exon
+                        self.cds_len = self.codingEndGenomic+1-self.codingStartGenomic
+                        if self.codingEndGenomic<ex.end:  # is there anything left for 3' utr in this exon
+                            self.three_prime_len += ex.end-self.codingEndGenomic  #ex.end+1-(self.codingEndGenomic+1)
+                    else: # Start in this one, but ends in another exon
+                        self.cds_len = ex.end +1 - self.codingStartGenomic
+                elif self.codingStartGenomic <=ex.start: # Already Past start codon
+                    if self.codingEndGenomic<=ex.end and self.codingEndGenomic> ex.start: # cds ends inside this exon
+                        self.cds_len += (self.codingEndGenomic-ex.start)
+                        if self.codingEndGenomic<ex.end:  # is there anything left for 3' utr in this exon
+                            self.three_prime_len += ex.end-self.codingEndGenomic  #ex.end+1-(self.codingEndGenomic+1)
+                    elif ex.end <= self.codingEndGenomic: # End in downstream exon
+                        self.cds_len += ex.end-ex.start
+                    else: # Already past cds
+                        self.three_prime_len += ex.end-ex.start
+            else:  # Minus strand (exons are in transcription order)
+                if self.codingStartGenomic > ex.start and self.codingStartGenomic<=ex.end: # start within this exon
+                    if self.codingEndGenomic>ex.start: # Both start and end within exon
+                        self.cds_len = self.codingStartGenomic +1 - self.codingEndGenomic
+                        if ex.start+1<self.codingEndGenomic:  # is there anything left for 3' utr in this exon
+                            self.three_prime_len += (self.codingEndGenomic-1 - ex.start)
+                    else: # end in another exon
+                        self.cds_len = self.codingStartGenomic - ex.start
+                elif self.codingStartGenomic > ex.end: # Already passed start codon
+                    if self.codingEndGenomic < ex.start:  # End in downstream exon or includes whole exon
+                        self.cds_len += ex.end - ex.start
+                    elif self.codingEndGenomic<=ex.end and self.codingEndGenomic> ex.start: # end inside this exon
+                        self.cds_len += (ex.end +1 - self.codingEndGenomic ) # already  covered case where start and stop both in same exon.
+                        if ex.start + 1 < self.codingEndGenomic:  # is there anything left for 3' utr in this exon
+                            self.three_prime_len += (self.codingEndGenomic - 1 - ex.start)
+                    else: # Already past cds
+                        self.three_prime_len += ex.end-ex.start
 
-    # self.reference=reference.getReference(self.chrom,self.transcriptStart,self.transcriptEnd)
+                # else before start codon
 
+    # self.reference=reference.getReference(self.chrom,self.transcriptStart,self.transcriptEnd)
     # Getting the full coding sequence of the transcript
+    # Note that the coding sequence starts at ATG, but ends all the way to the end of the UTR (to allow frameshifting to include new stop)
+
+# Get coding sequence of the Alternate Transcript.
+
     def getCodingSequence(self, reference, variant, exonseqs):
-        ret = ''
+        ret = ''  # transcript sequence including alt-allele
+        ret_ref = ''  # transcript sequence with ref allele
         ret_exonseqs = []
+        coding_start_alt = self.codingStart
+        trans_pos = 0
+        if exonseqs is None and self.exonseqs is not None:
+            exonseqs = self.exonseqs
 
         for i in range(len(self.exons)):
+            # Exons are ordered 5' to 3; (different order for strand = 1 or -1)
             exon = self.exons[i]
+            if exonseqs is None:
+                # bef = reference.getReference(self.chrom, exon.start + 1, variant.pos - 1)  # 1-base positions
+                # aft = reference.getReference(self.chrom, variant.pos + len(variant.ref), exon.end)  # 1-base positions
+                exonseqF = reference.getReference(self.chrom, exon.start + 1, exon.end)
+                if self.strand == 1:
+                    exonseq = exonseqF
+                else:
+                    exonseq = exonseqF.reverseComplement()
+            else:
+                exonseq = exonseqs[i]
+
+            if variant is not None:
+                # Should not be calling this function for Variant that overlaps the splice site.
+                # .. e.g. will not work if variant.pos<exon.start+1 and variant.pos+len(variant.ref)>= exon.start+1 (left exon)
+                # .. or variant.pos<=exon.end and variant.pos+len(variant.ref)>exon.end (right end of exon)
 
-            if not variant is None:
-                if exon.start < variant.pos <= exon.end:
+                if exon.start < variant.pos <= exon.end:  #  same as exon.start+1 <= variant.pos <= exon.end
                     if self.strand == 1:
-                        ret += reference.getReference(self.chrom, exon.start + 1,
-                                                      variant.pos - 1) + variant.alt + reference.getReference(
-                            self.chrom, variant.pos + len(variant.ref), exon.end)
+                        trans_pos += (variant.pos - exon.start)
+                        bef_end_index = variant.pos - exon.start -1 # Points to variant pos .. this index will not be included in sequence
+                        upstream = exonseq[0:bef_end_index]  # note [0:0] == '', so if variant.pos is first base of exon, bef ==''
+                        aft_start_index = variant.pos+len(variant.ref)- (exon.start+1)  # index points after variant, or other side of insertion.
+                        downstream = exonseq[aft_start_index:]   # if variant.ref extend outside exon, will only grab sequence inside exon .. but realistically
+                                                            # the splicing won't occur.. this is caught earlier in CAVA by checking type of variant
+                                                            # and not protein annotating variants that span Extron-intron or Intron-Exon
+                        temp_alt = upstream + variant.alt + downstream
+                        if variant.pos+len(variant.ref)-1>exon.end: # This won't splice, so should not be calling this function
+                            if i != len(self.exons) -1: # if it's the last exon, it's OK.. won't affect protein ..
+                                sys.stderr.write("CAVA: ERROR: Bug, tried to get protein sequence for variant spanning splice site\n")
+                            temp_ref = upstream + variant.ref[0:exon.end + 1 - variant.pos]
+                        else:
+                            temp_ref = upstream + variant.ref+ downstream
                     else:
-                        temp = Sequence(reference.getReference(self.chrom, exon.start + 1,
-                                                               variant.pos - 1) + variant.alt + reference.getReference(
-                            self.chrom, variant.pos + len(variant.ref), exon.end))
-                        ret += temp.reverseComplement()
+                        trans_pos += (exon.end + 1 - variant.pos)
+                        bef_end_index = exon.length - (variant.pos - exon.start -1)
+                        downstream = exonseq[bef_end_index:]  ## if bef_end_index == exon.length ==> ==''
+                        aft_start_index = exon.end -variant.pos-len(variant.ref) +1
+                        if aft_start_index>0:
+                            upstream = exonseq[:aft_start_index]  # if SNP is at end of exon exonseq[:0] == '', correctly
+                        else:
+                            upstream = Sequence('')
+                        temp_alt = upstream + Sequence(variant.alt).reverseComplement() + downstream
+                        if variant.pos+len(variant.ref)-1>exon.end: # This won't splice, so should not be calling this function
+                            sys.stderr.write("CAVA: ERROR: Bug, tried to get protein sequence for variant spanning splice site\n")
+                            temp_ref = upstream + Sequence(variant.ref[0:exon.end + 1 - variant.pos]).reverseComplement
+                        temp_ref = upstream + Sequence(variant.ref).reverseComplement() + downstream
+
+                    ret_ref += temp_ref
+                    ret += temp_alt
+                    if exonseqs is None:
+                        ret_exonseqs.append(temp_ref)
+                    if trans_pos<coding_start_alt:
+                        coding_start_alt += (len(variant.alt) - len(variant.ref))
                     continue
+                else: # Variant not within exon
+                    pass  # No-op for readibility
 
-            if self.strand == 1:
-                if exonseqs is None:
-                    exonseq = reference.getReference(self.chrom, exon.start + 1, exon.end)
-                    ret += exonseq
-                    ret_exonseqs.append(exonseq)
-                else:
-                    ret += exonseqs[i]
-            else:
-                if exonseqs is None:
-                    exonseq = reference.getReference(self.chrom, exon.start + 1, exon.end).reverseComplement()
-                    ret += exonseq
-                    ret_exonseqs.append(exonseq)
-                else:
-                    ret += exonseqs[i]
+            trans_pos += abs(exon.end-exon.start)
 
-        ret = ret[self.codingStart - 1:]
+            if exonseqs is None:
+                ret_exonseqs.append(exonseq)
 
+            ret += exonseq
+            ret_ref += exonseq
+
+        ret_transcript_alt = ret + ""
+        # HS: fixed bug that if variant was before coding start, "ret" would not point to ATG
+        ret = ret[coding_start_alt  - 1:]
+        if variant is None: # Respect the transcript annotation of the position of the Stop Codon.
+            ret = ret[0:self.cds_len]
+
+        self.transcriptseq = ret_ref
+        if self.exonseqs is None:
+            self.exonseqs = ret_exonseqs
         if exonseqs is None:
-            return ret, ret_exonseqs
+            return ret, ret_exonseqs, ret_transcript_alt, ret_ref
         else:
-            return ret, exonseqs
+            return ret, exonseqs,     ret_transcript_alt, ret_ref
+
+    def getTranscriptSeq(self,reference):
+        if self.transcriptseq is None:
+            codingsequencealt, exonseqalt, transcript_alt_seq, transcript_seq = self.getCodingSequence(reference,None,None)
+            # self.transcriptseq = transcript_seq  .. this is done inside self.getCodingSequence
+        return self.transcriptseq
 
     # Getting the translated protein sequence of the transcript
     # with the variant included as well as a list of the (reference) exon sequence.
+    # The exonseqs should NOT include the alt allele
+    # Ideally, call this function first with variant = None to get exonseq .. to use in 2nd call of this function.
+
     def getProteinSequence(self, reference, variant, exonseqs, codon_usage):
         # Translating coding sequence
         codon_usage = codon_usage
-        codingsequence, exonseqa = self.getCodingSequence(reference, variant, exonseqs)
-        if (self.chrom == 'chrM' or
-                self.chrom == 'chrMT' or
-                self.chrom == 'M' or
-                self.chrom == 'MT'):
-            ret = Sequence(codingsequence).translate('4')
+        # returns exonsseq of the alternate allele unless variant is None
+        codingsequencealt, exonseqalt, transcript_alt_seq, transcript_seq = self.getCodingSequence(reference, variant, exonseqs)
+        if self.chrom in ['chrM','chrMT' , 'M','MT']: # No selenocysteine genes in mitochondrion genome
+            ret = Sequence(codingsequencealt).translate('4')
+        elif self.geneSymbol in ['DIO1','DIO2','DIO3','GPX1','GPX2','GPX3','GPX4','GPX6','SELENOF','SELENOH','SELENOI',
+                                 'SELENOK','SELENOM', 'SELENON','SELENOO','SELENOP','SELENOS','SELENOT','SELENOU',
+                                 'SELENOV','SELENOW','MSRB1', 'SEPHS2', 'TXNRD1', 'TXNRD2', 'TXNRD3']:
+            # the 'CDS' annotation of that transcript was trusted.. any TAG remaining will be recoded
+            # as Sec/U = Selenocysteine .. and not as 'X'
+            # Some 25+ human genes genes recode  the UGA stop codons as selenocysteines,
+            # most have name SELENO* so cannot remove the "X" .. must trust the annotation
+            #
+            # DIO1,DIO2,DIO3,GPX1,GPX2,GPX3,GPX4,GPX6,SELENO[F,H,I,K,M,N,O,P,S,T,U,V,W],MSRB1,SEPHS2,TXNRD1,TXNRD2,TXNRD3
+
+            ret = Sequence(codingsequencealt).translate('7')
         else:
-            ret = Sequence(codingsequence).translate(codon_usage)
-        return ret, exonseqa
+            ret = Sequence(codingsequencealt).translate(codon_usage)
+        ret = trim_prot_after_stop(ret)  # trim end, keeping from start to and including the first X (if any)
+
+        return ret, exonseqalt
 
     # Checking if a given position is outside the region between the start and stop codon
     def isPositionOutsideCDS(self, pos):
         if self.strand == 1:
             return (pos < self.codingStartGenomic) or (pos > self.codingEndGenomic)
         else:
             return (pos > self.codingStartGenomic) or (pos < self.codingEndGenomic)
@@ -680,45 +1082,45 @@
     # Checking if a given position is downstream the region between the start and stop codon
     def isPositionOutsideCDS_3prime(self, pos):
         return (self.strand == 1 and pos > self.codingEndGenomic) or (self.strand == -1 and pos < self.codingEndGenomic)
 
     # Checking if the given variant is outside of the translated region of the transcript
     def isOutsideTranslatedRegion(self, variant):
         if self.strand == 1:
-            if variant.isInsertion():
+            if variant.is_insertion:
                 if variant.pos <= self.codingStartGenomic: return True
                 if variant.pos - 1 >= self.codingEndGenomic: return True
                 return False
             else:
                 if variant.pos + len(variant.ref) - 1 < self.codingStartGenomic: return True
                 if variant.pos > self.codingEndGenomic: return True
                 return False
         else:
-            if variant.isInsertion():
+            if variant.is_insertion:
                 if variant.pos <= self.codingEndGenomic: return True
                 if variant.pos - 1 >= self.codingStartGenomic: return True
                 return False
             else:
                 if variant.pos + len(variant.ref) - 1 < self.codingEndGenomic: return True
                 if variant.pos > self.codingStartGenomic: return True
                 return False
 
     # Checking if the given variant is outside of the translated region of the transcript, +/- the first and last 3 bases of the coding sequence
     def isOutsideTranslatedRegionPlus3(self, variant):
         if self.strand == 1:
-            if variant.isInsertion():
+            if variant.is_insertion:
                 if variant.pos <= self.codingStartGenomic + 3: return True
                 if variant.pos - 1 >= self.codingEndGenomic - 3: return True
                 return False
             else:
                 if variant.pos + len(variant.ref) - 1 < self.codingStartGenomic + 3: return True
                 if variant.pos > self.codingEndGenomic - 3: return True
                 return False
         else:
-            if variant.isInsertion():
+            if variant.is_insertion:
                 if variant.pos <= self.codingEndGenomic + 3: return True
                 if variant.pos - 1 >= self.codingStartGenomic - 3: return True
                 return False
             else:
                 if variant.pos + len(variant.ref) - 1 < self.codingEndGenomic + 3: return True
                 if variant.pos > self.codingStartGenomic - 3: return True
                 return False
@@ -745,24 +1147,24 @@
 
     # Checking if the given variant affects a +5 essential splice site
     def isIn_SS5_Site(self, variant):
         if not self.isOutsideTranslatedRegion(variant):
             if self.strand == 1:
                 for exon in self.exons:
                     if variant.overlap(exon.end + 1, exon.end + 5):
-                        if not variant.isSubstitution():
+                        if not variant.is_substitution:
                             if not (variant.pos == exon.end + 3 and len(variant.ref) == 2 and len(
                                     variant.alt) == 2): return True
                         else:
                             if variant.pos == exon.end + 5: return True
                 return False
             else:
                 for exon in self.exons:
                     if variant.overlap(exon.start - 4, exon.start):
-                        if not variant.isSubstitution():
+                        if not variant.is_substitution:
                             if not (variant.pos == exon.start - 3 and len(variant.ref) == 2 and len(
                                     variant.alt) == 2): return True
                         else:
                             if variant.pos == exon.start - 4: return True
                 return False
         else:
             return False
@@ -786,50 +1188,69 @@
                     self.strand == -1 and exon.end < pos <= prevexonend)):
                 if self.intronLength(exon.index) > 5 or self.intronLength(exon.index) == 3:
                     return 'In' + str(exon.index - 1) + '/' + str(exon.index)
                 else:
                     return 'fsIn' + str(exon.index - 1) + '/' + str(exon.index)
             if exon.start < pos <= exon.end:
                 if (self.strand == 1 and pos < self.codingStartGenomic) or (
-                        self.strand == -1 and pos > self.codingStartGenomic): return '5UTR'
+                        self.strand == -1 and pos > self.codingStartGenomic):
+                    return '5UTR'
                 if (self.strand == 1 and pos > self.codingEndGenomic) or (
-                        self.strand == -1 and pos < self.codingEndGenomic): return '3UTR'
+                        self.strand == -1 and pos < self.codingEndGenomic):
+                    return '3UTR'
                 return 'Ex' + str(exon.index)
             prevexonend = exon.end if self.strand == 1 else exon.start
 
         return '.'
 
     # Checking where a given variant is located in the transcript
     def whereIsThisVariant(self, variant):
         # Getting the locations of both end points of the variant
-        if variant.isInsertion():
+        if variant.is_insertion:
             first = self.whereIsThisPosition(variant.pos - 1)
             second = self.whereIsThisPosition(variant.pos)
         else:
             first = self.whereIsThisPosition(variant.pos)
             second = self.whereIsThisPosition(variant.pos + len(variant.ref) - 1)
         if first == second:
             return first
         if self.strand == 1:
-            return first + '-' + second
+            if (len(first) == 0 or first == '.') and (len(second) == 0 or second == '.'):
+                return '.'
+            elif first == '.' or len(first) == 0:
+                return second
+            elif second == '.' or len(second) == 0:
+                return first
+            else:
+                return first + '-' + second
         else:
-            return second + '-' + first
+            if (len(first) == 0 or first == '.') and (len(second) == 0 or second == '.'):
+                return '.'
+            elif first == '.' or len(first) ==0:
+                return second
+            elif second == '.' or len(second)==0:
+                return first
+            else:
+                return second + '-' + first
 
     # Getting the length of an intron, where idx is the index of the succeeding exon
     def intronLength(self, idx):
+        if idx <= 0:
+            return 0
         for exon in self.exons:
             if exon.index == idx:
                 if self.strand == 1:
                     return exon.start - prev
                 else:
                     return prev - exon.end
             if self.strand == 1:
                 prev = exon.end
             else:
                 prev = exon.start
+        return 0
 
 
 #######################################################################################################################
 
 # Class representing a single exon
 class Exon(object):
     # Constructor
@@ -841,15 +1262,15 @@
 
     def contains(self, pos):
         return self.start + 1 <= pos <= self.end
 
 
 #######################################################################################################################
 
-# Class representing a DNA sequence
+# Class representing a DNA sequence, inherits from str class
 class Sequence(str):
     # Translating to amino acid sequence
     def translate(self, letter):
         gencode = {}
         if letter == '1':
             gencode = {
                 'ATA': 'I', 'ATC': 'I', 'ATT': 'I', 'ATG': 'M',
@@ -864,15 +1285,15 @@
                 'GCA': 'A', 'GCC': 'A', 'GCG': 'A', 'GCT': 'A',
                 'GAC': 'D', 'GAT': 'D', 'GAA': 'E', 'GAG': 'E',
                 'GGA': 'G', 'GGC': 'G', 'GGG': 'G', 'GGT': 'G',
                 'TCA': 'S', 'TCC': 'S', 'TCG': 'S', 'TCT': 'S',
                 'TTC': 'F', 'TTT': 'F', 'TTA': 'L', 'TTG': 'L',
                 'TAC': 'Y', 'TAT': 'Y', 'TAA': 'X', 'TAG': 'X',
                 'TGC': 'C', 'TGT': 'C', 'TGA': 'X', 'TGG': 'W'}
-        if letter == '3':
+        elif letter == '3': # 3-letter code version of 1 (Human)
             gencode = {
                 'ATA': 'Ile', 'ATC': 'Ile', 'ATT': 'Ile', 'ATG': 'Met',
                 'ACA': 'Thr', 'ACC': 'Thr', 'ACG': 'Thr', 'ACT': 'Thr',
                 'AAC': 'Asn', 'AAT': 'Asn', 'AAA': 'Lys', 'AAG': 'Lys',
                 'AGC': 'Ser', 'AGT': 'Ser', 'AGA': 'Arg', 'AGG': 'Arg',
                 'CTA': 'Leu', 'CTC': 'Leu', 'CTG': 'Leu', 'CTT': 'Leu',
                 'CCA': 'Pro', 'CCC': 'Pro', 'CCG': 'Pro', 'CCT': 'Pro',
@@ -882,15 +1303,15 @@
                 'GCA': 'Ala', 'GCC': 'Ala', 'GCG': 'Ala', 'GCT': 'Ala',
                 'GAC': 'Asp', 'GAT': 'Asp', 'GAA': 'Glu', 'GAG': 'Glu',
                 'GGA': 'Gly', 'GGC': 'Gly', 'GGG': 'Gly', 'GGT': 'Gly',
                 'TCA': 'Ser', 'TCC': 'Ser', 'TCG': 'Ser', 'TCT': 'Ser',
                 'TTC': 'Phe', 'TTT': 'Phe', 'TTA': 'Leu', 'TTG': 'Leu',
                 'TAC': 'Tyr', 'TAT': 'Tyr', 'TAA': 'X', 'TAG': 'X',
                 'TGC': 'Cys', 'TGT': 'Cys', 'TGA': 'X', 'TGG': 'Trp'}
-        if letter == '4':
+        elif letter == '4': # Mitochondrgenetic code for vertebrates
             gencode = {
                 'ATA': 'M', 'ATC': 'I', 'ATT': 'I', 'ATG': 'M',
                 'ACA': 'T', 'ACC': 'T', 'ACG': 'T', 'ACT': 'T',
                 'AAC': 'N', 'AAT': 'N', 'AAA': 'K', 'AAG': 'K',
                 'AGC': 'S', 'AGT': 'S', 'AGA': 'X', 'AGG': 'X',
                 'CTA': 'L', 'CTC': 'L', 'CTG': 'L', 'CTT': 'L',
                 'CCA': 'P', 'CCC': 'P', 'CCG': 'P', 'CCT': 'P',
@@ -900,15 +1321,15 @@
                 'GCA': 'A', 'GCC': 'A', 'GCG': 'A', 'GCT': 'A',
                 'GAC': 'D', 'GAT': 'D', 'GAA': 'E', 'GAG': 'E',
                 'GGA': 'G', 'GGC': 'G', 'GGG': 'G', 'GGT': 'G',
                 'TCA': 'S', 'TCC': 'S', 'TCG': 'S', 'TCT': 'S',
                 'TTC': 'F', 'TTT': 'F', 'TTA': 'L', 'TTG': 'L',
                 'TAC': 'Y', 'TAT': 'Y', 'TAA': 'X', 'TAG': 'X',
                 'TGC': 'C', 'TGT': 'C', 'TGA': 'W', 'TGG': 'W'}
-        if letter == '5':
+        elif letter == '5': # 3-letter version of Mitochondria
             gencode = {
                 'AAA': 'K', 'AAC': 'N', 'AAG': 'K', 'AAT': 'N',
                 'ACA': 'T', 'ACC': 'T', 'ACG': 'T', 'ACT': 'T',
                 'AGA': 'R', 'AGC': 'S', 'AGG': 'R', 'AGT': 'S',
                 'ATA': 'I', 'ATC': 'I', 'ATG': 'M', 'ATT': 'I',
                 'CAA': 'Q', 'CAC': 'H', 'CAG': 'Q', 'CAT': 'H',
                 'CCA': 'P', 'CCC': 'P', 'CCG': 'P', 'CCT': 'P',
@@ -918,34 +1339,73 @@
                 'GCA': 'A', 'GCC': 'A', 'GCG': 'A', 'GCT': 'A',
                 'GGA': 'G', 'GGC': 'G', 'GGG': 'G', 'GGT': 'G',
                 'GTA': 'V', 'GTC': 'V', 'GTG': 'V', 'GTT': 'V',
                 'TAA': 'X', 'TAC': 'Y', 'TAG': 'X', 'TAT': 'Y',
                 'TCA': 'S', 'TCC': 'S', 'TCG': 'S', 'TCT': 'S',
                 'TGA': 'X', 'TGC': 'C', 'TGG': 'W', 'TGT': 'C',
                 'TTA': 'L', 'TTC': 'F', 'TTG': 'L', 'TTT': 'F'}
-        ret = ''
+        elif letter == '7': # Human genome for one of the 25 selenoproteins (TAG is Se-Cys (U/Sec)
+            gencode = {
+                'ATA': 'I', 'ATC': 'I', 'ATT': 'I', 'ATG': 'M',
+                'ACA': 'T', 'ACC': 'T', 'ACG': 'T', 'ACT': 'T',
+                'AAC': 'N', 'AAT': 'N', 'AAA': 'K', 'AAG': 'K',
+                'AGC': 'S', 'AGT': 'S', 'AGA': 'R', 'AGG': 'R',
+                'CTA': 'L', 'CTC': 'L', 'CTG': 'L', 'CTT': 'L',
+                'CCA': 'P', 'CCC': 'P', 'CCG': 'P', 'CCT': 'P',
+                'CAC': 'H', 'CAT': 'H', 'CAA': 'Q', 'CAG': 'Q',
+                'CGA': 'R', 'CGC': 'R', 'CGG': 'R', 'CGT': 'R',
+                'GTA': 'V', 'GTC': 'V', 'GTG': 'V', 'GTT': 'V',
+                'GCA': 'A', 'GCC': 'A', 'GCG': 'A', 'GCT': 'A',
+                'GAC': 'D', 'GAT': 'D', 'GAA': 'E', 'GAG': 'E',
+                'GGA': 'G', 'GGC': 'G', 'GGG': 'G', 'GGT': 'G',
+                'TCA': 'S', 'TCC': 'S', 'TCG': 'S', 'TCT': 'S',
+                'TTC': 'F', 'TTT': 'F', 'TTA': 'L', 'TTG': 'L',
+                'TAC': 'Y', 'TAT': 'Y', 'TAA': 'X', 'TAG': 'X',
+                'TGC': 'C', 'TGT': 'C', 'TGA': 'U', 'TGG': 'W'}
+        elif letter == '8': # 3-letter code version of 1 (Human) with SelenoCysteinr for ATG
+            gencode = {
+                'ATA': 'Ile', 'ATC': 'Ile', 'ATT': 'Ile', 'ATG': 'Met',
+                'ACA': 'Thr', 'ACC': 'Thr', 'ACG': 'Thr', 'ACT': 'Thr',
+                'AAC': 'Asn', 'AAT': 'Asn', 'AAA': 'Lys', 'AAG': 'Lys',
+                'AGC': 'Ser', 'AGT': 'Ser', 'AGA': 'Arg', 'AGG': 'Arg',
+                'CTA': 'Leu', 'CTC': 'Leu', 'CTG': 'Leu', 'CTT': 'Leu',
+                'CCA': 'Pro', 'CCC': 'Pro', 'CCG': 'Pro', 'CCT': 'Pro',
+                'CAC': 'His', 'CAT': 'His', 'CAA': 'Gln', 'CAG': 'Gln',
+                'CGA': 'Arg', 'CGC': 'Arg', 'CGG': 'Arg', 'CGT': 'Arg',
+                'GTA': 'Val', 'GTC': 'Val', 'GTG': 'Val', 'GTT': 'Val',
+                'GCA': 'Ala', 'GCC': 'Ala', 'GCG': 'Ala', 'GCT': 'Ala',
+                'GAC': 'Asp', 'GAT': 'Asp', 'GAA': 'Glu', 'GAG': 'Glu',
+                'GGA': 'Gly', 'GGC': 'Gly', 'GGG': 'Gly', 'GGT': 'Gly',
+                'TCA': 'Ser', 'TCC': 'Ser', 'TCG': 'Ser', 'TCT': 'Ser',
+                'TTC': 'Phe', 'TTT': 'Phe', 'TTA': 'Leu', 'TTG': 'Leu',
+                'TAC': 'Tyr', 'TAT': 'Tyr', 'TAA': 'X', 'TAG': 'X',
+                'TGC': 'Cys', 'TGT': 'Cys', 'TGA': 'Sec', 'TGG': 'Trp'}
+        ret_list = []
         index = 0
         while index + 3 <= len(self):
-            codon = self[index:index + 3].upper()
-            if codon.replace('A', '').replace('C', '').replace('G', '').replace('T', ''):
+            #codon = self[index:index + 3].upper()   # Upper is not necessary .. it is done in Referenge.getReference
+            codon = self[index:index + 3]
+# SLOWEST line of code.           if codon.replace('A', '').replace('C', '').replace('G', '').replace('T', ''):
+            if codon not in gencode:
                 # if 'N' in codon:
-                ret += '?'
+                ret_list.append('?')
                 index += 3
                 continue
-            ret += gencode[codon]
+            ret_list.append(gencode[codon])
             index += 3
-        return ret
+        return ''.join(ret_list)
 
     # Getting reverse complement sequence
     def reverseComplement(self):
         # 5/13/21 Added support for reverse complement of "."
         complement = {"A": "T", "T": "A", "C": "G", "G": "C", "N": "N", "a": "t", "t": "a", "c": "g", "g": "c",
                       "n": "n", "*": "*", ".": "."}
         ret = ''
-        for base in self[::-1]: ret += complement[base]
+        for base in self[::-1]:
+            ret += complement[base]
         return ret
 
 
 #######################################################################################################################
 
 # Class representing the collection of options specified in the configuration file
 class Options(object):
@@ -968,31 +1428,32 @@
         self.defs['logfile'] = ('boolean', False)
         self.defs['target'] = ('string', '.')
         self.defs['genelist'] = ('string', '.')
         self.defs['transcriptlist'] = ('string', '.')
         self.defs['snplist'] = ('string', '.')
         self.defs['nonannot'] = ('boolean', True)
         self.defs['givealt'] = ('boolean', True)
-        self.defs['givealtflag'] = ('boolean', False)
+        self.defs['givealtflag'] = ('boolean', True)
         self.defs['ssrange'] = ('string', '8')
         self.defs['ontology'] = ('string', 'both')
         self.defs['impactdef'] = ('string', 'SG,ESS,FS|SS5,IM,SL,EE,IF,NSY|SY,SS,INT,5PU,3PU')
         self.defs['prefix'] = ('boolean', False)
         self.defs['codon_usage'] = ('string', '1')
         self.defs['normalized_mitochondrial_chrom'] = ('string', 'not_normalized')
 
         self.defs['transcript2protein'] = ('string', '.')
+        self.defs['loadalltranscripts'] = ('boolean', True)
 
         # Reading options from file
         self.read()
 
         if self.args['ensembl'] == '.' or self.args['ensembl'] == '':
             d = os.path.dirname(os.path.realpath(__file__))
-            dir = d[:d.rfind('env/lib')]
-            self.args['ensembl'] = dir + '/defaultdb/ensembl75s.gz'
+            dirn = d[:d.rfind('env/lib')]
+            self.args['ensembl'] = dirn + '/defaultdb/ensembl75s.gz'
 
     # Reading options from configuration file
     def read(self):
         for line in open(self.configfn):
             line = line.strip()
             if line.startswith('@'):
                 key = line[1:line.index('=')].strip()
@@ -1005,27 +1466,79 @@
             if not key in list(self.args.keys()): self.args[key] = default
 
 
 #######################################################################################################################            
 
 # Other basic utility functions 
 
+#
+# Convert various chromosome nomenclatures to that found in file.
+#
+def convert_chrom(chrom, contigs):
+        # Checking if chromosome name exists
+        if chrom in contigs:
+            return chrom
+        if len(chrom)>3 and chrom.startswith("chr"):
+            goodchrom = chrom[3:]
+            if goodchrom in contigs:
+                return goodchrom
+
+            if goodchrom == "MT":
+                goodchrom = 'chrM'
+                if goodchrom in contigs:
+                    return goodchrom
+                goodchrom = "M"
+                if goodchrom in contigs:
+                    return goodchrom
+                else:
+                    return None
+        elif chrom == "MT": # Cannot be chrMT .. because those starting with chr dealth above
+            goodchrom = 'chrMT'
+            if goodchrom in contigs:
+                return goodchrom
+            goodchrom = 'chrM'
+            if goodchrom in contigs:
+                return goodchrom
+            goodchrom = "M"
+            if goodchrom in contigs:
+                return goodchrom
+        elif chrom == "M":  # Cannot be chrM .. because those starting with chr dealth above
+                goodchrom = "MT"
+                if goodchrom in contigs:
+                    return goodchrom
+                goodchrom = "chrMT"
+                if goodchrom in contigs:
+                    return goodchrom
+                goodchrom = "chrM"
+                if goodchrom in contigs:
+                    return goodchrom
+        else:
+            goodchrom = "chr"+chrom
+            if goodchrom in contigs:
+                return goodchrom
+        return None
+
+
 # Reading gene, transcript or snp list from file
 def readSet(options, tag):
     ret = set()
     if tag in list(options.args.keys()) and not (options.args[tag] == '' or options.args[tag] == '.'):
         for line in open(options.args[tag]):
             line = line.strip()
-            if line == '' or line == '.': continue
+            if line == '' or line == '.':
+                continue
             ret.add(line)
         if options.args['logfile']:
             txt = ''
-            if tag == 'genelist': txt = 'Gene list'
-            if tag == 'transcriptlist': txt = 'Transcript list'
-            if tag == 'snplist': txt = 'SNP list'
+            if tag == 'genelist':
+                txt = 'Gene list'
+            if tag == 'transcriptlist':
+                txt = 'Transcript list'
+            if tag == 'snplist':
+                txt = 'SNP list'
             logging.info(txt + ' loaded.')
     return ret
 
 
 # Reading dictionary (from transcript -> Protein)
 def read_dict(options, tag):
     ret = dict()
@@ -1068,14 +1581,15 @@
     headerinfo += '##INFO=<ID=' + prefix + 'ALTANN,Number=.,Type=String,Description=\"Alternate CSN annotation\",Source=\"CAVA\",Version=\"' + version + '\">\n'
     headerinfo += '##INFO=<ID=' + prefix + 'ALTCLASS,Number=.,Type=String,Description=\"Alternate CLASS annotation\",Source=\"CAVA\",Version=\"' + version + '\">\n'
     headerinfo += '##INFO=<ID=' + prefix + 'ALTSO,Number=.,Type=String,Description=\"Alternate SO annotation\",Source=\"CAVA\",Version=\"' + version + '\">\n'
     headerinfo += '##INFO=<ID=' + prefix + 'IMPACT,Number=.,Type=String,Description=\"Impact group the variant is stratified into\",Source=\"CAVA\",Version=\"' + version + '\">\n'
     headerinfo += '##INFO=<ID=' + prefix + 'DBSNP,Number=.,Type=String,Description=\"rsID from dbSNP\",Source=\"CAVA\",Version=\"' + version + '\">\n'
     headerinfo += '##INFO=<ID=' + prefix + 'HGVSc,Number=.,Type=String,Description=\"HGVS Nomenclature for cDNA changes\",Source=\"CAVA\",Version=\"' + version + '\">\n'
     headerinfo += '##INFO=<ID=' + prefix + 'HGVSp,Number=.,Type=String,Description=\"HGVS Nomenclature for protein changes\",Source=\"CAVA\",Version=\"' + version + '\">\n'
+    headerinfo += '##INFO=<ID=' + prefix + 'HGVSg,Number=.,Type=String,Description=\"HGVS Nomenclature for genomic changes, right-shifted\",Source=\"CAVA\",Version=\"' + version + '\">\n'
 
     dateline = '##fileDate=' + time.strftime("%Y-%m-%d")
 
     if options.args['outputformat'] == 'VCF':
         if header == '':
             if stdout:
                 print(
@@ -1084,53 +1598,55 @@
                 outfile.write(
                     '##fileformat=VCFv4.1\n' + dateline + '\n' + headerinfo + '#CHROM\tPOS\tID\tREF\tALT\tQUAL\tFILTER\tINFO\n')
         else:
             headerv = header.split('\n')
             headerm = []
             startline = '##fileformat=VCFv4.1'
             for x in headerv:
-                if x.startswith('##fileDate') or x.startswith('##filedate'): continue
+                if x.startswith('##fileDate') or x.startswith('##filedate'):
+                    continue
                 if x.startswith('##fileformat'):
                     startline = x
                     continue
                 headerm.append(x)
             if stdout:
                 print(startline + '\n' + dateline + '\n' + headerinfo + '\n'.join(headerm) + '\n')
             else:
                 outfile.write(startline + '\n' + dateline + '\n' + headerinfo + '\n'.join(headerm) + '\n')
 
     if options.args['outputformat'] == 'TSV':
-        str = 'ID\tCHROM\tPOS\tREF\tALT\tQUAL\tFILTER\tTYPE'
+        hstr = 'ID\tCHROM\tPOS\tREF\tALT\tQUAL\tFILTER\tTYPE'
         if (not options.args['ensembl'] == '.') and (not options.args['ensembl'] == ''):
-            if options.args[
-                'ontology'].upper() == 'CLASS': str += '\tTRANSCRIPT\tGENE\tGENEID\tTRINFO\tLOC\tCSN\tPROTPOS\tPROTREF\tPROTALT\tCLASS'
-            if options.args[
-                'ontology'].upper() == 'SO': str += '\tTRANSCRIPT\tGENE\tGENEID\tTRINFO\tLOC\tCSN\tPROTPOS\tPROTREF\tPROTALT\tSO'
-            if options.args[
-                'ontology'].upper() == 'BOTH': str += '\tTRANSCRIPT\tGENE\tGENEID\tTRINFO\tLOC\tCSN\tPROTPOS\tPROTREF\tPROTALT\tCLASS\tSO'
+            if options.args['ontology'].upper() == 'CLASS':
+                hstr += '\tTRANSCRIPT\tGENE\tGENEID\tTRINFO\tLOC\tCSN\tPROTPOS\tPROTREF\tPROTALT\tCLASS'
+            if options.args['ontology'].upper() == 'SO':
+                hstr += '\tTRANSCRIPT\tGENE\tGENEID\tTRINFO\tLOC\tCSN\tPROTPOS\tPROTREF\tPROTALT\tSO'
+            if options.args['ontology'].upper() == 'BOTH':
+                hstr += '\tTRANSCRIPT\tGENE\tGENEID\tTRINFO\tLOC\tCSN\tPROTPOS\tPROTREF\tPROTALT\tCLASS\tSO'
 
-            if not (options.args['impactdef'] == '.' or options.args['impactdef'] == ''): str += '\tIMPACT'
+            if not (options.args['impactdef'] == '.' or options.args['impactdef'] == ''):
+                hstr += '\tIMPACT'
 
             if options.args['givealt']:
-                if options.args['ontology'].upper() == 'CLASS': str += '\tALTANN\tALTCLASS'
-                if options.args['ontology'].upper() == 'SO': str += '\tALTANN\tALTSO'
-                if options.args['ontology'].upper() == 'BOTH': str += '\tALTANN\tALTCLASS\tALTSO'
+                if options.args['ontology'].upper() == 'CLASS': hstr += '\tALTANN\tALTCLASS'
+                if options.args['ontology'].upper() == 'SO': hstr += '\tALTANN\tALTSO'
+                if options.args['ontology'].upper() == 'BOTH': hstr += '\tALTANN\tALTCLASS\tALTSO'
 
             if (not options.args['givealt']) or options.args['givealtflag']:
-                str += '\tALTFLAG'
+                hstr += '\tALTFLAG'
 
         if (not options.args['dbsnp'] == '.') and (not options.args['dbsnp'] == ''):
-            str += '\tDBSNP'
+            hstr += '\tDBSNP'
 
-        str += '\tHGVSC\tHGVSP'
+        hstr += '\tHGVSG\tHGVSC\tHGVSP'
 
         if stdout:
-            print(str)
+            print(hstr)
         else:
-            outfile.write(str + '\n')
+            outfile.write(hstr + '\n')
 
 
 # Counting number of records in a file
 def countRecords(filename):
     ret = 0
     if filename.endswith('.gz'):
         inputf = gzip.open(filename, 'rt')
@@ -1141,41 +1657,41 @@
         if not (line.startswith("#") or line == ''): ret += 1
     return ret
 
 
 # Checking if options are correct
 def checkOptions(options):
     # Checking if @inputformat was given correct value
-    str = options.args['inputformat'].upper()
-    if not (str == 'VCF' or str == 'TXT'):
+    optstr = options.args['inputformat'].upper()
+    if not (optstr == 'VCF' or optstr == 'TXT'):
         print('ERROR: incorrect value of the tag @inputformat.')
         print('(Allowed values: \'VCF\' or \'TXT\')')
         print('\nNo output file written. CAVA quit.')
         print("--------------------------------------------------------------------\n")
         if options.args['logfile']:
             logging.error('Incorrect value of the tag @inputformat.')
             logging.info('No output file written. CAVA quit.')
         quit()
 
     # Checking if @outputformat was given correct value
-    str = options.args['outputformat'].upper()
-    if not (str == 'VCF' or str == 'TSV'):
+    optstr = options.args['outputformat'].upper()
+    if not (optstr == 'VCF' or optstr == 'TSV'):
         print('ERROR: incorrect value of the tag @outputformat.')
         print('(Allowed values: \'VCF\' or \'TSV\')')
         print('\nNo output file written. CAVA quit.')
         print("--------------------------------------------------------------------\n")
         if options.args['logfile']:
             logging.error('Incorrect value of the tag @outputformat.')
             logging.info('No output file written. CAVA quit.')
         quit()
 
     # Checking if @type was given correct value
-    str = options.args['type'].upper()
+    optstr = options.args['type'].upper()
     if not (
-            str == 'ALL' or str == 'SUBSTITUTION' or str == 'INDEL' or str == 'INSERTION' or str == 'DELETION' or str == 'COMPLEX'):
+            optstr == 'ALL' or optstr == 'SUBSTITUTION' or optstr == 'INDEL' or optstr == 'INSERTION' or optstr == 'DELETION' or optstr == 'COMPLEX'):
         print('ERROR: incorrect value of the tag @type.')
         print('(Allowed values: \'all\', \'substitution\', \'indel\', \'insertion\', \'deletion\' or \'complex\')')
         print('\nNo output file written. CAVA quit.')
         print("--------------------------------------------------------------------\n")
         if options.args['logfile']:
             logging.error('Incorrect value of the tag @type.')
             logging.info('No output file written. CAVA quit.')
@@ -1190,16 +1706,16 @@
         print("--------------------------------------------------------------------\n")
         if options.args['logfile']:
             logging.error('Incorrect value of the tag @ssrange.')
             logging.info('No output file written. CAVA quit.')
         quit()
 
     # Checking if @ontology was given correct value
-    str = options.args['ontology'].upper()
-    if not (str == 'CLASS' or str == 'SO' or str == 'BOTH'):
+    optstr = options.args['ontology'].upper()
+    if not (optstr == 'CLASS' or optstr == 'SO' or optstr == 'BOTH'):
         print('ERROR: incorrect value of the tag @ontology.')
         print('(Allowed values: \'CLASS\' or \'SO\' or \'both\')')
         print('\nNo output file written. CAVA quit.')
         print("--------------------------------------------------------------------\n")
         if options.args['logfile']:
             logging.error('Incorrect value of the tag @ontology.')
             logging.info('No output file written. CAVA quit.')
@@ -1321,27 +1837,36 @@
         if options.args['logfile']:
             logging.error('The file given as @snplist does not exist.')
             logging.info('No output file written. CAVA quit.')
         quit()
 
     # Checking if @transcript2protein file exists
     #  
-    if not (('transcripts2protein' not in options.args) or options.args['transcript2protein'] == '.' or options.args[
-        'transcript2protein'] == '') and not os.path.isfile(options.args['transcript2protein']):
+    if not (('transcripts2protein' not in options.args) or options.args['transcript2protein'] == '.'
+            or options.args['transcript2protein'] == '') and not os.path.isfile(options.args['transcript2protein']):
         print('ERROR: the file given as @transcript2protein does not exist.')
         print('\nNo output file written. CAVA quit.')
         print("--------------------------------------------------------------------\n")
         quit()
 
     # Checking if @normalized_mitochondrial_chrom was given correct value
-    str = options.args['normalized_mitochondrial_chrom']
-    if str != 'not_normalized' and not (str == 'M' or str == 'MT'):
+    optstr = options.args['normalized_mitochondrial_chrom']
+    if optstr != 'not_normalized' and not (optstr == 'M' or optstr == 'MT'):
         print('ERROR: incorrect value of the tag @normalized_mitochondrial_chrom.')
         print('(Allowed values: \'M\' or \'MT\')')
         print('\nNo output file written. CAVA quit.')
         print("--------------------------------------------------------------------\n")
         if options.args['logfile']:
             logging.error('Incorrect value of the tag @normalized_mitochondrial_chrom.')
             logging.info('No output file written. CAVA quit.')
         quit()
 
-#######################################################################################################################
+# trim protein, up to including the stop codon
+
+def trim_prot_after_stop(seq):
+    if 'X' in seq:
+        seq = seq[0:(seq.index('X') + 1)]
+    elif 'x' in seq:
+        seq = seq[0:(seq.index('x') + 1)]
+    return seq
+
+######################################################################################################################
```

### Comparing `CAVA-2.0.5/cava/utils/main.py` & `CAVA-2.0.7/cava/utils/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import datetime
 import gzip
 import logging
 import multiprocessing
 import os
 import sys
-
 import pysam
 
 from cava.utils.data import Ensembl
 from cava.utils.data import Reference
 from cava.utils.data import dbSNP
 from . import core
 from .core import Options
@@ -96,27 +95,29 @@
 
 
 # Finding break points in the input file
 def findFileBreaks(inputf, threads):
     ret = []
     started = False
     counter = 0
+    first =1
 
     if inputf.endswith('.gz'):
         infile = gzip.open(inputf, 'rt')
     else:
         infile = open(inputf)
 
     for line in infile:
         counter += 1
         line = line.strip()
         if line == '' or line.startswith('#'): continue
         if not started:
             started = True
             first = counter
+
     delta = int((counter - first + 1) / threads)
     for i in range(threads):
         if i < threads - 1:
             ret.append((first + i * delta, first + (i + 1) * delta - 1))
         else:
             ret.append((first + i * delta, ''))
     return ret
@@ -139,23 +140,23 @@
         else:
             break
 
     return ret
 
 
 # Merging tmp files to final output file
-def mergeTmpFiles(output, format, threads):
+def mergeTmpFiles(output, fileformat, threads):
     filenames = []
     for i in range(1, threads + 1):
-        if format == 'VCF':
+        if fileformat == 'VCF':
             filenames.append(output + '_tmp_' + str(i) + '.vcf')
         else:
             filenames.append(output + '_tmp_' + str(i) + '.txt')
 
-    if format == 'VCF':
+    if fileformat == 'VCF':
         outfn = output + '.vcf'
     else:
         outfn = output + '.txt'
 
     with open(outfn, 'a') as outfile:
         for fname in filenames:
             with open(fname) as infile:
@@ -231,36 +232,47 @@
         codon_usage = ['1']
         with open(copts.conf) as c:
             for line in c:
                 if line.startswith('@codon_usage'):
                     codon_usage = line[line.find('=') + 1:].strip().split(',')
                     self.codon_usage = codon_usage
 
+        # Reference genome
+        self.reference = Reference(options)
+        if options.args['logfile'] and threadidx == 1: logging.info('Connected to reference genome.')
+
         if (not options.args['ensembl'] == '.') and (not options.args['ensembl'] == ''):
-            self.ensembl = Ensembl(options, genelist, transcriptlist, codon_usage[0])
-            if options.args['logfile'] and threadidx == 1: logging.info('Connected to Ensembl database.')
+            # Pass reference to ensembl, so it can know the chromosome sizes
+            self.ensembl = Ensembl(options, genelist, transcriptlist, codon_usage[0], self.reference)
+            if options.args['logfile'] and threadidx == 1:
+                logging.info('Connected to Ensembl database.')
         else:
             self.ensembl = None
 
         if (not options.args['dbsnp'] == '.') and (not options.args['dbsnp'] == ''):
             self.dbsnp = dbSNP(options)
             if options.args['logfile'] and threadidx == 1: logging.info('Connected to dbSNP database.')
         else:
             self.dbsnp = None
 
-        # Reference genome
-        self.reference = Reference(options)
-        if options.args['logfile'] and threadidx == 1: logging.info('Connected to reference genome.')
 
         # Target BED file
         if (not options.args['target'] == '.') and (not options.args['target'] == ''):
             self.targetBED = pysam.Tabixfile(options.args['target'], parser=pysam.asBed())
         else:
             self.targetBED = None
 
+
+        # Reading (new) transcript2protein map for HGVSP annotation
+        if options.args['logfile'] and threadidx == 1:
+            logging.info("INFO: reading transcript2protein file\n")
+        options.transcript2protein = core.read_dict(options, 'transcript2protein')
+        if options.args['logfile'] and threadidx == 1:
+            logging.info("transcript2protein has " + str(len(options.transcript2protein)) + " mappings\n")
+
         if not copts.stdout and threadidx == 1: initProgressInfo()
 
         # Reading (new) transcript2protein map for HGVSP annotation
         if options.args['logfile'] and threadidx == 1:
             logging.info("INFO: reading transcript2protein file\n")
         options.transcript2protein = core.read_dict(options, 'transcript2protein')
         if options.args['logfile'] and threadidx == 1:
@@ -280,33 +292,34 @@
             # Considering lines between startline and endline only
             if counter < int(self.startline): continue
             if not self.endline == '':
                 if counter > int(self.endline): break
 
             line = line.strip()
             if line == '': continue
-
+#            sys.stderr.write("line="+line+"\n")
             # Printing out progress information
             if not self.copts.stdout and self.threadidx == 1:
                 if counter % 1000 == 0:
                     printProgressInfo(counter, int(self.numOfRecords / self.copts.threads))
 
             # Parsing record from input file
-            record = Record(line, self.options, self.targetBED)
+            record = Record(line, self.options, self.targetBED,self.reference)
 
-            # Filtering out REFCALL records
+            # Filtering out REFCALL records .. from original VCF annotation
             if record.filter == 'REFCALL': continue
 
             # Filtering record, if required
             if self.options.args['filter'] and not record.filter == 'PASS': continue
 
-            # Only include records of allowed chromosome names
+            # Only annotate records of allowed chromosome names
             if record.chrom not in self.chroms:
                 logging.warning(
-                    "\t!!!!!!Chromosome " + record.chrom + " not found, skipping annotation, but still printing!!!!!!\n")
+                    "\t!!!!!!Chromosome " + record.chrom + " not found, skipping annotation, "+
+                    "but still outputting in VCF as long as within target region (if specified)!!!!!!\n")
             else:
                 # Annotating the record based on the Ensembl, dbSNP and reference data
                 record.annotate(self.ensembl, self.dbsnp, self.reference, self.impactdir)
 
             # Writing annotated record to output file
             record.output(self.options.args['outputformat'], self.outfile, self.options, self.genelist,
                           self.transcriptlist, self.snplist, self.copts.stdout)
@@ -349,15 +362,17 @@
 
     # Initializing log file
     if options.args['logfile']:
         logging.basicConfig(filename=copts.output + '.log', filemode='w',
                             format='%(asctime)s %(levelname)s: %(message)s', level=logging.DEBUG)
 
     # Printing out version.py information and start time
-    if not copts.stdout: starttime = printStartInfo(version)
+
+    if not copts.stdout:
+        starttime = printStartInfo(version)
     if options.args['logfile']:
         logging.info('CAVA ' + version + ' started.')
 
     # Checking if options specified in the configuration file are correct
     core.checkOptions(options)
 
     # Printing out configuration, input and output file names
@@ -368,14 +383,15 @@
     genelist = core.readSet(options, 'genelist')
     transcriptlist = core.readSet(options, 'transcriptlist')
     snplist = core.readSet(options, 'snplist')
 
     # Reading (new) transcript2protein map for HGVSP annotation
     print("INFO: reading transcript2protein file\n")
     options.transcript2protein = core.read_dict(options, 'transcript2protein')
+
     print("transcript2protein has " + str(len(options.transcript2protein)) + " mappings\n")
     # Parsing @impactdef string
     if not (options.args['impactdef'] == '.' or options.args['impactdef'] == ''):
         impactdir = dict()
         valuev = options.args['impactdef'].split('|')
         for i in range(len(valuev)):
             classv = valuev[i].split(',')
@@ -399,14 +415,15 @@
     header = readHeader(copts.input)
     core.writeHeader(options, '\n'.join(header), outfile, copts.stdout, version)
     outfile.close()
 
     # Find break points in the input file
     breaks = findFileBreaks(copts.input, copts.threads)
 
+
     # Initializing annotation processes
     threadidx = 0
     processes = []
     for (startline, endline) in breaks:
         threadidx += 1
         processes.append(
             SingleJob(threadidx, options, copts, startline, endline, genelist, transcriptlist, snplist, impactdir,
@@ -418,10 +435,11 @@
     for process in processes:
         process.join()
 
     # Merging tmp files
     if copts.threads > 1:
         mergeTmpFiles(copts.output, options.args['outputformat'], copts.threads)
 
+
     # Printing out summary information and end time
     if not copts.stdout:
         printEndInfo(options, copts, starttime)
```

### Comparing `CAVA-2.0.5/setup.py` & `CAVA-2.0.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,19 +4,20 @@
     version = version_file.read().strip()
 
 with open('requirements.txt') as requires_file:
     requires = requires_file.read().split('\n')
 
 setup(
     name='CAVA',
+    python_requires=">=3.7",
     version=version,
     description='CAVA (Clinical Annotation of VAriants)',
     url='https://github.com/Steven-N-Hart/CAVA',
-    author='Steven-N-Hart',
-    author_email='hart.steven@mayo.edu',
+    author='Steven-N-Hart, Hugues-Sicotte',
+    author_email='hart.steven@mayo.edu, sicotte.hugues@mayo.edu',
     license='MIT',
     packages=['cava', 'cava.utils', 'cava.ensembldb'],
     install_requires=requires,
     zip_safe=False,
     include_package_data=True,
     test_suite='tests',
     tests_require=['wget'],
```

### Comparing `CAVA-2.0.5/test/test_csn.py` & `CAVA-2.0.7/cava/test/test_csn.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         expected = ('_p.Arg2Ter', ('2', 'R', 'X'))
         self.assertEqual(actual, expected)
 
     def test_makeProteinString_delMet1(self):
         print("Testing deletion of Initial Methionine")
         variant = Variant("chr1", 1000, "C", "T")
         actual = makeProteinString(variant, "MLRX", "LRX", 1)
-        expected = ('_p.?', ('1', 'M', '-'))
+        expected = ('_p.Met1?', ('1', 'M', '-'))
         self.assertEqual(actual, expected)
 
     def test_makeProteinString_del2(self):
         print("Testing deletion 2AA")
         variant = Variant("chr1", 1000, "C", "T")
         actual = makeProteinString(variant, "MLRYX", "MYX", 1)
         expected = ('_p.Leu2_Arg3del', ('2-3', 'LR', '-'))
@@ -83,29 +83,29 @@
         expected = ('_p.Leu2_Arg3insLeuTer', ('2-3', '-', 'LX'))
         self.assertEqual(actual, expected)
 
     def test_makeProteinString_checkShortExt(self):
         print("Testing checking extension")
         variant = Variant("chr1", 1000, "C", "T")
         actual = makeProteinString(variant, "MLRX", "MLRQX", 12)
-        expected = ('_p.Ter4GlnextX2', ('4', 'X', 'QX'))
+        expected = ('_p.Ter4GlnextTer1', ('4', 'X', 'QX'))
         self.assertEqual(actual, expected)
 
     def test_makeProteinString_checkLongExtInPhase(self):
         print("Testing checking long extension in phase")
         variant = Variant("chr1", 1000, "C", "T")
         actual = makeProteinString(variant, "MLRX", "MLRQLVYX", 12)
-        expected = ('_p.Ter4GlnextX5', ('4', 'X', 'QLVYX'))
+        expected = ('_p.Ter4GlnextTer4', ('4', 'X', 'QLVYX'))
         self.assertEqual(actual, expected)
 
     def test_makeProteinString_checkLongExtnotPhase(self):
         print("Testing checking long extension not in phase")
         variant = Variant("chr1", 1000, "C", "T")
         actual = makeProteinString(variant, "MLRX", "MLRQLVYX", 11)
-        expected = ('_p.Ter4GlnextX5', ('4', 'X', 'QLVYX'))
+        expected = ('_p.Ter4GlnextTer4', ('4', 'X', 'QLVYX'))
         self.assertEqual(actual, expected)
 
     def test_makeProteinString_checkShortFS(self):
         print("Testing checking frameshift with mutprot<prot")
         variant = Variant("chr1", 1000, "C", "T")
         actual = makeProteinString(variant, "MLRYQVRX", "MLSVX", 8)
         expected = ('_p.Arg3SerfsTer3', ('3', 'R', 'SVX'))
@@ -239,17 +239,17 @@
         expected = ('_p.Leu3Ter', ('3', 'L', 'X'))
         self.assertEqual(actual, expected)
 
     def test_makeProteinString_Met1toAA(self):
         print("Testing mutation of  Methionine")
         variant = Variant("chr1", 1000, "C", "T")
         actual = makeProteinString(variant, "MLRX", "LLRX", 1)
-        expected = ('_p.?', ('1', 'M', 'L'))
+        expected = ('_p.Met1?', ('1', 'M', 'L'))
         self.assertEqual(actual, expected)
 
 
     def test_makeProteinString_Met1toAAS(self):
         print("Testing mutation of  2 AA (including Methionine)")
         variant = Variant("chr1", 1000, "CTCT", "TCAG")
         actual = makeProteinString(variant, "MLRX", "LRRX", 1)
-        expected = ('_p.?', ('1-2', 'ML', 'LR'))
+        expected = ('_p.Met1?', ('1', 'M', 'L'))  # Once the methionine is modified, the rest of the protein translation does not matter.
         self.assertEqual(actual, expected)
```

