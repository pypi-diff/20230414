# Comparing `tmp/pysparkler-0.4.dev1681490474.tar.gz` & `tmp/pysparkler-0.4.dev1681497870.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysparkler-0.4.dev1681490474.tar", max compression
+gzip compressed data, was "pysparkler-0.4.dev1681497870.tar", max compression
```

## Comparing `pysparkler-0.4.dev1681490474.tar` & `pysparkler-0.4.dev1681497870.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     8862 2023-04-14 16:41:07.230337 pysparkler-0.4.dev1681490474/README.md
--rw-r--r--   0        0        0     1203 2023-04-14 16:41:14.658326 pysparkler-0.4.dev1681490474/pyproject.toml
--rw-r--r--   0        0        0      807 2023-04-14 16:41:07.230337 pysparkler-0.4.dev1681490474/pysparkler/__init__.py
--rw-r--r--   0        0        0     4258 2023-04-14 16:41:07.234337 pysparkler-0.4.dev1681490474/pysparkler/api.py
--rw-r--r--   0        0        0     5879 2023-04-14 16:41:07.234337 pysparkler-0.4.dev1681490474/pysparkler/base.py
--rw-r--r--   0        0        0     5734 2023-04-14 16:41:07.234337 pysparkler-0.4.dev1681490474/pysparkler/cli.py
--rw-r--r--   0        0        0    10520 2023-04-14 16:41:07.234337 pysparkler-0.4.dev1681490474/pysparkler/pyspark_24_to_30.py
--rw-r--r--   0        0        0     3967 2023-04-14 16:41:07.234337 pysparkler-0.4.dev1681490474/pysparkler/pyspark_31_to_32.py
--rw-r--r--   0        0        0     4413 2023-04-14 16:41:07.234337 pysparkler-0.4.dev1681490474/pysparkler/pyspark_32_to_33.py
--rw-r--r--   0        0        0     9741 1970-01-01 00:00:00.000000 pysparkler-0.4.dev1681490474/PKG-INFO
+-rw-r--r--   0        0        0     8895 2023-04-14 18:44:23.728667 pysparkler-0.4.dev1681497870/README.md
+-rw-r--r--   0        0        0     1203 2023-04-14 18:44:31.108843 pysparkler-0.4.dev1681497870/pyproject.toml
+-rw-r--r--   0        0        0      807 2023-04-14 18:44:23.728667 pysparkler-0.4.dev1681497870/pysparkler/__init__.py
+-rw-r--r--   0        0        0     4374 2023-04-14 18:44:23.728667 pysparkler-0.4.dev1681497870/pysparkler/api.py
+-rw-r--r--   0        0        0     5879 2023-04-14 18:44:23.728667 pysparkler-0.4.dev1681497870/pysparkler/base.py
+-rw-r--r--   0        0        0     5734 2023-04-14 18:44:23.728667 pysparkler-0.4.dev1681497870/pysparkler/cli.py
+-rw-r--r--   0        0        0     2204 2023-04-14 18:44:23.728667 pysparkler-0.4.dev1681497870/pysparkler/pyspark_23_to_24.py
+-rw-r--r--   0        0        0    10520 2023-04-14 18:44:23.728667 pysparkler-0.4.dev1681497870/pysparkler/pyspark_24_to_30.py
+-rw-r--r--   0        0        0     3967 2023-04-14 18:44:23.728667 pysparkler-0.4.dev1681497870/pysparkler/pyspark_31_to_32.py
+-rw-r--r--   0        0        0     4413 2023-04-14 18:44:23.728667 pysparkler-0.4.dev1681497870/pysparkler/pyspark_32_to_33.py
+-rw-r--r--   0        0        0     9774 1970-01-01 00:00:00.000000 pysparkler-0.4.dev1681497870/PKG-INFO
```

### Comparing `pysparkler-0.4.dev1681490474/README.md` & `pysparkler-0.4.dev1681497870/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # PySparkler
 
 ## About
 
-PySparkler is a tool that upgrades your PySpark scripts to Spark 3.3. It is a command line tool that takes a PySpark
-script as input and outputs a Spark 3.3 compatible script. It is written in Python and uses the
+PySparkler is a tool that upgrades your PySpark scripts to latest Spark version. It is a command line tool that takes a
+PySpark script as input and outputs a latest Spark version compatible script. It is written in Python and uses the
 [LibCST](https://github.com/Instagram/LibCST) module to parse the input script and generate the output script.
 
 ## Basic Usage
 
 Install from PyPI:
 
 ```bash
@@ -27,16 +27,16 @@
 
 | Migration                                       | Supported | Details                                                                                                                                      |
 |-------------------------------------------------|-----------|----------------------------------------------------------------------------------------------------------------------------------------------|
 | Upgrading from PySpark 3.3 to 3.4               | ❌         | [Link](https://spark.apache.org/docs/latest/api/python/migration_guide/pyspark_upgrade.html#upgrading-from-pyspark-3-3-to-3-4)               |
 | Upgrading from PySpark 3.2 to 3.3               | ✅         | [Link](https://spark.apache.org/docs/latest/api/python/migration_guide/pyspark_upgrade.html#upgrading-from-pyspark-3-2-to-3-3)               |
 | Upgrading from PySpark 3.1 to 3.2               | ✅         | [Link](https://spark.apache.org/docs/latest/api/python/migration_guide/pyspark_upgrade.html#upgrading-from-pyspark-3-1-to-3-2)               |
 | Upgrading from PySpark 2.4 to 3.0               | ✅         | [Link](https://spark.apache.org/docs/latest/api/python/migration_guide/pyspark_upgrade.html#upgrading-from-pyspark-2-4-to-3-0)               |
-| Upgrading from PySpark 2.3 to 2.4               | ❌         | [Link](https://spark.apache.org/docs/latest/api/python/migration_guide/pyspark_upgrade.html#upgrading-from-pyspark-2-3-to-2-4)               |
-| Upgrading from PySpark 2.3.0 to 2.3.1 and above | ❌         | [Link](https://spark.apache.org/docs/latest/api/python/migration_guide/pyspark_upgrade.html#upgrading-from-pyspark-2-3-0-to-2-3-1-and-above) |
+| Upgrading from PySpark 2.3 to 2.4               | ✅         | [Link](https://spark.apache.org/docs/latest/api/python/migration_guide/pyspark_upgrade.html#upgrading-from-pyspark-2-3-to-2-4)               |
+| Upgrading from PySpark 2.3.0 to 2.3.1 and above | ✅         | [Link](https://spark.apache.org/docs/latest/api/python/migration_guide/pyspark_upgrade.html#upgrading-from-pyspark-2-3-0-to-2-3-1-and-above) |
 | Upgrading from PySpark 2.2 to 2.3               | ❌         | [Link](https://spark.apache.org/docs/latest/api/python/migration_guide/pyspark_upgrade.html#upgrading-from-pyspark-2-2-to-2-3)               |
 | Upgrading from PySpark 1.4 to 1.5               | ❌         | [Link](https://spark.apache.org/docs/latest/api/python/migration_guide/pyspark_upgrade.html#upgrading-from-pyspark-1-4-to-1-5)               |
 | Upgrading from PySpark 1.0-1.2 to 1.3           | ❌         | [Link](https://spark.apache.org/docs/latest/api/python/migration_guide/pyspark_upgrade.html#upgrading-from-pyspark-1-0-1-2-to-1-3)           |
 
 ## Features Supported
 
 The tool supports the following features:
@@ -60,16 +60,16 @@
 
 ```bash
 pysparkler upgrade --input-file /path/to/script.py --output-file /path/to/output.py
 ```
 
 ### Upgrade PySpark Jupyter Notebook
 
-The tool can upgrade a PySpark Jupyter Notebook to Spark 3.3. It takes the path to the notebook as input and upgrades
-it in place:
+The tool can upgrade a PySpark Jupyter Notebook to latest Spark version. It takes the path to the notebook as input and
+upgrades it in place:
 
 ```bash
 pysparkler upgrade --input-file /path/to/notebook.ipynb
 ```
 
 Similar to upgrading python scripts, if you want to output the upgraded notebook to a different directory, you can use
 the `--output-file` flag:
@@ -181,16 +181,16 @@
 make test PYTEST_ARGS="-v"
 ```
 
 ## Architecture
 
 ### Why LibCST?
 
-LibCST is a Python library that provides a concrete syntax tree (CST) for Python code. CST preserves even the whitespaces
-of the source code which is very important since we only want to modify the code and not the formatting.
+LibCST is a Python library that provides a concrete syntax tree (CST) for Python code. CST preserves even the
+whitespaces of the source code which is very important since we only want to modify the code and not the formatting.
 
 ### How does it work?
 
 Using the codemod module of LibCST can simplify the process of writing a PySpark migration script, as it allows us to
 write small, reusable transformers and chain them together to perform a sequence of transformations.
 
 ### Why Transformer Codemod? Why not Visitor?
```

### Comparing `pysparkler-0.4.dev1681490474/pyproject.toml` & `pysparkler-0.4.dev1681497870/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysparkler"
-version = "0.4.dev1681490474"
+version = "0.4.dev1681497870"
 description = "A tool that upgrades your PySpark scripts to the latest Spark version as per Spark migration Guideline"
 authors = ["Dhruv Pratap <dhruv.pratap@gmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/holdenk/spark-upgrade"
 repository = "https://github.com/holdenk/spark-upgrade"
 maintainers = [
```

### Comparing `pysparkler-0.4.dev1681490474/pysparkler/__init__.py` & `pysparkler-0.4.dev1681497870/pysparkler/__init__.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.4.dev1681490474/pysparkler/api.py` & `pysparkler-0.4.dev1681497870/pysparkler/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 #  under the License.
 #
 import json
 
 import libcst as cst
 import nbformat
 
+from pysparkler.pyspark_23_to_24 import pyspark_23_to_24_transformers
 from pysparkler.pyspark_24_to_30 import pyspark_24_to_30_transformers
 from pysparkler.pyspark_31_to_32 import pyspark_31_to_32_transformers
 from pysparkler.pyspark_32_to_33 import pyspark_32_to_33_transformers
 
 
 class PySparkler:
     """Main class for PySparkler"""
@@ -34,14 +35,15 @@
         self.from_pyspark = from_pyspark
         self.to_pyspark = to_pyspark
         self.dry_run = dry_run
 
     @property
     def transformers(self):
         return [
+            *pyspark_23_to_24_transformers(),
             *pyspark_24_to_30_transformers(),
             *pyspark_31_to_32_transformers(),
             *pyspark_32_to_33_transformers(),
         ]
 
     def upgrade_script(self, input_file: str, output_file: str | None = None) -> str:
         """Upgrade a PySpark Python script file to the latest version and provides comments as hints for manual
```

### Comparing `pysparkler-0.4.dev1681490474/pysparkler/base.py` & `pysparkler-0.4.dev1681497870/pysparkler/base.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.4.dev1681490474/pysparkler/cli.py` & `pysparkler-0.4.dev1681497870/pysparkler/cli.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.4.dev1681490474/pysparkler/pyspark_24_to_30.py` & `pysparkler-0.4.dev1681497870/pysparkler/pyspark_24_to_30.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.4.dev1681490474/pysparkler/pyspark_31_to_32.py` & `pysparkler-0.4.dev1681497870/pysparkler/pyspark_31_to_32.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.4.dev1681490474/pysparkler/pyspark_32_to_33.py` & `pysparkler-0.4.dev1681497870/pysparkler/pyspark_32_to_33.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.4.dev1681490474/PKG-INFO` & `pysparkler-0.4.dev1681497870/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysparkler
-Version: 0.4.dev1681490474
+Version: 0.4.dev1681497870
 Summary: A tool that upgrades your PySpark scripts to the latest Spark version as per Spark migration Guideline
 Home-page: https://github.com/holdenk/spark-upgrade
 License: Apache-2.0
 Author: Dhruv Pratap
 Author-email: dhruv.pratap@gmail.com
 Maintainer: Holden Karau
 Maintainer-email: holden@pigscanfly.ca
@@ -20,16 +20,16 @@
 Project-URL: Repository, https://github.com/holdenk/spark-upgrade
 Description-Content-Type: text/markdown
 
 # PySparkler
 
 ## About
 
-PySparkler is a tool that upgrades your PySpark scripts to Spark 3.3. It is a command line tool that takes a PySpark
-script as input and outputs a Spark 3.3 compatible script. It is written in Python and uses the
+PySparkler is a tool that upgrades your PySpark scripts to latest Spark version. It is a command line tool that takes a
+PySpark script as input and outputs a latest Spark version compatible script. It is written in Python and uses the
 [LibCST](https://github.com/Instagram/LibCST) module to parse the input script and generate the output script.
 
 ## Basic Usage
 
 Install from PyPI:
 
 ```bash
@@ -49,16 +49,16 @@
 
 | Migration                                       | Supported | Details                                                                                                                                      |
 |-------------------------------------------------|-----------|----------------------------------------------------------------------------------------------------------------------------------------------|
 | Upgrading from PySpark 3.3 to 3.4               | ❌         | [Link](https://spark.apache.org/docs/latest/api/python/migration_guide/pyspark_upgrade.html#upgrading-from-pyspark-3-3-to-3-4)               |
 | Upgrading from PySpark 3.2 to 3.3               | ✅         | [Link](https://spark.apache.org/docs/latest/api/python/migration_guide/pyspark_upgrade.html#upgrading-from-pyspark-3-2-to-3-3)               |
 | Upgrading from PySpark 3.1 to 3.2               | ✅         | [Link](https://spark.apache.org/docs/latest/api/python/migration_guide/pyspark_upgrade.html#upgrading-from-pyspark-3-1-to-3-2)               |
 | Upgrading from PySpark 2.4 to 3.0               | ✅         | [Link](https://spark.apache.org/docs/latest/api/python/migration_guide/pyspark_upgrade.html#upgrading-from-pyspark-2-4-to-3-0)               |
-| Upgrading from PySpark 2.3 to 2.4               | ❌         | [Link](https://spark.apache.org/docs/latest/api/python/migration_guide/pyspark_upgrade.html#upgrading-from-pyspark-2-3-to-2-4)               |
-| Upgrading from PySpark 2.3.0 to 2.3.1 and above | ❌         | [Link](https://spark.apache.org/docs/latest/api/python/migration_guide/pyspark_upgrade.html#upgrading-from-pyspark-2-3-0-to-2-3-1-and-above) |
+| Upgrading from PySpark 2.3 to 2.4               | ✅         | [Link](https://spark.apache.org/docs/latest/api/python/migration_guide/pyspark_upgrade.html#upgrading-from-pyspark-2-3-to-2-4)               |
+| Upgrading from PySpark 2.3.0 to 2.3.1 and above | ✅         | [Link](https://spark.apache.org/docs/latest/api/python/migration_guide/pyspark_upgrade.html#upgrading-from-pyspark-2-3-0-to-2-3-1-and-above) |
 | Upgrading from PySpark 2.2 to 2.3               | ❌         | [Link](https://spark.apache.org/docs/latest/api/python/migration_guide/pyspark_upgrade.html#upgrading-from-pyspark-2-2-to-2-3)               |
 | Upgrading from PySpark 1.4 to 1.5               | ❌         | [Link](https://spark.apache.org/docs/latest/api/python/migration_guide/pyspark_upgrade.html#upgrading-from-pyspark-1-4-to-1-5)               |
 | Upgrading from PySpark 1.0-1.2 to 1.3           | ❌         | [Link](https://spark.apache.org/docs/latest/api/python/migration_guide/pyspark_upgrade.html#upgrading-from-pyspark-1-0-1-2-to-1-3)           |
 
 ## Features Supported
 
 The tool supports the following features:
@@ -82,16 +82,16 @@
 
 ```bash
 pysparkler upgrade --input-file /path/to/script.py --output-file /path/to/output.py
 ```
 
 ### Upgrade PySpark Jupyter Notebook
 
-The tool can upgrade a PySpark Jupyter Notebook to Spark 3.3. It takes the path to the notebook as input and upgrades
-it in place:
+The tool can upgrade a PySpark Jupyter Notebook to latest Spark version. It takes the path to the notebook as input and
+upgrades it in place:
 
 ```bash
 pysparkler upgrade --input-file /path/to/notebook.ipynb
 ```
 
 Similar to upgrading python scripts, if you want to output the upgraded notebook to a different directory, you can use
 the `--output-file` flag:
@@ -203,16 +203,16 @@
 make test PYTEST_ARGS="-v"
 ```
 
 ## Architecture
 
 ### Why LibCST?
 
-LibCST is a Python library that provides a concrete syntax tree (CST) for Python code. CST preserves even the whitespaces
-of the source code which is very important since we only want to modify the code and not the formatting.
+LibCST is a Python library that provides a concrete syntax tree (CST) for Python code. CST preserves even the
+whitespaces of the source code which is very important since we only want to modify the code and not the formatting.
 
 ### How does it work?
 
 Using the codemod module of LibCST can simplify the process of writing a PySpark migration script, as it allows us to
 write small, reusable transformers and chain them together to perform a sequence of transformations.
 
 ### Why Transformer Codemod? Why not Visitor?
```

