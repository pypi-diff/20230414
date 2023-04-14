# Comparing `tmp/osais-1.0.35.tar.gz` & `tmp/osais-1.0.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Websites\opensourceais\python\lib_osais\dist\.tmp-or1g8c_1\osais-1.0.35.tar", last modified: Thu Apr 13 21:41:48 2023, max compression
+gzip compressed data, was "D:\Websites\opensourceais\python\lib_osais\dist\.tmp-n6xscl2h\osais-1.0.36.tar", last modified: Fri Apr 14 09:43:00 2023, max compression
```

## Comparing `osais-1.0.35.tar` & `osais-1.0.36.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 21:41:48.894348 osais-1.0.35/
--rw-rw-rw-   0        0        0    33041 2023-04-05 11:19:20.000000 osais-1.0.35/LICENSE
--rw-rw-rw-   0        0        0     1113 2023-04-13 21:41:48.894348 osais-1.0.35/PKG-INFO
--rw-rw-rw-   0        0        0      339 2023-04-05 15:00:45.000000 osais-1.0.35/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 21:41:48.890349 osais-1.0.35/osais/
--rw-rw-rw-   0        0        0      652 2023-04-13 21:41:22.000000 osais-1.0.35/osais/__init__.py
--rw-rw-rw-   0        0        0    41405 2023-04-13 21:41:15.000000 osais-1.0.35/osais/osais.py
-drwxrwxrwx   0        0        0        0 2023-04-13 21:41:48.893350 osais-1.0.35/osais.egg-info/
--rw-rw-rw-   0        0        0     1113 2023-04-13 21:41:48.000000 osais-1.0.35/osais.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2023-04-13 21:41:48.000000 osais-1.0.35/osais.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 21:41:48.000000 osais-1.0.35/osais.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-04-13 21:41:48.000000 osais-1.0.35/osais.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-13 21:41:48.000000 osais-1.0.35/osais.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       95 2023-04-05 18:53:17.000000 osais-1.0.35/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-13 21:41:48.894348 osais-1.0.35/setup.cfg
--rw-rw-rw-   0        0        0     1124 2023-04-13 21:41:28.000000 osais-1.0.35/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 09:43:00.929769 osais-1.0.36/
+-rw-rw-rw-   0        0        0    33041 2023-04-05 11:19:20.000000 osais-1.0.36/LICENSE
+-rw-rw-rw-   0        0        0     1113 2023-04-14 09:43:00.928772 osais-1.0.36/PKG-INFO
+-rw-rw-rw-   0        0        0      339 2023-04-05 15:00:45.000000 osais-1.0.36/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 09:43:00.923769 osais-1.0.36/osais/
+-rw-rw-rw-   0        0        0      652 2023-04-14 09:42:35.000000 osais-1.0.36/osais/__init__.py
+-rw-rw-rw-   0        0        0    41525 2023-04-14 09:42:13.000000 osais-1.0.36/osais/osais.py
+drwxrwxrwx   0        0        0        0 2023-04-14 09:43:00.927770 osais-1.0.36/osais.egg-info/
+-rw-rw-rw-   0        0        0     1113 2023-04-14 09:43:00.000000 osais-1.0.36/osais.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2023-04-14 09:43:00.000000 osais-1.0.36/osais.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 09:43:00.000000 osais-1.0.36/osais.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-04-14 09:43:00.000000 osais-1.0.36/osais.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-14 09:43:00.000000 osais-1.0.36/osais.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       95 2023-04-05 18:53:17.000000 osais-1.0.36/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-14 09:43:00.929769 osais-1.0.36/setup.cfg
+-rw-rw-rw-   0        0        0     1124 2023-04-14 09:42:41.000000 osais-1.0.36/setup.py
```

### Comparing `osais-1.0.35/LICENSE` & `osais-1.0.36/LICENSE`

 * *Files identical despite different names*

### Comparing `osais-1.0.35/PKG-INFO` & `osais-1.0.36/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osais
-Version: 1.0.35
+Version: 1.0.36
 Summary: The osais Python lib for connecting AIs to OSAIS cloud
 Home-page: https://github.com/incubiq/osais
 Author: incubiq
 Author-email: eric@incubiq.com
 Keywords: osais,opensourceais
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `osais-1.0.35/osais/__init__.py` & `osais-1.0.36/osais/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 A package for OSAIS virtual AI.
 """
-__version__="1.0.35"
+__version__="1.0.36"
 __author__ = "incubiq"
 __email__ = "eric@incubiq.com"
 
 from .osais import osais_isLocal
 from .osais import osais_loadConfig
 from .osais import osais_getEnv
 from .osais import osais_getHarwareInfo
```

### Comparing `osais-1.0.35/osais/osais.py` & `osais-1.0.36/osais/osais.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-__version__="1.0.35"
+__version__="1.0.36"
 
 ## ========================================================================
 ## 
 ##                      Utilities starts here 
 ## 
 ## ========================================================================
 
@@ -97,14 +97,23 @@
         if modification_time < cutoff_time:
             os.remove(file_path)
             
 ## ------------------------------------------------------------------------
 #       System utils
 ## ------------------------------------------------------------------------
 
+def consoleLog(err): 
+    msg=""
+    if hasattr(err, 'msg'):
+        msg=err.msg
+    else:
+        if err.args and err.args[0]:
+            msg=err.args[0]                      
+    print("CRITICAL: "+msg)
+
 ## get a meaningful name for our machine
 def get_machine_name() :
     _machine=str (hex(uuid.getnode()))
     _isDocker=is_running_in_docker()
     if _isDocker:
         _machine = os.environ.get('HOSTNAME') or os.popen('hostname').read().strip()
     return _machine
@@ -636,26 +645,26 @@
     try:
         response = requests.post(f"{gOriginGateway}api/v1/public/ai/config", headers=headers, data=json.dumps(objParam))
         objRes=response.json()["data"]
         if objRes is None:
             raise ValueError("CRITICAL: could not notify Gateway")
 
     except Exception as err:
-        print("CRITICAL: "+err.msg)
+        consoleLog(err)
         raise err
     return True
 
 ## PUBLIC - Reset connection to local gateway
 def osais_resetGateway(_localGateway):
     global gOriginGateway
     gOriginGateway=_localGateway
     try:
         _notifyGateway()
     except Exception as err:
-        print("CRITICAL: "+err.msg)
+        consoleLog(err)
         raise err
     
     print("=> This AI is reset to talk to Gateway "+_localGateway)
     return True
 
 ## ------------------------------------------------------------------------
 #       authenticate into OSAIS as virtual AI
@@ -687,30 +696,30 @@
                 print("COULD NOT REGISTER, stopping it here")
                 sys.exit()
 
             gToken=objRes["token"]
             gSecret=objRes["secret"]
             print("We are REGISTERED with OSAIS Prod")
         except Exception as err:
-            print("CRITICAL: "+err.msg)
+            consoleLog(err)
             raise err
 
     ## reg with Local OSAIS (debug)
     else:
         try:
             response = requests.post(f"{gOriginLocalOSAIS}api/v1/public/virtualai/register", headers=headers, data=json.dumps(objParam))
             objRes=response.json()["data"]
             if objRes is None:
                 print("COULD NOT REGISTER with debug")
 
             gTokenLocal=objRes["token"]
             gSecretLocal=objRes["secret"]
             print("We are REGISTERED with OSAIS Local (debug)")
         except Exception as err:
-            print("CRITICAL: "+err.msg)
+            consoleLog(err)
             raise err
 
     return True
 
 # Authenticate into OSAIS
 def _loginVAI():
     global gToken
@@ -734,15 +743,15 @@
             objRes=response.json()["data"]
             if objRes is None:
                 print("COULD NOT LOGIN, stopping it here")
                 sys.exit()
             print("We got an authentication token into OSAIS")
             gAuthToken=objRes["authToken"]    
         except Exception as err:
-            print("CRITICAL: "+err.msg)
+            consoleLog(err)
             raise err
 
     if gTokenLocal!= None:
         try:
             response = requests.post(f"{gOriginLocalOSAIS}api/v1/public/virtualai/login", headers=headers, data=json.dumps({
                 "token": gTokenLocal,
                 "secret": gSecretLocal
@@ -768,15 +777,15 @@
     Resp={"data": None}
     if gIsVirtualAI:
 
         try:
             resp= _registerVAI()
             resp=_loginVAI()
         except Exception as err:
-            print("CRITICAL: "+err.msg)
+            consoleLog(err)
             raise err
         
         # Run the scheduler
         if gIsScheduled==False:
             gIsScheduled=True
             schedule.every().day.at("10:30").do(_loginVAI)
 
@@ -848,15 +857,15 @@
                 aArgForparserAI.append("-filename")
                 aArgForparserAI.append(_input)
             else:
                 ## min requirements
                 print("no image to process")
                 return "input required"
         except Exception as err:
-            print("CRITICAL: "+err.msg)
+            consoleLog(err)
             raise err
     
     ## Init OSAIS Params (from all args, keep only those for OSAIS)
     aArgForParserOSAIS=_getArgs(_args)
     args_ExclusiveOSAIS.append('-odir')
     args_ExclusiveOSAIS.append('-idir')
     aArgForParserOSAIS=_argsFromFilter(aArgForParserOSAIS, args_ExclusiveOSAIS, True)
@@ -892,15 +901,15 @@
             response=fn_run(aArgForparserAI)
         else:
             if len(args)==3:
                 response=fn_run(aArgForparserAI, args[2])
             else:
                 response=fn_run(aArgForparserAI, args[2], args[3])
     except Exception as err:
-        print("CRITICAL: "+err.msg)
+        consoleLog(err)
         raise err
 
     ## calculate cost
     gIsBusy=False
     end_date = datetime.utcnow()
     delta=end_date - beg_date
     cost = int(delta.total_seconds()* 1000 + delta.microseconds / 1000)
```

### Comparing `osais-1.0.35/osais.egg-info/PKG-INFO` & `osais-1.0.36/osais.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osais
-Version: 1.0.35
+Version: 1.0.36
 Summary: The osais Python lib for connecting AIs to OSAIS cloud
 Home-page: https://github.com/incubiq/osais
 Author: incubiq
 Author-email: eric@incubiq.com
 Keywords: osais,opensourceais
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `osais-1.0.35/setup.py` & `osais-1.0.36/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='osais',
-    version='1.0.35',
+    version='1.0.36',
     author='incubiq',
     author_email='eric@incubiq.com',
     description='The osais Python lib for connecting AIs to OSAIS cloud',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/incubiq/osais',
     keywords = "osais, opensourceais",
```

