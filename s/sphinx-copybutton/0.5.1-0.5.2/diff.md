# Comparing `tmp/sphinx-copybutton-0.5.1.tar.gz` & `tmp/sphinx-copybutton-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-copybutton-0.5.1.tar", last modified: Tue Nov 15 10:17:11 2022, max compression
+gzip compressed data, was "sphinx-copybutton-0.5.2.tar", last modified: Fri Apr 14 08:10:11 2023, max compression
```

## Comparing `sphinx-copybutton-0.5.1.tar` & `sphinx-copybutton-0.5.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 10:17:11.003572 sphinx-copybutton-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-11-15 10:16:59.000000 sphinx-copybutton-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-11-15 10:16:59.000000 sphinx-copybutton-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2891 2022-11-15 10:17:11.003572 sphinx-copybutton-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2169 2022-11-15 10:16:59.000000 sphinx-copybutton-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 10:17:11.003572 sphinx-copybutton-0.5.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      614 2022-11-15 10:16:59.000000 sphinx-copybutton-0.5.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 10:17:11.003572 sphinx-copybutton-0.5.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)      434 2022-11-15 10:16:59.000000 sphinx-copybutton-0.5.1/docs/_static/clipboard.svg
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-11-15 10:16:59.000000 sphinx-copybutton-0.5.1/docs/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 10:17:11.003572 sphinx-copybutton-0.5.1/docs/_static/test/
--rw-r--r--   0 runner    (1001) docker     (121)      611 2022-11-15 10:16:59.000000 sphinx-copybutton-0.5.1/docs/_static/test/TEST_COPYBUTTON.png
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-11-15 10:16:59.000000 sphinx-copybutton-0.5.1/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (121)     6460 2022-11-15 10:16:59.000000 sphinx-copybutton-0.5.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 10:17:11.003572 sphinx-copybutton-0.5.1/docs/contribute/
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-11-15 10:16:59.000000 sphinx-copybutton-0.5.1/docs/contribute/index.md
--rw-r--r--   0 runner    (1001) docker     (121)     2798 2022-11-15 10:16:59.000000 sphinx-copybutton-0.5.1/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 10:17:11.003572 sphinx-copybutton-0.5.1/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (121)     1774 2022-11-15 10:16:59.000000 sphinx-copybutton-0.5.1/docs/reference/example.md
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-11-15 10:16:59.000000 sphinx-copybutton-0.5.1/docs/reference/literal.py
--rw-r--r--   0 runner    (1001) docker     (121)    12606 2022-11-15 10:16:59.000000 sphinx-copybutton-0.5.1/docs/use.md
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-11-15 10:17:11.003572 sphinx-copybutton-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2141 2022-11-15 10:16:59.000000 sphinx-copybutton-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 10:17:11.003572 sphinx-copybutton-0.5.1/sphinx_copybutton/
--rw-r--r--   0 runner    (1001) docker     (121)     3662 2022-11-15 10:16:59.000000 sphinx-copybutton-0.5.1/sphinx_copybutton/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 10:17:11.003572 sphinx-copybutton-0.5.1/sphinx_copybutton/_static/
--rw-r--r--   0 runner    (1001) docker     (121)      313 2022-11-15 10:16:59.000000 sphinx-copybutton-0.5.1/sphinx_copybutton/_static/check-solid.svg
--rw-r--r--   0 runner    (1001) docker     (121)     9031 2022-11-15 10:17:04.000000 sphinx-copybutton-0.5.1/sphinx_copybutton/_static/clipboard.min.js
--rw-r--r--   0 runner    (1001) docker     (121)      411 2022-11-15 10:16:59.000000 sphinx-copybutton-0.5.1/sphinx_copybutton/_static/copy-button.svg
--rw-r--r--   0 runner    (1001) docker     (121)     2060 2022-11-15 10:16:59.000000 sphinx-copybutton-0.5.1/sphinx_copybutton/_static/copybutton.css
--rw-r--r--   0 runner    (1001) docker     (121)     6159 2022-11-15 10:16:59.000000 sphinx-copybutton-0.5.1/sphinx_copybutton/_static/copybutton.js_t
--rw-r--r--   0 runner    (1001) docker     (121)     2698 2022-11-15 10:16:59.000000 sphinx-copybutton-0.5.1/sphinx_copybutton/_static/copybutton_funcs.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 10:17:11.003572 sphinx-copybutton-0.5.1/sphinx_copybutton.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2891 2022-11-15 10:17:10.000000 sphinx-copybutton-0.5.1/sphinx_copybutton.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      775 2022-11-15 10:17:10.000000 sphinx-copybutton-0.5.1/sphinx_copybutton.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-15 10:17:10.000000 sphinx-copybutton-0.5.1/sphinx_copybutton.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-11-15 10:17:10.000000 sphinx-copybutton-0.5.1/sphinx_copybutton.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-11-15 10:17:10.000000 sphinx-copybutton-0.5.1/sphinx_copybutton.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:10:11.646607 sphinx-copybutton-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-14 08:10:02.000000 sphinx-copybutton-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-14 08:10:02.000000 sphinx-copybutton-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-14 08:10:11.646607 sphinx-copybutton-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-04-14 08:10:02.000000 sphinx-copybutton-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:10:11.642607 sphinx-copybutton-0.5.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-14 08:10:02.000000 sphinx-copybutton-0.5.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:10:11.642607 sphinx-copybutton-0.5.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-14 08:10:02.000000 sphinx-copybutton-0.5.2/docs/_static/clipboard.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-14 08:10:02.000000 sphinx-copybutton-0.5.2/docs/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:10:11.646607 sphinx-copybutton-0.5.2/docs/_static/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-14 08:10:02.000000 sphinx-copybutton-0.5.2/docs/_static/test/TEST_COPYBUTTON.png
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-14 08:10:02.000000 sphinx-copybutton-0.5.2/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-04-14 08:10:02.000000 sphinx-copybutton-0.5.2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:10:11.646607 sphinx-copybutton-0.5.2/docs/contribute/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-14 08:10:02.000000 sphinx-copybutton-0.5.2/docs/contribute/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-04-14 08:10:02.000000 sphinx-copybutton-0.5.2/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:10:11.646607 sphinx-copybutton-0.5.2/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-04-14 08:10:02.000000 sphinx-copybutton-0.5.2/docs/reference/example.md
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-14 08:10:02.000000 sphinx-copybutton-0.5.2/docs/reference/literal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13105 2023-04-14 08:10:02.000000 sphinx-copybutton-0.5.2/docs/use.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-14 08:10:11.646607 sphinx-copybutton-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-04-14 08:10:02.000000 sphinx-copybutton-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:10:11.646607 sphinx-copybutton-0.5.2/sphinx_copybutton/
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-04-14 08:10:02.000000 sphinx-copybutton-0.5.2/sphinx_copybutton/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:10:11.646607 sphinx-copybutton-0.5.2/sphinx_copybutton/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-14 08:10:02.000000 sphinx-copybutton-0.5.2/sphinx_copybutton/_static/check-solid.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-04-14 08:10:04.000000 sphinx-copybutton-0.5.2/sphinx_copybutton/_static/clipboard.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-14 08:10:02.000000 sphinx-copybutton-0.5.2/sphinx_copybutton/_static/copy-button.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-14 08:10:02.000000 sphinx-copybutton-0.5.2/sphinx_copybutton/_static/copybutton.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-04-14 08:10:02.000000 sphinx-copybutton-0.5.2/sphinx_copybutton/_static/copybutton.js_t
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-04-14 08:10:02.000000 sphinx-copybutton-0.5.2/sphinx_copybutton/_static/copybutton_funcs.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 08:10:11.646607 sphinx-copybutton-0.5.2/sphinx_copybutton.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-14 08:10:11.000000 sphinx-copybutton-0.5.2/sphinx_copybutton.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-14 08:10:11.000000 sphinx-copybutton-0.5.2/sphinx_copybutton.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 08:10:11.000000 sphinx-copybutton-0.5.2/sphinx_copybutton.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-14 08:10:11.000000 sphinx-copybutton-0.5.2/sphinx_copybutton.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-14 08:10:11.000000 sphinx-copybutton-0.5.2/sphinx_copybutton.egg-info/top_level.txt
```

### Comparing `sphinx-copybutton-0.5.1/LICENSE` & `sphinx-copybutton-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx-copybutton-0.5.1/PKG-INFO` & `sphinx-copybutton-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: sphinx-copybutton
-Version: 0.5.1
+Version: 0.5.2
 Summary: Add a copy button to each of your code cells.
 Home-page: https://github.com/executablebooks/sphinx-copybutton
 Author: Executable Book Project
 License: MIT License
+Classifier: Framework :: Sphinx :: Extension
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `sphinx-copybutton-0.5.1/README.md` & `sphinx-copybutton-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `sphinx-copybutton-0.5.1/docs/Makefile` & `sphinx-copybutton-0.5.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sphinx-copybutton-0.5.1/docs/_static/test/TEST_COPYBUTTON.png` & `sphinx-copybutton-0.5.2/docs/_static/test/TEST_COPYBUTTON.png`

 * *Files identical despite different names*

### Comparing `sphinx-copybutton-0.5.1/docs/conf.py` & `sphinx-copybutton-0.5.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sphinx-copybutton-0.5.1/docs/contribute/index.md` & `sphinx-copybutton-0.5.2/docs/contribute/index.md`

 * *Files identical despite different names*

### Comparing `sphinx-copybutton-0.5.1/docs/index.md` & `sphinx-copybutton-0.5.2/docs/index.md`

 * *Files 2% similar despite different names*

```diff
@@ -42,22 +42,22 @@
 123456789123456789123456789123456789123456789123456789123456789123456789123456789123456789123456789123456789123456789123456789123456789123456789123456789123456789
 ```
 
 You can configure `sphinx-copybutton` to detect *input prompts* in code
 cells, and then both remove these prompts before copying, as well as skip
 lines that *don't* start with prompts (in case they are output lines).
 
-For example, this site has been configured to strip Python prompts (">>> ").
+For example, this site has been configured to strip Python prompts (">>> ") and output lines.
 Try copy-pasting the code block below.
 
 ```python
 >>> a = 2
 >>> print(a)
 2
-
+>>>
 >>> b = 'wow'
 >>> print(b)
 wow
 ```
 
 ## Install
```

### Comparing `sphinx-copybutton-0.5.1/docs/reference/example.md` & `sphinx-copybutton-0.5.2/docs/reference/example.md`

 * *Files identical despite different names*

### Comparing `sphinx-copybutton-0.5.1/docs/use.md` & `sphinx-copybutton-0.5.2/docs/use.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,42 @@
 # Use and customize
 
 This section describes major ways to use and control `sphinx-copybutton`'s behavior.
 
 (configure-copy-text)=
+
+## Automatic exclusion of prompts from the copies
+
+The Sphinx code highlighter, Pygments, tags the prompts (`>>>`, `...`,
+`In [1]:`, `$`) of console sessions.
+Sphinx by default excludes prompts from being selectable.
+However, by default `sphinx-copybutton` will copy these prompts (for backwards compatibility with the other "manually-selectable exclude" options).
+
+To make `sphinx-copybutton` skip all prompt characters generated by pygments, use the following setting:
+
+```{code-block} python
+copybutton_exclude = '.linenos, .gp'
+```
+
+To **skip all console outputs**, add `.go` to the string above.
+
+For automatic exclusion, make sure to use the right highlight language.
+For example: `pythonconsole` instead of `python`, `console` instead of `bash`,
+`ipythonconsole` instead of `ipython`, etc.
+
+This setting can also be used to exclude arbitrary css classes from
+being copied.  By default `.linenos` are excluded.  `.linenos` is the
+Sphinx default for line numbers, `.gp` is the Pygments class for the
+prompts, and `.go` is the class for console outputs.
+
+This setting conflicts with most of pattern-based copy-selection
+settings below, so should not be used with them.  This will hopefully
+be improved in the future.
+
+
 ## Strip and configure input prompts for code cells
 
 By default, `sphinx-copybutton` will copy the entire contents of a code
 block when the button is clicked. For many languages, it is common to
 include **input prompts** with your examples, along with the outputs from
 running the code.
 
@@ -362,26 +392,7 @@
 }
 ```
 :::
 
 See the [Sphinx documentation on custom CSS for more information](https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-html_static_path).
 
 [regex101]: https://regex101.com
-
-
-## Exclude text from being copied
-
-You may exclude elements matching CSS selectors from being copied by
-specifying the `copybutton_exclude` option in ``conf.py``.  For
-example, a viewer usually doesn't want to copy the line numbers, and
-CSS provides a way to exclude this.  This option implements that
-option for sphinx-copybutton as well.
-
-
-```{code-block} python
-copybutton_exclude = '.exclude_me'
-```
-By default `.linenos, .gp` are excluded. If you specify the
-`copybutton_exclude` option it will replace the default.  `.linenos`
-is the Sphinx default for line numbers, and `.gp` is Pygments (the
-default highlighter of Sphinx) for "prompt", e.g. `$` in a
-shell-session. `.gp` is excluded in upstream Sphinx by default.
```

### Comparing `sphinx-copybutton-0.5.1/setup.py` & `sphinx-copybutton-0.5.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,14 +45,15 @@
             "_static/copybutton.js_t",
             "_static/copy-button.svg",
             "_static/check-solid.svg",
             "_static/clipboard.min.js",
         ]
     },
     classifiers=[
+        "Framework :: Sphinx :: Extension",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3 :: Only",
```

### Comparing `sphinx-copybutton-0.5.1/sphinx_copybutton/__init__.py` & `sphinx-copybutton-0.5.2/sphinx_copybutton/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """A small sphinx extension to add "copy" buttons to code blocks."""
 from pathlib import Path
 from sphinx.util import logging
 
-__version__ = "0.5.1"
+__version__ = "0.5.2"
 
 logger = logging.getLogger(__name__)
 
 
 def scb_static_path(app):
     app.config.html_static_path.append(
         str(Path(__file__).parent.joinpath("_static").absolute())
@@ -62,30 +62,29 @@
             .replace("export function", "function")
         }
     )
     config.html_context.update({"copybutton_exclude": config.copybutton_exclude})
 
 
 def setup(app):
-
     logger.verbose("Adding copy buttons to code blocks...")
     # Add our static path
     app.connect("builder-inited", scb_static_path)
 
     # configuration for this tool
     app.add_config_value("copybutton_prompt_text", "", "html")
     app.add_config_value("copybutton_prompt_is_regexp", False, "html")
     app.add_config_value("copybutton_only_copy_prompt_lines", True, "html")
     app.add_config_value("copybutton_remove_prompts", True, "html")
     app.add_config_value("copybutton_copy_empty_lines", True, "html")
     app.add_config_value("copybutton_line_continuation_character", "", "html")
     app.add_config_value("copybutton_here_doc_delimiter", "", "html")
     app.add_config_value("copybutton_image_svg", "", "html")
     app.add_config_value("copybutton_selector", "div.highlight pre", "html")
-    app.add_config_value("copybutton_exclude", ".linenos, .gp", "html")
+    app.add_config_value("copybutton_exclude", ".linenos", "html")
 
     # DEPRECATE THIS AFTER THE NEXT RELEASE
     app.add_config_value("copybutton_image_path", "", "html")
 
     # Add configuration value to the template
     app.connect("config-inited", add_to_context)
```

### Comparing `sphinx-copybutton-0.5.1/sphinx_copybutton/_static/clipboard.min.js` & `sphinx-copybutton-0.5.2/sphinx_copybutton/_static/clipboard.min.js`

 * *Files identical despite different names*

### Comparing `sphinx-copybutton-0.5.1/sphinx_copybutton/_static/copybutton.css` & `sphinx-copybutton-0.5.2/sphinx_copybutton/_static/copybutton.css`

 * *Files identical despite different names*

### Comparing `sphinx-copybutton-0.5.1/sphinx_copybutton/_static/copybutton.js_t` & `sphinx-copybutton-0.5.2/sphinx_copybutton/_static/copybutton.js_t`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     'copy': 'Kopieren',
     'copy_to_clipboard': 'In die Zwischenablage kopieren',
     'copy_success': 'Kopiert!',
     'copy_failure': 'Fehler beim Kopieren',
   },
   'fr' : {
     'copy': 'Copier',
-    'copy_to_clipboard': 'Copié dans le presse-papier',
+    'copy_to_clipboard': 'Copier dans le presse-papier',
     'copy_success': 'Copié !',
     'copy_failure': 'Échec de la copie',
   },
   'ru': {
     'copy': 'Скопировать',
     'copy_to_clipboard': 'Скопировать в буфер',
     'copy_success': 'Скопировано!',
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 // Localization support const messages = { 'en': { 'copy': 'Copy',
 'copy_to_clipboard': 'Copy to clipboard', 'copy_success': 'Copied!',
 'copy_failure': 'Failed to copy', }, 'es' : { 'copy': 'Copiar',
 'copy_to_clipboard': 'Copiar al portapapeles', 'copy_success': 'Â¡Copiado!',
 'copy_failure': 'Error al copiar', }, 'de' : { 'copy': 'Kopieren',
 'copy_to_clipboard': 'In die Zwischenablage kopieren', 'copy_success':
 'Kopiert!', 'copy_failure': 'Fehler beim Kopieren', }, 'fr' : { 'copy':
-'Copier', 'copy_to_clipboard': 'CopiÃ© dans le presse-papier', 'copy_success':
+'Copier', 'copy_to_clipboard': 'Copier dans le presse-papier', 'copy_success':
 'CopiÃ© !', 'copy_failure': 'Ãchec de la copie', }, 'ru': { 'copy':
 'Ð¡ÐºÐ¾Ð¿Ð¸ÑÐ¾Ð²Ð°ÑÑ', 'copy_to_clipboard': 'Ð¡ÐºÐ¾Ð¿Ð¸ÑÐ¾Ð²Ð°ÑÑ Ð²
 Ð±ÑÑÐµÑ', 'copy_success': 'Ð¡ÐºÐ¾Ð¿Ð¸ÑÐ¾Ð²Ð°Ð½Ð¾!', 'copy_failure': 'ÐÐµ
 ÑÐ´Ð°Ð»Ð¾ÑÑ ÑÐºÐ¾Ð¿Ð¸ÑÐ¾Ð²Ð°ÑÑ', }, 'zh-CN': { 'copy': 'å¤å¶',
 'copy_to_clipboard': 'å¤å¶å°åªè´´æ¿', 'copy_success': 'å¤å¶æå!',
 'copy_failure': 'å¤å¶å¤±è´¥', }, 'it' : { 'copy': 'Copiare',
 'copy_to_clipboard': 'Copiato negli appunti', 'copy_success': 'Copiato!',
```

### Comparing `sphinx-copybutton-0.5.1/sphinx_copybutton/_static/copybutton_funcs.js` & `sphinx-copybutton-0.5.2/sphinx_copybutton/_static/copybutton_funcs.js`

 * *Files identical despite different names*

### Comparing `sphinx-copybutton-0.5.1/sphinx_copybutton.egg-info/PKG-INFO` & `sphinx-copybutton-0.5.2/sphinx_copybutton.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: sphinx-copybutton
-Version: 0.5.1
+Version: 0.5.2
 Summary: Add a copy button to each of your code cells.
 Home-page: https://github.com/executablebooks/sphinx-copybutton
 Author: Executable Book Project
 License: MIT License
+Classifier: Framework :: Sphinx :: Extension
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `sphinx-copybutton-0.5.1/sphinx_copybutton.egg-info/SOURCES.txt` & `sphinx-copybutton-0.5.2/sphinx_copybutton.egg-info/SOURCES.txt`

 * *Files identical despite different names*

