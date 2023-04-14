# Comparing `tmp/grpc-interceptor-0.8.0.tar.gz` & `tmp/grpc-interceptor-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grpc-interceptor-0.8.0.tar", last modified: Sun Jul 19 23:05:57 2020, max compression
+gzip compressed data, was "grpc-interceptor-0.9.0.tar", last modified: Wed Jul 22 19:57:03 2020, max compression
```

## Comparing `grpc-interceptor-0.8.0.tar` & `grpc-interceptor-0.9.0.tar`

### file list

```diff
@@ -1,9 +1,16 @@
--rw-r--r--   0        0        0     1070 2020-07-19 23:04:55.182000 grpc-interceptor-0.8.0/LICENSE
--rw-r--r--   0        0        0      658 2020-07-19 23:04:55.182000 grpc-interceptor-0.8.0/README.md
--rw-r--r--   0        0        0     1062 2020-07-19 23:04:55.182000 grpc-interceptor-0.8.0/pyproject.toml
--rw-r--r--   0        0        0       43 2020-07-19 23:04:55.182000 grpc-interceptor-0.8.0/src/grpc_interceptor/__init__.py
--rw-r--r--   0        0        0     2509 2020-07-19 23:04:55.182000 grpc-interceptor-0.8.0/src/grpc_interceptor/base.py
--rw-r--r--   0        0        0      953 2020-07-19 23:04:55.182000 grpc-interceptor-0.8.0/src/grpc_interceptor/exception_to_status.py
--rw-r--r--   0        0        0     8901 2020-07-19 23:04:55.182000 grpc-interceptor-0.8.0/src/grpc_interceptor/exceptions.py
--rw-r--r--   0        0        0     1384 2020-07-19 23:05:57.959420 grpc-interceptor-0.8.0/setup.py
--rw-r--r--   0        0        0     1370 2020-07-19 23:05:57.959685 grpc-interceptor-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2020-07-22 19:50:22.432513 grpc-interceptor-0.9.0/LICENSE
+-rw-r--r--   0        0        0     3742 2020-07-22 19:50:22.432513 grpc-interceptor-0.9.0/README.md
+-rw-r--r--   0        0        0     1337 2020-07-22 19:50:22.432513 grpc-interceptor-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0       43 2020-07-22 19:50:22.432513 grpc-interceptor-0.9.0/src/grpc_interceptor/__init__.py
+-rw-r--r--   0        0        0     4342 2020-07-22 19:50:22.432513 grpc-interceptor-0.9.0/src/grpc_interceptor/base.py
+-rw-r--r--   0        0        0      953 2020-07-22 19:50:22.432513 grpc-interceptor-0.9.0/src/grpc_interceptor/exception_to_status.py
+-rw-r--r--   0        0        0     9216 2020-07-22 19:50:22.432513 grpc-interceptor-0.9.0/src/grpc_interceptor/exceptions.py
+-rw-r--r--   0        0        0      614 2020-07-22 19:50:22.432513 grpc-interceptor-0.9.0/src/grpc_interceptor/testing/__init__.py
+-rw-r--r--   0        0        0     2543 2020-07-22 19:50:22.432513 grpc-interceptor-0.9.0/src/grpc_interceptor/testing/dummy_client.py
+-rw-r--r--   0        0        0       40 2020-07-22 19:50:22.432513 grpc-interceptor-0.9.0/src/grpc_interceptor/testing/protos/__init__.py
+-rw-r--r--   0        0        0      199 2020-07-22 19:50:22.432513 grpc-interceptor-0.9.0/src/grpc_interceptor/testing/protos/dummy.proto
+-rw-r--r--   0        0        0     4318 2020-07-22 19:50:22.432513 grpc-interceptor-0.9.0/src/grpc_interceptor/testing/protos/dummy_pb2.py
+-rw-r--r--   0        0        0     1441 2020-07-22 19:50:22.432513 grpc-interceptor-0.9.0/src/grpc_interceptor/testing/protos/dummy_pb2.pyi
+-rw-r--r--   0        0        0     1738 2020-07-22 19:50:22.432513 grpc-interceptor-0.9.0/src/grpc_interceptor/testing/protos/dummy_pb2_grpc.py
+-rw-r--r--   0        0        0     4725 2020-07-22 19:57:03.867227 grpc-interceptor-0.9.0/setup.py
+-rw-r--r--   0        0        0     4539 2020-07-22 19:57:03.867784 grpc-interceptor-0.9.0/PKG-INFO
```

### Comparing `grpc-interceptor-0.8.0/LICENSE` & `grpc-interceptor-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `grpc-interceptor-0.8.0/src/grpc_interceptor/exception_to_status.py` & `grpc-interceptor-0.9.0/src/grpc_interceptor/exception_to_status.py`

 * *Files identical despite different names*

### Comparing `grpc-interceptor-0.8.0/src/grpc_interceptor/exceptions.py` & `grpc-interceptor-0.9.0/src/grpc_interceptor/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,14 +52,27 @@
         Returns:
             A string displaying the class name, status code, and details.
         """
         clsname = self.__class__.__name__
         sc = self.status_code.name
         return f"{clsname}(status_code={sc}, details={self.details!r})"
 
+    @property
+    def status_string(self):
+        """Return status_code as a string.
+
+        Returns:
+            The status code as a string.
+
+        Example:
+            GrpcException(status_code=StatusCode.NOT_FOUND).status_string
+            >>> "NOT_FOUND"
+        """
+        return self.status_code.name
+
 
 class Aborted(GrpcException):
     """The operation was aborted.
 
     Typically this is due to a concurrency issue such as a sequencer check failure or
     transaction abort. See the guidelines on other exceptions for deciding between
     FAILED_PRECONDITION, ABORTED, and UNAVAILABLE.
```

