# Comparing `tmp/dune_harmonizer-0.1.0.tar.gz` & `tmp/dune_harmonizer-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dune_harmonizer-0.1.0.tar", max compression
+gzip compressed data, was "dune_harmonizer-0.2.0.tar", max compression
```

## Comparing `dune_harmonizer-0.1.0.tar` & `dune_harmonizer-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1061 2023-04-14 09:56:53.728784 dune_harmonizer-0.1.0/LICENSE
--rw-r--r--   0        0        0     1865 2023-04-14 09:56:53.728784 dune_harmonizer-0.1.0/README.md
--rw-r--r--   0        0        0      440 2023-04-14 09:56:53.728784 dune_harmonizer-0.1.0/dune/harmonizer/__init__.py
--rw-r--r--   0        0        0      849 2023-04-14 09:57:13.144657 dune_harmonizer-0.1.0/dune/harmonizer/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    22213 2023-04-14 09:57:13.324656 dune_harmonizer-0.1.0/dune/harmonizer/__pycache__/custom_transforms.cpython-311.pyc
--rw-r--r--   0        0        0      630 2023-04-14 09:57:13.328656 dune_harmonizer-0.1.0/dune/harmonizer/__pycache__/errors.cpython-311.pyc
--rw-r--r--   0        0        0     3103 2023-04-14 09:57:13.328656 dune_harmonizer-0.1.0/dune/harmonizer/__pycache__/table_replacements.cpython-311.pyc
--rw-r--r--   0        0        0     3305 2023-04-14 09:57:13.148657 dune_harmonizer-0.1.0/dune/harmonizer/__pycache__/translate.cpython-311.pyc
--rw-r--r--   0        0        0       54 2023-04-14 09:56:53.728784 dune_harmonizer-0.1.0/dune/harmonizer/constants.py
--rw-r--r--   0        0        0    19493 2023-04-14 09:56:53.728784 dune_harmonizer-0.1.0/dune/harmonizer/custom_transforms.py
--rw-r--r--   0        0        0      105 2023-04-14 09:56:53.728784 dune_harmonizer-0.1.0/dune/harmonizer/errors.py
--rw-r--r--   0        0        0     2018 2023-04-14 09:56:53.728784 dune_harmonizer-0.1.0/dune/harmonizer/table_replacements.py
--rw-r--r--   0        0        0     3050 2023-04-14 09:56:53.728784 dune_harmonizer-0.1.0/dune/harmonizer/translate.py
--rw-r--r--   0        0        0      570 2023-04-14 09:56:53.728784 dune_harmonizer-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2201 1970-01-01 00:00:00.000000 dune_harmonizer-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-04-14 13:16:22.477932 dune_harmonizer-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1865 2023-04-14 13:16:22.477932 dune_harmonizer-0.2.0/README.md
+-rw-r--r--   0        0        0      440 2023-04-14 13:16:22.477932 dune_harmonizer-0.2.0/dune/harmonizer/__init__.py
+-rw-r--r--   0        0        0      849 2023-04-14 13:16:36.054141 dune_harmonizer-0.2.0/dune/harmonizer/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    22778 2023-04-14 13:16:36.226143 dune_harmonizer-0.2.0/dune/harmonizer/__pycache__/custom_transforms.cpython-311.pyc
+-rw-r--r--   0        0        0      630 2023-04-14 13:16:36.230144 dune_harmonizer-0.2.0/dune/harmonizer/__pycache__/errors.cpython-311.pyc
+-rw-r--r--   0        0        0     3103 2023-04-14 13:16:36.230144 dune_harmonizer-0.2.0/dune/harmonizer/__pycache__/table_replacements.cpython-311.pyc
+-rw-r--r--   0        0        0     3305 2023-04-14 13:16:36.054141 dune_harmonizer-0.2.0/dune/harmonizer/__pycache__/translate.cpython-311.pyc
+-rw-r--r--   0        0        0       54 2023-04-14 13:16:22.477932 dune_harmonizer-0.2.0/dune/harmonizer/constants.py
+-rw-r--r--   0        0        0    19851 2023-04-14 13:16:22.477932 dune_harmonizer-0.2.0/dune/harmonizer/custom_transforms.py
+-rw-r--r--   0        0        0      105 2023-04-14 13:16:22.477932 dune_harmonizer-0.2.0/dune/harmonizer/errors.py
+-rw-r--r--   0        0        0     2018 2023-04-14 13:16:22.477932 dune_harmonizer-0.2.0/dune/harmonizer/table_replacements.py
+-rw-r--r--   0        0        0     3050 2023-04-14 13:16:22.477932 dune_harmonizer-0.2.0/dune/harmonizer/translate.py
+-rw-r--r--   0        0        0      570 2023-04-14 13:16:22.477932 dune_harmonizer-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2201 1970-01-01 00:00:00.000000 dune_harmonizer-0.2.0/PKG-INFO
```

### Comparing `dune_harmonizer-0.1.0/LICENSE` & `dune_harmonizer-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dune_harmonizer-0.1.0/README.md` & `dune_harmonizer-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `dune_harmonizer-0.1.0/dune/harmonizer/__pycache__/__init__.cpython-311.pyc` & `dune_harmonizer-0.2.0/dune/harmonizer/__pycache__/__init__.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x65233964 (Fri Apr 14 09:56:53 2023 UTC)
+moddate:  0x26523964 (Fri Apr 14 13:16:22 2023 UTC)
 files sz: 440
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
```

### Comparing `dune_harmonizer-0.1.0/dune/harmonizer/__pycache__/custom_transforms.cpython-311.pyc` & `dune_harmonizer-0.2.0/dune/harmonizer/__pycache__/custom_transforms.cpython-311.pyc`

 * *Files 3% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x65233964 (Fri Apr 14 09:56:53 2023 UTC)
-files sz: 19493
+moddate:  0x26523964 (Fri Apr 14 13:16:22 2023 UTC)
+files sz: 19851
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c005a00640064026c016d025a020100640064016c035a
@@ -14,15 +14,15 @@
       0aac08a6020000ab0200000000000000005a0b020065026508640bac08a6
       020000ab0200000000000000005a0c020065026508640cac08a6020000ab
       0200000000000000005a0d640d84005a0e640e5a0f640f5a106410650f9b
       009d025a1165109b0064109d025a126411650f9b009d025a1365109b0064
       119d025a14641284005a15641384005a16641484005a17641584005a1864
       1684005a19641784005a1a641884005a1b641984005a1c641a84005a1d64
       1b84005a1e641c84005a1f641d84005a20641e84005a21641f84005a2264
-      2084005a23642184005a24642284005a2564015300
+      2084005a23642184005a24642284005a25642384005a2664015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (re)
                  8 STORE_NAME               0 (re)
    
@@ -136,79 +136,83 @@
                240 BUILD_STRING             2
                242 STORE_NAME              20 (single_quoted_param_right_placeholder)
    
    195         244 LOAD_CONST              18 (<code object interval_fix, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 195>)
                246 MAKE_FUNCTION            0
                248 STORE_NAME              21 (interval_fix)
    
-   255         250 LOAD_CONST              19 (<code object bytearray_parameter_fix, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 255>)
+   254         250 LOAD_CONST              19 (<code object bytearray_parameter_fix, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 254>)
                252 MAKE_FUNCTION            0
                254 STORE_NAME              22 (bytearray_parameter_fix)
    
-   282         256 LOAD_CONST              20 (<code object cast_numeric, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 282>)
+   281         256 LOAD_CONST              20 (<code object cast_numeric, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 281>)
                258 MAKE_FUNCTION            0
                260 STORE_NAME              23 (cast_numeric)
    
-   291         262 LOAD_CONST              21 (<code object cast_timestamp, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 291>)
+   290         262 LOAD_CONST              21 (<code object cast_timestamp, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 290>)
                264 MAKE_FUNCTION            0
                266 STORE_NAME              24 (cast_timestamp)
    
-   309         268 LOAD_CONST              22 (<code object fix_boolean, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 309>)
+   308         268 LOAD_CONST              22 (<code object fix_boolean, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 308>)
                270 MAKE_FUNCTION            0
                272 STORE_NAME              25 (fix_boolean)
    
-   319         274 LOAD_CONST              23 (<code object warn_unnest, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 319>)
+   318         274 LOAD_CONST              23 (<code object warn_unnest, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 318>)
                276 MAKE_FUNCTION            0
                278 STORE_NAME              26 (warn_unnest)
    
-   333         280 LOAD_CONST              24 (<code object warn_sequence, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 333>)
+   332         280 LOAD_CONST              24 (<code object warn_sequence, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 332>)
                282 MAKE_FUNCTION            0
                284 STORE_NAME              27 (warn_sequence)
    
-   347         286 LOAD_CONST              25 (<code object prep_query, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 347>)
+   346         286 LOAD_CONST              25 (<code object prep_query, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 346>)
                288 MAKE_FUNCTION            0
                290 STORE_NAME              28 (prep_query)
    
-   359         292 LOAD_CONST              26 (<code object rename_amount_column, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 359>)
+   358         292 LOAD_CONST              26 (<code object rename_amount_column, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 358>)
                294 MAKE_FUNCTION            0
                296 STORE_NAME              29 (rename_amount_column)
    
-   364         298 LOAD_CONST              27 (<code object bytea2numeric, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 364>)
+   363         298 LOAD_CONST              27 (<code object bytea2numeric, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 363>)
                300 MAKE_FUNCTION            0
                302 STORE_NAME              30 (bytea2numeric)
    
-   378         304 LOAD_CONST              28 (<code object fix_bytearray_param, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 378>)
+   377         304 LOAD_CONST              28 (<code object fix_bytearray_param, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 377>)
                306 MAKE_FUNCTION            0
                308 STORE_NAME              31 (fix_bytearray_param)
    
-   384         310 LOAD_CONST              29 (<code object fix_bytearray_lower, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 384>)
+   383         310 LOAD_CONST              29 (<code object fix_bytearray_lower, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 383>)
                312 MAKE_FUNCTION            0
                314 STORE_NAME              32 (fix_bytearray_lower)
    
-   393         316 LOAD_CONST              30 (<code object chain_where, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 393>)
+   392         316 LOAD_CONST              30 (<code object chain_where, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 392>)
                318 MAKE_FUNCTION            0
                320 STORE_NAME              33 (chain_where)
    
-   403         322 LOAD_CONST              31 (<code object postgres_transforms, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 403>)
+   402         322 LOAD_CONST              31 (<code object postgres_transforms, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 402>)
                324 MAKE_FUNCTION            0
                326 STORE_NAME              34 (postgres_transforms)
    
-   427         328 LOAD_CONST              32 (<code object remove_quotes_around_0x_strings, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 427>)
+   426         328 LOAD_CONST              32 (<code object remove_quotes_around_0x_strings, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 426>)
                330 MAKE_FUNCTION            0
                332 STORE_NAME              35 (remove_quotes_around_0x_strings)
    
-   436         334 LOAD_CONST              33 (<code object spark_transforms, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 436>)
+   435         334 LOAD_CONST              33 (<code object spark_function_replacements, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 435>)
                336 MAKE_FUNCTION            0
-               338 STORE_NAME              36 (spark_transforms)
+               338 STORE_NAME              36 (spark_function_replacements)
    
-   455         340 LOAD_CONST              34 (<code object add_warnings_and_banner, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 455>)
+   443         340 LOAD_CONST              34 (<code object spark_transforms, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 443>)
                342 MAKE_FUNCTION            0
-               344 STORE_NAME              37 (add_warnings_and_banner)
-               346 LOAD_CONST               1 (None)
-               348 RETURN_VALUE
+               344 STORE_NAME              37 (spark_transforms)
+   
+   463         346 LOAD_CONST              35 (<code object add_warnings_and_banner, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 463>)
+               348 MAKE_FUNCTION            0
+               350 STORE_NAME              38 (add_warnings_and_banner)
+               352 LOAD_CONST               1 (None)
+               354 RETURN_VALUE
    consts
       0
       None
       ('partial',)
       ('postgres_table_replacements',)
       code
          argcount  : 1
@@ -1028,15 +1032,15 @@
       "'"
       code
          argcount  : 1
          nlocals   : 9
          stacksize : 5
          flags     : 3
          code
-            0x870997007c006a00000000000000000064016b02000000009002729c74
+            0x870997007c006a00000000000000000064016b02000000009002729b74
             03000000000000000000007c006a020000000000000000a6010000ab0100
             000000000000007d017c0164021900000000000000000064036b02000000
             0072167c0164041900000000000000000064056b0200000000720a7c0164
             0664048502190000000000000000007d017407000000000000000000006a
             04000000000000000064077c01a6020000ab0200000000000000007d0264
             0884007c02640664098502190000000000000000004400a6000000ab0000
             000000000000007d03740b000000000000000000007c03a6010000ab0100
@@ -1057,41 +1061,41 @@
             0100000000000000009b00640e9d037c04a00b0000000000000000000000
             000000000000000000a6000000ab0000000000000000007a000000a00e00
             0000000000000000000000000000000000000064106411a6020000ab0200
             00000000000000a00e000000000000000000000000000000000000000064
             0c6411a6020000ab0200000000000000007d06741f000000000000000000
             006a10000000000000000064127c069b0064139d03a6010000ab01000000
             000000000053007c0053007c01a004000000000000000000000000000000
-            0000000000a6000000ab0000000000000000005e027d058a097d07090074
-            2300000000000000000000880966016414840864154400a6000000ab0000
-            00000000000000a6010000ab01000000000000000072ce8909a012000000
-            00000000000000000000000000000000006416a6010000ab010000000000
-            000000720a8909640964048502190000000000000000008a098909640c6b
-            020000000072297419000000000000000000007c05a6010000ab01000000
-            0000000000640f7a0500007d0564118a097c07a013000000000000000000
-            00000000000000000000006417a6010000ab010000000000000000010064
-            187403000000000000000000007c05a6010000ab0100000000000000007a
-            00000064197a00000089097a000000640aa0060000000000000000000000
-            0000000000000000007c07a6010000ab0100000000000000007a000000a0
-            0e0000000000000000000000000000000000000000742800000000000000
-            000000742a00000000000000000000a6020000ab020000000000000000a0
-            0e0000000000000000000000000000000000000000742c00000000000000
-            000000742e00000000000000000000a6020000ab0200000000000000007d
-            08741f000000000000000000006a1000000000000000007c08641aac1ba6
-            020000ab02000000000000000053007c005300
+            0000000000a6000000ab0000000000000000005e027d058a097d07742300
+            000000000000000000880966016414840864154400a6000000ab00000000
+            0000000000a6010000ab01000000000000000072ce8909a0120000000000
+            0000000000000000000000000000006416a6010000ab0100000000000000
+            00720a8909640964048502190000000000000000008a098909640c6b0200
+            00000072297419000000000000000000007c05a6010000ab010000000000
+            000000640f7a0500007d0564118a097c07a0130000000000000000000000
+            0000000000000000006417a6010000ab0100000000000000000100641874
+            03000000000000000000007c05a6010000ab0100000000000000007a0000
+            0064197a00000089097a000000640aa00600000000000000000000000000
+            000000000000007c07a6010000ab0100000000000000007a000000a00e00
+            000000000000000000000000000000000000007428000000000000000000
+            00742a00000000000000000000a6020000ab020000000000000000a00e00
+            00000000000000000000000000000000000000742c000000000000000000
+            00742e00000000000000000000a6020000ab0200000000000000007d0874
+            1f000000000000000000006a1000000000000000007c08641aac1ba60200
+            00ab02000000000000000053007c005300
                        0 MAKE_CELL                9 (granularity)
          
          195           2 RESUME                   0
          
          197           4 LOAD_FAST                0 (node)
                        6 LOAD_ATTR                0 (key)
                       16 LOAD_CONST               1 ('interval')
                       18 COMPARE_OP               2 (==)
                       24 EXTENDED_ARG             2
-                      26 POP_JUMP_FORWARD_IF_FALSE   668 (to 1364)
+                      26 POP_JUMP_FORWARD_IF_FALSE   667 (to 1362)
          
          199          28 LOAD_GLOBAL              3 (NULL + str)
                       40 LOAD_FAST                0 (node)
                       42 LOAD_ATTR                2 (this)
                       52 PRECALL                  1
                       56 CALL                     1
                       66 STORE_FAST               1 (interval_argument)
@@ -1267,110 +1271,108 @@
                      874 PRECALL                  0
                      878 CALL                     0
                      888 UNPACK_EX                2
                      890 STORE_FAST               5 (value)
                      892 STORE_DEREF              9 (granularity)
                      894 STORE_FAST               7 (rest)
          
-         227         896 NOP
-         
-         228         898 LOAD_GLOBAL             35 (NULL + any)
-                     910 LOAD_CLOSURE             9 (granularity)
-                     912 BUILD_TUPLE              1
-                     914 LOAD_CONST              20 (<code object <genexpr>, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 228>)
-                     916 MAKE_FUNCTION            8 (closure)
-         
-         230         918 LOAD_CONST              21 (('second', 'minute', 'hour', 'day', 'week', 'month', 'year'))
-         
-         228         920 GET_ITER
-                     922 PRECALL                  0
-                     926 CALL                     0
-                     936 PRECALL                  1
-                     940 CALL                     1
-                     950 POP_JUMP_FORWARD_IF_FALSE   206 (to 1364)
-         
-         240         952 LOAD_DEREF               9 (granularity)
-                     954 LOAD_METHOD             18 (endswith)
-                     976 LOAD_CONST              22 ('s')
-                     978 PRECALL                  1
-                     982 CALL                     1
-                     992 POP_JUMP_FORWARD_IF_FALSE    10 (to 1014)
-         
-         241         994 LOAD_DEREF               9 (granularity)
-                     996 LOAD_CONST               9 (None)
-                     998 LOAD_CONST               4 (-1)
-                    1000 BUILD_SLICE              2
-                    1002 BINARY_SUBSCR
-                    1012 STORE_DEREF              9 (granularity)
-         
-         242     >> 1014 LOAD_DEREF               9 (granularity)
-                    1016 LOAD_CONST              12 ('week')
-                    1018 COMPARE_OP               2 (==)
-                    1024 POP_JUMP_FORWARD_IF_FALSE    41 (to 1108)
-         
-         243        1026 LOAD_GLOBAL             25 (NULL + int)
-                    1038 LOAD_FAST                5 (value)
-                    1040 PRECALL                  1
-                    1044 CALL                     1
-                    1054 LOAD_CONST              15 (7)
-                    1056 BINARY_OP                5 (*)
-                    1060 STORE_FAST               5 (value)
-         
-         244        1062 LOAD_CONST              17 ('day')
-                    1064 STORE_DEREF              9 (granularity)
-         
-         245        1066 LOAD_FAST                7 (rest)
-                    1068 LOAD_METHOD             19 (append)
-                    1090 LOAD_CONST              23 ("--week doesn't work in DuneSQL\n")
-                    1092 PRECALL                  1
-                    1096 CALL                     1
-                    1106 POP_TOP
-         
-         247     >> 1108 LOAD_CONST              24 ("INTERVAL '")
-                    1110 LOAD_GLOBAL              3 (NULL + str)
-                    1122 LOAD_FAST                5 (value)
-                    1124 PRECALL                  1
-                    1128 CALL                     1
-                    1138 BINARY_OP                0 (+)
-                    1142 LOAD_CONST              25 ("' ")
-                    1144 BINARY_OP                0 (+)
-                    1148 LOAD_DEREF               9 (granularity)
-                    1150 BINARY_OP                0 (+)
-                    1154 LOAD_CONST              10 (' ')
-                    1156 LOAD_METHOD              6 (join)
-                    1178 LOAD_FAST                7 (rest)
-                    1180 PRECALL                  1
-                    1184 CALL                     1
-                    1194 BINARY_OP                0 (+)
-         
-         248        1198 LOAD_METHOD             14 (replace)
-                    1220 LOAD_GLOBAL             40 (param_left_placeholder)
-                    1232 LOAD_GLOBAL             42 (double_quoted_param_left_placeholder)
-                    1244 PRECALL                  2
-                    1248 CALL                     2
-         
-         249        1258 LOAD_METHOD             14 (replace)
-                    1280 LOAD_GLOBAL             44 (param_right_placeholder)
-                    1292 LOAD_GLOBAL             46 (double_quoted_param_right_placeholder)
-                    1304 PRECALL                  2
-                    1308 CALL                     2
-         
-         246        1318 STORE_FAST               8 (final_interval)
-         
-         251        1320 LOAD_GLOBAL             31 (NULL + sqlglot)
-                    1332 LOAD_ATTR               16 (parse_one)
-                    1342 LOAD_FAST                8 (final_interval)
-                    1344 LOAD_CONST              26 ('trino')
-                    1346 KW_NAMES                27
-                    1348 PRECALL                  2
-                    1352 CALL                     2
-                    1362 RETURN_VALUE
+         227         896 LOAD_GLOBAL             35 (NULL + any)
+                     908 LOAD_CLOSURE             9 (granularity)
+                     910 BUILD_TUPLE              1
+                     912 LOAD_CONST              20 (<code object <genexpr>, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 227>)
+                     914 MAKE_FUNCTION            8 (closure)
+         
+         229         916 LOAD_CONST              21 (('second', 'minute', 'hour', 'day', 'week', 'month', 'year'))
+         
+         227         918 GET_ITER
+                     920 PRECALL                  0
+                     924 CALL                     0
+                     934 PRECALL                  1
+                     938 CALL                     1
+                     948 POP_JUMP_FORWARD_IF_FALSE   206 (to 1362)
+         
+         239         950 LOAD_DEREF               9 (granularity)
+                     952 LOAD_METHOD             18 (endswith)
+                     974 LOAD_CONST              22 ('s')
+                     976 PRECALL                  1
+                     980 CALL                     1
+                     990 POP_JUMP_FORWARD_IF_FALSE    10 (to 1012)
+         
+         240         992 LOAD_DEREF               9 (granularity)
+                     994 LOAD_CONST               9 (None)
+                     996 LOAD_CONST               4 (-1)
+                     998 BUILD_SLICE              2
+                    1000 BINARY_SUBSCR
+                    1010 STORE_DEREF              9 (granularity)
+         
+         241     >> 1012 LOAD_DEREF               9 (granularity)
+                    1014 LOAD_CONST              12 ('week')
+                    1016 COMPARE_OP               2 (==)
+                    1022 POP_JUMP_FORWARD_IF_FALSE    41 (to 1106)
+         
+         242        1024 LOAD_GLOBAL             25 (NULL + int)
+                    1036 LOAD_FAST                5 (value)
+                    1038 PRECALL                  1
+                    1042 CALL                     1
+                    1052 LOAD_CONST              15 (7)
+                    1054 BINARY_OP                5 (*)
+                    1058 STORE_FAST               5 (value)
+         
+         243        1060 LOAD_CONST              17 ('day')
+                    1062 STORE_DEREF              9 (granularity)
+         
+         244        1064 LOAD_FAST                7 (rest)
+                    1066 LOAD_METHOD             19 (append)
+                    1088 LOAD_CONST              23 ("--week doesn't work in DuneSQL\n")
+                    1090 PRECALL                  1
+                    1094 CALL                     1
+                    1104 POP_TOP
+         
+         246     >> 1106 LOAD_CONST              24 ("INTERVAL '")
+                    1108 LOAD_GLOBAL              3 (NULL + str)
+                    1120 LOAD_FAST                5 (value)
+                    1122 PRECALL                  1
+                    1126 CALL                     1
+                    1136 BINARY_OP                0 (+)
+                    1140 LOAD_CONST              25 ("' ")
+                    1142 BINARY_OP                0 (+)
+                    1146 LOAD_DEREF               9 (granularity)
+                    1148 BINARY_OP                0 (+)
+                    1152 LOAD_CONST              10 (' ')
+                    1154 LOAD_METHOD              6 (join)
+                    1176 LOAD_FAST                7 (rest)
+                    1178 PRECALL                  1
+                    1182 CALL                     1
+                    1192 BINARY_OP                0 (+)
+         
+         247        1196 LOAD_METHOD             14 (replace)
+                    1218 LOAD_GLOBAL             40 (param_left_placeholder)
+                    1230 LOAD_GLOBAL             42 (double_quoted_param_left_placeholder)
+                    1242 PRECALL                  2
+                    1246 CALL                     2
+         
+         248        1256 LOAD_METHOD             14 (replace)
+                    1278 LOAD_GLOBAL             44 (param_right_placeholder)
+                    1290 LOAD_GLOBAL             46 (double_quoted_param_right_placeholder)
+                    1302 PRECALL                  2
+                    1306 CALL                     2
+         
+         245        1316 STORE_FAST               8 (final_interval)
+         
+         250        1318 LOAD_GLOBAL             31 (NULL + sqlglot)
+                    1330 LOAD_ATTR               16 (parse_one)
+                    1340 LOAD_FAST                8 (final_interval)
+                    1342 LOAD_CONST              26 ('trino')
+                    1344 KW_NAMES                27
+                    1346 PRECALL                  2
+                    1350 CALL                     2
+                    1360 RETURN_VALUE
          
-         252     >> 1364 LOAD_FAST                0 (node)
-                    1366 RETURN_VALUE
+         251     >> 1362 LOAD_FAST                0 (node)
+                    1364 RETURN_VALUE
          ExceptionTable:
            548 to 592 -> 596 [0]
            596 to 618 -> 626 [1] lasti
            624 to 624 -> 626 [1] lasti
          consts
             'Handle interval syntax change from Spark to Trino'
             'interval'
@@ -1429,44 +1431,44 @@
                flags     : 51
                code
                   0x95014b00010097007c005d1a7d017c018902a000000000000000000000
                   0000000000000000000000a6000000ab0000000000000000007600560097
                   0101008c1b64005300
                              0 COPY_FREE_VARS           1
                
-               228           2 RETURN_GENERATOR
+               227           2 RETURN_GENERATOR
                              4 POP_TOP
                              6 RESUME                   0
                              8 LOAD_FAST                0 (.0)
                        >>   10 FOR_ITER                26 (to 64)
                
-               230          12 STORE_FAST               1 (known_granularity)
+               229          12 STORE_FAST               1 (known_granularity)
                
-               229          14 LOAD_FAST                1 (known_granularity)
+               228          14 LOAD_FAST                1 (known_granularity)
                             16 LOAD_DEREF               2 (granularity)
                             18 LOAD_METHOD              0 (lower)
                             40 PRECALL                  0
                             44 CALL                     0
                             54 CONTAINS_OP              0
                
-               228          56 YIELD_VALUE
+               227          56 YIELD_VALUE
                             58 RESUME                   1
                             60 POP_TOP
                             62 JUMP_BACKWARD           27 (to 10)
                        >>   64 LOAD_CONST               0 (None)
                             66 RETURN_VALUE
                consts
                   None
                names      ('lower',)
                varnames   ('.0', 'known_granularity')
                freevars   ('granularity',)
                cellvars   ()
                filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
                name       '<genexpr>'
-               firstlineno 228
+               firstlineno 227
                lnotab 0x0c0202ff2aff
             ('second', 'minute', 'hour', 'day', 'week', 'month', 'year')
             's'
             "--week doesn't work in DuneSQL\n"
             "INTERVAL '"
             "' "
             'trino'
@@ -1476,16 +1478,16 @@
          freevars   ()
          cellvars   ('granularity',)
          filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
          name       'interval_fix'
          firstlineno 195
          lnotab
             0x040218022801300114022a032802260104012a024a02340138013e0102
-            013201120108ff0802a601300104032e010201140202fe200c2a0114010c
-            01240104012a025a013c013cfd02052c01
+            013201120108ff0802a601300104032e01140202fe200c2a0114010c0124
+            0104012a025a013c013cfd02052c01
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 7
          flags     : 3
          code
             0x8700970089006a00000000000000000064016b020000000072ed740300
@@ -1503,90 +1505,90 @@
             09a6010000ab010000000000000000a00a00000000000000000000000000
             00000000000000640aa6010000ab010000000000000000640b1900000000
             0000000000640c7a0000007c02a00b000000000000000000000000000000
             0000000000640da6010000ab0100000000000000007a000000640e7a0000
             006408ac0fa6020000ab020000000000000000530089005300
                        0 MAKE_CELL                0 (node)
          
-         255           2 RESUME                   0
+         254           2 RESUME                   0
          
-         257           4 LOAD_DEREF               0 (node)
+         256           4 LOAD_DEREF               0 (node)
                        6 LOAD_ATTR                0 (key)
                       16 LOAD_CONST               1 ('eq')
                       18 COMPARE_OP               2 (==)
                       24 POP_JUMP_FORWARD_IF_FALSE   237 (to 500)
          
-         258          26 LOAD_GLOBAL              3 (NULL + all)
+         257          26 LOAD_GLOBAL              3 (NULL + all)
                       38 LOAD_CLOSURE             0 (node)
                       40 BUILD_TUPLE              1
-                      42 LOAD_CONST               2 (<code object <genexpr>, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 258>)
+                      42 LOAD_CONST               2 (<code object <genexpr>, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 257>)
                       44 MAKE_FUNCTION            8 (closure)
          
-         261          46 LOAD_CONST               3 ('0x')
+         260          46 LOAD_CONST               3 ('0x')
          
-         262          48 LOAD_CONST               4 ('substring(')
+         261          48 LOAD_CONST               4 ('substring(')
          
-         263          50 LOAD_GLOBAL              4 (double_quoted_param_left_placeholder)
+         262          50 LOAD_GLOBAL              4 (double_quoted_param_left_placeholder)
          
-         264          62 LOAD_GLOBAL              6 (double_quoted_param_right_placeholder)
+         263          62 LOAD_GLOBAL              6 (double_quoted_param_right_placeholder)
          
-         260          74 BUILD_TUPLE              4
+         259          74 BUILD_TUPLE              4
          
-         258          76 GET_ITER
+         257          76 GET_ITER
                       78 PRECALL                  0
                       82 CALL                     0
                       92 PRECALL                  1
                       96 CALL                     1
                      106 POP_JUMP_FORWARD_IF_FALSE   196 (to 500)
          
-         269         108 LOAD_CONST               5 ('.*SUBSTRING\\(\\s*[\'\\"]')
+         268         108 LOAD_CONST               5 ('.*SUBSTRING\\(\\s*[\'\\"]')
          
-         270         110 LOAD_GLOBAL              9 (NULL + re)
+         269         110 LOAD_GLOBAL              9 (NULL + re)
                      122 LOAD_ATTR                5 (escape)
                      132 LOAD_GLOBAL              4 (double_quoted_param_left_placeholder)
                      144 PRECALL                  1
                      148 CALL                     1
          
-         269         158 BINARY_OP                0 (+)
+         268         158 BINARY_OP                0 (+)
          
-         271         162 LOAD_CONST               6 ('(.*?)')
+         270         162 LOAD_CONST               6 ('(.*?)')
          
-         269         164 BINARY_OP                0 (+)
+         268         164 BINARY_OP                0 (+)
          
-         272         168 LOAD_GLOBAL              9 (NULL + re)
+         271         168 LOAD_GLOBAL              9 (NULL + re)
                      180 LOAD_ATTR                5 (escape)
                      190 LOAD_GLOBAL              6 (double_quoted_param_right_placeholder)
                      202 PRECALL                  1
                      206 CALL                     1
          
-         269         216 BINARY_OP                0 (+)
+         268         216 BINARY_OP                0 (+)
          
-         273         220 LOAD_CONST               7 ('[\'\\"].*?\\)')
+         272         220 LOAD_CONST               7 ('[\'\\"].*?\\)')
          
-         269         222 BINARY_OP                0 (+)
+         268         222 BINARY_OP                0 (+)
          
-         268         226 STORE_FAST               1 (pattern)
+         267         226 STORE_FAST               1 (pattern)
          
-         275         228 LOAD_GLOBAL              9 (NULL + re)
+         274         228 LOAD_GLOBAL              9 (NULL + re)
                      240 LOAD_ATTR                6 (search)
                      250 LOAD_FAST                1 (pattern)
                      252 LOAD_DEREF               0 (node)
                      254 LOAD_METHOD              7 (sql)
                      276 LOAD_CONST               8 ('trino')
                      278 KW_NAMES                 9
                      280 PRECALL                  1
                      284 CALL                     1
                      294 PRECALL                  2
                      298 CALL                     2
                      308 STORE_FAST               2 (match)
          
-         276         310 LOAD_GLOBAL             17 (NULL + sqlglot)
+         275         310 LOAD_GLOBAL             17 (NULL + sqlglot)
                      322 LOAD_ATTR                9 (parse_one)
          
-         277         332 LOAD_DEREF               0 (node)
+         276         332 LOAD_DEREF               0 (node)
                      334 LOAD_METHOD              7 (sql)
                      356 LOAD_CONST               8 ('trino')
                      358 KW_NAMES                 9
                      360 PRECALL                  1
                      364 CALL                     1
                      374 LOAD_METHOD             10 (split)
                      396 LOAD_CONST              10 ('=')
@@ -1602,20 +1604,20 @@
                      456 PRECALL                  1
                      460 CALL                     1
                      470 BINARY_OP                0 (+)
                      474 LOAD_CONST              14 ('}}")')
                      476 BINARY_OP                0 (+)
                      480 LOAD_CONST               8 ('trino')
          
-         276         482 KW_NAMES                15
+         275         482 KW_NAMES                15
                      484 PRECALL                  2
                      488 CALL                     2
                      498 RETURN_VALUE
          
-         279     >>  500 LOAD_DEREF               0 (node)
+         278     >>  500 LOAD_DEREF               0 (node)
                      502 RETURN_VALUE
          consts
             'Take care of parameters that use bytearrays'
             'eq'
             code
                argcount  : 1
                nlocals   : 2
@@ -1624,35 +1626,35 @@
                code
                   0x95014b00010097007c005d2e7d017c018902a000000000000000000000
                   00000000000000000000006400ac01a6010000ab010000000000000000a0
                   010000000000000000000000000000000000000000a6000000ab00000000
                   000000000076005600970101008c2f64025300
                              0 COPY_FREE_VARS           1
                
-               258           2 RETURN_GENERATOR
+               257           2 RETURN_GENERATOR
                              4 POP_TOP
                              6 RESUME                   0
                              8 LOAD_FAST                0 (.0)
                        >>   10 FOR_ITER                46 (to 104)
                
-               260          12 STORE_FAST               1 (a_param)
+               259          12 STORE_FAST               1 (a_param)
                
-               259          14 LOAD_FAST                1 (a_param)
+               258          14 LOAD_FAST                1 (a_param)
                             16 LOAD_DEREF               2 (node)
                             18 LOAD_METHOD              0 (sql)
                             40 LOAD_CONST               0 ('trino')
                             42 KW_NAMES                 1
                             44 PRECALL                  1
                             48 CALL                     1
                             58 LOAD_METHOD              1 (lower)
                             80 PRECALL                  0
                             84 CALL                     0
                             94 CONTAINS_OP              0
                
-               258          96 YIELD_VALUE
+               257          96 YIELD_VALUE
                             98 RESUME                   1
                            100 POP_TOP
                            102 JUMP_BACKWARD           47 (to 10)
                        >>  104 LOAD_CONST               2 (None)
                            106 RETURN_VALUE
                consts
                   'trino'
@@ -1660,15 +1662,15 @@
                   None
                names      ('sql', 'lower')
                varnames   ('.0', 'a_param')
                freevars   ('node',)
                cellvars   ()
                filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
                name       '<genexpr>'
-               firstlineno 258
+               firstlineno 257
                lnotab 0x0c0202ff52ff
             '0x'
             'substring('
             '.*SUBSTRING\\(\\s*[\'\\"]'
             '(.*?)'
             '[\'\\"].*?\\)'
             'trino'
@@ -1681,15 +1683,15 @@
             ('read',)
          names      ('key', 'all', 'double_quoted_param_left_placeholder', 'double_quoted_param_right_placeholder', 're', 'escape', 'search', 'sql', 'sqlglot', 'parse_one', 'split', 'group')
          varnames   ('node', 'pattern', 'match')
          freevars   ()
          cellvars   ('node',)
          filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
          name       'bytearray_parameter_fix'
-         firstlineno 255
+         firstlineno 254
          lnotab
             0x040216011403020102010c010cfc02fe200b020130ff040202fe040330
             fd040402fc04ff02075201160196ff1203
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 4
@@ -1699,50 +1701,50 @@
             000000000000000000880066016402840864034400a6000000ab00000000
             0000000000a6010000ab0100000000000000007221740500000000000000
             0000006a030000000000000000640489006a0400000000000000007a0000
             0064057a0000006406ac07a6020000ab0200000000000000005300890053
             00
                        0 MAKE_CELL                0 (node)
          
-         282           2 RESUME                   0
+         281           2 RESUME                   0
          
-         285           4 LOAD_DEREF               0 (node)
+         284           4 LOAD_DEREF               0 (node)
                        6 LOAD_ATTR                0 (key)
                       16 LOAD_CONST               1 ('column')
                       18 COMPARE_OP               2 (==)
                       24 POP_JUMP_FORWARD_IF_FALSE    60 (to 146)
          
-         286          26 LOAD_GLOBAL              3 (NULL + any)
+         285          26 LOAD_GLOBAL              3 (NULL + any)
                       38 LOAD_CLOSURE             0 (node)
                       40 BUILD_TUPLE              1
-                      42 LOAD_CONST               2 (<code object <genexpr>, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 286>)
+                      42 LOAD_CONST               2 (<code object <genexpr>, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 285>)
                       44 MAKE_FUNCTION            8 (closure)
                       46 LOAD_CONST               3 (('amount', 'value'))
                       48 GET_ITER
                       50 PRECALL                  0
                       54 CALL                     0
                       64 PRECALL                  1
                       68 CALL                     1
                       78 POP_JUMP_FORWARD_IF_FALSE    33 (to 146)
          
-         287          80 LOAD_GLOBAL              5 (NULL + sqlglot)
+         286          80 LOAD_GLOBAL              5 (NULL + sqlglot)
                       92 LOAD_ATTR                3 (parse_one)
                      102 LOAD_CONST               4 ('cast(')
                      104 LOAD_DEREF               0 (node)
                      106 LOAD_ATTR                4 (name)
                      116 BINARY_OP                0 (+)
                      120 LOAD_CONST               5 (' as double)')
                      122 BINARY_OP                0 (+)
                      126 LOAD_CONST               6 ('trino')
                      128 KW_NAMES                 7
                      130 PRECALL                  2
                      134 CALL                     2
                      144 RETURN_VALUE
          
-         288     >>  146 LOAD_DEREF               0 (node)
+         287     >>  146 LOAD_DEREF               0 (node)
                      148 RETURN_VALUE
          consts
             'if a column is being added, subtracted, multiplied, divided, etc,\n    and it has amount/value in the name, cast to double'
             'column'
             code
                argcount  : 1
                nlocals   : 2
@@ -1750,15 +1752,15 @@
                flags     : 51
                code
                   0x95014b00010097007c005d1f7d017c0189026a000000000000000000a0
                   010000000000000000000000000000000000000000a6000000ab00000000
                   000000000076005600970101008c2064005300
                              0 COPY_FREE_VARS           1
                
-               286           2 RETURN_GENERATOR
+               285           2 RETURN_GENERATOR
                              4 POP_TOP
                              6 RESUME                   0
                              8 LOAD_FAST                0 (.0)
                        >>   10 FOR_ITER                31 (to 74)
                             12 STORE_FAST               1 (val)
                             14 LOAD_FAST                1 (val)
                             16 LOAD_DEREF               2 (node)
@@ -1777,28 +1779,28 @@
                   None
                names      ('name', 'lower')
                varnames   ('.0', 'val')
                freevars   ('node',)
                cellvars   ()
                filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
                name       '<genexpr>'
-               firstlineno 286
+               firstlineno 285
                lnotab 0x
             ('amount', 'value')
             'cast('
             ' as double)'
             'trino'
             ('read',)
          names      ('key', 'any', 'sqlglot', 'parse_one', 'name')
          varnames   ('node',)
          freevars   ()
          cellvars   ('node',)
          filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
          name       'cast_numeric'
-         firstlineno 282
+         firstlineno 281
          lnotab 0x0403160136014201
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 6
          flags     : 3
          code
@@ -1819,37 +1821,37 @@
             000000ab000000000000000000a6010000ab010000000000000000722f74
             09000000000000000000006a050000000000000000640a7c02a00a000000
             0000000000000000000000000000000000640ba6010000ab010000000000
             0000007a000000640c7a0000006403ac06a6020000ab0200000000000000
             00530089005300
                        0 MAKE_CELL                0 (node)
          
-         291           2 RESUME                   0
+         290           2 RESUME                   0
          
-         292           4 LOAD_DEREF               0 (node)
+         291           4 LOAD_DEREF               0 (node)
                        6 LOAD_ATTR                0 (key)
                       16 LOAD_CONST               1 ('literal')
                       18 COMPARE_OP               2 (==)
                       24 EXTENDED_ARG             1
                       26 POP_JUMP_FORWARD_IF_FALSE   257 (to 542)
          
-         294          28 LOAD_GLOBAL              3 (NULL + re)
+         293          28 LOAD_GLOBAL              3 (NULL + re)
                       40 LOAD_ATTR                2 (search)
                       50 LOAD_CONST               2 ('\\d{4}-\\d{2}-\\d{2}')
                       52 LOAD_DEREF               0 (node)
                       54 LOAD_METHOD              3 (sql)
                       76 LOAD_CONST               3 ('trino')
                       78 KW_NAMES                 4
                       80 PRECALL                  1
                       84 CALL                     1
                       94 PRECALL                  2
                       98 CALL                     2
                      108 POP_JUMP_FORWARD_IF_FALSE    45 (to 200)
          
-         295         110 LOAD_GLOBAL              9 (NULL + sqlglot)
+         294         110 LOAD_GLOBAL              9 (NULL + sqlglot)
                      122 LOAD_ATTR                5 (parse_one)
                      132 LOAD_CONST               5 ('timestamp ')
                      134 LOAD_DEREF               0 (node)
                      136 LOAD_METHOD              3 (sql)
                      158 LOAD_CONST               3 ('trino')
                      160 KW_NAMES                 4
                      162 PRECALL                  1
@@ -1857,63 +1859,63 @@
                      176 BINARY_OP                0 (+)
                      180 LOAD_CONST               3 ('trino')
                      182 KW_NAMES                 6
                      184 PRECALL                  2
                      188 CALL                     2
                      198 RETURN_VALUE
          
-         299     >>  200 LOAD_GLOBAL              3 (NULL + re)
+         298     >>  200 LOAD_GLOBAL              3 (NULL + re)
                      212 LOAD_ATTR                6 (escape)
                      222 LOAD_GLOBAL             14 (double_quoted_param_left_placeholder)
                      234 PRECALL                  1
                      238 CALL                     1
          
-         300         248 LOAD_CONST               7 ('(.*?)')
+         299         248 LOAD_CONST               7 ('(.*?)')
          
-         299         250 BINARY_OP                0 (+)
+         298         250 BINARY_OP                0 (+)
          
-         301         254 LOAD_GLOBAL              3 (NULL + re)
+         300         254 LOAD_GLOBAL              3 (NULL + re)
                      266 LOAD_ATTR                6 (escape)
                      276 LOAD_GLOBAL             16 (double_quoted_param_right_placeholder)
                      288 PRECALL                  1
                      292 CALL                     1
          
-         299         302 BINARY_OP                0 (+)
+         298         302 BINARY_OP                0 (+)
          
-         298         306 STORE_FAST               1 (pattern)
+         297         306 STORE_FAST               1 (pattern)
          
-         303         308 LOAD_GLOBAL              3 (NULL + re)
+         302         308 LOAD_GLOBAL              3 (NULL + re)
                      320 LOAD_ATTR                2 (search)
                      330 LOAD_FAST                1 (pattern)
                      332 LOAD_DEREF               0 (node)
                      334 LOAD_METHOD              3 (sql)
                      356 LOAD_CONST               3 ('trino')
                      358 KW_NAMES                 4
                      360 PRECALL                  1
                      364 CALL                     1
                      374 PRECALL                  2
                      378 CALL                     2
                      388 STORE_FAST               2 (match)
          
-         304         390 LOAD_FAST                2 (match)
+         303         390 LOAD_FAST                2 (match)
                      392 POP_JUMP_FORWARD_IF_FALSE    74 (to 542)
                      394 LOAD_GLOBAL             19 (NULL + any)
                      406 LOAD_CLOSURE             0 (node)
                      408 BUILD_TUPLE              1
-                     410 LOAD_CONST               8 (<code object <genexpr>, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 304>)
+                     410 LOAD_CONST               8 (<code object <genexpr>, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 303>)
                      412 MAKE_FUNCTION            8 (closure)
                      414 LOAD_CONST               9 (('date', 'time'))
                      416 GET_ITER
                      418 PRECALL                  0
                      422 CALL                     0
                      432 PRECALL                  1
                      436 CALL                     1
                      446 POP_JUMP_FORWARD_IF_FALSE    47 (to 542)
          
-         305         448 LOAD_GLOBAL              9 (NULL + sqlglot)
+         304         448 LOAD_GLOBAL              9 (NULL + sqlglot)
                      460 LOAD_ATTR                5 (parse_one)
                      470 LOAD_CONST              10 ("timestamp '{{")
                      472 LOAD_FAST                2 (match)
                      474 LOAD_METHOD             10 (group)
                      496 LOAD_CONST              11 (1)
                      498 PRECALL                  1
                      502 CALL                     1
@@ -1922,15 +1924,15 @@
                      518 BINARY_OP                0 (+)
                      522 LOAD_CONST               3 ('trino')
                      524 KW_NAMES                 6
                      526 PRECALL                  2
                      530 CALL                     2
                      540 RETURN_VALUE
          
-         306     >>  542 LOAD_DEREF               0 (node)
+         305     >>  542 LOAD_DEREF               0 (node)
                      544 RETURN_VALUE
          consts
             None
             'literal'
             '\\d{4}-\\d{2}-\\d{2}'
             'trino'
             ('dialect',)
@@ -1945,15 +1947,15 @@
                code
                   0x95014b00010097007c005d2e7d017c018902a000000000000000000000
                   00000000000000000000006400ac01a6010000ab010000000000000000a0
                   010000000000000000000000000000000000000000a6000000ab00000000
                   000000000076005600970101008c2f64025300
                              0 COPY_FREE_VARS           1
                
-               304           2 RETURN_GENERATOR
+               303           2 RETURN_GENERATOR
                              4 POP_TOP
                              6 RESUME                   0
                              8 LOAD_FAST                0 (.0)
                        >>   10 FOR_ITER                46 (to 104)
                             12 STORE_FAST               1 (d)
                             14 LOAD_FAST                1 (d)
                             16 LOAD_DEREF               2 (node)
@@ -1978,27 +1980,27 @@
                   None
                names      ('sql', 'lower')
                varnames   ('.0', 'd')
                freevars   ('node',)
                cellvars   ()
                filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
                name       '<genexpr>'
-               firstlineno 304
+               firstlineno 303
                lnotab 0x
             ('date', 'time')
             "timestamp '{{"
             1
             "}}'"
          names      ('key', 're', 'search', 'sql', 'sqlglot', 'parse_one', 'escape', 'double_quoted_param_left_placeholder', 'double_quoted_param_right_placeholder', 'any', 'group')
          varnames   ('node', 'pattern', 'match')
          freevars   ()
          cellvars   ('node',)
          filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
          name       'cast_timestamp'
-         firstlineno 291
+         firstlineno 290
          lnotab 0x0401180252015a04300102ff040230fe04ff020552013a015e01
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 4
          flags     : 3
          code
@@ -2009,36 +2011,36 @@
             000000a003000000000000000000000000000000000000000064066407a6
             020000ab020000000000000000a003000000000000000000000000000000
             000000000064086407a6020000ab0200000000000000007d017409000000
             000000000000006a0500000000000000007c016404ac09a6020000ab0200
             00000000000000530089005300
                        0 MAKE_CELL                0 (node)
          
-         309           2 RESUME                   0
+         308           2 RESUME                   0
          
-         311           4 LOAD_DEREF               0 (node)
+         310           4 LOAD_DEREF               0 (node)
                        6 LOAD_ATTR                0 (key)
                       16 LOAD_CONST               1 ('literal')
                       18 COMPARE_OP               2 (==)
                       24 POP_JUMP_FORWARD_IF_FALSE   111 (to 248)
          
-         312          26 LOAD_GLOBAL              3 (NULL + any)
+         311          26 LOAD_GLOBAL              3 (NULL + any)
                       38 LOAD_CLOSURE             0 (node)
                       40 BUILD_TUPLE              1
-                      42 LOAD_CONST               2 (<code object <genexpr>, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 312>)
+                      42 LOAD_CONST               2 (<code object <genexpr>, file "/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py", line 311>)
                       44 MAKE_FUNCTION            8 (closure)
                       46 LOAD_CONST               3 (('true', 'false'))
                       48 GET_ITER
                       50 PRECALL                  0
                       54 CALL                     0
                       64 PRECALL                  1
                       68 CALL                     1
                       78 POP_JUMP_FORWARD_IF_FALSE    84 (to 248)
          
-         314          80 LOAD_DEREF               0 (node)
+         313          80 LOAD_DEREF               0 (node)
                       82 LOAD_METHOD              2 (sql)
                      104 LOAD_CONST               4 ('trino')
                      106 KW_NAMES                 5
                      108 PRECALL                  1
                      112 CALL                     1
                      122 LOAD_METHOD              3 (replace)
                      144 LOAD_CONST               6 ('"')
@@ -2048,24 +2050,24 @@
                      162 LOAD_METHOD              3 (replace)
                      184 LOAD_CONST               8 ("'")
                      186 LOAD_CONST               7 ('')
                      188 PRECALL                  2
                      192 CALL                     2
                      202 STORE_FAST               1 (bool_cleaned)
          
-         315         204 LOAD_GLOBAL              9 (NULL + sqlglot)
+         314         204 LOAD_GLOBAL              9 (NULL + sqlglot)
                      216 LOAD_ATTR                5 (parse_one)
                      226 LOAD_FAST                1 (bool_cleaned)
                      228 LOAD_CONST               4 ('trino')
                      230 KW_NAMES                 9
                      232 PRECALL                  2
                      236 CALL                     2
                      246 RETURN_VALUE
          
-         316     >>  248 LOAD_DEREF               0 (node)
+         315     >>  248 LOAD_DEREF               0 (node)
                      250 RETURN_VALUE
          consts
             "If node.key is 'literal' and contains 'true' or 'false' then cast to boolean"
             'literal'
             code
                argcount  : 1
                nlocals   : 2
@@ -2074,15 +2076,15 @@
                code
                   0x95014b00010097007c005d2e7d017c018902a000000000000000000000
                   00000000000000000000006400ac01a6010000ab010000000000000000a0
                   010000000000000000000000000000000000000000a6000000ab00000000
                   000000000076005600970101008c2f64025300
                              0 COPY_FREE_VARS           1
                
-               312           2 RETURN_GENERATOR
+               311           2 RETURN_GENERATOR
                              4 POP_TOP
                              6 RESUME                   0
                              8 LOAD_FAST                0 (.0)
                        >>   10 FOR_ITER                46 (to 104)
                             12 STORE_FAST               1 (boolean)
                             14 LOAD_FAST                1 (boolean)
                             16 LOAD_DEREF               2 (node)
@@ -2107,232 +2109,232 @@
                   None
                names      ('sql', 'lower')
                varnames   ('.0', 'boolean')
                freevars   ('node',)
                cellvars   ()
                filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
                name       '<genexpr>'
-               firstlineno 312
+               firstlineno 311
                lnotab 0x
             ('true', 'false')
             'trino'
             ('dialect',)
             '"'
             ''
             "'"
             ('read',)
          names      ('key', 'any', 'sql', 'replace', 'sqlglot', 'parse_one')
          varnames   ('node', 'bool_cleaned')
          freevars   ()
          cellvars   ('node',)
          filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
          name       'fix_boolean'
-         firstlineno 309
+         firstlineno 308
          lnotab 0x0402160136027c012c01
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 5
          flags     : 3
          code
             0x97007c006a000000000000000000a00100000000000000000000000000
             00000000000000a6000000ab00000000000000000064017600722d740500
             0000000000000000006a0300000000000000007c00a00400000000000000
             000000000000000000000000006402ac03a6010000ab0100000000000000
             0064047a0000006402ac05a6020000ab02000000000000000053007c0053
             00
-         319           0 RESUME                   0
+         318           0 RESUME                   0
          
-         321           2 LOAD_FAST                0 (node)
+         320           2 LOAD_FAST                0 (node)
                        4 LOAD_ATTR                0 (name)
                       14 LOAD_METHOD              1 (lower)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 LOAD_CONST               1 (('unnest', 'explode'))
                       52 CONTAINS_OP              0
                       54 POP_JUMP_FORWARD_IF_FALSE    45 (to 146)
          
-         322          56 LOAD_GLOBAL              5 (NULL + sqlglot)
+         321          56 LOAD_GLOBAL              5 (NULL + sqlglot)
                       68 LOAD_ATTR                3 (parse_one)
          
-         323          78 LOAD_FAST                0 (node)
+         322          78 LOAD_FAST                0 (node)
                       80 LOAD_METHOD              4 (sql)
                      102 LOAD_CONST               2 ('trino')
                      104 KW_NAMES                 3
                      106 PRECALL                  1
                      110 CALL                     1
          
-         325         120 LOAD_CONST               4 ("-- WARNING: You can't use explode/unnest inside SELECT anymore, it must be LATERAL or CROSS JOIN instead. Check out the docs here: https://dune.com/docs/query/syntax-differences/")
+         324         120 LOAD_CONST               4 ("-- WARNING: You can't use explode/unnest inside SELECT anymore, it must be LATERAL or CROSS JOIN instead. Check out the docs here: https://dune.com/docs/query/syntax-differences/")
          
-         323         122 BINARY_OP                0 (+)
+         322         122 BINARY_OP                0 (+)
          
-         328         126 LOAD_CONST               2 ('trino')
+         327         126 LOAD_CONST               2 ('trino')
          
-         322         128 KW_NAMES                 5
+         321         128 KW_NAMES                 5
                      130 PRECALL                  2
                      134 CALL                     2
                      144 RETURN_VALUE
          
-         330     >>  146 LOAD_FAST                0 (node)
+         329     >>  146 LOAD_FAST                0 (node)
                      148 RETURN_VALUE
          consts
             'Add a warning to the query if there is an unnest function call'
             ('unnest', 'explode')
             'trino'
             ('dialect',)
             "-- WARNING: You can't use explode/unnest inside SELECT anymore, it must be LATERAL or CROSS JOIN instead. Check out the docs here: https://dune.com/docs/query/syntax-differences/"
             ('read',)
          names      ('name', 'lower', 'sqlglot', 'parse_one', 'sql')
          varnames   ('node',)
          freevars   ()
          cellvars   ()
          filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
          name       'warn_unnest'
-         firstlineno 319
+         firstlineno 318
          lnotab 0x0202360116012a0202fe040502fa1208
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 5
          flags     : 3
          code
             0x97007c006a000000000000000000a00100000000000000000000000000
             00000000000000a6000000ab00000000000000000064017600722d740500
             0000000000000000006a0300000000000000007c00a00400000000000000
             000000000000000000000000006402ac03a6010000ab0100000000000000
             0064047a0000006402ac05a6020000ab02000000000000000053007c0053
             00
-         333           0 RESUME                   0
+         332           0 RESUME                   0
          
-         335           2 LOAD_FAST                0 (node)
+         334           2 LOAD_FAST                0 (node)
                        4 LOAD_ATTR                0 (name)
                       14 LOAD_METHOD              1 (lower)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 LOAD_CONST               1 (('generate_series', 'sequence'))
                       52 CONTAINS_OP              0
                       54 POP_JUMP_FORWARD_IF_FALSE    45 (to 146)
          
-         336          56 LOAD_GLOBAL              5 (NULL + sqlglot)
+         335          56 LOAD_GLOBAL              5 (NULL + sqlglot)
                       68 LOAD_ATTR                3 (parse_one)
          
-         337          78 LOAD_FAST                0 (node)
+         336          78 LOAD_FAST                0 (node)
                       80 LOAD_METHOD              4 (sql)
                      102 LOAD_CONST               2 ('trino')
                      104 KW_NAMES                 3
                      106 PRECALL                  1
                      110 CALL                     1
          
-         339         120 LOAD_CONST               4 ('-- WARNING: Check out the docs for example of time series generation: https://dune.com/docs/query/syntax-differences/')
+         338         120 LOAD_CONST               4 ('-- WARNING: Check out the docs for example of time series generation: https://dune.com/docs/query/syntax-differences/')
          
-         337         122 BINARY_OP                0 (+)
+         336         122 BINARY_OP                0 (+)
          
-         342         126 LOAD_CONST               2 ('trino')
+         341         126 LOAD_CONST               2 ('trino')
          
-         336         128 KW_NAMES                 5
+         335         128 KW_NAMES                 5
                      130 PRECALL                  2
                      134 CALL                     2
                      144 RETURN_VALUE
          
-         344     >>  146 LOAD_FAST                0 (node)
+         343     >>  146 LOAD_FAST                0 (node)
                      148 RETURN_VALUE
          consts
             'Add a warning that links to docs if the query uses generate_series/sequence'
             ('generate_series', 'sequence')
             'trino'
             ('dialect',)
             '-- WARNING: Check out the docs for example of time series generation: https://dune.com/docs/query/syntax-differences/'
             ('read',)
          names      ('name', 'lower', 'sqlglot', 'parse_one', 'sql')
          varnames   ('node',)
          freevars   ()
          cellvars   ()
          filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
          name       'warn_sequence'
-         firstlineno 333
+         firstlineno 332
          lnotab 0x0202360116012a0202fe040502fa1208
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 7
          flags     : 3
          code
             0x9700640144005d427d017401000000000000000000006a010000000000
             00000064027401000000000000000000006a0200000000000000007c01a6
             010000ab0100000000000000007a00000064037a00000064047c017a0000
             0064047a0000007c007400000000000000000000006a0300000000000000
             00ac05a6040000ab0400000000000000007d008c437c005300
-         347           0 RESUME                   0
+         346           0 RESUME                   0
          
-         348           2 LOAD_CONST               1 (('replace',))
+         347           2 LOAD_CONST               1 (('replace',))
                        4 GET_ITER
                  >>    6 FOR_ITER                66 (to 140)
                        8 STORE_FAST               1 (keyword)
          
-         350          10 LOAD_GLOBAL              1 (NULL + re)
+         349          10 LOAD_GLOBAL              1 (NULL + re)
                       22 LOAD_ATTR                1 (sub)
          
-         351          32 LOAD_CONST               2 ('\\b')
+         350          32 LOAD_CONST               2 ('\\b')
                       34 LOAD_GLOBAL              1 (NULL + re)
                       46 LOAD_ATTR                2 (escape)
                       56 LOAD_FAST                1 (keyword)
                       58 PRECALL                  1
                       62 CALL                     1
                       72 BINARY_OP                0 (+)
                       76 LOAD_CONST               3 ('(?!\\()')
                       78 BINARY_OP                0 (+)
          
-         352          82 LOAD_CONST               4 ('"')
+         351          82 LOAD_CONST               4 ('"')
                       84 LOAD_FAST                1 (keyword)
                       86 BINARY_OP                0 (+)
                       90 LOAD_CONST               4 ('"')
                       92 BINARY_OP                0 (+)
          
-         353          96 LOAD_FAST                0 (query)
+         352          96 LOAD_FAST                0 (query)
          
-         354          98 LOAD_GLOBAL              0 (re)
+         353          98 LOAD_GLOBAL              0 (re)
                      110 LOAD_ATTR                3 (IGNORECASE)
          
-         350         120 KW_NAMES                 5
+         349         120 KW_NAMES                 5
                      122 PRECALL                  4
                      126 CALL                     4
                      136 STORE_FAST               0 (query)
                      138 JUMP_BACKWARD           67 (to 6)
          
-         356     >>  140 LOAD_FAST                0 (query)
+         355     >>  140 LOAD_FAST                0 (query)
                      142 RETURN_VALUE
          consts
             None
             ('replace',)
             '\\b'
             '(?!\\()'
             '"'
             ('flags',)
          names      ('re', 'sub', 'escape', 'IGNORECASE')
          varnames   ('query', 'keyword')
          freevars   ()
          cellvars   ()
          filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
          name       'prep_query'
-         firstlineno 347
+         firstlineno 346
          lnotab 0x02010802160132010e01020116fc1406
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 6
          flags     : 3
          code
             0x97007401000000000000000000006a0100000000000000007c00a00200
             000000000000000000000000000000000000006401ac02a6010000ab0100
             00000000000000a003000000000000000000000000000000000000000064
             036404a6020000ab0200000000000000006401ac05a6020000ab02000000
             00000000005300
-         359           0 RESUME                   0
+         358           0 RESUME                   0
          
-         361           2 LOAD_GLOBAL              1 (NULL + sqlglot)
+         360           2 LOAD_GLOBAL              1 (NULL + sqlglot)
                       14 LOAD_ATTR                1 (parse_one)
                       24 LOAD_FAST                0 (query)
                       26 LOAD_METHOD              2 (sql)
                       48 LOAD_CONST               1 ('trino')
                       50 KW_NAMES                 2
                       52 PRECALL                  1
                       56 CALL                     1
@@ -2355,15 +2357,15 @@
             ('read',)
          names      ('sqlglot', 'parse_one', 'sql', 'replace')
          varnames   ('query',)
          freevars   ()
          cellvars   ()
          filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
          name       'rename_amount_column'
-         firstlineno 359
+         firstlineno 358
          lnotab 0x0202
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 6
          flags     : 3
          code
@@ -2371,52 +2373,52 @@
             02a6010000ab0100000000000000007d0164037c01a00100000000000000
             00000000000000000000000000a6000000ab000000000000000000760072
             277405000000000000000000006a030000000000000000640364047c0174
             04000000000000000000006a040000000000000000ac05a6040000ab0400
             000000000000007d0164067c017a0000007d01740b000000000000000000
             006a0600000000000000007c016401ac07a6020000ab0200000000000000
             005300
-         364           0 RESUME                   0
+         363           0 RESUME                   0
          
-         366           2 LOAD_FAST                0 (node)
+         365           2 LOAD_FAST                0 (node)
                        4 LOAD_METHOD              0 (sql)
                       26 LOAD_CONST               1 ('trino')
                       28 KW_NAMES                 2
                       30 PRECALL                  1
                       34 CALL                     1
                       44 STORE_FAST               1 (query)
          
-         367          46 LOAD_CONST               3 ('bytea2numeric')
+         366          46 LOAD_CONST               3 ('bytea2numeric')
                       48 LOAD_FAST                1 (query)
                       50 LOAD_METHOD              1 (lower)
                       72 PRECALL                  0
                       76 CALL                     0
                       86 CONTAINS_OP              0
                       88 POP_JUMP_FORWARD_IF_FALSE    39 (to 168)
          
-         368          90 LOAD_GLOBAL              5 (NULL + re)
+         367          90 LOAD_GLOBAL              5 (NULL + re)
                      102 LOAD_ATTR                3 (sub)
                      112 LOAD_CONST               3 ('bytea2numeric')
                      114 LOAD_CONST               4 ('bytearray_to_bigint')
                      116 LOAD_FAST                1 (query)
                      118 LOAD_GLOBAL              4 (re)
                      130 LOAD_ATTR                4 (IGNORECASE)
                      140 KW_NAMES                 5
                      142 PRECALL                  4
                      146 CALL                     4
                      156 STORE_FAST               1 (query)
          
-         370         158 LOAD_CONST               6 ('/* !Bytea warning: We now have new bytearray functions to cover conversions and stuff like length, concat, substring, etc. Check out the docs here: https://dune.com/docs/reference/dune-v2/query-engine/#byte-array-to-numeric-functions */\n\n')
+         369         158 LOAD_CONST               6 ('/* !Bytea warning: We now have new bytearray functions to cover conversions and stuff like length, concat, substring, etc. Check out the docs here: https://dune.com/docs/reference/dune-v2/query-engine/#byte-array-to-numeric-functions */\n\n')
          
-         374         160 LOAD_FAST                1 (query)
+         373         160 LOAD_FAST                1 (query)
          
-         369         162 BINARY_OP                0 (+)
+         368         162 BINARY_OP                0 (+)
                      166 STORE_FAST               1 (query)
          
-         375     >>  168 LOAD_GLOBAL             11 (NULL + sqlglot)
+         374     >>  168 LOAD_GLOBAL             11 (NULL + sqlglot)
                      180 LOAD_ATTR                6 (parse_one)
                      190 LOAD_FAST                1 (query)
                      192 LOAD_CONST               1 ('trino')
                      194 KW_NAMES                 7
                      196 PRECALL                  2
                      200 CALL                     2
                      210 RETURN_VALUE
@@ -2431,31 +2433,31 @@
             ('read',)
          names      ('sql', 'lower', 're', 'sub', 'IGNORECASE', 'sqlglot', 'parse_one')
          varnames   ('node', 'query')
          freevars   ()
          cellvars   ()
          filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
          name       'bytea2numeric'
-         firstlineno 364
+         firstlineno 363
          lnotab 0x02022c012c014402020402fb0606
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 6
          flags     : 3
          code
             0x970064017d017401000000000000000000006a0100000000000000007c
             0164027c007400000000000000000000006a020000000000000000ac03a6
             040000ab0400000000000000005300
-         378           0 RESUME                   0
+         377           0 RESUME                   0
          
-         380           2 LOAD_CONST               1 ('lower\\(\\s*[\'\\"]\\{\\{(.*?)\\}\\}[\'\\"]\\s*\\)')
+         379           2 LOAD_CONST               1 ('lower\\(\\s*[\'\\"]\\{\\{(.*?)\\}\\}[\'\\"]\\s*\\)')
                        4 STORE_FAST               1 (pattern)
          
-         381           6 LOAD_GLOBAL              1 (NULL + re)
+         380           6 LOAD_GLOBAL              1 (NULL + re)
                       18 LOAD_ATTR                1 (sub)
                       28 LOAD_FAST                1 (pattern)
                       30 LOAD_CONST               2 ('{{\\1}}')
                       32 LOAD_FAST                0 (query)
                       34 LOAD_GLOBAL              0 (re)
                       46 LOAD_ATTR                2 (IGNORECASE)
                       56 KW_NAMES                 3
@@ -2469,95 +2471,95 @@
             ('flags',)
          names      ('re', 'sub', 'IGNORECASE')
          varnames   ('query', 'pattern')
          freevars   ()
          cellvars   ()
          filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
          name       'fix_bytearray_param'
-         firstlineno 378
+         firstlineno 377
          lnotab 0x02020401
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 6
          flags     : 3
          code
             0x970064017d017401000000000000000000006a0100000000000000007c
             0164027c007400000000000000000000006a020000000000000000ac03a6
             040000ab0400000000000000007d027c025300
-         384           0 RESUME                   0
+         383           0 RESUME                   0
          
-         388           2 LOAD_CONST               1 ('lower\\(\\s*[\'\\"]0x(.*?)[\'\\"]\\s*\\)')
+         387           2 LOAD_CONST               1 ('lower\\(\\s*[\'\\"]0x(.*?)[\'\\"]\\s*\\)')
                        4 STORE_FAST               1 (pattern)
          
-         389           6 LOAD_GLOBAL              1 (NULL + re)
+         388           6 LOAD_GLOBAL              1 (NULL + re)
                       18 LOAD_ATTR                1 (sub)
                       28 LOAD_FAST                1 (pattern)
                       30 LOAD_CONST               2 ('0x\\1')
                       32 LOAD_FAST                0 (query)
                       34 LOAD_GLOBAL              0 (re)
                       46 LOAD_ATTR                2 (IGNORECASE)
                       56 KW_NAMES                 3
                       58 PRECALL                  4
                       62 CALL                     4
                       72 STORE_FAST               2 (substituted)
          
-         390          74 LOAD_FAST                2 (substituted)
+         389          74 LOAD_FAST                2 (substituted)
                       76 RETURN_VALUE
          consts
             "Remove lower function call around '0x...' string literals, and remove the string since we have native hex types.\n\n    This has to happen after SQLGlot, since it will parse a bare 0x as a string literal"
             'lower\\(\\s*[\'\\"]0x(.*?)[\'\\"]\\s*\\)'
             '0x\\1'
             ('flags',)
          names      ('re', 'sub', 'IGNORECASE')
          varnames   ('query', 'pattern', 'substituted')
          freevars   ()
          cellvars   ()
          filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
          name       'fix_bytearray_lower'
-         firstlineno 384
+         firstlineno 383
          lnotab 0x020404014401
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 6
          flags     : 3
          code
             0x9700740000000000000000000000740200000000000000000000740400
             000000000000000000740600000000000000000000740800000000000000
             00000064019c057c00190000000000000000005300
-         393           0 RESUME                   0
+         392           0 RESUME                   0
          
-         395           2 LOAD_GLOBAL              0 (chain_where_gnosis)
+         394           2 LOAD_GLOBAL              0 (chain_where_gnosis)
          
-         396          14 LOAD_GLOBAL              2 (chain_where_optimism)
+         395          14 LOAD_GLOBAL              2 (chain_where_optimism)
          
-         397          26 LOAD_GLOBAL              4 (chain_where_bnb)
+         396          26 LOAD_GLOBAL              4 (chain_where_bnb)
          
-         398          38 LOAD_GLOBAL              6 (chain_where_polygon)
+         397          38 LOAD_GLOBAL              6 (chain_where_polygon)
          
-         399          50 LOAD_GLOBAL              8 (chain_where_ethereum)
+         398          50 LOAD_GLOBAL              8 (chain_where_ethereum)
          
-         394          62 LOAD_CONST               1 (('gnosis', 'optimism', 'bnb', 'polygon', 'ethereum'))
+         393          62 LOAD_CONST               1 (('gnosis', 'optimism', 'bnb', 'polygon', 'ethereum'))
                       64 BUILD_CONST_KEY_MAP      5
          
-         400          66 LOAD_FAST                0 (dataset)
+         399          66 LOAD_FAST                0 (dataset)
          
-         394          68 BINARY_SUBSCR
+         393          68 BINARY_SUBSCR
                       78 RETURN_VALUE
          consts
             None
             ('gnosis', 'optimism', 'bnb', 'polygon', 'ethereum')
          names      ('chain_where_gnosis', 'chain_where_optimism', 'chain_where_bnb', 'chain_where_polygon', 'chain_where_ethereum')
          varnames   ('dataset',)
          freevars   ()
          cellvars   ()
          filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
          name       'chain_where'
-         firstlineno 393
+         firstlineno 392
          lnotab 0x02020c010c010c010c010cfb040602fa
       code
          argcount  : 2
          nlocals   : 5
          stacksize : 12
          flags     : 3
          code
@@ -2567,260 +2569,330 @@
             000000000000000000740a00000000000000000000740c00000000000000
             000000740e00000000000000000000741000000000000000000000741200
             0000000000000000007415000000000000000000007c01a6010000ab0100
             000000000000007416000000000000000000007418000000000000000000
             00741a00000000000000000000660c7d037c0344005d177d047c02a00e00
             000000000000000000000000000000000000007c04a6010000ab01000000
             00000000007d028c187c025300
-         403           0 RESUME                   0
+         402           0 RESUME                   0
          
-         407           2 LOAD_GLOBAL              1 (NULL + sqlglot)
+         406           2 LOAD_GLOBAL              1 (NULL + sqlglot)
                       14 LOAD_ATTR                1 (parse_one)
                       24 LOAD_FAST                0 (query)
                       26 LOAD_CONST               1 ('postgres')
                       28 KW_NAMES                 2
                       30 PRECALL                  2
                       34 CALL                     2
                       44 STORE_FAST               2 (query_tree)
          
-         409          46 LOAD_GLOBAL              5 (NULL + postgres_table_replacements)
+         408          46 LOAD_GLOBAL              5 (NULL + postgres_table_replacements)
                       58 LOAD_FAST                1 (dataset)
                       60 PRECALL                  1
                       64 CALL                     1
          
-         410          74 LOAD_GLOBAL              6 (interval_fix)
+         409          74 LOAD_GLOBAL              6 (interval_fix)
          
-         411          86 LOAD_GLOBAL              8 (fix_boolean)
+         410          86 LOAD_GLOBAL              8 (fix_boolean)
          
-         412          98 LOAD_GLOBAL             10 (cast_numeric)
+         411          98 LOAD_GLOBAL             10 (cast_numeric)
          
-         413         110 LOAD_GLOBAL             12 (cast_timestamp)
+         412         110 LOAD_GLOBAL             12 (cast_timestamp)
          
-         414         122 LOAD_GLOBAL             14 (warn_unnest)
+         413         122 LOAD_GLOBAL             14 (warn_unnest)
          
-         415         134 LOAD_GLOBAL             16 (warn_sequence)
+         414         134 LOAD_GLOBAL             16 (warn_sequence)
          
-         416         146 LOAD_GLOBAL             18 (dex_trades_fixes)
+         415         146 LOAD_GLOBAL             18 (dex_trades_fixes)
          
-         417         158 LOAD_GLOBAL             21 (NULL + chain_where)
+         416         158 LOAD_GLOBAL             21 (NULL + chain_where)
                      170 LOAD_FAST                1 (dataset)
                      172 PRECALL                  1
                      176 CALL                     1
          
-         418         186 LOAD_GLOBAL             22 (bytearray_parameter_fix)
+         417         186 LOAD_GLOBAL             22 (bytearray_parameter_fix)
          
-         419         198 LOAD_GLOBAL             24 (rename_amount_column)
+         418         198 LOAD_GLOBAL             24 (rename_amount_column)
          
-         420         210 LOAD_GLOBAL             26 (bytea2numeric)
+         419         210 LOAD_GLOBAL             26 (bytea2numeric)
          
-         408         222 BUILD_TUPLE             12
+         407         222 BUILD_TUPLE             12
                      224 STORE_FAST               3 (transforms)
          
-         422         226 LOAD_FAST                3 (transforms)
+         421         226 LOAD_FAST                3 (transforms)
                      228 GET_ITER
                  >>  230 FOR_ITER                23 (to 278)
                      232 STORE_FAST               4 (f)
          
-         423         234 LOAD_FAST                2 (query_tree)
+         422         234 LOAD_FAST                2 (query_tree)
                      236 LOAD_METHOD             14 (transform)
                      258 LOAD_FAST                4 (f)
                      260 PRECALL                  1
                      264 CALL                     1
                      274 STORE_FAST               2 (query_tree)
                      276 JUMP_BACKWARD           24 (to 230)
          
-         424     >>  278 LOAD_FAST                2 (query_tree)
+         423     >>  278 LOAD_FAST                2 (query_tree)
                      280 RETURN_VALUE
          consts
             "Apply a series of transforms to the query tree, recursively using SQLGlot's recursive transform function.\n\n    Each transform takes and returns a sqlglot.Expression"
             'postgres'
             ('read',)
          names      ('sqlglot', 'parse_one', 'postgres_table_replacements', 'interval_fix', 'fix_boolean', 'cast_numeric', 'cast_timestamp', 'warn_unnest', 'warn_sequence', 'dex_trades_fixes', 'chain_where', 'bytearray_parameter_fix', 'rename_amount_column', 'bytea2numeric', 'transform')
          varnames   ('query', 'dataset', 'query_tree', 'transforms', 'f')
          freevars   ()
          cellvars   ()
          filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
          name       'postgres_transforms'
-         firstlineno 403
+         firstlineno 402
          lnotab
             0x02042c021c010c010c010c010c010c010c010c011c010c010c010cf404
             0e08012c01
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 6
          flags     : 3
          code
             0x970064017d017401000000000000000000006a0100000000000000007c
             0164027c007400000000000000000000006a020000000000000000ac03a6
             040000ab0400000000000000007d027c025300
-         427           0 RESUME                   0
+         426           0 RESUME                   0
          
-         431           2 LOAD_CONST               1 ("'0x(.*?)'")
+         430           2 LOAD_CONST               1 ("'0x(.*?)'")
                        4 STORE_FAST               1 (pattern)
          
-         432           6 LOAD_GLOBAL              1 (NULL + re)
+         431           6 LOAD_GLOBAL              1 (NULL + re)
                       18 LOAD_ATTR                1 (sub)
                       28 LOAD_FAST                1 (pattern)
                       30 LOAD_CONST               2 ('0x\\1')
                       32 LOAD_FAST                0 (query)
                       34 LOAD_GLOBAL              0 (re)
                       46 LOAD_ATTR                2 (IGNORECASE)
                       56 KW_NAMES                 3
                       58 PRECALL                  4
                       62 CALL                     4
                       72 STORE_FAST               2 (substituted)
          
-         433          74 LOAD_FAST                2 (substituted)
+         432          74 LOAD_FAST                2 (substituted)
                       76 RETURN_VALUE
          consts
             "Remove string quotes around '0x...' string literals\n\n    This has to happen after SQLGlot, since it will parse a bare 0x as a string literal"
             "'0x(.*?)'"
             '0x\\1'
             ('flags',)
          names      ('re', 'sub', 'IGNORECASE')
          varnames   ('query', 'pattern', 'substituted')
          freevars   ()
          cellvars   ()
          filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
          name       'remove_quotes_around_0x_strings'
-         firstlineno 427
+         firstlineno 426
          lnotab 0x020404014401
       code
          argcount  : 1
+         nlocals   : 2
+         stacksize : 6
+         flags     : 3
+         code
+            0x97007c00a00000000000000000000000000000000000000000006401ac
+            02a6010000ab0100000000000000007d0164037c01a00100000000000000
+            00000000000000000000000000a6000000ab000000000000000000760072
+            227405000000000000000000006a030000000000000000640464057c0174
+            04000000000000000000006a040000000000000000ac06a6040000ab0400
+            000000000000007d01740b000000000000000000006a0600000000000000
+            007c016401ac07a6020000ab0200000000000000005300
+         435           0 RESUME                   0
+         
+         437           2 LOAD_FAST                0 (node)
+                       4 LOAD_METHOD              0 (sql)
+                      26 LOAD_CONST               1 ('trino')
+                      28 KW_NAMES                 2
+                      30 PRECALL                  1
+                      34 CALL                     1
+                      44 STORE_FAST               1 (query)
+         
+         438          46 LOAD_CONST               3 ('timestamp(')
+                      48 LOAD_FAST                1 (query)
+                      50 LOAD_METHOD              1 (lower)
+                      72 PRECALL                  0
+                      76 CALL                     0
+                      86 CONTAINS_OP              0
+                      88 POP_JUMP_FORWARD_IF_FALSE    34 (to 158)
+         
+         439          90 LOAD_GLOBAL              5 (NULL + re)
+                     102 LOAD_ATTR                3 (sub)
+                     112 LOAD_CONST               4 ('timestamp')
+                     114 LOAD_CONST               5 ('from_unixtime')
+                     116 LOAD_FAST                1 (query)
+                     118 LOAD_GLOBAL              4 (re)
+                     130 LOAD_ATTR                4 (IGNORECASE)
+                     140 KW_NAMES                 6
+                     142 PRECALL                  4
+                     146 CALL                     4
+                     156 STORE_FAST               1 (query)
+         
+         440     >>  158 LOAD_GLOBAL             11 (NULL + sqlglot)
+                     170 LOAD_ATTR                6 (parse_one)
+                     180 LOAD_FAST                1 (query)
+                     182 LOAD_CONST               1 ('trino')
+                     184 KW_NAMES                 7
+                     186 PRECALL                  2
+                     190 CALL                     2
+                     200 RETURN_VALUE
+         consts
+            "Replace the Spark timestamp() function with Trino's from_unixtime() function"
+            'trino'
+            ('dialect',)
+            'timestamp('
+            'timestamp'
+            'from_unixtime'
+            ('flags',)
+            ('read',)
+         names      ('sql', 'lower', 're', 'sub', 'IGNORECASE', 'sqlglot', 'parse_one')
+         varnames   ('node', 'query')
+         freevars   ()
+         cellvars   ()
+         filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
+         name       'spark_function_replacements'
+         firstlineno 435
+         lnotab 0x02022c012c014401
+      code
+         argcount  : 1
          nlocals   : 4
-         stacksize : 7
+         stacksize : 8
          flags     : 3
          code
             0x97007401000000000000000000006a0100000000000000007c006401ac
             02a6020000ab0200000000000000007d0174040000000000000000000074
             0600000000000000000000740800000000000000000000740a0000000000
             0000000000740c00000000000000000000740e0000000000000000000074
-            100000000000000000000066077d027c0244005d177d037c01a009000000
-            00000000000000000000000000000000007c03a6010000ab010000000000
-            0000007d018c187c015300
-         436           0 RESUME                   0
+            100000000000000000000074120000000000000000000066087d027c0244
+            005d177d037c01a00a00000000000000000000000000000000000000007c
+            03a6010000ab0100000000000000007d018c187c015300
+         443           0 RESUME                   0
          
-         440           2 LOAD_GLOBAL              1 (NULL + sqlglot)
+         447           2 LOAD_GLOBAL              1 (NULL + sqlglot)
                       14 LOAD_ATTR                1 (parse_one)
                       24 LOAD_FAST                0 (query)
                       26 LOAD_CONST               1 ('trino')
                       28 KW_NAMES                 2
                       30 PRECALL                  2
                       34 CALL                     2
                       44 STORE_FAST               1 (query_tree)
          
-         442          46 LOAD_GLOBAL              4 (interval_fix)
+         449          46 LOAD_GLOBAL              4 (interval_fix)
+         
+         450          58 LOAD_GLOBAL              6 (fix_boolean)
          
-         443          58 LOAD_GLOBAL              6 (fix_boolean)
+         451          70 LOAD_GLOBAL              8 (cast_numeric)
          
-         444          70 LOAD_GLOBAL              8 (cast_numeric)
+         452          82 LOAD_GLOBAL             10 (cast_timestamp)
          
-         445          82 LOAD_GLOBAL             10 (cast_timestamp)
+         453          94 LOAD_GLOBAL             12 (warn_unnest)
          
-         446          94 LOAD_GLOBAL             12 (warn_unnest)
+         454         106 LOAD_GLOBAL             14 (warn_sequence)
          
-         447         106 LOAD_GLOBAL             14 (warn_sequence)
+         455         118 LOAD_GLOBAL             16 (bytea2numeric)
          
-         448         118 LOAD_GLOBAL             16 (bytea2numeric)
+         456         130 LOAD_GLOBAL             18 (spark_function_replacements)
          
-         441         130 BUILD_TUPLE              7
-                     132 STORE_FAST               2 (transforms)
+         448         142 BUILD_TUPLE              8
+                     144 STORE_FAST               2 (transforms)
          
-         450         134 LOAD_FAST                2 (transforms)
-                     136 GET_ITER
-                 >>  138 FOR_ITER                23 (to 186)
-                     140 STORE_FAST               3 (f)
+         458         146 LOAD_FAST                2 (transforms)
+                     148 GET_ITER
+                 >>  150 FOR_ITER                23 (to 198)
+                     152 STORE_FAST               3 (f)
          
-         451         142 LOAD_FAST                1 (query_tree)
-                     144 LOAD_METHOD              9 (transform)
-                     166 LOAD_FAST                3 (f)
-                     168 PRECALL                  1
-                     172 CALL                     1
-                     182 STORE_FAST               1 (query_tree)
-                     184 JUMP_BACKWARD           24 (to 138)
+         459         154 LOAD_FAST                1 (query_tree)
+                     156 LOAD_METHOD             10 (transform)
+                     178 LOAD_FAST                3 (f)
+                     180 PRECALL                  1
+                     184 CALL                     1
+                     194 STORE_FAST               1 (query_tree)
+                     196 JUMP_BACKWARD           24 (to 150)
          
-         452     >>  186 LOAD_FAST                1 (query_tree)
-                     188 RETURN_VALUE
+         460     >>  198 LOAD_FAST                1 (query_tree)
+                     200 RETURN_VALUE
          consts
             "Apply a series of transforms to the query tree, recursively using SQLGlot's recursive transform function.\n\n    Each transform takes and returns a sqlglot.Expression"
             'trino'
             ('read',)
-         names      ('sqlglot', 'parse_one', 'interval_fix', 'fix_boolean', 'cast_numeric', 'cast_timestamp', 'warn_unnest', 'warn_sequence', 'bytea2numeric', 'transform')
+         names      ('sqlglot', 'parse_one', 'interval_fix', 'fix_boolean', 'cast_numeric', 'cast_timestamp', 'warn_unnest', 'warn_sequence', 'bytea2numeric', 'spark_function_replacements', 'transform')
          varnames   ('query', 'query_tree', 'transforms', 'f')
          freevars   ()
          cellvars   ()
          filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
          name       'spark_transforms'
-         firstlineno 436
-         lnotab 0x02042c020c010c010c010c010c010c010cf9040908012c01
+         firstlineno 443
+         lnotab 0x02042c020c010c010c010c010c010c010c010cf8040a08012c01
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 4
          flags     : 3
          code
             0x970064017c00a0000000000000000000000000000000000000000000a6
             000000ab0000000000000000007600720564027c007a0000007d00740300
             0000000000000000006a02000000000000000064037c00a6020000ab0200
             00000000000000720564047c007a0000007d0064057c00a0000000000000
             000000000000000000000000000000a6000000ab00000000000000000076
             00720564067c007a0000007d0064077c007a0000005300
-         455           0 RESUME                   0
+         463           0 RESUME                   0
          
-         457           2 LOAD_CONST               1 ("lower('{{")
+         465           2 LOAD_CONST               1 ("lower('{{")
                        4 LOAD_FAST                0 (query)
                        6 LOAD_METHOD              0 (lower)
                       28 PRECALL                  0
                       32 CALL                     0
                       42 CONTAINS_OP              0
                       44 POP_JUMP_FORWARD_IF_FALSE     5 (to 56)
          
-         459          46 LOAD_CONST               2 ("/* !Bytea parameter warning: Make sure to change \\x to 0x in the parameters, bytea types are native now (no need for quotes or lower or \\x)' */\n\n")
+         467          46 LOAD_CONST               2 ("/* !Bytea parameter warning: Make sure to change \\x to 0x in the parameters, bytea types are native now (no need for quotes or lower or \\x)' */\n\n")
          
-         462          48 LOAD_FAST                0 (query)
+         470          48 LOAD_FAST                0 (query)
          
-         458          50 BINARY_OP                0 (+)
+         466          50 BINARY_OP                0 (+)
                       54 STORE_FAST               0 (query)
          
-         465     >>   56 LOAD_GLOBAL              3 (NULL + re)
+         473     >>   56 LOAD_GLOBAL              3 (NULL + re)
                       68 LOAD_ATTR                2 (search)
                       78 LOAD_CONST               3 ('\\[.*\\]')
                       80 LOAD_FAST                0 (query)
                       82 PRECALL                  2
                       86 CALL                     2
                       96 POP_JUMP_FORWARD_IF_FALSE     5 (to 108)
          
-         467          98 LOAD_CONST               4 ('/* !Array warning: Arrays in dune SQL are indexed from 1, not 0. The migrator will not catch this if you indexed using variables */\n\n')
+         475          98 LOAD_CONST               4 ('/* !Array warning: Arrays in dune SQL are indexed from 1, not 0. The migrator will not catch this if you indexed using variables */\n\n')
          
-         470         100 LOAD_FAST                0 (query)
+         478         100 LOAD_FAST                0 (query)
          
-         466         102 BINARY_OP                0 (+)
+         474         102 BINARY_OP                0 (+)
                      106 STORE_FAST               0 (query)
          
-         472     >>  108 LOAD_CONST               5 ('dune_user_generated')
+         480     >>  108 LOAD_CONST               5 ('dune_user_generated')
                      110 LOAD_FAST                0 (query)
                      112 LOAD_METHOD              0 (lower)
                      134 PRECALL                  0
                      138 CALL                     0
                      148 CONTAINS_OP              0
                      150 POP_JUMP_FORWARD_IF_FALSE     5 (to 162)
          
-         474         152 LOAD_CONST               6 ("/* !Generated view warning: you can't query views in dune_user_generated anymore. All queries in DuneSQL are by default views though (try querying the table 'query_1747157') */\n\n")
+         482         152 LOAD_CONST               6 ("/* !Generated view warning: you can't query views in dune_user_generated anymore. All queries in DuneSQL are by default views though (try querying the table 'query_1747157') */\n\n")
          
-         477         154 LOAD_FAST                0 (query)
+         485         154 LOAD_FAST                0 (query)
          
-         473         156 BINARY_OP                0 (+)
+         481         156 BINARY_OP                0 (+)
                      160 STORE_FAST               0 (query)
          
-         481     >>  162 LOAD_CONST               7 ("/* Success! If you're still running into issues, check out https://dune.com/docs/query/syntax-differences/ or reach out in the #dune-sql Discord channel. */\n\n")
+         489     >>  162 LOAD_CONST               7 ("/* Success! If you're still running into issues, check out https://dune.com/docs/query/syntax-differences/ or reach out in the #dune-sql Discord channel. */\n\n")
          
-         484         164 LOAD_FAST                0 (query)
+         492         164 LOAD_FAST                0 (query)
          
-         480         166 BINARY_OP                0 (+)
+         488         166 BINARY_OP                0 (+)
                      170 RETURN_VALUE
          consts
             "Add a success banner at the top, and look for a few cases of things we don't fix and add a warning if present"
             "lower('{{"
             "/* !Bytea parameter warning: Make sure to change \\x to 0x in the parameters, bytea types are native now (no need for quotes or lower or \\x)' */\n\n"
             '\\[.*\\]'
             '/* !Array warning: Arrays in dune SQL are indexed from 1, not 0. The migrator will not catch this if you indexed using variables */\n\n'
@@ -2829,22 +2901,22 @@
             "/* Success! If you're still running into issues, check out https://dune.com/docs/query/syntax-differences/ or reach out in the #dune-sql Discord channel. */\n\n"
          names      ('lower', 're', 'search')
          varnames   ('query',)
          freevars   ()
          cellvars   ()
          filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
          name       'add_warnings_and_banner'
-         firstlineno 455
+         firstlineno 463
          lnotab
             0x02022c02020302fc06072a02020302fc06062c02020302fc0608020302
             fc
-   names      ('re', 'functools', 'partial', 'sqlglot', 'dune.harmonizer.table_replacements', 'postgres_table_replacements', 'extract_nested_select', 'recurse_where', 'chain_where_blockchain', 'chain_where_ethereum', 'chain_where_gnosis', 'chain_where_optimism', 'chain_where_bnb', 'chain_where_polygon', 'dex_trades_fixes', 'param_left_placeholder', 'param_right_placeholder', 'double_quoted_param_left_placeholder', 'double_quoted_param_right_placeholder', 'single_quoted_param_left_placeholder', 'single_quoted_param_right_placeholder', 'interval_fix', 'bytearray_parameter_fix', 'cast_numeric', 'cast_timestamp', 'fix_boolean', 'warn_unnest', 'warn_sequence', 'prep_query', 'rename_amount_column', 'bytea2numeric', 'fix_bytearray_param', 'fix_bytearray_lower', 'chain_where', 'postgres_transforms', 'remove_quotes_around_0x_strings', 'spark_transforms', 'add_warnings_and_banner')
+   names      ('re', 'functools', 'partial', 'sqlglot', 'dune.harmonizer.table_replacements', 'postgres_table_replacements', 'extract_nested_select', 'recurse_where', 'chain_where_blockchain', 'chain_where_ethereum', 'chain_where_gnosis', 'chain_where_optimism', 'chain_where_bnb', 'chain_where_polygon', 'dex_trades_fixes', 'param_left_placeholder', 'param_right_placeholder', 'double_quoted_param_left_placeholder', 'double_quoted_param_right_placeholder', 'single_quoted_param_left_placeholder', 'single_quoted_param_right_placeholder', 'interval_fix', 'bytearray_parameter_fix', 'cast_numeric', 'cast_timestamp', 'fix_boolean', 'warn_unnest', 'warn_sequence', 'prep_query', 'rename_amount_column', 'bytea2numeric', 'fix_bytearray_param', 'fix_bytearray_lower', 'chain_where', 'postgres_transforms', 'remove_quotes_around_0x_strings', 'spark_function_replacements', 'spark_transforms', 'add_warnings_and_banner')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/runner/work/harmonizer/harmonizer/dune/harmonizer/custom_transforms.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff020108010c0208020c030613065906121a011a011a011a011a0306
-      2c040104010a010a010a010a04063c061b06090612060a060e060e060c06
-      05060e06060609060a061806090613
+      2c040104010a010a010a010a04063b061b06090612060a060e060e060c06
+      05060e06060609060a0618060906080614
```

### Comparing `dune_harmonizer-0.1.0/dune/harmonizer/__pycache__/errors.cpython-311.pyc` & `dune_harmonizer-0.2.0/dune/harmonizer/__pycache__/errors.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x65233964 (Fri Apr 14 09:56:53 2023 UTC)
+moddate:  0x26523964 (Fri Apr 14 13:16:22 2023 UTC)
 files sz: 105
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `dune_harmonizer-0.1.0/dune/harmonizer/__pycache__/table_replacements.cpython-311.pyc` & `dune_harmonizer-0.2.0/dune/harmonizer/__pycache__/table_replacements.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x65233964 (Fri Apr 14 09:56:53 2023 UTC)
+moddate:  0x26523964 (Fri Apr 14 13:16:22 2023 UTC)
 files sz: 2018
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code 0x9700640064016c005a00640064016c015a01640284005a0264015300
```

### Comparing `dune_harmonizer-0.1.0/dune/harmonizer/__pycache__/translate.cpython-311.pyc` & `dune_harmonizer-0.2.0/dune/harmonizer/__pycache__/translate.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x65233964 (Fri Apr 14 09:56:53 2023 UTC)
+moddate:  0x26523964 (Fri Apr 14 13:16:22 2023 UTC)
 files sz: 3050
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
```

### Comparing `dune_harmonizer-0.1.0/dune/harmonizer/custom_transforms.py` & `dune_harmonizer-0.2.0/dune/harmonizer/custom_transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -220,15 +220,14 @@
                     return node
                 new_unit = (f"'{str(value * 7)}'" + unit.sql()).replace("weeks", "day").replace("week", "day")
                 return sqlglot.parse_one(f"interval {new_unit} --week doesn't work in DuneSQL")
             return node
 
         # The interval value is most likely a string, like `interval '1 week'`
         value, granularity, *rest = interval_argument.split()
-        1 + 1
         if any(
             known_granularity in granularity.lower()
             for known_granularity in [
                 "second",
                 "minute",
                 "hour",
                 "day",
@@ -429,27 +428,36 @@
 
     This has to happen after SQLGlot, since it will parse a bare 0x as a string literal"""
     pattern = r"'0x(.*?)'"
     substituted = re.sub(pattern, r"0x\1", query, flags=re.IGNORECASE)
     return substituted
 
 
+def spark_function_replacements(node):
+    """Replace the Spark timestamp() function with Trino's from_unixtime() function"""
+    query = node.sql(dialect="trino")
+    if "timestamp(" in query.lower():
+        query = re.sub("timestamp", "from_unixtime", query, flags=re.IGNORECASE)
+    return sqlglot.parse_one(query, read="trino")
+
+
 def spark_transforms(query):
     """Apply a series of transforms to the query tree, recursively using SQLGlot's recursive transform function.
 
     Each transform takes and returns a sqlglot.Expression"""
     query_tree = sqlglot.parse_one(query, read="trino")
     transforms = (
         interval_fix,
         fix_boolean,
         cast_numeric,
         cast_timestamp,
         warn_unnest,
         warn_sequence,
         bytea2numeric,
+        spark_function_replacements,
     )
     for f in transforms:
         query_tree = query_tree.transform(f)
     return query_tree
 
 
 def add_warnings_and_banner(query):
```

### Comparing `dune_harmonizer-0.1.0/dune/harmonizer/table_replacements.py` & `dune_harmonizer-0.2.0/dune/harmonizer/table_replacements.py`

 * *Files identical despite different names*

### Comparing `dune_harmonizer-0.1.0/dune/harmonizer/translate.py` & `dune_harmonizer-0.2.0/dune/harmonizer/translate.py`

 * *Files identical despite different names*

### Comparing `dune_harmonizer-0.1.0/pyproject.toml` & `dune_harmonizer-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dune-harmonizer"
-version = "0.1.0"
+version = "0.2.0"
 description = ""
 authors = ["Vegard Stikbakke <vegard@dune.com>"]
 readme = "README.md"
 packages = [{include = "dune"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `dune_harmonizer-0.1.0/PKG-INFO` & `dune_harmonizer-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dune-harmonizer
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 Author: Vegard Stikbakke
 Author-email: vegard@dune.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: sqlglot (>=11.4.4,<12.0.0)
```

