# Comparing `tmp/mo_streams-1.368.23092-py2.py3-none-any.whl.zip` & `tmp/mo_streams-1.370.23104-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 23336 bytes, number of entries: 15
+Zip file size: 23366 bytes, number of entries: 15
 -rw-rw-rw-  2.0 fat     2894 b- defN 23-Apr-02 14:04 mo_streams/__init__.py
 -rw-rw-rw-  2.0 fat     3553 b- defN 23-Mar-11 19:14 mo_streams/_utils.py
 -rw-rw-rw-  2.0 fat     3864 b- defN 23-Apr-02 14:04 mo_streams/byte_stream.py
 -rw-rw-rw-  2.0 fat     1158 b- defN 23-Apr-02 14:04 mo_streams/empty_stream.py
 -rw-rw-rw-  2.0 fat     1644 b- defN 22-Dec-28 02:30 mo_streams/files.py
--rw-rw-rw-  2.0 fat    13340 b- defN 23-Apr-02 14:04 mo_streams/function_factory.py
+-rw-rw-rw-  2.0 fat    13868 b- defN 23-Apr-14 10:37 mo_streams/function_factory.py
 -rw-rw-rw-  2.0 fat    10850 b- defN 23-Apr-02 14:04 mo_streams/object_stream.py
 -rw-rw-rw-  2.0 fat     1724 b- defN 23-Apr-02 14:04 mo_streams/string_stream.py
 -rw-rw-rw-  2.0 fat      881 b- defN 23-Apr-02 14:04 mo_streams/type_parser.py
--rw-rw-rw-  2.0 fat     6662 b- defN 23-Apr-02 14:04 mo_streams/type_utils.py
--rw-rw-rw-  2.0 fat    17098 b- defN 23-Apr-02 14:04 mo_streams-1.368.23092.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     4145 b- defN 23-Apr-02 14:04 mo_streams-1.368.23092.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Apr-02 14:04 mo_streams-1.368.23092.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Apr-02 14:04 mo_streams-1.368.23092.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1249 b- defN 23-Apr-02 14:04 mo_streams-1.368.23092.dist-info/RECORD
-15 files, 69183 bytes uncompressed, 21276 bytes compressed:  69.2%
+-rw-rw-rw-  2.0 fat     6663 b- defN 23-Apr-14 10:37 mo_streams/type_utils.py
+-rw-rw-rw-  2.0 fat    17098 b- defN 23-Apr-14 10:37 mo_streams-1.370.23104.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     4145 b- defN 23-Apr-14 10:37 mo_streams-1.370.23104.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Apr-14 10:37 mo_streams-1.370.23104.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Apr-14 10:37 mo_streams-1.370.23104.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1249 b- defN 23-Apr-14 10:37 mo_streams-1.370.23104.dist-info/RECORD
+15 files, 69712 bytes uncompressed, 21306 bytes compressed:  69.4%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: mo_streams/type_parser.py
 Comment: 
 
 Filename: mo_streams/type_utils.py
 Comment: 
 
-Filename: mo_streams-1.368.23092.dist-info/LICENSE
+Filename: mo_streams-1.370.23104.dist-info/LICENSE
 Comment: 
 
-Filename: mo_streams-1.368.23092.dist-info/METADATA
+Filename: mo_streams-1.370.23104.dist-info/METADATA
 Comment: 
 
-Filename: mo_streams-1.368.23092.dist-info/WHEEL
+Filename: mo_streams-1.370.23104.dist-info/WHEEL
 Comment: 
 
-Filename: mo_streams-1.368.23092.dist-info/top_level.txt
+Filename: mo_streams-1.370.23104.dist-info/top_level.txt
 Comment: 
 
-Filename: mo_streams-1.368.23092.dist-info/RECORD
+Filename: mo_streams-1.370.23104.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mo_streams/function_factory.py

```diff
@@ -157,14 +157,29 @@
                     return None
                 return sv / ov
 
             return BuiltFunction(func, Typer(python_type=float), domain_schema)
 
         return FunctionFactory(builder, Typer(python_type=float), f"{other} / {self}")
 
+    def __rsub__(self, other):
+        func_other = factory(other)
+
+        def builder(domain_type, domain_schema) -> BuiltFunction:
+            sf, st, ss = self.build(domain_type, domain_schema)
+            of, ot, os = func_other.build(domain_type, domain_schema)
+
+            def func(v, a):
+                return of(v, a) - sf(v, a)
+
+            return BuiltFunction(func, st, domain_schema)
+
+        type_ = Typer(example=other) + _get(self, "typer")
+        return FunctionFactory(builder, type_, f"{other} - {self}")
+
     def __radd__(self, other):
         func_other = factory(other)
 
         def builder(domain_type, domain_schema) -> BuiltFunction:
             sf, st, ss = self.build(domain_type, domain_schema)
             of, ot, os = func_other.build(domain_type, domain_schema)
```

## mo_streams/type_utils.py

```diff
@@ -18,14 +18,15 @@
 
 
 class Typer:
     """
     Smooth out the lumps of Python type manipulation
     """
 
+
     def __init__(self, *, example=None, python_type=None, function=None):
         if function:
             # find function return type
             inspect.signature(function)
         elif example:
             self.python_type = type(example)
         elif python_type is LazyTyper:
```

## Comparing `mo_streams-1.368.23092.dist-info/LICENSE` & `mo_streams-1.370.23104.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mo_streams-1.368.23092.dist-info/METADATA` & `mo_streams-1.370.23104.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-streams
-Version: 1.368.23092
+Version: 1.370.23104
 Summary: More Streams! Chained function calls
 Home-page: https://github.com/klahnakoski/mo-streams
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Software Development :: Libraries
@@ -12,17 +12,17 @@
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mo-dots (==9.368.23092)
-Requires-Dist: mo-files (==6.368.23092)
+Requires-Dist: mo-files (==6.370.23104)
 Requires-Dist: mo-future (==7.340.23006)
-Requires-Dist: mo-json (==6.368.23092)
+Requires-Dist: mo-json (==6.370.23104)
 Provides-Extra: tests
 Requires-Dist: mo-files ; extra == 'tests'
 Requires-Dist: mo-logs ; extra == 'tests'
 Requires-Dist: zstandard ; extra == 'tests'
 Requires-Dist: boto3 ; extra == 'tests'
 Requires-Dist: moto ; extra == 'tests'
 Requires-Dist: pandas ; extra == 'tests'
```

## Comparing `mo_streams-1.368.23092.dist-info/RECORD` & `mo_streams-1.370.23104.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 mo_streams/__init__.py,sha256=Q18XCBhxiBflZH0cQBiqxrcuEt4ER8XPh_I8kowpkz0,2894
 mo_streams/_utils.py,sha256=WvhpnHgHr45mPxGC5Q3yt7GsPqBpe529YAwhEACF_QE,3553
 mo_streams/byte_stream.py,sha256=9ckKk-0eJkjpP-jdnJiobcydapAYz8hfgyJ8Mb0P0b8,3864
 mo_streams/empty_stream.py,sha256=sMEbfKjgoF2aAuWaEN1nWq7ds4DIqvQnU5awF1EfH_4,1158
 mo_streams/files.py,sha256=UMdhrjIFnmSDko5TiJQ9Ki7N5iv5u9eIR4Dllk1o30w,1644
-mo_streams/function_factory.py,sha256=3jrAbcC4M0qtBdyHcSL7vqJRUQB6uhhTYca3DKuVLns,13340
+mo_streams/function_factory.py,sha256=rVoWs0PhVQN-4WyXvN8U1YaFVmuiFDw7brzNhEG8e-Y,13868
 mo_streams/object_stream.py,sha256=SAt4KVNpM-ERG5lMtqLJbtuLOS6dHuktRUqO-9sBy-M,10850
 mo_streams/string_stream.py,sha256=HmYphG_kz2zKcdNxXb9fmGOcy4kkvMRtSilFPNe-08w,1724
 mo_streams/type_parser.py,sha256=GGkWvHYkuZK_cuFCCbITirDLEF6IYVnX8Ye7Nr7FfAk,881
-mo_streams/type_utils.py,sha256=wBIkF67A-UxZ4ytxbMP-pPO-onPaN6OrFX91CecZnLY,6662
-mo_streams-1.368.23092.dist-info/LICENSE,sha256=JoTeFzAOCkNGhvHsf4r2BFIHpLRXo_4EsrnOZV58XVA,17098
-mo_streams-1.368.23092.dist-info/METADATA,sha256=WEYVPhpmaZrTb1G93IbZ3weTEVI-Hs2fGmG12Paj7Ww,4145
-mo_streams-1.368.23092.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-mo_streams-1.368.23092.dist-info/top_level.txt,sha256=ebi1P9VRtYjLlesoDmWVYQGcYY1ky8AZHO4PbPBZ3o8,11
-mo_streams-1.368.23092.dist-info/RECORD,,
+mo_streams/type_utils.py,sha256=DDUvT2cgsp5xdBgeKQzzfPK0udC-zH-DAz8XWyymGxs,6663
+mo_streams-1.370.23104.dist-info/LICENSE,sha256=JoTeFzAOCkNGhvHsf4r2BFIHpLRXo_4EsrnOZV58XVA,17098
+mo_streams-1.370.23104.dist-info/METADATA,sha256=7z0TQG7F82xWsJUrwUq5goRLZ0pZGMrynREMmEifwU4,4145
+mo_streams-1.370.23104.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+mo_streams-1.370.23104.dist-info/top_level.txt,sha256=ebi1P9VRtYjLlesoDmWVYQGcYY1ky8AZHO4PbPBZ3o8,11
+mo_streams-1.370.23104.dist-info/RECORD,,
```

