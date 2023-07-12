# Comparing `tmp/woebin-python-0.1.3.tar.gz` & `tmp/woebin-python-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "woebin-python-0.1.3.tar", last modified: Wed Jul 12 11:38:22 2023, max compression
+gzip compressed data, was "woebin-python-0.1.4.tar", last modified: Wed Jul 12 11:42:22 2023, max compression
```

## Comparing `woebin-python-0.1.3.tar` & `woebin-python-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 11:38:22.993664 woebin-python-0.1.3/
--rw-rw-rw-   0        0        0     1498 2023-07-12 11:38:22.993664 woebin-python-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1271 2023-07-04 18:46:47.000000 woebin-python-0.1.3/README.md
--rw-rw-rw-   0        0        0       42 2023-07-12 11:38:22.993664 woebin-python-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      490 2023-07-12 11:32:53.000000 woebin-python-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-12 11:38:22.978337 woebin-python-0.1.3/target/
-drwxrwxrwx   0        0        0        0 2023-07-12 11:38:22.980659 woebin-python-0.1.3/target/release/
--rw-rw-rw-   0        0        0   224768 2023-07-12 11:38:22.000000 woebin-python-0.1.3/target/release/woebin.dll
-drwxrwxrwx   0        0        0        0 2023-07-12 11:38:22.981661 woebin-python-0.1.3/woebin/
--rw-rw-rw-   0        0        0     3998 2023-07-12 11:37:51.000000 woebin-python-0.1.3/woebin/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 11:38:22.992666 woebin-python-0.1.3/woebin_python.egg-info/
--rw-rw-rw-   0        0        0     1498 2023-07-12 11:38:22.000000 woebin-python-0.1.3/woebin_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      211 2023-07-12 11:38:22.000000 woebin-python-0.1.3/woebin_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 11:38:22.000000 woebin-python-0.1.3/woebin_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-12 11:38:22.000000 woebin-python-0.1.3/woebin_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-12 11:42:22.243932 woebin-python-0.1.4/
+-rw-rw-rw-   0        0        0     1498 2023-07-12 11:42:22.242934 woebin-python-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1271 2023-07-04 18:46:47.000000 woebin-python-0.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-12 11:42:22.243932 woebin-python-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      832 2023-07-12 11:41:55.000000 woebin-python-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 11:42:22.230388 woebin-python-0.1.4/target/
+drwxrwxrwx   0        0        0        0 2023-07-12 11:42:22.232390 woebin-python-0.1.4/target/release/
+-rw-rw-rw-   0        0        0   224768 2023-07-12 11:42:21.000000 woebin-python-0.1.4/target/release/woebin.dll
+drwxrwxrwx   0        0        0        0 2023-07-12 11:42:22.233387 woebin-python-0.1.4/woebin/
+-rw-rw-rw-   0        0        0     3998 2023-07-12 11:37:51.000000 woebin-python-0.1.4/woebin/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 11:42:22.241922 woebin-python-0.1.4/woebin_python.egg-info/
+-rw-rw-rw-   0        0        0     1498 2023-07-12 11:42:22.000000 woebin-python-0.1.4/woebin_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      211 2023-07-12 11:42:22.000000 woebin-python-0.1.4/woebin_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 11:42:22.000000 woebin-python-0.1.4/woebin_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-12 11:42:22.000000 woebin-python-0.1.4/woebin_python.egg-info/top_level.txt
```

### Comparing `woebin-python-0.1.3/PKG-INFO` & `woebin-python-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: woebin-python
-Version: 0.1.3
+Version: 0.1.4
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # woebin
```

### Comparing `woebin-python-0.1.3/README.md` & `woebin-python-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `woebin-python-0.1.3/target/release/woebin.dll` & `woebin-python-0.1.4/target/release/woebin.dll`

 * *Files 2% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180029e6c
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Wed Jul 12 11:38:22 2023
+Time/Date		Wed Jul 12 11:42:21 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	31
 SizeOfCode		000000000002ac00
 SizeOfInitializedData	000000000000c000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000029e6c
@@ -211,32 +211,32 @@
  000000018003703c:	0000000180001e20 0000000180001e57 00000001800327a4
  0000000180037048:	0000000180001e60 0000000180001e9a 00000001800327bc
  0000000180037054:	0000000180001ea0 0000000180002855 000000018003289c
  0000000180037060:	0000000180002860 0000000180002897 00000001800328c0
  000000018003706c:	00000001800028a0 00000001800028d7 00000001800328d8
  0000000180037078:	00000001800028e0 0000000180002c0c 0000000180032950
  0000000180037084:	0000000180002c10 0000000180002fcc 0000000180032968
- 0000000180037090:	0000000180002fd0 00000001800033b6 0000000180032950
- 000000018003709c:	00000001800033c0 0000000180003846 0000000180032968
- 00000001800370a8:	0000000180003850 0000000180003c22 0000000180032980
- 00000001800370b4:	0000000180003c30 0000000180003fd2 0000000180032998
+ 0000000180037090:	0000000180002fd0 0000000180003456 0000000180032968
+ 000000018003709c:	0000000180003460 0000000180003846 0000000180032950
+ 00000001800370a8:	0000000180003850 0000000180003bf2 0000000180032980
+ 00000001800370b4:	0000000180003c00 0000000180003fd2 0000000180032998
  00000001800370c0:	0000000180003fe0 0000000180004446 00000001800329b0
  00000001800370cc:	0000000180004450 0000000180004876 0000000180032950
  00000001800370d8:	0000000180004880 0000000180004e2c 00000001800329c8
  00000001800370e4:	0000000180004e30 000000018000541b 00000001800329e0
  00000001800370f0:	0000000180005420 0000000180005461 0000000180032a04
- 00000001800370fc:	0000000180005470 0000000180005784 0000000180032a64
- 0000000180037108:	0000000180005790 0000000180005a30 0000000180032a74
+ 00000001800370fc:	0000000180005470 0000000180005710 0000000180032a64
+ 0000000180037108:	0000000180005710 0000000180005a24 0000000180032a74
  0000000180037114:	0000000180005a30 0000000180005ba1 0000000180032a84
  0000000180037120:	0000000180005bb0 0000000180005be0 0000000180032aa4
  000000018003712c:	0000000180005be0 0000000180005d51 0000000180032b00
  0000000180037138:	0000000180005d60 0000000180005d90 0000000180032b20
  0000000180037144:	0000000180005d90 0000000180005e21 0000000180032b7c
- 0000000180037150:	0000000180005e30 0000000180005f01 0000000180032b88
- 000000018003715c:	0000000180005f10 0000000180005fd2 0000000180032b88
+ 0000000180037150:	0000000180005e30 0000000180005ef2 0000000180032b88
+ 000000018003715c:	0000000180005f00 0000000180005fd1 0000000180032b88
  0000000180037168:	0000000180006000 00000001800062f6 0000000180032b94
  0000000180037174:	0000000180006300 000000018000633c 0000000180032bb4
  0000000180037180:	0000000180006340 0000000180006385 0000000180032bc8
  000000018003718c:	0000000180006390 00000001800063cc 0000000180032bdc
  0000000180037198:	00000001800063d0 000000018000640c 0000000180032bf0
  00000001800371a4:	0000000180006410 000000018000662a 0000000180032c84
  00000001800371b0:	0000000180006630 0000000180006667 0000000180032ca8
@@ -328,15 +328,15 @@
  00000001800375b8:	000000018000e460 000000018000e4d8 0000000180033b84
  00000001800375c4:	000000018000e4e0 000000018000e519 0000000180033b98
  00000001800375d0:	000000018000e540 000000018000e57a 0000000180033744
  00000001800375dc:	000000018000e600 000000018000e67d 0000000180033bec
  00000001800375e8:	000000018000e680 000000018000e6b9 0000000180033c00
  00000001800375f4:	000000018000e730 000000018000e7ae 0000000180033c54
  0000000180037600:	000000018000e7b0 000000018000e7e9 0000000180033c68
- 000000018003760c:	000000018000e810 000000018000ec39 0000000180032980
+ 000000018003760c:	000000018000e810 000000018000ec39 0000000180032998
  0000000180037618:	000000018000ec40 000000018000edd6 0000000180033cbc
  0000000180037624:	000000018000ede0 000000018000ee2b 0000000180033cc4
  0000000180037630:	000000018000ee40 000000018000ef00 0000000180033020
  000000018003763c:	000000018000ef00 000000018000f01d 0000000180033b08
  0000000180037648:	000000018000f020 000000018000f033 0000000180033020
  0000000180037654:	000000018000f040 000000018000f082 0000000180033b14
  0000000180037660:	000000018000f090 000000018000f0d2 0000000180033b14
@@ -478,15 +478,15 @@
  0000000180037cc0:	00000001800186d0 000000018001870d 0000000180033020
  0000000180037ccc:	0000000180018710 0000000180018753 0000000180033020
  0000000180037cd8:	0000000180018760 00000001800187d2 00000001800331b8
  0000000180037ce4:	00000001800187e0 00000001800188c0 0000000180033020
  0000000180037cf0:	00000001800188c0 0000000180018902 0000000180033b14
  0000000180037cfc:	0000000180018940 0000000180018cf6 0000000180035044
  0000000180037d08:	0000000180018d00 0000000180018f02 0000000180034204
- 0000000180037d14:	0000000180018f10 0000000180019aef 0000000180032980
+ 0000000180037d14:	0000000180018f10 0000000180019aef 0000000180032998
  0000000180037d20:	0000000180019af0 000000018001a027 000000018003505c
  0000000180037d2c:	000000018001a030 000000018001a1d2 0000000180035074
  0000000180037d38:	000000018001a1e0 000000018001a2c1 0000000180033b08
  0000000180037d44:	000000018001a2d0 000000018001a384 0000000180032d80
  0000000180037d50:	000000018001a390 000000018001a45a 0000000180032d80
  0000000180037d5c:	000000018001a4c0 000000018001a685 0000000180035088
  0000000180037d68:	000000018001a690 000000018001a6e6 00000001800348c4
@@ -836,62 +836,51 @@
 	  pc+0x0b: push rbp
 	  pc+0x0a: push rdi
 	  pc+0x09: push rsi
 	  pc+0x08: push r12
 	  pc+0x06: push r13
 	  pc+0x04: push r14
 	  pc+0x02: push r15
- 0000000180032950 (rva: 00032950): 0000000180002fd0 - 00000001800033b6
+ 0000000180032968 also used for function at 0000000180002fd0
+ 0000000180032950 (rva: 00032950): 0000000180003460 - 0000000180003846
 	Version: 1, Flags: none
 	Nbr codes: 10, Prologue size: 0x13, Frame offset: 0x0, Frame reg: none
 	  pc+0x13: alloc large area: rsp = rsp - 0xb8
 	  pc+0x0c: push rbx
 	  pc+0x0b: push rbp
 	  pc+0x0a: push rdi
 	  pc+0x09: push rsi
 	  pc+0x08: push r12
 	  pc+0x06: push r13
 	  pc+0x04: push r14
 	  pc+0x02: push r15
- 0000000180032968 (rva: 00032968): 00000001800033c0 - 0000000180003846
+ 0000000180032980 (rva: 00032980): 0000000180003850 - 0000000180003bf2
 	Version: 1, Flags: none
 	Nbr codes: 10, Prologue size: 0x13, Frame offset: 0x0, Frame reg: none
-	  pc+0x13: alloc large area: rsp = rsp - 0x118
+	  pc+0x13: alloc large area: rsp = rsp - 0x98
 	  pc+0x0c: push rbx
 	  pc+0x0b: push rbp
 	  pc+0x0a: push rdi
 	  pc+0x09: push rsi
 	  pc+0x08: push r12
 	  pc+0x06: push r13
 	  pc+0x04: push r14
 	  pc+0x02: push r15
- 0000000180032980 (rva: 00032980): 0000000180003850 - 0000000180003c22
+ 0000000180032998 (rva: 00032998): 0000000180003c00 - 0000000180003fd2
 	Version: 1, Flags: none
 	Nbr codes: 10, Prologue size: 0x13, Frame offset: 0x0, Frame reg: none
 	  pc+0x13: alloc large area: rsp = rsp - 0xa8
 	  pc+0x0c: push rbx
 	  pc+0x0b: push rbp
 	  pc+0x0a: push rdi
 	  pc+0x09: push rsi
 	  pc+0x08: push r12
 	  pc+0x06: push r13
 	  pc+0x04: push r14
 	  pc+0x02: push r15
- 0000000180032998 (rva: 00032998): 0000000180003c30 - 0000000180003fd2
-	Version: 1, Flags: none
-	Nbr codes: 10, Prologue size: 0x13, Frame offset: 0x0, Frame reg: none
-	  pc+0x13: alloc large area: rsp = rsp - 0x98
-	  pc+0x0c: push rbx
-	  pc+0x0b: push rbp
-	  pc+0x0a: push rdi
-	  pc+0x09: push rsi
-	  pc+0x08: push r12
-	  pc+0x06: push r13
-	  pc+0x04: push r14
-	  pc+0x02: push r15
  00000001800329b0 (rva: 000329b0): 0000000180003fe0 - 0000000180004446
 	Version: 1, Flags: none
 	Nbr codes: 10, Prologue size: 0x13, Frame offset: 0x0, Frame reg: none
 	  pc+0x13: alloc large area: rsp = rsp - 0xd8
 	  pc+0x0c: push rbx
 	  pc+0x0b: push rbp
 	  pc+0x0a: push rdi
@@ -954,26 +943,26 @@
 	  pc+0x06: push rbp
 	User data:
 	  000: 22 05 93 19 01 00 00 00 44 2a 03 00 00 00 00 00
 	  010: 00 00 00 00 03 00 00 00 4c 2a 03 00 20 01 00 00
 	  020: 00 00 00 00 01 00 00 00 ff ff ff ff 20 54 00 00
 	  030: 30 4e 00 00 ff ff ff ff b1 4f 00 00 00 00 00 00
 	  040: 1a 54 00 00 ff ff ff ff
- 0000000180032a64 (rva: 00032a64): 0000000180005470 - 0000000180005784
+ 0000000180032a64 (rva: 00032a64): 0000000180005470 - 0000000180005710
 	Version: 1, Flags: none
 	Nbr codes: 6, Prologue size: 0x0c, Frame offset: 0x0, Frame reg: none
-	  pc+0x0c: alloc large area: rsp = rsp - 0xc8
+	  pc+0x0c: alloc large area: rsp = rsp - 0x88
 	  pc+0x05: push rbx
 	  pc+0x04: push rdi
 	  pc+0x03: push rsi
 	  pc+0x02: push r14
- 0000000180032a74 (rva: 00032a74): 0000000180005790 - 0000000180005a30
+ 0000000180032a74 (rva: 00032a74): 0000000180005710 - 0000000180005a24
 	Version: 1, Flags: none
 	Nbr codes: 6, Prologue size: 0x0c, Frame offset: 0x0, Frame reg: none
-	  pc+0x0c: alloc large area: rsp = rsp - 0x88
+	  pc+0x0c: alloc large area: rsp = rsp - 0xc8
 	  pc+0x05: push rbx
 	  pc+0x04: push rdi
 	  pc+0x03: push rsi
 	  pc+0x02: push r14
  0000000180032a84 (rva: 00032a84): 0000000180005a30 - 0000000180005ba1
 	Version: 1, Flags: UNW_FLAG_EHANDLER | UNW_FLAG_UHANDLER
 	Nbr codes: 9, Prologue size: 0x13, Frame offset: 0x3, Frame reg: rbp
@@ -1041,21 +1030,21 @@
  0000000180032b7c (rva: 00032b7c): 0000000180005d90 - 0000000180005e21
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x07, Frame offset: 0x0, Frame reg: none
 	  pc+0x07: alloc small area: rsp = rsp - 0x20
 	  pc+0x03: push rbx
 	  pc+0x02: push rdi
 	  pc+0x01: push rsi
- 0000000180032b88 (rva: 00032b88): 0000000180005e30 - 0000000180005f01
+ 0000000180032b88 (rva: 00032b88): 0000000180005e30 - 0000000180005ef2
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
 	  pc+0x06: alloc small area: rsp = rsp - 0x58
 	  pc+0x02: push rdi
 	  pc+0x01: push rsi
- 0000000180032b88 also used for function at 0000000180005f10
+ 0000000180032b88 also used for function at 0000000180005f00
  0000000180032b94 (rva: 00032b94): 0000000180006000 - 00000001800062f6
 	Version: 1, Flags: UNW_FLAG_EHANDLER | UNW_FLAG_UHANDLER
 	Nbr codes: 9, Prologue size: 0x17, Frame offset: 0x8, Frame reg: rbp
 	  pc+0x17: FPReg: rbp = rsp + 0x80 (info = 0x0)
 	  pc+0x0f: alloc large area: rsp = rsp - 0x158
 	  pc+0x08: push rbx
 	  pc+0x07: push rdi
@@ -2286,15 +2275,15 @@
 	  pc+0x06: push rbp
 	User data:
 	  000: 22 05 93 19 01 00 00 00 9c 3c 03 00 00 00 00 00
 	  010: 00 00 00 00 03 00 00 00 a4 3c 03 00 30 00 00 00
 	  020: 00 00 00 00 01 00 00 00 ff ff ff ff b0 e7 00 00
 	  030: 30 e7 00 00 ff ff ff ff 6b e7 00 00 00 00 00 00
 	  040: 6d e7 00 00 ff ff ff ff
- 0000000180032980 (rva: 00032980): 000000018000e810 - 000000018000ec39
+ 0000000180032998 (rva: 00032998): 000000018000e810 - 000000018000ec39
 	Version: 1, Flags: none
 	Nbr codes: 10, Prologue size: 0x13, Frame offset: 0x0, Frame reg: none
 	  pc+0x13: alloc large area: rsp = rsp - 0xa8
 	  pc+0x0c: push rbx
 	  pc+0x0b: push rbp
 	  pc+0x0a: push rdi
 	  pc+0x09: push rsi
@@ -3800,15 +3789,15 @@
 	  pc+0x0b: push rbp
 	  pc+0x0a: push rdi
 	  pc+0x09: push rsi
 	  pc+0x08: push r12
 	  pc+0x06: push r13
 	  pc+0x04: push r14
 	  pc+0x02: push r15
- 0000000180032980 (rva: 00032980): 0000000180018f10 - 0000000180019aef
+ 0000000180032998 (rva: 00032998): 0000000180018f10 - 0000000180019aef
 	Version: 1, Flags: none
 	Nbr codes: 10, Prologue size: 0x13, Frame offset: 0x0, Frame reg: none
 	  pc+0x13: alloc large area: rsp = rsp - 0xa8
 	  pc+0x0c: push rbx
 	  pc+0x0b: push rbp
 	  pc+0x0a: push rdi
 	  pc+0x09: push rsi
@@ -5604,15 +5593,15 @@
 	reloc    4 offset   a8 [360a8] DIR64
 	reloc    5 offset    0 [36000] ABSOLUTE
 
 There is a debug directory in .rdata at 0x1800321a0
 
 Type                Size     Rva      Offset
   2        CodeView 00000060 000322f4 000312f4
-(format RSDS signature cdc6a3f8db8343a1b2e6da5dcfb407e4 age 2 pdb C:\Users\alexander-o3\Development\woebin\target\release\deps\woebin.pdb)
+(format RSDS signature cdc6a3f8db8343a1b2e6da5dcfb407e4 age 3 pdb C:\Users\alexander-o3\Development\woebin\target\release\deps\woebin.pdb)
  12         Feature 00000014 00032354 00031354
  13         CoffGrp 00000318 00032368 00031368
 
 Sections:
 Idx Name          Size      VMA               LMA               File off  Algn
   0 .text         0002aae7  0000000180001000  0000000180001000  00000400  2**4
                   CONTENTS, ALLOC, LOAD, READONLY, CODE
@@ -7510,398 +7499,398 @@
    180002fd2:	push   %r14
    180002fd4:	push   %r13
    180002fd6:	push   %r12
    180002fd8:	push   %rsi
    180002fd9:	push   %rdi
    180002fda:	push   %rbp
    180002fdb:	push   %rbx
-   180002fdc:	sub    $0xb8,%rsp
+   180002fdc:	sub    $0x118,%rsp
    180002fe3:	mov    0x20(%rcx),%rbp
-   180002fe7:	movzwl 0x1c2(%rbp),%edi
-   180002fee:	lea    (%rdi,%rdx,1),%r10
-   180002ff2:	cmp    $0xb,%r10
-   180002ff6:	ja     0x180003372
-   180002ffc:	mov    %rdx,%rsi
-   180002fff:	mov    0x30(%rcx),%rbx
-   180003003:	movzwl 0x1c2(%rbx),%edx
-   18000300a:	sub    %rsi,%rdx
-   18000300d:	jb     0x18000338c
-   180003013:	mov    %r10w,0x1c2(%rbp)
-   18000301b:	mov    %dx,0x1c2(%rbx)
-   180003022:	lea    -0x1(%rsi),%r9
-   180003026:	mov    (%rbx,%rsi,8),%r11
-   18000302a:	mov    %rdx,0x48(%rsp)
-   18000302f:	mov    %r9,%r12
-   180003032:	shl    $0x5,%r12
-   180003036:	movups 0x60(%rbx,%r12,1),%xmm0
-   18000303c:	movups 0x70(%rbx,%r12,1),%xmm1
-   180003042:	movaps %xmm1,0x60(%rsp)
-   180003047:	movaps %xmm0,0x50(%rsp)
-   18000304c:	mov    0x8(%rcx),%rax
-   180003050:	mov    %rcx,0x40(%rsp)
-   180003055:	mov    0x10(%rcx),%rdx
-   180003059:	mov    0x8(%rax,%rdx,8),%r8
-   18000305e:	mov    %r11,0x8(%rax,%rdx,8)
-   180003063:	shl    $0x5,%rdx
-   180003067:	movups 0x60(%rax,%rdx,1),%xmm0
-   18000306c:	movups 0x70(%rax,%rdx,1),%xmm1
-   180003071:	movaps %xmm1,0xa0(%rsp)
-   180003079:	movaps %xmm0,0x90(%rsp)
-   180003081:	movaps 0x50(%rsp),%xmm0
-   180003086:	movaps 0x60(%rsp),%xmm1
-   18000308b:	movups %xmm1,0x70(%rax,%rdx,1)
-   180003090:	movups %xmm0,0x60(%rax,%rdx,1)
-   180003095:	movaps 0x90(%rsp),%xmm0
-   18000309d:	movaps 0xa0(%rsp),%xmm1
-   1800030a5:	movaps %xmm1,0x80(%rsp)
-   1800030ad:	movaps %xmm0,0x70(%rsp)
-   1800030b2:	mov    %r8,0x8(%rbp,%rdi,8)
-   1800030b7:	mov    %rdi,%rax
-   1800030ba:	shl    $0x5,%rax
-   1800030be:	movaps 0x70(%rsp),%xmm0
-   1800030c3:	movaps 0x80(%rsp),%xmm1
-   1800030cb:	movups %xmm1,0x70(%rbp,%rax,1)
-   1800030d0:	movups %xmm0,0x60(%rbp,%rax,1)
-   1800030d5:	mov    %rdi,0x30(%rsp)
-   1800030da:	lea    0x1(%rdi),%r13
-   1800030de:	mov    %r10,0x38(%rsp)
-   1800030e3:	mov    %r10,%rax
-   1800030e6:	sub    %r13,%rax
-   1800030e9:	cmp    %rax,%r9
-   1800030ec:	jne    0x18000339c
-   1800030f2:	lea    0x8(%rbx),%r14
-   1800030f6:	lea    0x60(%rbx),%r15
-   1800030fa:	lea    0x8(%rbp),%rax
-   1800030fe:	lea    0x60(%rbp),%rdi
-   180003102:	lea    (%rax,%r13,8),%rcx
-   180003106:	mov    %r9,0x28(%rsp)
-   18000310b:	lea    0x0(,%r9,8),%r8
-   180003113:	mov    %r14,%rdx
-   180003116:	call   0x18002a72b
-   18000311b:	mov    %r13,%rcx
-   18000311e:	shl    $0x5,%rcx
-   180003122:	add    %rdi,%rcx
-   180003125:	mov    %r15,%rdx
-   180003128:	mov    %r12,%r8
-   18000312b:	call   0x18002a72b
-   180003130:	lea    (%r14,%rsi,8),%rdx
-   180003134:	mov    0x48(%rsp),%rdi
-   180003139:	lea    0x0(,%rdi,8),%r8
-   180003141:	mov    %r14,%rcx
-   180003144:	call   0x18002a731
-   180003149:	mov    %rsi,%rdx
-   18000314c:	shl    $0x5,%rdx
-   180003150:	add    %r15,%rdx
-   180003153:	mov    %rdi,%r8
-   180003156:	shl    $0x5,%r8
-   18000315a:	mov    %r15,%rcx
-   18000315d:	call   0x18002a731
-   180003162:	mov    0x40(%rsp),%rax
-   180003167:	cmpq   $0x0,0x18(%rax)
-   18000316c:	mov    0x28(%rax),%rax
-   180003170:	je     0x18000329e
-   180003176:	test   %rax,%rax
-   180003179:	je     0x1800032a7
-   18000317f:	mov    %rdi,%r14
-   180003182:	lea    0x1c8(%rbx),%rdi
-   180003189:	lea    0x1c8(,%r13,8),%rcx
-   180003191:	add    %rbp,%rcx
-   180003194:	lea    0x0(,%rsi,8),%r8
-   18000319c:	mov    %rdi,%rdx
-   18000319f:	call   0x18002a72b
-   1800031a4:	lea    (%rbx,%rsi,8),%rdx
-   1800031a8:	add    $0x1c8,%rdx
-   1800031af:	lea    0x8(,%r14,8),%r8
-   1800031b7:	mov    %rdi,%rcx
-   1800031ba:	call   0x18002a731
-   1800031bf:	mov    0x38(%rsp),%r8
-   1800031c4:	mov    0x30(%rsp),%rax
-   1800031c9:	cmp    %rax,%r8
-   1800031cc:	jbe    0x18000327e
-   1800031d2:	and    $0x3,%rsi
-   1800031d6:	je     0x18000335e
-   1800031dc:	lea    0x1d0(,%rax,8),%rcx
-   1800031e4:	add    %rbp,%rcx
-   1800031e7:	xor    %eax,%eax
-   1800031e9:	mov    0x28(%rsp),%r9
-   1800031ee:	xchg   %ax,%ax
-   1800031f0:	mov    (%rcx,%rax,8),%rdx
-   1800031f4:	mov    %rbp,(%rdx)
-   1800031f7:	lea    (%rax,%r13,1),%edi
-   1800031fb:	mov    %di,0x1c0(%rdx)
-   180003202:	inc    %rax
-   180003205:	cmp    %rax,%rsi
-   180003208:	jne    0x1800031f0
-   18000320a:	add    %rax,%r13
-   18000320d:	cmp    $0x3,%r9
-   180003211:	jb     0x18000327e
-   180003213:	data16 data16 data16 cs nopw 0x0(%rax,%rax,1)
-   180003220:	mov    0x1c8(%rbp,%r13,8),%rax
-   180003228:	mov    %rbp,(%rax)
-   18000322b:	mov    %r13w,0x1c0(%rax)
-   180003233:	mov    0x1d0(%rbp,%r13,8),%rax
-   18000323b:	mov    %rbp,(%rax)
-   18000323e:	lea    0x1(%r13),%ecx
-   180003242:	mov    %cx,0x1c0(%rax)
-   180003249:	mov    0x1d8(%rbp,%r13,8),%rax
-   180003251:	mov    %rbp,(%rax)
-   180003254:	lea    0x2(%r13),%ecx
-   180003258:	mov    %cx,0x1c0(%rax)
-   18000325f:	mov    0x1e0(%rbp,%r13,8),%rax
-   180003267:	mov    %rbp,(%rax)
-   18000326a:	lea    0x3(%r13),%rcx
-   18000326e:	mov    %cx,0x1c0(%rax)
-   180003275:	add    $0x4,%r13
-   180003279:	cmp    %r8,%rcx
-   18000327c:	jne    0x180003220
-   18000327e:	cmp    $0xffffffffffffffff,%r14
-   180003282:	je     0x18000334a
-   180003288:	lea    0x1(%r14),%rdx
-   18000328c:	mov    %edx,%eax
-   18000328e:	and    $0x3,%eax
-   180003291:	cmp    $0x3,%r14
-   180003295:	jae    0x1800032ba
-   180003297:	xor    %ecx,%ecx
-   180003299:	jmp    0x180003320
-   18000329e:	test   %rax,%rax
-   1800032a1:	je     0x18000334a
-   1800032a7:	lea    0x29312(%rip),%rcx        # 0x18002c5c0
-   1800032ae:	lea    0x293db(%rip),%r8        # 0x18002c690
-   1800032b5:	jmp    0x1800033aa
-   1800032ba:	and    $0xfffffffffffffffc,%rdx
-   1800032be:	xor    %ecx,%ecx
-   1800032c0:	mov    0x1c8(%rbx,%rcx,8),%rbp
-   1800032c8:	mov    %rbx,0x0(%rbp)
-   1800032cc:	mov    %ecx,%edi
-   1800032ce:	mov    %cx,0x1c0(%rbp)
-   1800032d5:	mov    0x1d0(%rbx,%rcx,8),%rbp
-   1800032dd:	mov    %rbx,0x0(%rbp)
-   1800032e1:	lea    0x1(%rdi),%esi
-   1800032e4:	mov    %si,0x1c0(%rbp)
-   1800032eb:	mov    0x1d8(%rbx,%rcx,8),%rbp
-   1800032f3:	mov    %rbx,0x0(%rbp)
-   1800032f7:	lea    0x2(%rdi),%esi
-   1800032fa:	mov    %si,0x1c0(%rbp)
-   180003301:	mov    0x1e0(%rbx,%rcx,8),%rbp
-   180003309:	add    $0x4,%rcx
-   18000330d:	mov    %rbx,0x0(%rbp)
-   180003311:	add    $0x3,%edi
-   180003314:	mov    %di,0x1c0(%rbp)
-   18000331b:	cmp    %rdx,%rcx
-   18000331e:	jne    0x1800032c0
-   180003320:	test   %rax,%rax
-   180003323:	je     0x18000334a
-   180003325:	data16 cs nopw 0x0(%rax,%rax,1)
-   180003330:	mov    0x1c8(%rbx,%rcx,8),%rdx
-   180003338:	mov    %rbx,(%rdx)
-   18000333b:	mov    %cx,0x1c0(%rdx)
-   180003342:	inc    %rcx
-   180003345:	dec    %rax
-   180003348:	jne    0x180003330
-   18000334a:	add    $0xb8,%rsp
-   180003351:	pop    %rbx
-   180003352:	pop    %rbp
-   180003353:	pop    %rdi
-   180003354:	pop    %rsi
-   180003355:	pop    %r12
-   180003357:	pop    %r13
-   180003359:	pop    %r14
-   18000335b:	pop    %r15
-   18000335d:	ret
-   18000335e:	mov    0x28(%rsp),%r9
-   180003363:	cmp    $0x3,%r9
-   180003367:	jae    0x180003220
-   18000336d:	jmp    0x18000327e
-   180003372:	lea    0x29287(%rip),%rcx        # 0x18002c600
-   180003379:	lea    0x292b8(%rip),%r8        # 0x18002c638
-   180003380:	mov    $0x32,%edx
-   180003385:	call   0x18002b690
-   18000338a:	ud2
-   18000338c:	lea    0x292bd(%rip),%rcx        # 0x18002c650
-   180003393:	lea    0x292de(%rip),%r8        # 0x18002c678
-   18000339a:	jmp    0x1800033aa
-   18000339c:	lea    0x290cd(%rip),%rcx        # 0x18002c470
-   1800033a3:	lea    0x290ee(%rip),%r8        # 0x18002c498
-   1800033aa:	mov    $0x28,%edx
-   1800033af:	call   0x18002b690
-   1800033b4:	ud2
-   1800033b6:	int3
-   1800033b7:	int3
-   1800033b8:	int3
-   1800033b9:	int3
-   1800033ba:	int3
-   1800033bb:	int3
-   1800033bc:	int3
-   1800033bd:	int3
-   1800033be:	int3
-   1800033bf:	int3
-   1800033c0:	push   %r15
-   1800033c2:	push   %r14
-   1800033c4:	push   %r13
-   1800033c6:	push   %r12
-   1800033c8:	push   %rsi
-   1800033c9:	push   %rdi
-   1800033ca:	push   %rbp
-   1800033cb:	push   %rbx
-   1800033cc:	sub    $0x118,%rsp
-   1800033d3:	mov    0x20(%rcx),%rbp
-   1800033d7:	movzwl 0x322(%rbp),%edi
-   1800033de:	lea    (%rdi,%rdx,1),%r9
-   1800033e2:	cmp    $0xb,%r9
-   1800033e6:	ja     0x180003802
-   1800033ec:	mov    %rdx,%r12
-   1800033ef:	mov    0x30(%rcx),%rsi
-   1800033f3:	movzwl 0x322(%rsi),%r14d
-   1800033fb:	sub    %rdx,%r14
-   1800033fe:	jb     0x18000381c
-   180003404:	mov    %r9w,0x322(%rbp)
-   18000340c:	mov    %r14w,0x322(%rsi)
-   180003414:	lea    -0x1(%r12),%r10
-   180003419:	mov    (%rsi,%r12,8),%r11
-   18000341d:	mov    %r10,%rbx
-   180003420:	shl    $0x6,%rbx
-   180003424:	movups 0x60(%rsi,%rbx,1),%xmm0
-   180003429:	movups 0x70(%rsi,%rbx,1),%xmm1
-   18000342e:	movups 0x80(%rsi,%rbx,1),%xmm2
-   180003436:	movups 0x90(%rsi,%rbx,1),%xmm3
-   18000343e:	movaps %xmm3,0x80(%rsp)
-   180003446:	movaps %xmm2,0x70(%rsp)
-   18000344b:	movaps %xmm1,0x60(%rsp)
-   180003450:	movaps %xmm0,0x50(%rsp)
-   180003455:	mov    0x8(%rcx),%rax
-   180003459:	mov    %rcx,0x48(%rsp)
-   18000345e:	mov    0x10(%rcx),%rdx
-   180003462:	mov    0x8(%rax,%rdx,8),%r8
-   180003467:	mov    %r11,0x8(%rax,%rdx,8)
-   18000346c:	shl    $0x6,%rdx
-   180003470:	movups 0x60(%rax,%rdx,1),%xmm0
-   180003475:	movups 0x70(%rax,%rdx,1),%xmm1
-   18000347a:	movups 0x80(%rax,%rdx,1),%xmm2
-   180003482:	movups 0x90(%rax,%rdx,1),%xmm3
-   18000348a:	movaps %xmm3,0x100(%rsp)
-   180003492:	movaps %xmm2,0xf0(%rsp)
-   18000349a:	movaps %xmm1,0xe0(%rsp)
-   1800034a2:	movaps %xmm0,0xd0(%rsp)
-   1800034aa:	movaps 0x50(%rsp),%xmm0
-   1800034af:	movaps 0x60(%rsp),%xmm1
-   1800034b4:	movaps 0x70(%rsp),%xmm2
-   1800034b9:	movaps 0x80(%rsp),%xmm3
-   1800034c1:	movups %xmm3,0x90(%rax,%rdx,1)
-   1800034c9:	movups %xmm2,0x80(%rax,%rdx,1)
-   1800034d1:	movups %xmm1,0x70(%rax,%rdx,1)
-   1800034d6:	movups %xmm0,0x60(%rax,%rdx,1)
-   1800034db:	movaps 0xd0(%rsp),%xmm0
-   1800034e3:	movaps 0xe0(%rsp),%xmm1
-   1800034eb:	movaps 0xf0(%rsp),%xmm2
-   1800034f3:	movaps 0x100(%rsp),%xmm3
-   1800034fb:	movaps %xmm3,0xc0(%rsp)
-   180003503:	movaps %xmm2,0xb0(%rsp)
-   18000350b:	movaps %xmm1,0xa0(%rsp)
-   180003513:	movaps %xmm0,0x90(%rsp)
-   18000351b:	mov    %r8,0x8(%rbp,%rdi,8)
-   180003520:	mov    %rdi,%rax
-   180003523:	shl    $0x6,%rax
-   180003527:	movaps 0x90(%rsp),%xmm0
-   18000352f:	movaps 0xa0(%rsp),%xmm1
-   180003537:	movaps 0xb0(%rsp),%xmm2
-   18000353f:	movaps 0xc0(%rsp),%xmm3
-   180003547:	movups %xmm3,0x90(%rbp,%rax,1)
-   18000354f:	movups %xmm2,0x80(%rbp,%rax,1)
-   180003557:	movups %xmm1,0x70(%rbp,%rax,1)
-   18000355c:	movups %xmm0,0x60(%rbp,%rax,1)
-   180003561:	mov    %rdi,0x30(%rsp)
-   180003566:	lea    0x1(%rdi),%r13
-   18000356a:	mov    %r9,0x38(%rsp)
-   18000356f:	mov    %r9,%rax
-   180003572:	sub    %r13,%rax
-   180003575:	cmp    %rax,%r10
-   180003578:	jne    0x18000382c
-   18000357e:	lea    0x8(%rsi),%rdi
-   180003582:	lea    0x60(%rsi),%r15
-   180003586:	lea    0x8(%rbp),%rax
-   18000358a:	lea    0x60(%rbp),%rcx
-   18000358e:	mov    %rcx,0x40(%rsp)
-   180003593:	lea    (%rax,%r13,8),%rcx
-   180003597:	mov    %r10,0x28(%rsp)
-   18000359c:	lea    0x0(,%r10,8),%r8
-   1800035a4:	mov    %rdi,%rdx
-   1800035a7:	call   0x18002a72b
-   1800035ac:	mov    %r13,%rcx
-   1800035af:	shl    $0x6,%rcx
-   1800035b3:	add    0x40(%rsp),%rcx
-   1800035b8:	mov    %r15,%rdx
-   1800035bb:	mov    %rbx,%r8
-   1800035be:	call   0x18002a72b
-   1800035c3:	lea    (%rdi,%r12,8),%rdx
-   1800035c7:	lea    0x0(,%r14,8),%r8
-   1800035cf:	mov    %rdi,%rcx
-   1800035d2:	call   0x18002a731
-   1800035d7:	mov    %r12,%rdx
-   1800035da:	shl    $0x6,%rdx
-   1800035de:	add    %r15,%rdx
-   1800035e1:	mov    %r14,%r8
-   1800035e4:	shl    $0x6,%r8
-   1800035e8:	mov    %r15,%rcx
-   1800035eb:	call   0x18002a731
-   1800035f0:	mov    0x48(%rsp),%rax
-   1800035f5:	cmpq   $0x0,0x18(%rax)
-   1800035fa:	mov    0x28(%rax),%rax
-   1800035fe:	je     0x18000372e
-   180003604:	test   %rax,%rax
-   180003607:	je     0x180003737
-   18000360d:	lea    0x328(%rsi),%rdi
-   180003614:	lea    0x328(,%r13,8),%rcx
-   18000361c:	add    %rbp,%rcx
-   18000361f:	lea    0x0(,%r12,8),%r8
-   180003627:	mov    %rdi,%rdx
-   18000362a:	call   0x18002a72b
-   18000362f:	lea    (%rsi,%r12,8),%rdx
-   180003633:	add    $0x328,%rdx
-   18000363a:	lea    0x8(,%r14,8),%r8
-   180003642:	mov    %rdi,%rcx
-   180003645:	call   0x18002a731
-   18000364a:	mov    0x38(%rsp),%rdi
-   18000364f:	mov    0x30(%rsp),%rax
-   180003654:	cmp    %rax,%rdi
-   180003657:	jbe    0x18000370e
-   18000365d:	and    $0x3,%r12
-   180003661:	je     0x1800037ee
-   180003667:	lea    0x330(,%rax,8),%rcx
-   18000366f:	add    %rbp,%rcx
-   180003672:	xor    %eax,%eax
-   180003674:	mov    0x28(%rsp),%r8
-   180003679:	nopl   0x0(%rax)
+   180002fe7:	movzwl 0x322(%rbp),%edi
+   180002fee:	lea    (%rdi,%rdx,1),%r9
+   180002ff2:	cmp    $0xb,%r9
+   180002ff6:	ja     0x180003412
+   180002ffc:	mov    %rdx,%r12
+   180002fff:	mov    0x30(%rcx),%rsi
+   180003003:	movzwl 0x322(%rsi),%r14d
+   18000300b:	sub    %rdx,%r14
+   18000300e:	jb     0x18000342c
+   180003014:	mov    %r9w,0x322(%rbp)
+   18000301c:	mov    %r14w,0x322(%rsi)
+   180003024:	lea    -0x1(%r12),%r10
+   180003029:	mov    (%rsi,%r12,8),%r11
+   18000302d:	mov    %r10,%rbx
+   180003030:	shl    $0x6,%rbx
+   180003034:	movups 0x60(%rsi,%rbx,1),%xmm0
+   180003039:	movups 0x70(%rsi,%rbx,1),%xmm1
+   18000303e:	movups 0x80(%rsi,%rbx,1),%xmm2
+   180003046:	movups 0x90(%rsi,%rbx,1),%xmm3
+   18000304e:	movaps %xmm3,0x80(%rsp)
+   180003056:	movaps %xmm2,0x70(%rsp)
+   18000305b:	movaps %xmm1,0x60(%rsp)
+   180003060:	movaps %xmm0,0x50(%rsp)
+   180003065:	mov    0x8(%rcx),%rax
+   180003069:	mov    %rcx,0x48(%rsp)
+   18000306e:	mov    0x10(%rcx),%rdx
+   180003072:	mov    0x8(%rax,%rdx,8),%r8
+   180003077:	mov    %r11,0x8(%rax,%rdx,8)
+   18000307c:	shl    $0x6,%rdx
+   180003080:	movups 0x60(%rax,%rdx,1),%xmm0
+   180003085:	movups 0x70(%rax,%rdx,1),%xmm1
+   18000308a:	movups 0x80(%rax,%rdx,1),%xmm2
+   180003092:	movups 0x90(%rax,%rdx,1),%xmm3
+   18000309a:	movaps %xmm3,0x100(%rsp)
+   1800030a2:	movaps %xmm2,0xf0(%rsp)
+   1800030aa:	movaps %xmm1,0xe0(%rsp)
+   1800030b2:	movaps %xmm0,0xd0(%rsp)
+   1800030ba:	movaps 0x50(%rsp),%xmm0
+   1800030bf:	movaps 0x60(%rsp),%xmm1
+   1800030c4:	movaps 0x70(%rsp),%xmm2
+   1800030c9:	movaps 0x80(%rsp),%xmm3
+   1800030d1:	movups %xmm3,0x90(%rax,%rdx,1)
+   1800030d9:	movups %xmm2,0x80(%rax,%rdx,1)
+   1800030e1:	movups %xmm1,0x70(%rax,%rdx,1)
+   1800030e6:	movups %xmm0,0x60(%rax,%rdx,1)
+   1800030eb:	movaps 0xd0(%rsp),%xmm0
+   1800030f3:	movaps 0xe0(%rsp),%xmm1
+   1800030fb:	movaps 0xf0(%rsp),%xmm2
+   180003103:	movaps 0x100(%rsp),%xmm3
+   18000310b:	movaps %xmm3,0xc0(%rsp)
+   180003113:	movaps %xmm2,0xb0(%rsp)
+   18000311b:	movaps %xmm1,0xa0(%rsp)
+   180003123:	movaps %xmm0,0x90(%rsp)
+   18000312b:	mov    %r8,0x8(%rbp,%rdi,8)
+   180003130:	mov    %rdi,%rax
+   180003133:	shl    $0x6,%rax
+   180003137:	movaps 0x90(%rsp),%xmm0
+   18000313f:	movaps 0xa0(%rsp),%xmm1
+   180003147:	movaps 0xb0(%rsp),%xmm2
+   18000314f:	movaps 0xc0(%rsp),%xmm3
+   180003157:	movups %xmm3,0x90(%rbp,%rax,1)
+   18000315f:	movups %xmm2,0x80(%rbp,%rax,1)
+   180003167:	movups %xmm1,0x70(%rbp,%rax,1)
+   18000316c:	movups %xmm0,0x60(%rbp,%rax,1)
+   180003171:	mov    %rdi,0x30(%rsp)
+   180003176:	lea    0x1(%rdi),%r13
+   18000317a:	mov    %r9,0x38(%rsp)
+   18000317f:	mov    %r9,%rax
+   180003182:	sub    %r13,%rax
+   180003185:	cmp    %rax,%r10
+   180003188:	jne    0x18000343c
+   18000318e:	lea    0x8(%rsi),%rdi
+   180003192:	lea    0x60(%rsi),%r15
+   180003196:	lea    0x8(%rbp),%rax
+   18000319a:	lea    0x60(%rbp),%rcx
+   18000319e:	mov    %rcx,0x40(%rsp)
+   1800031a3:	lea    (%rax,%r13,8),%rcx
+   1800031a7:	mov    %r10,0x28(%rsp)
+   1800031ac:	lea    0x0(,%r10,8),%r8
+   1800031b4:	mov    %rdi,%rdx
+   1800031b7:	call   0x18002a72b
+   1800031bc:	mov    %r13,%rcx
+   1800031bf:	shl    $0x6,%rcx
+   1800031c3:	add    0x40(%rsp),%rcx
+   1800031c8:	mov    %r15,%rdx
+   1800031cb:	mov    %rbx,%r8
+   1800031ce:	call   0x18002a72b
+   1800031d3:	lea    (%rdi,%r12,8),%rdx
+   1800031d7:	lea    0x0(,%r14,8),%r8
+   1800031df:	mov    %rdi,%rcx
+   1800031e2:	call   0x18002a731
+   1800031e7:	mov    %r12,%rdx
+   1800031ea:	shl    $0x6,%rdx
+   1800031ee:	add    %r15,%rdx
+   1800031f1:	mov    %r14,%r8
+   1800031f4:	shl    $0x6,%r8
+   1800031f8:	mov    %r15,%rcx
+   1800031fb:	call   0x18002a731
+   180003200:	mov    0x48(%rsp),%rax
+   180003205:	cmpq   $0x0,0x18(%rax)
+   18000320a:	mov    0x28(%rax),%rax
+   18000320e:	je     0x18000333e
+   180003214:	test   %rax,%rax
+   180003217:	je     0x180003347
+   18000321d:	lea    0x328(%rsi),%rdi
+   180003224:	lea    0x328(,%r13,8),%rcx
+   18000322c:	add    %rbp,%rcx
+   18000322f:	lea    0x0(,%r12,8),%r8
+   180003237:	mov    %rdi,%rdx
+   18000323a:	call   0x18002a72b
+   18000323f:	lea    (%rsi,%r12,8),%rdx
+   180003243:	add    $0x328,%rdx
+   18000324a:	lea    0x8(,%r14,8),%r8
+   180003252:	mov    %rdi,%rcx
+   180003255:	call   0x18002a731
+   18000325a:	mov    0x38(%rsp),%rdi
+   18000325f:	mov    0x30(%rsp),%rax
+   180003264:	cmp    %rax,%rdi
+   180003267:	jbe    0x18000331e
+   18000326d:	and    $0x3,%r12
+   180003271:	je     0x1800033fe
+   180003277:	lea    0x330(,%rax,8),%rcx
+   18000327f:	add    %rbp,%rcx
+   180003282:	xor    %eax,%eax
+   180003284:	mov    0x28(%rsp),%r8
+   180003289:	nopl   0x0(%rax)
+   180003290:	mov    (%rcx,%rax,8),%rdx
+   180003294:	mov    %rbp,(%rdx)
+   180003297:	lea    (%rax,%r13,1),%ebx
+   18000329b:	mov    %bx,0x320(%rdx)
+   1800032a2:	inc    %rax
+   1800032a5:	cmp    %rax,%r12
+   1800032a8:	jne    0x180003290
+   1800032aa:	add    %rax,%r13
+   1800032ad:	cmp    $0x3,%r8
+   1800032b1:	jb     0x18000331e
+   1800032b3:	data16 data16 data16 cs nopw 0x0(%rax,%rax,1)
+   1800032c0:	mov    0x328(%rbp,%r13,8),%rax
+   1800032c8:	mov    %rbp,(%rax)
+   1800032cb:	mov    %r13w,0x320(%rax)
+   1800032d3:	mov    0x330(%rbp,%r13,8),%rax
+   1800032db:	mov    %rbp,(%rax)
+   1800032de:	lea    0x1(%r13),%ecx
+   1800032e2:	mov    %cx,0x320(%rax)
+   1800032e9:	mov    0x338(%rbp,%r13,8),%rax
+   1800032f1:	mov    %rbp,(%rax)
+   1800032f4:	lea    0x2(%r13),%ecx
+   1800032f8:	mov    %cx,0x320(%rax)
+   1800032ff:	mov    0x340(%rbp,%r13,8),%rax
+   180003307:	mov    %rbp,(%rax)
+   18000330a:	lea    0x3(%r13),%rcx
+   18000330e:	mov    %cx,0x320(%rax)
+   180003315:	add    $0x4,%r13
+   180003319:	cmp    %rdi,%rcx
+   18000331c:	jne    0x1800032c0
+   18000331e:	cmp    $0xffffffffffffffff,%r14
+   180003322:	je     0x1800033ea
+   180003328:	lea    0x1(%r14),%rdx
+   18000332c:	mov    %edx,%eax
+   18000332e:	and    $0x3,%eax
+   180003331:	cmp    $0x3,%r14
+   180003335:	jae    0x18000335a
+   180003337:	xor    %ecx,%ecx
+   180003339:	jmp    0x1800033c0
+   18000333e:	test   %rax,%rax
+   180003341:	je     0x1800033ea
+   180003347:	lea    0x29272(%rip),%rcx        # 0x18002c5c0
+   18000334e:	lea    0x2933b(%rip),%r8        # 0x18002c690
+   180003355:	jmp    0x18000344a
+   18000335a:	and    $0xfffffffffffffffc,%rdx
+   18000335e:	xor    %ecx,%ecx
+   180003360:	mov    0x328(%rsi,%rcx,8),%rbp
+   180003368:	mov    %rsi,0x0(%rbp)
+   18000336c:	mov    %ecx,%ebx
+   18000336e:	mov    %cx,0x320(%rbp)
+   180003375:	mov    0x330(%rsi,%rcx,8),%rbp
+   18000337d:	mov    %rsi,0x0(%rbp)
+   180003381:	lea    0x1(%rbx),%edi
+   180003384:	mov    %di,0x320(%rbp)
+   18000338b:	mov    0x338(%rsi,%rcx,8),%rbp
+   180003393:	mov    %rsi,0x0(%rbp)
+   180003397:	lea    0x2(%rbx),%edi
+   18000339a:	mov    %di,0x320(%rbp)
+   1800033a1:	mov    0x340(%rsi,%rcx,8),%rbp
+   1800033a9:	add    $0x4,%rcx
+   1800033ad:	mov    %rsi,0x0(%rbp)
+   1800033b1:	add    $0x3,%ebx
+   1800033b4:	mov    %bx,0x320(%rbp)
+   1800033bb:	cmp    %rdx,%rcx
+   1800033be:	jne    0x180003360
+   1800033c0:	test   %rax,%rax
+   1800033c3:	je     0x1800033ea
+   1800033c5:	data16 cs nopw 0x0(%rax,%rax,1)
+   1800033d0:	mov    0x328(%rsi,%rcx,8),%rdx
+   1800033d8:	mov    %rsi,(%rdx)
+   1800033db:	mov    %cx,0x320(%rdx)
+   1800033e2:	inc    %rcx
+   1800033e5:	dec    %rax
+   1800033e8:	jne    0x1800033d0
+   1800033ea:	add    $0x118,%rsp
+   1800033f1:	pop    %rbx
+   1800033f2:	pop    %rbp
+   1800033f3:	pop    %rdi
+   1800033f4:	pop    %rsi
+   1800033f5:	pop    %r12
+   1800033f7:	pop    %r13
+   1800033f9:	pop    %r14
+   1800033fb:	pop    %r15
+   1800033fd:	ret
+   1800033fe:	mov    0x28(%rsp),%r8
+   180003403:	cmp    $0x3,%r8
+   180003407:	jae    0x1800032c0
+   18000340d:	jmp    0x18000331e
+   180003412:	lea    0x291e7(%rip),%rcx        # 0x18002c600
+   180003419:	lea    0x29218(%rip),%r8        # 0x18002c638
+   180003420:	mov    $0x32,%edx
+   180003425:	call   0x18002b690
+   18000342a:	ud2
+   18000342c:	lea    0x2921d(%rip),%rcx        # 0x18002c650
+   180003433:	lea    0x2923e(%rip),%r8        # 0x18002c678
+   18000343a:	jmp    0x18000344a
+   18000343c:	lea    0x2902d(%rip),%rcx        # 0x18002c470
+   180003443:	lea    0x2904e(%rip),%r8        # 0x18002c498
+   18000344a:	mov    $0x28,%edx
+   18000344f:	call   0x18002b690
+   180003454:	ud2
+   180003456:	int3
+   180003457:	int3
+   180003458:	int3
+   180003459:	int3
+   18000345a:	int3
+   18000345b:	int3
+   18000345c:	int3
+   18000345d:	int3
+   18000345e:	int3
+   18000345f:	int3
+   180003460:	push   %r15
+   180003462:	push   %r14
+   180003464:	push   %r13
+   180003466:	push   %r12
+   180003468:	push   %rsi
+   180003469:	push   %rdi
+   18000346a:	push   %rbp
+   18000346b:	push   %rbx
+   18000346c:	sub    $0xb8,%rsp
+   180003473:	mov    0x20(%rcx),%rbp
+   180003477:	movzwl 0x1c2(%rbp),%edi
+   18000347e:	lea    (%rdi,%rdx,1),%r10
+   180003482:	cmp    $0xb,%r10
+   180003486:	ja     0x180003802
+   18000348c:	mov    %rdx,%rsi
+   18000348f:	mov    0x30(%rcx),%rbx
+   180003493:	movzwl 0x1c2(%rbx),%edx
+   18000349a:	sub    %rsi,%rdx
+   18000349d:	jb     0x18000381c
+   1800034a3:	mov    %r10w,0x1c2(%rbp)
+   1800034ab:	mov    %dx,0x1c2(%rbx)
+   1800034b2:	lea    -0x1(%rsi),%r9
+   1800034b6:	mov    (%rbx,%rsi,8),%r11
+   1800034ba:	mov    %rdx,0x48(%rsp)
+   1800034bf:	mov    %r9,%r12
+   1800034c2:	shl    $0x5,%r12
+   1800034c6:	movups 0x60(%rbx,%r12,1),%xmm0
+   1800034cc:	movups 0x70(%rbx,%r12,1),%xmm1
+   1800034d2:	movaps %xmm1,0x60(%rsp)
+   1800034d7:	movaps %xmm0,0x50(%rsp)
+   1800034dc:	mov    0x8(%rcx),%rax
+   1800034e0:	mov    %rcx,0x40(%rsp)
+   1800034e5:	mov    0x10(%rcx),%rdx
+   1800034e9:	mov    0x8(%rax,%rdx,8),%r8
+   1800034ee:	mov    %r11,0x8(%rax,%rdx,8)
+   1800034f3:	shl    $0x5,%rdx
+   1800034f7:	movups 0x60(%rax,%rdx,1),%xmm0
+   1800034fc:	movups 0x70(%rax,%rdx,1),%xmm1
+   180003501:	movaps %xmm1,0xa0(%rsp)
+   180003509:	movaps %xmm0,0x90(%rsp)
+   180003511:	movaps 0x50(%rsp),%xmm0
+   180003516:	movaps 0x60(%rsp),%xmm1
+   18000351b:	movups %xmm1,0x70(%rax,%rdx,1)
+   180003520:	movups %xmm0,0x60(%rax,%rdx,1)
+   180003525:	movaps 0x90(%rsp),%xmm0
+   18000352d:	movaps 0xa0(%rsp),%xmm1
+   180003535:	movaps %xmm1,0x80(%rsp)
+   18000353d:	movaps %xmm0,0x70(%rsp)
+   180003542:	mov    %r8,0x8(%rbp,%rdi,8)
+   180003547:	mov    %rdi,%rax
+   18000354a:	shl    $0x5,%rax
+   18000354e:	movaps 0x70(%rsp),%xmm0
+   180003553:	movaps 0x80(%rsp),%xmm1
+   18000355b:	movups %xmm1,0x70(%rbp,%rax,1)
+   180003560:	movups %xmm0,0x60(%rbp,%rax,1)
+   180003565:	mov    %rdi,0x30(%rsp)
+   18000356a:	lea    0x1(%rdi),%r13
+   18000356e:	mov    %r10,0x38(%rsp)
+   180003573:	mov    %r10,%rax
+   180003576:	sub    %r13,%rax
+   180003579:	cmp    %rax,%r9
+   18000357c:	jne    0x18000382c
+   180003582:	lea    0x8(%rbx),%r14
+   180003586:	lea    0x60(%rbx),%r15
+   18000358a:	lea    0x8(%rbp),%rax
+   18000358e:	lea    0x60(%rbp),%rdi
+   180003592:	lea    (%rax,%r13,8),%rcx
+   180003596:	mov    %r9,0x28(%rsp)
+   18000359b:	lea    0x0(,%r9,8),%r8
+   1800035a3:	mov    %r14,%rdx
+   1800035a6:	call   0x18002a72b
+   1800035ab:	mov    %r13,%rcx
+   1800035ae:	shl    $0x5,%rcx
+   1800035b2:	add    %rdi,%rcx
+   1800035b5:	mov    %r15,%rdx
+   1800035b8:	mov    %r12,%r8
+   1800035bb:	call   0x18002a72b
+   1800035c0:	lea    (%r14,%rsi,8),%rdx
+   1800035c4:	mov    0x48(%rsp),%rdi
+   1800035c9:	lea    0x0(,%rdi,8),%r8
+   1800035d1:	mov    %r14,%rcx
+   1800035d4:	call   0x18002a731
+   1800035d9:	mov    %rsi,%rdx
+   1800035dc:	shl    $0x5,%rdx
+   1800035e0:	add    %r15,%rdx
+   1800035e3:	mov    %rdi,%r8
+   1800035e6:	shl    $0x5,%r8
+   1800035ea:	mov    %r15,%rcx
+   1800035ed:	call   0x18002a731
+   1800035f2:	mov    0x40(%rsp),%rax
+   1800035f7:	cmpq   $0x0,0x18(%rax)
+   1800035fc:	mov    0x28(%rax),%rax
+   180003600:	je     0x18000372e
+   180003606:	test   %rax,%rax
+   180003609:	je     0x180003737
+   18000360f:	mov    %rdi,%r14
+   180003612:	lea    0x1c8(%rbx),%rdi
+   180003619:	lea    0x1c8(,%r13,8),%rcx
+   180003621:	add    %rbp,%rcx
+   180003624:	lea    0x0(,%rsi,8),%r8
+   18000362c:	mov    %rdi,%rdx
+   18000362f:	call   0x18002a72b
+   180003634:	lea    (%rbx,%rsi,8),%rdx
+   180003638:	add    $0x1c8,%rdx
+   18000363f:	lea    0x8(,%r14,8),%r8
+   180003647:	mov    %rdi,%rcx
+   18000364a:	call   0x18002a731
+   18000364f:	mov    0x38(%rsp),%r8
+   180003654:	mov    0x30(%rsp),%rax
+   180003659:	cmp    %rax,%r8
+   18000365c:	jbe    0x18000370e
+   180003662:	and    $0x3,%rsi
+   180003666:	je     0x1800037ee
+   18000366c:	lea    0x1d0(,%rax,8),%rcx
+   180003674:	add    %rbp,%rcx
+   180003677:	xor    %eax,%eax
+   180003679:	mov    0x28(%rsp),%r9
+   18000367e:	xchg   %ax,%ax
    180003680:	mov    (%rcx,%rax,8),%rdx
    180003684:	mov    %rbp,(%rdx)
-   180003687:	lea    (%rax,%r13,1),%ebx
-   18000368b:	mov    %bx,0x320(%rdx)
+   180003687:	lea    (%rax,%r13,1),%edi
+   18000368b:	mov    %di,0x1c0(%rdx)
    180003692:	inc    %rax
-   180003695:	cmp    %rax,%r12
+   180003695:	cmp    %rax,%rsi
    180003698:	jne    0x180003680
    18000369a:	add    %rax,%r13
-   18000369d:	cmp    $0x3,%r8
+   18000369d:	cmp    $0x3,%r9
    1800036a1:	jb     0x18000370e
    1800036a3:	data16 data16 data16 cs nopw 0x0(%rax,%rax,1)
-   1800036b0:	mov    0x328(%rbp,%r13,8),%rax
+   1800036b0:	mov    0x1c8(%rbp,%r13,8),%rax
    1800036b8:	mov    %rbp,(%rax)
-   1800036bb:	mov    %r13w,0x320(%rax)
-   1800036c3:	mov    0x330(%rbp,%r13,8),%rax
+   1800036bb:	mov    %r13w,0x1c0(%rax)
+   1800036c3:	mov    0x1d0(%rbp,%r13,8),%rax
    1800036cb:	mov    %rbp,(%rax)
    1800036ce:	lea    0x1(%r13),%ecx
-   1800036d2:	mov    %cx,0x320(%rax)
-   1800036d9:	mov    0x338(%rbp,%r13,8),%rax
+   1800036d2:	mov    %cx,0x1c0(%rax)
+   1800036d9:	mov    0x1d8(%rbp,%r13,8),%rax
    1800036e1:	mov    %rbp,(%rax)
    1800036e4:	lea    0x2(%r13),%ecx
-   1800036e8:	mov    %cx,0x320(%rax)
-   1800036ef:	mov    0x340(%rbp,%r13,8),%rax
+   1800036e8:	mov    %cx,0x1c0(%rax)
+   1800036ef:	mov    0x1e0(%rbp,%r13,8),%rax
    1800036f7:	mov    %rbp,(%rax)
    1800036fa:	lea    0x3(%r13),%rcx
-   1800036fe:	mov    %cx,0x320(%rax)
+   1800036fe:	mov    %cx,0x1c0(%rax)
    180003705:	add    $0x4,%r13
-   180003709:	cmp    %rdi,%rcx
+   180003709:	cmp    %r8,%rcx
    18000370c:	jne    0x1800036b0
    18000370e:	cmp    $0xffffffffffffffff,%r14
    180003712:	je     0x1800037da
    180003718:	lea    0x1(%r14),%rdx
    18000371c:	mov    %edx,%eax
    18000371e:	and    $0x3,%eax
    180003721:	cmp    $0x3,%r14
@@ -7911,54 +7900,54 @@
    18000372e:	test   %rax,%rax
    180003731:	je     0x1800037da
    180003737:	lea    0x28e82(%rip),%rcx        # 0x18002c5c0
    18000373e:	lea    0x28f4b(%rip),%r8        # 0x18002c690
    180003745:	jmp    0x18000383a
    18000374a:	and    $0xfffffffffffffffc,%rdx
    18000374e:	xor    %ecx,%ecx
-   180003750:	mov    0x328(%rsi,%rcx,8),%rbp
-   180003758:	mov    %rsi,0x0(%rbp)
-   18000375c:	mov    %ecx,%ebx
-   18000375e:	mov    %cx,0x320(%rbp)
-   180003765:	mov    0x330(%rsi,%rcx,8),%rbp
-   18000376d:	mov    %rsi,0x0(%rbp)
-   180003771:	lea    0x1(%rbx),%edi
-   180003774:	mov    %di,0x320(%rbp)
-   18000377b:	mov    0x338(%rsi,%rcx,8),%rbp
-   180003783:	mov    %rsi,0x0(%rbp)
-   180003787:	lea    0x2(%rbx),%edi
-   18000378a:	mov    %di,0x320(%rbp)
-   180003791:	mov    0x340(%rsi,%rcx,8),%rbp
+   180003750:	mov    0x1c8(%rbx,%rcx,8),%rbp
+   180003758:	mov    %rbx,0x0(%rbp)
+   18000375c:	mov    %ecx,%edi
+   18000375e:	mov    %cx,0x1c0(%rbp)
+   180003765:	mov    0x1d0(%rbx,%rcx,8),%rbp
+   18000376d:	mov    %rbx,0x0(%rbp)
+   180003771:	lea    0x1(%rdi),%esi
+   180003774:	mov    %si,0x1c0(%rbp)
+   18000377b:	mov    0x1d8(%rbx,%rcx,8),%rbp
+   180003783:	mov    %rbx,0x0(%rbp)
+   180003787:	lea    0x2(%rdi),%esi
+   18000378a:	mov    %si,0x1c0(%rbp)
+   180003791:	mov    0x1e0(%rbx,%rcx,8),%rbp
    180003799:	add    $0x4,%rcx
-   18000379d:	mov    %rsi,0x0(%rbp)
-   1800037a1:	add    $0x3,%ebx
-   1800037a4:	mov    %bx,0x320(%rbp)
+   18000379d:	mov    %rbx,0x0(%rbp)
+   1800037a1:	add    $0x3,%edi
+   1800037a4:	mov    %di,0x1c0(%rbp)
    1800037ab:	cmp    %rdx,%rcx
    1800037ae:	jne    0x180003750
    1800037b0:	test   %rax,%rax
    1800037b3:	je     0x1800037da
    1800037b5:	data16 cs nopw 0x0(%rax,%rax,1)
-   1800037c0:	mov    0x328(%rsi,%rcx,8),%rdx
-   1800037c8:	mov    %rsi,(%rdx)
-   1800037cb:	mov    %cx,0x320(%rdx)
+   1800037c0:	mov    0x1c8(%rbx,%rcx,8),%rdx
+   1800037c8:	mov    %rbx,(%rdx)
+   1800037cb:	mov    %cx,0x1c0(%rdx)
    1800037d2:	inc    %rcx
    1800037d5:	dec    %rax
    1800037d8:	jne    0x1800037c0
-   1800037da:	add    $0x118,%rsp
+   1800037da:	add    $0xb8,%rsp
    1800037e1:	pop    %rbx
    1800037e2:	pop    %rbp
    1800037e3:	pop    %rdi
    1800037e4:	pop    %rsi
    1800037e5:	pop    %r12
    1800037e7:	pop    %r13
    1800037e9:	pop    %r14
    1800037eb:	pop    %r15
    1800037ed:	ret
-   1800037ee:	mov    0x28(%rsp),%r8
-   1800037f3:	cmp    $0x3,%r8
+   1800037ee:	mov    0x28(%rsp),%r9
+   1800037f3:	cmp    $0x3,%r9
    1800037f7:	jae    0x1800036b0
    1800037fd:	jmp    0x18000370e
    180003802:	lea    0x28df7(%rip),%rcx        # 0x18002c600
    180003809:	lea    0x28e28(%rip),%r8        # 0x18002c638
    180003810:	mov    $0x32,%edx
    180003815:	call   0x18002b690
    18000381a:	ud2
@@ -7984,425 +7973,425 @@
    180003852:	push   %r14
    180003854:	push   %r13
    180003856:	push   %r12
    180003858:	push   %rsi
    180003859:	push   %rdi
    18000385a:	push   %rbp
    18000385b:	push   %rbx
-   18000385c:	sub    $0xa8,%rsp
+   18000385c:	sub    $0x98,%rsp
    180003863:	mov    0x20(%rcx),%rbp
    180003867:	mov    0x30(%rcx),%rax
-   18000386b:	movzwl 0x322(%rbp),%r12d
+   18000386b:	movzwl 0x1c2(%rbp),%r12d
    180003873:	mov    %rax,0x38(%rsp)
-   180003878:	movzwl 0x322(%rax),%eax
-   18000387f:	mov    %ax,0x26(%rsp)
+   180003878:	movzwl 0x1c2(%rax),%eax
+   18000387f:	mov    %ax,0x2e(%rsp)
    180003884:	movzwl %ax,%eax
-   180003887:	mov    %rax,0x30(%rsp)
-   18000388c:	lea    (%r12,%rax,1),%rdx
-   180003890:	inc    %rdx
-   180003893:	cmp    $0xb,%rdx
-   180003897:	ja     0x180003c08
-   18000389d:	mov    (%rcx),%rax
-   1800038a0:	mov    %rax,0x58(%rsp)
-   1800038a5:	mov    0x8(%rcx),%rbx
-   1800038a9:	movzwl 0x322(%rbx),%r13d
-   1800038b1:	lea    0x1(%r12),%r15
-   1800038b6:	mov    0x10(%rcx),%rsi
-   1800038ba:	mov    %rdx,0x48(%rsp)
-   1800038bf:	mov    %dx,0x322(%rbp)
-   1800038c6:	lea    0x8(%rbx,%rsi,8),%rcx
-   1800038cb:	mov    0x8(%rbx,%rsi,8),%rax
-   1800038d0:	mov    %rax,0x28(%rsp)
-   1800038d5:	lea    0x1(%rsi),%r14
-   1800038d9:	lea    (%rbx,%rsi,8),%rdx
-   1800038dd:	add    $0x10,%rdx
-   1800038e1:	mov    %rsi,%rdi
-   1800038e4:	not    %rdi
-   1800038e7:	add    %r13,%rdi
-   1800038ea:	lea    0x0(,%rdi,8),%r8
-   1800038f2:	mov    %r8,0x50(%rsp)
-   1800038f7:	call   0x18002a731
-   1800038fc:	mov    0x28(%rsp),%rax
-   180003901:	mov    %rax,0x8(%rbp,%r12,8)
-   180003906:	mov    0x38(%rsp),%rax
-   18000390b:	lea    0x8(%rax),%rdx
-   18000390f:	lea    0x8(%rbp,%r15,8),%rcx
-   180003914:	mov    0x30(%rsp),%rax
-   180003919:	lea    0x0(,%rax,8),%r8
-   180003921:	mov    %r8,0x40(%rsp)
-   180003926:	call   0x18002a72b
-   18000392b:	mov    %rsi,%rax
-   18000392e:	shl    $0x6,%rax
-   180003932:	lea    (%rbx,%rax,1),%rcx
-   180003936:	add    $0x60,%rcx
-   18000393a:	movups 0x60(%rbx,%rax,1),%xmm0
-   18000393f:	movups 0x70(%rbx,%rax,1),%xmm1
-   180003944:	movups 0x80(%rbx,%rax,1),%xmm2
-   18000394c:	movups 0x90(%rbx,%rax,1),%xmm3
-   180003954:	movaps %xmm3,0x90(%rsp)
-   18000395c:	movaps %xmm2,0x80(%rsp)
-   180003964:	movaps %xmm1,0x70(%rsp)
-   180003969:	movaps %xmm0,0x60(%rsp)
-   18000396e:	mov    %r14,%rax
-   180003971:	shl    $0x6,%rax
-   180003975:	lea    (%rbx,%rax,1),%rdx
-   180003979:	add    $0x60,%rdx
-   18000397d:	shl    $0x6,%rdi
-   180003981:	mov    %rdi,%r8
-   180003984:	call   0x18002a731
-   180003989:	mov    %r12,0x28(%rsp)
-   18000398e:	shl    $0x6,%r12
-   180003992:	movaps 0x60(%rsp),%xmm0
-   180003997:	movaps 0x70(%rsp),%xmm1
-   18000399c:	movaps 0x80(%rsp),%xmm2
-   1800039a4:	movaps 0x90(%rsp),%xmm3
-   1800039ac:	movups %xmm0,0x60(%rbp,%r12,1)
-   1800039b2:	movups %xmm1,0x70(%rbp,%r12,1)
-   1800039b8:	movups %xmm2,0x80(%rbp,%r12,1)
-   1800039c1:	movups %xmm3,0x90(%rbp,%r12,1)
-   1800039ca:	mov    0x38(%rsp),%r12
-   1800039cf:	lea    0x60(%r12),%rdx
-   1800039d4:	mov    %r15,%rax
-   1800039d7:	shl    $0x6,%rax
-   1800039db:	lea    (%rax,%rbp,1),%rcx
-   1800039df:	add    $0x60,%rcx
-   1800039e3:	mov    0x30(%rsp),%r8
-   1800039e8:	shl    $0x6,%r8
-   1800039ec:	call   0x18002a72b
-   1800039f1:	lea    (%rbx,%rsi,8),%rdi
-   1800039f5:	add    $0x330,%rdi
-   1800039fc:	lea    (%rbx,%rsi,8),%rdx
-   180003a00:	add    $0x338,%rdx
-   180003a07:	mov    %rdi,%rcx
-   180003a0a:	mov    0x50(%rsp),%r8
-   180003a0f:	call   0x18002a731
-   180003a14:	cmp    %r13,%r14
-   180003a17:	jae    0x180003ace
-   180003a1d:	mov    %esi,%eax
-   180003a1f:	not    %eax
-   180003a21:	lea    (%rax,%r13,1),%ecx
-   180003a25:	mov    %r13,%r8
-   180003a28:	sub    %rsi,%r8
-   180003a2b:	add    $0xfffffffffffffffe,%r8
-   180003a2f:	and    $0x3,%rcx
-   180003a33:	je     0x180003a5d
-   180003a35:	xor    %edx,%edx
-   180003a37:	nopw   0x0(%rax,%rax,1)
-   180003a40:	mov    (%rdi,%rdx,8),%rsi
-   180003a44:	mov    %rbx,(%rsi)
-   180003a47:	lea    (%r14,%rdx,1),%eax
-   180003a4b:	mov    %ax,0x320(%rsi)
-   180003a52:	inc    %rdx
-   180003a55:	cmp    %rdx,%rcx
-   180003a58:	jne    0x180003a40
-   180003a5a:	add    %rdx,%r14
-   180003a5d:	cmp    $0x3,%r8
-   180003a61:	jb     0x180003ace
-   180003a63:	data16 data16 data16 cs nopw 0x0(%rax,%rax,1)
-   180003a70:	mov    0x328(%rbx,%r14,8),%rax
-   180003a78:	mov    %rbx,(%rax)
-   180003a7b:	mov    %r14w,0x320(%rax)
-   180003a83:	mov    0x330(%rbx,%r14,8),%rax
-   180003a8b:	mov    %rbx,(%rax)
-   180003a8e:	lea    0x1(%r14),%ecx
-   180003a92:	mov    %cx,0x320(%rax)
-   180003a99:	mov    0x338(%rbx,%r14,8),%rax
-   180003aa1:	mov    %rbx,(%rax)
-   180003aa4:	lea    0x2(%r14),%ecx
-   180003aa8:	mov    %cx,0x320(%rax)
-   180003aaf:	mov    0x340(%rbx,%r14,8),%rax
-   180003ab7:	mov    %rbx,(%rax)
-   180003aba:	lea    0x3(%r14),%ecx
-   180003abe:	mov    %cx,0x320(%rax)
-   180003ac5:	add    $0x4,%r14
-   180003ac9:	cmp    %r13,%r14
-   180003acc:	jne    0x180003a70
-   180003ace:	decw   0x322(%rbx)
-   180003ad5:	mov    $0x8,%r14d
-   180003adb:	mov    $0x328,%edx
-   180003ae0:	mov    0x58(%rsp),%r13
-   180003ae5:	cmp    $0x2,%r13
-   180003ae9:	jb     0x180003be3
-   180003aef:	lea    0x328(%r12),%rdx
-   180003af7:	lea    0x328(,%r15,8),%rcx
-   180003aff:	add    %rbp,%rcx
-   180003b02:	mov    0x40(%rsp),%r8
-   180003b07:	add    $0x8,%r8
-   180003b0b:	call   0x18002a72b
-   180003b10:	mov    $0x388,%edx
-   180003b15:	mov    0x48(%rsp),%r8
-   180003b1a:	mov    0x28(%rsp),%rax
-   180003b1f:	cmp    %rax,%r8
-   180003b22:	jbe    0x180003be3
-   180003b28:	mov    0x30(%rsp),%rsi
-   180003b2d:	inc    %esi
-   180003b2f:	and    $0x3,%rsi
-   180003b33:	je     0x180003b6d
-   180003b35:	lea    0x330(,%rax,8),%rcx
-   180003b3d:	add    %rbp,%rcx
-   180003b40:	xor    %eax,%eax
-   180003b42:	data16 data16 data16 data16 cs nopw 0x0(%rax,%rax,1)
-   180003b50:	mov    (%rcx,%rax,8),%rdx
-   180003b54:	mov    %rbp,(%rdx)
-   180003b57:	lea    (%r15,%rax,1),%edi
-   180003b5b:	mov    %di,0x320(%rdx)
-   180003b62:	inc    %rax
-   180003b65:	cmp    %rax,%rsi
-   180003b68:	jne    0x180003b50
-   180003b6a:	add    %rax,%r15
-   180003b6d:	mov    $0x388,%edx
-   180003b72:	cmpw   $0x3,0x26(%rsp)
-   180003b78:	jb     0x180003be3
-   180003b7a:	nopw   0x0(%rax,%rax,1)
-   180003b80:	mov    0x328(%rbp,%r15,8),%rax
-   180003b88:	mov    %rbp,(%rax)
-   180003b8b:	mov    %r15w,0x320(%rax)
-   180003b93:	mov    0x330(%rbp,%r15,8),%rax
-   180003b9b:	mov    %rbp,(%rax)
-   180003b9e:	lea    0x1(%r15),%ecx
-   180003ba2:	mov    %cx,0x320(%rax)
-   180003ba9:	mov    0x338(%rbp,%r15,8),%rax
-   180003bb1:	mov    %rbp,(%rax)
-   180003bb4:	lea    0x2(%r15),%ecx
-   180003bb8:	mov    %cx,0x320(%rax)
-   180003bbf:	mov    0x340(%rbp,%r15,8),%rax
-   180003bc7:	mov    %rbp,(%rax)
-   180003bca:	lea    0x3(%r15),%rcx
-   180003bce:	mov    %cx,0x320(%rax)
-   180003bd5:	add    $0x4,%r15
-   180003bd9:	cmp    %r8,%rcx
-   180003bdc:	jne    0x180003b80
-   180003bde:	mov    $0x388,%edx
-   180003be3:	mov    %r12,%rcx
-   180003be6:	mov    %r14,%r8
-   180003be9:	call   0x18000df80
-   180003bee:	mov    %r13,%rax
-   180003bf1:	mov    %rbx,%rdx
-   180003bf4:	add    $0xa8,%rsp
-   180003bfb:	pop    %rbx
-   180003bfc:	pop    %rbp
-   180003bfd:	pop    %rdi
-   180003bfe:	pop    %rsi
-   180003bff:	pop    %r12
-   180003c01:	pop    %r13
-   180003c03:	pop    %r14
-   180003c05:	pop    %r15
-   180003c07:	ret
-   180003c08:	lea    0x28b49(%rip),%rcx        # 0x18002c758
-   180003c0f:	lea    0x28b72(%rip),%r8        # 0x18002c788
-   180003c16:	mov    $0x2a,%edx
-   180003c1b:	call   0x18002b690
-   180003c20:	ud2
-   180003c22:	int3
-   180003c23:	int3
-   180003c24:	int3
-   180003c25:	int3
-   180003c26:	int3
-   180003c27:	int3
-   180003c28:	int3
-   180003c29:	int3
-   180003c2a:	int3
-   180003c2b:	int3
-   180003c2c:	int3
-   180003c2d:	int3
-   180003c2e:	int3
-   180003c2f:	int3
-   180003c30:	push   %r15
-   180003c32:	push   %r14
-   180003c34:	push   %r13
-   180003c36:	push   %r12
-   180003c38:	push   %rsi
-   180003c39:	push   %rdi
-   180003c3a:	push   %rbp
-   180003c3b:	push   %rbx
-   180003c3c:	sub    $0x98,%rsp
-   180003c43:	mov    0x20(%rcx),%rbp
-   180003c47:	mov    0x30(%rcx),%rax
-   180003c4b:	movzwl 0x1c2(%rbp),%r12d
-   180003c53:	mov    %rax,0x38(%rsp)
-   180003c58:	movzwl 0x1c2(%rax),%eax
-   180003c5f:	mov    %ax,0x2e(%rsp)
-   180003c64:	movzwl %ax,%eax
-   180003c67:	lea    (%r12,%rax,1),%rdx
-   180003c6b:	inc    %rdx
-   180003c6e:	cmp    $0xb,%rdx
-   180003c72:	ja     0x180003fb8
-   180003c78:	mov    %rax,%r13
-   180003c7b:	mov    (%rcx),%rax
-   180003c7e:	mov    %rax,0x68(%rsp)
-   180003c83:	mov    0x8(%rcx),%rbx
-   180003c87:	movzwl 0x1c2(%rbx),%eax
-   180003c8e:	mov    %rax,0x60(%rsp)
-   180003c93:	lea    0x1(%r12),%r15
-   180003c98:	mov    0x10(%rcx),%rsi
-   180003c9c:	mov    %rdx,0x50(%rsp)
-   180003ca1:	mov    %dx,0x1c2(%rbp)
-   180003ca8:	lea    0x8(%rbx,%rsi,8),%rcx
-   180003cad:	mov    0x8(%rbx,%rsi,8),%rdx
-   180003cb2:	mov    %rdx,0x30(%rsp)
-   180003cb7:	lea    0x1(%rsi),%r14
-   180003cbb:	lea    (%rbx,%rsi,8),%rdx
-   180003cbf:	add    $0x10,%rdx
-   180003cc3:	mov    %rsi,%rdi
-   180003cc6:	not    %rdi
-   180003cc9:	add    %rax,%rdi
-   180003ccc:	lea    0x0(,%rdi,8),%r8
-   180003cd4:	mov    %r8,0x58(%rsp)
-   180003cd9:	call   0x18002a731
-   180003cde:	mov    0x30(%rsp),%rax
-   180003ce3:	mov    %rax,0x8(%rbp,%r12,8)
-   180003ce8:	mov    0x38(%rsp),%rax
-   180003ced:	lea    0x8(%rax),%rdx
-   180003cf1:	lea    0x8(,%r15,8),%rcx
-   180003cf9:	add    %rbp,%rcx
-   180003cfc:	lea    0x0(,%r13,8),%r8
-   180003d04:	mov    %r8,0x48(%rsp)
-   180003d09:	call   0x18002a72b
-   180003d0e:	mov    %rsi,%rax
-   180003d11:	shl    $0x5,%rax
-   180003d15:	lea    (%rbx,%rax,1),%rcx
-   180003d19:	add    $0x60,%rcx
-   180003d1d:	movups 0x60(%rbx,%rax,1),%xmm0
-   180003d22:	movups 0x70(%rbx,%rax,1),%xmm1
-   180003d27:	movaps %xmm1,0x80(%rsp)
-   180003d2f:	movaps %xmm0,0x70(%rsp)
-   180003d34:	mov    %r14,%rax
-   180003d37:	shl    $0x5,%rax
-   180003d3b:	lea    (%rbx,%rax,1),%rdx
-   180003d3f:	add    $0x60,%rdx
-   180003d43:	shl    $0x5,%rdi
-   180003d47:	mov    %rdi,%r8
-   180003d4a:	call   0x18002a731
-   180003d4f:	mov    %r12,0x30(%rsp)
-   180003d54:	shl    $0x5,%r12
-   180003d58:	movaps 0x70(%rsp),%xmm0
-   180003d5d:	movaps 0x80(%rsp),%xmm1
-   180003d65:	movups %xmm0,0x60(%rbp,%r12,1)
-   180003d6b:	movups %xmm1,0x70(%rbp,%r12,1)
-   180003d71:	mov    0x38(%rsp),%r12
-   180003d76:	lea    0x60(%r12),%rdx
-   180003d7b:	mov    %r15,%rax
-   180003d7e:	shl    $0x5,%rax
-   180003d82:	lea    (%rax,%rbp,1),%rcx
-   180003d86:	add    $0x60,%rcx
-   180003d8a:	mov    %r13,0x40(%rsp)
-   180003d8f:	shl    $0x5,%r13
-   180003d93:	mov    %r13,%r8
-   180003d96:	call   0x18002a72b
-   180003d9b:	lea    (%rbx,%rsi,8),%rdi
-   180003d9f:	add    $0x1d0,%rdi
-   180003da6:	lea    (%rbx,%rsi,8),%rdx
-   180003daa:	add    $0x1d8,%rdx
-   180003db1:	mov    %rdi,%rcx
-   180003db4:	mov    0x58(%rsp),%r8
-   180003db9:	call   0x18002a731
-   180003dbe:	mov    0x60(%rsp),%r9
-   180003dc3:	cmp    %r9,%r14
-   180003dc6:	jae    0x180003e7e
-   180003dcc:	mov    %esi,%eax
-   180003dce:	not    %eax
-   180003dd0:	lea    (%r9,%rax,1),%ecx
-   180003dd4:	mov    %r9,%r8
-   180003dd7:	sub    %rsi,%r8
-   180003dda:	add    $0xfffffffffffffffe,%r8
-   180003dde:	and    $0x3,%rcx
-   180003de2:	je     0x180003e0d
-   180003de4:	xor    %edx,%edx
-   180003de6:	cs nopw 0x0(%rax,%rax,1)
+   180003887:	lea    (%r12,%rax,1),%rdx
+   18000388b:	inc    %rdx
+   18000388e:	cmp    $0xb,%rdx
+   180003892:	ja     0x180003bd8
+   180003898:	mov    %rax,%r13
+   18000389b:	mov    (%rcx),%rax
+   18000389e:	mov    %rax,0x68(%rsp)
+   1800038a3:	mov    0x8(%rcx),%rbx
+   1800038a7:	movzwl 0x1c2(%rbx),%eax
+   1800038ae:	mov    %rax,0x60(%rsp)
+   1800038b3:	lea    0x1(%r12),%r15
+   1800038b8:	mov    0x10(%rcx),%rsi
+   1800038bc:	mov    %rdx,0x50(%rsp)
+   1800038c1:	mov    %dx,0x1c2(%rbp)
+   1800038c8:	lea    0x8(%rbx,%rsi,8),%rcx
+   1800038cd:	mov    0x8(%rbx,%rsi,8),%rdx
+   1800038d2:	mov    %rdx,0x30(%rsp)
+   1800038d7:	lea    0x1(%rsi),%r14
+   1800038db:	lea    (%rbx,%rsi,8),%rdx
+   1800038df:	add    $0x10,%rdx
+   1800038e3:	mov    %rsi,%rdi
+   1800038e6:	not    %rdi
+   1800038e9:	add    %rax,%rdi
+   1800038ec:	lea    0x0(,%rdi,8),%r8
+   1800038f4:	mov    %r8,0x58(%rsp)
+   1800038f9:	call   0x18002a731
+   1800038fe:	mov    0x30(%rsp),%rax
+   180003903:	mov    %rax,0x8(%rbp,%r12,8)
+   180003908:	mov    0x38(%rsp),%rax
+   18000390d:	lea    0x8(%rax),%rdx
+   180003911:	lea    0x8(,%r15,8),%rcx
+   180003919:	add    %rbp,%rcx
+   18000391c:	lea    0x0(,%r13,8),%r8
+   180003924:	mov    %r8,0x48(%rsp)
+   180003929:	call   0x18002a72b
+   18000392e:	mov    %rsi,%rax
+   180003931:	shl    $0x5,%rax
+   180003935:	lea    (%rbx,%rax,1),%rcx
+   180003939:	add    $0x60,%rcx
+   18000393d:	movups 0x60(%rbx,%rax,1),%xmm0
+   180003942:	movups 0x70(%rbx,%rax,1),%xmm1
+   180003947:	movaps %xmm1,0x80(%rsp)
+   18000394f:	movaps %xmm0,0x70(%rsp)
+   180003954:	mov    %r14,%rax
+   180003957:	shl    $0x5,%rax
+   18000395b:	lea    (%rbx,%rax,1),%rdx
+   18000395f:	add    $0x60,%rdx
+   180003963:	shl    $0x5,%rdi
+   180003967:	mov    %rdi,%r8
+   18000396a:	call   0x18002a731
+   18000396f:	mov    %r12,0x30(%rsp)
+   180003974:	shl    $0x5,%r12
+   180003978:	movaps 0x70(%rsp),%xmm0
+   18000397d:	movaps 0x80(%rsp),%xmm1
+   180003985:	movups %xmm0,0x60(%rbp,%r12,1)
+   18000398b:	movups %xmm1,0x70(%rbp,%r12,1)
+   180003991:	mov    0x38(%rsp),%r12
+   180003996:	lea    0x60(%r12),%rdx
+   18000399b:	mov    %r15,%rax
+   18000399e:	shl    $0x5,%rax
+   1800039a2:	lea    (%rax,%rbp,1),%rcx
+   1800039a6:	add    $0x60,%rcx
+   1800039aa:	mov    %r13,0x40(%rsp)
+   1800039af:	shl    $0x5,%r13
+   1800039b3:	mov    %r13,%r8
+   1800039b6:	call   0x18002a72b
+   1800039bb:	lea    (%rbx,%rsi,8),%rdi
+   1800039bf:	add    $0x1d0,%rdi
+   1800039c6:	lea    (%rbx,%rsi,8),%rdx
+   1800039ca:	add    $0x1d8,%rdx
+   1800039d1:	mov    %rdi,%rcx
+   1800039d4:	mov    0x58(%rsp),%r8
+   1800039d9:	call   0x18002a731
+   1800039de:	mov    0x60(%rsp),%r9
+   1800039e3:	cmp    %r9,%r14
+   1800039e6:	jae    0x180003a9e
+   1800039ec:	mov    %esi,%eax
+   1800039ee:	not    %eax
+   1800039f0:	lea    (%r9,%rax,1),%ecx
+   1800039f4:	mov    %r9,%r8
+   1800039f7:	sub    %rsi,%r8
+   1800039fa:	add    $0xfffffffffffffffe,%r8
+   1800039fe:	and    $0x3,%rcx
+   180003a02:	je     0x180003a2d
+   180003a04:	xor    %edx,%edx
+   180003a06:	cs nopw 0x0(%rax,%rax,1)
+   180003a10:	mov    (%rdi,%rdx,8),%rsi
+   180003a14:	mov    %rbx,(%rsi)
+   180003a17:	lea    (%r14,%rdx,1),%eax
+   180003a1b:	mov    %ax,0x1c0(%rsi)
+   180003a22:	inc    %rdx
+   180003a25:	cmp    %rdx,%rcx
+   180003a28:	jne    0x180003a10
+   180003a2a:	add    %rdx,%r14
+   180003a2d:	cmp    $0x3,%r8
+   180003a31:	jb     0x180003a9e
+   180003a33:	data16 data16 data16 cs nopw 0x0(%rax,%rax,1)
+   180003a40:	mov    0x1c8(%rbx,%r14,8),%rax
+   180003a48:	mov    %rbx,(%rax)
+   180003a4b:	mov    %r14w,0x1c0(%rax)
+   180003a53:	mov    0x1d0(%rbx,%r14,8),%rax
+   180003a5b:	mov    %rbx,(%rax)
+   180003a5e:	lea    0x1(%r14),%ecx
+   180003a62:	mov    %cx,0x1c0(%rax)
+   180003a69:	mov    0x1d8(%rbx,%r14,8),%rax
+   180003a71:	mov    %rbx,(%rax)
+   180003a74:	lea    0x2(%r14),%ecx
+   180003a78:	mov    %cx,0x1c0(%rax)
+   180003a7f:	mov    0x1e0(%rbx,%r14,8),%rax
+   180003a87:	mov    %rbx,(%rax)
+   180003a8a:	lea    0x3(%r14),%ecx
+   180003a8e:	mov    %cx,0x1c0(%rax)
+   180003a95:	add    $0x4,%r14
+   180003a99:	cmp    %r9,%r14
+   180003a9c:	jne    0x180003a40
+   180003a9e:	decw   0x1c2(%rbx)
+   180003aa5:	mov    $0x8,%r14d
+   180003aab:	mov    $0x1c8,%edx
+   180003ab0:	mov    0x68(%rsp),%r13
+   180003ab5:	cmp    $0x1,%r13
+   180003ab9:	jbe    0x180003bb3
+   180003abf:	lea    0x1c8(%r12),%rdx
+   180003ac7:	lea    0x1c8(,%r15,8),%rcx
+   180003acf:	add    %rbp,%rcx
+   180003ad2:	mov    0x48(%rsp),%r8
+   180003ad7:	add    $0x8,%r8
+   180003adb:	call   0x18002a72b
+   180003ae0:	mov    $0x228,%edx
+   180003ae5:	mov    0x50(%rsp),%r8
+   180003aea:	mov    0x30(%rsp),%rax
+   180003aef:	cmp    %rax,%r8
+   180003af2:	jbe    0x180003bb3
+   180003af8:	mov    0x40(%rsp),%rsi
+   180003afd:	inc    %esi
+   180003aff:	and    $0x3,%rsi
+   180003b03:	je     0x180003b3d
+   180003b05:	lea    0x1d0(,%rax,8),%rcx
+   180003b0d:	add    %rbp,%rcx
+   180003b10:	xor    %eax,%eax
+   180003b12:	data16 data16 data16 data16 cs nopw 0x0(%rax,%rax,1)
+   180003b20:	mov    (%rcx,%rax,8),%rdx
+   180003b24:	mov    %rbp,(%rdx)
+   180003b27:	lea    (%r15,%rax,1),%edi
+   180003b2b:	mov    %di,0x1c0(%rdx)
+   180003b32:	inc    %rax
+   180003b35:	cmp    %rax,%rsi
+   180003b38:	jne    0x180003b20
+   180003b3a:	add    %rax,%r15
+   180003b3d:	mov    $0x228,%edx
+   180003b42:	cmpw   $0x3,0x2e(%rsp)
+   180003b48:	jb     0x180003bb3
+   180003b4a:	nopw   0x0(%rax,%rax,1)
+   180003b50:	mov    0x1c8(%rbp,%r15,8),%rax
+   180003b58:	mov    %rbp,(%rax)
+   180003b5b:	mov    %r15w,0x1c0(%rax)
+   180003b63:	mov    0x1d0(%rbp,%r15,8),%rax
+   180003b6b:	mov    %rbp,(%rax)
+   180003b6e:	lea    0x1(%r15),%ecx
+   180003b72:	mov    %cx,0x1c0(%rax)
+   180003b79:	mov    0x1d8(%rbp,%r15,8),%rax
+   180003b81:	mov    %rbp,(%rax)
+   180003b84:	lea    0x2(%r15),%ecx
+   180003b88:	mov    %cx,0x1c0(%rax)
+   180003b8f:	mov    0x1e0(%rbp,%r15,8),%rax
+   180003b97:	mov    %rbp,(%rax)
+   180003b9a:	lea    0x3(%r15),%rcx
+   180003b9e:	mov    %cx,0x1c0(%rax)
+   180003ba5:	add    $0x4,%r15
+   180003ba9:	cmp    %r8,%rcx
+   180003bac:	jne    0x180003b50
+   180003bae:	mov    $0x228,%edx
+   180003bb3:	mov    %r12,%rcx
+   180003bb6:	mov    %r14,%r8
+   180003bb9:	call   0x18000df80
+   180003bbe:	mov    %r13,%rax
+   180003bc1:	mov    %rbx,%rdx
+   180003bc4:	add    $0x98,%rsp
+   180003bcb:	pop    %rbx
+   180003bcc:	pop    %rbp
+   180003bcd:	pop    %rdi
+   180003bce:	pop    %rsi
+   180003bcf:	pop    %r12
+   180003bd1:	pop    %r13
+   180003bd3:	pop    %r14
+   180003bd5:	pop    %r15
+   180003bd7:	ret
+   180003bd8:	lea    0x28b79(%rip),%rcx        # 0x18002c758
+   180003bdf:	lea    0x28ba2(%rip),%r8        # 0x18002c788
+   180003be6:	mov    $0x2a,%edx
+   180003beb:	call   0x18002b690
+   180003bf0:	ud2
+   180003bf2:	int3
+   180003bf3:	int3
+   180003bf4:	int3
+   180003bf5:	int3
+   180003bf6:	int3
+   180003bf7:	int3
+   180003bf8:	int3
+   180003bf9:	int3
+   180003bfa:	int3
+   180003bfb:	int3
+   180003bfc:	int3
+   180003bfd:	int3
+   180003bfe:	int3
+   180003bff:	int3
+   180003c00:	push   %r15
+   180003c02:	push   %r14
+   180003c04:	push   %r13
+   180003c06:	push   %r12
+   180003c08:	push   %rsi
+   180003c09:	push   %rdi
+   180003c0a:	push   %rbp
+   180003c0b:	push   %rbx
+   180003c0c:	sub    $0xa8,%rsp
+   180003c13:	mov    0x20(%rcx),%rbp
+   180003c17:	mov    0x30(%rcx),%rax
+   180003c1b:	movzwl 0x322(%rbp),%r12d
+   180003c23:	mov    %rax,0x38(%rsp)
+   180003c28:	movzwl 0x322(%rax),%eax
+   180003c2f:	mov    %ax,0x26(%rsp)
+   180003c34:	movzwl %ax,%eax
+   180003c37:	mov    %rax,0x30(%rsp)
+   180003c3c:	lea    (%r12,%rax,1),%rdx
+   180003c40:	inc    %rdx
+   180003c43:	cmp    $0xb,%rdx
+   180003c47:	ja     0x180003fb8
+   180003c4d:	mov    (%rcx),%rax
+   180003c50:	mov    %rax,0x58(%rsp)
+   180003c55:	mov    0x8(%rcx),%rbx
+   180003c59:	movzwl 0x322(%rbx),%r13d
+   180003c61:	lea    0x1(%r12),%r15
+   180003c66:	mov    0x10(%rcx),%rsi
+   180003c6a:	mov    %rdx,0x48(%rsp)
+   180003c6f:	mov    %dx,0x322(%rbp)
+   180003c76:	lea    0x8(%rbx,%rsi,8),%rcx
+   180003c7b:	mov    0x8(%rbx,%rsi,8),%rax
+   180003c80:	mov    %rax,0x28(%rsp)
+   180003c85:	lea    0x1(%rsi),%r14
+   180003c89:	lea    (%rbx,%rsi,8),%rdx
+   180003c8d:	add    $0x10,%rdx
+   180003c91:	mov    %rsi,%rdi
+   180003c94:	not    %rdi
+   180003c97:	add    %r13,%rdi
+   180003c9a:	lea    0x0(,%rdi,8),%r8
+   180003ca2:	mov    %r8,0x50(%rsp)
+   180003ca7:	call   0x18002a731
+   180003cac:	mov    0x28(%rsp),%rax
+   180003cb1:	mov    %rax,0x8(%rbp,%r12,8)
+   180003cb6:	mov    0x38(%rsp),%rax
+   180003cbb:	lea    0x8(%rax),%rdx
+   180003cbf:	lea    0x8(%rbp,%r15,8),%rcx
+   180003cc4:	mov    0x30(%rsp),%rax
+   180003cc9:	lea    0x0(,%rax,8),%r8
+   180003cd1:	mov    %r8,0x40(%rsp)
+   180003cd6:	call   0x18002a72b
+   180003cdb:	mov    %rsi,%rax
+   180003cde:	shl    $0x6,%rax
+   180003ce2:	lea    (%rbx,%rax,1),%rcx
+   180003ce6:	add    $0x60,%rcx
+   180003cea:	movups 0x60(%rbx,%rax,1),%xmm0
+   180003cef:	movups 0x70(%rbx,%rax,1),%xmm1
+   180003cf4:	movups 0x80(%rbx,%rax,1),%xmm2
+   180003cfc:	movups 0x90(%rbx,%rax,1),%xmm3
+   180003d04:	movaps %xmm3,0x90(%rsp)
+   180003d0c:	movaps %xmm2,0x80(%rsp)
+   180003d14:	movaps %xmm1,0x70(%rsp)
+   180003d19:	movaps %xmm0,0x60(%rsp)
+   180003d1e:	mov    %r14,%rax
+   180003d21:	shl    $0x6,%rax
+   180003d25:	lea    (%rbx,%rax,1),%rdx
+   180003d29:	add    $0x60,%rdx
+   180003d2d:	shl    $0x6,%rdi
+   180003d31:	mov    %rdi,%r8
+   180003d34:	call   0x18002a731
+   180003d39:	mov    %r12,0x28(%rsp)
+   180003d3e:	shl    $0x6,%r12
+   180003d42:	movaps 0x60(%rsp),%xmm0
+   180003d47:	movaps 0x70(%rsp),%xmm1
+   180003d4c:	movaps 0x80(%rsp),%xmm2
+   180003d54:	movaps 0x90(%rsp),%xmm3
+   180003d5c:	movups %xmm0,0x60(%rbp,%r12,1)
+   180003d62:	movups %xmm1,0x70(%rbp,%r12,1)
+   180003d68:	movups %xmm2,0x80(%rbp,%r12,1)
+   180003d71:	movups %xmm3,0x90(%rbp,%r12,1)
+   180003d7a:	mov    0x38(%rsp),%r12
+   180003d7f:	lea    0x60(%r12),%rdx
+   180003d84:	mov    %r15,%rax
+   180003d87:	shl    $0x6,%rax
+   180003d8b:	lea    (%rax,%rbp,1),%rcx
+   180003d8f:	add    $0x60,%rcx
+   180003d93:	mov    0x30(%rsp),%r8
+   180003d98:	shl    $0x6,%r8
+   180003d9c:	call   0x18002a72b
+   180003da1:	lea    (%rbx,%rsi,8),%rdi
+   180003da5:	add    $0x330,%rdi
+   180003dac:	lea    (%rbx,%rsi,8),%rdx
+   180003db0:	add    $0x338,%rdx
+   180003db7:	mov    %rdi,%rcx
+   180003dba:	mov    0x50(%rsp),%r8
+   180003dbf:	call   0x18002a731
+   180003dc4:	cmp    %r13,%r14
+   180003dc7:	jae    0x180003e7e
+   180003dcd:	mov    %esi,%eax
+   180003dcf:	not    %eax
+   180003dd1:	lea    (%rax,%r13,1),%ecx
+   180003dd5:	mov    %r13,%r8
+   180003dd8:	sub    %rsi,%r8
+   180003ddb:	add    $0xfffffffffffffffe,%r8
+   180003ddf:	and    $0x3,%rcx
+   180003de3:	je     0x180003e0d
+   180003de5:	xor    %edx,%edx
+   180003de7:	nopw   0x0(%rax,%rax,1)
    180003df0:	mov    (%rdi,%rdx,8),%rsi
    180003df4:	mov    %rbx,(%rsi)
    180003df7:	lea    (%r14,%rdx,1),%eax
-   180003dfb:	mov    %ax,0x1c0(%rsi)
+   180003dfb:	mov    %ax,0x320(%rsi)
    180003e02:	inc    %rdx
    180003e05:	cmp    %rdx,%rcx
    180003e08:	jne    0x180003df0
    180003e0a:	add    %rdx,%r14
    180003e0d:	cmp    $0x3,%r8
    180003e11:	jb     0x180003e7e
    180003e13:	data16 data16 data16 cs nopw 0x0(%rax,%rax,1)
-   180003e20:	mov    0x1c8(%rbx,%r14,8),%rax
+   180003e20:	mov    0x328(%rbx,%r14,8),%rax
    180003e28:	mov    %rbx,(%rax)
-   180003e2b:	mov    %r14w,0x1c0(%rax)
-   180003e33:	mov    0x1d0(%rbx,%r14,8),%rax
+   180003e2b:	mov    %r14w,0x320(%rax)
+   180003e33:	mov    0x330(%rbx,%r14,8),%rax
    180003e3b:	mov    %rbx,(%rax)
    180003e3e:	lea    0x1(%r14),%ecx
-   180003e42:	mov    %cx,0x1c0(%rax)
-   180003e49:	mov    0x1d8(%rbx,%r14,8),%rax
+   180003e42:	mov    %cx,0x320(%rax)
+   180003e49:	mov    0x338(%rbx,%r14,8),%rax
    180003e51:	mov    %rbx,(%rax)
    180003e54:	lea    0x2(%r14),%ecx
-   180003e58:	mov    %cx,0x1c0(%rax)
-   180003e5f:	mov    0x1e0(%rbx,%r14,8),%rax
+   180003e58:	mov    %cx,0x320(%rax)
+   180003e5f:	mov    0x340(%rbx,%r14,8),%rax
    180003e67:	mov    %rbx,(%rax)
    180003e6a:	lea    0x3(%r14),%ecx
-   180003e6e:	mov    %cx,0x1c0(%rax)
+   180003e6e:	mov    %cx,0x320(%rax)
    180003e75:	add    $0x4,%r14
-   180003e79:	cmp    %r9,%r14
+   180003e79:	cmp    %r13,%r14
    180003e7c:	jne    0x180003e20
-   180003e7e:	decw   0x1c2(%rbx)
+   180003e7e:	decw   0x322(%rbx)
    180003e85:	mov    $0x8,%r14d
-   180003e8b:	mov    $0x1c8,%edx
-   180003e90:	mov    0x68(%rsp),%r13
-   180003e95:	cmp    $0x1,%r13
-   180003e99:	jbe    0x180003f93
-   180003e9f:	lea    0x1c8(%r12),%rdx
-   180003ea7:	lea    0x1c8(,%r15,8),%rcx
+   180003e8b:	mov    $0x328,%edx
+   180003e90:	mov    0x58(%rsp),%r13
+   180003e95:	cmp    $0x2,%r13
+   180003e99:	jb     0x180003f93
+   180003e9f:	lea    0x328(%r12),%rdx
+   180003ea7:	lea    0x328(,%r15,8),%rcx
    180003eaf:	add    %rbp,%rcx
-   180003eb2:	mov    0x48(%rsp),%r8
+   180003eb2:	mov    0x40(%rsp),%r8
    180003eb7:	add    $0x8,%r8
    180003ebb:	call   0x18002a72b
-   180003ec0:	mov    $0x228,%edx
-   180003ec5:	mov    0x50(%rsp),%r8
-   180003eca:	mov    0x30(%rsp),%rax
+   180003ec0:	mov    $0x388,%edx
+   180003ec5:	mov    0x48(%rsp),%r8
+   180003eca:	mov    0x28(%rsp),%rax
    180003ecf:	cmp    %rax,%r8
    180003ed2:	jbe    0x180003f93
-   180003ed8:	mov    0x40(%rsp),%rsi
+   180003ed8:	mov    0x30(%rsp),%rsi
    180003edd:	inc    %esi
    180003edf:	and    $0x3,%rsi
    180003ee3:	je     0x180003f1d
-   180003ee5:	lea    0x1d0(,%rax,8),%rcx
+   180003ee5:	lea    0x330(,%rax,8),%rcx
    180003eed:	add    %rbp,%rcx
    180003ef0:	xor    %eax,%eax
    180003ef2:	data16 data16 data16 data16 cs nopw 0x0(%rax,%rax,1)
    180003f00:	mov    (%rcx,%rax,8),%rdx
    180003f04:	mov    %rbp,(%rdx)
    180003f07:	lea    (%r15,%rax,1),%edi
-   180003f0b:	mov    %di,0x1c0(%rdx)
+   180003f0b:	mov    %di,0x320(%rdx)
    180003f12:	inc    %rax
    180003f15:	cmp    %rax,%rsi
    180003f18:	jne    0x180003f00
    180003f1a:	add    %rax,%r15
-   180003f1d:	mov    $0x228,%edx
-   180003f22:	cmpw   $0x3,0x2e(%rsp)
+   180003f1d:	mov    $0x388,%edx
+   180003f22:	cmpw   $0x3,0x26(%rsp)
    180003f28:	jb     0x180003f93
    180003f2a:	nopw   0x0(%rax,%rax,1)
-   180003f30:	mov    0x1c8(%rbp,%r15,8),%rax
+   180003f30:	mov    0x328(%rbp,%r15,8),%rax
    180003f38:	mov    %rbp,(%rax)
-   180003f3b:	mov    %r15w,0x1c0(%rax)
-   180003f43:	mov    0x1d0(%rbp,%r15,8),%rax
+   180003f3b:	mov    %r15w,0x320(%rax)
+   180003f43:	mov    0x330(%rbp,%r15,8),%rax
    180003f4b:	mov    %rbp,(%rax)
    180003f4e:	lea    0x1(%r15),%ecx
-   180003f52:	mov    %cx,0x1c0(%rax)
-   180003f59:	mov    0x1d8(%rbp,%r15,8),%rax
+   180003f52:	mov    %cx,0x320(%rax)
+   180003f59:	mov    0x338(%rbp,%r15,8),%rax
    180003f61:	mov    %rbp,(%rax)
    180003f64:	lea    0x2(%r15),%ecx
-   180003f68:	mov    %cx,0x1c0(%rax)
-   180003f6f:	mov    0x1e0(%rbp,%r15,8),%rax
+   180003f68:	mov    %cx,0x320(%rax)
+   180003f6f:	mov    0x340(%rbp,%r15,8),%rax
    180003f77:	mov    %rbp,(%rax)
    180003f7a:	lea    0x3(%r15),%rcx
-   180003f7e:	mov    %cx,0x1c0(%rax)
+   180003f7e:	mov    %cx,0x320(%rax)
    180003f85:	add    $0x4,%r15
    180003f89:	cmp    %r8,%rcx
    180003f8c:	jne    0x180003f30
-   180003f8e:	mov    $0x228,%edx
+   180003f8e:	mov    $0x388,%edx
    180003f93:	mov    %r12,%rcx
    180003f96:	mov    %r14,%r8
    180003f99:	call   0x18000df80
    180003f9e:	mov    %r13,%rax
    180003fa1:	mov    %rbx,%rdx
-   180003fa4:	add    $0x98,%rsp
+   180003fa4:	add    $0xa8,%rsp
    180003fab:	pop    %rbx
    180003fac:	pop    %rbp
    180003fad:	pop    %rdi
    180003fae:	pop    %rsi
    180003faf:	pop    %r12
    180003fb1:	pop    %r13
    180003fb3:	pop    %r14
@@ -9052,15 +9041,15 @@
    180004ac0:	mov    0x28(%rsp),%rsi
    180004ac5:	mov    %rsi,0x48(%rsp)
    180004aca:	mov    %r14,0x50(%rsp)
    180004acf:	mov    %rsi,0x58(%rsp)
    180004ad4:	mov    %rdi,0x60(%rsp)
    180004ad9:	lea    0x30(%rsp),%rcx
    180004ade:	mov    $0x1,%edx
-   180004ae3:	call   0x180002fd0
+   180004ae3:	call   0x180003460
    180004ae8:	mov    %rsi,0xa8(%rsp)
    180004af0:	mov    %r14,0xb0(%rsp)
    180004af8:	mov    %r13,0xb8(%rsp)
    180004b00:	mov    0xa8(%rsp),%rax
    180004b08:	mov    %rax,0x28(%rsp)
    180004b0d:	mov    0xb0(%rsp),%r14
    180004b15:	mov    0xb8(%rsp),%r13
@@ -9083,15 +9072,15 @@
    180004b74:	mov    0x98(%rsp),%rbx
    180004b7c:	mov    %rbx,0x58(%rsp)
    180004b81:	mov    %rdx,0x40(%rsp)
    180004b86:	mov    %rbp,0x48(%rsp)
    180004b8b:	mov    %rax,0x30(%rsp)
    180004b90:	mov    %rcx,0x38(%rsp)
    180004b95:	lea    0x30(%rsp),%rcx
-   180004b9a:	call   0x180003c30
+   180004b9a:	call   0x180003850
    180004b9f:	mov    %rax,%rdi
    180004ba2:	test   %rdx,%rdx
    180004ba5:	je     0x180004cc6
    180004bab:	movzwl 0x1c2(%rdx),%eax
    180004bb2:	cmp    $0x4,%rax
    180004bb6:	ja     0x180004cc6
    180004bbc:	mov    (%rdx),%rcx
@@ -9135,15 +9124,15 @@
    180004c92:	add    %eax,%ecx
    180004c94:	inc    %ecx
    180004c96:	cmp    $0xc,%ecx
    180004c99:	jb     0x180004b40
    180004c9f:	mov    $0x5,%edx
    180004ca4:	sub    %rax,%rdx
    180004ca7:	mov    %r12,%rcx
-   180004caa:	call   0x180002fd0
+   180004caa:	call   0x180003460
    180004caf:	xor    %edx,%edx
    180004cb1:	jmp    0x180004ba2
    180004cb6:	test   %ax,%ax
    180004cb9:	jne    0x180004cc6
    180004cbb:	mov    0xc0(%rsp),%rax
    180004cc3:	movb   $0x1,(%rax)
    180004cc6:	movaps 0xe0(%rsp),%xmm0
@@ -9344,15 +9333,15 @@
    18000509e:	mov    0x98(%rbp),%rax
    1800050a5:	mov    %rax,0x78(%rbp)
    1800050a9:	mov    %r14,0x80(%rbp)
    1800050b0:	mov    %rax,0x88(%rbp)
    1800050b7:	mov    %rdi,0x90(%rbp)
    1800050be:	lea    0x60(%rbp),%rcx
    1800050c2:	mov    $0x1,%edx
-   1800050c7:	call   0x1800033c0
+   1800050c7:	call   0x180002fd0
    1800050cc:	mov    0x98(%rbp),%rax
    1800050d3:	mov    %rax,0x10(%rbp)
    1800050d7:	mov    %r14,0x18(%rbp)
    1800050db:	mov    %r15,0x20(%rbp)
    1800050df:	mov    0x10(%rbp),%rax
    1800050e3:	mov    %rax,0x98(%rbp)
    1800050ea:	mov    0x18(%rbp),%r14
@@ -9375,15 +9364,15 @@
    180005136:	mov    0x50(%rbp),%rdi
    18000513a:	mov    %rdi,0x88(%rbp)
    180005141:	mov    %rdx,0x70(%rbp)
    180005145:	mov    %rbx,0x78(%rbp)
    180005149:	mov    %rax,0x60(%rbp)
    18000514d:	mov    %rcx,0x68(%rbp)
    180005151:	lea    0x60(%rbp),%rcx
-   180005155:	call   0x180003850
+   180005155:	call   0x180003c00
    18000515a:	mov    %rax,%r13
    18000515d:	test   %rdx,%rdx
    180005160:	je     0x1800052ae
    180005166:	movzwl 0x322(%rdx),%eax
    18000516d:	cmp    $0x4,%rax
    180005171:	ja     0x1800052ae
    180005177:	mov    (%rdx),%rcx
@@ -9439,20 +9428,20 @@
    18000525b:	mov    0x50(%rbp),%rdi
    18000525f:	mov    %rdi,0x88(%rbp)
    180005266:	mov    %rdx,0x70(%rbp)
    18000526a:	mov    %rbx,0x78(%rbp)
    18000526e:	mov    %rax,0x60(%rbp)
    180005272:	mov    %rcx,0x68(%rbp)
    180005276:	lea    0x60(%rbp),%rcx
-   18000527a:	call   0x180003850
+   18000527a:	call   0x180003c00
    18000527f:	jmp    0x18000515a
    180005284:	mov    $0x5,%edx
    180005289:	sub    %rax,%rdx
    18000528c:	lea    0x28(%rbp),%rcx
-   180005290:	call   0x1800033c0
+   180005290:	call   0x180002fd0
    180005295:	xor    %edx,%edx
    180005297:	test   %rdx,%rdx
    18000529a:	jne    0x180005166
    1800052a0:	jmp    0x1800052ae
    1800052a2:	test   %ax,%ax
    1800052a5:	jne    0x1800052ae
    1800052a7:	mov    0x0(%rbp),%rax
@@ -9569,326 +9558,326 @@
    18000546d:	int3
    18000546e:	int3
    18000546f:	int3
    180005470:	push   %r14
    180005472:	push   %rsi
    180005473:	push   %rdi
    180005474:	push   %rbx
-   180005475:	sub    $0xc8,%rsp
+   180005475:	sub    $0x88,%rsp
    18000547c:	mov    %rcx,%r14
    18000547f:	mov    (%rdx),%rsi
    180005482:	mov    0x8(%rdx),%rax
    180005486:	mov    0x10(%rdx),%rcx
    18000548a:	test   %rsi,%rsi
-   18000548d:	je     0x180005710
-   180005493:	mov    0x328(%rax,%rcx,8),%rcx
+   18000548d:	je     0x1800056b0
+   180005493:	mov    0x1c8(%rax,%rcx,8),%rcx
    18000549b:	mov    %rsi,%rax
    18000549e:	dec    %rax
    1800054a1:	je     0x18000555e
    1800054a7:	add    $0xfffffffffffffffe,%rsi
    1800054ab:	mov    %rax,%rdx
    1800054ae:	and    $0x7,%rdx
    1800054b2:	je     0x1800054da
    1800054b4:	xor    %edi,%edi
    1800054b6:	cs nopw 0x0(%rax,%rax,1)
-   1800054c0:	movzwl 0x322(%rcx),%ebx
-   1800054c7:	mov    0x328(%rcx,%rbx,8),%rcx
+   1800054c0:	movzwl 0x1c2(%rcx),%ebx
+   1800054c7:	mov    0x1c8(%rcx,%rbx,8),%rcx
    1800054cf:	inc    %rdi
    1800054d2:	cmp    %rdi,%rdx
    1800054d5:	jne    0x1800054c0
    1800054d7:	sub    %rdi,%rax
    1800054da:	cmp    $0x7,%rsi
    1800054de:	jb     0x18000555e
-   1800054e0:	movzwl 0x322(%rcx),%edx
-   1800054e7:	mov    0x328(%rcx,%rdx,8),%rcx
-   1800054ef:	movzwl 0x322(%rcx),%edx
-   1800054f6:	mov    0x328(%rcx,%rdx,8),%rcx
-   1800054fe:	movzwl 0x322(%rcx),%edx
-   180005505:	mov    0x328(%rcx,%rdx,8),%rcx
-   18000550d:	movzwl 0x322(%rcx),%edx
-   180005514:	mov    0x328(%rcx,%rdx,8),%rcx
-   18000551c:	movzwl 0x322(%rcx),%edx
-   180005523:	mov    0x328(%rcx,%rdx,8),%rcx
-   18000552b:	movzwl 0x322(%rcx),%edx
-   180005532:	mov    0x328(%rcx,%rdx,8),%rcx
-   18000553a:	movzwl 0x322(%rcx),%edx
-   180005541:	mov    0x328(%rcx,%rdx,8),%rcx
-   180005549:	movzwl 0x322(%rcx),%edx
-   180005550:	mov    0x328(%rcx,%rdx,8),%rcx
+   1800054e0:	movzwl 0x1c2(%rcx),%edx
+   1800054e7:	mov    0x1c8(%rcx,%rdx,8),%rcx
+   1800054ef:	movzwl 0x1c2(%rcx),%edx
+   1800054f6:	mov    0x1c8(%rcx,%rdx,8),%rcx
+   1800054fe:	movzwl 0x1c2(%rcx),%edx
+   180005505:	mov    0x1c8(%rcx,%rdx,8),%rcx
+   18000550d:	movzwl 0x1c2(%rcx),%edx
+   180005514:	mov    0x1c8(%rcx,%rdx,8),%rcx
+   18000551c:	movzwl 0x1c2(%rcx),%edx
+   180005523:	mov    0x1c8(%rcx,%rdx,8),%rcx
+   18000552b:	movzwl 0x1c2(%rcx),%edx
+   180005532:	mov    0x1c8(%rcx,%rdx,8),%rcx
+   18000553a:	movzwl 0x1c2(%rcx),%edx
+   180005541:	mov    0x1c8(%rcx,%rdx,8),%rcx
+   180005549:	movzwl 0x1c2(%rcx),%edx
+   180005550:	mov    0x1c8(%rcx,%rdx,8),%rcx
    180005558:	add    $0xfffffffffffffff8,%rax
    18000555c:	jne    0x1800054e0
-   18000555e:	movzwl 0x322(%rcx),%eax
+   18000555e:	movzwl 0x1c2(%rcx),%eax
    180005565:	dec    %rax
-   180005568:	movq   $0x0,0x80(%rsp)
-   180005574:	mov    %rcx,0x88(%rsp)
-   18000557c:	mov    %rax,0x90(%rsp)
-   180005584:	lea    0x20(%rsp),%rcx
-   180005589:	lea    0x80(%rsp),%rdx
-   180005591:	call   0x180004e30
-   180005596:	mov    0x20(%rsp),%rsi
-   18000559b:	movups 0x28(%rsp),%xmm0
-   1800055a0:	movaps %xmm0,0x80(%rsp)
-   1800055a8:	movups 0x38(%rsp),%xmm0
-   1800055ad:	movaps %xmm0,0x90(%rsp)
-   1800055b5:	movups 0x48(%rsp),%xmm0
-   1800055ba:	movaps %xmm0,0xa0(%rsp)
-   1800055c2:	movups 0x58(%rsp),%xmm0
-   1800055c7:	movaps %xmm0,0xb0(%rsp)
-   1800055cf:	mov    0x68(%rsp),%rcx
-   1800055d4:	mov    0x70(%rsp),%rax
-   1800055d9:	mov    0x78(%rsp),%rdx
-   1800055de:	movzwl 0x322(%rax),%ebx
-   1800055e5:	cmp    %rbx,%rdx
-   1800055e8:	jae    0x1800055f0
-   1800055ea:	mov    %rax,%rdi
-   1800055ed:	jmp    0x180005609
-   1800055ef:	nop
-   1800055f0:	mov    (%rax),%rdi
-   1800055f3:	movzwl 0x320(%rax),%edx
-   1800055fa:	inc    %rcx
-   1800055fd:	mov    %rdi,%rax
-   180005600:	cmp    0x322(%rdi),%dx
-   180005607:	jae    0x1800055f0
-   180005609:	mov    %rdx,%rax
-   18000560c:	shl    $0x6,%rax
-   180005610:	mov    0x8(%rdi,%rdx,8),%r8
-   180005615:	mov    %rsi,0x8(%rdi,%rdx,8)
-   18000561a:	movups 0x60(%rdi,%rax,1),%xmm0
-   18000561f:	movups 0x70(%rdi,%rax,1),%xmm1
-   180005624:	movups 0x80(%rdi,%rax,1),%xmm2
-   18000562c:	movups 0x90(%rdi,%rax,1),%xmm3
-   180005634:	movaps %xmm3,0x50(%rsp)
-   180005639:	movaps %xmm2,0x40(%rsp)
-   18000563e:	movaps %xmm1,0x30(%rsp)
-   180005643:	movaps %xmm0,0x20(%rsp)
-   180005648:	movaps 0x80(%rsp),%xmm0
-   180005650:	movaps 0x90(%rsp),%xmm1
-   180005658:	movaps 0xa0(%rsp),%xmm2
-   180005660:	movaps 0xb0(%rsp),%xmm3
-   180005668:	movups %xmm0,0x60(%rdi,%rax,1)
-   18000566d:	movups %xmm1,0x70(%rdi,%rax,1)
-   180005672:	movups %xmm2,0x80(%rdi,%rax,1)
-   18000567a:	movups %xmm3,0x90(%rdi,%rax,1)
-   180005682:	test   %rcx,%rcx
-   180005685:	je     0x180005732
-   18000568b:	mov    0x330(%rdi,%rdx,8),%rdi
-   180005693:	mov    %rcx,%rsi
-   180005696:	dec    %rsi
-   180005699:	je     0x180005737
-   18000569f:	add    $0xfffffffffffffffe,%rcx
-   1800056a3:	mov    %rsi,%rax
-   1800056a6:	and    $0x7,%rax
-   1800056aa:	je     0x1800056c2
-   1800056ac:	xor    %edx,%edx
-   1800056ae:	xchg   %ax,%ax
-   1800056b0:	mov    0x328(%rdi),%rdi
-   1800056b7:	inc    %rdx
-   1800056ba:	cmp    %rdx,%rax
-   1800056bd:	jne    0x1800056b0
-   1800056bf:	sub    %rdx,%rsi
-   1800056c2:	xor    %edx,%edx
-   1800056c4:	cmp    $0x7,%rcx
-   1800056c8:	jb     0x180005739
-   1800056ca:	nopw   0x0(%rax,%rax,1)
-   1800056d0:	mov    0x328(%rdi),%rax
-   1800056d7:	mov    0x328(%rax),%rax
-   1800056de:	mov    0x328(%rax),%rax
-   1800056e5:	mov    0x328(%rax),%rax
-   1800056ec:	mov    0x328(%rax),%rax
-   1800056f3:	mov    0x328(%rax),%rax
-   1800056fa:	mov    0x328(%rax),%rax
-   180005701:	mov    0x328(%rax),%rdi
-   180005708:	add    $0xfffffffffffffff8,%rsi
-   18000570c:	jne    0x1800056d0
-   18000570e:	jmp    0x180005739
-   180005710:	movq   $0x0,0x20(%rsp)
-   180005719:	mov    %rax,0x28(%rsp)
-   18000571e:	mov    %rcx,0x30(%rsp)
-   180005723:	lea    0x20(%rsp),%rdx
-   180005728:	mov    %r14,%rcx
-   18000572b:	call   0x180004e30
-   180005730:	jmp    0x180005774
-   180005732:	inc    %rdx
-   180005735:	jmp    0x180005739
-   180005737:	xor    %edx,%edx
-   180005739:	movaps 0x20(%rsp),%xmm0
-   18000573e:	movaps 0x30(%rsp),%xmm1
-   180005743:	movaps 0x40(%rsp),%xmm2
-   180005748:	movaps 0x50(%rsp),%xmm3
-   18000574d:	movups %xmm3,0x38(%r14)
-   180005752:	movups %xmm2,0x28(%r14)
-   180005757:	movups %xmm1,0x18(%r14)
-   18000575c:	movups %xmm0,0x8(%r14)
-   180005761:	mov    %r8,(%r14)
-   180005764:	movq   $0x0,0x48(%r14)
-   18000576c:	mov    %rdi,0x50(%r14)
-   180005770:	mov    %rdx,0x58(%r14)
-   180005774:	mov    %r14,%rax
-   180005777:	add    $0xc8,%rsp
-   18000577e:	pop    %rbx
-   18000577f:	pop    %rdi
-   180005780:	pop    %rsi
-   180005781:	pop    %r14
-   180005783:	ret
-   180005784:	int3
-   180005785:	int3
-   180005786:	int3
-   180005787:	int3
-   180005788:	int3
-   180005789:	int3
-   18000578a:	int3
-   18000578b:	int3
-   18000578c:	int3
-   18000578d:	int3
-   18000578e:	int3
-   18000578f:	int3
-   180005790:	push   %r14
-   180005792:	push   %rsi
-   180005793:	push   %rdi
-   180005794:	push   %rbx
-   180005795:	sub    $0x88,%rsp
-   18000579c:	mov    %rcx,%r14
-   18000579f:	mov    (%rdx),%rsi
-   1800057a2:	mov    0x8(%rdx),%rax
-   1800057a6:	mov    0x10(%rdx),%rcx
-   1800057aa:	test   %rsi,%rsi
-   1800057ad:	je     0x1800059d0
-   1800057b3:	mov    0x1c8(%rax,%rcx,8),%rcx
-   1800057bb:	mov    %rsi,%rax
-   1800057be:	dec    %rax
-   1800057c1:	je     0x18000587e
-   1800057c7:	add    $0xfffffffffffffffe,%rsi
-   1800057cb:	mov    %rax,%rdx
-   1800057ce:	and    $0x7,%rdx
-   1800057d2:	je     0x1800057fa
-   1800057d4:	xor    %edi,%edi
-   1800057d6:	cs nopw 0x0(%rax,%rax,1)
-   1800057e0:	movzwl 0x1c2(%rcx),%ebx
-   1800057e7:	mov    0x1c8(%rcx,%rbx,8),%rcx
-   1800057ef:	inc    %rdi
-   1800057f2:	cmp    %rdi,%rdx
-   1800057f5:	jne    0x1800057e0
-   1800057f7:	sub    %rdi,%rax
-   1800057fa:	cmp    $0x7,%rsi
-   1800057fe:	jb     0x18000587e
-   180005800:	movzwl 0x1c2(%rcx),%edx
-   180005807:	mov    0x1c8(%rcx,%rdx,8),%rcx
-   18000580f:	movzwl 0x1c2(%rcx),%edx
-   180005816:	mov    0x1c8(%rcx,%rdx,8),%rcx
-   18000581e:	movzwl 0x1c2(%rcx),%edx
-   180005825:	mov    0x1c8(%rcx,%rdx,8),%rcx
-   18000582d:	movzwl 0x1c2(%rcx),%edx
-   180005834:	mov    0x1c8(%rcx,%rdx,8),%rcx
-   18000583c:	movzwl 0x1c2(%rcx),%edx
-   180005843:	mov    0x1c8(%rcx,%rdx,8),%rcx
-   18000584b:	movzwl 0x1c2(%rcx),%edx
-   180005852:	mov    0x1c8(%rcx,%rdx,8),%rcx
-   18000585a:	movzwl 0x1c2(%rcx),%edx
-   180005861:	mov    0x1c8(%rcx,%rdx,8),%rcx
-   180005869:	movzwl 0x1c2(%rcx),%edx
-   180005870:	mov    0x1c8(%rcx,%rdx,8),%rcx
-   180005878:	add    $0xfffffffffffffff8,%rax
-   18000587c:	jne    0x180005800
-   18000587e:	movzwl 0x1c2(%rcx),%eax
-   180005885:	dec    %rax
-   180005888:	movq   $0x0,0x20(%rsp)
-   180005891:	mov    %rcx,0x28(%rsp)
-   180005896:	mov    %rax,0x30(%rsp)
-   18000589b:	lea    0x40(%rsp),%rcx
-   1800058a0:	lea    0x20(%rsp),%rdx
-   1800058a5:	call   0x180004880
-   1800058aa:	mov    0x40(%rsp),%rsi
-   1800058af:	movups 0x48(%rsp),%xmm0
-   1800058b4:	movaps %xmm0,0x20(%rsp)
-   1800058b9:	movups 0x58(%rsp),%xmm0
-   1800058be:	movaps %xmm0,0x30(%rsp)
-   1800058c3:	mov    0x68(%rsp),%rdx
-   1800058c8:	mov    0x70(%rsp),%rax
-   1800058cd:	mov    0x78(%rsp),%rcx
-   1800058d2:	movzwl 0x1c2(%rax),%ebx
-   1800058d9:	cmp    %rbx,%rcx
-   1800058dc:	jae    0x1800058f0
-   1800058de:	mov    %rax,%rdi
-   1800058e1:	jmp    0x180005909
-   1800058e3:	data16 data16 data16 cs nopw 0x0(%rax,%rax,1)
-   1800058f0:	mov    (%rax),%rdi
-   1800058f3:	movzwl 0x1c0(%rax),%ecx
-   1800058fa:	inc    %rdx
-   1800058fd:	mov    %rdi,%rax
-   180005900:	cmp    0x1c2(%rdi),%cx
-   180005907:	jae    0x1800058f0
-   180005909:	mov    %rcx,%rax
-   18000590c:	shl    $0x5,%rax
-   180005910:	mov    0x8(%rdi,%rcx,8),%r8
-   180005915:	mov    %rsi,0x8(%rdi,%rcx,8)
-   18000591a:	movups 0x60(%rdi,%rax,1),%xmm0
-   18000591f:	movups 0x70(%rdi,%rax,1),%xmm1
-   180005924:	movaps %xmm1,0x50(%rsp)
-   180005929:	movaps %xmm0,0x40(%rsp)
-   18000592e:	movaps 0x20(%rsp),%xmm0
-   180005933:	movaps 0x30(%rsp),%xmm1
-   180005938:	movups %xmm0,0x60(%rdi,%rax,1)
-   18000593d:	movups %xmm1,0x70(%rdi,%rax,1)
-   180005942:	test   %rdx,%rdx
-   180005945:	je     0x1800059f2
-   18000594b:	mov    0x1d0(%rdi,%rcx,8),%rdi
-   180005953:	mov    %rdx,%rsi
-   180005956:	dec    %rsi
-   180005959:	je     0x1800059f7
-   18000595f:	add    $0xfffffffffffffffe,%rdx
-   180005963:	mov    %rsi,%rax
-   180005966:	and    $0x7,%rax
-   18000596a:	je     0x180005982
-   18000596c:	xor    %ecx,%ecx
-   18000596e:	xchg   %ax,%ax
-   180005970:	mov    0x1c8(%rdi),%rdi
-   180005977:	inc    %rcx
-   18000597a:	cmp    %rcx,%rax
-   18000597d:	jne    0x180005970
-   18000597f:	sub    %rcx,%rsi
-   180005982:	xor    %ecx,%ecx
-   180005984:	cmp    $0x7,%rdx
-   180005988:	jb     0x1800059f9
-   18000598a:	nopw   0x0(%rax,%rax,1)
-   180005990:	mov    0x1c8(%rdi),%rax
-   180005997:	mov    0x1c8(%rax),%rax
-   18000599e:	mov    0x1c8(%rax),%rax
-   1800059a5:	mov    0x1c8(%rax),%rax
-   1800059ac:	mov    0x1c8(%rax),%rax
-   1800059b3:	mov    0x1c8(%rax),%rax
-   1800059ba:	mov    0x1c8(%rax),%rax
-   1800059c1:	mov    0x1c8(%rax),%rdi
-   1800059c8:	add    $0xfffffffffffffff8,%rsi
-   1800059cc:	jne    0x180005990
-   1800059ce:	jmp    0x1800059f9
-   1800059d0:	movq   $0x0,0x40(%rsp)
-   1800059d9:	mov    %rax,0x48(%rsp)
-   1800059de:	mov    %rcx,0x50(%rsp)
-   1800059e3:	lea    0x40(%rsp),%rdx
-   1800059e8:	mov    %r14,%rcx
-   1800059eb:	call   0x180004880
-   1800059f0:	jmp    0x180005a20
-   1800059f2:	inc    %rcx
-   1800059f5:	jmp    0x1800059f9
-   1800059f7:	xor    %ecx,%ecx
-   1800059f9:	movaps 0x40(%rsp),%xmm0
-   1800059fe:	movaps 0x50(%rsp),%xmm1
-   180005a03:	movups %xmm1,0x18(%r14)
-   180005a08:	movups %xmm0,0x8(%r14)
-   180005a0d:	mov    %r8,(%r14)
-   180005a10:	movq   $0x0,0x28(%r14)
-   180005a18:	mov    %rdi,0x30(%r14)
-   180005a1c:	mov    %rcx,0x38(%r14)
-   180005a20:	mov    %r14,%rax
-   180005a23:	add    $0x88,%rsp
-   180005a2a:	pop    %rbx
-   180005a2b:	pop    %rdi
-   180005a2c:	pop    %rsi
-   180005a2d:	pop    %r14
-   180005a2f:	ret
+   180005568:	movq   $0x0,0x20(%rsp)
+   180005571:	mov    %rcx,0x28(%rsp)
+   180005576:	mov    %rax,0x30(%rsp)
+   18000557b:	lea    0x40(%rsp),%rcx
+   180005580:	lea    0x20(%rsp),%rdx
+   180005585:	call   0x180004880
+   18000558a:	mov    0x40(%rsp),%rsi
+   18000558f:	movups 0x48(%rsp),%xmm0
+   180005594:	movaps %xmm0,0x20(%rsp)
+   180005599:	movups 0x58(%rsp),%xmm0
+   18000559e:	movaps %xmm0,0x30(%rsp)
+   1800055a3:	mov    0x68(%rsp),%rdx
+   1800055a8:	mov    0x70(%rsp),%rax
+   1800055ad:	mov    0x78(%rsp),%rcx
+   1800055b2:	movzwl 0x1c2(%rax),%ebx
+   1800055b9:	cmp    %rbx,%rcx
+   1800055bc:	jae    0x1800055d0
+   1800055be:	mov    %rax,%rdi
+   1800055c1:	jmp    0x1800055e9
+   1800055c3:	data16 data16 data16 cs nopw 0x0(%rax,%rax,1)
+   1800055d0:	mov    (%rax),%rdi
+   1800055d3:	movzwl 0x1c0(%rax),%ecx
+   1800055da:	inc    %rdx
+   1800055dd:	mov    %rdi,%rax
+   1800055e0:	cmp    0x1c2(%rdi),%cx
+   1800055e7:	jae    0x1800055d0
+   1800055e9:	mov    %rcx,%rax
+   1800055ec:	shl    $0x5,%rax
+   1800055f0:	mov    0x8(%rdi,%rcx,8),%r8
+   1800055f5:	mov    %rsi,0x8(%rdi,%rcx,8)
+   1800055fa:	movups 0x60(%rdi,%rax,1),%xmm0
+   1800055ff:	movups 0x70(%rdi,%rax,1),%xmm1
+   180005604:	movaps %xmm1,0x50(%rsp)
+   180005609:	movaps %xmm0,0x40(%rsp)
+   18000560e:	movaps 0x20(%rsp),%xmm0
+   180005613:	movaps 0x30(%rsp),%xmm1
+   180005618:	movups %xmm0,0x60(%rdi,%rax,1)
+   18000561d:	movups %xmm1,0x70(%rdi,%rax,1)
+   180005622:	test   %rdx,%rdx
+   180005625:	je     0x1800056d2
+   18000562b:	mov    0x1d0(%rdi,%rcx,8),%rdi
+   180005633:	mov    %rdx,%rsi
+   180005636:	dec    %rsi
+   180005639:	je     0x1800056d7
+   18000563f:	add    $0xfffffffffffffffe,%rdx
+   180005643:	mov    %rsi,%rax
+   180005646:	and    $0x7,%rax
+   18000564a:	je     0x180005662
+   18000564c:	xor    %ecx,%ecx
+   18000564e:	xchg   %ax,%ax
+   180005650:	mov    0x1c8(%rdi),%rdi
+   180005657:	inc    %rcx
+   18000565a:	cmp    %rcx,%rax
+   18000565d:	jne    0x180005650
+   18000565f:	sub    %rcx,%rsi
+   180005662:	xor    %ecx,%ecx
+   180005664:	cmp    $0x7,%rdx
+   180005668:	jb     0x1800056d9
+   18000566a:	nopw   0x0(%rax,%rax,1)
+   180005670:	mov    0x1c8(%rdi),%rax
+   180005677:	mov    0x1c8(%rax),%rax
+   18000567e:	mov    0x1c8(%rax),%rax
+   180005685:	mov    0x1c8(%rax),%rax
+   18000568c:	mov    0x1c8(%rax),%rax
+   180005693:	mov    0x1c8(%rax),%rax
+   18000569a:	mov    0x1c8(%rax),%rax
+   1800056a1:	mov    0x1c8(%rax),%rdi
+   1800056a8:	add    $0xfffffffffffffff8,%rsi
+   1800056ac:	jne    0x180005670
+   1800056ae:	jmp    0x1800056d9
+   1800056b0:	movq   $0x0,0x40(%rsp)
+   1800056b9:	mov    %rax,0x48(%rsp)
+   1800056be:	mov    %rcx,0x50(%rsp)
+   1800056c3:	lea    0x40(%rsp),%rdx
+   1800056c8:	mov    %r14,%rcx
+   1800056cb:	call   0x180004880
+   1800056d0:	jmp    0x180005700
+   1800056d2:	inc    %rcx
+   1800056d5:	jmp    0x1800056d9
+   1800056d7:	xor    %ecx,%ecx
+   1800056d9:	movaps 0x40(%rsp),%xmm0
+   1800056de:	movaps 0x50(%rsp),%xmm1
+   1800056e3:	movups %xmm1,0x18(%r14)
+   1800056e8:	movups %xmm0,0x8(%r14)
+   1800056ed:	mov    %r8,(%r14)
+   1800056f0:	movq   $0x0,0x28(%r14)
+   1800056f8:	mov    %rdi,0x30(%r14)
+   1800056fc:	mov    %rcx,0x38(%r14)
+   180005700:	mov    %r14,%rax
+   180005703:	add    $0x88,%rsp
+   18000570a:	pop    %rbx
+   18000570b:	pop    %rdi
+   18000570c:	pop    %rsi
+   18000570d:	pop    %r14
+   18000570f:	ret
+   180005710:	push   %r14
+   180005712:	push   %rsi
+   180005713:	push   %rdi
+   180005714:	push   %rbx
+   180005715:	sub    $0xc8,%rsp
+   18000571c:	mov    %rcx,%r14
+   18000571f:	mov    (%rdx),%rsi
+   180005722:	mov    0x8(%rdx),%rax
+   180005726:	mov    0x10(%rdx),%rcx
+   18000572a:	test   %rsi,%rsi
+   18000572d:	je     0x1800059b0
+   180005733:	mov    0x328(%rax,%rcx,8),%rcx
+   18000573b:	mov    %rsi,%rax
+   18000573e:	dec    %rax
+   180005741:	je     0x1800057fe
+   180005747:	add    $0xfffffffffffffffe,%rsi
+   18000574b:	mov    %rax,%rdx
+   18000574e:	and    $0x7,%rdx
+   180005752:	je     0x18000577a
+   180005754:	xor    %edi,%edi
+   180005756:	cs nopw 0x0(%rax,%rax,1)
+   180005760:	movzwl 0x322(%rcx),%ebx
+   180005767:	mov    0x328(%rcx,%rbx,8),%rcx
+   18000576f:	inc    %rdi
+   180005772:	cmp    %rdi,%rdx
+   180005775:	jne    0x180005760
+   180005777:	sub    %rdi,%rax
+   18000577a:	cmp    $0x7,%rsi
+   18000577e:	jb     0x1800057fe
+   180005780:	movzwl 0x322(%rcx),%edx
+   180005787:	mov    0x328(%rcx,%rdx,8),%rcx
+   18000578f:	movzwl 0x322(%rcx),%edx
+   180005796:	mov    0x328(%rcx,%rdx,8),%rcx
+   18000579e:	movzwl 0x322(%rcx),%edx
+   1800057a5:	mov    0x328(%rcx,%rdx,8),%rcx
+   1800057ad:	movzwl 0x322(%rcx),%edx
+   1800057b4:	mov    0x328(%rcx,%rdx,8),%rcx
+   1800057bc:	movzwl 0x322(%rcx),%edx
+   1800057c3:	mov    0x328(%rcx,%rdx,8),%rcx
+   1800057cb:	movzwl 0x322(%rcx),%edx
+   1800057d2:	mov    0x328(%rcx,%rdx,8),%rcx
+   1800057da:	movzwl 0x322(%rcx),%edx
+   1800057e1:	mov    0x328(%rcx,%rdx,8),%rcx
+   1800057e9:	movzwl 0x322(%rcx),%edx
+   1800057f0:	mov    0x328(%rcx,%rdx,8),%rcx
+   1800057f8:	add    $0xfffffffffffffff8,%rax
+   1800057fc:	jne    0x180005780
+   1800057fe:	movzwl 0x322(%rcx),%eax
+   180005805:	dec    %rax
+   180005808:	movq   $0x0,0x80(%rsp)
+   180005814:	mov    %rcx,0x88(%rsp)
+   18000581c:	mov    %rax,0x90(%rsp)
+   180005824:	lea    0x20(%rsp),%rcx
+   180005829:	lea    0x80(%rsp),%rdx
+   180005831:	call   0x180004e30
+   180005836:	mov    0x20(%rsp),%rsi
+   18000583b:	movups 0x28(%rsp),%xmm0
+   180005840:	movaps %xmm0,0x80(%rsp)
+   180005848:	movups 0x38(%rsp),%xmm0
+   18000584d:	movaps %xmm0,0x90(%rsp)
+   180005855:	movups 0x48(%rsp),%xmm0
+   18000585a:	movaps %xmm0,0xa0(%rsp)
+   180005862:	movups 0x58(%rsp),%xmm0
+   180005867:	movaps %xmm0,0xb0(%rsp)
+   18000586f:	mov    0x68(%rsp),%rcx
+   180005874:	mov    0x70(%rsp),%rax
+   180005879:	mov    0x78(%rsp),%rdx
+   18000587e:	movzwl 0x322(%rax),%ebx
+   180005885:	cmp    %rbx,%rdx
+   180005888:	jae    0x180005890
+   18000588a:	mov    %rax,%rdi
+   18000588d:	jmp    0x1800058a9
+   18000588f:	nop
+   180005890:	mov    (%rax),%rdi
+   180005893:	movzwl 0x320(%rax),%edx
+   18000589a:	inc    %rcx
+   18000589d:	mov    %rdi,%rax
+   1800058a0:	cmp    0x322(%rdi),%dx
+   1800058a7:	jae    0x180005890
+   1800058a9:	mov    %rdx,%rax
+   1800058ac:	shl    $0x6,%rax
+   1800058b0:	mov    0x8(%rdi,%rdx,8),%r8
+   1800058b5:	mov    %rsi,0x8(%rdi,%rdx,8)
+   1800058ba:	movups 0x60(%rdi,%rax,1),%xmm0
+   1800058bf:	movups 0x70(%rdi,%rax,1),%xmm1
+   1800058c4:	movups 0x80(%rdi,%rax,1),%xmm2
+   1800058cc:	movups 0x90(%rdi,%rax,1),%xmm3
+   1800058d4:	movaps %xmm3,0x50(%rsp)
+   1800058d9:	movaps %xmm2,0x40(%rsp)
+   1800058de:	movaps %xmm1,0x30(%rsp)
+   1800058e3:	movaps %xmm0,0x20(%rsp)
+   1800058e8:	movaps 0x80(%rsp),%xmm0
+   1800058f0:	movaps 0x90(%rsp),%xmm1
+   1800058f8:	movaps 0xa0(%rsp),%xmm2
+   180005900:	movaps 0xb0(%rsp),%xmm3
+   180005908:	movups %xmm0,0x60(%rdi,%rax,1)
+   18000590d:	movups %xmm1,0x70(%rdi,%rax,1)
+   180005912:	movups %xmm2,0x80(%rdi,%rax,1)
+   18000591a:	movups %xmm3,0x90(%rdi,%rax,1)
+   180005922:	test   %rcx,%rcx
+   180005925:	je     0x1800059d2
+   18000592b:	mov    0x330(%rdi,%rdx,8),%rdi
+   180005933:	mov    %rcx,%rsi
+   180005936:	dec    %rsi
+   180005939:	je     0x1800059d7
+   18000593f:	add    $0xfffffffffffffffe,%rcx
+   180005943:	mov    %rsi,%rax
+   180005946:	and    $0x7,%rax
+   18000594a:	je     0x180005962
+   18000594c:	xor    %edx,%edx
+   18000594e:	xchg   %ax,%ax
+   180005950:	mov    0x328(%rdi),%rdi
+   180005957:	inc    %rdx
+   18000595a:	cmp    %rdx,%rax
+   18000595d:	jne    0x180005950
+   18000595f:	sub    %rdx,%rsi
+   180005962:	xor    %edx,%edx
+   180005964:	cmp    $0x7,%rcx
+   180005968:	jb     0x1800059d9
+   18000596a:	nopw   0x0(%rax,%rax,1)
+   180005970:	mov    0x328(%rdi),%rax
+   180005977:	mov    0x328(%rax),%rax
+   18000597e:	mov    0x328(%rax),%rax
+   180005985:	mov    0x328(%rax),%rax
+   18000598c:	mov    0x328(%rax),%rax
+   180005993:	mov    0x328(%rax),%rax
+   18000599a:	mov    0x328(%rax),%rax
+   1800059a1:	mov    0x328(%rax),%rdi
+   1800059a8:	add    $0xfffffffffffffff8,%rsi
+   1800059ac:	jne    0x180005970
+   1800059ae:	jmp    0x1800059d9
+   1800059b0:	movq   $0x0,0x20(%rsp)
+   1800059b9:	mov    %rax,0x28(%rsp)
+   1800059be:	mov    %rcx,0x30(%rsp)
+   1800059c3:	lea    0x20(%rsp),%rdx
+   1800059c8:	mov    %r14,%rcx
+   1800059cb:	call   0x180004e30
+   1800059d0:	jmp    0x180005a14
+   1800059d2:	inc    %rdx
+   1800059d5:	jmp    0x1800059d9
+   1800059d7:	xor    %edx,%edx
+   1800059d9:	movaps 0x20(%rsp),%xmm0
+   1800059de:	movaps 0x30(%rsp),%xmm1
+   1800059e3:	movaps 0x40(%rsp),%xmm2
+   1800059e8:	movaps 0x50(%rsp),%xmm3
+   1800059ed:	movups %xmm3,0x38(%r14)
+   1800059f2:	movups %xmm2,0x28(%r14)
+   1800059f7:	movups %xmm1,0x18(%r14)
+   1800059fc:	movups %xmm0,0x8(%r14)
+   180005a01:	mov    %r8,(%r14)
+   180005a04:	movq   $0x0,0x48(%r14)
+   180005a0c:	mov    %rdi,0x50(%r14)
+   180005a10:	mov    %rdx,0x58(%r14)
+   180005a14:	mov    %r14,%rax
+   180005a17:	add    $0xc8,%rsp
+   180005a1e:	pop    %rbx
+   180005a1f:	pop    %rdi
+   180005a20:	pop    %rsi
+   180005a21:	pop    %r14
+   180005a23:	ret
+   180005a24:	int3
+   180005a25:	int3
+   180005a26:	int3
+   180005a27:	int3
+   180005a28:	int3
+   180005a29:	int3
+   180005a2a:	int3
+   180005a2b:	int3
+   180005a2c:	int3
+   180005a2d:	int3
+   180005a2e:	int3
+   180005a2f:	int3
    180005a30:	push   %rbp
    180005a31:	push   %r15
    180005a33:	push   %r14
    180005a35:	push   %r12
    180005a37:	push   %rsi
    180005a38:	push   %rdi
    180005a39:	push   %rbx
@@ -10186,128 +10175,128 @@
    180005e2d:	int3
    180005e2e:	int3
    180005e2f:	int3
    180005e30:	push   %rsi
    180005e31:	push   %rdi
    180005e32:	sub    $0x58,%rsp
    180005e36:	inc    %rdx
-   180005e39:	je     0x180005ee5
+   180005e39:	je     0x180005ed6
    180005e3f:	mov    %rcx,%rsi
    180005e42:	mov    0x8(%rcx),%rax
    180005e46:	lea    (%rax,%rax,1),%rcx
    180005e4a:	cmp    %rdx,%rcx
    180005e4d:	cmova  %rcx,%rdx
    180005e51:	cmp    $0x5,%rdx
    180005e55:	mov    $0x4,%edi
    180005e5a:	cmovae %rdx,%rdi
-   180005e5e:	movabs $0x555555555555556,%rcx
-   180005e68:	xor    %r8d,%r8d
-   180005e6b:	cmp    %rcx,%rdi
-   180005e6e:	setb   %r8b
-   180005e72:	lea    0x0(,%rdi,8),%rcx
-   180005e7a:	lea    (%rcx,%rcx,2),%rdx
-   180005e7e:	shl    $0x3,%r8
-   180005e82:	test   %rax,%rax
-   180005e85:	je     0x180005ea7
-   180005e87:	mov    (%rsi),%rcx
-   180005e8a:	shl    $0x3,%rax
-   180005e8e:	lea    (%rax,%rax,2),%rax
-   180005e92:	mov    %rcx,0x28(%rsp)
-   180005e97:	mov    %rax,0x30(%rsp)
-   180005e9c:	movq   $0x8,0x38(%rsp)
-   180005ea5:	jmp    0x180005eb0
-   180005ea7:	movq   $0x0,0x38(%rsp)
-   180005eb0:	lea    0x40(%rsp),%rcx
-   180005eb5:	lea    0x28(%rsp),%r9
-   180005eba:	call   0x180005d90
-   180005ebf:	cmpq   $0x0,0x40(%rsp)
-   180005ec5:	mov    0x48(%rsp),%rcx
-   180005eca:	je     0x180005eec
-   180005ecc:	mov    0x50(%rsp),%rdx
-   180005ed1:	movabs $0x8000000000000001,%rax
-   180005edb:	cmp    %rax,%rdx
-   180005ede:	je     0x180005ef3
-   180005ee0:	test   %rdx,%rdx
-   180005ee3:	jne    0x180005efa
-   180005ee5:	call   0x18001ef90
-   180005eea:	ud2
-   180005eec:	mov    %rcx,(%rsi)
-   180005eef:	mov    %rdi,0x8(%rsi)
-   180005ef3:	add    $0x58,%rsp
-   180005ef7:	pop    %rdi
-   180005ef8:	pop    %rsi
-   180005ef9:	ret
-   180005efa:	call   0x18002b5f0
-   180005eff:	ud2
-   180005f01:	int3
-   180005f02:	int3
-   180005f03:	int3
-   180005f04:	int3
-   180005f05:	int3
-   180005f06:	int3
-   180005f07:	int3
-   180005f08:	int3
-   180005f09:	int3
-   180005f0a:	int3
-   180005f0b:	int3
-   180005f0c:	int3
-   180005f0d:	int3
-   180005f0e:	int3
-   180005f0f:	int3
-   180005f10:	push   %rsi
-   180005f11:	push   %rdi
-   180005f12:	sub    $0x58,%rsp
-   180005f16:	inc    %rdx
-   180005f19:	je     0x180005fb6
-   180005f1f:	mov    %rcx,%rsi
-   180005f22:	mov    0x8(%rcx),%rax
-   180005f26:	lea    (%rax,%rax,1),%rcx
-   180005f2a:	cmp    %rdx,%rcx
-   180005f2d:	cmova  %rcx,%rdx
-   180005f31:	cmp    $0x5,%rdx
-   180005f35:	mov    $0x4,%edi
-   180005f3a:	cmovae %rdx,%rdi
-   180005f3e:	xor    %r8d,%r8d
-   180005f41:	mov    %rdi,%rcx
-   180005f44:	shr    $0x3b,%rcx
-   180005f48:	sete   %r8b
-   180005f4c:	mov    %rdi,%rdx
-   180005f4f:	shl    $0x4,%rdx
-   180005f53:	shl    $0x3,%r8
-   180005f57:	test   %rax,%rax
-   180005f5a:	je     0x180005f78
-   180005f5c:	mov    (%rsi),%rcx
-   180005f5f:	shl    $0x4,%rax
-   180005f63:	mov    %rcx,0x28(%rsp)
-   180005f68:	mov    %rax,0x30(%rsp)
-   180005f6d:	movq   $0x8,0x38(%rsp)
-   180005f76:	jmp    0x180005f81
-   180005f78:	movq   $0x0,0x38(%rsp)
-   180005f81:	lea    0x40(%rsp),%rcx
-   180005f86:	lea    0x28(%rsp),%r9
-   180005f8b:	call   0x180005d90
-   180005f90:	cmpq   $0x0,0x40(%rsp)
-   180005f96:	mov    0x48(%rsp),%rcx
-   180005f9b:	je     0x180005fbd
-   180005f9d:	mov    0x50(%rsp),%rdx
-   180005fa2:	movabs $0x8000000000000001,%rax
-   180005fac:	cmp    %rax,%rdx
-   180005faf:	je     0x180005fc4
-   180005fb1:	test   %rdx,%rdx
-   180005fb4:	jne    0x180005fcb
-   180005fb6:	call   0x18001ef90
-   180005fbb:	ud2
-   180005fbd:	mov    %rcx,(%rsi)
-   180005fc0:	mov    %rdi,0x8(%rsi)
-   180005fc4:	add    $0x58,%rsp
-   180005fc8:	pop    %rdi
-   180005fc9:	pop    %rsi
-   180005fca:	ret
-   180005fcb:	call   0x18002b5f0
-   180005fd0:	ud2
+   180005e5e:	xor    %r8d,%r8d
+   180005e61:	mov    %rdi,%rcx
+   180005e64:	shr    $0x3b,%rcx
+   180005e68:	sete   %r8b
+   180005e6c:	mov    %rdi,%rdx
+   180005e6f:	shl    $0x4,%rdx
+   180005e73:	shl    $0x3,%r8
+   180005e77:	test   %rax,%rax
+   180005e7a:	je     0x180005e98
+   180005e7c:	mov    (%rsi),%rcx
+   180005e7f:	shl    $0x4,%rax
+   180005e83:	mov    %rcx,0x28(%rsp)
+   180005e88:	mov    %rax,0x30(%rsp)
+   180005e8d:	movq   $0x8,0x38(%rsp)
+   180005e96:	jmp    0x180005ea1
+   180005e98:	movq   $0x0,0x38(%rsp)
+   180005ea1:	lea    0x40(%rsp),%rcx
+   180005ea6:	lea    0x28(%rsp),%r9
+   180005eab:	call   0x180005d90
+   180005eb0:	cmpq   $0x0,0x40(%rsp)
+   180005eb6:	mov    0x48(%rsp),%rcx
+   180005ebb:	je     0x180005edd
+   180005ebd:	mov    0x50(%rsp),%rdx
+   180005ec2:	movabs $0x8000000000000001,%rax
+   180005ecc:	cmp    %rax,%rdx
+   180005ecf:	je     0x180005ee4
+   180005ed1:	test   %rdx,%rdx
+   180005ed4:	jne    0x180005eeb
+   180005ed6:	call   0x18001ef90
+   180005edb:	ud2
+   180005edd:	mov    %rcx,(%rsi)
+   180005ee0:	mov    %rdi,0x8(%rsi)
+   180005ee4:	add    $0x58,%rsp
+   180005ee8:	pop    %rdi
+   180005ee9:	pop    %rsi
+   180005eea:	ret
+   180005eeb:	call   0x18002b5f0
+   180005ef0:	ud2
+   180005ef2:	int3
+   180005ef3:	int3
+   180005ef4:	int3
+   180005ef5:	int3
+   180005ef6:	int3
+   180005ef7:	int3
+   180005ef8:	int3
+   180005ef9:	int3
+   180005efa:	int3
+   180005efb:	int3
+   180005efc:	int3
+   180005efd:	int3
+   180005efe:	int3
+   180005eff:	int3
+   180005f00:	push   %rsi
+   180005f01:	push   %rdi
+   180005f02:	sub    $0x58,%rsp
+   180005f06:	inc    %rdx
+   180005f09:	je     0x180005fb5
+   180005f0f:	mov    %rcx,%rsi
+   180005f12:	mov    0x8(%rcx),%rax
+   180005f16:	lea    (%rax,%rax,1),%rcx
+   180005f1a:	cmp    %rdx,%rcx
+   180005f1d:	cmova  %rcx,%rdx
+   180005f21:	cmp    $0x5,%rdx
+   180005f25:	mov    $0x4,%edi
+   180005f2a:	cmovae %rdx,%rdi
+   180005f2e:	movabs $0x555555555555556,%rcx
+   180005f38:	xor    %r8d,%r8d
+   180005f3b:	cmp    %rcx,%rdi
+   180005f3e:	setb   %r8b
+   180005f42:	lea    0x0(,%rdi,8),%rcx
+   180005f4a:	lea    (%rcx,%rcx,2),%rdx
+   180005f4e:	shl    $0x3,%r8
+   180005f52:	test   %rax,%rax
+   180005f55:	je     0x180005f77
+   180005f57:	mov    (%rsi),%rcx
+   180005f5a:	shl    $0x3,%rax
+   180005f5e:	lea    (%rax,%rax,2),%rax
+   180005f62:	mov    %rcx,0x28(%rsp)
+   180005f67:	mov    %rax,0x30(%rsp)
+   180005f6c:	movq   $0x8,0x38(%rsp)
+   180005f75:	jmp    0x180005f80
+   180005f77:	movq   $0x0,0x38(%rsp)
+   180005f80:	lea    0x40(%rsp),%rcx
+   180005f85:	lea    0x28(%rsp),%r9
+   180005f8a:	call   0x180005d90
+   180005f8f:	cmpq   $0x0,0x40(%rsp)
+   180005f95:	mov    0x48(%rsp),%rcx
+   180005f9a:	je     0x180005fbc
+   180005f9c:	mov    0x50(%rsp),%rdx
+   180005fa1:	movabs $0x8000000000000001,%rax
+   180005fab:	cmp    %rax,%rdx
+   180005fae:	je     0x180005fc3
+   180005fb0:	test   %rdx,%rdx
+   180005fb3:	jne    0x180005fca
+   180005fb5:	call   0x18001ef90
+   180005fba:	ud2
+   180005fbc:	mov    %rcx,(%rsi)
+   180005fbf:	mov    %rdi,0x8(%rsi)
+   180005fc3:	add    $0x58,%rsp
+   180005fc7:	pop    %rdi
+   180005fc8:	pop    %rsi
+   180005fc9:	ret
+   180005fca:	call   0x18002b5f0
+   180005fcf:	ud2
+   180005fd1:	int3
    180005fd2:	int3
    180005fd3:	int3
    180005fd4:	int3
    180005fd5:	int3
    180005fd6:	int3
    180005fd7:	int3
    180005fd8:	int3
@@ -10764,15 +10753,15 @@
    180006685:	mov    0x10(%rdx),%rax
    180006689:	mov    %rax,0x40(%rsp)
    18000668e:	movups (%rdx),%xmm0
    180006691:	movaps %xmm0,0x30(%rsp)
    180006696:	lea    0x58(%rsp),%rcx
    18000669b:	lea    0x30(%rsp),%rdx
    1800066a0:	lea    0x2f(%rsp),%r8
-   1800066a5:	call   0x180005790
+   1800066a5:	call   0x180005470
    1800066aa:	mov    0x78(%rsp),%rax
    1800066af:	mov    %rax,0x50(%rsp)
    1800066b4:	movups 0x58(%rsp),%xmm0
    1800066b9:	movups 0x68(%rsp),%xmm1
    1800066be:	movaps %xmm1,0x40(%rsp)
    1800066c3:	movaps %xmm0,0x30(%rsp)
    1800066c8:	decq   0x10(%rdi)
@@ -10834,15 +10823,15 @@
    180006795:	mov    0x10(%rdx),%rax
    180006799:	mov    %rax,0x10(%rbp)
    18000679d:	movups (%rdx),%xmm0
    1800067a0:	movaps %xmm0,0x0(%rbp)
    1800067a4:	lea    -0x60(%rbp),%rcx
    1800067a8:	mov    %rbp,%rdx
    1800067ab:	lea    0x57(%rbp),%r8
-   1800067af:	call   0x180005470
+   1800067af:	call   0x180005710
    1800067b4:	mov    -0x20(%rbp),%rax
    1800067b8:	mov    %rax,0x40(%rbp)
    1800067bc:	movups -0x60(%rbp),%xmm0
    1800067c0:	movups -0x50(%rbp),%xmm1
    1800067c4:	movups -0x40(%rbp),%xmm2
    1800067c8:	movups -0x30(%rbp),%xmm3
    1800067cc:	movaps %xmm3,0x30(%rbp)
@@ -11836,15 +11825,15 @@
    18000746a:	mov    %rcx,%rdi
    18000746d:	mov    0x10(%rcx),%rbx
    180007471:	mov    %rbx,%rax
    180007474:	cmp    0x8(%rcx),%rbx
    180007478:	jne    0x180007489
    18000747a:	mov    %rdi,%rcx
    18000747d:	mov    %rbx,%rdx
-   180007480:	call   0x180005e30
+   180007480:	call   0x180005f00
    180007485:	mov    0x10(%rdi),%rax
    180007489:	mov    (%rdi),%rcx
    18000748c:	lea    (%rax,%rax,2),%rax
    180007490:	mov    0x10(%rsi),%rdx
    180007494:	mov    %rdx,0x10(%rcx,%rax,8)
    180007499:	movups (%rsi),%xmm0
    18000749c:	movups %xmm0,(%rcx,%rax,8)
@@ -12980,26 +12969,26 @@
    18000853b:	mov    (%rcx),%rax
    18000853e:	mov    (%rax),%rsi
    180008541:	mov    0x10(%rax),%rdi
    180008545:	lea    0x30(%rsp),%rcx
    18000854a:	call   0x180025900
    18000854f:	test   %rdi,%rdi
    180008552:	je     0x18000858d
-   180008554:	shl    $0x6,%rdi
+   180008554:	shl    $0x3,%rdi
    180008558:	lea    0x24b81(%rip),%r14        # 0x18002d0e0
    18000855f:	lea    0x30(%rsp),%r15
    180008564:	lea    0x28(%rsp),%rbx
    180008569:	nopl   0x0(%rax)
    180008570:	mov    %rsi,0x28(%rsp)
-   180008575:	add    $0x40,%rsi
+   180008575:	add    $0x8,%rsi
    180008579:	mov    %r15,%rcx
    18000857c:	mov    %rbx,%rdx
    18000857f:	mov    %r14,%r8
    180008582:	call   0x180023960
-   180008587:	add    $0xffffffffffffffc0,%rdi
+   180008587:	add    $0xfffffffffffffff8,%rdi
    18000858b:	jne    0x180008570
    18000858d:	lea    0x30(%rsp),%rcx
    180008592:	call   0x180023980
    180008597:	nop
    180008598:	add    $0x40,%rsp
    18000859c:	pop    %rbx
    18000859d:	pop    %rdi
@@ -13028,26 +13017,26 @@
    1800085bb:	mov    (%rcx),%rax
    1800085be:	mov    (%rax),%rsi
    1800085c1:	mov    0x10(%rax),%rdi
    1800085c5:	lea    0x30(%rsp),%rcx
    1800085ca:	call   0x180025900
    1800085cf:	test   %rdi,%rdi
    1800085d2:	je     0x18000860d
-   1800085d4:	shl    $0x3,%rdi
+   1800085d4:	shl    $0x6,%rdi
    1800085d8:	lea    0x24b21(%rip),%r14        # 0x18002d100
    1800085df:	lea    0x30(%rsp),%r15
    1800085e4:	lea    0x28(%rsp),%rbx
    1800085e9:	nopl   0x0(%rax)
    1800085f0:	mov    %rsi,0x28(%rsp)
-   1800085f5:	add    $0x8,%rsi
+   1800085f5:	add    $0x40,%rsi
    1800085f9:	mov    %r15,%rcx
    1800085fc:	mov    %rbx,%rdx
    1800085ff:	mov    %r14,%r8
    180008602:	call   0x180023960
-   180008607:	add    $0xfffffffffffffff8,%rdi
+   180008607:	add    $0xffffffffffffffc0,%rdi
    18000860b:	jne    0x1800085f0
    18000860d:	lea    0x30(%rsp),%rcx
    180008612:	call   0x180023980
    180008617:	nop
    180008618:	add    $0x40,%rsp
    18000861c:	pop    %rbx
    18000861d:	pop    %rdi
@@ -14502,15 +14491,15 @@
    180009a94:	cmp    $0xa,%rdi
    180009a98:	jb     0x180009970
    180009a9e:	xchg   %ax,%ax
    180009aa0:	cmp    0x78(%rbp),%r14
    180009aa4:	jne    0x180009abd
    180009aa6:	lea    0x70(%rbp),%rcx
    180009aaa:	mov    %r14,%rdx
-   180009aad:	call   0x180005f10
+   180009aad:	call   0x180005e30
    180009ab2:	mov    0x70(%rbp),%rcx
    180009ab6:	mov    0x80(%rbp),%r14
    180009abd:	shl    $0x4,%r14
    180009ac1:	mov    %r12,(%rcx,%r14,1)
    180009ac5:	mov    %rdi,0x8(%rcx,%r14,1)
    180009aca:	mov    0x70(%rbp),%rcx
    180009ace:	mov    0x80(%rbp),%r14
@@ -16450,24 +16439,24 @@
    18000b74c:	movq   $0x0,-0x40(%rbp)
    18000b754:	lea    0x21645(%rip),%rax        # 0x18002cda0
    18000b75b:	mov    %rax,0x20(%rsp)
    18000b760:	lea    0x21609(%rip),%r8        # 0x18002cd70
    18000b767:	lea    -0x40(%rbp),%r9
    18000b76b:	xor    %ecx,%ecx
    18000b76d:	mov    %r14,%rdx
-   18000b770:	call   0x18002b270
+   18000b770:	call   0x18002b200
    18000b775:	ud2
    18000b777:	movq   $0x0,-0x40(%rbp)
    18000b77f:	lea    0x21632(%rip),%rax        # 0x18002cdb8
    18000b786:	mov    %rax,0x20(%rsp)
    18000b78b:	lea    0x8(%rbp),%rdx
    18000b78f:	lea    -0x58(%rbp),%r8
    18000b793:	lea    -0x40(%rbp),%r9
    18000b797:	xor    %ecx,%ecx
-   18000b799:	call   0x18002b200
+   18000b799:	call   0x18002b270
    18000b79e:	ud2
    18000b7a0:	mov    %rdx,0x10(%rsp)
    18000b7a5:	push   %rbp
    18000b7a6:	push   %r15
    18000b7a8:	push   %r14
    18000b7aa:	push   %r13
    18000b7ac:	push   %r12
@@ -16628,24 +16617,24 @@
    18000b9a9:	movq   $0x0,-0x40(%rbp)
    18000b9b1:	lea    0x21418(%rip),%rax        # 0x18002cdd0
    18000b9b8:	mov    %rax,0x20(%rsp)
    18000b9bd:	lea    0x213ac(%rip),%r8        # 0x18002cd70
    18000b9c4:	lea    -0x40(%rbp),%r9
    18000b9c8:	xor    %ecx,%ecx
    18000b9ca:	mov    %r14,%rdx
-   18000b9cd:	call   0x18002b270
+   18000b9cd:	call   0x18002b200
    18000b9d2:	ud2
    18000b9d4:	movq   $0x0,-0x40(%rbp)
    18000b9dc:	lea    0x21405(%rip),%rax        # 0x18002cde8
    18000b9e3:	mov    %rax,0x20(%rsp)
    18000b9e8:	lea    0x8(%rbp),%rdx
    18000b9ec:	lea    -0x58(%rbp),%r8
    18000b9f0:	lea    -0x40(%rbp),%r9
    18000b9f4:	xor    %ecx,%ecx
-   18000b9f6:	call   0x18002b200
+   18000b9f6:	call   0x18002b270
    18000b9fb:	ud2
    18000b9fd:	nopl   (%rax)
    18000ba00:	mov    %rdx,0x10(%rsp)
    18000ba05:	push   %rbp
    18000ba06:	push   %r15
    18000ba08:	push   %r14
    18000ba0a:	push   %r13
@@ -52856,15 +52845,15 @@
    18002b222:	movups 0x20(%r9),%xmm2
    18002b227:	movaps %xmm2,0x70(%rsp)
    18002b22c:	movaps %xmm1,0x60(%rsp)
    18002b231:	movaps %xmm0,0x50(%rsp)
    18002b236:	mov    %rax,0x30(%rsp)
    18002b23b:	lea    0x50(%rsp),%rax
    18002b240:	mov    %rax,0x28(%rsp)
-   18002b245:	lea    0x1eb4(%rip),%r8        # 0x18002d100
+   18002b245:	lea    0x1ed4(%rip),%r8        # 0x18002d120
    18002b24c:	mov    %r8,0x20(%rsp)
    18002b251:	lea    0x40(%rsp),%rdx
    18002b256:	lea    0x48(%rsp),%r9
    18002b25b:	call   0x180023120
    18002b260:	ud2
    18002b262:	int3
    18002b263:	int3
@@ -52889,15 +52878,15 @@
    18002b292:	movups 0x20(%r9),%xmm2
    18002b297:	movaps %xmm2,0x70(%rsp)
    18002b29c:	movaps %xmm1,0x60(%rsp)
    18002b2a1:	movaps %xmm0,0x50(%rsp)
    18002b2a6:	mov    %rax,0x30(%rsp)
    18002b2ab:	lea    0x50(%rsp),%rax
    18002b2b0:	mov    %rax,0x28(%rsp)
-   18002b2b5:	lea    0x1e64(%rip),%r8        # 0x18002d120
+   18002b2b5:	lea    0x1e24(%rip),%r8        # 0x18002d0e0
    18002b2bc:	mov    %r8,0x20(%rsp)
    18002b2c1:	lea    0x40(%rsp),%rdx
    18002b2c6:	lea    0x48(%rsp),%r9
    18002b2cb:	call   0x180023120
    18002b2d0:	ud2
    18002b2d2:	int3
    18002b2d3:	int3
@@ -55037,16 +55026,16 @@
    18002cf32:	add    %al,(%rax)
    18002cf34:	add    %al,(%rax)
    18002cf36:	add    %al,(%rax)
    18002cf38:	or     %al,(%rax)
    18002cf3a:	add    %al,(%rax)
    18002cf3c:	add    %al,(%rax)
    18002cf3e:	add    %al,(%rax)
-   18002cf40:	mov    $0x85,%al
-   18002cf42:	add    %al,0x1(%rax)
+   18002cf40:	xor    %al,0x18000(%rbp)
+   18002cf46:	add    %al,(%rax)
    18002cf48:	push   %rdi
    18002cf49:	outsl  %ds:(%rsi),(%dx)
    18002cf4a:	rex.X imul $0x43676e69,%gs:0x6e(%rsi),%ebp
    18002cf53:	insb   (%dx),%es:(%rdi)
    18002cf54:	jne    0x18002cfc9
    18002cf56:	je     0x18002cfbd
    18002cf58:	jb     0x18002cfc8
@@ -55210,30 +55199,30 @@
    18002d0ea:	add    %al,(%rax)
    18002d0ec:	add    %al,(%rax)
    18002d0ee:	add    %al,(%rax)
    18002d0f0:	or     %al,(%rax)
    18002d0f2:	add    %al,(%rax)
    18002d0f4:	add    %al,(%rax)
    18002d0f6:	add    %al,(%rax)
-   18002d0f8:	add    %dh,0x18000(%rcx)
+   18002d0f8:	nop
+   18002d0f9:	fiadds (%rax)
+   18002d0fb:	addb   $0x0,(%rcx)
    18002d0fe:	add    %al,(%rax)
    18002d100:	shrb   $0x80,0x0(%rax)
    18002d104:	add    %eax,(%rax)
    18002d106:	add    %al,(%rax)
    18002d108:	or     %al,(%rax)
    18002d10a:	add    %al,(%rax)
    18002d10c:	add    %al,(%rax)
    18002d10e:	add    %al,(%rax)
    18002d110:	or     %al,(%rax)
    18002d112:	add    %al,(%rax)
    18002d114:	add    %al,(%rax)
    18002d116:	add    %al,(%rax)
-   18002d118:	nop
-   18002d119:	fiadds (%rax)
-   18002d11b:	addb   $0x0,(%rcx)
+   18002d118:	add    %dh,0x18000(%rcx)
    18002d11e:	add    %al,(%rax)
    18002d120:	shrb   $0x80,0x0(%rax)
    18002d124:	add    %eax,(%rax)
    18002d126:	add    %al,(%rax)
    18002d128:	or     %al,(%rax)
    18002d12a:	add    %al,(%rax)
    18002d12c:	add    %al,(%rax)
@@ -55256,16 +55245,16 @@
    18002d152:	add    %al,(%rax)
    18002d154:	add    %al,(%rax)
    18002d156:	add    %al,(%rax)
    18002d158:	or     %al,(%rax)
    18002d15a:	add    %al,(%rax)
    18002d15c:	add    %al,(%rax)
    18002d15e:	add    %al,(%rax)
-   18002d160:	xor    %al,0x18000(%rbp)
-   18002d166:	add    %al,(%rax)
+   18002d160:	mov    $0x85,%al
+   18002d162:	add    %al,0x1(%rax)
    18002d168:	jae    0x18002d1dc
    18002d16a:	movsxd 0x6f(%rdi,%rsi,2),%ebx
    18002d16e:	gs pop %rdi
    18002d170:	(bad)
    18002d171:	imul   $0x5f676e69,0x6e(%rsi),%ebp
    18002d178:	jo     0x18002d1ec
    18002d17a:	outsl  %ds:(%rsi),(%dx)
@@ -63069,38 +63058,38 @@
    180032191:	ret    $0x8002
    180032194:	add    %eax,(%rax)
    180032196:	add    %al,(%rax)
    180032198:	push   $0x18002c2
    18003219d:	add    %al,(%rax)
    18003219f:	add    %al,(%rax)
    1800321a1:	add    %al,(%rax)
-   1800321a3:	add    %ch,0x64ae90(%rsi)
+   1800321a3:	add    %bl,0x64ae91(%rbp)
    1800321a9:	add    %al,(%rax)
    1800321ab:	add    %al,(%rdx)
    1800321ad:	add    %al,(%rax)
    1800321af:	add    %ah,0x0(%rax)
    1800321b2:	add    %al,(%rax)
    1800321b4:	hlt
    1800321b5:	and    (%rbx),%al
    1800321b7:	add    %dh,%ah
    1800321b9:	adc    (%rbx),%al
    1800321bb:	add    %al,(%rax)
    1800321bd:	add    %al,(%rax)
-   1800321bf:	add    %ch,0x64ae90(%rsi)
+   1800321bf:	add    %bl,0x64ae91(%rbp)
    1800321c5:	add    %al,(%rax)
    1800321c7:	add    %cl,(%rax,%rax,1)
    1800321ca:	add    %al,(%rax)
    1800321cc:	adc    $0x0,%al
    1800321ce:	add    %al,(%rax)
    1800321d0:	push   %rsp
    1800321d1:	and    (%rbx),%eax
    1800321d3:	add    %dl,0x3(%rbx,%rdx,1)
    1800321d7:	add    %al,(%rax)
    1800321d9:	add    %al,(%rax)
-   1800321db:	add    %ch,0x64ae90(%rsi)
+   1800321db:	add    %bl,0x64ae91(%rbp)
    1800321e1:	add    %al,(%rax)
    1800321e3:	add    %cl,0x18000000(%rip)        # 0x1980321e9
    1800321e9:	add    (%rax),%eax
    1800321eb:	add    %ch,0x23(%rax)
    1800321ee:	add    (%rax),%eax
    1800321f0:	push   $0x313
 	...
@@ -63190,15 +63179,15 @@
    1800322f4:	push   %rdx
    1800322f5:	push   %rbx
    1800322f6:	rex.R push %rbx
    1800322f8:	clc
    1800322f9:	movabs %eax,0xe6b243a1db83cdc6
    180032302:	ficompl -0x31(%rbp)
    180032305:	mov    $0x7,%ah
-   180032307:	in     $0x2,%al
+   180032307:	in     $0x3,%al
    180032309:	add    %al,(%rax)
    18003230b:	add    %al,0x3a(%rbx)
    18003230e:	pop    %rsp
    18003230f:	push   %rbp
    180032310:	jae    0x180032377
    180032312:	jb     0x180032387
    180032314:	pop    %rsp
@@ -63853,29 +63842,29 @@
    180032978:	or     %al,%al
    18003297a:	(bad)
    18003297b:	rolb   (%rax,%riz,8)
    18003297e:	add    %al,%dh
    180032980:	add    %edx,(%rbx)
    180032982:	or     (%rax),%al
    180032984:	adc    (%rcx),%eax
-   180032986:	adc    $0xb300c00,%eax
-   18003298b:	push   %rax
-   18003298c:	or     0x9(%rax),%dh
+   180032986:	adc    (%rax),%eax
+   180032988:	or     $0x30,%al
+   18003298a:	or     0xa(%rax),%edx
+   18003298d:	jo     0x180032998
    18003298f:	(bad)
    180032990:	or     %al,%al
    180032992:	(bad)
    180032993:	rolb   (%rax,%riz,8)
    180032996:	add    %al,%dh
    180032998:	add    %edx,(%rbx)
    18003299a:	or     (%rax),%al
    18003299c:	adc    (%rcx),%eax
-   18003299e:	adc    (%rax),%eax
-   1800329a0:	or     $0x30,%al
-   1800329a2:	or     0xa(%rax),%edx
-   1800329a5:	jo     0x1800329b0
+   18003299e:	adc    $0xb300c00,%eax
+   1800329a3:	push   %rax
+   1800329a4:	or     0x9(%rax),%dh
    1800329a7:	(bad)
    1800329a8:	or     %al,%al
    1800329aa:	(bad)
    1800329ab:	rolb   (%rax,%riz,8)
    1800329ae:	add    %al,%dh
    1800329b0:	add    %edx,(%rbx)
    1800329b2:	or     (%rax),%al
@@ -63954,21 +63943,21 @@
    180032a5e:	add    %al,(%rax)
    180032a60:	(bad)
    180032a61:	(bad)
    180032a62:	(bad)
    180032a63:	incl   (%rcx)
    180032a65:	or     $0x6,%al
    180032a67:	add    %cl,(%rcx,%rax,1)
-   180032a6a:	sbb    %eax,(%rax)
+   180032a6a:	adc    %eax,(%rax)
    180032a6c:	add    $0x3700430,%eax
    180032a71:	(bad)
    180032a72:	add    %al,%ah
    180032a74:	add    %ecx,(%rsi,%rax,1)
    180032a77:	add    %cl,(%rcx,%rax,1)
-   180032a7a:	adc    %eax,(%rax)
+   180032a7a:	sbb    %eax,(%rax)
    180032a7c:	add    $0x3700430,%eax
    180032a81:	(bad)
    180032a82:	add    %al,%ah
    180032a84:	sbb    %edx,(%rbx)
    180032a86:	or     %esi,0x520e0313(%rip)        # 0x1d2112d9f
    180032a8c:	or     (%rax),%dh
    180032a8e:	or     %esi,0x8(%rax)
@@ -69963,27 +69952,28 @@
    180037085:	sub    $0x0,%al
    180037087:	add    %cl,%ah
    180037089:	(bad)
    18003708a:	add    %al,(%rax)
    18003708c:	push   $0xffffffffd0000329
    180037091:	(bad)
    180037092:	add    %al,(%rax)
-   180037094:	mov    $0x33,%dh
-   180037096:	add    %al,(%rax)
-   180037098:	push   %rax
-   180037099:	sub    %eax,(%rbx)
-   18003709b:	add    %al,%al
-   18003709d:	xor    (%rax),%eax
+   180037094:	push   %rsi
+   180037095:	xor    $0x0,%al
+   180037097:	add    %ch,0x29(%rax)
+   18003709a:	add    (%rax),%eax
+   18003709c:	(bad)
+   18003709d:	xor    $0x0,%al
    18003709f:	add    %al,0x38(%rsi)
    1800370a2:	add    %al,(%rax)
-   1800370a4:	push   $0x50000329
-   1800370a9:	cmp    %al,(%rax)
-   1800370ab:	add    %ah,(%rdx)
-   1800370ad:	cmp    $0x0,%al
-   1800370af:	add    %al,0x30000329(%rax)
+   1800370a4:	push   %rax
+   1800370a5:	sub    %eax,(%rbx)
+   1800370a7:	add    %dl,0x38(%rax)
+   1800370aa:	add    %al,(%rax)
+   1800370ac:	repnz cmp (%rax),%eax
+   1800370af:	add    %al,0x329(%rax)
    1800370b5:	cmp    $0x0,%al
    1800370b7:	add    %dl,%dl
    1800370b9:	(bad)
    1800370ba:	add    %al,(%rax)
    1800370bc:	cwtl
    1800370bd:	sub    %eax,(%rbx)
    1800370bf:	add    %ah,%al
@@ -70012,18 +70002,20 @@
    1800370f4:	(bad)
    1800370f5:	push   %rsp
    1800370f6:	add    %al,(%rax)
    1800370f8:	add    $0x2a,%al
    1800370fa:	add    (%rax),%eax
    1800370fc:	jo     0x180037152
    1800370fe:	add    %al,(%rax)
-   180037100:	test   %dl,0x0(%rdi)
+   180037100:	adc    %dl,0x0(%rdi)
    180037103:	add    %ah,0x3(%rdx,%rbp,1)
-   180037107:	add    %dl,0x30000057(%rax)
-   18003710d:	pop    %rdx
+   180037107:	add    %dl,(%rax)
+   180037109:	push   %rdi
+   18003710a:	add    %al,(%rax)
+   18003710c:	and    $0x5a,%al
    18003710e:	add    %al,(%rax)
    180037110:	je     0x18003713c
    180037112:	add    (%rax),%eax
    180037114:	xor    %bl,0x0(%rdx)
    180037117:	add    %ah,-0x7bffffa5(%rcx)
    18003711d:	sub    (%rbx),%al
    18003711f:	add    %dh,-0x1fffffa5(%rax)
@@ -70051,26 +70043,33 @@
    180037145:	pop    %rbp
    180037146:	add    %al,(%rax)
    180037148:	and    %ebx,0x0(%rsi)
    18003714b:	add    %bh,0x3(%rbx,%rbp,1)
    18003714f:	add    %dh,(%rax)
    180037151:	pop    %rsi
    180037152:	add    %al,(%rax)
-   180037154:	add    %ebx,0x0(%rdi)
-   180037157:	add    %cl,0x1000032b(%rax)
-   18003715d:	pop    %rdi
-   18003715e:	add    %al,(%rax)
-   180037160:	rcrb   %cl,0x0(%rdi)
-   180037163:	add    %cl,0x32b(%rax)
-   180037169:	(bad)
-   18003716a:	add    %al,(%rax)
-   18003716c:	mulb   0x0(%rdx)
-   18003716f:	add    %dl,0x63000003(%rbx,%rbp,1)
-   180037176:	add    %al,(%rax)
-   180037178:	cmp    $0x63,%al
+   180037154:	repnz pop %rsi
+   180037156:	add    %al,(%rax)
+   180037158:	mov    %ch,(%rbx)
+   18003715a:	add    (%rax),%eax
+   18003715c:	add    %bl,0x0(%rdi)
+   18003715f:	add    %dl,%cl
+   180037161:	pop    %rdi
+   180037162:	add    %al,(%rax)
+   180037164:	mov    %ch,(%rbx)
+   180037166:	add    (%rax),%eax
+   180037168:	add    %ah,0x0(%rax)
+   18003716b:	add    %dh,%dh
+   18003716d:	(bad)
+   18003716e:	add    %al,(%rax)
+   180037170:	xchg   %eax,%esp
+   180037171:	sub    (%rbx),%eax
+   180037173:	add    %al,(%rax)
+   180037175:	movsxd (%rax),%eax
+   180037177:	add    %bh,(%rbx,%riz,2)
    18003717a:	add    %al,(%rax)
    18003717c:	mov    $0x2b,%ah
    18003717e:	add    (%rax),%eax
    180037180:	rex movsxd (%rax),%eax
    180037183:	add    %al,-0x37ffff9d(%rbp)
    180037189:	sub    (%rbx),%eax
    18003718b:	add    %dl,-0x33ffff9d(%rax)
@@ -70491,15 +70490,16 @@
    180037605:	out    %eax,$0x0
    180037607:	add    %ch,0x3c(%rax)
    18003760a:	add    (%rax),%eax
    18003760c:	adc    %ch,%al
    18003760e:	add    %al,(%rax)
    180037610:	cmp    %ebp,%esp
    180037612:	add    %al,(%rax)
-   180037614:	subb   $0x3,(%rcx)
+   180037614:	cwtl
+   180037615:	sub    %eax,(%rbx)
    180037617:	add    %al,-0x14(%rax)
    18003761a:	add    %al,(%rax)
    18003761c:	(bad)
    18003761d:	in     (%dx),%eax
    18003761e:	add    %al,(%rax)
    180037620:	mov    $0xe000033c,%esp
    180037625:	in     (%dx),%eax
@@ -71223,15 +71223,16 @@
    180037d09:	lea    (%rcx),%eax
    180037d0b:	add    %al,(%rdx)
    180037d0d:	pop    (%rcx)
    180037d0f:	add    %al,(%rdx,%rax,2)
    180037d12:	add    (%rax),%eax
    180037d14:	adc    %cl,-0x6510ffff(%rdi)
    180037d1a:	add    %eax,(%rax)
-   180037d1c:	subb   $0x3,(%rcx)
+   180037d1c:	cwtl
+   180037d1d:	sub    %eax,(%rbx)
    180037d1f:	add    %dh,%al
    180037d21:	(bad)
    180037d22:	add    %eax,(%rax)
    180037d24:	(bad)
    180037d25:	movabs 0xa0300003505c0001,%al
    180037d2e:	add    %eax,(%rax)
    180037d30:	shlb   %cl,0x50740001(%rcx)
```

### Comparing `woebin-python-0.1.3/woebin/__init__.py` & `woebin-python-0.1.4/woebin/__init__.py`

 * *Files identical despite different names*

### Comparing `woebin-python-0.1.3/woebin_python.egg-info/PKG-INFO` & `woebin-python-0.1.4/woebin_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: woebin-python
-Version: 0.1.3
+Version: 0.1.4
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # woebin
```

