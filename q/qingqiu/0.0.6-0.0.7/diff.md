# Comparing `tmp/qingqiu-0.0.6.tar.gz` & `tmp/qingqiu-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\qingqiu-0.0.6.tar", last modified: Fri Apr  7 02:36:50 2023, max compression
+gzip compressed data, was "dist\qingqiu-0.0.7.tar", last modified: Fri Apr 14 02:01:44 2023, max compression
```

## Comparing `qingqiu-0.0.6.tar` & `qingqiu-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 02:36:50.000000 qingqiu-0.0.6/
--rw-rw-rw-   0        0        0      849 2023-04-07 02:36:50.000000 qingqiu-0.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-07 02:36:50.000000 qingqiu-0.0.6/qingqiu/
--rw-rw-rw-   0        0        0      929 2023-03-30 07:06:53.000000 qingqiu-0.0.6/qingqiu/__init__.py
--rw-rw-rw-   0        0        0    28054 2023-04-06 07:11:00.000000 qingqiu-0.0.6/qingqiu/check.py
--rw-rw-rw-   0        0        0      958 2022-08-08 12:28:20.000000 qingqiu-0.0.6/qingqiu/conftest.py
--rw-rw-rw-   0        0        0      404 2023-03-30 08:08:56.000000 qingqiu-0.0.6/qingqiu/gl.py
--rw-rw-rw-   0        0        0     7965 2022-08-10 05:44:02.000000 qingqiu-0.0.6/qingqiu/handle.py
--rw-rw-rw-   0        0        0      603 2022-08-10 05:42:27.000000 qingqiu-0.0.6/qingqiu/help.py
--rw-rw-rw-   0        0        0    14208 2023-04-03 07:49:31.000000 qingqiu-0.0.6/qingqiu/qing.py
--rw-rw-rw-   0        0        0    14865 2023-04-07 02:31:45.000000 qingqiu-0.0.6/qingqiu/qiu.py
--rw-rw-rw-   0        0        0       73 2022-07-28 07:10:30.000000 qingqiu-0.0.6/qingqiu/test.py
--rw-rw-rw-   0        0        0     4117 2023-03-31 03:10:28.000000 qingqiu-0.0.6/qingqiu/tools.py
--rw-rw-rw-   0        0        0    17539 2022-08-24 05:50:53.000000 qingqiu-0.0.6/qingqiu/transform.py
-drwxrwxrwx   0        0        0        0 2023-04-07 02:36:50.000000 qingqiu-0.0.6/qingqiu.egg-info/
--rw-rw-rw-   0        0        0      849 2023-04-07 02:36:49.000000 qingqiu-0.0.6/qingqiu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      386 2023-04-07 02:36:49.000000 qingqiu-0.0.6/qingqiu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 02:36:49.000000 qingqiu-0.0.6/qingqiu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-04-07 02:36:49.000000 qingqiu-0.0.6/qingqiu.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       78 2023-04-07 02:36:49.000000 qingqiu-0.0.6/qingqiu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-07 02:36:49.000000 qingqiu-0.0.6/qingqiu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-07 02:36:50.000000 qingqiu-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1394 2023-04-07 02:36:29.000000 qingqiu-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 02:01:44.000000 qingqiu-0.0.7/
+-rw-rw-rw-   0        0        0      849 2023-04-14 02:01:44.000000 qingqiu-0.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-14 02:01:44.000000 qingqiu-0.0.7/qingqiu/
+-rw-rw-rw-   0        0        0      929 2023-04-07 12:02:13.000000 qingqiu-0.0.7/qingqiu/__init__.py
+-rw-rw-rw-   0        0        0    28054 2023-04-06 07:11:00.000000 qingqiu-0.0.7/qingqiu/check.py
+-rw-rw-rw-   0        0        0      958 2022-08-08 12:28:20.000000 qingqiu-0.0.7/qingqiu/conftest.py
+-rw-rw-rw-   0        0        0      404 2023-03-30 08:08:56.000000 qingqiu-0.0.7/qingqiu/gl.py
+-rw-rw-rw-   0        0        0     7965 2022-08-10 05:44:02.000000 qingqiu-0.0.7/qingqiu/handle.py
+-rw-rw-rw-   0        0        0      603 2022-08-10 05:42:27.000000 qingqiu-0.0.7/qingqiu/help.py
+-rw-rw-rw-   0        0        0    14208 2023-04-03 07:49:31.000000 qingqiu-0.0.7/qingqiu/qing.py
+-rw-rw-rw-   0        0        0    14945 2023-04-11 10:15:21.000000 qingqiu-0.0.7/qingqiu/qiu.py
+-rw-rw-rw-   0        0        0       73 2022-07-28 07:10:30.000000 qingqiu-0.0.7/qingqiu/test.py
+-rw-rw-rw-   0        0        0     4017 2023-04-10 02:23:22.000000 qingqiu-0.0.7/qingqiu/tools.py
+-rw-rw-rw-   0        0        0    17539 2022-08-24 05:50:53.000000 qingqiu-0.0.7/qingqiu/transform.py
+drwxrwxrwx   0        0        0        0 2023-04-14 02:01:44.000000 qingqiu-0.0.7/qingqiu.egg-info/
+-rw-rw-rw-   0        0        0      849 2023-04-14 02:01:43.000000 qingqiu-0.0.7/qingqiu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      386 2023-04-14 02:01:43.000000 qingqiu-0.0.7/qingqiu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 02:01:43.000000 qingqiu-0.0.7/qingqiu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-04-14 02:01:43.000000 qingqiu-0.0.7/qingqiu.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       78 2023-04-14 02:01:43.000000 qingqiu-0.0.7/qingqiu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-14 02:01:43.000000 qingqiu-0.0.7/qingqiu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-14 02:01:44.000000 qingqiu-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1394 2023-04-14 01:56:34.000000 qingqiu-0.0.7/setup.py
```

### Comparing `qingqiu-0.0.6/PKG-INFO` & `qingqiu-0.0.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: qingqiu
-Version: 0.0.6
+Version: 0.0.7
 Summary: 简单得接口测试框架
 Home-page: https://gitee.com/tuboyou/qingqiu
 Author: lixuecheng
 Author-email: lixuechengde@163.com
 License: MIT Licence
 Description: 简单得接口测试框架
 Keywords: pip,easy,requests,auto
```

### Comparing `qingqiu-0.0.6/qingqiu/__init__.py` & `qingqiu-0.0.7/qingqiu/__init__.py`

 * *Files identical despite different names*

### Comparing `qingqiu-0.0.6/qingqiu/check.py` & `qingqiu-0.0.7/qingqiu/check.py`

 * *Files identical despite different names*

### Comparing `qingqiu-0.0.6/qingqiu/conftest.py` & `qingqiu-0.0.7/qingqiu/conftest.py`

 * *Files identical despite different names*

### Comparing `qingqiu-0.0.6/qingqiu/handle.py` & `qingqiu-0.0.7/qingqiu/handle.py`

 * *Files identical despite different names*

### Comparing `qingqiu-0.0.6/qingqiu/help.py` & `qingqiu-0.0.7/qingqiu/help.py`

 * *Files identical despite different names*

### Comparing `qingqiu-0.0.6/qingqiu/qing.py` & `qingqiu-0.0.7/qingqiu/qing.py`

 * *Files identical despite different names*

### Comparing `qingqiu-0.0.6/qingqiu/qiu.py` & `qingqiu-0.0.7/qingqiu/qiu.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,15 +128,16 @@
         except Exception as e:
             if noException:
                 return False,str(e)
             else:
                 raise e
 
 
-    def checkResultJson(self, res: dict,noException=False):
+    def checkResultJson(self, resold: dict,noException=False):
+        res=resold.copy()
         try:
             if self.code == 0:
                 if isinstance(res, str):
                     try:
                         res = json.loads(res)
                     except Exception as e:
                         if not self.nolog:
@@ -276,20 +277,22 @@
                 except:
                     pass
                 raise Exception(kname+"结果校验错误:"+str(k)+"未在实际结果中")
                 
 
                     
 
-    def _handleCheckList(self, name: str, val: list, checkval: list):
+    def _handleCheckList(self, name: str, val: list, checkval1: list):
+        checkval=checkval1.copy()
         if len(checkval) > 0 :
             if checkval[0] == 'required':
                 if len(val) == 0:
                     raise Exception(name+"结果校验错误,长度为0")
                 del(checkval[0])
+            
             if checkval[0] == 'option' or checkval[0] == 'optional' or checkval[0] == 'null' or checkval[0] == 'none':
                 del(checkval[0])
             
         if len(checkval) == 1:
             index = 0
             for line in val:
                 kname = name+"[{}]".format(index)
```

### Comparing `qingqiu-0.0.6/qingqiu/tools.py` & `qingqiu-0.0.7/qingqiu/tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,14 @@
                 to=backup['lastTime']
         if timeFormat is not None and isinstance(timeFormat,str):
             to=datetime.datetime.fromisoformat(timeFormat.strip())
         if dayStart:
             to=to.replace(hour=0,minute=0,second=0,microsecond=0)
         if dayEnd:
             to=to.replace(hour=23,minute=59,second=59,microsecond=0)
-            # timeStamp = int(time.mktime(time.strptime(timeFormat.strip(), "%Y-%m-%d %H:%M:%S")))
         to=to+datetime.timedelta(days=days,minutes=minutes,hours=hours,seconds=seconds)
         backup['lastTime']=to
         timeStamp=to.timestamp()
         if ms:
             timeStamp = timeStamp*1000
         timeStamp=int(to.timestamp())
         if returnType == 'str':
```

### Comparing `qingqiu-0.0.6/qingqiu/transform.py` & `qingqiu-0.0.7/qingqiu/transform.py`

 * *Files identical despite different names*

### Comparing `qingqiu-0.0.6/qingqiu.egg-info/PKG-INFO` & `qingqiu-0.0.7/qingqiu.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: qingqiu
-Version: 0.0.6
+Version: 0.0.7
 Summary: 简单得接口测试框架
 Home-page: https://gitee.com/tuboyou/qingqiu
 Author: lixuecheng
 Author-email: lixuechengde@163.com
 License: MIT Licence
 Description: 简单得接口测试框架
 Keywords: pip,easy,requests,auto
```

### Comparing `qingqiu-0.0.6/setup.py` & `qingqiu-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from setuptools import setup, find_packages
 
 
 
 setup(
 name = "qingqiu",
-version = "0.0.6",
+version = "0.0.7",
 keywords = ["pip", "easy","requests","auto"],
 description = "简单得接口测试框架",
 long_description = "简单得接口测试框架",
 license = "MIT Licence",
 
 url = "https://gitee.com/tuboyou/qingqiu",
 author = "lixuecheng",
```

