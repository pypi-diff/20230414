# Comparing `tmp/multisigwallet-predeployed-1.1.0a8.tar.gz` & `tmp/multisigwallet-predeployed-1.1.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multisigwallet-predeployed-1.1.0a8.tar", last modified: Fri Apr 14 18:40:00 2023, max compression
+gzip compressed data, was "multisigwallet-predeployed-1.1.0b0.tar", last modified: Thu Dec 29 22:24:50 2022, max compression
```

## Comparing `multisigwallet-predeployed-1.1.0a8.tar` & `multisigwallet-predeployed-1.1.0b0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:40:00.037916 multisigwallet-predeployed-1.1.0a8/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-14 18:39:18.000000 multisigwallet-predeployed-1.1.0a8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-14 18:40:00.037916 multisigwallet-predeployed-1.1.0a8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-14 18:39:18.000000 multisigwallet-predeployed-1.1.0a8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-14 18:39:18.000000 multisigwallet-predeployed-1.1.0a8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-14 18:40:00.041916 multisigwallet-predeployed-1.1.0a8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:40:00.037916 multisigwallet-predeployed-1.1.0a8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:40:00.037916 multisigwallet-predeployed-1.1.0a8/src/multisigwallet_predeployed/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-14 18:39:18.000000 multisigwallet-predeployed-1.1.0a8/src/multisigwallet_predeployed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-14 18:39:18.000000 multisigwallet-predeployed-1.1.0a8/src/multisigwallet_predeployed/address.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:40:00.037916 multisigwallet-predeployed-1.1.0a8/src/multisigwallet_predeployed/artifacts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:39:18.000000 multisigwallet-predeployed-1.1.0a8/src/multisigwallet_predeployed/artifacts/.keep
--rw-r--r--   0 runner    (1001) docker     (123)    45064 2023-04-14 18:39:53.000000 multisigwallet-predeployed-1.1.0a8/src/multisigwallet_predeployed/artifacts/MultiSigWallet.json
--rw-r--r--   0 runner    (1001) docker     (123)    14053 2023-04-14 18:39:53.000000 multisigwallet-predeployed-1.1.0a8/src/multisigwallet_predeployed/artifacts/MultiSigWallet.meta.json
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-14 18:39:18.000000 multisigwallet-predeployed-1.1.0a8/src/multisigwallet_predeployed/multisigwallet_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:39:18.000000 multisigwallet-predeployed-1.1.0a8/src/multisigwallet_predeployed/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:40:00.037916 multisigwallet-predeployed-1.1.0a8/src/multisigwallet_predeployed.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-14 18:40:00.000000 multisigwallet-predeployed-1.1.0a8/src/multisigwallet_predeployed.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-14 18:40:00.000000 multisigwallet-predeployed-1.1.0a8/src/multisigwallet_predeployed.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 18:40:00.000000 multisigwallet-predeployed-1.1.0a8/src/multisigwallet_predeployed.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-14 18:40:00.000000 multisigwallet-predeployed-1.1.0a8/src/multisigwallet_predeployed.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-14 18:40:00.000000 multisigwallet-predeployed-1.1.0a8/src/multisigwallet_predeployed.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:40:00.037916 multisigwallet-predeployed-1.1.0a8/test/
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-04-14 18:39:18.000000 multisigwallet-predeployed-1.1.0a8/test/test_multisigwallet_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 18:39:53.000000 multisigwallet-predeployed-1.1.0a8/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 22:24:50.541087 multisigwallet-predeployed-1.1.0b0/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2022-12-29 22:24:06.000000 multisigwallet-predeployed-1.1.0b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2022-12-29 22:24:50.545087 multisigwallet-predeployed-1.1.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2022-12-29 22:24:06.000000 multisigwallet-predeployed-1.1.0b0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2022-12-29 22:24:06.000000 multisigwallet-predeployed-1.1.0b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2022-12-29 22:24:50.545087 multisigwallet-predeployed-1.1.0b0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 22:24:50.541087 multisigwallet-predeployed-1.1.0b0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 22:24:50.541087 multisigwallet-predeployed-1.1.0b0/src/multisigwallet_predeployed/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2022-12-29 22:24:06.000000 multisigwallet-predeployed-1.1.0b0/src/multisigwallet_predeployed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2022-12-29 22:24:06.000000 multisigwallet-predeployed-1.1.0b0/src/multisigwallet_predeployed/address.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 22:24:50.541087 multisigwallet-predeployed-1.1.0b0/src/multisigwallet_predeployed/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-29 22:24:06.000000 multisigwallet-predeployed-1.1.0b0/src/multisigwallet_predeployed/artifacts/.keep
+-rw-r--r--   0 runner    (1001) docker     (123)    45064 2022-12-29 22:24:42.000000 multisigwallet-predeployed-1.1.0b0/src/multisigwallet_predeployed/artifacts/MultiSigWallet.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14053 2022-12-29 22:24:42.000000 multisigwallet-predeployed-1.1.0b0/src/multisigwallet_predeployed/artifacts/MultiSigWallet.meta.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2022-12-29 22:24:06.000000 multisigwallet-predeployed-1.1.0b0/src/multisigwallet_predeployed/multisigwallet_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-29 22:24:06.000000 multisigwallet-predeployed-1.1.0b0/src/multisigwallet_predeployed/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 22:24:50.541087 multisigwallet-predeployed-1.1.0b0/src/multisigwallet_predeployed.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2022-12-29 22:24:50.000000 multisigwallet-predeployed-1.1.0b0/src/multisigwallet_predeployed.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2022-12-29 22:24:50.000000 multisigwallet-predeployed-1.1.0b0/src/multisigwallet_predeployed.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-29 22:24:50.000000 multisigwallet-predeployed-1.1.0b0/src/multisigwallet_predeployed.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2022-12-29 22:24:50.000000 multisigwallet-predeployed-1.1.0b0/src/multisigwallet_predeployed.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2022-12-29 22:24:50.000000 multisigwallet-predeployed-1.1.0b0/src/multisigwallet_predeployed.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-29 22:24:50.541087 multisigwallet-predeployed-1.1.0b0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2022-12-29 22:24:06.000000 multisigwallet-predeployed-1.1.0b0/test/test_multisigwallet_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2022-12-29 22:24:42.000000 multisigwallet-predeployed-1.1.0b0/version.txt
```

### Comparing `multisigwallet-predeployed-1.1.0a8/PKG-INFO` & `multisigwallet-predeployed-1.1.0b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multisigwallet-predeployed
-Version: 1.1.0a8
+Version: 1.1.0b0
 Summary: A tool for generating predeployed MultiSigWallet smart contract
 Home-page: https://github.com/skalenetwork/multisigwallet-predeployed
 Author: Vadim Yavorsky
 Author-email: vadim@skalelabs.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `multisigwallet-predeployed-1.1.0a8/README.md` & `multisigwallet-predeployed-1.1.0b0/README.md`

 * *Files identical despite different names*

### Comparing `multisigwallet-predeployed-1.1.0a8/setup.cfg` & `multisigwallet-predeployed-1.1.0b0/setup.cfg`

 * *Files identical despite different names*

### Comparing `multisigwallet-predeployed-1.1.0a8/src/multisigwallet_predeployed/artifacts/MultiSigWallet.json` & `multisigwallet-predeployed-1.1.0b0/src/multisigwallet_predeployed/artifacts/MultiSigWallet.json`

 * *Files identical despite different names*

### Comparing `multisigwallet-predeployed-1.1.0a8/src/multisigwallet_predeployed/artifacts/MultiSigWallet.meta.json` & `multisigwallet-predeployed-1.1.0b0/src/multisigwallet_predeployed/artifacts/MultiSigWallet.meta.json`

 * *Files identical despite different names*

### Comparing `multisigwallet-predeployed-1.1.0a8/src/multisigwallet_predeployed/multisigwallet_generator.py` & `multisigwallet-predeployed-1.1.0b0/src/multisigwallet_predeployed/multisigwallet_generator.py`

 * *Files identical despite different names*

### Comparing `multisigwallet-predeployed-1.1.0a8/src/multisigwallet_predeployed.egg-info/PKG-INFO` & `multisigwallet-predeployed-1.1.0b0/src/multisigwallet_predeployed.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multisigwallet-predeployed
-Version: 1.1.0a8
+Version: 1.1.0b0
 Summary: A tool for generating predeployed MultiSigWallet smart contract
 Home-page: https://github.com/skalenetwork/multisigwallet-predeployed
 Author: Vadim Yavorsky
 Author-email: vadim@skalelabs.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `multisigwallet-predeployed-1.1.0a8/src/multisigwallet_predeployed.egg-info/SOURCES.txt` & `multisigwallet-predeployed-1.1.0b0/src/multisigwallet_predeployed.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `multisigwallet-predeployed-1.1.0a8/test/test_multisigwallet_generator.py` & `multisigwallet-predeployed-1.1.0b0/test/test_multisigwallet_generator.py`

 * *Files identical despite different names*

