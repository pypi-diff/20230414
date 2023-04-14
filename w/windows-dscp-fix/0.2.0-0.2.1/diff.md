# Comparing `tmp/windows_dscp_fix-0.2.0.tar.gz` & `tmp/windows_dscp_fix-0.2.1.tar.gz`

## Comparing `windows_dscp_fix-0.2.0.tar` & `windows_dscp_fix-0.2.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      539 1970-01-01 00:00:00.000000 windows_dscp_fix-0.2.0/Cargo.toml
--rw-r--r--   0        0        0     1098 2023-04-13 11:37:44.000000 windows_dscp_fix-0.2.0/.github/workflows/CI.yml
--rw-r--r--   0        0        0      756 2023-04-13 09:21:37.000000 windows_dscp_fix-0.2.0/.gitignore
--rw-r--r--   0        0        0     1212 2023-04-13 11:38:23.000000 windows_dscp_fix-0.2.0/README.md
--rw-r--r--   0        0        0      340 2023-04-13 09:21:37.000000 windows_dscp_fix-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4025 2023-04-13 12:16:01.000000 windows_dscp_fix-0.2.0/src/lib.rs
--rw-r--r--   0        0        0      459 2023-04-13 11:16:59.000000 windows_dscp_fix-0.2.0/windows_dscp_fix/__init__.py
--rw-r--r--   0        0        0     7903 2023-04-13 12:16:37.000000 windows_dscp_fix-0.2.0/Cargo.lock
--rw-r--r--   0        0        0     1547 1970-01-01 00:00:00.000000 windows_dscp_fix-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      539 1970-01-01 00:00:00.000000 windows_dscp_fix-0.2.1/Cargo.toml
+-rw-r--r--   0        0        0     1098 2023-04-13 11:37:44.000000 windows_dscp_fix-0.2.1/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      756 2023-04-13 09:21:37.000000 windows_dscp_fix-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1212 2023-04-13 11:38:23.000000 windows_dscp_fix-0.2.1/README.md
+-rw-r--r--   0        0        0      697 2023-04-14 03:43:14.000000 windows_dscp_fix-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4025 2023-04-13 12:16:01.000000 windows_dscp_fix-0.2.1/src/lib.rs
+-rw-r--r--   0        0        0      459 2023-04-13 11:16:59.000000 windows_dscp_fix-0.2.1/windows_dscp_fix/__init__.py
+-rw-r--r--   0        0        0     7903 2023-04-14 03:47:26.000000 windows_dscp_fix-0.2.1/Cargo.lock
+-rw-r--r--   0        0        0     1844 1970-01-01 00:00:00.000000 windows_dscp_fix-0.2.1/PKG-INFO
```

### Comparing `windows_dscp_fix-0.2.0/Cargo.toml` & `windows_dscp_fix-0.2.1/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b70 6163 6b61 6765 5d0d 0a6e 616d 6520  [package]..name 
 00000010: 3d20 2277 696e 646f 7773 2d64 7363 702d  = "windows-dscp-
 00000020: 6669 7822 0d0a 7665 7273 696f 6e20 3d20  fix"..version = 
-00000030: 2230 2e32 2e30 220d 0a65 6469 7469 6f6e  "0.2.0"..edition
+00000030: 2230 2e32 2e31 220d 0a65 6469 7469 6f6e  "0.2.1"..edition
 00000040: 203d 2022 3230 3231 220d 0a0d 0a23 2053   = "2021"....# S
 00000050: 6565 206d 6f72 6520 6b65 7973 2061 6e64  ee more keys and
 00000060: 2074 6865 6972 2064 6566 696e 6974 696f   their definitio
 00000070: 6e73 2061 7420 6874 7470 733a 2f2f 646f  ns at https://do
 00000080: 632e 7275 7374 2d6c 616e 672e 6f72 672f  c.rust-lang.org/
 00000090: 6361 7267 6f2f 7265 6665 7265 6e63 652f  cargo/reference/
 000000a0: 6d61 6e69 6665 7374 2e68 746d 6c0d 0a5b  manifest.html..[
```

### Comparing `windows_dscp_fix-0.2.0/.github/workflows/CI.yml` & `windows_dscp_fix-0.2.1/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `windows_dscp_fix-0.2.0/.gitignore` & `windows_dscp_fix-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `windows_dscp_fix-0.2.0/README.md` & `windows_dscp_fix-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `windows_dscp_fix-0.2.0/src/lib.rs` & `windows_dscp_fix-0.2.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `windows_dscp_fix-0.2.0/Cargo.lock` & `windows_dscp_fix-0.2.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -215,15 +215,15 @@
 checksum = "cdacb41e6a96a052c6cb63a144f24900236121c6f63f4f8219fef5977ecb0c25"
 dependencies = [
  "windows-targets",
 ]
 
 [[package]]
 name = "windows-dscp-fix"
-version = "0.2.0"
+version = "0.2.1"
 dependencies = [
  "pyo3",
  "windows",
 ]
 
 [[package]]
 name = "windows-sys"
```

### Comparing `windows_dscp_fix-0.2.0/PKG-INFO` & `windows_dscp_fix-0.2.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 Metadata-Version: 2.1
 Name: windows-dscp-fix
-Version: 0.2.0
+Version: 0.2.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
+Summary: fix setsockopt behavior for ToS/DSCP on Windows.
+Keywords: windows,network,socket,development,tos,dscp
+Author-email: sudo_free <sudofree@163.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Project-URL: Homepage, https://github.com/iamhyc/windows-dscp-fix
+Project-URL: Bug Reports, https://github.com/iamhyc/windows-dscp-fix/issues
 
 # Windows DSCP Fix Python Package
 
 A Python package to fix `setsockopt(..,IP_TOS,..)` behavior on Windows.
 
 ### Why
```

