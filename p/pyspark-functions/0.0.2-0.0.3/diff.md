# Comparing `tmp/pyspark_functions-0.0.2.tar.gz` & `tmp/pyspark_functions-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspark_functions-0.0.2.tar", max compression
+gzip compressed data, was "pyspark_functions-0.0.3.tar", max compression
```

## Comparing `pyspark_functions-0.0.2.tar` & `pyspark_functions-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1069 2023-04-13 17:30:33.772007 pyspark_functions-0.0.2/LICENSE
--rw-r--r--   0        0        0     2137 2023-04-13 19:02:07.651920 pyspark_functions-0.0.2/README.md
--rw-r--r--   0        0        0      329 2023-04-13 19:07:23.591914 pyspark_functions-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-13 17:20:07.292013 pyspark_functions-0.0.2/pyspark_functions/__init__.py
--rw-r--r--   0        0        0       27 2023-04-13 17:20:11.692015 pyspark_functions-0.0.2/pyspark_functions/main.py
--rw-r--r--   0        0        0     2728 1970-01-01 00:00:00.000000 pyspark_functions-0.0.2/setup.py
--rw-r--r--   0        0        0     2541 1970-01-01 00:00:00.000000 pyspark_functions-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-13 17:30:33.772007 pyspark_functions-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2137 2023-04-13 19:02:07.651920 pyspark_functions-0.0.3/README.md
+-rw-r--r--   0        0        0      404 2023-04-13 22:07:28.960775 pyspark_functions-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-13 17:20:07.292013 pyspark_functions-0.0.3/pyspark_functions/__init__.py
+-rw-r--r--   0        0        0     3112 2023-04-13 22:06:48.870777 pyspark_functions-0.0.3/pyspark_functions/dataframe.py
+-rw-r--r--   0        0        0       27 2023-04-13 17:20:11.692015 pyspark_functions-0.0.3/pyspark_functions/main.py
+-rw-r--r--   0        0        0     2818 1970-01-01 00:00:00.000000 pyspark_functions-0.0.3/setup.py
+-rw-r--r--   0        0        0     2581 1970-01-01 00:00:00.000000 pyspark_functions-0.0.3/PKG-INFO
```

### Comparing `pyspark_functions-0.0.2/LICENSE` & `pyspark_functions-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyspark_functions-0.0.2/README.md` & `pyspark_functions-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyspark_functions-0.0.2/setup.py` & `pyspark_functions-0.0.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,24 +3,28 @@
 
 packages = \
 ['pyspark_functions']
 
 package_data = \
 {'': ['*']}
 
+install_requires = \
+['pyspark>=3.4.0,<4.0.0']
+
 setup_kwargs = {
     'name': 'pyspark-functions',
-    'version': '0.0.2',
+    'version': '0.0.3',
     'description': '',
     'long_description': '<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="Wise Up Data\'s Instagram" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/instagram.png" />   \n</a> \n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data\'s Discord" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/discord.png" />\n</a>\n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data | Twitter" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/twitter.png" />\n</a>\n<a href="https://github.com/wiseupdata/wiseupdata">\n  <img align="left" alt="wise Up Data\'s LinkedIN" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/linkedin.png" />\n</a>\n\n![visitors](https://visitor-badge.glitch.me/badge?page_id=wiseupdata.pyspark-functions&left_color=green&right_color=black)\n![license](https://img.shields.io/github/license/wiseupdata/pyspark-functions)\n\n---\n\n<a href="https://github.com/wiseupdata/wiseupdata">\n<img align="left" alt="img" src="https://raw.githubusercontent.com/wiseupdata/pyspark-functions/main/assets/pyspark.png" width="300" />\n</a>\n\n<h1>\nPyspark extra functions ❤️\n</h1>\n\n<br>\n<br>\n<br>\n<br>\n<br>\n<br>\n<br>\n<br>\n<a href="https://github.com/wiseupdata/wiseupdata">\n<img align="center" alt="img" src="https://raw.githubusercontent.com/wiseupdata/pyspark-functions/main/assets/under_construction.gif" width="300" />\n</a>\n\n<br>\n<br>\n<br>\n\n# References 🌍 🗄️\n\n1. [Wise Up Data](https://github.com/wiseupdata)\n1. [Emojis](https://github.com/wiseupdata/emojis)\n1. [Pypi Deploy](https://www.digitalocean.com/community/tutorials/how-to-publish-python-packages-to-pypi-using-poetry-on-ubuntu-22-04)\n\n<br><br>\n---\n\n#### Maintainer 🤗 👨\u200d💻\n\nSivio Liborio\n\n📧 silvio.liborio@wiseupdata.com\n\n<a href="https://www.linkedin.com/in/silvio-de-melo-liborio">silvio-de-melo-liborio <img align="left" alt="LinkedIN" width="18px" src="https://raw.githubusercontent.com/wiseupdata/wsl-latest/main/assets/linkedin.svg" />\n</a>\n',
     'author': 'wiseupdata',
     'author_email': 'silvio.liborio@wiseupdata.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
+    'install_requires': install_requires,
     'python_requires': '>=3.9,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
-['pyspark_functions'] package_data = \ {'': ['*']} setup_kwargs = { 'name':
-'pyspark-functions', 'version': '0.0.2', 'description': '', 'long_description':
-'\n_[Wise_Up_Data\'s_Instagram]_\n \n\n_[wise_Up_Data\'s_Discord]\n\n\n_[wise
-Up_Data_|_Twitter]\n\n\n_[wise_Up_Data\'s_LinkedIN]\n\n\n![visitors](https://
-visitor-badge.glitch.me/badge?page_id=wiseupdata.pyspark-
+['pyspark_functions'] package_data = \ {'': ['*']} install_requires = \
+['pyspark>=3.4.0,<4.0.0'] setup_kwargs = { 'name': 'pyspark-functions',
+'version': '0.0.3', 'description': '', 'long_description': '\n_[Wise_Up_Data\'s
+Instagram]_\n \n\n_[wise_Up_Data\'s_Discord]\n\n\n_[wise_Up_Data_|
+Twitter]\n\n\n_[wise_Up_Data\'s_LinkedIN]\n\n\n![visitors](https://visitor-
+badge.glitch.me/badge?page_id=wiseupdata.pyspark-
 functions&left_color=green&right_color=black)\n![license](https://
 img.shields.io/github/license/wiseupdata/pyspark-functions)\n\n---\n\n\n
 [img]\n\n\n
 ****** \nPyspark extra functions â¤ï¸\n ******
 \n\n
 \n
 \n
@@ -24,9 +25,9 @@
 Deploy](https://www.digitalocean.com/community/tutorials/how-to-publish-python-
 packages-to-pypi-using-poetry-on-ubuntu-22-04)\n\n
 
 \n---\n\n#### Maintainer ð¤ ð¨\u200dð»\n\nSivio Liborio\n\nð§
 silvio.liborio@wiseupdata.com\n\nsilvio-de-melo-liborio_[LinkedIN]\n\n',
 'author': 'wiseupdata', 'author_email': 'silvio.liborio@wiseupdata.com',
 'maintainer': 'None', 'maintainer_email': 'None', 'url': 'None', 'packages':
-packages, 'package_data': package_data, 'python_requires': '>=3.9,<4.0', }
-setup(**setup_kwargs)
+packages, 'package_data': package_data, 'install_requires': install_requires,
+'python_requires': '>=3.9,<4.0', } setup(**setup_kwargs)
```

### Comparing `pyspark_functions-0.0.2/PKG-INFO` & `pyspark_functions-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: pyspark-functions
-Version: 0.0.2
+Version: 0.0.3
 Summary: 
 Author: wiseupdata
 Author-email: silvio.liborio@wiseupdata.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pyspark (>=3.4.0,<4.0.0)
 Description-Content-Type: text/markdown
 
 <a href="https://github.com/wiseupdata/wiseupdata">
   <img align="left" alt="Wise Up Data's Instagram" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/instagram.png" />   
 </a> 
 <a href="https://github.com/wiseupdata/wiseupdata">
   <img align="left" alt="wise Up Data's Discord" width="22px" src="https://raw.githubusercontent.com/wiseupdata/wiseupdata/main/assets/discord.png" />
```

#### html2text {}

```diff
@@ -1,17 +1,18 @@
-Metadata-Version: 2.1 Name: pyspark-functions Version: 0.0.2 Summary: Author:
+Metadata-Version: 2.1 Name: pyspark-functions Version: 0.0.3 Summary: Author:
 wiseupdata Author-email: silvio.liborio@wiseupdata.com Requires-Python:
 >=3.9,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Description-
-Content-Type: text/markdown [Wise_Up_Data's_Instagram] [wise_Up_Data's_Discord]
-[wise_Up_Data_|_Twitter] [wise_Up_Data's_LinkedIN] ![visitors](https://visitor-
-badge.glitch.me/badge?page_id=wiseupdata.pyspark-
-functions&left_color=green&right_color=black) ![license](https://
-img.shields.io/github/license/wiseupdata/pyspark-functions) --- [img]
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
+Dist: pyspark (>=3.4.0,<4.0.0) Description-Content-Type: text/markdown [Wise_Up
+Data's_Instagram] [wise_Up_Data's_Discord] [wise_Up_Data_|_Twitter] [wise_Up
+Data's_LinkedIN] ![visitors](https://visitor-badge.glitch.me/
+badge?page_id=wiseupdata.pyspark-functions&left_color=green&right_color=black)
+![license](https://img.shields.io/github/license/wiseupdata/pyspark-functions)
+--- [img]
 ****** Pyspark extra functions â¤ï¸ ******
```

