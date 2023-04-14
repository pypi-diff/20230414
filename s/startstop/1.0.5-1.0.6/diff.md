# Comparing `tmp/startstop-1.0.5.tar.gz` & `tmp/startstop-1.0.6.tar.gz`

## Comparing `startstop-1.0.5.tar` & `startstop-1.0.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 startstop-1.0.5/.DS_Store
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 startstop-1.0.5/example.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 startstop-1.0.5/startstop/__about__.py
--rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 startstop-1.0.5/startstop/__init__.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 startstop-1.0.5/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 startstop-1.0.5/LICENSE.txt
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 startstop-1.0.5/README.md
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 startstop-1.0.5/pyproject.toml
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 startstop-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 startstop-1.0.6/.DS_Store
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 startstop-1.0.6/example.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 startstop-1.0.6/startstop/__about__.py
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 startstop-1.0.6/startstop/__init__.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 startstop-1.0.6/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 startstop-1.0.6/LICENSE.txt
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 startstop-1.0.6/README.md
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 startstop-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 startstop-1.0.6/PKG-INFO
```

### Comparing `startstop-1.0.5/.DS_Store` & `startstop-1.0.6/.DS_Store`

 * *Files identical despite different names*

### Comparing `startstop-1.0.5/example.py` & `startstop-1.0.6/example.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,47 +2,49 @@
 
 
 def your_code():
     for i in range(100000):
         i**2
 
 
-# Profiler
-p()
-your_code()
-p()
-
-
-# Profiler as contex manager
-with pc():
-    your_code()
-
-
-# Profiler as contex manager with config
-with pc(interval=0.002, async_mode="enabled"):
-    your_code()
-
-
 # Simple timer
 t()
 your_code()
 t()
-# ... TIMER: 0.024 sec
 
 
 # Simple timer with label and precision config
 t(label="your label", precision=2)
 your_code()
 t()
-# ... TIMER your label: 0.02 sec
 
 
 # Simple timer as contex manager
 with tc():
     your_code()
-# ... TIMER: 0.024 sec
 
 
 # Simple timer as contex manager label and precision config
 with tc(label="your label", precision=2):
     your_code()
-# ... TIMER your label: 0.02 sec
+
+
+# Profiler
+p()
+your_code()
+p()
+
+
+# Profiler with config
+p(interval=0.01, async_mode="enabled")
+your_code()
+p()
+
+
+# Profiler as contex manager
+with pc():
+    your_code()
+
+
+# Profiler as contex manager with config
+with pc(interval=0.002, async_mode="enabled"):
+    your_code()
```

### Comparing `startstop-1.0.5/startstop/__init__.py` & `startstop-1.0.6/startstop/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from pyinstrument import Profiler
 from time import perf_counter
 
 
 class StartStopProfiler:
-    def __init__(self, interval=0.001, async_mode="enabled"):
-        self.profiler = Profiler(interval, async_mode)
+    def __init__(self):
         self.running = False
 
-    def __call__(self):
+    def __call__(self, interval=0.001, async_mode="enabled"):
         if not self.running:
+            self.profiler = Profiler(interval, async_mode)
             self.profiler.start()
             self.running = True
         else:
             self.profiler.stop()
             self.running = False
             self.profiler.open_in_browser()
             self.profiler.reset()
```

### Comparing `startstop-1.0.5/.gitignore` & `startstop-1.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `startstop-1.0.5/LICENSE.txt` & `startstop-1.0.6/LICENSE.txt`

 * *Files identical despite different names*

