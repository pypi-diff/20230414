# Comparing `tmp/dune_query_translator-0.3.1.tar.gz` & `tmp/dune_query_translator-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dune_query_translator-0.3.1.tar", max compression
+gzip compressed data, was "dune_query_translator-0.4.0.tar", max compression
```

## Comparing `dune_query_translator-0.3.1.tar` & `dune_query_translator-0.4.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1061 2023-04-13 08:43:47.031824 dune_query_translator-0.3.1/LICENSE
--rw-r--r--   0        0        0     1258 2023-04-13 08:43:47.031824 dune_query_translator-0.3.1/README.md
--rw-r--r--   0        0        0      431 2023-04-13 08:43:47.031824 dune_query_translator-0.3.1/dune/translate/__init__.py
--rw-r--r--   0        0        0      861 2023-04-13 08:44:13.211611 dune_query_translator-0.3.1/dune/translate/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      651 2023-04-13 08:44:13.443610 dune_query_translator-0.3.1/dune/translate/__pycache__/errors.cpython-311.pyc
--rw-r--r--   0        0        0    20816 2023-04-13 08:44:13.447610 dune_query_translator-0.3.1/dune/translate/__pycache__/helpers.cpython-311.pyc
--rw-r--r--   0        0        0     3124 2023-04-13 08:44:13.447610 dune_query_translator-0.3.1/dune/translate/__pycache__/table_replacements.cpython-311.pyc
--rw-r--r--   0        0        0     3228 2023-04-13 08:44:13.215611 dune_query_translator-0.3.1/dune/translate/__pycache__/translate.cpython-311.pyc
--rw-r--r--   0        0        0       54 2023-04-13 08:43:47.031824 dune_query_translator-0.3.1/dune/translate/constants.py
--rw-r--r--   0        0        0      105 2023-04-13 08:43:47.031824 dune_query_translator-0.3.1/dune/translate/errors.py
--rw-r--r--   0        0        0    18400 2023-04-13 08:43:47.031824 dune_query_translator-0.3.1/dune/translate/helpers.py
--rw-r--r--   0        0        0     2018 2023-04-13 08:43:47.031824 dune_query_translator-0.3.1/dune/translate/table_replacements.py
--rw-r--r--   0        0        0     2978 2023-04-13 08:43:47.031824 dune_query_translator-0.3.1/dune/translate/translate.py
--rw-r--r--   0        0        0      576 2023-04-13 08:43:47.035824 dune_query_translator-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1600 1970-01-01 00:00:00.000000 dune_query_translator-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-04-14 07:15:42.820127 dune_query_translator-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1258 2023-04-14 07:15:42.820127 dune_query_translator-0.4.0/README.md
+-rw-r--r--   0        0        0      431 2023-04-14 07:15:42.820127 dune_query_translator-0.4.0/dune/translate/__init__.py
+-rw-r--r--   0        0        0      861 2023-04-14 07:15:58.596280 dune_query_translator-0.4.0/dune/translate/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    20968 2023-04-14 07:15:58.776283 dune_query_translator-0.4.0/dune/translate/__pycache__/custom_transforms.cpython-311.pyc
+-rw-r--r--   0        0        0      651 2023-04-14 07:15:58.776283 dune_query_translator-0.4.0/dune/translate/__pycache__/errors.cpython-311.pyc
+-rw-r--r--   0        0        0     3124 2023-04-14 07:15:58.776283 dune_query_translator-0.4.0/dune/translate/__pycache__/table_replacements.cpython-311.pyc
+-rw-r--r--   0        0        0     3224 2023-04-14 07:15:58.596280 dune_query_translator-0.4.0/dune/translate/__pycache__/translate.cpython-311.pyc
+-rw-r--r--   0        0        0       54 2023-04-14 07:15:42.820127 dune_query_translator-0.4.0/dune/translate/constants.py
+-rw-r--r--   0        0        0    18512 2023-04-14 07:15:42.820127 dune_query_translator-0.4.0/dune/translate/custom_transforms.py
+-rw-r--r--   0        0        0      105 2023-04-14 07:15:42.820127 dune_query_translator-0.4.0/dune/translate/errors.py
+-rw-r--r--   0        0        0     2018 2023-04-14 07:15:42.820127 dune_query_translator-0.4.0/dune/translate/table_replacements.py
+-rw-r--r--   0        0        0     2956 2023-04-14 07:15:42.820127 dune_query_translator-0.4.0/dune/translate/translate.py
+-rw-r--r--   0        0        0      576 2023-04-14 07:15:42.820127 dune_query_translator-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1600 1970-01-01 00:00:00.000000 dune_query_translator-0.4.0/PKG-INFO
```

### Comparing `dune_query_translator-0.3.1/LICENSE` & `dune_query_translator-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dune_query_translator-0.3.1/README.md` & `dune_query_translator-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `dune_query_translator-0.3.1/dune/translate/__pycache__/__init__.cpython-311.pyc` & `dune_query_translator-0.4.0/dune/translate/__pycache__/__init__.cpython-311.pyc`

 * *Files 14% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xc3c03764 (Thu Apr 13 08:43:47 2023 UTC)
+moddate:  0x9efd3864 (Fri Apr 14 07:15:42 2023 UTC)
 files sz: 431
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
```

### Comparing `dune_query_translator-0.3.1/dune/translate/__pycache__/errors.cpython-311.pyc` & `dune_query_translator-0.4.0/dune/translate/__pycache__/errors.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xc3c03764 (Thu Apr 13 08:43:47 2023 UTC)
+moddate:  0x9efd3864 (Fri Apr 14 07:15:42 2023 UTC)
 files sz: 105
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `dune_query_translator-0.3.1/dune/translate/__pycache__/helpers.cpython-311.pyc` & `dune_query_translator-0.4.0/dune/translate/__pycache__/custom_transforms.cpython-311.pyc`

 * *Files 3% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xc3c03764 (Thu Apr 13 08:43:47 2023 UTC)
-files sz: 18400
+moddate:  0x9efd3864 (Fri Apr 14 07:15:42 2023 UTC)
+files sz: 18512
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c005a00640064026c016d025a020100640064016c035a
@@ -41,166 +41,166 @@
      6          30 LOAD_CONST               0 (0)
                 32 LOAD_CONST               3 (('postgres_table_replacements',))
                 34 IMPORT_NAME              4 (dune.translate.table_replacements)
                 36 IMPORT_FROM              5 (postgres_table_replacements)
                 38 STORE_NAME               5 (postgres_table_replacements)
                 40 POP_TOP
    
-     9          42 LOAD_CONST               4 (<code object extract_nested_select, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py", line 9>)
+     9          42 LOAD_CONST               4 (<code object extract_nested_select, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/custom_transforms.py", line 9>)
                 44 MAKE_FUNCTION            0
                 46 STORE_NAME               6 (extract_nested_select)
    
-    27          48 LOAD_CONST               5 (<code object recurse_where, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py", line 27>)
+    28          48 LOAD_CONST               5 (<code object recurse_where, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/custom_transforms.py", line 28>)
                 50 MAKE_FUNCTION            0
                 52 STORE_NAME               7 (recurse_where)
    
-   119          54 LOAD_CONST               6 (<code object chain_where_blockchain, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py", line 119>)
+   117          54 LOAD_CONST               6 (<code object chain_where_blockchain, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/custom_transforms.py", line 117>)
                 56 MAKE_FUNCTION            0
                 58 STORE_NAME               8 (chain_where_blockchain)
    
-   137          60 PUSH_NULL
+   135          60 PUSH_NULL
                 62 LOAD_NAME                2 (partial)
                 64 LOAD_NAME                8 (chain_where_blockchain)
                 66 LOAD_CONST               7 ('ethereum')
                 68 KW_NAMES                 8
                 70 PRECALL                  2
                 74 CALL                     2
                 84 STORE_NAME               9 (chain_where_ethereum)
    
-   138          86 PUSH_NULL
+   136          86 PUSH_NULL
                 88 LOAD_NAME                2 (partial)
                 90 LOAD_NAME                8 (chain_where_blockchain)
                 92 LOAD_CONST               9 ('gnosis')
                 94 KW_NAMES                 8
                 96 PRECALL                  2
                100 CALL                     2
                110 STORE_NAME              10 (chain_where_gnosis)
    
-   139         112 PUSH_NULL
+   137         112 PUSH_NULL
                114 LOAD_NAME                2 (partial)
                116 LOAD_NAME                8 (chain_where_blockchain)
                118 LOAD_CONST              10 ('optimism')
                120 KW_NAMES                 8
                122 PRECALL                  2
                126 CALL                     2
                136 STORE_NAME              11 (chain_where_optimism)
    
-   140         138 PUSH_NULL
+   138         138 PUSH_NULL
                140 LOAD_NAME                2 (partial)
                142 LOAD_NAME                8 (chain_where_blockchain)
                144 LOAD_CONST              11 ('bnb')
                146 KW_NAMES                 8
                148 PRECALL                  2
                152 CALL                     2
                162 STORE_NAME              12 (chain_where_bnb)
    
-   141         164 PUSH_NULL
+   139         164 PUSH_NULL
                166 LOAD_NAME                2 (partial)
                168 LOAD_NAME                8 (chain_where_blockchain)
                170 LOAD_CONST              12 ('polygon')
                172 KW_NAMES                 8
                174 PRECALL                  2
                178 CALL                     2
                188 STORE_NAME              13 (chain_where_polygon)
    
-   144         190 LOAD_CONST              13 (<code object dex_trades_fixes, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py", line 144>)
+   142         190 LOAD_CONST              13 (<code object dex_trades_fixes, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/custom_transforms.py", line 142>)
                192 MAKE_FUNCTION            0
                194 STORE_NAME              14 (dex_trades_fixes)
    
-   187         196 LOAD_CONST              14 ('parameter_placeholder_left_bracket')
+   186         196 LOAD_CONST              14 ('parameter_placeholder_left_bracket')
                198 STORE_NAME              15 (param_left_placeholder)
    
-   188         200 LOAD_CONST              15 ('parameter_placeholder_right_bracket')
+   187         200 LOAD_CONST              15 ('parameter_placeholder_right_bracket')
                202 STORE_NAME              16 (param_right_placeholder)
    
-   189         204 LOAD_CONST              16 ('"')
+   188         204 LOAD_CONST              16 ('"')
                206 LOAD_NAME               15 (param_left_placeholder)
                208 FORMAT_VALUE             0
                210 BUILD_STRING             2
                212 STORE_NAME              17 (double_quoted_param_left_placeholder)
    
-   190         214 LOAD_NAME               16 (param_right_placeholder)
+   189         214 LOAD_NAME               16 (param_right_placeholder)
                216 FORMAT_VALUE             0
                218 LOAD_CONST              16 ('"')
                220 BUILD_STRING             2
                222 STORE_NAME              18 (double_quoted_param_right_placeholder)
    
-   191         224 LOAD_CONST              17 ("'")
+   190         224 LOAD_CONST              17 ("'")
                226 LOAD_NAME               15 (param_left_placeholder)
                228 FORMAT_VALUE             0
                230 BUILD_STRING             2
                232 STORE_NAME              19 (single_quoted_param_left_placeholder)
    
-   192         234 LOAD_NAME               16 (param_right_placeholder)
+   191         234 LOAD_NAME               16 (param_right_placeholder)
                236 FORMAT_VALUE             0
                238 LOAD_CONST              17 ("'")
                240 BUILD_STRING             2
                242 STORE_NAME              20 (single_quoted_param_right_placeholder)
    
-   196         244 LOAD_CONST              18 (<code object interval_fix, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py", line 196>)
+   195         244 LOAD_CONST              18 (<code object interval_fix, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/custom_transforms.py", line 195>)
                246 MAKE_FUNCTION            0
                248 STORE_NAME              21 (interval_fix)
    
-   240         250 LOAD_CONST              19 (<code object bytearray_parameter_fix, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py", line 240>)
+   241         250 LOAD_CONST              19 (<code object bytearray_parameter_fix, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/custom_transforms.py", line 241>)
                252 MAKE_FUNCTION            0
                254 STORE_NAME              22 (bytearray_parameter_fix)
    
-   267         256 LOAD_CONST              20 (<code object cast_numeric, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py", line 267>)
+   268         256 LOAD_CONST              20 (<code object cast_numeric, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/custom_transforms.py", line 268>)
                258 MAKE_FUNCTION            0
                260 STORE_NAME              23 (cast_numeric)
    
-   276         262 LOAD_CONST              21 (<code object cast_timestamp, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py", line 276>)
+   277         262 LOAD_CONST              21 (<code object cast_timestamp, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/custom_transforms.py", line 277>)
                264 MAKE_FUNCTION            0
                266 STORE_NAME              24 (cast_timestamp)
    
-   294         268 LOAD_CONST              22 (<code object fix_boolean, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py", line 294>)
+   295         268 LOAD_CONST              22 (<code object fix_boolean, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/custom_transforms.py", line 295>)
                270 MAKE_FUNCTION            0
                272 STORE_NAME              25 (fix_boolean)
    
-   304         274 LOAD_CONST              23 (<code object warn_unnest, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py", line 304>)
+   305         274 LOAD_CONST              23 (<code object warn_unnest, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/custom_transforms.py", line 305>)
                276 MAKE_FUNCTION            0
                278 STORE_NAME              26 (warn_unnest)
    
-   318         280 LOAD_CONST              24 (<code object warn_sequence, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py", line 318>)
+   319         280 LOAD_CONST              24 (<code object warn_sequence, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/custom_transforms.py", line 319>)
                282 MAKE_FUNCTION            0
                284 STORE_NAME              27 (warn_sequence)
    
-   332         286 LOAD_CONST              25 (<code object prep_query, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py", line 332>)
+   333         286 LOAD_CONST              25 (<code object prep_query, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/custom_transforms.py", line 333>)
                288 MAKE_FUNCTION            0
                290 STORE_NAME              28 (prep_query)
    
-   344         292 LOAD_CONST              26 (<code object rename_amount_column, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py", line 344>)
+   345         292 LOAD_CONST              26 (<code object rename_amount_column, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/custom_transforms.py", line 345>)
                294 MAKE_FUNCTION            0
                296 STORE_NAME              29 (rename_amount_column)
    
-   349         298 LOAD_CONST              27 (<code object bytea2numeric, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py", line 349>)
+   350         298 LOAD_CONST              27 (<code object bytea2numeric, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/custom_transforms.py", line 350>)
                300 MAKE_FUNCTION            0
                302 STORE_NAME              30 (bytea2numeric)
    
-   363         304 LOAD_CONST              28 (<code object fix_bytearray_param, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py", line 363>)
+   364         304 LOAD_CONST              28 (<code object fix_bytearray_param, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/custom_transforms.py", line 364>)
                306 MAKE_FUNCTION            0
                308 STORE_NAME              31 (fix_bytearray_param)
    
-   369         310 LOAD_CONST              29 (<code object fix_bytearray_lower, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py", line 369>)
+   370         310 LOAD_CONST              29 (<code object fix_bytearray_lower, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/custom_transforms.py", line 370>)
                312 MAKE_FUNCTION            0
                314 STORE_NAME              32 (fix_bytearray_lower)
    
-   378         316 LOAD_CONST              30 (<code object chain_where, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py", line 378>)
+   379         316 LOAD_CONST              30 (<code object chain_where, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/custom_transforms.py", line 379>)
                318 MAKE_FUNCTION            0
                320 STORE_NAME              33 (chain_where)
    
-   388         322 LOAD_CONST              31 (<code object sqlglot_postgres_transforms, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py", line 388>)
+   389         322 LOAD_CONST              31 (<code object postgres_transforms, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/custom_transforms.py", line 389>)
                324 MAKE_FUNCTION            0
-               326 STORE_NAME              34 (sqlglot_postgres_transforms)
+               326 STORE_NAME              34 (postgres_transforms)
    
-   412         328 LOAD_CONST              32 (<code object sqlglot_spark_transforms, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py", line 412>)
+   413         328 LOAD_CONST              32 (<code object spark_transforms, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/custom_transforms.py", line 413>)
                330 MAKE_FUNCTION            0
-               332 STORE_NAME              35 (sqlglot_spark_transforms)
+               332 STORE_NAME              35 (spark_transforms)
    
-   431         334 LOAD_CONST              33 (<code object add_warnings_and_banner, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py", line 431>)
+   432         334 LOAD_CONST              33 (<code object add_warnings_and_banner, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/custom_transforms.py", line 432>)
                336 MAKE_FUNCTION            0
                338 STORE_NAME              36 (add_warnings_and_banner)
                340 LOAD_CONST               1 (None)
                342 RETURN_VALUE
    consts
       0
       None
@@ -293,49 +293,49 @@
                      260 PRECALL                  0
                      264 CALL                     0
                      274 STORE_FAST               6 (substring)
          
           21         276 BUILD_LIST               0
                      278 STORE_FAST               1 (stack)
          
-          22         280 LOAD_GLOBAL             11 (NULL + re)
+          23         280 LOAD_GLOBAL             11 (NULL + re)
                      292 LOAD_ATTR                6 (search)
                      302 LOAD_CONST               5 ('^\\(\\s*select\\b')
                      304 LOAD_FAST                6 (substring)
                      306 LOAD_GLOBAL             10 (re)
                      318 LOAD_ATTR                7 (IGNORECASE)
                      328 PRECALL                  3
                      332 CALL                     3
                      342 POP_JUMP_FORWARD_IF_FALSE    21 (to 386)
          
-          23         344 LOAD_FAST                2 (results)
+          24         344 LOAD_FAST                2 (results)
                      346 LOAD_METHOD              1 (append)
                      368 LOAD_FAST                6 (substring)
                      370 PRECALL                  1
                      374 CALL                     1
                      384 POP_TOP
                  >>  386 JUMP_BACKWARD          174 (to 40)
          
-          24     >>  388 LOAD_FAST                2 (results)
+          25     >>  388 LOAD_FAST                2 (results)
                      390 RETURN_VALUE
          consts
             None
             '('
             ')'
             1
             0
             '^\\(\\s*select\\b'
          names      ('enumerate', 'append', 'len', 'pop', 'strip', 're', 'search', 'IGNORECASE')
          varnames   ('text', 'stack', 'results', 'i', 'char', 'end', 'substring')
          freevars   ()
          cellvars   ()
-         filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py'
+         filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/custom_transforms.py'
          name       'extract_nested_select'
          firstlineno 9
-         lnotab 0x02010401040128010c012c010c0126012a020a014401040140012c01
+         lnotab 0x02010401040128010c012c010c0126012a020a014401040240012c01
       code
          argcount  : 3
          nlocals   : 14
          stacksize : 8
          flags     : 3
          code
             0x97007401000000000000000000007c007402000000000000000000006a
@@ -382,347 +382,347 @@
             0000007c04a6010000ab01000000000000000064096b020000000072027c
             0353007413000000000000000000007c04a6010000ab0100000000000000
             0044005d3f5c0200007d067d07742b000000000000000000007c07640e64
             1a8502190000000000000000007c017c02a6030000ab0300000000000000
             007d0d7c03a00a00000000000000000000000000000000000000007c059b
             007c069b0064059d03641b7c0d7a000000641c7a000000a6020000ab0200
             000000000000007d038c407c035300
-          27           0 RESUME                   0
+          28           0 RESUME                   0
          
-          35           2 LOAD_GLOBAL              1 (NULL + isinstance)
+          36           2 LOAD_GLOBAL              1 (NULL + isinstance)
                       14 LOAD_FAST                0 (node)
                       16 LOAD_GLOBAL              2 (sqlglot)
                       28 LOAD_ATTR                2 (Expression)
                       38 PRECALL                  2
                       42 CALL                     2
                       52 POP_JUMP_FORWARD_IF_FALSE    23 (to 100)
          
-          36          54 LOAD_FAST                0 (node)
+          37          54 LOAD_FAST                0 (node)
                       56 LOAD_METHOD              3 (sql)
                       78 LOAD_CONST               1 ('trino')
                       80 KW_NAMES                 2
                       82 PRECALL                  1
                       86 CALL                     1
                       96 STORE_FAST               3 (statement)
                       98 JUMP_FORWARD            55 (to 210)
          
-          37     >>  100 LOAD_GLOBAL              1 (NULL + isinstance)
+          38     >>  100 LOAD_GLOBAL              1 (NULL + isinstance)
                      112 LOAD_FAST                0 (node)
                      114 LOAD_GLOBAL              8 (str)
                      126 PRECALL                  2
                      130 CALL                     2
                      140 POP_JUMP_FORWARD_IF_FALSE     3 (to 148)
          
-          38         142 LOAD_FAST                0 (node)
+          39         142 LOAD_FAST                0 (node)
                      144 STORE_FAST               3 (statement)
                      146 JUMP_FORWARD            31 (to 210)
          
-          40     >>  148 LOAD_GLOBAL             11 (NULL + ValueError)
+          41     >>  148 LOAD_GLOBAL             11 (NULL + ValueError)
                      160 LOAD_CONST               3 ('node must be a sqlglot.Expression or string, not ')
                      162 LOAD_GLOBAL             13 (NULL + type)
                      174 LOAD_FAST                0 (node)
                      176 PRECALL                  1
                      180 CALL                     1
                      190 FORMAT_VALUE             0
                      192 BUILD_STRING             2
                      194 PRECALL                  1
                      198 CALL                     1
                      208 RAISE_VARARGS            1
          
-          41     >>  210 LOAD_FAST                2 (condition_add)
+          42     >>  210 LOAD_FAST                2 (condition_add)
                      212 LOAD_METHOD              7 (strip)
                      234 PRECALL                  0
                      238 CALL                     0
                      248 STORE_FAST               2 (condition_add)
          
-          44         250 LOAD_GLOBAL             17 (NULL + extract_nested_select)
+          45         250 LOAD_GLOBAL             17 (NULL + extract_nested_select)
                      262 LOAD_FAST                3 (statement)
                      264 PRECALL                  1
                      268 CALL                     1
                      278 STORE_FAST               4 (match_groups)
          
-          46         280 LOAD_CONST               4 ('(SELECT * FROM __PLACEHOLDER')
+          47         280 LOAD_CONST               4 ('(SELECT * FROM __PLACEHOLDER')
                      282 STORE_FAST               5 (placeholder)
          
-          47         284 LOAD_GLOBAL             19 (NULL + enumerate)
+          48         284 LOAD_GLOBAL             19 (NULL + enumerate)
                      296 LOAD_FAST                4 (match_groups)
                      298 PRECALL                  1
                      302 CALL                     1
                      312 GET_ITER
                  >>  314 FOR_ITER                32 (to 380)
                      316 UNPACK_SEQUENCE          2
                      320 STORE_FAST               6 (i)
                      322 STORE_FAST               7 (group)
          
-          48         324 LOAD_FAST                3 (statement)
+          49         324 LOAD_FAST                3 (statement)
                      326 LOAD_METHOD             10 (replace)
                      348 LOAD_FAST                7 (group)
                      350 LOAD_FAST                5 (placeholder)
                      352 FORMAT_VALUE             0
                      354 LOAD_FAST                6 (i)
                      356 FORMAT_VALUE             0
                      358 LOAD_CONST               5 ('__)')
                      360 BUILD_STRING             3
                      362 PRECALL                  2
                      366 CALL                     2
                      376 STORE_FAST               3 (statement)
                      378 JUMP_BACKWARD           33 (to 314)
          
-          50     >>  380 LOAD_GLOBAL              3 (NULL + sqlglot)
+          51     >>  380 LOAD_GLOBAL              3 (NULL + sqlglot)
                      392 LOAD_ATTR               11 (parse_one)
                      402 LOAD_FAST                3 (statement)
                      404 LOAD_CONST               1 ('trino')
                      406 KW_NAMES                 6
                      408 PRECALL                  2
                      412 CALL                     2
                      422 LOAD_METHOD             12 (find_all)
                      444 LOAD_GLOBAL              2 (sqlglot)
                      456 LOAD_ATTR               13 (exp)
                      466 LOAD_ATTR               14 (Table)
                      476 PRECALL                  1
                      480 CALL                     1
                      490 STORE_FAST               8 (tables)
          
-          51         492 LOAD_FAST                8 (tables)
+          52         492 LOAD_FAST                8 (tables)
                      494 GET_ITER
                  >>  496 EXTENDED_ARG             1
                      498 FOR_ITER               360 (to 1220)
                      500 STORE_FAST               9 (table)
          
-          52         502 LOAD_FAST                1 (required_tables)
+          53         502 LOAD_FAST                1 (required_tables)
                      504 GET_ITER
                  >>  506 EXTENDED_ARG             1
                      508 FOR_ITER               353 (to 1216)
                      510 STORE_FAST              10 (req)
          
-          53         512 LOAD_FAST               10 (req)
+          54         512 LOAD_FAST               10 (req)
                      514 LOAD_GLOBAL              9 (NULL + str)
                      526 LOAD_FAST                9 (table)
                      528 PRECALL                  1
                      532 CALL                     1
                      542 LOAD_METHOD             10 (replace)
                      564 LOAD_CONST               7 ('"')
                      566 LOAD_CONST               8 ('')
                      568 PRECALL                  2
                      572 CALL                     2
                      582 CONTAINS_OP              0
                      584 EXTENDED_ARG             1
                      586 POP_JUMP_FORWARD_IF_FALSE   312 (to 1212)
          
-          54         588 LOAD_GLOBAL             31 (NULL + len)
+          55         588 LOAD_GLOBAL             31 (NULL + len)
                      600 LOAD_FAST                9 (table)
                      602 LOAD_ATTR               16 (alias)
                      612 PRECALL                  1
                      616 CALL                     1
                      626 LOAD_CONST               9 (0)
                      628 COMPARE_OP               4 (>)
                      634 POP_JUMP_FORWARD_IF_FALSE    17 (to 670)
          
-          55         636 LOAD_CONST              10 (' where ')
+          56         636 LOAD_CONST              10 (' where ')
                      638 LOAD_FAST                9 (table)
                      640 LOAD_ATTR               16 (alias)
                      650 BINARY_OP                0 (+)
                      654 LOAD_CONST              11 ('.')
                      656 BINARY_OP                0 (+)
                      660 LOAD_FAST                2 (condition_add)
                      662 BINARY_OP                0 (+)
                      666 STORE_FAST              11 (statement_to_add)
                      668 JUMP_FORWARD             5 (to 680)
          
-          57     >>  670 LOAD_CONST              10 (' where ')
+          58     >>  670 LOAD_CONST              10 (' where ')
                      672 LOAD_FAST                2 (condition_add)
                      674 BINARY_OP                0 (+)
                      678 STORE_FAST              11 (statement_to_add)
          
-          60     >>  680 LOAD_GLOBAL             35 (NULL + re)
+          61     >>  680 LOAD_GLOBAL             35 (NULL + re)
                      692 LOAD_ATTR               18 (split)
                      702 LOAD_CONST              12 ('where')
                      704 LOAD_FAST                3 (statement)
                      706 LOAD_GLOBAL             34 (re)
                      718 LOAD_ATTR               19 (IGNORECASE)
                      728 KW_NAMES                13
                      730 PRECALL                  3
                      734 CALL                     3
                      744 STORE_FAST              12 (where_statement)
          
-          62         746 LOAD_GLOBAL             31 (NULL + len)
+          63         746 LOAD_GLOBAL             31 (NULL + len)
                      758 LOAD_FAST               12 (where_statement)
                      760 PRECALL                  1
                      764 CALL                     1
                      774 LOAD_CONST              14 (1)
                      776 COMPARE_OP               4 (>)
                      782 POP_JUMP_FORWARD_IF_FALSE    38 (to 860)
          
-          63         784 LOAD_GLOBAL             35 (NULL + re)
+          64         784 LOAD_GLOBAL             35 (NULL + re)
                      796 LOAD_ATTR               20 (sub)
          
-          64         806 LOAD_CONST              12 ('where')
+          65         806 LOAD_CONST              12 ('where')
          
-          65         808 LOAD_FAST               11 (statement_to_add)
+          66         808 LOAD_FAST               11 (statement_to_add)
                      810 LOAD_CONST              15 (' and ')
                      812 BINARY_OP                0 (+)
          
-          66         816 LOAD_FAST                3 (statement)
+          67         816 LOAD_FAST                3 (statement)
          
-          67         818 LOAD_GLOBAL             34 (re)
+          68         818 LOAD_GLOBAL             34 (re)
                      830 LOAD_ATTR               19 (IGNORECASE)
          
-          63         840 KW_NAMES                13
+          64         840 KW_NAMES                13
                      842 PRECALL                  4
                      846 CALL                     4
                      856 STORE_FAST               3 (statement)
                      858 JUMP_BACKWARD          177 (to 506)
          
-          71     >>  860 LOAD_CONST              16 ('group by')
+          72     >>  860 LOAD_CONST              16 ('group by')
                      862 LOAD_FAST                3 (statement)
                      864 CONTAINS_OP              0
                      866 POP_JUMP_FORWARD_IF_FALSE    38 (to 944)
          
-          72         868 LOAD_GLOBAL             35 (NULL + re)
+          73         868 LOAD_GLOBAL             35 (NULL + re)
                      880 LOAD_ATTR               20 (sub)
          
-          73         890 LOAD_CONST              17 ('group')
+          74         890 LOAD_CONST              17 ('group')
          
-          74         892 LOAD_FAST               11 (statement_to_add)
+          75         892 LOAD_FAST               11 (statement_to_add)
                      894 LOAD_CONST              18 (' group ')
                      896 BINARY_OP                0 (+)
          
-          75         900 LOAD_FAST                3 (statement)
+          76         900 LOAD_FAST                3 (statement)
          
-          76         902 LOAD_GLOBAL             34 (re)
+          77         902 LOAD_GLOBAL             34 (re)
                      914 LOAD_ATTR               19 (IGNORECASE)
          
-          72         924 KW_NAMES                13
+          73         924 KW_NAMES                13
                      926 PRECALL                  4
                      930 CALL                     4
                      940 STORE_FAST               3 (statement)
                      942 JUMP_BACKWARD          219 (to 506)
          
-          78     >>  944 LOAD_CONST              19 ('order by')
+          79     >>  944 LOAD_CONST              19 ('order by')
                      946 LOAD_FAST                3 (statement)
                      948 CONTAINS_OP              0
                      950 POP_JUMP_FORWARD_IF_FALSE    39 (to 1030)
          
-          79         952 LOAD_GLOBAL             35 (NULL + re)
+          80         952 LOAD_GLOBAL             35 (NULL + re)
                      964 LOAD_ATTR               20 (sub)
          
-          80         974 LOAD_CONST              20 ('order')
+          81         974 LOAD_CONST              20 ('order')
          
-          81         976 LOAD_FAST               11 (statement_to_add)
+          82         976 LOAD_FAST               11 (statement_to_add)
                      978 LOAD_CONST              21 (' order ')
                      980 BINARY_OP                0 (+)
          
-          82         984 LOAD_FAST                3 (statement)
+          83         984 LOAD_FAST                3 (statement)
          
-          83         986 LOAD_GLOBAL             34 (re)
+          84         986 LOAD_GLOBAL             34 (re)
                      998 LOAD_ATTR               19 (IGNORECASE)
          
-          79        1008 KW_NAMES                13
+          80        1008 KW_NAMES                13
                     1010 PRECALL                  4
                     1014 CALL                     4
                     1024 STORE_FAST               3 (statement)
                     1026 EXTENDED_ARG             1
                     1028 JUMP_BACKWARD          262 (to 506)
          
-          85     >> 1030 LOAD_CONST              22 ('limit')
+          86     >> 1030 LOAD_CONST              22 ('limit')
                     1032 LOAD_FAST                3 (statement)
                     1034 CONTAINS_OP              0
                     1036 POP_JUMP_FORWARD_IF_FALSE    39 (to 1116)
          
-          86        1038 LOAD_GLOBAL             35 (NULL + re)
+          87        1038 LOAD_GLOBAL             35 (NULL + re)
                     1050 LOAD_ATTR               20 (sub)
          
-          87        1060 LOAD_CONST              22 ('limit')
+          88        1060 LOAD_CONST              22 ('limit')
          
-          88        1062 LOAD_FAST               11 (statement_to_add)
+          89        1062 LOAD_FAST               11 (statement_to_add)
                     1064 LOAD_CONST              23 (' limit ')
                     1066 BINARY_OP                0 (+)
          
-          89        1070 LOAD_FAST                3 (statement)
+          90        1070 LOAD_FAST                3 (statement)
          
-          90        1072 LOAD_GLOBAL             34 (re)
+          91        1072 LOAD_GLOBAL             34 (re)
                     1084 LOAD_ATTR               19 (IGNORECASE)
          
-          86        1094 KW_NAMES                13
+          87        1094 KW_NAMES                13
                     1096 PRECALL                  4
                     1100 CALL                     4
                     1110 STORE_FAST               3 (statement)
                     1112 EXTENDED_ARG             1
                     1114 JUMP_BACKWARD          305 (to 506)
          
-          92     >> 1116 LOAD_CONST              24 ('offset')
+          93     >> 1116 LOAD_CONST              24 ('offset')
                     1118 LOAD_FAST                3 (statement)
                     1120 CONTAINS_OP              0
                     1122 POP_JUMP_FORWARD_IF_FALSE    39 (to 1202)
          
-          93        1124 LOAD_GLOBAL             35 (NULL + re)
+          94        1124 LOAD_GLOBAL             35 (NULL + re)
                     1136 LOAD_ATTR               20 (sub)
          
-          94        1146 LOAD_CONST              24 ('offset')
+          95        1146 LOAD_CONST              24 ('offset')
          
-          95        1148 LOAD_FAST               11 (statement_to_add)
+          96        1148 LOAD_FAST               11 (statement_to_add)
                     1150 LOAD_CONST              25 (' offset ')
                     1152 BINARY_OP                0 (+)
          
-          96        1156 LOAD_FAST                3 (statement)
+          97        1156 LOAD_FAST                3 (statement)
          
-          97        1158 LOAD_GLOBAL             34 (re)
+          98        1158 LOAD_GLOBAL             34 (re)
                     1170 LOAD_ATTR               19 (IGNORECASE)
          
-          93        1180 KW_NAMES                13
+          94        1180 KW_NAMES                13
                     1182 PRECALL                  4
                     1186 CALL                     4
                     1196 STORE_FAST               3 (statement)
                     1198 EXTENDED_ARG             1
                     1200 JUMP_BACKWARD          348 (to 506)
          
-         101     >> 1202 LOAD_FAST                3 (statement)
+         102     >> 1202 LOAD_FAST                3 (statement)
                     1204 LOAD_FAST               11 (statement_to_add)
                     1206 BINARY_OP                0 (+)
                     1210 STORE_FAST               3 (statement)
                  >> 1212 EXTENDED_ARG             1
                     1214 JUMP_BACKWARD          355 (to 506)
          
-          52     >> 1216 EXTENDED_ARG             1
+          53     >> 1216 EXTENDED_ARG             1
                     1218 JUMP_BACKWARD          362 (to 496)
          
-         104     >> 1220 LOAD_GLOBAL             31 (NULL + len)
+         105     >> 1220 LOAD_GLOBAL             31 (NULL + len)
                     1232 LOAD_FAST                4 (match_groups)
                     1234 PRECALL                  1
                     1238 CALL                     1
                     1248 LOAD_CONST               9 (0)
                     1250 COMPARE_OP               2 (==)
                     1256 POP_JUMP_FORWARD_IF_FALSE     2 (to 1262)
          
-         105        1258 LOAD_FAST                3 (statement)
+         106        1258 LOAD_FAST                3 (statement)
                     1260 RETURN_VALUE
          
-         108     >> 1262 LOAD_GLOBAL             19 (NULL + enumerate)
+         109     >> 1262 LOAD_GLOBAL             19 (NULL + enumerate)
                     1274 LOAD_FAST                4 (match_groups)
                     1276 PRECALL                  1
                     1280 CALL                     1
                     1290 GET_ITER
                  >> 1292 FOR_ITER                63 (to 1420)
                     1294 UNPACK_SEQUENCE          2
                     1298 STORE_FAST               6 (i)
                     1300 STORE_FAST               7 (group)
          
-         110        1302 LOAD_GLOBAL             43 (NULL + recurse_where)
+         111        1302 LOAD_GLOBAL             43 (NULL + recurse_where)
                     1314 LOAD_FAST                7 (group)
                     1316 LOAD_CONST              14 (1)
                     1318 LOAD_CONST              26 (-1)
                     1320 BUILD_SLICE              2
                     1322 BINARY_SUBSCR
                     1332 LOAD_FAST                1 (required_tables)
                     1334 LOAD_FAST                2 (condition_add)
                     1336 PRECALL                  3
                     1340 CALL                     3
                     1350 STORE_FAST              13 (parsed_group)
          
-         111        1352 LOAD_FAST                3 (statement)
+         112        1352 LOAD_FAST                3 (statement)
                     1354 LOAD_METHOD             10 (replace)
                     1376 LOAD_FAST                5 (placeholder)
                     1378 FORMAT_VALUE             0
                     1380 LOAD_FAST                6 (i)
                     1382 FORMAT_VALUE             0
                     1384 LOAD_CONST               5 ('__)')
                     1386 BUILD_STRING             3
@@ -732,15 +732,15 @@
                     1396 LOAD_CONST              28 (')')
                     1398 BINARY_OP                0 (+)
                     1402 PRECALL                  2
                     1406 CALL                     2
                     1416 STORE_FAST               3 (statement)
                     1418 JUMP_BACKWARD           64 (to 1292)
          
-         113     >> 1420 LOAD_FAST                3 (statement)
+         114     >> 1420 LOAD_FAST                3 (statement)
                     1422 RETURN_VALUE
          consts
             '\n    we can\'t just iterate through the tree because of weird replace node behaviors, so this iterates\n    through SELECT statements and specifically adds WHERE statements with a specific condition_add\n    for a given set of required_tables, then goes through each removed select recursively to do the same thing\n\n    Useful for adding aliased "blockchain = \'ethereum\'"  or other where statements in the right places.\n    '
             'trino'
             ('dialect',)
             'node must be a sqlglot.Expression or string, not '
             '(SELECT * FROM __PLACEHOLDER'
@@ -768,17 +768,17 @@
             -1
             '('
             ')'
          names      ('isinstance', 'sqlglot', 'Expression', 'sql', 'str', 'ValueError', 'type', 'strip', 'extract_nested_select', 'enumerate', 'replace', 'parse_one', 'find_all', 'exp', 'Table', 'len', 'alias', 're', 'split', 'IGNORECASE', 'sub', 'recurse_where')
          varnames   ('node', 'required_tables', 'condition_add', 'statement', 'match_groups', 'placeholder', 'i', 'group', 'tables', 'table', 'req', 'statement_to_add', 'where_statement', 'parsed_group')
          freevars   ()
          cellvars   ()
-         filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py'
+         filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/custom_transforms.py'
          name       'recurse_where'
-         firstlineno 27
+         firstlineno 28
          lnotab
             0x020834012e012a0106023e0128031e0204012801380270010a010a014c
             01300122020a0342022601160102010801020116fc140808011601020108
             01020116fc14060801160102010801020116fc1606080116010201080102
             0116fc16060801160102010801020116fc16080ecf043426010403280232
             014402
       code
@@ -788,71 +788,71 @@
          flags     : 3
          code
             0x970067006401a2017d0264027c019b0064039d037d037c006a00000000
             000000000064046b0200000000722e7c006a010000000000000000802774
             05000000000000000000007c007c027c03a6030000ab0300000000000000
             007d047407000000000000000000006a0400000000000000007c046405ac
             06a6020000ab02000000000000000053007c005300
-         119           0 RESUME                   0
+         117           0 RESUME                   0
          
-         121           2 BUILD_LIST               0
+         119           2 BUILD_LIST               0
                        4 LOAD_CONST               1 (('nft.trades', 'dex.in.trades', 'tokens.erc20', 'tokens.nft', 'prices.usd'))
                        6 LIST_EXTEND              1
                        8 STORE_FAST               2 (required_tables)
          
-         128          10 LOAD_CONST               2 ("blockchain = '")
+         126          10 LOAD_CONST               2 ("blockchain = '")
                       12 LOAD_FAST                1 (blockchain)
                       14 FORMAT_VALUE             0
                       16 LOAD_CONST               3 ("'")
                       18 BUILD_STRING             3
                       20 STORE_FAST               3 (condition_add)
          
-         131          22 LOAD_FAST                0 (node)
+         129          22 LOAD_FAST                0 (node)
                       24 LOAD_ATTR                0 (key)
                       34 LOAD_CONST               4 ('select')
                       36 COMPARE_OP               2 (==)
                       42 POP_JUMP_FORWARD_IF_FALSE    46 (to 136)
                       44 LOAD_FAST                0 (node)
                       46 LOAD_ATTR                1 (parent)
                       56 POP_JUMP_FORWARD_IF_NOT_NONE    39 (to 136)
          
-         132          58 LOAD_GLOBAL              5 (NULL + recurse_where)
+         130          58 LOAD_GLOBAL              5 (NULL + recurse_where)
                       70 LOAD_FAST                0 (node)
                       72 LOAD_FAST                2 (required_tables)
                       74 LOAD_FAST                3 (condition_add)
                       76 PRECALL                  3
                       80 CALL                     3
                       90 STORE_FAST               4 (statement)
          
-         133          92 LOAD_GLOBAL              7 (NULL + sqlglot)
+         131          92 LOAD_GLOBAL              7 (NULL + sqlglot)
                      104 LOAD_ATTR                4 (parse_one)
                      114 LOAD_FAST                4 (statement)
                      116 LOAD_CONST               5 ('trino')
                      118 KW_NAMES                 6
                      120 PRECALL                  2
                      124 CALL                     2
                      134 RETURN_VALUE
          
-         134     >>  136 LOAD_FAST                0 (node)
+         132     >>  136 LOAD_FAST                0 (node)
                      138 RETURN_VALUE
          consts
             None
             ('nft.trades', 'dex.in.trades', 'tokens.erc20', 'tokens.nft', 'prices.usd')
             "blockchain = '"
             "'"
             'select'
             'trino'
             ('read',)
          names      ('key', 'parent', 'recurse_where', 'sqlglot', 'parse_one')
          varnames   ('node', 'blockchain', 'required_tables', 'condition_add', 'statement')
          freevars   ()
          cellvars   ()
-         filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py'
+         filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/custom_transforms.py'
          name       'chain_where_blockchain'
-         firstlineno 119
+         firstlineno 117
          lnotab 0x020208070c03240122012c01
       'ethereum'
       ('blockchain',)
       'gnosis'
       'optimism'
       'bnb'
       'polygon'
@@ -875,128 +875,128 @@
             0000000000ac0aa6040000ab0400000000000000007d018c3a7407000000
             000000000000006a050000000000000000640b640c7c0174060000000000
             00000000006a060000000000000000ac0aa6040000ab0400000000000000
             007d017407000000000000000000006a050000000000000000640d640e7c
             017406000000000000000000006a060000000000000000ac0aa6040000ab
             0400000000000000007d01740f000000000000000000006a080000000000
             0000007c016403ac0fa6020000ab02000000000000000053007c005300
-         144           0 RESUME                   0
+         142           0 RESUME                   0
          
-         146           2 LOAD_FAST                0 (node)
+         145           2 LOAD_FAST                0 (node)
                        4 LOAD_ATTR                0 (key)
                       14 LOAD_CONST               1 ('select')
                       16 COMPARE_OP               2 (==)
                       22 POP_JUMP_FORWARD_IF_FALSE   240 (to 504)
          
-         147          24 LOAD_CONST               2 ('dex.in.trades')
+         146          24 LOAD_CONST               2 ('dex.in.trades')
                       26 LOAD_FAST                0 (node)
                       28 LOAD_METHOD              1 (sql)
                       50 LOAD_CONST               3 ('trino')
                       52 KW_NAMES                 4
                       54 PRECALL                  1
                       58 CALL                     1
                       68 LOAD_METHOD              2 (replace)
                       90 LOAD_CONST               5 ('"')
                       92 LOAD_CONST               6 ('')
                       94 PRECALL                  2
                       98 CALL                     2
                      108 CONTAINS_OP              0
                      110 POP_JUMP_FORWARD_IF_FALSE   196 (to 504)
          
-         149         112 LOAD_FAST                0 (node)
+         148         112 LOAD_FAST                0 (node)
                      114 LOAD_METHOD              1 (sql)
                      136 LOAD_CONST               3 ('trino')
                      138 KW_NAMES                 4
                      140 PRECALL                  1
                      144 CALL                     1
                      154 LOAD_METHOD              2 (replace)
                      176 LOAD_CONST               7 ('exchange_contract_address')
                      178 LOAD_CONST               8 ('project_contract_address')
                      180 PRECALL                  2
                      184 CALL                     2
                      194 STORE_FAST               1 (final_where)
          
-         152         196 BUILD_LIST               0
+         151         196 BUILD_LIST               0
                      198 LOAD_CONST               9 (('(?i)\\w+\\.[\\\'"]?category[\\\'"]?\\s*=\\s*[\\\'"]dex.in[\\\'"]\\s*and', '(?i)and\\s*\\w+\\.[\\\'"]?category[\\\'"]?\\s*=\\s*[\\\'"]dex.in[\\\'"]', '(?i)where\\s*\\w+\\.[\\\'"]?category[\\\'"]?\\s*=\\s*[\\\'"]dex.in[\\\'"]', '(?i)[\\\'"]?category[\\\'"]?\\s*=\\s*[\\\'"]dex.in[\\\'"]\\s*and', '(?i)and\\s*[\\\'"]?category[\\\'"]?\\s*=\\s*[\\\'"]dex.in[\\\'"]', '(?i)where\\s*[\\\'"]?category[\\\'"]?\\s*=\\s*[\\\'"]dex.in[\\\'"]'))
                      200 LIST_EXTEND              1
                      202 STORE_FAST               2 (clean_matches)
          
-         164         204 LOAD_FAST                2 (clean_matches)
+         163         204 LOAD_FAST                2 (clean_matches)
                      206 GET_ITER
                  >>  208 FOR_ITER                57 (to 324)
                      210 STORE_FAST               3 (match)
          
-         165         212 LOAD_GLOBAL              7 (NULL + re)
+         164         212 LOAD_GLOBAL              7 (NULL + re)
                      224 LOAD_ATTR                4 (search)
                      234 LOAD_FAST                3 (match)
                      236 LOAD_FAST                1 (final_where)
                      238 PRECALL                  2
                      242 CALL                     2
                      252 POP_JUMP_FORWARD_IF_FALSE    34 (to 322)
          
-         167         254 LOAD_GLOBAL              7 (NULL + re)
+         166         254 LOAD_GLOBAL              7 (NULL + re)
                      266 LOAD_ATTR                5 (sub)
                      276 LOAD_FAST                3 (match)
                      278 LOAD_CONST               6 ('')
                      280 LOAD_FAST                1 (final_where)
                      282 LOAD_GLOBAL              6 (re)
                      294 LOAD_ATTR                6 (IGNORECASE)
                      304 KW_NAMES                10
                      306 PRECALL                  4
                      310 CALL                     4
                      320 STORE_FAST               1 (final_where)
                  >>  322 JUMP_BACKWARD           58 (to 208)
          
-         170     >>  324 LOAD_GLOBAL              7 (NULL + re)
+         169     >>  324 LOAD_GLOBAL              7 (NULL + re)
                      336 LOAD_ATTR                5 (sub)
          
-         171         346 LOAD_CONST              11 ('token_a_address')
+         170         346 LOAD_CONST              11 ('token_a_address')
          
-         172         348 LOAD_CONST              12 ('token_sold_address')
+         171         348 LOAD_CONST              12 ('token_sold_address')
          
-         173         350 LOAD_FAST                1 (final_where)
+         172         350 LOAD_FAST                1 (final_where)
          
-         174         352 LOAD_GLOBAL              6 (re)
+         173         352 LOAD_GLOBAL              6 (re)
                      364 LOAD_ATTR                6 (IGNORECASE)
          
-         170         374 KW_NAMES                10
+         169         374 KW_NAMES                10
                      376 PRECALL                  4
                      380 CALL                     4
                      390 STORE_FAST               1 (final_where)
          
-         176         392 LOAD_GLOBAL              7 (NULL + re)
+         175         392 LOAD_GLOBAL              7 (NULL + re)
                      404 LOAD_ATTR                5 (sub)
          
-         177         414 LOAD_CONST              13 ('token_b_address')
+         176         414 LOAD_CONST              13 ('token_b_address')
          
-         178         416 LOAD_CONST              14 ('token_bought_address')
+         177         416 LOAD_CONST              14 ('token_bought_address')
          
-         179         418 LOAD_FAST                1 (final_where)
+         178         418 LOAD_FAST                1 (final_where)
          
-         180         420 LOAD_GLOBAL              6 (re)
+         179         420 LOAD_GLOBAL              6 (re)
                      432 LOAD_ATTR                6 (IGNORECASE)
          
-         176         442 KW_NAMES                10
+         175         442 KW_NAMES                10
                      444 PRECALL                  4
                      448 CALL                     4
                      458 STORE_FAST               1 (final_where)
          
-         183         460 LOAD_GLOBAL             15 (NULL + sqlglot)
+         182         460 LOAD_GLOBAL             15 (NULL + sqlglot)
                      472 LOAD_ATTR                8 (parse_one)
                      482 LOAD_FAST                1 (final_where)
                      484 LOAD_CONST               3 ('trino')
                      486 KW_NAMES                15
                      488 PRECALL                  2
                      492 CALL                     2
                      502 RETURN_VALUE
          
-         184     >>  504 LOAD_FAST                0 (node)
+         183     >>  504 LOAD_FAST                0 (node)
                      506 RETURN_VALUE
          consts
-            None
+            'Fixes to dex.trades'
             'select'
             'dex.in.trades'
             'trino'
             ('dialect',)
             '"'
             ''
             'exchange_contract_address'
@@ -1008,236 +1008,253 @@
             'token_b_address'
             'token_bought_address'
             ('read',)
          names      ('key', 'sql', 'replace', 're', 'search', 'sub', 'IGNORECASE', 'sqlglot', 'parse_one')
          varnames   ('node', 'final_where', 'clean_matches', 'match')
          freevars   ()
          cellvars   ()
-         filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py'
+         filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/custom_transforms.py'
          name       'dex_trades_fixes'
-         firstlineno 144
+         firstlineno 142
          lnotab
-            0x0202160158025403080c08012a024603160102010201020116fc120616
+            0x0203160158025403080c08012a024603160102010201020116fc120616
             0102010201020116fc12072c01
       'parameter_placeholder_left_bracket'
       'parameter_placeholder_right_bracket'
       '"'
       "'"
       code
          argcount  : 1
-         nlocals   : 8
+         nlocals   : 7
          stacksize : 4
          flags     : 3
          code
-            0x870897007c006a00000000000000000064016b02000000009001728074
+            0x870797007c006a00000000000000000064016b0200000000900172b074
             03000000000000000000007c006a020000000000000000a6010000ab0100
             000000000000007d017c0164021900000000000000000064036b02000000
             0072167c0164041900000000000000000064056b0200000000720a7c0164
             0664048502190000000000000000007d017407000000000000000000006a
             04000000000000000064077c01a6020000ab0200000000000000007d0264
             0884007c02640664098502190000000000000000004400a6000000ab0000
             000000000000007d03740b000000000000000000007c03a6010000ab0100
             0000000000000064026b020000000072027c005300640aa0060000000000
             0000000000000000000000000000007c03a6010000ab0100000000000000
-            007d047c04a0040000000000000000000000000000000000000000a60000
-            00ab0000000000000000005e027d058a087d06740f000000000000000000
-            0088086601640b8408640c4400a6000000ab000000000000000000a60100
-            00ab01000000000000000072c58908640419000000000000000000640d6b
-            0200000000720a8908640964048502190000000000000000008a08890864
-            0e6b020000000072297411000000000000000000007c05a6010000ab0100
-            00000000000000640f7a0500007d0564108a087c06a00900000000000000
-            000000000000000000000000006411a6010000ab01000000000000000001
-            0064127403000000000000000000007c05a6010000ab0100000000000000
-            007a00000064137a00000089087a000000640aa006000000000000000000
-            00000000000000000000007c06a6010000ab0100000000000000007a0000
-            00a00a000000000000000000000000000000000000000074160000000000
-            0000000000741800000000000000000000a6020000ab0200000000000000
-            00a00a0000000000000000000000000000000000000000741a0000000000
-            0000000000741c00000000000000000000a6020000ab0200000000000000
-            007d07741f000000000000000000006a1000000000000000007c076414ac
-            15a6020000ab02000000000000000053007c005300
-                       0 MAKE_CELL                8 (granularity)
+            007d01740b000000000000000000007c01a0040000000000000000000000
+            000000000000000000a6000000ab000000000000000000a6010000ab0100
+            0000000000000064066b020000000072027c0053007c01a0040000000000
+            000000000000000000000000000000a6000000ab0000000000000000005e
+            027d048a077d05740f0000000000000000000088076601640b8408640c44
+            00a6000000ab000000000000000000a6010000ab01000000000000000072
+            ce8907a0080000000000000000000000000000000000000000640da60100
+            00ab010000000000000000720a8907640964048502190000000000000000
+            008a078907640e6b020000000072297413000000000000000000007c04a6
+            010000ab010000000000000000640f7a0500007d0464108a077c05a00a00
+            000000000000000000000000000000000000006411a6010000ab01000000
+            0000000000010064127403000000000000000000007c04a6010000ab0100
+            000000000000007a00000064137a00000089077a000000640aa006000000
+            00000000000000000000000000000000007c05a6010000ab010000000000
+            0000007a000000a00b000000000000000000000000000000000000000074
+            1800000000000000000000741a00000000000000000000a6020000ab0200
+            00000000000000a00b000000000000000000000000000000000000000074
+            1c00000000000000000000741e00000000000000000000a6020000ab0200
+            000000000000007d067421000000000000000000006a1100000000000000
+            007c066414ac15a6020000ab02000000000000000053007c005300
+                       0 MAKE_CELL                7 (granularity)
          
-         196           2 RESUME                   0
+         195           2 RESUME                   0
          
-         198           4 LOAD_FAST                0 (node)
+         197           4 LOAD_FAST                0 (node)
                        6 LOAD_ATTR                0 (key)
                       16 LOAD_CONST               1 ('interval')
                       18 COMPARE_OP               2 (==)
                       24 EXTENDED_ARG             1
-                      26 POP_JUMP_FORWARD_IF_FALSE   384 (to 796)
+                      26 POP_JUMP_FORWARD_IF_FALSE   432 (to 892)
          
-         200          28 LOAD_GLOBAL              3 (NULL + str)
+         199          28 LOAD_GLOBAL              3 (NULL + str)
                       40 LOAD_FAST                0 (node)
                       42 LOAD_ATTR                2 (this)
                       52 PRECALL                  1
                       56 CALL                     1
                       66 STORE_FAST               1 (interval_argument)
          
-         201          68 LOAD_FAST                1 (interval_argument)
+         200          68 LOAD_FAST                1 (interval_argument)
                       70 LOAD_CONST               2 (0)
                       72 BINARY_SUBSCR
                       82 LOAD_CONST               3 ('(')
                       84 COMPARE_OP               2 (==)
                       90 POP_JUMP_FORWARD_IF_FALSE    22 (to 136)
                       92 LOAD_FAST                1 (interval_argument)
                       94 LOAD_CONST               4 (-1)
                       96 BINARY_SUBSCR
                      106 LOAD_CONST               5 (')')
                      108 COMPARE_OP               2 (==)
                      114 POP_JUMP_FORWARD_IF_FALSE    10 (to 136)
          
-         202         116 LOAD_FAST                1 (interval_argument)
+         201         116 LOAD_FAST                1 (interval_argument)
                      118 LOAD_CONST               6 (1)
                      120 LOAD_CONST               4 (-1)
                      122 BUILD_SLICE              2
                      124 BINARY_SUBSCR
                      134 STORE_FAST               1 (interval_argument)
          
-         204     >>  136 LOAD_GLOBAL              7 (NULL + re)
+         203     >>  136 LOAD_GLOBAL              7 (NULL + re)
                      148 LOAD_ATTR                4 (split)
                      158 LOAD_CONST               7 ('[\\\'"]')
                      160 LOAD_FAST                1 (interval_argument)
                      162 PRECALL                  2
                      166 CALL                     2
                      176 STORE_FAST               2 (regex_split)
          
-         207         178 LOAD_CONST               8 (<code object <listcomp>, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py", line 207>)
+         206         178 LOAD_CONST               8 (<code object <listcomp>, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/custom_transforms.py", line 206>)
                      180 MAKE_FUNCTION            0
                      182 LOAD_FAST                2 (regex_split)
                      184 LOAD_CONST               6 (1)
                      186 LOAD_CONST               9 (None)
                      188 BUILD_SLICE              2
                      190 BINARY_SUBSCR
                      200 GET_ITER
                      202 PRECALL                  0
                      206 CALL                     0
                      216 STORE_FAST               3 (regex_matches)
          
-         209         218 LOAD_GLOBAL             11 (NULL + len)
+         208         218 LOAD_GLOBAL             11 (NULL + len)
                      230 LOAD_FAST                3 (regex_matches)
                      232 PRECALL                  1
                      236 CALL                     1
                      246 LOAD_CONST               2 (0)
                      248 COMPARE_OP               2 (==)
                      254 POP_JUMP_FORWARD_IF_FALSE     2 (to 260)
          
-         210         256 LOAD_FAST                0 (node)
+         209         256 LOAD_FAST                0 (node)
                      258 RETURN_VALUE
          
-         211     >>  260 LOAD_CONST              10 (' ')
+         210     >>  260 LOAD_CONST              10 (' ')
                      262 LOAD_METHOD              6 (join)
                      284 LOAD_FAST                3 (regex_matches)
                      286 PRECALL                  1
                      290 CALL                     1
-                     300 STORE_FAST               4 (identifier)
+                     300 STORE_FAST               1 (interval_argument)
          
-         212         302 LOAD_FAST                4 (identifier)
-                     304 LOAD_METHOD              4 (split)
-                     326 PRECALL                  0
-                     330 CALL                     0
-                     340 UNPACK_EX                2
-                     342 STORE_FAST               5 (value)
-                     344 STORE_DEREF              8 (granularity)
-                     346 STORE_FAST               6 (rest)
-         
-         213         348 LOAD_GLOBAL             15 (NULL + any)
-                     360 LOAD_CLOSURE             8 (granularity)
-                     362 BUILD_TUPLE              1
-                     364 LOAD_CONST              11 (<code object <genexpr>, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py", line 213>)
-                     366 MAKE_FUNCTION            8 (closure)
-         
-         215         368 LOAD_CONST              12 (('second', 'minute', 'hour', 'day', 'week', 'month', 'year'))
-         
-         213         370 GET_ITER
-                     372 PRECALL                  0
-                     376 CALL                     0
-                     386 PRECALL                  1
-                     390 CALL                     1
-                     400 POP_JUMP_FORWARD_IF_FALSE   197 (to 796)
-         
-         225         402 LOAD_DEREF               8 (granularity)
-                     404 LOAD_CONST               4 (-1)
-                     406 BINARY_SUBSCR
-                     416 LOAD_CONST              13 ('s')
-                     418 COMPARE_OP               2 (==)
-                     424 POP_JUMP_FORWARD_IF_FALSE    10 (to 446)
-         
-         226         426 LOAD_DEREF               8 (granularity)
-                     428 LOAD_CONST               9 (None)
-                     430 LOAD_CONST               4 (-1)
-                     432 BUILD_SLICE              2
-                     434 BINARY_SUBSCR
-                     444 STORE_DEREF              8 (granularity)
-         
-         227     >>  446 LOAD_DEREF               8 (granularity)
-                     448 LOAD_CONST              14 ('week')
-                     450 COMPARE_OP               2 (==)
-                     456 POP_JUMP_FORWARD_IF_FALSE    41 (to 540)
-         
-         228         458 LOAD_GLOBAL             17 (NULL + int)
-                     470 LOAD_FAST                5 (value)
-                     472 PRECALL                  1
-                     476 CALL                     1
-                     486 LOAD_CONST              15 (7)
-                     488 BINARY_OP                5 (*)
-                     492 STORE_FAST               5 (value)
-         
-         229         494 LOAD_CONST              16 ('day')
-                     496 STORE_DEREF              8 (granularity)
-         
-         230         498 LOAD_FAST                6 (rest)
-                     500 LOAD_METHOD              9 (append)
-                     522 LOAD_CONST              17 ("--week doesn't work in DuneSQL\n")
-                     524 PRECALL                  1
-                     528 CALL                     1
-                     538 POP_TOP
-         
-         232     >>  540 LOAD_CONST              18 ("INTERVAL '")
-                     542 LOAD_GLOBAL              3 (NULL + str)
-                     554 LOAD_FAST                5 (value)
-                     556 PRECALL                  1
-                     560 CALL                     1
-                     570 BINARY_OP                0 (+)
-                     574 LOAD_CONST              19 ("' ")
-                     576 BINARY_OP                0 (+)
-                     580 LOAD_DEREF               8 (granularity)
-                     582 BINARY_OP                0 (+)
-                     586 LOAD_CONST              10 (' ')
-                     588 LOAD_METHOD              6 (join)
-                     610 LOAD_FAST                6 (rest)
-                     612 PRECALL                  1
-                     616 CALL                     1
-                     626 BINARY_OP                0 (+)
+         211         302 LOAD_GLOBAL             11 (NULL + len)
+                     314 LOAD_FAST                1 (interval_argument)
+                     316 LOAD_METHOD              4 (split)
+                     338 PRECALL                  0
+                     342 CALL                     0
+                     352 PRECALL                  1
+                     356 CALL                     1
+                     366 LOAD_CONST               6 (1)
+                     368 COMPARE_OP               2 (==)
+                     374 POP_JUMP_FORWARD_IF_FALSE     2 (to 380)
+         
+         212         376 LOAD_FAST                0 (node)
+                     378 RETURN_VALUE
+         
+         213     >>  380 LOAD_FAST                1 (interval_argument)
+                     382 LOAD_METHOD              4 (split)
+                     404 PRECALL                  0
+                     408 CALL                     0
+                     418 UNPACK_EX                2
+                     420 STORE_FAST               4 (value)
+                     422 STORE_DEREF              7 (granularity)
+                     424 STORE_FAST               5 (rest)
+         
+         214         426 LOAD_GLOBAL             15 (NULL + any)
+                     438 LOAD_CLOSURE             7 (granularity)
+                     440 BUILD_TUPLE              1
+                     442 LOAD_CONST              11 (<code object <genexpr>, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/custom_transforms.py", line 214>)
+                     444 MAKE_FUNCTION            8 (closure)
+         
+         216         446 LOAD_CONST              12 (('second', 'minute', 'hour', 'day', 'week', 'month', 'year'))
+         
+         214         448 GET_ITER
+                     450 PRECALL                  0
+                     454 CALL                     0
+                     464 PRECALL                  1
+                     468 CALL                     1
+                     478 POP_JUMP_FORWARD_IF_FALSE   206 (to 892)
+         
+         226         480 LOAD_DEREF               7 (granularity)
+                     482 LOAD_METHOD              8 (endswith)
+                     504 LOAD_CONST              13 ('s')
+                     506 PRECALL                  1
+                     510 CALL                     1
+                     520 POP_JUMP_FORWARD_IF_FALSE    10 (to 542)
+         
+         227         522 LOAD_DEREF               7 (granularity)
+                     524 LOAD_CONST               9 (None)
+                     526 LOAD_CONST               4 (-1)
+                     528 BUILD_SLICE              2
+                     530 BINARY_SUBSCR
+                     540 STORE_DEREF              7 (granularity)
+         
+         228     >>  542 LOAD_DEREF               7 (granularity)
+                     544 LOAD_CONST              14 ('week')
+                     546 COMPARE_OP               2 (==)
+                     552 POP_JUMP_FORWARD_IF_FALSE    41 (to 636)
+         
+         229         554 LOAD_GLOBAL             19 (NULL + int)
+                     566 LOAD_FAST                4 (value)
+                     568 PRECALL                  1
+                     572 CALL                     1
+                     582 LOAD_CONST              15 (7)
+                     584 BINARY_OP                5 (*)
+                     588 STORE_FAST               4 (value)
+         
+         230         590 LOAD_CONST              16 ('day')
+                     592 STORE_DEREF              7 (granularity)
+         
+         231         594 LOAD_FAST                5 (rest)
+                     596 LOAD_METHOD             10 (append)
+                     618 LOAD_CONST              17 ("--week doesn't work in DuneSQL\n")
+                     620 PRECALL                  1
+                     624 CALL                     1
+                     634 POP_TOP
+         
+         233     >>  636 LOAD_CONST              18 ("INTERVAL '")
+                     638 LOAD_GLOBAL              3 (NULL + str)
+                     650 LOAD_FAST                4 (value)
+                     652 PRECALL                  1
+                     656 CALL                     1
+                     666 BINARY_OP                0 (+)
+                     670 LOAD_CONST              19 ("' ")
+                     672 BINARY_OP                0 (+)
+                     676 LOAD_DEREF               7 (granularity)
+                     678 BINARY_OP                0 (+)
+                     682 LOAD_CONST              10 (' ')
+                     684 LOAD_METHOD              6 (join)
+                     706 LOAD_FAST                5 (rest)
+                     708 PRECALL                  1
+                     712 CALL                     1
+                     722 BINARY_OP                0 (+)
+         
+         234         726 LOAD_METHOD             11 (replace)
+                     748 LOAD_GLOBAL             24 (param_left_placeholder)
+                     760 LOAD_GLOBAL             26 (double_quoted_param_left_placeholder)
+                     772 PRECALL                  2
+                     776 CALL                     2
+         
+         235         786 LOAD_METHOD             11 (replace)
+                     808 LOAD_GLOBAL             28 (param_right_placeholder)
+                     820 LOAD_GLOBAL             30 (double_quoted_param_right_placeholder)
+                     832 PRECALL                  2
+                     836 CALL                     2
+         
+         232         846 STORE_FAST               6 (final_interval)
+         
+         237         848 LOAD_GLOBAL             33 (NULL + sqlglot)
+                     860 LOAD_ATTR               17 (parse_one)
+                     870 LOAD_FAST                6 (final_interval)
+                     872 LOAD_CONST              20 ('trino')
+                     874 KW_NAMES                21
+                     876 PRECALL                  2
+                     880 CALL                     2
+                     890 RETURN_VALUE
          
-         233         630 LOAD_METHOD             10 (replace)
-                     652 LOAD_GLOBAL             22 (param_left_placeholder)
-                     664 LOAD_GLOBAL             24 (double_quoted_param_left_placeholder)
-                     676 PRECALL                  2
-                     680 CALL                     2
-         
-         234         690 LOAD_METHOD             10 (replace)
-                     712 LOAD_GLOBAL             26 (param_right_placeholder)
-                     724 LOAD_GLOBAL             28 (double_quoted_param_right_placeholder)
-                     736 PRECALL                  2
-                     740 CALL                     2
-         
-         231         750 STORE_FAST               7 (final_interval)
-         
-         236         752 LOAD_GLOBAL             31 (NULL + sqlglot)
-                     764 LOAD_ATTR               16 (parse_one)
-                     774 LOAD_FAST                7 (final_interval)
-                     776 LOAD_CONST              20 ('trino')
-                     778 KW_NAMES                21
-                     780 PRECALL                  2
-                     784 CALL                     2
-                     794 RETURN_VALUE
-         
-         237     >>  796 LOAD_FAST                0 (node)
-                     798 RETURN_VALUE
+         238     >>  892 LOAD_FAST                0 (node)
+                     894 RETURN_VALUE
          consts
             'Handle interval syntax change from Spark to Trino'
             'interval'
             0
             '('
             -1
             ')'
@@ -1247,15 +1264,15 @@
                argcount  : 1
                nlocals   : 2
                stacksize : 4
                flags     : 19
                code
                   0x970067007c005d0a7d017c0164006b0300000000af087c0191028c0b53
                   00
-               207           0 RESUME                   0
+               206           0 RESUME                   0
                              2 BUILD_LIST               0
                              4 LOAD_FAST                0 (.0)
                        >>    6 FOR_ITER                10 (to 28)
                              8 STORE_FAST               1 (i)
                             10 LOAD_FAST                1 (i)
                             12 LOAD_CONST               0 ('')
                             14 COMPARE_OP               3 (!=)
@@ -1266,82 +1283,82 @@
                        >>   28 RETURN_VALUE
                consts
                   ''
                names      ()
                varnames   ('.0', 'i')
                freevars   ()
                cellvars   ()
-               filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py'
+               filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/custom_transforms.py'
                name       '<listcomp>'
-               firstlineno 207
+               firstlineno 206
                lnotab 0x
             None
             ' '
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 4
                flags     : 51
                code
                   0x95014b00010097007c005d1a7d017c018902a000000000000000000000
                   0000000000000000000000a6000000ab0000000000000000007600560097
                   0101008c1b64005300
                              0 COPY_FREE_VARS           1
                
-               213           2 RETURN_GENERATOR
+               214           2 RETURN_GENERATOR
                              4 POP_TOP
                              6 RESUME                   0
                              8 LOAD_FAST                0 (.0)
                        >>   10 FOR_ITER                26 (to 64)
                
-               215          12 STORE_FAST               1 (known_granularity)
+               216          12 STORE_FAST               1 (known_granularity)
                
-               214          14 LOAD_FAST                1 (known_granularity)
+               215          14 LOAD_FAST                1 (known_granularity)
                             16 LOAD_DEREF               2 (granularity)
                             18 LOAD_METHOD              0 (lower)
                             40 PRECALL                  0
                             44 CALL                     0
                             54 CONTAINS_OP              0
                
-               213          56 YIELD_VALUE
+               214          56 YIELD_VALUE
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
-               filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py'
+               filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/custom_transforms.py'
                name       '<genexpr>'
-               firstlineno 213
+               firstlineno 214
                lnotab 0x0c0202ff2aff
             ('second', 'minute', 'hour', 'day', 'week', 'month', 'year')
             's'
             'week'
             7
             'day'
             "--week doesn't work in DuneSQL\n"
             "INTERVAL '"
             "' "
             'trino'
             ('read',)
-         names      ('key', 'str', 'this', 're', 'split', 'len', 'join', 'any', 'int', 'append', 'replace', 'param_left_placeholder', 'double_quoted_param_left_placeholder', 'param_right_placeholder', 'double_quoted_param_right_placeholder', 'sqlglot', 'parse_one')
-         varnames   ('node', 'interval_argument', 'regex_split', 'regex_matches', 'identifier', 'value', 'rest', 'final_interval')
+         names      ('key', 'str', 'this', 're', 'split', 'len', 'join', 'any', 'endswith', 'int', 'append', 'replace', 'param_left_placeholder', 'double_quoted_param_left_placeholder', 'param_right_placeholder', 'double_quoted_param_right_placeholder', 'sqlglot', 'parse_one')
+         varnames   ('node', 'interval_argument', 'regex_split', 'regex_matches', 'value', 'rest', 'final_interval')
          freevars   ()
          cellvars   ('granularity',)
-         filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py'
+         filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/custom_transforms.py'
          name       'interval_fix'
-         firstlineno 196
+         firstlineno 195
          lnotab
-            0x040218022801300114022a032802260104012a012e01140202fe200c18
-            0114010c01240104012a025a013c013cfd02052c01
+            0x040218022801300114022a032802260104012a014a0104012e01140202
+            fe200c2a0114010c01240104012a025a013c013cfd02052c01
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 7
          flags     : 3
          code
             0x8700970089006a00000000000000000064016b020000000072ed740300
@@ -1359,90 +1376,90 @@
             09a6010000ab010000000000000000a00a00000000000000000000000000
             00000000000000640aa6010000ab010000000000000000640b1900000000
             0000000000640c7a0000007c02a00b000000000000000000000000000000
             0000000000640da6010000ab0100000000000000007a000000640e7a0000
             006408ac0fa6020000ab020000000000000000530089005300
                        0 MAKE_CELL                0 (node)
          
-         240           2 RESUME                   0
+         241           2 RESUME                   0
          
-         242           4 LOAD_DEREF               0 (node)
+         243           4 LOAD_DEREF               0 (node)
                        6 LOAD_ATTR                0 (key)
                       16 LOAD_CONST               1 ('eq')
                       18 COMPARE_OP               2 (==)
                       24 POP_JUMP_FORWARD_IF_FALSE   237 (to 500)
          
-         243          26 LOAD_GLOBAL              3 (NULL + all)
+         244          26 LOAD_GLOBAL              3 (NULL + all)
                       38 LOAD_CLOSURE             0 (node)
                       40 BUILD_TUPLE              1
-                      42 LOAD_CONST               2 (<code object <genexpr>, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py", line 243>)
+                      42 LOAD_CONST               2 (<code object <genexpr>, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/custom_transforms.py", line 244>)
                       44 MAKE_FUNCTION            8 (closure)
          
-         246          46 LOAD_CONST               3 ('0x')
+         247          46 LOAD_CONST               3 ('0x')
          
-         247          48 LOAD_CONST               4 ('substring(')
+         248          48 LOAD_CONST               4 ('substring(')
          
-         248          50 LOAD_GLOBAL              4 (double_quoted_param_left_placeholder)
+         249          50 LOAD_GLOBAL              4 (double_quoted_param_left_placeholder)
          
-         249          62 LOAD_GLOBAL              6 (double_quoted_param_right_placeholder)
+         250          62 LOAD_GLOBAL              6 (double_quoted_param_right_placeholder)
          
-         245          74 BUILD_TUPLE              4
+         246          74 BUILD_TUPLE              4
          
-         243          76 GET_ITER
+         244          76 GET_ITER
                       78 PRECALL                  0
                       82 CALL                     0
                       92 PRECALL                  1
                       96 CALL                     1
                      106 POP_JUMP_FORWARD_IF_FALSE   196 (to 500)
          
-         254         108 LOAD_CONST               5 ('.*SUBSTRING\\(\\s*[\'\\"]')
+         255         108 LOAD_CONST               5 ('.*SUBSTRING\\(\\s*[\'\\"]')
          
-         255         110 LOAD_GLOBAL              9 (NULL + re)
+         256         110 LOAD_GLOBAL              9 (NULL + re)
                      122 LOAD_ATTR                5 (escape)
                      132 LOAD_GLOBAL              4 (double_quoted_param_left_placeholder)
                      144 PRECALL                  1
                      148 CALL                     1
          
-         254         158 BINARY_OP                0 (+)
+         255         158 BINARY_OP                0 (+)
          
-         256         162 LOAD_CONST               6 ('(.*?)')
+         257         162 LOAD_CONST               6 ('(.*?)')
          
-         254         164 BINARY_OP                0 (+)
+         255         164 BINARY_OP                0 (+)
          
-         257         168 LOAD_GLOBAL              9 (NULL + re)
+         258         168 LOAD_GLOBAL              9 (NULL + re)
                      180 LOAD_ATTR                5 (escape)
                      190 LOAD_GLOBAL              6 (double_quoted_param_right_placeholder)
                      202 PRECALL                  1
                      206 CALL                     1
          
-         254         216 BINARY_OP                0 (+)
+         255         216 BINARY_OP                0 (+)
          
-         258         220 LOAD_CONST               7 ('[\'\\"].*?\\)')
+         259         220 LOAD_CONST               7 ('[\'\\"].*?\\)')
          
-         254         222 BINARY_OP                0 (+)
+         255         222 BINARY_OP                0 (+)
          
-         253         226 STORE_FAST               1 (pattern)
+         254         226 STORE_FAST               1 (pattern)
          
-         260         228 LOAD_GLOBAL              9 (NULL + re)
+         261         228 LOAD_GLOBAL              9 (NULL + re)
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
          
-         261         310 LOAD_GLOBAL             17 (NULL + sqlglot)
+         262         310 LOAD_GLOBAL             17 (NULL + sqlglot)
                      322 LOAD_ATTR                9 (parse_one)
          
-         262         332 LOAD_DEREF               0 (node)
+         263         332 LOAD_DEREF               0 (node)
                      334 LOAD_METHOD              7 (sql)
                      356 LOAD_CONST               8 ('trino')
                      358 KW_NAMES                 9
                      360 PRECALL                  1
                      364 CALL                     1
                      374 LOAD_METHOD             10 (split)
                      396 LOAD_CONST              10 ('=')
@@ -1458,20 +1475,20 @@
                      456 PRECALL                  1
                      460 CALL                     1
                      470 BINARY_OP                0 (+)
                      474 LOAD_CONST              14 ('}}")')
                      476 BINARY_OP                0 (+)
                      480 LOAD_CONST               8 ('trino')
          
-         261         482 KW_NAMES                15
+         262         482 KW_NAMES                15
                      484 PRECALL                  2
                      488 CALL                     2
                      498 RETURN_VALUE
          
-         264     >>  500 LOAD_DEREF               0 (node)
+         265     >>  500 LOAD_DEREF               0 (node)
                      502 RETURN_VALUE
          consts
             'Take care of parameters that use bytearrays'
             'eq'
             code
                argcount  : 1
                nlocals   : 2
@@ -1480,51 +1497,51 @@
                code
                   0x95014b00010097007c005d2e7d017c018902a000000000000000000000
                   00000000000000000000006400ac01a6010000ab010000000000000000a0
                   010000000000000000000000000000000000000000a6000000ab00000000
                   000000000076005600970101008c2f64025300
                              0 COPY_FREE_VARS           1
                
-               243           2 RETURN_GENERATOR
+               244           2 RETURN_GENERATOR
                              4 POP_TOP
                              6 RESUME                   0
                              8 LOAD_FAST                0 (.0)
                        >>   10 FOR_ITER                46 (to 104)
                
-               245          12 STORE_FAST               1 (a_param)
+               246          12 STORE_FAST               1 (a_param)
                
-               244          14 LOAD_FAST                1 (a_param)
+               245          14 LOAD_FAST                1 (a_param)
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
                
-               243          96 YIELD_VALUE
+               244          96 YIELD_VALUE
                             98 RESUME                   1
                            100 POP_TOP
                            102 JUMP_BACKWARD           47 (to 10)
                        >>  104 LOAD_CONST               2 (None)
                            106 RETURN_VALUE
                consts
                   'trino'
                   ('dialect',)
                   None
                names      ('sql', 'lower')
                varnames   ('.0', 'a_param')
                freevars   ('node',)
                cellvars   ()
-               filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py'
+               filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/custom_transforms.py'
                name       '<genexpr>'
-               firstlineno 243
+               firstlineno 244
                lnotab 0x0c0202ff52ff
             '0x'
             'substring('
             '.*SUBSTRING\\(\\s*[\'\\"]'
             '(.*?)'
             '[\'\\"].*?\\)'
             'trino'
@@ -1535,17 +1552,17 @@
             1
             '}}")'
             ('read',)
          names      ('key', 'all', 'double_quoted_param_left_placeholder', 'double_quoted_param_right_placeholder', 're', 'escape', 'search', 'sql', 'sqlglot', 'parse_one', 'split', 'group')
          varnames   ('node', 'pattern', 'match')
          freevars   ()
          cellvars   ('node',)
-         filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py'
+         filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/custom_transforms.py'
          name       'bytearray_parameter_fix'
-         firstlineno 240
+         firstlineno 241
          lnotab
             0x040216011403020102010c010cfc02fe200b020130ff040202fe040330
             fd040402fc04ff02075201160196ff1203
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 4
@@ -1555,50 +1572,50 @@
             000000000000000000880066016402840864034400a6000000ab00000000
             0000000000a6010000ab0100000000000000007221740500000000000000
             0000006a030000000000000000640489006a0400000000000000007a0000
             0064057a0000006406ac07a6020000ab0200000000000000005300890053
             00
                        0 MAKE_CELL                0 (node)
          
-         267           2 RESUME                   0
+         268           2 RESUME                   0
          
-         270           4 LOAD_DEREF               0 (node)
+         271           4 LOAD_DEREF               0 (node)
                        6 LOAD_ATTR                0 (key)
                       16 LOAD_CONST               1 ('column')
                       18 COMPARE_OP               2 (==)
                       24 POP_JUMP_FORWARD_IF_FALSE    60 (to 146)
          
-         271          26 LOAD_GLOBAL              3 (NULL + any)
+         272          26 LOAD_GLOBAL              3 (NULL + any)
                       38 LOAD_CLOSURE             0 (node)
                       40 BUILD_TUPLE              1
-                      42 LOAD_CONST               2 (<code object <genexpr>, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py", line 271>)
+                      42 LOAD_CONST               2 (<code object <genexpr>, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/custom_transforms.py", line 272>)
                       44 MAKE_FUNCTION            8 (closure)
                       46 LOAD_CONST               3 (('amount', 'value'))
                       48 GET_ITER
                       50 PRECALL                  0
                       54 CALL                     0
                       64 PRECALL                  1
                       68 CALL                     1
                       78 POP_JUMP_FORWARD_IF_FALSE    33 (to 146)
          
-         272          80 LOAD_GLOBAL              5 (NULL + sqlglot)
+         273          80 LOAD_GLOBAL              5 (NULL + sqlglot)
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
          
-         273     >>  146 LOAD_DEREF               0 (node)
+         274     >>  146 LOAD_DEREF               0 (node)
                      148 RETURN_VALUE
          consts
             'if a column is being added, subtracted, multiplied, divided, etc,\n    and it has amount/value in the name, cast to double'
             'column'
             code
                argcount  : 1
                nlocals   : 2
@@ -1606,15 +1623,15 @@
                flags     : 51
                code
                   0x95014b00010097007c005d1f7d017c0189026a000000000000000000a0
                   010000000000000000000000000000000000000000a6000000ab00000000
                   000000000076005600970101008c2064005300
                              0 COPY_FREE_VARS           1
                
-               271           2 RETURN_GENERATOR
+               272           2 RETURN_GENERATOR
                              4 POP_TOP
                              6 RESUME                   0
                              8 LOAD_FAST                0 (.0)
                        >>   10 FOR_ITER                31 (to 74)
                             12 STORE_FAST               1 (val)
                             14 LOAD_FAST                1 (val)
                             16 LOAD_DEREF               2 (node)
@@ -1631,30 +1648,30 @@
                             76 RETURN_VALUE
                consts
                   None
                names      ('name', 'lower')
                varnames   ('.0', 'val')
                freevars   ('node',)
                cellvars   ()
-               filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py'
+               filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/custom_transforms.py'
                name       '<genexpr>'
-               firstlineno 271
+               firstlineno 272
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
-         filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py'
+         filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/custom_transforms.py'
          name       'cast_numeric'
-         firstlineno 267
+         firstlineno 268
          lnotab 0x0403160136014201
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 6
          flags     : 3
          code
@@ -1675,37 +1692,37 @@
             000000ab000000000000000000a6010000ab010000000000000000722f74
             09000000000000000000006a050000000000000000640a7c02a00a000000
             0000000000000000000000000000000000640ba6010000ab010000000000
             0000007a000000640c7a0000006403ac06a6020000ab0200000000000000
             00530089005300
                        0 MAKE_CELL                0 (node)
          
-         276           2 RESUME                   0
+         277           2 RESUME                   0
          
-         277           4 LOAD_DEREF               0 (node)
+         278           4 LOAD_DEREF               0 (node)
                        6 LOAD_ATTR                0 (key)
                       16 LOAD_CONST               1 ('literal')
                       18 COMPARE_OP               2 (==)
                       24 EXTENDED_ARG             1
                       26 POP_JUMP_FORWARD_IF_FALSE   257 (to 542)
          
-         279          28 LOAD_GLOBAL              3 (NULL + re)
+         280          28 LOAD_GLOBAL              3 (NULL + re)
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
          
-         280         110 LOAD_GLOBAL              9 (NULL + sqlglot)
+         281         110 LOAD_GLOBAL              9 (NULL + sqlglot)
                      122 LOAD_ATTR                5 (parse_one)
                      132 LOAD_CONST               5 ('timestamp ')
                      134 LOAD_DEREF               0 (node)
                      136 LOAD_METHOD              3 (sql)
                      158 LOAD_CONST               3 ('trino')
                      160 KW_NAMES                 4
                      162 PRECALL                  1
@@ -1713,63 +1730,63 @@
                      176 BINARY_OP                0 (+)
                      180 LOAD_CONST               3 ('trino')
                      182 KW_NAMES                 6
                      184 PRECALL                  2
                      188 CALL                     2
                      198 RETURN_VALUE
          
-         284     >>  200 LOAD_GLOBAL              3 (NULL + re)
+         285     >>  200 LOAD_GLOBAL              3 (NULL + re)
                      212 LOAD_ATTR                6 (escape)
                      222 LOAD_GLOBAL             14 (double_quoted_param_left_placeholder)
                      234 PRECALL                  1
                      238 CALL                     1
          
-         285         248 LOAD_CONST               7 ('(.*?)')
+         286         248 LOAD_CONST               7 ('(.*?)')
          
-         284         250 BINARY_OP                0 (+)
+         285         250 BINARY_OP                0 (+)
          
-         286         254 LOAD_GLOBAL              3 (NULL + re)
+         287         254 LOAD_GLOBAL              3 (NULL + re)
                      266 LOAD_ATTR                6 (escape)
                      276 LOAD_GLOBAL             16 (double_quoted_param_right_placeholder)
                      288 PRECALL                  1
                      292 CALL                     1
          
-         284         302 BINARY_OP                0 (+)
+         285         302 BINARY_OP                0 (+)
          
-         283         306 STORE_FAST               1 (pattern)
+         284         306 STORE_FAST               1 (pattern)
          
-         288         308 LOAD_GLOBAL              3 (NULL + re)
+         289         308 LOAD_GLOBAL              3 (NULL + re)
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
          
-         289         390 LOAD_FAST                2 (match)
+         290         390 LOAD_FAST                2 (match)
                      392 POP_JUMP_FORWARD_IF_FALSE    74 (to 542)
                      394 LOAD_GLOBAL             19 (NULL + any)
                      406 LOAD_CLOSURE             0 (node)
                      408 BUILD_TUPLE              1
-                     410 LOAD_CONST               8 (<code object <genexpr>, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py", line 289>)
+                     410 LOAD_CONST               8 (<code object <genexpr>, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/custom_transforms.py", line 290>)
                      412 MAKE_FUNCTION            8 (closure)
                      414 LOAD_CONST               9 (('date', 'time'))
                      416 GET_ITER
                      418 PRECALL                  0
                      422 CALL                     0
                      432 PRECALL                  1
                      436 CALL                     1
                      446 POP_JUMP_FORWARD_IF_FALSE    47 (to 542)
          
-         290         448 LOAD_GLOBAL              9 (NULL + sqlglot)
+         291         448 LOAD_GLOBAL              9 (NULL + sqlglot)
                      460 LOAD_ATTR                5 (parse_one)
                      470 LOAD_CONST              10 ("timestamp '{{")
                      472 LOAD_FAST                2 (match)
                      474 LOAD_METHOD             10 (group)
                      496 LOAD_CONST              11 (1)
                      498 PRECALL                  1
                      502 CALL                     1
@@ -1778,15 +1795,15 @@
                      518 BINARY_OP                0 (+)
                      522 LOAD_CONST               3 ('trino')
                      524 KW_NAMES                 6
                      526 PRECALL                  2
                      530 CALL                     2
                      540 RETURN_VALUE
          
-         291     >>  542 LOAD_DEREF               0 (node)
+         292     >>  542 LOAD_DEREF               0 (node)
                      544 RETURN_VALUE
          consts
             None
             'literal'
             '\\d{4}-\\d{2}-\\d{2}'
             'trino'
             ('dialect',)
@@ -1801,15 +1818,15 @@
                code
                   0x95014b00010097007c005d2e7d017c018902a000000000000000000000
                   00000000000000000000006400ac01a6010000ab010000000000000000a0
                   010000000000000000000000000000000000000000a6000000ab00000000
                   000000000076005600970101008c2f64025300
                              0 COPY_FREE_VARS           1
                
-               289           2 RETURN_GENERATOR
+               290           2 RETURN_GENERATOR
                              4 POP_TOP
                              6 RESUME                   0
                              8 LOAD_FAST                0 (.0)
                        >>   10 FOR_ITER                46 (to 104)
                             12 STORE_FAST               1 (d)
                             14 LOAD_FAST                1 (d)
                             16 LOAD_DEREF               2 (node)
@@ -1832,29 +1849,29 @@
                   'trino'
                   ('dialect',)
                   None
                names      ('sql', 'lower')
                varnames   ('.0', 'd')
                freevars   ('node',)
                cellvars   ()
-               filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py'
+               filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/custom_transforms.py'
                name       '<genexpr>'
-               firstlineno 289
+               firstlineno 290
                lnotab 0x
             ('date', 'time')
             "timestamp '{{"
             1
             "}}'"
          names      ('key', 're', 'search', 'sql', 'sqlglot', 'parse_one', 'escape', 'double_quoted_param_left_placeholder', 'double_quoted_param_right_placeholder', 'any', 'group')
          varnames   ('node', 'pattern', 'match')
          freevars   ()
          cellvars   ('node',)
-         filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py'
+         filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/custom_transforms.py'
          name       'cast_timestamp'
-         firstlineno 276
+         firstlineno 277
          lnotab 0x0401180252015a04300102ff040230fe04ff020552013a015e01
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 4
          flags     : 3
          code
@@ -1865,36 +1882,36 @@
             000000a003000000000000000000000000000000000000000064066407a6
             020000ab020000000000000000a003000000000000000000000000000000
             000000000064086407a6020000ab0200000000000000007d017409000000
             000000000000006a0500000000000000007c016404ac09a6020000ab0200
             00000000000000530089005300
                        0 MAKE_CELL                0 (node)
          
-         294           2 RESUME                   0
+         295           2 RESUME                   0
          
-         296           4 LOAD_DEREF               0 (node)
+         297           4 LOAD_DEREF               0 (node)
                        6 LOAD_ATTR                0 (key)
                       16 LOAD_CONST               1 ('literal')
                       18 COMPARE_OP               2 (==)
                       24 POP_JUMP_FORWARD_IF_FALSE   111 (to 248)
          
-         297          26 LOAD_GLOBAL              3 (NULL + any)
+         298          26 LOAD_GLOBAL              3 (NULL + any)
                       38 LOAD_CLOSURE             0 (node)
                       40 BUILD_TUPLE              1
-                      42 LOAD_CONST               2 (<code object <genexpr>, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py", line 297>)
+                      42 LOAD_CONST               2 (<code object <genexpr>, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/custom_transforms.py", line 298>)
                       44 MAKE_FUNCTION            8 (closure)
                       46 LOAD_CONST               3 (('true', 'false'))
                       48 GET_ITER
                       50 PRECALL                  0
                       54 CALL                     0
                       64 PRECALL                  1
                       68 CALL                     1
                       78 POP_JUMP_FORWARD_IF_FALSE    84 (to 248)
          
-         299          80 LOAD_DEREF               0 (node)
+         300          80 LOAD_DEREF               0 (node)
                       82 LOAD_METHOD              2 (sql)
                      104 LOAD_CONST               4 ('trino')
                      106 KW_NAMES                 5
                      108 PRECALL                  1
                      112 CALL                     1
                      122 LOAD_METHOD              3 (replace)
                      144 LOAD_CONST               6 ('"')
@@ -1904,24 +1921,24 @@
                      162 LOAD_METHOD              3 (replace)
                      184 LOAD_CONST               8 ("'")
                      186 LOAD_CONST               7 ('')
                      188 PRECALL                  2
                      192 CALL                     2
                      202 STORE_FAST               1 (bool_cleaned)
          
-         300         204 LOAD_GLOBAL              9 (NULL + sqlglot)
+         301         204 LOAD_GLOBAL              9 (NULL + sqlglot)
                      216 LOAD_ATTR                5 (parse_one)
                      226 LOAD_FAST                1 (bool_cleaned)
                      228 LOAD_CONST               4 ('trino')
                      230 KW_NAMES                 9
                      232 PRECALL                  2
                      236 CALL                     2
                      246 RETURN_VALUE
          
-         301     >>  248 LOAD_DEREF               0 (node)
+         302     >>  248 LOAD_DEREF               0 (node)
                      250 RETURN_VALUE
          consts
             "If node.key is 'literal' and contains 'true' or 'false' then cast to boolean"
             'literal'
             code
                argcount  : 1
                nlocals   : 2
@@ -1930,15 +1947,15 @@
                code
                   0x95014b00010097007c005d2e7d017c018902a000000000000000000000
                   00000000000000000000006400ac01a6010000ab010000000000000000a0
                   010000000000000000000000000000000000000000a6000000ab00000000
                   000000000076005600970101008c2f64025300
                              0 COPY_FREE_VARS           1
                
-               297           2 RETURN_GENERATOR
+               298           2 RETURN_GENERATOR
                              4 POP_TOP
                              6 RESUME                   0
                              8 LOAD_FAST                0 (.0)
                        >>   10 FOR_ITER                46 (to 104)
                             12 STORE_FAST               1 (boolean)
                             14 LOAD_FAST                1 (boolean)
                             16 LOAD_DEREF               2 (node)
@@ -1961,234 +1978,234 @@
                   'trino'
                   ('dialect',)
                   None
                names      ('sql', 'lower')
                varnames   ('.0', 'boolean')
                freevars   ('node',)
                cellvars   ()
-               filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py'
+               filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/custom_transforms.py'
                name       '<genexpr>'
-               firstlineno 297
+               firstlineno 298
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
-         filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py'
+         filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/custom_transforms.py'
          name       'fix_boolean'
-         firstlineno 294
+         firstlineno 295
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
-         304           0 RESUME                   0
+         305           0 RESUME                   0
          
-         306           2 LOAD_FAST                0 (node)
+         307           2 LOAD_FAST                0 (node)
                        4 LOAD_ATTR                0 (name)
                       14 LOAD_METHOD              1 (lower)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 LOAD_CONST               1 (('unnest', 'explode'))
                       52 CONTAINS_OP              0
                       54 POP_JUMP_FORWARD_IF_FALSE    45 (to 146)
          
-         307          56 LOAD_GLOBAL              5 (NULL + sqlglot)
+         308          56 LOAD_GLOBAL              5 (NULL + sqlglot)
                       68 LOAD_ATTR                3 (parse_one)
          
-         308          78 LOAD_FAST                0 (node)
+         309          78 LOAD_FAST                0 (node)
                       80 LOAD_METHOD              4 (sql)
                      102 LOAD_CONST               2 ('trino')
                      104 KW_NAMES                 3
                      106 PRECALL                  1
                      110 CALL                     1
          
-         310         120 LOAD_CONST               4 ("-- WARNING: You can't use explode/unnest inside SELECT anymore, it must be LATERAL or CROSS JOIN instead. Check out the docs here: https://dune.com/docs/query/syntax-differences/")
+         311         120 LOAD_CONST               4 ("-- WARNING: You can't use explode/unnest inside SELECT anymore, it must be LATERAL or CROSS JOIN instead. Check out the docs here: https://dune.com/docs/query/syntax-differences/")
          
-         308         122 BINARY_OP                0 (+)
+         309         122 BINARY_OP                0 (+)
          
-         313         126 LOAD_CONST               2 ('trino')
+         314         126 LOAD_CONST               2 ('trino')
          
-         307         128 KW_NAMES                 5
+         308         128 KW_NAMES                 5
                      130 PRECALL                  2
                      134 CALL                     2
                      144 RETURN_VALUE
          
-         315     >>  146 LOAD_FAST                0 (node)
+         316     >>  146 LOAD_FAST                0 (node)
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
-         filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py'
+         filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/custom_transforms.py'
          name       'warn_unnest'
-         firstlineno 304
+         firstlineno 305
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
-         318           0 RESUME                   0
+         319           0 RESUME                   0
          
-         320           2 LOAD_FAST                0 (node)
+         321           2 LOAD_FAST                0 (node)
                        4 LOAD_ATTR                0 (name)
                       14 LOAD_METHOD              1 (lower)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 LOAD_CONST               1 (('generate_series', 'sequence'))
                       52 CONTAINS_OP              0
                       54 POP_JUMP_FORWARD_IF_FALSE    45 (to 146)
          
-         321          56 LOAD_GLOBAL              5 (NULL + sqlglot)
+         322          56 LOAD_GLOBAL              5 (NULL + sqlglot)
                       68 LOAD_ATTR                3 (parse_one)
          
-         322          78 LOAD_FAST                0 (node)
+         323          78 LOAD_FAST                0 (node)
                       80 LOAD_METHOD              4 (sql)
                      102 LOAD_CONST               2 ('trino')
                      104 KW_NAMES                 3
                      106 PRECALL                  1
                      110 CALL                     1
          
-         324         120 LOAD_CONST               4 ('-- WARNING: Check out the docs for example of time series generation: https://dune.com/docs/query/syntax-differences/')
+         325         120 LOAD_CONST               4 ('-- WARNING: Check out the docs for example of time series generation: https://dune.com/docs/query/syntax-differences/')
          
-         322         122 BINARY_OP                0 (+)
+         323         122 BINARY_OP                0 (+)
          
-         327         126 LOAD_CONST               2 ('trino')
+         328         126 LOAD_CONST               2 ('trino')
          
-         321         128 KW_NAMES                 5
+         322         128 KW_NAMES                 5
                      130 PRECALL                  2
                      134 CALL                     2
                      144 RETURN_VALUE
          
-         329     >>  146 LOAD_FAST                0 (node)
+         330     >>  146 LOAD_FAST                0 (node)
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
-         filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py'
+         filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/custom_transforms.py'
          name       'warn_sequence'
-         firstlineno 318
+         firstlineno 319
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
-         332           0 RESUME                   0
+         333           0 RESUME                   0
          
-         333           2 LOAD_CONST               1 (('replace',))
+         334           2 LOAD_CONST               1 (('replace',))
                        4 GET_ITER
                  >>    6 FOR_ITER                66 (to 140)
                        8 STORE_FAST               1 (keyword)
          
-         335          10 LOAD_GLOBAL              1 (NULL + re)
+         336          10 LOAD_GLOBAL              1 (NULL + re)
                       22 LOAD_ATTR                1 (sub)
          
-         336          32 LOAD_CONST               2 ('\\b')
+         337          32 LOAD_CONST               2 ('\\b')
                       34 LOAD_GLOBAL              1 (NULL + re)
                       46 LOAD_ATTR                2 (escape)
                       56 LOAD_FAST                1 (keyword)
                       58 PRECALL                  1
                       62 CALL                     1
                       72 BINARY_OP                0 (+)
                       76 LOAD_CONST               3 ('(?!\\()')
                       78 BINARY_OP                0 (+)
          
-         337          82 LOAD_CONST               4 ('"')
+         338          82 LOAD_CONST               4 ('"')
                       84 LOAD_FAST                1 (keyword)
                       86 BINARY_OP                0 (+)
                       90 LOAD_CONST               4 ('"')
                       92 BINARY_OP                0 (+)
          
-         338          96 LOAD_FAST                0 (query)
+         339          96 LOAD_FAST                0 (query)
          
-         339          98 LOAD_GLOBAL              0 (re)
+         340          98 LOAD_GLOBAL              0 (re)
                      110 LOAD_ATTR                3 (IGNORECASE)
          
-         335         120 KW_NAMES                 5
+         336         120 KW_NAMES                 5
                      122 PRECALL                  4
                      126 CALL                     4
                      136 STORE_FAST               0 (query)
                      138 JUMP_BACKWARD           67 (to 6)
          
-         341     >>  140 LOAD_FAST                0 (query)
+         342     >>  140 LOAD_FAST                0 (query)
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
-         filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py'
+         filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/custom_transforms.py'
          name       'prep_query'
-         firstlineno 332
+         firstlineno 333
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
-         344           0 RESUME                   0
+         345           0 RESUME                   0
          
-         346           2 LOAD_GLOBAL              1 (NULL + sqlglot)
+         347           2 LOAD_GLOBAL              1 (NULL + sqlglot)
                       14 LOAD_ATTR                1 (parse_one)
                       24 LOAD_FAST                0 (query)
                       26 LOAD_METHOD              2 (sql)
                       48 LOAD_CONST               1 ('trino')
                       50 KW_NAMES                 2
                       52 PRECALL                  1
                       56 CALL                     1
@@ -2209,17 +2226,17 @@
             'usd_amount'
             'amount_usd'
             ('read',)
          names      ('sqlglot', 'parse_one', 'sql', 'replace')
          varnames   ('query',)
          freevars   ()
          cellvars   ()
-         filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py'
+         filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/custom_transforms.py'
          name       'rename_amount_column'
-         firstlineno 344
+         firstlineno 345
          lnotab 0x0202
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 6
          flags     : 3
          code
@@ -2227,52 +2244,52 @@
             02a6010000ab0100000000000000007d0164037c01a00100000000000000
             00000000000000000000000000a6000000ab000000000000000000760072
             277405000000000000000000006a030000000000000000640364047c0174
             04000000000000000000006a040000000000000000ac05a6040000ab0400
             000000000000007d0164067c017a0000007d01740b000000000000000000
             006a0600000000000000007c016401ac07a6020000ab0200000000000000
             005300
-         349           0 RESUME                   0
+         350           0 RESUME                   0
          
-         351           2 LOAD_FAST                0 (query_tree)
+         352           2 LOAD_FAST                0 (query_tree)
                        4 LOAD_METHOD              0 (sql)
                       26 LOAD_CONST               1 ('trino')
                       28 KW_NAMES                 2
                       30 PRECALL                  1
                       34 CALL                     1
                       44 STORE_FAST               1 (query)
          
-         352          46 LOAD_CONST               3 ('bytea2numeric')
+         353          46 LOAD_CONST               3 ('bytea2numeric')
                       48 LOAD_FAST                1 (query)
                       50 LOAD_METHOD              1 (lower)
                       72 PRECALL                  0
                       76 CALL                     0
                       86 CONTAINS_OP              0
                       88 POP_JUMP_FORWARD_IF_FALSE    39 (to 168)
          
-         353          90 LOAD_GLOBAL              5 (NULL + re)
+         354          90 LOAD_GLOBAL              5 (NULL + re)
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
          
-         355         158 LOAD_CONST               6 ('/* !Bytea warning: We now have new bytearray functions to cover conversions and stuff like length, concat, substring, etc. Check out the docs here: https://dune.com/docs/reference/dune-v2/query-engine/#byte-array-to-numeric-functions */\n\n')
+         356         158 LOAD_CONST               6 ('/* !Bytea warning: We now have new bytearray functions to cover conversions and stuff like length, concat, substring, etc. Check out the docs here: https://dune.com/docs/reference/dune-v2/query-engine/#byte-array-to-numeric-functions */\n\n')
          
-         359         160 LOAD_FAST                1 (query)
+         360         160 LOAD_FAST                1 (query)
          
-         354         162 BINARY_OP                0 (+)
+         355         162 BINARY_OP                0 (+)
                      166 STORE_FAST               1 (query)
          
-         360     >>  168 LOAD_GLOBAL             11 (NULL + sqlglot)
+         361     >>  168 LOAD_GLOBAL             11 (NULL + sqlglot)
                      180 LOAD_ATTR                6 (parse_one)
                      190 LOAD_FAST                1 (query)
                      192 LOAD_CONST               1 ('trino')
                      194 KW_NAMES                 7
                      196 PRECALL                  2
                      200 CALL                     2
                      210 RETURN_VALUE
@@ -2285,33 +2302,33 @@
             ('flags',)
             '/* !Bytea warning: We now have new bytearray functions to cover conversions and stuff like length, concat, substring, etc. Check out the docs here: https://dune.com/docs/reference/dune-v2/query-engine/#byte-array-to-numeric-functions */\n\n'
             ('read',)
          names      ('sql', 'lower', 're', 'sub', 'IGNORECASE', 'sqlglot', 'parse_one')
          varnames   ('query_tree', 'query')
          freevars   ()
          cellvars   ()
-         filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py'
+         filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/custom_transforms.py'
          name       'bytea2numeric'
-         firstlineno 349
+         firstlineno 350
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
-         363           0 RESUME                   0
+         364           0 RESUME                   0
          
-         365           2 LOAD_CONST               1 ('lower\\(\\s*[\'\\"]\\{\\{(.*?)\\}\\}[\'\\"]\\s*\\)')
+         366           2 LOAD_CONST               1 ('lower\\(\\s*[\'\\"]\\{\\{(.*?)\\}\\}[\'\\"]\\s*\\)')
                        4 STORE_FAST               1 (pattern)
          
-         366           6 LOAD_GLOBAL              1 (NULL + re)
+         367           6 LOAD_GLOBAL              1 (NULL + re)
                       18 LOAD_ATTR                1 (sub)
                       28 LOAD_FAST                1 (pattern)
                       30 LOAD_CONST               2 ('{{\\1}}')
                       32 LOAD_FAST                0 (query)
                       34 LOAD_GLOBAL              0 (re)
                       46 LOAD_ATTR                2 (IGNORECASE)
                       56 KW_NAMES                 3
@@ -2323,97 +2340,97 @@
             'lower\\(\\s*[\'\\"]\\{\\{(.*?)\\}\\}[\'\\"]\\s*\\)'
             '{{\\1}}'
             ('flags',)
          names      ('re', 'sub', 'IGNORECASE')
          varnames   ('query', 'pattern')
          freevars   ()
          cellvars   ()
-         filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py'
+         filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/custom_transforms.py'
          name       'fix_bytearray_param'
-         firstlineno 363
+         firstlineno 364
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
-         369           0 RESUME                   0
+         370           0 RESUME                   0
          
-         373           2 LOAD_CONST               1 ('lower\\(\\s*[\'\\"]0x(.*?)[\'\\"]\\s*\\)')
+         374           2 LOAD_CONST               1 ('lower\\(\\s*[\'\\"]0x(.*?)[\'\\"]\\s*\\)')
                        4 STORE_FAST               1 (pattern)
          
-         374           6 LOAD_GLOBAL              1 (NULL + re)
+         375           6 LOAD_GLOBAL              1 (NULL + re)
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
          
-         375          74 LOAD_FAST                2 (substituted)
+         376          74 LOAD_FAST                2 (substituted)
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
-         filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py'
+         filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/custom_transforms.py'
          name       'fix_bytearray_lower'
-         firstlineno 369
+         firstlineno 370
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
-         378           0 RESUME                   0
+         379           0 RESUME                   0
          
-         380           2 LOAD_GLOBAL              0 (chain_where_gnosis)
+         381           2 LOAD_GLOBAL              0 (chain_where_gnosis)
          
-         381          14 LOAD_GLOBAL              2 (chain_where_optimism)
+         382          14 LOAD_GLOBAL              2 (chain_where_optimism)
          
-         382          26 LOAD_GLOBAL              4 (chain_where_bnb)
+         383          26 LOAD_GLOBAL              4 (chain_where_bnb)
          
-         383          38 LOAD_GLOBAL              6 (chain_where_polygon)
+         384          38 LOAD_GLOBAL              6 (chain_where_polygon)
          
-         384          50 LOAD_GLOBAL              8 (chain_where_ethereum)
+         385          50 LOAD_GLOBAL              8 (chain_where_ethereum)
          
-         379          62 LOAD_CONST               1 (('gnosis', 'optimism', 'bnb', 'polygon', 'ethereum'))
+         380          62 LOAD_CONST               1 (('gnosis', 'optimism', 'bnb', 'polygon', 'ethereum'))
                       64 BUILD_CONST_KEY_MAP      5
          
-         385          66 LOAD_FAST                0 (dataset)
+         386          66 LOAD_FAST                0 (dataset)
          
-         379          68 BINARY_SUBSCR
+         380          68 BINARY_SUBSCR
                       78 RETURN_VALUE
          consts
             None
             ('gnosis', 'optimism', 'bnb', 'polygon', 'ethereum')
          names      ('chain_where_gnosis', 'chain_where_optimism', 'chain_where_bnb', 'chain_where_polygon', 'chain_where_ethereum')
          varnames   ('dataset',)
          freevars   ()
          cellvars   ()
-         filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py'
+         filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/custom_transforms.py'
          name       'chain_where'
-         firstlineno 378
+         firstlineno 379
          lnotab 0x02020c010c010c010c010cfb040602fa
       code
          argcount  : 2
          nlocals   : 5
          stacksize : 12
          flags     : 3
          code
@@ -2423,84 +2440,84 @@
             000000000000000000740a00000000000000000000740c00000000000000
             000000740e00000000000000000000741000000000000000000000741200
             0000000000000000007415000000000000000000007c01a6010000ab0100
             000000000000007416000000000000000000007418000000000000000000
             00741a00000000000000000000660c7d037c0344005d177d047c02a00e00
             000000000000000000000000000000000000007c04a6010000ab01000000
             00000000007d028c187c025300
-         388           0 RESUME                   0
+         389           0 RESUME                   0
          
-         392           2 LOAD_GLOBAL              1 (NULL + sqlglot)
+         393           2 LOAD_GLOBAL              1 (NULL + sqlglot)
                       14 LOAD_ATTR                1 (parse_one)
                       24 LOAD_FAST                0 (query)
                       26 LOAD_CONST               1 ('postgres')
                       28 KW_NAMES                 2
                       30 PRECALL                  2
                       34 CALL                     2
                       44 STORE_FAST               2 (query_tree)
          
-         394          46 LOAD_GLOBAL              5 (NULL + postgres_table_replacements)
+         395          46 LOAD_GLOBAL              5 (NULL + postgres_table_replacements)
                       58 LOAD_FAST                1 (dataset)
                       60 PRECALL                  1
                       64 CALL                     1
          
-         395          74 LOAD_GLOBAL              6 (interval_fix)
+         396          74 LOAD_GLOBAL              6 (interval_fix)
          
-         396          86 LOAD_GLOBAL              8 (fix_boolean)
+         397          86 LOAD_GLOBAL              8 (fix_boolean)
          
-         397          98 LOAD_GLOBAL             10 (cast_numeric)
+         398          98 LOAD_GLOBAL             10 (cast_numeric)
          
-         398         110 LOAD_GLOBAL             12 (cast_timestamp)
+         399         110 LOAD_GLOBAL             12 (cast_timestamp)
          
-         399         122 LOAD_GLOBAL             14 (warn_unnest)
+         400         122 LOAD_GLOBAL             14 (warn_unnest)
          
-         400         134 LOAD_GLOBAL             16 (warn_sequence)
+         401         134 LOAD_GLOBAL             16 (warn_sequence)
          
-         401         146 LOAD_GLOBAL             18 (dex_trades_fixes)
+         402         146 LOAD_GLOBAL             18 (dex_trades_fixes)
          
-         402         158 LOAD_GLOBAL             21 (NULL + chain_where)
+         403         158 LOAD_GLOBAL             21 (NULL + chain_where)
                      170 LOAD_FAST                1 (dataset)
                      172 PRECALL                  1
                      176 CALL                     1
          
-         403         186 LOAD_GLOBAL             22 (bytearray_parameter_fix)
+         404         186 LOAD_GLOBAL             22 (bytearray_parameter_fix)
          
-         404         198 LOAD_GLOBAL             24 (rename_amount_column)
+         405         198 LOAD_GLOBAL             24 (rename_amount_column)
          
-         405         210 LOAD_GLOBAL             26 (bytea2numeric)
+         406         210 LOAD_GLOBAL             26 (bytea2numeric)
          
-         393         222 BUILD_TUPLE             12
+         394         222 BUILD_TUPLE             12
                      224 STORE_FAST               3 (transforms)
          
-         407         226 LOAD_FAST                3 (transforms)
+         408         226 LOAD_FAST                3 (transforms)
                      228 GET_ITER
                  >>  230 FOR_ITER                23 (to 278)
                      232 STORE_FAST               4 (f)
          
-         408         234 LOAD_FAST                2 (query_tree)
+         409         234 LOAD_FAST                2 (query_tree)
                      236 LOAD_METHOD             14 (transform)
                      258 LOAD_FAST                4 (f)
                      260 PRECALL                  1
                      264 CALL                     1
                      274 STORE_FAST               2 (query_tree)
                      276 JUMP_BACKWARD           24 (to 230)
          
-         409     >>  278 LOAD_FAST                2 (query_tree)
+         410     >>  278 LOAD_FAST                2 (query_tree)
                      280 RETURN_VALUE
          consts
             "Apply a series of transforms to the query tree, recursively using SQLGlot's recursive transform function.\n\n    Each transform takes and returns a sqlglot.Expression"
             'postgres'
             ('read',)
          names      ('sqlglot', 'parse_one', 'postgres_table_replacements', 'interval_fix', 'fix_boolean', 'cast_numeric', 'cast_timestamp', 'warn_unnest', 'warn_sequence', 'dex_trades_fixes', 'chain_where', 'bytearray_parameter_fix', 'rename_amount_column', 'bytea2numeric', 'transform')
          varnames   ('query', 'dataset', 'query_tree', 'transforms', 'f')
          freevars   ()
          cellvars   ()
-         filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py'
-         name       'sqlglot_postgres_transforms'
-         firstlineno 388
+         filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/custom_transforms.py'
+         name       'postgres_transforms'
+         firstlineno 389
          lnotab
             0x02042c021c010c010c010c010c010c010c010c011c010c010c010cf404
             0e08012c01
       code
          argcount  : 1
          nlocals   : 4
          stacksize : 7
@@ -2509,157 +2526,157 @@
             0x97007401000000000000000000006a0100000000000000007c006401ac
             02a6020000ab0200000000000000007d0174040000000000000000000074
             0600000000000000000000740800000000000000000000740a0000000000
             0000000000740c00000000000000000000740e0000000000000000000074
             100000000000000000000066077d027c0244005d177d037c01a009000000
             00000000000000000000000000000000007c03a6010000ab010000000000
             0000007d018c187c015300
-         412           0 RESUME                   0
+         413           0 RESUME                   0
          
-         416           2 LOAD_GLOBAL              1 (NULL + sqlglot)
+         417           2 LOAD_GLOBAL              1 (NULL + sqlglot)
                       14 LOAD_ATTR                1 (parse_one)
                       24 LOAD_FAST                0 (query)
-                      26 LOAD_CONST               1 ('spark')
+                      26 LOAD_CONST               1 ('trino')
                       28 KW_NAMES                 2
                       30 PRECALL                  2
                       34 CALL                     2
                       44 STORE_FAST               1 (query_tree)
          
-         418          46 LOAD_GLOBAL              4 (interval_fix)
+         419          46 LOAD_GLOBAL              4 (interval_fix)
          
-         419          58 LOAD_GLOBAL              6 (fix_boolean)
+         420          58 LOAD_GLOBAL              6 (fix_boolean)
          
-         420          70 LOAD_GLOBAL              8 (cast_numeric)
+         421          70 LOAD_GLOBAL              8 (cast_numeric)
          
-         421          82 LOAD_GLOBAL             10 (cast_timestamp)
+         422          82 LOAD_GLOBAL             10 (cast_timestamp)
          
-         422          94 LOAD_GLOBAL             12 (warn_unnest)
+         423          94 LOAD_GLOBAL             12 (warn_unnest)
          
-         423         106 LOAD_GLOBAL             14 (warn_sequence)
+         424         106 LOAD_GLOBAL             14 (warn_sequence)
          
-         424         118 LOAD_GLOBAL             16 (bytea2numeric)
+         425         118 LOAD_GLOBAL             16 (bytea2numeric)
          
-         417         130 BUILD_TUPLE              7
+         418         130 BUILD_TUPLE              7
                      132 STORE_FAST               2 (transforms)
          
-         426         134 LOAD_FAST                2 (transforms)
+         427         134 LOAD_FAST                2 (transforms)
                      136 GET_ITER
                  >>  138 FOR_ITER                23 (to 186)
                      140 STORE_FAST               3 (f)
          
-         427         142 LOAD_FAST                1 (query_tree)
+         428         142 LOAD_FAST                1 (query_tree)
                      144 LOAD_METHOD              9 (transform)
                      166 LOAD_FAST                3 (f)
                      168 PRECALL                  1
                      172 CALL                     1
                      182 STORE_FAST               1 (query_tree)
                      184 JUMP_BACKWARD           24 (to 138)
          
-         428     >>  186 LOAD_FAST                1 (query_tree)
+         429     >>  186 LOAD_FAST                1 (query_tree)
                      188 RETURN_VALUE
          consts
             "Apply a series of transforms to the query tree, recursively using SQLGlot's recursive transform function.\n\n    Each transform takes and returns a sqlglot.Expression"
-            'spark'
+            'trino'
             ('read',)
          names      ('sqlglot', 'parse_one', 'interval_fix', 'fix_boolean', 'cast_numeric', 'cast_timestamp', 'warn_unnest', 'warn_sequence', 'bytea2numeric', 'transform')
          varnames   ('query', 'query_tree', 'transforms', 'f')
          freevars   ()
          cellvars   ()
-         filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py'
-         name       'sqlglot_spark_transforms'
-         firstlineno 412
+         filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/custom_transforms.py'
+         name       'spark_transforms'
+         firstlineno 413
          lnotab 0x02042c020c010c010c010c010c010c010cf9040908012c01
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
-         431           0 RESUME                   0
+         432           0 RESUME                   0
          
-         433           2 LOAD_CONST               1 ("lower('{{")
+         434           2 LOAD_CONST               1 ("lower('{{")
                        4 LOAD_FAST                0 (query)
                        6 LOAD_METHOD              0 (lower)
                       28 PRECALL                  0
                       32 CALL                     0
                       42 CONTAINS_OP              0
                       44 POP_JUMP_FORWARD_IF_FALSE     5 (to 56)
          
-         435          46 LOAD_CONST               2 ("/* !Bytea parameter warning: Make sure to change \\x to 0x in the parameters, bytea types are native now (no need for quotes or lower or \\x)' */\n\n")
+         436          46 LOAD_CONST               2 ("/* !Bytea parameter warning: Make sure to change \\x to 0x in the parameters, bytea types are native now (no need for quotes or lower or \\x)' */\n\n")
          
-         438          48 LOAD_FAST                0 (query)
+         439          48 LOAD_FAST                0 (query)
          
-         434          50 BINARY_OP                0 (+)
+         435          50 BINARY_OP                0 (+)
                       54 STORE_FAST               0 (query)
          
-         441     >>   56 LOAD_GLOBAL              3 (NULL + re)
+         442     >>   56 LOAD_GLOBAL              3 (NULL + re)
                       68 LOAD_ATTR                2 (search)
                       78 LOAD_CONST               3 ('\\[.*\\]')
                       80 LOAD_FAST                0 (query)
                       82 PRECALL                  2
                       86 CALL                     2
                       96 POP_JUMP_FORWARD_IF_FALSE     5 (to 108)
          
-         443          98 LOAD_CONST               4 ('/* !Array warning: Arrays in dune SQL are indexed from 1, not 0. The migrator will not catch this if you indexed using variables */\n\n')
+         444          98 LOAD_CONST               4 ('/* !Array warning: Arrays in dune SQL are indexed from 1, not 0. The migrator will not catch this if you indexed using variables */\n\n')
          
-         446         100 LOAD_FAST                0 (query)
+         447         100 LOAD_FAST                0 (query)
          
-         442         102 BINARY_OP                0 (+)
+         443         102 BINARY_OP                0 (+)
                      106 STORE_FAST               0 (query)
          
-         448     >>  108 LOAD_CONST               5 ('dune_user_generated')
+         449     >>  108 LOAD_CONST               5 ('dune_user_generated')
                      110 LOAD_FAST                0 (query)
                      112 LOAD_METHOD              0 (lower)
                      134 PRECALL                  0
                      138 CALL                     0
                      148 CONTAINS_OP              0
                      150 POP_JUMP_FORWARD_IF_FALSE     5 (to 162)
          
-         450         152 LOAD_CONST               6 ("/* !Generated view warning: you can't query views in dune_user_generated anymore. All queries in DuneSQL are by default views though (try querying the table 'query_1747157') */\n\n")
+         451         152 LOAD_CONST               6 ("/* !Generated view warning: you can't query views in dune_user_generated anymore. All queries in DuneSQL are by default views though (try querying the table 'query_1747157') */\n\n")
          
-         453         154 LOAD_FAST                0 (query)
+         454         154 LOAD_FAST                0 (query)
          
-         449         156 BINARY_OP                0 (+)
+         450         156 BINARY_OP                0 (+)
                      160 STORE_FAST               0 (query)
          
-         457     >>  162 LOAD_CONST               7 ("/* Success! If you're still running into issues, check out https://dune.com/docs/query/syntax-differences/ or reach out in the #dune-sql Discord channel. */\n\n")
+         458     >>  162 LOAD_CONST               7 ("/* Success! If you're still running into issues, check out https://dune.com/docs/query/syntax-differences/ or reach out in the #dune-sql Discord channel. */\n\n")
          
-         460         164 LOAD_FAST                0 (query)
+         461         164 LOAD_FAST                0 (query)
          
-         456         166 BINARY_OP                0 (+)
+         457         166 BINARY_OP                0 (+)
                      170 RETURN_VALUE
          consts
             "Add a success banner at the top, and look for a few cases of things we don't fix and add a warning if present"
             "lower('{{"
             "/* !Bytea parameter warning: Make sure to change \\x to 0x in the parameters, bytea types are native now (no need for quotes or lower or \\x)' */\n\n"
             '\\[.*\\]'
             '/* !Array warning: Arrays in dune SQL are indexed from 1, not 0. The migrator will not catch this if you indexed using variables */\n\n'
             'dune_user_generated'
             "/* !Generated view warning: you can't query views in dune_user_generated anymore. All queries in DuneSQL are by default views though (try querying the table 'query_1747157') */\n\n"
             "/* Success! If you're still running into issues, check out https://dune.com/docs/query/syntax-differences/ or reach out in the #dune-sql Discord channel. */\n\n"
          names      ('lower', 're', 'search')
          varnames   ('query',)
          freevars   ()
          cellvars   ()
-         filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py'
+         filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/custom_transforms.py'
          name       'add_warnings_and_banner'
-         firstlineno 431
+         firstlineno 432
          lnotab
             0x02022c02020302fc06072a02020302fc06062c02020302fc0608020302
             fc
-   names      ('re', 'functools', 'partial', 'sqlglot', 'dune.translate.table_replacements', 'postgres_table_replacements', 'extract_nested_select', 'recurse_where', 'chain_where_blockchain', 'chain_where_ethereum', 'chain_where_gnosis', 'chain_where_optimism', 'chain_where_bnb', 'chain_where_polygon', 'dex_trades_fixes', 'param_left_placeholder', 'param_right_placeholder', 'double_quoted_param_left_placeholder', 'double_quoted_param_right_placeholder', 'single_quoted_param_left_placeholder', 'single_quoted_param_right_placeholder', 'interval_fix', 'bytearray_parameter_fix', 'cast_numeric', 'cast_timestamp', 'fix_boolean', 'warn_unnest', 'warn_sequence', 'prep_query', 'rename_amount_column', 'bytea2numeric', 'fix_bytearray_param', 'fix_bytearray_lower', 'chain_where', 'sqlglot_postgres_transforms', 'sqlglot_spark_transforms', 'add_warnings_and_banner')
+   names      ('re', 'functools', 'partial', 'sqlglot', 'dune.translate.table_replacements', 'postgres_table_replacements', 'extract_nested_select', 'recurse_where', 'chain_where_blockchain', 'chain_where_ethereum', 'chain_where_gnosis', 'chain_where_optimism', 'chain_where_bnb', 'chain_where_polygon', 'dex_trades_fixes', 'param_left_placeholder', 'param_right_placeholder', 'double_quoted_param_left_placeholder', 'double_quoted_param_right_placeholder', 'single_quoted_param_left_placeholder', 'single_quoted_param_right_placeholder', 'interval_fix', 'bytearray_parameter_fix', 'cast_numeric', 'cast_timestamp', 'fix_boolean', 'warn_unnest', 'warn_sequence', 'prep_query', 'rename_amount_column', 'bytea2numeric', 'fix_bytearray_param', 'fix_bytearray_lower', 'chain_where', 'postgres_transforms', 'spark_transforms', 'add_warnings_and_banner')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/helpers.py'
+   filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/custom_transforms.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff020108010c0208020c030612065c06121a011a011a011a011a0306
-      2b040104010a010a010a010a04062c061b06090612060a060e060e060c06
+      0x00ff020108010c0208020c030613065906121a011a011a011a011a0306
+      2c040104010a010a010a010a04062e061b06090612060a060e060e060c06
       05060e06060609060a06180613
```

### Comparing `dune_query_translator-0.3.1/dune/translate/__pycache__/table_replacements.cpython-311.pyc` & `dune_query_translator-0.4.0/dune/translate/__pycache__/table_replacements.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0xc3c03764 (Thu Apr 13 08:43:47 2023 UTC)
+moddate:  0x9efd3864 (Fri Apr 14 07:15:42 2023 UTC)
 files sz: 2018
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code 0x9700640064016c005a00640064016c015a01640284005a0264015300
```

### Comparing `dune_query_translator-0.3.1/dune/translate/__pycache__/translate.cpython-311.pyc` & `dune_query_translator-0.4.0/dune/translate/__pycache__/translate.cpython-311.pyc`

 * *Files 10% similar despite different names*

#### Python bytecode

```diff
@@ -1,19 +1,19 @@
 magic:    0xa70d0d0a
-moddate:  0xc3c03764 (Thu Apr 13 08:43:47 2023 UTC)
-files sz: 2978
+moddate:  0x9efd3864 (Fri Apr 14 07:15:42 2023 UTC)
+files sz: 2956
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064026c016d025a0201
-      00640064036c036d045a040100640064046c056d065a066d075a076d085a
-      086d095a096d0a5a0a6d0b5a0b6d0c5a0c6d0d5a0d6d0e5a0e6d0f5a0f01
+      00640064036c036d045a046d055a056d065a066d075a076d085a086d095a
+      096d0a5a0a6d0b5a0b6d0c5a0c6d0d5a0d0100640064046c0e6d0f5a0f01
       00640584005a106407640684015a1164015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (re)
                  8 STORE_NAME               0 (re)
@@ -27,43 +27,43 @@
                 20 LOAD_CONST               2 (('ParseError',))
                 22 IMPORT_NAME              1 (sqlglot)
                 24 IMPORT_FROM              2 (ParseError)
                 26 STORE_NAME               2 (ParseError)
                 28 POP_TOP
    
      6          30 LOAD_CONST               0 (0)
-                32 LOAD_CONST               3 (('DuneTranslationError',))
-                34 IMPORT_NAME              3 (dune.translate.errors)
-                36 IMPORT_FROM              4 (DuneTranslationError)
-                38 STORE_NAME               4 (DuneTranslationError)
-                40 POP_TOP
+                32 LOAD_CONST               3 (('add_warnings_and_banner', 'double_quoted_param_left_placeholder', 'double_quoted_param_right_placeholder', 'fix_bytearray_lower', 'fix_bytearray_param', 'postgres_transforms', 'prep_query', 'single_quoted_param_left_placeholder', 'single_quoted_param_right_placeholder', 'spark_transforms'))
+                34 IMPORT_NAME              3 (dune.translate.custom_transforms)
+                36 IMPORT_FROM              4 (add_warnings_and_banner)
+                38 STORE_NAME               4 (add_warnings_and_banner)
+                40 IMPORT_FROM              5 (double_quoted_param_left_placeholder)
+                42 STORE_NAME               5 (double_quoted_param_left_placeholder)
+                44 IMPORT_FROM              6 (double_quoted_param_right_placeholder)
+                46 STORE_NAME               6 (double_quoted_param_right_placeholder)
+                48 IMPORT_FROM              7 (fix_bytearray_lower)
+                50 STORE_NAME               7 (fix_bytearray_lower)
+                52 IMPORT_FROM              8 (fix_bytearray_param)
+                54 STORE_NAME               8 (fix_bytearray_param)
+                56 IMPORT_FROM              9 (postgres_transforms)
+                58 STORE_NAME               9 (postgres_transforms)
+                60 IMPORT_FROM             10 (prep_query)
+                62 STORE_NAME              10 (prep_query)
+                64 IMPORT_FROM             11 (single_quoted_param_left_placeholder)
+                66 STORE_NAME              11 (single_quoted_param_left_placeholder)
+                68 IMPORT_FROM             12 (single_quoted_param_right_placeholder)
+                70 STORE_NAME              12 (single_quoted_param_right_placeholder)
+                72 IMPORT_FROM             13 (spark_transforms)
+                74 STORE_NAME              13 (spark_transforms)
+                76 POP_TOP
    
-     7          42 LOAD_CONST               0 (0)
-                44 LOAD_CONST               4 (('add_warnings_and_banner', 'double_quoted_param_left_placeholder', 'double_quoted_param_right_placeholder', 'fix_bytearray_lower', 'fix_bytearray_param', 'prep_query', 'single_quoted_param_left_placeholder', 'single_quoted_param_right_placeholder', 'sqlglot_postgres_transforms', 'sqlglot_spark_transforms'))
-                46 IMPORT_NAME              5 (dune.translate.helpers)
-                48 IMPORT_FROM              6 (add_warnings_and_banner)
-                50 STORE_NAME               6 (add_warnings_and_banner)
-                52 IMPORT_FROM              7 (double_quoted_param_left_placeholder)
-                54 STORE_NAME               7 (double_quoted_param_left_placeholder)
-                56 IMPORT_FROM              8 (double_quoted_param_right_placeholder)
-                58 STORE_NAME               8 (double_quoted_param_right_placeholder)
-                60 IMPORT_FROM              9 (fix_bytearray_lower)
-                62 STORE_NAME               9 (fix_bytearray_lower)
-                64 IMPORT_FROM             10 (fix_bytearray_param)
-                66 STORE_NAME              10 (fix_bytearray_param)
-                68 IMPORT_FROM             11 (prep_query)
-                70 STORE_NAME              11 (prep_query)
-                72 IMPORT_FROM             12 (single_quoted_param_left_placeholder)
-                74 STORE_NAME              12 (single_quoted_param_left_placeholder)
-                76 IMPORT_FROM             13 (single_quoted_param_right_placeholder)
-                78 STORE_NAME              13 (single_quoted_param_right_placeholder)
-                80 IMPORT_FROM             14 (sqlglot_postgres_transforms)
-                82 STORE_NAME              14 (sqlglot_postgres_transforms)
-                84 IMPORT_FROM             15 (sqlglot_spark_transforms)
-                86 STORE_NAME              15 (sqlglot_spark_transforms)
+    18          78 LOAD_CONST               0 (0)
+                80 LOAD_CONST               4 (('DuneTranslationError',))
+                82 IMPORT_NAME             14 (dune.translate.errors)
+                84 IMPORT_FROM             15 (DuneTranslationError)
+                86 STORE_NAME              15 (DuneTranslationError)
                 88 POP_TOP
    
     21          90 LOAD_CONST               5 (<code object _clean_dataset, file "/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/translate.py", line 21>)
                 92 MAKE_FUNCTION            0
                 94 STORE_NAME              16 (_clean_dataset)
    
     28          96 LOAD_CONST               7 ((None,))
@@ -72,16 +72,16 @@
                102 STORE_NAME              17 (_translate_query)
                104 LOAD_CONST               1 (None)
                106 RETURN_VALUE
    consts
       0
       None
       ('ParseError',)
+      ('add_warnings_and_banner', 'double_quoted_param_left_placeholder', 'double_quoted_param_right_placeholder', 'fix_bytearray_lower', 'fix_bytearray_param', 'postgres_transforms', 'prep_query', 'single_quoted_param_left_placeholder', 'single_quoted_param_right_placeholder', 'spark_transforms')
       ('DuneTranslationError',)
-      ('add_warnings_and_banner', 'double_quoted_param_left_placeholder', 'double_quoted_param_right_placeholder', 'fix_bytearray_lower', 'fix_bytearray_param', 'prep_query', 'single_quoted_param_left_placeholder', 'single_quoted_param_right_placeholder', 'sqlglot_postgres_transforms', 'sqlglot_spark_transforms')
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 4
          flags     : 3
          code
             0x9700640144005d1c7d017c017c00a00000000000000000000000000000
@@ -209,15 +209,15 @@
                      196 STORE_FAST               0 (query)
          
           41         198 LOAD_FAST                1 (sqlglot_dialect)
                      200 LOAD_CONST               7 ('spark')
                      202 COMPARE_OP               2 (==)
                      208 POP_JUMP_FORWARD_IF_FALSE    16 (to 242)
          
-          42         210 LOAD_GLOBAL             13 (NULL + sqlglot_spark_transforms)
+          42         210 LOAD_GLOBAL             13 (NULL + spark_transforms)
                      222 LOAD_FAST                0 (query)
                      224 PRECALL                  1
                      228 CALL                     1
                      238 STORE_FAST               3 (query_tree)
                      240 JUMP_FORWARD            44 (to 330)
          
           43     >>  242 LOAD_FAST                1 (sqlglot_dialect)
@@ -229,15 +229,15 @@
                      256 LOAD_METHOD              0 (replace)
                      278 LOAD_CONST               9 ('\\x')
                      280 LOAD_CONST              10 ('0x')
                      282 PRECALL                  2
                      286 CALL                     2
                      296 STORE_FAST               0 (query)
          
-          46         298 LOAD_GLOBAL             15 (NULL + sqlglot_postgres_transforms)
+          46         298 LOAD_GLOBAL             15 (NULL + postgres_transforms)
                      310 LOAD_FAST                0 (query)
                      312 LOAD_FAST                2 (dataset)
                      314 PRECALL                  2
                      318 CALL                     2
                      328 STORE_FAST               3 (query_tree)
          
           49     >>  330 LOAD_FAST                3 (query_tree)
@@ -378,27 +378,27 @@
             ('dialect', 'pretty')
             '\x1b[4m'
             ''
             '\x1b[0m'
             '. Line [0-9]+, Col: [0-9]+.'
             '.'
             None
-         names      ('replace', 'double_quoted_param_left_placeholder', 'double_quoted_param_right_placeholder', 'prep_query', 'sqlglot', 'transpile', 'sqlglot_spark_transforms', 'sqlglot_postgres_transforms', 'sql', 'single_quoted_param_left_placeholder', 'single_quoted_param_right_placeholder', 'fix_bytearray_param', 'fix_bytearray_lower', 'add_warnings_and_banner', 'ParseError', 'str', 're', 'sub', 'DuneTranslationError')
+         names      ('replace', 'double_quoted_param_left_placeholder', 'double_quoted_param_right_placeholder', 'prep_query', 'sqlglot', 'transpile', 'spark_transforms', 'postgres_transforms', 'sql', 'single_quoted_param_left_placeholder', 'single_quoted_param_right_placeholder', 'fix_bytearray_param', 'fix_bytearray_lower', 'add_warnings_and_banner', 'ParseError', 'str', 're', 'sub', 'DuneTranslationError')
          varnames   ('query', 'sqlglot_dialect', 'dataset', 'query_tree', 'e', 'error_message')
          freevars   ()
          cellvars   ()
          filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/translate.py'
          name       '_translate_query'
          firstlineno 28
          lnotab
             0x020202024a010eff10031e033c030c0120010c022c0120032e04340132
             01320132fc02081e011e02200212051c0128012801320132fb0208160102
             01020102fd100526ef
       (None,)
-   names      ('re', 'sqlglot', 'ParseError', 'dune.translate.errors', 'DuneTranslationError', 'dune.translate.helpers', 'add_warnings_and_banner', 'double_quoted_param_left_placeholder', 'double_quoted_param_right_placeholder', 'fix_bytearray_lower', 'fix_bytearray_param', 'prep_query', 'single_quoted_param_left_placeholder', 'single_quoted_param_right_placeholder', 'sqlglot_postgres_transforms', 'sqlglot_spark_transforms', '_clean_dataset', '_translate_query')
+   names      ('re', 'sqlglot', 'ParseError', 'dune.translate.custom_transforms', 'add_warnings_and_banner', 'double_quoted_param_left_placeholder', 'double_quoted_param_right_placeholder', 'fix_bytearray_lower', 'fix_bytearray_param', 'postgres_transforms', 'prep_query', 'single_quoted_param_left_placeholder', 'single_quoted_param_right_placeholder', 'spark_transforms', 'dune.translate.errors', 'DuneTranslationError', '_clean_dataset', '_translate_query')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/runner/work/dune-query-translator/dune-query-translator/dune/translate/translate.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff0201080208010c020c01300e0607
+   lnotab 0x00ff0201080208010c02300c0c030607
```

### Comparing `dune_query_translator-0.3.1/dune/translate/helpers.py` & `dune_query_translator-0.4.0/dune/translate/custom_transforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,16 @@
         elif char == ")":
             if len(stack) > 1:
                 stack.pop()  # if a ")" is found but stack is greater than 1, we're still in a nested select
             else:  # if stack is 1, we're at the end of the nested select
                 end = i + 1
                 substring = text[stack[0] : end].strip()
                 stack = []  # reset the stack after an end is found
-                if re.search(r"^\(\s*select\b", substring, re.IGNORECASE):  # if substring starts with "(select " then
+                # if substring starts with "(select "
+                if re.search(r"^\(\s*select\b", substring, re.IGNORECASE):
                     results.append(substring)
     return results
 
 
 def recurse_where(node, required_tables, condition_add):
     """
     we can't just iterate through the tree because of weird replace node behaviors, so this iterates
@@ -109,17 +110,14 @@
         # remove the outer parens so it isn't caught in infinite single recursion
         parsed_group = recurse_where(group[1:-1], required_tables, condition_add)
         statement = statement.replace(f"{placeholder}{i}__)", "(" + parsed_group + ")")
 
     return statement
 
 
-# SQLGlot functions
-
-
 def chain_where_blockchain(node, blockchain):
     # add a blockchain = 'ethereum' to the WHERE statement for trades, tokens, and prices tables.
     required_tables = [
         "nft.trades",
         "dex.in.trades",
         "tokens.erc20",
         "tokens.nft",
@@ -138,14 +136,15 @@
 chain_where_gnosis = partial(chain_where_blockchain, blockchain="gnosis")
 chain_where_optimism = partial(chain_where_blockchain, blockchain="optimism")
 chain_where_bnb = partial(chain_where_blockchain, blockchain="bnb")
 chain_where_polygon = partial(chain_where_blockchain, blockchain="polygon")
 
 
 def dex_trades_fixes(node):
+    """Fixes to dex.trades"""
     # doesn't matter if subquery or not, it will replace the found filter.
     if node.key == "select":
         if "dex.in.trades" in node.sql(dialect="trino").replace('"', ""):
             # change exchange_contract_address to project_contract_address
             final_where = node.sql(dialect="trino").replace("exchange_contract_address", "project_contract_address")
 
             # removing category from WHERE statement since that isn't in dex.in.trades anymore
@@ -188,15 +187,15 @@
 param_right_placeholder = "parameter_placeholder_right_bracket"
 double_quoted_param_left_placeholder = f'"{param_left_placeholder}'
 double_quoted_param_right_placeholder = f'{param_right_placeholder}"'
 single_quoted_param_left_placeholder = f"'{param_left_placeholder}"
 single_quoted_param_right_placeholder = f"{param_right_placeholder}'"
 
 
-# TODO: Remove this once https://github.com/tobymao/sqlglot/issues/1410 is fixed
+# TODO: Remove or simplify once the fix to https://github.com/tobymao/sqlglot/issues/1410 is released
 def interval_fix(node):
     """Handle interval syntax change from Spark to Trino"""
     if node.key == "interval":
         # node.this is the argument to the interval function, possibly a parenthesized expression
         interval_argument = str(node.this)
         if interval_argument[0] == "(" and interval_argument[-1] == ")":
             interval_argument = interval_argument[1:-1]
@@ -204,29 +203,31 @@
         regex_split = re.split(r'[\'"]', interval_argument)
         # remove empty elements (will occur if there are quotes inside the interval value)
         # matches start at index 1, index 0 is the original string
         regex_matches = [i for i in regex_split[1:] if i != ""]
         # no match, return
         if len(regex_matches) == 0:
             return node
-        identifier = " ".join(regex_matches)
-        value, granularity, *rest = identifier.split()
+        interval_argument = " ".join(regex_matches)
+        if len(interval_argument.split()) == 1:
+            return node
+        value, granularity, *rest = interval_argument.split()
         if any(
             known_granularity in granularity.lower()
             for known_granularity in [
                 "second",
                 "minute",
                 "hour",
                 "day",
                 "week",
                 "month",
                 "year",
             ]
         ):
-            if granularity[-1] == "s":
+            if granularity.endswith("s"):
                 granularity = granularity[:-1]
             if granularity == "week":  # we don't have week in Trino SQL
                 value = int(value) * 7
                 granularity = "day"
                 rest.append("--week doesn't work in DuneSQL\n")
             final_interval = (
                 ("INTERVAL '" + str(value) + "' " + granularity + " ".join(rest))
@@ -238,20 +239,20 @@
 
 
 def bytearray_parameter_fix(node):
     """Take care of parameters that use bytearrays"""
     if node.key == "eq":
         if all(
             a_param in node.sql(dialect="trino").lower()
-            for a_param in [
+            for a_param in (
                 "0x",
                 "substring(",
                 double_quoted_param_left_placeholder,
                 double_quoted_param_right_placeholder,
-            ]
+            )
         ):
             # include param_left variables in regex pattern
             pattern = (
                 r".*SUBSTRING\(\s*['\"]"
                 + re.escape(double_quoted_param_left_placeholder)
                 + r"(.*?)"
                 + re.escape(double_quoted_param_right_placeholder)
@@ -264,15 +265,15 @@
     return node
 
 
 def cast_numeric(node):
     """if a column is being added, subtracted, multiplied, divided, etc,
     and it has amount/value in the name, cast to double"""
     if node.key == "column":
-        if any(val in node.name.lower() for val in ["amount", "value"]):
+        if any(val in node.name.lower() for val in ("amount", "value")):
             return sqlglot.parse_one("cast(" + node.name + " as double)", read="trino")
     return node
 
 
 def cast_timestamp(node):
     if node.key == "literal":
         # and contains 'yyyy-mm-dd' format then cast to timestamp
@@ -290,15 +291,15 @@
             return sqlglot.parse_one("timestamp '{{" + match.group(1) + "}}'", read="trino")
     return node
 
 
 def fix_boolean(node):
     """If node.key is 'literal' and contains 'true' or 'false' then cast to boolean"""
     if node.key == "literal":
-        if any(boolean in node.sql(dialect="trino").lower() for boolean in ["true", "false"]):
+        if any(boolean in node.sql(dialect="trino").lower() for boolean in ("true", "false")):
             # remove single or double quotes
             bool_cleaned = node.sql(dialect="trino").replace('"', "").replace("'", "")
             return sqlglot.parse_one(bool_cleaned, read="trino")
     return node
 
 
 def warn_unnest(node):
@@ -381,15 +382,15 @@
         "optimism": chain_where_optimism,
         "bnb": chain_where_bnb,
         "polygon": chain_where_polygon,
         "ethereum": chain_where_ethereum,
     }[dataset]
 
 
-def sqlglot_postgres_transforms(query, dataset):
+def postgres_transforms(query, dataset):
     """Apply a series of transforms to the query tree, recursively using SQLGlot's recursive transform function.
 
     Each transform takes and returns a sqlglot.Expression"""
     query_tree = sqlglot.parse_one(query, read="postgres")
     transforms = (
         postgres_table_replacements(dataset),
         interval_fix,
@@ -405,19 +406,19 @@
         bytea2numeric,
     )
     for f in transforms:
         query_tree = query_tree.transform(f)
     return query_tree
 
 
-def sqlglot_spark_transforms(query):
+def spark_transforms(query):
     """Apply a series of transforms to the query tree, recursively using SQLGlot's recursive transform function.
 
     Each transform takes and returns a sqlglot.Expression"""
-    query_tree = sqlglot.parse_one(query, read="spark")
+    query_tree = sqlglot.parse_one(query, read="trino")
     transforms = (
         interval_fix,
         fix_boolean,
         cast_numeric,
         cast_timestamp,
         warn_unnest,
         warn_sequence,
```

### Comparing `dune_query_translator-0.3.1/dune/translate/table_replacements.py` & `dune_query_translator-0.4.0/dune/translate/table_replacements.py`

 * *Files identical despite different names*

### Comparing `dune_query_translator-0.3.1/dune/translate/translate.py` & `dune_query_translator-0.4.0/dune/translate/translate.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import re
 
 import sqlglot
 from sqlglot import ParseError
 
-from dune.translate.errors import DuneTranslationError
-from dune.translate.helpers import (
+from dune.translate.custom_transforms import (
     add_warnings_and_banner,
     double_quoted_param_left_placeholder,
     double_quoted_param_right_placeholder,
     fix_bytearray_lower,
     fix_bytearray_param,
+    postgres_transforms,
     prep_query,
     single_quoted_param_left_placeholder,
     single_quoted_param_right_placeholder,
-    sqlglot_postgres_transforms,
-    sqlglot_spark_transforms,
+    spark_transforms,
 )
+from dune.translate.errors import DuneTranslationError
 
 
 def _clean_dataset(dataset):
     for d in ("gnosis", "optimism", "bnb", "polygon", "ethereum"):
         if d in dataset.lower():
             return d
     raise ValueError(f"Unknown dataset: {dataset}")
@@ -35,19 +35,19 @@
         query = prep_query(query)
 
         # Transpile to Trino
         query = sqlglot.transpile(query, read=sqlglot_dialect, write="trino", pretty=True)[0]
 
         # Perform custom transformations using SQLGlot's parsed representation
         if sqlglot_dialect == "spark":
-            query_tree = sqlglot_spark_transforms(query)
+            query_tree = spark_transforms(query)
         elif sqlglot_dialect == "postgres":
             # Update bytearray syntax
             query = query.replace("\\x", "0x")
-            query_tree = sqlglot_postgres_transforms(query, dataset)
+            query_tree = postgres_transforms(query, dataset)
 
         # Turn back to SQL
         query = query_tree.sql(dialect="trino", pretty=True)
 
         # Replace placeholders with Dune params again
         query = (
             query.replace(double_quoted_param_left_placeholder, "{{")
```

### Comparing `dune_query_translator-0.3.1/pyproject.toml` & `dune_query_translator-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dune-query-translator"
-version = "0.3.1"
+version = "0.4.0"
 description = ""
 authors = ["Vegard Stikbakke <vegard@dune.com>"]
 readme = "README.md"
 packages = [{include = "dune"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `dune_query_translator-0.3.1/PKG-INFO` & `dune_query_translator-0.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dune-query-translator
-Version: 0.3.1
+Version: 0.4.0
 Summary: 
 Author: Vegard Stikbakke
 Author-email: vegard@dune.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: sqlglot (>=11.4.4,<12.0.0)
```

