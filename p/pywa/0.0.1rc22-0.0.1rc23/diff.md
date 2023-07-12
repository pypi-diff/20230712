# Comparing `tmp/pywa-0.0.1rc22-py3-none-any.whl.zip` & `tmp/pywa-0.0.1rc23-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,23 @@
-Zip file size: 32801 bytes, number of entries: 21
+Zip file size: 32962 bytes, number of entries: 21
 -rw-rw-r--  2.0 unx      117 b- defN 23-Jun-27 07:52 pywa/__init__.py
--rw-rw-r--  2.0 unx       26 b- defN 23-Jul-11 09:47 pywa/__version__.py
+-rw-rw-r--  2.0 unx       26 b- defN 23-Jul-12 08:12 pywa/__version__.py
 -rw-rw-r--  2.0 unx    14220 b- defN 23-Jul-10 21:52 pywa/api.py
 -rw-rw-r--  2.0 unx    29401 b- defN 23-Jul-11 08:06 pywa/client.py
 -rw-rw-r--  2.0 unx     7191 b- defN 23-Jul-03 08:28 pywa/errors.py
--rw-rw-r--  2.0 unx    21046 b- defN 23-Jul-10 21:34 pywa/filters.py
+-rw-rw-r--  2.0 unx    21419 b- defN 23-Jul-12 07:53 pywa/filters.py
 -rw-rw-r--  2.0 unx     3846 b- defN 23-Jul-11 08:37 pywa/handlers.py
 -rw-rw-r--  2.0 unx      873 b- defN 23-Jul-09 12:48 pywa/utils.py
 -rw-rw-r--  2.0 unx     4600 b- defN 23-Jul-11 09:43 pywa/webhook.py
 -rw-rw-r--  2.0 unx      336 b- defN 23-Jul-07 13:20 pywa/types/__init__.py
 -rw-rw-r--  2.0 unx     8951 b- defN 23-Jul-10 21:50 pywa/types/base_update.py
--rw-rw-r--  2.0 unx     5347 b- defN 23-Jul-11 09:47 pywa/types/callback.py
+-rw-rw-r--  2.0 unx     5501 b- defN 23-Jul-12 08:11 pywa/types/callback.py
 -rw-rw-r--  2.0 unx     4609 b- defN 23-Jul-09 14:47 pywa/types/media.py
 -rw-rw-r--  2.0 unx    11234 b- defN 23-Jul-09 17:38 pywa/types/message.py
 -rw-rw-r--  2.0 unx     1934 b- defN 23-Jul-07 13:28 pywa/types/message_status.py
 -rw-rw-r--  2.0 unx     9156 b- defN 23-Jul-07 13:38 pywa/types/others.py
--rw-rw-r--  2.0 unx     1066 b- defN 23-Jul-11 09:47 pywa-0.0.1rc22.dist-info/LICENSE
--rw-rw-r--  2.0 unx     4420 b- defN 23-Jul-11 09:47 pywa-0.0.1rc22.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-11 09:47 pywa-0.0.1rc22.dist-info/WHEEL
--rw-rw-r--  2.0 unx        5 b- defN 23-Jul-11 09:47 pywa-0.0.1rc22.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1591 b- defN 23-Jul-11 09:47 pywa-0.0.1rc22.dist-info/RECORD
-21 files, 130061 bytes uncompressed, 30275 bytes compressed:  76.7%
+-rw-rw-r--  2.0 unx     1066 b- defN 23-Jul-12 08:12 pywa-0.0.1rc23.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     4420 b- defN 23-Jul-12 08:12 pywa-0.0.1rc23.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-12 08:12 pywa-0.0.1rc23.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        5 b- defN 23-Jul-12 08:12 pywa-0.0.1rc23.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1591 b- defN 23-Jul-12 08:12 pywa-0.0.1rc23.dist-info/RECORD
+21 files, 130588 bytes uncompressed, 30436 bytes compressed:  76.7%
```

## zipnote {}

```diff
@@ -42,23 +42,23 @@
 
 Filename: pywa/types/message_status.py
 Comment: 
 
 Filename: pywa/types/others.py
 Comment: 
 
-Filename: pywa-0.0.1rc22.dist-info/LICENSE
+Filename: pywa-0.0.1rc23.dist-info/LICENSE
 Comment: 
 
-Filename: pywa-0.0.1rc22.dist-info/METADATA
+Filename: pywa-0.0.1rc23.dist-info/METADATA
 Comment: 
 
-Filename: pywa-0.0.1rc22.dist-info/WHEEL
+Filename: pywa-0.0.1rc23.dist-info/WHEEL
 Comment: 
 
-Filename: pywa-0.0.1rc22.dist-info/top_level.txt
+Filename: pywa-0.0.1rc23.dist-info/top_level.txt
 Comment: 
 
-Filename: pywa-0.0.1rc22.dist-info/RECORD
+Filename: pywa-0.0.1rc23.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pywa/__version__.py

```diff
@@ -1 +1 @@
-__version__ = "0.0.1rc22"
+__version__ = "0.0.1rc23"
```

## pywa/filters.py

```diff
@@ -155,21 +155,29 @@
 
 
 class TextFilter(_BaseUpdateFilter):
     """Useful filters for text messages."""
     
     __message_types__ = (Mt.TEXT,)
 
-    ANY: MessageT = lambda wa, m: m.type == Mt.TEXT
+    ANY: MessageT = lambda wa, m: m.type == Mt.TEXT and not TextFilter.COMMAND(wa, m)
     """
-    Filter for all text messages.
+    Filter for all text messages (excluding commands).
     
     >>> TextFilter.ANY
     """
 
+    COMMAND: MessageT = lambda wa, m: m.type == Mt.TEXT and m.text.startswith(("!", "/", "#"))
+    """
+    Filter for text messages that are commands (start with ``!``, ``/``, or ``#``).
+        - Use TextFilter.command if you want to filter for specific commands or prefixes.
+    
+    >>> TextFilter.COMMAND
+    """
+
     @staticmethod
     def match(*matches: str, ignore_case: bool = False) -> MessageT:
         """
         Filter for text messages that match exactly the given text/s.
             - Aliases: ``same_as``, ``matches``, ``equals``
 
         >>> TextFilter.match("Hello", "Hi")
```

## pywa/types/callback.py

```diff
@@ -24,14 +24,19 @@
         data: The data of the button.
         title: The title of the button.
     """
     reply_to_message: ReplyToMessage
     data: str
     title: str
 
+    @property
+    def message_id_to_reply(self) -> str:
+        """The ID of the message to reply to."""
+        return self.reply_to_message.message_id
+
     @classmethod
     def from_dict(cls, client: WhatsApp, value: dict):
         message = value['messages'][0]
         return cls(
             _client=client,
             id=message['id'],
             metadata=Metadata.from_dict(**value['metadata']),
```

## Comparing `pywa-0.0.1rc22.dist-info/LICENSE` & `pywa-0.0.1rc23.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pywa-0.0.1rc22.dist-info/METADATA` & `pywa-0.0.1rc23.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywa
-Version: 0.0.1rc22
+Version: 0.0.1rc23
 Summary: Python wrapper for the WhatsApp Cloud API
 Download-URL: https://pypi.org/project/pywa/
 Author: David Lev
 Author-email: davidlev@telegmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/david-lev/pywa#readme
 Project-URL: Issue Tracker, https://github.com/david-lev/pywa/issues
```

## Comparing `pywa-0.0.1rc22.dist-info/RECORD` & `pywa-0.0.1rc23.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 pywa/__init__.py,sha256=u98CpT0wYk8-XDPUGB_hW-a_23agBkzTSzfwmoqnsE0,117
-pywa/__version__.py,sha256=D-r2u3eVXoo2azIv3_4s8SdhUBwONufpw963nS514CQ,26
+pywa/__version__.py,sha256=EH3q0VcLwvMDzDRqHnSGMNxICRaBIEpXlqN-gj5lWiw,26
 pywa/api.py,sha256=xiFBJ-PHNkzN-3HFUXE0YO4xwgTWPDI1PSbafpmRuF0,14220
 pywa/client.py,sha256=wZLrY-weLF1qeOVzmXAZ7M0mONm8yP3yWVuoRjSxkzc,29401
 pywa/errors.py,sha256=ErB0UGIpIOF5vZXK39WmiSrB_PSYvTJL8PLIp90vTjU,7191
-pywa/filters.py,sha256=thOtWYSeFFmLkTJ-cegfQmOfFT5dxV3PnI9DQo6HY6Y,21046
+pywa/filters.py,sha256=X5gXvBnczQCz71ZAuJCE86o25nWpMeATxRDSMRoQ5vo,21419
 pywa/handlers.py,sha256=VD3Z3gocBbxRoHXscBkaP8SONt-M9CDVaiL8duWiL9w,3846
 pywa/utils.py,sha256=vIPGDuXFo80xAhv88mboE-rU-uDEv594cAxEPsMrIZg,873
 pywa/webhook.py,sha256=1IjiwZTYSh5RvRI-DTa2qajVg-tqBQepm_dcHO9rogo,4600
 pywa/types/__init__.py,sha256=HwhabvWT9b1bgPLnvXBDOmYNTh-FYjCC-ot-rh8xqzo,336
 pywa/types/base_update.py,sha256=EW5Fl6rWyCfnIzOQVz7PfCvPzDAnvXlVlqqZh-w4w3c,8951
-pywa/types/callback.py,sha256=5TkToHezrDTWsHw5-4MyzqXHspQGivfhWWlTcXfZMbk,5347
+pywa/types/callback.py,sha256=FbeMxsqWhI8yJ_Rm59BHORvlfGz9ILE_CzpXNHA1Nuk,5501
 pywa/types/media.py,sha256=4T5yOsoZwFmJaTUZf49VnMsXACsGLq1crC6wzSBqanA,4609
 pywa/types/message.py,sha256=zNKvifHA3P89TOxKoV4dLnt-B9jbu7whlP8gdu304Xo,11234
 pywa/types/message_status.py,sha256=wgUlrgTCaKKqEZgVaZt_yYY_PKyJMhBGz-Rh3WaXSB0,1934
 pywa/types/others.py,sha256=UeXSWEY1pekZDVBDacbUsXff_OmYbxbAe9P2o_am4es,9156
-pywa-0.0.1rc22.dist-info/LICENSE,sha256=RwljuP8WgWttLkSivccHoHEFSDhOY8aLM_vg6Ix48yQ,1066
-pywa-0.0.1rc22.dist-info/METADATA,sha256=ZyLhViD4qEkD8WAulMQTdq3y8WIjkRZoilyXAq13dYI,4420
-pywa-0.0.1rc22.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-pywa-0.0.1rc22.dist-info/top_level.txt,sha256=Cl24ggXVvxvOUnQfKRASer1LzHxpYCPZd5ZcVyS98Oo,5
-pywa-0.0.1rc22.dist-info/RECORD,,
+pywa-0.0.1rc23.dist-info/LICENSE,sha256=RwljuP8WgWttLkSivccHoHEFSDhOY8aLM_vg6Ix48yQ,1066
+pywa-0.0.1rc23.dist-info/METADATA,sha256=Fc6REs01GVZmBuX2E9fACr6D4IjdIsNTNyCwkUiiNE8,4420
+pywa-0.0.1rc23.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+pywa-0.0.1rc23.dist-info/top_level.txt,sha256=Cl24ggXVvxvOUnQfKRASer1LzHxpYCPZd5ZcVyS98Oo,5
+pywa-0.0.1rc23.dist-info/RECORD,,
```

