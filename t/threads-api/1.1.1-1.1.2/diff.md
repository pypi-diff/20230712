# Comparing `tmp/threads-api-1.1.1.tar.gz` & `tmp/threads-api-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threads-api-1.1.1.tar", last modified: Tue Jul 11 21:03:15 2023, max compression
+gzip compressed data, was "threads-api-1.1.2.tar", last modified: Tue Jul 11 22:07:24 2023, max compression
```

## Comparing `threads-api-1.1.1.tar` & `threads-api-1.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-11 21:03:15.113644 threads-api-1.1.1/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)     1068 2023-07-06 22:22:29.000000 threads-api-1.1.1/LICENSE
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    12748 2023-07-11 21:03:15.113644 threads-api-1.1.1/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    12218 2023-07-11 21:00:43.000000 threads-api-1.1.1/README.md
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      409 2023-07-11 21:00:43.000000 threads-api-1.1.1/pyproject.toml
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-07-11 21:03:15.113644 threads-api-1.1.1/setup.cfg
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      768 2023-07-11 21:00:43.000000 threads-api-1.1.1/setup.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-11 21:03:15.109644 threads-api-1.1.1/threads_api/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 20:59:49.000000 threads-api-1.1.1/threads_api/__init__.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-11 21:03:15.113644 threads-api-1.1.1/threads_api/src/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 21:13:21.000000 threads-api-1.1.1/threads_api/src/__init__.py
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    28252 2023-07-11 21:00:43.000000 threads-api-1.1.1/threads_api/src/threads_api.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-11 21:03:15.113644 threads-api-1.1.1/threads_api/tests/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 21:19:18.000000 threads-api-1.1.1/threads_api/tests/__init__.py
--rwxrwxr-x   0 daniel    (1000) daniel    (1000)      406 2023-07-11 20:05:14.000000 threads-api-1.1.1/threads_api/tests/get_threads_test.py
-drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-11 21:03:15.113644 threads-api-1.1.1/threads_api.egg-info/
--rw-rw-r--   0 daniel    (1000) daniel    (1000)    12748 2023-07-11 21:03:15.000000 threads-api-1.1.1/threads_api.egg-info/PKG-INFO
--rw-rw-r--   0 daniel    (1000) daniel    (1000)      366 2023-07-11 21:03:15.000000 threads-api-1.1.1/threads_api.egg-info/SOURCES.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-07-11 21:03:15.000000 threads-api-1.1.1/threads_api.egg-info/dependency_links.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)        8 2023-07-11 21:03:15.000000 threads-api-1.1.1/threads_api.egg-info/requires.txt
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       12 2023-07-11 21:03:15.000000 threads-api-1.1.1/threads_api.egg-info/top_level.txt
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-11 22:07:24.711254 threads-api-1.1.2/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)     1068 2023-07-06 22:22:29.000000 threads-api-1.1.2/LICENSE
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    13302 2023-07-11 22:07:24.711254 threads-api-1.1.2/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    12772 2023-07-11 22:04:27.000000 threads-api-1.1.2/README.md
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      409 2023-07-11 21:59:17.000000 threads-api-1.1.2/pyproject.toml
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-07-11 22:07:24.711254 threads-api-1.1.2/setup.cfg
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      768 2023-07-11 21:59:23.000000 threads-api-1.1.2/setup.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-11 22:07:24.711254 threads-api-1.1.2/threads_api/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 20:59:49.000000 threads-api-1.1.2/threads_api/__init__.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-11 22:07:24.711254 threads-api-1.1.2/threads_api/src/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 21:13:21.000000 threads-api-1.1.2/threads_api/src/__init__.py
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    31239 2023-07-11 21:48:26.000000 threads-api-1.1.2/threads_api/src/threads_api.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-11 22:07:24.711254 threads-api-1.1.2/threads_api/tests/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        0 2023-07-06 21:19:18.000000 threads-api-1.1.2/threads_api/tests/__init__.py
+-rwxrwxr-x   0 daniel    (1000) daniel    (1000)      406 2023-07-11 20:05:14.000000 threads-api-1.1.2/threads_api/tests/get_threads_test.py
+drwxrwxr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-11 22:07:24.711254 threads-api-1.1.2/threads_api.egg-info/
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)    13302 2023-07-11 22:07:24.000000 threads-api-1.1.2/threads_api.egg-info/PKG-INFO
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)      366 2023-07-11 22:07:24.000000 threads-api-1.1.2/threads_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        1 2023-07-11 22:07:24.000000 threads-api-1.1.2/threads_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)        8 2023-07-11 22:07:24.000000 threads-api-1.1.2/threads_api.egg-info/requires.txt
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       12 2023-07-11 22:07:24.000000 threads-api-1.1.2/threads_api.egg-info/top_level.txt
```

### Comparing `threads-api-1.1.1/LICENSE` & `threads-api-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `threads-api-1.1.1/PKG-INFO` & `threads-api-1.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threads-api
-Version: 1.1.1
+Version: 1.1.2
 Summary: Unofficial Python client for Meta Threads.net API
 Home-page: https://github.com/danie1/threads-api
 Author: Danie1
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -79,14 +79,25 @@
 
 # Create an event loop and run the main function
 loop = asyncio.get_event_loop()
 loop.run_until_complete(main())
 ```
 
 ## Usage Examples
+View [example.py](https://github.com/Danie1/threads-api/blob/main/example.py) for code examples. 
+At the end of the file you will be able to uncomment and run the individual examples with ease.
+
+Then simply run as:
+```
+# Pass the credentials as environment variables
+USERNAME=<Instagram Username> PASSWORD=<Instagram Password> python3 example.py
+```
+
+### Samples
+
 <details>
   <summary>"get_user_id_from_username" Function</summary>
 
 ``` python
 from threads_api.src.threads_api import ThreadsAPI
 import asyncio
 
@@ -340,33 +351,37 @@
 Post has been successfully posted
 ```
 </details>
 
 ## 📌 Roadmap
 
 - [x] ✅ Login functionality 🔒
-  - [x] ✅ Cache login token securely (reduce login requests)
+  - [x] ✅ Cache login token securely (reduce login requests / due to restrictive limits)
 - [x] ✅ Write Posts (Requires Login 🔒)
   - [x] ✅ Posts with just text
   - [x] ✅ Posts with text and an image
   - [x] ✅ Posts with text that share a url
+  - [x] ✅ Reply to Posts
   - [ ] 🚧 Post with text and share a video
-  - [ ] 🚧 Reply to Posts
 - [x] ✅ Perform Actions (Requires Login 🔒)
   - [x] ✅ Like Posts
   - [x] ✅ Unlike Posts
+  - [x] ✅ Delete post
   - [x] ✅ Follow User
   - [x] ✅ Unfollow User
-- [x] ✅ Read Data
+- [x] ✅ Read Public Data
   - [x] ✅ Read a user_id (eg. `314216`) via username(eg. `zuck`)
   - [x] ✅ Read a user's profile info
   - [x] ✅ Read list of a user's Threads
   - [x] ✅ Read list of a user's Replies
   - [x] ✅ Read Post and a list of its Replies
   - [x] ✅ View who liked a post
+- [x] ✅ Read Private Data (Requires Login 🔒)
+  - [x] ✅ Read a user's followers list
+  - [x] ✅ Read a user's following list
 - [x] ✅  CI/CD
   - [x] ✅  GitHub Actions Pipeline
   - [ ] 🚧  Pytest
 
 
 # License
 This project is licensed under the MIT license.
```

### Comparing `threads-api-1.1.1/README.md` & `threads-api-1.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -62,14 +62,25 @@
 
 # Create an event loop and run the main function
 loop = asyncio.get_event_loop()
 loop.run_until_complete(main())
 ```
 
 ## Usage Examples
+View [example.py](https://github.com/Danie1/threads-api/blob/main/example.py) for code examples. 
+At the end of the file you will be able to uncomment and run the individual examples with ease.
+
+Then simply run as:
+```
+# Pass the credentials as environment variables
+USERNAME=<Instagram Username> PASSWORD=<Instagram Password> python3 example.py
+```
+
+### Samples
+
 <details>
   <summary>"get_user_id_from_username" Function</summary>
 
 ``` python
 from threads_api.src.threads_api import ThreadsAPI
 import asyncio
 
@@ -323,33 +334,37 @@
 Post has been successfully posted
 ```
 </details>
 
 ## 📌 Roadmap
 
 - [x] ✅ Login functionality 🔒
-  - [x] ✅ Cache login token securely (reduce login requests)
+  - [x] ✅ Cache login token securely (reduce login requests / due to restrictive limits)
 - [x] ✅ Write Posts (Requires Login 🔒)
   - [x] ✅ Posts with just text
   - [x] ✅ Posts with text and an image
   - [x] ✅ Posts with text that share a url
+  - [x] ✅ Reply to Posts
   - [ ] 🚧 Post with text and share a video
-  - [ ] 🚧 Reply to Posts
 - [x] ✅ Perform Actions (Requires Login 🔒)
   - [x] ✅ Like Posts
   - [x] ✅ Unlike Posts
+  - [x] ✅ Delete post
   - [x] ✅ Follow User
   - [x] ✅ Unfollow User
-- [x] ✅ Read Data
+- [x] ✅ Read Public Data
   - [x] ✅ Read a user_id (eg. `314216`) via username(eg. `zuck`)
   - [x] ✅ Read a user's profile info
   - [x] ✅ Read list of a user's Threads
   - [x] ✅ Read list of a user's Replies
   - [x] ✅ Read Post and a list of its Replies
   - [x] ✅ View who liked a post
+- [x] ✅ Read Private Data (Requires Login 🔒)
+  - [x] ✅ Read a user's followers list
+  - [x] ✅ Read a user's following list
 - [x] ✅  CI/CD
   - [x] ✅  GitHub Actions Pipeline
   - [ ] 🚧  Pytest
 
 
 # License
 This project is licensed under the MIT license.
```

### Comparing `threads-api-1.1.1/setup.py` & `threads-api-1.1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='threads-api',
-    version='1.1.1',
+    version='1.1.2',
     description='Unofficial Python client for Meta Threads.net API',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Danie1',
     author_email='',
     url='https://github.com/danie1/threads-api',
     packages=find_packages(),
```

### Comparing `threads-api-1.1.1/threads_api/src/threads_api.py` & `threads-api-1.1.2/threads_api/src/threads_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -225,14 +225,18 @@
             raise
 
     async def __auth_required_post_request(self, url: str):
         async with aiohttp.ClientSession() as session:
             async with session.post(url, headers=self.auth_headers) as response:
                 return await response.json()
     
+    async def __auth_required_get_request(self, url: str):
+        async with aiohttp.ClientSession() as session:
+            async with session.get(url, headers=self.auth_headers) as response:
+                return await response.json()
     
 
     async def get_user_id_from_username(self, username: str) -> str:
         """
         Retrieves the user ID associated with a given username.
         
         Args:
@@ -397,30 +401,44 @@
                     text = await response.text()
                     data = json.loads(text)
                 except (aiohttp.ContentTypeError, json.JSONDecodeError):
                     raise Exception('Failed to decode response as JSON')
 
         threads = data['data']['mediaData']['threads']
         return threads
-    
+
+    async def get_user_followers(self, user_id: str) -> bool:
+        if not self.is_logged_in:
+            raise Exception("The action 'get_user_followers' can only be perfomed while logged-in")
+        
+        res = await self.__auth_required_get_request(f"{BASE_URL}/friendships/{user_id}/followers")
+        return res
+
+    async def get_user_following(self, user_id: str) -> bool:
+        if not self.is_logged_in:
+            raise Exception("The action 'get_user_following' can only be perfomed while logged-in")
+        
+        res = await self.__auth_required_get_request(f"{BASE_URL}/friendships/{user_id}/following")
+        return res
+
     async def follow_user(self, user_id: str) -> bool:
         """
         Follows a user with the given user ID.
 
         Args:
             user_id (str): The ID of the user to follow.
 
         Returns:
             bool: True if the user was followed successfully, False otherwise.
 
         Raises:
             Exception: If an error occurs during the follow process.
         """
         if not self.is_logged_in:
-            raise Exception("The action 'follow' can only be perfomed while logged-in")
+            raise Exception("The action 'follow_user' can only be perfomed while logged-in")
         
         res = await self.__auth_required_post_request(f"{BASE_URL}/friendships/create/{user_id}/")
         return res["status"] == "ok"
 
     async def unfollow_user(self, user_id: str) -> bool:
         """
         Unfollows a user with the given user ID.
@@ -431,20 +449,76 @@
         Returns:
             bool: True if the user was unfollowed successfully, False otherwise.
 
         Raises:
             Exception: If an error occurs during the unfollow process.
         """
         if not self.is_logged_in:
-            raise Exception("The action 'unfollow' can only be perfomed while logged-in")
+            raise Exception("The action 'unfollow_user' can only be perfomed while logged-in")
         
         res = await self.__auth_required_post_request(f"{BASE_URL}/friendships/destroy/{user_id}/")
         return res["status"] == "ok"
 
+    async def like_post(self, post_id: str) -> bool:
+        """
+        Likes a post with the given ID.
+
+        Args:
+            user_id (str): The ID of the post to like.
+
+        Returns:
+            bool: True if the post was liked successfully, False otherwise.
+
+        Raises:
+            Exception: If an error occurs during the like process.
+        """
+        if not self.is_logged_in:
+            raise Exception("The action 'like_post' can only be perfomed while logged-in")
+        
+        res = await self.__auth_required_post_request(f"{BASE_URL}/media/{post_id}_{self.user_id}/like/")
+        return res["status"] == "ok"
+    
+    async def unlike_post(self, post_id: str) -> bool:
+        """
+        Unlikes a post with the given ID.
+
+        Args:
+            user_id (str): The ID of the post to unlike.
+
+        Returns:
+            bool: True if the post was unliked successfully, False otherwise.
+
+        Raises:
+            Exception: If an error occurs during the like process.
+        """
+        if not self.is_logged_in:
+            raise Exception("The action 'unlike_post' can only be perfomed while logged-in")
+        
+        res = await self.__auth_required_post_request(f"{BASE_URL}/media/{post_id}_{self.user_id}/unlike/")
+        return res["status"] == "ok"
+    
+    async def delete_post(self, post_id: str) -> bool:
+        """
+        Deletes a post with the given ID.
+
+        Args:
+            user_id (str): The ID of the post to delete.
+
+        Returns:
+            bool: True if the post was deleted successfully, False otherwise.
 
+        Raises:
+            Exception: If an error occurs during the deletion process.
+        """
+        if not self.is_logged_in:
+            raise Exception("The action 'delete_post' can only be perfomed while logged-in")
+        
+        res = await self.__auth_required_post_request(f"{BASE_URL}/media/{post_id}_{self.user_id}/delete/?media_type=TEXT_POST")
+        return res["status"] == "ok"
+    
     async def get_post_id_from_url(self, post_url):
         """
         Retrieves the post ID from a given URL.
 
         Args:
             post_url (str): The URL of the post.
         Returns:
@@ -710,15 +784,17 @@
         params = json.dumps(params)
         payload = f"signed_body=SIGNATURE.{urllib.parse.quote(params)}"
         headers = __get_app_headers().copy()
 
         try:
             async with aiohttp.ClientSession() as session:
                 async with session.post(post_url, headers=headers, data=payload) as response:
-                    if response.status == 200:
-                        return True
+                    data = await response.json()
+
+                    if 'media' in data and 'pk' in data['media']:
+                        # Return the newly created post_id
+                        return data['media']['pk']
                     else:
-                        print(response)
                         raise Exception("Failed to post. Got response:\n" + str(response))
         except Exception as e:
             print("[ERROR] ", e)
             raise
```

### Comparing `threads-api-1.1.1/threads_api.egg-info/PKG-INFO` & `threads-api-1.1.2/threads_api.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threads-api
-Version: 1.1.1
+Version: 1.1.2
 Summary: Unofficial Python client for Meta Threads.net API
 Home-page: https://github.com/danie1/threads-api
 Author: Danie1
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -79,14 +79,25 @@
 
 # Create an event loop and run the main function
 loop = asyncio.get_event_loop()
 loop.run_until_complete(main())
 ```
 
 ## Usage Examples
+View [example.py](https://github.com/Danie1/threads-api/blob/main/example.py) for code examples. 
+At the end of the file you will be able to uncomment and run the individual examples with ease.
+
+Then simply run as:
+```
+# Pass the credentials as environment variables
+USERNAME=<Instagram Username> PASSWORD=<Instagram Password> python3 example.py
+```
+
+### Samples
+
 <details>
   <summary>"get_user_id_from_username" Function</summary>
 
 ``` python
 from threads_api.src.threads_api import ThreadsAPI
 import asyncio
 
@@ -340,33 +351,37 @@
 Post has been successfully posted
 ```
 </details>
 
 ## 📌 Roadmap
 
 - [x] ✅ Login functionality 🔒
-  - [x] ✅ Cache login token securely (reduce login requests)
+  - [x] ✅ Cache login token securely (reduce login requests / due to restrictive limits)
 - [x] ✅ Write Posts (Requires Login 🔒)
   - [x] ✅ Posts with just text
   - [x] ✅ Posts with text and an image
   - [x] ✅ Posts with text that share a url
+  - [x] ✅ Reply to Posts
   - [ ] 🚧 Post with text and share a video
-  - [ ] 🚧 Reply to Posts
 - [x] ✅ Perform Actions (Requires Login 🔒)
   - [x] ✅ Like Posts
   - [x] ✅ Unlike Posts
+  - [x] ✅ Delete post
   - [x] ✅ Follow User
   - [x] ✅ Unfollow User
-- [x] ✅ Read Data
+- [x] ✅ Read Public Data
   - [x] ✅ Read a user_id (eg. `314216`) via username(eg. `zuck`)
   - [x] ✅ Read a user's profile info
   - [x] ✅ Read list of a user's Threads
   - [x] ✅ Read list of a user's Replies
   - [x] ✅ Read Post and a list of its Replies
   - [x] ✅ View who liked a post
+- [x] ✅ Read Private Data (Requires Login 🔒)
+  - [x] ✅ Read a user's followers list
+  - [x] ✅ Read a user's following list
 - [x] ✅  CI/CD
   - [x] ✅  GitHub Actions Pipeline
   - [ ] 🚧  Pytest
 
 
 # License
 This project is licensed under the MIT license.
```

