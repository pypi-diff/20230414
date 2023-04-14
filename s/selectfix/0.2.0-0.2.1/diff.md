# Comparing `tmp/selectfix-0.2.0.tar.gz` & `tmp/selectfix-0.2.1.tar.gz`

## Comparing `selectfix-0.2.0.tar` & `selectfix-0.2.1.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0      438 1970-01-01 00:00:00.000000 selectfix-0.2.0/Cargo.toml
--rw-r--r--   0     1001      123      125 2022-12-13 08:05:51.000000 selectfix-0.2.0/README.md
--rw-r--r--   0        0        0       10 2022-12-13 08:08:32.000000 selectfix-0.2.0/dist/selectfix-0.2.0.tar.gz
--rw-r--r--   0     1001      123      313 2022-12-13 08:05:51.000000 selectfix-0.2.0/pyproject.toml
--rwxr-xr-x   0     1001      123      767 2022-12-13 08:06:24.000000 selectfix-0.2.0/run-maturin-action.sh
--rw-r--r--   0     1001      123     6268 2022-12-13 08:05:51.000000 selectfix-0.2.0/src/lib.rs
--rw-r--r--   0     1001      123        0 2022-12-13 08:05:51.000000 selectfix-0.2.0/tests/__init__.py
--rw-r--r--   0     1001      123     2461 2022-12-13 08:05:51.000000 selectfix-0.2.0/tests/test_selectfix.py
--rw-r--r--   0     1001      123     8559 2022-12-13 08:08:30.000000 selectfix-0.2.0/Cargo.lock
--rw-r--r--   0        0        0      453 1970-01-01 00:00:00.000000 selectfix-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      438 1970-01-01 00:00:00.000000 selectfix-0.2.1/Cargo.toml
+-rw-r--r--   0     1001      123     1209 2023-04-14 04:29:21.000000 selectfix-0.2.1/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123     1046 2023-04-14 04:29:21.000000 selectfix-0.2.1/.github/workflows/_workflow.yml
+-rw-r--r--   0     1001      123      685 2023-04-14 04:29:21.000000 selectfix-0.2.1/.gitignore
+-rw-r--r--   0     1001      123      125 2023-04-14 04:29:21.000000 selectfix-0.2.1/README.md
+-rw-r--r--   0     1001      123      313 2023-04-14 04:29:21.000000 selectfix-0.2.1/pyproject.toml
+-rwxr-xr-x   0     1001      123     1058 2023-04-14 04:31:36.000000 selectfix-0.2.1/run-maturin-action.sh
+-rw-r--r--   0     1001      123     6268 2023-04-14 04:29:21.000000 selectfix-0.2.1/src/lib.rs
+-rw-r--r--   0     1001      123        0 2023-04-14 04:29:21.000000 selectfix-0.2.1/tests/__init__.py
+-rw-r--r--   0     1001      123     2461 2023-04-14 04:29:21.000000 selectfix-0.2.1/tests/test_selectfix.py
+-rw-r--r--   0     1001      123     8559 2023-04-14 04:29:21.000000 selectfix-0.2.1/Cargo.lock
+-rw-r--r--   0        0        0      453 1970-01-01 00:00:00.000000 selectfix-0.2.1/PKG-INFO
```

### Comparing `selectfix-0.2.0/src/lib.rs` & `selectfix-0.2.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `selectfix-0.2.0/tests/test_selectfix.py` & `selectfix-0.2.1/tests/test_selectfix.py`

 * *Files identical despite different names*

### Comparing `selectfix-0.2.0/Cargo.lock` & `selectfix-0.2.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -211,15 +211,15 @@
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "selectfix"
-version = "0.2.0"
+version = "0.2.1"
 dependencies = [
  "anyhow",
  "bincode",
  "indexmap",
  "ordered-float",
  "pyo3",
  "serde",
```

