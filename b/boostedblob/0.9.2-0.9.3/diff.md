# Comparing `tmp/boostedblob-0.9.2.tar.gz` & `tmp/boostedblob-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boostedblob-0.9.2.tar", max compression
+gzip compressed data, was "boostedblob-0.9.3.tar", max compression
```

## Comparing `boostedblob-0.9.2.tar` & `boostedblob-0.9.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1135 2021-06-18 22:09:53.198667 boostedblob-0.9.2/README.md
--rw-r--r--   0        0        0      944 2021-11-20 23:14:15.497985 boostedblob-0.9.2/boostedblob/__init__.py
--rw-r--r--   0        0        0      294 2020-12-15 07:17:41.898951 boostedblob-0.9.2/boostedblob/__main__.py
--rw-r--r--   0        0        0    22555 2021-11-20 23:13:28.698571 boostedblob-0.9.2/boostedblob/azure_auth.py
--rw-r--r--   0        0        0    22739 2021-06-18 22:09:53.201458 boostedblob-0.9.2/boostedblob/boost.py
--rw-r--r--   0        0        0    24856 2021-11-10 23:00:19.040036 boostedblob-0.9.2/boostedblob/cli.py
--rw-r--r--   0        0        0    11806 2021-09-30 06:03:37.907762 boostedblob-0.9.2/boostedblob/copying.py
--rw-r--r--   0        0        0     6508 2021-07-03 18:07:53.512664 boostedblob-0.9.2/boostedblob/delete.py
--rw-r--r--   0        0        0     7895 2021-11-10 23:00:23.129227 boostedblob-0.9.2/boostedblob/globals.py
--rw-r--r--   0        0        0     9264 2021-09-30 06:26:18.180409 boostedblob-0.9.2/boostedblob/google_auth.py
--rw-r--r--   0        0        0    16682 2021-10-04 06:21:39.144550 boostedblob-0.9.2/boostedblob/listing.py
--rw-r--r--   0        0        0    16950 2021-11-10 23:00:19.041480 boostedblob-0.9.2/boostedblob/path.py
--rw-r--r--   0        0        0        0 2020-10-23 00:10:03.878441 boostedblob-0.9.2/boostedblob/py.typed
--rw-r--r--   0        0        0     6288 2021-09-20 20:13:33.462345 boostedblob-0.9.2/boostedblob/read.py
--rw-r--r--   0        0        0    13545 2021-11-18 00:05:29.633404 boostedblob-0.9.2/boostedblob/request.py
--rw-r--r--   0        0        0      817 2020-11-15 21:19:45.754216 boostedblob-0.9.2/boostedblob/share.py
--rw-r--r--   0        0        0     6668 2021-09-30 06:04:41.863546 boostedblob-0.9.2/boostedblob/syncing.py
--rw-r--r--   0        0        0    16304 2021-09-30 06:40:00.432641 boostedblob-0.9.2/boostedblob/write.py
--rw-r--r--   0        0        0     1322 2021-11-20 23:14:20.723960 boostedblob-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     2097 2021-11-20 23:14:52.729445 boostedblob-0.9.2/setup.py
--rw-r--r--   0        0        0     1946 2021-11-20 23:14:52.729775 boostedblob-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1135 2021-06-18 22:09:53.198667 boostedblob-0.9.3/README.md
+-rw-r--r--   0        0        0      944 2022-01-19 20:25:08.674757 boostedblob-0.9.3/boostedblob/__init__.py
+-rw-r--r--   0        0        0      294 2020-12-15 07:17:41.898951 boostedblob-0.9.3/boostedblob/__main__.py
+-rw-r--r--   0        0        0    22555 2021-11-20 23:13:28.698571 boostedblob-0.9.3/boostedblob/azure_auth.py
+-rw-r--r--   0        0        0    22739 2021-06-18 22:09:53.201458 boostedblob-0.9.3/boostedblob/boost.py
+-rw-r--r--   0        0        0    24856 2021-12-15 19:55:42.245793 boostedblob-0.9.3/boostedblob/cli.py
+-rw-r--r--   0        0        0    11806 2021-09-30 06:03:37.907762 boostedblob-0.9.3/boostedblob/copying.py
+-rw-r--r--   0        0        0     6508 2021-07-03 18:07:53.512664 boostedblob-0.9.3/boostedblob/delete.py
+-rw-r--r--   0        0        0     7895 2021-11-10 23:00:23.129227 boostedblob-0.9.3/boostedblob/globals.py
+-rw-r--r--   0        0        0     9264 2021-09-30 06:26:18.180409 boostedblob-0.9.3/boostedblob/google_auth.py
+-rw-r--r--   0        0        0    16926 2022-01-19 20:15:42.207248 boostedblob-0.9.3/boostedblob/listing.py
+-rw-r--r--   0        0        0    17126 2022-01-19 20:34:01.794609 boostedblob-0.9.3/boostedblob/path.py
+-rw-r--r--   0        0        0        0 2020-10-23 00:10:03.878441 boostedblob-0.9.3/boostedblob/py.typed
+-rw-r--r--   0        0        0     6288 2021-09-20 20:13:33.462345 boostedblob-0.9.3/boostedblob/read.py
+-rw-r--r--   0        0        0    13667 2022-01-19 20:18:29.563851 boostedblob-0.9.3/boostedblob/request.py
+-rw-r--r--   0        0        0      817 2020-11-15 21:19:45.754216 boostedblob-0.9.3/boostedblob/share.py
+-rw-r--r--   0        0        0     6668 2021-09-30 06:04:41.863546 boostedblob-0.9.3/boostedblob/syncing.py
+-rw-r--r--   0        0        0    16304 2021-09-30 06:40:00.432641 boostedblob-0.9.3/boostedblob/write.py
+-rw-r--r--   0        0        0     1322 2022-01-19 20:25:00.013539 boostedblob-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     2097 2022-01-19 20:41:07.773594 boostedblob-0.9.3/setup.py
+-rw-r--r--   0        0        0     1946 2022-01-19 20:41:07.774196 boostedblob-0.9.3/PKG-INFO
```

### Comparing `boostedblob-0.9.2/README.md` & `boostedblob-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `boostedblob-0.9.2/boostedblob/__init__.py` & `boostedblob-0.9.3/boostedblob/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.9.2"
+__version__ = "0.9.3"
 
 from . import read as read
 from . import share as share
 from . import write as write
 from .boost import BoostExecutor as BoostExecutor
 from .copying import copyfile as copyfile
 from .copying import copytree as copytree
```

### Comparing `boostedblob-0.9.2/boostedblob/azure_auth.py` & `boostedblob-0.9.3/boostedblob/azure_auth.py`

 * *Files identical despite different names*

### Comparing `boostedblob-0.9.2/boostedblob/boost.py` & `boostedblob-0.9.3/boostedblob/boost.py`

 * *Files identical despite different names*

### Comparing `boostedblob-0.9.2/boostedblob/cli.py` & `boostedblob-0.9.3/boostedblob/cli.py`

 * *Files identical despite different names*

### Comparing `boostedblob-0.9.2/boostedblob/copying.py` & `boostedblob-0.9.3/boostedblob/copying.py`

 * *Files identical despite different names*

### Comparing `boostedblob-0.9.2/boostedblob/delete.py` & `boostedblob-0.9.3/boostedblob/delete.py`

 * *Files identical despite different names*

### Comparing `boostedblob-0.9.2/boostedblob/globals.py` & `boostedblob-0.9.3/boostedblob/globals.py`

 * *Files identical despite different names*

### Comparing `boostedblob-0.9.2/boostedblob/google_auth.py` & `boostedblob-0.9.3/boostedblob/google_auth.py`

 * *Files identical despite different names*

### Comparing `boostedblob-0.9.2/boostedblob/listing.py` & `boostedblob-0.9.3/boostedblob/listing.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,14 +159,18 @@
         if entry.path == dirpath:
             continue
         yield entry
 
     # If we find nothing, then run some checks so we throw the appropriate error.
     # Doing this means we avoid extra requests in the happy path.
     if not subpath_exists:
+        if isinstance(path, AzurePath) and not path.blob:
+            # Special case empty containers (at this point we're guaranteed the container exists)
+            # TODO: double check this when anonymous containers work
+            return
         if not await isfile(path):
             raise FileNotFoundError(path)
         raise NotADirectoryError(path)
 
 
 @scandir.register  # type: ignore
 async def _local_scandir(path: LocalPath) -> AsyncIterator[DirEntry]:
```

### Comparing `boostedblob-0.9.2/boostedblob/path.py` & `boostedblob-0.9.3/boostedblob/path.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,25 +122,25 @@
 
     @staticmethod
     def from_str(url: str) -> AzurePath:
         parsed_url = urllib.parse.urlparse(url)
         if parsed_url.scheme == "https":
             account, host = parsed_url.netloc.split(".", maxsplit=1)
             if host != "blob.core.windows.net":
-                raise ValueError(f"Invalid URL '{url}'")
+                raise ValueError(f"Invalid URL '{url}'; unexpected host '{host}'")
         elif parsed_url.scheme == "az":
             account = parsed_url.netloc
         else:
-            raise ValueError(f"Invalid URL '{url}'")
+            raise ValueError(f"Invalid URL '{url}'; expected 'https' or 'az' scheme")
 
-        parts = parsed_url.path.split("/", maxsplit=2)
-        if parts[0]:
-            raise ValueError(f"Invalid URL '{url}'")
-        container = parts[1] if len(parts) >= 2 else ""
-        return AzurePath(account=account, container=container, blob="/".join(parts[2:]))
+        # split the unparsed URL
+        parts = url.split("/", maxsplit=4)
+        container = parts[3] if len(parts) >= 4 else ""
+        blob = parts[4] if len(parts) >= 5 else ""
+        return AzurePath(account=account, container=container, blob=blob)
 
     @property
     def name(self) -> str:
         return os.path.basename(_strip_slash(self.blob)) if self.blob else self.container
 
     @property
     def parent(self) -> AzurePath:
@@ -189,17 +189,20 @@
     bucket: str
     blob: str
 
     @staticmethod
     def from_str(url: str) -> GooglePath:
         parsed_url = urllib.parse.urlparse(url)
         if parsed_url.scheme != "gs":
-            raise ValueError(f"Invalid URL '{url}'")
+            raise ValueError(f"Invalid URL '{url}'; expected 'gs' scheme")
 
-        return GooglePath(bucket=parsed_url.netloc, blob=parsed_url.path[1:])
+        # split the unparsed URL
+        parts = url.split("/", maxsplit=3)
+        blob = parts[3] if len(parts) >= 4 else ""
+        return GooglePath(bucket=parsed_url.netloc, blob=blob)
 
     @property
     def name(self) -> str:
         return os.path.basename(_strip_slash(self.blob)) if self.blob else self.bucket
 
     @property
     def parent(self) -> GooglePath:
```

### Comparing `boostedblob-0.9.2/boostedblob/read.py` & `boostedblob-0.9.3/boostedblob/read.py`

 * *Files identical despite different names*

### Comparing `boostedblob-0.9.2/boostedblob/request.py` & `boostedblob-0.9.3/boostedblob/request.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,28 +69,30 @@
                     error = RequestFailure(reason=type(e).__name__ + ": " + str(e), request=self)
                 else:
                     if resp.status in self.success_codes:
                         yield resp
                         return
 
                     assert resp.reason is not None
-                    reason = str(resp.reason)
+                    reason = repr(resp.reason)
                     if config.debug_mode:
-                        reason += ", Body: " + (await resp.text())
+                        reason += (
+                            "\nBody:\n" + (await resp.text()) + "\nHeaders:\n" + str(resp.headers)
+                        )
                     error = RequestFailure(reason=reason, request=self, status=resp.status)
                     if resp.status not in self.retry_codes:
                         raise self.failure_exceptions.get(resp.status, error)
 
             if attempt >= config.retry_limit:
                 raise error
 
             if config.debug_mode or attempt + 1 >= 3:
                 print(
                     f"[boostedblob] Error when executing request on attempt {attempt + 1}, "
-                    f"sleeping for {backoff:.1f}s before retrying. Details: {error}",
+                    f"sleeping for {backoff:.1f}s before retrying. Details:\n{error}",
                     file=sys.stderr,
                 )
             await asyncio.sleep(backoff)
 
     async def execute_reponseless(self) -> None:
         """Helper to execute the request when we don't have further need of the response."""
         async with self.execute():
@@ -133,15 +135,15 @@
 class RequestFailure(Exception):
     def __init__(self, reason: str, request: Request, status: Optional[int] = None):
         self.reason = reason
         self.request = request
         self.status = status
 
     def __str__(self) -> str:
-        return f"{self.reason}, {self.status}, {self.request}"
+        return f"Reason: {self.reason}\nRequest: {self.request}\nStatus: {self.status}"
 
 
 async def execute_retrying_read(request: Request) -> bytes:
     # Retrying aiohttp.ServerTimeoutError is pretty straightforward
     # ClientPayloadError might be an aiohttp bug, see:
     # https://github.com/aio-libs/aiohttp/issues/4581
     # https://github.com/aio-libs/aiohttp/issues/3904#issuecomment-737094416
@@ -158,15 +160,15 @@
         except (aiohttp.ServerTimeoutError, aiohttp.ClientPayloadError) as error:
             if attempt >= config.retry_limit:
                 raise
 
             if config.debug_mode or attempt + 1 >= 3:
                 print(
                     f"[boostedblob] Error when executing request on attempt {attempt + 1}, "
-                    f"sleeping for {backoff:.1f}s before retrying. Details: {error}",
+                    f"sleeping for {backoff:.1f}s before retrying. Details:\n{error}",
                     file=sys.stderr,
                 )
             await asyncio.sleep(backoff)
     raise AssertionError
 
 
 # ==============================
```

### Comparing `boostedblob-0.9.2/boostedblob/share.py` & `boostedblob-0.9.3/boostedblob/share.py`

 * *Files identical despite different names*

### Comparing `boostedblob-0.9.2/boostedblob/syncing.py` & `boostedblob-0.9.3/boostedblob/syncing.py`

 * *Files identical despite different names*

### Comparing `boostedblob-0.9.2/boostedblob/write.py` & `boostedblob-0.9.3/boostedblob/write.py`

 * *Files identical despite different names*

### Comparing `boostedblob-0.9.2/pyproject.toml` & `boostedblob-0.9.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 [tool.isort]
 profile = "black"
 line_length = 100
 skip_gitignore = true
 
 [tool.poetry]
 name = "boostedblob"
-version = "0.9.2"
+version = "0.9.3"
 description = """
 Command line tool and async library to perform basic file operations on local \
 paths, Google Cloud Storage paths and Azure Blob Storage paths.\
 """
 authors = ["Shantanu Jain <hauntsaninja@gmail.com>"]
 license = "MIT"
 readme = "README.md"
@@ -46,15 +46,15 @@
 # poetry fails to resolve blobfile's dependencies
 urllib3 = "*"
 filelock = "*"
 # tools
 ipdb = "*"
 black = "^21.9b0"
 isort = "^5.7.0"
-mypy = "^0.910"
+mypy = "^0.931"
 flake8 = "^3.8.3"
 
 [tool.poetry.scripts]
 bbb = 'boostedblob.__main__:main'
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `boostedblob-0.9.2/setup.py` & `boostedblob-0.9.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'xmltodict>=0.12,<0.13']
 
 entry_points = \
 {'console_scripts': ['bbb = boostedblob.__main__:main']}
 
 setup_kwargs = {
     'name': 'boostedblob',
-    'version': '0.9.2',
+    'version': '0.9.3',
     'description': 'Command line tool and async library to perform basic file operations on local paths, Google Cloud Storage paths and Azure Blob Storage paths.',
     'long_description': '# boostedblob\n\nboostedblob is a command line tool and async library to perform basic file operations on local\npaths, Google Cloud Storage paths and Azure Blob Storage paths.\n\nboostedblob is derived from the excellent [blobfile](https://github.com/christopher-hesse/blobfile).\n\nThe fun part of implementing boostedblob is `boostedblob/boost.py`, which provides a\n`concurrent.futures`-like interface for running and composing async tasks in a concurrency limited\nenvironment.\n\n## Installation\n\nJust run `pip install boostedblob`. boostedblob requires Python 3.7 or better.\n\n## Usage\n\nFor an overview and list of commands:\n```sh\nbbb --help\n```\n\nFor help with a specific command:\n```sh\nbbb ls --help\n```\n\nTo enable tab completion, add the following to your shell config (replacing `zsh` with `bash`, if appropriate):\n```sh\neval "$(bbb complete init zsh)"\n```\nNote that the quotes are necessary. You can also inline the result of `bbb complete init zsh` into\nyour shell config to make your shell startup a little faster.\n\n## Contributing\n\nTo get started with developing boostedblob and running tests, see [CONTRIBUTING.md](CONTRIBUTING.md)\n',
     'author': 'Shantanu Jain',
     'author_email': 'hauntsaninja@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `boostedblob-0.9.2/PKG-INFO` & `boostedblob-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boostedblob
-Version: 0.9.2
+Version: 0.9.3
 Summary: Command line tool and async library to perform basic file operations on local paths, Google Cloud Storage paths and Azure Blob Storage paths.
 License: MIT
 Author: Shantanu Jain
 Author-email: hauntsaninja@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

