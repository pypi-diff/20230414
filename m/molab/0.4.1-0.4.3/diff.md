# Comparing `tmp/molab-0.4.1.tar.gz` & `tmp/molab-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molab-0.4.1.tar", last modified: Fri Apr  7 00:06:24 2023, max compression
+gzip compressed data, was "molab-0.4.3.tar", last modified: Fri Apr 14 18:09:10 2023, max compression
```

## Comparing `molab-0.4.1.tar` & `molab-0.4.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:06:24.843916 molab-0.4.1/
--rw-r--r--   0 root         (0) root         (0)      786 2023-04-07 00:06:24.843916 molab-0.4.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      275 2023-04-07 00:06:09.000000 molab-0.4.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:06:24.839339 molab-0.4.1/molab/
--rw-rw-rw-   0 root         (0) root         (0)      181 2023-04-07 00:06:09.000000 molab-0.4.1/molab/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18516 2023-04-07 00:06:09.000000 molab-0.4.1/molab/configure.py
--rw-rw-rw-   0 root         (0) root         (0)     2440 2023-04-07 00:06:09.000000 molab-0.4.1/molab/courses.py
--rw-rw-rw-   0 root         (0) root         (0)    15533 2023-04-07 00:06:09.000000 molab-0.4.1/molab/deploy.py
--rw-rw-rw-   0 root         (0) root         (0)     4922 2023-04-07 00:06:09.000000 molab-0.4.1/molab/destroy.py
--rw-rw-rw-   0 root         (0) root         (0)    20029 2023-04-07 00:06:09.000000 molab-0.4.1/molab/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:06:24.843916 molab-0.4.1/molab/template_files/
--rw-rw-rw-   0 root         (0) root         (0)    38695 2023-04-07 00:06:09.000000 molab-0.4.1/molab/template_files/MorpheusImage.png
--rw-rw-rw-   0 root         (0) root         (0)      835 2023-04-07 00:06:09.000000 molab-0.4.1/molab/template_files/admin_class_config.json
--rw-rw-rw-   0 root         (0) root         (0)      834 2023-04-07 00:06:09.000000 molab-0.4.1/molab/template_files/automation_class_config.json
--rw-rw-rw-   0 root         (0) root         (0)      353 2023-04-07 00:06:09.000000 molab-0.4.1/molab/template_files/git_auth_type_pat.json
--rw-rw-rw-   0 root         (0) root         (0)      834 2023-04-07 00:06:09.000000 molab-0.4.1/molab/template_files/install_class_config.json
--rw-rw-rw-   0 root         (0) root         (0)      518 2023-04-07 00:06:09.000000 molab-0.4.1/molab/template_files/instance_provisioning_payload.json
--rw-rw-rw-   0 root         (0) root         (0)     1124 2023-04-07 00:06:09.000000 molab-0.4.1/molab/template_files/manual_option_list_aws_regions.json
--rw-rw-rw-   0 root         (0) root         (0)      191 2023-04-07 00:06:09.000000 molab-0.4.1/molab/template_files/platform_setup.json
--rw-rw-rw-   0 root         (0) root         (0)      834 2023-04-07 00:06:09.000000 molab-0.4.1/molab/template_files/troubleshooting_class_config.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 00:06:24.841170 molab-0.4.1/molab.egg-info/
--rw-r--r--   0 root         (0) root         (0)      786 2023-04-07 00:06:24.000000 molab-0.4.1/molab.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      700 2023-04-07 00:06:24.000000 molab-0.4.1/molab.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 00:06:24.000000 molab-0.4.1/molab.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       77 2023-04-07 00:06:24.000000 molab-0.4.1/molab.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-04-07 00:06:24.000000 molab-0.4.1/molab.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-07 00:06:24.843916 molab-0.4.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1248 2023-04-07 00:06:09.000000 molab-0.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 18:09:10.369736 molab-0.4.3/
+-rw-r--r--   0 root         (0) root         (0)      786 2023-04-14 18:09:10.368736 molab-0.4.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      275 2023-04-14 18:08:53.000000 molab-0.4.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 18:09:10.363736 molab-0.4.3/molab/
+-rw-rw-rw-   0 root         (0) root         (0)      181 2023-04-14 18:08:53.000000 molab-0.4.3/molab/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18516 2023-04-14 18:08:53.000000 molab-0.4.3/molab/configure.py
+-rw-rw-rw-   0 root         (0) root         (0)     2440 2023-04-14 18:08:53.000000 molab-0.4.3/molab/courses.py
+-rw-rw-rw-   0 root         (0) root         (0)    15533 2023-04-14 18:08:53.000000 molab-0.4.3/molab/deploy.py
+-rw-rw-rw-   0 root         (0) root         (0)     4922 2023-04-14 18:08:53.000000 molab-0.4.3/molab/destroy.py
+-rw-rw-rw-   0 root         (0) root         (0)    20062 2023-04-14 18:08:53.000000 molab-0.4.3/molab/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 18:09:10.368736 molab-0.4.3/molab/template_files/
+-rw-rw-rw-   0 root         (0) root         (0)    38695 2023-04-14 18:08:53.000000 molab-0.4.3/molab/template_files/MorpheusImage.png
+-rw-rw-rw-   0 root         (0) root         (0)      835 2023-04-14 18:08:53.000000 molab-0.4.3/molab/template_files/admin_class_config.json
+-rw-rw-rw-   0 root         (0) root         (0)      834 2023-04-14 18:08:53.000000 molab-0.4.3/molab/template_files/automation_class_config.json
+-rw-rw-rw-   0 root         (0) root         (0)      353 2023-04-14 18:08:53.000000 molab-0.4.3/molab/template_files/git_auth_type_pat.json
+-rw-rw-rw-   0 root         (0) root         (0)      834 2023-04-14 18:08:53.000000 molab-0.4.3/molab/template_files/install_class_config.json
+-rw-rw-rw-   0 root         (0) root         (0)      518 2023-04-14 18:08:53.000000 molab-0.4.3/molab/template_files/instance_provisioning_payload.json
+-rw-rw-rw-   0 root         (0) root         (0)     1124 2023-04-14 18:08:53.000000 molab-0.4.3/molab/template_files/manual_option_list_aws_regions.json
+-rw-rw-rw-   0 root         (0) root         (0)      191 2023-04-14 18:08:53.000000 molab-0.4.3/molab/template_files/platform_setup.json
+-rw-rw-rw-   0 root         (0) root         (0)      834 2023-04-14 18:08:53.000000 molab-0.4.3/molab/template_files/troubleshooting_class_config.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 18:09:10.365736 molab-0.4.3/molab.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      786 2023-04-14 18:09:10.000000 molab-0.4.3/molab.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      700 2023-04-14 18:09:10.000000 molab-0.4.3/molab.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 18:09:10.000000 molab-0.4.3/molab.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       77 2023-04-14 18:09:10.000000 molab-0.4.3/molab.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-04-14 18:09:10.000000 molab-0.4.3/molab.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-14 18:09:10.369736 molab-0.4.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1248 2023-04-14 18:08:53.000000 molab-0.4.3/setup.py
```

### Comparing `molab-0.4.1/PKG-INFO` & `molab-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molab
-Version: 0.4.1
+Version: 0.4.3
 Summary: molab is a python package for configuring Morpheus training lab environments.
 Home-page: https://gitlab.com/morpheus_training/molab
 Author: Sean Jabro
 Author-email: sean.jabro@outlook.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `molab-0.4.1/molab/configure.py` & `molab-0.4.3/molab/configure.py`

 * *Files identical despite different names*

### Comparing `molab-0.4.1/molab/courses.py` & `molab-0.4.3/molab/courses.py`

 * *Files identical despite different names*

### Comparing `molab-0.4.1/molab/deploy.py` & `molab-0.4.3/molab/deploy.py`

 * *Files identical despite different names*

### Comparing `molab-0.4.1/molab/destroy.py` & `molab-0.4.3/molab/destroy.py`

 * *Files identical despite different names*

### Comparing `molab-0.4.1/molab/helpers.py` & `molab-0.4.3/molab/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,16 +71,16 @@
             if i[0]["type"] != "git":
                 logger.error(f'This is not a git based integration. No code repo to find')
                 return
             logger.info(f'Collecting the name of the code repository')
             cr = i[0]["url"].split("/")[-1]
             integration_id = i[0]["id"]
             try:
-                logger.info(f'Attempting to make the API call for: {url}{e2}?name={cr} - {integration_name}')
-                resp = requests.get(f'{url}{e2}?phrase={cr}',headers=headers)
+                logger.info(f'Attempting to make the API call for: {url}{e2}?integrationId={integration_id}')
+                resp = requests.get(f'{url}{e2}?integrationId={integration_id}',headers=headers, verify=False)
                 if "200" in str(resp):
                     logger.info("Success!")
                     i = resp.json()["data"]
                     if len(i) > 1:
                         logger.info('Found more than one code repo this url...thinking....')
                         for r in i:
                             if integration_name in r:
@@ -124,15 +124,15 @@
         data = resp.json()
     except Exception as e:
         logger.error(e)
         return
     if data["success"]:
         logger.info(f'Successfully add GIT integration at id: {data["integration"]["id"]}')
         logger.info(f'Pausing to allow code sync')
-        time.sleep(10)
+        time.sleep(30)
         logger.info(f'Acquiring linked code repo id...')
         code_repo_id = _get_code_repo_id_by_integration_name(url,headers,integration_name)
         logger.info(f'Acquired the code repo id: {code_repo_id}')
         integration_info = {
             "integration_id": data["integration"]["id"],
             "linked_code_repo_id": code_repo_id
             }
```

### Comparing `molab-0.4.1/molab/template_files/MorpheusImage.png` & `molab-0.4.3/molab/template_files/MorpheusImage.png`

 * *Files identical despite different names*

### Comparing `molab-0.4.1/molab/template_files/admin_class_config.json` & `molab-0.4.3/molab/template_files/admin_class_config.json`

 * *Files identical despite different names*

### Comparing `molab-0.4.1/molab/template_files/automation_class_config.json` & `molab-0.4.3/molab/template_files/automation_class_config.json`

 * *Files identical despite different names*

### Comparing `molab-0.4.1/molab/template_files/install_class_config.json` & `molab-0.4.3/molab/template_files/install_class_config.json`

 * *Files identical despite different names*

### Comparing `molab-0.4.1/molab/template_files/instance_provisioning_payload.json` & `molab-0.4.3/molab/template_files/instance_provisioning_payload.json`

 * *Files identical despite different names*

### Comparing `molab-0.4.1/molab/template_files/manual_option_list_aws_regions.json` & `molab-0.4.3/molab/template_files/manual_option_list_aws_regions.json`

 * *Files identical despite different names*

### Comparing `molab-0.4.1/molab/template_files/troubleshooting_class_config.json` & `molab-0.4.3/molab/template_files/troubleshooting_class_config.json`

 * *Files identical despite different names*

### Comparing `molab-0.4.1/molab.egg-info/PKG-INFO` & `molab-0.4.3/molab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molab
-Version: 0.4.1
+Version: 0.4.3
 Summary: molab is a python package for configuring Morpheus training lab environments.
 Home-page: https://gitlab.com/morpheus_training/molab
 Author: Sean Jabro
 Author-email: sean.jabro@outlook.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `molab-0.4.1/molab.egg-info/SOURCES.txt` & `molab-0.4.3/molab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `molab-0.4.1/setup.py` & `molab-0.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 setup(
     author="Sean Jabro",
     author_email="sean.jabro@outlook.com",
     name='molab',
     license="MIT",
     description='molab is a python package for configuring Morpheus training lab environments.',
-    version='0.4.1',
+    version='0.4.3',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://gitlab.com/morpheus_training/molab',
     packages=find_packages() + find_packages(where='template_files'),
     package_dir={'template_files': 'template_files'},
     package_data={'molab': ['template_files/*.*']},
     python_requires=">=3.8",
```

