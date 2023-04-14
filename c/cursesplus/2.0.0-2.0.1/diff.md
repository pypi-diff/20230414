# Comparing `tmp/cursesplus-2.0.0.tar.gz` & `tmp/cursesplus-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cursesplus-2.0.0.tar", last modified: Fri Apr  7 16:57:03 2023, max compression
+gzip compressed data, was "cursesplus-2.0.1.tar", last modified: Fri Apr 14 17:50:35 2023, max compression
```

## Comparing `cursesplus-2.0.0.tar` & `cursesplus-2.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-04-07 16:57:03.465613 cursesplus-2.0.0/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1089 2023-04-07 16:31:31.000000 cursesplus-2.0.0/LICENSE
--rw-r--r--   0 jordan    (1000) jordan    (1000)     1556 2023-04-07 16:57:03.465613 cursesplus-2.0.0/PKG-INFO
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      953 2023-04-07 16:31:31.000000 cursesplus-2.0.0/README.md
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      659 2023-04-07 16:31:31.000000 cursesplus-2.0.0/pyproject.toml
--rw-r--r--   0 jordan    (1000) jordan    (1000)       38 2023-04-07 16:57:03.465613 cursesplus-2.0.0/setup.cfg
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-04-07 16:57:03.465613 cursesplus-2.0.0/src/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      555 2023-04-07 16:31:31.000000 cursesplus-2.0.0/src/__cptest.py
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-04-07 16:57:03.465613 cursesplus-2.0.0/src/cursesplus/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      892 2023-04-07 16:31:31.000000 cursesplus-2.0.0/src/cursesplus/__init__.py
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)    11516 2023-04-07 16:31:31.000000 cursesplus-2.0.0/src/cursesplus/cp.py
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)    11277 2023-04-07 16:45:57.000000 cursesplus-2.0.0/src/cursesplus/filedialog.py
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     5666 2023-04-07 16:31:31.000000 cursesplus-2.0.0/src/cursesplus/messagebox.py
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-04-07 16:57:03.465613 cursesplus-2.0.0/src/cursesplus.egg-info/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1556 2023-04-07 16:57:03.000000 cursesplus-2.0.0/src/cursesplus.egg-info/PKG-INFO
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      306 2023-04-07 16:57:03.000000 cursesplus-2.0.0/src/cursesplus.egg-info/SOURCES.txt
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)        1 2023-04-07 16:57:03.000000 cursesplus-2.0.0/src/cursesplus.egg-info/dependency_links.txt
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)       20 2023-04-07 16:57:03.000000 cursesplus-2.0.0/src/cursesplus.egg-info/top_level.txt
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-04-14 17:50:35.783825 cursesplus-2.0.1/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1089 2023-04-07 16:31:31.000000 cursesplus-2.0.1/LICENSE
+-rw-r--r--   0 jordan    (1000) jordan    (1000)     1617 2023-04-14 17:50:35.783825 cursesplus-2.0.1/PKG-INFO
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1014 2023-04-14 17:48:06.000000 cursesplus-2.0.1/README.md
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      659 2023-04-14 17:48:12.000000 cursesplus-2.0.1/pyproject.toml
+-rw-r--r--   0 jordan    (1000) jordan    (1000)       38 2023-04-14 17:50:35.783825 cursesplus-2.0.1/setup.cfg
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-04-14 17:50:35.773825 cursesplus-2.0.1/src/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      555 2023-04-07 16:31:31.000000 cursesplus-2.0.1/src/__cptest.py
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-04-14 17:50:35.783825 cursesplus-2.0.1/src/cursesplus/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      892 2023-04-07 16:31:31.000000 cursesplus-2.0.1/src/cursesplus/__init__.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)    11516 2023-04-07 16:31:31.000000 cursesplus-2.0.1/src/cursesplus/cp.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)    11277 2023-04-07 16:45:57.000000 cursesplus-2.0.1/src/cursesplus/filedialog.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     5994 2023-04-14 17:49:51.000000 cursesplus-2.0.1/src/cursesplus/messagebox.py
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-04-14 17:50:35.783825 cursesplus-2.0.1/src/cursesplus.egg-info/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1617 2023-04-14 17:50:35.000000 cursesplus-2.0.1/src/cursesplus.egg-info/PKG-INFO
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      306 2023-04-14 17:50:35.000000 cursesplus-2.0.1/src/cursesplus.egg-info/SOURCES.txt
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)        1 2023-04-14 17:50:35.000000 cursesplus-2.0.1/src/cursesplus.egg-info/dependency_links.txt
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)       20 2023-04-14 17:50:35.000000 cursesplus-2.0.1/src/cursesplus.egg-info/top_level.txt
```

### Comparing `cursesplus-2.0.0/LICENSE` & `cursesplus-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cursesplus-2.0.0/PKG-INFO` & `cursesplus-2.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cursesplus
-Version: 2.0.0
+Version: 2.0.1
 Summary: An extension program to curses that offers option menus, message boxes, file dialogs and more
 Author-email: Enderbyte Programs <enderbyte09@gmail.com>
 Project-URL: Homepage, https://github.com/Enderbyte-Programs/Curses-Plus
 Project-URL: Bug Tracker, https://github.com/Enderbyte-Programs/Curses-Plus/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -36,15 +36,19 @@
 Microsoft Windows 11
 Any modern distro of Linux that supports Python3
 
 **Python Version 3.6 or newer**
 
 ## What's New?
 
-Version 2.0: Incompatible api changes
+### Version 2.0.1
+
+Colour is now optional in messagebox
+
+### Version 2.0: Incompatible api changes
 
 -askyesno now MUST be messagebox.askyesno
 -Rewrite colour system. load_colours() is now nonexistent.
 -Now use set_colour(background,foreground). A set of colour constants are defined in the cp class.
 
 ## Uses
```

### Comparing `cursesplus-2.0.0/README.md` & `cursesplus-2.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,19 @@
 Microsoft Windows 11
 Any modern distro of Linux that supports Python3
 
 **Python Version 3.6 or newer**
 
 ## What's New?
 
-Version 2.0: Incompatible api changes
+### Version 2.0.1
+
+Colour is now optional in messagebox
+
+### Version 2.0: Incompatible api changes
 
 -askyesno now MUST be messagebox.askyesno
 -Rewrite colour system. load_colours() is now nonexistent.
 -Now use set_colour(background,foreground). A set of colour constants are defined in the cp class.
 
 ## Uses
```

### Comparing `cursesplus-2.0.0/pyproject.toml` & `cursesplus-2.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "cursesplus"
-version = "2.0.0"
+version = "2.0.1"
 authors = [{name="Enderbyte Programs",email="enderbyte09@gmail.com"},]
 description = "An extension program to curses that offers option menus, message boxes, file dialogs and more"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
 	"Programming Language :: Python :: 3",
 	"License :: OSI Approved :: MIT License",
```

### Comparing `cursesplus-2.0.0/src/__cptest.py` & `cursesplus-2.0.1/src/__cptest.py`

 * *Files identical despite different names*

### Comparing `cursesplus-2.0.0/src/cursesplus/__init__.py` & `cursesplus-2.0.1/src/cursesplus/__init__.py`

 * *Files identical despite different names*

### Comparing `cursesplus-2.0.0/src/cursesplus/cp.py` & `cursesplus-2.0.1/src/cursesplus/cp.py`

 * *Files identical despite different names*

### Comparing `cursesplus-2.0.0/src/cursesplus/filedialog.py` & `cursesplus-2.0.1/src/cursesplus/filedialog.py`

 * *Files identical despite different names*

### Comparing `cursesplus-2.0.0/src/cursesplus/messagebox.py` & `cursesplus-2.0.1/src/cursesplus/messagebox.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 from . import cp
 import os
 from curses.textpad import rectangle
 import curses
 
-def askyesno(stdscr,message: list = []) -> bool:
+def askyesno(stdscr,message: list = [],colour=False) -> bool:
     """Display a messagebox that asks a user a questions. Returns TRUE on Yes and FALSE on No. Colour is green"""
     selected = True
     x,y = os.get_terminal_size()
     ox = 0
+    if colour:
+        BGCL = cp.GREEN
+    else:
+        BGCL = cp.BLACK
     for o in message:
         ox += 1
         if "\n" in o:
             message.insert(ox,o.split("\n")[1])
     message = [m[0:x-5].split("\n")[0] for m in message[0:y-5]]#Limiting characters
     maxs = max([len(s) for s in message])
     while True:
         for by in range(y//2-(len(message)//2)-1,y//2+(len(message)//2)+4):
             for bx in range(x//2-(maxs//2)-1,x//2+(maxs//2+1)+1):
-                stdscr.addstr(by,bx," ",cp.set_colour(cp.GREEN,cp.WHITE))
+                stdscr.addstr(by,bx," ",cp.set_colour(BGCL,cp.WHITE))
         rectangle(stdscr,y//2-(len(message)//2)-1, x//2-(maxs//2)-1, y//2+(len(message)//2)+4, x//2+(maxs//2+1)+1)
         stdscr.addstr(y//2+(len(message)//2)+4,x//2-(maxs//2),"Y: Yes | N: No")
         mi = -(len(message)/2)
         stdscr.addstr(y//2+(len(message)//2)+3,x//2-(maxs//2),"[Yes]",[cp.set_colour(cp.WHITE,cp.BLACK) if selected else cp.set_colour(cp.BLACK,cp.WHITE)][0])
         stdscr.addstr(y//2+(len(message)//2)+3,x//2-(maxs//2)+10,"[No]",[cp.set_colour(cp.BLACK,cp.WHITE) if selected else cp.set_colour(cp.WHITE,cp.BLACK)][0])   
         for msgl in message:
             mi += 1
@@ -33,87 +37,99 @@
         if ch == curses.KEY_RIGHT or ch == curses.KEY_LEFT:
             selected = not selected
         elif ch == 121 or ch == 110:
             return ch == 121
         elif ch == 10 or ch == 13 or ch == curses.KEY_ENTER:
             return selected
 
-def showinfo(stdscr,message: list = [],title:str="Info") -> None:
+def showinfo(stdscr,message: list = [],title:str="Info",colour=False) -> None:
     """Display a messagebox that shows info to a user. Background BLUE"""
     selected = True
+    if colour:
+        BGCL = cp.BLUE
+    else:
+        BGCL = cp.BLACK
     x,y = os.get_terminal_size()
     ox = 0
     for o in message:
         ox += 1
         if "\n" in o:
             message.insert(ox,o.split("\n")[1])
     message = [m[0:x-5].split("\n")[0] for m in message[0:y-5]]#Limiting characters
     maxs = max([len(s) for s in message])
     while True:
         for by in range(y//2-(len(message)//2)-1,y//2+(len(message)//2)+4):
             for bx in range(x//2-(maxs//2)-1,x//2+(maxs//2+1)+1):
-                stdscr.addstr(by,bx," ",cp.set_colour(cp.BLUE,cp.WHITE))
+                stdscr.addstr(by,bx," ",cp.set_colour(BGCL,cp.WHITE))
         rectangle(stdscr,y//2-(len(message)//2)-1, x//2-(maxs//2)-1, y//2+(len(message)//2)+4, x//2+(maxs//2+1)+1)
         stdscr.addstr(y//2-(len(message)//2)-1, x//2-(maxs//2)-1,title)
         mi = -(len(message)/2)
         stdscr.addstr(y//2+(len(message)//2)+3,x//2-(maxs//2),"[OK]",cp.set_colour(cp.WHITE,cp.BLACK)) 
         for msgl in message:
             mi += 1
             stdscr.addstr(int(y//2+mi),int(x//2-len(msgl)//2),msgl,cp.set_colour(cp.BLUE,cp.WHITE))
     
         stdscr.refresh()
         
         ch = stdscr.getch()
         if ch == 10 or ch == 13 or ch == curses.KEY_ENTER:
             return
 
-def showwarning(stdscr,message: list = [],title:str="Warning") -> None:
+def showwarning(stdscr,message: list = [],title:str="Warning",colour=False) -> None:
     """Display a messagebox that shows a warning to a user. Background YELLOW"""
     selected = True
+    if colour:
+        BGCL = cp.YELLOW
+    else:
+        BGCL = cp.BLACK
     x,y = os.get_terminal_size()
     ox = 0
     for o in message:
         ox += 1
         if "\n" in o:
             message.insert(ox,o.split("\n")[1])
     message = [m[0:x-5].split("\n")[0] for m in message[0:y-5]]#Limiting characters
     maxs = max([len(s) for s in message])
     while True:
         for by in range(y//2-(len(message)//2)-1,y//2+(len(message)//2)+4):
             for bx in range(x//2-(maxs//2)-1,x//2+(maxs//2+1)+1):
-                stdscr.addstr(by,bx," ",cp.set_colour(cp.YELLOW,cp.WHITE))
+                stdscr.addstr(by,bx," ",cp.set_colour(BGCL,cp.WHITE))
         rectangle(stdscr,y//2-(len(message)//2)-1, x//2-(maxs//2)-1, y//2+(len(message)//2)+4, x//2+(maxs//2+1)+1)
         stdscr.addstr(y//2-(len(message)//2)-1, x//2-(maxs//2)-1,title)
         mi = -(len(message)/2)
         stdscr.addstr(y//2+(len(message)//2)+3,x//2-(maxs//2),"[OK]",cp.set_colour(cp.WHITE,cp.BLACK)) 
         for msgl in message:
             mi += 1
             stdscr.addstr(int(y//2+mi),int(x//2-len(msgl)//2),msgl,cp.set_colour(cp.YELLOW,cp.WHITE))
     
         stdscr.refresh()
         
         ch = stdscr.getch()
         if ch == 10 or ch == 13 or ch == curses.KEY_ENTER:
             return
 
-def showerror(stdscr,message: list = [],title:str="Warning") -> None:
+def showerror(stdscr,message: list = [],title:str="Warning",colour=False) -> None:
     """Display a message to a user that shows an error. background red."""
     selected = True
     x,y = os.get_terminal_size()
     ox = 0
+    if colour:
+        BGCL = cp.RED
+    else:
+        BGCL = cp.BLACK
     for o in message:
         ox += 1
         if "\n" in o:
             message.insert(ox,o.split("\n")[1])
     message = [m[0:x-5].split("\n")[0] for m in message[0:y-5]]#Limiting characters
     maxs = max([len(s) for s in message])
     while True:
         for by in range(y//2-(len(message)//2)-1,y//2+(len(message)//2)+4):
             for bx in range(x//2-(maxs//2)-1,x//2+(maxs//2+1)+1):
-                stdscr.addstr(by,bx," ",cp.set_colour(cp.RED,cp.WHITE))
+                stdscr.addstr(by,bx," ",cp.set_colour(BGCL,cp.WHITE))
         rectangle(stdscr,y//2-(len(message)//2)-1, x//2-(maxs//2)-1, y//2+(len(message)//2)+4, x//2+(maxs//2+1)+1)
         stdscr.addstr(y//2-(len(message)//2)-1, x//2-(maxs//2)-1,title)
         mi = -(len(message)/2)
         stdscr.addstr(y//2+(len(message)//2)+3,x//2-(maxs//2),"[OK]",cp.set_colour(cp.WHITE,cp.BLACK)) 
         for msgl in message:
             mi += 1
             stdscr.addstr(int(y//2+mi),int(x//2-len(msgl)//2),msgl,cp.set_colour(cp.RED,cp.WHITE))
```

### Comparing `cursesplus-2.0.0/src/cursesplus.egg-info/PKG-INFO` & `cursesplus-2.0.1/src/cursesplus.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cursesplus
-Version: 2.0.0
+Version: 2.0.1
 Summary: An extension program to curses that offers option menus, message boxes, file dialogs and more
 Author-email: Enderbyte Programs <enderbyte09@gmail.com>
 Project-URL: Homepage, https://github.com/Enderbyte-Programs/Curses-Plus
 Project-URL: Bug Tracker, https://github.com/Enderbyte-Programs/Curses-Plus/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -36,15 +36,19 @@
 Microsoft Windows 11
 Any modern distro of Linux that supports Python3
 
 **Python Version 3.6 or newer**
 
 ## What's New?
 
-Version 2.0: Incompatible api changes
+### Version 2.0.1
+
+Colour is now optional in messagebox
+
+### Version 2.0: Incompatible api changes
 
 -askyesno now MUST be messagebox.askyesno
 -Rewrite colour system. load_colours() is now nonexistent.
 -Now use set_colour(background,foreground). A set of colour constants are defined in the cp class.
 
 ## Uses
```

