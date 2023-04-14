# Comparing `tmp/cushy-storage-1.0.0.tar.gz` & `tmp/cushy-storage-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\cushy-storage-1.0.0.tar", last modified: Mon Mar 13 14:40:30 2023, max compression
+gzip compressed data, was "dist\cushy-storage-1.0.1.tar", last modified: Fri Apr 14 11:53:32 2023, max compression
```

## Comparing `cushy-storage-1.0.0.tar` & `cushy-storage-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-03-13 14:40:30.000000 cushy-storage-1.0.0/
--rw-rw-rw-   0        0        0    11558 2023-03-08 11:01:44.000000 cushy-storage-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     4379 2023-03-13 14:40:30.000000 cushy-storage-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3501 2023-03-13 14:33:31.000000 cushy-storage-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-03-13 14:40:29.000000 cushy-storage-1.0.0/cushy_storage/
--rw-rw-rw-   0        0        0      827 2023-03-13 14:13:17.000000 cushy-storage-1.0.0/cushy_storage/__init__.py
--rw-rw-rw-   0        0        0     5910 2023-03-13 14:25:52.000000 cushy-storage-1.0.0/cushy_storage/_core.py
-drwxrwxrwx   0        0        0        0 2023-03-13 14:40:29.000000 cushy-storage-1.0.0/cushy_storage.egg-info/
--rw-rw-rw-   0        0        0     4379 2023-03-13 14:40:29.000000 cushy-storage-1.0.0/cushy_storage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2023-03-13 14:40:29.000000 cushy-storage-1.0.0/cushy_storage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-13 14:40:29.000000 cushy-storage-1.0.0/cushy_storage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-03-13 14:40:29.000000 cushy-storage-1.0.0/cushy_storage.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-13 14:40:30.000000 cushy-storage-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1814 2023-03-13 14:02:58.000000 cushy-storage-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-13 14:40:30.000000 cushy-storage-1.0.0/tests/
--rw-rw-rw-   0        0        0     1972 2023-03-13 14:39:34.000000 cushy-storage-1.0.0/tests/test_cushy_dict.py
--rw-rw-rw-   0        0        0     2365 2023-03-13 14:39:24.000000 cushy-storage-1.0.0/tests/test_dict_cache.py
+drwxrwxrwx   0        0        0        0 2023-04-14 11:53:32.000000 cushy-storage-1.0.1/
+-rw-rw-rw-   0        0        0    11558 2023-03-08 11:01:44.000000 cushy-storage-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     5234 2023-04-14 11:53:32.000000 cushy-storage-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4356 2023-04-14 11:53:05.000000 cushy-storage-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 11:53:32.000000 cushy-storage-1.0.1/cushy_storage/
+-rw-rw-rw-   0        0        0      827 2023-03-13 14:13:17.000000 cushy-storage-1.0.1/cushy_storage/__init__.py
+-rw-rw-rw-   0        0        0     6133 2023-04-14 11:51:52.000000 cushy-storage-1.0.1/cushy_storage/_core.py
+drwxrwxrwx   0        0        0        0 2023-04-14 11:53:32.000000 cushy-storage-1.0.1/cushy_storage.egg-info/
+-rw-rw-rw-   0        0        0     5234 2023-04-14 11:53:32.000000 cushy-storage-1.0.1/cushy_storage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      297 2023-04-14 11:53:32.000000 cushy-storage-1.0.1/cushy_storage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 11:53:32.000000 cushy-storage-1.0.1/cushy_storage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-14 11:53:32.000000 cushy-storage-1.0.1/cushy_storage.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-14 11:53:32.000000 cushy-storage-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1814 2023-04-14 11:53:31.000000 cushy-storage-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 11:53:32.000000 cushy-storage-1.0.1/tests/
+-rw-rw-rw-   0        0        0     1971 2023-03-18 07:38:01.000000 cushy-storage-1.0.1/tests/test_base_dict.py
+-rw-rw-rw-   0        0        0     1804 2023-03-18 08:01:59.000000 cushy-storage-1.0.1/tests/test_cushy_dict.py
+-rw-rw-rw-   0        0        0     2365 2023-03-13 14:39:24.000000 cushy-storage-1.0.1/tests/test_dict_cache.py
```

### Comparing `cushy-storage-1.0.0/LICENSE` & `cushy-storage-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cushy-storage-1.0.0/PKG-INFO` & `cushy-storage-1.0.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cushy-storage
-Version: 1.0.0
+Version: 1.0.1
 Summary: A data local persistence framework library
 Home-page: https://github.com/Undertone0809/cushy-storage
 Author: Zeeland
 Author-email: zeeland@foxmail.com
 License: Apache 2.0
 Keywords: storage,serialization,json,cushy-storage,cushy_storage
 Classifier: Development Status :: 3 - Alpha
@@ -20,15 +20,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">
     cushy-storage
 </h1>
 <p align="center">
-  <strong>cushy-storage是一个基于磁盘缓存的Python框架</strong>
+  <strong>一个基于磁盘缓存的Python框架</strong>
 </p>
 
 <p align="center">
     <a target="_blank" href="">
         <img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg?label=license" />
     </a>
     <a target="_blank" href=''>
@@ -40,67 +40,95 @@
 </p>
 
 [English](/README_en.md) [中文](/README.md)
 
 # 简介
 cushy-storage是一个基于磁盘缓存的Python库，可以将Python对象序列化后缓存到磁盘中，以便下次使用时直接读取，从而提高程序的执行效率。
 
+# 特性
+- 可以方便的将数据进行本地磁盘存储
+- 免去了直接操作文件的工作
+- 像操作dict一样读写，十分方便
+- 提供序列化操作
+- 提供多种数据压缩方式
+
 
 # 安装
 
 ```bash
 pip install cushy-storage --upgrade 
 ```
 
-# 使用方法
+# 快速上手
+
+`cushy-storage` 的使用主要分为三个类，`BaseDict` `CushyDict` `disk_cache`，其中`CushyDict`是`BaseDict`的增强版，可以实现
+`BaseDict`的所有功能，还增加了相应序列化操作，因此推荐直接使用`CushyDict`来操作保存数据。
 
 ## BaseDict类
 
 BaseDict类是CushyDict类的基础实现，提供了基本的字典结构和缓存操作。它可以用于缓存任何类型的Python对象，但不支持序列化和反序列化操作。
 
 ```python
 from cushy_storage import BaseDict
 
-cache = BaseDict('./cache')
+# 初始化cache，保存在./data文件夹下
+cache = BaseDict('./data')
 cache['key'] = b'value'
 value = cache['key']
+print(value)
 
 ```
 
 ## CushyDict类
 
-CushyDict类是CushyStorage库的高级实现，增加了对值进行序列化和反序列化的功能。它支持多种序列化算法（包括pickle和json）和压缩算法（包括zlib和lzma），可以根据需要选择不同的算法进行数据压缩和序列化。
+CushyDict类是BaseDict库的高级实现，增加了对值进行序列化和反序列化的功能。它支持多种序列化算法（包括pickle和json）和压缩算法（包括zlib和lzma），可以根据需要选择不同的算法进行数据压缩和序列化。
 
 ```python
 from cushy_storage import CushyDict
 
-cache = CushyDict('./cache')
+# 初始化cache，保存在./data文件夹下
+cache = CushyDict('./data')
 cache['key'] = {'value': 42}
 value = cache['key']
+print(value)
+
+```
+
+- 判断key是否存在
+
+```python
+from cushy_storage import CushyDict
+
+cache = CushyDict('./data')
+if 'key' in cache:
+    print("key exist")
+else:
+    print("key not exist")
 
 ```
 
 ## disk_cache装饰器函数
 
 disk_cache装饰器函数可以将函数的输出结果缓存到磁盘中，以便下次使用时直接读取。通过该装饰器，可以在不改变原有代码逻辑的情况下，大幅度提高程序的执行效率。
 
 ```python
 from cushy_storage import disk_cache
 
-@disk_cache('./cache')
+@disk_cache('./data')
 def my_func():
     return {'value': 42}
 
 result = my_func()
 
 ```
  
  
 # 待办
 
+- [ ] 提供单例模式解决方案，提供更加方便的磁盘缓存方案
 - [ ] 支持更多的压缩和序列化算法，以满足不同类型数据的需求
 - [ ] 提供更加友好的错误处理机制，让用户更容易发现和解决问题
 - [ ] 改进缓存管理策略，确保缓存数据的可靠性和一致性
 - [ ] 提供更加丰富的测试用例，并定期进行性能测试和升级
 - [ ] 支持分布式缓存，可以在多台机器上共享缓存数据
 - [ ] 增加缓存过期功能，可以自动删除长时间未使用的缓存数据
 - [ ] 改善文档结构和代码注释，方便用户理解和使用库
```

### Comparing `cushy-storage-1.0.0/README.md` & `cushy-storage-1.0.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 <h1 align="center">
     cushy-storage
 </h1>
 <p align="center">
-  <strong>cushy-storage是一个基于磁盘缓存的Python框架</strong>
+  <strong>一个基于磁盘缓存的Python框架</strong>
 </p>
 
 <p align="center">
     <a target="_blank" href="">
         <img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg?label=license" />
     </a>
     <a target="_blank" href=''>
@@ -18,67 +18,95 @@
 </p>
 
 [English](/README_en.md) [中文](/README.md)
 
 # 简介
 cushy-storage是一个基于磁盘缓存的Python库，可以将Python对象序列化后缓存到磁盘中，以便下次使用时直接读取，从而提高程序的执行效率。
 
+# 特性
+- 可以方便的将数据进行本地磁盘存储
+- 免去了直接操作文件的工作
+- 像操作dict一样读写，十分方便
+- 提供序列化操作
+- 提供多种数据压缩方式
+
 
 # 安装
 
 ```bash
 pip install cushy-storage --upgrade 
 ```
 
-# 使用方法
+# 快速上手
+
+`cushy-storage` 的使用主要分为三个类，`BaseDict` `CushyDict` `disk_cache`，其中`CushyDict`是`BaseDict`的增强版，可以实现
+`BaseDict`的所有功能，还增加了相应序列化操作，因此推荐直接使用`CushyDict`来操作保存数据。
 
 ## BaseDict类
 
 BaseDict类是CushyDict类的基础实现，提供了基本的字典结构和缓存操作。它可以用于缓存任何类型的Python对象，但不支持序列化和反序列化操作。
 
 ```python
 from cushy_storage import BaseDict
 
-cache = BaseDict('./cache')
+# 初始化cache，保存在./data文件夹下
+cache = BaseDict('./data')
 cache['key'] = b'value'
 value = cache['key']
+print(value)
 
 ```
 
 ## CushyDict类
 
-CushyDict类是CushyStorage库的高级实现，增加了对值进行序列化和反序列化的功能。它支持多种序列化算法（包括pickle和json）和压缩算法（包括zlib和lzma），可以根据需要选择不同的算法进行数据压缩和序列化。
+CushyDict类是BaseDict库的高级实现，增加了对值进行序列化和反序列化的功能。它支持多种序列化算法（包括pickle和json）和压缩算法（包括zlib和lzma），可以根据需要选择不同的算法进行数据压缩和序列化。
 
 ```python
 from cushy_storage import CushyDict
 
-cache = CushyDict('./cache')
+# 初始化cache，保存在./data文件夹下
+cache = CushyDict('./data')
 cache['key'] = {'value': 42}
 value = cache['key']
+print(value)
+
+```
+
+- 判断key是否存在
+
+```python
+from cushy_storage import CushyDict
+
+cache = CushyDict('./data')
+if 'key' in cache:
+    print("key exist")
+else:
+    print("key not exist")
 
 ```
 
 ## disk_cache装饰器函数
 
 disk_cache装饰器函数可以将函数的输出结果缓存到磁盘中，以便下次使用时直接读取。通过该装饰器，可以在不改变原有代码逻辑的情况下，大幅度提高程序的执行效率。
 
 ```python
 from cushy_storage import disk_cache
 
-@disk_cache('./cache')
+@disk_cache('./data')
 def my_func():
     return {'value': 42}
 
 result = my_func()
 
 ```
  
  
 # 待办
 
+- [ ] 提供单例模式解决方案，提供更加方便的磁盘缓存方案
 - [ ] 支持更多的压缩和序列化算法，以满足不同类型数据的需求
 - [ ] 提供更加友好的错误处理机制，让用户更容易发现和解决问题
 - [ ] 改进缓存管理策略，确保缓存数据的可靠性和一致性
 - [ ] 提供更加丰富的测试用例，并定期进行性能测试和升级
 - [ ] 支持分布式缓存，可以在多台机器上共享缓存数据
 - [ ] 增加缓存过期功能，可以自动删除长时间未使用的缓存数据
 - [ ] 改善文档结构和代码注释，方便用户理解和使用库
```

### Comparing `cushy-storage-1.0.0/cushy_storage/__init__.py` & `cushy-storage-1.0.1/cushy_storage/__init__.py`

 * *Files identical despite different names*

### Comparing `cushy-storage-1.0.0/cushy_storage/_core.py` & `cushy-storage-1.0.1/cushy_storage/_core.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,15 +55,17 @@
 
 # Locks for each hash value (hexadecimal representation of 0-255)
 _LOCKS = {hex(i)[2:].zfill(2): threading.Lock() for i in range(256)}
 _F = Union[str, Tuple[Callable, Callable], None]
 
 
 def _cf(s: _F, d: dict) -> Tuple[Callable, Callable]:
-    # Helper function to get the compression or serialization functions based on input parameter
+    """
+    Helper function to get the compression or serialization functions based on input parameter
+    """
     if s is None:
         return lambda x: x, lambda x: x
     elif isinstance(s, str):
         return d[s]
     else:
         return s
 
@@ -113,17 +115,26 @@
     def __iter__(self):
         # Iterate over all keys in the cache
         for a in os.listdir(self.path):
             for b in os.listdir(self.path / a):
                 yield a + b[:-1]
 
 
-# A subclass of BaseDict that can serialize and deserialize values using different algorithms
 class CushyDict(BaseDict):
+    """
+    A subclass of BaseDict that can serialize and deserialize values using different algorithms
+    """
+
     def __init__(self, path: str, compress: _F = None, serialize: _F = 'json'):
+        """
+
+        :param path: the path to save
+        :param compress: zlib or lzma
+        :param serialize: json or pickle
+        """
         super().__init__(path, compress)
         self.serialize, self.deserialize = _cf(serialize, _SERIALIZATION)
 
     def __getitem__(self, k: str):
         return self.deserialize(super().__getitem__(k))
 
     def __setitem__(self, k: str, v: Any):
@@ -132,16 +143,18 @@
 
 _EXT = {
     'pickle': 'pkl',
     'json': 'json',
 }
 
 
-def disk_cache(path=None, compress=None, serialize='json'):
-    # Decorator that caches the output of a function to disk
+def disk_cache(path: str = None, compress: str = None, serialize: str = 'json'):
+    """
+    Decorator that caches the output of a function to disk
+    """
     ext = _EXT.get(serialize, '_')
     dump = _cf(serialize, _SERIALIZATION)[0]
 
     def decorator(func):
         nonlocal path
         name = func.__name__
         if path is None:
```

### Comparing `cushy-storage-1.0.0/cushy_storage.egg-info/PKG-INFO` & `cushy-storage-1.0.1/cushy_storage.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cushy-storage
-Version: 1.0.0
+Version: 1.0.1
 Summary: A data local persistence framework library
 Home-page: https://github.com/Undertone0809/cushy-storage
 Author: Zeeland
 Author-email: zeeland@foxmail.com
 License: Apache 2.0
 Keywords: storage,serialization,json,cushy-storage,cushy_storage
 Classifier: Development Status :: 3 - Alpha
@@ -20,15 +20,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">
     cushy-storage
 </h1>
 <p align="center">
-  <strong>cushy-storage是一个基于磁盘缓存的Python框架</strong>
+  <strong>一个基于磁盘缓存的Python框架</strong>
 </p>
 
 <p align="center">
     <a target="_blank" href="">
         <img src="https://img.shields.io/badge/License-Apache%202.0-blue.svg?label=license" />
     </a>
     <a target="_blank" href=''>
@@ -40,67 +40,95 @@
 </p>
 
 [English](/README_en.md) [中文](/README.md)
 
 # 简介
 cushy-storage是一个基于磁盘缓存的Python库，可以将Python对象序列化后缓存到磁盘中，以便下次使用时直接读取，从而提高程序的执行效率。
 
+# 特性
+- 可以方便的将数据进行本地磁盘存储
+- 免去了直接操作文件的工作
+- 像操作dict一样读写，十分方便
+- 提供序列化操作
+- 提供多种数据压缩方式
+
 
 # 安装
 
 ```bash
 pip install cushy-storage --upgrade 
 ```
 
-# 使用方法
+# 快速上手
+
+`cushy-storage` 的使用主要分为三个类，`BaseDict` `CushyDict` `disk_cache`，其中`CushyDict`是`BaseDict`的增强版，可以实现
+`BaseDict`的所有功能，还增加了相应序列化操作，因此推荐直接使用`CushyDict`来操作保存数据。
 
 ## BaseDict类
 
 BaseDict类是CushyDict类的基础实现，提供了基本的字典结构和缓存操作。它可以用于缓存任何类型的Python对象，但不支持序列化和反序列化操作。
 
 ```python
 from cushy_storage import BaseDict
 
-cache = BaseDict('./cache')
+# 初始化cache，保存在./data文件夹下
+cache = BaseDict('./data')
 cache['key'] = b'value'
 value = cache['key']
+print(value)
 
 ```
 
 ## CushyDict类
 
-CushyDict类是CushyStorage库的高级实现，增加了对值进行序列化和反序列化的功能。它支持多种序列化算法（包括pickle和json）和压缩算法（包括zlib和lzma），可以根据需要选择不同的算法进行数据压缩和序列化。
+CushyDict类是BaseDict库的高级实现，增加了对值进行序列化和反序列化的功能。它支持多种序列化算法（包括pickle和json）和压缩算法（包括zlib和lzma），可以根据需要选择不同的算法进行数据压缩和序列化。
 
 ```python
 from cushy_storage import CushyDict
 
-cache = CushyDict('./cache')
+# 初始化cache，保存在./data文件夹下
+cache = CushyDict('./data')
 cache['key'] = {'value': 42}
 value = cache['key']
+print(value)
+
+```
+
+- 判断key是否存在
+
+```python
+from cushy_storage import CushyDict
+
+cache = CushyDict('./data')
+if 'key' in cache:
+    print("key exist")
+else:
+    print("key not exist")
 
 ```
 
 ## disk_cache装饰器函数
 
 disk_cache装饰器函数可以将函数的输出结果缓存到磁盘中，以便下次使用时直接读取。通过该装饰器，可以在不改变原有代码逻辑的情况下，大幅度提高程序的执行效率。
 
 ```python
 from cushy_storage import disk_cache
 
-@disk_cache('./cache')
+@disk_cache('./data')
 def my_func():
     return {'value': 42}
 
 result = my_func()
 
 ```
  
  
 # 待办
 
+- [ ] 提供单例模式解决方案，提供更加方便的磁盘缓存方案
 - [ ] 支持更多的压缩和序列化算法，以满足不同类型数据的需求
 - [ ] 提供更加友好的错误处理机制，让用户更容易发现和解决问题
 - [ ] 改进缓存管理策略，确保缓存数据的可靠性和一致性
 - [ ] 提供更加丰富的测试用例，并定期进行性能测试和升级
 - [ ] 支持分布式缓存，可以在多台机器上共享缓存数据
 - [ ] 增加缓存过期功能，可以自动删除长时间未使用的缓存数据
 - [ ] 改善文档结构和代码注释，方便用户理解和使用库
```

### Comparing `cushy-storage-1.0.0/setup.py` & `cushy-storage-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setuptools.setup(
     name="cushy-storage",
-    version="1.0.0",
+    version="1.0.1",
     author="Zeeland",
     author_email="zeeland@foxmail.com",
     description="A data local persistence framework library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Undertone0809/cushy-storage",
     packages=setuptools.find_packages(),
```

### Comparing `cushy-storage-1.0.0/tests/test_cushy_dict.py` & `cushy-storage-1.0.1/tests/test_base_dict.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # Project Link: https://github.com/Undertone0809/cushy-storage
 # Contact Email: zeeland@foxmail.com
 
 import unittest
 from cushy_storage import CushyDict
 
 
-class TestCushyDict(unittest.TestCase):
+class TestBaseDict(unittest.TestCase):
     def test_basic_operations(self):
         cache = CushyDict('./test-cache')
 
         # Test adding items to the cache
         cache['foo'] = b'bar'
         self.assertEqual(cache['foo'], b'bar')
```

### Comparing `cushy-storage-1.0.0/tests/test_dict_cache.py` & `cushy-storage-1.0.1/tests/test_dict_cache.py`

 * *Files identical despite different names*

