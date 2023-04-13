# Comparing `tmp/jarvis_leaderboard-2023.4.11.1.tar.gz` & `tmp/jarvis_leaderboard-2023.4.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jarvis_leaderboard-2023.4.11.1.tar", last modified: Thu Apr 13 21:40:47 2023, max compression
+gzip compressed data, was "jarvis_leaderboard-2023.4.12.tar", last modified: Thu Apr 13 22:36:51 2023, max compression
```

## Comparing `jarvis_leaderboard-2023.4.11.1.tar` & `jarvis_leaderboard-2023.4.12.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0 kamalch   (1000) kamalch   (1000)        0 2023-04-13 21:40:46.747073 jarvis_leaderboard-2023.4.11.1/
--rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)     1064 2023-02-25 21:44:25.000000 jarvis_leaderboard-2023.4.11.1/LICENSE
--rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)     6423 2023-04-13 21:40:46.745073 jarvis_leaderboard-2023.4.11.1/PKG-INFO
--rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)     5978 2023-04-11 22:13:11.000000 jarvis_leaderboard-2023.4.11.1/README.md
-drwxrwxrwx   0 kamalch   (1000) kamalch   (1000)        0 2023-04-13 21:40:46.687073 jarvis_leaderboard-2023.4.11.1/jarvis_leaderboard/
--rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)       51 2023-04-13 18:41:59.000000 jarvis_leaderboard-2023.4.11.1/jarvis_leaderboard/__init__.py
--rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)     3297 2023-04-07 21:22:48.000000 jarvis_leaderboard-2023.4.11.1/jarvis_leaderboard/jarvis_populate_data.py
--rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)      135 2023-04-12 02:59:35.000000 jarvis_leaderboard-2023.4.11.1/jarvis_leaderboard/jarvis_serve.py
--rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)     2942 2023-04-12 03:01:25.000000 jarvis_leaderboard-2023.4.11.1/jarvis_leaderboard/jarvis_upload.py
--rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)    29761 2023-04-12 03:00:01.000000 jarvis_leaderboard-2023.4.11.1/jarvis_leaderboard/rebuild.py
-drwxrwxrwx   0 kamalch   (1000) kamalch   (1000)        0 2023-04-13 21:40:46.735074 jarvis_leaderboard-2023.4.11.1/jarvis_leaderboard.egg-info/
--rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)     6423 2023-04-13 21:40:46.000000 jarvis_leaderboard-2023.4.11.1/jarvis_leaderboard.egg-info/PKG-INFO
--rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)      410 2023-04-13 21:40:46.000000 jarvis_leaderboard-2023.4.11.1/jarvis_leaderboard.egg-info/SOURCES.txt
--rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)        1 2023-04-13 21:40:46.000000 jarvis_leaderboard-2023.4.11.1/jarvis_leaderboard.egg-info/dependency_links.txt
--rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)      142 2023-04-13 21:40:46.000000 jarvis_leaderboard-2023.4.11.1/jarvis_leaderboard.egg-info/requires.txt
--rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)       19 2023-04-13 21:40:46.000000 jarvis_leaderboard-2023.4.11.1/jarvis_leaderboard.egg-info/top_level.txt
--rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)       38 2023-04-13 21:40:46.748074 jarvis_leaderboard-2023.4.11.1/setup.cfg
--rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)     1305 2023-04-13 18:41:46.000000 jarvis_leaderboard-2023.4.11.1/setup.py
+drwxrwxrwx   0 kamalch   (1000) kamalch   (1000)        0 2023-04-13 22:36:50.329055 jarvis_leaderboard-2023.4.12/
+-rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)     1064 2023-02-25 21:44:25.000000 jarvis_leaderboard-2023.4.12/LICENSE
+-rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)     6421 2023-04-13 22:36:50.328062 jarvis_leaderboard-2023.4.12/PKG-INFO
+-rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)     5978 2023-04-11 22:13:11.000000 jarvis_leaderboard-2023.4.12/README.md
+drwxrwxrwx   0 kamalch   (1000) kamalch   (1000)        0 2023-04-13 22:36:50.270055 jarvis_leaderboard-2023.4.12/jarvis_leaderboard/
+-rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)       49 2023-04-13 22:36:24.000000 jarvis_leaderboard-2023.4.12/jarvis_leaderboard/__init__.py
+-rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)     3297 2023-04-07 21:22:48.000000 jarvis_leaderboard-2023.4.12/jarvis_leaderboard/jarvis_populate_data.py
+-rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)      135 2023-04-12 02:59:35.000000 jarvis_leaderboard-2023.4.12/jarvis_leaderboard/jarvis_serve.py
+-rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)     3150 2023-04-13 22:14:42.000000 jarvis_leaderboard-2023.4.12/jarvis_leaderboard/jarvis_upload.py
+-rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)    30447 2023-04-13 22:34:31.000000 jarvis_leaderboard-2023.4.12/jarvis_leaderboard/rebuild.py
+drwxrwxrwx   0 kamalch   (1000) kamalch   (1000)        0 2023-04-13 22:36:50.317067 jarvis_leaderboard-2023.4.12/jarvis_leaderboard.egg-info/
+-rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)     6421 2023-04-13 22:36:49.000000 jarvis_leaderboard-2023.4.12/jarvis_leaderboard.egg-info/PKG-INFO
+-rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)      410 2023-04-13 22:36:50.000000 jarvis_leaderboard-2023.4.12/jarvis_leaderboard.egg-info/SOURCES.txt
+-rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)        1 2023-04-13 22:36:49.000000 jarvis_leaderboard-2023.4.12/jarvis_leaderboard.egg-info/dependency_links.txt
+-rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)      142 2023-04-13 22:36:49.000000 jarvis_leaderboard-2023.4.12/jarvis_leaderboard.egg-info/requires.txt
+-rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)       19 2023-04-13 22:36:49.000000 jarvis_leaderboard-2023.4.12/jarvis_leaderboard.egg-info/top_level.txt
+-rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)       38 2023-04-13 22:36:50.330057 jarvis_leaderboard-2023.4.12/setup.cfg
+-rwxrwxrwx   0 kamalch   (1000) kamalch   (1000)     1303 2023-04-13 22:36:14.000000 jarvis_leaderboard-2023.4.12/setup.py
```

### Comparing `jarvis_leaderboard-2023.4.11.1/LICENSE` & `jarvis_leaderboard-2023.4.12/LICENSE`

 * *Files identical despite different names*

### Comparing `jarvis_leaderboard-2023.4.11.1/PKG-INFO` & `jarvis_leaderboard-2023.4.12/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jarvis_leaderboard
-Version: 2023.4.11.1
+Version: 2023.4.12
 Summary: jarvis_leaderboard
 Home-page: https://github.com/knc6/jarvis_leaderboard
 Author: Kamal Choudhary
 Author-email: kamal.choudhary@nist.gov
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `jarvis_leaderboard-2023.4.11.1/README.md` & `jarvis_leaderboard-2023.4.12/README.md`

 * *Files identical despite different names*

### Comparing `jarvis_leaderboard-2023.4.11.1/jarvis_leaderboard/jarvis_populate_data.py` & `jarvis_leaderboard-2023.4.12/jarvis_leaderboard/jarvis_populate_data.py`

 * *Files identical despite different names*

### Comparing `jarvis_leaderboard-2023.4.11.1/jarvis_leaderboard/jarvis_upload.py` & `jarvis_leaderboard-2023.4.12/jarvis_leaderboard/jarvis_upload.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#! /usr/bin/env python
+#!/home/knc6/.conda/envs/mer/bin/python
 import argparse
 import os
 import sys
 import requests
 
 parser = argparse.ArgumentParser(description="Add data to JARVIS-Leaderboard.")
 
@@ -36,58 +36,61 @@
 def upload():
     args = parser.parse_args(sys.argv[1:])
     upstream_repo_name = args.upstream_repo_name
     upstream_repo_username = args.upstream_repo_username
     username = args.github_username
     your_benchmark_directory = args.your_benchmark_directory
     cwd = os.getcwd()
-    print("username", username)
+    print ('For help: jarvis_upload.py -h\n')
+    print("GitHub username", username)
     forked_url = "https://github.com/" + username + "/" + upstream_repo_name
     print("forked_url", forked_url)
     response = requests.get(forked_url)
+    print("response", response)
     if response.status_code > 400:
         cmd = (
             "curl -u "
             + username
             + " https://api.github.com/repos/"
             + upstream_repo_username
             + "/"
             + upstream_repo_name
             + "/forks -d ''"
         )
-        print(cmd)
+        print("Forking repo", cmd)
         os.system(cmd)
+    # sys.exit()
     if not os.path.exists(upstream_repo_name):
         cmd = "git clone " + forked_url + ".git"
-        print(cmd)
+        print("Cloning repo", cmd)
         os.system(cmd)
     if os.path.exists(your_benchmark_directory):
         print("Note: adding to existing directory.")
     cmd = (
-        "rsync -r "
+        "cp -r "
         + your_benchmark_directory
         + " jarvis_leaderboard/jarvis_leaderboard/benchmarks/"
     )
-    print(cmd)
+    print("Cpying files", cmd)
     os.system(cmd)
     # cmd='cd '+upstream_repo_name
     os.chdir(upstream_repo_name)
     add_dir = "jarvis_leaderboard/benchmarks/" + your_benchmark_directory
     cmd = "ls ./" + add_dir
-    print(cmd)
+    print("just ls", cmd)
     os.system(cmd)
 
     cmd = "git add ./" + add_dir + "/*"
-    print(cmd)
+    print("Add dir", cmd)
     os.system(cmd)
     cmd = "git commit -m 'Adding benchmark.'"
-    print(cmd)
+    print("Git commit", cmd)
     os.system(cmd)
     cmd = "git push"
-    print(cmd)
+    print("Push", cmd)
     os.system(cmd)
 
     cmd = "python jarvis_leaderboard/rebuild.py"
     print(cmd)
     os.system(cmd)
 
     cmd = (
```

### Comparing `jarvis_leaderboard-2023.4.11.1/jarvis_leaderboard/rebuild.py` & `jarvis_leaderboard-2023.4.12/jarvis_leaderboard/rebuild.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,14 +140,15 @@
     meta_path[-1] = "metadata.json"
     meta_path = "/".join(meta_path)
     meta_data = loadjson(meta_path)
     results["model_name"] = meta_data["model_name"]
     results["team_name"] = meta_data["team_name"]
     results["date_submitted"] = meta_data["date_submitted"]
     results["project_url"] = meta_data["project_url"]
+    results['num_entries']=len(csv_data)
     results["github_url"] = (
         "https://github.com/usnistgov/jarvis_leaderboard/tree/main/jarvis_leaderboard/benchmarks/"
         + bench_name
     )  # meta_path.split('metadata.json')[0]
 
     # print("meta_path", meta_data)
     # meta_data=loadjson()
@@ -239,14 +240,15 @@
 
     return results
 
 
 def rebuild_pages():
     print("Rebuilding web:")
     os.chdir(root_dir + "/..")
+    num_data=0
     for i in glob.glob("jarvis_leaderboard/benchmarks/*/*.csv.zip"):
         # if 'Text' in i:
         # print(i)
         fname = i.split("/")[-1].split(".csv.zip")[0]
         temp = fname.split("-")
         submod = temp[1]
         data_split = temp[4]
@@ -365,26 +367,30 @@
         #    metric,
         #    team,
         #    md_filename,
         #    md_path,
         # )
         with open(md_path, "r") as file:
             filedata = file.read().splitlines()
-        print("names", i)
+        #print("names", i)
         # print()
         res = get_metric_value(
             submod=submod,
             csv_path=i,
             dataset=dataset,
             prop=prop,
             data_split=data_split,
             method=method,
             metric=metric,
             bench_name=bench_name,
         )
+        
+        num_data+=res['dataset_size']
+        #num_data+=res['num_entries']
+        print ('num_data',i, num_data, res['dataset_size'],res['num_entries'])
         # res = 5
         # if clean:
 
         team = (
             '<a href="'
             + res["github_url"]
             + '" target="_blank">'
@@ -733,14 +739,16 @@
                 content.append("<!--table_content-->")
             elif "<!--number_of_benchmarks-->" in j:
                 content.append("<!--number_of_benchmarks-->")
             elif "<!--number_of_tasks-->" in j:
                 content.append("<!--number_of_tasks-->")
             elif "<!--number_of_methods-->" in j:
                 content.append("<!--number_of_methods-->")
+            elif "<!--number_of_datapoints-->" in j:
+                content.append("<!--number_of_datapoints-->")
             else:
                 content.append(j)
         with open(md_path, "w") as file:
             file.write("\n".join(content))
 
         with open(md_path, "r") as file:
             filedata = file.read().splitlines()
@@ -778,14 +786,23 @@
                 temp2 = (
                     "<!--number_of_benchmarks--> - Number of benchmarks: "
                     + str(n_benchs)
                     # + str(len(dat))
                     # + "\n"
                 )
                 content.append(temp2)
+            elif "<!--number_of_datapoints-->" in j:
+                temp2 = (
+                    "<!--number_of_datapoints--> - Number of datapoints: "
+                    + str(num_data)
+                    #+ str(num_data)
+                    # + str(len(dat))
+                    # + "\n"
+                )
+                content.append(temp2)
             else:
                 content.append(j)
         # filedata = filedata.replace('<!--table_content-->', temp)
 
         with open(md_path, "w") as file:
             file.write("\n".join(content))
```

### Comparing `jarvis_leaderboard-2023.4.11.1/jarvis_leaderboard.egg-info/PKG-INFO` & `jarvis_leaderboard-2023.4.12/jarvis_leaderboard.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jarvis-leaderboard
-Version: 2023.4.11.1
+Version: 2023.4.12
 Summary: jarvis_leaderboard
 Home-page: https://github.com/knc6/jarvis_leaderboard
 Author: Kamal Choudhary
 Author-email: kamal.choudhary@nist.gov
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `jarvis_leaderboard-2023.4.11.1/setup.py` & `jarvis_leaderboard-2023.4.12/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="jarvis_leaderboard",  # Replace with your own username
-    version="2023.04.11.1",
+    version="2023.04.12",
     author="Kamal Choudhary",
     author_email="kamal.choudhary@nist.gov",
     description="jarvis_leaderboard",
     install_requires=[
         "numpy>=1.19.5",
         "scipy>=1.6.3",
         "jarvis-tools>=2021.07.19",
```

