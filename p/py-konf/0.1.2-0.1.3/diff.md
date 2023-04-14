# Comparing `tmp/py_konf-0.1.2.tar.gz` & `tmp/py_konf-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_konf-0.1.2.tar", max compression
+gzip compressed data, was "py_konf-0.1.3.tar", max compression
```

## Comparing `py_konf-0.1.2.tar` & `py_konf-0.1.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0       99 2023-03-23 06:21:58.865805 py_konf-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-03-23 06:21:58.865805 py_konf-0.1.2/py_konf/__init__.py
--rw-r--r--   0        0        0      345 2023-03-23 06:21:58.865805 py_konf-0.1.2/py_konf/cli.py
--rw-r--r--   0        0        0     2638 2023-03-23 06:21:58.865805 py_konf-0.1.2/py_konf/config.py
--rw-r--r--   0        0        0        0 2023-03-23 06:21:58.865805 py_konf-0.1.2/py_konf/sources/__init__.py
--rw-r--r--   0        0        0      148 2023-03-23 06:27:01.452316 py_konf-0.1.2/py_konf/sources/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1522 2023-03-23 06:27:01.452316 py_konf-0.1.2/py_konf/sources/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0     1685 2023-03-23 06:27:01.452316 py_konf-0.1.2/py_konf/sources/__pycache__/cli.cpython-310.pyc
--rw-r--r--   0        0        0      945 2023-03-23 06:27:01.452316 py_konf-0.1.2/py_konf/sources/__pycache__/envvars.cpython-310.pyc
--rw-r--r--   0        0        0     2749 2023-03-23 06:27:01.460316 py_konf-0.1.2/py_konf/sources/__pycache__/files.cpython-310.pyc
--rw-r--r--   0        0        0     1907 2023-03-23 06:27:01.452316 py_konf-0.1.2/py_konf/sources/__pycache__/prompt.cpython-310.pyc
--rw-r--r--   0        0        0      645 2023-03-23 06:21:58.865805 py_konf-0.1.2/py_konf/sources/base.py
--rw-r--r--   0        0        0     1372 2023-03-23 06:21:58.865805 py_konf-0.1.2/py_konf/sources/cli.py
--rw-r--r--   0        0        0      872 2023-03-23 06:21:58.865805 py_konf-0.1.2/py_konf/sources/envvars.py
--rw-r--r--   0        0        0     1853 2023-03-23 06:21:58.865805 py_konf-0.1.2/py_konf/sources/files.py
--rw-r--r--   0        0        0     1140 2023-03-23 06:21:58.865805 py_konf-0.1.2/py_konf/sources/prompt.py
--rw-r--r--   0        0        0        0 2023-03-23 06:21:58.865805 py_konf-0.1.2/py_konf/test/__init__.py
--rw-r--r--   0        0        0      145 2023-03-23 06:27:01.440316 py_konf-0.1.2/py_konf/test/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      521 2023-03-23 06:27:01.440316 py_konf-0.1.2/py_konf/test/__pycache__/conftest.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     2486 2023-03-23 06:27:01.444316 py_konf-0.1.2/py_konf/test/__pycache__/test_cli.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     3908 2023-03-23 06:27:01.452316 py_konf-0.1.2/py_konf/test/__pycache__/test_config.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0      223 2023-03-23 06:21:58.865805 py_konf-0.1.2/py_konf/test/conftest.py
--rw-r--r--   0        0        0        0 2023-03-23 06:21:58.865805 py_konf-0.1.2/py_konf/test/sources/__init__.py
--rw-r--r--   0        0        0      153 2023-03-23 06:27:01.456316 py_konf-0.1.2/py_konf/test/sources/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3069 2023-03-23 06:27:01.456316 py_konf-0.1.2/py_konf/test/sources/__pycache__/test_cli.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     3757 2023-03-23 06:27:01.460316 py_konf-0.1.2/py_konf/test/sources/__pycache__/test_envvars.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     4387 2023-03-23 06:27:01.460316 py_konf-0.1.2/py_konf/test/sources/__pycache__/test_files.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     2237 2023-03-23 06:27:01.464316 py_konf-0.1.2/py_konf/test/sources/__pycache__/test_prompt.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0      918 2023-03-23 06:21:58.865805 py_konf-0.1.2/py_konf/test/sources/test_cli.py
--rw-r--r--   0        0        0     1531 2023-03-23 06:21:58.865805 py_konf-0.1.2/py_konf/test/sources/test_envvars.py
--rw-r--r--   0        0        0     1681 2023-03-23 06:21:58.865805 py_konf-0.1.2/py_konf/test/sources/test_files.py
--rw-r--r--   0        0        0      703 2023-03-23 06:21:58.865805 py_konf-0.1.2/py_konf/test/sources/test_prompt.py
--rw-r--r--   0        0        0     1161 2023-03-23 06:21:58.865805 py_konf-0.1.2/py_konf/test/test_cli.py
--rw-r--r--   0        0        0     1033 2023-03-23 06:21:58.865805 py_konf-0.1.2/py_konf/test/test_config.py
--rw-r--r--   0        0        0      921 2023-03-23 06:21:58.865805 py_konf-0.1.2/py_konf/value.py
--rw-r--r--   0        0        0      506 2023-03-23 06:33:27.160361 py_konf-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       40 2023-03-23 06:21:58.865805 py_konf-0.1.2/test_res/files/alt/test.json
--rw-r--r--   0        0        0       30 2023-03-23 06:21:58.865805 py_konf-0.1.2/test_res/files/json.json
--rw-r--r--   0        0        0       82 2023-03-23 06:21:58.865805 py_konf-0.1.2/test_res/files/sects.conf
--rw-r--r--   0        0        0       23 2023-03-23 06:21:58.865805 py_konf-0.1.2/test_res/files/test.conf
--rw-r--r--   0        0        0       41 2023-03-23 06:21:58.865805 py_konf-0.1.2/test_res/files/test.json
--rw-r--r--   0        0        0      711 1970-01-01 00:00:00.000000 py_konf-0.1.2/setup.py
--rw-r--r--   0        0        0      486 1970-01-01 00:00:00.000000 py_konf-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       99 2023-03-23 06:21:58.865805 py_konf-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-03-23 06:21:58.865805 py_konf-0.1.3/py_konf/__init__.py
+-rw-r--r--   0        0        0      345 2023-03-23 06:21:58.865805 py_konf-0.1.3/py_konf/cli.py
+-rw-r--r--   0        0        0     2638 2023-03-23 06:21:58.865805 py_konf-0.1.3/py_konf/config.py
+-rw-r--r--   0        0        0        0 2023-03-23 06:21:58.865805 py_konf-0.1.3/py_konf/sources/__init__.py
+-rw-r--r--   0        0        0      148 2023-03-23 06:27:01.452316 py_konf-0.1.3/py_konf/sources/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1522 2023-03-23 06:27:01.452316 py_konf-0.1.3/py_konf/sources/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0     1685 2023-03-23 06:27:01.452316 py_konf-0.1.3/py_konf/sources/__pycache__/cli.cpython-310.pyc
+-rw-r--r--   0        0        0      945 2023-03-23 06:27:01.452316 py_konf-0.1.3/py_konf/sources/__pycache__/envvars.cpython-310.pyc
+-rw-r--r--   0        0        0     2749 2023-03-23 06:27:01.460316 py_konf-0.1.3/py_konf/sources/__pycache__/files.cpython-310.pyc
+-rw-r--r--   0        0        0     1907 2023-03-23 06:27:01.452316 py_konf-0.1.3/py_konf/sources/__pycache__/prompt.cpython-310.pyc
+-rw-r--r--   0        0        0      645 2023-03-23 06:21:58.865805 py_konf-0.1.3/py_konf/sources/base.py
+-rw-r--r--   0        0        0     1345 2023-04-14 17:37:06.185471 py_konf-0.1.3/py_konf/sources/cli.py
+-rw-r--r--   0        0        0      872 2023-03-23 06:21:58.865805 py_konf-0.1.3/py_konf/sources/envvars.py
+-rw-r--r--   0        0        0     1853 2023-03-23 06:21:58.865805 py_konf-0.1.3/py_konf/sources/files.py
+-rw-r--r--   0        0        0     1140 2023-03-23 06:21:58.865805 py_konf-0.1.3/py_konf/sources/prompt.py
+-rw-r--r--   0        0        0        0 2023-03-23 06:21:58.865805 py_konf-0.1.3/py_konf/test/__init__.py
+-rw-r--r--   0        0        0      145 2023-03-23 06:27:01.440316 py_konf-0.1.3/py_konf/test/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      521 2023-03-23 06:27:01.440316 py_konf-0.1.3/py_konf/test/__pycache__/conftest.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     2486 2023-03-23 06:27:01.444316 py_konf-0.1.3/py_konf/test/__pycache__/test_cli.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     3908 2023-03-23 06:27:01.452316 py_konf-0.1.3/py_konf/test/__pycache__/test_config.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0      223 2023-03-23 06:21:58.865805 py_konf-0.1.3/py_konf/test/conftest.py
+-rw-r--r--   0        0        0        0 2023-03-23 06:21:58.865805 py_konf-0.1.3/py_konf/test/sources/__init__.py
+-rw-r--r--   0        0        0      153 2023-03-23 06:27:01.456316 py_konf-0.1.3/py_konf/test/sources/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3069 2023-03-23 06:27:01.456316 py_konf-0.1.3/py_konf/test/sources/__pycache__/test_cli.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     3757 2023-03-23 06:27:01.460316 py_konf-0.1.3/py_konf/test/sources/__pycache__/test_envvars.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     4387 2023-03-23 06:27:01.460316 py_konf-0.1.3/py_konf/test/sources/__pycache__/test_files.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     2237 2023-03-23 06:27:01.464316 py_konf-0.1.3/py_konf/test/sources/__pycache__/test_prompt.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0      918 2023-03-23 06:21:58.865805 py_konf-0.1.3/py_konf/test/sources/test_cli.py
+-rw-r--r--   0        0        0     1531 2023-03-23 06:21:58.865805 py_konf-0.1.3/py_konf/test/sources/test_envvars.py
+-rw-r--r--   0        0        0     1681 2023-03-23 06:21:58.865805 py_konf-0.1.3/py_konf/test/sources/test_files.py
+-rw-r--r--   0        0        0      703 2023-03-23 06:21:58.865805 py_konf-0.1.3/py_konf/test/sources/test_prompt.py
+-rw-r--r--   0        0        0     1161 2023-03-23 06:21:58.865805 py_konf-0.1.3/py_konf/test/test_cli.py
+-rw-r--r--   0        0        0     1033 2023-03-23 06:21:58.865805 py_konf-0.1.3/py_konf/test/test_config.py
+-rw-r--r--   0        0        0      921 2023-03-23 06:21:58.865805 py_konf-0.1.3/py_konf/value.py
+-rw-r--r--   0        0        0      506 2023-04-14 17:36:31.522802 py_konf-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       40 2023-03-23 06:21:58.865805 py_konf-0.1.3/test_res/files/alt/test.json
+-rw-r--r--   0        0        0       30 2023-03-23 06:21:58.865805 py_konf-0.1.3/test_res/files/json.json
+-rw-r--r--   0        0        0       82 2023-03-23 06:21:58.865805 py_konf-0.1.3/test_res/files/sects.conf
+-rw-r--r--   0        0        0       23 2023-03-23 06:21:58.865805 py_konf-0.1.3/test_res/files/test.conf
+-rw-r--r--   0        0        0       41 2023-03-23 06:21:58.865805 py_konf-0.1.3/test_res/files/test.json
+-rw-r--r--   0        0        0      711 1970-01-01 00:00:00.000000 py_konf-0.1.3/setup.py
+-rw-r--r--   0        0        0      486 1970-01-01 00:00:00.000000 py_konf-0.1.3/PKG-INFO
```

### Comparing `py_konf-0.1.2/py_konf/config.py` & `py_konf-0.1.3/py_konf/config.py`

 * *Files identical despite different names*

### Comparing `py_konf-0.1.2/py_konf/sources/__pycache__/base.cpython-310.pyc` & `py_konf-0.1.3/py_konf/sources/__pycache__/base.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `py_konf-0.1.2/py_konf/sources/__pycache__/cli.cpython-310.pyc` & `py_konf-0.1.3/py_konf/sources/__pycache__/cli.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `py_konf-0.1.2/py_konf/sources/__pycache__/envvars.cpython-310.pyc` & `py_konf-0.1.3/py_konf/sources/__pycache__/envvars.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `py_konf-0.1.2/py_konf/sources/__pycache__/files.cpython-310.pyc` & `py_konf-0.1.3/py_konf/sources/__pycache__/files.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `py_konf-0.1.2/py_konf/sources/__pycache__/prompt.cpython-310.pyc` & `py_konf-0.1.3/py_konf/sources/__pycache__/prompt.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `py_konf-0.1.2/py_konf/sources/base.py` & `py_konf-0.1.3/py_konf/sources/base.py`

 * *Files identical despite different names*

### Comparing `py_konf-0.1.2/py_konf/sources/cli.py` & `py_konf-0.1.3/py_konf/sources/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,14 @@
                 parser.add_argument(cval.cli_arg, **kwargs)
             else:
                 short, long = cval.cli_arg
                 parser.add_argument(short, long, **kwargs)
 
         args_parsed = vars(
             parser.parse_known_args(args=self.args)[0] if self.args is not None else parser.parse_known_args()[0])
-        print(args_parsed)
 
         vals = {}
         for key, cval in cli_vals.items():
             cli_arg = cval.cli_arg if type(cval.cli_arg) is str else cval.cli_arg[1]
             cli_arg = cli_arg.strip('-')
             v = args_parsed[cli_arg]
             if v is not None:
```

### Comparing `py_konf-0.1.2/py_konf/sources/envvars.py` & `py_konf-0.1.3/py_konf/sources/envvars.py`

 * *Files identical despite different names*

### Comparing `py_konf-0.1.2/py_konf/sources/files.py` & `py_konf-0.1.3/py_konf/sources/files.py`

 * *Files identical despite different names*

### Comparing `py_konf-0.1.2/py_konf/sources/prompt.py` & `py_konf-0.1.3/py_konf/sources/prompt.py`

 * *Files identical despite different names*

### Comparing `py_konf-0.1.2/py_konf/test/__pycache__/conftest.cpython-310-pytest-7.2.2.pyc` & `py_konf-0.1.3/py_konf/test/__pycache__/conftest.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `py_konf-0.1.2/py_konf/test/__pycache__/test_cli.cpython-310-pytest-7.2.2.pyc` & `py_konf-0.1.3/py_konf/test/__pycache__/test_cli.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `py_konf-0.1.2/py_konf/test/__pycache__/test_config.cpython-310-pytest-7.2.2.pyc` & `py_konf-0.1.3/py_konf/test/__pycache__/test_config.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `py_konf-0.1.2/py_konf/test/sources/__pycache__/test_cli.cpython-310-pytest-7.2.2.pyc` & `py_konf-0.1.3/py_konf/test/sources/__pycache__/test_cli.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `py_konf-0.1.2/py_konf/test/sources/__pycache__/test_envvars.cpython-310-pytest-7.2.2.pyc` & `py_konf-0.1.3/py_konf/test/sources/__pycache__/test_envvars.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `py_konf-0.1.2/py_konf/test/sources/__pycache__/test_files.cpython-310-pytest-7.2.2.pyc` & `py_konf-0.1.3/py_konf/test/sources/__pycache__/test_files.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `py_konf-0.1.2/py_konf/test/sources/__pycache__/test_prompt.cpython-310-pytest-7.2.2.pyc` & `py_konf-0.1.3/py_konf/test/sources/__pycache__/test_prompt.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `py_konf-0.1.2/py_konf/test/sources/test_cli.py` & `py_konf-0.1.3/py_konf/test/sources/test_cli.py`

 * *Files identical despite different names*

### Comparing `py_konf-0.1.2/py_konf/test/sources/test_envvars.py` & `py_konf-0.1.3/py_konf/test/sources/test_envvars.py`

 * *Files identical despite different names*

### Comparing `py_konf-0.1.2/py_konf/test/sources/test_files.py` & `py_konf-0.1.3/py_konf/test/sources/test_files.py`

 * *Files identical despite different names*

### Comparing `py_konf-0.1.2/py_konf/test/sources/test_prompt.py` & `py_konf-0.1.3/py_konf/test/sources/test_prompt.py`

 * *Files identical despite different names*

### Comparing `py_konf-0.1.2/py_konf/test/test_cli.py` & `py_konf-0.1.3/py_konf/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `py_konf-0.1.2/py_konf/test/test_config.py` & `py_konf-0.1.3/py_konf/test/test_config.py`

 * *Files identical despite different names*

### Comparing `py_konf-0.1.2/py_konf/value.py` & `py_konf-0.1.3/py_konf/value.py`

 * *Files identical despite different names*

### Comparing `py_konf-0.1.2/setup.py` & `py_konf-0.1.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['py_konf', 'py_konf.sources', 'py_konf.test', 'py_konf.test.sources']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'py-konf',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'Simple lib for loading run configurations',
     'long_description': '# py-konf\n\nA pure python library for gathering program run configuration\nfrom the user/environment\n',
     'author': 'Jordan Paoletti',
     'author_email': 'jordanspaoletti@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

