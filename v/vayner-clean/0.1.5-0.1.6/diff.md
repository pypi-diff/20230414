# Comparing `tmp/vayner_clean-0.1.5.tar.gz` & `tmp/vayner_clean-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vayner_clean-0.1.5.tar", last modified: Tue Mar 14 11:20:58 2023, max compression
+gzip compressed data, was "vayner_clean-0.1.6.tar", last modified: Fri Apr 14 08:57:55 2023, max compression
```

## Comparing `vayner_clean-0.1.5.tar` & `vayner_clean-0.1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-03-14 11:20:58.432298 vayner_clean-0.1.5/
--rw-r--r--   0 willbutler   (502) staff       (20)     1319 2023-03-14 11:20:58.432149 vayner_clean-0.1.5/PKG-INFO
--rw-r--r--   0 willbutler   (502) staff       (20)      623 2023-02-23 14:12:51.000000 vayner_clean-0.1.5/README.md
--rw-r--r--   0 willbutler   (502) staff       (20)       38 2023-03-14 11:20:58.432352 vayner_clean-0.1.5/setup.cfg
--rw-r--r--   0 willbutler   (502) staff       (20)     1314 2023-03-14 11:19:00.000000 vayner_clean-0.1.5/setup.py
-drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-03-14 11:20:58.431544 vayner_clean-0.1.5/vayner_clean.egg-info/
--rw-r--r--   0 willbutler   (502) staff       (20)     1319 2023-03-14 11:20:58.000000 vayner_clean-0.1.5/vayner_clean.egg-info/PKG-INFO
--rw-r--r--   0 willbutler   (502) staff       (20)      251 2023-03-14 11:20:58.000000 vayner_clean-0.1.5/vayner_clean.egg-info/SOURCES.txt
--rw-r--r--   0 willbutler   (502) staff       (20)        1 2023-03-14 11:20:58.000000 vayner_clean-0.1.5/vayner_clean.egg-info/dependency_links.txt
--rw-r--r--   0 willbutler   (502) staff       (20)       27 2023-03-14 11:20:58.000000 vayner_clean-0.1.5/vayner_clean.egg-info/requires.txt
--rw-r--r--   0 willbutler   (502) staff       (20)       10 2023-03-14 11:20:58.000000 vayner_clean-0.1.5/vayner_clean.egg-info/top_level.txt
-drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-03-14 11:20:58.431760 vayner_clean-0.1.5/vee_clean/
--rw-r--r--   0 willbutler   (502) staff       (20)        0 2023-02-23 14:12:51.000000 vayner_clean-0.1.5/vee_clean/__init__.py
--rw-r--r--   0 willbutler   (502) staff       (20)    16059 2023-03-14 11:16:36.000000 vayner_clean-0.1.5/vee_clean/cleaning_functions.py
+drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-04-14 08:57:55.620161 vayner_clean-0.1.6/
+-rw-r--r--   0 willbutler   (502) staff       (20)     1399 2023-04-14 08:57:55.620020 vayner_clean-0.1.6/PKG-INFO
+-rw-r--r--   0 willbutler   (502) staff       (20)      703 2023-03-14 11:27:46.000000 vayner_clean-0.1.6/README.md
+-rw-r--r--   0 willbutler   (502) staff       (20)       38 2023-04-14 08:57:55.620210 vayner_clean-0.1.6/setup.cfg
+-rw-r--r--   0 willbutler   (502) staff       (20)     1314 2023-04-14 08:57:46.000000 vayner_clean-0.1.6/setup.py
+drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-04-14 08:57:55.619430 vayner_clean-0.1.6/vayner_clean.egg-info/
+-rw-r--r--   0 willbutler   (502) staff       (20)     1399 2023-04-14 08:57:55.000000 vayner_clean-0.1.6/vayner_clean.egg-info/PKG-INFO
+-rw-r--r--   0 willbutler   (502) staff       (20)      251 2023-04-14 08:57:55.000000 vayner_clean-0.1.6/vayner_clean.egg-info/SOURCES.txt
+-rw-r--r--   0 willbutler   (502) staff       (20)        1 2023-04-14 08:57:55.000000 vayner_clean-0.1.6/vayner_clean.egg-info/dependency_links.txt
+-rw-r--r--   0 willbutler   (502) staff       (20)       27 2023-04-14 08:57:55.000000 vayner_clean-0.1.6/vayner_clean.egg-info/requires.txt
+-rw-r--r--   0 willbutler   (502) staff       (20)       10 2023-04-14 08:57:55.000000 vayner_clean-0.1.6/vayner_clean.egg-info/top_level.txt
+drwxr-xr-x   0 willbutler   (502) staff       (20)        0 2023-04-14 08:57:55.619662 vayner_clean-0.1.6/vee_clean/
+-rw-r--r--   0 willbutler   (502) staff       (20)        0 2023-02-23 14:12:51.000000 vayner_clean-0.1.6/vee_clean/__init__.py
+-rw-r--r--   0 willbutler   (502) staff       (20)    15751 2023-04-14 08:55:46.000000 vayner_clean-0.1.6/vee_clean/cleaning_functions.py
```

### Comparing `vayner_clean-0.1.5/PKG-INFO` & `vayner_clean-0.1.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vayner_clean
-Version: 0.1.5
+Version: 0.1.6
 Summary: Library for cleaning advertising data from Tracer
 Home-page: 
 Author: Will Butler
 Author-email: will.butler@vaynermedia.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -18,14 +18,16 @@
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # Getting Started 
 This library has generic functions for cleaning advertising data such as standardising column
 names between platforms and countries or extracting a Country like "France" from a string column
 
+[Full Online Documentation](https://VaynerMedia-London.github.io/vaynerclean/)
+
 ## Library Installation
 ```
 pip install vaynerclean
 ```
 To upgrade the library after an update
 ```
 pip install vayner-clean --upgrade
```

### Comparing `vayner_clean-0.1.5/README.md` & `vayner_clean-0.1.6/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Getting Started 
 This library has generic functions for cleaning advertising data such as standardising column
 names between platforms and countries or extracting a Country like "France" from a string column
 
+[Full Online Documentation](https://VaynerMedia-London.github.io/vaynerclean/)
+
 ## Library Installation
 ```
 pip install vaynerclean
 ```
 To upgrade the library after an update
 ```
 pip install vayner-clean --upgrade
```

### Comparing `vayner_clean-0.1.5/setup.py` & `vayner_clean-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="vayner_clean",
-    version="0.1.5",
+    version="0.1.6",
     description="Library for cleaning advertising data from Tracer",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     author="Will Butler",
     author_email="will.butler@vaynermedia.com",
     license="MIT",
```

### Comparing `vayner_clean-0.1.5/vayner_clean.egg-info/PKG-INFO` & `vayner_clean-0.1.6/vayner_clean.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vayner-clean
-Version: 0.1.5
+Version: 0.1.6
 Summary: Library for cleaning advertising data from Tracer
 Home-page: 
 Author: Will Butler
 Author-email: will.butler@vaynermedia.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -18,14 +18,16 @@
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # Getting Started 
 This library has generic functions for cleaning advertising data such as standardising column
 names between platforms and countries or extracting a Country like "France" from a string column
 
+[Full Online Documentation](https://VaynerMedia-London.github.io/vaynerclean/)
+
 ## Library Installation
 ```
 pip install vaynerclean
 ```
 To upgrade the library after an update
 ```
 pip install vayner-clean --upgrade
```

### Comparing `vayner_clean-0.1.5/vee_clean/cleaning_functions.py` & `vayner_clean-0.1.6/vee_clean/cleaning_functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,27 @@
 import pandas as pd
 import regex as re
 import logging
 import os
 import sys
 from unidecode import unidecode
+from veetility import utility_functions
 
 pickle_path = "Pickled Files/"
-
-logger = logging.getLogger('CleaningFunctions')
-if logger.hasHandlers():
-    logger.handlers = []
-if os.path.isdir('logs') == False:
-    os.mkdir('logs')
-logger.setLevel(logging.INFO)
-logger.addHandler(logging.StreamHandler(sys.stdout))
-formatter = logging.Formatter('%(levelname)s %(asctime)s - %(message)s')
-
-file_handler = logging.FileHandler(f'./logs/CleaningFunctions.log')
-file_handler.setFormatter(formatter)
-logger.addHandler(file_handler)
-
+cleaning_logger = utility_functions.Logger('Indeed','CleaningFunctions')
 # %% -----------------------------
 # Emojis to clean out of copy messages
 # -----------------------------
 emoji_pattern = re.compile("["
                            u"\U0001F600-\U0001F64F"  # emoticons
                            u"\U0001F300-\U0001F5FF"  # symbols & pictographs
                            u"\U0001F680-\U0001F6FF"  # transport & map symbols
                            u"\U0001F1E0-\U0001F1FF"  # flags (iOS)
                            "]+", flags=re.UNICODE)
 
-
-
 def clean_column_names(df, hardcode_col_dict = {},errors= 'ignore',cols_no_change = ['spend', 'date', 'currency', 
                             'cohort', 'creative_name', 'group_id', 'engagements', 'created',
                             'plays', 'saved', 'post_hastags', 'content_type', 'linked_content', 'post_id',
                             'video_duration', 'average_time_watched', 'total_time_watched',
                             'adset_targeting', 'completion_rate', 'targeting', 'cohort_new',
                             'video_completions', 'post_hashtags']):
 
@@ -84,15 +70,15 @@
             column = 'creative_name'
         elif ('video' in column) and ('impression' in column):                       
             column = 'video_impressions'
         elif ('shares' in column) or ('retweet' in column):
             column = 'shares'
         elif (('conversion' in column) or ('lifetime'in column)) and ('save' in column): #_1d_click_onsite_conversion_post_save in fb_ig_paid data
             column = 'saved'
-        elif ('video' in column) and (('100' in column) or ('complete' in column) or('full' in column)):
+        elif ('video' in column) and (('100' in column) or ('complet' in column) or('full' in column)):
             column = 'video_completions'
         elif ('video' in column) and ('view' in column) and ('0' not in column) and ('5' not in column): #don't include columsn with 25,50,75% completion
             column = 'video_views'
         elif ('organic' in column) and ('boosted' in column) or ( 'workstream' in column):
             column = 'workstream'
         elif 'currency' in column:
             column = 'currency'
@@ -122,19 +108,19 @@
             column = 'media_type'
         elif('cohort' in column):
             column = 'cohort'
         else:
             message = f'Column "{column}" is not handled in column cleaning function'
             if errors == 'raise':
                 raise Exception(message)
-            logger.info(message)
+            cleaning_logger.logger.info(message)
 
         new_columns.append(column)
     if len(new_columns) != len(set(new_columns)):
-        logger.exception(f'Duplicate column names found {sorted(new_columns)}')
+        cleaning_logger.logger.exception(f'Duplicate column names found {sorted(new_columns)}')
         raise ValueError
     df.columns = new_columns
 
     return df
 
 def extract_country_from_string(string, client_name, hardcode_dict):
     """Converts a string containing info identifying a certain
```

