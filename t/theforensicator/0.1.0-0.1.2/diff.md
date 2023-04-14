# Comparing `tmp/theforensicator-0.1.0.tar.gz` & `tmp/theforensicator-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "theforensicator-0.1.0.tar", max compression
+gzip compressed data, was "theforensicator-0.1.2.tar", max compression
```

## Comparing `theforensicator-0.1.0.tar` & `theforensicator-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,24 @@
--rw-r--r--   0        0        0     1072 2023-04-11 21:38:45.799344 theforensicator-0.1.0/LICENSE
--rw-r--r--   0        0        0     1091 2023-04-11 21:38:45.799344 theforensicator-0.1.0/README.md
--rw-r--r--   0        0        0     3100 2023-04-11 21:38:45.803344 theforensicator-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       45 2023-04-11 21:38:45.803344 theforensicator-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      586 2023-04-11 21:38:45.803344 theforensicator-0.1.0/tests/test_app.py
--rw-r--r--   0        0        0      145 2023-04-11 21:38:45.803344 theforensicator-0.1.0/theforensicator/__init__.py
--rw-r--r--   0        0        0     5253 2023-04-11 21:38:45.803344 theforensicator-0.1.0/theforensicator/app.py
--rw-r--r--   0        0        0        0 2023-04-11 21:38:45.803344 theforensicator-0.1.0/theforensicator/artefacts/browser.yaml
--rw-r--r--   0        0        0      288 2023-04-11 21:38:45.803344 theforensicator-0.1.0/theforensicator/artefacts/registry.yaml
--rw-r--r--   0        0        0      821 2023-04-11 21:38:45.803344 theforensicator-0.1.0/theforensicator/cli.py
--rw-r--r--   0        0        0       30 2023-04-11 21:38:45.803344 theforensicator-0.1.0/theforensicator/ewf/__init__.py
--rw-r--r--   0        0        0    19995 2023-04-11 21:38:45.803344 theforensicator-0.1.0/theforensicator/ewf/file_parsing.py
--rw-r--r--   0        0        0       65 2023-04-11 21:38:45.803344 theforensicator-0.1.0/theforensicator/fs/__init__.py
--rw-r--r--   0        0        0     1156 2023-04-11 21:38:45.803344 theforensicator-0.1.0/theforensicator/fs/gpt.py
--rw-r--r--   0        0        0     1014 2023-04-11 21:38:45.803344 theforensicator-0.1.0/theforensicator/fs/mbr.py
--rw-r--r--   0        0        0    32802 2023-04-11 21:38:45.803344 theforensicator-0.1.0/theforensicator/fs/ntfs.py
--rw-r--r--   0        0        0     3534 1970-01-01 00:00:00.000000 theforensicator-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-14 20:25:49.052108 theforensicator-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1091 2023-04-14 20:25:49.052108 theforensicator-0.1.2/README.md
+-rw-r--r--   0        0        0     3100 2023-04-14 20:25:49.056108 theforensicator-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       45 2023-04-14 20:25:49.056108 theforensicator-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0      586 2023-04-14 20:25:49.056108 theforensicator-0.1.2/tests/test_app.py
+-rw-r--r--   0        0        0      145 2023-04-14 20:25:49.056108 theforensicator-0.1.2/theforensicator/__init__.py
+-rw-r--r--   0        0        0     4939 2023-04-14 20:25:49.056108 theforensicator-0.1.2/theforensicator/app.py
+-rw-r--r--   0        0        0      473 2023-04-14 20:25:49.056108 theforensicator-0.1.2/theforensicator/artefacts/browser_chrome.yaml
+-rw-r--r--   0        0        0      116 2023-04-14 20:25:49.056108 theforensicator-0.1.2/theforensicator/artefacts/browser_edge.yaml
+-rw-r--r--   0        0        0      668 2023-04-14 20:25:49.056108 theforensicator-0.1.2/theforensicator/artefacts/browser_firefox.yaml
+-rw-r--r--   0        0        0      467 2023-04-14 20:25:49.056108 theforensicator-0.1.2/theforensicator/artefacts/browser_ie.yaml
+-rw-r--r--   0        0        0      170 2023-04-14 20:25:49.056108 theforensicator-0.1.2/theforensicator/artefacts/events_logs.yaml
+-rw-r--r--   0        0        0       97 2023-04-14 20:25:49.056108 theforensicator-0.1.2/theforensicator/artefacts/prefetch.yaml
+-rw-r--r--   0        0        0      366 2023-04-14 20:25:49.056108 theforensicator-0.1.2/theforensicator/artefacts/registry_system.yaml
+-rw-r--r--   0        0        0      129 2023-04-14 20:25:49.056108 theforensicator-0.1.2/theforensicator/artefacts/registry_user.yaml
+-rw-r--r--   0        0        0     2156 2023-04-14 20:25:49.056108 theforensicator-0.1.2/theforensicator/cli.py
+-rw-r--r--   0        0        0       30 2023-04-14 20:25:49.056108 theforensicator-0.1.2/theforensicator/ewf/__init__.py
+-rw-r--r--   0        0        0    19995 2023-04-14 20:25:49.056108 theforensicator-0.1.2/theforensicator/ewf/file_parsing.py
+-rw-r--r--   0        0        0       65 2023-04-14 20:25:49.056108 theforensicator-0.1.2/theforensicator/fs/__init__.py
+-rw-r--r--   0        0        0    12818 2023-04-14 20:25:49.056108 theforensicator-0.1.2/theforensicator/fs/defs.py
+-rw-r--r--   0        0        0     4929 2023-04-14 20:25:49.056108 theforensicator-0.1.2/theforensicator/fs/gpt.py
+-rw-r--r--   0        0        0     3421 2023-04-14 20:25:49.056108 theforensicator-0.1.2/theforensicator/fs/mbr.py
+-rw-r--r--   0        0        0    34074 2023-04-14 20:25:49.056108 theforensicator-0.1.2/theforensicator/fs/ntfs.py
+-rw-r--r--   0        0        0     3534 1970-01-01 00:00:00.000000 theforensicator-0.1.2/PKG-INFO
```

### Comparing `theforensicator-0.1.0/LICENSE` & `theforensicator-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `theforensicator-0.1.0/README.md` & `theforensicator-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `theforensicator-0.1.0/pyproject.toml` & `theforensicator-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "theforensicator"
-version = "0.1.0"
+version = "0.1.2"
 homepage = "https://github.com/ValekoZ/theforensicator"
 description = "School project for forensic investigations."
 authors = [
     "Joël RABAH <joel.rabah@ecole2600.com>",
     "Edouard GOUT <edouard.gout@ecole2600.com>",
     "Yann MAJEROWICZ <yann.majerowicz@ecole2600.com>",
     "Bastien WINTER DURENNEL <bastien.winter-durennel@ecole2600.com>",
```

### Comparing `theforensicator-0.1.0/tests/test_app.py` & `theforensicator-0.1.2/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `theforensicator-0.1.0/theforensicator/app.py` & `theforensicator-0.1.2/theforensicator/app.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,34 @@
 """Main module."""
 
 from struct import unpack
-
-# import pyewf as test
-import yaml
-
 from .fs import GPT, MBR, NTFS
 
 MBR_MAGIC = 0xD08EC033
 MBR_SIZE = 512
 
 NTFS_MAGIC = 0x4E9052EB
 
 SECTOR_SIZE = 512
 
 UINT32 = 4
 UINT64 = 8
 
-
 class EWFImage(object):
     """Object that reads the content of the EWF file and parses the content"""
 
     def __init__(self, filename: str) -> None:
         """Initialize the object with default values and the given filename
 
         Args:
             filename: The filename of the file to parse
         """
         self.filename = filename
         self.handle = None
-        self.verbosity = True
+        self.verbose = True
         self.ntfs_partitions = []
         self.mft_dump_location = None
         self.out_file_location = None
 
     def __enter__(self) -> None:
         """Open a handle on EWF files and read the content. Called when we enter
         a `with` block
@@ -135,49 +130,39 @@
         return self._read_int((nb_sector * 512) + offset)
 
     def _find_ntfs_partitions(self):
         """Retrieve all the NTFS partitions (_get_partitions needs to be called
         before this function)
         """
         for partition in self.gpt_partitions:
-            magic = self._read_int_at_sector_offset(partition.first_lba, 0)
+            magic = self._read_int_at_sector_offset(partition["first_lba"], 0)
             if magic == NTFS_MAGIC:
                 self.ntfs_partitions.append(NTFS(self, partition))
 
     def read_ewf(self):
         """Read the EWF file, and parse the partition tables"""
-        # self.handle.display_properties()
 
         if not self._is_mbr_partition():
             print("[!] No MBR partition found, exiting...")
             exit(-1)
 
         print("[+] MBR partition found.")
 
         self._get_partitions()
-
         self._find_ntfs_partitions()
 
-    def analyze_ntfs(self, out_dir: str, dump_dir: str, resolve_mft_file: str):
+    def analyze_ntfs(self, resolve_mft_file: str, clear_cache):
         """Analyze the NTFS partitions to extract the wanted files
 
         Args:
-            out_dir: Directory where non-resolved MFT will be stored
-            dump_dir: Directory where non-resolved MFT is stored
             resolve_mft_file: Output file of resolved MFT in JSON format
         """
-        out_file = ""
-        dump_file = ""
-
-        if out_dir:
-            out_file = f"{out_dir}/mft_dump.json"
-
-        if dump_dir:
-            dump_file = f"{dump_dir}/mft_dump.json"
+        for (part_idx, partition) in enumerate(self.ntfs_partitions):
+            partition.analyze_ntfs_header(part_idx, resolve_mft_file, clear_cache)
 
+    def dump_file(self, filenames: list, dump_dir: str):
         for partition in self.ntfs_partitions:
-            partition.analyze_ntfs_header(out_file, dump_file, resolve_mft_file)
-            partition.dump_file(["C:\\Windows\\System32\\config\\SYSTEM"])
+            partition.dump_file(filenames, dump_dir)
 
     def __exit__(self, exception_type, exception_value, exception_traceback):
         """Close and clean everything. Called when we exit a `with` block."""
         pass
```

### Comparing `theforensicator-0.1.0/theforensicator/ewf/file_parsing.py` & `theforensicator-0.1.2/theforensicator/ewf/file_parsing.py`

 * *Files identical despite different names*

### Comparing `theforensicator-0.1.0/theforensicator/fs/ntfs.py` & `theforensicator-0.1.2/theforensicator/fs/ntfs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 """Parser for NTFS"""
 
 import datetime
 import json
+import re
 from struct import unpack, unpack_from
-
-import pyreadpartitions as pypart
+from os.path import normpath, isfile
+from os import unlink
 
 import theforensicator
 
 SECTOR_SIZE = 512
 
-
 def SECTOR_NB(x):
     return x // SECTOR_SIZE
 
-
 BIOS_PARAMETER_BLOCK_T = "HBHBHHBHHHII"
 NTFS_BOOT_SECTOR_T = "<3sQ" + BIOS_PARAMETER_BLOCK_T + "IQQQB3sB3sQI426sH"
 
 MFT_HEADER_SIZE = 48
 MFT_ENTRY_SIZE = 1024
 MFT_RECORD_T = f"<IHHQHHHHIIQHHI{MFT_ENTRY_SIZE - MFT_HEADER_SIZE}s"
 
@@ -111,39 +110,41 @@
         Args:
             ewf_image: EWF object we are based on
             partition: Partition we will parse
         """
         self.ewf_image = ewf_image
 
         self.handle = self.ewf_image.handle
-        self.verbosity = self.ewf_image.verbosity
+        self.verbose = self.ewf_image.verbose
         self.partition = partition
-        self._start = self.partition.first_lba
-        self._end = self.partition.last_lba
+        self._start = self.partition["first_lba"]
+        self._end = self.partition["last_lba"]
 
         self.is_mft_dump = None
         self.dump_mft = None
 
         self.handle.seek(self._start * SECTOR_SIZE)
         self.ntfs_header = NTFSHeader(
             self._read_nsectors(0, SECTOR_NB(SECTOR_SIZE))
         ).ntfs_header
         self.cluster_block_size = (
             self.ntfs_header["bytes_per_sector"]
             * self.ntfs_header["sectors_per_cluster"]
         )
 
-        if self.verbosity:
-            self._pretty_print()
+        print("[+] NTFS partition at sector %#x" % (self._start))
+
+        if self.verbose:
+            pass
+            #self._pretty_print()
 
         self.mft = {}
 
     def _pretty_print(self):
         """Prints additionnal informations about the partition"""
-        print("[+] NTFS partition at sector %#x" % (self._start))
 
         for header_name in self.ntfs_header.keys():
             if type(self.ntfs_header[header_name]) is bytes or str:
                 print("\t%-18s : %s" % (header_name, self.ntfs_header[header_name]))
             else:
                 print("\t%-20s : %#x" % (header_name, self.ntfs_header[header_name]))
 
@@ -248,44 +249,46 @@
         Args:
             dump_file: Path of the dump
         """
         with open(dump_file, "r") as dmp_file:
             self.dump_mft = json.loads(dmp_file.read())
             dmp_file.close()
 
-    def analyze_ntfs_header(self, out_file: str, dump_file: str, resolve_mft_file: str):
+    def analyze_ntfs_header(self, partition_idx: str, resolve_mft_file: str, clear_cache):
         """Analyze the NTFS header
 
         Args:
             out_file: Where to store the output
             dump_file: Where the output has been stored in a previous run
             resolve_mft_file: Where the resolved MFT in JSON format will be stored
         """
+        mft_dump_filepath = f"MFT{partition_idx}.dump"
+
+        if clear_cache:
+            if isfile(mft_dump_filepath):
+                unlink(mft_dump_filepath)
+                print("[+] Cache cleared.")
+
         self.mft_start = self.ntfs_header["mft_lcn"]
 
         print("[+] Loading and analyzing MFT ...")
 
-        if out_file:
+        if not isfile(mft_dump_filepath):
             self.is_mft_dump = False
-            self.analyze_mft(out_file)
-
-        if dump_file:
+            self.analyze_mft(mft_dump_filepath)
+        else:
+            print("[+] Found %s, loading cache file." % (mft_dump_filepath))
             self.is_mft_dump = True
-            self.load_mft_dump(dump_file)
-
-        if not out_file and not dump_file:
-            print("[?] You didn't provide output arguments")
-            exit()
+            self.load_mft_dump(mft_dump_filepath)
+            print("[+] Cache file loaded.")
 
         print("[+] MFT loaded ...")
 
         self.resolve_mft(resolve_mft_file)
 
-        # return self.resolved_mft
-
     def _get_dump_mft_entry(self, idx: int):
         """Get a dump of the given mft entry
 
         Args:
             Index of the MFT entry to dump
         """
         return (
@@ -382,18 +385,19 @@
                         "info": path_infos,
                         "dates": entry["dates"],
                         "data": data,
                     }
 
         print("[+] MFT paths resolved ...")
 
-        if json_outfile:
+        if json_outfile and type(json_outfile) is str:
             with open(json_outfile, "w") as dmp:
                 dmp.write(json.dumps(self.resolved_mft))
                 dmp.close()
+            print("[+] %s successfully written." % (json_outfile))
 
     def analyze_mft(self, out_file: str):
         """Analyze the MFT
 
         Args:
             out_file: Where to store the output
         """
@@ -430,42 +434,68 @@
             dmp_file.close()
 
     def _dump_data(self, lcn_dict: dict) -> bytes:
         raw_data = lcn_dict["raw_data"]
 
         buf = b""
 
+        if lcn_dict["size"] == 0 and len(raw_data) == 0:
+            return b""
+
+        if type(raw_data) is str:
+            return bytes.fromhex(raw_data)
+
         for lcn in raw_data:
             for idx in range(lcn["lcn_length"]):
                 buf += self._read_cluster(lcn["lcn_offset"] + idx)
 
         return buf[: lcn_dict["init_size"]]
 
-    def dump_file(self, filenames: str) -> bytes:
+    def write_to_file(self, dump_dir, filename: str, data: bytes):
+        if dump_dir and type(dump_dir) is str:
+            out_filename = normpath(dump_dir + "/dump_" + filename.replace('\\', '_').replace(':', ''))
+        else:
+            out_filename = "./dump_" + filename.replace('\\', '_').replace(':', '')
+
+        with open(out_filename, "wb") as f:
+            f.write(data)
+            f.close()
+
+        print("[?] %s successfully dumped to %s." % (filename, out_filename))
+
+    def dump_file(self, filenames: list, dump_dir: str) -> bytes:
         """Dump a file using its filename
 
         Args:
             filenames: Filename of the file to dump
 
         Returns:
             The file content
         """
+
+        files_list_match = '(?:%s)' % '|'.join(filenames)
+
         for key in self.resolved_mft:
+            
             obj_type = self.resolved_mft[key]["type"]
 
             if obj_type not in ["FILE", "ORPHAN_FILE"]:
                 continue
 
             info = self.resolved_mft[key]["info"]
 
             for file in info:
-                if file["file_name"] in filenames:
+                if re.match(files_list_match, file["file_name"], flags=re.IGNORECASE):
                     data = self.resolved_mft[key]["data"]
                     if data:
-                        return self._dump_data(data)
+                        self.write_to_file(
+                            dump_dir,
+                            file["file_name"],
+                            self._dump_data(data)
+                        )
 
     def _analyze_registry(self):
         print("[?] Analyzing registries")
 
     def _analyze_winsec(self):
         print("[?] Analyzing Windows Security")
 
@@ -475,15 +505,15 @@
 
     def __init__(self, header: bytes, ntfs: "NTFS", verbose: bool) -> None:
         """Initialize the MFT class
 
         Args:
             header: Header of the MFT
             ntfs: NTFS
-            verbose: verbosity
+            verbose: verbose
         """
         self._mft_fields = [
             "magic",
             "usa_ofs",
             "usa_count",
             "lsn",
             "sequence_number",
```

### Comparing `theforensicator-0.1.0/PKG-INFO` & `theforensicator-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: theforensicator
-Version: 0.1.0
+Version: 0.1.2
 Summary: School project for forensic investigations.
 Home-page: https://github.com/ValekoZ/theforensicator
 License: MIT
 Author: Joël RABAH
 Author-email: joel.rabah@ecole2600.com
 Requires-Python: >=3.7.1,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

