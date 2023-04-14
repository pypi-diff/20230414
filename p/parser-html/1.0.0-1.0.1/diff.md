# Comparing `tmp/parser-html-1.0.0.tar.gz` & `tmp/parser-html-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parser-html-1.0.0.tar", last modified: Sat Apr  8 18:19:55 2023, max compression
+gzip compressed data, was "parser-html-1.0.1.tar", last modified: Fri Apr 14 10:17:54 2023, max compression
```

## Comparing `parser-html-1.0.0.tar` & `parser-html-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-08 18:19:55.919646 parser-html-1.0.0/
--rw-rw-rw-   0        0        0     1068 2023-04-08 17:51:36.000000 parser-html-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     1667 2023-04-08 18:19:55.918645 parser-html-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1100 2023-04-08 18:17:08.000000 parser-html-1.0.0/README.md
--rw-rw-rw-   0        0        0      592 2023-04-08 18:18:06.000000 parser-html-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-08 18:19:55.919646 parser-html-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-08 18:19:55.900844 parser-html-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-08 18:19:55.910528 parser-html-1.0.0/src/htmlparse/
--rw-rw-rw-   0        0        0       41 2023-04-08 17:59:07.000000 parser-html-1.0.0/src/htmlparse/__init__.py
--rw-rw-rw-   0        0        0     9301 2023-04-08 18:11:09.000000 parser-html-1.0.0/src/htmlparse/html.py
-drwxrwxrwx   0        0        0        0 2023-04-08 18:19:55.916649 parser-html-1.0.0/src/parser_html.egg-info/
--rw-rw-rw-   0        0        0     1667 2023-04-08 18:19:55.000000 parser-html-1.0.0/src/parser_html.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-04-08 18:19:55.000000 parser-html-1.0.0/src/parser_html.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-08 18:19:55.000000 parser-html-1.0.0/src/parser_html.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-08 18:19:55.000000 parser-html-1.0.0/src/parser_html.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 10:17:54.059038 parser-html-1.0.1/
+-rw-rw-rw-   0        0        0     1068 2023-04-08 17:51:36.000000 parser-html-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     2107 2023-04-14 10:17:54.058037 parser-html-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1533 2023-04-14 10:06:19.000000 parser-html-1.0.1/README.md
+-rw-rw-rw-   0        0        0      592 2023-04-13 19:13:18.000000 parser-html-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-14 10:17:54.059038 parser-html-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-14 10:17:54.042229 parser-html-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-14 10:17:54.049986 parser-html-1.0.1/src/htmlparse/
+-rw-rw-rw-   0        0        0       51 2023-04-14 09:48:06.000000 parser-html-1.0.1/src/htmlparse/__init__.py
+-rw-rw-rw-   0        0        0    12423 2023-04-14 10:13:59.000000 parser-html-1.0.1/src/htmlparse/html.py
+drwxrwxrwx   0        0        0        0 2023-04-14 10:17:54.056031 parser-html-1.0.1/src/parser_html.egg-info/
+-rw-rw-rw-   0        0        0     2107 2023-04-14 10:17:54.000000 parser-html-1.0.1/src/parser_html.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-04-14 10:17:54.000000 parser-html-1.0.1/src/parser_html.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 10:17:54.000000 parser-html-1.0.1/src/parser_html.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-14 10:17:54.000000 parser-html-1.0.1/src/parser_html.egg-info/top_level.txt
```

### Comparing `parser-html-1.0.0/LICENSE` & `parser-html-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `parser-html-1.0.0/PKG-INFO` & `parser-html-1.0.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parser-html
-Version: 1.0.0
+Version: 1.0.1
 Summary: A basic HTML parser in Python
 Author-email: Aarav Malani <aarav.malani@gmail.com>
 Project-URL: Homepage, https://github.com/AaravMalani/htmlparse
 Project-URL: Bug Tracker, https://github.com/AaravMalani/htmlparse/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -30,22 +30,29 @@
 with open('index.html', 'r') as f:
     element = htmlparse.parse_html(f.read())
     if not element:
         raise ValueError("Parsing failed!")
 print(element.children) # Sub-elements
 print(element.innerHTML) # Data enclosed by tag
 print(element.outerHTML) # Data enclosed by tag as well as the tag itself
-element.innerHTML = 'e' # Rebuilds this element and sets the innerHTML of all the parent elements
+element.innerHTML = 'e&gt;' # Rebuilds this element and sets the innerHTML of all the parent elements
+print(element.children) # ['e>'] (The HTMLText element is represented as a string literal)
+print(element.children[0].text) # e> (Use HTMLText.outerHTML for an HTML escaped string (e&gt;) however don't set it)
 element.outerHTML = '<div class="black blue"><a href="https://github.com/" id="abc"></div>' # Read above statement
 # assigning to element.children is in the works
-tag = element.getElementById('abc')
 print(tag.attrs) # {"href":"https://github.com/", "id":"abc"}
 print(tag.tag_name) # a
+element.children = []
+element.attrs = {} # WARNING! You have to set it, you can't do element.attrs.update or element.attrs |=
+print(tag.outerHTML) # <div></div>
 ```
 
 ## ToDo
 - [ ] Support for CSS styles 
 - [ ] Support for JS scripts
-- [ ] Support for assignment to `HTMLElement.children` list
+- [x] Support for assignment to `HTMLElement.children` list
+- [x] Support for text between strings
+- [ ] Support for CSS selectors
+- [ ] Support for XPATH
```

#### html2text {}

```diff
@@ -1,22 +1,27 @@
-Metadata-Version: 2.1 Name: parser-html Version: 1.0.0 Summary: A basic HTML
+Metadata-Version: 2.1 Name: parser-html Version: 1.0.1 Summary: A basic HTML
 parser in Python Author-email: Aarav Malani
 malani@gmail.com> Project-URL: Homepage, https://github.com/AaravMalani/
 htmlparse Project-URL: Bug Tracker, https://github.com/AaravMalani/htmlparse/
 issues Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE # htmlparse: A basic HTML parser in Python ## Installation ```sh #
 Linux python3 -m pip install parser-html # Windows python -m pip install
 parser-html # Build from source python -m pip install git+https://github.com/
 AaravMalani/htmlparse ``` ## Usage ```py import htmlparse with open
 ('index.html', 'r') as f: element = htmlparse.parse_html(f.read()) if not
 element: raise ValueError("Parsing failed!") print(element.children) # Sub-
 elements print(element.innerHTML) # Data enclosed by tag print
 (element.outerHTML) # Data enclosed by tag as well as the tag itself
-element.innerHTML = 'e' # Rebuilds this element and sets the innerHTML of all
-the parent elements element.outerHTML = '
-' # Read above statement # assigning to element.children is in the works tag =
-element.getElementById('abc') print(tag.attrs) # {"href":"https://github.com/",
-"id":"abc"} print(tag.tag_name) # a ``` ## ToDo - [ ] Support for CSS styles -
-[ ] Support for JS scripts - [ ] Support for assignment to
-`HTMLElement.children` list
+element.innerHTML = 'e>' # Rebuilds this element and sets the innerHTML of all
+the parent elements print(element.children) # ['e>'] (The HTMLText element is
+represented as a string literal) print(element.children[0].text) # e> (Use
+HTMLText.outerHTML for an HTML escaped string (e>) however don't set it)
+element.outerHTML = '
+' # Read above statement # assigning to element.children is in the works print
+(tag.attrs) # {"href":"https://github.com/", "id":"abc"} print(tag.tag_name) #
+a element.children = [] element.attrs = {} # WARNING! You have to set it, you
+can't do element.attrs.update or element.attrs |= print(tag.outerHTML) #
+``` ## ToDo - [ ] Support for CSS styles - [ ] Support for JS scripts - [x]
+Support for assignment to `HTMLElement.children` list - [x] Support for text
+between strings - [ ] Support for CSS selectors - [ ] Support for XPATH
```

### Comparing `parser-html-1.0.0/pyproject.toml` & `parser-html-1.0.1/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "parser-html"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Aarav Malani", email="aarav.malani@gmail.com" },
 ]
 description = "A basic HTML parser in Python"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `parser-html-1.0.0/src/parser_html.egg-info/PKG-INFO` & `parser-html-1.0.1/src/parser_html.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parser-html
-Version: 1.0.0
+Version: 1.0.1
 Summary: A basic HTML parser in Python
 Author-email: Aarav Malani <aarav.malani@gmail.com>
 Project-URL: Homepage, https://github.com/AaravMalani/htmlparse
 Project-URL: Bug Tracker, https://github.com/AaravMalani/htmlparse/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -30,22 +30,29 @@
 with open('index.html', 'r') as f:
     element = htmlparse.parse_html(f.read())
     if not element:
         raise ValueError("Parsing failed!")
 print(element.children) # Sub-elements
 print(element.innerHTML) # Data enclosed by tag
 print(element.outerHTML) # Data enclosed by tag as well as the tag itself
-element.innerHTML = 'e' # Rebuilds this element and sets the innerHTML of all the parent elements
+element.innerHTML = 'e&gt;' # Rebuilds this element and sets the innerHTML of all the parent elements
+print(element.children) # ['e>'] (The HTMLText element is represented as a string literal)
+print(element.children[0].text) # e> (Use HTMLText.outerHTML for an HTML escaped string (e&gt;) however don't set it)
 element.outerHTML = '<div class="black blue"><a href="https://github.com/" id="abc"></div>' # Read above statement
 # assigning to element.children is in the works
-tag = element.getElementById('abc')
 print(tag.attrs) # {"href":"https://github.com/", "id":"abc"}
 print(tag.tag_name) # a
+element.children = []
+element.attrs = {} # WARNING! You have to set it, you can't do element.attrs.update or element.attrs |=
+print(tag.outerHTML) # <div></div>
 ```
 
 ## ToDo
 - [ ] Support for CSS styles 
 - [ ] Support for JS scripts
-- [ ] Support for assignment to `HTMLElement.children` list
+- [x] Support for assignment to `HTMLElement.children` list
+- [x] Support for text between strings
+- [ ] Support for CSS selectors
+- [ ] Support for XPATH
```

#### html2text {}

```diff
@@ -1,22 +1,27 @@
-Metadata-Version: 2.1 Name: parser-html Version: 1.0.0 Summary: A basic HTML
+Metadata-Version: 2.1 Name: parser-html Version: 1.0.1 Summary: A basic HTML
 parser in Python Author-email: Aarav Malani
 malani@gmail.com> Project-URL: Homepage, https://github.com/AaravMalani/
 htmlparse Project-URL: Bug Tracker, https://github.com/AaravMalani/htmlparse/
 issues Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE # htmlparse: A basic HTML parser in Python ## Installation ```sh #
 Linux python3 -m pip install parser-html # Windows python -m pip install
 parser-html # Build from source python -m pip install git+https://github.com/
 AaravMalani/htmlparse ``` ## Usage ```py import htmlparse with open
 ('index.html', 'r') as f: element = htmlparse.parse_html(f.read()) if not
 element: raise ValueError("Parsing failed!") print(element.children) # Sub-
 elements print(element.innerHTML) # Data enclosed by tag print
 (element.outerHTML) # Data enclosed by tag as well as the tag itself
-element.innerHTML = 'e' # Rebuilds this element and sets the innerHTML of all
-the parent elements element.outerHTML = '
-' # Read above statement # assigning to element.children is in the works tag =
-element.getElementById('abc') print(tag.attrs) # {"href":"https://github.com/",
-"id":"abc"} print(tag.tag_name) # a ``` ## ToDo - [ ] Support for CSS styles -
-[ ] Support for JS scripts - [ ] Support for assignment to
-`HTMLElement.children` list
+element.innerHTML = 'e>' # Rebuilds this element and sets the innerHTML of all
+the parent elements print(element.children) # ['e>'] (The HTMLText element is
+represented as a string literal) print(element.children[0].text) # e> (Use
+HTMLText.outerHTML for an HTML escaped string (e>) however don't set it)
+element.outerHTML = '
+' # Read above statement # assigning to element.children is in the works print
+(tag.attrs) # {"href":"https://github.com/", "id":"abc"} print(tag.tag_name) #
+a element.children = [] element.attrs = {} # WARNING! You have to set it, you
+can't do element.attrs.update or element.attrs |= print(tag.outerHTML) #
+``` ## ToDo - [ ] Support for CSS styles - [ ] Support for JS scripts - [x]
+Support for assignment to `HTMLElement.children` list - [x] Support for text
+between strings - [ ] Support for CSS selectors - [ ] Support for XPATH
```

