# Comparing `tmp/analysisbykwok-0.0.18.tar.gz` & `tmp/analysisbykwok-0.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "analysisbykwok-0.0.18.tar", last modified: Wed Apr 12 07:13:46 2023, max compression
+gzip compressed data, was "analysisbykwok-0.0.19.tar", last modified: Fri Apr 14 05:21:27 2023, max compression
```

## Comparing `analysisbykwok-0.0.18.tar` & `analysisbykwok-0.0.19.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 07:13:46.959298 analysisbykwok-0.0.18/
--rw-rw-rw-   0        0        0       62 2023-04-12 07:13:46.958302 analysisbykwok-0.0.18/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-12 07:13:46.954314 analysisbykwok-0.0.18/analysisbykwok/
--rw-rw-rw-   0        0        0    15997 2023-04-12 07:13:27.000000 analysisbykwok-0.0.18/analysisbykwok/__init__.py
--rw-rw-rw-   0        0        0       23 2023-04-12 07:13:05.000000 analysisbykwok-0.0.18/analysisbykwok/_version.py
-drwxrwxrwx   0        0        0        0 2023-04-12 07:13:46.958302 analysisbykwok-0.0.18/analysisbykwok.egg-info/
--rw-rw-rw-   0        0        0       62 2023-04-12 07:13:46.000000 analysisbykwok-0.0.18/analysisbykwok.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2023-04-12 07:13:46.000000 analysisbykwok-0.0.18/analysisbykwok.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 07:13:46.000000 analysisbykwok-0.0.18/analysisbykwok.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-12 07:13:46.000000 analysisbykwok-0.0.18/analysisbykwok.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       70 2023-04-12 07:13:13.000000 analysisbykwok-0.0.18/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-12 07:13:46.959298 analysisbykwok-0.0.18/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-14 05:21:27.125430 analysisbykwok-0.0.19/
+-rw-rw-rw-   0        0        0       62 2023-04-14 05:21:27.125430 analysisbykwok-0.0.19/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-14 05:21:27.121441 analysisbykwok-0.0.19/analysisbykwok/
+-rw-rw-rw-   0        0        0    16655 2023-04-14 05:21:04.000000 analysisbykwok-0.0.19/analysisbykwok/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-04-14 05:20:39.000000 analysisbykwok-0.0.19/analysisbykwok/_version.py
+drwxrwxrwx   0        0        0        0 2023-04-14 05:21:27.124433 analysisbykwok-0.0.19/analysisbykwok.egg-info/
+-rw-rw-rw-   0        0        0       62 2023-04-14 05:21:27.000000 analysisbykwok-0.0.19/analysisbykwok.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      220 2023-04-14 05:21:27.000000 analysisbykwok-0.0.19/analysisbykwok.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 05:21:27.000000 analysisbykwok-0.0.19/analysisbykwok.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-14 05:21:27.000000 analysisbykwok-0.0.19/analysisbykwok.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       70 2023-04-14 05:20:46.000000 analysisbykwok-0.0.19/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-14 05:21:27.125430 analysisbykwok-0.0.19/setup.cfg
```

### Comparing `analysisbykwok-0.0.18/analysisbykwok/__init__.py` & `analysisbykwok-0.0.19/analysisbykwok/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -333,8 +333,25 @@
         a =function.GetPlateSon(PlateInfoName)
         print('正在下载' + str(PlateInfoName) + '板块的股票信息')
         for i in range(0, len(a['代码'])):
             code = FindCode(a['代码'][i])
             for son in code:
                 data = pro.daily(ts_code=son)
                 data.to_csv(r'{}\{}-{}.csv'.format(url, a['名称'][i], a['代码'][i]))
-                function.ProgressBar(i, len(a['代码']), a['名称'][i])
+                function.ProgressBar(i, len(a['代码']), a['名称'][i])
+    def MergeTable(data1, data2, on, data1name, data2name):
+        data1 = pd.merge(data1, data2, on=on, how='outer')
+        for i in range(0, len(list(data1))):
+            data1 = data1.rename(
+                columns={list(data1)[i]: list(data1)[i].replace('_x', data1name).replace('_y', data2name)})
+        return data1
+    def ChoiceColumn(date,name):
+        date1=date.copy()
+        if len(name)==0:
+            print(list(date))
+        else:
+            for i in range(0,len(list(date))):
+                if list(date)[i] in name:
+                    pass
+                else:
+                    del(date1[list(date)[i]])
+        return date1
```

