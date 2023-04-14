# Comparing `tmp/claspy-0.1.8.tar.gz` & `tmp/claspy-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "claspy-0.1.8.tar", last modified: Wed Apr 12 08:51:24 2023, max compression
+gzip compressed data, was "claspy-0.1.9.tar", last modified: Fri Apr 14 09:32:57 2023, max compression
```

## Comparing `claspy-0.1.8.tar` & `claspy-0.1.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 ermshaua   (501) staff       (20)        0 2023-04-12 08:51:24.498036 claspy-0.1.8/
--rw-r--r--   0 ermshaua   (501) staff       (20)     1500 2023-02-18 10:38:44.000000 claspy-0.1.8/LICENSE
--rw-r--r--   0 ermshaua   (501) staff       (20)     6880 2023-04-12 08:51:24.498260 claspy-0.1.8/PKG-INFO
--rw-r--r--   0 ermshaua   (501) staff       (20)     4084 2023-03-29 19:08:59.000000 claspy-0.1.8/README.md
-drwxr-xr-x   0 ermshaua   (501) staff       (20)        0 2023-04-12 08:51:24.489254 claspy-0.1.8/claspy/
--rw-r--r--   0 ermshaua   (501) staff       (20)        0 2023-02-18 10:41:51.000000 claspy-0.1.8/claspy/__init__.py
--rw-r--r--   0 ermshaua   (501) staff       (20)    16924 2023-04-12 08:45:16.000000 claspy-0.1.8/claspy/clasp.py
--rw-r--r--   0 ermshaua   (501) staff       (20)     4495 2023-02-26 13:47:51.000000 claspy-0.1.8/claspy/data_loader.py
--rw-r--r--   0 ermshaua   (501) staff       (20)     6456 2023-03-05 16:43:36.000000 claspy-0.1.8/claspy/distance.py
--rw-r--r--   0 ermshaua   (501) staff       (20)    15830 2023-04-12 07:38:40.000000 claspy-0.1.8/claspy/nearest_neighbour.py
--rw-r--r--   0 ermshaua   (501) staff       (20)     6099 2023-02-25 09:43:02.000000 claspy-0.1.8/claspy/scoring.py
--rw-r--r--   0 ermshaua   (501) staff       (20)    14897 2023-04-12 07:43:17.000000 claspy-0.1.8/claspy/segmentation.py
-drwxr-xr-x   0 ermshaua   (501) staff       (20)        0 2023-04-12 08:51:24.496604 claspy-0.1.8/claspy/tests/
--rw-r--r--   0 ermshaua   (501) staff       (20)        0 2023-02-20 16:05:58.000000 claspy-0.1.8/claspy/tests/__init__.py
--rw-r--r--   0 ermshaua   (501) staff       (20)     2560 2023-04-12 07:27:07.000000 claspy-0.1.8/claspy/tests/clasp_test.py
--rw-r--r--   0 ermshaua   (501) staff       (20)     6600 2023-02-24 12:09:02.000000 claspy-0.1.8/claspy/tests/evaluation.py
--rw-r--r--   0 ermshaua   (501) staff       (20)     2569 2023-04-12 07:25:30.000000 claspy-0.1.8/claspy/tests/nearest_neighbour_test.py
--rw-r--r--   0 ermshaua   (501) staff       (20)     2937 2023-04-12 07:43:17.000000 claspy-0.1.8/claspy/tests/segmentation_test.py
--rw-r--r--   0 ermshaua   (501) staff       (20)     1683 2023-02-28 15:56:43.000000 claspy-0.1.8/claspy/utils.py
--rw-r--r--   0 ermshaua   (501) staff       (20)     2918 2023-04-03 15:59:10.000000 claspy-0.1.8/claspy/validation.py
--rw-r--r--   0 ermshaua   (501) staff       (20)     6991 2023-02-28 19:59:17.000000 claspy-0.1.8/claspy/window_size.py
-drwxr-xr-x   0 ermshaua   (501) staff       (20)        0 2023-04-12 08:51:24.492299 claspy-0.1.8/claspy.egg-info/
--rw-r--r--   0 ermshaua   (501) staff       (20)     6880 2023-04-12 08:51:24.000000 claspy-0.1.8/claspy.egg-info/PKG-INFO
--rw-r--r--   0 ermshaua   (501) staff       (20)      585 2023-04-12 08:51:24.000000 claspy-0.1.8/claspy.egg-info/SOURCES.txt
--rw-r--r--   0 ermshaua   (501) staff       (20)        1 2023-04-12 08:51:24.000000 claspy-0.1.8/claspy.egg-info/dependency_links.txt
--rw-r--r--   0 ermshaua   (501) staff       (20)        1 2023-04-12 08:51:24.000000 claspy-0.1.8/claspy.egg-info/not-zip-safe
--rw-r--r--   0 ermshaua   (501) staff       (20)      137 2023-04-12 08:51:24.000000 claspy-0.1.8/claspy.egg-info/requires.txt
--rw-r--r--   0 ermshaua   (501) staff       (20)        7 2023-04-12 08:51:24.000000 claspy-0.1.8/claspy.egg-info/top_level.txt
--rw-r--r--   0 ermshaua   (501) staff       (20)     1560 2023-04-12 08:44:56.000000 claspy-0.1.8/pyproject.toml
--rw-r--r--   0 ermshaua   (501) staff       (20)       79 2023-04-12 08:51:24.498849 claspy-0.1.8/setup.cfg
--rw-r--r--   0 ermshaua   (501) staff       (20)     1376 2023-04-12 07:43:17.000000 claspy-0.1.8/setup.py
+drwxr-xr-x   0 ermshaua   (501) staff       (20)        0 2023-04-14 09:32:57.855593 claspy-0.1.9/
+-rw-r--r--   0 ermshaua   (501) staff       (20)     1500 2023-02-18 10:38:44.000000 claspy-0.1.9/LICENSE
+-rw-r--r--   0 ermshaua   (501) staff       (20)     6880 2023-04-14 09:32:57.855730 claspy-0.1.9/PKG-INFO
+-rw-r--r--   0 ermshaua   (501) staff       (20)     4084 2023-03-29 19:08:59.000000 claspy-0.1.9/README.md
+drwxr-xr-x   0 ermshaua   (501) staff       (20)        0 2023-04-14 09:32:57.848999 claspy-0.1.9/claspy/
+-rw-r--r--   0 ermshaua   (501) staff       (20)        0 2023-02-18 10:41:51.000000 claspy-0.1.9/claspy/__init__.py
+-rw-r--r--   0 ermshaua   (501) staff       (20)    16924 2023-04-12 08:45:16.000000 claspy-0.1.9/claspy/clasp.py
+-rw-r--r--   0 ermshaua   (501) staff       (20)     4495 2023-02-26 13:47:51.000000 claspy-0.1.9/claspy/data_loader.py
+-rw-r--r--   0 ermshaua   (501) staff       (20)     6456 2023-03-05 16:43:36.000000 claspy-0.1.9/claspy/distance.py
+-rw-r--r--   0 ermshaua   (501) staff       (20)    15896 2023-04-14 09:18:18.000000 claspy-0.1.9/claspy/nearest_neighbour.py
+-rw-r--r--   0 ermshaua   (501) staff       (20)     6099 2023-02-25 09:43:02.000000 claspy-0.1.9/claspy/scoring.py
+-rw-r--r--   0 ermshaua   (501) staff       (20)    14897 2023-04-12 07:43:17.000000 claspy-0.1.9/claspy/segmentation.py
+drwxr-xr-x   0 ermshaua   (501) staff       (20)        0 2023-04-14 09:32:57.854964 claspy-0.1.9/claspy/tests/
+-rw-r--r--   0 ermshaua   (501) staff       (20)        0 2023-02-20 16:05:58.000000 claspy-0.1.9/claspy/tests/__init__.py
+-rw-r--r--   0 ermshaua   (501) staff       (20)     2560 2023-04-12 07:27:07.000000 claspy-0.1.9/claspy/tests/clasp_test.py
+-rw-r--r--   0 ermshaua   (501) staff       (20)     6600 2023-02-24 12:09:02.000000 claspy-0.1.9/claspy/tests/evaluation.py
+-rw-r--r--   0 ermshaua   (501) staff       (20)     2569 2023-04-12 07:25:30.000000 claspy-0.1.9/claspy/tests/nearest_neighbour_test.py
+-rw-r--r--   0 ermshaua   (501) staff       (20)     2937 2023-04-12 07:43:17.000000 claspy-0.1.9/claspy/tests/segmentation_test.py
+-rw-r--r--   0 ermshaua   (501) staff       (20)     1683 2023-02-28 15:56:43.000000 claspy-0.1.9/claspy/utils.py
+-rw-r--r--   0 ermshaua   (501) staff       (20)     2918 2023-04-03 15:59:10.000000 claspy-0.1.9/claspy/validation.py
+-rw-r--r--   0 ermshaua   (501) staff       (20)     6991 2023-02-28 19:59:17.000000 claspy-0.1.9/claspy/window_size.py
+drwxr-xr-x   0 ermshaua   (501) staff       (20)        0 2023-04-14 09:32:57.851834 claspy-0.1.9/claspy.egg-info/
+-rw-r--r--   0 ermshaua   (501) staff       (20)     6880 2023-04-14 09:32:57.000000 claspy-0.1.9/claspy.egg-info/PKG-INFO
+-rw-r--r--   0 ermshaua   (501) staff       (20)      585 2023-04-14 09:32:57.000000 claspy-0.1.9/claspy.egg-info/SOURCES.txt
+-rw-r--r--   0 ermshaua   (501) staff       (20)        1 2023-04-14 09:32:57.000000 claspy-0.1.9/claspy.egg-info/dependency_links.txt
+-rw-r--r--   0 ermshaua   (501) staff       (20)        1 2023-04-14 09:32:57.000000 claspy-0.1.9/claspy.egg-info/not-zip-safe
+-rw-r--r--   0 ermshaua   (501) staff       (20)      137 2023-04-14 09:32:57.000000 claspy-0.1.9/claspy.egg-info/requires.txt
+-rw-r--r--   0 ermshaua   (501) staff       (20)        7 2023-04-14 09:32:57.000000 claspy-0.1.9/claspy.egg-info/top_level.txt
+-rw-r--r--   0 ermshaua   (501) staff       (20)     1560 2023-04-14 09:18:45.000000 claspy-0.1.9/pyproject.toml
+-rw-r--r--   0 ermshaua   (501) staff       (20)       79 2023-04-14 09:32:57.856258 claspy-0.1.9/setup.cfg
+-rw-r--r--   0 ermshaua   (501) staff       (20)     1376 2023-04-12 07:43:17.000000 claspy-0.1.9/setup.py
```

### Comparing `claspy-0.1.8/LICENSE` & `claspy-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `claspy-0.1.8/PKG-INFO` & `claspy-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: claspy
-Version: 0.1.8
+Version: 0.1.9
 Home-page: https://github.com/ermshaua/claspy
 Author: Arik Ermshaus
 Author-email: Arik Ermshaus <ermshaua@informatik.hu-berlin.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Arik Ermshaus
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: claspy Version: 0.1.8 Home-page: https://
+Metadata-Version: 2.1 Name: claspy Version: 0.1.9 Home-page: https://
 github.com/ermshaua/claspy Author: Arik Ermshaus Author-email: Arik Ermshaus
 informatik.hu-berlin.de> License: BSD 3-Clause License Copyright (c) 2023, Arik
 Ermshaus Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met: 1.
 Redistributions of source code must retain the above copyright notice, this
 list of conditions and the following disclaimer. 2. Redistributions in binary
 form must reproduce the above copyright notice, this list of conditions and the
```

### Comparing `claspy-0.1.8/README.md` & `claspy-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `claspy-0.1.8/claspy/clasp.py` & `claspy-0.1.9/claspy/clasp.py`

 * *Files identical despite different names*

### Comparing `claspy-0.1.8/claspy/data_loader.py` & `claspy-0.1.9/claspy/data_loader.py`

 * *Files identical despite different names*

### Comparing `claspy-0.1.8/claspy/distance.py` & `claspy-0.1.9/claspy/distance.py`

 * *Files identical despite different names*

### Comparing `claspy-0.1.8/claspy/nearest_neighbour.py` & `claspy-0.1.9/claspy/nearest_neighbour.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import os
 
 import numpy as np
 import numpy.fft as fft
-from numba import njit, prange
+from numba import njit, prange, objmode
 from numba.typed.typedlist import List
 
 from claspy.distance import map_distances
 from claspy.utils import check_input_time_series
 
 
+@njit(fastmath=True, cache=True)
 def _sliding_dot(query, time_series):
     """
     Calculate sliding dot product between a query and a time series.
     The sliding dot product (SDP) is a measure of similarity between two sequences,
     which is calculated as the dot product between a query and a window of the time
     series of the same length as the query, and then shifted by one element in the
     time series at a time.
@@ -43,26 +44,27 @@
     >>> dot_product = _sliding_dot(query, time_series)
     """
     m = len(query)
     n = len(time_series)
 
     time_series_add = 0
     if n % 2 == 1:
-        time_series = np.insert(time_series, 0, 0)
+        time_series = np.concatenate((np.array([0]), time_series))
         time_series_add = 1
 
     q_add = 0
     if m % 2 == 1:
-        query = np.insert(query, 0, 0)
+        query = np.concatenate((np.array([0]), query))
         q_add = 1
 
     query = query[::-1]
-    query = np.pad(query, (0, n - m + time_series_add - q_add), "constant")
+    query = np.concatenate((query, np.zeros(n - m + time_series_add - q_add)))
     trim = m - 1 + time_series_add
-    dot_product = fft.irfft(fft.rfft(time_series) * fft.rfft(query))
+    with objmode(dot_product="float64[:]"):
+        dot_product = fft.irfft(fft.rfft(time_series) * fft.rfft(query))
     return dot_product[trim:]
 
 
 @njit(fastmath=True, cache=True)
 def _argkmin(dist, k):
     """
     Compute the indices of the k smallest elements in a numpy array.
@@ -197,15 +199,15 @@
 
         dot_prev = dot_rolled
 
     return dists, knns
 
 
 @njit(fastmath=True, cache=True, parallel=True)
-def _parallel_knn(time_series, window_size, k_neighbours, pranges, tcs, dot_firsts, distance, distance_preprocessing):
+def _parallel_knn(time_series, window_size, k_neighbours, pranges, tcs, distance, distance_preprocessing):
     """
     Perform k-nearest neighbors search between all pairs of subsequences of `time_series`
     of length `window_size` in parallel with n_jobs threads.
 
     Parameters
     ----------
     time_series : ndarray of shape (n,)
@@ -214,36 +216,39 @@
         The length of the sliding window for comparison.
     k_neighbours : int
         The number of nearest neighbors to return for each query.
     pranges : ndarray of shape (m, 2), where each row is (start, end)
         Ranges in which the k-NNs are calculated per thread. Infers the number of threads.
     tcs : ndarray of shape (m, 2), where each row is (start, end)
         Temporal constraints to consider.
-    dot_firsts : ndarray of shape (n - window_size + 1,)
-        Dot product of the first sliding window with itself.
     distance: callable
         The distance function to be computed.
     distance_preprocessing: callable
         The distance preprocessing function to be computed.
 
     Returns
     -------
     dists : ndarray of shape (l, m * k_neighbours)
         Array of distances between subsequences, sorted in increasing order.
     knns : ndarray of shape (l, m * k_neighbours)
         Array of indices of k nearest neighbors for each subsequence.
     """
+    dot_firsts = np.zeros(shape=(len(pranges), len(time_series) - window_size + 1), dtype=np.float64)
     knns = np.zeros(shape=(len(time_series) - window_size + 1, len(tcs) * k_neighbours), dtype=np.int64)
     dists = np.zeros(shape=(len(time_series) - window_size + 1, len(tcs) * k_neighbours), dtype=np.float64)
 
     for idx in prange(len(pranges)):
         start, end = pranges[idx]
+        dot_firsts[idx] = _sliding_dot(time_series[start:start + window_size], time_series)
+
+    for idx in prange(len(pranges)):
+        start, end = pranges[idx]
 
         dists[start:end, :], knns[start:end, :] = _knn(
-            time_series.copy(),
+            time_series,
             start,
             end,
             window_size,
             k_neighbours,
             tcs,
             dot_firsts[idx],
             dot_firsts[0],
@@ -359,34 +364,29 @@
         self.time_series = time_series
 
         if temporal_constraints is None:
             self.temporal_constraints = np.asarray([(0, time_series.shape[0])], dtype=np.int64)
         else:
             self.temporal_constraints = temporal_constraints
 
-        pranges, dot_firsts = List(), List()
+        pranges = List()
         n_jobs = self.n_jobs
 
         while time_series.shape[0] // n_jobs < self.window_size * self.k_neighbours and n_jobs != 1:
             n_jobs -= 1
 
         bin_size = time_series.shape[0] // n_jobs
 
         for idx in range(n_jobs):
             start = idx * bin_size
-
             end = min((idx + 1) * bin_size, len(time_series)-self.window_size+1)
-            dot_first = _sliding_dot(time_series[start:start+self.window_size], time_series)
-
-            if end > start:
-                pranges.append((start, end))
-                dot_firsts.append(dot_first)
+            if end > start: pranges.append((start, end))
 
         self.distances, self.offsets = _parallel_knn(time_series, self.window_size, self.k_neighbours,
-                                                     pranges, List(self.temporal_constraints), dot_firsts,
+                                                     pranges, List(self.temporal_constraints),
                                                      self.distance, self.distance_preprocessing)
 
         return self
 
     def constrain(self, lbound, ubound):
         """
         Constrain the k-nearest neighbours search to a specific range.
```

### Comparing `claspy-0.1.8/claspy/scoring.py` & `claspy-0.1.9/claspy/scoring.py`

 * *Files identical despite different names*

### Comparing `claspy-0.1.8/claspy/segmentation.py` & `claspy-0.1.9/claspy/segmentation.py`

 * *Files identical despite different names*

### Comparing `claspy-0.1.8/claspy/tests/clasp_test.py` & `claspy-0.1.9/claspy/tests/clasp_test.py`

 * *Files identical despite different names*

### Comparing `claspy-0.1.8/claspy/tests/evaluation.py` & `claspy-0.1.9/claspy/tests/evaluation.py`

 * *Files identical despite different names*

### Comparing `claspy-0.1.8/claspy/tests/nearest_neighbour_test.py` & `claspy-0.1.9/claspy/tests/nearest_neighbour_test.py`

 * *Files identical despite different names*

### Comparing `claspy-0.1.8/claspy/tests/segmentation_test.py` & `claspy-0.1.9/claspy/tests/segmentation_test.py`

 * *Files identical despite different names*

### Comparing `claspy-0.1.8/claspy/utils.py` & `claspy-0.1.9/claspy/utils.py`

 * *Files identical despite different names*

### Comparing `claspy-0.1.8/claspy/validation.py` & `claspy-0.1.9/claspy/validation.py`

 * *Files identical despite different names*

### Comparing `claspy-0.1.8/claspy/window_size.py` & `claspy-0.1.9/claspy/window_size.py`

 * *Files identical despite different names*

### Comparing `claspy-0.1.8/claspy.egg-info/PKG-INFO` & `claspy-0.1.9/claspy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: claspy
-Version: 0.1.8
+Version: 0.1.9
 Home-page: https://github.com/ermshaua/claspy
 Author: Arik Ermshaus
 Author-email: Arik Ermshaus <ermshaua@informatik.hu-berlin.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Arik Ermshaus
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: claspy Version: 0.1.8 Home-page: https://
+Metadata-Version: 2.1 Name: claspy Version: 0.1.9 Home-page: https://
 github.com/ermshaua/claspy Author: Arik Ermshaus Author-email: Arik Ermshaus
 informatik.hu-berlin.de> License: BSD 3-Clause License Copyright (c) 2023, Arik
 Ermshaus Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met: 1.
 Redistributions of source code must retain the above copyright notice, this
 list of conditions and the following disclaimer. 2. Redistributions in binary
 form must reproduce the above copyright notice, this list of conditions and the
```

### Comparing `claspy-0.1.8/claspy.egg-info/SOURCES.txt` & `claspy-0.1.9/claspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `claspy-0.1.8/pyproject.toml` & `claspy-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "claspy"
 
-version = "0.1.8"
+version = "0.1.9"
 
 description = ""
 readme = "README.md"
 authors = [
     {name = "Arik Ermshaus", email = "ermshaua@informatik.hu-berlin.de"}
 ]
 keywords = [
```

### Comparing `claspy-0.1.8/setup.py` & `claspy-0.1.9/setup.py`

 * *Files identical despite different names*

