# Comparing `tmp/dcb_admin_page_generator-0.0.5.tar.gz` & `tmp/dcb_admin_page_generator-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcb_admin_page_generator-0.0.5.tar", last modified: Tue Apr 11 09:12:32 2023, max compression
+gzip compressed data, was "dcb_admin_page_generator-0.0.6.tar", last modified: Fri Apr 14 02:29:23 2023, max compression
```

## Comparing `dcb_admin_page_generator-0.0.5.tar` & `dcb_admin_page_generator-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 09:12:32.056390 dcb_admin_page_generator-0.0.5/
--rw-rw-rw-   0        0        0     1091 2023-03-29 08:48:00.000000 dcb_admin_page_generator-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      664 2023-04-11 09:12:32.055393 dcb_admin_page_generator-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-04-11 07:24:11.000000 dcb_admin_page_generator-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 09:12:32.036443 dcb_admin_page_generator-0.0.5/dcb_admin_page_generator/
--rw-rw-rw-   0        0        0       25 2023-03-30 02:20:19.000000 dcb_admin_page_generator-0.0.5/dcb_admin_page_generator/__init__.py
--rw-rw-rw-   0        0        0     2781 2023-04-11 08:44:31.000000 dcb_admin_page_generator-0.0.5/dcb_admin_page_generator/main.py
--rw-rw-rw-   0        0        0    10139 2023-04-11 08:45:36.000000 dcb_admin_page_generator-0.0.5/dcb_admin_page_generator/page_class.py
-drwxrwxrwx   0        0        0        0 2023-04-11 09:12:32.054394 dcb_admin_page_generator-0.0.5/dcb_admin_page_generator/template/
--rw-rw-rw-   0        0        0        0 2023-04-11 07:48:27.000000 dcb_admin_page_generator-0.0.5/dcb_admin_page_generator/template/__init__.py
--rw-rw-rw-   0        0        0     2531 2023-04-11 07:12:32.000000 dcb_admin_page_generator-0.0.5/dcb_admin_page_generator/template/add_or_edit.vue
--rw-rw-rw-   0        0        0     2258 2023-04-11 07:11:16.000000 dcb_admin_page_generator-0.0.5/dcb_admin_page_generator/template/dialog_add_or_edit.vue
--rw-rw-rw-   0        0        0     2762 2023-04-11 07:10:16.000000 dcb_admin_page_generator-0.0.5/dcb_admin_page_generator/template/dialog_list.vue
--rw-rw-rw-   0        0        0     5529 2023-04-06 07:21:58.000000 dcb_admin_page_generator-0.0.5/dcb_admin_page_generator/template/index.vue
-drwxrwxrwx   0        0        0        0 2023-04-11 09:12:32.041429 dcb_admin_page_generator-0.0.5/dcb_admin_page_generator.egg-info/
--rw-rw-rw-   0        0        0      664 2023-04-11 09:12:31.000000 dcb_admin_page_generator-0.0.5/dcb_admin_page_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      574 2023-04-11 09:12:31.000000 dcb_admin_page_generator-0.0.5/dcb_admin_page_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 09:12:31.000000 dcb_admin_page_generator-0.0.5/dcb_admin_page_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-04-11 09:12:31.000000 dcb_admin_page_generator-0.0.5/dcb_admin_page_generator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 09:12:32.056390 dcb_admin_page_generator-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      685 2023-04-11 09:12:19.000000 dcb_admin_page_generator-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 02:29:23.010128 dcb_admin_page_generator-0.0.6/
+-rw-rw-rw-   0        0        0     1088 2023-04-12 01:46:29.000000 dcb_admin_page_generator-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      664 2023-04-14 02:29:23.009131 dcb_admin_page_generator-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-04-11 07:24:11.000000 dcb_admin_page_generator-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 02:29:22.952305 dcb_admin_page_generator-0.0.6/dcb_admin_page_generator/
+-rw-rw-rw-   0        0        0       25 2023-03-30 02:20:19.000000 dcb_admin_page_generator-0.0.6/dcb_admin_page_generator/__init__.py
+-rw-rw-rw-   0        0        0     6617 2023-04-14 02:07:21.000000 dcb_admin_page_generator-0.0.6/dcb_admin_page_generator/config.py
+-rw-rw-rw-   0        0        0     3005 2023-04-14 02:16:54.000000 dcb_admin_page_generator-0.0.6/dcb_admin_page_generator/main.py
+-rw-rw-rw-   0        0        0    10139 2023-04-11 08:45:36.000000 dcb_admin_page_generator-0.0.6/dcb_admin_page_generator/page_class.py
+drwxrwxrwx   0        0        0        0 2023-04-14 02:29:23.008134 dcb_admin_page_generator-0.0.6/dcb_admin_page_generator/template/
+-rw-rw-rw-   0        0        0        0 2023-04-11 07:48:27.000000 dcb_admin_page_generator-0.0.6/dcb_admin_page_generator/template/__init__.py
+-rw-rw-rw-   0        0        0     2531 2023-04-11 07:12:32.000000 dcb_admin_page_generator-0.0.6/dcb_admin_page_generator/template/add_or_edit.vue
+-rw-rw-rw-   0        0        0     2258 2023-04-11 07:11:16.000000 dcb_admin_page_generator-0.0.6/dcb_admin_page_generator/template/dialog_add_or_edit.vue
+-rw-rw-rw-   0        0        0     2762 2023-04-11 07:10:16.000000 dcb_admin_page_generator-0.0.6/dcb_admin_page_generator/template/dialog_list.vue
+-rw-rw-rw-   0        0        0     5529 2023-04-06 07:21:58.000000 dcb_admin_page_generator-0.0.6/dcb_admin_page_generator/template/index.vue
+drwxrwxrwx   0        0        0        0 2023-04-14 02:29:22.958289 dcb_admin_page_generator-0.0.6/dcb_admin_page_generator.egg-info/
+-rw-rw-rw-   0        0        0      664 2023-04-14 02:29:22.000000 dcb_admin_page_generator-0.0.6/dcb_admin_page_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      609 2023-04-14 02:29:22.000000 dcb_admin_page_generator-0.0.6/dcb_admin_page_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 02:29:22.000000 dcb_admin_page_generator-0.0.6/dcb_admin_page_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-04-14 02:29:22.000000 dcb_admin_page_generator-0.0.6/dcb_admin_page_generator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-14 02:29:23.010128 dcb_admin_page_generator-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      695 2023-04-14 02:29:12.000000 dcb_admin_page_generator-0.0.6/setup.py
```

### Comparing `dcb_admin_page_generator-0.0.5/LICENSE` & `dcb_admin_page_generator-0.0.6/LICENSE`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-Copyright (c) 2019 The Python Packaging Authority
+MIT License
+
+Copyright (c) 2023 Wangyenzhi
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -12,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `dcb_admin_page_generator-0.0.5/PKG-INFO` & `dcb_admin_page_generator-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcb_admin_page_generator
-Version: 0.0.5
+Version: 0.0.6
 Summary: A small example package
 Home-page: https://github.com/pypa/sampleproject
 Author: wyz
 Author-email: 846630116@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dcb_admin_page_generator-0.0.5/dcb_admin_page_generator/main.py` & `dcb_admin_page_generator-0.0.6/dcb_admin_page_generator/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 import json
 from .page_class import *
+from .config import template_data
 
 
-def deal_yapi(configuration, file_path):
-    print('file_path', file_path)
-    yapi_url = input('请输入获取数据链接的YapiURL')
-    id_dict = get_id(yapi_url, configuration)
-    resp = requests.get(f'{configuration["serverUrl"]}{configuration["getInfoPath"]}', params=id_dict)
-    resp_text = json.loads(resp.text)
+def deal_yapi(configuration, file_path,yapi_type):
+    # print('file_path', file_path)
+    yapi_url = input('请输入获取数据链接的YapiURL(默认配置直接敲回车)')
+    if yapi_url:
+        id_dict = get_id(yapi_url, configuration)
+        resp = requests.get(f'{configuration["serverUrl"]}{configuration["getInfoPath"]}', params=id_dict)
+        resp_text = json.loads(resp.text)
+    else:
+        resp_text = template_data[yapi_type]
+    # print('resp_text', resp_text)
     resp_query_path = resp_text["data"]["query_path"]
     resp_body = json.loads(resp_text["data"]["res_body"])
     resp_body_other = json.loads(resp_text["data"]["req_body_other"])
-
     return resp_query_path, resp_body['properties'], resp_body_other['properties']
+    # else:
 
 
 def generate_page_list(configuration, generator_title, file_path, need_dialog=False):
-    resp_query_path, resp_body, resp_body_other = deal_yapi(configuration, file_path)
+    resp_query_path, resp_body, resp_body_other = deal_yapi(configuration, file_path,'list')
     resp_body = resp_body['data']['properties']['list']['items']['properties']
     return GenerateList(generator_title, resp_query_path, resp_body_other, resp_body, f'{"dialog_" if need_dialog else ""}list')
 
 
 def generate_page_add(configuration, generator_title, file_path, need_dialog=False):
-    resp_query_path, resp_body, resp_body_other = deal_yapi(configuration, file_path)
+    resp_query_path, resp_body, resp_body_other = deal_yapi(configuration, file_path,'add')
     return GenerateAdd(generator_title, resp_query_path, resp_body_other, resp_body, f'{"dialog_" if need_dialog else ""}add')
 
 
 def generator(config, generator_title, generator_type, file_path):
     # page_type = input('请输入想要生成的Page Type(list,add,form,dialog_list,dialog_add,dialog_form)')
     page_dict = {'1': 'list', 'list': 'list',
                  '2': 'add', 'add': 'add',
```

### Comparing `dcb_admin_page_generator-0.0.5/dcb_admin_page_generator/page_class.py` & `dcb_admin_page_generator-0.0.6/dcb_admin_page_generator/page_class.py`

 * *Files identical despite different names*

### Comparing `dcb_admin_page_generator-0.0.5/dcb_admin_page_generator/template/add_or_edit.vue` & `dcb_admin_page_generator-0.0.6/dcb_admin_page_generator/template/add_or_edit.vue`

 * *Files identical despite different names*

### Comparing `dcb_admin_page_generator-0.0.5/dcb_admin_page_generator/template/dialog_add_or_edit.vue` & `dcb_admin_page_generator-0.0.6/dcb_admin_page_generator/template/dialog_add_or_edit.vue`

 * *Files identical despite different names*

### Comparing `dcb_admin_page_generator-0.0.5/dcb_admin_page_generator/template/dialog_list.vue` & `dcb_admin_page_generator-0.0.6/dcb_admin_page_generator/template/dialog_list.vue`

 * *Files identical despite different names*

### Comparing `dcb_admin_page_generator-0.0.5/dcb_admin_page_generator/template/index.vue` & `dcb_admin_page_generator-0.0.6/dcb_admin_page_generator/template/index.vue`

 * *Files identical despite different names*

### Comparing `dcb_admin_page_generator-0.0.5/dcb_admin_page_generator.egg-info/PKG-INFO` & `dcb_admin_page_generator-0.0.6/dcb_admin_page_generator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcb-admin-page-generator
-Version: 0.0.5
+Version: 0.0.6
 Summary: A small example package
 Home-page: https://github.com/pypa/sampleproject
 Author: wyz
 Author-email: 846630116@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dcb_admin_page_generator-0.0.5/dcb_admin_page_generator.egg-info/SOURCES.txt` & `dcb_admin_page_generator-0.0.6/dcb_admin_page_generator.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 setup.py
 dcb_admin_page_generator/__init__.py
+dcb_admin_page_generator/config.py
 dcb_admin_page_generator/main.py
 dcb_admin_page_generator/page_class.py
 dcb_admin_page_generator.egg-info/PKG-INFO
 dcb_admin_page_generator.egg-info/SOURCES.txt
 dcb_admin_page_generator.egg-info/dependency_links.txt
 dcb_admin_page_generator.egg-info/top_level.txt
 dcb_admin_page_generator/template/__init__.py
```

### Comparing `dcb_admin_page_generator-0.0.5/setup.py` & `dcb_admin_page_generator-0.0.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dcb_admin_page_generator",
-    version="0.0.5",
+    version="0.0.6",
     author="wyz",
     author_email="846630116@qq.com",
     description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pypa/sampleproject",
-    packages=setuptools.find_packages(exclude=['ceshi']),
+    packages=setuptools.find_packages(exclude=['ceshi', 'config']),
     package_data={'': ['*.vue']},
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
```

