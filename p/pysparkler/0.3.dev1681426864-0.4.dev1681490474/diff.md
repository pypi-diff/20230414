# Comparing `tmp/pysparkler-0.3.dev1681426864.tar.gz` & `tmp/pysparkler-0.4.dev1681490474.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysparkler-0.3.dev1681426864.tar", max compression
+gzip compressed data, was "pysparkler-0.4.dev1681490474.tar", max compression
```

## Comparing `pysparkler-0.3.dev1681426864.tar` & `pysparkler-0.4.dev1681490474.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     4137 2023-04-13 23:00:57.465993 pysparkler-0.3.dev1681426864/README.md
--rw-r--r--   0        0        0     1188 2023-04-13 23:01:04.589201 pysparkler-0.3.dev1681426864/pyproject.toml
--rw-r--r--   0        0        0      807 2023-04-13 23:00:57.465993 pysparkler-0.3.dev1681426864/pysparkler/__init__.py
--rw-r--r--   0        0        0     4258 2023-04-13 23:00:57.465993 pysparkler-0.3.dev1681426864/pysparkler/api.py
--rw-r--r--   0        0        0     5879 2023-04-13 23:00:57.465993 pysparkler-0.3.dev1681426864/pysparkler/base.py
--rw-r--r--   0        0        0     5681 2023-04-13 23:00:57.465993 pysparkler-0.3.dev1681426864/pysparkler/cli.py
--rw-r--r--   0        0        0    10520 2023-04-13 23:00:57.465993 pysparkler-0.3.dev1681426864/pysparkler/pyspark_24_to_30.py
--rw-r--r--   0        0        0     3967 2023-04-13 23:00:57.465993 pysparkler-0.3.dev1681426864/pysparkler/pyspark_31_to_32.py
--rw-r--r--   0        0        0     4413 2023-04-13 23:00:57.465993 pysparkler-0.3.dev1681426864/pysparkler/pyspark_32_to_33.py
--rw-r--r--   0        0        0     5001 1970-01-01 00:00:00.000000 pysparkler-0.3.dev1681426864/PKG-INFO
+-rw-r--r--   0        0        0     8862 2023-04-14 16:41:07.230337 pysparkler-0.4.dev1681490474/README.md
+-rw-r--r--   0        0        0     1203 2023-04-14 16:41:14.658326 pysparkler-0.4.dev1681490474/pyproject.toml
+-rw-r--r--   0        0        0      807 2023-04-14 16:41:07.230337 pysparkler-0.4.dev1681490474/pysparkler/__init__.py
+-rw-r--r--   0        0        0     4258 2023-04-14 16:41:07.234337 pysparkler-0.4.dev1681490474/pysparkler/api.py
+-rw-r--r--   0        0        0     5879 2023-04-14 16:41:07.234337 pysparkler-0.4.dev1681490474/pysparkler/base.py
+-rw-r--r--   0        0        0     5734 2023-04-14 16:41:07.234337 pysparkler-0.4.dev1681490474/pysparkler/cli.py
+-rw-r--r--   0        0        0    10520 2023-04-14 16:41:07.234337 pysparkler-0.4.dev1681490474/pysparkler/pyspark_24_to_30.py
+-rw-r--r--   0        0        0     3967 2023-04-14 16:41:07.234337 pysparkler-0.4.dev1681490474/pysparkler/pyspark_31_to_32.py
+-rw-r--r--   0        0        0     4413 2023-04-14 16:41:07.234337 pysparkler-0.4.dev1681490474/pysparkler/pyspark_32_to_33.py
+-rw-r--r--   0        0        0     9741 1970-01-01 00:00:00.000000 pysparkler-0.4.dev1681490474/PKG-INFO
```

### Comparing `pysparkler-0.3.dev1681426864/pyproject.toml` & `pysparkler-0.4.dev1681490474/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "pysparkler"
-version = "0.3.dev1681426864"
-description = "A tool that upgrades your PySpark scripts to Spark 3.3 as per Spark migration Guideline"
+version = "0.4.dev1681490474"
+description = "A tool that upgrades your PySpark scripts to the latest Spark version as per Spark migration Guideline"
 authors = ["Dhruv Pratap <dhruv.pratap@gmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/holdenk/spark-upgrade"
 repository = "https://github.com/holdenk/spark-upgrade"
 maintainers = [
     "Holden Karau <holden@pigscanfly.ca>",
```

### Comparing `pysparkler-0.3.dev1681426864/pysparkler/__init__.py` & `pysparkler-0.4.dev1681490474/pysparkler/__init__.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.3.dev1681426864/pysparkler/api.py` & `pysparkler-0.4.dev1681490474/pysparkler/api.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.3.dev1681426864/pysparkler/base.py` & `pysparkler-0.4.dev1681490474/pysparkler/base.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.3.dev1681426864/pysparkler/cli.py` & `pysparkler-0.4.dev1681490474/pysparkler/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -100,15 +100,17 @@
     ctx: Context,
     input_file: str,
     output_file: str | None,
     dry_run: bool,
     file_type: str | None,
     output_kernel: str | None,
 ) -> None:
-    """Upgrade the PySparkler file to the latest version and provides comments as hints for manual changes"""
+    """Upgrades a PySpark script or Jupyter Notebook to the latest version, and where not context, provides comments as
+    code hints for manual changes.
+    """
 
     print_command_params(ctx)
     pysparkler = PySparkler(dry_run=dry_run)
 
     file_type = file_type or input_file.split(".")[-1]
     if file_type == "ipynb":
         output_file_content = pysparkler.upgrade_notebook(
```

### Comparing `pysparkler-0.3.dev1681426864/pysparkler/pyspark_24_to_30.py` & `pysparkler-0.4.dev1681490474/pysparkler/pyspark_24_to_30.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.3.dev1681426864/pysparkler/pyspark_31_to_32.py` & `pysparkler-0.4.dev1681490474/pysparkler/pyspark_31_to_32.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.3.dev1681426864/pysparkler/pyspark_32_to_33.py` & `pysparkler-0.4.dev1681490474/pysparkler/pyspark_32_to_33.py`

 * *Files identical despite different names*

