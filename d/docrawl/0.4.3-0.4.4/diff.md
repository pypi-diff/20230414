# Comparing `tmp/docrawl-0.4.3.tar.gz` & `tmp/docrawl-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docrawl-0.4.3.tar", last modified: Sun Apr  2 22:03:58 2023, max compression
+gzip compressed data, was "docrawl-0.4.4.tar", last modified: Fri Apr 14 06:40:27 2023, max compression
```

## Comparing `docrawl-0.4.3.tar` & `docrawl-0.4.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-02 22:03:57.995483 docrawl-0.4.3/
--rw-rw-rw-   0        0        0     1090 2021-08-16 12:38:07.000000 docrawl-0.4.3/LICENSE
--rw-rw-rw-   0        0        0      568 2023-04-02 22:03:57.995483 docrawl-0.4.3/PKG-INFO
--rw-rw-rw-   0        0        0       86 2021-08-16 12:38:07.000000 docrawl-0.4.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-02 22:03:57.975495 docrawl-0.4.3/docrawl/
--rw-rw-rw-   0        0        0        0 2021-08-16 12:40:29.000000 docrawl-0.4.3/docrawl/__init__.py
--rw-rw-rw-   0        0        0    40393 2023-04-02 22:03:21.000000 docrawl-0.4.3/docrawl/docrawl_core.py
--rw-rw-rw-   0        0        0     6355 2023-04-02 21:36:25.000000 docrawl-0.4.3/docrawl/docrawl_launcher.py
--rw-rw-rw-   0        0        0     1108 2023-02-25 18:40:39.000000 docrawl-0.4.3/docrawl/docrawl_logger.py
-drwxrwxrwx   0        0        0        0 2023-04-02 22:03:57.995483 docrawl-0.4.3/docrawl.egg-info/
--rw-rw-rw-   0        0        0      568 2023-04-02 22:03:57.000000 docrawl-0.4.3/docrawl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2023-04-02 22:03:57.000000 docrawl-0.4.3/docrawl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-02 22:03:57.000000 docrawl-0.4.3/docrawl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2023-04-02 22:03:57.000000 docrawl-0.4.3/docrawl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-02 22:03:57.000000 docrawl-0.4.3/docrawl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-02 22:03:57.995483 docrawl-0.4.3/setup.cfg
--rw-rw-rw-   0        0        0      834 2023-04-02 22:03:54.000000 docrawl-0.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 06:40:27.779397 docrawl-0.4.4/
+-rw-rw-rw-   0        0        0     1090 2021-08-16 12:38:07.000000 docrawl-0.4.4/LICENSE
+-rw-rw-rw-   0        0        0      568 2023-04-14 06:40:27.779397 docrawl-0.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2021-08-16 12:38:07.000000 docrawl-0.4.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 06:40:27.763440 docrawl-0.4.4/docrawl/
+-rw-rw-rw-   0        0        0        0 2021-08-16 12:40:29.000000 docrawl-0.4.4/docrawl/__init__.py
+-rw-rw-rw-   0        0        0    40996 2023-04-14 06:39:31.000000 docrawl-0.4.4/docrawl/docrawl_core.py
+-rw-rw-rw-   0        0        0     6355 2023-04-02 21:36:25.000000 docrawl-0.4.4/docrawl/docrawl_launcher.py
+-rw-rw-rw-   0        0        0     1108 2023-02-25 18:40:39.000000 docrawl-0.4.4/docrawl/docrawl_logger.py
+drwxrwxrwx   0        0        0        0 2023-04-14 06:40:27.778399 docrawl-0.4.4/docrawl.egg-info/
+-rw-rw-rw-   0        0        0      568 2023-04-14 06:40:27.000000 docrawl-0.4.4/docrawl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2023-04-14 06:40:27.000000 docrawl-0.4.4/docrawl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 06:40:27.000000 docrawl-0.4.4/docrawl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2023-04-14 06:40:27.000000 docrawl-0.4.4/docrawl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-14 06:40:27.000000 docrawl-0.4.4/docrawl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-14 06:40:27.779397 docrawl-0.4.4/setup.cfg
+-rw-rw-rw-   0        0        0      834 2023-04-14 06:40:23.000000 docrawl-0.4.4/setup.py
```

### Comparing `docrawl-0.4.3/LICENSE` & `docrawl-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `docrawl-0.4.3/PKG-INFO` & `docrawl-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docrawl
-Version: 0.4.3
+Version: 0.4.4
 Summary: Do automated crawling of pages using scrapy
 Home-page: https://github.com/DovaX/docrawl
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `docrawl-0.4.3/docrawl/docrawl_core.py` & `docrawl-0.4.4/docrawl/docrawl_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -276,18 +276,23 @@
             elems_pos.append({'rect': selector.rect,
                               'name': name,
                               'xpath': xpath,
                               'data': data})
 
             existing_xpaths.append(xpath)
 
-        elements_positions = elems_pos
-        elements_positions = VarSafe(elements_positions, 'elements_positions', 'elements_positions')
+        
 
-        save_variables(kept_variables, 'elements_positions.kpv')
+        elements_positions = {"elements_positions":elems_pos}
+        filename="elements_positions.kpv"
+        with open(filename,"w+", encoding="utf8",errors='ignore') as file: #TODO: improve KPV to enable multiple keep variable files -> it collided with browser_metadata_kpv,
+            file.write(str(elements_positions))
+            
+        #elements_positions = VarSafe(elements_positions, 'elements_positions', 'elements_positions')
+        #save_variables(kept_variables, 'elements_positions.kpv')
 
     def serialize_and_append_data(element_name, selector, xpath):
         """
         Serializes data behind the element and updates dictionary with final elements
             :param element_name: variable name to save
             :param selector: Selenium Selector
             :param xpath: XPath of element
@@ -412,16 +417,20 @@
             if len(data) > 0:
                 with open(path + '.pickle', 'wb') as pickle_file:
                     pickle.dump(data, pickle_file)
 
         if 'context' in element_name:
             data = None
         else:
-            data = pickle_file.name
-
+            try:
+                data = pickle_file.name
+            except Exception as e:
+                data = None
+                print(e)
+        
         final_elements.update({element_name:
                                    {'selector': selector,
                                     'data': data,
                                     'xpath': xpath}})
 
     def find_elements(tags, element_name, custom_tag=False):
         """
@@ -453,16 +462,17 @@
                 if element_name == 'table' and len(element.find_elements(By.XPATH, './/tr')) < 2:
                     continue
 
                 try:
                     xpath = find_element_xpath(elements_tree, i)
                     serialize_and_append_data(f'{element_name}_{i}', element, xpath)
 
-                except:
-                    pass
+                except Exception as e:
+                    print(e)
+                #    pass
 
     def find_element_xpath(tree, i):
         """
         Finds the XPath of element using HTML parser.
             :param tree: list of elements
             :param i: element's number
         """
@@ -527,15 +537,18 @@
                     break
 
             element_name = f'{element_name}_{i}'
 
             find_elements(custom_tag, element_name, custom_tag=True)
 
     if context_xpath:
-        find_elements([context_xpath], 'context', custom_tag=True)
+        try:
+            find_elements([context_xpath], 'context', custom_tag=True)
+        except Exception as e:
+            print(e)
 
     ##### SAVING COORDINATES OF ELEMENTS #####
 
     names = list(final_elements.keys())
     selectors = [x['selector'] for x in final_elements.values()]
     xpaths = [x['xpath'] for x in final_elements.values()]
     data = [x['data'] for x in final_elements.values()]
@@ -903,17 +916,18 @@
         'USER_AGENT': "Mozilla/5.0 (Windows NT 6.2; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/27.0.1453.93 Safari/537.36",
         'DEFAULT_REQUEST_HEADERS': {
             'Referer': 'https://forloop.ai'
         }
         #   'CONCURRENT_REQUESTS' : '20',
     }
 
-    def __init__(self):
+    def __init__(self, *a, **kw):
         # can be replaced for debugging with browser = webdriver.FireFox()
         # self.browser = webdriver.PhantomJS(executable_path=PHANTOMJS_PATH, service_args=['--ignore-ssl-errors=true'])
+        #super().__init__(*a, **kw)
         self.meta_data = BrowserMetaData()
 
         self.browser = self._initialise_browser()
 
         browser_info = {
             'driver': self.driver_type,
             'headless': self.headless,
```

### Comparing `docrawl-0.4.3/docrawl/docrawl_launcher.py` & `docrawl-0.4.4/docrawl/docrawl_launcher.py`

 * *Files identical despite different names*

### Comparing `docrawl-0.4.3/docrawl/docrawl_logger.py` & `docrawl-0.4.4/docrawl/docrawl_logger.py`

 * *Files identical despite different names*

### Comparing `docrawl-0.4.3/docrawl.egg-info/PKG-INFO` & `docrawl-0.4.4/docrawl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docrawl
-Version: 0.4.3
+Version: 0.4.4
 Summary: Do automated crawling of pages using scrapy
 Home-page: https://github.com/DovaX/docrawl
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `docrawl-0.4.3/setup.py` & `docrawl-0.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
     
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name='docrawl',
-    version='0.4.3',
+    version='0.4.4',
     author='DovaX',
     author_email='dovax.ai@gmail.com',
     description='Do automated crawling of pages using scrapy',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/DovaX/docrawl',
     packages=setuptools.find_packages(),
```

