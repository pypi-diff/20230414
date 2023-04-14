# Comparing `tmp/arcana_bids-0.2.3.tar.gz` & `tmp/arcana_bids-0.2.4.tar.gz`

## Comparing `arcana_bids-0.2.3.tar` & `arcana_bids-0.2.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 arcana_bids-0.2.3/arcana/bids/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 arcana_bids-0.2.3/arcana/bids/_version.py
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 arcana_bids-0.2.3/arcana/bids/cli.py
--rw-r--r--   0        0        0    23234 2020-02-02 00:00:00.000000 arcana_bids-0.2.3/arcana/bids/data.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 arcana_bids-0.2.3/arcana/bids/deploy.py
--rw-r--r--   0        0        0    15156 2020-02-02 00:00:00.000000 arcana_bids-0.2.3/arcana/bids/tasks.py
--rw-r--r--   0        0        0     4445 2020-02-02 00:00:00.000000 arcana_bids-0.2.3/arcana/bids/tests/test_cli.py
--rw-r--r--   0        0        0     7471 2020-02-02 00:00:00.000000 arcana_bids-0.2.3/arcana/bids/tests/test_data.py
--rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 arcana_bids-0.2.3/arcana/bids/tests/test_tasks.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 arcana_bids-0.2.3/.gitignore
--rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 arcana_bids-0.2.3/LICENSE
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 arcana_bids-0.2.3/README.rst
--rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 arcana_bids-0.2.3/pyproject.toml
--rw-r--r--   0        0        0    18603 2020-02-02 00:00:00.000000 arcana_bids-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 arcana_bids-0.2.4/arcana/bids/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 arcana_bids-0.2.4/arcana/bids/_version.py
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 arcana_bids-0.2.4/arcana/bids/cli.py
+-rw-r--r--   0        0        0    23277 2020-02-02 00:00:00.000000 arcana_bids-0.2.4/arcana/bids/data.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 arcana_bids-0.2.4/arcana/bids/deploy.py
+-rw-r--r--   0        0        0    15156 2020-02-02 00:00:00.000000 arcana_bids-0.2.4/arcana/bids/tasks.py
+-rw-r--r--   0        0        0     4445 2020-02-02 00:00:00.000000 arcana_bids-0.2.4/arcana/bids/tests/test_cli.py
+-rw-r--r--   0        0        0     7471 2020-02-02 00:00:00.000000 arcana_bids-0.2.4/arcana/bids/tests/test_data.py
+-rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 arcana_bids-0.2.4/arcana/bids/tests/test_tasks.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 arcana_bids-0.2.4/.gitignore
+-rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 arcana_bids-0.2.4/LICENSE
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 arcana_bids-0.2.4/README.rst
+-rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 arcana_bids-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0    18563 2020-02-02 00:00:00.000000 arcana_bids-0.2.4/PKG-INFO
```

### Comparing `arcana_bids-0.2.3/arcana/bids/cli.py` & `arcana_bids-0.2.4/arcana/bids/cli.py`

 * *Files identical despite different names*

### Comparing `arcana_bids-0.2.3/arcana/bids/data.py` & `arcana_bids-0.2.4/arcana/bids/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from operator import itemgetter
 import attrs
 import jq
 from pathlib import Path
 from arcana.core.data.store import LocalStore
 from fileformats.core import FileSet, Field
 from fileformats.generic import Directory
-from fileformats.medimage.nifti import WithBids
+from fileformats.medimage.nifti import WithBids, NiftiGzX
 from arcana.core.exceptions import ArcanaUsageError
 from arcana.core.data.tree import DataTree
 from arcana.core.data.set import Dataset
 from arcana.stdlib import Clinical
 from arcana.core.data.entry import DataEntry
 from arcana.core.data.row import DataRow
 
@@ -77,14 +77,16 @@
     VALID_HIERARCHIES = (
         ["subject", "timepoint"],
         ["session"],
         ["group", "subject", "timepoint"],
         ["group", "session"],
     )
 
+    DEFAULT_DATATYPE = NiftiGzX
+
     #################################
     # Abstract-method implementations
     #################################
 
     def populate_tree(self, tree: DataTree):
         """
         Find all rows within the dataset stored in the store and
```

### Comparing `arcana_bids-0.2.3/arcana/bids/tasks.py` & `arcana_bids-0.2.4/arcana/bids/tasks.py`

 * *Files identical despite different names*

### Comparing `arcana_bids-0.2.3/arcana/bids/tests/test_cli.py` & `arcana_bids-0.2.4/arcana/bids/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `arcana_bids-0.2.3/arcana/bids/tests/test_data.py` & `arcana_bids-0.2.4/arcana/bids/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `arcana_bids-0.2.3/arcana/bids/tests/test_tasks.py` & `arcana_bids-0.2.4/arcana/bids/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `arcana_bids-0.2.3/LICENSE` & `arcana_bids-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `arcana_bids-0.2.3/README.rst` & `arcana_bids-0.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `arcana_bids-0.2.3/pyproject.toml` & `arcana_bids-0.2.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -47,15 +47,14 @@
     "numpydoc>=0.6.0",
     "packaging",
     "sphinx >=2.1.2",
     "sphinx-argparse>=0.2.0",
     "sphinx-click>=3.1",
 ]
 test = [
-    "codecov",
     "fileformats-testing",
     "medimages4tests >=0.3",
     "pytest>=5.4.3",
     "pytest-cov>=2.12.1",
     "pytest-env>=0.6.2",
 ]
```

### Comparing `arcana_bids-0.2.3/PKG-INFO` & `arcana_bids-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcana-bids
-Version: 0.2.3
+Version: 0.2.4
 Summary: An Arcana extension for interacting with Brain Imaging Structure (BIDS) datasets and associated "Apps"
 Project-URL: documentation, https://arcana.readthedocs.io
 Project-URL: repository, https://github.com/ArcanaFramework/arcana-bids.git
 Author-email: "Thomas G. Close" <tom.g.close@gmail.com>
 Maintainer-email: "Thomas G. Close" <tom.g.close@gmail.com>
 License: Creative Commons Attribution 4.0 International Public License
         By exercising the Licensed Rights (defined below), You accept and agree to be bound by the terms and conditions of this Creative Commons Attribution 4.0 International Public License ("Public License"). To the extent this Public License may be interpreted as a contract, You are granted the Licensed Rights in consideration of Your acceptance of these terms and conditions, and the Licensor grants You such rights in consideration of benefits the Licensor receives from making the Licensed Material available under these terms and conditions.
@@ -127,15 +127,14 @@
 Requires-Dist: mock>1.0; extra == 'doc'
 Requires-Dist: numpydoc>=0.6.0; extra == 'doc'
 Requires-Dist: packaging; extra == 'doc'
 Requires-Dist: sphinx-argparse>=0.2.0; extra == 'doc'
 Requires-Dist: sphinx-click>=3.1; extra == 'doc'
 Requires-Dist: sphinx>=2.1.2; extra == 'doc'
 Provides-Extra: test
-Requires-Dist: codecov; extra == 'test'
 Requires-Dist: fileformats-testing; extra == 'test'
 Requires-Dist: medimages4tests>=0.3; extra == 'test'
 Requires-Dist: pytest-cov>=2.12.1; extra == 'test'
 Requires-Dist: pytest-env>=0.6.2; extra == 'test'
 Requires-Dist: pytest>=5.4.3; extra == 'test'
 Description-Content-Type: text/x-rst
```

