# Comparing `tmp/codeframe-0.1.8.tar.gz` & `tmp/codeframe-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codeframe-0.1.8.tar", last modified: Wed Apr  6 12:33:16 2022, max compression
+gzip compressed data, was "codeframe-0.1.9.tar", last modified: Tue Jan 10 15:05:17 2023, max compression
```

## Comparing `codeframe-0.1.8.tar` & `codeframe-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2022-04-06 12:33:16.705714 codeframe-0.1.8/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     2744 2022-04-06 12:33:16.705714 codeframe-0.1.8/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1858 2022-04-06 12:33:09.000000 codeframe-0.1.8/README.md
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2022-04-06 12:33:16.705714 codeframe-0.1.8/bin/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    30027 2022-04-06 12:32:56.000000 codeframe-0.1.8/bin/codeframe
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2022-04-06 12:33:16.705714 codeframe-0.1.8/codeframe/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      251 2021-10-05 12:11:35.000000 codeframe-0.1.8/codeframe/__init__.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     6835 2021-10-05 12:13:21.000000 codeframe-0.1.8/codeframe/config.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2299 2021-10-05 12:11:35.000000 codeframe-0.1.8/codeframe/prj_utils.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2022-04-06 12:33:16.000000 codeframe-0.1.8/codeframe/version.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2022-04-06 12:33:16.705714 codeframe-0.1.8/codeframe.egg-info/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     2744 2022-04-06 12:33:16.000000 codeframe-0.1.8/codeframe.egg-info/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      282 2022-04-06 12:33:16.000000 codeframe-0.1.8/codeframe.egg-info/SOURCES.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2022-04-06 12:33:16.000000 codeframe-0.1.8/codeframe.egg-info/dependency_links.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        5 2022-04-06 12:33:16.000000 codeframe-0.1.8/codeframe.egg-info/requires.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       10 2022-04-06 12:33:16.000000 codeframe-0.1.8/codeframe.egg-info/top_level.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2022-04-06 12:33:16.705714 codeframe-0.1.8/setup.cfg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1198 2021-10-05 12:11:35.000000 codeframe-0.1.8/setup.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-01-10 15:05:17.837070 codeframe-0.1.9/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     2744 2023-01-10 15:05:17.837070 codeframe-0.1.9/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     1858 2023-01-10 15:05:15.000000 codeframe-0.1.9/README.md
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-01-10 15:05:17.833070 codeframe-0.1.9/bin/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    30022 2023-01-10 15:04:48.000000 codeframe-0.1.9/bin/codeframe
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-01-10 15:05:17.837070 codeframe-0.1.9/codeframe/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      251 2021-10-05 12:11:35.000000 codeframe-0.1.9/codeframe/__init__.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     6511 2022-05-11 14:51:32.000000 codeframe-0.1.9/codeframe/config.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2299 2021-10-05 12:11:35.000000 codeframe-0.1.9/codeframe/prj_utils.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2023-01-10 15:05:17.000000 codeframe-0.1.9/codeframe/version.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-01-10 15:05:17.837070 codeframe-0.1.9/codeframe.egg-info/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     2744 2023-01-10 15:05:17.000000 codeframe-0.1.9/codeframe.egg-info/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      282 2023-01-10 15:05:17.000000 codeframe-0.1.9/codeframe.egg-info/SOURCES.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-01-10 15:05:17.000000 codeframe-0.1.9/codeframe.egg-info/dependency_links.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        5 2023-01-10 15:05:17.000000 codeframe-0.1.9/codeframe.egg-info/requires.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       10 2023-01-10 15:05:17.000000 codeframe-0.1.9/codeframe.egg-info/top_level.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-01-10 15:05:17.837070 codeframe-0.1.9/setup.cfg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1198 2021-10-05 12:11:35.000000 codeframe-0.1.9/setup.py
```

### Comparing `codeframe-0.1.8/PKG-INFO` & `codeframe-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codeframe
-Version: 0.1.8
+Version: 0.1.9
 Summary: Creates a simple package structure, git, PyPI, bumpversion, pytest and configfile ready
 Home-page: http://gitlab.com/jaromrax/codeframe
 Author: jaromrax
 Author-email: jaromrax@gmail.com
 License: GPL2
 Description: Project codeframe
         =================
```

### Comparing `codeframe-0.1.8/README.md` & `codeframe-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `codeframe-0.1.8/bin/codeframe` & `codeframe-0.1.9/bin/codeframe`

 * *Files 0% similar despite different names*

```diff
@@ -637,15 +637,15 @@
 
 echo "D...  convert ORG to MARKDOWN automatically"
 if [ -e README.org ]; then
     pandoc README.org -o README.md
 fi
 
 echo diff bin_{proj}.py bin/{proj}
-diff bin_codeframe.py bin/codeframe
+diff  bin_{proj}.py bin/{proj}
 if [ "$?" != "0" ]; then
 
   echo X... difference bin and bin
   exit 1
 fi
 
 echo " - i will run"
```

### Comparing `codeframe-0.1.8/codeframe/config.py` & `codeframe-0.1.9/codeframe/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,33 +2,15 @@
 from codeframe.version import __version__
 from fire import Fire
 
 import json
 import os
 import sys
 # ----- port here. 5000 is flask; is moved to 8000 by gunicorn; to 80 by nginx
-CONFIG={'x':640,
-        'y':480 ,
-        'interpolation':'None',
-        'mintime':0.1,       # normal picture rate
-        'videodev':0,
-        'filename':'~/.config/test/cfg.json',
-        'user':'aaa',
-        'password':'aaa',
-        'port':5000,
-        'change':None,
-        'autoiris':True,
-        'riris':1000,
-        'pantilt':False,
-        'pan':0,
-        'tilt':0,
-        'gamma_adjust':False,
-        'rgain':0,
-        'use_v4l':True,      # zdenek84 had a problem with. I try again
-        'quit':False         # this is howto quit
+CONFIG={"test":True
 }
 
 #CFG_DEBUG = True
 #CFG_DEBUG = False
 
 
 #===========================================================
@@ -47,15 +29,15 @@
         if os.path.isfile( os.path.expanduser(cfg)):
             with open(os.path.expanduser(cfg), "r") as f:
                 dicti = json.load(f)
         ok = True
         #if CFG_DEBUG:print("D... config verified")
     except:
         #if CFG_DEBUG:
-        print("D... verification config FAILED")
+        print("X... verification config FAILED")
     return ok
 
 def get_config_file():
     ''' returns the filename where config is stored'''
     global CONFIG
     return CONFIG['filename']
 
@@ -81,15 +63,15 @@
     else:
         cfg = filenamebk
 
     cfgbak = cfg + ".bak"
     #print("D... cfg:",cfg)
     #print("D... cfgbak:",cfgbak)
     #if CFG_DEBUG:
-    print("D... creating a backup config:", cfgbak )
+    #print("D... creating a backup config:", cfgbak )
     if not os.path.isfile( os.path.expanduser(cfg)):
         print(f"X... config {cfg} doesnt exist (yet?, OK)")
         return True
 
     ### rozXXXX
     try:
         os.rename(os.path.expanduser(cfg),
@@ -110,38 +92,38 @@
     if filenamebk=="":
         cfg = CONFIG['filename']
     else:
         cfg = filenamebk
 
     cfgbak = cfg + ".bak"
     #if CFG_DEBUG:
-    print("D... testing if backup config exists:", cfgbak)
+    #print("D... testing if backup config exists:", cfgbak)
     if os.path.isfile( os.path.expanduser(cfgbak)):
         #if CFG_DEBUG:
-        print("D... BACUP config exists:",cfgbak, "... renaming to:", cfg)
+        #print("D... BACUP config exists:",cfgbak, "... renaming to:", cfg)
         os.rename(os.path.expanduser(cfgbak),
                   os.path.expanduser(cfg))
         #if CFG_DEBUG:print("D... config is recovered from:", cfgbak)
-    else:
+    #else:
         #if CFG_DEBUG:
-        print("D... bak config did not exist:", cfgbak,"no bak file recovery")
+        #print("D... bak config did not exist:", cfgbak,"no bak file recovery")
 
 
 def save_config(filenamesv="", filename = ""): # duplicit... filename overrides
     '''FRONT function, save config to filename'''
     global CONFIG
     if filename != "":
         CONFIG['filename'] = filename
 
     if filenamesv=="":
         cfg = CONFIG['filename']
     else:
         cfg = filenamesv
 
-    print("D... calling cfg_to_bak:", cfg)
+    #print("D... calling cfg_to_bak:", cfg)
     if not cfg_to_bak(cfg):
         sys.exit(1)
 
     print("D... writing config:", cfg)
 
     ### rozxxx
     dir2create = os.path.dirname( cfg )
@@ -155,68 +137,75 @@
         f.write(json.dumps(CONFIG, indent=1))
         #if CFG_DEBUG:print("D... config was written:", cfg)
 
     if verify_config(filename):
         #if CFG_DEBUG:
         print("D... verified by verify_config ... ok ... ending here")
         return True
+    else:
+        print("D... verified by verify_config ... NOT ok ... ending here")
+        return False
     #====ELSE RECOVER BAK
     return bak_to_cfg()
 
 
 
 def load_config(filename=""):
     '''FRONT function, load config file'''
     global CONFIG
+    config_present=False
     if filename != "":
         CONFIG['filename'] = filename
     cfg = CONFIG['filename']
     cfg = cfg+".from_memory"
     #if CFG_DEBUG:
-    print("D... calling save_config:")
+    #print("D... calling save_config:")
     save_config( cfg )
 
     cfg = CONFIG['filename']
     #if CFG_DEBUG:print("D... loading config from",cfg)
 
     if not verify_config(filename):
         print("X... FAILED on verifications")
         return False
 
     #if CFG_DEBUG:
-    print("D... passed verification of:",cfg)
+    #print("D... passed verification of:",cfg)
     dicti = CONFIG
 
     #if CFG_DEBUG:
-    print("D... directly loading json:",cfg)
+    #print("D... directly loading json:",cfg)
     if os.path.isfile( os.path.expanduser(cfg)):
         with open(os.path.expanduser(cfg), "r") as f:
             dicti = json.load(f)
+        config_present = True
 
     # rewriting in memory
     if sorted(dicti.keys()) == sorted(CONFIG.keys()):
         #if CFG_DEBUG:
-        print("D... memory and disk identical:")
+        pass
+        #print("D... memory and disk identical:")
     else:
         #if CFG_DEBUG:
         print("X... memory and disk differ:")
         # show_config(CONFIG)
         # there may be more lines in the CODE after upgrade.
         for k in CONFIG.keys(): # search CODE version
             if not (k in dicti.keys()):
                 print("D... key not on DISK:", k )
                 dicti[k] = CONFIG[k]
 
 
     CONFIG = dicti
     #if CFG_DEBUG:
-    print("D... final CONFIG:")
+    #print("D... final CONFIG:")
     #show_config(filename)
     #if CFG_DEBUG:
-    print("D... end load")
+    #print("D... end load")
+    return config_present
 
 
 def loadsave(filename = ""):
     '''FRONT function, if DISK is earlier version than CODE, this may update DISK'''
     if filename != "":
         CONFIG['filename'] = filename
```

### Comparing `codeframe-0.1.8/codeframe/prj_utils.py` & `codeframe-0.1.9/codeframe/prj_utils.py`

 * *Files identical despite different names*

### Comparing `codeframe-0.1.8/codeframe.egg-info/PKG-INFO` & `codeframe-0.1.9/codeframe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codeframe
-Version: 0.1.8
+Version: 0.1.9
 Summary: Creates a simple package structure, git, PyPI, bumpversion, pytest and configfile ready
 Home-page: http://gitlab.com/jaromrax/codeframe
 Author: jaromrax
 Author-email: jaromrax@gmail.com
 License: GPL2
 Description: Project codeframe
         =================
```

### Comparing `codeframe-0.1.8/setup.py` & `codeframe-0.1.9/setup.py`

 * *Files identical despite different names*

