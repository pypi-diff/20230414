# Comparing `tmp/mingdaoyun-sdk-0.0.1.tar.gz` & `tmp/mingdaoyun-sdk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mingdaoyun-sdk-0.0.1.tar", last modified: Fri Apr 14 05:35:14 2023, max compression
+gzip compressed data, was "mingdaoyun-sdk-0.0.2.tar", last modified: Fri Apr 14 06:09:11 2023, max compression
```

## Comparing `mingdaoyun-sdk-0.0.1.tar` & `mingdaoyun-sdk-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 litao      (501) staff       (20)        0 2023-04-14 05:35:14.866644 mingdaoyun-sdk-0.0.1/
--rw-r--r--   0 litao      (501) staff       (20)      624 2023-04-14 05:35:14.866443 mingdaoyun-sdk-0.0.1/PKG-INFO
--rw-r--r--   0 litao      (501) staff       (20)      248 2023-04-14 05:33:16.000000 mingdaoyun-sdk-0.0.1/README.md
-drwxr-xr-x   0 litao      (501) staff       (20)        0 2023-04-14 05:35:14.865291 mingdaoyun-sdk-0.0.1/mingdaoyun-sdk/
--rw-r--r--   0 litao      (501) staff       (20)     4320 2023-04-14 05:27:56.000000 mingdaoyun-sdk-0.0.1/mingdaoyun-sdk/MingdaoOrg.py
--rw-r--r--   0 litao      (501) staff       (20)     8567 2023-04-14 05:26:53.000000 mingdaoyun-sdk-0.0.1/mingdaoyun-sdk/MingdaoYun.py
--rw-r--r--   0 litao      (501) staff       (20)        0 2023-04-14 05:20:52.000000 mingdaoyun-sdk-0.0.1/mingdaoyun-sdk/__init__.py
--rw-r--r--   0 litao      (501) staff       (20)      543 2023-04-14 05:27:18.000000 mingdaoyun-sdk-0.0.1/mingdaoyun-sdk/common.py
-drwxr-xr-x   0 litao      (501) staff       (20)        0 2023-04-14 05:35:14.866212 mingdaoyun-sdk-0.0.1/mingdaoyun_sdk.egg-info/
--rw-r--r--   0 litao      (501) staff       (20)      624 2023-04-14 05:35:14.000000 mingdaoyun-sdk-0.0.1/mingdaoyun_sdk.egg-info/PKG-INFO
--rw-r--r--   0 litao      (501) staff       (20)      280 2023-04-14 05:35:14.000000 mingdaoyun-sdk-0.0.1/mingdaoyun_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 litao      (501) staff       (20)        1 2023-04-14 05:35:14.000000 mingdaoyun-sdk-0.0.1/mingdaoyun_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 litao      (501) staff       (20)       15 2023-04-14 05:35:14.000000 mingdaoyun-sdk-0.0.1/mingdaoyun_sdk.egg-info/top_level.txt
--rw-r--r--   0 litao      (501) staff       (20)       38 2023-04-14 05:35:14.866698 mingdaoyun-sdk-0.0.1/setup.cfg
--rw-r--r--   0 litao      (501) staff       (20)     1422 2023-04-14 05:29:10.000000 mingdaoyun-sdk-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:09:11.066524 mingdaoyun-sdk-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-14 06:09:11.066524 mingdaoyun-sdk-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-14 06:08:57.000000 mingdaoyun-sdk-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:09:11.066524 mingdaoyun-sdk-0.0.2/mingdaoyun-sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-04-14 06:08:57.000000 mingdaoyun-sdk-0.0.2/mingdaoyun-sdk/MingdaoOrg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-04-14 06:08:57.000000 mingdaoyun-sdk-0.0.2/mingdaoyun-sdk/MingdaoYun.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 06:08:57.000000 mingdaoyun-sdk-0.0.2/mingdaoyun-sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-14 06:08:57.000000 mingdaoyun-sdk-0.0.2/mingdaoyun-sdk/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 06:09:11.066524 mingdaoyun-sdk-0.0.2/mingdaoyun_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-14 06:09:11.000000 mingdaoyun-sdk-0.0.2/mingdaoyun_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-14 06:09:11.000000 mingdaoyun-sdk-0.0.2/mingdaoyun_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 06:09:11.000000 mingdaoyun-sdk-0.0.2/mingdaoyun_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-14 06:09:11.000000 mingdaoyun-sdk-0.0.2/mingdaoyun_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 06:09:11.066524 mingdaoyun-sdk-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-14 06:08:57.000000 mingdaoyun-sdk-0.0.2/setup.py
```

### Comparing `mingdaoyun-sdk-0.0.1/PKG-INFO` & `mingdaoyun-sdk-0.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: mingdaoyun-sdk
-Version: 0.0.1
+Version: 0.0.2
 Summary: 针对mingdaoyun的API封装的Python-SDK包
-Home-page: https://dashen.tech
+Home-page: https://github.com/ghostlitao/mingdaoyun-python-sdk
 Author: Todd
-Author-email: ghostlitao@126.com
+Author-email: ghostlitao@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 mingdaoyun-Python-SDK
 -----
@@ -16,15 +16,15 @@
 针对mingdaoyun的API封装的Python-SDK包
 
 如果你在寻找PHP版本的,请点击(https://github.com/Lany-w/mingdaoyun-php-sdk)
 
 ## Installing
 
 ```shell
-$ pip install lany/mingdaoyun
+$ pip install mingdaoyun-sdk
 ```
 
 ## Usage
 
 ## License
 
 MIT
```

### Comparing `mingdaoyun-sdk-0.0.1/mingdaoyun-sdk/MingdaoOrg.py` & `mingdaoyun-sdk-0.0.2/mingdaoyun-sdk/MingdaoOrg.py`

 * *Files identical despite different names*

### Comparing `mingdaoyun-sdk-0.0.1/mingdaoyun-sdk/MingdaoYun.py` & `mingdaoyun-sdk-0.0.2/mingdaoyun-sdk/MingdaoYun.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,14 @@
         if not (self.appKey and self.sign and self.worksheetId):
             raise Exception('appKey,sign,table is required! ')
         auth_prams = {"appKey": self.appKey, "sign": self.sign, "worksheetId": self.worksheetId}
         if len(self.view) > 0:
             self.params["view"] = self.view
         if len(self.filters) > 0:
             self.params["filters"] = self.filters
-        print(self.params)
         data = http.post(self.host + uri, json={**self.params, **auth_prams}).json()
         return data
 
     def get_field_data_type(self, field: str) -> str:
         """
         或者字段类型
         :param field:
```

### Comparing `mingdaoyun-sdk-0.0.1/mingdaoyun-sdk/common.py` & `mingdaoyun-sdk-0.0.2/mingdaoyun-sdk/common.py`

 * *Files identical despite different names*

### Comparing `mingdaoyun-sdk-0.0.1/mingdaoyun_sdk.egg-info/PKG-INFO` & `mingdaoyun-sdk-0.0.2/mingdaoyun_sdk.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: mingdaoyun-sdk
-Version: 0.0.1
+Version: 0.0.2
 Summary: 针对mingdaoyun的API封装的Python-SDK包
-Home-page: https://dashen.tech
+Home-page: https://github.com/ghostlitao/mingdaoyun-python-sdk
 Author: Todd
-Author-email: ghostlitao@126.com
+Author-email: ghostlitao@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 mingdaoyun-Python-SDK
 -----
@@ -16,15 +16,15 @@
 针对mingdaoyun的API封装的Python-SDK包
 
 如果你在寻找PHP版本的,请点击(https://github.com/Lany-w/mingdaoyun-php-sdk)
 
 ## Installing
 
 ```shell
-$ pip install lany/mingdaoyun
+$ pip install mingdaoyun-sdk
 ```
 
 ## Usage
 
 ## License
 
 MIT
```

### Comparing `mingdaoyun-sdk-0.0.1/setup.py` & `mingdaoyun-sdk-0.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,27 +13,27 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     # 包的分发名称，使用字母、数字、_、-
     name="mingdaoyun-sdk",
     # 版本号, 版本号规范：https://www.python.org/dev/peps/pep-0440/
-    version="0.0.1",
+    version="0.0.2",
     # 作者名
     author="Todd",
     # 作者邮箱
-    author_email="ghostlitao@126.com",
+    author_email="ghostlitao@gmail.com",
     # 包的简介描述
     description="针对mingdaoyun的API封装的Python-SDK包",
     # 包的详细介绍(一般通过加载README.md)
     long_description=long_description,
     # 和上条命令配合使用，声明加载的是markdown文件
     long_description_content_type="text/markdown",
     # 项目开源地址
-    url="https://dashen.tech",
+    url="https://github.com/ghostlitao/mingdaoyun-python-sdk",
     # 如果项目由多个文件组成，我们可以使用find_packages()自动发现所有包和子包，而不是手动列出每个包，在这种情况下，包列表将是example_pkg
     packages=setuptools.find_packages(),
     # 关于包的其他元数据(metadata)
     classifiers=[
         # 该软件包仅与Python3兼容
         "Programming Language :: Python :: 3",
         # 根据MIT许可证开源
```

