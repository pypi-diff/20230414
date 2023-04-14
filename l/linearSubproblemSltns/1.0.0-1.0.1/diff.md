# Comparing `tmp/linearsubproblemsltns-1.0.0.tar.gz` & `tmp/linearsubproblemsltns-1.0.1.tar.gz`

## Comparing `linearsubproblemsltns-1.0.0.tar` & `linearsubproblemsltns-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,15 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.0/src/linearSubproblemSltns/__init__.py
--rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.0/src/linearSubproblemSltns/rand_py.py
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.0/src/linearSubproblemSltns/sp1_lib.py
--rw-r--r--   0        0        0     3501 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.0/src/linearSubproblemSltns/sp2E_lib.py
--rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.0/src/linearSubproblemSltns/sp2_lib.py
--rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.0/src/linearSubproblemSltns/sp3_lib.py
--rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.0/src/linearSubproblemSltns/sp4_lib.py
--rw-r--r--   0        0        0     5679 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.0/src/linearSubproblemSltns/sp5_lib.py
--rw-r--r--   0        0        0     5254 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.0/src/linearSubproblemSltns/sp6_lib.py
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.0/LICENSE
--rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.0/README.md
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.1/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.1/src/linearSubproblemSltns/__init__.py
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.1/src/linearSubproblemSltns/rand_py.py
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.1/src/linearSubproblemSltns/sp1_lib.py
+-rw-r--r--   0        0        0     3501 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.1/src/linearSubproblemSltns/sp2E_lib.py
+-rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.1/src/linearSubproblemSltns/sp2_lib.py
+-rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.1/src/linearSubproblemSltns/sp3_lib.py
+-rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.1/src/linearSubproblemSltns/sp4_lib.py
+-rw-r--r--   0        0        0     5679 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.1/src/linearSubproblemSltns/sp5_lib.py
+-rw-r--r--   0        0        0     5254 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.1/src/linearSubproblemSltns/sp6_lib.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.1/README.md
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 linearsubproblemsltns-1.0.1/PKG-INFO
```

### Comparing `linearsubproblemsltns-1.0.0/src/linearSubproblemSltns/rand_py.py` & `linearsubproblemsltns-1.0.1/src/linearSubproblemSltns/rand_py.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,20 +10,20 @@
    return round(r.random(), 15)*2*math.pi-math.pi
 
 #Create random matrix of size 3 x size (rows, cols)
 def rand_mat(size = 1): #Make list of lists, then pass to numpy
    return np.array([[round(r.random(), 15) for x in range(3)] for y in range(size)])
 
 #Create random vector of size 3 x N
-def rand_vec(): #Make list of lists, then pass to numpy
-   return np.array([round(r.random(), 15) for y in range(3)])
+def rand_vec(size = 3): #Make list of lists, then pass to numpy
+   return np.array([round(r.random(), 15) for y in range(size)])
 
 #Create random normal vector
-def rand_normal_vec():
-   vec = rand_vec()
+def rand_normal_vec(size = 3):
+   vec = rand_vec(size)
    return vec/np.linalg.norm(vec, 2)
 
 #Create random normal matrix
 def rand_normal_mat(size = 1):
    #vec = rand_vec()
    #return np.array([[rand_vec()/] for y in range(0, 3)])
    lst = np.zeros((size, 3))
```

### Comparing `linearsubproblemsltns-1.0.0/src/linearSubproblemSltns/sp1_lib.py` & `linearsubproblemsltns-1.0.1/src/linearSubproblemSltns/sp1_lib.py`

 * *Files identical despite different names*

### Comparing `linearsubproblemsltns-1.0.0/src/linearSubproblemSltns/sp2E_lib.py` & `linearsubproblemsltns-1.0.1/src/linearSubproblemSltns/sp2E_lib.py`

 * *Files identical despite different names*

### Comparing `linearsubproblemsltns-1.0.0/src/linearSubproblemSltns/sp2_lib.py` & `linearsubproblemsltns-1.0.1/src/linearSubproblemSltns/sp2_lib.py`

 * *Files identical despite different names*

### Comparing `linearsubproblemsltns-1.0.0/src/linearSubproblemSltns/sp3_lib.py` & `linearsubproblemsltns-1.0.1/src/linearSubproblemSltns/sp3_lib.py`

 * *Files identical despite different names*

### Comparing `linearsubproblemsltns-1.0.0/src/linearSubproblemSltns/sp4_lib.py` & `linearsubproblemsltns-1.0.1/src/linearSubproblemSltns/sp4_lib.py`

 * *Files identical despite different names*

### Comparing `linearsubproblemsltns-1.0.0/src/linearSubproblemSltns/sp5_lib.py` & `linearsubproblemsltns-1.0.1/src/linearSubproblemSltns/sp5_lib.py`

 * *Files identical despite different names*

### Comparing `linearsubproblemsltns-1.0.0/src/linearSubproblemSltns/sp6_lib.py` & `linearsubproblemsltns-1.0.1/src/linearSubproblemSltns/sp6_lib.py`

 * *Files identical despite different names*

### Comparing `linearsubproblemsltns-1.0.0/LICENSE` & `linearsubproblemsltns-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `linearsubproblemsltns-1.0.0/pyproject.toml` & `linearsubproblemsltns-1.0.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 [build-system]
-requires = ["hatchling", "numpy", "scipy"]
+requires = ["hatchling", "scipy", "numpy"]
 build-backend = "hatchling.build"
 [project]
 name = "linearSubproblemSltns"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name ="Alexander Elias", email ="eliasa3@rpi.edu" }, { name="Ashton Ropp", email="ashr8011@gmail.com" },
 ]
 description = "This is a new tool for multi-joint robotic arm calculations developed at RPI."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent",
 ]
+dependencies = [
+  "numpy>=1.22.3",
+  "scipy>=1.10.0",
+]
 
 [project.urls]
 "Homepage" = "https://github.com/rpiRobotics/linear-subproblem-solutions"
 "Bug Tracker" = "https://github.com/rpiRobotics/linear-subproblem-solutions/issues"
 "Paper" = "https://arxiv.org/pdf/2211.05737.pdf"
```

### Comparing `linearsubproblemsltns-1.0.0/PKG-INFO` & `linearsubproblemsltns-1.0.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: linearSubproblemSltns
-Version: 1.0.0
+Version: 1.0.1
 Summary: This is a new tool for multi-joint robotic arm calculations developed at RPI.
 Project-URL: Homepage, https://github.com/rpiRobotics/linear-subproblem-solutions
 Project-URL: Bug Tracker, https://github.com/rpiRobotics/linear-subproblem-solutions/issues
 Project-URL: Paper, https://arxiv.org/pdf/2211.05737.pdf
 Author-email: Alexander Elias <eliasa3@rpi.edu>, Ashton Ropp <ashr8011@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
+Requires-Dist: numpy>=1.22.3
+Requires-Dist: scipy>=1.10.0
 Description-Content-Type: text/markdown
 
 # Summary:
 - This is a research project led by Alexander Elias and Dr. John Wen at RPI.
 - Summation of research: https://arxiv.org/pdf/2211.05737.pdf
 - Included here is the Python version of the MATLAB-based canonical subproblems for inverse kinematics on robots.
 - Additional MATLAB, C++, Rust, and Python files are located at https://github.com/rpiRobotics/linear-subproblem-solutions/.
@@ -45,8 +47,20 @@
    p2 = [0.71384302 0.84785577 0.40390217]\
    k1 = [0.53432959 0.73260445 0.42164275]\
    k2 = [0.89871158 0.33336884 0.2849258 ]
 ### In MATLAB:
    p1 = [0.85421456; 0.9145417;  0.28164908]\
    p2 = [0.71384302; 0.84785577; 0.40390217]\
    k1 = [0.53432959; 0.73260445; 0.42164275]\
-   k2 = [0.89871158; 0.33336884; 0.2849258 ]
+   k2 = [0.89871158; 0.33336884; 0.2849258 ]
+
+---
+## Timing
+| Subproblem    | Time With Inputs | Time Without Inputs  |
+| ------------- | ---------------  | ------------------   |
+| Sp1           | 78716.896 ns     | 73754.058 ns         |
+| Sp2           | 325238.43 ns     | 318135.293 ns        |
+| Sp2E          | 409206.773 ns    | 400298.479 ns        |
+| Sp3           | 127781.537 ns    | 122444.399 ns        |
+| Sp4           | 104747.862 ns    | 99615.851 ns         |
+| Sp5           | 1353110.805 ns   | 1341531.159 ns       |
+| Sp6           | 614233.523 ns    | 596708.225 ns        |
```

