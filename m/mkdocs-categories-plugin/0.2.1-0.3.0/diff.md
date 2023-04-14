# Comparing `tmp/mkdocs-categories-plugin-0.2.1.tar.gz` & `tmp/mkdocs-categories-plugin-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-categories-plugin-0.2.1.tar", last modified: Sat Jul  2 21:20:19 2022, max compression
+gzip compressed data, was "mkdocs-categories-plugin-0.3.0.tar", last modified: Fri Apr 14 03:56:25 2023, max compression
```

## Comparing `mkdocs-categories-plugin-0.2.1.tar` & `mkdocs-categories-plugin-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-02 21:20:19.767861 mkdocs-categories-plugin-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1106 2022-07-02 21:20:07.000000 mkdocs-categories-plugin-0.2.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)     5194 2022-07-02 21:20:19.767861 mkdocs-categories-plugin-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4557 2022-07-02 21:20:07.000000 mkdocs-categories-plugin-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-02 21:20:19.767861 mkdocs-categories-plugin-0.2.1/categories/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-02 21:20:07.000000 mkdocs-categories-plugin-0.2.1/categories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8186 2022-07-02 21:20:07.000000 mkdocs-categories-plugin-0.2.1/categories/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-02 21:20:19.767861 mkdocs-categories-plugin-0.2.1/mkdocs_categories_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5194 2022-07-02 21:20:19.000000 mkdocs-categories-plugin-0.2.1/mkdocs_categories_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      363 2022-07-02 21:20:19.000000 mkdocs-categories-plugin-0.2.1/mkdocs_categories_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-02 21:20:19.000000 mkdocs-categories-plugin-0.2.1/mkdocs_categories_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-07-02 21:20:19.000000 mkdocs-categories-plugin-0.2.1/mkdocs_categories_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-07-02 21:20:19.000000 mkdocs-categories-plugin-0.2.1/mkdocs_categories_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-07-02 21:20:19.000000 mkdocs-categories-plugin-0.2.1/mkdocs_categories_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-02 21:20:19.767861 mkdocs-categories-plugin-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1128 2022-07-02 21:20:07.000000 mkdocs-categories-plugin-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:56:25.674928 mkdocs-categories-plugin-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-14 03:56:15.000000 mkdocs-categories-plugin-0.3.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-04-14 03:56:25.674928 mkdocs-categories-plugin-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-04-14 03:56:15.000000 mkdocs-categories-plugin-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:56:25.670928 mkdocs-categories-plugin-0.3.0/categories/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:56:15.000000 mkdocs-categories-plugin-0.3.0/categories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10425 2023-04-14 03:56:15.000000 mkdocs-categories-plugin-0.3.0/categories/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 03:56:25.674928 mkdocs-categories-plugin-0.3.0/mkdocs_categories_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-04-14 03:56:25.000000 mkdocs-categories-plugin-0.3.0/mkdocs_categories_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-14 03:56:25.000000 mkdocs-categories-plugin-0.3.0/mkdocs_categories_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 03:56:25.000000 mkdocs-categories-plugin-0.3.0/mkdocs_categories_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-14 03:56:25.000000 mkdocs-categories-plugin-0.3.0/mkdocs_categories_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 03:56:25.000000 mkdocs-categories-plugin-0.3.0/mkdocs_categories_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-14 03:56:25.000000 mkdocs-categories-plugin-0.3.0/mkdocs_categories_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 03:56:25.674928 mkdocs-categories-plugin-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-14 03:56:15.000000 mkdocs-categories-plugin-0.3.0/setup.py
```

### Comparing `mkdocs-categories-plugin-0.2.1/LICENSE.md` & `mkdocs-categories-plugin-0.3.0/LICENSE.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 The MIT License (MIT)
 =====================
 
-Copyright © 2022 Eddy Luten
+Copyright © 2023 Eddy Luten
 
 Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation
-files (the “Software”), to deal in the Software without
+files (the "Software"), to deal in the Software without
 restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the
 Software is furnished to do so, subject to the following
 conditions:
 
 The above copyright notice and this permission notice shall be
 included in all copies or substantial portions of the Software.
 
-THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND,
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
 EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES
 OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
 HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
 WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `mkdocs-categories-plugin-0.2.1/PKG-INFO` & `mkdocs-categories-plugin-0.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,18 @@
-Metadata-Version: 2.1
-Name: mkdocs-categories-plugin
-Version: 0.2.1
-Summary: An MkDocs plugin allowing for categorization of pages
-Home-page: https://github.com/eddyluten/mkdocs-categories-plugin
-Author: Eddy Luten
-Author-email: eddyluten@gmail.com
-License: MIT
-Keywords: mkdocs python markdown category categories link wiki
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.0
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 # mkdocs-categories-plugin
 
 [![PyPI version](https://badge.fury.io/py/mkdocs-categories-plugin.svg)](https://pypi.org/project/mkdocs-categories-plugin/)  [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) ![example workflow](https://github.com/eddyluten/mkdocs-categories-plugin/actions/workflows/pylint.yml/badge.svg) [![Downloads](https://pepy.tech/badge/mkdocs-categories-plugin)](https://pepy.tech/project/mkdocs-categories-plugin)
 
 An MkDocs plugin allowing for categorization of pages in your wiki. This plugin allows for multiple categories per page and will generate a category index page with links to each page within the category.
 
 If you like this MkDocs plugin, you'll probably also like [mkdocs-alias-plugin](https://github.com/EddyLuten/mkdocs-alias-plugin).
 
 ## Installation
 
-Install the package using pip:
+Using Python 3.10 or greater, install the package using pip:
 
 ```zsh
 pip install mkdocs-categories-plugin
 ```
 
 Then add the following entry to the plugins section of your `mkdocs.yml` file:
 
@@ -51,30 +34,47 @@
 categories:
     - Novels
     - Fiction
     - 19th Century Gothic Fiction
 ---
 ```
 
-New pages will be generated for each of these categories, with a list of links to each of the wiki pages within the category. The names of these categories are slugified before used in the category URLs. For example, `19th Century Gothic Fiction` becomes `19th-century-gothic-fiction`.
+New pages will be generated for each of these categories, with a list of links to each of the wiki pages within the category. Subcategories, links to the parent category, and a link to the "All Categories" page are automatically generated and placed on the page.
+
+Category names are slugified before used in category URLs. For example, `19th Century Gothic Fiction` becomes `19th-century-gothic-fiction`.
 
 Please refer to the [MkDocs documentation](https://www.mkdocs.org/user-guide/writing-your-docs/#yaml-style-meta-data) for more information on how the meta-data block is used.
 
+### Subcategories
+
+As of version 0.3.0, mkdocs-categories-plugin supports subcategorization. This is achieved by supplying a category name that separates parent from child categories using a separator (by default `|`, configurable via `category_separator`). You may supply as many levels of child categories as you like.
+
+For example:
+
+```yaml
+categories:
+    - Fiction|Romance
+    - Fiction|Books|British Authors|Female|19th Century
+```
+
+The first category definition in this example places the page in the *Romance* subcategory of the *Fiction* parent category. Note that the page will **not** be placed in the parent category of *Fiction*, but only in the *Romance* category. The second category definition places the page in the *19th Century* category, but not in any of its ancestor categories.
+
 ## Options
 
 You may customize the plugin by passing options into the plugin's configuration sections in `mkdocs.yml`:
 
 ```yaml
 plugins:
     - categories:
         generate_index: true
         verbose: false
         base_name: 'categories'
         section_title: 'Categories'
         no_nav: false
+        category_separator: '|'
 ```
 
 ### `generate_index`
 
 **Default:** `true`
 
 If true, an index page listing all of the generated categories is created at the `base_name` URL.
@@ -101,26 +101,36 @@
 
 **Default:** `false`
 
 By default, mkdocs-categories-plugin will generate navigation entries for each category page under the `base_name` that you provided. If you want to turn this behavior off, set this option to `true`.
 
 There's also a know issue with mkdocs-awesome-pages-plugin compatibility that does not allow you to reorder the position of the generated categories section by using a `.pages` file. If you would rather turn the navigation entries off entirely, this option is for you.
 
+### `category_separator`
+
+**Default:** `|`
+
+This string is used to split the category name in order to define a category hierarchy (see subcategories above).
+
 ## Troubleshooting
 
 ### There's a directory named `categories` in my project
 
 A fatal error must have occurred during the compilation of your site and left the temporary directory containing the intermediate markdown files used by this plugin behind. It is safe to delete this directory since it's only used during the build.
 
 ### `The categories object at URL was not a list, but TYPE`
 
 The page identified did not contain a valid categories configuration object. Please make sure that this is an array of strings.
 
 ## Changelog
 
+### 0.3.0
+
+Added support for subcategories. Python 3.10 or higher is now required.
+
 ### 0.2.1
 
 Patch release: implements a bug fix by @rpmzandwijk reported in [#1](https://github.com/EddyLuten/mkdocs-categories-plugin/issues/1).
 
 ### 0.2.0
 
 Introduces support for the automatic generation of category index pages. This new default behavior can be turned off using an option.
```

### Comparing `mkdocs-categories-plugin-0.2.1/README.md` & `mkdocs-categories-plugin-0.3.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,35 @@
+Metadata-Version: 2.1
+Name: mkdocs-categories-plugin
+Version: 0.3.0
+Summary: An MkDocs plugin allowing for categorization of pages
+Home-page: https://github.com/eddyluten/mkdocs-categories-plugin
+Author: Eddy Luten
+Author-email: eddyluten@gmail.com
+License: MIT
+Keywords: mkdocs python markdown category categories link wiki
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
 # mkdocs-categories-plugin
 
 [![PyPI version](https://badge.fury.io/py/mkdocs-categories-plugin.svg)](https://pypi.org/project/mkdocs-categories-plugin/)  [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) ![example workflow](https://github.com/eddyluten/mkdocs-categories-plugin/actions/workflows/pylint.yml/badge.svg) [![Downloads](https://pepy.tech/badge/mkdocs-categories-plugin)](https://pepy.tech/project/mkdocs-categories-plugin)
 
 An MkDocs plugin allowing for categorization of pages in your wiki. This plugin allows for multiple categories per page and will generate a category index page with links to each page within the category.
 
 If you like this MkDocs plugin, you'll probably also like [mkdocs-alias-plugin](https://github.com/EddyLuten/mkdocs-alias-plugin).
 
 ## Installation
 
-Install the package using pip:
+Using Python 3.10 or greater, install the package using pip:
 
 ```zsh
 pip install mkdocs-categories-plugin
 ```
 
 Then add the following entry to the plugins section of your `mkdocs.yml` file:
 
@@ -34,30 +51,47 @@
 categories:
     - Novels
     - Fiction
     - 19th Century Gothic Fiction
 ---
 ```
 
-New pages will be generated for each of these categories, with a list of links to each of the wiki pages within the category. The names of these categories are slugified before used in the category URLs. For example, `19th Century Gothic Fiction` becomes `19th-century-gothic-fiction`.
+New pages will be generated for each of these categories, with a list of links to each of the wiki pages within the category. Subcategories, links to the parent category, and a link to the "All Categories" page are automatically generated and placed on the page.
+
+Category names are slugified before used in category URLs. For example, `19th Century Gothic Fiction` becomes `19th-century-gothic-fiction`.
 
 Please refer to the [MkDocs documentation](https://www.mkdocs.org/user-guide/writing-your-docs/#yaml-style-meta-data) for more information on how the meta-data block is used.
 
+### Subcategories
+
+As of version 0.3.0, mkdocs-categories-plugin supports subcategorization. This is achieved by supplying a category name that separates parent from child categories using a separator (by default `|`, configurable via `category_separator`). You may supply as many levels of child categories as you like.
+
+For example:
+
+```yaml
+categories:
+    - Fiction|Romance
+    - Fiction|Books|British Authors|Female|19th Century
+```
+
+The first category definition in this example places the page in the *Romance* subcategory of the *Fiction* parent category. Note that the page will **not** be placed in the parent category of *Fiction*, but only in the *Romance* category. The second category definition places the page in the *19th Century* category, but not in any of its ancestor categories.
+
 ## Options
 
 You may customize the plugin by passing options into the plugin's configuration sections in `mkdocs.yml`:
 
 ```yaml
 plugins:
     - categories:
         generate_index: true
         verbose: false
         base_name: 'categories'
         section_title: 'Categories'
         no_nav: false
+        category_separator: '|'
 ```
 
 ### `generate_index`
 
 **Default:** `true`
 
 If true, an index page listing all of the generated categories is created at the `base_name` URL.
@@ -84,26 +118,36 @@
 
 **Default:** `false`
 
 By default, mkdocs-categories-plugin will generate navigation entries for each category page under the `base_name` that you provided. If you want to turn this behavior off, set this option to `true`.
 
 There's also a know issue with mkdocs-awesome-pages-plugin compatibility that does not allow you to reorder the position of the generated categories section by using a `.pages` file. If you would rather turn the navigation entries off entirely, this option is for you.
 
+### `category_separator`
+
+**Default:** `|`
+
+This string is used to split the category name in order to define a category hierarchy (see subcategories above).
+
 ## Troubleshooting
 
 ### There's a directory named `categories` in my project
 
 A fatal error must have occurred during the compilation of your site and left the temporary directory containing the intermediate markdown files used by this plugin behind. It is safe to delete this directory since it's only used during the build.
 
 ### `The categories object at URL was not a list, but TYPE`
 
 The page identified did not contain a valid categories configuration object. Please make sure that this is an array of strings.
 
 ## Changelog
 
+### 0.3.0
+
+Added support for subcategories. Python 3.10 or higher is now required.
+
 ### 0.2.1
 
 Patch release: implements a bug fix by @rpmzandwijk reported in [#1](https://github.com/EddyLuten/mkdocs-categories-plugin/issues/1).
 
 ### 0.2.0
 
 Introduces support for the automatic generation of category index pages. This new default behavior can be turned off using an option.
```

### Comparing `mkdocs-categories-plugin-0.2.1/categories/plugin.py` & `mkdocs-categories-plugin-0.3.0/categories/plugin.py`

 * *Files 21% similar despite different names*

```diff
@@ -38,15 +38,16 @@
     Defines the exported MkDocs plugin class and all its functionality.
     """
     config_scheme = (
         ('generate_index', config_options.Type(bool, default=True)),
         ('verbose', config_options.Type(bool, default=False)),
         ('no_nav', config_options.Type(bool, default=False)),
         ('base_name', config_options.Type(str, default='categories')),
-        ('section_title', config_options.Type(str, default='Categories'))
+        ('section_title', config_options.Type(str, default='Categories')),
+        ('category_separator', config_options.Type(str, default='|')),
     )
     log: Logger = getLogger(f'mkdocs.plugins.{__name__}')
     categories: dict = {}
     pages:dict = {}
     cat_path: Path = Path()
 
     def on_config(self, _):
@@ -73,65 +74,85 @@
             return nav
         for item in nav:
             if item.is_section and str(item.title).lower() == self.config['base_name']:
                 nav.items.remove(item)
                 break
         return nav
 
-    def on_build_error(self, **_):
+    def on_build_error(self, _error):
         """Executed after the build has failed."""
         self.categories.clear()
+        self.pages.clear()
         self.clean_temp_dir()
 
     def on_post_build(self, **_):
         """Executed after the build has successfully completed."""
         self.log.info("Defined %s categories.", len(self.categories))
         self.categories.clear()
+        self.pages.clear()
         self.clean_temp_dir()
 
-    def on_page_markdown(self, markdown: str, page: Page, **_):
+    def on_page_markdown(self, markdown: str, *, page: Page, **_):
         """Appends the category links section for a page to the markdown."""
         relative_url = get_relative_url(str(self.cat_path), page.file.url)
         if page.file.url not in self.pages:
             return markdown
         links = list(map(
-            lambda c: f"- [{c}]({relative_url}/{self.categories[c]['slug']}/)",
+            lambda c: (
+                f"- [{self.categories[c]['name']}]"
+                f"({relative_url}/{self.categories[c]['slug']}/)"
+            ),
             sorted(self.pages[page.file.url])
         ))
         return (
             markdown +
             f"\n## {self.config['section_title']}\n\n" +
             "\n".join(links)
         )
 
-    def add_category(self, cat_name: str) -> None:
-        """Register a category if it does not yet exist."""
-        if cat_name in self.categories:
-            return
-        slugified = slugify(cat_name)
-        self.categories[cat_name] = {
-            'name':  cat_name,
-            'slug':  slugified,
-            'pages': []
-        }
-        self.log.info('Defined new category "%s" with slug "%s"', cat_name, slugified)
+    def ensure_path(self, cat_path: list[str]) -> dict|None:
+        """Ensure that the category path exists and return the last category."""
+        if len(cat_path) <= 0:
+            return None
+        result = {}
+        for i, cat_name in enumerate(cat_path):
+            cat_key = '-'.join(cat_path[:i + 1])
+            if cat_key not in self.categories:
+                slugified = slugify(cat_key)
+                self.categories[cat_key] = {
+                    'name':     cat_name,
+                    'key':      cat_key,
+                    'slug':     slugify(cat_key),
+                    'pages':    [],
+                    'parent':   '-'.join(cat_path[:i]) if i > 0 else None,
+                    'children': [],
+                }
+                self.log.info(
+                    'Defined new category "%s" with slug "%s"',
+                    cat_path[i],
+                    slugified
+                )
+            if len(result) > 0 and cat_key not in result['children']:
+                result['children'].append(cat_key)
+            result = self.categories[cat_key]
+        return result
 
-    def register_page(self, cat_name: str, page_url: str, page_title: str) -> None:
+    def register_page(self, cat_path: list[str], page_url: str, page_title: str) -> None:
         """Register a page and, if it does not exist, its category."""
         # Each category stores which pages belong to it
-        self.add_category(cat_name)
-        self.categories[cat_name]['pages'].append({
+        category = self.ensure_path(cat_path)
+        category['pages'].append({
             'title': page_title,
             'url':   f"{page_url}{'' if page_url.endswith('/') else '/'}"
         })
 
         # Each page also stores which categories it belongs to
         if page_url not in self.pages:
             self.pages[page_url] = set()
-        self.pages[page_url].add(cat_name)
+        self.pages[page_url].add(category['key'])
 
     def define_categories(self, files) -> None:
         """Read all of the meta data and define any categories."""
         for file in filter(lambda f: f.is_documentation_page(), files):
             with open(file.abs_src_path, encoding='utf-8') as handle:
                 source, meta_data = meta.get_data(handle.read())
                 if len(meta_data) <= 0 or 'categories' not in meta_data:
@@ -141,15 +162,15 @@
                         'The categories object at %s was not a list, but %s',
                         str(file.url),
                         type(meta_data['categories'].__name__)
                     )
                     continue
                 for category in meta_data['categories']:
                     self.register_page(
-                        str(category),
+                        str(category).split(self.config['category_separator']),
                         str(file.url),
                         get_page_title(source, meta_data)
                     )
 
     def generate_index(self, config) -> File:
         """Generates a categories index page if the option is set."""
         joined = "\n".join(map(
@@ -167,40 +188,66 @@
         return File(
             path               = str(self.cat_path / 'index.md'),
             src_dir            = str(self.cat_path.parent),
             dest_dir           = config['site_dir'],
             use_directory_urls = True
         )
 
-    def all_categories_link(self) -> str:
+    def render_all_categories_link(self) -> str:
         """Generates a link to the categories index page if the option is set"""
         return (
             '' if not self.config['generate_index']
             else "[All Categories](../)\n\n"
         )
 
-    def on_files(self, files, config, **_):
+    def render_child_categories(self, category: dict) -> tuple[bool, str]:
+        """Renders the child categories of a category."""
+        if len(category['children']) <= 0:
+            return False, None
+        joined = "\n".join(map(
+            lambda c: f"- [{self.categories[c]['name']}](../{self.categories[c]['slug']}/)",
+            sorted(category['children'])
+        ))
+        return True, joined
+
+    def render_category_pages(self, category: dict) -> tuple[bool, str]:
+        """Renders the pages of a category."""
+        if len(category['pages']) <= 0:
+            return False, None
+        joined = "\n".join(map(
+            lambda p: f"- [{p['title']}](../../{p['url']})",
+            sorted(category['pages'], key=lambda p: p['title'])
+        ))
+        return True, joined
+
+    def render_parent_category(self, category: dict) -> str:
+        """Renders the parent category of a category."""
+        if not category['parent']:
+            return None
+        parent = self.categories[category['parent']]
+        return f"[{parent['name']}](../{parent['slug']})"
+
+    def on_files(self, files, *, config, **_):
         """When MkDocs loads its files, load any defined categories."""
         self.define_categories(files)
         for category in self.categories.values():
-            joined = "\n".join(map(
-                lambda p: f"- [{p['title']}](../../{p['url']})",
-                sorted(category['pages'], key=lambda p: p['title'])
-            ))
-
             file_name = f"{category['slug']}.md"
+            (has_pages, pages) = self.render_category_pages(category)
+            (has_children, children) = self.render_child_categories(category)
+            parent = self.render_parent_category(category)
+
             with open(self.cat_path / file_name, mode="w", encoding='utf-8') as file:
-                file.write(
-                    f"# {category['name']}\n"
-                    "\n"
-                    + self.all_categories_link() +
-                    f"This category contains {len(category['pages'])} page(s):\n"
-                    "\n"
-                    f"{joined}\n"
-                )
+                file.write(''.join([
+                    f"# Category: {category['name']}\n\n",
+                    (f"Parent category: {parent}\n\n" if parent else ''),
+                    (f"##Subcategories\n\n{children}\n\n" if has_children else ''),
+                    f"## Pages in category \"{category['name']}\"\n\n",
+                    f"{pages if has_pages else 'This category has no pages.'}\n\n",
+                    self.render_all_categories_link(),
+                ]))
 
             outfile = File(
                 path               = str(Path(self.config['base_name']) / file_name),
                 src_dir            = str(self.cat_path.parent),
                 dest_dir           = config['site_dir'],
                 use_directory_urls = True
             )
```

### Comparing `mkdocs-categories-plugin-0.2.1/mkdocs_categories_plugin.egg-info/PKG-INFO` & `mkdocs-categories-plugin-0.3.0/mkdocs_categories_plugin.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
 Name: mkdocs-categories-plugin
-Version: 0.2.1
+Version: 0.3.0
 Summary: An MkDocs plugin allowing for categorization of pages
 Home-page: https://github.com/eddyluten/mkdocs-categories-plugin
 Author: Eddy Luten
 Author-email: eddyluten@gmail.com
 License: MIT
 Keywords: mkdocs python markdown category categories link wiki
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.0
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # mkdocs-categories-plugin
 
 [![PyPI version](https://badge.fury.io/py/mkdocs-categories-plugin.svg)](https://pypi.org/project/mkdocs-categories-plugin/)  [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) ![example workflow](https://github.com/eddyluten/mkdocs-categories-plugin/actions/workflows/pylint.yml/badge.svg) [![Downloads](https://pepy.tech/badge/mkdocs-categories-plugin)](https://pepy.tech/project/mkdocs-categories-plugin)
 
 An MkDocs plugin allowing for categorization of pages in your wiki. This plugin allows for multiple categories per page and will generate a category index page with links to each page within the category.
 
 If you like this MkDocs plugin, you'll probably also like [mkdocs-alias-plugin](https://github.com/EddyLuten/mkdocs-alias-plugin).
 
 ## Installation
 
-Install the package using pip:
+Using Python 3.10 or greater, install the package using pip:
 
 ```zsh
 pip install mkdocs-categories-plugin
 ```
 
 Then add the following entry to the plugins section of your `mkdocs.yml` file:
 
@@ -51,30 +51,47 @@
 categories:
     - Novels
     - Fiction
     - 19th Century Gothic Fiction
 ---
 ```
 
-New pages will be generated for each of these categories, with a list of links to each of the wiki pages within the category. The names of these categories are slugified before used in the category URLs. For example, `19th Century Gothic Fiction` becomes `19th-century-gothic-fiction`.
+New pages will be generated for each of these categories, with a list of links to each of the wiki pages within the category. Subcategories, links to the parent category, and a link to the "All Categories" page are automatically generated and placed on the page.
+
+Category names are slugified before used in category URLs. For example, `19th Century Gothic Fiction` becomes `19th-century-gothic-fiction`.
 
 Please refer to the [MkDocs documentation](https://www.mkdocs.org/user-guide/writing-your-docs/#yaml-style-meta-data) for more information on how the meta-data block is used.
 
+### Subcategories
+
+As of version 0.3.0, mkdocs-categories-plugin supports subcategorization. This is achieved by supplying a category name that separates parent from child categories using a separator (by default `|`, configurable via `category_separator`). You may supply as many levels of child categories as you like.
+
+For example:
+
+```yaml
+categories:
+    - Fiction|Romance
+    - Fiction|Books|British Authors|Female|19th Century
+```
+
+The first category definition in this example places the page in the *Romance* subcategory of the *Fiction* parent category. Note that the page will **not** be placed in the parent category of *Fiction*, but only in the *Romance* category. The second category definition places the page in the *19th Century* category, but not in any of its ancestor categories.
+
 ## Options
 
 You may customize the plugin by passing options into the plugin's configuration sections in `mkdocs.yml`:
 
 ```yaml
 plugins:
     - categories:
         generate_index: true
         verbose: false
         base_name: 'categories'
         section_title: 'Categories'
         no_nav: false
+        category_separator: '|'
 ```
 
 ### `generate_index`
 
 **Default:** `true`
 
 If true, an index page listing all of the generated categories is created at the `base_name` URL.
@@ -101,26 +118,36 @@
 
 **Default:** `false`
 
 By default, mkdocs-categories-plugin will generate navigation entries for each category page under the `base_name` that you provided. If you want to turn this behavior off, set this option to `true`.
 
 There's also a know issue with mkdocs-awesome-pages-plugin compatibility that does not allow you to reorder the position of the generated categories section by using a `.pages` file. If you would rather turn the navigation entries off entirely, this option is for you.
 
+### `category_separator`
+
+**Default:** `|`
+
+This string is used to split the category name in order to define a category hierarchy (see subcategories above).
+
 ## Troubleshooting
 
 ### There's a directory named `categories` in my project
 
 A fatal error must have occurred during the compilation of your site and left the temporary directory containing the intermediate markdown files used by this plugin behind. It is safe to delete this directory since it's only used during the build.
 
 ### `The categories object at URL was not a list, but TYPE`
 
 The page identified did not contain a valid categories configuration object. Please make sure that this is an array of strings.
 
 ## Changelog
 
+### 0.3.0
+
+Added support for subcategories. Python 3.10 or higher is now required.
+
 ### 0.2.1
 
 Patch release: implements a bug fix by @rpmzandwijk reported in [#1](https://github.com/EddyLuten/mkdocs-categories-plugin/issues/1).
 
 ### 0.2.0
 
 Introduces support for the automatic generation of category index pages. This new default behavior can be turned off using an option.
```

### Comparing `mkdocs-categories-plugin-0.2.1/setup.py` & `mkdocs-categories-plugin-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 from setuptools import setup, find_packages
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name='mkdocs-categories-plugin',
-    version='0.2.1',
+    version='0.3.0',
     description=
     'An MkDocs plugin allowing for categorization of pages',
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords='mkdocs python markdown category categories link wiki',
     url='https://github.com/eddyluten/mkdocs-categories-plugin',
     author='Eddy Luten',
     author_email='eddyluten@gmail.com',
     license='MIT',
-    python_requires='>=3.0',
+    python_requires='>=3.10',
     install_requires=['mkdocs'],
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3 :: Only',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
```

