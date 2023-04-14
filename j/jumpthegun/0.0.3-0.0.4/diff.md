# Comparing `tmp/jumpthegun-0.0.3.tar.gz` & `tmp/jumpthegun-0.0.4.tar.gz`

## Comparing `jumpthegun-0.0.3.tar` & `jumpthegun-0.0.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/.flake8
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/test_requirements.txt
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/tox.ini
--rwxr-xr-x   0        0        0     3343 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/src/jumpthegun.sh
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/src/jumpthegun/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/src/jumpthegun/__version__.py
--rw-r--r--   0        0        0    14142 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/src/jumpthegun/jumpthegunctl.py
--rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/src/jumpthegun/output_redirect.py
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/src/jumpthegun/project.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/src/jumpthegun/testutils.py
--rw-r--r--   0        0        0     3298 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/src/jumpthegun/tools.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/src/jumpthegun/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/src/vendor/__init__.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/src/vendor/filelock/LICENSE
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/src/vendor/filelock/README.md
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/src/vendor/filelock/VERSION
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/src/vendor/filelock/__init__.py
--rw-r--r--   0        0        0     8896 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/src/vendor/filelock/_api.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/src/vendor/filelock/_error.py
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/src/vendor/filelock/_soft.py
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/src/vendor/filelock/_unix.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/src/vendor/filelock/_util.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/src/vendor/filelock/_windows.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/src/vendor/filelock/py.typed
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/src/vendor/filelock/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0     6524 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/tests/test_jumpthegun.py
--rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/tests/test_tools.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/tests/testproj/.flake8
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/tests/testproj/bad.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/tests/testproj/good.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/tests/testproj/pyproject.toml
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/LICENSE
--rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/README.md
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 jumpthegun-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/.flake8
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/test_requirements.txt
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/tox.ini
+-rwxr-xr-x   0        0        0     3343 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/src/jumpthegun.sh
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/src/jumpthegun/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/src/jumpthegun/__version__.py
+-rw-r--r--   0        0        0    14142 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/src/jumpthegun/jumpthegunctl.py
+-rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/src/jumpthegun/output_redirect.py
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/src/jumpthegun/project.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/src/jumpthegun/testutils.py
+-rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/src/jumpthegun/tools.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/src/jumpthegun/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/src/vendor/__init__.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/src/vendor/filelock/LICENSE
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/src/vendor/filelock/README.md
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/src/vendor/filelock/VERSION
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/src/vendor/filelock/__init__.py
+-rw-r--r--   0        0        0     8896 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/src/vendor/filelock/_api.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/src/vendor/filelock/_error.py
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/src/vendor/filelock/_soft.py
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/src/vendor/filelock/_unix.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/src/vendor/filelock/_util.py
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/src/vendor/filelock/_windows.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/src/vendor/filelock/py.typed
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/src/vendor/filelock/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0     6524 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/tests/test_jumpthegun.py
+-rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/tests/test_tools.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/tests/testproj/.flake8
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/tests/testproj/bad.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/tests/testproj/good.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/tests/testproj/pyproject.toml
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/README.md
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 jumpthegun-0.0.4/PKG-INFO
```

### Comparing `jumpthegun-0.0.3/src/jumpthegun.sh` & `jumpthegun-0.0.4/src/jumpthegun.sh`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.3/src/jumpthegun/jumpthegunctl.py` & `jumpthegun-0.0.4/src/jumpthegun/jumpthegunctl.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.3/src/jumpthegun/output_redirect.py` & `jumpthegun-0.0.4/src/jumpthegun/output_redirect.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.3/src/jumpthegun/project.py` & `jumpthegun-0.0.4/src/jumpthegun/project.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.3/src/jumpthegun/tools.py` & `jumpthegun-0.0.4/src/jumpthegun/tools.py`

 * *Files 18% similar despite different names*

```diff
@@ -63,28 +63,37 @@
 
 
 SCRIPT_ENCODING_HEADER_RE = re.compile(
     br'^#\s*-\*- coding: ([a-zA-Z0-9._-]+) -\*-\s*$',
     re.MULTILINE,
 )
 # See distlib: https://github.com/pypa/distlib/blob/05375908c1b2d6b0e74bdeb574569d3609db9f56/distlib/scripts.py#L43-L50
-ENTRYPOINT_SCRIPT_TEMPLATE = textwrap.dedent(r'''
+entrypoint_script_template = textwrap.dedent(r'''
     import re
     import sys
     from %(module)s import %(import_name)s
     if __name__ == '__main__':
         sys.argv[0] = re.sub(r'(-script\.pyw|\.exe)?$', '', sys.argv[0])
         sys.exit(%(func)s())
     ''')[1:]
-ENTRYPOINT_SCRIPT_RE = re.compile(
-    re.sub(
-        re.escape(re.escape('%(')) + r'(\w+)' + re.escape(re.escape(')s')),
-        r'(?P<\1>(?:\\w|\\.)+)',
-        re.escape(ENTRYPOINT_SCRIPT_TEMPLATE),
-    ),
+entrypoint_script_regexp_str = re.sub(
+    # Escape twice: Once because this is creating a regexp string, and again
+    # because this uses re.sub() on the regexp string.
+    re.escape(re.escape('%(')) + r'(\w+)' + re.escape(re.escape(')s')),
+    r'(?P<\1>(?:\\w|\\.)+)',
+    re.escape(entrypoint_script_template),
+)
+# Sometimes such entrypoint scripts have double-quotes rather than
+# single-quotes.
+# Example: https://src.fedoraproject.org/rpms/python-wheel/blob/rawhide/f/wheel-entrypoint
+entrypoint_script_any_quote_regexp_str = entrypoint_script_regexp_str.replace(
+    re.escape("'"), r'''['"]''',
+)
+ENTRYPOINT_SCRIPT_REGEXP = re.compile(
+    entrypoint_script_any_quote_regexp_str,
     re.IGNORECASE,
 )
 
 
 def find_entrypoint_func_in_entrypoint_script(tool_name: str) -> str | None:
     # Search for the executable.
     executable_path = shutil.which(tool_name)
@@ -101,10 +110,10 @@
             encoding = "utf-8"
         code = code_bytes.decode(encoding)
     except UnicodeDecodeError:
         # TODO: Warn
         return None
 
     # Try to find an entrypoint function in the script's code.
-    if entrypoint_script_match := ENTRYPOINT_SCRIPT_RE.search(code):
+    if entrypoint_script_match := ENTRYPOINT_SCRIPT_REGEXP.search(code):
         groupdict = entrypoint_script_match.groupdict()
         return f"{groupdict['module']}:{groupdict['func']}"
```

### Comparing `jumpthegun-0.0.3/src/jumpthegun/utils.py` & `jumpthegun-0.0.4/src/jumpthegun/utils.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.3/src/vendor/filelock/LICENSE` & `jumpthegun-0.0.4/src/vendor/filelock/LICENSE`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.3/src/vendor/filelock/README.md` & `jumpthegun-0.0.4/src/vendor/filelock/README.md`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.3/src/vendor/filelock/__init__.py` & `jumpthegun-0.0.4/src/vendor/filelock/__init__.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.3/src/vendor/filelock/_api.py` & `jumpthegun-0.0.4/src/vendor/filelock/_api.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.3/src/vendor/filelock/_soft.py` & `jumpthegun-0.0.4/src/vendor/filelock/_soft.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.3/src/vendor/filelock/_unix.py` & `jumpthegun-0.0.4/src/vendor/filelock/_unix.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.3/src/vendor/filelock/_util.py` & `jumpthegun-0.0.4/src/vendor/filelock/_util.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.3/src/vendor/filelock/_windows.py` & `jumpthegun-0.0.4/src/vendor/filelock/_windows.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.3/tests/test_jumpthegun.py` & `jumpthegun-0.0.4/tests/test_jumpthegun.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.3/tests/test_tools.py` & `jumpthegun-0.0.4/tests/test_tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,24 +25,37 @@
     from module_name.submodule_name.main import func_name
     if __name__ == '__main__':
         sys.argv[0] = re.sub(r'(-script\\.pyw|\\.exe)?$', '', sys.argv[0])
         sys.exit(func_name())
 ''')
 script2_entrypoint_str = "module_name.submodule_name.main:func_name"
 
+script3_code = textwrap.dedent('''\
+    #!/nonexistent/path/to/fake/venv/bin/python
+    import re
+    import sys
+    from module_name.submodule_name.main import func_name
+    if __name__ == "__main__":
+        sys.argv[0] = re.sub(r"(-script\\.pyw|\\.exe)?$", "", sys.argv[0])
+        sys.exit(func_name())
+''')
+script3_entrypoint_str = "module_name.submodule_name.main:func_name"
+
 
 @pytest.mark.parametrize(
     ["script_code", "entrypoint_str"],
     [
         (script1_code, script1_entrypoint_str),
         (script2_code, script2_entrypoint_str),
+        (script3_code, script3_entrypoint_str),
     ],
     ids=[
         "script1",
         "script2",
+        "script3",
     ],
 )
 def test_find_entrypoint_func_in_entrypoint_script(monkeypatch, tmp_path, script_code, entrypoint_str):
     """Test parsing an entrypoint script.
 
     Such scripts are created by pip and other tools which use distlib.
     """
```

### Comparing `jumpthegun-0.0.3/.gitignore` & `jumpthegun-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.3/LICENSE` & `jumpthegun-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.3/README.md` & `jumpthegun-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.3/pyproject.toml` & `jumpthegun-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.3/PKG-INFO` & `jumpthegun-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jumpthegun
-Version: 0.0.3
+Version: 0.0.4
 Summary: Make Python CLI tools win the speed race, by cheating!
 Project-URL: Homepage, https://github.com/taleinat/jumpthegun
 Author-email: Tal Einat <taleinat@gmail.com>
 License: Apache-2.0
 License-File: LICENSE
 Keywords: cli
 Classifier: Development Status :: 1 - Planning
```

