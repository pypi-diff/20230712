# Comparing `tmp/colored-2.2.2.tar.gz` & `tmp/colored-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colored-2.2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "colored-2.2.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `colored-2.2.2.tar` & `colored-2.2.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     3007 2023-06-26 14:22:25.000000 colored-2.2.2/README.md
--rw-r--r--   0        0        0      374 2023-06-26 14:22:25.000000 colored-2.2.2/colored/__init__.py
--rw-r--r--   0        0        0     1999 2023-06-26 14:22:25.000000 colored-2.2.2/colored/attributes.py
--rw-r--r--   0        0        0     1774 2023-06-26 14:22:25.000000 colored-2.2.2/colored/background.py
--rw-r--r--   0        0        0    10378 2023-06-26 14:22:25.000000 colored-2.2.2/colored/colored.py
--rw-r--r--   0        0        0     1873 2023-06-26 14:22:25.000000 colored-2.2.2/colored/controls.py
--rw-r--r--   0        0        0     1574 2023-06-26 14:22:25.000000 colored-2.2.2/colored/cprint.py
--rw-r--r--   0        0        0     1086 2023-06-26 14:22:25.000000 colored-2.2.2/colored/exceptions.py
--rw-r--r--   0        0        0     1742 2023-06-26 14:22:25.000000 colored-2.2.2/colored/foreground.py
--rw-r--r--   0        0        0     1853 2023-06-26 14:22:25.000000 colored-2.2.2/colored/hexadecimal.py
--rw-r--r--   0        0        0    15757 2023-06-26 14:22:25.000000 colored-2.2.2/colored/library.py
--rw-r--r--   0        0        0     4006 2023-06-26 14:22:25.000000 colored-2.2.2/colored/utilities.py
--rw-r--r--   0        0        0     1067 2023-06-26 14:22:25.000000 colored-2.2.2/pyproject.toml
--rw-r--r--   0        0        0     3857 1970-01-01 00:00:00.000000 colored-2.2.2/PKG-INFO
+-rw-r--r--   0        0        0     2728 2023-07-12 17:46:20.000000 colored-2.2.3/README.md
+-rw-r--r--   0        0        0      374 2023-07-12 17:46:20.000000 colored-2.2.3/colored/__init__.py
+-rw-r--r--   0        0        0     1999 2023-07-12 17:46:20.000000 colored-2.2.3/colored/attributes.py
+-rw-r--r--   0        0        0     1774 2023-07-12 17:46:20.000000 colored-2.2.3/colored/background.py
+-rw-r--r--   0        0        0    10377 2023-07-12 17:46:20.000000 colored-2.2.3/colored/colored.py
+-rw-r--r--   0        0        0     1873 2023-07-12 17:46:20.000000 colored-2.2.3/colored/controls.py
+-rw-r--r--   0        0        0     1574 2023-07-12 17:46:20.000000 colored-2.2.3/colored/cprint.py
+-rw-r--r--   0        0        0     1086 2023-07-12 17:46:20.000000 colored-2.2.3/colored/exceptions.py
+-rw-r--r--   0        0        0     1742 2023-07-12 17:46:20.000000 colored-2.2.3/colored/foreground.py
+-rw-r--r--   0        0        0     1853 2023-07-12 17:46:20.000000 colored-2.2.3/colored/hexadecimal.py
+-rw-r--r--   0        0        0    15757 2023-07-12 17:46:20.000000 colored-2.2.3/colored/library.py
+-rw-r--r--   0        0        0     4006 2023-07-12 17:46:20.000000 colored-2.2.3/colored/utilities.py
+-rw-r--r--   0        0        0     1067 2023-07-12 17:46:20.000000 colored-2.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3578 1970-01-01 00:00:00.000000 colored-2.2.3/PKG-INFO
```

### Comparing `colored-2.2.2/README.md` & `colored-2.2.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,17 +6,14 @@
 Colored, it's a simple Python library for color and formatting in terminal.
 Collection of color codes and names for 256 color terminal setups. 
 Colored now supports RGB color mode. As "true color" graphic cards with 16 to <a href="https://en.wikipedia.org/wiki/ANSI_escape_code#24-bit" target="_blank">24 bits</a> of color became common, 
 applications began to support 24-bit colors. Terminal emulators supporting setting 24-bit foreground and background 
 colors with escape sequences include Xterm, KDE's <a href="https://en.wikipedia.org/wiki/Konsole" target="_blank">Konsole</a>, and iTerm, as well as all libvte based terminals,
 including <a href="https://en.wikipedia.org/wiki/GNOME_Terminal" target="_blank">GNOME Terminal</a>.
 
-A list of [256 colors](https://dslackw.gitlab.io/colored/tables/colors/#full-chart-256-foreground-and-background-colors)
-for <a href="https://en.wikipedia.org/wiki/Xterm" target="_blank">Xterm</a>, containing an example of the displayed color, Xterm Name, Xterm Number and HEX.
-
 The colors work with most terminals and terminals emulators.
 <a href="https://en.wikipedia.org/wiki/ANSI_escape_code" target="_blank">ANSI/VT100 escape sequences</a> can be used in every programming languages.
 
 Colored is powerful and easy to use:
 
 ```python title="Python 3.9.17"
 >>> from colored import Fore, Back, Style
```

#### html2text {}

```diff
@@ -1,20 +1,17 @@
 [https://gitlab.com/dslackw/colored/-/raw/site/docs/images/colored.png] ##
 About Colored, it's a simple Python library for color and formatting in
 terminal. Collection of color codes and names for 256 color terminal setups.
 Colored now supports RGB color mode. As "true color" graphic cards with 16 to
 24_bits of color became common, applications began to support 24-bit colors.
 Terminal emulators supporting setting 24-bit foreground and background colors
 with escape sequences include Xterm, KDE's Konsole, and iTerm, as well as all
-libvte based terminals, including GNOME_Terminal. A list of [256 colors](https:
-//dslackw.gitlab.io/colored/tables/colors/#full-chart-256-foreground-and-
-background-colors) for Xterm, containing an example of the displayed color,
-Xterm Name, Xterm Number and HEX. The colors work with most terminals and
-terminals emulators. ANSI/VT100_escape_sequences can be used in every
-programming languages. Colored is powerful and easy to use: ```python
+libvte based terminals, including GNOME_Terminal. The colors work with most
+terminals and terminals emulators. ANSI/VT100_escape_sequences can be used in
+every programming languages. Colored is powerful and easy to use: ```python
 title="Python 3.9.17" >>> from colored import Fore, Back, Style >>> >>>
 Fore.red '\x1b[38;5;1m' >>> >>> Back.red '\x1b[48;5;1m' >>> >>> Style.reset
 '\x1b[0m' >>> >>> Fore.rgb('100%', '50%', '30%') '\x1b[38;2;255;130;79m' >>>
 >>> print(f'{Fore.white}{Back.green}Colored is Awesome!!!{Style.reset}') ```
 !!! success
 >>>  Colored is Awesome!!!
 ## Installing Open up a terminal and install colored with pip command: ```bash
```

### Comparing `colored-2.2.2/colored/attributes.py` & `colored-2.2.3/colored/attributes.py`

 * *Files identical despite different names*

### Comparing `colored-2.2.2/colored/background.py` & `colored-2.2.3/colored/background.py`

 * *Files identical despite different names*

### Comparing `colored-2.2.2/colored/colored.py` & `colored-2.2.3/colored/colored.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,15 @@
         mode = wintypes.DWORD(0)
         ok = windll.kernel32.GetConsoleMode(wintypes.HANDLE(hStdout), byref(mode))
         if not ok:
             _win_vterm_mode = False
             return
 
         mode = wintypes.DWORD(mode.value | ENABLE_VIRTUAL_TERMINAL_PROCESSING)
-        ok = windll.kernel32.SetsConsoleMode(wintypes.HANDLE(hStdout), mode)
+        ok = windll.kernel32.SetConsoleMode(wintypes.HANDLE(hStdout), mode)
         if not ok:
             # Something went wrong, probably a version too old
             # to support the VT100 mode.
             # To be more certain we could check kernel32.GetLastError
             # for STATUS_INVALID_PARAMETER, but since we only enable
             # one flag we can be certain enough.
             _win_vterm_mode = False
```

### Comparing `colored-2.2.2/colored/controls.py` & `colored-2.2.3/colored/controls.py`

 * *Files identical despite different names*

### Comparing `colored-2.2.2/colored/cprint.py` & `colored-2.2.3/colored/cprint.py`

 * *Files identical despite different names*

### Comparing `colored-2.2.2/colored/exceptions.py` & `colored-2.2.3/colored/exceptions.py`

 * *Files identical despite different names*

### Comparing `colored-2.2.2/colored/foreground.py` & `colored-2.2.3/colored/foreground.py`

 * *Files identical despite different names*

### Comparing `colored-2.2.2/colored/hexadecimal.py` & `colored-2.2.3/colored/hexadecimal.py`

 * *Files identical despite different names*

### Comparing `colored-2.2.2/colored/library.py` & `colored-2.2.3/colored/library.py`

 * *Files identical despite different names*

### Comparing `colored-2.2.2/colored/utilities.py` & `colored-2.2.3/colored/utilities.py`

 * *Files identical despite different names*

### Comparing `colored-2.2.2/pyproject.toml` & `colored-2.2.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core>=3.2.0,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "colored"
-version = "2.2.2"
+version = "2.2.3"
 authors = [
     {name = "Dimitris Zlatanidis", email = "dslackw@gmail.com"},
 ]
 description = "Simple python library for color and formatting to terminal"
 readme = "README.md"
 requires-python = ">=3.9"
 keywords = [
```

### Comparing `colored-2.2.2/PKG-INFO` & `colored-2.2.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colored
-Version: 2.2.2
+Version: 2.2.3
 Summary: Simple python library for color and formatting to terminal
 Keywords: xterm,color,colour,vt100,ansi,terminal,text,rgb,linux,windows
 Author-email: Dimitris Zlatanidis <dslackw@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -26,17 +26,14 @@
 Colored, it's a simple Python library for color and formatting in terminal.
 Collection of color codes and names for 256 color terminal setups. 
 Colored now supports RGB color mode. As "true color" graphic cards with 16 to <a href="https://en.wikipedia.org/wiki/ANSI_escape_code#24-bit" target="_blank">24 bits</a> of color became common, 
 applications began to support 24-bit colors. Terminal emulators supporting setting 24-bit foreground and background 
 colors with escape sequences include Xterm, KDE's <a href="https://en.wikipedia.org/wiki/Konsole" target="_blank">Konsole</a>, and iTerm, as well as all libvte based terminals,
 including <a href="https://en.wikipedia.org/wiki/GNOME_Terminal" target="_blank">GNOME Terminal</a>.
 
-A list of [256 colors](https://dslackw.gitlab.io/colored/tables/colors/#full-chart-256-foreground-and-background-colors)
-for <a href="https://en.wikipedia.org/wiki/Xterm" target="_blank">Xterm</a>, containing an example of the displayed color, Xterm Name, Xterm Number and HEX.
-
 The colors work with most terminals and terminals emulators.
 <a href="https://en.wikipedia.org/wiki/ANSI_escape_code" target="_blank">ANSI/VT100 escape sequences</a> can be used in every programming languages.
 
 Colored is powerful and easy to use:
 
 ```python title="Python 3.9.17"
 >>> from colored import Fore, Back, Style
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: colored Version: 2.2.2 Summary: Simple python
+Metadata-Version: 2.1 Name: colored Version: 2.2.3 Summary: Simple python
 library for color and formatting to terminal Keywords:
 xterm,color,colour,vt100,ansi,terminal,text,rgb,linux,windows Author-email:
 Dimitris Zlatanidis
 gmail.com> Requires-Python: >=3.9 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Console Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: POSIX :: Other Classifier: Operating System :: POSIX ::
@@ -13,25 +13,22 @@
 dslackw.gitlab.io/colored/ [https://gitlab.com/dslackw/colored/-/raw/site/docs/
 images/colored.png] ## About Colored, it's a simple Python library for color
 and formatting in terminal. Collection of color codes and names for 256 color
 terminal setups. Colored now supports RGB color mode. As "true color" graphic
 cards with 16 to 24_bits of color became common, applications began to support
 24-bit colors. Terminal emulators supporting setting 24-bit foreground and
 background colors with escape sequences include Xterm, KDE's Konsole, and
-iTerm, as well as all libvte based terminals, including GNOME_Terminal. A list
-of [256 colors](https://dslackw.gitlab.io/colored/tables/colors/#full-chart-
-256-foreground-and-background-colors) for Xterm, containing an example of the
-displayed color, Xterm Name, Xterm Number and HEX. The colors work with most
-terminals and terminals emulators. ANSI/VT100_escape_sequences can be used in
-every programming languages. Colored is powerful and easy to use: ```python
-title="Python 3.9.17" >>> from colored import Fore, Back, Style >>> >>>
-Fore.red '\x1b[38;5;1m' >>> >>> Back.red '\x1b[48;5;1m' >>> >>> Style.reset
-'\x1b[0m' >>> >>> Fore.rgb('100%', '50%', '30%') '\x1b[38;2;255;130;79m' >>>
->>> print(f'{Fore.white}{Back.green}Colored is Awesome!!!{Style.reset}') ```
-!!! success
+iTerm, as well as all libvte based terminals, including GNOME_Terminal. The
+colors work with most terminals and terminals emulators. ANSI/VT100_escape
+sequences can be used in every programming languages. Colored is powerful and
+easy to use: ```python title="Python 3.9.17" >>> from colored import Fore,
+Back, Style >>> >>> Fore.red '\x1b[38;5;1m' >>> >>> Back.red '\x1b[48;5;1m' >>>
+>>> Style.reset '\x1b[0m' >>> >>> Fore.rgb('100%', '50%', '30%') '\x1b
+[38;2;255;130;79m' >>> >>> print(f'{Fore.white}{Back.green}Colored is
+Awesome!!!{Style.reset}') ``` !!! success
 >>>  Colored is Awesome!!!
 ## Installing Open up a terminal and install colored with pip command: ```bash
 $ pip install colored ``` Alternatively, you can grab the latest source code
 from GitLab: ```bash $ git clone https://gitlab.com/dslackw/colored.git $ cd
 colored $ pip install . ``` ## Usage The [User Guide](https://
 dslackw.gitlab.io/colored/user_guide/user_guide/#user-guide) is the place to go
 to learn how to use the library. The [API Reference](https://dslackw.gitlab.io/
```

