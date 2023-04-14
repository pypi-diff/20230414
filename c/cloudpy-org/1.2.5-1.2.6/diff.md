# Comparing `tmp/cloudpy_org-1.2.5.tar.gz` & `tmp/cloudpy_org-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\cloudpy_org-1.2.5.tar", last modified: Wed Mar  8 17:41:18 2023, max compression
+gzip compressed data, was "dist\cloudpy_org-1.2.6.tar", last modified: Fri Apr 14 19:14:04 2023, max compression
```

## Comparing `cloudpy_org-1.2.5.tar` & `cloudpy_org-1.2.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-03-08 17:41:18.558546 cloudpy_org-1.2.5/
--rw-rw-rw-   0        0        0      895 2023-03-08 17:41:18.557951 cloudpy_org-1.2.5/PKG-INFO
--rw-rw-rw-   0        0        0      450 2023-01-27 10:31:15.000000 cloudpy_org-1.2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-03-08 17:41:18.462372 cloudpy_org-1.2.5/cloudpy_org/
--rw-rw-rw-   0        0        0       46 2023-01-27 10:30:03.000000 cloudpy_org-1.2.5/cloudpy_org/__init__.py
--rw-rw-rw-   0        0        0    44325 2023-03-08 17:14:02.000000 cloudpy_org-1.2.5/cloudpy_org/tools.py
-drwxrwxrwx   0        0        0        0 2023-03-08 17:41:18.537089 cloudpy_org-1.2.5/cloudpy_org.egg-info/
--rw-rw-rw-   0        0        0      895 2023-03-08 17:41:16.000000 cloudpy_org-1.2.5/cloudpy_org.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-03-08 17:41:17.000000 cloudpy_org-1.2.5/cloudpy_org.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-08 17:41:16.000000 cloudpy_org-1.2.5/cloudpy_org.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-03-08 17:41:16.000000 cloudpy_org-1.2.5/cloudpy_org.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-03-08 17:41:16.000000 cloudpy_org-1.2.5/cloudpy_org.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-08 17:41:18.558546 cloudpy_org-1.2.5/setup.cfg
--rw-rw-rw-   0        0        0     1277 2023-03-08 17:39:26.000000 cloudpy_org-1.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 19:14:04.334997 cloudpy_org-1.2.6/
+-rw-rw-rw-   0        0        0      899 2023-04-14 19:14:04.334496 cloudpy_org-1.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2023-04-14 05:11:55.000000 cloudpy_org-1.2.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 19:14:04.183958 cloudpy_org-1.2.6/cloudpy_org/
+-rw-rw-rw-   0        0        0       46 2023-01-27 10:30:03.000000 cloudpy_org-1.2.6/cloudpy_org/__init__.py
+-rw-rw-rw-   0        0        0    46837 2023-04-14 19:05:11.000000 cloudpy_org-1.2.6/cloudpy_org/tools.py
+drwxrwxrwx   0        0        0        0 2023-04-14 19:14:04.304633 cloudpy_org-1.2.6/cloudpy_org.egg-info/
+-rw-rw-rw-   0        0        0      899 2023-04-14 19:14:02.000000 cloudpy_org-1.2.6/cloudpy_org.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-04-14 19:14:03.000000 cloudpy_org-1.2.6/cloudpy_org.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 19:14:02.000000 cloudpy_org-1.2.6/cloudpy_org.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-04-14 19:14:02.000000 cloudpy_org-1.2.6/cloudpy_org.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-14 19:14:02.000000 cloudpy_org-1.2.6/cloudpy_org.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-14 19:14:04.334997 cloudpy_org-1.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     1288 2023-04-14 17:41:26.000000 cloudpy_org-1.2.6/setup.py
```

### Comparing `cloudpy_org-1.2.5/PKG-INFO` & `cloudpy_org-1.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: cloudpy_org
-Version: 1.2.5
+Version: 1.2.6
 Summary: Cloud data pipeline organization and automation library.
-Home-page: https://cloudpy.org/
+Home-page: https://www.cloudpy.org/
 Author: cloudpy.org
 Author-email: admin@cloudpy.org
 License: MIT
 Description: A library to programmatically create, interact, encrypt and automate your data pipelines making it simple to scale to the most popular cloud plattforms.
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cloudpy_org-1.2.5/cloudpy_org/tools.py` & `cloudpy_org-1.2.6/cloudpy_org/tools.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 
 from typing import Union
 from botocore.exceptions import ClientError
 from cryptography.fernet import Fernet
 import numpy as np
 import inspect
 from os import walk
+import s3fs
 
 """
 #pip install PyQt5==5.9.2
 plt.scatter(x, y)
 plt.plot(myline, mymodel(myline))
 plt.show()
 
@@ -244,15 +245,15 @@
         self.this_description = self.this_description.replace("  "," ").replace("#","\n").strip()
         exec(dynamic_code)
         return self.this_source_code, self.theseparams, self.this_returns, self.this_description
     #██████████████████████████████████████████████████████████████████████████          
 class processing_tools:
     
     def __init__(self,encryptedSession:str='',bucket_name:str=''):
-        self.alphavantage = {}
+
         self.sta_bucket,self.environment = '','local'
         self.local_directory = os.getcwd() + '/'
         self.s3_bucket = bucket_name.replace('/','') + '/'
         if bucket_name != '':
             self.sta_bucket =  's3://' + bucket_name + '/'
             self.environment = bucket_name
         self.documentation_path = self.local_directory + 'documentation/'
@@ -260,21 +261,100 @@
         self.settings = self.sta_bucket + 'settings/'
         self.secrets = self.settings + 'secrets/'
         self.metadata = self.settings + 'metadata/'
         self.datalake = self.s3_bucket + 'datalake-demo01/'
         self.hive = self.s3_bucket + 'default_hive/'
         self.dl_crypto = self.datalake + 'crypto/'
         self.dl_crypto_intraday = self.dl_crypto + 'intraday/'
-
-        self.api_key_path = self.secrets + 'alphavantage/api_key.txt'
+        try:
+            self.fs = s3fs.S3FileSystem()
+        except:
+            self.fs = None
         try:
             self.load_metadata()
         except:
             ...
     #__________________________________________________________________________
+    def dataframe_to_parquet(self,df_input:pd.DataFrame,folder_path:str,file_name:str)->str:
+        '''
+        ***
+        If the environment instance class equals "s3", then stores as parquet a given pandas dataframe to a given s3 folder url location under a given file name.
+        Otherwise, stores the dataframe locally as a parquet file in the given folder under the given file name.
+        ***
+        '''
+        extension = 'parquet'
+        rslt = ""
+        file_name = file_name.split(".")[0] + "." + extension
+        if "\\" in folder_path:
+            if folder_path[::-1][0:1] != "\\":
+                folder_path += "\\"  
+        elif folder_path[::-1][0:1] != "/":
+            folder_path += "/"
+        if self.environment == "s3":
+            try:
+                if self.fs != None:
+                    with self.fs.open(folder_path + file_name,'wb') as f:
+                        if extension == "parquet":
+                            df_input.to_parquet(f)
+                            rslt = "Data successfully stored in s3 as: " + folder_path + file_name
+                else:
+                    rslt = "Could not connect with s3 because AWS CLI credentials have not been set yet."
+            except Exception as e:
+                rslt = str(e)
+                
+        else:
+            try:
+                if extension == "parquet":
+                    df_input.to_parquet(folder_path + file_name)
+                    rslt = "Data successfully stored locally as: " + folder_path + file_name
+            except Exception as e:
+                rslt = str(e)
+        return rslt
+    #__________________________________________________________________________
+    def dataframe_to_csv(self,df_input:pd.DataFrame,folder_path:str,file_name:str,sep:str = ',',na_rep:str='',float_format:str = None,index:bool = True,encoding:str = 'utf-8')->str:
+        '''
+        ***
+        If the environment instance class equals "s3", then stores as parquet a given pandas dataframe to a given s3 folder url location under a given file name.
+        Otherwise, stores the dataframe locally as a parquet file in the given folder under the given file name.
+        ***
+        '''
+        extension = 'csv'
+        rslt = ""
+        file_name = file_name.split(".")[0] + "." + extension
+        if "\\" in folder_path:
+            if folder_path[::-1][0:1] != "\\":
+                folder_path += "\\"  
+        elif folder_path[::-1][0:1] != "/":
+            folder_path += "/"
+        if self.environment == "s3":
+            try:
+                if self.fs != None:
+                    with self.fs.open(folder_path + file_name,'wb') as f:
+                        if extension == "csv":
+                            df_input.to_csv(f,sep=sep,na_rep=na_rep,float_format=float_format,index=index,encoding=encoding)
+                            rslt = "Data successfully stored in s3 as: " + folder_path + file_name
+                else:
+                    rslt = "Could not connect with s3 because AWS CLI credentials have not been set yet."
+            except Exception as e:
+                rslt = str(e)
+                
+        else:
+            try:
+                if extension == "csv":
+                    df_input.to_csv(folder_path + file_name,sep=sep,na_rep=na_rep,float_format=float_format,index=index,encoding=encoding)
+                    rslt = "Data successfully stored locally as: " + folder_path + file_name
+            except Exception as e:
+                rslt = str(e)
+        return rslt
+                
+                
+
+                    
+                    
+    #__________________________________________________________________________
     def retrieve_object_name(self,objectInput:object)->str:
         '''
         ***
         Retrieves in a str, the name of the object provided.
         ***
         '''
         local_objects = inspect.currentframe().f_back.f_locals.items()
@@ -560,37 +640,15 @@
             fileKeys.append(obs.key)
         for fileKey in fileKeys:
             a=fileKey[::-1]
             ext='.'+fileKey.lower()[::-1].split('.')[0][::-1]
             thisFile=fileKey.replace(relativePath,'').replace('/','')
             these_files.add(thisFile)
         return these_files             
-    #__________________________________________________________________________ 
-    def store_api_staging_data(self,symbol:str)->Union[str,str]:
-        '''
-        ***
-        Description not available.
-        ***
-        '''
-        symbol = symbol.lower().strip()
-        s3FullPath,file_name = self.datetime_id_symbol_path(symbol,ext='json')
-        if self.environment.lower().strip() == 'local':
-            with open (self.api_key_path,'r') as input_file:
-                api_key = input_file.read()
-        else:
-            referenceName = self.api_key_path[::-1].split('/')[0][::-1]
-            s3FullFolderPath =  self.api_key_path.replace(referenceName,'')
-            api_key = self.get_s3_file_content(referenceName=referenceName,s3FullFolderPath=s3FullFolderPath)
-        this_url = self.alphavantage_config["cryptocurrencies"]["intraday"]["url"]\
-        .replace("@symbol",symbol).replace("@api_key",api_key)
-        data = requests.get(this_url).json()
-        self.standard_dict_to_json(jsonOrDictionary=data
-                                   ,fileName=file_name
-                                   ,folderPath=s3FullPath)
-        return file_name,s3FullPath
+
     #__________________________________________________________________________
     def consolidate_staging_data(self,symbol:str,date_id:int)->pd.DataFrame():
         '''
         ***
         Description not available.
         ***
         '''
```

### Comparing `cloudpy_org-1.2.5/cloudpy_org.egg-info/PKG-INFO` & `cloudpy_org-1.2.6/cloudpy_org.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: cloudpy-org
-Version: 1.2.5
+Version: 1.2.6
 Summary: Cloud data pipeline organization and automation library.
-Home-page: https://cloudpy.org/
+Home-page: https://www.cloudpy.org/
 Author: cloudpy.org
 Author-email: admin@cloudpy.org
 License: MIT
 Description: A library to programmatically create, interact, encrypt and automate your data pipelines making it simple to scale to the most popular cloud plattforms.
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cloudpy_org-1.2.5/setup.py` & `cloudpy_org-1.2.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 from os import path
 
 
 long_description = 'A library to programmatically create, interact, encrypt and automate your data pipelines making it simple to scale to the most popular cloud plattforms.'
 
 setup(
     name="cloudpy_org",
-    version="1.2.5",
+    version="1.2.6",
     description="Cloud data pipeline organization and automation library.",
     long_description_content_type="text/markdown",
     long_description=long_description,
-    url="https://cloudpy.org/",
+    url="https://www.cloudpy.org/",
     author="cloudpy.org",
     author_email="admin@cloudpy.org",
     license="MIT",
     classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
@@ -27,9 +27,9 @@
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Operating System :: OS Independent"
     ],
     packages=["cloudpy_org"],
     include_package_data=True,
-    install_requires=["pandas","pandasql","boto3","awswrangler","tqdm","numpy","cryptography"]
+    install_requires=["pandas","pandasql","boto3","awswrangler","tqdm","numpy","cryptography","s3fs"]
 )
```

