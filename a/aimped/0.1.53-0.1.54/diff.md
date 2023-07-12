# Comparing `tmp/aimped-0.1.53.tar.gz` & `tmp/aimped-0.1.54.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aimped-0.1.53.tar", last modified: Mon Jun 26 18:51:58 2023, max compression
+gzip compressed data, was "dist/aimped-0.1.54.tar", last modified: Wed Jul 12 13:02:41 2023, max compression
```

## Comparing `aimped-0.1.53.tar` & `aimped-0.1.54.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 18:51:58.706464 aimped-0.1.53/
--rw-rw-rw-   0        0        0     1063 2023-04-03 13:18:42.000000 aimped-0.1.53/LICENSE
--rw-rw-rw-   0        0        0     1778 2023-06-26 18:51:58.707456 aimped-0.1.53/PKG-INFO
--rw-rw-rw-   0        0        0     1205 2023-05-24 09:20:26.000000 aimped-0.1.53/README.md
-drwxrwxrwx   0        0        0        0 2023-06-26 18:51:58.657518 aimped-0.1.53/aimped/
--rw-rw-rw-   0        0        0       39 2023-06-26 18:49:01.000000 aimped-0.1.53/aimped/__init__.py
--rw-rw-rw-   0        0        0    13550 2023-06-26 18:40:19.000000 aimped-0.1.53/aimped/io_tasks.py
-drwxrwxrwx   0        0        0        0 2023-06-26 18:51:58.669518 aimped-0.1.53/aimped/model/
--rw-rw-rw-   0        0        0        0 2023-04-03 13:18:42.000000 aimped-0.1.53/aimped/model/__init__.py
--rw-rw-rw-   0        0        0     2338 2023-04-03 13:18:42.000000 aimped-0.1.53/aimped/model/load.py
--rw-rw-rw-   0        0        0      655 2023-06-06 20:37:28.000000 aimped-0.1.53/aimped/models.py
-drwxrwxrwx   0        0        0        0 2023-06-26 18:51:58.671521 aimped-0.1.53/aimped/nitro/
--rw-rw-rw-   0        0        0        0 2023-04-03 13:18:42.000000 aimped-0.1.53/aimped/nitro/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-26 18:51:58.692451 aimped-0.1.53/aimped/nlp/
--rw-rw-rw-   0        0        0      353 2023-04-03 13:18:42.000000 aimped-0.1.53/aimped/nlp/__init__.py
--rw-rw-rw-   0        0        0     2228 2023-04-03 13:18:42.000000 aimped-0.1.53/aimped/nlp/assertion.py
--rw-rw-rw-   0        0        0     3917 2023-04-03 13:18:42.000000 aimped-0.1.53/aimped/nlp/chunker.py
--rw-rw-rw-   0        0        0     2825 2023-04-03 13:18:42.000000 aimped-0.1.53/aimped/nlp/deid.py
--rw-rw-rw-   0        0        0     4521 2023-04-03 13:18:42.000000 aimped-0.1.53/aimped/nlp/ner.py
--rw-rw-rw-   0        0        0     2629 2023-04-03 13:18:42.000000 aimped-0.1.53/aimped/nlp/ner_cls_report.py
--rw-rw-rw-   0        0        0     7055 2023-06-26 17:27:03.000000 aimped-0.1.53/aimped/nlp/pipeline.py
--rw-rw-rw-   0        0        0     3899 2023-04-03 13:18:42.000000 aimped-0.1.53/aimped/nlp/regex_parser.py
--rw-rw-rw-   0        0        0     4394 2023-06-26 17:27:03.000000 aimped-0.1.53/aimped/nlp/relation.py
--rw-rw-rw-   0        0        0    19853 2023-04-03 15:23:07.000000 aimped-0.1.53/aimped/nlp/relation_visualizer.py
--rw-rw-rw-   0        0        0      803 2023-04-03 13:18:42.000000 aimped-0.1.53/aimped/nlp/tokenizer.py
--rw-rw-rw-   0        0        0     2251 2023-04-03 13:18:42.000000 aimped-0.1.53/aimped/nlp/tools.py
--rw-rw-rw-   0        0        0     2587 2023-05-24 09:15:05.000000 aimped-0.1.53/aimped/nlp/translation.py
-drwxrwxrwx   0        0        0        0 2023-06-26 18:51:58.705458 aimped-0.1.53/aimped/test/
--rw-rw-rw-   0        0        0        0 2023-04-03 13:18:42.000000 aimped-0.1.53/aimped/test/__init__.py
--rw-rw-rw-   0        0        0     2748 2023-04-03 13:18:42.000000 aimped-0.1.53/aimped/test/test_assertion.py
--rw-rw-rw-   0        0        0     1313 2023-04-03 13:18:42.000000 aimped-0.1.53/aimped/test/test_chunk_merger.py
--rw-rw-rw-   0        0        0     1866 2023-04-03 13:18:42.000000 aimped-0.1.53/aimped/test/test_deid_pipeline.py
--rw-rw-rw-   0        0        0     1297 2023-04-03 13:18:42.000000 aimped-0.1.53/aimped/test/test_ner_results.py
--rw-rw-rw-   0        0        0     1592 2023-04-03 13:18:42.000000 aimped-0.1.53/aimped/test/test_regex_parser.py
--rw-rw-rw-   0        0        0     3320 2023-04-03 13:18:42.000000 aimped-0.1.53/aimped/test/test_relation_pipeline.py
--rw-rw-rw-   0        0        0      610 2023-04-03 13:18:42.000000 aimped-0.1.53/aimped/test/test_tokenizer.py
--rw-rw-rw-   0        0        0     5585 2023-04-03 13:18:42.000000 aimped-0.1.53/aimped/test/test_translation_pipeline.py
--rw-rw-rw-   0        0        0     2060 2023-06-05 10:53:19.000000 aimped-0.1.53/aimped/utils.py
--rw-rw-rw-   0        0        0      130 2023-06-26 18:48:01.000000 aimped-0.1.53/aimped/version.py
-drwxrwxrwx   0        0        0        0 2023-06-26 18:51:58.667523 aimped-0.1.53/aimped.egg-info/
--rw-rw-rw-   0        0        0     1778 2023-06-26 18:51:58.000000 aimped-0.1.53/aimped.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      952 2023-06-26 18:51:58.000000 aimped-0.1.53/aimped.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 18:51:58.000000 aimped-0.1.53/aimped.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-06-26 18:51:58.000000 aimped-0.1.53/aimped.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-26 18:51:58.000000 aimped-0.1.53/aimped.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      111 2023-06-26 18:51:58.708452 aimped-0.1.53/setup.cfg
--rw-rw-rw-   0        0        0     1176 2023-06-26 18:51:33.000000 aimped-0.1.53/setup.py
+drwxr-xr-x   0 DataScience   (501) staff       (20)        0 2023-07-12 13:02:41.000000 aimped-0.1.54/
+-rw-r--r--   0 DataScience   (501) staff       (20)     1751 2023-07-12 13:02:41.000000 aimped-0.1.54/PKG-INFO
+drwxr-xr-x   0 DataScience   (501) staff       (20)        0 2023-07-12 13:02:41.000000 aimped-0.1.54/aimped/
+-rw-r--r--   0 DataScience   (501) staff       (20)    13257 2023-07-12 10:10:22.000000 aimped-0.1.54/aimped/io_tasks.py
+-rw-r--r--   0 DataScience   (501) staff       (20)      123 2023-07-12 10:26:36.000000 aimped-0.1.54/aimped/version.py
+-rw-r--r--   0 DataScience   (501) staff       (20)      655 2023-07-12 10:10:22.000000 aimped-0.1.54/aimped/models.py
+drwxr-xr-x   0 DataScience   (501) staff       (20)        0 2023-07-12 13:02:41.000000 aimped-0.1.54/aimped/test/
+-rw-r--r--   0 DataScience   (501) staff       (20)     1313 2023-06-24 16:48:55.000000 aimped-0.1.54/aimped/test/test_chunk_merger.py
+-rw-r--r--   0 DataScience   (501) staff       (20)     3320 2023-06-24 16:48:55.000000 aimped-0.1.54/aimped/test/test_relation_pipeline.py
+-rw-r--r--   0 DataScience   (501) staff       (20)      610 2023-06-24 16:48:55.000000 aimped-0.1.54/aimped/test/test_tokenizer.py
+-rw-r--r--   0 DataScience   (501) staff       (20)        0 2023-06-24 16:48:55.000000 aimped-0.1.54/aimped/test/__init__.py
+-rw-r--r--   0 DataScience   (501) staff       (20)     1592 2023-06-24 16:48:55.000000 aimped-0.1.54/aimped/test/test_regex_parser.py
+-rw-r--r--   0 DataScience   (501) staff       (20)     5585 2023-06-24 16:48:55.000000 aimped-0.1.54/aimped/test/test_translation_pipeline.py
+-rw-r--r--   0 DataScience   (501) staff       (20)     1297 2023-06-24 16:48:55.000000 aimped-0.1.54/aimped/test/test_ner_results.py
+-rw-r--r--   0 DataScience   (501) staff       (20)     2748 2023-06-24 16:48:55.000000 aimped-0.1.54/aimped/test/test_assertion.py
+-rw-r--r--   0 DataScience   (501) staff       (20)     1866 2023-06-24 16:48:55.000000 aimped-0.1.54/aimped/test/test_deid_pipeline.py
+-rw-r--r--   0 DataScience   (501) staff       (20)       39 2023-07-12 10:10:22.000000 aimped-0.1.54/aimped/__init__.py
+-rw-r--r--   0 DataScience   (501) staff       (20)     2060 2023-06-24 16:48:55.000000 aimped-0.1.54/aimped/utils.py
+drwxr-xr-x   0 DataScience   (501) staff       (20)        0 2023-07-12 13:02:41.000000 aimped-0.1.54/aimped/model/
+-rw-r--r--   0 DataScience   (501) staff       (20)        0 2023-06-24 16:48:55.000000 aimped-0.1.54/aimped/model/__init__.py
+-rw-r--r--   0 DataScience   (501) staff       (20)     2338 2023-06-24 16:48:55.000000 aimped-0.1.54/aimped/model/load.py
+drwxr-xr-x   0 DataScience   (501) staff       (20)        0 2023-07-12 13:02:41.000000 aimped-0.1.54/aimped/nlp/
+-rw-r--r--   0 DataScience   (501) staff       (20)    19853 2023-06-24 16:48:55.000000 aimped-0.1.54/aimped/nlp/relation_visualizer.py
+-rw-r--r--   0 DataScience   (501) staff       (20)     4290 2023-06-24 17:02:00.000000 aimped-0.1.54/aimped/nlp/relation.py
+-rw-r--r--   0 DataScience   (501) staff       (20)     3917 2023-06-24 16:48:55.000000 aimped-0.1.54/aimped/nlp/chunker.py
+-rw-r--r--   0 DataScience   (501) staff       (20)     2251 2023-06-24 16:48:55.000000 aimped-0.1.54/aimped/nlp/tools.py
+-rw-r--r--   0 DataScience   (501) staff       (20)      353 2023-06-24 16:48:55.000000 aimped-0.1.54/aimped/nlp/__init__.py
+-rw-r--r--   0 DataScience   (501) staff       (20)     2469 2023-07-12 10:17:42.000000 aimped-0.1.54/aimped/nlp/assertion.py
+-rw-r--r--   0 DataScience   (501) staff       (20)      803 2023-06-24 16:48:55.000000 aimped-0.1.54/aimped/nlp/tokenizer.py
+-rw-r--r--   0 DataScience   (501) staff       (20)     2629 2023-06-24 16:48:55.000000 aimped-0.1.54/aimped/nlp/ner_cls_report.py
+-rw-r--r--   0 DataScience   (501) staff       (20)     4521 2023-06-24 16:48:55.000000 aimped-0.1.54/aimped/nlp/ner.py
+-rw-r--r--   0 DataScience   (501) staff       (20)     2825 2023-06-24 16:48:55.000000 aimped-0.1.54/aimped/nlp/deid.py
+-rw-r--r--   0 DataScience   (501) staff       (20)     6947 2023-07-12 10:16:47.000000 aimped-0.1.54/aimped/nlp/pipeline.py
+-rwxr-xr-x   0 DataScience   (501) staff       (20)     2524 2023-06-24 16:48:55.000000 aimped-0.1.54/aimped/nlp/translation.py
+-rw-r--r--   0 DataScience   (501) staff       (20)     3899 2023-06-24 16:48:55.000000 aimped-0.1.54/aimped/nlp/regex_parser.py
+drwxr-xr-x   0 DataScience   (501) staff       (20)        0 2023-07-12 13:02:41.000000 aimped-0.1.54/aimped/nitro/
+-rw-r--r--   0 DataScience   (501) staff       (20)        0 2023-06-24 16:48:55.000000 aimped-0.1.54/aimped/nitro/__init__.py
+-rw-r--r--   0 DataScience   (501) staff       (20)     1063 2023-06-24 16:48:55.000000 aimped-0.1.54/LICENSE
+-rw-r--r--   0 DataScience   (501) staff       (20)     1157 2023-06-24 16:48:55.000000 aimped-0.1.54/README.md
+-rw-r--r--   0 DataScience   (501) staff       (20)     1176 2023-07-12 10:10:22.000000 aimped-0.1.54/setup.py
+drwxr-xr-x   0 DataScience   (501) staff       (20)        0 2023-07-12 13:02:41.000000 aimped-0.1.54/aimped.egg-info/
+-rw-r--r--   0 DataScience   (501) staff       (20)     1751 2023-07-12 13:02:40.000000 aimped-0.1.54/aimped.egg-info/PKG-INFO
+-rw-r--r--   0 DataScience   (501) staff       (20)      952 2023-07-12 13:02:40.000000 aimped-0.1.54/aimped.egg-info/SOURCES.txt
+-rw-r--r--   0 DataScience   (501) staff       (20)       48 2023-07-12 13:02:40.000000 aimped-0.1.54/aimped.egg-info/requires.txt
+-rw-r--r--   0 DataScience   (501) staff       (20)        7 2023-07-12 13:02:40.000000 aimped-0.1.54/aimped.egg-info/top_level.txt
+-rw-r--r--   0 DataScience   (501) staff       (20)        1 2023-07-12 13:02:40.000000 aimped-0.1.54/aimped.egg-info/dependency_links.txt
+-rw-r--r--   0 DataScience   (501) staff       (20)      103 2023-07-12 13:02:41.000000 aimped-0.1.54/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `aimped-0.1.53/LICENSE` & `aimped-0.1.54/LICENSE`

 * *Files identical despite different names*

### Comparing `aimped-0.1.53/PKG-INFO` & `aimped-0.1.54/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,64 +1,68 @@
-Metadata-Version: 2.1
-Name: aimped
-Version: 0.1.53
-Summary: Aimped is a unique library that provides classes and functions for only exclusively business-tailored AI-based NLP models.
-Home-page: https://dev.aimped.ai/
-Author: Russell C.
-Author-email: russell@aimped.com
-Maintainer: aimped
-Maintainer-email: contact@aimped.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# **aimped**
-![aimped](https://dev.aimped.ai/static/media/AimpedBirdLogo.0b3c7cc26d31afe7bd73db496acb01d1.svg)
-
-**Aimped is a unique python library that provides classes and functions for only exclusively business-tailored AI-based NLP models.**  
-
-# Installation  
-```python
-pip install aimped
-```
-
-# Usage  
-```python  
-import aimped
-print(aimped.__version__)
-```
-## Examples  
-
-### Example 1
-
-```python  
-from aimped import nlp
-
-result = nlp.sentence_tokenizer("Hi, welcome to aimped. Explore ai models.",language="english")
-print(result)
-# ['Hi, welcome to aimped.', 'Explore ai models.']
-```
-
-### Example 2
-```python  
-from aimped.nlp.tokenizer import sentence_tokenizer
-
-result = sentence_tokenizer("Hi, welcome to aimped. Explore ai models.",language="english")
-print(result)
-# ['Hi, welcome to aimped.', 'Explore ai models.']
-```
-
-### Example 3
-```python  
-from aimped.nlp.pipeline import Pipeline
-
-pipe = Pipeline(model=model, tokenizer=tokenizer, device='cpu')
-result = pipe.ner_result(
-                        text=text,
-                        sents_tokens_list=sents_tokens_list,
-                        sentences=sentences)
-print(result)
-```
-
+Metadata-Version: 2.1
+Name: aimped
+Version: 0.1.54
+Summary: Aimped is a unique library that provides classes and functions for only exclusively business-tailored AI-based NLP models.
+Home-page: https://dev.aimped.ai/
+Author: Russell C.
+Author-email: russell@aimped.com
+Maintainer: aimped
+Maintainer-email: contact@aimped.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# **aimped**
+![aimped](https://dev.aimped.ai/static/media/AimpedBirdLogo.0b3c7cc26d31afe7bd73db496acb01d1.svg)
+
+**Aimped is a unique python library that provides classes and functions for only exclusively business-tailored AI-based NLP models.**  
+
+# Installation  
+```python
+pip install aimped
+```
+
+# Usage  
+```python  
+import aimped
+print(aimped.__version__)
+```
+## Examples  
+
+### Example 1
+
+```python  
+from aimped import nlp
+
+result = nlp.sentence_tokenizer("Hi, welcome to aimped. Explore ai models.",language="english")
+print(result)
+# ['Hi, welcome to aimped.', 'Explore ai models.']
+```
+
+### Example 2
+```python  
+from aimped.nlp.tokenizer import sentence_tokenizer
+
+result = sentence_tokenizer("Hi, welcome to aimped. Explore ai models.",language="english")
+print(result)
+# ['Hi, welcome to aimped.', 'Explore ai models.']
+```
+
+### Example 3
+```python  
+from aimped.nlp.pipeline import Pipeline
+
+pipe = Pipeline(model=model, tokenizer=tokenizer, device='cpu')
+result = pipe.ner_result(
+                        text=text,
+                        sents_tokens_list=sents_tokens_list,
+                        sentences=sentences)
+print(result)
+```
+
+
+
```

### Comparing `aimped-0.1.53/README.md` & `aimped-0.1.54/README.md`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-# **aimped**
-![aimped](https://dev.aimped.ai/static/media/AimpedBirdLogo.0b3c7cc26d31afe7bd73db496acb01d1.svg)
-
-**Aimped is a unique python library that provides classes and functions for only exclusively business-tailored AI-based NLP models.**  
-
-# Installation  
-```python
-pip install aimped
-```
-
-# Usage  
-```python  
-import aimped
-print(aimped.__version__)
-```
-## Examples  
-
-### Example 1
-
-```python  
-from aimped import nlp
-
-result = nlp.sentence_tokenizer("Hi, welcome to aimped. Explore ai models.",language="english")
-print(result)
-# ['Hi, welcome to aimped.', 'Explore ai models.']
-```
-
-### Example 2
-```python  
-from aimped.nlp.tokenizer import sentence_tokenizer
-
-result = sentence_tokenizer("Hi, welcome to aimped. Explore ai models.",language="english")
-print(result)
-# ['Hi, welcome to aimped.', 'Explore ai models.']
-```
-
-### Example 3
-```python  
-from aimped.nlp.pipeline import Pipeline
-
-pipe = Pipeline(model=model, tokenizer=tokenizer, device='cpu')
-result = pipe.ner_result(
-                        text=text,
-                        sents_tokens_list=sents_tokens_list,
-                        sentences=sentences)
-print(result)
-```
-
+# **aimped**
+![aimped](https://dev.aimped.ai/static/media/AimpedBirdLogo.0b3c7cc26d31afe7bd73db496acb01d1.svg)
+
+**Aimped is a unique python library that provides classes and functions for only exclusively business-tailored AI-based NLP models.**  
+
+# Installation  
+```python
+pip install aimped
+```
+
+# Usage  
+```python  
+import aimped
+print(aimped.__version__)
+```
+## Examples  
+
+### Example 1
+
+```python  
+from aimped import nlp
+
+result = nlp.sentence_tokenizer("Hi, welcome to aimped. Explore ai models.",language="english")
+print(result)
+# ['Hi, welcome to aimped.', 'Explore ai models.']
+```
+
+### Example 2
+```python  
+from aimped.nlp.tokenizer import sentence_tokenizer
+
+result = sentence_tokenizer("Hi, welcome to aimped. Explore ai models.",language="english")
+print(result)
+# ['Hi, welcome to aimped.', 'Explore ai models.']
+```
+
+### Example 3
+```python  
+from aimped.nlp.pipeline import Pipeline
+
+pipe = Pipeline(model=model, tokenizer=tokenizer, device='cpu')
+result = pipe.ner_result(
+                        text=text,
+                        sents_tokens_list=sents_tokens_list,
+                        sentences=sentences)
+print(result)
+```
+
```

### Comparing `aimped-0.1.53/aimped/io_tasks.py` & `aimped-0.1.54/aimped/io_tasks.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,293 +1,293 @@
-# Author Aimped
-# Date: 2023-May-25
-# Description: This file contains standart input and output (sio) keys for each task
-
-from enum import Enum
-import json
-from dataclasses import dataclass, field
-from typing import Any, Dict, List, Union
-
-from pydantic import BaseModel, Extra, Field
-
-data_types = [
-    'data_json',
-    'data_pdf',
-    'data_image',
-    'data_svg',
-    'data_audio',
-    'data_csv',
-    'data_txt',
-    'data_excel',
-    'data_docx',
-    'data_xml',
-    'data_video',
-    'data_zip',
-    'data_char',
-    'data_file',
-    'raw_output',
-    'data_url'
-]
-
-
-################ Task: Text Classification ################
-
-class TextClassificationInput(BaseModel):
-    """Input data for text classification task"""
-    text: List[str] = Field(..., description="List of texts", example=["This is an example text for classification.",
-                                                                       "This is another example text for classification."])
-    class Config:
-        extra = Extra.allow
-
-class TextClassificationOutput(BaseModel):
-    """Output data for text classification task"""
-    status: bool = True
-    data_type: List[str] = Field(default=["data_json"], description="List of data types", enum=data_types)
-    output: Dict[str, Any] = Field(
-        default={"data_json": {"result": None}},
-        description="data_json output dictionary",
-        keys={"enum": data_types},
-        example={
-            'data_json': {
-                'result': [
-                    {
-                        'category': [str],
-                        'classes': [{'label': str, 'score': float},
-                                    {'label': str, 'score': float}]
-                    }
-                ]
-            }
-        }
-    )
-
-    def __init__(self, model_prediction: Any, **data: Any):
-        super().__init__(**data)
-        self.output['data_json']['result'] = model_prediction
-
-
-################ Task: Name Entity Recognition ################
-
-class NameEntityRecognitionInput(BaseModel):
-    """Input data for name entity recognition task"""
-    text: List[str] = Field(..., description="List of texts", example=["This is an example text for NER."])
-    entity: List[Any] = Field(..., description="List of entities", example=["PERSON", "ORG", "GPE"])
-
-    class Config:
-        extra = Extra.allow
-
-
-class NameEntityRecognitionOutput(BaseModel):
-    """Output data for name entity recognition task"""
-    status: bool = True
-    data_type: List[str] = Field(default=["data_json"], description="List of data types", enum=data_types)
-    output: Dict[str, Any] = Field(
-        default={"data_json": {"result": None}},
-        description="Output dictionary",
-        keys={"enum": data_types},
-        example={
-            'data_json': {
-                'result': [
-                    [{
-                        'entity': str,
-                        'confidence': float,
-                        'chunk': str,
-                        'begin': int,
-                        'end': int
-                    }]
-                ]
-            }
-        }
-    )
-
-    def __init__(self, model_prediction: Any, **data: Any):
-        super().__init__(**data)
-        self.output['data_json']['result'] = model_prediction
-
-
-######################### Task: Deidentification #########################
-
-class DeidentificationInput(BaseModel):
-    """Input data for deidentification task"""
-    text: List[str] = Field(..., description="List of texts", example=["This is an example text for deidentification."])
-    entity: List[str] = Field(..., description="List of entities", example=["PERSON", "ORG", "GPE"])
-
-    class Config:
-        extra = Extra.allow
-
-class DeidentificationOutput(BaseModel):
-    """Output data for deidentification task"""
-    status: bool = True
-    data_type: List[str] = Field(default=["data_json"], description="List of data types", enum=data_types)
-    output: Dict[str, Any] = Field(
-                                    default={"data_json": {"result": None}},
-                                    description="Output dictionary",
-                                    keys={"enum": data_types},
-                                    example={
-                                        'data_json': {'result': [
-                                            {'entities': [
-                                                {
-                                                    'entity': str,
-                                                    'confidence': float,
-                                                    'chunk': str,
-                                                    'begin': int,
-                                                    'end': int,
-                                                    'faked_chunk': str
-                                                }],
-                                                'masked_text': str,
-                                                'faked_text': str
-                                            }]
-                                        }}
-                                )
-
-    def __init__(self, model_prediction: Any, **data: Any):
-        super().__init__(**data)
-        self.output['data_json']['result'] = model_prediction
-
-
-####################### Task: Chatbot ###################### TODO: Still in development
-
-class ChatbotInput(BaseModel):
-    """Input data for chatbot task"""
-    messages: List[Dict[str, str]] = Field(..., description="List of messages",
-                                           example=[{"role": "user", "content": "Who are you?"},
-                                                    {"role": "assistant", "content": "I am Chat Bot. Who are you?"},
-                                                    {"role": "user", "content": "I am Joseph."}
-                                                    ])
-    stream: bool = False
-    max_tokens: int = 256
-    temperature: float = 0.7
-
-    class Config:
-        extra = Extra.allow
-
-class ChatbotOutput(BaseModel):
-    """Output data for chatbot task"""
-    status: bool = True
-    data_type: List[str] = Field(default=["data_json", "data_audio"],
-                                 description="List of data types",
-                                 enum=data_types)
-    # data_json: Dict[str, Any] = Field(default=None, description="Text API Output in dictionary", repr=False, exclude=True,)
-    # data_audio: str = Field(default=None, description="Audio API Output in base64 format", repr=False, exclude=True,
-    #                         example="data:audio/mp3;base64,//tQxA-audio-base64-format-string", )
-    raw_output: Dict[str, Any] = Field(default=None, description="Raw API Output in dictionary", repr=False,
-                                       exclude=True)
-    output: Dict[str, Any] = Field(
-        default={"data_json": {"text": None}, "data_audio": None, "raw_output": None},
-        description="Output dictionary",
-        keys={"enum": data_types},
-        example={
-            "data_json": {"text": "Well…   good luck…"},
-            "raw_output": {'choices': [{'message': {'content': 'Well… good luck…', 'role': 'assistant',
-                                                    'finish_reason': 'stop', 'index': 0, }}],
-                           'created': 1683618639,
-                           'id': 'chaxxpl-7EXXXXXwQNqPmXXXXXaYWkMtKNVjg',
-                           'model': 'gpt-3.5-turbo-0301',
-                           'object': 'chat.completion',
-                           'usage': {'completion_tokens': 27,
-                                     'prompt_tokens': 186,
-                                     'total_tokens': 213}},
-            "data_audio": "data:audio/mp3;base64,//tQxA-audio-base64-format-audio-file...==="},
-    )
-
-    def __init__(self, api_text: Any, api_result: Any, api_audio: Any, **data: Any):
-        super().__init__(**data)
-        self.output['data_json']['text'] = api_text
-        self.output['raw_output'] = api_result
-        self.output['data_audio'] = api_audio
-      
-
-######################## Task: OCR ######################## TODO: Still in development
-
-class OcrInput(BaseModel):
-    """Input data for OCR task"""
-    file_type: str = Field(..., description="File type image or pdf", example="image/png")
-    file: str = Field(..., description="File in base64 format", example="data:image/png;base64,//tQxA-image-base64-format-string")
-
-    class Config:
-        extra = Extra.allow
-
-class OcrOutput(BaseModel):
-    """Output data for OCR task"""
-    status: bool = True
-    data_type: List[str] = Field(default=["data_image"], description="List of data types", enum=data_types)
-    output: Dict[str, Any] = Field(
-                                    default={},
-                                    description="Output dictionary",
-                                    keys={"enum": data_types},
-                                    example={"data_image": ["data:image/png;base64,//tQxA-image-base64-format-string"]}
-                                )
-
-    def __init__(self, model_prediction: Any, data_type: List[str]=["data_image"], **data: Any):
-        super().__init__(**data)
-        self.data_type = data_type
-
-        if "data_image" in self.data_type:
-            self.output['data_image'] = model_prediction
-        elif "data_pdf" in self.data_type:
-            self.output['data_pdf'] = model_prediction
-        else:
-            raise ValueError("Invalid data_type, data_type must be data_image or data_pdf")
-        
-######################## Task: Translation ########################
-
-class TranslationInput(BaseModel):
-    """Input data for translation task"""
-    text: List[str] = Field(..., description="List of texts", example=["This is an example text for translation."])
-    source_language: str = Field(..., description="Source language", example="en")
-    output_language: str = Field(..., description="Output language", example="de")
-
-    class Config:
-        extra = Extra.allow
-
-
-class TranslationOutput(BaseModel):
-    """Output data for translation task"""
-    status: bool = True
-    data_type: List[str] = Field(default=["data_json"], description="List of data types one or more item of data_types", enum=data_types)
-    output: Dict[str, Any] = Field(
-                                    default={"data_json": {"result": {'output_language':None, 'translated_text':None}}},
-                                    description="Output dictionary",
-                                    keys={"enum": data_types},
-                                    example={
-                                            "data_json": {
-                                                            "result": {
-                                                                        "output_language": "<output_language>",
-                                                                        "translated_text": ["<translated_text>"]
-                                                                    }}}
-                                )
-
-    def __init__(self, model_prediction: Any, output_language: str, **data: Any):
-        super().__init__(**data)
-        self.output['data_json']['result']['output_language'] = output_language
-        self.output['data_json']['result']['translated_text'] = model_prediction
-
-######################## Task: Auto Speech Recognition ########################
-
-class ASRInput(BaseModel):
-    """Input data for ASR task"""
-    data_type: List[str] = Field(default=["data_audio"], description="List of data types one or more item of data_types", enum=data_types)
-    file: str = Field(default=None, description="File in base64 format", example="data:audio/mp3;base64,//tQxA-audio-base64-format-audio-file...===")
-    url: str = Field(default=None, description="Audio file url", example="https://www.example.com/audio.mp3")
-    translation: bool = Field(default=False, description="Translation flag", example=True)
-    language: str = Field(default=None, description="Language code", example="en")
-
-    class Config:
-        extra = Extra.allow
-
-class ASROutput(BaseModel):
-    status: bool = True
-    data_type: List[str] = Field(default=["data_json"], description="List of data types one or more item of data_types", enum=data_types)
-    output: Dict[str, Any] = Field(default={"data_json": {"transcription":None, 
-                                                          "translation":None, 
-                                                          "segments":None, 
-                                                          "language":None}}, description="Output dictionary", example={"data_json": {"transcription":"transcription_text", "translation": "translation_to_english_text_or_None", "segments": [{"text": "text_chunk_of_transcription.", "start": 0.0, "end": 3.0}], "language": "en"}})
-
-    def __init__(self, transcription:list=None, translation=None, language:str="en", segments: Any=None, **data: Any):
-        super().__init__(**data)
-        self.output['data_json']['transcription'] = transcription
-        self.output['data_json']['translation'] = translation
-        self.output['data_json']['language'] = language
-        self.output['data_json']['segments'] = segments
-
-        class Config:
-            extra = Extra.allow
-
+# Author Aimped
+# Date: 2023-May-25
+# Description: This file contains standart input and output (sio) keys for each task
+
+from enum import Enum
+import json
+from dataclasses import dataclass, field
+from typing import Any, Dict, List, Union
+
+from pydantic import BaseModel, Extra, Field
+
+data_types = [
+    'data_json',
+    'data_pdf',
+    'data_image',
+    'data_svg',
+    'data_audio',
+    'data_csv',
+    'data_txt',
+    'data_excel',
+    'data_docx',
+    'data_xml',
+    'data_video',
+    'data_zip',
+    'data_char',
+    'data_file',
+    'raw_output',
+    'data_url'
+]
+
+
+################ Task: Text Classification ################
+
+class TextClassificationInput(BaseModel):
+    """Input data for text classification task"""
+    text: List[str] = Field(..., description="List of texts", example=["This is an example text for classification.",
+                                                                       "This is another example text for classification."])
+    class Config:
+        extra = Extra.allow
+
+class TextClassificationOutput(BaseModel):
+    """Output data for text classification task"""
+    status: bool = True
+    data_type: List[str] = Field(default=["data_json"], description="List of data types", enum=data_types)
+    output: Dict[str, Any] = Field(
+        default={"data_json": {"result": None}},
+        description="data_json output dictionary",
+        keys={"enum": data_types},
+        example={
+            'data_json': {
+                'result': [
+                    {
+                        'category': [str],
+                        'classes': [{'label': str, 'score': float},
+                                    {'label': str, 'score': float}]
+                    }
+                ]
+            }
+        }
+    )
+
+    def __init__(self, model_prediction: Any, **data: Any):
+        super().__init__(**data)
+        self.output['data_json']['result'] = model_prediction
+
+
+################ Task: Name Entity Recognition ################
+
+class NameEntityRecognitionInput(BaseModel):
+    """Input data for name entity recognition task"""
+    text: List[str] = Field(..., description="List of texts", example=["This is an example text for NER."])
+    entity: List[Any] = Field(..., description="List of entities", example=["PERSON", "ORG", "GPE"])
+
+    class Config:
+        extra = Extra.allow
+
+
+class NameEntityRecognitionOutput(BaseModel):
+    """Output data for name entity recognition task"""
+    status: bool = True
+    data_type: List[str] = Field(default=["data_json"], description="List of data types", enum=data_types)
+    output: Dict[str, Any] = Field(
+        default={"data_json": {"result": None}},
+        description="Output dictionary",
+        keys={"enum": data_types},
+        example={
+            'data_json': {
+                'result': [
+                    [{
+                        'entity': str,
+                        'confidence': float,
+                        'chunk': str,
+                        'begin': int,
+                        'end': int
+                    }]
+                ]
+            }
+        }
+    )
+
+    def __init__(self, model_prediction: Any, **data: Any):
+        super().__init__(**data)
+        self.output['data_json']['result'] = model_prediction
+
+
+######################### Task: Deidentification #########################
+
+class DeidentificationInput(BaseModel):
+    """Input data for deidentification task"""
+    text: List[str] = Field(..., description="List of texts", example=["This is an example text for deidentification."])
+    entity: List[str] = Field(..., description="List of entities", example=["PERSON", "ORG", "GPE"])
+
+    class Config:
+        extra = Extra.allow
+
+class DeidentificationOutput(BaseModel):
+    """Output data for deidentification task"""
+    status: bool = True
+    data_type: List[str] = Field(default=["data_json"], description="List of data types", enum=data_types)
+    output: Dict[str, Any] = Field(
+                                    default={"data_json": {"result": None}},
+                                    description="Output dictionary",
+                                    keys={"enum": data_types},
+                                    example={
+                                        'data_json': {'result': [
+                                            {'entities': [
+                                                {
+                                                    'entity': str,
+                                                    'confidence': float,
+                                                    'chunk': str,
+                                                    'begin': int,
+                                                    'end': int,
+                                                    'faked_chunk': str
+                                                }],
+                                                'masked_text': str,
+                                                'faked_text': str
+                                            }]
+                                        }}
+                                )
+
+    def __init__(self, model_prediction: Any, **data: Any):
+        super().__init__(**data)
+        self.output['data_json']['result'] = model_prediction
+
+
+####################### Task: Chatbot ###################### TODO: Still in development
+
+class ChatbotInput(BaseModel):
+    """Input data for chatbot task"""
+    messages: List[Dict[str, str]] = Field(..., description="List of messages",
+                                           example=[{"role": "user", "content": "Who are you?"},
+                                                    {"role": "assistant", "content": "I am Chat Bot. Who are you?"},
+                                                    {"role": "user", "content": "I am Joseph."}
+                                                    ])
+    stream: bool = False
+    max_tokens: int = 256
+    temperature: float = 0.7
+
+    class Config:
+        extra = Extra.allow
+
+class ChatbotOutput(BaseModel):
+    """Output data for chatbot task"""
+    status: bool = True
+    data_type: List[str] = Field(default=["data_json", "data_audio"],
+                                 description="List of data types",
+                                 enum=data_types)
+    # data_json: Dict[str, Any] = Field(default=None, description="Text API Output in dictionary", repr=False, exclude=True,)
+    # data_audio: str = Field(default=None, description="Audio API Output in base64 format", repr=False, exclude=True,
+    #                         example="data:audio/mp3;base64,//tQxA-audio-base64-format-string", )
+    raw_output: Dict[str, Any] = Field(default=None, description="Raw API Output in dictionary", repr=False,
+                                       exclude=True)
+    output: Dict[str, Any] = Field(
+        default={"data_json": {"text": None}, "data_audio": None, "raw_output": None},
+        description="Output dictionary",
+        keys={"enum": data_types},
+        example={
+            "data_json": {"text": "Well…   good luck…"},
+            "raw_output": {'choices': [{'message': {'content': 'Well… good luck…', 'role': 'assistant',
+                                                    'finish_reason': 'stop', 'index': 0, }}],
+                           'created': 1683618639,
+                           'id': 'chaxxpl-7EXXXXXwQNqPmXXXXXaYWkMtKNVjg',
+                           'model': 'gpt-3.5-turbo-0301',
+                           'object': 'chat.completion',
+                           'usage': {'completion_tokens': 27,
+                                     'prompt_tokens': 186,
+                                     'total_tokens': 213}},
+            "data_audio": "data:audio/mp3;base64,//tQxA-audio-base64-format-audio-file...==="},
+    )
+
+    def __init__(self, api_text: Any, api_result: Any, api_audio: Any, **data: Any):
+        super().__init__(**data)
+        self.output['data_json']['text'] = api_text
+        self.output['raw_output'] = api_result
+        self.output['data_audio'] = api_audio
+      
+
+######################## Task: OCR ######################## TODO: Still in development
+
+class OcrInput(BaseModel):
+    """Input data for OCR task"""
+    file_type: str = Field(..., description="File type image or pdf", example="image/png")
+    file: str = Field(..., description="File in base64 format", example="data:image/png;base64,//tQxA-image-base64-format-string")
+
+    class Config:
+        extra = Extra.allow
+
+class OcrOutput(BaseModel):
+    """Output data for OCR task"""
+    status: bool = True
+    data_type: List[str] = Field(default=["data_image"], description="List of data types", enum=data_types)
+    output: Dict[str, Any] = Field(
+                                    default={},
+                                    description="Output dictionary",
+                                    keys={"enum": data_types},
+                                    example={"data_image": ["data:image/png;base64,//tQxA-image-base64-format-string"]}
+                                )
+
+    def __init__(self, model_prediction: Any, data_type: List[str]=["data_image"], **data: Any):
+        super().__init__(**data)
+        self.data_type = data_type
+
+        if "data_image" in self.data_type:
+            self.output['data_image'] = model_prediction
+        elif "data_pdf" in self.data_type:
+            self.output['data_pdf'] = model_prediction
+        else:
+            raise ValueError("Invalid data_type, data_type must be data_image or data_pdf")
+        
+######################## Task: Translation ########################
+
+class TranslationInput(BaseModel):
+    """Input data for translation task"""
+    text: List[str] = Field(..., description="List of texts", example=["This is an example text for translation."])
+    source_language: str = Field(..., description="Source language", example="en")
+    output_language: str = Field(..., description="Output language", example="de")
+
+    class Config:
+        extra = Extra.allow
+
+
+class TranslationOutput(BaseModel):
+    """Output data for translation task"""
+    status: bool = True
+    data_type: List[str] = Field(default=["data_json"], description="List of data types one or more item of data_types", enum=data_types)
+    output: Dict[str, Any] = Field(
+                                    default={"data_json": {"result": {'output_language':None, 'translated_text':None}}},
+                                    description="Output dictionary",
+                                    keys={"enum": data_types},
+                                    example={
+                                            "data_json": {
+                                                            "result": {
+                                                                        "output_language": "<output_language>",
+                                                                        "translated_text": ["<translated_text>"]
+                                                                    }}}
+                                )
+
+    def __init__(self, model_prediction: Any, output_language: str, **data: Any):
+        super().__init__(**data)
+        self.output['data_json']['result']['output_language'] = output_language
+        self.output['data_json']['result']['translated_text'] = model_prediction
+
+######################## Task: Auto Speech Recognition ########################
+
+class ASRInput(BaseModel):
+    """Input data for ASR task"""
+    data_type: List[str] = Field(default=["data_audio"], description="List of data types one or more item of data_types", enum=data_types)
+    file: str = Field(default=None, description="File in base64 format", example="data:audio/mp3;base64,//tQxA-audio-base64-format-audio-file...===")
+    url: str = Field(default=None, description="Audio file url", example="https://www.example.com/audio.mp3")
+    translation: bool = Field(default=False, description="Translation flag", example=True)
+    language: str = Field(default=None, description="Language code", example="en")
+
+    class Config:
+        extra = Extra.allow
+
+class ASROutput(BaseModel):
+    status: bool = True
+    data_type: List[str] = Field(default=["data_json"], description="List of data types one or more item of data_types", enum=data_types)
+    output: Dict[str, Any] = Field(default={"data_json": {"transcription":None, 
+                                                          "translation":None, 
+                                                          "segments":None, 
+                                                          "language":None}}, description="Output dictionary", example={"data_json": {"transcription":"transcription_text", "translation": "translation_to_english_text_or_None", "segments": [{"text": "text_chunk_of_transcription.", "start": 0.0, "end": 3.0}], "language": "en"}})
+
+    def __init__(self, transcription:list=None, translation=None, language:str="en", segments: Any=None, **data: Any):
+        super().__init__(**data)
+        self.output['data_json']['transcription'] = transcription
+        self.output['data_json']['translation'] = translation
+        self.output['data_json']['language'] = language
+        self.output['data_json']['segments'] = segments
+
+        class Config:
+            extra = Extra.allow
+
```

### Comparing `aimped-0.1.53/aimped/model/load.py` & `aimped-0.1.54/aimped/model/load.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.53/aimped/models.py` & `aimped-0.1.54/aimped/models.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.53/aimped/nlp/assertion.py` & `aimped-0.1.54/aimped/nlp/assertion.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         ' [Entity] ',
         df['sentence'][df['sent_begin']:df['sent_end']],
         ' [Entity] ',
         df['sentence'][df['sent_end']:]])
     return df['new_sentence']
 
 
-def AssertionModelResults(ner_results, sentences, classifier, assertion_white_label_list):
+def AssertionModelResults(ner_results, sentences, classifier, assertion_white_label_list, resolver = False):
     """
     It returns the assertion detection results of a text.
     parameters:
     ----------------
     ner_results: list of dict
     sentences: list of str
     tokenizer: transformers.tokenization_utils_base.PreTrainedTokenizer
@@ -50,11 +50,15 @@
             for i in df.sent_idx.unique():
                 df.loc[df[df.sent_idx == i].index, 'sentence'] = sentences[i]
             df['new_sentence'] = np.nan
             df['new_sentence'] = df.apply(AssertionAnnotateSentence, axis=1)
             df.reset_index(drop=True, inplace=True)
             rel_results = classifier(list(df['new_sentence']))
             df = pd.concat([df, pd.DataFrame(rel_results)], axis=1)
-            df = df[['begin', 'end', 'ner_label', 'chunk', 'label', 'score']]
-            df.columns = ['begin', 'end', 'ner_label', 'chunk', 'assertion', 'score']
-            df = df[df['assertion'].isin(assertion_white_label_list)]
+            if not resolver:
+                df = df[['begin', 'end', 'ner_label', 'chunk', 'label','score']]
+                df.columns = ['begin','end', 'ner_label', 'chunk', 'assertion','score']
+            else:
+                df = df[['begin', 'end', 'ner_label', 'chunk', 'sent_idx','label']]
+                df.columns = ['begin','end', 'entity', 'chunk','sent_idx', 'assertion']
+            df =df[df['assertion'].isin(assertion_white_label_list)]
     return df.to_dict(orient='records')
```

### Comparing `aimped-0.1.53/aimped/nlp/chunker.py` & `aimped-0.1.54/aimped/nlp/chunker.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.53/aimped/nlp/deid.py` & `aimped-0.1.54/aimped/nlp/deid.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.53/aimped/nlp/ner.py` & `aimped-0.1.54/aimped/nlp/ner.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.53/aimped/nlp/ner_cls_report.py` & `aimped-0.1.54/aimped/nlp/ner_cls_report.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.53/aimped/nlp/regex_parser.py` & `aimped-0.1.54/aimped/nlp/regex_parser.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.53/aimped/nlp/relation_visualizer.py` & `aimped-0.1.54/aimped/nlp/relation_visualizer.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.53/aimped/nlp/tokenizer.py` & `aimped-0.1.54/aimped/nlp/tokenizer.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.53/aimped/nlp/tools.py` & `aimped-0.1.54/aimped/nlp/tools.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.53/aimped/test/test_assertion.py` & `aimped-0.1.54/aimped/test/test_assertion.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.53/aimped/test/test_chunk_merger.py` & `aimped-0.1.54/aimped/test/test_chunk_merger.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.53/aimped/test/test_deid_pipeline.py` & `aimped-0.1.54/aimped/test/test_deid_pipeline.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.53/aimped/test/test_ner_results.py` & `aimped-0.1.54/aimped/test/test_ner_results.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.53/aimped/test/test_regex_parser.py` & `aimped-0.1.54/aimped/test/test_regex_parser.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.53/aimped/test/test_relation_pipeline.py` & `aimped-0.1.54/aimped/test/test_relation_pipeline.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.53/aimped/test/test_tokenizer.py` & `aimped-0.1.54/aimped/test/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.53/aimped/test/test_translation_pipeline.py` & `aimped-0.1.54/aimped/test/test_translation_pipeline.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.53/aimped/utils.py` & `aimped-0.1.54/aimped/utils.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.53/aimped.egg-info/PKG-INFO` & `aimped-0.1.54/aimped.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,64 +1,68 @@
-Metadata-Version: 2.1
-Name: aimped
-Version: 0.1.53
-Summary: Aimped is a unique library that provides classes and functions for only exclusively business-tailored AI-based NLP models.
-Home-page: https://dev.aimped.ai/
-Author: Russell C.
-Author-email: russell@aimped.com
-Maintainer: aimped
-Maintainer-email: contact@aimped.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# **aimped**
-![aimped](https://dev.aimped.ai/static/media/AimpedBirdLogo.0b3c7cc26d31afe7bd73db496acb01d1.svg)
-
-**Aimped is a unique python library that provides classes and functions for only exclusively business-tailored AI-based NLP models.**  
-
-# Installation  
-```python
-pip install aimped
-```
-
-# Usage  
-```python  
-import aimped
-print(aimped.__version__)
-```
-## Examples  
-
-### Example 1
-
-```python  
-from aimped import nlp
-
-result = nlp.sentence_tokenizer("Hi, welcome to aimped. Explore ai models.",language="english")
-print(result)
-# ['Hi, welcome to aimped.', 'Explore ai models.']
-```
-
-### Example 2
-```python  
-from aimped.nlp.tokenizer import sentence_tokenizer
-
-result = sentence_tokenizer("Hi, welcome to aimped. Explore ai models.",language="english")
-print(result)
-# ['Hi, welcome to aimped.', 'Explore ai models.']
-```
-
-### Example 3
-```python  
-from aimped.nlp.pipeline import Pipeline
-
-pipe = Pipeline(model=model, tokenizer=tokenizer, device='cpu')
-result = pipe.ner_result(
-                        text=text,
-                        sents_tokens_list=sents_tokens_list,
-                        sentences=sentences)
-print(result)
-```
-
+Metadata-Version: 2.1
+Name: aimped
+Version: 0.1.54
+Summary: Aimped is a unique library that provides classes and functions for only exclusively business-tailored AI-based NLP models.
+Home-page: https://dev.aimped.ai/
+Author: Russell C.
+Author-email: russell@aimped.com
+Maintainer: aimped
+Maintainer-email: contact@aimped.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# **aimped**
+![aimped](https://dev.aimped.ai/static/media/AimpedBirdLogo.0b3c7cc26d31afe7bd73db496acb01d1.svg)
+
+**Aimped is a unique python library that provides classes and functions for only exclusively business-tailored AI-based NLP models.**  
+
+# Installation  
+```python
+pip install aimped
+```
+
+# Usage  
+```python  
+import aimped
+print(aimped.__version__)
+```
+## Examples  
+
+### Example 1
+
+```python  
+from aimped import nlp
+
+result = nlp.sentence_tokenizer("Hi, welcome to aimped. Explore ai models.",language="english")
+print(result)
+# ['Hi, welcome to aimped.', 'Explore ai models.']
+```
+
+### Example 2
+```python  
+from aimped.nlp.tokenizer import sentence_tokenizer
+
+result = sentence_tokenizer("Hi, welcome to aimped. Explore ai models.",language="english")
+print(result)
+# ['Hi, welcome to aimped.', 'Explore ai models.']
+```
+
+### Example 3
+```python  
+from aimped.nlp.pipeline import Pipeline
+
+pipe = Pipeline(model=model, tokenizer=tokenizer, device='cpu')
+result = pipe.ner_result(
+                        text=text,
+                        sents_tokens_list=sents_tokens_list,
+                        sentences=sentences)
+print(result)
+```
+
+
+
```

### Comparing `aimped-0.1.53/aimped.egg-info/SOURCES.txt` & `aimped-0.1.54/aimped.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aimped-0.1.53/setup.py` & `aimped-0.1.54/setup.py`

 * *Files identical despite different names*

