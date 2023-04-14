# Comparing `tmp/sirqle-0.1.1.tar.gz` & `tmp/sirqle-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sirqle-0.1.1.tar", last modified: Thu Nov 17 11:23:22 2022, max compression
+gzip compressed data, was "sirqle-0.1.2.tar", last modified: Fri Apr 14 11:23:04 2023, max compression
```

## Comparing `sirqle-0.1.1.tar` & `sirqle-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rw-r--r--   0        0        0     1917 2022-11-07 10:40:09.758048 sirqle-0.1.1/.gitignore
--rw-r--r--   0        0        0      576 2022-11-07 12:15:50.964311 sirqle-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0    18092 2022-11-07 10:38:03.624761 sirqle-0.1.1/LICENSE
--rw-r--r--   0        0        0      890 2022-11-07 11:37:43.881947 sirqle-0.1.1/Makefile
--rw-r--r--   0        0        0     3374 2022-11-07 12:11:35.606902 sirqle-0.1.1/README.md
--rw-r--r--   0        0        0      846 2022-10-22 22:08:14.497554 sirqle-0.1.1/docs/gen_ref_pages.py
--rw-r--r--   0        0        0     1627 2022-10-12 10:05:55.306985 sirqle-0.1.1/docs/index.md
--rw-r--r--   0        0        0      153 2022-11-07 11:23:18.775395 sirqle-0.1.1/docs/reference.md
--rw-r--r--   0        0        0      159 2022-11-07 11:22:53.858933 sirqle-0.1.1/mkdocs.yml
--rw-r--r--   0        0        0     1299 2022-11-17 11:23:13.790553 sirqle-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      294 2022-10-10 10:05:16.503669 sirqle-0.1.1/requirements.txt
--rw-r--r--   0        0        0      884 2022-10-22 21:17:01.565081 sirqle-0.1.1/requirements_dev.txt
--rw-r--r--   0        0        0       38 2022-11-02 17:12:51.611854 sirqle-0.1.1/setup.py
--rw-r--r--   0        0        0      126 2022-11-02 17:52:37.873775 sirqle-0.1.1/src/sirqle/__init__.py
--rw-r--r--   0        0        0     9389 2022-11-14 14:07:47.421918 sirqle-0.1.1/src/sirqle/query.py
--rw-r--r--   0        0        0        0 2022-10-11 09:32:28.171344 sirqle-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0     2359 2022-11-07 12:14:26.481021 sirqle-0.1.1/tests/test_query.py
--rw-r--r--   0        0        0     4258 1970-01-01 00:00:00.000000 sirqle-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      683 2023-04-13 10:02:21.646915 sirqle-0.1.2/.github/workflows/bump.yml
+-rw-r--r--   0        0        0     1917 2022-11-07 10:40:09.758048 sirqle-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1149 2023-04-12 17:02:21.974466 sirqle-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    18092 2022-11-07 10:38:03.624761 sirqle-0.1.2/LICENSE
+-rw-r--r--   0        0        0      945 2023-04-12 17:02:21.974466 sirqle-0.1.2/Makefile
+-rw-r--r--   0        0        0     3341 2023-04-12 17:02:21.974466 sirqle-0.1.2/README.md
+-rw-r--r--   0        0        0      846 2022-10-22 22:08:14.497554 sirqle-0.1.2/docs/gen_ref_pages.py
+-rw-r--r--   0        0        0     1636 2023-04-12 17:02:21.974466 sirqle-0.1.2/docs/index.md
+-rw-r--r--   0        0        0      153 2022-11-07 11:23:18.775395 sirqle-0.1.2/docs/reference.md
+-rw-r--r--   0        0        0      155 2023-02-01 08:04:46.168879 sirqle-0.1.2/mkdocs.yml
+-rw-r--r--   0        0        0     1337 2023-04-14 11:22:42.773404 sirqle-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      294 2023-02-01 08:04:46.164879 sirqle-0.1.2/requirements.txt
+-rw-r--r--   0        0        0      884 2023-02-01 08:04:46.164879 sirqle-0.1.2/requirements_dev.txt
+-rw-r--r--   0        0        0       38 2022-11-02 17:12:51.611854 sirqle-0.1.2/setup.py
+-rw-r--r--   0        0        0      126 2023-04-12 17:01:06.634486 sirqle-0.1.2/src/sirqle/__init__.py
+-rw-r--r--   0        0        0     9579 2023-04-12 17:02:21.974466 sirqle-0.1.2/src/sirqle/query.py
+-rw-r--r--   0        0        0        0 2022-10-11 09:32:28.171344 sirqle-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0     1208 2023-04-13 10:02:21.650915 sirqle-0.1.2/tests/test_create.py
+-rw-r--r--   0        0        0     3447 2023-04-12 17:02:21.974466 sirqle-0.1.2/tests/test_insert.py
+-rw-r--r--   0        0        0     4318 1970-01-01 00:00:00.000000 sirqle-0.1.2/PKG-INFO
```

### Comparing `sirqle-0.1.1/.gitignore` & `sirqle-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `sirqle-0.1.1/LICENSE` & `sirqle-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sirqle-0.1.1/Makefile` & `sirqle-0.1.2/Makefile`

 * *Files 4% similar despite different names*

```diff
@@ -3,17 +3,20 @@
 .PHONY: data, help, install
 export
 
 SHELL = /bin/zsh
 BIN = .venv_dev/bin/
 
 
-install: ## install dev venv
+warn:
+	@echo "Use make for development only!"
+
+install: warn ## install dev venv
 	@python3 -m venv .venv_dev
-	@$(BIN)pip install '.[dev]'
+	@$(BIN)pip install -e '.[dev]'
 
 startdb: ## start the database
 	@surreal start --bind 127.0.0.1:9120 --log trace --user test --pass test memory > /dev/null 2>db_log.txt &
 	@echo "SurrealDB started at 127.0.0.1:9120"
 
 test: startdb ## run the test suite
 	@echo "URL='http://127.0.0.1:9120'\nNAMESPACE='test'\nDATABASE='test'\nUSERNAME='test'\nPASSWORD='test'" > .db_conf
```

### Comparing `sirqle-0.1.1/README.md` & `sirqle-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -35,35 +35,35 @@
 # the result
 
 response = [{'company': 'SurrealDB', 'id': 'person:it2e579rij23zu0iswk4', 'name': 'Tobie', 'skills': ['Rust', 'Go', 'JavaScript']}]
 ```
 
 ## Config Module
 
-The `Config` class is used to configure the connection the database. It uses the `HTTPClient` and requires the following arguments depending on the desired method:
+The `Config` class is used to configure the connection the database. It uses the `SurrealHTTP` client and requires the following arguments depending on the desired method:
 
-> 1.Manually enter the params
+> 1. Manually enter the parameters
 
 - `url` : URL of the database
 - `namespace` : The namespace of the database
 - `database` : The name of the database
 - `username` : The access username
 - `password` : The access password
 
-> 2.Pass a previous defined client
+> 2. Pass a previous defined client
 
-- `client` : an `HTTPClient` configured beforehand
+- `client` : an `SurrealHTTP` client from `surrealdb.py`
 
-> 3.Load the params from an `.env` file
+> 3. Load the parameters from a file
 
-- `from_env`: if it set to `True` then it expects a `.db_conf` file where all the previous arguments are defined
+- `env_file`: the name of the env file. Defaults to `.db_conf`.
 
 ## Query Module
 
-The Query module aims to replace the standard SurrealQL and make it more Python friendly. Internally it constructs a SurrealQL string from method chaining and sends the query to the database.
+The Query module aims to extend the standard SurrealQL and make it more Python friendly. Internally it constructs a SurrealQL string from method chaining and sends the query to the database.
 
 ### Initialize the query
 
 ```python
 query = Query(config)
 ```
```

### Comparing `sirqle-0.1.1/docs/gen_ref_pages.py` & `sirqle-0.1.2/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `sirqle-0.1.1/docs/index.md` & `sirqle-0.1.2/docs/index.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 ## Config Module
 
-The `Config` class is used to configure the connection the database. It uses the `HTTPClient` and requires the following arguments:
+The `Config` class is used to configure the connection the database. It uses the `SurrealHTTP` and requires the following arguments:
 
 - `url` : URL of the database
 - `namespace` : The namespace of the database
 - `database` : The name of the database
 - `username` : The access username
 - `password` : The access password
-- `client` : an `HTTPClient` configured beforehand
+- `client` : an `SurrealHTTP` client configured beforehand
 - `from_env`: if it set to `True` then it expects a `.db_conf` file where all the previous arguments are defined
 
 ## Query Module
 
 The Query module aims to replace the standard SurrealQL and make it more Python friendly. Internally it constructs a SurrealQL string from method chaining and sends the query to the database.
 
 ### Initialize the query
```

### Comparing `sirqle-0.1.1/pyproject.toml` & `sirqle-0.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "sirqle"
-version = "0.1.1"
+version = "0.1.2"
 authors = [{ name = "Pythia Dev Team", email = "dev@pythia.social" }]
 description = "SurrealDB Query interface"
 readme = "README.md"
 requires-python = ">=3.10"
-dependencies = ["python-dotenv", "surrealdb"]
+dependencies = ["python-dotenv", "surrealdb==0.3.0"]
 license = { file = "LICENSE" }
 [project.urls]
 Source = "https://github.com/PythiaSocialTech/sirqle"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 include = ["sirqle*"]
@@ -21,18 +21,20 @@
 [project.optional-dependencies]
 dev = [
   "pre-commit",
   "pytest",
   "pytest-asyncio",
   "pytest-dependency",
   "commitizen",
+  "flit",
 ]
 docs = [
   "mkdocs",
   "mkdocstrings",
+  'mkdocs-material',
   "mkdocs-literate-nav",
   "mkdocstrings[python]>=0.18",
   "mkdocs-gen-files",
   "mkdocs-literate-nav",
 ]
 
 [tool.black]
@@ -47,15 +49,15 @@
 include_trailing_comma = true
 force_grid_wrap = 0
 use_parentheses = true
 ensure_newline_before_comments = true
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.1.1"
+version = "0.1.2"
 version_files = ["pyproject.toml:version"]
 tag_format = "v$version"
 bump_message = "bump: $current_version → $new_version [skip ci]"
 
 
 [tool.pytest.ini_options]
 testpaths = 'tests'
```

### Comparing `sirqle-0.1.1/requirements_dev.txt` & `sirqle-0.1.2/requirements_dev.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 aiohttp==3.8.1
 aiosignal==1.2.0
 anyio==3.6.1
 argcomplete==2.0.0
 async-timeout==4.0.2
 attrs==22.1.0
 black==22.8.0
-certifi==2022.9.14
+certifi==2022.12.7
 cfgv==3.3.1
 charset-normalizer==2.1.1
 click==8.1.3
 colorama==0.4.5
 commitizen==2.35.0
 decli==0.5.2
 distlib==0.3.6
```

### Comparing `sirqle-0.1.1/src/sirqle/query.py` & `sirqle-0.1.2/src/sirqle/query.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,119 +1,107 @@
 from __future__ import annotations
 
-import asyncio
-from distutils.util import execute
-from typing import List
+from typing import List, Optional, Tuple
 from warnings import warn
 
 from dotenv import dotenv_values
-from surrealdb.clients.http import HTTPClient
+from surrealdb.http import SurrealHTTP
 
-# query.select(*).from(query.select().from()).where(jdsaf;)
+HTTP_PARAMS = ["URL", "NAMESPACE", "USERNAME", "PASSWORD", "DATABASE"]
 
 
 class Config:
     def __init__(
         self,
-        url: str = "",
-        namespace: str = "",
-        database: str = "",
-        username: str = "",
-        password: str = "",
-        client: HTTPClient | None = None,
-        from_env: bool = False,
+        env_file: str = ".db_conf",
+        client: Optional[SurrealHTTP] = None,
+        url: Optional[str] = None,
+        namespace: Optional[str] = None,
+        database: Optional[str] = None,
+        username: Optional[str] = None,
+        password: Optional[str] = None,
     ) -> None:
         """Generate a Config class is used to configure the connection the database.
 
-        It uses the `HTTPClient` from the `surrealdb` library
+        It uses the `SurrealHTTP` client from the `surrealdb` library
 
         Args:
             url: the URL to the database
             namespace: the namespace in the database
             database: the name of the database
             username: the username used for authentication
             password: the password used for authentication
-            client: an `HTTPClient` configured beforehand
-            from_env: if it's set to True, it will load an `.db_conf` file that has all the previous arguments set
+            client: an `SurrealHTTP` client configured beforehand
+            from_env: if it's set to True, it will load an `.db_conf`
+                file that has all the previous arguments set
 
         """
         if client:
             self.client = client
-        elif from_env:
-            conf = dotenv_values(".db_conf")
-            try:
-                self.client = HTTPClient(
-                    url=conf["URL"],
-                    namespace=conf["NAMESPACE"],
-                    database=conf["DATABASE"],
-                    username=conf["USERNAME"],
-                    password=conf["PASSWORD"],
+        elif env_file:
+            conf = dotenv_values(env_file)
+            if set(HTTP_PARAMS).issubset(set(conf.keys())):
+                self.client = SurrealHTTP(
+                    **{param.lower(): conf[param] for param in HTTP_PARAMS}
                 )
-            except Exception as e:
-                print(type(e))
-                print(e)
-        else:
-            try:
-                self.client = HTTPClient(
-                    url,
-                    namespace=namespace,
-                    database=database,
-                    username=username,
-                    password=password,
-                )
-            except Exception as e:
-                print(type(e))
-                print(e)
+        elif all([username, database, password, namespace, url]):
+            self.client = SurrealHTTP(
+                url,
+                namespace=namespace,
+                database=database,
+                username=username,
+                password=password,
+            )
 
 
 class Query:
     def __init__(self, config: Config | None = None):
         """Create a `Query` class
 
-        The Query module aims to replace the standard SurrealQL and make it more Python friendly. Internally it constructs a SurrealQL string from method chaining and sends the query to the database.
+        The Query module aims to replace the standard SurrealQL and make it more Python
+            friendly. Internally it constructs a SurrealQL string from method chaining
+            and sends the query to the database.
 
         Args:
             config: a `Config` object
         """
         self.query = ""
         self.last_query = ""
-        if (
-            config
-        ):  # TODO Process config here rather than having to instantiate another Config object
+        # TODO Process config here rather than having to instantiate another
+        if config:
             self.client = config.client
 
-    def _parse_args(self, args):
+    def _parse_args(self, args: str | list | dict | tuple | Query, quote=True) -> str:
         if isinstance(args, str):
-            self.query += args
+            if quote and ":" not in args:
+                return f"'{args}'"
+            return args
         elif isinstance(args, list):
-            for arg in args:
-                self.query += arg + ","
-            self.query = self.query[:-1]
+            if quote:
+                return "[" + ", ".join([self._parse_args(arg) for arg in args]) + "]"
+            else:
+                return ", ".join(args)
         elif isinstance(args, dict):
-            self.query += "{"
-            for key, value in args.items():
-                if not isinstance(value, str):
-                    self.query += f"\n{key}: {value}, "
-                else:
-                    self.query += f"\n{key}: '{value}', "
-            self.query = self.query[:-2]
-            self.query += "\n}"
+            return (
+                "{"
+                + "".join(
+                    [
+                        f"\n{key}: {self._parse_args(value)}, "
+                        for key, value in args.items()
+                    ]
+                )
+                + "\n}"
+            )
         elif isinstance(args, tuple):
-            self.query += "("
-            for value in args:
-                if not isinstance(value, str):
-                    self.query += f"{value}, "
-                else:
-                    self.query += f"'{value}', "
-            self.query = self.query[:-2]
-            self.query += ")"
+            return (
+                "(" + ", ".join([f"{self._parse_args(value)}" for value in args]) + ")"
+            )
+
         elif isinstance(args, Query):
-            if args[-1] == ";":
-                args = args[:-1]
-            self.query += f"({args})"
+            return f"({args[:-1]})"
 
     def custom(self, args: str) -> Query:
         """Create a simple query in SurrealQL.
 
 
         Args:
             args: a string containing a full and correct query
@@ -122,216 +110,226 @@
             Query: returns the same `Query` object
         """
         self.query += args
         return self
 
     def select(self, args: str | List[str]) -> Query:
         """SELECT statement.
-
         Args:
+
             args: a table or a list of tables
 
         Returns:
             Query: returns the same `Query` object
         """
         self.query = " SELECT "
-        self._parse_args(args)
+        self.query += self._parse_args(args, quote=False)
         return self
 
-    def from_(self, args: str | list | dict | Query) -> Query:
-        """FROM statement.
+    def insert(
+        self, args: str, values: Tuple[str] | List[Tuple[str]] | dict | str = ""
+    ) -> Query:
+        """INSERT statement.
 
         Args:
             args: arguments for the statement
 
         Returns:
             Query: returns the same `Query` object
         """
-        self.query += " FROM "
-        self._parse_args(args)
+        self.query += "INSERT INTO "
+        self.query += self._parse_args(args, quote=False) + " "
+        if values:
+            if isinstance(values, (str, tuple)):
+                self.query += " VALUES "
+                self.query += self._parse_args(values)
+            elif isinstance(values, (list, dict)):
+                self.query += self._parse_args(values)
+            else:
+                raise NotImplementedError()
         return self
 
-    def where(self, args: str | list | dict | Query) -> Query:
-        """WHERE statement.
+    def create(self, args: str | list | dict | Query) -> Query:
+        """CREATE statement.
 
         Args:
             args: arguments for the statement
 
         Returns:
             Query: returns the same `Query` object
         """
-        if args:
-            self.query += " WHERE "
-            self._parse_args(args)
-        else:
-            warn(
-                "No arguments for RETURN statement. RETURN statement not added to the query."
-            )
+        self.query += " CREATE "
+        self.query += self._parse_args(args, quote=False)
         return self
 
-    def use(self, args: str | list | dict | Query) -> Query:
-        """USE statement.
+    def update(self, args: str | list | dict | Query) -> Query:
+        """UPDATE statement.
 
         Args:
             args: arguments for the statement
 
         Returns:
             Query: returns the same `Query` object
         """
-        self.query += " USE "
-        self._parse_args(args)
+        self.query += " UPDATE "
+        self.query += self._parse_args(args, quote=False)
         return self
 
-    def return_(self, args: str | list | dict | Query | None) -> Query:
-        """RETURN statement.
+    def relate(
+        self,
+        node1: str,
+        edge: str,
+        node2: str,
+        args: str | list | dict | Query | None = None,
+    ) -> Query:
+        """RELATE statement.
+
+        Create a relation between two nodes.
 
         Args:
+            node1: the source node
+            edge: name of the relation
+            node2: the destination node
             args: arguments for the statement
 
         Returns:
             Query: returns the same `Query` object
         """
+        self.query += f" RELATE {node1}->{edge}->{node2}"
         if args:
-            self.query += " RETURN "
-            self._parse_args(args)
-        else:
-            warn(
-                "No arguments for RETURN statement. RETURN statement not added to the query."
-            )
+            self.query += " CONTENT "
+            self.query += self._parse_args(args)
         return self
 
-    def insert(
-        self, args: str | list | dict | Query, values: tuple[str] | str = ""
-    ) -> Query:
-        """INSERT statement.
+    def delete(self, args: str | list | dict | Query) -> Query:
+        """DELETE statement.
 
         Args:
             args: arguments for the statement
 
         Returns:
             Query: returns the same `Query` object
         """
-        self.query += "INSERT INTO "
-        if values:
-            if isinstance(args, str):
-                self.query += args
-                self.query += " VALUES "
-                self._parse_args(values)
-            else:
-                raise Exception(
-                    f"Incorrect argument type, expected {type(str)} got {type(args)}"
-                )
-        else:
-            self._parse_args(args)
-
+        self.query += " DELETE "
+        self.query += self._parse_args(args)
         return self
 
-    def delete(self, args: str | list | dict | Query) -> Query:
-        """DELETE statement.
+    def DEFINE(self, args: str | list | dict | Query) -> Query:
+        """DEFINE statement.
 
         Args:
             args: arguments for the statement
 
         Returns:
             Query: returns the same `Query` object
         """
         self.query += " DELETE "
-        self._parse_args(args)
+        self.query += self._parse_args(args)
         return self
 
-    def update(self, args: str | list | dict | Query) -> Query:
-        """UPDATE statement.
+    def from_(self, args: str | list | dict | Query) -> Query:
+        """FROM statement.
 
         Args:
             args: arguments for the statement
 
         Returns:
             Query: returns the same `Query` object
         """
-        self.query += " UPDATE "
-        self._parse_args(args)
+        self.query += " FROM "
+        self.query += self._parse_args(args, quote=False)
         return self
 
-    def create(self, args: str | list | dict | Query) -> Query:
-        """CREATE statement.
+    def where(self, args: str | list | dict | Query) -> Query:
+        """WHERE statement.
 
         Args:
             args: arguments for the statement
 
         Returns:
             Query: returns the same `Query` object
         """
-        self.query += " CREATE "
-        self._parse_args(args)
+        if args:
+            self.query += " WHERE "
+            self.query += self._parse_args(args)
+        else:
+            warn(
+                "No arguments for RETURN statement. RETURN statement not \
+                added to the query."
+            )
         return self
 
-    def relate(
-        self,
-        node1: str,
-        edge: str,
-        node2: str,
-        args: str | list | dict | Query | None = None,
-    ) -> Query:
-        """RELATE statement.
+    def use(self, args: str | list | dict | Query) -> Query:
+        """USE statement.
 
-        Create a relation between two nodes.
+        Args:
+            args: arguments for the statement
+
+        Returns:
+            Query: returns the same `Query` object
+        """
+        self.query += " USE "
+        self.query += self._parse_args(args)
+        return self
+
+    def return_(self, args: str | list | dict | Query | None) -> Query:
+        """RETURN statement.
 
         Args:
-            node1: the source node
-            edge: name of the relation
-            node2: the destination node
             args: arguments for the statement
 
         Returns:
             Query: returns the same `Query` object
         """
-        self.query += f" RELATE {node1}->{edge}->{node2}"
         if args:
-            self.query += " CONTENT "
-            self._parse_args(args)
+            self.query += " RETURN "
+            self.query += self._parse_args(args)
+        else:
+            warn(
+                "No arguments for RETURN statement. RETURN statement not \
+                added to the query."
+            )
         return self
 
     def content(self, args: str | list | dict | Query) -> Query:
         """CONTENT statement.
 
         Args:
             args: arguments for the statement
 
         Returns:
             Query: returns the same `Query` object
         """
         self.query += " CONTENT "
-        self._parse_args(args)
+        self.query += self._parse_args(args)
         return self
 
-    # NOTE: do we still need this?
-    def __getitem__(self, key):
-        return self.query[key]
-
     def _end(self):
-        if self.query[0] == " ":
-            self.query = self.query[1:]
+        self.query = self.query.strip()
         if self.query[-1] != ";":
             self.query += ";"
 
     async def _execute_query(self):
         self._end()
-        res = await self.client.execute(self.query)
+        res = await self.client.query(self.query)
         self.last_query = self.query
         self.query = ""
         return res
 
     async def execute(self):
         """Execute the query.
 
         Send the query to the databse and get the answert.
 
         """
-        if self.client == None:
+        if self.client is None:
             raise Exception("No client provided!")
         res = await self._execute_query()
         return res
 
     # HACK:
     def __repr__(self):
         self._end()
         return self.query
+
+    def __getitem__(self, key):
+        return self.query[key]
```

### Comparing `sirqle-0.1.1/tests/test_query.py` & `sirqle-0.1.2/tests/test_insert.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,80 +1,111 @@
 import asyncio
 
 import pytest
 
 from sirqle.query import Config, Query
 
-config = Config(from_env=True)
+config = Config(
+    url="127.0.0.1:9120",
+    namespace="test",
+    database="test_insert",
+    password="test",
+    username="test",
+)
 
 
 @pytest.fixture(scope="session")
 def event_loop():
     try:
         loop = asyncio.get_running_loop()
     except RuntimeError:
         loop = asyncio.new_event_loop()
     yield loop
     loop.close()
 
 
-@pytest.mark.asyncio
-async def test_create():
-    """Test the functionality of CREATE.
-
-    Create an entry in the database.
-    """
-    create_query = Query(config=config)
-    table_name = "person"
-    cont = {
-        "name": "Tobie",
-        "company": "SurrealDB",
-        "skills": ["Rust", "Go", "JavaScript"],
+class TestInsert:
+    data = {
+        "name": "SurrealDB",
+        "founded": "2021-09-10",
+        "founders": ["tobie", "jaime"],
+        "tags": ["big data", "database"],
     }
-    create_query.create(table_name).content(cont)
-    res = await create_query.execute()
-    assert res[0]["id"].split(":")[0] == table_name
-    assert res[0]["company"] == cont["company"]
-    assert res[0]["skills"] == cont["skills"]
-    assert res[0]["name"] == cont["name"]
-
-
-@pytest.mark.asyncio
-@pytest.mark.dependency(on=["test_create"])
-async def test_select():
-    """Test the functionality of CREATE by looking in the database."""
-    query = Query(config=config)
-    query.select(["name", "company", "skills"]).from_("person")
-    res = await query.execute()
-    assert res[0]["company"] == "SurrealDB"
-    assert res[0]["skills"] == ["Rust", "Go", "JavaScript"]
-    assert res[0]["name"] == "Tobie"
-
-
-@pytest.mark.asyncio
-async def test_insert():
-    """Test the functionality of INSERT.
-
-    Create an entry in the database.
-    """
-    insert_query = Query(config=config)
-    table_name = "person (name, company, founded)"
+
+    @pytest.mark.asyncio
+    async def test_insert(self):
+        """Test the functionality of INSERT.
+
+        Create an entry in the database.
+        """
+        insert_query = Query(config=config)
+        table_name = "company"
+        insert_query.insert(table_name, values=self.data)
+        res = await insert_query.execute()
+        res = res[0]["result"]
+        assert res[0]["id"].split(":")[0] == table_name.split(" ")[0]
+        assert res[0]["name"] == self.data["name"]
+        assert res[0]["founded"] == "2021-09-10T00:00:00Z"
+        assert res[0]["name"] == self.data["name"]
+
+
+class TestInsertSQL:
+    table_name = "person"
     data = tuple(["John", "SurrealDB", "2021-09-10"])
-    insert_query.insert(table_name, values=data)
-    res = await insert_query.execute()
-    assert res[0]["id"].split(":")[0] == table_name.split(" ")[0]
-    assert res[0]["company"] == "SurrealDB"
-    assert res[0]["founded"] == "2021-09-10T00:00:00Z"
-    assert res[0]["name"] == "John"
-
-
-@pytest.mark.asyncio
-@pytest.mark.dependency(on=["test_insert"])
-async def test_select2():
-    """Test the functionality of INSERT by looking in the database."""
-    query = Query(config=config)
-    query.select("*").from_("person")
-    res = await query.execute()
-    assert res[0]["company"] == "SurrealDB"
-    assert res[0]["founded"] == "2021-09-10T00:00:00Z"
-    assert res[0]["name"] == "John"
-    assert res[0]["id"].split(":")[0] == "person"
+    SQL = "INSERT INTO company (name, founded) VALUES ('SurrealDB', '2021-09-10');"
+
+    @pytest.mark.asyncio
+    async def test_insert_sql(self):
+        """Test the functionality of INSERT.
+
+        Create an entry in the database.
+        """
+        insert_query = Query(config=config)
+        table_name = f"{self.table_name} (name, company, founded)"
+        insert_query.insert(table_name, values=self.data)
+        res = await insert_query.execute()
+        res = res[0]["result"]
+        assert res[0]["company"] == "SurrealDB"
+        assert res[0]["founded"] == "2021-09-10T00:00:00Z"
+        assert res[0]["name"] == "John"
+
+    @pytest.mark.asyncio
+    @pytest.mark.dependency(on=["test_insert_sql"])
+    async def test_select(self):
+        """Test the functionality of INSERT by looking in the database."""
+        query = Query(config=config)
+        query.select("*").from_(self.table_name)
+        res = await query.execute()
+        res = res[0]["result"]
+        assert res[0]["company"] == self.data[1]
+        assert res[0]["founded"] == "2021-09-10T00:00:00Z"
+        assert res[0]["name"] == self.data[0]
+
+
+class TestInsertValue:
+    table = "company"
+    table_name = f"{table} (name, founded)"
+    data = tuple(["SurrealDB", "2021-09-10"])
+
+    @pytest.mark.asyncio
+    async def test_insert_value(self):
+        """Test the functionality of INSERT.
+
+        Create an entry in the database.
+        """
+        insert_query = Query(config=config)
+        insert_query.insert(self.table_name, values=self.data)
+        res = await insert_query.execute()
+        res = res[0]["result"]
+        assert res[0]["name"] == "SurrealDB"
+        assert res[0]["founded"] == "2021-09-10T00:00:00Z"
+
+    @pytest.mark.asyncio
+    @pytest.mark.dependency(on=["test_insert_value"])
+    async def test_select2(self):
+        """Test the functionality of INSERT by looking in the database."""
+        query = Query(config=config)
+        query.select("*").from_(self.table)
+        res = await query.execute()
+        res = res[0]["result"]
+        assert res[0]["name"] == "SurrealDB"
+        assert res[0]["founded"] == "2021-09-10T00:00:00Z"
```

### Comparing `sirqle-0.1.1/PKG-INFO` & `sirqle-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: sirqle
-Version: 0.1.1
+Version: 0.1.2
 Summary: SurrealDB Query interface
 Author-email: Pythia Dev Team <dev@pythia.social>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: python-dotenv
-Requires-Dist: surrealdb
+Requires-Dist: surrealdb==0.3.0
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: pytest ; extra == "dev"
 Requires-Dist: pytest-asyncio ; extra == "dev"
 Requires-Dist: pytest-dependency ; extra == "dev"
 Requires-Dist: commitizen ; extra == "dev"
+Requires-Dist: flit ; extra == "dev"
 Requires-Dist: mkdocs ; extra == "docs"
 Requires-Dist: mkdocstrings ; extra == "docs"
+Requires-Dist: mkdocs-material ; extra == "docs"
 Requires-Dist: mkdocs-literate-nav ; extra == "docs"
 Requires-Dist: mkdocstrings[python]>=0.18 ; extra == "docs"
 Requires-Dist: mkdocs-gen-files ; extra == "docs"
 Requires-Dist: mkdocs-literate-nav ; extra == "docs"
 Project-URL: Source, https://github.com/PythiaSocialTech/sirqle
 Provides-Extra: dev
 Provides-Extra: docs
@@ -59,35 +61,35 @@
 # the result
 
 response = [{'company': 'SurrealDB', 'id': 'person:it2e579rij23zu0iswk4', 'name': 'Tobie', 'skills': ['Rust', 'Go', 'JavaScript']}]
 ```
 
 ## Config Module
 
-The `Config` class is used to configure the connection the database. It uses the `HTTPClient` and requires the following arguments depending on the desired method:
+The `Config` class is used to configure the connection the database. It uses the `SurrealHTTP` client and requires the following arguments depending on the desired method:
 
-> 1.Manually enter the params
+> 1. Manually enter the parameters
 
 - `url` : URL of the database
 - `namespace` : The namespace of the database
 - `database` : The name of the database
 - `username` : The access username
 - `password` : The access password
 
-> 2.Pass a previous defined client
+> 2. Pass a previous defined client
 
-- `client` : an `HTTPClient` configured beforehand
+- `client` : an `SurrealHTTP` client from `surrealdb.py`
 
-> 3.Load the params from an `.env` file
+> 3. Load the parameters from a file
 
-- `from_env`: if it set to `True` then it expects a `.db_conf` file where all the previous arguments are defined
+- `env_file`: the name of the env file. Defaults to `.db_conf`.
 
 ## Query Module
 
-The Query module aims to replace the standard SurrealQL and make it more Python friendly. Internally it constructs a SurrealQL string from method chaining and sends the query to the database.
+The Query module aims to extend the standard SurrealQL and make it more Python friendly. Internally it constructs a SurrealQL string from method chaining and sends the query to the database.
 
 ### Initialize the query
 
 ```python
 query = Query(config)
 ```
```

