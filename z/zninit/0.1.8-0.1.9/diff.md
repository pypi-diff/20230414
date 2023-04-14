# Comparing `tmp/zninit-0.1.8.tar.gz` & `tmp/zninit-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zninit-0.1.8.tar", max compression
+gzip compressed data, was "zninit-0.1.9.tar", max compression
```

## Comparing `zninit-0.1.8.tar` & `zninit-0.1.9.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0    13575 2022-09-19 09:28:07.825297 zninit-0.1.8/LICENSE
--rw-r--r--   0        0        0     2801 2022-12-08 15:15:13.710312 zninit-0.1.8/README.md
--rw-r--r--   0        0        0     1487 2022-12-14 12:59:27.831163 zninit-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      295 2022-11-29 12:43:51.219511 zninit-0.1.8/zninit/__init__.py
--rw-r--r--   0        0        0     9897 2022-12-14 13:20:56.149029 zninit-0.1.8/zninit/core/__init__.py
--rw-r--r--   0        0        0     7362 2022-12-14 14:43:40.301711 zninit-0.1.8/zninit/descriptor/__init__.py
--rw-r--r--   0        0        0     3560 1970-01-01 00:00:00.000000 zninit-0.1.8/setup.py
--rw-r--r--   0        0        0     3545 1970-01-01 00:00:00.000000 zninit-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    13575 2023-03-14 10:37:20.833990 zninit-0.1.9/LICENSE
+-rw-r--r--   0        0        0     2974 2023-03-14 10:37:20.833990 zninit-0.1.9/README.md
+-rw-r--r--   0        0        0     1570 2023-03-14 11:06:48.394407 zninit-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      295 2023-03-14 10:37:20.953989 zninit-0.1.9/zninit/__init__.py
+-rw-r--r--   0        0        0    10232 2023-03-14 11:06:48.394407 zninit-0.1.9/zninit/core/__init__.py
+-rw-r--r--   0        0        0     7712 2023-03-14 10:37:20.953989 zninit-0.1.9/zninit/descriptor/__init__.py
+-rw-r--r--   0        0        0     3719 1970-01-01 00:00:00.000000 zninit-0.1.9/PKG-INFO
```

### Comparing `zninit-0.1.8/LICENSE` & `zninit-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `zninit-0.1.8/README.md` & `zninit-0.1.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 [![Coverage Status](https://coveralls.io/repos/github/zincware/ZnInit/badge.svg?branch=main)](https://coveralls.io/github/zincware/ZnInit?branch=main)
 ![PyTest](https://github.com/zincware/ZnInit/actions/workflows/pytest.yaml/badge.svg)
 [![PyPI version](https://badge.fury.io/py/zninit.svg)](https://badge.fury.io/py/zninit)
 [![code-style](https://img.shields.io/badge/code%20style-black-black)](https://github.com/psf/black/)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/zincware/ZnInit/HEAD)
+[![zincware](https://img.shields.io/badge/Powered%20by-zincware-darkcyan)](https://github.com/zincware)
 
 # ZnInit - Automatic Generation of ``__init__`` based on Descriptors
 
 This package provides a base class for ``dataclass`` like structures with the addition of using [Descriptors](https://docs.python.org/3/howto/descriptor.html).
 The main functionality is the automatic generation of an keyword-only``__init__`` based on selected descriptors.
 The descriptors can e.g. overwrite ``__set__`` or ``__get__`` or have custom metadata associated with them.
 The ``ZnInit`` package is used by [ZnTrack](https://github.com/zincware/ZnTrack) to enable lazy loading data from files as well as distinguishing between different types of descriptors such as `zn.params` or `zn.outputs`. An example can be found in the `examples` directory.
@@ -57,14 +58,15 @@
     def _post_init_(self):
         self.date = "2022-09-16"
 
 
 julian = Human(name="Julian")
 print(julian) # Human(language='DE', name='Julian')
 print(julian.date)  # 2022-09-16
+print(Input.get_dict(julian)) # {"name": "Julian", "language": "DE"}
 ````
 One benefit of ``ZnInit`` is that it also allows for inheritance.
 
 ````python
 from zninit import ZnInit, Descriptor
 
 class Animal(ZnInit):
```

### Comparing `zninit-0.1.8/pyproject.toml` & `zninit-0.1.9/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 [tool.poetry]
 name = "zninit"
-version = "0.1.8"
+version = "0.1.9"
 description = "Descriptor based dataclass implementation"
 authors = ["zincwarecode <zincwarecode@gmail.com>"]
 license = "Apache-2.0"
 keywords = ["dataclass", "descriptor"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 typeguard = {version = "^2.13.3", optional = true}
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.3"
-black = "^22.8.0"
-isort = "^5.10.1"
-jupyterlab = "^3.4.7"
 coverage = "^6.4.4"
 pylint = "^2.15.2"
 perflint = "^0.7.3"
 pre-commit = "^2.20.0"
-ruff = "^0.0.126"
+
+[tool.poetry.group.notebook.dependencies]
+jupyterlab = "^3.4.7"
+
+
+[tool.poetry.group.lint.dependencies]
+black = "^23.1.0"
+ruff = "^0.0.255"
+isort = "^5.12.0"
 
 [tool.poetry.extras]
 typeguard = ["typeguard"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `zninit-0.1.8/zninit/core/__init__.py` & `zninit-0.1.9/zninit/core/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     super_init: Callable
         typically this is Node.__init__
     """
     kwargs_no_default = [] if kwargs_no_default is None else kwargs_no_default
     kwargs_with_default = {} if kwargs_with_default is None else kwargs_with_default
 
     def auto_init(self, *args, **kwargs):
-        """Wrapper for the __init__."""
+        """Wrap the __init__ method to generate automatic keyword arguments."""
         init_kwargs = {}
         required_keys = []
         uses_auto_init = getattr(self.__init__, "uses_auto_init", False)
         cls_name = self.__class__.__name__
         if args:
             raise get_args_type_error(args, cls_name, uses_auto_init)
         log.debug(f"The '__init__' uses auto_init: {uses_auto_init}")
@@ -229,24 +229,25 @@
         return self.use_repr
 
     @property
     def _init_subclass_basecls_(self) -> typing.Type:
         return self.init_subclass_basecls
 
     def __init__(self):
-        """Required for Error messages.
+        """Define the __init__ because it is required for error messages.
 
         Otherwise, it would just raise 'object.__init__() takes exactly one argument'
 
         Raises
         ------
         TypeError: ZnInit.__init__() got an unexpected keyword argument ...
         """
 
     def __init_subclass__(cls, **kwargs):
+        """Magic method which is called upon class inheritance."""
         super().__init_subclass__(**kwargs)
         _init_subclass_basecls_ = object.__new__(cls)._init_subclass_basecls_
 
         if _init_subclass_basecls_ is None:
             _init_subclass_basecls_ = ZnInit
         for inherited in cls.__mro__:
             # Go through the mro until you find the init_subclass_basecls.
@@ -269,15 +270,20 @@
         if not self._use_repr_:
             return super().__repr__()
         repr_str = f"{self.__class__.__name__}("
         fields = []
         for descriptor in get_descriptors(descriptor=self._init_descriptors_, self=self):
             if not descriptor.use_repr:
                 continue
-            representation = descriptor.get_repr(getattr(self, descriptor.name))
+
+            try:
+                representation = descriptor.get_repr(getattr(self, descriptor.name))
+            except AttributeError:
+                # repr should never raise an AttributeError (or any error actually).
+                representation = "<AttributeError>"
 
             fields.append(f"{descriptor.name}={representation}")
         repr_str += ", ".join(fields)
         repr_str += ")"
         return repr_str
 
     def _post_init_(self):
```

### Comparing `zninit-0.1.8/zninit/descriptor/__init__.py` & `zninit-0.1.9/zninit/descriptor/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,14 +98,23 @@
         self.on_setattr = on_setattr
         self._frozen = weakref.WeakKeyDictionary()
         if check_types and ("typeguard" not in sys.modules):
             raise ImportError(
                 "Need to install 'pip install zninit[typeguard]' for type checking."
             )
 
+    @classmethod
+    def get_dict(cls, instance: typing.Any) -> dict:
+        """Get a {attribute-name: value} dict from instance for this descriptor."""
+        descriptors = get_descriptors(cls, self=instance)
+        return {
+            descriptor.name: getattr(instance, descriptor.name)
+            for descriptor in descriptors
+        }
+
     @property
     def name(self):
         """Property for the name attribute to protect changing it."""
         return self._name
 
     @property
     def owner(self):
@@ -128,24 +137,24 @@
 
         Raises
         ------
         KeyError:
             if type checking and the descriptor has no annotation.
         """
         try:
-            annotations = self.owner.__annotations__
+            annotations_ = self.owner.__annotations__
         except AttributeError:
-            annotations = {}
+            annotations_ = {}
 
-        if self.check_types and self.name not in annotations:
+        if self.check_types and self.name not in annotations_:
             raise KeyError(
                 f"Could not find 'annotation' for {self.name} in '{self.owner}' with"
                 " 'check_types=True'"
             )
-        return annotations.get(self.name)
+        return annotations_.get(self.name)
 
     def __set_name__(self, owner, name):
         """Store name of the descriptor in the parent class."""
         self._owner = owner
         self._name = name
 
     def __get__(self, instance, owner=None):
```

### Comparing `zninit-0.1.8/setup.py` & `zninit-0.1.9/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,100 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: zninit
+Version: 0.1.9
+Summary: Descriptor based dataclass implementation
+License: Apache-2.0
+Keywords: dataclass,descriptor
+Author: zincwarecode
+Author-email: zincwarecode@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: typeguard
+Requires-Dist: typeguard (>=2.13.3,<3.0.0) ; extra == "typeguard"
+Project-URL: repository, https://github.com/zincware/ZnInit
+Description-Content-Type: text/markdown
+
+[![Coverage Status](https://coveralls.io/repos/github/zincware/ZnInit/badge.svg?branch=main)](https://coveralls.io/github/zincware/ZnInit?branch=main)
+![PyTest](https://github.com/zincware/ZnInit/actions/workflows/pytest.yaml/badge.svg)
+[![PyPI version](https://badge.fury.io/py/zninit.svg)](https://badge.fury.io/py/zninit)
+[![code-style](https://img.shields.io/badge/code%20style-black-black)](https://github.com/psf/black/)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/zincware/ZnInit/HEAD)
+[![zincware](https://img.shields.io/badge/Powered%20by-zincware-darkcyan)](https://github.com/zincware)
+
+# ZnInit - Automatic Generation of ``__init__`` based on Descriptors
+
+This package provides a base class for ``dataclass`` like structures with the addition of using [Descriptors](https://docs.python.org/3/howto/descriptor.html).
+The main functionality is the automatic generation of an keyword-only``__init__`` based on selected descriptors.
+The descriptors can e.g. overwrite ``__set__`` or ``__get__`` or have custom metadata associated with them.
+The ``ZnInit`` package is used by [ZnTrack](https://github.com/zincware/ZnTrack) to enable lazy loading data from files as well as distinguishing between different types of descriptors such as `zn.params` or `zn.outputs`. An example can be found in the `examples` directory.
+
+# Example
+The most simple use case is a replication of a dataclass like structure.
+
+```python
+from zninit import ZnInit, Descriptor
+
+
+class Human(ZnInit):
+    name: str = Descriptor()
+    language: str = Descriptor("EN")
+
+
+# This will generate the following init:
+def __init__(self, *, name, language="EN"):
+    self.name = name
+    self.language = language
+
+
+fabian = Human(name="Fabian")
+# or
+fabian = Human(name="Fabian", language="DE")
+```
+
+The benefit of using ``ZnInit`` comes with using descriptors. You can subclass the `zninit.Descriptor` class and only add certain kwargs to the `__init__` defined in `init_descriptors: list`. Furthermore, a `post_init` method is available to run code immediately after initializing the class.
+
+````python
+from zninit import ZnInit, Descriptor
+
+
+class Input(Descriptor):
+    """A Parameter"""
+
+
+class Metric(Descriptor):
+    """An Output"""
+
+
+class Human(ZnInit):
+    _init_descriptors_ = [Input] # only add Input descriptors to the __init__
+    name: str = Input()
+    language: str = Input("DE")
+    date: str = Metric()  # will not appear in the __init__
+
+    def _post_init_(self):
+        self.date = "2022-09-16"
+
+
+julian = Human(name="Julian")
+print(julian) # Human(language='DE', name='Julian')
+print(julian.date)  # 2022-09-16
+print(Input.get_dict(julian)) # {"name": "Julian", "language": "DE"}
+````
+One benefit of ``ZnInit`` is that it also allows for inheritance.
+
+````python
+from zninit import ZnInit, Descriptor
+
+class Animal(ZnInit):
+    age: int = Descriptor()
+    
+class Cat(Animal):
+    name: str = Descriptor()
+    
+billy = Cat(age=4, name="Billy")
+````
 
-packages = \
-['zninit', 'zninit.core', 'zninit.descriptor']
-
-package_data = \
-{'': ['*']}
-
-extras_require = \
-{'typeguard': ['typeguard>=2.13.3,<3.0.0']}
-
-setup_kwargs = {
-    'name': 'zninit',
-    'version': '0.1.8',
-    'description': 'Descriptor based dataclass implementation',
-    'long_description': '[![Coverage Status](https://coveralls.io/repos/github/zincware/ZnInit/badge.svg?branch=main)](https://coveralls.io/github/zincware/ZnInit?branch=main)\n![PyTest](https://github.com/zincware/ZnInit/actions/workflows/pytest.yaml/badge.svg)\n[![PyPI version](https://badge.fury.io/py/zninit.svg)](https://badge.fury.io/py/zninit)\n[![code-style](https://img.shields.io/badge/code%20style-black-black)](https://github.com/psf/black/)\n[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/zincware/ZnInit/HEAD)\n\n# ZnInit - Automatic Generation of ``__init__`` based on Descriptors\n\nThis package provides a base class for ``dataclass`` like structures with the addition of using [Descriptors](https://docs.python.org/3/howto/descriptor.html).\nThe main functionality is the automatic generation of an keyword-only``__init__`` based on selected descriptors.\nThe descriptors can e.g. overwrite ``__set__`` or ``__get__`` or have custom metadata associated with them.\nThe ``ZnInit`` package is used by [ZnTrack](https://github.com/zincware/ZnTrack) to enable lazy loading data from files as well as distinguishing between different types of descriptors such as `zn.params` or `zn.outputs`. An example can be found in the `examples` directory.\n\n# Example\nThe most simple use case is a replication of a dataclass like structure.\n\n```python\nfrom zninit import ZnInit, Descriptor\n\n\nclass Human(ZnInit):\n    name: str = Descriptor()\n    language: str = Descriptor("EN")\n\n\n# This will generate the following init:\ndef __init__(self, *, name, language="EN"):\n    self.name = name\n    self.language = language\n\n\nfabian = Human(name="Fabian")\n# or\nfabian = Human(name="Fabian", language="DE")\n```\n\nThe benefit of using ``ZnInit`` comes with using descriptors. You can subclass the `zninit.Descriptor` class and only add certain kwargs to the `__init__` defined in `init_descriptors: list`. Furthermore, a `post_init` method is available to run code immediately after initializing the class.\n\n````python\nfrom zninit import ZnInit, Descriptor\n\n\nclass Input(Descriptor):\n    """A Parameter"""\n\n\nclass Metric(Descriptor):\n    """An Output"""\n\n\nclass Human(ZnInit):\n    _init_descriptors_ = [Input] # only add Input descriptors to the __init__\n    name: str = Input()\n    language: str = Input("DE")\n    date: str = Metric()  # will not appear in the __init__\n\n    def _post_init_(self):\n        self.date = "2022-09-16"\n\n\njulian = Human(name="Julian")\nprint(julian) # Human(language=\'DE\', name=\'Julian\')\nprint(julian.date)  # 2022-09-16\n````\nOne benefit of ``ZnInit`` is that it also allows for inheritance.\n\n````python\nfrom zninit import ZnInit, Descriptor\n\nclass Animal(ZnInit):\n    age: int = Descriptor()\n    \nclass Cat(Animal):\n    name: str = Descriptor()\n    \nbilly = Cat(age=4, name="Billy")\n````\n',
-    'author': 'zincwarecode',
-    'author_email': 'zincwarecode@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'extras_require': extras_require,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

