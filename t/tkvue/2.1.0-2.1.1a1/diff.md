# Comparing `tmp/tkvue-2.1.0-py3-none-any.whl.zip` & `tmp/tkvue-2.1.1a1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 195841 bytes, number of entries: 10
--rw-r--r--  2.0 unx    31690 b- defN 23-Apr-19 13:17 tkvue/__init__.py
+Zip file size: 196235 bytes, number of entries: 10
+-rw-r--r--  2.0 unx    31759 b- defN 23-Jul-12 18:21 tkvue/__init__.py
 -rw-rw-rw-  2.0 unx   170486 b- defN 22-Nov-09 20:32 tkvue/tests/preloader.gif
 -rw-rw-rw-  2.0 unx      814 b- defN 22-Nov-09 20:32 tkvue/tests/python_icon.png
--rw-rw-rw-  2.0 unx    22264 b- defN 23-Feb-26 16:44 tkvue/tests/test_tkvue.py
--rw-rw-rw-  2.0 unx    26523 b- defN 23-Apr-20 17:27 tkvue-2.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     6250 b- defN 23-Apr-20 17:27 tkvue-2.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-20 17:27 tkvue-2.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       47 b- defN 23-Apr-20 17:27 tkvue-2.1.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 23-Apr-20 17:27 tkvue-2.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      794 b- defN 23-Apr-20 17:27 tkvue-2.1.0.dist-info/RECORD
-10 files, 258966 bytes uncompressed, 194497 bytes compressed:  24.9%
+-rw-rw-rw-  2.0 unx    23217 b- defN 23-Jul-12 18:21 tkvue/tests/test_tkvue.py
+-rw-rw-rw-  2.0 unx    26523 b- defN 23-Jul-12 18:21 tkvue-2.1.1a1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6252 b- defN 23-Jul-12 18:21 tkvue-2.1.1a1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-12 18:21 tkvue-2.1.1a1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       47 b- defN 23-Jul-12 18:21 tkvue-2.1.1a1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 23-Jul-12 18:21 tkvue-2.1.1a1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      806 b- defN 23-Jul-12 18:21 tkvue-2.1.1a1.dist-info/RECORD
+10 files, 260002 bytes uncompressed, 194867 bytes compressed:  25.1%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: tkvue/tests/python_icon.png
 Comment: 
 
 Filename: tkvue/tests/test_tkvue.py
 Comment: 
 
-Filename: tkvue-2.1.0.dist-info/LICENSE
+Filename: tkvue-2.1.1a1.dist-info/LICENSE
 Comment: 
 
-Filename: tkvue-2.1.0.dist-info/METADATA
+Filename: tkvue-2.1.1a1.dist-info/METADATA
 Comment: 
 
-Filename: tkvue-2.1.0.dist-info/WHEEL
+Filename: tkvue-2.1.1a1.dist-info/WHEEL
 Comment: 
 
-Filename: tkvue-2.1.0.dist-info/entry_points.txt
+Filename: tkvue-2.1.1a1.dist-info/entry_points.txt
 Comment: 
 
-Filename: tkvue-2.1.0.dist-info/top_level.txt
+Filename: tkvue-2.1.1a1.dist-info/top_level.txt
 Comment: 
 
-Filename: tkvue-2.1.0.dist-info/RECORD
+Filename: tkvue-2.1.1a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tkvue/__init__.py

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2021 IKUS Software inc. All rights reserved.
+# Copyright (C) 2023 IKUS Software. All rights reserved.
 # IKUS Software inc. PROPRIETARY/CONFIDENTIAL.
 # Use is subject to license terms.
 import asyncio
 import collections
 import functools
 import logging
 import os
@@ -588,32 +588,33 @@
     Let provide our own Scrolled frame supporting styled background color.
     """
 
     def __init__(self, master, *args, **kw):
 
         # track changes to the canvas and frame width and sync them,
         # also updating the scrollbar
-        def _configure_interior(event):
-            # update the scrollbars to match the size of the inner frame
-            size = (interior.winfo_reqwidth(), interior.winfo_reqheight())
-            canvas.config(scrollregion="0 0 %s %s" % size)
-            if interior.winfo_reqwidth() != canvas.winfo_width():
-                # update the canvas's width to fit the inner frame
-                canvas.config(width=interior.winfo_reqwidth())
-
-        def _configure_canvas(event):
-            # update the inner frame's width to fill the canvas
-            if interior.winfo_reqwidth() != canvas.winfo_width():
-                canvas.itemconfigure(interior_id, width=canvas.winfo_width())
-            # Show / Hide vertical scrollbar
-            if canvas.yview() == (0.0, 1.0):
+        def _update_scroll_region(event):
+            # Update the scroll region when the interior widget is resized.
+            # Since we only scroll on y axis, take the width from canvas and height from interior.
+            canvas.config(scrollregion=(0, 0, interior.winfo_width(), interior.winfo_reqheight()))
+            # Show/hide scroll bar as needed
+            if canvas.winfo_height() > interior.winfo_reqheight():
                 self.vscrollbar.forget()
             else:
                 self.vscrollbar.pack(fill=tkinter.Y, side=tkinter.RIGHT, expand=tkinter.FALSE)
 
+        def _configure_canvas(event):
+            # The current width of the canvas
+            canvas_width = canvas.winfo_width()
+            # The interior widget's requested width
+            requested_width = interior.winfo_reqwidth()
+            # update the inner frame's width to fill the canvas
+            if canvas_width != requested_width:
+                canvas.itemconfigure(interior_id, width=canvas_width)
+
         def _on_mousewheel(event):
             # Skip scroll if canvas is bigger then content.
             if canvas.yview() == (0.0, 1.0):
                 return
             # Pick scroll directio dependinds of event <Button-?> or delta value <MouseWheel>
             if event.num == 5 or event.delta < 0:
                 scroll = 1
@@ -649,15 +650,15 @@
         canvas.xview_moveto(0)
         canvas.yview_moveto(0)
 
         # create a frame inside the canvas which will be scrolled with it
         self.interior = interior = ttk.Frame(canvas)
         interior_id = canvas.create_window(0, 0, window=interior, anchor=tkinter.NW)
 
-        interior.bind("<Configure>", _configure_interior)
+        interior.bind("<Configure>", _update_scroll_region)
         canvas.bind("<Configure>", _configure_canvas)
         canvas.bind("<Enter>", _bind_to_mousewheel)
         canvas.bind("<Leave>", _unbind_from_mousewheel)
         canvas.bind("<<ThemeChanged>>", _update_bg)
 
 
 class TemplateError(Exception):
```

## tkvue/tests/test_tkvue.py

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2021 IKUS Software inc. All rights reserved.
+# Copyright (C) 2023 IKUS Software. All rights reserved.
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This library is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -299,17 +299,19 @@
     def __init__(self, master=None):
         self.data = tkvue.Context({"items": []})
         super().__init__(master=master)
 
 
 class DialogWithScrolledFrame(tkvue.Component):
     template = """
-    <TopLevel>
-        <ScrolledFrame id="scrolled_frame">
-            <Label id="label1" text="{{item}}" for="item in range(1,25)"/>
+    <TopLevel geometry="500x500">
+        <ScrolledFrame id="scrolled_frame" pack-fill="both" pack-expand="1">
+            <Frame for="item in range(1,10)" pack-fill="x"  pack-expand="1">
+                <Label id="label1" pack-fill="x" pack-expand="1" text="Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. " wrap="1"/>
+            </Frame>
         </ScrolledFrame>
     </TopLevel>
     """
 
 
 class DialogWithInvalidCommand(tkvue.Component):
     template = """
@@ -550,14 +552,26 @@
             # Then widget get created
             self.assertEqual(2, len(dlg.winfo_children()))
 
     def test_scrolled_frame(self):
         with new_dialog(DialogWithScrolledFrame) as dlg:
             dlg.pump_events()
 
+    @unittest.skipUnless(IS_LINUX, "fail randomly on Windows and MacOS due to race condition")
+    def test_scrolled_frame_resize(self):
+        with new_dialog(DialogWithScrolledFrame) as dlg:
+            dlg.pump_events()
+            # Make sure scrollable is working
+            self.assertTrue(dlg.scrolled_frame.vscrollbar.winfo_ismapped())
+            # When dialog is resize
+            dlg.geometry('800x800')
+            dlg.pump_events()
+            # Then scrollbar is removed
+            self.assertFalse(dlg.scrolled_frame.vscrollbar.winfo_ismapped())
+
     def test_command_invalid(self):
         # Given a dialog with an invalid command name
         # When trying to create the dialog
         # Then an exception is raised
         with self.assertRaises(tkvue.TemplateError) as ctx:
             with new_dialog(DialogWithInvalidCommand) as dlg:
                 dlg.pump_events()
```

## Comparing `tkvue-2.1.0.dist-info/LICENSE` & `tkvue-2.1.1a1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tkvue-2.1.0.dist-info/METADATA` & `tkvue-2.1.1a1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkvue
-Version: 2.1.0
+Version: 2.1.1a1
 Summary: Declarative Tkinter UI using makup language with reactive data binding
 Home-page: https://gitlab.com/ikus-soft/tkvue
 Author: IKUS Software inc.
 Author-email: support@ikus-soft.com
 Maintainer: Patrik Dufresne
 Maintainer-email: patrik@ikus-soft.com
 License: LGPLv3
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tkvue Version: 2.1.0 Summary: Declarative Tkinter
+Metadata-Version: 2.1 Name: tkvue Version: 2.1.1a1 Summary: Declarative Tkinter
 UI using makup language with reactive data binding Home-page: https://
 gitlab.com/ikus-soft/tkvue Author: IKUS Software inc. Author-email:
 support@ikus-soft.com Maintainer: Patrik Dufresne Maintainer-email:
 patrik@ikus-soft.com License: LGPLv3 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: X11 Applications Classifier: Environment :: Win32
 (MS Windows) Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: End Users/Desktop Classifier: License :: OSI Approved :: GNU Lesser
```

## Comparing `tkvue-2.1.0.dist-info/RECORD` & `tkvue-2.1.1a1.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-tkvue/__init__.py,sha256=NJqQc7rPz-9_vi_qWHoYG2FY3CKzJZFKFYkClwvDM1c,31690
+tkvue/__init__.py,sha256=EKCfF5iy3hv1ECtXfORb2ajPuWDeYbALcTSzHKXSBIk,31759
 tkvue/tests/preloader.gif,sha256=4WubudKMAoutzmKtq4PR70A8DoCy5GC_fdVn08FRItc,170486
 tkvue/tests/python_icon.png,sha256=TNB4Jv9uPJYDC9CxCVUv6q5Fu6mlSx2Skuk68ckAcqQ,814
-tkvue/tests/test_tkvue.py,sha256=Kv2ktnpBG8k4xPIwcX9QYI9hh2BI06UOF1y8m8sNYM8,22264
-tkvue-2.1.0.dist-info/LICENSE,sha256=wOyDtdXHKbVMd0kW1v8xZvyrYk9MeGP2-70glJMR9nc,26523
-tkvue-2.1.0.dist-info/METADATA,sha256=8EWYG1-3J-S0jE_sIOAMiMmgzxpuRNP2CdQ-xNHsjnc,6250
-tkvue-2.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-tkvue-2.1.0.dist-info/entry_points.txt,sha256=8VY5M0e9X8hXWRDu4nXU60waEEcTmLS5mRgxCmcVE88,47
-tkvue-2.1.0.dist-info/top_level.txt,sha256=anZORAc3YItPGY-GYRZ9zA_9cHsS-bhOtuYTL0R6ffU,6
-tkvue-2.1.0.dist-info/RECORD,,
+tkvue/tests/test_tkvue.py,sha256=ou_M6PUEyTeVlPOA0UfTAaW4OyZigxjcXX7m86Cnv7A,23217
+tkvue-2.1.1a1.dist-info/LICENSE,sha256=wOyDtdXHKbVMd0kW1v8xZvyrYk9MeGP2-70glJMR9nc,26523
+tkvue-2.1.1a1.dist-info/METADATA,sha256=nv1HTIIoROWtnQdmDY_hZzgGW2DwmdwCfajhtoCe7nI,6252
+tkvue-2.1.1a1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+tkvue-2.1.1a1.dist-info/entry_points.txt,sha256=8VY5M0e9X8hXWRDu4nXU60waEEcTmLS5mRgxCmcVE88,47
+tkvue-2.1.1a1.dist-info/top_level.txt,sha256=anZORAc3YItPGY-GYRZ9zA_9cHsS-bhOtuYTL0R6ffU,6
+tkvue-2.1.1a1.dist-info/RECORD,,
```

