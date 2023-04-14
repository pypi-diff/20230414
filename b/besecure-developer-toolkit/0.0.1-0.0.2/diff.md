# Comparing `tmp/besecure_developer_toolkit-0.0.1.tar.gz` & `tmp/besecure_developer_toolkit-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "besecure_developer_toolkit-0.0.1.tar", max compression
+gzip compressed data, was "besecure_developer_toolkit-0.0.2.tar", max compression
```

## Comparing `besecure_developer_toolkit-0.0.1.tar` & `besecure_developer_toolkit-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,10 @@
--rw-r--r--   0        0        0     1834 2023-04-11 08:15:16.731716 besecure_developer_toolkit-0.0.1/README.md
--rw-r--r--   0        0        0      340 2023-04-10 11:19:33.073271 besecure_developer_toolkit-0.0.1/besecure_developer_toolkit/__init__.py
--rw-r--r--   0        0        0      203 2023-04-09 16:02:25.204287 besecure_developer_toolkit-0.0.1/besecure_developer_toolkit/__main__.py
--rw-r--r--   0        0        0     3080 2023-04-10 17:42:55.934135 besecure_developer_toolkit-0.0.1/besecure_developer_toolkit/cli.py
--rw-r--r--   0        0        0        0 2023-04-05 04:05:29.896606 besecure_developer_toolkit-0.0.1/besecure_developer_toolkit/config.py
--rw-r--r--   0        0        0     6618 2023-04-11 08:03:27.411904 besecure_developer_toolkit-0.0.1/besecure_developer_toolkit/src/CreateOsspMaster.py
--rw-r--r--   0        0        0     3651 2023-04-11 07:30:10.090236 besecure_developer_toolkit-0.0.1/besecure_developer_toolkit/src/CreateVersionData.py
--rw-r--r--   0        0        0     4318 2023-04-10 03:20:43.016876 besecure_developer_toolkit-0.0.1/besecure_developer_toolkit/src/GenerateReport.py
--rw-r--r--   0        0        0     5057 2023-04-11 08:03:28.135903 besecure_developer_toolkit-0.0.1/besecure_developer_toolkit/src/__pycache__/CreateOsspMaster.cpython-310.pyc
--rw-r--r--   0        0        0     3412 2023-04-11 07:30:10.786242 besecure_developer_toolkit-0.0.1/besecure_developer_toolkit/src/__pycache__/CreateVersionData.cpython-310.pyc
--rw-r--r--   0        0        0     3765 2023-04-10 03:23:51.937972 besecure_developer_toolkit-0.0.1/besecure_developer_toolkit/src/__pycache__/GenerateReport.cpython-310.pyc
--rw-r--r--   0        0        0      493 2023-04-10 10:46:25.800379 besecure_developer_toolkit-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2276 1970-01-01 00:00:00.000000 besecure_developer_toolkit-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1873 2023-04-14 10:59:12.451665 besecure_developer_toolkit-0.0.2/README.md
+-rw-r--r--   0        0        0      340 2023-04-10 11:19:33.073271 besecure_developer_toolkit-0.0.2/besecure_developer_toolkit/__init__.py
+-rw-r--r--   0        0        0      203 2023-04-09 16:02:25.204287 besecure_developer_toolkit-0.0.2/besecure_developer_toolkit/__main__.py
+-rw-r--r--   0        0        0     3080 2023-04-14 10:56:49.945336 besecure_developer_toolkit-0.0.2/besecure_developer_toolkit/cli.py
+-rw-r--r--   0        0        0        0 2023-04-05 04:05:29.896606 besecure_developer_toolkit-0.0.2/besecure_developer_toolkit/config.py
+-rw-r--r--   0        0        0     7232 2023-04-14 11:23:16.895125 besecure_developer_toolkit-0.0.2/besecure_developer_toolkit/src/CreateOsspMaster.py
+-rw-r--r--   0        0        0     3769 2023-04-14 11:24:48.998259 besecure_developer_toolkit-0.0.2/besecure_developer_toolkit/src/CreateVersionData.py
+-rw-r--r--   0        0        0     4318 2023-04-10 03:20:43.016876 besecure_developer_toolkit-0.0.2/besecure_developer_toolkit/src/GenerateReport.py
+-rw-r--r--   0        0        0      612 2023-04-14 11:28:26.704427 besecure_developer_toolkit-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2434 1970-01-01 00:00:00.000000 besecure_developer_toolkit-0.0.2/PKG-INFO
```

### Comparing `besecure_developer_toolkit-0.0.1/README.md` & `besecure_developer_toolkit-0.0.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,47 +1,49 @@
 # Be-Secure Developer Toolkit (bes-dev-kit)
 
 bes-dev-kit is a cli tool for generating metadata and assessment report for [BeSLighthouse](https://github.com/Be-Secure/BeSLighthouse).
 
-`Note: The code is still in testing phase`
+# Installation
+
+`$ python3 -m pip install besecure-developer-toolkit`
 
 # Pre-requisites
 
 1. [Poetry](https://python-poetry.org/)
 2. Python 3.x
 3. pip
 4. Github personal access token
 
 # Setting env variables
 
-`Note: Should be done before testing`
+`Note: Should be done before testing/running`
 
 1. Creating a json file in your user home dir under the name `bes-dev-kit.json`.
 2. Copy the below contents and paste it inside the file.
    
         {
         "GITHUB_ORG": "Be-Secure",
-        "OSSPOI_DIR": "<user-home>/besecure-osspoi-datastore",
-        "ASSESSMENT_DIR": "<user-home>/besecure-assessment-datastore",
+        "OSSPOI_DIR": "<complete_path_to>/besecure-osspoi-datastore",
+        "ASSESSMENT_DIR": "<complete_path_to>/besecure-assessment-datastore",
         "GITHUB_AUTH_TOKEN": "<token>"
         }
 3. Update `OSSPOI_DIR` and `ASSESSMENT_DIR` with complete path to your `besecure-assessment-datastore` and `besecure-osspoi-datastore`  dirs.
 4. Add your github personal access token
 
-# Testing Locally
 
-## Set up
+# Setting up locally
+
 1. Install [poetry](https://python-poetry.org/). Use the [link](https://python-poetry.org/docs/) to install Poetry.
 2. Clone the repo.
 3. Move into the cloned directory.
 4. Create a new virtual env using Poetry - `$ poetry shell`
 5. Run the command to install the tool- `$ poetry install`
 6. Check installation - `$ bes-dev-kit --help`
 
-## Commands
+# Usage
 
 ### Generate Metadata
 
 Command helps to generate metadata such as OSSP-master file data and version details file.
 
 `$ bes-dev-kit generate metadata`
```

### Comparing `besecure_developer_toolkit-0.0.1/besecure_developer_toolkit/cli.py` & `besecure_developer_toolkit-0.0.2/besecure_developer_toolkit/cli.py`

 * *Files identical despite different names*

### Comparing `besecure_developer_toolkit-0.0.1/besecure_developer_toolkit/src/CreateOsspMaster.py` & `besecure_developer_toolkit-0.0.2/besecure_developer_toolkit/src/CreateOsspMaster.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,17 +11,30 @@
     def check_issue_exists(self,id) -> None:
         try:
             urlopen('https://github.com/Be-Secure/Be-Secure/issues/'+str(id))
         except Exception as e:
             exc_type, exc_obj, exc_tb = sys.exc_info()
             fname = os.path.split(exc_tb.tb_frame.f_code.co_filename)[1]
             print(exc_type, fname, exc_tb.tb_lineno)
-            print("Could not find issue with id : "+id)
+            print("Could not find issue with id : "+str(id))
             sys.exit()
     
+    def check_issue_related_to_project(self):
+            
+        json_data = json.loads(urlopen(f'https://api.github.com/repos/Be-Secure/Be-Secure/issues/{self.id}').read())
+        issue_title = json_data["title"]
+        project_name = str(str(issue_title).split(":")[1]).replace(" ","")
+        if project_name != self.name:
+            print(f"[bold red]Alert! [yellow]Mismatch issue_id-project : [green] Issue id {self.id} does not match the project {self.name}")
+            sys.exit()
+        else:
+            pass
+
+        
+    
     def check_repo_exists(self,name) -> None:
         try:
             urlopen('https://api.github.com/repos/Be-Secure/'+name)
         except Exception as e:
             exc_type, exc_obj, exc_tb = sys.exc_info()
             fname = os.path.split(exc_tb.tb_frame.f_code.co_filename)[1]
             print(exc_type, fname, exc_tb.tb_lineno)
@@ -103,24 +116,25 @@
             f.truncate()
         
     
     
     def GenerateOsspMaster(self, overwrite: bool):
         self.check_issue_exists(self.id)
         self.check_repo_exists(self.name)
+        self.check_issue_related_to_project()
         osspoi_dir = os.environ['OSSPOI_DIR']
         namespace = os.environ['GITHUB_ORG']
         token = os.environ['GITHUB_AUTH_TOKEN']
         write_flag = True
         f = open(osspoi_dir+"/OSSP-Master.json", "r+")
         ossp_master_json = json.load(f)
         if not overwrite:                 
             for i in range(len(ossp_master_json["items"])):
                 if ossp_master_json["items"][i]["id"] == self.id:
-                    print("[bold red]Alert! [green]Entry for "+str(self.id)+"-"+self.name+" already present")
+                    print("[bold red]Alert! [green]Entry for "+str(self.id)+"-"+self.name+" already present under OSSP-Master.json")
                     write_flag = False
                     break
                 else:
                     write_flag = True
         if write_flag:
             # proc = subprocess.Popen([f'curl -L -H "Accept: application/vnd.github+json" -H "Authorization: Bearer <YOUR-TOKEN>"-H "X-GitHub-Api-Version: 2022-11-28" https://api.github.com//{namespace}/{self.name}'], stdout=subprocess.PIPE, shell=True)
             # (out, err) = proc.communicate()
```

### Comparing `besecure_developer_toolkit-0.0.1/besecure_developer_toolkit/src/CreateVersionData.py` & `besecure_developer_toolkit-0.0.2/besecure_developer_toolkit/src/CreateVersionData.py`

 * *Files 10% similar despite different names*

```diff
@@ -66,25 +66,27 @@
         path = osspoi_dir+"/version_details/"+str(self.id) + "-" + self.name + "-" "Versiondetails.json"
         if os.path.exists(path):
             f = open(path, "r+") 
             original_data = json.load(f)
             for i in range(len(original_data)):
                 if original_data[i]["version"] == version_data_new["version"] and not overwrite:
                     write_flag = False
-                    print("[bold red]Alert! [green]Version " +version_tag+ " exists")
+                    print(f"[bold red]Alert! [green]Version {version_tag} exists under {self.id}-{self.name}-Versiondetails.json ")
                     break
                 else:
                     write_flag = True
             if write_flag == True and not overwrite:
                 original_data.append(version_data_new)
                 f.seek(0)
                 f.write(json.dumps(original_data, indent=4))
                 f.truncate
-            else:
+            elif write_flag == True and overwrite:
                 self.overwrite_version_data(f, version_data_new, original_data, version_tag)
+            else:
+                pass
         else:
             f = open(path, "w")
             f.write(json.dumps(version_data_new, indent=4))
         self.cleanup()
         f.close()
```

### Comparing `besecure_developer_toolkit-0.0.1/besecure_developer_toolkit/src/GenerateReport.py` & `besecure_developer_toolkit-0.0.2/besecure_developer_toolkit/src/GenerateReport.py`

 * *Files identical despite different names*

### Comparing `besecure_developer_toolkit-0.0.1/PKG-INFO` & `besecure_developer_toolkit-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,61 +1,63 @@
 Metadata-Version: 2.1
 Name: besecure-developer-toolkit
-Version: 0.0.1
-Summary: 
+Version: 0.0.2
+Summary: cli tool for generating metadata and assessment report for [BeSLighthouse](https://github.com/Be-Secure/BeSLighthouse).
 Author: asa1997
 Author-email: arunsureshampadath@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pytest (>=7.3.0,<8.0.0)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown
 
 # Be-Secure Developer Toolkit (bes-dev-kit)
 
 bes-dev-kit is a cli tool for generating metadata and assessment report for [BeSLighthouse](https://github.com/Be-Secure/BeSLighthouse).
 
-`Note: The code is still in testing phase`
+# Installation
+
+`$ python3 -m pip install besecure-developer-toolkit`
 
 # Pre-requisites
 
 1. [Poetry](https://python-poetry.org/)
 2. Python 3.x
 3. pip
 4. Github personal access token
 
 # Setting env variables
 
-`Note: Should be done before testing`
+`Note: Should be done before testing/running`
 
 1. Creating a json file in your user home dir under the name `bes-dev-kit.json`.
 2. Copy the below contents and paste it inside the file.
    
         {
         "GITHUB_ORG": "Be-Secure",
-        "OSSPOI_DIR": "<user-home>/besecure-osspoi-datastore",
-        "ASSESSMENT_DIR": "<user-home>/besecure-assessment-datastore",
+        "OSSPOI_DIR": "<complete_path_to>/besecure-osspoi-datastore",
+        "ASSESSMENT_DIR": "<complete_path_to>/besecure-assessment-datastore",
         "GITHUB_AUTH_TOKEN": "<token>"
         }
 3. Update `OSSPOI_DIR` and `ASSESSMENT_DIR` with complete path to your `besecure-assessment-datastore` and `besecure-osspoi-datastore`  dirs.
 4. Add your github personal access token
 
-# Testing Locally
 
-## Set up
+# Setting up locally
+
 1. Install [poetry](https://python-poetry.org/). Use the [link](https://python-poetry.org/docs/) to install Poetry.
 2. Clone the repo.
 3. Move into the cloned directory.
 4. Create a new virtual env using Poetry - `$ poetry shell`
 5. Run the command to install the tool- `$ poetry install`
 6. Check installation - `$ bes-dev-kit --help`
 
-## Commands
+# Usage
 
 ### Generate Metadata
 
 Command helps to generate metadata such as OSSP-master file data and version details file.
 
 `$ bes-dev-kit generate metadata`
```

