# Comparing `tmp/mypy_baseline-0.4.5.tar.gz` & `tmp/mypy_baseline-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy_baseline-0.4.5.tar", last modified: Fri Mar 10 09:22:25 2023, max compression
+gzip compressed data, was "mypy_baseline-0.5.0.tar", last modified: Fri Apr 14 07:15:23 2023, max compression
```

## Comparing `mypy_baseline-0.4.5.tar` & `mypy_baseline-0.5.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0      654 2023-02-24 08:10:15.428694 mypy_baseline-0.4.5/.github/workflows/main.yml
--rw-r--r--   0        0        0      108 2023-02-21 08:54:27.062504 mypy_baseline-0.4.5/.gitignore
--rw-r--r--   0        0        0      325 2023-02-24 08:10:15.428694 mypy_baseline-0.4.5/.markdownlint.yaml
--rw-r--r--   0        0        0     1048 2022-09-01 10:06:03.899566 mypy_baseline-0.4.5/LICENSE
--rw-r--r--   0        0        0     1946 2023-02-21 08:54:27.062504 mypy_baseline-0.4.5/README.md
--rw-r--r--   0        0        0     3448 2023-02-21 08:54:27.062504 mypy_baseline-0.4.5/Taskfile.yml
--rw-r--r--   0        0        0   127812 2022-09-28 08:10:05.956227 mypy_baseline-0.4.5/assets/example.png
--rw-r--r--   0        0        0   180974 2022-10-01 08:47:06.040486 mypy_baseline-0.4.5/assets/history.png
--rw-r--r--   0        0        0      326 2023-02-21 08:54:27.062504 mypy_baseline-0.4.5/docs/conf.py
--rw-r--r--   0        0        0      811 2023-02-21 08:54:27.062504 mypy_baseline-0.4.5/docs/config.md
--rw-r--r--   0        0        0      512 2023-02-21 08:54:27.062504 mypy_baseline-0.4.5/docs/filter.md
--rw-r--r--   0        0        0     4410 2023-02-27 13:02:41.839663 mypy_baseline-0.4.5/docs/follower.md
--rw-r--r--   0        0        0      852 2023-02-21 08:54:27.062504 mypy_baseline-0.4.5/docs/history.md
--rw-r--r--   0        0        0      486 2023-02-24 08:04:06.077059 mypy_baseline-0.4.5/docs/index.md
--rw-r--r--   0        0        0     4341 2023-02-21 08:54:27.062504 mypy_baseline-0.4.5/docs/leader.md
--rw-r--r--   0        0        0      377 2023-02-21 08:54:27.062504 mypy_baseline-0.4.5/docs/plot.md
--rw-r--r--   0        0        0     1297 2023-02-27 12:49:23.969584 mypy_baseline-0.4.5/docs/suggest.md
--rw-r--r--   0        0        0      973 2023-02-21 08:54:27.062504 mypy_baseline-0.4.5/docs/sync.md
--rw-r--r--   0        0        0      540 2023-02-21 08:54:27.062504 mypy_baseline-0.4.5/docs/top-files.md
--rw-r--r--   0        0        0       74 2023-02-21 08:54:27.062504 mypy_baseline-0.4.5/docs/usage.md
--rw-r--r--   0        0        0      139 2023-03-10 09:22:19.906984 mypy_baseline-0.4.5/mypy_baseline/__init__.py
--rw-r--r--   0        0        0       44 2022-09-28 08:10:05.956227 mypy_baseline-0.4.5/mypy_baseline/__main__.py
--rw-r--r--   0        0        0      912 2022-09-28 08:10:05.956227 mypy_baseline-0.4.5/mypy_baseline/_cli.py
--rw-r--r--   0        0        0     2200 2022-10-08 07:27:10.462038 mypy_baseline-0.4.5/mypy_baseline/_colors.py
--rw-r--r--   0        0        0     4042 2023-02-24 08:04:06.077059 mypy_baseline-0.4.5/mypy_baseline/_config.py
--rw-r--r--   0        0        0     1878 2023-02-25 08:14:48.947572 mypy_baseline-0.4.5/mypy_baseline/_error.py
--rw-r--r--   0        0        0     2370 2022-10-08 07:27:10.462038 mypy_baseline-0.4.5/mypy_baseline/_git.py
--rw-r--r--   0        0        0      583 2023-02-24 08:04:06.077059 mypy_baseline-0.4.5/mypy_baseline/commands/__init__.py
--rw-r--r--   0        0        0      870 2022-10-26 09:21:57.066380 mypy_baseline-0.4.5/mypy_baseline/commands/_base.py
--rw-r--r--   0        0        0     3532 2022-11-05 08:39:22.834206 mypy_baseline-0.4.5/mypy_baseline/commands/_filter.py
--rw-r--r--   0        0        0     1219 2022-10-08 07:27:10.462038 mypy_baseline-0.4.5/mypy_baseline/commands/_history.py
--rw-r--r--   0        0        0     1514 2023-02-20 10:17:46.003690 mypy_baseline-0.4.5/mypy_baseline/commands/_plot.py
--rw-r--r--   0        0        0     7674 2023-03-10 09:22:19.906984 mypy_baseline-0.4.5/mypy_baseline/commands/_suggest.py
--rw-r--r--   0        0        0     2167 2022-11-05 08:39:22.834206 mypy_baseline-0.4.5/mypy_baseline/commands/_sync.py
--rw-r--r--   0        0        0     1508 2023-02-20 10:21:07.493456 mypy_baseline-0.4.5/mypy_baseline/commands/_top_files.py
--rw-r--r--   0        0        0      384 2022-09-28 08:10:05.960227 mypy_baseline-0.4.5/mypy_baseline/commands/_version.py
--rw-r--r--   0        0        0        0 2022-09-01 10:06:03.903566 mypy_baseline-0.4.5/mypy_baseline/py.typed
--rwxr-xr-x   0        0        0      147 2023-02-21 08:54:27.062504 mypy_baseline-0.4.5/netlify.sh
--rw-r--r--   0        0        0       95 2023-02-21 08:54:27.062504 mypy_baseline-0.4.5/netlify.toml
--rw-r--r--   0        0        0     1690 2023-02-27 12:49:23.969584 mypy_baseline-0.4.5/pyproject.toml
--rw-r--r--   0        0        0       66 2023-02-21 08:54:27.062504 mypy_baseline-0.4.5/setup.cfg
--rw-r--r--   0        0        0        0 2022-09-01 10:06:03.903566 mypy_baseline-0.4.5/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-02-24 08:04:06.077059 mypy_baseline-0.4.5/tests/test_commands/__init__.py
--rw-r--r--   0        0        0      438 2023-03-10 09:22:19.906984 mypy_baseline-0.4.5/tests/test_commands/helpers.py
--rw-r--r--   0        0        0      690 2023-02-24 08:04:06.081059 mypy_baseline-0.4.5/tests/test_commands/test_filter.py
--rw-r--r--   0        0        0      416 2023-02-24 08:04:06.081059 mypy_baseline-0.4.5/tests/test_commands/test_history.py
--rw-r--r--   0        0        0     3453 2023-03-10 09:22:19.906984 mypy_baseline-0.4.5/tests/test_commands/test_suggest.py
--rw-r--r--   0        0        0      615 2023-02-24 08:04:06.081059 mypy_baseline-0.4.5/tests/test_commands/test_sync.py
--rw-r--r--   0        0        0      375 2023-02-24 08:04:06.081059 mypy_baseline-0.4.5/tests/test_commands/test_top_files.py
--rw-r--r--   0        0        0      147 2023-02-24 08:04:06.081059 mypy_baseline-0.4.5/tests/test_commands/test_version.py
--rw-r--r--   0        0        0     1574 2022-09-28 08:10:05.960227 mypy_baseline-0.4.5/tests/test_error.py
--rw-r--r--   0        0        0     3060 1970-01-01 00:00:00.000000 mypy_baseline-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0      654 2023-02-24 08:10:15.428694 mypy_baseline-0.5.0/.github/workflows/main.yml
+-rw-r--r--   0        0        0      108 2023-02-21 08:54:27.062504 mypy_baseline-0.5.0/.gitignore
+-rw-r--r--   0        0        0      325 2023-02-24 08:10:15.428694 mypy_baseline-0.5.0/.markdownlint.yaml
+-rw-r--r--   0        0        0     1048 2022-09-01 10:06:03.899566 mypy_baseline-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1946 2023-04-14 07:02:53.049087 mypy_baseline-0.5.0/README.md
+-rw-r--r--   0        0        0     3448 2023-02-21 08:54:27.062504 mypy_baseline-0.5.0/Taskfile.yml
+-rw-r--r--   0        0        0   127812 2022-09-28 08:10:05.956227 mypy_baseline-0.5.0/assets/example.png
+-rw-r--r--   0        0        0   180974 2022-10-01 08:47:06.040486 mypy_baseline-0.5.0/assets/history.png
+-rw-r--r--   0        0        0      326 2023-02-21 08:54:27.062504 mypy_baseline-0.5.0/docs/conf.py
+-rw-r--r--   0        0        0      811 2023-02-21 08:54:27.062504 mypy_baseline-0.5.0/docs/config.md
+-rw-r--r--   0        0        0      512 2023-04-14 07:08:04.277478 mypy_baseline-0.5.0/docs/filter.md
+-rw-r--r--   0        0        0     4410 2023-02-27 13:02:41.839663 mypy_baseline-0.5.0/docs/follower.md
+-rw-r--r--   0        0        0      852 2023-02-21 08:54:27.062504 mypy_baseline-0.5.0/docs/history.md
+-rw-r--r--   0        0        0      486 2023-02-24 08:04:06.077059 mypy_baseline-0.5.0/docs/index.md
+-rw-r--r--   0        0        0     4341 2023-02-21 08:54:27.062504 mypy_baseline-0.5.0/docs/leader.md
+-rw-r--r--   0        0        0      377 2023-02-21 08:54:27.062504 mypy_baseline-0.5.0/docs/plot.md
+-rw-r--r--   0        0        0     1297 2023-02-27 12:49:23.969584 mypy_baseline-0.5.0/docs/suggest.md
+-rw-r--r--   0        0        0     1202 2023-04-14 07:15:00.364969 mypy_baseline-0.5.0/docs/sync.md
+-rw-r--r--   0        0        0      540 2023-02-21 08:54:27.062504 mypy_baseline-0.5.0/docs/top-files.md
+-rw-r--r--   0        0        0       74 2023-02-21 08:54:27.062504 mypy_baseline-0.5.0/docs/usage.md
+-rw-r--r--   0        0        0      139 2023-04-14 07:15:00.364969 mypy_baseline-0.5.0/mypy_baseline/__init__.py
+-rw-r--r--   0        0        0       44 2022-09-28 08:10:05.956227 mypy_baseline-0.5.0/mypy_baseline/__main__.py
+-rw-r--r--   0        0        0      912 2022-09-28 08:10:05.956227 mypy_baseline-0.5.0/mypy_baseline/_cli.py
+-rw-r--r--   0        0        0     2200 2022-10-08 07:27:10.462038 mypy_baseline-0.5.0/mypy_baseline/_colors.py
+-rw-r--r--   0        0        0     4042 2023-02-24 08:04:06.077059 mypy_baseline-0.5.0/mypy_baseline/_config.py
+-rw-r--r--   0        0        0     2311 2023-04-14 07:15:00.364969 mypy_baseline-0.5.0/mypy_baseline/_error.py
+-rw-r--r--   0        0        0     2370 2022-10-08 07:27:10.462038 mypy_baseline-0.5.0/mypy_baseline/_git.py
+-rw-r--r--   0        0        0      583 2023-02-24 08:04:06.077059 mypy_baseline-0.5.0/mypy_baseline/commands/__init__.py
+-rw-r--r--   0        0        0      870 2022-10-26 09:21:57.066380 mypy_baseline-0.5.0/mypy_baseline/commands/_base.py
+-rw-r--r--   0        0        0     3532 2022-11-05 08:39:22.834206 mypy_baseline-0.5.0/mypy_baseline/commands/_filter.py
+-rw-r--r--   0        0        0     1219 2022-10-08 07:27:10.462038 mypy_baseline-0.5.0/mypy_baseline/commands/_history.py
+-rw-r--r--   0        0        0     1514 2023-02-20 10:17:46.003690 mypy_baseline-0.5.0/mypy_baseline/commands/_plot.py
+-rw-r--r--   0        0        0     7674 2023-03-10 09:22:19.906984 mypy_baseline-0.5.0/mypy_baseline/commands/_suggest.py
+-rw-r--r--   0        0        0     2167 2022-11-05 08:39:22.834206 mypy_baseline-0.5.0/mypy_baseline/commands/_sync.py
+-rw-r--r--   0        0        0     1508 2023-02-20 10:21:07.493456 mypy_baseline-0.5.0/mypy_baseline/commands/_top_files.py
+-rw-r--r--   0        0        0      384 2022-09-28 08:10:05.960227 mypy_baseline-0.5.0/mypy_baseline/commands/_version.py
+-rw-r--r--   0        0        0        0 2022-09-01 10:06:03.903566 mypy_baseline-0.5.0/mypy_baseline/py.typed
+-rwxr-xr-x   0        0        0      147 2023-02-21 08:54:27.062504 mypy_baseline-0.5.0/netlify.sh
+-rw-r--r--   0        0        0       95 2023-02-21 08:54:27.062504 mypy_baseline-0.5.0/netlify.toml
+-rw-r--r--   0        0        0     1690 2023-02-27 12:49:23.969584 mypy_baseline-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0       66 2023-02-21 08:54:27.062504 mypy_baseline-0.5.0/setup.cfg
+-rw-r--r--   0        0        0        0 2022-09-01 10:06:03.903566 mypy_baseline-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-24 08:04:06.077059 mypy_baseline-0.5.0/tests/test_commands/__init__.py
+-rw-r--r--   0        0        0      698 2023-04-14 07:15:00.368969 mypy_baseline-0.5.0/tests/test_commands/helpers.py
+-rw-r--r--   0        0        0     1103 2023-04-14 07:15:00.368969 mypy_baseline-0.5.0/tests/test_commands/test_filter.py
+-rw-r--r--   0        0        0      416 2023-02-24 08:04:06.081059 mypy_baseline-0.5.0/tests/test_commands/test_history.py
+-rw-r--r--   0        0        0     3453 2023-03-10 09:22:19.906984 mypy_baseline-0.5.0/tests/test_commands/test_suggest.py
+-rw-r--r--   0        0        0     1086 2023-04-14 07:15:00.368969 mypy_baseline-0.5.0/tests/test_commands/test_sync.py
+-rw-r--r--   0        0        0      637 2023-04-14 07:15:00.368969 mypy_baseline-0.5.0/tests/test_commands/test_top_files.py
+-rw-r--r--   0        0        0      147 2023-02-24 08:04:06.081059 mypy_baseline-0.5.0/tests/test_commands/test_version.py
+-rw-r--r--   0        0        0     1574 2022-09-28 08:10:05.960227 mypy_baseline-0.5.0/tests/test_error.py
+-rw-r--r--   0        0        0     3060 1970-01-01 00:00:00.000000 mypy_baseline-0.5.0/PKG-INFO
```

### Comparing `mypy_baseline-0.4.5/.github/workflows/main.yml` & `mypy_baseline-0.5.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.4.5/LICENSE` & `mypy_baseline-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.4.5/README.md` & `mypy_baseline-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.4.5/Taskfile.yml` & `mypy_baseline-0.5.0/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.4.5/assets/example.png` & `mypy_baseline-0.5.0/assets/example.png`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.4.5/assets/history.png` & `mypy_baseline-0.5.0/assets/history.png`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.4.5/docs/config.md` & `mypy_baseline-0.5.0/docs/config.md`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.4.5/docs/filter.md` & `mypy_baseline-0.5.0/docs/filter.md`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.4.5/docs/follower.md` & `mypy_baseline-0.5.0/docs/follower.md`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.4.5/docs/history.md` & `mypy_baseline-0.5.0/docs/history.md`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.4.5/docs/leader.md` & `mypy_baseline-0.5.0/docs/leader.md`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.4.5/docs/suggest.md` & `mypy_baseline-0.5.0/docs/suggest.md`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.4.5/docs/sync.md` & `mypy_baseline-0.5.0/docs/sync.md`

 * *Files 12% similar despite different names*

```diff
@@ -5,7 +5,16 @@
 ```bash
 mypy | mypy-baseline sync
 ```
 
 The baseline file (`mypy-baseline.txt` by default) contains all errors that mypy spits out with line numbers replaced with zeros and colors removed. All errors recorded in the baseline will be filtered out from the future mypy runs by `mypy-baseline filter`.
 
 The lines in the baseline come in the same order as mypy produeces them. This order is fragile, and the order of files analyzed (and so the lines in the baseline) might change as the dependency graph between modules changes and even be different on different machines. When syncing the changes with an existing baseline, we try to preserve the lines order there, but sometimes it cannot be done, and the lines may jump around. If that causes merge conflicts, simply re-run `sync` instead of trying to fix conflicts manually.
+
+## Jupyter notebooks
+
+All mypy-baseline commands support [nbQA](https://github.com/nbQA-dev/nbQA) for checking [Jupyter notebooks](https://jupyter.org/):
+
+```bash
+python3 -m pip install nbqa
+nbqa mypy . | mypy-baseline sync
+```
```

### Comparing `mypy_baseline-0.4.5/docs/top-files.md` & `mypy_baseline-0.5.0/docs/top-files.md`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.4.5/mypy_baseline/_cli.py` & `mypy_baseline-0.5.0/mypy_baseline/_cli.py`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.4.5/mypy_baseline/_colors.py` & `mypy_baseline-0.5.0/mypy_baseline/_colors.py`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.4.5/mypy_baseline/_config.py` & `mypy_baseline-0.5.0/mypy_baseline/_config.py`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.4.5/mypy_baseline/_error.py` & `mypy_baseline-0.5.0/mypy_baseline/_error.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,35 +6,49 @@
 from pathlib import Path
 from typing import TYPE_CHECKING
 
 
 if TYPE_CHECKING:
     from ._config import Config
 
-COLOR_PATTERN = '(\x1b\\[\\d*m?|\x0f)*'
-REX_COLOR = re.compile(COLOR_PATTERN)
-REX_LINE = re.compile(rf"""
+REX_COLOR = re.compile('(\x1b\\[\\d*m?|\x0f)*')
+REX_COLOR_NBQA = re.compile(r'\[\d*m|\x1b|\(B')
+REX_LINE = re.compile(r"""
     (?P<path>.+\.py):
     (?P<lineno>[0-9]+):\s
-    {COLOR_PATTERN}(?P<severity>[a-z]+):{COLOR_PATTERN}\s
+    (?P<severity>[a-z]+):\s
     (?P<message>.+?)
-    (?:\s\s{COLOR_PATTERN}\[(?P<category>[a-z-]+)\]{COLOR_PATTERN})?
+    (?:\s\s\[(?P<category>[a-z-]+)\])?
+    \s*
+""", re.VERBOSE | re.MULTILINE)
+REX_LINE_NBQA = re.compile(r"""
+    (?P<path>.+\.ipynb:cell_[0-9]+):
+    (?P<lineno>[0-9]+):\s
+    (?P<severity>[a-z]+):\s
+    (?P<message>.+?)
+    (?:\s\s\[(?P<category>[a-z-]+)\])?
     \s*
 """, re.VERBOSE | re.MULTILINE)
 REX_LINE_IN_MSG = re.compile(r'defined on line \d+')
 
 
+def _remove_color_codes(line: str) -> str:
+    line = REX_COLOR.sub('', line)
+    return REX_COLOR_NBQA.sub('', line)
+
+
 @dataclass
 class Error:
     raw_line: str
     _match: re.Match[str]
 
     @classmethod
     def new(self, line: str) -> Error | None:
-        match = REX_LINE.fullmatch(line)
+        line = _remove_color_codes(line)
+        match = REX_LINE.fullmatch(line) or REX_LINE_NBQA.fullmatch(line)
         if match is None:
             return None
         return Error(line, match)
 
     @cached_property
     def path(self) -> Path:
         return Path(self._match.group('path'))
@@ -57,12 +71,13 @@
     def category(self) -> str:
         return self._match.group('category') or 'note'
 
     def get_clean_line(self, config: Config) -> str:
         path = Path(*self.path.parts[:config.depth])
         pos = self.line_number if config.preserve_position else 0
         msg = REX_COLOR.sub('', self.message).strip()
+        msg = REX_COLOR_NBQA.sub('', self.message).strip()
         msg = REX_LINE_IN_MSG.sub('defined on line 0', msg)
         line = f'{path}:{pos}: {self.severity}: {msg}'
         if self.category != 'note':
             line += f'  [{self.category}]'
         return line
```

### Comparing `mypy_baseline-0.4.5/mypy_baseline/_git.py` & `mypy_baseline-0.5.0/mypy_baseline/_git.py`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.4.5/mypy_baseline/commands/__init__.py` & `mypy_baseline-0.5.0/mypy_baseline/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.4.5/mypy_baseline/commands/_base.py` & `mypy_baseline-0.5.0/mypy_baseline/commands/_base.py`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.4.5/mypy_baseline/commands/_filter.py` & `mypy_baseline-0.5.0/mypy_baseline/commands/_filter.py`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.4.5/mypy_baseline/commands/_history.py` & `mypy_baseline-0.5.0/mypy_baseline/commands/_history.py`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.4.5/mypy_baseline/commands/_plot.py` & `mypy_baseline-0.5.0/mypy_baseline/commands/_plot.py`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.4.5/mypy_baseline/commands/_suggest.py` & `mypy_baseline-0.5.0/mypy_baseline/commands/_suggest.py`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.4.5/mypy_baseline/commands/_sync.py` & `mypy_baseline-0.5.0/mypy_baseline/commands/_sync.py`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.4.5/mypy_baseline/commands/_top_files.py` & `mypy_baseline-0.5.0/mypy_baseline/commands/_top_files.py`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.4.5/pyproject.toml` & `mypy_baseline-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.4.5/tests/test_commands/test_filter.py` & `mypy_baseline-0.5.0/tests/test_commands/test_filter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from io import StringIO
 
 from mypy_baseline import main
 
-from .helpers import LINE1, LINE2, run
+from .helpers import LINE1, LINE2, NOTEBOOK_LINE1, run
 
 
 def test_filter():
     stdin = StringIO()
     stdin.write(LINE1)
     stdin.write(LINE2)
     stdin.seek(0)
@@ -21,10 +21,26 @@
     assert LINE2.strip() in actual
     assert '  assignment  ' in actual
     assert '  union-attr  ' in actual
     assert '  unresolved' in actual
     assert 'Your changes introduced' in actual
 
 
+def test_filter_notebook():
+    stdin = StringIO()
+    stdin.write(NOTEBOOK_LINE1)
+
+    stdin.seek(0)
+    stdout = StringIO()
+    code = main(['filter'], stdin, stdout)
+    assert code == 1
+    stdout.seek(0)
+    actual = stdout.read()
+    assert NOTEBOOK_LINE1 in actual
+    assert '  return-value  ' in actual
+    assert '  unresolved' in actual
+    assert 'Your changes introduced' in actual
+
+
 def test_filter__empty_stdin():
     actual = run(['filter'])
     assert actual == ''
```

### Comparing `mypy_baseline-0.4.5/tests/test_commands/test_suggest.py` & `mypy_baseline-0.5.0/tests/test_commands/test_suggest.py`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.4.5/tests/test_error.py` & `mypy_baseline-0.5.0/tests/test_error.py`

 * *Files identical despite different names*

### Comparing `mypy_baseline-0.4.5/PKG-INFO` & `mypy_baseline-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mypy_baseline
-Version: 0.4.5
+Version: 0.5.0
 Summary: Integrate mypy with existing codebase.
 Keywords: mypy,typing,annotations,type annotations
 Author-email: Gram <git@orsinium.dev>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

