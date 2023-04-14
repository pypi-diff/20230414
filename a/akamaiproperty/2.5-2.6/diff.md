# Comparing `tmp/akamaiproperty-2.5-py3-none-any.whl.zip` & `tmp/akamaiproperty-2.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 13564 bytes, number of entries: 8
+Zip file size: 13852 bytes, number of entries: 8
 -rw-r--r--  2.0 unx      108 b- defN 22-Jun-12 17:02 akamaiproperty/__init__.py
--rw-r--r--  2.0 unx    27311 b- defN 23-Mar-24 08:13 akamaiproperty/akamaiproperty.py
+-rw-r--r--  2.0 unx    28603 b- defN 23-Apr-14 09:44 akamaiproperty/akamaiproperty.py
 -rw-r--r--  2.0 unx     7127 b- defN 22-Jun-12 17:02 akamaiproperty/http_calls.py
--rwx------  2.0 unx    11357 b- defN 23-Mar-24 08:17 akamaiproperty-2.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     2750 b- defN 23-Mar-24 08:17 akamaiproperty-2.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-24 08:17 akamaiproperty-2.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-Mar-24 08:17 akamaiproperty-2.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      669 b- defN 23-Mar-24 08:17 akamaiproperty-2.5.dist-info/RECORD
-8 files, 49429 bytes uncompressed, 12394 bytes compressed:  74.9%
+-rwx------  2.0 unx    11357 b- defN 23-Apr-14 09:47 akamaiproperty-2.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2750 b- defN 23-Apr-14 09:47 akamaiproperty-2.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-14 09:47 akamaiproperty-2.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-Apr-14 09:47 akamaiproperty-2.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      669 b- defN 23-Apr-14 09:47 akamaiproperty-2.6.dist-info/RECORD
+8 files, 50721 bytes uncompressed, 12682 bytes compressed:  75.0%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: akamaiproperty/akamaiproperty.py
 Comment: 
 
 Filename: akamaiproperty/http_calls.py
 Comment: 
 
-Filename: akamaiproperty-2.5.dist-info/LICENSE
+Filename: akamaiproperty-2.6.dist-info/LICENSE
 Comment: 
 
-Filename: akamaiproperty-2.5.dist-info/METADATA
+Filename: akamaiproperty-2.6.dist-info/METADATA
 Comment: 
 
-Filename: akamaiproperty-2.5.dist-info/WHEEL
+Filename: akamaiproperty-2.6.dist-info/WHEEL
 Comment: 
 
-Filename: akamaiproperty-2.5.dist-info/top_level.txt
+Filename: akamaiproperty-2.6.dist-info/top_level.txt
 Comment: 
 
-Filename: akamaiproperty-2.5.dist-info/RECORD
+Filename: akamaiproperty-2.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## akamaiproperty/akamaiproperty.py

```diff
@@ -404,14 +404,23 @@
             return []
         behaviorParsedList = self._getBehaviorParsedList(version)
         cpCodeList = []
         for behavior in behaviorParsedList:
             if behavior["behavior"]["name"] == 'cpCode':
                 cpCodeList.append(behavior["behavior"]["options"]['value']['id'])
         cpCodeList = list(dict.fromkeys(cpCodeList))
+        print(cpCodeList)
+        
+        ruleTree = self.getRuleTree(int(version))
+        cpCodeAdvancedList = self.extractCPCodes(ruleTree)
+        print(cpCodeAdvancedList)
+        cpCodeList = cpCodeList + cpCodeAdvancedList
+        cpCodeList = list(dict.fromkeys(cpCodeList))
+        print(cpCodeList)
+
         return cpCodeList
 
     def getMappings(self,productId):
         prdMappingJson = {'prd_Adaptive_Media_Delivery': 'Adaptive Media Delivery',
             'prd_Obj_Delivery': 'Object Delivery',
             'prd_Download_Delivery': 'Download Delivery',
             'prd_Dynamic_Site_Del': 'Dynamic Site Delivery',
@@ -547,14 +556,43 @@
         if version == 0:
             version = stagingVersion
             if version == 0:
                 version = latestVersion
 
         return version 
 
+    def extractCPCodes(self,json_data):
+        """
+        Extracts the numbers from a string that contains one or more occurrences of the tag <reporting:cpcode>
+        followed by the number.
+        """
+        start_tag = "<reporting:cpcode>"
+        end_tag = "</reporting:cpcode>"
+        start_index = 0
+        advancedCPCodeList = []
+        ruleTree = json.dumps(json_data)
+        
+        while True:
+            start_index = ruleTree.find(start_tag, start_index)
+            if start_index == -1:
+                break
+                
+            start_index += len(start_tag)
+            end_index = ruleTree.find(end_tag, start_index)
+            if end_index == -1:
+                break
+            
+            number = ruleTree[start_index:end_index].strip()
+            if number.isdigit():
+                advancedCPCodeList.append(int(number))
+                
+            start_index = end_index + len(end_tag)
+        
+        return advancedCPCodeList
+
 
 class AkamaiPropertyManager():
     def __init__(self,edgercLocation,accountSwitchKey=None):
         self.accountSwitchKey = ''
         self._edgerc = ''
         self._prdHttpCaller = ''
         self._session = ''
```

## Comparing `akamaiproperty-2.5.dist-info/LICENSE` & `akamaiproperty-2.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `akamaiproperty-2.5.dist-info/METADATA` & `akamaiproperty-2.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akamaiproperty
-Version: 2.5
+Version: 2.6
 Summary: A Pip Package for Akamai Property
 Home-page: https://github.com/Achuthananda/AkamaiPropertyManager
 Author: Achuthananda M P
 Author-email: achuthadivine@gmail.com
 Keywords: Akamai Property CDN AkamaiConfigs Edge
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `akamaiproperty-2.5.dist-info/RECORD` & `akamaiproperty-2.6.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 akamaiproperty/__init__.py,sha256=Pk0acNhv3PYXX7_BcWYe68ASjnpu29gCKUtCwpvbz7o,108
-akamaiproperty/akamaiproperty.py,sha256=lEe-zflwYs0mUOdoyD8Kh0jsomUdCKndBuuToE8Ok10,27311
+akamaiproperty/akamaiproperty.py,sha256=vsfmo_dWyilhiM9k-DEZx3Z-eW68JGOESVsocOwz7tI,28603
 akamaiproperty/http_calls.py,sha256=lQj18BM77O0RUNN4Knv1RkVRE2R65dsOm_Yk_TnD6Ww,7127
-akamaiproperty-2.5.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-akamaiproperty-2.5.dist-info/METADATA,sha256=jZqror6_uXwS-2-PolWxpYeX1R6kAYU063feZcg4ecc,2750
-akamaiproperty-2.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-akamaiproperty-2.5.dist-info/top_level.txt,sha256=WkJajYDRewKSoiM7pWtvfXJ2lGgf9kGLxu56DT7JXh0,15
-akamaiproperty-2.5.dist-info/RECORD,,
+akamaiproperty-2.6.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+akamaiproperty-2.6.dist-info/METADATA,sha256=C1FNaFeyRd35ymsFDgG_9VZqhFOLf7mDapll273j38M,2750
+akamaiproperty-2.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+akamaiproperty-2.6.dist-info/top_level.txt,sha256=WkJajYDRewKSoiM7pWtvfXJ2lGgf9kGLxu56DT7JXh0,15
+akamaiproperty-2.6.dist-info/RECORD,,
```

