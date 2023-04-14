# Comparing `tmp/vaynerqualityassessments-0.1.8.tar.gz` & `tmp/vaynerqualityassessments-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vaynerqualityassessments-0.1.8.tar", last modified: Wed Feb  8 17:14:33 2023, max compression
+gzip compressed data, was "vaynerqualityassessments-0.1.9.tar", last modified: Wed Feb  8 18:26:51 2023, max compression
```

## Comparing `vaynerqualityassessments-0.1.8.tar` & `vaynerqualityassessments-0.1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-02-08 17:14:33.282785 vaynerqualityassessments-0.1.8/
--rw-r--r--   0 willbutler   (502) staff       (20)     2019 2023-02-08 17:14:33.282567 vaynerqualityassessments-0.1.8/PKG-INFO
--rw-r--r--   0 willbutler   (502) staff       (20)     1316 2023-01-31 09:02:15.000000 vaynerqualityassessments-0.1.8/README.md
--rw-r--r--   0 willbutler   (502) staff       (20)       38 2023-02-08 17:14:33.282845 vaynerqualityassessments-0.1.8/setup.cfg
--rw-r--r--   0 willbutler   (502) staff       (20)     1478 2023-02-08 17:14:12.000000 vaynerqualityassessments-0.1.8/setup.py
-drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-02-08 17:14:33.281578 vaynerqualityassessments-0.1.8/vaynerqualityassessments.egg-info/
--rw-r--r--   0 willbutler   (502) staff       (20)     2019 2023-02-08 17:14:32.000000 vaynerqualityassessments-0.1.8/vaynerqualityassessments.egg-info/PKG-INFO
--rw-r--r--   0 willbutler   (502) staff       (20)      306 2023-02-08 17:14:33.000000 vaynerqualityassessments-0.1.8/vaynerqualityassessments.egg-info/SOURCES.txt
--rw-r--r--   0 willbutler   (502) staff       (20)        1 2023-02-08 17:14:32.000000 vaynerqualityassessments-0.1.8/vaynerqualityassessments.egg-info/dependency_links.txt
--rw-r--r--   0 willbutler   (502) staff       (20)       38 2023-02-08 17:14:33.000000 vaynerqualityassessments-0.1.8/vaynerqualityassessments.egg-info/requires.txt
--rw-r--r--   0 willbutler   (502) staff       (20)        7 2023-02-08 17:14:33.000000 vaynerqualityassessments-0.1.8/vaynerqualityassessments.egg-info/top_level.txt
-drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-02-08 17:14:33.281952 vaynerqualityassessments-0.1.8/vee_qa/
--rw-r--r--   0 willbutler   (502) staff       (20)        0 2023-01-31 09:02:15.000000 vaynerqualityassessments-0.1.8/vee_qa/__init__.py
--rw-r--r--   0 willbutler   (502) staff       (20)    23063 2023-02-08 17:13:17.000000 vaynerqualityassessments-0.1.8/vee_qa/quality_assessments.py
+drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-02-08 18:26:51.048844 vaynerqualityassessments-0.1.9/
+-rw-r--r--   0 willbutler   (502) staff       (20)     2019 2023-02-08 18:26:51.048542 vaynerqualityassessments-0.1.9/PKG-INFO
+-rw-r--r--   0 willbutler   (502) staff       (20)     1316 2023-01-31 09:02:15.000000 vaynerqualityassessments-0.1.9/README.md
+-rw-r--r--   0 willbutler   (502) staff       (20)       38 2023-02-08 18:26:51.049187 vaynerqualityassessments-0.1.9/setup.cfg
+-rw-r--r--   0 willbutler   (502) staff       (20)     1478 2023-02-08 18:26:46.000000 vaynerqualityassessments-0.1.9/setup.py
+drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-02-08 18:26:51.046666 vaynerqualityassessments-0.1.9/vaynerqualityassessments.egg-info/
+-rw-r--r--   0 willbutler   (502) staff       (20)     2019 2023-02-08 18:26:50.000000 vaynerqualityassessments-0.1.9/vaynerqualityassessments.egg-info/PKG-INFO
+-rw-r--r--   0 willbutler   (502) staff       (20)      306 2023-02-08 18:26:51.000000 vaynerqualityassessments-0.1.9/vaynerqualityassessments.egg-info/SOURCES.txt
+-rw-r--r--   0 willbutler   (502) staff       (20)        1 2023-02-08 18:26:50.000000 vaynerqualityassessments-0.1.9/vaynerqualityassessments.egg-info/dependency_links.txt
+-rw-r--r--   0 willbutler   (502) staff       (20)       38 2023-02-08 18:26:50.000000 vaynerqualityassessments-0.1.9/vaynerqualityassessments.egg-info/requires.txt
+-rw-r--r--   0 willbutler   (502) staff       (20)        7 2023-02-08 18:26:50.000000 vaynerqualityassessments-0.1.9/vaynerqualityassessments.egg-info/top_level.txt
+drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-02-08 18:26:51.047162 vaynerqualityassessments-0.1.9/vee_qa/
+-rw-r--r--   0 willbutler   (502) staff       (20)        0 2023-01-31 09:02:15.000000 vaynerqualityassessments-0.1.9/vee_qa/__init__.py
+-rw-r--r--   0 willbutler   (502) staff       (20)    23389 2023-02-08 18:09:56.000000 vaynerqualityassessments-0.1.9/vee_qa/quality_assessments.py
```

### Comparing `vaynerqualityassessments-0.1.8/PKG-INFO` & `vaynerqualityassessments-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vaynerqualityassessments
-Version: 0.1.8
+Version: 0.1.9
 Summary: Quality assessment functions for Tracer Data
 Home-page: 
 Author: Will Butler
 Author-email: will.butler@vaynermedia.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `vaynerqualityassessments-0.1.8/README.md` & `vaynerqualityassessments-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `vaynerqualityassessments-0.1.8/setup.py` & `vaynerqualityassessments-0.1.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="vaynerqualityassessments",
-    version="0.1.8",
+    version="0.1.9",
     description="Quality assessment functions for Tracer Data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     author="Will Butler",
     author_email="will.butler@vaynermedia.com",
     license="MIT",
```

### Comparing `vaynerqualityassessments-0.1.8/vaynerqualityassessments.egg-info/PKG-INFO` & `vaynerqualityassessments-0.1.9/vaynerqualityassessments.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vaynerqualityassessments
-Version: 0.1.8
+Version: 0.1.9
 Summary: Quality assessment functions for Tracer Data
 Home-page: 
 Author: Will Butler
 Author-email: will.butler@vaynermedia.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `vaynerqualityassessments-0.1.8/vee_qa/quality_assessments.py` & `vaynerqualityassessments-0.1.9/vee_qa/quality_assessments.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,16 @@
 
         if output_method == 'gsheet':
             self.util.write_to_gsheet(gsheet_name,tab_name,null_count_df)
         elif output_method == 'Dataframe': 
             return null_count_df
     
     def check_data_recency(self,df,cols_to_group,gsheet_name,tab_name='DataRecency',
-                            three_days_for_monday= True,date_col='date'):
+                            three_days_for_monday= True,date_col='date',
+                            dayfirst='EnterValue',yearfirst='EnterValue',format=None,errors='raise'):
         """Post a google sheet showing how many days since different channels have been active.
         Also return a list of channels that have been inactive for more than 2 days which
         might be indicative of an error
         
         Args:
             df (pandas.DataFrame): Dataframe of data containing a 'date' column
             cols_to_group (list or str): Columns to groupby effectively creating the 'channels'
@@ -86,14 +87,18 @@
             error_message (str): String error message describing which channels are recently inactive. This message can then be sent
                                 to a slack function"""
 
         error_message = ''
         organic_or_paid = self.util.identify_paid_or_organic(df)
         print(organic_or_paid)
         buffer_days_since_active = 2
+        #remove any timezone information from the date_col
+        df[date_col] = pd.to_datetime(df[date_col].dt.date,dayfirst=dayfirst,
+                                      yearfirst=yearfirst,format=format,errors=errors)
+
         data_recency = pd.DataFrame(df.groupby(cols_to_group)[date_col].max().apply(lambda x: (today - x).days)).reset_index().rename(columns={date_col:'DaysSinceActive'})  
     
         self.util.write_to_gsheet(gsheet_name,tab_name,data_recency,sheet_prefix=organic_or_paid)
 
         #create a tag string to identify a channel, a concatenation of all the column values specified in 'cols_to_group'
         def concat_cols(x):
             result=''
```

