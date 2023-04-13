# Comparing `tmp/py-partiql-parser-0.1.0.tar.gz` & `tmp/py-partiql-parser-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-partiql-parser-0.1.0.tar", last modified: Mon Mar 20 22:11:16 2023, max compression
+gzip compressed data, was "py-partiql-parser-0.2.0.tar", last modified: Thu Apr 13 22:46:15 2023, max compression
```

## Comparing `py-partiql-parser-0.1.0.tar` & `py-partiql-parser-0.2.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 22:11:16.818468 py-partiql-parser-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-20 22:10:59.000000 py-partiql-parser-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-03-20 22:11:16.818468 py-partiql-parser-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-03-20 22:10:59.000000 py-partiql-parser-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 22:11:16.810468 py-partiql-parser-0.1.0/py_partiql_parser/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-20 22:10:59.000000 py-partiql-parser-0.1.0/py_partiql_parser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 22:11:16.814468 py-partiql-parser-0.1.0/py_partiql_parser/_internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 22:10:59.000000 py-partiql-parser-0.1.0/py_partiql_parser/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-03-20 22:10:59.000000 py-partiql-parser-0.1.0/py_partiql_parser/_internal/case_insensitive_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-03-20 22:10:59.000000 py-partiql-parser-0.1.0/py_partiql_parser/_internal/clause_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-03-20 22:10:59.000000 py-partiql-parser-0.1.0/py_partiql_parser/_internal/csv_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-03-20 22:10:59.000000 py-partiql-parser-0.1.0/py_partiql_parser/_internal/from_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-03-20 22:10:59.000000 py-partiql-parser-0.1.0/py_partiql_parser/_internal/json_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-03-20 22:10:59.000000 py-partiql-parser-0.1.0/py_partiql_parser/_internal/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-03-20 22:10:59.000000 py-partiql-parser-0.1.0/py_partiql_parser/_internal/select_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-03-20 22:10:59.000000 py-partiql-parser-0.1.0/py_partiql_parser/_internal/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-03-20 22:10:59.000000 py-partiql-parser-0.1.0/py_partiql_parser/_internal/where_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 22:11:16.814468 py-partiql-parser-0.1.0/py_partiql_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-03-20 22:11:16.000000 py-partiql-parser-0.1.0/py_partiql_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-03-20 22:11:16.000000 py-partiql-parser-0.1.0/py_partiql_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 22:11:16.000000 py-partiql-parser-0.1.0/py_partiql_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-20 22:11:16.000000 py-partiql-parser-0.1.0/py_partiql_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-20 22:11:16.000000 py-partiql-parser-0.1.0/py_partiql_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-03-20 22:11:09.000000 py-partiql-parser-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-20 22:11:16.818468 py-partiql-parser-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 22:11:16.818468 py-partiql-parser-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-03-20 22:10:59.000000 py-partiql-parser-0.1.0/tests/test_aws_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-03-20 22:10:59.000000 py-partiql-parser-0.1.0/tests/test_csv_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-03-20 22:10:59.000000 py-partiql-parser-0.1.0/tests/test_from_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-03-20 22:10:59.000000 py-partiql-parser-0.1.0/tests/test_json_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-03-20 22:10:59.000000 py-partiql-parser-0.1.0/tests/test_select_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-03-20 22:10:59.000000 py-partiql-parser-0.1.0/tests/test_select_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-03-20 22:10:59.000000 py-partiql-parser-0.1.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-03-20 22:10:59.000000 py-partiql-parser-0.1.0/tests/test_where_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:46:15.875878 py-partiql-parser-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-13 22:45:57.000000 py-partiql-parser-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-04-13 22:46:15.875878 py-partiql-parser-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-13 22:45:57.000000 py-partiql-parser-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:46:15.871878 py-partiql-parser-0.2.0/py_partiql_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-13 22:45:57.000000 py-partiql-parser-0.2.0/py_partiql_parser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:46:15.875878 py-partiql-parser-0.2.0/py_partiql_parser/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 22:45:57.000000 py-partiql-parser-0.2.0/py_partiql_parser/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-13 22:45:57.000000 py-partiql-parser-0.2.0/py_partiql_parser/_internal/case_insensitive_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-13 22:45:57.000000 py-partiql-parser-0.2.0/py_partiql_parser/_internal/clause_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-13 22:45:57.000000 py-partiql-parser-0.2.0/py_partiql_parser/_internal/csv_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-13 22:45:57.000000 py-partiql-parser-0.2.0/py_partiql_parser/_internal/from_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-04-13 22:45:57.000000 py-partiql-parser-0.2.0/py_partiql_parser/_internal/json_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-13 22:45:57.000000 py-partiql-parser-0.2.0/py_partiql_parser/_internal/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-04-13 22:45:57.000000 py-partiql-parser-0.2.0/py_partiql_parser/_internal/select_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-04-13 22:45:57.000000 py-partiql-parser-0.2.0/py_partiql_parser/_internal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-04-13 22:45:57.000000 py-partiql-parser-0.2.0/py_partiql_parser/_internal/where_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:46:15.871878 py-partiql-parser-0.2.0/py_partiql_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-04-13 22:46:15.000000 py-partiql-parser-0.2.0/py_partiql_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-13 22:46:15.000000 py-partiql-parser-0.2.0/py_partiql_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 22:46:15.000000 py-partiql-parser-0.2.0/py_partiql_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-13 22:46:15.000000 py-partiql-parser-0.2.0/py_partiql_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-13 22:46:15.000000 py-partiql-parser-0.2.0/py_partiql_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-13 22:46:08.000000 py-partiql-parser-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 22:46:15.875878 py-partiql-parser-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:46:15.875878 py-partiql-parser-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-04-13 22:45:57.000000 py-partiql-parser-0.2.0/tests/test_aws_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-04-13 22:45:57.000000 py-partiql-parser-0.2.0/tests/test_csv_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-13 22:45:57.000000 py-partiql-parser-0.2.0/tests/test_dynamodb_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-13 22:45:57.000000 py-partiql-parser-0.2.0/tests/test_from_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-04-13 22:45:57.000000 py-partiql-parser-0.2.0/tests/test_json_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-13 22:45:57.000000 py-partiql-parser-0.2.0/tests/test_select_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-13 22:45:57.000000 py-partiql-parser-0.2.0/tests/test_select_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-13 22:45:57.000000 py-partiql-parser-0.2.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-04-13 22:45:57.000000 py-partiql-parser-0.2.0/tests/test_where_parser.py
```

### Comparing `py-partiql-parser-0.1.0/LICENSE` & `py-partiql-parser-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.1.0/PKG-INFO` & `py-partiql-parser-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-partiql-parser
-Version: 0.1.0
+Version: 0.2.0
 Summary: Pure Python PartiQL Parser
 Author-email: Bert Blommers <info@bertblommers.nl>
 License: MIT
 Keywords: pypartiql,parser
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `py-partiql-parser-0.1.0/README.md` & `py-partiql-parser-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.1.0/py_partiql_parser/_internal/case_insensitive_dict.py` & `py-partiql-parser-0.2.0/py_partiql_parser/_internal/case_insensitive_dict.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.1.0/py_partiql_parser/_internal/clause_tokenizer.py` & `py-partiql-parser-0.2.0/py_partiql_parser/_internal/clause_tokenizer.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.1.0/py_partiql_parser/_internal/csv_converter.py` & `py-partiql-parser-0.2.0/py_partiql_parser/_internal/csv_converter.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.1.0/py_partiql_parser/_internal/from_parser.py` & `py-partiql-parser-0.2.0/py_partiql_parser/_internal/from_parser.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.1.0/py_partiql_parser/_internal/json_parser.py` & `py-partiql-parser-0.2.0/py_partiql_parser/_internal/json_parser.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.1.0/py_partiql_parser/_internal/parser.py` & `py-partiql-parser-0.2.0/py_partiql_parser/_internal/parser.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,40 +2,41 @@
 
 from typing import Dict, Any, Union, List, AnyStr
 
 from .from_parser import FromParser
 from .json_parser import JsonParser
 from .select_parser import SelectParser
 from .where_parser import WhereParser
+from .utils import is_dict
 
 
 class Parser:
     RETURN_TYPE = Union[Dict[AnyStr, Any], List]
 
-    def __init__(self, source_data: Dict[str, str]):
-        self.source_data = source_data
+    def __init__(self, source_data: Dict[str, str], query_has_table_prefix=True):
         # Source data is in the format: {source: json}
         # Where 'json' is one or more json documents separated by a newline
-        self.documents = {key: value for key, value in source_data.items()}
+        self.documents = source_data
+        self.query_has_table_prefix = query_has_table_prefix
 
     def parse(self, query: str) -> List[Dict[str, Any]]:
         query = query.replace("\n", " ")
         clauses = re.split("SELECT | FROM | WHERE ", query, flags=re.IGNORECASE)
         # First clause is whatever comes in front of SELECT - which should be nothing
         _ = clauses[0]
         # FROM
         from_clauses = FromParser().parse(clauses[2])
+        source_data = self.documents[list(from_clauses.values())[0]]
+        source_data = JsonParser().parse(source_data)
+        if is_dict(source_data):
+            source_data = [source_data]  # type: ignore
+
         # WHERE
         if len(clauses) > 3:
             where_clause = clauses[3]
-            self.documents = WhereParser(self.source_data).parse(
-                from_clauses, where_clause
+            source_data = WhereParser(source_data, self.query_has_table_prefix).parse(
+                where_clause
             )
-        else:
-            for key, value in self.documents.items():
-                self.documents[key] = JsonParser().parse(value)
-                if isinstance(self.documents[key], dict):
-                    self.documents[key] = [self.documents[key]]  # type: ignore
 
         # SELECT
         select_clause = clauses[1]
-        return SelectParser().parse(select_clause, from_clauses, self.documents)
+        return SelectParser().parse(select_clause, from_clauses, source_data)
```

### Comparing `py-partiql-parser-0.1.0/py_partiql_parser/_internal/select_parser.py` & `py-partiql-parser-0.2.0/py_partiql_parser/_internal/select_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 class SelectClause:
     def __init__(self, value: str):
         self.value = value.strip()
 
     def select(self, aliases: Dict[str, str], document: Dict[str, Any]):
         if self.value == "*":
+            # return document[alias]
             return document["s3object"]
         if "." in self.value:
             key, remaining = self.value.split(".", maxsplit=1)
             return find_nested_data_in_object(
                 select_clause=remaining, json_doc=document[aliases.get(key, key)]
             )
         else:
@@ -47,40 +48,32 @@
 
 
 class SelectParser:
     def parse(
         self,
         select_clause: str,
         aliases: Dict[str, Any],
-        data: Dict[str, List[Dict[str, Any]]],
+        documents: List[Dict[str, Any]],
     ) -> List[Dict[str, Any]]:
         clauses = self.parse_clauses(select_clause)
 
-        if isinstance(data["s3object"], CaseInsensitiveDict):
-            documents = [data["s3object"]]
-        else:
-            documents = data["s3object"]
-
         for clause in clauses:
             if isinstance(clause, FunctionClause):
                 return [clause.execute(aliases, documents)]
 
         result: List[Dict[str, Any]] = []
 
         for json_document in documents:
             filtered_document = dict()
             for clause in clauses:
+                # TODO: go through all keys, the table/file can be called anything - not just 's3object'
                 attr = clause.select(aliases, {"s3object": json_document})
-                print(f"{clause}.select == {attr}")
-                print(type(attr))
                 if attr is not None:
                     filtered_document.update(attr)
             result.append(filtered_document)
-        print(data)
-        print(result)
         return result
 
     def parse_clauses(self, select_clause: str) -> List[SelectClause]:
         results = []
         tokenizer = ClauseTokenizer(select_clause)
         current_clause = fn_name = ""
         while True:
```

### Comparing `py-partiql-parser-0.1.0/py_partiql_parser/_internal/utils.py` & `py-partiql-parser-0.2.0/py_partiql_parser/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.1.0/py_partiql_parser/_internal/where_parser.py` & `py-partiql-parser-0.2.0/py_partiql_parser/_internal/where_parser.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,45 +2,32 @@
 
 from .clause_tokenizer import ClauseTokenizer
 from .json_parser import JsonParser
 from .utils import find_value_in_document
 
 
 class WhereParser:
-    def __init__(self, partially_prepped_data: Any = None):
-        print(f"WhereParser({partially_prepped_data})")
-        self.partially_prepped_data = partially_prepped_data or {}
-        for key, value in self.partially_prepped_data.items():
-            self.partially_prepped_data[key] = JsonParser().parse(value)
-        print(self.partially_prepped_data)
-
-    def parse(self, aliases: Dict[str, str], where_clause: str) -> Any:
-        return_all = where_clause == "TRUE"
-        if return_all:
-            alias, key, value = ("", "", "")
-        else:
-            filter_keys, filter_value = self.parse_where_clause(where_clause)
-
-        for data_key in self.partially_prepped_data:
-            all_rows = self.partially_prepped_data[data_key]
-            filtered_rows = self.filter_rows(
-                aliases, filter_keys, filter_value, data_key, all_rows
-            )
-            self.partially_prepped_data[data_key] = filtered_rows
+    def __init__(self, source_data: Any, query_has_table_prefix: bool):
+        self.source_data = source_data
+        self.query_has_table_prefix = query_has_table_prefix
 
-        return self.partially_prepped_data
+    def parse(self, where_clause: str) -> Any:
+        filter_keys, filter_value = self.parse_where_clause(where_clause)
 
-    def filter_rows(self, aliases, filter_keys, filter_value, data_key, all_rows):
+        return self.filter_rows(filter_keys, filter_value)
+
+    def filter_rows(self, filter_keys, filter_value):
         def _filter(row):
-            if aliases.get(filter_keys[0], filter_keys[0]) == data_key:
+            if self.query_has_table_prefix:
                 actual_value = find_value_in_document(filter_keys[1:], row)
                 return actual_value == filter_value
-            return False
+            else:
+                return find_value_in_document(filter_keys, row) == filter_value
 
-        return [row for row in all_rows if _filter(row)]
+        return [row for row in self.source_data if _filter(row)]
 
     def parse_where_clause(self, where_clause: str) -> Tuple[List[str], str]:
         where_clause_parser = ClauseTokenizer(where_clause)
         keys: List[str] = []
         value = ""
         section: Optional[str] = "KEY"
         current_phrase = ""
```

### Comparing `py-partiql-parser-0.1.0/py_partiql_parser.egg-info/PKG-INFO` & `py-partiql-parser-0.2.0/py_partiql_parser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-partiql-parser
-Version: 0.1.0
+Version: 0.2.0
 Summary: Pure Python PartiQL Parser
 Author-email: Bert Blommers <info@bertblommers.nl>
 License: MIT
 Keywords: pypartiql,parser
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `py-partiql-parser-0.1.0/py_partiql_parser.egg-info/SOURCES.txt` & `py-partiql-parser-0.2.0/py_partiql_parser.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,13 +15,14 @@
 py_partiql_parser/_internal/json_parser.py
 py_partiql_parser/_internal/parser.py
 py_partiql_parser/_internal/select_parser.py
 py_partiql_parser/_internal/utils.py
 py_partiql_parser/_internal/where_parser.py
 tests/test_aws_examples.py
 tests/test_csv_converter.py
+tests/test_dynamodb_examples.py
 tests/test_from_parser.py
 tests/test_json_parser.py
 tests/test_select_functions.py
 tests/test_select_parser.py
 tests/test_utils.py
 tests/test_where_parser.py
```

### Comparing `py-partiql-parser-0.1.0/tests/test_aws_examples.py` & `py-partiql-parser-0.2.0/tests/test_aws_examples.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.1.0/tests/test_csv_converter.py` & `py-partiql-parser-0.2.0/tests/test_csv_converter.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.1.0/tests/test_from_parser.py` & `py-partiql-parser-0.2.0/tests/test_from_parser.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.1.0/tests/test_json_parser.py` & `py-partiql-parser-0.2.0/tests/test_json_parser.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.1.0/tests/test_select_functions.py` & `py-partiql-parser-0.2.0/tests/test_select_functions.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.1.0/tests/test_select_parser.py` & `py-partiql-parser-0.2.0/tests/test_select_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     result = SelectParser().parse_clauses("count(*)")
     assert result == [FunctionClause(function_name="count", value="*")]
 
 
 @pytest.mark.xfail(message="Not yet implemented")
 def test_parse_function_alias_clause():
     result = SelectParser().parse_clauses("count(*) as cnt")
-    assert result == [FunctionClause(function_name="count", value="*", alias="cnt")]
+    assert result == [FunctionClause(function_name="count", value="*")]
 
 
 def test_parse_mix_of_function_and_regular_clauses():
     result = SelectParser().parse_clauses("count(*), s.city, max(s.citizens)")
     assert len(result) == 3
     assert FunctionClause(function_name="count", value="*") in result
     assert FunctionClause(function_name="max", value="s.citizens") in result
```

### Comparing `py-partiql-parser-0.1.0/tests/test_utils.py` & `py-partiql-parser-0.2.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.1.0/tests/test_where_parser.py` & `py-partiql-parser-0.2.0/tests/test_where_parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,43 @@
 import pytest
 from py_partiql_parser._internal.parser import WhereParser
 
 
 class TestWhereClause:
     def test_single_key(self):
         where_clause = "s3object.city = 'Chicago'"
-        assert WhereParser().parse_where_clause(where_clause) == (
+        assert WhereParser({}, False).parse_where_clause(where_clause) == (
             ["s3object", "city"],
             "Chicago",
         )
 
     def test_nested_key(self):
         where_clause = "s3object.city.street = 'Chicago'"
-        assert WhereParser().parse_where_clause(where_clause) == (
+        assert WhereParser({}, False).parse_where_clause(where_clause) == (
             ["s3object", "city", "street"],
             "Chicago",
         )
 
     def test_quoted_key(self):
         where_clause = "s3object.\"city\" = 'Chicago'"
-        assert WhereParser().parse_where_clause(where_clause) == (
+        assert WhereParser({}, False).parse_where_clause(where_clause) == (
             ["s3object", "city"],
             "Chicago",
         )
 
     def test_quoted_nested_key(self):
         where_clause = "s3object.\"city details\".street = 'Chicago'"
-        assert WhereParser().parse_where_clause(where_clause) == (
+        assert WhereParser({}, False).parse_where_clause(where_clause) == (
             ["s3object", "city details", "street"],
             "Chicago",
         )
 
-    @pytest.mark.xfail(
-        message="Multiple clauses are not yet supported - this just returns the first clause at the moment"
-    )
     def test_multiple_keys(self):
         where_clause = "s3object.city = 'Chicago', s3object.name = 'Tommy'"
-        assert WhereParser().parse_where_clause(where_clause) == (
+        assert WhereParser({}, False).parse_where_clause(where_clause) == (
             ["s3object", "city"],
             "Chicago",
         )
 
 
 class TestFilter:
     all_rows = [
@@ -50,64 +47,57 @@
         {"Name": "Jane", "city": "Chicago"},
         {"Name": "Sean", "city": "Chicago"},
         {"Name": "Mary", "city": "Chicago", "notes": {"extra": "y"}},
         {"Name": "Kate", "city": "Chicago", "notes": {"extra": "n"}},
     ]
 
     def test_simple(self):
-        aliases = {"s3object": "s3object"}
         filter_keys = ["s3object", "city"]
         filter_value = "Los Angeles"
-        data_key = "s3object"
-        assert WhereParser().filter_rows(
-            aliases=aliases,
-            filter_keys=filter_keys,
-            filter_value=filter_value,
-            data_key=data_key,
-            all_rows=TestFilter.all_rows,
-        ) == [{"Name": "Vinod", "city": "Los Angeles"}]
+        assert WhereParser(
+            TestFilter.all_rows, query_has_table_prefix=True
+        ).filter_rows(filter_keys=filter_keys, filter_value=filter_value,) == [
+            {"Name": "Vinod", "city": "Los Angeles"}
+        ]
+
+    def test_without_prefix(self):
+        filter_keys = ["city"]
+        filter_value = "Los Angeles"
+        assert WhereParser(
+            TestFilter.all_rows, query_has_table_prefix=False
+        ).filter_rows(filter_keys=filter_keys, filter_value=filter_value,) == [
+            {"Name": "Vinod", "city": "Los Angeles"}
+        ]
 
     def test_alias(self):
-        aliases = {"s": "s3object"}
         filter_keys = ["s", "city"]
         filter_value = "Los Angeles"
-        data_key = "s3object"
-        assert WhereParser().filter_rows(
-            aliases=aliases,
-            filter_keys=filter_keys,
-            filter_value=filter_value,
-            data_key=data_key,
-            all_rows=TestFilter.all_rows,
-        ) == [{"Name": "Vinod", "city": "Los Angeles"}]
+        assert WhereParser(
+            TestFilter.all_rows, query_has_table_prefix=True
+        ).filter_rows(filter_keys=filter_keys, filter_value=filter_value,) == [
+            {"Name": "Vinod", "city": "Los Angeles"}
+        ]
 
     def test_alias_nested_key(self):
-        aliases = {"s3object": "s3object"}
         filter_keys = ["s3object", "notes", "extra"]
         filter_value = "y"
-        data_key = "s3object"
-        assert WhereParser().filter_rows(
-            aliases=aliases,
-            filter_keys=filter_keys,
-            filter_value=filter_value,
-            data_key=data_key,
-            all_rows=TestFilter.all_rows,
-        ) == [{"Name": "Mary", "city": "Chicago", "notes": {"extra": "y"}}]
+        assert WhereParser(
+            TestFilter.all_rows, query_has_table_prefix=True
+        ).filter_rows(filter_keys=filter_keys, filter_value=filter_value,) == [
+            {"Name": "Mary", "city": "Chicago", "notes": {"extra": "y"}}
+        ]
 
     @pytest.mark.xfail(message="Not yet implemented")
     def test_case_insensitivity(self):
-        aliases = {"s3object": "s3object"}
         # Filter by lower case "city"
         filter_keys = ["s3object", "city"]
         filter_value = "Chicago"
-        data_key = "s3object"
         # Data has upper case CITY
         all_rows = [
             {"Name": "Sam", "CITY": "Irvine"},
             {"Name": "Vinod", "City": "Los Angeles"},
         ]
         assert WhereParser().filter_rows(
-            aliases=aliases,
             filter_keys=filter_keys,
             filter_value=filter_value,
-            data_key=data_key,
             all_rows=all_rows,
         ) == [{"Name": "Jane", "City": "Chicago"}]
```

