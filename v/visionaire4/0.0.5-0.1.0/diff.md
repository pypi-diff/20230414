# Comparing `tmp/visionaire4-0.0.5.tar.gz` & `tmp/visionaire4-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/visionaire4-0.0.5.tar", last modified: Tue Mar 21 04:18:59 2023, max compression
+gzip compressed data, was "visionaire4-0.1.0.tar", last modified: Fri Apr 14 02:49:58 2023, max compression
```

## Comparing `visionaire4-0.0.5.tar` & `visionaire4-0.1.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 04:18:59.000000 visionaire4-0.0.5/
--rw-r--r--   0 root         (0) root         (0)     4156 2023-03-21 04:18:59.000000 visionaire4-0.0.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      972 2023-03-21 04:18:43.000000 visionaire4-0.0.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 04:18:59.000000 visionaire4-0.0.5/visionaire4/
--rw-rw-rw-   0 root         (0) root         (0)     7751 2023-03-21 04:18:43.000000 visionaire4-0.0.5/visionaire4/export.py
--rw-rw-rw-   0 root         (0) root         (0)    18499 2023-03-21 04:18:43.000000 visionaire4-0.0.5/visionaire4/report.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 04:18:59.000000 visionaire4-0.0.5/visionaire4/configs/
--rw-rw-rw-   0 root         (0) root         (0)     2577 2023-03-21 04:18:43.000000 visionaire4-0.0.5/visionaire4/configs/generator.py
--rw-rw-rw-   0 root         (0) root         (0)     2403 2023-03-21 04:18:43.000000 visionaire4-0.0.5/visionaire4/configs/compose.py
--rw-rw-rw-   0 root         (0) root         (0)      208 2023-03-21 04:18:43.000000 visionaire4-0.0.5/visionaire4/configs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    19133 2023-03-21 04:18:43.000000 visionaire4-0.0.5/visionaire4/configs/hybrid_dashboard.py
--rw-rw-rw-   0 root         (0) root         (0)      498 2023-03-21 04:18:43.000000 visionaire4-0.0.5/visionaire4/configs/configs.py
--rw-rw-rw-   0 root         (0) root         (0)    34434 2023-03-21 04:18:43.000000 visionaire4-0.0.5/visionaire4/configs/resource_dashboard.py
--rw-rw-rw-   0 root         (0) root         (0)    59053 2023-03-21 04:18:43.000000 visionaire4-0.0.5/visionaire4/configs/visionaire4_dashboard.py
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-03-21 04:18:43.000000 visionaire4-0.0.5/visionaire4/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2607 2023-03-21 04:18:43.000000 visionaire4-0.0.5/visionaire4/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     7082 2023-03-21 04:18:43.000000 visionaire4-0.0.5/visionaire4/restore.py
--rw-rw-rw-   0 root         (0) root         (0)     2109 2023-03-21 04:18:43.000000 visionaire4-0.0.5/visionaire4/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-03-21 04:18:43.000000 visionaire4-0.0.5/visionaire4/version.py
--rw-rw-rw-   0 root         (0) root         (0)     3832 2023-03-21 04:18:43.000000 visionaire4-0.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 04:18:59.000000 visionaire4-0.0.5/visionaire4.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4156 2023-03-21 04:18:59.000000 visionaire4-0.0.5/visionaire4.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      643 2023-03-21 04:18:59.000000 visionaire4-0.0.5/visionaire4.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       59 2023-03-21 04:18:59.000000 visionaire4-0.0.5/visionaire4.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-21 04:18:59.000000 visionaire4-0.0.5/visionaire4.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-03-21 04:18:59.000000 visionaire4-0.0.5/visionaire4.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       91 2023-03-21 04:18:59.000000 visionaire4-0.0.5/visionaire4.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-21 04:18:59.000000 visionaire4-0.0.5/setup.cfg
+drwxrwxr-x   0 nodeflux  (1000) nodeflux  (1000)        0 2023-04-14 02:49:58.477730 visionaire4-0.1.0/
+-rw-rw-r--   0 nodeflux  (1000) nodeflux  (1000)     5480 2023-04-14 02:49:58.477730 visionaire4-0.1.0/PKG-INFO
+-rw-rw-r--   0 nodeflux  (1000) nodeflux  (1000)     4129 2023-04-11 07:51:30.000000 visionaire4-0.1.0/README.md
+-rw-rw-r--   0 nodeflux  (1000) nodeflux  (1000)       38 2023-04-14 02:49:58.477730 visionaire4-0.1.0/setup.cfg
+-rw-rw-r--   0 nodeflux  (1000) nodeflux  (1000)      972 2023-03-24 07:33:05.000000 visionaire4-0.1.0/setup.py
+drwxrwxr-x   0 nodeflux  (1000) nodeflux  (1000)        0 2023-04-14 02:49:58.469730 visionaire4-0.1.0/visionaire4/
+-rw-rw-r--   0 nodeflux  (1000) nodeflux  (1000)       33 2023-03-24 07:33:05.000000 visionaire4-0.1.0/visionaire4/__init__.py
+-rw-rw-r--   0 nodeflux  (1000) nodeflux  (1000)     2109 2023-03-24 07:33:05.000000 visionaire4-0.1.0/visionaire4/__main__.py
+drwxrwxr-x   0 nodeflux  (1000) nodeflux  (1000)        0 2023-04-14 02:49:58.473730 visionaire4-0.1.0/visionaire4/configs/
+-rw-rw-r--   0 nodeflux  (1000) nodeflux  (1000)      208 2023-03-24 07:33:05.000000 visionaire4-0.1.0/visionaire4/configs/__init__.py
+-rw-rw-r--   0 nodeflux  (1000) nodeflux  (1000)     2403 2023-03-24 07:33:05.000000 visionaire4-0.1.0/visionaire4/configs/compose.py
+-rw-rw-r--   0 nodeflux  (1000) nodeflux  (1000)      498 2023-03-24 07:33:05.000000 visionaire4-0.1.0/visionaire4/configs/configs.py
+-rw-rw-r--   0 nodeflux  (1000) nodeflux  (1000)     2577 2023-03-24 07:33:05.000000 visionaire4-0.1.0/visionaire4/configs/generator.py
+-rw-rw-r--   0 nodeflux  (1000) nodeflux  (1000)    19133 2023-03-24 07:33:05.000000 visionaire4-0.1.0/visionaire4/configs/hybrid_dashboard.py
+-rw-rw-r--   0 nodeflux  (1000) nodeflux  (1000)    34434 2023-03-24 07:33:05.000000 visionaire4-0.1.0/visionaire4/configs/resource_dashboard.py
+-rw-rw-r--   0 nodeflux  (1000) nodeflux  (1000)    59053 2023-03-24 07:33:05.000000 visionaire4-0.1.0/visionaire4/configs/visionaire4_dashboard.py
+-rw-rw-r--   0 nodeflux  (1000) nodeflux  (1000)     4682 2023-04-13 07:14:30.000000 visionaire4-0.1.0/visionaire4/dataset.py
+-rw-rw-r--   0 nodeflux  (1000) nodeflux  (1000)     7751 2023-03-24 07:33:05.000000 visionaire4-0.1.0/visionaire4/export.py
+-rw-rw-r--   0 nodeflux  (1000) nodeflux  (1000)    18499 2023-03-24 07:33:05.000000 visionaire4-0.1.0/visionaire4/report.py
+-rw-rw-r--   0 nodeflux  (1000) nodeflux  (1000)     7992 2023-04-11 11:33:22.000000 visionaire4-0.1.0/visionaire4/restore.py
+-rw-rw-r--   0 nodeflux  (1000) nodeflux  (1000)     2607 2023-03-24 07:33:05.000000 visionaire4-0.1.0/visionaire4/utils.py
+-rw-rw-r--   0 nodeflux  (1000) nodeflux  (1000)       22 2023-04-11 08:24:59.000000 visionaire4-0.1.0/visionaire4/version.py
+drwxrwxr-x   0 nodeflux  (1000) nodeflux  (1000)        0 2023-04-14 02:49:58.473730 visionaire4-0.1.0/visionaire4.egg-info/
+-rw-rw-r--   0 nodeflux  (1000) nodeflux  (1000)     5480 2023-04-14 02:49:58.000000 visionaire4-0.1.0/visionaire4.egg-info/PKG-INFO
+-rw-rw-r--   0 nodeflux  (1000) nodeflux  (1000)      666 2023-04-14 02:49:58.000000 visionaire4-0.1.0/visionaire4.egg-info/SOURCES.txt
+-rw-rw-r--   0 nodeflux  (1000) nodeflux  (1000)        1 2023-04-14 02:49:58.000000 visionaire4-0.1.0/visionaire4.egg-info/dependency_links.txt
+-rw-rw-r--   0 nodeflux  (1000) nodeflux  (1000)       59 2023-04-14 02:49:58.000000 visionaire4-0.1.0/visionaire4.egg-info/entry_points.txt
+-rw-rw-r--   0 nodeflux  (1000) nodeflux  (1000)      114 2023-04-14 02:49:58.000000 visionaire4-0.1.0/visionaire4.egg-info/requires.txt
+-rw-rw-r--   0 nodeflux  (1000) nodeflux  (1000)       24 2023-04-14 02:49:58.000000 visionaire4-0.1.0/visionaire4.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `visionaire4-0.0.5/PKG-INFO` & `visionaire4-0.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: visionaire4
-Version: 0.0.5
-Summary: Visionaire4 maintenance tools suite
-Home-page: https://pypi.org/project/visionaire4/
-Author: Tri Wahyu Utomo
-Author-email: tri@nodeflux.io
-License: UNKNOWN
-Platform: UNKNOWN
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-
 # VISIONAIRE4
 
 A suite of tools used for Visionaire4 maintenance.  
 Supported function subcommand:
 - `report`: Generate Visionaire4 and FRemisN status report.
 - `export`: Export metrics and edge cases data from current machine to files.
 - `import`: Import metrics and edge cases data from the exported files to current machine.
@@ -96,14 +83,19 @@
 
 This will extract edge case data and separate image data from the label into default config directory `~/nodeflux/import`.  
 You can configure the config directory with:
 ```
 $ visionaire4 import edge -f <path to exported file> --cfg-dir <config directory>
 ```
 
+By default, the data will be dumped as v4 original annotation structure. Optionally, output format can be changed to other common dataset format, i.e. coco (currently only support coco), as:
+```
+$ visionaire4 import edge -f <path to exported file> --cfg-dir <config directory> --out-fmt coco
+```
+
 ### Report
 
 To generate status report for Visionaire4 and or FRemisN, run:
 ```bash
 $ visionaire4 report
 ```
 This will try to locate a running Visionaire4 and or FRemisN, check the system status, and generate a summary for it. 
@@ -129,9 +121,7 @@
 By default the report will also plot the last 5 minutes (300 seconds) of useful metrics from prometheus server, 
 you can specify the time range using:
 ``` bash
 $ visionaire4 report --range <SECONDS>
 # or
 $ visionaire4 report -r <SECONDS>
 ```
-
-
```

### Comparing `visionaire4-0.0.5/setup.py` & `visionaire4-0.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `visionaire4-0.0.5/visionaire4/export.py` & `visionaire4-0.1.0/visionaire4/export.py`

 * *Files identical despite different names*

### Comparing `visionaire4-0.0.5/visionaire4/report.py` & `visionaire4-0.1.0/visionaire4/report.py`

 * *Files identical despite different names*

### Comparing `visionaire4-0.0.5/visionaire4/configs/generator.py` & `visionaire4-0.1.0/visionaire4/configs/generator.py`

 * *Files identical despite different names*

### Comparing `visionaire4-0.0.5/visionaire4/configs/compose.py` & `visionaire4-0.1.0/visionaire4/configs/compose.py`

 * *Files identical despite different names*

### Comparing `visionaire4-0.0.5/visionaire4/configs/hybrid_dashboard.py` & `visionaire4-0.1.0/visionaire4/configs/hybrid_dashboard.py`

 * *Files identical despite different names*

### Comparing `visionaire4-0.0.5/visionaire4/configs/resource_dashboard.py` & `visionaire4-0.1.0/visionaire4/configs/resource_dashboard.py`

 * *Files identical despite different names*

### Comparing `visionaire4-0.0.5/visionaire4/configs/visionaire4_dashboard.py` & `visionaire4-0.1.0/visionaire4/configs/visionaire4_dashboard.py`

 * *Files identical despite different names*

### Comparing `visionaire4-0.0.5/visionaire4/utils.py` & `visionaire4-0.1.0/visionaire4/utils.py`

 * *Files identical despite different names*

### Comparing `visionaire4-0.0.5/visionaire4/restore.py` & `visionaire4-0.1.0/visionaire4/restore.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import argparse
 import logging
 import tarfile
 import shutil
-import base64
 import json
 import os
 
+from tqdm import tqdm
 from pathlib import Path, PosixPath
 from datetime import datetime, timezone
 
 from visionaire4 import configs
+from visionaire4.dataset import V4, COCO
 
+DATASET_FORMAT = ["v4", "coco"]
 IMPORT_TYPE = ["metrics", "edge"]
 logger = logging.getLogger()
 
 
 def extract_tar(filepath: str, out_dir: str) -> str:
     out_dir: PosixPath = Path(out_dir).expanduser().resolve()
     out_dir.mkdir(parents=True, exist_ok=True)
@@ -108,62 +110,75 @@
         f"or by running '{cmd_msg}'"
     )
     logger.info(
         "Monitoring servers available at http://localhost:3000 with user 'admin' and password 'admin'"
     )
 
 
-def process_edgecase_data(fpath: str, out_dir: str):
-    fpath: PosixPath = Path(fpath)
-    if fpath.suffix != ".json":
-        logger.warn(f"exported file {fpath} is not a json file, skipping")
+def process_edgecase_data(target_dir: PosixPath, input_json: PosixPath, out_fmt):
+    if input_json.suffix != ".json":
+        logger.warn(f"exported file {input_json} is not a json file, skipping")
         return
 
-    with fpath.open("r") as f:
+    content = {}
+    with input_json.open("r") as f:
         content = json.load(f)
 
-    out_dir: PosixPath = Path(out_dir)
-    out_dir.mkdir(parents=True, exist_ok=True)
-
-    labelpath = out_dir.joinpath(fpath.name)
-    with labelpath.open("w") as f:
-        json.dump(content["additional_params"], f)
-
-    img_path = out_dir.joinpath(f"{fpath.stem}.jpeg")
-    img_data = base64.b64decode(
-        content["images"][0].replace("data:image/jpeg;base64,", "")
-    )
-    with img_path.open("wb") as f:
-        f.write(img_data)
+    if content:
+        out_fmt.dump(target_dir, input_json, content)
+    else:
+        logger.warn(f"exported file {input_json} contains invalid json, skipping")
 
 
 def import_edgecase(args):
     cfg_dir: PosixPath = Path(args.cfg_dir).expanduser().resolve()
     if cfg_dir.is_file():
         raise RuntimeError(
             f"Config directory (--cfg-dir) '{args.cfg_dir}' is file, "
             "expected to be a directory."
         )
     cfg_dir.mkdir(parents=True, exist_ok=True)
 
-    dump_dir = cfg_dir.joinpath("edgecase")
-    logger.debug(f"Extracting exported data {args.file} to {dump_dir}")
-    extract_tar(args.file, dump_dir)
-    extracted = dump_dir.joinpath("dump")
+    target_dir = cfg_dir.joinpath("edgecase")
+    logger.debug(f"Extracting exported data {args.file} to {target_dir}")
+    extract_tar(args.file, target_dir)
+    tmp_dump_dir = target_dir.joinpath("dump")
+
+    if args.out_fmt.lower() == "COCO".lower():
+        logger.info(f"Importing data as coco dataset format.")
+        out_fmt = COCO()
+    else:
+        logger.info(f"Importing data as original Visionaire4 format.")
+        out_fmt = V4()
+
+    # calculate total files to estimate time of works
+    num_of_files = sum([len(files) for r, d, files in os.walk(tmp_dump_dir)])
+    prog_bar = tqdm(total=num_of_files + 1)
 
-    for d in extracted.iterdir():
+    for d in tmp_dump_dir.iterdir():
         if d.is_file():
             continue
-        out_dir = dump_dir.joinpath(d.name)
         for f in d.iterdir():
             if not f.is_file():
                 continue
-            process_edgecase_data(f, out_dir)
-    shutil.rmtree(extracted)
-    logger.info(f"Successfully imported edge case data to {dump_dir}")
+            process_edgecase_data(target_dir, f, out_fmt)
+            prog_bar.update(1)
+
+    if args.out_fmt.lower() == "COCO".lower():
+        out_dir = target_dir.joinpath("annotations")
+        out_dir.mkdir(parents=True, exist_ok=True)
+        labelpath = out_dir.joinpath("instances_default.json")
+        with labelpath.open("w") as f:
+            del out_fmt.labels
+            f.write(out_fmt.toJSON())
+
+    shutil.rmtree(tmp_dump_dir)
+    prog_bar.update(1)  # set to 100% for the last
+    prog_bar.close()
+    logger.info(f"Successfully imported edge case data to {target_dir}")
 
 
 def main(args):
     msg_type = "edge cases" if args.type == "edge" else args.type
     logger.info(f"Start importing Visionaire4 {msg_type} data.")
 
     if args.file == "":
@@ -192,14 +207,23 @@
         "type",
         type=str,
         metavar="TYPE",
         help="type of data to import, choice: [{}]".format(", ".join(IMPORT_TYPE)),
         choices=IMPORT_TYPE,
     )
     parser.add_argument(
+        "--out-fmt",
+        "-o",
+        type=str,
+        metavar="FORMAT",
+        help="output dataset format, choice: [{}]".format(", ".join(DATASET_FORMAT)),
+        choices=DATASET_FORMAT,
+        default="v4",
+    )
+    parser.add_argument(
         "--file",
         "-f",
         type=str,
         default="",
         help="Path to exported file to be imported.",
     )
     parser.add_argument("--down", action="store_true", help="stop docker compose")
```

### Comparing `visionaire4-0.0.5/visionaire4/__main__.py` & `visionaire4-0.1.0/visionaire4/__main__.py`

 * *Files identical despite different names*

### Comparing `visionaire4-0.0.5/visionaire4.egg-info/SOURCES.txt` & `visionaire4-0.1.0/visionaire4.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 README.md
 setup.py
 visionaire4/__init__.py
 visionaire4/__main__.py
+visionaire4/dataset.py
 visionaire4/export.py
 visionaire4/report.py
 visionaire4/restore.py
 visionaire4/utils.py
 visionaire4/version.py
 visionaire4.egg-info/PKG-INFO
 visionaire4.egg-info/SOURCES.txt
```

