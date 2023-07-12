# Comparing `tmp/anipie-0.0.5.tar.gz` & `tmp/anipie-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anipie-0.0.5.tar", last modified: Sat Oct 29 10:27:29 2022, max compression
+gzip compressed data, was "anipie-0.0.6.tar", last modified: Wed Jul 12 16:52:42 2023, max compression
```

## Comparing `anipie-0.0.5.tar` & `anipie-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,15 @@
-drwxrwxrwx   0        0        0        0 2022-10-29 10:27:29.534364 anipie-0.0.5/
--rw-rw-rw-   0        0        0     1089 2022-10-16 04:28:16.000000 anipie-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      460 2022-10-29 10:27:29.533367 anipie-0.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-10-29 10:27:29.501452 anipie-0.0.5/anipie/
--rw-rw-rw-   0        0        0       86 2022-10-28 16:45:06.000000 anipie-0.0.5/anipie/__init__.py
--rw-rw-rw-   0        0        0     2836 2022-10-28 16:59:30.000000 anipie-0.0.5/anipie/searchAnime.py
--rw-rw-rw-   0        0        0     2863 2022-10-28 16:57:43.000000 anipie-0.0.5/anipie/searchManga.py
--rw-rw-rw-   0        0        0     1384 2022-10-28 16:49:35.000000 anipie-0.0.5/anipie/testDataFuntion.py
--rw-rw-rw-   0        0        0       95 2022-10-28 17:00:10.000000 anipie-0.0.5/anipie/testdata.py
-drwxrwxrwx   0        0        0        0 2022-10-29 10:27:29.532370 anipie-0.0.5/anipie.egg-info/
--rw-rw-rw-   0        0        0      460 2022-10-29 10:27:28.000000 anipie-0.0.5/anipie.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2022-10-29 10:27:29.000000 anipie-0.0.5/anipie.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-29 10:27:28.000000 anipie-0.0.5/anipie.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2022-10-29 10:27:29.000000 anipie-0.0.5/anipie.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-10-29 10:27:29.000000 anipie-0.0.5/anipie.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-10-29 10:27:29.534364 anipie-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      588 2022-10-29 10:27:15.000000 anipie-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 16:52:42.758591 anipie-0.0.6/
+-rw-rw-rw-   0        0        0     1089 2023-07-12 10:40:29.000000 anipie-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      410 2023-07-12 16:52:42.758591 anipie-0.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-12 16:52:42.742477 anipie-0.0.6/anipie/
+-rw-rw-rw-   0        0        0       76 2023-07-12 16:32:59.000000 anipie-0.0.6/anipie/__init__.py
+-rw-rw-rw-   0        0        0     2820 2023-07-12 16:33:05.000000 anipie-0.0.6/anipie/searchAnime.py
+-rw-rw-rw-   0        0        0     2855 2023-07-12 16:33:10.000000 anipie-0.0.6/anipie/searchManga.py
+drwxrwxrwx   0        0        0        0 2023-07-12 16:52:42.757545 anipie-0.0.6/anipie.egg-info/
+-rw-rw-rw-   0        0        0      410 2023-07-12 16:52:42.000000 anipie-0.0.6/anipie.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      228 2023-07-12 16:52:42.000000 anipie-0.0.6/anipie.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 16:52:42.000000 anipie-0.0.6/anipie.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-12 16:52:42.000000 anipie-0.0.6/anipie.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-12 16:52:42.000000 anipie-0.0.6/anipie.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-12 16:52:42.758591 anipie-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      588 2023-07-12 16:49:14.000000 anipie-0.0.6/setup.py
```

### Comparing `anipie-0.0.5/LICENSE` & `anipie-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `anipie-0.0.5/anipie/searchAnime.py` & `anipie-0.0.6/anipie/searchAnime.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import re
 import requests
 
+
 class SearchAnime:
 
-    def __init__(self, search):
-        self.search = search
+    def __init__(self, title):
+        self.title = title
         self.animeSearch()
 
-
     def animeSearch(self):
         self.query = '''
         query ($search: String! $type: MediaType!) { 
             Media (search: $search type: $type) { 
                 id
                 title {
                     romaji
@@ -38,62 +38,62 @@
                 episodes
                 season
                 format
             }
         }
         '''
         self.variables = {
-            'search' : self.search,
-            'type' : 'ANIME',
+            'search': self.title,
+            'type': 'ANIME',
         }
         self.url = 'https://graphql.anilist.co'
-        self.response = requests.post(self.url, json={'query': self.query, 'variables': self.variables})
+        self.response = requests.post(
+            self.url, json={'query': self.query, 'variables': self.variables})
         self.response = self.response.json()
         self.Media = self.response.get('data').get('Media')
 
     def getAnimeData(self):
         return self.response
 
     def getAnimeRomajiName(self):
         return self.Media.get('title').get('romaji')
 
     def getAnimeEnglishName(self):
         return self.Media.get('title').get('english')
-    
+
     def getAnimeStatus(self):
         return self.Media.get('status')
-    
+
     def getAnimeDescription(self):
         des = self.Media.get('description')
-        return  re.sub(re.compile('<.*?>') , '', des)
-    
+        return re.sub(re.compile('<.*?>'), '', des)
+
     def getAnimeEpisodes(self):
         return self.Media.get('episodes')
 
     def getAnimeCoverImage(self):
         return self.Media.get('coverImage').get('large')
-    
+
     def getAnimeGenres(self):
         return ", ".join(self.Media.get('genres'))
-    
+
     def getAnimeSiteUrl(self):
         return self.Media.get('siteUrl')
 
     def getAnimeStartDate(self):
         esd = self.Media.get('startDate')
         return str(esd.get('month')) + '/' + str(esd.get('day')) + '/' + str(esd.get('year'))
 
     def getAnimeEndDate(self):
         exp = self.Media.get('endDate')
         return str(exp.get('month')) + '/' + str(exp.get('day')) + '/' + str(exp.get('year'))
 
     def getAnimeAverageScore(self):
         return int(self.Media.get('averageScore'))/10
 
-
     def getAnimeSeason(self):
         return self.Media.get('season')
 
     def getAnimeFormat(self):
         return self.Media.get('format')
 
     def getAnimeID(self):
```

### Comparing `anipie-0.0.5/anipie/searchManga.py` & `anipie-0.0.6/anipie/searchManga.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import requests
 import re
 
+
 class SearchManga:
-    
-    def __init__(self, search):
-        self.search = search
+
+    def __init__(self, title):
+        self.title = title
         self.response = None
         self.mangaSearch()
 
     def mangaSearch(self):
         self.query = '''
         query ($search: String! $type: MediaType!) { 
             Media (search: $search type: $type) { 
@@ -38,53 +39,53 @@
                 chapters
                 volumes
                 format
             }
         }
         '''
         self.variables = {
-            'search' : self.search,
-            'type' : 'MANGA',
+            'search': self.title,
+            'type': 'MANGA',
         }
         self.url = 'https://graphql.anilist.co'
-        self.response = requests.post(self.url, json={'query': self.query, 'variables': self.variables})
+        self.response = requests.post(
+            self.url, json={'query': self.query, 'variables': self.variables})
         self.response = self.response.json()
         self.Media = self.response.get('data').get('Media')
 
     def getMangaData(self):
         return self.response
 
     def getMangaRomajiName(self):
         return self.Media.get('title').get('romaji')
-    
+
     def getMangaEnglishName(self):
         return self.Media.get('title').get('english')
 
     def getMangaStatus(self):
         return self.Media.get('status')
-    
+
     def getMangaDescription(self):
         des = self.Media.get('description')
-        return  re.sub(re.compile('<.*?>') , '', des)
-
+        return re.sub(re.compile('<.*?>'), '', des)
 
     def getMangaStartDate(self):
         esd = self.Media.get('startDate')
         return str(esd.get('month')) + '/' + str(esd.get('day')) + '/' + str(esd.get('year'))
 
     def getMangaEndDate(self):
         exp = self.Media.get('endDate')
         return str(exp.get('month')) + '/' + str(exp.get('day')) + '/' + str(exp.get('year'))
 
     def getMangaCoverImage(self):
         return self.Media.get('coverImage').get('large')
 
     def getMangaGenres(self):
         return ", ".join(self.Media.get('genres'))
-    
+
     def getMangaSiteUrl(self):
         return self.Media.get('siteUrl')
 
     def getMangaVolumes(self):
         return self.Media.get('volumes')
 
     def getMangaChapters(self):
@@ -93,8 +94,8 @@
     def getMangaAverageScore(self):
         return int(self.Media.get('averageScore')) / 10
 
     def getMangaFormat(self):
         return self.Media.get('format')
 
     def getMangaID(self):
-        return self.Media.get('id')
+        return self.Media.get('id')
```

### Comparing `anipie-0.0.5/setup.py` & `anipie-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 
 setuptools.setup(
     name="anipie", 
-    version="0.0.5",
+    version="0.0.6",
     author="Aritsu",
     author_email="lynniswaifu@gmail.com",
     description="a simple python wrapper for the Anilist API",
     long_description="",
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

