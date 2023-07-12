# Comparing `tmp/promptrix-0.3.0.tar.gz` & `tmp/promptrix-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptrix-0.3.0.tar", last modified: Sat Jul  8 01:26:00 2023, max compression
+gzip compressed data, was "promptrix-0.3.1.tar", last modified: Wed Jul 12 01:37:06 2023, max compression
```

## Comparing `promptrix-0.3.0.tar` & `promptrix-0.3.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-08 01:26:00.392543 promptrix-0.3.0/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-01 23:37:06.000000 promptrix-0.3.0/LICENSE
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2163 2023-07-08 01:26:00.392543 promptrix-0.3.0/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1607 2023-06-15 20:10:06.000000 promptrix-0.3.0/README.md
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      833 2023-07-08 01:25:51.000000 promptrix-0.3.0/pyproject.toml
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-07-08 01:26:00.392543 promptrix-0.3.0/setup.cfg
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-08 01:26:00.392543 promptrix-0.3.0/src/
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-08 01:26:00.392543 promptrix-0.3.0/src/promptrix/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      759 2023-06-27 16:18:19.000000 promptrix-0.3.0/src/promptrix/AssistantMessage.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2576 2023-06-27 16:18:52.000000 promptrix-0.3.0/src/promptrix/ConversationHistory.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1164 2023-06-05 23:10:10.000000 promptrix-0.3.0/src/promptrix/FunctionRegistry.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      607 2023-06-14 17:33:19.000000 promptrix-0.3.0/src/promptrix/GPT3Tokenizer.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1187 2023-06-15 17:06:46.000000 promptrix-0.3.0/src/promptrix/GroupSection.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     5159 2023-06-15 17:06:10.000000 promptrix-0.3.0/src/promptrix/LayoutEngine.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      421 2023-06-02 18:46:08.000000 promptrix-0.3.0/src/promptrix/Prompt.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2507 2023-07-07 19:01:24.000000 promptrix-0.3.0/src/promptrix/PromptSectionBase.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      475 2023-06-02 18:46:08.000000 promptrix-0.3.0/src/promptrix/SystemMessage.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     5879 2023-07-07 18:58:41.000000 promptrix-0.3.0/src/promptrix/TemplateSection.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      821 2023-06-02 18:46:08.000000 promptrix-0.3.0/src/promptrix/TextSection.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      636 2023-06-14 17:01:45.000000 promptrix-0.3.0/src/promptrix/UserMessage.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      746 2023-07-07 18:57:37.000000 promptrix-0.3.0/src/promptrix/Utilities.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      936 2023-06-19 22:47:47.000000 promptrix-0.3.0/src/promptrix/VolatileMemory.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:55.000000 promptrix-0.3.0/src/promptrix/__init__.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1494 2023-06-02 18:46:08.000000 promptrix-0.3.0/src/promptrix/promptrixTypes.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-08 01:26:00.392543 promptrix-0.3.0/src/promptrix.egg-info/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2163 2023-07-08 01:26:00.000000 promptrix-0.3.0/src/promptrix.egg-info/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      710 2023-07-08 01:26:00.000000 promptrix-0.3.0/src/promptrix.egg-info/SOURCES.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-07-08 01:26:00.000000 promptrix-0.3.0/src/promptrix.egg-info/dependency_links.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       71 2023-07-08 01:26:00.000000 promptrix-0.3.0/src/promptrix.egg-info/requires.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       10 2023-07-08 01:26:00.000000 promptrix-0.3.0/src/promptrix.egg-info/top_level.txt
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-12 01:37:06.002371 promptrix-0.3.1/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-01 23:37:06.000000 promptrix-0.3.1/LICENSE
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2163 2023-07-12 01:37:06.002371 promptrix-0.3.1/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1607 2023-06-15 20:10:06.000000 promptrix-0.3.1/README.md
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      833 2023-07-12 01:35:42.000000 promptrix-0.3.1/pyproject.toml
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-07-12 01:37:06.002371 promptrix-0.3.1/setup.cfg
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-12 01:37:05.998371 promptrix-0.3.1/src/
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-12 01:37:06.002371 promptrix-0.3.1/src/promptrix/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      759 2023-06-27 16:18:19.000000 promptrix-0.3.1/src/promptrix/AssistantMessage.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2564 2023-07-10 15:48:31.000000 promptrix-0.3.1/src/promptrix/ConversationHistory.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1164 2023-06-05 23:10:10.000000 promptrix-0.3.1/src/promptrix/FunctionRegistry.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      608 2023-07-08 17:46:06.000000 promptrix-0.3.1/src/promptrix/GPT3Tokenizer.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1175 2023-07-10 15:49:05.000000 promptrix-0.3.1/src/promptrix/GroupSection.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     4967 2023-07-10 15:54:08.000000 promptrix-0.3.1/src/promptrix/LayoutEngine.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      421 2023-06-02 18:46:08.000000 promptrix-0.3.1/src/promptrix/Prompt.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2489 2023-07-10 15:51:54.000000 promptrix-0.3.1/src/promptrix/PromptSectionBase.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      475 2023-06-02 18:46:08.000000 promptrix-0.3.1/src/promptrix/SystemMessage.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     5155 2023-07-10 15:52:28.000000 promptrix-0.3.1/src/promptrix/TemplateSection.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      815 2023-07-10 15:52:42.000000 promptrix-0.3.1/src/promptrix/TextSection.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      636 2023-06-14 17:01:45.000000 promptrix-0.3.1/src/promptrix/UserMessage.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      746 2023-07-07 18:57:37.000000 promptrix-0.3.1/src/promptrix/Utilities.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      936 2023-06-19 22:47:47.000000 promptrix-0.3.1/src/promptrix/VolatileMemory.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:55.000000 promptrix-0.3.1/src/promptrix/__init__.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1494 2023-06-02 18:46:08.000000 promptrix-0.3.1/src/promptrix/promptrixTypes.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-12 01:37:06.002371 promptrix-0.3.1/src/promptrix.egg-info/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2163 2023-07-12 01:37:05.000000 promptrix-0.3.1/src/promptrix.egg-info/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      710 2023-07-12 01:37:05.000000 promptrix-0.3.1/src/promptrix.egg-info/SOURCES.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-07-12 01:37:05.000000 promptrix-0.3.1/src/promptrix.egg-info/dependency_links.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       71 2023-07-12 01:37:05.000000 promptrix-0.3.1/src/promptrix.egg-info/requires.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       10 2023-07-12 01:37:05.000000 promptrix-0.3.1/src/promptrix.egg-info/top_level.txt
```

### Comparing `promptrix-0.3.0/LICENSE` & `promptrix-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `promptrix-0.3.0/PKG-INFO` & `promptrix-0.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptrix
-Version: 0.3.0
+Version: 0.3.1
 Summary: Promptrix. A prompt layout manager for LLMs
 Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
 Project-URL: Homepage, https://tuuyi.io/promptrix
 Project-URL: Bug Tracker, https://github.com/Stevenic/promptrix-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `promptrix-0.3.0/README.md` & `promptrix-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `promptrix-0.3.0/pyproject.toml` & `promptrix-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "promptrix"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
   { name="Steven Ickman", email="author@example.com" },
   { name="Bruce DAmbrosio", email="bruce.dambrosio@gmail.com" },
 ]
 
 description = "Promptrix. A prompt layout manager for LLMs"
 #documentation = "https://github.com/Stevenic/promptrix-py/README.md"
```

### Comparing `promptrix-0.3.0/src/promptrix/AssistantMessage.py` & `promptrix-0.3.1/src/promptrix/AssistantMessage.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.3.0/src/promptrix/ConversationHistory.py` & `promptrix-0.3.1/src/promptrix/ConversationHistory.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 class ConversationHistory(PromptSectionBase):
     def __init__(self, variable, tokens=1.0, required=False, userPrefix='user', assistantPrefix='assistant', separator='\n'):
         super().__init__(tokens, required, separator)
         self.variable = variable
         self.userPrefix = userPrefix
         self.assistantPrefix = assistantPrefix
 
-    async def renderAsText(self, memory, functions, tokenizer, maxTokens):
+    def renderAsText(self, memory, functions, tokenizer, maxTokens):
         history = memory.get(self.variable)
         if history is None: history=[]
         tokens = 0
         budget = min(self.tokens, maxTokens) if self.tokens > 1.0 else maxTokens
         separatorLength = len(tokenizer.encode(self.separator))
         lines = []
         for i in range(len(history)-1, -1, -1):
@@ -28,15 +28,15 @@
                 continue
             if tokens + length > budget:
                 break
             tokens += length
             lines.insert(0, line)
         return RenderedPromptSection(output=self.separator.join(lines), length=tokens, tooLong=tokens > maxTokens)
 
-    async def renderAsMessages(self, memory, functions, tokenizer, maxTokens):
+    def renderAsMessages(self, memory, functions, tokenizer, maxTokens):
         history = memory.get(self.variable)
         if history is None: history = []
         tokens = 0
         budget = min(self.tokens, maxTokens) if self.tokens > 1.0 else maxTokens
         messages = []
         for i in range(len(history)-1, -1, -1):
             msg = history[i]
```

### Comparing `promptrix-0.3.0/src/promptrix/FunctionRegistry.py` & `promptrix-0.3.1/src/promptrix/FunctionRegistry.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.3.0/src/promptrix/GPT3Tokenizer.py` & `promptrix-0.3.1/src/promptrix/GPT3Tokenizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import List
-from transformers import AutoModelForCausalLM, AutoTokenizer, LlamaTokenizer, StoppingCriteria, StoppingCriteriaList, TextIteratorStreamer
+#from transformers import AutoModelForCausalLM, AutoTokenizer, LlamaTokenizer, StoppingCriteria, StoppingCriteriaList, TextIteratorStreamer
 import tiktoken
 enc = tiktoken.get_encoding("cl100k_base")
 assert enc.decode(enc.encode("hello world")) == "hello world"
 
 class GPT3Tokenizer:
     def __init__(self):
         self.ttk = tiktoken.get_encoding("cl100k_base")
```

### Comparing `promptrix-0.3.0/src/promptrix/GroupSection.py` & `promptrix-0.3.1/src/promptrix/GroupSection.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,14 @@
 class GroupSection(PromptSectionBase):
     def __init__(self, sections: List[PromptSection], role: str = 'system', tokens: int = -1, required: bool = True, separator: str = '\n\n', textPrefix: str = 'system'):
         super().__init__(tokens, required, separator, textPrefix)
         self._layoutEngine = LayoutEngine(sections, tokens, required, separator)
         self.sections = sections
         self.role = role
 
-    async def renderAsMessages(self, memory: PromptMemory, functions: PromptFunctions, tokenizer: Tokenizer, maxTokens: int):
+    def renderAsMessages(self, memory: PromptMemory, functions: PromptFunctions, tokenizer: Tokenizer, maxTokens: int):
         # Render sections to text
-        renderedPromptSection = await self._layoutEngine.renderAsText(memory, functions, tokenizer, maxTokens)
+        renderedPromptSection = self._layoutEngine.renderAsText(memory, functions, tokenizer, maxTokens)
         output = renderedPromptSection.output
         length = renderedPromptSection.length
         # Return output as a single message
         return self.return_messages([{'role': self.role, 'content': output}], length, tokenizer, maxTokens)
```

### Comparing `promptrix-0.3.0/src/promptrix/LayoutEngine.py` & `promptrix-0.3.1/src/promptrix/LayoutEngine.py`

 * *Files 19% similar despite different names*

```diff
@@ -22,37 +22,37 @@
         self.tokens = tokens
         self.separator = separator
 
 class LayoutEngine(PromptSection):
     def __init__(self, sections: List[PromptSection], tokens: int, required: bool, separator: str):
         super().__init__(sections, tokens, required, separator)
 
-    async def renderAsText(self, memory, functions, tokenizer, maxTokens):
+    def renderAsText(self, memory, functions, tokenizer, maxTokens):
         layout = []
         self.addSectionsToLayout(self.sections, layout)
 
-        remaining = await self.layoutSections(
+        remaining = self.layoutSections(
             layout,
             maxTokens,
             lambda section: section.renderAsText(memory, functions, tokenizer, maxTokens),
             lambda section, remaining: section.renderAsText(memory, functions, tokenizer, remaining),
             True,
             tokenizer
         )
 
         output = [section.layout.output for section in layout if section.layout]
         text = self.separator.join(output)
         return RenderedPromptSection(text, len(tokenizer.encode(text)), remaining < 0)
 
-    async def renderAsMessages(self, memory: 'PromptMemory', functions: 'PromptFunctions', tokenizer: 'Tokenizer', maxTokens: int) -> RenderedPromptSection:
+    def renderAsMessages(self, memory: 'PromptMemory', functions: 'PromptFunctions', tokenizer: 'Tokenizer', maxTokens: int) -> RenderedPromptSection:
 
         layout = []
         self.addSectionsToLayout(self.sections, layout)
 
-        remaining = await self.layoutSections(
+        remaining = self.layoutSections(
             layout,
             maxTokens,
             lambda section: section.renderAsMessages(memory, functions, tokenizer, maxTokens),
             lambda section, remaining: section.renderAsMessages(memory, functions, tokenizer, remaining)
         )
 
         output = [message for section in layout if section.layout for message in section.layout.output]
@@ -61,48 +61,46 @@
     def addSectionsToLayout(self, sections: List[PromptSection], layout: List):
         for section in sections:
             if isinstance(section, LayoutEngine):
                 self.addSectionsToLayout(section.sections, layout)
             else:
                 layout.append(PromptSectionLayout(section))
 
-    async def layoutSections(self, layout, maxTokens, cbFixed, cbProportional, textLayout=False, tokenizer=None):
-        await self.layoutFixedSections(layout, cbFixed)
+    def layoutSections(self, layout, maxTokens, cbFixed, cbProportional, textLayout=False, tokenizer=None):
+        self.layoutFixedSections(layout, cbFixed)
 
         remaining = maxTokens - self.getLayoutLength(layout, textLayout, tokenizer)
         while remaining < 0 and self.dropLastOptionalSection(layout):
             remaining = maxTokens - self.getLayoutLength(layout, textLayout, tokenizer)
 
         if self.needsMoreLayout(layout) and remaining > 0:
-            await self.layoutProportionalSections(layout, lambda section: cbProportional(section, remaining))
+            self.layoutProportionalSections(layout, lambda section: cbProportional(section, remaining))
 
             remaining = maxTokens - self.getLayoutLength(layout, textLayout, tokenizer)
             while remaining < 0 and self.dropLastOptionalSection(layout):
                 remaining = maxTokens - self.getLayoutLength(layout, textLayout, tokenizer)
 
         return remaining
 
-    async def layoutFixedSections(self, layout, callback):
+    def layoutFixedSections(self, layout, callback):
 
-        async def process_section(section):
-            output = await callback(section.section)
+        def process_section(section):
+            output = callback(section.section)
             setattr(section, 'layout', output)
 
         tasks = [process_section(section) for section in layout if section.section.tokens < 0 or section.section.tokens > 1.0]
-        await asyncio.gather(*tasks)
         #promises = [callback(section.section).then(lambda output: setattr(section, 'layout', output)) for section in layout if section.section.tokens < 0 or section.section.tokens > 1.0]
-        #await asyncio.gather(*promises)
 
-    async def layoutProportionalSections(self, layout, callback):
-        async def process_section(section):
-            output = await callback(section.section)
+
+    def layoutProportionalSections(self, layout, callback):
+        def process_section(section):
+            output = callback(section.section)
             setattr(section, 'layout', output)
 
         tasks = [process_section(section) for section in layout if 0.0 <= section.section.tokens <= 1.0]
-        await asyncio.gather(*tasks)
 
     def getLayoutLength(self, layout, textLayout=False, tokenizer=None) -> int:
         if textLayout and tokenizer:
             output = [section.layout.output for section in layout if section.layout]
             return len(tokenizer.encode(self.separator.join(output)))
         else:
             return sum(section.layout.length for section in layout if section.layout)
```

### Comparing `promptrix-0.3.0/src/promptrix/PromptSectionBase.py` & `promptrix-0.3.1/src/promptrix/PromptSectionBase.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,19 +11,19 @@
         self.tokens = tokens
         self.separator = separator
         self.text_prefix = text_prefix
         if text_prefix is None:
             raise Exception
 
     @abstractmethod
-    async def renderAsMessages(self, memory, functions, tokenizer, max_tokens):
+    def renderAsMessages(self, memory, functions, tokenizer, max_tokens):
         pass
 
-    async def renderAsText(self, memory, functions, tokenizer, max_tokens):
-        as_messages = await self.renderAsMessages(memory, functions, tokenizer, max_tokens)
+    def renderAsText(self, memory, functions, tokenizer, max_tokens):
+        as_messages = self.renderAsMessages(memory, functions, tokenizer, max_tokens)
         messages = as_messages.output
         text = ''
         for message in messages:
             text += message['content']+'\n'
         #text = self.separator.join([message['content'] for message in messages])
         prefix_length = len(tokenizer.encode(self.text_prefix))
         separator_length = len(tokenizer.encode(self.separator))
```

### Comparing `promptrix-0.3.0/src/promptrix/TemplateSection.py` & `promptrix-0.3.1/src/promptrix/TemplateSection.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,31 +19,23 @@
         super().__init__(tokens, required, separator, text_prefix)
         self.template = template
         self.role = role
         self._parts = []
         self.parse_template()
         #print(f'***** TemplateSection init template {self._parts}')
         
-    async def renderAsMessages(self, memory: 'PromptMemory', functions: 'PromptFunctions', tokenizer: 'Tokenizer', max_tokens: int) -> 'RenderedPromptSection[List[Message]]':
+    def renderAsMessages(self, memory: 'PromptMemory', functions: 'PromptFunctions', tokenizer: 'Tokenizer', max_tokens: int) -> 'RenderedPromptSection[List[Message]]':
         #print(f'***** TemplateSection entry {self._parts}')
         rendered_parts = [part(memory, functions, tokenizer, max_tokens) for part in self._parts]
         text = ''.join(rendered_parts)
         #print(f'***** TemplateSection rendered parts {rendered_parts}')
         length = len(tokenizer.encode(text))
         #print(f'***** TemplateSection rendered parts {text}')
         return self.return_messages([{'role': self.role, 'content': text}], length, tokenizer, max_tokens)
 
-    """
-    async def renderAsMessages(self, memory: 'PromptMemory', functions: 'PromptFunctions', tokenizer: 'Tokenizer', max_tokens: int) -> 'RenderedPromptSection[List[Message]]':
-        rendered_parts = await asyncio.gather(*(part(memory, functions, tokenizer, max_tokens) for part in self._parts))
-        text = ''.join(rendered_parts)
-        length = len(tokenizer.encode(text))
-        return self.return_messages([{'role': self.role, 'content': text}], length, tokenizer, max_tokens)
-    """
-    
     def parse_template(self):
         part = ''
         state = ParseState.IN_TEXT
         string_delim = ''
         skip_next = False
         for i in range(len(self.template)):
             if skip_next:
@@ -122,13 +114,9 @@
                 if char == string_delim:
                     save_part()
                     state = ParseState.IN_TEXT
                 else:
                     part += char
         save_part()
         
-        #def renderer(memory, functions, tokenizer, max_tokens):
-        #    value = await functions.invoke(name, memory, functions, tokenizer, args)
-        #    return Utilities.to_string(tokenizer, value)
-
         return lambda memory, functions, tokenizer, max_tokens: Utilities.to_string(tokenizer, functions.invoke(name, memory, functions, tokenizer, args))
```

### Comparing `promptrix-0.3.0/src/promptrix/TextSection.py` & `promptrix-0.3.1/src/promptrix/TextSection.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,12 +4,12 @@
 class TextSection(PromptSectionBase):
     def __init__(self, text: str, role: str, tokens: int = -1, required: bool = True, separator: str = '\n', text_prefix: str = None):
         super().__init__(tokens, required, separator, text_prefix)
         self.text = text
         self.role = role
         self._length = -1
 
-    async def renderAsMessages(self, memory: PromptMemory, functions: PromptFunctions, tokenizer: Tokenizer, max_tokens: int):
+    def renderAsMessages(self, memory: PromptMemory, functions: PromptFunctions, tokenizer: Tokenizer, max_tokens: int):
         if self._length < 0:
             self._length = len(tokenizer.encode(self.text))
 
         return self.return_messages([{'role': self.role, 'content': self.text}], self._length, tokenizer, max_tokens)
```

### Comparing `promptrix-0.3.0/src/promptrix/UserMessage.py` & `promptrix-0.3.1/src/promptrix/UserMessage.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.3.0/src/promptrix/Utilities.py` & `promptrix-0.3.1/src/promptrix/Utilities.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.3.0/src/promptrix/VolatileMemory.py` & `promptrix-0.3.1/src/promptrix/VolatileMemory.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.3.0/src/promptrix/promptrixTypes.py` & `promptrix-0.3.1/src/promptrix/promptrixTypes.py`

 * *Files identical despite different names*

### Comparing `promptrix-0.3.0/src/promptrix.egg-info/PKG-INFO` & `promptrix-0.3.1/src/promptrix.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptrix
-Version: 0.3.0
+Version: 0.3.1
 Summary: Promptrix. A prompt layout manager for LLMs
 Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
 Project-URL: Homepage, https://tuuyi.io/promptrix
 Project-URL: Bug Tracker, https://github.com/Stevenic/promptrix-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `promptrix-0.3.0/src/promptrix.egg-info/SOURCES.txt` & `promptrix-0.3.1/src/promptrix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

