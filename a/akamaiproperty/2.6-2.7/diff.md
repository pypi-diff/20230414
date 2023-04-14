# Comparing `tmp/akamaiproperty-2.6-py3-none-any.whl.zip` & `tmp/akamaiproperty-2.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 13852 bytes, number of entries: 8
+Zip file size: 13855 bytes, number of entries: 8
 -rw-r--r--  2.0 unx      108 b- defN 22-Jun-12 17:02 akamaiproperty/__init__.py
--rw-r--r--  2.0 unx    28603 b- defN 23-Apr-14 09:44 akamaiproperty/akamaiproperty.py
+-rw-r--r--  2.0 unx    28606 b- defN 23-Apr-14 09:55 akamaiproperty/akamaiproperty.py
 -rw-r--r--  2.0 unx     7127 b- defN 22-Jun-12 17:02 akamaiproperty/http_calls.py
--rwx------  2.0 unx    11357 b- defN 23-Apr-14 09:47 akamaiproperty-2.6.dist-info/LICENSE
--rw-r--r--  2.0 unx     2750 b- defN 23-Apr-14 09:47 akamaiproperty-2.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-14 09:47 akamaiproperty-2.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-Apr-14 09:47 akamaiproperty-2.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      669 b- defN 23-Apr-14 09:47 akamaiproperty-2.6.dist-info/RECORD
-8 files, 50721 bytes uncompressed, 12682 bytes compressed:  75.0%
+-rwx------  2.0 unx    11357 b- defN 23-Apr-14 09:55 akamaiproperty-2.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2750 b- defN 23-Apr-14 09:55 akamaiproperty-2.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-14 09:55 akamaiproperty-2.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-Apr-14 09:55 akamaiproperty-2.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      669 b- defN 23-Apr-14 09:55 akamaiproperty-2.7.dist-info/RECORD
+8 files, 50724 bytes uncompressed, 12685 bytes compressed:  75.0%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: akamaiproperty/akamaiproperty.py
 Comment: 
 
 Filename: akamaiproperty/http_calls.py
 Comment: 
 
-Filename: akamaiproperty-2.6.dist-info/LICENSE
+Filename: akamaiproperty-2.7.dist-info/LICENSE
 Comment: 
 
-Filename: akamaiproperty-2.6.dist-info/METADATA
+Filename: akamaiproperty-2.7.dist-info/METADATA
 Comment: 
 
-Filename: akamaiproperty-2.6.dist-info/WHEEL
+Filename: akamaiproperty-2.7.dist-info/WHEEL
 Comment: 
 
-Filename: akamaiproperty-2.6.dist-info/top_level.txt
+Filename: akamaiproperty-2.7.dist-info/top_level.txt
 Comment: 
 
-Filename: akamaiproperty-2.6.dist-info/RECORD
+Filename: akamaiproperty-2.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## akamaiproperty/akamaiproperty.py

```diff
@@ -404,22 +404,22 @@
             return []
         behaviorParsedList = self._getBehaviorParsedList(version)
         cpCodeList = []
         for behavior in behaviorParsedList:
             if behavior["behavior"]["name"] == 'cpCode':
                 cpCodeList.append(behavior["behavior"]["options"]['value']['id'])
         cpCodeList = list(dict.fromkeys(cpCodeList))
-        print(cpCodeList)
+        #print(cpCodeList)
         
         ruleTree = self.getRuleTree(int(version))
         cpCodeAdvancedList = self.extractCPCodes(ruleTree)
-        print(cpCodeAdvancedList)
+        #print(cpCodeAdvancedList)
         cpCodeList = cpCodeList + cpCodeAdvancedList
         cpCodeList = list(dict.fromkeys(cpCodeList))
-        print(cpCodeList)
+        #print(cpCodeList)
 
         return cpCodeList
 
     def getMappings(self,productId):
         prdMappingJson = {'prd_Adaptive_Media_Delivery': 'Adaptive Media Delivery',
             'prd_Obj_Delivery': 'Object Delivery',
             'prd_Download_Delivery': 'Download Delivery',
```

## Comparing `akamaiproperty-2.6.dist-info/LICENSE` & `akamaiproperty-2.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `akamaiproperty-2.6.dist-info/METADATA` & `akamaiproperty-2.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akamaiproperty
-Version: 2.6
+Version: 2.7
 Summary: A Pip Package for Akamai Property
 Home-page: https://github.com/Achuthananda/AkamaiPropertyManager
 Author: Achuthananda M P
 Author-email: achuthadivine@gmail.com
 Keywords: Akamai Property CDN AkamaiConfigs Edge
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `akamaiproperty-2.6.dist-info/RECORD` & `akamaiproperty-2.7.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 akamaiproperty/__init__.py,sha256=Pk0acNhv3PYXX7_BcWYe68ASjnpu29gCKUtCwpvbz7o,108
-akamaiproperty/akamaiproperty.py,sha256=vsfmo_dWyilhiM9k-DEZx3Z-eW68JGOESVsocOwz7tI,28603
+akamaiproperty/akamaiproperty.py,sha256=ZsgDusOmtEbe5YVBkMNddxnywkpa2sz9-TfCtYH-i5o,28606
 akamaiproperty/http_calls.py,sha256=lQj18BM77O0RUNN4Knv1RkVRE2R65dsOm_Yk_TnD6Ww,7127
-akamaiproperty-2.6.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-akamaiproperty-2.6.dist-info/METADATA,sha256=C1FNaFeyRd35ymsFDgG_9VZqhFOLf7mDapll273j38M,2750
-akamaiproperty-2.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-akamaiproperty-2.6.dist-info/top_level.txt,sha256=WkJajYDRewKSoiM7pWtvfXJ2lGgf9kGLxu56DT7JXh0,15
-akamaiproperty-2.6.dist-info/RECORD,,
+akamaiproperty-2.7.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+akamaiproperty-2.7.dist-info/METADATA,sha256=ecfozEYj_v2JD73WQ5hjYrJiEOrSIqQpxBFlFEVkUhw,2750
+akamaiproperty-2.7.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+akamaiproperty-2.7.dist-info/top_level.txt,sha256=WkJajYDRewKSoiM7pWtvfXJ2lGgf9kGLxu56DT7JXh0,15
+akamaiproperty-2.7.dist-info/RECORD,,
```

