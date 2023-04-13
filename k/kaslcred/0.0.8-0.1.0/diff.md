# Comparing `tmp/kaslcred-0.0.8.tar.gz` & `tmp/kaslcred-0.1.0.tar.gz`

## Comparing `kaslcred-0.0.8.tar` & `kaslcred-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaslcred-0.0.8/.projectile
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 kaslcred-0.0.8/Dockerfile
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 kaslcred-0.0.8/Makefile
--rw-r--r--   0        0        0     5409 2020-02-02 00:00:00.000000 kaslcred-0.0.8/sample_schemas/hello-acdc-chain-schema.json
--rw-r--r--   0        0        0     6074 2020-02-02 00:00:00.000000 kaslcred-0.0.8/sample_schemas/hello-admit-schema.json
--rw-r--r--   0        0        0     6370 2020-02-02 00:00:00.000000 kaslcred-0.0.8/sample_schemas/hello-attend-schema.json
--rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 kaslcred-0.0.8/sample_schemas/hello-keri-schema.json
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 kaslcred-0.0.8/sample_schemas/single-schema-map.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaslcred-0.0.8/src/kaslcred/__init__.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 kaslcred-0.0.8/src/kaslcred/__main__.py
--rw-r--r--   0        0        0    11474 2020-02-02 00:00:00.000000 kaslcred-0.0.8/src/kaslcred/link.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 kaslcred-0.0.8/tests/__init__.py
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 kaslcred-0.0.8/tests/test_link.py
--rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 kaslcred-0.0.8/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 kaslcred-0.0.8/LICENSE
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 kaslcred-0.0.8/README.md
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 kaslcred-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 kaslcred-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 kaslcred-0.1.0/.DS_Store
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaslcred-0.1.0/.projectile
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 kaslcred-0.1.0/Dockerfile
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 kaslcred-0.1.0/Makefile
+-rw-r--r--   0        0        0    40144 2020-02-02 00:00:00.000000 kaslcred-0.1.0/Pipfile.lock
+-rw-r--r--   0        0        0     5409 2020-02-02 00:00:00.000000 kaslcred-0.1.0/sample_schemas/hello-acdc-chain-schema.json
+-rw-r--r--   0        0        0     6074 2020-02-02 00:00:00.000000 kaslcred-0.1.0/sample_schemas/hello-admit-schema.json
+-rw-r--r--   0        0        0     6370 2020-02-02 00:00:00.000000 kaslcred-0.1.0/sample_schemas/hello-attend-schema.json
+-rw-r--r--   0        0        0     4247 2020-02-02 00:00:00.000000 kaslcred-0.1.0/sample_schemas/hello-keri-schema.json
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 kaslcred-0.1.0/sample_schemas/single-schema-map.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaslcred-0.1.0/src/kaslcred/__init__.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 kaslcred-0.1.0/src/kaslcred/__main__.py
+-rw-r--r--   0        0        0    11484 2020-02-02 00:00:00.000000 kaslcred-0.1.0/src/kaslcred/link.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 kaslcred-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 kaslcred-0.1.0/tests/test_link.py
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 kaslcred-0.1.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 kaslcred-0.1.0/LICENSE
+-rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 kaslcred-0.1.0/README.md
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 kaslcred-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2733 2020-02-02 00:00:00.000000 kaslcred-0.1.0/PKG-INFO
```

### Comparing `kaslcred-0.0.8/Dockerfile` & `kaslcred-0.1.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `kaslcred-0.0.8/sample_schemas/hello-acdc-chain-schema.json` & `kaslcred-0.1.0/sample_schemas/hello-acdc-chain-schema.json`

 * *Files identical despite different names*

### Comparing `kaslcred-0.0.8/sample_schemas/hello-admit-schema.json` & `kaslcred-0.1.0/sample_schemas/hello-admit-schema.json`

 * *Files identical despite different names*

### Comparing `kaslcred-0.0.8/sample_schemas/hello-attend-schema.json` & `kaslcred-0.1.0/sample_schemas/hello-attend-schema.json`

 * *Files identical despite different names*

### Comparing `kaslcred-0.0.8/sample_schemas/hello-keri-schema.json` & `kaslcred-0.1.0/sample_schemas/hello-keri-schema.json`

 * *Files identical despite different names*

### Comparing `kaslcred-0.0.8/src/kaslcred/link.py` & `kaslcred-0.1.0/src/kaslcred/link.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,18 +104,18 @@
     """Save SAIDified schema to results directory."""
     for (schema_name, schema) in saidified_schemas:
         save_result(schema_name, schema_results_dir, schema, pretty)
 
 
 def get_schema_said(schema):
     """Get SAID for target schema using default ID symbol."""
-    if not schema[coring.Ids.dollar] or schema[coring.Ids.dollar] == "":
+    if not schema[coring.Saids.dollar] or schema[coring.Saids.dollar] == "":
         raise RuntimeError(
-            f'Cannot get schema SAID: {coring.Ids.dollar} attribute empty or missing from schema {schema}')
-    return schema[coring.Ids.dollar]
+            f'Cannot get schema SAID: {coring.Saids.dollar} attribute empty or missing from schema {schema}')
+    return schema[coring.Saids.dollar]
 
 
 def construct_schema(schema: ACDCSchema, schema_root_path: str, schema_results: dict):
     """
     Create a linked schema in root_path with needed edges from schema_results.
 
     Will use any edge name overrides specified in the map file.
@@ -227,15 +227,15 @@
     for dep in dependencies:
         if dep not in schema_names:
             invalid_dependencies.append(dep)
             valid = False
     return valid, invalid_dependencies
 
 
-def populateSAIDS(schema: dict, idage: str = coring.Ids.dollar,
+def populateSAIDS(schema: dict, idage: str = coring.Saids.dollar,
                   code: str = coring.MtrDex.Blake3_256):
     """
     Calculate and write self addressing identifiers (SAIDS).
 
     Applies to root, attribute (a), edge (e), and rules (r) sections.
     :param schema (dict): The schema to calculate SAIDs for and write to
     :param idage (str): The property name to use to write SAIDs to.
```

### Comparing `kaslcred-0.0.8/tests/test_link.py` & `kaslcred-0.1.0/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `kaslcred-0.0.8/.gitignore` & `kaslcred-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `kaslcred-0.0.8/LICENSE` & `kaslcred-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kaslcred-0.0.8/pyproject.toml` & `kaslcred-0.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "kaslcred"
-version = "0.0.8"
+version = "0.1.0"
 authors = [
     {name="Kent Bull", email="kent@tetraveda.com"},
     {name="Kevin Griffin", email="griffin.kev@gmail.com"}
 ]
 description = "A credential schema linker for the KERI and ACDC ecosystem."
 readme = "README.md"
-requires-python = ">=3.10"
+requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent"
 ]
 dependencies=[
-    "keri >= 0.6.8"
+    "keri >= 1.0.0"
 ]
 
 
 [project.urls]
 "Homepage" = "https://github.com/tetraveda/kaslcred"
 
 [tool.pytest.ini_options]
```

