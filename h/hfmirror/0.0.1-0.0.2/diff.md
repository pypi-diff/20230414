# Comparing `tmp/hfmirror-0.0.1.tar.gz` & `tmp/hfmirror-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hfmirror-0.0.1.tar", last modified: Thu Apr 13 13:36:53 2023, max compression
+gzip compressed data, was "hfmirror-0.0.2.tar", last modified: Fri Apr 14 14:54:03 2023, max compression
```

## Comparing `hfmirror-0.0.1.tar` & `hfmirror-0.0.2.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:36:53.000319 hfmirror-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-13 13:36:21.000000 hfmirror-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-13 13:36:21.000000 hfmirror-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7550 2023-04-13 13:36:53.000319 hfmirror-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-04-13 13:36:21.000000 hfmirror-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:36:52.996319 hfmirror-0.0.1/hfmirror/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-13 13:36:21.000000 hfmirror-0.0.1/hfmirror/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:36:52.996319 hfmirror-0.0.1/hfmirror/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 13:36:21.000000 hfmirror-0.0.1/hfmirror/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-13 13:36:21.000000 hfmirror-0.0.1/hfmirror/config/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:36:52.996319 hfmirror-0.0.1/hfmirror/resource/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-13 13:36:21.000000 hfmirror-0.0.1/hfmirror/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-04-13 13:36:21.000000 hfmirror-0.0.1/hfmirror/resource/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-04-13 13:36:21.000000 hfmirror-0.0.1/hfmirror/resource/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-04-13 13:36:21.000000 hfmirror-0.0.1/hfmirror/resource/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:36:52.996319 hfmirror-0.0.1/hfmirror/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-13 13:36:21.000000 hfmirror-0.0.1/hfmirror/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-13 13:36:21.000000 hfmirror-0.0.1/hfmirror/storage/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-04-13 13:36:21.000000 hfmirror-0.0.1/hfmirror/storage/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-13 13:36:21.000000 hfmirror-0.0.1/hfmirror/storage/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:36:52.996319 hfmirror-0.0.1/hfmirror/sync/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-13 13:36:21.000000 hfmirror-0.0.1/hfmirror/sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-04-13 13:36:21.000000 hfmirror-0.0.1/hfmirror/sync/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:36:52.996319 hfmirror-0.0.1/hfmirror/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-13 13:36:21.000000 hfmirror-0.0.1/hfmirror/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-13 13:36:21.000000 hfmirror-0.0.1/hfmirror/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-13 13:36:21.000000 hfmirror-0.0.1/hfmirror/utils/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-13 13:36:21.000000 hfmirror-0.0.1/hfmirror/utils/segments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-04-13 13:36:21.000000 hfmirror-0.0.1/hfmirror/utils/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-13 13:36:21.000000 hfmirror-0.0.1/hfmirror/utils/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 13:36:52.996319 hfmirror-0.0.1/hfmirror.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7550 2023-04-13 13:36:52.000000 hfmirror-0.0.1/hfmirror.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-13 13:36:52.000000 hfmirror-0.0.1/hfmirror.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 13:36:52.000000 hfmirror-0.0.1/hfmirror.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-13 13:36:52.000000 hfmirror-0.0.1/hfmirror.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-13 13:36:52.000000 hfmirror-0.0.1/hfmirror.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-13 13:36:21.000000 hfmirror-0.0.1/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-13 13:36:21.000000 hfmirror-0.0.1/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-13 13:36:21.000000 hfmirror-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 13:36:53.000319 hfmirror-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-04-13 13:36:21.000000 hfmirror-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:54:03.289446 hfmirror-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-14 14:53:30.000000 hfmirror-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-14 14:53:30.000000 hfmirror-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7550 2023-04-14 14:54:03.289446 hfmirror-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-04-14 14:53:30.000000 hfmirror-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:54:03.285446 hfmirror-0.0.2/hfmirror/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-14 14:53:30.000000 hfmirror-0.0.2/hfmirror/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:54:03.285446 hfmirror-0.0.2/hfmirror/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 14:53:30.000000 hfmirror-0.0.2/hfmirror/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-14 14:53:30.000000 hfmirror-0.0.2/hfmirror/config/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:54:03.285446 hfmirror-0.0.2/hfmirror/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-14 14:53:30.000000 hfmirror-0.0.2/hfmirror/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-14 14:53:30.000000 hfmirror-0.0.2/hfmirror/resource/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-04-14 14:53:30.000000 hfmirror-0.0.2/hfmirror/resource/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-04-14 14:53:30.000000 hfmirror-0.0.2/hfmirror/resource/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-04-14 14:53:30.000000 hfmirror-0.0.2/hfmirror/resource/sourceforge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-04-14 14:53:30.000000 hfmirror-0.0.2/hfmirror/resource/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:54:03.285446 hfmirror-0.0.2/hfmirror/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-14 14:53:30.000000 hfmirror-0.0.2/hfmirror/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-14 14:53:30.000000 hfmirror-0.0.2/hfmirror/storage/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7747 2023-04-14 14:53:30.000000 hfmirror-0.0.2/hfmirror/storage/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-04-14 14:53:30.000000 hfmirror-0.0.2/hfmirror/storage/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:54:03.285446 hfmirror-0.0.2/hfmirror/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-14 14:53:30.000000 hfmirror-0.0.2/hfmirror/sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-04-14 14:53:30.000000 hfmirror-0.0.2/hfmirror/sync/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:54:03.289446 hfmirror-0.0.2/hfmirror/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-14 14:53:30.000000 hfmirror-0.0.2/hfmirror/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-14 14:53:30.000000 hfmirror-0.0.2/hfmirror/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-14 14:53:30.000000 hfmirror-0.0.2/hfmirror/utils/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-14 14:53:30.000000 hfmirror-0.0.2/hfmirror/utils/segments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-04-14 14:53:30.000000 hfmirror-0.0.2/hfmirror/utils/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-14 14:53:30.000000 hfmirror-0.0.2/hfmirror/utils/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 14:54:03.285446 hfmirror-0.0.2/hfmirror.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7550 2023-04-14 14:54:03.000000 hfmirror-0.0.2/hfmirror.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-14 14:54:03.000000 hfmirror-0.0.2/hfmirror.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 14:54:03.000000 hfmirror-0.0.2/hfmirror.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-14 14:54:03.000000 hfmirror-0.0.2/hfmirror.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-14 14:54:03.000000 hfmirror-0.0.2/hfmirror.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-14 14:53:30.000000 hfmirror-0.0.2/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-14 14:53:30.000000 hfmirror-0.0.2/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-14 14:53:30.000000 hfmirror-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 14:54:03.289446 hfmirror-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-04-14 14:53:30.000000 hfmirror-0.0.2/setup.py
```

### Comparing `hfmirror-0.0.1/LICENSE` & `hfmirror-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.1/PKG-INFO` & `hfmirror-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hfmirror
-Version: 0.0.1
+Version: 0.0.2
 Summary: Mirror for resources to local and huggingface.
 Home-page: https://github.com/narugo1992/hfmirror
 Author: narugo1992
 Author-email: narugo@126.com
 License: Apache License, Version 2.0
 Keywords: A simple tool for automatic parameter tuning.
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `hfmirror-0.0.1/README.md` & `hfmirror-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.1/hfmirror/resource/github.py` & `hfmirror-0.0.2/hfmirror/resource/github.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,98 +1,61 @@
-import re
 import warnings
 from typing import Tuple, Mapping, Any, Union, Iterable, Optional
 
 from github import Github
 from github.GitRelease import GitRelease
 from tqdm.auto import tqdm
 
-from .resource import SyncResource, TargetPathType
+from .resource import TargetPathType
+from .version import VersionBasedResource
 
 
 def _to_int(v: Union[str, int]) -> Union[str, int]:
     try:
         return int(v)
     except (TypeError, ValueError):
         return v
 
 
-class GithubReleaseResource(SyncResource):
+class GithubReleaseResource(VersionBasedResource):
     def __init__(self, repo: str, *,
                  github_client: Optional[Github] = None,
                  access_token: Optional[str] = None,
                  add_version_attachment: bool = True):
+        VersionBasedResource.__init__(self, add_version_attachment)
         self.repo = repo
         if github_client and access_token:
             warnings.warn('Github client provided, so access token will be ignored.', stacklevel=2)
         self.github_client = github_client or Github(access_token)
-        self.add_version_attachment = add_version_attachment
 
     def _tag_filter(self, tag):
         return tag
 
     def _filename_filter(self, tag, filename):
         _ = tag
         return filename
 
-    __version_pattern__ = r'^([a-zA-Z]+(\.|-)?)?(?P<version>[\d.]+)$'
-    __version_file_prefix__ = 'LATEST_RELEASE'
-
-    def _version_to_tuple(self, version):
-        matching = re.fullmatch(self.__version_pattern__, version)
-        if matching:
-            version_text = matching.group('version')
-            return tuple(map(_to_int, version_text.split('.')))
-        else:
-            raise ValueError(f'Invalid version for release - {version!r}.')
-
-    def grab(self) -> Iterable[Union[
+    def grab_for_items(self) -> Iterable[Union[
         Tuple[str, Any, TargetPathType, Mapping],
         Tuple[str, Any, TargetPathType],
     ]]:
         repo = self.github_client.get_repo(self.repo)
-        versions = []
+        yield 'metadata', {'source': repo.html_url}, ''
         repo_tqdm = tqdm(repo.get_releases())
         for release in repo_tqdm:
             release: GitRelease
             tag_name = self._tag_filter(release.tag_name)
             repo_tqdm.set_description(tag_name)
             if not tag_name:
                 continue
 
-            versions.append(tag_name)
+            yield 'version', tag_name, tag_name
             release_metadata = {'version': release.tag_name, 'title': release.title, 'url': release.html_url}
             yield 'metadata', release_metadata, tag_name
             for asset in release.get_assets():
                 filename = self._filename_filter(tag_name, asset.name)
                 if not filename:
                     continue
 
                 download_url = asset.browser_download_url
                 metadata = {'tag': release.tag_name, 'filename': asset.name}
                 yield 'remote', download_url, f'{tag_name}/{filename}', metadata
-
-        if self.add_version_attachment:
-            version_map = {}
-            for version in versions:
-                try:
-                    _tuple = self._version_to_tuple(version)
-                except ValueError:
-                    warnings.warn(f'Version {version!r} does not match the regular expression, '
-                                  f'so it will be ignored in version indexing.')
-                    continue
-
-                for i in range(len(_tuple) + 1):
-                    _part_tuple = _tuple[:i]
-                    if _part_tuple in version_map:
-                        _exist_tuple, _exist_version = version_map[_part_tuple]
-                        if _tuple > _exist_tuple:
-                            version_map[_part_tuple] = (_tuple, version)
-                    else:
-                        version_map[_part_tuple] = (_tuple, version)
-
-            for tuple_, (_, version) in version_map.items():
-                if tuple_:
-                    schema_file = f'{self.__version_file_prefix__}_{".".join(map(str, tuple_))}'
-                else:
-                    schema_file = self.__version_file_prefix__
-                yield 'text', version, schema_file
```

### Comparing `hfmirror-0.0.1/hfmirror/resource/item.py` & `hfmirror-0.0.2/hfmirror/resource/item.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,23 +42,24 @@
                    (other._value, other.metadata, other.segments)
         else:
             return False
 
 
 class RemoteSyncItem(SyncItem):
     __type__ = 'remote'
+    __headers__ = {}
 
     def __init__(self, url, metadata, segments: List[str]):
         SyncItem.__init__(self, url, metadata, segments)
         self.url = url
         self._session = None
 
     def _get_session(self) -> requests.Session:
         if self._session is None:
-            self._session = get_requests_session()
+            self._session = get_requests_session(headers=self.__headers__)
 
         return self._session
 
     def _file_process(self, filename):
         pass
 
     @contextmanager
```

### Comparing `hfmirror-0.0.1/hfmirror/resource/resource.py` & `hfmirror-0.0.2/hfmirror/resource/resource.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import io
 import warnings
 from operator import itemgetter
-from typing import Tuple, List, Mapping, Any, Iterable, Union, Dict
+from typing import Tuple, List, Mapping, Any, Iterable, Union, Dict, Callable
 
 from hbutils.string.tree import format_tree
 
-from .item import create_sync_item, SyncItem, _PRESERVED_NAMES
+from .item import create_sync_item, SyncItem, _PRESERVED_NAMES, _REGISTERED_SYNC_TYPES
 from ..utils import hash_anything, to_segments, TargetPathType, text_concat, text_parallel
 
 
 class MetadataItem:
     def __init__(self, data: Mapping, segments: List[str]):
         self.data = data
         self.segments = segments
@@ -126,20 +126,31 @@
             return False
 
 
 SyncItemType = Union[SyncItem, MetadataItem]
 
 
 class SyncResource:
+    def __init__(self):
+        self._registered_ops: Dict[str, Callable] = {}
+
     def grab(self) -> Iterable[Union[
         Tuple[str, Any, TargetPathType, Mapping],
         Tuple[str, Any, TargetPathType],
     ]]:
         raise NotImplementedError  # pragma: no cover
 
+    def register_operation(self, name: str, func: Callable):
+        if name in _PRESERVED_NAMES or name in _REGISTERED_SYNC_TYPES:
+            raise KeyError(f'Operation name {name!r} has already been preserved or registered as a sync item.')
+        elif name not in self._registered_ops:
+            self._registered_ops[name] = func
+        else:
+            raise KeyError(f'Operation {name} has already been registered.')
+
     def iter_sync_items(self) -> Iterable[SyncItemType]:
         for tpl in self.grab():
             if isinstance(tpl, tuple):
                 if len(tpl) == 3:
                     (type_, value, path), attached_data = tpl, {}
                 elif len(tpl) == 4:
                     type_, value, path, attached_data = tpl
@@ -154,14 +165,16 @@
                             warnings.warn(f'Attached data {attached_data!r} for position {tpl!r} '
                                           f'will be ignored when defining metadata.')
                         yield MetadataItem(value, segments)
 
                     else:
                         assert False, f'Undefined preserved operation - {type_!r}, ' \
                                       f'please notice the author about this.'  # pragma: no cover
+                elif type_ in self._registered_ops:
+                    self._registered_ops[type_](value, segments, attached_data)
                 else:
                     yield create_sync_item(type_, value, attached_data, segments)
 
             else:
                 raise TypeError(f'Invalid sync type data - {tpl!r}.')
 
     def sync_tree(self) -> SyncTree:
```

### Comparing `hfmirror-0.0.1/hfmirror/storage/base.py` & `hfmirror-0.0.2/hfmirror/storage/base.py`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.1/hfmirror/storage/huggingface.py` & `hfmirror-0.0.2/hfmirror/storage/huggingface.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,15 +29,15 @@
             sha.update(data)
 
     return sha.hexdigest() == oid
 
 
 def hf_local_upload_check(uploads: List[Tuple[Optional[str], str]],
                           repo_id: str, repo_type='dataset', revision='main',
-                          chunk_for_hash: int = 1 << 20, session=None) -> List[bool]:
+                          chunk_for_hash: int = 1 << 20, session=None) -> List[Tuple[bool, str]]:
     """
     Overview:
         Check resource on huggingface repo and local.
 
     :param uploads: Tuples of uploads, the first item is the local file, second item is the file in repo. When \
         first item is None, it means delete this item in repo.
     :param repo_id: Repository id, the same as that in huggingface library.
@@ -58,28 +58,31 @@
 
     checks = []
     for f_in_local, f_in_repo in uploads:
         fs_in_repo = tuple(to_segments(f_in_repo))
         f_meta = online_file_info.get(fs_in_repo, None)
         if not f_meta:
             if f_in_local is not None:  # not exist in repo, need to upload
-                checks.append(True)
+                checks.append((True, 'file'))
             else:  # not exist in repo, do not need to delete
-                checks.append(False)
+                checks.append((False, None))
         else:
             if f_in_local is not None:  # going to upload
                 if 'lfs' in f_meta:  # is a lfs file
                     is_lfs, oid, filesize = True, f_meta['lfs']['oid'], f_meta['lfs']['size']
                 else:  # not lfs
                     is_lfs, oid, filesize = False, f_meta['oid'], f_meta['size']
 
+                if f_meta['type'] != 'file':
+                    raise FileExistsError(f'Path {f_meta["path"]!r} is a {f_meta["type"]} on huggingface, '
+                                          f'unable to replace it with local file {f_in_local!r}.')
                 _is_duplicated = _single_resource_is_duplicated(f_in_local, is_lfs, oid, filesize, chunk_for_hash)
-                checks.append(not _is_duplicated)  # exist, need to upload if not the same
+                checks.append((not _is_duplicated, f_meta['type']))  # exist, need to upload if not the same
             else:  # going to delete
-                checks.append(True)
+                checks.append((True, f_meta['type']))
 
     return checks
 
 
 def _check_repo_type(repo_type):
     if repo_type in {'model', 'dataset', 'space'}:
         return repo_type
@@ -136,18 +139,23 @@
             (local_filename, self.path_join(*file_in_repo))
             for file_in_repo, local_filename in _map_changes.items()
         ]
         uploads_is_needed = hf_local_upload_check(uploads, self.repo, self.repo_type, self.revision,
                                                   session=self.session)
 
         operations, op_items, additions, deletions = [], [], 0, 0
-        for (local_filename, fip), need in zip(uploads, uploads_is_needed):
+        for (local_filename, fip), (need, objtype) in zip(uploads, uploads_is_needed):
             if need:
                 if local_filename is None:
-                    operations.append(CommitOperationDelete(path_in_repo=fip))
+                    if objtype == 'directory':  # a / should be at the end of path when deleting a folder
+                        fip = f'{fip}/'
+                        is_folder = True
+                    else:
+                        is_folder = False
+                    operations.append(CommitOperationDelete(path_in_repo=fip, is_folder=is_folder))
                     op_items.append(f'-{fip}')
                     deletions += 1
                 else:
                     operations.append(CommitOperationAdd(path_in_repo=fip, path_or_fileobj=local_filename))
                     op_items.append(f'+{fip}')
                     additions += 1
```

### Comparing `hfmirror-0.0.1/hfmirror/storage/local.py` & `hfmirror-0.0.2/hfmirror/storage/local.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os.path
 import pathlib
-import shutil
 from contextlib import contextmanager
 from typing import List, Optional, Tuple, Union
 
+from hbutils.system import copy, remove
 from hbutils.system.filesystem.tempfile import TemporaryDirectory
 
 from .base import BaseStorage
 from ..utils import to_segments
 
 
 class LocalStorage(BaseStorage):
@@ -32,42 +32,42 @@
             # record all the files
             records = []
             for i, file_in_storage in enumerate(state):
                 file_in_storage = self.path_join(*file_in_storage)
                 if os.path.exists(file_in_storage):
                     file_in_temp = os.path.join(td, f'{i}', os.path.basename(file_in_storage))
                     os.makedirs(os.path.join(td, f'{i}'), exist_ok=True)
-                    shutil.copyfile(file_in_storage, file_in_temp)
+                    copy(file_in_storage, file_in_temp)
                     records.append(file_in_temp)
                 else:
                     records.append(None)
 
             try:
                 yield
             except:
                 # recover all the files
                 for file_in_temp, file_in_storage in zip(records, state):
                     file_in_storage = self.path_join(*file_in_storage)
                     if file_in_temp is None:
                         if os.path.exists(file_in_storage):
-                            os.remove(file_in_storage)
+                            remove(file_in_storage)
                     else:
                         directory = os.path.dirname(file_in_storage)
                         if directory:
                             os.makedirs(directory, exist_ok=True)
-                        shutil.copyfile(file_in_temp, file_in_storage)
+                        copy(file_in_temp, file_in_storage)
 
                 raise
 
     def batch_change_files(self, changes: List[Tuple[Optional[str], List[str]]]):
         states = [file_in_storage for _, file_in_storage in changes]
         with self.recover_state_when_failed(states):
             for local_file, file_in_storage in changes:
                 file_in_storage = self.path_join(*file_in_storage)
                 if local_file is None:
                     if os.path.exists(file_in_storage):
-                        os.remove(file_in_storage)
+                        remove(file_in_storage)
                 else:
                     directory = os.path.dirname(file_in_storage)
                     if directory:
                         os.makedirs(directory, exist_ok=True)
-                    shutil.copyfile(local_file, file_in_storage)
+                    copy(local_file, file_in_storage)
```

### Comparing `hfmirror-0.0.1/hfmirror/sync/sync.py` & `hfmirror-0.0.2/hfmirror/sync/sync.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import os.path
+from itertools import chain
 from typing import List, Tuple
 
 from hbutils.reflection import nested_with
 from hbutils.string import plural_word
 from hbutils.system.filesystem.tempfile import TemporaryDirectory
 from tqdm import tqdm as _TqdmType
 from tqdm.auto import tqdm
@@ -42,16 +43,18 @@
             else:
                 items.append((key, value))
 
         meta_file_segments = [*segments, self.meta_filename]
         if self.storage.file_exists(meta_file_segments):
             old_metadata = json.loads(self.storage.read_text(meta_file_segments))
             old_files = {item['name']: item for item in old_metadata['files']}
+            old_item_names = {item['name'] for item in chain(old_metadata['files'], old_metadata['folders'])}
         else:
             old_files = {}
+            old_item_names = set()
 
         m_folders = []
         for key, folder in folders:
             self._sync_tree(folder, [*segments, key], tqdms)
             m_folders.append({'name': key, 'metadata': folder.metadata})
 
         m_files = []
@@ -88,18 +91,21 @@
                 json.dump({
                     'path': '/'.join(segments),
                     'metadata': tree.metadata,
                     'files': m_files,
                     'folders': m_folders,
                 }, f, indent=4, ensure_ascii=False)
 
+            new_item_names = {item['name'] for item in chain(m_files, m_folders)}
             with nested_with(*[item.load_file() for _, item in need_load_files]) as file_paths:
-                changes = [(local_metafile, [*segments, self.meta_filename])]
-                for local_file, (key, _) in zip(file_paths, need_load_files):
+                changes = [(local_metafile, [*segments, self.meta_filename])]  # .meta.json
+                for local_file, (key, _) in zip(file_paths, need_load_files):  # items to add
                     changes.append((local_file, [*segments, key]))
+                for key in sorted(old_item_names - new_item_names):  # items to delete
+                    changes.append((None, [*segments, key]))
 
                 self.storage.batch_change_files(changes)
 
             file_tqdm.update(len(need_load_files))
             file_tqdm.set_description(plural_word(file_tqdm.n, 'file'))
 
         tree_tqdm.update()
```

### Comparing `hfmirror-0.0.1/hfmirror/utils/download.py` & `hfmirror-0.0.2/hfmirror/utils/download.py`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.1/hfmirror/utils/hash.py` & `hfmirror-0.0.2/hfmirror/utils/hash.py`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.1/hfmirror/utils/segments.py` & `hfmirror-0.0.2/hfmirror/utils/segments.py`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.1/hfmirror/utils/session.py` & `hfmirror-0.0.2/hfmirror/utils/session.py`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.1/hfmirror/utils/text.py` & `hfmirror-0.0.2/hfmirror/utils/text.py`

 * *Files identical despite different names*

### Comparing `hfmirror-0.0.1/hfmirror.egg-info/PKG-INFO` & `hfmirror-0.0.2/hfmirror.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hfmirror
-Version: 0.0.1
+Version: 0.0.2
 Summary: Mirror for resources to local and huggingface.
 Home-page: https://github.com/narugo1992/hfmirror
 Author: narugo1992
 Author-email: narugo@126.com
 License: Apache License, Version 2.0
 Keywords: A simple tool for automatic parameter tuning.
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `hfmirror-0.0.1/hfmirror.egg-info/SOURCES.txt` & `hfmirror-0.0.2/hfmirror.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 hfmirror.egg-info/top_level.txt
 hfmirror/config/__init__.py
 hfmirror/config/meta.py
 hfmirror/resource/__init__.py
 hfmirror/resource/github.py
 hfmirror/resource/item.py
 hfmirror/resource/resource.py
+hfmirror/resource/sourceforge.py
+hfmirror/resource/version.py
 hfmirror/storage/__init__.py
 hfmirror/storage/base.py
 hfmirror/storage/huggingface.py
 hfmirror/storage/local.py
 hfmirror/sync/__init__.py
 hfmirror/sync/sync.py
 hfmirror/utils/__init__.py
```

### Comparing `hfmirror-0.0.1/hfmirror.egg-info/requires.txt` & `hfmirror-0.0.2/hfmirror.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 hbutils>=0.8.6
 tqdm>=4.0.0
 click>=7.0.0
 requests
+pyquery
 pygithub
 huggingface_hub
 
 [doc]
 Jinja2~=3.0.0
 sphinx~=3.2.0
 sphinx_rtd_theme~=0.4.3
```

### Comparing `hfmirror-0.0.1/setup.py` & `hfmirror-0.0.2/setup.py`

 * *Files identical despite different names*

