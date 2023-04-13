# Comparing `tmp/PyDesmos-0.1.1.tar.gz` & `tmp/PyDesmos-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyDesmos-0.1.1.tar", last modified: Thu Apr 13 18:58:02 2023, max compression
+gzip compressed data, was "PyDesmos-0.1.2.tar", last modified: Thu Apr 13 23:27:24 2023, max compression
```

## Comparing `PyDesmos-0.1.1.tar` & `PyDesmos-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 18:58:02.366411 PyDesmos-0.1.1/
--rw-rw-rw-   0        0        0      306 2023-04-13 18:57:15.000000 PyDesmos-0.1.1/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1064 2023-04-10 19:18:21.000000 PyDesmos-0.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0       30 2023-04-13 09:32:41.000000 PyDesmos-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3693 2023-04-13 18:58:02.366411 PyDesmos-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-13 18:58:02.345466 PyDesmos-0.1.1/PyDesmos/
--rw-rw-rw-   0        0        0     9245 2023-04-13 18:57:37.000000 PyDesmos-0.1.1/PyDesmos/__init__.py
--rw-rw-rw-   0        0        0     5310 2023-04-13 02:09:44.000000 PyDesmos-0.1.1/PyDesmos/logo.png
-drwxrwxrwx   0        0        0        0 2023-04-13 18:58:02.364416 PyDesmos-0.1.1/PyDesmos.egg-info/
--rw-rw-rw-   0        0        0     3693 2023-04-13 18:58:02.000000 PyDesmos-0.1.1/PyDesmos.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2023-04-13 18:58:02.000000 PyDesmos-0.1.1/PyDesmos.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 18:58:02.000000 PyDesmos-0.1.1/PyDesmos.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-13 18:58:02.000000 PyDesmos-0.1.1/PyDesmos.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-13 18:58:02.000000 PyDesmos-0.1.1/PyDesmos.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2770 2023-04-13 09:59:00.000000 PyDesmos-0.1.1/README.md
--rw-rw-rw-   0        0        0     5310 2023-04-13 02:09:44.000000 PyDesmos-0.1.1/logo.png
--rw-rw-rw-   0        0        0       42 2023-04-13 18:58:02.367408 PyDesmos-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      869 2023-04-13 18:55:12.000000 PyDesmos-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-13 23:27:24.729995 PyDesmos-0.1.2/
+-rw-rw-rw-   0        0        0      421 2023-04-13 23:21:23.000000 PyDesmos-0.1.2/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1064 2023-04-10 19:18:21.000000 PyDesmos-0.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       30 2023-04-13 09:32:41.000000 PyDesmos-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     4073 2023-04-13 23:27:24.728000 PyDesmos-0.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-13 23:27:24.704064 PyDesmos-0.1.2/PyDesmos/
+-rw-rw-rw-   0        0        0    12867 2023-04-13 23:26:30.000000 PyDesmos-0.1.2/PyDesmos/__init__.py
+-rw-rw-rw-   0        0        0     5310 2023-04-13 02:09:44.000000 PyDesmos-0.1.2/PyDesmos/logo.png
+drwxrwxrwx   0        0        0        0 2023-04-13 23:27:24.725008 PyDesmos-0.1.2/PyDesmos.egg-info/
+-rw-rw-rw-   0        0        0     4073 2023-04-13 23:27:24.000000 PyDesmos-0.1.2/PyDesmos.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2023-04-13 23:27:24.000000 PyDesmos-0.1.2/PyDesmos.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 23:27:24.000000 PyDesmos-0.1.2/PyDesmos.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-13 23:27:24.000000 PyDesmos-0.1.2/PyDesmos.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-13 23:27:24.000000 PyDesmos-0.1.2/PyDesmos.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3010 2023-04-13 23:21:15.000000 PyDesmos-0.1.2/README.md
+-rw-rw-rw-   0        0        0     5310 2023-04-13 02:09:44.000000 PyDesmos-0.1.2/logo.png
+-rw-rw-rw-   0        0        0       42 2023-04-13 23:27:24.730992 PyDesmos-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      909 2023-04-13 23:26:50.000000 PyDesmos-0.1.2/setup.py
```

### Comparing `PyDesmos-0.1.1/LICENSE.txt` & `PyDesmos-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyDesmos-0.1.1/PKG-INFO` & `PyDesmos-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PyDesmos
-Version: 0.1.1
-Summary: An easy-to-use Python to Desmos graph HTML compiler via the Desmos API.
+Version: 0.1.2
+Summary: An easy-to-use Python to Desmos graph HTML compiler via the Desmos API (with OEIS support).
 Home-page: 
 Author: Lyam Boylan
 Author-email: lyamboylan@gmail.com
 License: MIT
-Keywords: math,graph,desmos,graphing software,html,sympy,api
+Keywords: math,graph,desmos,graphing software,html,sympy,api,oeis
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
@@ -86,14 +86,25 @@
 Alright, I'm sure you get it. PyDesmos is awesome. But one last thing. All of these methods have additional (optional) kwargs for absolute customization, such as color, line thickness, etc.
 You may read about them [here](https://www.desmos.com/api/v1.7/docs/index.html#document-manipulating-expressions), under "expression_state Name and Values". For example,
 ```python
 G(y=G.x ** 2, color='#FF0000')  # appends the expression "y=x^2" with color #FF0000.
 ```
 Happy PyDesmos-ing!
 
+---
+
+**New:** To plot a sequence from the [OEIS](https://oeis.org/):
+```python
+G.plot_oeis('A000001')  # optional max_terms parameter
+```
+Or to just get a dictionary:
+```python
+A000001 = oeis('A000001')  # {0: 0, 1: 1, ...}
+```
+
 Change Log
 ==========
 
 0.0.1 (12/04/2023)
 -------------------
 - First Release
 
@@ -103,7 +114,12 @@
 - Major code revisions
 - improved README.md
 
 0.1.1 (13/04/2023)
 -------------------
 - Minor tweaks (mostly to README.md)
 - Fixed optional kwargs with tables
+
+0.1.2 (13/04/2023)
+-------------------
+- Added simple OEIS integration
+- Added support for all greek letters
```

### Comparing `PyDesmos-0.1.1/PyDesmos/__init__.py` & `PyDesmos-0.1.2/PyDesmos/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,95 @@
 import types
 import webbrowser
 from sympy import *
 import math
-
+import requests
 
 desmos_symbols = {chr(i): chr(i) for i in range(65, 91)}
 desmos_symbols.update({chr(i): chr(i) for i in range(97, 123)})
 desmos_symbols.update({
     'alpha': r'\alpha',
+    'nu': r'\nu',
     'beta': r'\beta',
+    'xi': r'\xi',
+    'Xi': r'\Xi',
+    'gamma': r'\gamma',
+    'Gamma': r'\Gamma',
+    'delta': r'\delta',
     'Delta': r'\Delta',
+    'pi': r'\pi',
+    'Pi': r'\Pi',
+    'epsilon': r'\epsilon',
+    'varepsilon': r'\varepsilon',
+    'rho': r'\rho',
+    'varrho': r'\varrho',
+    'zeta': r'\zeta',
+    'sigma': r'\sigma',
+    'Sigma': r'\Sigma',
+    'eta': r'\eta',
+    'tau': r'\tau',
     'theta': r'\theta',
+    'vartheta': r'\vartheta',
+    'Theta': r'\Theta',
+    'upsilon': r'\upsilon',
+    'Upsilon': r'\Upsilon',
+    'iota': r'\iota',
     'phi': r'\phi',
-    'pi': r'\pi',
+    'varphi': r'\varphi',
+    'Phi': r'\Phi',
+    'kappa': r'\kappa',
+    'chi': r'\chi',
+    'lambda': r'\lambda',
+    'psi': r'\psi',
+    'Psi': r'\Psi',
+    'mu': r'\mu',
+    'omega': r'\omega',
+    'Omega': r'\Omega',
     'ln': r'\ln',
 })
 
 
+def oeis(sequence, max_terms=None):
+    sequence = str(sequence)
+    if sequence.startswith('A'):
+        sequence = sequence[1:]
+    sequence = sequence.zfill(6)
+
+    raw = requests.get(f'https://oeis.org/A{sequence}/b{sequence}.txt').text
+
+    if 'Sorry, the page you requested was not found' in raw:
+        raise ValueError('Sorry, the page you requested was not found')
+
+    def parse_raw(text):
+        entries = {}
+        for line in text.split('\n'):
+            # print(line)
+            index, value = None, None
+            digits = ''
+            for character in line + ' ':
+                if character in '0123456789-':
+                    digits += character
+                elif character in '#':
+                    break
+                elif digits:
+                    if index is None:
+                        index = int(digits)
+                        digits = ''
+                    else:
+                        value = int(digits)
+                        break
+            if value is not None:
+                entries[index] = value
+                if max_terms and len(entries) >= max_terms:
+                    break
+        return entries
+
+    return parse_raw(raw)
+
+
 class Variable(Symbol):
     """extension of the sympy Symbol class to allow for quick and dirty interaction with the desmos graph"""
     def __new__(cls, symbol, graph):
         obj = Symbol.__new__(cls, symbol)
         obj.graph = graph
         return obj
 
@@ -101,17 +170,31 @@
         self.e, self.f, self.g = Variable('e', self), Variable('f', self), Variable('g', self)
         self.h, self.i, self.j = Variable('h', self), Variable('i', self), Variable('j', self)
         self.k, self.l, self.m = Variable('k', self), Variable('l', self), Variable('m', self)
         self.n, self.o, self.p = Variable('n', self), Variable('o', self), Variable('p', self)
         self.q, self.r, self.s = Variable('q', self), Variable('r', self), Variable('s', self)
         self.t, self.u, self.v = Variable('t', self), Variable('u', self), Variable('v', self)
         self.w, self.x, self.y = Variable('w', self), Variable('x', self), Variable('y', self)
-        self.z, self.alpha, self.beta = Variable('z', self), Variable(r'\alpha', self), Variable(r'\beta', self)
-        self.Delta, self.theta, self.phi = Variable(r'\Delta', self), Variable(r'\theta', self), Variable(r'\phi', self)
-        self.pi, self.ln = Variable(r'\pi', self), Variable(r'\ln', self)
+        self.z = Variable('z', self)
+        self.alpha, self.nu, self.beta = Variable(r'\alpha', self), Variable(r'\nu', self), Variable(r'\beta', self)
+        self.xi, self.Xi, self.gamma = Variable(r'\xi', self), Variable(r'\Xi', self), Variable(r'\gamma', self)
+        self.Gamma, self.delta = Variable(r'\Gamma', self), Variable(r'\delta', self)
+        self.Delta, self.pi, self.Pi = Variable(r'\Delta', self), Variable(r'\pi', self), Variable(r'\Pi', self)
+        self.epsilon, self.varepsilon = Variable(r'\epsilon', self), Variable(r'\varepsilon', self)
+        self.rho, self.varrho = Variable(r'\rho', self), Variable(r'\varrho', self)
+        self.zeta, self.sigma = Variable(r'\zeta', self), Variable(r'\sigma', self)
+        self.Sigma, self.eta, self.tau = Variable(r'\Sigma', self), Variable(r'\eta', self), Variable(r'\tau', self)
+        self.theta, self.vartheta = Variable(r'\theta', self), Variable(r'\vartheta', self)
+        self.Theta, self.upsilon = Variable(r'\Theta', self), Variable(r'\upsilon', self)
+        self.Upsilon, self.iota = Variable(r'\Upsilon', self), Variable(r'\iota', self)
+        self.phi, self.varphi, self.Phi = Variable(r'\phi', self), Variable(r'\varphi', self), Variable(r'\Phi', self)
+        self.kappa, self.chi = Variable(r'\kappa', self), Variable(r'\chi', self)
+        self.lambda_, self.psi, self.Psi = Variable(r'\lambda', self), Variable(r'\psi', self), Variable(r'\Psi', self)
+        self.mu, self.omega, self.Omega = Variable(r'\mu', self), Variable(r'\omega', self), Variable(r'\Omega', self)
+        self.ln = Variable(r'\ln', self)
 
     def set_expression(self, **kwargs):
         """based on desmos api v1.7"""
         if 'id' not in kwargs:
             kwargs['id'] = str(self.expression_count)
             self.expression_count += 1
         self.html += f'\tcalculator.setExpression({parse_dict(kwargs, 1)});\n'
@@ -199,9 +282,14 @@
 
     def plot_function(self, function, min, max, step=1, independent_variable='x', dependent_variable='y', **kwargs):
         N = math.ceil((max - min) / step)
         X = [min + step * n for n in range(int(N))]
         Y = [function(x) for x in X]
         self.new_table({independent_variable: X, dependent_variable: Y}, **kwargs)
 
+    def plot_oeis(self, sequence, max_terms=None, **kwargs):
+        n, A = zip(*oeis(sequence, max_terms).items())
+        sequence = int(sequence[int(sequence.startswith('A')):]) if isinstance(sequence, str) else sequence
+        self.new_table({'n_{%d}' % sequence: n, 'A_{%d}' % sequence: A}, **kwargs)
+
     def __or__(self, other):
-        self.__call__(other)
+        self.__call__(other)
```

### Comparing `PyDesmos-0.1.1/PyDesmos/logo.png` & `PyDesmos-0.1.2/PyDesmos/logo.png`

 * *Files identical despite different names*

### Comparing `PyDesmos-0.1.1/PyDesmos.egg-info/PKG-INFO` & `PyDesmos-0.1.2/PyDesmos.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PyDesmos
-Version: 0.1.1
-Summary: An easy-to-use Python to Desmos graph HTML compiler via the Desmos API.
+Version: 0.1.2
+Summary: An easy-to-use Python to Desmos graph HTML compiler via the Desmos API (with OEIS support).
 Home-page: 
 Author: Lyam Boylan
 Author-email: lyamboylan@gmail.com
 License: MIT
-Keywords: math,graph,desmos,graphing software,html,sympy,api
+Keywords: math,graph,desmos,graphing software,html,sympy,api,oeis
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
@@ -86,14 +86,25 @@
 Alright, I'm sure you get it. PyDesmos is awesome. But one last thing. All of these methods have additional (optional) kwargs for absolute customization, such as color, line thickness, etc.
 You may read about them [here](https://www.desmos.com/api/v1.7/docs/index.html#document-manipulating-expressions), under "expression_state Name and Values". For example,
 ```python
 G(y=G.x ** 2, color='#FF0000')  # appends the expression "y=x^2" with color #FF0000.
 ```
 Happy PyDesmos-ing!
 
+---
+
+**New:** To plot a sequence from the [OEIS](https://oeis.org/):
+```python
+G.plot_oeis('A000001')  # optional max_terms parameter
+```
+Or to just get a dictionary:
+```python
+A000001 = oeis('A000001')  # {0: 0, 1: 1, ...}
+```
+
 Change Log
 ==========
 
 0.0.1 (12/04/2023)
 -------------------
 - First Release
 
@@ -103,7 +114,12 @@
 - Major code revisions
 - improved README.md
 
 0.1.1 (13/04/2023)
 -------------------
 - Minor tweaks (mostly to README.md)
 - Fixed optional kwargs with tables
+
+0.1.2 (13/04/2023)
+-------------------
+- Added simple OEIS integration
+- Added support for all greek letters
```

### Comparing `PyDesmos-0.1.1/README.md` & `PyDesmos-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -67,8 +67,19 @@
 ...
 
 Alright, I'm sure you get it. PyDesmos is awesome. But one last thing. All of these methods have additional (optional) kwargs for absolute customization, such as color, line thickness, etc.
 You may read about them [here](https://www.desmos.com/api/v1.7/docs/index.html#document-manipulating-expressions), under "expression_state Name and Values". For example,
 ```python
 G(y=G.x ** 2, color='#FF0000')  # appends the expression "y=x^2" with color #FF0000.
 ```
-Happy PyDesmos-ing!
+Happy PyDesmos-ing!
+
+---
+
+**New:** To plot a sequence from the [OEIS](https://oeis.org/):
+```python
+G.plot_oeis('A000001')  # optional max_terms parameter
+```
+Or to just get a dictionary:
+```python
+A000001 = oeis('A000001')  # {0: 0, 1: 1, ...}
+```
```

### Comparing `PyDesmos-0.1.1/logo.png` & `PyDesmos-0.1.2/logo.png`

 * *Files identical despite different names*

### Comparing `PyDesmos-0.1.1/setup.py` & `PyDesmos-0.1.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,20 +6,20 @@
     'Operating System :: Microsoft :: Windows :: Windows 10',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name='PyDesmos',
-    version='0.1.1',
-    description='An easy-to-use Python to Desmos graph HTML compiler via the Desmos API.',
+    version='0.1.2',
+    description='An easy-to-use Python to Desmos graph HTML compiler via the Desmos API (with OEIS support).',
     long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
     long_description_content_type='text/markdown',
     url='',
     author='Lyam Boylan',
     author_email='lyamboylan@gmail.com',
     license='MIT',
-    keywords=['math', 'graph', 'desmos', 'graphing software', 'html', 'sympy', 'api'],
+    keywords=['math', 'graph', 'desmos', 'graphing software', 'html', 'sympy', 'api', 'oeis'],
     classifiers=classifiers,
     packages=find_packages(),
-    install_requires=['sympy']
+    install_requires=['sympy', 'requests']
 )
```

