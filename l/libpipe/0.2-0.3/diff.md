# Comparing `tmp/libpipe-0.2.tar.gz` & `tmp/libpipe-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libpipe-0.2.tar", max compression
+gzip compressed data, was "libpipe-0.3.tar", max compression
```

## Comparing `libpipe-0.2.tar` & `libpipe-0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    35057 2020-04-03 15:29:02.397708 libpipe-0.2/LICENSE
--rw-r--r--   0        0        0      182 2020-04-29 09:53:09.881424 libpipe-0.2/README.md
--rw-r--r--   0        0        0      167 2021-04-30 12:59:43.682586 libpipe-0.2/libpipe/__init__.py
--rw-r--r--   0        0        0    10034 2020-04-23 10:11:29.322356 libpipe-0.2/libpipe/attrmap.py
--rw-r--r--   0        0        0     2739 2020-09-25 06:38:40.815433 libpipe-0.2/libpipe/futils.py
--rw-r--r--   0        0        0      242 2021-04-30 09:12:53.498588 libpipe-0.2/libpipe/msutils.py
--rw-r--r--   0        0        0     5345 2020-10-10 15:54:45.180432 libpipe-0.2/libpipe/settings.py
--rw-r--r--   0        0        0        0 2021-04-30 12:59:59.474670 libpipe-0.2/libpipe/tests/__init__.py
--rw-r--r--   0        0        0     1159 2020-04-06 12:52:20.961073 libpipe-0.2/libpipe/tests/settings_test.toml
--rw-r--r--   0        0        0     7525 2020-10-12 09:40:11.021388 libpipe-0.2/libpipe/tests/test_settings.py
--rw-r--r--   0        0        0     6373 2022-12-09 10:50:43.669298 libpipe-0.2/libpipe/tests/test_worker.py
--rw-r--r--   0        0        0        0 2020-06-14 14:48:49.404220 libpipe-0.2/libpipe/tools/__init__.py
--rw-r--r--   0        0        0      737 2020-12-17 09:21:00.875134 libpipe-0.2/libpipe/tools/libnodes_bash.sh
--rw-r--r--   0        0        0     4207 2023-02-12 14:13:30.531560 libpipe-0.2/libpipe/tools/nodetool.py
--rw-r--r--   0        0        0    18925 2023-02-12 14:12:48.155589 libpipe-0.2/libpipe/worker.py
--rw-r--r--   0        0        0      641 2023-02-12 14:21:02.667248 libpipe-0.2/pyproject.toml
--rw-r--r--   0        0        0     1149 1970-01-01 00:00:00.000000 libpipe-0.2/setup.py
--rw-r--r--   0        0        0     1162 1970-01-01 00:00:00.000000 libpipe-0.2/PKG-INFO
+-rw-r--r--   0        0        0    35057 2020-04-03 15:29:02.397708 libpipe-0.3/LICENSE
+-rw-r--r--   0        0        0      182 2020-04-29 09:53:09.881424 libpipe-0.3/README.md
+-rw-r--r--   0        0        0      167 2021-04-30 12:59:43.682586 libpipe-0.3/libpipe/__init__.py
+-rw-r--r--   0        0        0    10034 2020-04-23 10:11:29.322356 libpipe-0.3/libpipe/attrmap.py
+-rw-r--r--   0        0        0     2739 2020-09-25 06:38:40.815433 libpipe-0.3/libpipe/futils.py
+-rw-r--r--   0        0        0      242 2021-04-30 09:12:53.498588 libpipe-0.3/libpipe/msutils.py
+-rw-r--r--   0        0        0     5345 2020-10-10 15:54:45.180432 libpipe-0.3/libpipe/settings.py
+-rw-r--r--   0        0        0        0 2021-04-30 12:59:59.474670 libpipe-0.3/libpipe/tests/__init__.py
+-rw-r--r--   0        0        0     1159 2020-04-06 12:52:20.961073 libpipe-0.3/libpipe/tests/settings_test.toml
+-rw-r--r--   0        0        0     7525 2020-10-12 09:40:11.021388 libpipe-0.3/libpipe/tests/test_settings.py
+-rw-r--r--   0        0        0     7461 2023-04-14 16:24:06.234086 libpipe-0.3/libpipe/tests/test_worker.py
+-rw-r--r--   0        0        0        0 2020-06-14 14:48:49.404220 libpipe-0.3/libpipe/tools/__init__.py
+-rw-r--r--   0        0        0      737 2020-12-17 09:21:00.875134 libpipe-0.3/libpipe/tools/libnodes_bash.sh
+-rw-r--r--   0        0        0     4207 2023-02-12 14:13:30.531560 libpipe-0.3/libpipe/tools/nodetool.py
+-rw-r--r--   0        0        0    19429 2023-04-14 16:21:27.194166 libpipe-0.3/libpipe/worker.py
+-rw-r--r--   0        0        0      641 2023-04-14 16:26:28.926015 libpipe-0.3/pyproject.toml
+-rw-r--r--   0        0        0     1149 1970-01-01 00:00:00.000000 libpipe-0.3/setup.py
+-rw-r--r--   0        0        0     1162 1970-01-01 00:00:00.000000 libpipe-0.3/PKG-INFO
```

### Comparing `libpipe-0.2/LICENSE` & `libpipe-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `libpipe-0.2/libpipe/attrmap.py` & `libpipe-0.3/libpipe/attrmap.py`

 * *Files identical despite different names*

### Comparing `libpipe-0.2/libpipe/futils.py` & `libpipe-0.3/libpipe/futils.py`

 * *Files identical despite different names*

### Comparing `libpipe-0.2/libpipe/settings.py` & `libpipe-0.3/libpipe/settings.py`

 * *Files identical despite different names*

### Comparing `libpipe-0.2/libpipe/tests/settings_test.toml` & `libpipe-0.3/libpipe/tests/settings_test.toml`

 * *Files identical despite different names*

### Comparing `libpipe-0.2/libpipe/tests/test_settings.py` & `libpipe-0.3/libpipe/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `libpipe-0.2/libpipe/tests/test_worker.py` & `libpipe-0.3/libpipe/tests/test_worker.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import string
 import random
+import functools
 
 from unittest import mock
 
 from libpipe import worker
 
 
 def test_worker(tmp_path):
@@ -169,14 +170,45 @@
     success, errors = w.execute()
 
     assert len(success) == 1
     assert len(errors) == 0
     assert done
 
 
+def test_task_done_callback():
+    w = worker.WorkerPool([worker.localhost_shortname], 'Test', max_time=2)
+
+    done = 0
+
+    def callback(task):
+        print(task)
+        nonlocal done
+        assert isinstance(task, worker.Task)
+        if task.name == 'Error':
+            assert task.returncode == 1
+        else:    
+            assert task.returncode == 0
+        done += 1
+
+    def callback_with_extra(name, task):
+        assert name == 'test'
+        callback(task)
+
+    w.add('echo 0', task_done_callback=callback, name='Success1')
+    w.add('echo 0', task_done_callback=callback, name='Success2')
+    w.add('echo 3; cat non_existing_file', task_done_callback=functools.partial(callback_with_extra, 'test'), name='Error')
+    w.add('echo 4;', task_done_callback=functools.partial(callback_with_extra, 'test_err'), name='CBK Error')
+
+    success, errors = w.execute()
+
+    assert len(success) == 4
+    assert len(errors) == 0
+    assert done == 3
+
+
 class FakeSSHClient(worker.LocalClient):
 
     def __init__(self, host, user=None, force_sync=True, password=None):
         worker.LocalClient.__init__(self, force_sync=force_sync)
         self.host = host
 
     async def execute(self, task):
@@ -225,7 +257,13 @@
             if 'Done' in line:
                 has_done = True
 
     assert has_long_line
     assert has_done
     assert len(errors) == 0
     assert len(success) == 3
+
+
+def test_client():
+    client = worker.Client('localhost')
+
+    task = worker.Task('Check size', 'du -hs *')
```

### Comparing `libpipe-0.2/libpipe/tools/libnodes_bash.sh` & `libpipe-0.3/libpipe/tools/libnodes_bash.sh`

 * *Files identical despite different names*

### Comparing `libpipe-0.2/libpipe/tools/nodetool.py` & `libpipe-0.3/libpipe/tools/nodetool.py`

 * *Files identical despite different names*

### Comparing `libpipe-0.2/libpipe/worker.py` & `libpipe-0.3/libpipe/worker.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,31 +87,47 @@
     Attributes:
         name (str): Name of the task (set by the worker pool).
         command (str): Command
         output_file (str): Optional log file. None if not set.
         returncode (int): Return code. None if task was not executed.
     """
 
-    def __init__(self, name, command, output_file=None, done_callback=None, 
+    def __init__(self, name, command, output_file=None, done_callback=None, task_done_callback=None,
                  run_on_host=None, n_try=3, pid_filename=None, keep_pid_file_on_error=False):
         self.name = name
         self.command = command
         self.output_file = output_file
         self.fd = None
         self.returncode = None
         self.n_try = 0
-        self.done_callback = done_callback
+        self._done_callback = done_callback
+        self._task_done_callback = task_done_callback
         self.run_on_host = run_on_host
         self.status = TaskStatus.WAITING
         self.process = None
         self.n_try = n_try
         self.timed_out = False
         self.pid_filename = pid_filename
         self.keep_pid_file_on_error = keep_pid_file_on_error
 
+    def done_callback(self):
+        err_msg = ''
+        if self._done_callback is not None:
+            try:
+                self._done_callback()
+            except Exception as exc:
+                err_msg = f'Error executing return callback of task {self.name}: {str(exc)}\n'
+        if self._task_done_callback is not None:
+            try:
+                self._task_done_callback(self)
+            except Exception as exc:
+                err_msg = f'Error executing return callback of task {self.name}: {str(exc)}\n'
+
+        return err_msg
+
     def init_log(self):
         if self.output_file is not None:
             self.fd = open(self.output_file, 'w')
             self.fd.write(f'# Logging starting at {datetime.datetime.now()}\n')
             self.fd.write(f'# Input command: {self.command}\n')
 
     def set_process(self, process):
@@ -338,19 +354,15 @@
             err_msg = f'Task {self.name} has been canceled\n'
             return True, err_msg
         except Exception as exc:
             err_msg = f'Error executing task {self.name}: {str(exc)}\n'
             self.status = WorkerStatus.IDLE
             return False, err_msg
 
-        if task.done_callback is not None:
-            try:
-                task.done_callback()
-            except Exception as exc:
-                err_msg = f'Error executing return callback of task {self.name}: {str(exc)}\n'
+        err_msg = task.done_callback()
 
         self.status = WorkerStatus.IDLE
 
         return True, err_msg
 
     def close(self):
         self.status = WorkerStatus.CLOSED
@@ -417,15 +429,15 @@
                         host = None
                     continue
                 if worker.status is WorkerStatus.IDLE:
                     worker.status = WorkerStatus.COMMITED
                     return worker
             await asyncio.sleep(0.1)
 
-    def add(self, command, name=None, output_file=None, done_callback=None, 
+    def add(self, command, name=None, output_file=None, task_done_callback=None, done_callback=None, 
             run_on_host=None, n_try=3, pid_filename=None, keep_pid_file_on_error=False):
         """Add a command to execute by a worker in the pool. Optionally output result in output_file.
 
         Args:
             command (str): Command to execute.
             name (str, optional): Name of the task. If not set it will be set by the worker pool
             output_file (str, optional): Optional filename to log output into.
@@ -443,16 +455,16 @@
 
         if self.debug:
             print(command)
         if self.dry_run:
             return
 
         self.tasks.append(Task(name, command, output_file=output_file, done_callback=done_callback,
-                               run_on_host=run_on_host, n_try=n_try, pid_filename=pid_filename, 
-                               keep_pid_file_on_error=keep_pid_file_on_error))
+                               task_done_callback=task_done_callback, run_on_host=run_on_host, n_try=n_try, 
+                               pid_filename=pid_filename, keep_pid_file_on_error=keep_pid_file_on_error))
 
     def get_all_tasks(self):
         tasks = collections.defaultdict(list)
         for t in self.tasks:
             tasks[t.status].append(t)
         return tasks
```

### Comparing `libpipe-0.2/pyproject.toml` & `libpipe-0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "libpipe"
-version = "0.2"
+version = "0.3"
 description = ""
 authors = ["\"Florent Mertens\" <\"florent.mertens@gmail.com\">"]
 license = "GPL-3.0-or-later"
 readme = 'README.md'
 repository = "https://gitlab.com/flomertens/libpipe"
 
 [tool.poetry.dependencies]
```

### Comparing `libpipe-0.2/setup.py` & `libpipe-0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 {':python_version < "3.8"': ['importlib-metadata>=1.0,<2.0']}
 
 entry_points = \
 {'console_scripts': ['nodetool = libpipe.tools.nodetool:main']}
 
 setup_kwargs = {
     'name': 'libpipe',
-    'version': '0.2',
+    'version': '0.3',
     'description': '',
     'long_description': 'Libpipe\n=======\n\nCommon pipeline framework and library\n\nInstallation\n------------\n\nlibpipe can be installed via pip:\n\n    $ pip install libpipe\n\nand requires Python 3.6.0 or higher.\n',
     'author': '"Florent Mertens"',
     'author_email': '"florent.mertens@gmail.com"',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://gitlab.com/flomertens/libpipe',
```

### Comparing `libpipe-0.2/PKG-INFO` & `libpipe-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libpipe
-Version: 0.2
+Version: 0.3
 Summary: 
 Home-page: https://gitlab.com/flomertens/libpipe
 License: GPL-3.0-or-later
 Author: "Florent Mertens"
 Author-email: "florent.mertens@gmail.com"
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

