# Comparing `tmp/tklinenums-1.6.5.tar.gz` & `tmp/tklinenums-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tklinenums-1.6.5.tar", last modified: Sat Apr 22 19:07:28 2023, max compression
+gzip compressed data, was "tklinenums-1.7.0.tar", last modified: Wed Jul 12 13:03:57 2023, max compression
```

## Comparing `tklinenums-1.6.5.tar` & `tklinenums-1.7.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 19:07:28.629502 tklinenums-1.6.5/
--rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-04-22 19:07:28.629502 tklinenums-1.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-04-22 19:07:08.000000 tklinenums-1.6.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-22 19:07:08.000000 tklinenums-1.6.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 19:07:28.629502 tklinenums-1.6.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-22 19:07:08.000000 tklinenums-1.6.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 19:07:28.629502 tklinenums-1.6.5/tklinenums/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 19:07:08.000000 tklinenums-1.6.5/tklinenums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10970 2023-04-22 19:07:08.000000 tklinenums-1.6.5/tklinenums/tklinenums.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 19:07:28.629502 tklinenums-1.6.5/tklinenums.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-04-22 19:07:28.000000 tklinenums-1.6.5/tklinenums.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-22 19:07:28.000000 tklinenums-1.6.5/tklinenums.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 19:07:28.000000 tklinenums-1.6.5/tklinenums.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-22 19:07:28.000000 tklinenums-1.6.5/tklinenums.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:03:57.002887 tklinenums-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-07-12 13:03:57.002887 tklinenums-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-07-12 13:03:39.000000 tklinenums-1.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-12 13:03:39.000000 tklinenums-1.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 13:03:57.002887 tklinenums-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-12 13:03:39.000000 tklinenums-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:03:56.998886 tklinenums-1.7.0/tklinenums/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-12 13:03:39.000000 tklinenums-1.7.0/tklinenums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12865 2023-07-12 13:03:39.000000 tklinenums-1.7.0/tklinenums/tklinenums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 13:03:57.002887 tklinenums-1.7.0/tklinenums.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-07-12 13:03:56.000000 tklinenums-1.7.0/tklinenums.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-12 13:03:56.000000 tklinenums-1.7.0/tklinenums.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 13:03:56.000000 tklinenums-1.7.0/tklinenums.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-12 13:03:56.000000 tklinenums-1.7.0/tklinenums.egg-info/top_level.txt
```

### Comparing `tklinenums-1.6.5/PKG-INFO` & `tklinenums-1.7.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tklinenums
-Version: 1.6.5
+Version: 1.7.0
 Summary: A simple Tkinter widget for displaying line numbers
 Home-page: https://github.com/Moosems/TkLineNums
 Author: Moosems
 Author-email: moosems.j@gmail.com
 Description-Content-Type: text/markdown
 
 <h1 align="center">TkLineNums</h1>
@@ -18,73 +18,63 @@
 ![img](https://github.com/Moosems/TkLineNums/raw/main/images/TkLineNumsPhoto.png)
 
 ## Features of the `TkLineNums` widget:
 
 - Clicking on line numbers will set the insert to the beginning of the line.
 - Shift clicking will select all text from the end of the line clicked by cursor and the insert position.
 - Scrolling the linebar will scroll the text widget (and vice versa).
-- Supports ttk themes (by usage of the `.set_to_ttk_style()` method)
-- Supports left, right, and center alignment with the `-justify` option
-- Clicking and then dragging the mouse will scroll the text widget (see [#8](https://github.com/Moosems/TkLineNums/pull/8))
+- Can handle elided lines (elided lines are lines that are not visible in the text widget).
+- Supports ttk themes and allows easy color customization.
+- Supports left, right, and center alignment with the `-justify` option.
+- Clicking and then dragging the mouse will scroll the text widget (see [#8](https://github.com/Moosems/TkLineNums/pull/8)).
 
 # Installation
-`pip install tklinenums`
+
+In the Command Line, paste the following: `pip install tklinenums`.
 
 ## Documentation
 ### `TkLineNums` Widget
 |Options|Description|Type|
 |---|---|---|
 |master|The parent widget|Tkinter widget (defaults to `tkinter.Misc`)|
-|editor|The `Text` widget the line numbers will connect to|Tkinter `Text` widget (or child class)|
+|textwidget|The `Text` widget the line numbers will connect to|Tkinter `Text` widget (or child class)|
 |justify|The alignment of the line numbers|A string as either `"left"`, `"right"`, or `"center"`|
+|colors|A way to provide coloring to the line numbers|A function, `(foreground, background)` tuple, or None. None (default) makes it use the `Text` widget's coloring. The function should return a `(foreground, background)` tuple: it will be called whenever the colors are needed, and it is useful when the colors can change.|
 |*args|Arguments for the `Canvas` widget|Any arguments used for the `Canvas` widget|
 |**kwargs|Keyword arguments for the `Canvas` widget|Any keyword arguments used for the `Canvas` widget|
 
 ### Basic Usage:
 ```python
-from platform import system
 from tkinter import Text, Tk
 from tkinter.ttk import Style
 
 from tklinenums import TkLineNumbers
 
-# This is to make the example work on both Windows and Mac
-if system() == "Darwin":
-    contmand: str = "Command"
-else:
-    contmand: str = "Control"
-
 # Create the root window
 root = Tk()
 
-# Set the ttk style (tkinter's way of styling) for the line numbers
-style = Style()
-style.configure("TLineNumbers", background="#ffffff", foreground="#2197db")
-
 # Create the Text widget and pack it to the right
 text = Text(root)
 text.pack(side="right")
 
 # Insert 50 lines of text into the Text widget
 for i in range(50):
     text.insert("end", f"Line {i+1}\n")
 
 # Create the TkLineNumbers widget and pack it to the left
-linenums = TkLineNumbers(root, text)
+linenums = TkLineNumbers(root, text, justify="center", colors=("#2197db", "#ffffff"))
 linenums.pack(fill="y", side="left")
 
-# Create binds to redraw the line numbers for most common events that change the text in the Text widget
-text.bind("<Key>", lambda event: root.after_idle(linenums.redraw), add=True)
-text.bind("<BackSpace>", lambda event: root.after_idle(linenums.redraw), add=True)
-text.bind(f"<{contmand}-v>", lambda event: root.after_idle(linenums.redraw), add=True)
+# Redraw the line numbers when the text widget contents are modified
+text.bind("<<Modified>>", lambda event: root.after_idle(linenums.redraw), add=True)
 
 # Start the mainloop for the root window
 root.mainloop()
 ```
-For a more complete example, see the [example.py](./tests/example.py) file.
+For a more complete example, see [example.py](./tests/example.py).
 
 ## How to run and contribute
 
 ### Running
 
 To run the example, run `python3 tests/example.py` in the root directory. The project uses only standard library modules, so there are no dependencies. It will create a window with a `Text` widget and a `TkLineNumbers` widget and 50 lines of text to mess around with.
```

### Comparing `tklinenums-1.6.5/README.md` & `tklinenums-1.7.0/tklinenums.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1
+Name: tklinenums
+Version: 1.7.0
+Summary: A simple Tkinter widget for displaying line numbers
+Home-page: https://github.com/Moosems/TkLineNums
+Author: Moosems
+Author-email: moosems.j@gmail.com
+Description-Content-Type: text/markdown
+
 <h1 align="center">TkLineNums</h1>
 
 > **Note**
 > If Python was installed via Homebrew, installed on Mac by default, or installed on Linux, tkinter will likely not work properly and may need to be installed via `brew install python-tk` or with the distro package manager on Linux as documented [here](https://tecadmin.net/how-to-install-python-tkinter-on-linux/).
 
 ## Description
 `TkLineNums` is a simple line numbering widget for Python's `tkinter` GUI library. It is directly connects to a `Text` widget and even supports ttk themes through the set_to_ttk_style method.
@@ -9,73 +18,63 @@
 ![img](https://github.com/Moosems/TkLineNums/raw/main/images/TkLineNumsPhoto.png)
 
 ## Features of the `TkLineNums` widget:
 
 - Clicking on line numbers will set the insert to the beginning of the line.
 - Shift clicking will select all text from the end of the line clicked by cursor and the insert position.
 - Scrolling the linebar will scroll the text widget (and vice versa).
-- Supports ttk themes (by usage of the `.set_to_ttk_style()` method)
-- Supports left, right, and center alignment with the `-justify` option
-- Clicking and then dragging the mouse will scroll the text widget (see [#8](https://github.com/Moosems/TkLineNums/pull/8))
+- Can handle elided lines (elided lines are lines that are not visible in the text widget).
+- Supports ttk themes and allows easy color customization.
+- Supports left, right, and center alignment with the `-justify` option.
+- Clicking and then dragging the mouse will scroll the text widget (see [#8](https://github.com/Moosems/TkLineNums/pull/8)).
 
 # Installation
-`pip install tklinenums`
+
+In the Command Line, paste the following: `pip install tklinenums`.
 
 ## Documentation
 ### `TkLineNums` Widget
 |Options|Description|Type|
 |---|---|---|
 |master|The parent widget|Tkinter widget (defaults to `tkinter.Misc`)|
-|editor|The `Text` widget the line numbers will connect to|Tkinter `Text` widget (or child class)|
+|textwidget|The `Text` widget the line numbers will connect to|Tkinter `Text` widget (or child class)|
 |justify|The alignment of the line numbers|A string as either `"left"`, `"right"`, or `"center"`|
+|colors|A way to provide coloring to the line numbers|A function, `(foreground, background)` tuple, or None. None (default) makes it use the `Text` widget's coloring. The function should return a `(foreground, background)` tuple: it will be called whenever the colors are needed, and it is useful when the colors can change.|
 |*args|Arguments for the `Canvas` widget|Any arguments used for the `Canvas` widget|
 |**kwargs|Keyword arguments for the `Canvas` widget|Any keyword arguments used for the `Canvas` widget|
 
 ### Basic Usage:
 ```python
-from platform import system
 from tkinter import Text, Tk
 from tkinter.ttk import Style
 
 from tklinenums import TkLineNumbers
 
-# This is to make the example work on both Windows and Mac
-if system() == "Darwin":
-    contmand: str = "Command"
-else:
-    contmand: str = "Control"
-
 # Create the root window
 root = Tk()
 
-# Set the ttk style (tkinter's way of styling) for the line numbers
-style = Style()
-style.configure("TLineNumbers", background="#ffffff", foreground="#2197db")
-
 # Create the Text widget and pack it to the right
 text = Text(root)
 text.pack(side="right")
 
 # Insert 50 lines of text into the Text widget
 for i in range(50):
     text.insert("end", f"Line {i+1}\n")
 
 # Create the TkLineNumbers widget and pack it to the left
-linenums = TkLineNumbers(root, text)
+linenums = TkLineNumbers(root, text, justify="center", colors=("#2197db", "#ffffff"))
 linenums.pack(fill="y", side="left")
 
-# Create binds to redraw the line numbers for most common events that change the text in the Text widget
-text.bind("<Key>", lambda event: root.after_idle(linenums.redraw), add=True)
-text.bind("<BackSpace>", lambda event: root.after_idle(linenums.redraw), add=True)
-text.bind(f"<{contmand}-v>", lambda event: root.after_idle(linenums.redraw), add=True)
+# Redraw the line numbers when the text widget contents are modified
+text.bind("<<Modified>>", lambda event: root.after_idle(linenums.redraw), add=True)
 
 # Start the mainloop for the root window
 root.mainloop()
 ```
-For a more complete example, see the [example.py](./tests/example.py) file.
+For a more complete example, see [example.py](./tests/example.py).
 
 ## How to run and contribute
 
 ### Running
 
 To run the example, run `python3 tests/example.py` in the root directory. The project uses only standard library modules, so there are no dependencies. It will create a window with a `Text` widget and a `TkLineNumbers` widget and 50 lines of text to mess around with.
```

### Comparing `tklinenums-1.6.5/tklinenums/tklinenums.py` & `tklinenums-1.7.0/tklinenums/tklinenums.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,277 +1,346 @@
 """TkLineNumbers - A line number widget for tkinter Text widgets"""
 from __future__ import annotations
 
-import platform
-from tkinter import Canvas, Event, Misc, Text
+from platform import system
+from tkinter import Canvas, Event, Misc, Text, getboolean
 from tkinter.font import Font
+from typing import Callable, Optional
 
-system: str = str(platform.system())
-if system in ("Darwin" or "Windows"):
-    scroll_inversion = lambda delta: -delta
-else:
-    scroll_inversion = lambda delta: int(delta / 120)
+SYSTEM = system()
+
+
+def scroll_fix(delta: int) -> int:
+    """Corrects scrolling numbers across platforms"""
+
+    # The scroll events passed by MacOS are different from Windows and Linux
+    # so it must to be rectified to work properly when dealing with the events.
+    # Originally found here: https://stackoverflow.com/a/17457843/17053202
+    if delta in (4, 5):
+        # Linux device
+        result = delta / 4 if delta == 4 else -delta / 5
+    result = -delta if SYSTEM == "Darwin" else delta / 120
+    return int(result)
 
 
 class TkLineNumError(Exception):
     ...
 
 
 class TkLineNumbers(Canvas):
     """
     Creates a line number widget for a text widget. Options are the same as a tkinter Canvas widget and add the following:
-        * -editor (Text): The text widget to attach the line numbers to. (Required) (Second argument after master)
+        * -textwidget (Text): The text widget to attach the line numbers to. (Required) (Second argument after master)
         * -justify (str): The justification of the line numbers. Can be "left", "right", or "center". Default is "left".
 
     Methods to be used outside externally:
-        * .redraw(): Redraws the widget
-        * .resize(): Calculates the required width of the widget and resizes it according to the text widget's font and the number of lines
-        * .set_to_ttk_style(): Sets the foreground and background colors to the ttk style of the text widget
-        * .reload(): Reloads the style of the widget and redraws it.
+        * .redraw(): Redraws the widget (to be used when the text widget is modified)
     """
 
     def __init__(
-        self,
+        self: TkLineNumbers,
         master: Misc,
-        editor: Text,
+        textwidget: Text,
         justify: str = "left",
+        # None means take colors from text widget (default).
+        # Otherwise it is a function that takes no arguments and returns (fg, bg) tuple.
+        colors: Callable[[], tuple[str, str]] | tuple[str, str] | None = None,
         *args,
         **kwargs,
     ) -> None:
         """Initializes the widget -- Internal use only"""
+
+        # Initialize the Canvas widget
         Canvas.__init__(
             self,
             master,
             width=kwargs.pop("width", 40),
             highlightthickness=kwargs.pop("highlightthickness", 0),
             borderwidth=kwargs.pop("borderwidth", 2),
             relief=kwargs.pop("relief", "ridge"),
             *args,
             **kwargs,
         )
-    
-        # Set variable
-        self.textwidget = editor
+
+        # Set variables
+        self.textwidget = textwidget
         self.master = master
         self.justify = justify
+        self.cancellable_after: Optional[str] = None
         self.click_pos: None = None
+        self.colors = colors
+        self.x = None
+        self.y = None
+
+        # Set style and its binding
+        self.set_colors()
+        self.bind("<<ThemeChanged>>", self.set_colors, add=True)
 
-        # Set style
-        self.set_to_ttk_style()
-
-        # Event bindings
+        # Mouse scroll binding
         self.bind("<MouseWheel>", self.mouse_scroll, add=True)
+        self.bind("<Button-4>", self.mouse_scroll, add=True)
+        self.bind("<Button-5>", self.mouse_scroll, add=True)
+
+        # Click bindings
         self.bind("<Button-1>", self.click_see, add=True)
         self.bind("<ButtonRelease-1>", self.unclick, add=True)
         self.bind("<Double-Button-1>", self.double_click, add=True)
-        self.bind("<Button1-Motion>", self.drag, add=True)
-        self.bind("<Button1-Leave>", self.auto_scroll, add=True)
+
+        # Mouse drag bindings
+        self.bind("<Button1-Motion>", self.in_widget_select_mouse_drag, add=True)
+        self.bind("<Button1-Leave>", self.mouse_off_screen_scroll, add=True)
+        self.bind("<Button1-Enter>", self.stop_mouse_off_screen_scroll, add=True)
 
         # Set the yscrollcommand of the text widget to redraw the widget
-        editor["yscrollcommand"] = self.redraw
+        textwidget["yscrollcommand"] = self.redraw
 
-    def redraw(self, *args) -> None:
+        # Redraw the widget
+        self.redraw()
+
+    def redraw(self, *_) -> None:
         """Redraws the widget"""
-        # Resize the widget based on the number of lines in the editor
+
+        # Resize the widget based on the number of lines in the textwidget and set colors
         self.resize()
+        self.set_colors()
 
         # Delete all the old line numbers
         self.delete("all")
 
-        # Get the first and last line numbers for the editor (all other lines are in between)
+        # Get the first and last line numbers for the textwidget (all other lines are in between)
         first_line, last_line = int(self.textwidget.index("@0,0").split(".")[0]), int(
             self.textwidget.index(f"@0,{self.textwidget.winfo_height()}").split(".")[0]
         )
 
         # Draw the line numbers looping through the lines
         for lineno in range(first_line, last_line + 1):
+            # Check if line is elided
+            tags: list = self.textwidget.tag_names(f"{lineno}.0")
+            elide_values: tuple = (
+                self.textwidget.tag_cget(tag, "elide") for tag in tags
+            )
+            # elide values can be empty
+            line_elided: bool = any(getboolean(v or "false") for v in elide_values)
 
             # If the line is not visible, skip it
-            if (dlineinfo := self.textwidget.dlineinfo(f"{lineno}.0")) is None:
+            if (
+                dlineinfo := self.textwidget.dlineinfo(f"{lineno}.0")
+            ) is None or line_elided:
                 continue
 
             # Create the line number
             self.create_text(
                 0
                 if self.justify == "left"
                 else int(self["width"])
                 if self.justify == "right"
                 else int(self["width"]) / 2,
                 dlineinfo[1],
                 text=f" {lineno} " if self.justify != "center" else f"{lineno}",
                 anchor={"left": "nw", "right": "ne", "center": "n"}[self.justify],
                 font=self.textwidget.cget("font"),
-                fill=self.foreground,
+                fill=self.foreground_color,
             )
 
     def mouse_scroll(self, event: Event) -> None:
         """Scrolls the text widget when the mouse wheel is scrolled -- Internal use only"""
-        if system == "Darwin":
-            self.textwidget.yview_scroll(scroll_inversion(event.delta), "units")
-        else:
-            self.textwidget.yview_scroll(int(scroll_inversion(event.delta)), "units")
+
+        # Scroll the text widget and then redraw the widget
+        self.textwidget.yview_scroll(
+            int(scroll_fix(event.delta if event.delta else event.num)), "units"
+        )
+        self.redraw()
 
     def click_see(self, event: Event) -> None:
         """When clicking on a line number it scrolls to that line if not shifting -- Internal use only"""
 
         # If the shift key is down, redirect to self.shift_click()
         if event.state == 1:
             self.shift_click(event)
             return
 
-        #Remove the selection tag from the text widget
+        # Remove the selection tag from the text widget
         self.textwidget.tag_remove("sel", "1.0", "end")
 
+        [line, _] = self.textwidget.index(f"@{event.x},{event.y}").split(".")
+        click_pos = f"{line}.0"
+
         # Set the insert position to the line number clicked
-        self.textwidget.mark_set(
-            "insert",
-            f"{self.textwidget.index(f'@{event.x},{event.y}').split('.')[0]}.0",
-        )
+        self.textwidget.mark_set("insert", click_pos)
 
         # Scroll to the location of the insert position
         self.textwidget.see("insert")
 
-        # If the line clicked is at the edge of the screen, scroll by one line to bring it into view
-        first_visible_line, last_visible_line = int(self.textwidget.index("@0,0").split(".")[0]), int(
-            self.textwidget.index(f"@0,{self.textwidget.winfo_height()}").split(".")[0]
-        )
-        if (insert := int(self.textwidget.index("insert").split(".")[0])) == first_visible_line:
-            self.textwidget.yview_scroll(-1, "units")
-        elif insert == last_visible_line:
-            self.textwidget.yview_scroll(1, "units")
-        self.click_pos = self.textwidget.index("insert")
+        self.click_pos: str = click_pos
+        self.redraw()
 
-    def unclick(self, event: Event) -> None:
-        """When the mouse button is released the click position is None -- Internal use only"""
-        self.click_pos: None = None
+    def unclick(self, _: Event) -> None:
+        """When the mouse button is released it removes the selection -- Internal use only"""
+
+        self.click_pos = None
 
-    def double_click(self, event: Event) -> None:
+    def double_click(self, _: Event) -> None:
         """Selects the line when double clicked -- Internal use only"""
-        # Add the selection tag to the line double clicked
+
+        # Remove the selection tag from the text widget and select the line
         self.textwidget.tag_remove("sel", "1.0", "end")
         self.textwidget.tag_add("sel", "insert", "insert + 1 line")
+        self.redraw()
 
-    def auto_scroll(self, event: Event) -> None:
-        """Automatically scrolls the text widget when the mouse is near the top or bottom, similar to the drag function -- Internal use only"""
+    def mouse_off_screen_scroll(self, event: Event) -> None:
+        """Automatically scrolls the text widget when the mouse is near the top or bottom,
+        similar to the in_widget_select_mouse_drag function -- Internal use only"""
+
+        self.x = event.x
+        self.y = event.y
+        self.text_auto_scan(event)
 
-        # If the mouse is not down, return
+    def text_auto_scan(self, event):
         if self.click_pos is None:
             return
 
         # Taken from the Text source: https://github.com/tcltk/tk/blob/main/library/text.tcl#L676
         # Scrolls the widget if the cursor is off of the screen
-        if event.y >= self.winfo_height():
-            self.textwidget.yview_scroll(1 if system == "Darwin" else (1 / 120), "units")
-        elif event.y < 0:
-            self.textwidget.yview_scroll(-1 if system == "Darwin" else (-1 / 120), "units")
+        if self.y >= self.winfo_height():
+            self.textwidget.yview_scroll(1 + self.y - self.winfo_height(), "pixels")
+        elif self.y < 0:
+            self.textwidget.yview_scroll(-1 + self.y, "pixels")
+        elif self.x >= self.winfo_width():
+            self.textwidget.xview_scroll(2, "units")
+        elif self.x < 0:
+            self.textwidget.xview_scroll(-2, "units")
         else:
             return
 
-        #  Set the selection tag and insert position
-        start, end = self.textwidget.index("insert"), self.click_pos
-        if self.textwidget.compare("insert", ">", self.click_pos):
-            start, end = end, str(float(start) + 1)
-        else:
-            end = str(float(end) + 1)
-        self.textwidget.tag_remove("sel", "1.0", "end")
-        self.textwidget.tag_add("sel", start, end)
-        self.textwidget.mark_set("insert", f"@{event.x},{event.y}")
+        # Select the text
+        self.select_text(self.x - self.winfo_width(), self.y)
+
+        # After 50ms, call this function again
+        self.cancellable_after = self.after(50, self.text_auto_scan, event)
+        self.redraw()
 
-        # Call the function recursively using the after method with a delay of 50 milliseconds
-        # Also stolen from the Text source: https://github.com/tcltk/tk/blob/main/library/text.tcl#L704
-        self.after(50, self.auto_scroll, event)
-
-    def drag(self, event: Event) -> None:
-        """When click dragging it selects the text -- Internal use only"""
-
-        # If the mouse is not down or outside of the widget, return
-        if (
-            self.click_pos is None
-            or event.x < 0
-            or event.x >= self.winfo_width()
-            or event.y < 0
-            or event.y >= self.winfo_height()
-        ):
+    def stop_mouse_off_screen_scroll(self, _: Event) -> None:
+        """Stops the auto scroll when the cursor re-enters the line numbers -- Internal use only"""
+
+        # If the after has not been cancelled, cancel it
+        if self.cancellable_after is not None:
+            self.after_cancel(self.cancellable_after)
+            self.cancellable_after: None = None
+
+    def check_side_scroll(self, event: Event) -> None:
+        """Detects if the mouse is off the screen to the sides \
+(a case not covered in mouse_off_screen_scroll) -- Internal use only"""
+
+        # Determine if the mouse is off the sides of the widget
+        off_side = (
+            event.x < self.winfo_x() or event.x > self.winfo_x() + self.winfo_width()
+        )
+        if not off_side:
             return
 
-        # Set the selection tag and insert position
-        start, end = self.textwidget.index("insert"), self.click_pos
-        if self.textwidget.compare("insert", ">", self.click_pos):
-            start, end = end, str(float(start) + 1)
+        # Determine if its above or below the widget
+        if event.y >= self.winfo_height():
+            self.textwidget.yview_scroll(1, "units")
+        elif event.y < 0:
+            self.textwidget.yview_scroll(-1, "units")
         else:
-            end = str(float(end) + 1)
+            return
 
-        self.textwidget.tag_remove("sel", "1.0", "end")
-        self.textwidget.tag_add("sel", start.split(".")[0] + ".0", end.split(".")[0] + ".0")
-        self.textwidget.mark_set("insert", self.textwidget.index(f"@{event.x},{event.y} linestart + 1 line"))
+        # Select the text
+        self.select_text(event.x - self.winfo_width(), event.y)
 
         # Redraw the widget
         self.redraw()
 
+    def in_widget_select_mouse_drag(self, event: Event) -> None:
+        """When click in_widget_select_mouse_dragging it selects the text -- Internal use only"""
+
+        # If the click position is None, return
+        if self.click_pos is None:
+            return
+
+        self.x = event.x
+        self.y = event.y
+
+        # Select the text
+        self.select_text(event.x - self.winfo_width(), event.y)
+        self.redraw()
+
+    def select_text(self, x, y) -> None:
+        """Selects the text between the start and end positions -- Internal use only"""
+
+        drag_pos = self.textwidget.index(f"@{x}, {y}")
+        if self.textwidget.compare(drag_pos, ">", self.click_pos):
+            start = self.click_pos
+            end = drag_pos
+        else:
+            start = drag_pos
+            end = self.click_pos
+
+        self.textwidget.tag_remove("sel", "1.0", "end")
+        self.textwidget.tag_add("sel", start, end)
+        self.textwidget.mark_set("insert", drag_pos)
+
     def shift_click(self, event: Event) -> None:
         """When shift clicking it selects the text between the click and the cursor -- Internal use only"""
 
         # Add the selection tag to the text between the click and the cursor
-        start_pos, end_pos = self.textwidget.index("insert"), self.textwidget.index(f"@0,{event.y}")
+        start_pos: str = self.textwidget.index("insert")
+        end_pos: str = self.textwidget.index(f"@0,{event.y}")
         self.textwidget.tag_remove("sel", "1.0", "end")
         if self.textwidget.compare(start_pos, ">", end_pos):
             start_pos, end_pos = end_pos, start_pos
         self.textwidget.tag_add("sel", start_pos, end_pos)
+        self.redraw()
 
     def resize(self) -> None:
-        """Resizes the widget to fit the text widget"""
+        """Resizes the widget to fit the text widget -- Internal use only"""
 
         # Get amount of lines in the text widget
         end = self.textwidget.index("end").split(".")[0]
 
         # Set the width of the widget to the required width to display the biggest line number
-        self.config(width=Font(font=(temp_font := self.textwidget.cget("font"))).measure(" 1234 ")) if int(
+        temp_font = self.textwidget.cget("font")
+        self.config(width=Font(font=temp_font).measure(" 1234 ")) if int(
             end
         ) <= 1000 else self.config(width=temp_font.measure(f" {end} "))
 
-    def set_to_ttk_style(self) -> None:
-        """Sets the widget to the ttk style"""
+    def set_colors(self, _: Event | None = None) -> None:
+        """Sets the colors of the widget according to self.colors - Internal use only"""
 
-        # Set the background and foreground to the ttk style
-        self["bg"] = self.tk.eval("ttk::style lookup TLineNumbers -background")
-        self.foreground = self.tk.eval("ttk::style lookup TLineNumbers -foreground")
-
-    def reload(self) -> None:
-        """Reloads the widget"""
-        self.set_to_ttk_style()
-        self.redraw()
+        # If the color provider is None, set the foreground color to the Text widget's foreground color
+        if self.colors is None:
+            self.foreground_color = self.textwidget["fg"]
+            self["bg"] = self.textwidget["bg"]
+        elif isinstance(self.colors, tuple):
+            self.foreground_color, self["bg"] = self.colors
+        else:
+            self.foreground_color, self["bg"] = self.colors()
 
 
 if __name__ == "__main__":
-    import platform
-    from tkinter import Text, Tk
-    from tkinter.font import Font
+    from tkinter import Tk
     from tkinter.ttk import Style
 
-    system = str(platform.system())
-
-    if system == "Darwin":
-        contmand = "Command"
-    else:
-        contmand = "Control"
-
     root = Tk()
 
     style = Style()
-    style.configure("TLineNumbers", background="#ffffff", foreground="#2197db")
+    style.configure("TkLineNumbers", foreground="#2197db", background="#ffffff")
 
-    text = Text(root, wrap="char", font=("Courier New bold", 15))
+    text = Text(root)
     text.pack(side="right")
-    text.focus()
 
-    for i in range(500):
+    for i in range(50):
         text.insert("end", f"Line {i+1}\n")
 
-    linenums = TkLineNumbers(root, text)
+    def ttk_theme_colors() -> tuple[str, str]:
+        fg: str = style.lookup("TkLineNumbers", "foreground", default="black")
+        bg: str = style.lookup("TkLineNumbers", "background", default="white")
+        return (fg, bg)
+
+    linenums = TkLineNumbers(root, text, colors=ttk_theme_colors)
     linenums.pack(fill="y", side="left", expand=True)
 
-    text.bind("<Key>", lambda event: root.after_idle(linenums.redraw), add=True)
-    text.bind(f"<BackSpace>", lambda event: root.after_idle(linenums.redraw), add=True)
-    text.bind(f"<{contmand}-v>", lambda event: root.after_idle(linenums.redraw), add=True)
+    text.bind("<<Modified>>", lambda _: linenums.redraw())
     text.config(font=("Courier New bold", 15))
 
     root.mainloop()
```

### Comparing `tklinenums-1.6.5/tklinenums.egg-info/PKG-INFO` & `tklinenums-1.7.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: tklinenums
-Version: 1.6.5
-Summary: A simple Tkinter widget for displaying line numbers
-Home-page: https://github.com/Moosems/TkLineNums
-Author: Moosems
-Author-email: moosems.j@gmail.com
-Description-Content-Type: text/markdown
-
 <h1 align="center">TkLineNums</h1>
 
 > **Note**
 > If Python was installed via Homebrew, installed on Mac by default, or installed on Linux, tkinter will likely not work properly and may need to be installed via `brew install python-tk` or with the distro package manager on Linux as documented [here](https://tecadmin.net/how-to-install-python-tkinter-on-linux/).
 
 ## Description
 `TkLineNums` is a simple line numbering widget for Python's `tkinter` GUI library. It is directly connects to a `Text` widget and even supports ttk themes through the set_to_ttk_style method.
@@ -18,73 +9,63 @@
 ![img](https://github.com/Moosems/TkLineNums/raw/main/images/TkLineNumsPhoto.png)
 
 ## Features of the `TkLineNums` widget:
 
 - Clicking on line numbers will set the insert to the beginning of the line.
 - Shift clicking will select all text from the end of the line clicked by cursor and the insert position.
 - Scrolling the linebar will scroll the text widget (and vice versa).
-- Supports ttk themes (by usage of the `.set_to_ttk_style()` method)
-- Supports left, right, and center alignment with the `-justify` option
-- Clicking and then dragging the mouse will scroll the text widget (see [#8](https://github.com/Moosems/TkLineNums/pull/8))
+- Can handle elided lines (elided lines are lines that are not visible in the text widget).
+- Supports ttk themes and allows easy color customization.
+- Supports left, right, and center alignment with the `-justify` option.
+- Clicking and then dragging the mouse will scroll the text widget (see [#8](https://github.com/Moosems/TkLineNums/pull/8)).
 
 # Installation
-`pip install tklinenums`
+
+In the Command Line, paste the following: `pip install tklinenums`.
 
 ## Documentation
 ### `TkLineNums` Widget
 |Options|Description|Type|
 |---|---|---|
 |master|The parent widget|Tkinter widget (defaults to `tkinter.Misc`)|
-|editor|The `Text` widget the line numbers will connect to|Tkinter `Text` widget (or child class)|
+|textwidget|The `Text` widget the line numbers will connect to|Tkinter `Text` widget (or child class)|
 |justify|The alignment of the line numbers|A string as either `"left"`, `"right"`, or `"center"`|
+|colors|A way to provide coloring to the line numbers|A function, `(foreground, background)` tuple, or None. None (default) makes it use the `Text` widget's coloring. The function should return a `(foreground, background)` tuple: it will be called whenever the colors are needed, and it is useful when the colors can change.|
 |*args|Arguments for the `Canvas` widget|Any arguments used for the `Canvas` widget|
 |**kwargs|Keyword arguments for the `Canvas` widget|Any keyword arguments used for the `Canvas` widget|
 
 ### Basic Usage:
 ```python
-from platform import system
 from tkinter import Text, Tk
 from tkinter.ttk import Style
 
 from tklinenums import TkLineNumbers
 
-# This is to make the example work on both Windows and Mac
-if system() == "Darwin":
-    contmand: str = "Command"
-else:
-    contmand: str = "Control"
-
 # Create the root window
 root = Tk()
 
-# Set the ttk style (tkinter's way of styling) for the line numbers
-style = Style()
-style.configure("TLineNumbers", background="#ffffff", foreground="#2197db")
-
 # Create the Text widget and pack it to the right
 text = Text(root)
 text.pack(side="right")
 
 # Insert 50 lines of text into the Text widget
 for i in range(50):
     text.insert("end", f"Line {i+1}\n")
 
 # Create the TkLineNumbers widget and pack it to the left
-linenums = TkLineNumbers(root, text)
+linenums = TkLineNumbers(root, text, justify="center", colors=("#2197db", "#ffffff"))
 linenums.pack(fill="y", side="left")
 
-# Create binds to redraw the line numbers for most common events that change the text in the Text widget
-text.bind("<Key>", lambda event: root.after_idle(linenums.redraw), add=True)
-text.bind("<BackSpace>", lambda event: root.after_idle(linenums.redraw), add=True)
-text.bind(f"<{contmand}-v>", lambda event: root.after_idle(linenums.redraw), add=True)
+# Redraw the line numbers when the text widget contents are modified
+text.bind("<<Modified>>", lambda event: root.after_idle(linenums.redraw), add=True)
 
 # Start the mainloop for the root window
 root.mainloop()
 ```
-For a more complete example, see the [example.py](./tests/example.py) file.
+For a more complete example, see [example.py](./tests/example.py).
 
 ## How to run and contribute
 
 ### Running
 
 To run the example, run `python3 tests/example.py` in the root directory. The project uses only standard library modules, so there are no dependencies. It will create a window with a `Text` widget and a `TkLineNumbers` widget and 50 lines of text to mess around with.
```

