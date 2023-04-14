# Comparing `tmp/turbo_queue-0.5.2.tar.gz` & `tmp/turbo_queue-0.5.2.2.tar.gz`

## Comparing `turbo_queue-0.5.2.tar` & `turbo_queue-0.5.2.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0  1145211 2020-02-02 00:00:00.000000 turbo_queue-0.5.2/monitor_queue.gif
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 turbo_queue-0.5.2/requirements.txt
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 turbo_queue-0.5.2/src/turbo_queue/__init__.py
--rw-r--r--   0        0        0    20955 2020-02-02 00:00:00.000000 turbo_queue-0.5.2/src/turbo_queue/_turbo_queue.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 turbo_queue-0.5.2/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 turbo_queue-0.5.2/LICENSE
--rw-r--r--   0        0        0     8324 2020-02-02 00:00:00.000000 turbo_queue-0.5.2/README.md
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 turbo_queue-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     8864 2020-02-02 00:00:00.000000 turbo_queue-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0  1145211 2020-02-02 00:00:00.000000 turbo_queue-0.5.2.2/monitor_queue.gif
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 turbo_queue-0.5.2.2/requirements.txt
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 turbo_queue-0.5.2.2/src/turbo_queue/__init__.py
+-rw-r--r--   0        0        0    20992 2020-02-02 00:00:00.000000 turbo_queue-0.5.2.2/src/turbo_queue/_turbo_queue.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 turbo_queue-0.5.2.2/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 turbo_queue-0.5.2.2/LICENSE
+-rw-r--r--   0        0        0     8324 2020-02-02 00:00:00.000000 turbo_queue-0.5.2.2/README.md
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 turbo_queue-0.5.2.2/pyproject.toml
+-rw-r--r--   0        0        0     8866 2020-02-02 00:00:00.000000 turbo_queue-0.5.2.2/PKG-INFO
```

### Comparing `turbo_queue-0.5.2/monitor_queue.gif` & `turbo_queue-0.5.2.2/monitor_queue.gif`

 * *Files identical despite different names*

### Comparing `turbo_queue-0.5.2/src/turbo_queue/_turbo_queue.py` & `turbo_queue-0.5.2.2/src/turbo_queue/_turbo_queue.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,18 +270,19 @@
                     except:
                         file_error = True
                 if file_error:
                     if self._remove_invalid:
                         try:
                             os.remove(file)
                         except:
-                            rename(
-                                file,
-                                f"{new_file_path}/invalid_file_{self.get_current_epoch_int()}_{self.get_uuid()}_recovered.db",
-                            )
+                            #rename(
+                            #    file,
+                            #    f"{new_file_path}/invalid_file_{self.get_current_epoch_int()}_{self.get_uuid()}_recovered.db",
+                            #)
+                            pass
                     else:
                         rename(
                             file,
                             f"{new_file_path}/invalid_file_{self.get_current_epoch_int()}_{self.get_uuid()}_recovered.db",
                         )
                 else:
                     rename(
```

### Comparing `turbo_queue-0.5.2/LICENSE` & `turbo_queue-0.5.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `turbo_queue-0.5.2/README.md` & `turbo_queue-0.5.2.2/README.md`

 * *Files identical despite different names*

### Comparing `turbo_queue-0.5.2/pyproject.toml` & `turbo_queue-0.5.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "turbo-queue"
-version = "0.5.2"
+version = "0.5.2.2"
 authors = [
   { name="Dave Waters", email="dave@1waters.com" },
 ]
 description = "A Python module to improve performance of multiprocessing queues"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `turbo_queue-0.5.2/PKG-INFO` & `turbo_queue-0.5.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turbo-queue
-Version: 0.5.2
+Version: 0.5.2.2
 Summary: A Python module to improve performance of multiprocessing queues
 Project-URL: Homepage, https://github.com/davewat/turbo-queue
 Project-URL: Bug Tracker, https://github.com/davewat/turbo-queue/issues
 Author-email: Dave Waters <dave@1waters.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

