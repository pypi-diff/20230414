# Comparing `tmp/babichjacob_coordinator-0.1.0.tar.gz` & `tmp/babichjacob_coordinator-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "babichjacob_coordinator-0.1.0.tar", max compression
+gzip compressed data, was "babichjacob_coordinator-0.1.1.tar", max compression
```

## Comparing `babichjacob_coordinator-0.1.0.tar` & `babichjacob_coordinator-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     4427 2023-04-14 06:26:42.816582 babichjacob_coordinator-0.1.0/coordinator/__init__.py
--rw-r--r--   0        0        0        0 2023-04-14 04:36:31.699203 babichjacob_coordinator-0.1.0/coordinator/py.typed
--rw-r--r--   0        0        0      910 2023-04-14 06:28:40.439874 babichjacob_coordinator-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      608 2023-04-14 06:23:16.985236 babichjacob_coordinator-0.1.0/README.md
--rw-r--r--   0        0        0     1515 1970-01-01 00:00:00.000000 babichjacob_coordinator-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      579 2023-04-14 06:32:22.697370 babichjacob_coordinator-0.1.1/README.md
+-rw-r--r--   0        0        0     4259 2023-04-14 06:32:22.697370 babichjacob_coordinator-0.1.1/coordinator/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-14 06:32:22.697370 babichjacob_coordinator-0.1.1/coordinator/py.typed
+-rw-r--r--   0        0        0      884 2023-04-14 06:32:22.697370 babichjacob_coordinator-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1515 1970-01-01 00:00:00.000000 babichjacob_coordinator-0.1.1/PKG-INFO
```

### Comparing `babichjacob_coordinator-0.1.0/coordinator/__init__.py` & `babichjacob_coordinator-0.1.1/coordinator/__init__.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,168 +1,168 @@
-from asyncio import FIRST_COMPLETED, CancelledError, Event, Future, create_task, wait
-from dataclasses import dataclass
-from typing import AsyncIterator, Generic, Tuple, TypeVar
-
-from option_and_result import NONE, Option, Some
-
-T = TypeVar("T")
-
-
-@dataclass
-class MutableContainer(Generic[T]):
-    value: T
-
-
-@dataclass
-class Request(Generic[T]):
-    _future: Future[T]
-
-    def fulfill(self, value: T):
-        self._future.set_result(value)
-
-
-@dataclass
-class Responder(Generic[T]):
-    _shared_future: MutableContainer[Future[Future[T]]]
-    _closed: Event
-    _disconnected: Event
-
-    async def wait_for_poll(self) -> Option[Request[T]]:
-        disconnected_event = create_task(self._disconnected.wait())
-        get_task = create_task(wait_for_future(self._shared_future.value))
-        try:
-            done, _pending = await wait(
-                [get_task, disconnected_event], return_when=FIRST_COMPLETED
-            )
-        except CancelledError:
-            disconnected_event.cancel()
-            get_task.cancel()
-            raise
-
-        if disconnected_event in done:
-            get_task.cancel()
-            return NONE()
-
-        assert get_task in done
-        disconnected_event.cancel()
-        if self._closed.is_set():
-            self._disconnected.set()
-
-        return Some(Request(get_task.result()))
-
-    async def __aiter__(self) -> AsyncIterator[Request[T]]:
-        while True:
-            received = await self.wait_for_poll()
-
-            if received.is_none():
-                return
-
-            yield received.unwrap()
-
-    def close(self):
-        self._closed.set()
-        self._disconnected.set()
-
-    def __del__(self):
-        self.close()
-
-
-@dataclass
-class Response(Generic[T]):
-    _future: Future[T]
-
-    def __await__(self):
-        return self._future.__await__()
-
-
-async def wait_for_future(future: Future[T]) -> T:
-    return await future
-
-
-@dataclass
-class Requester(Generic[T]):
-    _shared_future: MutableContainer[Future[Future[T]]]
-    _closed: Event
-    _disconnected: Event
-    _waiters: int
-
-    async def request(self) -> Option[Response[T]]:
-        if self._waiters == 0:
-            self._shared_future.value.set_result(Future())
-
-        self._waiters += 1
-
-        disconnected_event = create_task(self._disconnected.wait())
-        get_task = create_task(wait_for_future(self._shared_future.value))
-        try:
-            done, _pending = await wait(
-                [get_task, disconnected_event], return_when=FIRST_COMPLETED
-            )
-        except CancelledError:
-            disconnected_event.cancel()
-            get_task.cancel()
-            self._waiters -= 1
-            raise
-
-        if disconnected_event in done:
-            get_task.cancel()
-            self._waiters -= 1
-            return NONE()
-
-        assert get_task in done
-        disconnected_event.cancel()
-        if self._closed.is_set():
-            self._disconnected.set()
-
-        self._waiters -= 1
-
-        if self._waiters == 0:
-            self._shared_future.value = Future()
-
-        return Some(Response(get_task.result()))
-
-    async def request_and_wait(self) -> Option[T]:
-        future_option = await self.request()
-
-        if future_option.is_none():
-            return NONE()
-
-        future = future_option.unwrap()
-        result = await future
-        return Some(result)
-
-    async def __aiter__(self) -> AsyncIterator[T]:
-        while True:
-            received = await self.request_and_wait()
-
-            if received.is_none():
-                return
-
-            yield received.unwrap()
-
-    def close(self):
-        self._closed.set()
-        if not self._shared_future.value.done():
-            self._disconnected.set()
-
-    def __del__(self):
-        self.close()
-
-
-def coordinator() -> Tuple[Responder[T], Requester[T]]:
-    shared_future: MutableContainer[Future[Future[T]]] = MutableContainer(Future())
-    closed = Event()
-    disconnected = Event()
-
-    responder = Responder(
-        _shared_future=shared_future,
-        _closed=closed,
-        _disconnected=disconnected,
-    )
-    requester = Requester(
-        _shared_future=shared_future,
-        _closed=closed,
-        _disconnected=disconnected,
-        _waiters=0,
-    )
-
-    return (responder, requester)
+from asyncio import FIRST_COMPLETED, CancelledError, Event, Future, create_task, wait
+from dataclasses import dataclass
+from typing import AsyncIterator, Generic, Tuple, TypeVar
+
+from option_and_result import NONE, Option, Some
+
+T = TypeVar("T")
+
+
+@dataclass
+class MutableContainer(Generic[T]):
+    value: T
+
+
+@dataclass
+class Request(Generic[T]):
+    _future: Future[T]
+
+    def fulfill(self, value: T):
+        self._future.set_result(value)
+
+
+@dataclass
+class Responder(Generic[T]):
+    _shared_future: MutableContainer[Future[Future[T]]]
+    _closed: Event
+    _disconnected: Event
+
+    async def wait_for_poll(self) -> Option[Request[T]]:
+        disconnected_event = create_task(self._disconnected.wait())
+        get_task = create_task(wait_for_future(self._shared_future.value))
+        try:
+            done, _pending = await wait(
+                [get_task, disconnected_event], return_when=FIRST_COMPLETED
+            )
+        except CancelledError:
+            disconnected_event.cancel()
+            get_task.cancel()
+            raise
+
+        if disconnected_event in done:
+            get_task.cancel()
+            return NONE()
+
+        assert get_task in done
+        disconnected_event.cancel()
+        if self._closed.is_set():
+            self._disconnected.set()
+
+        return Some(Request(get_task.result()))
+
+    async def __aiter__(self) -> AsyncIterator[Request[T]]:
+        while True:
+            received = await self.wait_for_poll()
+
+            if received.is_none():
+                return
+
+            yield received.unwrap()
+
+    def close(self):
+        self._closed.set()
+        self._disconnected.set()
+
+    def __del__(self):
+        self.close()
+
+
+@dataclass
+class Response(Generic[T]):
+    _future: Future[T]
+
+    def __await__(self):
+        return self._future.__await__()
+
+
+async def wait_for_future(future: Future[T]) -> T:
+    return await future
+
+
+@dataclass
+class Requester(Generic[T]):
+    _shared_future: MutableContainer[Future[Future[T]]]
+    _closed: Event
+    _disconnected: Event
+    _waiters: int
+
+    async def request(self) -> Option[Response[T]]:
+        if self._waiters == 0:
+            self._shared_future.value.set_result(Future())
+
+        self._waiters += 1
+
+        disconnected_event = create_task(self._disconnected.wait())
+        get_task = create_task(wait_for_future(self._shared_future.value))
+        try:
+            done, _pending = await wait(
+                [get_task, disconnected_event], return_when=FIRST_COMPLETED
+            )
+        except CancelledError:
+            disconnected_event.cancel()
+            get_task.cancel()
+            self._waiters -= 1
+            raise
+
+        if disconnected_event in done:
+            get_task.cancel()
+            self._waiters -= 1
+            return NONE()
+
+        assert get_task in done
+        disconnected_event.cancel()
+        if self._closed.is_set():
+            self._disconnected.set()
+
+        self._waiters -= 1
+
+        if self._waiters == 0:
+            self._shared_future.value = Future()
+
+        return Some(Response(get_task.result()))
+
+    async def request_and_wait(self) -> Option[T]:
+        future_option = await self.request()
+
+        if future_option.is_none():
+            return NONE()
+
+        future = future_option.unwrap()
+        result = await future
+        return Some(result)
+
+    async def __aiter__(self) -> AsyncIterator[T]:
+        while True:
+            received = await self.request_and_wait()
+
+            if received.is_none():
+                return
+
+            yield received.unwrap()
+
+    def close(self):
+        self._closed.set()
+        if not self._shared_future.value.done():
+            self._disconnected.set()
+
+    def __del__(self):
+        self.close()
+
+
+def coordinator() -> Tuple[Responder[T], Requester[T]]:
+    shared_future: MutableContainer[Future[Future[T]]] = MutableContainer(Future())
+    closed = Event()
+    disconnected = Event()
+
+    responder = Responder(
+        _shared_future=shared_future,
+        _closed=closed,
+        _disconnected=disconnected,
+    )
+    requester = Requester(
+        _shared_future=shared_future,
+        _closed=closed,
+        _disconnected=disconnected,
+        _waiters=0,
+    )
+
+    return (responder, requester)
```

### Comparing `babichjacob_coordinator-0.1.0/README.md` & `babichjacob_coordinator-0.1.1/README.md`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-<h1 align="center">TODO emoji Coordinator</h1>
-
-TODO
-
-## 💻 Installation
-
-This package is [published to PyPI as `babichjacob-coordinator`](https://pypi.org/project/babichjacob-coordinator/).
-
-## 🛠 Usage
-
-```py
-# TODO: write this
-```
-
-## 😵 Help! I have a question
-
-Create an issue and I'll try to help.
-
-## 😡 Fix! There is something that needs improvement
-
-Create an issue or pull request and I'll try to fix.
-
-## 📄 License
-
-MIT
-
-## 🙏 Attribution
-
-_This README was generated with ❤️ by [readme-md-generator](https://github.com/kefranabg/readme-md-generator)_
+<h1 align="center">TODO emoji Coordinator</h1>
+
+TODO
+
+## 💻 Installation
+
+This package is [published to PyPI as `babichjacob-coordinator`](https://pypi.org/project/babichjacob-coordinator/).
+
+## 🛠 Usage
+
+```py
+# TODO: write this
+```
+
+## 😵 Help! I have a question
+
+Create an issue and I'll try to help.
+
+## 😡 Fix! There is something that needs improvement
+
+Create an issue or pull request and I'll try to fix.
+
+## 📄 License
+
+MIT
+
+## 🙏 Attribution
+
+_This README was generated with ❤️ by [readme-md-generator](https://github.com/kefranabg/readme-md-generator)_
```

### Comparing `babichjacob_coordinator-0.1.0/PKG-INFO` & `babichjacob_coordinator-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: babichjacob-coordinator
-Version: 0.1.0
+Version: 0.1.1
 Summary: A tool for coordinating producers and consumers of data
 Home-page: https://github.com/babichjacob/python-coordinator
 License: MIT
 Author: J or Jacob Babich
 Author-email: jacobbabichpublic+git@gmail.com
 Requires-Python: >=3.5,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

