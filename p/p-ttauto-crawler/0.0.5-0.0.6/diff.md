# Comparing `tmp/p-ttauto-crawler-0.0.5.tar.gz` & `tmp/p-ttauto-crawler-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p-ttauto-crawler-0.0.5.tar", last modified: Thu Apr 13 11:27:26 2023, max compression
+gzip compressed data, was "p-ttauto-crawler-0.0.6.tar", last modified: Fri Apr 14 06:00:47 2023, max compression
```

## Comparing `p-ttauto-crawler-0.0.5.tar` & `p-ttauto-crawler-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 11:27:26.457567 p-ttauto-crawler-0.0.5/
--rw-rw-rw-   0        0        0     1074 2023-02-27 11:23:20.000000 p-ttauto-crawler-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      397 2023-04-13 11:27:26.457567 p-ttauto-crawler-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       14 2023-04-11 08:07:03.000000 p-ttauto-crawler-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 11:27:26.453566 p-ttauto-crawler-0.0.5/p_ttauto_crawler.egg-info/
--rw-rw-rw-   0        0        0      397 2023-04-13 11:27:26.000000 p-ttauto-crawler-0.0.5/p_ttauto_crawler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      373 2023-04-13 11:27:26.000000 p-ttauto-crawler-0.0.5/p_ttauto_crawler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 11:27:26.000000 p-ttauto-crawler-0.0.5/p_ttauto_crawler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-04-13 11:27:26.000000 p-ttauto-crawler-0.0.5/p_ttauto_crawler.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       63 2023-04-13 11:27:26.000000 p-ttauto-crawler-0.0.5/p_ttauto_crawler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-13 11:27:26.000000 p-ttauto-crawler-0.0.5/p_ttauto_crawler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 11:27:26.458566 p-ttauto-crawler-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      938 2023-04-13 11:27:21.000000 p-ttauto-crawler-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 11:27:26.455568 p-ttauto-crawler-0.0.5/ttauto_crawler/
--rw-rw-rw-   0        0        0        0 2023-04-07 05:52:07.000000 p-ttauto-crawler-0.0.5/ttauto_crawler/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 11:27:26.456567 p-ttauto-crawler-0.0.5/ttauto_crawler/bin/
--rw-rw-rw-   0        0        0        0 2023-04-07 05:52:07.000000 p-ttauto-crawler-0.0.5/ttauto_crawler/bin/__init__.py
--rw-rw-rw-   0        0        0    13940 2023-04-13 11:27:13.000000 p-ttauto-crawler-0.0.5/ttauto_crawler/main.py
--rw-rw-rw-   0        0        0     8894 2023-04-13 11:08:16.000000 p-ttauto-crawler-0.0.5/ttauto_crawler/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-14 06:00:47.953769 p-ttauto-crawler-0.0.6/
+-rw-rw-rw-   0        0        0     1074 2023-02-27 11:23:20.000000 p-ttauto-crawler-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      397 2023-04-14 06:00:47.952770 p-ttauto-crawler-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2023-04-11 08:07:03.000000 p-ttauto-crawler-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 06:00:47.934771 p-ttauto-crawler-0.0.6/p_ttauto_crawler.egg-info/
+-rw-rw-rw-   0        0        0      397 2023-04-14 06:00:47.000000 p-ttauto-crawler-0.0.6/p_ttauto_crawler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      373 2023-04-14 06:00:47.000000 p-ttauto-crawler-0.0.6/p_ttauto_crawler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 06:00:47.000000 p-ttauto-crawler-0.0.6/p_ttauto_crawler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-04-14 06:00:47.000000 p-ttauto-crawler-0.0.6/p_ttauto_crawler.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       63 2023-04-14 06:00:47.000000 p-ttauto-crawler-0.0.6/p_ttauto_crawler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-14 06:00:47.000000 p-ttauto-crawler-0.0.6/p_ttauto_crawler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-14 06:00:47.953769 p-ttauto-crawler-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      938 2023-04-14 05:46:59.000000 p-ttauto-crawler-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 06:00:47.949771 p-ttauto-crawler-0.0.6/ttauto_crawler/
+-rw-rw-rw-   0        0        0        0 2023-04-07 05:52:07.000000 p-ttauto-crawler-0.0.6/ttauto_crawler/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 06:00:47.951770 p-ttauto-crawler-0.0.6/ttauto_crawler/bin/
+-rw-rw-rw-   0        0        0        0 2023-04-07 05:52:07.000000 p-ttauto-crawler-0.0.6/ttauto_crawler/bin/__init__.py
+-rw-rw-rw-   0        0        0    16089 2023-04-14 05:46:50.000000 p-ttauto-crawler-0.0.6/ttauto_crawler/main.py
+-rw-rw-rw-   0        0        0    10719 2023-04-14 06:00:31.000000 p-ttauto-crawler-0.0.6/ttauto_crawler/utils.py
```

### Comparing `p-ttauto-crawler-0.0.5/LICENSE` & `p-ttauto-crawler-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `p-ttauto-crawler-0.0.5/setup.py` & `p-ttauto-crawler-0.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="p-ttauto-crawler",
-    version="0.0.5",
+    version="0.0.6",
     author="pengjun",
     author_email="mr_lonely@foxmail.com",
     description="template tools",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `p-ttauto-crawler-0.0.5/ttauto_crawler/main.py` & `p-ttauto-crawler-0.0.6/ttauto_crawler/main.py`

 * *Files 15% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 def clearDir():
     s = os.path.join(rootDir, ".download")
     if os.path.exists(s):
         shutil.rmtree(s)
     s1 = os.path.join(rootDir, ".out")
     if os.path.exists(s1):
-        shutil.rmtree(s)
+        shutil.rmtree(s1)
 
 def curDownloadDir():
     s = os.path.join(rootDir, ".download", str(curGroupId))
     if os.path.exists(s) == False:
         os.makedirs(s)
     return s
 
@@ -48,16 +48,20 @@
             "id": curGroupId,
             "video_path": ossurl,
             "video_num": count
         }
         s = requests.session()
         s.headers.update({'Connection':'close'})
         res = s.post(f"https://beta.2tianxin.com/common/admin/tta/get_set_task_complete", json.dumps(param), verify=False)
-        resContext = res.content.decode(encoding="utf8", errors="ignore")
-        logging.info(f"notifyMessage res:{resContext}")
+        if res.status_code == 200:
+            logging.info(f"notifyMessage success")
+        else:
+            resContext = res.content.decode(encoding="utf8", errors="ignore")
+            logging.info(f"notifyMessage fail! code={res.status_code}, context={resContext}")
+            print("report error!")
         s.close()
     except Exception as e:
         logging.info(f"notifyMessage exception :{e}")
 
 def processAllVideo(crawler_template_name):
     src = curDownloadDir()
     dst = curOutputDir()
@@ -240,23 +244,23 @@
             zip1.write(filepath, writepath)
     zip1.close()
     shutil.copyfile(dist1, f"d://{curGroupId}_out.zip")
     os.remove(dist1)
 
 def process(url, crawler_template_name):
     global successCount
-    ### downlaod
-    print(f"=== downloading ")
-    aaaapp(True, url, "", 0)
-    ### process
-    print(f"=== processing ")
-    processAllVideo(crawler_template_name)
-    cacheDir() #cache file to d://
-    ### upload
-    print(f"=== uploading ")
+    # ### downlaod
+    # print(f"=== downloading ")
+    # aaaapp(True, url, "", 0)
+    # ### process
+    # print(f"=== processing ")
+    # processAllVideo(crawler_template_name)
+    # cacheDir() #cache file to d://
+    # ### upload
+    # print(f"=== uploading ")
     dist = os.path.join(os.path.dirname(curOutputDir()), f"{curGroupId}.zip")
     zip = zipfile.ZipFile(dist, "w", zipfile.ZIP_DEFLATED) 
     for rt,dirs,files in os.walk(curOutputDir()):
         for file in files:
             if str(file).startswith("~$"):
                 continue
             filepath = os.path.join(rt, file)
@@ -314,37 +318,56 @@
                 print(f"complate => {curGroupId} rst={successCount}/{allCount} duration={(current_pts - start_pts)}")
                 logging.info(f"================ end {curGroupId} rst={successCount}/{allCount} duration={(current_pts - start_pts)}===================")
         except Exception as e:
             notifyMessage(False, str(e))
             logging.error("====================== uncatch Exception ======================")
             logging.error(e)
             logging.error("======================      end      ======================")
-        time.sleep(10)
+        time.sleep(2)
     os.remove(os.path.join(thisFileDir, "stop.now"))
     print(f"stoped !")
         
 if __name__ == '__main__':
         main()
  
   
+
 # urllib3.disable_warnings()
 # d = datetime.datetime.now().strftime('%Y_%m_%d_%H_%M_%S')
 # thisFileDir = os.path.dirname(os.path.abspath(__file__))
 # logging.basicConfig(filename=f"{thisFileDir}/ttauto_crawler_{d}.log", 
 #                     format='%(asctime)s %(filename)s [line:%(lineno)d] %(levelname)s %(message)s',
 #                     datefmt='%a, %d %b %Y %H:%M:%S',
 #                     encoding="utf-8",
 #                     level=logging.DEBUG)
 # rootDir = thisFileDir
-       
-# curGroupId = 650
-# allCount = 0
-# successCount = 0
-# start_pts = calendar.timegm(time.gmtime())
-# logging.info(f"================ begin {curGroupId} ===================")
-# print(f"=== begin {curGroupId}")
-# url = "https://www.tiktok.com/@773ao3ama"
-# crawler_template_name = "template8"
-# process(url, crawler_template_name)
-# current_pts = calendar.timegm(time.gmtime())
-# print(f"complate => {curGroupId} rst={successCount}/{allCount} duration={(current_pts - start_pts)}")
-# logging.info(f"================ end {curGroupId} ===================")
+
+# data = {
+#     "655": "https://www.douyin.com/user/MS4wLjABAAAA8HZMhOtYrVWIrJpatn8qDerHqJwU9lq0auwzKB_WGu0?is_search=0&list_name=follow&nt=1",
+#     "656": "https://www.douyin.com/user/MS4wLjABAAAADYVRgncl5JXnmSrJ-W5sUkESnKmo_Jk8JYS2tMFcclQ?is_search=0&list_name=follow&nt=6",
+#     "657": "https://www.douyin.com/user/MS4wLjABAAAAiuzGYPakHGpmrnTN3keMBHjdmVjNa4nymsZyZ1-YeRg?enter_from=personal_homepage&enter_method=follow_list&is_search=0&list_name=follow&nt=3&tab_name=follow_lish",
+#     "658": "https://www.douyin.com/user/MS4wLjABAAAAOGMf-61v-fMT08Rm74xyww7yvt6e3sWdCKXCRWN0kyk?is_search=0&list_name=follow&nt=2",
+#     "659": "https://www.douyin.com/user/MS4wLjABAAAAJoPPHri240u2Qu3bslnYYoPMUWEFIRttmPor12iWVTg?is_search=0&list_name=follow&nt=5",
+#     "660": "https://www.douyin.com/user/MS4wLjABAAAAf3zlyh2TNQqN9IvNVhVL66dvwTI6dLMlp9WzAzrzaV9wxb9xspiNaVo-hsV3kpVS?is_search=0&list_name=follow&nt=6",
+#     "661": "https://www.douyin.com/user/MS4wLjABAAAAAF_Tk5hGJMRGreCk8Yc4H-AMB8by1J_uYJJICwVeW5g?is_search=0&list_name=follow&nt=8",
+#     "662": "https://www.douyin.com/user/MS4wLjABAAAA44R40ALq6aA4bRmOB63nmtY5qgStRh8KiJI32LcRntRzzTOknkw3QbbPXPCfAkf2?is_search=0&list_name=follow&nt=0",
+#     "663": "https://www.douyin.com/user/MS4wLjABAAAApGFo2iYnfSnQzJZ0WxesCM4RJrRuw6wOxgPEJIID5Ms?is_search=0&list_name=follow&nt=0",
+#     "664": "https://www.douyin.com/user/MS4wLjABAAAA347ySfj3QLAogzxDrYKdNj5ef5xEwCUObHpqf7JcxK8?is_search=0&list_name=follow&nt=1",
+#     "665": "https://www.douyin.com/user/MS4wLjABAAAAZ-1VxguZ7ukGEdERr2TCbclyaQUGdpsMqUggpuXrx4c?is_search=0&list_name=follow&nt=0",
+#     "666": "https://www.douyin.com/user/MS4wLjABAAAA8ye7i8MvmMhfF7h8whsdAZL3EezBICN9-7t0-6vWQlo?is_search=0&list_name=follow&nt=0",
+#     "667": "https://www.douyin.com/user/MS4wLjABAAAAWOj7rND1K1-nuizauPdmrs0lR0Hi97OanrRc7e1R0uo5_qaRytpbHXYRO1eOEYVP?is_search=0&list_name=follow&nt=3",
+# }
+
+# for k in data:
+#     curGroupId = int(k)
+#     allCount = 0
+#     successCount = 0
+#     start_pts = calendar.timegm(time.gmtime())
+#     logging.info(f"================ begin {curGroupId} ===================")
+#     print(f"=== begin {curGroupId}")
+#     url = data[k]
+#     crawler_template_name = "template8"
+#     process(url, crawler_template_name)
+#     current_pts = calendar.timegm(time.gmtime())
+#     print(f"complate => {curGroupId} rst={successCount}/{allCount} duration={(current_pts - start_pts)}")
+#     logging.info(f"================ end {curGroupId} ===================")
+
```

### Comparing `p-ttauto-crawler-0.0.5/ttauto_crawler/utils.py` & `p-ttauto-crawler-0.0.6/ttauto_crawler/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -180,15 +180,63 @@
 def getLocalImageSize(p):
     try:
         image = Image.open(BytesIO(p), "r")
         return image.size
     except:
         return 0, 0
 
-def deepFtpUpload(file, ftp, remote_dir=''):
+def deepFtpUpload50(file, ftp, remote_dir=''):
+    append_dir = f'{remote_dir}'
+    if len(remote_dir) > 0:
+        remote_path = f'video/{append_dir}/'
+        try:
+            ftp.cwd(remote_path)
+        except ftplib.error_perm as e:
+            if e.args[0].startswith('550'):
+                # 如果远程目录不存在，则创建它
+                ftp.mkd(remote_path)
+                ftp.cwd(remote_path)
+
+    s = []
+    if os.path.isfile(file):
+        with open(file, 'rb') as f:
+            ftp.storbinary(f'STOR {os.path.basename(file)}', f)
+        s.append(f"ftp://192.168.50.113/video/{append_dir}{os.path.basename(file)}")
+    elif os.path.isdir(file):
+        for filename in os.listdir(file):
+            local_file = os.path.join(file, filename)
+            if os.path.isfile(local_file):
+                with open(local_file, 'rb', encoding='UTF-8') as file:
+                    ftp.storbinary(f'STOR {filename}', file)
+                s.append(f"ftp://192.168.50.113/video/{append_dir}{filename}")
+            elif os.path.isdir(local_file):
+                subdir = os.path.join(remote_dir, filename)
+                s.append(ftpUpload50(local_file, ftp, subdir))
+    return s
+
+def ftpUpload50(file, ftp = None):
+    if not ftp:
+        ftp = ftplib.FTP('192.168.50.113')
+        ftp.login('ftpuser', 'ftpuser')
+
+    remote_path = f'video/'
+    try:
+        ftp.cwd(remote_path)
+    except ftplib.error_perm as e:
+        if e.args[0].startswith('550'):
+            # 如果远程目录不存在，则创建它
+            ftp.mkd(remote_path)
+            ftp.cwd(remote_path)
+
+    s = deepFtpUpload50(file, ftp, "")
+    ftp.quit()
+    return s
+
+
+def deepFtpUpload3(file, ftp, remote_dir=''):
     append_dir = f'{remote_dir}'
     if len(remote_dir) > 0:
         remote_path = f'1TB01/data/video/{append_dir}/'
         try:
             ftp.cwd(remote_path)
         except ftplib.error_perm as e:
             if e.args[0].startswith('550'):
@@ -206,27 +254,33 @@
             local_file = os.path.join(file, filename)
             if os.path.isfile(local_file):
                 with open(local_file, 'rb', encoding='UTF-8') as file:
                     ftp.storbinary(f'STOR {filename}', file)
                 s.append(f"http://192.168.3.220/01/video/{append_dir}{filename}")
             elif os.path.isdir(local_file):
                 subdir = os.path.join(remote_dir, filename)
-                s.append(ftpUpload(local_file, ftp, subdir))
+                s.append(ftpUpload3(local_file, ftp, subdir))
     return s
 
-def ftpUpload(file, ftp = None):
+def ftpUpload3(file, ftp = None):
     if not ftp:
         ftp = ftplib.FTP('192.168.3.220')
         ftp.login('xinyu100', 'xinyu100.com')
 
     remote_path = f'1TB01/data/video/'
     try:
         ftp.cwd(remote_path)
     except ftplib.error_perm as e:
         if e.args[0].startswith('550'):
             # 如果远程目录不存在，则创建它
             ftp.mkd(remote_path)
             ftp.cwd(remote_path)
 
-    s = deepFtpUpload(file, ftp, "")
+    s = deepFtpUpload3(file, ftp, "")
     ftp.quit()
-    return s
+    return s
+
+def ftpUpload(file):
+    try:
+        ftpUpload50(file)
+    except:
+        ftpUpload3(file)
```

