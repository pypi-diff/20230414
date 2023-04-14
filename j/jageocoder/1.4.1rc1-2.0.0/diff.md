# Comparing `tmp/jageocoder-1.4.1rc1.tar.gz` & `tmp/jageocoder-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jageocoder-1.4.1rc1.tar", max compression
+gzip compressed data, was "jageocoder-2.0.0.tar", max compression
```

## Comparing `jageocoder-1.4.1rc1.tar` & `jageocoder-2.0.0.tar`

### file list

```diff
@@ -1,21 +1,18 @@
--rw-r--r--   0        0        0      113 2023-03-13 04:34:17.970010 jageocoder-1.4.1rc1/LICENSE
--rw-r--r--   0        0        0    11683 2023-03-13 04:34:17.970010 jageocoder-1.4.1rc1/README.md
--rw-r--r--   0        0        0     1365 2023-04-07 01:57:33.442274 jageocoder-1.4.1rc1/jageocoder/__init__.py
--rw-r--r--   0        0        0     5792 2023-04-07 01:40:25.133090 jageocoder-1.4.1rc1/jageocoder/__main__.py
--rw-r--r--   0        0        0     2574 2023-03-13 04:34:17.974010 jageocoder-1.4.1rc1/jageocoder/address.py
--rw-r--r--   0        0        0    12277 2023-04-07 01:18:05.462895 jageocoder-1.4.1rc1/jageocoder/aza_master.py
--rw-r--r--   0        0        0      339 2023-04-07 01:18:05.462895 jageocoder-1.4.1rc1/jageocoder/base.py
--rw-r--r--   0        0        0      676 2023-04-07 01:18:05.462895 jageocoder-1.4.1rc1/jageocoder/dataset.py
--rw-r--r--   0        0        0      691 2023-03-13 04:34:17.974010 jageocoder-1.4.1rc1/jageocoder/exceptions.py
--rw-r--r--   0        0        0    18862 2023-04-07 01:47:15.772927 jageocoder-1.4.1rc1/jageocoder/itaiji.py
--rw-r--r--   0        0        0    14220 2023-03-13 04:34:17.974010 jageocoder-1.4.1rc1/jageocoder/itaiji_dic.json
--rw-r--r--   0        0        0    12242 2023-04-07 01:40:58.365275 jageocoder-1.4.1rc1/jageocoder/module.py
--rw-r--r--   0        0        0    29136 2023-04-07 01:18:05.466894 jageocoder-1.4.1rc1/jageocoder/node.py
--rw-r--r--   0        0        0      991 2023-04-07 01:18:05.466894 jageocoder-1.4.1rc1/jageocoder/note.py
--rw-r--r--   0        0        0     2643 2023-04-07 01:49:25.338650 jageocoder-1.4.1rc1/jageocoder/result.py
--rw-r--r--   0        0        0    16727 2023-04-07 01:55:47.264507 jageocoder-1.4.1rc1/jageocoder/rev.py
--rw-r--r--   0        0        0     7854 2023-03-13 04:34:17.974010 jageocoder-1.4.1rc1/jageocoder/strlib.py
--rw-r--r--   0        0        0    51920 2023-04-07 01:46:02.292036 jageocoder-1.4.1rc1/jageocoder/tree.py
--rw-r--r--   0        0        0     5185 2023-04-07 01:18:05.466894 jageocoder-1.4.1rc1/jageocoder/trie.py
--rw-r--r--   0        0        0     1071 2023-04-07 01:57:24.862130 jageocoder-1.4.1rc1/pyproject.toml
--rw-r--r--   0        0        0    13007 1970-01-01 00:00:00.000000 jageocoder-1.4.1rc1/PKG-INFO
+-rw-r--r--   0        0        0      113 2023-04-14 08:49:30.870739 jageocoder-2.0.0/LICENSE
+-rw-r--r--   0        0        0     8253 2023-04-14 11:42:42.077451 jageocoder-2.0.0/README.md
+-rw-r--r--   0        0        0     1405 2023-04-14 11:42:42.077451 jageocoder-2.0.0/jageocoder/__init__.py
+-rw-r--r--   0        0        0     4028 2023-04-14 11:42:42.077451 jageocoder-2.0.0/jageocoder/__main__.py
+-rw-r--r--   0        0        0     2574 2023-04-14 08:49:30.886739 jageocoder-2.0.0/jageocoder/address.py
+-rw-r--r--   0        0        0    12147 2023-04-14 11:42:42.077451 jageocoder-2.0.0/jageocoder/aza_master.py
+-rw-r--r--   0        0        0     1171 2023-04-14 11:42:42.077451 jageocoder-2.0.0/jageocoder/dataset.py
+-rw-r--r--   0        0        0      691 2023-04-14 08:49:30.886739 jageocoder-2.0.0/jageocoder/exceptions.py
+-rw-r--r--   0        0        0    18862 2023-04-14 11:42:42.077451 jageocoder-2.0.0/jageocoder/itaiji.py
+-rw-r--r--   0        0        0    14220 2023-04-14 08:49:30.890739 jageocoder-2.0.0/jageocoder/itaiji_dic.json
+-rw-r--r--   0        0        0    10983 2023-04-14 11:42:42.077451 jageocoder-2.0.0/jageocoder/module.py
+-rw-r--r--   0        0        0    36822 2023-04-14 11:42:42.081451 jageocoder-2.0.0/jageocoder/node.py
+-rw-r--r--   0        0        0     2631 2023-04-14 11:42:42.081451 jageocoder-2.0.0/jageocoder/result.py
+-rw-r--r--   0        0        0     7854 2023-04-14 08:49:30.890739 jageocoder-2.0.0/jageocoder/strlib.py
+-rw-r--r--   0        0        0    48184 2023-04-14 11:42:42.081451 jageocoder-2.0.0/jageocoder/tree.py
+-rw-r--r--   0        0        0     4995 2023-04-14 11:42:42.081451 jageocoder-2.0.0/jageocoder/trie.py
+-rw-r--r--   0        0        0     1150 2023-04-14 11:42:42.081451 jageocoder-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     9566 1970-01-01 00:00:00.000000 jageocoder-2.0.0/PKG-INFO
```

### Comparing `jageocoder-1.4.1rc1/README.md` & `jageocoder-2.0.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -16,71 +16,51 @@
 {'matched': '新宿区西新宿2-8-', 'candidates': [{'id': 5961406, 'name': '8番', 'x': 139.691778, 'y': 35.689627, 'level': 7, 'note': None, 'fullname': ['東京都', '新宿区', '西新宿', '二丁目', '8番']}]}
 ```
 
 # How to install
 
 ## Prerequisites
 
-Requires Python 3.6.x or later.
+Requires Python 3.7.x or later.
 
-The following packages will be installed automatically.
-
-- [marisa-trie](https://pypi.org/project/marisa-trie/)
-    for building and retrieving TRIE index
-- [SQLAlchemy](https://pypi.org/project/SQLAlchemy/)
-    for abstracting access to the RDBMS
+All other required packages will be installed automatically.
 
 ## Install instructions
 
 - Install the package with `pip install jageocoder`
+- Download an address database file compatible with that version from 
+  [here](https://www.info-proto.com/static/jageocoder/latest/v2/)
 - Install the dictionary with `install-dictionary` command
 
 ```sh
 pip install jageocoder
-jageocoder install-dictionary
+wget https://www.info-proto.com/static/jageocoder/latest/v2/jukyo_all_v20.zip
+jageocoder install-dictionary jukyo_all_v20.zip
 ```
 
-The dictionary database will be created under
-`{sys.prefix}/jageocoder/db/`, or if the user doesn't have 
-write permission there `{site.USER_DATA}/jageocoder/db/`
-by default.
-
-If you need to know the location of the directory containing
-the dictionary database, perform `get-db-dir` command as follows,
-or call `jageocoder.get_db_dir()` in your script.
+The dictionary database will be installed under
+`{sys.prefix}/jageocoder/db2/` by default,
+however if the user doesn't have write permission there,
+`{site.USER_DATA}/jageocoder/db2/` instead.
+
+If you need to know the location of the dictionary directory,
+perform `get-db-dir` command as follows. (Or call
+`jageocoder.get_db_dir()` in your script)
 
 ```sh
 jageocoder get-db-dir
 ```
 
 If you prefer to create it in another location, set the environment
-variable `JAGEOCODER_DB_DIR` before executing `install_dictionary()`
+variable `JAGEOCODER_DB2_DIR` before executing `install_dictionary()`
 to specify the directory.
 
 ```sh
-export JAGEOCODER_DB_DIR='/usr/local/share/jageocoder/db'
-install-dictionary
-```
-
-## Migrate dictinary
-
-The `install-dictionary` command will download and install
-a version of the address dictionary file that is compatible with
-the currently installed jageocoder package.
-
-If you upgrade the jageocoder package after installing
-the address dictionary file, it may no longer be compatible with
-the installed address dictionary file.
-In which case you will need to reinstall or migrate the dictionary.
-
-To migrate the dictionary, run the `migrate-dictionary` command.
-This process may take a long time.
-
-```sh
-jageocoder migrate-dictionary
+export JAGEOCODER_DB2_DIR='/usr/local/share/jageocoder/db2'
+install-dictionary <db-file>
 ```
 
 ## Uninstall instructions
 
 Remove the directory containing the database, or perform 
 `uninstall-dictionary` command as follows.
 
@@ -102,21 +82,14 @@
 as a library and used by calling the API, but for testing purposes,
 you can check the geocoding results with the following command.
 
 ```sh
 jageocoder search 新宿区西新宿２－８－１
 ```
 
-If you want to look up an address from longitude and latitude,
-specify `reverse` instead of `search`.
-
-```sh
-jageocoder reverse 139.6917 35.6896
-```
-
 You can check the list of available commands with `--help`.
 
 ```sh
 jageocoder --help
 ```
 
 ## Using API
@@ -159,91 +132,15 @@
 - level: Address level (1:Prefecture, 2:County, 3:City and 23 district,
     4:Ward, 5:Oaza, 6:Aza and Chome, 7:Block, 8:Building)
 - note: Notes such as city codes
 - fullname: List of address notations from the prefecture level to this node
 
 ### Search for addresses by longitude and latitude
 
-Use `reverse()` to find addresses by longitude and latitude
-(so called 'reverse geocoding').
-
-The `reverse()` function returns the three addresses surrounding
-the specified longitude and latitude.
-(The results are formatted for better viewing)
-
-The `candidate` of each element contains information about
-the address node (AddressNode), and the `dist` contains
-the distance (geodesic distance, in meters)
-from the specified point to the representative point of the address.
-
-```
->>> jageocoder.reverse(139.6917, 35.6896)
-[
-  {
-    'candidate': {
-      'id': 12299330, 'name': '二丁目',
-      'x': 139.691774, 'y': 35.68945, 'level': 6,
-      'note': 'postcode:1600023',
-      'fullname': ['東京都', '新宿区', '西新宿', '二丁目']
-    },
-    'dist': 17.940303970792183
-  }, {
-    'candidate': {
-      'id': 12300198, 'name': '六丁目',
-      'x': 139.690969, 'y': 35.693426, 'level': 6,
-      'note': 'postcode:1600023',
-      'fullname': ['東京都', '新宿区', '西新宿', '六丁目']
-    },
-    'dist': 429.6327545403412
-  }, {
-    'candidate': {
-      'id': 12300498, 'name': '四丁目',
-      'x': 139.68762, 'y': 35.68754, 'level': 6,
-      'note': 'postcode:1600023',
-      'fullname': ['東京都', '新宿区', '西新宿', '四丁目']
-    },
-    'dist': 434.31591285255234
-  }
-]
-```
-
-If the `level` optional parameter is specified,
-it will return a more detailed address.
-However, it takes time to calculate.
-
-```
->>> jageocoder.reverse(139.6917, 35.6896, level=7)
-[
-  {
-    'candidate': {
-      'id': 12299340, 'name': '8番',
-      'x': 139.691778, 'y': 35.689627, 'level': 7,
-      'note': None,
-      'fullname': ['東京都', '新宿区', '西新宿', '二丁目', '8番']
-    },
-    'dist': 7.669497303543382
-  }, {
-    'candidate': {
-      'id': 12299330, 'name': '二丁目',
-      'x': 139.691774, 'y': 35.68945, 'level': 6,
-      'note': 'postcode:1600023',
-      'fullname': ['東京都', '新宿区', '西新宿', '二丁目']
-    },
-    'dist': 17.940303970792183
-  }, {
-    'candidate': {
-      'id': 12300588, 'name': '15番',
-      'x': 139.688172, 'y': 35.689264, 'level': 7,
-      'note': None,
-      'fullname': ['東京都', '新宿区', '西新宿', '四丁目', '15番']
-    },
-    'dist': 321.50874020809823
-  }
-]
-```
+Note: This method is not available in v2 series.
 
 ### Explore the attribute information of an address
 
 Use `searchNode()` to retrieve information about an address.
 
 This function returns a list of type `jageocoder.result.Result` .
 You can access the address node from node element of the Result object.
@@ -330,44 +227,17 @@
 ```
 >>> parent.children
 <sqlalchemy.orm.dynamic.AppenderQuery object at 0x7fbc08404b38>
 >>> [child.name for child in parent.children]
 ['10番', '11番', '1番', '2番', '3番', '4番', '5番', '6番', '7番', '8番', '9番']
 ```
 
-# For developers
-
-## Running the unittests
-
-```sh
-python -m unittest
-``` 
-
-`tests.test_search` tests for some special address notations.
-
-- Street address in Sapporo city such as '北3西1' for '北三条西一丁目'
-- Toorina in Kyoto city such as '下立売通新町西入薮ノ内町' for '薮ノ内町'
-
 ## Create your own dictionary
 
-Please use the dictionary coverter
-[jageocoder-converter](https://github.com/t-sagara/jageocoder-converter).
-
-## Sample Web Application
-
-A sample of a simple web app using Flask is available under
-`flask-demo`.
-
-Perform the following steps. Then, access port 5000.
-
-```
-cd flask-demo
-pip install flask flask-cors
-bash run.sh
-```
+Consider using [jageocoder-converter](https://github.com/t-sagara/jageocoder-converter).
 
 ## ToDos
 
 - Supporting address changes
 
     The functionality to handle address changes due to municipal consolidation, etc.
     has already been implemented in the C++ version, but will be implemented
```

### Comparing `jageocoder-1.4.1rc1/jageocoder/__init__.py` & `jageocoder-2.0.0/jageocoder/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 running the following steps.
 
     >>> import jageocoder
     >>> jageocoder.init()
     >>> jageocoder.searchNode('<Japanese-address>')
 """
 
-__version__ = '1.4.1rc1'  # The package version
-__dictionary_version__ = '20220519'  # Compatible dictionary version
+__version__ = '2.0.0'  # The package version
+__dictionary_version__ = '20230405'  # Compatible dictionary version
 __author__ = 'Takeshi Sagara <sagara@info-proto.com>'
 
 __all__ = [
     'init',
     'free',
     'is_initialized',
     'set_search_config',
@@ -46,8 +46,8 @@
 ]
 
 from jageocoder.module import init, free, is_initialized,\
     get_db_dir, set_search_config, get_search_config,\
     get_module_tree, download_dictionary, install_dictionary,\
     uninstall_dictionary, migrate_dictionary, create_trie_index,\
     search, searchNode, reverse, version, dictionary_version,\
-    installed_dictionary_version
+    installed_dictionary_version, installed_dictionary_readme  # noqa: F401
```

### Comparing `jageocoder-1.4.1rc1/jageocoder/address.py` & `jageocoder-2.0.0/jageocoder/address.py`

 * *Files identical despite different names*

### Comparing `jageocoder-1.4.1rc1/jageocoder/exceptions.py` & `jageocoder-2.0.0/jageocoder/exceptions.py`

 * *Files identical despite different names*

### Comparing `jageocoder-1.4.1rc1/jageocoder/itaiji.py` & `jageocoder-2.0.0/jageocoder/itaiji.py`

 * *Files identical despite different names*

### Comparing `jageocoder-1.4.1rc1/jageocoder/itaiji_dic.json` & `jageocoder-2.0.0/jageocoder/itaiji_dic.json`

 * *Files identical despite different names*

### Comparing `jageocoder-1.4.1rc1/jageocoder/module.py` & `jageocoder-2.0.0/jageocoder/module.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import logging
 import os
-import tempfile
+import shutil
 from typing import Optional, Union, List
 import urllib.request
 from urllib.error import URLError
-import zipfile
 
 import jageocoder
 from jageocoder.exceptions import JageocoderError
 from jageocoder.tree import AddressTree, get_db_dir
 from jageocoder.result import Result
 
 _tree = None  # The default AddressTree
@@ -43,15 +42,15 @@
 
     debug: bool, Optional(default=False)
         Debugging flag.
     """
     global _tree
 
     if _tree:
-        _tree.close()
+        del _tree
 
     _tree = AddressTree(db_dir=db_dir, mode=mode, debug=debug)
     set_search_config(**kwargs)
 
 
 def free():
     """
@@ -169,80 +168,51 @@
     except (URLError, ValueError,):
         raise JageocoderError(
             "The dictionary file could not be downloaded"
             + " from the URL {}".format(url))
 
 
 def install_dictionary(
-        path_or_url: os.PathLike,
+        path: os.PathLike,
         db_dir: Optional[os.PathLike] = None) -> None:
     """
-    Install address-dictionary from the specified path or url.
+    Install address-dictionary from the specified path.
 
     Parameters
     ----------
-    path_or_url: os.PathLike
-        The file path or url where the zipped address-dictionary file
-        is available.
+    path: os.PathLike
+        The file path where the zipped address-dictionary file exists.
 
     db_dir: os.PathLike, optional
-        The directory where the database files will be installed.
-        If omitted, it will be determined by `get_db_dir()`.
+        The directory directory where the database files will
+        be installed.
+
+        If omitted, use `get_db_dir()` to decide the directory.
     """
     # Set default value
     if db_dir is None:
         db_dir = get_db_dir(mode='w')
 
-    # Open a local file
-    tmppath = None
-
-    if os.path.exists(path_or_url):
-        path = path_or_url
+    if os.path.exists(path):
+        path = path
     else:
-        try:
-            # Try to download a file
-            fp, path = tempfile.mkstemp()
-            os.close(fp)
-            logger.info(
-                'Downloading zipped dictionary from {}'.format(path_or_url))
-            urllib.request.urlretrieve(path_or_url, path)
-            logger.info('.. download complete.')
-            tmppath = path
-        except (URLError, ValueError,):
-            raise JageocoderError("Can't open file {}".format(path_or_url))
-
-    # Unzip the file
-    with zipfile.ZipFile(path) as zipf:
-        logger.info('Extracting {} to {}'.format(path, db_dir))
-        zipf.extract(member='address.db', path=db_dir)
-        try:
-            zipf.extract(member='README.txt', path=db_dir)
-            logger.info(
-                'Please check {} for terms and conditions of use.'.format(
-                    os.path.join(db_dir, 'README.txt')))
-        except KeyError:
-            pass
-
-    if tmppath:
-        os.remove(tmppath)
-
-    # Create trie-index
-    init(db_dir=db_dir, mode='a')
-    global _tree
-    if not _tree.is_version_compatible():
-        logger.warning(('Migrating the database file since'
-                        ' it is not compatible with the package.'))
-        _tree.update_name_index()
+        raise JageocoderError("Can't open file '{}'".format(path))
 
-    logger.info('Creating TRIE index at {}'.format(_tree.trie_path))
-    _tree.create_trie_index()
-
-    # Put metadata.txt
-    with open(os.path.join(db_dir, "metadata.txt"), "w") as f:
-        print(os.path.basename(path_or_url), file=f)
+    # Unzip the archive
+    shutil.rmtree(db_dir)
+    shutil.unpack_archive(
+        filename=str(path),
+        extract_dir=str(db_dir),
+    )
+    for readme_fname in ("README.txt", "README.md",):
+        readme_path = os.path.join(db_dir, readme_fname)
+        if os.path.exists(readme_path):
+            logger.info(
+                "Please read '{}' for terms and conditions of use.".format(
+                    readme_path))
 
     logger.info('Installation completed.')
 
 
 def uninstall_dictionary(db_dir: Optional[os.PathLike] = None) -> None:
     """
     Uninstall address-dictionary.
@@ -277,16 +247,16 @@
     # Set default value
     if db_dir is None:
         db_dir = get_db_dir(mode='a')
 
     # Update the name and trie index
     init(db_dir=db_dir, mode='a')
     global _tree
-    logger.info('Updating name index')
-    _tree.update_name_index()
+    # logger.info('Updating name index')
+    # _tree.update_name_index()
     logger.info('Updating TRIE index {}'.format(_tree.trie_path))
     _tree.create_trie_index()
     logger.info('The dictionary is successfully migrated.')
 
 
 def installed_dictionary_version(db_dir: Optional[os.PathLike] = None) -> str:
     """
@@ -415,23 +385,16 @@
 
 
 def reverse(x: float, y: float, level: Optional[int] = None) -> dict:
     """
     Reverse geocoding.
 
     """
-    if not is_initialized():
-        raise JageocoderError("Not initialized. Call 'init()' first.")
-    from jageocoder.rev import Reverse
-
-    global _tree
-    _reverse = Reverse(x=x, y=y, tree=_tree, max_level=level)
-    results = _reverse.search()
-
-    return results
+    raise JageocoderError(
+        "The 'reverse' method is not yet available in version 2.")
 
 
 def create_trie_index() -> None:
     """
     Create the TRIE index from the database file.
 
     This function is a shortcut for AddressTree.create_trie_index().
```

### Comparing `jageocoder-1.4.1rc1/jageocoder/node.py` & `jageocoder-2.0.0/jageocoder/node.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,193 +1,418 @@
+from __future__ import annotations
 from functools import lru_cache
 import json
 import logging
+import os
 import re
-from typing import List, Optional
+from typing import List, Optional, TYPE_CHECKING
 
-from sqlalchemy import Column, Float, ForeignKey, Integer, SmallInteger, String, Text
-from sqlalchemy import or_
-from sqlalchemy.orm import deferred
-from sqlalchemy.orm import backref, relationship
+from PortableTab import BaseTable
 
 from jageocoder.address import AddressLevel
-from jageocoder.aza_master import AzaMaster
-from jageocoder.base import Base, get_session
-from jageocoder.dataset import Dataset  #
+from jageocoder.dataset import Dataset
 from jageocoder.itaiji import Converter
 from jageocoder.result import Result
 from jageocoder.strlib import strlib
 
+if TYPE_CHECKING:
+    from jageocoder.tree import AddressTree
 
 logger = logging.getLogger(__name__)
 default_itaiji_converter = Converter()  # With default settings
 
 
-class AddressNode(Base):
+class AddressNodeTable(BaseTable):
+    """
+    The address node table.
     """
-    The address-node structure stored in 'node' table.
 
-    Attributes
+    __tablename__ = "address_node"
+    __schema__ = """
+        struct AddressNode {
+            id @0 :UInt32;
+            name @1 :Text;
+            nameIndex @2 :Text;
+            x @3 :Float32;
+            y @4 :Float32;
+            level @5 :Int8;
+            priority @6 :Int8;
+            note @7 :Text;
+            parentId @8 :UInt32;
+            siblingId @9 :UInt32;
+        }
+        """
+    __record_type__ = "AddressNode"
+
+    def __init__(self, db_dir: os.PathLike) -> None:
+        super().__init__(db_dir=db_dir)
+        self.datasets = Dataset(db_dir=db_dir)
+
+    @lru_cache(maxsize=1024)
+    def get_record(self, pos: int) -> AddressNode:
+        """
+        Get the record at the specified position
+        and convert it to AddressNode object.
+
+        Parameters
+        ----------
+        pos: int
+            The position.
+
+        Returns
+        -------
+        AddressNode
+            The converted object.
+        """
+        capnp_record = super().get_record(pos=pos)
+        node = AddressNode.from_record(capnp_record)
+        node.table = self
+        return node
+
+    def create_indexes(self) -> None:
+        """
+        Create TRIE index on "name" and "note" columns.
+        """
+        self.create_trie_on("nameIndex")
+        self.create_trie_on(
+            attr="note",
+            func=lambda x: re.split(r"\s*/\s*", x))
+
+
+class AddressNode(object):
+    """
+    The address node stored in 'address_node' table.
+
+    Parameters
     ----------
     id : int
         The key identifier that is automatically sequentially numbered.
     name : str
         The name of the address element, such as '東京都' or '新宿区'
-    name_index : str
-        The standardized string for indexing created from its name.
     x : float
         X-coordinate value. (Longitude)
     y : float
         Y-coordinate value. (Latitude)
     level : int
         The level of the address element.
         The meaning of each value is as follows.
     priority : int
         Priority assigned to each source of data.
         Smaller value indicates higher priority.
     note : string
         Note or comment.
     parent_id : int
         The id of the parent node.
-    children : list of AddressNode
-        The child nodes.
-    dataset : source dataset where the node come from.
-    """
-    __tablename__ = 'node'
+    sibling_id : int
+        The id of the next sibling node.
+
+    Attributes
+    ----------
+    name_index : str
+        The standardized string for indexing created from its name.
 
-    id = Column(Integer, primary_key=True)
-    name = deferred(Column(String(256), nullable=False))
-    name_index = Column(String(256), nullable=False)
-    x = deferred(Column(Float, nullable=True))
-    y = deferred(Column(Float, nullable=True))
-    level = Column(SmallInteger, nullable=True)
-    priority = Column(SmallInteger, ForeignKey('dataset.id'), nullable=True)
-    note = deferred(Column(Text, nullable=True))
-    parent_id = Column(Integer, ForeignKey('node.id'), nullable=True)
-    children = relationship(
-        "AddressNode",
-        cascade="all",
-        backref=backref("parent", remote_side="AddressNode.id"),
-        lazy="dynamic",
-    )
-    dataset = relationship(Dataset, cascade="all")
+    """
+    ROOT_NODE_ID = 0
 
-    def __init__(self, *args, **kwargs):
+    def __init__(
+            self,
+            id: Optional[int] = None,
+            name: Optional[str] = None,
+            name_index: Optional[str] = None,
+            x: Optional[float] = None,
+            y: Optional[float] = None,
+            level: Optional[int] = None,
+            priority: Optional[int] = None,
+            note: Optional[str] = None,
+            parent_id: Optional[int] = None,
+            sibling_id: Optional[int] = None,
+    ) -> None:
         """
         The initializer of the node.
 
         In addition to the initialization of the record,
         the name_index is also created.
         """
-        super().__init__(*args, **kwargs)
-        # Basic attributes
-        self.name = kwargs.get('name', '')
-
-        # Set extended attributes
-        self.set_attributes(**kwargs)
+        # Set basic attributes
+        self.id = id
+        self.name = name
+        self.name_index = name_index
+        self.x = x
+        self.y = y
+        self.level = level
+        self.priority = priority
+        self.note = note
+        self.parent_id = parent_id
+        self.sibling_id = sibling_id
 
         # For indexing
-        self.name_index = default_itaiji_converter.standardize(self.name)
+        if self.name_index is None:
+            self.name_index = default_itaiji_converter.standardize(self.name)
+
+        # Set relations
+        self.table = None
+
+    @property
+    def dataset(self):
+        """
+        Get dataset record.
+        """
+        return self.table.datasets.get(id=self.priority)
+
+    @classmethod
+    def from_record(cls, record) -> AddressNode:
+        """
+        East: 153°59'12″
+        West: 122°55'57″
+        South: 20°25'31″
+        North: 45°33'26″
+        """
+        return AddressNode(
+            id=record.id,
+            name=record.name,
+            name_index=record.nameIndex,
+            x=record.x,
+            y=record.y,
+            level=record.level,
+            priority=record.priority,
+            note=record.note,
+            parent_id=record.parentId,
+            sibling_id=record.siblingId,
+        )
+
+    def to_record(self):
+        x = float(self.x or 999.9)
+        y = float(self.y or 999.9)
 
-        # Relations
-        self.parent_id = kwargs.get('parent_id', None)
+        return {
+            "id": int(self.id),
+            "name": str(self.name or ""),
+            "nameIndex": str(self.name_index or ""),
+            "x": x if x <= 180.0 and x >= -180.0 else 999.9,
+            "y": y if y <= 90.0 and y >= -90.0 else 999.9,
+            "level": int(self.level or 0),
+            "priority": int(self.priority or 0),
+            "note": str(self.note or ""),
+            "parentId": int(self.parent_id or 0),
+            "siblingId": int(self.sibling_id or 0),
+        }
+
+    @classmethod
+    def root(cls) -> AddressNode:
+        return AddressNode(
+            id=cls.ROOT_NODE_ID,
+            name="_root_",
+            x=999.9,
+            y=999.9,
+            level=0,
+            priority=0,
+            note="",
+            parent_id=cls.ROOT_NODE_ID,
+        )
 
     def set_attributes(self, **kwargs):
         """
         Set attributes of this node by kwargs values.
         'name' can't be modified.
         """
         self.x = kwargs.get('x', kwargs.get('lon'))
         self.y = kwargs.get('y', kwargs.get('lat'))
         self.level = kwargs.get('level')
         self.priority = kwargs.get('priority', 99)
         self.note = kwargs.get('note', None)
 
-    def add_child(self, child):
-        """
-        Add a node as a child of this node.
+    @property
+    def parent(self) -> Optional[AddressNode]:
+        return self.get_parent()
 
-        Parameters
-        ----------
-        child : AddressNode
-            The node that will be a child node.
+    def get_parent(self) -> Optional[AddressNode]:
         """
-        self.children.append(child)
+        Get the parent node.
 
-    def add_to_parent(self, parent):
-        """
-        Add this node as a child of an other node.
+        Returns
+        -------
+        AddressNode
+            The parent.
 
-        Parameters
-        ----------
-        parent : AddressNode
-            The node that will be the parent.
+        Notes
+        -----
+        - Returns None if the current node is directly under the root node.
         """
-        self.parent = parent
+        if self.parent_id == self.__class__.ROOT_NODE_ID:
+            return None
+
+        parent = self.table.get_record(pos=self.parent_id)
+        return parent
 
-    def get_child(self, target_name: str):
+    def get_child(self, target_name: str) -> AddressNode:
         """
         Get a child node with the specified name.
 
         Parameters
         ----------
         target_name : str
             The name (or standardized name) of the target node.
 
         Return
         ------
         Returns the relevand node if it is found,
         or None if it is not.
         """
-        return self.children.filter(or_(
-            AddressNode.name == target_name,
-            AddressNode.name_index == target_name
-        )).one_or_none()
+        address_node = self.table.get_record(pos=self.id)
+        next_pos = self.id + 1
+        while next_pos < address_node.siblingId:
+            candidate = self.table.get_record(pos=next_pos)
+            if candidate.parentId != self.id:
+                next_pos += 1
+                continue
+
+            if candidate.name == target_name or \
+                    candidate.name_index == target_name:
+                child = AddressNode.from_record(candidate)
+                return child
+
+            next_pos = candidate.siblingId
+
+        return None
+
+    @property
+    def children(self) -> List[AddressNode]:
+        return self.get_children()
+
+    def get_children(self) -> List[AddressNode]:
+        """
+        Get all children of the node.
+
+        Returns
+        -------
+        List[AddressNode]
+        """
+        children = []
+        pos: int = self.id + 1
+        while pos < self.sibling_id:
+            node = self.table.get_record(pos=pos)
+            if node.parent_id == self.id:
+                children.append(node)
+                pos = node.sibling_id
+            else:
+                parent = self.table.get_record(pos=node.parent_id)
+                pos = parent.sibling_id
+
+        return children
 
-    @lru_cache(maxsize=512)
     def search_child_with_criteria(
             self,
             pattern: str,
+            min_candidate: Optional[str] = None,
+            gt_candidate: Optional[str] = None,
             max_level: Optional[int] = None,
             require_coordinates: bool = False):
-        conds = []
-        conds.append(AddressNode.name_index.like(pattern))
-        logger.debug("  conds: name_index LIKE '{}'".format(pattern))
+        """
+        Search for children nodes that satisfy the specified conditions.
 
+        Parameters
+        ----------
+        pattern: str
+            The regular expression that the child node's name must match.
+        min_candidate: str, optional
+            The smallest string that satisfies the condition
+            as the name of a child node.
+        gt_candidate: str, optional
+            The smallest string that exceeds the upper limit
+            that satisfies the condition as the name of a child node.
+        max_level: int, optional
+            Maximum level of child nodes; unlimited if None.
+        require_coordinates: bool [False]
+            If set to True, the child node must have valid coordinates.
+        """
+        logger.debug(f"Searching '{pattern}' under '{self.name}'({self.id})")
+        logger.debug(f"  cond.1: name_index match '{pattern}'")
         if max_level is not None:
-            conds.append(AddressNode.level <= max_level)
-            logger.debug("    and level <= {}".format(max_level))
+            logger.debug(f"  cond.2: level <= {max_level}")
+
+        if require_coordinates:
+            logger.debug("  cond.3: coordinates are required.")
+
+        re_pattern = re.compile(pattern)
+        address_node = self.table.get_record(pos=self.id)
+        children = []
+
+        if self.sibling_id == self.id + 1:  # No child
+            return []
+
+        # Find the range of IDs of nodes that satisfy the condition
+        lb: int = self.id + 1  # lower bound
+        if min_candidate is None:
+            next_pos = self.id
+        else:
+            # Use binary search
+            ub: int = address_node.sibling_id  # upper bound
+            cp: int = 0
+            candidate: AddressNode = None
+            while candidate is None or \
+                    ub > self.table.get_record(pos=lb).sibling_id:
+                cp = int((lb + ub) / 2)  # current position
+                candidate = self.table.get_record(pos=cp)
+                if candidate.parent_id != self.id:
+                    while candidate.parent_id != self.id:
+                        cp = candidate.parent_id
+                        candidate = self.table.get_record(pos=cp)
+
+                    if cp == lb and candidate.sibling_id < ub:
+                        cp = candidate.sibling_id
+                        candidate = self.table.get_record(pos=cp)
+
+                if candidate.name_index < min_candidate:
+                    lb = cp
+                else:
+                    ub = cp
+
+            next_pos = lb
+
+        # Scan all records in the range
+        while next_pos < address_node.sibling_id:
+            candidate = self.table.get_record(pos=next_pos)
+
+            if gt_candidate is not None and \
+                    candidate.name_index >= gt_candidate:
+                break
+
+            if re_pattern.match(candidate.name_index) and \
+                    (max_level is None or candidate.level <= max_level) and \
+                    (require_coordinates is False or candidate.y <= 90.0):
+                children.append(candidate)
+
+            next_pos = candidate.sibling_id
 
-        if require_coordinates is True:
-            conds.append(AddressNode.y < 90.0)
-            logger.debug("    and having valid coordinates")
-
-        filtered_children = self.children.filter(*conds).order_by(
-            AddressNode.id)
-        logger.debug("  -> {} found.".format(filtered_children.count()))
-        return filtered_children
+        logger.debug("  -> {} found.".format(len(children)))
+        return children
 
     def search_recursive(
-        self, index: str, tree: 'AddressTree',  # noqa
-        processed_nodes: Optional[List['AddressNode']] = None
+            self,
+            tree: AddressTree,
+            index: str,
+            processed_nodes: Optional[List[int]] = None
     ) -> List[Result]:
         """
         Search nodes recursively that match the specified address notation.
 
         Parameters
         ----------
+        tree: AddressTree
+            The tree containing this node.
         index : str
             The standardized address notation.
-        processed_nodes: List of AddressNode, optional
-            List of nodes that have already been processed
-            by TRIE search results
+        processed_nodes: List of the AddressNode's id, optional
+            List of node's id that have already been processed
+            by TRIE search results.
 
         Return
         ------
-        A list of relevant AddressNode.
+        List[AddressNode]
+            List of relevant AddressNode.
         """
         l_optional_prefix = tree.converter.check_optional_prefixes(index)
         optional_prefix = index[0: l_optional_prefix]
         index = index[l_optional_prefix:]
 
         logger.debug("node:{}, index:{}, optional_prefix:{}".format(
             self, index, optional_prefix))
@@ -195,36 +420,44 @@
             return [Result(self, optional_prefix, 0)]
 
         max_level = None
         v = strlib.get_number(index)
         if v['i'] > 0:
             # If it starts with a number,
             # look for a node that matches the numeric part exactly.
-            substr = '{}.%'.format(v['n'])
+            substr = str(v['n']) + r'\..*'
+            min_candidate = str(v['n']) + '.'
+            gt_candidate = str(v['n']) + '/'  # '/' is next char of '.'
         else:
             # If it starts with not a number,
             # look for a node with a maching first letter.
-            substr = index[0:1] + '%'
+            substr = re.escape(index[0:1]) + r'.*'
+            min_candidate = index[0:1]
+            gt_candidate = chr(ord(index[0:1]) + 1)
 
         if '字' in optional_prefix:
             max_level = AddressLevel.AZA
 
         filtered_children = self.search_child_with_criteria(
             pattern=substr,
+            min_candidate=min_candidate,
+            gt_candidate=gt_candidate,
             max_level=max_level,
             require_coordinates=tree.get_config('require_coordinates'))
 
         # Check if the index begins with an extra character of
         # the current node.
-        if filtered_children.count() == 0 and \
+        if len(filtered_children) == 0 and \
                 index[0] in tree.converter.extra_characters:
-            logger.debug("Beginning with an extra character: {}".format(
-                index[0]))
+            logger.debug((
+                "Remove the leading extra character '{}' and "
+                "search candidates again.").format(index[0]))
             candidates = self.search_recursive(
-                index=index[1:], tree=tree,
+                tree=tree,
+                index=index[1:],
                 processed_nodes=processed_nodes)
             if len(candidates) > 0:
                 new_candidates = []
                 for candidate in candidates:
                     new_candidate = Result(
                         candidate.node,
                         index[0] + candidate.matched,
@@ -232,58 +465,60 @@
                     new_candidates.append(new_candidate)
 
                 return new_candidates
 
             return []
 
         if logger.isEnabledFor(logging.DEBUG):
-            if filtered_children.count() == 0:
+            if len(filtered_children) == 0:
                 msg = 'No candidates. Children are; {}'.format(
-                    ','.join([x.name for x in self.children]))
+                    ','.join([x.name for x in self.get_children()]))
             else:
                 msg = 'Filtered children are; {}'.format(
                     ','.join([x.name for x in filtered_children]))
 
             logger.debug(msg)
 
         candidates = []
         for child in filtered_children:
-            if child in processed_nodes or []:
+            if processed_nodes is None or child.id in processed_nodes:
                 msg = "-> Skip {}({}) (already processed)."
                 logger.debug(msg.format(child.name, child.id))
                 continue
 
             logger.debug("-> comparing; {}".format(child.name_index))
             new_candidates = self._get_candidates_from_child(
+                tree=tree,
                 child=child,
                 index=index,
                 optional_prefix=optional_prefix,
-                tree=tree,
                 processed_nodes=processed_nodes)
 
             if len(new_candidates) > 0:
                 candidates += new_candidates
 
-        if self.level == AddressLevel.WARD and self.parent.name == '京都市':
+        parent_node = self.get_parent()
+        if self.level == AddressLevel.WARD and parent_node.name == '京都市':
             # Street name (通り名) support in Kyoto City
             # If a matching part of the search string is found in the
             # child nodes, the part before the name is skipped
             # as a street name.
-            for child in self.children:
+            for child in self.get_children():
                 pos = index.rfind(child.name_index)
                 if pos <= 0:
                     continue
 
                 offset = pos + len(child.name_index)
                 rest_index = index[offset:]
                 logger.debug(
                     "child:{} match {} chars".format(child, offset))
+                processed_nodes.append(child.id)
                 for cand in child.search_recursive(
-                        index=rest_index,
                         tree=tree,
+                        index=rest_index,
                         processed_nodes=processed_nodes):
                     candidates.append(Result(
                         cand[0],
                         optional_prefix +
                         index[0: offset] + cand[1],
                         l_optional_prefix +
                         len(child.name_index) + len(cand[1])))
@@ -291,21 +526,23 @@
         # Search for subnodes with queries excludes Aza-name candidates
         aza_skip = tree.get_config('aza_skip')
         omissible_index = ""   # Skip = off
         if aza_skip is True:   # Skip = on
             omissible_index = index
         elif aza_skip is None:  # Skip = auto
             omissible_index = self.get_omissible_index(
-                index, tree, processed_nodes)
+                tree=tree,
+                index=index,
+                processed_nodes=processed_nodes
+            )
 
         if omissible_index != "":
             msg = "Checking Aza-name, current_node:{}, processed:{}"
             logger.debug(msg.format(self, processed_nodes))
-            aza_positions = tree.converter.optional_aza_len(
-                index, 0)
+            aza_positions = tree.converter.optional_aza_len(index, 0)
             aza_positions.append(len(omissible_index))
             if len(index) in aza_positions:
                 aza_positions.remove(len(index))
 
             aza_positions.sort()
 
             for azalen in aza_positions:
@@ -314,16 +551,16 @@
 
                 msg = '"{}" in index "{}" can be optional.'
                 logger.debug(msg.format(index[:azalen], index))
                 # Note: Disable 'aza_skip' here not to perform
                 # repeated skip processing.
                 tree.set_config(aza_skip=False)
                 sub_candidates = self.search_recursive(
-                    index=index[azalen:],
                     tree=tree,
+                    index=index[azalen:],
                     processed_nodes=processed_nodes)
                 tree.set_config(aza_skip=aza_skip)
                 if sub_candidates[0].matched == '':
                     continue
 
                 for cand in sub_candidates:
                     if cand.node.level < AddressLevel.BLOCK and \
@@ -342,36 +579,38 @@
         if len(candidates) == 0:
             candidates = [Result(self, '', 0)]
 
         logger.debug("node:{} returns {}".format(self.name, candidates))
         return candidates
 
     def _get_candidates_from_child(
-            self, child: 'AddressNode',
-            index: str, optional_prefix: str,
-            tree: 'AddressTree',  # noqa
-            processed_nodes: List['AddressNode']) -> list:
+            self,
+            tree: AddressTree,
+            child: AddressNode,
+            index: str,
+            optional_prefix: str,
+            processed_nodes: List[AddressNode]) -> List[AddressNode]:
         """
         Get candidates from the child.
 
         Parameters
         ----------
+        tree: AddressTree
+            The tree containing this node.
         child: AddressNode
             The starting child node.
         index: str
             Standardized query string. Numeric characters are kept as
             original notation.
-        tree: AddressTree
-            The address tree.
         optional_prefix: str
             The option string that preceded the string passed by index.
 
         Returns
         -------
-        list
+        List[AddressNode]
             The list of candidates.
             Each element of the array has the matched AddressNode
             as the first element and the matched string
             as the second element.
         """
 
         match_len = tree.converter.match_len(index, child.name_index)
@@ -406,62 +645,63 @@
 
         candidates = []
         offset = match_len
         rest_index = index[offset:]
         l_optional_prefix = len(optional_prefix)
         logger.debug("child:{} match {} chars".format(child, offset))
         for cand in child.search_recursive(
-                index=rest_index,
                 tree=tree,
+                index=rest_index,
                 processed_nodes=processed_nodes):
             candidates.append(Result(
                 cand.node,
                 optional_prefix + index[0:match_len] + cand.matched,
                 l_optional_prefix + match_len + cand.nchars))
 
         return candidates
 
     def get_omissible_index(
             self,
+            tree: AddressTree,
             index: str,
-            tree: 'AddressTree',  # noqa
-            processed_nodes: List['AddressNode']) -> str:
+            processed_nodes: List[AddressNode]) -> str:
         """
         Obtains an optional leading substring from the search string index.
 
         Parameters
         ----------
+        tree: AddressTree
+            The tree containing this node.
         index: str
             Target string.
-        tree: AddressTree
-            Current working tree object.
         processed_nodes: List of AddressNode
             List of nodes that have already been processed
             by TRIE search results.
 
         Returns
         -------
         str
             The optional leading substring.
             If not omissible, an empty string is returned.
 
         Notes
         -----
-        Retrieve the lower address elements of this node
-        that have start_count_type is 1 from the aza_master.
-
-        If the name of the element is contained in the index,
-        the substring before the name is returned.
+        - Retrieve the lower address elements of this node
+          that have start_count_type is 1 from the aza_master.
+        - If the name of the element is contained in the index,
+          the substring before the name is returned.
         """
         if self.level < AddressLevel.CITY or \
                 self.level > AddressLevel.AZA:
             return ""
 
-        for node in processed_nodes or []:
-            if node.parent_id == self.parent_id:
+        for id in processed_nodes or []:
+            node = self.table.get_record(pos=id)
+            if node.parent_id == self.parent_id and \
+                    node.name_index != self.name_index:
                 logger.debug((
                     "Can't skip substring after '{}', "
                     "a sibling node {} had been selected").format(
                         self.name, node.name))
                 return ""
 
             elif node.parent_id == self.id:
@@ -474,42 +714,47 @@
         if self.level < AddressLevel.OAZA:
             target_prefix = self.get_city_jiscode()
         else:
             target_prefix = self.get_aza_code().rstrip('0')
 
         if target_prefix == "":
             logger.debug((
-                "Can't skip substring after '{}', "
-                "the node {} doesn't have city/aza code.").format(
-                    self.name, self.name))
-            return ""
+                "Consider '{}' is omissible, "
+                "since the node {} doesn't have city/aza code.").format(
+                    index, self.name))
+            return index
 
-        # self_names = self.get_fullname()
+        # Search sub-aza-records using TRIE index on "code"
+        logger.debug("Scanning sub aza-records in '{}'".format(index))
         omissible_index = index
-        for aza_row in tree.session.query(AzaMaster).filter(
-                AzaMaster.code.like('{}%'.format(target_prefix)),
-                AzaMaster.aza_class == 3,
-                AzaMaster.start_count_type == 1):
-
-            # logger.debug("Checking {}.".format(aza_row.names))
-
-            logger.debug("  -> {} is not omissible.".format(
-                aza_row.names))
-
-            names = json.loads(aza_row.names)
-            name = tree.converter.standardize(names[-1][1])
-            pos = omissible_index.find(name)
-            if pos >= 0:
+        aza_records = tree.aza_masters.search_records_on(
+            attr="code",
+            value=target_prefix,
+            funcname="keys"
+        )
+        for aza_record in aza_records:
+            if aza_record.azaClass == 3 and \
+                aza_record.startCountType == 1 or \
+                    aza_record.azaClass == 1:
+
+                names = json.loads(aza_record.names)
                 logger.debug(
-                    "Can't ommit substring '{}' in {}".format(
-                        names[-1][1], omissible_index))
-                omissible_index = omissible_index[0:pos]
-                if pos == 0:
-                    break
+                    "  -> '{}' is not omissible.".format(names[-1][1]))
+                name = tree.converter.standardize(names[-1][1])
+                pos = omissible_index.find(name)
+                if pos >= 0:
+                    logger.debug(
+                        "Can't omit substring '{}' from '{}' in {}".format(
+                            name, names[-1][1], omissible_index))
+                    omissible_index = omissible_index[0:pos]
 
+                    if pos == 0:
+                        break
+
+        logger.debug("  -> omissible '{}'".format(omissible_index))
         return omissible_index
 
     def save_recursive(self, session):
         """
         Add the node to the database recursively.
 
         Parameters
@@ -559,29 +804,29 @@
     def get_fullname(self):
         """
         Returns a complete address notation starting with the name of
         the prefecture.
         """
         names = []
         cur_node = self
-        while cur_node.parent:
+        while cur_node is not None:
             names.insert(0, cur_node.name)
-            cur_node = cur_node.parent
+            cur_node = cur_node.get_parent()
 
         return names
 
     def get_parent_list(self):
         """
         Returns a complete node list starting with the prefecture.
         """
         nodes = []
         cur_node = self
-        while cur_node.parent:
+        while cur_node is not None:
             nodes.insert(0, cur_node)
-            cur_node = cur_node.parent
+            cur_node = cur_node.get_parent()
 
         return nodes
 
     def get_nodes_by_level(self):
         """
         The function returns an array of this node and its upper nodes.
         The Nth node of the array contains the node corresponding
@@ -593,44 +838,44 @@
         >>> import jageocoder
         >>> jageocoder.init()
         >>> node = jageocoder.searchNode('多摩市落合1-15')[0][0]
         >>> [str(x) for x in node.get_node_array_by_level()]
         ['None', '[11460206:東京都(139.69164,35.6895)1(jisx0401:13)]', 'None', '[12063501:多摩市(139.446366,35.636959)3(jisx0402:13224)]', 'None',
                                 '[12065382:落合(139.427097,35.624877)5(None)]', '[12065383:一丁目(139.427097,35.624877)6(None)]', '[12065389:15番地(139.428969,35.625779)7(None)]']
         """  # noqa: E501
-        result = [None] * (self.level + 1)
+        result = [None for _ in range(self.level + 1)]
         cur_node = self
-        while cur_node.parent:
+        while cur_node is not None:
             result[cur_node.level] = cur_node
-            cur_node = cur_node.parent
+            cur_node = cur_node.get_parent()
 
         return result
 
     def __str__(self):
         return '[{}:{}({},{}){}({})]'.format(
             self.id, self.name, self.x, self.y, self.level, str(self.note))
 
     def __repr__(self):
         r = []
         cur_node = self
-        while cur_node.parent:
+        while cur_node is not None:
             r.insert(0, str(cur_node))
-            cur_node = cur_node.parent
+            cur_node = cur_node.get_parent()
 
         return '>'.join(r)
 
     def retrieve_upper_node(self, target_levels: List[int]):
         """
         Retrieves the node at the specified level from
         the this node or one of its upper nodes.
         """
         cur_node = self
-        while cur_node.parent and cur_node.level not in target_levels:
-            parent = cur_node.parent
-            cur_node = parent
+        while cur_node.id is not None and \
+                cur_node.level not in target_levels:
+            cur_node = cur_node.get_parent()
 
         if cur_node.level in target_levels:
             return cur_node
 
         return None
 
     def get_pref_name(self) -> str:
@@ -734,15 +979,15 @@
         node = self
         while True:
             if node.note and 'aza_id' in node.note:
                 m = re.search(r'aza_id:(\d{7})', node.note)
                 if m:
                     return m.group(1)
 
-            node = node.parent
+            node = node.get_parent()
             if node is None:
                 break
 
         return ''
 
     def get_aza_code(self) -> str:
         """
@@ -751,18 +996,26 @@
         """
         aza_id = self.get_aza_id()
         if aza_id != '':
             return self.get_city_jiscode() + aza_id
 
         return ''
 
-    def get_aza_names(self) -> list:
+    def get_aza_names(
+        self,
+        tree: AddressTree,
+    ) -> list:
         """
         Returns representation of Aza node containing this node.
 
+        Parameters
+        ----------
+        tree: AddressTree
+            The tree containing this node.
+
         Returns
         -------
         list
             A list containing notations from the prefecture level
             to the Aza level in the following format:
 
             [AddressLevel, Kanji, Kana, English, code]
@@ -770,37 +1023,36 @@
         if self.level >= AddressLevel.OAZA:
             code = self.get_aza_code()
         elif self.level >= AddressLevel.CITY:
             code = self.get_city_jiscode()
         else:
             code = self.get_pref_jiscode()
 
-        aza_record = AzaMaster.search_by_code(
-            code, get_session(self))
+        aza_record = tree.aza_masters.search_by_code(code)
         if aza_record:
             return json.loads(aza_record.names)
 
         return []
 
     def get_postcode(self) -> str:
         """
         Returns the 7digit postcode of the oaza that
         contains this node.
         """
         node = self
-        while True:
+        while node is not None:
             if node.level <= AddressLevel.COUNTY:
                 break
 
             if node.note and 'postcode' in node.note:
                 m = re.search(r'postcode:(\d{7})', node.note)
                 if m:
                     return m.group(1)
 
-            node = node.parent
+            node = node.get_parent()
 
         return ''
 
     def get_gsimap_link(self) -> str:
         """
         Returns the URL for GSI Map with parameters.
         ex. https://maps.gsi.go.jp/#13/35.713556/139.750385/
```

### Comparing `jageocoder-1.4.1rc1/jageocoder/result.py` & `jageocoder-2.0.0/jageocoder/result.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 import json
 from logging import getLogger
-from typing import NoReturn, Optional, Union, TYPE_CHECKING
+from typing import Optional, Union, TYPE_CHECKING
 
 if TYPE_CHECKING:
     from jageocoder.node import AddressNode
 
 logger = getLogger(__name__)
 
 
@@ -29,15 +29,15 @@
                  matched: str = '',
                  nchars: int = 0):
         self.node = node
         self.matched = matched
         self.nchars = nchars
 
     def set(self, node: AddressNode,
-            matched: str, nchars: int = 0) -> Result:
+            matched: str, nchars: int = 0) -> 'Result':
         """
         Set node and matched string.
         """
         self.node = node
         self.matched = matched
         self.matched = nchars or len(matched)
         return self
@@ -73,15 +73,15 @@
         elif pos == 1:
             return self.matched
         elif pos == 2:
             return self.nchars
 
         raise IndexError()
 
-    def __setitem__(self, pos, val: Union[AddressNode, str]) -> NoReturn:
+    def __setitem__(self, pos, val: Union[AddressNode, str]) -> None:
         from jageocoder.node import AddressNode
         if pos == 0 and isinstance(val, AddressNode):
             self.node = val
         elif pos == 1 and isinstance(val, str):
             self.matched = val
         elif pos == 2 and isinstance(val, int):
             self.nchars = val
```

### Comparing `jageocoder-1.4.1rc1/jageocoder/strlib.py` & `jageocoder-2.0.0/jageocoder/strlib.py`

 * *Files identical despite different names*

### Comparing `jageocoder-1.4.1rc1/jageocoder/tree.py` & `jageocoder-2.0.0/jageocoder/tree.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,91 +1,93 @@
 from collections import OrderedDict
 import csv
 from logging import getLogger
 import os
+from pathlib import Path
 import re
 import site
 import sys
-from typing import Any, Union, List, Optional, TextIO
+from typing import Any, Union, List, NoReturn, Optional, TextIO
 
 from deprecated import deprecated
-from sqlalchemy import Index
-from sqlalchemy.orm import sessionmaker, Session
-from sqlalchemy.orm.exc import NoResultFound
-from sqlalchemy.pool import NullPool
-from sqlalchemy import create_engine
-from sqlalchemy.exc import OperationalError
-from sqlalchemy.sql import text
 
 import jageocoder
 from jageocoder.address import AddressLevel
-from jageocoder.base import Base
+from jageocoder.aza_master import AzaMaster
 from jageocoder.exceptions import AddressTreeException
 from jageocoder.itaiji import Converter
-from jageocoder.node import AddressNode
-from jageocoder.note import NoteNode
+from jageocoder.node import AddressNode, AddressNodeTable
 from jageocoder.result import Result
 from jageocoder.trie import AddressTrie, TrieNode
 
 logger = getLogger(__name__)
 
 
-def get_db_dir(mode: str = 'r') -> os.PathLike:
+def get_db_dir(mode: str = 'r') -> Optional[Path]:
     """
     Get the database directory.
 
     Parameters
     ----------
     mode: str, optional(default='r')
         Specifies the mode for searching the database directory.
         If 'a' or 'w' is set, search a writable directory.
         If 'r' is set, search a database file that already exists.
 
     Return
     ------
-    The path to the database directory.
-    If no suitable directory is found, raise an AddressTreeException.
+    Path or None
+        The path to the database directory.
+        If no suitable directory is found, raise an AddressTreeException.
 
     Notes
     -----
     This method searches a directory in the following order of priority.
     - 'JAGEOCODER_DB_DIR' environment variable
-    - '(sys.prefix)/jageocoder/db/'
-    - '(site.USER_BASE)/jageocoder/db/'
+    - '(sys.prefix)/jageocoder/db2/'
+    - '(site.USER_BASE)/jageocoder/db2/'
     """
     if mode not in ('a', 'w', 'r'):
         raise AddressTreeException(
             'Invalid mode value. Specify one of "a", "w", or "r".')
 
-    db_dirs = []
-    if 'JAGEOCODER_DB_DIR' in os.environ:
-        db_dirs.append(os.environ['JAGEOCODER_DB_DIR'])
+    db_dirs: List[Path] = []
+    if 'JAGEOCODER_DB2_DIR' in os.environ:
+        db_dirs.append(Path(os.environ['JAGEOCODER_DB2_DIR']))
 
     db_dirs += [
-        os.path.join(sys.prefix, 'jageocoder/db/'),
-        os.path.join(site.USER_BASE, 'jageocoder/db/'),
+        Path(sys.prefix) / 'jageocoder/db2/',
+        Path(site.USER_BASE) / 'jageocoder/db2/',
     ]
 
     for db_dir in db_dirs:
-        path = os.path.join(db_dir, 'address.db')
-        if os.path.exists(path):
+        path = db_dir / 'address_node'
+        if path.exists():
             return db_dir
 
         if mode == 'r':
             continue
 
         try:
+            path = "__write_test__"
             os.makedirs(db_dir, mode=0o777, exist_ok=True)
-            fp = open(path, 'a')
-            fp.close()
+            with open(path, 'a') as fp:
+                fp.write("test")
+
+            os.remove(path)
             return db_dir
         except (FileNotFoundError, PermissionError):
             continue
 
-    return None
+    if mode in ('a', 'w',):
+        raise AddressTreeException(
+            "Cannot find a directory where the database can be created."
+        )
+
+    return None  # In case of read-only mode.
 
 
 class LRU(OrderedDict):
     'Limit size, evicting the least recently looked-up key when full'
 
     def __init__(self, maxsize=512, *args, **kwds):
         self.maxsize = maxsize
@@ -164,68 +166,47 @@
         debug: bool, optional (default=False)
             Debugging flag. If set to True, write debugging messages.
             If omitted, refer 'JAGEOCODER_DEBUG' environment variable,
             or False if the environment variable is also undefined.
         """
         # Set default values
         self.mode = mode
-        db_dir = db_dir or get_db_dir(mode)
         if db_dir is None:
-            msg = "Dictionary is not installed correctly."
-            raise AddressTreeException(msg)
+            db_dir = get_db_dir(mode)
         else:
-            db_dir = os.path.abspath(db_dir)
+            db_dir = Path(db_dir).absolute()
 
-        if not os.path.isdir(db_dir):
+        if db_dir is None or not db_dir.is_dir():
             msg = "Directory '{}' does not exist.".format(db_dir)
             raise AddressTreeException(msg)
 
-        self.db_path = os.path.join(db_dir, 'address.db')
-        self.dsn = 'sqlite:///' + self.db_path
-        self.trie_path = os.path.join(db_dir, 'address.trie')
+        self.db_dir = db_dir
+        self.address_nodes: AddressNodeTable = AddressNodeTable(
+            db_dir=self.db_dir)
+        self.aza_masters: AzaMaster = AzaMaster(db_dir=self.db_dir)
+        self.trie_nodes: TrieNode = self.get_trie_nodes()
+        self.trie_path = db_dir / 'address.trie'
 
         # Options
         self.debug = debug or bool(os.environ.get('JAGEOCODER_DEBUG', False))
 
-        # Clear database?
+        # Clear database when in write mode.
         if self.mode == 'w':
-            if os.path.exists(self.db_path):
-                os.remove(self.db_path)
-
+            self.address_nodes.delete()
             if os.path.exists(self.trie_path):
                 os.remove(self.trie_path)
 
-        # Database connection
-        self.engine = create_engine(
-            self.dsn, echo=self.debug,
-            connect_args={'check_same_thread': False},
-            poolclass=NullPool)
-        self.conn = self.engine.connect()
-        _session = sessionmaker()
-        _session.configure(bind=self.engine)
-        self.session = _session()
-
         self.root = None
         self.trie = AddressTrie(self.trie_path)
 
         # Regular expression
         self.re_float = re.compile(r'^\-?\d+\.?\d*$')
         self.re_int = re.compile(r'^\-?\d+$')
         self.re_address = re.compile(r'^(\d+);(.*)$')
 
-        # Check database version
-        if self.mode == 'w':
-            self.__create_db()
-
-        db_version = self.get_version()
-        if not self.is_version_compatible():
-            logger.warning((
-                "The database ({}) is not compatible with the module ({})."
-            ).format(db_version, jageocoder.dictionary_version()))
-
         # Set default settings
         self.config = {
             'debug': False,
             'aza_skip': None,
             'best_only': True,
             'target_area': [],
             'require_coordinates': True,
@@ -238,22 +219,16 @@
             'require_coordinates': os.environ.get(
                 'JAGEOCODER_REQUIRE_COORDINATES', True),
         })
 
         # Itaiji converter
         self.converter = Converter()
 
-    def close(self) -> None:
-        if self.session:
-            self.session.close()
-
-        if self.engine:
-            self.engine.dispose()
-            del self.engine
-            self.engine = None
+    def close(self) -> NoReturn:
+        raise RuntimeError("Unnecessary function close was called.")
 
     def is_version_compatible(self) -> bool:
         """
         Check if the dictionary version is compatible with the package.
 
         Returns
         -------
@@ -273,57 +248,28 @@
 
         If the mode is read-only, AddressTreeException will be raised.
         """
         if self.mode == 'r':
             raise AddressTreeException(
                 'This method is not available in read-only mode.')
 
-    def __create_db(self) -> None:
-        """
-        Create database and tables.
-        """
-        self.__not_in_readonly_mode()
-        Base.metadata.create_all(self.engine)
-        root = self.get_root()
-        root.save_recursive(self.session)
-        self.session.commit()
-
-    def get_session(self) -> Session:
-        """
-        Get the database session.
-
-        Returns
-        -------
-        sqlalchemy.orm.Session:
-            The current session object.
-        """
-        return self.session
-
     def get_root(self) -> AddressNode:
         """
         Get the root-node of the tree.
         If not set yet, create and get the node from the database.
 
         Returns
         -------
         AddressNode:
             The root node object.
         """
-        if self.root:
-            return self.root
-
-        # Try to get root from the database
-        try:
-            self.root = self.session.query(
-                AddressNode).filter_by(id=-1).one()
-        except NoResultFound:
-            # Create a new root
-            self.root = AddressNode(
-                id=-1, name="_root_", parent_id=None,
-                note=jageocoder.dictionary_version())
+        if self.root is None:
+            self.root = AddressNode.get(
+                tree=self,
+                pos=AddressNode.ROOT_NODE_ID)
 
         return self.root
 
     def get_version(self) -> str:
         """
         Get the version of the tree file.
 
@@ -347,15 +293,15 @@
         node_id: int
             The target node id.
 
         Return
         ------
         AddressNode
         """
-        return self.session.get(AddressNode, node_id)
+        return self.address_nodes.get_record(node_id)
 
     def search_nodes_by_codes(
             self,
             category: str,
             value: str) -> List[AddressNode]:
         """
         Search nodes by category and value.
@@ -369,19 +315,18 @@
         levels: List[int], optional
             The address levels of target nodes.
 
         Returns
         -------
         List[AddressNode]
         """
+        nodes = []
         pattern = '{}:{}'.format(category, value)
-        node_id_list = self.session.query(NoteNode.node_id).filter(
-            NoteNode.note == pattern).all()
-        nodes = self.session.query(AddressNode).filter(
-            AddressNode.id.in_(x[0] for x in node_id_list)).all()
+        nodes = self.address_nodes.search_records_on(
+            attr="note", value=pattern)  # exact match
 
         return nodes
 
     def get_node_fullname(self, node: Union[AddressNode, int]) -> List[str]:
         if isinstance(node, AddressNode):
             node_id = node.id
         else:
@@ -447,18 +392,17 @@
                 return
 
             # Check if the value is a name of node in the database.
             std = self.converter.standardize(value)
             candidates = self.trie.common_prefixes(std)
             if std in candidates:
                 trie_node_id = candidates[std]
-                trie_nodes = self.session.query(TrieNode).filter_by(
-                    trie_id=trie_node_id).all()
-                for trie_node in trie_nodes:
-                    if trie_node.node.name == value:
+                for node_id in self.trie_nodes.get_record(pos=trie_node_id).nodes:
+                    node = self.address_nodes.get_record(pos=node_id)
+                    if node.name == value:
                         return
 
             msg = "'{}' is not a valid value for {}.".format(value, key)
             raise RuntimeError(msg)
 
         else:
             return
@@ -864,29 +808,43 @@
         root_node = self.get_root()
         root_node.note = jageocoder.dictionary_version()
         self.session.add(root_node)
         self.session.commit()
 
         return diffs
 
+    def get_trie_nodes(self) -> TrieNode:
+        """
+        Get the TRIE node table.
+
+        Notes
+        -----
+        - Todo: If the trie index is not created, create.
+        """
+        return TrieNode(db_dir=self.db_dir)
+
     def create_trie_index(self) -> None:
         """
         Create the TRIE index from the tree.
         """
         self.__not_in_readonly_mode()
         self.index_table = {}
         logger.debug("Collecting labels for the trie index...")
         self._get_index_table()
         self._extend_index_table()
 
         logger.debug("Building Trie...")
         self.trie = AddressTrie(self.trie_path, self.index_table)
         self.trie.save()
 
-        self._set_index_table()
+        records = self._set_index_table()
+        # Create and write TrieNode table
+        self.trie_nodes = TrieNode(db_dir=self.db_dir)
+        self.trie_nodes.create()
+        self.trie_nodes.append_records(records)
 
     def _get_index_table(self) -> None:
         """
         Collect the names of all address elements
         to be registered in the TRIE index.
         The collected notations will be stored in `tree.index_table`.
 
@@ -894,36 +852,47 @@
         the prefecture to the name of the oaza without abbreviation,
         notations that omit the name of the prefecture, or notations
         that omit the name of the prefecture and the city.
         """
         # Build temporary lookup table
         logger.debug("Building temporary lookup table..")
         tmp_id_name_table = {}
-        for node in self.session.query(
-            AddressNode.id, AddressNode.name, AddressNode.name_index,
-            AddressNode.parent_id).filter(
-                AddressNode.level <= AddressLevel.OAZA):
-            tmp_id_name_table[node.id] = node
+        pos = AddressNode.ROOT_NODE_ID + 1
+        while pos < self.address_nodes.count_records():
+            node = self.address_nodes.get_record(pos=pos)
+            if node.level <= AddressLevel.OAZA:
+                tmp_id_name_table[node.id] = node
+                if node.level < AddressLevel.OAZA:
+                    pos += 1
+                else:
+                    pos = node.sibling_id
+
+            else:
+                parent = self.address_nodes.get_record(pos=node.parent_id)
+                if parent.level < AddressLevel.OAZA:
+                    pos += 1
+                else:
+                    pos = parent.sibling_id
+
+                continue
 
         logger.debug("  {} records found.".format(
             len(tmp_id_name_table)))
 
         # Create index_table
         self.index_table = {}
         for k, v in tmp_id_name_table.items():
             node_prefixes = []
             cur_node = v
             while True:
                 node_prefixes.insert(0, cur_node.name)
-                if cur_node.parent_id < 0:
+                if cur_node.parent_id == AddressNode.ROOT_NODE_ID:
                     break
 
                 if cur_node.parent_id not in tmp_id_name_table:
-                    import pdb
-                    pdb.set_trace()
                     raise RuntimeError(
                         ('The parent_id:{} of node:{} is not'.format(
                             cur_node.parent_id, cur_node),
                          ' in the tmp_id_table'))
 
                 cur_node = tmp_id_name_table[cur_node.parent_id]
 
@@ -944,35 +913,38 @@
                     continue
 
                 if candidate in self.index_table:
                     self.index_table[candidate].append(v.id)
                 else:
                     self.index_table[candidate] = [v.id]
 
-        # self.session.commit()
-
     def _extend_index_table(self) -> None:
         """
         Expand the index, including support for omission of county names.
         """
         # Build temporary lookup table
         logger.debug("Building temporary town and village table..")
         tmp_id_name_table = {}
-        for node in self.session.query(
-            AddressNode.id, AddressNode.name, AddressNode.name_index,
-            AddressNode.parent_id, AddressNode.level).filter(
-                AddressNode.level <= AddressLevel.CITY):
-            tmp_id_name_table[node.id] = node
+        pos = AddressNode.ROOT_NODE_ID + 1
+        while pos < self.address_nodes.count_records():
+            node = self.address_nodes.get_record(pos=pos)
+            if node.level <= AddressLevel.CITY:
+                tmp_id_name_table[node.id] = node
+                pos += 1
+            else:
+                parent = self.address_nodes.get_record(pos=node.parent_id)
+                pos = parent.sibling_id
+                continue
 
         logger.debug("  {} records found.".format(
             len(tmp_id_name_table)))
 
         # Extend index_table
         for k, v in tmp_id_name_table.items():
-            if v.parent_id == -1:
+            if v.parent_id == AddressNode.ROOT_NODE_ID:
                 continue
 
             parent_node = tmp_id_name_table[v.parent_id]
             if parent_node.level == AddressLevel.PREF:
                 continue
 
             pref_node = tmp_id_name_table[parent_node.parent_id]
@@ -982,55 +954,38 @@
             label = pref_node.name + v.name
             label_standardized = self.converter.standardize(label)
             if label_standardized in self.index_table:
                 self.index_table[label_standardized].append(v.id)
             else:
                 self.index_table[label_standardized] = [v.id]
 
-        # self.session.commit()
-
-    def _set_index_table(self) -> None:
+    def _set_index_table(self) -> list:
         """
         Map all the id of the TRIE index (TRIE id) to the node id.
 
         Collect notations recursively the names of all address elements
         which was registered in the TRIE index, retrieve
         the id of each notations in the TRIE index,
         then add the TrieNode to the database that maps
         the TRIE id to the node id.
         """
         logger.debug("Creating mapping table from trie_id:node_id")
-        logger.debug("  Deleting old TrieNode table...")
-        self.session.query(TrieNode).delete()
-        logger.debug("  Dropping index...")
-        try:
-            self.session.execute(text("DROP INDEX ix_trienode_trie_id"))
-            self.session.commit()
-        except OperationalError as e:  # noqa: F841
-            logger.debug("    the index does not exist. (ignored)")
-
-        logger.debug("  Adding mapping records...")
+        trie_nodes = []
         for k, node_id_list in self.index_table.items():
             trie_id = self.trie.get_id(k)
-            for node_id in node_id_list:
-                tn = TrieNode(trie_id=trie_id, node_id=node_id)
-                self.session.add(tn)
-
-        self.session.commit()
+            if len(trie_nodes) <= trie_id:
+                trie_nodes += [None for _ in range(
+                    trie_id - len(trie_nodes) + 1)]
+
+            trie_nodes[trie_id] = {
+                "id": trie_id,
+                "nodes": node_id_list,
+            }
 
-        logger.debug("  Creating index on trienode.trie_id ...")
-        trienode_trie_id_index = Index(
-            'ix_trienode_trie_id', TrieNode.trie_id)
-        try:
-            trienode_trie_id_index.create(self.engine)
-        except OperationalError as e:
-            logger.warning(e)
-            logger.debug("  the index already exists. (ignored)")
-
-        logger.debug("  done.")
+        return trie_nodes
 
     def save_all(self) -> None:
         """
         Save all AddressNode in the tree to the database.
         """
         self.__not_in_readonly_mode()
         logger.debug("Starting save full tree (recursive)...")
@@ -1139,41 +1094,14 @@
             for node in stocked:
                 self.session.add(node)
 
             self.session.commit()
 
         logger.debug("Done.")
 
-    def drop_indexes(self) -> None:
-        """
-        Drop indexes to improve the speed of bulk insertion.
-        - ix_node_parent_id ON node (parent_id)
-        - ix_trienode_trie_id ON trienode (trie_id)
-        """
-        self.__not_in_readonly_mode()
-        logger.debug("Dropping indexes...")
-        self.session.execute(text("DROP INDEX ix_node_parent_id"))
-        logger.debug("  done.")
-
-    def create_tree_index(self) -> None:
-        """
-        Add index later that were not initially defined.
-        - ix_node_parent_id ON node (parent_id)
-        """
-        self.__not_in_readonly_mode()
-        logger.debug("Creating index on node.parent_id ...")
-        node_parent_id_index = Index(
-            'ix_node_parent_id', AddressNode.parent_id)
-        try:
-            node_parent_id_index.create(self.engine)
-        except OperationalError:
-            logger.warning("  the index already exists. (ignored)")
-
-        logger.debug("  done.")
-
     def search_by_tree(self, address_names: List[str]) -> AddressNode:
         """
         Get the corresponding node id from the list of address element names,
         recursively search for child nodes using the tree.
 
         For example, ['東京都','新宿区','西新宿','二丁目'] will search
         the '東京都' node under the root node, search the '新宿区' node
@@ -1234,43 +1162,42 @@
 
         keys = sorted(candidates.keys(),
                       key=len, reverse=True)
 
         logger.debug("Trie: {}".format(','.join(keys)))
 
         min_key = ''
-        processed_nodes = []
+        processed_nodes: List[int] = []
 
         for k in keys:
             if len(k) < len(min_key):
                 logger.debug("Key '{}' is shorter than '{}'".format(
                     k, min_key))
                 continue
 
             trie_id = candidates[k]
             logger.debug("Trie_id of key '{}' = {}".format(
                 k, trie_id))
-            trienodes = self.session.query(
-                TrieNode).filter_by(trie_id=trie_id).all()
+            trie_node = self.trie_nodes.get_record(pos=trie_id)
             offset = self.converter.match_len(index, k)
             key = index[0:offset]
             rest_index = index[offset:]
-            for trienode in trienodes:
-                node = trienode.node
+            for node_id in trie_node.nodes:
+                node = self.get_address_node(id=node_id)
 
                 if min_key == '' and node.level <= AddressLevel.WARD:
                     # To make the process quicker, once a node higher
                     # than the city level is found, addresses shorter
                     # than the node are not searched after this.
                     logger.debug((
                         "A node with ward or higher levels found. "
                         "Set min_key to '{}'").format(k))
                     min_key = k
 
-                if node in processed_nodes:
+                if node_id in processed_nodes:
                     logger.debug("Node {}({}) already processed.".format(
                         node.name, node.id))
                     continue
 
                 if len(target_area) > 0:
                     # Check if the node is inside the specified area
                     for area in target_area:
@@ -1282,18 +1209,18 @@
                         msg = "Node {}({}) is not in the target area."
                         logger.debug(msg.format(node.name, node.id))
                         continue
 
                 logger.debug("Search '{}' under {}({})".format(
                     rest_index, node.name, node.id))
                 results_by_node = node.search_recursive(
-                    index=rest_index,
                     tree=self,
+                    index=rest_index,
                     processed_nodes=processed_nodes)
-                processed_nodes.append(node)
+                processed_nodes.append(node_id)
                 logger.debug('{}({}) marked as processed'.format(
                     node.name, node.id))
 
                 for cand in results_by_node:
                     if len(target_area) > 0:
                         for area in target_area:
                             inside = cand.node.is_inside(area)
@@ -1327,17 +1254,34 @@
                         results[cand.node.id] = [cand.node, key + cand[1]]
                         max_len = max(_len, max_len)
                         if min_part is None:
                             min_part = _part
                         else:
                             min_part = min(min_part, _part)
 
-        logger.debug(AddressNode.search_child_with_criteria.cache_info())
         return results
 
+    def get_address_node(self, id: int) -> AddressNode:
+        """
+        Get address node from the tree by its id.
+
+        Parameters
+        ----------
+        id: int
+            The node id.
+
+        Returns
+        -------
+        AddressNode
+            Node with the specified ID.
+        """
+        node = self.address_nodes.get_record(pos=id)
+        node.tree = self
+        return node
+
     @deprecated(('Renamed to `searchNode()` because it was confusing'
                  ' with jageocoder.search()'))
     def search(self, query: str, **kwargs) -> list:
         return self.searchNode(query, **kwargs)
 
     def searchNode(self, query: str) -> List[Result]:
         """
@@ -1449,63 +1393,19 @@
                 recovered = query[0:pos+1]
             elif query[-2:] in ('通り', '通リ'):
                 # '通' can be expressed as '通り'
                 recovered = query[0:pos+1]
 
         return recovered
 
-    def create_reverse_index(self) -> None:
-        """
-        Create table and index for reverse geocoding.
-        """
-        self.__not_in_readonly_mode()
-        logger.info("Creating aza table for reverse geocoding...")
-        sql = text("DROP TABLE IF EXISTS node_aza")
-        self.session.execute(sql)
-
-        sql = text("CREATE TABLE node_aza AS"
-                   " SELECT id, x, y, level FROM node"
-                   " WHERE level IN (:oaza, :aza)")
-        self.session.execute(sql, {
-            "oaza": AddressLevel.OAZA,
-            "aza": AddressLevel.AZA,
-        })
-
-        sql = text("CREATE INDEX idx_node_aza_x ON node_aza (x)")
-        self.session.execute(sql)
-
-        sql = text("CREATE INDEX idx_node_aza_y ON node_aza (y)")
-        self.session.execute(sql)
-
     def create_note_index_table(self) -> None:
         """
         Collect notes from all address elements and create
         search table with index.
         """
-        self.__not_in_readonly_mode()
-        logger.info("Creating note-node table...")
-        sql = text("DROP TABLE IF EXISTS {}".format(NoteNode.__table__))
-        self.session.execute(sql)
-        Base.metadata.create_all(
-            bind=self.engine,
-            tables=[NoteNode.__table__])
-
-        # Create correspondence records between a note and a node id.
-        for node in self.session.query(
-            AddressNode.id, AddressNode.note).filter(
-                AddressNode.note.isnot(None)):
-            for note in node.note.split('/'):
-                if note == '':
-                    continue
+        self.address_nodes.create_indexes()
 
-                notenode = NoteNode(node_id=node.id, note=note)
-                self.session.add(notenode)
-
-        logger.debug("  Creating index on notenode.note ...")
-        notenode_note_index = Index(
-            'ix_notenode_note', NoteNode.note)
-        try:
-            notenode_note_index.create(self.engine)
-        except OperationalError:
-            logger.debug("  the index already exists. (ignored)")
-
-        self.session.commit()
+    def get_cache_info(self) -> dict:
+        cache_info = {
+            "get_record": AddressNodeTable.get_record.cache_info(),
+        }
+        return cache_info
```

### Comparing `jageocoder-1.4.1rc1/jageocoder/trie.py` & `jageocoder-2.0.0/jageocoder/trie.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,44 @@
 from logging import getLogger
 import os
 
 import marisa_trie
-from sqlalchemy import Column, ForeignKey, Integer
-from sqlalchemy.orm import relationship
+from PortableTab import BaseTable
 
-from jageocoder.base import Base
 from jageocoder.exceptions import AddressTrieError
 
 logger = getLogger(__name__)
 
 
-class TrieNode(Base):
+class TrieNode(BaseTable):
     """
     The mapping-table of TRIE id and Node id. Stored in 'trienode' table.
 
     Attributes
     ----------
     id : int
-        The key identifier that is automatically sequentially numbered.
-    trie_id : int
-        TRIE id that corresponds one-to-one to a notation.
-    node_id : int
-        Node id that corresponds one-to-one to an AddressNode.
-    node : AddressNode
-        The node with node_id as its id.
+        The TRIE id.
+    nodes : List[int]
+        List of node id that corresponds to the TRIE id.
 
     Note
     ----
-    Some of the notations correspond to multiple address elements.
-    For example, "中央区中央" exists in either 千葉市 and 相模原市,
-    so TRIE id and Node id correspond one-to-many.
+    - Some of the notations correspond to multiple address elements.
+      For example, "中央区中央" exists in either 千葉市 and 相模原市,
+      so TRIE id and node id correspond one-to-many.
     """
 
     __tablename__ = 'trienode'
-
-    id = Column(Integer, primary_key=True)
-    trie_id = Column(Integer, nullable=False)
-    node_id = Column(Integer, ForeignKey('node.id'), nullable=False)
-
-    node = relationship("AddressNode")
+    __schema__ = """
+        struct TrieNode {
+            id @0 :UInt32;
+            nodes @1 :List(UInt32);
+        }
+        """
+    __record_type__ = "TrieNode"
 
 
 class AddressTrie(object):
     """
     Implementation of TRIE Index using marisa trie.
 
     Attributes
@@ -67,15 +62,15 @@
         ----------
         path : str
             Path to the TRIE file.
             Used both to open an existing file and to create a new file.
         words : dict (default : {})
             A dict whose key is the address notation to be registered.
         """
-        self.path = path
+        self.path = str(path)  # Marisa-trie uses string path
         self.trie = None
         self.words = words
 
         if os.path.exists(path):
             self.connect()
 
     def connect(self):
@@ -142,15 +137,17 @@
             The query string.
 
         Return
         ------
         A dict with a prefix string as key and a TRIE id as value.
         """
         if self.trie is None:
-            raise AddressTrieError('The trie-index is not created.')
+            raise AddressTrieError((
+                "The trie-index is not created."
+                "Try running 'jageocoder migrate-dictinary'"))
 
         results = {}
         for p in self.trie.iter_prefixes(query):
             results[p] = self.trie.key_id(p)
 
         return results
```

### Comparing `jageocoder-1.4.1rc1/pyproject.toml` & `jageocoder-2.0.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jageocoder"
-version = "1.4.1rc1"
+version = "2.0.0"
 description = "A Japanese-address geocoder for Python."
 authors = ["Takeshi Sagara <sagara@info-proto.com>"]
 repository = "https://github.com/t-sagara/jageocoder/"
 license = "The MIT License"
 readme = "README.md"
 documentation = "https://jageocoder.readthedocs.io/"
 packages = [
@@ -18,25 +18,29 @@
     "Programming Language :: Python :: 3",
 ]
 include = ["itaiji_dic.json"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 marisa-trie = "^0.7.8"
-SQLAlchemy = "^2.0.4"
 jaconv = "^0.3.4"
 docopt = "^0.6.2"
-geographiclib = "^2.0"
 deprecated = "^1.2.13"
 Werkzeug = ">=2.2.3"
+pycapnp = "^1.3.0"
+portabletab = "0.3.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 flake8 = "^5.0.0"
 twine = "^4.0.2"
+flask = "^2.2.3"
+flask-cors = "^3.0.10"
+sphinx = "<6.0.0"
+sphinx-rtd-theme = "^1.2.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 jageocoder = "jageocoder.__main__:main"
```

### Comparing `jageocoder-1.4.1rc1/PKG-INFO` & `jageocoder-2.0.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jageocoder
-Version: 1.4.1rc1
+Version: 2.0.0
 Summary: A Japanese-address geocoder for Python.
 Home-page: https://github.com/t-sagara/jageocoder/
 License: The MIT License
 Author: Takeshi Sagara
 Author-email: sagara@info-proto.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -15,21 +15,21 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
-Requires-Dist: SQLAlchemy (>=2.0.4,<3.0.0)
 Requires-Dist: Werkzeug (>=2.2.3)
 Requires-Dist: deprecated (>=1.2.13,<2.0.0)
 Requires-Dist: docopt (>=0.6.2,<0.7.0)
-Requires-Dist: geographiclib (>=2.0,<3.0)
 Requires-Dist: jaconv (>=0.3.4,<0.4.0)
 Requires-Dist: marisa-trie (>=0.7.8,<0.8.0)
+Requires-Dist: portabletab (==0.3.1)
+Requires-Dist: pycapnp (>=1.3.0,<2.0.0)
 Project-URL: Documentation, https://jageocoder.readthedocs.io/
 Project-URL: Repository, https://github.com/t-sagara/jageocoder/
 Description-Content-Type: text/markdown
 
 # jageocoder - A Python Japanese geocoder
 
 日本語版は README_ja.md をお読みください。
@@ -48,71 +48,51 @@
 {'matched': '新宿区西新宿2-8-', 'candidates': [{'id': 5961406, 'name': '8番', 'x': 139.691778, 'y': 35.689627, 'level': 7, 'note': None, 'fullname': ['東京都', '新宿区', '西新宿', '二丁目', '8番']}]}
 ```
 
 # How to install
 
 ## Prerequisites
 
-Requires Python 3.6.x or later.
+Requires Python 3.7.x or later.
 
-The following packages will be installed automatically.
-
-- [marisa-trie](https://pypi.org/project/marisa-trie/)
-    for building and retrieving TRIE index
-- [SQLAlchemy](https://pypi.org/project/SQLAlchemy/)
-    for abstracting access to the RDBMS
+All other required packages will be installed automatically.
 
 ## Install instructions
 
 - Install the package with `pip install jageocoder`
+- Download an address database file compatible with that version from 
+  [here](https://www.info-proto.com/static/jageocoder/latest/v2/)
 - Install the dictionary with `install-dictionary` command
 
 ```sh
 pip install jageocoder
-jageocoder install-dictionary
+wget https://www.info-proto.com/static/jageocoder/latest/v2/jukyo_all_v20.zip
+jageocoder install-dictionary jukyo_all_v20.zip
 ```
 
-The dictionary database will be created under
-`{sys.prefix}/jageocoder/db/`, or if the user doesn't have 
-write permission there `{site.USER_DATA}/jageocoder/db/`
-by default.
-
-If you need to know the location of the directory containing
-the dictionary database, perform `get-db-dir` command as follows,
-or call `jageocoder.get_db_dir()` in your script.
+The dictionary database will be installed under
+`{sys.prefix}/jageocoder/db2/` by default,
+however if the user doesn't have write permission there,
+`{site.USER_DATA}/jageocoder/db2/` instead.
+
+If you need to know the location of the dictionary directory,
+perform `get-db-dir` command as follows. (Or call
+`jageocoder.get_db_dir()` in your script)
 
 ```sh
 jageocoder get-db-dir
 ```
 
 If you prefer to create it in another location, set the environment
-variable `JAGEOCODER_DB_DIR` before executing `install_dictionary()`
+variable `JAGEOCODER_DB2_DIR` before executing `install_dictionary()`
 to specify the directory.
 
 ```sh
-export JAGEOCODER_DB_DIR='/usr/local/share/jageocoder/db'
-install-dictionary
-```
-
-## Migrate dictinary
-
-The `install-dictionary` command will download and install
-a version of the address dictionary file that is compatible with
-the currently installed jageocoder package.
-
-If you upgrade the jageocoder package after installing
-the address dictionary file, it may no longer be compatible with
-the installed address dictionary file.
-In which case you will need to reinstall or migrate the dictionary.
-
-To migrate the dictionary, run the `migrate-dictionary` command.
-This process may take a long time.
-
-```sh
-jageocoder migrate-dictionary
+export JAGEOCODER_DB2_DIR='/usr/local/share/jageocoder/db2'
+install-dictionary <db-file>
 ```
 
 ## Uninstall instructions
 
 Remove the directory containing the database, or perform 
 `uninstall-dictionary` command as follows.
 
@@ -134,21 +114,14 @@
 as a library and used by calling the API, but for testing purposes,
 you can check the geocoding results with the following command.
 
 ```sh
 jageocoder search 新宿区西新宿２－８－１
 ```
 
-If you want to look up an address from longitude and latitude,
-specify `reverse` instead of `search`.
-
-```sh
-jageocoder reverse 139.6917 35.6896
-```
-
 You can check the list of available commands with `--help`.
 
 ```sh
 jageocoder --help
 ```
 
 ## Using API
@@ -191,91 +164,15 @@
 - level: Address level (1:Prefecture, 2:County, 3:City and 23 district,
     4:Ward, 5:Oaza, 6:Aza and Chome, 7:Block, 8:Building)
 - note: Notes such as city codes
 - fullname: List of address notations from the prefecture level to this node
 
 ### Search for addresses by longitude and latitude
 
-Use `reverse()` to find addresses by longitude and latitude
-(so called 'reverse geocoding').
-
-The `reverse()` function returns the three addresses surrounding
-the specified longitude and latitude.
-(The results are formatted for better viewing)
-
-The `candidate` of each element contains information about
-the address node (AddressNode), and the `dist` contains
-the distance (geodesic distance, in meters)
-from the specified point to the representative point of the address.
-
-```
->>> jageocoder.reverse(139.6917, 35.6896)
-[
-  {
-    'candidate': {
-      'id': 12299330, 'name': '二丁目',
-      'x': 139.691774, 'y': 35.68945, 'level': 6,
-      'note': 'postcode:1600023',
-      'fullname': ['東京都', '新宿区', '西新宿', '二丁目']
-    },
-    'dist': 17.940303970792183
-  }, {
-    'candidate': {
-      'id': 12300198, 'name': '六丁目',
-      'x': 139.690969, 'y': 35.693426, 'level': 6,
-      'note': 'postcode:1600023',
-      'fullname': ['東京都', '新宿区', '西新宿', '六丁目']
-    },
-    'dist': 429.6327545403412
-  }, {
-    'candidate': {
-      'id': 12300498, 'name': '四丁目',
-      'x': 139.68762, 'y': 35.68754, 'level': 6,
-      'note': 'postcode:1600023',
-      'fullname': ['東京都', '新宿区', '西新宿', '四丁目']
-    },
-    'dist': 434.31591285255234
-  }
-]
-```
-
-If the `level` optional parameter is specified,
-it will return a more detailed address.
-However, it takes time to calculate.
-
-```
->>> jageocoder.reverse(139.6917, 35.6896, level=7)
-[
-  {
-    'candidate': {
-      'id': 12299340, 'name': '8番',
-      'x': 139.691778, 'y': 35.689627, 'level': 7,
-      'note': None,
-      'fullname': ['東京都', '新宿区', '西新宿', '二丁目', '8番']
-    },
-    'dist': 7.669497303543382
-  }, {
-    'candidate': {
-      'id': 12299330, 'name': '二丁目',
-      'x': 139.691774, 'y': 35.68945, 'level': 6,
-      'note': 'postcode:1600023',
-      'fullname': ['東京都', '新宿区', '西新宿', '二丁目']
-    },
-    'dist': 17.940303970792183
-  }, {
-    'candidate': {
-      'id': 12300588, 'name': '15番',
-      'x': 139.688172, 'y': 35.689264, 'level': 7,
-      'note': None,
-      'fullname': ['東京都', '新宿区', '西新宿', '四丁目', '15番']
-    },
-    'dist': 321.50874020809823
-  }
-]
-```
+Note: This method is not available in v2 series.
 
 ### Explore the attribute information of an address
 
 Use `searchNode()` to retrieve information about an address.
 
 This function returns a list of type `jageocoder.result.Result` .
 You can access the address node from node element of the Result object.
@@ -362,44 +259,17 @@
 ```
 >>> parent.children
 <sqlalchemy.orm.dynamic.AppenderQuery object at 0x7fbc08404b38>
 >>> [child.name for child in parent.children]
 ['10番', '11番', '1番', '2番', '3番', '4番', '5番', '6番', '7番', '8番', '9番']
 ```
 
-# For developers
-
-## Running the unittests
-
-```sh
-python -m unittest
-``` 
-
-`tests.test_search` tests for some special address notations.
-
-- Street address in Sapporo city such as '北3西1' for '北三条西一丁目'
-- Toorina in Kyoto city such as '下立売通新町西入薮ノ内町' for '薮ノ内町'
-
 ## Create your own dictionary
 
-Please use the dictionary coverter
-[jageocoder-converter](https://github.com/t-sagara/jageocoder-converter).
-
-## Sample Web Application
-
-A sample of a simple web app using Flask is available under
-`flask-demo`.
-
-Perform the following steps. Then, access port 5000.
-
-```
-cd flask-demo
-pip install flask flask-cors
-bash run.sh
-```
+Consider using [jageocoder-converter](https://github.com/t-sagara/jageocoder-converter).
 
 ## ToDos
 
 - Supporting address changes
 
     The functionality to handle address changes due to municipal consolidation, etc.
     has already been implemented in the C++ version, but will be implemented
```

