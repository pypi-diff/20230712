# Comparing `tmp/CTkMessagebox-2.2.tar.gz` & `tmp/CTkMessagebox-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CTkMessagebox-2.2.tar", last modified: Mon Jul 10 06:17:45 2023, max compression
+gzip compressed data, was "CTkMessagebox-2.3.tar", last modified: Wed Jul 12 14:39:38 2023, max compression
```

## Comparing `CTkMessagebox-2.2.tar` & `CTkMessagebox-2.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 06:17:45.256214 CTkMessagebox-2.2/
-drwxrwxrwx   0        0        0        0 2023-07-10 06:17:45.226214 CTkMessagebox-2.2/CTkMessagebox/
--rw-rw-rw-   0        0        0      232 2023-07-10 06:13:56.000000 CTkMessagebox-2.2/CTkMessagebox/__init__.py
--rw-rw-rw-   0        0        0    14935 2023-07-10 06:12:40.000000 CTkMessagebox-2.2/CTkMessagebox/ctkmessagebox.py
-drwxrwxrwx   0        0        0        0 2023-07-10 06:17:45.256214 CTkMessagebox-2.2/CTkMessagebox/icons/
--rw-rw-rw-   0        0        0    38437 2023-02-24 17:58:14.000000 CTkMessagebox-2.2/CTkMessagebox/icons/cancel.png
--rw-rw-rw-   0        0        0    31308 2023-02-24 17:40:20.000000 CTkMessagebox-2.2/CTkMessagebox/icons/check.png
--rw-rw-rw-   0        0        0    14921 2023-02-24 18:08:36.000000 CTkMessagebox-2.2/CTkMessagebox/icons/info.png
--rw-rw-rw-   0        0        0    15030 2023-04-14 12:27:30.000000 CTkMessagebox-2.2/CTkMessagebox/icons/question.png
--rw-rw-rw-   0        0        0    17104 2023-02-24 18:03:33.000000 CTkMessagebox-2.2/CTkMessagebox/icons/warning.png
-drwxrwxrwx   0        0        0        0 2023-07-10 06:17:45.245962 CTkMessagebox-2.2/CTkMessagebox.egg-info/
--rw-rw-rw-   0        0        0     7104 2023-07-10 06:17:45.000000 CTkMessagebox-2.2/CTkMessagebox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      432 2023-07-10 06:17:45.000000 CTkMessagebox-2.2/CTkMessagebox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       73 2023-07-10 06:17:45.000000 CTkMessagebox-2.2/CTkMessagebox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-07-10 06:17:45.000000 CTkMessagebox-2.2/CTkMessagebox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-10 06:17:45.000000 CTkMessagebox-2.2/CTkMessagebox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7048 2022-11-20 16:16:56.000000 CTkMessagebox-2.2/LICENSE
--rw-rw-rw-   0        0        0     7104 2023-07-10 06:17:45.256214 CTkMessagebox-2.2/PKG-INFO
--rw-rw-rw-   0        0        0     6406 2023-07-08 07:24:42.000000 CTkMessagebox-2.2/README.md
--rw-rw-rw-   0        0        0      625 2023-07-10 06:17:45.256214 CTkMessagebox-2.2/setup.cfg
--rw-rw-rw-   0        0        0     1361 2023-07-10 06:14:15.000000 CTkMessagebox-2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 14:39:38.700017 CTkMessagebox-2.3/
+drwxrwxrwx   0        0        0        0 2023-07-12 14:39:38.653143 CTkMessagebox-2.3/CTkMessagebox/
+-rw-rw-rw-   0        0        0      232 2023-07-12 14:33:56.000000 CTkMessagebox-2.3/CTkMessagebox/__init__.py
+-rw-rw-rw-   0        0        0    17006 2023-07-12 14:33:23.000000 CTkMessagebox-2.3/CTkMessagebox/ctkmessagebox.py
+drwxrwxrwx   0        0        0        0 2023-07-12 14:39:38.700017 CTkMessagebox-2.3/CTkMessagebox/icons/
+-rw-rw-rw-   0        0        0    38437 2023-02-24 17:58:14.000000 CTkMessagebox-2.3/CTkMessagebox/icons/cancel.png
+-rw-rw-rw-   0        0        0    31308 2023-02-24 17:40:20.000000 CTkMessagebox-2.3/CTkMessagebox/icons/check.png
+-rw-rw-rw-   0        0        0    14921 2023-02-24 18:08:36.000000 CTkMessagebox-2.3/CTkMessagebox/icons/info.png
+-rw-rw-rw-   0        0        0    15030 2023-04-14 12:27:30.000000 CTkMessagebox-2.3/CTkMessagebox/icons/question.png
+-rw-rw-rw-   0        0        0    17104 2023-02-24 18:03:33.000000 CTkMessagebox-2.3/CTkMessagebox/icons/warning.png
+drwxrwxrwx   0        0        0        0 2023-07-12 14:39:38.668769 CTkMessagebox-2.3/CTkMessagebox.egg-info/
+-rw-rw-rw-   0        0        0     7184 2023-07-12 14:39:38.000000 CTkMessagebox-2.3/CTkMessagebox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      432 2023-07-12 14:39:38.000000 CTkMessagebox-2.3/CTkMessagebox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       73 2023-07-12 14:39:38.000000 CTkMessagebox-2.3/CTkMessagebox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-07-12 14:39:38.000000 CTkMessagebox-2.3/CTkMessagebox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-12 14:39:38.000000 CTkMessagebox-2.3/CTkMessagebox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7048 2022-11-20 16:16:56.000000 CTkMessagebox-2.3/LICENSE
+-rw-rw-rw-   0        0        0     7184 2023-07-12 14:39:38.700017 CTkMessagebox-2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6486 2023-07-12 14:35:39.000000 CTkMessagebox-2.3/README.md
+-rw-rw-rw-   0        0        0      625 2023-07-12 14:39:38.700017 CTkMessagebox-2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1361 2023-07-12 14:38:12.000000 CTkMessagebox-2.3/setup.py
```

### Comparing `CTkMessagebox-2.2/CTkMessagebox/ctkmessagebox.py` & `CTkMessagebox-2.3/CTkMessagebox/ctkmessagebox.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """
 CustomTkinter Messagebox
 Author: Akash Bora
-Version: 2.2
+Version: 2.3
 """
 
 import customtkinter
 from PIL import Image
 import os
 import sys
 import time
+from typing import Literal
 
 class CTkMessagebox(customtkinter.CTkToplevel):
     ICONS = {
         "check": None,
         "cancel": None,
         "info": None,
         "question": None,
@@ -44,19 +45,22 @@
                  button_hover_color: str = "default",
                  icon: str = "info",
                  icon_size: tuple = None,
                  corner_radius: int = 15,
                  font: tuple = None,
                  header: bool = False,
                  topmost: bool = True,
-                 fade_in_duration: int = 0):
+                 fade_in_duration: int = 0,
+                 option_focus: Literal[1, 2, 3] = None):
         
         super().__init__()
-
+        
+        
         self.master_window = master
+     
         self.width = 250 if width<250 else width
         self.height = 150 if height<150 else  height
             
         if self.master_window is None:
             self.spawn_x = int((self.winfo_screenwidth()-self.width)/2)
             self.spawn_y = int((self.winfo_screenheight()-self.height)/2)
         else:
@@ -68,15 +72,15 @@
         self.title(title)
         self.resizable(width=False, height=False)
         self.fade = fade_in_duration
         
         if self.fade:
             self.fade = 20 if self.fade<20 else self.fade
             self.attributes("-alpha", 0)
-            
+        
         if not header:
             self.overrideredirect(1)
     
         if topmost:
             self.attributes("-topmost", True)
         else:
             self.transient(self.master_window)
@@ -91,14 +95,15 @@
             default_cancel_button = "circle"
         else:
             self.transparent_color = '#000001'
             corner_radius = 0
             default_cancel_button = "cross"
 
         self.lift()
+        
         self.config(background=self.transparent_color)
         self.protocol("WM_DELETE_WINDOW", self.button_event)
         self.grid_columnconfigure(0, weight=1)
         self.grid_rowconfigure(0, weight=1)    
         self.x = self.winfo_x()
         self.y = self.winfo_y()
         self._title = title
@@ -230,24 +235,24 @@
         self.button_1 = customtkinter.CTkButton(self.frame_top, text=self.option_text_1, fg_color=self.button_color[0],
                                                 width=self.button_width, font=self.font, text_color=self.bt_text_color,
                                                 hover_color=self.bt_hv_color, height=self.button_height,
                                                 command=lambda: self.button_event(self.option_text_1))
         
         self.button_1.grid(row=2, column=3, sticky="news", padx=(0,10), pady=10)
 
-        if option_2:
-            self.option_text_2 = option_2      
+        self.option_text_2 = option_2 
+        if option_2:     
             self.button_2 = customtkinter.CTkButton(self.frame_top, text=self.option_text_2, fg_color=self.button_color[1],
                                                     width=self.button_width, font=self.font, text_color=self.bt_text_color,
                                                     hover_color=self.bt_hv_color, height=self.button_height,
                                                     command=lambda: self.button_event(self.option_text_2))
             self.button_2.grid(row=2, column=2, sticky="news", padx=10, pady=10)
-            
+
+        self.option_text_3 = option_3
         if option_3:
-            self.option_text_3 = option_3
             self.button_3 = customtkinter.CTkButton(self.frame_top, text=self.option_text_3, fg_color=self.button_color[2],
                                                     width=self.button_width, font=self.font, text_color=self.bt_text_color,
                                                     hover_color=self.bt_hv_color, height=self.button_height,
                                                     command=lambda: self.button_event(self.option_text_3))
             self.button_3.grid(row=2, column=1, sticky="news", padx=(10,0), pady=10)
 
         if header:
@@ -257,14 +262,69 @@
 
         if self.winfo_exists():
             self.grab_set()
             
         if self.fade:
             self.fade_in()
             
+        if option_focus:
+            self.option_focus = option_focus
+            self.focus_button(self.option_focus)
+        else:
+            if not self.option_text_2 and not self.option_text_3:
+                self.button_1.focus()
+                self.button_1.bind("<Return>", lambda event: self.button_event(self.option_text_1))
+ 
+        self.bind("<Escape>", lambda e: self.button_event())
+        
+    def focus_button(self, option_focus):
+        try:
+            self.selected_button = getattr(self, "button_"+str(option_focus))
+            self.selected_button.focus()
+            self.selected_button.configure(border_color=self.bt_hv_color, border_width=3)
+            self.selected_option = getattr(self, "option_text_"+str(option_focus))
+            self.selected_button.bind("<Return>", lambda event: self.button_event(self.selected_option))
+        except AttributeError:
+            return
+        
+        self.bind("<Left>", lambda e: self.change_left())
+        self.bind("<Right>", lambda e: self.change_right())
+        
+    def change_left(self):
+        if self.option_focus==3:
+            return
+        
+        self.selected_button.unbind("<Return>")
+        self.selected_button.configure(border_width=0)
+    
+        if self.option_focus==1:
+            if self.option_text_2:
+                self.option_focus = 2
+        
+        elif self.option_focus==2:
+            if self.option_text_3:
+                self.option_focus = 3
+  
+        self.focus_button(self.option_focus)
+        
+    def change_right(self):
+        if self.option_focus==1:
+            return
+        
+        self.selected_button.unbind("<Return>")
+        self.selected_button.configure(border_width=0)
+
+        if self.option_focus==2:
+            self.option_focus = 1
+
+        elif self.option_focus==3:
+            self.option_focus = 2
+                
+        self.focus_button(self.option_focus)
+    
     def load_icon(self, icon, icon_size):
         if icon not in self.ICONS or self.ICONS[icon] is None:
             if icon in ["check", "cancel", "info", "question", "warning"]:
                 image_path = os.path.join(os.path.dirname(os.path.realpath(__file__)), 'icons', icon + '.png')
             else:
                 image_path = icon
             if icon_size:
```

### Comparing `CTkMessagebox-2.2/CTkMessagebox/icons/cancel.png` & `CTkMessagebox-2.3/CTkMessagebox/icons/cancel.png`

 * *Files identical despite different names*

### Comparing `CTkMessagebox-2.2/CTkMessagebox/icons/check.png` & `CTkMessagebox-2.3/CTkMessagebox/icons/check.png`

 * *Files identical despite different names*

### Comparing `CTkMessagebox-2.2/CTkMessagebox/icons/info.png` & `CTkMessagebox-2.3/CTkMessagebox/icons/info.png`

 * *Files identical despite different names*

### Comparing `CTkMessagebox-2.2/CTkMessagebox/icons/question.png` & `CTkMessagebox-2.3/CTkMessagebox/icons/question.png`

 * *Files identical despite different names*

### Comparing `CTkMessagebox-2.2/CTkMessagebox/icons/warning.png` & `CTkMessagebox-2.3/CTkMessagebox/icons/warning.png`

 * *Files identical despite different names*

### Comparing `CTkMessagebox-2.2/CTkMessagebox.egg-info/PKG-INFO` & `CTkMessagebox-2.3/CTkMessagebox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTkMessagebox
-Version: 2.2
+Version: 2.3
 Summary: A modern messagebox for customtkinter
 Home-page: https://github.com/Akascape/CTkMessagebox
 Author: Akash Bora
 License: Creative Commons Zero v1.0 Universal
 Keywords: customtkinter,customtkinter-dialog,customtkinter-messagebox,customtkinter-message-box,tkinter-messagebox,customtkinter-tkinter-messagebox,messagebox-widget,modern-tkinter-messagebox,ctkmessagebox
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3
@@ -159,14 +159,15 @@
   | _cancel_button_color_ | color of the **close** button, **set it to 'transparent' if you want to hide it** |
   | **_icon_** | icon that will be shown in the messagebox [Default is the 'info' icon] |
   | _icon_size_ | define the size of the icon image manually (tuple) |
   | _corner_radius_ | corner roundness of the messagebox window [**not applicable in linux**] |
   | _font_ | font of the messagebox text (tuple) |
   | _header_ | add the original header back if you don't like **overrideredirect** (bool) |
   | _topmost_ | disable the topmost window outside the app (bool) |
+  | _focus_option_ | select an option by default when `Enter` key is pressed |
   | **_fade_in_duration_** | enable a fade-in and fade-out animation (int, default is 0)  |
 
 </div>
 
 <br>
 
 <h2 align="center"> Icons </h2>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: CTkMessagebox Version: 2.2 Summary: A modern
+Metadata-Version: 2.1 Name: CTkMessagebox Version: 2.3 Summary: A modern
 messagebox for customtkinter Home-page: https://github.com/Akascape/
 CTkMessagebox Author: Akash Bora License: Creative Commons Zero v1.0 Universal
 Keywords: customtkinter,customtkinter-dialog,customtkinter-
 messagebox,customtkinter-message-box,tkinter-messagebox,customtkinter-tkinter-
 messagebox,messagebox-widget,modern-tkinter-messagebox,ctkmessagebox
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
@@ -80,14 +80,15 @@
 of the **close** button, **set it to 'transparent' if you want to hide it** | |
  **_icon_** | icon that will be shown in the messagebox [Default is the 'info'
 icon] | | _icon_size_ | define the size of the icon image manually (tuple) | |
  _corner_radius_ | corner roundness of the messagebox window [**not applicable
 in linux**] | | _font_ | font of the messagebox text (tuple) | | _header_ | add
   the original header back if you don't like **overrideredirect** (bool) | |
        _topmost_ | disable the topmost window outside the app (bool) | |
+ _focus_option_ | select an option by default when `Enter` key is pressed | |
 **_fade_in_duration_** | enable a fade-in and fade-out animation (int, default
                                     is 0) |
 
                                ***** Icons *****
 **Default icons:** ![icons](https://user-images.githubusercontent.com/89206401/
  221258403-aafea575-856e-4f4e-b3af-f995785c9879.png) (*These icons are created
          using Paint.NET, free to use!*) **For custom images, just use
```

### Comparing `CTkMessagebox-2.2/LICENSE` & `CTkMessagebox-2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `CTkMessagebox-2.2/PKG-INFO` & `CTkMessagebox-2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTkMessagebox
-Version: 2.2
+Version: 2.3
 Summary: A modern messagebox for customtkinter
 Home-page: https://github.com/Akascape/CTkMessagebox
 Author: Akash Bora
 License: Creative Commons Zero v1.0 Universal
 Keywords: customtkinter,customtkinter-dialog,customtkinter-messagebox,customtkinter-message-box,tkinter-messagebox,customtkinter-tkinter-messagebox,messagebox-widget,modern-tkinter-messagebox,ctkmessagebox
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3
@@ -159,14 +159,15 @@
   | _cancel_button_color_ | color of the **close** button, **set it to 'transparent' if you want to hide it** |
   | **_icon_** | icon that will be shown in the messagebox [Default is the 'info' icon] |
   | _icon_size_ | define the size of the icon image manually (tuple) |
   | _corner_radius_ | corner roundness of the messagebox window [**not applicable in linux**] |
   | _font_ | font of the messagebox text (tuple) |
   | _header_ | add the original header back if you don't like **overrideredirect** (bool) |
   | _topmost_ | disable the topmost window outside the app (bool) |
+  | _focus_option_ | select an option by default when `Enter` key is pressed |
   | **_fade_in_duration_** | enable a fade-in and fade-out animation (int, default is 0)  |
 
 </div>
 
 <br>
 
 <h2 align="center"> Icons </h2>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: CTkMessagebox Version: 2.2 Summary: A modern
+Metadata-Version: 2.1 Name: CTkMessagebox Version: 2.3 Summary: A modern
 messagebox for customtkinter Home-page: https://github.com/Akascape/
 CTkMessagebox Author: Akash Bora License: Creative Commons Zero v1.0 Universal
 Keywords: customtkinter,customtkinter-dialog,customtkinter-
 messagebox,customtkinter-message-box,tkinter-messagebox,customtkinter-tkinter-
 messagebox,messagebox-widget,modern-tkinter-messagebox,ctkmessagebox
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
@@ -80,14 +80,15 @@
 of the **close** button, **set it to 'transparent' if you want to hide it** | |
  **_icon_** | icon that will be shown in the messagebox [Default is the 'info'
 icon] | | _icon_size_ | define the size of the icon image manually (tuple) | |
  _corner_radius_ | corner roundness of the messagebox window [**not applicable
 in linux**] | | _font_ | font of the messagebox text (tuple) | | _header_ | add
   the original header back if you don't like **overrideredirect** (bool) | |
        _topmost_ | disable the topmost window outside the app (bool) | |
+ _focus_option_ | select an option by default when `Enter` key is pressed | |
 **_fade_in_duration_** | enable a fade-in and fade-out animation (int, default
                                     is 0) |
 
                                ***** Icons *****
 **Default icons:** ![icons](https://user-images.githubusercontent.com/89206401/
  221258403-aafea575-856e-4f4e-b3af-f995785c9879.png) (*These icons are created
          using Paint.NET, free to use!*) **For custom images, just use
```

### Comparing `CTkMessagebox-2.2/README.md` & `CTkMessagebox-2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -144,14 +144,15 @@
   | _cancel_button_color_ | color of the **close** button, **set it to 'transparent' if you want to hide it** |
   | **_icon_** | icon that will be shown in the messagebox [Default is the 'info' icon] |
   | _icon_size_ | define the size of the icon image manually (tuple) |
   | _corner_radius_ | corner roundness of the messagebox window [**not applicable in linux**] |
   | _font_ | font of the messagebox text (tuple) |
   | _header_ | add the original header back if you don't like **overrideredirect** (bool) |
   | _topmost_ | disable the topmost window outside the app (bool) |
+  | _focus_option_ | select an option by default when `Enter` key is pressed |
   | **_fade_in_duration_** | enable a fade-in and fade-out animation (int, default is 0)  |
 
 </div>
 
 <br>
 
 <h2 align="center"> Icons </h2>
```

#### html2text {}

```diff
@@ -70,14 +70,15 @@
 of the **close** button, **set it to 'transparent' if you want to hide it** | |
  **_icon_** | icon that will be shown in the messagebox [Default is the 'info'
 icon] | | _icon_size_ | define the size of the icon image manually (tuple) | |
  _corner_radius_ | corner roundness of the messagebox window [**not applicable
 in linux**] | | _font_ | font of the messagebox text (tuple) | | _header_ | add
   the original header back if you don't like **overrideredirect** (bool) | |
        _topmost_ | disable the topmost window outside the app (bool) | |
+ _focus_option_ | select an option by default when `Enter` key is pressed | |
 **_fade_in_duration_** | enable a fade-in and fade-out animation (int, default
                                     is 0) |
 
                                ***** Icons *****
 **Default icons:** ![icons](https://user-images.githubusercontent.com/89206401/
  221258403-aafea575-856e-4f4e-b3af-f995785c9879.png) (*These icons are created
          using Paint.NET, free to use!*) **For custom images, just use
```

### Comparing `CTkMessagebox-2.2/setup.cfg` & `CTkMessagebox-2.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2043 546b 4d65 7373 6167 6562 6f78   = CTkMessagebox
-00000020: 0d0a 7665 7273 696f 6e20 3d20 322e 320d  ..version = 2.2.
+00000020: 0d0a 7665 7273 696f 6e20 3d20 322e 330d  ..version = 2.3.
 00000030: 0a64 6573 6372 6970 7469 6f6e 203d 2041  .description = A
 00000040: 206d 6f64 6572 6e20 6d65 7373 6167 6562   modern messageb
 00000050: 6f78 2066 6f72 2063 7573 746f 6d74 6b69  ox for customtki
 00000060: 6e74 6572 0d0a 6c6f 6e67 5f64 6573 6372  nter..long_descr
 00000070: 6970 7469 6f6e 203d 2066 696c 653a 2052  iption = file: R
 00000080: 4541 444d 452e 6d64 0d0a 6c6f 6e67 5f64  EADME.md..long_d
 00000090: 6573 6372 6970 7469 6f6e 5f63 6f6e 7465  escription_conte
```

### Comparing `CTkMessagebox-2.2/setup.py` & `CTkMessagebox-2.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     """Opens and fetches text of long descrition file."""
     with open(path, 'r') as f:
         text = f.read()
     return text
 
 setup(
     name = 'CTkMessagebox',
-    version = '2.2',
+    version = '2.3',
     description = "A modern messagebox for customtkinter",
     license = "Creative Commons Zero v1.0 Universal",
     readme = "README.md",
     long_description = get_long_description('README.md'),
     long_description_content_type = "text/markdown",
     author = 'Akash Bora',
     url = "https://github.com/Akascape/CTkMessagebox",
```

