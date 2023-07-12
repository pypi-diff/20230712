# Comparing `tmp/paper-qa-3.2.1.tar.gz` & `tmp/paper-qa-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paper-qa-3.2.1.tar", last modified: Tue Jul 11 16:39:18 2023, max compression
+gzip compressed data, was "paper-qa-3.3.0.tar", last modified: Wed Jul 12 20:44:11 2023, max compression
```

## Comparing `paper-qa-3.2.1.tar` & `paper-qa-3.3.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:39:18.912966 paper-qa-3.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-11 16:38:25.000000 paper-qa-3.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-07-11 16:39:18.912966 paper-qa-3.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17701 2023-07-11 16:38:25.000000 paper-qa-3.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:39:18.908966 paper-qa-3.2.1/paper_qa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-07-11 16:39:18.000000 paper-qa-3.2.1/paper_qa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-11 16:39:18.000000 paper-qa-3.2.1/paper_qa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 16:39:18.000000 paper-qa-3.2.1/paper_qa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-11 16:39:18.000000 paper-qa-3.2.1/paper_qa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-11 16:39:18.000000 paper-qa-3.2.1/paper_qa.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:39:18.912966 paper-qa-3.2.1/paperqa/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-11 16:38:25.000000 paper-qa-3.2.1/paperqa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-07-11 16:38:25.000000 paper-qa-3.2.1/paperqa/chains.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:39:18.912966 paper-qa-3.2.1/paperqa/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-11 16:38:25.000000 paper-qa-3.2.1/paperqa/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-07-11 16:38:25.000000 paper-qa-3.2.1/paperqa/contrib/zotero.py
--rw-r--r--   0 runner    (1001) docker     (123)    22951 2023-07-11 16:38:25.000000 paper-qa-3.2.1/paperqa/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-11 16:38:25.000000 paper-qa-3.2.1/paperqa/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-11 16:38:25.000000 paper-qa-3.2.1/paperqa/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-07-11 16:38:25.000000 paper-qa-3.2.1/paperqa/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-07-11 16:38:25.000000 paper-qa-3.2.1/paperqa/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-11 16:38:25.000000 paper-qa-3.2.1/paperqa/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-11 16:38:25.000000 paper-qa-3.2.1/paperqa/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 16:39:18.912966 paper-qa-3.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-11 16:38:25.000000 paper-qa-3.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:39:18.912966 paper-qa-3.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    26790 2023-07-11 16:38:25.000000 paper-qa-3.2.1/tests/test_paperqa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:44:11.043539 paper-qa-3.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-12 20:43:24.000000 paper-qa-3.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-07-12 20:44:11.039539 paper-qa-3.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17701 2023-07-12 20:43:24.000000 paper-qa-3.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:44:11.035539 paper-qa-3.3.0/paper_qa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-07-12 20:44:11.000000 paper-qa-3.3.0/paper_qa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-12 20:44:11.000000 paper-qa-3.3.0/paper_qa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 20:44:11.000000 paper-qa-3.3.0/paper_qa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-12 20:44:11.000000 paper-qa-3.3.0/paper_qa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-12 20:44:11.000000 paper-qa-3.3.0/paper_qa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:44:11.039539 paper-qa-3.3.0/paperqa/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-12 20:43:24.000000 paper-qa-3.3.0/paperqa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-07-12 20:43:24.000000 paper-qa-3.3.0/paperqa/chains.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:44:11.039539 paper-qa-3.3.0/paperqa/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-12 20:43:24.000000 paper-qa-3.3.0/paperqa/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-07-12 20:43:24.000000 paper-qa-3.3.0/paperqa/contrib/zotero.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23474 2023-07-12 20:43:24.000000 paper-qa-3.3.0/paperqa/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-12 20:43:24.000000 paper-qa-3.3.0/paperqa/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-12 20:43:24.000000 paper-qa-3.3.0/paperqa/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-07-12 20:43:24.000000 paper-qa-3.3.0/paperqa/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-07-12 20:43:24.000000 paper-qa-3.3.0/paperqa/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-12 20:43:24.000000 paper-qa-3.3.0/paperqa/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 20:43:24.000000 paper-qa-3.3.0/paperqa/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 20:44:11.043539 paper-qa-3.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-12 20:43:24.000000 paper-qa-3.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 20:44:11.039539 paper-qa-3.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    27622 2023-07-12 20:43:24.000000 paper-qa-3.3.0/tests/test_paperqa.py
```

### Comparing `paper-qa-3.2.1/LICENSE` & `paper-qa-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `paper-qa-3.2.1/PKG-INFO` & `paper-qa-3.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 3.2.1
+Version: 3.3.0
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paper-qa-3.2.1/README.md` & `paper-qa-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `paper-qa-3.2.1/paper_qa.egg-info/PKG-INFO` & `paper-qa-3.3.0/paper_qa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 3.2.1
+Version: 3.3.0
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paper-qa-3.2.1/paperqa/chains.py` & `paper-qa-3.3.0/paperqa/chains.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.2.1/paperqa/contrib/zotero.py` & `paper-qa-3.3.0/paperqa/contrib/zotero.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.2.1/paperqa/docs.py` & `paper-qa-3.3.0/paperqa/docs.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     index_path: Optional[Path] = PAPERQA_DIR / name
     embeddings: Embeddings = OpenAIEmbeddings(client=None)
     max_concurrent: int = 5
     deleted_dockeys: Set[DocKey] = set()
     prompts: PromptCollection = PromptCollection()
     memory: bool = False
     memory_model: Optional[BaseChatMemory] = None
+    jit_texts_index: bool = False
 
     # TODO: Not sure how to get this to work
     # while also passing mypy checks
     @validator("llm", "summary_llm")
     def check_llm(cls, v: Union[BaseLanguageModel, str]) -> BaseLanguageModel:
         if type(v) is str:
             return ChatOpenAI(temperature=0.1, model=v, client=None)
@@ -79,14 +80,19 @@
                     output_key="Answer",
                 )
             if v.memory_variables()[0] != "memory":
                 raise ValueError("Memory model must have memory_variables=['memory']")
             return values["memory_model"]
         return None
 
+    def clear_docs(self):
+        self.texts = []
+        self.docs = {}
+        self.docnames = set()
+
     def update_llm(
         self,
         llm: Union[BaseLanguageModel, str],
         summary_llm: Optional[Union[BaseLanguageModel, str]] = None,
     ) -> None:
         """Update the LLM for answering questions."""
         if type(llm) is str:
@@ -276,17 +282,17 @@
         del self.docs[dockey]
         self.deleted_dockeys.add(dockey)
 
     async def adoc_match(
         self, query: str, k: int = 25, get_callbacks: CallbackFactory = lambda x: None
     ) -> Set[DocKey]:
         """Return a list of dockeys that match the query."""
-        if len(self.docs) == 0:
-            return set()
         if self.doc_index is None:
+            if len(self.docs) == 0:
+                return set()
             texts = [doc.citation for doc in self.docs.values()]
             metadatas = [d.dict() for d in self.docs.values()]
             self.doc_index = FAISS.from_texts(
                 texts, metadatas=metadatas, embedding=self.embeddings
             )
         matches = self.doc_index.max_marginal_relevance_search(
             query, k=k + len(self.deleted_dockeys)
@@ -325,19 +331,27 @@
         try:
             self.texts_index = FAISS.load_local(self.index_path, self.embeddings)
         except Exception:
             # they use some special exception type, but I don't want to import it
             self.texts_index = None
         self.doc_index = None
 
-    def _build_texts_index(self):
+    def _build_texts_index(self, keys: Optional[Set[DocKey]] = None):
+        if keys is not None and self.jit_texts_index:
+            del self.texts_index
+            self.texts_index = None
         if self.texts_index is None:
-            raw_texts = [t.text for t in self.texts]
-            text_embeddings = [t.embeddings for t in self.texts]
-            metadatas = [t.dict(exclude={"embeddings", "text"}) for t in self.texts]
+            texts = self.texts
+            if keys is not None:
+                texts = [t for t in texts if t.doc.dockey in keys]
+            if len(texts) == 0:
+                return
+            raw_texts = [t.text for t in texts]
+            text_embeddings = [t.embeddings for t in texts]
+            metadatas = [t.dict(exclude={"embeddings", "text"}) for t in texts]
             self.texts_index = FAISS.from_embeddings(
                 # wow adding list to the zip was tricky
                 text_embeddings=list(zip(raw_texts, text_embeddings)),
                 embedding=self.embeddings,
                 metadatas=metadatas,
             )
 
@@ -380,16 +394,17 @@
         k: int = 3,
         max_sources: int = 5,
         marginal_relevance: bool = True,
         get_callbacks: CallbackFactory = lambda x: None,
     ) -> Answer:
         if len(self.docs) == 0 and self.doc_index is None:
             return answer
+        self._build_texts_index(keys=answer.dockey_filter)
         if self.texts_index is None:
-            self._build_texts_index()
+            return answer
         self.texts_index = cast(VectorStore, self.texts_index)
         _k = k
         if answer.dockey_filter is not None:
             _k = k * 10  # heuristic
         # want to work through indices but less k
         if marginal_relevance:
             matches = self.texts_index.max_marginal_relevance_search(
```

### Comparing `paper-qa-3.2.1/paperqa/prompts.py` & `paper-qa-3.3.0/paperqa/prompts.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.2.1/paperqa/readers.py` & `paper-qa-3.3.0/paperqa/readers.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.2.1/paperqa/types.py` & `paper-qa-3.3.0/paperqa/types.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.2.1/paperqa/utils.py` & `paper-qa-3.3.0/paperqa/utils.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.2.1/setup.py` & `paper-qa-3.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.2.1/tests/test_paperqa.py` & `paper-qa-3.3.0/tests/test_paperqa.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,24 +188,25 @@
     assert doc.llm == doc.summary_llm
 
     doc.update_llm(OpenAI(client=None, temperature=0.1, model="text-ada-001"))
     assert doc.llm == doc.summary_llm
 
 
 def test_evidence():
-    doc_path = "example.txt"
+    doc_path = "example.html"
     with open(doc_path, "w", encoding="utf-8") as f:
         # get wiki page about politician
         r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
         f.write(r.text)
     docs = Docs()
     docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
     evidence = docs.get_evidence(
         Answer(question="For which state was Bates a governor?"), k=1, max_sources=1
     )
+    print(evidence.context)
     assert "Missouri" in evidence.context
     os.remove(doc_path)
 
 
 def test_query():
     docs = Docs()
     docs.add_url(
@@ -252,15 +253,15 @@
             citation="WikiMedia Foundation, 2023, Accessed now",
             dockey="test",
         )
         docs.adoc_match("What is Frederick Bates's greatest accomplishment?")
 
 
 def test_docs_pickle():
-    doc_path = "example.txt"
+    doc_path = "example.html"
     with open(doc_path, "w", encoding="utf-8") as f:
         # get front page of wikipedia
         r = requests.get("https://en.wikipedia.org/wiki/Take_Your_Dog_to_Work_Day")
         f.write(r.text)
     llm = OpenAI(client=None, temperature=0.0, model="text-curie-001")
     docs = Docs(llm=llm)
     docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now", chunk_chars=1000)
@@ -291,15 +292,15 @@
     )
     assert strings_similarity(context1, context2) > 0.75
     # make sure we can query
     docs.query("What date is bring your dog to work in the US?")
 
 
 def test_docs_pickle_no_faiss():
-    doc_path = "example.txt"
+    doc_path = "example.html"
     with open(doc_path, "w", encoding="utf-8") as f:
         # get front page of wikipedia
         r = requests.get("https://en.wikipedia.org/wiki/Take_Your_Dog_to_Work_Day")
         f.write(r.text)
     llm = OpenAI(client=None, temperature=0.0, model="text-curie-001")
     docs = Docs(llm=llm)
     docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now", chunk_chars=1000)
@@ -588,21 +589,21 @@
         template="Answer the question '{question}' "
         "using the country name alone. For example: "
         "A: United States\nA: Canada\nA: Mexico\n\n Using the context:\n\n{context}\n\nA: ",
     )
 
     docs = Docs(prompts=PromptCollection(qa=my_qaprompt))
 
-    doc_path = "example.txt"
+    doc_path = "example.html"
     with open(doc_path, "w", encoding="utf-8") as f:
         # get wiki page about politician
         r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
         f.write(r.text)
     docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
-    answer = docs.query("What country is Bates from?")
+    answer = docs.query("What country is Frederick Bates from?")
     print(answer.answer)
     assert "United States" in answer.answer
 
 
 def test_pre_prompt():
     pre = PromptTemplate(
         input_variables=["question"],
@@ -639,34 +640,34 @@
         r = requests.get("https://en.wikipedia.org/wiki/Frederick_Bates_(politician)")
         f.write(r.text)
     docs.add(doc_path, "WikiMedia Foundation, 2023, Accessed now")
     docs.query("What country is Bates from?")
 
 
 def test_memory():
-    docs = Docs(memory=True, k=3, max_sources=1, llm="gpt-3.5-turbo", key_filter=False)
+    # Not sure why, but gpt-3.5 cannot do this anymore.
+    docs = Docs(memory=True, k=3, max_sources=1, llm="gpt-4", key_filter=False)
     docs.add_url(
         "https://en.wikipedia.org/wiki/Red_Army",
         citation="WikiMedia Foundation, 2023, Accessed now",
         dockey="test",
     )
     answer1 = docs.query("When did the Soviet Union and Japan agree to a cease-fire?")
-    print(answer1.answer)
     assert answer1.memory is not None
     assert "1939" in answer1.answer
     assert "Answer" in docs.memory_model.load_memory_variables({})["memory"]
-    answer2 = docs.query("When was the conflict resolved?")
+    answer2 = docs.query("When was it resolved?")
     assert "1941" in answer2.answer or "1945" in answer2.answer
     assert answer2.memory is not None
     assert "Answer" in docs.memory_model.load_memory_variables({})["memory"]
     print(answer2.answer)
 
     docs.clear_memory()
 
-    answer3 = docs.query("When was the conflict resolved?")
+    answer3 = docs.query("When was it resolved?")
     assert answer3.memory is not None
     assert (
         "I cannot answer" in answer3.answer
         or "insufficient" in answer3.answer
         or "does not provide" in answer3.answer
     )
 
@@ -717,7 +718,28 @@
         dockey="test",
     )
     evidence = docs.query(query="What is the date of flag day?", key_filter=True)
     docs2 = Docs(doc_index=docs.doc_index, texts_index=docs.texts_index)
     assert len(docs2.docs) == 0
     evidence = docs2.query("What is the date of flag day?", key_filter=True)
     assert "February 15" in evidence.context
+
+
+def test_external_texts_index():
+    docs = Docs(jit_texts_index=True)
+    docs.add_url(
+        "https://en.wikipedia.org/wiki/National_Flag_of_Canada_Day",
+        citation="Flag Day of Canada, WikiMedia Foundation, 2023, Accessed now",
+    )
+    answer = docs.query(query="What is the date of flag day?", key_filter=True)
+    assert "February 15" in answer.answer
+
+    docs.add_url(
+        "https://en.wikipedia.org/wiki/Frederick_Bates_(politician)",
+        citation="Fredrick Bates, WikiMedia Foundation, 2023, Accessed now",
+    )
+
+    answer = docs.query(query="What is the date of flag day?", key_filter=False)
+    assert "February 15" in answer.answer
+
+    answer = docs.query(query="What is the date of flag day?", key_filter=True)
+    assert "February 15" in answer.answer
```

