# Comparing `tmp/vicedtools-0.0.8.tar.gz` & `tmp/vicedtools-0.0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vicedtools-0.0.8.tar", last modified: Fri Apr 14 07:48:37 2023, max compression
+gzip compressed data, was "vicedtools-0.0.8.1.tar", last modified: Fri Apr 14 16:38:57 2023, max compression
```

## Comparing `vicedtools-0.0.8.tar` & `vicedtools-0.0.8.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 07:48:37.799431 vicedtools-0.0.8/
--rw-rw-rw-   0        0        0    11558 2021-05-29 17:10:03.000000 vicedtools-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     5210 2023-04-14 07:48:37.799431 vicedtools-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     4636 2023-04-14 07:45:30.000000 vicedtools-0.0.8/README.md
--rw-rw-rw-   0        0        0      108 2021-05-29 17:13:52.000000 vicedtools-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0      860 2023-04-14 07:48:37.831735 vicedtools-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     3857 2023-04-14 06:14:58.000000 vicedtools-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 07:48:37.231913 vicedtools-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-04-14 07:48:37.334756 vicedtools-0.0.8/src/vicedtools/
--rw-rw-rw-   0        0        0     1498 2023-04-13 17:39:10.000000 vicedtools-0.0.8/src/vicedtools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 07:48:37.550889 vicedtools-0.0.8/src/vicedtools/acer/
--rw-rw-rw-   0        0        0     1341 2023-04-13 17:39:11.000000 vicedtools-0.0.8/src/vicedtools/acer/__init__.py
--rw-rw-rw-   0        0        0     4191 2023-04-13 17:39:10.000000 vicedtools-0.0.8/src/vicedtools/acer/ewritesittings.py
--rw-rw-rw-   0        0        0     1188 2023-04-13 17:39:10.000000 vicedtools-0.0.8/src/vicedtools/acer/extraoarsauthenticators.py
--rw-rw-rw-   0        0        0     7223 2023-04-13 17:39:10.000000 vicedtools-0.0.8/src/vicedtools/acer/oars.py
--rw-rw-rw-   0        0        0     2269 2023-04-13 17:39:10.000000 vicedtools-0.0.8/src/vicedtools/acer/oarsauthenticators.py
--rw-rw-rw-   0        0        0     4902 2023-04-13 17:39:10.000000 vicedtools-0.0.8/src/vicedtools/acer/oarscandidates.py
--rw-rw-rw-   0        0        0    16115 2023-04-13 17:39:10.000000 vicedtools-0.0.8/src/vicedtools/acer/oarssession.py
--rw-rw-rw-   0        0        0     5368 2023-04-13 17:39:10.000000 vicedtools-0.0.8/src/vicedtools/acer/oarstests.py
--rw-rw-rw-   0        0        0     1878 2023-04-13 17:39:10.000000 vicedtools-0.0.8/src/vicedtools/acer/patitems.py
--rw-rw-rw-   0        0        0    15529 2023-04-13 17:39:10.000000 vicedtools-0.0.8/src/vicedtools/acer/patresults.py
--rw-rw-rw-   0        0        0     6964 2023-04-13 17:39:10.000000 vicedtools-0.0.8/src/vicedtools/acer/patsittings.py
--rw-rw-rw-   0        0        0    21888 2023-04-13 17:39:11.000000 vicedtools-0.0.8/src/vicedtools/acer/plots.py
-drwxrwxrwx   0        0        0        0 2023-04-14 07:48:37.618889 vicedtools-0.0.8/src/vicedtools/compass/
--rw-rw-rw-   0        0        0      982 2023-04-13 17:44:21.000000 vicedtools-0.0.8/src/vicedtools/compass/__init__.py
--rw-rw-rw-   0        0        0     4384 2023-04-13 17:44:21.000000 vicedtools-0.0.8/src/vicedtools/compass/compassauthenticators.py
--rw-rw-rw-   0        0        0    19553 2023-04-13 17:44:21.000000 vicedtools-0.0.8/src/vicedtools/compass/compasssession.py
--rw-rw-rw-   0        0        0     1113 2023-04-13 17:44:21.000000 vicedtools-0.0.8/src/vicedtools/compass/extraauthenticators.py
--rw-rw-rw-   0        0        0    18015 2023-04-13 17:44:21.000000 vicedtools-0.0.8/src/vicedtools/compass/reports.py
--rw-rw-rw-   0        0        0     3645 2023-04-13 17:39:10.000000 vicedtools-0.0.8/src/vicedtools/educationperfect.py
-drwxrwxrwx   0        0        0        0 2023-04-14 07:48:37.683796 vicedtools-0.0.8/src/vicedtools/gcp/
--rw-rw-rw-   0        0        0     1338 2023-04-13 17:39:11.000000 vicedtools-0.0.8/src/vicedtools/gcp/__init__.py
--rw-rw-rw-   0        0        0     2725 2023-04-13 17:39:11.000000 vicedtools-0.0.8/src/vicedtools/gcp/api.py
--rw-rw-rw-   0        0        0     2042 2023-04-13 17:39:11.000000 vicedtools-0.0.8/src/vicedtools/gcp/format.py
--rw-rw-rw-   0        0        0     6566 2023-04-13 17:39:11.000000 vicedtools-0.0.8/src/vicedtools/gcp/schema.py
-drwxrwxrwx   0        0        0        0 2023-04-14 07:48:37.733900 vicedtools-0.0.8/src/vicedtools/naplan/
--rw-rw-rw-   0        0        0      815 2023-04-13 17:39:12.000000 vicedtools-0.0.8/src/vicedtools/naplan/__init__.py
--rw-rw-rw-   0        0        0     5815 2023-04-13 17:39:11.000000 vicedtools-0.0.8/src/vicedtools/naplan/dataservicesession.py
--rw-rw-rw-   0        0        0     6193 2023-04-14 07:39:34.000000 vicedtools-0.0.8/src/vicedtools/naplan/sssrdata.py
--rw-rw-rw-   0        0        0     2004 2023-04-13 17:39:10.000000 vicedtools-0.0.8/src/vicedtools/sportstrak.py
-drwxrwxrwx   0        0        0        0 2023-04-14 07:48:37.797145 vicedtools-0.0.8/src/vicedtools/vce/
--rw-rw-rw-   0        0        0      798 2023-04-13 17:39:14.000000 vicedtools-0.0.8/src/vicedtools/vce/__init__.py
--rw-rw-rw-   0        0        0     3020 2023-04-13 17:39:13.000000 vicedtools-0.0.8/src/vicedtools/vce/schoolscores.py
--rw-rw-rw-   0        0        0    34328 2023-04-13 17:39:13.000000 vicedtools-0.0.8/src/vicedtools/vce/vasssession.py
-drwxrwxrwx   0        0        0        0 2023-04-14 07:48:37.425447 vicedtools-0.0.8/src/vicedtools.egg-info/
--rw-rw-rw-   0        0        0     5210 2023-04-14 07:48:37.000000 vicedtools-0.0.8/src/vicedtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1326 2023-04-14 07:48:37.000000 vicedtools-0.0.8/src/vicedtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 07:48:37.000000 vicedtools-0.0.8/src/vicedtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     3162 2023-04-14 07:48:37.000000 vicedtools-0.0.8/src/vicedtools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      118 2023-04-14 07:48:37.000000 vicedtools-0.0.8/src/vicedtools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-14 07:48:37.000000 vicedtools-0.0.8/src/vicedtools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 16:38:56.996809 vicedtools-0.0.8.1/
+-rw-rw-rw-   0        0        0    11558 2021-05-29 17:10:03.000000 vicedtools-0.0.8.1/LICENSE
+-rw-rw-rw-   0        0        0     5212 2023-04-14 16:38:56.996809 vicedtools-0.0.8.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4636 2023-04-14 07:45:30.000000 vicedtools-0.0.8.1/README.md
+-rw-rw-rw-   0        0        0      108 2021-05-29 17:13:52.000000 vicedtools-0.0.8.1/pyproject.toml
+-rw-rw-rw-   0        0        0      863 2023-04-14 16:38:56.999809 vicedtools-0.0.8.1/setup.cfg
+-rw-rw-rw-   0        0        0     3857 2023-04-14 06:14:58.000000 vicedtools-0.0.8.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 16:38:56.774253 vicedtools-0.0.8.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-14 16:38:56.801418 vicedtools-0.0.8.1/src/vicedtools/
+-rw-rw-rw-   0        0        0     1498 2023-04-13 17:39:10.000000 vicedtools-0.0.8.1/src/vicedtools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 16:38:56.900111 vicedtools-0.0.8.1/src/vicedtools/acer/
+-rw-rw-rw-   0        0        0     1341 2023-04-13 17:39:11.000000 vicedtools-0.0.8.1/src/vicedtools/acer/__init__.py
+-rw-rw-rw-   0        0        0     4191 2023-04-13 17:39:10.000000 vicedtools-0.0.8.1/src/vicedtools/acer/ewritesittings.py
+-rw-rw-rw-   0        0        0     1188 2023-04-13 17:39:10.000000 vicedtools-0.0.8.1/src/vicedtools/acer/extraoarsauthenticators.py
+-rw-rw-rw-   0        0        0     7223 2023-04-13 17:39:10.000000 vicedtools-0.0.8.1/src/vicedtools/acer/oars.py
+-rw-rw-rw-   0        0        0     2269 2023-04-13 17:39:10.000000 vicedtools-0.0.8.1/src/vicedtools/acer/oarsauthenticators.py
+-rw-rw-rw-   0        0        0     4902 2023-04-13 17:39:10.000000 vicedtools-0.0.8.1/src/vicedtools/acer/oarscandidates.py
+-rw-rw-rw-   0        0        0    16115 2023-04-13 17:39:10.000000 vicedtools-0.0.8.1/src/vicedtools/acer/oarssession.py
+-rw-rw-rw-   0        0        0     5368 2023-04-13 17:39:10.000000 vicedtools-0.0.8.1/src/vicedtools/acer/oarstests.py
+-rw-rw-rw-   0        0        0     1878 2023-04-13 17:39:10.000000 vicedtools-0.0.8.1/src/vicedtools/acer/patitems.py
+-rw-rw-rw-   0        0        0    15529 2023-04-13 17:39:10.000000 vicedtools-0.0.8.1/src/vicedtools/acer/patresults.py
+-rw-rw-rw-   0        0        0     6964 2023-04-13 17:39:10.000000 vicedtools-0.0.8.1/src/vicedtools/acer/patsittings.py
+-rw-rw-rw-   0        0        0    21888 2023-04-13 17:39:11.000000 vicedtools-0.0.8.1/src/vicedtools/acer/plots.py
+drwxrwxrwx   0        0        0        0 2023-04-14 16:38:56.926357 vicedtools-0.0.8.1/src/vicedtools/compass/
+-rw-rw-rw-   0        0        0      982 2023-04-13 17:44:21.000000 vicedtools-0.0.8.1/src/vicedtools/compass/__init__.py
+-rw-rw-rw-   0        0        0     4384 2023-04-13 17:44:21.000000 vicedtools-0.0.8.1/src/vicedtools/compass/compassauthenticators.py
+-rw-rw-rw-   0        0        0    19553 2023-04-13 17:44:21.000000 vicedtools-0.0.8.1/src/vicedtools/compass/compasssession.py
+-rw-rw-rw-   0        0        0     1113 2023-04-13 17:44:21.000000 vicedtools-0.0.8.1/src/vicedtools/compass/extraauthenticators.py
+-rw-rw-rw-   0        0        0    18167 2023-04-14 16:23:35.000000 vicedtools-0.0.8.1/src/vicedtools/compass/reports.py
+-rw-rw-rw-   0        0        0     3645 2023-04-13 17:39:10.000000 vicedtools-0.0.8.1/src/vicedtools/educationperfect.py
+drwxrwxrwx   0        0        0        0 2023-04-14 16:38:56.947019 vicedtools-0.0.8.1/src/vicedtools/gcp/
+-rw-rw-rw-   0        0        0     1338 2023-04-13 17:39:11.000000 vicedtools-0.0.8.1/src/vicedtools/gcp/__init__.py
+-rw-rw-rw-   0        0        0     2725 2023-04-13 17:39:11.000000 vicedtools-0.0.8.1/src/vicedtools/gcp/api.py
+-rw-rw-rw-   0        0        0     2042 2023-04-13 17:39:11.000000 vicedtools-0.0.8.1/src/vicedtools/gcp/format.py
+-rw-rw-rw-   0        0        0     6566 2023-04-13 17:39:11.000000 vicedtools-0.0.8.1/src/vicedtools/gcp/schema.py
+drwxrwxrwx   0        0        0        0 2023-04-14 16:38:56.972019 vicedtools-0.0.8.1/src/vicedtools/naplan/
+-rw-rw-rw-   0        0        0      815 2023-04-13 17:39:12.000000 vicedtools-0.0.8.1/src/vicedtools/naplan/__init__.py
+-rw-rw-rw-   0        0        0     5815 2023-04-13 17:39:11.000000 vicedtools-0.0.8.1/src/vicedtools/naplan/dataservicesession.py
+-rw-rw-rw-   0        0        0     6193 2023-04-14 07:39:34.000000 vicedtools-0.0.8.1/src/vicedtools/naplan/sssrdata.py
+-rw-rw-rw-   0        0        0     2004 2023-04-13 17:39:10.000000 vicedtools-0.0.8.1/src/vicedtools/sportstrak.py
+drwxrwxrwx   0        0        0        0 2023-04-14 16:38:56.994086 vicedtools-0.0.8.1/src/vicedtools/vce/
+-rw-rw-rw-   0        0        0      798 2023-04-13 17:39:14.000000 vicedtools-0.0.8.1/src/vicedtools/vce/__init__.py
+-rw-rw-rw-   0        0        0     3020 2023-04-13 17:39:13.000000 vicedtools-0.0.8.1/src/vicedtools/vce/schoolscores.py
+-rw-rw-rw-   0        0        0    34328 2023-04-13 17:39:13.000000 vicedtools-0.0.8.1/src/vicedtools/vce/vasssession.py
+drwxrwxrwx   0        0        0        0 2023-04-14 16:38:56.849317 vicedtools-0.0.8.1/src/vicedtools.egg-info/
+-rw-rw-rw-   0        0        0     5212 2023-04-14 16:38:56.000000 vicedtools-0.0.8.1/src/vicedtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1326 2023-04-14 16:38:56.000000 vicedtools-0.0.8.1/src/vicedtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 16:38:56.000000 vicedtools-0.0.8.1/src/vicedtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     3162 2023-04-14 16:38:56.000000 vicedtools-0.0.8.1/src/vicedtools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      119 2023-04-14 16:38:56.000000 vicedtools-0.0.8.1/src/vicedtools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-14 16:38:56.000000 vicedtools-0.0.8.1/src/vicedtools.egg-info/top_level.txt
```

### Comparing `vicedtools-0.0.8/LICENSE` & `vicedtools-0.0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8/PKG-INFO` & `vicedtools-0.0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vicedtools
-Version: 0.0.8
+Version: 0.0.8.1
 Summary: A collection of tools for school data in Victorian schools.
 Home-page: https://github.com/gregbreese/vicedtools
 Author: Greg Breese
 Project-URL: Bug Tracker, https://github.com/gregbreese/vicedtools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `vicedtools-0.0.8/README.md` & `vicedtools-0.0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8/setup.cfg` & `vicedtools-0.0.8.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6963 6564 746f 6f6c 730d 0a76   = vicedtools..v
-00000020: 6572 7369 6f6e 203d 2030 2e30 2e38 0d0a  ersion = 0.0.8..
-00000030: 6175 7468 6f72 203d 2047 7265 6720 4272  author = Greg Br
-00000040: 6565 7365 0d0a 6465 7363 7269 7074 696f  eese..descriptio
-00000050: 6e20 3d20 4120 636f 6c6c 6563 7469 6f6e  n = A collection
-00000060: 206f 6620 746f 6f6c 7320 666f 7220 7363   of tools for sc
-00000070: 686f 6f6c 2064 6174 6120 696e 2056 6963  hool data in Vic
-00000080: 746f 7269 616e 2073 6368 6f6f 6c73 2e0d  torian schools..
-00000090: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
-000000a0: 6e20 3d20 6669 6c65 3a20 5245 4144 4d45  n = file: README
-000000b0: 2e6d 640d 0a6c 6f6e 675f 6465 7363 7269  .md..long_descri
-000000c0: 7074 696f 6e5f 636f 6e74 656e 745f 7479  ption_content_ty
-000000d0: 7065 203d 2074 6578 742f 6d61 726b 646f  pe = text/markdo
-000000e0: 776e 0d0a 7572 6c20 3d20 6874 7470 733a  wn..url = https:
-000000f0: 2f2f 6769 7468 7562 2e63 6f6d 2f67 7265  //github.com/gre
-00000100: 6762 7265 6573 652f 7669 6365 6474 6f6f  gbreese/vicedtoo
-00000110: 6c73 0d0a 7072 6f6a 6563 745f 7572 6c73  ls..project_urls
-00000120: 203d 200d 0a09 4275 6720 5472 6163 6b65   = ...Bug Tracke
-00000130: 7220 3d20 6874 7470 733a 2f2f 6769 7468  r = https://gith
-00000140: 7562 2e63 6f6d 2f67 7265 6762 7265 6573  ub.com/gregbrees
-00000150: 652f 7669 6365 6474 6f6f 6c73 2f69 7373  e/vicedtools/iss
-00000160: 7565 730d 0a63 6c61 7373 6966 6965 7273  ues..classifiers
-00000170: 203d 200d 0a09 5072 6f67 7261 6d6d 696e   = ...Programmin
-00000180: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000190: 7468 6f6e 203a 3a20 330d 0a09 4c69 6365  thon :: 3...Lice
-000001a0: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
-000001b0: 7665 6420 3a3a 2041 7061 6368 6520 536f  ved :: Apache So
-000001c0: 6674 7761 7265 204c 6963 656e 7365 0d0a  ftware License..
-000001d0: 094f 7065 7261 7469 6e67 2053 7973 7465  .Operating Syste
-000001e0: 6d20 3a3a 204f 5320 496e 6465 7065 6e64  m :: OS Independ
-000001f0: 656e 740d 0a09 4465 7665 6c6f 706d 656e  ent...Developmen
-00000200: 7420 5374 6174 7573 203a 3a20 3320 2d20  t Status :: 3 - 
-00000210: 416c 7068 610d 0a0d 0a5b 6f70 7469 6f6e  Alpha....[option
-00000220: 735d 0d0a 7061 636b 6167 655f 6469 7220  s]..package_dir 
-00000230: 3d20 0d0a 093d 2073 7263 0d0a 7061 636b  = ...= src..pack
-00000240: 6167 6573 203d 2066 696e 643a 0d0a 7079  ages = find:..py
-00000250: 7468 6f6e 5f72 6571 7569 7265 7320 3d20  thon_requires = 
-00000260: 3e3d 332e 380d 0a69 6e73 7461 6c6c 5f72  >=3.8..install_r
-00000270: 6571 7569 7265 7320 3d20 0d0a 0962 726f  equires = ...bro
-00000280: 7773 6572 5f63 6f6f 6b69 6533 0d0a 0962  wser_cookie3...b
-00000290: 7334 0d0a 0964 656d 6a73 6f6e 0d0a 0967  s4...demjson...g
-000002a0: 6f6f 676c 652d 636c 6f75 642d 6269 6771  oogle-cloud-bigq
-000002b0: 7565 7279 0d0a 0967 6f6f 676c 652d 636c  uery...google-cl
-000002c0: 6f75 642d 7374 6f72 6167 650d 0a09 6d61  oud-storage...ma
-000002d0: 7470 6c6f 746c 6962 0d0a 096e 756d 7079  tplotlib...numpy
-000002e0: 0d0a 0970 616e 6461 730d 0a09 7365 6162  ...pandas...seab
-000002f0: 6f72 6e0d 0a09 7365 6c65 6e69 756d 0d0a  orn...selenium..
-00000300: 0974 6f6d 6c69 0d0a 0d0a 5b6f 7074 696f  .tomli....[optio
-00000310: 6e73 2e70 6163 6b61 6765 732e 6669 6e64  ns.packages.find
-00000320: 5d0d 0a77 6865 7265 203d 2073 7263 0d0a  ]..where = src..
-00000330: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
-00000340: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
-00000350: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
+00000020: 6572 7369 6f6e 203d 2030 2e30 2e38 2e31  ersion = 0.0.8.1
+00000030: 0d0a 6175 7468 6f72 203d 2047 7265 6720  ..author = Greg 
+00000040: 4272 6565 7365 0d0a 6465 7363 7269 7074  Breese..descript
+00000050: 696f 6e20 3d20 4120 636f 6c6c 6563 7469  ion = A collecti
+00000060: 6f6e 206f 6620 746f 6f6c 7320 666f 7220  on of tools for 
+00000070: 7363 686f 6f6c 2064 6174 6120 696e 2056  school data in V
+00000080: 6963 746f 7269 616e 2073 6368 6f6f 6c73  ictorian schools
+00000090: 2e0d 0a6c 6f6e 675f 6465 7363 7269 7074  ...long_descript
+000000a0: 696f 6e20 3d20 6669 6c65 3a20 5245 4144  ion = file: READ
+000000b0: 4d45 2e6d 640d 0a6c 6f6e 675f 6465 7363  ME.md..long_desc
+000000c0: 7269 7074 696f 6e5f 636f 6e74 656e 745f  ription_content_
+000000d0: 7479 7065 203d 2074 6578 742f 6d61 726b  type = text/mark
+000000e0: 646f 776e 0d0a 7572 6c20 3d20 6874 7470  down..url = http
+000000f0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f67  s://github.com/g
+00000100: 7265 6762 7265 6573 652f 7669 6365 6474  regbreese/vicedt
+00000110: 6f6f 6c73 0d0a 7072 6f6a 6563 745f 7572  ools..project_ur
+00000120: 6c73 203d 200d 0a09 4275 6720 5472 6163  ls = ...Bug Trac
+00000130: 6b65 7220 3d20 6874 7470 733a 2f2f 6769  ker = https://gi
+00000140: 7468 7562 2e63 6f6d 2f67 7265 6762 7265  thub.com/gregbre
+00000150: 6573 652f 7669 6365 6474 6f6f 6c73 2f69  ese/vicedtools/i
+00000160: 7373 7565 730d 0a63 6c61 7373 6966 6965  ssues..classifie
+00000170: 7273 203d 200d 0a09 5072 6f67 7261 6d6d  rs = ...Programm
+00000180: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000190: 5079 7468 6f6e 203a 3a20 330d 0a09 4c69  Python :: 3...Li
+000001a0: 6365 6e73 6520 3a3a 204f 5349 2041 7070  cense :: OSI App
+000001b0: 726f 7665 6420 3a3a 2041 7061 6368 6520  roved :: Apache 
+000001c0: 536f 6674 7761 7265 204c 6963 656e 7365  Software License
+000001d0: 0d0a 094f 7065 7261 7469 6e67 2053 7973  ...Operating Sys
+000001e0: 7465 6d20 3a3a 204f 5320 496e 6465 7065  tem :: OS Indepe
+000001f0: 6e64 656e 740d 0a09 4465 7665 6c6f 706d  ndent...Developm
+00000200: 656e 7420 5374 6174 7573 203a 3a20 3320  ent Status :: 3 
+00000210: 2d20 416c 7068 610d 0a0d 0a5b 6f70 7469  - Alpha....[opti
+00000220: 6f6e 735d 0d0a 7061 636b 6167 655f 6469  ons]..package_di
+00000230: 7220 3d20 0d0a 093d 2073 7263 0d0a 7061  r = ...= src..pa
+00000240: 636b 6167 6573 203d 2066 696e 643a 0d0a  ckages = find:..
+00000250: 7079 7468 6f6e 5f72 6571 7569 7265 7320  python_requires 
+00000260: 3d20 3e3d 332e 380d 0a69 6e73 7461 6c6c  = >=3.8..install
+00000270: 5f72 6571 7569 7265 7320 3d20 0d0a 0962  _requires = ...b
+00000280: 726f 7773 6572 5f63 6f6f 6b69 6533 0d0a  rowser_cookie3..
+00000290: 0962 7334 0d0a 0964 656d 6a73 6f6e 330d  .bs4...demjson3.
+000002a0: 0a09 676f 6f67 6c65 2d63 6c6f 7564 2d62  ..google-cloud-b
+000002b0: 6967 7175 6572 790d 0a09 676f 6f67 6c65  igquery...google
+000002c0: 2d63 6c6f 7564 2d73 746f 7261 6765 0d0a  -cloud-storage..
+000002d0: 096d 6174 706c 6f74 6c69 620d 0a09 6e75  .matplotlib...nu
+000002e0: 6d70 790d 0a09 7061 6e64 6173 0d0a 0973  mpy...pandas...s
+000002f0: 6561 626f 726e 0d0a 0973 656c 656e 6975  eaborn...seleniu
+00000300: 6d0d 0a09 746f 6d6c 690d 0a0d 0a5b 6f70  m...tomli....[op
+00000310: 7469 6f6e 732e 7061 636b 6167 6573 2e66  tions.packages.f
+00000320: 696e 645d 0d0a 7768 6572 6520 3d20 7372  ind]..where = sr
+00000330: 630d 0a0d 0a5b 6567 675f 696e 666f 5d0d  c....[egg_info].
+00000340: 0a74 6167 5f62 7569 6c64 203d 200d 0a74  .tag_build = ..t
+00000350: 6167 5f64 6174 6520 3d20 300d 0a0d 0a    ag_date = 0....
```

### Comparing `vicedtools-0.0.8/setup.py` & `vicedtools-0.0.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8/src/vicedtools/__init__.py` & `vicedtools-0.0.8.1/src/vicedtools/__init__.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8/src/vicedtools/acer/__init__.py` & `vicedtools-0.0.8.1/src/vicedtools/acer/__init__.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8/src/vicedtools/acer/ewritesittings.py` & `vicedtools-0.0.8.1/src/vicedtools/acer/ewritesittings.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8/src/vicedtools/acer/extraoarsauthenticators.py` & `vicedtools-0.0.8.1/src/vicedtools/acer/extraoarsauthenticators.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8/src/vicedtools/acer/oars.py` & `vicedtools-0.0.8.1/src/vicedtools/acer/oars.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8/src/vicedtools/acer/oarsauthenticators.py` & `vicedtools-0.0.8.1/src/vicedtools/acer/oarsauthenticators.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8/src/vicedtools/acer/oarscandidates.py` & `vicedtools-0.0.8.1/src/vicedtools/acer/oarscandidates.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8/src/vicedtools/acer/oarssession.py` & `vicedtools-0.0.8.1/src/vicedtools/acer/oarssession.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8/src/vicedtools/acer/oarstests.py` & `vicedtools-0.0.8.1/src/vicedtools/acer/oarstests.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8/src/vicedtools/acer/patitems.py` & `vicedtools-0.0.8.1/src/vicedtools/acer/patitems.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8/src/vicedtools/acer/patresults.py` & `vicedtools-0.0.8.1/src/vicedtools/acer/patresults.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8/src/vicedtools/acer/patsittings.py` & `vicedtools-0.0.8.1/src/vicedtools/acer/patsittings.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8/src/vicedtools/acer/plots.py` & `vicedtools-0.0.8.1/src/vicedtools/acer/plots.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8/src/vicedtools/compass/__init__.py` & `vicedtools-0.0.8.1/src/vicedtools/compass/__init__.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8/src/vicedtools/compass/compassauthenticators.py` & `vicedtools-0.0.8.1/src/vicedtools/compass/compassauthenticators.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8/src/vicedtools/compass/compasssession.py` & `vicedtools-0.0.8.1/src/vicedtools/compass/compasssession.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8/src/vicedtools/compass/extraauthenticators.py` & `vicedtools-0.0.8.1/src/vicedtools/compass/extraauthenticators.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8/src/vicedtools/compass/reports.py` & `vicedtools-0.0.8.1/src/vicedtools/compass/reports.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,15 +135,15 @@
         return cls(temp_df[columns])
 
     @classmethod
     def fromLearningTasksExport(
             cls,
             filename: str,
             year: str = None,
-            grade_score_mapper: Callable[[str], float] = None,
+            grade_score_mapper: dict[str, float] = None,
             grade_dtype: pd.api.types.CategoricalDtype = None,
             learning_task_filter: Callable[[pd.DataFrame], pd.DataFrame] = None,
             replace_values: dict[str, dict] = None) -> Reports:
         """Creates a new Reports instance from a Compass Learning Tasks export."""
         try:
             temp_df = pd.read_csv(filename,
                                   na_values=None,
@@ -198,15 +198,15 @@
     @classmethod
     def fromProgressReportsExport(
             cls,
             filename: str,
             progress_report_items: list[str],
             year: str = None,
             term: str = None,
-            grade_score_mapper: Callable[[str], float] = None,
+            grade_score_mapper: dict[str, float] = None,
             grade_dtype: pd.api.types.CategoricalDtype = None,
             replace_values: dict[str, dict] = None) -> Reports:
         """Creates a new Reports instance from a Compass progress reports export."""
         try:
             temp_df = pd.read_csv(filename,
                                   na_values=None,
                                   keep_default_na=False)
@@ -406,28 +406,31 @@
         ]
         self.data = pd.merge(self.data[reports_columns],
                              classes_df[classes_columns],
                              how="left",
                              on=["ClassCode", "Year"])
         if replace_values:
             self.data.replace(replace_values, inplace=True)
-        self.data.drop(columns="Year", inplace=False)
+        self.data.drop(columns="Year", inplace=True)
 
     def updateFromClassDetails(self) -> None:
         """Infills TeacherCode data with data available from other reports."""
 
         self.data.drop(columns="TeacherCode", inplace=True, errors="ignore")
         self.data = pd.merge(self.data,
                              self.class_details,
                              how="left",
                              on=["Time", "ClassCode"])
 
     def summary(self) -> pd.DataFrame:
         """Aggregates Academic and Work Habits results to produce a summary."""
-        grpd = self.data.groupby([
+        columns = ['Time', 'ClassCode', 'StudentCode',
+       'ResultScore', 'Type', 'LearningArea', 'SubjectCode',
+       'SubjectName', 'TeacherCode']
+        grpd = self.data[columns].groupby([
             'Time', 'ClassCode', 'StudentCode', 'Type', 'SubjectCode',
             'SubjectName', 'LearningArea', 'TeacherCode'
         ],
                                  as_index=False).mean()
         pvtd = grpd.pivot_table(index=[
             'Time', 'ClassCode', 'StudentCode', 'SubjectCode', 'SubjectName',
             'LearningArea', 'TeacherCode'
```

### Comparing `vicedtools-0.0.8/src/vicedtools/educationperfect.py` & `vicedtools-0.0.8.1/src/vicedtools/educationperfect.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8/src/vicedtools/gcp/__init__.py` & `vicedtools-0.0.8.1/src/vicedtools/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8/src/vicedtools/gcp/api.py` & `vicedtools-0.0.8.1/src/vicedtools/gcp/api.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8/src/vicedtools/gcp/format.py` & `vicedtools-0.0.8.1/src/vicedtools/gcp/format.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8/src/vicedtools/gcp/schema.py` & `vicedtools-0.0.8.1/src/vicedtools/gcp/schema.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8/src/vicedtools/naplan/__init__.py` & `vicedtools-0.0.8.1/src/vicedtools/naplan/__init__.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8/src/vicedtools/naplan/dataservicesession.py` & `vicedtools-0.0.8.1/src/vicedtools/naplan/dataservicesession.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8/src/vicedtools/naplan/sssrdata.py` & `vicedtools-0.0.8.1/src/vicedtools/naplan/sssrdata.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8/src/vicedtools/sportstrak.py` & `vicedtools-0.0.8.1/src/vicedtools/sportstrak.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8/src/vicedtools/vce/__init__.py` & `vicedtools-0.0.8.1/src/vicedtools/vce/__init__.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8/src/vicedtools/vce/schoolscores.py` & `vicedtools-0.0.8.1/src/vicedtools/vce/schoolscores.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8/src/vicedtools/vce/vasssession.py` & `vicedtools-0.0.8.1/src/vicedtools/vce/vasssession.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8/src/vicedtools.egg-info/PKG-INFO` & `vicedtools-0.0.8.1/src/vicedtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vicedtools
-Version: 0.0.8
+Version: 0.0.8.1
 Summary: A collection of tools for school data in Victorian schools.
 Home-page: https://github.com/gregbreese/vicedtools
 Author: Greg Breese
 Project-URL: Bug Tracker, https://github.com/gregbreese/vicedtools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `vicedtools-0.0.8/src/vicedtools.egg-info/SOURCES.txt` & `vicedtools-0.0.8.1/src/vicedtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8/src/vicedtools.egg-info/entry_points.txt` & `vicedtools-0.0.8.1/src/vicedtools.egg-info/entry_points.txt`

 * *Files identical despite different names*

