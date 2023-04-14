# Comparing `tmp/jumpthegun-0.0.1.tar.gz` & `tmp/jumpthegun-0.0.2.tar.gz`

## Comparing `jumpthegun-0.0.1.tar` & `jumpthegun-0.0.2.tar`

### file list

```diff
@@ -1,35 +1,38 @@
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 jumpthegun-0.0.1/.flake8
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 jumpthegun-0.0.1/README.md
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 jumpthegun-0.0.1/test_requirements.txt
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 jumpthegun-0.0.1/tox.ini
--rwxr-xr-x   0        0        0     2979 2020-02-02 00:00:00.000000 jumpthegun-0.0.1/src/forklift.sh
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 jumpthegun-0.0.1/src/jumpthegun/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jumpthegun-0.0.1/src/jumpthegun/__version__.py
--rw-r--r--   0        0        0    13339 2020-02-02 00:00:00.000000 jumpthegun-0.0.1/src/jumpthegun/jumpthegunctl.py
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 jumpthegun-0.0.1/src/jumpthegun/project.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 jumpthegun-0.0.1/src/jumpthegun/testutils.py
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 jumpthegun-0.0.1/src/jumpthegun/tools.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 jumpthegun-0.0.1/src/jumpthegun/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jumpthegun-0.0.1/src/vendor/__init__.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 jumpthegun-0.0.1/src/vendor/filelock/LICENSE
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 jumpthegun-0.0.1/src/vendor/filelock/README.md
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 jumpthegun-0.0.1/src/vendor/filelock/VERSION
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 jumpthegun-0.0.1/src/vendor/filelock/__init__.py
--rw-r--r--   0        0        0     8896 2020-02-02 00:00:00.000000 jumpthegun-0.0.1/src/vendor/filelock/_api.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 jumpthegun-0.0.1/src/vendor/filelock/_error.py
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 jumpthegun-0.0.1/src/vendor/filelock/_soft.py
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 jumpthegun-0.0.1/src/vendor/filelock/_unix.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 jumpthegun-0.0.1/src/vendor/filelock/_util.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 jumpthegun-0.0.1/src/vendor/filelock/_windows.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jumpthegun-0.0.1/src/vendor/filelock/py.typed
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 jumpthegun-0.0.1/src/vendor/filelock/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jumpthegun-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     4491 2020-02-02 00:00:00.000000 jumpthegun-0.0.1/tests/test_forklift.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 jumpthegun-0.0.1/tests/testproj/.flake8
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 jumpthegun-0.0.1/tests/testproj/bad.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 jumpthegun-0.0.1/tests/testproj/good.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 jumpthegun-0.0.1/tests/testproj/pyproject.toml
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 jumpthegun-0.0.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 jumpthegun-0.0.1/LICENSE
--rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 jumpthegun-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 jumpthegun-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/.flake8
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/test_requirements.txt
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/tox.ini
+-rwxr-xr-x   0        0        0     3343 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/src/jumpthegun.sh
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/src/jumpthegun/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/src/jumpthegun/__version__.py
+-rw-r--r--   0        0        0    14142 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/src/jumpthegun/jumpthegunctl.py
+-rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/src/jumpthegun/output_redirect.py
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/src/jumpthegun/project.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/src/jumpthegun/testutils.py
+-rw-r--r--   0        0        0     3298 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/src/jumpthegun/tools.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/src/jumpthegun/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/src/vendor/__init__.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/src/vendor/filelock/LICENSE
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/src/vendor/filelock/README.md
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/src/vendor/filelock/VERSION
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/src/vendor/filelock/__init__.py
+-rw-r--r--   0        0        0     8896 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/src/vendor/filelock/_api.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/src/vendor/filelock/_error.py
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/src/vendor/filelock/_soft.py
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/src/vendor/filelock/_unix.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/src/vendor/filelock/_util.py
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/src/vendor/filelock/_windows.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/src/vendor/filelock/py.typed
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/src/vendor/filelock/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     6524 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/tests/test_jumpthegun.py
+-rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/tests/test_tools.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/tests/testproj/.flake8
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/tests/testproj/bad.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/tests/testproj/good.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/tests/testproj/pyproject.toml
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/README.md
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 jumpthegun-0.0.2/PKG-INFO
```

### Comparing `jumpthegun-0.0.1/README.md` & `jumpthegun-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.1/src/forklift.sh` & `jumpthegun-0.0.2/src/jumpthegun.sh`

 * *Files 17% similar despite different names*

```diff
@@ -2,68 +2,82 @@
 set -eEu -o pipefail
 
 function usage() {
   echo "Usage: $0 command tool_name ..."
   echo
   echo "Available commands:"
   echo
-  echo "start tool_name            Start a background daemon for a CLI tool."
-  echo "stop tool_name             Stop a background daemon for a CLI tool."
-  echo "restart tool_name          Restart a background daemon for a CLI tool."
-  echo "run tool_name [arg ...]    Run a CLI tool using a background process."
+  echo "run tool_name [OPTIONS] [arg ...]    Run a CLI tool."
+  echo "start tool_name                      Start a daemon for a CLI tool."
+  echo "stop tool_name                       Stop a daemon for a CLI tool."
+  echo "restart tool_name                    Restart a daemon for a CLI tool."
   echo
 }
 
 function err_exit() {
   err_msg="$1"
   echo "$err_msg" >&2
   exit 1
 }
 
+autorun=1
 case "${1:-}" in
 -h|--help)
   usage && exit 0 ;;
 start|stop|restart|version|--version)
   exec jumpthegunctl "$@" ;;
 run)
   shift
   [[ $# -eq 0 ]] && usage && exit 1
+  if [[ "$1" == "--no-autorun" ]]; then
+    autorun=0
+    shift
+  fi
   ([[ "$1" == "-h" ]] || [[ "$1" == "--help" ]]) && usage && exit 0
   tool_name="$1"
   shift
   ;;
 *)
   usage && exit 1 ;;
 esac
 
-
 # Find service runtime directory.
 runtime_dir="${XDG_RUNTIME_DIR:-}"
 if [ -n "$runtime_dir" ]; then
   service_runtime_dir="$runtime_dir/jumpthegun"
 else
   temp_dir="${TMPDIR:-/tmp}"
   shopt -s nullglob
   service_runtime_dirs=("$temp_dir/jumpthegun-$USER"-??????)
   shopt -u nullglob
   if [[ ${#service_runtime_dirs[@]} -eq 0 ]]; then
-    err_exit "Service not running."
+    [[ autorun -eq 1 ]] && jumpthegunctl start "$tool_name" >/dev/null 2>&1
+    exec "$tool_name" "$@"
   elif [[ ${#service_runtime_dirs[@]} -gt 1 ]]; then
     err_exit "Error: Multiple service runtime dirs found."
   fi
   service_runtime_dir="${service_runtime_dirs[0]}"
 fi
 
 # Calculate the isolated path for pid and port files.
 isolated_root="$(dirname "$(command -v "$tool_name")")"
-isolated_root_hash="$(echo -n "$isolated_root" | sha256sum - | head -c 8)"
+if [[ $OSTYPE == "darwin"* ]]; then
+  isolated_root_hash="$(echo -n "$isolated_root" | shasum -a 256 - | head -c 8)"
+else
+  isolated_root_hash="$(echo -n "$isolated_root" | sha256sum - | head -c 8)"
+fi
 isolated_path="$service_runtime_dir/$isolated_root_hash/"
 
+# Check that port file exists.
+if [[ ! -f "$isolated_path/$tool_name.port" ]]; then
+  [[ autorun -eq 1 ]] && jumpthegunctl start "$tool_name" >/dev/null 2>&1
+  exec "$tool_name" "$@"
+fi
+
 # Read port from port file.
-[ -f "$isolated_path/$tool_name.port" ] || err_exit "Service not running."
 IFS= read -r port <"$isolated_path/$tool_name.port"
 
 # Open TCP connection.
 exec 3<>"/dev/tcp/127.0.0.1/$port"
 
 # Close TCP connection upon exit.
 function close_connection {
```

### Comparing `jumpthegun-0.0.1/src/jumpthegun/jumpthegunctl.py` & `jumpthegun-0.0.2/src/jumpthegun/jumpthegunctl.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 import hashlib
 import io
+import json
 import os
 import random
 import shlex
 import signal
 import socket
 import string
 import subprocess
 import sys
 import tempfile
 import time
 import traceback
+from dataclasses import dataclass
 from pathlib import Path
-from typing import Any, BinaryIO, Optional, Set, Tuple, Union, cast
+from typing import Any, BinaryIO, Optional, Set, Tuple, cast
 
-from jumpthegun.project import get_tool_names
 from vendor.filelock import FileLock
 
 from .__version__ import __version__
-from .tools import ToolExceptionBase, UnsupportedTool, get_tool_runner
+from .output_redirect import SocketOutputRedirector
+from .project import get_tool_names
+from .tools import ToolExceptionBase, UnsupportedTool, get_tool_entrypoint
 from .utils import pid_exists
 
 
 class InvalidCommand(Exception):
     def __init__(self, command: str):
         super().__init__(command)
         self.command = command
@@ -34,39 +37,14 @@
 
 
 class DaemonDoesNotExistError(ToolExceptionBase):
     def __str__(self):
         return f'Jump the Gun daemon process for tool "{self.tool_name}" does not exist.'
 
 
-class _SocketWriter(io.RawIOBase):
-    """TODO!"""
-
-    def __init__(self, sock: socket.socket, prefix: Union[bytes, bytearray]) -> None:
-        self._sock = sock
-        self._prefix = prefix
-
-    def readable(self) -> bool:
-        return False
-
-    def writable(self) -> bool:
-        return True
-
-    def write(self, b: Union[bytes, bytearray]) -> int:  # type: ignore[override]
-        n_newlines = b.count(10)
-        # print(b"%b%d\n%b\n" % (self._prefix, n_newlines, b), file=sys.__stderr__)
-        self._sock.sendall(b"%b%d\n%b\n" % (self._prefix, n_newlines, b))
-        # print("DONE WRITING", file=sys.__stderr__)
-        with memoryview(b) as view:
-            return view.nbytes
-
-    def fileno(self) -> Any:
-        return self._sock.fileno()
-
-
 class StdinWrapper(io.RawIOBase):
     """TODO!"""
 
     def __init__(self, sock: socket.socket) -> None:
         self._sock = sock
         self._buf = bytearray()
 
@@ -102,14 +80,48 @@
 
     read = readline
 
     def fileno(self) -> Any:
         return self._sock.fileno()
 
 
+def get_xdg_config_dir() -> Path:
+    env_var = os.environ.get('XDG_CONFIG_HOME')
+    if env_var:
+        return Path(env_var)
+    return Path.home() / '.config'
+
+
+@dataclass(frozen=True)
+class JumpTheGunConfig:
+    idle_timeout_seconds: Optional[int] = 4 * 60 * 60  # 4 hours
+
+    def __post_init__(self):
+        if self.idle_timeout_seconds is None:
+            pass
+        elif isinstance(self.idle_timeout_seconds, int):
+            if self.idle_timeout_seconds <= 0:
+                raise ValueError("idle_timeout_seconds must be positive.")
+        else:
+            raise TypeError("idle_timeout_seconds must be an int or None.")
+
+
+def read_config() -> JumpTheGunConfig:
+    config_dir = get_xdg_config_dir()
+    if not config_dir.exists():
+        return JumpTheGunConfig()
+    config_file = config_dir / "jumpthegun.json"
+    if not config_file.exists():
+        return JumpTheGunConfig()
+    with config_file.open(encoding="utf-8") as f:
+        config_data = json.load(f)
+    config = JumpTheGunConfig(**config_data)
+    return config
+
+
 def get_service_runtime_dir_path() -> Path:
     runtime_dir = os.getenv("XDG_RUNTIME_DIR")
     if runtime_dir:
         service_runtime_dir = Path(runtime_dir) / "jumpthegun"
         service_runtime_dir.mkdir(exist_ok=True, mode=0o700)
         return service_runtime_dir
 
@@ -180,15 +192,24 @@
         file_pid = int(pid_file_path.read_text())
         if file_pid == pid:
             pid_file_path.unlink(missing_ok=True)
             port_file_path.unlink(missing_ok=True)
 
 
 def start(tool_name: str, daemonize: bool = True) -> None:
-    tool_runner = get_tool_runner(tool_name)
+    config = read_config()
+
+    # Import the tool and get its entrypoint function.
+    #
+    # Override sys.stdout and sys.stderr while loading the tool runner,
+    # so that any references to them kept during module imports (e.g for
+    # setting up logging) already reference the overrides.
+    output_redirector = SocketOutputRedirector()
+    with output_redirector.override_outputs_for_imports():
+        tool_runner = get_tool_entrypoint(tool_name)
 
     pid_file_path, port_file_path = get_pid_and_port_file_paths(tool_name)
 
     if pid_file_path.exists():
         file_pid = int(pid_file_path.read_text())
         if pid_exists(file_pid):
             raise DaemonAlreadyExistsError(tool_name=tool_name)
@@ -207,22 +228,22 @@
         os.setsid()
 
         pid = os.fork()
         if pid > 0:
             sys.exit(0)
 
         # redirect standard file descriptors
-        sys.stdout.flush()
-        sys.stderr.flush()
+        sys.__stdout__.flush()
+        sys.__stderr__.flush()
         stdin = open("/dev/null", "rb")
         stdout = open("/dev/null", "ab")
         stderr = open("/dev/null", "ab")
-        os.dup2(stdin.fileno(), sys.stdin.fileno())
-        os.dup2(stdout.fileno(), sys.stdout.fileno())
-        os.dup2(stderr.fileno(), sys.stderr.fileno())
+        os.dup2(stdin.fileno(), sys.__stdin__.fileno())
+        os.dup2(stdout.fileno(), sys.__stdout__.fileno())
+        os.dup2(stderr.fileno(), sys.__stderr__.fileno())
 
     # Write pid file.
     pid = os.getpid()
     pid_file_path.write_bytes(b"%d\n" % pid)
 
     # Open socket.
     sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
@@ -231,53 +252,51 @@
     # Write port file.
     host, port = sock.getsockname()
     port_file_path.write_bytes(b"%d\n" % port)
 
     # Listen for connections.
     sock.listen()
     print(f"Listening on {host}:{port} (pid={pid}) ...")
+    sock.settimeout(config.idle_timeout_seconds)
     subproc_pids = set()
     try:
         while True:
             conn, address = sock.accept()
             print(f"Got connection from: {address}")
             newpid = os.fork()
             if newpid == 0:
                 break
 
             # Avoid "zombie" processes: Reap completed sub-processes.
             done_subproc_pids = {x for x in subproc_pids if os.waitpid(x, os.WNOHANG)[0] != 0}
-            print(f"{done_subproc_pids=}")
             subproc_pids -= done_subproc_pids
             subproc_pids.add(newpid)
-    except BaseException:
+    except BaseException as exc:
         # Server is exiting: Clean up as needed.
         sock.close()
         if pid_file_path.exists():
             file_pid = int(pid_file_path.read_text())
             if file_pid == pid:
                 pid_file_path.unlink(missing_ok=True)
                 port_file_path.unlink(missing_ok=True)
+        if isinstance(exc, socket.timeout):
+            print(f"Exiting after receiving no connections for {config.idle_timeout_seconds} seconds.")
+            return
         raise
 
     # Send pid.
     conn.sendall(b"%d\n" % os.getpid())
 
     rfile = conn.makefile("rb", 0)
     sys.argv[1:] = shlex.split(rfile.readline().strip().decode())
     sys.argv[0] = tool_name
 
     sys.stdin.close()
     sys.stdin = io.TextIOWrapper(cast(BinaryIO, StdinWrapper(conn)))
-    sys.stdout = io.TextIOWrapper(
-        cast(BinaryIO, _SocketWriter(conn, b"1")), write_through=True
-    )
-    sys.stderr = io.TextIOWrapper(
-        cast(BinaryIO, _SocketWriter(conn, b"2")), write_through=True
-    )
+    output_redirector.set_socket(conn)
 
     # start_time = time.monotonic()
     try:
         retval = tool_runner()
     except BaseException as exc:
         # end_time = time.monotonic()
         # print(f"Time: {end_time - start_time}", file=sys.__stdout__)
@@ -306,15 +325,15 @@
         sys.stderr.close()
         conn.shutdown(socket.SHUT_WR)
         sys.exit(0)
 
 
 def stop(tool_name: str) -> None:
     try:
-        get_tool_runner(tool_name)
+        get_tool_entrypoint(tool_name)
     except UnsupportedTool:
         raise DaemonDoesNotExistError(tool_name)
 
     try:
         pid_file_path, _port_file_path = get_pid_and_port_file_paths(tool_name)
         if not pid_file_path.exists():
             raise DaemonDoesNotExistError(tool_name)
```

### Comparing `jumpthegun-0.0.1/src/jumpthegun/project.py` & `jumpthegun-0.0.2/src/jumpthegun/project.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.1/src/jumpthegun/utils.py` & `jumpthegun-0.0.2/src/jumpthegun/utils.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.1/src/vendor/filelock/LICENSE` & `jumpthegun-0.0.2/src/vendor/filelock/LICENSE`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.1/src/vendor/filelock/README.md` & `jumpthegun-0.0.2/src/vendor/filelock/README.md`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.1/src/vendor/filelock/__init__.py` & `jumpthegun-0.0.2/src/vendor/filelock/__init__.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.1/src/vendor/filelock/_api.py` & `jumpthegun-0.0.2/src/vendor/filelock/_api.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.1/src/vendor/filelock/_soft.py` & `jumpthegun-0.0.2/src/vendor/filelock/_soft.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.1/src/vendor/filelock/_unix.py` & `jumpthegun-0.0.2/src/vendor/filelock/_unix.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.1/src/vendor/filelock/_util.py` & `jumpthegun-0.0.2/src/vendor/filelock/_util.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.1/src/vendor/filelock/_windows.py` & `jumpthegun-0.0.2/src/vendor/filelock/_windows.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.1/.gitignore` & `jumpthegun-0.0.2/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -126,7 +126,10 @@
 dmypy.json
 
 # Pyre type checker
 .pyre/
 
 # IntelliJ / PyCharm
 .idea/
+
+# Test environments
+.testenvs/
```

### Comparing `jumpthegun-0.0.1/LICENSE` & `jumpthegun-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.1/pyproject.toml` & `jumpthegun-0.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "jumpthegun"
-description = "Make Python CLI tools blazing fast 🚀"
+description = "Make Python CLI tools win the speed race, by cheating!"
 license = { text = "Apache-2.0" }
 requires-python = ">=3.7"
 authors = [
   { name = "Tal Einat", email = "taleinat@gmail.com" },
 ]
 keywords = [
   "cli",
@@ -14,40 +14,40 @@
   "Environment :: Console",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: Apache Software License",
   "Operating System :: MacOS :: MacOS X",
   "Operating System :: POSIX :: Linux",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3 :: Only",
-  "Programming Language :: Python :: 3.6",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Topic :: Software Development :: Libraries",
 ]
 dependencies = [
   "tomli>=1.1.0; python_version < '3.11'",
 ]
-dynamic = ["readme", "version"]
+readme = "README.md"
+dynamic = ["version"]
 
 [project.optional-dependencies]
 test = [
   "pytest>=7,<8",
 ]
 
 [project.scripts]
 jumpthegunctl = "jumpthegun.jumpthegunctl:main"
 
 [project.urls]
 Homepage = "https://github.com/taleinat/jumpthegun"
 
 [build-system]
-requires = ["hatchling>=1.8.0", "hatch-fancy-pypi-readme"]
+requires = ["hatchling>=1.8.0"]
 build-backend = "hatchling.build"
 
 [tool.hatch.version]
 path = "src/jumpthegun/__version__.py"
 
 [tool.hatch.build.targets.sdist]
 exclude = [
@@ -59,23 +59,17 @@
 
 [tool.hatch.build.targets.wheel]
 only-include = ["src"]
 sources = ["src"]
 [tool.hatch.build.targets.wheel.shared-data]
 "src/jumpthegun.sh" = "bin/jumpthegun"
 
-[tool.hatch.metadata.hooks.fancy-pypi-readme]
-content-type = "text/markdown"
-fragments = [
-  { path = "README.md" },
-]
-
 [tool.black]
 line-length = 88
-target-version = ["py36", "py37", "py38", "py39", "py310", "py311"]
+target-version = ["py37", "py38", "py39", "py310", "py311"]
 include = '\.pyi?$'
 extend-exclude = 'vendor|tests/testproj'
 
 [tool.isort]
 atomic = true
 profile = "black"
 line_length = 88
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `jumpthegun-0.0.1/PKG-INFO` & `jumpthegun-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: jumpthegun
-Version: 0.0.1
-Summary: Make Python CLI tools blazing fast 🚀
+Version: 0.0.2
+Summary: Make Python CLI tools win the speed race, by cheating!
 Project-URL: Homepage, https://github.com/taleinat/jumpthegun
 Author-email: Tal Einat <taleinat@gmail.com>
 License: Apache-2.0
 License-File: LICENSE
 Keywords: cli
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

