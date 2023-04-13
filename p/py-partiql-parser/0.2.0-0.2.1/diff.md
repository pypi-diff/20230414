# Comparing `tmp/py-partiql-parser-0.2.0.tar.gz` & `tmp/py-partiql-parser-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-partiql-parser-0.2.0.tar", last modified: Thu Apr 13 22:46:15 2023, max compression
+gzip compressed data, was "py-partiql-parser-0.2.1.tar", last modified: Thu Apr 13 22:55:42 2023, max compression
```

## Comparing `py-partiql-parser-0.2.0.tar` & `py-partiql-parser-0.2.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:46:15.875878 py-partiql-parser-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-13 22:45:57.000000 py-partiql-parser-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-04-13 22:46:15.875878 py-partiql-parser-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-13 22:45:57.000000 py-partiql-parser-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:46:15.871878 py-partiql-parser-0.2.0/py_partiql_parser/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-13 22:45:57.000000 py-partiql-parser-0.2.0/py_partiql_parser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:46:15.875878 py-partiql-parser-0.2.0/py_partiql_parser/_internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 22:45:57.000000 py-partiql-parser-0.2.0/py_partiql_parser/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-13 22:45:57.000000 py-partiql-parser-0.2.0/py_partiql_parser/_internal/case_insensitive_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-13 22:45:57.000000 py-partiql-parser-0.2.0/py_partiql_parser/_internal/clause_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-13 22:45:57.000000 py-partiql-parser-0.2.0/py_partiql_parser/_internal/csv_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-13 22:45:57.000000 py-partiql-parser-0.2.0/py_partiql_parser/_internal/from_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-04-13 22:45:57.000000 py-partiql-parser-0.2.0/py_partiql_parser/_internal/json_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-13 22:45:57.000000 py-partiql-parser-0.2.0/py_partiql_parser/_internal/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-04-13 22:45:57.000000 py-partiql-parser-0.2.0/py_partiql_parser/_internal/select_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-04-13 22:45:57.000000 py-partiql-parser-0.2.0/py_partiql_parser/_internal/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-04-13 22:45:57.000000 py-partiql-parser-0.2.0/py_partiql_parser/_internal/where_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:46:15.871878 py-partiql-parser-0.2.0/py_partiql_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-04-13 22:46:15.000000 py-partiql-parser-0.2.0/py_partiql_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-13 22:46:15.000000 py-partiql-parser-0.2.0/py_partiql_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 22:46:15.000000 py-partiql-parser-0.2.0/py_partiql_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-13 22:46:15.000000 py-partiql-parser-0.2.0/py_partiql_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-13 22:46:15.000000 py-partiql-parser-0.2.0/py_partiql_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-13 22:46:08.000000 py-partiql-parser-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 22:46:15.875878 py-partiql-parser-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:46:15.875878 py-partiql-parser-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-04-13 22:45:57.000000 py-partiql-parser-0.2.0/tests/test_aws_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-04-13 22:45:57.000000 py-partiql-parser-0.2.0/tests/test_csv_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-13 22:45:57.000000 py-partiql-parser-0.2.0/tests/test_dynamodb_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-13 22:45:57.000000 py-partiql-parser-0.2.0/tests/test_from_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-04-13 22:45:57.000000 py-partiql-parser-0.2.0/tests/test_json_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-13 22:45:57.000000 py-partiql-parser-0.2.0/tests/test_select_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-13 22:45:57.000000 py-partiql-parser-0.2.0/tests/test_select_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-13 22:45:57.000000 py-partiql-parser-0.2.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-04-13 22:45:57.000000 py-partiql-parser-0.2.0/tests/test_where_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:55:42.781393 py-partiql-parser-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-13 22:55:24.000000 py-partiql-parser-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-04-13 22:55:42.777392 py-partiql-parser-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-13 22:55:24.000000 py-partiql-parser-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:55:42.777392 py-partiql-parser-0.2.1/py_partiql_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-13 22:55:24.000000 py-partiql-parser-0.2.1/py_partiql_parser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:55:42.777392 py-partiql-parser-0.2.1/py_partiql_parser/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 22:55:24.000000 py-partiql-parser-0.2.1/py_partiql_parser/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-13 22:55:24.000000 py-partiql-parser-0.2.1/py_partiql_parser/_internal/case_insensitive_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-13 22:55:24.000000 py-partiql-parser-0.2.1/py_partiql_parser/_internal/clause_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-13 22:55:24.000000 py-partiql-parser-0.2.1/py_partiql_parser/_internal/csv_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-13 22:55:24.000000 py-partiql-parser-0.2.1/py_partiql_parser/_internal/from_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-04-13 22:55:24.000000 py-partiql-parser-0.2.1/py_partiql_parser/_internal/json_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-04-13 22:55:24.000000 py-partiql-parser-0.2.1/py_partiql_parser/_internal/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-04-13 22:55:24.000000 py-partiql-parser-0.2.1/py_partiql_parser/_internal/select_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-04-13 22:55:24.000000 py-partiql-parser-0.2.1/py_partiql_parser/_internal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-04-13 22:55:24.000000 py-partiql-parser-0.2.1/py_partiql_parser/_internal/where_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:55:42.777392 py-partiql-parser-0.2.1/py_partiql_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-04-13 22:55:42.000000 py-partiql-parser-0.2.1/py_partiql_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-13 22:55:42.000000 py-partiql-parser-0.2.1/py_partiql_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 22:55:42.000000 py-partiql-parser-0.2.1/py_partiql_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-13 22:55:42.000000 py-partiql-parser-0.2.1/py_partiql_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-13 22:55:42.000000 py-partiql-parser-0.2.1/py_partiql_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-13 22:55:35.000000 py-partiql-parser-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 22:55:42.781393 py-partiql-parser-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:55:42.777392 py-partiql-parser-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-04-13 22:55:24.000000 py-partiql-parser-0.2.1/tests/test_aws_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-04-13 22:55:24.000000 py-partiql-parser-0.2.1/tests/test_csv_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-13 22:55:24.000000 py-partiql-parser-0.2.1/tests/test_dynamodb_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-13 22:55:24.000000 py-partiql-parser-0.2.1/tests/test_from_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-04-13 22:55:24.000000 py-partiql-parser-0.2.1/tests/test_json_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-13 22:55:24.000000 py-partiql-parser-0.2.1/tests/test_select_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-13 22:55:24.000000 py-partiql-parser-0.2.1/tests/test_select_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-13 22:55:24.000000 py-partiql-parser-0.2.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-04-13 22:55:24.000000 py-partiql-parser-0.2.1/tests/test_where_parser.py
```

### Comparing `py-partiql-parser-0.2.0/LICENSE` & `py-partiql-parser-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.2.0/PKG-INFO` & `py-partiql-parser-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-partiql-parser
-Version: 0.2.0
+Version: 0.2.1
 Summary: Pure Python PartiQL Parser
 Author-email: Bert Blommers <info@bertblommers.nl>
 License: MIT
 Keywords: pypartiql,parser
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `py-partiql-parser-0.2.0/README.md` & `py-partiql-parser-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.2.0/py_partiql_parser/_internal/case_insensitive_dict.py` & `py-partiql-parser-0.2.1/py_partiql_parser/_internal/case_insensitive_dict.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.2.0/py_partiql_parser/_internal/clause_tokenizer.py` & `py-partiql-parser-0.2.1/py_partiql_parser/_internal/clause_tokenizer.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.2.0/py_partiql_parser/_internal/csv_converter.py` & `py-partiql-parser-0.2.1/py_partiql_parser/_internal/csv_converter.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.2.0/py_partiql_parser/_internal/from_parser.py` & `py-partiql-parser-0.2.1/py_partiql_parser/_internal/from_parser.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.2.0/py_partiql_parser/_internal/json_parser.py` & `py-partiql-parser-0.2.1/py_partiql_parser/_internal/json_parser.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.2.0/py_partiql_parser/_internal/parser.py` & `py-partiql-parser-0.2.1/py_partiql_parser/_internal/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     def parse(self, query: str) -> List[Dict[str, Any]]:
         query = query.replace("\n", " ")
         clauses = re.split("SELECT | FROM | WHERE ", query, flags=re.IGNORECASE)
         # First clause is whatever comes in front of SELECT - which should be nothing
         _ = clauses[0]
         # FROM
         from_clauses = FromParser().parse(clauses[2])
-        source_data = self.documents[list(from_clauses.values())[0]]
+        source_data = self.documents[list(from_clauses.values())[0].lower()]
         source_data = JsonParser().parse(source_data)
         if is_dict(source_data):
             source_data = [source_data]  # type: ignore
 
         # WHERE
         if len(clauses) > 3:
             where_clause = clauses[3]
```

### Comparing `py-partiql-parser-0.2.0/py_partiql_parser/_internal/select_parser.py` & `py-partiql-parser-0.2.1/py_partiql_parser/_internal/select_parser.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.2.0/py_partiql_parser/_internal/utils.py` & `py-partiql-parser-0.2.1/py_partiql_parser/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.2.0/py_partiql_parser/_internal/where_parser.py` & `py-partiql-parser-0.2.1/py_partiql_parser/_internal/where_parser.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.2.0/py_partiql_parser.egg-info/PKG-INFO` & `py-partiql-parser-0.2.1/py_partiql_parser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-partiql-parser
-Version: 0.2.0
+Version: 0.2.1
 Summary: Pure Python PartiQL Parser
 Author-email: Bert Blommers <info@bertblommers.nl>
 License: MIT
 Keywords: pypartiql,parser
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `py-partiql-parser-0.2.0/py_partiql_parser.egg-info/SOURCES.txt` & `py-partiql-parser-0.2.1/py_partiql_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.2.0/tests/test_aws_examples.py` & `py-partiql-parser-0.2.1/tests/test_aws_examples.py`

 * *Files 6% similar despite different names*

```diff
@@ -122,13 +122,21 @@
     query = "SELECT * FROM s3object"
     result = Parser(source_data={"s3object": json.dumps(input_json_object)}).parse(
         query
     )
     result.should.equal([input_json_object])
 
 
+def test_aws_sample__s3object_is_case_insensitive():
+    query = "SELECT * FROM s3obJEct"
+    result = Parser(source_data={"s3object": json.dumps(input_json_object)}).parse(
+        query
+    )
+    result.should.equal([input_json_object])
+
+
 def test_aws_sample__object_select_attr():
     query = "SELECT s.a1 FROM s3object AS s"
     result = Parser(source_data={"s3object": json.dumps(input_json_object)}).parse(
         query
     )
     result.should.equal([{"a1": "b1"}])
```

### Comparing `py-partiql-parser-0.2.0/tests/test_csv_converter.py` & `py-partiql-parser-0.2.1/tests/test_csv_converter.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.2.0/tests/test_dynamodb_examples.py` & `py-partiql-parser-0.2.1/tests/test_dynamodb_examples.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.2.0/tests/test_from_parser.py` & `py-partiql-parser-0.2.1/tests/test_from_parser.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.2.0/tests/test_json_parser.py` & `py-partiql-parser-0.2.1/tests/test_json_parser.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.2.0/tests/test_select_functions.py` & `py-partiql-parser-0.2.1/tests/test_select_functions.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.2.0/tests/test_select_parser.py` & `py-partiql-parser-0.2.1/tests/test_select_parser.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.2.0/tests/test_utils.py` & `py-partiql-parser-0.2.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.2.0/tests/test_where_parser.py` & `py-partiql-parser-0.2.1/tests/test_where_parser.py`

 * *Files identical despite different names*

