# Comparing `tmp/chain-aide-1.0.3.tar.gz` & `tmp/chain-aide-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chain-aide-1.0.3.tar", last modified: Fri Apr 14 06:56:02 2023, max compression
+gzip compressed data, was "chain-aide-1.0.4.tar", last modified: Fri Apr 14 08:26:46 2023, max compression
```

## Comparing `chain-aide-1.0.3.tar` & `chain-aide-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 06:56:02.220872 chain-aide-1.0.3/
--rw-rw-rw-   0        0        0     1083 2023-03-23 06:13:36.000000 chain-aide-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     3589 2023-04-14 06:56:02.220872 chain-aide-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2716 2023-03-31 09:03:39.000000 chain-aide-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 06:56:02.215872 chain-aide-1.0.3/chain_aide/
--rw-rw-rw-   0        0        0       65 2023-03-23 06:25:45.000000 chain-aide-1.0.3/chain_aide/__init__.py
--rw-rw-rw-   0        0        0     2586 2023-03-31 06:26:42.000000 chain-aide-1.0.3/chain_aide/contract.py
--rw-rw-rw-   0        0        0     6095 2023-03-31 06:21:32.000000 chain-aide-1.0.3/chain_aide/main.py
--rw-rw-rw-   0        0        0     1635 2023-03-31 06:13:53.000000 chain-aide-1.0.3/chain_aide/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-14 06:56:02.219872 chain-aide-1.0.3/chain_aide.egg-info/
--rw-rw-rw-   0        0        0     3589 2023-04-14 06:56:02.000000 chain-aide-1.0.3/chain_aide.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      313 2023-04-14 06:56:02.000000 chain-aide-1.0.3/chain_aide.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 06:56:02.000000 chain-aide-1.0.3/chain_aide.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-14 06:56:02.000000 chain-aide-1.0.3/chain_aide.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      174 2023-04-14 06:56:02.000000 chain-aide-1.0.3/chain_aide.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-14 06:56:02.000000 chain-aide-1.0.3/chain_aide.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-14 06:56:02.220872 chain-aide-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1620 2023-04-14 06:55:22.000000 chain-aide-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 08:26:46.204867 chain-aide-1.0.4/
+-rw-rw-rw-   0        0        0     1083 2023-03-23 06:13:36.000000 chain-aide-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     3589 2023-04-14 08:26:46.189257 chain-aide-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2716 2023-03-31 09:03:39.000000 chain-aide-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 08:26:46.189257 chain-aide-1.0.4/chain_aide/
+-rw-rw-rw-   0        0        0       65 2023-03-23 06:25:45.000000 chain-aide-1.0.4/chain_aide/__init__.py
+-rw-rw-rw-   0        0        0     2586 2023-03-31 06:26:42.000000 chain-aide-1.0.4/chain_aide/contract.py
+-rw-rw-rw-   0        0        0     6176 2023-04-14 08:25:32.000000 chain-aide-1.0.4/chain_aide/main.py
+-rw-rw-rw-   0        0        0     1635 2023-03-31 06:13:53.000000 chain-aide-1.0.4/chain_aide/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-14 08:26:46.189257 chain-aide-1.0.4/chain_aide.egg-info/
+-rw-rw-rw-   0        0        0     3589 2023-04-14 08:26:46.000000 chain-aide-1.0.4/chain_aide.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      313 2023-04-14 08:26:46.000000 chain-aide-1.0.4/chain_aide.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 08:26:46.000000 chain-aide-1.0.4/chain_aide.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-14 06:56:02.000000 chain-aide-1.0.4/chain_aide.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      174 2023-04-14 08:26:46.000000 chain-aide-1.0.4/chain_aide.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-14 08:26:46.000000 chain-aide-1.0.4/chain_aide.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-14 08:26:46.207260 chain-aide-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1620 2023-04-14 08:25:58.000000 chain-aide-1.0.4/setup.py
```

### Comparing `chain-aide-1.0.3/LICENSE` & `chain-aide-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `chain-aide-1.0.3/PKG-INFO` & `chain-aide-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chain-aide
-Version: 1.0.3
+Version: 1.0.4
 Summary: An aide that helps you quickly access mainstream public chain and use its basic functions.
 Home-page: https://github.com/shinnng/chain-aide
 Author: Shinnng
 Author-email: shinnng@outlook.com
 License: MIT
 Keywords: chain
 Classifier: Development Status :: 4 - Beta
```

### Comparing `chain-aide-1.0.3/README.md` & `chain-aide-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `chain-aide-1.0.3/chain_aide/contract.py` & `chain-aide-1.0.4/chain_aide/contract.py`

 * *Files identical despite different names*

### Comparing `chain-aide-1.0.3/chain_aide/main.py` & `chain-aide-1.0.4/chain_aide/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,15 +131,17 @@
 
         if private_key:
             account = self.eth.account.from_key(private_key)
         else:
             account = self.default_account
 
         if not txn.get('from'):
+            txn.pop('gas')
             txn['from'] = account.address
+            txn['gas'] = self.eth.estimate_gas(txn)
 
         if not txn.get('nonce'):
             txn['nonce'] = self.eth.get_transaction_count(account.address)
 
         signed_txn = self.eth.account.sign_transaction(txn, account.key)
         if result_type == "txn":
             return signed_txn
```

### Comparing `chain-aide-1.0.3/chain_aide/utils.py` & `chain-aide-1.0.4/chain_aide/utils.py`

 * *Files identical despite different names*

### Comparing `chain-aide-1.0.3/chain_aide.egg-info/PKG-INFO` & `chain-aide-1.0.4/chain_aide.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chain-aide
-Version: 1.0.3
+Version: 1.0.4
 Summary: An aide that helps you quickly access mainstream public chain and use its basic functions.
 Home-page: https://github.com/shinnng/chain-aide
 Author: Shinnng
 Author-email: shinnng@outlook.com
 License: MIT
 Keywords: chain
 Classifier: Development Status :: 4 - Beta
```

### Comparing `chain-aide-1.0.3/setup.py` & `chain-aide-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 with open('./README.md', encoding='utf-8') as readme:
     long_description = readme.read()
 
 setup(
     name='chain-aide',
     # *IMPORTANT*: Don't manually change the version here. Use the 'bumpversion' utility.
-    version='1.0.3',
+    version='1.0.4',
     description="""An aide that helps you quickly access mainstream public chain and use its basic functions.""",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Shinnng',
     author_email='shinnng@outlook.com',
     url='https://github.com/shinnng/chain-aide',
     include_package_data=True,
```

