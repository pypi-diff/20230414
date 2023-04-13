# Comparing `tmp/isic-cli-5.0.0.tar.gz` & `tmp/isic-cli-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isic-cli-5.0.0.tar", last modified: Fri Jan 20 17:36:09 2023, max compression
+gzip compressed data, was "isic-cli-5.1.0.tar", last modified: Thu Apr 13 23:15:59 2023, max compression
```

## Comparing `isic-cli-5.0.0.tar` & `isic-cli-5.1.0.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 17:36:09.798738 isic-cli-5.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-01-20 17:35:51.000000 isic-cli-5.0.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-01-20 17:35:51.000000 isic-cli-5.0.0/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 17:36:09.790738 isic-cli-5.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 17:36:09.794738 isic-cli-5.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-01-20 17:35:51.000000 isic-cli-5.0.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-01-20 17:35:51.000000 isic-cli-5.0.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-01-20 17:35:51.000000 isic-cli-5.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-01-20 17:35:51.000000 isic-cli-5.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-01-20 17:36:09.794738 isic-cli-5.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-01-20 17:35:51.000000 isic-cli-5.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 17:36:09.794738 isic-cli-5.0.0/isic_cli/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-01-20 17:35:51.000000 isic-cli-5.0.0/isic_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 17:36:09.794738 isic-cli-5.0.0/isic_cli/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     7979 2023-01-20 17:35:51.000000 isic-cli-5.0.0/isic_cli/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-01-20 17:35:51.000000 isic-cli-5.0.0/isic_cli/cli/accession.py
--rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-01-20 17:35:51.000000 isic-cli-5.0.0/isic_cli/cli/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-01-20 17:35:51.000000 isic-cli-5.0.0/isic_cli/cli/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-01-20 17:35:51.000000 isic-cli-5.0.0/isic_cli/cli/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-01-20 17:35:51.000000 isic-cli-5.0.0/isic_cli/cli/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-01-20 17:35:51.000000 isic-cli-5.0.0/isic_cli/cli/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-01-20 17:35:51.000000 isic-cli-5.0.0/isic_cli/cli/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-01-20 17:35:51.000000 isic-cli-5.0.0/isic_cli/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 17:36:09.794738 isic-cli-5.0.0/isic_cli/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 17:35:51.000000 isic-cli-5.0.0/isic_cli/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-01-20 17:35:51.000000 isic-cli-5.0.0/isic_cli/io/http.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-01-20 17:35:51.000000 isic-cli-5.0.0/isic_cli/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-01-20 17:35:51.000000 isic-cli-5.0.0/isic_cli/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 17:36:09.794738 isic-cli-5.0.0/isic_cli/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 17:35:51.000000 isic-cli-5.0.0/isic_cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-01-20 17:35:51.000000 isic-cli-5.0.0/isic_cli/utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 17:36:09.794738 isic-cli-5.0.0/isic_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-01-20 17:36:09.000000 isic-cli-5.0.0/isic_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-01-20 17:36:09.000000 isic-cli-5.0.0/isic_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-20 17:36:09.000000 isic-cli-5.0.0/isic_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-01-20 17:36:09.000000 isic-cli-5.0.0/isic_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-01-20 17:36:09.000000 isic-cli-5.0.0/isic_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-20 17:36:09.000000 isic-cli-5.0.0/isic_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-01-20 17:35:51.000000 isic-cli-5.0.0/justfile
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-01-20 17:35:51.000000 isic-cli-5.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-20 17:36:09.798738 isic-cli-5.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-01-20 17:35:51.000000 isic-cli-5.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 17:36:09.794738 isic-cli-5.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-01-20 17:35:51.000000 isic-cli-5.0.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-01-20 17:35:51.000000 isic-cli-5.0.0/tests/test_cli_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-01-20 17:35:51.000000 isic-cli-5.0.0/tests/test_cli_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-01-20 17:35:51.000000 isic-cli-5.0.0/tests/test_cli_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-01-20 17:35:51.000000 isic-cli-5.0.0/tests/test_cli_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-20 17:35:51.000000 isic-cli-5.0.0/tests/test_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-01-20 17:35:51.000000 isic-cli-5.0.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-01-20 17:35:51.000000 isic-cli-5.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:15:59.913542 isic-cli-5.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-13 23:15:37.000000 isic-cli-5.1.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-13 23:15:37.000000 isic-cli-5.1.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:15:59.897542 isic-cli-5.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:15:59.901542 isic-cli-5.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-13 23:15:37.000000 isic-cli-5.1.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-13 23:15:37.000000 isic-cli-5.1.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-13 23:15:37.000000 isic-cli-5.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-13 23:15:37.000000 isic-cli-5.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-04-13 23:15:59.913542 isic-cli-5.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-13 23:15:37.000000 isic-cli-5.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:15:59.905542 isic-cli-5.1.0/isic_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-13 23:15:37.000000 isic-cli-5.1.0/isic_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:15:59.913542 isic-cli-5.1.0/isic_cli/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     7979 2023-04-13 23:15:37.000000 isic-cli-5.1.0/isic_cli/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-04-13 23:15:37.000000 isic-cli-5.1.0/isic_cli/cli/accession.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-04-13 23:15:37.000000 isic-cli-5.1.0/isic_cli/cli/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-13 23:15:37.000000 isic-cli-5.1.0/isic_cli/cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-04-13 23:15:37.000000 isic-cli-5.1.0/isic_cli/cli/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-04-13 23:15:37.000000 isic-cli-5.1.0/isic_cli/cli/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-13 23:15:37.000000 isic-cli-5.1.0/isic_cli/cli/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-13 23:15:37.000000 isic-cli-5.1.0/isic_cli/cli/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-04-13 23:15:37.000000 isic-cli-5.1.0/isic_cli/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:15:59.913542 isic-cli-5.1.0/isic_cli/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 23:15:37.000000 isic-cli-5.1.0/isic_cli/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-04-13 23:15:37.000000 isic-cli-5.1.0/isic_cli/io/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-13 23:15:37.000000 isic-cli-5.1.0/isic_cli/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-13 23:15:37.000000 isic-cli-5.1.0/isic_cli/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:15:59.913542 isic-cli-5.1.0/isic_cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 23:15:37.000000 isic-cli-5.1.0/isic_cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-13 23:15:37.000000 isic-cli-5.1.0/isic_cli/utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:15:59.913542 isic-cli-5.1.0/isic_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-04-13 23:15:59.000000 isic-cli-5.1.0/isic_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-13 23:15:59.000000 isic-cli-5.1.0/isic_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 23:15:59.000000 isic-cli-5.1.0/isic_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-13 23:15:59.000000 isic-cli-5.1.0/isic_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-13 23:15:59.000000 isic-cli-5.1.0/isic_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-13 23:15:59.000000 isic-cli-5.1.0/isic_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-13 23:15:37.000000 isic-cli-5.1.0/justfile
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-13 23:15:37.000000 isic-cli-5.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 23:15:59.913542 isic-cli-5.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-04-13 23:15:37.000000 isic-cli-5.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 23:15:59.913542 isic-cli-5.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-13 23:15:37.000000 isic-cli-5.1.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-04-13 23:15:37.000000 isic-cli-5.1.0/tests/test_cli_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-04-13 23:15:37.000000 isic-cli-5.1.0/tests/test_cli_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-13 23:15:37.000000 isic-cli-5.1.0/tests/test_cli_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-04-13 23:15:37.000000 isic-cli-5.1.0/tests/test_cli_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-13 23:15:37.000000 isic-cli-5.1.0/tests/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-13 23:15:37.000000 isic-cli-5.1.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-13 23:15:37.000000 isic-cli-5.1.0/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-13 23:15:37.000000 isic-cli-5.1.0/tox.ini
```

### Comparing `isic-cli-5.0.0/.github/workflows/ci.yml` & `isic-cli-5.1.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `isic-cli-5.0.0/.github/workflows/release.yml` & `isic-cli-5.1.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `isic-cli-5.0.0/.gitignore` & `isic-cli-5.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `isic-cli-5.0.0/LICENSE` & `isic-cli-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `isic-cli-5.0.0/PKG-INFO` & `isic-cli-5.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isic-cli
-Version: 5.0.0
+Version: 5.1.0
 Home-page: https://github.com/ImageMarkup/isic-cli
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/ImageMarkup/isic-cli/issues
 Project-URL: Source, https://github.com/ImageMarkup/isic-cli
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `isic-cli-5.0.0/README.md` & `isic-cli-5.1.0/README.md`

 * *Files identical despite different names*

### Comparing `isic-cli-5.0.0/isic_cli/cli/__init__.py` & `isic-cli-5.1.0/isic_cli/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `isic-cli-5.0.0/isic_cli/cli/accession.py` & `isic-cli-5.1.0/isic_cli/cli/accession.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 @require_login
 def upload(
     ctx: IsicContext,
     cohort_id: int,
     accession: Path,
     json_: bool,
 ):
-
     console = Console(stderr=True)
     with console.status("Uploading"):
         from isic_cli.cli import DOMAINS
 
         s3ff_client = S3FileFieldClient(f"{DOMAINS[ctx.env]}/api/v2/s3-upload/", ctx.session)
 
         with accession.open("rb") as file_stream:
```

### Comparing `isic-cli-5.0.0/isic_cli/cli/collection.py` & `isic-cli-5.1.0/isic_cli/cli/collection.py`

 * *Files identical despite different names*

### Comparing `isic-cli-5.0.0/isic_cli/cli/image.py` & `isic-cli-5.1.0/isic_cli/cli/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import click
 from click.types import IntRange
 from humanize import intcomma
 from rich.console import Console
 from rich.progress import Progress
 
 from isic_cli.cli.context import IsicContext
-from isic_cli.cli.types import SearchString
+from isic_cli.cli.types import CommaSeparatedIdentifiers, SearchString
 from isic_cli.cli.utils import _extract_metadata, get_attributions, suggest_guest_login
 from isic_cli.io.http import download_image, get_images, get_num_images
 
 
 def cleanup_partially_downloaded_files(directory: Path) -> None:
     for p in directory.glob("**/.isic-partial.*"):
         # missing_ok=True because it's possible that another thread moved the temporary file to
@@ -41,14 +41,15 @@
     type=SearchString(),
     default="",
     help="e.g. 'diagnosis:\"solar lentigo\" AND age_approx:50'",
 )
 @click.option(
     "-c",
     "--collections",
+    type=CommaSeparatedIdentifiers(),
     default="",
     help=(
         "Filter the images based on a comma separated string of collection"
         " ids (see isic collection list)."
     ),
 )
 @click.option(
```

### Comparing `isic-cli-5.0.0/isic_cli/cli/metadata.py` & `isic-cli-5.1.0/isic_cli/cli/metadata.py`

 * *Files identical despite different names*

### Comparing `isic-cli-5.0.0/isic_cli/cli/types.py` & `isic-cli-5.1.0/isic_cli/cli/types.py`

 * *Files identical despite different names*

### Comparing `isic-cli-5.0.0/isic_cli/cli/user.py` & `isic-cli-5.1.0/isic_cli/cli/user.py`

 * *Files identical despite different names*

### Comparing `isic-cli-5.0.0/isic_cli/cli/utils.py` & `isic-cli-5.1.0/isic_cli/cli/utils.py`

 * *Files identical despite different names*

### Comparing `isic-cli-5.0.0/isic_cli/io/http.py` & `isic-cli-5.1.0/isic_cli/io/http.py`

 * *Files identical despite different names*

### Comparing `isic-cli-5.0.0/isic_cli/session.py` & `isic-cli-5.1.0/isic_cli/session.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,11 +50,12 @@
 
         return r
 
 
 def get_session(
     base_url: str = "https://api.isic-archive.com/api/v2/", headers: Optional[dict] = None
 ) -> IsicCliSession:
+    logger.debug(f"Establishing requests session with {base_url}")
     session = IsicCliSession(base_url)
     if headers:
         session.headers.update(headers)
     return session
```

### Comparing `isic-cli-5.0.0/isic_cli/utils/version.py` & `isic-cli-5.1.0/isic_cli/utils/version.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from importlib.metadata import PackageNotFoundError, version
 import logging
 import sys
 from typing import Optional
 
 import click
 from packaging.version import Version
-from pkg_resources import parse_version
 import requests
 from requests.exceptions import RequestException
 
 logger = logging.getLogger(__name__)
 
 
 def get_version() -> Optional[Version]:
     try:
-        return parse_version(version("isic-cli"))
+        return Version(version("isic-cli"))
     except PackageNotFoundError:
         # package is not installed
         return None
 
 
 def is_dev_install():
     version = get_version()
@@ -30,18 +29,22 @@
         return "major"
     elif to_version.minor > from_version.minor:
         return "minor"
     elif to_version.micro > from_version.micro:
         return "micro"
 
 
-def newest_version_available() -> Optional[Version]:
+def _pypi_releases():
     r = requests.get("https://pypi.org/pypi/isic-cli/json", timeout=(5, 5))
     r.raise_for_status()
-    releases = [parse_version(v) for v in r.json()["releases"].keys()]
+    return r.json()["releases"]
+
+
+def newest_version_available() -> Optional[Version]:
+    releases = [Version(v) for v in _pypi_releases().keys()]
     real_releases = [x for x in releases if not x.is_prerelease and not x.is_devrelease]
     if real_releases:
         return sorted(real_releases)[-1]
 
 
 def check_for_newer_version():
     this_version = get_version()
```

### Comparing `isic-cli-5.0.0/isic_cli.egg-info/PKG-INFO` & `isic-cli-5.1.0/isic_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isic-cli
-Version: 5.0.0
+Version: 5.1.0
 Home-page: https://github.com/ImageMarkup/isic-cli
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/ImageMarkup/isic-cli/issues
 Project-URL: Source, https://github.com/ImageMarkup/isic-cli
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `isic-cli-5.0.0/isic_cli.egg-info/SOURCES.txt` & `isic-cli-5.1.0/isic_cli.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -33,8 +33,9 @@
 isic_cli/utils/version.py
 tests/conftest.py
 tests/test_cli_base.py
 tests/test_cli_collection.py
 tests/test_cli_image.py
 tests/test_cli_metadata.py
 tests/test_user.py
-tests/test_utils.py
+tests/test_utils.py
+tests/test_version.py
```

### Comparing `isic-cli-5.0.0/pyproject.toml` & `isic-cli-5.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `isic-cli-5.0.0/setup.py` & `isic-cli-5.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,15 +32,16 @@
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python",
     ],
     python_requires=">=3.9",
     packages=find_packages(),
     entry_points={"console_scripts": ["isic = isic_cli.cli:main"]},
     install_requires=[
-        "click",
+        # we use the path_type=Path feature from click which was added in Click 8
+        "click>=8",
         "django-s3-file-field-client",
         "girder-cli-oauth-client",
         "humanize",
         "isic-metadata>=0.0.6",
         "more-itertools",
         "numpy",
         "packaging",
```

### Comparing `isic-cli-5.0.0/tests/conftest.py` & `isic-cli-5.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `isic-cli-5.0.0/tests/test_cli_base.py` & `isic-cli-5.1.0/tests/test_cli_base.py`

 * *Files identical despite different names*

### Comparing `isic-cli-5.0.0/tests/test_cli_collection.py` & `isic-cli-5.1.0/tests/test_cli_collection.py`

 * *Files identical despite different names*

### Comparing `isic-cli-5.0.0/tests/test_cli_image.py` & `isic-cli-5.1.0/tests/test_cli_image.py`

 * *Files identical despite different names*

### Comparing `isic-cli-5.0.0/tests/test_cli_metadata.py` & `isic-cli-5.1.0/tests/test_cli_metadata.py`

 * *Files identical despite different names*

### Comparing `isic-cli-5.0.0/tests/test_utils.py` & `isic-cli-5.1.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `isic-cli-5.0.0/tox.ini` & `isic-cli-5.1.0/tox.ini`

 * *Files identical despite different names*

