# Comparing `tmp/bifrost_common_py-0.7.tar.gz` & `tmp/bifrost_common_py-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Z00440pu\Projects\bifrost-common-python\dist\tmps3c6lx03\bifrost_common_py-0.7.tar", last modified: Tue Oct 25 06:16:52 2022, max compression
+gzip compressed data, was "bifrost_common_py-0.8.tar", last modified: Fri Apr 14 10:43:18 2023, max compression
```

## Comparing `bifrost_common_py-0.7.tar` & `bifrost_common_py-0.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2022-10-25 06:16:52.000000 bifrost_common_py-0.7/
-drwxrwxrwx   0        0        0        0 2022-10-25 06:16:52.000000 bifrost_common_py-0.7/bifrost_common_py/
--rw-rw-rw-   0        0        0    22100 2022-01-25 10:56:27.000000 bifrost_common_py-0.7/bifrost_common_py/DataFrame.py
--rw-rw-rw-   0        0        0     1329 2021-09-06 06:53:39.000000 bifrost_common_py-0.7/bifrost_common_py/idOfRef.py
--rw-rw-rw-   0        0        0     5077 2021-09-07 07:32:13.000000 bifrost_common_py-0.7/bifrost_common_py/Log.py
--rw-rw-rw-   0        0        0     1579 2021-08-31 05:18:28.000000 bifrost_common_py-0.7/bifrost_common_py/safepointer.py
--rw-rw-rw-   0        0        0    24361 2022-10-25 06:12:40.000000 bifrost_common_py-0.7/bifrost_common_py/SelectFrom.py
--rw-rw-rw-   0        0        0    12386 2022-01-25 08:25:17.000000 bifrost_common_py-0.7/bifrost_common_py/selectors.py
--rw-rw-rw-   0        0        0     2105 2022-01-25 09:01:59.000000 bifrost_common_py-0.7/bifrost_common_py/time.py
--rw-rw-rw-   0        0        0      583 2021-08-31 05:18:28.000000 bifrost_common_py-0.7/bifrost_common_py/tokens.py
--rw-rw-rw-   0        0        0        0 2021-08-31 05:18:12.000000 bifrost_common_py-0.7/bifrost_common_py/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-25 06:16:52.000000 bifrost_common_py-0.7/bifrost_common_py.egg-info/
--rw-rw-rw-   0        0        0        1 2022-10-25 06:16:52.000000 bifrost_common_py-0.7/bifrost_common_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     3523 2022-10-25 06:16:52.000000 bifrost_common_py-0.7/bifrost_common_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      472 2022-10-25 06:16:52.000000 bifrost_common_py-0.7/bifrost_common_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       18 2022-10-25 06:16:52.000000 bifrost_common_py-0.7/bifrost_common_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3523 2022-10-25 06:16:52.000000 bifrost_common_py-0.7/PKG-INFO
--rw-rw-rw-   0        0        0      108 2021-09-06 08:23:18.000000 bifrost_common_py-0.7/pyproject.toml
--rw-rw-rw-   0        0        0     3164 2021-09-07 08:03:02.000000 bifrost_common_py-0.7/README.md
--rw-rw-rw-   0        0        0       86 2022-10-25 06:16:52.000000 bifrost_common_py-0.7/setup.cfg
--rw-rw-rw-   0        0        0      681 2022-10-25 06:16:29.000000 bifrost_common_py-0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 10:43:18.650262 bifrost_common_py-0.8/
+-rw-rw-rw-   0        0        0     3500 2023-04-14 10:43:18.650262 bifrost_common_py-0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3164 2023-04-14 09:48:39.000000 bifrost_common_py-0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 10:43:18.638589 bifrost_common_py-0.8/bifrost_common_py/
+-rw-rw-rw-   0        0        0    22858 2023-04-14 10:42:10.000000 bifrost_common_py-0.8/bifrost_common_py/DataFrame.py
+-rw-rw-rw-   0        0        0     5077 2023-04-14 09:48:39.000000 bifrost_common_py-0.8/bifrost_common_py/Log.py
+-rw-rw-rw-   0        0        0    24361 2023-04-14 09:48:39.000000 bifrost_common_py-0.8/bifrost_common_py/SelectFrom.py
+-rw-rw-rw-   0        0        0        0 2023-04-14 09:48:39.000000 bifrost_common_py-0.8/bifrost_common_py/__init__.py
+-rw-rw-rw-   0        0        0     1329 2023-04-14 09:48:39.000000 bifrost_common_py-0.8/bifrost_common_py/idOfRef.py
+-rw-rw-rw-   0        0        0     1579 2023-04-14 09:48:39.000000 bifrost_common_py-0.8/bifrost_common_py/safepointer.py
+-rw-rw-rw-   0        0        0    12386 2023-04-14 09:48:39.000000 bifrost_common_py-0.8/bifrost_common_py/selectors.py
+-rw-rw-rw-   0        0        0     2105 2023-04-14 09:48:39.000000 bifrost_common_py-0.8/bifrost_common_py/time.py
+-rw-rw-rw-   0        0        0      583 2023-04-14 09:48:39.000000 bifrost_common_py-0.8/bifrost_common_py/tokens.py
+drwxrwxrwx   0        0        0        0 2023-04-14 10:43:18.650262 bifrost_common_py-0.8/bifrost_common_py.egg-info/
+-rw-rw-rw-   0        0        0     3500 2023-04-14 10:43:18.000000 bifrost_common_py-0.8/bifrost_common_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      472 2023-04-14 10:43:18.000000 bifrost_common_py-0.8/bifrost_common_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 10:43:18.000000 bifrost_common_py-0.8/bifrost_common_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-04-14 10:43:18.000000 bifrost_common_py-0.8/bifrost_common_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2023-04-14 09:48:39.000000 bifrost_common_py-0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-04-14 10:43:18.650262 bifrost_common_py-0.8/setup.cfg
+-rw-rw-rw-   0        0        0      681 2023-04-14 10:42:42.000000 bifrost_common_py-0.8/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `bifrost_common_py-0.7/bifrost_common_py/DataFrame.py` & `bifrost_common_py-0.8/bifrost_common_py/DataFrame.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 
 # This is the standard data format for dynamics data exchange inside and outside of BIFROST JOTUNN.
 # 
 # @module DataFrame
 # @author Ralf Mosshammer <bifrost.at@siemens.com>, ported by Manuel Matzinger <manuel.matzinger@siemens.com>
 # @copyright Ralf Mosshammer, Siemens AG, 2020, 2021
 
-TYPEID = 'DATAFRAME'
+from typing import Any
 import json
 import uuid
+TYPEID = 'DATAFRAME'
 
 """
 This is the standard data exchange format for BIFROST dynamics data. A data frame
  reflects the values of one or more dynamics across a common time vector (which can be one).
 
  dataFrame := {
    dataFrameId: ...                   An optional, unique frame ID
@@ -105,23 +106,27 @@
                 raise Exception('Invalid "flags" cardinality for DataFrame ('+str(len(flags))+'): must be '+str(cardinality)+'.')
         else:
             # Infer the flags array
             flags = [[] for i in range(cardinality)]
 
         #Try to automatically determine the type if none is given
         if not datatype:
-            datatype = self.inferType(values[0])
+            datatype = DataFrame.inferType(values[0])
 
 
         # Type verification
         if datatype != self.types()['UNKNOWN']:
             _v = values[0][0] if isinstance(values[0], list) else values[0]
             if _v != self.values()['NULL']:
                 detectedType = type(_v)
-                if detectedType is not self.pytypes()[datatype]:
+                if datatype == DataFrame.types()['INTEGER'] or datatype == DataFrame.types()['FLOAT']:
+                    if not (detectedType is int or detectedType is float):
+                        raise Exception(
+                            'Invalid "values" type for DataFrame: must be '+str(datatype)+' (was '+str(detectedType)+').')
+                elif detectedType is not self.pytypes()[datatype]:
                     raise Exception('Type mismatch: declared type is {'+str(datatype)+'}, but detected type is {'+str(detectedType)+'}.')
                 
         # Existing elements are purged
         try:
             idx = -1
             idx = self.series.index(dynamicId)
             #idx = self.series.findIndex(entry => entry.dynamicId == dynamicId)
@@ -185,14 +190,24 @@
     Yield a JSON string representing this frame.
     """
     def toJSONString(self, pretty = False):
         if pretty:
             return json.dumps(self.toObject(), indent=2)
         return json.dumps(self.toObject())
     
+    def getValuesById(self, dynamicId: str):
+        """
+        Get the values for a given dynamic ID. Returns None if the dynamic ID is not found.
+        """
+        entry = next(
+            (entry for entry in self.series if entry['dynamicId'] == dynamicId), None)
+        if entry == None:
+            return None
+        return entry['values']
+
     """
     String representation of the data frame header info.
     """
     def formatHeader(self):
         result = ''
         id = self.dataFrameId or '(anonymous)'
         if self.isEmpty():
@@ -282,16 +297,16 @@
     Allowed value types.
     """
     @staticmethod
     def types():
         return {
             'BOOLEAN' : 'boolean',
             'INTEGER' : 'integer',
-            'FLOAT'   : 'float',
-            'NUMBER'  : 'float',
+            'FLOAT'   : 'number',
+            'NUMBER'  : 'number',
             'STRING'  : 'string',
             'UNKNOWN' : 'unknown',
             'DEFAULT' : 'string'
         }
     
     """
     Python type equivalents.
@@ -476,15 +491,15 @@
             result = result + str(_value)
         else:
             result = result + '[ '
             result = result + sep.join([str(elem) for elem in _value])
             result = result + ' ]'
         return result
 
-
+    @staticmethod
     def inferType(_value):
         value = _value
         if isinstance(value, list):
             if len(value) > 0:
                 value = value[0]
             else:
                 value = None
```

### Comparing `bifrost_common_py-0.7/bifrost_common_py/idOfRef.py` & `bifrost_common_py-0.8/bifrost_common_py/idOfRef.py`

 * *Files identical despite different names*

### Comparing `bifrost_common_py-0.7/bifrost_common_py/Log.py` & `bifrost_common_py-0.8/bifrost_common_py/Log.py`

 * *Files identical despite different names*

### Comparing `bifrost_common_py-0.7/bifrost_common_py/safepointer.py` & `bifrost_common_py-0.8/bifrost_common_py/safepointer.py`

 * *Files identical despite different names*

### Comparing `bifrost_common_py-0.7/bifrost_common_py/SelectFrom.py` & `bifrost_common_py-0.8/bifrost_common_py/SelectFrom.py`

 * *Files identical despite different names*

### Comparing `bifrost_common_py-0.7/bifrost_common_py/selectors.py` & `bifrost_common_py-0.8/bifrost_common_py/selectors.py`

 * *Files identical despite different names*

### Comparing `bifrost_common_py-0.7/bifrost_common_py/time.py` & `bifrost_common_py-0.8/bifrost_common_py/time.py`

 * *Files identical despite different names*

### Comparing `bifrost_common_py-0.7/bifrost_common_py/tokens.py` & `bifrost_common_py-0.8/bifrost_common_py/tokens.py`

 * *Files identical despite different names*

### Comparing `bifrost_common_py-0.7/bifrost_common_py.egg-info/PKG-INFO` & `bifrost_common_py-0.8/bifrost_common_py.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: bifrost-common-py
-Version: 0.7
+Version: 0.8
 Summary: Common python library functions for interacting with BIFROST.
 Home-page: https://bifrost.siemens.com/en
+Download-URL: 
 Author: Manuel Matzinger
 Author-email: bifrost.at@siemens.com
-License: UNKNOWN
 Keywords: bifrost,bifrost-common
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # bifrost-common
 
 A library of commonly used functions to interact with BIFROST. Useful for module developers.
 
 ## Installation
@@ -122,8 +121,7 @@
 
     SelectFrom(state).allDynamics().ofType('VOLTAGE-3P').asValueMap()
 
     SelectFrom(subs).allEntries().ofType('CLIMATE-MODEL').asValueList()
 
     SelectFrom(subs, state).allEntries().withParentOfType('WEATHER').asValueMap()
 ```
-
```

### Comparing `bifrost_common_py-0.7/PKG-INFO` & `bifrost_common_py-0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: bifrost_common_py
-Version: 0.7
+Version: 0.8
 Summary: Common python library functions for interacting with BIFROST.
 Home-page: https://bifrost.siemens.com/en
+Download-URL: 
 Author: Manuel Matzinger
 Author-email: bifrost.at@siemens.com
-License: UNKNOWN
 Keywords: bifrost,bifrost-common
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # bifrost-common
 
 A library of commonly used functions to interact with BIFROST. Useful for module developers.
 
 ## Installation
@@ -122,8 +121,7 @@
 
     SelectFrom(state).allDynamics().ofType('VOLTAGE-3P').asValueMap()
 
     SelectFrom(subs).allEntries().ofType('CLIMATE-MODEL').asValueList()
 
     SelectFrom(subs, state).allEntries().withParentOfType('WEATHER').asValueMap()
 ```
-
```

### Comparing `bifrost_common_py-0.7/README.md` & `bifrost_common_py-0.8/README.md`

 * *Files identical despite different names*

### Comparing `bifrost_common_py-0.7/setup.py` & `bifrost_common_py-0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = 'bifrost_common_py',
     packages = ['bifrost_common_py'],
-    version = '0.7',  # Ideally should be same as your GitHub release tag varsion
+    version = '0.8',  # Ideally should be same as your GitHub release tag varsion
     description = 'Common python library functions for interacting with BIFROST.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author = 'Manuel Matzinger',
     author_email = 'bifrost.at@siemens.com',
     url = 'https://bifrost.siemens.com/en',
     download_url = '',
```

