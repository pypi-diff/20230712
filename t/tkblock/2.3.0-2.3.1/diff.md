# Comparing `tmp/tkblock-2.3.0.tar.gz` & `tmp/tkblock-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkblock-2.3.0.tar", last modified: Fri Jun  2 18:27:34 2023, max compression
+gzip compressed data, was "tkblock-2.3.1.tar", last modified: Wed Jul 12 15:33:03 2023, max compression
```

## Comparing `tkblock-2.3.0.tar` & `tkblock-2.3.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 18:27:34.557546 tkblock-2.3.0/
--rw-rw-rw-   0        0        0     1077 2023-06-02 17:09:00.000000 tkblock-2.3.0/LICENSE
--rw-rw-rw-   0        0        0    15304 2023-06-02 18:27:34.555550 tkblock-2.3.0/PKG-INFO
--rw-rw-rw-   0        0        0    14580 2023-06-02 11:06:20.000000 tkblock-2.3.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-02 18:27:34.558546 tkblock-2.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1017 2023-06-02 18:25:46.000000 tkblock-2.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-02 18:27:34.538599 tkblock-2.3.0/tkblock/
--rw-rw-rw-   0        0        0      584 2023-05-19 17:11:52.000000 tkblock-2.3.0/tkblock/__init__.py
--rw-rw-rw-   0        0        0     3408 2023-05-19 17:11:52.000000 tkblock-2.3.0/tkblock/block_framebase.py
--rw-rw-rw-   0        0        0    21644 2023-05-19 17:11:52.000000 tkblock-2.3.0/tkblock/block_framework.py
--rw-rw-rw-   0        0        0    41266 2023-06-02 18:23:40.000000 tkblock-2.3.0/tkblock/block_service.py
--rw-rw-rw-   0        0        0      426 2023-05-19 17:11:52.000000 tkblock-2.3.0/tkblock/block_util.py
--rw-rw-rw-   0        0        0     3750 2023-06-02 18:21:40.000000 tkblock-2.3.0/tkblock/block_waiting_screen.py
--rw-rw-rw-   0        0        0     1418 2023-05-19 17:11:52.000000 tkblock-2.3.0/tkblock/canvas.py
--rw-rw-rw-   0        0        0      494 2023-05-19 17:11:53.000000 tkblock-2.3.0/tkblock/layout.py
--rw-rw-rw-   0        0        0      368 2023-05-19 17:11:53.000000 tkblock-2.3.0/tkblock/scrollbar.py
-drwxrwxrwx   0        0        0        0 2023-06-02 18:27:34.551562 tkblock-2.3.0/tkblock.egg-info/
--rw-rw-rw-   0        0        0    15304 2023-06-02 18:27:34.000000 tkblock-2.3.0/tkblock.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2023-06-02 18:27:34.000000 tkblock-2.3.0/tkblock.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 18:27:34.000000 tkblock-2.3.0/tkblock.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-02 18:27:34.000000 tkblock-2.3.0/tkblock.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-12 15:33:03.161235 tkblock-2.3.1/
+-rw-rw-rw-   0        0        0     1077 2023-06-02 17:09:00.000000 tkblock-2.3.1/LICENSE
+-rw-rw-rw-   0        0        0    15304 2023-07-12 15:33:03.160269 tkblock-2.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0    14580 2023-06-02 11:06:20.000000 tkblock-2.3.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-12 15:33:03.162233 tkblock-2.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1017 2023-07-12 15:32:18.000000 tkblock-2.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 15:33:03.146208 tkblock-2.3.1/tkblock/
+-rw-rw-rw-   0        0        0      584 2023-05-19 17:11:52.000000 tkblock-2.3.1/tkblock/__init__.py
+-rw-rw-rw-   0        0        0     3408 2023-05-19 17:11:52.000000 tkblock-2.3.1/tkblock/block_framebase.py
+-rw-rw-rw-   0        0        0    21644 2023-05-19 17:11:52.000000 tkblock-2.3.1/tkblock/block_framework.py
+-rw-rw-rw-   0        0        0    41449 2023-06-18 14:16:06.000000 tkblock-2.3.1/tkblock/block_service.py
+-rw-rw-rw-   0        0        0      426 2023-05-19 17:11:52.000000 tkblock-2.3.1/tkblock/block_util.py
+-rw-rw-rw-   0        0        0     3750 2023-06-02 18:21:40.000000 tkblock-2.3.1/tkblock/block_waiting_screen.py
+-rw-rw-rw-   0        0        0     1574 2023-06-18 14:21:05.000000 tkblock-2.3.1/tkblock/canvas.py
+-rw-rw-rw-   0        0        0      494 2023-05-19 17:11:53.000000 tkblock-2.3.1/tkblock/layout.py
+-rw-rw-rw-   0        0        0      368 2023-05-19 17:11:53.000000 tkblock-2.3.1/tkblock/scrollbar.py
+drwxrwxrwx   0        0        0        0 2023-07-12 15:33:03.158240 tkblock-2.3.1/tkblock.egg-info/
+-rw-rw-rw-   0        0        0    15304 2023-07-12 15:33:02.000000 tkblock-2.3.1/tkblock.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2023-07-12 15:33:02.000000 tkblock-2.3.1/tkblock.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 15:33:02.000000 tkblock-2.3.1/tkblock.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-12 15:33:02.000000 tkblock-2.3.1/tkblock.egg-info/top_level.txt
```

### Comparing `tkblock-2.3.0/LICENSE` & `tkblock-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tkblock-2.3.0/PKG-INFO` & `tkblock-2.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkblock
-Version: 2.3.0
+Version: 2.3.1
 Summary: tkinter block framework
 Home-page: https://github.com/kuri-pome/tkblock
 Author: kuri_pome
 License: MIT
 Keywords: tkinter place widget easy
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `tkblock-2.3.0/README.md` & `tkblock-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `tkblock-2.3.0/setup.py` & `tkblock-2.3.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 # README.mdをlong_discriptionにするために読み込む
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 setup(
     name=package_name,
-    version="2.3.0",
+    version="2.3.1",
     description="tkinter block framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kuri-pome/tkblock",
     author="kuri_pome",
     license="MIT",
     keywords="tkinter place widget easy",
```

### Comparing `tkblock-2.3.0/tkblock/__init__.py` & `tkblock-2.3.1/tkblock/__init__.py`

 * *Files identical despite different names*

### Comparing `tkblock-2.3.0/tkblock/block_framebase.py` & `tkblock-2.3.1/tkblock/block_framebase.py`

 * *Files identical despite different names*

### Comparing `tkblock-2.3.0/tkblock/block_framework.py` & `tkblock-2.3.1/tkblock/block_framework.py`

 * *Files identical despite different names*

### Comparing `tkblock-2.3.0/tkblock/block_service.py` & `tkblock-2.3.1/tkblock/block_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,25 +28,29 @@
     def wrapper(func):
         @wraps(func)
         def wait_processe(*args, **kwargs):
             root = BlockService.root if frame is None else frame
             result = [None]
             is_force_finish = [False]
             wait_screen = BlockWaitingScreen(root, is_force_finish)
-            
+
             def _execute(result, wait_screen, func, *args, **kwargs):
                 result[0] = func(*args, **kwargs)
                 wait_screen.end_thread()
 
             # # スレッドを実行して、関数を実行
             wait_thread = threading.Thread(target=wait_screen.start_thread)
             # wait_thread.daemon = False
             wait_thread.start()
             # run_thread = threading.Thread(target=partial(_execute, result, wait_screen, func, args=args, kwargs=kwargs), args=args, kwargs=kwargs)
-            run_thread = threading.Thread(target=partial(_execute, result, wait_screen, func), args=args, kwargs=kwargs)
+            run_thread = threading.Thread(
+                target=partial(_execute, result, wait_screen, func),
+                args=args,
+                kwargs=kwargs,
+            )
             # run_thread.daemon = True
             run_thread.start()
             return result[0]
 
         return wait_processe
 
     return wrapper
@@ -256,14 +260,15 @@
         row_start,
         row_end,
         *args,
         pad_left=0.0,
         pad_right=0.0,
         pad_up=0.0,
         pad_down=0.0,
+        is_resize=True,
         **kwargs,
     ):
         """BlockCanvasを作成する
 
         例
         cavas1 = BlockService.create_canvas(self.frame, 42, 49, 15, 20)
         cavas1.create_line(0, 0, 430, 300)
@@ -278,15 +283,18 @@
             pad_right (float, optional): 横幅の右側の隙間(0~1). Defaults to 0.0.
             pad_up (float, optional): 立幅の上側の隙間(0~1). Defaults to 0.0.
             pad_down (float, optional): 立幅の下側の隙間(0~1). Defaults to 0.0.
 
         Returns:
             BlockCanvas: BlockCanvas
         """
-        canvas = BlockCanvas(frame, *args, **kwargs)
+        if is_resize:
+            canvas = ResizingCanvas(frame, *args, **kwargs)
+        else:
+            canvas = BlockCanvas(frame, *args, **kwargs)
         canvas.layout = cls.layout(
             col_start,
             col_end,
             row_start,
             row_end,
             pad_left=pad_left,
             pad_right=pad_right,
```

### Comparing `tkblock-2.3.0/tkblock/block_waiting_screen.py` & `tkblock-2.3.1/tkblock/block_waiting_screen.py`

 * *Files identical despite different names*

### Comparing `tkblock-2.3.0/tkblock/canvas.py` & `tkblock-2.3.1/tkblock/canvas.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,33 +4,40 @@
 """ResizingCanvas
 
 自動調整されるキャンバス
 """
 import tkinter as tk
 
 
+class BlockCanvas(tk.Canvas):
+    """tk.Canvas"""
+
+    def __init__(self, frame, *args, **kwargs):
+        super().__init__(frame, *args, **kwargs)
+
+
 class ResizingCanvas(tk.Canvas):
     """ユーザーがフレームサイズを変更した場合、自動調整されるキャンバス
 
     既存のCanvasはユーザーがwindowsのサイズを変更した場合追従をしてくれない。
     それを回避するために、サイズ変更のイベントのたびに、変更するクラスを作成。
 
     Args:
         tk (tk.Canvas): キャンバス
     """
 
-    def __init__(self, parent: tk.Frame, **kwargs) -> None:
+    def __init__(self, frame, *args, **kwargs) -> None:
         """コンストラクタ
 
         Args:
-            parent (tk.Frame): キャンバスを乗せる親フレーム
+            frame (tk.Frame): キャンバスを乗せる親フレーム
         """
-        super().__init__(parent, **kwargs)
-        self.width: int = parent.width
-        self.height: int = parent.height
+        super().__init__(frame, *args, **kwargs)
+        self.width: int = frame.width
+        self.height: int = frame.height
         self.bind("<Configure>", self.on_resize)
 
     def on_resize(self, event: tk.Event) -> None:
         """リサイズを行う
 
         Args:
             event (tk.Event): イベント
```

### Comparing `tkblock-2.3.0/tkblock.egg-info/PKG-INFO` & `tkblock-2.3.1/tkblock.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkblock
-Version: 2.3.0
+Version: 2.3.1
 Summary: tkinter block framework
 Home-page: https://github.com/kuri-pome/tkblock
 Author: kuri_pome
 License: MIT
 Keywords: tkinter place widget easy
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
```

