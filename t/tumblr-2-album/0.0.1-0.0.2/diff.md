# Comparing `tmp/tumblr_2_album-0.0.1.tar.gz` & `tmp/tumblr_2_album-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tumblr_2_album-0.0.1.tar", last modified: Wed Jul 12 20:53:32 2023, max compression
+gzip compressed data, was "tumblr_2_album-0.0.2.tar", last modified: Wed Jul 12 20:58:31 2023, max compression
```

## Comparing `tumblr_2_album-0.0.1.tar` & `tumblr_2_album-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-12 20:53:32.000000 tumblr_2_album-0.0.1/
--rw-r--r--   0 user       (501) staff       (20)    35149 2023-07-12 19:49:57.000000 tumblr_2_album-0.0.1/LICENSE
--rw-r--r--   0 user       (501) staff       (20)      599 2023-07-12 20:53:32.000000 tumblr_2_album-0.0.1/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)       94 2023-07-12 20:45:08.000000 tumblr_2_album-0.0.1/README.md
--rw-r--r--   0 user       (501) staff       (20)       38 2023-07-12 20:53:32.000000 tumblr_2_album-0.0.1/setup.cfg
--rw-r--r--   0 user       (501) staff       (20)      813 2023-07-12 20:43:31.000000 tumblr_2_album-0.0.1/setup.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-12 20:53:32.000000 tumblr_2_album-0.0.1/tumblr_2_album/
--rw-r--r--   0 user       (501) staff       (20)     2452 2023-07-12 20:53:11.000000 tumblr_2_album-0.0.1/tumblr_2_album/__init__.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-12 20:53:32.000000 tumblr_2_album-0.0.1/tumblr_2_album.egg-info/
--rw-r--r--   0 user       (501) staff       (20)      599 2023-07-12 20:53:32.000000 tumblr_2_album-0.0.1/tumblr_2_album.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      242 2023-07-12 20:53:32.000000 tumblr_2_album-0.0.1/tumblr_2_album.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2023-07-12 20:53:32.000000 tumblr_2_album-0.0.1/tumblr_2_album.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)       45 2023-07-12 20:53:32.000000 tumblr_2_album-0.0.1/tumblr_2_album.egg-info/requires.txt
--rw-r--r--   0 user       (501) staff       (20)       15 2023-07-12 20:53:32.000000 tumblr_2_album-0.0.1/tumblr_2_album.egg-info/top_level.txt
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-12 20:58:31.000000 tumblr_2_album-0.0.2/
+-rw-r--r--   0 user       (501) staff       (20)    35149 2023-07-12 19:49:57.000000 tumblr_2_album-0.0.2/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)      599 2023-07-12 20:58:31.000000 tumblr_2_album-0.0.2/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)       94 2023-07-12 20:45:08.000000 tumblr_2_album-0.0.2/README.md
+-rw-r--r--   0 user       (501) staff       (20)       38 2023-07-12 20:58:31.000000 tumblr_2_album-0.0.2/setup.cfg
+-rw-r--r--   0 user       (501) staff       (20)      813 2023-07-12 20:57:38.000000 tumblr_2_album-0.0.2/setup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-12 20:58:31.000000 tumblr_2_album-0.0.2/tumblr_2_album/
+-rw-r--r--   0 user       (501) staff       (20)     2484 2023-07-12 20:58:19.000000 tumblr_2_album-0.0.2/tumblr_2_album/__init__.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-07-12 20:58:31.000000 tumblr_2_album-0.0.2/tumblr_2_album.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)      599 2023-07-12 20:58:31.000000 tumblr_2_album-0.0.2/tumblr_2_album.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      242 2023-07-12 20:58:31.000000 tumblr_2_album-0.0.2/tumblr_2_album.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2023-07-12 20:58:31.000000 tumblr_2_album-0.0.2/tumblr_2_album.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)       45 2023-07-12 20:58:31.000000 tumblr_2_album-0.0.2/tumblr_2_album.egg-info/requires.txt
+-rw-r--r--   0 user       (501) staff       (20)       15 2023-07-12 20:58:31.000000 tumblr_2_album-0.0.2/tumblr_2_album.egg-info/top_level.txt
```

### Comparing `tumblr_2_album-0.0.1/LICENSE` & `tumblr_2_album-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tumblr_2_album-0.0.1/PKG-INFO` & `tumblr_2_album-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tumblr_2_album
-Version: 0.0.1
+Version: 0.0.2
 Summary: Return photo list and caption (markdown format) from tumblr.
 Home-page: https://github.com/gaoyunzhi/tumblr_2_album
 Author: Yunzhi Gao
 Author-email: gaoyunzhi@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tumblr_2_album-0.0.1/setup.py` & `tumblr_2_album-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tumblr_2_album",
-    version="0.0.1",
+    version="0.0.2",
     author="Yunzhi Gao",
     author_email="gaoyunzhi@gmail.com",
     description="Return photo list and caption (markdown format) from tumblr.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gaoyunzhi/tumblr_2_album",
     packages=setuptools.find_packages(),
```

### Comparing `tumblr_2_album-0.0.1/tumblr_2_album/__init__.py` & `tumblr_2_album-0.0.2/tumblr_2_album/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,42 +17,42 @@
         old_stdout = sys.stdout
         sys.stdout = devnull
         try:  
             yield
         finally:
             sys.stdout = old_stdout
 
-def getImgs(content):
-    soup = BeautifulSoup(content, 'html.parser')
+def getImgs(post):
+    soup = BeautifulSoup(post, 'html.parser')
     has_video = False
     for item in soup.find_all('source'):
         if item.get('type') != 'video/mp4':
             continue
         if not item.get('src'):
             continue
         has_video = True
         yield item['src']
     if not has_video:
         for item in soup.find_all('img'):
             yield item['src']
 
-def getImgsJson(content):
-    for photo in content:
+def getImgsJson(post):
+    for photo in post:
         yield photo['original_size']['url']
 
 def preDownload(img):
     filename = cached_url.getFilePath(img)
     if os.path.exists(filename):
         return
     # seems this is not silent
     with suppress_stdout():
         downloader.download(img, filename, silent=True)
 
-def getText(content):
-    soup = BeautifulSoup(content, 'html.parser')
+def getText(post):
+    soup = BeautifulSoup(post, 'html.parser')
     for item in soup.find_all('a', class_='tumblr_blog'):
         item.decompose()
     for tag in ['figure', 'img']:
         for item in soup.find_all(tag):
             item.decompose()
     lines = []
     for item in soup.find_all():
@@ -66,18 +66,22 @@
 def getBlogNameAndPostId(url):
     blog_name = url.split('/')[2].split('.')[0]
     if blog_name == 'www':
         blog_name = url.split('/')[3]
     post_id = int(url.strip('/').split('/')[-1])
     return blog_name, post_id
 
-def get(client, url):
+def getFromPost(post):
     result = Result()
-    result.url = url
-    blog_name, post_id = getBlogNameAndPostId(url)
-    content = client.posts(blog_name, id=post_id)['posts'][0]
-    result.video = content.get('video_url')
-    result.cap_html_v2 = getText(content.get('caption', '')) or getText(content.get('body', '')) or content['summary']
-    result.imgs = list(getImgsJson(content.get('photos', []))) or list(getImgs(content.get('body', '')))
+    result.url = post['post_url']
+    result.video = post.get('video_url')
+    result.cap_html_v2 = getText(post.get('caption', '')) or getText(post.get('body', '')) or post['summary']
+    result.imgs = list(getImgsJson(post.get('photos', []))) or list(getImgs(post.get('body', '')))
     for img in result.imgs:
         preDownload(img)
-    return result
+    return result
+
+def get(client, url):
+    blog_name, post_id = getBlogNameAndPostId(url)
+    post = client.posts(blog_name, id=post_id)['posts'][0]
+    return getFromPost(post)
+
```

### Comparing `tumblr_2_album-0.0.1/tumblr_2_album.egg-info/PKG-INFO` & `tumblr_2_album-0.0.2/tumblr_2_album.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tumblr-2-album
-Version: 0.0.1
+Version: 0.0.2
 Summary: Return photo list and caption (markdown format) from tumblr.
 Home-page: https://github.com/gaoyunzhi/tumblr_2_album
 Author: Yunzhi Gao
 Author-email: gaoyunzhi@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

