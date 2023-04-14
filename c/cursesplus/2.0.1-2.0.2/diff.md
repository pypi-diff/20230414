# Comparing `tmp/cursesplus-2.0.1.tar.gz` & `tmp/cursesplus-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cursesplus-2.0.1.tar", last modified: Fri Apr 14 17:50:35 2023, max compression
+gzip compressed data, was "cursesplus-2.0.2.tar", last modified: Fri Apr 14 17:55:16 2023, max compression
```

## Comparing `cursesplus-2.0.1.tar` & `cursesplus-2.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-04-14 17:50:35.783825 cursesplus-2.0.1/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1089 2023-04-07 16:31:31.000000 cursesplus-2.0.1/LICENSE
--rw-r--r--   0 jordan    (1000) jordan    (1000)     1617 2023-04-14 17:50:35.783825 cursesplus-2.0.1/PKG-INFO
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1014 2023-04-14 17:48:06.000000 cursesplus-2.0.1/README.md
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      659 2023-04-14 17:48:12.000000 cursesplus-2.0.1/pyproject.toml
--rw-r--r--   0 jordan    (1000) jordan    (1000)       38 2023-04-14 17:50:35.783825 cursesplus-2.0.1/setup.cfg
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-04-14 17:50:35.773825 cursesplus-2.0.1/src/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      555 2023-04-07 16:31:31.000000 cursesplus-2.0.1/src/__cptest.py
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-04-14 17:50:35.783825 cursesplus-2.0.1/src/cursesplus/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      892 2023-04-07 16:31:31.000000 cursesplus-2.0.1/src/cursesplus/__init__.py
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)    11516 2023-04-07 16:31:31.000000 cursesplus-2.0.1/src/cursesplus/cp.py
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)    11277 2023-04-07 16:45:57.000000 cursesplus-2.0.1/src/cursesplus/filedialog.py
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     5994 2023-04-14 17:49:51.000000 cursesplus-2.0.1/src/cursesplus/messagebox.py
-drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-04-14 17:50:35.783825 cursesplus-2.0.1/src/cursesplus.egg-info/
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1617 2023-04-14 17:50:35.000000 cursesplus-2.0.1/src/cursesplus.egg-info/PKG-INFO
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)      306 2023-04-14 17:50:35.000000 cursesplus-2.0.1/src/cursesplus.egg-info/SOURCES.txt
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)        1 2023-04-14 17:50:35.000000 cursesplus-2.0.1/src/cursesplus.egg-info/dependency_links.txt
--rwxr-xr-x   0 jordan    (1000) jordan    (1000)       20 2023-04-14 17:50:35.000000 cursesplus-2.0.1/src/cursesplus.egg-info/top_level.txt
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-04-14 17:55:16.873825 cursesplus-2.0.2/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1089 2023-04-07 16:31:31.000000 cursesplus-2.0.2/LICENSE
+-rw-r--r--   0 jordan    (1000) jordan    (1000)     1617 2023-04-14 17:55:16.873825 cursesplus-2.0.2/PKG-INFO
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1014 2023-04-14 17:48:06.000000 cursesplus-2.0.2/README.md
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      659 2023-04-14 17:55:01.000000 cursesplus-2.0.2/pyproject.toml
+-rw-r--r--   0 jordan    (1000) jordan    (1000)       38 2023-04-14 17:55:16.873825 cursesplus-2.0.2/setup.cfg
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-04-14 17:55:16.873825 cursesplus-2.0.2/src/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      555 2023-04-07 16:31:31.000000 cursesplus-2.0.2/src/__cptest.py
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-04-14 17:55:16.873825 cursesplus-2.0.2/src/cursesplus/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      892 2023-04-07 16:31:31.000000 cursesplus-2.0.2/src/cursesplus/__init__.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)    11516 2023-04-07 16:31:31.000000 cursesplus-2.0.2/src/cursesplus/cp.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)    11277 2023-04-07 16:45:57.000000 cursesplus-2.0.2/src/cursesplus/filedialog.py
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     5980 2023-04-14 17:54:57.000000 cursesplus-2.0.2/src/cursesplus/messagebox.py
+drwxr-xr-x   0 jordan    (1000) jordan    (1000)        0 2023-04-14 17:55:16.873825 cursesplus-2.0.2/src/cursesplus.egg-info/
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)     1617 2023-04-14 17:55:16.000000 cursesplus-2.0.2/src/cursesplus.egg-info/PKG-INFO
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)      306 2023-04-14 17:55:16.000000 cursesplus-2.0.2/src/cursesplus.egg-info/SOURCES.txt
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)        1 2023-04-14 17:55:16.000000 cursesplus-2.0.2/src/cursesplus.egg-info/dependency_links.txt
+-rwxr-xr-x   0 jordan    (1000) jordan    (1000)       20 2023-04-14 17:55:16.000000 cursesplus-2.0.2/src/cursesplus.egg-info/top_level.txt
```

### Comparing `cursesplus-2.0.1/LICENSE` & `cursesplus-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cursesplus-2.0.1/PKG-INFO` & `cursesplus-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cursesplus
-Version: 2.0.1
+Version: 2.0.2
 Summary: An extension program to curses that offers option menus, message boxes, file dialogs and more
 Author-email: Enderbyte Programs <enderbyte09@gmail.com>
 Project-URL: Homepage, https://github.com/Enderbyte-Programs/Curses-Plus
 Project-URL: Bug Tracker, https://github.com/Enderbyte-Programs/Curses-Plus/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cursesplus-2.0.1/README.md` & `cursesplus-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `cursesplus-2.0.1/pyproject.toml` & `cursesplus-2.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "cursesplus"
-version = "2.0.1"
+version = "2.0.2"
 authors = [{name="Enderbyte Programs",email="enderbyte09@gmail.com"},]
 description = "An extension program to curses that offers option menus, message boxes, file dialogs and more"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
 	"Programming Language :: Python :: 3",
 	"License :: OSI Approved :: MIT License",
```

### Comparing `cursesplus-2.0.1/src/__cptest.py` & `cursesplus-2.0.2/src/__cptest.py`

 * *Files identical despite different names*

### Comparing `cursesplus-2.0.1/src/cursesplus/__init__.py` & `cursesplus-2.0.2/src/cursesplus/__init__.py`

 * *Files identical despite different names*

### Comparing `cursesplus-2.0.1/src/cursesplus/cp.py` & `cursesplus-2.0.2/src/cursesplus/cp.py`

 * *Files identical despite different names*

### Comparing `cursesplus-2.0.1/src/cursesplus/filedialog.py` & `cursesplus-2.0.2/src/cursesplus/filedialog.py`

 * *Files identical despite different names*

### Comparing `cursesplus-2.0.1/src/cursesplus/messagebox.py` & `cursesplus-2.0.2/src/cursesplus/messagebox.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         rectangle(stdscr,y//2-(len(message)//2)-1, x//2-(maxs//2)-1, y//2+(len(message)//2)+4, x//2+(maxs//2+1)+1)
         stdscr.addstr(y//2+(len(message)//2)+4,x//2-(maxs//2),"Y: Yes | N: No")
         mi = -(len(message)/2)
         stdscr.addstr(y//2+(len(message)//2)+3,x//2-(maxs//2),"[Yes]",[cp.set_colour(cp.WHITE,cp.BLACK) if selected else cp.set_colour(cp.BLACK,cp.WHITE)][0])
         stdscr.addstr(y//2+(len(message)//2)+3,x//2-(maxs//2)+10,"[No]",[cp.set_colour(cp.BLACK,cp.WHITE) if selected else cp.set_colour(cp.WHITE,cp.BLACK)][0])   
         for msgl in message:
             mi += 1
-            stdscr.addstr(int(y//2+mi),int(x//2-len(msgl)//2),msgl,cp.set_colour(cp.GREEN,cp.WHITE))
+            stdscr.addstr(int(y//2+mi),int(x//2-len(msgl)//2),msgl,cp.set_colour(BGCL,cp.WHITE))
     
         stdscr.refresh()
         
         ch = stdscr.getch()
         if ch == curses.KEY_RIGHT or ch == curses.KEY_LEFT:
             selected = not selected
         elif ch == 121 or ch == 110:
@@ -62,15 +62,15 @@
                 stdscr.addstr(by,bx," ",cp.set_colour(BGCL,cp.WHITE))
         rectangle(stdscr,y//2-(len(message)//2)-1, x//2-(maxs//2)-1, y//2+(len(message)//2)+4, x//2+(maxs//2+1)+1)
         stdscr.addstr(y//2-(len(message)//2)-1, x//2-(maxs//2)-1,title)
         mi = -(len(message)/2)
         stdscr.addstr(y//2+(len(message)//2)+3,x//2-(maxs//2),"[OK]",cp.set_colour(cp.WHITE,cp.BLACK)) 
         for msgl in message:
             mi += 1
-            stdscr.addstr(int(y//2+mi),int(x//2-len(msgl)//2),msgl,cp.set_colour(cp.BLUE,cp.WHITE))
+            stdscr.addstr(int(y//2+mi),int(x//2-len(msgl)//2),msgl,cp.set_colour(BGCL,cp.WHITE))
     
         stdscr.refresh()
         
         ch = stdscr.getch()
         if ch == 10 or ch == 13 or ch == curses.KEY_ENTER:
             return
 
@@ -95,15 +95,15 @@
                 stdscr.addstr(by,bx," ",cp.set_colour(BGCL,cp.WHITE))
         rectangle(stdscr,y//2-(len(message)//2)-1, x//2-(maxs//2)-1, y//2+(len(message)//2)+4, x//2+(maxs//2+1)+1)
         stdscr.addstr(y//2-(len(message)//2)-1, x//2-(maxs//2)-1,title)
         mi = -(len(message)/2)
         stdscr.addstr(y//2+(len(message)//2)+3,x//2-(maxs//2),"[OK]",cp.set_colour(cp.WHITE,cp.BLACK)) 
         for msgl in message:
             mi += 1
-            stdscr.addstr(int(y//2+mi),int(x//2-len(msgl)//2),msgl,cp.set_colour(cp.YELLOW,cp.WHITE))
+            stdscr.addstr(int(y//2+mi),int(x//2-len(msgl)//2),msgl,cp.set_colour(BGCL,cp.WHITE))
     
         stdscr.refresh()
         
         ch = stdscr.getch()
         if ch == 10 or ch == 13 or ch == curses.KEY_ENTER:
             return
 
@@ -128,14 +128,14 @@
                 stdscr.addstr(by,bx," ",cp.set_colour(BGCL,cp.WHITE))
         rectangle(stdscr,y//2-(len(message)//2)-1, x//2-(maxs//2)-1, y//2+(len(message)//2)+4, x//2+(maxs//2+1)+1)
         stdscr.addstr(y//2-(len(message)//2)-1, x//2-(maxs//2)-1,title)
         mi = -(len(message)/2)
         stdscr.addstr(y//2+(len(message)//2)+3,x//2-(maxs//2),"[OK]",cp.set_colour(cp.WHITE,cp.BLACK)) 
         for msgl in message:
             mi += 1
-            stdscr.addstr(int(y//2+mi),int(x//2-len(msgl)//2),msgl,cp.set_colour(cp.RED,cp.WHITE))
+            stdscr.addstr(int(y//2+mi),int(x//2-len(msgl)//2),msgl,cp.set_colour(BGCL,cp.WHITE))
     
         stdscr.refresh()
         
         ch = stdscr.getch()
         if ch == 10 or ch == 13 or ch == curses.KEY_ENTER:
             return
```

### Comparing `cursesplus-2.0.1/src/cursesplus.egg-info/PKG-INFO` & `cursesplus-2.0.2/src/cursesplus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cursesplus
-Version: 2.0.1
+Version: 2.0.2
 Summary: An extension program to curses that offers option menus, message boxes, file dialogs and more
 Author-email: Enderbyte Programs <enderbyte09@gmail.com>
 Project-URL: Homepage, https://github.com/Enderbyte-Programs/Curses-Plus
 Project-URL: Bug Tracker, https://github.com/Enderbyte-Programs/Curses-Plus/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

