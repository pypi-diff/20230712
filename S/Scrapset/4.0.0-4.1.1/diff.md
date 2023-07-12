# Comparing `tmp/Scrapset-4.0.0.tar.gz` & `tmp/Scrapset-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Scrapset-4.0.0.tar", last modified: Wed Jul 12 16:08:56 2023, max compression
+gzip compressed data, was "Scrapset-4.1.1.tar", last modified: Wed Jul 12 16:28:08 2023, max compression
```

## Comparing `Scrapset-4.0.0.tar` & `Scrapset-4.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 16:08:56.616337 Scrapset-4.0.0/
--rw-rw-rw-   0        0        0     4280 2023-07-12 16:08:56.617535 Scrapset-4.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     4049 2023-06-05 16:18:22.000000 Scrapset-4.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 16:08:56.606305 Scrapset-4.0.0/Scrapset/
--rw-rw-rw-   0        0        0     8754 2023-07-12 16:05:48.000000 Scrapset-4.0.0/Scrapset/Scrapset.py
--rw-rw-rw-   0        0        0       49 2023-06-06 18:47:28.000000 Scrapset-4.0.0/Scrapset/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 16:08:56.615075 Scrapset-4.0.0/Scrapset.egg-info/
--rw-rw-rw-   0        0        0     4280 2023-07-12 16:08:56.000000 Scrapset-4.0.0/Scrapset.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2023-07-12 16:08:56.000000 Scrapset-4.0.0/Scrapset.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 16:08:56.000000 Scrapset-4.0.0/Scrapset.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-25 18:38:20.000000 Scrapset-4.0.0/Scrapset.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-07-12 16:08:56.000000 Scrapset-4.0.0/Scrapset.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-12 16:08:56.000000 Scrapset-4.0.0/Scrapset.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      632 2023-06-05 15:50:58.000000 Scrapset-4.0.0/licence.txt
--rw-rw-rw-   0        0        0      158 2023-07-12 16:08:56.618753 Scrapset-4.0.0/setup.cfg
--rw-rw-rw-   0        0        0      499 2023-07-12 16:07:43.000000 Scrapset-4.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-12 16:28:08.810793 Scrapset-4.1.1/
+-rw-rw-rw-   0        0        0     4648 2023-07-12 16:28:08.810793 Scrapset-4.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4417 2023-07-12 16:15:55.000000 Scrapset-4.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-12 16:28:08.798218 Scrapset-4.1.1/Scrapset/
+-rw-rw-rw-   0        0        0     8754 2023-07-12 16:27:13.000000 Scrapset-4.1.1/Scrapset/Scrapset.py
+-rw-rw-rw-   0        0        0       49 2023-06-06 18:47:28.000000 Scrapset-4.1.1/Scrapset/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-12 16:28:08.809809 Scrapset-4.1.1/Scrapset.egg-info/
+-rw-rw-rw-   0        0        0     4648 2023-07-12 16:28:08.000000 Scrapset-4.1.1/Scrapset.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-07-12 16:28:08.000000 Scrapset-4.1.1/Scrapset.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-12 16:28:08.000000 Scrapset-4.1.1/Scrapset.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-12 16:28:08.000000 Scrapset-4.1.1/Scrapset.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-07-12 16:28:08.000000 Scrapset-4.1.1/Scrapset.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-12 16:28:08.000000 Scrapset-4.1.1/Scrapset.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      632 2023-06-05 15:50:58.000000 Scrapset-4.1.1/licence.txt
+-rw-rw-rw-   0        0        0      158 2023-07-12 16:28:08.811791 Scrapset-4.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      499 2023-07-12 16:26:36.000000 Scrapset-4.1.1/setup.py
```

### Comparing `Scrapset-4.0.0/PKG-INFO` & `Scrapset-4.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: Scrapset
-Version: 4.0.0
-Summary: DataScraper: Effortless Dataset Extraction
-Author: Ibrahim
-Author-email: string2025@gmail.com
-Description-Content-Type: text/markdown
-License-File: licence.txt
-
 # Dataset Scraper (Scrapset)
 
 
 
 Scrapset is a Python module specifically created for web scraping data from websites like Kaggle and Data.gov. It simplifies the task of extracting dataset information such as titles, upvotes (for Kaggle), and recent views (for Data.gov).
 
 By utilizing the Scrapset module, you can automate the retrieval of dataset details from these platforms. This can be beneficial for various purposes such as data analysis, research, or developing machine learning models. The module employs the Selenium library to interact with the websites and extract the desired data.
@@ -60,14 +51,27 @@
 data=df.data_set_page('https://kaggle.com',last_page=10,initial_page=5)
 datf=pd.DataFrame(data)
 datf.to_csv('kaggle.csv',index=False)
 
 
 ```
 
+# Example code to extract job details from indeed 
+# You get the details in the form of a dictionary
+There are three arguments in indeed_jobs method 
+First: Url
+Second: last page that you want to scrap the data
+query: what job do you want to scrap
+
+```
+import indeed as in
+dictionary=in()
+data = indeed('https://ie.indeed.com', 40, 'data scientist')
+```
+
 #  Note:  This is for running Scrapset in google colab : 
 
 ```
 
 #run this command in the cell 
 !apt-get update
 !apt-get install chromium  chromium-driver
```

### Comparing `Scrapset-4.0.0/README.md` & `Scrapset-4.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1
+Name: Scrapset
+Version: 4.1.1
+Summary: DataScraper: Effortless Dataset Extraction
+Author: Ibrahim
+Author-email: string2025@gmail.com
+Description-Content-Type: text/markdown
+License-File: licence.txt
+
 # Dataset Scraper (Scrapset)
 
 
 
 Scrapset is a Python module specifically created for web scraping data from websites like Kaggle and Data.gov. It simplifies the task of extracting dataset information such as titles, upvotes (for Kaggle), and recent views (for Data.gov).
 
 By utilizing the Scrapset module, you can automate the retrieval of dataset details from these platforms. This can be beneficial for various purposes such as data analysis, research, or developing machine learning models. The module employs the Selenium library to interact with the websites and extract the desired data.
@@ -51,14 +60,27 @@
 data=df.data_set_page('https://kaggle.com',last_page=10,initial_page=5)
 datf=pd.DataFrame(data)
 datf.to_csv('kaggle.csv',index=False)
 
 
 ```
 
+# Example code to extract job details from indeed 
+# You get the details in the form of a dictionary
+There are three arguments in indeed_jobs method 
+First: Url
+Second: last page that you want to scrap the data
+query: what job do you want to scrap
+
+```
+import indeed as in
+dictionary=in()
+data = indeed('https://ie.indeed.com', 40, 'data scientist')
+```
+
 #  Note:  This is for running Scrapset in google colab : 
 
 ```
 
 #run this command in the cell 
 !apt-get update
 !apt-get install chromium  chromium-driver
```

### Comparing `Scrapset-4.0.0/Scrapset/Scrapset.py` & `Scrapset-4.1.1/Scrapset/Scrapset.py`

 * *Files identical despite different names*

### Comparing `Scrapset-4.0.0/Scrapset.egg-info/PKG-INFO` & `Scrapset-4.1.1/Scrapset.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Scrapset
-Version: 4.0.0
+Version: 4.1.1
 Summary: DataScraper: Effortless Dataset Extraction
 Author: Ibrahim
 Author-email: string2025@gmail.com
 Description-Content-Type: text/markdown
 License-File: licence.txt
 
 # Dataset Scraper (Scrapset)
@@ -60,14 +60,27 @@
 data=df.data_set_page('https://kaggle.com',last_page=10,initial_page=5)
 datf=pd.DataFrame(data)
 datf.to_csv('kaggle.csv',index=False)
 
 
 ```
 
+# Example code to extract job details from indeed 
+# You get the details in the form of a dictionary
+There are three arguments in indeed_jobs method 
+First: Url
+Second: last page that you want to scrap the data
+query: what job do you want to scrap
+
+```
+import indeed as in
+dictionary=in()
+data = indeed('https://ie.indeed.com', 40, 'data scientist')
+```
+
 #  Note:  This is for running Scrapset in google colab : 
 
 ```
 
 #run this command in the cell 
 !apt-get update
 !apt-get install chromium  chromium-driver
```

### Comparing `Scrapset-4.0.0/licence.txt` & `Scrapset-4.1.1/licence.txt`

 * *Files identical despite different names*

