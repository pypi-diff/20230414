# Comparing `tmp/txt2tei-1.0.6.post1-py3-none-any.whl.zip` & `tmp/txt2tei-1.0.6.post2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 39358 bytes, number of entries: 17
+Zip file size: 39367 bytes, number of entries: 17
 -rw-r--r--  2.0 unx       23 b- defN 23-Jan-31 12:10 txt2tei/__init__.py
 -rw-r--r--  2.0 unx      893 b- defN 23-Mar-09 15:42 txt2tei/addmetre.py
 -rw-r--r--  2.0 unx     2457 b- defN 22-Apr-08 21:20 txt2tei/authors.py
 -rw-r--r--  2.0 unx     1422 b- defN 22-Apr-08 21:31 txt2tei/authors.xml
 -rw-r--r--  2.0 unx      715 b- defN 23-Jan-31 09:11 txt2tei/edition.py
 -rw-r--r--  2.0 unx    14360 b- defN 23-Mar-16 13:38 txt2tei/libtxt2tei.py
 -rw-r--r--  2.0 unx     1910 b- defN 23-Jan-31 12:06 txt2tei/makelist.py
 -rw-r--r--  2.0 unx    12011 b- defN 22-Feb-02 16:16 txt2tei/sexos.csv
 -rw-r--r--  2.0 unx     4175 b- defN 23-Jan-30 14:00 txt2tei/tei2txt.py
 -rw-r--r--  2.0 unx    16599 b- defN 23-Jan-31 12:06 txt2tei/txt2tei-a.py
--rw-r--r--  2.0 unx    20920 b- defN 23-Apr-11 06:30 txt2tei/txt2tei.py
--rw-r--r--  2.0 unx    35149 b- defN 23-Apr-14 09:03 txt2tei-1.0.6.post1.dist-info/LICENSE
--rw-r--r--  2.0 unx     5521 b- defN 23-Apr-14 09:03 txt2tei-1.0.6.post1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-14 09:03 txt2tei-1.0.6.post1.dist-info/WHEEL
--rw-r--r--  2.0 unx       41 b- defN 23-Apr-14 09:03 txt2tei-1.0.6.post1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 23-Apr-14 09:03 txt2tei-1.0.6.post1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1350 b- defN 23-Apr-14 09:03 txt2tei-1.0.6.post1.dist-info/RECORD
-17 files, 117646 bytes uncompressed, 37162 bytes compressed:  68.4%
+-rw-r--r--  2.0 unx    20919 b- defN 23-Apr-14 09:08 txt2tei/txt2tei.py
+-rw-r--r--  2.0 unx    35149 b- defN 23-Apr-14 09:41 txt2tei-1.0.6.post2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5547 b- defN 23-Apr-14 09:41 txt2tei-1.0.6.post2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-14 09:41 txt2tei-1.0.6.post2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       41 b- defN 23-Apr-14 09:41 txt2tei-1.0.6.post2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-Apr-14 09:41 txt2tei-1.0.6.post2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1350 b- defN 23-Apr-14 09:41 txt2tei-1.0.6.post2.dist-info/RECORD
+17 files, 117671 bytes uncompressed, 37171 bytes compressed:  68.4%
```

## zipnote {}

```diff
@@ -27,26 +27,26 @@
 
 Filename: txt2tei/txt2tei-a.py
 Comment: 
 
 Filename: txt2tei/txt2tei.py
 Comment: 
 
-Filename: txt2tei-1.0.6.post1.dist-info/LICENSE
+Filename: txt2tei-1.0.6.post2.dist-info/LICENSE
 Comment: 
 
-Filename: txt2tei-1.0.6.post1.dist-info/METADATA
+Filename: txt2tei-1.0.6.post2.dist-info/METADATA
 Comment: 
 
-Filename: txt2tei-1.0.6.post1.dist-info/WHEEL
+Filename: txt2tei-1.0.6.post2.dist-info/WHEEL
 Comment: 
 
-Filename: txt2tei-1.0.6.post1.dist-info/entry_points.txt
+Filename: txt2tei-1.0.6.post2.dist-info/entry_points.txt
 Comment: 
 
-Filename: txt2tei-1.0.6.post1.dist-info/top_level.txt
+Filename: txt2tei-1.0.6.post2.dist-info/top_level.txt
 Comment: 
 
-Filename: txt2tei-1.0.6.post1.dist-info/RECORD
+Filename: txt2tei-1.0.6.post2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## txt2tei/txt2tei.py

```diff
@@ -477,15 +477,15 @@
     return encoding
 
 
 def main(input_arguments=sys.argv):
     input_file = input_arguments[1]
     output = f'{input_file.rsplit(".", 1)[0]}.xml'
     enc = unixfy(input_file)
-    with open(input_file, 'rU', encoding=enc) as f:
+    with open(input_file, 'r', encoding=enc) as f:
         characters_list = find_characters(f)
         f.seek(0)
         lines = f.readlines()
     author = date = title = n = sp = ''
     for line in lines:
         if line.startswith('<'):
             label = re.search(r'^\s*<(\w*)>', line.strip()).group(1)
```

## Comparing `txt2tei-1.0.6.post1.dist-info/LICENSE` & `txt2tei-1.0.6.post2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `txt2tei-1.0.6.post1.dist-info/METADATA` & `txt2tei-1.0.6.post2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: txt2tei
-Version: 1.0.6.post1
+Version: 1.0.6.post2
 Summary: An aid to encoding plays as XML-TEI
 Home-page: https://github.com/fsanzl/txt2tei
 Author: Fernando Sanz-Lázaro
 Author-email: fsanzl@gmail.com
 License: LGPL
 Project-URL: Source, https://github.com/fsanzl/txt2tei/
 Project-URL: Tracker, https://github.com/fsanzl/txt2tei/issues
@@ -138,17 +138,19 @@
 
 ## Contributions
 
 Feel free to contribute using the [GitHub Issue Tracker](https://github.com/fsanzl/txt2tei/issues) for feedback, suggestions, or bug reports.
 
 ## Changelog
 
-### 1.0.6-1
+
+### 1.0.6-2
 
 - Added chardet to dependencies
+- Solved deprecated 'rU'
 
 ### 1.0.6
 
 - Solved empty date crash. 
 - Handling BOM and Hasefroch line terminators
 - Changelog markdown syntax
```

## Comparing `txt2tei-1.0.6.post1.dist-info/RECORD` & `txt2tei-1.0.6.post2.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -4,14 +4,14 @@
 txt2tei/authors.xml,sha256=mZ9uCw-rkD7bO7Tq2sX9Wsz-F4wAB1bDjC5JWyiJOJ4,1422
 txt2tei/edition.py,sha256=FyfWw32iOOLxGU5ukedLy94u0ZgTFAoDEG2MB9RqWaw,715
 txt2tei/libtxt2tei.py,sha256=DJ4owqD0hF-W08Wwsghhh2nzo_RpABISrFbUvLzME3A,14360
 txt2tei/makelist.py,sha256=V87nklsu0em-sBras7ZxBaFhZlzFrXw5mmTM4-cSgaw,1910
 txt2tei/sexos.csv,sha256=lnITdEOuZimUEKKtCr2L_Jw2YsFbamWE7j6JDyyjA9E,12011
 txt2tei/tei2txt.py,sha256=lbSxOTrcB5kAr3VTwYEtI1uDl4w1UHyTNogvnzKUc0o,4175
 txt2tei/txt2tei-a.py,sha256=A3mMrGgdWCqQgxdd_aQxb83mQ5y5N01S8iCSUlVqD3s,16599
-txt2tei/txt2tei.py,sha256=WNNTGhbOjgwKgDyYzAT45sY36U6IvHT-1ODNEacdLE0,20920
-txt2tei-1.0.6.post1.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-txt2tei-1.0.6.post1.dist-info/METADATA,sha256=XcIBBaYVU9IexHK7aTrQP187ful77pcKIWa-2YpK9WU,5521
-txt2tei-1.0.6.post1.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-txt2tei-1.0.6.post1.dist-info/entry_points.txt,sha256=T05Iugv-A3ZSiNpNsI4qlKHsjFEUQGxFS6V-veVV2Rw,41
-txt2tei-1.0.6.post1.dist-info/top_level.txt,sha256=Kg9uQhLgw8ga_rs1i79lwxWAS4on0mxNXssSduxWpL4,8
-txt2tei-1.0.6.post1.dist-info/RECORD,,
+txt2tei/txt2tei.py,sha256=Co0iIbFJENI9UF2XQSGHnl1PMTCtLvuNMoTu9R2TB2Y,20919
+txt2tei-1.0.6.post2.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+txt2tei-1.0.6.post2.dist-info/METADATA,sha256=6qLOc1UyTQqaVCto1HWOUkq9ly5oKCZT8iHszzYAvKk,5547
+txt2tei-1.0.6.post2.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+txt2tei-1.0.6.post2.dist-info/entry_points.txt,sha256=T05Iugv-A3ZSiNpNsI4qlKHsjFEUQGxFS6V-veVV2Rw,41
+txt2tei-1.0.6.post2.dist-info/top_level.txt,sha256=Kg9uQhLgw8ga_rs1i79lwxWAS4on0mxNXssSduxWpL4,8
+txt2tei-1.0.6.post2.dist-info/RECORD,,
```

