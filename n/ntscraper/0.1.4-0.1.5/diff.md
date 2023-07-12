# Comparing `tmp/ntscraper-0.1.4.tar.gz` & `tmp/ntscraper-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ntscraper-0.1.4.tar", last modified: Tue May  9 07:58:58 2023, max compression
+gzip compressed data, was "ntscraper-0.1.5.tar", last modified: Wed Jul 12 09:58:27 2023, max compression
```

## Comparing `ntscraper-0.1.4.tar` & `ntscraper-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 07:58:58.438847 ntscraper-0.1.4/
--rw-rw-rw-   0        0        0     1091 2023-01-15 20:51:11.000000 ntscraper-0.1.4/LICENSE.txt
--rw-rw-rw-   0        0        0     3485 2023-05-09 07:58:58.436843 ntscraper-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     2559 2023-05-06 07:24:10.000000 ntscraper-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-09 07:58:58.392840 ntscraper-0.1.4/ntscraper/
--rw-rw-rw-   0        0        0       26 2023-01-31 13:55:18.000000 ntscraper-0.1.4/ntscraper/__init__.py
--rw-rw-rw-   0        0        0    27292 2023-05-08 09:45:29.000000 ntscraper-0.1.4/ntscraper/nitter.py
-drwxrwxrwx   0        0        0        0 2023-05-09 07:58:58.434843 ntscraper-0.1.4/ntscraper.egg-info/
--rw-rw-rw-   0        0        0     3485 2023-05-09 07:58:58.000000 ntscraper-0.1.4/ntscraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-05-09 07:58:58.000000 ntscraper-0.1.4/ntscraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 07:58:58.000000 ntscraper-0.1.4/ntscraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-05-09 07:58:58.000000 ntscraper-0.1.4/ntscraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-09 07:58:58.000000 ntscraper-0.1.4/ntscraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-09 07:58:58.438847 ntscraper-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1356 2023-05-08 09:46:48.000000 ntscraper-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 09:58:27.341008 ntscraper-0.1.5/
+-rw-rw-rw-   0        0        0     1091 2023-01-15 20:51:11.000000 ntscraper-0.1.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     3497 2023-07-12 09:58:27.333025 ntscraper-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2571 2023-07-12 09:48:40.000000 ntscraper-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 09:58:27.300998 ntscraper-0.1.5/ntscraper/
+-rw-rw-rw-   0        0        0       26 2023-07-12 09:21:01.000000 ntscraper-0.1.5/ntscraper/__init__.py
+-rw-rw-rw-   0        0        0    27718 2023-07-12 09:46:56.000000 ntscraper-0.1.5/ntscraper/nitter.py
+drwxrwxrwx   0        0        0        0 2023-07-12 09:58:27.333025 ntscraper-0.1.5/ntscraper.egg-info/
+-rw-rw-rw-   0        0        0     3497 2023-07-12 09:58:26.000000 ntscraper-0.1.5/ntscraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-07-12 09:58:27.000000 ntscraper-0.1.5/ntscraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 09:58:26.000000 ntscraper-0.1.5/ntscraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-07-12 09:58:26.000000 ntscraper-0.1.5/ntscraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-12 09:58:27.000000 ntscraper-0.1.5/ntscraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 09:58:27.341008 ntscraper-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1356 2023-07-12 09:48:05.000000 ntscraper-0.1.5/setup.py
```

### Comparing `ntscraper-0.1.4/LICENSE.txt` & `ntscraper-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ntscraper-0.1.4/PKG-INFO` & `ntscraper-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntscraper
-Version: 0.1.4
+Version: 0.1.5
 Summary: Unofficial library to scrape Twitter profiles and posts from Nitter instances
 Author: Lorenzo Bocchi
 Author-email: lorenzobocchi99@yahoo.com
 License: MIT
 Project-URL: Homepage, https://github.com/bocchilorenzo/ntscraper
 Project-URL: Source, https://github.com/bocchilorenzo/ntscraper
 Project-URL: Documentation, https://github.com/bocchilorenzo/ntscraper
@@ -100,8 +100,8 @@
 
 ## Note
 
 Unfortunately, at the moment searching for tweets either via 'term' or 'hashtag' doesn't work because Twitter removed the ability to search without being registered, and as consequence Nitter's search is broken. You can still scrape user profiles.
 
 ## To do list
 
-- [ ] Add scraping of posts and comments
+- [ ] Add scraping of individual posts with comments
```

### Comparing `ntscraper-0.1.4/README.md` & `ntscraper-0.1.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -78,8 +78,8 @@
 
 ## Note
 
 Unfortunately, at the moment searching for tweets either via 'term' or 'hashtag' doesn't work because Twitter removed the ability to search without being registered, and as consequence Nitter's search is broken. You can still scrape user profiles.
 
 ## To do list
 
-- [ ] Add scraping of posts and comments
+- [ ] Add scraping of individual posts with comments
```

### Comparing `ntscraper-0.1.4/ntscraper/nitter.py` & `ntscraper-0.1.5/ntscraper/nitter.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,20 +57,27 @@
 
         :return: list of Nitter instances, or None if lookup failed
         """
         self.r = requests.get("https://github.com/zedeus/nitter/wiki/Instances")
         instance_list = []
         if self.r.ok:
             soup = BeautifulSoup(self.r.text, "lxml")
+            official = soup.find_all("tbody")[0]
+            instance_list.append(official.find("a")["href"])
             table = soup.find_all("tbody")[1]
             for instance in table.find_all("tr"):
-                url = instance.find("a").contents[0]
-                if not url.endswith(".onion"):
-                    url = "https://" + url
-                    instance_list.append(url)
+                columns = instance.find_all("td")
+                if (
+                    columns[1].find("g-emoji") and columns[1].find("g-emoji").get("alias") == "white_check_mark"
+                    ) and (
+                    columns[2].find("g-emoji") and columns[2].find("g-emoji").get("alias") == "white_check_mark"
+                ):
+                    url = instance.find("a")["href"]
+                    if not url.endswith(".onion"):
+                        instance_list.append(url)
             return instance_list
         else:
             return None
 
     def __get_page(self, endpoint, instance, max_retries=5):
         """
         Download page from Nitter instance
```

### Comparing `ntscraper-0.1.4/ntscraper.egg-info/PKG-INFO` & `ntscraper-0.1.5/ntscraper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntscraper
-Version: 0.1.4
+Version: 0.1.5
 Summary: Unofficial library to scrape Twitter profiles and posts from Nitter instances
 Author: Lorenzo Bocchi
 Author-email: lorenzobocchi99@yahoo.com
 License: MIT
 Project-URL: Homepage, https://github.com/bocchilorenzo/ntscraper
 Project-URL: Source, https://github.com/bocchilorenzo/ntscraper
 Project-URL: Documentation, https://github.com/bocchilorenzo/ntscraper
@@ -100,8 +100,8 @@
 
 ## Note
 
 Unfortunately, at the moment searching for tweets either via 'term' or 'hashtag' doesn't work because Twitter removed the ability to search without being registered, and as consequence Nitter's search is broken. You can still scrape user profiles.
 
 ## To do list
 
-- [ ] Add scraping of posts and comments
+- [ ] Add scraping of individual posts with comments
```

### Comparing `ntscraper-0.1.4/setup.py` & `ntscraper-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 HERE = path.abspath(path.dirname(__file__))
 
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="ntscraper",
-    version="0.1.4",
+    version="0.1.5",
     description="Unofficial library to scrape Twitter profiles and posts from Nitter instances",
     long_description=long_description,
     long_description_content_type="text/markdown",
     project_urls={
         'Homepage': 'https://github.com/bocchilorenzo/ntscraper',
         'Source': 'https://github.com/bocchilorenzo/ntscraper',
         'Documentation': 'https://github.com/bocchilorenzo/ntscraper'
```

