# Comparing `tmp/python-dxf-8.0.2.tar.gz` & `tmp/python-dxf-9.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-dxf-8.0.2.tar", last modified: Thu Feb  9 20:49:05 2023, max compression
+gzip compressed data, was "python-dxf-9.0.1.tar", last modified: Sat Feb 11 21:24:50 2023, max compression
```

## Comparing `python-dxf-8.0.2.tar` & `python-dxf-9.0.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-02-09 20:49:05.084382 python-dxf-8.0.2/
--rw-r--r--   0 david     (1000) david     (1000)     1089 2015-12-03 10:03:59.000000 python-dxf-8.0.2/LICENCE
--rw-rw-r--   0 david     (1000) david     (1000)     9192 2023-02-09 20:49:05.084382 python-dxf-8.0.2/PKG-INFO
--rw-r--r--   0 david     (1000) david     (1000)     8880 2023-02-09 20:30:04.000000 python-dxf-8.0.2/README.rst
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-02-09 20:49:05.084382 python-dxf-8.0.2/dxf/
--rw-rw-r--   0 david     (1000) david     (1000)    37644 2023-02-09 20:07:45.000000 python-dxf-8.0.2/dxf/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)       32 2015-12-09 23:12:16.000000 python-dxf-8.0.2/dxf/__main__.py
--rw-rw-r--   0 david     (1000) david     (1000)     3080 2022-09-04 19:37:54.000000 python-dxf-8.0.2/dxf/exceptions.py
--rw-r--r--   0 david     (1000) david     (1000)     7975 2022-09-04 20:06:50.000000 python-dxf-8.0.2/dxf/main.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-02-09 20:49:05.084382 python-dxf-8.0.2/python_dxf.egg-info/
--rw-rw-r--   0 david     (1000) david     (1000)     9192 2023-02-09 20:49:05.000000 python-dxf-8.0.2/python_dxf.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)      332 2023-02-09 20:49:05.000000 python-dxf-8.0.2/python_dxf.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2023-02-09 20:49:05.000000 python-dxf-8.0.2/python_dxf.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1000) david     (1000)       39 2023-02-09 20:49:05.000000 python-dxf-8.0.2/python_dxf.egg-info/entry_points.txt
--rw-rw-r--   0 david     (1000) david     (1000)       70 2023-02-09 20:49:05.000000 python-dxf-8.0.2/python_dxf.egg-info/requires.txt
--rw-rw-r--   0 david     (1000) david     (1000)        4 2023-02-09 20:49:05.000000 python-dxf-8.0.2/python_dxf.egg-info/top_level.txt
--rw-rw-r--   0 david     (1000) david     (1000)       38 2023-02-09 20:49:05.084382 python-dxf-8.0.2/setup.cfg
--rw-rw-r--   0 david     (1000) david     (1000)      785 2023-02-09 20:28:39.000000 python-dxf-8.0.2/setup.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-02-09 20:49:05.084382 python-dxf-8.0.2/test/
--rw-r--r--   0 david     (1000) david     (1000)    17258 2021-12-13 20:00:54.000000 python-dxf-8.0.2/test/test_cli.py
--rw-r--r--   0 david     (1000) david     (1000)    10654 2021-12-13 19:47:31.000000 python-dxf-8.0.2/test/test_module.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-02-11 21:24:50.586889 python-dxf-9.0.1/
+-rw-r--r--   0 david     (1000) david     (1000)     1089 2015-12-03 10:03:59.000000 python-dxf-9.0.1/LICENCE
+-rw-rw-r--   0 david     (1000) david     (1000)     9192 2023-02-11 21:24:50.586889 python-dxf-9.0.1/PKG-INFO
+-rw-r--r--   0 david     (1000) david     (1000)     8880 2023-02-11 20:46:19.000000 python-dxf-9.0.1/README.rst
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-02-11 21:24:50.586889 python-dxf-9.0.1/dxf/
+-rw-rw-r--   0 david     (1000) david     (1000)    37108 2023-02-11 21:02:40.000000 python-dxf-9.0.1/dxf/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)       32 2015-12-09 23:12:16.000000 python-dxf-9.0.1/dxf/__main__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3080 2022-09-04 19:37:54.000000 python-dxf-9.0.1/dxf/exceptions.py
+-rw-rw-r--   0 david     (1000) david     (1000)     7995 2023-02-11 19:40:23.000000 python-dxf-9.0.1/dxf/main.py
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2023-02-11 19:40:23.000000 python-dxf-9.0.1/dxf/py.typed
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-02-11 21:24:50.586889 python-dxf-9.0.1/python_dxf.egg-info/
+-rw-rw-r--   0 david     (1000) david     (1000)     9192 2023-02-11 21:24:50.000000 python-dxf-9.0.1/python_dxf.egg-info/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)      345 2023-02-11 21:24:50.000000 python-dxf-9.0.1/python_dxf.egg-info/SOURCES.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2023-02-11 21:24:50.000000 python-dxf-9.0.1/python_dxf.egg-info/dependency_links.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       39 2023-02-11 21:24:50.000000 python-dxf-9.0.1/python_dxf.egg-info/entry_points.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       70 2023-02-11 21:24:50.000000 python-dxf-9.0.1/python_dxf.egg-info/requires.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        4 2023-02-11 21:24:50.000000 python-dxf-9.0.1/python_dxf.egg-info/top_level.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       38 2023-02-11 21:24:50.586889 python-dxf-9.0.1/setup.cfg
+-rw-rw-r--   0 david     (1000) david     (1000)      825 2023-02-11 21:02:40.000000 python-dxf-9.0.1/setup.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2023-02-11 21:24:50.586889 python-dxf-9.0.1/test/
+-rw-r--r--   0 david     (1000) david     (1000)    17258 2021-12-13 20:00:54.000000 python-dxf-9.0.1/test/test_cli.py
+-rw-r--r--   0 david     (1000) david     (1000)    10654 2021-12-13 19:47:31.000000 python-dxf-9.0.1/test/test_module.py
```

### Comparing `python-dxf-8.0.2/LICENCE` & `python-dxf-9.0.1/LICENCE`

 * *Files identical despite different names*

### Comparing `python-dxf-8.0.2/PKG-INFO` & `python-dxf-9.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: python-dxf
-Version: 8.0.2
+Version: 9.0.1
 Summary: Package for accessing a Docker v2 registry
 Home-page: https://github.com/davedoesdev/dxf
 Author: David Halls
 Author-email: dave@davedoesdev.com
 License: MIT
 Keywords: docker registry
 Platform: UNKNOWN
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 License-File: LICENCE
 
 |Build Status| |Coverage Status| |PyPI version|
 
 Python module and command-line tool for storing and retrieving data in a
 Docker registry.
```

### Comparing `python-dxf-8.0.2/README.rst` & `python-dxf-9.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `python-dxf-8.0.2/dxf/__init__.py` & `python-dxf-9.0.1/dxf/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,72 +1,80 @@
 """
 Module for accessing a Docker v2 Registry
 """
 
+from typing import Optional, Union, List, Callable, Iterable, Type, Iterator, TypeVar, Tuple, TYPE_CHECKING, Dict, cast
+from types import ModuleType
 import base64
 import hashlib
 import json
 import sys
 import warnings
 
-try:
-    import urllib.parse as urlparse
-    from urllib.parse import urlencode
-except ImportError:
-    # pylint: disable=import-error,no-name-in-module,wrong-import-order
-    from urllib import urlencode
-    import urlparse
+import urllib.parse as urlparse
+from urllib.parse import urlencode
 
 import requests
-try:
-    from requests.packages import urllib3
-except ImportError:
-    import urllib3
 from urllib3.exceptions import InsecureRequestWarning
 
-from jwcrypto import jwk, jws
-import www_authenticate
+from jwcrypto import jwk, jws # type: ignore
+import www_authenticate # type: ignore
 # pylint: disable=wildcard-import
 from dxf import exceptions
 
+_schema1_mimetype = 'application/vnd.docker.distribution.manifest.v1+json'
+
 _schema2_mimetype = 'application/vnd.docker.distribution.manifest.v2+json'
 _schema2_list_mimetype = 'application/vnd.docker.distribution.manifest.list.v2+json'
 
+# OCIv1 equivalent of a docker registry v2 manifests
+_ociv1_manifest_mimetype = 'application/vnd.oci.image.manifest.v1+json'
+# OCIv1 equivalent of a docker registry v2 "manifests list"
+_ociv1_index_mimetype = 'application/vnd.oci.image.index.v1+json'
+
+_accept_header = {'Accept': ', '.join((
+    _schema1_mimetype,
+    _schema2_mimetype,
+    _schema2_list_mimetype,
+    _ociv1_manifest_mimetype,
+    _ociv1_index_mimetype,
+))}
+
 if sys.version_info < (3, 0):
     _binary_type = str
 else:
     _binary_type = bytes
     # pylint: disable=redefined-builtin
     long = int
 
+# Note: From Python 3.11 onwards we can use typing.Self instead of these
+T = TypeVar('T', bound='DXFBase')
+TD = TypeVar('TD', bound='DXF')
+
 def _to_bytes_2and3(s):
     return s if isinstance(s, _binary_type) else s.encode('utf-8')
 
-def hash_bytes(buf):
+def hash_bytes(buf: _binary_type) -> str:
     """
     Hash bytes using the same method the registry uses (currently SHA-256).
 
     :param buf: Bytes to hash
-    :type buf: binary str
 
-    :rtype: str
     :returns: Hex-encoded hash of file's content (prefixed by ``sha256:``)
     """
     sha256 = hashlib.sha256()
     sha256.update(buf)
     return 'sha256:' + sha256.hexdigest()
 
-def hash_file(filename):
+def hash_file(filename: str) -> str:
     """
     Hash a file using the same method the registry uses (currently SHA-256).
 
     :param filename: Name of file to hash
-    :type filename: str
 
-    :rtype: str
     :returns: Hex-encoded hash of file's content (prefixed by ``sha256:``)
     """
     sha256 = hashlib.sha256()
     with open(filename, 'rb') as f:
         for chunk in iter(lambda: f.read(8192), b''):
             sha256.update(chunk)
     return 'sha256:' + sha256.hexdigest()
@@ -125,15 +133,15 @@
 class PaginatingResponse(object):
     # pylint: disable=too-few-public-methods
     def __init__(self, dxf_obj, req_meth, path, header, **kwargs):
         self._meth = getattr(dxf_obj, req_meth)
         self._path = path
         self._header = header
         self._kwargs = kwargs
-    def __iter__(self):
+    def __iter__(self) -> Iterator[str]:
         while self._path:
             response = self._meth('get', self._path, **self._kwargs)
             self._kwargs = {}
             for v in response.json()[self._header] or []:
                 yield v
             nxt = response.links.get('next')
             self._path = nxt['url'] if nxt else None
@@ -155,45 +163,39 @@
     When the context exits, all the session's connections are closed.
 
     If you don't use :class:`DXFBase` as a context manager, each request
     uses an ephemeral session. If you don't read all the data from an iterator
     returned by :meth:`DXF.pull_blob` then the underlying connection won't be
     closed until Python garbage collects the iterator.
     """
-    def __init__(self, host,
-                 auth=None, insecure=False, auth_host=None, tlsverify=True, timeout=None):
+    def __init__(self, host: str,
+            auth: Optional[Callable[['DXFBase', requests.Response], None]]=None, insecure: bool=False, auth_host: Optional[str]=None, tlsverify: Union[bool, str]=True, timeout: Optional[float]=None):
         # pylint: disable=too-many-arguments
         """
         :param host: Host name of registry. Can contain port numbers. e.g. ``registry-1.docker.io``, ``localhost:5000``.
-        :type host: str
 
         :param auth: Authentication function to be called whenever authentication to the registry is required. Receives the :class:`DXFBase` object and a HTTP response object. It should call :meth:`authenticate` with a username, password and ``response`` before it returns.
-        :type auth: function(dxf_obj, response)
 
         :param insecure: Use HTTP instead of HTTPS (which is the default) when connecting to the registry.
-        :type insecure: bool
 
         :param auth_host: Host to use for token authentication. If set, overrides host returned by then registry.
-        :type auth_host: str
 
         :param tlsverify: When set to False, do not verify TLS certificate. When pointed to a `<ca bundle>.crt` file use this for TLS verification. See `requests.verify <http://docs.python-requests.org/en/latest/user/advanced/#ssl-cert-verification>`_ for more details.
-        :type tlsverify: bool or str
 
         :param timeout: Optional timeout for requests. See `requests.timeout <https://requests.readthedocs.io/en/latest/user/quickstart/#timeouts>`_ for more details.
-        :type timeout: float
         """
         self._base_url = ('http' if insecure else 'https') + '://' + host + '/v2/'
         self._host = host
         self._auth = auth
         self._insecure = insecure
         self._auth_host = auth_host
         self._token = None
-        self._headers = {}
-        self._repo = None
-        self._sessions = [requests]
+        self._headers: Dict[str, str] = {}
+        self._repo: Optional[str] = None
+        self._sessions: List[Union[ModuleType, requests.Session]] = [requests]
         self._tlsverify = tlsverify
         self._timeout = timeout
 
     @property
     def token(self):
         """
         str: Authentication token. This will be obtained automatically when
@@ -229,42 +231,35 @@
                 with warnings.catch_warnings():
                     _ignore_warnings(self)
                     r = getattr(self._sessions[0], method)(url, **make_kwargs())
         _raise_for_status(r)
         return r
 
     def authenticate(self,
-                     username=None, password=None,
-                     actions=None, response=None,
-                     authorization=None,
-                     user_agent='Docker-Client/19.03.2 (linux)'):
+            username: Optional[str]=None, password: Optional[str]=None,
+            actions: Optional[List[str]]=None, response: Optional[requests.Response]=None,
+            authorization: Optional[str]=None,
+            user_agent: str='Docker-Client/19.03.2 (linux)') -> Optional[str]:
         # pylint: disable=too-many-arguments,too-many-locals,too-many-branches
         """
         Authenticate to the registry using a username and password,
         an authorization header or otherwise as the anonymous user.
 
         :param username: User name to authenticate as.
-        :type username: str
 
         :param password: User's password.
-        :type password: str
 
         :param actions: If you know which types of operation you need to make on the registry, specify them here. Valid actions are ``pull``, ``push`` and ``*``.
-        :type actions: list
 
         :param response: When the ``auth`` function you passed to :class:`DXFBase`'s constructor is called, it is passed a HTTP response object. Pass it back to :meth:`authenticate` to have it automatically detect which actions are required.
-        :type response: requests.Response
 
         :param authorization: ``Authorization`` header value.
-        :type authorization: str
 
         :param user_agent: ``User-Agent`` header value.
-        :type user_agent: str
 
-        :rtype: str
         :returns: Authentication token, if the registry supports bearer tokens. Otherwise ``None``, and HTTP Basic auth is used (if the registry requires authentication).
         """
         if response is None:
             with warnings.catch_warnings():
                 _ignore_warnings(self)
                 response = self._sessions[0].get(self._base_url,
                                                  verify=self._tlsverify,
@@ -326,33 +321,30 @@
             # Use 'access_token' value if present and not empty, else 'token' value.
             self.token = rjson.get('access_token') or rjson['token']
             return self._token
 
         self._headers = headers
         return None
 
-    def list_repos(self, batch_size=None, iterate=False):
+    def list_repos(self, batch_size: Optional[int]=None, iterate: bool=False) -> Union[List[str], Iterable[str]]:
         """
         List all repositories in the registry.
 
         :param batch_size: Number of repository names to ask the server for at a time.
-        :type batch_size: int
 
         :param iterate: Whether to return iterator over the names or a list of all the names.
-        :type iterate: bool
 
-        :rtype: list or iterator of strings
         :returns: Repository names.
         """
         it = PaginatingResponse(self, '_base_request',
                                 '_catalog', 'repositories',
                                 params={'n': batch_size})
         return it if iterate else list(it)
 
-    def __enter__(self):
+    def __enter__(self: T) -> T:
         assert self._sessions
         session = requests.Session()
         session.__enter__()
         self._sessions.insert(0, session)
         return self
 
     def __exit__(self, *args):
@@ -362,37 +354,30 @@
 
 class DXF(DXFBase):
     """
     Class for operating on a Docker v2 repositories.
     """
     # pylint: disable=too-many-instance-attributes
 
-    def __init__(self, host, repo, auth=None, insecure=False, auth_host=None, tlsverify=True, timeout=None):
+    def __init__(self: TD, host: str, repo: str, auth: Optional[Callable[['DXFBase', requests.Response], None]]=None, insecure: bool=False, auth_host: Optional[str]=None, tlsverify: Union[bool, str]=True, timeout: Optional[float]=None):
         # pylint: disable=too-many-arguments
         """
         :param host: Host name of registry. Can contain port numbers. e.g. ``registry-1.docker.io``, ``localhost:5000``.
-        :type host: str
 
         :param repo: Name of the repository to access on the registry. Typically this is of the form ``username/reponame`` but for your own registries you don't actually have to stick to that.
-        :type repo: str
 
         :param auth: Authentication function to be called whenever authentication to the registry is required. Receives the :class:`DXF` object and a HTTP response object. It should call :meth:`DXFBase.authenticate` with a username, password and ``response`` before it returns.
-        :type auth: function(dxf_obj, response)
 
         :param insecure: Use HTTP instead of HTTPS (which is the default) when connecting to the registry.
-        :type insecure: bool
 
         :param auth_host: Host to use for token authentication. If set, overrides host returned by then registry.
-        :type auth_host: str
 
         :param tlsverify: When set to False, do not verify TLS certificate. When pointed to a `<ca bundle>.crt` file use this for TLS verification. See `requests.verify <http://docs.python-requests.org/en/latest/user/advanced/#ssl-cert-verification>`_ for more details.
-        :type tlsverify: bool or str
 
         :param timeout: Optional timeout for requests. See `requests.timeout <https://requests.readthedocs.io/en/latest/user/quickstart/#timeouts>`_ for more details.
-        :type timeout: float
         """
         super(DXF, self).__init__(host, auth, insecure, auth_host, tlsverify, timeout)
         self._repo = repo
         self._repo_path = self._get_repo_path(repo)
 
     def _get_repo_path(self, repo, suffix='/'):
         repo_path = ''
@@ -405,87 +390,79 @@
     def _request(self, method, path, **kwargs):
         return self._base_request(
             method,
             urlparse.urljoin(self._repo_path, path),
             **kwargs)
 
     def push_blob(self,
-                  filename=None,
-                  progress=None,
-                  data=None, digest=None,
-                  check_exists=True):
+            filename: Optional[str]=None,
+            progress: Optional[Callable[[str, _binary_type, int], None]]=None,
+            data: Optional[Iterable[_binary_type]]=None, digest: Optional[str]=None,
+            check_exists: bool=True) -> str:
         # pylint: disable=too-many-arguments
         """
         Upload a file to the registry and return its (SHA-256) hash.
 
         The registry is content-addressable so the file's content (aka blob)
         can be retrieved later by passing the hash to :meth:`pull_blob`.
 
         :param filename: File to upload.
-        :type filename: str
 
         :param data: Data to upload if ``filename`` isn't given. The data is uploaded in chunks and you must also pass ``digest``.
-        :type data: Generator or iterator
 
         :param digest: Hash of the data to be uploaded in ``data``, if specified.
-        :type digest: str (hex-encoded SHA-256, prefixed by ``sha256:``)
 
         :param progress: Optional function to call as the upload progresses. The function will be called with the hash of the file's content (or ``digest``), the blob just read from the file (or chunk from ``data``) and if ``filename`` is specified the total size of the file.
-        :type progress: function(dgst, chunk, size)
 
         :param check_exists: Whether to check if a blob with the same hash already exists in the registry. If so, it won't be uploaded again.
-        :type check_exists: bool
 
-        :rtype: str
         :returns: Hash of file's content.
         """
         if filename is None:
             dgst = digest
+            if dgst is None:
+                raise TypeError("digest must be provided if filename is None")
         else:
             dgst = hash_file(filename)
         if check_exists:
             try:
                 self._request('head', 'blobs/' + dgst)
                 return dgst
             except requests.exceptions.HTTPError as ex:
                 # pylint: disable=no-member
                 if ex.response.status_code != requests.codes.not_found:
                     raise
         r = self._request('post', 'blobs/uploads/')
         upload_url = r.headers['Location']
         url_parts = list(urlparse.urlparse(upload_url))
         query = urlparse.parse_qs(url_parts[4])
-        query.update({'digest': dgst})
+        query.update({'digest': [dgst]})
         url_parts[4] = urlencode(query, True)
         url_parts[0] = 'http' if self._insecure else 'https'
         upload_url = urlparse.urlunparse(url_parts)
         if filename is None:
             data = _ReportingChunks(dgst, data, progress) if progress else data
             self._base_request('put', upload_url, data=data)
         else:
             with open(filename, 'rb') as f:
                 data = _ReportingFile(dgst, f, progress) if progress else f
                 self._base_request('put', upload_url, data=data)
         return dgst
 
     # pylint: disable=no-self-use
-    def pull_blob(self, digest, size=False, chunk_size=None):
+    def pull_blob(self, digest: str, size: bool=False, chunk_size: Optional[int]=None) -> Union[Iterable[_binary_type], Tuple[Iterable[_binary_type], long]]:
         """
         Download a blob from the registry given the hash of its content.
 
         :param digest: Hash of the blob's content (prefixed by ``sha256:``).
-        :type digest: str
 
         :param size: Whether to return the size of the blob too.
-        :type size: bool
 
         :param chunk_size: Number of bytes to download at a time. Defaults to 8192.
-        :type chunk_size: int
 
-        :rtype: iterator
         :returns: If ``size`` is falsey, a byte string iterator over the blob's content. If ``size`` is truthy, a tuple containing the iterator and the blob's size.
         """
         if chunk_size is None:
             chunk_size = 8192
         r = self._request('get', 'blobs/' + digest, stream=True)
         class Chunks(object):
             # pylint: disable=too-few-public-methods
@@ -495,55 +472,49 @@
                     sha256.update(chunk)
                     yield chunk
                 dgst = 'sha256:' + sha256.hexdigest()
                 if dgst != digest:
                     raise exceptions.DXFDigestMismatchError(dgst, digest)
         return (Chunks(), long(r.headers['content-length'])) if size else Chunks()
 
-    def blob_size(self, digest):
+    def blob_size(self, digest: str) -> long:
         """
         Return the size of a blob in the registry given the hash of its content.
 
         :param digest: Hash of the blob's content (prefixed by ``sha256:``).
-        :type digest: str
 
-        :rtype: long
         :returns: Size of the blob in bytes.
         """
         r = self._request('head', 'blobs/' + digest)
         return long(r.headers['content-length'])
 
-    def mount_blob(self, repo, digest):
+    def mount_blob(self, repo: str, digest: str) -> str:
         """
         Mount a blob from another repository in the registry.
 
         :param repo: Repository containing the existing blob.
-        :type repo: str
 
         :param digest: Hash of the existing blob's content (prefixed by ``sha256:``).
-        :type digest: str
 
-        :rtype: str
         :returns: Hash of blob's content.
         """
         r = self._request('post', 'blobs/uploads/?' + urlencode({
             'mount': digest,
             'from': self._get_repo_path(repo, suffix='')
         }))
         # pylint: disable=no-member
         if r.status_code != requests.codes.created:
             raise exceptions.DXFMountFailed()
         return r.headers.get('Docker-Content-Digest')
 
-    def del_blob(self, digest):
+    def del_blob(self, digest: str):
         """
         Delete a blob from the registry given the hash of its content.
 
         :param digest: Hash of the blob's content (prefixed by ``sha256:``).
-        :type digest: str
         """
         self._request('delete', 'blobs/' + digest)
 
     # For dtuf; highly unlikely anyone else will want this
     def make_manifest(self, *digests):
         layers = [{
             'mediaType': 'application/octet-stream',
@@ -560,43 +531,38 @@
                 'mediaType': 'application/vnd.docker.container.image.v1+json',
                 'size': layers[0]['size'],
                 'digest': layers[0]['digest']
             },
             'layers': layers
         }, sort_keys=True)
 
-    def set_manifest(self, alias, manifest_json):
+    def set_manifest(self, alias: str, manifest_json: str):
         """
         Give a name (alias) to a manifest.
 
         :param alias: Alias name
-        :type alias: str
 
         :param manifest_json: A V2 Schema 2 manifest JSON string
-        :type digests: list
         """
         media_type = json.loads(manifest_json)['mediaType']
         self._request('put',
                       'manifests/' + alias,
                       data=manifest_json,
                       headers={'Content-Type': media_type})
 
-    def set_alias(self, alias, *digests):
+    def set_alias(self, alias: str, *digests: str) -> str:
         # pylint: disable=too-many-locals
         """
         Give a name (alias) to a set of blobs. Each blob is specified by
         the hash of its content.
 
         :param alias: Alias name
-        :type alias: str
 
         :param digests: List of blob hashes (prefixed by ``sha256:``).
-        :type digests: list of strings
 
-        :rtype: str
         :returns: The registry manifest used to define the alias. You almost definitely won't need this.
         """
         try:
             manifest_json = self.make_manifest(*digests)
             self.set_manifest(alias, manifest_json)
             return manifest_json
         except requests.exceptions.HTTPError as ex:
@@ -604,41 +570,35 @@
             if ex.response.status_code != requests.codes.bad_request:
                 raise
             manifest_json = self.make_unsigned_manifest(alias, *digests)
             signed_json = _sign_manifest(manifest_json)
             self._request('put', 'manifests/' + alias, data=signed_json)
             return signed_json
 
-    def get_manifest_and_response(self, alias):
+    def get_manifest_and_response(self, alias: str) -> Tuple[str, requests.Response]:
         """
         Request the manifest for an alias and return the manifest and the
         response.
 
         :param alias: Alias name.
-        :type alias: str
 
-        :rtype: tuple
         :returns: Tuple containing the manifest as a string (JSON) and the `requests.Response <http://docs.python-requests.org/en/master/api/#requests.Response>`_
         """
         r = self._request('get',
                           'manifests/' + alias,
-                          headers={'Accept': ', '.join((
-                              _schema2_mimetype,
-                              _schema1_mimetype,
-                              _schema2_list_mimetype))})
+                          headers=_accept_header)
+
         return r.content.decode('utf-8'), r
 
-    def get_manifest(self, alias):
+    def get_manifest(self, alias: str) -> str:
         """
         Get the manifest for an alias
 
         :param alias: Alias name.
-        :type alias: str
 
-        :rtype: str
         :returns: The manifest as string (JSON)
         """
         manifest, _ = self.get_manifest_and_response(alias)
         return manifest
 
     def _get_alias(self, alias, manifest, verify, sizes, dcd, get_digest):
         # pylint: disable=too-many-arguments
@@ -674,97 +634,84 @@
                     method + ':' + expected_dgst)
 
         if get_digest:
             dgst = parsed_manifest['config']['digest']
             split_digest(dgst)
             return dgst
 
-        if parsed_manifest['mediaType'] == _schema2_mimetype:
+        if parsed_manifest['mediaType'] == _schema2_mimetype or parsed_manifest['mediaType'] == _ociv1_manifest_mimetype:
             blobs_key = 'layers'
-        elif parsed_manifest['mediaType'] == _schema2_list_mimetype:
+        elif parsed_manifest['mediaType'] == _schema2_list_mimetype or parsed_manifest["mediaType"] == _ociv1_index_mimetype:
             blobs_key = 'manifests'
         else:
             raise exceptions.DXFUnsupportedSchemaType(parsed_manifest['mediaType'])
 
         r = []
         for layer in parsed_manifest[blobs_key]:
             dgst = layer['digest']
             split_digest(dgst)
             r.append((dgst, layer['size']) if sizes else dgst)
         return r
 
     def get_alias(self,
-                  alias=None,
-                  manifest=None,
-                  verify=True,
-                  sizes=False,
-                  dcd=None):
+            alias: Optional[str]=None,
+            manifest: Optional[str]=None,
+            verify: bool=True,
+            sizes: bool=False,
+            dcd: Optional[str]=None) -> Union[List[str], List[Tuple[str, long]]]:
         # pylint: disable=too-many-arguments
         """
         Get the blob hashes assigned to an alias.
 
         :param alias: Alias name. You almost definitely will only need to pass this argument.
-        :type alias: str
 
         :param manifest: If you previously obtained a manifest, specify it here instead of ``alias``. You almost definitely won't need to do this.
-        :type manifest: str
 
         :param verify: (v1 schema only) Whether to verify the integrity of the alias definition in the registry itself. You almost definitely won't need to change this from the default (``True``).
-        :type verify: bool
 
         :param sizes: Whether to return sizes of the blobs along with their hashes
-        :type sizes: bool
 
         :param dcd: (if ``manifest`` is specified) The Docker-Content-Digest header returned when getting the manifest. If present, this is checked against the manifest.
-        :type dcd: str
 
-        :rtype: list
         :returns: If ``sizes`` is falsey, a list of blob hashes (strings) which are assigned to the alias. If ``sizes`` is truthy, a list of (hash,size) tuples for each blob.
         """
         return self._get_alias(alias, manifest, verify, sizes, dcd, False)
 
     def get_digest(self,
-                   alias=None,
-                   manifest=None,
-                   verify=True,
-                   dcd=None):
+            alias: Optional[str]=None,
+            manifest: Optional[str]=None,
+            verify: bool=True,
+            dcd: Optional[str]=None) -> str:
         """
         (v2 schema only) Get the hash of an alias's configuration blob.
 
         For an alias created using ``dxf``, this is the hash of the first blob
         assigned to the alias.
 
         For a Docker image tag, this is the same as
         ``docker inspect alias --format='{{.Id}}'``.
 
         :param alias: Alias name. You almost definitely will only need to pass this argument.
-        :type alias: str
 
         :param manifest: If you previously obtained a manifest, specify it here instead of ``alias``. You almost definitely won't need to do this.
-        :type manifest: str
 
         :param verify: (v1 schema only) Whether to verify the integrity of the alias definition in the registry itself. You almost definitely won't need to change this from the default (``True``).
-        :type verify: bool
 
         :param dcd: (if ``manifest`` is specified) The Docker-Content-Digest header returned when getting the manifest. If present, this is checked against the manifest.
-        :type dcd: str
 
-        :rtype: str
         :returns: Hash of the alias's configuration blob.
         """
         return self._get_alias(alias, manifest, verify, False, dcd, True)
 
-    def _get_dcd(self, alias):
+    def _get_dcd(self, alias: str) -> str:
         """
         Get the Docker-Content-Digest header for an alias.
 
         :param alias: Alias name.
-        :type alias: str
 
-        :rtype: str
         :returns: DCD header for the alias.
         """
         # https://docs.docker.com/registry/spec/api/#deleting-an-image
         # Note When deleting a manifest from a registry version 2.3 or later,
         # the Accept header must be set correctly to overlap with the mediaType
         # when HEAD or GET-ing the manifest.
         # E.g. a manifest.list type manifest contains a list of regular manifests
@@ -772,80 +719,69 @@
         # is sent when querying an alias, the registry will not return the digest
         # of the manifest.list, but instead, the digest of the first regular manifest in the list.
         # This is a valid and deletable digest, but ends up leaving the registry broken
         # as it still has the manifest-list with references to the now deleted manifest.
         return self._request(
             'head',
             'manifests/{}'.format(alias),
-            headers={'Accept': ','.join([
-                _schema2_mimetype,
-                _schema2_list_mimetype])},
+            headers=_accept_header
         ).headers.get('Docker-Content-Digest')
 
-    def del_alias(self, alias):
+    def del_alias(self, alias: str) -> List[str]:
         """
         Delete an alias from the registry. The blobs it points to won't be deleted. Use :meth:`del_blob` for that.
 
         .. Note::
            On private registry, garbage collection might need to be run manually; see:
            https://docs.docker.com/registry/garbage-collection/
 
         :param alias: Alias name.
-        :type alias: str
 
-        :rtype: list
         :returns: A list of blob hashes (strings) which were assigned to the alias.
         """
         dcd = self._get_dcd(alias)
-        dgsts = self.get_alias(alias)
+        dgsts = cast(List[str], self.get_alias(alias))
         self._request('delete', 'manifests/{}'.format(dcd))
         return dgsts
 
-    def list_aliases(self, batch_size=None, iterate=False):
+    def list_aliases(self, batch_size: Optional[int]=None, iterate: bool=False) -> Union[Iterable[str], List[str]]:
         """
         List all aliases defined in the repository.
 
         :param batch_size: Number of alias names to ask the server for at a time.
-        :type batch_size: int
 
         :param iterate: Whether to return iterator over the names or a list of all the names.
-        :type iterate: bool
 
-        :rtype: list or iterator of strings
         :returns: Alias names.
         """
         it = PaginatingResponse(self, '_request',
                                 'tags/list', 'tags',
                                 params={'n': batch_size})
         return it if iterate else list(it)
 
-    def api_version_check(self):
+    def api_version_check(self) -> Tuple[str, requests.Response]:
         """
         Performs API version check
 
-        :rtype: tuple
         :returns: verson check response as a string (JSON) and requests.Response
         """
         r = self._base_request('get', '')
         return r.content.decode('utf-8'), r
 
     @classmethod
-    def from_base(cls, base, repo):
+    def from_base(cls: Type[TD], base: 'DXFBase', repo: str) -> TD:
         """
         Create a :class:`DXF` object which uses the same host, settings and
         session as an existing :class:`DXFBase` object.
 
         :param base: Existing :class:`DXFBase` object.
-        :type base: :class:`DXFBase`
 
         :param repo: Name of the repository to access on the registry. Typically this is of the form ``username/reponame`` but for your own registries you don't actually have to stick to that.
-        :type repo: str
 
         :returns: :class:`DXF` object which shares configuration and session with ``base`` but which can also be used to operate on the ``repo`` repository.
-        :rtype: :class:`DXF`
         """
         # pylint: disable=protected-access
         r = cls(base._host, repo, base._auth, base._insecure, base._auth_host, base._tlsverify, base._timeout)
         r._token = base._token
         r._headers = base._headers
         r._sessions = [base._sessions[0]]
         return r
@@ -857,16 +793,14 @@
             'schemaVersion': 1,
             'name': self._repo,
             'tag': alias,
             'fsLayers': [{'blobSum': dgst} for dgst in digests],
             'history': [{'v1Compatibility': '{}'} for dgst in digests]
         }, sort_keys=True)
 
-_schema1_mimetype = 'application/vnd.docker.distribution.manifest.v1+json'
-
 def _urlsafe_b64encode(s):
     return base64.urlsafe_b64encode(_to_bytes_2and3(s)).rstrip(b'=').decode('utf-8')
 
 def _pad64(s):
     return s + b'=' * (-len(s) % 4)
 
 def _urlsafe_b64decode(s):
```

### Comparing `python-dxf-8.0.2/dxf/exceptions.py` & `python-dxf-9.0.1/dxf/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-dxf-8.0.2/dxf/main.py` & `python-dxf-9.0.1/dxf/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,28 +32,28 @@
 
 def _flatten(l):
     return [item for sublist in l for item in sublist]
 
 # pylint: disable=too-many-statements
 def doit(args, environ):
     dxf_progress = environ.get('DXF_PROGRESS')
+    progress = None
     if dxf_progress == '1' or (dxf_progress != '0' and sys.stderr.isatty()):
         bars = {}
-        def progress(dgst, chunk, size):
+        def do_progress(dgst, chunk, size):
             if dgst not in bars:
                 bars[dgst] = tqdm.tqdm(desc=dgst[0:8],
                                        total=size,
                                        leave=True)
             if chunk:
                 bars[dgst].update(len(chunk))
             if bars[dgst].n >= bars[dgst].total:
                 bars[dgst].close()
                 del bars[dgst]
-    else:
-        progress = None
+        progress = do_progress
 
     dxf_skiptlsverify = environ.get('DXF_SKIPTLSVERIFY')
     if dxf_skiptlsverify == '1':
         dxf_tlsverify = False
     else:
         dxf_tlsverify = environ.get('DXF_TLSVERIFY', True)
```

### Comparing `python-dxf-8.0.2/python_dxf.egg-info/PKG-INFO` & `python-dxf-9.0.1/python_dxf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: python-dxf
-Version: 8.0.2
+Version: 9.0.1
 Summary: Package for accessing a Docker v2 registry
 Home-page: https://github.com/davedoesdev/dxf
 Author: David Halls
 Author-email: dave@davedoesdev.com
 License: MIT
 Keywords: docker registry
 Platform: UNKNOWN
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 License-File: LICENCE
 
 |Build Status| |Coverage Status| |PyPI version|
 
 Python module and command-line tool for storing and retrieving data in a
 Docker registry.
```

### Comparing `python-dxf-8.0.2/setup.py` & `python-dxf-9.0.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,23 +4,24 @@
 
 def read(name):
     file_path = os.path.join(os.path.dirname(__file__), name)
     return io.open(file_path, encoding='utf8').read()
 
 setup(
     name='python-dxf',
-    version='8.0.2',
+    version='9.0.1',
     description="Package for accessing a Docker v2 registry",
     long_description=read('README.rst'),
     keywords='docker registry',
     author='David Halls',
     author_email='dave@davedoesdev.com',
     url='https://github.com/davedoesdev/dxf',
     license='MIT',
     packages=['dxf'],
+    package_data={"dxf": ["py.typed"]},
     entry_points={'console_scripts': ['dxf=dxf.main:main']},
     install_requires=['www-authenticate>=0.9.2',
                       'requests>=2.18.4',
                       'jwcrypto>=1.4.2',
                       'tqdm>=4.19.4'],
-    python_requires='>=3.6'
+    python_requires='>=3.7'
 )
```

### Comparing `python-dxf-8.0.2/test/test_cli.py` & `python-dxf-9.0.1/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `python-dxf-8.0.2/test/test_module.py` & `python-dxf-9.0.1/test/test_module.py`

 * *Files identical despite different names*

