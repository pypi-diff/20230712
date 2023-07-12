# Comparing `tmp/ectool-1.1.6.tar.gz` & `tmp/ectool-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ectool-1.1.6.tar", last modified: Mon Jul 10 15:50:19 2023, max compression
+gzip compressed data, was "ectool-1.1.7.tar", last modified: Wed Jul 12 04:29:38 2023, max compression
```

## Comparing `ectool-1.1.6.tar` & `ectool-1.1.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 15:50:19.890507 ectool-1.1.6/
--rw-rw-rw-   0        0        0     1100 2023-07-06 14:25:24.000000 ectool-1.1.6/LICENSE
--rw-rw-rw-   0        0        0     2440 2023-07-10 15:50:19.891506 ectool-1.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     1397 2023-07-10 15:46:25.000000 ectool-1.1.6/README.md
--rw-rw-rw-   0        0        0      113 2023-07-10 15:50:19.891506 ectool-1.1.6/setup.cfg
--rw-rw-rw-   0        0        0     7947 2023-07-10 15:45:44.000000 ectool-1.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-10 15:50:19.868507 ectool-1.1.6/src/
-drwxrwxrwx   0        0        0        0 2023-07-10 15:50:19.883507 ectool-1.1.6/src/ectool/
--rw-rw-rw-   0        0        0      110 2023-07-07 03:56:54.000000 ectool-1.1.6/src/ectool/__init__.py
--rw-rw-rw-   0        0        0    16211 2023-07-08 05:57:46.000000 ectool-1.1.6/src/ectool/ecaction.py
--rw-rw-rw-   0        0        0   141543 2023-07-08 06:53:08.000000 ectool-1.1.6/src/ectool/ecag.py
--rw-rw-rw-   0        0        0    10483 2023-07-10 15:44:30.000000 ectool-1.1.6/src/ectool/eccli.py
--rw-rw-rw-   0        0        0     1655 2023-07-08 06:53:06.000000 ectool-1.1.6/src/ectool/ecconst.py
--rw-rw-rw-   0        0        0     3624 2023-07-10 15:44:41.000000 ectool-1.1.6/src/ectool/eclogs.py
--rw-rw-rw-   0        0        0     6002 2023-07-06 14:56:04.000000 ectool-1.1.6/src/ectool/ecstruct.py
--rw-rw-rw-   0        0        0     3912 2023-07-08 05:24:57.000000 ectool-1.1.6/src/ectool/unpkg.py
-drwxrwxrwx   0        0        0        0 2023-07-10 15:50:19.889506 ectool-1.1.6/src/ectool.egg-info/
--rw-rw-rw-   0        0        0     2440 2023-07-10 15:50:19.000000 ectool-1.1.6/src/ectool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      413 2023-07-10 15:50:19.000000 ectool-1.1.6/src/ectool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 15:50:19.000000 ectool-1.1.6/src/ectool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-07-10 15:50:19.000000 ectool-1.1.6/src/ectool.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       62 2023-07-10 15:50:19.000000 ectool-1.1.6/src/ectool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-10 15:50:19.000000 ectool-1.1.6/src/ectool.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-12 04:29:38.777932 ectool-1.1.7/
+-rw-rw-rw-   0        0        0     1100 2023-07-06 14:25:24.000000 ectool-1.1.7/LICENSE
+-rw-rw-rw-   0        0        0     2542 2023-07-12 04:29:38.777932 ectool-1.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1499 2023-07-12 04:26:17.000000 ectool-1.1.7/README.md
+-rw-rw-rw-   0        0        0      113 2023-07-12 04:29:38.778931 ectool-1.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     7947 2023-07-12 04:24:13.000000 ectool-1.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 04:29:38.751934 ectool-1.1.7/src/
+drwxrwxrwx   0        0        0        0 2023-07-12 04:29:38.767932 ectool-1.1.7/src/ectool/
+-rw-rw-rw-   0        0        0      110 2023-07-07 03:56:54.000000 ectool-1.1.7/src/ectool/__init__.py
+-rw-rw-rw-   0        0        0    16211 2023-07-08 05:57:46.000000 ectool-1.1.7/src/ectool/ecaction.py
+-rw-rw-rw-   0        0        0   141543 2023-07-08 06:53:08.000000 ectool-1.1.7/src/ectool/ecag.py
+-rw-rw-rw-   0        0        0    11475 2023-07-12 04:23:44.000000 ectool-1.1.7/src/ectool/eccli.py
+-rw-rw-rw-   0        0        0     1655 2023-07-08 06:53:06.000000 ectool-1.1.7/src/ectool/ecconst.py
+-rw-rw-rw-   0        0        0     3624 2023-07-10 15:44:41.000000 ectool-1.1.7/src/ectool/eclogs.py
+-rw-rw-rw-   0        0        0     6002 2023-07-06 14:56:04.000000 ectool-1.1.7/src/ectool/ecstruct.py
+-rw-rw-rw-   0        0        0     3912 2023-07-08 05:24:57.000000 ectool-1.1.7/src/ectool/unpkg.py
+drwxrwxrwx   0        0        0        0 2023-07-12 04:29:38.776931 ectool-1.1.7/src/ectool.egg-info/
+-rw-rw-rw-   0        0        0     2542 2023-07-12 04:29:38.000000 ectool-1.1.7/src/ectool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2023-07-12 04:29:38.000000 ectool-1.1.7/src/ectool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 04:29:38.000000 ectool-1.1.7/src/ectool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-07-12 04:29:38.000000 ectool-1.1.7/src/ectool.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       62 2023-07-12 04:29:38.000000 ectool-1.1.7/src/ectool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-12 04:29:38.000000 ectool-1.1.7/src/ectool.egg-info/top_level.txt
```

### Comparing `ectool-1.1.6/LICENSE` & `ectool-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ectool-1.1.6/PKG-INFO` & `ectool-1.1.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ectool
-Version: 1.1.6
+Version: 1.1.7
 Summary: A tools for EC modules, like EC618/EC616/EC718
 Home-page: https://github.com/openLuat/ectool2py
 Author: Wendal Chen
 Project-URL: Bug Reports, https://github.com/openLuat/ectool2py/issues
 Project-URL: Source, https://github.com/openLuat/ectool2py/
 Keywords: ec618,development
 Classifier: Development Status :: 3 - Alpha
@@ -24,24 +24,26 @@
 Provides-Extra: test
 License-File: LICENSE
 
 # 移芯工具箱
 
 支持移芯方案的刷机, 解包, windows/linux/macos 可用
 
-当前支持EC618系列, 例如Air780E/Air700E等模块
+当前支持EC618系列, 例如Air780E/Air700E/Air600E/Air780EG等模块
+
+本库可支持被引用, eccli本身就是调用实例.
 
 ## 用法
 
 先安装ectool, 在命令行或控制台执行
 
 ```bash
 # 清华镜像
 pip3 install -U -i https://pypi.tuna.tsinghua.edu.cn/simple ectool
-# 无镜像,或者系统默认镜像
+# 若安装失败, 可尝试以下命令, 从pypi直接进行安装
 pip3 install -U ectool
 ```
 
 刷机(当前仅USB刷机), 支持binpkg和soc文件
 
 ```bash
 ectool burn -f example.binpkg
@@ -50,20 +52,20 @@
 
 更多参数执行 `ectool -h` 获取说明
 
 ## TODO List
 
 * [x] EC618使用USB刷机
 * [x] binpkg解包
-* [x] 测试Linux下的兼容性
+* [x] 兼容Linux下刷机
 * [x] 支持只刷AP或CP
 * [x] 支持跳过AgentBoot
 * [x] 支持擦除指定区域的数据
 * [x] SoC日志解析(简易)
-* [ ] 支持从http加载固件文件进行下载
+* [x] 支持从http加载固件文件进行下载
 * [ ] EC618使用物理UART刷机
 * [ ] 测试Mac下的兼容性
 * [ ] 支持刷LuatOS的script.bin
 * [ ] 完整的注释
 * [ ] SoC日志解析(完整)
 * [ ] binpkg打包
```

### Comparing `ectool-1.1.6/README.md` & `ectool-1.1.7/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # 移芯工具箱
 
 支持移芯方案的刷机, 解包, windows/linux/macos 可用
 
-当前支持EC618系列, 例如Air780E/Air700E等模块
+当前支持EC618系列, 例如Air780E/Air700E/Air600E/Air780EG等模块
+
+本库可支持被引用, eccli本身就是调用实例.
 
 ## 用法
 
 先安装ectool, 在命令行或控制台执行
 
 ```bash
 # 清华镜像
 pip3 install -U -i https://pypi.tuna.tsinghua.edu.cn/simple ectool
-# 无镜像,或者系统默认镜像
+# 若安装失败, 可尝试以下命令, 从pypi直接进行安装
 pip3 install -U ectool
 ```
 
 刷机(当前仅USB刷机), 支持binpkg和soc文件
 
 ```bash
 ectool burn -f example.binpkg
@@ -24,20 +26,20 @@
 
 更多参数执行 `ectool -h` 获取说明
 
 ## TODO List
 
 * [x] EC618使用USB刷机
 * [x] binpkg解包
-* [x] 测试Linux下的兼容性
+* [x] 兼容Linux下刷机
 * [x] 支持只刷AP或CP
 * [x] 支持跳过AgentBoot
 * [x] 支持擦除指定区域的数据
 * [x] SoC日志解析(简易)
-* [ ] 支持从http加载固件文件进行下载
+* [x] 支持从http加载固件文件进行下载
 * [ ] EC618使用物理UART刷机
 * [ ] 测试Mac下的兼容性
 * [ ] 支持刷LuatOS的script.bin
 * [ ] 完整的注释
 * [ ] SoC日志解析(完整)
 * [ ] binpkg打包
```

### Comparing `ectool-1.1.6/setup.py` & `ectool-1.1.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     name="ectool",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="1.1.6",  # Required
+    version="1.1.7",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="A tools for EC modules, like EC618/EC616/EC718",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

### Comparing `ectool-1.1.6/src/ectool/ecaction.py` & `ectool-1.1.7/src/ectool/ecaction.py`

 * *Files identical despite different names*

### Comparing `ectool-1.1.6/src/ectool/ecag.py` & `ectool-1.1.7/src/ectool/ecag.py`

 * *Files identical despite different names*

### Comparing `ectool-1.1.6/src/ectool/eccli.py` & `ectool-1.1.7/src/ectool/eccli.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,15 +78,27 @@
     return 0
 
 def cli_burn() :
     if not ecargs.file :
         logger.error("require -f/--file !!!")
         sys.exit(3)
     import ectool.unpkg as unpkg
-    jdata = unpkg.binpkg_unpack(ecargs.file, outpath_dir=None, ram=True, debug=ecargs.debug)
+
+    if str(ecargs.file).startswith("http://") or str(ecargs.file).startswith("https://") :
+        logger.info("downloading ... " + ecargs.file)
+        import requests
+        resp = requests.get(ecargs.file)
+        if resp.status_code != 200 :
+            logger.error("http resp {}".format(resp.status_code))
+            sys.exit(4)
+        fdata = resp.content
+        logger.info("size {}".format(len(fdata)))
+        jdata = unpkg.binpkg_unpack(fdata, outpath_dir=None, ram=True, debug=ecargs.debug)
+    else :
+        jdata = unpkg.binpkg_unpack(ecargs.file, outpath_dir=None, ram=True, debug=ecargs.debug)
     logger.info("Files " + json.dumps(list(jdata.keys())))
     
     if not select_com() :
         sys.exit(2)
     logger.info("Select " + ecargs.port)
     
 
@@ -98,32 +110,49 @@
     if 0 != burn_sync(burncom, enSynHandshakeType.SYNC_HANDSHAKE_DLBOOT, 2) :
         return -1
     logging.info("Done Sync")
 
     if do_agentboot(burncom) != 0 :
         return -1
 
+    # 根据image_type得出各分区的名称
+    BL_NAME = None
+    CP_NAME = None
+    AP_NAME = None
+    for name in jdata :
+        if not "data" in jdata[name] :
+            continue
+        if jdata[name]["image_type"] == "BL" :
+            BL_NAME = name
+        if jdata[name]["image_type"] == "CP" :
+            CP_NAME = name
+        if jdata[name]["image_type"] == "AP" :
+            if name == "script" :
+                continue
+            else :
+                AP_NAME = name
+
     while 1 :
-        if "ap_bootloader" in jdata and ecargs.burn_bl == "y" :
+        if BL_NAME and ecargs.burn_bl == "y" :
             logging.info("Go   BL download")
-            ret = burn_img(burncom, jdata["ap_bootloader"]["data"], enBurnImageType.BTYPE_BOOTLOADER, STYPE_AP_FLASH, 0, tag="BL")
+            ret = burn_img(burncom, jdata[BL_NAME]["data"], enBurnImageType.BTYPE_BOOTLOADER, STYPE_AP_FLASH, 0, tag="BL")
             if ret != 0 :
                 logging.error("burn_img BootLoader fail")
                 break
             logging.info("Done BL download")
-        if "ap" in jdata and ecargs.burn_ap == "y" :
+        if AP_NAME and ecargs.burn_ap == "y" :
             logging.info("Go   AP download")
-            ret = burn_img(burncom, jdata["ap"]["data"], enBurnImageType.BTYPE_AP, STYPE_AP_FLASH, 0x24000, tag="AP")
+            ret = burn_img(burncom, jdata[AP_NAME]["data"], enBurnImageType.BTYPE_AP, STYPE_AP_FLASH, 0x24000, tag="AP")
             if ret != 0 :
                 logging.error("burn_img AP fail")
                 break
             logging.info("Done AP download")
-        if "cp-demo-flash" in jdata and ecargs.burn_cp == "y" :
+        if CP_NAME and ecargs.burn_cp == "y" :
             logging.info("Go   CP download")
-            ret = burn_img(burncom, jdata["cp-demo-flash"]["data"], enBurnImageType.BTYPE_CP, STYPE_CP_FLASH, 0, tag="CP")
+            ret = burn_img(burncom, jdata[CP_NAME]["data"], enBurnImageType.BTYPE_CP, STYPE_CP_FLASH, 0, tag="CP")
             if ret != 0 :
                 logging.error("burn_img CP fail")
                 break
             logging.info("Done CP download")
 
         if "script" in jdata and ecargs.burn_script == "y" :
             logging.info("Do   Script download")
```

### Comparing `ectool-1.1.6/src/ectool/ecconst.py` & `ectool-1.1.7/src/ectool/ecconst.py`

 * *Files identical despite different names*

### Comparing `ectool-1.1.6/src/ectool/eclogs.py` & `ectool-1.1.7/src/ectool/eclogs.py`

 * *Files identical despite different names*

### Comparing `ectool-1.1.6/src/ectool/ecstruct.py` & `ectool-1.1.7/src/ectool/ecstruct.py`

 * *Files identical despite different names*

### Comparing `ectool-1.1.6/src/ectool/unpkg.py` & `ectool-1.1.7/src/ectool/unpkg.py`

 * *Files identical despite different names*

### Comparing `ectool-1.1.6/src/ectool.egg-info/PKG-INFO` & `ectool-1.1.7/src/ectool.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ectool
-Version: 1.1.6
+Version: 1.1.7
 Summary: A tools for EC modules, like EC618/EC616/EC718
 Home-page: https://github.com/openLuat/ectool2py
 Author: Wendal Chen
 Project-URL: Bug Reports, https://github.com/openLuat/ectool2py/issues
 Project-URL: Source, https://github.com/openLuat/ectool2py/
 Keywords: ec618,development
 Classifier: Development Status :: 3 - Alpha
@@ -24,24 +24,26 @@
 Provides-Extra: test
 License-File: LICENSE
 
 # 移芯工具箱
 
 支持移芯方案的刷机, 解包, windows/linux/macos 可用
 
-当前支持EC618系列, 例如Air780E/Air700E等模块
+当前支持EC618系列, 例如Air780E/Air700E/Air600E/Air780EG等模块
+
+本库可支持被引用, eccli本身就是调用实例.
 
 ## 用法
 
 先安装ectool, 在命令行或控制台执行
 
 ```bash
 # 清华镜像
 pip3 install -U -i https://pypi.tuna.tsinghua.edu.cn/simple ectool
-# 无镜像,或者系统默认镜像
+# 若安装失败, 可尝试以下命令, 从pypi直接进行安装
 pip3 install -U ectool
 ```
 
 刷机(当前仅USB刷机), 支持binpkg和soc文件
 
 ```bash
 ectool burn -f example.binpkg
@@ -50,20 +52,20 @@
 
 更多参数执行 `ectool -h` 获取说明
 
 ## TODO List
 
 * [x] EC618使用USB刷机
 * [x] binpkg解包
-* [x] 测试Linux下的兼容性
+* [x] 兼容Linux下刷机
 * [x] 支持只刷AP或CP
 * [x] 支持跳过AgentBoot
 * [x] 支持擦除指定区域的数据
 * [x] SoC日志解析(简易)
-* [ ] 支持从http加载固件文件进行下载
+* [x] 支持从http加载固件文件进行下载
 * [ ] EC618使用物理UART刷机
 * [ ] 测试Mac下的兼容性
 * [ ] 支持刷LuatOS的script.bin
 * [ ] 完整的注释
 * [ ] SoC日志解析(完整)
 * [ ] binpkg打包
```

