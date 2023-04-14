# Comparing `tmp/wop-2.2.1.tar.gz` & `tmp/wop-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\rlafage\workspace\WhatsOpt-CLI\dist\.tmp-irsvq2j5\wop-2.2.1.tar", last modified: Mon Mar 20 14:43:42 2023, max compression
+gzip compressed data, was "dist\wop-2.3.0.tar", last modified: Fri Apr 14 19:20:23 2023, max compression
```

## Comparing `wop-2.2.1.tar` & `wop-2.3.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-03-20 14:43:42.057626 wop-2.2.1/
--rw-rw-rw-   0        0        0    11558 2019-10-20 20:51:42.000000 wop-2.2.1/LICENSE
--rw-rw-rw-   0        0        0      851 2023-03-20 14:43:42.057626 wop-2.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1786 2021-05-16 20:10:24.000000 wop-2.2.1/README.md
--rw-rw-rw-   0        0        0       42 2023-03-20 14:43:42.057626 wop-2.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1421 2022-08-17 14:04:44.000000 wop-2.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-20 14:43:41.995747 wop-2.2.1/tests/
--rw-rw-rw-   0        0        0      517 2023-03-20 14:35:21.000000 wop-2.2.1/tests/test_convert_utils.py
--rw-rw-rw-   0        0        0      476 2022-06-10 09:28:53.000000 wop-2.2.1/tests/test_mooptimization.py
--rw-rw-rw-   0        0        0     2170 2023-03-20 14:35:21.000000 wop-2.2.1/tests/test_push_command.py
--rw-rw-rw-   0        0        0     2960 2023-03-20 14:35:21.000000 wop-2.2.1/tests/test_push_utils.py
--rw-rw-rw-   0        0        0     3452 2023-03-20 14:35:21.000000 wop-2.2.1/tests/test_upload_utils.py
--rw-rw-rw-   0        0        0     3872 2023-03-20 14:35:21.000000 wop-2.2.1/tests/test_utils.py
--rw-rw-rw-   0        0        0      350 2022-02-21 15:06:38.000000 wop-2.2.1/tests/test_whatsopt_client.py
--rw-rw-rw-   0        0        0     2108 2023-03-20 14:35:21.000000 wop-2.2.1/tests/test_wop.py
-drwxrwxrwx   0        0        0        0 2023-03-20 14:43:42.026993 wop-2.2.1/whatsopt/
--rw-rw-rw-   0        0        0       23 2023-03-20 14:38:37.000000 wop-2.2.1/whatsopt/__init__.py
--rw-rw-rw-   0        0        0     1493 2021-10-07 14:47:53.000000 wop-2.2.1/whatsopt/convert_utils.py
--rw-rw-rw-   0        0        0      502 2022-06-02 07:27:07.000000 wop-2.2.1/whatsopt/logging.py
--rw-rw-rw-   0        0        0     3186 2022-06-10 09:28:53.000000 wop-2.2.1/whatsopt/mooptimization.py
--rw-rw-rw-   0        0        0    11578 2023-03-20 14:35:21.000000 wop-2.2.1/whatsopt/optimization.py
--rw-rw-rw-   0        0        0    15185 2023-03-20 14:35:21.000000 wop-2.2.1/whatsopt/push_command.py
--rw-rw-rw-   0        0        0     5644 2023-03-19 12:20:40.000000 wop-2.2.1/whatsopt/push_utils.py
--rw-rw-rw-   0        0        0     1483 2021-06-21 11:38:00.000000 wop-2.2.1/whatsopt/show_utils.py
--rw-rw-rw-   0        0        0     7448 2022-06-29 16:15:18.000000 wop-2.2.1/whatsopt/upload_utils.py
--rw-rw-rw-   0        0        0     5616 2022-08-17 12:43:17.000000 wop-2.2.1/whatsopt/utils.py
--rw-rw-rw-   0        0        0    33598 2023-03-20 14:35:21.000000 wop-2.2.1/whatsopt/whatsopt_client.py
--rw-rw-rw-   0        0        0    11424 2022-06-29 16:21:30.000000 wop-2.2.1/whatsopt/wop.py
-drwxrwxrwx   0        0        0        0 2023-03-20 14:43:42.057626 wop-2.2.1/wop.egg-info/
--rw-rw-rw-   0        0        0      851 2023-03-20 14:43:41.000000 wop-2.2.1/wop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      693 2023-03-20 14:43:41.000000 wop-2.2.1/wop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-20 14:43:41.000000 wop-2.2.1/wop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-03-20 14:43:41.000000 wop-2.2.1/wop.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      107 2023-03-20 14:43:41.000000 wop-2.2.1/wop.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-20 14:43:41.000000 wop-2.2.1/wop.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2019-12-02 13:07:07.000000 wop-2.2.1/wop.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-04-14 19:20:23.101657 wop-2.3.0/
+-rw-rw-rw-   0        0        0    11558 2019-10-20 20:51:42.000000 wop-2.3.0/LICENSE
+-rw-rw-rw-   0        0        0      851 2023-04-14 19:20:23.101657 wop-2.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1786 2021-05-16 20:10:24.000000 wop-2.3.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-14 19:20:23.101657 wop-2.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1481 2023-04-14 19:05:22.000000 wop-2.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 19:20:23.039125 wop-2.3.0/tests/
+-rw-rw-rw-   0        0        0      517 2023-03-20 14:35:21.000000 wop-2.3.0/tests/test_convert_utils.py
+-rw-rw-rw-   0        0        0      476 2022-06-10 09:28:53.000000 wop-2.3.0/tests/test_mooptimization.py
+-rw-rw-rw-   0        0        0     2170 2023-03-20 14:35:21.000000 wop-2.3.0/tests/test_push_command.py
+-rw-rw-rw-   0        0        0     2960 2023-03-20 14:35:21.000000 wop-2.3.0/tests/test_push_utils.py
+-rw-rw-rw-   0        0        0     3452 2023-03-20 14:35:21.000000 wop-2.3.0/tests/test_upload_utils.py
+-rw-rw-rw-   0        0        0     3872 2023-03-20 14:35:21.000000 wop-2.3.0/tests/test_utils.py
+-rw-rw-rw-   0        0        0      350 2022-02-21 15:06:38.000000 wop-2.3.0/tests/test_whatsopt_client.py
+-rw-rw-rw-   0        0        0     2108 2023-03-20 14:35:21.000000 wop-2.3.0/tests/test_wop.py
+drwxrwxrwx   0        0        0        0 2023-04-14 19:20:23.086006 wop-2.3.0/whatsopt/
+-rw-rw-rw-   0        0        0       23 2023-04-12 16:39:47.000000 wop-2.3.0/whatsopt/__init__.py
+-rw-rw-rw-   0        0        0     1493 2021-10-07 14:47:53.000000 wop-2.3.0/whatsopt/convert_utils.py
+-rw-rw-rw-   0        0        0      502 2022-06-02 07:27:07.000000 wop-2.3.0/whatsopt/logging.py
+-rw-rw-rw-   0        0        0     3186 2022-06-10 09:28:53.000000 wop-2.3.0/whatsopt/mooptimization.py
+-rw-rw-rw-   0        0        0    11578 2023-03-20 14:35:21.000000 wop-2.3.0/whatsopt/optimization.py
+-rw-rw-rw-   0        0        0      232 2023-04-12 16:39:47.000000 wop-2.3.0/whatsopt/publish_utils.py
+-rw-rw-rw-   0        0        0    15185 2023-03-20 14:35:21.000000 wop-2.3.0/whatsopt/push_command.py
+-rw-rw-rw-   0        0        0     5644 2023-03-19 12:20:40.000000 wop-2.3.0/whatsopt/push_utils.py
+-rw-rw-rw-   0        0        0     1483 2021-06-21 11:38:00.000000 wop-2.3.0/whatsopt/show_utils.py
+-rw-rw-rw-   0        0        0     7448 2022-06-29 16:15:18.000000 wop-2.3.0/whatsopt/upload_utils.py
+-rw-rw-rw-   0        0        0     5616 2023-04-07 15:50:56.000000 wop-2.3.0/whatsopt/utils.py
+-rw-rw-rw-   0        0        0    36682 2023-04-14 19:05:22.000000 wop-2.3.0/whatsopt/whatsopt_client.py
+-rw-rw-rw-   0        0        0    11955 2023-04-14 19:05:22.000000 wop-2.3.0/whatsopt/wop.py
+drwxrwxrwx   0        0        0        0 2023-04-14 19:20:23.101657 wop-2.3.0/wop.egg-info/
+-rw-rw-rw-   0        0        0      851 2023-04-14 19:20:22.000000 wop-2.3.0/wop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      719 2023-04-14 19:20:22.000000 wop-2.3.0/wop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 19:20:22.000000 wop-2.3.0/wop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-04-14 19:20:22.000000 wop-2.3.0/wop.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      131 2023-04-14 19:20:22.000000 wop-2.3.0/wop.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-14 19:20:22.000000 wop-2.3.0/wop.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2019-12-02 13:07:07.000000 wop-2.3.0/wop.egg-info/zip-safe
```

### Comparing `wop-2.2.1/LICENSE` & `wop-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wop-2.2.1/PKG-INFO` & `wop-2.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wop
-Version: 2.2.1
+Version: 2.3.0
 Summary: WhatsOpt web application command line client
 Home-page: https://github.com/OneraHub/WhatsOpt-CLI
 Download-URL: https://github.com/OneraHub/WhatsOpt-CLI/releases
 Author: Rémi Lafage
 Author-email: remi.lafage@onera.fr
 License: Apache License, Version 2.0
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `wop-2.2.1/README.md` & `wop-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `wop-2.2.1/setup.py` & `wop-2.3.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,22 +26,25 @@
     description="WhatsOpt web application command line client",
     author="Rémi Lafage",
     author_email="remi.lafage@onera.fr",
     license="Apache License, Version 2.0",
     classifiers=[_f for _f in CLASSIFIERS.split("\n") if _f],
     packages=["whatsopt"],
     install_requires=[
+        "build",
+        "click>=6.7",
         "openmdao>=3.4.0",
-        "openmdao_extensions>=1.1.0",
-        "xdsmjs>=1.0.0",
-        "Click>=6.7",
-        "tabulate>=0.8.2",
+        "openmdao_extensions>=1.2.0",
+        "packaging",
+        "pkginfo",
         "requests",
+        "tabulate>=0.8.2",
         "tomli",
         "tomli-w",
+        "xdsmjs>=1.0.0",
     ],
     python_requires=">=3.7",
     entry_points="""
         [console_scripts]
         wop=whatsopt.wop:wop
     """,
     zip_safe=True,
```

### Comparing `wop-2.2.1/tests/test_convert_utils.py` & `wop-2.3.0/tests/test_convert_utils.py`

 * *Files identical despite different names*

### Comparing `wop-2.2.1/tests/test_push_command.py` & `wop-2.3.0/tests/test_push_command.py`

 * *Files identical despite different names*

### Comparing `wop-2.2.1/tests/test_push_utils.py` & `wop-2.3.0/tests/test_push_utils.py`

 * *Files identical despite different names*

### Comparing `wop-2.2.1/tests/test_upload_utils.py` & `wop-2.3.0/tests/test_upload_utils.py`

 * *Files identical despite different names*

### Comparing `wop-2.2.1/tests/test_utils.py` & `wop-2.3.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `wop-2.2.1/tests/test_wop.py` & `wop-2.3.0/tests/test_wop.py`

 * *Files identical despite different names*

### Comparing `wop-2.2.1/whatsopt/convert_utils.py` & `wop-2.3.0/whatsopt/convert_utils.py`

 * *Files identical despite different names*

### Comparing `wop-2.2.1/whatsopt/mooptimization.py` & `wop-2.3.0/whatsopt/mooptimization.py`

 * *Files identical despite different names*

### Comparing `wop-2.2.1/whatsopt/optimization.py` & `wop-2.3.0/whatsopt/optimization.py`

 * *Files identical despite different names*

### Comparing `wop-2.2.1/whatsopt/push_command.py` & `wop-2.3.0/whatsopt/push_command.py`

 * *Files identical despite different names*

### Comparing `wop-2.2.1/whatsopt/push_utils.py` & `wop-2.3.0/whatsopt/push_utils.py`

 * *Files identical despite different names*

### Comparing `wop-2.2.1/whatsopt/show_utils.py` & `wop-2.3.0/whatsopt/show_utils.py`

 * *Files identical despite different names*

### Comparing `wop-2.2.1/whatsopt/upload_utils.py` & `wop-2.3.0/whatsopt/upload_utils.py`

 * *Files identical despite different names*

### Comparing `wop-2.2.1/whatsopt/utils.py` & `wop-2.3.0/whatsopt/utils.py`

 * *Files identical despite different names*

### Comparing `wop-2.2.1/whatsopt/whatsopt_client.py` & `wop-2.3.0/whatsopt/whatsopt_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from http import HTTPStatus
 from shutil import move
 import os
 import sys
 import json
 import getpass
 import requests
 import copy
@@ -10,24 +11,26 @@
 import tempfile
 import numpy as np
 import time
 import tomli
 import tomli_w
 from tabulate import tabulate
 from urllib.parse import urlparse
+from packaging.version import Version
 
 # push
 import openmdao.utils.hooks as hooks
 from openmdao.utils.file_utils import _load_and_exec
 
 from openmdao.utils.webview import webview
 from openmdao.api import IndepVarComp
 from whatsopt.convert_utils import convert_sqlite_to_csv
 
 from whatsopt.logging import log, info, warn, error, debug
+from whatsopt.publish_utils import build_package, get_pkg_metadata
 from whatsopt.utils import (
     FRAMEWORK_GEMSEO,
     FRAMEWORK_OPENMDAO,
     MODE_PACKAGE,
     MODE_PLAIN,
     extract_remote_name,
     is_analysis_user_file,
@@ -630,17 +633,17 @@
             error("Please choose either --openmdao or --gemseo.")
             sys.exit(-1)
         opts.update(
             {
                 "--base": True,
                 "--update": True,
                 "--gemseo": opts["--gemseo"]
-                or (not opts["--openmdao"] and is_based_on("gemseo")),
+                or (not opts["--openmdao"] and is_based_on(FRAMEWORK_GEMSEO)),
                 "--openmdao": opts["--openmdao"]
-                or (not opts["--gemseo"] and is_based_on("openmdao")),
+                or (not opts["--gemseo"] and is_based_on(FRAMEWORK_OPENMDAO)),
                 "--package": is_package_mode(),
             }
         )
         self.pull_mda(mda_id, opts, "Analysis #{} updated".format(mda_id))
 
     def show_mda(self, analysis_id, pbfile, name, outfile, batch, depth):
         options = {
@@ -862,14 +865,89 @@
         if not (extension == ".sqlite" or re.match(r"\.sqlite_\d+$", extension)):
             warn(
                 f"File {filename} should have '.sqlite[_n]' extension, got '{extension}'"
             )
         basename = os.path.basename(pathname)
         convert_sqlite_to_csv(filename, basename)
 
+    def publish(self, force=False, analysis_id=None):
+        mda_id = analysis_id if analysis_id else get_analysis_id()
+        url = self.endpoint(f"/api/v1/analyses/{mda_id}/package")
+        if not force:
+            resp = self.session.get(url, headers=self.headers)
+            if resp.ok:
+                existing_meta = resp.json()
+            elif resp.status_code == HTTPStatus.NOT_FOUND:
+                existing_meta = None
+            else:
+                resp.raise_for_status()
+
+            if existing_meta:
+                warn(
+                    f"Existing package {existing_meta['name']} {existing_meta['version']} will be lost."
+                )
+                answer = input("Do you want to continue? (yes/no): ")
+                if answer.lower() == "yes":
+                    pass
+                else:
+                    info("Publishing aborted")
+                    exit(-1)
+
+        info("Package building...")
+        filename = self.build()
+        if not os.path.exists(filename):
+            error(f"File {filename} not found")
+            exit(-1)
+        meta = get_pkg_metadata(filename)
+        if (
+            not force
+            and existing_meta
+            and existing_meta["name"] == meta.name
+            and Version(existing_meta["version"]) >= Version(meta.version)
+        ):
+            error(f"You have to bump the version (> {existing_meta['version']})")
+            error("Publishing aborted")
+            exit(-1)
+
+        files = {
+            "package[description]": (None, meta.summary, "application/json"),
+            "package[archive]": (filename, open(filename, "rb"), "application/gzip"),
+        }
+        info("Package publishing...")
+        resp = self.session.post(url, headers=self.headers, files=files)
+        if resp.ok:
+            info(
+                f"Package {meta.name} v{meta.version} is published on WopStore({self.endpoint('/packages')})"
+            )
+        elif resp.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
+            error(resp.json()["message"])
+            error("Duplicate detected! The package already exists on WopStore!")
+            exit(-1)
+        else:
+            resp.raise_for_status()
+
+    def build(self, analysis_id=None):
+        if not is_package_mode():
+            error("Package mode is required!")
+            exit(-1)
+        update_options = {
+            "--dry-run": False,
+            "--force": False,
+            "--server": False,
+            "--egmdo": False,
+            "--run-ops": False,
+            "--test-units": False,
+            "--gemseo": is_based_on(FRAMEWORK_GEMSEO),
+            "--openmdao": is_based_on(FRAMEWORK_OPENMDAO),
+        }
+        mda_id = analysis_id if analysis_id else get_analysis_id()
+        self.update_mda(mda_id, update_options)
+        filename = build_package()
+        return filename
+
     def _test_connection(self):
         if self.api_key:
             self.headers = {
                 "Authorization": "Token token=" + self.api_key,
                 "User-Agent": "wop/{}".format(__version__),
             }
             url = self.endpoint("/api/v1/versioning")
```

### Comparing `wop-2.2.1/whatsopt/wop.py` & `wop-2.3.0/whatsopt/wop.py`

 * *Files 6% similar despite different names*

```diff
@@ -442,9 +442,30 @@
 def convert(
     sqlite_filename,
 ):
     """Convert given sqlite file from OpenMDAO to csv file format."""
     WhatsOpt().convert(sqlite_filename)
 
 
+@wop.command()
+@click.option(
+    "-f",
+    "--force",
+    is_flag=True,
+    default=False,
+    help="overwrite current published package anyway",
+)
+@click.pass_context
+def publish(ctx, force):
+    """Publish current analysis as Python package on WhatsOpt Package Store. Package mode is required."""
+    WhatsOpt(**ctx.obj).login().publish(force)
+
+
+@wop.command()
+@click.pass_context
+def build(ctx):
+    """Build current analysis package. Package mode is required."""
+    WhatsOpt(**ctx.obj).login().build()
+
+
 if __name__ == "__main__":
     wop()
```

### Comparing `wop-2.2.1/wop.egg-info/PKG-INFO` & `wop-2.3.0/wop.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wop
-Version: 2.2.1
+Version: 2.3.0
 Summary: WhatsOpt web application command line client
 Home-page: https://github.com/OneraHub/WhatsOpt-CLI
 Download-URL: https://github.com/OneraHub/WhatsOpt-CLI/releases
 Author: Rémi Lafage
 Author-email: remi.lafage@onera.fr
 License: Apache License, Version 2.0
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `wop-2.2.1/wop.egg-info/SOURCES.txt` & `wop-2.3.0/wop.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 tests/test_whatsopt_client.py
 tests/test_wop.py
 whatsopt/__init__.py
 whatsopt/convert_utils.py
 whatsopt/logging.py
 whatsopt/mooptimization.py
 whatsopt/optimization.py
+whatsopt/publish_utils.py
 whatsopt/push_command.py
 whatsopt/push_utils.py
 whatsopt/show_utils.py
 whatsopt/upload_utils.py
 whatsopt/utils.py
 whatsopt/whatsopt_client.py
 whatsopt/wop.py
```

