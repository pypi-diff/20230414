# Comparing `tmp/tarjan-0.2.3.2.tar.gz` & `tmp/tarjan-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tarjan-0.2.3.2.tar", last modified: Wed Dec 28 10:56:29 2016, max compression
+gzip compressed data, was "tarjan-0.2.4.tar", last modified: Fri Apr 14 08:36:34 2023, max compression
```

## Comparing `tarjan-0.2.3.2.tar` & `tarjan-0.2.4.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 bas        (501) staff       (20)        0 2016-12-28 10:56:29.000000 tarjan-0.2.3.2/
--rw-r--r--   0 bas        (501) staff       (20)      408 2016-12-28 10:56:28.000000 tarjan-0.2.3.2/CHANGES.rst
--rw-r--r--   0 bas        (501) staff       (20)       39 2016-12-28 10:56:28.000000 tarjan-0.2.3.2/MANIFEST.in
--rw-r--r--   0 bas        (501) staff       (20)     4069 2016-12-28 10:56:29.000000 tarjan-0.2.3.2/PKG-INFO
--rw-r--r--   0 bas        (501) staff       (20)     2071 2016-12-28 10:56:28.000000 tarjan-0.2.3.2/README.rst
--rw-r--r--   0 bas        (501) staff       (20)       59 2016-12-28 10:56:29.000000 tarjan-0.2.3.2/setup.cfg
--rw-r--r--   0 bas        (501) staff       (20)     1092 2016-12-28 10:56:28.000000 tarjan-0.2.3.2/setup.py
-drwxr-xr-x   0 bas        (501) staff       (20)        0 2016-12-28 10:56:29.000000 tarjan-0.2.3.2/src/
--rw-r--r--   0 bas        (501) staff       (20)     5523 2016-12-28 10:56:28.000000 tarjan-0.2.3.2/src/__init__.py
--rw-r--r--   0 bas        (501) staff       (20)      639 2016-12-28 10:56:28.000000 tarjan-0.2.3.2/src/tc.py
-drwxr-xr-x   0 bas        (501) staff       (20)        0 2016-12-28 10:56:29.000000 tarjan-0.2.3.2/src/tests/
--rw-r--r--   0 bas        (501) staff       (20)        0 2016-12-28 10:56:28.000000 tarjan-0.2.3.2/src/tests/__init__.py
--rw-r--r--   0 bas        (501) staff       (20)      604 2016-12-28 10:56:28.000000 tarjan-0.2.3.2/src/tests/test_tarjan.py
--rw-r--r--   0 bas        (501) staff       (20)      897 2016-12-28 10:56:28.000000 tarjan-0.2.3.2/src/tests/test_tc.py
-drwxr-xr-x   0 bas        (501) staff       (20)        0 2016-12-28 10:56:29.000000 tarjan-0.2.3.2/tarjan.egg-info/
--rw-r--r--   0 bas        (501) staff       (20)        1 2016-12-28 10:56:29.000000 tarjan-0.2.3.2/tarjan.egg-info/dependency_links.txt
--rw-r--r--   0 bas        (501) staff       (20)     4069 2016-12-28 10:56:29.000000 tarjan-0.2.3.2/tarjan.egg-info/PKG-INFO
--rw-r--r--   0 bas        (501) staff       (20)      282 2016-12-28 10:56:29.000000 tarjan-0.2.3.2/tarjan.egg-info/SOURCES.txt
--rw-r--r--   0 bas        (501) staff       (20)        7 2016-12-28 10:56:29.000000 tarjan-0.2.3.2/tarjan.egg-info/top_level.txt
--rw-r--r--   0 bas        (501) staff       (20)        1 2016-12-28 10:56:29.000000 tarjan-0.2.3.2/tarjan.egg-info/zip-safe
+drwxr-xr-x   0 bas        (501) staff       (20)        0 2023-04-14 08:36:34.298114 tarjan-0.2.4/
+-rw-r--r--   0 bas        (501) staff       (20)      593 2023-04-14 08:36:34.000000 tarjan-0.2.4/CHANGES.rst
+-rw-r--r--   0 bas        (501) staff       (20)     7652 2023-04-14 08:36:34.000000 tarjan-0.2.4/LICENSE
+-rw-r--r--   0 bas        (501) staff       (20)       39 2023-04-14 08:36:34.000000 tarjan-0.2.4/MANIFEST.in
+-rw-r--r--   0 bas        (501) staff       (20)     3336 2023-04-14 08:36:34.298009 tarjan-0.2.4/PKG-INFO
+-rw-r--r--   0 bas        (501) staff       (20)     2103 2023-04-14 08:36:34.000000 tarjan-0.2.4/README.rst
+-rw-r--r--   0 bas        (501) staff       (20)       38 2023-04-14 08:36:34.298143 tarjan-0.2.4/setup.cfg
+-rw-r--r--   0 bas        (501) staff       (20)      961 2023-04-14 08:36:34.000000 tarjan-0.2.4/setup.py
+drwxr-xr-x   0 bas        (501) staff       (20)        0 2023-04-14 08:36:34.297038 tarjan-0.2.4/tarjan/
+-rw-r--r--   0 bas        (501) staff       (20)     4023 2023-04-14 08:36:34.000000 tarjan-0.2.4/tarjan/__init__.py
+-rw-r--r--   0 bas        (501) staff       (20)      495 2023-04-14 08:36:34.000000 tarjan-0.2.4/tarjan/tc.py
+drwxr-xr-x   0 bas        (501) staff       (20)        0 2023-04-14 08:36:34.297863 tarjan-0.2.4/tarjan/tests/
+-rw-r--r--   0 bas        (501) staff       (20)        0 2023-04-14 08:36:34.000000 tarjan-0.2.4/tarjan/tests/__init__.py
+-rw-r--r--   0 bas        (501) staff       (20)      706 2023-04-14 08:36:34.000000 tarjan-0.2.4/tarjan/tests/test_tarjan.py
+-rw-r--r--   0 bas        (501) staff       (20)      983 2023-04-14 08:36:34.000000 tarjan-0.2.4/tarjan/tests/test_tc.py
+drwxr-xr-x   0 bas        (501) staff       (20)        0 2023-04-14 08:36:34.297560 tarjan-0.2.4/tarjan.egg-info/
+-rw-r--r--   0 bas        (501) staff       (20)     3336 2023-04-14 08:36:34.000000 tarjan-0.2.4/tarjan.egg-info/PKG-INFO
+-rw-r--r--   0 bas        (501) staff       (20)      305 2023-04-14 08:36:34.000000 tarjan-0.2.4/tarjan.egg-info/SOURCES.txt
+-rw-r--r--   0 bas        (501) staff       (20)        1 2023-04-14 08:36:34.000000 tarjan-0.2.4/tarjan.egg-info/dependency_links.txt
+-rw-r--r--   0 bas        (501) staff       (20)        7 2023-04-14 08:36:34.000000 tarjan-0.2.4/tarjan.egg-info/top_level.txt
+-rw-r--r--   0 bas        (501) staff       (20)        1 2023-04-14 08:36:34.000000 tarjan-0.2.4/tarjan.egg-info/zip-safe
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tarjan-0.2.3.2/README.rst` & `tarjan-0.2.4/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 is a graph that contains the same vertices and contains an edge from *v*
 to *w* if and only if there is a path from *v* to *w* in *G*.)
 
 The transitive closure is implemented in `tarjan.tc`:
 
 .. code::
 
+    >>> from tarjan.tc import tc
     >>> tc({1:[2],2:[1,5],3:[4],4:[3,5],5:[6],6:[7],7:[8],8:[6,9],9:[]})
     {1: (1, 2, 5, 6, 7, 8, 9),
      2: (1, 2, 5, 6, 7, 8, 9),
      3: (3, 4, 5, 6, 7, 8, 9),
      4: (3, 4, 5, 6, 7, 8, 9),
      5: (8, 9, 6, 7),
      6: (8, 9, 6, 7),
@@ -59,15 +60,15 @@
 
 Installation
 ------------
 Simply execute
 
 .. code::
 
-    easy_install tarjan
+    pip install tarjan
 
 or from this source distribution, run
 
 .. code::
 
     python setup.py install
```

### Comparing `tarjan-0.2.3.2/src/__init__.py` & `tarjan-0.2.4/tarjan/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,150 +1,141 @@
 from collections import namedtuple
 
-__all__ = ['tarjan',
-           'tarjan_iter',
-           'tarjan_recursive']
+__all__ = ["tarjan", "tarjan_iter", "tarjan_recursive"]
 
 """ Context used to implement the algorithm without recursion in @tarjan
     and @tarjan_iter """
-TarjanContext = namedtuple('TarjanContext',
-                                ['g',           # the graph
-                                 'S',           # The main stack of the alg.
-                                 'S_set',       # == set(S) for performance
-                                 'index',       # { v : <index of v> }
-                                 'lowlink',     # { v : <lowlink of v> }
-                                 'T',           # stack to replace recursion
-                                 'ret'])        # return code
+TarjanContext = namedtuple(
+    "TarjanContext",
+    [
+        "g",  # the graph
+        "S",  # The main stack of the alg.
+        "S_set",  # == set(S) for performance
+        "index",  # { v : <index of v> }
+        "lowlink",  # { v : <lowlink of v> }
+        "T",  # stack to replace recursion
+        "ret",
+    ],
+)  # return code
+
 
 def _tarjan_head(ctx, v):
-        """ Used by @tarjan and @tarjan_iter.  This is the head of the
-            main iteration """
-        ctx.index[v] = len(ctx.index)
-        ctx.lowlink[v] = ctx.index[v]
-        ctx.S.append(v)
-        ctx.S_set.add(v)
-        it = iter(ctx.g.get(v, ()))
-        ctx.T.append((it,False,v,None))
+    """Used by @tarjan and @tarjan_iter.  This is the head of the
+    main iteration"""
+    ctx.index[v] = len(ctx.index)
+    ctx.lowlink[v] = ctx.index[v]
+    ctx.S.append(v)
+    ctx.S_set.add(v)
+    it = iter(ctx.g.get(v, ()))
+    ctx.T.append((it, False, v, None))
+
 
 def _tarjan_body(ctx, it, v):
-        """ Used by @tarjan and @tarjan_iter.  This is the body of the
-            main iteration """
-        for w in it:
-                if w not in ctx.index:
-                        ctx.T.append((it,True,v,w))
-                        _tarjan_head(ctx, w)
-                        return
-                if w in ctx.S_set:
-                        ctx.lowlink[v] = min(ctx.lowlink[v], ctx.index[w])
-        if ctx.lowlink[v] == ctx.index[v]:
-                scc = []
-                w = None
-                while v != w:
-                        w = ctx.S.pop()
-                        scc.append(w)
-                        ctx.S_set.remove(w)
-                ctx.ret.append(scc)
+    """Used by @tarjan and @tarjan_iter.  This is the body of the
+    main iteration"""
+    for w in it:
+        if w not in ctx.index:
+            ctx.T.append((it, True, v, w))
+            _tarjan_head(ctx, w)
+            return
+        if w in ctx.S_set:
+            ctx.lowlink[v] = min(ctx.lowlink[v], ctx.index[w])
+    if ctx.lowlink[v] == ctx.index[v]:
+        scc = []
+        w = None
+        while v != w:
+            w = ctx.S.pop()
+            scc.append(w)
+            ctx.S_set.remove(w)
+        ctx.ret.append(scc)
+
 
 def tarjan_iter(g):
-        """ Returns the strongly connected components of the graph @g
-            in a topological order.
+    """Returns the strongly connected components of the graph @g
+    in a topological order.
+
+        @g is the graph represented as a dictionary
+                { <vertex> : <successors of vertex> }.
 
-                @g is the graph represented as a dictionary
-                        { <vertex> : <successors of vertex> }.
+    This function does not recurse.  It returns an iterator."""
+    ctx = TarjanContext(g=g, S=[], S_set=set(), index={}, lowlink={}, T=[], ret=[])
+    main_iter = iter(g)
+    while True:
+        try:
+            v = next(main_iter)
+        except StopIteration:
+            return
+        if v not in ctx.index:
+            _tarjan_head(ctx, v)
+        while ctx.T:
+            it, inside, v, w = ctx.T.pop()
+            if inside:
+                ctx.lowlink[v] = min(ctx.lowlink[w], ctx.lowlink[v])
+            _tarjan_body(ctx, it, v)
+            if ctx.ret:
+                assert len(ctx.ret) == 1
+                yield ctx.ret.pop()
 
-            This function does not recurse.  It returns an iterator. """
-        ctx = TarjanContext(
-                g = g,
-                S = [],
-                S_set = set(),
-                index = {},
-                lowlink = {},
-                T = [],
-                ret = [])
-        main_iter = iter(g)
-        while True:
-                try:
-                        v = next(main_iter)
-                except StopIteration:
-                        return
-                if v not in ctx.index:
-                        _tarjan_head(ctx, v)
-                while ctx.T:
-                        it, inside, v, w = ctx.T.pop()
-                        if inside:
-                                ctx.lowlink[v] = min(ctx.lowlink[w],
-                                                        ctx.lowlink[v])
-                        _tarjan_body(ctx, it, v)
-                        if ctx.ret:
-                                assert len(ctx.ret) == 1
-                                yield ctx.ret.pop()
 
 def tarjan(g):
-        """ Returns the strongly connected components of the graph @g
-            in a topological order.
+    """Returns the strongly connected components of the graph @g
+    in a topological order.
+
+        @g is the graph represented as a dictionary
+                { <vertex> : <successors of vertex> }.
+
+    This function does not recurse."""
+    ctx = TarjanContext(g=g, S=[], S_set=set(), index={}, lowlink={}, T=[], ret=[])
+    main_iter = iter(g)
+    while True:
+        try:
+            v = next(main_iter)
+        except StopIteration:
+            return ctx.ret
+        if v not in ctx.index:
+            _tarjan_head(ctx, v)
+        while ctx.T:
+            it, inside, v, w = ctx.T.pop()
+            if inside:
+                ctx.lowlink[v] = min(ctx.lowlink[w], ctx.lowlink[v])
+            _tarjan_body(ctx, it, v)
 
-                @g is the graph represented as a dictionary
-                        { <vertex> : <successors of vertex> }.
-        
-            This function does not recurse. """
-        ctx = TarjanContext(
-                g = g,
-                S = [],
-                S_set = set(),
-                index = {},
-                lowlink = {},
-                T = [],
-                ret = [])
-        main_iter = iter(g)
-        while True:
-                try:
-                        v = next(main_iter)
-                except StopIteration:
-                        return ctx.ret
-                if v not in ctx.index:
-                        _tarjan_head(ctx, v)
-                while ctx.T:
-                        it, inside, v, w = ctx.T.pop()
-                        if inside:
-                                ctx.lowlink[v] = min(ctx.lowlink[w],
-                                                        ctx.lowlink[v])
-                        _tarjan_body(ctx, it, v)
 
 def tarjan_recursive(g):
-        """ Returns the strongly connected components of the graph @g
-            in a topological order.
+    """Returns the strongly connected components of the graph @g
+    in a topological order.
+
+        @g is the graph represented as a dictionary
+                { <vertex> : <successors of vertex> }.
 
-                @g is the graph represented as a dictionary
-                        { <vertex> : <successors of vertex> }.
-                        
-            This function recurses --- large graphs may cause a stack
-            overflow. """
-        S = []
-        S_set = set()
-        index = {}
-        lowlink = {}
-        ret = []
-
-        def visit(v):
-                index[v] = len(index)
-                lowlink[v] = index[v]
-                S.append(v)
-                S_set.add(v)
-                for w in g.get(v,()):
-                        if w not in index:
-                                visit(w)
-                                lowlink[v] = min(lowlink[w], lowlink[v])
-                        elif w in S_set:
-                                lowlink[v] = min(lowlink[v], index[w])
-                if lowlink[v] == index[v]:
-                        scc = []
-                        w = None
-                        while v != w:
-                                w = S.pop()
-                                scc.append(w)
-                                S_set.remove(w)
-                        ret.append(scc)
-
-        for v in g:
-                if not v in index:
-                        visit(v)
-        return ret
+    This function recurses --- large graphs may cause a stack
+    overflow."""
+    S = []
+    S_set = set()
+    index = {}
+    lowlink = {}
+    ret = []
+
+    def visit(v):
+        index[v] = len(index)
+        lowlink[v] = index[v]
+        S.append(v)
+        S_set.add(v)
+        for w in g.get(v, ()):
+            if w not in index:
+                visit(w)
+                lowlink[v] = min(lowlink[w], lowlink[v])
+            elif w in S_set:
+                lowlink[v] = min(lowlink[v], index[w])
+        if lowlink[v] == index[v]:
+            scc = []
+            w = None
+            while v != w:
+                w = S.pop()
+                scc.append(w)
+                S_set.remove(w)
+            ret.append(scc)
+
+    for v in g:
+        if v not in index:
+            visit(v)
+    return ret
```

### Comparing `tarjan-0.2.3.2/src/tests/test_tc.py` & `tarjan-0.2.4/tarjan/tests/test_tc.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,38 @@
 import unittest
 import tarjan.tc
 
+
 class TestMain(unittest.TestCase):
     def test_mainExample(self):
         # see doc/example.png
-        g = {1:[2],2:[1,5],3:[4],4:[3,5], 5:[6],6:[7],7:[8],8:[6,9],9:[]}
+        g = {
+            1: [2],
+            2: [1, 5],
+            3: [4],
+            4: [3, 5],
+            5: [6],
+            6: [7],
+            7: [8],
+            8: [6, 9],
+            9: [],
+        }
         res = tarjan.tc.tc(g)
         res = dict([(k, frozenset(res[k])) for k in res])
-        self.assertEqual(res, {1: frozenset([1, 2, 5, 6, 7, 8, 9]),
-                               2: frozenset([1, 2, 5, 6, 7, 8, 9]),
-                               3: frozenset([3, 4, 5, 6, 7, 8, 9]),
-                               4: frozenset([3, 4, 5, 6, 7, 8, 9]),
-                               5: frozenset([8, 9, 6, 7]),
-                               6: frozenset([8, 9, 6, 7]),
-                               7: frozenset([8, 9, 6, 7]),
-                               8: frozenset([8, 9, 6, 7]),
-                               9: frozenset()})
+        self.assertEqual(
+            res,
+            {
+                1: frozenset([1, 2, 5, 6, 7, 8, 9]),
+                2: frozenset([1, 2, 5, 6, 7, 8, 9]),
+                3: frozenset([3, 4, 5, 6, 7, 8, 9]),
+                4: frozenset([3, 4, 5, 6, 7, 8, 9]),
+                5: frozenset([8, 9, 6, 7]),
+                6: frozenset([8, 9, 6, 7]),
+                7: frozenset([8, 9, 6, 7]),
+                8: frozenset([8, 9, 6, 7]),
+                9: frozenset(),
+            },
+        )
+
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

