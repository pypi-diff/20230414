# Comparing `tmp/thunno2-2.0.6.tar.gz` & `tmp/thunno2-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thunno2-2.0.6.tar", last modified: Wed Apr 12 15:38:06 2023, max compression
+gzip compressed data, was "thunno2-2.0.7.tar", last modified: Fri Apr 14 16:14:39 2023, max compression
```

## Comparing `thunno2-2.0.6.tar` & `thunno2-2.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-12 15:38:06.962514 thunno2-2.0.6/
--rw-r--r--   0 nayak      (501) staff       (20)      959 2023-04-12 15:38:06.962402 thunno2-2.0.6/PKG-INFO
--rw-r--r--   0 nayak      (501) staff       (20)       38 2023-04-12 15:38:06.962550 thunno2-2.0.6/setup.cfg
--rw-r--r--   0 nayak      (501) staff       (20)     1354 2023-04-12 09:58:27.000000 thunno2-2.0.6/setup.py
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-12 15:38:06.961693 thunno2-2.0.6/thunno2/
--rw-r--r--   0 nayak      (501) staff       (20)       22 2023-04-03 16:07:07.000000 thunno2-2.0.6/thunno2/__init__.py
--rw-r--r--   0 nayak      (501) staff       (20)     1412 2023-04-03 16:27:37.000000 thunno2-2.0.6/thunno2/codepage.py
--rw-r--r--   0 nayak      (501) staff       (20)    39327 2023-04-11 16:50:16.000000 thunno2-2.0.6/thunno2/commands.py
--rw-r--r--   0 nayak      (501) staff       (20)     2891 2023-04-03 16:27:37.000000 thunno2-2.0.6/thunno2/constants.py
--rw-r--r--   0 nayak      (501) staff       (20)   244557 2023-04-08 16:04:36.000000 thunno2-2.0.6/thunno2/dictionary.py
--rw-r--r--   0 nayak      (501) staff       (20)     4260 2023-04-12 15:37:54.000000 thunno2-2.0.6/thunno2/flags.py
--rw-r--r--   0 nayak      (501) staff       (20)    40904 2023-04-11 19:11:59.000000 thunno2-2.0.6/thunno2/helpers.py
--rw-r--r--   0 nayak      (501) staff       (20)    18356 2023-04-11 14:03:07.000000 thunno2-2.0.6/thunno2/interpreter.py
--rw-r--r--   0 nayak      (501) staff       (20)    14374 2023-04-11 14:03:07.000000 thunno2-2.0.6/thunno2/lexer.py
--rw-r--r--   0 nayak      (501) staff       (20)     1215 2023-04-12 10:14:32.000000 thunno2-2.0.6/thunno2/run.py
--rw-r--r--   0 nayak      (501) staff       (20)    55521 2023-04-11 17:00:38.000000 thunno2-2.0.6/thunno2/tests.py
--rw-r--r--   0 nayak      (501) staff       (20)     1004 2023-04-06 20:08:08.000000 thunno2-2.0.6/thunno2/tokens.py
--rw-r--r--   0 nayak      (501) staff       (20)       97 2023-04-12 15:37:54.000000 thunno2-2.0.6/thunno2/version.py
-drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-12 15:38:06.962249 thunno2-2.0.6/thunno2.egg-info/
--rw-r--r--   0 nayak      (501) staff       (20)      959 2023-04-12 15:38:06.000000 thunno2-2.0.6/thunno2.egg-info/PKG-INFO
--rw-r--r--   0 nayak      (501) staff       (20)      414 2023-04-12 15:38:06.000000 thunno2-2.0.6/thunno2.egg-info/SOURCES.txt
--rw-r--r--   0 nayak      (501) staff       (20)        1 2023-04-12 15:38:06.000000 thunno2-2.0.6/thunno2.egg-info/dependency_links.txt
--rw-r--r--   0 nayak      (501) staff       (20)       54 2023-04-12 15:38:06.000000 thunno2-2.0.6/thunno2.egg-info/entry_points.txt
--rw-r--r--   0 nayak      (501) staff       (20)        8 2023-04-12 15:38:06.000000 thunno2-2.0.6/thunno2.egg-info/top_level.txt
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-14 16:14:39.405978 thunno2-2.0.7/
+-rw-r--r--   0 nayak      (501) staff       (20)      959 2023-04-14 16:14:39.405825 thunno2-2.0.7/PKG-INFO
+-rw-r--r--   0 nayak      (501) staff       (20)       38 2023-04-14 16:14:39.406018 thunno2-2.0.7/setup.cfg
+-rw-r--r--   0 nayak      (501) staff       (20)     1354 2023-04-12 09:58:27.000000 thunno2-2.0.7/setup.py
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-14 16:14:39.404841 thunno2-2.0.7/thunno2/
+-rw-r--r--   0 nayak      (501) staff       (20)       22 2023-04-03 16:07:07.000000 thunno2-2.0.7/thunno2/__init__.py
+-rw-r--r--   0 nayak      (501) staff       (20)     1412 2023-04-03 16:27:37.000000 thunno2-2.0.7/thunno2/codepage.py
+-rw-r--r--   0 nayak      (501) staff       (20)    46659 2023-04-14 08:28:09.000000 thunno2-2.0.7/thunno2/commands.py
+-rw-r--r--   0 nayak      (501) staff       (20)     2891 2023-04-03 16:27:37.000000 thunno2-2.0.7/thunno2/constants.py
+-rw-r--r--   0 nayak      (501) staff       (20)   245513 2023-04-14 08:28:09.000000 thunno2-2.0.7/thunno2/dictionary.py
+-rw-r--r--   0 nayak      (501) staff       (20)     4608 2023-04-13 17:15:28.000000 thunno2-2.0.7/thunno2/flags.py
+-rw-r--r--   0 nayak      (501) staff       (20)    47961 2023-04-13 17:15:28.000000 thunno2-2.0.7/thunno2/helpers.py
+-rw-r--r--   0 nayak      (501) staff       (20)    25412 2023-04-13 17:15:28.000000 thunno2-2.0.7/thunno2/interpreter.py
+-rw-r--r--   0 nayak      (501) staff       (20)    21430 2023-04-13 17:15:28.000000 thunno2-2.0.7/thunno2/lexer.py
+-rw-r--r--   0 nayak      (501) staff       (20)     1215 2023-04-12 10:14:32.000000 thunno2-2.0.7/thunno2/run.py
+-rw-r--r--   0 nayak      (501) staff       (20)    62646 2023-04-14 08:28:09.000000 thunno2-2.0.7/thunno2/tests.py
+-rw-r--r--   0 nayak      (501) staff       (20)     1004 2023-04-06 20:08:08.000000 thunno2-2.0.7/thunno2/tokens.py
+-rw-r--r--   0 nayak      (501) staff       (20)       97 2023-04-14 16:14:32.000000 thunno2-2.0.7/thunno2/version.py
+drwxr-xr-x   0 nayak      (501) staff       (20)        0 2023-04-14 16:14:39.405562 thunno2-2.0.7/thunno2.egg-info/
+-rw-r--r--   0 nayak      (501) staff       (20)      959 2023-04-14 16:14:39.000000 thunno2-2.0.7/thunno2.egg-info/PKG-INFO
+-rw-r--r--   0 nayak      (501) staff       (20)      414 2023-04-14 16:14:39.000000 thunno2-2.0.7/thunno2.egg-info/SOURCES.txt
+-rw-r--r--   0 nayak      (501) staff       (20)        1 2023-04-14 16:14:39.000000 thunno2-2.0.7/thunno2.egg-info/dependency_links.txt
+-rw-r--r--   0 nayak      (501) staff       (20)       54 2023-04-14 16:14:39.000000 thunno2-2.0.7/thunno2.egg-info/entry_points.txt
+-rw-r--r--   0 nayak      (501) staff       (20)        8 2023-04-14 16:14:39.000000 thunno2-2.0.7/thunno2.egg-info/top_level.txt
```

### Comparing `thunno2-2.0.6/PKG-INFO` & `thunno2-2.0.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: thunno2
-Version: 2.0.6
+Version: 2.0.7
 Summary: A golfing language
 Home-page: https://github.com/Thunno/Thunno2
 Author: Rujul Nayak
 Author-email: rujulnayak@outlook.com
 License: MIT
-Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.0.6.tar.gz
+Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.0.7.tar.gz
 Keywords: golfing,code-golf,language
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `thunno2-2.0.6/setup.py` & `thunno2-2.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.6/thunno2/codepage.py` & `thunno2-2.0.7/thunno2/codepage.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.6/thunno2/constants.py` & `thunno2-2.0.7/thunno2/constants.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.6/thunno2/dictionary.py` & `thunno2-2.0.7/thunno2/dictionary.py`

 * *Files 0% similar despite different names*

```diff
@@ -15238,48 +15238,108 @@
 0003b850: 6e67 0a7a 6f6f 6d73 0a7a 6f6f 730a 7a75  ng.zooms.zoos.zu
 0003b860: 6c75 0a7a 756c 7573 2222 222e 7370 6c69  lu.zulus""".spli
 0003b870: 746c 696e 6573 2829 0a0a 6672 6f6d 2074  tlines()..from t
 0003b880: 6875 6e6e 6f32 2069 6d70 6f72 7420 636f  hunno2 import co
 0003b890: 6465 7061 6765 0a66 726f 6d20 7468 756e  depage.from thun
 0003b8a0: 6e6f 3220 696d 706f 7274 2068 656c 7065  no2 import helpe
 0003b8b0: 7273 0a69 6d70 6f72 7420 7374 7269 6e67  rs.import string
-0003b8c0: 0a0a 6967 6e6f 7265 5f63 6861 7273 203d  ..ignore_chars =
-0003b8d0: 2073 7472 696e 672e 6173 6369 695f 6c65   string.ascii_le
-0003b8e0: 7474 6572 7320 2b20 7374 7269 6e67 2e64  tters + string.d
-0003b8f0: 6967 6974 7320 2b20 7227 2727 2e2c 213f  igits + r'''.,!?
-0003b900: 3a5c 2227 2528 2920 e280 98e2 8099 2727  :\"'%() ......''
-0003b910: 270a 6469 6374 696f 6e61 7279 5f63 6f64  '.dictionary_cod
-0003b920: 6570 6167 6520 3d20 2727 2e6a 6f69 6e28  epage = ''.join(
-0003b930: 6368 6172 2066 6f72 2063 6861 7220 696e  char for char in
-0003b940: 2063 6f64 6570 6167 652e 434f 4445 5041   codepage.CODEPA
-0003b950: 4745 2069 6620 6368 6172 206e 6f74 2069  GE if char not i
-0003b960: 6e20 6967 6e6f 7265 5f63 6861 7273 290a  n ignore_chars).
-0003b970: 0a61 7373 6572 7420 6c65 6e28 6469 6374  .assert len(dict
-0003b980: 696f 6e61 7279 5f63 6f64 6570 6167 6529  ionary_codepage)
-0003b990: 203d 3d20 3138 300a 0a0a 6465 6620 6469   == 180...def di
-0003b9a0: 6374 696f 6e61 7279 5f63 6f6d 7072 6573  ctionary_compres
-0003b9b0: 735f 776f 7264 2877 6f72 6429 3a0a 2020  s_word(word):.  
-0003b9c0: 2020 6966 2077 6f72 6420 6e6f 7420 696e    if word not in
-0003b9d0: 2077 6f72 6473 3a0a 2020 2020 2020 2020   words:.        
-0003b9e0: 7265 7475 726e 202d 310a 2020 2020 696e  return -1.    in
-0003b9f0: 6465 7820 3d20 776f 7264 732e 696e 6465  dex = words.inde
-0003ba00: 7828 776f 7264 290a 2020 2020 6261 7365  x(word).    base
-0003ba10: 5f31 3830 5f6e 756d 203d 2068 656c 7065  _180_num = helpe
-0003ba20: 7273 2e6e 756d 6265 725f 746f 5f62 6173  rs.number_to_bas
-0003ba30: 655f 6469 6769 7473 2869 6e64 6578 2c20  e_digits(index, 
-0003ba40: 3138 3029 0a20 2020 2072 6574 7572 6e20  180).    return 
-0003ba50: 2727 2e6a 6f69 6e28 6d61 7028 6469 6374  ''.join(map(dict
-0003ba60: 696f 6e61 7279 5f63 6f64 6570 6167 652e  ionary_codepage.
-0003ba70: 5f5f 6765 7469 7465 6d5f 5f2c 2062 6173  __getitem__, bas
-0003ba80: 655f 3138 305f 6e75 6d29 292e 726a 7573  e_180_num)).rjus
-0003ba90: 7428 322c 2027 c2a1 2729 0a0a 6465 6620  t(2, '..')..def 
-0003baa0: 6469 6374 696f 6e61 7279 5f64 6563 6f6d  dictionary_decom
-0003bab0: 7072 6573 735f 7374 7269 6e67 2873 293a  press_string(s):
-0003bac0: 0a20 2020 2062 6173 655f 3138 305f 6e75  .    base_180_nu
-0003bad0: 6d20 3d20 5b2a 6d61 7028 6469 6374 696f  m = [*map(dictio
-0003bae0: 6e61 7279 5f63 6f64 6570 6167 652e 696e  nary_codepage.in
-0003baf0: 6465 782c 2073 295d 0a20 2020 2069 6e64  dex, s)].    ind
-0003bb00: 6578 203d 2068 656c 7065 7273 2e66 726f  ex = helpers.fro
-0003bb10: 6d5f 6c69 7374 5f6f 665f 6469 6769 7473  m_list_of_digits
-0003bb20: 5f32 2862 6173 655f 3138 305f 6e75 6d2c  _2(base_180_num,
-0003bb30: 2031 3830 290a 2020 2020 7265 7475 726e   180).    return
-0003bb40: 2077 6f72 6473 5b69 6e64 6578 5d          words[index]
+0003b8c0: 2c20 7265 0a0a 6967 6e6f 7265 5f63 6861  , re..ignore_cha
+0003b8d0: 7273 203d 2073 7472 696e 672e 6173 6369  rs = string.asci
+0003b8e0: 695f 6c65 7474 6572 7320 2b20 7374 7269  i_letters + stri
+0003b8f0: 6e67 2e64 6967 6974 7320 2b20 7227 2727  ng.digits + r'''
+0003b900: 2e2c 213f 3a5c 2227 2528 2920 e280 98e2  .,!?:\"'%() ....
+0003b910: 8099 2727 270a 6469 6374 696f 6e61 7279  ..'''.dictionary
+0003b920: 5f63 6f64 6570 6167 6520 3d20 2727 2e6a  _codepage = ''.j
+0003b930: 6f69 6e28 6368 6172 2066 6f72 2063 6861  oin(char for cha
+0003b940: 7220 696e 2063 6f64 6570 6167 652e 434f  r in codepage.CO
+0003b950: 4445 5041 4745 2069 6620 6368 6172 206e  DEPAGE if char n
+0003b960: 6f74 2069 6e20 6967 6e6f 7265 5f63 6861  ot in ignore_cha
+0003b970: 7273 290a 0a61 7373 6572 7420 6c65 6e28  rs)..assert len(
+0003b980: 6469 6374 696f 6e61 7279 5f63 6f64 6570  dictionary_codep
+0003b990: 6167 6529 203d 3d20 3138 300a 0a0a 6465  age) == 180...de
+0003b9a0: 6620 6469 6374 696f 6e61 7279 5f63 6f6d  f dictionary_com
+0003b9b0: 7072 6573 735f 776f 7264 2877 6f72 6429  press_word(word)
+0003b9c0: 3a0a 2020 2020 6966 2077 6f72 6420 6e6f  :.    if word no
+0003b9d0: 7420 696e 2077 6f72 6473 3a0a 2020 2020  t in words:.    
+0003b9e0: 2020 2020 7265 7475 726e 202d 310a 2020      return -1.  
+0003b9f0: 2020 696e 6465 7820 3d20 776f 7264 732e    index = words.
+0003ba00: 696e 6465 7828 776f 7264 290a 2020 2020  index(word).    
+0003ba10: 6261 7365 5f31 3830 5f6e 756d 203d 2068  base_180_num = h
+0003ba20: 656c 7065 7273 2e6e 756d 6265 725f 746f  elpers.number_to
+0003ba30: 5f62 6173 655f 6469 6769 7473 2869 6e64  _base_digits(ind
+0003ba40: 6578 2c20 3138 3029 0a20 2020 2072 6574  ex, 180).    ret
+0003ba50: 7572 6e20 2727 2e6a 6f69 6e28 6d61 7028  urn ''.join(map(
+0003ba60: 6469 6374 696f 6e61 7279 5f63 6f64 6570  dictionary_codep
+0003ba70: 6167 652e 5f5f 6765 7469 7465 6d5f 5f2c  age.__getitem__,
+0003ba80: 2062 6173 655f 3138 305f 6e75 6d29 292e   base_180_num)).
+0003ba90: 726a 7573 7428 322c 2027 c2a1 2729 0a0a  rjust(2, '..')..
+0003baa0: 0a64 6566 2064 6963 7469 6f6e 6172 795f  .def dictionary_
+0003bab0: 6465 636f 6d70 7265 7373 5f73 7472 696e  decompress_strin
+0003bac0: 6728 7329 3a0a 2020 2020 6261 7365 5f31  g(s):.    base_1
+0003bad0: 3830 5f6e 756d 203d 205b 2a6d 6170 2864  80_num = [*map(d
+0003bae0: 6963 7469 6f6e 6172 795f 636f 6465 7061  ictionary_codepa
+0003baf0: 6765 2e69 6e64 6578 2c20 7329 5d0a 2020  ge.index, s)].  
+0003bb00: 2020 696e 6465 7820 3d20 6865 6c70 6572    index = helper
+0003bb10: 732e 6672 6f6d 5f6c 6973 745f 6f66 5f64  s.from_list_of_d
+0003bb20: 6967 6974 735f 3228 6261 7365 5f31 3830  igits_2(base_180
+0003bb30: 5f6e 756d 2c20 3138 3029 0a20 2020 2072  _num, 180).    r
+0003bb40: 6574 7572 6e20 776f 7264 735b 696e 6465  eturn words[inde
+0003bb50: 785d 0a0a 0a64 6566 2062 6163 6b73 6c61  x]...def backsla
+0003bb60: 7368 6966 7928 7329 3a0a 2020 2020 7220  shify(s):.    r 
+0003bb70: 3d20 2727 0a20 2020 2066 6f72 2063 2069  = ''.    for c i
+0003bb80: 6e20 733a 0a20 2020 2020 2020 2069 6620  n s:.        if 
+0003bb90: 6320 696e 2064 6963 7469 6f6e 6172 795f  c in dictionary_
+0003bba0: 636f 6465 7061 6765 202b 2027 5c5c 273a  codepage + '\\':
+0003bbb0: 0a20 2020 2020 2020 2020 2020 2072 202b  .            r +
+0003bbc0: 3d20 275c 5c27 202b 2063 0a20 2020 2020  = '\\' + c.     
+0003bbd0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0003bbe0: 2020 2020 2072 202b 3d20 630a 2020 2020       r += c.    
+0003bbf0: 7265 7475 726e 2072 0a0a 0a64 6566 206f  return r...def o
+0003bc00: 7074 696d 616c 5f64 6963 7469 6f6e 6172  ptimal_dictionar
+0003bc10: 795f 636f 6d70 7265 7373 696f 6e28 7329  y_compression(s)
+0003bc20: 3a0a 2020 2020 776f 7264 7320 3d20 7265  :.    words = re
+0003bc30: 2e66 696e 6461 6c6c 2827 285b 612d 7a5d  .findall('([a-z]
+0003bc40: 2b29 285b 5e61 2d7a 5d2b 2927 2c20 7374  +)([^a-z]+)', st
+0003bc50: 7228 7329 2e6c 6f77 6572 2829 290a 2020  r(s).lower()).  
+0003bc60: 2020 7265 7420 3d20 2727 0a20 2020 2066    ret = ''.    f
+0003bc70: 6f72 2077 6f72 642c 206f 7468 6572 5f73  or word, other_s
+0003bc80: 7475 6666 2069 6e20 776f 7264 733a 0a20  tuff in words:. 
+0003bc90: 2020 2020 2020 2069 6620 6e6f 7420 2877         if not (w
+0003bca0: 6f72 6420 2b20 6f74 6865 725f 7374 7566  ord + other_stuf
+0003bcb0: 6629 3a0a 2020 2020 2020 2020 2020 2020  f):.            
+0003bcc0: 636f 6e74 696e 7565 0a20 2020 2020 2020  continue.       
+0003bcd0: 2063 6f6d 7072 6573 7369 6f6e 7320 3d20   compressions = 
+0003bce0: 5b5d 0a20 2020 2020 2020 2066 6f72 206c  [].        for l
+0003bcf0: 2069 6e20 6865 6c70 6572 732e 696e 7465   in helpers.inte
+0003bd00: 6765 725f 7061 7274 6974 696f 6e73 286c  ger_partitions(l
+0003bd10: 656e 2877 6f72 6429 295b 3a3a 2d31 5d3a  en(word))[::-1]:
+0003bd20: 0a20 2020 2020 2020 2020 2020 206e 6577  .            new
+0003bd30: 5f77 6f72 6420 3d20 776f 7264 0a20 2020  _word = word.   
+0003bd40: 2020 2020 2020 2020 2078 203d 205b 5d0a           x = [].
+0003bd50: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0003bd60: 6920 696e 206c 3a0a 2020 2020 2020 2020  i in l:.        
+0003bd70: 2020 2020 2020 2020 782e 6170 7065 6e64          x.append
+0003bd80: 286e 6577 5f77 6f72 645b 3a69 5d29 0a20  (new_word[:i]). 
+0003bd90: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+0003bda0: 6577 5f77 6f72 6420 3d20 6e65 775f 776f  ew_word = new_wo
+0003bdb0: 7264 5b69 3a5d 0a20 2020 2020 2020 2020  rd[i:].         
+0003bdc0: 2020 2063 6f6d 7072 6573 7369 6f6e 732e     compressions.
+0003bdd0: 6170 7065 6e64 280a 2020 2020 2020 2020  append(.        
+0003bde0: 2020 2020 2020 2020 2727 2e6a 6f69 6e28          ''.join(
+0003bdf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0003be00: 2020 2020 2064 6963 7469 6f6e 6172 795f       dictionary_
+0003be10: 636f 6d70 7265 7373 5f77 6f72 6428 7729  compress_word(w)
+0003be20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0003be30: 2020 2020 2069 6620 6469 6374 696f 6e61       if dictiona
+0003be40: 7279 5f63 6f6d 7072 6573 735f 776f 7264  ry_compress_word
+0003be50: 2877 2920 213d 202d 310a 2020 2020 2020  (w) != -1.      
+0003be60: 2020 2020 2020 2020 2020 2020 2020 656c                el
+0003be70: 7365 2077 0a20 2020 2020 2020 2020 2020  se w.           
+0003be80: 2020 2020 2020 2020 2066 6f72 2077 2069           for w i
+0003be90: 6e20 780a 2020 2020 2020 2020 2020 2020  n x.            
+0003bea0: 2020 2020 2920 2b20 6261 636b 736c 6173      ) + backslas
+0003beb0: 6869 6679 286f 7468 6572 5f73 7475 6666  hify(other_stuff
+0003bec0: 290a 2020 2020 2020 2020 2020 2020 290a  ).            ).
+0003bed0: 2020 2020 2020 2020 7265 7420 2b3d 206d          ret += m
+0003bee0: 696e 2863 6f6d 7072 6573 7369 6f6e 732c  in(compressions,
+0003bef0: 206b 6579 3d6c 656e 290a 2020 2020 7265   key=len).    re
+0003bf00: 7475 726e 2072 6574 0a                   turn ret.
```

### Comparing `thunno2-2.0.6/thunno2/flags.py` & `thunno2-2.0.7/thunno2/flags.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,14 +104,25 @@
 
         if 'h' == flag:
             commands.ctx.stack.push(commands.commands['h']()[0])
 
         if 't' == flag:
             commands.ctx.stack.push(commands.commands['t']()[0])
 
+        if 'B' == flag:
+            x = (commands.ctx.stack + commands.ctx.other_il + [0])[0]
+            if isinstance(x, list):
+                r = ''
+                for i in x:
+                    try:
+                        r += chr(int(i))
+                    except:
+                        pass
+                commands.ctx.stack.push(r)
+
     if (commands.ctx.implicit_print or ('O' in flags)) and not ('o' in flags):
         print(next(commands.ctx.stack.rmv(1)))
 
 
 def run(flags, code, inputs):
 
     if 'V' in flags:
```

### Comparing `thunno2-2.0.6/thunno2/run.py` & `thunno2-2.0.7/thunno2/run.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.6/thunno2/tests.py` & `thunno2-2.0.7/thunno2/tests.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,145 @@
 from thunno2.commands import *
 
 """Here we test every command implemented in the commands dictionary"""
 
+"""Creative Commons Legal Code
+
+CC0 1.0 Universal
+
+    CREATIVE COMMONS CORPORATION IS NOT A LAW FIRM AND DOES NOT PROVIDE
+    LEGAL SERVICES. DISTRIBUTION OF THIS DOCUMENT DOES NOT CREATE AN
+    ATTORNEY-CLIENT RELATIONSHIP. CREATIVE COMMONS PROVIDES THIS
+    INFORMATION ON AN "AS-IS" BASIS. CREATIVE COMMONS MAKES NO WARRANTIES
+    REGARDING THE USE OF THIS DOCUMENT OR THE INFORMATION OR WORKS
+    PROVIDED HEREUNDER, AND DISCLAIMS LIABILITY FOR DAMAGES RESULTING FROM
+    THE USE OF THIS DOCUMENT OR THE INFORMATION OR WORKS PROVIDED
+    HEREUNDER.
+
+Statement of Purpose
+
+The laws of most jurisdictions throughout the world automatically confer
+exclusive Copyright and Related Rights (defined below) upon the creator
+and subsequent owner(s) (each and all, an "owner") of an original work of
+authorship and/or a database (each, a "Work").
+
+Certain owners wish to permanently relinquish those rights to a Work for
+the purpose of contributing to a commons of creative, cultural and
+scientific works ("Commons") that the public can reliably and without fear
+of later claims of infringement build upon, modify, incorporate in other
+works, reuse and redistribute as freely as possible in any form whatsoever
+and for any purposes, including without limitation commercial purposes.
+These owners may contribute to the Commons to promote the ideal of a free
+culture and the further production of creative, cultural and scientific
+works, or to gain reputation or greater distribution for their Work in
+part through the use and efforts of others.
+
+For these and/or other purposes and motivations, and without any
+expectation of additional consideration or compensation, the person
+associating CC0 with a Work (the "Affirmer"), to the extent that he or she
+is an owner of Copyright and Related Rights in the Work, voluntarily
+elects to apply CC0 to the Work and publicly distribute the Work under its
+terms, with knowledge of his or her Copyright and Related Rights in the
+Work and the meaning and intended legal effect of CC0 on those rights.
+
+1. Copyright and Related Rights. A Work made available under CC0 may be
+protected by copyright and related or neighboring rights ("Copyright and
+Related Rights"). Copyright and Related Rights include, but are not
+limited to, the following:
+
+  i. the right to reproduce, adapt, distribute, perform, display,
+     communicate, and translate a Work;
+ ii. moral rights retained by the original author(s) and/or performer(s);
+iii. publicity and privacy rights pertaining to a person's image or
+     likeness depicted in a Work;
+ iv. rights protecting against unfair competition in regards to a Work,
+     subject to the limitations in paragraph 4(a), below;
+  v. rights protecting the extraction, dissemination, use and reuse of data
+     in a Work;
+ vi. database rights (such as those arising under Directive 96/9/EC of the
+     European Parliament and of the Council of 11 March 1996 on the legal
+     protection of databases, and under any national implementation
+     thereof, including any amended or successor version of such
+     directive); and
+vii. other similar, equivalent or corresponding rights throughout the
+     world based on applicable law or treaty, and any national
+     implementations thereof.
+
+2. Waiver. To the greatest extent permitted by, but not in contravention
+of, applicable law, Affirmer hereby overtly, fully, permanently,
+irrevocably and unconditionally waives, abandons, and surrenders all of
+Affirmer's Copyright and Related Rights and associated claims and causes
+of action, whether now known or unknown (including existing as well as
+future claims and causes of action), in the Work (i) in all territories
+worldwide, (ii) for the maximum duration provided by applicable law or
+treaty (including future time extensions), (iii) in any current or future
+medium and for any number of copies, and (iv) for any purpose whatsoever,
+including without limitation commercial, advertising or promotional
+purposes (the "Waiver"). Affirmer makes the Waiver for the benefit of each
+member of the public at large and to the detriment of Affirmer's heirs and
+successors, fully intending that such Waiver shall not be subject to
+revocation, rescission, cancellation, termination, or any other legal or
+equitable action to disrupt the quiet enjoyment of the Work by the public
+as contemplated by Affirmer's express Statement of Purpose.
+
+3. Public License Fallback. Should any part of the Waiver for any reason
+be judged legally invalid or ineffective under applicable law, then the
+Waiver shall be preserved to the maximum extent permitted taking into
+account Affirmer's express Statement of Purpose. In addition, to the
+extent the Waiver is so judged Affirmer hereby grants to each affected
+person a royalty-free, non transferable, non sublicensable, non exclusive,
+irrevocable and unconditional license to exercise Affirmer's Copyright and
+Related Rights in the Work (i) in all territories worldwide, (ii) for the
+maximum duration provided by applicable law or treaty (including future
+time extensions), (iii) in any current or future medium and for any number
+of copies, and (iv) for any purpose whatsoever, including without
+limitation commercial, advertising or promotional purposes (the
+"License"). The License shall be deemed effective as of the date CC0 was
+applied by Affirmer to the Work. Should any part of the License for any
+reason be judged legally invalid or ineffective under applicable law, such
+partial invalidity or ineffectiveness shall not invalidate the remainder
+of the License, and in such case Affirmer hereby affirms that he or she
+will not (i) exercise any of his or her remaining Copyright and Related
+Rights in the Work or (ii) assert any associated claims and causes of
+action with respect to the Work, in either case contrary to Affirmer's
+express Statement of Purpose.
+
+4. Limitations and Disclaimers.
+
+ a. No trademark or patent rights held by Affirmer are waived, abandoned,
+    surrendered, licensed or otherwise affected by this document.
+ b. Affirmer offers the Work as-is and makes no representations or
+    warranties of any kind concerning the Work, express, implied,
+    statutory or otherwise, including without limitation warranties of
+    title, merchantability, fitness for a particular purpose, non
+    infringement, or the absence of latent or other defects, accuracy, or
+    the present or absence of errors, whether or not discoverable, all to
+    the greatest extent permissible under applicable law.
+ c. Affirmer disclaims responsibility for clearing rights of other persons
+    that may apply to the Work or any use thereof, including without
+    limitation any person's Copyright and Related Rights in the Work.
+    Further, Affirmer disclaims responsibility for obtaining any necessary
+    consents, permissions or other rights required for any use of the
+    Work.
+ d. Affirmer understands and acknowledges that Creative Commons is not a
+    party to this document and has no duty or obligation with respect to
+    this CC0 or use of the Work.
+"""
+
 tests_counter = 0
 tested_commands = []
 
 UNTESTABLE = 'ɼ'
 
 
 def call(cmd, *stk):
     ctx.stack = Stack(stk)
     ctx.warnings = True
     tested_commands.append(cmd)
-    return commands[cmd]()
+    return get_a_function(cmd)()
 
 
 def assert_eq(a, *b):
     global tests_counter
     tests_counter += 1
     #               Because 1 == True
     #               but '1' != 'True'
@@ -1779,14 +1902,18 @@
 
 assert_eq(call('ẓ', -3, 'abcde'), 'abc')
 assert_eq(call('ẓ', '', 10), '')
 
 assert_eq(call('ẓ', 2, [123, 456, 789]), [123])
 assert_eq(call('ẓ', ['abc', 'def', 'ghi', 'jkl', 'mno'], 3), ['abc', 'def'])
 
+# øD
+
+assert_eq(call('øD', 'Hello, World!'), 'Ƙ¥, «ʋ!')
+
 # After all the tests
 
 untested_commands = sorted({*commands} - {*tested_commands} - {*UNTESTABLE}, key=[*commands].index)
 if untested_commands:
     print(f'\u001b[33mUntested commands: {", ".join(untested_commands)}')
 
 print(f'\u001b[32mPassed {tests_counter} tests on {len({*tested_commands})} commands.')
```

### Comparing `thunno2-2.0.6/thunno2/tokens.py` & `thunno2-2.0.7/thunno2/tokens.py`

 * *Files identical despite different names*

### Comparing `thunno2-2.0.6/thunno2.egg-info/PKG-INFO` & `thunno2-2.0.7/thunno2.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: thunno2
-Version: 2.0.6
+Version: 2.0.7
 Summary: A golfing language
 Home-page: https://github.com/Thunno/Thunno2
 Author: Rujul Nayak
 Author-email: rujulnayak@outlook.com
 License: MIT
-Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.0.6.tar.gz
+Download-URL: https://github.com/Thunno/Thunno2/archive/refs/tags/v2.0.7.tar.gz
 Keywords: golfing,code-golf,language
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

