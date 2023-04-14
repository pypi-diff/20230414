# Comparing `tmp/geovisio_cli-0.0.3.tar.gz` & `tmp/geovisio_cli-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geovisio_cli-0.0.3.tar", last modified: Wed Apr 12 20:09:04 2023, max compression
+gzip compressed data, was "geovisio_cli-0.0.4.tar", last modified: Fri Apr 14 11:24:02 2023, max compression
```

## Comparing `geovisio_cli-0.0.3.tar` & `geovisio_cli-0.0.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0       47 2023-03-24 13:15:13.689899 geovisio_cli-0.0.3/.gitignore
--rw-r--r--   0        0        0     1732 2023-03-24 13:15:13.689899 geovisio_cli-0.0.3/.gitlab-ci.yml
--rw-r--r--   0        0        0     1048 2023-04-12 20:00:20.693628 geovisio_cli-0.0.3/CHANGELOG.md
--rw-r--r--   0        0        0     5468 2023-03-24 13:15:13.689899 geovisio_cli-0.0.3/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1070 2023-03-14 15:26:20.137987 geovisio_cli-0.0.3/LICENSE
--rw-r--r--   0        0        0      551 2023-03-14 15:26:20.137987 geovisio_cli-0.0.3/Makefile
--rw-r--r--   0        0        0     4639 2023-04-07 07:41:38.712978 geovisio_cli-0.0.3/README.md
--rw-r--r--   0        0        0     2290 2023-04-11 15:14:50.737428 geovisio_cli-0.0.3/USAGE.md
--rw-r--r--   0        0        0       53 2023-04-12 20:00:20.693628 geovisio_cli-0.0.3/geovisio_cli/__init__.py
--rw-r--r--   0        0        0     1572 2023-03-14 16:32:00.535627 geovisio_cli-0.0.3/geovisio_cli/auth.py
--rw-r--r--   0        0        0       90 2023-03-14 15:26:20.137987 geovisio_cli-0.0.3/geovisio_cli/exception.py
--rw-r--r--   0        0        0     3617 2023-04-11 15:19:40.311478 geovisio_cli-0.0.3/geovisio_cli/main.py
--rw-r--r--   0        0        0      173 2023-03-14 15:26:20.137987 geovisio_cli-0.0.3/geovisio_cli/model.py
--rw-r--r--   0        0        0    13024 2023-04-11 15:19:40.311478 geovisio_cli-0.0.3/geovisio_cli/sequence.py
--rw-r--r--   0        0        0      896 2023-03-14 16:32:00.535627 geovisio_cli-0.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-14 15:26:20.137987 geovisio_cli-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0      191 2023-03-14 15:26:20.137987 geovisio_cli-0.0.3/tests/conftest.py
--rw-r--r--   0        0        0   523332 2023-03-14 15:26:20.137987 geovisio_cli-0.0.3/tests/fixtures/e1.jpg
--rw-r--r--   0        0        0   483454 2023-03-14 15:26:20.141986 geovisio_cli-0.0.3/tests/fixtures/e2.jpg
--rw-r--r--   0        0        0   529344 2023-03-14 15:26:20.141986 geovisio_cli-0.0.3/tests/fixtures/e3.jpg
--rw-r--r--   0        0        0       16 2023-03-14 15:26:20.141986 geovisio_cli-0.0.3/tests/fixtures/invalid_pic.jpg
--rw-r--r--   0        0        0       27 2023-03-14 15:26:20.141986 geovisio_cli-0.0.3/tests/fixtures/not_a_pic.md
--rw-r--r--   0        0        0        0 2023-03-14 15:26:20.141986 geovisio_cli-0.0.3/tests/integration/__init__.py
--rw-r--r--   0        0        0      865 2023-03-14 15:26:20.141986 geovisio_cli-0.0.3/tests/integration/conftest.py
--rw-r--r--   0        0        0      671 2023-03-14 16:32:00.535627 geovisio_cli-0.0.3/tests/integration/docker-compose-geovisio.yml
--rw-r--r--   0        0        0      319 2023-04-07 07:41:38.712978 geovisio_cli-0.0.3/tests/integration/test_status.py
--rw-r--r--   0        0        0     3042 2023-04-07 07:41:38.712978 geovisio_cli-0.0.3/tests/integration/test_upload.py
--rw-r--r--   0        0        0      528 2023-03-24 13:15:13.689899 geovisio_cli-0.0.3/tests/test_process.py
--rw-r--r--   0        0        0      813 2023-03-24 13:15:13.689899 geovisio_cli-0.0.3/tests/test_sequence.py
--rw-r--r--   0        0        0     5498 1970-01-01 00:00:00.000000 geovisio_cli-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       47 2023-03-24 13:15:13.689899 geovisio_cli-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1732 2023-03-24 13:15:13.689899 geovisio_cli-0.0.4/.gitlab-ci.yml
+-rw-r--r--   0        0        0     1527 2023-04-14 11:18:33.201654 geovisio_cli-0.0.4/CHANGELOG.md
+-rw-r--r--   0        0        0     5468 2023-03-24 13:15:13.689899 geovisio_cli-0.0.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1070 2023-03-14 15:26:20.137987 geovisio_cli-0.0.4/LICENSE
+-rw-r--r--   0        0        0      551 2023-03-14 15:26:20.137987 geovisio_cli-0.0.4/Makefile
+-rw-r--r--   0        0        0     4632 2023-04-14 07:21:46.587626 geovisio_cli-0.0.4/README.md
+-rw-r--r--   0        0        0     2320 2023-04-14 07:21:46.587626 geovisio_cli-0.0.4/USAGE.md
+-rw-r--r--   0        0        0       53 2023-04-14 11:18:33.205654 geovisio_cli-0.0.4/geovisio_cli/__init__.py
+-rw-r--r--   0        0        0     1972 2023-04-14 11:12:54.559203 geovisio_cli-0.0.4/geovisio_cli/auth.py
+-rw-r--r--   0        0        0      284 2023-04-14 11:12:54.559203 geovisio_cli-0.0.4/geovisio_cli/exception.py
+-rw-r--r--   0        0        0     3621 2023-04-14 07:21:46.587626 geovisio_cli-0.0.4/geovisio_cli/main.py
+-rw-r--r--   0        0        0      173 2023-03-14 15:26:20.137987 geovisio_cli-0.0.4/geovisio_cli/model.py
+-rw-r--r--   0        0        0    13940 2023-04-14 11:12:54.559203 geovisio_cli-0.0.4/geovisio_cli/sequence.py
+-rw-r--r--   0        0        0      896 2023-03-14 16:32:00.535627 geovisio_cli-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-14 15:26:20.137987 geovisio_cli-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0      191 2023-03-14 15:26:20.137987 geovisio_cli-0.0.4/tests/conftest.py
+-rw-r--r--   0        0        0   523332 2023-03-14 15:26:20.137987 geovisio_cli-0.0.4/tests/fixtures/e1.jpg
+-rw-r--r--   0        0        0   483454 2023-03-14 15:26:20.141986 geovisio_cli-0.0.4/tests/fixtures/e2.jpg
+-rw-r--r--   0        0        0   529344 2023-03-14 15:26:20.141986 geovisio_cli-0.0.4/tests/fixtures/e3.jpg
+-rw-r--r--   0        0        0       16 2023-03-14 15:26:20.141986 geovisio_cli-0.0.4/tests/fixtures/invalid_pic.jpg
+-rw-r--r--   0        0        0       27 2023-03-14 15:26:20.141986 geovisio_cli-0.0.4/tests/fixtures/not_a_pic.md
+-rw-r--r--   0        0        0        0 2023-03-14 15:26:20.141986 geovisio_cli-0.0.4/tests/integration/__init__.py
+-rw-r--r--   0        0        0      865 2023-03-14 15:26:20.141986 geovisio_cli-0.0.4/tests/integration/conftest.py
+-rw-r--r--   0        0        0      671 2023-03-14 16:32:00.535627 geovisio_cli-0.0.4/tests/integration/docker-compose-geovisio.yml
+-rw-r--r--   0        0        0      319 2023-04-07 07:41:38.712978 geovisio_cli-0.0.4/tests/integration/test_status.py
+-rw-r--r--   0        0        0     4914 2023-04-14 11:12:54.559203 geovisio_cli-0.0.4/tests/integration/test_upload.py
+-rw-r--r--   0        0        0      528 2023-03-24 13:15:13.689899 geovisio_cli-0.0.4/tests/test_process.py
+-rw-r--r--   0        0        0      813 2023-03-24 13:15:13.689899 geovisio_cli-0.0.4/tests/test_sequence.py
+-rw-r--r--   0        0        0     5491 1970-01-01 00:00:00.000000 geovisio_cli-0.0.4/PKG-INFO
```

### Comparing `geovisio_cli-0.0.3/.gitlab-ci.yml` & `geovisio_cli-0.0.4/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.0.3/CODE_OF_CONDUCT.md` & `geovisio_cli-0.0.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.0.3/LICENSE` & `geovisio_cli-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.0.3/Makefile` & `geovisio_cli-0.0.4/Makefile`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.0.3/README.md` & `geovisio_cli-0.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 ```bash
 geovisio upload --help
 ```
 
 If you want to upload pictures from a `my_sequence` directory to a GeoVisio instance (running locally in this example), launch this command:
 
 ```bash
-geovisio upload --path ./my_sequence --api-url http://localhost:5000/
+geovisio upload --api-url http://localhost:5000/ ./my_sequence
 ```
 
 You can also add a `--wait` flag to wait for geovisio to process all the pictures.
 
 #### Authentication
 
 If the GeoVisio API requires a login for the upload, the user/password can either be set:
```

### Comparing `geovisio_cli-0.0.3/USAGE.md` & `geovisio_cli-0.0.4/USAGE.md`

 * *Files 8% similar despite different names*

```diff
@@ -44,35 +44,41 @@
 ## `geovisio test-process`
 
 (For testing) Generates a JSON file with metadata used for upload
 
 **Usage**:
 
 ```console
-$ geovisio test-process [OPTIONS]
+$ geovisio test-process [OPTIONS] PATH
 ```
 
+**Arguments**:
+
+* `PATH`: Local path to your sequence folder  [required]
+
 **Options**:
 
-* `--path PATH`: Local path to your sequence folder  [required]
 * `--help`: Show this message and exit.
 
 ## `geovisio upload`
 
 Processes and sends a given sequence on your GeoVisio API
 
 **Usage**:
 
 ```console
-$ geovisio upload [OPTIONS]
+$ geovisio upload [OPTIONS] PATH
 ```
 
+**Arguments**:
+
+* `PATH`: Local path to your sequence folder  [required]
+
 **Options**:
 
-* `--path PATH`: Local path to your sequence folder  [required]
 * `--api-url TEXT`: GeoVisio endpoint URL  [required]
 * `--user TEXT`: GeoVisio user name if the geovisio instance needs it.
 If none is provided and the geovisio instance requires it, the username will be asked during run.  [env var: GEOVISIO_USER]
 * `--password TEXT`: GeoVisio password if the geovisio instance needs it.
 If none is provided and the geovisio instance requires it, the password will be asked during run.
 Note: is is advised to wait for prompt without using this variable.  [env var: GEOVISIO_PASSWORD]
 * `--wait / --no-wait`: Wait for all pictures to be ready  [default: no-wait]
```

### Comparing `geovisio_cli-0.0.3/geovisio_cli/auth.py` & `geovisio_cli-0.0.4/geovisio_cli/auth.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from requests import Session
 from geovisio_cli.model import Geovisio
-from geovisio_cli.exception import CliException
+from geovisio_cli.exception import CliException, raise_for_status
 import getpass
 from rich.prompt import Prompt
 
 
 def _get_keycloak_authenticate_form_url(response):
     """Little hack to parse keycloak HTML to get the url to the authenticate form"""
     import re
@@ -43,8 +43,15 @@
 
     r = s.post(
         url,
         data={"username": username, "password": password},
         headers={"Content-Type": "application/x-www-form-urlencoded"},
         allow_redirects=True,
     )
-    r.raise_for_status()
+
+    # a bit hacky, but since for the moment we only submit a form to keycloak, to know if the login was successful,
+    # we need to check that we were redirected to geovisio
+    raise_for_status(r, "Impossible to log in geovisio")
+    if len(r.history) == 0:
+        raise CliException(
+            "The username or password is invalid, make sure you have correct credentials and please retry."
+        )
```

### Comparing `geovisio_cli-0.0.3/geovisio_cli/main.py` & `geovisio_cli-0.0.4/geovisio_cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 app = typer.Typer(help="GeoVisio command-line client")
 
 
 @app.command()
 def upload(
-    path: Path = typer.Option(..., help="Local path to your sequence folder"),
+    path: Path = typer.Argument(..., help="Local path to your sequence folder"),
     api_url: str = typer.Option(..., help="GeoVisio endpoint URL"),
     user: str = typer.Option(
         default=None,
         help="""GeoVisio user name if the geovisio instance needs it.
 If none is provided and the geovisio instance requires it, the username will be asked during run.
 """,
         envvar="GEOVISIO_USER",
@@ -49,15 +49,15 @@
             )
         )
         return 1
 
 
 @app.command()
 def test_process(
-    path: Path = typer.Option(..., help="Local path to your sequence folder"),
+    path: Path = typer.Argument(..., help="Local path to your sequence folder"),
 ):
     """(For testing) Generates a JSON file with metadata used for upload"""
 
     import json
     from dataclasses import asdict
 
     try:
```

### Comparing `geovisio_cli-0.0.3/geovisio_cli/sequence.py` & `geovisio_cli-0.0.4/geovisio_cli/sequence.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     TimeElapsedColumn,
     BarColumn,
     MofNCompleteColumn,
 )
 from rich.panel import Panel
 from rich.console import Group
 from rich.live import Live
-from geovisio_cli.exception import CliException
+from geovisio_cli.exception import CliException, raise_for_status
 from geovisio_cli.auth import login
 from geovisio_cli.model import Geovisio
 from time import sleep
 from datetime import timedelta
 
 
 @dataclass
@@ -123,15 +123,15 @@
         data["title"] = sequence.title
 
     with requests.session() as s:
         seq = s.post(f"{geovisio.url}/api/collections", data=data)
         if seq.status_code == 401:
             login(s, geovisio)
             seq = s.post(f"{geovisio.url}/api/collections", data=data)
-        seq.raise_for_status()
+        raise_for_status(seq, "Impossible to query geovisio")
 
         seq_location = seq.headers["Location"]
         print(f"✅ Created collection {seq_location}")
         report = UploadReport(location=seq_location)
 
         uploading_progress = Progress(
             TextColumn("{task.description}"),
@@ -276,17 +276,48 @@
 
 
 def _test_geovisio_url(geovisio: str):
     full_url = f"{geovisio}/api/collections"
     try:
         r = requests.get(full_url)
     except requests.ConnectionError as e:
-        raise CliException(f"Impossible to query geovisio base url:\n\t{e}")
-    if r.status_code >= 400:
-        raise CliException(f"Impossible to query geovisio: {r.status_code}:\n {r.text}")
+        raise CliException(
+            f"""The API is not reachable. Please check error and used URL below, and retry later if the URL is correct.
+
+[bold]Used URL:[/bold] {full_url}
+[bold]Error:[/bold]
+{e}"""
+        )
+    except Exception as e:
+        raise CliException(
+            f"""Error while connecting to the API. Please check error and used URL below
+
+[bold]Used URL:[/bold] {full_url}
+[bold]Error:[/bold]
+{e}"""
+        )
+
+    if r.status_code == 404:
+        raise CliException(
+            f"""The API URL is not valid.
+
+Note that your URL should be the API root (something like https://geovisio.fr, https://panoramax.ign.fr or any other geovisio instance).
+Please make sure you gave the correct URL and retry.
+
+[bold]Used URL:[/bold] {full_url}
+[bold]Error:[/bold]
+{r.text}"""
+        )
+    if r.status_code > 404:
+        raise CliException(
+            f"""The API is unavailable for now. Please check given error and retry later.
+[bold]Used URL:[/bold] {full_url}
+[bold]Error[/bold] (code [cyan]{r.status_code}[/cyan]):
+{r.text}"""
+        )
 
 
 def status(sequence_location: str) -> SequenceStatus:
     s = requests.get(f"{sequence_location}/geovisio_status")
     if s.status_code == 404:
         raise CliException(f"Sequence {sequence_location} not found")
     if s.status_code >= 400:
```

### Comparing `geovisio_cli-0.0.3/pyproject.toml` & `geovisio_cli-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.0.3/tests/fixtures/e1.jpg` & `geovisio_cli-0.0.4/tests/fixtures/e1.jpg`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.0.3/tests/fixtures/e2.jpg` & `geovisio_cli-0.0.4/tests/fixtures/e2.jpg`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.0.3/tests/fixtures/e3.jpg` & `geovisio_cli-0.0.4/tests/fixtures/e3.jpg`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.0.3/tests/integration/conftest.py` & `geovisio_cli-0.0.4/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.0.3/tests/integration/docker-compose-geovisio.yml` & `geovisio_cli-0.0.4/tests/integration/docker-compose-geovisio.yml`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.0.3/tests/test_process.py` & `geovisio_cli-0.0.4/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.0.3/tests/test_sequence.py` & `geovisio_cli-0.0.4/tests/test_sequence.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.0.3/PKG-INFO` & `geovisio_cli-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geovisio_cli
-Version: 0.0.3
+Version: 0.0.4
 Summary: Geovio client cli tool
 Author-email: Antoine Desbordes <antoine.desbordes@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: requests ~= 2.28.0
 Requires-Dist: typer ~= 0.7.0
 Requires-Dist: rich[all] ~= 13.3.0
@@ -115,15 +115,15 @@
 ```bash
 geovisio upload --help
 ```
 
 If you want to upload pictures from a `my_sequence` directory to a GeoVisio instance (running locally in this example), launch this command:
 
 ```bash
-geovisio upload --path ./my_sequence --api-url http://localhost:5000/
+geovisio upload --api-url http://localhost:5000/ ./my_sequence
 ```
 
 You can also add a `--wait` flag to wait for geovisio to process all the pictures.
 
 #### Authentication
 
 If the GeoVisio API requires a login for the upload, the user/password can either be set:
```

