# Comparing `tmp/bmxp-0.0.8.tar.gz` & `tmp/bmxp-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmxp-0.0.8.tar", last modified: Tue Jan  3 22:52:06 2023, max compression
+gzip compressed data, was "bmxp-0.0.9.tar", last modified: Tue Jan  3 23:14:18 2023, max compression
```

## Comparing `bmxp-0.0.8.tar` & `bmxp-0.0.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-01-03 22:52:06.591506 bmxp-0.0.8/
--rw-rw-rw-   0        0        0     1093 2022-11-18 17:19:36.000000 bmxp-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      189 2022-12-21 20:29:36.000000 bmxp-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     1257 2023-01-03 22:52:06.590376 bmxp-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      750 2022-11-22 21:07:50.000000 bmxp-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-01-03 22:52:06.481588 bmxp-0.0.8/bmxp/
-drwxrwxrwx   0        0        0        0 2023-01-03 22:52:06.527138 bmxp-0.0.8/bmxp/eclipse/
--rw-rw-rw-   0        0        0    47118 2022-11-18 17:19:36.000000 bmxp-0.0.8/bmxp/eclipse/__init__.py
--rw-rw-rw-   0        0        0     4347 2022-11-18 17:19:36.000000 bmxp-0.0.8/bmxp/eclipse/eclipse_example.py
-drwxrwxrwx   0        0        0        0 2023-01-03 22:52:06.534746 bmxp-0.0.8/bmxp/gravity/
--rw-rw-rw-   0        0        0     9327 2023-01-03 22:49:39.000000 bmxp-0.0.8/bmxp/gravity/__init__.py
--rw-rw-rw-   0        0        0     7848 2023-01-03 22:32:45.000000 bmxp-0.0.8/bmxp/gravity/correlation.c
--rw-rw-rw-   0        0        0    17408 2023-01-03 22:32:58.000000 bmxp-0.0.8/bmxp/gravity/correlation.dll
--rw-rw-rw-   0        0        0    16120 2023-01-03 22:32:58.000000 bmxp-0.0.8/bmxp/gravity/correlation.so
--rw-rw-rw-   0        0        0      615 2023-01-03 18:46:44.000000 bmxp-0.0.8/bmxp/gravity/gravity_example.py
-drwxrwxrwx   0        0        0        0 2023-01-03 22:52:06.523614 bmxp-0.0.8/bmxp.egg-info/
--rw-rw-rw-   0        0        0     1257 2023-01-03 22:52:06.000000 bmxp-0.0.8/bmxp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      633 2023-01-03 22:52:06.000000 bmxp-0.0.8/bmxp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-03 22:52:06.000000 bmxp-0.0.8/bmxp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-01-03 22:52:06.000000 bmxp-0.0.8/bmxp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-01-03 22:52:06.000000 bmxp-0.0.8/bmxp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       48 2022-11-18 17:19:36.000000 bmxp-0.0.8/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-01-03 22:52:06.591506 bmxp-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1178 2023-01-03 22:49:24.000000 bmxp-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-03 22:52:06.586388 bmxp-0.0.8/tests/
-drwxrwxrwx   0        0        0        0 2023-01-03 22:52:06.588395 bmxp-0.0.8/tests/__pycache__/
--rw-rw-rw-   0        0        0    18126 2022-11-21 22:24:15.000000 bmxp-0.0.8/tests/__pycache__/test_mseclipse.cpython-38-pytest-7.1.2.pyc
--rw-rw-rw-   0        0        0    18988 2022-11-18 17:19:36.000000 bmxp-0.0.8/tests/example1.csv
--rw-rw-rw-   0        0        0      202 2022-11-18 17:19:36.000000 bmxp-0.0.8/tests/make_pickle.py
--rw-rw-rw-   0        0        0   118411 2022-11-18 17:19:36.000000 bmxp-0.0.8/tests/mseclipse.pickle
--rw-rw-rw-   0        0        0    13087 2022-11-18 17:19:36.000000 bmxp-0.0.8/tests/test1.csv
--rw-rw-rw-   0        0        0    12512 2022-11-18 17:19:36.000000 bmxp-0.0.8/tests/test2.csv
--rw-rw-rw-   0        0        0     1239 2022-11-18 17:19:36.000000 bmxp-0.0.8/tests/test3.csv
--rw-rw-rw-   0        0        0    78529 2022-11-22 21:07:50.000000 bmxp-0.0.8/tests/test_gravity.csv
--rw-rw-rw-   0        0        0      562 2022-11-22 21:07:50.000000 bmxp-0.0.8/tests/test_gravity.py
--rw-rw-rw-   0        0        0     9433 2022-11-18 17:19:36.000000 bmxp-0.0.8/tests/test_mseclipse.py
+drwxrwxrwx   0        0        0        0 2023-01-03 23:14:18.621991 bmxp-0.0.9/
+-rw-rw-rw-   0        0        0     1093 2022-11-18 17:19:36.000000 bmxp-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      189 2022-12-21 20:29:36.000000 bmxp-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     1257 2023-01-03 23:14:18.621991 bmxp-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      750 2022-11-22 21:07:50.000000 bmxp-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-01-03 23:14:18.569976 bmxp-0.0.9/bmxp/
+drwxrwxrwx   0        0        0        0 2023-01-03 23:14:18.595820 bmxp-0.0.9/bmxp/eclipse/
+-rw-rw-rw-   0        0        0    47118 2022-11-18 17:19:36.000000 bmxp-0.0.9/bmxp/eclipse/__init__.py
+-rw-rw-rw-   0        0        0     4347 2022-11-18 17:19:36.000000 bmxp-0.0.9/bmxp/eclipse/eclipse_example.py
+drwxrwxrwx   0        0        0        0 2023-01-03 23:14:18.604455 bmxp-0.0.9/bmxp/gravity/
+-rw-rw-rw-   0        0        0     9327 2023-01-03 23:12:59.000000 bmxp-0.0.9/bmxp/gravity/__init__.py
+-rw-rw-rw-   0        0        0     7896 2023-01-03 23:10:35.000000 bmxp-0.0.9/bmxp/gravity/correlation.c
+-rw-rw-rw-   0        0        0    17408 2023-01-03 23:10:39.000000 bmxp-0.0.9/bmxp/gravity/correlation.dll
+-rw-rw-rw-   0        0        0    16120 2023-01-03 23:10:39.000000 bmxp-0.0.9/bmxp/gravity/correlation.so
+-rw-rw-rw-   0        0        0      615 2023-01-03 18:46:44.000000 bmxp-0.0.9/bmxp/gravity/gravity_example.py
+drwxrwxrwx   0        0        0        0 2023-01-03 23:14:18.593823 bmxp-0.0.9/bmxp.egg-info/
+-rw-rw-rw-   0        0        0     1257 2023-01-03 23:14:18.000000 bmxp-0.0.9/bmxp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      633 2023-01-03 23:14:18.000000 bmxp-0.0.9/bmxp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-01-03 23:14:18.000000 bmxp-0.0.9/bmxp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-01-03 23:14:18.000000 bmxp-0.0.9/bmxp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-01-03 23:14:18.000000 bmxp-0.0.9/bmxp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       48 2022-11-18 17:19:36.000000 bmxp-0.0.9/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-01-03 23:14:18.623051 bmxp-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1178 2023-01-03 23:12:40.000000 bmxp-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-01-03 23:14:18.617886 bmxp-0.0.9/tests/
+drwxrwxrwx   0        0        0        0 2023-01-03 23:14:18.620002 bmxp-0.0.9/tests/__pycache__/
+-rw-rw-rw-   0        0        0    18126 2022-11-21 22:24:15.000000 bmxp-0.0.9/tests/__pycache__/test_mseclipse.cpython-38-pytest-7.1.2.pyc
+-rw-rw-rw-   0        0        0    18988 2022-11-18 17:19:36.000000 bmxp-0.0.9/tests/example1.csv
+-rw-rw-rw-   0        0        0      202 2022-11-18 17:19:36.000000 bmxp-0.0.9/tests/make_pickle.py
+-rw-rw-rw-   0        0        0   118411 2022-11-18 17:19:36.000000 bmxp-0.0.9/tests/mseclipse.pickle
+-rw-rw-rw-   0        0        0    13087 2022-11-18 17:19:36.000000 bmxp-0.0.9/tests/test1.csv
+-rw-rw-rw-   0        0        0    12512 2022-11-18 17:19:36.000000 bmxp-0.0.9/tests/test2.csv
+-rw-rw-rw-   0        0        0     1239 2022-11-18 17:19:36.000000 bmxp-0.0.9/tests/test3.csv
+-rw-rw-rw-   0        0        0    78529 2022-11-22 21:07:50.000000 bmxp-0.0.9/tests/test_gravity.csv
+-rw-rw-rw-   0        0        0      562 2022-11-22 21:07:50.000000 bmxp-0.0.9/tests/test_gravity.py
+-rw-rw-rw-   0        0        0     9433 2022-11-18 17:19:36.000000 bmxp-0.0.9/tests/test_mseclipse.py
```

### Comparing `bmxp-0.0.8/LICENSE` & `bmxp-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bmxp-0.0.8/PKG-INFO` & `bmxp-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmxp
-Version: 0.0.8
+Version: 0.0.9
 Summary: LCMS Processing tools used by the Metabolomics Platform at the Broad Institute.
 Home-page: https://github.com/broadinstitute/bmxp
 Author: Daniel S. Hitchcock
 Author-email: daniel.s.hitchcock@gmail.com
 License: MIT
 Keywords: LCMS,Alignment,Processing,Metabolomics,Clustering
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bmxp-0.0.8/README.md` & `bmxp-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `bmxp-0.0.8/bmxp/eclipse/__init__.py` & `bmxp-0.0.9/bmxp/eclipse/__init__.py`

 * *Files identical despite different names*

### Comparing `bmxp-0.0.8/bmxp/eclipse/eclipse_example.py` & `bmxp-0.0.9/bmxp/eclipse/eclipse_example.py`

 * *Files identical despite different names*

### Comparing `bmxp-0.0.8/bmxp/gravity/__init__.py` & `bmxp-0.0.9/bmxp/gravity/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 correlation.spearman.argtypes = [c_array, c_array, c_int32, c_int32]
 correlation.spearman.restype = c_double
 
 logging.basicConfig()
 LOGGER = logging.getLogger(__name__)
 LOGGER.setLevel(logging.INFO)
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 ECLIPSE_COLUMNS = [
     "RT",
     "MZ",
     "Intensity",
     "Non_Quant",
     "Compound_ID",
     "Adduct",
```

### Comparing `bmxp-0.0.8/bmxp/gravity/correlation.c` & `bmxp-0.0.9/bmxp/gravity/correlation.c`

 * *Files 1% similar despite different names*

```diff
@@ -252,14 +252,16 @@
 
   double result = pearson(xRanks, yRanks, size);
   free(sortedX);
   free(sortedY);
   free(xRanks);
   free(yRanks);
   free(eitherNan);
+  free(y_idx_to_fill);
+  free(x_idx_to_fill);
   return result;
 }
 
 double spearman_array(double* arr, int32_t r1_start, int32_t r2_start, int32_t size, int32_t dropNan) {
   return spearman(&arr[r1_start * size], &arr[r2_start * size], size, dropNan);
 }
```

### Comparing `bmxp-0.0.8/bmxp/gravity/correlation.dll` & `bmxp-0.0.9/bmxp/gravity/correlation.dll`

 * *Files 5% similar despite different names*

#### objdump

```diff
@@ -7,15 +7,15 @@
 	executable
 	line numbers stripped
 	symbols stripped
 	large address aware
 	debugging information removed
 	DLL
 
-Time/Date		Tue Jan  3 22:32:58 2023
+Time/Date		Tue Jan  3 23:10:39 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	2
 MinorLinkerVersion	38
 SizeOfCode		0000000000002400
 SizeOfInitializedData	0000000000004000
 SizeOfUninitializedData	0000000000000200
 AddressOfEntryPoint	0000000000001350
@@ -28,15 +28,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	5
 MinorSubsystemVersion	2
 Win32Version		00000000
 SizeOfImage		0000e000
 SizeOfHeaders		00000400
-CheckSum		00005683
+CheckSum		000058b6
 Subsystem		00000003	(Windows CUI)
 DllCharacteristics	00000160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 SizeOfStackReserve	0000000000200000
 SizeOfStackCommit	0000000000001000
@@ -108,15 +108,15 @@
  0000a028	00000000 00000000 00000000 00000000 00000000
 
 There is an export table in .edata at 0x2e2319000
 
 The Export Tables (interpreted .edata section contents)
 
 Export Flags 			0
-Time/Date stamp 		63b4ad1a
+Time/Date stamp 		63b4b5ef
 Major/Minor 			0/0
 Name 				000000000000908c correlation.dll
 Ordinal Base 			1
 Number in:
 	Export Address Table 		0000000a
 	[Name Pointer/Ordinal] Table	0000000a
 Table Addresses
@@ -126,17 +126,17 @@
 
 Export Address Table -- Ordinal Base 1
 	[   0] +base[   1] 13a0 Export RVA
 	[   1] +base[   2] 1400 Export RVA
 	[   2] +base[   3] 18b0 Export RVA
 	[   3] +base[   4] 1500 Export RVA
 	[   4] +base[   5] 1590 Export RVA
-	[   5] +base[   6] 1fd0 Export RVA
+	[   5] +base[   6] 2010 Export RVA
 	[   6] +base[   7] 18c0 Export RVA
-	[   7] +base[   8] 1fa0 Export RVA
+	[   7] +base[   8] 1fe0 Export RVA
 	[   8] +base[   9] 1470 Export RVA
 	[   9] +base[  10] 13c0 Export RVA
 
 [Ordinal/Name Pointer] Table
 	[   0] comparator
 	[   1] covariance_m
 	[   2] free_p
@@ -160,51 +160,51 @@
  00000002e2316054:	00000002e23113a0 00000002e23113b9 00000002e2317038
  00000002e2316060:	00000002e23113c0 00000002e23113f5 00000002e231703c
  00000002e231606c:	00000002e2311400 00000002e2311461 00000002e2317040
  00000002e2316078:	00000002e2311470 00000002e23114f3 00000002e2317044
  00000002e2316084:	00000002e2311500 00000002e2311581 00000002e2317048
  00000002e2316090:	00000002e2311590 00000002e23118a6 00000002e2317058
  00000002e231609c:	00000002e23118b0 00000002e23118b5 00000002e231707c
- 00000002e23160a8:	00000002e23118c0 00000002e2311fa0 00000002e2317080
- 00000002e23160b4:	00000002e2311fa0 00000002e2311fc9 00000002e231709c
- 00000002e23160c0:	00000002e2311fd0 00000002e2311ff1 00000002e23170a0
- 00000002e23160cc:	00000002e2312000 00000002e231203a 00000002e23170a4
- 00000002e23160d8:	00000002e2312040 00000002e23120aa 00000002e23170ac
- 00000002e23160e4:	00000002e23120b0 00000002e23120cf 00000002e23170b8
- 00000002e23160f0:	00000002e23120d0 00000002e23120ff 00000002e23170bc
- 00000002e23160fc:	00000002e2312100 00000002e2312181 00000002e23170c4
- 00000002e2316108:	00000002e2312190 00000002e2312193 00000002e23170d0
- 00000002e2316114:	00000002e23121a0 00000002e231220a 00000002e23170d4
- 00000002e2316120:	00000002e2312210 00000002e231242d 00000002e23170e0
- 00000002e231612c:	00000002e2312430 00000002e2312715 00000002e23170f0
- 00000002e2316138:	00000002e2312720 00000002e231278b 00000002e2317108
- 00000002e2316144:	00000002e2312790 00000002e2312808 00000002e2317118
- 00000002e2316150:	00000002e2312810 00000002e2312899 00000002e2317124
- 00000002e231615c:	00000002e23128a0 00000002e2312980 00000002e231712c
- 00000002e2316168:	00000002e2312980 00000002e231299e 00000002e2317134
- 00000002e2316174:	00000002e23129a0 00000002e23129b3 00000002e2317138
- 00000002e2316180:	00000002e23129c0 00000002e2312a08 00000002e231713c
- 00000002e231618c:	00000002e2312a10 00000002e2312aaf 00000002e2317140
- 00000002e2316198:	00000002e2312ab0 00000002e2312b31 00000002e231714c
- 00000002e23161a4:	00000002e2312b40 00000002e2312b6b 00000002e2317154
- 00000002e23161b0:	00000002e2312b70 00000002e2312bdc 00000002e231715c
- 00000002e23161bc:	00000002e2312be0 00000002e2312c08 00000002e2317164
- 00000002e23161c8:	00000002e2312c10 00000002e2312c95 00000002e231716c
- 00000002e23161d4:	00000002e2312ca0 00000002e2312d52 00000002e2317174
- 00000002e23161e0:	00000002e2312d60 00000002e2312d63 00000002e231717c
- 00000002e23161ec:	00000002e2312db0 00000002e2312db6 00000002e2317180
- 00000002e23161f8:	00000002e2312dc0 00000002e2312dc6 00000002e2317184
- 00000002e2316204:	00000002e2312dd0 00000002e2312f0f 00000002e2317188
- 00000002e2316210:	00000002e2312f80 00000002e2312fa5 00000002e2317194
- 00000002e231621c:	00000002e2312fb0 00000002e2313084 00000002e2317198
- 00000002e2316228:	00000002e2313090 00000002e2313101 00000002e23171a8
- 00000002e2316234:	00000002e2313110 00000002e231312f 00000002e23171b4
- 00000002e2316240:	00000002e23131a0 00000002e23131e1 00000002e23171bc
- 00000002e231624c:	00000002e23131f0 00000002e23131fc 00000002e23171c4
- 00000002e2316258:	00000002e2313210 00000002e2313215 00000002e23171c8
+ 00000002e23160a8:	00000002e23118c0 00000002e2311fdc 00000002e2317080
+ 00000002e23160b4:	00000002e2311fe0 00000002e2312009 00000002e231709c
+ 00000002e23160c0:	00000002e2312010 00000002e2312031 00000002e23170a0
+ 00000002e23160cc:	00000002e2312040 00000002e231207a 00000002e23170a4
+ 00000002e23160d8:	00000002e2312080 00000002e23120ea 00000002e23170ac
+ 00000002e23160e4:	00000002e23120f0 00000002e231210f 00000002e23170b8
+ 00000002e23160f0:	00000002e2312110 00000002e231213f 00000002e23170bc
+ 00000002e23160fc:	00000002e2312140 00000002e23121c1 00000002e23170c4
+ 00000002e2316108:	00000002e23121d0 00000002e23121d3 00000002e23170d0
+ 00000002e2316114:	00000002e23121e0 00000002e231224a 00000002e23170d4
+ 00000002e2316120:	00000002e2312250 00000002e231246d 00000002e23170e0
+ 00000002e231612c:	00000002e2312470 00000002e2312755 00000002e23170f0
+ 00000002e2316138:	00000002e2312760 00000002e23127cb 00000002e2317108
+ 00000002e2316144:	00000002e23127d0 00000002e2312848 00000002e2317118
+ 00000002e2316150:	00000002e2312850 00000002e23128d9 00000002e2317124
+ 00000002e231615c:	00000002e23128e0 00000002e23129c0 00000002e231712c
+ 00000002e2316168:	00000002e23129c0 00000002e23129de 00000002e2317134
+ 00000002e2316174:	00000002e23129e0 00000002e23129f3 00000002e2317138
+ 00000002e2316180:	00000002e2312a00 00000002e2312a48 00000002e231713c
+ 00000002e231618c:	00000002e2312a50 00000002e2312aef 00000002e2317140
+ 00000002e2316198:	00000002e2312af0 00000002e2312b71 00000002e231714c
+ 00000002e23161a4:	00000002e2312b80 00000002e2312bab 00000002e2317154
+ 00000002e23161b0:	00000002e2312bb0 00000002e2312c1c 00000002e231715c
+ 00000002e23161bc:	00000002e2312c20 00000002e2312c48 00000002e2317164
+ 00000002e23161c8:	00000002e2312c50 00000002e2312cd5 00000002e231716c
+ 00000002e23161d4:	00000002e2312ce0 00000002e2312d92 00000002e2317174
+ 00000002e23161e0:	00000002e2312da0 00000002e2312da3 00000002e231717c
+ 00000002e23161ec:	00000002e2312df0 00000002e2312df6 00000002e2317180
+ 00000002e23161f8:	00000002e2312e00 00000002e2312e06 00000002e2317184
+ 00000002e2316204:	00000002e2312e10 00000002e2312f4f 00000002e2317188
+ 00000002e2316210:	00000002e2312fc0 00000002e2312fe5 00000002e2317194
+ 00000002e231621c:	00000002e2312ff0 00000002e23130c4 00000002e2317198
+ 00000002e2316228:	00000002e23130d0 00000002e2313141 00000002e23171a8
+ 00000002e2316234:	00000002e2313150 00000002e231316f 00000002e23171b4
+ 00000002e2316240:	00000002e23131e0 00000002e2313221 00000002e23171bc
+ 00000002e231624c:	00000002e2313230 00000002e231323c 00000002e23171c4
+ 00000002e2316258:	00000002e2313250 00000002e2313255 00000002e23171c8
 
 Dump of .xdata
  00000002e2317000 (rva: 00007000): 00000002e2311000 - 00000002e231100c
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
  00000002e2317004 (rva: 00007004): 00000002e2311010 - 00000002e23111ff
 	Version: 1, Flags: none
@@ -269,206 +269,206 @@
 	  pc+0x04: push rbx
 	  pc+0x03: push rsi
 	  pc+0x02: push rdi
 	  pc+0x01: push rbp
  00000002e231707c (rva: 0000707c): 00000002e23118b0 - 00000002e23118b5
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000002e2317080 (rva: 00007080): 00000002e23118c0 - 00000002e2311fa0
+ 00000002e2317080 (rva: 00007080): 00000002e23118c0 - 00000002e2311fdc
 	Version: 1, Flags: none
 	Nbr codes: 11, Prologue size: 0x15, Frame offset: 0x0, Frame reg: none
 	  pc+0x15: save xmm6 at rsp + 0x50
 	  pc+0x10: alloc small area: rsp = rsp - 0x68
 	  pc+0x0c: push rbx
 	  pc+0x0b: push rsi
 	  pc+0x0a: push rdi
 	  pc+0x09: push rbp
 	  pc+0x08: push r12
 	  pc+0x06: push r13
 	  pc+0x04: push r14
 	  pc+0x02: push r15
- 00000002e231709c (rva: 0000709c): 00000002e2311fa0 - 00000002e2311fc9
+ 00000002e231709c (rva: 0000709c): 00000002e2311fe0 - 00000002e2312009
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000002e23170a0 (rva: 000070a0): 00000002e2311fd0 - 00000002e2311ff1
+ 00000002e23170a0 (rva: 000070a0): 00000002e2312010 - 00000002e2312031
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000002e23170a4 (rva: 000070a4): 00000002e2312000 - 00000002e231203a
+ 00000002e23170a4 (rva: 000070a4): 00000002e2312040 - 00000002e231207a
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 00000002e23170ac (rva: 000070ac): 00000002e2312040 - 00000002e23120aa
+ 00000002e23170ac (rva: 000070ac): 00000002e2312080 - 00000002e23120ea
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
 	  pc+0x06: alloc small area: rsp = rsp - 0x28
 	  pc+0x02: push rbx
 	  pc+0x01: push rsi
- 00000002e23170b8 (rva: 000070b8): 00000002e23120b0 - 00000002e23120cf
+ 00000002e23170b8 (rva: 000070b8): 00000002e23120f0 - 00000002e231210f
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000002e23170bc (rva: 000070bc): 00000002e23120d0 - 00000002e23120ff
+ 00000002e23170bc (rva: 000070bc): 00000002e2312110 - 00000002e231213f
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 00000002e23170c4 (rva: 000070c4): 00000002e2312100 - 00000002e2312181
+ 00000002e23170c4 (rva: 000070c4): 00000002e2312140 - 00000002e23121c1
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
 	  pc+0x06: alloc small area: rsp = rsp - 0x28
 	  pc+0x02: push rbx
 	  pc+0x01: push rsi
- 00000002e23170d0 (rva: 000070d0): 00000002e2312190 - 00000002e2312193
+ 00000002e23170d0 (rva: 000070d0): 00000002e23121d0 - 00000002e23121d3
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000002e23170d4 (rva: 000070d4): 00000002e23121a0 - 00000002e231220a
+ 00000002e23170d4 (rva: 000070d4): 00000002e23121e0 - 00000002e231224a
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x07, Frame offset: 0x0, Frame reg: none
 	  pc+0x07: alloc small area: rsp = rsp - 0x38
 	  pc+0x03: push rbx
 	  pc+0x02: push r12
- 00000002e23170e0 (rva: 000070e0): 00000002e2312210 - 00000002e231242d
+ 00000002e23170e0 (rva: 000070e0): 00000002e2312250 - 00000002e231246d
 	Version: 1, Flags: none
 	Nbr codes: 6, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: none
 	  pc+0x0a: alloc small area: rsp = rsp - 0x50
 	  pc+0x06: push rbx
 	  pc+0x05: push rsi
 	  pc+0x04: push rdi
 	  pc+0x03: push rbp
 	  pc+0x02: push r12
- 00000002e23170f0 (rva: 000070f0): 00000002e2312430 - 00000002e2312715
+ 00000002e23170f0 (rva: 000070f0): 00000002e2312470 - 00000002e2312755
 	Version: 1, Flags: none
 	Nbr codes: 10, Prologue size: 0x18, Frame offset: 0x8, Frame reg: rbp
 	  pc+0x18: FPReg: rbp = rsp + 0x80 (info = 0x0)
 	  pc+0x10: alloc small area: rsp = rsp - 0x38
 	  pc+0x0c: push rbx
 	  pc+0x0b: push rsi
 	  pc+0x0a: push rdi
 	  pc+0x09: push r12
 	  pc+0x07: push r13
 	  pc+0x05: push r14
 	  pc+0x03: push r15
 	  pc+0x01: push rbp
- 00000002e2317108 (rva: 00007108): 00000002e2312720 - 00000002e231278b
+ 00000002e2317108 (rva: 00007108): 00000002e2312760 - 00000002e23127cb
 	Version: 1, Flags: none
 	Nbr codes: 5, Prologue size: 0x09, Frame offset: 0x0, Frame reg: none
 	  pc+0x09: alloc small area: rsp = rsp - 0x28
 	  pc+0x05: push rbx
 	  pc+0x04: push rsi
 	  pc+0x03: push rdi
 	  pc+0x02: push r12
- 00000002e2317118 (rva: 00007118): 00000002e2312790 - 00000002e2312808
+ 00000002e2317118 (rva: 00007118): 00000002e23127d0 - 00000002e2312848
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x07, Frame offset: 0x0, Frame reg: none
 	  pc+0x07: alloc small area: rsp = rsp - 0x20
 	  pc+0x03: push rbx
 	  pc+0x02: push rsi
 	  pc+0x01: push rdi
- 00000002e2317124 (rva: 00007124): 00000002e2312810 - 00000002e2312899
+ 00000002e2317124 (rva: 00007124): 00000002e2312850 - 00000002e23128d9
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x05, Frame offset: 0x0, Frame reg: none
 	  pc+0x05: alloc small area: rsp = rsp - 0x20
 	  pc+0x01: push rbx
- 00000002e231712c (rva: 0000712c): 00000002e23128a0 - 00000002e2312980
+ 00000002e231712c (rva: 0000712c): 00000002e23128e0 - 00000002e23129c0
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x05, Frame offset: 0x0, Frame reg: none
 	  pc+0x05: alloc small area: rsp = rsp - 0x20
 	  pc+0x01: push rbx
- 00000002e2317134 (rva: 00007134): 00000002e2312980 - 00000002e231299e
+ 00000002e2317134 (rva: 00007134): 00000002e23129c0 - 00000002e23129de
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000002e2317138 (rva: 00007138): 00000002e23129a0 - 00000002e23129b3
+ 00000002e2317138 (rva: 00007138): 00000002e23129e0 - 00000002e23129f3
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000002e231713c (rva: 0000713c): 00000002e23129c0 - 00000002e2312a08
+ 00000002e231713c (rva: 0000713c): 00000002e2312a00 - 00000002e2312a48
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000002e2317140 (rva: 00007140): 00000002e2312a10 - 00000002e2312aaf
+ 00000002e2317140 (rva: 00007140): 00000002e2312a50 - 00000002e2312aef
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x08, Frame offset: 0x0, Frame reg: none
 	  pc+0x08: alloc small area: rsp = rsp - 0x20
 	  pc+0x04: push rbx
 	  pc+0x03: push rsi
 	  pc+0x02: push r12
- 00000002e231714c (rva: 0000714c): 00000002e2312ab0 - 00000002e2312b31
+ 00000002e231714c (rva: 0000714c): 00000002e2312af0 - 00000002e2312b71
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 00000002e2317154 (rva: 00007154): 00000002e2312b40 - 00000002e2312b6b
+ 00000002e2317154 (rva: 00007154): 00000002e2312b80 - 00000002e2312bab
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 00000002e231715c (rva: 0000715c): 00000002e2312b70 - 00000002e2312bdc
+ 00000002e231715c (rva: 0000715c): 00000002e2312bb0 - 00000002e2312c1c
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 00000002e2317164 (rva: 00007164): 00000002e2312be0 - 00000002e2312c08
+ 00000002e2317164 (rva: 00007164): 00000002e2312c20 - 00000002e2312c48
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 00000002e231716c (rva: 0000716c): 00000002e2312c10 - 00000002e2312c95
+ 00000002e231716c (rva: 0000716c): 00000002e2312c50 - 00000002e2312cd5
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 00000002e2317174 (rva: 00007174): 00000002e2312ca0 - 00000002e2312d52
+ 00000002e2317174 (rva: 00007174): 00000002e2312ce0 - 00000002e2312d92
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 00000002e231717c (rva: 0000717c): 00000002e2312d60 - 00000002e2312d63
+ 00000002e231717c (rva: 0000717c): 00000002e2312da0 - 00000002e2312da3
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000002e2317180 (rva: 00007180): 00000002e2312db0 - 00000002e2312db6
+ 00000002e2317180 (rva: 00007180): 00000002e2312df0 - 00000002e2312df6
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000002e2317184 (rva: 00007184): 00000002e2312dc0 - 00000002e2312dc6
+ 00000002e2317184 (rva: 00007184): 00000002e2312e00 - 00000002e2312e06
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000002e2317188 (rva: 00007188): 00000002e2312dd0 - 00000002e2312f0f
+ 00000002e2317188 (rva: 00007188): 00000002e2312e10 - 00000002e2312f4f
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: none
 	  pc+0x0a: save xmm6 at rsp + 0x40
 	  pc+0x05: alloc small area: rsp = rsp - 0x50
 	  pc+0x01: push rbx
- 00000002e2317194 (rva: 00007194): 00000002e2312f80 - 00000002e2312fa5
+ 00000002e2317194 (rva: 00007194): 00000002e2312fc0 - 00000002e2312fe5
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000002e2317198 (rva: 00007198): 00000002e2312fb0 - 00000002e2313084
+ 00000002e2317198 (rva: 00007198): 00000002e2312ff0 - 00000002e23130c4
 	Version: 1, Flags: none
 	Nbr codes: 5, Prologue size: 0x08, Frame offset: 0x0, Frame reg: none
 	  pc+0x08: alloc small area: rsp = rsp - 0x28
 	  pc+0x04: push rbx
 	  pc+0x03: push rsi
 	  pc+0x02: push rdi
 	  pc+0x01: push rbp
- 00000002e23171a8 (rva: 000071a8): 00000002e2313090 - 00000002e2313101
+ 00000002e23171a8 (rva: 000071a8): 00000002e23130d0 - 00000002e2313141
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x08, Frame offset: 0x0, Frame reg: none
 	  pc+0x08: alloc small area: rsp = rsp - 0x20
 	  pc+0x04: push rbx
 	  pc+0x03: push rsi
 	  pc+0x02: push r12
- 00000002e23171b4 (rva: 000071b4): 00000002e2313110 - 00000002e231312f
+ 00000002e23171b4 (rva: 000071b4): 00000002e2313150 - 00000002e231316f
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x05, Frame offset: 0x0, Frame reg: none
 	  pc+0x05: alloc small area: rsp = rsp - 0x20
 	  pc+0x01: push rbx
- 00000002e23171bc (rva: 000071bc): 00000002e23131a0 - 00000002e23131e1
+ 00000002e23171bc (rva: 000071bc): 00000002e23131e0 - 00000002e2313221
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x58
- 00000002e23171c4 (rva: 000071c4): 00000002e23131f0 - 00000002e23131fc
+ 00000002e23171c4 (rva: 000071c4): 00000002e2313230 - 00000002e231323c
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000002e23171c8 (rva: 000071c8): 00000002e2313210 - 00000002e2313215
+ 00000002e23171c8 (rva: 000071c8): 00000002e2313250 - 00000002e2313255
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
 
 
 PE File Base Relocations (interpreted .reloc section contents)
 
 Virtual Address: 00003000 Chunk size 12 (0xc) Number of fixups 2
-	reloc    0 offset  228 [3228] DIR64
+	reloc    0 offset  268 [3268] DIR64
 	reloc    1 offset    0 [3000] ABSOLUTE
 
 Virtual Address: 00004000 Chunk size 20 (0x14) Number of fixups 6
 	reloc    0 offset   10 [4010] DIR64
 	reloc    1 offset   40 [4040] DIR64
 	reloc    2 offset   48 [4048] DIR64
 	reloc    3 offset   50 [4050] DIR64
@@ -501,15 +501,15 @@
 	reloc    0 offset   18 [b018] DIR64
 	reloc    1 offset   30 [b030] DIR64
 	reloc    2 offset   38 [b038] DIR64
 	reloc    3 offset    0 [b000] ABSOLUTE
 
 Sections:
 Idx Name          Size      VMA               LMA               File off  Algn
-  0 .text         00002248  00000002e2311000  00000002e2311000  00000400  2**4
+  0 .text         00002288  00000002e2311000  00000002e2311000  00000400  2**4
                   CONTENTS, ALLOC, LOAD, READONLY, CODE, DATA
   1 .data         00000070  00000002e2314000  00000002e2314000  00002800  2**4
                   CONTENTS, ALLOC, LOAD, DATA
   2 .rdata        00000560  00000002e2315000  00000002e2315000  00002a00  2**4
                   CONTENTS, ALLOC, LOAD, READONLY, DATA
   3 .pdata        00000264  00000002e2316000  00000002e2316000  00003000  2**2
                   CONTENTS, ALLOC, LOAD, READONLY, DATA
@@ -532,15 +532,15 @@
 
 
 
 Disassembly of section .text:
 
 00000002e2311000 <.text>:
    2e2311000:	lea    0x6ff9(%rip),%rcx        # 0x2e2318000
-   2e2311007:	jmp    0x2e2312f80
+   2e2311007:	jmp    0x2e2312fc0
    2e231100c:	nopl   0x0(%rax)
    2e2311010:	push   %r13
    2e2311012:	push   %r12
    2e2311014:	push   %rbp
    2e2311015:	push   %rdi
    2e2311016:	push   %rsi
    2e2311017:	push   %rbx
@@ -569,15 +569,15 @@
    2e231106a:	test   %rax,%rax
    2e231106d:	jne    0x2e2311058
    2e231106f:	mov    0x41ca(%rip),%rdi        # 0x2e2315240
    2e2311076:	mov    (%rdi),%eax
    2e2311078:	cmp    $0x2,%eax
    2e231107b:	je     0x2e2311170
    2e2311081:	mov    $0x1f,%ecx
-   2e2311086:	call   0x2e2312f70
+   2e2311086:	call   0x2e2312fb0
    2e231108b:	mov    $0x1,%eax
    2e2311090:	add    $0x28,%rsp
    2e2311094:	pop    %rbx
    2e2311095:	pop    %rsi
    2e2311096:	pop    %rdi
    2e2311097:	pop    %rbp
    2e2311098:	pop    %r12
@@ -640,15 +640,15 @@
    2e2311163:	pop    %rdi
    2e2311164:	pop    %rbp
    2e2311165:	pop    %r12
    2e2311167:	pop    %r13
    2e2311169:	ret
    2e231116a:	nopw   0x0(%rax,%rax,1)
    2e2311170:	lea    0x6e89(%rip),%rcx        # 0x2e2318000
-   2e2311177:	call   0x2e2313090
+   2e2311177:	call   0x2e23130d0
    2e231117c:	movl   $0x0,(%rdi)
    2e2311182:	xchg   %rsi,(%rbx)
    2e2311185:	mov    $0x1,%eax
    2e231118a:	jmp    0x2e2311090
    2e231118f:	nop
    2e2311190:	mov    $0x1,%edi
    2e2311195:	jmp    0x2e23110ef
@@ -656,25 +656,25 @@
    2e23111a0:	xor    %eax,%eax
    2e23111a2:	xchg   %rax,(%rbx)
    2e23111a5:	jmp    0x2e231111e
    2e23111aa:	nopw   0x0(%rax,%rax,1)
    2e23111b0:	mov    0x40c9(%rip),%rdx        # 0x2e2315280
    2e23111b7:	mov    0x40b2(%rip),%rcx        # 0x2e2315270
    2e23111be:	movl   $0x1,(%rsi)
-   2e23111c4:	call   0x2e2312f60
+   2e23111c4:	call   0x2e2312fa0
    2e23111c9:	jmp    0x2e231110b
    2e23111ce:	xchg   %ax,%ax
    2e23111d0:	mov    0x4089(%rip),%rdx        # 0x2e2315260
    2e23111d7:	mov    0x4072(%rip),%rcx        # 0x2e2315250
-   2e23111de:	call   0x2e2312f60
+   2e23111de:	call   0x2e2312fa0
    2e23111e3:	movl   $0x2,(%rsi)
    2e23111e9:	jmp    0x2e2311116
    2e23111ee:	xchg   %ax,%ax
    2e23111f0:	mov    $0x1f,%ecx
-   2e23111f5:	call   0x2e2312f70
+   2e23111f5:	call   0x2e2312fb0
    2e23111fa:	jmp    0x2e231110b
    2e23111ff:	nop
    2e2311200:	push   %r14
    2e2311202:	push   %r13
    2e2311204:	push   %r12
    2e2311206:	push   %rsi
    2e2311207:	push   %rbx
@@ -685,23 +685,23 @@
    2e2311218:	mov    %edx,%r12d
    2e231121b:	mov    %r8,%rbx
    2e231121e:	test   %edx,%edx
    2e2311220:	jne    0x2e2311280
    2e2311222:	mov    0x6df0(%rip),%eax        # 0x2e2318018
    2e2311228:	test   %eax,%eax
    2e231122a:	je     0x2e2311261
-   2e231122c:	call   0x2e2312430
+   2e231122c:	call   0x2e2312470
    2e2311231:	mov    %rbx,%r8
    2e2311234:	xor    %edx,%edx
    2e2311236:	mov    %r13,%rcx
-   2e2311239:	call   0x2e2312dc0
+   2e2311239:	call   0x2e2312e00
    2e231123e:	mov    %rbx,%r8
    2e2311241:	mov    %r12d,%edx
    2e2311244:	mov    %r13,%rcx
-   2e2311247:	call   0x2e2312db0
+   2e2311247:	call   0x2e2312df0
    2e231124c:	mov    %rbx,%r8
    2e231124f:	mov    %r12d,%edx
    2e2311252:	mov    %r13,%rcx
    2e2311255:	mov    %eax,%r14d
    2e2311258:	call   0x2e2311010
    2e231125d:	test   %eax,%eax
    2e231125f:	jne    0x2e2311264
@@ -712,80 +712,80 @@
    2e2311271:	pop    %rbx
    2e2311272:	pop    %rsi
    2e2311273:	pop    %r12
    2e2311275:	pop    %r13
    2e2311277:	pop    %r14
    2e2311279:	ret
    2e231127a:	nopw   0x0(%rax,%rax,1)
-   2e2311280:	call   0x2e2312430
+   2e2311280:	call   0x2e2312470
    2e2311285:	lea    -0x1(%r12),%eax
    2e231128a:	mov    %rbx,%r8
    2e231128d:	mov    %r12d,%edx
    2e2311290:	mov    %r13,%rcx
    2e2311293:	cmp    $0x1,%eax
    2e2311296:	ja     0x2e2311308
    2e2311298:	call   0x2e2311010
    2e231129d:	test   %eax,%eax
    2e231129f:	je     0x2e2311261
    2e23112a1:	mov    %rbx,%r8
    2e23112a4:	mov    %r12d,%edx
    2e23112a7:	mov    %r13,%rcx
-   2e23112aa:	call   0x2e2312db0
+   2e23112aa:	call   0x2e2312df0
    2e23112af:	mov    %eax,%r14d
    2e23112b2:	test   %eax,%eax
    2e23112b4:	je     0x2e2311320
    2e23112b6:	cmp    $0x1,%r12d
    2e23112ba:	jne    0x2e231132c
-   2e23112bc:	call   0x2e23120b0
+   2e23112bc:	call   0x2e23120f0
    2e23112c1:	mov    %rbx,%r8
    2e23112c4:	mov    $0x1,%edx
    2e23112c9:	mov    %r13,%rcx
-   2e23112cc:	call   0x2e2312dc0
+   2e23112cc:	call   0x2e2312e00
    2e23112d1:	mov    %eax,%r14d
    2e23112d4:	test   %eax,%eax
    2e23112d6:	jne    0x2e2311264
    2e23112d8:	mov    %rbx,%r8
    2e23112db:	xor    %edx,%edx
    2e23112dd:	mov    %r13,%rcx
-   2e23112e0:	call   0x2e2312dc0
+   2e23112e0:	call   0x2e2312e00
    2e23112e5:	mov    %rbx,%r8
    2e23112e8:	xor    %edx,%edx
    2e23112ea:	mov    %r13,%rcx
-   2e23112ed:	call   0x2e2312db0
+   2e23112ed:	call   0x2e2312df0
    2e23112f2:	mov    %rbx,%r8
    2e23112f5:	xor    %edx,%edx
    2e23112f7:	mov    %r13,%rcx
    2e23112fa:	call   0x2e2311010
    2e23112ff:	jmp    0x2e2311264
    2e2311304:	nopl   0x0(%rax)
-   2e2311308:	call   0x2e2312dc0
+   2e2311308:	call   0x2e2312e00
    2e231130d:	mov    %eax,%r14d
    2e2311310:	cmp    $0x3,%r12d
    2e2311314:	jne    0x2e2311264
    2e231131a:	jmp    0x2e231123e
    2e231131f:	nop
    2e2311320:	cmp    $0x1,%r12d
    2e2311324:	jne    0x2e2311261
    2e231132a:	jmp    0x2e23112f2
    2e231132c:	mov    %rbx,%r8
    2e231132f:	mov    $0x2,%edx
    2e2311334:	mov    %r13,%rcx
-   2e2311337:	call   0x2e2312dc0
+   2e2311337:	call   0x2e2312e00
    2e231133c:	mov    %eax,%r14d
    2e231133f:	jmp    0x2e2311264
    2e2311344:	data16 cs nopw 0x0(%rax,%rax,1)
    2e231134f:	nop
    2e2311350:	mov    0x3f39(%rip),%rax        # 0x2e2315290
    2e2311357:	movl   $0x0,(%rax)
    2e231135d:	jmp    0x2e2311200
    2e2311362:	data16 cs nopw 0x0(%rax,%rax,1)
    2e231136d:	nopl   (%rax)
    2e2311370:	mov    %rcx,%rdx
    2e2311373:	lea    0x6c86(%rip),%rcx        # 0x2e2318000
-   2e231137a:	jmp    0x2e2312fb0
+   2e231137a:	jmp    0x2e2312ff0
    2e231137f:	nop
    2e2311380:	lea    0x9(%rip),%rcx        # 0x2e2311390
    2e2311387:	jmp    0x2e2311370
    2e231138c:	nopl   0x0(%rax)
    2e2311390:	ret
    2e2311391:	nop
    2e2311392:	nop
@@ -888,27 +888,27 @@
    2e23114d2:	movupd %xmm2,%xmm0
    2e23114d6:	ret
    2e23114d7:	nopw   0x0(%rax,%rax,1)
    2e23114e0:	pxor   %xmm3,%xmm3
    2e23114e4:	movupd %xmm3,%xmm2
    2e23114e8:	jmp    0x2e23114bc
    2e23114ea:	movupd %xmm2,%xmm0
-   2e23114ee:	jmp    0x2e2312dd0
+   2e23114ee:	jmp    0x2e2312e10
    2e23114f3:	data16 cs nopw 0x0(%rax,%rax,1)
    2e23114fe:	xchg   %ax,%ax
    2e2311500:	push   %rbp
    2e2311501:	push   %rdi
    2e2311502:	push   %rsi
    2e2311503:	push   %rbx
    2e2311504:	sub    $0x28,%rsp
    2e2311508:	movslq %r8d,%rsi
    2e231150b:	mov    %rcx,%rbx
    2e231150e:	mov    %rdx,%rdi
    2e2311511:	lea    0x0(,%rsi,4),%rcx
-   2e2311519:	call   0x2e2312f38
+   2e2311519:	call   0x2e2312f78
    2e231151e:	mov    %rax,%r9
    2e2311521:	test   %esi,%esi
    2e2311523:	jle    0x2e231155c
    2e2311525:	xor    %eax,%eax
    2e2311527:	nopw   0x0(%rax,%rax,1)
    2e2311530:	movsd  (%rbx,%rax,8),%xmm0
    2e2311535:	ucomisd %xmm0,%xmm0
@@ -950,15 +950,15 @@
    2e23115ab:	movups %xmm9,0x60(%rsp)
    2e23115b1:	movups %xmm10,0x70(%rsp)
    2e23115b7:	movslq %r8d,%rdi
    2e23115ba:	mov    %rcx,%rbx
    2e23115bd:	mov    %rdx,%rsi
    2e23115c0:	lea    0x0(,%rdi,4),%rcx
    2e23115c8:	mov    %rdi,%rbp
-   2e23115cb:	call   0x2e2312f38
+   2e23115cb:	call   0x2e2312f78
    2e23115d0:	mov    %rax,%rcx
    2e23115d3:	test   %edi,%edi
    2e23115d5:	jle    0x2e2311830
    2e23115db:	lea    -0x1(%rdi),%r8d
    2e23115df:	mov    %edi,%edx
    2e23115e1:	xor    %eax,%eax
    2e23115e3:	nopl   0x0(%rax,%rax,1)
@@ -1101,15 +1101,15 @@
    2e23117d5:	cmp    %rdi,%rax
    2e23117d8:	jne    0x2e23117b9
    2e23117da:	divsd  %xmm9,%xmm1
    2e23117df:	ucomisd %xmm1,%xmm8
    2e23117e4:	ja     0x2e231186c
    2e23117ea:	movupd %xmm1,%xmm6
    2e23117ee:	sqrtsd %xmm6,%xmm6
-   2e23117f2:	call   0x2e2312f48
+   2e23117f2:	call   0x2e2312f88
    2e23117f7:	mulsd  %xmm10,%xmm6
    2e23117fc:	movups 0x50(%rsp),%xmm8
    2e2311802:	movups 0x60(%rsp),%xmm9
    2e2311808:	movups 0x70(%rsp),%xmm10
    2e231180e:	divsd  %xmm6,%xmm7
    2e2311812:	movups 0x30(%rsp),%xmm6
    2e2311817:	movupd %xmm7,%xmm0
@@ -1132,26 +1132,26 @@
    2e2311858:	movupd %xmm8,%xmm1
    2e231185d:	jmp    0x2e23117da
    2e2311862:	xor    %eax,%eax
    2e2311864:	xor    %r8d,%r8d
    2e2311867:	jmp    0x2e231167b
    2e231186c:	movupd %xmm1,%xmm0
    2e2311870:	mov    %rcx,0x28(%rsp)
-   2e2311875:	call   0x2e2312dd0
+   2e2311875:	call   0x2e2312e10
    2e231187a:	mov    0x28(%rsp),%rcx
    2e231187f:	movupd %xmm0,%xmm6
    2e2311883:	jmp    0x2e23117f2
    2e2311888:	movupd %xmm10,%xmm0
    2e231188d:	mov    %rcx,0x28(%rsp)
-   2e2311892:	call   0x2e2312dd0
+   2e2311892:	call   0x2e2312e10
    2e2311897:	mov    0x28(%rsp),%rcx
    2e231189c:	movupd %xmm0,%xmm10
    2e23118a1:	jmp    0x2e231179a
    2e23118a6:	cs nopw 0x0(%rax,%rax,1)
-   2e23118b0:	jmp    0x2e2312f48
+   2e23118b0:	jmp    0x2e2312f88
    2e23118b5:	data16 cs nopw 0x0(%rax,%rax,1)
    2e23118c0:	push   %r15
    2e23118c2:	push   %r14
    2e23118c4:	push   %r13
    2e23118c6:	push   %r12
    2e23118c8:	push   %rbp
    2e23118c9:	push   %rdi
@@ -1163,139 +1163,139 @@
    2e23118d8:	mov    %rcx,%rsi
    2e23118db:	mov    %rdx,%rbx
    2e23118de:	mov    %r9d,%ebp
    2e23118e1:	mov    %rdi,%r12
    2e23118e4:	mov    %r8d,0xc0(%rsp)
    2e23118ec:	shl    $0x4,%r12
    2e23118f0:	mov    %r12,%rcx
-   2e23118f3:	call   0x2e2312f38
+   2e23118f3:	call   0x2e2312f78
    2e23118f8:	mov    %r12,%rcx
    2e23118fb:	mov    %rax,%r14
-   2e23118fe:	call   0x2e2312f38
+   2e23118fe:	call   0x2e2312f78
    2e2311903:	lea    0x0(,%rdi,4),%rcx
    2e231190b:	mov    %rax,%r13
-   2e231190e:	call   0x2e2312f38
+   2e231190e:	call   0x2e2312f78
    2e2311913:	lea    0x0(,%rdi,8),%r8
    2e231191b:	mov    %r8,%rcx
-   2e231191e:	mov    %r8,0x30(%rsp)
+   2e231191e:	mov    %r8,0x28(%rsp)
    2e2311923:	mov    %rax,%r12
-   2e2311926:	call   0x2e2312f38
-   2e231192b:	mov    0x30(%rsp),%r8
-   2e2311930:	mov    %rax,0x28(%rsp)
+   2e2311926:	call   0x2e2312f78
+   2e231192b:	mov    0x28(%rsp),%r8
+   2e2311930:	mov    %rax,0x20(%rsp)
    2e2311935:	mov    %r8,%rcx
-   2e2311938:	call   0x2e2312f38
+   2e2311938:	call   0x2e2312f78
    2e231193d:	mov    0xc0(%rsp),%r8d
    2e2311945:	mov    %rax,%r15
    2e2311948:	test   %r8d,%r8d
-   2e231194b:	jle    0x2e2311f46
-   2e2311951:	mov    0x30(%rsp),%r8
-   2e2311956:	mov    0x28(%rsp),%rcx
+   2e231194b:	jle    0x2e2311f6a
+   2e2311951:	mov    0x28(%rsp),%r8
+   2e2311956:	mov    0x20(%rsp),%rcx
    2e231195b:	mov    %rsi,%rdx
-   2e231195e:	call   0x2e2312f30
-   2e2311963:	mov    0x30(%rsp),%r8
+   2e231195e:	call   0x2e2312f70
+   2e2311963:	mov    0x28(%rsp),%r8
    2e2311968:	mov    %r15,%rcx
    2e231196b:	mov    %rbx,%rdx
-   2e231196e:	call   0x2e2312f30
-   2e2311973:	mov    %r12,0x30(%rsp)
+   2e231196e:	call   0x2e2312f70
+   2e2311973:	mov    %r12,0x28(%rsp)
    2e2311978:	xor    %eax,%eax
    2e231197a:	xor    %r10d,%r10d
    2e231197d:	movsd  0x367b(%rip),%xmm1        # 0x2e2315000
    2e2311985:	mov    0xc0(%rsp),%r12d
    2e231198d:	mov    $0xffffffff,%r9d
    2e2311993:	xor    %ecx,%ecx
    2e2311995:	mov    $0xffffffff,%r8d
    2e231199b:	nopl   0x0(%rax,%rax,1)
    2e23119a0:	movsd  (%rsi,%rax,8),%xmm0
    2e23119a5:	mov    %eax,%r11d
    2e23119a8:	ucomisd %xmm0,%xmm0
-   2e23119ac:	jp     0x2e2311bbe
+   2e23119ac:	jp     0x2e2311bce
    2e23119b2:	movslq %ecx,%rdx
    2e23119b5:	add    $0x1,%ecx
    2e23119b8:	shl    $0x4,%rdx
    2e23119bc:	add    %r14,%rdx
    2e23119bf:	mov    %eax,0x8(%rdx)
    2e23119c2:	movq   %xmm0,(%rdx)
    2e23119c6:	movsd  (%rbx,%rax,8),%xmm0
    2e23119cb:	ucomisd %xmm0,%xmm0
-   2e23119cf:	jp     0x2e2311b9f
+   2e23119cf:	jp     0x2e2311baf
    2e23119d5:	movslq %r10d,%rdx
    2e23119d8:	add    $0x1,%r10d
    2e23119dc:	shl    $0x4,%rdx
    2e23119e0:	add    %r13,%rdx
    2e23119e3:	mov    %r11d,0x8(%rdx)
    2e23119e7:	movq   %xmm0,(%rdx)
    2e23119eb:	add    $0x1,%rax
    2e23119ef:	cmp    %rax,%rdi
    2e23119f2:	jne    0x2e23119a0
    2e23119f4:	mov    %r10d,%edi
    2e23119f7:	movslq %ecx,%rdx
-   2e23119fa:	mov    0x30(%rsp),%r12
+   2e23119fa:	mov    0x28(%rsp),%r12
    2e23119ff:	lea    -0x666(%rip),%r9        # 0x2e23113a0
-   2e2311a06:	mov    %ecx,0x30(%rsp)
+   2e2311a06:	mov    %ecx,0x28(%rsp)
    2e2311a0a:	mov    $0x10,%r8d
    2e2311a10:	mov    %r14,%rcx
-   2e2311a13:	call   0x2e2312f28
+   2e2311a13:	call   0x2e2312f68
    2e2311a18:	movslq %edi,%rdx
    2e2311a1b:	lea    -0x682(%rip),%r9        # 0x2e23113a0
    2e2311a22:	mov    %r13,%rcx
    2e2311a25:	mov    $0x10,%r8d
-   2e2311a2b:	call   0x2e2312f28
-   2e2311a30:	mov    0x30(%rsp),%ecx
-   2e2311a34:	mov    %edi,0x3c(%rsp)
-   2e2311a38:	cmp    %edi,%ecx
-   2e2311a3a:	cmovle %ecx,%edi
+   2e2311a2b:	call   0x2e2312f68
+   2e2311a30:	mov    0x28(%rsp),%eax
+   2e2311a34:	mov    %edi,0x40(%rsp)
+   2e2311a38:	cmp    %edi,%eax
+   2e2311a3a:	cmovle %eax,%edi
    2e2311a3d:	movslq %edi,%rcx
    2e2311a40:	shl    $0x2,%rcx
-   2e2311a44:	mov    %rcx,0x40(%rsp)
-   2e2311a49:	call   0x2e2312f38
-   2e2311a4e:	mov    0x40(%rsp),%rcx
-   2e2311a53:	mov    %rax,0x48(%rsp)
-   2e2311a58:	call   0x2e2312f38
-   2e2311a5d:	mov    %rax,%r9
-   2e2311a60:	test   %ebp,%ebp
-   2e2311a62:	jne    0x2e2311be0
-   2e2311a68:	mov    0x3c(%rsp),%ecx
-   2e2311a6c:	test   %edi,%edi
-   2e2311a6e:	mov    0x48(%rsp),%r11
-   2e2311a73:	setg   %al
-   2e2311a76:	test   %ecx,%ecx
-   2e2311a78:	mov    0x30(%rsp),%ecx
-   2e2311a7c:	setg   %r10b
-   2e2311a80:	and    %eax,%r10d
-   2e2311a83:	test   %ecx,%ecx
-   2e2311a85:	jle    0x2e2311f99
-   2e2311a8b:	test   %al,%al
-   2e2311a8d:	je     0x2e2311f99
-   2e2311a93:	lea    -0x1(%rcx),%eax
-   2e2311a96:	xor    %edx,%edx
-   2e2311a98:	cltq
-   2e2311a9a:	nopw   0x0(%rax,%rax,1)
+   2e2311a44:	mov    %rcx,0x30(%rsp)
+   2e2311a49:	call   0x2e2312f78
+   2e2311a4e:	mov    0x30(%rsp),%rcx
+   2e2311a53:	mov    %rax,0x38(%rsp)
+   2e2311a58:	call   0x2e2312f78
+   2e2311a5d:	mov    %rax,0x30(%rsp)
+   2e2311a62:	test   %ebp,%ebp
+   2e2311a64:	jne    0x2e2311bf0
+   2e2311a6a:	mov    0x40(%rsp),%ecx
+   2e2311a6e:	test   %edi,%edi
+   2e2311a70:	setg   %al
+   2e2311a73:	test   %ecx,%ecx
+   2e2311a75:	mov    0x28(%rsp),%ecx
+   2e2311a79:	setg   %r9b
+   2e2311a7d:	and    %eax,%r9d
+   2e2311a80:	test   %ecx,%ecx
+   2e2311a82:	jle    0x2e2311fd5
+   2e2311a88:	test   %al,%al
+   2e2311a8a:	je     0x2e2311fd5
+   2e2311a90:	lea    -0x1(%rcx),%eax
+   2e2311a93:	mov    0x38(%rsp),%r10
+   2e2311a98:	xor    %edx,%edx
+   2e2311a9a:	cltq
+   2e2311a9c:	nopl   0x0(%rax)
    2e2311aa0:	mov    %rax,%rcx
    2e2311aa3:	shl    $0x4,%rcx
    2e2311aa7:	movslq 0x8(%r14,%rcx,1),%r8
    2e2311aac:	movsd  (%rbx,%r8,8),%xmm0
    2e2311ab2:	mov    %r8,%rcx
    2e2311ab5:	ucomisd %xmm0,%xmm0
    2e2311ab9:	jnp    0x2e2311ac5
    2e2311abb:	movslq %edx,%r8
    2e2311abe:	add    $0x1,%edx
-   2e2311ac1:	mov    %ecx,(%r11,%r8,4)
+   2e2311ac1:	mov    %ecx,(%r10,%r8,4)
    2e2311ac5:	test   %eax,%eax
    2e2311ac7:	setg   %r8b
    2e2311acb:	cmp    %edi,%edx
    2e2311acd:	setl   %cl
    2e2311ad0:	sub    $0x1,%rax
    2e2311ad4:	test   %cl,%r8b
    2e2311ad7:	jne    0x2e2311aa0
-   2e2311ad9:	mov    0x3c(%rsp),%eax
+   2e2311ad9:	mov    0x40(%rsp),%eax
    2e2311add:	sub    $0x1,%eax
    2e2311ae0:	cltq
-   2e2311ae2:	test   %r10b,%r10b
-   2e2311ae5:	je     0x2e2311f86
-   2e2311aeb:	nopl   0x0(%rax,%rax,1)
+   2e2311ae2:	test   %r9b,%r9b
+   2e2311ae5:	je     0x2e2311fc2
+   2e2311aeb:	mov    0x30(%rsp),%r9
    2e2311af0:	mov    %rax,%rcx
    2e2311af3:	shl    $0x4,%rcx
    2e2311af7:	movslq 0x8(%r13,%rcx,1),%r8
    2e2311afc:	movsd  (%rsi,%r8,8),%xmm0
    2e2311b02:	mov    %r8,%rcx
    2e2311b05:	ucomisd %xmm0,%xmm0
    2e2311b09:	jnp    0x2e2311b15
@@ -1306,1757 +1306,1770 @@
    2e2311b17:	setg   %r8b
    2e2311b1b:	cmp    %edi,%ebp
    2e2311b1d:	setl   %cl
    2e2311b20:	sub    $0x1,%rax
    2e2311b24:	test   %cl,%r8b
    2e2311b27:	jne    0x2e2311af0
    2e2311b29:	test   %ebp,%ebp
-   2e2311b2b:	je     0x2e2311f86
-   2e2311b31:	mov    0x28(%rsp),%rdi
-   2e2311b36:	movslq %ebp,%rax
-   2e2311b39:	lea    0x1(%rbp),%r10d
-   2e2311b3d:	nopl   (%rax)
-   2e2311b40:	mov    %r10d,%r8d
-   2e2311b43:	pxor   %xmm0,%xmm0
-   2e2311b47:	movslq -0x4(%r9,%rax,4),%rcx
-   2e2311b4c:	sub    %eax,%r8d
-   2e2311b4f:	sub    $0x1,%rax
-   2e2311b53:	cvtsi2sd %r8d,%xmm0
-   2e2311b58:	movsd  %xmm0,(%rdi,%rcx,8)
-   2e2311b5d:	test   %eax,%eax
-   2e2311b5f:	jne    0x2e2311b40
-   2e2311b61:	mov    %r10d,%r9d
-   2e2311b64:	test   %edx,%edx
-   2e2311b66:	je     0x2e2311f79
-   2e2311b6c:	movslq %edx,%rax
-   2e2311b6f:	lea    0x1(%rdx),%r8d
-   2e2311b73:	nopl   0x0(%rax,%rax,1)
-   2e2311b78:	mov    %r8d,%ecx
-   2e2311b7b:	pxor   %xmm0,%xmm0
-   2e2311b7f:	movslq -0x4(%r11,%rax,4),%rdx
-   2e2311b84:	sub    %eax,%ecx
-   2e2311b86:	sub    $0x1,%rax
-   2e2311b8a:	cvtsi2sd %ecx,%xmm0
-   2e2311b8e:	movsd  %xmm0,(%r15,%rdx,8)
-   2e2311b94:	test   %eax,%eax
-   2e2311b96:	jne    0x2e2311b78
-   2e2311b98:	mov    %r8d,0x40(%rsp)
-   2e2311b9d:	jmp    0x2e2311bee
-   2e2311b9f:	lea    (%r12,%r8,1),%edx
-   2e2311ba3:	sub    $0x1,%r8d
-   2e2311ba7:	movslq %edx,%rdx
-   2e2311baa:	shl    $0x4,%rdx
-   2e2311bae:	add    %r13,%rdx
-   2e2311bb1:	mov    %r11d,0x8(%rdx)
-   2e2311bb5:	movsd  %xmm1,(%rdx)
-   2e2311bb9:	jmp    0x2e23119eb
-   2e2311bbe:	lea    (%r12,%r9,1),%edx
-   2e2311bc2:	sub    $0x1,%r9d
-   2e2311bc6:	movslq %edx,%rdx
-   2e2311bc9:	shl    $0x4,%rdx
-   2e2311bcd:	add    %r14,%rdx
-   2e2311bd0:	mov    %eax,0x8(%rdx)
-   2e2311bd3:	movsd  %xmm1,(%rdx)
-   2e2311bd7:	jmp    0x2e23119c6
-   2e2311bdc:	nopl   0x0(%rax)
-   2e2311be0:	movl   $0x1,0x40(%rsp)
-   2e2311be8:	mov    $0x1,%r9d
-   2e2311bee:	mov    0xc0(%rsp),%eax
-   2e2311bf5:	mov    0x28(%rsp),%r8
-   2e2311bfa:	lea    -0x1(%rax),%ecx
-   2e2311bfd:	xor    %eax,%eax
-   2e2311bff:	jmp    0x2e2311c0b
-   2e2311c01:	nopl   0x0(%rax)
-   2e2311c08:	mov    %rdx,%rax
-   2e2311c0b:	movsd  (%r15,%rax,8),%xmm0
-   2e2311c11:	ucomisd %xmm0,%xmm0
-   2e2311c15:	jp     0x2e2311f14
-   2e2311c1b:	movsd  (%r8,%rax,8),%xmm0
-   2e2311c21:	xor    %edx,%edx
-   2e2311c23:	ucomisd %xmm0,%xmm0
-   2e2311c27:	setp   %dl
-   2e2311c2a:	mov    %edx,(%r12,%rax,4)
-   2e2311c2e:	lea    0x1(%rax),%rdx
-   2e2311c32:	cmp    %rax,%rcx
-   2e2311c35:	jne    0x2e2311c08
-   2e2311c37:	mov    0x30(%rsp),%edx
-   2e2311c3b:	movsd  0x33c5(%rip),%xmm2        # 0x2e2315008
-   2e2311c43:	xor    %edi,%edi
-   2e2311c45:	test   %edx,%edx
-   2e2311c47:	je     0x2e2311d84
-   2e2311c4d:	mov    %r13,0x48(%rsp)
-   2e2311c52:	mov    0x28(%rsp),%rbp
-   2e2311c57:	mov    0x30(%rsp),%r13d
-   2e2311c5c:	mov    %rbx,0xb8(%rsp)
-   2e2311c64:	mov    %r15,0x30(%rsp)
-   2e2311c69:	mov    %r9d,%r15d
-   2e2311c6c:	jmp    0x2e2311c7c
-   2e2311c6e:	xchg   %ax,%ax
-   2e2311c70:	add    $0x1,%edi
-   2e2311c73:	cmp    %r13d,%edi
-   2e2311c76:	jge    0x2e2311d72
-   2e2311c7c:	movslq %edi,%rax
-   2e2311c7f:	shl    $0x4,%rax
-   2e2311c83:	add    %r14,%rax
-   2e2311c86:	movslq 0x8(%rax),%rdx
-   2e2311c8a:	mov    (%r12,%rdx,4),%r10d
-   2e2311c8e:	test   %r10d,%r10d
-   2e2311c91:	jne    0x2e2311c70
-   2e2311c93:	movsd  (%rsi,%rdx,8),%xmm0
-   2e2311c98:	mov    %r13d,%edx
-   2e2311c9b:	sub    %edi,%edx
-   2e2311c9d:	test   %edx,%edx
-   2e2311c9f:	jle    0x2e2311f2e
-   2e2311ca5:	lea    -0x1(%rdi,%rdx,1),%ebx
-   2e2311ca9:	mov    %edi,%r11d
-   2e2311cac:	mov    %edi,%edx
-   2e2311cae:	mov    %rax,%rcx
-   2e2311cb1:	xor    %r8d,%r8d
-   2e2311cb4:	xor    %r9d,%r9d
-   2e2311cb7:	jmp    0x2e2311ccb
-   2e2311cb9:	nopl   0x0(%rax)
-   2e2311cc0:	movslq 0x8(%rcx),%r8
-   2e2311cc4:	add    $0x1,%edx
-   2e2311cc7:	mov    (%r12,%r8,4),%r8d
-   2e2311ccb:	test   %r8d,%r8d
-   2e2311cce:	jne    0x2e2311cf0
-   2e2311cd0:	movslq %edx,%r8
-   2e2311cd3:	shl    $0x4,%r8
-   2e2311cd7:	movslq 0x8(%r14,%r8,1),%r8
-   2e2311cdc:	ucomisd (%rsi,%r8,8),%xmm0
-   2e2311ce2:	jp     0x2e2311cf8
-   2e2311ce4:	comisd (%rsi,%r8,8),%xmm0
-   2e2311cea:	jne    0x2e2311cf8
-   2e2311cec:	add    $0x1,%r9d
-   2e2311cf0:	add    $0x10,%rcx
-   2e2311cf4:	cmp    %edx,%ebx
-   2e2311cf6:	jne    0x2e2311cc0
-   2e2311cf8:	lea    -0x1(%r9),%ecx
-   2e2311cfc:	pxor   %xmm0,%xmm0
-   2e2311d00:	pxor   %xmm1,%xmm1
-   2e2311d04:	cvtsi2sd %ecx,%xmm0
-   2e2311d08:	cvtsi2sd %r15d,%xmm1
-   2e2311d0d:	add    %r9d,%r15d
-   2e2311d10:	mulsd  %xmm2,%xmm0
-   2e2311d14:	addsd  %xmm1,%xmm0
-   2e2311d18:	test   %r9d,%r9d
-   2e2311d1b:	je     0x2e2311d64
-   2e2311d1d:	xor    %edx,%edx
-   2e2311d1f:	jmp    0x2e2311d53
-   2e2311d21:	nopl   0x0(%rax)
-   2e2311d28:	movslq %r11d,%rdx
-   2e2311d2b:	add    $0x1,%r10d
-   2e2311d2f:	add    $0x10,%rax
-   2e2311d33:	add    $0x1,%r11d
-   2e2311d37:	shl    $0x4,%rdx
-   2e2311d3b:	movslq 0x8(%r14,%rdx,1),%rdx
-   2e2311d40:	movsd  %xmm0,0x0(%rbp,%rdx,8)
-   2e2311d46:	cmp    %r9d,%r10d
-   2e2311d49:	jge    0x2e2311d64
-   2e2311d4b:	movslq 0x8(%rax),%rdx
-   2e2311d4f:	mov    (%r12,%rdx,4),%edx
-   2e2311d53:	test   %edx,%edx
-   2e2311d55:	je     0x2e2311d28
-   2e2311d57:	add    $0x10,%rax
-   2e2311d5b:	add    $0x1,%r11d
-   2e2311d5f:	cmp    %r10d,%r9d
-   2e2311d62:	jg     0x2e2311d4b
-   2e2311d64:	add    %ecx,%edi
-   2e2311d66:	add    $0x1,%edi
-   2e2311d69:	cmp    %r13d,%edi
-   2e2311d6c:	jl     0x2e2311c7c
-   2e2311d72:	mov    0x48(%rsp),%r13
-   2e2311d77:	mov    0x30(%rsp),%r15
-   2e2311d7c:	mov    0xb8(%rsp),%rbx
-   2e2311d84:	mov    0x3c(%rsp),%eax
-   2e2311d88:	movsd  0x3278(%rip),%xmm2        # 0x2e2315008
-   2e2311d90:	xor    %esi,%esi
-   2e2311d92:	test   %eax,%eax
-   2e2311d94:	je     0x2e2311eb6
-   2e2311d9a:	mov    %r14,0x30(%rsp)
-   2e2311d9f:	mov    0x3c(%rsp),%ebp
-   2e2311da3:	mov    0x40(%rsp),%r14d
-   2e2311da8:	jmp    0x2e2311dbb
-   2e2311daa:	nopw   0x0(%rax,%rax,1)
-   2e2311db0:	add    $0x1,%esi
-   2e2311db3:	cmp    %ebp,%esi
-   2e2311db5:	jge    0x2e2311eb1
-   2e2311dbb:	movslq %esi,%rax
-   2e2311dbe:	shl    $0x4,%rax
-   2e2311dc2:	add    %r13,%rax
-   2e2311dc5:	movslq 0x8(%rax),%rdx
-   2e2311dc9:	mov    (%r12,%rdx,4),%r10d
-   2e2311dcd:	test   %r10d,%r10d
-   2e2311dd0:	jne    0x2e2311db0
-   2e2311dd2:	movsd  (%rbx,%rdx,8),%xmm0
-   2e2311dd7:	mov    %ebp,%edx
-   2e2311dd9:	sub    %esi,%edx
-   2e2311ddb:	test   %edx,%edx
-   2e2311ddd:	jle    0x2e2311f3a
-   2e2311de3:	lea    -0x1(%rsi,%rdx,1),%edi
-   2e2311de7:	mov    %esi,%r11d
-   2e2311dea:	mov    %esi,%edx
-   2e2311dec:	mov    %rax,%rcx
-   2e2311def:	xor    %r8d,%r8d
-   2e2311df2:	xor    %r9d,%r9d
-   2e2311df5:	jmp    0x2e2311e0b
-   2e2311df7:	nopw   0x0(%rax,%rax,1)
-   2e2311e00:	movslq 0x8(%rcx),%r8
-   2e2311e04:	add    $0x1,%edx
-   2e2311e07:	mov    (%r12,%r8,4),%r8d
-   2e2311e0b:	test   %r8d,%r8d
-   2e2311e0e:	jne    0x2e2311e30
-   2e2311e10:	movslq %edx,%r8
-   2e2311e13:	shl    $0x4,%r8
-   2e2311e17:	movslq 0x8(%r13,%r8,1),%r8
-   2e2311e1c:	ucomisd (%rbx,%r8,8),%xmm0
-   2e2311e22:	jp     0x2e2311e38
-   2e2311e24:	comisd (%rbx,%r8,8),%xmm0
-   2e2311e2a:	jne    0x2e2311e38
-   2e2311e2c:	add    $0x1,%r9d
-   2e2311e30:	add    $0x10,%rcx
-   2e2311e34:	cmp    %edx,%edi
-   2e2311e36:	jne    0x2e2311e00
-   2e2311e38:	lea    -0x1(%r9),%ecx
-   2e2311e3c:	pxor   %xmm0,%xmm0
-   2e2311e40:	pxor   %xmm1,%xmm1
-   2e2311e44:	cvtsi2sd %ecx,%xmm0
-   2e2311e48:	cvtsi2sd %r14d,%xmm1
-   2e2311e4d:	add    %r9d,%r14d
-   2e2311e50:	mulsd  %xmm2,%xmm0
-   2e2311e54:	addsd  %xmm1,%xmm0
-   2e2311e58:	test   %r9d,%r9d
-   2e2311e5b:	je     0x2e2311ea4
-   2e2311e5d:	xor    %edx,%edx
-   2e2311e5f:	jmp    0x2e2311e93
-   2e2311e61:	nopl   0x0(%rax)
-   2e2311e68:	movslq %r11d,%rdx
-   2e2311e6b:	add    $0x1,%r10d
-   2e2311e6f:	add    $0x10,%rax
-   2e2311e73:	add    $0x1,%r11d
-   2e2311e77:	shl    $0x4,%rdx
-   2e2311e7b:	movslq 0x8(%r13,%rdx,1),%rdx
-   2e2311e80:	movsd  %xmm0,(%r15,%rdx,8)
-   2e2311e86:	cmp    %r9d,%r10d
-   2e2311e89:	jge    0x2e2311ea4
-   2e2311e8b:	movslq 0x8(%rax),%rdx
-   2e2311e8f:	mov    (%r12,%rdx,4),%edx
-   2e2311e93:	test   %edx,%edx
-   2e2311e95:	je     0x2e2311e68
-   2e2311e97:	add    $0x10,%rax
-   2e2311e9b:	add    $0x1,%r11d
-   2e2311e9f:	cmp    %r10d,%r9d
-   2e2311ea2:	jg     0x2e2311e8b
-   2e2311ea4:	add    %ecx,%esi
-   2e2311ea6:	add    $0x1,%esi
-   2e2311ea9:	cmp    %ebp,%esi
-   2e2311eab:	jl     0x2e2311dbb
-   2e2311eb1:	mov    0x30(%rsp),%r14
-   2e2311eb6:	mov    0x28(%rsp),%rbx
-   2e2311ebb:	mov    0xc0(%rsp),%r8d
-   2e2311ec3:	mov    %r15,%rdx
-   2e2311ec6:	mov    %rbx,%rcx
-   2e2311ec9:	call   0x2e2311590
-   2e2311ece:	mov    %r14,%rcx
-   2e2311ed1:	movupd %xmm0,%xmm6
-   2e2311ed5:	call   0x2e2312f48
-   2e2311eda:	mov    %r13,%rcx
-   2e2311edd:	call   0x2e2312f48
-   2e2311ee2:	mov    %rbx,%rcx
-   2e2311ee5:	call   0x2e2312f48
-   2e2311eea:	mov    %r15,%rcx
-   2e2311eed:	call   0x2e2312f48
-   2e2311ef2:	mov    %r12,%rcx
-   2e2311ef5:	call   0x2e2312f48
-   2e2311efa:	movupd %xmm6,%xmm0
-   2e2311efe:	movups 0x50(%rsp),%xmm6
-   2e2311f03:	add    $0x68,%rsp
-   2e2311f07:	pop    %rbx
-   2e2311f08:	pop    %rsi
-   2e2311f09:	pop    %rdi
-   2e2311f0a:	pop    %rbp
-   2e2311f0b:	pop    %r12
-   2e2311f0d:	pop    %r13
-   2e2311f0f:	pop    %r14
-   2e2311f11:	pop    %r15
-   2e2311f13:	ret
-   2e2311f14:	movl   $0x1,(%r12,%rax,4)
-   2e2311f1c:	lea    0x1(%rax),%rdx
-   2e2311f20:	cmp    %rax,%rcx
-   2e2311f23:	jne    0x2e2311c08
-   2e2311f29:	jmp    0x2e2311c37
-   2e2311f2e:	mov    $0xffffffff,%ecx
-   2e2311f33:	add    %ecx,%edi
-   2e2311f35:	jmp    0x2e2311d66
-   2e2311f3a:	mov    $0xffffffff,%ecx
-   2e2311f3f:	add    %ecx,%esi
-   2e2311f41:	jmp    0x2e2311ea6
-   2e2311f46:	xor    %edx,%edx
-   2e2311f48:	mov    %r14,%rcx
-   2e2311f4b:	lea    -0xbb2(%rip),%r9        # 0x2e23113a0
-   2e2311f52:	mov    $0x10,%r8d
-   2e2311f58:	call   0x2e2312f28
-   2e2311f5d:	mov    $0x10,%r8d
-   2e2311f63:	xor    %edx,%edx
-   2e2311f65:	mov    %r13,%rcx
-   2e2311f68:	lea    -0xbcf(%rip),%r9        # 0x2e23113a0
-   2e2311f6f:	call   0x2e2312f28
-   2e2311f74:	jmp    0x2e2311eb6
-   2e2311f79:	movl   $0x1,0x40(%rsp)
-   2e2311f81:	jmp    0x2e2311bee
-   2e2311f86:	test   %edx,%edx
-   2e2311f88:	je     0x2e2311be0
-   2e2311f8e:	mov    $0x1,%r9d
-   2e2311f94:	jmp    0x2e2311b6c
-   2e2311f99:	xor    %edx,%edx
-   2e2311f9b:	jmp    0x2e2311ad9
-   2e2311fa0:	imul   %r9d,%r8d
-   2e2311fa4:	mov    %r9d,%eax
-   2e2311fa7:	imul   %r9d,%edx
-   2e2311fab:	mov    0x28(%rsp),%r9d
-   2e2311fb0:	movslq %r8d,%r8
-   2e2311fb3:	lea    (%rcx,%r8,8),%r10
-   2e2311fb7:	movslq %edx,%rdx
-   2e2311fba:	mov    %eax,%r8d
-   2e2311fbd:	lea    (%rcx,%rdx,8),%rcx
-   2e2311fc1:	mov    %r10,%rdx
-   2e2311fc4:	jmp    0x2e23118c0
-   2e2311fc9:	nopl   0x0(%rax)
-   2e2311fd0:	imul   %r9d,%r8d
-   2e2311fd4:	imul   %r9d,%edx
-   2e2311fd8:	movslq %r8d,%r8
-   2e2311fdb:	lea    (%rcx,%r8,8),%r10
-   2e2311fdf:	movslq %edx,%rdx
-   2e2311fe2:	mov    %r9d,%r8d
-   2e2311fe5:	lea    (%rcx,%rdx,8),%rcx
-   2e2311fe9:	mov    %r10,%rdx
-   2e2311fec:	jmp    0x2e2311590
-   2e2311ff1:	nop
-   2e2311ff2:	nop
-   2e2311ff3:	nop
-   2e2311ff4:	nop
-   2e2311ff5:	nop
-   2e2311ff6:	nop
-   2e2311ff7:	nop
-   2e2311ff8:	nop
-   2e2311ff9:	nop
-   2e2311ffa:	nop
-   2e2311ffb:	nop
-   2e2311ffc:	nop
-   2e2311ffd:	nop
-   2e2311ffe:	nop
-   2e2311fff:	nop
-   2e2312000:	sub    $0x28,%rsp
-   2e2312004:	mov    0x2005(%rip),%rax        # 0x2e2314010
-   2e231200b:	mov    (%rax),%rax
-   2e231200e:	test   %rax,%rax
-   2e2312011:	je     0x2e2312035
-   2e2312013:	nopl   0x0(%rax,%rax,1)
-   2e2312018:	call   *%rax
-   2e231201a:	mov    0x1fef(%rip),%rax        # 0x2e2314010
-   2e2312021:	lea    0x8(%rax),%rdx
-   2e2312025:	mov    0x8(%rax),%rax
-   2e2312029:	mov    %rdx,0x1fe0(%rip)        # 0x2e2314010
-   2e2312030:	test   %rax,%rax
-   2e2312033:	jne    0x2e2312018
-   2e2312035:	add    $0x28,%rsp
-   2e2312039:	ret
-   2e231203a:	nopw   0x0(%rax,%rax,1)
-   2e2312040:	push   %rsi
-   2e2312041:	push   %rbx
-   2e2312042:	sub    $0x28,%rsp
-   2e2312046:	mov    0x3183(%rip),%rdx        # 0x2e23151d0
-   2e231204d:	mov    (%rdx),%rax
-   2e2312050:	mov    %eax,%ecx
-   2e2312052:	cmp    $0xffffffff,%eax
-   2e2312055:	je     0x2e2312090
-   2e2312057:	test   %ecx,%ecx
-   2e2312059:	je     0x2e231207b
-   2e231205b:	mov    %ecx,%eax
-   2e231205d:	sub    $0x1,%ecx
-   2e2312060:	lea    (%rdx,%rax,8),%rbx
-   2e2312064:	sub    %rcx,%rax
-   2e2312067:	lea    -0x8(%rdx,%rax,8),%rsi
-   2e231206c:	nopl   0x0(%rax)
-   2e2312070:	call   *(%rbx)
-   2e2312072:	sub    $0x8,%rbx
-   2e2312076:	cmp    %rsi,%rbx
-   2e2312079:	jne    0x2e2312070
-   2e231207b:	lea    -0x82(%rip),%rcx        # 0x2e2312000
-   2e2312082:	add    $0x28,%rsp
-   2e2312086:	pop    %rbx
-   2e2312087:	pop    %rsi
-   2e2312088:	jmp    0x2e2311370
-   2e231208d:	nopl   (%rax)
-   2e2312090:	xor    %eax,%eax
-   2e2312092:	nopw   0x0(%rax,%rax,1)
-   2e2312098:	lea    0x1(%rax),%r8d
-   2e231209c:	mov    %eax,%ecx
-   2e231209e:	cmpq   $0x0,(%rdx,%r8,8)
-   2e23120a3:	mov    %r8,%rax
-   2e23120a6:	jne    0x2e2312098
-   2e23120a8:	jmp    0x2e2312057
-   2e23120aa:	nopw   0x0(%rax,%rax,1)
-   2e23120b0:	mov    0x5f6a(%rip),%eax        # 0x2e2318020
-   2e23120b6:	test   %eax,%eax
-   2e23120b8:	je     0x2e23120c0
-   2e23120ba:	ret
-   2e23120bb:	nopl   0x0(%rax,%rax,1)
-   2e23120c0:	movl   $0x1,0x5f56(%rip)        # 0x2e2318020
-   2e23120ca:	jmp    0x2e2312040
-   2e23120cf:	nop
-   2e23120d0:	sub    $0x28,%rsp
-   2e23120d4:	cmp    $0x3,%edx
-   2e23120d7:	je     0x2e23120f0
-   2e23120d9:	test   %edx,%edx
-   2e23120db:	je     0x2e23120f0
-   2e23120dd:	mov    $0x1,%eax
-   2e23120e2:	add    $0x28,%rsp
-   2e23120e6:	ret
-   2e23120e7:	nopw   0x0(%rax,%rax,1)
-   2e23120f0:	call   0x2e23128a0
-   2e23120f5:	mov    $0x1,%eax
-   2e23120fa:	add    $0x28,%rsp
-   2e23120fe:	ret
-   2e23120ff:	nop
-   2e2312100:	push   %rsi
-   2e2312101:	push   %rbx
-   2e2312102:	sub    $0x28,%rsp
-   2e2312106:	mov    0x30b3(%rip),%rax        # 0x2e23151c0
-   2e231210d:	cmpl   $0x2,(%rax)
-   2e2312110:	je     0x2e2312118
-   2e2312112:	movl   $0x2,(%rax)
-   2e2312118:	cmp    $0x2,%edx
+   2e2311b2b:	je     0x2e2311fc2
+   2e2311b31:	mov    0x20(%rsp),%r10
+   2e2311b36:	mov    0x30(%rsp),%r11
+   2e2311b3b:	movslq %ebp,%rax
+   2e2311b3e:	lea    0x1(%rbp),%r9d
+   2e2311b42:	nopw   0x0(%rax,%rax,1)
+   2e2311b48:	mov    %r9d,%r8d
+   2e2311b4b:	pxor   %xmm0,%xmm0
+   2e2311b4f:	movslq -0x4(%r11,%rax,4),%rcx
+   2e2311b54:	sub    %eax,%r8d
+   2e2311b57:	sub    $0x1,%rax
+   2e2311b5b:	cvtsi2sd %r8d,%xmm0
+   2e2311b60:	movsd  %xmm0,(%r10,%rcx,8)
+   2e2311b66:	test   %eax,%eax
+   2e2311b68:	jne    0x2e2311b48
+   2e2311b6a:	mov    %r9d,%r11d
+   2e2311b6d:	test   %edx,%edx
+   2e2311b6f:	je     0x2e2311fb5
+   2e2311b75:	mov    0x38(%rsp),%r9
+   2e2311b7a:	movslq %edx,%rax
+   2e2311b7d:	lea    0x1(%rdx),%r8d
+   2e2311b81:	nopl   0x0(%rax)
+   2e2311b88:	mov    %r8d,%ecx
+   2e2311b8b:	pxor   %xmm0,%xmm0
+   2e2311b8f:	movslq -0x4(%r9,%rax,4),%rdx
+   2e2311b94:	sub    %eax,%ecx
+   2e2311b96:	sub    $0x1,%rax
+   2e2311b9a:	cvtsi2sd %ecx,%xmm0
+   2e2311b9e:	movsd  %xmm0,(%r15,%rdx,8)
+   2e2311ba4:	test   %eax,%eax
+   2e2311ba6:	jne    0x2e2311b88
+   2e2311ba8:	mov    %r8d,0x44(%rsp)
+   2e2311bad:	jmp    0x2e2311bfe
+   2e2311baf:	lea    (%r12,%r8,1),%edx
+   2e2311bb3:	sub    $0x1,%r8d
+   2e2311bb7:	movslq %edx,%rdx
+   2e2311bba:	shl    $0x4,%rdx
+   2e2311bbe:	add    %r13,%rdx
+   2e2311bc1:	mov    %r11d,0x8(%rdx)
+   2e2311bc5:	movsd  %xmm1,(%rdx)
+   2e2311bc9:	jmp    0x2e23119eb
+   2e2311bce:	lea    (%r12,%r9,1),%edx
+   2e2311bd2:	sub    $0x1,%r9d
+   2e2311bd6:	movslq %edx,%rdx
+   2e2311bd9:	shl    $0x4,%rdx
+   2e2311bdd:	add    %r14,%rdx
+   2e2311be0:	mov    %eax,0x8(%rdx)
+   2e2311be3:	movsd  %xmm1,(%rdx)
+   2e2311be7:	jmp    0x2e23119c6
+   2e2311bec:	nopl   0x0(%rax)
+   2e2311bf0:	movl   $0x1,0x44(%rsp)
+   2e2311bf8:	mov    $0x1,%r11d
+   2e2311bfe:	mov    0xc0(%rsp),%eax
+   2e2311c05:	mov    0x20(%rsp),%r8
+   2e2311c0a:	lea    -0x1(%rax),%ecx
+   2e2311c0d:	xor    %eax,%eax
+   2e2311c0f:	jmp    0x2e2311c1b
+   2e2311c11:	nopl   0x0(%rax)
+   2e2311c18:	mov    %rdx,%rax
+   2e2311c1b:	movsd  (%r15,%rax,8),%xmm0
+   2e2311c21:	ucomisd %xmm0,%xmm0
+   2e2311c25:	jp     0x2e2311f38
+   2e2311c2b:	movsd  (%r8,%rax,8),%xmm0
+   2e2311c31:	xor    %edx,%edx
+   2e2311c33:	ucomisd %xmm0,%xmm0
+   2e2311c37:	setp   %dl
+   2e2311c3a:	mov    %edx,(%r12,%rax,4)
+   2e2311c3e:	lea    0x1(%rax),%rdx
+   2e2311c42:	cmp    %rax,%rcx
+   2e2311c45:	jne    0x2e2311c18
+   2e2311c47:	mov    0x28(%rsp),%edx
+   2e2311c4b:	movsd  0x33b5(%rip),%xmm2        # 0x2e2315008
+   2e2311c53:	xor    %edi,%edi
+   2e2311c55:	test   %edx,%edx
+   2e2311c57:	je     0x2e2311d94
+   2e2311c5d:	mov    %r13,0x48(%rsp)
+   2e2311c62:	mov    0x20(%rsp),%rbp
+   2e2311c67:	mov    0x28(%rsp),%r13d
+   2e2311c6c:	mov    %rbx,0xb8(%rsp)
+   2e2311c74:	mov    %r15,0x28(%rsp)
+   2e2311c79:	mov    %r11d,%r15d
+   2e2311c7c:	jmp    0x2e2311c8c
+   2e2311c7e:	xchg   %ax,%ax
+   2e2311c80:	add    $0x1,%edi
+   2e2311c83:	cmp    %r13d,%edi
+   2e2311c86:	jge    0x2e2311d82
+   2e2311c8c:	movslq %edi,%rax
+   2e2311c8f:	shl    $0x4,%rax
+   2e2311c93:	add    %r14,%rax
+   2e2311c96:	movslq 0x8(%rax),%rdx
+   2e2311c9a:	mov    (%r12,%rdx,4),%r10d
+   2e2311c9e:	test   %r10d,%r10d
+   2e2311ca1:	jne    0x2e2311c80
+   2e2311ca3:	movsd  (%rsi,%rdx,8),%xmm0
+   2e2311ca8:	mov    %r13d,%edx
+   2e2311cab:	sub    %edi,%edx
+   2e2311cad:	test   %edx,%edx
+   2e2311caf:	jle    0x2e2311f52
+   2e2311cb5:	lea    -0x1(%rdi,%rdx,1),%ebx
+   2e2311cb9:	mov    %edi,%r11d
+   2e2311cbc:	mov    %edi,%edx
+   2e2311cbe:	mov    %rax,%rcx
+   2e2311cc1:	xor    %r8d,%r8d
+   2e2311cc4:	xor    %r9d,%r9d
+   2e2311cc7:	jmp    0x2e2311cdb
+   2e2311cc9:	nopl   0x0(%rax)
+   2e2311cd0:	movslq 0x8(%rcx),%r8
+   2e2311cd4:	add    $0x1,%edx
+   2e2311cd7:	mov    (%r12,%r8,4),%r8d
+   2e2311cdb:	test   %r8d,%r8d
+   2e2311cde:	jne    0x2e2311d00
+   2e2311ce0:	movslq %edx,%r8
+   2e2311ce3:	shl    $0x4,%r8
+   2e2311ce7:	movslq 0x8(%r14,%r8,1),%r8
+   2e2311cec:	ucomisd (%rsi,%r8,8),%xmm0
+   2e2311cf2:	jp     0x2e2311d08
+   2e2311cf4:	comisd (%rsi,%r8,8),%xmm0
+   2e2311cfa:	jne    0x2e2311d08
+   2e2311cfc:	add    $0x1,%r9d
+   2e2311d00:	add    $0x10,%rcx
+   2e2311d04:	cmp    %edx,%ebx
+   2e2311d06:	jne    0x2e2311cd0
+   2e2311d08:	lea    -0x1(%r9),%ecx
+   2e2311d0c:	pxor   %xmm0,%xmm0
+   2e2311d10:	pxor   %xmm1,%xmm1
+   2e2311d14:	cvtsi2sd %ecx,%xmm0
+   2e2311d18:	cvtsi2sd %r15d,%xmm1
+   2e2311d1d:	add    %r9d,%r15d
+   2e2311d20:	mulsd  %xmm2,%xmm0
+   2e2311d24:	addsd  %xmm1,%xmm0
+   2e2311d28:	test   %r9d,%r9d
+   2e2311d2b:	je     0x2e2311d74
+   2e2311d2d:	xor    %edx,%edx
+   2e2311d2f:	jmp    0x2e2311d63
+   2e2311d31:	nopl   0x0(%rax)
+   2e2311d38:	movslq %r11d,%rdx
+   2e2311d3b:	add    $0x1,%r10d
+   2e2311d3f:	add    $0x10,%rax
+   2e2311d43:	add    $0x1,%r11d
+   2e2311d47:	shl    $0x4,%rdx
+   2e2311d4b:	movslq 0x8(%r14,%rdx,1),%rdx
+   2e2311d50:	movsd  %xmm0,0x0(%rbp,%rdx,8)
+   2e2311d56:	cmp    %r9d,%r10d
+   2e2311d59:	jge    0x2e2311d74
+   2e2311d5b:	movslq 0x8(%rax),%rdx
+   2e2311d5f:	mov    (%r12,%rdx,4),%edx
+   2e2311d63:	test   %edx,%edx
+   2e2311d65:	je     0x2e2311d38
+   2e2311d67:	add    $0x10,%rax
+   2e2311d6b:	add    $0x1,%r11d
+   2e2311d6f:	cmp    %r10d,%r9d
+   2e2311d72:	jg     0x2e2311d5b
+   2e2311d74:	add    %ecx,%edi
+   2e2311d76:	add    $0x1,%edi
+   2e2311d79:	cmp    %r13d,%edi
+   2e2311d7c:	jl     0x2e2311c8c
+   2e2311d82:	mov    0x48(%rsp),%r13
+   2e2311d87:	mov    0x28(%rsp),%r15
+   2e2311d8c:	mov    0xb8(%rsp),%rbx
+   2e2311d94:	mov    0x40(%rsp),%eax
+   2e2311d98:	movsd  0x3268(%rip),%xmm2        # 0x2e2315008
+   2e2311da0:	xor    %esi,%esi
+   2e2311da2:	test   %eax,%eax
+   2e2311da4:	je     0x2e2311ec6
+   2e2311daa:	mov    %r14,0x28(%rsp)
+   2e2311daf:	mov    0x40(%rsp),%ebp
+   2e2311db3:	mov    0x44(%rsp),%r14d
+   2e2311db8:	jmp    0x2e2311dcb
+   2e2311dba:	nopw   0x0(%rax,%rax,1)
+   2e2311dc0:	add    $0x1,%esi
+   2e2311dc3:	cmp    %ebp,%esi
+   2e2311dc5:	jge    0x2e2311ec1
+   2e2311dcb:	movslq %esi,%rax
+   2e2311dce:	shl    $0x4,%rax
+   2e2311dd2:	add    %r13,%rax
+   2e2311dd5:	movslq 0x8(%rax),%rdx
+   2e2311dd9:	mov    (%r12,%rdx,4),%r10d
+   2e2311ddd:	test   %r10d,%r10d
+   2e2311de0:	jne    0x2e2311dc0
+   2e2311de2:	movsd  (%rbx,%rdx,8),%xmm0
+   2e2311de7:	mov    %ebp,%edx
+   2e2311de9:	sub    %esi,%edx
+   2e2311deb:	test   %edx,%edx
+   2e2311ded:	jle    0x2e2311f5e
+   2e2311df3:	lea    -0x1(%rsi,%rdx,1),%edi
+   2e2311df7:	mov    %esi,%r11d
+   2e2311dfa:	mov    %esi,%edx
+   2e2311dfc:	mov    %rax,%rcx
+   2e2311dff:	xor    %r8d,%r8d
+   2e2311e02:	xor    %r9d,%r9d
+   2e2311e05:	jmp    0x2e2311e1b
+   2e2311e07:	nopw   0x0(%rax,%rax,1)
+   2e2311e10:	movslq 0x8(%rcx),%r8
+   2e2311e14:	add    $0x1,%edx
+   2e2311e17:	mov    (%r12,%r8,4),%r8d
+   2e2311e1b:	test   %r8d,%r8d
+   2e2311e1e:	jne    0x2e2311e40
+   2e2311e20:	movslq %edx,%r8
+   2e2311e23:	shl    $0x4,%r8
+   2e2311e27:	movslq 0x8(%r13,%r8,1),%r8
+   2e2311e2c:	ucomisd (%rbx,%r8,8),%xmm0
+   2e2311e32:	jp     0x2e2311e48
+   2e2311e34:	comisd (%rbx,%r8,8),%xmm0
+   2e2311e3a:	jne    0x2e2311e48
+   2e2311e3c:	add    $0x1,%r9d
+   2e2311e40:	add    $0x10,%rcx
+   2e2311e44:	cmp    %edi,%edx
+   2e2311e46:	jne    0x2e2311e10
+   2e2311e48:	lea    -0x1(%r9),%ecx
+   2e2311e4c:	pxor   %xmm0,%xmm0
+   2e2311e50:	pxor   %xmm1,%xmm1
+   2e2311e54:	cvtsi2sd %ecx,%xmm0
+   2e2311e58:	cvtsi2sd %r14d,%xmm1
+   2e2311e5d:	add    %r9d,%r14d
+   2e2311e60:	mulsd  %xmm2,%xmm0
+   2e2311e64:	addsd  %xmm1,%xmm0
+   2e2311e68:	test   %r9d,%r9d
+   2e2311e6b:	je     0x2e2311eb4
+   2e2311e6d:	xor    %edx,%edx
+   2e2311e6f:	jmp    0x2e2311ea3
+   2e2311e71:	nopl   0x0(%rax)
+   2e2311e78:	movslq %r11d,%rdx
+   2e2311e7b:	add    $0x1,%r10d
+   2e2311e7f:	add    $0x10,%rax
+   2e2311e83:	add    $0x1,%r11d
+   2e2311e87:	shl    $0x4,%rdx
+   2e2311e8b:	movslq 0x8(%r13,%rdx,1),%rdx
+   2e2311e90:	movsd  %xmm0,(%r15,%rdx,8)
+   2e2311e96:	cmp    %r9d,%r10d
+   2e2311e99:	jge    0x2e2311eb4
+   2e2311e9b:	movslq 0x8(%rax),%rdx
+   2e2311e9f:	mov    (%r12,%rdx,4),%edx
+   2e2311ea3:	test   %edx,%edx
+   2e2311ea5:	je     0x2e2311e78
+   2e2311ea7:	add    $0x10,%rax
+   2e2311eab:	add    $0x1,%r11d
+   2e2311eaf:	cmp    %r10d,%r9d
+   2e2311eb2:	jg     0x2e2311e9b
+   2e2311eb4:	add    %ecx,%esi
+   2e2311eb6:	add    $0x1,%esi
+   2e2311eb9:	cmp    %ebp,%esi
+   2e2311ebb:	jl     0x2e2311dcb
+   2e2311ec1:	mov    0x28(%rsp),%r14
+   2e2311ec6:	mov    0x20(%rsp),%rdi
+   2e2311ecb:	mov    0xc0(%rsp),%r8d
+   2e2311ed3:	mov    %r15,%rdx
+   2e2311ed6:	mov    %rdi,%rcx
+   2e2311ed9:	call   0x2e2311590
+   2e2311ede:	mov    %r14,%rcx
+   2e2311ee1:	movupd %xmm0,%xmm6
+   2e2311ee5:	call   0x2e2312f88
+   2e2311eea:	mov    %r13,%rcx
+   2e2311eed:	call   0x2e2312f88
+   2e2311ef2:	mov    %rdi,%rcx
+   2e2311ef5:	call   0x2e2312f88
+   2e2311efa:	mov    %r15,%rcx
+   2e2311efd:	call   0x2e2312f88
+   2e2311f02:	mov    %r12,%rcx
+   2e2311f05:	call   0x2e2312f88
+   2e2311f0a:	mov    0x38(%rsp),%rcx
+   2e2311f0f:	call   0x2e2312f88
+   2e2311f14:	mov    0x30(%rsp),%rcx
+   2e2311f19:	call   0x2e2312f88
+   2e2311f1e:	movupd %xmm6,%xmm0
+   2e2311f22:	movups 0x50(%rsp),%xmm6
+   2e2311f27:	add    $0x68,%rsp
+   2e2311f2b:	pop    %rbx
+   2e2311f2c:	pop    %rsi
+   2e2311f2d:	pop    %rdi
+   2e2311f2e:	pop    %rbp
+   2e2311f2f:	pop    %r12
+   2e2311f31:	pop    %r13
+   2e2311f33:	pop    %r14
+   2e2311f35:	pop    %r15
+   2e2311f37:	ret
+   2e2311f38:	movl   $0x1,(%r12,%rax,4)
+   2e2311f40:	lea    0x1(%rax),%rdx
+   2e2311f44:	cmp    %rax,%rcx
+   2e2311f47:	jne    0x2e2311c18
+   2e2311f4d:	jmp    0x2e2311c47
+   2e2311f52:	mov    $0xffffffff,%ecx
+   2e2311f57:	add    %ecx,%edi
+   2e2311f59:	jmp    0x2e2311d76
+   2e2311f5e:	mov    $0xffffffff,%ecx
+   2e2311f63:	add    %ecx,%esi
+   2e2311f65:	jmp    0x2e2311eb6
+   2e2311f6a:	lea    -0xbd1(%rip),%r9        # 0x2e23113a0
+   2e2311f71:	mov    $0x10,%r8d
+   2e2311f77:	xor    %edx,%edx
+   2e2311f79:	mov    %r14,%rcx
+   2e2311f7c:	call   0x2e2312f68
+   2e2311f81:	mov    $0x10,%r8d
+   2e2311f87:	xor    %edx,%edx
+   2e2311f89:	mov    %r13,%rcx
+   2e2311f8c:	lea    -0xbf3(%rip),%r9        # 0x2e23113a0
+   2e2311f93:	call   0x2e2312f68
+   2e2311f98:	xor    %ecx,%ecx
+   2e2311f9a:	call   0x2e2312f78
+   2e2311f9f:	xor    %ecx,%ecx
+   2e2311fa1:	mov    %rax,0x38(%rsp)
+   2e2311fa6:	call   0x2e2312f78
+   2e2311fab:	mov    %rax,0x30(%rsp)
+   2e2311fb0:	jmp    0x2e2311ec6
+   2e2311fb5:	movl   $0x1,0x44(%rsp)
+   2e2311fbd:	jmp    0x2e2311bfe
+   2e2311fc2:	test   %edx,%edx
+   2e2311fc4:	je     0x2e2311bf0
+   2e2311fca:	mov    $0x1,%r11d
+   2e2311fd0:	jmp    0x2e2311b75
+   2e2311fd5:	xor    %edx,%edx
+   2e2311fd7:	jmp    0x2e2311ad9
+   2e2311fdc:	nopl   0x0(%rax)
+   2e2311fe0:	imul   %r9d,%r8d
+   2e2311fe4:	mov    %r9d,%eax
+   2e2311fe7:	imul   %r9d,%edx
+   2e2311feb:	mov    0x28(%rsp),%r9d
+   2e2311ff0:	movslq %r8d,%r8
+   2e2311ff3:	lea    (%rcx,%r8,8),%r10
+   2e2311ff7:	movslq %edx,%rdx
+   2e2311ffa:	mov    %eax,%r8d
+   2e2311ffd:	lea    (%rcx,%rdx,8),%rcx
+   2e2312001:	mov    %r10,%rdx
+   2e2312004:	jmp    0x2e23118c0
+   2e2312009:	nopl   0x0(%rax)
+   2e2312010:	imul   %r9d,%r8d
+   2e2312014:	imul   %r9d,%edx
+   2e2312018:	movslq %r8d,%r8
+   2e231201b:	lea    (%rcx,%r8,8),%r10
+   2e231201f:	movslq %edx,%rdx
+   2e2312022:	mov    %r9d,%r8d
+   2e2312025:	lea    (%rcx,%rdx,8),%rcx
+   2e2312029:	mov    %r10,%rdx
+   2e231202c:	jmp    0x2e2311590
+   2e2312031:	nop
+   2e2312032:	nop
+   2e2312033:	nop
+   2e2312034:	nop
+   2e2312035:	nop
+   2e2312036:	nop
+   2e2312037:	nop
+   2e2312038:	nop
+   2e2312039:	nop
+   2e231203a:	nop
+   2e231203b:	nop
+   2e231203c:	nop
+   2e231203d:	nop
+   2e231203e:	nop
+   2e231203f:	nop
+   2e2312040:	sub    $0x28,%rsp
+   2e2312044:	mov    0x1fc5(%rip),%rax        # 0x2e2314010
+   2e231204b:	mov    (%rax),%rax
+   2e231204e:	test   %rax,%rax
+   2e2312051:	je     0x2e2312075
+   2e2312053:	nopl   0x0(%rax,%rax,1)
+   2e2312058:	call   *%rax
+   2e231205a:	mov    0x1faf(%rip),%rax        # 0x2e2314010
+   2e2312061:	lea    0x8(%rax),%rdx
+   2e2312065:	mov    0x8(%rax),%rax
+   2e2312069:	mov    %rdx,0x1fa0(%rip)        # 0x2e2314010
+   2e2312070:	test   %rax,%rax
+   2e2312073:	jne    0x2e2312058
+   2e2312075:	add    $0x28,%rsp
+   2e2312079:	ret
+   2e231207a:	nopw   0x0(%rax,%rax,1)
+   2e2312080:	push   %rsi
+   2e2312081:	push   %rbx
+   2e2312082:	sub    $0x28,%rsp
+   2e2312086:	mov    0x3143(%rip),%rdx        # 0x2e23151d0
+   2e231208d:	mov    (%rdx),%rax
+   2e2312090:	mov    %eax,%ecx
+   2e2312092:	cmp    $0xffffffff,%eax
+   2e2312095:	je     0x2e23120d0
+   2e2312097:	test   %ecx,%ecx
+   2e2312099:	je     0x2e23120bb
+   2e231209b:	mov    %ecx,%eax
+   2e231209d:	sub    $0x1,%ecx
+   2e23120a0:	lea    (%rdx,%rax,8),%rbx
+   2e23120a4:	sub    %rcx,%rax
+   2e23120a7:	lea    -0x8(%rdx,%rax,8),%rsi
+   2e23120ac:	nopl   0x0(%rax)
+   2e23120b0:	call   *(%rbx)
+   2e23120b2:	sub    $0x8,%rbx
+   2e23120b6:	cmp    %rsi,%rbx
+   2e23120b9:	jne    0x2e23120b0
+   2e23120bb:	lea    -0x82(%rip),%rcx        # 0x2e2312040
+   2e23120c2:	add    $0x28,%rsp
+   2e23120c6:	pop    %rbx
+   2e23120c7:	pop    %rsi
+   2e23120c8:	jmp    0x2e2311370
+   2e23120cd:	nopl   (%rax)
+   2e23120d0:	xor    %eax,%eax
+   2e23120d2:	nopw   0x0(%rax,%rax,1)
+   2e23120d8:	lea    0x1(%rax),%r8d
+   2e23120dc:	mov    %eax,%ecx
+   2e23120de:	cmpq   $0x0,(%rdx,%r8,8)
+   2e23120e3:	mov    %r8,%rax
+   2e23120e6:	jne    0x2e23120d8
+   2e23120e8:	jmp    0x2e2312097
+   2e23120ea:	nopw   0x0(%rax,%rax,1)
+   2e23120f0:	mov    0x5f2a(%rip),%eax        # 0x2e2318020
+   2e23120f6:	test   %eax,%eax
+   2e23120f8:	je     0x2e2312100
+   2e23120fa:	ret
+   2e23120fb:	nopl   0x0(%rax,%rax,1)
+   2e2312100:	movl   $0x1,0x5f16(%rip)        # 0x2e2318020
+   2e231210a:	jmp    0x2e2312080
+   2e231210f:	nop
+   2e2312110:	sub    $0x28,%rsp
+   2e2312114:	cmp    $0x3,%edx
+   2e2312117:	je     0x2e2312130
+   2e2312119:	test   %edx,%edx
    2e231211b:	je     0x2e2312130
-   2e231211d:	cmp    $0x1,%edx
-   2e2312120:	je     0x2e2312170
-   2e2312122:	mov    $0x1,%eax
-   2e2312127:	add    $0x28,%rsp
-   2e231212b:	pop    %rbx
-   2e231212c:	pop    %rsi
-   2e231212d:	ret
-   2e231212e:	xchg   %ax,%ax
-   2e2312130:	lea    0x8f19(%rip),%rbx        # 0x2e231b050
-   2e2312137:	lea    0x8f12(%rip),%rsi        # 0x2e231b050
-   2e231213e:	cmp    %rbx,%rsi
-   2e2312141:	je     0x2e2312122
-   2e2312143:	nopl   0x0(%rax,%rax,1)
-   2e2312148:	mov    (%rbx),%rax
-   2e231214b:	test   %rax,%rax
-   2e231214e:	je     0x2e2312152
-   2e2312150:	call   *%rax
-   2e2312152:	add    $0x8,%rbx
-   2e2312156:	cmp    %rbx,%rsi
-   2e2312159:	jne    0x2e2312148
-   2e231215b:	mov    $0x1,%eax
-   2e2312160:	add    $0x28,%rsp
-   2e2312164:	pop    %rbx
-   2e2312165:	pop    %rsi
-   2e2312166:	ret
-   2e2312167:	nopw   0x0(%rax,%rax,1)
-   2e2312170:	call   0x2e23128a0
-   2e2312175:	mov    $0x1,%eax
-   2e231217a:	add    $0x28,%rsp
-   2e231217e:	pop    %rbx
-   2e231217f:	pop    %rsi
-   2e2312180:	ret
-   2e2312181:	data16 cs nopw 0x0(%rax,%rax,1)
-   2e231218c:	nopl   0x0(%rax)
-   2e2312190:	xor    %eax,%eax
-   2e2312192:	ret
-   2e2312193:	nop
-   2e2312194:	nop
-   2e2312195:	nop
-   2e2312196:	nop
-   2e2312197:	nop
-   2e2312198:	nop
-   2e2312199:	nop
-   2e231219a:	nop
-   2e231219b:	nop
-   2e231219c:	nop
-   2e231219d:	nop
-   2e231219e:	nop
-   2e231219f:	nop
-   2e23121a0:	push   %r12
-   2e23121a2:	push   %rbx
-   2e23121a3:	sub    $0x38,%rsp
-   2e23121a7:	mov    %rcx,%r12
-   2e23121aa:	lea    0x58(%rsp),%rax
-   2e23121af:	mov    $0x2,%ecx
-   2e23121b4:	mov    %rdx,0x58(%rsp)
-   2e23121b9:	mov    %r8,0x60(%rsp)
-   2e23121be:	mov    %r9,0x68(%rsp)
-   2e23121c3:	mov    %rax,0x28(%rsp)
-   2e23121c8:	call   0x2e2313110
-   2e23121cd:	mov    $0x1b,%r8d
-   2e23121d3:	mov    $0x1,%edx
-   2e23121d8:	lea    0x2ea1(%rip),%rcx        # 0x2e2315080
-   2e23121df:	mov    %rax,%r9
-   2e23121e2:	call   0x2e2312f40
-   2e23121e7:	mov    0x28(%rsp),%rbx
-   2e23121ec:	mov    $0x2,%ecx
-   2e23121f1:	call   0x2e2313110
-   2e23121f6:	mov    %r12,%rdx
-   2e23121f9:	mov    %rax,%rcx
-   2e23121fc:	mov    %rbx,%r8
-   2e23121ff:	call   0x2e2312f10
-   2e2312204:	call   0x2e2312f58
-   2e2312209:	nop
-   2e231220a:	nopw   0x0(%rax,%rax,1)
-   2e2312210:	push   %r12
-   2e2312212:	push   %rbp
-   2e2312213:	push   %rdi
-   2e2312214:	push   %rsi
-   2e2312215:	push   %rbx
-   2e2312216:	sub    $0x50,%rsp
-   2e231221a:	movslq 0x5e33(%rip),%rdi        # 0x2e2318054
-   2e2312221:	mov    %rcx,%r12
-   2e2312224:	mov    %rdx,%rsi
-   2e2312227:	mov    %r8,%rbx
-   2e231222a:	test   %edi,%edi
-   2e231222c:	jle    0x2e23123c0
-   2e2312232:	mov    0x5e1f(%rip),%rax        # 0x2e2318058
-   2e2312239:	xor    %ecx,%ecx
-   2e231223b:	add    $0x18,%rax
-   2e231223f:	nop
-   2e2312240:	mov    (%rax),%rdx
-   2e2312243:	cmp    %rdx,%r12
-   2e2312246:	jb     0x2e231225c
-   2e2312248:	mov    0x8(%rax),%r8
-   2e231224c:	mov    0x8(%r8),%r8d
-   2e2312250:	add    %r8,%rdx
-   2e2312253:	cmp    %rdx,%r12
-   2e2312256:	jb     0x2e23122e7
-   2e231225c:	add    $0x1,%ecx
-   2e231225f:	add    $0x28,%rax
-   2e2312263:	cmp    %edi,%ecx
-   2e2312265:	jne    0x2e2312240
-   2e2312267:	mov    %r12,%rcx
-   2e231226a:	call   0x2e2312ab0
-   2e231226f:	mov    %rax,%rbp
-   2e2312272:	test   %rax,%rax
-   2e2312275:	je     0x2e231241d
-   2e231227b:	mov    0x5dd6(%rip),%rax        # 0x2e2318058
-   2e2312282:	lea    (%rdi,%rdi,4),%rdi
-   2e2312286:	shl    $0x3,%rdi
-   2e231228a:	add    %rdi,%rax
-   2e231228d:	mov    %rbp,0x20(%rax)
-   2e2312291:	movl   $0x0,(%rax)
-   2e2312297:	call   0x2e2312be0
-   2e231229c:	mov    0xc(%rbp),%ecx
-   2e231229f:	lea    0x20(%rsp),%rdx
-   2e23122a4:	mov    $0x30,%r8d
-   2e23122aa:	add    %rax,%rcx
-   2e23122ad:	mov    0x5da4(%rip),%rax        # 0x2e2318058
-   2e23122b4:	mov    %rcx,0x18(%rax,%rdi,1)
-   2e23122b9:	call   *0x7ea5(%rip)        # 0x2e231a164
-   2e23122bf:	test   %rax,%rax
-   2e23122c2:	je     0x2e2312402
-   2e23122c8:	mov    0x44(%rsp),%eax
-   2e23122cc:	lea    -0x40(%rax),%edx
-   2e23122cf:	and    $0xffffffbf,%edx
-   2e23122d2:	je     0x2e23122e0
-   2e23122d4:	lea    -0x4(%rax),%edx
-   2e23122d7:	and    $0xfffffffb,%edx
-   2e23122da:	jne    0x2e2312370
-   2e23122e0:	addl   $0x1,0x5d6d(%rip)        # 0x2e2318054
-   2e23122e7:	cmp    $0x8,%ebx
-   2e23122ea:	jae    0x2e2312318
-   2e23122ec:	test   $0x4,%bl
-   2e23122ef:	jne    0x2e23123d0
-   2e23122f5:	test   %ebx,%ebx
-   2e23122f7:	je     0x2e2312309
-   2e23122f9:	movzbl (%rsi),%eax
-   2e23122fc:	mov    %al,(%r12)
-   2e2312300:	test   $0x2,%bl
-   2e2312303:	jne    0x2e23123f0
-   2e2312309:	add    $0x50,%rsp
-   2e231230d:	pop    %rbx
-   2e231230e:	pop    %rsi
-   2e231230f:	pop    %rdi
-   2e2312310:	pop    %rbp
-   2e2312311:	pop    %r12
-   2e2312313:	ret
-   2e2312314:	nopl   0x0(%rax)
-   2e2312318:	mov    (%rsi),%rax
-   2e231231b:	lea    0x8(%r12),%rcx
-   2e2312320:	and    $0xfffffffffffffff8,%rcx
-   2e2312324:	mov    %rax,(%r12)
-   2e2312328:	mov    %ebx,%eax
-   2e231232a:	mov    -0x8(%rsi,%rax,1),%rdx
-   2e231232f:	mov    %rdx,-0x8(%r12,%rax,1)
-   2e2312334:	sub    %rcx,%r12
-   2e2312337:	add    %r12d,%ebx
-   2e231233a:	sub    %r12,%rsi
-   2e231233d:	and    $0xfffffff8,%ebx
-   2e2312340:	cmp    $0x8,%ebx
-   2e2312343:	jb     0x2e2312309
-   2e2312345:	and    $0xfffffff8,%ebx
-   2e2312348:	xor    %eax,%eax
-   2e231234a:	mov    %eax,%edx
-   2e231234c:	add    $0x8,%eax
-   2e231234f:	mov    (%rsi,%rdx,1),%r8
-   2e2312353:	mov    %r8,(%rcx,%rdx,1)
-   2e2312357:	cmp    %ebx,%eax
-   2e2312359:	jb     0x2e231234a
-   2e231235b:	add    $0x50,%rsp
-   2e231235f:	pop    %rbx
-   2e2312360:	pop    %rsi
-   2e2312361:	pop    %rdi
-   2e2312362:	pop    %rbp
-   2e2312363:	pop    %r12
-   2e2312365:	ret
-   2e2312366:	cs nopw 0x0(%rax,%rax,1)
-   2e2312370:	cmp    $0x2,%eax
-   2e2312373:	mov    0x20(%rsp),%rcx
-   2e2312378:	mov    0x38(%rsp),%rdx
-   2e231237d:	mov    $0x4,%r8d
-   2e2312383:	mov    $0x40,%eax
-   2e2312388:	cmovne %eax,%r8d
-   2e231238c:	add    0x5cc5(%rip),%rdi        # 0x2e2318058
-   2e2312393:	mov    %rcx,0x8(%rdi)
-   2e2312397:	mov    %rdi,%r9
-   2e231239a:	mov    %rdx,0x10(%rdi)
-   2e231239e:	call   *0x7db8(%rip)        # 0x2e231a15c
-   2e23123a4:	test   %eax,%eax
-   2e23123a6:	jne    0x2e23122e0
-   2e23123ac:	call   *0x7d82(%rip)        # 0x2e231a134
-   2e23123b2:	lea    0x2d3f(%rip),%rcx        # 0x2e23150f8
-   2e23123b9:	mov    %eax,%edx
-   2e23123bb:	call   0x2e23121a0
-   2e23123c0:	xor    %edi,%edi
-   2e23123c2:	jmp    0x2e2312267
-   2e23123c7:	nopw   0x0(%rax,%rax,1)
-   2e23123d0:	mov    (%rsi),%eax
-   2e23123d2:	mov    %ebx,%ebx
-   2e23123d4:	mov    %eax,(%r12)
-   2e23123d8:	mov    -0x4(%rsi,%rbx,1),%eax
-   2e23123dc:	mov    %eax,-0x4(%r12,%rbx,1)
-   2e23123e1:	jmp    0x2e2312309
-   2e23123e6:	cs nopw 0x0(%rax,%rax,1)
-   2e23123f0:	mov    %ebx,%ebx
-   2e23123f2:	movzwl -0x2(%rsi,%rbx,1),%eax
-   2e23123f7:	mov    %ax,-0x2(%r12,%rbx,1)
-   2e23123fd:	jmp    0x2e2312309
-   2e2312402:	mov    0x5c4f(%rip),%rax        # 0x2e2318058
-   2e2312409:	mov    0x8(%rbp),%edx
-   2e231240c:	lea    0x2cad(%rip),%rcx        # 0x2e23150c0
-   2e2312413:	mov    0x18(%rax,%rdi,1),%r8
-   2e2312418:	call   0x2e23121a0
-   2e231241d:	mov    %r12,%rdx
-   2e2312420:	lea    0x2c79(%rip),%rcx        # 0x2e23150a0
-   2e2312427:	call   0x2e23121a0
-   2e231242c:	nop
-   2e231242d:	nopl   (%rax)
-   2e2312430:	push   %rbp
-   2e2312431:	push   %r15
-   2e2312433:	push   %r14
-   2e2312435:	push   %r13
-   2e2312437:	push   %r12
-   2e2312439:	push   %rdi
-   2e231243a:	push   %rsi
-   2e231243b:	push   %rbx
-   2e231243c:	sub    $0x38,%rsp
-   2e2312440:	lea    0x80(%rsp),%rbp
-   2e2312448:	mov    0x5c02(%rip),%esi        # 0x2e2318050
-   2e231244e:	test   %esi,%esi
-   2e2312450:	je     0x2e2312468
-   2e2312452:	lea    -0x48(%rbp),%rsp
-   2e2312456:	pop    %rbx
-   2e2312457:	pop    %rsi
-   2e2312458:	pop    %rdi
-   2e2312459:	pop    %r12
-   2e231245b:	pop    %r13
-   2e231245d:	pop    %r14
-   2e231245f:	pop    %r15
-   2e2312461:	pop    %rbp
-   2e2312462:	ret
-   2e2312463:	nopl   0x0(%rax,%rax,1)
-   2e2312468:	movl   $0x1,0x5bde(%rip)        # 0x2e2318050
-   2e2312472:	call   0x2e2312b40
-   2e2312477:	cltq
-   2e2312479:	lea    (%rax,%rax,4),%rax
-   2e231247d:	lea    0xf(,%rax,8),%rax
-   2e2312485:	and    $0xfffffffffffffff0,%rax
-   2e2312489:	call   0x2e2312d70
-   2e231248e:	mov    0x2d4b(%rip),%r12        # 0x2e23151e0
-   2e2312495:	mov    0x2d54(%rip),%rbx        # 0x2e23151f0
-   2e231249c:	movl   $0x0,0x5bae(%rip)        # 0x2e2318054
-   2e23124a6:	sub    %rax,%rsp
-   2e23124a9:	lea    0x20(%rsp),%rax
-   2e23124ae:	mov    %rax,0x5ba3(%rip)        # 0x2e2318058
-   2e23124b5:	mov    %r12,%rax
-   2e23124b8:	sub    %rbx,%rax
-   2e23124bb:	cmp    $0x7,%rax
-   2e23124bf:	jle    0x2e2312452
-   2e23124c1:	mov    (%rbx),%edx
-   2e23124c3:	cmp    $0xb,%rax
-   2e23124c7:	jg     0x2e2312618
-   2e23124cd:	test   %edx,%edx
-   2e23124cf:	jne    0x2e23126a0
-   2e23124d5:	mov    0x4(%rbx),%eax
-   2e23124d8:	test   %eax,%eax
-   2e23124da:	jne    0x2e23126a0
-   2e23124e0:	mov    0x8(%rbx),%edx
-   2e23124e3:	cmp    $0x1,%edx
-   2e23124e6:	jne    0x2e2312708
-   2e23124ec:	add    $0xc,%rbx
-   2e23124f0:	lea    -0x58(%rbp),%r15
-   2e23124f4:	mov    0x2d15(%rip),%r13        # 0x2e2315210
-   2e23124fb:	movabs $0xffffffff00000000,%r14
-   2e2312505:	cmp    %r12,%rbx
-   2e2312508:	jb     0x2e2312549
-   2e231250a:	jmp    0x2e2312452
-   2e231250f:	nop
-   2e2312510:	movzbl (%rcx),%r8d
-   2e2312514:	mov    %r15,%rdi
-   2e2312517:	mov    %r8,%r10
-   2e231251a:	or     $0xffffffffffffff00,%r10
-   2e2312521:	test   %r8b,%r8b
-   2e2312524:	cmovs  %r10,%r8
-   2e2312528:	sub    %rdx,%r8
-   2e231252b:	mov    %r15,%rdx
-   2e231252e:	add    %r9,%r8
-   2e2312531:	mov    %r8,-0x58(%rbp)
-   2e2312535:	mov    $0x1,%r8d
-   2e231253b:	call   0x2e2312210
-   2e2312540:	add    $0xc,%rbx
-   2e2312544:	cmp    %r12,%rbx
-   2e2312547:	jae    0x2e23125c0
-   2e2312549:	mov    (%rbx),%edx
-   2e231254b:	mov    0x4(%rbx),%ecx
-   2e231254e:	movzbl 0x8(%rbx),%r8d
-   2e2312553:	add    %r13,%rdx
-   2e2312556:	add    %r13,%rcx
-   2e2312559:	mov    (%rdx),%r9
-   2e231255c:	cmp    $0x20,%r8d
-   2e2312560:	je     0x2e2312670
-   2e2312566:	ja     0x2e2312640
-   2e231256c:	cmp    $0x8,%r8d
-   2e2312570:	je     0x2e2312510
-   2e2312572:	cmp    $0x10,%r8d
-   2e2312576:	jne    0x2e23126f1
-   2e231257c:	movzwl (%rcx),%r8d
-   2e2312580:	mov    %r15,%rdi
-   2e2312583:	mov    %r8,%r10
-   2e2312586:	or     $0xffffffffffff0000,%r10
-   2e231258d:	test   %r8w,%r8w
-   2e2312591:	cmovs  %r10,%r8
-   2e2312595:	add    $0xc,%rbx
-   2e2312599:	sub    %rdx,%r8
-   2e231259c:	mov    %r15,%rdx
-   2e231259f:	add    %r9,%r8
-   2e23125a2:	mov    %r8,-0x58(%rbp)
-   2e23125a6:	mov    $0x2,%r8d
-   2e23125ac:	call   0x2e2312210
-   2e23125b1:	cmp    %r12,%rbx
-   2e23125b4:	jb     0x2e2312549
-   2e23125b6:	cs nopw 0x0(%rax,%rax,1)
-   2e23125c0:	mov    0x5a8e(%rip),%eax        # 0x2e2318054
-   2e23125c6:	test   %eax,%eax
-   2e23125c8:	jle    0x2e2312452
-   2e23125ce:	mov    0x7b87(%rip),%r12        # 0x2e231a15c
-   2e23125d5:	xor    %ebx,%ebx
-   2e23125d7:	nopw   0x0(%rax,%rax,1)
-   2e23125e0:	mov    0x5a71(%rip),%rax        # 0x2e2318058
-   2e23125e7:	add    %rbx,%rax
-   2e23125ea:	mov    (%rax),%r8d
-   2e23125ed:	test   %r8d,%r8d
-   2e23125f0:	je     0x2e2312600
-   2e23125f2:	mov    0x10(%rax),%rdx
-   2e23125f6:	mov    0x8(%rax),%rcx
-   2e23125fa:	mov    %rdi,%r9
-   2e23125fd:	call   *%r12
-   2e2312600:	add    $0x1,%esi
-   2e2312603:	add    $0x28,%rbx
-   2e2312607:	cmp    0x5a47(%rip),%esi        # 0x2e2318054
-   2e231260d:	jl     0x2e23125e0
-   2e231260f:	jmp    0x2e2312452
-   2e2312614:	nopl   0x0(%rax)
-   2e2312618:	test   %edx,%edx
-   2e231261a:	jne    0x2e23126a0
-   2e2312620:	mov    0x4(%rbx),%eax
-   2e2312623:	mov    %eax,%edi
-   2e2312625:	or     0x8(%rbx),%edi
-   2e2312628:	jne    0x2e23124d8
-   2e231262e:	mov    0xc(%rbx),%edx
-   2e2312631:	add    $0xc,%rbx
-   2e2312635:	jmp    0x2e23124cd
-   2e231263a:	nopw   0x0(%rax,%rax,1)
-   2e2312640:	cmp    $0x40,%r8d
-   2e2312644:	jne    0x2e23126f1
-   2e231264a:	mov    (%rcx),%rax
-   2e231264d:	mov    $0x8,%r8d
-   2e2312653:	mov    %r15,%rdi
-   2e2312656:	sub    %rdx,%rax
-   2e2312659:	mov    %r15,%rdx
-   2e231265c:	add    %r9,%rax
-   2e231265f:	mov    %rax,-0x58(%rbp)
-   2e2312663:	call   0x2e2312210
-   2e2312668:	jmp    0x2e2312540
-   2e231266d:	nopl   (%rax)
-   2e2312670:	mov    (%rcx),%eax
-   2e2312672:	mov    %r15,%rdi
-   2e2312675:	mov    %rax,%r8
-   2e2312678:	or     %r14,%rax
-   2e231267b:	test   %r8d,%r8d
-   2e231267e:	cmovns %r8,%rax
-   2e2312682:	mov    $0x4,%r8d
-   2e2312688:	sub    %rdx,%rax
-   2e231268b:	mov    %r15,%rdx
-   2e231268e:	add    %r9,%rax
-   2e2312691:	mov    %rax,-0x58(%rbp)
-   2e2312695:	call   0x2e2312210
-   2e231269a:	jmp    0x2e2312540
-   2e231269f:	nop
-   2e23126a0:	cmp    %r12,%rbx
-   2e23126a3:	jae    0x2e2312452
-   2e23126a9:	sub    $0x1,%r12
-   2e23126ad:	mov    0x2b5c(%rip),%r13        # 0x2e2315210
-   2e23126b4:	lea    -0x58(%rbp),%rdi
-   2e23126b8:	sub    %rbx,%r12
-   2e23126bb:	shr    $0x3,%r12
-   2e23126bf:	lea    0x8(%rbx,%r12,8),%r12
-   2e23126c4:	nopl   0x0(%rax)
-   2e23126c8:	mov    0x4(%rbx),%ecx
-   2e23126cb:	mov    (%rbx),%eax
-   2e23126cd:	mov    $0x4,%r8d
-   2e23126d3:	mov    %rdi,%rdx
-   2e23126d6:	add    $0x8,%rbx
-   2e23126da:	add    %r13,%rcx
-   2e23126dd:	add    (%rcx),%eax
-   2e23126df:	mov    %eax,-0x58(%rbp)
-   2e23126e2:	call   0x2e2312210
-   2e23126e7:	cmp    %r12,%rbx
-   2e23126ea:	jne    0x2e23126c8
-   2e23126ec:	jmp    0x2e23125c0
-   2e23126f1:	mov    %r8d,%edx
-   2e23126f4:	lea    0x2a5d(%rip),%rcx        # 0x2e2315158
-   2e23126fb:	movq   $0x0,-0x58(%rbp)
-   2e2312703:	call   0x2e23121a0
-   2e2312708:	lea    0x2a11(%rip),%rcx        # 0x2e2315120
-   2e231270f:	call   0x2e23121a0
-   2e2312714:	nop
-   2e2312715:	nop
-   2e2312716:	nop
-   2e2312717:	nop
-   2e2312718:	nop
-   2e2312719:	nop
-   2e231271a:	nop
-   2e231271b:	nop
-   2e231271c:	nop
-   2e231271d:	nop
-   2e231271e:	nop
-   2e231271f:	nop
-   2e2312720:	push   %r12
-   2e2312722:	push   %rdi
-   2e2312723:	push   %rsi
-   2e2312724:	push   %rbx
-   2e2312725:	sub    $0x28,%rsp
-   2e2312729:	lea    0x5950(%rip),%rcx        # 0x2e2318080
-   2e2312730:	call   *0x79f6(%rip)        # 0x2e231a12c
-   2e2312736:	mov    0x5923(%rip),%rbx        # 0x2e2318060
-   2e231273d:	test   %rbx,%rbx
-   2e2312740:	je     0x2e2312774
-   2e2312742:	mov    0x7a0b(%rip),%rdi        # 0x2e231a154
-   2e2312749:	mov    0x79e4(%rip),%rsi        # 0x2e231a134
-   2e2312750:	mov    (%rbx),%ecx
-   2e2312752:	call   *%rdi
-   2e2312754:	mov    %rax,%r12
-   2e2312757:	call   *%rsi
-   2e2312759:	test   %eax,%eax
-   2e231275b:	jne    0x2e231276b
-   2e231275d:	test   %r12,%r12
-   2e2312760:	je     0x2e231276b
-   2e2312762:	mov    0x8(%rbx),%rax
-   2e2312766:	mov    %r12,%rcx
-   2e2312769:	call   *%rax
-   2e231276b:	mov    0x10(%rbx),%rbx
-   2e231276f:	test   %rbx,%rbx
-   2e2312772:	jne    0x2e2312750
-   2e2312774:	lea    0x5905(%rip),%rcx        # 0x2e2318080
-   2e231277b:	add    $0x28,%rsp
-   2e231277f:	pop    %rbx
-   2e2312780:	pop    %rsi
-   2e2312781:	pop    %rdi
-   2e2312782:	pop    %r12
-   2e2312784:	rex.W jmp *0x79b9(%rip)        # 0x2e231a144
-   2e231278b:	nopl   0x0(%rax,%rax,1)
-   2e2312790:	push   %rdi
-   2e2312791:	push   %rsi
-   2e2312792:	push   %rbx
-   2e2312793:	sub    $0x20,%rsp
-   2e2312797:	mov    0x58cb(%rip),%eax        # 0x2e2318068
-   2e231279d:	mov    %ecx,%edi
-   2e231279f:	mov    %rdx,%rsi
-   2e23127a2:	test   %eax,%eax
-   2e23127a4:	jne    0x2e23127b0
-   2e23127a6:	add    $0x20,%rsp
-   2e23127aa:	pop    %rbx
-   2e23127ab:	pop    %rsi
-   2e23127ac:	pop    %rdi
-   2e23127ad:	ret
-   2e23127ae:	xchg   %ax,%ax
-   2e23127b0:	mov    $0x18,%edx
-   2e23127b5:	mov    $0x1,%ecx
-   2e23127ba:	call   0x2e2312f50
-   2e23127bf:	mov    %rax,%rbx
-   2e23127c2:	test   %rax,%rax
-   2e23127c5:	je     0x2e2312803
-   2e23127c7:	mov    %edi,(%rax)
-   2e23127c9:	lea    0x58b0(%rip),%rcx        # 0x2e2318080
-   2e23127d0:	mov    %rsi,0x8(%rax)
-   2e23127d4:	call   *0x7952(%rip)        # 0x2e231a12c
-   2e23127da:	mov    0x587f(%rip),%rax        # 0x2e2318060
-   2e23127e1:	lea    0x5898(%rip),%rcx        # 0x2e2318080
-   2e23127e8:	mov    %rbx,0x5871(%rip)        # 0x2e2318060
-   2e23127ef:	mov    %rax,0x10(%rbx)
-   2e23127f3:	call   *0x794b(%rip)        # 0x2e231a144
-   2e23127f9:	xor    %eax,%eax
-   2e23127fb:	add    $0x20,%rsp
-   2e23127ff:	pop    %rbx
-   2e2312800:	pop    %rsi
-   2e2312801:	pop    %rdi
-   2e2312802:	ret
-   2e2312803:	or     $0xffffffff,%eax
-   2e2312806:	jmp    0x2e23127a6
-   2e2312808:	nopl   0x0(%rax,%rax,1)
-   2e2312810:	push   %rbx
-   2e2312811:	sub    $0x20,%rsp
-   2e2312815:	mov    0x584d(%rip),%eax        # 0x2e2318068
-   2e231281b:	mov    %ecx,%ebx
-   2e231281d:	test   %eax,%eax
-   2e231281f:	jne    0x2e2312830
-   2e2312821:	xor    %eax,%eax
-   2e2312823:	add    $0x20,%rsp
-   2e2312827:	pop    %rbx
-   2e2312828:	ret
-   2e2312829:	nopl   0x0(%rax)
-   2e2312830:	lea    0x5849(%rip),%rcx        # 0x2e2318080
-   2e2312837:	call   *0x78ef(%rip)        # 0x2e231a12c
-   2e231283d:	mov    0x581c(%rip),%rcx        # 0x2e2318060
-   2e2312844:	test   %rcx,%rcx
-   2e2312847:	je     0x2e2312873
-   2e2312849:	xor    %edx,%edx
-   2e231284b:	jmp    0x2e231285b
-   2e231284d:	nopl   (%rax)
-   2e2312850:	mov    %rcx,%rdx
-   2e2312853:	test   %rax,%rax
-   2e2312856:	je     0x2e2312873
-   2e2312858:	mov    %rax,%rcx
-   2e231285b:	mov    (%rcx),%eax
-   2e231285d:	cmp    %ebx,%eax
-   2e231285f:	mov    0x10(%rcx),%rax
-   2e2312863:	jne    0x2e2312850
-   2e2312865:	test   %rdx,%rdx
-   2e2312868:	je     0x2e2312890
-   2e231286a:	mov    %rax,0x10(%rdx)
-   2e231286e:	call   0x2e2312f48
-   2e2312873:	lea    0x5806(%rip),%rcx        # 0x2e2318080
-   2e231287a:	call   *0x78c4(%rip)        # 0x2e231a144
-   2e2312880:	xor    %eax,%eax
-   2e2312882:	add    $0x20,%rsp
-   2e2312886:	pop    %rbx
-   2e2312887:	ret
-   2e2312888:	nopl   0x0(%rax,%rax,1)
-   2e2312890:	mov    %rax,0x57c9(%rip)        # 0x2e2318060
-   2e2312897:	jmp    0x2e231286e
-   2e2312899:	nopl   0x0(%rax)
-   2e23128a0:	push   %rbx
-   2e23128a1:	sub    $0x20,%rsp
-   2e23128a5:	cmp    $0x2,%edx
-   2e23128a8:	je     0x2e2312970
-   2e23128ae:	ja     0x2e23128d8
-   2e23128b0:	test   %edx,%edx
-   2e23128b2:	je     0x2e2312900
-   2e23128b4:	mov    0x57ae(%rip),%eax        # 0x2e2318068
-   2e23128ba:	test   %eax,%eax
-   2e23128bc:	je     0x2e23128f0
-   2e23128be:	movl   $0x1,0x57a0(%rip)        # 0x2e2318068
-   2e23128c8:	mov    $0x1,%eax
-   2e23128cd:	add    $0x20,%rsp
-   2e23128d1:	pop    %rbx
-   2e23128d2:	ret
-   2e23128d3:	nopl   0x0(%rax,%rax,1)
-   2e23128d8:	cmp    $0x3,%edx
-   2e23128db:	jne    0x2e23128c8
-   2e23128dd:	mov    0x5785(%rip),%eax        # 0x2e2318068
-   2e23128e3:	test   %eax,%eax
-   2e23128e5:	je     0x2e23128c8
-   2e23128e7:	call   0x2e2312720
-   2e23128ec:	jmp    0x2e23128c8
-   2e23128ee:	xchg   %ax,%ax
-   2e23128f0:	lea    0x5789(%rip),%rcx        # 0x2e2318080
-   2e23128f7:	call   *0x783f(%rip)        # 0x2e231a13c
-   2e23128fd:	jmp    0x2e23128be
-   2e23128ff:	nop
-   2e2312900:	mov    0x5762(%rip),%eax        # 0x2e2318068
-   2e2312906:	test   %eax,%eax
-   2e2312908:	je     0x2e231290f
-   2e231290a:	call   0x2e2312720
-   2e231290f:	mov    0x5753(%rip),%eax        # 0x2e2318068
-   2e2312915:	cmp    $0x1,%eax
-   2e2312918:	jne    0x2e23128c8
-   2e231291a:	mov    0x573f(%rip),%rbx        # 0x2e2318060
-   2e2312921:	test   %rbx,%rbx
-   2e2312924:	je     0x2e2312941
-   2e2312926:	cs nopw 0x0(%rax,%rax,1)
-   2e2312930:	mov    %rbx,%rcx
-   2e2312933:	mov    0x10(%rbx),%rbx
-   2e2312937:	call   0x2e2312f48
-   2e231293c:	test   %rbx,%rbx
-   2e231293f:	jne    0x2e2312930
-   2e2312941:	lea    0x5738(%rip),%rcx        # 0x2e2318080
-   2e2312948:	movq   $0x0,0x570d(%rip)        # 0x2e2318060
-   2e2312953:	movl   $0x0,0x570b(%rip)        # 0x2e2318068
-   2e231295d:	call   *0x77c1(%rip)        # 0x2e231a124
-   2e2312963:	jmp    0x2e23128c8
-   2e2312968:	nopl   0x0(%rax,%rax,1)
-   2e2312970:	call   0x2e2312d60
-   2e2312975:	mov    $0x1,%eax
-   2e231297a:	add    $0x20,%rsp
-   2e231297e:	pop    %rbx
-   2e231297f:	ret
-   2e2312980:	movslq 0x3c(%rcx),%rax
-   2e2312984:	lea    (%rax,%rcx,1),%rdx
-   2e2312988:	xor    %eax,%eax
-   2e231298a:	cmpl   $0x4550,(%rdx)
-   2e2312990:	jne    0x2e231299d
-   2e2312992:	xor    %eax,%eax
-   2e2312994:	cmpw   $0x20b,0x18(%rdx)
-   2e231299a:	sete   %al
-   2e231299d:	ret
-   2e231299e:	xchg   %ax,%ax
-   2e23129a0:	cmpw   $0x5a4d,(%rcx)
-   2e23129a5:	jne    0x2e23129b0
-   2e23129a7:	jmp    0x2e2312980
-   2e23129a9:	nopl   0x0(%rax)
-   2e23129b0:	xor    %eax,%eax
-   2e23129b2:	ret
-   2e23129b3:	data16 cs nopw 0x0(%rax,%rax,1)
-   2e23129be:	xchg   %ax,%ax
+   2e231211d:	mov    $0x1,%eax
+   2e2312122:	add    $0x28,%rsp
+   2e2312126:	ret
+   2e2312127:	nopw   0x0(%rax,%rax,1)
+   2e2312130:	call   0x2e23128e0
+   2e2312135:	mov    $0x1,%eax
+   2e231213a:	add    $0x28,%rsp
+   2e231213e:	ret
+   2e231213f:	nop
+   2e2312140:	push   %rsi
+   2e2312141:	push   %rbx
+   2e2312142:	sub    $0x28,%rsp
+   2e2312146:	mov    0x3073(%rip),%rax        # 0x2e23151c0
+   2e231214d:	cmpl   $0x2,(%rax)
+   2e2312150:	je     0x2e2312158
+   2e2312152:	movl   $0x2,(%rax)
+   2e2312158:	cmp    $0x2,%edx
+   2e231215b:	je     0x2e2312170
+   2e231215d:	cmp    $0x1,%edx
+   2e2312160:	je     0x2e23121b0
+   2e2312162:	mov    $0x1,%eax
+   2e2312167:	add    $0x28,%rsp
+   2e231216b:	pop    %rbx
+   2e231216c:	pop    %rsi
+   2e231216d:	ret
+   2e231216e:	xchg   %ax,%ax
+   2e2312170:	lea    0x8ed9(%rip),%rbx        # 0x2e231b050
+   2e2312177:	lea    0x8ed2(%rip),%rsi        # 0x2e231b050
+   2e231217e:	cmp    %rbx,%rsi
+   2e2312181:	je     0x2e2312162
+   2e2312183:	nopl   0x0(%rax,%rax,1)
+   2e2312188:	mov    (%rbx),%rax
+   2e231218b:	test   %rax,%rax
+   2e231218e:	je     0x2e2312192
+   2e2312190:	call   *%rax
+   2e2312192:	add    $0x8,%rbx
+   2e2312196:	cmp    %rbx,%rsi
+   2e2312199:	jne    0x2e2312188
+   2e231219b:	mov    $0x1,%eax
+   2e23121a0:	add    $0x28,%rsp
+   2e23121a4:	pop    %rbx
+   2e23121a5:	pop    %rsi
+   2e23121a6:	ret
+   2e23121a7:	nopw   0x0(%rax,%rax,1)
+   2e23121b0:	call   0x2e23128e0
+   2e23121b5:	mov    $0x1,%eax
+   2e23121ba:	add    $0x28,%rsp
+   2e23121be:	pop    %rbx
+   2e23121bf:	pop    %rsi
+   2e23121c0:	ret
+   2e23121c1:	data16 cs nopw 0x0(%rax,%rax,1)
+   2e23121cc:	nopl   0x0(%rax)
+   2e23121d0:	xor    %eax,%eax
+   2e23121d2:	ret
+   2e23121d3:	nop
+   2e23121d4:	nop
+   2e23121d5:	nop
+   2e23121d6:	nop
+   2e23121d7:	nop
+   2e23121d8:	nop
+   2e23121d9:	nop
+   2e23121da:	nop
+   2e23121db:	nop
+   2e23121dc:	nop
+   2e23121dd:	nop
+   2e23121de:	nop
+   2e23121df:	nop
+   2e23121e0:	push   %r12
+   2e23121e2:	push   %rbx
+   2e23121e3:	sub    $0x38,%rsp
+   2e23121e7:	mov    %rcx,%r12
+   2e23121ea:	lea    0x58(%rsp),%rax
+   2e23121ef:	mov    $0x2,%ecx
+   2e23121f4:	mov    %rdx,0x58(%rsp)
+   2e23121f9:	mov    %r8,0x60(%rsp)
+   2e23121fe:	mov    %r9,0x68(%rsp)
+   2e2312203:	mov    %rax,0x28(%rsp)
+   2e2312208:	call   0x2e2313150
+   2e231220d:	mov    $0x1b,%r8d
+   2e2312213:	mov    $0x1,%edx
+   2e2312218:	lea    0x2e61(%rip),%rcx        # 0x2e2315080
+   2e231221f:	mov    %rax,%r9
+   2e2312222:	call   0x2e2312f80
+   2e2312227:	mov    0x28(%rsp),%rbx
+   2e231222c:	mov    $0x2,%ecx
+   2e2312231:	call   0x2e2313150
+   2e2312236:	mov    %r12,%rdx
+   2e2312239:	mov    %rax,%rcx
+   2e231223c:	mov    %rbx,%r8
+   2e231223f:	call   0x2e2312f50
+   2e2312244:	call   0x2e2312f98
+   2e2312249:	nop
+   2e231224a:	nopw   0x0(%rax,%rax,1)
+   2e2312250:	push   %r12
+   2e2312252:	push   %rbp
+   2e2312253:	push   %rdi
+   2e2312254:	push   %rsi
+   2e2312255:	push   %rbx
+   2e2312256:	sub    $0x50,%rsp
+   2e231225a:	movslq 0x5df3(%rip),%rdi        # 0x2e2318054
+   2e2312261:	mov    %rcx,%r12
+   2e2312264:	mov    %rdx,%rsi
+   2e2312267:	mov    %r8,%rbx
+   2e231226a:	test   %edi,%edi
+   2e231226c:	jle    0x2e2312400
+   2e2312272:	mov    0x5ddf(%rip),%rax        # 0x2e2318058
+   2e2312279:	xor    %ecx,%ecx
+   2e231227b:	add    $0x18,%rax
+   2e231227f:	nop
+   2e2312280:	mov    (%rax),%rdx
+   2e2312283:	cmp    %rdx,%r12
+   2e2312286:	jb     0x2e231229c
+   2e2312288:	mov    0x8(%rax),%r8
+   2e231228c:	mov    0x8(%r8),%r8d
+   2e2312290:	add    %r8,%rdx
+   2e2312293:	cmp    %rdx,%r12
+   2e2312296:	jb     0x2e2312327
+   2e231229c:	add    $0x1,%ecx
+   2e231229f:	add    $0x28,%rax
+   2e23122a3:	cmp    %edi,%ecx
+   2e23122a5:	jne    0x2e2312280
+   2e23122a7:	mov    %r12,%rcx
+   2e23122aa:	call   0x2e2312af0
+   2e23122af:	mov    %rax,%rbp
+   2e23122b2:	test   %rax,%rax
+   2e23122b5:	je     0x2e231245d
+   2e23122bb:	mov    0x5d96(%rip),%rax        # 0x2e2318058
+   2e23122c2:	lea    (%rdi,%rdi,4),%rdi
+   2e23122c6:	shl    $0x3,%rdi
+   2e23122ca:	add    %rdi,%rax
+   2e23122cd:	mov    %rbp,0x20(%rax)
+   2e23122d1:	movl   $0x0,(%rax)
+   2e23122d7:	call   0x2e2312c20
+   2e23122dc:	mov    0xc(%rbp),%ecx
+   2e23122df:	lea    0x20(%rsp),%rdx
+   2e23122e4:	mov    $0x30,%r8d
+   2e23122ea:	add    %rax,%rcx
+   2e23122ed:	mov    0x5d64(%rip),%rax        # 0x2e2318058
+   2e23122f4:	mov    %rcx,0x18(%rax,%rdi,1)
+   2e23122f9:	call   *0x7e65(%rip)        # 0x2e231a164
+   2e23122ff:	test   %rax,%rax
+   2e2312302:	je     0x2e2312442
+   2e2312308:	mov    0x44(%rsp),%eax
+   2e231230c:	lea    -0x40(%rax),%edx
+   2e231230f:	and    $0xffffffbf,%edx
+   2e2312312:	je     0x2e2312320
+   2e2312314:	lea    -0x4(%rax),%edx
+   2e2312317:	and    $0xfffffffb,%edx
+   2e231231a:	jne    0x2e23123b0
+   2e2312320:	addl   $0x1,0x5d2d(%rip)        # 0x2e2318054
+   2e2312327:	cmp    $0x8,%ebx
+   2e231232a:	jae    0x2e2312358
+   2e231232c:	test   $0x4,%bl
+   2e231232f:	jne    0x2e2312410
+   2e2312335:	test   %ebx,%ebx
+   2e2312337:	je     0x2e2312349
+   2e2312339:	movzbl (%rsi),%eax
+   2e231233c:	mov    %al,(%r12)
+   2e2312340:	test   $0x2,%bl
+   2e2312343:	jne    0x2e2312430
+   2e2312349:	add    $0x50,%rsp
+   2e231234d:	pop    %rbx
+   2e231234e:	pop    %rsi
+   2e231234f:	pop    %rdi
+   2e2312350:	pop    %rbp
+   2e2312351:	pop    %r12
+   2e2312353:	ret
+   2e2312354:	nopl   0x0(%rax)
+   2e2312358:	mov    (%rsi),%rax
+   2e231235b:	lea    0x8(%r12),%rcx
+   2e2312360:	and    $0xfffffffffffffff8,%rcx
+   2e2312364:	mov    %rax,(%r12)
+   2e2312368:	mov    %ebx,%eax
+   2e231236a:	mov    -0x8(%rsi,%rax,1),%rdx
+   2e231236f:	mov    %rdx,-0x8(%r12,%rax,1)
+   2e2312374:	sub    %rcx,%r12
+   2e2312377:	add    %r12d,%ebx
+   2e231237a:	sub    %r12,%rsi
+   2e231237d:	and    $0xfffffff8,%ebx
+   2e2312380:	cmp    $0x8,%ebx
+   2e2312383:	jb     0x2e2312349
+   2e2312385:	and    $0xfffffff8,%ebx
+   2e2312388:	xor    %eax,%eax
+   2e231238a:	mov    %eax,%edx
+   2e231238c:	add    $0x8,%eax
+   2e231238f:	mov    (%rsi,%rdx,1),%r8
+   2e2312393:	mov    %r8,(%rcx,%rdx,1)
+   2e2312397:	cmp    %ebx,%eax
+   2e2312399:	jb     0x2e231238a
+   2e231239b:	add    $0x50,%rsp
+   2e231239f:	pop    %rbx
+   2e23123a0:	pop    %rsi
+   2e23123a1:	pop    %rdi
+   2e23123a2:	pop    %rbp
+   2e23123a3:	pop    %r12
+   2e23123a5:	ret
+   2e23123a6:	cs nopw 0x0(%rax,%rax,1)
+   2e23123b0:	cmp    $0x2,%eax
+   2e23123b3:	mov    0x20(%rsp),%rcx
+   2e23123b8:	mov    0x38(%rsp),%rdx
+   2e23123bd:	mov    $0x4,%r8d
+   2e23123c3:	mov    $0x40,%eax
+   2e23123c8:	cmovne %eax,%r8d
+   2e23123cc:	add    0x5c85(%rip),%rdi        # 0x2e2318058
+   2e23123d3:	mov    %rcx,0x8(%rdi)
+   2e23123d7:	mov    %rdi,%r9
+   2e23123da:	mov    %rdx,0x10(%rdi)
+   2e23123de:	call   *0x7d78(%rip)        # 0x2e231a15c
+   2e23123e4:	test   %eax,%eax
+   2e23123e6:	jne    0x2e2312320
+   2e23123ec:	call   *0x7d42(%rip)        # 0x2e231a134
+   2e23123f2:	lea    0x2cff(%rip),%rcx        # 0x2e23150f8
+   2e23123f9:	mov    %eax,%edx
+   2e23123fb:	call   0x2e23121e0
+   2e2312400:	xor    %edi,%edi
+   2e2312402:	jmp    0x2e23122a7
+   2e2312407:	nopw   0x0(%rax,%rax,1)
+   2e2312410:	mov    (%rsi),%eax
+   2e2312412:	mov    %ebx,%ebx
+   2e2312414:	mov    %eax,(%r12)
+   2e2312418:	mov    -0x4(%rsi,%rbx,1),%eax
+   2e231241c:	mov    %eax,-0x4(%r12,%rbx,1)
+   2e2312421:	jmp    0x2e2312349
+   2e2312426:	cs nopw 0x0(%rax,%rax,1)
+   2e2312430:	mov    %ebx,%ebx
+   2e2312432:	movzwl -0x2(%rsi,%rbx,1),%eax
+   2e2312437:	mov    %ax,-0x2(%r12,%rbx,1)
+   2e231243d:	jmp    0x2e2312349
+   2e2312442:	mov    0x5c0f(%rip),%rax        # 0x2e2318058
+   2e2312449:	mov    0x8(%rbp),%edx
+   2e231244c:	lea    0x2c6d(%rip),%rcx        # 0x2e23150c0
+   2e2312453:	mov    0x18(%rax,%rdi,1),%r8
+   2e2312458:	call   0x2e23121e0
+   2e231245d:	mov    %r12,%rdx
+   2e2312460:	lea    0x2c39(%rip),%rcx        # 0x2e23150a0
+   2e2312467:	call   0x2e23121e0
+   2e231246c:	nop
+   2e231246d:	nopl   (%rax)
+   2e2312470:	push   %rbp
+   2e2312471:	push   %r15
+   2e2312473:	push   %r14
+   2e2312475:	push   %r13
+   2e2312477:	push   %r12
+   2e2312479:	push   %rdi
+   2e231247a:	push   %rsi
+   2e231247b:	push   %rbx
+   2e231247c:	sub    $0x38,%rsp
+   2e2312480:	lea    0x80(%rsp),%rbp
+   2e2312488:	mov    0x5bc2(%rip),%esi        # 0x2e2318050
+   2e231248e:	test   %esi,%esi
+   2e2312490:	je     0x2e23124a8
+   2e2312492:	lea    -0x48(%rbp),%rsp
+   2e2312496:	pop    %rbx
+   2e2312497:	pop    %rsi
+   2e2312498:	pop    %rdi
+   2e2312499:	pop    %r12
+   2e231249b:	pop    %r13
+   2e231249d:	pop    %r14
+   2e231249f:	pop    %r15
+   2e23124a1:	pop    %rbp
+   2e23124a2:	ret
+   2e23124a3:	nopl   0x0(%rax,%rax,1)
+   2e23124a8:	movl   $0x1,0x5b9e(%rip)        # 0x2e2318050
+   2e23124b2:	call   0x2e2312b80
+   2e23124b7:	cltq
+   2e23124b9:	lea    (%rax,%rax,4),%rax
+   2e23124bd:	lea    0xf(,%rax,8),%rax
+   2e23124c5:	and    $0xfffffffffffffff0,%rax
+   2e23124c9:	call   0x2e2312db0
+   2e23124ce:	mov    0x2d0b(%rip),%r12        # 0x2e23151e0
+   2e23124d5:	mov    0x2d14(%rip),%rbx        # 0x2e23151f0
+   2e23124dc:	movl   $0x0,0x5b6e(%rip)        # 0x2e2318054
+   2e23124e6:	sub    %rax,%rsp
+   2e23124e9:	lea    0x20(%rsp),%rax
+   2e23124ee:	mov    %rax,0x5b63(%rip)        # 0x2e2318058
+   2e23124f5:	mov    %r12,%rax
+   2e23124f8:	sub    %rbx,%rax
+   2e23124fb:	cmp    $0x7,%rax
+   2e23124ff:	jle    0x2e2312492
+   2e2312501:	mov    (%rbx),%edx
+   2e2312503:	cmp    $0xb,%rax
+   2e2312507:	jg     0x2e2312658
+   2e231250d:	test   %edx,%edx
+   2e231250f:	jne    0x2e23126e0
+   2e2312515:	mov    0x4(%rbx),%eax
+   2e2312518:	test   %eax,%eax
+   2e231251a:	jne    0x2e23126e0
+   2e2312520:	mov    0x8(%rbx),%edx
+   2e2312523:	cmp    $0x1,%edx
+   2e2312526:	jne    0x2e2312748
+   2e231252c:	add    $0xc,%rbx
+   2e2312530:	lea    -0x58(%rbp),%r15
+   2e2312534:	mov    0x2cd5(%rip),%r13        # 0x2e2315210
+   2e231253b:	movabs $0xffffffff00000000,%r14
+   2e2312545:	cmp    %r12,%rbx
+   2e2312548:	jb     0x2e2312589
+   2e231254a:	jmp    0x2e2312492
+   2e231254f:	nop
+   2e2312550:	movzbl (%rcx),%r8d
+   2e2312554:	mov    %r15,%rdi
+   2e2312557:	mov    %r8,%r10
+   2e231255a:	or     $0xffffffffffffff00,%r10
+   2e2312561:	test   %r8b,%r8b
+   2e2312564:	cmovs  %r10,%r8
+   2e2312568:	sub    %rdx,%r8
+   2e231256b:	mov    %r15,%rdx
+   2e231256e:	add    %r9,%r8
+   2e2312571:	mov    %r8,-0x58(%rbp)
+   2e2312575:	mov    $0x1,%r8d
+   2e231257b:	call   0x2e2312250
+   2e2312580:	add    $0xc,%rbx
+   2e2312584:	cmp    %r12,%rbx
+   2e2312587:	jae    0x2e2312600
+   2e2312589:	mov    (%rbx),%edx
+   2e231258b:	mov    0x4(%rbx),%ecx
+   2e231258e:	movzbl 0x8(%rbx),%r8d
+   2e2312593:	add    %r13,%rdx
+   2e2312596:	add    %r13,%rcx
+   2e2312599:	mov    (%rdx),%r9
+   2e231259c:	cmp    $0x20,%r8d
+   2e23125a0:	je     0x2e23126b0
+   2e23125a6:	ja     0x2e2312680
+   2e23125ac:	cmp    $0x8,%r8d
+   2e23125b0:	je     0x2e2312550
+   2e23125b2:	cmp    $0x10,%r8d
+   2e23125b6:	jne    0x2e2312731
+   2e23125bc:	movzwl (%rcx),%r8d
+   2e23125c0:	mov    %r15,%rdi
+   2e23125c3:	mov    %r8,%r10
+   2e23125c6:	or     $0xffffffffffff0000,%r10
+   2e23125cd:	test   %r8w,%r8w
+   2e23125d1:	cmovs  %r10,%r8
+   2e23125d5:	add    $0xc,%rbx
+   2e23125d9:	sub    %rdx,%r8
+   2e23125dc:	mov    %r15,%rdx
+   2e23125df:	add    %r9,%r8
+   2e23125e2:	mov    %r8,-0x58(%rbp)
+   2e23125e6:	mov    $0x2,%r8d
+   2e23125ec:	call   0x2e2312250
+   2e23125f1:	cmp    %r12,%rbx
+   2e23125f4:	jb     0x2e2312589
+   2e23125f6:	cs nopw 0x0(%rax,%rax,1)
+   2e2312600:	mov    0x5a4e(%rip),%eax        # 0x2e2318054
+   2e2312606:	test   %eax,%eax
+   2e2312608:	jle    0x2e2312492
+   2e231260e:	mov    0x7b47(%rip),%r12        # 0x2e231a15c
+   2e2312615:	xor    %ebx,%ebx
+   2e2312617:	nopw   0x0(%rax,%rax,1)
+   2e2312620:	mov    0x5a31(%rip),%rax        # 0x2e2318058
+   2e2312627:	add    %rbx,%rax
+   2e231262a:	mov    (%rax),%r8d
+   2e231262d:	test   %r8d,%r8d
+   2e2312630:	je     0x2e2312640
+   2e2312632:	mov    0x10(%rax),%rdx
+   2e2312636:	mov    0x8(%rax),%rcx
+   2e231263a:	mov    %rdi,%r9
+   2e231263d:	call   *%r12
+   2e2312640:	add    $0x1,%esi
+   2e2312643:	add    $0x28,%rbx
+   2e2312647:	cmp    0x5a07(%rip),%esi        # 0x2e2318054
+   2e231264d:	jl     0x2e2312620
+   2e231264f:	jmp    0x2e2312492
+   2e2312654:	nopl   0x0(%rax)
+   2e2312658:	test   %edx,%edx
+   2e231265a:	jne    0x2e23126e0
+   2e2312660:	mov    0x4(%rbx),%eax
+   2e2312663:	mov    %eax,%edi
+   2e2312665:	or     0x8(%rbx),%edi
+   2e2312668:	jne    0x2e2312518
+   2e231266e:	mov    0xc(%rbx),%edx
+   2e2312671:	add    $0xc,%rbx
+   2e2312675:	jmp    0x2e231250d
+   2e231267a:	nopw   0x0(%rax,%rax,1)
+   2e2312680:	cmp    $0x40,%r8d
+   2e2312684:	jne    0x2e2312731
+   2e231268a:	mov    (%rcx),%rax
+   2e231268d:	mov    $0x8,%r8d
+   2e2312693:	mov    %r15,%rdi
+   2e2312696:	sub    %rdx,%rax
+   2e2312699:	mov    %r15,%rdx
+   2e231269c:	add    %r9,%rax
+   2e231269f:	mov    %rax,-0x58(%rbp)
+   2e23126a3:	call   0x2e2312250
+   2e23126a8:	jmp    0x2e2312580
+   2e23126ad:	nopl   (%rax)
+   2e23126b0:	mov    (%rcx),%eax
+   2e23126b2:	mov    %r15,%rdi
+   2e23126b5:	mov    %rax,%r8
+   2e23126b8:	or     %r14,%rax
+   2e23126bb:	test   %r8d,%r8d
+   2e23126be:	cmovns %r8,%rax
+   2e23126c2:	mov    $0x4,%r8d
+   2e23126c8:	sub    %rdx,%rax
+   2e23126cb:	mov    %r15,%rdx
+   2e23126ce:	add    %r9,%rax
+   2e23126d1:	mov    %rax,-0x58(%rbp)
+   2e23126d5:	call   0x2e2312250
+   2e23126da:	jmp    0x2e2312580
+   2e23126df:	nop
+   2e23126e0:	cmp    %r12,%rbx
+   2e23126e3:	jae    0x2e2312492
+   2e23126e9:	sub    $0x1,%r12
+   2e23126ed:	mov    0x2b1c(%rip),%r13        # 0x2e2315210
+   2e23126f4:	lea    -0x58(%rbp),%rdi
+   2e23126f8:	sub    %rbx,%r12
+   2e23126fb:	shr    $0x3,%r12
+   2e23126ff:	lea    0x8(%rbx,%r12,8),%r12
+   2e2312704:	nopl   0x0(%rax)
+   2e2312708:	mov    0x4(%rbx),%ecx
+   2e231270b:	mov    (%rbx),%eax
+   2e231270d:	mov    $0x4,%r8d
+   2e2312713:	mov    %rdi,%rdx
+   2e2312716:	add    $0x8,%rbx
+   2e231271a:	add    %r13,%rcx
+   2e231271d:	add    (%rcx),%eax
+   2e231271f:	mov    %eax,-0x58(%rbp)
+   2e2312722:	call   0x2e2312250
+   2e2312727:	cmp    %r12,%rbx
+   2e231272a:	jne    0x2e2312708
+   2e231272c:	jmp    0x2e2312600
+   2e2312731:	mov    %r8d,%edx
+   2e2312734:	lea    0x2a1d(%rip),%rcx        # 0x2e2315158
+   2e231273b:	movq   $0x0,-0x58(%rbp)
+   2e2312743:	call   0x2e23121e0
+   2e2312748:	lea    0x29d1(%rip),%rcx        # 0x2e2315120
+   2e231274f:	call   0x2e23121e0
+   2e2312754:	nop
+   2e2312755:	nop
+   2e2312756:	nop
+   2e2312757:	nop
+   2e2312758:	nop
+   2e2312759:	nop
+   2e231275a:	nop
+   2e231275b:	nop
+   2e231275c:	nop
+   2e231275d:	nop
+   2e231275e:	nop
+   2e231275f:	nop
+   2e2312760:	push   %r12
+   2e2312762:	push   %rdi
+   2e2312763:	push   %rsi
+   2e2312764:	push   %rbx
+   2e2312765:	sub    $0x28,%rsp
+   2e2312769:	lea    0x5910(%rip),%rcx        # 0x2e2318080
+   2e2312770:	call   *0x79b6(%rip)        # 0x2e231a12c
+   2e2312776:	mov    0x58e3(%rip),%rbx        # 0x2e2318060
+   2e231277d:	test   %rbx,%rbx
+   2e2312780:	je     0x2e23127b4
+   2e2312782:	mov    0x79cb(%rip),%rdi        # 0x2e231a154
+   2e2312789:	mov    0x79a4(%rip),%rsi        # 0x2e231a134
+   2e2312790:	mov    (%rbx),%ecx
+   2e2312792:	call   *%rdi
+   2e2312794:	mov    %rax,%r12
+   2e2312797:	call   *%rsi
+   2e2312799:	test   %eax,%eax
+   2e231279b:	jne    0x2e23127ab
+   2e231279d:	test   %r12,%r12
+   2e23127a0:	je     0x2e23127ab
+   2e23127a2:	mov    0x8(%rbx),%rax
+   2e23127a6:	mov    %r12,%rcx
+   2e23127a9:	call   *%rax
+   2e23127ab:	mov    0x10(%rbx),%rbx
+   2e23127af:	test   %rbx,%rbx
+   2e23127b2:	jne    0x2e2312790
+   2e23127b4:	lea    0x58c5(%rip),%rcx        # 0x2e2318080
+   2e23127bb:	add    $0x28,%rsp
+   2e23127bf:	pop    %rbx
+   2e23127c0:	pop    %rsi
+   2e23127c1:	pop    %rdi
+   2e23127c2:	pop    %r12
+   2e23127c4:	rex.W jmp *0x7979(%rip)        # 0x2e231a144
+   2e23127cb:	nopl   0x0(%rax,%rax,1)
+   2e23127d0:	push   %rdi
+   2e23127d1:	push   %rsi
+   2e23127d2:	push   %rbx
+   2e23127d3:	sub    $0x20,%rsp
+   2e23127d7:	mov    0x588b(%rip),%eax        # 0x2e2318068
+   2e23127dd:	mov    %ecx,%edi
+   2e23127df:	mov    %rdx,%rsi
+   2e23127e2:	test   %eax,%eax
+   2e23127e4:	jne    0x2e23127f0
+   2e23127e6:	add    $0x20,%rsp
+   2e23127ea:	pop    %rbx
+   2e23127eb:	pop    %rsi
+   2e23127ec:	pop    %rdi
+   2e23127ed:	ret
+   2e23127ee:	xchg   %ax,%ax
+   2e23127f0:	mov    $0x18,%edx
+   2e23127f5:	mov    $0x1,%ecx
+   2e23127fa:	call   0x2e2312f90
+   2e23127ff:	mov    %rax,%rbx
+   2e2312802:	test   %rax,%rax
+   2e2312805:	je     0x2e2312843
+   2e2312807:	mov    %edi,(%rax)
+   2e2312809:	lea    0x5870(%rip),%rcx        # 0x2e2318080
+   2e2312810:	mov    %rsi,0x8(%rax)
+   2e2312814:	call   *0x7912(%rip)        # 0x2e231a12c
+   2e231281a:	mov    0x583f(%rip),%rax        # 0x2e2318060
+   2e2312821:	lea    0x5858(%rip),%rcx        # 0x2e2318080
+   2e2312828:	mov    %rbx,0x5831(%rip)        # 0x2e2318060
+   2e231282f:	mov    %rax,0x10(%rbx)
+   2e2312833:	call   *0x790b(%rip)        # 0x2e231a144
+   2e2312839:	xor    %eax,%eax
+   2e231283b:	add    $0x20,%rsp
+   2e231283f:	pop    %rbx
+   2e2312840:	pop    %rsi
+   2e2312841:	pop    %rdi
+   2e2312842:	ret
+   2e2312843:	or     $0xffffffff,%eax
+   2e2312846:	jmp    0x2e23127e6
+   2e2312848:	nopl   0x0(%rax,%rax,1)
+   2e2312850:	push   %rbx
+   2e2312851:	sub    $0x20,%rsp
+   2e2312855:	mov    0x580d(%rip),%eax        # 0x2e2318068
+   2e231285b:	mov    %ecx,%ebx
+   2e231285d:	test   %eax,%eax
+   2e231285f:	jne    0x2e2312870
+   2e2312861:	xor    %eax,%eax
+   2e2312863:	add    $0x20,%rsp
+   2e2312867:	pop    %rbx
+   2e2312868:	ret
+   2e2312869:	nopl   0x0(%rax)
+   2e2312870:	lea    0x5809(%rip),%rcx        # 0x2e2318080
+   2e2312877:	call   *0x78af(%rip)        # 0x2e231a12c
+   2e231287d:	mov    0x57dc(%rip),%rcx        # 0x2e2318060
+   2e2312884:	test   %rcx,%rcx
+   2e2312887:	je     0x2e23128b3
+   2e2312889:	xor    %edx,%edx
+   2e231288b:	jmp    0x2e231289b
+   2e231288d:	nopl   (%rax)
+   2e2312890:	mov    %rcx,%rdx
+   2e2312893:	test   %rax,%rax
+   2e2312896:	je     0x2e23128b3
+   2e2312898:	mov    %rax,%rcx
+   2e231289b:	mov    (%rcx),%eax
+   2e231289d:	cmp    %ebx,%eax
+   2e231289f:	mov    0x10(%rcx),%rax
+   2e23128a3:	jne    0x2e2312890
+   2e23128a5:	test   %rdx,%rdx
+   2e23128a8:	je     0x2e23128d0
+   2e23128aa:	mov    %rax,0x10(%rdx)
+   2e23128ae:	call   0x2e2312f88
+   2e23128b3:	lea    0x57c6(%rip),%rcx        # 0x2e2318080
+   2e23128ba:	call   *0x7884(%rip)        # 0x2e231a144
+   2e23128c0:	xor    %eax,%eax
+   2e23128c2:	add    $0x20,%rsp
+   2e23128c6:	pop    %rbx
+   2e23128c7:	ret
+   2e23128c8:	nopl   0x0(%rax,%rax,1)
+   2e23128d0:	mov    %rax,0x5789(%rip)        # 0x2e2318060
+   2e23128d7:	jmp    0x2e23128ae
+   2e23128d9:	nopl   0x0(%rax)
+   2e23128e0:	push   %rbx
+   2e23128e1:	sub    $0x20,%rsp
+   2e23128e5:	cmp    $0x2,%edx
+   2e23128e8:	je     0x2e23129b0
+   2e23128ee:	ja     0x2e2312918
+   2e23128f0:	test   %edx,%edx
+   2e23128f2:	je     0x2e2312940
+   2e23128f4:	mov    0x576e(%rip),%eax        # 0x2e2318068
+   2e23128fa:	test   %eax,%eax
+   2e23128fc:	je     0x2e2312930
+   2e23128fe:	movl   $0x1,0x5760(%rip)        # 0x2e2318068
+   2e2312908:	mov    $0x1,%eax
+   2e231290d:	add    $0x20,%rsp
+   2e2312911:	pop    %rbx
+   2e2312912:	ret
+   2e2312913:	nopl   0x0(%rax,%rax,1)
+   2e2312918:	cmp    $0x3,%edx
+   2e231291b:	jne    0x2e2312908
+   2e231291d:	mov    0x5745(%rip),%eax        # 0x2e2318068
+   2e2312923:	test   %eax,%eax
+   2e2312925:	je     0x2e2312908
+   2e2312927:	call   0x2e2312760
+   2e231292c:	jmp    0x2e2312908
+   2e231292e:	xchg   %ax,%ax
+   2e2312930:	lea    0x5749(%rip),%rcx        # 0x2e2318080
+   2e2312937:	call   *0x77ff(%rip)        # 0x2e231a13c
+   2e231293d:	jmp    0x2e23128fe
+   2e231293f:	nop
+   2e2312940:	mov    0x5722(%rip),%eax        # 0x2e2318068
+   2e2312946:	test   %eax,%eax
+   2e2312948:	je     0x2e231294f
+   2e231294a:	call   0x2e2312760
+   2e231294f:	mov    0x5713(%rip),%eax        # 0x2e2318068
+   2e2312955:	cmp    $0x1,%eax
+   2e2312958:	jne    0x2e2312908
+   2e231295a:	mov    0x56ff(%rip),%rbx        # 0x2e2318060
+   2e2312961:	test   %rbx,%rbx
+   2e2312964:	je     0x2e2312981
+   2e2312966:	cs nopw 0x0(%rax,%rax,1)
+   2e2312970:	mov    %rbx,%rcx
+   2e2312973:	mov    0x10(%rbx),%rbx
+   2e2312977:	call   0x2e2312f88
+   2e231297c:	test   %rbx,%rbx
+   2e231297f:	jne    0x2e2312970
+   2e2312981:	lea    0x56f8(%rip),%rcx        # 0x2e2318080
+   2e2312988:	movq   $0x0,0x56cd(%rip)        # 0x2e2318060
+   2e2312993:	movl   $0x0,0x56cb(%rip)        # 0x2e2318068
+   2e231299d:	call   *0x7781(%rip)        # 0x2e231a124
+   2e23129a3:	jmp    0x2e2312908
+   2e23129a8:	nopl   0x0(%rax,%rax,1)
+   2e23129b0:	call   0x2e2312da0
+   2e23129b5:	mov    $0x1,%eax
+   2e23129ba:	add    $0x20,%rsp
+   2e23129be:	pop    %rbx
+   2e23129bf:	ret
    2e23129c0:	movslq 0x3c(%rcx),%rax
-   2e23129c4:	add    %rax,%rcx
-   2e23129c7:	movzwl 0x14(%rcx),%eax
-   2e23129cb:	lea    0x18(%rcx,%rax,1),%rax
-   2e23129d0:	movzwl 0x6(%rcx),%ecx
-   2e23129d4:	test   %ecx,%ecx
-   2e23129d6:	je     0x2e2312a05
-   2e23129d8:	sub    $0x1,%ecx
-   2e23129db:	lea    (%rcx,%rcx,4),%rcx
-   2e23129df:	lea    0x28(%rax,%rcx,8),%r9
-   2e23129e4:	nopl   0x0(%rax)
-   2e23129e8:	mov    0xc(%rax),%r8d
-   2e23129ec:	mov    %r8,%rcx
-   2e23129ef:	cmp    %rdx,%r8
-   2e23129f2:	ja     0x2e23129fc
-   2e23129f4:	add    0x8(%rax),%ecx
-   2e23129f7:	cmp    %rdx,%rcx
-   2e23129fa:	ja     0x2e2312a07
-   2e23129fc:	add    $0x28,%rax
-   2e2312a00:	cmp    %r9,%rax
-   2e2312a03:	jne    0x2e23129e8
-   2e2312a05:	xor    %eax,%eax
-   2e2312a07:	ret
-   2e2312a08:	nopl   0x0(%rax,%rax,1)
-   2e2312a10:	push   %r12
-   2e2312a12:	push   %rsi
-   2e2312a13:	push   %rbx
-   2e2312a14:	sub    $0x20,%rsp
-   2e2312a18:	mov    %rcx,%rbx
-   2e2312a1b:	call   0x2e2312f20
-   2e2312a20:	cmp    $0x8,%rax
-   2e2312a24:	ja     0x2e2312aa0
-   2e2312a26:	mov    0x27e3(%rip),%rcx        # 0x2e2315210
-   2e2312a2d:	xor    %r12d,%r12d
-   2e2312a30:	cmpw   $0x5a4d,(%rcx)
-   2e2312a35:	jne    0x2e2312a8e
-   2e2312a37:	call   0x2e2312980
-   2e2312a3c:	test   %eax,%eax
-   2e2312a3e:	je     0x2e2312a8e
-   2e2312a40:	movslq 0x3c(%rcx),%rax
-   2e2312a44:	add    %rax,%rcx
-   2e2312a47:	movzwl 0x14(%rcx),%eax
-   2e2312a4b:	lea    0x18(%rcx,%rax,1),%r12
-   2e2312a50:	movzwl 0x6(%rcx),%eax
-   2e2312a54:	test   %eax,%eax
-   2e2312a56:	je     0x2e2312aa0
-   2e2312a58:	sub    $0x1,%eax
-   2e2312a5b:	lea    (%rax,%rax,4),%rax
-   2e2312a5f:	lea    0x28(%r12,%rax,8),%rsi
-   2e2312a64:	jmp    0x2e2312a79
-   2e2312a66:	cs nopw 0x0(%rax,%rax,1)
-   2e2312a70:	add    $0x28,%r12
-   2e2312a74:	cmp    %rsi,%r12
-   2e2312a77:	je     0x2e2312aa0
-   2e2312a79:	mov    $0x8,%r8d
-   2e2312a7f:	mov    %rbx,%rdx
-   2e2312a82:	mov    %r12,%rcx
-   2e2312a85:	call   0x2e2312f18
-   2e2312a8a:	test   %eax,%eax
-   2e2312a8c:	jne    0x2e2312a70
-   2e2312a8e:	mov    %r12,%rax
-   2e2312a91:	add    $0x20,%rsp
-   2e2312a95:	pop    %rbx
-   2e2312a96:	pop    %rsi
-   2e2312a97:	pop    %r12
-   2e2312a99:	ret
-   2e2312a9a:	nopw   0x0(%rax,%rax,1)
-   2e2312aa0:	xor    %r12d,%r12d
-   2e2312aa3:	mov    %r12,%rax
-   2e2312aa6:	add    $0x20,%rsp
-   2e2312aaa:	pop    %rbx
-   2e2312aab:	pop    %rsi
-   2e2312aac:	pop    %r12
-   2e2312aae:	ret
-   2e2312aaf:	nop
-   2e2312ab0:	sub    $0x28,%rsp
-   2e2312ab4:	mov    0x2755(%rip),%r10        # 0x2e2315210
-   2e2312abb:	xor    %r8d,%r8d
-   2e2312abe:	cmpw   $0x5a4d,(%r10)
-   2e2312ac4:	mov    %rcx,%r9
-   2e2312ac7:	jne    0x2e2312b29
-   2e2312ac9:	mov    %r10,%rcx
-   2e2312acc:	call   0x2e2312980
-   2e2312ad1:	test   %eax,%eax
-   2e2312ad3:	je     0x2e2312b29
-   2e2312ad5:	movslq 0x3c(%r10),%rax
-   2e2312ad9:	mov    %r9,%rcx
-   2e2312adc:	sub    %r10,%rcx
-   2e2312adf:	add    %rax,%r10
-   2e2312ae2:	movzwl 0x14(%r10),%eax
-   2e2312ae7:	lea    0x18(%r10,%rax,1),%r8
-   2e2312aec:	movzwl 0x6(%r10),%eax
-   2e2312af1:	test   %eax,%eax
-   2e2312af3:	je     0x2e2312b26
-   2e2312af5:	sub    $0x1,%eax
-   2e2312af8:	lea    (%rax,%rax,4),%rax
-   2e2312afc:	lea    0x28(%r8,%rax,8),%r9
-   2e2312b01:	nopl   0x0(%rax)
-   2e2312b08:	mov    0xc(%r8),%edx
-   2e2312b0c:	mov    %rdx,%rax
-   2e2312b0f:	cmp    %rdx,%rcx
-   2e2312b12:	jb     0x2e2312b1d
-   2e2312b14:	add    0x8(%r8),%eax
-   2e2312b18:	cmp    %rax,%rcx
-   2e2312b1b:	jb     0x2e2312b29
-   2e2312b1d:	add    $0x28,%r8
-   2e2312b21:	cmp    %r9,%r8
-   2e2312b24:	jne    0x2e2312b08
-   2e2312b26:	xor    %r8d,%r8d
-   2e2312b29:	mov    %r8,%rax
-   2e2312b2c:	add    $0x28,%rsp
-   2e2312b30:	ret
-   2e2312b31:	data16 cs nopw 0x0(%rax,%rax,1)
-   2e2312b3c:	nopl   0x0(%rax)
-   2e2312b40:	sub    $0x28,%rsp
-   2e2312b44:	mov    0x26c5(%rip),%rcx        # 0x2e2315210
-   2e2312b4b:	xor    %eax,%eax
-   2e2312b4d:	cmpw   $0x5a4d,(%rcx)
-   2e2312b52:	jne    0x2e2312b66
-   2e2312b54:	call   0x2e2312980
-   2e2312b59:	test   %eax,%eax
-   2e2312b5b:	je     0x2e2312b66
-   2e2312b5d:	movslq 0x3c(%rcx),%rax
-   2e2312b61:	movzwl 0x6(%rax,%rcx,1),%eax
-   2e2312b66:	add    $0x28,%rsp
-   2e2312b6a:	ret
-   2e2312b6b:	nopl   0x0(%rax,%rax,1)
-   2e2312b70:	sub    $0x28,%rsp
-   2e2312b74:	xor    %r8d,%r8d
-   2e2312b77:	mov    %rcx,%r9
-   2e2312b7a:	mov    0x268f(%rip),%rcx        # 0x2e2315210
-   2e2312b81:	cmpw   $0x5a4d,(%rcx)
-   2e2312b86:	jne    0x2e2312bd4
-   2e2312b88:	call   0x2e2312980
-   2e2312b8d:	test   %eax,%eax
-   2e2312b8f:	je     0x2e2312bd4
-   2e2312b91:	movslq 0x3c(%rcx),%rax
-   2e2312b95:	add    %rax,%rcx
-   2e2312b98:	movzwl 0x14(%rcx),%eax
-   2e2312b9c:	lea    0x18(%rcx,%rax,1),%r8
-   2e2312ba1:	movzwl 0x6(%rcx),%eax
-   2e2312ba5:	test   %eax,%eax
-   2e2312ba7:	je     0x2e2312bd1
-   2e2312ba9:	sub    $0x1,%eax
-   2e2312bac:	lea    (%rax,%rax,4),%rax
-   2e2312bb0:	lea    0x28(%r8,%rax,8),%rax
-   2e2312bb5:	nopl   (%rax)
-   2e2312bb8:	testb  $0x20,0x27(%r8)
-   2e2312bbd:	je     0x2e2312bc8
-   2e2312bbf:	test   %r9,%r9
-   2e2312bc2:	je     0x2e2312bd4
-   2e2312bc4:	sub    $0x1,%r9
-   2e2312bc8:	add    $0x28,%r8
-   2e2312bcc:	cmp    %rax,%r8
-   2e2312bcf:	jne    0x2e2312bb8
-   2e2312bd1:	xor    %r8d,%r8d
-   2e2312bd4:	mov    %r8,%rax
-   2e2312bd7:	add    $0x28,%rsp
-   2e2312bdb:	ret
-   2e2312bdc:	nopl   0x0(%rax)
-   2e2312be0:	sub    $0x28,%rsp
-   2e2312be4:	mov    0x2625(%rip),%rcx        # 0x2e2315210
-   2e2312beb:	xor    %r8d,%r8d
-   2e2312bee:	cmpw   $0x5a4d,(%rcx)
-   2e2312bf3:	jne    0x2e2312c00
-   2e2312bf5:	call   0x2e2312980
-   2e2312bfa:	test   %eax,%eax
-   2e2312bfc:	cmovne %rcx,%r8
-   2e2312c00:	mov    %r8,%rax
-   2e2312c03:	add    $0x28,%rsp
-   2e2312c07:	ret
-   2e2312c08:	nopl   0x0(%rax,%rax,1)
-   2e2312c10:	sub    $0x28,%rsp
-   2e2312c14:	mov    0x25f5(%rip),%r9        # 0x2e2315210
-   2e2312c1b:	xor    %eax,%eax
-   2e2312c1d:	cmpw   $0x5a4d,(%r9)
-   2e2312c23:	mov    %rcx,%r8
-   2e2312c26:	jne    0x2e2312c7f
-   2e2312c28:	mov    %r9,%rcx
-   2e2312c2b:	call   0x2e2312980
-   2e2312c30:	test   %eax,%eax
-   2e2312c32:	je     0x2e2312c7f
-   2e2312c34:	movslq 0x3c(%r9),%rax
-   2e2312c38:	mov    %r8,%rcx
-   2e2312c3b:	sub    %r9,%rcx
-   2e2312c3e:	add    %rax,%r9
-   2e2312c41:	movzwl 0x14(%r9),%eax
-   2e2312c46:	movzwl 0x6(%r9),%edx
-   2e2312c4b:	lea    0x18(%r9,%rax,1),%rax
-   2e2312c50:	test   %edx,%edx
-   2e2312c52:	je     0x2e2312c7d
-   2e2312c54:	sub    $0x1,%edx
-   2e2312c57:	lea    (%rdx,%rdx,4),%rdx
-   2e2312c5b:	lea    0x28(%rax,%rdx,8),%r9
-   2e2312c60:	mov    0xc(%rax),%r8d
-   2e2312c64:	mov    %r8,%rdx
-   2e2312c67:	cmp    %r8,%rcx
-   2e2312c6a:	jb     0x2e2312c74
-   2e2312c6c:	add    0x8(%rax),%edx
-   2e2312c6f:	cmp    %rdx,%rcx
-   2e2312c72:	jb     0x2e2312c88
-   2e2312c74:	add    $0x28,%rax
-   2e2312c78:	cmp    %r9,%rax
-   2e2312c7b:	jne    0x2e2312c60
-   2e2312c7d:	xor    %eax,%eax
-   2e2312c7f:	add    $0x28,%rsp
-   2e2312c83:	ret
-   2e2312c84:	nopl   0x0(%rax)
-   2e2312c88:	mov    0x24(%rax),%eax
-   2e2312c8b:	not    %eax
-   2e2312c8d:	shr    $0x1f,%eax
-   2e2312c90:	add    $0x28,%rsp
-   2e2312c94:	ret
-   2e2312c95:	data16 cs nopw 0x0(%rax,%rax,1)
-   2e2312ca0:	sub    $0x28,%rsp
-   2e2312ca4:	mov    0x2565(%rip),%r11        # 0x2e2315210
-   2e2312cab:	xor    %r9d,%r9d
-   2e2312cae:	cmpw   $0x5a4d,(%r11)
-   2e2312cb4:	mov    %ecx,%r8d
-   2e2312cb7:	jne    0x2e2312d18
-   2e2312cb9:	mov    %r11,%rcx
-   2e2312cbc:	call   0x2e2312980
-   2e2312cc1:	test   %eax,%eax
-   2e2312cc3:	je     0x2e2312d18
-   2e2312cc5:	movslq 0x3c(%r11),%rcx
-   2e2312cc9:	add    %r11,%rcx
-   2e2312ccc:	mov    0x90(%rcx),%eax
-   2e2312cd2:	test   %eax,%eax
-   2e2312cd4:	je     0x2e2312d18
-   2e2312cd6:	movzwl 0x14(%rcx),%edx
-   2e2312cda:	lea    0x18(%rcx,%rdx,1),%rdx
-   2e2312cdf:	movzwl 0x6(%rcx),%ecx
-   2e2312ce3:	test   %ecx,%ecx
-   2e2312ce5:	je     0x2e2312d18
-   2e2312ce7:	sub    $0x1,%ecx
-   2e2312cea:	lea    (%rcx,%rcx,4),%rcx
-   2e2312cee:	lea    0x28(%rdx,%rcx,8),%r10
-   2e2312cf3:	nopl   0x0(%rax,%rax,1)
-   2e2312cf8:	mov    0xc(%rdx),%r9d
-   2e2312cfc:	mov    %r9,%rcx
-   2e2312cff:	cmp    %r9,%rax
-   2e2312d02:	jb     0x2e2312d0c
-   2e2312d04:	add    0x8(%rdx),%ecx
-   2e2312d07:	cmp    %rcx,%rax
-   2e2312d0a:	jb     0x2e2312d20
-   2e2312d0c:	add    $0x28,%rdx
-   2e2312d10:	cmp    %r10,%rdx
-   2e2312d13:	jne    0x2e2312cf8
-   2e2312d15:	xor    %r9d,%r9d
-   2e2312d18:	mov    %r9,%rax
-   2e2312d1b:	add    $0x28,%rsp
-   2e2312d1f:	ret
-   2e2312d20:	add    %r11,%rax
-   2e2312d23:	jmp    0x2e2312d30
-   2e2312d25:	nopl   (%rax)
-   2e2312d28:	sub    $0x1,%r8d
-   2e2312d2c:	add    $0x14,%rax
-   2e2312d30:	mov    0x4(%rax),%ecx
-   2e2312d33:	test   %ecx,%ecx
-   2e2312d35:	jne    0x2e2312d3e
-   2e2312d37:	mov    0xc(%rax),%edx
-   2e2312d3a:	test   %edx,%edx
-   2e2312d3c:	je     0x2e2312d15
-   2e2312d3e:	test   %r8d,%r8d
-   2e2312d41:	jg     0x2e2312d28
-   2e2312d43:	mov    0xc(%rax),%r9d
-   2e2312d47:	add    %r11,%r9
-   2e2312d4a:	mov    %r9,%rax
-   2e2312d4d:	add    $0x28,%rsp
-   2e2312d51:	ret
-   2e2312d52:	nop
-   2e2312d53:	nop
-   2e2312d54:	nop
-   2e2312d55:	nop
-   2e2312d56:	nop
-   2e2312d57:	nop
-   2e2312d58:	nop
-   2e2312d59:	nop
-   2e2312d5a:	nop
-   2e2312d5b:	nop
-   2e2312d5c:	nop
-   2e2312d5d:	nop
-   2e2312d5e:	nop
-   2e2312d5f:	nop
-   2e2312d60:	fninit
-   2e2312d62:	ret
-   2e2312d63:	nop
-   2e2312d64:	nop
-   2e2312d65:	nop
-   2e2312d66:	nop
-   2e2312d67:	nop
-   2e2312d68:	nop
-   2e2312d69:	nop
-   2e2312d6a:	nop
-   2e2312d6b:	nop
-   2e2312d6c:	nop
-   2e2312d6d:	nop
-   2e2312d6e:	nop
-   2e2312d6f:	nop
-   2e2312d70:	push   %rcx
-   2e2312d71:	push   %rax
-   2e2312d72:	cmp    $0x1000,%rax
-   2e2312d78:	lea    0x18(%rsp),%rcx
-   2e2312d7d:	jb     0x2e2312d98
-   2e2312d7f:	sub    $0x1000,%rcx
-   2e2312d86:	orq    $0x0,(%rcx)
-   2e2312d8a:	sub    $0x1000,%rax
-   2e2312d90:	cmp    $0x1000,%rax
-   2e2312d96:	ja     0x2e2312d7f
-   2e2312d98:	sub    %rax,%rcx
-   2e2312d9b:	orq    $0x0,(%rcx)
-   2e2312d9f:	pop    %rax
-   2e2312da0:	pop    %rcx
-   2e2312da1:	ret
-   2e2312da2:	nop
+   2e23129c4:	lea    (%rax,%rcx,1),%rdx
+   2e23129c8:	xor    %eax,%eax
+   2e23129ca:	cmpl   $0x4550,(%rdx)
+   2e23129d0:	jne    0x2e23129dd
+   2e23129d2:	xor    %eax,%eax
+   2e23129d4:	cmpw   $0x20b,0x18(%rdx)
+   2e23129da:	sete   %al
+   2e23129dd:	ret
+   2e23129de:	xchg   %ax,%ax
+   2e23129e0:	cmpw   $0x5a4d,(%rcx)
+   2e23129e5:	jne    0x2e23129f0
+   2e23129e7:	jmp    0x2e23129c0
+   2e23129e9:	nopl   0x0(%rax)
+   2e23129f0:	xor    %eax,%eax
+   2e23129f2:	ret
+   2e23129f3:	data16 cs nopw 0x0(%rax,%rax,1)
+   2e23129fe:	xchg   %ax,%ax
+   2e2312a00:	movslq 0x3c(%rcx),%rax
+   2e2312a04:	add    %rax,%rcx
+   2e2312a07:	movzwl 0x14(%rcx),%eax
+   2e2312a0b:	lea    0x18(%rcx,%rax,1),%rax
+   2e2312a10:	movzwl 0x6(%rcx),%ecx
+   2e2312a14:	test   %ecx,%ecx
+   2e2312a16:	je     0x2e2312a45
+   2e2312a18:	sub    $0x1,%ecx
+   2e2312a1b:	lea    (%rcx,%rcx,4),%rcx
+   2e2312a1f:	lea    0x28(%rax,%rcx,8),%r9
+   2e2312a24:	nopl   0x0(%rax)
+   2e2312a28:	mov    0xc(%rax),%r8d
+   2e2312a2c:	mov    %r8,%rcx
+   2e2312a2f:	cmp    %rdx,%r8
+   2e2312a32:	ja     0x2e2312a3c
+   2e2312a34:	add    0x8(%rax),%ecx
+   2e2312a37:	cmp    %rdx,%rcx
+   2e2312a3a:	ja     0x2e2312a47
+   2e2312a3c:	add    $0x28,%rax
+   2e2312a40:	cmp    %r9,%rax
+   2e2312a43:	jne    0x2e2312a28
+   2e2312a45:	xor    %eax,%eax
+   2e2312a47:	ret
+   2e2312a48:	nopl   0x0(%rax,%rax,1)
+   2e2312a50:	push   %r12
+   2e2312a52:	push   %rsi
+   2e2312a53:	push   %rbx
+   2e2312a54:	sub    $0x20,%rsp
+   2e2312a58:	mov    %rcx,%rbx
+   2e2312a5b:	call   0x2e2312f60
+   2e2312a60:	cmp    $0x8,%rax
+   2e2312a64:	ja     0x2e2312ae0
+   2e2312a66:	mov    0x27a3(%rip),%rcx        # 0x2e2315210
+   2e2312a6d:	xor    %r12d,%r12d
+   2e2312a70:	cmpw   $0x5a4d,(%rcx)
+   2e2312a75:	jne    0x2e2312ace
+   2e2312a77:	call   0x2e23129c0
+   2e2312a7c:	test   %eax,%eax
+   2e2312a7e:	je     0x2e2312ace
+   2e2312a80:	movslq 0x3c(%rcx),%rax
+   2e2312a84:	add    %rax,%rcx
+   2e2312a87:	movzwl 0x14(%rcx),%eax
+   2e2312a8b:	lea    0x18(%rcx,%rax,1),%r12
+   2e2312a90:	movzwl 0x6(%rcx),%eax
+   2e2312a94:	test   %eax,%eax
+   2e2312a96:	je     0x2e2312ae0
+   2e2312a98:	sub    $0x1,%eax
+   2e2312a9b:	lea    (%rax,%rax,4),%rax
+   2e2312a9f:	lea    0x28(%r12,%rax,8),%rsi
+   2e2312aa4:	jmp    0x2e2312ab9
+   2e2312aa6:	cs nopw 0x0(%rax,%rax,1)
+   2e2312ab0:	add    $0x28,%r12
+   2e2312ab4:	cmp    %rsi,%r12
+   2e2312ab7:	je     0x2e2312ae0
+   2e2312ab9:	mov    $0x8,%r8d
+   2e2312abf:	mov    %rbx,%rdx
+   2e2312ac2:	mov    %r12,%rcx
+   2e2312ac5:	call   0x2e2312f58
+   2e2312aca:	test   %eax,%eax
+   2e2312acc:	jne    0x2e2312ab0
+   2e2312ace:	mov    %r12,%rax
+   2e2312ad1:	add    $0x20,%rsp
+   2e2312ad5:	pop    %rbx
+   2e2312ad6:	pop    %rsi
+   2e2312ad7:	pop    %r12
+   2e2312ad9:	ret
+   2e2312ada:	nopw   0x0(%rax,%rax,1)
+   2e2312ae0:	xor    %r12d,%r12d
+   2e2312ae3:	mov    %r12,%rax
+   2e2312ae6:	add    $0x20,%rsp
+   2e2312aea:	pop    %rbx
+   2e2312aeb:	pop    %rsi
+   2e2312aec:	pop    %r12
+   2e2312aee:	ret
+   2e2312aef:	nop
+   2e2312af0:	sub    $0x28,%rsp
+   2e2312af4:	mov    0x2715(%rip),%r10        # 0x2e2315210
+   2e2312afb:	xor    %r8d,%r8d
+   2e2312afe:	cmpw   $0x5a4d,(%r10)
+   2e2312b04:	mov    %rcx,%r9
+   2e2312b07:	jne    0x2e2312b69
+   2e2312b09:	mov    %r10,%rcx
+   2e2312b0c:	call   0x2e23129c0
+   2e2312b11:	test   %eax,%eax
+   2e2312b13:	je     0x2e2312b69
+   2e2312b15:	movslq 0x3c(%r10),%rax
+   2e2312b19:	mov    %r9,%rcx
+   2e2312b1c:	sub    %r10,%rcx
+   2e2312b1f:	add    %rax,%r10
+   2e2312b22:	movzwl 0x14(%r10),%eax
+   2e2312b27:	lea    0x18(%r10,%rax,1),%r8
+   2e2312b2c:	movzwl 0x6(%r10),%eax
+   2e2312b31:	test   %eax,%eax
+   2e2312b33:	je     0x2e2312b66
+   2e2312b35:	sub    $0x1,%eax
+   2e2312b38:	lea    (%rax,%rax,4),%rax
+   2e2312b3c:	lea    0x28(%r8,%rax,8),%r9
+   2e2312b41:	nopl   0x0(%rax)
+   2e2312b48:	mov    0xc(%r8),%edx
+   2e2312b4c:	mov    %rdx,%rax
+   2e2312b4f:	cmp    %rdx,%rcx
+   2e2312b52:	jb     0x2e2312b5d
+   2e2312b54:	add    0x8(%r8),%eax
+   2e2312b58:	cmp    %rax,%rcx
+   2e2312b5b:	jb     0x2e2312b69
+   2e2312b5d:	add    $0x28,%r8
+   2e2312b61:	cmp    %r9,%r8
+   2e2312b64:	jne    0x2e2312b48
+   2e2312b66:	xor    %r8d,%r8d
+   2e2312b69:	mov    %r8,%rax
+   2e2312b6c:	add    $0x28,%rsp
+   2e2312b70:	ret
+   2e2312b71:	data16 cs nopw 0x0(%rax,%rax,1)
+   2e2312b7c:	nopl   0x0(%rax)
+   2e2312b80:	sub    $0x28,%rsp
+   2e2312b84:	mov    0x2685(%rip),%rcx        # 0x2e2315210
+   2e2312b8b:	xor    %eax,%eax
+   2e2312b8d:	cmpw   $0x5a4d,(%rcx)
+   2e2312b92:	jne    0x2e2312ba6
+   2e2312b94:	call   0x2e23129c0
+   2e2312b99:	test   %eax,%eax
+   2e2312b9b:	je     0x2e2312ba6
+   2e2312b9d:	movslq 0x3c(%rcx),%rax
+   2e2312ba1:	movzwl 0x6(%rax,%rcx,1),%eax
+   2e2312ba6:	add    $0x28,%rsp
+   2e2312baa:	ret
+   2e2312bab:	nopl   0x0(%rax,%rax,1)
+   2e2312bb0:	sub    $0x28,%rsp
+   2e2312bb4:	xor    %r8d,%r8d
+   2e2312bb7:	mov    %rcx,%r9
+   2e2312bba:	mov    0x264f(%rip),%rcx        # 0x2e2315210
+   2e2312bc1:	cmpw   $0x5a4d,(%rcx)
+   2e2312bc6:	jne    0x2e2312c14
+   2e2312bc8:	call   0x2e23129c0
+   2e2312bcd:	test   %eax,%eax
+   2e2312bcf:	je     0x2e2312c14
+   2e2312bd1:	movslq 0x3c(%rcx),%rax
+   2e2312bd5:	add    %rax,%rcx
+   2e2312bd8:	movzwl 0x14(%rcx),%eax
+   2e2312bdc:	lea    0x18(%rcx,%rax,1),%r8
+   2e2312be1:	movzwl 0x6(%rcx),%eax
+   2e2312be5:	test   %eax,%eax
+   2e2312be7:	je     0x2e2312c11
+   2e2312be9:	sub    $0x1,%eax
+   2e2312bec:	lea    (%rax,%rax,4),%rax
+   2e2312bf0:	lea    0x28(%r8,%rax,8),%rax
+   2e2312bf5:	nopl   (%rax)
+   2e2312bf8:	testb  $0x20,0x27(%r8)
+   2e2312bfd:	je     0x2e2312c08
+   2e2312bff:	test   %r9,%r9
+   2e2312c02:	je     0x2e2312c14
+   2e2312c04:	sub    $0x1,%r9
+   2e2312c08:	add    $0x28,%r8
+   2e2312c0c:	cmp    %rax,%r8
+   2e2312c0f:	jne    0x2e2312bf8
+   2e2312c11:	xor    %r8d,%r8d
+   2e2312c14:	mov    %r8,%rax
+   2e2312c17:	add    $0x28,%rsp
+   2e2312c1b:	ret
+   2e2312c1c:	nopl   0x0(%rax)
+   2e2312c20:	sub    $0x28,%rsp
+   2e2312c24:	mov    0x25e5(%rip),%rcx        # 0x2e2315210
+   2e2312c2b:	xor    %r8d,%r8d
+   2e2312c2e:	cmpw   $0x5a4d,(%rcx)
+   2e2312c33:	jne    0x2e2312c40
+   2e2312c35:	call   0x2e23129c0
+   2e2312c3a:	test   %eax,%eax
+   2e2312c3c:	cmovne %rcx,%r8
+   2e2312c40:	mov    %r8,%rax
+   2e2312c43:	add    $0x28,%rsp
+   2e2312c47:	ret
+   2e2312c48:	nopl   0x0(%rax,%rax,1)
+   2e2312c50:	sub    $0x28,%rsp
+   2e2312c54:	mov    0x25b5(%rip),%r9        # 0x2e2315210
+   2e2312c5b:	xor    %eax,%eax
+   2e2312c5d:	cmpw   $0x5a4d,(%r9)
+   2e2312c63:	mov    %rcx,%r8
+   2e2312c66:	jne    0x2e2312cbf
+   2e2312c68:	mov    %r9,%rcx
+   2e2312c6b:	call   0x2e23129c0
+   2e2312c70:	test   %eax,%eax
+   2e2312c72:	je     0x2e2312cbf
+   2e2312c74:	movslq 0x3c(%r9),%rax
+   2e2312c78:	mov    %r8,%rcx
+   2e2312c7b:	sub    %r9,%rcx
+   2e2312c7e:	add    %rax,%r9
+   2e2312c81:	movzwl 0x14(%r9),%eax
+   2e2312c86:	movzwl 0x6(%r9),%edx
+   2e2312c8b:	lea    0x18(%r9,%rax,1),%rax
+   2e2312c90:	test   %edx,%edx
+   2e2312c92:	je     0x2e2312cbd
+   2e2312c94:	sub    $0x1,%edx
+   2e2312c97:	lea    (%rdx,%rdx,4),%rdx
+   2e2312c9b:	lea    0x28(%rax,%rdx,8),%r9
+   2e2312ca0:	mov    0xc(%rax),%r8d
+   2e2312ca4:	mov    %r8,%rdx
+   2e2312ca7:	cmp    %r8,%rcx
+   2e2312caa:	jb     0x2e2312cb4
+   2e2312cac:	add    0x8(%rax),%edx
+   2e2312caf:	cmp    %rdx,%rcx
+   2e2312cb2:	jb     0x2e2312cc8
+   2e2312cb4:	add    $0x28,%rax
+   2e2312cb8:	cmp    %r9,%rax
+   2e2312cbb:	jne    0x2e2312ca0
+   2e2312cbd:	xor    %eax,%eax
+   2e2312cbf:	add    $0x28,%rsp
+   2e2312cc3:	ret
+   2e2312cc4:	nopl   0x0(%rax)
+   2e2312cc8:	mov    0x24(%rax),%eax
+   2e2312ccb:	not    %eax
+   2e2312ccd:	shr    $0x1f,%eax
+   2e2312cd0:	add    $0x28,%rsp
+   2e2312cd4:	ret
+   2e2312cd5:	data16 cs nopw 0x0(%rax,%rax,1)
+   2e2312ce0:	sub    $0x28,%rsp
+   2e2312ce4:	mov    0x2525(%rip),%r11        # 0x2e2315210
+   2e2312ceb:	xor    %r9d,%r9d
+   2e2312cee:	cmpw   $0x5a4d,(%r11)
+   2e2312cf4:	mov    %ecx,%r8d
+   2e2312cf7:	jne    0x2e2312d58
+   2e2312cf9:	mov    %r11,%rcx
+   2e2312cfc:	call   0x2e23129c0
+   2e2312d01:	test   %eax,%eax
+   2e2312d03:	je     0x2e2312d58
+   2e2312d05:	movslq 0x3c(%r11),%rcx
+   2e2312d09:	add    %r11,%rcx
+   2e2312d0c:	mov    0x90(%rcx),%eax
+   2e2312d12:	test   %eax,%eax
+   2e2312d14:	je     0x2e2312d58
+   2e2312d16:	movzwl 0x14(%rcx),%edx
+   2e2312d1a:	lea    0x18(%rcx,%rdx,1),%rdx
+   2e2312d1f:	movzwl 0x6(%rcx),%ecx
+   2e2312d23:	test   %ecx,%ecx
+   2e2312d25:	je     0x2e2312d58
+   2e2312d27:	sub    $0x1,%ecx
+   2e2312d2a:	lea    (%rcx,%rcx,4),%rcx
+   2e2312d2e:	lea    0x28(%rdx,%rcx,8),%r10
+   2e2312d33:	nopl   0x0(%rax,%rax,1)
+   2e2312d38:	mov    0xc(%rdx),%r9d
+   2e2312d3c:	mov    %r9,%rcx
+   2e2312d3f:	cmp    %r9,%rax
+   2e2312d42:	jb     0x2e2312d4c
+   2e2312d44:	add    0x8(%rdx),%ecx
+   2e2312d47:	cmp    %rcx,%rax
+   2e2312d4a:	jb     0x2e2312d60
+   2e2312d4c:	add    $0x28,%rdx
+   2e2312d50:	cmp    %r10,%rdx
+   2e2312d53:	jne    0x2e2312d38
+   2e2312d55:	xor    %r9d,%r9d
+   2e2312d58:	mov    %r9,%rax
+   2e2312d5b:	add    $0x28,%rsp
+   2e2312d5f:	ret
+   2e2312d60:	add    %r11,%rax
+   2e2312d63:	jmp    0x2e2312d70
+   2e2312d65:	nopl   (%rax)
+   2e2312d68:	sub    $0x1,%r8d
+   2e2312d6c:	add    $0x14,%rax
+   2e2312d70:	mov    0x4(%rax),%ecx
+   2e2312d73:	test   %ecx,%ecx
+   2e2312d75:	jne    0x2e2312d7e
+   2e2312d77:	mov    0xc(%rax),%edx
+   2e2312d7a:	test   %edx,%edx
+   2e2312d7c:	je     0x2e2312d55
+   2e2312d7e:	test   %r8d,%r8d
+   2e2312d81:	jg     0x2e2312d68
+   2e2312d83:	mov    0xc(%rax),%r9d
+   2e2312d87:	add    %r11,%r9
+   2e2312d8a:	mov    %r9,%rax
+   2e2312d8d:	add    $0x28,%rsp
+   2e2312d91:	ret
+   2e2312d92:	nop
+   2e2312d93:	nop
+   2e2312d94:	nop
+   2e2312d95:	nop
+   2e2312d96:	nop
+   2e2312d97:	nop
+   2e2312d98:	nop
+   2e2312d99:	nop
+   2e2312d9a:	nop
+   2e2312d9b:	nop
+   2e2312d9c:	nop
+   2e2312d9d:	nop
+   2e2312d9e:	nop
+   2e2312d9f:	nop
+   2e2312da0:	fninit
+   2e2312da2:	ret
    2e2312da3:	nop
    2e2312da4:	nop
    2e2312da5:	nop
    2e2312da6:	nop
    2e2312da7:	nop
    2e2312da8:	nop
    2e2312da9:	nop
    2e2312daa:	nop
    2e2312dab:	nop
    2e2312dac:	nop
    2e2312dad:	nop
    2e2312dae:	nop
    2e2312daf:	nop
-   2e2312db0:	mov    $0x1,%eax
-   2e2312db5:	ret
-   2e2312db6:	nop
-   2e2312db7:	nop
-   2e2312db8:	nop
-   2e2312db9:	nop
-   2e2312dba:	nop
-   2e2312dbb:	nop
-   2e2312dbc:	nop
-   2e2312dbd:	nop
-   2e2312dbe:	nop
-   2e2312dbf:	nop
-   2e2312dc0:	mov    $0x1,%eax
-   2e2312dc5:	ret
-   2e2312dc6:	nop
-   2e2312dc7:	nop
-   2e2312dc8:	nop
-   2e2312dc9:	nop
-   2e2312dca:	nop
-   2e2312dcb:	nop
-   2e2312dcc:	nop
-   2e2312dcd:	nop
-   2e2312dce:	nop
-   2e2312dcf:	nop
-   2e2312dd0:	push   %rbx
-   2e2312dd1:	sub    $0x50,%rsp
-   2e2312dd5:	movups %xmm6,0x40(%rsp)
-   2e2312dda:	movq   %xmm0,%rdx
-   2e2312ddf:	movq   %xmm0,%rbx
-   2e2312de4:	shr    $0x20,%rdx
-   2e2312de8:	mov    %edx,%eax
-   2e2312dea:	mov    %edx,%ecx
-   2e2312dec:	and    $0xfffff,%eax
-   2e2312df1:	and    $0x7ff00000,%ecx
-   2e2312df7:	or     %ebx,%eax
-   2e2312df9:	mov    %eax,%r8d
-   2e2312dfc:	or     %ecx,%r8d
-   2e2312dff:	je     0x2e2312ea8
-   2e2312e05:	test   %ecx,%ecx
-   2e2312e07:	je     0x2e2312e11
-   2e2312e09:	cmp    $0x7ff00000,%ecx
-   2e2312e0f:	je     0x2e2312e50
-   2e2312e11:	test   %edx,%edx
-   2e2312e13:	js     0x2e2312e60
-   2e2312e15:	movq   %rbx,%xmm1
-   2e2312e1a:	ucomisd 0x238e(%rip),%xmm1        # 0x2e23151b0
-   2e2312e22:	jnp    0x2e2312f08
-   2e2312e28:	mov    %rbx,0x38(%rsp)
-   2e2312e2d:	fldl   0x38(%rsp)
-   2e2312e31:	fsqrt
-   2e2312e33:	fstpl  0x38(%rsp)
-   2e2312e37:	movsd  0x38(%rsp),%xmm0
-   2e2312e3d:	movups 0x40(%rsp),%xmm6
-   2e2312e42:	add    $0x50,%rsp
-   2e2312e46:	pop    %rbx
-   2e2312e47:	ret
-   2e2312e48:	nopl   0x0(%rax,%rax,1)
-   2e2312e50:	test   %eax,%eax
-   2e2312e52:	jne    0x2e2312ec8
-   2e2312e54:	movsd  0x233c(%rip),%xmm0        # 0x2e2315198
-   2e2312e5c:	test   %edx,%edx
-   2e2312e5e:	jns    0x2e2312e3d
-   2e2312e60:	call   0x2e2312f68
-   2e2312e65:	pxor   %xmm3,%xmm3
-   2e2312e69:	movsd  0x232f(%rip),%xmm6        # 0x2e23151a0
-   2e2312e71:	movq   %rbx,%xmm2
-   2e2312e76:	movl   $0x21,(%rax)
-   2e2312e7c:	lea    0x230d(%rip),%rdx        # 0x2e2315190
-   2e2312e83:	mov    $0x1,%ecx
-   2e2312e88:	movsd  %xmm6,0x20(%rsp)
-   2e2312e8e:	call   0x2e23131a0
-   2e2312e93:	movupd %xmm6,%xmm0
-   2e2312e97:	movups 0x40(%rsp),%xmm6
-   2e2312e9c:	add    $0x50,%rsp
-   2e2312ea0:	pop    %rbx
-   2e2312ea1:	ret
-   2e2312ea2:	nopw   0x0(%rax,%rax,1)
-   2e2312ea8:	movsd  0x22f8(%rip),%xmm0        # 0x2e23151a8
-   2e2312eb0:	test   %edx,%edx
-   2e2312eb2:	js     0x2e2312e3d
-   2e2312eb4:	movups 0x40(%rsp),%xmm6
-   2e2312eb9:	pxor   %xmm0,%xmm0
-   2e2312ebd:	add    $0x50,%rsp
-   2e2312ec1:	pop    %rbx
-   2e2312ec2:	ret
-   2e2312ec3:	nopl   0x0(%rax,%rax,1)
-   2e2312ec8:	call   0x2e2312f68
-   2e2312ecd:	pxor   %xmm3,%xmm3
-   2e2312ed1:	movq   %rbx,%xmm2
-   2e2312ed6:	lea    0x22b3(%rip),%rdx        # 0x2e2315190
-   2e2312edd:	movl   $0x21,(%rax)
-   2e2312ee3:	mov    $0x1,%ecx
-   2e2312ee8:	mov    %rbx,0x20(%rsp)
-   2e2312eed:	call   0x2e23131a0
-   2e2312ef2:	nop
-   2e2312ef3:	movups 0x40(%rsp),%xmm6
-   2e2312ef8:	movq   %rbx,%xmm0
+   2e2312db0:	push   %rcx
+   2e2312db1:	push   %rax
+   2e2312db2:	cmp    $0x1000,%rax
+   2e2312db8:	lea    0x18(%rsp),%rcx
+   2e2312dbd:	jb     0x2e2312dd8
+   2e2312dbf:	sub    $0x1000,%rcx
+   2e2312dc6:	orq    $0x0,(%rcx)
+   2e2312dca:	sub    $0x1000,%rax
+   2e2312dd0:	cmp    $0x1000,%rax
+   2e2312dd6:	ja     0x2e2312dbf
+   2e2312dd8:	sub    %rax,%rcx
+   2e2312ddb:	orq    $0x0,(%rcx)
+   2e2312ddf:	pop    %rax
+   2e2312de0:	pop    %rcx
+   2e2312de1:	ret
+   2e2312de2:	nop
+   2e2312de3:	nop
+   2e2312de4:	nop
+   2e2312de5:	nop
+   2e2312de6:	nop
+   2e2312de7:	nop
+   2e2312de8:	nop
+   2e2312de9:	nop
+   2e2312dea:	nop
+   2e2312deb:	nop
+   2e2312dec:	nop
+   2e2312ded:	nop
+   2e2312dee:	nop
+   2e2312def:	nop
+   2e2312df0:	mov    $0x1,%eax
+   2e2312df5:	ret
+   2e2312df6:	nop
+   2e2312df7:	nop
+   2e2312df8:	nop
+   2e2312df9:	nop
+   2e2312dfa:	nop
+   2e2312dfb:	nop
+   2e2312dfc:	nop
+   2e2312dfd:	nop
+   2e2312dfe:	nop
+   2e2312dff:	nop
+   2e2312e00:	mov    $0x1,%eax
+   2e2312e05:	ret
+   2e2312e06:	nop
+   2e2312e07:	nop
+   2e2312e08:	nop
+   2e2312e09:	nop
+   2e2312e0a:	nop
+   2e2312e0b:	nop
+   2e2312e0c:	nop
+   2e2312e0d:	nop
+   2e2312e0e:	nop
+   2e2312e0f:	nop
+   2e2312e10:	push   %rbx
+   2e2312e11:	sub    $0x50,%rsp
+   2e2312e15:	movups %xmm6,0x40(%rsp)
+   2e2312e1a:	movq   %xmm0,%rdx
+   2e2312e1f:	movq   %xmm0,%rbx
+   2e2312e24:	shr    $0x20,%rdx
+   2e2312e28:	mov    %edx,%eax
+   2e2312e2a:	mov    %edx,%ecx
+   2e2312e2c:	and    $0xfffff,%eax
+   2e2312e31:	and    $0x7ff00000,%ecx
+   2e2312e37:	or     %ebx,%eax
+   2e2312e39:	mov    %eax,%r8d
+   2e2312e3c:	or     %ecx,%r8d
+   2e2312e3f:	je     0x2e2312ee8
+   2e2312e45:	test   %ecx,%ecx
+   2e2312e47:	je     0x2e2312e51
+   2e2312e49:	cmp    $0x7ff00000,%ecx
+   2e2312e4f:	je     0x2e2312e90
+   2e2312e51:	test   %edx,%edx
+   2e2312e53:	js     0x2e2312ea0
+   2e2312e55:	movq   %rbx,%xmm1
+   2e2312e5a:	ucomisd 0x234e(%rip),%xmm1        # 0x2e23151b0
+   2e2312e62:	jnp    0x2e2312f48
+   2e2312e68:	mov    %rbx,0x38(%rsp)
+   2e2312e6d:	fldl   0x38(%rsp)
+   2e2312e71:	fsqrt
+   2e2312e73:	fstpl  0x38(%rsp)
+   2e2312e77:	movsd  0x38(%rsp),%xmm0
+   2e2312e7d:	movups 0x40(%rsp),%xmm6
+   2e2312e82:	add    $0x50,%rsp
+   2e2312e86:	pop    %rbx
+   2e2312e87:	ret
+   2e2312e88:	nopl   0x0(%rax,%rax,1)
+   2e2312e90:	test   %eax,%eax
+   2e2312e92:	jne    0x2e2312f08
+   2e2312e94:	movsd  0x22fc(%rip),%xmm0        # 0x2e2315198
+   2e2312e9c:	test   %edx,%edx
+   2e2312e9e:	jns    0x2e2312e7d
+   2e2312ea0:	call   0x2e2312fa8
+   2e2312ea5:	pxor   %xmm3,%xmm3
+   2e2312ea9:	movsd  0x22ef(%rip),%xmm6        # 0x2e23151a0
+   2e2312eb1:	movq   %rbx,%xmm2
+   2e2312eb6:	movl   $0x21,(%rax)
+   2e2312ebc:	lea    0x22cd(%rip),%rdx        # 0x2e2315190
+   2e2312ec3:	mov    $0x1,%ecx
+   2e2312ec8:	movsd  %xmm6,0x20(%rsp)
+   2e2312ece:	call   0x2e23131e0
+   2e2312ed3:	movupd %xmm6,%xmm0
+   2e2312ed7:	movups 0x40(%rsp),%xmm6
+   2e2312edc:	add    $0x50,%rsp
+   2e2312ee0:	pop    %rbx
+   2e2312ee1:	ret
+   2e2312ee2:	nopw   0x0(%rax,%rax,1)
+   2e2312ee8:	movsd  0x22b8(%rip),%xmm0        # 0x2e23151a8
+   2e2312ef0:	test   %edx,%edx
+   2e2312ef2:	js     0x2e2312e7d
+   2e2312ef4:	movups 0x40(%rsp),%xmm6
+   2e2312ef9:	pxor   %xmm0,%xmm0
    2e2312efd:	add    $0x50,%rsp
    2e2312f01:	pop    %rbx
    2e2312f02:	ret
    2e2312f03:	nopl   0x0(%rax,%rax,1)
-   2e2312f08:	je     0x2e2312ef3
-   2e2312f0a:	jmp    0x2e2312e28
-   2e2312f0f:	nop
-   2e2312f10:	jmp    *0x72e6(%rip)        # 0x2e231a1fc
-   2e2312f16:	nop
-   2e2312f17:	nop
-   2e2312f18:	jmp    *0x72d6(%rip)        # 0x2e231a1f4
-   2e2312f1e:	nop
-   2e2312f1f:	nop
-   2e2312f20:	jmp    *0x72c6(%rip)        # 0x2e231a1ec
-   2e2312f26:	nop
-   2e2312f27:	nop
-   2e2312f28:	jmp    *0x72ae(%rip)        # 0x2e231a1dc
-   2e2312f2e:	nop
-   2e2312f2f:	nop
-   2e2312f30:	jmp    *0x729e(%rip)        # 0x2e231a1d4
-   2e2312f36:	nop
-   2e2312f37:	nop
-   2e2312f38:	jmp    *0x728e(%rip)        # 0x2e231a1cc
-   2e2312f3e:	nop
-   2e2312f3f:	nop
-   2e2312f40:	jmp    *0x727e(%rip)        # 0x2e231a1c4
-   2e2312f46:	nop
-   2e2312f47:	nop
-   2e2312f48:	jmp    *0x726e(%rip)        # 0x2e231a1bc
-   2e2312f4e:	nop
+   2e2312f08:	call   0x2e2312fa8
+   2e2312f0d:	pxor   %xmm3,%xmm3
+   2e2312f11:	movq   %rbx,%xmm2
+   2e2312f16:	lea    0x2273(%rip),%rdx        # 0x2e2315190
+   2e2312f1d:	movl   $0x21,(%rax)
+   2e2312f23:	mov    $0x1,%ecx
+   2e2312f28:	mov    %rbx,0x20(%rsp)
+   2e2312f2d:	call   0x2e23131e0
+   2e2312f32:	nop
+   2e2312f33:	movups 0x40(%rsp),%xmm6
+   2e2312f38:	movq   %rbx,%xmm0
+   2e2312f3d:	add    $0x50,%rsp
+   2e2312f41:	pop    %rbx
+   2e2312f42:	ret
+   2e2312f43:	nopl   0x0(%rax,%rax,1)
+   2e2312f48:	je     0x2e2312f33
+   2e2312f4a:	jmp    0x2e2312e68
    2e2312f4f:	nop
-   2e2312f50:	jmp    *0x725e(%rip)        # 0x2e231a1b4
+   2e2312f50:	jmp    *0x72a6(%rip)        # 0x2e231a1fc
    2e2312f56:	nop
    2e2312f57:	nop
-   2e2312f58:	jmp    *0x724e(%rip)        # 0x2e231a1ac
+   2e2312f58:	jmp    *0x7296(%rip)        # 0x2e231a1f4
    2e2312f5e:	nop
    2e2312f5f:	nop
-   2e2312f60:	jmp    *0x722e(%rip)        # 0x2e231a194
+   2e2312f60:	jmp    *0x7286(%rip)        # 0x2e231a1ec
    2e2312f66:	nop
    2e2312f67:	nop
-   2e2312f68:	jmp    *0x721e(%rip)        # 0x2e231a18c
+   2e2312f68:	jmp    *0x726e(%rip)        # 0x2e231a1dc
    2e2312f6e:	nop
    2e2312f6f:	nop
-   2e2312f70:	jmp    *0x720e(%rip)        # 0x2e231a184
+   2e2312f70:	jmp    *0x725e(%rip)        # 0x2e231a1d4
    2e2312f76:	nop
    2e2312f77:	nop
-   2e2312f78:	nopl   0x0(%rax,%rax,1)
-   2e2312f80:	test   %rcx,%rcx
-   2e2312f83:	je     0x2e2312f9f
-   2e2312f85:	xor    %eax,%eax
-   2e2312f87:	movq   $0x0,0x10(%rcx)
-   2e2312f8f:	movq   $0x0,0x8(%rcx)
-   2e2312f97:	movq   $0x0,(%rcx)
-   2e2312f9e:	ret
-   2e2312f9f:	mov    $0xffffffff,%eax
-   2e2312fa4:	ret
-   2e2312fa5:	data16 cs nopw 0x0(%rax,%rax,1)
-   2e2312fb0:	push   %rbp
-   2e2312fb1:	push   %rdi
-   2e2312fb2:	push   %rsi
-   2e2312fb3:	push   %rbx
-   2e2312fb4:	sub    $0x28,%rsp
-   2e2312fb8:	mov    %rcx,%rbx
-   2e2312fbb:	mov    %rdx,%rdi
-   2e2312fbe:	test   %rcx,%rcx
-   2e2312fc1:	je     0x2e231306b
-   2e2312fc7:	mov    $0x8,%ecx
-   2e2312fcc:	call   0x2e2313140
-   2e2312fd1:	cmpq   $0x0,(%rbx)
-   2e2312fd5:	je     0x2e2313040
-   2e2312fd7:	mov    0x8(%rbx),%rax
-   2e2312fdb:	mov    0x10(%rbx),%rdx
-   2e2312fdf:	cmp    %rax,%rdx
-   2e2312fe2:	je     0x2e2313008
-   2e2312fe4:	lea    0x8(%rax),%rdx
-   2e2312fe8:	mov    $0x8,%ecx
-   2e2312fed:	mov    %rdx,0x8(%rbx)
-   2e2312ff1:	mov    %rdi,(%rax)
-   2e2312ff4:	call   0x2e2313138
-   2e2312ff9:	xor    %eax,%eax
-   2e2312ffb:	add    $0x28,%rsp
-   2e2312fff:	pop    %rbx
-   2e2313000:	pop    %rsi
-   2e2313001:	pop    %rdi
-   2e2313002:	pop    %rbp
-   2e2313003:	ret
-   2e2313004:	nopl   0x0(%rax)
-   2e2313008:	mov    (%rbx),%rcx
-   2e231300b:	sub    %rcx,%rax
-   2e231300e:	mov    %rax,%rdx
-   2e2313011:	mov    %rax,%rsi
-   2e2313014:	sar    $0x3,%rdx
-   2e2313018:	shl    $0x4,%rdx
-   2e231301c:	mov    %rdx,%rbp
-   2e231301f:	call   0x2e2313130
-   2e2313024:	mov    %rax,%rdx
-   2e2313027:	test   %rax,%rax
-   2e231302a:	je     0x2e2313072
-   2e231302c:	add    %rbp,%rdx
-   2e231302f:	mov    %rax,(%rbx)
-   2e2313032:	lea    (%rax,%rsi,1),%rax
-   2e2313036:	mov    %rdx,0x10(%rbx)
-   2e231303a:	jmp    0x2e2312fe4
-   2e231303c:	nopl   0x0(%rax)
-   2e2313040:	mov    $0x8,%edx
-   2e2313045:	mov    $0x20,%ecx
-   2e231304a:	call   0x2e2312f50
-   2e231304f:	mov    %rax,(%rbx)
-   2e2313052:	test   %rax,%rax
-   2e2313055:	je     0x2e2313072
-   2e2313057:	lea    0x100(%rax),%rdx
-   2e231305e:	mov    %rax,0x8(%rbx)
-   2e2313062:	mov    %rdx,0x10(%rbx)
-   2e2313066:	jmp    0x2e2312fdf
-   2e231306b:	mov    $0xffffffff,%eax
-   2e2313070:	jmp    0x2e2312ffb
-   2e2313072:	mov    $0x8,%ecx
-   2e2313077:	call   0x2e2313138
-   2e231307c:	or     $0xffffffff,%eax
-   2e231307f:	jmp    0x2e2312ffb
-   2e2313084:	data16 cs nopw 0x0(%rax,%rax,1)
-   2e231308f:	nop
-   2e2313090:	push   %r12
-   2e2313092:	push   %rsi
-   2e2313093:	push   %rbx
-   2e2313094:	sub    $0x20,%rsp
-   2e2313098:	mov    %rcx,%rsi
-   2e231309b:	mov    $0x8,%ecx
-   2e23130a0:	call   0x2e2313140
-   2e23130a5:	mov    (%rsi),%r12
-   2e23130a8:	mov    0x8(%rsi),%rbx
-   2e23130ac:	movq   $0x0,0x10(%rsi)
-   2e23130b4:	movq   $0x0,0x8(%rsi)
-   2e23130bc:	mov    $0x8,%ecx
-   2e23130c1:	movq   $0x0,(%rsi)
-   2e23130c8:	call   0x2e2313138
-   2e23130cd:	test   %r12,%r12
-   2e23130d0:	je     0x2e23130f6
-   2e23130d2:	sub    $0x8,%rbx
-   2e23130d6:	cmp    %rbx,%r12
-   2e23130d9:	ja     0x2e23130ee
-   2e23130db:	mov    (%rbx),%rax
-   2e23130de:	test   %rax,%rax
-   2e23130e1:	je     0x2e23130d2
-   2e23130e3:	call   *%rax
-   2e23130e5:	sub    $0x8,%rbx
-   2e23130e9:	cmp    %rbx,%r12
-   2e23130ec:	jbe    0x2e23130db
-   2e23130ee:	mov    %r12,%rcx
-   2e23130f1:	call   0x2e2312f48
-   2e23130f6:	xor    %eax,%eax
-   2e23130f8:	add    $0x20,%rsp
-   2e23130fc:	pop    %rbx
-   2e23130fd:	pop    %rsi
-   2e23130fe:	pop    %r12
-   2e2313100:	ret
-   2e2313101:	nop
-   2e2313102:	nop
-   2e2313103:	nop
-   2e2313104:	nop
-   2e2313105:	nop
-   2e2313106:	nop
-   2e2313107:	nop
-   2e2313108:	nop
-   2e2313109:	nop
-   2e231310a:	nop
-   2e231310b:	nop
-   2e231310c:	nop
-   2e231310d:	nop
-   2e231310e:	nop
-   2e231310f:	nop
-   2e2313110:	push   %rbx
-   2e2313111:	sub    $0x20,%rsp
-   2e2313115:	mov    %ecx,%ebx
-   2e2313117:	call   0x2e2313148
-   2e231311c:	mov    %ebx,%ecx
-   2e231311e:	lea    (%rcx,%rcx,2),%rdx
-   2e2313122:	shl    $0x4,%rdx
-   2e2313126:	add    %rdx,%rax
-   2e2313129:	add    $0x20,%rsp
-   2e231312d:	pop    %rbx
-   2e231312e:	ret
-   2e231312f:	nop
-   2e2313130:	jmp    *0x70ae(%rip)        # 0x2e231a1e4
-   2e2313136:	nop
-   2e2313137:	nop
-   2e2313138:	jmp    *0x7066(%rip)        # 0x2e231a1a4
-   2e231313e:	nop
-   2e231313f:	nop
-   2e2313140:	jmp    *0x7056(%rip)        # 0x2e231a19c
+   2e2312f78:	jmp    *0x724e(%rip)        # 0x2e231a1cc
+   2e2312f7e:	nop
+   2e2312f7f:	nop
+   2e2312f80:	jmp    *0x723e(%rip)        # 0x2e231a1c4
+   2e2312f86:	nop
+   2e2312f87:	nop
+   2e2312f88:	jmp    *0x722e(%rip)        # 0x2e231a1bc
+   2e2312f8e:	nop
+   2e2312f8f:	nop
+   2e2312f90:	jmp    *0x721e(%rip)        # 0x2e231a1b4
+   2e2312f96:	nop
+   2e2312f97:	nop
+   2e2312f98:	jmp    *0x720e(%rip)        # 0x2e231a1ac
+   2e2312f9e:	nop
+   2e2312f9f:	nop
+   2e2312fa0:	jmp    *0x71ee(%rip)        # 0x2e231a194
+   2e2312fa6:	nop
+   2e2312fa7:	nop
+   2e2312fa8:	jmp    *0x71de(%rip)        # 0x2e231a18c
+   2e2312fae:	nop
+   2e2312faf:	nop
+   2e2312fb0:	jmp    *0x71ce(%rip)        # 0x2e231a184
+   2e2312fb6:	nop
+   2e2312fb7:	nop
+   2e2312fb8:	nopl   0x0(%rax,%rax,1)
+   2e2312fc0:	test   %rcx,%rcx
+   2e2312fc3:	je     0x2e2312fdf
+   2e2312fc5:	xor    %eax,%eax
+   2e2312fc7:	movq   $0x0,0x10(%rcx)
+   2e2312fcf:	movq   $0x0,0x8(%rcx)
+   2e2312fd7:	movq   $0x0,(%rcx)
+   2e2312fde:	ret
+   2e2312fdf:	mov    $0xffffffff,%eax
+   2e2312fe4:	ret
+   2e2312fe5:	data16 cs nopw 0x0(%rax,%rax,1)
+   2e2312ff0:	push   %rbp
+   2e2312ff1:	push   %rdi
+   2e2312ff2:	push   %rsi
+   2e2312ff3:	push   %rbx
+   2e2312ff4:	sub    $0x28,%rsp
+   2e2312ff8:	mov    %rcx,%rbx
+   2e2312ffb:	mov    %rdx,%rdi
+   2e2312ffe:	test   %rcx,%rcx
+   2e2313001:	je     0x2e23130ab
+   2e2313007:	mov    $0x8,%ecx
+   2e231300c:	call   0x2e2313180
+   2e2313011:	cmpq   $0x0,(%rbx)
+   2e2313015:	je     0x2e2313080
+   2e2313017:	mov    0x8(%rbx),%rax
+   2e231301b:	mov    0x10(%rbx),%rdx
+   2e231301f:	cmp    %rax,%rdx
+   2e2313022:	je     0x2e2313048
+   2e2313024:	lea    0x8(%rax),%rdx
+   2e2313028:	mov    $0x8,%ecx
+   2e231302d:	mov    %rdx,0x8(%rbx)
+   2e2313031:	mov    %rdi,(%rax)
+   2e2313034:	call   0x2e2313178
+   2e2313039:	xor    %eax,%eax
+   2e231303b:	add    $0x28,%rsp
+   2e231303f:	pop    %rbx
+   2e2313040:	pop    %rsi
+   2e2313041:	pop    %rdi
+   2e2313042:	pop    %rbp
+   2e2313043:	ret
+   2e2313044:	nopl   0x0(%rax)
+   2e2313048:	mov    (%rbx),%rcx
+   2e231304b:	sub    %rcx,%rax
+   2e231304e:	mov    %rax,%rdx
+   2e2313051:	mov    %rax,%rsi
+   2e2313054:	sar    $0x3,%rdx
+   2e2313058:	shl    $0x4,%rdx
+   2e231305c:	mov    %rdx,%rbp
+   2e231305f:	call   0x2e2313170
+   2e2313064:	mov    %rax,%rdx
+   2e2313067:	test   %rax,%rax
+   2e231306a:	je     0x2e23130b2
+   2e231306c:	add    %rbp,%rdx
+   2e231306f:	mov    %rax,(%rbx)
+   2e2313072:	lea    (%rax,%rsi,1),%rax
+   2e2313076:	mov    %rdx,0x10(%rbx)
+   2e231307a:	jmp    0x2e2313024
+   2e231307c:	nopl   0x0(%rax)
+   2e2313080:	mov    $0x8,%edx
+   2e2313085:	mov    $0x20,%ecx
+   2e231308a:	call   0x2e2312f90
+   2e231308f:	mov    %rax,(%rbx)
+   2e2313092:	test   %rax,%rax
+   2e2313095:	je     0x2e23130b2
+   2e2313097:	lea    0x100(%rax),%rdx
+   2e231309e:	mov    %rax,0x8(%rbx)
+   2e23130a2:	mov    %rdx,0x10(%rbx)
+   2e23130a6:	jmp    0x2e231301f
+   2e23130ab:	mov    $0xffffffff,%eax
+   2e23130b0:	jmp    0x2e231303b
+   2e23130b2:	mov    $0x8,%ecx
+   2e23130b7:	call   0x2e2313178
+   2e23130bc:	or     $0xffffffff,%eax
+   2e23130bf:	jmp    0x2e231303b
+   2e23130c4:	data16 cs nopw 0x0(%rax,%rax,1)
+   2e23130cf:	nop
+   2e23130d0:	push   %r12
+   2e23130d2:	push   %rsi
+   2e23130d3:	push   %rbx
+   2e23130d4:	sub    $0x20,%rsp
+   2e23130d8:	mov    %rcx,%rsi
+   2e23130db:	mov    $0x8,%ecx
+   2e23130e0:	call   0x2e2313180
+   2e23130e5:	mov    (%rsi),%r12
+   2e23130e8:	mov    0x8(%rsi),%rbx
+   2e23130ec:	movq   $0x0,0x10(%rsi)
+   2e23130f4:	movq   $0x0,0x8(%rsi)
+   2e23130fc:	mov    $0x8,%ecx
+   2e2313101:	movq   $0x0,(%rsi)
+   2e2313108:	call   0x2e2313178
+   2e231310d:	test   %r12,%r12
+   2e2313110:	je     0x2e2313136
+   2e2313112:	sub    $0x8,%rbx
+   2e2313116:	cmp    %rbx,%r12
+   2e2313119:	ja     0x2e231312e
+   2e231311b:	mov    (%rbx),%rax
+   2e231311e:	test   %rax,%rax
+   2e2313121:	je     0x2e2313112
+   2e2313123:	call   *%rax
+   2e2313125:	sub    $0x8,%rbx
+   2e2313129:	cmp    %rbx,%r12
+   2e231312c:	jbe    0x2e231311b
+   2e231312e:	mov    %r12,%rcx
+   2e2313131:	call   0x2e2312f88
+   2e2313136:	xor    %eax,%eax
+   2e2313138:	add    $0x20,%rsp
+   2e231313c:	pop    %rbx
+   2e231313d:	pop    %rsi
+   2e231313e:	pop    %r12
+   2e2313140:	ret
+   2e2313141:	nop
+   2e2313142:	nop
+   2e2313143:	nop
+   2e2313144:	nop
+   2e2313145:	nop
    2e2313146:	nop
    2e2313147:	nop
-   2e2313148:	jmp    *0x7026(%rip)        # 0x2e231a174
+   2e2313148:	nop
+   2e2313149:	nop
+   2e231314a:	nop
+   2e231314b:	nop
+   2e231314c:	nop
+   2e231314d:	nop
    2e231314e:	nop
    2e231314f:	nop
-   2e2313150:	jmp    *0x700e(%rip)        # 0x2e231a164
-   2e2313156:	nop
-   2e2313157:	nop
-   2e2313158:	jmp    *0x6ffe(%rip)        # 0x2e231a15c
-   2e231315e:	nop
-   2e231315f:	nop
-   2e2313160:	jmp    *0x6fee(%rip)        # 0x2e231a154
-   2e2313166:	nop
-   2e2313167:	nop
-   2e2313168:	jmp    *0x6fde(%rip)        # 0x2e231a14c
-   2e231316e:	nop
+   2e2313150:	push   %rbx
+   2e2313151:	sub    $0x20,%rsp
+   2e2313155:	mov    %ecx,%ebx
+   2e2313157:	call   0x2e2313188
+   2e231315c:	mov    %ebx,%ecx
+   2e231315e:	lea    (%rcx,%rcx,2),%rdx
+   2e2313162:	shl    $0x4,%rdx
+   2e2313166:	add    %rdx,%rax
+   2e2313169:	add    $0x20,%rsp
+   2e231316d:	pop    %rbx
+   2e231316e:	ret
    2e231316f:	nop
-   2e2313170:	jmp    *0x6fce(%rip)        # 0x2e231a144
+   2e2313170:	jmp    *0x706e(%rip)        # 0x2e231a1e4
    2e2313176:	nop
    2e2313177:	nop
-   2e2313178:	jmp    *0x6fbe(%rip)        # 0x2e231a13c
+   2e2313178:	jmp    *0x7026(%rip)        # 0x2e231a1a4
    2e231317e:	nop
    2e231317f:	nop
-   2e2313180:	jmp    *0x6fae(%rip)        # 0x2e231a134
+   2e2313180:	jmp    *0x7016(%rip)        # 0x2e231a19c
    2e2313186:	nop
    2e2313187:	nop
-   2e2313188:	jmp    *0x6f9e(%rip)        # 0x2e231a12c
+   2e2313188:	jmp    *0x6fe6(%rip)        # 0x2e231a174
    2e231318e:	nop
    2e231318f:	nop
-   2e2313190:	jmp    *0x6f8e(%rip)        # 0x2e231a124
+   2e2313190:	jmp    *0x6fce(%rip)        # 0x2e231a164
    2e2313196:	nop
    2e2313197:	nop
-   2e2313198:	nopl   0x0(%rax,%rax,1)
-   2e23131a0:	sub    $0x58,%rsp
-   2e23131a4:	mov    0x4f45(%rip),%rax        # 0x2e23180f0
-   2e23131ab:	test   %rax,%rax
-   2e23131ae:	je     0x2e23131dc
-   2e23131b0:	movsd  0x80(%rsp),%xmm0
-   2e23131b9:	mov    %ecx,0x20(%rsp)
-   2e23131bd:	lea    0x20(%rsp),%rcx
-   2e23131c2:	mov    %rdx,0x28(%rsp)
-   2e23131c7:	movsd  %xmm2,0x30(%rsp)
-   2e23131cd:	movsd  %xmm3,0x38(%rsp)
-   2e23131d3:	movsd  %xmm0,0x40(%rsp)
-   2e23131d9:	call   *%rax
-   2e23131db:	nop
-   2e23131dc:	add    $0x58,%rsp
-   2e23131e0:	ret
-   2e23131e1:	data16 cs nopw 0x0(%rax,%rax,1)
-   2e23131ec:	nopl   0x0(%rax)
-   2e23131f0:	mov    %rcx,0x4ef9(%rip)        # 0x2e23180f0
-   2e23131f7:	jmp    0x2e2313200
-   2e23131fc:	nop
-   2e23131fd:	nop
-   2e23131fe:	nop
-   2e23131ff:	nop
-   2e2313200:	jmp    *0x6f76(%rip)        # 0x2e231a17c
-   2e2313206:	nop
-   2e2313207:	nop
-   2e2313208:	nopl   0x0(%rax,%rax,1)
-   2e2313210:	jmp    0x2e2311380
-   2e2313215:	nop
-   2e2313216:	nop
-   2e2313217:	nop
-   2e2313218:	nop
-   2e2313219:	nop
-   2e231321a:	nop
+   2e2313198:	jmp    *0x6fbe(%rip)        # 0x2e231a15c
+   2e231319e:	nop
+   2e231319f:	nop
+   2e23131a0:	jmp    *0x6fae(%rip)        # 0x2e231a154
+   2e23131a6:	nop
+   2e23131a7:	nop
+   2e23131a8:	jmp    *0x6f9e(%rip)        # 0x2e231a14c
+   2e23131ae:	nop
+   2e23131af:	nop
+   2e23131b0:	jmp    *0x6f8e(%rip)        # 0x2e231a144
+   2e23131b6:	nop
+   2e23131b7:	nop
+   2e23131b8:	jmp    *0x6f7e(%rip)        # 0x2e231a13c
+   2e23131be:	nop
+   2e23131bf:	nop
+   2e23131c0:	jmp    *0x6f6e(%rip)        # 0x2e231a134
+   2e23131c6:	nop
+   2e23131c7:	nop
+   2e23131c8:	jmp    *0x6f5e(%rip)        # 0x2e231a12c
+   2e23131ce:	nop
+   2e23131cf:	nop
+   2e23131d0:	jmp    *0x6f4e(%rip)        # 0x2e231a124
+   2e23131d6:	nop
+   2e23131d7:	nop
+   2e23131d8:	nopl   0x0(%rax,%rax,1)
+   2e23131e0:	sub    $0x58,%rsp
+   2e23131e4:	mov    0x4f05(%rip),%rax        # 0x2e23180f0
+   2e23131eb:	test   %rax,%rax
+   2e23131ee:	je     0x2e231321c
+   2e23131f0:	movsd  0x80(%rsp),%xmm0
+   2e23131f9:	mov    %ecx,0x20(%rsp)
+   2e23131fd:	lea    0x20(%rsp),%rcx
+   2e2313202:	mov    %rdx,0x28(%rsp)
+   2e2313207:	movsd  %xmm2,0x30(%rsp)
+   2e231320d:	movsd  %xmm3,0x38(%rsp)
+   2e2313213:	movsd  %xmm0,0x40(%rsp)
+   2e2313219:	call   *%rax
    2e231321b:	nop
-   2e231321c:	nop
-   2e231321d:	nop
-   2e231321e:	nop
-   2e231321f:	nop
-   2e2313220:	(bad)
-   2e2313221:	(bad)
-   2e2313222:	(bad)
-   2e2313223:	(bad)
-   2e2313224:	(bad)
-   2e2313225:	(bad)
-   2e2313226:	(bad)
-   2e2313227:	call   *(%rax)
-   2e2313229:	xor    (%rcx),%dh
-   2e231322b:	loop   0x2e231322f
-	...
-   2e2313235:	add    %al,(%rax)
-   2e2313237:	add    %bh,%bh
-   2e2313239:	(bad)
-   2e231323a:	(bad)
-   2e231323b:	(bad)
-   2e231323c:	(bad)
-   2e231323d:	(bad)
-   2e231323e:	(bad)
-   2e231323f:	incl   (%rax)
-   2e2313241:	add    %al,(%rax)
-   2e2313243:	add    %al,(%rax)
-   2e2313245:	add    %al,(%rax)
+   2e231321c:	add    $0x58,%rsp
+   2e2313220:	ret
+   2e2313221:	data16 cs nopw 0x0(%rax,%rax,1)
+   2e231322c:	nopl   0x0(%rax)
+   2e2313230:	mov    %rcx,0x4eb9(%rip)        # 0x2e23180f0
+   2e2313237:	jmp    0x2e2313240
+   2e231323c:	nop
+   2e231323d:	nop
+   2e231323e:	nop
+   2e231323f:	nop
+   2e2313240:	jmp    *0x6f36(%rip)        # 0x2e231a17c
+   2e2313246:	nop
+   2e2313247:	nop
+   2e2313248:	nopl   0x0(%rax,%rax,1)
+   2e2313250:	jmp    0x2e2311380
+   2e2313255:	nop
+   2e2313256:	nop
+   2e2313257:	nop
+   2e2313258:	nop
+   2e2313259:	nop
+   2e231325a:	nop
+   2e231325b:	nop
+   2e231325c:	nop
+   2e231325d:	nop
+   2e231325e:	nop
+   2e231325f:	nop
+   2e2313260:	(bad)
+   2e2313261:	(bad)
+   2e2313262:	(bad)
+   2e2313263:	(bad)
+   2e2313264:	(bad)
+   2e2313265:	(bad)
+   2e2313266:	(bad)
+   2e2313267:	call   *0x32(%rax)
+   2e231326a:	xor    %esp,%edx
+   2e231326c:	add    (%rax),%al
+	...
+   2e2313276:	add    %al,(%rax)
+   2e2313278:	(bad)
+   2e2313279:	(bad)
+   2e231327a:	(bad)
+   2e231327b:	(bad)
+   2e231327c:	(bad)
+   2e231327d:	(bad)
+   2e231327e:	(bad)
+   2e231327f:	incl   (%rax)
+   2e2313281:	add    %al,(%rax)
+   2e2313283:	add    %al,(%rax)
+   2e2313285:	add    %al,(%rax)
 	...
 
 Disassembly of section .data:
 
 00000002e2314000 <.data>:
    2e2314000:	add    %eax,(%rax)
 	...
    2e231400e:	add    %al,(%rax)
-   2e2314010:	xor    (%rcx),%sil
+   2e2314010:	xorb   $0x31,(%rdx)
    2e2314013:	loop   0x2e2314017
 	...
    2e231401d:	add    %al,(%rax)
    2e231401f:	add    %bh,%bh
    2e2314021:	(bad)
    2e2314022:	(bad)
    2e2314023:	(bad)
@@ -3066,24 +3079,30 @@
    2e2314027:	incl   (%rax)
    2e2314029:	add    %al,(%rax)
    2e231402b:	add    %al,(%rax)
    2e231402d:	add    %al,(%rax)
    2e231402f:	add    %al,(%rdx)
 	...
    2e231403d:	add    %al,(%rax)
-   2e231403f:	add    %dl,0x2e23130(%rax)
+   2e231403f:	add    %dl,%al
+   2e2314041:	xor    %dh,(%rcx)
+   2e2314043:	loop   0x2e2314047
    2e2314045:	add    %al,(%rax)
-   2e2314047:	add    %dh,0x2e2312f(%rax)
-   2e231404d:	add    %al,(%rax)
-   2e231404f:	add    %al,0x2e2312f(%rax)
+   2e2314047:	add    %dh,%al
+   2e2314049:	(bad)
+   2e231404a:	xor    %esp,%edx
+   2e231404c:	add    (%rax),%al
+   2e231404e:	add    %al,(%rax)
+   2e2314050:	shrb   $0x31,(%rdi)
+   2e2314053:	loop   0x2e2314057
 	...
    2e231405d:	add    %al,(%rax)
-   2e231405f:	add    %dl,(%rax)
-   2e2314061:	xor    %esi,(%rcx)
-   2e2314063:	loop   0x2e2314067
+   2e231405f:	add    %dl,0x31(%rax)
+   2e2314062:	xor    %esp,%edx
+   2e2314064:	add    (%rax),%al
 	...
 
 Disassembly of section .rdata:
 
 00000002e2315000 <.rdata>:
    2e2315000:	add    %al,(%rax)
    2e2315002:	add    %al,(%rax)
@@ -3091,21 +3110,18 @@
    2e2315006:	clc
    2e2315007:	jg     0x2e2315009
    2e2315009:	add    %al,(%rax)
    2e231500b:	add    %al,(%rax)
    2e231500d:	add    %ah,%al
    2e231500f:	(bad)
 	...
-   2e2315020:	add    %ah,(%rcx)
-   2e2315022:	xor    %esp,%edx
-   2e2315024:	add    (%rax),%al
-	...
-   2e231503e:	add    %al,(%rax)
-   2e2315040:	add    %al,%al
-   2e2315042:	xor    %esp,%edx
+   2e2315020:	rex and %esi,(%rcx)
+   2e2315023:	loop   0x2e2315027
+	...
+   2e2315041:	shlb   $0xe2,(%rcx)
    2e2315044:	add    (%rax),%al
    2e2315046:	add    %al,(%rax)
    2e2315048:	or     %al,%al
    2e231504a:	xor    %esp,%edx
    2e231504c:	add    (%rax),%al
    2e231504e:	add    %al,(%rax)
    2e2315050:	cmp    $0x80,%al
@@ -3223,20 +3239,21 @@
    2e23151b4:	add    %al,(%rax)
    2e23151b6:	lock (bad)
 	...
    2e23151c0:	xor    %al,0x31(%rax)
    2e23151c3:	loop   0x2e23151c7
 	...
    2e23151cd:	add    %al,(%rax)
-   2e23151cf:	add    %ah,(%rax)
-   2e23151d1:	xor    (%rcx),%dh
-   2e23151d3:	loop   0x2e23151d7
-	...
-   2e23151dd:	add    %al,(%rax)
-   2e23151df:	add    %ah,0x55(%rax)
+   2e23151cf:	add    %ah,0x32(%rax)
+   2e23151d2:	xor    %esp,%edx
+   2e23151d4:	add    (%rax),%al
+	...
+   2e23151de:	add    %al,(%rax)
+   2e23151e0:	(bad)
+   2e23151e1:	push   %rbp
    2e23151e2:	xor    %esp,%edx
    2e23151e4:	add    (%rax),%al
 	...
    2e23151ee:	add    %al,(%rax)
    2e23151f0:	(bad)
    2e23151f1:	push   %rbp
    2e23151f2:	xor    %esp,%edx
@@ -3638,170 +3655,196 @@
    2e231609c:	mov    $0x18,%al
    2e231609e:	add    %al,(%rax)
    2e23160a0:	mov    $0x18,%ch
    2e23160a2:	add    %al,(%rax)
    2e23160a4:	jl     0x2e2316116
    2e23160a6:	add    %al,(%rax)
    2e23160a8:	rcrb   $0x0,(%rax)
-   2e23160ab:	add    %ah,-0x7fffffe1(%rax)
-   2e23160b1:	jo     0x2e23160b3
-   2e23160b3:	add    %ah,-0x36ffffe1(%rax)
-   2e23160b9:	(bad)
+   2e23160ab:	add    %bl,%ah
+   2e23160ad:	(bad)
+   2e23160ae:	add    %al,(%rax)
+   2e23160b0:	xorb   $0x0,0x0(%rax)
+   2e23160b4:	loopne 0x2e23160d5
+   2e23160b6:	add    %al,(%rax)
+   2e23160b8:	or     %esp,(%rax)
    2e23160ba:	add    %al,(%rax)
    2e23160bc:	pushf
    2e23160bd:	jo     0x2e23160bf
-   2e23160bf:	add    %dl,%al
-   2e23160c1:	(bad)
-   2e23160c2:	add    %al,(%rax)
-   2e23160c4:	int1
-   2e23160c5:	(bad)
-   2e23160c6:	add    %al,(%rax)
-   2e23160c8:	movabs 0x3a00002000000070,%al
-   2e23160d1:	and    %al,(%rax)
-   2e23160d3:	add    %ah,0x20400000(%rax,%rsi,2)
-   2e23160da:	add    %al,(%rax)
-   2e23160dc:	stos   %al,%es:(%rdi)
+   2e23160bf:	add    %dl,(%rax)
+   2e23160c1:	and    %al,(%rax)
+   2e23160c3:	add    %dh,(%rcx)
+   2e23160c5:	and    %al,(%rax)
+   2e23160c7:	add    %ah,0x40000070(%rax)
+   2e23160cd:	and    %al,(%rax)
+   2e23160cf:	add    %bh,0x20(%rdx)
+   2e23160d2:	add    %al,(%rax)
+   2e23160d4:	movsb  %ds:(%rsi),%es:(%rdi)
+   2e23160d5:	jo     0x2e23160d7
+   2e23160d7:	add    %al,-0x15ffffe0(%rax)
    2e23160dd:	and    %al,(%rax)
-   2e23160df:	add    %ch,0x20b00000(%rax,%rsi,2)
+   2e23160df:	add    %ch,0x20f00000(%rax,%rsi,2)
    2e23160e6:	add    %al,(%rax)
-   2e23160e8:	iret
-   2e23160e9:	and    %al,(%rax)
-   2e23160eb:	add    %bh,-0x2fffff90(%rax)
-   2e23160f1:	and    %al,(%rax)
-   2e23160f3:	add    %bh,%bh
-   2e23160f5:	and    %al,(%rax)
-   2e23160f7:	add    %bh,0x21000000(%rax,%rsi,2)
+   2e23160e8:	mov    %db0,%rax
+   2e23160eb:	add    %bh,0x10000070(%rax)
+   2e23160f1:	and    %eax,(%rax)
+   2e23160f3:	add    %bh,(%rdi)
+   2e23160f5:	and    %eax,(%rax)
+   2e23160f7:	add    %bh,0x21400000(%rax,%rsi,2)
    2e23160fe:	add    %al,(%rax)
-   2e2316100:	andl   $0x70c40000,(%rcx)
-   2e2316106:	add    %al,(%rax)
-   2e2316108:	nop
+   2e2316100:	shll   $0x0,(%rcx)
+   2e2316103:	add    %al,%ah
+   2e2316105:	jo     0x2e2316107
+   2e2316107:	add    %dl,%al
    2e2316109:	and    %eax,(%rax)
-   2e231610b:	add    %dl,-0x2fffffdf(%rbx)
+   2e231610b:	add    %dl,%bl
+   2e231610d:	and    %eax,(%rax)
+   2e231610f:	add    %dl,%al
    2e2316111:	jo     0x2e2316113
-   2e2316113:	add    %ah,0xa000021(%rax)
-   2e2316119:	and    (%rax),%al
-   2e231611b:	add    %dl,%ah
+   2e2316113:	add    %ah,%al
+   2e2316115:	and    %eax,(%rax)
+   2e2316117:	add    %cl,0x22(%rdx)
+   2e231611a:	add    %al,(%rax)
+   2e231611c:	(bad)
    2e231611d:	jo     0x2e231611f
-   2e231611f:	add    %dl,(%rax)
-   2e2316121:	and    (%rax),%al
-   2e2316123:	add    %ch,-0x1fffffdc(%rip)        # 0x2c231614d
+   2e231611f:	add    %dl,0x22(%rax)
+   2e2316122:	add    %al,(%rax)
+   2e2316124:	insl   (%dx),%es:(%rdi)
+   2e2316125:	and    $0x0,%al
+   2e2316127:	add    %ah,%al
    2e2316129:	jo     0x2e231612b
-   2e231612b:	add    %dh,(%rax)
-   2e231612d:	and    $0x0,%al
-   2e231612f:	add    %dl,-0xfffffd9(%rip)        # 0x2d231615c
-   2e2316135:	jo     0x2e2316137
-   2e2316137:	add    %ah,(%rax)
-   2e2316139:	(bad)
+   2e231612b:	add    %dh,0x24(%rax)
+   2e231612e:	add    %al,(%rax)
+   2e2316130:	push   %rbp
+   2e2316131:	(bad)
+   2e2316132:	add    %al,(%rax)
+   2e2316134:	lock jo 0x2e2316137
+   2e2316137:	add    %ah,0x27(%rax)
    2e231613a:	add    %al,(%rax)
-   2e231613c:	mov    (%rdi),%esp
+   2e231613c:	lret
+   2e231613d:	(bad)
    2e231613e:	add    %al,(%rax)
    2e2316140:	or     %dh,0x0(%rcx)
-   2e2316143:	add    %dl,0x8000027(%rax)
-   2e2316149:	sub    %al,(%rax)
+   2e2316143:	add    %dl,%al
+   2e2316145:	(bad)
+   2e2316146:	add    %al,(%rax)
+   2e2316148:	rex.W sub %al,(%rax)
    2e231614b:	add    %bl,(%rax)
    2e231614d:	jno    0x2e231614f
-   2e231614f:	add    %dl,(%rax)
-   2e2316151:	sub    %al,(%rax)
-   2e2316153:	add    %bl,0x24000028(%rcx)
-   2e2316159:	jno    0x2e231615b
-   2e231615b:	add    %ah,-0x7fffffd8(%rax)
-   2e2316161:	sub    %eax,(%rax)
+   2e231614f:	add    %dl,0x28(%rax)
+   2e2316152:	add    %al,(%rax)
+   2e2316154:	fldcw  (%rax)
+   2e2316156:	add    %al,(%rax)
+   2e2316158:	and    $0x71,%al
+   2e231615a:	add    %al,(%rax)
+   2e231615c:	loopne 0x2e2316186
+   2e231615e:	add    %al,(%rax)
+   2e2316160:	shrb   $0x0,(%rcx)
    2e2316163:	add    %ch,(%rcx,%rsi,2)
    2e2316166:	add    %al,(%rax)
-   2e2316168:	subb   $0x0,(%rcx)
-   2e231616b:	add    %bl,0x34000029(%rsi)
-   2e2316171:	jno    0x2e2316173
-   2e2316173:	add    %ah,-0x4cffffd7(%rax)
-   2e2316179:	sub    %eax,(%rax)
+   2e2316168:	shrb   $0x0,(%rcx)
+   2e231616b:	add    %bl,%dh
+   2e231616d:	sub    %eax,(%rax)
+   2e231616f:	add    %dh,(%rcx,%rsi,2)
+   2e2316172:	add    %al,(%rax)
+   2e2316174:	loopne 0x2e231619f
+   2e2316176:	add    %al,(%rax)
+   2e2316178:	repz sub %eax,(%rax)
    2e231617b:	add    %bh,(%rax)
    2e231617d:	jno    0x2e231617f
-   2e231617f:	add    %al,%al
-   2e2316181:	sub    %eax,(%rax)
-   2e2316183:	add    %cl,(%rax)
-   2e2316185:	sub    (%rax),%al
-   2e2316187:	add    %bh,(%rcx,%rsi,2)
+   2e231617f:	add    %al,(%rax)
+   2e2316181:	sub    (%rax),%al
+   2e2316183:	add    %cl,0x2a(%rax)
+   2e2316186:	add    %al,(%rax)
+   2e2316188:	cmp    $0x71,%al
    2e231618a:	add    %al,(%rax)
-   2e231618c:	adc    %ch,(%rdx)
-   2e231618e:	add    %al,(%rax)
-   2e2316190:	scas   %es:(%rdi),%eax
+   2e231618c:	push   %rax
+   2e231618d:	sub    (%rax),%al
+   2e231618f:	add    %ch,%bh
    2e2316191:	sub    (%rax),%al
    2e2316193:	add    %al,0x71(%rax)
    2e2316196:	add    %al,(%rax)
-   2e2316198:	mov    $0x2a,%al
-   2e231619a:	add    %al,(%rax)
-   2e231619c:	xor    %ebp,(%rbx)
+   2e2316198:	lock sub (%rax),%al
+   2e231619b:	add    %dh,0x2b(%rcx)
    2e231619e:	add    %al,(%rax)
    2e23161a0:	rex.WR jno 0x2e23161a3
-   2e23161a3:	add    %al,0x2b(%rax)
-   2e23161a6:	add    %al,(%rax)
-   2e23161a8:	imul   $0x0,(%rbx),%ebp
+   2e23161a3:	add    %al,-0x54ffffd5(%rax)
+   2e23161a9:	sub    (%rax),%eax
    2e23161ab:	add    %dl,0x0(%rcx,%rsi,2)
-   2e23161af:	add    %dh,0x2b(%rax)
-   2e23161b2:	add    %al,(%rax)
-   2e23161b4:	fsubrl (%rbx)
-   2e23161b6:	add    %al,(%rax)
-   2e23161b8:	pop    %rsp
-   2e23161b9:	jno    0x2e23161bb
-   2e23161bb:	add    %ah,%al
-   2e23161bd:	sub    (%rax),%eax
-   2e23161bf:	add    %cl,(%rax)
-   2e23161c1:	sub    $0x0,%al
-   2e23161c3:	add    %ah,0x0(%rcx,%rsi,2)
-   2e23161c7:	add    %dl,(%rax)
-   2e23161c9:	sub    $0x0,%al
-   2e23161cb:	add    %dl,0x6c00002c(%rbp)
-   2e23161d1:	jno    0x2e23161d3
-   2e23161d3:	add    %ah,0x5200002c(%rax)
-   2e23161d9:	sub    $0x71740000,%eax
-   2e23161de:	add    %al,(%rax)
-   2e23161e0:	(bad)
-   2e23161e1:	sub    $0x2d630000,%eax
-   2e23161e6:	add    %al,(%rax)
-   2e23161e8:	jl     0x2e231625b
+   2e23161af:	add    %dh,0x1c00002b(%rax)
+   2e23161b5:	sub    $0x0,%al
+   2e23161b7:	add    %bl,0x0(%rcx,%rsi,2)
+   2e23161bb:	add    %ah,(%rax)
+   2e23161bd:	sub    $0x0,%al
+   2e23161bf:	add    %cl,0x2c(%rax)
+   2e23161c2:	add    %al,(%rax)
+   2e23161c4:	fs jno 0x2e23161c7
+   2e23161c7:	add    %dl,0x2c(%rax)
+   2e23161ca:	add    %al,(%rax)
+   2e23161cc:	(bad)
+   2e23161cd:	sub    $0x0,%al
+   2e23161cf:	add    %ch,0x0(%rcx,%rsi,2)
+   2e23161d3:	add    %ah,%al
+   2e23161d5:	sub    $0x0,%al
+   2e23161d7:	add    %dl,0x7400002d(%rdx)
+   2e23161dd:	jno    0x2e23161df
+   2e23161df:	add    %ah,-0x5cffffd3(%rax)
+   2e23161e5:	sub    $0x717c0000,%eax
    2e23161ea:	add    %al,(%rax)
-   2e23161ec:	mov    $0x2d,%al
-   2e23161ee:	add    %al,(%rax)
-   2e23161f0:	mov    $0x2d,%dh
+   2e23161ec:	lock sub $0x2df60000,%eax
    2e23161f2:	add    %al,(%rax)
    2e23161f4:	xorb   $0x0,0x0(%rcx)
-   2e23161f8:	shrb   $0x0,0x2dc60000(%rip)        # 0x30ff761ff
-   2e23161ff:	add    %al,0x2dd00000(%rcx,%rsi,2)
-   2e2316206:	add    %al,(%rax)
-   2e2316208:	comiss (%rax),%xmm0
-   2e231620b:	add    %cl,-0x7fffff8f(%rax)
+   2e23161f8:	add    %ch,(%rsi)
+   2e23161fa:	add    %al,(%rax)
+   2e23161fc:	(bad)
+   2e23161fd:	cs add %al,(%rax)
+   2e2316200:	test   %dh,0x0(%rcx)
+   2e2316203:	add    %dl,(%rax)
+   2e2316205:	cs add %al,(%rax)
+   2e2316208:	rex.WRXB (bad)
+   2e231620a:	add    %al,(%rax)
+   2e231620c:	mov    %dh,0x0(%rcx)
+   2e231620f:	add    %al,%al
    2e2316211:	(bad)
    2e2316212:	add    %al,(%rax)
-   2e2316214:	movsl  %ds:(%rsi),%es:(%rdi)
-   2e2316215:	(bad)
+   2e2316214:	in     $0x2f,%eax
    2e2316216:	add    %al,(%rax)
    2e2316218:	xchg   %eax,%esp
    2e2316219:	jno    0x2e231621b
-   2e231621b:	add    %dh,-0x7bffffd1(%rax)
+   2e231621b:	add    %dh,%al
+   2e231621d:	(bad)
+   2e231621e:	add    %al,(%rax)
+   2e2316220:	(bad)
    2e2316221:	xor    %al,(%rax)
-   2e2316223:	add    %bl,-0x6fffff8f(%rax)
+   2e2316223:	add    %bl,-0x2fffff8f(%rax)
    2e2316229:	xor    %al,(%rax)
-   2e231622b:	add    %al,(%rcx)
-   2e231622d:	xor    %eax,(%rax)
-   2e231622f:	add    %ch,0x10000071(%rax)
+   2e231622b:	add    %al,0x31(%rcx)
+   2e231622e:	add    %al,(%rax)
+   2e2316230:	test   $0x71,%al
+   2e2316232:	add    %al,(%rax)
+   2e2316234:	push   %rax
    2e2316235:	xor    %eax,(%rax)
-   2e2316237:	add    %ch,(%rdi)
-   2e2316239:	xor    %eax,(%rax)
-   2e231623b:	add    %dh,0x31a00000(%rcx,%rsi,2)
+   2e2316237:	add    %ch,0x31(%rdi)
+   2e231623a:	add    %al,(%rax)
+   2e231623c:	mov    $0x71,%ah
+   2e231623e:	add    %al,(%rax)
+   2e2316240:	loopne 0x2e2316273
    2e2316242:	add    %al,(%rax)
-   2e2316244:	loope  0x2e2316277
+   2e2316244:	and    %esi,(%rdx)
    2e2316246:	add    %al,(%rax)
-   2e2316248:	mov    $0xf0000071,%esp
-   2e231624d:	xor    %eax,(%rax)
-   2e231624f:	add    %bh,%ah
-   2e2316251:	xor    %eax,(%rax)
-   2e2316253:	add    %al,%ah
+   2e2316248:	mov    $0x30000071,%esp
+   2e231624d:	xor    (%rax),%al
+   2e231624f:	add    %bh,(%rdx,%rsi,1)
+   2e2316252:	add    %al,(%rax)
+   2e2316254:	(bad)
    2e2316255:	jno    0x2e2316257
-   2e2316257:	add    %dl,(%rax)
-   2e2316259:	xor    (%rax),%al
-   2e231625b:	add    %dl,-0x37ffffce(%rip)        # 0x2aa316293
+   2e2316257:	add    %dl,0x32(%rax)
+   2e231625a:	add    %al,(%rax)
+   2e231625c:	push   %rbp
+   2e231625d:	xor    (%rax),%al
+   2e231625f:	add    %cl,%al
    2e2316261:	jno    0x2e2316263
 	...
 
 Disassembly of section .xdata:
 
 00000002e2317000 <.xdata>:
    2e2317000:	add    %eax,(%rax)
@@ -4010,38 +4053,42 @@
 	...
 
 Disassembly of section .edata:
 
 00000002e2319000 <.edata>:
    2e2319000:	add    %al,(%rax)
    2e2319002:	add    %al,(%rax)
-   2e2319004:	sbb    0x63b4(%rbp),%ch
-   2e231900a:	add    %al,(%rax)
-   2e231900c:	mov    %ss,0x10000(%rax)
+   2e2319004:	out    %eax,(%dx)
+   2e2319005:	mov    $0xb4,%ch
+   2e2319007:	movsxd (%rax),%eax
+   2e2319009:	add    %al,(%rax)
+   2e231900b:	add    %cl,0x10000(%rax,%rdx,4)
    2e2319012:	add    %al,(%rax)
    2e2319014:	or     (%rax),%al
    2e2319016:	add    %al,(%rax)
    2e2319018:	or     (%rax),%al
    2e231901a:	add    %al,(%rax)
    2e231901c:	sub    %dl,-0x6fb00000(%rax)
    2e2319022:	add    %al,(%rax)
    2e2319024:	js     0x2e2318fb6
    2e2319026:	add    %al,(%rax)
    2e2319028:	movabs 0xb000001400000013,%al
    2e2319031:	sbb    %al,(%rax)
    2e2319033:	add    %al,(%rax)
    2e2319035:	adc    $0x15900000,%eax
    2e231903a:	add    %al,(%rax)
-   2e231903c:	rcrb   (%rdi)
+   2e231903c:	adc    %ah,(%rax)
    2e231903e:	add    %al,(%rax)
    2e2319040:	rcrb   $0x0,(%rax)
-   2e2319043:	add    %ah,0x7000001f(%rax)
-   2e2319049:	adc    $0x0,%al
-   2e231904b:	add    %al,%al
-   2e231904d:	adc    (%rax),%eax
+   2e2319043:	add    %ah,%al
+   2e2319045:	(bad)
+   2e2319046:	add    %al,(%rax)
+   2e2319048:	jo     0x2e231905e
+   2e231904a:	add    %al,(%rax)
+   2e231904c:	rclb   $0x0,(%rbx)
    2e231904f:	add    %bl,-0x6f590000(%rax,%rdx,4)
    2e2319056:	add    %al,(%rax)
    2e2319058:	mov    $0x90,%ah
    2e231905a:	add    %al,(%rax)
    2e231905c:	mov    $0xc3000090,%ebx
    2e2319061:	nop
    2e2319062:	add    %al,(%rax)
@@ -4500,37 +4547,36 @@
 00000002e231b000 <.CRT>:
 	...
    2e231b018:	add    %dl,(%rax)
    2e231b01a:	xor    %esp,%edx
    2e231b01c:	add    (%rax),%al
 	...
    2e231b02e:	add    %al,(%rax)
-   2e231b030:	add    %ah,(%rcx)
-   2e231b032:	xor    %esp,%edx
-   2e231b034:	add    (%rax),%al
-   2e231b036:	add    %al,(%rax)
-   2e231b038:	shlb   (%rax)
-   2e231b03a:	xor    %esp,%edx
-   2e231b03c:	add    (%rax),%al
+   2e231b030:	rex and %esi,(%rcx)
+   2e231b033:	loop   0x2e231b037
+   2e231b035:	add    %al,(%rax)
+   2e231b037:	add    %dl,(%rax)
+   2e231b039:	and    %esi,(%rcx)
+   2e231b03b:	loop   0x2e231b03f
 	...
 
 Disassembly of section .tls:
 
 00000002e231c000 <.tls>:
 	...
 
 Disassembly of section .reloc:
 
 00000002e231d000 <.reloc>:
    2e231d000:	add    %dh,(%rax)
    2e231d002:	add    %al,(%rax)
    2e231d004:	or     $0x0,%al
    2e231d006:	add    %al,(%rax)
-   2e231d008:	sub    %ah,0x40000000(%rdx)
-   2e231d00e:	add    %al,(%rax)
+   2e231d008:	push   $0xa2
+   2e231d00d:	rex add %al,(%rax)
    2e231d010:	adc    $0x0,%al
    2e231d012:	add    %al,(%rax)
    2e231d014:	adc    %ah,-0x5fb75fc0(%rax)
    2e231d01a:	push   %rax
    2e231d01b:	movabs 0x50000000a060,%al
    2e231d024:	xor    %al,(%rax)
    2e231d026:	add    %al,(%rax)
```

### Comparing `bmxp-0.0.8/bmxp/gravity/correlation.so` & `bmxp-0.0.9/bmxp/gravity/correlation.so`

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

 * *Files 10% similar despite different names*

#### readelf --wide --program-header {}

```diff
@@ -2,15 +2,15 @@
 Elf file type is DYN (Shared object file)
 Entry point 0x0
 There are 11 program headers, starting at offset 64
 
 Program Headers:
   Type           Offset   VirtAddr           PhysAddr           FileSiz  MemSiz   Flg Align
   LOAD           0x000000 0x0000000000000000 0x0000000000000000 0x000838 0x000838 R   0x1000
-  LOAD           0x001000 0x0000000000001000 0x0000000000001000 0x000d25 0x000d25 R E 0x1000
+  LOAD           0x001000 0x0000000000001000 0x0000000000001000 0x000d55 0x000d55 R E 0x1000
   LOAD           0x002000 0x0000000000002000 0x0000000000002000 0x000254 0x000254 R   0x1000
   LOAD           0x002e08 0x0000000000003e08 0x0000000000003e08 0x000270 0x000278 RW  0x1000
   DYNAMIC        0x002e18 0x0000000000003e18 0x0000000000003e18 0x0001c0 0x0001c0 RW  0x8
   NOTE           0x0002a8 0x00000000000002a8 0x00000000000002a8 0x000020 0x000020 R   0x8
   NOTE           0x0002c8 0x00000000000002c8 0x00000000000002c8 0x000024 0x000024 R   0x4
   GNU_PROPERTY   0x0002a8 0x00000000000002a8 0x00000000000002a8 0x000020 0x000020 R   0x8
   GNU_EH_FRAME   0x002010 0x0000000000002010 0x0000000000002010 0x000074 0x000074 R   0x4
```

#### readelf --wide --sections {}

```diff
@@ -12,16 +12,16 @@
   [ 7] .gnu.version_r    VERNEED         0000000000000640 000640 000030 00   A  5   1  8
   [ 8] .rela.dyn         RELA            0000000000000670 000670 0000c0 18   A  4   0  8
   [ 9] .rela.plt         RELA            0000000000000730 000730 000108 18  AI  4  23  8
   [10] .init             PROGBITS        0000000000001000 001000 00001b 00  AX  0   0  4
   [11] .plt              PROGBITS        0000000000001020 001020 0000c0 10  AX  0   0 16
   [12] .plt.got          PROGBITS        00000000000010e0 0010e0 000010 10  AX  0   0 16
   [13] .plt.sec          PROGBITS        00000000000010f0 0010f0 0000b0 10  AX  0   0 16
-  [14] .text             PROGBITS        00000000000011a0 0011a0 000b76 00  AX  0   0 16
-  [15] .fini             PROGBITS        0000000000001d18 001d18 00000d 00  AX  0   0  4
+  [14] .text             PROGBITS        00000000000011a0 0011a0 000ba6 00  AX  0   0 16
+  [15] .fini             PROGBITS        0000000000001d48 001d48 00000d 00  AX  0   0  4
   [16] .rodata           PROGBITS        0000000000002000 002000 000010 08  AM  0   0  8
   [17] .eh_frame_hdr     PROGBITS        0000000000002010 002010 000074 00   A  0   0  4
   [18] .eh_frame         PROGBITS        0000000000002088 002088 0001cc 00   A  0   0  8
   [19] .init_array       INIT_ARRAY      0000000000003e08 002e08 000008 08  WA  0   0  8
   [20] .fini_array       FINI_ARRAY      0000000000003e10 002e10 000008 08  WA  0   0  8
   [21] .dynamic          DYNAMIC         0000000000003e18 002e18 0001c0 10  WA  5   0  8
   [22] .got              PROGBITS        0000000000003fd8 002fd8 000028 08  WA  0   0  8
```

#### readelf --wide --symbols {}

```diff
@@ -10,21 +10,21 @@
      6: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND malloc@GLIBC_2.2.5 (2)
      7: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND sqrt
      8: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_registerTMCloneTable
      9: 0000000000000000     0 FUNC    WEAK   DEFAULT  UND __cxa_finalize@GLIBC_2.2.5 (2)
     10: 00000000000015b0     9 FUNC    GLOBAL DEFAULT   14 free_p
     11: 0000000000001390   111 FUNC    GLOBAL DEFAULT   14 nanMask
     12: 0000000000001400   418 FUNC    GLOBAL DEFAULT   14 pearson
-    13: 0000000000001cf0    38 FUNC    GLOBAL DEFAULT   14 pearson_array
-    14: 0000000000001cc0    41 FUNC    GLOBAL DEFAULT   14 spearman_array
+    13: 0000000000001d20    38 FUNC    GLOBAL DEFAULT   14 pearson_array
+    14: 0000000000001cf0    41 FUNC    GLOBAL DEFAULT   14 spearman_array
     15: 0000000000001280    53 FUNC    GLOBAL DEFAULT   14 sum_m
     16: 0000000000001310   119 FUNC    GLOBAL DEFAULT   14 stdev_m
     17: 0000000000001260    29 FUNC    GLOBAL DEFAULT   14 comparator
     18: 00000000000012c0    77 FUNC    GLOBAL DEFAULT   14 covariance_m
-    19: 00000000000015c0  1777 FUNC    GLOBAL DEFAULT   14 spearman
+    19: 00000000000015c0  1838 FUNC    GLOBAL DEFAULT   14 spearman
 
 Symbol table '.symtab' contains 39 entries:
    Num:    Value          Size Type    Bind   Vis      Ndx Name
      0: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT  UND 
      1: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS crtstuff.c
      2: 00000000000011a0     0 FUNC    LOCAL  DEFAULT   14 deregister_tm_clones
      3: 00000000000011d0     0 FUNC    LOCAL  DEFAULT   14 register_tm_clones
@@ -33,33 +33,33 @@
      6: 0000000000003e10     0 OBJECT  LOCAL  DEFAULT   20 __do_global_dtors_aux_fini_array_entry
      7: 0000000000001250     0 FUNC    LOCAL  DEFAULT   14 frame_dummy
      8: 0000000000003e08     0 OBJECT  LOCAL  DEFAULT   19 __frame_dummy_init_array_entry
      9: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS correlation.c
     10: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS crtstuff.c
     11: 0000000000002250     0 OBJECT  LOCAL  DEFAULT   18 __FRAME_END__
     12: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS 
-    13: 0000000000001d18     0 FUNC    LOCAL  DEFAULT   15 _fini
+    13: 0000000000001d48     0 FUNC    LOCAL  DEFAULT   15 _fini
     14: 0000000000004070     0 OBJECT  LOCAL  DEFAULT   24 __dso_handle
     15: 0000000000003e18     0 OBJECT  LOCAL  DEFAULT   21 _DYNAMIC
     16: 0000000000002010     0 NOTYPE  LOCAL  DEFAULT   17 __GNU_EH_FRAME_HDR
     17: 0000000000004078     0 OBJECT  LOCAL  DEFAULT   24 __TMC_END__
     18: 0000000000004000     0 OBJECT  LOCAL  DEFAULT   23 _GLOBAL_OFFSET_TABLE_
     19: 0000000000001000     0 FUNC    LOCAL  DEFAULT   10 _init
     20: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND free@GLIBC_2.2.5
     21: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_deregisterTMCloneTable
     22: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND qsort@GLIBC_2.2.5
     23: 00000000000015b0     9 FUNC    GLOBAL DEFAULT   14 free_p
     24: 0000000000001390   111 FUNC    GLOBAL DEFAULT   14 nanMask
     25: 0000000000001400   418 FUNC    GLOBAL DEFAULT   14 pearson
     26: 00000000000012c0    77 FUNC    GLOBAL DEFAULT   14 covariance_m
-    27: 0000000000001cf0    38 FUNC    GLOBAL DEFAULT   14 pearson_array
+    27: 0000000000001d20    38 FUNC    GLOBAL DEFAULT   14 pearson_array
     28: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND __gmon_start__
     29: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND memcpy@GLIBC_2.14
-    30: 00000000000015c0  1777 FUNC    GLOBAL DEFAULT   14 spearman
-    31: 0000000000001cc0    41 FUNC    GLOBAL DEFAULT   14 spearman_array
+    30: 00000000000015c0  1838 FUNC    GLOBAL DEFAULT   14 spearman
+    31: 0000000000001cf0    41 FUNC    GLOBAL DEFAULT   14 spearman_array
     32: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND malloc@GLIBC_2.2.5
     33: 0000000000001310   119 FUNC    GLOBAL DEFAULT   14 stdev_m
     34: 0000000000001260    29 FUNC    GLOBAL DEFAULT   14 comparator
     35: 0000000000001280    53 FUNC    GLOBAL DEFAULT   14 sum_m
     36: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND sqrt
     37: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_registerTMCloneTable
     38: 0000000000000000     0 FUNC    WEAK   DEFAULT  UND __cxa_finalize@GLIBC_2.2.5
```

#### readelf --wide --dynamic {}

```diff
@@ -1,13 +1,13 @@
 
 Dynamic section at offset 0x2e18 contains 24 entries:
   Tag        Type                         Name/Value
  0x0000000000000001 (NEEDED)             Shared library: [libc.so.6]
  0x000000000000000c (INIT)               0x1000
- 0x000000000000000d (FINI)               0x1d18
+ 0x000000000000000d (FINI)               0x1d48
  0x0000000000000019 (INIT_ARRAY)         0x3e08
  0x000000000000001b (INIT_ARRAYSZ)       8 (bytes)
  0x000000000000001a (FINI_ARRAY)         0x3e10
  0x000000000000001c (FINI_ARRAYSZ)       8 (bytes)
  0x000000006ffffef5 (GNU_HASH)           0x2f0
  0x0000000000000005 (STRTAB)             0x520
  0x0000000000000006 (SYMTAB)             0x340
```

#### readelf --wide --notes {}

```diff
@@ -1,8 +1,8 @@
 
 Displaying notes found in: .note.gnu.property
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 feature: IBT, SHSTK
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 40d1c104864d36a37d538ab07ffff868d770f64a
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 55b563f5edb0298427cea5249818a28dbbf662a3
```

#### readelf --wide --debug-dump=frames {}

```diff
@@ -123,15 +123,15 @@
   DW_CFA_restore_state
 
 0000013c 0000000000000010 00000140 FDE cie=00000000 pc=00000000000015b0..00000000000015b9
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000150 000000000000004c 00000154 FDE cie=00000000 pc=00000000000015c0..0000000000001cb1
+00000150 000000000000004c 00000154 FDE cie=00000000 pc=00000000000015c0..0000000000001cee
   DW_CFA_advance_loc: 6 to 00000000000015c6
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
   DW_CFA_advance_loc: 2 to 00000000000015c8
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
   DW_CFA_advance_loc: 5 to 00000000000015cd
@@ -144,41 +144,41 @@
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
   DW_CFA_advance_loc: 1 to 00000000000015d1
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
   DW_CFA_advance_loc: 7 to 00000000000015d8
   DW_CFA_def_cfa_offset: 128
-  DW_CFA_advance_loc2: 1618 to 0000000000001c2a
+  DW_CFA_advance_loc2: 1654 to 0000000000001c4e
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 1 to 0000000000001c2b
+  DW_CFA_advance_loc: 1 to 0000000000001c4f
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 0000000000001c2c
+  DW_CFA_advance_loc: 1 to 0000000000001c50
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 0000000000001c2e
+  DW_CFA_advance_loc: 2 to 0000000000001c52
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 0000000000001c30
+  DW_CFA_advance_loc: 2 to 0000000000001c54
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 0000000000001c32
+  DW_CFA_advance_loc: 2 to 0000000000001c56
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 0000000000001c34
+  DW_CFA_advance_loc: 2 to 0000000000001c58
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 0000000000001c35
+  DW_CFA_advance_loc: 1 to 0000000000001c59
   DW_CFA_restore_state
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000001a0 0000000000000010 000001a4 FDE cie=00000000 pc=0000000000001cc0..0000000000001ce9
+000001a0 0000000000000010 000001a4 FDE cie=00000000 pc=0000000000001cf0..0000000000001d19
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-000001b4 0000000000000010 000001b8 FDE cie=00000000 pc=0000000000001cf0..0000000000001d16
+000001b4 0000000000000010 000001b8 FDE cie=00000000 pc=0000000000001d20..0000000000001d46
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
 000001c8 ZERO terminator
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -337,65 +337,65 @@
 	mov    %rdi,%r14
 	push   %r13
 	push   %r12
 	push   %rbp
 	push   %rbx
 	mov    %rsi,%rbx
 	sub    $0x48,%rsp
-	mov    %ecx,0x20(%rsp)
+	mov    %ecx,0x28(%rsp)
 	movslq %edx,%rcx
 	mov    %rcx,%rbp
-	mov    %edx,0x38(%rsp)
+	mov    %edx,0x1c(%rsp)
 	shl    $0x4,%rbp
 	mov    %rcx,0x8(%rsp)
 	mov    %rbp,%rdi
 	call   1160 <malloc@plt>
 	mov    %rbp,%rdi
 	mov    %rax,%r13
 	call   1160 <malloc@plt>
 	mov    0x8(%rsp),%rcx
 	mov    %rax,%r12
 	lea    0x0(,%rcx,4),%rdi
 	call   1160 <malloc@plt>
 	mov    0x8(%rsp),%rcx
 	mov    %rax,%rbp
 	lea    0x0(,%rcx,8),%rdx
-	mov    %rcx,0x18(%rsp)
+	mov    %rcx,0x20(%rsp)
 	mov    %rdx,%rdi
 	mov    %rdx,0x10(%rsp)
 	call   1160 <malloc@plt>
 	mov    0x10(%rsp),%rdi
 	mov    %rax,0x8(%rsp)
 	call   1160 <malloc@plt>
-	mov    0x38(%rsp),%edi
+	mov    0x1c(%rsp),%edi
 	mov    0x8(%rsp),%r8
 	mov    %rax,%r15
 	test   %edi,%edi
-	jle    1c51 <spearman+0x691>
+	jle    1c75 <spearman+0x6b5>
 	mov    0x10(%rsp),%rdx
 	mov    %r8,%rdi
 	mov    %r14,%rsi
 	call   1140 <memcpy@plt>
 	mov    0x10(%rsp),%rdx
 	mov    %rbx,%rsi
 	mov    %r15,%rdi
 	call   1140 <memcpy@plt>
 	mov    0x8(%rsp),%r8
 	xor    %edx,%edx
 	xor    %r10d,%r10d
-	mov    0x20(%rsp),%r9d
-	mov    0x18(%rsp),%rcx
+	mov    0x28(%rsp),%r9d
+	mov    0x20(%rsp),%rcx
 	xor    %eax,%eax
 	mov    $0xffffffff,%edi
 	mov    %r8,0x10(%rsp)
 	movsd  0x95c(%rip),%xmm1        
 	mov    $0xffffffff,%esi
 	mov    %r10d,%r8d
-	mov    %r9d,0x18(%rsp)
-	mov    0x38(%rsp),%r11d
+	mov    %r9d,0x20(%rsp)
+	mov    0x1c(%rsp),%r11d
 	mov    %edx,%r9d
 	jmp    1705 <spearman+0x145>
 	nopl   0x0(%rax,%rax,1)
 	lea    (%r11,%rdi,1),%edx
 	movsd  (%rbx,%rax,8),%xmm0
 	sub    $0x1,%edi
 	movslq %edx,%rdx
@@ -437,325 +437,327 @@
 	movsd  %xmm0,(%rdx)
 	cmp    %rax,%rcx
 	jne    1705 <spearman+0x145>
 	movslq %r8d,%rsi
 	mov    %r9d,0x8(%rsp)
 	mov    0x10(%rsp),%r8
 	mov    %r13,%rdi
-	mov    0x18(%rsp),%r9d
+	mov    0x20(%rsp),%r9d
 	mov    0x2879(%rip),%rcx        
 	mov    $0x10,%edx
 	mov    %esi,0x10(%rsp)
-	mov    %r8,0x28(%rsp)
-	mov    %r9d,0x20(%rsp)
+	mov    %r8,0x30(%rsp)
+	mov    %r9d,0x38(%rsp)
 	call   1100 <qsort@plt>
 	movslq 0x8(%rsp),%rsi
 	mov    $0x10,%edx
 	mov    %r12,%rdi
 	mov    0x284d(%rip),%rcx        
 	call   1100 <qsort@plt>
 	mov    0x10(%rsp),%eax
 	mov    0x8(%rsp),%ecx
 	cmp    %ecx,%eax
 	cmovle %eax,%ecx
 	movslq %ecx,%rdi
 	mov    %ecx,0x3c(%rsp)
 	shl    $0x2,%rdi
-	mov    %rdi,0x18(%rsp)
+	mov    %rdi,0x28(%rsp)
 	call   1160 <malloc@plt>
-	mov    0x18(%rsp),%rdi
-	mov    %rax,0x30(%rsp)
+	mov    0x28(%rsp),%rdi
+	mov    %rax,0x20(%rsp)
 	call   1160 <malloc@plt>
-	mov    0x20(%rsp),%r9d
-	mov    0x28(%rsp),%r8
-	mov    %rax,%rdi
+	mov    0x38(%rsp),%r9d
+	mov    0x30(%rsp),%r8
+	mov    %rax,0x28(%rsp)
 	test   %r9d,%r9d
-	jne    1920 <spearman+0x360>
+	jne    1930 <spearman+0x370>
 	mov    0x3c(%rsp),%ecx
 	mov    0x8(%rsp),%esi
-	mov    0x30(%rsp),%r11
 	test   %ecx,%ecx
 	setg   %al
 	test   %esi,%esi
 	mov    0x10(%rsp),%esi
 	setg   %dl
 	and    %eax,%edx
+	mov    %edx,%r10d
 	test   %esi,%esi
-	mov    %dl,0x18(%rsp)
-	jle    1caa <spearman+0x6ea>
+	jle    1ce7 <spearman+0x727>
 	test   %al,%al
-	je     1caa <spearman+0x6ea>
+	je     1ce7 <spearman+0x727>
 	lea    -0x1(%rsi),%eax
+	mov    0x20(%rsp),%rdi
 	xor    %edx,%edx
 	cltq
-	nop
 	mov    %rax,%rsi
 	shl    $0x4,%rsi
-	movslq 0x8(%r13,%rsi,1),%r10
-	movsd  (%rbx,%r10,8),%xmm0
-	mov    %r10,%rsi
+	movslq 0x8(%r13,%rsi,1),%r11
+	movsd  (%rbx,%r11,8),%xmm0
+	mov    %r11,%rsi
 	ucomisd %xmm0,%xmm0
 	jnp    1845 <spearman+0x285>
-	movslq %edx,%r10
+	movslq %edx,%r11
 	add    $0x1,%edx
-	mov    %esi,(%r11,%r10,4)
+	mov    %esi,(%rdi,%r11,4)
 	test   %eax,%eax
-	setg   %r10b
+	setg   %r11b
 	cmp    %ecx,%edx
 	setl   %sil
 	sub    $0x1,%rax
-	test   %sil,%r10b
+	test   %sil,%r11b
 	jne    1820 <spearman+0x260>
 	mov    0x8(%rsp),%eax
 	sub    $0x1,%eax
-	cmpb   $0x0,0x18(%rsp)
 	cltq
-	je     1c98 <spearman+0x6d8>
-	xchg   %ax,%ax
+	test   %r10b,%r10b
+	je     1cd4 <spearman+0x714>
+	mov    0x28(%rsp),%r10
+	nopl   0x0(%rax)
 	mov    %rax,%rsi
 	shl    $0x4,%rsi
-	movslq 0x8(%r12,%rsi,1),%r10
-	movsd  (%r14,%r10,8),%xmm0
-	mov    %r10,%rsi
+	movslq 0x8(%r12,%rsi,1),%rdi
+	movsd  (%r14,%rdi,8),%xmm0
+	mov    %rdi,%rsi
 	ucomisd %xmm0,%xmm0
-	jnp    1896 <spearman+0x2d6>
-	movslq %r9d,%r10
+	jnp    189e <spearman+0x2de>
+	movslq %r9d,%rdi
 	add    $0x1,%r9d
-	mov    %esi,(%rdi,%r10,4)
+	mov    %esi,(%r10,%rdi,4)
 	test   %eax,%eax
-	setg   %r10b
+	setg   %dil
 	cmp    %ecx,%r9d
 	setl   %sil
 	sub    $0x1,%rax
-	test   %sil,%r10b
-	jne    1870 <spearman+0x2b0>
+	test   %sil,%dil
+	jne    1878 <spearman+0x2b8>
 	test   %r9d,%r9d
-	je     1c98 <spearman+0x6d8>
+	je     1cd4 <spearman+0x714>
 	movslq %r9d,%rax
-	add    $0x1,%r9d
+	lea    0x1(%r9),%edi
+	mov    0x28(%rsp),%r9
 	nopl   0x0(%rax)
-	mov    %r9d,%esi
+	mov    %edi,%esi
 	pxor   %xmm0,%xmm0
-	movslq -0x4(%rdi,%rax,4),%rcx
+	movslq -0x4(%r9,%rax,4),%rcx
 	sub    %eax,%esi
 	sub    $0x1,%rax
 	cvtsi2sd %esi,%xmm0
 	movsd  %xmm0,(%r8,%rcx,8)
 	test   %eax,%eax
-	jne    18c0 <spearman+0x300>
-	mov    %r9d,%edi
+	jne    18d0 <spearman+0x310>
+	mov    %edi,%r10d
 	test   %edx,%edx
-	je     1c8b <spearman+0x6cb>
+	je     1cc7 <spearman+0x707>
+	mov    0x20(%rsp),%rdi
 	movslq %edx,%rax
 	lea    0x1(%rdx),%esi
-	nopl   0x0(%rax)
+	nopl   (%rax)
 	mov    %esi,%ecx
 	pxor   %xmm0,%xmm0
-	movslq -0x4(%r11,%rax,4),%rdx
+	movslq -0x4(%rdi,%rax,4),%rdx
 	sub    %eax,%ecx
 	sub    $0x1,%rax
 	cvtsi2sd %ecx,%xmm0
 	movsd  %xmm0,(%r15,%rdx,8)
 	test   %eax,%eax
-	jne    18f8 <spearman+0x338>
-	mov    %esi,0x18(%rsp)
-	jmp    192d <spearman+0x36d>
+	jne    1908 <spearman+0x348>
+	mov    %esi,0x38(%rsp)
+	jmp    193e <spearman+0x37e>
 	nopl   (%rax)
-	movl   $0x1,0x18(%rsp)
-	mov    $0x1,%edi
-	mov    0x38(%rsp),%eax
+	movl   $0x1,0x38(%rsp)
+	mov    $0x1,%r10d
+	mov    0x1c(%rsp),%eax
 	lea    -0x1(%rax),%ecx
 	xor    %eax,%eax
-	jmp    195f <spearman+0x39f>
-	nopl   0x0(%rax,%rax,1)
+	jmp    196f <spearman+0x3af>
+	nopl   0x0(%rax)
 	movsd  (%r8,%rax,8),%xmm0
 	xor    %edx,%edx
 	ucomisd %xmm0,%xmm0
 	setp   %dl
 	mov    %edx,0x0(%rbp,%rax,4)
 	lea    0x1(%rax),%rdx
 	cmp    %rax,%rcx
-	je     197c <spearman+0x3bc>
+	je     198c <spearman+0x3cc>
 	mov    %rdx,%rax
 	movsd  (%r15,%rax,8),%xmm0
 	ucomisd %xmm0,%xmm0
-	jnp    1940 <spearman+0x380>
+	jnp    1950 <spearman+0x390>
 	movl   $0x1,0x0(%rbp,%rax,4)
 	lea    0x1(%rax),%rdx
 	cmp    %rax,%rcx
-	jne    195c <spearman+0x39c>
+	jne    196c <spearman+0x3ac>
 	mov    0x10(%rsp),%edx
-	movsd  0x680(%rip),%xmm2        
+	movsd  0x670(%rip),%xmm2        
 	xor    %r11d,%r11d
 	test   %edx,%edx
-	je     1ab1 <spearman+0x4f1>
-	mov    %r12,0x20(%rsp)
+	je     1ac1 <spearman+0x501>
+	mov    %r12,0x30(%rsp)
 	mov    0x10(%rsp),%r12d
 	mov    %r15,0x10(%rsp)
-	mov    %edi,%r15d
-	jmp    19bd <spearman+0x3fd>
+	mov    %r10d,%r15d
+	jmp    19cd <spearman+0x40d>
 	nopw   0x0(%rax,%rax,1)
 	add    $0x1,%r11d
-	cmp    %r11d,%r12d
-	jle    1aa7 <spearman+0x4e7>
+	cmp    %r12d,%r11d
+	jge    1ab7 <spearman+0x4f7>
 	movslq %r11d,%rax
 	mov    %rax,%rdx
 	shl    $0x4,%rdx
 	add    %r13,%rdx
 	movslq 0x8(%rdx),%rcx
 	mov    0x0(%rbp,%rcx,4),%edi
 	test   %edi,%edi
-	jne    19b0 <spearman+0x3f0>
+	jne    19c0 <spearman+0x400>
 	movsd  (%r14,%rcx,8),%xmm0
 	mov    %r12d,%ecx
 	sub    %r11d,%ecx
 	test   %ecx,%ecx
-	jle    1c35 <spearman+0x675>
+	jle    1c59 <spearman+0x699>
 	lea    -0x1(%rcx),%r10d
 	xor    %r9d,%r9d
 	xor    %esi,%esi
 	add    %rax,%r10
 	mov    %rdx,%rax
 	shl    $0x4,%r10
 	add    %r13,%r10
-	jmp    1a15 <spearman+0x455>
+	jmp    1a25 <spearman+0x465>
 	nopw   0x0(%rax,%rax,1)
 	movslq 0x18(%rax),%rcx
 	add    $0x10,%rax
 	mov    0x0(%rbp,%rcx,4),%r9d
 	movslq 0x8(%rax),%rcx
 	test   %r9d,%r9d
-	jne    1a2b <spearman+0x46b>
+	jne    1a3b <spearman+0x47b>
 	ucomisd (%r14,%rcx,8),%xmm0
-	jp     1a30 <spearman+0x470>
-	jne    1a30 <spearman+0x470>
+	jp     1a40 <spearman+0x480>
+	jne    1a40 <spearman+0x480>
 	add    $0x1,%esi
 	cmp    %rax,%r10
-	jne    1a08 <spearman+0x448>
+	jne    1a18 <spearman+0x458>
 	lea    -0x1(%rsi),%r9d
 	pxor   %xmm0,%xmm0
 	pxor   %xmm1,%xmm1
 	cvtsi2sd %r9d,%xmm0
 	cvtsi2sd %r15d,%xmm1
 	add    %esi,%r15d
 	mulsd  %xmm2,%xmm0
 	addsd  %xmm1,%xmm0
 	test   %esi,%esi
-	je     1a97 <spearman+0x4d7>
+	je     1aa7 <spearman+0x4e7>
 	mov    %r11d,%eax
 	xor    %ecx,%ecx
-	jmp    1a88 <spearman+0x4c8>
+	jmp    1a98 <spearman+0x4d8>
 	nopl   0x0(%rax)
 	movslq %eax,%rcx
 	add    $0x1,%edi
 	add    $0x10,%rdx
 	add    $0x1,%eax
 	shl    $0x4,%rcx
 	movslq 0x8(%r13,%rcx,1),%rcx
 	movsd  %xmm0,(%r8,%rcx,8)
 	cmp    %esi,%edi
-	jge    1a97 <spearman+0x4d7>
+	jge    1aa7 <spearman+0x4e7>
 	movslq 0x8(%rdx),%rcx
 	mov    0x0(%rbp,%rcx,4),%ecx
 	test   %ecx,%ecx
-	je     1a60 <spearman+0x4a0>
+	je     1a70 <spearman+0x4b0>
 	add    $0x10,%rdx
 	add    $0x1,%eax
 	cmp    %edi,%esi
-	jg     1a80 <spearman+0x4c0>
+	jg     1a90 <spearman+0x4d0>
 	add    %r9d,%r11d
 	add    $0x1,%r11d
-	cmp    %r11d,%r12d
-	jg     19bd <spearman+0x3fd>
-	mov    0x20(%rsp),%r12
+	cmp    %r12d,%r11d
+	jl     19cd <spearman+0x40d>
+	mov    0x30(%rsp),%r12
 	mov    0x10(%rsp),%r15
 	mov    0x8(%rsp),%eax
-	movsd  0x54b(%rip),%xmm2        
+	movsd  0x53b(%rip),%xmm2        
 	xor    %r11d,%r11d
 	test   %eax,%eax
-	je     1bdc <spearman+0x61c>
+	je     1bec <spearman+0x62c>
 	mov    %r13,0x10(%rsp)
-	mov    0x18(%rsp),%r14d
+	mov    0x38(%rsp),%r14d
 	mov    0x8(%rsp),%r13d
-	jmp    1aed <spearman+0x52d>
+	jmp    1afd <spearman+0x53d>
 	nopl   0x0(%rax)
 	add    $0x1,%r11d
-	cmp    %r11d,%r13d
-	jle    1bd7 <spearman+0x617>
+	cmp    %r13d,%r11d
+	jge    1be7 <spearman+0x627>
 	movslq %r11d,%rax
 	mov    %rax,%rdx
 	shl    $0x4,%rdx
 	add    %r12,%rdx
 	movslq 0x8(%rdx),%rcx
 	mov    0x0(%rbp,%rcx,4),%edi
 	test   %edi,%edi
-	jne    1ae0 <spearman+0x520>
+	jne    1af0 <spearman+0x530>
 	movsd  (%rbx,%rcx,8),%xmm0
 	mov    %r13d,%ecx
 	sub    %r11d,%ecx
 	test   %ecx,%ecx
-	jle    1c43 <spearman+0x683>
+	jle    1c67 <spearman+0x6a7>
 	lea    -0x1(%rcx),%r10d
 	xor    %r9d,%r9d
 	xor    %esi,%esi
 	add    %rax,%r10
 	mov    %rdx,%rax
 	shl    $0x4,%r10
 	add    %r12,%r10
-	jmp    1b45 <spearman+0x585>
+	jmp    1b55 <spearman+0x595>
 	nopl   0x0(%rax)
 	movslq 0x18(%rax),%rcx
 	add    $0x10,%rax
 	mov    0x0(%rbp,%rcx,4),%r9d
 	movslq 0x8(%rax),%rcx
 	test   %r9d,%r9d
-	jne    1b5a <spearman+0x59a>
+	jne    1b6a <spearman+0x5aa>
 	ucomisd (%rbx,%rcx,8),%xmm0
-	jp     1b5f <spearman+0x59f>
-	jne    1b5f <spearman+0x59f>
+	jp     1b6f <spearman+0x5af>
+	jne    1b6f <spearman+0x5af>
 	add    $0x1,%esi
 	cmp    %r10,%rax
-	jne    1b38 <spearman+0x578>
+	jne    1b48 <spearman+0x588>
 	lea    -0x1(%rsi),%r9d
 	pxor   %xmm0,%xmm0
 	pxor   %xmm1,%xmm1
 	cvtsi2sd %r9d,%xmm0
 	cvtsi2sd %r14d,%xmm1
 	add    %esi,%r14d
 	mulsd  %xmm2,%xmm0
 	addsd  %xmm1,%xmm0
 	test   %esi,%esi
-	je     1bc7 <spearman+0x607>
+	je     1bd7 <spearman+0x617>
 	mov    %r11d,%eax
 	xor    %ecx,%ecx
-	jmp    1bb8 <spearman+0x5f8>
+	jmp    1bc8 <spearman+0x608>
 	nopl   0x0(%rax,%rax,1)
 	movslq %eax,%rcx
 	add    $0x1,%edi
 	add    $0x10,%rdx
 	add    $0x1,%eax
 	shl    $0x4,%rcx
 	movslq 0x8(%r12,%rcx,1),%rcx
 	movsd  %xmm0,(%r15,%rcx,8)
 	cmp    %esi,%edi
-	jge    1bc7 <spearman+0x607>
+	jge    1bd7 <spearman+0x617>
 	movslq 0x8(%rdx),%rcx
 	mov    0x0(%rbp,%rcx,4),%ecx
 	test   %ecx,%ecx
-	je     1b90 <spearman+0x5d0>
+	je     1ba0 <spearman+0x5e0>
 	add    $0x10,%rdx
 	add    $0x1,%eax
 	cmp    %edi,%esi
-	jg     1bb0 <spearman+0x5f0>
+	jg     1bc0 <spearman+0x600>
 	add    %r9d,%r11d
 	add    $0x1,%r11d
-	cmp    %r11d,%r13d
-	jg     1aed <spearman+0x52d>
+	cmp    %r13d,%r11d
+	jl     1afd <spearman+0x53d>
 	mov    0x10(%rsp),%r13
-	mov    0x38(%rsp),%edx
+	mov    0x1c(%rsp),%edx
 	mov    %r15,%rsi
 	mov    %r8,%rdi
 	mov    %r8,0x10(%rsp)
 	call   1120 <pearson@plt>
 	mov    %r13,%rdi
 	movsd  %xmm0,0x8(%rsp)
 	call   10f0 <free@plt>
@@ -763,55 +765,64 @@
 	call   10f0 <free@plt>
 	mov    0x10(%rsp),%rdi
 	call   10f0 <free@plt>
 	mov    %r15,%rdi
 	call   10f0 <free@plt>
 	mov    %rbp,%rdi
 	call   10f0 <free@plt>
+	mov    0x20(%rsp),%rdi
+	call   10f0 <free@plt>
+	mov    0x28(%rsp),%rdi
+	call   10f0 <free@plt>
 	movsd  0x8(%rsp),%xmm0
 	add    $0x48,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
 	ret
 	mov    $0xffffffff,%r9d
 	add    %r9d,%r11d
-	jmp    1a9a <spearman+0x4da>
+	jmp    1aaa <spearman+0x4ea>
 	mov    $0xffffffff,%r9d
 	add    %r9d,%r11d
-	jmp    1bca <spearman+0x60a>
+	jmp    1bda <spearman+0x61a>
 	mov    $0x10,%edx
 	xor    %esi,%esi
 	mov    %r13,%rdi
 	mov    %r8,0x8(%rsp)
-	mov    0x2381(%rip),%r14        
+	mov    0x235d(%rip),%r14        
 	mov    %r14,%rcx
 	call   1100 <qsort@plt>
 	mov    %r14,%rcx
 	mov    $0x10,%edx
 	xor    %esi,%esi
 	mov    %r12,%rdi
 	call   1100 <qsort@plt>
+	xor    %edi,%edi
+	call   1160 <malloc@plt>
+	xor    %edi,%edi
+	mov    %rax,0x20(%rsp)
+	call   1160 <malloc@plt>
 	mov    0x8(%rsp),%r8
-	jmp    1bdc <spearman+0x61c>
-	movl   $0x1,0x18(%rsp)
-	jmp    192d <spearman+0x36d>
+	mov    %rax,0x28(%rsp)
+	jmp    1bec <spearman+0x62c>
+	movl   $0x1,0x38(%rsp)
+	jmp    193e <spearman+0x37e>
 	test   %edx,%edx
-	je     1920 <spearman+0x360>
-	mov    $0x1,%edi
-	jmp    18eb <spearman+0x32b>
+	je     1930 <spearman+0x370>
+	mov    $0x1,%r10d
+	jmp    18fa <spearman+0x33a>
 	xor    %edx,%edx
 	jmp    185a <spearman+0x29a>
-	data16 cs nopw 0x0(%rax,%rax,1)
-	nopl   0x0(%rax)
+	xchg   %ax,%ax
 
-0000000000001cc0 <spearman_array>:
+0000000000001cf0 <spearman_array>:
 spearman_array():
 	endbr64
 	mov    %edx,%r9d
 	mov    %ecx,%edx
 	mov    %r8d,%ecx
 	imul   %edx,%r9d
 	imul   %edx,%esi
@@ -819,15 +830,15 @@
 	lea    (%rdi,%r9,8),%r8
 	movslq %esi,%rsi
 	lea    (%rdi,%rsi,8),%rdi
 	mov    %r8,%rsi
 	jmp    1150 <spearman@plt>
 	nopl   0x0(%rax)
 
-0000000000001cf0 <pearson_array>:
+0000000000001d20 <pearson_array>:
 pearson_array():
 	endbr64
 	mov    %edx,%r8d
 	imul   %ecx,%esi
 	mov    %ecx,%edx
 	imul   %ecx,%r8d
 	movslq %esi,%rsi
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.fini {}

```diff
@@ -1,11 +1,11 @@
 
 
 
 Disassembly of section .fini:
 
-0000000000001d18 <_fini>:
+0000000000001d48 <_fini>:
 _fini():
 	endbr64
 	sub    $0x8,%rsp
 	add    $0x8,%rsp
 	ret
```

#### readelf --wide --decompress --hex-dump=.eh_frame_hdr {}

```diff
@@ -2,10 +2,10 @@
 Hex dump of section '.eh_frame_hdr':
   0x00002010 011b033b 74000000 0d000000 10f0ffff ...;t...........
   0x00002020 90000000 d0f0ffff b8000000 e0f0ffff ................
   0x00002030 d0000000 50f2ffff e8000000 70f2ffff ....P.......p...
   0x00002040 fc000000 b0f2ffff 10010000 00f3ffff ................
   0x00002050 24010000 80f3ffff 38010000 f0f3ffff $.......8.......
   0x00002060 70010000 a0f5ffff b4010000 b0f5ffff p...............
-  0x00002070 c8010000 b0fcffff 18020000 e0fcffff ................
+  0x00002070 c8010000 e0fcffff 18020000 10fdffff ................
   0x00002080 2c020000                            ,...
```

#### readelf --wide --decompress --hex-dump=.eh_frame {}

```diff
@@ -17,16 +17,16 @@
   0x00002168 440e2883 054f0e30 02490e28 410e2041 D.(..O.0.I.(A. A
   0x00002178 0e18420e 10420e08 40000000 fc000000 ..B..B..@.......
   0x00002188 78f2ffff a2010000 00460e10 8f02450e x........F....E.
   0x00002198 188e0345 0e208d04 420e288c 05410e30 ...E. ..B.(..A.0
   0x000021a8 8606460e 50036401 0a0e3041 0e28420e ..F.P.d...0A.(B.
   0x000021b8 20420e18 420e1042 0e084a0b 10000000  B..B..B..J.....
   0x000021c8 40010000 e4f3ffff 09000000 00000000 @...............
-  0x000021d8 4c000000 54010000 e0f3ffff f1060000 L...T...........
+  0x000021d8 4c000000 54010000 e0f3ffff 2e070000 L...T...........
   0x000021e8 00460e10 8f02420e 188e0345 0e208d04 .F....B....E. ..
   0x000021f8 420e288c 05410e30 8606410e 38830747 B.(..A.0..A.8..G
-  0x00002208 0e800103 52060a0e 38410e30 410e2842 ....R...8A.0A.(B
+  0x00002208 0e800103 76060a0e 38410e30 410e2842 ....v...8A.0A.(B
   0x00002218 0e20420e 18420e10 420e0841 0b000000 . B..B..B..A....
-  0x00002228 10000000 a4010000 90faffff 29000000 ............)...
-  0x00002238 00000000 10000000 b8010000 acfaffff ................
+  0x00002228 10000000 a4010000 c0faffff 29000000 ............)...
+  0x00002238 00000000 10000000 b8010000 dcfaffff ................
   0x00002248 26000000 00000000 00000000          &...........
```

### Comparing `bmxp-0.0.8/bmxp/gravity/gravity_example.py` & `bmxp-0.0.9/bmxp/gravity/gravity_example.py`

 * *Files identical despite different names*

### Comparing `bmxp-0.0.8/bmxp.egg-info/PKG-INFO` & `bmxp-0.0.9/bmxp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmxp
-Version: 0.0.8
+Version: 0.0.9
 Summary: LCMS Processing tools used by the Metabolomics Platform at the Broad Institute.
 Home-page: https://github.com/broadinstitute/bmxp
 Author: Daniel S. Hitchcock
 Author-email: daniel.s.hitchcock@gmail.com
 License: MIT
 Keywords: LCMS,Alignment,Processing,Metabolomics,Clustering
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bmxp-0.0.8/bmxp.egg-info/SOURCES.txt` & `bmxp-0.0.9/bmxp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bmxp-0.0.8/setup.py` & `bmxp-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 with open(os.path.join(HERE, "requirements.txt"), encoding="utf-8") as f:
     REQUIREMENTS = f.read()
 
 module1 = Extension
 setup(
     name="bmxp",
     install_requires=REQUIREMENTS.split("\n"),
-    version="0.0.8",
+    version="0.0.9",
     description="LCMS Processing tools used by the Metabolomics Platform at the Broad"
     " Institute.",
     packages=find_namespace_packages(include=["bmxp.*"]),
     license="MIT",
     author="Daniel S. Hitchcock",
     author_email="daniel.s.hitchcock@gmail.com",
     long_description_content_type="text/markdown",
```

### Comparing `bmxp-0.0.8/tests/__pycache__/test_mseclipse.cpython-38-pytest-7.1.2.pyc` & `bmxp-0.0.9/tests/__pycache__/test_mseclipse.cpython-38-pytest-7.1.2.pyc`

 * *Files identical despite different names*

### Comparing `bmxp-0.0.8/tests/example1.csv` & `bmxp-0.0.9/tests/example1.csv`

 * *Files identical despite different names*

### Comparing `bmxp-0.0.8/tests/mseclipse.pickle` & `bmxp-0.0.9/tests/mseclipse.pickle`

 * *Files identical despite different names*

### Comparing `bmxp-0.0.8/tests/test1.csv` & `bmxp-0.0.9/tests/test1.csv`

 * *Files identical despite different names*

### Comparing `bmxp-0.0.8/tests/test2.csv` & `bmxp-0.0.9/tests/test2.csv`

 * *Files identical despite different names*

### Comparing `bmxp-0.0.8/tests/test3.csv` & `bmxp-0.0.9/tests/test3.csv`

 * *Files identical despite different names*

### Comparing `bmxp-0.0.8/tests/test_gravity.csv` & `bmxp-0.0.9/tests/test_gravity.csv`

 * *Files identical despite different names*

### Comparing `bmxp-0.0.8/tests/test_gravity.py` & `bmxp-0.0.9/tests/test_gravity.py`

 * *Files identical despite different names*

### Comparing `bmxp-0.0.8/tests/test_mseclipse.py` & `bmxp-0.0.9/tests/test_mseclipse.py`

 * *Files identical despite different names*

