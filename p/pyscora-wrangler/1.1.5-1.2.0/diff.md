# Comparing `tmp/pyscora_wrangler-1.1.5.tar.gz` & `tmp/pyscora_wrangler-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyscora_wrangler-1.1.5.tar", max compression
+gzip compressed data, was "pyscora_wrangler-1.2.0.tar", max compression
```

## Comparing `pyscora_wrangler-1.1.5.tar` & `pyscora_wrangler-1.2.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0     1049 2023-04-11 01:17:18.607700 pyscora_wrangler-1.1.5/LICENSE
--rw-r--r--   0        0        0      659 2023-04-11 01:17:18.607700 pyscora_wrangler-1.1.5/README.md
--rw-r--r--   0        0        0     1116 2023-04-11 01:17:18.607700 pyscora_wrangler-1.1.5/pyproject.toml
--rw-r--r--   0        0        0       51 2023-04-11 01:17:18.607700 pyscora_wrangler-1.1.5/pyscora_wrangler/__init__.py
--rw-r--r--   0        0        0    14258 2023-04-11 01:17:18.607700 pyscora_wrangler-1.1.5/pyscora_wrangler/aws/README.md
--rw-r--r--   0        0        0       85 2023-04-11 01:17:18.607700 pyscora_wrangler-1.1.5/pyscora_wrangler/aws/__init__.py
--rw-r--r--   0        0        0     7114 2023-04-11 01:17:18.607700 pyscora_wrangler-1.1.5/pyscora_wrangler/aws/athena/__init__.py
--rw-r--r--   0        0        0    15796 2023-04-11 01:17:18.607700 pyscora_wrangler-1.1.5/pyscora_wrangler/aws/cognito/__init__.py
--rw-r--r--   0        0        0       88 2023-04-11 01:17:18.607700 pyscora_wrangler-1.1.5/pyscora_wrangler/aws/constants.py
--rw-r--r--   0        0        0     6697 2023-04-11 01:17:18.607700 pyscora_wrangler-1.1.5/pyscora_wrangler/aws/dynamodb/__init__.py
--rw-r--r--   0        0        0      671 2023-04-11 01:17:18.607700 pyscora_wrangler-1.1.5/pyscora_wrangler/aws/utils.py
--rw-r--r--   0        0        0      165 2023-04-11 01:17:18.607700 pyscora_wrangler-1.1.5/pyscora_wrangler/constants.py
--rw-r--r--   0        0        0      495 2023-04-11 01:17:18.607700 pyscora_wrangler-1.1.5/pyscora_wrangler/ldap/README.md
--rw-r--r--   0        0        0       60 2023-04-11 01:17:18.607700 pyscora_wrangler-1.1.5/pyscora_wrangler/ldap/__init__.py
--rw-r--r--   0        0        0     7585 2023-04-11 01:17:18.611699 pyscora_wrangler-1.1.5/pyscora_wrangler/ldap/service/__init__.py
--rw-r--r--   0        0        0       22 2023-04-11 01:17:18.611699 pyscora_wrangler-1.1.5/pyscora_wrangler/ldap/utils.py
--rw-r--r--   0        0        0     2692 2023-04-11 01:17:18.611699 pyscora_wrangler-1.1.5/pyscora_wrangler/utils.py
--rw-r--r--   0        0        0     1998 1970-01-01 00:00:00.000000 pyscora_wrangler-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1049 2023-04-13 15:26:10.695539 pyscora_wrangler-1.2.0/LICENSE
+-rw-r--r--   0        0        0      659 2023-04-13 15:26:10.695539 pyscora_wrangler-1.2.0/README.md
+-rw-r--r--   0        0        0     1069 2023-04-13 15:26:10.695539 pyscora_wrangler-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0       51 2023-04-13 15:26:10.695539 pyscora_wrangler-1.2.0/pyscora_wrangler/__init__.py
+-rw-r--r--   0        0        0    14331 2023-04-13 15:26:10.695539 pyscora_wrangler-1.2.0/pyscora_wrangler/aws/README.md
+-rw-r--r--   0        0        0      119 2023-04-13 15:26:10.695539 pyscora_wrangler-1.2.0/pyscora_wrangler/aws/__init__.py
+-rw-r--r--   0        0        0     7114 2023-04-13 15:26:10.695539 pyscora_wrangler-1.2.0/pyscora_wrangler/aws/athena/__init__.py
+-rw-r--r--   0        0        0    15796 2023-04-13 15:26:10.695539 pyscora_wrangler-1.2.0/pyscora_wrangler/aws/cognito/__init__.py
+-rw-r--r--   0        0        0       88 2023-04-13 15:26:10.695539 pyscora_wrangler-1.2.0/pyscora_wrangler/aws/constants.py
+-rw-r--r--   0        0        0     6697 2023-04-13 15:26:10.695539 pyscora_wrangler-1.2.0/pyscora_wrangler/aws/dynamodb/__init__.py
+-rw-r--r--   0        0        0     2156 2023-04-13 15:26:10.699539 pyscora_wrangler-1.2.0/pyscora_wrangler/aws/secretsmanager/__init__.py
+-rw-r--r--   0        0        0      671 2023-04-13 15:26:10.699539 pyscora_wrangler-1.2.0/pyscora_wrangler/aws/utils.py
+-rw-r--r--   0        0        0      165 2023-04-13 15:26:10.699539 pyscora_wrangler-1.2.0/pyscora_wrangler/constants.py
+-rw-r--r--   0        0        0      495 2023-04-13 15:26:10.699539 pyscora_wrangler-1.2.0/pyscora_wrangler/ldap/README.md
+-rw-r--r--   0        0        0       60 2023-04-13 15:26:10.699539 pyscora_wrangler-1.2.0/pyscora_wrangler/ldap/__init__.py
+-rw-r--r--   0        0        0     7585 2023-04-13 15:26:10.699539 pyscora_wrangler-1.2.0/pyscora_wrangler/ldap/service/__init__.py
+-rw-r--r--   0        0        0       22 2023-04-13 15:26:10.699539 pyscora_wrangler-1.2.0/pyscora_wrangler/ldap/utils.py
+-rw-r--r--   0        0        0     2692 2023-04-13 15:26:10.699539 pyscora_wrangler-1.2.0/pyscora_wrangler/utils.py
+-rw-r--r--   0        0        0     1947 1970-01-01 00:00:00.000000 pyscora_wrangler-1.2.0/PKG-INFO
```

### Comparing `pyscora_wrangler-1.1.5/LICENSE` & `pyscora_wrangler-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyscora_wrangler-1.1.5/README.md` & `pyscora_wrangler-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pyscora_wrangler-1.1.5/pyproject.toml` & `pyscora_wrangler-1.2.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 [tool.poetry]
 name = "pyscora-wrangler"
-version = "1.1.5"
+version = "1.2.0"
 description = "Python lib for DE"
-authors = ["Oncase <suporte@oncase.com.br>"]
+authors = ["Oncase <contato@oncase.com.br>"]
 maintainers = ["Guilherme Morone <guilherme.morone@oncase.com.br>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/oncase/pyscora-wrangler"
 repository = "https://github.com/oncase/pyscora-wrangler"
 keywords = ["wrapper", "scora", "python", "data_engineering"]
 classifiers = [
     "Intended Audience :: Developers",
     "Natural Language :: English",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.10"
 ]
 include = ["LICENSE"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 boto3 = "^1.26.108"
 awswrangler = "^2.20.1"
```

### Comparing `pyscora_wrangler-1.1.5/pyscora_wrangler/aws/README.md` & `pyscora_wrangler-1.2.0/pyscora_wrangler/aws/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -214,10 +214,14 @@
 
 `None`
 
 ## DynamoDB
 
 See `./dynamodb/__init__.py` for more details.
 
+## SecretsManager
+
+See `./secretsmanager/__init__.py` for more details.
+
 ## Other Services
 
 Check out [boto3 docs](https://boto3.amazonaws.com/v1/documentation/api/latest/index.html) and [awswrangler docs](https://pypi.org/project/awswrangler/) for more information.
```

### Comparing `pyscora_wrangler-1.1.5/pyscora_wrangler/aws/athena/__init__.py` & `pyscora_wrangler-1.2.0/pyscora_wrangler/aws/athena/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscora_wrangler-1.1.5/pyscora_wrangler/aws/cognito/__init__.py` & `pyscora_wrangler-1.2.0/pyscora_wrangler/aws/cognito/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscora_wrangler-1.1.5/pyscora_wrangler/aws/dynamodb/__init__.py` & `pyscora_wrangler-1.2.0/pyscora_wrangler/aws/dynamodb/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscora_wrangler-1.1.5/pyscora_wrangler/aws/utils.py` & `pyscora_wrangler-1.2.0/pyscora_wrangler/aws/utils.py`

 * *Files identical despite different names*

### Comparing `pyscora_wrangler-1.1.5/pyscora_wrangler/ldap/service/__init__.py` & `pyscora_wrangler-1.2.0/pyscora_wrangler/ldap/service/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscora_wrangler-1.1.5/pyscora_wrangler/utils.py` & `pyscora_wrangler-1.2.0/pyscora_wrangler/utils.py`

 * *Files identical despite different names*

### Comparing `pyscora_wrangler-1.1.5/PKG-INFO` & `pyscora_wrangler-1.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: pyscora-wrangler
-Version: 1.1.5
+Version: 1.2.0
 Summary: Python lib for DE
 Home-page: https://github.com/oncase/pyscora-wrangler
 License: MIT
 Keywords: wrapper,scora,python,data_engineering
 Author: Oncase
-Author-email: suporte@oncase.com.br
+Author-email: contato@oncase.com.br
 Maintainer: Guilherme Morone
 Maintainer-email: guilherme.morone@oncase.com.br
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: asyncio (>=3.4.3,<4.0.0)
 Requires-Dist: awswrangler (>=2.20.1,<3.0.0)
 Requires-Dist: boto3 (>=1.26.108,<2.0.0)
 Requires-Dist: ldap3 (>=2.9.1,<3.0.0)
 Requires-Dist: pyathena (>=2.23.0,<3.0.0)
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: pyscora-wrangler Version: 1.1.5 Summary: Python lib
+Metadata-Version: 2.1 Name: pyscora-wrangler Version: 1.2.0 Summary: Python lib
 for DE Home-page: https://github.com/oncase/pyscora-wrangler License: MIT
 Keywords: wrapper,scora,python,data_engineering Author: Oncase Author-email:
-suporte@oncase.com.br Maintainer: Guilherme Morone Maintainer-email:
+contato@oncase.com.br Maintainer: Guilherme Morone Maintainer-email:
 guilherme.morone@oncase.com.br Requires-Python: >=3.8,<4.0 Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Requires-Dist: asyncio (>=3.4.3,<4.0.0)
-Requires-Dist: awswrangler (>=2.20.1,<3.0.0) Requires-Dist: boto3
-(>=1.26.108,<2.0.0) Requires-Dist: ldap3 (>=2.9.1,<3.0.0) Requires-Dist:
-pyathena (>=2.23.0,<3.0.0) Requires-Dist: pyyaml (>=6.0,<7.0) Requires-Dist:
-typeguard (>=3.0.2,<4.0.0) Project-URL: Repository, https://github.com/oncase/
-pyscora-wrangler Description-Content-Type: text/markdown # Pyscora Wrangler
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Requires-Dist:
+asyncio (>=3.4.3,<4.0.0) Requires-Dist: awswrangler (>=2.20.1,<3.0.0) Requires-
+Dist: boto3 (>=1.26.108,<2.0.0) Requires-Dist: ldap3 (>=2.9.1,<3.0.0) Requires-
+Dist: pyathena (>=2.23.0,<3.0.0) Requires-Dist: pyyaml (>=6.0,<7.0) Requires-
+Dist: typeguard (>=3.0.2,<4.0.0) Project-URL: Repository, https://github.com/
+oncase/pyscora-wrangler Description-Content-Type: text/markdown # Pyscora
+Wrangler
              [Python versions] [License:_MIT] [Code_style:_black]
 Python package that consists mainly of wrappers for Data Engineering tasks. In
 order to see the docs, click on the module that you want inside the folder
 `pyscora_wrangler/${MODULE}`
```

