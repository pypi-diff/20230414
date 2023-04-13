# Comparing `tmp/yunxiao-0.1.5.tar.gz` & `tmp/yunxiao-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yunxiao-0.1.5.tar", last modified: Tue Apr 11 18:10:19 2023, max compression
+gzip compressed data, was "yunxiao-0.1.6.tar", last modified: Thu Apr 13 23:00:48 2023, max compression
```

## Comparing `yunxiao-0.1.5.tar` & `yunxiao-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 18:10:19.122410 yunxiao-0.1.5/
--rw-rw-rw-   0        0        0    35821 2023-04-09 12:33:49.000000 yunxiao-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     7017 2023-04-11 18:10:19.121409 yunxiao-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     6530 2023-04-10 01:07:24.000000 yunxiao-0.1.5/README.md
--rw-rw-rw-   0        0        0      587 2023-04-11 18:09:56.000000 yunxiao-0.1.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-11 18:10:19.122410 yunxiao-0.1.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-11 18:10:19.109887 yunxiao-0.1.5/yunxiao/
--rw-rw-rw-   0        0        0       66 2023-04-09 13:09:35.000000 yunxiao-0.1.5/yunxiao/__init__.py
--rw-rw-rw-   0        0        0    18394 2023-04-10 14:56:31.000000 yunxiao-0.1.5/yunxiao/app.py
--rw-rw-rw-   0        0        0     8916 2023-04-11 18:09:17.000000 yunxiao-0.1.5/yunxiao/web.py
--rw-rw-rw-   0        0        0     6516 2023-04-08 20:37:39.000000 yunxiao-0.1.5/yunxiao/yunxiao.py
-drwxrwxrwx   0        0        0        0 2023-04-11 18:10:19.120408 yunxiao-0.1.5/yunxiao.egg-info/
--rw-rw-rw-   0        0        0     7017 2023-04-11 18:10:18.000000 yunxiao-0.1.5/yunxiao.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2023-04-11 18:10:18.000000 yunxiao-0.1.5/yunxiao.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 18:10:18.000000 yunxiao-0.1.5/yunxiao.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-04-11 18:10:18.000000 yunxiao-0.1.5/yunxiao.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-11 18:10:18.000000 yunxiao-0.1.5/yunxiao.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-13 23:00:48.056815 yunxiao-0.1.6/
+-rw-rw-rw-   0        0        0    35821 2023-04-09 12:33:49.000000 yunxiao-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     7017 2023-04-13 23:00:48.047303 yunxiao-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     6530 2023-04-10 01:07:24.000000 yunxiao-0.1.6/README.md
+-rw-rw-rw-   0        0        0      587 2023-04-13 23:00:36.000000 yunxiao-0.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-13 23:00:48.056815 yunxiao-0.1.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-13 23:00:48.040295 yunxiao-0.1.6/yunxiao/
+-rw-rw-rw-   0        0        0       66 2023-04-09 13:09:35.000000 yunxiao-0.1.6/yunxiao/__init__.py
+-rw-rw-rw-   0        0        0    18394 2023-04-10 14:56:31.000000 yunxiao-0.1.6/yunxiao/app.py
+-rw-rw-rw-   0        0        0     8934 2023-04-13 22:59:48.000000 yunxiao-0.1.6/yunxiao/web.py
+-rw-rw-rw-   0        0        0     6516 2023-04-08 20:37:39.000000 yunxiao-0.1.6/yunxiao/yunxiao.py
+drwxrwxrwx   0        0        0        0 2023-04-13 23:00:48.045301 yunxiao-0.1.6/yunxiao.egg-info/
+-rw-rw-rw-   0        0        0     7017 2023-04-13 23:00:48.000000 yunxiao-0.1.6/yunxiao.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2023-04-13 23:00:48.000000 yunxiao-0.1.6/yunxiao.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 23:00:48.000000 yunxiao-0.1.6/yunxiao.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-04-13 23:00:48.000000 yunxiao-0.1.6/yunxiao.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-13 23:00:48.000000 yunxiao-0.1.6/yunxiao.egg-info/top_level.txt
```

### Comparing `yunxiao-0.1.5/LICENSE` & `yunxiao-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `yunxiao-0.1.5/PKG-INFO` & `yunxiao-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yunxiao
-Version: 0.1.5
+Version: 0.1.6
 Summary: An API tool for Cloud School Education Institution Management System.
 Author-email: YiZixuan <admin@sqkkyzx.com>
 License: GPL-3.0-only
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `yunxiao-0.1.5/README.md` & `yunxiao-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `yunxiao-0.1.5/pyproject.toml` & `yunxiao-0.1.6/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "yunxiao"
-version = "0.1.5"
+version = "0.1.6"
 description = "An API tool for Cloud School Education Institution Management System."
 readme = "README.md"
 authors = [
     {name = "YiZixuan", email = "admin@sqkkyzx.com"},
 ]
 license.text = "GPL-3.0-only"
 classifiers = [
```

### Comparing `yunxiao-0.1.5/yunxiao/app.py` & `yunxiao-0.1.6/yunxiao/app.py`

 * *Files identical despite different names*

### Comparing `yunxiao-0.1.5/yunxiao/web.py` & `yunxiao-0.1.6/yunxiao/web.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from .yunxiao import WebOAuth, UsedTime
 
 
 class Web(WebOAuth):
-    def __init__(self, userphone: str, password: str, campus: list =None):
+    def __init__(self, userphone: str, password: str, campus: list = None):
         super().__init__(userphone, password)
         if campus is None:
             self.campus = []
         else:
             self.campus = campus
         self.reportpath = "https://yunxiao.xiaogj.com/api/cs-pc-report/cs-report/reports/"
         self.edupath = "https://yunxiao.xiaogj.com/api/cs-pc-edu/"
@@ -165,23 +165,23 @@
             }
         ).json()
 
     def find_payment_list(
             self,
             pay_start_date: str = UsedTime.weekstrat,
             pay_end_date: str = UsedTime.weekend,
-            order_status: int = 1,
+            order_status: int = "",
             page_num: int = 1,
             page_size: int = 9999
     ):
         """
         收入明细报表。
         :param pay_start_date: 支付起始时间
         :param pay_end_date: 支付结束时间
-        :param order_status: 订单状态 1>已付款
+        :param order_status: 订单状态 1>已付款 4>已作废
         :param page_num: 页数
         :param page_size: 每页项目数
         :return:
         """
         return self.session.post(
             url=self.reportpath + "findPaymentList",
             json={
@@ -259,10 +259,11 @@
                 "paymentGroupId": payment_group_id
             }
         )
 
 
 if __name__ == "__main__":
     import sys
+
     web = Web(sys.argv[1], sys.argv[2])
     res = web.receipt(5744750, 5744752)
-    print(res.content.decode("utf-8"))
+    print(res.content.decode("utf-8"))
```

### Comparing `yunxiao-0.1.5/yunxiao/yunxiao.py` & `yunxiao-0.1.6/yunxiao/yunxiao.py`

 * *Files identical despite different names*

### Comparing `yunxiao-0.1.5/yunxiao.egg-info/PKG-INFO` & `yunxiao-0.1.6/yunxiao.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yunxiao
-Version: 0.1.5
+Version: 0.1.6
 Summary: An API tool for Cloud School Education Institution Management System.
 Author-email: YiZixuan <admin@sqkkyzx.com>
 License: GPL-3.0-only
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.11
```

