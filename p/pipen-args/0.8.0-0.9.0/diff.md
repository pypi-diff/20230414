# Comparing `tmp/pipen_args-0.8.0.tar.gz` & `tmp/pipen_args-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipen_args-0.8.0.tar", max compression
+gzip compressed data, was "pipen_args-0.9.0.tar", max compression
```

## Comparing `pipen_args-0.8.0.tar` & `pipen_args-0.9.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2289 2023-03-29 22:40:26.987219 pipen_args-0.8.0/README.md
--rw-r--r--   0        0        0      969 2023-03-29 22:40:26.987219 pipen_args-0.8.0/pipen_args/__init__.py
--rw-r--r--   0        0        0     3851 2023-03-29 22:40:26.987219 pipen_args-0.8.0/pipen_args/defaults.py
--rw-r--r--   0        0        0     4860 2023-03-29 22:40:26.987219 pipen_args-0.8.0/pipen_args/install.py
--rw-r--r--   0        0        0     9490 2023-03-29 22:40:26.987219 pipen_args-0.8.0/pipen_args/parser_.py
--rw-r--r--   0        0        0     3277 2023-03-29 22:40:26.987219 pipen_args-0.8.0/pipen_args/procgroup.py
--rw-r--r--   0        0        0       22 2023-03-29 22:40:26.991219 pipen_args-0.8.0/pipen_args/version.py
--rw-r--r--   0        0        0     1164 2023-03-29 22:40:26.991219 pipen_args-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     3030 1970-01-01 00:00:00.000000 pipen_args-0.8.0/setup.py
--rw-r--r--   0        0        0     2980 1970-01-01 00:00:00.000000 pipen_args-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     2159 2023-04-14 20:12:43.760336 pipen_args-0.9.0/README.md
+-rw-r--r--   0        0        0      969 2023-04-14 20:12:43.760336 pipen_args-0.9.0/pipen_args/__init__.py
+-rw-r--r--   0        0        0     3851 2023-04-14 20:12:43.760336 pipen_args-0.9.0/pipen_args/defaults.py
+-rw-r--r--   0        0        0     9490 2023-04-14 20:12:43.760336 pipen_args-0.9.0/pipen_args/parser_.py
+-rw-r--r--   0        0        0     4784 2023-04-14 20:12:43.760336 pipen_args-0.9.0/pipen_args/plugin.py
+-rw-r--r--   0        0        0     3277 2023-04-14 20:12:43.760336 pipen_args-0.9.0/pipen_args/procgroup.py
+-rw-r--r--   0        0        0       22 2023-04-14 20:12:43.760336 pipen_args-0.9.0/pipen_args/version.py
+-rw-r--r--   0        0        0     1185 2023-04-14 20:12:43.760336 pipen_args-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     3001 1970-01-01 00:00:00.000000 pipen_args-0.9.0/setup.py
+-rw-r--r--   0        0        0     2850 1970-01-01 00:00:00.000000 pipen_args-0.9.0/PKG-INFO
```

### Comparing `pipen_args-0.8.0/README.md` & `pipen_args-0.9.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -2,17 +2,15 @@
 
 Command line argument parser for [pipen][1]
 
 ## Usage
 
 ```python
 from pipen import Proc, Pipen
-# Note that unlike other plugins, you need to import install
-# to activate the plugin
-from pipen_args import install  # noqa: F401
+
 
 class Process(Proc):
     """My process
 
     Input:
         a: Input data
     """
```

### Comparing `pipen_args-0.8.0/pipen_args/__init__.py` & `pipen_args-0.9.0/pipen_args/__init__.py`

 * *Files identical despite different names*

### Comparing `pipen_args-0.8.0/pipen_args/defaults.py` & `pipen_args-0.9.0/pipen_args/defaults.py`

 * *Files identical despite different names*

### Comparing `pipen_args-0.8.0/pipen_args/install.py` & `pipen_args-0.9.0/pipen_args/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 from pathlib import Path
 
 from argx import Namespace
 from simpleconf import ProfileConfig
-from slugify import slugify
 from pipen import plugin
 from pipen.defaults import CONFIG_FILES
 from pipen.utils import copy_dict
 
 from .version import __version__
 from .parser_ import Parser
 
@@ -69,19 +68,19 @@
             "plugins",
         ):
             if getattr(parsed, key, None) is not None:
                 config[key] = getattr(parsed, key)
 
         if parsed.name not in (None, pipen.name):
             pipen.name = parsed.name
-            pipen.workdir = Path(config["workdir"]) / slugify(pipen.name)
+            pipen.workdir = Path(config["workdir"]) / pipen.name
             pipen.workdir.mkdir(parents=True, exist_ok=True)
             if parsed.outdir in (None, pipen_outdir):
                 pipen.outdir = Path(
-                    f"./{slugify(pipen.name)}_results"
+                    f"./{pipen.name}_results"
                 ).resolve()
 
         for key in ("plugin_opts", "template_opts", "scheduler_opts"):
             old = copy_dict(config[key] or {}, 3)
             old.update(getattr(parsed, key, None) or {})
             config[key] = old
 
@@ -142,10 +141,7 @@
             for key in ("plugin_opts", "scheduler_opts"):
                 if key in proc_args:
                     if proc_args[key]:
                         proc_opts = getattr(proc, key, None)
                         if proc_opts is None:
                             setattr(proc, key, {})
                         getattr(proc, key).update(proc_args[key])
-
-
-plugin.register(ArgsPlugin)
```

### Comparing `pipen_args-0.8.0/pipen_args/parser_.py` & `pipen_args-0.9.0/pipen_args/parser_.py`

 * *Files identical despite different names*

### Comparing `pipen_args-0.8.0/pipen_args/procgroup.py` & `pipen_args-0.9.0/pipen_args/procgroup.py`

 * *Files identical despite different names*

### Comparing `pipen_args-0.8.0/pyproject.toml` & `pipen_args-0.9.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 [tool.poetry]
 name = "pipen-args"
-version = "0.8.0"
+version = "0.9.0"
 description = "Command-line argument parser for pipen."
 authors = ["pwwang <pwwang@pwwang.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/pwwang/pipen-args"
 repository = "https://github.com/pwwang/pipen-args"
 
 [tool.poetry.build]
 generate-setup-file = true
 
 [tool.poetry.dependencies]
-python = "^3.7.1"
-pipen-annotate = "^0.6"
-# # required by xqute > pipen
-# diot = "^0.1"
+python = "^3.8"
+pipen-annotate = "^0.7.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7"
 pytest-cov = "^4"
 pytest-xdist = "^3"
 pytest-forked = "^1"
-pipen-verbose = "^0.5"
+pipen-verbose = "^0.6"
+
+[tool.poetry.plugins.pipen]
+args = "pipen_args.plugin:ArgsPlugin"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
 
 [tool.pytest.ini_options]
 addopts = "-v -n auto --cov pipen_args --cov-report xml:.coverage.xml --cov-report term-missing"
```

### Comparing `pipen_args-0.8.0/setup.py` & `pipen_args-0.9.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,27 +4,31 @@
 packages = \
 ['pipen_args']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['pipen-annotate>=0.6,<0.7']
+['pipen-annotate>=0.7.1,<0.8.0']
+
+entry_points = \
+{'pipen': ['args = pipen_args.plugin:ArgsPlugin']}
 
 setup_kwargs = {
     'name': 'pipen-args',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'Command-line argument parser for pipen.',
-    'long_description': '# pipen-args\n\nCommand line argument parser for [pipen][1]\n\n## Usage\n\n```python\nfrom pipen import Proc, Pipen\n# Note that unlike other plugins, you need to import install\n# to activate the plugin\nfrom pipen_args import install  # noqa: F401\n\nclass Process(Proc):\n    """My process\n\n    Input:\n        a: Input data\n    """\n    input = \'a\'\n    input_data = range(10)\n    script = \'echo {{in.a}}\'\n\nPipen().set_start(Process).run()\n```\n\n```shell\n$ python example.py --help\nUsage: test.py [-h | -h+] [options]\n\nUndescribed process.\nUse `@configfile` to load default values for the options.\n\nPipeline Options:\n  --name NAME           The name for the pipeline, will affect the default workdir and\n                        outdir. [default: pipen-0]\n  --profile PROFILE     The default profile from the configuration to run the pipeline.\n                        This profile will be used unless a profile is specified in the\n                        process or in the .run method of pipen. You can check the\n                        available profiles by running `pipen profile`\n  --outdir OUTDIR       The output directory of the pipeline [default: ./<name>_results]\n  --forks FORKS         How many jobs to run simultaneously by the scheduler\n  --scheduler SCHEDULER\n                        The scheduler to run the jobs\n\nNamespace <in>:\n  --in.a A [A ...]      Input data\n\nOptional Arguments:\n  -h, --help, -h+, --help+\n                        show help message (with + to show more options) and exit\n```\n\nSee more examples in `tests/pipelines/` folder.\n\n## Metadata for env items\n\nThe metadata in the docstring of env items determines how the arguments are defined.\n\n```python\nclass Process(Proc):\n    """My process\n\n    # other docstring sections\n\n    Envs:\n        a (<metadata>): ...\n```\n\nThe metadata could be key-value pairs separated by `;`. The separator `:` or `=` is used to\nseparate the key and value. The value is optional. If the value is not specified, it\nwill be set to `True`. The keys are valid arguments of `argx.ArgumentParser.add_argument`, except that `hidden` will be interpreted as `show=False` in `argx.ArgumentParser.add_argument`. If the value of `choices` is not specified, the subkeys of the env item will be used as the choices.\n\n[1]: https://github.com/pwwang/pipen\n',
+    'long_description': '# pipen-args\n\nCommand line argument parser for [pipen][1]\n\n## Usage\n\n```python\nfrom pipen import Proc, Pipen\n\n\nclass Process(Proc):\n    """My process\n\n    Input:\n        a: Input data\n    """\n    input = \'a\'\n    input_data = range(10)\n    script = \'echo {{in.a}}\'\n\nPipen().set_start(Process).run()\n```\n\n```shell\n$ python example.py --help\nUsage: test.py [-h | -h+] [options]\n\nUndescribed process.\nUse `@configfile` to load default values for the options.\n\nPipeline Options:\n  --name NAME           The name for the pipeline, will affect the default workdir and\n                        outdir. [default: pipen-0]\n  --profile PROFILE     The default profile from the configuration to run the pipeline.\n                        This profile will be used unless a profile is specified in the\n                        process or in the .run method of pipen. You can check the\n                        available profiles by running `pipen profile`\n  --outdir OUTDIR       The output directory of the pipeline [default: ./<name>_results]\n  --forks FORKS         How many jobs to run simultaneously by the scheduler\n  --scheduler SCHEDULER\n                        The scheduler to run the jobs\n\nNamespace <in>:\n  --in.a A [A ...]      Input data\n\nOptional Arguments:\n  -h, --help, -h+, --help+\n                        show help message (with + to show more options) and exit\n```\n\nSee more examples in `tests/pipelines/` folder.\n\n## Metadata for env items\n\nThe metadata in the docstring of env items determines how the arguments are defined.\n\n```python\nclass Process(Proc):\n    """My process\n\n    # other docstring sections\n\n    Envs:\n        a (<metadata>): ...\n```\n\nThe metadata could be key-value pairs separated by `;`. The separator `:` or `=` is used to\nseparate the key and value. The value is optional. If the value is not specified, it\nwill be set to `True`. The keys are valid arguments of `argx.ArgumentParser.add_argument`, except that `hidden` will be interpreted as `show=False` in `argx.ArgumentParser.add_argument`. If the value of `choices` is not specified, the subkeys of the env item will be used as the choices.\n\n[1]: https://github.com/pwwang/pipen\n',
     'author': 'pwwang',
     'author_email': 'pwwang@pwwang.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/pwwang/pipen-args',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.7.1,<4.0.0',
+    'entry_points': entry_points,
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `pipen_args-0.8.0/PKG-INFO` & `pipen_args-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 Metadata-Version: 2.1
 Name: pipen-args
-Version: 0.8.0
+Version: 0.9.0
 Summary: Command-line argument parser for pipen.
 Home-page: https://github.com/pwwang/pipen-args
 License: MIT
 Author: pwwang
 Author-email: pwwang@pwwang.com
-Requires-Python: >=3.7.1,<4.0.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pipen-annotate (>=0.6,<0.7)
+Requires-Dist: pipen-annotate (>=0.7.1,<0.8.0)
 Project-URL: Repository, https://github.com/pwwang/pipen-args
 Description-Content-Type: text/markdown
 
 # pipen-args
 
 Command line argument parser for [pipen][1]
 
 ## Usage
 
 ```python
 from pipen import Proc, Pipen
-# Note that unlike other plugins, you need to import install
-# to activate the plugin
-from pipen_args import install  # noqa: F401
+
 
 class Process(Proc):
     """My process
 
     Input:
         a: Input data
     """
```

