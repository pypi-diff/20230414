# Comparing `tmp/alfred5-1.1.2.tar.gz` & `tmp/alfred5-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alfred5-1.1.2.tar", last modified: Thu Apr 13 21:31:33 2023, max compression
+gzip compressed data, was "alfred5-1.1.3.tar", last modified: Fri Apr 14 09:48:46 2023, max compression
```

## Comparing `alfred5-1.1.2.tar` & `alfred5-1.1.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:31:33.867080 alfred5-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-04-13 21:31:22.000000 alfred5-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-13 21:31:22.000000 alfred5-1.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-04-13 21:31:33.867080 alfred5-1.1.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:31:33.867080 alfred5-1.1.2/alfred5/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-13 21:31:22.000000 alfred5-1.1.2/alfred5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9960 2023-04-13 21:31:22.000000 alfred5-1.1.2/alfred5/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-13 21:31:22.000000 alfred5-1.1.2/alfred5/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:31:33.867080 alfred5-1.1.2/alfred5/icons/
--rw-r--r--   0 runner    (1001) docker     (123)    14257 2023-04-13 21:31:22.000000 alfred5-1.1.2/alfred5/icons/download.png
--rw-r--r--   0 runner    (1001) docker     (123)    35477 2023-04-13 21:31:22.000000 alfred5-1.1.2/alfred5/icons/error.png
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-04-13 21:31:22.000000 alfred5-1.1.2/alfred5/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:31:33.867080 alfred5-1.1.2/alfred5.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-04-13 21:31:33.000000 alfred5-1.1.2/alfred5.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-13 21:31:33.000000 alfred5-1.1.2/alfred5.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 21:31:33.000000 alfred5-1.1.2/alfred5.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 21:31:33.000000 alfred5-1.1.2/alfred5.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-13 21:31:33.000000 alfred5-1.1.2/alfred5.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-13 21:31:33.000000 alfred5-1.1.2/alfred5.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:31:33.867080 alfred5-1.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-04-13 21:31:22.000000 alfred5-1.1.2/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 21:31:33.867080 alfred5-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-13 21:31:22.000000 alfred5-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 21:31:33.867080 alfred5-1.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 21:31:22.000000 alfred5-1.1.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-13 21:31:22.000000 alfred5-1.1.2/tests/test_snippets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:48:46.542957 alfred5-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-04-14 09:48:35.000000 alfred5-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-14 09:48:35.000000 alfred5-1.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5405 2023-04-14 09:48:46.542957 alfred5-1.1.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:48:46.538957 alfred5-1.1.3/alfred5/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-14 09:48:35.000000 alfred5-1.1.3/alfred5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11588 2023-04-14 09:48:35.000000 alfred5-1.1.3/alfred5/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-14 09:48:35.000000 alfred5-1.1.3/alfred5/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:48:46.542957 alfred5-1.1.3/alfred5/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)    14257 2023-04-14 09:48:35.000000 alfred5-1.1.3/alfred5/icons/download.png
+-rw-r--r--   0 runner    (1001) docker     (123)    35477 2023-04-14 09:48:35.000000 alfred5-1.1.3/alfred5/icons/error.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-04-14 09:48:35.000000 alfred5-1.1.3/alfred5/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:48:46.542957 alfred5-1.1.3/alfred5.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5405 2023-04-14 09:48:46.000000 alfred5-1.1.3/alfred5.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-14 09:48:46.000000 alfred5-1.1.3/alfred5.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 09:48:46.000000 alfred5-1.1.3/alfred5.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 09:48:46.000000 alfred5-1.1.3/alfred5.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-14 09:48:46.000000 alfred5-1.1.3/alfred5.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-14 09:48:46.000000 alfred5-1.1.3/alfred5.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:48:46.542957 alfred5-1.1.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-04-14 09:48:35.000000 alfred5-1.1.3/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 09:48:46.542957 alfred5-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-14 09:48:35.000000 alfred5-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:48:46.542957 alfred5-1.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:48:35.000000 alfred5-1.1.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-14 09:48:35.000000 alfred5-1.1.3/tests/test_snippets.py
```

### Comparing `alfred5-1.1.2/LICENSE` & `alfred5-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alfred5-1.1.2/PKG-INFO` & `alfred5-1.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alfred5
-Version: 1.1.2
+Version: 1.1.3
 Summary: Simple python wrapper for alfred5 workflow / snippets
 Home-page: https://github.com/yedhrab/alfred5
 Author: Yunus Emre Ak
 Author-email: yemreak.com@gmail.com
 License: Apache Software License 2.0
 Project-URL: Source, https://github.com/yedhrab/alfred5/
 Project-URL: Changelog, https://github.com/yedhrab/alfred5/releases
@@ -23,37 +23,44 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 #  🎩 AlfredClient
 
 Simplest Alfred Client that I use my own projects.
 
+## Usage
+
 ```bash
 pip install alfred5
 ```
-
+- Projects dir structure
+    - Put your codes and `requirements.txt` to `src` folders
+    - Install `alfred5` via 
+        ```bash
+        pip install alfred5 --target=src/lib
+        ```
+    - If u want to use different `--target` for ex `.` use `WorkflowClient.run(packagedir=".")`
+    - Sample of default structure: 
+        - ![structure](https://i.imgur.com/doLWDR4.png)
+    - **If u install all of requirements, dont need to create `requirements.txt` file in `src`**
 - Via `SnippetsClient` API create custom snippets programmaically
 - Via `WorkflowClient` API create custom alfred workflow
     - Craete `requirements.txt` file for your python project to let `alfred5` installs them if needed 🙃
     - To install `from requirements.txt` do all import packages inside `main`
             - Use `global` keyword to access imported packages globally
         - `client.query` is the query string
         - `client.page_count` is the page count for pagination results
     - Dont need to add `alfred5` to `requirements.txt`
 - Use `WorkflowClient.log` to log your message to alfred debugger 
     - [debugging alfred workflow](https://www.alfredapp.com/help/workflows/utilities/debug/)
     - [why this project use stderr for all logging operation](https://www.alfredforum.com/topic/14721-get-the-python-output-back-to-alfred/?do=findComment&comment=75303)
-- Use `client.load_cached_response` and `client.cache_response` method to use caching system
-    - Just do it for static response (not timebased response)
+- Use `WorkflowClient(main, cache=True)` method to use caching system
+    - Just do it for static (not timebased nor any dynamic stuff) response 
     - Db path is `db/results.yml` also you can see it from workflow debug panel
 
-## Example Db Format
-
-![example-db](https://i.imgur.com/r2whZsi.png)
-
 ## ⭐️ Example Project
 
 ![alt](https://i.imgur.com/tUJjVUJ.png)
 
 ```python
 from re import sub
 from urllib.parse import quote_plus
@@ -65,15 +72,15 @@
     # To auto install requirements all import operation must be in here
     global get
     from requests import get
 
     query = client.query
     client.log(f"my query: {query}")  # use it to see your log in workflow debug panel
 
-    # (use cache=True) Use cache system to quick response
+    # (use cache=True) Use cache system to quick response instead of old style that below
     # if client.load_cached_response():
     #     return
 
     char_count = str(len( query))
     word_count = str(len(query.split(" ")))
     line_count = str(len(query.split("\n")))
 
@@ -91,19 +98,20 @@
     client.add_result(lower_case, "Lower Case", arg=lower_case)
     client.add_result(capitalized, "Capitalized", arg=capitalized)
     client.add_result(template, "Template", arg=template)
     client.add_result(char_count, "Characters", arg=char_count)
     client.add_result(word_count, "Words", arg=word_count)
     client.add_result(line_count, "Lines", arg=line_count)
     
-    # (use cache=True) to cache result for query (if u work with static results (not dynamic; coin price etc.))
+    # (use cache=True) to cache result for query instead of old style that below
+    #     if u work with static results (not dynamic; coin price etc.)
     # client.cache_response()  
 
 if __name__ == "__main__":
-    WorkflowClient.run(main)
+    WorkflowClient.run(main)  # WorkflowClient.run(main, cache=True)
 
 ```
 
 
 ## 🔰 How to Create Workflow
 
 ![insturaction1](https://i.imgur.com/2oDMChr.png)
```

### Comparing `alfred5-1.1.2/alfred5/client.py` & `alfred5-1.1.3/alfred5/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,41 +54,46 @@
                     zipfile.write(snippet_iconpath, snippet_iconpath.name)
 
             destination = (Path(dst) if dst else Path.cwd()) / f"{name}.alfredsnippets"
             move(snippet_path, destination)
 
 
 class WorkflowClient:
-    bare_query: str
-    query: str
+    bare_query: str | None
+    query: str | None
     page_count: int
-    bundleid: str
 
+    bundleid: str
+    package_dir: Path
     icondir: Path
-
     datadir: Path
     db_results: Path
-
     results: list[Result]
 
     logger: Logger
 
-    def __init__(self) -> None:
+    def __init__(self, package_dir: str = "src/libs") -> None:
         self.logger = Logger("alfred5")
         self.logger.addHandler(StreamHandler(sys.stderr))
         self.log(f"logger initted")
 
-        self.bare_query = sys.argv[1]
-        self.page_count = self.bare_query.count("+") + 1
-        self.query = self.bare_query.replace("+", "")
+        if len(sys.argv) > 1:
+            self.bare_query = sys.argv[1]
+            self.page_count = self.bare_query.count("+") + 1
+            self.query = self.bare_query.replace("+", "")
+        else:
+            self.bare_query = None
+            self.page_count = 0
+            self.query = None
 
         self.log(
             f"sys.argv: {sys.argv} page_count: {self.page_count} query: {self.query}"
         )
 
+        self.package_dir = Path(package_dir)
         self.icondir = Path(__file__).parent / "icons"
 
         self.log(f"bundleid reading from info.plist...")
         with Path("info.plist").open("rb") as f:
             self.bundleid = plist_load(f)["bundleid"]
             self.log(f"bundleid: {self.bundleid}")
         self.datadir = Path("db")
@@ -104,38 +109,45 @@
 
     def log(self, msg: str):
         self.logger.debug(msg)
 
     def install_requirements(self) -> None:
         """Check if requirements are met"""
         self.log(f"checking requirements...")
-        req_file = Path("requirements.txt")
+        req_file = self.package_dir / ".." / "requirements.txt"
         if req_file.exists():
             packages = req_file.read_text().splitlines()
             self.log(f"found requirements.txt: {packages}")
 
             try:
                 pkg_resources.require(packages)
             except pkg_resources.DistributionNotFound:
                 import subprocess
 
-                command = ["python3", "-m", "pip", "install", "--target=.", *packages]
+                command = [
+                    "python3",
+                    "-m",
+                    "pip",
+                    "install",
+                    f"--target={self.package_dir}",
+                    *packages,
+                ]
                 subprocess.Popen(
                     command,
                     start_new_session=True,
                     stdout=subprocess.DEVNULL,
                     stderr=subprocess.DEVNULL,
                 )
                 self.add_result(
                     title="Requirements are installing (you can close alfred)",
                     subtitle=f"Executed command: {' '.join(command)}",
                     icon_path=self.icondir / "download.png",
                     arg=" ".join(command),
                 )
-                self.response()
+                self.response_with_results()
         else:
             self.log(f"no requirements.txt found")
 
     def cache_response(self) -> None:
         """Cache response to workflow db_results"""
         if not self.db_results.exists():
             self.db_results.parent.mkdir(parents=True, exist_ok=True)
@@ -153,20 +165,24 @@
         ]
         with self.db_results.open("w") as f:
             yaml_dump(data, f)
             self.log(f"cached response to {self.db_results}")
 
     def load_cached_response(self) -> bool:
         """Load cached result from alfred"""
+        if self.bare_query:
+            self.log("skipped, bare_query is None")
+            return False
+
         self.log(f"checking if `{self.bare_query}` exists in `{self.db_results}`")
         if self.db_results.exists():
             with self.db_results.open("r") as f:
                 data: dict[str, list[dict[str, str]]] = self.yaml.load(f)
                 self.log(f"loaded data from {self.db_results} {len(data.keys())}")
-                if self.bare_query in data:
+                if self.bare_query and self.bare_query in data:
                     self.results = [
                         Result(
                             title=result["title"],
                             subtitle=result["subtitle"],
                             icon=Result.Icon(result["icon_path"])
                             if result["icon_path"]
                             else None,
@@ -180,20 +196,22 @@
         return False
 
     @classmethod
     def run(
         cls,
         func: Callable[[WorkflowClient], Coroutine[None, None, None]],
         cache: bool = False,
+        package_dir: str = "src/libs",
     ) -> NoReturn:
         """Give async main function, no need to call `client.response` method
 
         Args:
             `func`: async main function that takes `client` as argument
             `cache`: cache response to workflow db_results, if cache exists, it will be loaded instead of executing `func`
+            `package_dir`: directory to install `requirements.txt` packages
 
         - To install `from requirements.txt` do all import packages inside it
             - Use `global` keyword to access imported packages globally
         - `client.bare_query` is the bare query string
         - `client.query` is the query string without `+` (page count)
         - `client.page_count` is the page count for pagination results
 
@@ -206,23 +224,24 @@
                 from requests import get
                 pass
 
             if __name__ == "__main__":
                 WorkflowClient.run(main)
             ```
         """
-        client = cls()
+        client = cls(package_dir=package_dir)
+        sys.path.insert(0, package_dir)
         if cache and client.load_cached_response():
-            client.response()
+            client.response_with_results()
         try:
             client.install_requirements()
             run(func(client))
             if cache:
                 client.cache_response()
-            client.response()
+            client.response_with_results()
         except Exception as e:
             if isinstance(e, WorkflowError):
                 client.error_response(
                     title=e.title,
                     subtitle=e.subtitle,
                     arg=e.arg,
                 )
@@ -274,16 +293,46 @@
         """
         self.add_result(
             title=title,
             subtitle=subtitle,
             icon_path=icon_path or self.icondir / "error.png",
             arg=arg,
         )
-        self.response()
+        self.response_with_results()
 
-    def response(self) -> NoReturn:
-        """Print alfred results and exit
+    def response_with_results(self) -> NoReturn:
+        """Print saved alfred results and exit
 
         - terminate: terminate workflow
         """
         print(json.dumps({"items": [result.to_dict() for result in self.results]}))
         exit(0)
+
+    def response(
+        self,
+        title: str,
+        subtitle: str = "",
+        icon_path: str | Path | None = None,
+        arg: str = "",
+    ) -> NoReturn:
+        """Print alfred result and exit
+
+        - title: result title
+        - subtitle: result subtitle
+        - icon_path: result icon path
+        - arg: argument to pass to alfred
+        """
+        print(
+            json.dumps(
+                {
+                    "items": [
+                        Result(
+                            title=title,
+                            subtitle=subtitle,
+                            icon=Result.Icon(str(icon_path)) if icon_path else None,
+                            arg=arg,
+                        ).to_dict()
+                    ]
+                }
+            )
+        )
+        exit(0)
```

### Comparing `alfred5-1.1.2/alfred5/icons/download.png` & `alfred5-1.1.3/alfred5/icons/download.png`

 * *Files identical despite different names*

### Comparing `alfred5-1.1.2/alfred5/icons/error.png` & `alfred5-1.1.3/alfred5/icons/error.png`

 * *Files identical despite different names*

### Comparing `alfred5-1.1.2/alfred5/models.py` & `alfred5-1.1.3/alfred5/models.py`

 * *Files identical despite different names*

### Comparing `alfred5-1.1.2/alfred5.egg-info/PKG-INFO` & `alfred5-1.1.3/alfred5.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alfred5
-Version: 1.1.2
+Version: 1.1.3
 Summary: Simple python wrapper for alfred5 workflow / snippets
 Home-page: https://github.com/yedhrab/alfred5
 Author: Yunus Emre Ak
 Author-email: yemreak.com@gmail.com
 License: Apache Software License 2.0
 Project-URL: Source, https://github.com/yedhrab/alfred5/
 Project-URL: Changelog, https://github.com/yedhrab/alfred5/releases
@@ -23,37 +23,44 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 #  🎩 AlfredClient
 
 Simplest Alfred Client that I use my own projects.
 
+## Usage
+
 ```bash
 pip install alfred5
 ```
-
+- Projects dir structure
+    - Put your codes and `requirements.txt` to `src` folders
+    - Install `alfred5` via 
+        ```bash
+        pip install alfred5 --target=src/lib
+        ```
+    - If u want to use different `--target` for ex `.` use `WorkflowClient.run(packagedir=".")`
+    - Sample of default structure: 
+        - ![structure](https://i.imgur.com/doLWDR4.png)
+    - **If u install all of requirements, dont need to create `requirements.txt` file in `src`**
 - Via `SnippetsClient` API create custom snippets programmaically
 - Via `WorkflowClient` API create custom alfred workflow
     - Craete `requirements.txt` file for your python project to let `alfred5` installs them if needed 🙃
     - To install `from requirements.txt` do all import packages inside `main`
             - Use `global` keyword to access imported packages globally
         - `client.query` is the query string
         - `client.page_count` is the page count for pagination results
     - Dont need to add `alfred5` to `requirements.txt`
 - Use `WorkflowClient.log` to log your message to alfred debugger 
     - [debugging alfred workflow](https://www.alfredapp.com/help/workflows/utilities/debug/)
     - [why this project use stderr for all logging operation](https://www.alfredforum.com/topic/14721-get-the-python-output-back-to-alfred/?do=findComment&comment=75303)
-- Use `client.load_cached_response` and `client.cache_response` method to use caching system
-    - Just do it for static response (not timebased response)
+- Use `WorkflowClient(main, cache=True)` method to use caching system
+    - Just do it for static (not timebased nor any dynamic stuff) response 
     - Db path is `db/results.yml` also you can see it from workflow debug panel
 
-## Example Db Format
-
-![example-db](https://i.imgur.com/r2whZsi.png)
-
 ## ⭐️ Example Project
 
 ![alt](https://i.imgur.com/tUJjVUJ.png)
 
 ```python
 from re import sub
 from urllib.parse import quote_plus
@@ -65,15 +72,15 @@
     # To auto install requirements all import operation must be in here
     global get
     from requests import get
 
     query = client.query
     client.log(f"my query: {query}")  # use it to see your log in workflow debug panel
 
-    # (use cache=True) Use cache system to quick response
+    # (use cache=True) Use cache system to quick response instead of old style that below
     # if client.load_cached_response():
     #     return
 
     char_count = str(len( query))
     word_count = str(len(query.split(" ")))
     line_count = str(len(query.split("\n")))
 
@@ -91,19 +98,20 @@
     client.add_result(lower_case, "Lower Case", arg=lower_case)
     client.add_result(capitalized, "Capitalized", arg=capitalized)
     client.add_result(template, "Template", arg=template)
     client.add_result(char_count, "Characters", arg=char_count)
     client.add_result(word_count, "Words", arg=word_count)
     client.add_result(line_count, "Lines", arg=line_count)
     
-    # (use cache=True) to cache result for query (if u work with static results (not dynamic; coin price etc.))
+    # (use cache=True) to cache result for query instead of old style that below
+    #     if u work with static results (not dynamic; coin price etc.)
     # client.cache_response()  
 
 if __name__ == "__main__":
-    WorkflowClient.run(main)
+    WorkflowClient.run(main)  # WorkflowClient.run(main, cache=True)
 
 ```
 
 
 ## 🔰 How to Create Workflow
 
 ![insturaction1](https://i.imgur.com/2oDMChr.png)
```

### Comparing `alfred5-1.1.2/docs/README.md` & `alfred5-1.1.3/docs/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 #  🎩 AlfredClient
 
 Simplest Alfred Client that I use my own projects.
 
+## Usage
+
 ```bash
 pip install alfred5
 ```
-
+- Projects dir structure
+    - Put your codes and `requirements.txt` to `src` folders
+    - Install `alfred5` via 
+        ```bash
+        pip install alfred5 --target=src/lib
+        ```
+    - If u want to use different `--target` for ex `.` use `WorkflowClient.run(packagedir=".")`
+    - Sample of default structure: 
+        - ![structure](https://i.imgur.com/doLWDR4.png)
+    - **If u install all of requirements, dont need to create `requirements.txt` file in `src`**
 - Via `SnippetsClient` API create custom snippets programmaically
 - Via `WorkflowClient` API create custom alfred workflow
     - Craete `requirements.txt` file for your python project to let `alfred5` installs them if needed 🙃
     - To install `from requirements.txt` do all import packages inside `main`
             - Use `global` keyword to access imported packages globally
         - `client.query` is the query string
         - `client.page_count` is the page count for pagination results
     - Dont need to add `alfred5` to `requirements.txt`
 - Use `WorkflowClient.log` to log your message to alfred debugger 
     - [debugging alfred workflow](https://www.alfredapp.com/help/workflows/utilities/debug/)
     - [why this project use stderr for all logging operation](https://www.alfredforum.com/topic/14721-get-the-python-output-back-to-alfred/?do=findComment&comment=75303)
-- Use `client.load_cached_response` and `client.cache_response` method to use caching system
-    - Just do it for static response (not timebased response)
+- Use `WorkflowClient(main, cache=True)` method to use caching system
+    - Just do it for static (not timebased nor any dynamic stuff) response 
     - Db path is `db/results.yml` also you can see it from workflow debug panel
 
-## Example Db Format
-
-![example-db](https://i.imgur.com/r2whZsi.png)
-
 ## ⭐️ Example Project
 
 ![alt](https://i.imgur.com/tUJjVUJ.png)
 
 ```python
 from re import sub
 from urllib.parse import quote_plus
@@ -40,15 +47,15 @@
     # To auto install requirements all import operation must be in here
     global get
     from requests import get
 
     query = client.query
     client.log(f"my query: {query}")  # use it to see your log in workflow debug panel
 
-    # (use cache=True) Use cache system to quick response
+    # (use cache=True) Use cache system to quick response instead of old style that below
     # if client.load_cached_response():
     #     return
 
     char_count = str(len( query))
     word_count = str(len(query.split(" ")))
     line_count = str(len(query.split("\n")))
 
@@ -66,19 +73,20 @@
     client.add_result(lower_case, "Lower Case", arg=lower_case)
     client.add_result(capitalized, "Capitalized", arg=capitalized)
     client.add_result(template, "Template", arg=template)
     client.add_result(char_count, "Characters", arg=char_count)
     client.add_result(word_count, "Words", arg=word_count)
     client.add_result(line_count, "Lines", arg=line_count)
     
-    # (use cache=True) to cache result for query (if u work with static results (not dynamic; coin price etc.))
+    # (use cache=True) to cache result for query instead of old style that below
+    #     if u work with static results (not dynamic; coin price etc.)
     # client.cache_response()  
 
 if __name__ == "__main__":
-    WorkflowClient.run(main)
+    WorkflowClient.run(main)  # WorkflowClient.run(main, cache=True)
 
 ```
 
 
 ## 🔰 How to Create Workflow
 
 ![insturaction1](https://i.imgur.com/2oDMChr.png)
```

### Comparing `alfred5-1.1.2/setup.py` & `alfred5-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 """
 
 from glob import glob
 from os.path import basename, splitext
 from setuptools import find_packages, setup
 from pathlib import Path
 
-VERSION = "1.1.2"
+VERSION = "1.1.3"
 DESCRIPTION = "Simple python wrapper for alfred5 workflow / snippets"
 README_PATH = "docs/README.md"
 USERNAME = "yedhrab"
 REPOSITORY = "alfred5"
 KEYWORDS = [
     "alfred",
     "alfred5",
```

