# Comparing `tmp/dingtalk-stream-0.6.2.tar.gz` & `tmp/dingtalk-stream-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dingtalk-stream-0.6.2.tar", last modified: Mon Jul 10 08:12:20 2023, max compression
+gzip compressed data, was "dingtalk-stream-0.7.0.tar", last modified: Wed Jul 12 01:21:54 2023, max compression
```

## Comparing `dingtalk-stream-0.6.2.tar` & `dingtalk-stream-0.7.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:12:20.879393 dingtalk-stream-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-10 08:12:18.000000 dingtalk-stream-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-07-10 08:12:20.879393 dingtalk-stream-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-07-10 08:12:18.000000 dingtalk-stream-0.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:12:20.875393 dingtalk-stream-0.6.2/dingtalk_stream/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-10 08:12:18.000000 dingtalk-stream-0.6.2/dingtalk_stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-07-10 08:12:18.000000 dingtalk-stream-0.6.2/dingtalk_stream/card_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     9052 2023-07-10 08:12:18.000000 dingtalk-stream-0.6.2/dingtalk_stream/card_replier.py
--rw-r--r--   0 runner    (1001) docker     (123)    18427 2023-07-10 08:12:18.000000 dingtalk-stream-0.6.2/dingtalk_stream/chatbot.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-10 08:12:18.000000 dingtalk-stream-0.6.2/dingtalk_stream/credential.py
--rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-07-10 08:12:18.000000 dingtalk-stream-0.6.2/dingtalk_stream/frames.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-07-10 08:12:18.000000 dingtalk-stream-0.6.2/dingtalk_stream/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-07-10 08:12:18.000000 dingtalk-stream-0.6.2/dingtalk_stream/interactive_card.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-10 08:12:18.000000 dingtalk-stream-0.6.2/dingtalk_stream/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     8443 2023-07-10 08:12:18.000000 dingtalk-stream-0.6.2/dingtalk_stream/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-10 08:12:18.000000 dingtalk-stream-0.6.2/dingtalk_stream/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:12:20.879393 dingtalk-stream-0.6.2/dingtalk_stream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-07-10 08:12:20.000000 dingtalk-stream-0.6.2/dingtalk_stream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-10 08:12:20.000000 dingtalk-stream-0.6.2/dingtalk_stream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 08:12:20.000000 dingtalk-stream-0.6.2/dingtalk_stream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-10 08:12:20.000000 dingtalk-stream-0.6.2/dingtalk_stream.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-10 08:12:20.000000 dingtalk-stream-0.6.2/dingtalk_stream.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 08:12:20.879393 dingtalk-stream-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-10 08:12:18.000000 dingtalk-stream-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:21:54.629850 dingtalk-stream-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-12 01:21:53.000000 dingtalk-stream-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-07-12 01:21:54.629850 dingtalk-stream-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-07-12 01:21:53.000000 dingtalk-stream-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:21:54.629850 dingtalk-stream-0.7.0/dingtalk_stream/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-12 01:21:53.000000 dingtalk-stream-0.7.0/dingtalk_stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-07-12 01:21:53.000000 dingtalk-stream-0.7.0/dingtalk_stream/card_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9052 2023-07-12 01:21:53.000000 dingtalk-stream-0.7.0/dingtalk_stream/card_replier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23572 2023-07-12 01:21:53.000000 dingtalk-stream-0.7.0/dingtalk_stream/chatbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-12 01:21:53.000000 dingtalk-stream-0.7.0/dingtalk_stream/credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-07-12 01:21:53.000000 dingtalk-stream-0.7.0/dingtalk_stream/frames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-07-12 01:21:53.000000 dingtalk-stream-0.7.0/dingtalk_stream/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11930 2023-07-12 01:21:53.000000 dingtalk-stream-0.7.0/dingtalk_stream/interactive_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-12 01:21:53.000000 dingtalk-stream-0.7.0/dingtalk_stream/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8443 2023-07-12 01:21:53.000000 dingtalk-stream-0.7.0/dingtalk_stream/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-12 01:21:53.000000 dingtalk-stream-0.7.0/dingtalk_stream/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 01:21:54.629850 dingtalk-stream-0.7.0/dingtalk_stream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-07-12 01:21:54.000000 dingtalk-stream-0.7.0/dingtalk_stream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-12 01:21:54.000000 dingtalk-stream-0.7.0/dingtalk_stream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 01:21:54.000000 dingtalk-stream-0.7.0/dingtalk_stream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-12 01:21:54.000000 dingtalk-stream-0.7.0/dingtalk_stream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-12 01:21:54.000000 dingtalk-stream-0.7.0/dingtalk_stream.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 01:21:54.629850 dingtalk-stream-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-12 01:21:53.000000 dingtalk-stream-0.7.0/setup.py
```

### Comparing `dingtalk-stream-0.6.2/LICENSE` & `dingtalk-stream-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.6.2/PKG-INFO` & `dingtalk-stream-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dingtalk-stream
-Version: 0.6.2
+Version: 0.7.0
 Summary: A Python library for sending messages to DingTalk chatbot
 Home-page: https://github.com/open-dingtalk/dingtalk-stream-sdk-python
 Author: Ke Jie
 Author-email: jinxi.kj@alibaba-inc.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dingtalk-stream-0.6.2/README.md` & `dingtalk-stream-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.6.2/dingtalk_stream/__init__.py` & `dingtalk-stream-0.7.0/dingtalk_stream/__init__.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.6.2/dingtalk_stream/card_instance.py` & `dingtalk-stream-0.7.0/dingtalk_stream/card_instance.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.6.2/dingtalk_stream/card_replier.py` & `dingtalk-stream-0.7.0/dingtalk_stream/card_replier.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.6.2/dingtalk_stream/chatbot.py` & `dingtalk-stream-0.7.0/dingtalk_stream/chatbot.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from .stream import CallbackHandler, CallbackMessage
 from .frames import AckMessage, Headers
 from .interactive_card import generate_multi_text_line_card_data
 from .utils import DINGTALK_OPENAPI_ENDPOINT
 from concurrent.futures import ThreadPoolExecutor
 import uuid
 from .card_instance import MarkdownCardInstance, AIMarkdownCardInstance
+import traceback
 
 
 class AtUser(object):
     def __init__(self):
         self.dingtalk_id = None
         self.staff_id = None
         self.extensions = {}
@@ -65,14 +66,55 @@
     def to_dict(self):
         result = self.extensions.copy()
         if self.content is not None:
             result['content'] = self.content
         return result
 
 
+class ImageContent(object):
+
+    def __init__(self):
+        self.download_code = None
+
+    @classmethod
+    def from_dict(cls, d):
+        content = ImageContent()
+        for name, value in d.items():
+            if name == 'downloadCode':
+                content.download_code = value
+        return content
+
+    def to_dict(self):
+        result = {}
+        if self.download_code is not None:
+            result['downloadCode'] = self.download_code
+        return result
+
+
+class RichTextContent(object):
+
+    def __init__(self):
+        self.rich_text_list = None
+
+    @classmethod
+    def from_dict(cls, d):
+        content = RichTextContent()
+        content.rich_text_list = []
+        for name, value in d.items():
+            if name == 'richText':
+                content.rich_text_list = value
+        return content
+
+    def to_dict(self):
+        result = {}
+        if self.rich_text_list is not None:
+            result['richText'] = self.rich_text_list
+        return result
+
+
 class ChatbotMessage(object):
     TOPIC = '/v1.0/im/bot/messages/get'
     text: TextContent
 
     def __init__(self):
         self.is_in_at_list = None
         self.session_webhook = None
@@ -88,14 +130,16 @@
         self.text = None
         self.conversation_type = None
         self.at_users = []
         self.chatbot_corp_id = None
         self.sender_corp_id = None
         self.conversation_title = None
         self.message_type = None
+        self.image_content = None
+        self.rich_text_content = None
         self.sender_staff_id = None
 
         self.extensions = {}
 
     @classmethod
     def from_dict(cls, d):
         msg = ChatbotMessage()
@@ -119,28 +163,32 @@
                 msg.chatbot_user_id = value
             elif name == 'conversationId':
                 msg.conversation_id = value
             elif name == 'isAdmin':
                 msg.is_admin = value
             elif name == 'createAt':
                 msg.create_at = value
-            elif name == 'text':
-                msg.text = TextContent.from_dict(value)
             elif name == 'conversationType':
                 msg.conversation_type = value
             elif name == 'atUsers':
                 msg.at_users = [AtUser.from_dict(i) for i in value]
             elif name == 'chatbotCorpId':
                 msg.chatbot_corp_id = value
             elif name == 'senderCorpId':
                 msg.sender_corp_id = value
             elif name == 'conversationTitle':
                 msg.conversation_title = value
             elif name == 'msgtype':
                 msg.message_type = value
+                if value == 'text':
+                    msg.text = TextContent.from_dict(d['text'])
+                elif value == 'picture':
+                    msg.image_content = ImageContent.from_dict(d['content'])
+                elif value == 'richText':
+                    msg.rich_text_content = RichTextContent.from_dict(d['content'])
             elif name == 'senderStaffId':
                 msg.sender_staff_id = value
             else:
                 msg.extensions[name] = value
         return msg
 
     def to_dict(self):
@@ -165,14 +213,18 @@
             result['conversationId'] = self.conversation_id
         if self.is_admin is not None:
             result['isAdmin'] = self.is_admin
         if self.create_at is not None:
             result['createAt'] = self.create_at
         if self.text is not None:
             result['text'] = self.text.to_dict()
+        if self.image_content is not None:
+            result['content'] = self.image_content.to_dict()
+        if self.rich_text_content is not None:
+            result['content'] = self.rich_text_content.to_dict()
         if self.conversation_type is not None:
             result['conversationType'] = self.conversation_type
         if self.at_users is not None:
             result['atUsers'] = [i.to_dict() for i in self.at_users]
         if self.chatbot_corp_id is not None:
             result['chatbotCorpId'] = self.chatbot_corp_id
         if self.sender_corp_id is not None:
@@ -181,14 +233,36 @@
             result['conversationTitle'] = self.conversation_title
         if self.message_type is not None:
             result['msgtype'] = self.message_type
         if self.sender_staff_id is not None:
             result['senderStaffId'] = self.sender_staff_id
         return result
 
+    def get_text_list(self):
+        if self.message_type == 'text':
+            return [self.text.content]
+        elif self.message_type == 'richText':
+            text = []
+            for item in self.rich_text_content.rich_text_list:
+                if 'text' in item:
+                    text.append(item["text"])
+
+            return text
+
+    def get_image_list(self):
+        if self.message_type == 'picture':
+            return [self.image_content.download_code]
+        elif self.message_type == 'richText':
+            images = []
+            for item in self.rich_text_content.rich_text_list:
+                if 'downloadCode' in item:
+                    images.append(item['downloadCode'])
+
+            return images
+
     def __str__(self):
         return 'ChatbotMessage(message_type=%s, text=%s, sender_nick=%s, conversation_title=%s)' % (
             self.message_type,
             self.text,
             self.sender_nick,
             self.conversation_title,
         )
@@ -229,14 +303,83 @@
         """
         ai_markdown_card_instance = AIMarkdownCardInstance(self.dingtalk_client, incoming_message)
         ai_markdown_card_instance.set_title_and_logo(title, logo)
 
         ai_markdown_card_instance.ai_start()
         return ai_markdown_card_instance
 
+    def extract_text_from_incoming_message(self, incoming_message: ChatbotMessage) -> list:
+        """
+        获取文本列表
+        :param incoming_message:
+        :return: text list。如果是纯文本消息，结果列表中只有一个元素；如果是富文本消息，结果是长列表，按富文本消息的逻辑分割，大致是按换行符分割的。
+        """
+        return incoming_message.get_text_list()
+
+    def extract_image_from_incoming_message(self, incoming_message: ChatbotMessage) -> list:
+        """
+        获取用户发送的图片，重新上传，获取新的mediaId列表
+        :param incoming_message:
+        :return: mediaid list
+        """
+        image_list = incoming_message.get_image_list()
+        if image_list is None or len(image_list) == 0:
+            return None
+
+        mediaids = []
+        for download_code in image_list:
+            download_url = self.get_image_download_url(download_code)
+
+            image_content = requests.get(download_url)
+            mediaid = self.dingtalk_client.upload_to_dingtalk(image_content.content, filetype='image',
+                                                              filename='image.png',
+                                                              mimetype='image/png')
+
+            mediaids.append(mediaid)
+
+        return mediaids
+
+    def get_image_download_url(self, download_code: str) -> str:
+        """
+        根据downloadCode获取下载链接 https://open.dingtalk.com/document/isvapp/download-the-file-content-of-the-robot-receiving-message
+        :param download_code:
+        :return:
+        """
+        access_token = self.dingtalk_client.get_access_token()
+        if not access_token:
+            self.logger.error('send_off_duty_prompt failed, cannot get dingtalk access token')
+            return None
+
+        request_headers = {
+            'Content-Type': 'application/json',
+            'Accept': '*/*',
+            'x-acs-dingtalk-access-token': access_token,
+            'User-Agent': ('DingTalkStream/1.0 SDK/0.1.0 Python/%s '
+                           '(+https://github.com/open-dingtalk/dingtalk-stream-sdk-python)'
+                           ) % platform.python_version(),
+        }
+
+        values = {
+            'robotCode': self.dingtalk_client.credential.client_id,
+            'downloadCode': download_code,
+        }
+
+        url = DINGTALK_OPENAPI_ENDPOINT + '/v1.0/robot/messageFiles/download'
+
+        try:
+            response = requests.post(url,
+                                     headers=request_headers,
+                                     data=json.dumps(values))
+
+            response.raise_for_status()
+        except Exception as e:
+            self.logger.error('get_image_download_url, error=%s, response=%s', e, response.text)
+            return ""
+        return response.json()["downloadUrl"]
+
     def set_off_duty_prompt(self, text: str, title: str = "", logo: str = ""):
         """
         设置离线提示词，需要使用OpenAPI，当前仅支持自建应用。
         :param text: 离线提示词，支持markdown
         :param title: 机器人名称，默认："钉钉Stream机器人"
         :param logo: 机器人logo，默认："@lALPDfJ6V_FPDmvNAfTNAfQ"
         :return:
@@ -478,15 +621,15 @@
         return AckMessage.STATUS_NOT_IMPLEMENT, 'not implement'
 
     async def raw_process(self, callback_message: CallbackMessage):
         def func():
             try:
                 self.process(callback_message)
             except Exception as e:
-                self.logger.error('async process exception, error=%s', e)
+                self.logger.error(traceback.format_exc())
 
         self.async_executor.submit(func)
 
         ack_message = AckMessage()
         ack_message.code = AckMessage.STATUS_OK
         ack_message.headers.message_id = callback_message.headers.message_id
         ack_message.headers.content_type = Headers.CONTENT_TYPE_APPLICATION_JSON
```

### Comparing `dingtalk-stream-0.6.2/dingtalk_stream/frames.py` & `dingtalk-stream-0.7.0/dingtalk_stream/frames.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.6.2/dingtalk_stream/handlers.py` & `dingtalk-stream-0.7.0/dingtalk_stream/handlers.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.6.2/dingtalk_stream/interactive_card.py` & `dingtalk-stream-0.7.0/dingtalk_stream/interactive_card.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.6.2/dingtalk_stream/stream.py` & `dingtalk-stream-0.7.0/dingtalk_stream/stream.py`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.6.2/dingtalk_stream.egg-info/PKG-INFO` & `dingtalk-stream-0.7.0/dingtalk_stream.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dingtalk-stream
-Version: 0.6.2
+Version: 0.7.0
 Summary: A Python library for sending messages to DingTalk chatbot
 Home-page: https://github.com/open-dingtalk/dingtalk-stream-sdk-python
 Author: Ke Jie
 Author-email: jinxi.kj@alibaba-inc.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dingtalk-stream-0.6.2/dingtalk_stream.egg-info/SOURCES.txt` & `dingtalk-stream-0.7.0/dingtalk_stream.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dingtalk-stream-0.6.2/setup.py` & `dingtalk-stream-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='dingtalk-stream',
-    version='0.6.2',
+    version='0.7.0',
     description='A Python library for sending messages to DingTalk chatbot',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/open-dingtalk/dingtalk-stream-sdk-python',
     author='Ke Jie',
     author_email='jinxi.kj@alibaba-inc.com',
     license='MIT',
```

