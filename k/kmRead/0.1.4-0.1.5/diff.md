# Comparing `tmp/kmRead-0.1.4.tar.gz` & `tmp/kmRead-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kmRead-0.1.4.tar", last modified: Fri Aug 26 08:40:59 2022, max speed, from FAT filesystem (MS-DOS, OS/2, NT)
+gzip compressed data, was "dist\kmRead-0.1.5.tar", last modified: Fri Apr 14 12:14:44 2023, max compression
```

## Comparing `kmRead-0.1.4.tar` & `kmRead-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2022-08-26 08:39:56.000000 kmRead-0.1.4/
--rw-rw-rw-   0        0        0      321 2022-08-26 08:39:56.000000 kmRead-0.1.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-08-26 08:39:56.000000 kmRead-0.1.4/kmRead/
--rw-rw-rw-   0        0        0        0 2021-08-23 12:53:33.000000 kmRead-0.1.4/kmRead/__init__.py
--rwxrwxrwx   0        0        0     7602 2022-08-26 08:40:56.000000 kmRead-0.1.4/kmRead/kmRead.py
-drwxrwxrwx   0        0        0        0 2022-08-26 08:39:56.000000 kmRead-0.1.4/kmRead.egg-info/
--rw-rw-rw-   0        0        0      321 2022-08-26 08:39:56.000000 kmRead-0.1.4/kmRead.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2022-08-26 08:39:56.000000 kmRead-0.1.4/kmRead.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-26 08:39:56.000000 kmRead-0.1.4/kmRead.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       98 2022-08-26 08:39:56.000000 kmRead-0.1.4/kmRead.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2022-08-26 08:39:56.000000 kmRead-0.1.4/kmRead.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-08-26 08:39:56.000000 kmRead-0.1.4/kmRead.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-08-26 08:39:56.000000 kmRead-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      936 2022-08-26 08:39:45.000000 kmRead-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 12:14:44.000000 kmRead-0.1.5/
+-rw-rw-rw-   0        0        0      337 2023-04-14 12:14:44.000000 kmRead-0.1.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-14 12:14:44.000000 kmRead-0.1.5/kmRead/
+-rw-rw-rw-   0        0        0        0 2021-08-23 12:53:33.000000 kmRead-0.1.5/kmRead/__init__.py
+-rw-rw-rw-   0        0        0     9424 2023-04-14 07:45:40.000000 kmRead-0.1.5/kmRead/kmRead.py
+drwxrwxrwx   0        0        0        0 2023-04-14 12:14:44.000000 kmRead-0.1.5/kmRead.egg-info/
+-rw-rw-rw-   0        0        0      337 2023-04-14 12:14:43.000000 kmRead-0.1.5/kmRead.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2023-04-14 12:14:44.000000 kmRead-0.1.5/kmRead.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 12:14:43.000000 kmRead-0.1.5/kmRead.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       98 2023-04-14 12:14:43.000000 kmRead-0.1.5/kmRead.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-04-14 12:14:44.000000 kmRead-0.1.5/kmRead.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-14 12:14:44.000000 kmRead-0.1.5/kmRead.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-14 12:14:44.000000 kmRead-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      952 2023-04-14 12:14:03.000000 kmRead-0.1.5/setup.py
```

### Comparing `kmRead-0.1.4/kmRead/kmRead.py` & `kmRead-0.1.5/kmRead/kmRead.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from openpyxl import Workbook,styles
 import zipfile
 
 
 def un_zxm(file_name):
     """unzip zip file"""
     zip_file = zipfile.ZipFile(file_name)
-    data=zip_file.read('content.json').decode()
-    data=json.loads(data, encoding='utf8')
+    data=zip_file.read('content.json')
+    data=json.loads(data)
     zip_file.close()
     return data
 
 def write_csv_file(path, head, data):
     '''
     用途：把list数据写入csv文件中
     path 文件地址
@@ -75,18 +75,17 @@
         for vdata in csvList:
             if vdata in tmpDict:
                 tmpList.append(tmpDict.get(vdata))
             else:
                 tmpList.append("")
         datas.append(tmpList.copy())
     if(isCSV):
-        write_csv_file(fileName.replace('.km', '.csv').replace('.zxm','.csv'), csvList, datas)
+        write_csv_file(fileName.replace('.xmind', '.csv').replace('.km', '.csv').replace('.zxm','.csv'), csvList, datas)
     else:
-        write_excel_file(fileName.replace('.km', '.xlsx').replace('.zxm','.xlsx'), csvList, datas)
-
+        write_excel_file(fileName.replace('.xmind', '.xlsx').replace('.km', '.xlsx').replace('.zxm','.xlsx'), csvList, datas)
 
 def getDataFromKM(root, data, nowList):
     '''
     用途：使用嵌套循环获取km文件内容并生产list数据
     root 文件目录
     data 获取单层内容
     nowList 当前已获取的数据
@@ -95,14 +94,28 @@
     if len(data['children']) > 0:  # 判断是否含有子目录
         for childrenData in data['children']:
             getDataFromKM(root+','+tmpData, childrenData, nowList)
     else:
         nowList.append({root: tmpData})
     return nowList
 
+def getDataFromXmind(root, data, nowList):
+    '''
+    用途：使用嵌套循环获取km文件内容并生产list数据
+    root 文件目录
+    data 获取单层内容
+    nowList 当前已获取的数据
+    '''
+    tmpData = str(data['title']).strip()  # 临时数据报保存当前值
+    if 'children' in data and len(data['children']['attached']) > 0:  # 判断是否含有子目录
+        for childrenData in data['children']['attached']:
+            getDataFromXmind(root+','+tmpData, childrenData, nowList)
+    else:
+        nowList.append({root: tmpData})
+    return nowList
 
 def getFile(path):
     '''
     用途：获取文件并转成dict格式
     path 文件路径
     '''
     if not os.path.exists(path):
@@ -125,25 +138,29 @@
     if len(data['children']) > 0:  # 判断是否含有子目录
         for childrenData in data['children']:
             getDataFromKM(root+','+tmpData, childrenData, nowList)
     else:
         nowList.append({root: tmpData})
     return nowList
 
+
+
 def run(filepath, xuid, pid,isCSV=True):
     '''
     用途：执行脚本
     filepath km文件的绝对路径
     xuid 需求id 
     pid p账号
     '''
     if str(filepath).endswith('.km'):
         fileLine = getDataFromKM('', getFile(filepath)['root'], [])
     elif str(filepath).endswith('.zxm'):
         fileLine = getDataFromZXM('', un_zxm(filepath)['root'], [])
+    elif str(filepath).endswith('.xmind'):
+        fileLine = getDataFromXmind('', un_zxm(filepath)[0]['rootTopic'], [])
     else:
         raise Exception("文件格式错误")
     caseDict = {}
     for line in fileLine:
         for k, v in line.items():
             if caseDict.get(k) is None:
                 caseDict[k]=v
@@ -155,15 +172,15 @@
     f=""
     if (len(sys.argv)==1):
         f=input("请填写文件地址：")
         sys.argv.append(f)
     x=""
     if  (len(sys.argv)==2):
         filename=str(sys.argv[1]).strip('"').strip("'")
-        if not filename.endswith('.km') and  not filename.endswith('.zxm'):
+        if not filename.endswith('.km') and  not filename.endswith('.zxm') and  not filename.endswith('.xmind'):
             print("指定文件不正确，是检查路径是否存在空格，&等特殊字符，如果存在，请在头尾添加双引号！\n")
             sys.exit(1)
         x=input("请填写需求id：")
         sys.argv.append(x)
     p=""
     if  (len(sys.argv)==3):
         pv=""
@@ -207,17 +224,44 @@
 
    
 def mainInit():
     print('''reg add "HKEY_CLASSES_ROOT\SystemFileAssociations\.km\shell\km2Excel\command" /f /d "\\\"{}kme.exe\\\" \\\"%1\\\""'''.format(sys.argv[0][:-3]))
     os.system('''reg add "HKEY_CLASSES_ROOT\SystemFileAssociations\.km\shell\km2Excel\command" /f /d "\\\"{}kme.exe\\\" \\\"%1\\\""'''.format(sys.argv[0][:-3]))
     os.system('''reg add "HKEY_CLASSES_ROOT\SystemFileAssociations\.zxm\shell\zxm2Excel\command" /f /d "\\\"{}kme.exe\\\" \\\"%1\\\""'''.format(sys.argv[0][:-3]))
 
+    # pv=""
+    # p=""
+    # if os.environ.get('HOME') is not None:
+    #     pv=os.path.join(os.environ.get('HOME'),".km")
+    # elif os.environ.get('HOMEPATH') is not None:
+    #     pv=os.path.join(os.environ.get('HOMEPATH'),".km")
+    # if len(pv)>0:
+    #     if os.path.exists(pv):
+    #         for i in os.listdir(pv):
+    #             if i.startswith('pzhanghaofile.'):
+    #                 p=i[14:]
+    #                 break
+    # if len(p)==0:
+    #     p=input("请填写p账号：")
+    #     try:
+    #         os.makedirs(pv)
+    #         with open(os.path.join(pv,'pzhanghaofile.'+p),"w") as f1:
+    #             f1.write("\n")
+    #     except:
+    #         pass
+# maine()
+# def un_zip(file_name):
+#     """unzip zip file"""
+#     zip_file = zipfile.ZipFile(file_name)
+#     data=zip_file.read('content.json').decode()
+#     data=json.loads(data)
+#     zip_file.close()
+#     return data
 
-
-
+# un_zip(r'C:\Users\Administrator\Envs\test1\test\腾讯视频增加畅读卡落地页.zxm')
```

### Comparing `kmRead-0.1.4/setup.py` & `kmRead-0.1.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 
 from setuptools import setup, find_packages
 
 
 
 setup(
 name = "kmRead",
-version = "0.1.4",
+version = "0.1.5",
 keywords = ["pip", "km","mind","csv"],
-description = "把km和zxm文件转换成表格文件",
-long_description = "把km和zxm文件转换成表格文件",
+description = "把km、zxm和xmind文件转换成表格文件",
+long_description = "把km、zxm和xmind文件转换成表格文件",
 license = "MIT Licence",
 
 url = "https://gitee.com/tuboyou/km-read",
 author = "lixuecheng",
 author_email = "lixuechengde@163.com",
 packages = find_packages(),
 include_package_data = True,
```

