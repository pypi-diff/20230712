# Comparing `tmp/Scrapset-3.4.0.tar.gz` & `tmp/Scrapset-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Scrapset-3.4.0.tar", last modified: Sun Jun 25 18:38:20 2023, max compression
+gzip compressed data, was "Scrapset-4.0.0.tar", last modified: Wed Jul 12 16:08:56 2023, max compression
```

## Comparing `Scrapset-3.4.0.tar` & `Scrapset-4.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 18:38:20.479450 Scrapset-3.4.0/
--rw-rw-rw-   0        0        0     4280 2023-06-25 18:38:20.479450 Scrapset-3.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     4049 2023-06-05 16:18:22.000000 Scrapset-3.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-25 18:38:20.471162 Scrapset-3.4.0/Scrapset/
--rw-rw-rw-   0        0        0     6576 2023-06-25 18:37:56.000000 Scrapset-3.4.0/Scrapset/Scrapset.py
--rw-rw-rw-   0        0        0       49 2023-06-06 18:47:28.000000 Scrapset-3.4.0/Scrapset/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 18:38:20.478184 Scrapset-3.4.0/Scrapset.egg-info/
--rw-rw-rw-   0        0        0     4280 2023-06-25 18:38:20.000000 Scrapset-3.4.0/Scrapset.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2023-06-25 18:38:20.000000 Scrapset-3.4.0/Scrapset.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 18:38:20.000000 Scrapset-3.4.0/Scrapset.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-25 18:38:20.000000 Scrapset-3.4.0/Scrapset.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-06-25 18:38:20.000000 Scrapset-3.4.0/Scrapset.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-25 18:38:20.000000 Scrapset-3.4.0/Scrapset.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      632 2023-06-05 15:50:58.000000 Scrapset-3.4.0/licence.txt
--rw-rw-rw-   0        0        0      158 2023-06-25 18:38:20.480501 Scrapset-3.4.0/setup.cfg
--rw-rw-rw-   0        0        0      499 2023-06-25 18:38:10.000000 Scrapset-3.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 16:08:56.616337 Scrapset-4.0.0/
+-rw-rw-rw-   0        0        0     4280 2023-07-12 16:08:56.617535 Scrapset-4.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4049 2023-06-05 16:18:22.000000 Scrapset-4.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 16:08:56.606305 Scrapset-4.0.0/Scrapset/
+-rw-rw-rw-   0        0        0     8754 2023-07-12 16:05:48.000000 Scrapset-4.0.0/Scrapset/Scrapset.py
+-rw-rw-rw-   0        0        0       49 2023-06-06 18:47:28.000000 Scrapset-4.0.0/Scrapset/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 16:08:56.615075 Scrapset-4.0.0/Scrapset.egg-info/
+-rw-rw-rw-   0        0        0     4280 2023-07-12 16:08:56.000000 Scrapset-4.0.0/Scrapset.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-07-12 16:08:56.000000 Scrapset-4.0.0/Scrapset.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 16:08:56.000000 Scrapset-4.0.0/Scrapset.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-25 18:38:20.000000 Scrapset-4.0.0/Scrapset.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-07-12 16:08:56.000000 Scrapset-4.0.0/Scrapset.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-12 16:08:56.000000 Scrapset-4.0.0/Scrapset.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      632 2023-06-05 15:50:58.000000 Scrapset-4.0.0/licence.txt
+-rw-rw-rw-   0        0        0      158 2023-07-12 16:08:56.618753 Scrapset-4.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      499 2023-07-12 16:07:43.000000 Scrapset-4.0.0/setup.py
```

### Comparing `Scrapset-3.4.0/PKG-INFO` & `Scrapset-4.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Scrapset
-Version: 3.4.0
+Version: 4.0.0
 Summary: DataScraper: Effortless Dataset Extraction
 Author: Ibrahim
 Author-email: string2025@gmail.com
 Description-Content-Type: text/markdown
 License-File: licence.txt
 
 # Dataset Scraper (Scrapset)
```

### Comparing `Scrapset-3.4.0/README.md` & `Scrapset-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `Scrapset-3.4.0/Scrapset/Scrapset.py` & `Scrapset-4.0.0/Scrapset/Scrapset.py`

 * *Files 13% similar despite different names*

```diff
@@ -86,15 +86,14 @@
 
 
 class DataDotGov:
     def web_driver_chrome(self):
         options = webdriver.ChromeOptions()
         options.add_argument("--verbose")
         options.add_argument('--no-sandbox')
-        # options.add_argument('--headless')
         options.add_argument('--disable-gpu')
         options.add_argument("--window-size=1920,1200")
         options.add_argument('--disable-dev-shm-usage')
         driver = webdriver.Chrome(options=options)
         return driver
     def data_set_page(self, url, last_page, initial_page):
         try:
@@ -120,7 +119,51 @@
                     list_of_datasets['title'].append( data_set_title)
                     list_of_datasets['recent_views'].append( data_set_views)
                     list_of_datasets['author'].append( data_set_author)
             driver.quit()
             return list_of_datasets
         except:
             logging.error("Invalid Url")
+class indeed:
+    def web_driver_chrome(self):
+        options = webdriver.ChromeOptions()
+        options.add_argument("--verbose")
+        options.add_argument('--no-sandbox')
+        options.add_argument('--disable-gpu')
+        options.add_argument("--window-size=1920,1200")
+        options.add_argument('--disable-dev-shm-usage')
+        driver = webdriver.Chrome(options=options)
+        return driver 
+    def indeed_jobs(self,url,last_page,query):
+        try:
+            driver = self.web_driver_chrome()
+            self.url=url
+            time.sleep(1)
+            list_of_dic = {'title': [],'all_details':[],'salary':[]}  
+            initial_page=0
+            while initial_page < last_page:
+                time.sleep(2)
+                driver.get(url + f'/jobs?q={query}'+f'&start={initial_page}')
+                initial_page+=10
+                cards=driver.find_elements(By.XPATH,'.//*[@id="mosaic-provider-jobcards"]/ul/li/div/div[1]/div/div[1]/div/table[1]/tbody/tr/td/div[1]/h2')
+                details=driver.find_elements(By.XPATH,'.//*[@id="mosaic-provider-jobcards"]/ul/li/div/div[1]/div/div[1]/div/table[1]/tbody/tr/td/div[2]')    
+                salaries=driver.find_elements(By.XPATH,'.//*[@id="mosaic-provider-jobcards"]/ul/li/div/div[1]/div/div[1]/div/table[1]/tbody/tr/td/div[3]/div/div')             
+                for card in cards:
+                        try:
+                                list_of_dic['title'].append(card.text)
+                        except:
+                                list_of_dic['title'].append(" ")
+                for detail in details:
+                        try:
+                                list_of_dic['all_details'].append(detail.text)
+                        except:
+                                list_of_dic['all_details'].append(" ")
+
+                for salary in salaries:
+                        try: 
+                                list_of_dic['salary'].append(salary.text)
+                        except:
+                                list_of_dic['salary'].append(" ")
+            driver.quit()
+            return list_of_dic  
+        except:
+             logging.error("Invalid url")
```

### Comparing `Scrapset-3.4.0/Scrapset.egg-info/PKG-INFO` & `Scrapset-4.0.0/Scrapset.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Scrapset
-Version: 3.4.0
+Version: 4.0.0
 Summary: DataScraper: Effortless Dataset Extraction
 Author: Ibrahim
 Author-email: string2025@gmail.com
 Description-Content-Type: text/markdown
 License-File: licence.txt
 
 # Dataset Scraper (Scrapset)
```

### Comparing `Scrapset-3.4.0/licence.txt` & `Scrapset-4.0.0/licence.txt`

 * *Files identical despite different names*

