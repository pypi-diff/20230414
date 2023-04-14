# Comparing `tmp/eptools-8.5.3.tar.gz` & `tmp/eptools-8.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\EasypostLibrary\eptools\dist\tmp5ih67x9r\eptools-8.5.3.tar", last modified: Fri Apr  7 12:46:56 2023, max compression
+gzip compressed data, was "C:\EasypostLibrary\eptools\dist\tmpr648nnm6\eptools-8.5.4.tar", last modified: Fri Apr 14 07:52:20 2023, max compression
```

## Comparing `eptools-8.5.3.tar` & `eptools-8.5.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 12:46:56.000000 eptools-8.5.3/
-drwxrwxrwx   0        0        0        0 2023-04-07 12:46:56.000000 eptools-8.5.3/eptools/
--rw-rw-rw-   0        0        0      759 2022-10-20 08:53:57.000000 eptools-8.5.3/eptools/configuration.py
--rw-rw-rw-   0        0        0     6313 2022-06-28 08:12:23.000000 eptools-8.5.3/eptools/InvoiceDate.py
--rw-rw-rw-   0        0        0     9099 2023-03-24 15:00:32.000000 eptools-8.5.3/eptools/logger.py
--rw-rw-rw-   0        0        0     2401 2023-03-20 16:11:43.000000 eptools-8.5.3/eptools/mail_factory.py
--rw-rw-rw-   0        0        0    21080 2023-04-07 12:44:24.000000 eptools-8.5.3/eptools/SalesForceApiIntegration.py
--rw-rw-rw-   0        0        0     2305 2023-03-24 16:33:51.000000 eptools-8.5.3/eptools/sf_factory.py
--rw-rw-rw-   0        0        0    12808 2023-02-23 18:24:58.000000 eptools-8.5.3/eptools/slacker.py
--rw-rw-rw-   0        0        0    10181 2023-03-24 16:02:09.000000 eptools-8.5.3/eptools/slack_factory.py
--rw-rw-rw-   0        0        0    12117 2023-04-04 16:10:33.000000 eptools-8.5.3/eptools/SQLFactory.py
--rw-rw-rw-   0        0        0    31294 2023-03-24 15:03:41.000000 eptools-8.5.3/eptools/WindowsServiceBase.py
--rw-rw-rw-   0        0        0        0 2021-06-30 13:43:34.000000 eptools-8.5.3/eptools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 12:46:56.000000 eptools-8.5.3/eptools.egg-info/
--rw-rw-rw-   0        0        0        1 2023-04-07 12:46:56.000000 eptools-8.5.3/eptools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      944 2023-04-07 12:46:56.000000 eptools-8.5.3/eptools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       92 2023-04-07 12:46:56.000000 eptools-8.5.3/eptools.egg-info/requires.txt
--rw-rw-rw-   0        0        0      469 2023-04-07 12:46:56.000000 eptools-8.5.3/eptools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2023-04-07 12:46:56.000000 eptools-8.5.3/eptools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1069 2021-03-05 11:50:38.000000 eptools-8.5.3/LICENSE
--rw-rw-rw-   0        0        0      944 2023-04-07 12:46:56.000000 eptools-8.5.3/PKG-INFO
--rw-rw-rw-   0        0        0      108 2021-03-05 11:44:12.000000 eptools-8.5.3/pyproject.toml
--rw-rw-rw-   0        0        0      500 2022-03-29 12:52:14.000000 eptools-8.5.3/README.md
--rw-rw-rw-   0        0        0      588 2023-04-07 12:46:56.000000 eptools-8.5.3/setup.cfg
--rw-rw-rw-   0        0        0       39 2021-03-05 11:49:21.000000 eptools-8.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 07:52:20.000000 eptools-8.5.4/
+drwxrwxrwx   0        0        0        0 2023-04-14 07:52:20.000000 eptools-8.5.4/eptools/
+-rw-rw-rw-   0        0        0      759 2022-10-20 08:53:57.000000 eptools-8.5.4/eptools/configuration.py
+-rw-rw-rw-   0        0        0     6313 2022-06-28 08:12:23.000000 eptools-8.5.4/eptools/InvoiceDate.py
+-rw-rw-rw-   0        0        0     9099 2023-03-24 15:00:32.000000 eptools-8.5.4/eptools/logger.py
+-rw-rw-rw-   0        0        0     2401 2023-03-20 16:11:43.000000 eptools-8.5.4/eptools/mail_factory.py
+-rw-rw-rw-   0        0        0    21241 2023-04-13 13:52:45.000000 eptools-8.5.4/eptools/SalesForceApiIntegration.py
+-rw-rw-rw-   0        0        0     2305 2023-03-24 16:33:51.000000 eptools-8.5.4/eptools/sf_factory.py
+-rw-rw-rw-   0        0        0    12808 2023-02-23 18:24:58.000000 eptools-8.5.4/eptools/slacker.py
+-rw-rw-rw-   0        0        0    10181 2023-03-24 16:02:09.000000 eptools-8.5.4/eptools/slack_factory.py
+-rw-rw-rw-   0        0        0    12117 2023-04-04 16:10:33.000000 eptools-8.5.4/eptools/SQLFactory.py
+-rw-rw-rw-   0        0        0    31294 2023-03-24 15:03:41.000000 eptools-8.5.4/eptools/WindowsServiceBase.py
+-rw-rw-rw-   0        0        0        0 2021-06-30 13:43:34.000000 eptools-8.5.4/eptools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 07:52:20.000000 eptools-8.5.4/eptools.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-04-14 07:52:20.000000 eptools-8.5.4/eptools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      944 2023-04-14 07:52:20.000000 eptools-8.5.4/eptools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       92 2023-04-14 07:52:20.000000 eptools-8.5.4/eptools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      469 2023-04-14 07:52:20.000000 eptools-8.5.4/eptools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        8 2023-04-14 07:52:20.000000 eptools-8.5.4/eptools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1069 2021-03-05 11:50:38.000000 eptools-8.5.4/LICENSE
+-rw-rw-rw-   0        0        0      944 2023-04-14 07:52:20.000000 eptools-8.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0      108 2021-03-05 11:44:12.000000 eptools-8.5.4/pyproject.toml
+-rw-rw-rw-   0        0        0      500 2022-03-29 12:52:14.000000 eptools-8.5.4/README.md
+-rw-rw-rw-   0        0        0      588 2023-04-14 07:52:20.000000 eptools-8.5.4/setup.cfg
+-rw-rw-rw-   0        0        0       39 2021-03-05 11:49:21.000000 eptools-8.5.4/setup.py
```

### Comparing `eptools-8.5.3/eptools/configuration.py` & `eptools-8.5.4/eptools/configuration.py`

 * *Files identical despite different names*

### Comparing `eptools-8.5.3/eptools/InvoiceDate.py` & `eptools-8.5.4/eptools/InvoiceDate.py`

 * *Files identical despite different names*

### Comparing `eptools-8.5.3/eptools/logger.py` & `eptools-8.5.4/eptools/logger.py`

 * *Files identical despite different names*

### Comparing `eptools-8.5.3/eptools/mail_factory.py` & `eptools-8.5.4/eptools/mail_factory.py`

 * *Files identical despite different names*

### Comparing `eptools-8.5.3/eptools/SalesForceApiIntegration.py` & `eptools-8.5.4/eptools/SalesForceApiIntegration.py`

 * *Files 2% similar despite different names*

```diff
@@ -316,32 +316,32 @@
                                        server = '10.10.10.30,1433',
                                        database = 'EasyPost',                                       
                                        user = 'sa',
                                        password = 'sql')
         sql = """
                 DECLARE @CustomerIdPost INT -- replace INT with the data type of your CustomerIdPost column
 
-                SET @CustomerIdPost = {} -- replace 12345 with the client number you want to search for
+                SET @CustomerIdPost = 7254 -- replace 12345 with the client number you want to search for
 
                 -- Search for the client number in SFPickupLocations
-                IF EXISTS(SELECT * FROM SFPickupLocations WHERE CustomerIdPost = @CustomerIdPost and Hub is not null and Hub !='' and RouteName is not null and RouteName !='')
+                IF EXISTS(SELECT * FROM EasyPost.dbo.SFPickupLocations WHERE CustomerIdPost = @CustomerIdPost and Hub is not null and Hub !='' and RouteName is not null and RouteName !='')
                 BEGIN
-                    SELECT CustomerIdPost, Hub,RouteName,Name, 'SFPickupLocations' as Location FROM SFPickupLocations WHERE CustomerIdPost = @CustomerIdPost
+                    SELECT CustomerIdPost, Hub,RouteName,Name, 'SFPickupLocations' as Location FROM EasyPost.dbo.SFPickupLocations WHERE CustomerIdPost = @CustomerIdPost
                 END
                 ELSE
                 -- If the client number is not found in SFPickupLocations, search for it in SFDepartment
-                IF EXISTS(SELECT * FROM SFPickupLocations WHERE SFId = (SELECT SFId FROM SFDepartments WHERE CustomerIdPost = @CustomerIdPost))
+                IF EXISTS(SELECT * FROM EasyPost.dbo.SFPickupLocations WHERE SFId = (SELECT SFId FROM SFDepartments WHERE CustomerIdPost = @CustomerIdPost))
                 BEGIN
-                    SELECT CustomerIdPost, Hub,RouteName,Name, 'SFDepartment' as Location FROM SFPickupLocations WHERE SFId = (SELECT SFId FROM SFDepartments WHERE CustomerIdPost = @CustomerIdPost)
+                    SELECT CustomerIdPost, Hub,RouteName,Name, 'SFDepartment' as Location FROM EasyPost.dbo.SFPickupLocations WHERE SFId = (SELECT SFId FROM EasyPost.dbo.SFDepartments WHERE CustomerIdPost = @CustomerIdPost)
                 END
                 ELSE
                 -- If the client number is not found in SFDepartment, search for it in SFAccount
-                IF EXISTS(SELECT * FROM SFAccounts WHERE CustomerIdPost = @CustomerIdPost and Hub is not null and RouteName is not null and Hub !='' and RouteName !='')
+                IF EXISTS(SELECT * FROM EasyPost.dbo.SFAccounts WHERE CustomerIdPost = @CustomerIdPost and Hub is not null and RouteName is not null and Hub !='' and RouteName !='')
                 BEGIN
-                    SELECT CustomerIdPost, Hub, RouteName, Name, 'SFAccount' as Location FROM SFAccounts WHERE CustomerIdPost = @CustomerIdPost
+                    SELECT CustomerIdPost, Hub,RouteName,Name, 'SFAccount' as Location FROM EasyPost.dbo.SFPickupLocations WHERE SFAccountId = (SELECT SFId FROM EasyPost.dbo.SFAccounts WHERE CustomerIdPost = @CustomerIdPost)
                 END
                 ELSE
                 -- If the client number is not found in SFAccount, search for it in EasyPostLogistiek.dbo.CustomerHub
                 IF EXISTS(SELECT * FROM EasyPostLogistiek.dbo.CustomerHub WHERE CustomerId = @CustomerIdPost)
                 BEGIN
                     SELECT CustomerId,HubName as Hub, RoundName as RouteName, c.Name, 'CustomerHub' as Location  FROM EasyPostLogistiek.dbo.CustomerHub ch LEFT JOIN EasyPost.dbo.Companies c on ch.CustomerId=c.Id WHERE CustomerId = @CustomerIdPost
                 END
```

### Comparing `eptools-8.5.3/eptools/sf_factory.py` & `eptools-8.5.4/eptools/sf_factory.py`

 * *Files identical despite different names*

### Comparing `eptools-8.5.3/eptools/slacker.py` & `eptools-8.5.4/eptools/slacker.py`

 * *Files identical despite different names*

### Comparing `eptools-8.5.3/eptools/slack_factory.py` & `eptools-8.5.4/eptools/slack_factory.py`

 * *Files identical despite different names*

### Comparing `eptools-8.5.3/eptools/SQLFactory.py` & `eptools-8.5.4/eptools/SQLFactory.py`

 * *Files identical despite different names*

### Comparing `eptools-8.5.3/eptools/WindowsServiceBase.py` & `eptools-8.5.4/eptools/WindowsServiceBase.py`

 * *Files identical despite different names*

### Comparing `eptools-8.5.3/eptools.egg-info/PKG-INFO` & `eptools-8.5.4/eptools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eptools
-Version: 8.5.3
+Version: 8.5.4
 Summary: EasyPost Tools
 Home-page: UNKNOWN
 Author: Arno De Decker
 Author-email: arno.dedecker@easypost.eu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eptools-8.5.3/LICENSE` & `eptools-8.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `eptools-8.5.3/PKG-INFO` & `eptools-8.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eptools
-Version: 8.5.3
+Version: 8.5.4
 Summary: EasyPost Tools
 Home-page: UNKNOWN
 Author: Arno De Decker
 Author-email: arno.dedecker@easypost.eu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eptools-8.5.3/setup.cfg` & `eptools-8.5.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2065 7074 6f6f 6c73 0d0a 7665 7273   = eptools..vers
-00000020: 696f 6e20 3d20 382e 352e 330d 0a61 7574  ion = 8.5.3..aut
+00000020: 696f 6e20 3d20 382e 352e 340d 0a61 7574  ion = 8.5.4..aut
 00000030: 686f 7220 3d20 4172 6e6f 2044 6520 4465  hor = Arno De De
 00000040: 636b 6572 0d0a 6175 7468 6f72 5f65 6d61  cker..author_ema
 00000050: 696c 203d 2061 726e 6f2e 6465 6465 636b  il = arno.dedeck
 00000060: 6572 4065 6173 7970 6f73 742e 6575 0d0a  er@easypost.eu..
 00000070: 6465 7363 7269 7074 696f 6e20 3d20 4561  description = Ea
 00000080: 7379 506f 7374 2054 6f6f 6c73 0d0a 6c6f  syPost Tools..lo
 00000090: 6e67 5f64 6573 6372 6970 7469 6f6e 203d  ng_description =
```

