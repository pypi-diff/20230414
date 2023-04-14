# Comparing `tmp/planetmapper-1.6.1.tar.gz` & `tmp/planetmapper-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "planetmapper-1.6.1.tar", last modified: Thu Apr 13 16:41:52 2023, max compression
+gzip compressed data, was "planetmapper-1.6.2.tar", last modified: Fri Apr 14 13:18:35 2023, max compression
```

## Comparing `planetmapper-1.6.1.tar` & `planetmapper-1.6.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:41:52.399560 planetmapper-1.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-04-13 16:41:52.399560 planetmapper-1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-04-13 16:41:41.000000 planetmapper-1.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:41:52.395560 planetmapper-1.6.1/planetmapper/
--rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-04-13 16:41:41.000000 planetmapper-1.6.1/planetmapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13940 2023-04-13 16:41:41.000000 planetmapper-1.6.1/planetmapper/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-13 16:41:41.000000 planetmapper-1.6.1/planetmapper/basic_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    72134 2023-04-13 16:41:41.000000 planetmapper-1.6.1/planetmapper/body.py
--rw-r--r--   0 runner    (1001) docker     (123)    99198 2023-04-13 16:41:41.000000 planetmapper-1.6.1/planetmapper/body_xy.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-13 16:41:41.000000 planetmapper-1.6.1/planetmapper/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:41:52.395560 planetmapper-1.6.1/planetmapper/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-04-13 16:41:41.000000 planetmapper-1.6.1/planetmapper/data/rings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-13 16:41:41.000000 planetmapper-1.6.1/planetmapper/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)   108552 2023-04-13 16:41:41.000000 planetmapper-1.6.1/planetmapper/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-04-13 16:41:41.000000 planetmapper-1.6.1/planetmapper/kernel_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    42961 2023-04-13 16:41:41.000000 planetmapper-1.6.1/planetmapper/observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7855 2023-04-13 16:41:41.000000 planetmapper-1.6.1/planetmapper/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)    12553 2023-04-13 16:41:41.000000 planetmapper-1.6.1/planetmapper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:41:52.395560 planetmapper-1.6.1/planetmapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-04-13 16:41:52.000000 planetmapper-1.6.1/planetmapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-13 16:41:52.000000 planetmapper-1.6.1/planetmapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 16:41:52.000000 planetmapper-1.6.1/planetmapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-13 16:41:52.000000 planetmapper-1.6.1/planetmapper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-13 16:41:52.000000 planetmapper-1.6.1/planetmapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-13 16:41:52.000000 planetmapper-1.6.1/planetmapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-13 16:41:41.000000 planetmapper-1.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 16:41:52.399560 planetmapper-1.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-04-13 16:41:41.000000 planetmapper-1.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 16:41:52.399560 planetmapper-1.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10773 2023-04-13 16:41:41.000000 planetmapper-1.6.1/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-13 16:41:41.000000 planetmapper-1.6.1/tests/test_basic_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    20532 2023-04-13 16:41:41.000000 planetmapper-1.6.1/tests/test_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    25253 2023-04-13 16:41:41.000000 planetmapper-1.6.1/tests/test_body_xy.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-13 16:41:41.000000 planetmapper-1.6.1/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-13 16:41:41.000000 planetmapper-1.6.1/tests/test_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-13 16:41:41.000000 planetmapper-1.6.1/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)    17684 2023-04-13 16:41:41.000000 planetmapper-1.6.1/tests/test_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-04-13 16:41:41.000000 planetmapper-1.6.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:18:35.173646 planetmapper-1.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-04-14 13:18:35.173646 planetmapper-1.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-04-14 13:18:24.000000 planetmapper-1.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:18:35.169646 planetmapper-1.6.2/planetmapper/
+-rw-r--r--   0 runner    (1001) docker     (123)     4318 2023-04-14 13:18:24.000000 planetmapper-1.6.2/planetmapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13940 2023-04-14 13:18:24.000000 planetmapper-1.6.2/planetmapper/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-04-14 13:18:24.000000 planetmapper-1.6.2/planetmapper/basic_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72134 2023-04-14 13:18:24.000000 planetmapper-1.6.2/planetmapper/body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99198 2023-04-14 13:18:24.000000 planetmapper-1.6.2/planetmapper/body_xy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-14 13:18:24.000000 planetmapper-1.6.2/planetmapper/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:18:35.173646 planetmapper-1.6.2/planetmapper/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-04-14 13:18:24.000000 planetmapper-1.6.2/planetmapper/data/rings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-14 13:18:24.000000 planetmapper-1.6.2/planetmapper/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)   109295 2023-04-14 13:18:24.000000 planetmapper-1.6.2/planetmapper/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-04-14 13:18:24.000000 planetmapper-1.6.2/planetmapper/kernel_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43334 2023-04-14 13:18:24.000000 planetmapper-1.6.2/planetmapper/observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7855 2023-04-14 13:18:24.000000 planetmapper-1.6.2/planetmapper/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12553 2023-04-14 13:18:24.000000 planetmapper-1.6.2/planetmapper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:18:35.169646 planetmapper-1.6.2/planetmapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-04-14 13:18:35.000000 planetmapper-1.6.2/planetmapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-14 13:18:35.000000 planetmapper-1.6.2/planetmapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 13:18:35.000000 planetmapper-1.6.2/planetmapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-14 13:18:35.000000 planetmapper-1.6.2/planetmapper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-14 13:18:35.000000 planetmapper-1.6.2/planetmapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-14 13:18:35.000000 planetmapper-1.6.2/planetmapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-14 13:18:24.000000 planetmapper-1.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 13:18:35.173646 planetmapper-1.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-04-14 13:18:24.000000 planetmapper-1.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 13:18:35.173646 planetmapper-1.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10773 2023-04-14 13:18:24.000000 planetmapper-1.6.2/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-14 13:18:24.000000 planetmapper-1.6.2/tests/test_basic_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20532 2023-04-14 13:18:24.000000 planetmapper-1.6.2/tests/test_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25253 2023-04-14 13:18:24.000000 planetmapper-1.6.2/tests/test_body_xy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-14 13:18:24.000000 planetmapper-1.6.2/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-14 13:18:24.000000 planetmapper-1.6.2/tests/test_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-14 13:18:24.000000 planetmapper-1.6.2/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17684 2023-04-14 13:18:24.000000 planetmapper-1.6.2/tests/test_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-04-14 13:18:24.000000 planetmapper-1.6.2/tests/test_utils.py
```

### Comparing `planetmapper-1.6.1/PKG-INFO` & `planetmapper-1.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planetmapper
-Version: 1.6.1
+Version: 1.6.2
 Summary: A Python module for visualising, navigating and mapping Solar System observations
 Home-page: https://github.com/ortk95/planetmapper
 Download-URL: https://pypi.org/project/planetmapper/
 Author: Oliver King
 Author-email: oliver.king95@gmail.com
 Project-URL: Documentation, https://planetmapper.readthedocs.io/
 Project-URL: GitHub, https://github.com/ortk95/planetmapper
```

### Comparing `planetmapper-1.6.1/README.md` & `planetmapper-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.1/planetmapper/__init__.py` & `planetmapper-1.6.2/planetmapper/__init__.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.1/planetmapper/base.py` & `planetmapper-1.6.2/planetmapper/base.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.1/planetmapper/basic_body.py` & `planetmapper-1.6.2/planetmapper/basic_body.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.1/planetmapper/body.py` & `planetmapper-1.6.2/planetmapper/body.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.1/planetmapper/body_xy.py` & `planetmapper-1.6.2/planetmapper/body_xy.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.1/planetmapper/data/rings.json` & `planetmapper-1.6.2/planetmapper/data/rings.json`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.1/planetmapper/data_loader.py` & `planetmapper-1.6.2/planetmapper/data_loader.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.1/planetmapper/gui.py` & `planetmapper-1.6.2/planetmapper/gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg, NavigationToolbar2Tk
 from matplotlib.backend_bases import MouseEvent, MouseButton
 from matplotlib.text import Text
 import matplotlib as mpl
 
 from matplotlib.backends._backend_tk import NavigationToolbar2Tk  # TODO delete this?
 
-from . import base, data_loader, utils
+from . import base, common, data_loader, utils
 from .body import Body, BasicBody, NotFoundError
 from .body_xy import _MapKwargs
 from .observation import Observation
 from . import progress
 
 
 Widget = TypeVar('Widget', bound=tk.Widget)
@@ -88,22 +88,20 @@
 GRID_INTERVALS = ['10', '30', '45', '90']
 CMAPS = ['gray', 'viridis', 'plasma', 'inferno', 'magma', 'cividis']
 LIMIT_TYPES = ['absolute', 'percentile']
 
 MAP_INTERPOLATIONS = ('nearest', 'linear', 'quadratic', 'cubic')
 MAP_PROJECTIONS = ('rectangular', 'orthographic', 'azimuthal')
 
-DEFAULT_HINT = (
-    'Use the various options in "Find disc" to automatically adjust the disc position'
-)
+DEFAULT_HINT = ''
 
 
 def _main(*args):
     """Called with `planetmapper` from the command line"""
-    print('Launching planetmapper...')
+    print(f'Launching PlanetMapper {common.__version__}')
     gui = GUI()
     if args:
         gui.set_observation(Observation(args[0]))
     gui.run()
 
 
 class Quit(Exception):
@@ -317,14 +315,15 @@
         else:
             self.plot_settings['_']['image_mode'] = 'sum'
 
         if self.gui_built:
             self.run_all_ui_callbacks()
             self.rebuild_plot()
             self.root.title(self.get_observation().get_description(multiline=False))
+            self.reset_help_hint()
 
         self.click_locations = []
         self.clear_click_location()
 
     def get_observation(self) -> Observation:
         if self._observation is None:
             self.load_observation()
@@ -434,27 +433,27 @@
             frame=frame,
             label='Rotation',
             buttons=[
                 ('↺', 'anticlockwise', self.rotate_left, 0, 0),
                 ('↻', 'clockwise', self.rotate_right, 1, 0),
             ],
             button_tooltip_base='Rotate fitted disc {hint}',
-            entry_tooltip='Set the rotation (in degrees) of the disc',
+            entry_tooltip='Set the rotation of the disc in degrees',
             numeric_entries=[('rotation', 'Rotation (°)')],
         )
 
         self.build_main_controls_section(
             frame=frame,
             label='Size',
             buttons=[
                 ('-', 'Decrease', self.decrease_radius, 0, 0),
                 ('+', 'Increase', self.increase_radius, 1, 0),
             ],
             button_tooltip_base='{hint} fitted disc radius',
-            entry_tooltip='Set the equatorial radius, r0, in pixels of the disc',
+            entry_tooltip='Set the equatorial radius of the disc, r0, in pixels',
             numeric_entries=[
                 ('r0', 'r0'),
                 ('plate_scale_arcsec', 'arcsec/pixel'),
                 ('plate_scale_km', 'km/pixel'),
             ],
             add_callbacks=['r0', 'plate_scale_arcsec', 'plate_scale_km'],
         )
@@ -669,35 +668,43 @@
         return button_command
 
     def build_help_hint(self) -> None:
         frame = ttk.Frame(self.hint_frame)
         frame.pack(fill='x', padx=5, pady=1)
         self.help_hint = ttk.Label(frame, text=DEFAULT_HINT)
         self.help_hint.pack(side='left')
+        self.help_hint.bind('<Enter>', lambda e: self.reset_help_hint(hover=True))
+        self.help_hint.bind('<Leave>', lambda e: self.reset_help_hint())
+        self.reset_help_hint()
+
+    def set_help_hint(self, msg: str, *, color: str = 'black'):
+        self.help_hint.configure(text=msg, foreground=color)
+
+    def reset_help_hint(self, *, hover: bool = False):
+        path = self.get_observation().path
+        if path is None:
+            msg = ''
+        else:
+            msg = path if hover else os.path.basename(path)
+        self.set_help_hint(msg, color='gray50')
 
     def add_tooltip(
-        self, widget: Widget, msg: str, shortcut_fn: Callable | None = None
+        self, widget: Widget, msg: str, shortcut_fn: Callable | None = None, **kw
     ) -> Widget:
         if shortcut_fn is not None:
             keys = self.shortcuts.get(shortcut_fn, None)
             if keys is not None:
                 key = keys[0]
                 key = key.replace('<less>', '<').upper()
                 if key[0] == '<' and key[-1] == '>' and len(key) > 2:
                     key = key[1:-1]
                 msg = f'{msg} (keyboard shortcut: {key})'
 
-        def f_enter(event):
-            self.help_hint.configure(text=msg)
-
-        def f_leave(event):
-            self.help_hint.configure(text='')
-
-        widget.bind('<Enter>', f_enter)
-        widget.bind('<Leave>', f_leave)
+        widget.bind('<Enter>', lambda e: self.set_help_hint(msg, **kw))
+        widget.bind('<Leave>', lambda e: self.reset_help_hint())
         return widget
 
     # Coords
     def build_coords_tab(self):
         top_level_frame = ttk.Frame(self.notebook)
         top_level_frame.pack()
         self.notebook.add(top_level_frame, text='Coords')
@@ -977,14 +984,19 @@
         )
         self.toolbar.pack(side='bottom', fill='x')
 
         self.fig.canvas.callbacks.connect(
             'button_press_event', self.figure_click_callback
         )
 
+        self.add_tooltip(
+            self.canvas.get_tk_widget(),
+            'Customise the displayed data, colour scales and plotted features in the "Settings" tab',
+        )
+
     def rebuild_plot(self) -> None:
         self.transform = (
             self.get_observation().matplotlib_radec2xy_transform() + self.ax.transData
         )
         self.replot_all()
         self.format_plot()
         self.update_plot()
@@ -2021,19 +2033,19 @@
                 title=f'Error saving files',
                 message=f'Error: {e}' + '\n\nSee terminal for more details',
             )
             return False
         finally:
             self.gui.get_observation()._remove_progress_hook()
 
-        self.gui.help_hint.configure(
-            text='File{s} saved successfully'.format(
-                s='s' if save_nav and save_map else ''
-            )
+        self.gui.set_help_hint(
+            'File{s} saved successfully'.format(s='s' if save_nav and save_map else ''),
+            color='green',
         )
+
         if keep_open:
             return False
         return True
 
 
 class SavingProgress(Popup):
     def __init__(
@@ -2382,15 +2394,17 @@
                     textvariable=textvariable,
                     from_=0,
                     to=idx_max,
                     increment=1,
                     width=10,
                 )
 
-        self.grid: list[tuple[tk.Widget, tk.Widget, set[IMAGE_MODE|Literal['_readonly']]]] = [
+        self.grid: list[
+            tuple[tk.Widget, tk.Widget, set[IMAGE_MODE | Literal['_readonly']]]
+        ] = [
             (
                 ttk.Label(frame, text='Wavelength index (single): '),
                 IndexInput(self.image_idx_single),
                 {'single'},
             ),
             (
                 ttk.Label(frame, text='Wavelength index (red): '),
@@ -3052,24 +3066,26 @@
                 path_effects.Normal(),
             ]  # type: ignore
         )
 
 
 class CustomNavigationToolbar(NavigationToolbar2Tk):
     def __init__(self, canvas, window, *, pack_toolbar: bool = True, gui: GUI) -> None:
-        # Default tooltips don't work with tk (on my laptop with dark mode at lease)
+        # Default tooltips don't work with tk (on my laptop with dark mode at least)
         # so disable them here by setting to None, then use our custom tooltips instead.
-        # This list also removes the Save and Subplots buttons which we don't want.
+        # This list also removes the and Subplots button which we don't want.
         self.toolitems = (
             ('Home', None, 'home', 'home'),
             ('Back', None, 'back', 'back'),
             ('Forward', None, 'forward', 'forward'),
             (None, None, None, None),
             ('Pan', None, 'move', 'pan'),
             ('Zoom', None, 'zoom_to_rect', 'zoom'),
+            (None, None, None, None),
+            ('Save', None, 'filesave', 'save_figure'),
         )
         super().__init__(canvas, window, pack_toolbar=pack_toolbar)
         try:
             self._message_label.configure(foreground='#666666')
         except:
             pass
         try:
```

### Comparing `planetmapper-1.6.1/planetmapper/kernel_downloader.py` & `planetmapper-1.6.2/planetmapper/kernel_downloader.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.1/planetmapper/observation.py` & `planetmapper-1.6.2/planetmapper/observation.py`

 * *Files 2% similar despite different names*

```diff
@@ -460,20 +460,29 @@
     def fit_disc_radius(self) -> None:
         """
         Automatically find and set `r0` using aperture photometry.
 
         This routine calculates the brightness in concentric annular apertures around
         `(x0, y0)` and sets `r0` as the radius where the brightness decreases the
         fastest. Note that this uses circular apertures, so will be less reliable for
-        targets with greater flattening.
+        targets with greater flattening and may not work well for targets which are not
+        entirely in the image frame.
+
+        Raises:
+            ValueError: if `x0` or `y0` are not within the image frame.
         """
+        if not self._xy_in_image_frame(self.get_x0(), self.get_y0()):
+            raise ValueError(
+                'x0 and y0 must be within the image frame to fit the radius'
+            )
+
         img = self._get_img_for_fitting()
         centroid = np.array([self.get_x0(), self.get_y0()])
 
-        r_ceil = int(min(*centroid, *(img.shape - centroid)))
+        r_ceil = max(int(min(*centroid, *(img.shape - centroid))), 2)
         if r_ceil > 100:
             r_list = np.linspace(1, r_ceil + 1, 100)
         else:
             r_list = np.array(range(1, r_ceil + 1))
         apertures = [photutils.aperture.CircularAperture(centroid, r) for r in r_list]
 
         val_list = []
```

### Comparing `planetmapper-1.6.1/planetmapper/progress.py` & `planetmapper-1.6.2/planetmapper/progress.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.1/planetmapper/utils.py` & `planetmapper-1.6.2/planetmapper/utils.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.1/planetmapper.egg-info/PKG-INFO` & `planetmapper-1.6.2/planetmapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planetmapper
-Version: 1.6.1
+Version: 1.6.2
 Summary: A Python module for visualising, navigating and mapping Solar System observations
 Home-page: https://github.com/ortk95/planetmapper
 Download-URL: https://pypi.org/project/planetmapper/
 Author: Oliver King
 Author-email: oliver.king95@gmail.com
 Project-URL: Documentation, https://planetmapper.readthedocs.io/
 Project-URL: GitHub, https://github.com/ortk95/planetmapper
```

### Comparing `planetmapper-1.6.1/planetmapper.egg-info/SOURCES.txt` & `planetmapper-1.6.2/planetmapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.1/setup.py` & `planetmapper-1.6.2/setup.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.1/tests/test_base.py` & `planetmapper-1.6.2/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.1/tests/test_basic_body.py` & `planetmapper-1.6.2/tests/test_basic_body.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.1/tests/test_body.py` & `planetmapper-1.6.2/tests/test_body.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.1/tests/test_body_xy.py` & `planetmapper-1.6.2/tests/test_body_xy.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.1/tests/test_init.py` & `planetmapper-1.6.2/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.1/tests/test_observation.py` & `planetmapper-1.6.2/tests/test_observation.py`

 * *Files identical despite different names*

### Comparing `planetmapper-1.6.1/tests/test_utils.py` & `planetmapper-1.6.2/tests/test_utils.py`

 * *Files identical despite different names*

