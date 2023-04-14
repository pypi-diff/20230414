# Comparing `tmp/hadmin-1.1.3.tar.gz` & `tmp/hadmin-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hadmin-1.1.3.tar", last modified: Thu Mar 30 14:04:46 2023, max compression
+gzip compressed data, was "dist/hadmin-1.1.4.tar", last modified: Fri Apr 14 03:17:38 2023, max compression
```

## Comparing `hadmin-1.1.3.tar` & `hadmin-1.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 hofeng     (501) staff       (20)        0 2023-03-30 14:04:46.000000 hadmin-1.1.3/
--rw-r--r--   0 hofeng     (501) staff       (20)     1070 2022-11-18 12:30:16.000000 hadmin-1.1.3/LICENSE
--rw-r--r--   0 hofeng     (501) staff       (20)    16527 2023-03-30 14:04:46.000000 hadmin-1.1.3/PKG-INFO
--rw-r--r--   0 hofeng     (501) staff       (20)    16079 2023-03-30 13:57:51.000000 hadmin-1.1.3/README.md
-drwxr-xr-x   0 hofeng     (501) staff       (20)        0 2023-03-30 14:04:46.000000 hadmin-1.1.3/hadmin/
--rw-r--r--   0 hofeng     (501) staff       (20)        0 2022-11-18 12:31:48.000000 hadmin-1.1.3/hadmin/__init__.py
--rw-r--r--   0 hofeng     (501) staff       (20)    16540 2023-03-30 13:57:07.000000 hadmin-1.1.3/hadmin/mixins.py
-drwxr-xr-x   0 hofeng     (501) staff       (20)        0 2023-03-30 14:04:46.000000 hadmin-1.1.3/hadmin.egg-info/
--rw-r--r--   0 hofeng     (501) staff       (20)    16527 2023-03-30 14:04:46.000000 hadmin-1.1.3/hadmin.egg-info/PKG-INFO
--rw-r--r--   0 hofeng     (501) staff       (20)      211 2023-03-30 14:04:46.000000 hadmin-1.1.3/hadmin.egg-info/SOURCES.txt
--rw-r--r--   0 hofeng     (501) staff       (20)        1 2023-03-30 14:04:46.000000 hadmin-1.1.3/hadmin.egg-info/dependency_links.txt
--rw-r--r--   0 hofeng     (501) staff       (20)       20 2023-03-30 14:04:46.000000 hadmin-1.1.3/hadmin.egg-info/requires.txt
--rw-r--r--   0 hofeng     (501) staff       (20)        7 2023-03-30 14:04:46.000000 hadmin-1.1.3/hadmin.egg-info/top_level.txt
--rw-r--r--   0 hofeng     (501) staff       (20)       38 2023-03-30 14:04:46.000000 hadmin-1.1.3/setup.cfg
--rw-r--r--   0 hofeng     (501) staff       (20)      957 2023-03-30 13:58:11.000000 hadmin-1.1.3/setup.py
+drwxr-xr-x   0 hofeng     (501) staff       (20)        0 2023-04-14 03:17:38.000000 hadmin-1.1.4/
+-rw-r--r--   0 hofeng     (501) staff       (20)     1070 2023-04-14 03:08:57.000000 hadmin-1.1.4/LICENSE
+-rw-r--r--   0 hofeng     (501) staff       (20)    16564 2023-04-14 03:17:38.000000 hadmin-1.1.4/PKG-INFO
+-rw-r--r--   0 hofeng     (501) staff       (20)    16116 2023-04-14 03:13:44.000000 hadmin-1.1.4/README.md
+drwxr-xr-x   0 hofeng     (501) staff       (20)        0 2023-04-14 03:17:38.000000 hadmin-1.1.4/hadmin/
+-rw-r--r--   0 hofeng     (501) staff       (20)        0 2023-04-14 03:08:57.000000 hadmin-1.1.4/hadmin/__init__.py
+-rw-r--r--   0 hofeng     (501) staff       (20)    16689 2023-04-14 03:10:14.000000 hadmin-1.1.4/hadmin/mixins.py
+drwxr-xr-x   0 hofeng     (501) staff       (20)        0 2023-04-14 03:17:38.000000 hadmin-1.1.4/hadmin.egg-info/
+-rw-r--r--   0 hofeng     (501) staff       (20)    16564 2023-04-14 03:17:38.000000 hadmin-1.1.4/hadmin.egg-info/PKG-INFO
+-rw-r--r--   0 hofeng     (501) staff       (20)      211 2023-04-14 03:17:38.000000 hadmin-1.1.4/hadmin.egg-info/SOURCES.txt
+-rw-r--r--   0 hofeng     (501) staff       (20)        1 2023-04-14 03:17:38.000000 hadmin-1.1.4/hadmin.egg-info/dependency_links.txt
+-rw-r--r--   0 hofeng     (501) staff       (20)       20 2023-04-14 03:17:38.000000 hadmin-1.1.4/hadmin.egg-info/requires.txt
+-rw-r--r--   0 hofeng     (501) staff       (20)        7 2023-04-14 03:17:38.000000 hadmin-1.1.4/hadmin.egg-info/top_level.txt
+-rw-r--r--   0 hofeng     (501) staff       (20)       38 2023-04-14 03:17:38.000000 hadmin-1.1.4/setup.cfg
+-rw-r--r--   0 hofeng     (501) staff       (20)      957 2023-04-14 03:12:58.000000 hadmin-1.1.4/setup.py
```

### Comparing `hadmin-1.1.3/LICENSE` & `hadmin-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hadmin-1.1.3/PKG-INFO` & `hadmin-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hadmin
-Version: 1.1.3
+Version: 1.1.4
 Summary: 针对自动化给予前端配置文件的DRF封装
 Home-page: https://github.com/spirits001/python-HAdmin
 Author: 代码厨子
 Author-email: 15755153@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -698,7 +698,9 @@
 1.1.0  增加update
 
 1.1.1  修改默认tabs
 
 1.1.2  修复bug
 
 1.1.3  修复bug
+
+1.1.4  inlines内增加filter参数
```

### Comparing `hadmin-1.1.3/README.md` & `hadmin-1.1.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -683,8 +683,10 @@
 
 1.1.0  增加update
 
 1.1.1  修改默认tabs
 
 1.1.2  修复bug
 
-1.1.3  修复bug
+1.1.3  修复bug
+
+1.1.4  inlines内增加filter参数
```

### Comparing `hadmin-1.1.3/hadmin/mixins.py` & `hadmin-1.1.4/hadmin/mixins.py`

 * *Files 1% similar despite different names*

```diff
@@ -345,19 +345,23 @@
                         del inline_create['fields'][field_value.field_name]
                     self._build_create(inline_create, inline_custom, field_value)
                 create['inlines'][inline_key] = {
                     'label': inline_value['label'] if 'label' in inline_value else inline_serializer.Meta.model._meta.verbose_name,
                     'create': inline_create,
                     'limit': inline_value['limit'] if 'limit' in inline_value else self.inlines_limit,
                     'api': inline_value['api'] if 'api' in inline_value else '',
-                    'field': field
+                    'field': field,
+                    'filter': inline_value['filter'] if 'filter' in inline_value else []
                 }
                 create['fields'][inline_key] = []
         res = {
             "filter": filter_data,
             "create": create,
             "update": update,
             "list": self._build_list(self.list_class),  # 列表字段生成器，业务逻辑和创建的差不多了
             "read": self._build_list(self.read_class),  # 读取格式数据，业务逻辑和创建的差不多了
             "extra": self.extra
         }
         return Response(res)
+
+# python setup.py sdist bdist_wheel
+# twine upload dist/*
```

### Comparing `hadmin-1.1.3/hadmin.egg-info/PKG-INFO` & `hadmin-1.1.4/hadmin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hadmin
-Version: 1.1.3
+Version: 1.1.4
 Summary: 针对自动化给予前端配置文件的DRF封装
 Home-page: https://github.com/spirits001/python-HAdmin
 Author: 代码厨子
 Author-email: 15755153@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -698,7 +698,9 @@
 1.1.0  增加update
 
 1.1.1  修改默认tabs
 
 1.1.2  修复bug
 
 1.1.3  修复bug
+
+1.1.4  inlines内增加filter参数
```

### Comparing `hadmin-1.1.3/setup.py` & `hadmin-1.1.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="hadmin",  # 模块名称
-    version="1.1.3",  # 当前版本
+    version="1.1.4",  # 当前版本
     author="代码厨子",  # 作者
     author_email="15755153@qq.com",  # 作者邮箱
     description="针对自动化给予前端配置文件的DRF封装",  # 模块简介
     long_description=long_description,  # 模块详细介绍
     long_description_content_type="text/markdown",  # 模块详细介绍格式
     url="https://github.com/spirits001/python-HAdmin",  # 模块github地址
     packages=setuptools.find_packages(),  # 自动找到项目中导入的模块
```

