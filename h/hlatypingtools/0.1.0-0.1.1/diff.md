# Comparing `tmp/hlatypingtools-0.1.0.tar.gz` & `tmp/hlatypingtools-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hlatypingtools-0.1.0.tar", max compression
+gzip compressed data, was "hlatypingtools-0.1.1.tar", max compression
```

## Comparing `hlatypingtools-0.1.0.tar` & `hlatypingtools-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0        0 2023-04-14 14:02:29.564981 hlatypingtools-0.1.0/hlatypingtools/__init__.py
--rw-r--r--   0        0        0      371 2023-04-14 14:42:35.560295 hlatypingtools-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      779 2023-04-14 14:45:16.610754 hlatypingtools-0.1.0/README.md
--rw-r--r--   0        0        0     1299 1970-01-01 00:00:00.000000 hlatypingtools-0.1.0/setup.py
--rw-r--r--   0        0        0     1107 1970-01-01 00:00:00.000000 hlatypingtools-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-14 14:02:29.564981 hlatypingtools-0.1.1/hlatypingtools/__init__.py
+-rw-r--r--   0        0        0      558 2023-04-14 15:43:18.514188 hlatypingtools-0.1.1/hlatypingtools/decrypt_file.py
+-rw-r--r--   0        0        0      529 2023-04-14 15:44:09.067655 hlatypingtools-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1178 2023-04-14 15:43:57.953770 hlatypingtools-0.1.1/README.md
+-rw-r--r--   0        0        0     1884 1970-01-01 00:00:00.000000 hlatypingtools-0.1.1/setup.py
+-rw-r--r--   0        0        0     1668 1970-01-01 00:00:00.000000 hlatypingtools-0.1.1/PKG-INFO
```

### Comparing `hlatypingtools-0.1.0/setup.py` & `hlatypingtools-0.1.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,24 +3,31 @@
 
 packages = \
 ['hlatypingtools']
 
 package_data = \
 {'': ['*']}
 
+install_requires = \
+['openpyxl>=3.1.2,<4.0.0',
+ 'pandas-stubs>=2.0.0.230412,<3.0.0.0',
+ 'pandas>=2.0.0,<3.0.0',
+ 'pyaescrypt>=6.0.0,<7.0.0']
+
 setup_kwargs = {
     'name': 'hlatypingtools',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': '',
-    'long_description': '# HLATypingTools\n\n## Getting Started\n#### Install from PyPI (recommended)\nTo use `HLATypingTools`, run `pip install HLATypingTools` in your terminal.\n\n#### Usage\n\n\n#### Exit codes\n\n\n## About the source code\n- Follows [PEP8](https://peps.python.org/pep-0008/) Style Guidelines.\n- All functions are unit-tested with [pytest](https://docs.pytest.org/en/stable/).\n- All variables are correctly type-hinted, reviewed with [static type checker](https://mypy.readthedocs.io/en/stable/)\n`mypy`.\n- All functions are documented with [docstrings](https://www.python.org/dev/peps/pep-0257/).\n\n\n## Useful links:\n- [Corresponding GitHub repository](https://github.com/JasonMendoza2008/HLATypingTools)\n- [Corresponding PyPI page](https://pypi.org/project/HLATypingTools)\n',
+    'long_description': '# HLATypingTools\n\n## Getting Started\n#### Install from PyPI (recommended)\nTo use `HLATypingTools`, run `pip install HLATypingTools` in your terminal.\n\n#### Usage\nIf you haven\'t decrypted the data yet (first time you are using the package and you did purchase the product),\nrun:\n```py\nfrom hlatypingtools.decrypt_file import decrypt_file\n\npassword: str = "___"   # Replace with password provided by the author \ndecrypt_file(password)\n```\nIt should print `File decrypted successfully`.\n\nThen you can use the package as follows:\n```py\n\n```\n\n#### Exit codes\n```py\n\n```\n\n## About the source code\n- Follows [PEP8](https://peps.python.org/pep-0008/) Style Guidelines.\n- All functions are unit-tested with [pytest](https://docs.pytest.org/en/stable/).\n- All variables are correctly type-hinted, reviewed with [static type checker](https://mypy.readthedocs.io/en/stable/)\n`mypy`.\n- All functions are documented with [docstrings](https://www.python.org/dev/peps/pep-0257/).\n\n\n## Useful links:\n- [Corresponding GitHub repository](https://github.com/JasonMendoza2008/HLATypingTools)\n- [Corresponding PyPI page](https://pypi.org/project/HLATypingTools)\n',
     'author': 'JasonMendoza2008',
     'author_email': 'lhotteromain@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
+    'install_requires': install_requires,
     'python_requires': '>=3.10,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `hlatypingtools-0.1.0/PKG-INFO` & `hlatypingtools-0.1.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,49 @@
 Metadata-Version: 2.1
 Name: hlatypingtools
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: JasonMendoza2008
 Author-email: lhotteromain@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
+Requires-Dist: pandas (>=2.0.0,<3.0.0)
+Requires-Dist: pandas-stubs (>=2.0.0.230412,<3.0.0.0)
+Requires-Dist: pyaescrypt (>=6.0.0,<7.0.0)
 Description-Content-Type: text/markdown
 
 # HLATypingTools
 
 ## Getting Started
 #### Install from PyPI (recommended)
 To use `HLATypingTools`, run `pip install HLATypingTools` in your terminal.
 
 #### Usage
+If you haven't decrypted the data yet (first time you are using the package and you did purchase the product),
+run:
+```py
+from hlatypingtools.decrypt_file import decrypt_file
+
+password: str = "___"   # Replace with password provided by the author 
+decrypt_file(password)
+```
+It should print `File decrypted successfully`.
 
+Then you can use the package as follows:
+```py
+
+```
 
 #### Exit codes
+```py
 
+```
 
 ## About the source code
 - Follows [PEP8](https://peps.python.org/pep-0008/) Style Guidelines.
 - All functions are unit-tested with [pytest](https://docs.pytest.org/en/stable/).
 - All variables are correctly type-hinted, reviewed with [static type checker](https://mypy.readthedocs.io/en/stable/)
 `mypy`.
 - All functions are documented with [docstrings](https://www.python.org/dev/peps/pep-0257/).
```

