# Comparing `tmp/tokenmonster-1.1.2.tar.gz` & `tmp/tokenmonster-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tokenmonster-1.1.2.tar", last modified: Tue Jul 11 08:54:03 2023, max compression
+gzip compressed data, was "tokenmonster-1.1.3.tar", last modified: Wed Jul 12 14:07:31 2023, max compression
```

## Comparing `tokenmonster-1.1.2.tar` & `tokenmonster-1.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 08:54:03.702963 tokenmonster-1.1.2/
--rw-r--r--   0 root         (0) root         (0)    16187 2023-07-11 08:54:03.702963 tokenmonster-1.1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    16433 2023-07-11 08:52:51.000000 tokenmonster-1.1.2/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 08:54:03.702963 tokenmonster-1.1.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      550 2023-07-11 08:50:27.000000 tokenmonster-1.1.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 08:54:03.702963 tokenmonster-1.1.2/tokenmonster.egg-info/
--rw-r--r--   0 root         (0) root         (0)    16187 2023-07-11 08:54:03.000000 tokenmonster-1.1.2/tokenmonster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      178 2023-07-11 08:54:03.000000 tokenmonster-1.1.2/tokenmonster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 08:54:03.000000 tokenmonster-1.1.2/tokenmonster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-11 08:54:03.000000 tokenmonster-1.1.2/tokenmonster.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)    46267 2023-07-11 08:49:42.000000 tokenmonster-1.1.2/tokenmonster.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:07:31.357601 tokenmonster-1.1.3/
+-rw-r--r--   0 root         (0) root         (0)    16622 2023-07-12 14:07:31.357601 tokenmonster-1.1.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    16887 2023-07-12 14:01:39.000000 tokenmonster-1.1.3/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 14:07:31.357601 tokenmonster-1.1.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      550 2023-07-12 14:00:34.000000 tokenmonster-1.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:07:31.357601 tokenmonster-1.1.3/tokenmonster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    16622 2023-07-12 14:07:31.000000 tokenmonster-1.1.3/tokenmonster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      178 2023-07-12 14:07:31.000000 tokenmonster-1.1.3/tokenmonster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 14:07:31.000000 tokenmonster-1.1.3/tokenmonster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-12 14:07:31.000000 tokenmonster-1.1.3/tokenmonster.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)    49036 2023-07-12 14:03:25.000000 tokenmonster-1.1.3/tokenmonster.py
```

### Comparing `tokenmonster-1.1.2/PKG-INFO` & `tokenmonster-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tokenmonster
-Version: 1.1.2
+Version: 1.1.3
 Summary: Tokenize and decode text with TokenMonster vocabularies.
 Home-page: https://github.com/alasdairforsythe/tokenmonster
 Author: Alasdair Forsythe
 Author-email: 77910352+alasdairforsythe@users.noreply.github.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -15,14 +15,15 @@
 2. Loading & Exporting
     - [tokenmonster.load(path)](#tokenmonsterloadpath)
     - [tokenmonster.new(yaml)](#tokenmonsternewyaml)
     - [vocab.save(fname)](#vocabsavefname)
     - [vocab.export_yaml(order_by_score=False)](#vocabexport_yamlorder_by_scorefalse)
 3. Tokenization & Detokenization
     - [vocab.tokenize(text)](#vocabtokenizetext)
+    - [vocab.tokenize_count(text)](#vocabtokenize_counttext)
     - [vocab.decode(tokens)](#vocabdecodetokens)
     - [vocab.decoder()](#vocabdecoder)
     - [decoder.decode(tokens)](#decoderdecodetokens)
 4. Vocabulary Information
     - [len(vocab)](#lenvocab)
     - [vocab.get_dictionary()](#vocabget_dictionary)
     - [vocab.charset()](#vocabcharset)
@@ -145,32 +146,50 @@
 ## Tokenization & Detokenization
 
 ### vocab.tokenize(text)
 
 Tokenizes a string into tokens according to the vocabulary.
 
 You can pass a string or a list of strings. If you pass a list of strings they are tokenized
-in parallel using as many threads as you supplied strings. Note that if you pass a string
-it is converted to a binary string, so if you binary string in the first place, feel
+in parallel using as many threads as the list size. Note that if you pass a string
+it is converted to a binary string, so if you have binary string in the first place, feel
 free to pass that instead.
 
 #### Parameters
 
 - `text` (string or list of strings): A string or bytes string, or list of strings or bytes strings.
 
 #### Returns
 
-- `tokens` (int or list of int): The tokens to decode into a string.
+- `tokens` (list of ints or list of list of ints): The tokens IDs
 
 #### Usage
 
 ```python
 tokens = vocab.tokenize(text)
 ```
 
+### vocab.tokenize_count(text)
+
+Same as tokenize, but it returns only the number of tokens.
+
+#### Parameters
+
+- `text` (string or list of strings): A string or bytes string, or list of strings or bytes strings.
+
+#### Returns
+
+- `n_tokens` (int or list of ints): The number of tokens for each input string
+
+#### Usage
+
+```python
+number_of_tokens = vocab.tokenize_count(text)
+```
+
 ### vocab.decode(tokens)
 
 Decodes tokens into a string.
 
 Only use this "decode" method if you are decoding a complete "batch" or complete "conversation" in one go.
 For decoding an incomplete batch sequentially (as the tokens become available) instead
 use the decoder object.
@@ -541,15 +560,15 @@
 
 - `string`: A human-readable string derived from the input tokens.
 
 #### Usage
 
 ```python
 vocab = tokenmonster.load("english-32000-balanced-v1")
-decoder = vocab.Decoder()
+decoder = vocab.decoder()
 decoded_string = decoder.decode(tokens)
 decoded_string += decoder.decode(more_tokens)
 ```
 
 ## Other
 
 ### tokenmonster.set_local_directory(dir=None)
```

### Comparing `tokenmonster-1.1.2/README.md` & `tokenmonster-1.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 2. Loading & Exporting
     - [tokenmonster.load(path)](#tokenmonsterloadpath)
     - [tokenmonster.new(yaml)](#tokenmonsternewyaml)
     - [vocab.save(fname)](#vocabsavefname)
     - [vocab.export_yaml(order_by_score=False)](#vocabexport_yamlorder_by_scorefalse)
 3. Tokenization & Detokenization
     - [vocab.tokenize(text)](#vocabtokenizetext)
+    - [vocab.tokenize_count(text)](#vocabtokenize_counttext)
     - [vocab.decode(tokens)](#vocabdecodetokens)
     - [vocab.decoder()](#vocabdecoder)
     - [decoder.decode(tokens)](#decoderdecodetokens)
 4. Vocabulary Information
     - [len(vocab)](#lenvocab)
     - [vocab.get_dictionary()](#vocabget_dictionary)
     - [vocab.charset()](#vocabcharset)
@@ -134,32 +135,50 @@
 ## Tokenization & Detokenization
 
 ### vocab.tokenize(text)
 
 Tokenizes a string into tokens according to the vocabulary.
 
 You can pass a string or a list of strings. If you pass a list of strings they are tokenized
-in parallel using as many threads as you supplied strings. Note that if you pass a string
-it is converted to a binary string, so if you binary string in the first place, feel
+in parallel using as many threads as the list size. Note that if you pass a string
+it is converted to a binary string, so if you have binary string in the first place, feel
 free to pass that instead.
 
 #### Parameters
 
 - `text` (string or list of strings): A string or bytes string, or list of strings or bytes strings.
 
 #### Returns
 
-- `tokens` (int or list of int): The tokens to decode into a string.
+- `tokens` (list of ints or list of list of ints): The tokens IDs
 
 #### Usage
 
 ```python
 tokens = vocab.tokenize(text)
 ```
 
+### vocab.tokenize_count(text)
+
+Same as tokenize, but it returns only the number of tokens.
+
+#### Parameters
+
+- `text` (string or list of strings): A string or bytes string, or list of strings or bytes strings.
+
+#### Returns
+
+- `n_tokens` (int or list of ints): The number of tokens for each input string
+
+#### Usage
+
+```python
+number_of_tokens = vocab.tokenize_count(text)
+```
+
 ### vocab.decode(tokens)
 
 Decodes tokens into a string.
 
 Only use this "decode" method if you are decoding a complete "batch" or complete "conversation" in one go.
 For decoding an incomplete batch sequentially (as the tokens become available) instead
 use the decoder object.
@@ -530,15 +549,15 @@
 
 - `string`: A human-readable string derived from the input tokens.
 
 #### Usage
 
 ```python
 vocab = tokenmonster.load("english-32000-balanced-v1")
-decoder = vocab.Decoder()
+decoder = vocab.decoder()
 decoded_string = decoder.decode(tokens)
 decoded_string += decoder.decode(more_tokens)
 ```
 
 ## Other
 
 ### tokenmonster.set_local_directory(dir=None)
```

### Comparing `tokenmonster-1.1.2/setup.py` & `tokenmonster-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='tokenmonster',
-    version='1.1.2',
+    version='1.1.3',
     py_modules=['tokenmonster'],
     author='Alasdair Forsythe',
     author_email='77910352+alasdairforsythe@users.noreply.github.com',
     description='Tokenize and decode text with TokenMonster vocabularies.',
     url='https://github.com/alasdairforsythe/tokenmonster',
     license='MIT',
     long_description=long_description,
```

### Comparing `tokenmonster-1.1.2/tokenmonster.egg-info/PKG-INFO` & `tokenmonster-1.1.3/tokenmonster.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tokenmonster
-Version: 1.1.2
+Version: 1.1.3
 Summary: Tokenize and decode text with TokenMonster vocabularies.
 Home-page: https://github.com/alasdairforsythe/tokenmonster
 Author: Alasdair Forsythe
 Author-email: 77910352+alasdairforsythe@users.noreply.github.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -15,14 +15,15 @@
 2. Loading & Exporting
     - [tokenmonster.load(path)](#tokenmonsterloadpath)
     - [tokenmonster.new(yaml)](#tokenmonsternewyaml)
     - [vocab.save(fname)](#vocabsavefname)
     - [vocab.export_yaml(order_by_score=False)](#vocabexport_yamlorder_by_scorefalse)
 3. Tokenization & Detokenization
     - [vocab.tokenize(text)](#vocabtokenizetext)
+    - [vocab.tokenize_count(text)](#vocabtokenize_counttext)
     - [vocab.decode(tokens)](#vocabdecodetokens)
     - [vocab.decoder()](#vocabdecoder)
     - [decoder.decode(tokens)](#decoderdecodetokens)
 4. Vocabulary Information
     - [len(vocab)](#lenvocab)
     - [vocab.get_dictionary()](#vocabget_dictionary)
     - [vocab.charset()](#vocabcharset)
@@ -145,32 +146,50 @@
 ## Tokenization & Detokenization
 
 ### vocab.tokenize(text)
 
 Tokenizes a string into tokens according to the vocabulary.
 
 You can pass a string or a list of strings. If you pass a list of strings they are tokenized
-in parallel using as many threads as you supplied strings. Note that if you pass a string
-it is converted to a binary string, so if you binary string in the first place, feel
+in parallel using as many threads as the list size. Note that if you pass a string
+it is converted to a binary string, so if you have binary string in the first place, feel
 free to pass that instead.
 
 #### Parameters
 
 - `text` (string or list of strings): A string or bytes string, or list of strings or bytes strings.
 
 #### Returns
 
-- `tokens` (int or list of int): The tokens to decode into a string.
+- `tokens` (list of ints or list of list of ints): The tokens IDs
 
 #### Usage
 
 ```python
 tokens = vocab.tokenize(text)
 ```
 
+### vocab.tokenize_count(text)
+
+Same as tokenize, but it returns only the number of tokens.
+
+#### Parameters
+
+- `text` (string or list of strings): A string or bytes string, or list of strings or bytes strings.
+
+#### Returns
+
+- `n_tokens` (int or list of ints): The number of tokens for each input string
+
+#### Usage
+
+```python
+number_of_tokens = vocab.tokenize_count(text)
+```
+
 ### vocab.decode(tokens)
 
 Decodes tokens into a string.
 
 Only use this "decode" method if you are decoding a complete "batch" or complete "conversation" in one go.
 For decoding an incomplete batch sequentially (as the tokens become available) instead
 use the decoder object.
@@ -541,15 +560,15 @@
 
 - `string`: A human-readable string derived from the input tokens.
 
 #### Usage
 
 ```python
 vocab = tokenmonster.load("english-32000-balanced-v1")
-decoder = vocab.Decoder()
+decoder = vocab.decoder()
 decoded_string = decoder.decode(tokens)
 decoded_string += decoder.decode(more_tokens)
 ```
 
 ## Other
 
 ### tokenmonster.set_local_directory(dir=None)
```

### Comparing `tokenmonster-1.1.2/tokenmonster.py` & `tokenmonster-1.1.3/tokenmonster.py`

 * *Files 2% similar despite different names*

```diff
@@ -376,23 +376,23 @@
             return decoded
     
     def tokenize(self, text):
         """
         Tokenizes a string into tokens according to the vocabulary.
 
         You can pass a string or a list of strings. If you pass a list of strings they are tokenized
-        in parallel using as many threads as you supplied strings. Note that if you pass a string
-        it is converted to a binary string, so if you binary string in the first place, feel
+        in parallel using as many threads as the list size. Note that if you pass a string
+        it is converted to a binary string, so if you have binary string in the first place, feel
         free to pass that instead.
 
         Parameters:
             string or list of strings: A string or bytes string, or list of strings or bytes strings.
 
         Returns:
-            tokens (int or list of int): The tokens to decode into a string
+            tokens (list of ints or list of list of ints): The tokens IDs
 
         Usage:
             tokens = vocab.tokenize(text)
         """
         if self._modified_id == -1:
             raise RuntimeError("TokenMonster: Access denied to expired Vocab instance.")
         length = 4
@@ -433,25 +433,92 @@
         # Send
         job_type = 1
         payload[0] = _write_uint32(batch_size)
         response = Vocab._communicate(job_type, self.id, length, payload)
         batches_reply = _read_uint32(response[0:4])
         if batches_reply != batch_size:
             raise RuntimeError("TokenMonster: batch size of response differs from request")
-        tokens = [None] * batches_reply
         offset = 4
+        if single:
+            batch_length = _read_uint64(response[offset:offset+8])
+            offset += 8
+            return self.deserialize_tokens(response[offset:offset+batch_length])
+        tokens = [None] * batches_reply
         for i in range(batch_size):
             batch_length = _read_uint64(response[offset:offset+8])
             offset += 8
             tokens[i] = self.deserialize_tokens(response[offset:offset+batch_length])
             offset += batch_length
-        if single:
-            return tokens[0]
+        return tokens
+        
+    def tokenize_count(self, text):
+        """
+        Same as tokenize, but it returns only the number of tokens.
+
+        Parameters:
+            string or list of strings: A string or bytes string, or list of strings or bytes strings.
+
+        Returns:
+            n_tokens (int or list of ints): The number of tokens for each input string
+
+        Usage:
+            tokens = vocab.tokenize_count(text)
+        """
+        if self._modified_id == -1:
+            raise RuntimeError("TokenMonster: Access denied to expired Vocab instance.")
+        length = 4
+        batch_size = 1
+        payload = [b'']
+        single = False
+        if isinstance(text, str):
+            if len(text) == 0:
+                return
+            data = self._string_to_bytes(text)
+            length += len(data) + 8
+            payload.append(_write_uint64(len(data)))
+            payload.append(data)
+            single = True
+        elif isinstance(text, bytes):
+            if len(text) == 0:
+                return
+            length += len(text) + 8
+            payload.append(_write_uint64(len(text)))
+            payload.append(text)
+            single = True
+        elif is_iterable(text):
+            batch_size = len(text)
+            for i, item in enumerate(text):
+                if isinstance(item, str):
+                    data = self._string_to_bytes(item)
+                    payload.append(_write_uint64(len(data)))
+                    payload.append(data)
+                    length += len(data) + 8
+                elif isinstance(item, bytes):
+                    payload.append(_write_uint64(len(item)))
+                    payload.append(item)
+                    length += len(item) + 8
+                else:
+                    raise ValueError("TokenMonster: Input to tokenize must be a string or a list of strings.")
         else:
-            return tokens
+            raise ValueError("TokenMonster: Input to tokenize must be a string or a list of strings.")
+        # Send
+        job_type = 20
+        payload[0] = _write_uint32(batch_size)
+        response = Vocab._communicate(job_type, self.id, length, payload)
+        batches_reply = _read_uint32(response[0:4])
+        if batches_reply != batch_size:
+            raise RuntimeError("TokenMonster: batch size of response differs from request")
+        offset = 4
+        if single:
+            return _read_uint64(response[offset:offset+8])
+        tokens = [0] * batch_size
+        for i in range(batch_size):
+            tokens[i] = _read_uint64(response[offset:offset+8])
+            offset += 8
+        return tokens
 
     def get_dictionary(self):
         """
         Returns a dictionary of all tokens in the vocabulary.
 
         This returns a list of dictionaries with keys "id", "token", "token_decoded", "type" and "score".
         Note that you should not attempt to use this to interpret tokenized sequences because the capcode
@@ -1200,8 +1267,8 @@
 
 def is_iterable(obj):
     if isinstance(obj, (str, bytes)):
         return False
     return isinstance(obj, Iterable)
 
 _TOKENMONSTER_URL = "https://huggingface.co/alasdairforsythe/tokenmonster/resolve/main/"
-_TMS_VERSION_ID = 1
+_TMS_VERSION_ID = 2
```

