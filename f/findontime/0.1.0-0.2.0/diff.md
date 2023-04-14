# Comparing `tmp/findontime-0.1.0.tar.gz` & `tmp/findontime-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findontime-0.1.0.tar", max compression
+gzip compressed data, was "findontime-0.2.0.tar", max compression
```

## Comparing `findontime-0.1.0.tar` & `findontime-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    31904 2023-04-09 11:15:18.037313 findontime-0.1.0/LICENSE
--rw-r--r--   0        0        0     6174 2023-04-13 11:02:56.335133 findontime-0.1.0/README.md
--rw-r--r--   0        0        0      839 2023-04-13 11:16:18.412351 findontime-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       24 2023-04-11 13:13:09.220772 findontime-0.1.0/src/findontime/__init__.py
--rw-r--r--   0        0        0      315 2023-04-11 13:32:03.758472 findontime-0.1.0/src/findontime/__main__.py
--rw-r--r--   0        0        0     1997 2023-04-13 10:13:25.550855 findontime-0.1.0/src/findontime/configs.py
--rw-r--r--   0        0        0     8736 2023-04-11 13:01:20.270281 findontime-0.1.0/src/findontime/connectors.py
--rw-r--r--   0        0        0     3646 2023-04-11 13:01:20.270281 findontime-0.1.0/src/findontime/drones.py
--rw-r--r--   0        0        0    14936 2023-04-11 13:01:20.270281 findontime-0.1.0/src/findontime/insaflu_uploads.py
--rw-r--r--   0        0        0     7475 2023-04-13 10:12:55.627104 findontime-0.1.0/src/findontime/manager.py
--rw-r--r--   0        0        0     4822 2023-04-11 13:01:20.270281 findontime-0.1.0/src/findontime/plot_utils.py
--rw-r--r--   0        0        0     9902 2023-04-09 11:12:06.161507 findontime-0.1.0/src/findontime/plotting_from_all_reports.py
--rw-r--r--   0        0        0     3447 2023-04-11 13:01:20.270281 findontime-0.1.0/src/findontime/records.py
--rw-r--r--   0        0        0     3444 2023-04-11 13:01:20.270281 findontime-0.1.0/src/findontime/tables_post.py
--rw-r--r--   0        0        0    21536 2023-04-11 13:01:20.270281 findontime-0.1.0/src/findontime/upload_utils.py
--rw-r--r--   0        0        0     7326 2023-04-13 11:16:20.665020 findontime-0.1.0/setup.py
--rw-r--r--   0        0        0     6973 2023-04-13 11:16:20.665587 findontime-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    31904 2023-04-09 11:15:18.037313 findontime-0.2.0/LICENSE
+-rw-r--r--   0        0        0    11060 2023-04-14 12:51:03.222693 findontime-0.2.0/README.md
+-rw-r--r--   0        0        0      875 2023-04-14 12:55:02.990727 findontime-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       24 2023-04-11 13:13:09.220772 findontime-0.2.0/src/findontime/__init__.py
+-rw-r--r--   0        0        0      315 2023-04-13 15:22:43.482616 findontime-0.2.0/src/findontime/__main__.py
+-rw-r--r--   0        0        0     1997 2023-04-13 10:13:25.550855 findontime-0.2.0/src/findontime/configs.py
+-rw-r--r--   0        0        0     9288 2023-04-13 13:28:27.639194 findontime-0.2.0/src/findontime/connectors.py
+-rw-r--r--   0        0        0     3646 2023-04-11 13:01:20.270281 findontime-0.2.0/src/findontime/drones.py
+-rw-r--r--   0        0        0    14936 2023-04-11 13:01:20.270281 findontime-0.2.0/src/findontime/insaflu_uploads.py
+-rw-r--r--   0        0        0     9302 2023-04-13 14:13:56.590072 findontime-0.2.0/src/findontime/manager.py
+-rw-r--r--   0        0        0     4822 2023-04-11 13:01:20.270281 findontime-0.2.0/src/findontime/plot_utils.py
+-rw-r--r--   0        0        0     9902 2023-04-09 11:12:06.161507 findontime-0.2.0/src/findontime/plotting_from_all_reports.py
+-rw-r--r--   0        0        0     3447 2023-04-11 13:01:20.270281 findontime-0.2.0/src/findontime/records.py
+-rw-r--r--   0        0        0     3444 2023-04-11 13:01:20.270281 findontime-0.2.0/src/findontime/tables_post.py
+-rw-r--r--   0        0        0    21536 2023-04-13 13:27:24.031739 findontime-0.2.0/src/findontime/upload_utils.py
+-rw-r--r--   0        0        0    12293 2023-04-14 12:55:33.681719 findontime-0.2.0/setup.py
+-rw-r--r--   0        0        0    11964 2023-04-14 12:55:33.682532 findontime-0.2.0/PKG-INFO
```

### Comparing `findontime-0.1.0/LICENSE` & `findontime-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `findontime-0.1.0/pyproject.toml` & `findontime-0.2.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 [tool.poetry]
 name = "findontime"
-version = "0.1.0"
+version = "0.2.0"
 description = "A tool to upload Fastq files to the INSaFLU database and perform metagenomics pathogen detection"
 authors = ["SantosJGND <dourado.jns@gmail.com>", "insapathogenomics <insapathogenomics@insa.min-saude.pt>"]
 readme = "README.md"
+license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 xopen = "1.7.0"
 dash-bootstrap-components = "1.4.1"
 dataclasses = "0.6"
 natsort = "8.3.1"
 seaborn = "0.12.2"
 Twisted = "16.7.0rc2"
 sqlalchemy = "1.4.23"
 fastq-handler = "^0.2.0"
+paramiko = "^3.1.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.2"
 mock-ssh-server = "0.9.1"
 pytest-cov = "4.0.0"
 
 [build-system]
```

### Comparing `findontime-0.1.0/src/findontime/configs.py` & `findontime-0.2.0/src/findontime/configs.py`

 * *Files identical despite different names*

### Comparing `findontime-0.1.0/src/findontime/connectors.py` & `findontime-0.2.0/src/findontime/connectors.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,41 @@
         pass
 
     @abstractmethod
     def __exit__(self, exc_type, exc_val, exc_tb):
         pass
 
 
+class ConnectorNull(Connector):
+
+    def __init__(self):
+        super().__init__()
+
+    def test_connection(self) -> None:
+        pass
+
+    def execute_command(self, command: str) -> str:
+        return ""
+
+    def check_file_exists(self, file_path: str) -> bool:
+        return False
+
+    def upload_file(self, file_path: str, remote_path: str):
+        pass
+
+    def download_file(self, file_path: str, remote_path: str):
+        pass
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        pass
+
+
 class ConnectorParamiko(Connector):
 
     def __init__(self, config_file: str) -> None:
         super().__init__()
         self.prep_input(config_file)
         self.connect()
```

### Comparing `findontime-0.1.0/src/findontime/drones.py` & `findontime-0.2.0/src/findontime/drones.py`

 * *Files identical despite different names*

### Comparing `findontime-0.1.0/src/findontime/insaflu_uploads.py` & `findontime-0.2.0/src/findontime/insaflu_uploads.py`

 * *Files identical despite different names*

### Comparing `findontime-0.1.0/src/findontime/manager.py` & `findontime-0.2.0/src/findontime/manager.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,74 @@
 
+from typing import Protocol
 import argparse
 import os
 import signal
 import sys
 import time
 from dataclasses import dataclass
 from typing import Tuple
 
+from fastq_handler.fastq_handler import PreMain
 from fastq_handler.actions import ProcessActionMergeWithLast, ProcessActionDownsize
+from fastq_handler.configs import RunConfig
 from findontime.configs import InfluConfig
 from findontime.connectors import ConnectorDocker, ConnectorParamiko
 from findontime.drones import (InsafluFileProcessThread, LockWithOwner,
                                TelevirFileProcessThread, signal_handler)
 from findontime.insaflu_uploads import (InfluConfig, InsafluFileProcess,
                                         TelevirFileProcess)
-from findontime.upload_utils import InsafluUploadRemote, UploadAll, UploadLast
+from findontime.upload_utils import InsafluUploadRemote, UploadAll, UploadLast, UploadNone
+
+
+def get_arguments():
+
+    parser = argparse.ArgumentParser(description="Process fastq files.")
+    parser.add_argument(
+        "-i", "--in_dir", help="Input directory", required=True)
+    parser.add_argument("-o", "--out_dir",
+                        help="Output directory", required=True)
+    parser.add_argument("-s", "--sleep", help="Sleep time between checks in monitor mode", default=600,
+                        type=int)
+
+    parser.add_argument("-n", "--tag", help="name tag, if given, will be added to the output file names",
+                        required=False, type=str, default="")
+
+    parser.add_argument("--config", help="config file",
+                        required=False, type=str, default="config.ini")
+
+    parser.add_argument(
+        "--max_size", help="max size of the output file, in kilobytes", type=int, default=400000)
+
+    parser.add_argument("--merge", help="merge files", action="store_true")
+
+    parser.add_argument(
+        "--downsize", help="downsize fastq files", action="store_true")
+
+    parser.add_argument('--upload',
+                        default='last',
+                        choices=['last', 'all', 'none'],
+                        help='file upload stategy (default: last)',)
+
+    parser.add_argument('--connect',
+                        default='docker',
+                        choices=['docker', 'ssh'],
+                        help='file upload stategy (default: docker)',)
+
+    parser.add_argument(
+        "--keep_names", help="keep original file names", action="store_true")
+
+    parser.add_argument(
+        "--monitor", help="monitor directory until killed", action="store_true")
+
+    parser.add_argument(
+        "--televir", help="deploy televir pathogen identification on each sample", action="store_true"
+    )
+
+    return ArgsClass(**parser.parse_args().__dict__)
 
 
 @dataclass
 class ArgsClass:
 
     in_dir: str
     out_dir: str
@@ -42,59 +92,92 @@
 
 
 class MainInsaflu:
 
     def __init__(self):
         pass
 
-    def get_arguments(self):
+    def select_manager(self, args: ArgsClass):
 
-        parser = argparse.ArgumentParser(description="Process fastq files.")
-        parser.add_argument(
-            "-i", "--in_dir", help="Input directory", required=True)
-        parser.add_argument("-o", "--out_dir",
-                            help="Output directory", required=True)
-        parser.add_argument("-s", "--sleep", help="Sleep time between checks in monitor mode", default=600,
-                            type=int)
+        if args.upload == 'none':
+            print("No upload specified, using fastq handler")
+            return FastqHandlerManager(args)
+        else:
+            return InsafluManager(args)
 
-        parser.add_argument("-n", "--tag", help="name tag, if given, will be added to the output file names",
-                            required=False, type=str, default="")
+    def run(self):
+        args = get_arguments()
+        manager = self.select_manager(args)
+        manager.run()
 
-        parser.add_argument("--config", help="config file",
-                            required=False, type=str, default="config.ini")
 
-        parser.add_argument(
-            "--max_size", help="max size of the output file, in kilobytes", type=int, default=400000)
+class Deployer(Protocol):
 
-        parser.add_argument("--merge", help="merge files", action="store_true")
+    def __init__(self, args: ArgsClass) -> None:
+        ...
 
-        parser.add_argument(
-            "--downsize", help="downsize fastq files", action="store_true")
+    def run(self) -> None:
+        ...
 
-        parser.add_argument('--upload',
-                            default='last',
-                            choices=['last', 'all'],
-                            help='file upload stategy (default: all)',)
 
-        parser.add_argument('--connect',
-                            default='docker',
-                            choices=['docker', 'ssh'],
-                            help='file upload stategy (default: docker)',)
+class FastqHandlerManager:
 
-        parser.add_argument(
-            "--keep_names", help="keep original file names", action="store_true")
+    def __init__(self, args: ArgsClass):
+        self.args = args
 
-        parser.add_argument(
-            "--monitor", help="monitor directory until killed", action="store_true")
+    def setup_config(self, args: ArgsClass):
 
-        parser.add_argument(
-            "--televir", help="deploy televir pathogen identification on each sample", action="store_true"
+        actions = []
+
+        if args.merge:
+            actions.append(ProcessActionMergeWithLast())
+
+        if args.downsize:
+            actions.append(ProcessActionDownsize(args.max_size))
+
+        if not actions:
+            print("No actions specified, will merge files by default")
+            actions.append(ProcessActionMergeWithLast())
+
+        run_metadata = RunConfig(
+            fastq_dir=args.in_dir,
+            output_dir=args.out_dir,
+            name_tag=args.tag,
+            actions=actions,
+            keep_name=args.keep_names,
+            sleep_time=args.sleep,
+            max_size=(args.max_size),
         )
+        actions = []
+
+        return run_metadata
+
+    def setup_compressor(self, run_metadata: RunConfig):
+
+        compressor = PreMain(run_metadata)
 
-        return ArgsClass(**parser.parse_args().__dict__)
+        return compressor
+
+    def run(self):
+
+        compressor = self.setup_compressor(self.setup_config(self.args))
+
+        if self.args.monitor:
+
+            compressor.run_until_killed()
+
+        else:
+
+            compressor.run()
+
+
+class InsafluManager:
+
+    def __init__(self, args: ArgsClass):
+        self.args = args
 
     def setup_config(self, args: ArgsClass, test=False):
 
         # check input dir exists
         if not os.path.isdir(args.in_dir):
             print("Input directory does not exist")
             sys.exit(1)
@@ -114,21 +197,23 @@
             connector = ConnectorParamiko(args.config)
 
         insaflu_upload = InsafluUploadRemote(connector, args.config)
 
         # determine upload strategy
         if args.upload == 'last':
             upload_strategy = UploadLast
+        elif args.upload == 'none':
+            upload_strategy = UploadNone
         else:
             upload_strategy = UploadAll
 
         # determine actions
         actions = []
         if args.merge:
-            actions.append(ProcessActionMergeWithLast)
+            actions.append(ProcessActionMergeWithLast())
 
         if args.downsize:
             actions.append(ProcessActionDownsize(args.max_size))
 
         if not actions:
             print("No actions specified, will merge files by default")
             actions.append(ProcessActionMergeWithLast())
@@ -192,15 +277,15 @@
         if file_processor_task.error or televir_processor_task.error:
             return False
 
         return True
 
     def run(self):
 
-        args = self.get_arguments()
+        args = self.args
 
         run_metadata = self.setup_config(args)
 
         influ_compressor, televir_processor = self.generate_runners(
             run_metadata)
 
         file_processor_task, televir_processor_task = self.generate_threads(
```

### Comparing `findontime-0.1.0/src/findontime/plot_utils.py` & `findontime-0.2.0/src/findontime/plot_utils.py`

 * *Files identical despite different names*

### Comparing `findontime-0.1.0/src/findontime/plotting_from_all_reports.py` & `findontime-0.2.0/src/findontime/plotting_from_all_reports.py`

 * *Files identical despite different names*

### Comparing `findontime-0.1.0/src/findontime/records.py` & `findontime-0.2.0/src/findontime/records.py`

 * *Files identical despite different names*

### Comparing `findontime-0.1.0/src/findontime/tables_post.py` & `findontime-0.2.0/src/findontime/tables_post.py`

 * *Files identical despite different names*

### Comparing `findontime-0.1.0/src/findontime/upload_utils.py` & `findontime-0.2.0/src/findontime/upload_utils.py`

 * *Files identical despite different names*

