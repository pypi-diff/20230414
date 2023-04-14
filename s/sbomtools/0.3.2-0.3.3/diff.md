# Comparing `tmp/sbomtools-0.3.2.tar.gz` & `tmp/sbomtools-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sbomtools-0.3.2.tar", last modified: Fri Feb  4 12:24:54 2022, max compression
+gzip compressed data, was "sbomtools-0.3.3.tar", last modified: Fri Apr 14 13:17:19 2023, max compression
```

## Comparing `sbomtools-0.3.2.tar` & `sbomtools-0.3.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 elear      (501) staff       (20)        0 2022-02-04 12:24:54.664644 sbomtools-0.3.2/
--rw-r--r--   0 elear      (501) staff       (20)     1542 2022-01-24 11:44:55.000000 sbomtools-0.3.2/LICENSE.txt
--rw-r--r--   0 elear      (501) staff       (20)     4690 2022-02-04 12:24:54.664795 sbomtools-0.3.2/PKG-INFO
--rw-r--r--   0 elear      (501) staff       (20)     4379 2022-02-01 09:55:32.000000 sbomtools-0.3.2/README.md
--rw-r--r--   0 elear      (501) staff       (20)       90 2022-01-24 11:44:42.000000 sbomtools-0.3.2/pyproject.toml
-drwxr-xr-x   0 elear      (501) staff       (20)        0 2022-02-04 12:24:54.662518 sbomtools-0.3.2/sbomtools/
--rw-r--r--   0 elear      (501) staff       (20)      217 2022-01-31 12:11:57.000000 sbomtools-0.3.2/sbomtools/__init__.py
--rw-r--r--   0 elear      (501) staff       (20)      106 2022-01-31 12:10:42.000000 sbomtools-0.3.2/sbomtools/constants.py
--rw-r--r--   0 elear      (501) staff       (20)     5009 2022-02-01 09:55:32.000000 sbomtools-0.3.2/sbomtools/cyclonedx.py
--rw-r--r--   0 elear      (501) staff       (20)      602 2022-01-28 10:20:18.000000 sbomtools-0.3.2/sbomtools/exceptions.py
--rw-r--r--   0 elear      (501) staff       (20)      981 2022-02-04 10:26:04.000000 sbomtools-0.3.2/sbomtools/grep.py
--rw-r--r--   0 elear      (501) staff       (20)     1134 2022-01-28 10:33:55.000000 sbomtools-0.3.2/sbomtools/remove.py
--rw-r--r--   0 elear      (501) staff       (20)     2648 2022-02-04 10:44:34.000000 sbomtools-0.3.2/sbomtools/sbomgrep.py
--rw-r--r--   0 elear      (501) staff       (20)     2598 2022-02-04 10:43:41.000000 sbomtools-0.3.2/sbomtools/sbomls.py
--rw-r--r--   0 elear      (501) staff       (20)     1583 2022-01-31 18:05:42.000000 sbomtools-0.3.2/sbomtools/sbomrm.py
--rw-r--r--   0 elear      (501) staff       (20)     2372 2022-01-31 13:06:34.000000 sbomtools-0.3.2/sbomtools/sbomupdate.py
--rw-r--r--   0 elear      (501) staff       (20)     6332 2022-02-01 09:55:32.000000 sbomtools-0.3.2/sbomtools/spdx.py
--rw-r--r--   0 elear      (501) staff       (20)     1373 2022-01-28 10:43:39.000000 sbomtools-0.3.2/sbomtools/update.py
-drwxr-xr-x   0 elear      (501) staff       (20)        0 2022-02-04 12:24:54.664321 sbomtools-0.3.2/sbomtools.egg-info/
--rw-r--r--   0 elear      (501) staff       (20)     4690 2022-02-04 12:24:54.000000 sbomtools-0.3.2/sbomtools.egg-info/PKG-INFO
--rw-r--r--   0 elear      (501) staff       (20)      477 2022-02-04 12:24:54.000000 sbomtools-0.3.2/sbomtools.egg-info/SOURCES.txt
--rw-r--r--   0 elear      (501) staff       (20)        1 2022-02-04 12:24:54.000000 sbomtools-0.3.2/sbomtools.egg-info/dependency_links.txt
--rw-r--r--   0 elear      (501) staff       (20)      151 2022-02-04 12:24:54.000000 sbomtools-0.3.2/sbomtools.egg-info/entry_points.txt
--rw-r--r--   0 elear      (501) staff       (20)       10 2022-02-04 12:24:54.000000 sbomtools-0.3.2/sbomtools.egg-info/top_level.txt
--rw-r--r--   0 elear      (501) staff       (20)      548 2022-02-04 12:24:54.665513 sbomtools-0.3.2/setup.cfg
--rw-r--r--   0 elear      (501) staff       (20)       38 2022-01-24 11:44:48.000000 sbomtools-0.3.2/setup.py
+drwxr-xr-x   0 elear      (501) staff       (20)        0 2023-04-14 13:17:19.180206 sbomtools-0.3.3/
+-rw-r--r--   0 elear      (501) staff       (20)     1542 2022-01-24 11:44:55.000000 sbomtools-0.3.3/LICENSE.txt
+-rw-r--r--   0 elear      (501) staff       (20)     4670 2023-04-14 13:17:19.180397 sbomtools-0.3.3/PKG-INFO
+-rw-r--r--   0 elear      (501) staff       (20)     4379 2022-02-01 09:55:32.000000 sbomtools-0.3.3/README.md
+-rw-r--r--   0 elear      (501) staff       (20)       90 2022-01-24 11:44:42.000000 sbomtools-0.3.3/pyproject.toml
+drwxr-xr-x   0 elear      (501) staff       (20)        0 2023-04-14 13:17:19.176476 sbomtools-0.3.3/sbomtools/
+-rw-r--r--   0 elear      (501) staff       (20)      217 2022-01-31 12:11:57.000000 sbomtools-0.3.3/sbomtools/__init__.py
+-rw-r--r--   0 elear      (501) staff       (20)      106 2022-01-31 12:10:42.000000 sbomtools-0.3.3/sbomtools/constants.py
+-rw-r--r--   0 elear      (501) staff       (20)     5009 2022-02-01 09:55:32.000000 sbomtools-0.3.3/sbomtools/cyclonedx.py
+-rw-r--r--   0 elear      (501) staff       (20)      602 2022-01-28 10:20:18.000000 sbomtools-0.3.3/sbomtools/exceptions.py
+-rw-r--r--   0 elear      (501) staff       (20)      981 2022-02-04 10:26:04.000000 sbomtools-0.3.3/sbomtools/grep.py
+-rw-r--r--   0 elear      (501) staff       (20)     1134 2022-01-28 10:33:55.000000 sbomtools-0.3.3/sbomtools/remove.py
+-rw-r--r--   0 elear      (501) staff       (20)     2852 2023-04-14 11:43:17.000000 sbomtools-0.3.3/sbomtools/sbomgrep.py
+-rw-r--r--   0 elear      (501) staff       (20)     2598 2022-02-04 10:43:41.000000 sbomtools-0.3.3/sbomtools/sbomls.py
+-rw-r--r--   0 elear      (501) staff       (20)     1583 2022-01-31 18:05:42.000000 sbomtools-0.3.3/sbomtools/sbomrm.py
+-rw-r--r--   0 elear      (501) staff       (20)     2372 2022-01-31 13:06:34.000000 sbomtools-0.3.3/sbomtools/sbomupdate.py
+-rw-r--r--   0 elear      (501) staff       (20)     6576 2023-04-14 13:16:33.000000 sbomtools-0.3.3/sbomtools/spdx.py
+-rw-r--r--   0 elear      (501) staff       (20)     1373 2022-01-28 10:43:39.000000 sbomtools-0.3.3/sbomtools/update.py
+drwxr-xr-x   0 elear      (501) staff       (20)        0 2023-04-14 13:17:19.179745 sbomtools-0.3.3/sbomtools.egg-info/
+-rw-r--r--   0 elear      (501) staff       (20)     4670 2023-04-14 13:17:19.000000 sbomtools-0.3.3/sbomtools.egg-info/PKG-INFO
+-rw-r--r--   0 elear      (501) staff       (20)      477 2023-04-14 13:17:19.000000 sbomtools-0.3.3/sbomtools.egg-info/SOURCES.txt
+-rw-r--r--   0 elear      (501) staff       (20)        1 2023-04-14 13:17:19.000000 sbomtools-0.3.3/sbomtools.egg-info/dependency_links.txt
+-rw-r--r--   0 elear      (501) staff       (20)      150 2023-04-14 13:17:19.000000 sbomtools-0.3.3/sbomtools.egg-info/entry_points.txt
+-rw-r--r--   0 elear      (501) staff       (20)       10 2023-04-14 13:17:19.000000 sbomtools-0.3.3/sbomtools.egg-info/top_level.txt
+-rw-r--r--   0 elear      (501) staff       (20)      548 2023-04-14 13:17:19.181370 sbomtools-0.3.3/setup.cfg
+-rw-r--r--   0 elear      (501) staff       (20)       38 2022-01-24 11:44:48.000000 sbomtools-0.3.3/setup.py
```

### Comparing `sbomtools-0.3.2/LICENSE.txt` & `sbomtools-0.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sbomtools-0.3.2/PKG-INFO` & `sbomtools-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: sbomtools
-Version: 0.3.2
+Version: 0.3.3
 Summary: SBOM tools
 Home-page: https://github.com/sbomtools/sbomtools
 Author: Eliot Lear
 Author-email: lear@cisco.com
 License: BSD 3-Clause License
-Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Welcome to sbomtools
 
 **WARNING**
@@ -136,9 +135,7 @@
  - PackageNotFound: you tried to edit/remove a package that wasn't present.
  - DependencyNotMet: you tried to remove something that had a dependency
    		     and you didn't use -r.
  - AlreadyExists: you tried to add an entry that already exists, and you
                   didn't use -O
  - FileFormatError: there is something wrong with the JSON or the SBOM.
  - UnknownError: Something weird happened.  Open an Issue ;-(
-
-
```

### Comparing `sbomtools-0.3.2/README.md` & `sbomtools-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `sbomtools-0.3.2/sbomtools/cyclonedx.py` & `sbomtools-0.3.3/sbomtools/cyclonedx.py`

 * *Files identical despite different names*

### Comparing `sbomtools-0.3.2/sbomtools/exceptions.py` & `sbomtools-0.3.3/sbomtools/exceptions.py`

 * *Files identical despite different names*

### Comparing `sbomtools-0.3.2/sbomtools/grep.py` & `sbomtools-0.3.3/sbomtools/grep.py`

 * *Files identical despite different names*

### Comparing `sbomtools-0.3.2/sbomtools/remove.py` & `sbomtools-0.3.3/sbomtools/remove.py`

 * *Files identical despite different names*

### Comparing `sbomtools-0.3.2/sbomtools/sbomgrep.py` & `sbomtools-0.3.3/sbomtools/sbomgrep.py`

 * *Files 21% similar despite different names*

```diff
@@ -49,25 +49,30 @@
     """
     Main program to process sbomgrep
     """
 
     if args.files == []:
         results=sbom_grep(stdin,args.searchstr[0])[1]
         if results:
-            print(f'stdin: {results["name"]} version {results["version"]}\n')
+            if results["version"]:
+                print(f'stdin: {results["name"]} version {results["version"]}\n')
+            else:
+                print(f'stdin: {results["name"]}\n')
         return
 
     results=''
     for filename in args.files:
         try:
             with open(filename,'r',encoding='utf8') as s_fp:
                 output=sbom_grep(s_fp,args.searchstr[0],args.json)[1]
                 for entry in output:
-                    results=results + f'{filename}: {entry["name"]} ' + \
-                        f'version {entry["version"]}\n'
+                    results=results + f'{filename}: {entry["name"]}'
+                    if entry["version"]:
+                        results=results + f' version {entry["version"]}'
+                    results=results+'\n'
         except OSError as file_except:
             print(f'{filename}: ' + str(file_except) + '\n')
             return
     print(results,end='')
     return
 
 def cli():
```

### Comparing `sbomtools-0.3.2/sbomtools/sbomls.py` & `sbomtools-0.3.3/sbomtools/sbomls.py`

 * *Files identical despite different names*

### Comparing `sbomtools-0.3.2/sbomtools/sbomrm.py` & `sbomtools-0.3.3/sbomtools/sbomrm.py`

 * *Files identical despite different names*

### Comparing `sbomtools-0.3.2/sbomtools/sbomupdate.py` & `sbomtools-0.3.3/sbomtools/sbomupdate.py`

 * *Files identical despite different names*

### Comparing `sbomtools-0.3.2/sbomtools/spdx.py` & `sbomtools-0.3.3/sbomtools/spdx.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,23 +19,27 @@
         return False
     rets=[]
     prog=re.compile(searchstr)
     for entry in sbom['packages']:
         if prog.match(entry['name']):
             if want_json:
                 rets.append(entry)
-            else:
+            elif 'versionInfo' in entry:
                 rets.append({'name': entry['name'], 'version': entry['versionInfo']})
-        if 'checksums' in entry:
+            else:
+                rets.append({'name': entry['name'], 'version': False })
+        elif 'checksums' in entry:
             for hash_entry in entry['checksums']:
                 if prog.match(hash_entry['checksumValue']):
                     if want_json:
                         rets.append(entry)
-                    else:
+                    elif 'versionInfo' in entry:
                         rets.append({'name': entry['name'], 'version': entry['versionInfo']})
+                    else:
+                        rets.append({'name': entry['name'], 'version': False })
     return rets
 
 def spdx_update(sbom,component_name,version,
                      supplier,email, url, sha256, sha1,
 		     md5,website,overwrite,deps):
     """
     Update SPDX file.
```

### Comparing `sbomtools-0.3.2/sbomtools/update.py` & `sbomtools-0.3.3/sbomtools/update.py`

 * *Files identical despite different names*

### Comparing `sbomtools-0.3.2/sbomtools.egg-info/PKG-INFO` & `sbomtools-0.3.3/sbomtools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: sbomtools
-Version: 0.3.2
+Version: 0.3.3
 Summary: SBOM tools
 Home-page: https://github.com/sbomtools/sbomtools
 Author: Eliot Lear
 Author-email: lear@cisco.com
 License: BSD 3-Clause License
-Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Welcome to sbomtools
 
 **WARNING**
@@ -136,9 +135,7 @@
  - PackageNotFound: you tried to edit/remove a package that wasn't present.
  - DependencyNotMet: you tried to remove something that had a dependency
    		     and you didn't use -r.
  - AlreadyExists: you tried to add an entry that already exists, and you
                   didn't use -O
  - FileFormatError: there is something wrong with the JSON or the SBOM.
  - UnknownError: Something weird happened.  Open an Issue ;-(
-
-
```

### Comparing `sbomtools-0.3.2/setup.cfg` & `sbomtools-0.3.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sbomtools
-version = 0.3.2
+version = 0.3.3
 author = Eliot Lear
 author_email = lear@cisco.com
 url = https://github.com/sbomtools/sbomtools
 description = SBOM tools
 long_description = file:README.md
 long_description_content_type = text/markdown
 license = BSD 3-Clause License
```

