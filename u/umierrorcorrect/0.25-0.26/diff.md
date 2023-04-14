# Comparing `tmp/umierrorcorrect-0.25.tar.gz` & `tmp/umierrorcorrect-0.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/xsteto/new/umierrorcorrect/dist/tmpknog79x4/umierrorcorrect-0.25.tar", last modified: Thu Apr  6 07:57:28 2023, max compression
+gzip compressed data, was "/home/xsteto/new/umierrorcorrect/dist/tmpzdatilqv/umierrorcorrect-0.26.tar", last modified: Fri Apr 14 12:15:47 2023, max compression
```

## Comparing `umierrorcorrect-0.25.tar` & `umierrorcorrect-0.26.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 xsteto    (1208) unix       (110)        0 2023-04-06 07:57:28.000000 umierrorcorrect-0.25/
-drwxrwxr-x   0 xsteto    (1208) unix       (110)        0 2023-04-06 07:57:28.000000 umierrorcorrect-0.25/umierrorcorrect/
-drwxrwxr-x   0 xsteto    (1208) unix       (110)        0 2023-04-06 07:57:28.000000 umierrorcorrect-0.25/umierrorcorrect/src/
--rw-rw-r--   0 xsteto    (1208) unix       (110)        0 2021-11-24 14:09:37.000000 umierrorcorrect-0.25/umierrorcorrect/src/__init__.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)     4739 2023-03-30 12:01:41.000000 umierrorcorrect-0.25/umierrorcorrect/src/check_args.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)    12262 2022-03-16 12:25:44.000000 umierrorcorrect-0.25/umierrorcorrect/src/get_cons_info.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)    18485 2023-04-05 11:12:26.000000 umierrorcorrect-0.25/umierrorcorrect/src/get_consensus3.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)     3756 2022-03-22 07:54:18.000000 umierrorcorrect-0.25/umierrorcorrect/src/get_regions_from_bed.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)     6566 2022-08-30 07:25:37.000000 umierrorcorrect-0.25/umierrorcorrect/src/group.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)      868 2022-03-22 13:55:44.000000 umierrorcorrect-0.25/umierrorcorrect/src/handle_sequences.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)     7529 2023-03-30 12:01:41.000000 umierrorcorrect-0.25/umierrorcorrect/src/umi_cluster.py
--rw-rw-r--   0 xsteto    (1208) unix       (110)        0 2021-11-24 14:09:37.000000 umierrorcorrect-0.25/umierrorcorrect/__init__.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)     7853 2023-04-06 07:06:12.000000 umierrorcorrect-0.25/umierrorcorrect/call_variants.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)     2889 2022-01-12 10:39:15.000000 umierrorcorrect-0.25/umierrorcorrect/downsampling_plots.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)     1165 2021-11-24 14:09:37.000000 umierrorcorrect-0.25/umierrorcorrect/filter_bam.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)     1895 2021-11-24 14:09:37.000000 umierrorcorrect-0.25/umierrorcorrect/filter_cons.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)     2669 2021-11-24 14:09:37.000000 umierrorcorrect-0.25/umierrorcorrect/filter_cons2.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)     1806 2021-11-24 14:09:37.000000 umierrorcorrect-0.25/umierrorcorrect/filter_vcf.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)     4254 2021-11-24 14:09:37.000000 umierrorcorrect-0.25/umierrorcorrect/fit_background_model.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)    12378 2023-03-30 12:01:41.000000 umierrorcorrect-0.25/umierrorcorrect/get_consensus_statistics.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)    12645 2022-02-01 13:00:49.000000 umierrorcorrect-0.25/umierrorcorrect/get_consensus_statistics2.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)     1798 2022-03-22 09:26:19.000000 umierrorcorrect-0.25/umierrorcorrect/get_umi_cluster_info.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)    10143 2022-04-25 08:51:53.000000 umierrorcorrect-0.25/umierrorcorrect/preprocess.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)     5643 2023-03-30 12:01:41.000000 umierrorcorrect-0.25/umierrorcorrect/run_mapping.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)     8899 2023-04-05 11:12:26.000000 umierrorcorrect-0.25/umierrorcorrect/run_umierrorcorrect.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)     3226 2021-11-24 14:09:38.000000 umierrorcorrect-0.25/umierrorcorrect/test_cons_info_indel.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)    25528 2023-04-06 07:06:12.000000 umierrorcorrect-0.25/umierrorcorrect/umi_error_correct.py
--rwxrwxr-x   0 xsteto    (1208) unix       (110)       19 2023-04-06 07:56:07.000000 umierrorcorrect-0.25/umierrorcorrect/version.py
-drwxrwxr-x   0 xsteto    (1208) unix       (110)        0 2023-04-06 07:57:28.000000 umierrorcorrect-0.25/umierrorcorrect.egg-info/
--rw-rw-r--   0 xsteto    (1208) unix       (110)     3129 2023-04-06 07:57:28.000000 umierrorcorrect-0.25/umierrorcorrect.egg-info/PKG-INFO
--rw-rw-r--   0 xsteto    (1208) unix       (110)     1156 2023-04-06 07:57:28.000000 umierrorcorrect-0.25/umierrorcorrect.egg-info/SOURCES.txt
--rw-rw-r--   0 xsteto    (1208) unix       (110)        1 2023-04-06 07:57:28.000000 umierrorcorrect-0.25/umierrorcorrect.egg-info/dependency_links.txt
--rw-rw-r--   0 xsteto    (1208) unix       (110)        1 2022-01-24 15:00:25.000000 umierrorcorrect-0.25/umierrorcorrect.egg-info/not-zip-safe
--rw-rw-r--   0 xsteto    (1208) unix       (110)       30 2023-04-06 07:57:28.000000 umierrorcorrect-0.25/umierrorcorrect.egg-info/requires.txt
--rw-rw-r--   0 xsteto    (1208) unix       (110)       16 2023-04-06 07:57:28.000000 umierrorcorrect-0.25/umierrorcorrect.egg-info/top_level.txt
--rwxrwxr-x   0 xsteto    (1208) unix       (110)     1065 2021-11-29 10:11:37.000000 umierrorcorrect-0.25/LICENSE.txt
--rw-rw-r--   0 xsteto    (1208) unix       (110)     2715 2023-04-05 11:12:26.000000 umierrorcorrect-0.25/README.md
--rw-rw-r--   0 xsteto    (1208) unix       (110)       79 2023-04-06 07:57:28.000000 umierrorcorrect-0.25/setup.cfg
--rwxrwxr-x   0 xsteto    (1208) unix       (110)     1447 2023-03-30 12:01:41.000000 umierrorcorrect-0.25/setup.py
--rw-rw-r--   0 xsteto    (1208) unix       (110)     3129 2023-04-06 07:57:28.000000 umierrorcorrect-0.25/PKG-INFO
+drwxrwxr-x   0 xsteto    (1208) unix       (110)        0 2023-04-14 12:15:47.000000 umierrorcorrect-0.26/
+drwxrwxr-x   0 xsteto    (1208) unix       (110)        0 2023-04-14 12:15:46.000000 umierrorcorrect-0.26/umierrorcorrect/
+drwxrwxr-x   0 xsteto    (1208) unix       (110)        0 2023-04-14 12:15:47.000000 umierrorcorrect-0.26/umierrorcorrect/src/
+-rw-rw-r--   0 xsteto    (1208) unix       (110)        0 2021-11-24 14:09:37.000000 umierrorcorrect-0.26/umierrorcorrect/src/__init__.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)     4943 2023-04-14 12:03:38.000000 umierrorcorrect-0.26/umierrorcorrect/src/check_args.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)    12262 2022-03-16 12:25:44.000000 umierrorcorrect-0.26/umierrorcorrect/src/get_cons_info.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)    18485 2023-04-06 11:29:48.000000 umierrorcorrect-0.26/umierrorcorrect/src/get_consensus3.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)     3756 2022-03-22 07:54:18.000000 umierrorcorrect-0.26/umierrorcorrect/src/get_regions_from_bed.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)     6566 2022-08-30 07:25:37.000000 umierrorcorrect-0.26/umierrorcorrect/src/group.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)      868 2022-03-22 13:55:44.000000 umierrorcorrect-0.26/umierrorcorrect/src/handle_sequences.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)     7529 2023-03-30 12:01:41.000000 umierrorcorrect-0.26/umierrorcorrect/src/umi_cluster.py
+-rw-rw-r--   0 xsteto    (1208) unix       (110)        0 2021-11-24 14:09:37.000000 umierrorcorrect-0.26/umierrorcorrect/__init__.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)     7853 2023-04-06 10:10:04.000000 umierrorcorrect-0.26/umierrorcorrect/call_variants.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)     2889 2022-01-12 10:39:15.000000 umierrorcorrect-0.26/umierrorcorrect/downsampling_plots.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)     1165 2021-11-24 14:09:37.000000 umierrorcorrect-0.26/umierrorcorrect/filter_bam.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)     1895 2021-11-24 14:09:37.000000 umierrorcorrect-0.26/umierrorcorrect/filter_cons.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)     2669 2021-11-24 14:09:37.000000 umierrorcorrect-0.26/umierrorcorrect/filter_cons2.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)     1806 2021-11-24 14:09:37.000000 umierrorcorrect-0.26/umierrorcorrect/filter_vcf.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)     4254 2021-11-24 14:09:37.000000 umierrorcorrect-0.26/umierrorcorrect/fit_background_model.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)    12378 2023-03-30 12:01:41.000000 umierrorcorrect-0.26/umierrorcorrect/get_consensus_statistics.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)    12645 2022-02-01 13:00:49.000000 umierrorcorrect-0.26/umierrorcorrect/get_consensus_statistics2.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)     1798 2022-03-22 09:26:19.000000 umierrorcorrect-0.26/umierrorcorrect/get_umi_cluster_info.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)    11999 2023-04-14 12:03:38.000000 umierrorcorrect-0.26/umierrorcorrect/preprocess.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)     5643 2023-03-30 12:01:41.000000 umierrorcorrect-0.26/umierrorcorrect/run_mapping.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)     9404 2023-04-14 12:03:38.000000 umierrorcorrect-0.26/umierrorcorrect/run_umierrorcorrect.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)     3226 2021-11-24 14:09:38.000000 umierrorcorrect-0.26/umierrorcorrect/test_cons_info_indel.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)    25529 2023-04-14 12:03:38.000000 umierrorcorrect-0.26/umierrorcorrect/umi_error_correct.py
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)       19 2023-04-14 12:12:43.000000 umierrorcorrect-0.26/umierrorcorrect/version.py
+drwxrwxr-x   0 xsteto    (1208) unix       (110)        0 2023-04-14 12:15:47.000000 umierrorcorrect-0.26/umierrorcorrect.egg-info/
+-rw-rw-r--   0 xsteto    (1208) unix       (110)     3129 2023-04-14 12:15:44.000000 umierrorcorrect-0.26/umierrorcorrect.egg-info/PKG-INFO
+-rw-rw-r--   0 xsteto    (1208) unix       (110)     1156 2023-04-14 12:15:45.000000 umierrorcorrect-0.26/umierrorcorrect.egg-info/SOURCES.txt
+-rw-rw-r--   0 xsteto    (1208) unix       (110)        1 2023-04-14 12:15:44.000000 umierrorcorrect-0.26/umierrorcorrect.egg-info/dependency_links.txt
+-rw-rw-r--   0 xsteto    (1208) unix       (110)        1 2022-01-24 15:00:25.000000 umierrorcorrect-0.26/umierrorcorrect.egg-info/not-zip-safe
+-rw-rw-r--   0 xsteto    (1208) unix       (110)       30 2023-04-14 12:15:44.000000 umierrorcorrect-0.26/umierrorcorrect.egg-info/requires.txt
+-rw-rw-r--   0 xsteto    (1208) unix       (110)       16 2023-04-14 12:15:44.000000 umierrorcorrect-0.26/umierrorcorrect.egg-info/top_level.txt
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)     1065 2021-11-29 10:11:37.000000 umierrorcorrect-0.26/LICENSE.txt
+-rw-rw-r--   0 xsteto    (1208) unix       (110)     2715 2023-04-06 10:10:04.000000 umierrorcorrect-0.26/README.md
+-rw-rw-r--   0 xsteto    (1208) unix       (110)       79 2023-04-14 12:15:47.000000 umierrorcorrect-0.26/setup.cfg
+-rwxrwxr-x   0 xsteto    (1208) unix       (110)     1447 2023-03-30 12:01:41.000000 umierrorcorrect-0.26/setup.py
+-rw-rw-r--   0 xsteto    (1208) unix       (110)     3129 2023-04-14 12:15:47.000000 umierrorcorrect-0.26/PKG-INFO
```

### Comparing `umierrorcorrect-0.25/umierrorcorrect/src/check_args.py` & `umierrorcorrect-0.26/umierrorcorrect/src/check_args.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,18 @@
 
 def check_args_fastq(args):
     '''Function for checking arguments'''
     args.output_path = check_output_directory(args.output_path)
     is_pigz=is_tool('pigz')
     is_gzip=is_tool('gzip')
     is_bwa=is_tool('bwa')
+    if args.adapter_trimming:
+        is_cutadapt=is_tool('cutadapt')
+        if not is_cutadapt:
+            raise ValueError('Cannot find program "cutadapt". Please install it and add it to the path.')
     if not is_bwa:
         raise ValueError('Cannot find program "bwa". Please install it and add it to the path.')
     if is_pigz:
         args.gziptool='pigz'
     elif is_gzip:
         args.gziptool='gzip'
     else:
```

### Comparing `umierrorcorrect-0.25/umierrorcorrect/src/get_cons_info.py` & `umierrorcorrect-0.26/umierrorcorrect/src/get_cons_info.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.25/umierrorcorrect/src/get_consensus3.py` & `umierrorcorrect-0.26/umierrorcorrect/src/get_consensus3.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.25/umierrorcorrect/src/get_regions_from_bed.py` & `umierrorcorrect-0.26/umierrorcorrect/src/get_regions_from_bed.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.25/umierrorcorrect/src/group.py` & `umierrorcorrect-0.26/umierrorcorrect/src/group.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.25/umierrorcorrect/src/handle_sequences.py` & `umierrorcorrect-0.26/umierrorcorrect/src/handle_sequences.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.25/umierrorcorrect/src/umi_cluster.py` & `umierrorcorrect-0.26/umierrorcorrect/src/umi_cluster.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.25/umierrorcorrect/call_variants.py` & `umierrorcorrect-0.26/umierrorcorrect/call_variants.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.25/umierrorcorrect/downsampling_plots.py` & `umierrorcorrect-0.26/umierrorcorrect/downsampling_plots.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.25/umierrorcorrect/filter_bam.py` & `umierrorcorrect-0.26/umierrorcorrect/filter_bam.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.25/umierrorcorrect/filter_cons.py` & `umierrorcorrect-0.26/umierrorcorrect/filter_cons.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.25/umierrorcorrect/filter_cons2.py` & `umierrorcorrect-0.26/umierrorcorrect/filter_cons2.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.25/umierrorcorrect/filter_vcf.py` & `umierrorcorrect-0.26/umierrorcorrect/filter_vcf.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.25/umierrorcorrect/fit_background_model.py` & `umierrorcorrect-0.26/umierrorcorrect/fit_background_model.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.25/umierrorcorrect/get_consensus_statistics.py` & `umierrorcorrect-0.26/umierrorcorrect/get_consensus_statistics.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.25/umierrorcorrect/get_consensus_statistics2.py` & `umierrorcorrect-0.26/umierrorcorrect/get_consensus_statistics2.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.25/umierrorcorrect/get_umi_cluster_info.py` & `umierrorcorrect-0.26/umierrorcorrect/get_umi_cluster_info.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.25/umierrorcorrect/preprocess.py` & `umierrorcorrect-0.26/umierrorcorrect/preprocess.py`

 * *Files 18% similar despite different names*

```diff
@@ -53,14 +53,18 @@
     parser.add_argument('-tmpdir', '--tmp_dir', dest='tmpdir', 
                         help="temp directory where the temporary files are written and then removed. Should be the \
                               scratch directory on the node. Default is a temp directory in the output folder.")
     parser.add_argument('-f', '--force', dest='force',action='store_true',
                         help='Include this flag to force output files to be overwritten')
     parser.add_argument('-t', '--num_threads', dest='num_threads', 
                         help='Number of threads to run the program on. Default=%(default)s', default='1')
+    parser.add_argument('-trim','--adapter_trimming', dest='adapter_trimming', action='store_true',
+                        help="Include this flag to perform automatic 3' adapter trimming (readthrough adapters).")
+    parser.add_argument('-a', '--adapter_sequence',dest='adapter_sequence',
+                        help="Adapter to trim off 3' end. Select one of 'illumina','nextera' or 'small-rna' or enter a custom sequence (see documentation). Default=%(default)s (AGATCGGAAGAGC)", default='illumina')
     args = parser.parse_args(sys.argv[1:])
     logging.basicConfig(format='%(asctime)s %(message)s', datefmt='%Y-%m-%d %H:%M:%S', level=logging.DEBUG)
     logging.info('Starting UMI Error Correct')
 
     return(args)
 
 
@@ -173,14 +177,44 @@
         if args.mode == 'paired':
             r1file = run_unpigz(args.read1, newtmpdir, args.num_threads, args.gziptool)
             r2file = run_unpigz(args.read2, newtmpdir, args.num_threads, args.gziptool)
         else:
             r1file = run_unpigz(args.read1, newtmpdir, args.num_threads, args.gziptool)
 
     logging.info('Writing output files to {}'.format(args.output_path))
+    if args.adapter_trimming==True:
+        if args.adapter_sequence.lower()=='illumina':
+            adapter='AGATCGGAAGAGC'
+        elif args.adapter_sequence.lower()=='nextera':
+            adapter='CTGTCTCTTATA'
+        elif args.adapter_sequence.lower()=='small-rna':
+            adapter='ATGGAATTCTCG'
+        else:
+            adapter=args.adapter_sequence.upper()
+    
+        if args.mode == 'single':
+            outfilename = args.output_path + '/' + args.sample_name + '_trimmed.fastq'
+            command=['cutadapt', '-a', adapter, '-o', outfilename, '-O', '3', '-m', '20', r1file]
+        else:
+            outfile1 = args.output_path + '/' + args.sample_name + '_R1_trimmed.fastq'
+            outfile2 = args.output_path + '/' + args.sample_name + '_R2_trimmed.fastq'
+            command=['cutadapt', '-a', adapter, '-A', adapter,'-o', outfile1, '-p', outfile2, '-O', '3', '-m', '20', r1file,r2file]
+        logging.info("Performing adapter trimming using cutadapt with adapter sequence {}".format(adapter))
+        p = subprocess.Popen(command, stdout=subprocess.PIPE)
+        p.communicate()
+        p.wait()
+        if args.mode=='single':
+            os.remove(r1file)
+            r1file=outfilename
+        else:
+            os.remove(r1file)
+            os.remove(r2file)
+            r1file=outfile1
+            r2file=outfile2
+
     if args.mode == 'single':
         outfilename = args.output_path + '/' + args.sample_name + '_umis_in_header.fastq'
         nseqs = preprocess_se(r1file, outfilename, args.umi_length, args.spacer_length)
         run_pigz(outfilename, args.num_threads, args.gziptool)
         os.remove(r1file)
         os.rmdir(newtmpdir)
         fastqfiles=[outfilename + '.gz']
```

### Comparing `umierrorcorrect-0.25/umierrorcorrect/run_mapping.py` & `umierrorcorrect-0.26/umierrorcorrect/run_mapping.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.25/umierrorcorrect/run_umierrorcorrect.py` & `umierrorcorrect-0.26/umierrorcorrect/run_umierrorcorrect.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,14 +38,18 @@
                         help='Path to a BED file defining the targeted regions, i.e. chromosomal positions. \
                              The Bed file is used for annotation.')
     group1.add_argument('-s', '--sample_name', dest='sample_name', 
                         help='Sample name that will be used as base name for the output files. \
                               If excluded the sample name will be extracted from the fastq files.')
     group1.add_argument('-remove', '--remove_large_files',  dest='remove_large_files', action='store_true',\
                         help='Include this flag to emove the original Fastq and BAM files (reads without error correction).')
+    group1.add_argument('-trim','--adapter_trimming', dest='adapter_trimming', action='store_true',
+                        help="Include this flag to perform automatic 3' adapter trimming (readthrough adapters).")
+    group1.add_argument('-a', '--adapter_sequence',dest='adapter_sequence',
+                        help="Adapter to trim off 3' end. Select one of 'illumina','nextera' or 'small-rna' or enter a custom sequence (see documentation). Default=%(default)s (AGATCGGAAGAGC)", default='illumina')
     group2 = parser.add_argument_group('UMI definition options')
     group2.add_argument('-ul', '--umi_length', dest='umi_length', 
                         help='Length of UMI sequence (number of nucleotides). The UMI is assumed to \
                              be located at the start of the read. Required', required=True)
     group2.add_argument('-sl', '--spacer_length', dest='spacer_length', 
                         help='Length of spacer (The number of nucleotides between the UMI and the beginning \
                              of the read). The UMI + spacer will be trimmed off, and the spacer will be \
```

### Comparing `umierrorcorrect-0.25/umierrorcorrect/test_cons_info_indel.py` & `umierrorcorrect-0.26/umierrorcorrect/test_cons_info_indel.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.25/umierrorcorrect/umi_error_correct.py` & `umierrorcorrect-0.26/umierrorcorrect/umi_error_correct.py`

 * *Files 0% similar despite different names*

```diff
@@ -528,15 +528,15 @@
     if args.bed_file:
         bedregions = read_bed(args.bed_file)
         bedregions = sort_regions(bedregions)
         if group_method=='fromBed':
             bedregions = merge_regions(bedregions, 0)
     else:
         bedregions = []
-    print(bedregions)
+    #print(bedregions)
     if group_method=='fromTag':
         bamfilelist = cluster_umis_all_regions(regions, ends, edit_distance_threshold,
                                            args.sample_name, args.bam_file, args.output_path,
                                            args.include_singletons, fasta, bedregions,
                                            num_cpus, args.indel_frequency_threshold,
                                            args.consensus_frequency_threshold,
                                            args.regions_from_tag, starts)
```

### Comparing `umierrorcorrect-0.25/umierrorcorrect.egg-info/PKG-INFO` & `umierrorcorrect-0.26/umierrorcorrect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: umierrorcorrect
-Version: 0.25
+Version: 0.26
 Summary: UMI error correct
 Home-page: http://github.com/stahlberggroup/umierrorcorrect
 Author: Tobias Osterlund
 Author-email: tobias.osterlund@gu.se
 License: mit
-Download-URL: https://github.com/stahlberggroup/umierrorcorrect/archive/0.25.tar.gz
+Download-URL: https://github.com/stahlberggroup/umierrorcorrect/archive/0.26.tar.gz
 Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 License-File: LICENSE.txt
 
 # umierrorcorrect
 
 Pipeline for analyzing barcoded amplicon sequencing data with Unique molecular identifiers (UMI)
```

### Comparing `umierrorcorrect-0.25/umierrorcorrect.egg-info/SOURCES.txt` & `umierrorcorrect-0.26/umierrorcorrect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.25/LICENSE.txt` & `umierrorcorrect-0.26/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.25/README.md` & `umierrorcorrect-0.26/README.md`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.25/setup.py` & `umierrorcorrect-0.26/setup.py`

 * *Files identical despite different names*

### Comparing `umierrorcorrect-0.25/PKG-INFO` & `umierrorcorrect-0.26/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: umierrorcorrect
-Version: 0.25
+Version: 0.26
 Summary: UMI error correct
 Home-page: http://github.com/stahlberggroup/umierrorcorrect
 Author: Tobias Osterlund
 Author-email: tobias.osterlund@gu.se
 License: mit
-Download-URL: https://github.com/stahlberggroup/umierrorcorrect/archive/0.25.tar.gz
+Download-URL: https://github.com/stahlberggroup/umierrorcorrect/archive/0.26.tar.gz
 Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 License-File: LICENSE.txt
 
 # umierrorcorrect
 
 Pipeline for analyzing barcoded amplicon sequencing data with Unique molecular identifiers (UMI)
```

