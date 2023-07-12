# Comparing `tmp/jigsawwm-1.2.1.tar.gz` & `tmp/jigsawwm-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jigsawwm-1.2.1.tar", last modified: Wed Apr  5 06:52:04 2023, max compression
+gzip compressed data, was "jigsawwm-2.0.0.tar", last modified: Wed Jul 12 11:04:32 2023, max compression
```

## Comparing `jigsawwm-1.2.1.tar` & `jigsawwm-2.0.0.tar`

### file list

```diff
@@ -1,46 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-04-05 06:52:04.428669 jigsawwm-1.2.1/
--rw-rw-rw-   0        0        0     7815 2023-03-04 03:31:55.000000 jigsawwm-1.2.1/LICENSE
--rw-rw-rw-   0        0        0       29 2023-04-05 06:10:39.000000 jigsawwm-1.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0     6909 2023-04-05 06:52:04.427667 jigsawwm-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     6106 2023-04-05 06:45:52.000000 jigsawwm-1.2.1/README.md
--rw-rw-rw-   0        0        0      851 2023-04-05 06:41:17.000000 jigsawwm-1.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       58 2023-04-05 03:25:51.000000 jigsawwm-1.2.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-05 06:52:04.428669 jigsawwm-1.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-05 06:52:04.390501 jigsawwm-1.2.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-05 06:52:04.402557 jigsawwm-1.2.1/src/jigsawwm/
--rw-rw-rw-   0        0        0        0 2023-02-08 14:52:01.000000 jigsawwm-1.2.1/src/jigsawwm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:52:04.416592 jigsawwm-1.2.1/src/jigsawwm/assets/
--rw-rw-rw-   0        0        0      460 2023-01-10 02:38:42.000000 jigsawwm-1.2.1/src/jigsawwm/assets/dwindle.png
--rw-rw-rw-   0        0        0     5948 2023-01-10 02:38:42.000000 jigsawwm-1.2.1/src/jigsawwm/assets/icons.svg
--rw-rw-rw-   0        0        0     1411 2023-01-10 02:38:42.000000 jigsawwm-1.2.1/src/jigsawwm/assets/logo.png
--rw-rw-rw-   0        0        0      638 2023-01-10 02:38:42.000000 jigsawwm-1.2.1/src/jigsawwm/assets/obs.png
--rw-rw-rw-   0        0        0      611 2023-01-10 02:38:42.000000 jigsawwm-1.2.1/src/jigsawwm/assets/wide-dwindle.png
--rw-rw-rw-   0        0        0     7280 2023-04-05 05:40:39.000000 jigsawwm-1.2.1/src/jigsawwm/daemon.py
--rw-rw-rw-   0        0        0     7786 2023-04-05 04:05:34.000000 jigsawwm-1.2.1/src/jigsawwm/hotkey.py
--rw-rw-rw-   0        0        0    23226 2023-02-27 15:04:05.000000 jigsawwm-1.2.1/src/jigsawwm/manager.py
--rw-rw-rw-   0        0        0     4552 2023-04-05 06:17:12.000000 jigsawwm-1.2.1/src/jigsawwm/services.py
--rw-rw-rw-   0        0        0     3342 2023-04-05 03:52:28.000000 jigsawwm-1.2.1/src/jigsawwm/smartstart.py
--rw-rw-rw-   0        0        0     2199 2023-04-04 04:10:13.000000 jigsawwm-1.2.1/src/jigsawwm/state.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:52:04.418592 jigsawwm-1.2.1/src/jigsawwm/tiler/
--rw-rw-rw-   0        0        0        0 2023-02-08 14:55:06.000000 jigsawwm-1.2.1/src/jigsawwm/tiler/__init__.py
--rw-rw-rw-   0        0        0     3800 2023-02-15 15:35:07.000000 jigsawwm-1.2.1/src/jigsawwm/tiler/layouts.py
--rw-rw-rw-   0        0        0     4757 2023-02-15 15:35:03.000000 jigsawwm-1.2.1/src/jigsawwm/tiler/tilers.py
--rw-rw-rw-   0        0        0     2526 2023-01-10 02:38:42.000000 jigsawwm-1.2.1/src/jigsawwm/virtdeskstub.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:52:04.426668 jigsawwm-1.2.1/src/jigsawwm/w32/
--rw-rw-rw-   0        0        0        0 2023-01-10 02:38:42.000000 jigsawwm-1.2.1/src/jigsawwm/w32/__init__.py
--rw-rw-rw-   0        0        0    10263 2023-02-15 15:35:48.000000 jigsawwm-1.2.1/src/jigsawwm/w32/hook.py
--rw-rw-rw-   0        0        0     6444 2023-02-15 15:56:30.000000 jigsawwm-1.2.1/src/jigsawwm/w32/idesktopwallpaper.py
--rw-rw-rw-   0        0        0     2748 2023-02-15 15:58:24.000000 jigsawwm-1.2.1/src/jigsawwm/w32/ivirtualdesktopmanager.py
--rw-rw-rw-   0        0        0     6358 2023-02-16 14:34:35.000000 jigsawwm-1.2.1/src/jigsawwm/w32/monitor.py
--rw-rw-rw-   0        0        0     3628 2023-04-04 08:49:42.000000 jigsawwm-1.2.1/src/jigsawwm/w32/process.py
--rw-rw-rw-   0        0        0     2674 2023-02-16 14:38:01.000000 jigsawwm-1.2.1/src/jigsawwm/w32/sendinput.py
--rw-rw-rw-   0        0        0     8152 2023-02-16 14:39:01.000000 jigsawwm-1.2.1/src/jigsawwm/w32/vk.py
--rw-rw-rw-   0        0        0    15820 2023-02-16 14:52:19.000000 jigsawwm-1.2.1/src/jigsawwm/w32/window.py
--rw-rw-rw-   0        0        0     3835 2023-01-10 02:38:42.000000 jigsawwm-1.2.1/src/jigsawwm/w32/window_structs.py
--rw-rw-rw-   0        0        0     4152 2023-01-10 02:38:42.000000 jigsawwm-1.2.1/src/jigsawwm/w32/winevent.py
-drwxrwxrwx   0        0        0        0 2023-04-05 06:52:04.412072 jigsawwm-1.2.1/src/jigsawwm.egg-info/
--rw-rw-rw-   0        0        0     6909 2023-04-05 06:52:04.000000 jigsawwm-1.2.1/src/jigsawwm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1019 2023-04-05 06:52:04.000000 jigsawwm-1.2.1/src/jigsawwm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-05 06:52:04.000000 jigsawwm-1.2.1/src/jigsawwm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-04-05 06:52:04.000000 jigsawwm-1.2.1/src/jigsawwm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-05 06:52:04.000000 jigsawwm-1.2.1/src/jigsawwm.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-12 11:04:32.142297 jigsawwm-2.0.0/
+-rw-rw-rw-   0        0        0     7815 2023-03-04 03:31:55.000000 jigsawwm-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0       29 2023-04-05 06:10:39.000000 jigsawwm-2.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     8884 2023-07-12 11:04:32.142297 jigsawwm-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7864 2023-07-12 10:59:07.000000 jigsawwm-2.0.0/README.md
+-rw-rw-rw-   0        0        0     1068 2023-07-12 10:59:36.000000 jigsawwm-2.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       37 2023-07-12 10:44:04.000000 jigsawwm-2.0.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 11:04:32.143295 jigsawwm-2.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-12 11:04:32.088541 jigsawwm-2.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-12 11:04:32.100766 jigsawwm-2.0.0/src/jigsawwm/
+-rw-rw-rw-   0        0        0        0 2023-02-08 14:52:01.000000 jigsawwm-2.0.0/src/jigsawwm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 11:04:32.124775 jigsawwm-2.0.0/src/jigsawwm/assets/
+-rw-rw-rw-   0        0        0      460 2023-01-10 02:38:42.000000 jigsawwm-2.0.0/src/jigsawwm/assets/dwindle.png
+-rw-rw-rw-   0        0        0     5948 2023-01-10 02:38:42.000000 jigsawwm-2.0.0/src/jigsawwm/assets/icons.svg
+-rw-rw-rw-   0        0        0     1411 2023-01-10 02:38:42.000000 jigsawwm-2.0.0/src/jigsawwm/assets/logo.png
+-rw-rw-rw-   0        0        0      638 2023-01-10 02:38:42.000000 jigsawwm-2.0.0/src/jigsawwm/assets/obs.png
+-rw-rw-rw-   0        0        0      611 2023-01-10 02:38:42.000000 jigsawwm-2.0.0/src/jigsawwm/assets/wide-dwindle.png
+-rw-rw-rw-   0        0        0      947 2023-07-12 10:41:40.000000 jigsawwm-2.0.0/src/jigsawwm/chrome.py
+-rw-rw-rw-   0        0        0     6116 2023-07-12 10:41:40.000000 jigsawwm-2.0.0/src/jigsawwm/daemon.py
+drwxrwxrwx   0        0        0        0 2023-07-12 11:04:32.127775 jigsawwm-2.0.0/src/jigsawwm/jmk/
+-rw-rw-rw-   0        0        0      458 2023-07-12 10:41:40.000000 jigsawwm-2.0.0/src/jigsawwm/jmk/__init__.py
+-rw-rw-rw-   0        0        0    12075 2023-07-12 10:41:40.000000 jigsawwm-2.0.0/src/jigsawwm/jmk/core.py
+-rw-rw-rw-   0        0        0     3836 2023-07-12 10:41:40.000000 jigsawwm-2.0.0/src/jigsawwm/jmk/hotkey.py
+-rw-rw-rw-   0        0        0     6689 2023-07-12 10:41:40.000000 jigsawwm-2.0.0/src/jigsawwm/jmk/sysinout.py
+-rw-rw-rw-   0        0        0      786 2023-07-12 10:41:40.000000 jigsawwm-2.0.0/src/jigsawwm/smartstart.py
+-rw-rw-rw-   0        0        0     2199 2023-04-04 04:10:13.000000 jigsawwm-2.0.0/src/jigsawwm/state.py
+drwxrwxrwx   0        0        0        0 2023-07-12 11:04:32.130298 jigsawwm-2.0.0/src/jigsawwm/tiler/
+-rw-rw-rw-   0        0        0        0 2023-02-08 14:55:06.000000 jigsawwm-2.0.0/src/jigsawwm/tiler/__init__.py
+-rw-rw-rw-   0        0        0     4248 2023-07-12 10:41:40.000000 jigsawwm-2.0.0/src/jigsawwm/tiler/layouts.py
+-rw-rw-rw-   0        0        0     4910 2023-07-12 10:41:40.000000 jigsawwm-2.0.0/src/jigsawwm/tiler/tilers.py
+-rw-rw-rw-   0        0        0     2526 2023-01-10 02:38:42.000000 jigsawwm-2.0.0/src/jigsawwm/virtdeskstub.py
+drwxrwxrwx   0        0        0        0 2023-07-12 11:04:32.139294 jigsawwm-2.0.0/src/jigsawwm/w32/
+-rw-rw-rw-   0        0        0       38 2023-07-12 10:41:40.000000 jigsawwm-2.0.0/src/jigsawwm/w32/__init__.py
+-rw-rw-rw-   0        0        0     9552 2023-07-12 10:41:40.000000 jigsawwm-2.0.0/src/jigsawwm/w32/hook.py
+-rw-rw-rw-   0        0        0     6444 2023-02-15 15:56:30.000000 jigsawwm-2.0.0/src/jigsawwm/w32/idesktopwallpaper.py
+-rw-rw-rw-   0        0        0     2748 2023-02-15 15:58:24.000000 jigsawwm-2.0.0/src/jigsawwm/w32/ivirtualdesktopmanager.py
+-rw-rw-rw-   0        0        0     6358 2023-02-16 14:34:35.000000 jigsawwm-2.0.0/src/jigsawwm/w32/monitor.py
+-rw-rw-rw-   0        0        0     3628 2023-04-23 15:10:37.000000 jigsawwm-2.0.0/src/jigsawwm/w32/process.py
+-rw-rw-rw-   0        0        0     7893 2023-07-12 10:41:40.000000 jigsawwm-2.0.0/src/jigsawwm/w32/sendinput.py
+-rw-rw-rw-   0        0        0    11294 2023-07-12 10:41:40.000000 jigsawwm-2.0.0/src/jigsawwm/w32/vk.py
+-rw-rw-rw-   0        0        0    16293 2023-07-12 10:41:40.000000 jigsawwm-2.0.0/src/jigsawwm/w32/window.py
+-rw-rw-rw-   0        0        0     3835 2023-01-10 02:38:42.000000 jigsawwm-2.0.0/src/jigsawwm/w32/window_structs.py
+-rw-rw-rw-   0        0        0     4152 2023-01-10 02:38:42.000000 jigsawwm-2.0.0/src/jigsawwm/w32/winevent.py
+-rw-rw-rw-   0        0        0    25772 2023-07-12 10:41:40.000000 jigsawwm-2.0.0/src/jigsawwm/wm.py
+drwxrwxrwx   0        0        0        0 2023-07-12 11:04:32.120774 jigsawwm-2.0.0/src/jigsawwm.egg-info/
+-rw-rw-rw-   0        0        0     8884 2023-07-12 11:04:32.000000 jigsawwm-2.0.0/src/jigsawwm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1147 2023-07-12 11:04:32.000000 jigsawwm-2.0.0/src/jigsawwm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 11:04:32.000000 jigsawwm-2.0.0/src/jigsawwm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-07-12 11:04:32.000000 jigsawwm-2.0.0/src/jigsawwm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-12 11:04:32.000000 jigsawwm-2.0.0/src/jigsawwm.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-12 11:04:32.141297 jigsawwm-2.0.0/tests/
+-rw-rw-rw-   0        0        0     3715 2023-07-12 10:41:40.000000 jigsawwm-2.0.0/tests/test_jmk_core.py
+-rw-rw-rw-   0        0        0     1038 2023-07-12 10:41:40.000000 jigsawwm-2.0.0/tests/test_jmk_hotkey.py
```

### Comparing `jigsawwm-1.2.1/LICENSE` & `jigsawwm-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jigsawwm-1.2.1/PKG-INFO` & `jigsawwm-2.0.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: jigsawwm
-Version: 1.2.1
-Summary: JigsawWM is a dynamic window manager for Windows10/11 just like the suckless dwm for the X
+Version: 2.0.0
+Summary: JigsawWM is a free and open-source project that aims to increase your productivity by offering a set of automation facilities, including the jmk module as an AHK alternative, a Tiling Window Manager to free you from managing windows manually and the Daemon to support any customization you may have in mind.
 Author-email: Klesh Wong <klesh@qq.com>
 Project-URL: Documentation, https://jigsawwm.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/klesh/JigsawWM
 Project-URL: Issue Tracker, https://github.com/klesh/JigsawWM/issues
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
@@ -14,178 +14,212 @@
 Classifier: Operating System :: POSIX :: BSD
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # JigsawWM
 
-JigsawWM is a dynamic window manager for Windows10/11 just like the suckless dwm for the X.
-JigsawWM is a free and open-source project that aims to increase your productivity.
+JigsawWM is a free and open-source project that aims to increase your productivity by offering a set of automation facilities, including the jmk module as an AHK alternative, a Tiling Window Manager to free you from managing windows manually and the Daemon to support any customization you may have in mind.
 
-## Demo
+# What Can I Do?
 
-https://user-images.githubusercontent.com/61080/210168366-e70dd649-f6ef-41bb-a8e5-941e392d770a.mp4
+## Service: jmk
+Software-defined keyboard/mouse automation which mimics the [QMK](https://qmk.fm) as an alternative to [AutoHotkey](https://autohotkey.com)
 
-## Installation
+1. My pinky is hurting - the dual-role key
+You should try using `F` as the `Control` key, the following code would turn it into a dual-role key: it acts as the `LControl` when held, `F` when tapped:
+```
+        Vk.F: JmkTapHold(tap=Vk.F, hold=Vk.LCONTROL),
+```
+What if I need to enter a bunch of `F`?
+Tap it and then hold it down within `quick_tap_term`(default 120ms)
+
+2. I use F12 a lot, can I tap it without looking at the keyboard? - the layers
+Sure, the problem with modern keyboards is they are enormous, 104 or even more. It is inconvenient when the keys you use frequently are far away from the Home Row (`a`, `s`, `d`, `f`, ...). With `layer` you may "move" the needed key into your reach:
+```
+layers = [
+    { # layer 0
+        # activate layer 3 when held
+        Vk.T: JmkTapHold(tap=Vk.T, hold=3),
+    },
+    { # layer 1
+      ...
+    },
+    { # layer 2
+      ...
+    },
+    { # layer 3
+        Vk.Z: JmkKey(Vk.F1),
+    }
+```
+Now, hold the key `T` and press `Z`, you get `F1`
 
-Tested on **Windows 11 Build 22000** and **Python 3.11.1**.
-Should work on **Windows 10** and **Python 3.8**
+3. I would like to press `Win+Q` to close the active Window.
+`hotkey` at your service, furthermore, you may press `Win+N` to minimize or `Win+M` to maximize the active window
+```python
+hotkeys = [
+    ("Win+q", "LAlt+F4"),
+    # Win+n to minimize active window
+    ([Vk.WIN, Vk.N], minimize_active_window),
+    # Win+m to maximize active window
+    ([Vk.WIN, Vk.M], toggle_maximize_active_window),
+]
+```
 
+4. For browsing smoothingly with the Mouse, try the following setup
+- `Mouse Forward + Left Button`: send `Ctrl + w` (close tab in Chrome and other apps)
+- `Mouse Forward + Wheel Up`: send `Ctrl + PageUp` (previous tab in Chrome and other apps)
+- `Mouse Forward + Wheel Down`: send `Ctrl + PageDown` (next tab in Chrome and other apps)
 
-Install from pypi
-```
-pip install jigsawwm
-```
+5. Check out the [examples/jmk.pyw](example/jmk.pyw) to find out more
 
-Install from github repo
-```
-pip install git+https://github.com/klesh/JigsawWM.git
-```
 
-## Quick Start
+## Service: tiling window manager
 
-**JigsawWm** follows the [suckless philosophy](https://suckless.org/philosophy/) and works just like [dwm - dynamic window manager | suckless.org software that sucks less](https://dwm.suckless.org/). All windows are treated as a `Ordered List`, they will be moved into places based on their `Order` and specified `Layout` **automatically** to improve your productivity.
+The **WindowManager** follows the [suckless philosophy](https://suckless.org/philosophy/) and works just like the [dwm](https://dwm.suckless.org/). All windows are treated as an `Ordered List`, they will be moved into places based on their `Order` and specified `Layout` **automatically**, save you from arranging them manually.
 
+### Demo
 
-### Step 1: Create a `.pyw` file as the "Configuration"
+https://user-images.githubusercontent.com/61080/210168366-e70dd649-f6ef-41bb-a8e5-941e392d770a.mp4
+
+### Default keybindings
 
-1. Download the [example.pyw](src/example.pyw) to your local hard drive
-2. Edit the code as you see fit
-3. Double-click the file and it should launch with a tray icon, or you may have to create a file association to the `Python` program
-4. Create a shortcut in your `Startup` folder if you like it
-
-### Step 2: Using hotkeys to manage your windows
-
-- `Win + j`: activate next window and move cursor to its center
-- `Win + k`: activate previous window and move cursor to its center
-- `Win + Shift + j`: move active window down in the list / swap with the next one
-- `Win + Shift + k`: move active window up in the list / swap with the previous one
-- `Win + n`: minimized active window
-- `Win + m`: maximize/unmaximized active window
-- `Win + /`: swap active window with **first window** in the list or **second window** if it is the first window already
-- `Win + q`: kill active window
+- `Win + j`: activate next window and move the cursor to its center
+- `Win + k`: activate the previous window and move the cursor to its center
+- `Win + Shift + j`: move the active window down in the list (swap with the next one) 
+- `Win + Shift + k`: move the active window up in the list (swap with the previous one)
+- `Win + /`: swap the active window with **the first window** in the list or **the second window** if it is the first window already
 - `Win + Space`: next theme, `Theme` consists of `Layout`, `Background`, `gap`, etc. to determine how windows should be placed
-- `Win + i`: activate first window of the next monitor if any or move cursor only
-- `Win + u`: activate first window of the previous monitor if any or move cursor only
-- `Win + Shift + i`: move active window to next monitor
-- `Win + Shift + u`: move active window to previous monitor
-- `Win + Control + i`: inspect active window
+- `Win + i`: activate the first window of the next monitor if any or move cursor only
+- `Win + u`: activate the first window of the previous monitor if any or move cursor only
+- `Win + Shift + i`: move the active window to the next monitor
+- `Win + Shift + u`: move the active window to the previous monitor
 
-### Step 3: Launch at startup
+## Service: run console program in the background
 
-1. Open your **Startup** folder by pressing `Win + r` to activate the **Run** dialog and type in `shell:startup`, a FileExplorer should pop up.
-2. Create a shortcut to your `.pyw` file. Done!
+Sometimes, software that should be run as a system service may not offer an installer to do the job, worse, it may ship as a Console Program. Nobody wants a Console Window stays on their desktops, and yes, I'm talking about [SyncThing](https://syncthing.net/). I love it but I would like it to run in the background quietly.
+
+```py
+class SyncthingService(daemon.ProcessService):
+    name = "syncthing"
+    args = [
+        r"C:\Programs\syncthing-windows-amd64-v1.23.2\syncthing.exe",
+        "-no-browser",
+        "-no-restart",
+        "-no-upgrade",
+    ]
+    log_path = r"C:\Programs\syncthing-windows-amd64-v1.23.2\syncthing.log"
 
 
-## Useful features:
+daemon.register(SyncthingService)
+```
 
-### Services
 
-To run a console program (e.g. syncthing) in the background as a service
+## Task: automate your workflows with tasks
 
+1. I would like to open a folder inside the Chromium Bookmark on the first boot-up every day.
 ```python
-from jigsawwm.daemon import Daemon
+class DailyRoutine(daemon.Task):
+    name = "daily routine"
 
-class MyDaemon(Daemon):
-    def setup(self):
-        from jigsawwm.services import ServiceEntry, register_service
-        register_service(
-            ServiceEntry(
-                name="syncthing",
-                args=[
-                    r"C:\Programs\syncthing-windows-amd64-v1.23.2\syncthing.exe",
-                    "-no-browser",
-                    "-no-restart",
-                    "-no-upgrade",
-                ],
-                log_path=r"C:\Programs\syncthing-windows-amd64-v1.23.2\syncthing.log",
-            )
-        )
+    def run(self):
+        chrome.open_fav_folder("bookmark_bar", "daily")
 
-MyDaemon(Daemon)
-```
+    def condition(self):
+        # trigger only once on daily-basis
+        return smartstart.daily_once("daily websites")
 
-### Smart Start
 
-To launch apps/tasks at login conditionally
+daemon.register(DailyRoutine)
+```
 
-1. What if I would like a folder named `daily` in my Chrome Bookmark Bar to be opened automatically on my first boot-up every day?
+2. I would like to launch my IM / Mail Client on workdays
 ```python
-from jigsawwm.daemon import Daemon
+class WorkdayRoutine(daemon.Task):
+    name = "workday routine"
 
-class MyDaemon(Daemon):
-    def setup(self):
-        from jigsawwm.smartstart import (
-            SmartStartEntry,
-            daily_once,
-            open_chrome_fav_folder,
-            register_smartstart,
+    def __init__(self) -> None:
+        super().__init__()
+        self.holiday_book = ChinaHolidayBook()
+
+    def run(self):
+        smartstart.start_if_not_running(
+            r"C:\Users\Klesh\AppData\Local\Feishu\Feishu.exe"
         )
-        register_smartstart(
-            SmartStartEntry(
-                name="daily routine",
-                launch=lambda: open_chrome_fav_folder("bookmark_bar", "daily"),
-                condition=lambda: daily_once("daily websites"),
-            )
+        smartstart.start_if_not_running(
+            r"C:\Program Files\Mozilla Thunderbird\thunderbird.exe"
         )
 
-MyDaemon(Daemon)
+    def condition(self):
+        return self.holiday_book.is_workhour(extend=timedelta(hours=2))
+
+
+daemon.register(WorkdayRoutine)
 ```
-2. What if I would like a couple of apps to be launched when I boot up the computer within work hours?
-```python
 
-        holiday_book = ChinaHolidayBook()
 
-        def open_worklog():
-            """Open worklog (a markdown file) for today (create if it doesn't exist yet)."""
-            next_workday = holiday_book.next_workday()
-            latest_workday = holiday_book.latest_workday()
-            worklog_path = os.path.join(
-                os.path.expanduser("~/Documents/Sync/worklog"),
-                f"{next_workday.isoformat()}.md",
-            )
-            if not os.path.exists(worklog_path):
-                with open(worklog_path, "w") as f:
-                    prevdate = latest_workday.strftime("%m/%d")
-                    nextdate = next_workday.strftime("%m/%d")
-                    f.write(f"{prevdate}\n1. \n\n{nextdate}\n1. ")
-            os.startfile(worklog_path)
-
-        register_smartstart(
-            SmartStartEntry(
-                name="workhour routine",
-                launch=[
-                    r"C:\Users\Klesh\AppData\Local\Feishu\Feishu.exe",
-                    r"C:\Program Files\Mozilla Thunderbird\thunderbird.exe",
-                    open_worklog,
-                ],
-                # in case I might boot up the computer a little bit earlier
-                condition=lambda: holiday_book.is_workhour(extend=timedelta(hours=2)),
-            )
-        )
+# Installation
+
+Tested on **Windows 11 Build 22000** and **Python 3.11.1**.
+Should work on **Windows 10** and **Python 3.8**
+
+
+Install from pypi
+```
+pip install jigsawwm
+```
 
+Install from Github repo
 ```
+pip install git+https://github.com/klesh/JigsawWM.git
+```
+
+## Quick Start
 
-### Tray menu
 
-![tray menu](docs/img/tray_menu.png)
 
-Functionalities:
+### Step 1: Create a `.pyw` file as your "Configuration"
 
-1. Stop/start a `service` 
-2. Run a `smartstart` without condition
+Choose services you like from the [examples](examples) folder, you may use any of the following directly.
+
+- [examples/jmk.pyw](examples/jmk.pyw) if you are looking for a QMK/AutoHotkey alternative
+- [examples/services.pyw](examples/services.pyw) if you are trying to run some Console Program as Service in the background
+- [examples/tasks.pyw](examples/tasks.pyw) if you are looking for a solution to automate your workflow smartly on startup
+- [examples/wm.pyw](examples/wm.pyw) if you are looking for a tiling window manager
+- [examples/jigsaw.pyw](examples/wm.pyw) the whole package of the above
+
+### Step 2: Launch your `.pyw` file and manage your services
+
+Double-click the `.pyw` file and a tray icon should appear, right-click the icon to manage your services.
+![image](https://github.com/klesh/JigsawWM/assets/61080/dd6b0c05-19eb-4a55-a7b6-8c66afff09b9)
+
+
+### Step 3: Launch at startup
+
+1. Open your **Startup** folder by pressing `Win + r` to activate the **Run** dialog and type in `shell:startup`, a FileExplorer should pop up.
+2. Create a shortcut to your `.pyw` file. Done!
 
 
 ## Document
 
 [Read the Docs](https://jigsawwm.readthedocs.io/en/latest/)
 
 
 ## Changelog
 
+### 2023-07-12 (v2.0)
+
+- refactor: divided features into multiple services to allow users to use only what they need
+- feat: replace the `hotkey` module with the `jmk` module, which mimics the basic functionality
+  of [QMK](https://qmk.fm/) as an alternative to [AutoHotkey](https://www.autohotkey.com/)
+
+### 2023-04-07
+
+- hotkey support mouse buttons, forward/backward buttons as modifier
+
 ### 2023-04-05
 
 - add `smartstart` feature
 - BREAKING CHANGE: rename `svcmgr` to `services`
 - adopt `pyproject.toml`
 
 ### 2023-03-21
```

### Comparing `jigsawwm-1.2.1/src/jigsawwm/assets/icons.svg` & `jigsawwm-2.0.0/src/jigsawwm/assets/icons.svg`

 * *Files identical despite different names*

### Comparing `jigsawwm-1.2.1/src/jigsawwm/assets/logo.png` & `jigsawwm-2.0.0/src/jigsawwm/assets/logo.png`

 * *Files identical despite different names*

### Comparing `jigsawwm-1.2.1/src/jigsawwm/assets/obs.png` & `jigsawwm-2.0.0/src/jigsawwm/assets/obs.png`

 * *Files identical despite different names*

### Comparing `jigsawwm-1.2.1/src/jigsawwm/assets/wide-dwindle.png` & `jigsawwm-2.0.0/src/jigsawwm/assets/wide-dwindle.png`

 * *Files identical despite different names*

### Comparing `jigsawwm-1.2.1/src/jigsawwm/manager.py` & `jigsawwm-2.0.0/src/jigsawwm/wm.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,40 @@
 from dataclasses import dataclass
+from datetime import datetime
 from os import path
 from typing import Dict, List, Optional, Set
 
 from jigsawwm.tiler.tilers import *
 from jigsawwm.virtdeskstub import find_or_create_virtdeskstub
+from jigsawwm.w32 import hook
 from jigsawwm.w32.idesktopwallpaper import desktop_wallpaper
 from jigsawwm.w32.ivirtualdesktopmanager import GUID, virtual_desktop_manager
 from jigsawwm.w32.monitor import (
     Monitor,
     get_monitor_from_cursor,
     get_monitor_from_window,
     get_monitors,
     get_topo_sorted_monitors,
     set_cursor_pos,
 )
 from jigsawwm.w32.window import (
+    DWORD,
     HWND,
+    LONG,
     RECT,
     Window,
     get_active_window,
     get_first_app_window,
     get_foreground_window,
     get_manageable_windows,
+    is_app_window,
+    is_window,
     sprint_window,
 )
+from jigsawwm.w32.winevent import WinEvent
 
 
 @dataclass
 class Theme:
     """Theme is a set of preference packed together for users to switch easily,
     typically, it consists of a LayoutTiler, Background, Gap between windows and
     other options.
@@ -42,17 +49,18 @@
     # unused
     icon_path: Optional[str] = None
     # background, color if the string starts with `#`, otherwise treated as image path
     background: Optional[str] = None
     # new appeared window would be prepended to the list if the option was set to True
     new_window_as_master: Optional[bool] = None
     # gap between windows / monitor edges
-    gap: Optional[int] = None
+    gap: Optional[int] = 0
     # forbid
     strict: Optional[bool] = None
+    hook_ids: List[int] = None
 
 
 class MonitorState:
     """MonitorState holds variables needed by a Monitor
 
 
     :param VirtDeskState virtdesk_state: associated virtual desktop
@@ -73,14 +81,15 @@
         theme: Optional[str] = None,
     ):
         self.virtdesk_state = virtdesk_state
         self.monitor = monitor
         self.theme = theme
         self.windows = []
         self.last_active_window = None
+        self.hook_ids = []
 
     def get_theme(self) -> Theme:
         """Retrieves theme for monitor in current virtual desktop"""
         mgr = self.virtdesk_state.manager
         return mgr.themes[mgr.get_theme_index(self.theme)]
 
     def get_existing_windows(self) -> List[Window]:
@@ -258,19 +267,21 @@
     :param ignore_exe_names: list of executable filenames that you don't want them
                              to be managed/arranged
     """
 
     _state: Dict[GUID, VirtDeskState]
     themes: List[Theme]
     ignore_exe_names: Set[str]
+    force_managed_exe_names: Set[str]
 
     def __init__(
         self,
         themes: List[Theme] = None,
         ignore_exe_names: Set[str] = None,
+        force_managed_exe_names: Set[str] = None,
     ):
         self._state = {}
         self.themes = themes or [
             Theme(
                 name="WideScreen Dwindle",
                 layout_tiler=widescreen_dwindle_layout_tiler,
                 icon_name="wide-dwindle.png",
@@ -283,14 +294,15 @@
             Theme(
                 name="Dwindle",
                 layout_tiler=dwindle_layout_tiler,
                 icon_name="dwindle.png",
             ),
         ]
         self.ignore_exe_names = set(ignore_exe_names or [])
+        self.force_managed_exe_names = set(force_managed_exe_names or [])
         self.theme = self.themes[0].name
         self.sync(init=True)
 
     def try_get_virtdesk_state(
         self, hwnd: Optional[HWND] = None
     ) -> Optional[VirtDeskState]:
         """Retrieve virtual desktop state without exception.
@@ -330,17 +342,24 @@
             proc.kill()
         return virtdesk_state
 
     def is_ignored(self, window: Window) -> bool:
         exepath = window.exe
         return not exepath or path.basename(exepath) in self.ignore_exe_names
 
+    def is_force_managed(self, hwnd: HWND) -> bool:
+        try:
+            exepath = Window(hwnd).exe
+            return exepath and path.basename(exepath) in self.force_managed_exe_names
+        except:
+            return False
+
     def sync(self, init=False, restrict=False) -> bool:
         """Update manager state(monitors, windows) to match OS's and arrange windows if it is changed"""
-        manageable_windows = list(get_manageable_windows())
+        manageable_windows = list(get_manageable_windows(self.is_force_managed))
         if not manageable_windows:
             return
         virtdesk_state = self.try_get_virtdesk_state(manageable_windows[0].handle)
         if not virtdesk_state:
             return
         # gather all manageable windows and group them by monitor
         group_wins_by_mons: Dict[Monitor, Set[Window]] = {}
@@ -591,13 +610,73 @@
         """Move active window to previous monitor"""
         self.move_to_monitor_by_offset(-1)
 
     def move_to_next_monitor(self):
         """Move active window to next monitor"""
         self.move_to_monitor_by_offset(+1)
 
+    def _winevent_callback(
+        self,
+        event: WinEvent,
+        hwnd: HWND,
+        id_obj: LONG,
+        id_chd: LONG,
+        id_evt_thread: DWORD,
+        evt_time: DWORD,
+    ):
+        if (
+            id_obj
+            or id_chd
+            or not is_window(hwnd)
+            or not is_app_window(hwnd)
+            or self.is_ignored(Window(hwnd))
+        ):
+            return
+        print(
+            "[{now}] {event:30s} {hwnd:8d} {title}".format(
+                now=datetime.now().strftime("%M:%S.%f"),
+                event=event.name,
+                hwnd=hwnd,
+                #  ido: {id_obj:6d} idc: {id_chd:6d}
+                # id_obj=id_obj,
+                # id_chd=id_chd,
+                title=Window(hwnd).title,
+            )
+        )
+        self.sync(restrict=event == WinEvent.EVENT_SYSTEM_MOVESIZEEND)
+
+    def install_hooks(self):
+        """Install hooks for window events"""
+        self.hook_ids = [
+            hook.hook_winevent(
+                WinEvent.EVENT_OBJECT_SHOW,
+                WinEvent.EVENT_OBJECT_HIDE,
+                self._winevent_callback,
+            ),
+            hook.hook_winevent(
+                WinEvent.EVENT_OBJECT_CLOAKED,
+                WinEvent.EVENT_OBJECT_UNCLOAKED,
+                self._winevent_callback,
+            ),
+            hook.hook_winevent(
+                WinEvent.EVENT_SYSTEM_MINIMIZESTART,
+                WinEvent.EVENT_SYSTEM_MINIMIZEEND,
+                self._winevent_callback,
+            ),
+            hook.hook_winevent(
+                WinEvent.EVENT_SYSTEM_MOVESIZEEND,
+                WinEvent.EVENT_SYSTEM_MOVESIZEEND,
+                self._winevent_callback,
+            ),
+        ]
+
+    def uninstall_hooks(self):
+        for hook_id in self.hook_ids:
+            hook.unhook_winevent(hook_id)
+        self.hook_ids = []
+
 
 if __name__ == "__main__":
     wm = WindowManager()
     wm.sync()
     print()
     wm.sync()
```

### Comparing `jigsawwm-1.2.1/src/jigsawwm/state.py` & `jigsawwm-2.0.0/src/jigsawwm/state.py`

 * *Files identical despite different names*

### Comparing `jigsawwm-1.2.1/src/jigsawwm/tiler/layouts.py` & `jigsawwm-2.0.0/src/jigsawwm/tiler/layouts.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,36 @@
 # FloatRect holds relative coordinate for rectangle (left/top/right/bottom)
 FloatRect = Tuple[float, float, float, float]
 
 # Layout accepts an integer (total number of windows) and return a FloatRect generator
 Layout = Callable[[int], Iterator[FloatRect]]
 
 
+def mono(n: int) -> Iterator[FloatRect]:
+    """The mono Layout
+
+    .. code-block:: text
+
+        +-----------+
+        |           |
+        |           |
+        |           |
+        |     1     |
+        |           |
+        |           |
+        |           |
+        +-----------+
+
+    :param n: total number of windows
+    :rtype: Iterator[FloatRect]
+    """
+    for i in range(n):
+        yield 0.0, 0.0, 1.0, 1.0
+
+
 def dwindle(n: int) -> Iterator[FloatRect]:
     """The dwindle Layout
 
     .. code-block:: text
 
         +-----------+-----------+
         |           |           |
```

### Comparing `jigsawwm-1.2.1/src/jigsawwm/tiler/tilers.py` & `jigsawwm-2.0.0/src/jigsawwm/tiler/tilers.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ``Tiler`` is a generator which generates Rects with specified Layout for given monitor work area and total number of windows
 
 ``LayoutTiler`` is similar to `Tiler` except the Layout was predefined
 
 """
 from typing import Callable, Iterator, Tuple
 
-from .layouts import Layout, dwindle, plug_rect, widescreen_dwindle
+from .layouts import Layout, dwindle, mono, plug_rect, widescreen_dwindle
 
 # Rect holds physical coordinate for rectangle (left/top/right/bottom)
 Rect = Tuple[int, int, int, int]
 
 # Tiler generates physical Rects for specified total number of windows based on given Layout
 Tiler = Callable[[Layout, Rect, int], Iterator[Rect]]
 
@@ -89,14 +89,19 @@
     yield fr, wt + obs_height, wr, wb
     if total_windows == 2:
         return
     obs_rect = (fr, wt, wr, wt + obs_height)
     yield from direct_tiler(layout, obs_rect, total_windows - 2)
 
 
+def mono_layout_tiler(*args, **kwargs) -> Iterator[Rect]:
+    """The dwindle layout tiler"""
+    return direct_tiler(mono, *args, **kwargs)
+
+
 def dwindle_layout_tiler(*args, **kwargs) -> Iterator[Rect]:
     """The dwindle layout tiler"""
     return direct_tiler(dwindle, *args, **kwargs)
 
 
 def widescreen_dwindle_layout_tiler(*args, **kwargs) -> Iterator[Rect]:
     """The wide-screen dwindle layout tiler"""
```

### Comparing `jigsawwm-1.2.1/src/jigsawwm/virtdeskstub.py` & `jigsawwm-2.0.0/src/jigsawwm/virtdeskstub.py`

 * *Files identical despite different names*

### Comparing `jigsawwm-1.2.1/src/jigsawwm/w32/idesktopwallpaper.py` & `jigsawwm-2.0.0/src/jigsawwm/w32/idesktopwallpaper.py`

 * *Files identical despite different names*

### Comparing `jigsawwm-1.2.1/src/jigsawwm/w32/ivirtualdesktopmanager.py` & `jigsawwm-2.0.0/src/jigsawwm/w32/ivirtualdesktopmanager.py`

 * *Files identical despite different names*

### Comparing `jigsawwm-1.2.1/src/jigsawwm/w32/monitor.py` & `jigsawwm-2.0.0/src/jigsawwm/w32/monitor.py`

 * *Files identical despite different names*

### Comparing `jigsawwm-1.2.1/src/jigsawwm/w32/process.py` & `jigsawwm-2.0.0/src/jigsawwm/w32/process.py`

 * *Files identical despite different names*

### Comparing `jigsawwm-1.2.1/src/jigsawwm/w32/window.py` & `jigsawwm-2.0.0/src/jigsawwm/w32/window.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,20 +133,25 @@
     return bool(
         not is_window_cloaked(hwnd)
         and WindowStyle.SIZEBOX in style
         and not process.is_elevated(get_window_pid(hwnd))
     )
 
 
-def is_manageable_window(hwnd: HWND) -> bool:
+def is_manageable_window(
+    hwnd: HWND,
+    is_force_managed: Optional[Callable[[HWND], bool]] = None,
+) -> bool:
     """Check if window is able to be managed by us"""
+    is_force_managed = is_force_managed or (lambda hwnd: False)
+    #  or is_force_managed(hwnd)
     style = get_window_style(hwnd)
     return bool(
         is_app_window(hwnd, style)
-        and get_window_title(hwnd)
+        and (get_window_title(hwnd) or is_force_managed(hwnd))
         and WindowStyle.MAXIMIZEBOX & style
         and WindowStyle.MINIMIZEBOX & style
         and WindowStyle.VISIBLE in style
         and not WindowStyle.MINIMIZE & style
     )
 
 
@@ -369,21 +374,23 @@
             lambda hwnd: EnumCheckResult.CAPTURE
             if is_app_window(hwnd)
             else EnumCheckResult.SKIP
         ),
     )
 
 
-def get_manageable_windows() -> Iterator[Window]:
+def get_manageable_windows(
+    is_force_managed: Optional[Callable[[HWND], bool]] = None,
+) -> Iterator[Window]:
     """Get all manageable windows of specified/current desktop"""
     return map(
         Window,
         enum_windows(
             lambda hwnd: EnumCheckResult.CAPTURE
-            if is_manageable_window(hwnd)
+            if is_manageable_window(hwnd, is_force_managed)
             else EnumCheckResult.SKIP
         ),
     )
 
 
 def get_active_window() -> Optional[Window]:
     """Retrieves current activated window"""
@@ -489,14 +496,17 @@
             exstyle_flags.append(s.name)
     print("exstyle      :", ", ".join(exstyle_flags), file=file)
     print("is_cloaked   :", window.is_cloaked, file=file)
     rect = window.get_rect()
     print("rect         :", rect.left, rect.top, rect.right, rect.bottom, file=file)
     bound = window.get_extended_frame_bounds()
     print("bound        :", bound.left, bound.top, bound.right, bound.bottom, file=file)
+    print("is_app_window:", is_app_window(hwnd), file=file)
+    print("is_manageable:", is_manageable_window(hwnd), file=file)
+    print("is_evelated  :", window.is_evelated, file=file)
 
 
 def inspect_active_window():
     text = sprint_window(get_foreground_window())
     messagebox.showinfo("JigsawWM", text)
```

### Comparing `jigsawwm-1.2.1/src/jigsawwm/w32/window_structs.py` & `jigsawwm-2.0.0/src/jigsawwm/w32/window_structs.py`

 * *Files identical despite different names*

### Comparing `jigsawwm-1.2.1/src/jigsawwm/w32/winevent.py` & `jigsawwm-2.0.0/src/jigsawwm/w32/winevent.py`

 * *Files identical despite different names*

### Comparing `jigsawwm-1.2.1/src/jigsawwm.egg-info/PKG-INFO` & `jigsawwm-2.0.0/src/jigsawwm.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: jigsawwm
-Version: 1.2.1
-Summary: JigsawWM is a dynamic window manager for Windows10/11 just like the suckless dwm for the X
+Version: 2.0.0
+Summary: JigsawWM is a free and open-source project that aims to increase your productivity by offering a set of automation facilities, including the jmk module as an AHK alternative, a Tiling Window Manager to free you from managing windows manually and the Daemon to support any customization you may have in mind.
 Author-email: Klesh Wong <klesh@qq.com>
 Project-URL: Documentation, https://jigsawwm.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/klesh/JigsawWM
 Project-URL: Issue Tracker, https://github.com/klesh/JigsawWM/issues
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
@@ -14,178 +14,212 @@
 Classifier: Operating System :: POSIX :: BSD
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # JigsawWM
 
-JigsawWM is a dynamic window manager for Windows10/11 just like the suckless dwm for the X.
-JigsawWM is a free and open-source project that aims to increase your productivity.
+JigsawWM is a free and open-source project that aims to increase your productivity by offering a set of automation facilities, including the jmk module as an AHK alternative, a Tiling Window Manager to free you from managing windows manually and the Daemon to support any customization you may have in mind.
 
-## Demo
+# What Can I Do?
 
-https://user-images.githubusercontent.com/61080/210168366-e70dd649-f6ef-41bb-a8e5-941e392d770a.mp4
+## Service: jmk
+Software-defined keyboard/mouse automation which mimics the [QMK](https://qmk.fm) as an alternative to [AutoHotkey](https://autohotkey.com)
 
-## Installation
+1. My pinky is hurting - the dual-role key
+You should try using `F` as the `Control` key, the following code would turn it into a dual-role key: it acts as the `LControl` when held, `F` when tapped:
+```
+        Vk.F: JmkTapHold(tap=Vk.F, hold=Vk.LCONTROL),
+```
+What if I need to enter a bunch of `F`?
+Tap it and then hold it down within `quick_tap_term`(default 120ms)
+
+2. I use F12 a lot, can I tap it without looking at the keyboard? - the layers
+Sure, the problem with modern keyboards is they are enormous, 104 or even more. It is inconvenient when the keys you use frequently are far away from the Home Row (`a`, `s`, `d`, `f`, ...). With `layer` you may "move" the needed key into your reach:
+```
+layers = [
+    { # layer 0
+        # activate layer 3 when held
+        Vk.T: JmkTapHold(tap=Vk.T, hold=3),
+    },
+    { # layer 1
+      ...
+    },
+    { # layer 2
+      ...
+    },
+    { # layer 3
+        Vk.Z: JmkKey(Vk.F1),
+    }
+```
+Now, hold the key `T` and press `Z`, you get `F1`
 
-Tested on **Windows 11 Build 22000** and **Python 3.11.1**.
-Should work on **Windows 10** and **Python 3.8**
+3. I would like to press `Win+Q` to close the active Window.
+`hotkey` at your service, furthermore, you may press `Win+N` to minimize or `Win+M` to maximize the active window
+```python
+hotkeys = [
+    ("Win+q", "LAlt+F4"),
+    # Win+n to minimize active window
+    ([Vk.WIN, Vk.N], minimize_active_window),
+    # Win+m to maximize active window
+    ([Vk.WIN, Vk.M], toggle_maximize_active_window),
+]
+```
 
+4. For browsing smoothingly with the Mouse, try the following setup
+- `Mouse Forward + Left Button`: send `Ctrl + w` (close tab in Chrome and other apps)
+- `Mouse Forward + Wheel Up`: send `Ctrl + PageUp` (previous tab in Chrome and other apps)
+- `Mouse Forward + Wheel Down`: send `Ctrl + PageDown` (next tab in Chrome and other apps)
 
-Install from pypi
-```
-pip install jigsawwm
-```
+5. Check out the [examples/jmk.pyw](example/jmk.pyw) to find out more
 
-Install from github repo
-```
-pip install git+https://github.com/klesh/JigsawWM.git
-```
 
-## Quick Start
+## Service: tiling window manager
 
-**JigsawWm** follows the [suckless philosophy](https://suckless.org/philosophy/) and works just like [dwm - dynamic window manager | suckless.org software that sucks less](https://dwm.suckless.org/). All windows are treated as a `Ordered List`, they will be moved into places based on their `Order` and specified `Layout` **automatically** to improve your productivity.
+The **WindowManager** follows the [suckless philosophy](https://suckless.org/philosophy/) and works just like the [dwm](https://dwm.suckless.org/). All windows are treated as an `Ordered List`, they will be moved into places based on their `Order` and specified `Layout` **automatically**, save you from arranging them manually.
 
+### Demo
 
-### Step 1: Create a `.pyw` file as the "Configuration"
+https://user-images.githubusercontent.com/61080/210168366-e70dd649-f6ef-41bb-a8e5-941e392d770a.mp4
+
+### Default keybindings
 
-1. Download the [example.pyw](src/example.pyw) to your local hard drive
-2. Edit the code as you see fit
-3. Double-click the file and it should launch with a tray icon, or you may have to create a file association to the `Python` program
-4. Create a shortcut in your `Startup` folder if you like it
-
-### Step 2: Using hotkeys to manage your windows
-
-- `Win + j`: activate next window and move cursor to its center
-- `Win + k`: activate previous window and move cursor to its center
-- `Win + Shift + j`: move active window down in the list / swap with the next one
-- `Win + Shift + k`: move active window up in the list / swap with the previous one
-- `Win + n`: minimized active window
-- `Win + m`: maximize/unmaximized active window
-- `Win + /`: swap active window with **first window** in the list or **second window** if it is the first window already
-- `Win + q`: kill active window
+- `Win + j`: activate next window and move the cursor to its center
+- `Win + k`: activate the previous window and move the cursor to its center
+- `Win + Shift + j`: move the active window down in the list (swap with the next one) 
+- `Win + Shift + k`: move the active window up in the list (swap with the previous one)
+- `Win + /`: swap the active window with **the first window** in the list or **the second window** if it is the first window already
 - `Win + Space`: next theme, `Theme` consists of `Layout`, `Background`, `gap`, etc. to determine how windows should be placed
-- `Win + i`: activate first window of the next monitor if any or move cursor only
-- `Win + u`: activate first window of the previous monitor if any or move cursor only
-- `Win + Shift + i`: move active window to next monitor
-- `Win + Shift + u`: move active window to previous monitor
-- `Win + Control + i`: inspect active window
+- `Win + i`: activate the first window of the next monitor if any or move cursor only
+- `Win + u`: activate the first window of the previous monitor if any or move cursor only
+- `Win + Shift + i`: move the active window to the next monitor
+- `Win + Shift + u`: move the active window to the previous monitor
 
-### Step 3: Launch at startup
+## Service: run console program in the background
 
-1. Open your **Startup** folder by pressing `Win + r` to activate the **Run** dialog and type in `shell:startup`, a FileExplorer should pop up.
-2. Create a shortcut to your `.pyw` file. Done!
+Sometimes, software that should be run as a system service may not offer an installer to do the job, worse, it may ship as a Console Program. Nobody wants a Console Window stays on their desktops, and yes, I'm talking about [SyncThing](https://syncthing.net/). I love it but I would like it to run in the background quietly.
+
+```py
+class SyncthingService(daemon.ProcessService):
+    name = "syncthing"
+    args = [
+        r"C:\Programs\syncthing-windows-amd64-v1.23.2\syncthing.exe",
+        "-no-browser",
+        "-no-restart",
+        "-no-upgrade",
+    ]
+    log_path = r"C:\Programs\syncthing-windows-amd64-v1.23.2\syncthing.log"
 
 
-## Useful features:
+daemon.register(SyncthingService)
+```
 
-### Services
 
-To run a console program (e.g. syncthing) in the background as a service
+## Task: automate your workflows with tasks
 
+1. I would like to open a folder inside the Chromium Bookmark on the first boot-up every day.
 ```python
-from jigsawwm.daemon import Daemon
+class DailyRoutine(daemon.Task):
+    name = "daily routine"
 
-class MyDaemon(Daemon):
-    def setup(self):
-        from jigsawwm.services import ServiceEntry, register_service
-        register_service(
-            ServiceEntry(
-                name="syncthing",
-                args=[
-                    r"C:\Programs\syncthing-windows-amd64-v1.23.2\syncthing.exe",
-                    "-no-browser",
-                    "-no-restart",
-                    "-no-upgrade",
-                ],
-                log_path=r"C:\Programs\syncthing-windows-amd64-v1.23.2\syncthing.log",
-            )
-        )
+    def run(self):
+        chrome.open_fav_folder("bookmark_bar", "daily")
 
-MyDaemon(Daemon)
-```
+    def condition(self):
+        # trigger only once on daily-basis
+        return smartstart.daily_once("daily websites")
 
-### Smart Start
 
-To launch apps/tasks at login conditionally
+daemon.register(DailyRoutine)
+```
 
-1. What if I would like a folder named `daily` in my Chrome Bookmark Bar to be opened automatically on my first boot-up every day?
+2. I would like to launch my IM / Mail Client on workdays
 ```python
-from jigsawwm.daemon import Daemon
+class WorkdayRoutine(daemon.Task):
+    name = "workday routine"
 
-class MyDaemon(Daemon):
-    def setup(self):
-        from jigsawwm.smartstart import (
-            SmartStartEntry,
-            daily_once,
-            open_chrome_fav_folder,
-            register_smartstart,
+    def __init__(self) -> None:
+        super().__init__()
+        self.holiday_book = ChinaHolidayBook()
+
+    def run(self):
+        smartstart.start_if_not_running(
+            r"C:\Users\Klesh\AppData\Local\Feishu\Feishu.exe"
         )
-        register_smartstart(
-            SmartStartEntry(
-                name="daily routine",
-                launch=lambda: open_chrome_fav_folder("bookmark_bar", "daily"),
-                condition=lambda: daily_once("daily websites"),
-            )
+        smartstart.start_if_not_running(
+            r"C:\Program Files\Mozilla Thunderbird\thunderbird.exe"
         )
 
-MyDaemon(Daemon)
+    def condition(self):
+        return self.holiday_book.is_workhour(extend=timedelta(hours=2))
+
+
+daemon.register(WorkdayRoutine)
 ```
-2. What if I would like a couple of apps to be launched when I boot up the computer within work hours?
-```python
 
-        holiday_book = ChinaHolidayBook()
 
-        def open_worklog():
-            """Open worklog (a markdown file) for today (create if it doesn't exist yet)."""
-            next_workday = holiday_book.next_workday()
-            latest_workday = holiday_book.latest_workday()
-            worklog_path = os.path.join(
-                os.path.expanduser("~/Documents/Sync/worklog"),
-                f"{next_workday.isoformat()}.md",
-            )
-            if not os.path.exists(worklog_path):
-                with open(worklog_path, "w") as f:
-                    prevdate = latest_workday.strftime("%m/%d")
-                    nextdate = next_workday.strftime("%m/%d")
-                    f.write(f"{prevdate}\n1. \n\n{nextdate}\n1. ")
-            os.startfile(worklog_path)
-
-        register_smartstart(
-            SmartStartEntry(
-                name="workhour routine",
-                launch=[
-                    r"C:\Users\Klesh\AppData\Local\Feishu\Feishu.exe",
-                    r"C:\Program Files\Mozilla Thunderbird\thunderbird.exe",
-                    open_worklog,
-                ],
-                # in case I might boot up the computer a little bit earlier
-                condition=lambda: holiday_book.is_workhour(extend=timedelta(hours=2)),
-            )
-        )
+# Installation
+
+Tested on **Windows 11 Build 22000** and **Python 3.11.1**.
+Should work on **Windows 10** and **Python 3.8**
+
+
+Install from pypi
+```
+pip install jigsawwm
+```
 
+Install from Github repo
 ```
+pip install git+https://github.com/klesh/JigsawWM.git
+```
+
+## Quick Start
 
-### Tray menu
 
-![tray menu](docs/img/tray_menu.png)
 
-Functionalities:
+### Step 1: Create a `.pyw` file as your "Configuration"
 
-1. Stop/start a `service` 
-2. Run a `smartstart` without condition
+Choose services you like from the [examples](examples) folder, you may use any of the following directly.
+
+- [examples/jmk.pyw](examples/jmk.pyw) if you are looking for a QMK/AutoHotkey alternative
+- [examples/services.pyw](examples/services.pyw) if you are trying to run some Console Program as Service in the background
+- [examples/tasks.pyw](examples/tasks.pyw) if you are looking for a solution to automate your workflow smartly on startup
+- [examples/wm.pyw](examples/wm.pyw) if you are looking for a tiling window manager
+- [examples/jigsaw.pyw](examples/wm.pyw) the whole package of the above
+
+### Step 2: Launch your `.pyw` file and manage your services
+
+Double-click the `.pyw` file and a tray icon should appear, right-click the icon to manage your services.
+![image](https://github.com/klesh/JigsawWM/assets/61080/dd6b0c05-19eb-4a55-a7b6-8c66afff09b9)
+
+
+### Step 3: Launch at startup
+
+1. Open your **Startup** folder by pressing `Win + r` to activate the **Run** dialog and type in `shell:startup`, a FileExplorer should pop up.
+2. Create a shortcut to your `.pyw` file. Done!
 
 
 ## Document
 
 [Read the Docs](https://jigsawwm.readthedocs.io/en/latest/)
 
 
 ## Changelog
 
+### 2023-07-12 (v2.0)
+
+- refactor: divided features into multiple services to allow users to use only what they need
+- feat: replace the `hotkey` module with the `jmk` module, which mimics the basic functionality
+  of [QMK](https://qmk.fm/) as an alternative to [AutoHotkey](https://www.autohotkey.com/)
+
+### 2023-04-07
+
+- hotkey support mouse buttons, forward/backward buttons as modifier
+
 ### 2023-04-05
 
 - add `smartstart` feature
 - BREAKING CHANGE: rename `svcmgr` to `services`
 - adopt `pyproject.toml`
 
 ### 2023-03-21
```

### Comparing `jigsawwm-1.2.1/src/jigsawwm.egg-info/SOURCES.txt` & `jigsawwm-2.0.0/src/jigsawwm.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 requirements.txt
 src/jigsawwm/__init__.py
+src/jigsawwm/chrome.py
 src/jigsawwm/daemon.py
-src/jigsawwm/hotkey.py
-src/jigsawwm/manager.py
-src/jigsawwm/services.py
 src/jigsawwm/smartstart.py
 src/jigsawwm/state.py
 src/jigsawwm/virtdeskstub.py
+src/jigsawwm/wm.py
 src/jigsawwm.egg-info/PKG-INFO
 src/jigsawwm.egg-info/SOURCES.txt
 src/jigsawwm.egg-info/dependency_links.txt
 src/jigsawwm.egg-info/requires.txt
 src/jigsawwm.egg-info/top_level.txt
 src/jigsawwm/assets/dwindle.png
 src/jigsawwm/assets/icons.svg
 src/jigsawwm/assets/logo.png
 src/jigsawwm/assets/obs.png
 src/jigsawwm/assets/wide-dwindle.png
+src/jigsawwm/jmk/__init__.py
+src/jigsawwm/jmk/core.py
+src/jigsawwm/jmk/hotkey.py
+src/jigsawwm/jmk/sysinout.py
 src/jigsawwm/tiler/__init__.py
 src/jigsawwm/tiler/layouts.py
 src/jigsawwm/tiler/tilers.py
 src/jigsawwm/w32/__init__.py
 src/jigsawwm/w32/hook.py
 src/jigsawwm/w32/idesktopwallpaper.py
 src/jigsawwm/w32/ivirtualdesktopmanager.py
 src/jigsawwm/w32/monitor.py
 src/jigsawwm/w32/process.py
 src/jigsawwm/w32/sendinput.py
 src/jigsawwm/w32/vk.py
 src/jigsawwm/w32/window.py
 src/jigsawwm/w32/window_structs.py
-src/jigsawwm/w32/winevent.py
+src/jigsawwm/w32/winevent.py
+tests/test_jmk_core.py
+tests/test_jmk_hotkey.py
```

