# Comparing `tmp/phoebusgen-2.4.5.tar.gz` & `tmp/phoebusgen-2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phoebusgen-2.4.5.tar", last modified: Mon Jul 25 02:10:07 2022, max compression
+gzip compressed data, was "phoebusgen-2.5.tar", last modified: Thu Apr 13 23:45:52 2023, max compression
```

## Comparing `phoebusgen-2.4.5.tar` & `phoebusgen-2.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-25 02:10:07.229543 phoebusgen-2.4.5/
--rw-r--r--   0 runner    (1001) docker     (121)    17987 2022-07-25 02:09:51.000000 phoebusgen-2.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      209 2022-07-25 02:09:51.000000 phoebusgen-2.4.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4783 2022-07-25 02:10:07.229543 phoebusgen-2.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4210 2022-07-25 02:09:51.000000 phoebusgen-2.4.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-25 02:10:07.229543 phoebusgen-2.4.5/phoebusgen/
--rw-r--r--   0 runner    (1001) docker     (121)     4515 2022-07-25 02:09:51.000000 phoebusgen-2.4.5/phoebusgen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8107 2022-07-25 02:09:51.000000 phoebusgen-2.4.5/phoebusgen/_shared_property_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-07-25 02:10:07.229543 phoebusgen-2.4.5/phoebusgen/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-25 02:10:07.229543 phoebusgen-2.4.5/phoebusgen/config/
--rw-r--r--   0 runner    (1001) docker     (121)     3150 2022-07-25 02:09:51.000000 phoebusgen-2.4.5/phoebusgen/config/classes.bcf
--rw-r--r--   0 runner    (1001) docker     (121)     1911 2022-07-25 02:09:51.000000 phoebusgen-2.4.5/phoebusgen/config/color.def
--rw-r--r--   0 runner    (1001) docker     (121)     2105 2022-07-25 02:09:51.000000 phoebusgen-2.4.5/phoebusgen/config/font.def
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-25 02:10:07.229543 phoebusgen-2.4.5/phoebusgen/screen/
--rw-r--r--   0 runner    (1001) docker     (121)     1237 2022-07-25 02:09:51.000000 phoebusgen-2.4.5/phoebusgen/screen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4372 2022-07-25 02:09:51.000000 phoebusgen-2.4.5/phoebusgen/screen/screen.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-25 02:10:07.229543 phoebusgen-2.4.5/phoebusgen/widget/
--rw-r--r--   0 runner    (1001) docker     (121)     1273 2022-07-25 02:09:51.000000 phoebusgen-2.4.5/phoebusgen/widget/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    65736 2022-07-25 02:09:51.000000 phoebusgen-2.4.5/phoebusgen/widget/properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     9065 2022-07-25 02:09:51.000000 phoebusgen-2.4.5/phoebusgen/widget/widget.py
--rw-r--r--   0 runner    (1001) docker     (121)    27624 2022-07-25 02:09:51.000000 phoebusgen-2.4.5/phoebusgen/widget/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-25 02:10:07.229543 phoebusgen-2.4.5/phoebusgen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4783 2022-07-25 02:10:07.000000 phoebusgen-2.4.5/phoebusgen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      562 2022-07-25 02:10:07.000000 phoebusgen-2.4.5/phoebusgen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-25 02:10:07.000000 phoebusgen-2.4.5/phoebusgen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-07-25 02:10:07.000000 phoebusgen-2.4.5/phoebusgen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-25 02:09:51.000000 phoebusgen-2.4.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      198 2022-07-25 02:10:07.229543 phoebusgen-2.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1020 2022-07-25 02:09:51.000000 phoebusgen-2.4.5/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    81180 2022-07-25 02:09:51.000000 phoebusgen-2.4.5/versioneer.py
+drwxr-xr-x   0 tford     (1000) tford     (1000)        0 2023-04-13 23:45:52.409371 phoebusgen-2.5/
+-rw-rw-r--   0 tford     (1000) tford     (1000)    17987 2022-05-20 06:18:45.000000 phoebusgen-2.5/LICENSE
+-rw-rw-r--   0 tford     (1000) tford     (1000)      209 2022-05-20 06:18:45.000000 phoebusgen-2.5/MANIFEST.in
+-rw-r--r--   0 tford     (1000) tford     (1000)     4778 2023-04-13 23:45:52.409371 phoebusgen-2.5/PKG-INFO
+-rw-rw-r--   0 tford     (1000) tford     (1000)     4207 2023-04-12 05:14:47.000000 phoebusgen-2.5/README.md
+drwxr-xr-x   0 tford     (1000) tford     (1000)        0 2023-04-13 23:45:52.409371 phoebusgen-2.5/phoebusgen/
+-rw-rw-r--   0 tford     (1000) tford     (1000)     4515 2023-04-12 05:20:14.000000 phoebusgen-2.5/phoebusgen/__init__.py
+-rw-rw-r--   0 tford     (1000) tford     (1000)     8107 2022-06-28 02:59:04.000000 phoebusgen-2.5/phoebusgen/_shared_property_helpers.py
+-rw-r--r--   0 tford     (1000) tford     (1000)      495 2023-04-13 23:45:52.409371 phoebusgen-2.5/phoebusgen/_version.py
+drwxr-xr-x   0 tford     (1000) tford     (1000)        0 2023-04-13 23:45:52.407370 phoebusgen-2.5/phoebusgen/config/
+-rw-rw-r--   0 tford     (1000) tford     (1000)     3150 2022-05-20 06:18:45.000000 phoebusgen-2.5/phoebusgen/config/classes.bcf
+-rw-rw-r--   0 tford     (1000) tford     (1000)     1911 2022-05-20 06:18:45.000000 phoebusgen-2.5/phoebusgen/config/color.def
+-rw-rw-r--   0 tford     (1000) tford     (1000)     2103 2023-04-12 05:14:47.000000 phoebusgen-2.5/phoebusgen/config/font.def
+drwxr-xr-x   0 tford     (1000) tford     (1000)        0 2023-04-13 23:45:52.408370 phoebusgen-2.5/phoebusgen/screen/
+-rw-rw-r--   0 tford     (1000) tford     (1000)     1237 2023-04-12 05:20:13.000000 phoebusgen-2.5/phoebusgen/screen/__init__.py
+-rw-rw-r--   0 tford     (1000) tford     (1000)     4372 2023-04-12 05:20:13.000000 phoebusgen-2.5/phoebusgen/screen/screen.py
+drwxr-xr-x   0 tford     (1000) tford     (1000)        0 2023-04-13 23:45:52.408370 phoebusgen-2.5/phoebusgen/widget/
+-rw-rw-r--   0 tford     (1000) tford     (1000)     1273 2023-04-12 05:20:14.000000 phoebusgen-2.5/phoebusgen/widget/__init__.py
+-rw-rw-r--   0 tford     (1000) tford     (1000)    65736 2023-04-12 05:20:14.000000 phoebusgen-2.5/phoebusgen/widget/properties.py
+-rw-rw-r--   0 tford     (1000) tford     (1000)     9033 2023-04-13 22:44:54.000000 phoebusgen-2.5/phoebusgen/widget/widget.py
+-rw-rw-r--   0 tford     (1000) tford     (1000)    27623 2023-04-12 05:14:47.000000 phoebusgen-2.5/phoebusgen/widget/widgets.py
+drwxr-xr-x   0 tford     (1000) tford     (1000)        0 2023-04-13 23:45:52.407370 phoebusgen-2.5/phoebusgen.egg-info/
+-rw-r--r--   0 tford     (1000) tford     (1000)     4778 2023-04-13 23:45:52.000000 phoebusgen-2.5/phoebusgen.egg-info/PKG-INFO
+-rw-r--r--   0 tford     (1000) tford     (1000)      562 2023-04-13 23:45:52.000000 phoebusgen-2.5/phoebusgen.egg-info/SOURCES.txt
+-rw-r--r--   0 tford     (1000) tford     (1000)        1 2023-04-13 23:45:52.000000 phoebusgen-2.5/phoebusgen.egg-info/dependency_links.txt
+-rw-r--r--   0 tford     (1000) tford     (1000)       11 2023-04-13 23:45:52.000000 phoebusgen-2.5/phoebusgen.egg-info/top_level.txt
+-rw-rw-r--   0 tford     (1000) tford     (1000)        0 2022-05-20 06:18:45.000000 phoebusgen-2.5/requirements.txt
+-rw-rw-r--   0 tford     (1000) tford     (1000)      198 2023-04-13 23:45:52.409371 phoebusgen-2.5/setup.cfg
+-rw-rw-r--   0 tford     (1000) tford     (1000)     1019 2023-04-12 05:20:14.000000 phoebusgen-2.5/setup.py
+-rw-rw-r--   0 tford     (1000) tford     (1000)    81180 2023-04-12 05:20:14.000000 phoebusgen-2.5/versioneer.py
```

### Comparing `phoebusgen-2.4.5/LICENSE` & `phoebusgen-2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.4.5/PKG-INFO` & `phoebusgen-2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phoebusgen
-Version: 2.4.5
+Version: 2.5
 Summary: Control screen generator for Phoebus
 Home-page: https://github.com/tynanford/phoebusgen
 Author: Tynan Ford
 Author-email: tford@lbl.gov
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
@@ -66,15 +66,15 @@
   <font>
     <font family="Liberation Sans" size="14" style="BOLD"/>
   </font>
 </widget>
 
 ```
 
-## Modules 
+## Modules
 
 ### phoebusgen.widget
 
 Python API to directly create Phoebus widgets. All standard Phoebus widgets are available, but some (3) are not fully feature complete.
 
 [Widgets Docs](https://als-epics.github.io/phoebusgen/source/phoebusgen.widget.html#module-phoebusgen.widget.widgets)
 
@@ -82,15 +82,15 @@
 -   Image
 -   Strip Chart
 -   X/Y Plot
 
 Example
 -   ```text_update_xml = phoebusgen.widget.TextUpdate(widget_name, pv_name, x, y, width, height)```
 
-### phoebusgen.screen 
+### phoebusgen.screen
 
 Python object to represent a Phoebus screen. Widgets can be added to the screen object and the screen object can be written to a .bob file to be opened in Phoebus.
 
 [Screen Docs](https://als-epics.github.io/phoebusgen/source/phoebusgen.screen.html#module-phoebusgen.screen.screen)
 
 Example
 ```pycon
@@ -118,15 +118,15 @@
     <pv_name>test:PV</pv_name>
   </widget>
 </display>
 ```
 
 ## Site specific color and font definitions
 
-Place a custon color.def or font.def in ~/.phoebusgen/ to force phoebusgen.colors or phoebusgen.fonts to reflect your site's custom definitions. 
+Place a custon color.def or font.def in ~/.phoebusgen/ to force phoebusgen.colors or phoebusgen.fonts to reflect your site's custom definitions.
 
 ```python
 my_widget.predefined_font(phoebusgen.fonts.Header1)
 ```
 ```python
 my_widget.predefined_color(phoebusgen.colors.OK)
 ```
```

### Comparing `phoebusgen-2.4.5/README.md` & `phoebusgen-2.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
   <font>
     <font family="Liberation Sans" size="14" style="BOLD"/>
   </font>
 </widget>
 
 ```
 
-## Modules 
+## Modules
 
 ### phoebusgen.widget
 
 Python API to directly create Phoebus widgets. All standard Phoebus widgets are available, but some (3) are not fully feature complete.
 
 [Widgets Docs](https://als-epics.github.io/phoebusgen/source/phoebusgen.widget.html#module-phoebusgen.widget.widgets)
 
@@ -66,15 +66,15 @@
 -   Image
 -   Strip Chart
 -   X/Y Plot
 
 Example
 -   ```text_update_xml = phoebusgen.widget.TextUpdate(widget_name, pv_name, x, y, width, height)```
 
-### phoebusgen.screen 
+### phoebusgen.screen
 
 Python object to represent a Phoebus screen. Widgets can be added to the screen object and the screen object can be written to a .bob file to be opened in Phoebus.
 
 [Screen Docs](https://als-epics.github.io/phoebusgen/source/phoebusgen.screen.html#module-phoebusgen.screen.screen)
 
 Example
 ```pycon
@@ -102,15 +102,15 @@
     <pv_name>test:PV</pv_name>
   </widget>
 </display>
 ```
 
 ## Site specific color and font definitions
 
-Place a custon color.def or font.def in ~/.phoebusgen/ to force phoebusgen.colors or phoebusgen.fonts to reflect your site's custom definitions. 
+Place a custon color.def or font.def in ~/.phoebusgen/ to force phoebusgen.colors or phoebusgen.fonts to reflect your site's custom definitions.
 
 ```python
 my_widget.predefined_font(phoebusgen.fonts.Header1)
 ```
 ```python
 my_widget.predefined_color(phoebusgen.colors.OK)
 ```
```

### Comparing `phoebusgen-2.4.5/phoebusgen/__init__.py` & `phoebusgen-2.5/phoebusgen/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     #print('Using color.def file at: {}'.format(file_path))
     predefined_colors = {}
     if not _path.isfile(file_path):
         print('File at this path does not exist: {}'.format(file_path))
     with open(file_path, 'r') as color_file:
         for line in color_file:
             line = line.partition('#')[0].rstrip()
-            if line != "":
+            if line != '':
                 color, value = line.split('=')
                 color = color.strip()
                 vals = [v.strip() for v in value.split(',')]
                 if len(vals) == 1:
                     predefined_colors[color] = predefined_colors[vals[0]]
                 else:
                     if len(vals) == 4:
@@ -67,15 +67,15 @@
             os = 'linux'
         elif 'darwin' in os:
             os = 'macosx'
         elif 'win' in os:
             os = 'windows'
         for line in font_file:
             line = line.partition('//')[0].rstrip()
-            if line != "":
+            if line != '':
                 font, value = line.split('=')
                 font = font.strip()
                 os_name = _re.search('\(([^)]+)', font)
                 if os_name:
                     os_name = os_name.group(1)
                     if os_name != os:
                         continue
```

### Comparing `phoebusgen-2.4.5/phoebusgen/_shared_property_helpers.py` & `phoebusgen-2.5/phoebusgen/_shared_property_helpers.py`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.4.5/phoebusgen/config/classes.bcf` & `phoebusgen-2.5/phoebusgen/config/classes.bcf`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.4.5/phoebusgen/config/color.def` & `phoebusgen-2.5/phoebusgen/config/color.def`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.4.5/phoebusgen/config/font.def` & `phoebusgen-2.5/phoebusgen/config/font.def`

 * *Files 0% similar despite different names*

```diff
@@ -51,9 +51,7 @@
 Oddball = Comic Sans MS-regular-40
 
 // On Linux resp. MacOS, these will be used instead,
 // replacnig the definition shown above.
 // Operating system selectors are: "windows", "linux", "macosx"
 Oddball(linux) = PakTypeNaqsh-regular-40
 Oddball(macosx) = Herculanum-regular-40
-
-
```

### Comparing `phoebusgen-2.4.5/phoebusgen/screen/__init__.py` & `phoebusgen-2.5/phoebusgen/screen/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,8 +33,8 @@
 """
 
 # Copyright (c) 2022 Lawrence Berkeley National Laboratory,
 # Advanced Light Source, Engineering Division
 
 from phoebusgen.screen.screen import *
 
-__all__ = ["screen"]
+__all__ = ['screen']
```

### Comparing `phoebusgen-2.4.5/phoebusgen/screen/screen.py` & `phoebusgen-2.5/phoebusgen/screen/screen.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 def prettify(elem):
     """Return a pretty-printed XML string for the Element.
         From: https://pymotw.com/3/xml.etree.ElementTree/create.html
     """
     rough_string = tostring(elem, 'utf-8')
     reparse_xml = minidom.parseString(rough_string)
-    return reparse_xml.toprettyxml(indent="  ", newl="\n")
+    return reparse_xml.toprettyxml(indent='  ', newl='\n')
 
 
 class Screen(object):
     """ Phoebus Screen object that holds widgets and can be written to .bob file """
     def __init__(self, name: str, f_name: str = None) -> None:
         """
         Create Phoebus screen object. File name is optional and can be specified later
@@ -40,15 +40,15 @@
         if file_name is None:
             file_name = self.bob_file
         if file_name is None:
             print('Output Phoebus file name is not set! First set bob_file or use file_name parameter')
             return False
         else:
             with open(file_name, 'w') as f:
-                reparse_xml.writexml(f, indent="  ", addindent="  ", newl="\n", encoding="UTF-8")
+                reparse_xml.writexml(f, indent='  ', addindent='  ', newl='\n', encoding='UTF-8')
             return True
 
     def find_widget(self, widget_tag_name: str) -> Element:
         """
         Find widget in the screen
 
         :param widget_tag_name: Tag name of widget to find
```

### Comparing `phoebusgen-2.4.5/phoebusgen/widget/__init__.py` & `phoebusgen-2.5/phoebusgen/widget/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,8 +29,8 @@
 """
 
 # Copyright (c) 2022 Lawrence Berkeley National Laboratory,
 # Advanced Light Source, Engineering Division
 
 from phoebusgen.widget.widgets import *
 
-__all__ = ["widgets"]
+__all__ = ['widgets']
```

### Comparing `phoebusgen-2.4.5/phoebusgen/widget/properties.py` & `phoebusgen-2.5/phoebusgen/widget/properties.py`

 * *Files 1% similar despite different names*

```diff
@@ -715,15 +715,15 @@
             root_action = SubElement(self.root, 'actions')
         action = SubElement(root_action, 'action')
         action.attrib['type'] = action_type
         sub = SubElement(action, 'description')
         sub.text = str(description)
         if macros:
             if not isinstance(macros, dict):
-                print("macros parameter must be of type dict, not: {}".format(type(macros)))
+                print('macros parameter must be of type dict, not: {}'.format(type(macros)))
             else:
                 for key, val in macros.items():
                     self._shared.add_macro(key, val, action)
         for arg, val in args.items():
             sub = SubElement(action, arg)
             sub.text = str(val)
 
@@ -1364,37 +1364,37 @@
 
         :param name: Tab name, should be unique
         """
         root_tab = self.root.find('tabs')
         if root_tab is None:
             root_tab = SubElement(self.root, 'tabs')
         tab_elem = SubElement(root_tab, 'tab')
-        name_elem = SubElement(tab_elem, "name")
+        name_elem = SubElement(tab_elem, 'name')
         name_elem.text = name
-        SubElement(tab_elem, "children")
+        SubElement(tab_elem, 'children')
 
     def add_widget(self, tab_name: str, elem: object) -> None:
         """
         Add widget to a specific tab with given tab_name
 
         :param tab_name: Name of the tab to add widget to
         :param elem: <Phoebusgen.widget> Widget to add to tab
         """
         root_tab = self.root.find('tabs')
         if root_tab is None:
-            print("No tabs widget available!")
+            print('No tabs widget available!')
         else:
             tab_elem_list = root_tab.findall('tab')
             foundIt = False
             for tab in tab_elem_list:
                 if tab.find('name').text == tab_name:
                     tab.find('children').append(elem.root)
                     foundIt = True
             if not foundIt:
-                print("No tab with the given name: {}".format(tab_name))
+                print('No tab with the given name: {}'.format(tab_name))
 
 class _NavTabs(object):
     def tab(self, name: str, file_name: str, group_name: str, macros: dict = None) -> None:
         """
         Add tab to the Navigation Tab widget. Nav tabs use bob files. Macro arg is optional
 
         :param name: Tab name
@@ -1402,21 +1402,21 @@
         :param group_name: Tab group name
         :param macros: Dictionary of macros. key=macro name and value=macro value
         """
         root_tab = self.root.find('tabs')
         if root_tab is None:
             root_tab = SubElement(self.root, 'tabs')
         tab_elem = SubElement(root_tab, 'tab')
-        self._shared.generic_property(tab_elem, "name", name)
-        self._shared.generic_property(tab_elem, "file", file_name)
-        self._shared.generic_property(tab_elem, "group_name", group_name)
-        SubElement(tab_elem, "macros")
+        self._shared.generic_property(tab_elem, 'name', name)
+        self._shared.generic_property(tab_elem, 'file', file_name)
+        self._shared.generic_property(tab_elem, 'group_name', group_name)
+        SubElement(tab_elem, 'macros')
         if macros is not None:
             if not isinstance(macros, dict):
-                print("macros parameter must be of type dict, not: {}".format(type(macros)))
+                print('macros parameter must be of type dict, not: {}'.format(type(macros)))
             else:
                 for key, val in macros.items():
                     self._shared.add_macro(key, val, tab_elem)
 
 class _ActiveTab(object):
     def active_tab(self, tab_num: int) -> None:
         """
@@ -1497,25 +1497,25 @@
     def labels(self, label_list_or_name: Union[list, str]) -> None:
         """
         Add label property to widget
 
         :param label_list_or_name: List of label strings or a single label string
         """
         if not isinstance(label_list_or_name, list) and not isinstance(label_list_or_name, str):
-            print("Parameter to labels must be a list of strings or a single string, not: {}".format(type(label_list_or_name)))
+            print('Parameter to labels must be a list of strings or a single string, not: {}'.format(type(label_list_or_name)))
         else:
             root_label_tag = self.root.find('labels')
             if root_label_tag is None:
                 root_label_tag = SubElement(self.root, 'labels')
             if isinstance(label_list_or_name, list):
                 for label in label_list_or_name:
-                    label_elem = SubElement(root_label_tag, "text")
+                    label_elem = SubElement(root_label_tag, 'text')
                     label_elem.text = label
             else:
-                self._shared.generic_property(root_label_tag, "text", label_list_or_name)
+                self._shared.generic_property(root_label_tag, 'text', label_list_or_name)
 
 class _ArrayIndex(object):
     def array_index(self, index: int) -> None:
         """
         Add array index to widget
 
         :param index: Array index
@@ -1526,25 +1526,25 @@
     def symbols(self, symbol_list_or_string: Union[list, str]) -> None:
         """
         Add symbol to widget. Symbols can be file name or text symbol
 
         :param symbol_list_or_string: List of strings/file names or single string/file name
         """
         if not isinstance(symbol_list_or_string, list) and not isinstance(symbol_list_or_string, str):
-            print("Parameter to labels must be a list of strings or a single string, not: {}".format(type(symbol_list_or_string)))
+            print('Parameter to labels must be a list of strings or a single string, not: {}'.format(type(symbol_list_or_string)))
         else:
             root_label_tag = self.root.find('symbols')
             if root_label_tag is None:
                 root_label_tag = SubElement(self.root, 'symbols')
             if isinstance(symbol_list_or_string, list):
                 for label in symbol_list_or_string:
-                    label_elem = SubElement(root_label_tag, "symbol")
+                    label_elem = SubElement(root_label_tag, 'symbol')
                     label_elem.text = label
             else:
-                self._shared.generic_property(root_label_tag, "symbol", symbol_list_or_string)
+                self._shared.generic_property(root_label_tag, 'symbol', symbol_list_or_string)
 
 class _InitialIndex(object):
     def initial_index(self, index: int) -> None:
         """
         Add initial index to widget
 
         :param index: Index
@@ -1758,35 +1758,35 @@
         Add column property to widget
 
         :param name: Name of column
         :param width: Column width
         :param editable: Is column editable?
         :param options: List of strings or single string
         """
-        columns_root = self.root.find("columns")
+        columns_root = self.root.find('columns')
         if columns_root is None:
-            columns_root = SubElement(self.root, "columns")
-        column_elem = SubElement(columns_root, "column")
-        self._shared.generic_property(column_elem, "name", name)
-        self._shared.integer_property(column_elem, "width", width)
-        self._shared.boolean_property(column_elem, "editable", editable)
+            columns_root = SubElement(self.root, 'columns')
+        column_elem = SubElement(columns_root, 'column')
+        self._shared.generic_property(column_elem, 'name', name)
+        self._shared.integer_property(column_elem, 'width', width)
+        self._shared.boolean_property(column_elem, 'editable', editable)
         if options is None:
             return
         elif not isinstance(options, list) and not isinstance(options, str):
-            print("options parameter must be a list of strings or a single string")
+            print('options parameter must be a list of strings or a single string')
             return
-        options_root = column_elem.find("options")
+        options_root = column_elem.find('options')
         if options_root is None:
-            options_root = SubElement(column_elem, "options")
+            options_root = SubElement(column_elem, 'options')
         if isinstance(options, list):
             for opt in options:
-                option_elem = SubElement(options_root, "option")
+                option_elem = SubElement(options_root, 'option')
                 option_elem.text = opt
         else:
-            self._shared.generic_property(options_root, "option", options)
+            self._shared.generic_property(options_root, 'option', options)
 
 class _Title(object):
     def title(self, title: str) -> None:
         """
         Add title to widget
 
         :param title: Title
```

### Comparing `phoebusgen-2.4.5/phoebusgen/widget/widget.py` & `phoebusgen-2.5/phoebusgen/widget/widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 def prettify(elem):
     """Return a pretty-printed XML string for the Element.
         From: https://pymotw.com/3/xml.etree.ElementTree/create.html
     """
     rough_string = tostring(elem, 'utf-8')
     reparse_xml = minidom.parseString(rough_string)
-    return reparse_xml.toprettyxml(indent="  ", newl="\n")
+    return reparse_xml.toprettyxml(indent='  ', newl='\n')
 
 
 class _Widget(object):
     """ Base Class for all Phoebus widgets """
     def __init__(self, w_type: str, name: str, x_pos: int, y_pos: int, width: int, height: int) -> None:
         """
         Base Class for all Phoebus widgets
@@ -108,27 +108,26 @@
         root_rules = self.root.find('rules')
         if root_rules is None:
             root_rules = SubElement(self.root, 'rules')
         root_rule = SubElement(root_rules, 'rule')
         root_rule.attrib['name'] = name
         root_rule.attrib['prop_id'] = widget_property
         if value_as_expression is True:
-            root_rule.attrib['out_exp'] = "true"
+            root_rule.attrib['out_exp'] = 'true'
         else:
-            root_rule.attrib['out_exp'] = "false"
+            root_rule.attrib['out_exp'] = 'false'
         if expression_dict is not None:
             for expression, value in expression_dict.items():
-                print(expression, value)
                 expression_element = SubElement(root_rule, 'exp', {'bool_exp': expression})
                 if value_as_expression is True:
                     val_as_exp_element = SubElement(expression_element, 'expression')
-                    val_as_exp_element.text = value
+                    val_as_exp_element.text = str(value)
                 else:
                     val_element = SubElement(expression_element, 'value')
-                    val_element.text = value
+                    val_element.text = str(value)
         if pv_dict is not None:
             for pv, trigger in pv_dict.items():
                 pv_element = SubElement(root_rule, 'pv_name', {'trigger': str(trigger).lower()})
                 pv_element.text = pv
 
     def _script(self, file_name, script_contents, pv_dict, only_trigger_if_connected):
         root_scripts = self.root.find('scripts')
@@ -151,26 +150,26 @@
         """
         Add an embedded Jython (Python) script to the widget
 
         :param python_script: Usually multi-line string representing the actual python code to attach to widget
         :param pv_dict: Dictionary of PVs for the script, format - { pvName: triggerOnPV }
         :param only_trigger_if_connected: Defaults to True. If False, script will run even if PVs are not connected
         """
-        file_name = "EmbeddedPy"
+        file_name = 'EmbeddedPy'
         self._script(file_name, python_script, pv_dict, only_trigger_if_connected)
 
     def embedded_javascript_script(self, js_script: str, pv_dict: dict, only_trigger_if_connected: bool = True) -> None:
         """
         Add an embedded JS script to the widget
 
         :param js_script: Usually multi-line string representing the actual JS code to attach to widget
         :param pv_dict: Dictionary of PVs for the script, format - { pvName: triggerOnPV }
         :param only_trigger_if_connected: Defaults to True. If False, script will run even if PVs are not connected
         """
-        file_name = "EmbeddedJs"
+        file_name = 'EmbeddedJs'
         self._script(file_name, js_script, pv_dict, only_trigger_if_connected)
 
     def external_script(self, file_name: str, pv_dict: dict, only_trigger_if_connected: bool = True) -> None:
         """
         Add an external script to the widget, either jython (.py) or javascript (.js)
 
         :param file_name: Path and file name of the external script to attach to widget
@@ -227,8 +226,7 @@
 
 
     def __str__(self):
         return prettify(self.root)
 
     def __repr__(self):
         return prettify(self.root)
-
```

### Comparing `phoebusgen-2.4.5/phoebusgen/widget/widgets.py` & `phoebusgen-2.5/phoebusgen/widget/widgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -696,8 +696,7 @@
         :param x: X position
         :param y: Y position
         :param width: Widget width
         :param height: Widget height
         """
         _Widget.__init__(self, 'webbrowser', name, x, y, width, height)
         self.url(url)
-
```

### Comparing `phoebusgen-2.4.5/phoebusgen.egg-info/PKG-INFO` & `phoebusgen-2.5/phoebusgen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phoebusgen
-Version: 2.4.5
+Version: 2.5
 Summary: Control screen generator for Phoebus
 Home-page: https://github.com/tynanford/phoebusgen
 Author: Tynan Ford
 Author-email: tford@lbl.gov
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
@@ -66,15 +66,15 @@
   <font>
     <font family="Liberation Sans" size="14" style="BOLD"/>
   </font>
 </widget>
 
 ```
 
-## Modules 
+## Modules
 
 ### phoebusgen.widget
 
 Python API to directly create Phoebus widgets. All standard Phoebus widgets are available, but some (3) are not fully feature complete.
 
 [Widgets Docs](https://als-epics.github.io/phoebusgen/source/phoebusgen.widget.html#module-phoebusgen.widget.widgets)
 
@@ -82,15 +82,15 @@
 -   Image
 -   Strip Chart
 -   X/Y Plot
 
 Example
 -   ```text_update_xml = phoebusgen.widget.TextUpdate(widget_name, pv_name, x, y, width, height)```
 
-### phoebusgen.screen 
+### phoebusgen.screen
 
 Python object to represent a Phoebus screen. Widgets can be added to the screen object and the screen object can be written to a .bob file to be opened in Phoebus.
 
 [Screen Docs](https://als-epics.github.io/phoebusgen/source/phoebusgen.screen.html#module-phoebusgen.screen.screen)
 
 Example
 ```pycon
@@ -118,15 +118,15 @@
     <pv_name>test:PV</pv_name>
   </widget>
 </display>
 ```
 
 ## Site specific color and font definitions
 
-Place a custon color.def or font.def in ~/.phoebusgen/ to force phoebusgen.colors or phoebusgen.fonts to reflect your site's custom definitions. 
+Place a custon color.def or font.def in ~/.phoebusgen/ to force phoebusgen.colors or phoebusgen.fonts to reflect your site's custom definitions.
 
 ```python
 my_widget.predefined_font(phoebusgen.fonts.Header1)
 ```
 ```python
 my_widget.predefined_color(phoebusgen.colors.OK)
 ```
```

### Comparing `phoebusgen-2.4.5/phoebusgen.egg-info/SOURCES.txt` & `phoebusgen-2.5/phoebusgen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phoebusgen-2.4.5/versioneer.py` & `phoebusgen-2.5/versioneer.py`

 * *Files 8% similar despite different names*

```diff
@@ -298,71 +298,71 @@
 def get_root():
     """Get the project root directory.
 
     We require that all commands are run from the project root, i.e. the
     directory that contains setup.py, setup.cfg, and versioneer.py .
     """
     root = os.path.realpath(os.path.abspath(os.getcwd()))
-    setup_py = os.path.join(root, "setup.py")
-    versioneer_py = os.path.join(root, "versioneer.py")
+    setup_py = os.path.join(root, 'setup.py')
+    versioneer_py = os.path.join(root, 'versioneer.py')
     if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
         # allow 'python path/to/setup.py COMMAND'
         root = os.path.dirname(os.path.realpath(os.path.abspath(sys.argv[0])))
-        setup_py = os.path.join(root, "setup.py")
-        versioneer_py = os.path.join(root, "versioneer.py")
+        setup_py = os.path.join(root, 'setup.py')
+        versioneer_py = os.path.join(root, 'versioneer.py')
     if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
-        err = ("Versioneer was unable to run the project root directory. "
-               "Versioneer requires setup.py to be executed from "
+        err = ('Versioneer was unable to run the project root directory. '
+               'Versioneer requires setup.py to be executed from '
                "its immediate directory (like 'python setup.py COMMAND'), "
-               "or in a way that lets it use sys.argv[0] to find the root "
+               'or in a way that lets it use sys.argv[0] to find the root '
                "(like 'python path/to/setup.py COMMAND').")
         raise VersioneerBadRootError(err)
     try:
         # Certain runtime workflows (setup.py install/develop in a setuptools
         # tree) execute all dependencies in a single python process, so
         # "versioneer" may be imported multiple times, and python's shared
         # module-import table will cache the first one. So we can't use
         # os.path.dirname(__file__), as that will find whichever
         # versioneer.py was first imported, even in later projects.
         my_path = os.path.realpath(os.path.abspath(__file__))
         me_dir = os.path.normcase(os.path.splitext(my_path)[0])
         vsr_dir = os.path.normcase(os.path.splitext(versioneer_py)[0])
         if me_dir != vsr_dir:
-            print("Warning: build in %s is using versioneer.py from %s"
+            print('Warning: build in %s is using versioneer.py from %s'
                   % (os.path.dirname(my_path), versioneer_py))
     except NameError:
         pass
     return root
 
 
 def get_config_from_root(root):
     """Read the project setup.cfg file to determine Versioneer config."""
     # This might raise OSError (if setup.cfg is missing), or
     # configparser.NoSectionError (if it lacks a [versioneer] section), or
     # configparser.NoOptionError (if it lacks "VCS="). See the docstring at
     # the top of versioneer.py for instructions on writing your setup.cfg .
-    setup_cfg = os.path.join(root, "setup.cfg")
+    setup_cfg = os.path.join(root, 'setup.cfg')
     parser = configparser.ConfigParser()
-    with open(setup_cfg, "r") as cfg_file:
+    with open(setup_cfg, 'r') as cfg_file:
         parser.read_file(cfg_file)
-    VCS = parser.get("versioneer", "VCS")  # mandatory
+    VCS = parser.get('versioneer', 'VCS')  # mandatory
 
     # Dict-like interface for non-mandatory entries
-    section = parser["versioneer"]
+    section = parser['versioneer']
 
     cfg = VersioneerConfig()
     cfg.VCS = VCS
-    cfg.style = section.get("style", "")
-    cfg.versionfile_source = section.get("versionfile_source")
-    cfg.versionfile_build = section.get("versionfile_build")
-    cfg.tag_prefix = section.get("tag_prefix")
+    cfg.style = section.get('style', '')
+    cfg.versionfile_source = section.get('versionfile_source')
+    cfg.versionfile_build = section.get('versionfile_build')
+    cfg.tag_prefix = section.get('tag_prefix')
     if cfg.tag_prefix in ("''", '""'):
-        cfg.tag_prefix = ""
-    cfg.parentdir_prefix = section.get("parentdir_prefix")
-    cfg.verbose = section.get("verbose")
+        cfg.tag_prefix = ''
+    cfg.parentdir_prefix = section.get('parentdir_prefix')
+    cfg.verbose = section.get('verbose')
     return cfg
 
 
 class NotThisMethod(Exception):
     """Exception raised if a method is not valid for the current scenario."""
 
 
@@ -383,19 +383,19 @@
 def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False,
                 env=None):
     """Call the given command(s)."""
     assert isinstance(commands, list)
     process = None
 
     popen_kwargs = {}
-    if sys.platform == "win32":
+    if sys.platform == 'win32':
         # This hides the console window if pythonw.exe is used
         startupinfo = subprocess.STARTUPINFO()
         startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
-        popen_kwargs["startupinfo"] = startupinfo
+        popen_kwargs['startupinfo'] = startupinfo
 
     for command in commands:
         try:
             dispcmd = str([command] + args)
             # remember shell=False, so use git.cmd on windows, not just git
             process = subprocess.Popen([command] + args, cwd=cwd, env=env,
                                        stdout=subprocess.PIPE,
@@ -403,26 +403,26 @@
                                                else None), **popen_kwargs)
             break
         except OSError:
             e = sys.exc_info()[1]
             if e.errno == errno.ENOENT:
                 continue
             if verbose:
-                print("unable to run %s" % dispcmd)
+                print('unable to run %s' % dispcmd)
                 print(e)
             return None, None
     else:
         if verbose:
-            print("unable to find command, tried %s" % (commands,))
+            print('unable to find command, tried %s' % (commands,))
         return None, None
     stdout = process.communicate()[0].strip().decode()
     if process.returncode != 0:
         if verbose:
-            print("unable to run %s (error)" % dispcmd)
-            print("stdout was %s" % stdout)
+            print('unable to run %s (error)' % dispcmd)
+            print('stdout was %s' % stdout)
         return None, process.returncode
     return stdout, process.returncode
 
 
 LONG_VERSION_PY['git'] = r'''
 # This file helps to compute a version number in source trees obtained from
 # git-archive tarball (such as those provided by githubs download-from-tag
@@ -1080,297 +1080,297 @@
 
     return {"version": "0+unknown", "full-revisionid": None,
             "dirty": None,
             "error": "unable to compute version", "date": None}
 '''
 
 
-@register_vcs_handler("git", "get_keywords")
+@register_vcs_handler('git', 'get_keywords')
 def git_get_keywords(versionfile_abs):
     """Extract version information from the given file."""
     # the code embedded in _version.py can just fetch the value of these
     # keywords. When used from setup.py, we don't want to import _version.py,
     # so we do it with a regexp instead. This function is not used from
     # _version.py.
     keywords = {}
     try:
-        with open(versionfile_abs, "r") as fobj:
+        with open(versionfile_abs, 'r') as fobj:
             for line in fobj:
-                if line.strip().startswith("git_refnames ="):
+                if line.strip().startswith('git_refnames ='):
                     mo = re.search(r'=\s*"(.*)"', line)
                     if mo:
-                        keywords["refnames"] = mo.group(1)
-                if line.strip().startswith("git_full ="):
+                        keywords['refnames'] = mo.group(1)
+                if line.strip().startswith('git_full ='):
                     mo = re.search(r'=\s*"(.*)"', line)
                     if mo:
-                        keywords["full"] = mo.group(1)
-                if line.strip().startswith("git_date ="):
+                        keywords['full'] = mo.group(1)
+                if line.strip().startswith('git_date ='):
                     mo = re.search(r'=\s*"(.*)"', line)
                     if mo:
-                        keywords["date"] = mo.group(1)
+                        keywords['date'] = mo.group(1)
     except OSError:
         pass
     return keywords
 
 
-@register_vcs_handler("git", "keywords")
+@register_vcs_handler('git', 'keywords')
 def git_versions_from_keywords(keywords, tag_prefix, verbose):
     """Get version information from git keywords."""
-    if "refnames" not in keywords:
-        raise NotThisMethod("Short version file found")
-    date = keywords.get("date")
+    if 'refnames' not in keywords:
+        raise NotThisMethod('Short version file found')
+    date = keywords.get('date')
     if date is not None:
         # Use only the last line.  Previous lines may contain GPG signature
         # information.
         date = date.splitlines()[-1]
 
         # git-2.2.0 added "%cI", which expands to an ISO-8601 -compliant
         # datestamp. However we prefer "%ci" (which expands to an "ISO-8601
         # -like" string, which we must then edit to make compliant), because
         # it's been around since git-1.5.3, and it's too difficult to
         # discover which version we're using, or to work around using an
         # older one.
-        date = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
-    refnames = keywords["refnames"].strip()
-    if refnames.startswith("$Format"):
+        date = date.strip().replace(' ', 'T', 1).replace(' ', '', 1)
+    refnames = keywords['refnames'].strip()
+    if refnames.startswith('$Format'):
         if verbose:
-            print("keywords are unexpanded, not using")
-        raise NotThisMethod("unexpanded keywords, not a git-archive tarball")
-    refs = {r.strip() for r in refnames.strip("()").split(",")}
+            print('keywords are unexpanded, not using')
+        raise NotThisMethod('unexpanded keywords, not a git-archive tarball')
+    refs = {r.strip() for r in refnames.strip('()').split(',')}
     # starting in git-1.8.3, tags are listed as "tag: foo-1.0" instead of
     # just "foo-1.0". If we see a "tag: " prefix, prefer those.
-    TAG = "tag: "
+    TAG = 'tag: '
     tags = {r[len(TAG):] for r in refs if r.startswith(TAG)}
     if not tags:
         # Either we're using git < 1.8.3, or there really are no tags. We use
         # a heuristic: assume all version tags have a digit. The old git %d
         # expansion behaves like git log --decorate=short and strips out the
         # refs/heads/ and refs/tags/ prefixes that would let us distinguish
         # between branches and tags. By ignoring refnames without digits, we
         # filter out many common branch names like "release" and
         # "stabilization", as well as "HEAD" and "master".
         tags = {r for r in refs if re.search(r'\d', r)}
         if verbose:
-            print("discarding '%s', no digits" % ",".join(refs - tags))
+            print("discarding '%s', no digits" % ','.join(refs - tags))
     if verbose:
-        print("likely tags: %s" % ",".join(sorted(tags)))
+        print('likely tags: %s' % ','.join(sorted(tags)))
     for ref in sorted(tags):
         # sorting will prefer e.g. "2.0" over "2.0rc1"
         if ref.startswith(tag_prefix):
             r = ref[len(tag_prefix):]
             # Filter out refs that exactly match prefix or that don't start
             # with a number once the prefix is stripped (mostly a concern
             # when prefix is '')
             if not re.match(r'\d', r):
                 continue
             if verbose:
-                print("picking %s" % r)
-            return {"version": r,
-                    "full-revisionid": keywords["full"].strip(),
-                    "dirty": False, "error": None,
-                    "date": date}
+                print('picking %s' % r)
+            return {'version': r,
+                    'full-revisionid': keywords['full'].strip(),
+                    'dirty': False, 'error': None,
+                    'date': date}
     # no suitable tags, so version is "0+unknown", but full hex is still there
     if verbose:
-        print("no suitable tags, using unknown + full revision id")
-    return {"version": "0+unknown",
-            "full-revisionid": keywords["full"].strip(),
-            "dirty": False, "error": "no suitable tags", "date": None}
+        print('no suitable tags, using unknown + full revision id')
+    return {'version': '0+unknown',
+            'full-revisionid': keywords['full'].strip(),
+            'dirty': False, 'error': 'no suitable tags', 'date': None}
 
 
-@register_vcs_handler("git", "pieces_from_vcs")
+@register_vcs_handler('git', 'pieces_from_vcs')
 def git_pieces_from_vcs(tag_prefix, root, verbose, runner=run_command):
     """Get version from 'git describe' in the root of the source tree.
 
     This only gets called if the git-archive 'subst' keywords were *not*
     expanded, and _version.py hasn't already been rewritten with a short
     version string, meaning we're inside a checked out source tree.
     """
-    GITS = ["git"]
-    if sys.platform == "win32":
-        GITS = ["git.cmd", "git.exe"]
+    GITS = ['git']
+    if sys.platform == 'win32':
+        GITS = ['git.cmd', 'git.exe']
 
     # GIT_DIR can interfere with correct operation of Versioneer.
     # It may be intended to be passed to the Versioneer-versioned project,
     # but that should not change where we get our version from.
     env = os.environ.copy()
-    env.pop("GIT_DIR", None)
+    env.pop('GIT_DIR', None)
     runner = functools.partial(runner, env=env)
 
-    _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root,
+    _, rc = runner(GITS, ['rev-parse', '--git-dir'], cwd=root,
                    hide_stderr=True)
     if rc != 0:
         if verbose:
-            print("Directory %s not under git control" % root)
+            print('Directory %s not under git control' % root)
         raise NotThisMethod("'git rev-parse --git-dir' returned error")
 
-    MATCH_ARGS = ["--match", "%s*" % tag_prefix] if tag_prefix else []
+    MATCH_ARGS = ['--match', '%s*' % tag_prefix] if tag_prefix else []
 
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
-    describe_out, rc = runner(GITS, ["describe", "--tags", "--dirty",
-                                     "--always", "--long", *MATCH_ARGS],
+    describe_out, rc = runner(GITS, ['describe', '--tags', '--dirty',
+                                     '--always', '--long', *MATCH_ARGS],
                               cwd=root)
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
-    full_out, rc = runner(GITS, ["rev-parse", "HEAD"], cwd=root)
+    full_out, rc = runner(GITS, ['rev-parse', 'HEAD'], cwd=root)
     if full_out is None:
         raise NotThisMethod("'git rev-parse' failed")
     full_out = full_out.strip()
 
     pieces = {}
-    pieces["long"] = full_out
-    pieces["short"] = full_out[:7]  # maybe improved later
-    pieces["error"] = None
+    pieces['long'] = full_out
+    pieces['short'] = full_out[:7]  # maybe improved later
+    pieces['error'] = None
 
-    branch_name, rc = runner(GITS, ["rev-parse", "--abbrev-ref", "HEAD"],
+    branch_name, rc = runner(GITS, ['rev-parse', '--abbrev-ref', 'HEAD'],
                              cwd=root)
     # --abbrev-ref was added in git-1.6.3
     if rc != 0 or branch_name is None:
         raise NotThisMethod("'git rev-parse --abbrev-ref' returned error")
     branch_name = branch_name.strip()
 
-    if branch_name == "HEAD":
+    if branch_name == 'HEAD':
         # If we aren't exactly on a branch, pick a branch which represents
         # the current commit. If all else fails, we are on a branchless
         # commit.
-        branches, rc = runner(GITS, ["branch", "--contains"], cwd=root)
+        branches, rc = runner(GITS, ['branch', '--contains'], cwd=root)
         # --contains was added in git-1.5.4
         if rc != 0 or branches is None:
             raise NotThisMethod("'git branch --contains' returned error")
-        branches = branches.split("\n")
+        branches = branches.split('\n')
 
         # Remove the first line if we're running detached
-        if "(" in branches[0]:
+        if '(' in branches[0]:
             branches.pop(0)
 
         # Strip off the leading "* " from the list of branches.
         branches = [branch[2:] for branch in branches]
-        if "master" in branches:
-            branch_name = "master"
+        if 'master' in branches:
+            branch_name = 'master'
         elif not branches:
             branch_name = None
         else:
             # Pick the first branch that is returned. Good or bad.
             branch_name = branches[0]
 
-    pieces["branch"] = branch_name
+    pieces['branch'] = branch_name
 
     # parse describe_out. It will be like TAG-NUM-gHEX[-dirty] or HEX[-dirty]
     # TAG might have hyphens.
     git_describe = describe_out
 
     # look for -dirty suffix
-    dirty = git_describe.endswith("-dirty")
-    pieces["dirty"] = dirty
+    dirty = git_describe.endswith('-dirty')
+    pieces['dirty'] = dirty
     if dirty:
-        git_describe = git_describe[:git_describe.rindex("-dirty")]
+        git_describe = git_describe[:git_describe.rindex('-dirty')]
 
     # now we have TAG-NUM-gHEX or HEX
 
-    if "-" in git_describe:
+    if '-' in git_describe:
         # TAG-NUM-gHEX
         mo = re.search(r'^(.+)-(\d+)-g([0-9a-f]+)$', git_describe)
         if not mo:
             # unparsable. Maybe git-describe is misbehaving?
-            pieces["error"] = ("unable to parse git-describe output: '%s'"
+            pieces['error'] = ("unable to parse git-describe output: '%s'"
                                % describe_out)
             return pieces
 
         # tag
         full_tag = mo.group(1)
         if not full_tag.startswith(tag_prefix):
             if verbose:
                 fmt = "tag '%s' doesn't start with prefix '%s'"
                 print(fmt % (full_tag, tag_prefix))
-            pieces["error"] = ("tag '%s' doesn't start with prefix '%s'"
+            pieces['error'] = ("tag '%s' doesn't start with prefix '%s'"
                                % (full_tag, tag_prefix))
             return pieces
-        pieces["closest-tag"] = full_tag[len(tag_prefix):]
+        pieces['closest-tag'] = full_tag[len(tag_prefix):]
 
         # distance: number of commits since tag
-        pieces["distance"] = int(mo.group(2))
+        pieces['distance'] = int(mo.group(2))
 
         # commit: short hex revision ID
-        pieces["short"] = mo.group(3)
+        pieces['short'] = mo.group(3)
 
     else:
         # HEX: no tags
-        pieces["closest-tag"] = None
-        count_out, rc = runner(GITS, ["rev-list", "HEAD", "--count"], cwd=root)
-        pieces["distance"] = int(count_out)  # total number of commits
+        pieces['closest-tag'] = None
+        count_out, rc = runner(GITS, ['rev-list', 'HEAD', '--count'], cwd=root)
+        pieces['distance'] = int(count_out)  # total number of commits
 
     # commit date: see ISO-8601 comment in git_versions_from_keywords()
-    date = runner(GITS, ["show", "-s", "--format=%ci", "HEAD"], cwd=root)[0].strip()
+    date = runner(GITS, ['show', '-s', '--format=%ci', 'HEAD'], cwd=root)[0].strip()
     # Use only the last line.  Previous lines may contain GPG signature
     # information.
     date = date.splitlines()[-1]
-    pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
+    pieces['date'] = date.strip().replace(' ', 'T', 1).replace(' ', '', 1)
 
     return pieces
 
 
 def do_vcs_install(manifest_in, versionfile_source, ipy):
     """Git-specific installation logic for Versioneer.
 
     For Git, this means creating/changing .gitattributes to mark _version.py
     for export-subst keyword substitution.
     """
-    GITS = ["git"]
-    if sys.platform == "win32":
-        GITS = ["git.cmd", "git.exe"]
+    GITS = ['git']
+    if sys.platform == 'win32':
+        GITS = ['git.cmd', 'git.exe']
     files = [manifest_in, versionfile_source]
     if ipy:
         files.append(ipy)
     try:
         my_path = __file__
-        if my_path.endswith(".pyc") or my_path.endswith(".pyo"):
-            my_path = os.path.splitext(my_path)[0] + ".py"
+        if my_path.endswith('.pyc') or my_path.endswith('.pyo'):
+            my_path = os.path.splitext(my_path)[0] + '.py'
         versioneer_file = os.path.relpath(my_path)
     except NameError:
-        versioneer_file = "versioneer.py"
+        versioneer_file = 'versioneer.py'
     files.append(versioneer_file)
     present = False
     try:
-        with open(".gitattributes", "r") as fobj:
+        with open('.gitattributes', 'r') as fobj:
             for line in fobj:
                 if line.strip().startswith(versionfile_source):
-                    if "export-subst" in line.strip().split()[1:]:
+                    if 'export-subst' in line.strip().split()[1:]:
                         present = True
                         break
     except OSError:
         pass
     if not present:
-        with open(".gitattributes", "a+") as fobj:
-            fobj.write(f"{versionfile_source} export-subst\n")
-        files.append(".gitattributes")
-    run_command(GITS, ["add", "--"] + files)
+        with open('.gitattributes', 'a+') as fobj:
+            fobj.write(f'{versionfile_source} export-subst\n')
+        files.append('.gitattributes')
+    run_command(GITS, ['add', '--'] + files)
 
 
 def versions_from_parentdir(parentdir_prefix, root, verbose):
     """Try to determine the version from the parent directory name.
 
     Source tarballs conventionally unpack into a directory that includes both
     the project name and a version string. We will also support searching up
     two directory levels for an appropriately named parent directory
     """
     rootdirs = []
 
     for _ in range(3):
         dirname = os.path.basename(root)
         if dirname.startswith(parentdir_prefix):
-            return {"version": dirname[len(parentdir_prefix):],
-                    "full-revisionid": None,
-                    "dirty": False, "error": None, "date": None}
+            return {'version': dirname[len(parentdir_prefix):],
+                    'full-revisionid': None,
+                    'dirty': False, 'error': None, 'date': None}
         rootdirs.append(root)
         root = os.path.dirname(root)  # up a level
 
     if verbose:
-        print("Tried directories %s but none started with prefix %s" %
+        print('Tried directories %s but none started with prefix %s' %
               (str(rootdirs), parentdir_prefix))
     raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
 
 
 SHORT_VERSION_PY = """
 # This file was generated by 'versioneer.py' (0.22) from
 # revision-control system data, or from the parent directory name of an
@@ -1391,379 +1391,379 @@
 
 def versions_from_file(filename):
     """Try to determine the version from _version.py if present."""
     try:
         with open(filename) as f:
             contents = f.read()
     except OSError:
-        raise NotThisMethod("unable to read _version.py")
+        raise NotThisMethod('unable to read _version.py')
     mo = re.search(r"version_json = '''\n(.*)'''  # END VERSION_JSON",
                    contents, re.M | re.S)
     if not mo:
         mo = re.search(r"version_json = '''\r\n(.*)'''  # END VERSION_JSON",
                        contents, re.M | re.S)
     if not mo:
-        raise NotThisMethod("no version_json in _version.py")
+        raise NotThisMethod('no version_json in _version.py')
     return json.loads(mo.group(1))
 
 
 def write_to_version_file(filename, versions):
     """Write the given version number to the given _version.py file."""
     os.unlink(filename)
     contents = json.dumps(versions, sort_keys=True,
-                          indent=1, separators=(",", ": "))
-    with open(filename, "w") as f:
+                          indent=1, separators=(',', ': '))
+    with open(filename, 'w') as f:
         f.write(SHORT_VERSION_PY % contents)
 
-    print("set %s to '%s'" % (filename, versions["version"]))
+    print("set %s to '%s'" % (filename, versions['version']))
 
 
 def plus_or_dot(pieces):
     """Return a + if we don't already have one, else return a ."""
-    if "+" in pieces.get("closest-tag", ""):
-        return "."
-    return "+"
+    if '+' in pieces.get('closest-tag', ''):
+        return '.'
+    return '+'
 
 
 def render_pep440(pieces):
     """Build up version string, with post-release "local version identifier".
 
     Our goal: TAG[+DISTANCE.gHEX[.dirty]] . Note that if you
     get a tagged build and then dirty it, you'll get TAG+0.gHEX.dirty
 
     Exceptions:
     1: no tags. git_describe was just HEX. 0+untagged.DISTANCE.gHEX[.dirty]
     """
-    if pieces["closest-tag"]:
-        rendered = pieces["closest-tag"]
-        if pieces["distance"] or pieces["dirty"]:
+    if pieces['closest-tag']:
+        rendered = pieces['closest-tag']
+        if pieces['distance'] or pieces['dirty']:
             rendered += plus_or_dot(pieces)
-            rendered += "%d.g%s" % (pieces["distance"], pieces["short"])
-            if pieces["dirty"]:
-                rendered += ".dirty"
+            rendered += '%d.g%s' % (pieces['distance'], pieces['short'])
+            if pieces['dirty']:
+                rendered += '.dirty'
     else:
         # exception #1
-        rendered = "0+untagged.%d.g%s" % (pieces["distance"],
-                                          pieces["short"])
-        if pieces["dirty"]:
-            rendered += ".dirty"
+        rendered = '0+untagged.%d.g%s' % (pieces['distance'],
+                                          pieces['short'])
+        if pieces['dirty']:
+            rendered += '.dirty'
     return rendered
 
 
 def render_pep440_branch(pieces):
     """TAG[[.dev0]+DISTANCE.gHEX[.dirty]] .
 
     The ".dev0" means not master branch. Note that .dev0 sorts backwards
     (a feature branch will appear "older" than the master branch).
 
     Exceptions:
     1: no tags. 0[.dev0]+untagged.DISTANCE.gHEX[.dirty]
     """
-    if pieces["closest-tag"]:
-        rendered = pieces["closest-tag"]
-        if pieces["distance"] or pieces["dirty"]:
-            if pieces["branch"] != "master":
-                rendered += ".dev0"
+    if pieces['closest-tag']:
+        rendered = pieces['closest-tag']
+        if pieces['distance'] or pieces['dirty']:
+            if pieces['branch'] != 'master':
+                rendered += '.dev0'
             rendered += plus_or_dot(pieces)
-            rendered += "%d.g%s" % (pieces["distance"], pieces["short"])
-            if pieces["dirty"]:
-                rendered += ".dirty"
+            rendered += '%d.g%s' % (pieces['distance'], pieces['short'])
+            if pieces['dirty']:
+                rendered += '.dirty'
     else:
         # exception #1
-        rendered = "0"
-        if pieces["branch"] != "master":
-            rendered += ".dev0"
-        rendered += "+untagged.%d.g%s" % (pieces["distance"],
-                                          pieces["short"])
-        if pieces["dirty"]:
-            rendered += ".dirty"
+        rendered = '0'
+        if pieces['branch'] != 'master':
+            rendered += '.dev0'
+        rendered += '+untagged.%d.g%s' % (pieces['distance'],
+                                          pieces['short'])
+        if pieces['dirty']:
+            rendered += '.dirty'
     return rendered
 
 
 def pep440_split_post(ver):
     """Split pep440 version string at the post-release segment.
 
     Returns the release segments before the post-release and the
     post-release version number (or -1 if no post-release segment is present).
     """
-    vc = str.split(ver, ".post")
+    vc = str.split(ver, '.post')
     return vc[0], int(vc[1] or 0) if len(vc) == 2 else None
 
 
 def render_pep440_pre(pieces):
     """TAG[.postN.devDISTANCE] -- No -dirty.
 
     Exceptions:
     1: no tags. 0.post0.devDISTANCE
     """
-    if pieces["closest-tag"]:
-        if pieces["distance"]:
+    if pieces['closest-tag']:
+        if pieces['distance']:
             # update the post release segment
-            tag_version, post_version = pep440_split_post(pieces["closest-tag"])
+            tag_version, post_version = pep440_split_post(pieces['closest-tag'])
             rendered = tag_version
             if post_version is not None:
-                rendered += ".post%d.dev%d" % (post_version+1, pieces["distance"])
+                rendered += '.post%d.dev%d' % (post_version+1, pieces['distance'])
             else:
-                rendered += ".post0.dev%d" % (pieces["distance"])
+                rendered += '.post0.dev%d' % (pieces['distance'])
         else:
             # no commits, use the tag as the version
-            rendered = pieces["closest-tag"]
+            rendered = pieces['closest-tag']
     else:
         # exception #1
-        rendered = "0.post0.dev%d" % pieces["distance"]
+        rendered = '0.post0.dev%d' % pieces['distance']
     return rendered
 
 
 def render_pep440_post(pieces):
     """TAG[.postDISTANCE[.dev0]+gHEX] .
 
     The ".dev0" means dirty. Note that .dev0 sorts backwards
     (a dirty tree will appear "older" than the corresponding clean one),
     but you shouldn't be releasing software with -dirty anyways.
 
     Exceptions:
     1: no tags. 0.postDISTANCE[.dev0]
     """
-    if pieces["closest-tag"]:
-        rendered = pieces["closest-tag"]
-        if pieces["distance"] or pieces["dirty"]:
-            rendered += ".post%d" % pieces["distance"]
-            if pieces["dirty"]:
-                rendered += ".dev0"
+    if pieces['closest-tag']:
+        rendered = pieces['closest-tag']
+        if pieces['distance'] or pieces['dirty']:
+            rendered += '.post%d' % pieces['distance']
+            if pieces['dirty']:
+                rendered += '.dev0'
             rendered += plus_or_dot(pieces)
-            rendered += "g%s" % pieces["short"]
+            rendered += 'g%s' % pieces['short']
     else:
         # exception #1
-        rendered = "0.post%d" % pieces["distance"]
-        if pieces["dirty"]:
-            rendered += ".dev0"
-        rendered += "+g%s" % pieces["short"]
+        rendered = '0.post%d' % pieces['distance']
+        if pieces['dirty']:
+            rendered += '.dev0'
+        rendered += '+g%s' % pieces['short']
     return rendered
 
 
 def render_pep440_post_branch(pieces):
     """TAG[.postDISTANCE[.dev0]+gHEX[.dirty]] .
 
     The ".dev0" means not master branch.
 
     Exceptions:
     1: no tags. 0.postDISTANCE[.dev0]+gHEX[.dirty]
     """
-    if pieces["closest-tag"]:
-        rendered = pieces["closest-tag"]
-        if pieces["distance"] or pieces["dirty"]:
-            rendered += ".post%d" % pieces["distance"]
-            if pieces["branch"] != "master":
-                rendered += ".dev0"
+    if pieces['closest-tag']:
+        rendered = pieces['closest-tag']
+        if pieces['distance'] or pieces['dirty']:
+            rendered += '.post%d' % pieces['distance']
+            if pieces['branch'] != 'master':
+                rendered += '.dev0'
             rendered += plus_or_dot(pieces)
-            rendered += "g%s" % pieces["short"]
-            if pieces["dirty"]:
-                rendered += ".dirty"
+            rendered += 'g%s' % pieces['short']
+            if pieces['dirty']:
+                rendered += '.dirty'
     else:
         # exception #1
-        rendered = "0.post%d" % pieces["distance"]
-        if pieces["branch"] != "master":
-            rendered += ".dev0"
-        rendered += "+g%s" % pieces["short"]
-        if pieces["dirty"]:
-            rendered += ".dirty"
+        rendered = '0.post%d' % pieces['distance']
+        if pieces['branch'] != 'master':
+            rendered += '.dev0'
+        rendered += '+g%s' % pieces['short']
+        if pieces['dirty']:
+            rendered += '.dirty'
     return rendered
 
 
 def render_pep440_old(pieces):
     """TAG[.postDISTANCE[.dev0]] .
 
     The ".dev0" means dirty.
 
     Exceptions:
     1: no tags. 0.postDISTANCE[.dev0]
     """
-    if pieces["closest-tag"]:
-        rendered = pieces["closest-tag"]
-        if pieces["distance"] or pieces["dirty"]:
-            rendered += ".post%d" % pieces["distance"]
-            if pieces["dirty"]:
-                rendered += ".dev0"
+    if pieces['closest-tag']:
+        rendered = pieces['closest-tag']
+        if pieces['distance'] or pieces['dirty']:
+            rendered += '.post%d' % pieces['distance']
+            if pieces['dirty']:
+                rendered += '.dev0'
     else:
         # exception #1
-        rendered = "0.post%d" % pieces["distance"]
-        if pieces["dirty"]:
-            rendered += ".dev0"
+        rendered = '0.post%d' % pieces['distance']
+        if pieces['dirty']:
+            rendered += '.dev0'
     return rendered
 
 
 def render_git_describe(pieces):
     """TAG[-DISTANCE-gHEX][-dirty].
 
     Like 'git describe --tags --dirty --always'.
 
     Exceptions:
     1: no tags. HEX[-dirty]  (note: no 'g' prefix)
     """
-    if pieces["closest-tag"]:
-        rendered = pieces["closest-tag"]
-        if pieces["distance"]:
-            rendered += "-%d-g%s" % (pieces["distance"], pieces["short"])
+    if pieces['closest-tag']:
+        rendered = pieces['closest-tag']
+        if pieces['distance']:
+            rendered += '-%d-g%s' % (pieces['distance'], pieces['short'])
     else:
         # exception #1
-        rendered = pieces["short"]
-    if pieces["dirty"]:
-        rendered += "-dirty"
+        rendered = pieces['short']
+    if pieces['dirty']:
+        rendered += '-dirty'
     return rendered
 
 
 def render_git_describe_long(pieces):
     """TAG-DISTANCE-gHEX[-dirty].
 
     Like 'git describe --tags --dirty --always -long'.
     The distance/hash is unconditional.
 
     Exceptions:
     1: no tags. HEX[-dirty]  (note: no 'g' prefix)
     """
-    if pieces["closest-tag"]:
-        rendered = pieces["closest-tag"]
-        rendered += "-%d-g%s" % (pieces["distance"], pieces["short"])
+    if pieces['closest-tag']:
+        rendered = pieces['closest-tag']
+        rendered += '-%d-g%s' % (pieces['distance'], pieces['short'])
     else:
         # exception #1
-        rendered = pieces["short"]
-    if pieces["dirty"]:
-        rendered += "-dirty"
+        rendered = pieces['short']
+    if pieces['dirty']:
+        rendered += '-dirty'
     return rendered
 
 
 def render(pieces, style):
     """Render the given version pieces into the requested style."""
-    if pieces["error"]:
-        return {"version": "unknown",
-                "full-revisionid": pieces.get("long"),
-                "dirty": None,
-                "error": pieces["error"],
-                "date": None}
+    if pieces['error']:
+        return {'version': 'unknown',
+                'full-revisionid': pieces.get('long'),
+                'dirty': None,
+                'error': pieces['error'],
+                'date': None}
 
-    if not style or style == "default":
-        style = "pep440"  # the default
+    if not style or style == 'default':
+        style = 'pep440'  # the default
 
-    if style == "pep440":
+    if style == 'pep440':
         rendered = render_pep440(pieces)
-    elif style == "pep440-branch":
+    elif style == 'pep440-branch':
         rendered = render_pep440_branch(pieces)
-    elif style == "pep440-pre":
+    elif style == 'pep440-pre':
         rendered = render_pep440_pre(pieces)
-    elif style == "pep440-post":
+    elif style == 'pep440-post':
         rendered = render_pep440_post(pieces)
-    elif style == "pep440-post-branch":
+    elif style == 'pep440-post-branch':
         rendered = render_pep440_post_branch(pieces)
-    elif style == "pep440-old":
+    elif style == 'pep440-old':
         rendered = render_pep440_old(pieces)
-    elif style == "git-describe":
+    elif style == 'git-describe':
         rendered = render_git_describe(pieces)
-    elif style == "git-describe-long":
+    elif style == 'git-describe-long':
         rendered = render_git_describe_long(pieces)
     else:
         raise ValueError("unknown style '%s'" % style)
 
-    return {"version": rendered, "full-revisionid": pieces["long"],
-            "dirty": pieces["dirty"], "error": None,
-            "date": pieces.get("date")}
+    return {'version': rendered, 'full-revisionid': pieces['long'],
+            'dirty': pieces['dirty'], 'error': None,
+            'date': pieces.get('date')}
 
 
 class VersioneerBadRootError(Exception):
     """The project root directory is unknown or missing key files."""
 
 
 def get_versions(verbose=False):
     """Get the project version from whatever source is available.
 
     Returns dict with two keys: 'version' and 'full'.
     """
-    if "versioneer" in sys.modules:
+    if 'versioneer' in sys.modules:
         # see the discussion in cmdclass.py:get_cmdclass()
-        del sys.modules["versioneer"]
+        del sys.modules['versioneer']
 
     root = get_root()
     cfg = get_config_from_root(root)
 
-    assert cfg.VCS is not None, "please set [versioneer]VCS= in setup.cfg"
+    assert cfg.VCS is not None, 'please set [versioneer]VCS= in setup.cfg'
     handlers = HANDLERS.get(cfg.VCS)
     assert handlers, "unrecognized VCS '%s'" % cfg.VCS
     verbose = verbose or cfg.verbose
     assert cfg.versionfile_source is not None, \
-        "please set versioneer.versionfile_source"
-    assert cfg.tag_prefix is not None, "please set versioneer.tag_prefix"
+        'please set versioneer.versionfile_source'
+    assert cfg.tag_prefix is not None, 'please set versioneer.tag_prefix'
 
     versionfile_abs = os.path.join(root, cfg.versionfile_source)
 
     # extract version from first of: _version.py, VCS command (e.g. 'git
     # describe'), parentdir. This is meant to work for developers using a
     # source checkout, for users of a tarball created by 'setup.py sdist',
     # and for users of a tarball/zipball created by 'git archive' or github's
     # download-from-tag feature or the equivalent in other VCSes.
 
-    get_keywords_f = handlers.get("get_keywords")
-    from_keywords_f = handlers.get("keywords")
+    get_keywords_f = handlers.get('get_keywords')
+    from_keywords_f = handlers.get('keywords')
     if get_keywords_f and from_keywords_f:
         try:
             keywords = get_keywords_f(versionfile_abs)
             ver = from_keywords_f(keywords, cfg.tag_prefix, verbose)
             if verbose:
-                print("got version from expanded keyword %s" % ver)
+                print('got version from expanded keyword %s' % ver)
             return ver
         except NotThisMethod:
             pass
 
     try:
         ver = versions_from_file(versionfile_abs)
         if verbose:
-            print("got version from file %s %s" % (versionfile_abs, ver))
+            print('got version from file %s %s' % (versionfile_abs, ver))
         return ver
     except NotThisMethod:
         pass
 
-    from_vcs_f = handlers.get("pieces_from_vcs")
+    from_vcs_f = handlers.get('pieces_from_vcs')
     if from_vcs_f:
         try:
             pieces = from_vcs_f(cfg.tag_prefix, root, verbose)
             ver = render(pieces, cfg.style)
             if verbose:
-                print("got version from VCS %s" % ver)
+                print('got version from VCS %s' % ver)
             return ver
         except NotThisMethod:
             pass
 
     try:
         if cfg.parentdir_prefix:
             ver = versions_from_parentdir(cfg.parentdir_prefix, root, verbose)
             if verbose:
-                print("got version from parentdir %s" % ver)
+                print('got version from parentdir %s' % ver)
             return ver
     except NotThisMethod:
         pass
 
     if verbose:
-        print("unable to compute version")
+        print('unable to compute version')
 
-    return {"version": "0+unknown", "full-revisionid": None,
-            "dirty": None, "error": "unable to compute version",
-            "date": None}
+    return {'version': '0+unknown', 'full-revisionid': None,
+            'dirty': None, 'error': 'unable to compute version',
+            'date': None}
 
 
 def get_version():
     """Get the short version string for this project."""
-    return get_versions()["version"]
+    return get_versions()['version']
 
 
 def get_cmdclass(cmdclass=None):
     """Get the custom setuptools/distutils subclasses used by Versioneer.
 
     If the package uses a different cmdclass (e.g. one from numpy), it
     should be provide as an argument.
     """
-    if "versioneer" in sys.modules:
-        del sys.modules["versioneer"]
+    if 'versioneer' in sys.modules:
+        del sys.modules['versioneer']
         # this fixes the "python setup.py develop" case (also 'install' and
         # 'easy_install .'), in which subdependencies of the main project are
         # built (using setup.py bdist_egg) in the same python process. Assume
         # a main project A and a dependency B, which use different versions
         # of Versioneer. A's setup.py imports A's Versioneer, leaving it in
         # sys.modules by the time B's setup.py is executed, causing B to run
         # with the wrong versioneer. Setuptools wraps the sub-dep builds in a
@@ -1778,33 +1778,33 @@
     # we add "version" to both distutils and setuptools
     try:
         from setuptools import Command
     except ImportError:
         from distutils.core import Command
 
     class cmd_version(Command):
-        description = "report generated version string"
+        description = 'report generated version string'
         user_options = []
         boolean_options = []
 
         def initialize_options(self):
             pass
 
         def finalize_options(self):
             pass
 
         def run(self):
             vers = get_versions(verbose=True)
-            print("Version: %s" % vers["version"])
-            print(" full-revisionid: %s" % vers.get("full-revisionid"))
-            print(" dirty: %s" % vers.get("dirty"))
-            print(" date: %s" % vers.get("date"))
-            if vers["error"]:
-                print(" error: %s" % vers["error"])
-    cmds["version"] = cmd_version
+            print('Version: %s' % vers['version'])
+            print(' full-revisionid: %s' % vers.get('full-revisionid'))
+            print(' dirty: %s' % vers.get('dirty'))
+            print(' date: %s' % vers.get('date'))
+            if vers['error']:
+                print(' error: %s' % vers['error'])
+    cmds['version'] = cmd_version
 
     # we override "build_py" in both distutils and setuptools
     #
     # most invocation pathways end up running build_py:
     #  distutils/build -> build_py
     #  distutils/install -> distutils/build ->..
     #  setuptools/bdist_wheel -> distutils/install ->..
@@ -1816,15 +1816,15 @@
     #   if .git isn't copied too, 'git describe' will fail
     #   then does setup.py bdist_wheel, or sometimes setup.py install
     #  setup.py egg_info -> ?
 
     # we override different "build_py" commands for both environments
     if 'build_py' in cmds:
         _build_py = cmds['build_py']
-    elif "setuptools" in sys.modules:
+    elif 'setuptools' in sys.modules:
         from setuptools.command.build_py import build_py as _build_py
     else:
         from distutils.command.build_py import build_py as _build_py
 
     class cmd_build_py(_build_py):
         def run(self):
             root = get_root()
@@ -1832,21 +1832,21 @@
             versions = get_versions()
             _build_py.run(self)
             # now locate _version.py in the new build/ directory and replace
             # it with an updated value
             if cfg.versionfile_build:
                 target_versionfile = os.path.join(self.build_lib,
                                                   cfg.versionfile_build)
-                print("UPDATING %s" % target_versionfile)
+                print('UPDATING %s' % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
-    cmds["build_py"] = cmd_build_py
+    cmds['build_py'] = cmd_build_py
 
     if 'build_ext' in cmds:
         _build_ext = cmds['build_ext']
-    elif "setuptools" in sys.modules:
+    elif 'setuptools' in sys.modules:
         from setuptools.command.build_ext import build_ext as _build_ext
     else:
         from distutils.command.build_ext import build_ext as _build_ext
 
     class cmd_build_ext(_build_ext):
         def run(self):
             root = get_root()
@@ -1859,104 +1859,104 @@
                 # As in place builds will already have a _version.py
                 # in the module dir, we do not need to write one.
                 return
             # now locate _version.py in the new build/ directory and replace
             # it with an updated value
             target_versionfile = os.path.join(self.build_lib,
                                               cfg.versionfile_build)
-            print("UPDATING %s" % target_versionfile)
+            print('UPDATING %s' % target_versionfile)
             write_to_version_file(target_versionfile, versions)
-    cmds["build_ext"] = cmd_build_ext
+    cmds['build_ext'] = cmd_build_ext
 
-    if "cx_Freeze" in sys.modules:  # cx_freeze enabled?
+    if 'cx_Freeze' in sys.modules:  # cx_freeze enabled?
         from cx_Freeze.dist import build_exe as _build_exe
         # nczeczulin reports that py2exe won't like the pep440-style string
         # as FILEVERSION, but it can be used for PRODUCTVERSION, e.g.
         # setup(console=[{
         #   "version": versioneer.get_version().split("+", 1)[0], # FILEVERSION
         #   "product_version": versioneer.get_version(),
         #   ...
 
         class cmd_build_exe(_build_exe):
             def run(self):
                 root = get_root()
                 cfg = get_config_from_root(root)
                 versions = get_versions()
                 target_versionfile = cfg.versionfile_source
-                print("UPDATING %s" % target_versionfile)
+                print('UPDATING %s' % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
                 _build_exe.run(self)
                 os.unlink(target_versionfile)
-                with open(cfg.versionfile_source, "w") as f:
+                with open(cfg.versionfile_source, 'w') as f:
                     LONG = LONG_VERSION_PY[cfg.VCS]
                     f.write(LONG %
-                            {"DOLLAR": "$",
-                             "STYLE": cfg.style,
-                             "TAG_PREFIX": cfg.tag_prefix,
-                             "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                             "VERSIONFILE_SOURCE": cfg.versionfile_source,
+                            {'DOLLAR': '$',
+                             'STYLE': cfg.style,
+                             'TAG_PREFIX': cfg.tag_prefix,
+                             'PARENTDIR_PREFIX': cfg.parentdir_prefix,
+                             'VERSIONFILE_SOURCE': cfg.versionfile_source,
                              })
-        cmds["build_exe"] = cmd_build_exe
-        del cmds["build_py"]
+        cmds['build_exe'] = cmd_build_exe
+        del cmds['build_py']
 
     if 'py2exe' in sys.modules:  # py2exe enabled?
         from py2exe.distutils_buildexe import py2exe as _py2exe
 
         class cmd_py2exe(_py2exe):
             def run(self):
                 root = get_root()
                 cfg = get_config_from_root(root)
                 versions = get_versions()
                 target_versionfile = cfg.versionfile_source
-                print("UPDATING %s" % target_versionfile)
+                print('UPDATING %s' % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
                 _py2exe.run(self)
                 os.unlink(target_versionfile)
-                with open(cfg.versionfile_source, "w") as f:
+                with open(cfg.versionfile_source, 'w') as f:
                     LONG = LONG_VERSION_PY[cfg.VCS]
                     f.write(LONG %
-                            {"DOLLAR": "$",
-                             "STYLE": cfg.style,
-                             "TAG_PREFIX": cfg.tag_prefix,
-                             "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                             "VERSIONFILE_SOURCE": cfg.versionfile_source,
+                            {'DOLLAR': '$',
+                             'STYLE': cfg.style,
+                             'TAG_PREFIX': cfg.tag_prefix,
+                             'PARENTDIR_PREFIX': cfg.parentdir_prefix,
+                             'VERSIONFILE_SOURCE': cfg.versionfile_source,
                              })
-        cmds["py2exe"] = cmd_py2exe
+        cmds['py2exe'] = cmd_py2exe
 
     # we override different "sdist" commands for both environments
     if 'sdist' in cmds:
         _sdist = cmds['sdist']
-    elif "setuptools" in sys.modules:
+    elif 'setuptools' in sys.modules:
         from setuptools.command.sdist import sdist as _sdist
     else:
         from distutils.command.sdist import sdist as _sdist
 
     class cmd_sdist(_sdist):
         def run(self):
             versions = get_versions()
             self._versioneer_generated_versions = versions
             # unless we update this, the command will keep using the old
             # version
-            self.distribution.metadata.version = versions["version"]
+            self.distribution.metadata.version = versions['version']
             return _sdist.run(self)
 
         def make_release_tree(self, base_dir, files):
             root = get_root()
             cfg = get_config_from_root(root)
             _sdist.make_release_tree(self, base_dir, files)
             # now locate _version.py in the new base_dir directory
             # (remembering that it may be a hardlink) and replace it with an
             # updated value
             target_versionfile = os.path.join(base_dir, cfg.versionfile_source)
-            print("UPDATING %s" % target_versionfile)
+            print('UPDATING %s' % target_versionfile)
             write_to_version_file(target_versionfile,
                                   self._versioneer_generated_versions)
-    cmds["sdist"] = cmd_sdist
+    cmds['sdist'] = cmd_sdist
 
     return cmds
 
 
 CONFIG_ERROR = """
 setup.cfg is missing the necessary Versioneer configuration. You need
 a section like:
@@ -2010,131 +2010,131 @@
     """Do main VCS-independent setup function for installing Versioneer."""
     root = get_root()
     try:
         cfg = get_config_from_root(root)
     except (OSError, configparser.NoSectionError,
             configparser.NoOptionError) as e:
         if isinstance(e, (OSError, configparser.NoSectionError)):
-            print("Adding sample versioneer config to setup.cfg",
+            print('Adding sample versioneer config to setup.cfg',
                   file=sys.stderr)
-            with open(os.path.join(root, "setup.cfg"), "a") as f:
+            with open(os.path.join(root, 'setup.cfg'), 'a') as f:
                 f.write(SAMPLE_CONFIG)
         print(CONFIG_ERROR, file=sys.stderr)
         return 1
 
-    print(" creating %s" % cfg.versionfile_source)
-    with open(cfg.versionfile_source, "w") as f:
+    print(' creating %s' % cfg.versionfile_source)
+    with open(cfg.versionfile_source, 'w') as f:
         LONG = LONG_VERSION_PY[cfg.VCS]
-        f.write(LONG % {"DOLLAR": "$",
-                        "STYLE": cfg.style,
-                        "TAG_PREFIX": cfg.tag_prefix,
-                        "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                        "VERSIONFILE_SOURCE": cfg.versionfile_source,
+        f.write(LONG % {'DOLLAR': '$',
+                        'STYLE': cfg.style,
+                        'TAG_PREFIX': cfg.tag_prefix,
+                        'PARENTDIR_PREFIX': cfg.parentdir_prefix,
+                        'VERSIONFILE_SOURCE': cfg.versionfile_source,
                         })
 
     ipy = os.path.join(os.path.dirname(cfg.versionfile_source),
-                       "__init__.py")
+                       '__init__.py')
     if os.path.exists(ipy):
         try:
-            with open(ipy, "r") as f:
+            with open(ipy, 'r') as f:
                 old = f.read()
         except OSError:
-            old = ""
+            old = ''
         module = os.path.splitext(os.path.basename(cfg.versionfile_source))[0]
         snippet = INIT_PY_SNIPPET.format(module)
         if OLD_SNIPPET in old:
-            print(" replacing boilerplate in %s" % ipy)
-            with open(ipy, "w") as f:
+            print(' replacing boilerplate in %s' % ipy)
+            with open(ipy, 'w') as f:
                 f.write(old.replace(OLD_SNIPPET, snippet))
         elif snippet not in old:
-            print(" appending to %s" % ipy)
-            with open(ipy, "a") as f:
+            print(' appending to %s' % ipy)
+            with open(ipy, 'a') as f:
                 f.write(snippet)
         else:
-            print(" %s unmodified" % ipy)
+            print(' %s unmodified' % ipy)
     else:
         print(" %s doesn't exist, ok" % ipy)
         ipy = None
 
     # Make sure both the top-level "versioneer.py" and versionfile_source
     # (PKG/_version.py, used by runtime code) are in MANIFEST.in, so
     # they'll be copied into source distributions. Pip won't be able to
     # install the package without this.
-    manifest_in = os.path.join(root, "MANIFEST.in")
+    manifest_in = os.path.join(root, 'MANIFEST.in')
     simple_includes = set()
     try:
-        with open(manifest_in, "r") as f:
+        with open(manifest_in, 'r') as f:
             for line in f:
-                if line.startswith("include "):
+                if line.startswith('include '):
                     for include in line.split()[1:]:
                         simple_includes.add(include)
     except OSError:
         pass
     # That doesn't cover everything MANIFEST.in can do
     # (http://docs.python.org/2/distutils/sourcedist.html#commands), so
     # it might give some false negatives. Appending redundant 'include'
     # lines is safe, though.
-    if "versioneer.py" not in simple_includes:
+    if 'versioneer.py' not in simple_includes:
         print(" appending 'versioneer.py' to MANIFEST.in")
-        with open(manifest_in, "a") as f:
-            f.write("include versioneer.py\n")
+        with open(manifest_in, 'a') as f:
+            f.write('include versioneer.py\n')
     else:
         print(" 'versioneer.py' already in MANIFEST.in")
     if cfg.versionfile_source not in simple_includes:
         print(" appending versionfile_source ('%s') to MANIFEST.in" %
               cfg.versionfile_source)
-        with open(manifest_in, "a") as f:
-            f.write("include %s\n" % cfg.versionfile_source)
+        with open(manifest_in, 'a') as f:
+            f.write('include %s\n' % cfg.versionfile_source)
     else:
-        print(" versionfile_source already in MANIFEST.in")
+        print(' versionfile_source already in MANIFEST.in')
 
     # Make VCS-specific changes. For git, this means creating/changing
     # .gitattributes to mark _version.py for export-subst keyword
     # substitution.
     do_vcs_install(manifest_in, cfg.versionfile_source, ipy)
     return 0
 
 
 def scan_setup_py():
     """Validate the contents of setup.py against Versioneer's expectations."""
     found = set()
     setters = False
     errors = 0
-    with open("setup.py", "r") as f:
+    with open('setup.py', 'r') as f:
         for line in f.readlines():
-            if "import versioneer" in line:
-                found.add("import")
-            if "versioneer.get_cmdclass()" in line:
-                found.add("cmdclass")
-            if "versioneer.get_version()" in line:
-                found.add("get_version")
-            if "versioneer.VCS" in line:
+            if 'import versioneer' in line:
+                found.add('import')
+            if 'versioneer.get_cmdclass()' in line:
+                found.add('cmdclass')
+            if 'versioneer.get_version()' in line:
+                found.add('get_version')
+            if 'versioneer.VCS' in line:
                 setters = True
-            if "versioneer.versionfile_source" in line:
+            if 'versioneer.versionfile_source' in line:
                 setters = True
     if len(found) != 3:
-        print("")
-        print("Your setup.py appears to be missing some important items")
-        print("(but I might be wrong). Please make sure it has something")
-        print("roughly like the following:")
-        print("")
-        print(" import versioneer")
-        print(" setup( version=versioneer.get_version(),")
-        print("        cmdclass=versioneer.get_cmdclass(),  ...)")
-        print("")
+        print('')
+        print('Your setup.py appears to be missing some important items')
+        print('(but I might be wrong). Please make sure it has something')
+        print('roughly like the following:')
+        print('')
+        print(' import versioneer')
+        print(' setup( version=versioneer.get_version(),')
+        print('        cmdclass=versioneer.get_cmdclass(),  ...)')
+        print('')
         errors += 1
     if setters:
         print("You should remove lines like 'versioneer.VCS = ' and")
         print("'versioneer.versionfile_source = ' . This configuration")
-        print("now lives in setup.cfg, and should be removed from setup.py")
-        print("")
+        print('now lives in setup.cfg, and should be removed from setup.py')
+        print('')
         errors += 1
     return errors
 
 
-if __name__ == "__main__":
+if __name__ == '__main__':
     cmd = sys.argv[1]
-    if cmd == "setup":
+    if cmd == 'setup':
         errors = do_setup()
         errors += scan_setup_py()
         if errors:
             sys.exit(1)
```

