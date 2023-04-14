# Comparing `tmp/gravity-1.0.2.tar.gz` & `tmp/gravity-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gravity-1.0.2.tar", last modified: Tue Mar 28 16:50:33 2023, max compression
+gzip compressed data, was "gravity-1.0.3.tar", last modified: Fri Apr 14 15:41:12 2023, max compression
```

## Comparing `gravity-1.0.2.tar` & `gravity-1.0.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 16:50:33.540325 gravity-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     9208 2023-03-28 16:50:23.000000 gravity-1.0.2/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-03-28 16:50:23.000000 gravity-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-28 16:50:23.000000 gravity-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13491 2023-03-28 16:50:33.540325 gravity-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-03-28 16:50:23.000000 gravity-1.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 16:50:33.532325 gravity-1.0.2/gravity/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-28 16:50:23.000000 gravity-1.0.2/gravity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-03-28 16:50:23.000000 gravity-1.0.2/gravity/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 16:50:33.536325 gravity-1.0.2/gravity/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 16:50:23.000000 gravity-1.0.2/gravity/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-03-28 16:50:23.000000 gravity-1.0.2/gravity/commands/cmd_exec.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-03-28 16:50:23.000000 gravity-1.0.2/gravity/commands/cmd_follow.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-03-28 16:50:23.000000 gravity-1.0.2/gravity/commands/cmd_graceful.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-03-28 16:50:23.000000 gravity-1.0.2/gravity/commands/cmd_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-03-28 16:50:23.000000 gravity-1.0.2/gravity/commands/cmd_pm.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-03-28 16:50:23.000000 gravity-1.0.2/gravity/commands/cmd_restart.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-03-28 16:50:23.000000 gravity-1.0.2/gravity/commands/cmd_show.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-03-28 16:50:23.000000 gravity-1.0.2/gravity/commands/cmd_shutdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-03-28 16:50:23.000000 gravity-1.0.2/gravity/commands/cmd_start.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-03-28 16:50:23.000000 gravity-1.0.2/gravity/commands/cmd_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-03-28 16:50:23.000000 gravity-1.0.2/gravity/commands/cmd_stop.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-03-28 16:50:23.000000 gravity-1.0.2/gravity/commands/cmd_update.py
--rw-r--r--   0 runner    (1001) docker     (123)    18413 2023-03-28 16:50:23.000000 gravity-1.0.2/gravity/config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-03-28 16:50:23.000000 gravity-1.0.2/gravity/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-03-28 16:50:23.000000 gravity-1.0.2/gravity/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 16:50:33.540325 gravity-1.0.2/gravity/process_manager/
--rw-r--r--   0 runner    (1001) docker     (123)    15469 2023-03-28 16:50:23.000000 gravity-1.0.2/gravity/process_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19136 2023-03-28 16:50:23.000000 gravity-1.0.2/gravity/process_manager/supervisor.py
--rw-r--r--   0 runner    (1001) docker     (123)    16689 2023-03-28 16:50:23.000000 gravity-1.0.2/gravity/process_manager/systemd.py
--rw-r--r--   0 runner    (1001) docker     (123)    19274 2023-03-28 16:50:23.000000 gravity-1.0.2/gravity/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    20454 2023-03-28 16:50:23.000000 gravity-1.0.2/gravity/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 16:50:33.540325 gravity-1.0.2/gravity/util/
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-03-28 16:50:23.000000 gravity-1.0.2/gravity/util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 16:50:33.536325 gravity-1.0.2/gravity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13491 2023-03-28 16:50:33.000000 gravity-1.0.2/gravity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-03-28 16:50:33.000000 gravity-1.0.2/gravity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 16:50:33.000000 gravity-1.0.2/gravity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-28 16:50:33.000000 gravity-1.0.2/gravity.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 16:50:33.000000 gravity-1.0.2/gravity.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-28 16:50:33.000000 gravity-1.0.2/gravity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-28 16:50:33.000000 gravity-1.0.2/gravity.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-03-28 16:50:23.000000 gravity-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-28 16:50:33.540325 gravity-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-03-28 16:50:23.000000 gravity-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 16:50:33.540325 gravity-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-03-28 16:50:23.000000 gravity-1.0.2/tests/test_config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    11256 2023-03-28 16:50:23.000000 gravity-1.0.2/tests/test_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)    25130 2023-03-28 16:50:23.000000 gravity-1.0.2/tests/test_process_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-03-28 16:50:23.000000 gravity-1.0.2/tests/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:41:12.468332 gravity-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-04-14 15:41:02.000000 gravity-1.0.3/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-14 15:41:02.000000 gravity-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-14 15:41:02.000000 gravity-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13671 2023-04-14 15:41:12.468332 gravity-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-04-14 15:41:02.000000 gravity-1.0.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:41:12.464331 gravity-1.0.3/gravity/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-14 15:41:02.000000 gravity-1.0.3/gravity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-04-14 15:41:02.000000 gravity-1.0.3/gravity/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:41:12.468332 gravity-1.0.3/gravity/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:41:02.000000 gravity-1.0.3/gravity/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-14 15:41:02.000000 gravity-1.0.3/gravity/commands/cmd_exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-14 15:41:02.000000 gravity-1.0.3/gravity/commands/cmd_follow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-14 15:41:02.000000 gravity-1.0.3/gravity/commands/cmd_graceful.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-14 15:41:02.000000 gravity-1.0.3/gravity/commands/cmd_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-14 15:41:02.000000 gravity-1.0.3/gravity/commands/cmd_pm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-14 15:41:02.000000 gravity-1.0.3/gravity/commands/cmd_restart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-14 15:41:02.000000 gravity-1.0.3/gravity/commands/cmd_show.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-14 15:41:02.000000 gravity-1.0.3/gravity/commands/cmd_shutdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-04-14 15:41:02.000000 gravity-1.0.3/gravity/commands/cmd_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-14 15:41:02.000000 gravity-1.0.3/gravity/commands/cmd_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-14 15:41:02.000000 gravity-1.0.3/gravity/commands/cmd_stop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-14 15:41:02.000000 gravity-1.0.3/gravity/commands/cmd_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18413 2023-04-14 15:41:02.000000 gravity-1.0.3/gravity/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-14 15:41:02.000000 gravity-1.0.3/gravity/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-14 15:41:02.000000 gravity-1.0.3/gravity/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:41:12.468332 gravity-1.0.3/gravity/process_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)    15664 2023-04-14 15:41:02.000000 gravity-1.0.3/gravity/process_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19143 2023-04-14 15:41:02.000000 gravity-1.0.3/gravity/process_manager/supervisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16689 2023-04-14 15:41:02.000000 gravity-1.0.3/gravity/process_manager/systemd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19274 2023-04-14 15:41:02.000000 gravity-1.0.3/gravity/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20454 2023-04-14 15:41:02.000000 gravity-1.0.3/gravity/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:41:12.468332 gravity-1.0.3/gravity/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-04-14 15:41:02.000000 gravity-1.0.3/gravity/util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:41:12.464331 gravity-1.0.3/gravity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13671 2023-04-14 15:41:12.000000 gravity-1.0.3/gravity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-14 15:41:12.000000 gravity-1.0.3/gravity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 15:41:12.000000 gravity-1.0.3/gravity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-14 15:41:12.000000 gravity-1.0.3/gravity.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 15:41:12.000000 gravity-1.0.3/gravity.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-14 15:41:12.000000 gravity-1.0.3/gravity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 15:41:12.000000 gravity-1.0.3/gravity.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-14 15:41:02.000000 gravity-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-14 15:41:12.468332 gravity-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-04-14 15:41:02.000000 gravity-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:41:12.468332 gravity-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-04-14 15:41:02.000000 gravity-1.0.3/tests/test_config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11256 2023-04-14 15:41:02.000000 gravity-1.0.3/tests/test_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25130 2023-04-14 15:41:02.000000 gravity-1.0.3/tests/test_process_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-04-14 15:41:02.000000 gravity-1.0.3/tests/test_settings.py
```

### Comparing `gravity-1.0.2/HISTORY.rst` & `gravity-1.0.3/HISTORY.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =========
  History
 =========
 
+1.0.3
+=====
+
+- Don't create supervisor conf dir unless necessary, create the gravity data dir as the correct user by @natefoo in https://github.com/galaxyproject/gravity/pull/105
+
 1.0.2
 =====
 
 - Pin a minimum package version of gx-it-proxy by @natefoo in https://github.com/galaxyproject/gravity/pull/102
 
 1.0.1
 =====
```

### Comparing `gravity-1.0.2/LICENSE` & `gravity-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gravity-1.0.2/PKG-INFO` & `gravity-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gravity
-Version: 1.0.2
+Version: 1.0.3
 Summary: Command-line utilities to assist in managing Galaxy servers
 Home-page: https://github.com/galaxyproject/gravity
 Author: The Galaxy Team
 Author-email: team@galaxyproject.org
 License: MIT
 Keywords: gravity galaxy
 Classifier: Intended Audience :: System Administrators
@@ -118,14 +118,19 @@
 .. _the full documentation: https://gravity.readthedocs.io
 
 
 =========
  History
 =========
 
+1.0.3
+=====
+
+- Don't create supervisor conf dir unless necessary, create the gravity data dir as the correct user by @natefoo in https://github.com/galaxyproject/gravity/pull/105
+
 1.0.2
 =====
 
 - Pin a minimum package version of gx-it-proxy by @natefoo in https://github.com/galaxyproject/gravity/pull/102
 
 1.0.1
 =====
```

### Comparing `gravity-1.0.2/README.rst` & `gravity-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `gravity-1.0.2/gravity/cli.py` & `gravity-1.0.3/gravity/cli.py`

 * *Files identical despite different names*

### Comparing `gravity-1.0.2/gravity/commands/cmd_exec.py` & `gravity-1.0.3/gravity/commands/cmd_exec.py`

 * *Files identical despite different names*

### Comparing `gravity-1.0.2/gravity/commands/cmd_follow.py` & `gravity-1.0.3/gravity/commands/cmd_follow.py`

 * *Files identical despite different names*

### Comparing `gravity-1.0.2/gravity/commands/cmd_graceful.py` & `gravity-1.0.3/gravity/commands/cmd_graceful.py`

 * *Files identical despite different names*

### Comparing `gravity-1.0.2/gravity/commands/cmd_list.py` & `gravity-1.0.3/gravity/commands/cmd_list.py`

 * *Files identical despite different names*

### Comparing `gravity-1.0.2/gravity/commands/cmd_restart.py` & `gravity-1.0.3/gravity/commands/cmd_restart.py`

 * *Files identical despite different names*

### Comparing `gravity-1.0.2/gravity/commands/cmd_show.py` & `gravity-1.0.3/gravity/commands/cmd_show.py`

 * *Files identical despite different names*

### Comparing `gravity-1.0.2/gravity/commands/cmd_start.py` & `gravity-1.0.3/gravity/commands/cmd_start.py`

 * *Files identical despite different names*

### Comparing `gravity-1.0.2/gravity/commands/cmd_status.py` & `gravity-1.0.3/gravity/commands/cmd_status.py`

 * *Files identical despite different names*

### Comparing `gravity-1.0.2/gravity/commands/cmd_stop.py` & `gravity-1.0.3/gravity/commands/cmd_stop.py`

 * *Files identical despite different names*

### Comparing `gravity-1.0.2/gravity/config_manager.py` & `gravity-1.0.3/gravity/config_manager.py`

 * *Files identical despite different names*

### Comparing `gravity-1.0.2/gravity/io.py` & `gravity-1.0.3/gravity/io.py`

 * *Files identical despite different names*

### Comparing `gravity-1.0.2/gravity/options.py` & `gravity-1.0.3/gravity/options.py`

 * *Files identical despite different names*

### Comparing `gravity-1.0.2/gravity/process_manager/__init__.py` & `gravity-1.0.3/gravity/process_manager/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,14 +272,21 @@
         format_vars = self._service_format_vars(config, service_instance)
         print_env = ' '.join('{}={}'.format(k, shlex.quote(v)) for k, v in format_vars["environment"].items())
 
         cmd = shlex.split(format_vars["command"])
         env = {**dict(os.environ), **format_vars["environment"]}
         cwd = format_vars["galaxy_root"]
 
+        # ensure the data dir exists
+        try:
+            os.makedirs(config.gravity_data_dir)
+        except OSError as exc:
+            if exc.errno != errno.EEXIST:
+                raise
+
         gravity.io.info(f"Working directory: {cwd}")
         gravity.io.info(f"Executing: {print_env} {format_vars['command']}")
 
         if not no_exec:
             os.chdir(cwd)
             os.execvpe(cmd[0], cmd, env)
```

### Comparing `gravity-1.0.2/gravity/process_manager/supervisor.py` & `gravity-1.0.3/gravity/process_manager/supervisor.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,17 +157,14 @@
         self.supervisord_conf_path = os.path.join(self.supervisor_state_dir, "supervisord.conf")
         self.supervisord_conf_dir = os.path.join(self.supervisor_state_dir, "supervisord.conf.d")
         self.supervisord_pid_path = os.path.join(self.supervisor_state_dir, "supervisord.pid")
         self.supervisord_sock_path = os.environ.get("SUPERVISORD_SOCKET", os.path.join(self.supervisor_state_dir, "supervisor.sock"))
         self.__supervisord_popen = None
         self.foreground = foreground
 
-        if not os.path.exists(self.supervisord_conf_dir):
-            os.makedirs(self.supervisord_conf_dir)
-
     @property
     def log_file(self):
         return os.path.join(self.supervisor_state_dir, "supervisord.log")
 
     def __supervisord_is_running(self):
         try:
             assert os.path.exists(self.supervisord_pid_path)
@@ -180,14 +177,16 @@
     def __supervisord(self):
         format_vars = {"supervisor_state_dir": self.supervisor_state_dir, "supervisord_conf_dir": self.supervisord_conf_dir}
         supervisord_cmd = [self.supervisord_exe, "-c", self.supervisord_conf_path]
         if self.foreground:
             supervisord_cmd.append('--nodaemon')
         if not self.__supervisord_is_running():
             # any time that supervisord is not running, let's rewrite supervisord.conf
+            if not os.path.exists(self.supervisord_conf_dir):
+                os.makedirs(self.supervisord_conf_dir)
             open(self.supervisord_conf_path, "w").write(SUPERVISORD_CONF_TEMPLATE.format(**format_vars))
             self.__supervisord_popen = subprocess.Popen(supervisord_cmd, env=os.environ)
             rc = self.__supervisord_popen.poll()
             if rc:
                 gravity.io.error("supervisord exited with code %d" % rc)
             start = time.time()
             while not os.path.exists(self.supervisord_pid_path) or not os.path.exists(self.supervisord_sock_path):
```

### Comparing `gravity-1.0.2/gravity/process_manager/systemd.py` & `gravity-1.0.3/gravity/process_manager/systemd.py`

 * *Files identical despite different names*

### Comparing `gravity-1.0.2/gravity/settings.py` & `gravity-1.0.3/gravity/settings.py`

 * *Files identical despite different names*

### Comparing `gravity-1.0.2/gravity/state.py` & `gravity-1.0.3/gravity/state.py`

 * *Files identical despite different names*

### Comparing `gravity-1.0.2/gravity/util/__init__.py` & `gravity-1.0.3/gravity/util/__init__.py`

 * *Files identical despite different names*

### Comparing `gravity-1.0.2/gravity.egg-info/PKG-INFO` & `gravity-1.0.3/gravity.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gravity
-Version: 1.0.2
+Version: 1.0.3
 Summary: Command-line utilities to assist in managing Galaxy servers
 Home-page: https://github.com/galaxyproject/gravity
 Author: The Galaxy Team
 Author-email: team@galaxyproject.org
 License: MIT
 Keywords: gravity galaxy
 Classifier: Intended Audience :: System Administrators
@@ -118,14 +118,19 @@
 .. _the full documentation: https://gravity.readthedocs.io
 
 
 =========
  History
 =========
 
+1.0.3
+=====
+
+- Don't create supervisor conf dir unless necessary, create the gravity data dir as the correct user by @natefoo in https://github.com/galaxyproject/gravity/pull/105
+
 1.0.2
 =====
 
 - Pin a minimum package version of gx-it-proxy by @natefoo in https://github.com/galaxyproject/gravity/pull/102
 
 1.0.1
 =====
```

### Comparing `gravity-1.0.2/gravity.egg-info/SOURCES.txt` & `gravity-1.0.3/gravity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gravity-1.0.2/setup.py` & `gravity-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `gravity-1.0.2/tests/test_config_manager.py` & `gravity-1.0.3/tests/test_config_manager.py`

 * *Files identical despite different names*

### Comparing `gravity-1.0.2/tests/test_operations.py` & `gravity-1.0.3/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `gravity-1.0.2/tests/test_process_manager.py` & `gravity-1.0.3/tests/test_process_manager.py`

 * *Files identical despite different names*

### Comparing `gravity-1.0.2/tests/test_settings.py` & `gravity-1.0.3/tests/test_settings.py`

 * *Files identical despite different names*

