# Comparing `tmp/tklinenums-1.6.2.tar.gz` & `tmp/tklinenums-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tklinenums-1.6.2.tar", last modified: Sun Apr  9 19:25:24 2023, max compression
+gzip compressed data, was "tklinenums-1.6.3.tar", last modified: Fri Apr 14 01:18:46 2023, max compression
```

## Comparing `tklinenums-1.6.2.tar` & `tklinenums-1.6.3.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 joshyacktman   (501) staff       (20)        0 2023-04-09 19:25:24.830981 tklinenums-1.6.2/
--rw-r--r--   0 joshyacktman   (501) staff       (20)      862 2023-04-09 19:25:24.830712 tklinenums-1.6.2/PKG-INFO
--rw-r--r--   0 joshyacktman   (501) staff       (20)      606 2023-04-09 19:24:42.000000 tklinenums-1.6.2/README.md
--rw-r--r--   0 joshyacktman   (501) staff       (20)       38 2023-04-09 19:25:24.831045 tklinenums-1.6.2/setup.cfg
--rw-r--r--   0 joshyacktman   (501) staff       (20)      461 2023-04-09 19:24:49.000000 tklinenums-1.6.2/setup.py
-drwxr-xr-x   0 joshyacktman   (501) staff       (20)        0 2023-04-09 19:25:24.828739 tklinenums-1.6.2/tklinenums/
--rw-r--r--   0 joshyacktman   (501) staff       (20)       38 2023-04-07 18:10:10.000000 tklinenums-1.6.2/tklinenums/__init__.py
--rw-r--r--   0 joshyacktman   (501) staff       (20)    10056 2023-04-09 19:21:06.000000 tklinenums-1.6.2/tklinenums/tklinenums.py
-drwxr-xr-x   0 joshyacktman   (501) staff       (20)        0 2023-04-09 19:25:24.830368 tklinenums-1.6.2/tklinenums.egg-info/
--rw-r--r--   0 joshyacktman   (501) staff       (20)      862 2023-04-09 19:25:24.000000 tklinenums-1.6.2/tklinenums.egg-info/PKG-INFO
--rw-r--r--   0 joshyacktman   (501) staff       (20)      202 2023-04-09 19:25:24.000000 tklinenums-1.6.2/tklinenums.egg-info/SOURCES.txt
--rw-r--r--   0 joshyacktman   (501) staff       (20)        1 2023-04-09 19:25:24.000000 tklinenums-1.6.2/tklinenums.egg-info/dependency_links.txt
--rw-r--r--   0 joshyacktman   (501) staff       (20)       11 2023-04-09 19:25:24.000000 tklinenums-1.6.2/tklinenums.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:18:46.815963 tklinenums-1.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-14 01:18:46.815963 tklinenums-1.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-14 01:18:31.000000 tklinenums-1.6.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-14 01:18:31.000000 tklinenums-1.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 01:18:46.815963 tklinenums-1.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-14 01:18:31.000000 tklinenums-1.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:18:46.811963 tklinenums-1.6.3/tklinenums/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 01:18:31.000000 tklinenums-1.6.3/tklinenums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10212 2023-04-14 01:18:31.000000 tklinenums-1.6.3/tklinenums/tklinenums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 01:18:46.815963 tklinenums-1.6.3/tklinenums.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-14 01:18:46.000000 tklinenums-1.6.3/tklinenums.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-14 01:18:46.000000 tklinenums-1.6.3/tklinenums.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 01:18:46.000000 tklinenums-1.6.3/tklinenums.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-14 01:18:46.000000 tklinenums-1.6.3/tklinenums.egg-info/top_level.txt
```

### Comparing `tklinenums-1.6.2/PKG-INFO` & `tklinenums-1.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: tklinenums
-Version: 1.6.2
+Version: 1.6.3
 Summary: A simple Tkinter widget for displaying line numbers
 Home-page: https://github.com/Moosems/TkLineNums
 Author: Moosems
 Author-email: moosems.j@gmail.com
 Description-Content-Type: text/markdown
 
-# TkLineNums V.1.6.2
+# TkLineNums V.1.6.3
 
 TkLineNums is a simple line numbering widget for Tkinter. It supports ttk themes through the set_to_ttk_style method.
 
 ![img](https://github.com/Moosems/TkLineNums/raw/main/images/TkLineNumsPhoto.png)
 
 ## Features
```

### Comparing `tklinenums-1.6.2/README.md` & `tklinenums-1.6.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# TkLineNums V.1.6.2
+# TkLineNums V.1.6.3
 
 TkLineNums is a simple line numbering widget for Tkinter. It supports ttk themes through the set_to_ttk_style method.
 
 ![img](https://github.com/Moosems/TkLineNums/raw/main/images/TkLineNumsPhoto.png)
 
 ## Features
```

### Comparing `tklinenums-1.6.2/tklinenums/tklinenums.py` & `tklinenums-1.6.3/tklinenums/tklinenums.py`

 * *Files 12% similar despite different names*

```diff
@@ -41,32 +41,32 @@
         """Initializes the widget -- Internal use only"""
         self.textwidget = editor
         self.master = master
         self.justify = justify
         Canvas.__init__(
             self,
             master,
-            width=40 if kwargs.get("width") is None else kwargs.get("width"),
-            highlightthickness=0
-            if kwargs.get("highlightthickness") is None
-            else kwargs.get("highlightthickness"),
-            borderwidth=2
-            if kwargs.get("borderwidth") is None
-            else kwargs.get("borderwidth"),
-            relief="ridge" if kwargs.get("relief") is None else kwargs.get("relief"),
+            width=kwargs.get("width", 40),
+            highlightthickness=kwargs.get("highlightthickness", 0),
+            borderwidth=kwargs.get("borderwidth", 2),
+            relief=kwargs.get("relief", "ridge"),
             *args,
             **kwargs,
         )
         self.set_to_ttk_style()
 
         self.bind("<MouseWheel>", self.mouse_scroll, add=True)
+        # If I'm mouse scrolling and I am clicking on line numbers, it should select the lines from where I clicked to where I am scrolling
+        # TODO: Make it so that it selects the lines from where I clicked to where I am scrolling
+        # Not a feauture in VS Code
         self.bind("<Button-1>", self.click_see, add=True)
         self.bind("<ButtonRelease-1>", self.unclick, add=True)
         self.bind("<Double-Button-1>", self.double_click, add=True)
         self.bind("<Button1-Motion>", self.drag, add=True)
+        self.bind("<Button1-Leave>", self.auto_scroll, add=True)
 
         self.click_pos: None = None
 
     def redraw(self, *args) -> None:
         """Redraws the widget"""
         self.resize()
         self.delete("all")
@@ -90,118 +90,112 @@
             )
 
     def mouse_scroll(self, event: Event) -> None:
         """Scrolls the text widget when the mouse wheel is scrolled -- Internal use only"""
         if system == "Darwin":
             self.textwidget.yview_scroll(scroll_inversion * event.delta, "units")
         else:
-            self.textwidget.yview_scroll(
-                int(scroll_inversion * (event.delta / 120)), "units"
-            )
+            self.textwidget.yview_scroll(int(scroll_inversion * (event.delta / 120)), "units")
         self.redraw()
 
     def click_see(self, event: Event) -> None:
         """When clicking on a line number it scrolls to that line if not shifting -- Internal use only"""
         if event.state == 1:
             self.shift_click(event)
             return
         self.textwidget.tag_remove("sel", "1.0", "end")
         self.textwidget.mark_set(
             "insert",
             f"{self.textwidget.index(f'@{event.x},{event.y}').split('.')[0]}.0",
         )
         self.textwidget.see("insert")
-        first_visible_line, last_visible_line = int(
-            self.textwidget.index("@0,0").split(".")[0]
-        ), int(
+        first_visible_line, last_visible_line = int(self.textwidget.index("@0,0").split(".")[0]), int(
             self.textwidget.index(f"@0,{self.textwidget.winfo_height()}").split(".")[0]
         )
-        if (
-            insert := int(self.textwidget.index("insert").split(".")[0])
-        ) == first_visible_line:
+        if (insert := int(self.textwidget.index("insert").split(".")[0])) == first_visible_line:
             self.textwidget.yview_scroll(-1, "units")
         elif insert == last_visible_line:
             self.textwidget.yview_scroll(1, "units")
         self.click_pos = self.textwidget.index("insert")
 
     def unclick(self, event: Event) -> None:
         """When the mouse button is released it removes the selection -- Internal use only"""
         self.click_pos: None = None
 
     def double_click(self, event: Event) -> None:
         """Selects the line when double clicked -- Internal use only"""
         self.textwidget.tag_remove("sel", "1.0", "end")
         self.textwidget.tag_add("sel", "insert", "insert + 1 line")
 
+    def auto_scroll(self, event: Event) -> None:
+        """Automatically scrolls the text widget when the mouse is near the top or bottom, similar to the drag function -- Internal use only"""
+        if self.click_pos is None:
+            return
+        if event.y >= self.winfo_height():
+            self.textwidget.yview_scroll(1 if system == "Darwin" else (1 / 120), "units")
+        elif event.y < 0:
+            self.textwidget.yview_scroll(-1 if system == "Darwin" else (-1 / 120), "units")
+        elif event.x >= self.winfo_width():
+            self.textwidget.xview_scroll(2 if system == "Darwin" else (2 / 120), "units")
+        elif event.x < 0:
+            self.textwidget.xview_scroll(-2 if system == "Darwin" else (-2 / 120), "units")
+        else:
+            return
+        start, end = self.textwidget.index("insert"), self.click_pos
+        if self.textwidget.compare("insert", ">", self.click_pos):
+            start, end = end, str(float(start) + 1)
+        else:
+            end = str(float(end) + 1)
+        self.textwidget.tag_remove("sel", "1.0", "end")
+        self.textwidget.tag_add("sel", start, end)
+        self.textwidget.mark_set("insert", f"@{event.x},{event.y}")
+        self.after(50, self.auto_scroll, event)
+
     def drag(self, event: Event) -> None:
         """When click dragging it selects the text -- Internal use only"""
-
-        """
-        Issues:
-         - Once it starts going it's hard to stop drag clicking (because most people pull back up when done but this is still
-           considered dragging and it remembers the direction meaning it will continue to drag in that direction)
-         - When you reach your end point for scroll clicking you can't go back unless you go completely the opposite way which 
-           then means you can't go back the original way
-         - When you go down and then try to go back up you can't
-         - Must continue to drag cursor for it to select more even if cursor is off-screen or trying to slowly select more (Means
-           it might need to become recursive)
-        """  # TODO: Fix issues
-        if self.click_pos is None:
+        if (
+            self.click_pos is None
+            or event.x < 0
+            or event.x >= self.winfo_width()
+            or event.y < 0
+            or event.y >= self.winfo_height()
+        ):
             return
         start, end = self.textwidget.index("insert"), self.click_pos
         if self.textwidget.compare("insert", ">", self.click_pos):
+            start, end = start, str(float(end) + 1)
+
+        if self.textwidget.compare(start, ">", end):
             start, end = end, start
-        self.textwidget.mark_set("insert", f"@0,{event.y}")
         self.textwidget.tag_remove("sel", "1.0", "end")
         self.textwidget.tag_add("sel", start, end)
-        first_line, last_line = (
-            self.textwidget.index("@0,0").split(".")[0],
-            self.textwidget.index(f"@0,{self.textwidget.winfo_height()}").split(".")[0],
-        )
-        if end.split(".")[0] == last_line and event.y > self.winfo_y():
-            self.textwidget.yview_scroll(
-                1, "units"
-            ) if system == "Darwin" else self.textwidget.yview_scroll(
-                (1 / 120), "units"
-            )
-            self.textwidget.tag_add("sel", start, str(float(end) + 1))
-            self.textwidget.mark_set("insert", str(float(end) + 1))
-            return None
-        elif (
-            start.split(".")[0] == first_line
-            and event.y < self.winfo_y() + self.winfo_height()
-        ):
-            self.textwidget.yview_scroll(
-                -1, "units"
-            ) if system == "Darwin" else self.textwidget.yview_scroll(
-                (-1 / 120), "units"
-            )
-            self.textwidget.tag_add("sel", str(float(start) - 1), end)
-            self.textwidget.mark_set("insert", str(float(start) - 1))
-            return None
+        self.textwidget.mark_set("insert", self.textwidget.index(f"@{event.x},{event.y} linestart"))
         self.redraw()
 
+        """
+        Issues:
+         - Once it starts going it's hard to stop drag clicking (because most people pull back up when done but this is still
+           considered dragging and it remembers the direction meaning it will continue to drag in that direction)unless you unclick
+         - Once it goes past the end of the text widget it will continue to drag in that direction until unclicked
+        """  # TODO: Fix issues
+
     def shift_click(self, event: Event) -> None:
         """When shift clicking it selects the text between the click and the cursor -- Internal use only"""
-        start_pos, end_pos = self.textwidget.index("insert"), self.textwidget.index(
-            f"@0,{event.y}"
-        )
+        start_pos, end_pos = self.textwidget.index("insert"), self.textwidget.index(f"@0,{event.y}")
         self.textwidget.tag_remove("sel", "1.0", "end")
         if self.textwidget.compare(start_pos, ">", end_pos):
             start_pos, end_pos = end_pos, start_pos
         self.textwidget.tag_add("sel", start_pos, end_pos)
 
     def resize(self) -> None:
         """Resizes the widget to fit the text widget"""
         end = self.textwidget.index("end").split(".")[0]
-        self.config(
-            width=Font(font=(temp_font := self.textwidget.cget("font"))).measure(
-                " 1234 "
-            )
-        ) if int(end) <= 1000 else self.config(width=temp_font.measure(f" {end} "))
+        self.config(width=Font(font=(temp_font := self.textwidget.cget("font"))).measure(" 1234 ")) if int(
+            end
+        ) <= 1000 else self.config(width=temp_font.measure(f" {end} "))
 
     def set_to_ttk_style(self) -> None:
         """Sets the widget to the ttk style"""
         self["bg"] = self.tk.eval("ttk::style lookup TLineNumbers -background")
         self.foreground = self.tk.eval("ttk::style lookup TLineNumbers -foreground")
 
     def reload(self) -> None:
@@ -236,14 +230,12 @@
         text.insert("end", f"Line {i+1}\n")
 
     linenums = TkLineNumbers(root, text)
     linenums.pack(fill="y", side="left", expand=True)
 
     text.bind("<Key>", lambda event: root.after_idle(linenums.redraw), add=True)
     text.bind(f"<BackSpace>", lambda event: root.after_idle(linenums.redraw), add=True)
-    text.bind(
-        f"<{contmand}-v>", lambda event: root.after_idle(linenums.redraw), add=True
-    )
+    text.bind(f"<{contmand}-v>", lambda event: root.after_idle(linenums.redraw), add=True)
     text["yscrollcommand"] = linenums.redraw
     text.config(font=("Courier New bold", 13))
 
     root.mainloop()
```

### Comparing `tklinenums-1.6.2/tklinenums.egg-info/PKG-INFO` & `tklinenums-1.6.3/tklinenums.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: tklinenums
-Version: 1.6.2
+Version: 1.6.3
 Summary: A simple Tkinter widget for displaying line numbers
 Home-page: https://github.com/Moosems/TkLineNums
 Author: Moosems
 Author-email: moosems.j@gmail.com
 Description-Content-Type: text/markdown
 
-# TkLineNums V.1.6.2
+# TkLineNums V.1.6.3
 
 TkLineNums is a simple line numbering widget for Tkinter. It supports ttk themes through the set_to_ttk_style method.
 
 ![img](https://github.com/Moosems/TkLineNums/raw/main/images/TkLineNumsPhoto.png)
 
 ## Features
```

