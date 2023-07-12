# Comparing `tmp/SempCode-0.5.2.13-py3-none-any.whl.zip` & `tmp/SempCode-0.5.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,12 @@
-Zip file size: 6394 bytes, number of entries: 9
+Zip file size: 7766 bytes, number of entries: 10
 -rw-rw-rw-  2.0 fat     1808 b- defN 23-Jul-10 12:58 Semp/Command.py
+-rw-rw-rw-  2.0 fat     1814 b- defN 23-Jul-12 09:22 Semp/Progressbar.py
 -rw-rw-rw-  2.0 fat     2390 b- defN 23-Jul-08 10:25 Semp/SempWrite.py
--rw-rw-rw-  2.0 fat     5623 b- defN 23-Jul-11 09:52 Semp/__init__.py
+-rw-rw-rw-  2.0 fat     6606 b- defN 23-Jul-12 09:22 Semp/__init__.py
 -rw-rw-rw-  2.0 fat      370 b- defN 23-Jul-08 11:54 Semp/about.py
 -rw-rw-rw-  2.0 fat     2644 b- defN 23-Jul-11 09:21 Semp/EasyTkinter/__init__.py
--rw-rw-rw-  2.0 fat     1118 b- defN 23-Jul-11 09:53 SempCode-0.5.2.13.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-11 09:53 SempCode-0.5.2.13.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 23-Jul-11 09:53 SempCode-0.5.2.13.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      686 b- defN 23-Jul-11 09:53 SempCode-0.5.2.13.dist-info/RECORD
-9 files, 14736 bytes uncompressed, 5222 bytes compressed:  64.6%
+-rw-rw-rw-  2.0 fat     1381 b- defN 23-Jul-12 09:22 SempCode-0.5.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-12 09:22 SempCode-0.5.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 23-Jul-12 09:22 SempCode-0.5.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      750 b- defN 23-Jul-12 09:22 SempCode-0.5.5.dist-info/RECORD
+10 files, 17860 bytes uncompressed, 6504 bytes compressed:  63.6%
```

## zipnote {}

```diff
@@ -1,28 +1,31 @@
 Filename: Semp/Command.py
 Comment: 
 
+Filename: Semp/Progressbar.py
+Comment: 
+
 Filename: Semp/SempWrite.py
 Comment: 
 
 Filename: Semp/__init__.py
 Comment: 
 
 Filename: Semp/about.py
 Comment: 
 
 Filename: Semp/EasyTkinter/__init__.py
 Comment: 
 
-Filename: SempCode-0.5.2.13.dist-info/METADATA
+Filename: SempCode-0.5.5.dist-info/METADATA
 Comment: 
 
-Filename: SempCode-0.5.2.13.dist-info/WHEEL
+Filename: SempCode-0.5.5.dist-info/WHEEL
 Comment: 
 
-Filename: SempCode-0.5.2.13.dist-info/top_level.txt
+Filename: SempCode-0.5.5.dist-info/top_level.txt
 Comment: 
 
-Filename: SempCode-0.5.2.13.dist-info/RECORD
+Filename: SempCode-0.5.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Semp/__init__.py

```diff
@@ -1,18 +1,19 @@
 """
     Semp Python Tool by Win12Home
-    Version:0.5.2.13 Beta
+    Version:0.5.3.3 Beta
     
 """
 from PIL import Image,ImageTk
 from requests import *
 from sys import set_int_max_str_digits as max
 from subprocess import Popen
 from random import randint
 from datetime import datetime
+from time import time
 
 
 max(0)
 BINARY_TRUE="BTRUE"
 BINARY_FALSE="BFALSE"
 
 AUTO="AutoEnter"
@@ -25,14 +26,17 @@
 class BoolError(Exception):
     def __init__(self, *args, **kwargs):
         pass
 
 class ArgumentError(Exception):
     def __init__(self, *args, **kwargs):
         pass
+class OtherError(Exception):
+    def __init__(self,*args,**kwargs):
+        pass
 
 def PhotoTk(file: str = ...):
     photo=Image.open(file)
     #Open Photo
     tkphoto=ImageTk.PhotoImage(image=photo)
     #Save Photo
     return tkphoto
@@ -60,24 +64,24 @@
         for __count in range(5):
             temps=sslist[randint(0,len(sslist)-1)]
         password+=temps
     return password
 
 
 class request_simplifies:
-    def Download(website: str = ...,name: str = ...,binary: bool = ...):
+    def Download(website: str = ...,name: str = ...,binary=...):
         r = get(website)
         if binary == True or binary == BINARY_TRUE:
             with open(name, "wb") as f:
-                for chunk in r.iter_content(chunk_size=512):
+                for chunk in r.iter_content(chunk_size=5120):
                     f.write(chunk)
         #This method can download JPG file, EXE file, PNG file, etc
         elif binary == False or binary == BINARY_FALSE:
             with open(name, "wb") as f:
-                for chunk in r.iter_content(chunk_size=512):
+                for chunk in r.iter_content(chunk_size=5120):
                     f.write(chunk)
         #This method can download TXT file, JSON file, JS file, etc
         else:
             raise BoolError("Not be "+str(name)+".Expected BINARY_TRUE or BINARY_FALSE")
     def ResponseGet(website: str = ...):
         r=get(website)
         return {"Status_Code":r.status_code,"URL":r.url,"Text":r.text}
@@ -147,26 +151,57 @@
         for word in text:
             markdown+=word
         with open(name,"w") as f:
             f.write(markdown)
     else:
         raise ArgumentError("Not in AUTO or NONE")
 
-def GetTime(format:str = "%Y.%m.%d %H:%M:%S"):
+def GetTime(format:str = "%Y.%m.%d %I:%M:%S %p"):
     return datetime.now().strftime(format)
 
 def NowDate():
     return datetime.now()
 
 def Date(year:int = ...,month:int = ...,day: int = ...):
     return datetime(year,month,day)
 
 def DateWeekday(datevar):
     weekday={1:"Monday",2:"Tuesday",3:"Wednesday",4:"Thursday",5:"Friday",6:"Saturday",7:"Sunday"}
     return weekday[int(datevar.isoweekday())]
+
+def Translator(text: str = ...):
+    url = 'http://fanyi.youdao.com/translate'
+    data = {
+        "i": text,
+        "from": "AUTO",
+        "to": "AUTO",
+        "smartresult": "dict",
+        "client": "fanyideskweb",
+        "salt": "16081210430989",
+        "doctype": "json",
+        "version": "2.1",
+        "keyfrom": "fanyi.web",
+        "action": "FY_BY_CLICKBUTTION"
+    }
+    try:
+        res = post(url, data=data).json()
+        sys = res['translateResult'][0][0]
+        inc=0
+        word=""
+        for __count in range(1000):
+            try:
+                word += res['translateResult'][0][inc]["tgt"]
+                word += " "
+                inc+=1
+            except Exception:
+                break
+        return word
+    except:
+        raise OtherError("Request Error")
+
 """
 Here are some examples.
 Response(variable):
     response=Requester("https://1.1.1.1/")
     response.ResponseGet()
 Response(code):
     request_simplifies.ResponseGet("https://1.1.1.1/")
@@ -182,8 +217,10 @@
     root.title("Test")
     img=PhotoTk("C:/test.jpg")
     a=Label(self,image=img)
     a.pack()
     root.mainloop()
 Markdown Creator:
     CreateMarkdown("Hello World!",["They are some example","They are some example"],"README.md")
+Translator:
+    Translator("Hello World!")
 """
```

## Comparing `SempCode-0.5.2.13.dist-info/METADATA` & `SempCode-0.5.5.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SempCode
-Version: 0.5.2.13
+Version: 0.5.5
 Summary: Simplified the Python Code
 Author: 是真的Win12Home
 Author-email: mcdhj-work@outlook.com
 License: Mozilla Public License Version 2.0
 Classifier: Development Status :: 4 - Beta
 Requires: requests
 Requires: pillow
@@ -17,14 +17,20 @@
 Description-Content-Type: text/markdown
 
 ---
 Hello Semp!
 ---
 Semp is can simple some code in Python.\
 **1.Updates**\
+*v0.5.3.3(Update)*\
+Add Translator\
+Add Semp.Progressbar\
+----Add VirtualProgressbar(description:str,time:int)\
+----Add EasyProgressbar() Notice:Default VirtualProgressbar\
+----Add DownloadProgressbar(description:str,website:str,name:str,chunk_size:int=None)\
 *v0.5.2.13(Update)*\
 Add CreatePassword(length)\
 Add CreateMarkdown(title,text:list[],name,auto=AUTO/NONE)\
 Add GetTime(format="%Y.%m.%d %H:%M:%S")\
 Add NowDate()\
 Add Date(year,month,day)\
 Add DateWeekday(datevar(NowDate/Date))\
```

## Comparing `SempCode-0.5.2.13.dist-info/RECORD` & `SempCode-0.5.5.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 Semp/Command.py,sha256=UsUVJF2yeo7Ur_yUQDI68lhpxD1qVu4AHp8nm5LvCnA,1808
+Semp/Progressbar.py,sha256=L2u2CvYo1grxlQYn3JoSVFFs_9mMaDrPYjmp8r3jOhg,1814
 Semp/SempWrite.py,sha256=RDlzqY7yFAZjXh5w8LlGtoaDHJ9U9czvO5p_MW7N3sc,2390
-Semp/__init__.py,sha256=_wNXvVUt7Ymd3Nt_norihuSeyQf5ZNz67cXMG4WHKTM,5623
+Semp/__init__.py,sha256=GPnVRbvindBjZZHpUBThF3ATJbblc0WeAxaYKhN2zBw,6606
 Semp/about.py,sha256=6dnRbFTZdDyFoMssu3qYmZtdWQhjDqU2VgN4jryIwpk,370
 Semp/EasyTkinter/__init__.py,sha256=mf16bL8THEjsuRgolX2yxrE3_r4KXNdPVx9hmBt-7pU,2644
-SempCode-0.5.2.13.dist-info/METADATA,sha256=3C9bGoPHZ0Lbo2rPgGeLvEHUTpLbFgthceErbbRI9DM,1118
-SempCode-0.5.2.13.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-SempCode-0.5.2.13.dist-info/top_level.txt,sha256=Di-SqoMJG3xW7CoY0ksMcZ_26p4QE8NuQV9einW_26k,5
-SempCode-0.5.2.13.dist-info/RECORD,,
+SempCode-0.5.5.dist-info/METADATA,sha256=fpsL0GsMDieG6HJ00piZ3H-6myGMyC9SibJrjFlOkLU,1381
+SempCode-0.5.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+SempCode-0.5.5.dist-info/top_level.txt,sha256=Di-SqoMJG3xW7CoY0ksMcZ_26p4QE8NuQV9einW_26k,5
+SempCode-0.5.5.dist-info/RECORD,,
```

