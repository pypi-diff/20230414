# Comparing `tmp/stress_injector-0.4-py3-none-any.whl.zip` & `tmp/stress_injector-0.4a0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 12692 bytes, number of entries: 12
--rw-r--r--  2.0 unx      248 b- defN 23-Apr-14 03:21 stressinjector/__init__.py
--rw-r--r--  2.0 unx     4767 b- defN 23-Apr-14 03:21 stressinjector/cpu.py
--rw-r--r--  2.0 unx     2997 b- defN 23-Apr-14 03:21 stressinjector/echo.py
--rw-r--r--  2.0 unx     4565 b- defN 23-Apr-14 03:21 stressinjector/memory.py
--rw-r--r--  2.0 unx     1082 b- defN 23-Apr-14 03:21 stressinjector/models.py
--rw-r--r--  2.0 unx       49 b- defN 23-Apr-14 03:21 stressinjector/requirements.txt
--rw-r--r--  2.0 unx     4477 b- defN 23-Apr-14 03:21 stressinjector/url.py
--rw-r--r--  2.0 unx     1078 b- defN 23-Apr-14 03:22 stress_injector-0.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     8509 b- defN 23-Apr-14 03:22 stress_injector-0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-14 03:22 stress_injector-0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-Apr-14 03:22 stress_injector-0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      981 b- defN 23-Apr-14 03:22 stress_injector-0.4.dist-info/RECORD
-12 files, 28860 bytes uncompressed, 11042 bytes compressed:  61.7%
+Zip file size: 12493 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      189 b- defN 23-Apr-14 02:34 stressinjector/__init__.py
+-rw-r--r--  2.0 unx     4767 b- defN 23-Apr-14 02:34 stressinjector/cpu.py
+-rw-r--r--  2.0 unx     2997 b- defN 23-Apr-14 02:34 stressinjector/echo.py
+-rw-r--r--  2.0 unx     4565 b- defN 23-Apr-14 02:34 stressinjector/memory.py
+-rw-r--r--  2.0 unx      838 b- defN 23-Apr-14 02:34 stressinjector/models.py
+-rw-r--r--  2.0 unx       40 b- defN 23-Apr-14 02:34 stressinjector/requirements.txt
+-rw-r--r--  2.0 unx     4664 b- defN 23-Apr-14 02:34 stressinjector/url.py
+-rw-r--r--  2.0 unx     1078 b- defN 23-Apr-14 02:34 stress_injector-0.4a0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7808 b- defN 23-Apr-14 02:34 stress_injector-0.4a0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-14 02:34 stress_injector-0.4a0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-Apr-14 02:34 stress_injector-0.4a0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      990 b- defN 23-Apr-14 02:34 stress_injector-0.4a0.dist-info/RECORD
+12 files, 28043 bytes uncompressed, 10823 bytes compressed:  61.4%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: stressinjector/requirements.txt
 Comment: 
 
 Filename: stressinjector/url.py
 Comment: 
 
-Filename: stress_injector-0.4.dist-info/LICENSE
+Filename: stress_injector-0.4a0.dist-info/LICENSE
 Comment: 
 
-Filename: stress_injector-0.4.dist-info/METADATA
+Filename: stress_injector-0.4a0.dist-info/METADATA
 Comment: 
 
-Filename: stress_injector-0.4.dist-info/WHEEL
+Filename: stress_injector-0.4a0.dist-info/WHEEL
 Comment: 
 
-Filename: stress_injector-0.4.dist-info/top_level.txt
+Filename: stress_injector-0.4a0.dist-info/top_level.txt
 Comment: 
 
-Filename: stress_injector-0.4.dist-info/RECORD
+Filename: stress_injector-0.4a0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## stressinjector/__init__.py

```diff
@@ -1,6 +1,5 @@
 from stressinjector.cpu import CPUStress  # noqa: F401
 from stressinjector.memory import MemoryStress  # noqa: F401
-from stressinjector.models import RequestType  # noqa: F401
 from stressinjector.url import URLStress  # noqa: F401
 
-version = "0.4"
+version = "0.4a"
```

## stressinjector/models.py

```diff
@@ -1,14 +1,11 @@
 import logging
 import os
 import platform
 from enum import Enum
-from typing import Callable
-
-import requests
 
 LOGGER = logging.getLogger(__name__)
 LOGGER.addHandler(logging.StreamHandler())
 LOGGER.setLevel(logging.DEBUG)
 
 
 class UnsupportedOS(OSError):
@@ -32,20 +29,11 @@
     pid: int = os.getpid()
     os: str = platform.system()
 
 
 settings = Settings
 
 
-class RequestType:
-    """Wrapper for request types."""
-
-    GET: Callable = requests.get
-    PUT: Callable = requests.put
-    POST: Callable = requests.post
-    DELETE: Callable = requests.delete
-
-
 _supported_systems = (operating_system.macOS, operating_system.linux, operating_system.windows)
 
 if settings.os not in _supported_systems:
     raise UnsupportedOS(f"\n\ncurrently supported only on {', '.join(_supported_systems)}\n")
```

## stressinjector/requirements.txt

```diff
@@ -1,4 +1,3 @@
 numpy>=1.20.0
 psutil>=5.9.0
-tqdm>=4.56.0
-requests
+tqdm>=4.56.0
```

## stressinjector/url.py

```diff
@@ -1,70 +1,72 @@
+import http.client
 import logging
 import time
+import urllib.error
 import urllib.parse
+import urllib.request
 import warnings
 from concurrent.futures import ThreadPoolExecutor, as_completed
-from typing import Callable, NoReturn, Union
+from typing import NoReturn, Union
 
-from .models import LOGGER, RequestType
+from .models import LOGGER
 
 RESULT = {'success': 0, 'errors': 0}
 
 
 class URLStress:
     """Controller for URL stress using threadpool. Gets url as input.
 
     >>> URLStress
 
     """
 
     def __init__(self, url: str, rate: int = 1e+5, timeout: Union[int, float] = 5e-1,
                  retry_limit: Union[int, float] = 5, circuit_break: Union[int, float] = 5,
-                 logger: logging.Logger = None, request_type: Callable = RequestType.GET,
-                 **kwargs):
+                 logger: logging.Logger = None, **kwargs):
         """Instantiate the object, parse and validate the URL.
 
         Args:
             url: URL to inject stress.
             rate: Number of calls to make.
             timeout: Timeout for each request.
             retry_limit: Retry limit if the system is unable to spinup more threads.
             circuit_break: Wait time in seconds between retries.
-            logger: Custom logger.
-            request_type: Function from ``requests`` module.
             kwargs: Keyword arguments to use in the request.
         """
         self.parsed = urllib.parse.urlparse(url=url, allow_fragments=True)
         if self.parsed.scheme not in ('http', 'https', 'ws'):
             raise ValueError(
                 f"\n\nbad url: {url}\n{self.parsed.scheme}"
             )
         self.LOGGER = logger or LOGGER
         self.request_url = url
         self.request_rate = int(rate)
         self.timeout = timeout
         self.retry_limit = retry_limit
         self.circuit_break = circuit_break
         self.kwargs = kwargs or {}
-        self.request_type = request_type
 
     def make_request(self, sample: bool = False) -> NoReturn:
         """Makes a GET request to the endpoint.
 
         Args:
             sample: Boolean flag to indicate if the request is sample.
         """
         if sample:
-            response = self.request_type(url=self.request_url, **self.kwargs)
+            response: http.client.HTTPResponse = urllib.request.urlopen(url=self.request_url, timeout=self.timeout,
+                                                                        **self.kwargs)
         else:
-            response = self.request_type(url=self.request_url, timeout=self.timeout, **self.kwargs)
-        if response.ok:
+            response: http.client.HTTPResponse = urllib.request.urlopen(url=self.request_url, **self.kwargs)
+        response_code = response.getcode()
+        if 200 <= response_code <= 399:
             return
         else:
-            response.raise_for_status()
+            raise urllib.error.HTTPError(code=response_code, url=response.geturl(),
+                                         msg=response.msg.__str__(), hdrs=response.headers, fp=response.fp)
 
     def initiate_injection(self) -> NoReturn:
         """Initiates injection in a thread pool."""
         futures = {}
         retries = 0
         executor = ThreadPoolExecutor(max_workers=self.request_rate)
         with executor:
```

## Comparing `stress_injector-0.4.dist-info/LICENSE` & `stress_injector-0.4a0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `stress_injector-0.4.dist-info/METADATA` & `stress_injector-0.4a0.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stress-injector
-Version: 0.4
+Version: 0.4a0
 Summary: Python module, to inject memory and CPU stress, and URL load test
 Author-email: Vignesh Sivanandha Rao <svignesh1793@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Vignesh Sivanandha Rao
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -42,15 +42,14 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy (>=1.20.0)
 Requires-Dist: psutil (>=5.9.0)
 Requires-Dist: tqdm (>=4.56.0)
-Requires-Dist: requests
 Provides-Extra: dev
 Requires-Dist: pre-commit ; extra == 'dev'
 
 [![Pypi-version](https://img.shields.io/pypi/v/stress-injector)](https://pypi.org/project/stress-injector)
 [![Pypi-py-version](https://img.shields.io/pypi/pyversions/stress-injector)](https://pypi.org/project/stress-injector)
 
 ![docs](https://github.com/thevickypedia/stress-injector/actions/workflows/docs.yml/badge.svg)
@@ -87,61 +86,36 @@
 * I have then used `getrusage` (get resource usage) for `SELF` to get the memory consumed only by the current script.
 * The `size_converter` converts the bytes from resource usage to a human understandable format.
 </details>
 <br>
 <details>
 <summary><strong>Insights about <a href="https://github.com/thevickypedia/stress-injector/blob/main/stressinjector/onus.py">URL Stress</a></strong></summary>
 
-* In this script, I have used threadpools to make concurrent requests.
-* The script uses `requests` module to make calls.
+* In this script, I have used threadpools to make concurrent GET requests.
+* The script uses builtin library `urllib` to make the GET calls.
 * Takes arguments
   * **rate**: Number of calls to make. _Defaults to 100K_
   * **timeout**: Timeout for each request. _Defaults to 0.5_
   * **retry_limit**: Retry limit if the system is unable to spinup more threads. _Defaults to 5_
   * **circuit_break**: Wait time in seconds between retries. _Defaults to 5_
-  * **request_type**: Function from `requests` module.
 
 </details>
 
 ### Usage
 `pip install stress-injector`
 
 [CPU Stress](https://github.com/thevickypedia/stress-injector/blob/main/stressinjector/cpu.py)
 ```python
 import stressinjector as injector
 
 
 if __name__ == '__main__':
     injector.CPUStress(seconds=300).run()
-```
-
-[Memory Stress](https://github.com/thevickypedia/stress-injector/blob/main/stressinjector/memory.py)
-```python
-import stressinjector as injector
-
-
-if __name__ == '__main__':
     injector.MemoryStress(gigabytes=2_000).run()
-```
-
-[URL Stress](https://github.com/thevickypedia/stress-injector/blob/main/stressinjector/url.py)
-```python
-import stressinjector as injector
-
-
-if __name__ == '__main__':
-    injector.URLStress(url='http://0.0.0.0:5002/').run()  # Stress test GET calls
-
-    # Stress test POST calls, also supports PUT, and DELETE
-    sample_data = {'data': {'username': 'test', 'password': 'test'}}
-    injector.URLStress(
-      url='http://0.0.0.0:5002/',
-      request_type=injector.RequestType.POST,
-      **sample_data
-    ).run()
+    injector.URLStress(url='http://0.0.0.0:5002/').run()
 ```
 
 #### Coding Standards
 Docstring format: [`Google`](https://google.github.io/styleguide/pyguide.html#38-comments-and-docstrings) <br>
 Styling conventions: [`PEP 8`](https://www.python.org/dev/peps/pep-0008/) <br>
 Clean code with pre-commit hooks: [`flake8`](https://flake8.pycqa.org/en/latest/) and 
 [`isort`](https://pycqa.github.io/isort/)
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: stress-injector Version: 0.4 Summary: Python
+Metadata-Version: 2.1 Name: stress-injector Version: 0.4a0 Summary: Python
 module, to inject memory and CPU stress, and URL load test Author-email:
 Vignesh Sivanandha Rao
 gmail.com> License: MIT License Copyright (c) 2021 Vignesh Sivanandha Rao
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
@@ -27,19 +27,19 @@
 Classifier: Intended Audience :: Information Technology Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Python: >=3.8 Description-Content-Type:
 text/markdown License-File: LICENSE Requires-Dist: numpy (>=1.20.0) Requires-
-Dist: psutil (>=5.9.0) Requires-Dist: tqdm (>=4.56.0) Requires-Dist: requests
-Provides-Extra: dev Requires-Dist: pre-commit ; extra == 'dev' [![Pypi-version]
-(https://img.shields.io/pypi/v/stress-injector)](https://pypi.org/project/
-stress-injector) [![Pypi-py-version](https://img.shields.io/pypi/pyversions/
-stress-injector)](https://pypi.org/project/stress-injector) ![docs](https://
+Dist: psutil (>=5.9.0) Requires-Dist: tqdm (>=4.56.0) Provides-Extra: dev
+Requires-Dist: pre-commit ; extra == 'dev' [![Pypi-version](https://
+img.shields.io/pypi/v/stress-injector)](https://pypi.org/project/stress-
+injector) [![Pypi-py-version](https://img.shields.io/pypi/pyversions/stress-
+injector)](https://pypi.org/project/stress-injector) ![docs](https://
 github.com/thevickypedia/stress-injector/actions/workflows/docs.yml/badge.svg)
 ![pypi](https://github.com/thevickypedia/stress-injector/actions/workflows/
 python-publish.yml/badge.svg) [![Pypi-format](https://img.shields.io/pypi/
 format/stress-injector)](https://pypi.org/project/stress-injector/#files) [!
 [Pypi-status](https://img.shields.io/pypi/status/stress-injector)](https://
 pypi.org/project/stress-injector) ![Maintained](https://img.shields.io/
 maintenance/yes/2023) [![GitHub Repo created](https://img.shields.io/date/
@@ -61,35 +61,26 @@
  Insights about Memory_Stress * In this script, I have used
 `numpy.random.bytes` which are sampled from uniform distribution. * Generating
 these random bytes induces a stress on the machine's memory usage. * I have
 then used `getrusage` (get resource usage) for `SELF` to get the memory
 consumed only by the current script. * The `size_converter` converts the bytes
 from resource usage to a human understandable format.
  Insights about URL_Stress * In this script, I have used threadpools to make
-concurrent requests. * The script uses `requests` module to make calls. * Takes
-arguments * **rate**: Number of calls to make. _Defaults to 100K_ *
-**timeout**: Timeout for each request. _Defaults to 0.5_ * **retry_limit**:
-Retry limit if the system is unable to spinup more threads. _Defaults to 5_ *
-**circuit_break**: Wait time in seconds between retries. _Defaults to 5_ *
-**request_type**: Function from `requests` module.  ### Usage `pip install
-stress-injector` [CPU Stress](https://github.com/thevickypedia/stress-injector/
-blob/main/stressinjector/cpu.py) ```python import stressinjector as injector if
-__name__ == '__main__': injector.CPUStress(seconds=300).run() ``` [Memory
-Stress](https://github.com/thevickypedia/stress-injector/blob/main/
-stressinjector/memory.py) ```python import stressinjector as injector if
-__name__ == '__main__': injector.MemoryStress(gigabytes=2_000).run() ``` [URL
-Stress](https://github.com/thevickypedia/stress-injector/blob/main/
-stressinjector/url.py) ```python import stressinjector as injector if __name__
-== '__main__': injector.URLStress(url='http://0.0.0.0:5002/').run() # Stress
-test GET calls # Stress test POST calls, also supports PUT, and DELETE
-sample_data = {'data': {'username': 'test', 'password': 'test'}}
-injector.URLStress( url='http://0.0.0.0:5002/',
-request_type=injector.RequestType.POST, **sample_data ).run() ``` #### Coding
-Standards Docstring format: [`Google`](https://google.github.io/styleguide/
-pyguide.html#38-comments-and-docstrings)
+concurrent GET requests. * The script uses builtin library `urllib` to make the
+GET calls. * Takes arguments * **rate**: Number of calls to make. _Defaults to
+100K_ * **timeout**: Timeout for each request. _Defaults to 0.5_ *
+**retry_limit**: Retry limit if the system is unable to spinup more threads.
+_Defaults to 5_ * **circuit_break**: Wait time in seconds between retries.
+_Defaults to 5_  ### Usage `pip install stress-injector` [CPU Stress](https://
+github.com/thevickypedia/stress-injector/blob/main/stressinjector/cpu.py)
+```python import stressinjector as injector if __name__ == '__main__':
+injector.CPUStress(seconds=300).run() injector.MemoryStress
+(gigabytes=2_000).run() injector.URLStress(url='http://0.0.0.0:5002/').run()
+``` #### Coding Standards Docstring format: [`Google`](https://
+google.github.io/styleguide/pyguide.html#38-comments-and-docstrings)
 Styling conventions: [`PEP 8`](https://www.python.org/dev/peps/pep-0008/)
 Clean code with pre-commit hooks: [`flake8`](https://flake8.pycqa.org/en/
 latest/) and [`isort`](https://pycqa.github.io/isort/) #### [Release Notes]
 (https://github.com/thevickypedia/stress-injector/blob/main/release_notes.rst)
 **Requirement** ```shell python -m pip install changelog-generator ```
 **Usage** ```shell changelog reverse -f release_notes.rst -t 'Release Notes'
 ``` #### Linting `PreCommit` will ensure linting, and the doc creation are run
```

