# Comparing `tmp/wwpdb.io-0.27.tar.gz` & `tmp/wwpdb.io-0.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.io-0.27.tar", last modified: Sun Apr  2 12:46:23 2023, max compression
+gzip compressed data, was "wwpdb.io-0.28.tar", last modified: Fri Apr 14 12:08:51 2023, max compression
```

## Comparing `wwpdb.io-0.27.tar` & `wwpdb.io-0.28.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-02 12:46:23.904993 wwpdb.io-0.27/
--rw-r--r--   0 vsts      (1001) docker     (123)      552 2023-04-02 12:45:11.000000 wwpdb.io-0.27/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (123)      731 2023-04-02 12:46:23.904993 wwpdb.io-0.27/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      764 2023-04-02 12:45:11.000000 wwpdb.io-0.27/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-04-02 12:46:23.904993 wwpdb.io-0.27/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (123)     2019 2023-04-02 12:45:11.000000 wwpdb.io-0.27/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-02 12:46:23.900993 wwpdb.io-0.27/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-04-02 12:45:11.000000 wwpdb.io-0.27/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-02 12:46:23.900993 wwpdb.io-0.27/wwpdb/io/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-04-02 12:45:11.000000 wwpdb.io-0.27/wwpdb/io/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-02 12:46:23.900993 wwpdb.io-0.27/wwpdb/io/cvs/
--rw-r--r--   0 vsts      (1001) docker     (123)    30369 2023-04-02 12:45:11.000000 wwpdb.io-0.27/wwpdb/io/cvs/CvsAdmin.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8868 2023-04-02 12:45:11.000000 wwpdb.io-0.27/wwpdb/io/cvs/CvsUtility.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-02 12:45:11.000000 wwpdb.io-0.27/wwpdb/io/cvs/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-02 12:46:23.900993 wwpdb.io-0.27/wwpdb/io/file/
--rwxr-xr-x   0 vsts      (1001) docker     (123)    24712 2023-04-02 12:45:11.000000 wwpdb.io-0.27/wwpdb/io/file/DataExchange.py
--rw-r--r--   0 vsts      (1001) docker     (123)    20256 2023-04-02 12:45:11.000000 wwpdb.io-0.27/wwpdb/io/file/DataFile.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)    19073 2023-04-02 12:45:11.000000 wwpdb.io-0.27/wwpdb/io/file/DataMaintenance.py
--rw-r--r--   0 vsts      (1001) docker     (123)    19244 2023-04-02 12:45:11.000000 wwpdb.io-0.27/wwpdb/io/file/ValidateXml.py
--rw-r--r--   0 vsts      (1001) docker     (123)      150 2023-04-02 12:45:11.000000 wwpdb.io-0.27/wwpdb/io/file/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5643 2023-04-02 12:45:11.000000 wwpdb.io-0.27/wwpdb/io/file/mmCIFUtil.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-02 12:46:23.900993 wwpdb.io-0.27/wwpdb/io/graphics/
--rw-r--r--   0 vsts      (1001) docker     (123)    21126 2023-04-02 12:45:11.000000 wwpdb.io-0.27/wwpdb/io/graphics/GraphicsContext3D.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-02 12:45:11.000000 wwpdb.io-0.27/wwpdb/io/graphics/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-02 12:46:23.904993 wwpdb.io-0.27/wwpdb/io/locator/
--rw-r--r--   0 vsts      (1001) docker     (123)     7798 2023-04-02 12:45:11.000000 wwpdb.io-0.27/wwpdb/io/locator/ChemRefPathInfo.py
--rw-r--r--   0 vsts      (1001) docker     (123)    46376 2023-04-02 12:45:11.000000 wwpdb.io-0.27/wwpdb/io/locator/DataReference.py
--rw-r--r--   0 vsts      (1001) docker     (123)    26661 2023-04-02 12:45:11.000000 wwpdb.io-0.27/wwpdb/io/locator/PathInfo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6396 2023-04-02 12:45:11.000000 wwpdb.io-0.27/wwpdb/io/locator/ReleaseFileNames.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3718 2023-04-02 12:45:11.000000 wwpdb.io-0.27/wwpdb/io/locator/ReleasePathInfo.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-02 12:45:11.000000 wwpdb.io-0.27/wwpdb/io/locator/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2669 2023-04-02 12:45:11.000000 wwpdb.io-0.27/wwpdb/io/locator/localFTPPathInfo.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-02 12:46:23.904993 wwpdb.io-0.27/wwpdb/io/misc/
--rw-r--r--   0 vsts      (1001) docker     (123)     3765 2023-04-02 12:45:11.000000 wwpdb.io-0.27/wwpdb/io/misc/FormatOut.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-02 12:45:11.000000 wwpdb.io-0.27/wwpdb/io/misc/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-02 12:46:23.904993 wwpdb.io-0.27/wwpdb/io/sftp/
--rw-r--r--   0 vsts      (1001) docker     (123)     2301 2023-04-02 12:45:11.000000 wwpdb.io-0.27/wwpdb/io/sftp/ArchiveIoBase.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7319 2023-04-02 12:45:11.000000 wwpdb.io-0.27/wwpdb/io/sftp/ArchiveIoSftp.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-02 12:45:11.000000 wwpdb.io-0.27/wwpdb/io/sftp/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-02 12:46:23.900993 wwpdb.io-0.27/wwpdb.io.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      731 2023-04-02 12:46:23.000000 wwpdb.io-0.27/wwpdb.io.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      961 2023-04-02 12:46:23.000000 wwpdb.io-0.27/wwpdb.io.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-02 12:46:23.000000 wwpdb.io-0.27/wwpdb.io.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-02 12:46:03.000000 wwpdb.io-0.27/wwpdb.io.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       96 2023-04-02 12:46:23.000000 wwpdb.io-0.27/wwpdb.io.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-04-02 12:46:23.000000 wwpdb.io-0.27/wwpdb.io.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-14 12:08:51.295142 wwpdb.io-0.28/
+-rw-r--r--   0 vsts      (1001) docker     (123)      552 2023-04-14 12:07:57.000000 wwpdb.io-0.28/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (123)      731 2023-04-14 12:08:51.295142 wwpdb.io-0.28/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      764 2023-04-14 12:07:57.000000 wwpdb.io-0.28/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-04-14 12:08:51.295142 wwpdb.io-0.28/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     2019 2023-04-14 12:07:57.000000 wwpdb.io-0.28/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-14 12:08:51.291142 wwpdb.io-0.28/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-04-14 12:07:57.000000 wwpdb.io-0.28/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-14 12:08:51.291142 wwpdb.io-0.28/wwpdb/io/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-04-14 12:07:57.000000 wwpdb.io-0.28/wwpdb/io/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-14 12:08:51.295142 wwpdb.io-0.28/wwpdb/io/cvs/
+-rw-r--r--   0 vsts      (1001) docker     (123)    30369 2023-04-14 12:07:57.000000 wwpdb.io-0.28/wwpdb/io/cvs/CvsAdmin.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8868 2023-04-14 12:07:57.000000 wwpdb.io-0.28/wwpdb/io/cvs/CvsUtility.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-14 12:07:57.000000 wwpdb.io-0.28/wwpdb/io/cvs/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-14 12:08:51.295142 wwpdb.io-0.28/wwpdb/io/file/
+-rwxr-xr-x   0 vsts      (1001) docker     (123)    24712 2023-04-14 12:07:57.000000 wwpdb.io-0.28/wwpdb/io/file/DataExchange.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    20256 2023-04-14 12:07:57.000000 wwpdb.io-0.28/wwpdb/io/file/DataFile.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)    19073 2023-04-14 12:07:57.000000 wwpdb.io-0.28/wwpdb/io/file/DataMaintenance.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    19244 2023-04-14 12:07:57.000000 wwpdb.io-0.28/wwpdb/io/file/ValidateXml.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      150 2023-04-14 12:07:57.000000 wwpdb.io-0.28/wwpdb/io/file/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5643 2023-04-14 12:07:57.000000 wwpdb.io-0.28/wwpdb/io/file/mmCIFUtil.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-14 12:08:51.295142 wwpdb.io-0.28/wwpdb/io/graphics/
+-rw-r--r--   0 vsts      (1001) docker     (123)    21126 2023-04-14 12:07:57.000000 wwpdb.io-0.28/wwpdb/io/graphics/GraphicsContext3D.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-14 12:07:57.000000 wwpdb.io-0.28/wwpdb/io/graphics/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-14 12:08:51.295142 wwpdb.io-0.28/wwpdb/io/locator/
+-rw-r--r--   0 vsts      (1001) docker     (123)     7798 2023-04-14 12:07:57.000000 wwpdb.io-0.28/wwpdb/io/locator/ChemRefPathInfo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    46376 2023-04-14 12:07:57.000000 wwpdb.io-0.28/wwpdb/io/locator/DataReference.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    27016 2023-04-14 12:07:57.000000 wwpdb.io-0.28/wwpdb/io/locator/PathInfo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6396 2023-04-14 12:07:57.000000 wwpdb.io-0.28/wwpdb/io/locator/ReleaseFileNames.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3718 2023-04-14 12:07:57.000000 wwpdb.io-0.28/wwpdb/io/locator/ReleasePathInfo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-14 12:07:57.000000 wwpdb.io-0.28/wwpdb/io/locator/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2669 2023-04-14 12:07:57.000000 wwpdb.io-0.28/wwpdb/io/locator/localFTPPathInfo.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-14 12:08:51.295142 wwpdb.io-0.28/wwpdb/io/misc/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3765 2023-04-14 12:07:57.000000 wwpdb.io-0.28/wwpdb/io/misc/FormatOut.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-14 12:07:57.000000 wwpdb.io-0.28/wwpdb/io/misc/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-14 12:08:51.295142 wwpdb.io-0.28/wwpdb/io/sftp/
+-rw-r--r--   0 vsts      (1001) docker     (123)     2301 2023-04-14 12:07:57.000000 wwpdb.io-0.28/wwpdb/io/sftp/ArchiveIoBase.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7319 2023-04-14 12:07:57.000000 wwpdb.io-0.28/wwpdb/io/sftp/ArchiveIoSftp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-04-14 12:07:57.000000 wwpdb.io-0.28/wwpdb/io/sftp/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-14 12:08:51.291142 wwpdb.io-0.28/wwpdb.io.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      731 2023-04-14 12:08:51.000000 wwpdb.io-0.28/wwpdb.io.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      961 2023-04-14 12:08:51.000000 wwpdb.io-0.28/wwpdb.io.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-14 12:08:51.000000 wwpdb.io-0.28/wwpdb.io.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-14 12:08:34.000000 wwpdb.io-0.28/wwpdb.io.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       96 2023-04-14 12:08:51.000000 wwpdb.io-0.28/wwpdb.io.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-04-14 12:08:51.000000 wwpdb.io-0.28/wwpdb.io.egg-info/top_level.txt
```

### Comparing `wwpdb.io-0.27/LICENSE` & `wwpdb.io-0.28/LICENSE`

 * *Files identical despite different names*

### Comparing `wwpdb.io-0.27/PKG-INFO` & `wwpdb.io-0.28/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.io
-Version: 0.27
+Version: 0.28
 Summary: wwPDB Python Configuration Parsing
 Home-page: https://github.com/rcsb/py-wwpdb_io
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.io-0.27/README.md` & `wwpdb.io-0.28/README.md`

 * *Files identical despite different names*

### Comparing `wwpdb.io-0.27/setup.py` & `wwpdb.io-0.28/setup.py`

 * *Files identical despite different names*

### Comparing `wwpdb.io-0.27/wwpdb/io/cvs/CvsAdmin.py` & `wwpdb.io-0.28/wwpdb/io/cvs/CvsAdmin.py`

 * *Files identical despite different names*

### Comparing `wwpdb.io-0.27/wwpdb/io/cvs/CvsUtility.py` & `wwpdb.io-0.28/wwpdb/io/cvs/CvsUtility.py`

 * *Files identical despite different names*

### Comparing `wwpdb.io-0.27/wwpdb/io/file/DataExchange.py` & `wwpdb.io-0.28/wwpdb/io/file/DataExchange.py`

 * *Files identical despite different names*

### Comparing `wwpdb.io-0.27/wwpdb/io/file/DataFile.py` & `wwpdb.io-0.28/wwpdb/io/file/DataFile.py`

 * *Files identical despite different names*

### Comparing `wwpdb.io-0.27/wwpdb/io/file/DataMaintenance.py` & `wwpdb.io-0.28/wwpdb/io/file/DataMaintenance.py`

 * *Files identical despite different names*

### Comparing `wwpdb.io-0.27/wwpdb/io/file/ValidateXml.py` & `wwpdb.io-0.28/wwpdb/io/file/ValidateXml.py`

 * *Files identical despite different names*

### Comparing `wwpdb.io-0.27/wwpdb/io/file/mmCIFUtil.py` & `wwpdb.io-0.28/wwpdb/io/file/mmCIFUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.io-0.27/wwpdb/io/graphics/GraphicsContext3D.py` & `wwpdb.io-0.28/wwpdb/io/graphics/GraphicsContext3D.py`

 * *Files identical despite different names*

### Comparing `wwpdb.io-0.27/wwpdb/io/locator/ChemRefPathInfo.py` & `wwpdb.io-0.28/wwpdb/io/locator/ChemRefPathInfo.py`

 * *Files identical despite different names*

### Comparing `wwpdb.io-0.27/wwpdb/io/locator/DataReference.py` & `wwpdb.io-0.28/wwpdb/io/locator/DataReference.py`

 * *Files identical despite different names*

### Comparing `wwpdb.io-0.27/wwpdb/io/locator/PathInfo.py` & `wwpdb.io-0.28/wwpdb/io/locator/PathInfo.py`

 * *Files 1% similar despite different names*

```diff
@@ -356,14 +356,19 @@
             versionId=versionId,
             partNumber="1",
             contentTypeBase="nmr-chemical-shifts",
             formatType=formatType,
             mileStone=mileStone,
         )
 
+    def getAssemblyModelFilePath(self, dataSetId, wfInstanceId=None, fileSource="deposit", versionId="latest", mileStone=None):
+        return self.__getStandardPath(
+            dataSetId=dataSetId, wfInstanceId=wfInstanceId, fileSource=fileSource, versionId=versionId, contentTypeBase="assembly-model", formatType="pdbx", mileStone=mileStone
+        )
+
     def getStatusHistoryFilePath(self, dataSetId, fileSource="archive", versionId="latest"):
         return self.__getStandardPath(
             dataSetId=dataSetId, wfInstanceId=None, fileSource=fileSource, versionId=versionId, partNumber="1", contentTypeBase="status-history", formatType="pdbx", mileStone=None
         )
 
     #
     def getFilePath(self, dataSetId, wfInstanceId=None, contentType=None, formatType=None, fileSource="archive", versionId="latest", partNumber="1", mileStone=None):
```

### Comparing `wwpdb.io-0.27/wwpdb/io/locator/ReleaseFileNames.py` & `wwpdb.io-0.28/wwpdb/io/locator/ReleaseFileNames.py`

 * *Files identical despite different names*

### Comparing `wwpdb.io-0.27/wwpdb/io/locator/ReleasePathInfo.py` & `wwpdb.io-0.28/wwpdb/io/locator/ReleasePathInfo.py`

 * *Files identical despite different names*

### Comparing `wwpdb.io-0.27/wwpdb/io/locator/localFTPPathInfo.py` & `wwpdb.io-0.28/wwpdb/io/locator/localFTPPathInfo.py`

 * *Files identical despite different names*

### Comparing `wwpdb.io-0.27/wwpdb/io/misc/FormatOut.py` & `wwpdb.io-0.28/wwpdb/io/misc/FormatOut.py`

 * *Files identical despite different names*

### Comparing `wwpdb.io-0.27/wwpdb/io/sftp/ArchiveIoBase.py` & `wwpdb.io-0.28/wwpdb/io/sftp/ArchiveIoBase.py`

 * *Files identical despite different names*

### Comparing `wwpdb.io-0.27/wwpdb/io/sftp/ArchiveIoSftp.py` & `wwpdb.io-0.28/wwpdb/io/sftp/ArchiveIoSftp.py`

 * *Files identical despite different names*

### Comparing `wwpdb.io-0.27/wwpdb.io.egg-info/PKG-INFO` & `wwpdb.io-0.28/wwpdb.io.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.io
-Version: 0.27
+Version: 0.28
 Summary: wwPDB Python Configuration Parsing
 Home-page: https://github.com/rcsb/py-wwpdb_io
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.io-0.27/wwpdb.io.egg-info/SOURCES.txt` & `wwpdb.io-0.28/wwpdb.io.egg-info/SOURCES.txt`

 * *Files identical despite different names*

