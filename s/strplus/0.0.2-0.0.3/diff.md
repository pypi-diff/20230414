# Comparing `tmp/strplus-0.0.2.tar.gz` & `tmp/strplus-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strplus-0.0.2.tar", max compression
+gzip compressed data, was "strplus-0.0.3.tar", max compression
```

## Comparing `strplus-0.0.2.tar` & `strplus-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1069 2023-04-14 07:01:01.064336 strplus-0.0.2/LICENSE
--rw-r--r--   0        0        0     2242 2023-04-14 07:25:23.113912 strplus-0.0.2/README.md
--rw-r--r--   0        0        0      650 2023-04-14 07:34:26.003747 strplus-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      160 2023-04-14 07:14:43.924095 strplus-0.0.2/strplus/__init__.py
--rw-r--r--   0        0        0      646 2023-04-14 07:01:01.064336 strplus-0.0.2/strplus/strplus.py
--rw-r--r--   0        0        0     2870 1970-01-01 00:00:00.000000 strplus-0.0.2/setup.py
--rw-r--r--   0        0        0     2820 1970-01-01 00:00:00.000000 strplus-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-14 07:01:01.064336 strplus-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2247 2023-04-14 07:35:45.313725 strplus-0.0.3/README.md
+-rw-r--r--   0        0        0      650 2023-04-14 07:36:23.993714 strplus-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      160 2023-04-14 07:14:43.924095 strplus-0.0.3/strplus/__init__.py
+-rw-r--r--   0        0        0      646 2023-04-14 07:01:01.064336 strplus-0.0.3/strplus/strplus.py
+-rw-r--r--   0        0        0     2876 1970-01-01 00:00:00.000000 strplus-0.0.3/setup.py
+-rw-r--r--   0        0        0     2825 1970-01-01 00:00:00.000000 strplus-0.0.3/PKG-INFO
```

### Comparing `strplus-0.0.2/LICENSE` & `strplus-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `strplus-0.0.2/README.md` & `strplus-0.0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -71,9 +71,10 @@
 </a>
 
 
 <br>
 <br>
 <br>
 <br>
+<br>
 
 > WiseUpData
```

#### html2text {}

```diff
@@ -24,8 +24,9 @@
 pypi-using-poetry-on-ubuntu-22-04)
 
 --- #### Maintainer ð¤ ð¨âð» Sivio Liborio ð§
 silvio.liborio@wiseupdata.com silvio-de-melo-liborio_[LinkedIN]
 
 
 
+
 > WiseUpData
```

### Comparing `strplus-0.0.2/pyproject.toml` & `strplus-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strplus"
-version = "0.0.2"
+version = "0.0.3"
 authors = ["Silvio Liborio <silvio.liborio@wiseupdata.com>"]
 readme = "README.md"
 
 description = "Python extra functions for strings"
 
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `strplus-0.0.2/strplus/strplus.py` & `strplus-0.0.3/strplus/strplus.py`

 * *Files identical despite different names*

### Comparing `strplus-0.0.2/setup.py` & `strplus-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 ['strplus']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'strplus',
-    'version': '0.0.2',
+    'version': '0.0.3',
     'description': 'Python extra functions for strings',
-    'long_description': '<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="Wise Up Data\'s Instagram" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/instagram.png" />   \n</a> \n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data\'s Discord" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/discord.png" />\n</a>\n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data | Twitter" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/twitter.png" />\n</a>\n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data\'s LinkedIN" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/linkedin.png" />\n</a>\n\n![visitors](https://visitor-badge.glitch.me/badge?page_id=wiseupdata.strplus&left_color=green&right_color=black)\n![license](https://img.shields.io/github/license/wiseupdata/strplus)\n\n---\n\n<br>\n<br>\n\n<a href="https://github.com/wiseupdata/wiseupdata">\n<img align="left" alt="img" src="https://raw.githubusercontent.com/wiseupdata/strplus/main/assets/python.png" width="300" />\n</a>\n\n<h1>\nPython extra functions for strings ❤️\n</h1>\n\n<br>\n<br>\n<br>\n<br>\n<br>\n<br>\n\n```\nfrom strplus import Str\ns = Str("hello")\nassert s.upper() == "HELLO"\n```\n\n<br>\n<br>\n<br>\n<br>\n<a href="https://github.com/wiseupdata/wiseupdata">\n<img align="center" alt="img" src="https://raw.githubusercontent.com/wiseupdata/strplus/main/assets/under_construction.gif" width="300" />\n</a>\n\n<br>\n<br>\n<br>\n\n# References 🌍 🗄️\n\n1. [Wise Up Data](https://github.com/wiseupdata)\n1. [Emojis](https://github.com/wiseupdata/emojis)\n1. [Pypi Deploy](https://www.digitalocean.com/community/tutorials/how-to-publish-python-packages-to-pypi-using-poetry-on-ubuntu-22-04)\n\n<br><br>\n---\n\n#### Maintainer 🤗 👨\u200d💻\n\nSivio Liborio\n\n📧 silvio.liborio@wiseupdata.com\n\n<a href="https://www.linkedin.com/in/silvio-de-melo-liborio">silvio-de-melo-liborio <img align="left" alt="LinkedIN" width="18px" src="https://raw.githubusercontent.com/wiseupdata/wsl-latest/main/assets/linkedin.svg" />\n</a>\n\n\n<br>\n<br>\n<br>\n<br>\n\n> WiseUpData',
+    'long_description': '<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="Wise Up Data\'s Instagram" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/instagram.png" />   \n</a> \n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data\'s Discord" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/discord.png" />\n</a>\n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data | Twitter" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/twitter.png" />\n</a>\n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data\'s LinkedIN" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/linkedin.png" />\n</a>\n\n![visitors](https://visitor-badge.glitch.me/badge?page_id=wiseupdata.strplus&left_color=green&right_color=black)\n![license](https://img.shields.io/github/license/wiseupdata/strplus)\n\n---\n\n<br>\n<br>\n\n<a href="https://github.com/wiseupdata/wiseupdata">\n<img align="left" alt="img" src="https://raw.githubusercontent.com/wiseupdata/strplus/main/assets/python.png" width="300" />\n</a>\n\n<h1>\nPython extra functions for strings ❤️\n</h1>\n\n<br>\n<br>\n<br>\n<br>\n<br>\n<br>\n\n```\nfrom strplus import Str\ns = Str("hello")\nassert s.upper() == "HELLO"\n```\n\n<br>\n<br>\n<br>\n<br>\n<a href="https://github.com/wiseupdata/wiseupdata">\n<img align="center" alt="img" src="https://raw.githubusercontent.com/wiseupdata/strplus/main/assets/under_construction.gif" width="300" />\n</a>\n\n<br>\n<br>\n<br>\n\n# References 🌍 🗄️\n\n1. [Wise Up Data](https://github.com/wiseupdata)\n1. [Emojis](https://github.com/wiseupdata/emojis)\n1. [Pypi Deploy](https://www.digitalocean.com/community/tutorials/how-to-publish-python-packages-to-pypi-using-poetry-on-ubuntu-22-04)\n\n<br><br>\n---\n\n#### Maintainer 🤗 👨\u200d💻\n\nSivio Liborio\n\n📧 silvio.liborio@wiseupdata.com\n\n<a href="https://www.linkedin.com/in/silvio-de-melo-liborio">silvio-de-melo-liborio <img align="left" alt="LinkedIN" width="18px" src="https://raw.githubusercontent.com/wiseupdata/wsl-latest/main/assets/linkedin.svg" />\n</a>\n\n\n<br>\n<br>\n<br>\n<br>\n<br>\n\n> WiseUpData',
     'author': 'Silvio Liborio',
     'author_email': 'silvio.liborio@wiseupdata.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['strplus']
 package_data = \ {'': ['*']} setup_kwargs = { 'name': 'strplus', 'version':
-'0.0.2', 'description': 'Python extra functions for strings',
+'0.0.3', 'description': 'Python extra functions for strings',
 'long_description': '\n_[Wise_Up_Data\'s_Instagram]_\n \n\n_[wise_Up_Data\'s
 Discord]\n\n\n_[wise_Up_Data_|_Twitter]\n\n\n_[wise_Up_Data\'s_LinkedIN]\n\n\n!
 [visitors](https://visitor-badge.glitch.me/
 badge?page_id=wiseupdata.strplus&left_color=green&right_color=black)\n!
 [license](https://img.shields.io/github/license/wiseupdata/strplus)\n\n---\n\n
 \n
 \n\n\n[img]\n\n\n
@@ -29,11 +29,12 @@
 packages-to-pypi-using-poetry-on-ubuntu-22-04)\n\n
 
 \n---\n\n#### Maintainer ð¤ ð¨\u200dð»\n\nSivio Liborio\n\nð§
 silvio.liborio@wiseupdata.com\n\nsilvio-de-melo-liborio_[LinkedIN]\n\n\n\n
 \n
 \n
 \n
+\n
 \n\n> WiseUpData', 'author': 'Silvio Liborio', 'author_email':
 'silvio.liborio@wiseupdata.com', 'maintainer': 'None', 'maintainer_email':
 'None', 'url': 'None', 'packages': packages, 'package_data': package_data,
 'python_requires': '>=3.9,<4.0', } setup(**setup_kwargs)
```

### Comparing `strplus-0.0.2/PKG-INFO` & `strplus-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strplus
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python extra functions for strings
 Author: Silvio Liborio
 Author-email: silvio.liborio@wiseupdata.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -87,9 +87,10 @@
 </a>
 
 
 <br>
 <br>
 <br>
 <br>
+<br>
 
 > WiseUpData
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: strplus Version: 0.0.2 Summary: Python extra
+Metadata-Version: 2.1 Name: strplus Version: 0.0.3 Summary: Python extra
 functions for strings Author: Silvio Liborio Author-email:
 silvio.liborio@wiseupdata.com Requires-Python: >=3.9,<4.0 Classifier: License
 :: OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3 Description-Content-Type: text/markdown [Wise_Up_Data's
@@ -32,8 +32,9 @@
 pypi-using-poetry-on-ubuntu-22-04)
 
 --- #### Maintainer ð¤ ð¨âð» Sivio Liborio ð§
 silvio.liborio@wiseupdata.com silvio-de-melo-liborio_[LinkedIN]
 
 
 
+
 > WiseUpData
```

