# Comparing `tmp/seven_cloudapp_ppmt-1.0.8.tar.gz` & `tmp/seven_cloudapp_ppmt-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\seven_cloudapp_ppmt-1.0.8.tar", last modified: Tue Apr 27 03:44:56 2021, max compression
+gzip compressed data, was "dist\seven_cloudapp_ppmt-1.0.9.tar", last modified: Tue May 11 06:53:16 2021, max compression
```

## Comparing `seven_cloudapp_ppmt-1.0.8.tar` & `seven_cloudapp_ppmt-1.0.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2021-04-27 03:44:56.623711 seven_cloudapp_ppmt-1.0.8/
--rw-rw-rw-   0        0        0     1064 2021-04-27 03:44:56.622710 seven_cloudapp_ppmt-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      186 2021-04-27 03:44:33.000000 seven_cloudapp_ppmt-1.0.8/README.md
--rw-rw-rw-   0        0        0       42 2021-04-27 03:44:56.625710 seven_cloudapp_ppmt-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1315 2021-04-27 03:44:43.000000 seven_cloudapp_ppmt-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2021-04-27 03:44:56.485710 seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt/
--rw-rw-rw-   0        0        0      141 2021-04-19 07:11:41.000000 seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt/__init__.py
-drwxrwxrwx   0        0        0        0 2021-04-27 03:44:56.513710 seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt/handlers/
--rw-rw-rw-   0        0        0      166 2021-04-19 07:11:41.000000 seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt/handlers/__init__.py
-drwxrwxrwx   0        0        0        0 2021-04-27 03:44:56.530710 seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt/handlers/client/
--rw-rw-rw-   0        0        0      202 2021-04-19 07:11:41.000000 seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt/handlers/client/__init__.py
--rw-rw-rw-   0        0        0    11111 2021-04-27 03:34:19.000000 seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt/handlers/client/act.py
--rw-rw-rw-   0        0        0    61223 2021-04-27 03:34:19.000000 seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt/handlers/client/lottery.py
--rw-rw-rw-   0        0        0    26378 2021-04-19 07:11:41.000000 seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt/handlers/client/user.py
-drwxrwxrwx   0        0        0        0 2021-04-27 03:44:56.573711 seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt/handlers/server/
--rw-rw-rw-   0        0        0      262 2021-04-19 07:11:41.000000 seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt/handlers/server/__init__.py
--rw-rw-rw-   0        0        0    22448 2021-04-19 07:11:41.000000 seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt/handlers/server/act_s.py
--rw-rw-rw-   0        0        0     5172 2021-04-19 07:11:41.000000 seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt/handlers/server/app_s.py
--rw-rw-rw-   0        0        0     8919 2021-04-27 03:43:53.000000 seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt/handlers/server/machine_s.py
--rw-rw-rw-   0        0        0    20063 2021-04-19 07:11:41.000000 seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt/handlers/server/order_s.py
--rw-rw-rw-   0        0        0    12584 2021-04-19 07:11:41.000000 seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt/handlers/server/prize_s.py
--rw-rw-rw-   0        0        0    11882 2021-04-19 07:11:41.000000 seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt/handlers/server/report_s.py
--rw-rw-rw-   0        0        0     2344 2021-04-19 07:11:41.000000 seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt/handlers/server/throw_s.py
--rw-rw-rw-   0        0        0    22183 2021-04-19 07:11:41.000000 seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt/handlers/server/user_s.py
-drwxrwxrwx   0        0        0        0 2021-04-27 03:44:56.580709 seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt/models/
--rw-rw-rw-   0        0        0      141 2021-04-19 07:11:42.000000 seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt/models/__init__.py
-drwxrwxrwx   0        0        0        0 2021-04-27 03:44:56.584710 seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt/models/db_models/
--rw-rw-rw-   0        0        0      141 2021-04-19 07:11:42.000000 seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt/models/db_models/__init__.py
-drwxrwxrwx   0        0        0        0 2021-04-27 03:44:56.597710 seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt/models/db_models/act/
--rw-rw-rw-   0        0        0       45 2021-04-19 07:11:42.000000 seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt/models/db_models/act/__init__.py
--rw-rw-rw-   0        0        0     3243 2021-04-19 07:11:42.000000 seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt/models/db_models/act/act_info_model.py
--rw-rw-rw-   0        0        0     2959 2021-04-19 07:11:42.000000 seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt/models/db_models/act/act_prize_model.py
-drwxrwxrwx   0        0        0        0 2021-04-27 03:44:56.606710 seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt/models/db_models/machine/
--rw-rw-rw-   0        0        0       31 2021-04-19 07:11:42.000000 seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt/models/db_models/machine/__init__.py
--rw-rw-rw-   0        0        0     2922 2021-04-19 07:11:42.000000 seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt/models/db_models/machine/machine_info_model.py
-drwxrwxrwx   0        0        0        0 2021-04-27 03:44:56.616710 seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt/models/db_models/prize/
--rw-rw-rw-   0        0        0       31 2021-04-19 07:11:42.000000 seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt/models/db_models/prize/__init__.py
--rw-rw-rw-   0        0        0     3298 2021-04-19 07:11:42.000000 seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt/models/db_models/prize/prize_roster_model.py
--rw-rw-rw-   0        0        0     7609 2021-04-19 07:11:42.000000 seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt/route.py
-drwxrwxrwx   0        0        0        0 2021-04-27 03:44:56.507710 seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt.egg-info/
--rw-rw-rw-   0        0        0     1064 2021-04-27 03:44:56.000000 seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1442 2021-04-27 03:44:56.000000 seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-04-27 03:44:56.000000 seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2021-04-27 03:44:56.000000 seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2021-04-27 03:44:56.000000 seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2021-05-11 06:53:16.255043 seven_cloudapp_ppmt-1.0.9/
+-rw-rw-rw-   0        0        0     1064 2021-05-11 06:53:16.254043 seven_cloudapp_ppmt-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      186 2021-05-11 06:52:33.000000 seven_cloudapp_ppmt-1.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2021-05-11 06:53:16.258042 seven_cloudapp_ppmt-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1315 2021-05-11 06:52:45.000000 seven_cloudapp_ppmt-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2021-05-11 06:53:16.037043 seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt/
+-rw-rw-rw-   0        0        0      141 2021-04-19 07:11:41.000000 seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt/__init__.py
+drwxrwxrwx   0        0        0        0 2021-05-11 06:53:16.099041 seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt/handlers/
+-rw-rw-rw-   0        0        0      166 2021-04-19 07:11:41.000000 seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt/handlers/__init__.py
+drwxrwxrwx   0        0        0        0 2021-05-11 06:53:16.125043 seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt/handlers/client/
+-rw-rw-rw-   0        0        0      202 2021-04-19 07:11:41.000000 seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt/handlers/client/__init__.py
+-rw-rw-rw-   0        0        0    11111 2021-04-27 03:34:19.000000 seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt/handlers/client/act.py
+-rw-rw-rw-   0        0        0    61223 2021-04-27 03:34:19.000000 seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt/handlers/client/lottery.py
+-rw-rw-rw-   0        0        0    26378 2021-05-11 06:51:41.000000 seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt/handlers/client/user.py
+drwxrwxrwx   0        0        0        0 2021-05-11 06:53:16.176041 seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt/handlers/server/
+-rw-rw-rw-   0        0        0      262 2021-04-19 07:11:41.000000 seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt/handlers/server/__init__.py
+-rw-rw-rw-   0        0        0    22448 2021-04-19 07:11:41.000000 seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt/handlers/server/act_s.py
+-rw-rw-rw-   0        0        0     5172 2021-04-19 07:11:41.000000 seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt/handlers/server/app_s.py
+-rw-rw-rw-   0        0        0     8919 2021-04-27 03:43:53.000000 seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt/handlers/server/machine_s.py
+-rw-rw-rw-   0        0        0    20063 2021-04-19 07:11:41.000000 seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt/handlers/server/order_s.py
+-rw-rw-rw-   0        0        0    12584 2021-04-19 07:11:41.000000 seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt/handlers/server/prize_s.py
+-rw-rw-rw-   0        0        0    11882 2021-04-19 07:11:41.000000 seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt/handlers/server/report_s.py
+-rw-rw-rw-   0        0        0     2344 2021-04-19 07:11:41.000000 seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt/handlers/server/throw_s.py
+-rw-rw-rw-   0        0        0    22183 2021-04-19 07:11:41.000000 seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt/handlers/server/user_s.py
+drwxrwxrwx   0        0        0        0 2021-05-11 06:53:16.181043 seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt/models/
+-rw-rw-rw-   0        0        0      141 2021-04-19 07:11:42.000000 seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt/models/__init__.py
+drwxrwxrwx   0        0        0        0 2021-05-11 06:53:16.197044 seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt/models/db_models/
+-rw-rw-rw-   0        0        0      141 2021-04-19 07:11:42.000000 seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt/models/db_models/__init__.py
+drwxrwxrwx   0        0        0        0 2021-05-11 06:53:16.213043 seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt/models/db_models/act/
+-rw-rw-rw-   0        0        0       45 2021-04-19 07:11:42.000000 seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt/models/db_models/act/__init__.py
+-rw-rw-rw-   0        0        0     3243 2021-04-19 07:11:42.000000 seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt/models/db_models/act/act_info_model.py
+-rw-rw-rw-   0        0        0     2959 2021-04-19 07:11:42.000000 seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt/models/db_models/act/act_prize_model.py
+drwxrwxrwx   0        0        0        0 2021-05-11 06:53:16.223047 seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt/models/db_models/machine/
+-rw-rw-rw-   0        0        0       31 2021-04-19 07:11:42.000000 seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt/models/db_models/machine/__init__.py
+-rw-rw-rw-   0        0        0     2922 2021-04-19 07:11:42.000000 seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt/models/db_models/machine/machine_info_model.py
+drwxrwxrwx   0        0        0        0 2021-05-11 06:53:16.248046 seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt/models/db_models/prize/
+-rw-rw-rw-   0        0        0       31 2021-04-19 07:11:42.000000 seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt/models/db_models/prize/__init__.py
+-rw-rw-rw-   0        0        0     3298 2021-04-19 07:11:42.000000 seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt/models/db_models/prize/prize_roster_model.py
+-rw-rw-rw-   0        0        0     7609 2021-04-19 07:11:42.000000 seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt/route.py
+drwxrwxrwx   0        0        0        0 2021-05-11 06:53:16.094041 seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt.egg-info/
+-rw-rw-rw-   0        0        0     1064 2021-05-11 06:53:15.000000 seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1442 2021-05-11 06:53:15.000000 seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-05-11 06:53:15.000000 seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2021-05-11 06:53:15.000000 seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2021-05-11 06:53:15.000000 seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt.egg-info/top_level.txt
```

### Comparing `seven_cloudapp_ppmt-1.0.8/PKG-INFO` & `seven_cloudapp_ppmt-1.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: seven_cloudapp_ppmt
-Version: 1.0.8
+Version: 1.0.9
 Summary: seven cloudapp ppmt
 Home-page: http://gitlab.tdtech.gao7.com/TaoBaoCloud/seven_cloudapp_ppmt.git
 Author: seven
 Author-email: tech@gao7.com
 License: MIT
 Description: # seven_cloudapp_ppmt
         
         ## 天志互联Python淘宝云应用框架库(潮玩盲盒)
         
-        ### 1.0.8 更新内容
+        ### 1.0.9 更新内容
         * 潮玩盲盒v2.0整合
         
         ### 1.0.2 更新内容
         * 框架内容添加
         
 Platform: UNKNOWN
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `seven_cloudapp_ppmt-1.0.8/setup.py` & `seven_cloudapp_ppmt-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="seven_cloudapp_ppmt",
-    version="1.0.8",
+    version="1.0.9",
     author="seven",
     author_email="tech@gao7.com",
     description="seven cloudapp ppmt",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     url="http://gitlab.tdtech.gao7.com/TaoBaoCloud/seven_cloudapp_ppmt.git",
```

### Comparing `seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt/handlers/client/act.py` & `seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt/handlers/client/act.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt/handlers/client/lottery.py` & `seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt/handlers/client/lottery.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt/handlers/client/user.py` & `seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt/handlers/client/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 """
 :Author: HuangJingCan
 :Date: 2020-05-19 11:33:16
-:LastEditTime: 2021-04-15 14:48:26
-:LastEditors: HuangJingCan
+@LastEditTime: 2021-05-11 14:50:27
+@LastEditors: HuangJianYi
 :description: 用户处理
 """
 from seven_cloudapp.handlers.top_base import *
 
 from seven_cloudapp.models.behavior_model import *
 from seven_cloudapp.models.seven_model import PageInfo
 from seven_cloudapp.models.db_models.user.user_info_model import *
@@ -437,15 +437,15 @@
             params = [act_id, machine_id]
         act_prize_list_dict = ActPrizeModel(context=self).get_dict_list("act_id=%s and is_prize_notice=0", params=[act_id])
         if act_prize_list_dict:
             prize_id_list = [str(i["id"]) for i in act_prize_list_dict]
             if len(prize_id_list) > 0:
                 prize_ids = ",".join(prize_id_list)
                 condition += " and prize_id not in (" + prize_ids + ")"
-        condition += f" and create_date>'{TimeHelper.add_hours_by_format_time(hour=7)}'"
+        condition += f" and create_date>'{TimeHelper.add_hours_by_format_time(hour=-1)}'"
         prize_roster_model = PrizeRosterModel(context=self)
         page_list = prize_roster_model.get_dict_list(condition, "", "create_date desc", str(page_size), "user_nick,prize_name,tag_id,machine_name", params)
         total = int(len(page_list))
         if total == 0:
             page_list = []
         else:
             for i in range(len(page_list)):
```

### Comparing `seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt/handlers/server/act_s.py` & `seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt/handlers/server/act_s.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt/handlers/server/app_s.py` & `seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt/handlers/server/app_s.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt/handlers/server/machine_s.py` & `seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt/handlers/server/machine_s.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt/handlers/server/order_s.py` & `seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt/handlers/server/order_s.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt/handlers/server/prize_s.py` & `seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt/handlers/server/prize_s.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt/handlers/server/report_s.py` & `seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt/handlers/server/report_s.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt/handlers/server/throw_s.py` & `seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt/handlers/server/throw_s.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt/handlers/server/user_s.py` & `seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt/handlers/server/user_s.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt/models/db_models/act/act_info_model.py` & `seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt/models/db_models/act/act_info_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt/models/db_models/act/act_prize_model.py` & `seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt/models/db_models/act/act_prize_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt/models/db_models/machine/machine_info_model.py` & `seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt/models/db_models/machine/machine_info_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt/models/db_models/prize/prize_roster_model.py` & `seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt/models/db_models/prize/prize_roster_model.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt/route.py` & `seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt/route.py`

 * *Files identical despite different names*

### Comparing `seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt.egg-info/PKG-INFO` & `seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: seven-cloudapp-ppmt
-Version: 1.0.8
+Version: 1.0.9
 Summary: seven cloudapp ppmt
 Home-page: http://gitlab.tdtech.gao7.com/TaoBaoCloud/seven_cloudapp_ppmt.git
 Author: seven
 Author-email: tech@gao7.com
 License: MIT
 Description: # seven_cloudapp_ppmt
         
         ## 天志互联Python淘宝云应用框架库(潮玩盲盒)
         
-        ### 1.0.8 更新内容
+        ### 1.0.9 更新内容
         * 潮玩盲盒v2.0整合
         
         ### 1.0.2 更新内容
         * 框架内容添加
         
 Platform: UNKNOWN
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `seven_cloudapp_ppmt-1.0.8/seven_cloudapp_ppmt.egg-info/SOURCES.txt` & `seven_cloudapp_ppmt-1.0.9/seven_cloudapp_ppmt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

