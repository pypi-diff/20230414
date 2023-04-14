# Comparing `tmp/durkon-0.0.7.tar.gz` & `tmp/durkon-0.0.8.tar.gz`

## Comparing `durkon-0.0.7.tar` & `durkon-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 durkon-0.0.7/src/durkon/__init__.py
--rw-r--r--   0        0        0    35433 2020-02-02 00:00:00.000000 durkon-0.0.7/src/durkon/actual_modelling.py
--rw-r--r--   0        0        0     5455 2020-02-02 00:00:00.000000 durkon-0.0.7/src/durkon/calculus.py
--rw-r--r--   0        0        0     8842 2020-02-02 00:00:00.000000 durkon-0.0.7/src/durkon/export.py
--rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 durkon-0.0.7/src/durkon/metrics.py
--rw-r--r--   0        0        0    23509 2020-02-02 00:00:00.000000 durkon-0.0.7/src/durkon/misc.py
--rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 durkon-0.0.7/src/durkon/pena.py
--rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 durkon-0.0.7/src/durkon/prep.py
--rw-r--r--   0        0        0     3948 2020-02-02 00:00:00.000000 durkon-0.0.7/src/durkon/rele.py
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 durkon-0.0.7/src/durkon/util.py
--rw-r--r--   0        0        0    12912 2020-02-02 00:00:00.000000 durkon-0.0.7/src/durkon/viz.py
--rw-r--r--   0        0        0    38674 2020-02-02 00:00:00.000000 durkon-0.0.7/src/durkon/wraps.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 durkon-0.0.7/LICENSE
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 durkon-0.0.7/README.md
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 durkon-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 durkon-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 durkon-0.0.8/src/durkon/__init__.py
+-rw-r--r--   0        0        0    35481 2020-02-02 00:00:00.000000 durkon-0.0.8/src/durkon/actual_modelling.py
+-rw-r--r--   0        0        0     5455 2020-02-02 00:00:00.000000 durkon-0.0.8/src/durkon/calculus.py
+-rw-r--r--   0        0        0     8842 2020-02-02 00:00:00.000000 durkon-0.0.8/src/durkon/export.py
+-rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 durkon-0.0.8/src/durkon/metrics.py
+-rw-r--r--   0        0        0    23509 2020-02-02 00:00:00.000000 durkon-0.0.8/src/durkon/misc.py
+-rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 durkon-0.0.8/src/durkon/pena.py
+-rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 durkon-0.0.8/src/durkon/prep.py
+-rw-r--r--   0        0        0     3948 2020-02-02 00:00:00.000000 durkon-0.0.8/src/durkon/rele.py
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 durkon-0.0.8/src/durkon/util.py
+-rw-r--r--   0        0        0    12912 2020-02-02 00:00:00.000000 durkon-0.0.8/src/durkon/viz.py
+-rw-r--r--   0        0        0    38674 2020-02-02 00:00:00.000000 durkon-0.0.8/src/durkon/wraps.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 durkon-0.0.8/LICENSE
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 durkon-0.0.8/README.md
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 durkon-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 durkon-0.0.8/PKG-INFO
```

### Comparing `durkon-0.0.7/src/durkon/actual_modelling.py` & `durkon-0.0.8/src/durkon/actual_modelling.py`

 * *Files 1% similar despite different names*

```diff
@@ -330,27 +330,30 @@
   
   history.append(models)
  
  if record: 
   return models, history
  return models
 
-def train_model(inputDf, target, nrounds, lr, startingModel, weight=None, staticFeats = [], pen=0, specificPens={}, lossgrad=calculus.Poisson_grad, link=calculus.Unity_link, linkgrad=calculus.Unity_link_grad, minRela=None, prints="verbose", record=False):
+def train_model(inputDf, target, nrounds, lr, startingModel, weightCol=None, staticFeats = [], pen=0, specificPens={}, lossgrad=calculus.Poisson_grad, link=calculus.Unity_link, linkgrad=calculus.Unity_link_grad, minRela=None, prints="verbose", record=False):
  
  history=[]
  
  inputDf = inputDf.reset_index()
  
  model = copy.deepcopy(startingModel)
  
  if prints!="silent":
   print("initial weights and relevances setup")
  
- if weight==None:
+ 
+ if weightCol==None:
   weight = np.ones(len(inputDf))
+ else:
+  weight = inputDf[weightCol]
  w = np.array(np.transpose(np.matrix(weight)))
  
  cord = rele.produce_cont_relevances_dict(inputDf,model) #d(feat)/d(pt)
  card = rele.produce_cat_relevances_dict(inputDf,model) #d(feat)/d(pt)
  tord = rele.produce_total_relevances_dict(cord, card)
  
  cowrd = rele.produce_wReleDict(cord, w) #d(feat)/d(pt), adjusted for weighting
```

### Comparing `durkon-0.0.7/src/durkon/calculus.py` & `durkon-0.0.8/src/durkon/calculus.py`

 * *Files identical despite different names*

### Comparing `durkon-0.0.7/src/durkon/export.py` & `durkon-0.0.8/src/durkon/export.py`

 * *Files identical despite different names*

### Comparing `durkon-0.0.7/src/durkon/metrics.py` & `durkon-0.0.8/src/durkon/metrics.py`

 * *Files identical despite different names*

### Comparing `durkon-0.0.7/src/durkon/misc.py` & `durkon-0.0.8/src/durkon/misc.py`

 * *Files identical despite different names*

### Comparing `durkon-0.0.7/src/durkon/pena.py` & `durkon-0.0.8/src/durkon/pena.py`

 * *Files identical despite different names*

### Comparing `durkon-0.0.7/src/durkon/prep.py` & `durkon-0.0.8/src/durkon/prep.py`

 * *Files identical despite different names*

### Comparing `durkon-0.0.7/src/durkon/rele.py` & `durkon-0.0.8/src/durkon/rele.py`

 * *Files identical despite different names*

### Comparing `durkon-0.0.7/src/durkon/viz.py` & `durkon-0.0.8/src/durkon/viz.py`

 * *Files identical despite different names*

### Comparing `durkon-0.0.7/src/durkon/wraps.py` & `durkon-0.0.8/src/durkon/wraps.py`

 * *Files identical despite different names*

### Comparing `durkon-0.0.7/LICENSE` & `durkon-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `durkon-0.0.7/pyproject.toml` & `durkon-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "durkon"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Hugh Panton", email="hugh.panton@protonmail.com" },
 ]
 description = "A package for creating insurance-style GLM models, and extensions thereof."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `durkon-0.0.7/PKG-INFO` & `durkon-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: durkon
-Version: 0.0.7
+Version: 0.0.8
 Summary: A package for creating insurance-style GLM models, and extensions thereof.
 Project-URL: Homepage, https://github.com/H-B-P/DURKON
 Project-URL: Bug Tracker, https://github.com/H-B-P/DURKON/issues
 Author-email: Hugh Panton <hugh.panton@protonmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Operating System :: OS Independent
```

