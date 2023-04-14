# Comparing `tmp/stretchy-1.0b3.tar.gz` & `tmp/stretchy-1.1b1.tar.gz`

## Comparing `stretchy-1.0b3.tar` & `stretchy-1.1b1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 stretchy-1.0b3/src/stretchy/__init__.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 stretchy-1.0b3/src/stretchy/__init__.pyi
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 stretchy-1.0b3/src/stretchy/abc.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 stretchy-1.0b3/src/stretchy/abc.pyi
--rw-r--r--   0        0        0     5361 2020-02-02 00:00:00.000000 stretchy-1.0b3/src/stretchy/array1d.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 stretchy-1.0b3/src/stretchy/array1d.pyi
--rw-r--r--   0        0        0     8116 2020-02-02 00:00:00.000000 stretchy-1.0b3/src/stretchy/arraynd.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 stretchy-1.0b3/src/stretchy/arraynd.pyi
--rw-r--r--   0        0        0     4730 2020-02-02 00:00:00.000000 stretchy-1.0b3/src/stretchy/format.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 stretchy-1.0b3/src/stretchy/format.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stretchy-1.0b3/src/stretchy/py.typed
--rw-r--r--   0        0        0     5686 2020-02-02 00:00:00.000000 stretchy-1.0b3/tests/test_array1d.py
--rw-r--r--   0        0        0     9382 2020-02-02 00:00:00.000000 stretchy-1.0b3/tests/test_arraynd.py
--rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 stretchy-1.0b3/tests/test_main.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 stretchy-1.0b3/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 stretchy-1.0b3/LICENSE
--rw-r--r--   0        0        0    15617 2020-02-02 00:00:00.000000 stretchy-1.0b3/README.md
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 stretchy-1.0b3/pyproject.toml
--rw-r--r--   0        0        0    16181 2020-02-02 00:00:00.000000 stretchy-1.0b3/PKG-INFO
+-rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 stretchy-1.1b1/src/stretchy/__init__.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 stretchy-1.1b1/src/stretchy/__init__.pyi
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 stretchy-1.1b1/src/stretchy/abc.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 stretchy-1.1b1/src/stretchy/abc.pyi
+-rw-r--r--   0        0        0     6517 2020-02-02 00:00:00.000000 stretchy-1.1b1/src/stretchy/array1d.py
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 stretchy-1.1b1/src/stretchy/array1d.pyi
+-rw-r--r--   0        0        0    10368 2020-02-02 00:00:00.000000 stretchy-1.1b1/src/stretchy/arraynd.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 stretchy-1.1b1/src/stretchy/arraynd.pyi
+-rw-r--r--   0        0        0     4730 2020-02-02 00:00:00.000000 stretchy-1.1b1/src/stretchy/format.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 stretchy-1.1b1/src/stretchy/format.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stretchy-1.1b1/src/stretchy/py.typed
+-rw-r--r--   0        0        0     7862 2020-02-02 00:00:00.000000 stretchy-1.1b1/tests/test_array1d.py
+-rw-r--r--   0        0        0    12139 2020-02-02 00:00:00.000000 stretchy-1.1b1/tests/test_arraynd.py
+-rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 stretchy-1.1b1/tests/test_main.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 stretchy-1.1b1/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 stretchy-1.1b1/LICENSE
+-rw-r--r--   0        0        0    17781 2020-02-02 00:00:00.000000 stretchy-1.1b1/README.md
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 stretchy-1.1b1/pyproject.toml
+-rw-r--r--   0        0        0    18345 2020-02-02 00:00:00.000000 stretchy-1.1b1/PKG-INFO
```

### Comparing `stretchy-1.0b3/src/stretchy/__init__.py` & `stretchy-1.1b1/src/stretchy/__init__.py`

 * *Files identical despite different names*

### Comparing `stretchy-1.0b3/src/stretchy/array1d.py` & `stretchy-1.1b1/src/stretchy/array1d.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/python3
 
 import itertools
-from typing import Any, Callable, TypeVar
+from typing import Any, Callable, TypeVar, overload
 from collections.abc import Iterable, Iterator
 
 from .abc import Array
 from .format import *
 
 T = TypeVar('T')
 Boundaries = tuple[tuple[int, int], ...]
@@ -49,14 +49,49 @@
             for index in range(-offset-1,-1,-1):
                 self._neg[index] = next(it)
             while True:
                 self._pos.append(next(it))
         except StopIteration:
             return
 
+    def trim(self) -> None:
+        while self._pos and self._pos[-1] == self._default:
+            self._pos.pop()
+        while self._neg and self._neg[-1] == self._default:
+            self._neg.pop()
+
+    @overload
+    def shrink_by(self, by: int) -> None: ...
+    @overload
+    def shrink_by(self, by: tuple[int, int]) -> None: ...
+
+    def shrink_by(self, by) -> None:
+        if isinstance(by, int):
+            by = (by, by)
+        bound: int = len(self._neg) - by[0]
+        if bound < 0:
+            bound = 0
+        del self._neg[bound:]
+        bound = len(self._pos) - by[1]
+        if bound < 0:
+            bound = 0
+        del self._pos[bound:]
+
+    def crop_to(self, boundaries: tuple[int, int]) -> None:
+        neg_bound, pos_bound = boundaries
+        if neg_bound > 0 or pos_bound < 0:
+            raise ValueError('Lower bound cannot be positive and upper one cannot be negative')
+        if len(self._pos) > pos_bound:
+            del self._pos[pos_bound:]
+        if len(self._neg) > -neg_bound:
+            del self._neg[-neg_bound:]
+
+
+    def __bool__(self) -> bool:
+        return bool(self._neg) or bool(self._pos)
 
     def __setitem__(self, index: int|slice, value: T|None) -> None:
         dim: list[int|None] = [None, None]
         if isinstance(index, slice):
             range_indices = self._range_indices(index)
             # Fill with value! (Python collections do not support this)
             for i in range(*range_indices):
```

### Comparing `stretchy-1.0b3/src/stretchy/array1d.pyi` & `stretchy-1.1b1/src/stretchy/array1d.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 from .format import *
 import itertools
 from .abc import Array as Array
 from collections.abc import Iterable, Iterator
-from typing import TypeVar
+from typing import TypeVar, overload
 
 T = TypeVar('T')
 Boundaries = tuple[tuple[int, int], ...]
 
 class Array1D(Array):
     def __init__(self, default: Union[T, None] = ..., *, content: Union[Iterable, None] = ..., offset: int = ...) -> None: ...
     @property
     def dim(self) -> int: ...
     @property
     def offset(self) -> int: ...
     @property
     def boundaries(self) -> tuple[int, int]: ...
     def replace_content(self, content: Iterable, offset: int = ...) -> None: ...
+    def trim(self) -> None: ...
+    @overload
+    def shrink_by(self, by: int) -> None: ...
+    @overload
+    def shrink_by(self, by: tuple[int, int]) -> None: ...
+    def crop_to(self, boundaries: tuple[int, int]) -> None: ...
+    def __bool__(self) -> bool: ...
     def __setitem__(self, index: Union[int, slice], value: Union[T, None]) -> None: ...
     def __getitem__(self, index: Union[int, slice]) -> Union[T, Iterator, None]: ...
     def __iter__(self) -> itertools.chain: ...
     def __len__(self) -> int: ...
     def __format__(self, format: str) -> str: ...
```

### Comparing `stretchy-1.0b3/src/stretchy/arraynd.py` & `stretchy-1.1b1/src/stretchy/arraynd.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 #!/usr/bin/python3
 
 from collections.abc import Iterator, Sequence
 import itertools
-from typing import Any, TypeVar
+from typing import Any, TypeVar, overload
 #>from typing import Self # from v3.11!
 
 from .abc import Array
 from .array1d import Array1D
 from .format import *
 
 T = TypeVar('T')
-Boundaries = tuple[tuple[int, int], ...]
+#>Boundaries = tuple[tuple[int, int], ...] | list[tuple[int, int] | list[int]]
+Boundaries = Sequence[tuple[int, int] | list[int]]
 
 def _minmax(arr: tuple[tuple[int, int], ...]) -> tuple[int, int]:
     minarr, maxarr = zip(*arr)
     return min(minarr), max(maxarr)
 
 
 class ArrayND(Array):
@@ -57,38 +58,95 @@
             all_bounds = ((plane.boundaries,) for plane in self)
         else:
             all_bounds = (plane.boundaries for plane in self)
         boundmax: Iterator[tuple[int, int]] = (_minmax(a) for a in zip(*all_bounds))
         return ((-len(self._neg), len(self._pos)), *boundmax)
 
 
-    def replace_content(self, array: Sequence,
-                        offset: tuple[int,...]|list[int]|int = 0) -> None:
+    def replace_content(self, content: Sequence|None = None,
+                        offset: tuple[int,...]|list[int]|int = 0,
+                        *, array: Sequence|None = None) -> None:
+        if content is None:
+            content = array
+        assert content is not None
         self._neg = []
         self._pos = []
         if isinstance(offset, int):
             offset = [offset] * self._dim
         offset = list(offset)
         current_offset: int = 0
         sub_offset: list[int] = [0]
         if len(offset) > 0:
             current_offset = offset[0]
             if len(offset) > 1:
                 sub_offset = offset[1:]
-        for index, subarray in enumerate(array, current_offset):
+        for index, subcontent in enumerate(content, current_offset):
             plane = self._getplane(index) # Self|Array1D
             if self._dim == 2:
-                plane.replace_content(subarray, sub_offset[0])
+                plane.replace_content(subcontent, sub_offset[0])
             else:
-                plane.replace_content(subarray, sub_offset)
+                plane.replace_content(subcontent, sub_offset)
+
+    def trim(self) -> None:
+        for plane in self:
+            plane.trim()
+        while self._pos and not self._pos[-1]:
+            self._pos.pop()
+        while self._neg and not self._neg[-1]:
+            self._neg.pop()
+
+    @overload
+    def shrink_by(self, by: int) -> None: ...
+    @overload
+    def shrink_by(self, by: tuple[int, ...]) -> None: ...
+    @overload
+    def shrink_by(self, by: tuple[tuple[int, int], ...]) -> None: ...
+
+    def shrink_by(self, by) -> None:
+        if isinstance(by, int):
+            by = ((by, by),) * self._dim
+        if not isinstance(by, tuple) or len(by) != self._dim \
+                or any(map(lambda x: not isinstance(x, (int, tuple)), by)):
+            raise TypeError(f'`by` value must be an int or a {self._dim} element tuple of integers or integer pairs')
+        if isinstance(by[0], int):
+            by = tuple((b, b) for b in by)
+        boundaries: list[tuple[int, int]] = []
+        for curby, (curlow, curup) in zip(by, self.boundaries):
+            neg_bound: int = curlow + curby[0]
+            if neg_bound > 0:
+                neg_bound = 0
+            pos_bound: int = curup - curby[1]
+            if pos_bound < 0:
+                pos_bound = 0
+            boundaries.append((neg_bound, pos_bound))
+        self.crop_to(boundaries)
+
+    def crop_to(self, boundaries: Boundaries) -> None:
+        neg_bound, pos_bound = boundaries[0]
+        if neg_bound > 0 or pos_bound < 0:
+            raise ValueError(f'Lower bounds cannot be positive and upper ones cannot be negative')
+        if len(self._pos) > pos_bound:
+            del self._pos[pos_bound:]
+        if len(self._neg) > -neg_bound:
+            del self._neg[-neg_bound:]
+        if self._dim == 2:
+            for plane in self:
+                plane.crop_to(boundaries[1])
+        else:
+            for plane in self:
+                plane.crop_to(boundaries[1:])
+
+
+    def __bool__(self) -> bool:
+        return bool(self._neg) or bool(self._pos)
 
     def __setitem__(self, index: tuple[int, ...], value: T) -> None:
         if not isinstance(index, tuple) or len(index) != self._dim \
                 or any(map(lambda x: not isinstance(x, int), index)):
-            raise TypeError('Index must be a {self._dim} element tuple of integers')
+            raise TypeError(f'Index must be a {self._dim} element tuple of integers')
         plane = self._getplane(index[0]) # Self|Array1D
         if self._dim == 2:
             plane[index[1]] = value
         else:
             plane[index[1:]] = value
 
     def __getitem__(self, index: int|tuple[int, ...]|slice) -> Any: # Self|Array1D|T
@@ -96,15 +154,15 @@
             range_indices = self._range_indices(index)
             # Return iterator instead of some arbitrary collection
             return (self._getplane(i) for i in range(*range_indices))
         if isinstance(index, int):
             return self._getplane(index)
         if not isinstance(index, tuple) or len(index) != self._dim \
                 or any(map(lambda x: not isinstance(x, int), index)):
-            raise TypeError('Index must be a {self._dim} element tuple of integers')
+            raise TypeError(f'Index must be a {self._dim} element tuple of integers')
         plane = self._getplane(index[0], create=False)
         if plane is None:
             return self._default
         elif self._dim == 2:
             return plane[index[1]]
         else:
             return plane[index[1:]]
```

### Comparing `stretchy-1.0b3/src/stretchy/arraynd.pyi` & `stretchy-1.1b1/src/stretchy/arraynd.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,37 @@
 from .format import *
 import itertools
 from .abc import Array as Array
 from .array1d import Array1D as Array1D
+from _typeshed import Incomplete
 from collections.abc import Sequence
-from typing import Any, TypeVar
+from typing import Any, TypeVar, overload
 
 T = TypeVar('T')
-Boundaries = tuple[tuple[int, int], ...]
+Boundaries: Incomplete
 
 class ArrayND(Array):
     index_format: Union[str, None]
     def __init__(self, dim: int, default: Union[T, None] = ..., *, content: Union[Sequence, None] = ..., offset: Union[tuple[int, ...], list[int], int] = ...) -> None: ...
     @property
     def dim(self) -> int: ...
     @property
     def offset(self) -> tuple[int, ...]: ...
     @property
     def shape(self) -> tuple[int, ...]: ...
     @property
     def boundaries(self) -> Boundaries: ...
-    def replace_content(self, array: Sequence, offset: Union[tuple[int, ...], list[int], int] = ...) -> None: ...
+    def replace_content(self, content: Union[Sequence, None] = ..., offset: Union[tuple[int, ...], list[int], int] = ..., *, array: Union[Sequence, None] = ...) -> None: ...
+    def trim(self) -> None: ...
+    @overload
+    def shrink_by(self, by: int) -> None: ...
+    @overload
+    def shrink_by(self, by: tuple[int, ...]) -> None: ...
+    @overload
+    def shrink_by(self, by: tuple[tuple[int, int], ...]) -> None: ...
+    def crop_to(self, boundaries: Boundaries) -> None: ...
+    def __bool__(self) -> bool: ...
     def __setitem__(self, index: tuple[int, ...], value: T) -> None: ...
     def __getitem__(self, index: Union[int, tuple[int, ...], slice]) -> Any: ...
     def __iter__(self) -> itertools.chain: ...
     def __len__(self) -> int: ...
     def __format__(self, format: str) -> str: ...
```

### Comparing `stretchy-1.0b3/src/stretchy/format.py` & `stretchy-1.1b1/src/stretchy/format.py`

 * *Files identical despite different names*

### Comparing `stretchy-1.0b3/src/stretchy/format.pyi` & `stretchy-1.1b1/src/stretchy/format.pyi`

 * *Files identical despite different names*

### Comparing `stretchy-1.0b3/tests/test_array1d.py` & `stretchy-1.1b1/tests/test_array1d.py`

 * *Files 20% similar despite different names*

```diff
@@ -97,14 +97,15 @@
 def test_getitem_slice(indices, content, got):
     s = Array1D(default='.', content='abcdefghi', offset=-4)
     assert ''.join(s[slice(*indices)]) == got
 
 
 # Followings test also the `replace_content` method
 TEST_DATA = (
+    ((tuple(),), []),
     (((7,),), [7]),
     (((7,),2), [None, None, 7]),
     (((7,),-2), [7, None]),
     (((7,8,9),2), [None, None, 7, 8, 9]),
     (((7,8,9),-2), [7, 8, 9]),
 )
 
@@ -128,14 +129,22 @@
 def test_len(arr, content):
     s = Array1D()
     s.replace_content(*arr)
     assert len(s) == len(content)
 
 
 @pytest.mark.parametrize('arr, content', TEST_DATA)
+def test_bool(arr, content):
+    s = Array1D()
+    s.replace_content(*arr)
+    exp = content != []
+    assert bool(s) is exp
+
+
+@pytest.mark.parametrize('arr, content', TEST_DATA)
 def test_iter(arr, content):
     s = Array1D()
     s.replace_content(*arr)
     assert list(s) == content
 
 
 @pytest.mark.parametrize('params, offset, content',
@@ -144,20 +153,89 @@
         (('12345',3), 0, '...12345'),
         (('12345',-3), -3, '12345'),
         (('12345',-7), -7, '12345..'),
         (((1,2,3,4,5),-3), -3, '12345'),
         (([1,2,3,4,5],-3), -3, '12345'),
     )
 )
-def test_set(params, offset, content):
+def test_replace_content(params, offset, content):
     s = Array1D('.')
     s.replace_content(*params)
     assert s.offset == offset
     assert f'{s:s}' == content
 
+# ======== Resizing ========
+
+@pytest.mark.parametrize('params, content',
+    (
+        (('...12345...',), '...12345'),
+        (('...12345...', -2), '.12345'),
+        (('...12345...', -3), '12345'),
+        (('...12345...', -5), '12345'),
+        (('...12345...', -8), '12345'),
+        (('...12345...', -9), '12345.'),
+        (('...12345...', 1), '....12345'),
+        (('......', -3), ''),
+        (('......', -10), ''),
+        (('......', 10), ''),
+    )
+)
+def test_trim(params, content):
+    s = Array1D('.')
+    s.replace_content(*params)
+    s.trim()
+    assert f'{s:s}' == content
+
+@pytest.mark.parametrize('params, by, content',
+    (
+        (('123456789',), 3, '123456'),
+        (('123456789',), 0, '123456789'),
+        (('123456789',), 10, ''),
+        (('123456789',-2), 3, '3456'),
+        (('123456789',-2), 0, '123456789'),
+        (('123456789',-2), 10, ''),
+        (('123456789',-9), 3, '456789'),
+        (('123456789',-12), 10, '..'),
+        (('123456789',3), 10, '..'),
+        (('123456789',-4), (2,4), '345'),
+    )
+)
+def test_shrinkby(params, by, content):
+    s = Array1D('.')
+    s.replace_content(*params)
+    s.shrink_by(by)
+    assert f'{s:s}' == content
+
+@pytest.mark.parametrize('params, to, content',
+    (
+        (('123456789',), (-2,3), '123'),
+        (('123456789',), (-2,10), '123456789'),
+        (('123456789',-3), (-1,4), '34567'),
+        (('123456789',-3), (0,4), '4567'),
+        (('123456789',-3), (-3,0), '123'),
+        (('123456789',-3), (-10,10), '123456789'),
+        (('123456789',-12), (-5,5), '89...'),
+        (('123456789',3), (-5,5), '...12'),
+    )
+)
+def test_cropto(params, to, content):
+    s = Array1D('.')
+    s.replace_content(*params)
+    s.crop_to(to)
+    assert f'{s:s}' == content
+
+def test_wrong_cropto(array):
+    s = Array1D('.')
+    with pytest.raises(ValueError):
+        s.crop_to((2,5))
+    with pytest.raises(ValueError):
+        s.crop_to((-5,-2))
+
+
+# ======== Formatting ========
 
 @pytest.fixture
 def array():
     s = Array1D(default='.', offset=-3,
         content=('x', None,'.',234,'.',False,6.7))
     return s
```

### Comparing `stretchy-1.0b3/tests/test_arraynd.py` & `stretchy-1.1b1/tests/test_arraynd.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pytest
+import copy
 
 from stretchy import ArrayND
 
 def rows_to_str(rows):
     return '\n'.join(rows)
 
 
@@ -181,14 +182,18 @@
         c = max(plane[i,i] for i in (-1, 0, 1))
         check.append(c)
     assert ''.join(check) == content
 
 
 INPUT_DATA = (
     (
+        (tuple()),
+        ((0,0),(0,0)),
+        tuple()
+    ), (
         ((-1,-2),(-3,-1)),
         ((-3,0),(-2,0)),
         ('#','','#.')
     ), (
         ((1,2),(3,1)),
         ((0,4),(0,3)),
         ('','..#','','.#')
@@ -240,20 +245,113 @@
     s = ArrayND(len(boundaries), '.')
     for cell in cells:
         s[cell] = '#'
     assert len(s) == len(planes)
 
 
 @pytest.mark.parametrize('cells, boundaries, planes', INPUT_DATA)
+def test_bool(cells, boundaries, planes):
+    s = ArrayND(len(boundaries), '.')
+    for cell in cells:
+        s[cell] = '#'
+    exp = planes != tuple()
+    assert bool(s) is exp
+
+
+@pytest.mark.parametrize('cells, boundaries, planes', INPUT_DATA)
 def test_iter(cells, boundaries, planes):
     s = ArrayND(len(boundaries), '.')
     for cell in cells:
         s[cell] = '#'
     assert tuple(f'{sub:s}' for sub in s) == planes
 
+# ======== Resizing ========
+
+#       \/                            \/
+#   ..........  ..........  ..........  ..........  ..........  ..........
+# \ ..........  ..........  ...12345..  ..........  12345.....  ..........
+# / ..........  .....12345  ..........  ..........  ..........  ..........
+#   ..........  ..........  ..........  .......123  345.......  ..........
+#   ..........  ..........  ..........  ..........  ..........  ..........
+@pytest.fixture(scope='module')
+def trimmed():
+    s = ArrayND(3, '.')
+    empty = '.' * 10
+    empty_block = [empty] * 5
+    s.replace_content(array=[empty_block, [
+            empty, empty, '.....12345', empty, empty
+        ], [
+            empty, '...12345..', empty, empty, empty
+        ], [
+            empty, empty, empty, '.......123', empty
+        ], [
+            empty, '12345.....', empty, '345.......', empty
+        ], empty_block],
+        offset=(-3, -2, -5)
+        )
+    s.trim()
+    return s
+
+@pytest.mark.parametrize('select, content',
+    (
+        ((-2,), '12345'),
+        ((-2,0), '12345'),
+        ((-1,), '12345'),
+        ((-1,-1), '12345'),
+        ((0,), '.....\n..123'),
+        ((0,0), ''),
+        ((0,1), '..123'),
+        ((1,), '12345\n.....\n345..'),
+        ((1,0), ''),
+        ((1,1), '345..'),
+    )
+)
+def test_trim(select, content, trimmed):
+    s = copy.deepcopy(trimmed)
+    for n in select:
+        s = s[n]
+    assert f'{s:s}' == content
+
+@pytest.mark.parametrize('offset, by, content',
+    (
+        (0, 3, 'ab\nfg'),
+        (-2, 3, ''),
+        ((-2,2), 2, '..klm'),
+        ((-4,-7), 3, 'st..'),
+        (-2, (2,1), 'lmn'),
+        (-2, ((1,2),(0,1)), 'fghi\nklmn'),
+    )
+)
+def test_shrinkby(offset, by, content):
+    s = ArrayND(2, '.')
+    s.replace_content(
+        content=['abcde', 'fghij', 'klmno', 'pqrst', 'uvwxy'],
+        offset=offset
+        )
+    s.shrink_by(by)
+    assert f'{s:s}' == content
+
+@pytest.mark.parametrize('offset, to, content',
+    (
+        (0, ((-3,2),(-2,3)), 'abc\nfgh'),
+        (-2, ((0,0),(0,0)), ''),
+        (2, ((-1,1),(-1,1)), ''), # Note there is an empty "row" in there
+        ((-2,-3), ((-1,2),(-2,1)), 'ghi\nlmn\nqrs'),
+    )
+)
+def test_cropto(offset, to, content):
+    s = ArrayND(2, '.')
+    s.replace_content(
+        content=['abcde', 'fghij', 'klmno', 'pqrst', 'uvwxy'],
+        offset=offset
+        )
+    s.crop_to(to)
+    assert f'{s:s}' == content
+
+# ======== Formatting ========
 
 def test_str(array):
     expected = [
         '[[[[x          ]',
         '   [.       234]]',
         '',
         '  [[.     False]',
```

### Comparing `stretchy-1.0b3/tests/test_main.py` & `stretchy-1.1b1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `stretchy-1.0b3/LICENSE` & `stretchy-1.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `stretchy-1.0b3/README.md` & `stretchy-1.1b1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -295,23 +295,35 @@
 ```
 
 The function call gives the size  of the highest dimension of the array.
 This is  the length of  the array in  the one-dimensional case,  and the
 number of sub-planes (alse the first element of the `shape` property) in
 the case of multi-dimensional arrays.
 
+### Check array content
+
+```python
+if not array:
+    print("Array is empty!")
+```
+
+Casting array to bool works similarly to python sequences, i.e. if array
+is empty, it is converted to `False`, otherwise to `True`. The result is
+`True` also if array contains  exclusively default values. In this case,
+after [trimming](#trim), the result of the conversion will be `False`.
+
 ### Getting values or subplanes
 
 By indexing a stretchy array, you can perform several tasks depending on
 the type of index.
 
 ```python
-value: Any = array[5,-7,-2]
-subplane: stretchy.Array = array[3]
-itr: Iterator = array[-10:10:2]
+value = array[5,-7,-2]
+subplane = array[3]
+subplane_iterator = array[-10:10:2]
 ```
 
 To get the  **value** of a cell,  use a `tuple` in which  the values are
 the indices  of all dimensions. If  a non-existent cell is  indexed, the
 default value of the array is returned.
 
 You can also  get a **subplane** of  the array (indexed by  an `int`) on
@@ -367,18 +379,79 @@
 ```python
 replace_content(self, content: Iterable, offset: int = 0) -> None
 ```
 
 Multi-dimensional arrays:
 
 ```python
-replace_content(self, array: Sequence,
+replace_content(self, content: Sequence,
                       offset: tuple[int,...]|list[int]|int = 0) -> None
 ```
 
+Note, that `content` has been called  `array` in a previous version, but
+it has been deprecated by now. It will be removed in a later version.
+
+### Changing array size
+
+Thera are three methods, which can be used to resize/reshape the array:
+
+- [`trim`](#trim)
+- [`shrink_by`](#shrink_by)
+- [`crop_to`](#crop_to)
+
+These are described below.
+
+#### `trim`
+
+```python
+def trim(self) -> None
+```
+
+The method  can be  used to  cut off redundant  parts, i.e.  those where
+default values are  not followed by others. In such  a case, after trim,
+the array returns the same values at all positions as before (of course,
+other properties, such as boundary, may change).
+
+### `shrink_by`
+
+```python
+def shrink_by(self, by: int) -> None
+# dim >= 2:
+def shrink_by(self, by: tuple[int, ...]) -> None
+def shrink_by(self, by: tuple[tuple[int, int], ...]) -> None
+# dim = 1:
+def shrink_by(self, by: tuple[int, int]) -> None
+```
+
+The  method  can  be used  to  reduce  the  size  of the  array  in  all
+directions.  This can  lose  significant  data, but  if  there are  only
+default  values within  the specified  amount in  each directions,  only
+those values will  be deleted and the array will  not change in content.
+Of course, in all cases the the boundary's values will be reduced by the
+amount(s) of `by` (they will not exceed 0).
+
+If `by`  is of type `int`,  the array is  reduced by the same  amount in
+each direction. If  the type is a `tuple`, then  the amount of reduction
+along each axis in each direction must be given. In all cases the amount
+must be greater than or equal to zero.
+
+#### `crop_to`
+
+```python
+# dim >= 2:
+def crop_to(self, by: tuple[tuple[int, int], ...]) -> None
+# dim = 1:
+def crop_to(self, by: tuple[int, int]) -> None
+```
+
+The method can be used to cut  the array to any size in either direction
+in either dimension. Subject, of course, to the restriction that the two
+boundaries cannot  extend past the  zero point, i.e. the  lower boundary
+cannot be positive and the upper boundary cannot be negative.
+
 ### Iterating over the array
 
 Stretchy  arrays are  iterable.  This  means, that  you  can  use it  as
 follows:
 
 ```python
 import stretchy
@@ -599,18 +672,14 @@
 print(f'{array:s}')
 ```
 
 ## Future plans
 
 There are some ideas for future development:
 
-- **arbitrary  croping**:  Cut  to specified  size,  increase/shrink  by
-  amount (`int`) or reshape to boundaries
-- **normalization**:  Cut off  the default values  at the  boundaries to
-  prevent unnecessary storage
 - **offset  shifting**: Offset  an existing  array without  changing the
   contents. Also, offset to center.
 - **non-zero centric operation**: Do not require storage starting from 0
   if all elements are in the positive or negative range.
 - **sub-sub-planes**:  with  partial indexing  you  can  get plane  from
   any  levels. E.g.  in a  4-dimensional array,  `array[2,5]` returns  a
   2-dimensional one
```

### Comparing `stretchy-1.0b3/pyproject.toml` & `stretchy-1.1b1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "stretchy"
-version = "1.0b3"
+version = "1.1b1"
 authors = [
   { name="Ferenc Vajda", email="ferenc.vajda@gmail.com" },
 ]
 description = "One- and multi-dimensional containers that grow automatically in all directions"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `stretchy-1.0b3/PKG-INFO` & `stretchy-1.1b1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stretchy
-Version: 1.0b3
+Version: 1.1b1
 Summary: One- and multi-dimensional containers that grow automatically in all directions
 Project-URL: Homepage, https://github.com/fercsi/pylib-stretchy
 Project-URL: Bug Tracker, https://github.com/fercsi/pylib-stretchy/issues
 Author-email: Ferenc Vajda <ferenc.vajda@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -309,23 +309,35 @@
 ```
 
 The function call gives the size  of the highest dimension of the array.
 This is  the length of  the array in  the one-dimensional case,  and the
 number of sub-planes (alse the first element of the `shape` property) in
 the case of multi-dimensional arrays.
 
+### Check array content
+
+```python
+if not array:
+    print("Array is empty!")
+```
+
+Casting array to bool works similarly to python sequences, i.e. if array
+is empty, it is converted to `False`, otherwise to `True`. The result is
+`True` also if array contains  exclusively default values. In this case,
+after [trimming](#trim), the result of the conversion will be `False`.
+
 ### Getting values or subplanes
 
 By indexing a stretchy array, you can perform several tasks depending on
 the type of index.
 
 ```python
-value: Any = array[5,-7,-2]
-subplane: stretchy.Array = array[3]
-itr: Iterator = array[-10:10:2]
+value = array[5,-7,-2]
+subplane = array[3]
+subplane_iterator = array[-10:10:2]
 ```
 
 To get the  **value** of a cell,  use a `tuple` in which  the values are
 the indices  of all dimensions. If  a non-existent cell is  indexed, the
 default value of the array is returned.
 
 You can also  get a **subplane** of  the array (indexed by  an `int`) on
@@ -381,18 +393,79 @@
 ```python
 replace_content(self, content: Iterable, offset: int = 0) -> None
 ```
 
 Multi-dimensional arrays:
 
 ```python
-replace_content(self, array: Sequence,
+replace_content(self, content: Sequence,
                       offset: tuple[int,...]|list[int]|int = 0) -> None
 ```
 
+Note, that `content` has been called  `array` in a previous version, but
+it has been deprecated by now. It will be removed in a later version.
+
+### Changing array size
+
+Thera are three methods, which can be used to resize/reshape the array:
+
+- [`trim`](#trim)
+- [`shrink_by`](#shrink_by)
+- [`crop_to`](#crop_to)
+
+These are described below.
+
+#### `trim`
+
+```python
+def trim(self) -> None
+```
+
+The method  can be  used to  cut off redundant  parts, i.e.  those where
+default values are  not followed by others. In such  a case, after trim,
+the array returns the same values at all positions as before (of course,
+other properties, such as boundary, may change).
+
+### `shrink_by`
+
+```python
+def shrink_by(self, by: int) -> None
+# dim >= 2:
+def shrink_by(self, by: tuple[int, ...]) -> None
+def shrink_by(self, by: tuple[tuple[int, int], ...]) -> None
+# dim = 1:
+def shrink_by(self, by: tuple[int, int]) -> None
+```
+
+The  method  can  be used  to  reduce  the  size  of the  array  in  all
+directions.  This can  lose  significant  data, but  if  there are  only
+default  values within  the specified  amount in  each directions,  only
+those values will  be deleted and the array will  not change in content.
+Of course, in all cases the the boundary's values will be reduced by the
+amount(s) of `by` (they will not exceed 0).
+
+If `by`  is of type `int`,  the array is  reduced by the same  amount in
+each direction. If  the type is a `tuple`, then  the amount of reduction
+along each axis in each direction must be given. In all cases the amount
+must be greater than or equal to zero.
+
+#### `crop_to`
+
+```python
+# dim >= 2:
+def crop_to(self, by: tuple[tuple[int, int], ...]) -> None
+# dim = 1:
+def crop_to(self, by: tuple[int, int]) -> None
+```
+
+The method can be used to cut  the array to any size in either direction
+in either dimension. Subject, of course, to the restriction that the two
+boundaries cannot  extend past the  zero point, i.e. the  lower boundary
+cannot be positive and the upper boundary cannot be negative.
+
 ### Iterating over the array
 
 Stretchy  arrays are  iterable.  This  means, that  you  can  use it  as
 follows:
 
 ```python
 import stretchy
@@ -613,18 +686,14 @@
 print(f'{array:s}')
 ```
 
 ## Future plans
 
 There are some ideas for future development:
 
-- **arbitrary  croping**:  Cut  to specified  size,  increase/shrink  by
-  amount (`int`) or reshape to boundaries
-- **normalization**:  Cut off  the default values  at the  boundaries to
-  prevent unnecessary storage
 - **offset  shifting**: Offset  an existing  array without  changing the
   contents. Also, offset to center.
 - **non-zero centric operation**: Do not require storage starting from 0
   if all elements are in the positive or negative range.
 - **sub-sub-planes**:  with  partial indexing  you  can  get plane  from
   any  levels. E.g.  in a  4-dimensional array,  `array[2,5]` returns  a
   2-dimensional one
```

