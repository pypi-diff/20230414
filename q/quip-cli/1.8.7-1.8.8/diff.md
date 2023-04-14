# Comparing `tmp/quip-cli-1.8.7.tar.gz` & `tmp/quip-cli-1.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quip-cli-1.8.7.tar", last modified: Fri Mar 17 21:12:08 2023, max compression
+gzip compressed data, was "quip-cli-1.8.8.tar", last modified: Fri Apr 14 18:34:55 2023, max compression
```

## Comparing `quip-cli-1.8.7.tar` & `quip-cli-1.8.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2023-03-17 21:12:08.286625 quip-cli-1.8.7/
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    27790 2023-03-17 21:12:08.286492 quip-cli-1.8.7/PKG-INFO
--rwxrw-r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    27390 2022-11-10 22:02:44.000000 quip-cli-1.8.7/README.md
--rwxrw-r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       89 2023-02-23 14:36:14.000000 quip-cli-1.8.7/pyproject.toml
-drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2023-03-17 21:12:08.285328 quip-cli-1.8.7/quip/
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2276 2023-03-17 21:03:28.000000 quip-cli-1.8.7/quip/__init__.py
--rwxrwxr--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    20044 2023-02-20 20:33:28.000000 quip-cli-1.8.7/quip/external.py
--rwxrwxr--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    19670 2022-11-10 22:25:14.000000 quip-cli-1.8.7/quip/field_builder.py
--rwxrwxr--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    72696 2023-03-17 21:01:45.000000 quip-cli-1.8.7/quip/quip.py
--rwxrwxr--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     7104 2022-12-05 17:10:38.000000 quip-cli-1.8.7/quip/version_builder.py
-drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2023-03-17 21:12:08.286295 quip-cli-1.8.7/quip_cli.egg-info/
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    27790 2023-03-17 21:12:08.000000 quip-cli-1.8.7/quip_cli.egg-info/PKG-INFO
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      320 2023-03-17 21:12:08.000000 quip-cli-1.8.7/quip_cli.egg-info/SOURCES.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        1 2023-03-17 21:12:08.000000 quip-cli-1.8.7/quip_cli.egg-info/dependency_links.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       39 2023-03-17 21:12:08.000000 quip-cli-1.8.7/quip_cli.egg-info/entry_points.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      101 2023-03-17 21:12:08.000000 quip-cli-1.8.7/quip_cli.egg-info/requires.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        5 2023-03-17 21:12:08.000000 quip-cli-1.8.7/quip_cli.egg-info/top_level.txt
--rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       38 2023-03-17 21:12:08.286663 quip-cli-1.8.7/setup.cfg
--rwxrw-r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1281 2022-10-06 20:00:12.000000 quip-cli-1.8.7/setup.py
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2023-04-14 18:34:55.375705 quip-cli-1.8.8/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    27790 2023-04-14 18:34:55.375370 quip-cli-1.8.8/PKG-INFO
+-rwxrw-r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    27390 2022-11-10 22:02:44.000000 quip-cli-1.8.8/README.md
+-rwxrw-r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       89 2023-02-23 14:36:14.000000 quip-cli-1.8.8/pyproject.toml
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2023-04-14 18:34:55.372090 quip-cli-1.8.8/quip/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     2276 2023-04-14 17:57:00.000000 quip-cli-1.8.8/quip/__init__.py
+-rwxrwxr--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    20123 2023-04-14 18:15:41.000000 quip-cli-1.8.8/quip/external.py
+-rwxrwxr--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    19670 2022-11-10 22:25:14.000000 quip-cli-1.8.8/quip/field_builder.py
+-rwxrwxr--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    73416 2023-04-14 18:24:04.000000 quip-cli-1.8.8/quip/quip.py
+-rwxrwxr--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     7104 2022-12-05 17:10:38.000000 quip-cli-1.8.8/quip/version_builder.py
+drwxr-xr-x   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        0 2023-04-14 18:34:55.374920 quip-cli-1.8.8/quip_cli.egg-info/
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)    27790 2023-04-14 18:34:55.000000 quip-cli-1.8.8/quip_cli.egg-info/PKG-INFO
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      320 2023-04-14 18:34:55.000000 quip-cli-1.8.8/quip_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        1 2023-04-14 18:34:55.000000 quip-cli-1.8.8/quip_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       39 2023-04-14 18:34:55.000000 quip-cli-1.8.8/quip_cli.egg-info/entry_points.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)      101 2023-04-14 18:34:55.000000 quip-cli-1.8.8/quip_cli.egg-info/requires.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)        5 2023-04-14 18:34:55.000000 quip-cli-1.8.8/quip_cli.egg-info/top_level.txt
+-rw-r--r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)       38 2023-04-14 18:34:55.375766 quip-cli-1.8.8/setup.cfg
+-rwxrw-r--   0 h.gomleksizoglu (612458557) STONEBRANCH\Domain Users (287026403)     1281 2022-10-06 20:00:12.000000 quip-cli-1.8.8/setup.py
```

### Comparing `quip-cli-1.8.7/PKG-INFO` & `quip-cli-1.8.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quip-cli
-Version: 1.8.7
+Version: 1.8.8
 Summary: Tool for creating/updating new universal integrations
 Author: Stonebranch
 Author-email: huseyin.gomleksizoglu@stonebranch.com
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `quip-cli-1.8.7/README.md` & `quip-cli-1.8.8/README.md`

 * *Files identical despite different names*

### Comparing `quip-cli-1.8.7/quip/__init__.py` & `quip-cli-1.8.8/quip/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from colorama import Fore, Style, init
 init()
 
-__version__ = "1.8.7"
+__version__ = "1.8.8"
 
 def cprint(text, color, end='\n', style='Normal'):
     if len(str(text).strip()) == 0: return
     fore = getattr(Fore, color.upper())
     style = getattr(Style, style.upper())
     print('{0}{1}{2}{3}'.format(fore, style, text, Style.RESET_ALL), end=end)
```

### Comparing `quip-cli-1.8.7/quip/external.py` & `quip-cli-1.8.8/quip/external.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,14 +214,15 @@
                 result.append((project.path_with_namespace, project.id))
             
             return result
         
         return projects
 
     def create_project(self, name, group_id, config=None):
+        self.log.info(f"Creating repository name={name} namespace={group_id}")
         self.project = self.gl.projects.create({"name": name, "namespace_id": group_id})
         if config is not None:
             if "protected_branch" in config:
                 self.log.info("Creating protected branch for the repository.")
                 protected_branch = config.get("protected_branch", None)
                 if protected_branch is not None:
                     result = self.create_protected_branch(protected_branch)
```

### Comparing `quip-cli-1.8.7/quip/field_builder.py` & `quip-cli-1.8.8/quip/field_builder.py`

 * *Files identical despite different names*

### Comparing `quip-cli-1.8.7/quip/quip.py` & `quip-cli-1.8.8/quip/quip.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,15 +210,19 @@
                 self.update_rename_scripts()
             else:
                 self.update_project(self.args.uuid, self.args.new_uuid, new_project=False)
             self.dump_fields(write=True)
         elif action in DELETE_ACTION:
             self.delete_project()
         elif action in CLONE_ACTION:
-            self.clone_project(self.args.source)
+            if self.args.template:
+                exclude_list = self._global_conf_defaults.get("bootstrap", {}).get("template-exclude", None)
+            else:
+                exclude_list = self._global_conf_defaults.get("bootstrap", {}).get("exclude", None)
+            self.clone_project(self.args.source, all_files=True, exclude_list=exclude_list)
             self.dump_fields(write=True)
         elif action in BOOTSTRAP_ACTION:
             if self.args.template:
                 self.bootstrap_template()
             else:
                 self.bootstrap_project()
             self.dump_fields(write=True)
@@ -323,15 +327,15 @@
             print("ERROR: Folder already exists")
             sys.exit(1)
         
         os.makedirs(self.project_folder_name)
         self.uip_init(self.project_folder_name, self.default_template)
         self.update_extension_yaml(self.extension_name)
         self.update_uip_config(self.project_name, new_project=True)
-        self.update_template_json(self.project_name)
+        self.update_template_json(self.project_name, new_project=True)
 
     def update_project(self, update_uuid=False, update_new_uuid=False, new_project=True):
         logging.info(f"Updating extension {self.template_name}")
         if not self.args.template:
             self.update_extension_yaml(self.extension_name, new_project=new_project)
             self.update_uip_config(self.project_name, new_project=new_project)
         else:
@@ -863,18 +867,23 @@
         sq.create_project(sq_project_name)
 
     def create_gitlab(self, gl, repository_name=None, config=None):
         logging.info("Creating GitLab Repository.")
         
         if repository_name is None:
             groups = gl.get_groups()
+            logging.debug(f"Groups = {groups}")
             group = choose_one(groups, title="Gitlab Groups", default=gl.default_group)
+            logging.debug(f"Selected group = {group}")
             group_id = group[1]
+            logging.debug(f"group_id = {group_id}")
             _group = gl.gl.groups.get(group_id)
-            group_path = _group.path
+            logging.debug(f"_group = {_group}")
+            group_path = _group.full_path
+            logging.debug(f"group_path = {group_path}")
             repository_name = f"{group_path}/{self.extension_name}"
         
         if self.check_gitlab_repository_exists(gl, repository_name):
             cprint(f"There is a repository already exists in GitLab. ({repository_name})", "yellow")
             cprint(f"Run `git remote add origin {gl.base_url}/{repository_name}.git", "yellow")
         else:
             gl.create_project(self.extension_name, group_id, config=config)
@@ -901,15 +910,15 @@
                     cprint(f"Be sure you rename README.md file and run ", "yellow")
                     cprint(f"     git checkout -b {gl.default_branch}", "yellow")
                     cprint(f"     git pull origin {gl.default_branch}", "yellow")
             
         return repository_name
     
     def check_gitlab_repository_exists(self, gl, repository_name):
-        logging.info("Checking GitLab if the repository exists.")
+        logging.info(f"Checking GitLab if the repository exists. Repository={repository_name}")
             
         projects = gl.get_projects()
         for project in projects:
             if repository_name == project[0]:
                 gl.project_id = project[1]
                 return True
         
@@ -1198,41 +1207,42 @@
             with open(template_path, "r") as f:
                 template_content = f.read()
                 return json.loads(template_content)
         else:
             logging.error(f"ERROR: template.json file is missing! Path= {template_path}")
             sys.exit(1)
 
-    def update_template_json(self, project_name, update_uuid=False, update_new_uuid=False):
+    def update_template_json(self, project_name, update_uuid=False, update_new_uuid=False, new_project=False):
         logging.info("Updating template.json file")
         template = self.join_path("src", "templates", "template.json")
         if os.path.exists(template):
             with open(template, "r") as f:
                 template_content = f.read()
                 if update_uuid:
                     logging.info("Updating SysIds in template.json")
                     template_content = self.update_all_sysid_values(template_content)
                 if update_new_uuid:
                     logging.info("Updating new_uuid with a valid SysIds in template.json")
                     template_content = self.update_new_uuid_values(template_content)
-
-            with open(template, "w") as f:
-                _json = json.loads(template_content)
-                if "extension" in _json and _json["extension"] is not None:
-                    _json["extension"] = self.extension_name
-                _json["name"] = self.template_name
-                if "variablePrefix" in _json:
-                    if self.args.template:
-                        _json["variablePrefix"] = "var"    
-                    else:
-                        _json["variablePrefix"] = self.extension_name.replace("-", "_")
-                        if len(_json["variablePrefix"]) > 20:
-                            _json["variablePrefix"] = "ext"
-                f.write(self.format_json(_json))
-                logging.debug("template.json file is updated")
+            
+            if new_project:
+                with open(template, "w") as f:
+                    _json = json.loads(template_content)
+                    if "extension" in _json and _json["extension"] is not None:
+                        _json["extension"] = self.extension_name
+                    _json["name"] = self.template_name
+                    if "variablePrefix" in _json:
+                        if self.args.template:
+                            _json["variablePrefix"] = "var"
+                        else:
+                            _json["variablePrefix"] = self.extension_name.replace("-", "_")
+                            if len(_json["variablePrefix"]) > 20:
+                                _json["variablePrefix"] = "ext"
+                    f.write(self.format_json(_json))
+            logging.debug("template.json file is updated")
         else:
             logging.error(f"ERROR: template.json file is missing! Path= {template}")
             sys.exit(1)
     
     def merge_template_scripts(self, project_name):
         logging.info("Merging scripts to template.json file")
         template = self.join_path("src", "templates", "template.json")
```

### Comparing `quip-cli-1.8.7/quip/version_builder.py` & `quip-cli-1.8.8/quip/version_builder.py`

 * *Files identical despite different names*

### Comparing `quip-cli-1.8.7/quip_cli.egg-info/PKG-INFO` & `quip-cli-1.8.8/quip_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quip-cli
-Version: 1.8.7
+Version: 1.8.8
 Summary: Tool for creating/updating new universal integrations
 Author: Stonebranch
 Author-email: huseyin.gomleksizoglu@stonebranch.com
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `quip-cli-1.8.7/setup.py` & `quip-cli-1.8.8/setup.py`

 * *Files identical despite different names*

