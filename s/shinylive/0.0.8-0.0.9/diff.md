# Comparing `tmp/shinylive-0.0.8.tar.gz` & `tmp/shinylive-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shinylive-0.0.8.tar", last modified: Wed Oct 26 17:50:46 2022, max compression
+gzip compressed data, was "shinylive-0.0.9.tar", last modified: Thu Mar  2 20:10:17 2023, max compression
```

## Comparing `shinylive-0.0.8.tar` & `shinylive-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 17:50:46.256404 shinylive-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-10-26 17:50:40.000000 shinylive-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4288 2022-10-26 17:50:46.256404 shinylive-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3402 2022-10-26 17:50:40.000000 shinylive-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1359 2022-10-26 17:50:46.260404 shinylive-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-26 17:50:40.000000 shinylive-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 17:50:46.256404 shinylive-0.0.8/shinylive/
--rw-r--r--   0 runner    (1001) docker     (121)      158 2022-10-26 17:50:40.000000 shinylive-0.0.8/shinylive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4210 2022-10-26 17:50:40.000000 shinylive-0.0.8/shinylive/_app_json.py
--rw-r--r--   0 runner    (1001) docker     (121)     7383 2022-10-26 17:50:40.000000 shinylive-0.0.8/shinylive/_assets.py
--rw-r--r--   0 runner    (1001) docker     (121)    14801 2022-10-26 17:50:40.000000 shinylive-0.0.8/shinylive/_deps.py
--rw-r--r--   0 runner    (1001) docker     (121)     3936 2022-10-26 17:50:40.000000 shinylive-0.0.8/shinylive/_export.py
--rw-r--r--   0 runner    (1001) docker     (121)     6688 2022-10-26 17:50:40.000000 shinylive-0.0.8/shinylive/_main.py
--rw-r--r--   0 runner    (1001) docker     (121)     3433 2022-10-26 17:50:40.000000 shinylive-0.0.8/shinylive/_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-10-26 17:50:40.000000 shinylive-0.0.8/shinylive/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 17:50:46.256404 shinylive-0.0.8/shinylive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4288 2022-10-26 17:50:46.000000 shinylive-0.0.8/shinylive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      435 2022-10-26 17:50:46.000000 shinylive-0.0.8/shinylive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-26 17:50:46.000000 shinylive-0.0.8/shinylive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-10-26 17:50:46.000000 shinylive-0.0.8/shinylive.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-26 17:50:46.000000 shinylive-0.0.8/shinylive.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-10-26 17:50:46.000000 shinylive-0.0.8/shinylive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-10-26 17:50:46.000000 shinylive-0.0.8/shinylive.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:10:17.671871 shinylive-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-02 20:10:08.000000 shinylive-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-03-02 20:10:17.671871 shinylive-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-03-02 20:10:08.000000 shinylive-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-03-02 20:10:17.671871 shinylive-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-02 20:10:08.000000 shinylive-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:10:17.671871 shinylive-0.0.9/shinylive/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-03-02 20:10:08.000000 shinylive-0.0.9/shinylive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-03-02 20:10:08.000000 shinylive-0.0.9/shinylive/_app_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-03-02 20:10:08.000000 shinylive-0.0.9/shinylive/_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14741 2023-03-02 20:10:08.000000 shinylive-0.0.9/shinylive/_deps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-03-02 20:10:08.000000 shinylive-0.0.9/shinylive/_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-03-02 20:10:08.000000 shinylive-0.0.9/shinylive/_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-03-02 20:10:08.000000 shinylive-0.0.9/shinylive/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-03-02 20:10:08.000000 shinylive-0.0.9/shinylive/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 20:10:17.671871 shinylive-0.0.9/shinylive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-03-02 20:10:17.000000 shinylive-0.0.9/shinylive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-03-02 20:10:17.000000 shinylive-0.0.9/shinylive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 20:10:17.000000 shinylive-0.0.9/shinylive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-02 20:10:17.000000 shinylive-0.0.9/shinylive.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 20:10:17.000000 shinylive-0.0.9/shinylive.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-03-02 20:10:17.000000 shinylive-0.0.9/shinylive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-02 20:10:17.000000 shinylive-0.0.9/shinylive.egg-info/top_level.txt
```

### Comparing `shinylive-0.0.8/LICENSE` & `shinylive-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `shinylive-0.0.8/PKG-INFO` & `shinylive-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shinylive
-Version: 0.0.8
+Version: 0.0.9
 Summary: Run Shiny applications running Python in the browser.
 Home-page: https://github.com/rstudio/py-shinylive
 Author: Winston Chang
 Author-email: winston@rstudio.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/rstudio/py-shinylive/issues
 Project-URL: Documentation, https://shiny.rstudio.com/py/docs/shinylive.html
@@ -15,14 +15,16 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: test
+Provides-Extra: dev
 License-File: LICENSE
 
 Shinylive Python package
 ========================
 
 [![Build and test](https://github.com/rstudio/py-shinylive/actions/workflows/build.yml/badge.svg)](https://github.com/rstudio/py-shinylive/actions/)
 [![PyPI Latest Release](https://img.shields.io/pypi/v/shinylive.svg)](https://pypi.org/project/shinylive/)
@@ -53,15 +55,15 @@
 ```
 shinylive export myapp site
 ```
 
 Then you can preview the application by running a web server and visiting it in a browser:
 
 ```
-python3 -m http.server --directory site 8008
+python3 -m http.server --directory site --bind localhost 8008
 ```
 
 At this point, you can deploy the `site/` directory to any static web hosting service.
 
 
 ### Multiple applications
```

### Comparing `shinylive-0.0.8/README.md` & `shinylive-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 ```
 shinylive export myapp site
 ```
 
 Then you can preview the application by running a web server and visiting it in a browser:
 
 ```
-python3 -m http.server --directory site 8008
+python3 -m http.server --directory site --bind localhost 8008
 ```
 
 At this point, you can deploy the `site/` directory to any static web hosting service.
 
 
 ### Multiple applications
```

### Comparing `shinylive-0.0.8/shinylive/_app_json.py` & `shinylive-0.0.9/shinylive/_app_json.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,44 +1,46 @@
+from __future__ import annotations
+
 import base64
 import json
 import os
 from pathlib import Path
-from typing import List, Literal, TypedDict
+from typing import Literal, TypedDict
 
 from . import _utils
 
 
 # This is the same as the FileContentJson type in TypeScript.
 class FileContentJson(TypedDict):
     name: str
     content: str
     type: Literal["text", "binary"]
 
 
 class AppInfo(TypedDict):
     appdir: str
     subdir: str
-    files: List[FileContentJson]
+    files: list[FileContentJson]
 
 
 # =============================================================================
-def read_app_files(appdir: Path, destdir: Path) -> List[FileContentJson]:
+def read_app_files(appdir: Path, destdir: Path) -> list[FileContentJson]:
     """
     Load files for a Shiny application.
 
     Parameters
     ----------
     appdir : str
        Directory containing the application.
 
     destdir : str
        Destination directory. This is used only to avoid adding shinylive assets when
        they are in a subdir of the application.
     """
-    app_files: List[FileContentJson] = []
+    app_files: list[FileContentJson] = []
     # Recursively iterate over files in app directory, and collect the files into
     # app_files data structure.
     exclude_names = {"__pycache__", "venv", ".venv"}
     for root, dirs, files in os.walk(appdir, topdown=True):
         root = Path(root)
 
         if _utils.is_relative_to(Path(root), destdir):
```

### Comparing `shinylive-0.0.8/shinylive/_assets.py` & `shinylive-0.0.9/shinylive/_assets.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
+from __future__ import annotations
+
 import os
 import re
 import shutil
 import sys
 import urllib.request
 from pathlib import Path
-from typing import List, Optional, Union
+from typing import Optional
 
-from ._version import SHINYLIVE_ASSETS_VERSION
 from ._utils import tar_safe_extractall
+from ._version import SHINYLIVE_ASSETS_VERSION
 
 
 def download_shinylive(
-    destdir: Union[str, Path, None] = None,
+    destdir: str | Path | None = None,
     version: str = SHINYLIVE_ASSETS_VERSION,
     url: Optional[str] = None,
 ) -> None:
     if destdir is None:
         # Note that this is the cache directory, which is the parent of the assets
         # directory. The tarball will have the assets directory as the top-level subdir.
         destdir = shinylive_cache_dir()
@@ -68,16 +70,16 @@
 def repodata_json_file(version: str = SHINYLIVE_ASSETS_VERSION) -> Path:
     return (
         Path(shinylive_assets_dir(version)) / "shinylive" / "pyodide" / "repodata.json"
     )
 
 
 def copy_shinylive_local(
-    source_dir: Union[str, Path],
-    destdir: Optional[Union[str, Path]] = None,
+    source_dir: str | Path,
+    destdir: Optional[str | Path] = None,
     version: str = SHINYLIVE_ASSETS_VERSION,
 ):
     if destdir is None:
         destdir = Path(shinylive_cache_dir())
 
     destdir = Path(destdir)
 
@@ -90,16 +92,16 @@
     elif target_dir.is_dir():
         shutil.rmtree(target_dir)
 
     shutil.copytree(source_dir, target_dir)
 
 
 def link_shinylive_local(
-    source_dir: Union[str, Path],
-    destdir: Optional[Union[str, Path]] = None,
+    source_dir: str | Path,
+    destdir: Optional[str | Path] = None,
     version: str = SHINYLIVE_ASSETS_VERSION,
 ):
     if destdir is None:
         destdir = Path(shinylive_cache_dir())
 
     destdir = Path(destdir)
 
@@ -114,15 +116,15 @@
     elif target_dir.is_dir():
         shutil.rmtree(target_dir)
 
     target_dir.symlink_to(source_dir)
 
 
 def ensure_shinylive_assets(
-    destdir: Union[Path, None] = None,
+    destdir: Path | None = None,
     version: str = SHINYLIVE_ASSETS_VERSION,
     url: Optional[str] = None,
 ) -> Path:
     """Ensure that there is a local copy of shinylive."""
 
     if destdir is None:
         destdir = Path(shinylive_cache_dir())
@@ -139,15 +141,15 @@
         print(f"{shinylive_bundle_dir} does not exist.", file=sys.stderr)
         download_shinylive(url=url, version=version, destdir=destdir)
 
     return shinylive_bundle_dir
 
 
 def cleanup_shinylive_assets(
-    shinylive_dir: Union[str, Path],
+    shinylive_dir: str | Path,
 ) -> None:
     """Removes local copies of shinylive web assets, except for the one used by the
     current version of the shinylive python package.
 
     Parameters
     ----------
     shinylive_dir
@@ -163,16 +165,16 @@
         print("Keeping version " + SHINYLIVE_ASSETS_VERSION)
         version.remove(SHINYLIVE_ASSETS_VERSION)
 
     remove_shinylive_assets(shinylive_dir, version)
 
 
 def remove_shinylive_assets(
-    shinylive_dir: Union[str, Path],
-    version: Union[str, List[str]],
+    shinylive_dir: str | Path,
+    version: str | list[str],
 ) -> None:
     """Removes local copy of shinylive.
 
     Parameters
     ----------
     shinylive_dir
         The directory where shinylive is stored. If None, the default directory will
@@ -202,15 +204,15 @@
             target_dir.unlink()
         elif target_dir.is_dir():
             shutil.rmtree(target_dir)
         else:
             print(f"{target_dir} does not exist.")
 
 
-def _installed_shinylive_versions(shinylive_dir: Optional[Path] = None) -> List[str]:
+def _installed_shinylive_versions(shinylive_dir: Optional[Path] = None) -> list[str]:
     if shinylive_dir is None:
         shinylive_dir = Path(shinylive_cache_dir())
 
     shinylive_dir = Path(shinylive_dir)
     subdirs = shinylive_dir.iterdir()
     subdirs = [re.sub("^shinylive-", "", str(s)) for s in subdirs]
     return subdirs
```

### Comparing `shinylive-0.0.8/shinylive/_deps.py` & `shinylive-0.0.9/shinylive/_deps.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,26 +6,26 @@
 import copy
 import functools
 import json
 import os
 import sys
 from pathlib import Path
 from textwrap import dedent
-from typing import Callable, Dict, Iterable, List, Literal, Optional, Set, Union
+from typing import Callable, Iterable, Literal, Optional
 
 # Even though TypedDict is available in Python 3.8, because it's used with NotRequired,
 # they should both come from the same typing module.
 # https://peps.python.org/pep-0655/#usage-in-python-3-11
 if sys.version_info >= (3, 11):
     from typing import NotRequired, TypedDict
 else:
     from typing_extensions import NotRequired, TypedDict
 
-from ._assets import shinylive_assets_dir, repodata_json_file, ensure_shinylive_assets
 from ._app_json import FileContentJson
+from ._assets import ensure_shinylive_assets, repodata_json_file, shinylive_assets_dir
 from ._version import SHINYLIVE_ASSETS_VERSION
 
 # Files in Pyodide that should always be included.
 BASE_PYODIDE_FILES = {
     "pyodide_py.tar",
     "pyodide.asm.js",
     "pyodide.asm.data",
@@ -43,57 +43,57 @@
 # Note: This block of code is copied from /scripts/pyodide_packages.py
 class PyodidePackageInfo(TypedDict):
     name: str
     version: str
     file_name: str
     install_dir: Literal["lib", "site"]
     sha256: str
-    depends: List[str]
-    imports: List[str]
+    depends: list[str]
+    imports: list[str]
     unvendored_tests: NotRequired[bool]
 
 
 # The package information structure used by Pyodide's repodata.json.
 class PyodideRepodataFile(TypedDict):
-    info: Dict[str, str]
-    packages: Dict[str, PyodidePackageInfo]
+    info: dict[str, str]
+    packages: dict[str, PyodidePackageInfo]
 
 
 # =============================================================================
 # HTML Dependency types
 # =============================================================================
 class HtmlDepItem(TypedDict):
     name: str
     path: str
-    attribs: NotRequired[Dict[str, str]]
+    attribs: NotRequired[dict[str, str]]
 
 
 class HtmlDepServiceworkerItem(TypedDict):
     source: str
     destination: str
 
 
 class QuartoHtmlDependency(TypedDict):
     name: str
     version: NotRequired[str]
-    scripts: NotRequired[List[Union[str, HtmlDepItem]]]
-    stylesheets: NotRequired[List[Union[str, HtmlDepItem]]]
-    resources: NotRequired[List[HtmlDepItem]]
-    meta: NotRequired[Dict[str, str]]
-    serviceworkers: NotRequired[List[HtmlDepServiceworkerItem]]
+    scripts: NotRequired[list[str | HtmlDepItem]]
+    stylesheets: NotRequired[list[str | HtmlDepItem]]
+    resources: NotRequired[list[HtmlDepItem]]
+    meta: NotRequired[dict[str, str]]
+    serviceworkers: NotRequired[list[HtmlDepServiceworkerItem]]
 
 
 # =============================================================================
 # Conversion functions
 # =============================================================================
 def _dep_names_to_pyodide_pkg_infos(
     dep_names: Iterable[str],
-) -> List[PyodidePackageInfo]:
+) -> list[PyodidePackageInfo]:
     repodata = _pyodide_repodata()
-    pkg_infos: List[PyodidePackageInfo] = [
+    pkg_infos: list[PyodidePackageInfo] = [
         copy.deepcopy(repodata["packages"][dep_name]) for dep_name in dep_names
     ]
     return pkg_infos
 
 
 def _pyodide_pkg_info_to_quarto_html_dep_item(
     pkg: PyodidePackageInfo,
@@ -107,25 +107,25 @@
     return {
         "name": os.path.join("shinylive", "pyodide", pkg["file_name"]),
         "path": os.path.join(assets_dir, "shinylive", "pyodide", pkg["file_name"]),
     }
 
 
 def _pyodide_pkg_infos_to_quarto_html_dep_items(
-    pkgs: List[PyodidePackageInfo],
-) -> List[HtmlDepItem]:
+    pkgs: list[PyodidePackageInfo],
+) -> list[HtmlDepItem]:
     return [_pyodide_pkg_info_to_quarto_html_dep_item(pkg) for pkg in pkgs]
 
 
 # =============================================================================
 # Shinylive base dependencies
 # =============================================================================
 def shinylive_base_deps_htmldep(
     sw_dir: Optional[str] = None,
-) -> List[QuartoHtmlDependency]:
+) -> list[QuartoHtmlDependency]:
     return [
         _serviceworker_dep(sw_dir),
         _shinylive_common_dep_htmldep(),
     ]
 
 
 # =============================================================================
@@ -138,17 +138,17 @@
     """
     assets_dir = shinylive_assets_dir()
 
     # First, get the list of base files.
     base_files = shinylive_common_files()
 
     # Next, categorize the base files into scripts, stylesheets, and resources.
-    scripts: List[Union[str, HtmlDepItem]] = []
-    stylesheets: List[Union[str, HtmlDepItem]] = []
-    resources: List[HtmlDepItem] = []
+    scripts: list[str | HtmlDepItem] = []
+    stylesheets: list[str | HtmlDepItem] = []
+    resources: list[HtmlDepItem] = []
 
     for file in base_files:
         if os.path.basename(file) in [
             "load-shinylive-sw.js",
             "run-python-blocks.js",
         ]:
             script_item: HtmlDepItem = {
@@ -182,15 +182,15 @@
             )
 
     # Add base python packages as resources
     resources.extend(base_package_deps_htmldepitems())
 
     # Sort scripts so that load-serviceworker.js is first, and run-python-blocks.js is
     # last.
-    def scripts_sort_fun(x: Union[str, HtmlDepItem]) -> int:
+    def scripts_sort_fun(x: str | HtmlDepItem) -> int:
         if isinstance(x, str):
             filename = x
         else:
             filename = os.path.basename(x["name"])
 
         if filename == "load-serviceworker.js":
             return 0
@@ -206,22 +206,22 @@
         "version": SHINYLIVE_ASSETS_VERSION,
         "scripts": scripts,
         "stylesheets": stylesheets,
         "resources": resources,
     }
 
 
-def shinylive_common_files() -> List[str]:
+def shinylive_common_files() -> list[str]:
     """
     Return a list of files that are base dependencies; in other words, the files that are
     always included in a Shinylive deployment.
     """
     ensure_shinylive_assets()
 
-    base_files: List[str] = []
+    base_files: list[str] = []
     for root, dirs, files in os.walk(shinylive_assets_dir()):
         root = Path(root)
         rel_root = root.relative_to(shinylive_assets_dir())
         if rel_root == Path("."):
             dirs.remove("scripts")
             dirs.remove("export_template")
         elif rel_root == Path("shinylive"):
@@ -257,18 +257,18 @@
     return dep
 
 
 # =============================================================================
 # Find which packages are used by a Shiny application
 # =============================================================================
 def package_deps_htmldepitems(
-    json_file: Optional[Union[str, Path]],
+    json_file: Optional[str | Path],
     json_content: Optional[str],
     verbose: bool = True,
-) -> List[HtmlDepItem]:
+) -> list[HtmlDepItem]:
     """
     Find package dependencies from an app.json file, and return as a list of
     QuartoHtmlDependency objects.
 
     Requires either `json_file` or `json_content`, but not both.
     """
 
@@ -277,15 +277,15 @@
     ):
         raise RuntimeError("Must provide either `json_file` or `json_content`.")
 
     def verbose_print(*args: object) -> None:
         if verbose:
             print(*args, file=sys.stderr)
 
-    file_contents: List[FileContentJson] = []
+    file_contents: list[FileContentJson] = []
 
     if json_file is not None:
         json_file = Path(json_file)
         with open(json_file) as f:
             file_contents = json.load(f)
 
     if json_content is not None:
@@ -293,47 +293,47 @@
 
     pkg_infos = find_package_deps(file_contents)
     deps = _pyodide_pkg_infos_to_quarto_html_dep_items(pkg_infos)
     return deps
 
 
 def find_package_deps(
-    app_contents: List[FileContentJson],
+    app_contents: list[FileContentJson],
     verbose_print: Callable[..., None] = lambda *args: None,
-) -> List[PyodidePackageInfo]:
+) -> list[PyodidePackageInfo]:
     """
     Find package dependencies from the contents of an app.json file. The returned data
     structure is a list of PyodidePackageInfo objects.
     """
 
-    imports: Set[str] = _find_import_app_contents(app_contents)
+    imports: set[str] = _find_import_app_contents(app_contents)
 
     # TODO: Need to also add in requirements.txt, and find dependencies of those
     # packages, in case any of those dependencies are included as part of pyodide.
     verbose_print("Imports detected in app:\n ", ", ".join(sorted(imports)))
 
     dep_names = _find_recursive_deps(imports, verbose_print)
     pkg_infos = _dep_names_to_pyodide_pkg_infos(dep_names)
 
     return pkg_infos
 
 
-def base_package_deps_htmldepitems() -> List[HtmlDepItem]:
+def base_package_deps_htmldepitems() -> list[HtmlDepItem]:
     """
     Return list of packages that should be included in all Shinylive deployments. The
     returned data structure is a list of PyodidePackageInfo objects.
     """
     dep_names = _find_recursive_deps(BASE_PYODIDE_PACKAGES)
     pkg_infos = _dep_names_to_pyodide_pkg_infos(dep_names)
     deps = _pyodide_pkg_infos_to_quarto_html_dep_items(pkg_infos)
 
     return deps
 
 
-def base_package_deps() -> List[PyodidePackageInfo]:
+def base_package_deps() -> list[PyodidePackageInfo]:
     """
     Return list of packages that should be included in all Shinylive deployments. The
     returned data structure is a list of PyodidePackageInfo objects.
     """
     dep_names = _find_recursive_deps(BASE_PYODIDE_PACKAGES)
     pkg_infos = _dep_names_to_pyodide_pkg_infos(dep_names)
 
@@ -342,15 +342,15 @@
 
 # =============================================================================
 # Internal functions
 # =============================================================================
 def _find_recursive_deps(
     pkgs: Iterable[str],
     verbose_print: Callable[..., None] = lambda *args: None,
-) -> List[str]:
+) -> list[str]:
     """
     Given a list of packages, recursively find all dependencies that are contained in
     repodata.json. This returns a list of all dependencies, including the original
     packages passed in.
     """
     repodata = _pyodide_repodata()
     deps = list(pkgs)
@@ -379,30 +379,30 @@
     Given the name of a dependency, like "pandas", return the name of the .whl file,
     like "pandas-1.4.2-cp310-cp310-emscripten_3_1_14_wasm32.whl".
     """
     repodata = _pyodide_repodata()
     return repodata["packages"][dep_name]["file_name"]
 
 
-def _dep_names_to_dep_files(dep_names: List[str]) -> List[str]:
+def _dep_names_to_dep_files(dep_names: list[str]) -> list[str]:
     """
     Given a list of dependency names, like ["pandas"], return a list with the names of
     corresponding .whl files (from data in repodata.json), like
     ["pandas-1.4.2-cp310-cp310-emscripten_3_1_14_wasm32.whl"].
     """
     repodata = _pyodide_repodata()
     dep_files = [repodata["packages"][x]["file_name"] for x in dep_names]
     return dep_files
 
 
-def _find_import_app_contents(app_contents: List[FileContentJson]) -> Set[str]:
+def _find_import_app_contents(app_contents: list[FileContentJson]) -> set[str]:
     """
     Given an app.json file, find packages that are imported.
     """
-    imports: Set[str] = set()
+    imports: set[str] = set()
     for file_content in app_contents:
         if not file_content["name"].endswith(".py"):
             continue
 
         imports = imports.union(_find_imports(file_content["content"]))
 
     return imports
@@ -416,26 +416,26 @@
     restarted.
     """
     with open(repodata_json_file(), "r") as f:
         return json.load(f)
 
 
 # From pyodide._base.find_imports
-def _find_imports(source: str) -> List[str]:
+def _find_imports(source: str) -> list[str]:
     """
     Finds the imports in a Python source code string
 
     Parameters
     ----------
     source : str
        The Python source code to inspect for imports.
 
     Returns
     -------
-    ``List[str]``
+    ``list[str]``
         A list of module names that are imported in ``source``. If ``source`` is not
         syntactically correct Python code (after dedenting), returns an empty list.
 
     Examples
     --------
     >>> from pyodide import find_imports
     >>> source = "import numpy as np; import scipy.stats"
@@ -445,15 +445,15 @@
     # handle mis-indented input from multi-line strings
     source = dedent(source)
 
     try:
         mod = ast.parse(source)
     except SyntaxError:
         return []
-    imports: Set[str] = set()
+    imports: set[str] = set()
     for node in ast.walk(mod):
         if isinstance(node, ast.Import):
             for name in node.names:
                 node_name = name.name
                 imports.add(node_name.split(".")[0])
         elif isinstance(node, ast.ImportFrom):
             module_name = node.module
```

### Comparing `shinylive-0.0.8/shinylive/_export.py` & `shinylive-0.0.9/shinylive/_export.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,23 @@
+from __future__ import annotations
+
 import os
 import sys
 from pathlib import Path
-from typing import List, Union
 
 from . import _deps, _utils
 from ._app_json import AppInfo, read_app_files, write_app_json
 from ._assets import shinylive_assets_dir
 
 
 def export(
-    appdir: Union[str, Path],
-    destdir: Union[str, Path],
+    appdir: str | Path,
+    destdir: str | Path,
     *,
-    subdir: Union[str, Path, None] = None,
+    subdir: str | Path | None = None,
     verbose: bool = False,
     full_shinylive: bool = False,
 ):
     def verbose_print(*args: object) -> None:
         if verbose:
             print(*args)
 
@@ -80,15 +81,15 @@
             for file in package_files
             if os.path.join("shinylive", "pyodide", file) not in base_files
         ]
 
     else:
         deps = _deps.base_package_deps() + _deps.find_package_deps(app_info["files"])
 
-        package_files: List[str] = [dep["file_name"] for dep in deps]
+        package_files: list[str] = [dep["file_name"] for dep in deps]
 
         print(
             f"Copying imported packages from {assets_dir}/shinylive/pyodide/ to {destdir}/shinylive/pyodide/",
             file=sys.stderr,
         )
         verbose_print(" ", ", ".join(package_files))
 
@@ -107,10 +108,11 @@
     write_app_json(
         app_info,
         destdir,
         html_source_dir=Path(shinylive_assets_dir()) / "export_template",
     )
 
     print(
-        f"\nRun the following to serve the app:\n  python3 -m http.server --directory {destdir} 8008",
+        "\nRun the following to serve the app:\n"
+        f"  python3 -m http.server --directory {destdir} --bind localhost 8008",
         file=sys.stderr,
     )
```

### Comparing `shinylive-0.0.8/shinylive/_main.py` & `shinylive-0.0.9/shinylive/_main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+from __future__ import annotations
+
 import json
-from pathlib import Path
 import sys
-from typing import Optional, Union
+from pathlib import Path
+from typing import Optional
 
 import click
 
 from . import _assets, _deps, _export, _version
 
 
 @click.group(
@@ -38,15 +40,15 @@
 DESTDIR is the destination directory where the output files will be written to. This
 directory can be deployed as a static web site.
 
 This command will not include the contents of venv/ or any files that start with '.'
 
 After writing the output files, you can serve them locally with the following command:
 
-    python3 -m http.server --directory DESTDIR 8008
+    python3 -m http.server --directory DESTDIR --bind localhost 8008
 """,
     no_args_is_help=True,
 )
 @click.argument("appdir", type=str)
 @click.argument("destdir", type=str)
 @click.option(
     "--verbose",
@@ -68,15 +70,15 @@
     default=False,
     help="Include the full Shinylive assets, including all Pyodide packages. Without this flag, only the packages needed to run the application are included.",
     show_default=True,
 )
 def export(
     appdir: str,
     destdir: str,
-    subdir: Union[str, None],
+    subdir: str | None,
     verbose: bool,
     full_shinylive: bool,
 ) -> None:
     _export.export(
         appdir,
         destdir,
         subdir=subdir,
@@ -131,15 +133,15 @@
     default=None,
     help="Directory where shinylive assets will be copied from. Must be used with 'copy' command.",
 )
 def assets(
     command: str,
     version: Optional[str],
     url: Optional[str],
-    dir: Union[str, Path],
+    dir: Optional[str | Path],
     source: Optional[str],
 ) -> None:
     if dir is None:
         dir = _assets.shinylive_cache_dir()
     dir = Path(dir)
 
     if command == "download":
@@ -202,15 +204,15 @@
 @click.argument(
     "json_file",
     required=False,
     type=str,
     default=None,
 )
 def package_deps(json_file: Optional[str]) -> None:
-    json_content: Union[str, None] = None
+    json_content: str | None = None
     if json_file is None:
         json_content = sys.stdin.read()
 
     deps = _deps.package_deps_htmldepitems(json_file, json_content)
     print(json.dumps(deps, indent=2))
```

### Comparing `shinylive-0.0.8/shinylive/_utils.py` & `shinylive-0.0.9/shinylive/_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+from __future__ import annotations
+
 import filecmp
 import os
 import shutil
 import sys
 from pathlib import Path
-from typing import Callable, List, Union
+from typing import Callable
 
 
 def is_relative_to(path: Path, base: Path) -> bool:
     """
     Wrapper for `PurePath.is_relative_to`, which was added in Python 3.9.
     """
     if sys.version_info >= (3, 9):
@@ -16,15 +18,15 @@
         try:
             path.relative_to(base)
             return True
         except ValueError:
             return False
 
 
-def path_length(path: Union[str, Path]) -> int:
+def path_length(path: str | Path) -> int:
     """Returns the number of elements in a path.
 
     For example 'a' has length 1, 'a/b' has length 2, etc.
     """
 
     path = str(path)
     if os.path.isabs(path):
@@ -38,30 +40,30 @@
     # On Windows, replace backslashes with forward slashes.
     if os.name == "nt":
         path.replace("\\", "/")
 
     return len(path.split("/"))
 
 
-def listdir_recursive(dir: Union[str, Path]) -> List[str]:
+def listdir_recursive(dir: str | Path) -> list[str]:
     dir = Path(dir)
-    all_files: List[str] = []
+    all_files: list[str] = []
 
     for root, _dirs, files in os.walk(dir):
         root = Path(root)
         rel_root = root.relative_to(dir)
 
         for file in files:
             all_files.append(os.path.join(rel_root / file))
 
     return all_files
 
 
 def copy_file_and_substitute(
-    src: Union[str, Path], dest: Union[str, Path], search_str: str, replace_str: str
+    src: str | Path, dest: str | Path, search_str: str, replace_str: str
 ) -> None:
     with open(src, "r") as fin:
         in_content = fin.read()
         in_content = in_content.replace(search_str, replace_str)
         with open(dest, "w") as fout:
             fout.write(in_content)
 
@@ -95,15 +97,15 @@
 
         shutil.copy2(src, dst, **kwargs)
 
     return copy_fn
 
 
 # Wrapper for TarFile.extractall(), to avoid CVE-2007-4559.
-def tar_safe_extractall(file: Union[str, Path], destdir: Union[str, Path]) -> None:
+def tar_safe_extractall(file: str | Path, destdir: str | Path) -> None:
     import tarfile
 
     destdir = Path(destdir).resolve()
 
     with tarfile.open(file) as tar:
         for member in tar.getmembers():
             member_path = (destdir / member.name).resolve()
```

### Comparing `shinylive-0.0.8/shinylive.egg-info/PKG-INFO` & `shinylive-0.0.9/shinylive.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shinylive
-Version: 0.0.8
+Version: 0.0.9
 Summary: Run Shiny applications running Python in the browser.
 Home-page: https://github.com/rstudio/py-shinylive
 Author: Winston Chang
 Author-email: winston@rstudio.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/rstudio/py-shinylive/issues
 Project-URL: Documentation, https://shiny.rstudio.com/py/docs/shinylive.html
@@ -15,14 +15,16 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: test
+Provides-Extra: dev
 License-File: LICENSE
 
 Shinylive Python package
 ========================
 
 [![Build and test](https://github.com/rstudio/py-shinylive/actions/workflows/build.yml/badge.svg)](https://github.com/rstudio/py-shinylive/actions/)
 [![PyPI Latest Release](https://img.shields.io/pypi/v/shinylive.svg)](https://pypi.org/project/shinylive/)
@@ -53,15 +55,15 @@
 ```
 shinylive export myapp site
 ```
 
 Then you can preview the application by running a web server and visiting it in a browser:
 
 ```
-python3 -m http.server --directory site 8008
+python3 -m http.server --directory site --bind localhost 8008
 ```
 
 At this point, you can deploy the `site/` directory to any static web hosting service.
 
 
 ### Multiple applications
```

