# Comparing `tmp/fleter-0.2.0.tar.gz` & `tmp/fleter-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fleter-0.2.0.tar", last modified: Sat Feb 25 05:42:07 2023, max compression
+gzip compressed data, was "fleter-0.3.0.tar", last modified: Fri Apr 14 13:51:20 2023, max compression
```

## Comparing `fleter-0.2.0.tar` & `fleter-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-02-25 05:42:07.937285 fleter-0.2.0/
--rw-rw-rw-   0        0        0     7517 2023-02-25 05:42:07.937285 fleter-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     7155 2022-11-15 14:25:17.000000 fleter-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-02-25 05:42:07.884452 fleter-0.2.0/fler/
--rw-rw-rw-   0        0        0       31 2022-09-03 04:30:00.000000 fleter-0.2.0/fler/__init__.py
--rw-rw-rw-   0        0        0      256 2022-09-03 05:00:48.000000 fleter-0.2.0/fler/test.py
--rw-rw-rw-   0        0        0     1087 2022-09-03 05:09:57.000000 fleter-0.2.0/fler/window.py
-drwxrwxrwx   0        0        0        0 2023-02-25 05:42:07.898983 fleter-0.2.0/fleter/
--rw-rw-rw-   0        0        0       74 2022-12-28 10:02:23.000000 fleter-0.2.0/fleter/__init__.py
--rw-rw-rw-   0        0        0     5697 2023-02-25 05:37:04.000000 fleter-0.2.0/fleter/buttons.py
--rw-rw-rw-   0        0        0    17315 2023-02-25 05:38:48.000000 fleter-0.2.0/fleter/controls.py
--rw-rw-rw-   0        0        0     4935 2022-11-14 03:57:28.000000 fleter-0.2.0/fleter/icons_browser.py
-drwxrwxrwx   0        0        0        0 2023-02-25 05:42:07.934283 fleter-0.2.0/fleter.egg-info/
--rw-rw-rw-   0        0        0     7517 2023-02-25 05:42:07.000000 fleter-0.2.0/fleter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-02-25 05:42:07.000000 fleter-0.2.0/fleter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-25 05:42:07.000000 fleter-0.2.0/fleter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-02-25 05:42:07.000000 fleter-0.2.0/fleter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       12 2023-02-25 05:42:07.000000 fleter-0.2.0/fleter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-02-25 05:42:07.000000 fleter-0.2.0/fleter.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-25 05:42:07.935287 fleter-0.2.0/fleter_demo/
--rw-rw-rw-   0        0        0      779 2022-11-16 01:26:16.000000 fleter-0.2.0/fleter_demo/__init__.py
--rw-rw-rw-   0        0        0       90 2022-07-04 10:17:18.000000 fleter-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-25 05:42:07.939481 fleter-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      851 2023-02-25 05:42:06.000000 fleter-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:51:20.523776 fleter-0.3.0/
+-rw-rw-rw-   0        0        0     8090 2023-04-14 13:51:20.524782 fleter-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7728 2023-04-14 13:32:27.000000 fleter-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 13:51:20.470458 fleter-0.3.0/fleter/
+-rw-rw-rw-   0        0        0       74 2023-04-09 08:02:47.000000 fleter-0.3.0/fleter/__init__.py
+-rw-rw-rw-   0        0        0     6602 2023-04-14 13:47:18.000000 fleter-0.3.0/fleter/buttons.py
+-rw-rw-rw-   0        0        0    16354 2023-04-14 13:38:13.000000 fleter-0.3.0/fleter/controls.py
+-rw-rw-rw-   0        0        0     4935 2023-04-09 08:02:47.000000 fleter-0.3.0/fleter/icons_browser.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:51:20.486256 fleter-0.3.0/fleter.egg-info/
+-rw-rw-rw-   0        0        0     8090 2023-04-14 13:51:20.000000 fleter-0.3.0/fleter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      385 2023-04-14 13:51:20.000000 fleter-0.3.0/fleter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 13:51:20.000000 fleter-0.3.0/fleter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-04-14 13:51:20.000000 fleter-0.3.0/fleter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       12 2023-04-14 13:51:20.000000 fleter-0.3.0/fleter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       35 2023-04-14 13:51:20.000000 fleter-0.3.0/fleter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-14 13:51:20.489279 fleter-0.3.0/fleter_demo/
+-rw-rw-rw-   0        0        0     1061 2023-04-14 13:35:56.000000 fleter-0.3.0/fleter_demo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-14 13:51:20.508493 fleter-0.3.0/fleter_designer/
+-rw-rw-rw-   0        0        0      931 2023-04-09 08:56:38.000000 fleter-0.3.0/fleter_designer/__init__.py
+-rw-rw-rw-   0        0        0      923 2023-04-09 12:22:57.000000 fleter-0.3.0/fleter_designer/__main__.py
+-rw-rw-rw-   0        0        0       90 2023-04-09 08:02:47.000000 fleter-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-14 13:51:20.529338 fleter-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      892 2023-04-14 13:31:04.000000 fleter-0.3.0/setup.py
```

### Comparing `fleter-0.2.0/PKG-INFO` & `fleter-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fleter
-Version: 0.2.0
+Version: 0.3.0
 Summary: flet extension library
 Author: XiangQinxi
 Author-email: XiangQinxi@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -15,15 +15,19 @@
 ![PyPI - Downloads](https://img.shields.io/pypi/dd/fleter?color=1d8bf8)
 ![PyPI - Downloads](https://img.shields.io/pypi/dw/fleter?color=1976d2)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/fleter?color=115293)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/fleter?color=115293)
 ![PyPI - Format](https://img.shields.io/pypi/format/fleter?color=115293)
 ![PyPI - License](https://img.shields.io/pypi/l/fleter?color=115293)
 
-一个flet的扩展组件库，提供一些常用组件及功能。
+flet的扩展组件库，提供一些常用组件及功能。
+
+>自`2.0`版本起我们将不支持`flet<0.4.0`的版本
+> 
+>自`3.0`版本起我们将不支持`flet<0.5.2`的版本
 
 ## ComboBox
 用于简化`Dropdown`的开发过程，`option`可以使用列表设置，如`["Hello", "World"]`。
 
 ![](https://xiangqinxi-development-resourse.netlify.app/_downloads/cdce347339a24c65eba9ab74cf25c918/ComboBox.gif)
 ```python
 import flet
@@ -217,15 +221,15 @@
 
 ![](https://xiangqinxi-development-resourse.netlify.app/_downloads/66614d49add24beda5ebe2d69c3f8196/SwichThemeButton.gif)
 ```python
 import flet
 import fleter
 
 def main(page: flet.Page):
-    swich_theme_button = fleter.SwichThemeButton(page)
+    swich_theme_button = fleter.SwitchThemeButton(page)
     page.add(
         swich_theme_button
     )
     page.update()
 
 flet.app(target=main)
 ```
@@ -243,14 +247,37 @@
         swich_theme_button
     )
     page.update()
 
 flet.app(target=main)
 ```
 
+## SwitchThemePopupMenuItem
+用于快速切换窗口主题的图标弹窗菜单组件。
+
+### 常规
+
+![](https://xiangqinxi.pages.dev/_images/SwitchThemePopupMenuItem.gif)
+```python
+import flet
+import fleter
+
+def main(page: flet.Page):
+    page.add(
+        flet.PopupMenuButton(
+            items=[
+                fleter.SwitchThemePopupMenuItem(page)
+            ]
+        )
+    )
+    page.update()
+
+flet.app(target=main)
+```
+
 ## SpinBox
 进步器，用于调整整数或浮点数的数值
 
 ![](https://xiangqinxi-development-resourse.netlify.app/_downloads/a30e33a93f13e0703ad5df21e0089217/SphinBox.gif)
 ```python
 import flet
 import fleter
```

### Comparing `fleter-0.2.0/README.md` & `fleter-0.3.0/fleter.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,33 @@
+Metadata-Version: 2.1
+Name: fleter
+Version: 0.3.0
+Summary: flet extension library
+Author: XiangQinxi
+Author-email: XiangQinxi@outlook.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
 # fleter
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/fleter)
 ![PyPI - Downloads](https://img.shields.io/pypi/dd/fleter?color=1d8bf8)
 ![PyPI - Downloads](https://img.shields.io/pypi/dw/fleter?color=1976d2)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/fleter?color=115293)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/fleter?color=115293)
 ![PyPI - Format](https://img.shields.io/pypi/format/fleter?color=115293)
 ![PyPI - License](https://img.shields.io/pypi/l/fleter?color=115293)
 
-一个flet的扩展组件库，提供一些常用组件及功能。
+flet的扩展组件库，提供一些常用组件及功能。
+
+>自`2.0`版本起我们将不支持`flet<0.4.0`的版本
+> 
+>自`3.0`版本起我们将不支持`flet<0.5.2`的版本
 
 ## ComboBox
 用于简化`Dropdown`的开发过程，`option`可以使用列表设置，如`["Hello", "World"]`。
 
 ![](https://xiangqinxi-development-resourse.netlify.app/_downloads/cdce347339a24c65eba9ab74cf25c918/ComboBox.gif)
 ```python
 import flet
@@ -205,15 +221,15 @@
 
 ![](https://xiangqinxi-development-resourse.netlify.app/_downloads/66614d49add24beda5ebe2d69c3f8196/SwichThemeButton.gif)
 ```python
 import flet
 import fleter
 
 def main(page: flet.Page):
-    swich_theme_button = fleter.SwichThemeButton(page)
+    swich_theme_button = fleter.SwitchThemeButton(page)
     page.add(
         swich_theme_button
     )
     page.update()
 
 flet.app(target=main)
 ```
@@ -231,14 +247,37 @@
         swich_theme_button
     )
     page.update()
 
 flet.app(target=main)
 ```
 
+## SwitchThemePopupMenuItem
+用于快速切换窗口主题的图标弹窗菜单组件。
+
+### 常规
+
+![](https://xiangqinxi.pages.dev/_images/SwitchThemePopupMenuItem.gif)
+```python
+import flet
+import fleter
+
+def main(page: flet.Page):
+    page.add(
+        flet.PopupMenuButton(
+            items=[
+                fleter.SwitchThemePopupMenuItem(page)
+            ]
+        )
+    )
+    page.update()
+
+flet.app(target=main)
+```
+
 ## SpinBox
 进步器，用于调整整数或浮点数的数值
 
 ![](https://xiangqinxi-development-resourse.netlify.app/_downloads/a30e33a93f13e0703ad5df21e0089217/SphinBox.gif)
 ```python
 import flet
 import fleter
@@ -298,8 +337,8 @@
 
     time = fleter.Time(tick)
     time.start("time", 10)
 
     page.update()
 
 flet.app(target=main)
-```
+```
```

### Comparing `fleter-0.2.0/fleter/buttons.py` & `fleter-0.3.0/fleter/buttons.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,35 +5,18 @@
 
     from flet import ButtonStyle
     from flet import Control, OptionalNumber
     from flet import Ref
 except:
     pass
 
-__all__ = [
-    # Widgets
-    "SwichThemeButton",
-    "CloseButton",
-    "MaximizeButton",
-    "MinimizeButton",
-
-    # Id
-    "CLOSE_ID",
-    "MAXIMIZE_ID",
-    "MINIMIZE_ID",
-
-    # Constant
-    "THEME_AUTO",
-    "THEME_LIGHT",
-    "THEME_DARK",
-]
-
 
 def close(page: flet.Page):
     page.window_close()
+    page.close_in_app_web_view()
 
 
 def maximize(page: flet.Page):
     if page.window_maximized:
         page.window_maximized = False
     elif not page.window_maximized:
         page.window_maximized = True
@@ -56,41 +39,46 @@
 
 
 def theme_dark(page: flet.Page):
     page.theme_mode = "dark"
     page.update()
 
 
+def theme_color(page: flet.Page, color):
+    page.theme = page.dark_theme = flet.Theme().use_material3
+    page.update()
+
+
 CLOSE_ID = close
 
 MAXIMIZE_ID = maximize
 
 MINIMIZE_ID = minimize
 
 THEME_AUTO = theme_auto
 
 THEME_LIGHT = theme_light
 
 THEME_DARK = theme_dark
 
 
-class SwichThemeButton(flet.IconButton):
+class SwitchThemeButton(flet.IconButton):
     __name__ = "fleter.SwichThemeButton"
 
     def __init__(self,
                  page: flet.Page,
 
                  on_click=None,
 
                  light_icon=flet.icons.BRIGHTNESS_7,
                  dark_icon=flet.icons.BRIGHTNESS_5,
                  system_icon=flet.icons.BRIGHTNESS_AUTO,
                  has_system: bool = True,
                  ):
-        super(SwichThemeButton, self).__init__(
+        super(SwitchThemeButton, self).__init__(
             on_click=on_click,
         )
 
         self._page = page
         if has_system:
             THEME_AUTO(self._page)
         else:
@@ -163,14 +151,50 @@
             elif self._page.theme_mode == "dark":
                 self.icon = self._light_icon
                 THEME_LIGHT(self._page)
 
         self._page.update()
 
 
+class SwitchThemePopupMenuItem(flet.PopupMenuItem):
+    __name__ = "fleter.SwichThemePopupMenuItem"
+
+    def __init__(self,
+                 page: flet.Page,
+
+                 *args,
+
+                 text: str = "Toggle Dark Theme",
+
+                 light_icon=flet.icons.BRIGHTNESS_7,
+                 dark_icon=flet.icons.BRIGHTNESS_5,
+
+                 **kwargs
+                 ):
+        self._light_icon = light_icon
+        self._dark_icon = dark_icon
+
+        page.theme_mode = "light"
+
+        super().__init__(*args, text=text, checked=False, on_click=lambda evt: self.swich_theme(), **kwargs)
+
+        self._page = page
+
+    def swich_theme(self):
+        if self._page.theme_mode == "light":
+            self.icon = self._dark_icon
+            self.checked = True
+            THEME_DARK(self._page)
+
+        elif self._page.theme_mode == "dark":
+            self.icon = self._light_icon
+            self.checked = False
+            THEME_LIGHT(self._page)
+
+
 class CloseButton(flet.IconButton):
     __name__ = "fleter.CloseButton"
 
     def __init__(self,
                  page: flet.Page,
                  icon=flet.icons.CLOSE_ROUNDED,
                  on_click=None,
@@ -229,7 +253,8 @@
         if on_click is None:
             self.on_click = lambda _: self.minimize()
 
     def minimize(self):
         self._page.window_minimized = True
         MINIMIZE_ID(self._page)
         self._page.update()
+
```

### Comparing `fleter-0.2.0/fleter/controls.py` & `fleter-0.3.0/fleter/controls.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,14 @@
 import flet
 from typing import Optional, Literal
 from flet import icons, TextAlign
 from flet import Control
 from fleter import buttons
 
 
-__all__ = [
-    "animation_show",
-    "empty",
-    "enabled_harmonysans",
-    "enable_material3_theme",
-    "disable_material3_theme",
-    "AudioControlBar",
-    "ComboBox",
-    "Editor",
-    "HeaderBar",
-    "Manage",
-    "NoteBook",
-    "SpinBox",
-    "Time",
-]
-
 
 def animation_show(container: flet.Container, time=300):
     container.animate_opacity = 0
     container.opacity = False
     container.animate_opacity = time
     container.opacity = True
     container.update()
@@ -64,25 +48,19 @@
         super().__init__()
 
         self._play_button = flet.IconButton()
 
 
 class ComboBox(flet.Dropdown):
     def __init__(self,
-                 #
-                 # DropDown Specific
-                 #
-                 value: Optional[str] = None,
-                 autofocus: Optional[bool] = None,
                  options: Optional[str] = [""],
-                 on_change=None,
-                 on_focus=None,
-                 on_blur=None,
+                 *args,
+                 **kwargs
                  ):
-        super(ComboBox, self).__init__()
+        super(ComboBox, self).__init__(*args, **kwargs)
 
         self._option = []
         self._options = options
 
         self.option = self._options
 
     @property
@@ -100,16 +78,19 @@
                 self._option.append(flet.dropdown.Option(item[0], disabled=disabled))
             else:
                 self._option.append(flet.dropdown.Option(item))
         self.options = self._option
 
 
 class Editor(flet.TextField):
-    def __init__(self):
-        super().__init__(min_lines=100000, expand=True, multiline=True)
+    def __init__(self,
+                 *args,
+                 **kwargs
+                 ):
+        super().__init__(*args, **kwargs, min_lines=100000, expand=True, multiline=True)
 
 
 class FilpView():
     def __init__(self):
         pass
 
 
@@ -118,23 +99,26 @@
                  page: flet.Page,
                  has_close: bool = True,
                  has_maximize: bool = False,
                  has_minimize: bool = False,
                  frameless: bool = False,
                  title: str = "",
                  title_align: TextAlign = "center",
+
+                 *args,
+                 **kwargs
                  ):
         """
 
         :param page: 为被设置页面窗口
         :param has_close: 决定是否有关闭按钮
         :param title: 设置标题栏的标题
         :param title_align: 设置标题栏的标题对齐
         """
-        super(HeaderBar, self).__init__()
+        super(HeaderBar, self).__init__(*args, **kwargs)
         self._page = page
         if frameless:
             self._page.window_frameless = True
         else:
             self._page.window_title_bar_hidden = True
             self._page.window_title_bar_buttons_hidden = True
 
@@ -304,44 +288,14 @@
     def minimize_button(self, control: Control):
         self._minimize_button = control
 
     def show(self):
         self._page.add(self)
 
 
-class Manage(object):
-    def __init__(self, page: flet.Page):
-        self.build(page)
-
-    def build(self, page: flet.Page):
-        self._page = page
-        self._page.update()
-
-    @property
-    def page(self):
-        return self._page
-
-    @page.setter
-    def page(self, page: flet.Page):
-        self.page = page
-
-    def resize(self, width: int = None, height: int = None):
-        if width is not None:
-            self._page.window_width = width
-        if height is not None:
-            self._page.window_height = height
-
-    def create_titlebar(self, has_close: bool = True,
-                        title: str = "",
-                        title_align: Literal["left", "right", "center", "justify", "start", "end"] = "left"):
-        titlebar = HeaderBar(self._page, has_close=has_close, title=title, title_align=title_align)
-        titlebar.show()
-        return titlebar
-
-
 class NoteBook(flet.Tabs):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def create(self, text: str = "", content=None, note_content=None, icon=None):
         tab = flet.Tab(text=text, content=content, tab_content=note_content, icon=icon)
         return tab
@@ -556,22 +510,29 @@
 
 
 class Widget(flet.UserControl):
     def build(self):
         pass
 
 
+class PopupColorItem(flet.PopupMenuItem):
+    def __init__(self, color, name):
+        flet.PopupMenuItem.__init__(self)
+        self.content = flet.Row(controls=[
+            flet.Icon(name=flet.icons.COLOR_LENS_OUTLINED, color=color),
+            flet.Text(name)],
+        )
+        self.on_click = self.seed_color_changed
+        self.data = color
+
+    def seed_color_changed(self, e):
+        self.page.theme = self.page.dark_theme = flet.theme.Theme(color_scheme_seed=self.data)
+        self.page.update()
+
+
 if __name__ == '__main__':
     def main(page: flet.Page):
-        enabled_harmonysans(page)
-        notebook = NoteBook()
-        tab1 = notebook.create("Hello")
-        tab2 = notebook.create_with_can_close()
-        notebook.add(tab1)
 
-        page.add(
-            notebook
-        )
         page.update()
 
 
     flet.app(target=main)
```

### Comparing `fleter-0.2.0/fleter/icons_browser.py` & `fleter-0.3.0/fleter/icons_browser.py`

 * *Files identical despite different names*

### Comparing `fleter-0.2.0/fleter.egg-info/PKG-INFO` & `fleter-0.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,21 @@
-Metadata-Version: 2.1
-Name: fleter
-Version: 0.2.0
-Summary: flet extension library
-Author: XiangQinxi
-Author-email: XiangQinxi@outlook.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
 # fleter
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/fleter)
 ![PyPI - Downloads](https://img.shields.io/pypi/dd/fleter?color=1d8bf8)
 ![PyPI - Downloads](https://img.shields.io/pypi/dw/fleter?color=1976d2)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/fleter?color=115293)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/fleter?color=115293)
 ![PyPI - Format](https://img.shields.io/pypi/format/fleter?color=115293)
 ![PyPI - License](https://img.shields.io/pypi/l/fleter?color=115293)
 
-一个flet的扩展组件库，提供一些常用组件及功能。
+flet的扩展组件库，提供一些常用组件及功能。
+
+>自`2.0`版本起我们将不支持`flet<0.4.0`的版本
+> 
+>自`3.0`版本起我们将不支持`flet<0.5.2`的版本
 
 ## ComboBox
 用于简化`Dropdown`的开发过程，`option`可以使用列表设置，如`["Hello", "World"]`。
 
 ![](https://xiangqinxi-development-resourse.netlify.app/_downloads/cdce347339a24c65eba9ab74cf25c918/ComboBox.gif)
 ```python
 import flet
@@ -217,15 +209,15 @@
 
 ![](https://xiangqinxi-development-resourse.netlify.app/_downloads/66614d49add24beda5ebe2d69c3f8196/SwichThemeButton.gif)
 ```python
 import flet
 import fleter
 
 def main(page: flet.Page):
-    swich_theme_button = fleter.SwichThemeButton(page)
+    swich_theme_button = fleter.SwitchThemeButton(page)
     page.add(
         swich_theme_button
     )
     page.update()
 
 flet.app(target=main)
 ```
@@ -243,14 +235,37 @@
         swich_theme_button
     )
     page.update()
 
 flet.app(target=main)
 ```
 
+## SwitchThemePopupMenuItem
+用于快速切换窗口主题的图标弹窗菜单组件。
+
+### 常规
+
+![](https://xiangqinxi.pages.dev/_images/SwitchThemePopupMenuItem.gif)
+```python
+import flet
+import fleter
+
+def main(page: flet.Page):
+    page.add(
+        flet.PopupMenuButton(
+            items=[
+                fleter.SwitchThemePopupMenuItem(page)
+            ]
+        )
+    )
+    page.update()
+
+flet.app(target=main)
+```
+
 ## SpinBox
 进步器，用于调整整数或浮点数的数值
 
 ![](https://xiangqinxi-development-resourse.netlify.app/_downloads/a30e33a93f13e0703ad5df21e0089217/SphinBox.gif)
 ```python
 import flet
 import fleter
@@ -310,8 +325,8 @@
 
     time = fleter.Time(tick)
     time.start("time", 10)
 
     page.update()
 
 flet.app(target=main)
-```
+```
```

### Comparing `fleter-0.2.0/fleter_demo/__init__.py` & `fleter-0.3.0/fleter_demo/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,23 @@
 import flet
 import fleter
-
+import flet_core
 
 def run():
     def main(page: flet.Page):
         headerbar = fleter.HeaderBar(page, has_close=True, has_minimize=True, has_maximize=True)
-        headerbar.controls.insert(1, fleter.SwichThemeButton(page))
+        headerbar.controls.insert(1, fleter.SwitchThemeButton(page))
+        headerbar.controls.insert(
+            2,
+            flet.PopupMenuButton(
+                items=(
+                    fleter.PopupColorItem(flet_core.colors.BLUE_500, "Blue")
+                )
+            )
+        )
 
         combobox = fleter.ComboBox(
             options=[
                 "normal",
                 ("disabled", True),
                 ("active", False),
             ]
@@ -24,12 +32,13 @@
 
         page.add(
             headerbar,
             notebook,
         )
         page.update()
 
-    flet.app(target=main)
+        print(page.controls)
 
+    flet.app(target=main)
 
 if __name__ == '__main__':
     run()
```

### Comparing `fleter-0.2.0/setup.py` & `fleter-0.3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 from setuptools import find_packages, setup
 
 setup(
     name="fleter",
-    version="0.2.0",
+    version="0.3.0",
     author="XiangQinxi",
     author_email="XiangQinxi@outlook.com",
     description="flet extension library",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     python_requires=">=3.7",
     install_requires=[
-        "flet>=0.4.0"
+        "flet>=0.5.2"
     ],
-    packages=find_packages(exclude=["*.tests", "*.tests.*", "tests"]),
+    packages=find_packages(
+        exclude=["*.tests", "*.tests.*", "tests", "docs", "fleter_test"]
+
+    ),
     package_data={"fleter": ["*.ttc"]},
     include_package_data=True,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

