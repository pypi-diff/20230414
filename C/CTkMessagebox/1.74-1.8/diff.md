# Comparing `tmp/CTkMessagebox-1.74.tar.gz` & `tmp/CTkMessagebox-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CTkMessagebox-1.74.tar", last modified: Mon Apr  3 16:18:39 2023, max compression
+gzip compressed data, was "CTkMessagebox-1.8.tar", last modified: Fri Apr 14 12:45:38 2023, max compression
```

## Comparing `CTkMessagebox-1.74.tar` & `CTkMessagebox-1.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-03 16:18:39.768668 CTkMessagebox-1.74/
-drwxrwxrwx   0        0        0        0 2023-04-03 16:18:39.737409 CTkMessagebox-1.74/CTkMessagebox/
--rw-rw-rw-   0        0        0      233 2023-04-03 16:16:44.000000 CTkMessagebox-1.74/CTkMessagebox/__init__.py
--rw-rw-rw-   0        0        0    12002 2023-04-03 16:16:33.000000 CTkMessagebox-1.74/CTkMessagebox/ctkmessagebox.py
-drwxrwxrwx   0        0        0        0 2023-04-03 16:18:39.753039 CTkMessagebox-1.74/CTkMessagebox/icons/
--rw-rw-rw-   0        0        0    38437 2023-02-24 17:58:14.000000 CTkMessagebox-1.74/CTkMessagebox/icons/cancel.png
--rw-rw-rw-   0        0        0    31308 2023-02-24 17:40:20.000000 CTkMessagebox-1.74/CTkMessagebox/icons/check.png
--rw-rw-rw-   0        0        0    14921 2023-02-24 18:08:36.000000 CTkMessagebox-1.74/CTkMessagebox/icons/info.png
--rw-rw-rw-   0        0        0    14873 2023-02-24 18:10:32.000000 CTkMessagebox-1.74/CTkMessagebox/icons/question.png
--rw-rw-rw-   0        0        0    17104 2023-02-24 18:03:33.000000 CTkMessagebox-1.74/CTkMessagebox/icons/warning.png
-drwxrwxrwx   0        0        0        0 2023-04-03 16:18:39.753039 CTkMessagebox-1.74/CTkMessagebox.egg-info/
--rw-rw-rw-   0        0        0     5907 2023-04-03 16:18:39.000000 CTkMessagebox-1.74/CTkMessagebox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      432 2023-04-03 16:18:39.000000 CTkMessagebox-1.74/CTkMessagebox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       73 2023-04-03 16:18:39.000000 CTkMessagebox-1.74/CTkMessagebox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-04-03 16:18:39.000000 CTkMessagebox-1.74/CTkMessagebox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-03 16:18:39.000000 CTkMessagebox-1.74/CTkMessagebox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7048 2022-11-20 16:16:56.000000 CTkMessagebox-1.74/LICENSE
--rw-rw-rw-   0        0        0     5907 2023-04-03 16:18:39.768668 CTkMessagebox-1.74/PKG-INFO
--rw-rw-rw-   0        0        0     5208 2023-04-03 12:47:38.000000 CTkMessagebox-1.74/README.md
--rw-rw-rw-   0        0        0      626 2023-04-03 16:18:39.768668 CTkMessagebox-1.74/setup.cfg
--rw-rw-rw-   0        0        0     1362 2023-04-03 16:17:30.000000 CTkMessagebox-1.74/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 12:45:38.954699 CTkMessagebox-1.8/
+drwxrwxrwx   0        0        0        0 2023-04-14 12:45:38.939076 CTkMessagebox-1.8/CTkMessagebox/
+-rw-rw-rw-   0        0        0      232 2023-04-14 12:41:18.000000 CTkMessagebox-1.8/CTkMessagebox/__init__.py
+-rw-rw-rw-   0        0        0    12817 2023-04-14 12:34:46.000000 CTkMessagebox-1.8/CTkMessagebox/ctkmessagebox.py
+drwxrwxrwx   0        0        0        0 2023-04-14 12:45:38.954699 CTkMessagebox-1.8/CTkMessagebox/icons/
+-rw-rw-rw-   0        0        0    38437 2023-02-24 17:58:14.000000 CTkMessagebox-1.8/CTkMessagebox/icons/cancel.png
+-rw-rw-rw-   0        0        0    31308 2023-02-24 17:40:20.000000 CTkMessagebox-1.8/CTkMessagebox/icons/check.png
+-rw-rw-rw-   0        0        0    14921 2023-02-24 18:08:36.000000 CTkMessagebox-1.8/CTkMessagebox/icons/info.png
+-rw-rw-rw-   0        0        0    15030 2023-04-14 12:27:30.000000 CTkMessagebox-1.8/CTkMessagebox/icons/question.png
+-rw-rw-rw-   0        0        0    17104 2023-02-24 18:03:33.000000 CTkMessagebox-1.8/CTkMessagebox/icons/warning.png
+drwxrwxrwx   0        0        0        0 2023-04-14 12:45:38.954699 CTkMessagebox-1.8/CTkMessagebox.egg-info/
+-rw-rw-rw-   0        0        0     5959 2023-04-14 12:45:38.000000 CTkMessagebox-1.8/CTkMessagebox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      432 2023-04-14 12:45:38.000000 CTkMessagebox-1.8/CTkMessagebox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       73 2023-04-14 12:45:38.000000 CTkMessagebox-1.8/CTkMessagebox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-04-14 12:45:38.000000 CTkMessagebox-1.8/CTkMessagebox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-14 12:45:38.000000 CTkMessagebox-1.8/CTkMessagebox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7048 2022-11-20 16:16:56.000000 CTkMessagebox-1.8/LICENSE
+-rw-rw-rw-   0        0        0     5959 2023-04-14 12:45:38.970323 CTkMessagebox-1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     5261 2023-04-14 12:41:41.000000 CTkMessagebox-1.8/README.md
+-rw-rw-rw-   0        0        0      625 2023-04-14 12:45:38.970323 CTkMessagebox-1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1361 2023-04-14 12:41:29.000000 CTkMessagebox-1.8/setup.py
```

### Comparing `CTkMessagebox-1.74/CTkMessagebox/ctkmessagebox.py` & `CTkMessagebox-1.8/CTkMessagebox/ctkmessagebox.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 CustomTkinter Messagebox
 Author: Akash Bora
-Version: 1.74
+Version: 1.8
 """
 
 import customtkinter
 from PIL import Image
 import os
 import sys
 import time
@@ -28,14 +28,15 @@
                  fg_color: str = "default",
                  text_color: str = "default",
                  title_color: str = "default",
                  button_text_color: str = "default",
                  button_width: int = None,
                  button_height: int = None,
                  cancel_button_color: str = "#c42b1c",
+                 button_hover_color: str = "default",
                  icon: str = "info",
                  icon_size: tuple = None,
                  corner_radius: int = 15,
                  font: tuple = None,
                  header: bool = False,
                  topmost: bool = True,
                  fade_in_duration: int = 0):
@@ -68,15 +69,15 @@
     
         if topmost:
             self.attributes("-topmost", True)
         else:
             self.transient(self.master_window)
     
         if sys.platform.startswith("win"):
-            self.transparent_color = '#000001'
+            self.transparent_color = self._apply_appearance_mode(self._fg_color)
             self.attributes("-transparentcolor", self.transparent_color)
         elif sys.platform.startswith("darwin"):
             self.transparent_color = 'systemTransparent'
             self.attributes("-transparent", True)
         else:
             self.transparent_color = '#000001'
             corner_radius = 0
@@ -135,14 +136,19 @@
         else:
             self.title_color = title_color
             
         if button_text_color=="default":
             self.bt_text_color = self._apply_appearance_mode(customtkinter.ThemeManager.theme["CTkButton"]["text_color"])
         else:
             self.bt_text_color = button_text_color
+
+        if button_hover_color=="default":
+            self.bt_hv_color = self._apply_appearance_mode(customtkinter.ThemeManager.theme["CTkButton"]["hover_color"])
+        else:
+            self.bt_hv_color = button_hover_color
             
         if border_color=="default":
             self.border_color = self._apply_appearance_mode(customtkinter.ThemeManager.theme["CTkFrame"]["border_color"])
         else:
             self.border_color = border_color
             
         if icon_size:
@@ -180,38 +186,45 @@
         self.button_close.grid(row=0, column=3, sticky="ne", padx=10, pady=10)
 
         self.title_label = customtkinter.CTkLabel(self.frame_top, width=1, text=self._title, text_color=self.title_color, font=self.font)
         self.title_label.grid(row=0, column=0, columnspan=4, sticky="nw", padx=(15,30), pady=5)
         self.title_label.bind("<B1-Motion>", self.move_window)
         self.title_label.bind("<ButtonPress-1>", self.oldxyset)
         
-        self.info = customtkinter.CTkButton(self.frame_top,  width=1, height=100, corner_radius=0, text=self.message, font=self.font,
+        self.info = customtkinter.CTkButton(self.frame_top,  width=1, height=self.height/2, corner_radius=0, text=self.message, font=self.font,
                                             fg_color=self.fg_color, hover=False, text_color=self.text_color, image=self.icon)
         self.info._text_label.configure(wraplength=self.width/2, justify="left")
         self.info.grid(row=1, column=0, columnspan=4, sticky="nwes", padx=self.border_width)
         
+        if self.info._text_label.winfo_reqheight()>self.height/2:
+            height_offset = int((self.info._text_label.winfo_reqheight())-(self.height/2) + self.height)
+            self.geometry(f"{self.width}x{height_offset}")
+            
         self.option_text_1 = option_1
         self.button_1 = customtkinter.CTkButton(self.frame_top, text=self.option_text_1, fg_color=self.button_color[0],
                                                 width=self.button_width, font=self.font, text_color=self.bt_text_color,
-                                                height=self.button_height, command=lambda: self.button_event(self.option_text_1))
+                                                hover_color=self.bt_hv_color, height=self.button_height,
+                                                command=lambda: self.button_event(self.option_text_1))
         
         self.button_1.grid(row=2, column=3, sticky="news", padx=(0,10), pady=10)
 
         if option_2:
             self.option_text_2 = option_2      
             self.button_2 = customtkinter.CTkButton(self.frame_top, text=self.option_text_2, fg_color=self.button_color[1],
                                                     width=self.button_width, font=self.font, text_color=self.bt_text_color,
-                                                    height=self.button_height, command=lambda: self.button_event(self.option_text_2))
+                                                    hover_color=self.bt_hv_color, height=self.button_height,
+                                                    command=lambda: self.button_event(self.option_text_2))
             self.button_2.grid(row=2, column=2, sticky="news", padx=10, pady=10)
             
         if option_3:
             self.option_text_3 = option_3
             self.button_3 = customtkinter.CTkButton(self.frame_top, text=self.option_text_3, fg_color=self.button_color[2],
                                                     width=self.button_width, font=self.font, text_color=self.bt_text_color,
-                                                    height=self.button_height, command=lambda: self.button_event(self.option_text_3))
+                                                    hover_color=self.bt_hv_color, height=self.button_height,
+                                                    command=lambda: self.button_event(self.option_text_3))
             self.button_3.grid(row=2, column=1, sticky="news", padx=(10,0), pady=10)
 
         if header:
             self.title_label.grid_forget()
             self.button_close.grid_forget()
             self.frame_top.configure(corner_radius=0)
 
@@ -260,11 +273,11 @@
             pass
 
         if self.fade:
             self.fade_out()
         self.grab_release()
         self.destroy()
         self.event = event
-        
+
 if __name__ == "__main__":
     app = CTkMessagebox()
     app.mainloop()
```

### Comparing `CTkMessagebox-1.74/CTkMessagebox/icons/cancel.png` & `CTkMessagebox-1.8/CTkMessagebox/icons/cancel.png`

 * *Files identical despite different names*

### Comparing `CTkMessagebox-1.74/CTkMessagebox/icons/check.png` & `CTkMessagebox-1.8/CTkMessagebox/icons/check.png`

 * *Files identical despite different names*

### Comparing `CTkMessagebox-1.74/CTkMessagebox/icons/info.png` & `CTkMessagebox-1.8/CTkMessagebox/icons/info.png`

 * *Files identical despite different names*

### Comparing `CTkMessagebox-1.74/CTkMessagebox/icons/warning.png` & `CTkMessagebox-1.8/CTkMessagebox/icons/warning.png`

 * *Files identical despite different names*

### Comparing `CTkMessagebox-1.74/CTkMessagebox.egg-info/PKG-INFO` & `CTkMessagebox-1.8/CTkMessagebox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTkMessagebox
-Version: 1.74
+Version: 1.8
 Summary: A modern messagebox for customtkinter
 Home-page: https://github.com/Akascape/CTkMessagebox
 Author: Akash Bora
 License: Creative Commons Zero v1.0 Universal
 Keywords: customtkinter,customtkinter-dialog,customtkinter-messagebox,customtkinter-message-box,tkinter-messagebox,customtkinter-tkinter-messagebox,messagebox-widget,modern-tkinter-messagebox,ctkmessagebox
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3
@@ -104,31 +104,32 @@
   | **_option_1_** | the text on the first button [Default is 'OK'] |
   | **_option_2_** | the text on the second button |
   | **_option_3_** | the text on the last button |
   | _button_color_ | color of the buttons |
   | _text_color_ | color of the message-text |
   | _title_color_ | color of the title-text |
   | _button_text_color_ | color of the button-text |
+  | _button_hover_color_ | hover color of the buttons |
   | _button_width_ | width of the buttons in px |
   | _button_height_ | height of the buttons in px |
   | _border_width_ | width of the border around the main frame [Default is 1] |
   | _border_color_ | color of the frame border |
   | _cancel_button_color_ | color of the **close** button, **set it to 'transparent' if you want to hide it** |
   | **_icon_** | icon that will be shown in the messagebox [Default is the 'info' icon] |
   | _icon_size_ | define the size of the icon image manually (tuple) |
   | _corner_radius_ | corner roundness of the messagebox window [**not applicable in linux**] |
   | _font_ | font of the messagebox text (tuple) |
   | _header_ | add the original header back if you don't like **overrideredirect** (bool) |
   | _topmost_ | disable the topmost window outside the app (bool) |
   | **_fade_in_duration_** | enable a fade-in and fade-out animation (int, default is 0)  |
-
+  
 ### Icons
 
 **Default icons:**
 
 ![icons](https://user-images.githubusercontent.com/89206401/221258403-aafea575-856e-4f4e-b3af-f995785c9879.png)
 
-(*These icons are created by me using Paint.NET, free to use!*)
+(*These icons are created using Paint.NET, free to use!*)
 
 **For custom images, just use `icon="path_to_the_image.png"`**
 
 ## That's all, hope it will help in UI development!
```

### Comparing `CTkMessagebox-1.74/LICENSE` & `CTkMessagebox-1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `CTkMessagebox-1.74/PKG-INFO` & `CTkMessagebox-1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTkMessagebox
-Version: 1.74
+Version: 1.8
 Summary: A modern messagebox for customtkinter
 Home-page: https://github.com/Akascape/CTkMessagebox
 Author: Akash Bora
 License: Creative Commons Zero v1.0 Universal
 Keywords: customtkinter,customtkinter-dialog,customtkinter-messagebox,customtkinter-message-box,tkinter-messagebox,customtkinter-tkinter-messagebox,messagebox-widget,modern-tkinter-messagebox,ctkmessagebox
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3
@@ -104,31 +104,32 @@
   | **_option_1_** | the text on the first button [Default is 'OK'] |
   | **_option_2_** | the text on the second button |
   | **_option_3_** | the text on the last button |
   | _button_color_ | color of the buttons |
   | _text_color_ | color of the message-text |
   | _title_color_ | color of the title-text |
   | _button_text_color_ | color of the button-text |
+  | _button_hover_color_ | hover color of the buttons |
   | _button_width_ | width of the buttons in px |
   | _button_height_ | height of the buttons in px |
   | _border_width_ | width of the border around the main frame [Default is 1] |
   | _border_color_ | color of the frame border |
   | _cancel_button_color_ | color of the **close** button, **set it to 'transparent' if you want to hide it** |
   | **_icon_** | icon that will be shown in the messagebox [Default is the 'info' icon] |
   | _icon_size_ | define the size of the icon image manually (tuple) |
   | _corner_radius_ | corner roundness of the messagebox window [**not applicable in linux**] |
   | _font_ | font of the messagebox text (tuple) |
   | _header_ | add the original header back if you don't like **overrideredirect** (bool) |
   | _topmost_ | disable the topmost window outside the app (bool) |
   | **_fade_in_duration_** | enable a fade-in and fade-out animation (int, default is 0)  |
-
+  
 ### Icons
 
 **Default icons:**
 
 ![icons](https://user-images.githubusercontent.com/89206401/221258403-aafea575-856e-4f4e-b3af-f995785c9879.png)
 
-(*These icons are created by me using Paint.NET, free to use!*)
+(*These icons are created using Paint.NET, free to use!*)
 
 **For custom images, just use `icon="path_to_the_image.png"`**
 
 ## That's all, hope it will help in UI development!
```

### Comparing `CTkMessagebox-1.74/README.md` & `CTkMessagebox-1.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -89,31 +89,32 @@
   | **_option_1_** | the text on the first button [Default is 'OK'] |
   | **_option_2_** | the text on the second button |
   | **_option_3_** | the text on the last button |
   | _button_color_ | color of the buttons |
   | _text_color_ | color of the message-text |
   | _title_color_ | color of the title-text |
   | _button_text_color_ | color of the button-text |
+  | _button_hover_color_ | hover color of the buttons |
   | _button_width_ | width of the buttons in px |
   | _button_height_ | height of the buttons in px |
   | _border_width_ | width of the border around the main frame [Default is 1] |
   | _border_color_ | color of the frame border |
   | _cancel_button_color_ | color of the **close** button, **set it to 'transparent' if you want to hide it** |
   | **_icon_** | icon that will be shown in the messagebox [Default is the 'info' icon] |
   | _icon_size_ | define the size of the icon image manually (tuple) |
   | _corner_radius_ | corner roundness of the messagebox window [**not applicable in linux**] |
   | _font_ | font of the messagebox text (tuple) |
   | _header_ | add the original header back if you don't like **overrideredirect** (bool) |
   | _topmost_ | disable the topmost window outside the app (bool) |
   | **_fade_in_duration_** | enable a fade-in and fade-out animation (int, default is 0)  |
-
+  
 ### Icons
 
 **Default icons:**
 
 ![icons](https://user-images.githubusercontent.com/89206401/221258403-aafea575-856e-4f4e-b3af-f995785c9879.png)
 
-(*These icons are created by me using Paint.NET, free to use!*)
+(*These icons are created using Paint.NET, free to use!*)
 
 **For custom images, just use `icon="path_to_the_image.png"`**
 
 ## That's all, hope it will help in UI development!
```

### Comparing `CTkMessagebox-1.74/setup.cfg` & `CTkMessagebox-1.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2043 546b 4d65 7373 6167 6562 6f78   = CTkMessagebox
-00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 3734  ..version = 1.74
-00000030: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
-00000040: 4120 6d6f 6465 726e 206d 6573 7361 6765  A modern message
-00000050: 626f 7820 666f 7220 6375 7374 6f6d 746b  box for customtk
-00000060: 696e 7465 720d 0a6c 6f6e 675f 6465 7363  inter..long_desc
-00000070: 7269 7074 696f 6e20 3d20 6669 6c65 3a20  ription = file: 
-00000080: 5245 4144 4d45 2e6d 640d 0a6c 6f6e 675f  README.md..long_
-00000090: 6465 7363 7269 7074 696f 6e5f 636f 6e74  description_cont
-000000a0: 656e 745f 7479 7065 203d 2074 6578 742f  ent_type = text/
-000000b0: 6d61 726b 646f 776e 0d0a 7572 6c20 3d20  markdown..url = 
-000000c0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000000d0: 6f6d 2f41 6b61 7363 6170 652f 4354 6b4d  om/Akascape/CTkM
-000000e0: 6573 7361 6765 626f 780d 0a61 7574 686f  essagebox..autho
-000000f0: 7220 3d20 416b 6173 6820 426f 7261 0d0a  r = Akash Bora..
-00000100: 6c69 6365 6e73 6520 3d20 4372 6561 7469  license = Creati
-00000110: 7665 2043 6f6d 6d6f 6e73 205a 6572 6f20  ve Commons Zero 
-00000120: 7631 2e30 2055 6e69 7665 7273 616c 0d0a  v1.0 Universal..
-00000130: 6c69 6365 6e73 655f 6669 6c65 203d 204c  license_file = L
-00000140: 4943 454e 5345 0d0a 636c 6173 7369 6669  ICENSE..classifi
-00000150: 6572 7320 3d20 0d0a 094c 6963 656e 7365  ers = ...License
-00000160: 203a 3a20 4343 3020 312e 3020 556e 6976   :: CC0 1.0 Univ
-00000170: 6572 7361 6c20 2843 4330 2031 2e30 2920  ersal (CC0 1.0) 
-00000180: 5075 626c 6963 2044 6f6d 6169 6e20 4465  Public Domain De
-00000190: 6469 6361 7469 6f6e 0d0a 094f 7065 7261  dication...Opera
-000001a0: 7469 6e67 2053 7973 7465 6d20 3a3a 204f  ting System :: O
-000001b0: 5320 496e 6465 7065 6e64 656e 740d 0a09  S Independent...
-000001c0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-000001d0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-000001e0: 3a20 3320 3a3a 204f 6e6c 790d 0a0d 0a5b  : 3 :: Only....[
-000001f0: 6f70 7469 6f6e 735d 0d0a 7079 7468 6f6e  options]..python
-00000200: 5f72 6571 7569 7265 7320 3d20 3e3d 332e  _requires = >=3.
-00000210: 360d 0a70 6163 6b61 6765 7320 3d20 0d0a  6..packages = ..
-00000220: 0943 546b 4d65 7373 6167 6562 6f78 0d0a  .CTkMessagebox..
-00000230: 0943 546b 4d65 7373 6167 6562 6f78 2e69  .CTkMessagebox.i
-00000240: 636f 6e73 0d0a 0d0a 5b65 6767 5f69 6e66  cons....[egg_inf
-00000250: 6f5d 0d0a 7461 675f 6275 696c 6420 3d20  o]..tag_build = 
-00000260: 0d0a 7461 675f 6461 7465 203d 2030 0d0a  ..tag_date = 0..
-00000270: 0d0a                                     ..
+00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 380d  ..version = 1.8.
+00000030: 0a64 6573 6372 6970 7469 6f6e 203d 2041  .description = A
+00000040: 206d 6f64 6572 6e20 6d65 7373 6167 6562   modern messageb
+00000050: 6f78 2066 6f72 2063 7573 746f 6d74 6b69  ox for customtki
+00000060: 6e74 6572 0d0a 6c6f 6e67 5f64 6573 6372  nter..long_descr
+00000070: 6970 7469 6f6e 203d 2066 696c 653a 2052  iption = file: R
+00000080: 4541 444d 452e 6d64 0d0a 6c6f 6e67 5f64  EADME.md..long_d
+00000090: 6573 6372 6970 7469 6f6e 5f63 6f6e 7465  escription_conte
+000000a0: 6e74 5f74 7970 6520 3d20 7465 7874 2f6d  nt_type = text/m
+000000b0: 6172 6b64 6f77 6e0d 0a75 726c 203d 2068  arkdown..url = h
+000000c0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000000d0: 6d2f 416b 6173 6361 7065 2f43 546b 4d65  m/Akascape/CTkMe
+000000e0: 7373 6167 6562 6f78 0d0a 6175 7468 6f72  ssagebox..author
+000000f0: 203d 2041 6b61 7368 2042 6f72 610d 0a6c   = Akash Bora..l
+00000100: 6963 656e 7365 203d 2043 7265 6174 6976  icense = Creativ
+00000110: 6520 436f 6d6d 6f6e 7320 5a65 726f 2076  e Commons Zero v
+00000120: 312e 3020 556e 6976 6572 7361 6c0d 0a6c  1.0 Universal..l
+00000130: 6963 656e 7365 5f66 696c 6520 3d20 4c49  icense_file = LI
+00000140: 4345 4e53 450d 0a63 6c61 7373 6966 6965  CENSE..classifie
+00000150: 7273 203d 200d 0a09 4c69 6365 6e73 6520  rs = ...License 
+00000160: 3a3a 2043 4330 2031 2e30 2055 6e69 7665  :: CC0 1.0 Unive
+00000170: 7273 616c 2028 4343 3020 312e 3029 2050  rsal (CC0 1.0) P
+00000180: 7562 6c69 6320 446f 6d61 696e 2044 6564  ublic Domain Ded
+00000190: 6963 6174 696f 6e0d 0a09 4f70 6572 6174  ication...Operat
+000001a0: 696e 6720 5379 7374 656d 203a 3a20 4f53  ing System :: OS
+000001b0: 2049 6e64 6570 656e 6465 6e74 0d0a 0950   Independent...P
+000001c0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+000001d0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+000001e0: 2033 203a 3a20 4f6e 6c79 0d0a 0d0a 5b6f   3 :: Only....[o
+000001f0: 7074 696f 6e73 5d0d 0a70 7974 686f 6e5f  ptions]..python_
+00000200: 7265 7175 6972 6573 203d 203e 3d33 2e36  requires = >=3.6
+00000210: 0d0a 7061 636b 6167 6573 203d 200d 0a09  ..packages = ...
+00000220: 4354 6b4d 6573 7361 6765 626f 780d 0a09  CTkMessagebox...
+00000230: 4354 6b4d 6573 7361 6765 626f 782e 6963  CTkMessagebox.ic
+00000240: 6f6e 730d 0a0d 0a5b 6567 675f 696e 666f  ons....[egg_info
+00000250: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
+00000260: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
+00000270: 0a                                       .
```

### Comparing `CTkMessagebox-1.74/setup.py` & `CTkMessagebox-1.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     """Opens and fetches text of long descrition file."""
     with open(path, 'r') as f:
         text = f.read()
     return text
 
 setup(
     name = 'CTkMessagebox',
-    version = '1.74',
+    version = '1.8',
     description = "A modern messagebox for customtkinter",
     license = "Creative Commons Zero v1.0 Universal",
     readme = "README.md",
     long_description = get_long_description('README.md'),
     long_description_content_type = "text/markdown",
     author = 'Akash Bora',
     url = "https://github.com/Akascape/CTkMessagebox",
```

