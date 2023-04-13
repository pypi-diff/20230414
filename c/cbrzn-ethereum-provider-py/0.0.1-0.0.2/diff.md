# Comparing `tmp/cbrzn_ethereum_provider_py-0.0.1.tar.gz` & `tmp/cbrzn_ethereum_provider_py-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbrzn_ethereum_provider_py-0.0.1.tar", max compression
+gzip compressed data, was "cbrzn_ethereum_provider_py-0.0.2.tar", max compression
```

## Comparing `cbrzn_ethereum_provider_py-0.0.1.tar` & `cbrzn_ethereum_provider_py-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2999 2023-04-11 23:25:43.088688 cbrzn_ethereum_provider_py-0.0.1/cbrzn_ethereum_provider_py/__init__.py
--rw-r--r--   0        0        0     1862 2023-04-11 23:25:43.084688 cbrzn_ethereum_provider_py-0.0.1/cbrzn_ethereum_provider_py/connection.py
--rw-r--r--   0        0        0     3147 2023-04-11 23:25:43.088688 cbrzn_ethereum_provider_py-0.0.1/cbrzn_ethereum_provider_py/connections.py
--rw-r--r--   0        0        0      559 2023-04-11 15:28:55.628769 cbrzn_ethereum_provider_py-0.0.1/cbrzn_ethereum_provider_py/networks.py
--rw-r--r--   0        0        0      519 2023-04-11 16:00:10.761474 cbrzn_ethereum_provider_py-0.0.1/cbrzn_ethereum_provider_py/wrap/types.py
--rw-r--r--   0        0        0     1095 2023-04-11 23:20:02.060550 cbrzn_ethereum_provider_py-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      725 1970-01-01 00:00:00.000000 cbrzn_ethereum_provider_py-0.0.1/setup.py
--rw-r--r--   0        0        0      443 1970-01-01 00:00:00.000000 cbrzn_ethereum_provider_py-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2999 2023-04-13 22:45:42.021696 cbrzn_ethereum_provider_py-0.0.2/cbrzn_ethereum_provider_py/__init__.py
+-rw-r--r--   0        0        0     1862 2023-04-13 22:45:42.021696 cbrzn_ethereum_provider_py-0.0.2/cbrzn_ethereum_provider_py/connection.py
+-rw-r--r--   0        0        0     3147 2023-04-13 22:45:42.025697 cbrzn_ethereum_provider_py-0.0.2/cbrzn_ethereum_provider_py/connections.py
+-rw-r--r--   0        0        0      559 2023-04-11 15:28:55.628769 cbrzn_ethereum_provider_py-0.0.2/cbrzn_ethereum_provider_py/networks.py
+-rw-r--r--   0        0        0      519 2023-04-11 16:00:10.761474 cbrzn_ethereum_provider_py-0.0.2/cbrzn_ethereum_provider_py/wrap/types.py
+-rw-r--r--   0        0        0     1095 2023-04-13 22:45:51.789746 cbrzn_ethereum_provider_py-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      725 1970-01-01 00:00:00.000000 cbrzn_ethereum_provider_py-0.0.2/setup.py
+-rw-r--r--   0        0        0      443 1970-01-01 00:00:00.000000 cbrzn_ethereum_provider_py-0.0.2/PKG-INFO
```

### Comparing `cbrzn_ethereum_provider_py-0.0.1/cbrzn_ethereum_provider_py/__init__.py` & `cbrzn_ethereum_provider_py-0.0.2/cbrzn_ethereum_provider_py/__init__.py`

 * *Files identical despite different names*

### Comparing `cbrzn_ethereum_provider_py-0.0.1/cbrzn_ethereum_provider_py/connection.py` & `cbrzn_ethereum_provider_py-0.0.2/cbrzn_ethereum_provider_py/connection.py`

 * *Files identical despite different names*

### Comparing `cbrzn_ethereum_provider_py-0.0.1/cbrzn_ethereum_provider_py/connections.py` & `cbrzn_ethereum_provider_py-0.0.2/cbrzn_ethereum_provider_py/connections.py`

 * *Files identical despite different names*

### Comparing `cbrzn_ethereum_provider_py-0.0.1/cbrzn_ethereum_provider_py/networks.py` & `cbrzn_ethereum_provider_py-0.0.2/cbrzn_ethereum_provider_py/networks.py`

 * *Files identical despite different names*

### Comparing `cbrzn_ethereum_provider_py-0.0.1/cbrzn_ethereum_provider_py/wrap/types.py` & `cbrzn_ethereum_provider_py-0.0.2/cbrzn_ethereum_provider_py/wrap/types.py`

 * *Files identical despite different names*

### Comparing `cbrzn_ethereum_provider_py-0.0.1/pyproject.toml` & `cbrzn_ethereum_provider_py-0.0.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "cbrzn-ethereum-provider-py"
-version = "0.0.1"
+version = "0.0.2"
 description = "Ethereum provider in python"
 authors = ["Cesar <cesar@polywrap.io>"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 web3 = "6.1.0"
 eth_account = "0.8.0"
-polywrap-plugin = "0.1.0a15"
+polywrap-plugin = "0.1.0a28"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 pytest-asyncio = "^0.19.0"
 pylint = "^2.15.4"
 black = "^22.10.0"
 bandit = { version = "^1.7.4", extras = ["toml"]}
 tox = "^3.26.0"
 tox-poetry = "^0.4.1"
 isort = "^5.10.1"
 pyright = "^1.1.275"
 pydocstyle = "^6.1.1"
-polywrap-client = "0.1.0a15"
-polywrap-client-config-builder = "0.1.0a15"
+polywrap-client = "0.1.0a28"
+polywrap-client-config-builder = "0.1.0a28"
 
 [tool.bandit]
 exclude_dirs = ["tests"]
 
 [tool.black]
 target-version = ["py310"]
```

### Comparing `cbrzn_ethereum_provider_py-0.0.1/setup.py` & `cbrzn_ethereum_provider_py-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['cbrzn_ethereum_provider_py', 'cbrzn_ethereum_provider_py.wrap']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['eth_account==0.8.0', 'polywrap-plugin==0.1.0a15', 'web3==6.1.0']
+['eth_account==0.8.0', 'polywrap-plugin==0.1.0a28', 'web3==6.1.0']
 
 setup_kwargs = {
     'name': 'cbrzn-ethereum-provider-py',
-    'version': '0.0.1',
+    'version': '0.0.2',
     'description': 'Ethereum provider in python',
     'long_description': 'None',
     'author': 'Cesar',
     'author_email': 'cesar@polywrap.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

