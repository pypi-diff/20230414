# Comparing `tmp/PyDesmos-0.1.2.tar.gz` & `tmp/PyDesmos-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyDesmos-0.1.2.tar", last modified: Thu Apr 13 23:27:24 2023, max compression
+gzip compressed data, was "PyDesmos-0.1.3.tar", last modified: Fri Apr 14 00:36:15 2023, max compression
```

## Comparing `PyDesmos-0.1.2.tar` & `PyDesmos-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 23:27:24.729995 PyDesmos-0.1.2/
--rw-rw-rw-   0        0        0      421 2023-04-13 23:21:23.000000 PyDesmos-0.1.2/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1064 2023-04-10 19:18:21.000000 PyDesmos-0.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0       30 2023-04-13 09:32:41.000000 PyDesmos-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     4073 2023-04-13 23:27:24.728000 PyDesmos-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-13 23:27:24.704064 PyDesmos-0.1.2/PyDesmos/
--rw-rw-rw-   0        0        0    12867 2023-04-13 23:26:30.000000 PyDesmos-0.1.2/PyDesmos/__init__.py
--rw-rw-rw-   0        0        0     5310 2023-04-13 02:09:44.000000 PyDesmos-0.1.2/PyDesmos/logo.png
-drwxrwxrwx   0        0        0        0 2023-04-13 23:27:24.725008 PyDesmos-0.1.2/PyDesmos.egg-info/
--rw-rw-rw-   0        0        0     4073 2023-04-13 23:27:24.000000 PyDesmos-0.1.2/PyDesmos.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2023-04-13 23:27:24.000000 PyDesmos-0.1.2/PyDesmos.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 23:27:24.000000 PyDesmos-0.1.2/PyDesmos.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-13 23:27:24.000000 PyDesmos-0.1.2/PyDesmos.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-13 23:27:24.000000 PyDesmos-0.1.2/PyDesmos.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3010 2023-04-13 23:21:15.000000 PyDesmos-0.1.2/README.md
--rw-rw-rw-   0        0        0     5310 2023-04-13 02:09:44.000000 PyDesmos-0.1.2/logo.png
--rw-rw-rw-   0        0        0       42 2023-04-13 23:27:24.730992 PyDesmos-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      909 2023-04-13 23:26:50.000000 PyDesmos-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 00:36:15.233097 PyDesmos-0.1.3/
+-rw-rw-rw-   0        0        0      579 2023-04-14 00:35:43.000000 PyDesmos-0.1.3/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1064 2023-04-10 19:18:21.000000 PyDesmos-0.1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0       30 2023-04-13 09:32:41.000000 PyDesmos-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     4479 2023-04-14 00:36:15.232100 PyDesmos-0.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-14 00:36:15.213151 PyDesmos-0.1.3/PyDesmos/
+-rw-rw-rw-   0        0        0    14079 2023-04-14 00:30:14.000000 PyDesmos-0.1.3/PyDesmos/__init__.py
+-rw-rw-rw-   0        0        0     5310 2023-04-13 02:09:44.000000 PyDesmos-0.1.3/PyDesmos/logo.png
+drwxrwxrwx   0        0        0        0 2023-04-14 00:36:15.231103 PyDesmos-0.1.3/PyDesmos.egg-info/
+-rw-rw-rw-   0        0        0     4479 2023-04-14 00:36:15.000000 PyDesmos-0.1.3/PyDesmos.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2023-04-14 00:36:15.000000 PyDesmos-0.1.3/PyDesmos.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 00:36:15.000000 PyDesmos-0.1.3/PyDesmos.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-14 00:36:15.000000 PyDesmos-0.1.3/PyDesmos.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-14 00:36:15.000000 PyDesmos-0.1.3/PyDesmos.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3258 2023-04-14 00:34:57.000000 PyDesmos-0.1.3/README.md
+-rw-rw-rw-   0        0        0     5310 2023-04-13 02:09:44.000000 PyDesmos-0.1.3/logo.png
+-rw-rw-rw-   0        0        0       42 2023-04-14 00:36:15.233097 PyDesmos-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      909 2023-04-14 00:35:01.000000 PyDesmos-0.1.3/setup.py
```

### Comparing `PyDesmos-0.1.2/LICENSE.txt` & `PyDesmos-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyDesmos-0.1.2/PKG-INFO` & `PyDesmos-0.1.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyDesmos
-Version: 0.1.2
+Version: 0.1.3
 Summary: An easy-to-use Python to Desmos graph HTML compiler via the Desmos API (with OEIS support).
 Home-page: 
 Author: Lyam Boylan
 Author-email: lyamboylan@gmail.com
 License: MIT
 Keywords: math,graph,desmos,graphing software,html,sympy,api,oeis
 Classifier: Development Status :: 3 - Alpha
@@ -94,15 +94,24 @@
 
 **New:** To plot a sequence from the [OEIS](https://oeis.org/):
 ```python
 G.plot_oeis('A000001')  # optional max_terms parameter
 ```
 Or to just get a dictionary:
 ```python
-A000001 = oeis('A000001')  # {0: 0, 1: 1, ...}
+A000001 = oeis('A000001')  # returns {0: 0, 1: 1, ...}
+```
+Query support:
+```python
+G.plot_oeis('the prime numbers')  # OR
+G.plot_oeis([2, 3, 5, 7])
+```
+Related method with the OEIS
+```python
+oeis_query('the prime numbers')  # returns a list of the first few most relevant sequence ids
 ```
 
 Change Log
 ==========
 
 0.0.1 (12/04/2023)
 -------------------
@@ -119,7 +128,11 @@
 - Minor tweaks (mostly to README.md)
 - Fixed optional kwargs with tables
 
 0.1.2 (13/04/2023)
 -------------------
 - Added simple OEIS integration
 - Added support for all greek letters
+
+0.1.3 (13/04/2023)
+-------------------
+- Increased OEIS support. (allows for querying the most relevant sequences based off a list of terms or keywords)
```

### Comparing `PyDesmos-0.1.2/PyDesmos/__init__.py` & `PyDesmos-0.1.3/PyDesmos/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,21 +44,54 @@
     'mu': r'\mu',
     'omega': r'\omega',
     'Omega': r'\Omega',
     'ln': r'\ln',
 })
 
 
-def oeis(sequence, max_terms=None):
-    sequence = str(sequence)
+def oeis_query(query):
+    """returns a list of of the first OEIS sequence ids sorted by their relevance to the query"""
+    query_text = ','.join(str(int(x)) for x in query) if isinstance(query, list) else repr(query)
+    url = f'https://oeis.org/search?q={query_text}'
+    raw = requests.get(url).text
+    if 'Sorry, but the terms do not match anything in the table' in raw:
+        raise ValueError('Sorry, but the terms do not match anything in the table')
+    prefix = '/search?q=id:'
+    sequences = []
+    while prefix in raw:
+        raw = raw[raw.index(prefix) + len(prefix):]
+        sequence = raw[:7]
+        sequences.append(sequence)
+    return sequences
+
+
+def oeis_sequence_id(value):
+    """returns the most relevant valid OEIS sequence id from the given value"""
+    def is_query(value):
+        if isinstance(value, list):
+            return True
+        if isinstance(value, str):
+            return not value.isdigit() and not (value.startswith('A') and value[1:].isdigit())
+
+    if is_query(value):
+        return oeis_query(value)[0]
+
+    sequence = str(value)
     if sequence.startswith('A'):
         sequence = sequence[1:]
-    sequence = sequence.zfill(6)
 
-    raw = requests.get(f'https://oeis.org/A{sequence}/b{sequence}.txt').text
+    return 'A' + sequence.zfill(6)
+
+
+def oeis(sequence, max_terms=None):
+    """returns a dictionary based on the most relevant OEIS sequence given by the input sequence"""
+
+    sequence_id = oeis_sequence_id(sequence)[1:]
+
+    raw = requests.get(f'https://oeis.org/A{sequence_id}/b{sequence_id}.txt').text
 
     if 'Sorry, the page you requested was not found' in raw:
         raise ValueError('Sorry, the page you requested was not found')
 
     def parse_raw(text):
         entries = {}
         for line in text.split('\n'):
@@ -283,13 +316,13 @@
     def plot_function(self, function, min, max, step=1, independent_variable='x', dependent_variable='y', **kwargs):
         N = math.ceil((max - min) / step)
         X = [min + step * n for n in range(int(N))]
         Y = [function(x) for x in X]
         self.new_table({independent_variable: X, dependent_variable: Y}, **kwargs)
 
     def plot_oeis(self, sequence, max_terms=None, **kwargs):
-        n, A = zip(*oeis(sequence, max_terms).items())
-        sequence = int(sequence[int(sequence.startswith('A')):]) if isinstance(sequence, str) else sequence
-        self.new_table({'n_{%d}' % sequence: n, 'A_{%d}' % sequence: A}, **kwargs)
+        sequence_id = oeis_sequence_id(sequence)[1:]
+        n, A = zip(*oeis(sequence_id, max_terms).items())
+        self.new_table({'n_{%d}' % int(sequence_id): n, 'A_{%d}' % int(sequence_id): A}, **kwargs)
 
     def __or__(self, other):
         self.__call__(other)
```

### Comparing `PyDesmos-0.1.2/PyDesmos/logo.png` & `PyDesmos-0.1.3/PyDesmos/logo.png`

 * *Files identical despite different names*

### Comparing `PyDesmos-0.1.2/PyDesmos.egg-info/PKG-INFO` & `PyDesmos-0.1.3/PyDesmos.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyDesmos
-Version: 0.1.2
+Version: 0.1.3
 Summary: An easy-to-use Python to Desmos graph HTML compiler via the Desmos API (with OEIS support).
 Home-page: 
 Author: Lyam Boylan
 Author-email: lyamboylan@gmail.com
 License: MIT
 Keywords: math,graph,desmos,graphing software,html,sympy,api,oeis
 Classifier: Development Status :: 3 - Alpha
@@ -94,15 +94,24 @@
 
 **New:** To plot a sequence from the [OEIS](https://oeis.org/):
 ```python
 G.plot_oeis('A000001')  # optional max_terms parameter
 ```
 Or to just get a dictionary:
 ```python
-A000001 = oeis('A000001')  # {0: 0, 1: 1, ...}
+A000001 = oeis('A000001')  # returns {0: 0, 1: 1, ...}
+```
+Query support:
+```python
+G.plot_oeis('the prime numbers')  # OR
+G.plot_oeis([2, 3, 5, 7])
+```
+Related method with the OEIS
+```python
+oeis_query('the prime numbers')  # returns a list of the first few most relevant sequence ids
 ```
 
 Change Log
 ==========
 
 0.0.1 (12/04/2023)
 -------------------
@@ -119,7 +128,11 @@
 - Minor tweaks (mostly to README.md)
 - Fixed optional kwargs with tables
 
 0.1.2 (13/04/2023)
 -------------------
 - Added simple OEIS integration
 - Added support for all greek letters
+
+0.1.3 (13/04/2023)
+-------------------
+- Increased OEIS support. (allows for querying the most relevant sequences based off a list of terms or keywords)
```

### Comparing `PyDesmos-0.1.2/README.md` & `PyDesmos-0.1.3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -77,9 +77,18 @@
 
 **New:** To plot a sequence from the [OEIS](https://oeis.org/):
 ```python
 G.plot_oeis('A000001')  # optional max_terms parameter
 ```
 Or to just get a dictionary:
 ```python
-A000001 = oeis('A000001')  # {0: 0, 1: 1, ...}
+A000001 = oeis('A000001')  # returns {0: 0, 1: 1, ...}
+```
+Query support:
+```python
+G.plot_oeis('the prime numbers')  # OR
+G.plot_oeis([2, 3, 5, 7])
+```
+Related method with the OEIS
+```python
+oeis_query('the prime numbers')  # returns a list of the first few most relevant sequence ids
 ```
```

### Comparing `PyDesmos-0.1.2/logo.png` & `PyDesmos-0.1.3/logo.png`

 * *Files identical despite different names*

### Comparing `PyDesmos-0.1.2/setup.py` & `PyDesmos-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'Operating System :: Microsoft :: Windows :: Windows 10',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='PyDesmos',
-    version='0.1.2',
+    version='0.1.3',
     description='An easy-to-use Python to Desmos graph HTML compiler via the Desmos API (with OEIS support).',
     long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
     long_description_content_type='text/markdown',
     url='',
     author='Lyam Boylan',
     author_email='lyamboylan@gmail.com',
     license='MIT',
```

