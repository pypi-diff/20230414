# Comparing `tmp/CTkColorPicker-0.4.0.tar.gz` & `tmp/CTkColorPicker-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CTkColorPicker-0.4.0.tar", last modified: Sat Apr  1 16:18:23 2023, max compression
+gzip compressed data, was "CTkColorPicker-0.5.0.tar", last modified: Fri Apr 14 11:22:56 2023, max compression
```

## Comparing `CTkColorPicker-0.4.0.tar` & `CTkColorPicker-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-01 16:18:23.206728 CTkColorPicker-0.4.0/
-drwxrwxrwx   0        0        0        0 2023-04-01 16:18:23.191098 CTkColorPicker-0.4.0/CTkColorPicker/
--rw-rw-rw-   0        0        0      221 2023-04-01 16:07:26.000000 CTkColorPicker-0.4.0/CTkColorPicker/__init__.py
--rw-rw-rw-   0        0        0   111614 2020-05-30 05:51:52.000000 CTkColorPicker-0.4.0/CTkColorPicker/color_wheel.png
--rw-rw-rw-   0        0        0     6346 2023-04-01 16:10:31.000000 CTkColorPicker-0.4.0/CTkColorPicker/ctk_color_picker.py
--rw-rw-rw-   0        0        0      933 2020-05-30 05:51:52.000000 CTkColorPicker-0.4.0/CTkColorPicker/target.png
-drwxrwxrwx   0        0        0        0 2023-04-01 16:18:23.206728 CTkColorPicker-0.4.0/CTkColorPicker.egg-info/
--rw-rw-rw-   0        0        0     1823 2023-04-01 16:18:23.000000 CTkColorPicker-0.4.0/CTkColorPicker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      344 2023-04-01 16:18:23.000000 CTkColorPicker-0.4.0/CTkColorPicker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       73 2023-04-01 16:18:23.000000 CTkColorPicker-0.4.0/CTkColorPicker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-04-01 16:18:23.000000 CTkColorPicker-0.4.0/CTkColorPicker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-01 16:18:23.000000 CTkColorPicker-0.4.0/CTkColorPicker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7048 2022-11-20 16:16:56.000000 CTkColorPicker-0.4.0/LICENSE
--rw-rw-rw-   0        0        0     1823 2023-04-01 16:18:23.206728 CTkColorPicker-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     1144 2023-04-01 16:14:57.000000 CTkColorPicker-0.4.0/README.md
--rw-rw-rw-   0        0        0      607 2023-04-01 16:18:23.222359 CTkColorPicker-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1317 2023-04-01 16:17:56.000000 CTkColorPicker-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 11:22:56.306281 CTkColorPicker-0.5.0/
+drwxrwxrwx   0        0        0        0 2023-04-14 11:22:56.286117 CTkColorPicker-0.5.0/CTkColorPicker/
+-rw-rw-rw-   0        0        0      221 2023-04-14 10:14:45.000000 CTkColorPicker-0.5.0/CTkColorPicker/__init__.py
+-rw-rw-rw-   0        0        0   111614 2020-05-30 05:51:52.000000 CTkColorPicker-0.5.0/CTkColorPicker/color_wheel.png
+-rw-rw-rw-   0        0        0     9078 2023-04-14 11:17:37.000000 CTkColorPicker-0.5.0/CTkColorPicker/ctk_color_picker.py
+-rw-rw-rw-   0        0        0      933 2020-05-30 05:51:52.000000 CTkColorPicker-0.5.0/CTkColorPicker/target.png
+drwxrwxrwx   0        0        0        0 2023-04-14 11:22:56.306281 CTkColorPicker-0.5.0/CTkColorPicker.egg-info/
+-rw-rw-rw-   0        0        0     2601 2023-04-14 11:22:56.000000 CTkColorPicker-0.5.0/CTkColorPicker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      344 2023-04-14 11:22:56.000000 CTkColorPicker-0.5.0/CTkColorPicker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       73 2023-04-14 11:22:56.000000 CTkColorPicker-0.5.0/CTkColorPicker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-04-14 11:22:56.000000 CTkColorPicker-0.5.0/CTkColorPicker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-14 11:22:56.000000 CTkColorPicker-0.5.0/CTkColorPicker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7048 2022-11-20 16:16:56.000000 CTkColorPicker-0.5.0/LICENSE
+-rw-rw-rw-   0        0        0     2601 2023-04-14 11:22:56.306281 CTkColorPicker-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1922 2023-04-14 11:20:38.000000 CTkColorPicker-0.5.0/README.md
+-rw-rw-rw-   0        0        0      607 2023-04-14 11:22:56.318617 CTkColorPicker-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1317 2023-04-14 11:19:22.000000 CTkColorPicker-0.5.0/setup.py
```

### Comparing `CTkColorPicker-0.4.0/CTkColorPicker/color_wheel.png` & `CTkColorPicker-0.5.0/CTkColorPicker/color_wheel.png`

 * *Files identical despite different names*

### Comparing `CTkColorPicker-0.4.0/CTkColorPicker/ctk_color_picker.py` & `CTkColorPicker-0.5.0/CTkColorPicker/ctk_color_picker.py`

 * *Files 27% similar despite different names*

```diff
@@ -16,73 +16,95 @@
     except:
         pass
 
 PATH = os.path.dirname(os.path.realpath(__file__))
 
 class AskColor(customtkinter.CTkToplevel):
     
-    def __init__(self, color=(255, 255, 255), width: int=300):
-        
+    def __init__(self,
+                 width: int = 300,
+                 title: str = "Choose Color",
+                 initial_color: str = None,
+                 bg_color: str = None,
+                 fg_color: str = None,
+                 button_color: str = None,
+                 button_hover_color: str = None,
+                 text: str = "OK",
+                 corner_radius: int = 24,
+                 slider_border: int = 1,
+                 **button_kwargs):
+    
         super().__init__()
         
-        self.title("Choose Color")
+        self.title(title)
         WIDTH = width if width>=200 else 200
         HEIGHT = WIDTH + 150
         self.image_dimension = WIDTH - 100
             
         self.maxsize(WIDTH, HEIGHT)
         self.minsize(WIDTH, HEIGHT)
         self.resizable(width=False, height=False)
         self.transient(self.master)
         self.lift()
         self.grid_columnconfigure(0, weight=1)
         self.grid_rowconfigure(0, weight=1)
         self.after(10)
         self.protocol("WM_DELETE_WINDOW", self._on_closing)
-
-        self.default_color = [color[0], color[1], color[2]]
-        self.rgb_color = self.default_color[:]
         
-        self.frame = customtkinter.CTkFrame(master=self)
+        self.default_hex_color = "#ffffff"  
+        self.default_rgb = [255, 255, 255]
+        self.rgb_color = self.default_rgb[:]
+        
+        self.bg_color = self._apply_appearance_mode(customtkinter.ThemeManager.theme["CTkFrame"]["fg_color"]) if bg_color is None else bg_color
+        self.fg_color = self.fg_color = self._apply_appearance_mode(customtkinter.ThemeManager.theme["CTkFrame"]["top_fg_color"]) if fg_color is None else fg_color
+        self.button_color = self._apply_appearance_mode(customtkinter.ThemeManager.theme["CTkButton"]["fg_color"]) if button_color is None else button_color
+        self.button_hover_color = self._apply_appearance_mode(customtkinter.ThemeManager.theme["CTkButton"]["hover_color"]) if button_hover_color is None else button_hover_color
+        self.button_text = text
+        self.corner_radius = corner_radius
+        self.slider_width = 10 if slider_border>=10 else slider_border
+        
+        self.config(bg=self.bg_color)
+        
+        self.frame = customtkinter.CTkFrame(master=self, fg_color=self.fg_color, bg_color=self.bg_color)
         self.frame.grid(padx=20, pady=20, sticky="nswe")
           
-        self.canvas = tkinter.Canvas(self.frame, height=self.image_dimension, width=self.image_dimension, highlightthickness=0,
-                                bg=self.frame._apply_appearance_mode(self.frame._fg_color))
+        self.canvas = tkinter.Canvas(self.frame, height=self.image_dimension, width=self.image_dimension, highlightthickness=0, bg=self.fg_color)
         self.canvas.pack(pady=20)
         self.canvas.bind("<B1-Motion>", self.on_mouse_drag)
 
         self.img1 = Image.open(os.path.join(PATH, 'color_wheel.png')).resize((self.image_dimension, self.image_dimension), Image.Resampling.LANCZOS)
         self.img2 = Image.open(os.path.join(PATH, 'target.png')).resize((20, 20), Image.Resampling.LANCZOS)
 
         self.wheel = ImageTk.PhotoImage(self.img1)
         self.target = ImageTk.PhotoImage(self.img2)
-
+        
         self.canvas.create_image(self.image_dimension/2, self.image_dimension/2, image=self.wheel)
-        self.canvas.create_image(self.image_dimension/2, self.image_dimension/2, image=self.target)
+        self.set_initial_color(initial_color)
         
         self.brightness_slider_value = customtkinter.IntVar()
         self.brightness_slider_value.set(255)
         
-        self.slider = customtkinter.CTkSlider(master=self.frame, height=20, border_width=1,
-                                              button_length=15, progress_color="white", from_=0, to=255,
-                                              variable=self.brightness_slider_value, number_of_steps=256, 
+        self.slider = customtkinter.CTkSlider(master=self.frame, height=20, border_width=self.slider_width,
+                                              button_length=15, progress_color=self.default_hex_color, from_=0, to=255,
+                                              variable=self.brightness_slider_value, number_of_steps=256,
+                                              button_corner_radius=self.corner_radius, corner_radius=self.corner_radius,
+                                              button_color=self.button_color, button_hover_color=self.button_hover_color,
                                               command=lambda x:self.update_colors())
-        self.slider.pack(fill="both", pady=(0,15), padx=20)
-        
-        self.label = customtkinter.CTkLabel(master=self.frame, text_color="#000000", height=50, fg_color="#ffffff",
-                                            corner_radius=24, text="#ffffff")
+        self.slider.pack(fill="both", pady=(0,15), padx=20-self.slider_width)
+
+        self.label = customtkinter.CTkLabel(master=self.frame, text_color="#000000", height=50, fg_color=self.default_hex_color,
+                                            corner_radius=self.corner_radius, text=self.default_hex_color)
         self.label.pack(fill="both", padx=10)
         
-
-        self.button = customtkinter.CTkButton(master=self.frame, text="OK", height=50, corner_radius=24,
-                                              command=self._ok_event)
+        self.button = customtkinter.CTkButton(master=self.frame, text=self.button_text, height=50, corner_radius=self.corner_radius, fg_color=self.button_color,
+                                              hover_color=self.button_hover_color, command=self._ok_event, **button_kwargs)
         self.button.pack(fill="both", padx=10, pady=20)
-        
+                
         self.after(150, lambda: self.label.focus())
-        
+                
         self.grab_set()
         
     def get(self):
         self._color = self.label._fg_color
         self.master.wait_window(self)
         return self._color
     
@@ -109,44 +131,44 @@
         else:
             self.target_x, self.target_y = self.projection_on_circle(x, y, self.image_dimension/2, self.image_dimension/2, self.image_dimension/2 -1)
 
         self.canvas.create_image(self.target_x, self.target_y, image=self.target)
         
         self.get_target_color()
         self.update_colors()
-
-    
+  
     def get_target_color(self):
         try:
             self.rgb_color = self.img1.getpixel((self.target_x, self.target_y))
             
             r = self.rgb_color[0]
             g = self.rgb_color[1]
             b = self.rgb_color[2]    
             self.rgb_color = [r, g, b]
+            
         except AttributeError:
-            self.rgb_color = self.default_color
+            self.rgb_color = self.default_rgb
     
     def update_colors(self):
         brightness = self.brightness_slider_value.get()
 
         self.get_target_color()
 
         r = int(self.rgb_color[0] * (brightness/255))
         g = int(self.rgb_color[1] * (brightness/255))
         b = int(self.rgb_color[2] * (brightness/255))
         
         self.rgb_color = [r, g, b]
 
-        self.hex_color = "#{:02x}{:02x}{:02x}".format(*self.rgb_color)
+        self.default_hex_color = "#{:02x}{:02x}{:02x}".format(*self.rgb_color)
         
-        self.slider.configure(progress_color=self.hex_color)
-        self.label.configure(fg_color=self.hex_color)
+        self.slider.configure(progress_color=self.default_hex_color)
+        self.label.configure(fg_color=self.default_hex_color)
         
-        self.label.configure(text=str(self.hex_color))
+        self.label.configure(text=str(self.default_hex_color))
         
         if self.brightness_slider_value.get() < 70:
             self.label.configure(text_color="white")
         else:
             self.label.configure(text_color="black")
             
         if str(self.label._fg_color)=="black":
@@ -154,11 +176,32 @@
             
     def projection_on_circle(self, point_x, point_y, circle_x, circle_y, radius):
         angle = math.atan2(point_y - circle_y, point_x - circle_x)
         projection_x = circle_x + radius * math.cos(angle)
         projection_y = circle_y + radius * math.sin(angle)
 
         return projection_x, projection_y
-
+    
+    def set_initial_color(self, initial_color):
+        # set_initial_color is in beta stage, cannot seek all colors accurately
+        
+        if initial_color and initial_color.startswith("#"):
+            try:
+                r,g,b = tuple(int(initial_color.lstrip('#')[i:i+2], 16) for i in (0, 2, 4))
+            except ValueError:
+                return
+            
+            self.default_hex_color = initial_color
+            for i in range(0, self.image_dimension):
+                for j in range(0, self.image_dimension):
+                    self.rgb_color = self.img1.getpixel((i, j))
+                    if (self.rgb_color[0], self.rgb_color[1], self.rgb_color[2])==(r,g,b):
+                        self.canvas.create_image(i, j, image=self.target)
+                        self.target_x = i
+                        self.target_y = j
+                        return
+                    
+        self.canvas.create_image(self.image_dimension/2, self.image_dimension/2, image=self.target)
+        
 if __name__ == "__main__":
-    app = AskColor()               
+    app = AskColor()
     app.mainloop()
```

### Comparing `CTkColorPicker-0.4.0/CTkColorPicker/target.png` & `CTkColorPicker-0.5.0/CTkColorPicker/target.png`

 * *Files identical despite different names*

### Comparing `CTkColorPicker-0.4.0/CTkColorPicker.egg-info/PKG-INFO` & `CTkColorPicker-0.5.0/CTkColorPicker.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTkColorPicker
-Version: 0.4.0
+Version: 0.5.0
 Summary: A modern color picker for customtkinter
 Home-page: https://github.com/Akascape/CTkColorPicker
 Author: Akash Bora
 License: Creative Commons Zero v1.0 Universal
 Keywords: customtkinter,customtkinter-dialog,customtkinter-color-picker,customtkinter-colour-picker,customtkinter-color,customtkinter-color-chooser,color-picker,python-color-picker
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3
@@ -24,26 +24,43 @@
 pip install CTkColorPicker
 ```
 
 ### [<img alt="GitHub repo size" src="https://img.shields.io/github/repo-size/Akascape/CTkColorPicker?&color=white&label=Source%20Code&logo=Python&logoColor=yellow&style=for-the-badge"  width="300">](https://github.com/Akascape/CTkColorPicker/archive/refs/heads/main.zip)
 
 ## Requirements
 - [customtkinter](https://github.com/TomSchimansky/CustomTkinter)
+- [pillow](https://pypi.org/project/Pillow/)
 
 ### How to use?
 ```python
 import customtkinter as ctk
 from CTkColorPicker import AskColor
 
 def ask_color():
-    pick_color = AskColor(width=300) # Open the Color Picker, size of the window can be changed by adjusting width parameter
-    color = pick_color.get() # Get the color
+    pick_color = AskColor() # open the color picker
+    color = pick_color.get() # get the color string
     button.configure(fg_color=color)
     
 root = ctk.CTk()
 
 button = ctk.CTkButton(master=root, text="CHOOSE COLOR", text_color="black", command=ask_color)
 button.pack(padx=30, pady=20)
 root.mainloop()
 ```
 
-**Thats all, hope it will help!**
+# Options
+| Arguments | Description |
+|---------|-------------|
+| width | set the overall size of the color picker window |
+| title | change the title of color picker window |
+| fg_color | change forground color of the color picker frame |
+| bg_color | change background color of the color picker frame |
+| button_color | change the color of the button and slider |
+| button_hover_color | change the hover color of the buttons |
+| text | change the default text of the 'OK' button |
+| initial_color | set the default color of color picker (currently in beta stage) |
+| slider_border | change the border width of slider |
+| corner_radius | change the corner radius of all the widgets inside color picker |
+| _**other button parameters_ | pass other button arguments if required |
+
+
+**That's all, hope it will help!**
```

### Comparing `CTkColorPicker-0.4.0/LICENSE` & `CTkColorPicker-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `CTkColorPicker-0.4.0/PKG-INFO` & `CTkColorPicker-0.5.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTkColorPicker
-Version: 0.4.0
+Version: 0.5.0
 Summary: A modern color picker for customtkinter
 Home-page: https://github.com/Akascape/CTkColorPicker
 Author: Akash Bora
 License: Creative Commons Zero v1.0 Universal
 Keywords: customtkinter,customtkinter-dialog,customtkinter-color-picker,customtkinter-colour-picker,customtkinter-color,customtkinter-color-chooser,color-picker,python-color-picker
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3
@@ -24,26 +24,43 @@
 pip install CTkColorPicker
 ```
 
 ### [<img alt="GitHub repo size" src="https://img.shields.io/github/repo-size/Akascape/CTkColorPicker?&color=white&label=Source%20Code&logo=Python&logoColor=yellow&style=for-the-badge"  width="300">](https://github.com/Akascape/CTkColorPicker/archive/refs/heads/main.zip)
 
 ## Requirements
 - [customtkinter](https://github.com/TomSchimansky/CustomTkinter)
+- [pillow](https://pypi.org/project/Pillow/)
 
 ### How to use?
 ```python
 import customtkinter as ctk
 from CTkColorPicker import AskColor
 
 def ask_color():
-    pick_color = AskColor(width=300) # Open the Color Picker, size of the window can be changed by adjusting width parameter
-    color = pick_color.get() # Get the color
+    pick_color = AskColor() # open the color picker
+    color = pick_color.get() # get the color string
     button.configure(fg_color=color)
     
 root = ctk.CTk()
 
 button = ctk.CTkButton(master=root, text="CHOOSE COLOR", text_color="black", command=ask_color)
 button.pack(padx=30, pady=20)
 root.mainloop()
 ```
 
-**Thats all, hope it will help!**
+# Options
+| Arguments | Description |
+|---------|-------------|
+| width | set the overall size of the color picker window |
+| title | change the title of color picker window |
+| fg_color | change forground color of the color picker frame |
+| bg_color | change background color of the color picker frame |
+| button_color | change the color of the button and slider |
+| button_hover_color | change the hover color of the buttons |
+| text | change the default text of the 'OK' button |
+| initial_color | set the default color of color picker (currently in beta stage) |
+| slider_border | change the border width of slider |
+| corner_radius | change the corner radius of all the widgets inside color picker |
+| _**other button parameters_ | pass other button arguments if required |
+
+
+**That's all, hope it will help!**
```

### Comparing `CTkColorPicker-0.4.0/README.md` & `CTkColorPicker-0.5.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -9,26 +9,43 @@
 pip install CTkColorPicker
 ```
 
 ### [<img alt="GitHub repo size" src="https://img.shields.io/github/repo-size/Akascape/CTkColorPicker?&color=white&label=Source%20Code&logo=Python&logoColor=yellow&style=for-the-badge"  width="300">](https://github.com/Akascape/CTkColorPicker/archive/refs/heads/main.zip)
 
 ## Requirements
 - [customtkinter](https://github.com/TomSchimansky/CustomTkinter)
+- [pillow](https://pypi.org/project/Pillow/)
 
 ### How to use?
 ```python
 import customtkinter as ctk
 from CTkColorPicker import AskColor
 
 def ask_color():
-    pick_color = AskColor(width=300) # Open the Color Picker, size of the window can be changed by adjusting width parameter
-    color = pick_color.get() # Get the color
+    pick_color = AskColor() # open the color picker
+    color = pick_color.get() # get the color string
     button.configure(fg_color=color)
     
 root = ctk.CTk()
 
 button = ctk.CTkButton(master=root, text="CHOOSE COLOR", text_color="black", command=ask_color)
 button.pack(padx=30, pady=20)
 root.mainloop()
 ```
 
-**Thats all, hope it will help!**
+# Options
+| Arguments | Description |
+|---------|-------------|
+| width | set the overall size of the color picker window |
+| title | change the title of color picker window |
+| fg_color | change forground color of the color picker frame |
+| bg_color | change background color of the color picker frame |
+| button_color | change the color of the button and slider |
+| button_hover_color | change the hover color of the buttons |
+| text | change the default text of the 'OK' button |
+| initial_color | set the default color of color picker (currently in beta stage) |
+| slider_border | change the border width of slider |
+| corner_radius | change the corner radius of all the widgets inside color picker |
+| _**other button parameters_ | pass other button arguments if required |
+
+
+**That's all, hope it will help!**
```

### Comparing `CTkColorPicker-0.4.0/setup.cfg` & `CTkColorPicker-0.5.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2043 546b 436f 6c6f 7250 6963 6b65   = CTkColorPicke
-00000020: 720d 0a76 6572 7369 6f6e 203d 2030 2e34  r..version = 0.4
+00000020: 720d 0a76 6572 7369 6f6e 203d 2030 2e35  r..version = 0.5
 00000030: 2e30 0d0a 6465 7363 7269 7074 696f 6e20  .0..description 
 00000040: 3d20 4120 6d6f 6465 726e 2063 6f6c 6f72  = A modern color
 00000050: 2070 6963 6b65 7220 666f 7220 6375 7374   picker for cust
 00000060: 6f6d 746b 696e 7465 720d 0a6c 6f6e 675f  omtkinter..long_
 00000070: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
 00000080: 6c65 3a20 5245 4144 4d45 2e6d 640d 0a6c  le: README.md..l
 00000090: 6f6e 675f 6465 7363 7269 7074 696f 6e5f  ong_description_
```

### Comparing `CTkColorPicker-0.4.0/setup.py` & `CTkColorPicker-0.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     """Opens and fetches text of long descrition file."""
     with open(path, 'r') as f:
         text = f.read()
     return text
 
 setup(
     name = 'CTkColorPicker',
-    version = '0.4.0',
+    version = '0.5.0',
     description = "A modern color picker for customtkinter",
     license = "Creative Commons Zero v1.0 Universal",
     readme = "README.md",
     long_description = get_long_description('README.md'),
     long_description_content_type = "text/markdown",
     author = 'Akash Bora',
     url = "https://github.com/Akascape/CTkColorPicker",
```

