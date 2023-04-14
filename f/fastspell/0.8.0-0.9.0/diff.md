# Comparing `tmp/fastspell-0.8.0.tar.gz` & `tmp/fastspell-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/work/jzaragoza/hardrules/fastspell/dist/.tmp-34uhfod8/fastspell-0.8.0.tar", last modified: Thu Mar  9 15:51:15 2023, max compression
+gzip compressed data, was "fastspell-0.9.0.tar", last modified: Fri Apr 14 15:42:06 2023, max compression
```

## Comparing `fastspell-0.8.0.tar` & `fastspell-0.9.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxrwxr-x   0 jzaragoza  (1002) jzaragoza  (1002)        0 2023-03-09 15:51:15.641460 fastspell-0.8.0/
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)    10032 2023-03-09 15:51:15.641460 fastspell-0.8.0/PKG-INFO
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     8748 2023-03-09 15:14:12.000000 fastspell-0.8.0/README.md
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     1708 2023-03-09 15:48:14.000000 fastspell-0.8.0/pyproject.toml
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)       38 2023-03-09 15:51:15.641460 fastspell-0.8.0/setup.cfg
-drwxrwxr-x   0 jzaragoza  (1002) jzaragoza  (1002)        0 2023-03-09 15:51:15.641460 fastspell-0.8.0/src/
-drwxrwxr-x   0 jzaragoza  (1002) jzaragoza  (1002)        0 2023-03-09 15:51:15.641460 fastspell-0.8.0/src/fastspell/
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      141 2023-03-06 15:04:09.000000 fastspell-0.8.0/src/fastspell/__init__.py
-drwxrwxr-x   0 jzaragoza  (1002) jzaragoza  (1002)        0 2023-03-09 15:51:15.641460 fastspell-0.8.0/src/fastspell/config/
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      578 2023-03-09 15:43:47.000000 fastspell-0.8.0/src/fastspell/config/hunspell.yaml
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      514 2023-03-09 15:43:06.000000 fastspell-0.8.0/src/fastspell/config/similar.yaml
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)    12875 2023-03-09 14:51:17.000000 fastspell-0.8.0/src/fastspell/fastspell.py
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     4250 2023-03-09 15:01:59.000000 fastspell-0.8.0/src/fastspell/fastspell_download.py
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)     4329 2023-03-06 16:51:08.000000 fastspell-0.8.0/src/fastspell/util.py
-drwxrwxr-x   0 jzaragoza  (1002) jzaragoza  (1002)        0 2023-03-09 15:51:15.641460 fastspell-0.8.0/src/fastspell.egg-info/
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)    10032 2023-03-09 15:51:15.000000 fastspell-0.8.0/src/fastspell.egg-info/PKG-INFO
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      428 2023-03-09 15:51:15.000000 fastspell-0.8.0/src/fastspell.egg-info/SOURCES.txt
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)        1 2023-03-09 15:51:15.000000 fastspell-0.8.0/src/fastspell.egg-info/dependency_links.txt
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)      110 2023-03-09 15:51:15.000000 fastspell-0.8.0/src/fastspell.egg-info/entry_points.txt
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)       75 2023-03-09 15:51:15.000000 fastspell-0.8.0/src/fastspell.egg-info/requires.txt
--rw-rw-r--   0 jzaragoza  (1002) jzaragoza  (1002)       10 2023-03-09 15:51:15.000000 fastspell-0.8.0/src/fastspell.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:42:06.664455 fastspell-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-04-14 15:42:06.664455 fastspell-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-04-14 15:41:56.000000 fastspell-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-04-14 15:41:56.000000 fastspell-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 15:42:06.664455 fastspell-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:42:06.660455 fastspell-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:42:06.664455 fastspell-0.9.0/src/fastspell/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-14 15:41:56.000000 fastspell-0.9.0/src/fastspell/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:42:06.664455 fastspell-0.9.0/src/fastspell/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-14 15:41:56.000000 fastspell-0.9.0/src/fastspell/config/hunspell.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-14 15:41:56.000000 fastspell-0.9.0/src/fastspell/config/similar.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    12844 2023-04-14 15:41:56.000000 fastspell-0.9.0/src/fastspell/fastspell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-04-14 15:41:56.000000 fastspell-0.9.0/src/fastspell/fastspell_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-04-14 15:41:56.000000 fastspell-0.9.0/src/fastspell/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:42:06.664455 fastspell-0.9.0/src/fastspell.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-04-14 15:42:06.000000 fastspell-0.9.0/src/fastspell.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-14 15:42:06.000000 fastspell-0.9.0/src/fastspell.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 15:42:06.000000 fastspell-0.9.0/src/fastspell.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-14 15:42:06.000000 fastspell-0.9.0/src/fastspell.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-14 15:42:06.000000 fastspell-0.9.0/src/fastspell.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-14 15:42:06.000000 fastspell-0.9.0/src/fastspell.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:42:06.664455 fastspell-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-14 15:41:56.000000 fastspell-0.9.0/tests/test_fastspell.py
```

### Comparing `fastspell-0.8.0/PKG-INFO` & `fastspell-0.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastspell
-Version: 0.8.0
+Version: 0.9.0
 Summary: Targetted language identifier, based on FastText and Hunspell.
 Author-email: Prompsit Language Engineering <info@prompsit.com>
 Maintainer-email: Marta Bañon <mbanon@prompsit.com>, Jaume Zaragoza <jzaragoza@prompsit.com>
 Project-URL: Homepage, https://github.com/mbanon/fastspell
 Project-URL: FastSpell on GitHub, https://github.com/mbanon/fastspell
 Project-URL: Prompsit Language Engineering, http://www.prompsit.com
 Project-URL: Paracrawl, https://paracrawl.eu/
@@ -41,45 +41,47 @@
 ```
 pip install fastspell
 ```
 or directly from source:
 ```
 pip install .
 ```
-Note that **Hunspell** requires `python-dev` and `libhunspell-dev`:
+Note that it requires Python3.8 or higher, and the `python3-dev` package:
 
 ```
-sudo apt-get install python-dev libhunspell-dev
+sudo apt-get install python3-dev
 ```
 
+**IMPORTANT**:
+In some cases (for example, when using Python 3.10), the `cyhunspell` version 2.0.2 installation will fail. If that's the case, you need to install `cyhunspell==2.0.3` before installing `fastspell`:
+```
+pip install git+https://github.com/MSeal/cython_hunspell@2.0.3
+```
+
+### Model download
+
 To trigger the FastText model download before running fastspell, run:
 ```
 fastspell-download
 ```
-
 Since version 0.7 all the dictionaries are installed automatically with pip and there is no need to do anything else.
 For further explanation about how configuration works, [see below](#configuration).
 
 ### Conda
 Also, you can install the conda package:
 ```
 conda install -c conda-forge -c bitextor fastspell
 ```
 
-### RedHat installation
-For RedHat and its derivatives
+### Automatic testing
+Some automatic tests are provided to check that the installation went fine. In order to check it, go to the `/tests` directory and run:
 ```
-sudo dnf install hunspell hunspell-devel
-```
-must be ran to install Hunspell.
-
-If you found an installation error during `pip install hunspell` that says `/usr/bin/ld: cannot find -lhunspell`, you'll probably need to add a symlink to `/usr/lib64` or other path in your environment (like `/home/user/.local/lib`).
-```
-sudo ln -s /usr/lib64/libhunspell-1.7.so /usr/lib64/libhunspell.so
+python3 -m unittest discover
 ```
+You might need to istall the `unittest` package with `pip`, in  case you don't have it installed beforehand.
 
 ## Configuration
 
 A few configuration files are provided under the `fastspell/config` directory.
 If you need to change default configuration, you can provide the path to your config directory with `-c`/`--config` or with the environment variable `FASTSPELL_CONFIG`.
 
 #### similar.yaml
@@ -154,14 +156,15 @@
   -q, --quiet        Silent logging mode (default: False)
   --debug            Debug logging mode (default: False)
   --logfile LOGFILE  Store log to a file (default: <_io.TextIOWrapper
                      name='<stderr>' mode='w' encoding='UTF-8'>)
   -v, --version      show version of this script and exit
 ```
 
+
 ## Aggressive vs Conservative
 
 FastSpell comes in two flavours: Aggressive and Conservative.
 
 The **Aggressive** mode is less hesitant to tag a sentence with the target language, and never has doubts. The **Conservative** version, on the other hand, is more reluctant to tag a sentence with the target language and will use the `unk`(unknown) tag in case of doubt (when there is a tie between the target language and other language, for example)
 
 ## Benchmark 
@@ -182,16 +185,16 @@
 Saltar á navegación Navegación INICIO
 Julio Freire, competidor da FGA, invitado polo Kennel club de Inglaterra, para participar nos Crufts 2014 (Birmingham, 6 - 9 de marzo).
 25 de xullo - Truong Tan Sang toma posesión como presidente de Vietnam
 Quen pode solicitar o dito financiamento?
 ```
 Command:
 ```
-fastspell $L --aggr inputtext
-fastspell $L --cons inputtext
+fastspell  --aggr lang inputtext
+fastspell  --cons lang inputtext
 ```
 Aggressive output:
 ```
 19-01-2011 47 comentarios 7o Xornadas de Xardinería de Galicia (RE)PLANTEAR     gl
 • Proceso de valoración de idoneidade: entrevistas psicosociais e visita domiciliaria e aplicación de test psicolóxicos, se é o caso.   gl
 - Chrome e Firefox en MacOS non son compatibles (unicamente Safari é compatible con MacOS), pero invocarase PSAL ao intentar empregar Chrome ou Firefox.        gl
 Mago da luz / Maga da luz       gl
@@ -214,16 +217,16 @@
 Saltar á navegación Navegación INICIO   gl
 Julio Freire, competidor da FGA, invitado polo Kennel club de Inglaterra, para participar nos Crufts 2014 (Birmingham, 6 - 9 de marzo). es
 25 de xullo - Truong Tan Sang toma posesión como presidente de Vietnam  gl
 Quen pode solicitar o dito financiamento?       gl
 ```
 Getting stats:
 ```
-cat inputtext | fastspell $L --aggr | cut -f2 | sort | uniq -c | sort -nr
-cat inputtext | fastspell $L --cons | cut -f2 | sort | uniq -c | sort -nr
+cat inputtext | fastspell --aggr $L | cut -f2 | sort | uniq -c | sort -nr
+cat inputtext | fastspell --cons $L | cut -f2 | sort | uniq -c | sort -nr
 ```
 Aggressive:
 ```
 9 gl
 1 es
 ```
 Conservative:
```

### Comparing `fastspell-0.8.0/README.md` & `fastspell-0.9.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -15,45 +15,47 @@
 ```
 pip install fastspell
 ```
 or directly from source:
 ```
 pip install .
 ```
-Note that **Hunspell** requires `python-dev` and `libhunspell-dev`:
+Note that it requires Python3.8 or higher, and the `python3-dev` package:
 
 ```
-sudo apt-get install python-dev libhunspell-dev
+sudo apt-get install python3-dev
 ```
 
+**IMPORTANT**:
+In some cases (for example, when using Python 3.10), the `cyhunspell` version 2.0.2 installation will fail. If that's the case, you need to install `cyhunspell==2.0.3` before installing `fastspell`:
+```
+pip install git+https://github.com/MSeal/cython_hunspell@2.0.3
+```
+
+### Model download
+
 To trigger the FastText model download before running fastspell, run:
 ```
 fastspell-download
 ```
-
 Since version 0.7 all the dictionaries are installed automatically with pip and there is no need to do anything else.
 For further explanation about how configuration works, [see below](#configuration).
 
 ### Conda
 Also, you can install the conda package:
 ```
 conda install -c conda-forge -c bitextor fastspell
 ```
 
-### RedHat installation
-For RedHat and its derivatives
+### Automatic testing
+Some automatic tests are provided to check that the installation went fine. In order to check it, go to the `/tests` directory and run:
 ```
-sudo dnf install hunspell hunspell-devel
-```
-must be ran to install Hunspell.
-
-If you found an installation error during `pip install hunspell` that says `/usr/bin/ld: cannot find -lhunspell`, you'll probably need to add a symlink to `/usr/lib64` or other path in your environment (like `/home/user/.local/lib`).
-```
-sudo ln -s /usr/lib64/libhunspell-1.7.so /usr/lib64/libhunspell.so
+python3 -m unittest discover
 ```
+You might need to istall the `unittest` package with `pip`, in  case you don't have it installed beforehand.
 
 ## Configuration
 
 A few configuration files are provided under the `fastspell/config` directory.
 If you need to change default configuration, you can provide the path to your config directory with `-c`/`--config` or with the environment variable `FASTSPELL_CONFIG`.
 
 #### similar.yaml
@@ -128,14 +130,15 @@
   -q, --quiet        Silent logging mode (default: False)
   --debug            Debug logging mode (default: False)
   --logfile LOGFILE  Store log to a file (default: <_io.TextIOWrapper
                      name='<stderr>' mode='w' encoding='UTF-8'>)
   -v, --version      show version of this script and exit
 ```
 
+
 ## Aggressive vs Conservative
 
 FastSpell comes in two flavours: Aggressive and Conservative.
 
 The **Aggressive** mode is less hesitant to tag a sentence with the target language, and never has doubts. The **Conservative** version, on the other hand, is more reluctant to tag a sentence with the target language and will use the `unk`(unknown) tag in case of doubt (when there is a tie between the target language and other language, for example)
 
 ## Benchmark 
@@ -156,16 +159,16 @@
 Saltar á navegación Navegación INICIO
 Julio Freire, competidor da FGA, invitado polo Kennel club de Inglaterra, para participar nos Crufts 2014 (Birmingham, 6 - 9 de marzo).
 25 de xullo - Truong Tan Sang toma posesión como presidente de Vietnam
 Quen pode solicitar o dito financiamento?
 ```
 Command:
 ```
-fastspell $L --aggr inputtext
-fastspell $L --cons inputtext
+fastspell  --aggr lang inputtext
+fastspell  --cons lang inputtext
 ```
 Aggressive output:
 ```
 19-01-2011 47 comentarios 7o Xornadas de Xardinería de Galicia (RE)PLANTEAR     gl
 • Proceso de valoración de idoneidade: entrevistas psicosociais e visita domiciliaria e aplicación de test psicolóxicos, se é o caso.   gl
 - Chrome e Firefox en MacOS non son compatibles (unicamente Safari é compatible con MacOS), pero invocarase PSAL ao intentar empregar Chrome ou Firefox.        gl
 Mago da luz / Maga da luz       gl
@@ -188,16 +191,16 @@
 Saltar á navegación Navegación INICIO   gl
 Julio Freire, competidor da FGA, invitado polo Kennel club de Inglaterra, para participar nos Crufts 2014 (Birmingham, 6 - 9 de marzo). es
 25 de xullo - Truong Tan Sang toma posesión como presidente de Vietnam  gl
 Quen pode solicitar o dito financiamento?       gl
 ```
 Getting stats:
 ```
-cat inputtext | fastspell $L --aggr | cut -f2 | sort | uniq -c | sort -nr
-cat inputtext | fastspell $L --cons | cut -f2 | sort | uniq -c | sort -nr
+cat inputtext | fastspell --aggr $L | cut -f2 | sort | uniq -c | sort -nr
+cat inputtext | fastspell --cons $L | cut -f2 | sort | uniq -c | sort -nr
 ```
 Aggressive:
 ```
 9 gl
 1 es
 ```
 Conservative:
```

### Comparing `fastspell-0.8.0/pyproject.toml` & `fastspell-0.9.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [project]
 name = "fastspell"
-version = "0.8.0"
+version = "0.9.0"
 license = {file = "LICENSE"}
 readme = "README.md"
 description = "Targetted language identifier, based on FastText and Hunspell."
 requires-python = ">=3.8"
 dependencies = [
+    "cyhunspell>=2.0.2, <=2.0.3",
     "fastspell-dictionaries==3.0",
     "fasttext==0.9.2",
-    "hunspell==0.5.5",
     "urllib3",
     "PyYAML",
 ]
 classifiers = [
     "Environment :: Console",
     "Intended Audience :: Science/Research",
     "Programming Language :: Python :: 3.8",
```

### Comparing `fastspell-0.8.0/src/fastspell/config/hunspell.yaml` & `fastspell-0.9.0/src/fastspell/config/hunspell.yaml`

 * *Files identical despite different names*

### Comparing `fastspell-0.8.0/src/fastspell/config/similar.yaml` & `fastspell-0.9.0/src/fastspell/config/similar.yaml`

 * *Files identical despite different names*

### Comparing `fastspell-0.8.0/src/fastspell/fastspell.py` & `fastspell-0.9.0/src/fastspell/fastspell.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,18 +94,18 @@
 
     def search_hunspell_dict(self, lang_code):
         ''' Search in the paths for a hunspell dictionary and load it '''
         for p in self.hunspell_paths:
             if os.path.exists(f"{p}/{lang_code}.dic") and os.path.exists(f"{p}/{lang_code}.aff"):
                 try:
                     dicpath = p + '/' + lang_code
-                    hunspell_obj = hunspell.HunSpell(f"{dicpath}.dic", f"{dicpath}.aff")
+                    hunspell_obj = hunspell.Hunspell(lang_code, hunspell_data_dir=p)
                     logging.debug(f"Loaded hunspell obj for '{lang_code}' in path: {dicpath}")
                     break
-                except hunspell.HunSpellError:
+                except:
                     logging.error("Failed building Hunspell object for " + lang_code)
                     logging.error("Aborting.")
                     exit(1)
         else:
             raise RuntimeError(f"It does not exist any valid dictionary directory"
                                f"for {lang_code} in the paths {self.hunspell_paths}."
                                f"Please, execute 'fastspell-download'.")
@@ -209,15 +209,15 @@
             for l in current_similar:
                 #Get spellchecking for all the mistakeable languages
                 logging.debug(l)
                 dec_sent = sent.encode(encoding='UTF-8',errors='strict').decode('UTF-8') #Not 100% sure about this...
                 raw_toks = sent.strip().split(" ")
                 toks = remove_unwanted_words(raw_toks, self.lang)
                 try:
-                    correct_list = list(map(self.hunspell_objs.get(l).spell, toks))
+                    correct_list = list(map(self.hunspell_objs[l].spell, toks))
                 except UnicodeEncodeError: #...because it sometimes fails here for certain characters
                     correct_list = []
                 corrects = sum(correct_list*1)
                 logging.debug("Tokens: " +str(toks))
                 logging.debug("Corrects: " + str(correct_list))
                 logging.debug("Total: " + str(len(toks)))
                 if corrects > 0:
```

### Comparing `fastspell-0.8.0/src/fastspell/fastspell_download.py` & `fastspell-0.9.0/src/fastspell/fastspell_download.py`

 * *Files identical despite different names*

### Comparing `fastspell-0.8.0/src/fastspell/util.py` & `fastspell-0.9.0/src/fastspell/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,20 +67,20 @@
             config_path = None
 
     if not config_path:
         cur_path = os.path.dirname(__file__)
         config_path = cur_path + "/config"
 
     #similar languages
-    similar_yaml_file = open(config_path+"/similar.yaml")
-    similar_langs = yaml.safe_load(similar_yaml_file)["similar"]
+    with open(config_path+"/similar.yaml") as similar_yaml_file:
+        similar_langs = yaml.safe_load(similar_yaml_file)["similar"]
 
     #hunspell
-    hunspell_codes_file = open(config_path+"/hunspell.yaml")
-    hunspell_config = yaml.safe_load(hunspell_codes_file)
+    with open(config_path+"/hunspell.yaml") as hunspell_codes_file:
+        hunspell_config = yaml.safe_load(hunspell_codes_file)
     hunspell_codes = hunspell_config["hunspell_codes"]
     if hunspell_config["dictpath"]:
         # If config has a hunspell path, add it
         if os.path.isabs(hunspell_config["dictpath"]):
             config_dictpath = hunspell_config["dictpath"]
         else:
             config_dictpath = os.path.join(config_path, hunspell_config["dictpath"])
```

### Comparing `fastspell-0.8.0/src/fastspell.egg-info/PKG-INFO` & `fastspell-0.9.0/src/fastspell.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastspell
-Version: 0.8.0
+Version: 0.9.0
 Summary: Targetted language identifier, based on FastText and Hunspell.
 Author-email: Prompsit Language Engineering <info@prompsit.com>
 Maintainer-email: Marta Bañon <mbanon@prompsit.com>, Jaume Zaragoza <jzaragoza@prompsit.com>
 Project-URL: Homepage, https://github.com/mbanon/fastspell
 Project-URL: FastSpell on GitHub, https://github.com/mbanon/fastspell
 Project-URL: Prompsit Language Engineering, http://www.prompsit.com
 Project-URL: Paracrawl, https://paracrawl.eu/
@@ -41,45 +41,47 @@
 ```
 pip install fastspell
 ```
 or directly from source:
 ```
 pip install .
 ```
-Note that **Hunspell** requires `python-dev` and `libhunspell-dev`:
+Note that it requires Python3.8 or higher, and the `python3-dev` package:
 
 ```
-sudo apt-get install python-dev libhunspell-dev
+sudo apt-get install python3-dev
 ```
 
+**IMPORTANT**:
+In some cases (for example, when using Python 3.10), the `cyhunspell` version 2.0.2 installation will fail. If that's the case, you need to install `cyhunspell==2.0.3` before installing `fastspell`:
+```
+pip install git+https://github.com/MSeal/cython_hunspell@2.0.3
+```
+
+### Model download
+
 To trigger the FastText model download before running fastspell, run:
 ```
 fastspell-download
 ```
-
 Since version 0.7 all the dictionaries are installed automatically with pip and there is no need to do anything else.
 For further explanation about how configuration works, [see below](#configuration).
 
 ### Conda
 Also, you can install the conda package:
 ```
 conda install -c conda-forge -c bitextor fastspell
 ```
 
-### RedHat installation
-For RedHat and its derivatives
+### Automatic testing
+Some automatic tests are provided to check that the installation went fine. In order to check it, go to the `/tests` directory and run:
 ```
-sudo dnf install hunspell hunspell-devel
-```
-must be ran to install Hunspell.
-
-If you found an installation error during `pip install hunspell` that says `/usr/bin/ld: cannot find -lhunspell`, you'll probably need to add a symlink to `/usr/lib64` or other path in your environment (like `/home/user/.local/lib`).
-```
-sudo ln -s /usr/lib64/libhunspell-1.7.so /usr/lib64/libhunspell.so
+python3 -m unittest discover
 ```
+You might need to istall the `unittest` package with `pip`, in  case you don't have it installed beforehand.
 
 ## Configuration
 
 A few configuration files are provided under the `fastspell/config` directory.
 If you need to change default configuration, you can provide the path to your config directory with `-c`/`--config` or with the environment variable `FASTSPELL_CONFIG`.
 
 #### similar.yaml
@@ -154,14 +156,15 @@
   -q, --quiet        Silent logging mode (default: False)
   --debug            Debug logging mode (default: False)
   --logfile LOGFILE  Store log to a file (default: <_io.TextIOWrapper
                      name='<stderr>' mode='w' encoding='UTF-8'>)
   -v, --version      show version of this script and exit
 ```
 
+
 ## Aggressive vs Conservative
 
 FastSpell comes in two flavours: Aggressive and Conservative.
 
 The **Aggressive** mode is less hesitant to tag a sentence with the target language, and never has doubts. The **Conservative** version, on the other hand, is more reluctant to tag a sentence with the target language and will use the `unk`(unknown) tag in case of doubt (when there is a tie between the target language and other language, for example)
 
 ## Benchmark 
@@ -182,16 +185,16 @@
 Saltar á navegación Navegación INICIO
 Julio Freire, competidor da FGA, invitado polo Kennel club de Inglaterra, para participar nos Crufts 2014 (Birmingham, 6 - 9 de marzo).
 25 de xullo - Truong Tan Sang toma posesión como presidente de Vietnam
 Quen pode solicitar o dito financiamento?
 ```
 Command:
 ```
-fastspell $L --aggr inputtext
-fastspell $L --cons inputtext
+fastspell  --aggr lang inputtext
+fastspell  --cons lang inputtext
 ```
 Aggressive output:
 ```
 19-01-2011 47 comentarios 7o Xornadas de Xardinería de Galicia (RE)PLANTEAR     gl
 • Proceso de valoración de idoneidade: entrevistas psicosociais e visita domiciliaria e aplicación de test psicolóxicos, se é o caso.   gl
 - Chrome e Firefox en MacOS non son compatibles (unicamente Safari é compatible con MacOS), pero invocarase PSAL ao intentar empregar Chrome ou Firefox.        gl
 Mago da luz / Maga da luz       gl
@@ -214,16 +217,16 @@
 Saltar á navegación Navegación INICIO   gl
 Julio Freire, competidor da FGA, invitado polo Kennel club de Inglaterra, para participar nos Crufts 2014 (Birmingham, 6 - 9 de marzo). es
 25 de xullo - Truong Tan Sang toma posesión como presidente de Vietnam  gl
 Quen pode solicitar o dito financiamento?       gl
 ```
 Getting stats:
 ```
-cat inputtext | fastspell $L --aggr | cut -f2 | sort | uniq -c | sort -nr
-cat inputtext | fastspell $L --cons | cut -f2 | sort | uniq -c | sort -nr
+cat inputtext | fastspell --aggr $L | cut -f2 | sort | uniq -c | sort -nr
+cat inputtext | fastspell --cons $L | cut -f2 | sort | uniq -c | sort -nr
 ```
 Aggressive:
 ```
 9 gl
 1 es
 ```
 Conservative:
```

