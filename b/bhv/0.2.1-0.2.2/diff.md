# Comparing `tmp/bhv-0.2.1.tar.gz` & `tmp/bhv-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bhv-0.2.1.tar", last modified: Wed Apr 12 17:38:49 2023, max compression
+gzip compressed data, was "bhv-0.2.2.tar", last modified: Thu Apr 13 23:23:36 2023, max compression
```

## Comparing `bhv-0.2.1.tar` & `bhv-0.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-04-12 17:38:49.661271 bhv-0.2.1/
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1005 2023-04-12 17:38:49.661271 bhv-0.2.1/PKG-INFO
-drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-04-12 17:38:49.661271 bhv-0.2.1/bhv/
--rw-r--r--   0 adamv     (1000) adamv     (1000)       64 2023-04-11 14:49:00.000000 bhv-0.2.1/bhv/__init__.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)    11023 2023-04-12 17:37:58.000000 bhv-0.2.1/bhv/abstract.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1635 2023-04-11 14:49:00.000000 bhv-0.2.1/bhv/embedding.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     9571 2023-04-12 17:37:58.000000 bhv-0.2.1/bhv/np.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     7088 2023-04-12 17:37:58.000000 bhv-0.2.1/bhv/pytorch.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     2022 2023-04-11 14:49:00.000000 bhv-0.2.1/bhv/shared.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     8626 2023-04-12 17:37:58.000000 bhv-0.2.1/bhv/symbolic.py
-drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-04-12 17:38:49.661271 bhv-0.2.1/bhv.egg-info/
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1005 2023-04-12 17:38:49.000000 bhv-0.2.1/bhv.egg-info/PKG-INFO
--rw-r--r--   0 adamv     (1000) adamv     (1000)      246 2023-04-12 17:38:49.000000 bhv-0.2.1/bhv.egg-info/SOURCES.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)        1 2023-04-12 17:38:49.000000 bhv-0.2.1/bhv.egg-info/dependency_links.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)       73 2023-04-12 17:38:49.000000 bhv-0.2.1/bhv.egg-info/requires.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)        4 2023-04-12 17:38:49.000000 bhv-0.2.1/bhv.egg-info/top_level.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)       38 2023-04-12 17:38:49.661271 bhv-0.2.1/setup.cfg
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1331 2023-04-12 17:38:05.000000 bhv-0.2.1/setup.py
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-04-13 23:23:36.918571 bhv-0.2.2/
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1005 2023-04-13 23:23:36.918571 bhv-0.2.2/PKG-INFO
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-04-13 23:23:36.918571 bhv-0.2.2/bhv/
+-rw-r--r--   0 adamv     (1000) adamv     (1000)       64 2023-04-11 14:49:00.000000 bhv-0.2.2/bhv/__init__.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    11347 2023-04-13 17:08:27.000000 bhv-0.2.2/bhv/abstract.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1635 2023-04-11 14:49:00.000000 bhv-0.2.2/bhv/embedding.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     9571 2023-04-12 17:37:58.000000 bhv-0.2.2/bhv/np.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     7088 2023-04-12 17:37:58.000000 bhv-0.2.2/bhv/pytorch.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     2022 2023-04-11 14:49:00.000000 bhv-0.2.2/bhv/shared.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     8750 2023-04-13 22:34:48.000000 bhv-0.2.2/bhv/symbolic.py
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-04-13 23:23:36.918571 bhv-0.2.2/bhv.egg-info/
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1005 2023-04-13 23:23:36.000000 bhv-0.2.2/bhv.egg-info/PKG-INFO
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      246 2023-04-13 23:23:36.000000 bhv-0.2.2/bhv.egg-info/SOURCES.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)        1 2023-04-13 23:23:36.000000 bhv-0.2.2/bhv.egg-info/dependency_links.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)       73 2023-04-13 23:23:36.000000 bhv-0.2.2/bhv.egg-info/requires.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)        4 2023-04-13 23:23:36.000000 bhv-0.2.2/bhv.egg-info/top_level.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)       38 2023-04-13 23:23:36.918571 bhv-0.2.2/setup.cfg
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1331 2023-04-13 22:35:40.000000 bhv-0.2.2/setup.py
```

### Comparing `bhv-0.2.1/PKG-INFO` & `bhv-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bhv
-Version: 0.2.1
+Version: 0.2.2
 Summary: Boolean Hypervectors
 Author: Adam Vandervorst
 Author-email: contact@adamv.be
 Keywords: ai binary hypervector hdc bsc
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `bhv-0.2.1/bhv/abstract.py` & `bhv-0.2.2/bhv/abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,28 @@
 
     @classmethod
     def majority3(cls, x, y, z) -> Self:
         return cls.majority([x, y, z])
 
     @classmethod
     def majority(cls, vs: list[Self]) -> Self:
-        assert len(vs) % 2 == 1,  "The majority function which is only defined on uneven length inputs, see maj_bundle"
+        n = len(vs)
+
+        if n == 0:
+            return cls.rand()
+        elif n == 1:
+            return vs[0]
+        elif n % 2 == 0:
+            return cls.majority([cls.rand()] + vs)
+        else:
+            return cls._true_majority(vs)
+
+    @classmethod
+    def _true_majority(cls, vs: list[Self]) -> Self:
+        assert len(vs) % 2 == 1,  "The true majority function which is only defined on uneven length inputs, see `majority`"
         half = len(vs)//2
         disjunction = list(accumulate(vs[:half-1:-1], or_))[1:]
         conjunction = list(accumulate(vs[:half-1:-1], and_))[1:]
 
         @cache
         def rec(ons, offs):
             if ons + 1 > half:
```

### Comparing `bhv-0.2.1/bhv/embedding.py` & `bhv-0.2.2/bhv/embedding.py`

 * *Files identical despite different names*

### Comparing `bhv-0.2.1/bhv/np.py` & `bhv-0.2.2/bhv/np.py`

 * *Files identical despite different names*

### Comparing `bhv-0.2.1/bhv/pytorch.py` & `bhv-0.2.2/bhv/pytorch.py`

 * *Files identical despite different names*

### Comparing `bhv-0.2.1/bhv/shared.py` & `bhv-0.2.2/bhv/shared.py`

 * *Files identical despite different names*

### Comparing `bhv-0.2.1/bhv/symbolic.py` & `bhv-0.2.2/bhv/symbolic.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,16 +71,16 @@
     global randpermid
     randpermid += 1
     return randpermid
 @dataclass
 class PermRandom(SymbolicPermutation):
     id: int = field(default_factory=next_perm_id)
 
-    def show(self, impl="", **kwargs):
-        return impl + "random()"
+    def show(self, impl="", random_id=False, **kwargs):
+        return f"<{impl}random {self.id}>" if random_id else impl + "random()"
 @dataclass
 class PermCompose(SymbolicPermutation):
     l: 'SymbolicPermutation'
     r: 'SymbolicPermutation'
 
     def show(self, **kwargs):
         return f"({self.l.show(**kwargs)} * {self.r.show(**kwargs)})"
@@ -199,16 +199,16 @@
     global randid
     randid += 1
     return randid
 @dataclass
 class Rand(SymbolicBHV):
     id: int = field(default_factory=next_id)
 
-    def show(self, impl="", **kwargs):
-        return impl + "rand()"
+    def show(self, impl="", random_id=False, **kwargs):
+        return f"<{impl}rand {self.id}>" if random_id else impl + "rand()"
 @dataclass
 class Rand2(SymbolicBHV):
     power: int
 
     def show(self, impl="", **kwargs):
         return impl + f"rand2({self.power})"
 @dataclass
```

### Comparing `bhv-0.2.1/bhv.egg-info/PKG-INFO` & `bhv-0.2.2/bhv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bhv
-Version: 0.2.1
+Version: 0.2.2
 Summary: Boolean Hypervectors
 Author: Adam Vandervorst
 Author-email: contact@adamv.be
 Keywords: ai binary hypervector hdc bsc
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `bhv-0.2.1/setup.py` & `bhv-0.2.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.2.1'
+VERSION = '0.2.2'
 DESCRIPTION = 'Boolean Hypervectors'
 LONG_DESCRIPTION = 'Boolean Hypervectors with various operators for experiments in hyperdimensional computing (HDC).'
 
 setup(
     name="bhv",
     version=VERSION,
     author="Adam Vandervorst",
```

