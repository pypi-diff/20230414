# Comparing `tmp/parselib-0.0.4.tar.gz` & `tmp/parselib-0.0.5.tar.gz`

## Comparing `parselib-0.0.4.tar` & `parselib-0.0.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 parselib-0.0.4/src/parselib/__init__.py
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 parselib-0.0.4/src/parselib/element.py
--rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 parselib-0.0.4/src/parselib/finder.py
--rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 parselib-0.0.4/src/parselib/parser.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 parselib-0.0.4/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 parselib-0.0.4/LICENSE
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 parselib-0.0.4/README.rst
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 parselib-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 parselib-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 parselib-0.0.5/src/parselib/__init__.py
+-rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 parselib-0.0.5/src/parselib/element.py
+-rw-r--r--   0        0        0     2372 2020-02-02 00:00:00.000000 parselib-0.0.5/src/parselib/finder.py
+-rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 parselib-0.0.5/src/parselib/parser.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 parselib-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 parselib-0.0.5/LICENSE
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 parselib-0.0.5/README.md
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 parselib-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 parselib-0.0.5/PKG-INFO
```

### Comparing `parselib-0.0.4/src/parselib/element.py` & `parselib-0.0.5/src/parselib/element.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,52 +5,75 @@
 
 class HTMLElement():
     def __init__(self,
                  tagname: str,
                  closed: bool = False,
                  attrs=None,
                  text: str = "",
-                 _all_text=[],
                  descendants=[],
-                 _children=[],
                  parent=None,
                  previous_sibling=None,
-                 next_sibling=None
+                 next_sibling=None,
+                 _all_text=[],
+                 _children=[]
                  ):
         self.tagname = tagname
+        self.closed = closed
         self.attrs = attrs
         self.text = text
-        self._all_text = _all_text
-        self.closed = closed
         self.descendants = descendants
-        self._children = _children
         self.parent = parent
         self.previous_sibling = previous_sibling
         self.next_sibling = next_sibling
+        self._all_text = _all_text
+        self._children = _children
 
     def __repr__(self) -> str:
         return f"{self.tagname.upper()} attrs={self.attrs} text={self.text}"
 
     def find_all(self, tag: str, attrs: Optional[Dict[str, str | None]] = None, exclude_attrs: Optional[Dict[str, List[str | None]]] = None):
         """Return all matching elements"""
         return _find_all(self.descendants, tag, attrs, exclude_attrs)
 
     def find(self, tag: str, attrs: Optional[Dict[str, str | None]] = None, exclude_attrs: Optional[Dict[str, List[str | None]]] = None):
         """Return first matching element"""
         return _find(self.descendants, tag, attrs, exclude_attrs)
 
     @property
-    def children(self):
+    def children(self) -> List:
         """Return elements one level down"""
-        self._children.reverse()
-        return self._children
+        return reversed(self._children)
 
     @property
     def all_text(self) -> str:
         """Return all text within element"""
         res = ""
         for text_or_obj in self._all_text:
             if type(text_or_obj) == str:
                 res += text_or_obj
                 continue
             res += text_or_obj.all_text
         return res
+
+    @property
+    def previous_siblings(self):
+        """Generate previous elements on the same level"""
+        prev = self.previous_sibling
+        while prev:
+            yield prev
+            prev = prev.previous_sibling
+
+    @property
+    def next_siblings(self):
+        """Generate next elements on the same level"""
+        nxt = self.next_sibling
+        while nxt:
+            yield nxt
+            nxt = nxt.next_sibling
+
+    @property
+    def ancestors(self):
+        """Generate all elements within element"""
+        parent = self.parent
+        while parent:
+            yield parent
+            parent = parent.parent
```

### Comparing `parselib-0.0.4/src/parselib/finder.py` & `parselib-0.0.5/src/parselib/finder.py`

 * *Files identical despite different names*

### Comparing `parselib-0.0.4/src/parselib/parser.py` & `parselib-0.0.5/src/parselib/parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,36 +24,37 @@
     def handle_starttag(self, tag: str, attrs) -> None:
         new_element = HTMLElement(tag, attrs=dict(attrs))
         if self.elements:
             new_element.parent = self.current_element
             self.current_element._all_text = self.current_element._all_text + [new_element]
         if self.previous_element.closed:
             self.previous_element.next_sibling = new_element
+            new_element.previous_sibling = self.previous_element
         self.current_element = new_element
         self.elements.append(self.current_element)
         if tag in SELF_CLOSING_TAGS:
             self.current_element.closed = True
 
     def handle_endtag(self, tag: str) -> None:
         self.current_element.descendants = self.elements[self.elements.index(self.current_element) + 1:]
         self.current_element.closed = True
         self.previous_element = self.current_element
-        ind = self.elements.index(self.current_element)
+        ind = self.elements.index(self.current_element) - 1
         children = []
         children.append(self.current_element)
-        while ind > 0:
-            ind -= 1
+        while ind >= 0:
             prev_element = self.elements[ind]
             if prev_element.closed:
                 children.append(prev_element)
-                self.current_element.previous_sibling = prev_element
             else:
                 self.current_element = prev_element
                 self.current_element._children = children
+                self.current_element.descendants = self.elements[ind + 1:]
                 return
+            ind -= 1
 
     def handle_data(self, data: str) -> None:
         data = data.strip()
         self.current_element.text += data
         self.current_element._all_text = self.current_element._all_text + [data]
 
     def find_all(self, tag: str, attrs: Optional[Dict[str, str | None]] = None, exclude_attrs: Optional[Dict[str, List[str | None]]] = None) -> List[HTMLElement]:
```

### Comparing `parselib-0.0.4/LICENSE` & `parselib-0.0.5/LICENSE`

 * *Files identical despite different names*

