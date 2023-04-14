# Comparing `tmp/ODetaM-1.4.0.tar.gz` & `tmp/ODetaM-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ODetaM-1.4.0.tar", max compression
+gzip compressed data, was "ODetaM-1.5.0.tar", max compression
```

## Comparing `ODetaM-1.4.0.tar` & `ODetaM-1.5.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1067 2023-03-24 19:58:47.969087 ODetaM-1.4.0/LICENSE
--rw-r--r--   0        0        0     6072 2023-03-24 21:17:09.736288 ODetaM-1.4.0/README.md
--rw-r--r--   0        0        0       51 2023-03-24 19:58:47.969290 ODetaM-1.4.0/odetam/__init__.py
--rw-r--r--   0        0        0     4589 2023-03-24 21:26:42.700173 ODetaM-1.4.0/odetam/async_model.py
--rw-r--r--   0        0        0      169 2023-03-24 19:58:47.969472 ODetaM-1.4.0/odetam/exceptions.py
--rw-r--r--   0        0        0     4053 2023-03-24 21:26:42.726201 ODetaM-1.4.0/odetam/field.py
--rw-r--r--   0        0        0     8488 2023-03-24 21:26:42.794477 ODetaM-1.4.0/odetam/model.py
--rw-r--r--   0        0        0     2332 2023-03-24 21:26:42.706985 ODetaM-1.4.0/odetam/query.py
--rw-r--r--   0        0        0      671 2023-03-24 21:34:57.245295 ODetaM-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     7069 1970-01-01 00:00:00.000000 ODetaM-1.4.0/setup.py
--rw-r--r--   0        0        0     6843 1970-01-01 00:00:00.000000 ODetaM-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-14 17:50:37.193237 ODetaM-1.5.0/LICENSE
+-rw-r--r--   0        0        0     6072 2023-04-14 17:50:37.193347 ODetaM-1.5.0/README.md
+-rw-r--r--   0        0        0       51 2023-04-14 17:50:37.193443 ODetaM-1.5.0/odetam/__init__.py
+-rw-r--r--   0        0        0     4589 2023-04-14 17:50:37.193531 ODetaM-1.5.0/odetam/async_model.py
+-rw-r--r--   0        0        0      169 2023-04-14 17:50:37.193586 ODetaM-1.5.0/odetam/exceptions.py
+-rw-r--r--   0        0        0     4053 2023-04-14 17:50:37.193661 ODetaM-1.5.0/odetam/field.py
+-rw-r--r--   0        0        0     8554 2023-04-14 17:50:37.193761 ODetaM-1.5.0/odetam/model.py
+-rw-r--r--   0        0        0     2332 2023-04-14 17:50:37.193830 ODetaM-1.5.0/odetam/query.py
+-rw-r--r--   0        0        0      671 2023-04-14 17:52:27.522832 ODetaM-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     7069 1970-01-01 00:00:00.000000 ODetaM-1.5.0/setup.py
+-rw-r--r--   0        0        0     6843 1970-01-01 00:00:00.000000 ODetaM-1.5.0/PKG-INFO
```

### Comparing `ODetaM-1.4.0/LICENSE` & `ODetaM-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ODetaM-1.4.0/README.md` & `ODetaM-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `ODetaM-1.4.0/odetam/async_model.py` & `ODetaM-1.5.0/odetam/async_model.py`

 * *Files identical despite different names*

### Comparing `ODetaM-1.4.0/odetam/field.py` & `ODetaM-1.5.0/odetam/field.py`

 * *Files identical despite different names*

### Comparing `ODetaM-1.4.0/odetam/model.py` & `ODetaM-1.5.0/odetam/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,17 @@
 
         return as_dict
 
     @classmethod
     def _deserialize(cls, data: Dict[str, Any]) -> Self:
         as_dict: Dict[str, Any] = {}
         for field_name, field in cls.__fields__.items():
-            if data.get(field_name) is None:
+            if field_name not in data:
+                continue
+            elif data.get(field_name) is None:
                 as_dict[field_name] = None
             elif field.type_ in DETA_TYPES:
                 as_dict[field_name] = data[field_name]
             elif field.type_ == datetime.datetime:
                 as_dict[field_name] = datetime.datetime.fromtimestamp(data[field_name])
             elif field.type_ == datetime.date:
                 as_dict[field_name] = datetime.datetime.strptime(
```

### Comparing `ODetaM-1.4.0/odetam/query.py` & `ODetaM-1.5.0/odetam/query.py`

 * *Files identical despite different names*

### Comparing `ODetaM-1.4.0/pyproject.toml` & `ODetaM-1.5.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ODetaM"
-version = "1.4.0"
+version = "1.5.0"
 description = "A simple ODM (Object Document Mapper) for Deta Base, based on pydantic."
 authors = ["Rick Henry <rickhenry@rickhenry.dev>"]
 readme = "README.md"
 repository = "https://github.com/rickh94/odetam"
 
 [tool.poetry.dependencies]
 python = ">=3.7,<4.0"
```

### Comparing `ODetaM-1.4.0/setup.py` & `ODetaM-1.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['deta[async]==1.1.0a2',
  'pydantic>=1.7,<2.0',
  'typing-extensions>=4.5.0,<5.0.0',
  'ujson>=4.0,<5.0']
 
 setup_kwargs = {
     'name': 'odetam',
-    'version': '1.4.0',
+    'version': '1.5.0',
     'description': 'A simple ODM (Object Document Mapper) for Deta Base, based on pydantic.',
     'long_description': '# ODetaM\n\n[![Test](https://github.com/rickh94/ODetaM/actions/workflows/test.yml/badge.svg)](https://github.com/rickh94/ODetaM/actions/workflows/test.yml)\n[![codecov](https://codecov.io/gh/rickh94/odetam/branch/main/graph/badge.svg?token=BLDIMHU9FB)](https://codecov.io/gh/rickh94/odetam)\n\nA simple ODM (Object Document Mapper) for [Deta Base](https://deta.sh) base on\n[pydantic](https://github.com/samuelcolvin/pydantic/).\n\n## Installation\n\n`pip install odetam`\n\n## Usage\n\nCreate pydantic models as normal, but inherit from `DetaModel` instead of \npydantic BaseModel. You will need to set the environment variable \n`DETA_PROJECT_KEY` to your Deta project key so that databases can be \naccessed/created, instead you are working under deta initialized project. \nYour also can specify Deta project key in Config class of your model, for \nmigration from Deta Cloud or importing external Collection (read [DetaBase Docs](https://deta.space/docs/en/basics/data)) \nThis is a secret key, so handle it appropriately (hence the environment variable).\n\nBases will be automatically created based on model names (changed from \nPascalCase/CamelCase case to snake_case). A `key` field (Deta\'s unique id) will \nbe automatically added to any model. You can supply the key on creation, or \nDeta will generate one automatically and it will be added to the object when it \nis saved.\n\n## Async Support\n\nAsync/await is now supported! As of version 1.2.0, you can now \n`from odetam.async_model import AsyncDetaModel`, inherit from that, and run all \nthe examples below just the same, but with `await` in front of the calls.\n\nYou must `pip install deta[async]`, to use asynchronous base.\n\n\n### Get All\n\n`DetaModel.get_all()` should handle large bases better now, but you should \nconsider querying instead of getting everything if possible, because it is\nunlikely to perform well on large bases.\n\n\n## Example\n\n### Basics\n\n```python\nimport datetime\nfrom typing import List\n\nfrom odetam import DetaModel\n\n\nclass Captain(DetaModel):\n    name: str\n    joined: datetime.date\n    ships: List[str]\n\n\n# create\nkirk = Captain(\n        name="James T. Kirk",\n        joined=datetime.date(2252, 1, 1),\n        ships=["Enterprise"],\n        )\n\nsisko = Captain(\n        name="Benjamin Sisko",\n        joined=datetime.date(2350, 1, 1),\n        ships=["Deep Space 9", "Defiant"],\n        )\n\n# initial save, key is now set\nkirk.save()\n\n# update the object\nkirk.ships.append("Enterprise-A")\n\n# save again, this will be an update\nkirk.save()\n\nsisko.save()\n\nCaptain.get_all()\n# [\n#     Captain(\n#         name="James T. Kirk", \n#         joined=datetime.date(2252, 01, 01), \n#         ships=["Enterprise", "Enterprise-A"],\n#         key="key1",\n#     ),\n#     Captain(\n#         name="Benjamin Sisko",\n#         joined=datetime.date(2350, 01, 01), \n#         ships=["Deep Space 9", "Defiant"],\n#         key="key2",\n#     ),\n# ]\n\nCaptain.get("key1")\n# Captain(\n#     name="James T. Kirk", \n#     joined=datetime.date(2252, 01, 01), \n#     ships=["Enterprise", "Enterprise-A"],\n#     key="key1",\n# )\n\nCaptain.get("key3")\n# Traceback (most recent call last):\n#   File "<stdin>", line 1, in <module>\n# odetam.exceptions.ItemNotFound\n\nCaptain.get_or_none("key3")\n# None\n\nCaptain.query(Captain.name == "James T. Kirk")\n# Captain(\n#     name="James T. Kirk", \n#     joined=datetime.date(2252, 01, 01), \n#     ships=["Enterprise", "Enterprise-A"],\n#     key="key1",\n# )\n\nCaptain.query(Captain.ships.contains("Defiant"))\n# Captain(\n#     name="Benjamin Sisko",\n#     joined=datetime.date(2350, 01, 01),\n#     ships=["Deep Space 9", "Defiant"],\n# )\n\nCaptain.query(Captain.name.prefix("Ben"))\n# Captain(\n#     name="Benjamin Sisko",\n#     joined=datetime.date(2350, 01, 01),\n#     ships=["Deep Space 9", "Defiant"],\n# )\n\nkirk.delete()\nCaptain.delete_key("key2")\n\nCaptain.get_all()\n# []\n\n# you can also save several at once for better speed\nCaptain.put_many([kirk, sisko])\n# [\n#     Captain(\n#         name="James T. Kirk", \n#         joined=datetime.date(2252, 01, 01), \n#         ships=["Enterprise", "Enterprise-A"],\n#         key="key1",\n#     ),\n#     Captain(\n#         name="Benjamin Sisko",\n#         joined=datetime.date(2350, 01, 01), \n#         ships=["Deep Space 9", "Defiant"],\n#         key="key2",\n#     ),\n# ]\n\n```\n\n### Async model\n\n```python\nimport datetime\nfrom typing import List\n\nfrom odetam.async_model import AsyncDetaModel\n\n\nclass Captain(AsyncDetaModel):\n    name: str\n    joined: datetime.date\n    ships: List[str]\n\n\nasync foo():\n    items = await Captain.get_all()\n\n```\n\n### Config\n\n```python\n\nclass Captain(AsyncDetaModel):\n    name: str\n    joined: datetime.date\n    ships: List[str]\n\n    class Config:\n        table_name = "my_custom_table_name"\n        deta_key = "123_123" # project key from Deta Cloud or Data Key from another Deta Space project\n\n```\n\n## Save\n\nModels have the `.save()` method which will always behave as an upsert, \nupdating a record if it has a key, otherwise creating it and setting a key. \nDeta has pure insert behavior, but it\'s less performant. If you need it, please \nopen a pull request.\n\n## Querying\n\nAll basic comparison operators are implemented to map to their equivalents as \n`(Model.field >= comparison_value)`. There is also a `.contains()` and \n`.not_contains()` method for strings and lists of strings, as well as a \n`.prefix()` method for strings. There is also a `.range()` for number types \nthat takes a lower and upper bound. You can also use `&`  as AND and `|` as OR. \nORs cannot be nested within ands, use a list of options as comparison instead. \nYou can use as many ORs as you want, as long as they execute after the ANDs in \nthe order of operations. This is due to how the Deta Base api works.\n\n## Deta Base\n\nDirect access to the base is available in the dunder attribute `__db__`, though \nthe point is to avoid that.\n\n## Exceptions\n\n - `DetaError`: Base exception when anything goes wrong.\n - `ItemNotFound`: Fairly self-explanatory...\n - `InvalidDetaQuery`: Something is wrong with queries. Make sure you aren\'t using\n queries with unsupported types\n',
     'author': 'Rick Henry',
     'author_email': 'rickhenry@rickhenry.dev',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/rickh94/odetam',
```

### Comparing `ODetaM-1.4.0/PKG-INFO` & `ODetaM-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odetam
-Version: 1.4.0
+Version: 1.5.0
 Summary: A simple ODM (Object Document Mapper) for Deta Base, based on pydantic.
 Home-page: https://github.com/rickh94/odetam
 Author: Rick Henry
 Author-email: rickhenry@rickhenry.dev
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

