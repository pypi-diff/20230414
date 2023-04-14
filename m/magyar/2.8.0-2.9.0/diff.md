# Comparing `tmp/magyar-2.8.0.tar.gz` & `tmp/magyar-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magyar-2.8.0.tar", last modified: Fri Apr 14 16:37:19 2023, max compression
+gzip compressed data, was "magyar-2.9.0.tar", last modified: Fri Apr 14 20:33:37 2023, max compression
```

## Comparing `magyar-2.8.0.tar` & `magyar-2.9.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-04-14 16:37:19.105306 magyar-2.8.0/
--rw-rw-r--   0 bela      (1000) bela      (1000)     1535 2023-04-14 16:37:19.105306 magyar-2.8.0/PKG-INFO
--rw-rw-r--   0 bela      (1000) bela      (1000)     1164 2023-04-13 19:21:03.000000 magyar-2.8.0/README.md
-drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-04-14 16:37:19.105306 magyar-2.8.0/magyar.egg-info/
--rw-rw-r--   0 bela      (1000) bela      (1000)     1535 2023-04-14 16:37:19.000000 magyar-2.8.0/magyar.egg-info/PKG-INFO
--rw-rw-r--   0 bela      (1000) bela      (1000)      148 2023-04-14 16:37:19.000000 magyar-2.8.0/magyar.egg-info/SOURCES.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)        1 2023-04-14 16:37:19.000000 magyar-2.8.0/magyar.egg-info/dependency_links.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)        7 2023-04-14 16:37:19.000000 magyar-2.8.0/magyar.egg-info/top_level.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)     9057 2023-04-13 19:56:03.000000 magyar-2.8.0/magyar.py
--rw-rw-r--   0 bela      (1000) bela      (1000)       38 2023-04-14 16:37:19.105306 magyar-2.8.0/setup.cfg
--rw-rw-r--   0 bela      (1000) bela      (1000)      588 2023-04-14 16:35:12.000000 magyar-2.8.0/setup.py
+drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-04-14 20:33:37.108044 magyar-2.9.0/
+-rw-rw-r--   0 bela      (1000) bela      (1000)     1798 2023-04-14 20:33:37.108044 magyar-2.9.0/PKG-INFO
+-rw-rw-r--   0 bela      (1000) bela      (1000)     1427 2023-04-14 20:32:03.000000 magyar-2.9.0/README.md
+drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-04-14 20:33:37.108044 magyar-2.9.0/magyar.egg-info/
+-rw-rw-r--   0 bela      (1000) bela      (1000)     1798 2023-04-14 20:33:37.000000 magyar-2.9.0/magyar.egg-info/PKG-INFO
+-rw-rw-r--   0 bela      (1000) bela      (1000)      148 2023-04-14 20:33:37.000000 magyar-2.9.0/magyar.egg-info/SOURCES.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)        1 2023-04-14 20:33:37.000000 magyar-2.9.0/magyar.egg-info/dependency_links.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)        7 2023-04-14 20:33:37.000000 magyar-2.9.0/magyar.egg-info/top_level.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)    10941 2023-04-14 20:21:52.000000 magyar-2.9.0/magyar.py
+-rw-rw-r--   0 bela      (1000) bela      (1000)       38 2023-04-14 20:33:37.108044 magyar-2.9.0/setup.cfg
+-rw-rw-r--   0 bela      (1000) bela      (1000)      588 2023-04-14 20:33:32.000000 magyar-2.9.0/setup.py
```

### Comparing `magyar-2.8.0/PKG-INFO` & `magyar-2.9.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magyar
-Version: 2.8.0
+Version: 2.9.0
 Summary: Hungarian names...
 Home-page: https://github.com/kobanya/nevek
 Author: Nagy Béla
 Author-email: nagy.belabudapest@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -24,32 +24,46 @@
 4. utcanevek = magyar.utca
 5. telelpülésnevek= magyar.telepules
 6. vármegyék nevei = magyar.megye
 7. folyók nevei = magyar.folyo
 8. a hét napjai = magyar.nap
 9. az év hónapjai = magyar.honap
 
+Szótárak  (dictionary): 
+1. Királyok és uralkodásuk ideje  = magyar.kiraly
+
 ## Description
 1. last names =  magyar.vezeteknev
 2. female first names = magyar.keresztnev_n
 3. male first names  = magyar.keresztnev_f
 4. street names = magyar.utca
 5. city names = magyar.telepules
 6. names of counties = magyar.megye
 7. names of rivers = magyar.folyo
 8. he days of the week = magyar.nap
 9. the months of the year = magyar.honap
-## Használat:
 
- Főként véletlengenerátorok kiegészítőjeként ajánlom
+Dictionary:
+1. Hungarian Kings and Reigns = magyar.kiraly
+
+## Listák használat:
+
+ Főként véletlengenerátorok kiegészítőjeként ajánlom a listákat
  
 I recommend it mainly as a supplement to random number generators. 
        
              random.choice
-telepulesek = random.choices(magyar.telepules, k=25)
+telepulesek = random.choice(magyar.telepules)
+
+## Szótárak:
+Több adatot tartalmaznak.
+
+magyar.kiraly tartalma :
+
+kiraly = {'király neve' : (tól, ig)}
 
 
 ## Szerző
 
 * Név: Nagy BÉLa
 * E-mail:nagy.bela.budapest@gmail.com
```

### Comparing `magyar-2.8.0/README.md` & `magyar-2.9.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -12,32 +12,46 @@
 4. utcanevek = magyar.utca
 5. telelpülésnevek= magyar.telepules
 6. vármegyék nevei = magyar.megye
 7. folyók nevei = magyar.folyo
 8. a hét napjai = magyar.nap
 9. az év hónapjai = magyar.honap
 
+Szótárak  (dictionary): 
+1. Királyok és uralkodásuk ideje  = magyar.kiraly
+
 ## Description
 1. last names =  magyar.vezeteknev
 2. female first names = magyar.keresztnev_n
 3. male first names  = magyar.keresztnev_f
 4. street names = magyar.utca
 5. city names = magyar.telepules
 6. names of counties = magyar.megye
 7. names of rivers = magyar.folyo
 8. he days of the week = magyar.nap
 9. the months of the year = magyar.honap
-## Használat:
 
- Főként véletlengenerátorok kiegészítőjeként ajánlom
+Dictionary:
+1. Hungarian Kings and Reigns = magyar.kiraly
+
+## Listák használat:
+
+ Főként véletlengenerátorok kiegészítőjeként ajánlom a listákat
  
 I recommend it mainly as a supplement to random number generators. 
        
              random.choice
-telepulesek = random.choices(magyar.telepules, k=25)
+telepulesek = random.choice(magyar.telepules)
+
+## Szótárak:
+Több adatot tartalmaznak.
+
+magyar.kiraly tartalma :
+
+kiraly = {'király neve' : (tól, ig)}
 
 
 ## Szerző
 
 * Név: Nagy BÉLa
 * E-mail:nagy.bela.budapest@gmail.com
```

### Comparing `magyar-2.8.0/magyar.egg-info/PKG-INFO` & `magyar-2.9.0/magyar.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magyar
-Version: 2.8.0
+Version: 2.9.0
 Summary: Hungarian names...
 Home-page: https://github.com/kobanya/nevek
 Author: Nagy Béla
 Author-email: nagy.belabudapest@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -24,32 +24,46 @@
 4. utcanevek = magyar.utca
 5. telelpülésnevek= magyar.telepules
 6. vármegyék nevei = magyar.megye
 7. folyók nevei = magyar.folyo
 8. a hét napjai = magyar.nap
 9. az év hónapjai = magyar.honap
 
+Szótárak  (dictionary): 
+1. Királyok és uralkodásuk ideje  = magyar.kiraly
+
 ## Description
 1. last names =  magyar.vezeteknev
 2. female first names = magyar.keresztnev_n
 3. male first names  = magyar.keresztnev_f
 4. street names = magyar.utca
 5. city names = magyar.telepules
 6. names of counties = magyar.megye
 7. names of rivers = magyar.folyo
 8. he days of the week = magyar.nap
 9. the months of the year = magyar.honap
-## Használat:
 
- Főként véletlengenerátorok kiegészítőjeként ajánlom
+Dictionary:
+1. Hungarian Kings and Reigns = magyar.kiraly
+
+## Listák használat:
+
+ Főként véletlengenerátorok kiegészítőjeként ajánlom a listákat
  
 I recommend it mainly as a supplement to random number generators. 
        
              random.choice
-telepulesek = random.choices(magyar.telepules, k=25)
+telepulesek = random.choice(magyar.telepules)
+
+## Szótárak:
+Több adatot tartalmaznak.
+
+magyar.kiraly tartalma :
+
+kiraly = {'király neve' : (tól, ig)}
 
 
 ## Szerző
 
 * Név: Nagy BÉLa
 * E-mail:nagy.bela.budapest@gmail.com
```

### Comparing `magyar-2.8.0/setup.py` & `magyar-2.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="magyar",
-    version="2.8.0",
+    version="2.9.0",
     author="Nagy Béla",
     author_email="nagy.belabudapest@gmail.com",
     description="Hungarian names...",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kobanya/nevek",
     py_modules=["magyar"],
```

