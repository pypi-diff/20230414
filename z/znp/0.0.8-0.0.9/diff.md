# Comparing `tmp/znp-0.0.8.tar.gz` & `tmp/znp-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "znp-0.0.8.tar", last modified: Tue Oct 11 04:50:24 2022, max compression
+gzip compressed data, was "znp-0.0.9.tar", last modified: Mon Nov 14 03:44:02 2022, max compression
```

## Comparing `znp-0.0.8.tar` & `znp-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2022-10-11 04:50:24.074983 znp-0.0.8/
--rw-r--r--   0 anon      (1000) wheel      (998)    34846 2022-09-12 23:22:21.000000 znp-0.0.8/LICENSE
--rw-r--r--   0 anon      (1000) wheel      (998)     5091 2022-10-11 04:50:24.074983 znp-0.0.8/PKG-INFO
--rw-r--r--   0 anon      (1000) wheel      (998)     4767 2022-09-15 20:11:09.000000 znp-0.0.8/README.md
--rw-r--r--   0 anon      (1000) wheel      (998)      557 2022-10-11 04:50:19.000000 znp-0.0.8/pyproject.toml
--rw-r--r--   0 anon      (1000) wheel      (998)       38 2022-10-11 04:50:24.074983 znp-0.0.8/setup.cfg
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2022-10-11 04:50:24.071650 znp-0.0.8/src/
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2022-10-11 04:50:24.071650 znp-0.0.8/src/znp/
--rwxr-xr-x   0 anon      (1000) wheel      (998)       23 2022-09-12 23:24:52.000000 znp-0.0.8/src/znp/__init__.py
--rw-r--r--   0 anon      (1000) wheel      (998)     5117 2022-09-21 23:34:45.000000 znp-0.0.8/src/znp/__main__.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     2263 2022-09-15 20:11:09.000000 znp-0.0.8/src/znp/options.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     1874 2022-09-21 23:34:45.000000 znp-0.0.8/src/znp/prompts.py
--rw-r--r--   0 anon      (1000) wheel      (998)     3252 2022-09-12 23:24:52.000000 znp-0.0.8/src/znp/utils.py
--rw-r--r--   0 anon      (1000) wheel      (998)     7606 2022-10-11 04:49:45.000000 znp-0.0.8/src/znp/zathura.py
--rw-r--r--   0 anon      (1000) wheel      (998)     3904 2022-09-15 20:11:09.000000 znp-0.0.8/src/znp/zsocket.py
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2022-10-11 04:50:24.071650 znp-0.0.8/src/znp.egg-info/
--rw-r--r--   0 anon      (1000) wheel      (998)     5091 2022-10-11 04:50:24.000000 znp-0.0.8/src/znp.egg-info/PKG-INFO
--rw-r--r--   0 anon      (1000) wheel      (998)      353 2022-10-11 04:50:24.000000 znp-0.0.8/src/znp.egg-info/SOURCES.txt
--rw-r--r--   0 anon      (1000) wheel      (998)        1 2022-10-11 04:50:24.000000 znp-0.0.8/src/znp.egg-info/dependency_links.txt
--rw-r--r--   0 anon      (1000) wheel      (998)       42 2022-10-11 04:50:24.000000 znp-0.0.8/src/znp.egg-info/entry_points.txt
--rw-r--r--   0 anon      (1000) wheel      (998)       49 2022-10-11 04:50:24.000000 znp-0.0.8/src/znp.egg-info/requires.txt
--rw-r--r--   0 anon      (1000) wheel      (998)        4 2022-10-11 04:50:24.000000 znp-0.0.8/src/znp.egg-info/top_level.txt
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2022-11-14 03:44:02.001291 znp-0.0.9/
+-rw-r--r--   0 anon      (1000) wheel      (998)    34846 2022-09-12 23:22:21.000000 znp-0.0.9/LICENSE
+-rw-r--r--   0 anon      (1000) wheel      (998)     5091 2022-11-14 03:44:02.001291 znp-0.0.9/PKG-INFO
+-rw-r--r--   0 anon      (1000) wheel      (998)     4767 2022-09-15 20:11:09.000000 znp-0.0.9/README.md
+-rw-r--r--   0 anon      (1000) wheel      (998)      557 2022-11-14 03:43:00.000000 znp-0.0.9/pyproject.toml
+-rw-r--r--   0 anon      (1000) wheel      (998)       38 2022-11-14 03:44:02.001291 znp-0.0.9/setup.cfg
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2022-11-14 03:44:02.001291 znp-0.0.9/src/
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2022-11-14 03:44:02.001291 znp-0.0.9/src/znp/
+-rwxr-xr-x   0 anon      (1000) wheel      (998)       23 2022-09-12 23:24:52.000000 znp-0.0.9/src/znp/__init__.py
+-rw-r--r--   0 anon      (1000) wheel      (998)     5340 2022-11-14 03:29:51.000000 znp-0.0.9/src/znp/__main__.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     2762 2022-11-14 03:03:09.000000 znp-0.0.9/src/znp/options.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     1874 2022-09-21 23:34:45.000000 znp-0.0.9/src/znp/prompts.py
+-rw-r--r--   0 anon      (1000) wheel      (998)     3252 2022-09-12 23:24:52.000000 znp-0.0.9/src/znp/utils.py
+-rw-r--r--   0 anon      (1000) wheel      (998)     7987 2022-11-14 03:41:59.000000 znp-0.0.9/src/znp/zathura.py
+-rw-r--r--   0 anon      (1000) wheel      (998)     4025 2022-11-14 03:24:58.000000 znp-0.0.9/src/znp/zsocket.py
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2022-11-14 03:44:02.001291 znp-0.0.9/src/znp.egg-info/
+-rw-r--r--   0 anon      (1000) wheel      (998)     5091 2022-11-14 03:44:01.000000 znp-0.0.9/src/znp.egg-info/PKG-INFO
+-rw-r--r--   0 anon      (1000) wheel      (998)      353 2022-11-14 03:44:02.000000 znp-0.0.9/src/znp.egg-info/SOURCES.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)        1 2022-11-14 03:44:01.000000 znp-0.0.9/src/znp.egg-info/dependency_links.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)       42 2022-11-14 03:44:01.000000 znp-0.0.9/src/znp.egg-info/entry_points.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)       49 2022-11-14 03:44:01.000000 znp-0.0.9/src/znp.egg-info/requires.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)        4 2022-11-14 03:44:01.000000 znp-0.0.9/src/znp.egg-info/top_level.txt
```

### Comparing `znp-0.0.8/LICENSE` & `znp-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `znp-0.0.8/PKG-INFO` & `znp-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: znp
-Version: 0.0.8
+Version: 0.0.9
 Summary: Simple program to open a file in existing zathura instance
 License: GNU General Public License v3 (GPLv3)
 Project-URL: repository, https://codeberg.org/johndovern/znp
 Keywords: zathura
 Description-Content-Type: text/markdown
 Provides-Extra: x11
 License-File: LICENSE
```

### Comparing `znp-0.0.8/README.md` & `znp-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `znp-0.0.8/pyproject.toml` & `znp-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "znp"
-version = "0.0.8"
+version = "0.0.9"
 description = "Simple program to open a file in existing zathura instance"
 readme = "README.md"
 license = { text = "GNU General Public License v3 (GPLv3)" }
 keywords = [ "zathura" ]
 dependencies = [
     "python-magic",
     "psutil",
```

### Comparing `znp-0.0.8/src/znp/__main__.py` & `znp-0.0.9/src/znp/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 
 def open_next_or_prev(
     file_path,
     next_file=False,
     prev_file=False,
     prompt_cmd=None,
+    page_number=-1,
 ):
     """
     Open file in zathura optionally open the next file in
     the directory of the given file
     """
     # Try to get the next or prev file in the cwd
     try:
@@ -51,31 +52,27 @@
             z.open(file_path=next_or_prev_file, pid=z.epid)
             return 0
         # Failed so we contiue and get the pid the hard way
         except TypeError:
             pass
     # Try searching for the given file manually
     # If found open it and exit
-    if z.zathura_search(z.pids, search_file=file_path):
+    if z.zathura_search(z.pids, search_file=file_path, page_number=page_number):
         z.open(file_path=next_or_prev_file, pid=z.search_pid)
-        # z.remove_tmp_files()
         return 0
     # No prompt_cmd given, exit
     if not prompt_cmd:
-        # z.remove_tmp_files()
         return 1
     # Prompt user for their desired instance
     choice = zathura_prompt(pid_dict=z.pid_dict, prompt_cmd=prompt_cmd)
     # No selection made, exit
     if not choice:
-        # z.remove_tmp_files()
         return 1
     # Try opening the next file and exit
     z.open(file_path=next_or_prev_file, pid=choice)
-    # z.remove_tmp_files()
     return 0
 
 
 def open_given_file(
     file_path,
     prompt_cmd,
     prompt_args=None,
@@ -147,26 +144,32 @@
     # to the calling znp server
     if args.client is not None:
         return send_to_socket(
             pid=args.pid,
             parent_pid=args.source,
             file_path=args.file,
             server_address=args.client,
+            page_number=args.page,
         )
     # User is opening next or prev file
     if args.next or args.prev:
         return open_next_or_prev(
             file_path=args.file,
             next_file=args.next,
             prev_file=args.prev,
             prompt_cmd=user.settings["prompt_cmd"],
+            page_number=args.page,
         )
     # User just wants a the pid of a specific instance
     if args.query:
-        return z.query(search_file=args.file)
+        return z.query(search_file=args.file, page_number=args.page)
+    if args.execute is not None:
+        if z.query(search_file=args.file, page_number=args.page, print_result=False):
+            return 1
+        return z.execute(pid=z.search_pid, command=args.execute)
     # User wants to open the given file in an optionally given zathura instance
     return open_given_file(
         file_path=args.file,
         prompt_cmd=user.settings["prompt_cmd"],
         prompt_args=user.settings["prompt_args"],
         pid=args.pid,
     )
```

### Comparing `znp-0.0.8/src/znp/options.py` & `znp-0.0.9/src/znp/options.py`

 * *Files 19% similar despite different names*

```diff
@@ -22,14 +22,35 @@
         sent and need not be an actual message. Used internally when searching for active
         instances and their open files and is executed like so:
         `znp -P 1234567 -c "/tmp/znp/znp_socket" "/path/to/current.pdf"` from the instance
         that belongs to pid 1234567.
         """,
     )
     parser.add_argument(
+        "-e",
+        "--execute",
+        metavar="COMMAND",
+        action="store",
+        help="""
+        Execute the given command in the instance corresponding to the given
+        FILE
+        """,
+    )
+    parser.add_argument(
+        "-g",
+        "--page",
+        metavar="PAGE_NUMBER",
+        action="store",
+        type=int,
+        default=-1,
+        help="""
+        Used for executing commands for greater precision but not required.
+        """,
+    )
+    parser.add_argument(
         "-n",
         "--next",
         action="store_true",
         help="""
         Go to the next file in the directory of the given file
         """,
     )
```

### Comparing `znp-0.0.8/src/znp/prompts.py` & `znp-0.0.9/src/znp/prompts.py`

 * *Files identical despite different names*

### Comparing `znp-0.0.8/src/znp/utils.py` & `znp-0.0.9/src/znp/utils.py`

 * *Files identical despite different names*

### Comparing `znp-0.0.8/src/znp/zathura.py` & `znp-0.0.9/src/znp/zathura.py`

 * *Files 6% similar despite different names*

```diff
@@ -118,15 +118,15 @@
             return 0
         # Close current file so progress is saved
         # Open the given file
         zathuraName = "org.pwmt.zathura.PID-" + str(pid)
         zathuraObject = dbus.SessionBus().get_object(zathuraName, "/org/pwmt/zathura")
         zathuraDBus = dbus.Interface(zathuraObject, "org.pwmt.zathura")
         zathuraDBus.ExecuteCommand("close")
-        zathuraDBus.ExecuteCommand(f"open \"{file_path}\"")
+        zathuraDBus.ExecuteCommand(f'open "{file_path}"')
         return 0
 
     def pid_search(self, name="zathura"):
         """
         Search for zathura pid(s). Used when:
             1. User is using Wayland
             2. ewmh fails for some reason
@@ -140,31 +140,35 @@
                 continue
             if p_name == name:
                 pids.append(proc.pid)
         self.pids = pids
         self.pid_count = len(pids)
         return None
 
-    def query(self, search_file):
+    def query(self, search_file, page_number, print_result=True):
         """
         Query zathura instances for the instance with search_file open.
         If found prints the pid, else nothing and exits with status 1.
         """
         if self.pid_count == 0:
             return 1
         elif self.pid_count == 1:
-            print(self.pids[0])
+            if print_result:
+                print(self.pids[0])
             return 0
-        elif self.zathura_search(self.pids, search_file=search_file):
-            print(self.search_pid)
+        elif self.zathura_search(
+            self.pids, search_file=search_file, page_number=page_number
+        ):
+            if print_result:
+                print(self.search_pid)
             return 0
 
         return 1
 
-    def zathura_search(self, pids, search_file=None, prog="znp"):
+    def zathura_search(self, pids, search_file=None, page_number=-1, prog="znp"):
         """
         Search for an instance of zathura using bad means.
         This creates a dictionary of zathura instances if multiple exist:
             >>> zathura = Zathura()
             >>> print(zathura.pid_dict)
             >>> '{ "123456": ["/path/to/file.pdf", "123456: /path/to/file.pdf"]
                    "154684": ["/path/to/file.epub", "154684: /path/to/file.epub"] }'
@@ -178,33 +182,38 @@
         # Start SocketListener and expect as many messages as pids
         pid_count = len(pids)
         server = SocketListener(
             server_address=server_address,
             expected_messages=pid_count,
         )
         # Give server some time to start
-        time.sleep(0.05)
+        time.sleep(0.005)
         # Get pid of current script in case client fails it will kill
         # this script so user is not left with a hanging process/socket
         ppid = os.getpid()
         # Run clients to find current files in each pid
         for pid in pids:
             self.execute(
-                pid, f"exec znp -P {pid} -s {ppid} -c {server_address} '$FILE'"
+                pid,
+                f"exec znp -P {pid} -s {ppid} -c {server_address} '$FILE' -g '$PAGE'",
             )
         # Wait for server to get all client messages
         while server.recieved < pid_count:
             pass
         # Server must have recieved all messages, store it's data
         self.pid_dict = server.pid_dict
         self.search_pid = None
         # If not searching for a specific file return True
         if not search_file:
             return True
         # Search the pid_dict for the desired file
         for key, value in server.pid_dict.items():
-            if value[0] == search_file:
-                # Search_file found set search_pid and return True
-                self.search_pid = key
-                return True
+            if value[2] == search_file:
+                # Search_file found, set search_pid and return True
+                if page_number > -1 and page_number == int(value[1]):
+                    self.search_pid = key
+                    return True
+                elif page_number == -1:
+                    self.search_pid = key
+                    return True
         # Desired instance wasn't found return False
         return False
```

### Comparing `znp-0.0.8/src/znp/zsocket.py` & `znp-0.0.9/src/znp/zsocket.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 #!/usr/bin/env python3
 import os
 import signal
 import socket
 import sys
-import time
 from threading import Thread
 
 
 class SocketListener:
     """
     Run a socket listener in the background and listen for x connections
     """
@@ -34,45 +33,47 @@
         # Chmod the socket
         os.chmod(self.server_address, mode=0o600)
         # Listen for incoming connections
         sock.listen(self.expected)
         # Loop until recieved the expected number of connections
         while self.recieved < self.expected:
             # Clean up data for new connection
+            page = None
             path = None
             pid = None
             # Listen for connection
             connection, client_address = sock.accept()
             # Connection found, try receiving info
             try:
                 while True:
                     # Get header, should be a pid padded with zeros
                     if not pid:
                         pid = connection.recv(7)
+                    if not page:
+                        page = connection.recv(24)
                     # Store temp_data
                     temp_path = connection.recv(1024)
                     if temp_path:
                         # Set data to temp_data if none stored yet
                         if not path:
                             path = temp_path
                         # Else add it to already stored data
                         else:
                             path = path + temp_path
                     # Connection complete store info
                     else:
                         # Decode message
                         pid = pid.decode(encoding="utf-8")
                         pid = str(int(pid))
-                        path = path.decode(encoding="utf-8")
-                        # self.pids.append(header)
+                        page = page.decode(encoding="utf-8")
+                        if path is not None:
+                            path = path.decode(encoding="utf-8")
                         pids.append(pid)
-                        # self.pid_dict[header] = []
                         pid_dict[pid] = []
-                        # self.pid_dict[header].extend([path, f"{pid}: {path}"])
-                        pid_dict[pid].extend([path, f"{pid}: {path}"])
+                        pid_dict[pid].extend([pid, page, path])
                         break
             finally:
                 # Clean up the connection
                 connection.close()
                 self.recieved += 1
         # Finished receiving data, store it
         self.pids = pids
@@ -82,15 +83,15 @@
         try:
             os.unlink(self.server_address)
         except OSError:
             if os.path.exists(self.server_address):
                 raise
 
 
-def send_to_socket(pid, parent_pid, file_path, server_address):
+def send_to_socket(pid, parent_pid, file_path, server_address, page_number):
     """
     Send message to socket.
     The pid is used as the header.
     The file_path is used as the message.
     The server_address is the address to send the message to.
     """
     # Set pid to 0000000 if none given
@@ -103,14 +104,16 @@
     except socket.error as msg:
         print(f"Received error: {msg}\nKilling server.", sys.stderr)
         os.kill(parent_pid, signal.SIGKILL)
         return 1
     # Try sending data
     try:
         pid = bytes(str(pid).zfill(7), encoding="utf-8")
+        page = bytes(str(page_number).zfill(24), encoding="utf-8")
         file_path = bytes(str(file_path), encoding="utf-8")
         sock.sendall(pid)
+        sock.sendall(page)
         sock.sendall(file_path)
     finally:
         sock.close()
 
     return 0
```

### Comparing `znp-0.0.8/src/znp.egg-info/PKG-INFO` & `znp-0.0.9/src/znp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: znp
-Version: 0.0.8
+Version: 0.0.9
 Summary: Simple program to open a file in existing zathura instance
 License: GNU General Public License v3 (GPLv3)
 Project-URL: repository, https://codeberg.org/johndovern/znp
 Keywords: zathura
 Description-Content-Type: text/markdown
 Provides-Extra: x11
 License-File: LICENSE
```

