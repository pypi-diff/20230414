# Comparing `tmp/pipen_annotate-0.6.3.tar.gz` & `tmp/pipen_annotate-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipen_annotate-0.6.3.tar", max compression
+gzip compressed data, was "pipen_annotate-0.7.0.tar", max compression
```

## Comparing `pipen_annotate-0.6.3.tar` & `pipen_annotate-0.7.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1063 2023-04-10 21:40:06.361035 pipen_annotate-0.6.3/LICENSE
--rw-r--r--   0        0        0     1592 2023-04-10 21:40:06.361035 pipen_annotate-0.6.3/README.md
--rw-r--r--   0        0        0      108 2023-04-10 21:40:06.361035 pipen_annotate-0.6.3/pipen_annotate/__init__.py
--rw-r--r--   0        0        0     5804 2023-04-10 21:40:06.361035 pipen_annotate-0.6.3/pipen_annotate/annotate.py
--rw-r--r--   0        0        0    10938 2023-04-10 21:40:06.361035 pipen_annotate-0.6.3/pipen_annotate/sections.py
--rw-r--r--   0        0        0      960 2023-04-10 21:40:06.361035 pipen_annotate-0.6.3/pyproject.toml
--rw-r--r--   0        0        0     2377 1970-01-01 00:00:00.000000 pipen_annotate-0.6.3/setup.py
--rw-r--r--   0        0        0     2170 1970-01-01 00:00:00.000000 pipen_annotate-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-04-14 02:11:01.246979 pipen_annotate-0.7.0/LICENSE
+-rw-r--r--   0        0        0     1592 2023-04-14 02:11:01.246979 pipen_annotate-0.7.0/README.md
+-rw-r--r--   0        0        0      108 2023-04-14 02:11:01.246979 pipen_annotate-0.7.0/pipen_annotate/__init__.py
+-rw-r--r--   0        0        0     5804 2023-04-14 02:11:01.246979 pipen_annotate-0.7.0/pipen_annotate/annotate.py
+-rw-r--r--   0        0        0    10938 2023-04-14 02:11:01.246979 pipen_annotate-0.7.0/pipen_annotate/sections.py
+-rw-r--r--   0        0        0      958 2023-04-14 02:11:01.246979 pipen_annotate-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     2374 1970-01-01 00:00:00.000000 pipen_annotate-0.7.0/setup.py
+-rw-r--r--   0        0        0     2167 1970-01-01 00:00:00.000000 pipen_annotate-0.7.0/PKG-INFO
```

### Comparing `pipen_annotate-0.6.3/LICENSE` & `pipen_annotate-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pipen_annotate-0.6.3/README.md` & `pipen_annotate-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pipen_annotate-0.6.3/pipen_annotate/annotate.py` & `pipen_annotate-0.7.0/pipen_annotate/annotate.py`

 * *Files identical despite different names*

### Comparing `pipen_annotate-0.6.3/pipen_annotate/sections.py` & `pipen_annotate-0.7.0/pipen_annotate/sections.py`

 * *Files identical despite different names*

### Comparing `pipen_annotate-0.6.3/pyproject.toml` & `pipen_annotate-0.7.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "pipen-annotate"
-version = "0.6.3"
+version = "0.7.0"
 description = "Use docstring to annotate pipen processes"
 authors = ["pwwang <pwwang@pwwang.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.build]
 generate-setup-file = true
 
 [tool.poetry.dependencies]
-python = "^3.7.1"
-pipen = "^0.7"
+python = "^3.8"
+pipen = "^0.9"
 # diot required by xqute that's required by pipen
 
 [tool.poetry.dev-dependencies]
 pytest = "^7"
 pytest-cov = "^4"
 
 [build-system]
```

### Comparing `pipen_annotate-0.6.3/setup.py` & `pipen_annotate-0.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 packages = \
 ['pipen_annotate']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['pipen>=0.7,<0.8']
+['pipen>=0.9,<0.10']
 
 setup_kwargs = {
     'name': 'pipen-annotate',
-    'version': '0.6.3',
+    'version': '0.7.0',
     'description': 'Use docstring to annotate pipen processes',
     'long_description': '# pipen-annotate\n\nUse docstring to annotate [pipen](https://github.com/pwwang/pipen) processes\n\n## Installation\n\n```shell\npip install -U pipen-annotate\n```\n\n## Usage\n\n```python\nfrom pprint import pprint\nfrom pipen import Proc\nfrom pipen_annotate import annotate\n\n\nclass Process(Proc):\n    """Short description\n\n    Long description\n\n    Input:\n        infile: An input file\n        invar: An input variable\n\n    Output:\n        outfile: The output file\n\n    Envs:\n        ncores: Number of cores\n    """\n    input = "infile:file, invar"\n    output = "outfile:file:output.txt"\n    args = {\'ncores\': 1}\n\nannotated = annotate(Process)\n# prints:\n{\'Envs\': {\'ncores\': {\'attrs\': OrderedDiot([(\'default\', 1)]),\n                     \'help\': \'Number of cores\',\n                     \'terms\': OrderedDiot([])}},\n \'Input\': {\'infile\': {\'attrs\': {\'action\': \'extend\',\n                                \'itype\': \'file\',\n                                \'nargs\': \'+\'},\n                      \'help\': \'An input file\',\n                      \'terms\': OrderedDiot([])},\n           \'invar\': {\'attrs\': {\'action\': \'extend\',\n                               \'itype\': \'var\',\n                               \'nargs\': \'+\'},\n                     \'help\': \'An input variable\',\n                     \'terms\': OrderedDiot([])}},\n \'Output\': {\'outfile\': {\'attrs\': {\'default\': \'output.txt\',\n                                  \'otype\': \'file\'},\n                        \'help\': \'The output file\',\n                        \'terms\': OrderedDiot([])}},\n \'Summary\': {\'long\': \'Long description\\n\',\n             \'short\': \'Short description\'}}\n```\n',
     'author': 'pwwang',
     'author_email': 'pwwang@pwwang.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.7.1,<4.0.0',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `pipen_annotate-0.6.3/PKG-INFO` & `pipen_annotate-0.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: pipen-annotate
-Version: 0.6.3
+Version: 0.7.0
 Summary: Use docstring to annotate pipen processes
 License: MIT
 Author: pwwang
 Author-email: pwwang@pwwang.com
-Requires-Python: >=3.7.1,<4.0.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pipen (>=0.7,<0.8)
+Requires-Dist: pipen (>=0.9,<0.10)
 Description-Content-Type: text/markdown
 
 # pipen-annotate
 
 Use docstring to annotate [pipen](https://github.com/pwwang/pipen) processes
 
 ## Installation
```

