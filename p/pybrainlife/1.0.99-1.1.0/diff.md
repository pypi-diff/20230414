# Comparing `tmp/pybrainlife-1.0.99.tar.gz` & `tmp/pybrainlife-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybrainlife-1.0.99.tar", max compression
+gzip compressed data, was "pybrainlife-1.1.0.tar", max compression
```

## Comparing `pybrainlife-1.0.99.tar` & `pybrainlife-1.1.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2370 2023-02-13 20:00:45.821811 pybrainlife-1.0.99/README.md
--rw-r--r--   0        0        0       22 2023-02-13 15:57:42.245812 pybrainlife-1.0.99/pybrainlife/__init__.py
--rwxr-xr-x   0        0        0    18114 2023-04-12 18:47:32.386736 pybrainlife-1.0.99/pybrainlife/data/collect.py
--rwxr-xr-x   0        0        0    19287 2023-04-12 21:52:50.584436 pybrainlife-1.0.99/pybrainlife/data/manipulate.py
--rw-r--r--   0        0        0     4011 2023-02-13 15:57:42.245812 pybrainlife-1.0.99/pybrainlife/vis/__pycache__/data.cpython-38.pyc
--rw-r--r--   0        0        0     7091 2023-02-13 15:57:42.245812 pybrainlife-1.0.99/pybrainlife/vis/__pycache__/plots.cpython-38.pyc
--rwxr-xr-x   0        0        0    19483 2023-02-13 19:55:42.426571 pybrainlife-1.0.99/pybrainlife/vis/plots.py
--rw-r--r--   0        0        0      748 2023-04-12 21:52:58.620415 pybrainlife-1.0.99/pyproject.toml
--rw-r--r--   0        0        0     3489 1970-01-01 00:00:00.000000 pybrainlife-1.0.99/setup.py
--rw-r--r--   0        0        0     3427 1970-01-01 00:00:00.000000 pybrainlife-1.0.99/PKG-INFO
+-rw-r--r--   0        0        0     2370 2023-02-13 20:00:45.821811 pybrainlife-1.1.0/README.md
+-rw-r--r--   0        0        0       22 2023-02-13 15:57:42.245812 pybrainlife-1.1.0/pybrainlife/__init__.py
+-rwxr-xr-x   0        0        0    19061 2023-04-14 16:41:38.884617 pybrainlife-1.1.0/pybrainlife/data/collect.py
+-rwxr-xr-x   0        0        0    19287 2023-04-12 21:52:50.584436 pybrainlife-1.1.0/pybrainlife/data/manipulate.py
+-rw-r--r--   0        0        0     4011 2023-02-13 15:57:42.245812 pybrainlife-1.1.0/pybrainlife/vis/__pycache__/data.cpython-38.pyc
+-rw-r--r--   0        0        0     7091 2023-02-13 15:57:42.245812 pybrainlife-1.1.0/pybrainlife/vis/__pycache__/plots.cpython-38.pyc
+-rwxr-xr-x   0        0        0    19483 2023-02-13 19:55:42.426571 pybrainlife-1.1.0/pybrainlife/vis/plots.py
+-rw-r--r--   0        0        0      747 2023-04-14 16:42:26.952514 pybrainlife-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3488 1970-01-01 00:00:00.000000 pybrainlife-1.1.0/setup.py
+-rw-r--r--   0        0        0     3426 1970-01-01 00:00:00.000000 pybrainlife-1.1.0/PKG-INFO
```

### Comparing `pybrainlife-1.0.99/README.md` & `pybrainlife-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pybrainlife-1.0.99/pybrainlife/data/collect.py` & `pybrainlife-1.1.0/pybrainlife/data/collect.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,46 +25,57 @@
     
     if 'datatype_tags' not in data.keys():
         data['datatype_tags'] = [ dtags for f in range(len(data)) ]
         
     return data
 
 ## this will add a subjectID and sessionID column to the output data
-def add_subjects_sessions(subject,session,path,data):
+def add_subjects_sessions(subject,session,data):
     
     if 'subjectID' not in data.keys():
         data['subjectID'] = [ str(subject) for f in range(len(data)) ]
     
     if 'sessionID' not in data.keys():
         data['sessionID'] = [ str(session) for f in range(len(data)) ]
         
     return data
 
+## this will add a finish date column to the output data
+def add_finish_dates(finish_date,data):
+    
+    if 'finish_dates' not in data.keys():
+        data['finish_dates'] = [ finish_date for f in range(len(data)) ]
+        
+    return data
+
 ## this function calles check_for_duplicates and attempts to find duplicates. then uses that output, sets a dumby sessionID if not present,
 ## and appends the object data
-def append_data(subjects,sessions,paths,finish_dates,obj,filename,obj_tags,obj_datatype_tags):
+def append_data(subjects,sessions,paths,finish_dates,obj,filename,obj_tags,obj_datatype_tags,duplicates):
         
     # check for duplicates. if so, remove
-    finish_dates, subjects, sessions, paths, obj_tags, obj_datatype_tags = check_for_duplicates(obj,finish_dates,subjects,sessions,paths,obj_tags,obj_datatype_tags)
-
-    # append data to appropriate lists
-    subjects = np.append(subjects,str(obj['output']['meta']['subject']))
-    if 'session' in obj['output']['meta'].keys():
-        sessions = np.append(sessions,obj['output']['meta']['session'])
-    else:
-        sessions = np.append(sessions,'1')
-    paths = np.append(paths,"input/"+obj["path"]+"/"+filename)
-    finish_dates = np.append(finish_dates,obj['finish_date'])
-    obj_datatype_tags = obj_datatype_tags + [obj['output']['datatype_tags']]
-    obj_tags = obj_tags + [obj['output']['tags']]
+    skip = 0
+    if duplicates:
+        finish_dates, subjects, sessions, paths, obj_tags, obj_datatype_tags, skip = check_for_duplicates(obj,finish_dates,subjects,sessions,paths,obj_tags,obj_datatype_tags)
+
+    if skip == 0:
+        # append data to appropriate lists
+        subjects = np.append(subjects,str(obj['output']['meta']['subject']))
+        if 'session' in obj['output']['meta'].keys():
+            sessions = np.append(sessions,obj['output']['meta']['session'])
+        else:
+            sessions = np.append(sessions,'1')
+        paths = np.append(paths,"input/"+obj["path"]+"/"+filename)
+        finish_dates = np.append(finish_dates,obj['finish_date'])
+        obj_datatype_tags = obj_datatype_tags + [obj['output']['datatype_tags']]
+        obj_tags = obj_tags + [obj['output']['tags']]
     
     return finish_dates, subjects, sessions, paths, obj_tags, obj_datatype_tags
 
 ## this function will call add_subjects_sessions to add the appropriate columns and will append the object data to a study-wide dataframe
-def compile_data(paths,subjects,sessions,data,dtags,tags):
+def compile_data(paths,subjects,sessions,data,dtags,tags,finish_dates):
     # loops through all paths
     for i in range(len(paths)):
         # if network, use igraph and pandas. if not, use just pandas
         if 'network.json.gz' in paths[i]:
             # tmpdata = pd.read_json(paths[i],orient='index').reset_index(drop=True)
             tmpdata = pd.DataFrame()
             tmpdata['igraph'] = jgf.igraph.load(paths[i],compressed=True)
@@ -72,16 +83,17 @@
             # tmpdata = add_tags_dtags(tags[i],dtags[i],tmpdata) # added 4/12/2023
         else:
             if '.tsv' in paths[i]:
                 sep = '\t'
             else:
                 sep = ','
             tmpdata = pd.read_csv(paths[i],sep=sep)
-        tmpdata = add_subjects_sessions(subjects[i],sessions[i],paths[i],tmpdata)
+        tmpdata = add_subjects_sessions(subjects[i],sessions[i],tmpdata)
         tmpdata = add_tags_dtags(tags[i],dtags[i],tmpdata)
+        tmpdata = add_finish_dates(finish_dates[i],tmpdata)
 
         #data = data.append(tmpdata,ignore_index=True)
         data = pd.concat([data,tmpdata])
 
     # replace empty spaces with nans
     data = data.replace(r'^\s+$', np.nan, regex=True)
     
@@ -100,15 +112,15 @@
 ### load data
 ## this function is useful for identifying duplicate datatypes. if it finds one, it will update the data with the latest finishing dataset.
 def check_for_duplicates(obj,finish_dates,subjects,sessions,paths,obj_tags,obj_datatype_tags):
     
     # first checks if there is a session id available in the keys of the object. if finds one, then checks if the subject and session ID 
     # were already looped over. if so, will delete position in list and update with appropriate path. if it doesn't find a session ID, it
     # just attempts to find if the subject has already been looped over
-    
+    skip=0
     if 'session' in obj['output']['meta'].keys():
         if (obj['output']['meta']['subject'] in subjects) and (obj['output']['meta']['session'] in sessions):
             index = np.where(np.logical_and(subjects == obj['output']['meta']['subject'],sessions == obj['output']['meta']['session']))
             index_identified = True
         else:
             index_identified = False
     else:
@@ -117,20 +129,21 @@
             index = np.where(subjects == obj['output']['meta']['subject'])
             index_identified = True
         else:
             index_identified = False
     
     if index_identified == True:
         if len(index[0]) > 1:
-            finish_dates, subjects, sessions, paths, obj_tags, obj_datatype_tags = remove_duplicates(index,obj,subjects,sessions,paths,finish_dates,obj_tags,obj_datatype_tags)
+            finish_dates, subjects, sessions, paths, obj_tags, obj_datatype_tags, skip = remove_duplicates(index,obj,subjects,sessions,paths,finish_dates,obj_tags,obj_datatype_tags)
 
-    return finish_dates, subjects, sessions, paths, obj_tags, obj_datatype_tags
+    return finish_dates, subjects, sessions, paths, obj_tags, obj_datatype_tags, skip
 
 def remove_duplicates(index,obj,subjects,sessions,paths,finish_dates,obj_tags,obj_datatype_tags):
     
+    skip = 0
     # are the datatype tags the same
     tmp_datatype_tags = [ obj_datatype_tags[f] for f in list(index[0]) ]
     duplicate_datatype_tags_index = [ index[0][f] for f in range(len(list(index[0]))) if tmp_datatype_tags[f] == obj['output']['datatype_tags'] ]
 
     if len(duplicate_datatype_tags_index) > 0:
         duplicate_datatype_tags = True
     else:
@@ -144,16 +157,26 @@
         duplicate_tags = True
     else:
         duplicate_tags = False
 
     # if yes to both above, check for finish dates
     if duplicate_tags == True and duplicate_datatype_tags == True:
         duplicate_index = list(set(duplicate_tags_index) & set(duplicate_datatype_tags_index))
+        if obj['finish_date'] >= finish_dates[duplicate_index]:
+            finish_dates = np.delete(finish_dates,duplicate_index)
+            subjects = np.delete(subjects,duplicate_index)
+            sessions = np.delete(sessions,duplicate_index)
+            paths = np.delete(paths,duplicate_index)
+            del obj_tags[duplicate_index[0]]
+            del obj_datatype_tags[duplicate_index[0]]
+            skip = 0
+        else:
+            skip = 1
             
-    return finish_dates, subjects, sessions, paths, obj_tags, obj_datatype_tags
+    return finish_dates, subjects, sessions, paths, obj_tags, obj_datatype_tags, skip
     
 # this will check to see if the datatype tags or tags of the datatype object exists within the filtered ('!') tags
 def check_for_filter_tags(input_tags,obj,tagOrDatatypeTag):
     
     filter_checks = 0
     for i in input_tags:
         if i.replace('!','') not in obj['output'][tagOrDatatypeTag]:
@@ -170,15 +193,15 @@
         if i in obj['output'][tagOrDatatypeTag]:
             ctr=ctr+1
     
     return ctr
 
 ## this function is the wrapper function that calls all the prevouis functions to generate a dataframe for the entire project of the appropriate datatype
 # def collect_data(datatype,datatype_tags,tags,filename,outPath,net_adj): # net_adj no longer necessary
-def collect_data(datatype,datatype_tags,tags,filename,outPath):
+def collect_data(datatype,datatype_tags,tags,filename,outPath,duplicates=False):
 
     # grab path and data objects
     objects = requests.get('https://brainlife.io/api/warehouse/secondary/list/%s'%os.environ['PROJECT_ID']).json()
 
     # subjects and paths
     subjects = []
     sessions = []
@@ -245,30 +268,29 @@
                             tag_filter = False
                 else:
                     tag_filter = False
             else:
                 tag_filter = True
 
             if datatype_tag_filter == True & tag_filter == True:
-                finish_dates, subjects, sessions, paths, obj_tags, obj_datatype_tags = append_data(subjects,sessions,paths,finish_dates,obj,filename,obj_tags,obj_datatype_tags)
-
+                finish_dates, subjects, sessions, paths, obj_tags, obj_datatype_tags = append_data(subjects,sessions,paths,finish_dates,obj,filename,obj_tags,obj_datatype_tags,duplicates)
     # check if tab separated or comma separated by looking at input filename
     if '.tsv' in filename:
         sep = '\t'
     else:
         sep = ','
 
     # compile data
     # if net_adj:
     #     data = {}
     #     data = compile_network_adjacency_matrices(paths,subjects,sessions,data)
     #     if outPath:
     #         np.save(outPath,data)
     # else:
-    data = compile_data(paths,subjects,sessions,data,obj_datatype_tags,obj_tags)
+    data = compile_data(paths,subjects,sessions,data,obj_datatype_tags,obj_tags,finish_dates)
 
     # output data structure for records and any further analyses
     if outPath:
         data.to_csv(outPath,sep=sep,index=False)
 
     return data, obj_tags, obj_datatype_tags
```

### Comparing `pybrainlife-1.0.99/pybrainlife/data/manipulate.py` & `pybrainlife-1.1.0/pybrainlife/data/manipulate.py`

 * *Files identical despite different names*

### Comparing `pybrainlife-1.0.99/pybrainlife/vis/__pycache__/data.cpython-38.pyc` & `pybrainlife-1.1.0/pybrainlife/vis/__pycache__/data.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pybrainlife-1.0.99/pybrainlife/vis/__pycache__/plots.cpython-38.pyc` & `pybrainlife-1.1.0/pybrainlife/vis/__pycache__/plots.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pybrainlife-1.0.99/pybrainlife/vis/plots.py` & `pybrainlife-1.1.0/pybrainlife/vis/plots.py`

 * *Files identical despite different names*

### Comparing `pybrainlife-1.0.99/pyproject.toml` & `pybrainlife-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pybrainlife"
-version = "1.0.99"
+version = "1.1.0"
 description = "This project is a collection of functions that are useful for analyzing MRI data derivatives generated on brainlife.io"
 authors = ["Brad Caron <bacaron245@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/brainlife/pybrainlife"
 repository = "https://github.com/brainlife/pybrainlife"
 keywords = ["brainlife"]
```

### Comparing `pybrainlife-1.0.99/setup.py` & `pybrainlife-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'requests>=2.28.1,<3.0.0',
  'scikit-learn>=1.0.2,<2.0.0',
  'scipy>=1.8.0,<2.0.0',
  'seaborn>=0.12.2,<0.13.0']
 
 setup_kwargs = {
     'name': 'pybrainlife',
-    'version': '1.0.99',
+    'version': '1.1.0',
     'description': 'This project is a collection of functions that are useful for analyzing MRI data derivatives generated on brainlife.io',
     'long_description': '[![Abcdspec-compliant](https://img.shields.io/badge/ABCD_Spec-v1.1-green.svg)](https://github.com/soichih/abcd-spec)\n\n# pybrainlife\nThis repository contains the python package for collecting, collating, manipulating, analyzing, and visualizing MRI data generated on brainlife.io. Designed to used within the brainlife.io Analysis tab Jupyter notebooks, can be installed as a pypi package to your local machine.\n\n### Authors\n- Brad Caron (bacaron@iu.edu)\n\n### Contributors\n- Soichi Hayashi (hayashi@iu.edu)\n- Franco Pestilli (franpest@indiana.edu)\n\n### Funding\n[![NSF-BCS-1734853](https://img.shields.io/badge/NSF_BCS-1734853-blue.svg)](https://nsf.gov/awardsearch/showAward?AWD_ID=1734853)\n[![NSF-BCS-1636893](https://img.shields.io/badge/NSF_BCS-1636893-blue.svg)](https://nsf.gov/awardsearch/showAward?AWD_ID=1636893)\n\n### Citations\n\nPlease cite the following articles when publishing papers that used data, code or other resources created by the brainlife.io community.\n\n1. Avesani, P., McPherson, B., Hayashi, S. et al. The open diffusion data derivatives, brain data upcycling via integrated publishing of derivatives and reproducible open cloud services. Sci Data 6, 69 (2019). https://doi.org/10.1038/s41597-019-0073-y\n\n### Directory structure\n```\npybrainlife\n├── dist\n│\xa0\xa0 ├── pybrainlife-1.0.0-py3-none-any.whl\n│\xa0\xa0 └── pybrainlife-1.0.0.tar.gz\n├── poetry.lock\n├── pybrainlife\n│\xa0\xa0 ├── data\n│\xa0\xa0 │\xa0\xa0 ├── collect.py\n│\xa0\xa0 │\xa0\xa0 └── manipulate.py\n│\xa0\xa0 ├── __init__.py\n│\xa0\xa0 └── vis\n│\xa0\xa0     ├── plots.py\n│\xa0\xa0     └── __pycache__\n│\xa0\xa0         ├── data.cpython-38.pyc\n│\xa0\xa0         └── plots.cpython-38.pyc\n├── pyproject.toml\n├── README.md\n└── tests\n    ├── __init__.py\n    └── test_pybrainlife.py\n```\n\n### Installing locally\nThis package can be installed locally via PyPi using the following command:\n\n```\npip install pybrainlife\n```\n\n### Dependencies\n\nThis package requires the following libraries.\n  - python = "3.8"\n  - numpy = "^1.9.3"\n  - bctpy = "^0.5.2"\n  - seaborn = "^0.11.2"\n  - jgf = "^0.2.2"\n  - scikit-learn = "^1.0.2"\n  - pandas = "^1.4.2"\n  - scipy = "^1.8.0"\n  - requests = "^2.27.1"\n\nLibrary of Modules for Loading Data and Analyzing Data from brainlife.io\n\n2022 The University of Texas at Austin\n',
     'author': 'Brad Caron',
     'author_email': 'bacaron245@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/brainlife/pybrainlife',
```

### Comparing `pybrainlife-1.0.99/PKG-INFO` & `pybrainlife-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybrainlife
-Version: 1.0.99
+Version: 1.1.0
 Summary: This project is a collection of functions that are useful for analyzing MRI data derivatives generated on brainlife.io
 Home-page: https://github.com/brainlife/pybrainlife
 Keywords: brainlife
 Author: Brad Caron
 Author-email: bacaron245@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
```

