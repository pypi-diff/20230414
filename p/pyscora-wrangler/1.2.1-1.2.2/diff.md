# Comparing `tmp/pyscora_wrangler-1.2.1.tar.gz` & `tmp/pyscora_wrangler-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyscora_wrangler-1.2.1.tar", max compression
+gzip compressed data, was "pyscora_wrangler-1.2.2.tar", max compression
```

## Comparing `pyscora_wrangler-1.2.1.tar` & `pyscora_wrangler-1.2.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1049 2023-04-14 15:14:19.543579 pyscora_wrangler-1.2.1/LICENSE
--rw-r--r--   0        0        0      659 2023-04-14 15:14:19.543579 pyscora_wrangler-1.2.1/README.md
--rw-r--r--   0        0        0     1069 2023-04-14 15:14:19.543579 pyscora_wrangler-1.2.1/pyproject.toml
--rw-r--r--   0        0        0       51 2023-04-14 15:14:19.543579 pyscora_wrangler-1.2.1/pyscora_wrangler/__init__.py
--rw-r--r--   0        0        0    14331 2023-04-14 15:14:19.543579 pyscora_wrangler-1.2.1/pyscora_wrangler/aws/README.md
--rw-r--r--   0        0        0      119 2023-04-14 15:14:19.543579 pyscora_wrangler-1.2.1/pyscora_wrangler/aws/__init__.py
--rw-r--r--   0        0        0     7114 2023-04-14 15:14:19.543579 pyscora_wrangler-1.2.1/pyscora_wrangler/aws/athena/__init__.py
--rw-r--r--   0        0        0    15796 2023-04-14 15:14:19.543579 pyscora_wrangler-1.2.1/pyscora_wrangler/aws/cognito/__init__.py
--rw-r--r--   0        0        0       88 2023-04-14 15:14:19.543579 pyscora_wrangler-1.2.1/pyscora_wrangler/aws/constants.py
--rw-r--r--   0        0        0     6697 2023-04-14 15:14:19.543579 pyscora_wrangler-1.2.1/pyscora_wrangler/aws/dynamodb/__init__.py
--rw-r--r--   0        0        0     2156 2023-04-14 15:14:19.543579 pyscora_wrangler-1.2.1/pyscora_wrangler/aws/secretsmanager/__init__.py
--rw-r--r--   0        0        0      671 2023-04-14 15:14:19.543579 pyscora_wrangler-1.2.1/pyscora_wrangler/aws/utils.py
--rw-r--r--   0        0        0      165 2023-04-14 15:14:19.543579 pyscora_wrangler-1.2.1/pyscora_wrangler/constants.py
--rw-r--r--   0        0        0      492 2023-04-14 15:14:19.543579 pyscora_wrangler-1.2.1/pyscora_wrangler/ldap/README.md
--rw-r--r--   0        0        0       60 2023-04-14 15:14:19.543579 pyscora_wrangler-1.2.1/pyscora_wrangler/ldap/__init__.py
--rw-r--r--   0        0        0     7711 2023-04-14 15:14:19.543579 pyscora_wrangler-1.2.1/pyscora_wrangler/ldap/service/__init__.py
--rw-r--r--   0        0        0       22 2023-04-14 15:14:19.543579 pyscora_wrangler-1.2.1/pyscora_wrangler/ldap/utils.py
--rw-r--r--   0        0        0     2693 2023-04-14 15:14:19.543579 pyscora_wrangler-1.2.1/pyscora_wrangler/utils.py
--rw-r--r--   0        0        0     1947 1970-01-01 00:00:00.000000 pyscora_wrangler-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1049 2023-04-14 17:59:30.594918 pyscora_wrangler-1.2.2/LICENSE
+-rw-r--r--   0        0        0      646 2023-04-14 17:59:30.594918 pyscora_wrangler-1.2.2/README.md
+-rw-r--r--   0        0        0     1069 2023-04-14 17:59:30.594918 pyscora_wrangler-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0       51 2023-04-14 17:59:30.594918 pyscora_wrangler-1.2.2/pyscora_wrangler/__init__.py
+-rw-r--r--   0        0        0    14331 2023-04-14 17:59:30.594918 pyscora_wrangler-1.2.2/pyscora_wrangler/aws/README.md
+-rw-r--r--   0        0        0      119 2023-04-14 17:59:30.594918 pyscora_wrangler-1.2.2/pyscora_wrangler/aws/__init__.py
+-rw-r--r--   0        0        0     7114 2023-04-14 17:59:30.594918 pyscora_wrangler-1.2.2/pyscora_wrangler/aws/athena/__init__.py
+-rw-r--r--   0        0        0    15796 2023-04-14 17:59:30.594918 pyscora_wrangler-1.2.2/pyscora_wrangler/aws/cognito/__init__.py
+-rw-r--r--   0        0        0       88 2023-04-14 17:59:30.594918 pyscora_wrangler-1.2.2/pyscora_wrangler/aws/constants.py
+-rw-r--r--   0        0        0     6697 2023-04-14 17:59:30.594918 pyscora_wrangler-1.2.2/pyscora_wrangler/aws/dynamodb/__init__.py
+-rw-r--r--   0        0        0     2156 2023-04-14 17:59:30.594918 pyscora_wrangler-1.2.2/pyscora_wrangler/aws/secretsmanager/__init__.py
+-rw-r--r--   0        0        0      671 2023-04-14 17:59:30.594918 pyscora_wrangler-1.2.2/pyscora_wrangler/aws/utils.py
+-rw-r--r--   0        0        0      165 2023-04-14 17:59:30.594918 pyscora_wrangler-1.2.2/pyscora_wrangler/constants.py
+-rw-r--r--   0        0        0      492 2023-04-14 17:59:30.594918 pyscora_wrangler-1.2.2/pyscora_wrangler/ldap/README.md
+-rw-r--r--   0        0        0       60 2023-04-14 17:59:30.594918 pyscora_wrangler-1.2.2/pyscora_wrangler/ldap/__init__.py
+-rw-r--r--   0        0        0     9797 2023-04-14 17:59:30.594918 pyscora_wrangler-1.2.2/pyscora_wrangler/ldap/service/__init__.py
+-rw-r--r--   0        0        0       22 2023-04-14 17:59:30.594918 pyscora_wrangler-1.2.2/pyscora_wrangler/ldap/utils.py
+-rw-r--r--   0        0        0     2693 2023-04-14 17:59:30.594918 pyscora_wrangler-1.2.2/pyscora_wrangler/utils.py
+-rw-r--r--   0        0        0     1934 1970-01-01 00:00:00.000000 pyscora_wrangler-1.2.2/PKG-INFO
```

### Comparing `pyscora_wrangler-1.2.1/LICENSE` & `pyscora_wrangler-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyscora_wrangler-1.2.1/README.md` & `pyscora_wrangler-1.2.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Pyscora Wrangler
 
 <p align="center">
-<img alt="Python versions" src="https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-brightgreen.svg">
+<img alt="Python versions" src="https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-brightgreen.svg">
 <a href="https://github.com/oncase/pyscora-wrangler/blob/main/LICENSE"><img alt="License: MIT" src="https://black.readthedocs.io/en/stable/_static/license.svg"></a>
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a></p>
 
 Python package that consists mainly of wrappers for Data Engineering tasks.
 
 In order to see the docs, click on the module that you want inside the folder `pyscora_wrangler/${MODULE}`
```

### Comparing `pyscora_wrangler-1.2.1/pyproject.toml` & `pyscora_wrangler-1.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyscora-wrangler"
-version = "1.2.1"
+version = "1.2.2"
 description = "Python lib for DE"
 authors = ["Oncase <contato@oncase.com.br>"]
 maintainers = ["Guilherme Morone <guilherme.morone@oncase.com.br>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/oncase/pyscora-wrangler"
 repository = "https://github.com/oncase/pyscora-wrangler"
```

### Comparing `pyscora_wrangler-1.2.1/pyscora_wrangler/aws/README.md` & `pyscora_wrangler-1.2.2/pyscora_wrangler/aws/README.md`

 * *Files identical despite different names*

### Comparing `pyscora_wrangler-1.2.1/pyscora_wrangler/aws/athena/__init__.py` & `pyscora_wrangler-1.2.2/pyscora_wrangler/aws/athena/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscora_wrangler-1.2.1/pyscora_wrangler/aws/cognito/__init__.py` & `pyscora_wrangler-1.2.2/pyscora_wrangler/aws/cognito/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscora_wrangler-1.2.1/pyscora_wrangler/aws/dynamodb/__init__.py` & `pyscora_wrangler-1.2.2/pyscora_wrangler/aws/dynamodb/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscora_wrangler-1.2.1/pyscora_wrangler/aws/secretsmanager/__init__.py` & `pyscora_wrangler-1.2.2/pyscora_wrangler/aws/secretsmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscora_wrangler-1.2.1/pyscora_wrangler/aws/utils.py` & `pyscora_wrangler-1.2.2/pyscora_wrangler/aws/utils.py`

 * *Files identical despite different names*

### Comparing `pyscora_wrangler-1.2.1/pyscora_wrangler/utils.py` & `pyscora_wrangler-1.2.2/pyscora_wrangler/utils.py`

 * *Files identical despite different names*

### Comparing `pyscora_wrangler-1.2.1/PKG-INFO` & `pyscora_wrangler-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyscora-wrangler
-Version: 1.2.1
+Version: 1.2.2
 Summary: Python lib for DE
 Home-page: https://github.com/oncase/pyscora-wrangler
 License: MIT
 Keywords: wrapper,scora,python,data_engineering
 Author: Oncase
 Author-email: contato@oncase.com.br
 Maintainer: Guilherme Morone
@@ -30,15 +30,15 @@
 Requires-Dist: typeguard (>=3.0.2,<4.0.0)
 Project-URL: Repository, https://github.com/oncase/pyscora-wrangler
 Description-Content-Type: text/markdown
 
 # Pyscora Wrangler
 
 <p align="center">
-<img alt="Python versions" src="https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-brightgreen.svg">
+<img alt="Python versions" src="https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-brightgreen.svg">
 <a href="https://github.com/oncase/pyscora-wrangler/blob/main/LICENSE"><img alt="License: MIT" src="https://black.readthedocs.io/en/stable/_static/license.svg"></a>
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a></p>
 
 Python package that consists mainly of wrappers for Data Engineering tasks.
 
 In order to see the docs, click on the module that you want inside the folder `pyscora_wrangler/${MODULE}`
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyscora-wrangler Version: 1.2.1 Summary: Python lib
+Metadata-Version: 2.1 Name: pyscora-wrangler Version: 1.2.2 Summary: Python lib
 for DE Home-page: https://github.com/oncase/pyscora-wrangler License: MIT
 Keywords: wrapper,scora,python,data_engineering Author: Oncase Author-email:
 contato@oncase.com.br Maintainer: Guilherme Morone Maintainer-email:
 guilherme.morone@oncase.com.br Requires-Python: >=3.8,<4.0 Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
```

