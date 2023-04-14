# Comparing `tmp/Huggy_qmk-0.0.1-py3-none-any.whl.zip` & `tmp/Huggy_qmk-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
 Zip file size: 1442 bytes, number of entries: 5
--rw-r--r--  2.0 unx      165 b- defN 23-Apr-11 04:04 query_making/query_mk.py
--rw-r--r--  2.0 unx      368 b- defN 23-Apr-11 04:12 Huggy_qmk-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-11 04:12 Huggy_qmk-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 23-Apr-11 04:12 Huggy_qmk-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      385 b- defN 23-Apr-11 04:12 Huggy_qmk-0.0.1.dist-info/RECORD
+-rw-r--r--  2.0 unx      165 b- defN 23-Apr-14 06:11 query_making/query_mk.py
+-rw-r--r--  2.0 unx      368 b- defN 23-Apr-14 06:13 Huggy_qmk-0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-14 06:13 Huggy_qmk-0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 23-Apr-14 06:13 Huggy_qmk-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      385 b- defN 23-Apr-14 06:13 Huggy_qmk-0.0.2.dist-info/RECORD
 5 files, 1023 bytes uncompressed, 720 bytes compressed:  29.6%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: query_making/query_mk.py
 Comment: 
 
-Filename: Huggy_qmk-0.0.1.dist-info/METADATA
+Filename: Huggy_qmk-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: Huggy_qmk-0.0.1.dist-info/WHEEL
+Filename: Huggy_qmk-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: Huggy_qmk-0.0.1.dist-info/top_level.txt
+Filename: Huggy_qmk-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: Huggy_qmk-0.0.1.dist-info/RECORD
+Filename: Huggy_qmk-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## query_making/query_mk.py

```diff
@@ -1,4 +1,4 @@
 def qcreate(db_name):
   return "Create database {}".format(db_name)
 def qread(table_name,filed_name="*"):
-  return "Select {} from {}".foramt(table_name,filed_name)
+  return "Select {} from {}".format(table_name,filed_name)
```

