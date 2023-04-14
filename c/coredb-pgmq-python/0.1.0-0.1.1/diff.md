# Comparing `tmp/coredb_pgmq_python-0.1.0.tar.gz` & `tmp/coredb_pgmq_python-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coredb_pgmq_python-0.1.0.tar", max compression
+gzip compressed data, was "coredb_pgmq_python-0.1.1.tar", max compression
```

## Comparing `coredb_pgmq_python-0.1.0.tar` & `coredb_pgmq_python-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1465 2023-04-14 18:13:23.241886 coredb_pgmq_python-0.1.0/README.md
--rw-r--r--   0        0        0      106 2023-04-14 18:13:23.241886 coredb_pgmq_python-0.1.0/coredb_pgmq_python/__init__.py
--rw-r--r--   0        0        0     3485 2023-04-14 18:13:23.241886 coredb_pgmq_python-0.1.0/coredb_pgmq_python/queue.py
--rw-r--r--   0        0        0      745 2023-04-14 18:13:23.241886 coredb_pgmq_python-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2256 1970-01-01 00:00:00.000000 coredb_pgmq_python-0.1.0/setup.py
--rw-r--r--   0        0        0     2106 1970-01-01 00:00:00.000000 coredb_pgmq_python-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1465 2023-04-14 18:23:56.964191 coredb_pgmq_python-0.1.1/README.md
+-rw-r--r--   0        0        0      106 2023-04-14 18:23:56.964191 coredb_pgmq_python-0.1.1/coredb_pgmq_python/__init__.py
+-rw-r--r--   0        0        0     3485 2023-04-14 18:23:56.964191 coredb_pgmq_python-0.1.1/coredb_pgmq_python/queue.py
+-rw-r--r--   0        0        0     1015 2023-04-14 18:23:56.964191 coredb_pgmq_python-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2256 1970-01-01 00:00:00.000000 coredb_pgmq_python-0.1.1/setup.py
+-rw-r--r--   0        0        0     2380 1970-01-01 00:00:00.000000 coredb_pgmq_python-0.1.1/PKG-INFO
```

### Comparing `coredb_pgmq_python-0.1.0/README.md` & `coredb_pgmq_python-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `coredb_pgmq_python-0.1.0/coredb_pgmq_python/queue.py` & `coredb_pgmq_python-0.1.1/coredb_pgmq_python/queue.py`

 * *Files identical despite different names*

### Comparing `coredb_pgmq_python-0.1.0/setup.py` & `coredb_pgmq_python-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_requires = \
 ['orjson>=3.8.10,<4.0.0',
  'psycopg[binary,pool]>=3.1.8,<4.0.0',
  'pydantic>=1.10.7,<2.0.0']
 
 setup_kwargs = {
     'name': 'coredb-pgmq-python',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'Python client for the PGMQ Postgres extension.',
     'long_description': '# Coredb\'s Python Client for PGMQ\n\n## Installation\n\nInstall with `pip` from pypi.org\n\n```bash\npip install coredb-pgmq-python\n```\n\nDependencies\n\nPostgres running the [CoreDB PGMQ extension](https://github.com/CoreDB-io/coredb/tree/main/extensions/pgmq).\n\n## Usage\n\n## Start a Postgres Instance with the CoreDB extension installed\n\n```bash\ndocker run -d -p 5432:5432 quay.io/coredb/coredb-pg:latest\n```\n\nInitialize a connection to Postgres\n\n```python\n\nfrom coredb_pgmq_python import PGMQueue, Message\n\nqueue = PGMQueue(host="0.0.0.0")\n```\n\nCreate a queue (or a partitioned queue)\n\n```python\nqueue.create_queue("my_queue")\n# queue.create_partitioned_queue("my_partitioned_queue", partition_size=10000)\n```\n\n\nSend a message\n\n```python\nmsg_id: int = queue.send("my_queue", {"hello": "world"})\n```\n\nRead a message, set it invisible for 30 seconds.\n\n```python\nread_message: Message = queue.read("my_queue", vt=10)\nprint(read_message)\n```\n\nArchive the message after we\'re done with it. Archived messages are moved to an archive table.\n\n```python\narchived: bool = queue.archive("my_queue", read_message.msg_id)\n```\n\nDelete a message completely.\n\n```python\nmsg_id: int = queue.send("my_queue", {"hello": "world"})\nread_message: Message = queue.read("my_queue")\ndeleted: bool = queue.delete("my_queue", read_message.msg_id)\n```\n\nPop a message, deleting it and reading it in one transaction.\n\n```python\npopped_message: Message = queue.pop("my_queue")\nprint(popped_message)\n```\n',
     'author': 'Adam Hendel',
     'author_email': 'adam@coredb.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `coredb_pgmq_python-0.1.0/PKG-INFO` & `coredb_pgmq_python-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: coredb-pgmq-python
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python client for the PGMQ Postgres extension.
 License: Apache 2.0
 Author: Adam Hendel
 Author-email: adam@coredb.io
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: orjson (>=3.8.10,<4.0.0)
 Requires-Dist: psycopg[binary,pool] (>=3.1.8,<4.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
+Project-URL: Documentation, https://github.com/CoreDB-io/coredb/tree/main/extensions/pgmq/coredb-pgmq-python
+Project-URL: Homepage, https://github.com/CoreDB-io/coredb
+Project-URL: Repository, https://github.com/CoreDB-io/coredb/tree/main/extensions/pgmq/coredb-pgmq-python
 Description-Content-Type: text/markdown
 
 # Coredb's Python Client for PGMQ
 
 ## Installation
 
 Install with `pip` from pypi.org
```

