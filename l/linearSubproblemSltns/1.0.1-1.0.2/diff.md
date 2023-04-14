# Comparing `tmp/linearsubproblemsltns-1.0.1.tar.gz` & `tmp/linearsubproblemsltns-1.0.2.tar.gz`

## Comparing `linearsubproblemsltns-1.0.1.tar` & `linearsubproblemsltns-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.1/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.1/src/linearSubproblemSltns/__init__.py
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.1/src/linearSubproblemSltns/rand_py.py
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.1/src/linearSubproblemSltns/sp1_lib.py
--rw-r--r--   0        0        0     3501 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.1/src/linearSubproblemSltns/sp2E_lib.py
--rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.1/src/linearSubproblemSltns/sp2_lib.py
--rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.1/src/linearSubproblemSltns/sp3_lib.py
--rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.1/src/linearSubproblemSltns/sp4_lib.py
--rw-r--r--   0        0        0     5679 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.1/src/linearSubproblemSltns/sp5_lib.py
--rw-r--r--   0        0        0     5254 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.1/src/linearSubproblemSltns/sp6_lib.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.1/.gitignore
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.1/LICENSE
--rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.1/README.md
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.2/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.2/src/linearSubproblemSltns/__init__.py
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.2/src/linearSubproblemSltns/rand_py.py
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.2/src/linearSubproblemSltns/sp1_lib.py
+-rw-r--r--   0        0        0     3501 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.2/src/linearSubproblemSltns/sp2E_lib.py
+-rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.2/src/linearSubproblemSltns/sp2_lib.py
+-rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.2/src/linearSubproblemSltns/sp3_lib.py
+-rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.2/src/linearSubproblemSltns/sp4_lib.py
+-rw-r--r--   0        0        0     5679 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.2/src/linearSubproblemSltns/sp5_lib.py
+-rw-r--r--   0        0        0     5254 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.2/src/linearSubproblemSltns/sp6_lib.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.2/LICENSE
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.2/README.md
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.2/PKG-INFO
```

### Comparing `linearsubproblemsltns-1.0.1/src/linearSubproblemSltns/rand_py.py` & `linearsubproblemsltns-1.0.2/src/linearSubproblemSltns/rand_py.py`

 * *Files identical despite different names*

### Comparing `linearsubproblemsltns-1.0.1/src/linearSubproblemSltns/sp1_lib.py` & `linearsubproblemsltns-1.0.2/src/linearSubproblemSltns/sp1_lib.py`

 * *Files identical despite different names*

### Comparing `linearsubproblemsltns-1.0.1/src/linearSubproblemSltns/sp2E_lib.py` & `linearsubproblemsltns-1.0.2/src/linearSubproblemSltns/sp2E_lib.py`

 * *Files identical despite different names*

### Comparing `linearsubproblemsltns-1.0.1/src/linearSubproblemSltns/sp2_lib.py` & `linearsubproblemsltns-1.0.2/src/linearSubproblemSltns/sp2_lib.py`

 * *Files identical despite different names*

### Comparing `linearsubproblemsltns-1.0.1/src/linearSubproblemSltns/sp3_lib.py` & `linearsubproblemsltns-1.0.2/src/linearSubproblemSltns/sp3_lib.py`

 * *Files identical despite different names*

### Comparing `linearsubproblemsltns-1.0.1/src/linearSubproblemSltns/sp4_lib.py` & `linearsubproblemsltns-1.0.2/src/linearSubproblemSltns/sp4_lib.py`

 * *Files identical despite different names*

### Comparing `linearsubproblemsltns-1.0.1/src/linearSubproblemSltns/sp5_lib.py` & `linearsubproblemsltns-1.0.2/src/linearSubproblemSltns/sp5_lib.py`

 * *Files identical despite different names*

### Comparing `linearsubproblemsltns-1.0.1/src/linearSubproblemSltns/sp6_lib.py` & `linearsubproblemsltns-1.0.2/src/linearSubproblemSltns/sp6_lib.py`

 * *Files identical despite different names*

### Comparing `linearsubproblemsltns-1.0.1/LICENSE` & `linearsubproblemsltns-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `linearsubproblemsltns-1.0.1/README.md` & `linearsubproblemsltns-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `linearsubproblemsltns-1.0.1/pyproject.toml` & `linearsubproblemsltns-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling", "scipy", "numpy"]
 build-backend = "hatchling.build"
 [project]
 name = "linearSubproblemSltns"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name ="Alexander Elias", email ="eliasa3@rpi.edu" }, { name="Ashton Ropp", email="ashr8011@gmail.com" },
 ]
 description = "This is a new tool for multi-joint robotic arm calculations developed at RPI."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `linearsubproblemsltns-1.0.1/PKG-INFO` & `linearsubproblemsltns-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linearSubproblemSltns
-Version: 1.0.1
+Version: 1.0.2
 Summary: This is a new tool for multi-joint robotic arm calculations developed at RPI.
 Project-URL: Homepage, https://github.com/rpiRobotics/linear-subproblem-solutions
 Project-URL: Bug Tracker, https://github.com/rpiRobotics/linear-subproblem-solutions/issues
 Project-URL: Paper, https://arxiv.org/pdf/2211.05737.pdf
 Author-email: Alexander Elias <eliasa3@rpi.edu>, Ashton Ropp <ashr8011@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: BSD License
```

