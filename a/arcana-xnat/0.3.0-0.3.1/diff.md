# Comparing `tmp/arcana_xnat-0.3.0.tar.gz` & `tmp/arcana_xnat-0.3.1.tar.gz`

## Comparing `arcana_xnat-0.3.0.tar` & `arcana_xnat-0.3.1.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 arcana_xnat-0.3.0/arcana/xnat/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 arcana_xnat-0.3.0/arcana/xnat/_version.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 arcana_xnat-0.3.0/arcana/xnat/cli/__init__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 arcana_xnat-0.3.0/arcana/xnat/cli/base.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 arcana_xnat-0.3.0/arcana/xnat/cli/entrypoint.py
--rw-r--r--   0        0        0     4850 2020-02-02 00:00:00.000000 arcana_xnat-0.3.0/arcana/xnat/cli/update_release.py
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 arcana_xnat-0.3.0/arcana/xnat/cli/tests/test_cli_add_columns.py
--rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 arcana_xnat-0.3.0/arcana/xnat/cli/tests/test_cli_store.py
--rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 arcana_xnat-0.3.0/arcana/xnat/cli/tests/test_cli_xnat_images.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 arcana_xnat-0.3.0/arcana/xnat/data/__init__.py
--rw-r--r--   0        0        0    23117 2020-02-02 00:00:00.000000 arcana_xnat-0.3.0/arcana/xnat/data/api.py
--rw-r--r--   0        0        0     6143 2020-02-02 00:00:00.000000 arcana_xnat-0.3.0/arcana/xnat/data/cs.py
--rw-r--r--   0        0        0     6855 2020-02-02 00:00:00.000000 arcana_xnat-0.3.0/arcana/xnat/data/tests/test_store.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 arcana_xnat-0.3.0/arcana/xnat/deploy/__init__.py
--rw-r--r--   0        0        0    12988 2020-02-02 00:00:00.000000 arcana_xnat-0.3.0/arcana/xnat/deploy/command.py
--rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 arcana_xnat-0.3.0/arcana/xnat/deploy/image.py
--rw-r--r--   0        0        0     6933 2020-02-02 00:00:00.000000 arcana_xnat-0.3.0/arcana/xnat/deploy/tests/test_app.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arcana_xnat-0.3.0/arcana/xnat/utils/__init__.py
--rw-r--r--   0        0        0     5554 2020-02-02 00:00:00.000000 arcana_xnat-0.3.0/arcana/xnat/utils/testing.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 arcana_xnat-0.3.0/.gitignore
--rw-r--r--   0        0        0    16577 2020-02-02 00:00:00.000000 arcana_xnat-0.3.0/LICENSE
--rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 arcana_xnat-0.3.0/README.rst
--rw-r--r--   0        0        0     2388 2020-02-02 00:00:00.000000 arcana_xnat-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    21771 2020-02-02 00:00:00.000000 arcana_xnat-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 arcana_xnat-0.3.1/arcana/xnat/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 arcana_xnat-0.3.1/arcana/xnat/_version.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 arcana_xnat-0.3.1/arcana/xnat/cli/__init__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 arcana_xnat-0.3.1/arcana/xnat/cli/base.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 arcana_xnat-0.3.1/arcana/xnat/cli/entrypoint.py
+-rw-r--r--   0        0        0     4850 2020-02-02 00:00:00.000000 arcana_xnat-0.3.1/arcana/xnat/cli/update_release.py
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 arcana_xnat-0.3.1/arcana/xnat/cli/tests/test_cli_add_columns.py
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 arcana_xnat-0.3.1/arcana/xnat/cli/tests/test_cli_dataset_export.py
+-rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 arcana_xnat-0.3.1/arcana/xnat/cli/tests/test_cli_store.py
+-rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 arcana_xnat-0.3.1/arcana/xnat/cli/tests/test_cli_xnat_images.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 arcana_xnat-0.3.1/arcana/xnat/data/__init__.py
+-rw-r--r--   0        0        0    24033 2020-02-02 00:00:00.000000 arcana_xnat-0.3.1/arcana/xnat/data/api.py
+-rw-r--r--   0        0        0     6126 2020-02-02 00:00:00.000000 arcana_xnat-0.3.1/arcana/xnat/data/cs.py
+-rw-r--r--   0        0        0     6846 2020-02-02 00:00:00.000000 arcana_xnat-0.3.1/arcana/xnat/data/tests/test_store.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 arcana_xnat-0.3.1/arcana/xnat/deploy/__init__.py
+-rw-r--r--   0        0        0    12979 2020-02-02 00:00:00.000000 arcana_xnat-0.3.1/arcana/xnat/deploy/command.py
+-rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 arcana_xnat-0.3.1/arcana/xnat/deploy/image.py
+-rw-r--r--   0        0        0     6933 2020-02-02 00:00:00.000000 arcana_xnat-0.3.1/arcana/xnat/deploy/tests/test_app.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arcana_xnat-0.3.1/arcana/xnat/utils/__init__.py
+-rw-r--r--   0        0        0     5545 2020-02-02 00:00:00.000000 arcana_xnat-0.3.1/arcana/xnat/utils/testing.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 arcana_xnat-0.3.1/.gitignore
+-rw-r--r--   0        0        0    16577 2020-02-02 00:00:00.000000 arcana_xnat-0.3.1/LICENSE
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 arcana_xnat-0.3.1/README.rst
+-rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 arcana_xnat-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0    21719 2020-02-02 00:00:00.000000 arcana_xnat-0.3.1/PKG-INFO
```

### Comparing `arcana_xnat-0.3.0/arcana/xnat/cli/entrypoint.py` & `arcana_xnat-0.3.1/arcana/xnat/cli/entrypoint.py`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.0/arcana/xnat/cli/update_release.py` & `arcana_xnat-0.3.1/arcana/xnat/cli/update_release.py`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.0/arcana/xnat/cli/tests/test_cli_add_columns.py` & `arcana_xnat-0.3.1/arcana/xnat/cli/tests/test_cli_add_columns.py`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.0/arcana/xnat/cli/tests/test_cli_store.py` & `arcana_xnat-0.3.1/arcana/xnat/cli/tests/test_cli_store.py`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.0/arcana/xnat/cli/tests/test_cli_xnat_images.py` & `arcana_xnat-0.3.1/arcana/xnat/cli/tests/test_cli_xnat_images.py`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.0/arcana/xnat/data/api.py` & `arcana_xnat-0.3.1/arcana/xnat/data/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import typing as ty
 from glob import glob
 import tempfile
 import logging
 import hashlib
 import json
 import re
+from operator import attrgetter
 from zipfile import ZipFile, BadZipfile
 import attrs
 import xnat.session
 from fileformats.core import FileSet, Field
 from fileformats.medimage import DicomSet
 from fileformats.core.exceptions import FormatRecognitionError
 from arcana.core.utils.misc import (
@@ -24,15 +25,15 @@
 from arcana.core.exceptions import (
     ArcanaError,
     ArcanaUsageError,
 )
 from arcana.core.utils.serialize import asdict
 from arcana.core.data.tree import DataTree
 from arcana.core.data.entry import DataEntry
-from arcana.core.data import Clinical
+from arcana.stdlib import Clinical
 
 
 logger = logging.getLogger("arcana")
 
 tag_parse_re = re.compile(r"\((\d+),(\d+)\)")
 
 RELEVANT_DICOM_TAG_TYPES = set(("UI", "CS", "DA", "TM", "SH", "LO", "PN", "ST", "AS"))
@@ -59,15 +60,16 @@
         The amount of time to wait before checking that the required
         fileset has been downloaded to cache by another process has
         completed if they are attempting to download the same fileset
     """
 
     depth = 2
     DEFAULT_SPACE = Clinical
-    DEFAULT_HIERARCHY = ["subject", "session"]
+    DEFAULT_HIERARCHY = ("subject", "session")
+    # DEFAULT_ID_PATTERNS = (("timepoint", "session:order"),)
     PROV_RESOURCE = "PROVENANCE"
 
     #############################
     # DataStore implementations #
     #############################
 
     def populate_tree(self, tree: DataTree):
@@ -77,16 +79,35 @@
         Parameters
         ----------
         tree : DataTree
             The tree to populate with nodes via the ``DataTree.add_leaf`` method
         """
         with self.connection:
             # Get all "leaf" nodes, i.e. XNAT imaging session objects
-            for exp in self.connection.projects[tree.dataset_id].experiments.values():
-                tree.add_leaf([exp.subject.label, exp.label])
+            xproject = self.connection.projects[tree.dataset_id]
+            subjects = sorted(xproject.subjects.values(), key=attrgetter("label"))
+            for xsubject in subjects:
+                # Sort sessions into a logical order
+                xsessions = sorted(
+                    xsubject.experiments.values(),
+                    key=lambda x: (x.date, x.time, x.label),
+                )
+                for xsess in xsessions:
+                    date = xsess.date.strftime("%Y%m%d") if xsess.date else None
+                    metadata = {
+                        "session": {
+                            "date": date,
+                            "visit_id": xsess.visit_id,
+                            "age": xsess.age,
+                            "modality": xsess.modality,
+                        }
+                    }
+                    tree.add_leaf(
+                        [xsubject.label, xsess.label], metadata=metadata
+                    )
 
     def populate_row(self, row: DataRow):
         """
         Populate a row with all data entries found in the corresponding node in the data
         store (e.g. files within a directory, scans within an XNAT session).
 
         Parameters
```

### Comparing `arcana_xnat-0.3.0/arcana/xnat/data/cs.py` & `arcana_xnat-0.3.1/arcana/xnat/data/cs.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 Helper functions for generating XNAT Container Service compatible Docker
 containers
 """
 import os
 import re
 import logging
 from pathlib import Path
-import shutil
 import attrs
 from fileformats.core.base import FileSet
-from arcana.core.data import Clinical
+from arcana.stdlib import Clinical
 from arcana.core.data.space import DataSpace
 from arcana.core.data.row import DataRow
 from arcana.core.data.entry import DataEntry
 from arcana.core.exceptions import ArcanaNoDirectXnatMountException
 from .api import Xnat, path2label
 
 logger = logging.getLogger("arcana")
```

### Comparing `arcana_xnat-0.3.0/arcana/xnat/data/tests/test_store.py` & `arcana_xnat-0.3.1/arcana/xnat/data/tests/test_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import logging
 from pathlib import Path
 from functools import reduce
 import itertools
 import pytest
 from fileformats.generic import File
 from fileformats.field import Text as TextField
-from arcana.core.data.space import Clinical
+from arcana.stdlib import Clinical
 from arcana.core.data.set import Dataset
 from arcana.xnat.data import XnatViaCS
 from arcana.core.utils.serialize import asdict
 
 if sys.platform == "win32":
 
     def get_perms(f):
```

### Comparing `arcana_xnat-0.3.0/arcana/xnat/deploy/command.py` & `arcana_xnat-0.3.1/arcana/xnat/deploy/command.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 import typing as ty
 import re
 import attrs
 from fileformats.core import FileSet
 from arcana.core.deploy.command.base import ContainerCommand
 from arcana.xnat.data import XnatViaCS
-from arcana.core.data.space import Clinical
+from arcana.stdlib import Clinical
 from arcana.core.utils.serialize import ClassResolver
 
 if ty.TYPE_CHECKING:
     from .image import XnatApp
 
 
 @attrs.define(kw_only=True)
```

### Comparing `arcana_xnat-0.3.0/arcana/xnat/deploy/image.py` & `arcana_xnat-0.3.1/arcana/xnat/deploy/image.py`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.0/arcana/xnat/deploy/tests/test_app.py` & `arcana_xnat-0.3.1/arcana/xnat/deploy/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.0/arcana/xnat/utils/testing.py` & `arcana_xnat-0.3.1/arcana/xnat/utils/testing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import typing as ty
 import time
 from pathlib import Path
 import logging
 import tempfile
 import attrs
 import xnat
-from arcana.core.data.space import Clinical
+from arcana.stdlib import Clinical
 from arcana.core.data.space import DataSpace
 from arcana.core.data.row import DataRow
 from arcana.testing.data.blueprint import TestDatasetBlueprint, FileSetEntryBlueprint
 from arcana.core.exceptions import ArcanaError
 
 
 logger = logging.getLogger("arcana")
```

### Comparing `arcana_xnat-0.3.0/LICENSE` & `arcana_xnat-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `arcana_xnat-0.3.0/README.rst` & `arcana_xnat-0.3.1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 .. image:: https://img.shields.io/pypi/pyversions/arcana-xnat.svg
    :target: https://pypi.python.org/pypi/arcana-xnat/
    :alt: Python versions
 .. image:: https://img.shields.io/pypi/v/arcana-xnat.svg
    :target: https://pypi.python.org/pypi/arcana-xnat/
    :alt: Latest Version  
 .. image:: https://github.com/ArcanaFramework/arcana/actions/workflows/docs.yml/badge.svg
-   :target: http://arcana.readthedocs.io/en/latest/?badge=latest
+   :target: https://arcanaframework.github.io/arcana
    :alt: Docs
 
 
 An extension for the Arcana_ framework that adds the following classes to allow integrated
 deployment of workflows and analysis classes with XNAT_ imaging data repositories:
 
 * ``Xnat`` data store for accessing data via REST API (only)
```

### Comparing `arcana_xnat-0.3.0/pyproject.toml` & `arcana_xnat-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,14 @@
     "sphinx >=2.1.2",
     "sphinx-argparse >=0.2.0",
     "sphinx-click >=3.1",
 ]
 test = [
     "arcana-bids >=0.1",
     "fileformats-testing",
-    "codecov",
     "medimages4tests >=0.3",
     "pytest >=5.4.3",
     "pytest-cov >=2.12.1",
     "pytest-env >=0.6.2",
     "xnat4tests >=0.3.3",
     "imageio >=2.25.0"
 ]
```

### Comparing `arcana_xnat-0.3.0/PKG-INFO` & `arcana_xnat-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcana-xnat
-Version: 0.3.0
+Version: 0.3.1
 Summary: An extension of the Arcana framework to apply workflows and analyses on data stored within XNAT data repositories
 Project-URL: documentation, https://arcana.readthedocs.io
 Project-URL: repository, https://github.com/ArcanaFramework/arcana-xnat.git
 Author-email: "Thomas G. Close" <tom.g.close@gmail.com>
 Maintainer-email: "Thomas G. Close" <tom.g.close@gmail.com>
 License: Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International Public License
         
@@ -147,15 +147,14 @@
 Requires-Dist: numpydoc>=0.6.0; extra == 'doc'
 Requires-Dist: packaging; extra == 'doc'
 Requires-Dist: sphinx-argparse>=0.2.0; extra == 'doc'
 Requires-Dist: sphinx-click>=3.1; extra == 'doc'
 Requires-Dist: sphinx>=2.1.2; extra == 'doc'
 Provides-Extra: test
 Requires-Dist: arcana-bids>=0.1; extra == 'test'
-Requires-Dist: codecov; extra == 'test'
 Requires-Dist: fileformats-testing; extra == 'test'
 Requires-Dist: imageio>=2.25.0; extra == 'test'
 Requires-Dist: medimages4tests>=0.3; extra == 'test'
 Requires-Dist: pytest-cov>=2.12.1; extra == 'test'
 Requires-Dist: pytest-env>=0.6.2; extra == 'test'
 Requires-Dist: pytest>=5.4.3; extra == 'test'
 Requires-Dist: xnat4tests>=0.3.3; extra == 'test'
@@ -170,15 +169,15 @@
 .. image:: https://img.shields.io/pypi/pyversions/arcana-xnat.svg
    :target: https://pypi.python.org/pypi/arcana-xnat/
    :alt: Python versions
 .. image:: https://img.shields.io/pypi/v/arcana-xnat.svg
    :target: https://pypi.python.org/pypi/arcana-xnat/
    :alt: Latest Version  
 .. image:: https://github.com/ArcanaFramework/arcana/actions/workflows/docs.yml/badge.svg
-   :target: http://arcana.readthedocs.io/en/latest/?badge=latest
+   :target: https://arcanaframework.github.io/arcana
    :alt: Docs
 
 
 An extension for the Arcana_ framework that adds the following classes to allow integrated
 deployment of workflows and analysis classes with XNAT_ imaging data repositories:
 
 * ``Xnat`` data store for accessing data via REST API (only)
```

