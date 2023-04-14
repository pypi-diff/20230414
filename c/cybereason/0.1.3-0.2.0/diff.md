# Comparing `tmp/cybereason-0.1.3.tar.gz` & `tmp/cybereason-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cybereason-0.1.3.tar", last modified: Wed Apr 12 17:41:57 2023, max compression
+gzip compressed data, was "cybereason-0.2.0.tar", last modified: Fri Apr 14 00:37:04 2023, max compression
```

## Comparing `cybereason-0.1.3.tar` & `cybereason-0.2.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 17:41:57.845063 cybereason-0.1.3/
--rw-rw-rw-   0        0        0     1481 2023-04-12 17:30:28.000000 cybereason-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     2986 2023-04-12 17:41:57.845063 cybereason-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2069 2023-04-12 17:41:57.849074 cybereason-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0       60 2023-04-12 17:30:28.000000 cybereason-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-12 17:41:57.743979 cybereason-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-12 17:41:57.805167 cybereason-0.1.3/src/cybereason/
--rw-rw-rw-   0        0        0      198 2023-04-12 17:32:03.000000 cybereason-0.1.3/src/cybereason/__init__.py
--rw-rw-rw-   0        0        0     3023 2023-04-12 17:30:28.000000 cybereason-0.1.3/src/cybereason/_patch.py
--rw-rw-rw-   0        0        0     1243 2023-04-12 17:30:28.000000 cybereason-0.1.3/src/cybereason/_typing.py
--rw-rw-rw-   0        0        0    15392 2023-04-12 17:35:50.000000 cybereason-0.1.3/src/cybereason/client.py
--rw-rw-rw-   0        0        0     2640 2023-04-12 17:30:28.000000 cybereason-0.1.3/src/cybereason/custom_rules.py
--rw-rw-rw-   0        0        0     3775 2023-04-12 17:30:28.000000 cybereason-0.1.3/src/cybereason/exceptions.py
--rw-rw-rw-   0        0        0     3531 2023-04-12 17:30:28.000000 cybereason-0.1.3/src/cybereason/incident_reponse.py
--rw-rw-rw-   0        0        0     5212 2023-04-12 17:30:28.000000 cybereason-0.1.3/src/cybereason/malops.py
-drwxrwxrwx   0        0        0        0 2023-04-12 17:41:57.833578 cybereason-0.1.3/src/cybereason/parse/
--rw-rw-rw-   0        0        0      147 2023-04-12 17:30:28.000000 cybereason-0.1.3/src/cybereason/parse/__init__.py
--rw-rw-rw-   0        0        0     2472 2023-04-12 17:30:28.000000 cybereason-0.1.3/src/cybereason/parse/cef.py
--rw-rw-rw-   0        0        0     2846 2023-04-12 17:30:28.000000 cybereason-0.1.3/src/cybereason/parse/server.py
--rw-rw-rw-   0        0        0        0 2023-04-12 17:30:28.000000 cybereason-0.1.3/src/cybereason/py.typed
--rw-rw-rw-   0        0        0    16783 2023-04-12 17:30:28.000000 cybereason-0.1.3/src/cybereason/sensors.py
--rw-rw-rw-   0        0        0     4477 2023-04-12 17:30:28.000000 cybereason-0.1.3/src/cybereason/system.py
--rw-rw-rw-   0        0        0     6444 2023-04-12 17:30:28.000000 cybereason-0.1.3/src/cybereason/threat_intel.py
-drwxrwxrwx   0        0        0        0 2023-04-12 17:41:57.841210 cybereason-0.1.3/src/cybereason/utils/
--rw-rw-rw-   0        0        0     2967 2023-04-12 17:30:28.000000 cybereason-0.1.3/src/cybereason/utils/__init__.py
--rw-rw-rw-   0        0        0      796 2023-04-12 17:30:28.000000 cybereason-0.1.3/src/cybereason/utils/guid.py
-drwxrwxrwx   0        0        0        0 2023-04-12 17:41:57.822298 cybereason-0.1.3/src/cybereason.egg-info/
--rw-rw-rw-   0        0        0     2986 2023-04-12 17:41:57.000000 cybereason-0.1.3/src/cybereason.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      735 2023-04-12 17:41:57.000000 cybereason-0.1.3/src/cybereason.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 17:41:57.000000 cybereason-0.1.3/src/cybereason.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-12 17:41:57.000000 cybereason-0.1.3/src/cybereason.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      229 2023-04-12 17:41:57.000000 cybereason-0.1.3/src/cybereason.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-12 17:41:57.000000 cybereason-0.1.3/src/cybereason.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 00:37:04.941291 cybereason-0.2.0/
+-rw-rw-rw-   0        0        0     1481 2023-04-12 17:30:28.000000 cybereason-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     2986 2023-04-14 00:37:04.942615 cybereason-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2078 2023-04-14 00:37:04.943954 cybereason-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0       60 2023-04-12 17:30:28.000000 cybereason-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 00:37:04.838613 cybereason-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-14 00:37:04.903251 cybereason-0.2.0/src/cybereason/
+-rw-rw-rw-   0        0        0      198 2023-04-13 22:34:20.000000 cybereason-0.2.0/src/cybereason/__init__.py
+-rw-rw-rw-   0        0        0     3023 2023-04-12 17:30:28.000000 cybereason-0.2.0/src/cybereason/_patch.py
+-rw-rw-rw-   0        0        0     1306 2023-04-13 17:53:18.000000 cybereason-0.2.0/src/cybereason/_typing.py
+-rw-rw-rw-   0        0        0    15785 2023-04-14 00:09:11.000000 cybereason-0.2.0/src/cybereason/client.py
+-rw-rw-rw-   0        0        0     2640 2023-04-12 17:30:28.000000 cybereason-0.2.0/src/cybereason/custom_rules.py
+-rw-rw-rw-   0        0        0     4573 2023-04-13 17:48:23.000000 cybereason-0.2.0/src/cybereason/exceptions.py
+-rw-rw-rw-   0        0        0     3531 2023-04-12 17:30:28.000000 cybereason-0.2.0/src/cybereason/incident_reponse.py
+-rw-rw-rw-   0        0        0     5373 2023-04-13 22:25:58.000000 cybereason-0.2.0/src/cybereason/malops.py
+drwxrwxrwx   0        0        0        0 2023-04-14 00:37:04.929885 cybereason-0.2.0/src/cybereason/parse/
+-rw-rw-rw-   0        0        0      147 2023-04-12 17:30:28.000000 cybereason-0.2.0/src/cybereason/parse/__init__.py
+-rw-rw-rw-   0        0        0     2472 2023-04-12 17:30:28.000000 cybereason-0.2.0/src/cybereason/parse/cef.py
+-rw-rw-rw-   0        0        0     2846 2023-04-12 17:30:28.000000 cybereason-0.2.0/src/cybereason/parse/server.py
+-rw-rw-rw-   0        0        0        0 2023-04-12 17:30:28.000000 cybereason-0.2.0/src/cybereason/py.typed
+-rw-rw-rw-   0        0        0    16783 2023-04-12 17:30:28.000000 cybereason-0.2.0/src/cybereason/sensors.py
+-rw-rw-rw-   0        0        0     4477 2023-04-12 17:30:28.000000 cybereason-0.2.0/src/cybereason/system.py
+-rw-rw-rw-   0        0        0     6444 2023-04-12 17:30:28.000000 cybereason-0.2.0/src/cybereason/threat_intel.py
+drwxrwxrwx   0        0        0        0 2023-04-14 00:37:04.938555 cybereason-0.2.0/src/cybereason/utils/
+-rw-rw-rw-   0        0        0     4642 2023-04-14 00:07:58.000000 cybereason-0.2.0/src/cybereason/utils/__init__.py
+-rw-rw-rw-   0        0        0      796 2023-04-12 17:30:28.000000 cybereason-0.2.0/src/cybereason/utils/guid.py
+drwxrwxrwx   0        0        0        0 2023-04-14 00:37:04.918827 cybereason-0.2.0/src/cybereason.egg-info/
+-rw-rw-rw-   0        0        0     2986 2023-04-14 00:37:04.000000 cybereason-0.2.0/src/cybereason.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      735 2023-04-14 00:37:04.000000 cybereason-0.2.0/src/cybereason.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 00:37:04.000000 cybereason-0.2.0/src/cybereason.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-14 00:37:04.000000 cybereason-0.2.0/src/cybereason.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      229 2023-04-14 00:37:04.000000 cybereason-0.2.0/src/cybereason.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-14 00:37:04.000000 cybereason-0.2.0/src/cybereason.egg-info/top_level.txt
```

### Comparing `cybereason-0.1.3/LICENSE` & `cybereason-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cybereason-0.1.3/PKG-INFO` & `cybereason-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybereason
-Version: 0.1.3
+Version: 0.2.0
 Summary: Async Cybereason API client
 Home-page: https://github.com/forensic-security/cybereason#readme
 Author: Nuno André
 Author-email: mail@nunoand.re
 License: BSD-3-Clause
 Project-URL: Source, https://github.com/forensic-security/cybereason
 Project-URL: Bug Tracker, https://github.com/forensic-security/cybereason/issues
@@ -60,15 +60,15 @@
 from cybereason import Cybereason
 import asyncio
 import json
 
 async def dump_policies_config():
     '''Save metadata and config for every policy.
     '''
-    async with Cybereason(<server>, <username>, <password>) as client:
+    async with Cybereason(<tenant>, <username>, <password>) as client:
         async for policy in client.get_policies(show_config=True):
             filename = f'{policy["metadata"]["name"]}.json'
             with open(filename, 'w') as f:
                 json.dump(policy, f, indent=4)
 
 asyncio.run(dump_policies_config())
 ```
@@ -76,15 +76,15 @@
 ### Download and parse into JSON all user audit logs (action log)
 ```python
 from cybereason import Cybereason
 import asyncio
 import json
 
 async def user_audit():
-    async with Cybereason(<server>, <username>, <password>) as client:
+    async with Cybereason(<tenant>, <username>, <password>) as client:
         # rotated=False to get only the latest logs
         logs = [log async for log in client.get_user_audit_logs(rotated=True)]
         with open('user_audit.json', 'w') as f:
             json.dump(logs, f, indent=4)
 
 asyncio.run(user_audit())
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cybereason Version: 0.1.3 Summary: Async Cybereason
+Metadata-Version: 2.1 Name: cybereason Version: 0.2.0 Summary: Async Cybereason
 API client Home-page: https://github.com/forensic-security/cybereason#readme
 Author: Nuno AndrÃ© Author-email: mail@nunoand.re License: BSD-3-Clause
 Project-URL: Source, https://github.com/forensic-security/cybereason Project-
 URL: Bug Tracker, https://github.com/forensic-security/cybereason/issues
 Keywords: cybereason,cybersecurity,security,edr Platform: any Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators Classifier: Framework ::
```

### Comparing `cybereason-0.1.3/setup.cfg` & `cybereason-0.2.0/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -108,23 +108,23 @@
 000006b0: 385d 0d0a 6967 6e6f 7265 203d 2045 3131  8]..ignore = E11
 000006c0: 352c 2045 3232 312c 2045 3234 312c 2045  5, E221, E241, E
 000006d0: 3430 322c 2045 3733 310d 0a65 7863 6c75  402, E731..exclu
 000006e0: 6465 203d 200d 0a09 2e67 6974 2c0d 0a09  de = ....git,...
 000006f0: 5f5f 7079 6361 6368 655f 5f2c 0d0a 092e  __pycache__,....
 00000700: 6d79 7079 5f63 6163 6865 2c0d 0a09 2e70  mypy_cache,....p
 00000710: 7974 6573 745f 6361 6368 652c 0d0a 092e  ytest_cache,....
-00000720: 7665 6e76 2c0d 0a09 6275 696c 642c 0d0a  venv,...build,..
-00000730: 0974 6573 742e 2a2c 0d0a 095f 7479 7069  .test.*,..._typi
-00000740: 6e67 2e70 790d 0a69 6e6c 696e 652d 7175  ng.py..inline-qu
-00000750: 6f74 6573 203d 2073 696e 676c 650d 0a6d  otes = single..m
-00000760: 6178 2d63 6f6d 706c 6578 6974 7920 3d20  ax-complexity = 
-00000770: 3133 0d0a 6d61 782d 6c69 6e65 2d6c 656e  13..max-line-len
-00000780: 6774 6820 3d20 3939 0d0a 6d75 6c74 696c  gth = 99..multil
-00000790: 696e 652d 7175 6f74 6573 203d 2073 696e  ine-quotes = sin
-000007a0: 676c 650d 0a64 6f63 7374 7269 6e67 2d71  gle..docstring-q
-000007b0: 756f 7465 7320 3d20 7369 6e67 6c65 0d0a  uotes = single..
-000007c0: 0d0a 5b6d 7970 795d 0d0a 6967 6e6f 7265  ..[mypy]..ignore
-000007d0: 5f6d 6973 7369 6e67 5f69 6d70 6f72 7473  _missing_imports
-000007e0: 203d 2054 7275 650d 0a0d 0a5b 6567 675f   = True....[egg_
-000007f0: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
-00000800: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
-00000810: 300d 0a0d 0a                             0....
+00000720: 7665 6e76 2c0d 0a09 2e65 6767 732c 0d0a  venv,....eggs,..
+00000730: 0962 7569 6c64 2c0d 0a09 7465 7374 2e2a  .build,...test.*
+00000740: 2c0d 0a09 5f74 7970 696e 672e 7079 0d0a  ,..._typing.py..
+00000750: 696e 6c69 6e65 2d71 756f 7465 7320 3d20  inline-quotes = 
+00000760: 7369 6e67 6c65 0d0a 6d61 782d 636f 6d70  single..max-comp
+00000770: 6c65 7869 7479 203d 2031 330d 0a6d 6178  lexity = 13..max
+00000780: 2d6c 696e 652d 6c65 6e67 7468 203d 2039  -line-length = 9
+00000790: 390d 0a6d 756c 7469 6c69 6e65 2d71 756f  9..multiline-quo
+000007a0: 7465 7320 3d20 7369 6e67 6c65 0d0a 646f  tes = single..do
+000007b0: 6373 7472 696e 672d 7175 6f74 6573 203d  cstring-quotes =
+000007c0: 2073 696e 676c 650d 0a0d 0a5b 6d79 7079   single....[mypy
+000007d0: 5d0d 0a69 676e 6f72 655f 6d69 7373 696e  ]..ignore_missin
+000007e0: 675f 696d 706f 7274 7320 3d20 5472 7565  g_imports = True
+000007f0: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
+00000800: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
+00000810: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
```

### Comparing `cybereason-0.1.3/src/cybereason/_patch.py` & `cybereason-0.2.0/src/cybereason/_patch.py`

 * *Files identical despite different names*

### Comparing `cybereason-0.1.3/src/cybereason/_typing.py` & `cybereason-0.2.0/src/cybereason/_typing.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     class CybereasonProtocol(Protocol):
         proxy:     Optional[str]
         totp_code: Optional[str]
 
         @property
         def session(self) -> AsyncClient: ...
 
+        def check_resp(self, resp: dict[str, Any]) -> Any: ...
         async def get(self, path: UrlPath, query: Query=None, raw: bool=False) -> Any: ...
         async def post(self, path: UrlPath, data: Any, files: Query=None, raw_data: bool=False) -> Any: ...
         async def delete(self, path: UrlPath, query: Query=None) -> Any: ...
         async def download(self, path: UrlPath, folder: PathLike, *, query: Query=None, extract: bool=False) -> Path: ...
         async def aiter_pages(self, path: UrlPath, data: Any, key: str, page_size: int=0, sort: Literal['ASC', 'DESC']='ASC') -> AsyncIterator[Dict[str, Any]]: ...
         async def post_sage(self, path: UrlPath, data: Any) -> Any: ...
 else:
```

### Comparing `cybereason-0.1.3/src/cybereason/client.py` & `cybereason-0.2.0/src/cybereason/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,17 +9,18 @@
 import httpx
 from ._patch import normalize_and_validate
 httpx._transports.default.httpcore._async.http11.h11._headers.normalize_and_validate = normalize_and_validate  # noqa: E501
 from httpx import AsyncClient, HTTPStatusError, ConnectError
 
 from .exceptions import (
     AccessDenied, AuthenticationError, ResourceNotFoundError,
-    UnauthorizedRequest, CybereasonException, ServerError, ClientError,
+    UnauthorizedRequest, ServerError, ClientError,
+    get_response_error,
 )
-from .utils import get_filename, to_list
+from .utils import get_filename, to_list, get_config_from_env, parse_query_response
 from .custom_rules import CustomRulesMixin
 from .incident_reponse import IncidentResponseMixin
 from .malops import MalopsMixin
 from .sensors import SensorsMixin
 from .system import SystemMixin
 from .threat_intel import ThreatIntelligenceMixin
 
@@ -43,33 +44,33 @@
     MalopsMixin,
     SensorsMixin,
     SystemMixin,
     ThreatIntelligenceMixin,
 ):
     def __init__(
         self,
-        server:    str,
+        tenant:    str,
         username:  str,
         password:  str,
         proxy:     Optional[str] = None,
         totp_code: Optional[str] = None,
         timeout:   float = DEFAULT_TIMEOUT,
     ):
-        self.server = server.split('.')[0]
+        self.tenant = tenant.split('.')[0]
         self.username = username
         self.password = password
         self.proxy = proxy
         self.totp_code = totp_code
         self.timeout = timeout
 
     @cached_property
     def session(self) -> AsyncClient:
         from . import __version__
 
-        base_url = f'https://{self.server}.cybereason.net'
+        base_url = f'https://{self.tenant}.cybereason.net'
         headers  = {
             'content-type': 'application/json',
             'user-agent': f'python-cybereason/{".".join(map(str, __version__))}',
         }
 
         if self.proxy and self.proxy.startswith('socks'):
             # https://github.com/encode/httpx/discussions/2305
@@ -107,15 +108,15 @@
         )
 
     async def login(self) -> None:
         headers = {'content-type': 'application/x-www-form-urlencoded'}
         options = {'headers': headers, 'follow_redirects': True}
 
         auth = {'username': self.username, 'password': self.password}
-        log.debug('Logging %r in on %r', self.username, self.server)
+        log.debug('Logging %r in on %r', self.username, self.tenant)
 
         try:
             resp = await self.session.post('login.html', data=auth, **options)  # type: ignore
         except ConnectError as e:
             raise ConnectionError(e) from None
 
         if 'error' in str(resp.url):
@@ -150,14 +151,21 @@
         return self
 
     async def __aexit__(self, exc_type, exc_value, traceback) -> None:
         await self.aclose()
         if exc_type:
             raise exc_type(*to_list(exc_value))
 
+    @classmethod
+    def from_env(cls) -> 'Cybereason':
+        '''Retrieves class parameters from environment variables.
+        '''
+        config = get_config_from_env(cls)
+        return cls(**config)
+
     async def aclose(self) -> None:
         if 'session' in self.__dict__:
             await self.logout()
             await self.session.aclose()
         if 'session_sage' in self.__dict__:
             await self.session_sage.aclose()
 
@@ -174,14 +182,21 @@
 
         async def run_task(task):
             async with semaphore:
                 return await task
 
         return await asyncio.gather(*(run_task(task) for task in tasks))
 
+    def check_resp(self, resp):
+        if resp['status'] == 'SUCCESS':
+            return resp['data']
+        else:
+            exc = get_response_error(resp['status'])
+            raise exc(resp.get('message'))
+
     async def _request(
         self,
         method:   str,
         path:     'UrlPath',
         data:     Any = None,
         query:    'Query' = None,
         files:    'Query' = None,
@@ -269,44 +284,38 @@
         self,
         path:     'UrlPath',
         folder:   'PathLike',
         *, query: 'Query' = None,
         extract:  bool = False,
     ) -> Path:
         filename, buffer = await self.raw_download(path, query=query)
-        unknown = False
         folder = Path(folder)
         folder.mkdir(exist_ok=True, parents=True)
 
-        if extract:
+        if extract and filename.endswith(('.zip', '.gz')):
             openfile: 'Callable[[Any], Union[TarFile, ZipFile]]'
-
             subfolder, ext = filename.rsplit('.', 1)
             if ext == 'zip':
                 import zipfile
                 openfile = lambda b: zipfile.ZipFile(b, mode='r')
-            elif ext == 'gz':
+            else:  # gz
                 import tarfile
                 openfile = lambda b: tarfile.open(fileobj=b, mode='r:gz')
-            else:
-                unknown = True
-                log.warning('Unknown compression method: %s', filename)
 
-            if not unknown:
-                destpath = folder / subfolder
-                archive = openfile(buffer)
-                archive.extractall(path=destpath)
-                log.info('%s extracted into %s', filename, destpath)
+            destpath = folder / subfolder
+            archive = openfile(buffer)
+            archive.extractall(path=destpath)
+            log.info('%s extracted into %s', filename, destpath)
 
-        if not extract or unknown:
-            destpath = folder / filename
-
-            with open(folder / filename, 'wb') as f:
-                f.write(buffer.read())
+        else:
+            if extract:
+                log.warning('Unknown compression method: %s', filename)
 
+            destpath = folder / filename
+            destpath.write_bytes(buffer.read())
             log.info('%s saved as %s', filename, destpath)
 
         return destpath.resolve()
 
     async def aiter_pages(
         self,
         path:          'UrlPath',
@@ -429,25 +438,28 @@
         _, archive = await self.raw_download('monitor/global/userAuditLog')
         async for content in extract_logfiles(archive, 'userAuditSyslog', rotated):
             # yield latest logs first
             for line in content.splitlines()[::-1]:
                 yield cefparse(line.decode())
 
     # https://nest.cybereason.com/documentation/api-documentation/all-versions/how-build-queries
-    async def query(self, data: 'Dict[str, Any]') -> 'Dict[str, Any]':
+    async def query(self, query: 'Dict[str, Any]', parsed: bool = True) -> 'Dict[str, Any]':
         # default since version 20.1.381
-        data.setdefault('perGroupLimit', 100)
-        if data['perGroupLimit'] > 1000:
-            data['perGroupLimit'] = 1000
-
-        # log.debug('Running query %s', data)
-        resp = await self.post('visualsearch/query/simple', data)
-        if resp['status'] == 'FAILURE':
-            raise CybereasonException(resp['message'])
-        return resp['data']
+        query.setdefault('perGroupLimit', 100)
+        if query['perGroupLimit'] > 1000:
+            query['perGroupLimit'] = 1000
+
+        # log.debug('Running query %s', query)
+        resp = await self.post('visualsearch/query/simple', query)
+        data = self.check_resp(resp)
+
+        if parsed is True:
+            return parse_query_response(data)
+        else:
+            return data
 
     # TODO: https://nest.cybereason.com/documentation/product-documentation/221/machine-timeline
     async def get_process_timeline(self, guid: str, minutes: int):
         '''
         Provides additional context for a process by displaying details
         about sensor activity before and after the selected event,
         within a certain time frame.
```

### Comparing `cybereason-0.1.3/src/cybereason/custom_rules.py` & `cybereason-0.2.0/src/cybereason/custom_rules.py`

 * *Files identical despite different names*

### Comparing `cybereason-0.1.3/src/cybereason/incident_reponse.py` & `cybereason-0.2.0/src/cybereason/incident_reponse.py`

 * *Files identical despite different names*

### Comparing `cybereason-0.1.3/src/cybereason/malops.py` & `cybereason-0.2.0/src/cybereason/malops.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from datetime import datetime, date, timezone
 from typing import TYPE_CHECKING
 import logging
 
-from .exceptions import CybereasonException, authz, min_version
+from .exceptions import authz, min_version
+from .utils import parse_query_response
 from ._typing import CybereasonProtocol
 
 if TYPE_CHECKING:
     from typing import Any, AsyncIterator, Dict, List, Optional, Union
     from ._typing import MalopId
 
     Label = Dict[str, Union[str, int]]
@@ -42,64 +43,66 @@
 
         return (await self.post('detection/inbox', data))['malops']
 
     async def get_active_malops(self, logon: bool = False) -> 'AsyncIterator[Dict[str, Any]]':
         '''Get all malops currently active.
         '''
 
-        data = {
+        payload = {
             'totalResultLimit': 10000,
             'perGroupLimit':    10000,
             'perFeatureLimit':  100,
             'templateContext':  'OVERVIEW',
             'customFields':     [],
             'queryPath':        [{'result': True, 'filters': None}],
         }
 
         for req_type in ('MalopProcess', 'MalopLogonSession'):
-            data['queryPath'][0]['requestedType'] = req_type  # type: ignore
-
-            resp = await self.post('crimes/unified', data)
+            payload['queryPath'][0]['requestedType'] = req_type  # type: ignore
 
-            if not resp['status'] == 'SUCCESS':
-                raise CybereasonException(resp['message'])
+            resp = await self.post('crimes/unified', payload)
+            data = self.check_resp(resp)
 
-            for malop in resp['data']['resultIdToElementDataMap'].values():
-                yield malop
+            for malop in data['resultIdToElementDataMap'].values():
+                yield parse_query_response(malop)
 
     # TODO: retrieve details for Auto Hunt Malops
     # TODO: endpoint fails
     # @min_version(20, 1, 43)
     # async def get_edr_malop_details(self, malop_id: 'MalopId'):
     #     '''Returns details about a specified Endpoint Protection Malop.
     #     '''
     #     data = {'malopGuid': malop_id}
     #     return await self.post('detection/details', data)
 
+    async def get_malop_status(self, malop_id: 'MalopId') -> 'Dict[str, Any]':
+        resp = await self.get(f'mmng/v2/malops/metadata/{malop_id}')
+        return self.check_resp(resp)
+
     async def has_malop_history(self, malop_id: 'MalopId') -> bool:
         data = {'guids': [malop_id], 'elementType': 'MalopProcess'}
         return await self.post('remediate/has-history', data)  # TODO: also bool if True?
 
-    @min_version(17, 5)
-    @authz('Analyst L1')
-    async def get_malware_alerts(self, filters=None) -> 'AsyncIterator[Any]':
-        data = {'filters': filters or [], 'sortingFieldName': 'timestamp'}
-        async for alert in self.aiter_pages('malware/query', data, key='malwares'):
-            yield alert
-
     async def get_malop_comments(
         self, malop_id: 'MalopId',
     ) -> 'List[Dict[str, Union[str, int]]]':
         from html import unescape
 
         resp = await self.post('crimes/get-comments', malop_id, raw_data=True)
         for msg in resp:
             msg['message'] = unescape(msg['message'])
         return resp
 
+    @min_version(17, 5)
+    @authz('Analyst L1')
+    async def get_malware_alerts(self, filters=None) -> 'AsyncIterator[Any]':
+        data = {'filters': filters or [], 'sortingFieldName': 'timestamp'}
+        async for alert in self.aiter_pages('malware/query', data, key='malwares'):
+            yield alert
+
 # region LABELS
     @min_version(20, 1, 43)
     async def get_malops_labels(
         self, malops_ids: 'Optional[List[MalopId]]' = None
     ) -> 'List[Label]':
         '''Returns a list of all Malop labels.
```

### Comparing `cybereason-0.1.3/src/cybereason/parse/cef.py` & `cybereason-0.2.0/src/cybereason/parse/cef.py`

 * *Files identical despite different names*

### Comparing `cybereason-0.1.3/src/cybereason/parse/server.py` & `cybereason-0.2.0/src/cybereason/parse/server.py`

 * *Files identical despite different names*

### Comparing `cybereason-0.1.3/src/cybereason/sensors.py` & `cybereason-0.2.0/src/cybereason/sensors.py`

 * *Files identical despite different names*

### Comparing `cybereason-0.1.3/src/cybereason/system.py` & `cybereason-0.2.0/src/cybereason/system.py`

 * *Files identical despite different names*

### Comparing `cybereason-0.1.3/src/cybereason/threat_intel.py` & `cybereason-0.2.0/src/cybereason/threat_intel.py`

 * *Files identical despite different names*

### Comparing `cybereason-0.1.3/src/cybereason/utils/guid.py` & `cybereason-0.2.0/src/cybereason/utils/guid.py`

 * *Files identical despite different names*

### Comparing `cybereason-0.1.3/src/cybereason.egg-info/PKG-INFO` & `cybereason-0.2.0/src/cybereason.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybereason
-Version: 0.1.3
+Version: 0.2.0
 Summary: Async Cybereason API client
 Home-page: https://github.com/forensic-security/cybereason#readme
 Author: Nuno André
 Author-email: mail@nunoand.re
 License: BSD-3-Clause
 Project-URL: Source, https://github.com/forensic-security/cybereason
 Project-URL: Bug Tracker, https://github.com/forensic-security/cybereason/issues
@@ -60,15 +60,15 @@
 from cybereason import Cybereason
 import asyncio
 import json
 
 async def dump_policies_config():
     '''Save metadata and config for every policy.
     '''
-    async with Cybereason(<server>, <username>, <password>) as client:
+    async with Cybereason(<tenant>, <username>, <password>) as client:
         async for policy in client.get_policies(show_config=True):
             filename = f'{policy["metadata"]["name"]}.json'
             with open(filename, 'w') as f:
                 json.dump(policy, f, indent=4)
 
 asyncio.run(dump_policies_config())
 ```
@@ -76,15 +76,15 @@
 ### Download and parse into JSON all user audit logs (action log)
 ```python
 from cybereason import Cybereason
 import asyncio
 import json
 
 async def user_audit():
-    async with Cybereason(<server>, <username>, <password>) as client:
+    async with Cybereason(<tenant>, <username>, <password>) as client:
         # rotated=False to get only the latest logs
         logs = [log async for log in client.get_user_audit_logs(rotated=True)]
         with open('user_audit.json', 'w') as f:
             json.dump(logs, f, indent=4)
 
 asyncio.run(user_audit())
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cybereason Version: 0.1.3 Summary: Async Cybereason
+Metadata-Version: 2.1 Name: cybereason Version: 0.2.0 Summary: Async Cybereason
 API client Home-page: https://github.com/forensic-security/cybereason#readme
 Author: Nuno AndrÃ© Author-email: mail@nunoand.re License: BSD-3-Clause
 Project-URL: Source, https://github.com/forensic-security/cybereason Project-
 URL: Bug Tracker, https://github.com/forensic-security/cybereason/issues
 Keywords: cybereason,cybersecurity,security,edr Platform: any Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators Classifier: Framework ::
```

### Comparing `cybereason-0.1.3/src/cybereason.egg-info/SOURCES.txt` & `cybereason-0.2.0/src/cybereason.egg-info/SOURCES.txt`

 * *Files identical despite different names*

